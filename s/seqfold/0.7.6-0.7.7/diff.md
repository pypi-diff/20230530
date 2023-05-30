# Comparing `tmp/seqfold-0.7.6.tar.gz` & `tmp/seqfold-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/seqfold-0.7.6.tar", last modified: Thu Mar  4 00:55:23 2021, max compression
+gzip compressed data, was "dist/seqfold-0.7.7.tar", last modified: Thu Mar  4 00:55:46 2021, max compression
```

## Comparing `seqfold-0.7.6.tar` & `seqfold-0.7.7.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2021-03-04 00:55:23.000000 seqfold-0.7.6/
--rw-r--r--   0 root         (0) staff       (20)       93 2021-03-04 00:55:23.000000 seqfold-0.7.6/.bumpversion.cfg
--rw-r--r--   0 root         (0) staff       (20)     1940 2020-01-09 17:13:46.000000 seqfold-0.7.6/.gitignore
--rw-r--r--   0 root         (0) staff       (20)     1075 2020-01-06 19:01:50.000000 seqfold-0.7.6/LICENSE
--rw-r--r--   0 root         (0) staff       (20)      524 2021-03-04 00:54:16.000000 seqfold-0.7.6/Makefile
--rw-r--r--   0 root         (0) staff       (20)     9648 2021-03-04 00:55:23.000000 seqfold-0.7.6/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     7948 2020-02-05 15:14:47.000000 seqfold-0.7.6/README.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2021-03-04 00:55:23.000000 seqfold-0.7.6/data/
--rw-r--r--   0 root         (0) staff       (20)      308 2020-01-08 15:01:34.000000 seqfold-0.7.6/data/README.md
--rw-r--r--   0 root         (0) staff       (20)     6643 2020-01-08 22:44:52.000000 seqfold-0.7.6/data/_rna.py
--rw-r--r--   0 root         (0) staff       (20)     5380 2020-01-06 19:01:50.000000 seqfold-0.7.6/data/rna.dangle.dh.txt
--rw-r--r--   0 root         (0) staff       (20)     5394 2020-01-06 19:01:50.000000 seqfold-0.7.6/data/rna.dangle.txt
--rw-r--r--   0 root         (0) staff       (20)     1886 2020-01-06 19:01:50.000000 seqfold-0.7.6/data/rna.loop.dh.txt
--rw-r--r--   0 root         (0) staff       (20)     1854 2020-01-06 19:01:50.000000 seqfold-0.7.6/data/rna.loop.txt
--rw-r--r--   0 root         (0) staff       (20)      281 2020-01-16 18:32:49.000000 seqfold-0.7.6/data/rna.py.template
--rw-r--r--   0 root         (0) staff       (20)     4147 2020-01-06 19:01:50.000000 seqfold-0.7.6/data/rna.stack.dh.txt
--rw-r--r--   0 root         (0) staff       (20)     4135 2020-01-06 19:01:50.000000 seqfold-0.7.6/data/rna.stack.txt
--rw-r--r--   0 root         (0) staff       (20)     4113 2020-01-06 19:01:50.000000 seqfold-0.7.6/data/rna.tstack.dh.txt
--rw-r--r--   0 root         (0) staff       (20)     4111 2020-01-06 19:01:50.000000 seqfold-0.7.6/data/rna.tstack.txt
-drwxr-xr-x   0 root         (0) staff       (20)        0 2021-03-04 00:55:23.000000 seqfold-0.7.6/examples/
--rw-r--r--   0 root         (0) staff       (20)      536 2020-01-28 17:27:56.000000 seqfold-0.7.6/examples/dna.csv
--rw-r--r--   0 root         (0) staff       (20)     1449 2020-01-28 17:28:02.000000 seqfold-0.7.6/examples/rna.csv
--rw-r--r--   0 root         (0) staff       (20)        0 2020-01-28 17:44:14.000000 seqfold-0.7.6/requirements.txt
-drwxr-xr-x   0 root         (0) staff       (20)        0 2021-03-04 00:55:23.000000 seqfold-0.7.6/seqfold/
--rw-r--r--   0 root         (0) staff       (20)      479 2020-01-23 18:50:21.000000 seqfold-0.7.6/seqfold/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    13161 2021-03-04 00:32:17.000000 seqfold-0.7.6/seqfold/dna.py
--rw-r--r--   0 root         (0) staff       (20)    26858 2020-01-28 17:09:39.000000 seqfold-0.7.6/seqfold/fold.py
--rw-r--r--   0 root         (0) staff       (20)     2143 2020-02-03 16:58:04.000000 seqfold-0.7.6/seqfold/main.py
--rw-r--r--   0 root         (0) staff       (20)    19479 2020-01-16 18:05:09.000000 seqfold-0.7.6/seqfold/rna.py
--rw-r--r--   0 root         (0) staff       (20)     9465 2020-01-23 18:58:42.000000 seqfold-0.7.6/seqfold/tm.py
--rw-r--r--   0 root         (0) staff       (20)     1189 2020-01-23 14:15:18.000000 seqfold-0.7.6/seqfold/types.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2021-03-04 00:55:23.000000 seqfold-0.7.6/seqfold.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     9648 2021-03-04 00:55:23.000000 seqfold-0.7.6/seqfold.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      759 2021-03-04 00:55:23.000000 seqfold-0.7.6/seqfold.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2021-03-04 00:55:23.000000 seqfold-0.7.6/seqfold.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       46 2021-03-04 00:55:23.000000 seqfold-0.7.6/seqfold.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2020-01-16 19:54:02.000000 seqfold-0.7.6/seqfold.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) staff       (20)       39 2021-03-04 00:55:23.000000 seqfold-0.7.6/seqfold.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)       14 2021-03-04 00:55:23.000000 seqfold-0.7.6/seqfold.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)       38 2021-03-04 00:55:23.000000 seqfold-0.7.6/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     1239 2021-03-04 00:55:23.000000 seqfold-0.7.6/setup.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2021-03-04 00:55:23.000000 seqfold-0.7.6/tests/
--rw-r--r--   0 root         (0) staff       (20)        0 2020-01-06 19:01:50.000000 seqfold-0.7.6/tests/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3132 2020-01-28 17:27:28.000000 seqfold-0.7.6/tests/fold_examples.py
--rw-r--r--   0 root         (0) staff       (20)      562 2020-01-28 17:25:28.000000 seqfold-0.7.6/tests/fold_profile.py
--rw-r--r--   0 root         (0) staff       (20)     7041 2021-03-04 00:34:34.000000 seqfold-0.7.6/tests/fold_test.py
--rw-r--r--   0 root         (0) staff       (20)     1807 2021-03-04 00:35:33.000000 seqfold-0.7.6/tests/tm_test.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-03-04 00:55:46.000000 seqfold-0.7.7/
+-rw-r--r--   0 root         (0) staff       (20)       93 2021-03-04 00:55:46.000000 seqfold-0.7.7/.bumpversion.cfg
+-rw-r--r--   0 root         (0) staff       (20)     1940 2020-01-09 17:13:46.000000 seqfold-0.7.7/.gitignore
+-rw-r--r--   0 root         (0) staff       (20)     1075 2020-01-06 19:01:50.000000 seqfold-0.7.7/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)      524 2021-03-04 00:54:16.000000 seqfold-0.7.7/Makefile
+-rw-r--r--   0 root         (0) staff       (20)     9648 2021-03-04 00:55:46.000000 seqfold-0.7.7/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     7948 2020-02-05 15:14:47.000000 seqfold-0.7.7/README.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-03-04 00:55:46.000000 seqfold-0.7.7/data/
+-rw-r--r--   0 root         (0) staff       (20)      308 2020-01-08 15:01:34.000000 seqfold-0.7.7/data/README.md
+-rw-r--r--   0 root         (0) staff       (20)     6643 2020-01-08 22:44:52.000000 seqfold-0.7.7/data/_rna.py
+-rw-r--r--   0 root         (0) staff       (20)     5380 2020-01-06 19:01:50.000000 seqfold-0.7.7/data/rna.dangle.dh.txt
+-rw-r--r--   0 root         (0) staff       (20)     5394 2020-01-06 19:01:50.000000 seqfold-0.7.7/data/rna.dangle.txt
+-rw-r--r--   0 root         (0) staff       (20)     1886 2020-01-06 19:01:50.000000 seqfold-0.7.7/data/rna.loop.dh.txt
+-rw-r--r--   0 root         (0) staff       (20)     1854 2020-01-06 19:01:50.000000 seqfold-0.7.7/data/rna.loop.txt
+-rw-r--r--   0 root         (0) staff       (20)      281 2020-01-16 18:32:49.000000 seqfold-0.7.7/data/rna.py.template
+-rw-r--r--   0 root         (0) staff       (20)     4147 2020-01-06 19:01:50.000000 seqfold-0.7.7/data/rna.stack.dh.txt
+-rw-r--r--   0 root         (0) staff       (20)     4135 2020-01-06 19:01:50.000000 seqfold-0.7.7/data/rna.stack.txt
+-rw-r--r--   0 root         (0) staff       (20)     4113 2020-01-06 19:01:50.000000 seqfold-0.7.7/data/rna.tstack.dh.txt
+-rw-r--r--   0 root         (0) staff       (20)     4111 2020-01-06 19:01:50.000000 seqfold-0.7.7/data/rna.tstack.txt
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-03-04 00:55:46.000000 seqfold-0.7.7/examples/
+-rw-r--r--   0 root         (0) staff       (20)      536 2020-01-28 17:27:56.000000 seqfold-0.7.7/examples/dna.csv
+-rw-r--r--   0 root         (0) staff       (20)     1449 2020-01-28 17:28:02.000000 seqfold-0.7.7/examples/rna.csv
+-rw-r--r--   0 root         (0) staff       (20)        0 2020-01-28 17:44:14.000000 seqfold-0.7.7/requirements.txt
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-03-04 00:55:46.000000 seqfold-0.7.7/seqfold/
+-rw-r--r--   0 root         (0) staff       (20)      479 2020-01-23 18:50:21.000000 seqfold-0.7.7/seqfold/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)    13161 2021-03-04 00:32:17.000000 seqfold-0.7.7/seqfold/dna.py
+-rw-r--r--   0 root         (0) staff       (20)    26858 2020-01-28 17:09:39.000000 seqfold-0.7.7/seqfold/fold.py
+-rw-r--r--   0 root         (0) staff       (20)     2143 2020-02-03 16:58:04.000000 seqfold-0.7.7/seqfold/main.py
+-rw-r--r--   0 root         (0) staff       (20)    19479 2020-01-16 18:05:09.000000 seqfold-0.7.7/seqfold/rna.py
+-rw-r--r--   0 root         (0) staff       (20)     9465 2020-01-23 18:58:42.000000 seqfold-0.7.7/seqfold/tm.py
+-rw-r--r--   0 root         (0) staff       (20)     1189 2020-01-23 14:15:18.000000 seqfold-0.7.7/seqfold/types.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-03-04 00:55:46.000000 seqfold-0.7.7/seqfold.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     9648 2021-03-04 00:55:46.000000 seqfold-0.7.7/seqfold.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      759 2021-03-04 00:55:46.000000 seqfold-0.7.7/seqfold.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2021-03-04 00:55:46.000000 seqfold-0.7.7/seqfold.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       46 2021-03-04 00:55:46.000000 seqfold-0.7.7/seqfold.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2020-01-16 19:54:02.000000 seqfold-0.7.7/seqfold.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) staff       (20)       39 2021-03-04 00:55:46.000000 seqfold-0.7.7/seqfold.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)       14 2021-03-04 00:55:46.000000 seqfold-0.7.7/seqfold.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)       38 2021-03-04 00:55:46.000000 seqfold-0.7.7/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     1239 2021-03-04 00:55:46.000000 seqfold-0.7.7/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2021-03-04 00:55:46.000000 seqfold-0.7.7/tests/
+-rw-r--r--   0 root         (0) staff       (20)        0 2020-01-06 19:01:50.000000 seqfold-0.7.7/tests/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3132 2020-01-28 17:27:28.000000 seqfold-0.7.7/tests/fold_examples.py
+-rw-r--r--   0 root         (0) staff       (20)      562 2020-01-28 17:25:28.000000 seqfold-0.7.7/tests/fold_profile.py
+-rw-r--r--   0 root         (0) staff       (20)     7041 2021-03-04 00:34:34.000000 seqfold-0.7.7/tests/fold_test.py
+-rw-r--r--   0 root         (0) staff       (20)     1807 2021-03-04 00:35:33.000000 seqfold-0.7.7/tests/tm_test.py
```

### Comparing `seqfold-0.7.6/.gitignore` & `seqfold-0.7.7/.gitignore`

 * *Files identical despite different names*

### Comparing `seqfold-0.7.6/LICENSE` & `seqfold-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `seqfold-0.7.6/Makefile` & `seqfold-0.7.7/Makefile`

 * *Files identical despite different names*

