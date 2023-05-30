# Comparing `tmp/keyrings.google_artifactregistry_auth_py2-1.1.2.post2-py2-none-any.whl.zip` & `tmp/keyrings.google_artifactregistry_auth_py2-1.1.2.post3-py2-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7963 bytes, number of entries: 7
--rw-r--r--  2.0 unx     3223 b- defN 23-May-29 13:46 keyrings/google-artifactregistry-auth-py2/gauth.py
--rw-r--r--  2.0 unx    11358 b- defN 23-May-30 09:13 keyrings.google_artifactregistry_auth_py2-1.1.2.post2.dist-info/LICENSE
--rw-r--r--  2.0 unx     1143 b- defN 23-May-30 09:13 keyrings.google_artifactregistry_auth_py2-1.1.2.post2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-30 09:13 keyrings.google_artifactregistry_auth_py2-1.1.2.post2.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 23-May-30 09:13 keyrings.google_artifactregistry_auth_py2-1.1.2.post2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-May-30 09:13 keyrings.google_artifactregistry_auth_py2-1.1.2.post2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      828 b- defN 23-May-30 09:13 keyrings.google_artifactregistry_auth_py2-1.1.2.post2.dist-info/RECORD
-7 files, 16702 bytes uncompressed, 6431 bytes compressed:  61.5%
+Zip file size: 8005 bytes, number of entries: 7
+-rw-r--r--  2.0 unx     3223 b- defN 23-May-30 09:14 keyrings/google-artifactregistry-auth-py2/gauth.py
+-rw-r--r--  2.0 unx    11358 b- defN 23-May-30 10:54 keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1275 b- defN 23-May-30 10:54 keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-30 10:54 keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 23-May-30 10:54 keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-May-30 10:54 keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      828 b- defN 23-May-30 10:54 keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/RECORD
+7 files, 16834 bytes uncompressed, 6473 bytes compressed:  61.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: keyrings/google-artifactregistry-auth-py2/gauth.py
 Comment: 
 
-Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post2.dist-info/LICENSE
+Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/LICENSE
 Comment: 
 
-Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post2.dist-info/METADATA
+Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/METADATA
 Comment: 
 
-Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post2.dist-info/WHEEL
+Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/WHEEL
 Comment: 
 
-Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post2.dist-info/entry_points.txt
+Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/entry_points.txt
 Comment: 
 
-Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post2.dist-info/top_level.txt
+Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/top_level.txt
 Comment: 
 
-Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post2.dist-info/RECORD
+Filename: keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `keyrings.google_artifactregistry_auth_py2-1.1.2.post2.dist-info/LICENSE` & `keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `keyrings.google_artifactregistry_auth_py2-1.1.2.post2.dist-info/METADATA` & `keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keyrings.google-artifactregistry-auth-py2
-Version: 1.1.2.post2
+Version: 1.1.2.post3
 Summary: Keyring backend for Google Auth tokens - a fork for Python 2
 Home-page: UNKNOWN
 Author: Megan Kuo
 Author-email: megankuo@google.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,14 +13,18 @@
 Classifier: Programming Language :: Python :: 2
 Requires-Python: >=2.7
 Description-Content-Type: text/markdown
 Requires-Dist: keyring (<19.0.0)
 Requires-Dist: google-auth (<2)
 Requires-Dist: requests (<2.28)
 Requires-Dist: pluggy (<2)
+Requires-Dist: cachetools (<4)
+Requires-Dist: entrypoints (<0.4)
+Requires-Dist: cryptography (<3.4)
+Requires-Dist: setuptools (<45)
 
 # Artifact Registry tools for Python 2
 
 This repository contains an alternate [keyring](https://pypi.python.org/pypi/keyring) backend implementation to help with interacting with Python repositories hosted on Artifact Registry.
 
 This is a fork of the original [Google Cloud Platform repo](https://github.com/GoogleCloudPlatform/artifact-registry-python-tools) backported to support Python 2.
```

## Comparing `keyrings.google_artifactregistry_auth_py2-1.1.2.post2.dist-info/RECORD` & `keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 keyrings/google-artifactregistry-auth-py2/gauth.py,sha256=p36uSbm-07XJqYKNKLb0z3CYJV1owm0ohZ9doahNsBg,3223
-keyrings.google_artifactregistry_auth_py2-1.1.2.post2.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-keyrings.google_artifactregistry_auth_py2-1.1.2.post2.dist-info/METADATA,sha256=avHDegc69jhp179XWXvXOcR10-k0wVyN-GUxvqE5RKo,1143
-keyrings.google_artifactregistry_auth_py2-1.1.2.post2.dist-info/WHEEL,sha256=CbUdLTqD3-4zWemf83rgR_2_MC4TeXw9qXwrXte5w4w,92
-keyrings.google_artifactregistry_auth_py2-1.1.2.post2.dist-info/entry_points.txt,sha256=8wO7OlzhILJcVDvqJ0Bp6RQ7lAlZo5iDOnCYUVYjYg0,49
-keyrings.google_artifactregistry_auth_py2-1.1.2.post2.dist-info/top_level.txt,sha256=CFU-m0Q3B8OHGUonsk82bd-w5tsD16QsqpnMH4hufJY,9
-keyrings.google_artifactregistry_auth_py2-1.1.2.post2.dist-info/RECORD,,
+keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/METADATA,sha256=pnMpoLefKJKFngjvGy_ooFxRPAuLIwsoPp0xdHmq0kQ,1275
+keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/WHEEL,sha256=CbUdLTqD3-4zWemf83rgR_2_MC4TeXw9qXwrXte5w4w,92
+keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/entry_points.txt,sha256=8wO7OlzhILJcVDvqJ0Bp6RQ7lAlZo5iDOnCYUVYjYg0,49
+keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/top_level.txt,sha256=CFU-m0Q3B8OHGUonsk82bd-w5tsD16QsqpnMH4hufJY,9
+keyrings.google_artifactregistry_auth_py2-1.1.2.post3.dist-info/RECORD,,
```

