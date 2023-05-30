# Comparing `tmp/mb_pandas-1.0.202305301240-py3-none-any.whl.zip` & `tmp/mb_pandas-1.0.202305301527-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 9591 bytes, number of entries: 13
+Zip file size: 9704 bytes, number of entries: 13
 -rw-rw-r--  2.0 unx      162 b- defN 23-May-25 03:48 mb_pandas/src/__init__.py
 -rw-rw-r--  2.0 unx     1612 b- defN 23-May-25 03:36 mb_pandas/src/aio.py
 -rw-rw-r--  2.0 unx      482 b- defN 23-May-25 03:36 mb_pandas/src/convert_data.py
 -rw-rw-r--  2.0 unx     3516 b- defN 23-May-29 10:17 mb_pandas/src/dfload.py
 -rw-rw-r--  2.0 unx     2418 b- defN 23-May-25 03:36 mb_pandas/src/profiler.py
--rw-rw-r--  2.0 unx     6721 b- defN 23-May-30 12:40 mb_pandas/src/transform.py
--rw-rw-r--  2.0 unx      396 b- defN 23-May-30 12:40 mb_pandas/src/version.py
--rwxrwxr-x  2.0 unx     1671 b- defN 23-May-30 12:40 mb_pandas-1.0.202305301240.data/scripts/df_profile
--rwxrwxr-x  2.0 unx     3683 b- defN 23-May-30 12:40 mb_pandas-1.0.202305301240.data/scripts/df_view
--rw-rw-r--  2.0 unx      224 b- defN 23-May-30 12:40 mb_pandas-1.0.202305301240.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-30 12:40 mb_pandas-1.0.202305301240.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-May-30 12:40 mb_pandas-1.0.202305301240.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1128 b- defN 23-May-30 12:40 mb_pandas-1.0.202305301240.dist-info/RECORD
-13 files, 22115 bytes uncompressed, 7683 bytes compressed:  65.3%
+-rw-rw-r--  2.0 unx     7018 b- defN 23-May-30 15:26 mb_pandas/src/transform.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-May-30 15:27 mb_pandas/src/version.py
+-rwxrwxr-x  2.0 unx     1671 b- defN 23-May-30 15:27 mb_pandas-1.0.202305301527.data/scripts/df_profile
+-rwxrwxr-x  2.0 unx     3683 b- defN 23-May-30 15:27 mb_pandas-1.0.202305301527.data/scripts/df_view
+-rw-rw-r--  2.0 unx      224 b- defN 23-May-30 15:27 mb_pandas-1.0.202305301527.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-30 15:27 mb_pandas-1.0.202305301527.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-May-30 15:27 mb_pandas-1.0.202305301527.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1128 b- defN 23-May-30 15:27 mb_pandas-1.0.202305301527.dist-info/RECORD
+13 files, 22412 bytes uncompressed, 7796 bytes compressed:  65.2%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: mb_pandas/src/transform.py
 Comment: 
 
 Filename: mb_pandas/src/version.py
 Comment: 
 
-Filename: mb_pandas-1.0.202305301240.data/scripts/df_profile
+Filename: mb_pandas-1.0.202305301527.data/scripts/df_profile
 Comment: 
 
-Filename: mb_pandas-1.0.202305301240.data/scripts/df_view
+Filename: mb_pandas-1.0.202305301527.data/scripts/df_view
 Comment: 
 
-Filename: mb_pandas-1.0.202305301240.dist-info/METADATA
+Filename: mb_pandas-1.0.202305301527.dist-info/METADATA
 Comment: 
 
-Filename: mb_pandas-1.0.202305301240.dist-info/WHEEL
+Filename: mb_pandas-1.0.202305301527.dist-info/WHEEL
 Comment: 
 
-Filename: mb_pandas-1.0.202305301240.dist-info/top_level.txt
+Filename: mb_pandas-1.0.202305301527.dist-info/top_level.txt
 Comment: 
 
-Filename: mb_pandas-1.0.202305301240.dist-info/RECORD
+Filename: mb_pandas-1.0.202305301527.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mb_pandas/src/transform.py

```diff
@@ -2,39 +2,48 @@
 
 import pandas as pd
 import os
 from .dfload import load_any_df
 from mb_utils.src.logging import logger
 import numpy as np
 import cv2
-from mb_utils.src.extra import timer
 
 __all__ = ['check_null','remove_unnamed','rename_columns','check_drop_duplicates','get_dftype','merge_chunk']
 
-@timer
 def merge_chunk(df1,df2,chunksize=10000,logger=None,**kwargs):
     """
     Merging 2 DataFrames in chunks
     
     Args:
         df1 : First DataFrame
         df2 : Second DataFrame
         chunksize : chunksize to merge
         logger : logger
     Returns:
         df : merged DataFrame
     """
     if df1.shape[0] > df2.shape[0]:
         df1,df2 = df2,df1
+
+    merge_on = set(df1.columns) & set(df2.columns)
+    if not merge_on:
+        raise ValueError("No common columns to merge on") 
     
     list_df = [df2[i:i+chunksize] for i in range(0, df2.shape[0],chunksize)]
+    if logger:
+        logger.info(f'Size of chunk: {chunksize}')
+        logger.info(f'Number of chunks: {len(list_df)}')
+    
     res = pd.DataFrame() 
 
     for chunk in list_df:
-        res = pd.concat([res, df1.merge(chunk,**kwargs)])
+        merged_chunk = pd.merge(df1,chunk,**kwargs)
+        res = pd.concat([res, merged_chunk])
+    
+    res = res.reset_index(drop=True)
     return res
     
 
 def check_null(file_path,fillna=False,logger=None) -> pd.DataFrame:
     """
     Pandas file checker. Checks Null values
     Input:
```