### Comparing `seqfold-0.7.6/PKG-INFO` & `seqfold-0.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqfold
-Version: 0.7.6
+Version: 0.7.7
 Summary: Predict the minimum free energy structure of nucleic acids
 Home-page: https://github.com/Lattice-Automation/seqfold
 Author: JJTimmons
 Author-email: jtimmons@latticeautomation.com
 License: mit
 Description: # seqfold
```

### Comparing `seqfold-0.7.6/README.md` & `seqfold-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `seqfold-0.7.6/data/_rna.py` & `seqfold-0.7.7/data/_rna.py`

 * *Files identical despite different names*

### Comparing `seqfold-0.7.6/data/rna.dangle.dh.txt` & `seqfold-0.7.7/data/rna.dangle.dh.txt`

 * *Files identical despite different names*

### Comparing `seqfold-0.7.6/data/rna.dangle.txt` & `seqfold-0.7.7/data/rna.dangle.txt`

 * *Files identical despite different names*

### Comparing `seqfold-0.7.6/data/rna.loop.dh.txt` & `seqfold-0.7.7/data/rna.loop.dh.txt`

 * *Files identical despite different names*

### Comparing `seqfold-0.7.6/data/rna.loop.txt` & `seqfold-0.7.7/data/rna.loop.txt`

 * *Files identical despite different names*

