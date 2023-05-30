# Comparing `tmp/embedbase-1.2.2.tar.gz` & `tmp/embedbase-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedbase-1.2.2.tar", max compression
+gzip compressed data, was "embedbase-1.2.3.tar", max compression
```

## Comparing `embedbase-1.2.2.tar` & `embedbase-1.2.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1069 2023-05-29 17:06:51.527840 embedbase-1.2.2/LICENSE
--rw-r--r--   0        0        0     4931 2023-05-29 17:06:51.527840 embedbase-1.2.2/README.md
--rw-r--r--   0        0        0      121 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/__init__.py
--rw-r--r--   0        0        0     1716 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/__main__.py
--rw-r--r--   0        0        0      976 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/api.py
--rw-r--r--   0        0        0    17884 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/app.py
--rw-r--r--   0        0        0       88 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/database/__init__.py
--rw-r--r--   0        0        0     3436 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/database/base.py
--rw-r--r--   0        0        0     6220 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/database/memory_db.py
--rw-r--r--   0        0        0    10254 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/database/postgres_db.py
--rw-r--r--   0        0        0     7608 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/database/supabase_db.py
--rw-r--r--   0        0        0       77 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/embedding/__init__.py
--rw-r--r--   0        0        0      858 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/embedding/base.py
--rw-r--r--   0        0        0     1237 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/embedding/cohere.py
--rw-r--r--   0        0        0     2059 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/embedding/openai.py
--rw-r--r--   0        0        0     1551 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/firebase_auth.py
--rw-r--r--   0        0        0      690 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/logging_utils.py
--rw-r--r--   0        0        0     1095 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/models.py
--rw-r--r--   0        0        0     1285 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/settings.py
--rw-r--r--   0        0        0     3208 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/strings.py
--rw-r--r--   0        0        0      301 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/supabase_auth.py
--rw-r--r--   0        0        0     3867 2023-05-29 17:06:51.663847 embedbase-1.2.2/embedbase/utils.py
--rw-r--r--   0        0        0     3730 2023-05-29 17:06:51.667847 embedbase-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     6363 1970-01-01 00:00:00.000000 embedbase-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-30 07:11:11.725420 embedbase-1.2.3/LICENSE
+-rw-r--r--   0        0        0     4931 2023-05-30 07:11:11.725420 embedbase-1.2.3/README.md
+-rw-r--r--   0        0        0      121 2023-05-30 07:11:11.857422 embedbase-1.2.3/embedbase/__init__.py
+-rw-r--r--   0        0        0     1716 2023-05-30 07:11:11.857422 embedbase-1.2.3/embedbase/__main__.py
+-rw-r--r--   0        0        0      416 2023-05-30 07:11:11.857422 embedbase-1.2.3/embedbase/api.py
+-rw-r--r--   0        0        0    17884 2023-05-30 07:11:11.857422 embedbase-1.2.3/embedbase/app.py
+-rw-r--r--   0        0        0       88 2023-05-30 07:11:11.857422 embedbase-1.2.3/embedbase/database/__init__.py
+-rw-r--r--   0        0        0     3436 2023-05-30 07:11:11.857422 embedbase-1.2.3/embedbase/database/base.py
+-rw-r--r--   0        0        0     6220 2023-05-30 07:11:11.857422 embedbase-1.2.3/embedbase/database/memory_db.py
+-rw-r--r--   0        0        0    10254 2023-05-30 07:11:11.857422 embedbase-1.2.3/embedbase/database/postgres_db.py
+-rw-r--r--   0        0        0     7608 2023-05-30 07:11:11.857422 embedbase-1.2.3/embedbase/database/supabase_db.py
+-rw-r--r--   0        0        0       77 2023-05-30 07:11:11.857422 embedbase-1.2.3/embedbase/embedding/__init__.py
+-rw-r--r--   0        0        0      858 2023-05-30 07:11:11.857422 embedbase-1.2.3/embedbase/embedding/base.py
+-rw-r--r--   0        0        0     1237 2023-05-30 07:11:11.857422 embedbase-1.2.3/embedbase/embedding/cohere.py
+-rw-r--r--   0        0        0     2059 2023-05-30 07:11:11.857422 embedbase-1.2.3/embedbase/embedding/openai.py
+-rw-r--r--   0        0        0     1551 2023-05-30 07:11:11.857422 embedbase-1.2.3/embedbase/firebase_auth.py
+-rw-r--r--   0        0        0      690 2023-05-30 07:11:11.857422 embedbase-1.2.3/embedbase/logging_utils.py
+-rw-r--r--   0        0        0     1095 2023-05-30 07:11:11.857422 embedbase-1.2.3/embedbase/models.py
+-rw-r--r--   0        0        0     1245 2023-05-30 07:11:11.857422 embedbase-1.2.3/embedbase/settings.py
+-rw-r--r--   0        0        0     3208 2023-05-30 07:11:11.857422 embedbase-1.2.3/embedbase/strings.py
+-rw-r--r--   0        0        0      301 2023-05-30 07:11:11.857422 embedbase-1.2.3/embedbase/supabase_auth.py
+-rw-r--r--   0        0        0     3867 2023-05-30 07:11:11.857422 embedbase-1.2.3/embedbase/utils.py
+-rw-r--r--   0        0        0     3730 2023-05-30 07:11:11.861422 embedbase-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     6363 1970-01-01 00:00:00.000000 embedbase-1.2.3/PKG-INFO
```

### Comparing `embedbase-1.2.2/LICENSE` & `embedbase-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.2/README.md` & `embedbase-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.2/embedbase/__main__.py` & `embedbase-1.2.3/embedbase/__main__.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.2/embedbase/app.py` & `embedbase-1.2.3/embedbase/app.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.2/embedbase/database/base.py` & `embedbase-1.2.3/embedbase/database/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.2/embedbase/database/memory_db.py` & `embedbase-1.2.3/embedbase/database/memory_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.2/embedbase/database/postgres_db.py` & `embedbase-1.2.3/embedbase/database/postgres_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.2/embedbase/database/supabase_db.py` & `embedbase-1.2.3/embedbase/database/supabase_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.2/embedbase/embedding/base.py` & `embedbase-1.2.3/embedbase/embedding/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.2/embedbase/embedding/cohere.py` & `embedbase-1.2.3/embedbase/embedding/cohere.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.2/embedbase/embedding/openai.py` & `embedbase-1.2.3/embedbase/embedding/openai.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.2/embedbase/firebase_auth.py` & `embedbase-1.2.3/embedbase/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.2/embedbase/logging_utils.py` & `embedbase-1.2.3/embedbase/logging_utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.2/embedbase/models.py` & `embedbase-1.2.3/embedbase/models.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.2/embedbase/settings.py` & `embedbase-1.2.3/embedbase/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     openai_api_key: typing.Optional[str] = None
     openai_organization: typing.Optional[str] = None
     supabase_url: typing.Optional[str] = None
     supabase_key: typing.Optional[str] = None
     
     log_level: str = "INFO"
     auth: typing.Optional[str] = None
