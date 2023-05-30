# Comparing `tmp/zenithlib-0.0.1.tar.gz` & `tmp/zenithlib-0.0.2.tar.gz`

## Comparing `zenithlib-0.0.1.tar` & `zenithlib-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 zenithlib-0.0.1/.gitattributes
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zenithlib-0.0.1/Zenith/__init__.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 zenithlib-0.0.1/Zenith/src/tests.py
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 zenithlib-0.0.1/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zenithlib-0.0.1/LICENSE
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 zenithlib-0.0.1/README.md
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 zenithlib-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 zenithlib-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 zenithlib-0.0.2/.gitattributes
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 zenithlib-0.0.2/Zenith/Web.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 zenithlib-0.0.2/Zenith/__init__.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 zenithlib-0.0.2/Zenith/src/tests.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 zenithlib-0.0.2/examples/check_vers.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 zenithlib-0.0.2/scripts/bupload.sh
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 zenithlib-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zenithlib-0.0.2/LICENSE
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 zenithlib-0.0.2/README.md
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 zenithlib-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 zenithlib-0.0.2/PKG-INFO
```

### Comparing `zenithlib-0.0.1/.gitignore` & `zenithlib-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `zenithlib-0.0.1/LICENSE` & `zenithlib-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zenithlib-0.0.1/README.md` & `zenithlib-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `zenithlib-0.0.1/pyproject.toml` & `zenithlib-0.0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ZenithLib"
-version = "0.0.01"
+version = "0.0.02"
 authors = [
   { name="Ryan Rudd", email="rsrudd@gmail.com" },
 ]
 description = "Zenith is a powerful Python framework that revolutionizes web development by enabling declarative and efficient UI components for building interactive and scalable websites."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `zenithlib-0.0.1/PKG-INFO` & `zenithlib-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ZenithLib
-Version: 0.0.1
+Version: 0.0.2
 Summary: Zenith is a powerful Python framework that revolutionizes web development by enabling declarative and efficient UI components for building interactive and scalable websites.
 Project-URL: Homepage, https://github.com/Ryan-Rudd/Zenith
 Project-URL: Bug Tracker, https://github.com/Ryan-Rudd/Zenith/issues
 Author-email: Ryan Rudd <rsrudd@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ZenithLib Version: 0.0.1 Summary: Zenith is a
+Metadata-Version: 2.1 Name: ZenithLib Version: 0.0.2 Summary: Zenith is a
 powerful Python framework that revolutionizes web development by enabling
 declarative and efficient UI components for building interactive and scalable
 websites. Project-URL: Homepage, https://github.com/Ryan-Rudd/Zenith Project-
 URL: Bug Tracker, https://github.com/Ryan-Rudd/Zenith/issues Author-email: Ryan
 Rudd
 gmail.com> License-File: LICENSE Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
```

