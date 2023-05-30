# Comparing `tmp/doodleverse-utils-0.0.8.tar.gz` & `tmp/doodleverse-utils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doodleverse-utils-0.0.8.tar", last modified: Thu Oct  6 23:22:34 2022, max compression
+gzip compressed data, was "doodleverse-utils-0.0.9.tar", last modified: Fri Oct  7 22:48:43 2022, max compression
```

## Comparing `doodleverse-utils-0.0.8.tar` & `doodleverse-utils-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2022-10-06 23:22:34.768096 doodleverse-utils-0.0.8/
--rw-rw-rw-   0        0        0     1089 2022-05-17 15:56:22.000000 doodleverse-utils-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      123 2022-05-17 15:56:22.000000 doodleverse-utils-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      399 2022-10-06 23:22:34.768096 doodleverse-utils-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2022-05-17 15:56:22.000000 doodleverse-utils-0.0.8/README.rst
-drwxrwxrwx   0        0        0        0 2022-10-06 23:22:34.768096 doodleverse-utils-0.0.8/doodleverse_utils/
--rw-rw-rw-   0        0        0      154 2022-05-17 15:56:22.000000 doodleverse-utils-0.0.8/doodleverse_utils/__init__.py
--rw-rw-rw-   0        0        0      519 2022-10-06 23:22:34.768096 doodleverse-utils-0.0.8/doodleverse_utils/_version.py
--rw-rw-rw-   0        0        0     7289 2022-10-03 23:28:01.000000 doodleverse-utils-0.0.8/doodleverse_utils/imports.py
--rw-rw-rw-   0        0        0    11401 2022-05-17 15:56:22.000000 doodleverse-utils-0.0.8/doodleverse_utils/make_mndwi_4pred.py
--rw-rw-rw-   0        0        0    27446 2022-07-13 18:47:31.000000 doodleverse-utils-0.0.8/doodleverse_utils/make_mndwi_dataset.py
--rw-rw-rw-   0        0        0    11384 2022-05-17 15:56:22.000000 doodleverse-utils-0.0.8/doodleverse_utils/make_ndwi_4pred.py
--rw-rw-rw-   0        0        0    27921 2022-07-13 18:47:31.000000 doodleverse-utils-0.0.8/doodleverse_utils/make_ndwi_dataset.py
--rw-rw-rw-   0        0        0    11860 2022-05-17 15:56:22.000000 doodleverse-utils-0.0.8/doodleverse_utils/merge_nd_inputs4pred.py
--rw-rw-rw-   0        0        0    34870 2022-10-06 21:23:59.000000 doodleverse-utils-0.0.8/doodleverse_utils/model_imports.py
--rw-rw-rw-   0        0        0     5506 2022-10-03 23:28:01.000000 doodleverse-utils-0.0.8/doodleverse_utils/model_metrics.py
--rw-rw-rw-   0        0        0    27364 2022-10-06 22:59:10.000000 doodleverse-utils-0.0.8/doodleverse_utils/prediction_imports.py
--rw-rw-rw-   0        0        0    10476 2022-07-13 18:47:31.000000 doodleverse-utils-0.0.8/doodleverse_utils/vggjson2mask.py
--rw-rw-rw-   0        0        0    11682 2022-05-17 15:56:22.000000 doodleverse-utils-0.0.8/doodleverse_utils/zoo_make_mndwi_4pred.py
--rw-rw-rw-   0        0        0    11665 2022-05-17 15:56:22.000000 doodleverse-utils-0.0.8/doodleverse_utils/zoo_make_ndwi_4pred.py
--rw-rw-rw-   0        0        0    11926 2022-05-17 15:56:22.000000 doodleverse-utils-0.0.8/doodleverse_utils/zoo_merge_nd_inputs4pred.py
-drwxrwxrwx   0        0        0        0 2022-10-06 23:22:34.768096 doodleverse-utils-0.0.8/doodleverse_utils.egg-info/
--rw-rw-rw-   0        0        0      399 2022-10-06 23:22:34.000000 doodleverse-utils-0.0.8/doodleverse_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      842 2022-10-06 23:22:34.000000 doodleverse-utils-0.0.8/doodleverse_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-06 23:22:34.000000 doodleverse-utils-0.0.8/doodleverse_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2022-10-06 23:22:34.000000 doodleverse-utils-0.0.8/doodleverse_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2022-10-06 23:22:34.000000 doodleverse-utils-0.0.8/doodleverse_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       10 2022-05-17 15:56:22.000000 doodleverse-utils-0.0.8/requirements.txt
--rw-rw-rw-   0        0        0      224 2022-10-06 23:22:34.768096 doodleverse-utils-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      825 2022-05-17 15:56:22.000000 doodleverse-utils-0.0.8/setup.py
--rw-rw-rw-   0        0        0    83369 2022-05-17 15:56:22.000000 doodleverse-utils-0.0.8/versioneer.py
+drwxrwxrwx   0        0        0        0 2022-10-07 22:48:43.407231 doodleverse-utils-0.0.9/
+-rw-rw-rw-   0        0        0     1089 2022-05-17 15:56:22.000000 doodleverse-utils-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      123 2022-05-17 15:56:22.000000 doodleverse-utils-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      399 2022-10-07 22:48:43.407231 doodleverse-utils-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2022-05-17 15:56:22.000000 doodleverse-utils-0.0.9/README.rst
+drwxrwxrwx   0        0        0        0 2022-10-07 22:48:43.408250 doodleverse-utils-0.0.9/doodleverse_utils/
+-rw-rw-rw-   0        0        0      154 2022-05-17 15:56:22.000000 doodleverse-utils-0.0.9/doodleverse_utils/__init__.py
+-rw-rw-rw-   0        0        0      519 2022-10-07 22:48:43.408250 doodleverse-utils-0.0.9/doodleverse_utils/_version.py
+-rw-rw-rw-   0        0        0     7289 2022-10-03 23:28:01.000000 doodleverse-utils-0.0.9/doodleverse_utils/imports.py
+-rw-rw-rw-   0        0        0    11401 2022-05-17 15:56:22.000000 doodleverse-utils-0.0.9/doodleverse_utils/make_mndwi_4pred.py
+-rw-rw-rw-   0        0        0    27446 2022-07-13 18:47:31.000000 doodleverse-utils-0.0.9/doodleverse_utils/make_mndwi_dataset.py
+-rw-rw-rw-   0        0        0    11384 2022-05-17 15:56:22.000000 doodleverse-utils-0.0.9/doodleverse_utils/make_ndwi_4pred.py
+-rw-rw-rw-   0        0        0    27921 2022-07-13 18:47:31.000000 doodleverse-utils-0.0.9/doodleverse_utils/make_ndwi_dataset.py
+-rw-rw-rw-   0        0        0    11860 2022-05-17 15:56:22.000000 doodleverse-utils-0.0.9/doodleverse_utils/merge_nd_inputs4pred.py
+-rw-rw-rw-   0        0        0    36232 2022-10-07 22:46:53.000000 doodleverse-utils-0.0.9/doodleverse_utils/model_imports.py
+-rw-rw-rw-   0        0        0     5506 2022-10-03 23:28:01.000000 doodleverse-utils-0.0.9/doodleverse_utils/model_metrics.py
+-rw-rw-rw-   0        0        0    27364 2022-10-06 22:59:10.000000 doodleverse-utils-0.0.9/doodleverse_utils/prediction_imports.py
+-rw-rw-rw-   0        0        0    10476 2022-07-13 18:47:31.000000 doodleverse-utils-0.0.9/doodleverse_utils/vggjson2mask.py
+-rw-rw-rw-   0        0        0    11682 2022-05-17 15:56:22.000000 doodleverse-utils-0.0.9/doodleverse_utils/zoo_make_mndwi_4pred.py
+-rw-rw-rw-   0        0        0    11665 2022-05-17 15:56:22.000000 doodleverse-utils-0.0.9/doodleverse_utils/zoo_make_ndwi_4pred.py
+-rw-rw-rw-   0        0        0    11926 2022-05-17 15:56:22.000000 doodleverse-utils-0.0.9/doodleverse_utils/zoo_merge_nd_inputs4pred.py
+drwxrwxrwx   0        0        0        0 2022-10-07 22:48:43.406255 doodleverse-utils-0.0.9/doodleverse_utils.egg-info/
+-rw-rw-rw-   0        0        0      399 2022-10-07 22:48:43.000000 doodleverse-utils-0.0.9/doodleverse_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      842 2022-10-07 22:48:43.000000 doodleverse-utils-0.0.9/doodleverse_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-07 22:48:43.000000 doodleverse-utils-0.0.9/doodleverse_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2022-10-07 22:48:43.000000 doodleverse-utils-0.0.9/doodleverse_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2022-10-07 22:48:43.000000 doodleverse-utils-0.0.9/doodleverse_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       10 2022-05-17 15:56:22.000000 doodleverse-utils-0.0.9/requirements.txt
+-rw-rw-rw-   0        0        0      224 2022-10-07 22:48:43.408250 doodleverse-utils-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      825 2022-05-17 15:56:22.000000 doodleverse-utils-0.0.9/setup.py
+-rw-rw-rw-   0        0        0    83369 2022-05-17 15:56:22.000000 doodleverse-utils-0.0.9/versioneer.py
```

### Comparing `doodleverse-utils-0.0.8/LICENSE` & `doodleverse-utils-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `doodleverse-utils-0.0.8/doodleverse_utils/imports.py` & `doodleverse-utils-0.0.9/doodleverse_utils/imports.py`

 * *Files identical despite different names*

