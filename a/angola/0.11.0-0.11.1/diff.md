# Comparing `tmp/angola-0.11.0.tar.gz` & `tmp/angola-0.11.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angola-0.11.0.tar", last modified: Mon May 29 09:34:25 2023, max compression
+gzip compressed data, was "angola-0.11.1.tar", last modified: Tue May 30 04:56:37 2023, max compression
```

## Comparing `angola-0.11.0.tar` & `angola-0.11.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-29 09:34:25.240895 angola-0.11.0/
--rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-21 05:31:22.000000 angola-0.11.0/LICENSE
--rw-r--r--   0 mardix     (501) staff       (20)       26 2022-11-28 18:23:44.000000 angola-0.11.0/MANIFEST.in
--rw-r--r--   0 mardix     (501) staff       (20)     1257 2023-05-29 09:34:25.240975 angola-0.11.0/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      877 2022-11-30 18:28:40.000000 angola-0.11.0/README.md
--rw-r--r--   0 mardix     (501) staff       (20)       79 2023-05-29 09:34:25.241246 angola-0.11.0/setup.cfg
--rw-r--r--   0 mardix     (501) staff       (20)      799 2023-05-29 09:33:29.000000 angola-0.11.0/setup.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-29 09:34:25.235483 angola-0.11.0/src/
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-29 09:34:25.238486 angola-0.11.0/src/angola/
--rw-r--r--   0 mardix     (501) staff       (20)      314 2023-04-30 19:58:20.000000 angola-0.11.0/src/angola/__init__.py
--rw-r--r--   0 mardix     (501) staff       (20)    48031 2023-05-08 02:57:37.000000 angola-0.11.0/src/angola/database.py
--rw-r--r--   0 mardix     (501) staff       (20)    13959 2023-05-29 06:51:31.000000 angola-0.11.0/src/angola/dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)    18847 2023-02-21 03:11:29.000000 angola-0.11.0/src/angola/dict_query.py
--rw-r--r--   0 mardix     (501) staff       (20)    16742 2023-03-08 03:08:31.000000 angola-0.11.0/src/angola/lib.py
--rw-r--r--   0 mardix     (501) staff       (20)    16737 2023-05-29 09:32:03.000000 angola-0.11.0/src/angola/lib_xql.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-29 09:34:25.239141 angola-0.11.0/src/angola.egg-info/
--rw-r--r--   0 mardix     (501) staff       (20)     1257 2023-05-29 09:34:25.000000 angola-0.11.0/src/angola.egg-info/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      464 2023-05-29 09:34:25.000000 angola-0.11.0/src/angola.egg-info/SOURCES.txt
--rw-r--r--   0 mardix     (501) staff       (20)        1 2023-05-29 09:34:25.000000 angola-0.11.0/src/angola.egg-info/dependency_links.txt
--rw-r--r--   0 mardix     (501) staff       (20)       59 2023-05-29 09:34:25.000000 angola-0.11.0/src/angola.egg-info/requires.txt
--rw-r--r--   0 mardix     (501) staff       (20)        7 2023-05-29 09:34:25.000000 angola-0.11.0/src/angola.egg-info/top_level.txt
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-29 09:34:25.240779 angola-0.11.0/tests/
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 angola-0.11.0/tests/test_cursor.py
--rw-r--r--   0 mardix     (501) staff       (20)      716 2022-11-28 18:20:13.000000 angola-0.11.0/tests/test_database.py
--rw-r--r--   0 mardix     (501) staff       (20)     1184 2022-11-28 18:20:13.000000 angola-0.11.0/tests/test_dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)     3301 2022-06-29 07:01:37.000000 angola-0.11.0/tests/test_lib.py
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 angola-0.11.0/tests/test_query.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-30 04:56:37.566597 angola-0.11.1/
+-rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-21 05:31:22.000000 angola-0.11.1/LICENSE
+-rw-r--r--   0 mardix     (501) staff       (20)       26 2022-11-28 18:23:44.000000 angola-0.11.1/MANIFEST.in
+-rw-r--r--   0 mardix     (501) staff       (20)     1257 2023-05-30 04:56:37.566666 angola-0.11.1/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      877 2022-11-30 18:28:40.000000 angola-0.11.1/README.md
+-rw-r--r--   0 mardix     (501) staff       (20)       79 2023-05-30 04:56:37.566915 angola-0.11.1/setup.cfg
+-rw-r--r--   0 mardix     (501) staff       (20)      799 2023-05-30 04:55:50.000000 angola-0.11.1/setup.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-30 04:56:37.561551 angola-0.11.1/src/
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-30 04:56:37.564200 angola-0.11.1/src/angola/
+-rw-r--r--   0 mardix     (501) staff       (20)      314 2023-04-30 19:58:20.000000 angola-0.11.1/src/angola/__init__.py
+-rw-r--r--   0 mardix     (501) staff       (20)    48027 2023-05-30 03:49:44.000000 angola-0.11.1/src/angola/database.py
+-rw-r--r--   0 mardix     (501) staff       (20)    13959 2023-05-29 06:51:31.000000 angola-0.11.1/src/angola/dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)    18847 2023-02-21 03:11:29.000000 angola-0.11.1/src/angola/dict_query.py
+-rw-r--r--   0 mardix     (501) staff       (20)    16742 2023-03-08 03:08:31.000000 angola-0.11.1/src/angola/lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)    18685 2023-05-30 04:36:37.000000 angola-0.11.1/src/angola/lib_xql.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-30 04:56:37.565050 angola-0.11.1/src/angola.egg-info/
+-rw-r--r--   0 mardix     (501) staff       (20)     1257 2023-05-30 04:56:37.000000 angola-0.11.1/src/angola.egg-info/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      464 2023-05-30 04:56:37.000000 angola-0.11.1/src/angola.egg-info/SOURCES.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        1 2023-05-30 04:56:37.000000 angola-0.11.1/src/angola.egg-info/dependency_links.txt
+-rw-r--r--   0 mardix     (501) staff       (20)       59 2023-05-30 04:56:37.000000 angola-0.11.1/src/angola.egg-info/requires.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        7 2023-05-30 04:56:37.000000 angola-0.11.1/src/angola.egg-info/top_level.txt
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-30 04:56:37.566484 angola-0.11.1/tests/
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 angola-0.11.1/tests/test_cursor.py
+-rw-r--r--   0 mardix     (501) staff       (20)      716 2022-11-28 18:20:13.000000 angola-0.11.1/tests/test_database.py
+-rw-r--r--   0 mardix     (501) staff       (20)     1184 2022-11-28 18:20:13.000000 angola-0.11.1/tests/test_dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)     3301 2022-06-29 07:01:37.000000 angola-0.11.1/tests/test_lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 angola-0.11.1/tests/test_query.py
```

### Comparing `angola-0.11.0/LICENSE` & `angola-0.11.1/LICENSE`

 * *Files identical despite different names*

### Comparing `angola-0.11.0/PKG-INFO` & `angola-0.11.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angola
-Version: 0.11.0
+Version: 0.11.1
 Summary: angola 
 Home-page: https://github.com/mardix/angola
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
```

### Comparing `angola-0.11.0/README.md` & `angola-0.11.1/README.md`

 * *Files identical despite different names*

### Comparing `angola-0.11.0/setup.py` & `angola-0.11.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 
 def long_description():
     with open('README.md', 'r') as file:
         return file.read()
 
