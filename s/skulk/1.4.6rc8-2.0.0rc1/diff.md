# Comparing `tmp/skulk-1.4.6rc8-py2.py3-none-any.whl.zip` & `tmp/skulk-2.0.0rc1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8922 bytes, number of entries: 10
--rw-r--r--  2.0 unx       10 b- defN 23-May-30 05:44 skulk/VERSION
--rw-r--r--  2.0 unx        0 b- defN 23-May-30 05:44 skulk/__init__.py
--rw-r--r--  2.0 unx     9348 b- defN 23-May-30 05:44 skulk/bumper.py
--rw-r--r--  2.0 unx     9105 b- defN 23-May-30 05:44 skulk/skulk.py
--rw-r--r--  2.0 unx     2625 b- defN 23-May-30 05:44 skulk/util.py
--rw-r--r--  2.0 unx      649 b- defN 23-May-30 05:44 skulk-1.4.6rc8.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-30 05:44 skulk-1.4.6rc8.dist-info/WHEEL
--rw-r--r--  2.0 unx       44 b- defN 23-May-30 05:44 skulk-1.4.6rc8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 23-May-30 05:44 skulk-1.4.6rc8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      749 b- defN 23-May-30 05:44 skulk-1.4.6rc8.dist-info/RECORD
-10 files, 22646 bytes uncompressed, 7650 bytes compressed:  66.2%
+Zip file size: 8921 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       10 b- defN 23-May-30 06:09 skulk/VERSION
+-rw-r--r--  2.0 unx        0 b- defN 23-May-30 06:09 skulk/__init__.py
+-rw-r--r--  2.0 unx     9348 b- defN 23-May-30 06:09 skulk/bumper.py
+-rw-r--r--  2.0 unx     9105 b- defN 23-May-30 06:09 skulk/skulk.py
+-rw-r--r--  2.0 unx     2625 b- defN 23-May-30 06:09 skulk/util.py
+-rw-r--r--  2.0 unx      649 b- defN 23-May-30 06:09 skulk-2.0.0rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-30 06:09 skulk-2.0.0rc1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       44 b- defN 23-May-30 06:09 skulk-2.0.0rc1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 23-May-30 06:09 skulk-2.0.0rc1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      749 b- defN 23-May-30 06:09 skulk-2.0.0rc1.dist-info/RECORD
+10 files, 22646 bytes uncompressed, 7649 bytes compressed:  66.2%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: skulk/skulk.py
 Comment: 
 
 Filename: skulk/util.py
 Comment: 
 
-Filename: skulk-1.4.6rc8.dist-info/METADATA
+Filename: skulk-2.0.0rc1.dist-info/METADATA
 Comment: 
 
-Filename: skulk-1.4.6rc8.dist-info/WHEEL
+Filename: skulk-2.0.0rc1.dist-info/WHEEL
 Comment: 
 
-Filename: skulk-1.4.6rc8.dist-info/entry_points.txt
+Filename: skulk-2.0.0rc1.dist-info/entry_points.txt
 Comment: 
 
-Filename: skulk-1.4.6rc8.dist-info/top_level.txt
+Filename: skulk-2.0.0rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: skulk-1.4.6rc8.dist-info/RECORD
+Filename: skulk-2.0.0rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## skulk/VERSION

```diff
@@ -1 +1 @@
-1.4.6-rc.8
+2.0.0-rc.1
```

## Comparing `skulk-1.4.6rc8.dist-info/METADATA` & `skulk-2.0.0rc1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skulk
-Version: 1.4.6rc8
+Version: 2.0.0rc1
 Summary: Streamline release for Conductor client tools and others
 Home-page: https://github.com/ConductorTechnologies/skulk
 Author: Julian Mann
 Author-email: julian@conductortech.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

## Comparing `skulk-1.4.6rc8.dist-info/RECORD` & `skulk-2.0.0rc1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-skulk/VERSION,sha256=FL1JCEHgyA-o7Hd068lhxq_TSd58SLzKDYSN8HtDS9A,10
+skulk/VERSION,sha256=9hNpYAYjM6P8IFcmPTbqsyNgrep7Oy37HWq0RCmR91U,10
 skulk/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 skulk/bumper.py,sha256=UMqPRQD3Pt1HrG0lcBb7-f2oqHCx_jZEpgVto5yDbcU,9348
 skulk/skulk.py,sha256=sGpBUM8pXlOY7sUNJaKk-WtCC43npxC_YcmQFP4A4Kk,9105
 skulk/util.py,sha256=64hqDrkuXZTPVmCydXUdsp_79Gl_UU8QcqxeDzH6PQk,2625
-skulk-1.4.6rc8.dist-info/METADATA,sha256=Vfpg6aOEKJc8LrDm6_XkP3oBGFhQ5qzM2hIMu8Hhnj0,649
-skulk-1.4.6rc8.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-skulk-1.4.6rc8.dist-info/entry_points.txt,sha256=Gis7pLiCEkPWw7tn3_U-G9XPwOtBvTL4m11EqDi613o,44
-skulk-1.4.6rc8.dist-info/top_level.txt,sha256=EOnQuA1Vdf2WjOz9xLTPLCynTq2IdzLPGQ54LdhP7oY,6
-skulk-1.4.6rc8.dist-info/RECORD,,
+skulk-2.0.0rc1.dist-info/METADATA,sha256=A9mn7KXnlsWYQbQF9zUDlw2wxlL7V0hw2kStK8aCqyY,649
+skulk-2.0.0rc1.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+skulk-2.0.0rc1.dist-info/entry_points.txt,sha256=Gis7pLiCEkPWw7tn3_U-G9XPwOtBvTL4m11EqDi613o,44
+skulk-2.0.0rc1.dist-info/top_level.txt,sha256=EOnQuA1Vdf2WjOz9xLTPLCynTq2IdzLPGQ54LdhP7oY,6
+skulk-2.0.0rc1.dist-info/RECORD,,
```