### Comparing `doodleverse-utils-0.0.8/doodleverse_utils/make_mndwi_4pred.py` & `doodleverse-utils-0.0.9/doodleverse_utils/make_mndwi_4pred.py`

 * *Files identical despite different names*

### Comparing `doodleverse-utils-0.0.8/doodleverse_utils/make_mndwi_dataset.py` & `doodleverse-utils-0.0.9/doodleverse_utils/make_mndwi_dataset.py`

 * *Files identical despite different names*

### Comparing `doodleverse-utils-0.0.8/doodleverse_utils/make_ndwi_4pred.py` & `doodleverse-utils-0.0.9/doodleverse_utils/make_ndwi_4pred.py`

 * *Files identical despite different names*

### Comparing `doodleverse-utils-0.0.8/doodleverse_utils/make_ndwi_dataset.py` & `doodleverse-utils-0.0.9/doodleverse_utils/make_ndwi_dataset.py`

 * *Files identical despite different names*

### Comparing `doodleverse-utils-0.0.8/doodleverse_utils/merge_nd_inputs4pred.py` & `doodleverse-utils-0.0.9/doodleverse_utils/merge_nd_inputs4pred.py`

 * *Files identical despite different names*

### Comparing `doodleverse-utils-0.0.8/doodleverse_utils/model_imports.py` & `doodleverse-utils-0.0.9/doodleverse_utils/model_imports.py`

 * *Files 2% similar despite different names*

