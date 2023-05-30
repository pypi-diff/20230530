# Comparing `tmp/bcvcontext-0.1.4.tar.gz` & `tmp/bcvcontext-0.1.5.tar.gz`

## Comparing `bcvcontext-0.1.4.tar` & `bcvcontext-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bcvcontext-0.1.4/src/bcvContext/__init__.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 bcvcontext-0.1.4/src/bcvContext/bcvContext.py
--rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 bcvcontext-0.1.4/.gitignore
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 bcvcontext-0.1.4/LICENSE
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 bcvcontext-0.1.4/README.md
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 bcvcontext-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 bcvcontext-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bcvcontext-0.1.5/src/bcvContext/__init__.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 bcvcontext-0.1.5/src/bcvContext/bcvContext.py
+-rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 bcvcontext-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 bcvcontext-0.1.5/LICENSE
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 bcvcontext-0.1.5/README.md
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 bcvcontext-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 bcvcontext-0.1.5/PKG-INFO
```

### Comparing `bcvcontext-0.1.4/src/bcvContext/bcvContext.py` & `bcvcontext-0.1.5/src/bcvContext/bcvContext.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 from subprocess import call
 
 notarizationPath = ""
 isAudit = True
 
 def init(_notarizationPath, _isAudit) :
+    global notarizationPath, isAudit
     notarizationPath = _notarizationPath
     isAudit = _isAudit
 
 def scriptContext(filename) :
     return filename
 
 def notarizationContextRawfile():
```

### Comparing `bcvcontext-0.1.4/.gitignore` & `bcvcontext-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `bcvcontext-0.1.4/LICENSE` & `bcvcontext-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bcvcontext-0.1.4/PKG-INFO` & `bcvcontext-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcvContext
-Version: 0.1.4
+Version: 0.1.5
 Summary: A small package to handle context path for the BCV generic workflow
 Author-email: CEA <thomas.marques@cea.fr>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

