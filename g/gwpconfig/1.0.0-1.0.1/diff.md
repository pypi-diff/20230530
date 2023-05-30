# Comparing `tmp/gwpconfig-1.0.0-py3-none-any.whl.zip` & `tmp/gwpconfig-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4290 bytes, number of entries: 8
+Zip file size: 4293 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-23 12:13 gwpconfig/__init__.py
 -rw-rw-rw-  2.0 fat     3698 b- defN 23-May-24 13:27 gwpconfig/commconstants.py
--rw-rw-rw-  2.0 fat     1221 b- defN 23-May-12 10:58 gwpconfig/wall.py
--rw-rw-rw-  2.0 fat     1086 b- defN 23-May-30 08:29 gwpconfig-1.0.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      221 b- defN 23-May-30 08:29 gwpconfig-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 08:29 gwpconfig-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-May-30 08:29 gwpconfig-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      627 b- defN 23-May-30 08:29 gwpconfig-1.0.0.dist-info/RECORD
-8 files, 6955 bytes uncompressed, 3194 bytes compressed:  54.1%
+-rw-rw-rw-  2.0 fat     1220 b- defN 23-May-30 12:23 gwpconfig/wall.py
+-rw-rw-rw-  2.0 fat     1086 b- defN 23-May-30 12:28 gwpconfig-1.0.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      221 b- defN 23-May-30 12:28 gwpconfig-1.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 12:28 gwpconfig-1.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-May-30 12:28 gwpconfig-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      627 b- defN 23-May-30 12:28 gwpconfig-1.0.1.dist-info/RECORD
+8 files, 6954 bytes uncompressed, 3197 bytes compressed:  54.0%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: gwpconfig/commconstants.py
 Comment: 
 
 Filename: gwpconfig/wall.py
 Comment: 
 
-Filename: gwpconfig-1.0.0.dist-info/LICENSE
+Filename: gwpconfig-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: gwpconfig-1.0.0.dist-info/METADATA
+Filename: gwpconfig-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: gwpconfig-1.0.0.dist-info/WHEEL
+Filename: gwpconfig-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: gwpconfig-1.0.0.dist-info/top_level.txt
+Filename: gwpconfig-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: gwpconfig-1.0.0.dist-info/RECORD
+Filename: gwpconfig-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gwpconfig/wall.py

```diff
@@ -1,18 +1,19 @@
 """Module with wall measurements and method for creating grid of pins.
 """
 import math
 import numpy as np
 
 # Wall size given in meters - (x, y).
-WALL_SIZE = [1.25, 1.3]
+WALL_SIZE = [4.1, 3.1]
 # Pin raster - distances between pins in (x, y).
 WALL_RASTER = [0.2, 0.25]
 PIN_HEIGHT = 0.0
 
+
 def create_grid(three_dim):
     """Calculate pins positions. Pins are placed in squared pattern.
 
     Args:
         threeDim (bool): If True, calculate pins positions in 3d space, otherwise in 2d space (without height dimension).
 
     Returns:
@@ -29,8 +30,7 @@
         for y in y_grid:
             if not three_dim:
                 pins.append([x, y])
             else:
                 pins.append([x, y, PIN_HEIGHT])
 
     return np.array(pins)
-
```

## Comparing `gwpconfig-1.0.0.dist-info/LICENSE` & `gwpconfig-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gwpconfig-1.0.0.dist-info/RECORD` & `gwpconfig-1.0.1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 gwpconfig/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 gwpconfig/commconstants.py,sha256=PT6nJBwCbFXXiJAOHnSCgfXOAV-fLiuigAknd2ZFF_g,3698
-gwpconfig/wall.py,sha256=e6pgG61b3itmf5U0m24piquyRMzlASnCl-Y83-_42Ws,1221
-gwpconfig-1.0.0.dist-info/LICENSE,sha256=n6yLoS-d2VDNk_Qp5QhbosDrLk2PLd-eonfrWKWSBkE,1086
-gwpconfig-1.0.0.dist-info/METADATA,sha256=iGLptZrV025Hq6Z5zneaE1YVFiBPMj0X0ahHmMzHDsw,221
-gwpconfig-1.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-gwpconfig-1.0.0.dist-info/top_level.txt,sha256=hfusZ8S8b2fEoz0K1N8aDfo0ytpJ2XX5ZnQvIqafjrM,10
-gwpconfig-1.0.0.dist-info/RECORD,,
+gwpconfig/wall.py,sha256=snVkVtG3pNetjt5VTf8oM2Px28S9FjGc4GsA1Zttrhw,1220
+gwpconfig-1.0.1.dist-info/LICENSE,sha256=n6yLoS-d2VDNk_Qp5QhbosDrLk2PLd-eonfrWKWSBkE,1086
+gwpconfig-1.0.1.dist-info/METADATA,sha256=PfyOHWHK-2KDeeO41QMk9e2JYdlCE90r2oP3Zv1LKcg,221
+gwpconfig-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+gwpconfig-1.0.1.dist-info/top_level.txt,sha256=hfusZ8S8b2fEoz0K1N8aDfo0ytpJ2XX5ZnQvIqafjrM,10
+gwpconfig-1.0.1.dist-info/RECORD,,
```

