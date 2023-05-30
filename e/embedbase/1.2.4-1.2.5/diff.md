# Comparing `tmp/embedbase-1.2.4.tar.gz` & `tmp/embedbase-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedbase-1.2.4.tar", max compression
+gzip compressed data, was "embedbase-1.2.5.tar", max compression
```

## Comparing `embedbase-1.2.4.tar` & `embedbase-1.2.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1069 2023-05-30 12:20:15.030939 embedbase-1.2.4/LICENSE
--rw-r--r--   0        0        0     4931 2023-05-30 12:20:15.030939 embedbase-1.2.4/README.md
--rw-r--r--   0        0        0      121 2023-05-30 12:20:15.174954 embedbase-1.2.4/embedbase/__init__.py
--rw-r--r--   0        0        0     1716 2023-05-30 12:20:15.174954 embedbase-1.2.4/embedbase/__main__.py
--rw-r--r--   0        0        0      416 2023-05-30 12:20:15.174954 embedbase-1.2.4/embedbase/api.py
--rw-r--r--   0        0        0    21232 2023-05-30 12:20:15.174954 embedbase-1.2.4/embedbase/app.py
--rw-r--r--   0        0        0       88 2023-05-30 12:20:15.174954 embedbase-1.2.4/embedbase/database/__init__.py
--rw-r--r--   0        0        0     3920 2023-05-30 12:20:15.174954 embedbase-1.2.4/embedbase/database/base.py
--rw-r--r--   0        0        0     6962 2023-05-30 12:20:15.174954 embedbase-1.2.4/embedbase/database/memory_db.py
--rw-r--r--   0        0        0    11071 2023-05-30 12:20:15.174954 embedbase-1.2.4/embedbase/database/postgres_db.py
--rw-r--r--   0        0        0     8873 2023-05-30 12:20:15.174954 embedbase-1.2.4/embedbase/database/supabase_db.py
--rw-r--r--   0        0        0       77 2023-05-30 12:20:15.174954 embedbase-1.2.4/embedbase/embedding/__init__.py
--rw-r--r--   0        0        0      858 2023-05-30 12:20:15.174954 embedbase-1.2.4/embedbase/embedding/base.py
--rw-r--r--   0        0        0     1237 2023-05-30 12:20:15.174954 embedbase-1.2.4/embedbase/embedding/cohere.py
--rw-r--r--   0        0        0     2059 2023-05-30 12:20:15.174954 embedbase-1.2.4/embedbase/embedding/openai.py
--rw-r--r--   0        0        0     1551 2023-05-30 12:20:15.174954 embedbase-1.2.4/embedbase/firebase_auth.py
--rw-r--r--   0        0        0      690 2023-05-30 12:20:15.174954 embedbase-1.2.4/embedbase/logging_utils.py
--rw-r--r--   0        0        0     1313 2023-05-30 12:20:15.174954 embedbase-1.2.4/embedbase/models.py
--rw-r--r--   0        0        0     1245 2023-05-30 12:20:15.174954 embedbase-1.2.4/embedbase/settings.py
--rw-r--r--   0        0        0     3208 2023-05-30 12:20:15.174954 embedbase-1.2.4/embedbase/strings.py
--rw-r--r--   0        0        0      301 2023-05-30 12:20:15.174954 embedbase-1.2.4/embedbase/supabase_auth.py
--rw-r--r--   0        0        0     3867 2023-05-30 12:20:15.174954 embedbase-1.2.4/embedbase/utils.py
--rw-r--r--   0        0        0     3730 2023-05-30 12:20:15.178954 embedbase-1.2.4/pyproject.toml
--rw-r--r--   0        0        0     6363 1970-01-01 00:00:00.000000 embedbase-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-30 12:49:44.775864 embedbase-1.2.5/LICENSE
+-rw-r--r--   0        0        0     4931 2023-05-30 12:49:44.775864 embedbase-1.2.5/README.md
+-rw-r--r--   0        0        0      121 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/__init__.py
+-rw-r--r--   0        0        0     1716 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/__main__.py
+-rw-r--r--   0        0        0      416 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/api.py
+-rw-r--r--   0        0        0    21232 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/app.py
+-rw-r--r--   0        0        0       88 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/database/__init__.py
+-rw-r--r--   0        0        0     3920 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/database/base.py
+-rw-r--r--   0        0        0     6962 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/database/memory_db.py
+-rw-r--r--   0        0        0    11071 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/database/postgres_db.py
+-rw-r--r--   0        0        0     9430 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/database/supabase_db.py
+-rw-r--r--   0        0        0       77 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/embedding/__init__.py
+-rw-r--r--   0        0        0      858 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/embedding/base.py
+-rw-r--r--   0        0        0     1237 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/embedding/cohere.py
+-rw-r--r--   0        0        0     2059 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/embedding/openai.py
+-rw-r--r--   0        0        0     1551 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/firebase_auth.py
+-rw-r--r--   0        0        0      690 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/logging_utils.py
+-rw-r--r--   0        0        0     1313 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/models.py
+-rw-r--r--   0        0        0     1245 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/settings.py
+-rw-r--r--   0        0        0     3208 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/strings.py
+-rw-r--r--   0        0        0      301 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/supabase_auth.py
+-rw-r--r--   0        0        0     3867 2023-05-30 12:49:44.911867 embedbase-1.2.5/embedbase/utils.py
+-rw-r--r--   0        0        0     3730 2023-05-30 12:49:44.915866 embedbase-1.2.5/pyproject.toml
+-rw-r--r--   0        0        0     6363 1970-01-01 00:00:00.000000 embedbase-1.2.5/PKG-INFO
```

### Comparing `embedbase-1.2.4/LICENSE` & `embedbase-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.4/README.md` & `embedbase-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.4/embedbase/__main__.py` & `embedbase-1.2.5/embedbase/__main__.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.4/embedbase/app.py` & `embedbase-1.2.5/embedbase/app.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.4/embedbase/database/base.py` & `embedbase-1.2.5/embedbase/database/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.4/embedbase/database/memory_db.py` & `embedbase-1.2.5/embedbase/database/memory_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.4/embedbase/database/postgres_db.py` & `embedbase-1.2.5/embedbase/database/postgres_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.4/embedbase/database/supabase_db.py` & `embedbase-1.2.5/embedbase/database/supabase_db.py`

 * *Files 4% similar despite different names*

```diff
@@ -186,28 +186,44 @@
     async def clear(self, dataset_id: str, user_id: Optional[str] = None):
         req = self.supabase.table("documents").delete().eq("dataset_id", dataset_id)
         if user_id:
             req = req.eq("user_id", user_id)
         req.execute()
 
     async def get_datasets(self, user_id: Optional[str] = None):
