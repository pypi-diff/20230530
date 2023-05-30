# Comparing `tmp/bcvcontext-0.1.3.tar.gz` & `tmp/bcvcontext-0.1.4.tar.gz`

## Comparing `bcvcontext-0.1.3.tar` & `bcvcontext-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bcvcontext-0.1.3/src/bcvContext/__init__.py
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 bcvcontext-0.1.3/src/bcvContext/bcvContext.py
--rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 bcvcontext-0.1.3/.gitignore
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 bcvcontext-0.1.3/LICENSE
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 bcvcontext-0.1.3/README.md
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 bcvcontext-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 bcvcontext-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bcvcontext-0.1.4/src/bcvContext/__init__.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 bcvcontext-0.1.4/src/bcvContext/bcvContext.py
+-rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 bcvcontext-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 bcvcontext-0.1.4/LICENSE
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 bcvcontext-0.1.4/README.md
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 bcvcontext-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 bcvcontext-0.1.4/PKG-INFO
```

### Comparing `bcvcontext-0.1.3/src/bcvContext/bcvContext.py` & `bcvcontext-0.1.4/src/bcvContext/bcvContext.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import json
-from prefect import variables 
 from subprocess import call
 
+notarizationPath = ""
+isAudit = True
+
+def init(_notarizationPath, _isAudit) :
+    notarizationPath = _notarizationPath
+    isAudit = _isAudit
+
 def scriptContext(filename) :
     return filename
 
 def notarizationContextRawfile():
-    notarizationPath = variables.get('notarization_path')
     return "../.." + notarizationPath + "/../rawFile.csv"
 
 def notarizationContext(filename) :
-    notarizationPath = variables.get('notarization_path')
     return "../.." + notarizationPath + "/" + filename
 
-def dayContext(m, filename) :
-    notarizationPath = variables.get('notarization_path')
-    if (m >= 0) : raise Exception("No history at J", str(m))
-    day = json.load(open("../.." + notarizationPath + "/.config.json"))["day"] + m
+def dayContext(_m, _filename) :
+    if (_m >= 0) : raise Exception("No history at J", str(_m))
+    day = json.load(open("../.." + notarizationPath + "/.config.json"))["day"] + _m
     if (day < 0) : raise Exception("No history at J", str(day))
     lastNotarization = json.load(open("../.." + notarizationPath + "/../../Day" + str(day) + "/.dayConfig.json"))["lastNotarization"]
-    return "../.." + notarizationPath + "/../../Day" + str(day) + "/Notarization" + str(lastNotarization) + "/" + filename
+    return "../.." + notarizationPath + "/../../Day" + str(day) + "/Notarization" + str(lastNotarization) + "/" + _filename
 
 def finish(*args) :
-    notarizationPath = variables.get('notarization_path')
-    isAudit = variables.get('is_audit')
-
     call(["rm", "-r","../__cache__"])
     if isAudit == "1" :
         call(["mkdir","../__cache__"])
         for i in args :
             call(["mv",str(i),"../__cache__"])
         print("Final result at :", "../__cache__")
```

### Comparing `bcvcontext-0.1.3/.gitignore` & `bcvcontext-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `bcvcontext-0.1.3/LICENSE` & `bcvcontext-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bcvcontext-0.1.3/PKG-INFO` & `bcvcontext-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcvContext
-Version: 0.1.3
+Version: 0.1.4
 Summary: A small package to handle context path for the BCV generic workflow
 Author-email: CEA <thomas.marques@cea.fr>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

