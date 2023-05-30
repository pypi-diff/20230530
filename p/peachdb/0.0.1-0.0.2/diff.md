# Comparing `tmp/peachdb-0.0.1.tar.gz` & `tmp/peachdb-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peachdb-0.0.1.tar", last modified: Tue May 30 15:24:01 2023, max compression
+gzip compressed data, was "peachdb-0.0.2.tar", last modified: Tue May 30 15:26:39 2023, max compression
```

## Comparing `peachdb-0.0.1.tar` & `peachdb-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 15:24:01.677105 peachdb-0.0.1/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11356 2023-05-29 20:30:02.000000 peachdb-0.0.1/LICENSE
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       73 2023-05-30 15:24:01.677105 peachdb-0.0.1/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5415 2023-05-30 13:14:30.000000 peachdb-0.0.1/README.md
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 15:24:01.673105 peachdb-0.0.1/peachdb/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7855 2023-05-30 10:56:06.000000 peachdb-0.0.1/peachdb/__init__.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 15:24:01.677105 peachdb-0.0.1/peachdb/backends/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      923 2023-05-29 16:37:03.000000 peachdb-0.0.1/peachdb/backends/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3161 2023-05-30 10:57:00.000000 peachdb-0.0.1/peachdb/backends/backend_base.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2056 2023-05-30 11:29:19.000000 peachdb-0.0.1/peachdb/backends/hnsw_backend.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2669 2023-05-29 16:37:03.000000 peachdb-0.0.1/peachdb/backends/numpy_backend.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3894 2023-05-29 20:30:02.000000 peachdb-0.0.1/peachdb/backends/torch_backend.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      223 2023-05-29 16:37:03.000000 peachdb-0.0.1/peachdb/constants.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 15:24:01.677105 peachdb-0.0.1/peachdb/embedder/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     4936 2023-05-30 11:00:29.000000 peachdb-0.0.1/peachdb/embedder/__init__.py
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2718 2023-05-30 10:47:11.000000 peachdb-0.0.1/peachdb/embedder/utils.py
-drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 15:24:01.673105 peachdb-0.0.1/peachdb.egg-info/
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       73 2023-05-30 15:24:01.000000 peachdb-0.0.1/peachdb.egg-info/PKG-INFO
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      454 2023-05-30 15:24:01.000000 peachdb-0.0.1/peachdb.egg-info/SOURCES.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       39 2023-05-30 15:24:01.000000 peachdb-0.0.1/peachdb.egg-info/dependency_links.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      177 2023-05-30 15:24:01.000000 peachdb-0.0.1/peachdb.egg-info/requires.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        8 2023-05-30 15:24:01.000000 peachdb-0.0.1/peachdb.egg-info/top_level.txt
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       64 2023-05-26 17:11:39.000000 peachdb-0.0.1/pyproject.toml
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-05-30 15:24:01.677105 peachdb-0.0.1/setup.cfg
--rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      364 2023-05-30 15:23:50.000000 peachdb-0.0.1/setup.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 15:26:39.932657 peachdb-0.0.2/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)    11356 2023-05-29 20:30:02.000000 peachdb-0.0.2/LICENSE
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5530 2023-05-30 15:26:39.932657 peachdb-0.0.2/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5415 2023-05-30 13:14:30.000000 peachdb-0.0.2/README.md
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 15:26:39.932657 peachdb-0.0.2/peachdb/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     7855 2023-05-30 10:56:06.000000 peachdb-0.0.2/peachdb/__init__.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 15:26:39.932657 peachdb-0.0.2/peachdb/backends/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      923 2023-05-29 16:37:03.000000 peachdb-0.0.2/peachdb/backends/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3161 2023-05-30 10:57:00.000000 peachdb-0.0.2/peachdb/backends/backend_base.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2056 2023-05-30 11:29:19.000000 peachdb-0.0.2/peachdb/backends/hnsw_backend.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2669 2023-05-29 16:37:03.000000 peachdb-0.0.2/peachdb/backends/numpy_backend.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     3894 2023-05-29 20:30:02.000000 peachdb-0.0.2/peachdb/backends/torch_backend.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      223 2023-05-29 16:37:03.000000 peachdb-0.0.2/peachdb/constants.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 15:26:39.932657 peachdb-0.0.2/peachdb/embedder/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     4936 2023-05-30 11:00:29.000000 peachdb-0.0.2/peachdb/embedder/__init__.py
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     2718 2023-05-30 10:47:11.000000 peachdb-0.0.2/peachdb/embedder/utils.py
+drwxrwxr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-05-30 15:26:39.932657 peachdb-0.0.2/peachdb.egg-info/
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)     5530 2023-05-30 15:26:39.000000 peachdb-0.0.2/peachdb.egg-info/PKG-INFO
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      454 2023-05-30 15:26:39.000000 peachdb-0.0.2/peachdb.egg-info/SOURCES.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       39 2023-05-30 15:26:39.000000 peachdb-0.0.2/peachdb.egg-info/dependency_links.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      177 2023-05-30 15:26:39.000000 peachdb-0.0.2/peachdb.egg-info/requires.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)        8 2023-05-30 15:26:39.000000 peachdb-0.0.2/peachdb.egg-info/top_level.txt
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       64 2023-05-26 17:11:39.000000 peachdb-0.0.2/pyproject.toml
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-05-30 15:26:39.932657 peachdb-0.0.2/setup.cfg
+-rw-rw-r--   0 ec2-user  (1000) ec2-user  (1000)      609 2023-05-30 15:26:36.000000 peachdb-0.0.2/setup.py
```

### Comparing `peachdb-0.0.1/LICENSE` & `peachdb-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.1/README.md` & `peachdb-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.1/peachdb/__init__.py` & `peachdb-0.0.2/peachdb/__init__.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.1/peachdb/backends/__init__.py` & `peachdb-0.0.2/peachdb/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.1/peachdb/backends/backend_base.py` & `peachdb-0.0.2/peachdb/backends/backend_base.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.1/peachdb/backends/hnsw_backend.py` & `peachdb-0.0.2/peachdb/backends/hnsw_backend.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.1/peachdb/backends/numpy_backend.py` & `peachdb-0.0.2/peachdb/backends/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.1/peachdb/backends/torch_backend.py` & `peachdb-0.0.2/peachdb/backends/torch_backend.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.1/peachdb/embedder/__init__.py` & `peachdb-0.0.2/peachdb/embedder/__init__.py`

 * *Files identical despite different names*

### Comparing `peachdb-0.0.1/peachdb/embedder/utils.py` & `peachdb-0.0.2/peachdb/embedder/utils.py`

 * *Files identical despite different names*