-    sentry: typing.Optional[str] = None
     firebase_service_account_path: typing.Optional[str] = None
 
 @lru_cache()
 def get_settings_from_file(path: str = "config.yaml"):
     """
     Read settings from a file, only supports yaml for now
     """
```

### Comparing `embedbase-1.2.2/embedbase/strings.py` & `embedbase-1.2.3/embedbase/strings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.2/embedbase/utils.py` & `embedbase-1.2.3/embedbase/utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.2.2/pyproject.toml` & `embedbase-1.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [virtualenvs]
 create = true
 in-project = true
 
 [tool.poetry]
 name = "embedbase"
-version = "1.2.2"
+version = "1.2.3"
 description = "Open-source API & SDK to integrate your data and easily hook them up to LLMs."
 readme = "README.md"
 authors = ["Different AI <louis@embedbase.xyz>"]
 license = "MIT"
 repository = "https://github.com/different-ai/embedbase"
 homepage = "https://github.com/different-ai/embedbase"
 keywords = ["embeddings", "machine learning", "artificial intelligence", "llm"]
```

### Comparing `embedbase-1.2.2/PKG-INFO` & `embedbase-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedbase
-Version: 1.2.2
+Version: 1.2.3
 Summary: Open-source API & SDK to integrate your data and easily hook them up to LLMs.
 Home-page: https://github.com/different-ai/embedbase
 License: MIT
 Keywords: embeddings,machine learning,artificial intelligence,llm
 Author: Different AI
 Author-email: louis@embedbase.xyz
 Requires-Python: >=3.8,<4.0
```