```diff
@@ -987,15 +987,14 @@
         y_pred = tf.one_hot(tf.argmax(y_pred, -1), nclasses)
         for index in range(nclasses):
             iousum += basic_iou(y_true[:,:,:,index], y_pred[:,:,:,index])
         return iousum/nclasses
 
     return mean_iou
 
-
 # -----------------------------------
 #define basic Dice formula
 def basic_dice_coef(y_true, y_pred):
     """
     dice_coef(y_true, y_pred)
 
     This function computes the mean Dice coefficient between `y_true` and `y_pred`: this version is tensorflow (not numpy) and is used by tensorflow training and evaluation functions
@@ -1034,15 +1033,14 @@
         #y_pred = tf.one_hot(tf.argmax(y_pred, -1), 4)
         for index in range(nclasses):
             dice += basic_dice_coef(y_true[:,:,:,index], y_pred[:,:,:,index])
         return dice/nclasses
 
     return dice_coef
 
-
 # ---------------------------------------------------
 #define Dice loss for multiple classes
 def dice_coef_loss(nclasses):
     """
     dice_coef_loss(y_true, y_pred)
 
     This function computes the mean Dice loss (1 - Dice coefficient) between `y_true` and `y_pred`: this version is tensorflow (not numpy) and is used by tensorflow training and evaluation functions
@@ -1071,15 +1069,50 @@
         #y_pred = tf.one_hot(tf.argmax(y_pred, -1), 4)
         for index in range(nclasses):
             dice += basic_dice_coef(y_true[:,:,:,index], y_pred[:,:,:,index])
         return 1 - (dice/nclasses)
 
     return MC_dice_coef_loss
 
+#define weighted Dice loss for multiple classes
+def weighted_dice_coef_loss(nclasses, weights):
+    """
+    weighted_MC_dice_coef_loss(y_true, y_pred)
+
+    This function computes the mean Dice loss (1 - Dice coefficient) between `y_true` and `y_pred`: this version is tensorflow (not numpy) and is used by tensorflow training and evaluation functions
+
+    INPUTS:
+        * y_true: true masks, one-hot encoded.
+            * Inputs are B*W*H*N tensors, with
+                B = batch size,
+                W = width,
+                H = height,
+                N = number of classes
+        * y_pred: predicted masks, either softmax outputs, or one-hot encoded.
+            * Inputs are B*W*H*N tensors, with
+                B = batch size,
+                W = width,
+                H = height,
+                N = number of classes
+    OPTIONAL INPUTS: None
+    GLOBAL INPUTS: None
+    OUTPUTS:
+        * Dice loss [tensor]
+    """
+
+    def weighted_MC_dice_coef_loss(y_true, y_pred):
+        dice = 0
+        #can't have an argmax in a loss
+        #y_pred = tf.one_hot(tf.argmax(y_pred, -1), 4)
+        for index in range(nclasses):
+            dice += basic_dice_coef(y_true[:,:,:,index], y_pred[:,:,:,index])*weights[index]
+        meandice = (dice/nclasses)
+        return 1 - meandice
 
+    return weighted_MC_dice_coef_loss
 
 def mean_iou_np(y_true, y_pred, nclasses):
     iousum = 0
     y_pred = tf.one_hot(tf.argmax(y_pred, -1), nclasses)
     for index in range(nclasses):
         iousum += basic_iou(y_true[:,:,:,index], y_pred[:,:,:,index])
     return (iousum/nclasses).numpy()
```

