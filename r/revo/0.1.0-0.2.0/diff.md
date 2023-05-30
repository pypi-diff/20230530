# Comparing `tmp/revo-0.1.0-py3-none-any.whl.zip` & `tmp/revo-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3688 bytes, number of entries: 7
+Zip file size: 6476 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       24 b- defN 23-May-29 11:26 revo/__init__.py
--rw-r--r--  2.0 unx     4924 b- defN 23-May-29 11:25 revo/_revo.py
--rw-r--r--  2.0 unx     1068 b- defN 23-May-29 12:30 revo-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      541 b- defN 23-May-29 12:30 revo-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-29 12:30 revo-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-May-29 12:30 revo-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      510 b- defN 23-May-29 12:30 revo-0.1.0.dist-info/RECORD
-7 files, 7164 bytes uncompressed, 2788 bytes compressed:  61.1%
+-rw-r--r--  2.0 unx     5476 b- defN 23-May-30 05:57 revo/_revo.py
+-rw-r--r--  2.0 unx     1068 b- defN 23-May-30 07:02 revo-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     6600 b- defN 23-May-30 07:02 revo-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-30 07:02 revo-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-May-30 07:02 revo-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      511 b- defN 23-May-30 07:02 revo-0.2.0.dist-info/RECORD
+7 files, 13776 bytes uncompressed, 5576 bytes compressed:  59.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: revo/__init__.py
 Comment: 
 
 Filename: revo/_revo.py
 Comment: 
 
-Filename: revo-0.1.0.dist-info/LICENSE
+Filename: revo-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: revo-0.1.0.dist-info/METADATA
+Filename: revo-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: revo-0.1.0.dist-info/WHEEL
+Filename: revo-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: revo-0.1.0.dist-info/top_level.txt
+Filename: revo-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: revo-0.1.0.dist-info/RECORD
+Filename: revo-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## revo/_revo.py

```diff
@@ -76,79 +76,101 @@
     if isinstance(obj, dict):
         for key, val in obj.items():
             for k, v in _revo_melt(val):
                 yield (f'{key}/{k}', v) if k else (key, val)
     elif isinstance(obj, list):
         for idx, val in enumerate(obj):
             for k, v in _revo_melt(val):
-                yield (f'{idx}/{k}', v) if k else (key, val)
+                yield (f'{idx}/{k}', v) if k else (str(idx), val)
     else:
         yield (None, obj)
 
 
 class Revo(MutableMapping):
-    def __init__(self, obj, overrides=None, *, mercy=True, merge_defs=False):
+
+    def __init__(self, obj, overrides=None, *,
+                 mercy=False, absorb=False, retain=True):
         self.val = obj
         if not isinstance(obj, (list, dict)):
             raise TypeError('Only list or dict object allowed')
+
+        self.mercy  = mercy   # allow unresolved or illegal references
+        self.absorb = absorb  # merge definitions into the tree
+        self.retain = retain  # try to keep reference value type
+
+        # top-level overrides not found in original object are definitions
+        self.defs = []
+
         if overrides:
-            self.resolve(overrides, mercy=mercy, merge_defs=merge_defs)
+            self.resolve(overrides)
 
 
-    def melt(self):
-        return _revo_melt(self.val)
+    def override(self, spec):
+        for key, val in _parse_overrides(spec).items():
+            # treat new top-level keys as definitions
+            if '/' not in key and key not in self.val:
+                self.val[key] = val
+                if not self.absorb:
+                    self.defs.append(key)
+            else:
+                self[key] = val
 
+        return self
 
-    def resolve(self, override_spec=None, *, mercy=True, merge_defs=False):
-        # top-level overrides not found in original object are definitions
-        defs = []
 
+    def resolve(self, override_spec=None):
         # apply overrides
         if override_spec:
-            for key, val in _parse_overrides(override_spec).items():
-                # treat new top-level keys as definitions
-                if '/' not in key and key not in self.val:
-                    self.val[key] = val
-                    if not merge_defs:
-                        defs.append(key)
-                else:
-                    self[key] = val
+            self.override(override_spec)
 
-        # resolve value references
-        flat = {key: str(val) for key, val in self.melt()}
-        while any('$(' in val for val in flat.values()):
+        # resolve value references bottom-up
+        flat = {key: val for key, val in self.melt()}
+        while any('$(' in str(val) for val in flat.values()):
             subs = list(flat.keys())
             changed = 0
             for sub in subs:
+                var = f'$({sub})'
                 for key, val in flat.items():
-                    if f'$({sub})' in val:
+                    val = str(val)
+                    if var in val:
                         if key == sub:
+                            if self.mercy:
+                                continue
                             raise ValueError(f'self-reference of {sub}')
                         changed += 1
-                        self[key] = val.replace(f'$({sub})', flat[sub])
+                        if self.retain and val == var:
+                            self[key] = flat[sub]
+                        else:
+                            self[key] = val.replace(var, str(flat[sub]))
             if not changed:
                 break
-            flat = {key: str(val) for key, val in self.melt()}
+            flat = {key: val for key, val in self.melt()}
 
         # remove definitions
-        for key in defs:
+        for key in self.defs:
             del self[key]
 
         # mercy on unresolved or illegal references?
-        if not mercy:
+        if not self.mercy:
             for key, val in self.melt():
-                if '$(' not in val:
+                if '$(' not in str(val):
                     continue
                 mo = re.search(r'(\$\(.+\))', val)
                 if not mo:
                     err = f'illegal reference "{val}" (from {key})'
                 else:
                     err = f'reference {mo.group(1)} unresolved (from {key})'
                 raise ValueError(err)
 
+        return self
+
+
+    def melt(self):
+        return _revo_melt(self.val)
+
 
     def __getitem__(self, key): return _revo_get(self.val, key)
     def __setitem__(self, key, val): _revo_set(self.val, key, val)
     def __delitem__(self, key): _revo_del(self.val, key)
     def __iter__(self): return iter(self.val)
     def __len__(self): return len(self.val)
     def __str__(self): return str(self.val)
```

## Comparing `revo-0.1.0.dist-info/LICENSE` & `revo-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

