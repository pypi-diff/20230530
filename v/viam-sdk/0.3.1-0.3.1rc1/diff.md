# Comparing `tmp/viam_sdk-0.3.1-py3-none-manylinux2014_x86_64.whl.zip` & `tmp/viam_sdk-0.3.1rc1-py3-none-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 9907073 bytes, number of entries: 372
+Zip file size: 9907100 bytes, number of entries: 372
 -rw-r--r--  2.0 unx    11358 b- defN 80-Jan-01 00:00 LICENSE
 -rw-r--r--  2.0 unx     1411 b- defN 80-Jan-01 00:00 viam/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 viam/components/__init__.py
 -rw-r--r--  2.0 unx     1075 b- defN 80-Jan-01 00:00 viam/components/arm/__init__.py
 -rw-r--r--  2.0 unx     2870 b- defN 80-Jan-01 00:00 viam/components/arm/arm.py
 -rw-r--r--  2.0 unx     3734 b- defN 80-Jan-01 00:00 viam/components/arm/client.py
 -rw-r--r--  2.0 unx     5124 b- defN 80-Jan-01 00:00 viam/components/arm/service.py
@@ -363,12 +363,12 @@
 -rw-r--r--  2.0 unx      369 b- defN 80-Jan-01 00:00 viam/services/slam/__init__.py
 -rw-r--r--  2.0 unx     2181 b- defN 80-Jan-01 00:00 viam/services/slam/client.py
 -rw-r--r--  2.0 unx     3173 b- defN 80-Jan-01 00:00 viam/services/slam/service.py
 -rw-r--r--  2.0 unx     1633 b- defN 80-Jan-01 00:00 viam/services/slam/slam.py
 -rw-r--r--  2.0 unx      134 b- defN 80-Jan-01 00:00 viam/services/vision/__init__.py
 -rw-r--r--  2.0 unx     8133 b- defN 80-Jan-01 00:00 viam/services/vision/client.py
 -rw-r--r--  2.0 unx     7927 b- defN 80-Jan-01 00:00 viam/utils.py
--rw-r--r--  2.0 unx    11358 b- defN 80-Jan-01 00:00 viam_sdk-0.3.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     7385 b- defN 80-Jan-01 00:00 viam_sdk-0.3.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 viam_sdk-0.3.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx    34341 b- defN 16-Jan-01 00:00 viam_sdk-0.3.1.dist-info/RECORD
-372 files, 30310549 bytes uncompressed, 9851755 bytes compressed:  67.5%
+-rw-r--r--  2.0 unx    11358 b- defN 80-Jan-01 00:00 viam_sdk-0.3.1rc1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7388 b- defN 80-Jan-01 00:00 viam_sdk-0.3.1rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 viam_sdk-0.3.1rc1.dist-info/WHEEL
+?rw-r--r--  2.0 unx    34353 b- defN 16-Jan-01 00:00 viam_sdk-0.3.1rc1.dist-info/RECORD
+372 files, 30310564 bytes uncompressed, 9851758 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -1098,20 +1098,20 @@
 
 Filename: viam/services/vision/client.py
 Comment: 
 
 Filename: viam/utils.py
 Comment: 
 
-Filename: viam_sdk-0.3.1.dist-info/LICENSE
+Filename: viam_sdk-0.3.1rc1.dist-info/LICENSE
 Comment: 
 
-Filename: viam_sdk-0.3.1.dist-info/METADATA
+Filename: viam_sdk-0.3.1rc1.dist-info/METADATA
 Comment: 
 
-Filename: viam_sdk-0.3.1.dist-info/WHEEL
+Filename: viam_sdk-0.3.1rc1.dist-info/WHEEL
 Comment: 
 
-Filename: viam_sdk-0.3.1.dist-info/RECORD
+Filename: viam_sdk-0.3.1rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `viam_sdk-0.3.1.dist-info/LICENSE` & `viam_sdk-0.3.1rc1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `viam_sdk-0.3.1.dist-info/METADATA` & `viam_sdk-0.3.1rc1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viam-sdk
-Version: 0.3.1
+Version: 0.3.1rc1
 Summary: Viam Robotics Python SDK
 License: Apache-2.0
 Author: Naveed
 Author-email: naveed@viam.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `viam_sdk-0.3.1.dist-info/RECORD` & `viam_sdk-0.3.1rc1.dist-info/RECORD`

 * *Files 0% similar despite different names*

```diff
@@ -362,11 +362,11 @@
 viam/services/slam/__init__.py,sha256=ybSjAFas69OVwy2RltL1CUhwAs1E0nHClObEaIZ_1s4,369
 viam/services/slam/client.py,sha256=co-PshdxsuJJVJPpJToTbhOy8H92fGtoB_AVjHFWwS8,2181
 viam/services/slam/service.py,sha256=oXO6Nr2VZWonPO7YovUjjVv28uzUTKphhezvxNuiYXc,3173
 viam/services/slam/slam.py,sha256=872OV9JvSEvwWRBDiX-P8Zs87fNBp-5mbMx4ruot-gY,1633
 viam/services/vision/__init__.py,sha256=3DddNMlIAwC9TJORUmOk9qbb_Wpb_B6ekGWO0Awj67A,134
 viam/services/vision/client.py,sha256=VrxoKC7hxlSZOgU8b32M9hFPMcRvwlnZ4feSzB3656Q,8133
 viam/utils.py,sha256=gGoMOLkeJSerDIH2nPDydTfL7-p2AWqZCMU4jQEp0go,7927
-viam_sdk-0.3.1.dist-info/LICENSE,sha256=yVuuHRzgI17MzTVgt3LsHvuX80innw--CmNPDCzO_iw,11358
-viam_sdk-0.3.1.dist-info/METADATA,sha256=T-P8r_yGQw-fG_lwIGU2sp2WGPQDyAVdKhMaEsdT8MY,7385
-viam_sdk-0.3.1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-viam_sdk-0.3.1.dist-info/RECORD,,
+viam_sdk-0.3.1rc1.dist-info/LICENSE,sha256=yVuuHRzgI17MzTVgt3LsHvuX80innw--CmNPDCzO_iw,11358
+viam_sdk-0.3.1rc1.dist-info/METADATA,sha256=-E-spjBe-Mx8NZVWbsRJ8wg92OcOlz46scMchlNiY8A,7388
+viam_sdk-0.3.1rc1.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
+viam_sdk-0.3.1rc1.dist-info/RECORD,,
```

