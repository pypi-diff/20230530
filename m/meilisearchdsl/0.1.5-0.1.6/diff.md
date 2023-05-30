# Comparing `tmp/meilisearchdsl-0.1.5.tar.gz` & `tmp/meilisearchdsl-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meilisearchdsl-0.1.5.tar", last modified: Tue Apr 11 16:15:17 2023, max compression
+gzip compressed data, was "meilisearchdsl-0.1.6.tar", last modified: Tue May 30 09:20:00 2023, max compression
```

## Comparing `meilisearchdsl-0.1.5.tar` & `meilisearchdsl-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:15:17.052399 meilisearchdsl-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-11 16:15:01.000000 meilisearchdsl-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-11 16:15:17.052399 meilisearchdsl-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-11 16:15:01.000000 meilisearchdsl-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:15:17.052399 meilisearchdsl-0.1.5/meilisearchdsl/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-11 16:15:01.000000 meilisearchdsl-0.1.5/meilisearchdsl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-04-11 16:15:01.000000 meilisearchdsl-0.1.5/meilisearchdsl/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22432 2023-04-11 16:15:01.000000 meilisearchdsl-0.1.5/meilisearchdsl/index.py
--rw-r--r--   0 runner    (1001) docker     (123)    10865 2023-04-11 16:15:01.000000 meilisearchdsl-0.1.5/meilisearchdsl/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-04-11 16:15:01.000000 meilisearchdsl-0.1.5/meilisearchdsl/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 16:15:17.052399 meilisearchdsl-0.1.5/meilisearchdsl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-04-11 16:15:17.000000 meilisearchdsl-0.1.5/meilisearchdsl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-11 16:15:17.000000 meilisearchdsl-0.1.5/meilisearchdsl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 16:15:17.000000 meilisearchdsl-0.1.5/meilisearchdsl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-11 16:15:17.000000 meilisearchdsl-0.1.5/meilisearchdsl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-11 16:15:17.000000 meilisearchdsl-0.1.5/meilisearchdsl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 16:15:17.052399 meilisearchdsl-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-04-11 16:15:08.000000 meilisearchdsl-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:20:00.416088 meilisearchdsl-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-30 09:19:44.000000 meilisearchdsl-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-30 09:20:00.416088 meilisearchdsl-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-30 09:19:44.000000 meilisearchdsl-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:20:00.416088 meilisearchdsl-0.1.6/meilisearchdsl/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-30 09:19:44.000000 meilisearchdsl-0.1.6/meilisearchdsl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-05-30 09:19:44.000000 meilisearchdsl-0.1.6/meilisearchdsl/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24104 2023-05-30 09:19:44.000000 meilisearchdsl-0.1.6/meilisearchdsl/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-30 09:19:44.000000 meilisearchdsl-0.1.6/meilisearchdsl/index_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10865 2023-05-30 09:19:44.000000 meilisearchdsl-0.1.6/meilisearchdsl/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-05-30 09:19:44.000000 meilisearchdsl-0.1.6/meilisearchdsl/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:20:00.416088 meilisearchdsl-0.1.6/meilisearchdsl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-05-30 09:20:00.000000 meilisearchdsl-0.1.6/meilisearchdsl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-30 09:20:00.000000 meilisearchdsl-0.1.6/meilisearchdsl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 09:20:00.000000 meilisearchdsl-0.1.6/meilisearchdsl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 09:20:00.000000 meilisearchdsl-0.1.6/meilisearchdsl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-30 09:20:00.000000 meilisearchdsl-0.1.6/meilisearchdsl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 09:20:00.416088 meilisearchdsl-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-30 09:19:51.000000 meilisearchdsl-0.1.6/setup.py
```

### Comparing `meilisearchdsl-0.1.5/LICENSE` & `meilisearchdsl-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `meilisearchdsl-0.1.5/PKG-INFO` & `meilisearchdsl-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meilisearchdsl
-Version: 0.1.5
+Version: 0.1.6
 Summary: MeiliSearch DSL is a Python package providing a Django-like Q object syntax for querying MeiliSearch, an open-source search engine. It simplifies search query building and offers a convenient wrapper for MeiliSearch indexes and clients, streamlining search interactions and improving maintainability.
 Home-page: https://github.com/UnattendedFlight/meilisearch-dsl
 Author: Adrian Leo
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `meilisearchdsl-0.1.5/README.md` & `meilisearchdsl-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `meilisearchdsl-0.1.5/meilisearchdsl/client.py` & `meilisearchdsl-0.1.6/meilisearchdsl/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """MeiliClient is a wrapper around the MeiliSearch client. It provides a
 simple interface to create indexes and add documents to them. It also
 provides a simple interface to delete indexes and documents from them.
 """
 from typing import Dict, List
 
 from meilisearch import Client
-from .index import Index
+from meilisearch.index import Index
 
 from .index import MeiliIndex
 
 
 class MeiliClient:
     """MeiliClient is a wrapper around the MeiliSearch client. It provides a
     simple interface to create indexes and add documents to them. It also
```

