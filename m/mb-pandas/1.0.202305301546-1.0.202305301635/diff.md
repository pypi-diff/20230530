# Comparing `tmp/mb_pandas-1.0.202305301546-py3-none-any.whl.zip` & `tmp/mb_pandas-1.0.202305301635-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 9755 bytes, number of entries: 13
+Zip file size: 9750 bytes, number of entries: 13
 -rw-rw-r--  2.0 unx      162 b- defN 23-May-25 03:48 mb_pandas/src/__init__.py
 -rw-rw-r--  2.0 unx     1612 b- defN 23-May-25 03:36 mb_pandas/src/aio.py
 -rw-rw-r--  2.0 unx      482 b- defN 23-May-25 03:36 mb_pandas/src/convert_data.py
 -rw-rw-r--  2.0 unx     3516 b- defN 23-May-29 10:17 mb_pandas/src/dfload.py
 -rw-rw-r--  2.0 unx     2418 b- defN 23-May-25 03:36 mb_pandas/src/profiler.py
--rw-rw-r--  2.0 unx     7271 b- defN 23-May-30 15:46 mb_pandas/src/transform.py
--rw-rw-r--  2.0 unx      396 b- defN 23-May-30 15:46 mb_pandas/src/version.py
--rwxrwxr-x  2.0 unx     1671 b- defN 23-May-30 15:47 mb_pandas-1.0.202305301546.data/scripts/df_profile
--rwxrwxr-x  2.0 unx     3683 b- defN 23-May-30 15:47 mb_pandas-1.0.202305301546.data/scripts/df_view
--rw-rw-r--  2.0 unx      224 b- defN 23-May-30 15:47 mb_pandas-1.0.202305301546.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-30 15:47 mb_pandas-1.0.202305301546.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-May-30 15:47 mb_pandas-1.0.202305301546.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1128 b- defN 23-May-30 15:47 mb_pandas-1.0.202305301546.dist-info/RECORD
-13 files, 22665 bytes uncompressed, 7847 bytes compressed:  65.4%
+-rw-rw-r--  2.0 unx     7226 b- defN 23-May-30 16:35 mb_pandas/src/transform.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-May-30 16:35 mb_pandas/src/version.py
+-rwxrwxr-x  2.0 unx     1671 b- defN 23-May-30 16:35 mb_pandas-1.0.202305301635.data/scripts/df_profile
+-rwxrwxr-x  2.0 unx     3683 b- defN 23-May-30 16:35 mb_pandas-1.0.202305301635.data/scripts/df_view
+-rw-rw-r--  2.0 unx      224 b- defN 23-May-30 16:35 mb_pandas-1.0.202305301635.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-30 16:35 mb_pandas-1.0.202305301635.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-May-30 16:35 mb_pandas-1.0.202305301635.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1128 b- defN 23-May-30 16:35 mb_pandas-1.0.202305301635.dist-info/RECORD
+13 files, 22620 bytes uncompressed, 7842 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: mb_pandas/src/transform.py
 Comment: 
 
 Filename: mb_pandas/src/version.py
 Comment: 
 
-Filename: mb_pandas-1.0.202305301546.data/scripts/df_profile
+Filename: mb_pandas-1.0.202305301635.data/scripts/df_profile
 Comment: 
 
-Filename: mb_pandas-1.0.202305301546.data/scripts/df_view
+Filename: mb_pandas-1.0.202305301635.data/scripts/df_view
 Comment: 
 
-Filename: mb_pandas-1.0.202305301546.dist-info/METADATA
+Filename: mb_pandas-1.0.202305301635.dist-info/METADATA
 Comment: 
 
-Filename: mb_pandas-1.0.202305301546.dist-info/WHEEL
+Filename: mb_pandas-1.0.202305301635.dist-info/WHEEL
 Comment: 
 
-Filename: mb_pandas-1.0.202305301546.dist-info/top_level.txt
+Filename: mb_pandas-1.0.202305301635.dist-info/top_level.txt
 Comment: 
 
-Filename: mb_pandas-1.0.202305301546.dist-info/RECORD
+Filename: mb_pandas-1.0.202305301635.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mb_pandas/src/transform.py

