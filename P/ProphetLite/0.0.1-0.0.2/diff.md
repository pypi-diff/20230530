# Comparing `tmp/ProphetLite-0.0.1-py3-none-any.whl.zip` & `tmp/ProphetLite-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,12 @@
-Zip file size: 2604 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     1087 b- defN 23-May-29 22:41 ProphetLite-0.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1734 b- defN 23-May-29 22:41 ProphetLite-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-29 22:41 ProphetLite-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 23-May-29 22:41 ProphetLite-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      405 b- defN 23-May-29 22:41 ProphetLite-0.0.1.dist-info/RECORD
-5 files, 3319 bytes uncompressed, 1844 bytes compressed:  44.4%
+Zip file size: 6531 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat       27 b- defN 23-May-29 22:43 ProphetLite/__init__.py
+-rw-rw-rw-  2.0 fat     1264 b- defN 23-May-22 15:04 ProphetLite/fourier.py
+-rw-rw-rw-  2.0 fat     2840 b- defN 23-May-29 21:25 ProphetLite/linear_basis.py
+-rw-rw-rw-  2.0 fat      812 b- defN 23-May-29 21:23 ProphetLite/model.py
+-rw-rw-rw-  2.0 fat     6882 b- defN 23-May-29 22:39 ProphetLite/prophetlite.py
+-rw-rw-rw-  2.0 fat     1087 b- defN 23-May-29 22:43 ProphetLite-0.0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1734 b- defN 23-May-29 22:43 ProphetLite-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-29 22:43 ProphetLite-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-May-29 22:43 ProphetLite-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      806 b- defN 23-May-29 22:43 ProphetLite-0.0.2.dist-info/RECORD
+10 files, 15556 bytes uncompressed, 5155 bytes compressed:  66.9%
```

## zipnote {}

```diff
@@ -1,16 +1,31 @@
-Filename: ProphetLite-0.0.1.dist-info/LICENSE
+Filename: ProphetLite/__init__.py
 Comment: 
 
-Filename: ProphetLite-0.0.1.dist-info/METADATA
+Filename: ProphetLite/fourier.py
 Comment: 
 
-Filename: ProphetLite-0.0.1.dist-info/WHEEL
+Filename: ProphetLite/linear_basis.py
 Comment: 
 
-Filename: ProphetLite-0.0.1.dist-info/top_level.txt
+Filename: ProphetLite/model.py
 Comment: 
 
-Filename: ProphetLite-0.0.1.dist-info/RECORD
+Filename: ProphetLite/prophetlite.py
+Comment: 
+
+Filename: ProphetLite-0.0.2.dist-info/LICENSE
+Comment: 
+
+Filename: ProphetLite-0.0.2.dist-info/METADATA
+Comment: 
+
+Filename: ProphetLite-0.0.2.dist-info/WHEEL
+Comment: 
+
+Filename: ProphetLite-0.0.2.dist-info/top_level.txt
+Comment: 
+
+Filename: ProphetLite-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ProphetLite-0.0.1.dist-info/LICENSE` & `ProphetLite-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ProphetLite-0.0.1.dist-info/METADATA` & `ProphetLite-0.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ProphetLite
-Version: 0.0.1
+Version: 0.0.2
 Summary: Like Prophet but using Numba and LASSO.
 Home-page: https://github.com/tblume1992/ProphetLite
 Author: Tyler Blume
 Author-email: tblume@mail.USF.edu
 Keywords: forecasting,time series,seasonality,trend
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