### Comparing `meilisearchdsl-0.1.5/meilisearchdsl/index.py` & `meilisearchdsl-0.1.6/meilisearchdsl/index.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,58 +1,57 @@
 # pylint: disable=W0719,C0103,R0904,E1131,import-error
 """Index Module"""
 from time import sleep
 from typing import Any, Dict, List, Optional, Union
 
 import meilisearch
-from meilisearch.errors import MeiliSearchApiError
+from meilisearch.errors import MeilisearchApiError
 from meilisearch.index import Index
 from meilisearch.models.task import TaskInfo, Task
 
 from .query import Q
 
 
 class MeiliIndex:
     """MeiliIndex class."""
 
     def __init__(self, index_name: str, client: meilisearch.Client, primary_key: str):
         self.index_name = index_name
         self.client: meilisearch.Client = client
         try:
             self._index: Index = self.get_index(index_name, primary_key)
-        except Exception:
+        except MeilisearchApiError:
             self._index: Index = self.create_index(index_name, primary_key)
 
     def get_index(
         self,
         index_name: str,
         primary_key: Optional[str] = None,
         options: Union[Dict[str, Any], None] = None,
     ) -> Index:
         """Get an index from Meilisearch."""
         assert self.client is not None, "No Meilisearch client"
         try:
             self._index = self.client.get_index(index_name)
-        except Exception:
+        except MeilisearchApiError:
             index_options = {}
             if options is not None:
-                assert isinstance(
-                    options, dict), "Options must be a dictionary"
+                assert isinstance(options, dict), "Options must be a dictionary"
             if primary_key is not None:
                 index_options["primaryKey"] = primary_key
             if options is not None:
                 index_options.update(options)
 
             self._call_long_index_method(
                 self.client.create_index, index_name, index_options
             )
 
             self._index = self.client.get_index(index_name)
         return self._index
-    
+
     def create_index(
         self,
         index_name: str,
         primary_key: Optional[str] = None,
         options: Union[Dict[str, Any], None] = None,
     ) -> Index:
         """Create an index in Meilisearch."""
@@ -68,15 +67,17 @@
         self._call_long_index_method(
             self.client.create_index, index_name, index_options
         )
 
         self._index = self.client.get_index(index_name)
         return self._index
 
-    def update_filterable_attributes(self, attributes: List[str]) -> Union[TaskInfo, Task]:
+    def update_filterable_attributes(
+        self, attributes: List[str]
+    ) -> Union[TaskInfo, Task]:
         """Update filterable attributes of the index.
 
         Parameters
         ----------
         body:
             List containing the filterable attributes.
 
@@ -120,15 +121,17 @@
             An error containing details about why Meilisearch can't process your request.
             Meilisearch error codes are described here:
             https://docs.meilisearch.com/errors/#meilisearch-errors
         """
         assert self._index is not None, "No Meilisearch index"
         return self._index.update_filterable_attributes(attributes)
 
-    def update_searchable_attributes(self, attributes: List[str]) -> Union[TaskInfo, Task]:
+    def update_searchable_attributes(
+        self, attributes: List[str]
+    ) -> Union[TaskInfo, Task]:
         """Update searchable attributes of the index.
 
         Parameters
         ----------
         body:
             List containing the searchable attributes.
 
@@ -172,15 +175,17 @@
             An error containing details about why Meilisearch can't process your request.
             Meilisearch error codes are described here:
             https://docs.meilisearch.com/errors/#meilisearch-errors
         """
         assert self._index is not None, "No Meilisearch index"
         return self._index.update_searchable_attributes(attributes)
 
-    def update_displayed_attributes(self, attributes: List[str]) -> Union[TaskInfo, Task]:
+    def update_displayed_attributes(
+        self, attributes: List[str]
+    ) -> Union[TaskInfo, Task]:
         """Update displayed attributes of the index.
 
         Parameters
         ----------
         body:
             List containing the displayed attributes.
 
@@ -199,14 +204,54 @@
             https://docs.meilisearch.com/errors/#meilisearch-errors
         """
         assert self._index is not None, "No Meilisearch index"
         return self._call_long_index_method(
             self._index.update_displayed_attributes, attributes
         )
 
