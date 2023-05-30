# Comparing `tmp/keyrings.google_artifactregistry_auth_py2-1.1.2.post6-py2-none-any.whl.zip` & `tmp/keyrings.google_artifactregistry_auth_py2-1.1.2.post7-py2-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 9631 bytes, number of entries: 9
+Zip file size: 9651 bytes, number of entries: 9
 -rw-r--r--  2.0 unx        0 b- defN 23-May-30 14:06 keyrings/__init__.py
--rw-r--r--  2.0 unx     3243 b- defN 23-May-30 11:16 keyrings/gauth.py
+-rw-r--r--  2.0 unx     3207 b- defN 23-May-30 15:46 keyrings/gauth.py
 -rw-r--r--  2.0 unx     3243 b- defN 23-May-30 11:16 keyrings/google-artifactregistry-auth-py2/gauth.py
--rw-r--r--  2.0 unx    11358 b- defN 23-May-30 14:06 keyrings.google_artifactregistry_auth_py2-1.1.2.post6.dist-info/LICENSE
--rw-r--r--  2.0 unx     1275 b- defN 23-May-30 14:06 keyrings.google_artifactregistry_auth_py2-1.1.2.post6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-30 14:06 keyrings.google_artifactregistry_auth_py2-1.1.2.post6.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 23-May-30 14:06 keyrings.google_artifactregistry_auth_py2-1.1.2.post6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-May-30 14:06 keyrings.google_artifactregistry_auth_py2-1.1.2.post6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      976 b- defN 23-May-30 14:06 keyrings.google_artifactregistry_auth_py2-1.1.2.post6.dist-info/RECORD
-9 files, 20245 bytes uncompressed, 7873 bytes compressed:  61.1%
+-rw-r--r--  2.0 unx    11358 b- defN 23-May-30 15:46 keyrings.google_artifactregistry_auth_py2-1.1.2.post7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1275 b- defN 23-May-30 15:46 keyrings.google_artifactregistry_auth_py2-1.1.2.post7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-30 15:46 keyrings.google_artifactregistry_auth_py2-1.1.2.post7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 23-May-30 15:46 keyrings.google_artifactregistry_auth_py2-1.1.2.post7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-May-30 15:46 keyrings.google_artifactregistry_auth_py2-1.1.2.post7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      976 b- defN 23-May-30 15:46 keyrings.google_artifactregistry_auth_py2-1.1.2.post7.dist-info/RECORD
+9 files, 20209 bytes uncompressed, 7893 bytes compressed:  60.9%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: keyrings/gauth.py
 Comment: 
 
 Filename: keyrings/google-artifactregistry-auth-py2/gauth.py
 Comment: 
 
-Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post6.dist-info/LICENSE
+Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post7.dist-info/LICENSE
 Comment: 
 
-Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post6.dist-info/METADATA
+Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post7.dist-info/METADATA
 Comment: 
 
-Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post6.dist-info/WHEEL
+Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post7.dist-info/WHEEL
 Comment: 
 
-Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post6.dist-info/entry_points.txt
+Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post7.dist-info/entry_points.txt
 Comment: 
 
-Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post6.dist-info/top_level.txt
+Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post7.dist-info/top_level.txt
 Comment: 
 
-Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post6.dist-info/RECORD
+Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## keyrings/gauth.py

```diff
@@ -73,15 +73,15 @@
 def get_gcloud_credential():
 
   # fall back to fetching credentials from gcloud if Application Default Credentials fails
   try:
     logging.warning("Trying to retrieve credentials from gcloud...")
     command = subprocess.check_output(
       ['gcloud','config','config-helper','--format=json(credential)'],
-      check=True, stdout=subprocess.PIPE, universal_newlines=True
+      universal_newlines=True
     )
   except Exception as e:
     raise Exception ("gcloud command exited with status: {0}".format(e))
   result = json.loads(command)
   credential = result.get("credential")
   if credential is None:
     raise Exception("No credential returned from gcloud")
```

## Comparing `keyrings.google_artifactregistry_auth_py2-1.1.2.post6.dist-info/LICENSE` & `keyrings.google_artifactregistry_auth_py2-1.1.2.post7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `keyrings.google_artifactregistry_auth_py2-1.1.2.post6.dist-info/METADATA` & `keyrings.google_artifactregistry_auth_py2-1.1.2.post7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keyrings.google-artifactregistry-auth-py2
-Version: 1.1.2.post6
+Version: 1.1.2.post7
 Summary: Keyring backend for Google Auth tokens - a fork for Python 2
 Home-page: UNKNOWN
 Author: Megan Kuo
 Author-email: megankuo@google.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `keyrings.google_artifactregistry_auth_py2-1.1.2.post6.dist-info/RECORD` & `keyrings.google_artifactregistry_auth_py2-1.1.2.post7.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 keyrings/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-keyrings/gauth.py,sha256=TABhl9Xdo1DBpOuBbYgElwDmRK4yo8tsU8OeXk6-G3Y,3243
+keyrings/gauth.py,sha256=3L9zpqnLQ9NYSHgvGa0JkQBNLJdYk74Y1AoCnRNrM1Q,3207
 keyrings/google-artifactregistry-auth-py2/gauth.py,sha256=TABhl9Xdo1DBpOuBbYgElwDmRK4yo8tsU8OeXk6-G3Y,3243
-keyrings.google_artifactregistry_auth_py2-1.1.2.post6.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-keyrings.google_artifactregistry_auth_py2-1.1.2.post6.dist-info/METADATA,sha256=auYo2BZCkK1N-PObv2SUw9znDhw2I8Y43mBGDqzTM3M,1275
-keyrings.google_artifactregistry_auth_py2-1.1.2.post6.dist-info/WHEEL,sha256=CbUdLTqD3-4zWemf83rgR_2_MC4TeXw9qXwrXte5w4w,92
-keyrings.google_artifactregistry_auth_py2-1.1.2.post6.dist-info/entry_points.txt,sha256=8wO7OlzhILJcVDvqJ0Bp6RQ7lAlZo5iDOnCYUVYjYg0,49
-keyrings.google_artifactregistry_auth_py2-1.1.2.post6.dist-info/top_level.txt,sha256=CFU-m0Q3B8OHGUonsk82bd-w5tsD16QsqpnMH4hufJY,9
-keyrings.google_artifactregistry_auth_py2-1.1.2.post6.dist-info/RECORD,,
+keyrings.google_artifactregistry_auth_py2-1.1.2.post7.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+keyrings.google_artifactregistry_auth_py2-1.1.2.post7.dist-info/METADATA,sha256=4fbovc7mjhh3h-4MxPEt58KbKZ04xrYstWO6vAEuYSE,1275
+keyrings.google_artifactregistry_auth_py2-1.1.2.post7.dist-info/WHEEL,sha256=CbUdLTqD3-4zWemf83rgR_2_MC4TeXw9qXwrXte5w4w,92
+keyrings.google_artifactregistry_auth_py2-1.1.2.post7.dist-info/entry_points.txt,sha256=8wO7OlzhILJcVDvqJ0Bp6RQ7lAlZo5iDOnCYUVYjYg0,49
+keyrings.google_artifactregistry_auth_py2-1.1.2.post7.dist-info/top_level.txt,sha256=CFU-m0Q3B8OHGUonsk82bd-w5tsD16QsqpnMH4hufJY,9
+keyrings.google_artifactregistry_auth_py2-1.1.2.post7.dist-info/RECORD,,
```