-VERSION = "0.11.0"
+VERSION = "0.11.1"
 setuptools.setup(
     name='angola',
     version=VERSION,
     author='Mardix',
     author_email='mardix@blackdevhub.io',
     description='angola ',
     long_description=long_description(),
```

### Comparing `angola-0.11.0/src/angola/database.py` & `angola-0.11.1/src/angola/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -366,15 +366,15 @@
             data that was removed        
         """
         op = "%s:$xpopl" % self._make_path(path)
         oplog = self._update({op: True})
         return oplog.get(op)
 
     def timestamp(self, path:str, value:Any=True):
-        op = "%s:$timestamp" % self._make_path(path)
+        op = "%s:$datetime" % self._make_path(path)
         oplog = self._update({op: value})
         return oplog.get(op)   
 
     def template(self, path:str, value:str):
         op = "%s:$template" % self._make_path(path)
         oplog = self._update({op: value})
         return oplog.get(op)
@@ -629,15 +629,15 @@
         Params:
             - nattime:str - Natural time - ie 1hour, 60seconds
 
         Returns:
             self
         """
         if isinstance(nattime, str):
-            self.update({"__ttl:$timestamp": nattime})
+            self.update({"__ttl:$datetime": nattime})
         elif nattime is False:
             self.update({"__ttl": None})
         return self
 
     def delete(self) -> bool:
         """
         To delete an item
@@ -1520,26 +1520,26 @@
     return "edges__%s--%s" % (from_name, to_name)
 
 def _create_document_item(data:dict={}) -> dict:
     _key = data["_key"] if "_key" in data else lib.gen_key()
 
     return {
         "_key": _key,
-        "_created_at:$timestamp": True,
+        "_created_at:$datetime": True,
         "_modified_at": None,
         "__ttl": None,
         **data,
     }
 
 def _create_subdocument_item(data:dict={}) -> dict:
     _key = data["_key"] if "_key" in data else lib.gen_key()
 
     return {
         "_key": _key,
-        "_created_at:$timestamp": True,
+        "_created_at:$datetime": True,
         "_modified_at": None,
         **data,
     }
 
 def _ascdesc(v, as_str=True):
     if as_str:
         if isinstance(v, int):
```

### Comparing `angola-0.11.0/src/angola/dict_mutator.py` & `angola-0.11.1/src/angola/dict_mutator.py`

 * *Files identical despite different names*

### Comparing `angola-0.11.0/src/angola/dict_query.py` & `angola-0.11.1/src/angola/dict_query.py`

 * *Files identical despite different names*

### Comparing `angola-0.11.0/src/angola/lib.py` & `angola-0.11.1/src/angola/lib.py`

 * *Files identical despite different names*

### Comparing `angola-0.11.0/src/angola/lib_xql.py` & `angola-0.11.1/src/angola/lib_xql.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,71 +2,56 @@
 # -- Angola --
 # -----------------------------
 
 import re
 from slugify import slugify
 from . import lib
 
-# === AQL Functions
-# -----------------------------------------------------------------------------
-
-AQL_FILTER_LOGIC = {
-    "$AND": " AND ",
-    "$OR": " OR ",
-    "$NOT": " NOT ",
-    "$NOR": " NOR "
-}
 
-# AQL UTILITIES
-AQL_FILTER_OPERATORS = {
-    "$EQ": "==",  # equal
-    "$NE": "!=",  # not equal
-    "$GT": ">",  # greater than
-    "$GTE": ">=",  # greater than or equal
-    "$LT": "<",  # lesser than
-    "$LTE": "<=",  # lesser than or equal
-
-    # INCLUDES + XINCLUDES
-    # Test if data in RIGHT(string|int) is in data in LEFT(array)
-    # ie: "__subcollections.something[*].value:$INCLUDES": "my-value"
-    # --> "my-value" IN __subcollections.something[*].value 
-    "$INCLUDES": "IN",
-    "$XINCLUDES": "NOT IN",
-
-    # IN + NIN
-    # reverse the order of INCLUDES
-    # To test if data in (LEFT:str|int) is in the (RIGHT:array)
-    # ie "city:$IN": ["charlotte", "atlanta"]
-    # --> u.city IN ["charlotte", "atlanta"]
-    "$IN": "IN",
-    "$XIN": "NOT IN",
+# -----------------------------------------------------------------------------
+# === XQLDEFINITION -----------------------------------------------------------
 
+class XQLDEFINITION:
+    """
+    XQL Schema Definition:
 
-    # LIKE + NOTLIKE
-    # right hand in left hand array -> values IN [field.value]
-    "$LIKE": "LIKE",  # search
-    "$NLIKE": "NOT LIKE",  # 
-    #TODO:
-    # == for case insensitive ==
-    # "$ILIKE": "",
-    # "$NILIKE": ""
-}
-# reverse operator, where the right hand will point to left hand
-# ie: cities:$INCLUDES: 'charlotte' -> 'charlotte' IN cities
-_rev_ops_order = ['$INCLUDES', '$XINCLUDES']
+        :param FROM: str = the collection name
+        :param ALIAS: str = alias
+        :param FILTERS: dict = filters
+        :param SORT: list/str = sort 
+        :param OFFSET: int = the offset of the limit, default=0
+        :param LIMIT: int = the limit of result, default=10
+        :param PAGE: int = help calculate the skip by using a page number. 
+        :param JOIN: list[XQL]
+        :param COUNT_AS: str =  To count all the document, and return the value. Alias to `COLLECT WITH COUNT INTO`
+        :param RETURN: str = string representation
+        :param MERGE: str = on JOIN, to merge the data.
+            ie: MERGE: "{__profile: profile}" 
+            Can be done manually with RETURN MERGE(doc, {data})
 