### Comparing `seqfold-0.7.6/data/rna.stack.dh.txt` & `seqfold-0.7.7/data/rna.stack.dh.txt`

 * *Files identical despite different names*

### Comparing `seqfold-0.7.6/data/rna.stack.txt` & `seqfold-0.7.7/data/rna.stack.txt`

 * *Files identical despite different names*

### Comparing `seqfold-0.7.6/data/rna.tstack.dh.txt` & `seqfold-0.7.7/data/rna.tstack.dh.txt`

 * *Files identical despite different names*

### Comparing `seqfold-0.7.6/data/rna.tstack.txt` & `seqfold-0.7.7/data/rna.tstack.txt`

 * *Files identical despite different names*

### Comparing `seqfold-0.7.6/examples/dna.csv` & `seqfold-0.7.7/examples/dna.csv`

 * *Files identical despite different names*

### Comparing `seqfold-0.7.6/examples/rna.csv` & `seqfold-0.7.7/examples/rna.csv`

 * *Files identical despite different names*

### Comparing `seqfold-0.7.6/seqfold/dna.py` & `seqfold-0.7.7/seqfold/dna.py`

 * *Files identical despite different names*

### Comparing `seqfold-0.7.6/seqfold/fold.py` & `seqfold-0.7.7/seqfold/fold.py`

 * *Files identical despite different names*

