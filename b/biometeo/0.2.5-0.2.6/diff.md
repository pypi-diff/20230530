# Comparing `tmp/biometeo-0.2.5-cp39-cp39-win_amd64.whl.zip` & `tmp/biometeo-0.2.6-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,11 @@
-Zip file size: 574674 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat   130560 b- defN 23-May-19 02:08 biometeo/Tmrt_utils.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat  1282560 b- defN 23-May-19 02:08 biometeo/__init__.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1417 b- defN 23-May-19 02:08 biometeo-0.2.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-19 02:08 biometeo-0.2.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-19 02:08 biometeo-0.2.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      495 b- defN 23-May-19 02:08 biometeo-0.2.5.dist-info/RECORD
-6 files, 1415141 bytes uncompressed, 573784 bytes compressed:  59.5%
+Zip file size: 4158783 bytes, number of entries: 9
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-29 11:40 biometeo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-29 11:40 biometeo.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-29 11:40 biometeo-0.2.6.dist-info/
+-rwxr-xr-x  2.0 unx  1309488 b- defN 23-May-29 11:40 biometeo/Tmrt_utils.cpython-39-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx 15705296 b- defN 23-May-29 11:40 biometeo/__init__.cpython-39-x86_64-linux-gnu.so
+-rw-rw-r--  2.0 unx      527 b- defN 23-May-29 11:40 biometeo-0.2.6.dist-info/RECORD
+-rw-r--r--  2.0 unx        9 b- defN 23-May-29 11:40 biometeo-0.2.6.dist-info/top_level.txt
+-rw-r--r--  2.0 unx     1399 b- defN 23-May-29 11:40 biometeo-0.2.6.dist-info/METADATA
+-rw-r--r--  2.0 unx      148 b- defN 23-May-29 11:40 biometeo-0.2.6.dist-info/WHEEL
+9 files, 17016867 bytes uncompressed, 4157521 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -1,19 +1,28 @@
-Filename: biometeo/Tmrt_utils.cp39-win_amd64.pyd
+Filename: biometeo/
 Comment: 
 
-Filename: biometeo/__init__.cp39-win_amd64.pyd
+Filename: biometeo.libs/
 Comment: 
 
-Filename: biometeo-0.2.5.dist-info/METADATA
+Filename: biometeo-0.2.6.dist-info/
 Comment: 
 
-Filename: biometeo-0.2.5.dist-info/WHEEL
+Filename: biometeo/Tmrt_utils.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: biometeo-0.2.5.dist-info/top_level.txt
+Filename: biometeo/__init__.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: biometeo-0.2.5.dist-info/RECORD
+Filename: biometeo-0.2.6.dist-info/RECORD
+Comment: 
+
+Filename: biometeo-0.2.6.dist-info/top_level.txt
+Comment: 
+
+Filename: biometeo-0.2.6.dist-info/METADATA
+Comment: 
+
+Filename: biometeo-0.2.6.dist-info/WHEEL
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## Comparing `biometeo-0.2.5.dist-info/METADATA` & `biometeo-0.2.6.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1
-Name: biometeo
-Version: 0.2.5
-Summary: This package is applied to calculate thermal indicators for human biometeorology.  The available thermal indicators are Physiological Equivalent Temperature (PET), modified Physiological Equivalent Temperature (mPET), Predicted Mean Vote (PMV), Standard Effective Temperature* (SET*) and Universal Thermal Climate Index (UTCI) in this package.  An additional function named GlobalRadiation_Tmrt is appended in the package for applying G, N, and Omega to calculate Tmrt from part of original RayMan model code.
-Home-page: UNKNOWN
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Dist: numpy (>=1.19.2)
-Requires-Dist: Cython (>=0.29.28)
-
-This package is applied to calculate thermal indicators for human biometeorology.
-The available thermal indicators are Physiological Equivalent Temperature (PET), modified Physiological Equivalent Temperature (mPET), Predicted Mean Vote (PMV), Standard Effective Temperature* (SET*) and Universal Thermal Climate Index (UTCI) in this package.
-An additional function named GlobalRadiation_Tmrt is appended in the package for applying G, N, and Omega to calculate Tmrt from part of original RayMan model code.
-
-Copyright: (CC BY-NC-ND 3.0 TW) National Chung Hsing University, Dr. Yung-Chang Chen, Prof. Kang-Ting Tsai and Prof. Andreas Matzarakis, 2022.
-
-Contact: Dr. Yung-Chang Chen, ycchen0422@gmail.com .
-
+Metadata-Version: 2.1
+Name: biometeo
+Version: 0.2.6
+Summary: This package is applied to calculate thermal indicators for human biometeorology.  The available thermal indicators are Physiological Equivalent Temperature (PET), modified Physiological Equivalent Temperature (mPET), Predicted Mean Vote (PMV), Standard Effective Temperature* (SET*) and Universal Thermal Climate Index (UTCI) in this package.  An additional function named GlobalRadiation_Tmrt is appended in the package for applying G, N, and Omega to calculate Tmrt from part of original RayMan model code.
+Home-page: UNKNOWN
+License: UNKNOWN
+Platform: UNKNOWN
+Requires-Dist: numpy (>=1.19.2)
+Requires-Dist: Cython (>=0.29.28)
+
+This package is applied to calculate thermal indicators for human biometeorology.
+The available thermal indicators are Physiological Equivalent Temperature (PET), modified Physiological Equivalent Temperature (mPET), Predicted Mean Vote (PMV), Standard Effective Temperature* (SET*) and Universal Thermal Climate Index (UTCI) in this package.
+An additional function named GlobalRadiation_Tmrt is appended in the package for applying G, N, and Omega to calculate Tmrt from part of original RayMan model code.
+
+Copyright: (CC BY-NC-ND 3.0 TW) National Chung Hsing University, Dr. Yung-Chang Chen, Prof. Kang-Ting Tsai and Prof. Andreas Matzarakis, 2022.
+
+Contact: Dr. Yung-Chang Chen, ycchen0422@gmail.com .
+
```