+    """
+    FROM: str = None
+    ALIAS: str = None
+    FILTERS: dict = {}
+    SORT: list = []
+    OFFSET: int = 0
+    LIMIT: int = 10
+    PAGE: int = 1
+    JOIN: list = []
+    COUNT_AS: str = None
+    RETURN: str = None
+    MERGE: str = None
 
 
 # -----------------------------------------------------------------------------
 # === MACROS ------------------------------------------------------------------
 
 def _re_match(pattern, value) -> re:
     return re.match(pattern, value, flags=re.IGNORECASE)
 
-
 def _macro_now(re_match:re):
     """
     This macro eval the NOW|DATETIME in the query
     
     :Params:
         :re_match: regexp match the 
 
@@ -91,15 +76,14 @@
         dt_format = dt_format.strip()
 
     now = lib.get_datetime()
     if shifter:
         now = lib.arrow_date_shifter(now, shifter)
     return now.format(dt_format )
 
-
 MACROS_DEFS = [
     {
         # [[@MACRO:NOW, +2Days, YYYY-MM-DD HH:mm:ss]]
         "name": "NOW",
         "pattern": "^\[\[\@MACRO:NOW\s*,?\s*(.*)]]$",
         "func": _macro_now
     }
@@ -110,58 +94,151 @@
     for item in MACROS_DEFS:
         if isinstance(value, str) and (m := _re_match(item.get("pattern"), value)):
             return item.get("func")(m)
         elif isinstance(value, list):
             return [eval_macros(v) for v in value]
     return value
 
+
 # -----------------------------------------------------------------------------
-# -----------------------------------------------------------------------------
+# === QUERY OPERATORS ---------------------------------------------------------
+
+AQL_FILTER_LOGIC = {
+    "$AND": " AND ",
+    "$OR": " OR ",
+    "$NOT": " NOT ",
+    "$NOR": " NOR "
+}
+
+# AQL UTILITIES
+AQL_FILTER_OPERATORS = {
+    "_": None, # Not an operator
+
+    "$EQ": "==",  # equal
+    "$NE": "!=",  # not equal
+    "$GT": ">",  # greater than
+    "$GTE": ">=",  # greater than or equal
+    "$LT": "<",  # lesser than
+    "$LTE": "<=",  # lesser than or equal
+    #?$BETWEEN: LOGIC IMPLEMENTED IN CODE
+
+
+    # INCLUDES + XINCLUDES
+    # Test if data in RIGHT(string|int) is in data in LEFT(array)
+    # ie: "__subcollections.something[*].value:$INCLUDES": "my-value"
+    # --> "my-value" IN __subcollections.something[*].value 
+    "$INCLUDES": "IN",
+    "$XINCLUDES": "NOT IN",
+
+    # IN + NIN
+    # reverse the order of INCLUDES
+    # To test if data in (LEFT:str|int) is in the (RIGHT:array)
+    # ie "city:$IN": ["charlotte", "atlanta"]
+    # --> u.city IN ["charlotte", "atlanta"]
+    "$IN": "IN",
+    "$XIN": "NOT IN",
 
 
-def aql_sort_builder(sorts: list, propkey: str) -> str:
+    # LIKE + NOTLIKE
+    # right hand in left hand array -> values IN [field.value]
+    "$LIKE": "LIKE",  # search
+    "$NLIKE": "NOT LIKE",  # 
+
+    # "$CONTAINS": "" # will turn into 
+    # must return a tuple of [statement:str, dict:{value, ...}]
+    "$CONTAINS": lambda odict: ("{propkey}.{key} LIKE @{ukey}", {**odict, "value": "%{value}%".format(value=odict.get("value"))}),
+    "$XCONTAINS": lambda odict: ("{propkey}.{key} NOT LIKE @{ukey}", {**odict, "value": "%{value}%".format(value=odict.get("value"))}),
+
+    #TODO:
+    # == for case insensitive ==
+    # "$ILIKE": "",
+    # "$NILIKE": ""
+}
+# reverse operator, where the right hand will point to left hand
+# ie: cities:$INCLUDES: 'charlotte' -> 'charlotte' IN cities
+_rev_ops_order = ['$INCLUDES', '$XINCLUDES']
+
+
+def filter_builder(filters: dict, propkey: str) -> tuple:
     """
-    Create a SORT clause
+    Create a FILTERS clause
 
-    Params
-        sorts: list
-            ["name:desc", "id:asc", "some.deep.path:desc"]
-            alternative to list, it can be string
-                sorts: "name:desc"
-                sorts: "name" // will be ASC by default
+    Params:
+        filter: dict
+            {
+                'name': 'something',
+                'age:$gt': 18,
+                'cities:$in': ['charlotte', 'Concord'],
+                'date:$between:["[[@MACRO:NOW, -2Days]]", "[[@MACRO:NOW, -1Days]]"],
+                
+                # Logical Operators 
+                == as a dict, it will make the comparison between the values, by turning it into dict
+                '$or': {
+                    key1: v1,
+                    key2: v2
+                }, #-> [{key1: v1}, {key2: v2}]
+
+                == as list, it will group all the dict with AND and create OR between
+                '$or': [
+                    {
+                       "cities:$in": [],
+                       "_perms.read:$in":[] 
+                    }, 
+                    {
+                        "k2": v2,
+                        "k3": v3
+                    }
+                 ]
+                ]
+            }
         propkey:str
             the property key from the parent query
-    Returns
-        str
-    """
-    if not sorts:
-        return ""
 
-    # you can pass it as string
-    # sorts: "name"
-    if isinstance(sorts, str):
-        sorts = [sorts]
-    # make compatible with previous implementations.
-    # sorts must now be a list, not dict.
-    elif isinstance(sorts, dict):
-        sorts = ["%s:%s" % (k, v) for k, v in sorts.items()]
-
-    aql = ["%s.%s %s" % (propkey, s.split(":")[0], s.split(
-        ":")[1] if len(s.split(":")) > 1 else "ASC") for s in sorts]
-    return " SORT " + ", ".join(aql) + " "
+    Returns
+        tuple(aql:str, params:dict)
 
+    """
+    logical_keys = AQL_FILTER_LOGIC.keys()
+    params = {}
+    aql = ""
+    for k in filters:
 
-def xql_collects_builder(collects: list, propkey: str) -> str:
-    if not collects:
-        return ""
-    # TODO
-    return ""
+        #* LOGICAL OPERATION
+        if k.startswith("$"):
+            k_ = k.upper()
+            # operation
+            if k_ in logical_keys and isinstance(filters[k], (dict, list)):
+                fk = filters[k]
+                _logic_op = AQL_FILTER_LOGIC[k_]
+                _and_op = AQL_FILTER_LOGIC["$AND"]
+                
+                # A flat dict will turn into a list dict to apply OR on all 
+                if isinstance(fk, dict):
+                    fk = [{_1:_2} for _1, _2 in fk.items()]
+                
+                logic_aql = []
+                for k0 in fk:
+                    tmp_aql = []
+                    for k2 in k0:
+                        _aql, _params = _parse_filter_row(k2, k0[k2], propkey)
+                        tmp_aql.append(_aql)
+                        params.update(_params)
+                    logic_aql.append("\n(%s)" % _and_op.join(tmp_aql))
+                aql += "FILTER (%s)\n" % _logic_op.join(logic_aql)
+            else:
+                raise Exception("INVALID_LOGIC_OPERATOR: %s" % k)
+        
+        else:
+            _aql, _params = _parse_filter_row(k, filters[k], propkey)
+            aql += "FILTER (%s)\n" % _aql
+            params.update(_params)
+    return aql, params
 
 
-def _parse_filter_row(k, value, propkey):
+def _parse_filter_row(k, value, propkey) -> tuple:
     operator = "$EQ"  # default operator
     # extract the key and the operator
     # ie -> "name:$eq" or "city:$in"
     # link#, especially in join: "'name': '#parent.key'"
 
     if ":" in k:
         k, operator = k.split(":", 2)
@@ -177,105 +254,107 @@
 
     # gen a unique number to make sure values generated are unique
     num_ = lib.gen_number(6)
     ukey = slugify("%s_%s" % (k, num_), separator="_")
     stmt = ""
     params = {}
     value = eval_macros(value=value)
+
     if dlit:
         value = value.replace("#", "")
         if operator in _rev_ops_order:  # reverse order
             stmt = " {value} {operator} {propkey}.{key}"
         else:
             stmt = " {propkey}.{key} {operator} {value}"
+    
+    # between -> $gte and $lte
+    elif operator == "$BETWEEN":
+        if not isinstance(value, list) or len(value) != 2:
+            raise Exception("INVALID_DATA_TYPE_FOR_BETWEEN")
+        gte = slugify("%s_gte_%s" % (k, num_), separator="_")
+        lte = slugify("%s_lte_%s" % (k, num_), separator="_")
+        stmt = " {propkey}.{key} >= @%s AND <= @%s" % (gte, lte)
+        operator = "_" 
+        params = {
+            gte: value[0],
+            lte: value[1],
+        }
+
     else:
         params = {
             ukey: value
         }
         if operator in _rev_ops_order:  # reverse order
             stmt = " @{ukey} {operator} {propkey}.{key}"
+            
+        elif callable(AQL_FILTER_OPERATORS.get(operator)):
+            """
+            An operator can be callable function that accepts a DICT of data as first arg
+            and must return a 
+                -> tuple(stmt:str, data:dict)
+
+            ie:
+                "$CONTAINS": lambda odict: ("{propkey}.{key} LIKE @{ukey}", {**odict, "value": "%{value}%".format(value=odict.get("value"))})
+            
+            """
+            stmt, odict = AQL_FILTER_OPERATORS.get(operator)({"value": value})
+            params = {
+                ukey: odict.get("value")
+            }
+            operator = "_"
         else:
             stmt = " {propkey}.{key} {operator} @{ukey}"
 
     aql = stmt.format(
         value=value,
         propkey=propkey,
         key=k,
         operator=AQL_FILTER_OPERATORS[operator],
         ukey=ukey)
 
     return aql, params
 
 
-def aql_filter_builder(filters: dict, propkey: str) -> tuple:
+def sort_builder(sorts: list, propkey: str) -> str:
     """
-    Create a FILTERS clause
+    Create a SORT clause
 
-    Params:
-        filter: dict
-            {
-                'name': 'something',
-                'age:$gt': 18,
-                'cities:$in': ['charlotte', 'Concord'],
-                '$or': [{
-                       "cities:$in": [],
-                       "_perms.read:$in":[] 
-                 }]
-                ]
-            }
+    Params
+        sorts: list
+            ["name:desc", "id:asc", "some.deep.path:desc"]
+            alternative to list, it can be string
+                sorts: "name:desc"
+                sorts: "name" // will be ASC by default
         propkey:str
             the property key from the parent query
