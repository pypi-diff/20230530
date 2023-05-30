# Comparing `tmp/bcvcontext-0.1.5.tar.gz` & `tmp/bcvcontext-0.1.6.tar.gz`

## Comparing `bcvcontext-0.1.5.tar` & `bcvcontext-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bcvcontext-0.1.5/src/bcvContext/__init__.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 bcvcontext-0.1.5/src/bcvContext/bcvContext.py
--rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 bcvcontext-0.1.5/.gitignore
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 bcvcontext-0.1.5/LICENSE
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 bcvcontext-0.1.5/README.md
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 bcvcontext-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 bcvcontext-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bcvcontext-0.1.6/src/bcvContext/__init__.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 bcvcontext-0.1.6/src/bcvContext/bcvContext.py
+-rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 bcvcontext-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 bcvcontext-0.1.6/LICENSE
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 bcvcontext-0.1.6/README.md
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 bcvcontext-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 bcvcontext-0.1.6/PKG-INFO
```

### Comparing `bcvcontext-0.1.5/src/bcvContext/bcvContext.py` & `bcvcontext-0.1.6/src/bcvContext/bcvContext.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from subprocess import call
 
 notarizationPath = ""
-isAudit = True
+isAudit = 1
 
 def init(_notarizationPath, _isAudit) :
     global notarizationPath, isAudit
     notarizationPath = _notarizationPath
     isAudit = _isAudit
 
 def scriptContext(filename) :
@@ -23,15 +23,15 @@
     day = json.load(open("../.." + notarizationPath + "/.config.json"))["day"] + _m
     if (day < 0) : raise Exception("No history at J", str(day))
     lastNotarization = json.load(open("../.." + notarizationPath + "/../../Day" + str(day) + "/.dayConfig.json"))["lastNotarization"]
     return "../.." + notarizationPath + "/../../Day" + str(day) + "/Notarization" + str(lastNotarization) + "/" + _filename
 
 def finish(*args) :
     call(["rm", "-r","../__cache__"])
-    if isAudit == "1" :
+    if isAudit == 1 :
         call(["mkdir","../__cache__"])
         for i in args :
             call(["mv",str(i),"../__cache__"])
         print("Final result at :", "../__cache__")
 
     else : 
         for i in args :
```

### Comparing `bcvcontext-0.1.5/.gitignore` & `bcvcontext-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `bcvcontext-0.1.5/LICENSE` & `bcvcontext-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bcvcontext-0.1.5/PKG-INFO` & `bcvcontext-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcvContext
-Version: 0.1.5
+Version: 0.1.6
 Summary: A small package to handle context path for the BCV generic workflow
 Author-email: CEA <thomas.marques@cea.fr>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

