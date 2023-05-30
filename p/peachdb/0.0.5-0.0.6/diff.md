# Comparing `tmp/peachdb-0.0.5.tar.gz` & `tmp/peachdb-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peachdb-0.0.5.tar", last modified: Tue May 30 16:39:35 2023, max compression
+gzip compressed data, was "peachdb-0.0.6.tar", last modified: Tue May 30 16:46:01 2023, max compression
```

## Comparing `peachdb-0.0.5.tar` & `peachdb-0.0.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 16:39:35.100368 peachdb-0.0.5/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11356 2023-05-29 20:30:02.000000 peachdb-0.0.5/LICENSE
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       25 2023-05-30 16:35:10.000000 peachdb-0.0.5/MANIFEST.in
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6370 2023-05-30 16:39:35.100368 peachdb-0.0.5/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6051 2023-05-30 16:38:49.000000 peachdb-0.0.5/README.md
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 16:39:35.100368 peachdb-0.0.5/peachdb/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7855 2023-05-30 10:56:06.000000 peachdb-0.0.5/peachdb/__init__.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 16:39:35.100368 peachdb-0.0.5/peachdb/backends/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      923 2023-05-29 16:37:03.000000 peachdb-0.0.5/peachdb/backends/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3161 2023-05-30 10:57:00.000000 peachdb-0.0.5/peachdb/backends/backend_base.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2056 2023-05-30 11:29:19.000000 peachdb-0.0.5/peachdb/backends/hnsw_backend.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2669 2023-05-29 16:37:03.000000 peachdb-0.0.5/peachdb/backends/numpy_backend.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3894 2023-05-29 20:30:02.000000 peachdb-0.0.5/peachdb/backends/torch_backend.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      223 2023-05-29 16:37:03.000000 peachdb-0.0.5/peachdb/constants.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 16:39:35.100368 peachdb-0.0.5/peachdb/embedder/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     4936 2023-05-30 11:00:29.000000 peachdb-0.0.5/peachdb/embedder/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2718 2023-05-30 10:47:11.000000 peachdb-0.0.5/peachdb/embedder/utils.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 16:39:35.100368 peachdb-0.0.5/peachdb.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6370 2023-05-30 16:39:35.000000 peachdb-0.0.5/peachdb.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      483 2023-05-30 16:39:35.000000 peachdb-0.0.5/peachdb.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       39 2023-05-30 16:39:35.000000 peachdb-0.0.5/peachdb.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      177 2023-05-30 16:39:35.000000 peachdb-0.0.5/peachdb.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        8 2023-05-30 16:39:35.000000 peachdb-0.0.5/peachdb.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       64 2023-05-30 16:30:14.000000 peachdb-0.0.5/pyproject.toml
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      177 2023-05-30 16:30:18.000000 peachdb-0.0.5/requirements.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-05-30 16:39:35.100368 peachdb-0.0.5/setup.cfg
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      852 2023-05-30 16:38:51.000000 peachdb-0.0.5/setup.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 16:46:01.478524 peachdb-0.0.6/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11356 2023-05-29 20:30:02.000000 peachdb-0.0.6/LICENSE
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       25 2023-05-30 16:35:10.000000 peachdb-0.0.6/MANIFEST.in
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6370 2023-05-30 16:46:01.478524 peachdb-0.0.6/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6051 2023-05-30 16:38:49.000000 peachdb-0.0.6/README.md
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 16:46:01.478524 peachdb-0.0.6/peachdb/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7855 2023-05-30 10:56:06.000000 peachdb-0.0.6/peachdb/__init__.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 16:46:01.478524 peachdb-0.0.6/peachdb/backends/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      923 2023-05-29 16:37:03.000000 peachdb-0.0.6/peachdb/backends/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3161 2023-05-30 10:57:00.000000 peachdb-0.0.6/peachdb/backends/backend_base.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2056 2023-05-30 11:29:19.000000 peachdb-0.0.6/peachdb/backends/hnsw_backend.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2669 2023-05-29 16:37:03.000000 peachdb-0.0.6/peachdb/backends/numpy_backend.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3894 2023-05-29 20:30:02.000000 peachdb-0.0.6/peachdb/backends/torch_backend.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      223 2023-05-29 16:37:03.000000 peachdb-0.0.6/peachdb/constants.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 16:46:01.478524 peachdb-0.0.6/peachdb/embedder/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     4936 2023-05-30 11:00:29.000000 peachdb-0.0.6/peachdb/embedder/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2718 2023-05-30 10:47:11.000000 peachdb-0.0.6/peachdb/embedder/utils.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 16:46:01.478524 peachdb-0.0.6/peachdb.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     6370 2023-05-30 16:46:01.000000 peachdb-0.0.6/peachdb.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      483 2023-05-30 16:46:01.000000 peachdb-0.0.6/peachdb.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       39 2023-05-30 16:46:01.000000 peachdb-0.0.6/peachdb.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      138 2023-05-30 16:46:01.000000 peachdb-0.0.6/peachdb.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        8 2023-05-30 16:46:01.000000 peachdb-0.0.6/peachdb.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       64 2023-05-30 16:30:14.000000 peachdb-0.0.6/pyproject.toml
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      138 2023-05-30 16:44:43.000000 peachdb-0.0.6/requirements.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-05-30 16:46:01.478524 peachdb-0.0.6/setup.cfg
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      852 2023-05-30 16:44:49.000000 peachdb-0.0.6/setup.py
```

### Comparing `peachdb-0.0.5/LICENSE` & `peachdb-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.5/PKG-INFO` & `peachdb-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peachdb
-Version: 0.0.5
+Version: 0.0.6
 License: Apache License 2.0
 Project-URL: Source on GitHub, https://github.com/peach-db/peachdb
 Project-URL: Documentation, https://github.com/peach-db/peachdb/blob/master/README.md
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `peachdb-0.0.5/README.md` & `peachdb-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.5/peachdb/__init__.py` & `peachdb-0.0.6/peachdb/__init__.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.5/peachdb/backends/__init__.py` & `peachdb-0.0.6/peachdb/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.5/peachdb/backends/backend_base.py` & `peachdb-0.0.6/peachdb/backends/backend_base.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.5/peachdb/backends/hnsw_backend.py` & `peachdb-0.0.6/peachdb/backends/hnsw_backend.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.5/peachdb/backends/numpy_backend.py` & `peachdb-0.0.6/peachdb/backends/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.5/peachdb/backends/torch_backend.py` & `peachdb-0.0.6/peachdb/backends/torch_backend.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.5/peachdb/embedder/__init__.py` & `peachdb-0.0.6/peachdb/embedder/__init__.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.5/peachdb/embedder/utils.py` & `peachdb-0.0.6/peachdb/embedder/utils.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.5/peachdb.egg-info/PKG-INFO` & `peachdb-0.0.6/peachdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peachdb
-Version: 0.0.5
+Version: 0.0.6
 License: Apache License 2.0
 Project-URL: Source on GitHub, https://github.com/peach-db/peachdb
 Project-URL: Documentation, https://github.com/peach-db/peachdb/blob/master/README.md
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `peachdb-0.0.5/setup.py` & `peachdb-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # read the contents README
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="peachdb",
-    version="0.0.5",
+    version="0.0.6",
     packages=find_packages(),
     install_requires=requirements,
     dependency_links=["https://download.pytorch.org/whl/cu113"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Apache License 2.0",
     project_urls={
```

