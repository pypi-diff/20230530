# Comparing `tmp/pyread_eagle-1.0.2.tar.gz` & `tmp/pyread_eagle-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyread_eagle-1.0.2.tar", last modified: Thu Mar 16 17:33:21 2023, max compression
+gzip compressed data, was "pyread_eagle-1.0.3.tar", last modified: Tue May 30 13:52:04 2023, max compression
```

## Comparing `pyread_eagle-1.0.2.tar` & `pyread_eagle-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 koman     (1000) koman     (1000)        0 2023-03-16 17:33:21.786907 pyread_eagle-1.0.2/
--rw-------   0 koman     (1000) koman     (1000)    35148 2021-10-05 09:39:35.000000 pyread_eagle-1.0.2/LICENSE.md
--rw-------   0 koman     (1000) koman     (1000)       45 2021-10-05 09:39:35.000000 pyread_eagle-1.0.2/MANIFEST.in
--rw-rw-r--   0 koman     (1000) koman     (1000)    13129 2023-03-16 17:33:21.786907 pyread_eagle-1.0.2/PKG-INFO
--rw-rw-r--   0 koman     (1000) koman     (1000)    12569 2023-03-16 17:29:24.000000 pyread_eagle-1.0.2/README.md
--rw-rw-r--   0 koman     (1000) koman     (1000)      674 2023-03-16 17:32:42.000000 pyread_eagle-1.0.2/pyproject.toml
-drwxrwxr-x   0 koman     (1000) koman     (1000)        0 2023-03-16 17:33:21.786907 pyread_eagle-1.0.2/pyread_eagle/
--rw-rw-r--   0 koman     (1000) koman     (1000)       78 2023-03-16 17:29:24.000000 pyread_eagle-1.0.2/pyread_eagle/__init__.py
--rw-rw-r--   0 koman     (1000) koman     (1000)       22 2023-03-16 17:32:56.000000 pyread_eagle-1.0.2/pyread_eagle/__version__.py
--rw-rw-r--   0 koman     (1000) koman     (1000)    22482 2023-03-16 17:30:20.000000 pyread_eagle-1.0.2/pyread_eagle/_pyread_eagle.py
-drwxrwxr-x   0 koman     (1000) koman     (1000)        0 2023-03-16 17:33:21.786907 pyread_eagle-1.0.2/pyread_eagle.egg-info/
--rw-------   0 koman     (1000) koman     (1000)    13129 2023-03-16 17:33:21.000000 pyread_eagle-1.0.2/pyread_eagle.egg-info/PKG-INFO
--rw-------   0 koman     (1000) koman     (1000)      331 2023-03-16 17:33:21.000000 pyread_eagle-1.0.2/pyread_eagle.egg-info/SOURCES.txt
--rw-------   0 koman     (1000) koman     (1000)        1 2023-03-16 17:33:21.000000 pyread_eagle-1.0.2/pyread_eagle.egg-info/dependency_links.txt
--rw-------   0 koman     (1000) koman     (1000)       11 2023-03-16 17:33:21.000000 pyread_eagle-1.0.2/pyread_eagle.egg-info/requires.txt
--rw-------   0 koman     (1000) koman     (1000)       13 2023-03-16 17:33:21.000000 pyread_eagle-1.0.2/pyread_eagle.egg-info/top_level.txt
--rw-rw-r--   0 koman     (1000) koman     (1000)       38 2023-03-16 17:33:21.786907 pyread_eagle-1.0.2/setup.cfg
-drwxrwxr-x   0 koman     (1000) koman     (1000)        0 2023-03-16 17:33:21.786907 pyread_eagle-1.0.2/tests/
--rw-rw-r--   0 koman     (1000) koman     (1000)     5345 2022-03-25 16:56:32.000000 pyread_eagle-1.0.2/tests/test_regions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:52:04.306392 pyread_eagle-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-30 13:51:33.000000 pyread_eagle-1.0.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-30 13:51:33.000000 pyread_eagle-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13129 2023-05-30 13:52:04.306392 pyread_eagle-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-05-30 13:51:33.000000 pyread_eagle-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-30 13:51:33.000000 pyread_eagle-1.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:52:04.306392 pyread_eagle-1.0.3/pyread_eagle/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-30 13:51:33.000000 pyread_eagle-1.0.3/pyread_eagle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 13:51:33.000000 pyread_eagle-1.0.3/pyread_eagle/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22538 2023-05-30 13:51:33.000000 pyread_eagle-1.0.3/pyread_eagle/_pyread_eagle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:52:04.306392 pyread_eagle-1.0.3/pyread_eagle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13129 2023-05-30 13:52:04.000000 pyread_eagle-1.0.3/pyread_eagle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-30 13:52:04.000000 pyread_eagle-1.0.3/pyread_eagle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:52:04.000000 pyread_eagle-1.0.3/pyread_eagle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-30 13:52:04.000000 pyread_eagle-1.0.3/pyread_eagle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 13:52:04.000000 pyread_eagle-1.0.3/pyread_eagle.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 13:52:04.306392 pyread_eagle-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:52:04.306392 pyread_eagle-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-05-30 13:51:33.000000 pyread_eagle-1.0.3/tests/test_regions.py
```

### Comparing `pyread_eagle-1.0.2/LICENSE.md` & `pyread_eagle-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyread_eagle-1.0.2/PKG-INFO` & `pyread_eagle-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyread_eagle
-Version: 1.0.2
+Version: 1.0.3
 Summary: Pure-python port of J. Helly's read_eagle.
 Author-email: Kyle Oman <kyle.a.oman@durham.ac.uk>
 Project-URL: Homepage, https://github.com/kyleaoman/pyread_eagle
 Project-URL: Bug Tracker, https://github.com/kyleaoman/pyread_eagle/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `pyread_eagle-1.0.2/README.md` & `pyread_eagle-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyread_eagle-1.0.2/pyproject.toml` & `pyread_eagle-1.0.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyread_eagle"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Kyle Oman", email="kyle.a.oman@durham.ac.uk" },
 ]
 description = "Pure-python port of J. Helly's read_eagle."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pyread_eagle-1.0.2/pyread_eagle/_pyread_eagle.py` & `pyread_eagle-1.0.3/pyread_eagle/_pyread_eagle.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,21 +271,21 @@
         yvec = np.array(yvec)
         zvec = np.array(zvec)
         length = np.array(length)
         if any([param.shape != (3,) for param in (centre, xvec, yvec, zvec, length)]):
             raise ValueError(
                 "select_rotated_region parameters must all have " "shape (3, )"
             )
