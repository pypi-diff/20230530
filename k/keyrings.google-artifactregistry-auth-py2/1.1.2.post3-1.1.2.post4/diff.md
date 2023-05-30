# Comparing `tmp/keyrings.google_artifactregistry_auth_py2-1.1.2.post3-py2-none-any.whl.zip` & `tmp/keyrings.google_artifactregistry_auth_py2-1.1.2.post4-py2-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 8005 bytes, number of entries: 7
--rw-r--r--  2.0 unx     3223 b- defN 23-May-30 09:14 keyrings/google-artifactregistry-auth-py2/gauth.py
--rw-r--r--  2.0 unx    11358 b- defN 23-May-30 10:54 keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/LICENSE
--rw-r--r--  2.0 unx     1275 b- defN 23-May-30 10:54 keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-30 10:54 keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 23-May-30 10:54 keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-May-30 10:54 keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      828 b- defN 23-May-30 10:54 keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/RECORD
-7 files, 16834 bytes uncompressed, 6473 bytes compressed:  61.5%
+Zip file size: 8012 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     3243 b- defN 23-May-30 11:16 keyrings/google-artifactregistry-auth-py2/gauth.py
+-rw-r--r--  2.0 unx    11358 b- defN 23-May-30 11:19 keyrings.google_artifactregistry_auth_py2-1.1.2.post4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1275 b- defN 23-May-30 11:19 keyrings.google_artifactregistry_auth_py2-1.1.2.post4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-30 11:19 keyrings.google_artifactregistry_auth_py2-1.1.2.post4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 23-May-30 11:19 keyrings.google_artifactregistry_auth_py2-1.1.2.post4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-May-30 11:19 keyrings.google_artifactregistry_auth_py2-1.1.2.post4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      828 b- defN 23-May-30 11:19 keyrings.google_artifactregistry_auth_py2-1.1.2.post4.dist-info/RECORD
+7 files, 16854 bytes uncompressed, 6480 bytes compressed:  61.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: keyrings/google-artifactregistry-auth-py2/gauth.py
 Comment: 
 
-Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/LICENSE
+Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post4.dist-info/LICENSE
 Comment: 
 
-Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/METADATA
+Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post4.dist-info/METADATA
 Comment: 
 
-Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/WHEEL
+Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post4.dist-info/WHEEL
 Comment: 
 
-Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/entry_points.txt
+Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post4.dist-info/entry_points.txt
 Comment: 
 
-Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/top_level.txt
+Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post4.dist-info/top_level.txt
 Comment: 
 
-Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/RECORD
+Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## keyrings/google-artifactregistry-auth-py2/gauth.py

```diff
@@ -71,18 +71,21 @@
 
 
 def get_gcloud_credential():
 
   # fall back to fetching credentials from gcloud if Application Default Credentials fails
   try:
     logging.warning("Trying to retrieve credentials from gcloud...")
-    command = subprocess.run(['gcloud','config','config-helper','--format=json(credential)'], check=True, stdout=subprocess.PIPE, universal_newlines=True)
+    command = subprocess.check_output(
+      ['gcloud','config','config-helper','--format=json(credential)'],
+      check=True, stdout=subprocess.PIPE, universal_newlines=True
+    )
   except Exception as e:
     raise Exception ("gcloud command exited with status: {0}".format(e))
-  result = json.loads(command.stdout)
+  result = json.loads(command)
   credential = result.get("credential")
   if credential is None:
     raise Exception("No credential returned from gcloud")
   if "access_token" not in credential or "token_expiry" not in credential:
     raise Exception("Malformed response from gcloud")
   return credential.get("access_token")
```

## Comparing `keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/LICENSE` & `keyrings.google_artifactregistry_auth_py2-1.1.2.post4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/METADATA` & `keyrings.google_artifactregistry_auth_py2-1.1.2.post4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keyrings.google-artifactregistry-auth-py2
-Version: 1.1.2.post3
+Version: 1.1.2.post4
 Summary: Keyring backend for Google Auth tokens - a fork for Python 2
 Home-page: UNKNOWN
 Author: Megan Kuo
 Author-email: megankuo@google.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/RECORD` & `keyrings.google_artifactregistry_auth_py2-1.1.2.post4.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-keyrings/google-artifactregistry-auth-py2/gauth.py,sha256=p36uSbm-07XJqYKNKLb0z3CYJV1owm0ohZ9doahNsBg,3223
-keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/METADATA,sha256=pnMpoLefKJKFngjvGy_ooFxRPAuLIwsoPp0xdHmq0kQ,1275
-keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/WHEEL,sha256=CbUdLTqD3-4zWemf83rgR_2_MC4TeXw9qXwrXte5w4w,92
-keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/entry_points.txt,sha256=8wO7OlzhILJcVDvqJ0Bp6RQ7lAlZo5iDOnCYUVYjYg0,49
-keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/top_level.txt,sha256=CFU-m0Q3B8OHGUonsk82bd-w5tsD16QsqpnMH4hufJY,9
-keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/RECORD,,
+keyrings/google-artifactregistry-auth-py2/gauth.py,sha256=TABhl9Xdo1DBpOuBbYgElwDmRK4yo8tsU8OeXk6-G3Y,3243
+keyrings.google_artifactregistry_auth_py2-1.1.2.post4.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+keyrings.google_artifactregistry_auth_py2-1.1.2.post4.dist-info/METADATA,sha256=kDTwB6-2-FOx7_BOAKTeKWql8fp0D9X7QVELjgsXNZ4,1275
+keyrings.google_artifactregistry_auth_py2-1.1.2.post4.dist-info/WHEEL,sha256=CbUdLTqD3-4zWemf83rgR_2_MC4TeXw9qXwrXte5w4w,92
+keyrings.google_artifactregistry_auth_py2-1.1.2.post4.dist-info/entry_points.txt,sha256=8wO7OlzhILJcVDvqJ0Bp6RQ7lAlZo5iDOnCYUVYjYg0,49
+keyrings.google_artifactregistry_auth_py2-1.1.2.post4.dist-info/top_level.txt,sha256=CFU-m0Q3B8OHGUonsk82bd-w5tsD16QsqpnMH4hufJY,9
+keyrings.google_artifactregistry_auth_py2-1.1.2.post4.dist-info/RECORD,,
```

