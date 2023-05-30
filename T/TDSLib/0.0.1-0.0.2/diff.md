# Comparing `tmp/tdslib-0.0.1.tar.gz` & `tmp/tdslib-0.0.2.tar.gz`

## Comparing `tdslib-0.0.1.tar` & `tdslib-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     3058 2020-02-02 00:00:00.000000 tdslib-0.0.1/pyproject.toml~
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 tdslib-0.0.1/src/tdslib/__about__.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 tdslib-0.0.1/src/tdslib/__init__.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 tdslib-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 tdslib-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 tdslib-0.0.1/README.md
--rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 tdslib-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 tdslib-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 tdslib-0.0.2/pyproject.toml~
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 tdslib-0.0.2/src/tdslib/__about__.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 tdslib-0.0.2/src/tdslib/__init__.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 tdslib-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 tdslib-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 tdslib-0.0.2/README.md
+-rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 tdslib-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 tdslib-0.0.2/PKG-INFO
```

### Comparing `tdslib-0.0.1/pyproject.toml~` & `tdslib-0.0.2/pyproject.toml~`

 * *Files 0% similar despite different names*

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

### Comparing `tdslib-0.0.1/LICENSE.txt` & `tdslib-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tdslib-0.0.1/pyproject.toml` & `tdslib-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
-name = "tdslib"
+name = "TDSLib"
 dynamic = ["version"]
 description = ''
 readme = "README.md"
 requires-python = ">=3.7"
 license = "MIT"
 keywords = []
 authors = [
```

### Comparing `tdslib-0.0.1/PKG-INFO` & `tdslib-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: tdslib
-Version: 0.0.1
+Name: TDSLib
+Version: 0.0.2
 Project-URL: Documentation, https://github.com/unknown/tdslib#readme
 Project-URL: Issues, https://github.com/unknown/tdslib/issues
 Project-URL: Source, https://github.com/unknown/tdslib
 Author-email: "J. Steven Dodge" <jsdodge@sfu.ca>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 1 - Planning
```

