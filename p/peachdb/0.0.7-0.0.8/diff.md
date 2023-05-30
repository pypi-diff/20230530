# Comparing `tmp/peachdb-0.0.7.tar.gz` & `tmp/peachdb-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peachdb-0.0.7.tar", last modified: Tue May 30 16:51:29 2023, max compression
+gzip compressed data, was "peachdb-0.0.8.tar", last modified: Tue May 30 17:00:39 2023, max compression
```

## Comparing `peachdb-0.0.7.tar` & `peachdb-0.0.8.tar`

### file list

```diff
@@ -1,31 +1,35 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 16:51:29.609455 peachdb-0.0.7/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11356 2023-05-29 20:30:02.000000 peachdb-0.0.7/LICENSE
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       25 2023-05-30 16:35:10.000000 peachdb-0.0.7/MANIFEST.in
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6370 2023-05-30 16:51:29.609455 peachdb-0.0.7/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6051 2023-05-30 16:38:49.000000 peachdb-0.0.7/README.md
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 16:51:29.605455 peachdb-0.0.7/peachdb/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7855 2023-05-30 10:56:06.000000 peachdb-0.0.7/peachdb/__init__.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 16:51:29.609455 peachdb-0.0.7/peachdb/backends/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      923 2023-05-29 16:37:03.000000 peachdb-0.0.7/peachdb/backends/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3161 2023-05-30 10:57:00.000000 peachdb-0.0.7/peachdb/backends/backend_base.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2056 2023-05-30 11:29:19.000000 peachdb-0.0.7/peachdb/backends/hnsw_backend.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2669 2023-05-29 16:37:03.000000 peachdb-0.0.7/peachdb/backends/numpy_backend.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3894 2023-05-29 20:30:02.000000 peachdb-0.0.7/peachdb/backends/torch_backend.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      223 2023-05-29 16:37:03.000000 peachdb-0.0.7/peachdb/constants.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 16:51:29.609455 peachdb-0.0.7/peachdb/embedder/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     4936 2023-05-30 11:00:29.000000 peachdb-0.0.7/peachdb/embedder/__init__.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 16:51:29.609455 peachdb-0.0.7/peachdb/embedder/containers/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 16:50:04.000000 peachdb-0.0.7/peachdb/embedder/containers/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1671 2023-05-29 20:30:02.000000 peachdb-0.0.7/peachdb/embedder/containers/base.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1568 2023-05-29 20:32:06.000000 peachdb-0.0.7/peachdb/embedder/containers/sentence_transformer.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2718 2023-05-30 10:47:11.000000 peachdb-0.0.7/peachdb/embedder/utils.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 16:51:29.605455 peachdb-0.0.7/peachdb.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6370 2023-05-30 16:51:29.000000 peachdb-0.0.7/peachdb.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      611 2023-05-30 16:51:29.000000 peachdb-0.0.7/peachdb.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       39 2023-05-30 16:51:29.000000 peachdb-0.0.7/peachdb.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      138 2023-05-30 16:51:29.000000 peachdb-0.0.7/peachdb.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        8 2023-05-30 16:51:29.000000 peachdb-0.0.7/peachdb.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       64 2023-05-30 16:30:14.000000 peachdb-0.0.7/pyproject.toml
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      138 2023-05-30 16:44:43.000000 peachdb-0.0.7/requirements.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-05-30 16:51:29.609455 peachdb-0.0.7/setup.cfg
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      852 2023-05-30 16:50:44.000000 peachdb-0.0.7/setup.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 17:00:39.543553 peachdb-0.0.8/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11356 2023-05-29 20:30:02.000000 peachdb-0.0.8/LICENSE
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       25 2023-05-30 16:35:10.000000 peachdb-0.0.8/MANIFEST.in
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6370 2023-05-30 17:00:39.543553 peachdb-0.0.8/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6051 2023-05-30 16:38:49.000000 peachdb-0.0.8/README.md
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 17:00:39.543553 peachdb-0.0.8/peachdb/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7855 2023-05-30 10:56:06.000000 peachdb-0.0.8/peachdb/__init__.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 17:00:39.543553 peachdb-0.0.8/peachdb/backends/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      923 2023-05-29 16:37:03.000000 peachdb-0.0.8/peachdb/backends/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3161 2023-05-30 10:57:00.000000 peachdb-0.0.8/peachdb/backends/backend_base.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2056 2023-05-30 11:29:19.000000 peachdb-0.0.8/peachdb/backends/hnsw_backend.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2669 2023-05-29 16:37:03.000000 peachdb-0.0.8/peachdb/backends/numpy_backend.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3894 2023-05-29 20:30:02.000000 peachdb-0.0.8/peachdb/backends/torch_backend.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      223 2023-05-29 16:37:03.000000 peachdb-0.0.8/peachdb/constants.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 17:00:39.543553 peachdb-0.0.8/peachdb/embedder/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     4936 2023-05-30 11:00:29.000000 peachdb-0.0.8/peachdb/embedder/__init__.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 17:00:39.543553 peachdb-0.0.8/peachdb/embedder/containers/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 16:50:04.000000 peachdb-0.0.8/peachdb/embedder/containers/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1671 2023-05-29 20:30:02.000000 peachdb-0.0.8/peachdb/embedder/containers/base.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     1568 2023-05-29 20:32:06.000000 peachdb-0.0.8/peachdb/embedder/containers/sentence_transformer.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 17:00:39.543553 peachdb-0.0.8/peachdb/embedder/models/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 16:49:59.000000 peachdb-0.0.8/peachdb/embedder/models/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      288 2023-05-26 16:27:29.000000 peachdb-0.0.8/peachdb/embedder/models/base.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      598 2023-05-29 10:12:31.000000 peachdb-0.0.8/peachdb/embedder/models/sentence_transformer.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2718 2023-05-30 10:47:11.000000 peachdb-0.0.8/peachdb/embedder/utils.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 17:00:39.543553 peachdb-0.0.8/peachdb.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6370 2023-05-30 17:00:39.000000 peachdb-0.0.8/peachdb.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      727 2023-05-30 17:00:39.000000 peachdb-0.0.8/peachdb.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       39 2023-05-30 17:00:39.000000 peachdb-0.0.8/peachdb.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      138 2023-05-30 17:00:39.000000 peachdb-0.0.8/peachdb.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        8 2023-05-30 17:00:39.000000 peachdb-0.0.8/peachdb.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       64 2023-05-30 16:30:14.000000 peachdb-0.0.8/pyproject.toml
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      138 2023-05-30 16:44:43.000000 peachdb-0.0.8/requirements.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-05-30 17:00:39.543553 peachdb-0.0.8/setup.cfg
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      852 2023-05-30 17:00:09.000000 peachdb-0.0.8/setup.py
```

### Comparing `peachdb-0.0.7/LICENSE` & `peachdb-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.7/PKG-INFO` & `peachdb-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peachdb
-Version: 0.0.7
+Version: 0.0.8
 License: Apache License 2.0
 Project-URL: Source on GitHub, https://github.com/peach-db/peachdb
 Project-URL: Documentation, https://github.com/peach-db/peachdb/blob/master/README.md
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `peachdb-0.0.7/README.md` & `peachdb-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.7/peachdb/__init__.py` & `peachdb-0.0.8/peachdb/__init__.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.7/peachdb/backends/__init__.py` & `peachdb-0.0.8/peachdb/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.7/peachdb/backends/backend_base.py` & `peachdb-0.0.8/peachdb/backends/backend_base.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.7/peachdb/backends/hnsw_backend.py` & `peachdb-0.0.8/peachdb/backends/hnsw_backend.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.7/peachdb/backends/numpy_backend.py` & `peachdb-0.0.8/peachdb/backends/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.7/peachdb/backends/torch_backend.py` & `peachdb-0.0.8/peachdb/backends/torch_backend.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.7/peachdb/embedder/__init__.py` & `peachdb-0.0.8/peachdb/embedder/__init__.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.7/peachdb/embedder/containers/base.py` & `peachdb-0.0.8/peachdb/embedder/containers/base.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.7/peachdb/embedder/containers/sentence_transformer.py` & `peachdb-0.0.8/peachdb/embedder/containers/sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.7/peachdb/embedder/utils.py` & `peachdb-0.0.8/peachdb/embedder/utils.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.7/peachdb.egg-info/PKG-INFO` & `peachdb-0.0.8/peachdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peachdb
-Version: 0.0.7
+Version: 0.0.8
 License: Apache License 2.0
 Project-URL: Source on GitHub, https://github.com/peach-db/peachdb
 Project-URL: Documentation, https://github.com/peach-db/peachdb/blob/master/README.md
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `peachdb-0.0.7/peachdb.egg-info/SOURCES.txt` & `peachdb-0.0.8/peachdb.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -16,8 +16,11 @@
 peachdb/backends/hnsw_backend.py
 peachdb/backends/numpy_backend.py
 peachdb/backends/torch_backend.py
 peachdb/embedder/__init__.py
 peachdb/embedder/utils.py
 peachdb/embedder/containers/__init__.py
 peachdb/embedder/containers/base.py
-peachdb/embedder/containers/sentence_transformer.py
+peachdb/embedder/containers/sentence_transformer.py
+peachdb/embedder/models/__init__.py
+peachdb/embedder/models/base.py
+peachdb/embedder/models/sentence_transformer.py
```

### Comparing `peachdb-0.0.7/setup.py` & `peachdb-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # read the contents README
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="peachdb",
-    version="0.0.7",
+    version="0.0.8",
     packages=find_packages(),
     install_requires=requirements,
     dependency_links=["https://download.pytorch.org/whl/cu113"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Apache License 2.0",
     project_urls={
```

