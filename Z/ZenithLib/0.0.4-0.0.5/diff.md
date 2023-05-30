# Comparing `tmp/zenithlib-0.0.4.tar.gz` & `tmp/zenithlib-0.0.5.tar.gz`

## Comparing `zenithlib-0.0.4.tar` & `zenithlib-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 zenithlib-0.0.4/.gitattributes
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 zenithlib-0.0.4/Zenith/Web.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 zenithlib-0.0.4/Zenith/__init__.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 zenithlib-0.0.4/Zenith/src/tests.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zenithlib-0.0.4/examples/check_vers.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 zenithlib-0.0.4/scripts/bupload.sh
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 zenithlib-0.0.4/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zenithlib-0.0.4/LICENSE
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 zenithlib-0.0.4/README.md
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 zenithlib-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 zenithlib-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 zenithlib-0.0.5/.gitattributes
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 zenithlib-0.0.5/Zenith/Web.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 zenithlib-0.0.5/Zenith/__init__.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 zenithlib-0.0.5/Zenith/src/tests.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zenithlib-0.0.5/examples/check_vers.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 zenithlib-0.0.5/scripts/bupload.sh
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 zenithlib-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zenithlib-0.0.5/LICENSE
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 zenithlib-0.0.5/README.md
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 zenithlib-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 zenithlib-0.0.5/PKG-INFO
```

### Comparing `zenithlib-0.0.4/.gitignore` & `zenithlib-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `zenithlib-0.0.4/LICENSE` & `zenithlib-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `zenithlib-0.0.4/README.md` & `zenithlib-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `zenithlib-0.0.4/pyproject.toml` & `zenithlib-0.0.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ZenithLib"
-version = "0.0.04"
+version = "0.0.05"
 authors = [
   { name="Ryan Rudd", email="rsrudd@gmail.com" },
 ]
 description = "Zenith is a powerful Python framework that revolutionizes web development by enabling declarative and efficient UI components for building interactive and scalable websites."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `zenithlib-0.0.4/PKG-INFO` & `zenithlib-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ZenithLib
-Version: 0.0.4
+Version: 0.0.5
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
-Metadata-Version: 2.1 Name: ZenithLib Version: 0.0.4 Summary: Zenith is a
+Metadata-Version: 2.1 Name: ZenithLib Version: 0.0.5 Summary: Zenith is a
 powerful Python framework that revolutionizes web development by enabling
 declarative and efficient UI components for building interactive and scalable
 websites. Project-URL: Homepage, https://github.com/Ryan-Rudd/Zenith Project-
 URL: Bug Tracker, https://github.com/Ryan-Rudd/Zenith/issues Author-email: Ryan
 Rudd
 gmail.com> License-File: LICENSE Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
```

