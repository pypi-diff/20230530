# Comparing `tmp/tdspy-0.0.1.tar.gz` & `tmp/tdspy-0.0.2.tar.gz`

## Comparing `tdspy-0.0.1.tar` & `tdspy-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 tdspy-0.0.1/pyproject.toml~
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 tdspy-0.0.1/src/tdspy/__about__.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 tdspy-0.0.1/src/tdspy/__init__.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 tdspy-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 tdspy-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 tdspy-0.0.1/README.md
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 tdspy-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 tdspy-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 tdspy-0.0.2/pyproject.toml~
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 tdspy-0.0.2/src/tdspy/__about__.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 tdspy-0.0.2/src/tdspy/__init__.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 tdspy-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 tdspy-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 tdspy-0.0.2/README.md
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 tdspy-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 tdspy-0.0.2/PKG-INFO
```

### Comparing `tdspy-0.0.1/pyproject.toml~` & `tdspy-0.0.2/pyproject.toml~`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 requires-python = ">=3.7"
 license = "MIT"
 keywords = []
 authors = [
   { name = "J. Steven Dodge", email = "jsdodge@sfu.ca" },
 ]
 classifiers = [
-  "Development Status :: 4 - Beta",
+  "Development Status :: 1 - Planning",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
```

### Comparing `tdspy-0.0.1/LICENSE.txt` & `tdspy-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tdspy-0.0.1/pyproject.toml` & `tdspy-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
-name = "tdspy"
+name = "TDSPy"
 dynamic = ["version"]
 description = ''
 readme = "README.md"
 requires-python = ">=3.7"
 license = "MIT"
 keywords = []
 authors = [
```

### Comparing `tdspy-0.0.1/PKG-INFO` & `tdspy-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: tdspy
-Version: 0.0.1
+Name: TDSPy
+Version: 0.0.2
 Project-URL: Documentation, https://github.com/unknown/tdspy#readme
 Project-URL: Issues, https://github.com/unknown/tdspy/issues
 Project-URL: Source, https://github.com/unknown/tdspy
 Author-email: "J. Steven Dodge" <jsdodge@sfu.ca>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 1 - Planning
```

