# Comparing `tmp/sypht-0.5.8.tar.gz` & `tmp/sypht-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sypht-0.5.8.tar", last modified: Wed Jun 23 01:05:10 2021, max compression
+gzip compressed data, was "dist/sypht-0.5.9.tar", last modified: Wed Jun 23 03:27:21 2021, max compression
```

## Comparing `sypht-0.5.8.tar` & `sypht-0.5.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-23 01:05:10.000000 sypht-0.5.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2293 2021-06-23 01:04:47.000000 sypht-0.5.8/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      570 2021-06-23 01:04:47.000000 sypht-0.5.8/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1070 2021-06-23 01:04:47.000000 sypht-0.5.8/LICENSE
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-23 01:05:10.000000 sypht-0.5.8/sypht.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2021-06-23 01:05:10.000000 sypht-0.5.8/sypht.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       20 2021-06-23 01:05:10.000000 sypht-0.5.8/sypht.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      353 2021-06-23 01:05:10.000000 sypht-0.5.8/sypht.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-06-23 01:05:10.000000 sypht-0.5.8/sypht.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       47 2021-06-23 01:05:10.000000 sypht-0.5.8/sypht.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      254 2021-06-23 01:05:10.000000 sypht-0.5.8/sypht.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-06-23 01:05:10.000000 sypht-0.5.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      353 2021-06-23 01:05:10.000000 sypht-0.5.8/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-23 01:05:10.000000 sypht-0.5.8/sypht/
--rw-rw-r--   0 travis    (2000) travis    (2000)    24954 2021-06-23 01:04:47.000000 sypht-0.5.8/sypht/client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1935 2021-06-23 01:04:47.000000 sypht-0.5.8/sypht/__main__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-06-23 01:04:47.000000 sypht-0.5.8/sypht/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-23 03:27:21.000000 sypht-0.5.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2293 2021-06-23 03:26:59.000000 sypht-0.5.9/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      570 2021-06-23 03:26:59.000000 sypht-0.5.9/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1070 2021-06-23 03:26:59.000000 sypht-0.5.9/LICENSE
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-23 03:27:21.000000 sypht-0.5.9/sypht.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        6 2021-06-23 03:27:21.000000 sypht-0.5.9/sypht.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       20 2021-06-23 03:27:21.000000 sypht-0.5.9/sypht.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      353 2021-06-23 03:27:21.000000 sypht-0.5.9/sypht.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-06-23 03:27:21.000000 sypht-0.5.9/sypht.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       47 2021-06-23 03:27:21.000000 sypht-0.5.9/sypht.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      254 2021-06-23 03:27:21.000000 sypht-0.5.9/sypht.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2021-06-23 03:27:21.000000 sypht-0.5.9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      353 2021-06-23 03:27:21.000000 sypht-0.5.9/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-06-23 03:27:21.000000 sypht-0.5.9/sypht/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25375 2021-06-23 03:26:59.000000 sypht-0.5.9/sypht/client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1935 2021-06-23 03:26:59.000000 sypht-0.5.9/sypht/__main__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2021-06-23 03:26:59.000000 sypht-0.5.9/sypht/__init__.py
```

### Comparing `sypht-0.5.8/README.md` & `sypht-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `sypht-0.5.8/setup.py` & `sypht-0.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-__version__ = "0.5.8"
+__version__ = "0.5.9"
 __pkg_name__ = "sypht"
 
 setup(
     name=__pkg_name__,
     version=__version__,
     description="Sypht Python Client",
     author="Sypht Pty Ltd.",
```

### Comparing `sypht-0.5.8/LICENSE` & `sypht-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sypht-0.5.8/sypht/client.py` & `sypht-0.5.9/sypht/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -506,23 +506,36 @@
         params = {}
         if page:
             params["page"] = page
         if limit:
             params["limit"] = int(limit)
         return self._parse_response(self.requests.get(endpoint, headers=headers, params=params))
 
-    def get_all_entity_ids(self, entity_type, company_id=None, endpoint=None):
+    def get_all_entity_ids(self, entity_type, verbose=True, company_id=None, endpoint=None):
+        """Get all entity_ids for specified entity_type.
+
+        Returns list of objects if verbose (by default):
+        [{"entity_id": "id_0"}, {"entity_id": "id_1"}, ...]
+
+        Returns list of entity_id if not verbose:
+        ["id_0", "id_1", ...]
+        """
         entity_ids = []
         next_page = True
         while next_page:
             if next_page is True:
                 next_page = None  # first page request
             res = self.list_entities(entity_type, company_id, page=next_page)
             next_page = res.get("next_page")
-            entity_ids.extend([{"entity_id": entity_id} for entity_id in res.get("entities")])
+            if verbose:
+                entity_ids.extend(
+                    [{"entity_id": entity_id} for entity_id in res.get("entities")]
+                )
+            else:
+                entity_ids.extend(res.get("entities"))
         return entity_ids
 
     def set_entity(self, entity_id, entity_type, data, company_id=None, endpoint=None):
         company_id = company_id or self.company_id
         entity_id = quote_plus(entity_id)
         entity_type = quote_plus(entity_type)
         endpoint = urljoin(
```

### Comparing `sypht-0.5.8/sypht/__main__.py` & `sypht-0.5.9/sypht/__main__.py`

 * *Files identical despite different names*