```diff
@@ -35,17 +35,15 @@
     
     merged_chunks = []
 
     for chunk in list_df:
         merged_chunk = pd.merge(df1, chunk, **kwargs)
         merged_chunks.append(merged_chunk)
 
-    res = pd.DataFrame() 
-    res = pd.concat(merged_chunks)
-    res = res.reset_index(drop=True)
+    res = pd.concat(merged_chunks,ignore_index=True)
     return res    
     
     # for chunk in list_df:
     #     merged_chunk = pd.merge(df1,chunk,**kwargs)
     #     res = pd.concat([res, merged_chunk])
     
     # res = res.reset_index(drop=True)
```

## mb_pandas/src/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('05')
 VERSION_DAY = int('30')
-VERSION_HOUR = int('15')
-VERSION_MINUTE = int('46')
+VERSION_HOUR = int('16')
+VERSION_MINUTE = int('35')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202305301546
-version_date = '2023/05/30 15:46'
+PATCH_VERSION = 202305301635
+version_date = '2023/05/30 16:35'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `mb_pandas-1.0.202305301546.data/scripts/df_profile` & `mb_pandas-1.0.202305301635.data/scripts/df_profile`

 * *Files identical despite different names*

## Comparing `mb_pandas-1.0.202305301546.data/scripts/df_view` & `mb_pandas-1.0.202305301635.data/scripts/df_view`

 * *Files identical despite different names*

## Comparing `mb_pandas-1.0.202305301546.dist-info/RECORD` & `mb_pandas-1.0.202305301635.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 mb_pandas/src/__init__.py,sha256=WU80RSEXwgPXneLCZV_JyaMkKzAGEvYo9Icq0QzfBJE,162
 mb_pandas/src/aio.py,sha256=UK3o2TMFDeNQvhiFAulAyd1fKJPjrShEbK-Y-85tlsM,1612
 mb_pandas/src/convert_data.py,sha256=Wp1yDT9Ie-lBZGE7WmsMXB7nN3mv0MwbiloInr1aoc0,482
 mb_pandas/src/dfload.py,sha256=Yet5dq8R0NDi69UXiUAfQMwbWqhLRGjXqhUvJI5pBSw,3516
 mb_pandas/src/profiler.py,sha256=iX_nAksh-HzjyhQLnbutvEtNVGfVwja2CsQ1zaYZbeA,2418
-mb_pandas/src/transform.py,sha256=Qm98bHkxoQha7lRpjyW_doR4FF94Vs-pKHxQaw6jkZg,7271
-mb_pandas/src/version.py,sha256=3Z22anLKRFjaQWepVfAFgGeYWyEpnz8P5BXZlPC-F5c,396
-mb_pandas-1.0.202305301546.data/scripts/df_profile,sha256=zi4GRNQ6P5_JEB_0wMYB1KzLRG59eHXxRZG_I84lTYQ,1671
-mb_pandas-1.0.202305301546.data/scripts/df_view,sha256=BbS_rNgrPl7Raz_zVmTBqw_dvyAhc3-KqS4W2LV0_yo,3683
-mb_pandas-1.0.202305301546.dist-info/METADATA,sha256=OeCL5j3eWM7Ox1w3lOVQ8rgB2QuPWwpAuB1XSQ0au48,224
-mb_pandas-1.0.202305301546.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-mb_pandas-1.0.202305301546.dist-info/top_level.txt,sha256=5JkDz2-6yNAp6GiwpeR4FpxqXVysaksS5MD1iAvfMgo,10
-mb_pandas-1.0.202305301546.dist-info/RECORD,,
+mb_pandas/src/transform.py,sha256=shaD06A5eZcPMy7YIncntPVC41sQf952gi9bIyAQC-w,7226
+mb_pandas/src/version.py,sha256=vHFiYS09rKHxsUto9h9shzKvxTq2DLZft_TUDCRJCbk,396
+mb_pandas-1.0.202305301635.data/scripts/df_profile,sha256=zi4GRNQ6P5_JEB_0wMYB1KzLRG59eHXxRZG_I84lTYQ,1671
+mb_pandas-1.0.202305301635.data/scripts/df_view,sha256=BbS_rNgrPl7Raz_zVmTBqw_dvyAhc3-KqS4W2LV0_yo,3683
+mb_pandas-1.0.202305301635.dist-info/METADATA,sha256=l5k1E7HADdx7AzlfqE0TbM8xEQ3bIcjQxB1D2kelboM,224
+mb_pandas-1.0.202305301635.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+mb_pandas-1.0.202305301635.dist-info/top_level.txt,sha256=5JkDz2-6yNAp6GiwpeR4FpxqXVysaksS5MD1iAvfMgo,10
+mb_pandas-1.0.202305301635.dist-info/RECORD,,
```