+    def update_sortable_attributes(
+        self, attributes: List[str]
+    ) -> Union[TaskInfo, Task]:
+        """Update sortable attributes of the index.
+
+        Parameters
+        ----------
+        body:
+            List containing the sortable attributes.
+
+        Returns
+        -------
+        task_info:
+            TaskInfo instance containing information about a task to track
+            the progress of an asynchronous process.
+            https://docs.meilisearch.com/reference/api/tasks.html
+        """
+        assert self._index is not None, "No Meilisearch index"
+        return self._call_long_index_method(
+            self._index.update_sortable_attributes, attributes
+        )
+
+    def aupdate_sortable_attributes(self, attributes: List[str]) -> TaskInfo:
+        """Update sortable attributes of the index.
+
+        Parameters
+        ----------
+        body:
+            List containing the sortable attributes.
+
+        Returns
+        -------
+        task_info:
+            TaskInfo instance containing information about a task to track
+            the progress of an asynchronous process.
+            https://docs.meilisearch.com/reference/api/tasks.html
+        """
+        assert self._index is not None, "No Meilisearch index"
+        return self._index.update_sortable_attributes(attributes)
+
     def aupdate_displayed_attributes(self, attributes: List[str]) -> TaskInfo:
         """Update displayed attributes of the index.
 
         Parameters
         ----------
         body:
             List containing the displayed attributes.
@@ -588,29 +633,39 @@
     ) -> Dict[str, Any]:
         """Search for documents in the index."""
         search_params = {}
         if q is not None:
             assert isinstance(q, Q), "q must be a Q object"
             search_params["filter"] = q.to_query_string()
         if opt_params is not None:
-            assert isinstance(
-                opt_params, dict), "opt_params must be a dictionary"
+            assert isinstance(opt_params, dict), "opt_params must be a dictionary"
             search_params.update(opt_params)
 
         return self._index.search(search_string, search_params)
 
+    def multisearch(
+        self,
+        index_queries: List[IndexSearch],
+    ):
+        """Search for documents in multiple indexes."""
+        return self.client.http.post(
+            f"{self.client.config.paths.multi_search}",
+            body={"queries": [q.query() for q in index_queries]},
+        )
+
     def _await_running_task(self, task_info: TaskInfo) -> Any:
         """Wait for a task to complete and return the task info object."""
         complete = False
         timeout_seconds = 10
         count = 0
         while not complete:
             if count > timeout_seconds:
                 print(
-                    f"Task '{task_info['type']}:{task_info['taskUid']}'", # type: ignore
+                    # type: ignore
+                    f"Task '{task_info.type}:{task_info.task_uid}'",
                     f"timed out after {timeout_seconds} seconds",
                 )
                 break
             task = self.client.get_task(task_info.task_uid)
             if task["status"] == "succeeded":
                 return task
             if task["status"] == "failed":
```

### Comparing `meilisearchdsl-0.1.5/meilisearchdsl/query.py` & `meilisearchdsl-0.1.6/meilisearchdsl/query.py`

 * *Files identical despite different names*

### Comparing `meilisearchdsl-0.1.5/meilisearchdsl/test.py` & `meilisearchdsl-0.1.6/meilisearchdsl/test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 """ Basic tests for the MeiliSearch DSL """
 import unittest
 
-from meilisearchdsl.client import MeiliClient
-from meilisearchdsl.query import Q
+# from meilisearchdsl.client import MeiliClient
+from .client import MeiliClient
+
+# from meilisearchdsl.query import Q
+from .query import Q
+from .index_query import IndexSearch
 
 
 class TestQAndMeiliIndex(unittest.TestCase):
     """Test the Q object and MeiliIndex class"""
 
     def setUp(self):
         # print("Running test:", self._testMethodName)
         self.client = MeiliClient(
-            "http://172.25.0.4:7700", "MJPZij#@4o$NgYIRwxoU2aa^CUq9%5Lq"
+            "ip", "master-key"
         )
-        self.index = self.client.get_index("test_index")
+        self.index = self.client.get_index("test_index", "pk")
         self.index.delete_all_documents()
         self.index.add_documents(
             [
                 {
-                    "id": 1,
+                    "pk": 1,
                     "name": "John Simmons",
                     "age": 28,
                     "number": 12,
                     "category": "a",
                 },
-                {"id": 2, "name": "Alice", "age": 21, "number": 15, "category": "b"},
-                {"id": 3, "name": "Bob", "age": 35, "number": 22, "category": "c"},
-                {"id": 4, "name": "Alice", "age": 35, "number": 15, "category": "b"},
-                {"id": 5, "name": "Alice", "age": 19, "number": 25, "category": "a"},
+                {"pk": 2, "name": "Alice", "age": 21, "number": 15, "category": "b"},
+                {"pk": 3, "name": "Bob", "age": 35, "number": 22, "category": "c"},
+                {"pk": 4, "name": "Alice", "age": 35, "number": 15, "category": "b"},
+                {"pk": 5, "name": "Alice", "age": 19, "number": 25, "category": "a"},
             ]
         )
         self.index.update_filterable_attributes(["name", "age", "number", "category"])
+        self.index.update_sortable_attributes(["age"])
 
     def test_q_negation(self):
         """Test the negation of Q objects"""
         query = ~Q(name="John Simmons")
         query_string = query.to_query_string()
         self.assertEqual(query_string, 'name != "John Simmons"')
 
@@ -79,18 +84,18 @@
         results = self.index.search("", q_filter)
         self.assertEqual(len(results["hits"]), 3)
 
     def test_update_document(self):
         """Test the update_document method of MeiliIndex"""
         self.index.update_document(
             {
-                "id": 1,
+                "pk": 1,
                 "name": "Johnathan",
             },
-            "id",
+            "pk",
         )
         query = Q(name="John")
         results = self.index.search("", query)
         self.assertEqual(len(results["hits"]), 0)
 
         results = self.index.search("", Q(name="Johnathan"))
         self.assertEqual(len(results["hits"]), 1)
@@ -109,10 +114,48 @@
     def test_delete_all_documents(self):
         """Test the delete_all_documents method of MeiliIndex"""
         self.index.delete_all_documents()
         query = Q(name="John")
         results = self.index.search("", query)
         self.assertEqual(len(results["hits"]), 0)
 
+    def test_multi_search(self):
+        """Test the multisearch method of MeiliIndex"""
+        index_search = IndexSearch(self.index.index_name, "John")
+        index_search.filter(Q(age__gt=19)).retrieve_attributes(
+            ["name", "age"]
+        ).highlight_attributes(["name"]).facets(["category"]).limit(
+            2
+        ).show_matches_position(
+            True
+        ).sort(
+            ["age:asc"]
+        )
+        self.assertEqual(
+            index_search.query(),
+            {
+                "indexUid": "test_index",
+                "q": "John",
+                "filter": "age > 19",
+                "limit": 2,
+                "facets": ["category"],
+                "attributesToRetrieve": ["name", "age"],
+                "attributesToHighlight": ["name"],
+                "showMatchesPosition": True,
+                "sort": ["age:asc"],
+            },
+        )
+        response = self.index.multisearch([index_search])
+        self.assertEqual(
+            response["results"][0]["hits"][0]["_formatted"]["name"],
+            "<em>John</em> Simmons",
+        )
+        self.assertEqual(
+            response["results"][0]["hits"][0]["_matchesPosition"]["name"],
+            [{"start": 0, "length": 4}],
+        )
+        self.assertEqual(response["results"][0]["hits"][0]["age"], 28)
+        self.assertEqual(response["results"][0]["hits"][0]["_formatted"]["age"], "28")
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `meilisearchdsl-0.1.5/meilisearchdsl.egg-info/PKG-INFO` & `meilisearchdsl-0.1.6/meilisearchdsl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meilisearchdsl
-Version: 0.1.5
+Version: 0.1.6
 Summary: MeiliSearch DSL is a Python package providing a Django-like Q object syntax for querying MeiliSearch, an open-source search engine. It simplifies search query building and offers a convenient wrapper for MeiliSearch indexes and clients, streamlining search interactions and improving maintainability.
 Home-page: https://github.com/UnattendedFlight/meilisearch-dsl
 Author: Adrian Leo
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `meilisearchdsl-0.1.5/setup.py` & `meilisearchdsl-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # pylint: disable=missing-docstring, invalid-name, line-too-long, R1732
 from setuptools import setup, find_packages
 
 setup(
     name="meilisearchdsl",
-    version="0.1.5",
+    version="0.1.6",
     description="MeiliSearch DSL is a Python package providing a Django-like Q object syntax for"
     + " querying MeiliSearch, an open-source search engine."
     + " It simplifies search query building and offers a convenient wrapper"
     + " for MeiliSearch indexes and clients, streamlining search interactions"
     + " and improving maintainability.",
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
@@ -22,10 +22,10 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
     ],
     install_requires=[
         # List your package's dependencies here
-        "meilisearch>=0.25.0",
+        "meilisearch==0.26.0",
     ],
 )
```