-
     Returns
-        tuple(aql:str, params:dict)
-
+        str
     """
-    params = {}
-    aql = ""
-    for k in filters:
+    if not sorts:
+        return ""
 
-        if k.startswith("$"):
-            k_ = k.upper()
-            # operation
-            if k_ in AQL_FILTER_LOGIC.keys() and isinstance(filters[k], (dict, list)):
-                fk = filters[k]
-                if isinstance(fk, dict):
-                    fk = [fk]
-                for k0 in fk:
-                    tmp_aql = []
-                    for k2 in k0:
-                        _aql, _params = _parse_filter_row(k2, k0[k2], propkey)
-                        tmp_aql.append(_aql)
-                        params.update(_params)
-                    aql += "FILTER (%s)\n" % AQL_FILTER_LOGIC[k_].join(tmp_aql)
-            else:
-                raise Exception("Invalid logic: %s" % k)
-        else:
-            _aql, _params = _parse_filter_row(k, filters[k], propkey)
-            aql += "FILTER (%s)\n" % _aql
-            params.update(_params)
-        # value = filters[k]
-        # operator = "$EQ"  # default operator
+    # you can pass it as string
+    # sorts: "name"
+    if isinstance(sorts, str):
+        sorts = [sorts]
+    # make compatible with previous implementations.
+    # sorts must now be a list, not dict.
+    elif isinstance(sorts, dict):
+        sorts = ["%s:%s" % (k, v) for k, v in sorts.items()]
 
-        # # extract the key and the operator
-        # # ie -> "name:$eq" or "city:$in"
-        # if ":" in k:
-        #     k, operator = k.split(":", 2)
-        #     operator = operator.upper()
-
-        # # gen a unique number to make sure values generated are unique
-        # num_ = lib.gen_number(6)
-        # ukey = "%s_%s" % (k, num_)
-        # aql += " FILTER {propkey}.{key} {operator} @{ukey} \n".format(
-        #     propkey=propkey,
-        #     key=k,
-        #     operator=AQL_FILTER_OPERATORS[operator],
-        #     ukey=ukey)
-        # params[ukey] = value
-    return aql, params
+    aql = ["%s.%s %s" % (propkey, s.split(":")[0], s.split(
+        ":")[1] if len(s.split(":")) > 1 else "ASC") for s in sorts]
+    return " SORT " + ", ".join(aql) + " "
+
+
+def collects_builder(collects: list, propkey: str) -> str:
+    if not collects:
+        return ""
+    # TODO
+    return ""
 
 
 def prepare_xql(xql: dict) -> dict:
     _defaults = {
         "FROM": None,
         "ALIAS": "root__",
         "FILTERS": {},
@@ -317,46 +396,14 @@
         LIMIT = per_page
     if LIMIT > max_limit:
         LIMIT = max_limit
 
     return LIMIT, OFFSET, PAGE
 
 
-class XQLDEFINITION:
-    """
-    XQL Schema Definition:
-
-        :param FROM: str = the collection name
-        :param ALIAS: str = alias
-        :param FILTERS: dict = filters
-        :param SORT: list/str = sort 
-        :param OFFSET: int = the offset of the limit, default=0
-        :param LIMIT: int = the limit of result, default=10
-        :param PAGE: int = help calculate the skip by using a page number. 
-        :param JOIN: list[XQL]
-        :param COUNT_AS: str =  To count all the document, and return the value. Alias to `COLLECT WITH COUNT INTO`
-        :param RETURN: str = string representation
-        :param MERGE: str = on JOIN, to merge the data.
-            ie: MERGE: "{__profile: profile}" 
-            Can be done manually with RETURN MERGE(doc, {data})
-
-    """
-    FROM: str = None
-    ALIAS: str = None
-    FILTERS: dict = {}
-    SORT: list = []
-    OFFSET: int = 0
-    LIMIT: int = 10
-    PAGE: int = 1
-    JOIN: list = []
-    COUNT_AS: str = None
-    RETURN: str = None
-    MERGE: str = None
-
-
 def xql_to_aql(xql: dict, vars: dict = {}, max_limit=100, parser=None):
     """
     XQL:=
     Xtensible Query Language to query data in ArangoDB 
 
     Params:
         xql: 