### Comparing `seqfold-0.7.6/seqfold/main.py` & `seqfold-0.7.7/seqfold/main.py`

 * *Files identical despite different names*

### Comparing `seqfold-0.7.6/seqfold/rna.py` & `seqfold-0.7.7/seqfold/rna.py`

 * *Files identical despite different names*

### Comparing `seqfold-0.7.6/seqfold/tm.py` & `seqfold-0.7.7/seqfold/tm.py`

 * *Files identical despite different names*

### Comparing `seqfold-0.7.6/seqfold/types.py` & `seqfold-0.7.7/seqfold/types.py`

 * *Files identical despite different names*

### Comparing `seqfold-0.7.6/seqfold.egg-info/PKG-INFO` & `seqfold-0.7.7/seqfold.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqfold
-Version: 0.7.6
+Version: 0.7.7
 Summary: Predict the minimum free energy structure of nucleic acids
 Home-page: https://github.com/Lattice-Automation/seqfold
 Author: JJTimmons
 Author-email: jtimmons@latticeautomation.com
 License: mit
 Description: # seqfold
```

### Comparing `seqfold-0.7.6/seqfold.egg-info/SOURCES.txt` & `seqfold-0.7.7/seqfold.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seqfold-0.7.6/setup.py` & `seqfold-0.7.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     require("setuptools>=38.3")
 except VersionConflict:
     print("Error: version of setuptools is too old (<38.3)!")
     sys.exit(1)
 
 setup(
     name="seqfold",
-    version="0.7.6",
+    version="0.7.7",
     description="Predict the minimum free energy structure of nucleic acids",
     author="JJTimmons",
     author_email="jtimmons@latticeautomation.com",
     license="mit",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `seqfold-0.7.6/tests/fold_examples.py` & `seqfold-0.7.7/tests/fold_examples.py`

 * *Files identical despite different names*

### Comparing `seqfold-0.7.6/tests/fold_profile.py` & `seqfold-0.7.7/tests/fold_profile.py`

 * *Files identical despite different names*

### Comparing `seqfold-0.7.6/tests/fold_test.py` & `seqfold-0.7.7/tests/fold_test.py`

 * *Files identical despite different names*

### Comparing `seqfold-0.7.6/tests/tm_test.py` & `seqfold-0.7.7/tests/tm_test.py`

 * *Files identical despite different names*