## mb_pandas/src/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('05')
 VERSION_DAY = int('30')
-VERSION_HOUR = int('12')
-VERSION_MINUTE = int('40')
+VERSION_HOUR = int('15')
+VERSION_MINUTE = int('27')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202305301240
-version_date = '2023/05/30 12:40'
+PATCH_VERSION = 202305301527
+version_date = '2023/05/30 15:27'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `mb_pandas-1.0.202305301240.data/scripts/df_profile` & `mb_pandas-1.0.202305301527.data/scripts/df_profile`

 * *Files identical despite different names*

## Comparing `mb_pandas-1.0.202305301240.data/scripts/df_view` & `mb_pandas-1.0.202305301527.data/scripts/df_view`

 * *Files identical despite different names*

## Comparing `mb_pandas-1.0.202305301240.dist-info/RECORD` & `mb_pandas-1.0.202305301527.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 mb_pandas/src/__init__.py,sha256=WU80RSEXwgPXneLCZV_JyaMkKzAGEvYo9Icq0QzfBJE,162
 mb_pandas/src/aio.py,sha256=UK3o2TMFDeNQvhiFAulAyd1fKJPjrShEbK-Y-85tlsM,1612
 mb_pandas/src/convert_data.py,sha256=Wp1yDT9Ie-lBZGE7WmsMXB7nN3mv0MwbiloInr1aoc0,482
 mb_pandas/src/dfload.py,sha256=Yet5dq8R0NDi69UXiUAfQMwbWqhLRGjXqhUvJI5pBSw,3516
 mb_pandas/src/profiler.py,sha256=iX_nAksh-HzjyhQLnbutvEtNVGfVwja2CsQ1zaYZbeA,2418
-mb_pandas/src/transform.py,sha256=CGF3uikSnpV4E0gYaOQJED16P9797hC6n-OjhpPtYwo,6721
-mb_pandas/src/version.py,sha256=CYWP2wTK-i4cbqP9zQL7PBxePmpxbAHV2CFyQDtTkJo,396
-mb_pandas-1.0.202305301240.data/scripts/df_profile,sha256=zi4GRNQ6P5_JEB_0wMYB1KzLRG59eHXxRZG_I84lTYQ,1671
-mb_pandas-1.0.202305301240.data/scripts/df_view,sha256=BbS_rNgrPl7Raz_zVmTBqw_dvyAhc3-KqS4W2LV0_yo,3683
-mb_pandas-1.0.202305301240.dist-info/METADATA,sha256=M_ZgNcGplhCHb5tDPBb7JKF9BEaB1ijSD9oqKO5Bfi4,224
-mb_pandas-1.0.202305301240.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-mb_pandas-1.0.202305301240.dist-info/top_level.txt,sha256=5JkDz2-6yNAp6GiwpeR4FpxqXVysaksS5MD1iAvfMgo,10
-mb_pandas-1.0.202305301240.dist-info/RECORD,,
+mb_pandas/src/transform.py,sha256=OEzePaeekz28iJgl_nXKIhjxKQ8AXFwdUuRVWd2pua8,7018
+mb_pandas/src/version.py,sha256=ea0yJKpESujyAetJm0I2EpTWwm8fF_iJkmmc60HGqkk,396
+mb_pandas-1.0.202305301527.data/scripts/df_profile,sha256=zi4GRNQ6P5_JEB_0wMYB1KzLRG59eHXxRZG_I84lTYQ,1671
+mb_pandas-1.0.202305301527.data/scripts/df_view,sha256=BbS_rNgrPl7Raz_zVmTBqw_dvyAhc3-KqS4W2LV0_yo,3683
+mb_pandas-1.0.202305301527.dist-info/METADATA,sha256=iJSEc3Q5juAQnDH-KPDlWSDu_DFBWXpO68dJ48RpH6I,224
+mb_pandas-1.0.202305301527.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+mb_pandas-1.0.202305301527.dist-info/top_level.txt,sha256=5JkDz2-6yNAp6GiwpeR4FpxqXVysaksS5MD1iAvfMgo,10
+mb_pandas-1.0.202305301527.dist-info/RECORD,,
```