@@ -477,28 +524,26 @@
     COUNT_AS = xql.get("COUNT_AS")
     COLLECTS = xql.get("COLLECT") or []
     RETURN = xql.get("RETURN") or ALIAS
 
     # work with take/skip
     if OFFSET is None:
         page = PAGE or 1
-        per_page = LIMIT
-        if per_page > max_limit:
-            per_page = max_limit
+        per_page = max_limit if per_page > max_limit else LIMIT
         OFFSET = lib.calc_pagination_offset(page=page, per_page=per_page)
         LIMIT = per_page
     if LIMIT > max_limit:
         LIMIT = max_limit
 
 
     # unique num to give each field to prevent name collision
     num_ = lib.gen_number(6)
-    aql_filter, filter_vars = aql_filter_builder(FILTERS, propkey=ALIAS)
-    aql_sorting = aql_sort_builder(SORTS, propkey=ALIAS)
-    aql_collects = xql_collects_builder(COLLECTS, propkey=ALIAS)
+    aql_filter, filter_vars = filter_builder(FILTERS, propkey=ALIAS)
+    aql_sorting = sort_builder(SORTS, propkey=ALIAS)
+    aql_collects = collects_builder(COLLECTS, propkey=ALIAS)
     if COUNT_AS:
         aql_collects += " COLLECT WITH COUNT INTO %s " % COUNT_AS
 
     bind_vars = {}
 
     # SUBQUERY/JOINS
     subquery = ""
```

### Comparing `angola-0.11.0/src/angola.egg-info/PKG-INFO` & `angola-0.11.1/src/angola.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angola
-Version: 0.11.0
+Version: 0.11.1
 Summary: angola 
 Home-page: https://github.com/mardix/angola
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
```

### Comparing `angola-0.11.0/tests/test_database.py` & `angola-0.11.1/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `angola-0.11.0/tests/test_dict_mutator.py` & `angola-0.11.1/tests/test_dict_mutator.py`

 * *Files identical despite different names*

### Comparing `angola-0.11.0/tests/test_lib.py` & `angola-0.11.1/tests/test_lib.py`

 * *Files identical despite different names*