### Comparing `doodleverse-utils-0.0.8/doodleverse_utils/model_metrics.py` & `doodleverse-utils-0.0.9/doodleverse_utils/model_metrics.py`

 * *Files identical despite different names*

### Comparing `doodleverse-utils-0.0.8/doodleverse_utils/prediction_imports.py` & `doodleverse-utils-0.0.9/doodleverse_utils/prediction_imports.py`

 * *Files identical despite different names*

### Comparing `doodleverse-utils-0.0.8/doodleverse_utils/vggjson2mask.py` & `doodleverse-utils-0.0.9/doodleverse_utils/vggjson2mask.py`

 * *Files identical despite different names*

### Comparing `doodleverse-utils-0.0.8/doodleverse_utils/zoo_make_mndwi_4pred.py` & `doodleverse-utils-0.0.9/doodleverse_utils/zoo_make_mndwi_4pred.py`

 * *Files identical despite different names*

### Comparing `doodleverse-utils-0.0.8/doodleverse_utils/zoo_make_ndwi_4pred.py` & `doodleverse-utils-0.0.9/doodleverse_utils/zoo_make_ndwi_4pred.py`

 * *Files identical despite different names*

### Comparing `doodleverse-utils-0.0.8/doodleverse_utils/zoo_merge_nd_inputs4pred.py` & `doodleverse-utils-0.0.9/doodleverse_utils/zoo_merge_nd_inputs4pred.py`

 * *Files identical despite different names*

### Comparing `doodleverse-utils-0.0.8/doodleverse_utils.egg-info/SOURCES.txt` & `doodleverse-utils-0.0.9/doodleverse_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `doodleverse-utils-0.0.8/setup.py` & `doodleverse-utils-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `doodleverse-utils-0.0.8/versioneer.py` & `doodleverse-utils-0.0.9/versioneer.py`

 * *Files identical despite different names*

