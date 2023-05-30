# Comparing `tmp/zenithlib-0.0.7.tar.gz` & `tmp/zenithlib-0.0.8.tar.gz`

## Comparing `zenithlib-0.0.7.tar` & `zenithlib-0.0.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 zenithlib-0.0.7/.gitattributes
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 zenithlib-0.0.7/Zenith/Web.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 zenithlib-0.0.7/Zenith/__init__.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 zenithlib-0.0.7/Zenith/src/tests.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 zenithlib-0.0.7/examples/check_vers.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 zenithlib-0.0.7/scripts/bupload.sh
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 zenithlib-0.0.7/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zenithlib-0.0.7/LICENSE
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 zenithlib-0.0.7/README.md
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 zenithlib-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 zenithlib-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 zenithlib-0.0.8/.gitattributes
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 zenithlib-0.0.8/Zenith/Web.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 zenithlib-0.0.8/Zenith/__init__.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 zenithlib-0.0.8/Zenith/src/tests.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 zenithlib-0.0.8/examples/check_vers.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 zenithlib-0.0.8/scripts/bupload.sh
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 zenithlib-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zenithlib-0.0.8/LICENSE
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 zenithlib-0.0.8/README.md
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 zenithlib-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 zenithlib-0.0.8/PKG-INFO
```

### Comparing `zenithlib-0.0.7/Zenith/Web.py` & `zenithlib-0.0.8/Zenith/Web.py`

 * *Files identical despite different names*

### Comparing `zenithlib-0.0.7/.gitignore` & `zenithlib-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `zenithlib-0.0.7/LICENSE` & `zenithlib-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `zenithlib-0.0.7/README.md` & `zenithlib-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `zenithlib-0.0.7/pyproject.toml` & `zenithlib-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ZenithLib"
-version = "0.0.07"
+version = "0.0.08"
 authors = [
   { name="Ryan Rudd", email="rsrudd@gmail.com" },
 ]
 description = "Zenith is a powerful Python framework that revolutionizes web development by enabling declarative and efficient UI components for building interactive and scalable websites."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `zenithlib-0.0.7/PKG-INFO` & `zenithlib-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ZenithLib
-Version: 0.0.7
+Version: 0.0.8
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
-Metadata-Version: 2.1 Name: ZenithLib Version: 0.0.7 Summary: Zenith is a
+Metadata-Version: 2.1 Name: ZenithLib Version: 0.0.8 Summary: Zenith is a
 powerful Python framework that revolutionizes web development by enabling
 declarative and efficient UI components for building interactive and scalable
 websites. Project-URL: Homepage, https://github.com/Ryan-Rudd/Zenith Project-
 URL: Bug Tracker, https://github.com/Ryan-Rudd/Zenith/issues Author-email: Ryan
 Rudd
 gmail.com> License-File: LICENSE Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
```

