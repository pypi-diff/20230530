# Comparing `tmp/mb_pandas-1.0.202305291017-py3-none-any.whl.zip` & `tmp/mb_pandas-1.0.202305301226-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 9363 bytes, number of entries: 13
+Zip file size: 9582 bytes, number of entries: 13
 -rw-rw-r--  2.0 unx      162 b- defN 23-May-25 03:48 mb_pandas/src/__init__.py
 -rw-rw-r--  2.0 unx     1612 b- defN 23-May-25 03:36 mb_pandas/src/aio.py
 -rw-rw-r--  2.0 unx      482 b- defN 23-May-25 03:36 mb_pandas/src/convert_data.py
 -rw-rw-r--  2.0 unx     3516 b- defN 23-May-29 10:17 mb_pandas/src/dfload.py
 -rw-rw-r--  2.0 unx     2418 b- defN 23-May-25 03:36 mb_pandas/src/profiler.py
--rw-rw-r--  2.0 unx     6091 b- defN 23-Apr-04 14:19 mb_pandas/src/transform.py
--rw-rw-r--  2.0 unx      396 b- defN 23-May-29 10:17 mb_pandas/src/version.py
--rwxrwxr-x  2.0 unx     1671 b- defN 23-May-29 10:17 mb_pandas-1.0.202305291017.data/scripts/df_profile
--rwxrwxr-x  2.0 unx     3683 b- defN 23-May-29 10:17 mb_pandas-1.0.202305291017.data/scripts/df_view
--rw-rw-r--  2.0 unx      224 b- defN 23-May-29 10:17 mb_pandas-1.0.202305291017.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-29 10:17 mb_pandas-1.0.202305291017.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-May-29 10:17 mb_pandas-1.0.202305291017.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1128 b- defN 23-May-29 10:17 mb_pandas-1.0.202305291017.dist-info/RECORD
-13 files, 21485 bytes uncompressed, 7455 bytes compressed:  65.3%
+-rw-rw-r--  2.0 unx     6678 b- defN 23-May-30 12:26 mb_pandas/src/transform.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-May-30 12:26 mb_pandas/src/version.py
+-rwxrwxr-x  2.0 unx     1671 b- defN 23-May-30 12:27 mb_pandas-1.0.202305301226.data/scripts/df_profile
+-rwxrwxr-x  2.0 unx     3683 b- defN 23-May-30 12:27 mb_pandas-1.0.202305301226.data/scripts/df_view
+-rw-rw-r--  2.0 unx      224 b- defN 23-May-30 12:27 mb_pandas-1.0.202305301226.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-30 12:27 mb_pandas-1.0.202305301226.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-May-30 12:27 mb_pandas-1.0.202305301226.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1128 b- defN 23-May-30 12:27 mb_pandas-1.0.202305301226.dist-info/RECORD
+13 files, 22072 bytes uncompressed, 7674 bytes compressed:  65.2%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: mb_pandas/src/transform.py
 Comment: 
 
 Filename: mb_pandas/src/version.py
 Comment: 
 
-Filename: mb_pandas-1.0.202305291017.data/scripts/df_profile
+Filename: mb_pandas-1.0.202305301226.data/scripts/df_profile
 Comment: 
 
-Filename: mb_pandas-1.0.202305291017.data/scripts/df_view
+Filename: mb_pandas-1.0.202305301226.data/scripts/df_view
 Comment: 
 
-Filename: mb_pandas-1.0.202305291017.dist-info/METADATA
+Filename: mb_pandas-1.0.202305301226.dist-info/METADATA
 Comment: 
 
-Filename: mb_pandas-1.0.202305291017.dist-info/WHEEL
+Filename: mb_pandas-1.0.202305301226.dist-info/WHEEL
 Comment: 
 
-Filename: mb_pandas-1.0.202305291017.dist-info/top_level.txt
+Filename: mb_pandas-1.0.202305301226.dist-info/top_level.txt
 Comment: 
 
-Filename: mb_pandas-1.0.202305291017.dist-info/RECORD
+Filename: mb_pandas-1.0.202305301226.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mb_pandas/src/transform.py

```diff
@@ -3,15 +3,39 @@
 import pandas as pd
 import os
 from .dfload import load_any_df
 from mb_utils.src.logging import logger
 import numpy as np
 import cv2
 
-__all__ = ['check_null','remove_unnamed','rename_columns','check_drop_duplicates','get_dftype']
+__all__ = ['check_null','remove_unnamed','rename_columns','check_drop_duplicates','get_dftype','merge_chuck']
+
+
+def merge_chuck(df1,df2,chunksize=10000,logger=None,**kwargs):
+    """
+    Merging 2 DataFrames in chunks
+    
+    Args:
+        df1 : First DataFrame
+        df2 : Second DataFrame
+        chunksize : chunksize to merge
+        logger : logger
+    Returns:
+        df : merged DataFrame
+    """
+    if df1.shape[0] > df2.shape[0]:
+        df1,df2 = df2,df1
+    
+    list_df = [df2[i:i+chunksize] for i in range(0, df2.shape[0],chunksize)]
+    res = pd.DataFrame() 
+
+    for chunk in list_df:
+        res = pd.concat([res, df1.merge(chunk,**kwargs)])
+    return res
+    
 
 def check_null(file_path,fillna=False,logger=None) -> pd.DataFrame:
     """
     Pandas file checker. Checks Null values
     Input: 
         file_path (csv): path to csv file
         fillna (bool): fillna with False
```