-        if any(
+        if not all(
             [
-                np.dot(xvec, yvec) != 0.0,
-                np.dot(xvec, zvec) != 0,
-                np.linalg.norm(xvec) != 1.0,
-                np.linalg.norm(yvec) != 1.0,
-                np.linalg.norm(zvec) != 1.0,
+                np.isclose(np.dot(xvec, yvec), 0.0),
+                np.isclose(np.dot(xvec, zvec), 0.0),
+                np.isclose(np.linalg.norm(xvec), 1.0),
+                np.isclose(np.linalg.norm(yvec), 1.0),
+                np.isclose(np.linalg.norm(zvec), 1.0),
             ]
         ):
             raise ValueError(
                 "select_rotated_region parameters xvec, yvec &"
                 " zvec must be mutually orthogonal unit vectors"
             )
         diagonal = np.sqrt(3) * self.boxsize / self.ncell
```

### Comparing `pyread_eagle-1.0.2/pyread_eagle.egg-info/PKG-INFO` & `pyread_eagle-1.0.3/pyread_eagle.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyread-eagle
-Version: 1.0.2
+Version: 1.0.3
 Summary: Pure-python port of J. Helly's read_eagle.
 Author-email: Kyle Oman <kyle.a.oman@durham.ac.uk>
 Project-URL: Homepage, https://github.com/kyleaoman/pyread_eagle
 Project-URL: Bug Tracker, https://github.com/kyleaoman/pyread_eagle/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `pyread_eagle-1.0.2/tests/test_regions.py` & `pyread_eagle-1.0.3/tests/test_regions.py`

 * *Files identical despite different names*