-        req = self.supabase.table("datasets").select(
-            "name", "documents_count", "created_at"
+        req = self.supabase.table("distinct_datasets").select(
+            "dataset_id", "documents_count"
         )
         if user_id:
-            req = req.eq("owner", user_id)
+            req = req.eq("user_id", user_id)
         data = req.execute().data
         return [
             Dataset(
-                dataset_id=row["name"],
+                dataset_id=row["dataset_id"],
                 documents_count=row["documents_count"],
-                created_at=row["created_at"],
             )
             for row in data
         ]
+    
+    # TODO: above old, below new, temporary hack
+    # async def get_datasets(self, user_id: Optional[str] = None):
+    #     req = self.supabase.table("datasets").select(
+    #         "name", "documents_count", "created_at"
+    #     )
+    #     if user_id:
+    #         req = req.eq("owner", user_id)
+    #     data = req.execute().data
+    #     return [
+    #         Dataset(
+    #             dataset_id=row["name"],
+    #             documents_count=row["documents_count"],
+    #             created_at=row["created_at"],
+    #         )
+    #         for row in data
+    #     ]
 
     async def list(
         self,
         dataset_id: str,
         user_id: Optional[str] = None,
         offset: int = 0,
         limit: int = 100,
```

### Comparing `embedbase-1.2.4/embedbase/embedding/base.py` & `embedbase-1.2.5/embedbase/embedding/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.4/embedbase/embedding/cohere.py` & `embedbase-1.2.5/embedbase/embedding/cohere.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.4/embedbase/embedding/openai.py` & `embedbase-1.2.5/embedbase/embedding/openai.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.4/embedbase/firebase_auth.py` & `embedbase-1.2.5/embedbase/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.4/embedbase/logging_utils.py` & `embedbase-1.2.5/embedbase/logging_utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.4/embedbase/models.py` & `embedbase-1.2.5/embedbase/models.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.4/embedbase/settings.py` & `embedbase-1.2.5/embedbase/settings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.4/embedbase/strings.py` & `embedbase-1.2.5/embedbase/strings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.4/embedbase/utils.py` & `embedbase-1.2.5/embedbase/utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.4/pyproject.toml` & `embedbase-1.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [virtualenvs]
 create = true
 in-project = true
 
 [tool.poetry]
 name = "embedbase"
-version = "1.2.4"
+version = "1.2.5"
 description = "Open-source API & SDK to integrate your data and easily hook them up to LLMs."
 readme = "README.md"
 authors = ["Different AI <louis@embedbase.xyz>"]
 license = "MIT"
 repository = "https://github.com/different-ai/embedbase"
 homepage = "https://github.com/different-ai/embedbase"
 keywords = ["embeddings", "machine learning", "artificial intelligence", "llm"]
```

### Comparing `embedbase-1.2.4/PKG-INFO` & `embedbase-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedbase
-Version: 1.2.4
+Version: 1.2.5
 Summary: Open-source API & SDK to integrate your data and easily hook them up to LLMs.
 Home-page: https://github.com/different-ai/embedbase
 License: MIT
 Keywords: embeddings,machine learning,artificial intelligence,llm
 Author: Different AI
 Author-email: louis@embedbase.xyz
 Requires-Python: >=3.8,<4.0
```