## mb_pandas/src/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('05')
-VERSION_DAY = int('29')
-VERSION_HOUR = int('10')
-VERSION_MINUTE = int('17')
+VERSION_DAY = int('30')
+VERSION_HOUR = int('12')
+VERSION_MINUTE = int('26')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202305291017
-version_date = '2023/05/29 10:17'
+PATCH_VERSION = 202305301226
+version_date = '2023/05/30 12:26'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `mb_pandas-1.0.202305291017.data/scripts/df_profile` & `mb_pandas-1.0.202305301226.data/scripts/df_profile`

 * *Files identical despite different names*

## Comparing `mb_pandas-1.0.202305291017.data/scripts/df_view` & `mb_pandas-1.0.202305301226.data/scripts/df_view`

 * *Files identical despite different names*

## Comparing `mb_pandas-1.0.202305291017.dist-info/RECORD` & `mb_pandas-1.0.202305301226.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 mb_pandas/src/__init__.py,sha256=WU80RSEXwgPXneLCZV_JyaMkKzAGEvYo9Icq0QzfBJE,162
 mb_pandas/src/aio.py,sha256=UK3o2TMFDeNQvhiFAulAyd1fKJPjrShEbK-Y-85tlsM,1612
 mb_pandas/src/convert_data.py,sha256=Wp1yDT9Ie-lBZGE7WmsMXB7nN3mv0MwbiloInr1aoc0,482
 mb_pandas/src/dfload.py,sha256=Yet5dq8R0NDi69UXiUAfQMwbWqhLRGjXqhUvJI5pBSw,3516
 mb_pandas/src/profiler.py,sha256=iX_nAksh-HzjyhQLnbutvEtNVGfVwja2CsQ1zaYZbeA,2418
-mb_pandas/src/transform.py,sha256=Pq-xTzpfktzAlpu4dg42Kd6uoSI5mcq8vHhetFhgDUM,6091
-mb_pandas/src/version.py,sha256=r9EY8Si-2jT7bo407jqyZmS5iTZeshf1SxOT4X365d4,396
-mb_pandas-1.0.202305291017.data/scripts/df_profile,sha256=zi4GRNQ6P5_JEB_0wMYB1KzLRG59eHXxRZG_I84lTYQ,1671
-mb_pandas-1.0.202305291017.data/scripts/df_view,sha256=BbS_rNgrPl7Raz_zVmTBqw_dvyAhc3-KqS4W2LV0_yo,3683
-mb_pandas-1.0.202305291017.dist-info/METADATA,sha256=B7nAjdhT6Ui67ENDTE5aDn7Aso-gU6B5GlC1iEkG95Q,224
-mb_pandas-1.0.202305291017.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-mb_pandas-1.0.202305291017.dist-info/top_level.txt,sha256=5JkDz2-6yNAp6GiwpeR4FpxqXVysaksS5MD1iAvfMgo,10
-mb_pandas-1.0.202305291017.dist-info/RECORD,,
+mb_pandas/src/transform.py,sha256=4zBejQoRoVJWizxFrHzsExa2va3AjLGB8eF6d-qf0MI,6678
+mb_pandas/src/version.py,sha256=dn27Q7tVsd_dzkKENpaYZ1OYUZXXOyuO7szhL-dMMKM,396
+mb_pandas-1.0.202305301226.data/scripts/df_profile,sha256=zi4GRNQ6P5_JEB_0wMYB1KzLRG59eHXxRZG_I84lTYQ,1671
+mb_pandas-1.0.202305301226.data/scripts/df_view,sha256=BbS_rNgrPl7Raz_zVmTBqw_dvyAhc3-KqS4W2LV0_yo,3683
+mb_pandas-1.0.202305301226.dist-info/METADATA,sha256=74u7a19Cb0FCTkjuwwrZFl726nHGcLLF42bLB_-SGA0,224
+mb_pandas-1.0.202305301226.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+mb_pandas-1.0.202305301226.dist-info/top_level.txt,sha256=5JkDz2-6yNAp6GiwpeR4FpxqXVysaksS5MD1iAvfMgo,10
+mb_pandas-1.0.202305301226.dist-info/RECORD,,
```

