# Comparing `tmp/impy_array-2.2.3.tar.gz` & `tmp/impy_array-2.2.4.tar.gz`

## Comparing `impy_array-2.2.3.tar` & `impy_array-2.2.4.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/__init__.py
--rw-r--r--   0        0        0     4974 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/__main__.py
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/_const.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/_types.py
--rw-r--r--   0        0        0     4839 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/array_api.py
--rw-r--r--   0        0        0     9651 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/binder.py
--rw-r--r--   0        0        0    10946 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/collections.py
--rw-r--r--   0        0        0    29654 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/core.py
--rw-r--r--   0        0        0    28398 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/correlation.py
--rw-r--r--   0        0        0    19241 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/io.py
--rw-r--r--   0        0        0     7035 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/random.py
--rw-r--r--   0        0        0    14164 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/roi.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/arrays/__init__.py
--rw-r--r--   0        0        0    13143 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/arrays/_deprecated.py
--rw-r--r--   0        0        0     6517 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/arrays/_imshow.py
--rw-r--r--   0        0        0    10570 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/arrays/axesmixin.py
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/arrays/big.py
--rw-r--r--   0        0        0   155930 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/arrays/imgarray.py
--rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/arrays/label.py
--rw-r--r--   0        0        0    56945 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/arrays/labeledarray.py
--rw-r--r--   0        0        0    55446 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/arrays/lazy.py
--rw-r--r--   0        0        0    13937 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/arrays/phasearray.py
--rw-r--r--   0        0        0     7886 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/arrays/specials.py
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/arrays/tiled.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/arrays/_utils/__init__.py
--rw-r--r--   0        0        0    10031 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/arrays/_utils/_corr.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/arrays/_utils/_deconv.py
--rw-r--r--   0        0        0     4968 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/arrays/_utils/_docs.py
--rw-r--r--   0        0        0     7212 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/arrays/_utils/_filters.py
--rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/arrays/_utils/_glcm.py
--rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/arrays/_utils/_linalg.py
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/arrays/_utils/_misc.py
--rw-r--r--   0        0        0     5042 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/arrays/_utils/_plot.py
--rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/arrays/_utils/_process_numba.py
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/arrays/_utils/_skimage.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/arrays/_utils/_structures.py
--rw-r--r--   0        0        0    12762 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/arrays/_utils/_transform.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/arrays/bases/__init__.py
--rw-r--r--   0        0        0    27104 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/arrays/bases/metaarray.py
--rw-r--r--   0        0        0     9359 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/arrays/bases/overload.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/axes/__init__.py
--rw-r--r--   0        0        0    12134 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/axes/_axes.py
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/axes/_axes_tuple.py
--rw-r--r--   0        0        0     7630 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/axes/_axis.py
--rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/axes/_slicer.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/frame/__init__.py
--rw-r--r--   0        0        0    12354 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/frame/frames.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/utils/__init__.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/utils/axesop.py
--rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/utils/deco.py
--rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/utils/gauss.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/utils/misc.py
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/utils/slicer.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/utils/utilcls.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/viewer/__init__.py
--rw-r--r--   0        0        0    12187 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/viewer/utils.py
--rw-r--r--   0        0        0    17561 2020-02-02 00:00:00.000000 impy_array-2.2.3/impy/viewer/viewer.py
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 impy_array-2.2.3/.gitignore
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 impy_array-2.2.3/LICENSE
--rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 impy_array-2.2.3/README.md
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 impy_array-2.2.3/pyproject.toml
--rw-r--r--   0        0        0     6322 2020-02-02 00:00:00.000000 impy_array-2.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/__init__.py
+-rw-r--r--   0        0        0     4974 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/__main__.py
+-rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/_const.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/_types.py
+-rw-r--r--   0        0        0     4839 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/array_api.py
+-rw-r--r--   0        0        0     9651 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/binder.py
+-rw-r--r--   0        0        0    10946 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/collections.py
+-rw-r--r--   0        0        0    29654 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/core.py
+-rw-r--r--   0        0        0    28398 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/correlation.py
+-rw-r--r--   0        0        0    19241 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/io.py
+-rw-r--r--   0        0        0     7035 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/random.py
+-rw-r--r--   0        0        0    14164 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/roi.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/__init__.py
+-rw-r--r--   0        0        0    13143 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/_deprecated.py
+-rw-r--r--   0        0        0     6517 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/_imshow.py
+-rw-r--r--   0        0        0    10570 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/axesmixin.py
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/big.py
+-rw-r--r--   0        0        0   155930 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/imgarray.py
+-rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/label.py
+-rw-r--r--   0        0        0    56945 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/labeledarray.py
+-rw-r--r--   0        0        0    55446 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/lazy.py
+-rw-r--r--   0        0        0    13937 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/phasearray.py
+-rw-r--r--   0        0        0     7886 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/specials.py
+-rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/tiled.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/_utils/__init__.py
+-rw-r--r--   0        0        0    10031 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/_utils/_corr.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/_utils/_deconv.py
+-rw-r--r--   0        0        0     4968 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/_utils/_docs.py
+-rw-r--r--   0        0        0     7212 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/_utils/_filters.py
+-rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/_utils/_glcm.py
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/_utils/_linalg.py
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/_utils/_misc.py
+-rw-r--r--   0        0        0     5042 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/_utils/_plot.py
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/_utils/_process_numba.py
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/_utils/_skimage.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/_utils/_structures.py
+-rw-r--r--   0        0        0    12762 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/_utils/_transform.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/bases/__init__.py
+-rw-r--r--   0        0        0    27104 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/bases/metaarray.py
+-rw-r--r--   0        0        0     9359 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/bases/overload.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/axes/__init__.py
+-rw-r--r--   0        0        0    12134 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/axes/_axes.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/axes/_axes_tuple.py
+-rw-r--r--   0        0        0     7630 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/axes/_axis.py
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/axes/_slicer.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/frame/__init__.py
+-rw-r--r--   0        0        0    12354 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/frame/frames.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/utils/__init__.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/utils/axesop.py
+-rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/utils/deco.py
+-rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/utils/gauss.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/utils/misc.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/utils/slicer.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/utils/utilcls.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/viewer/__init__.py
+-rw-r--r--   0        0        0    12187 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/viewer/utils.py
+-rw-r--r--   0        0        0    17561 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/viewer/viewer.py
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 impy_array-2.2.4/.gitignore
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 impy_array-2.2.4/LICENSE
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 impy_array-2.2.4/README.md
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 impy_array-2.2.4/pyproject.toml
+-rw-r--r--   0        0        0     6322 2020-02-02 00:00:00.000000 impy_array-2.2.4/PKG-INFO
```

### Comparing `impy_array-2.2.3/impy/__init__.py` & `impy_array-2.2.4/impy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.2.3"
+__version__ = "2.2.4"
 __author__ = "Hanjin Liu"
 __email__ = "liuhanjin-sc@g.ecc.u-tokyo.ac.jp"
 
 import logging
 
 from ._const import Const, SetConst, use
```

### Comparing `impy_array-2.2.3/impy/__main__.py` & `impy_array-2.2.4/impy/__main__.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/_const.py` & `impy_array-2.2.4/impy/_const.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/_types.py` & `impy_array-2.2.4/impy/_types.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/array_api.py` & `impy_array-2.2.4/impy/array_api.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/binder.py` & `impy_array-2.2.4/impy/binder.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/collections.py` & `impy_array-2.2.4/impy/collections.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/core.py` & `impy_array-2.2.4/impy/core.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/correlation.py` & `impy_array-2.2.4/impy/correlation.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/io.py` & `impy_array-2.2.4/impy/io.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/random.py` & `impy_array-2.2.4/impy/random.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/roi.py` & `impy_array-2.2.4/impy/roi.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/arrays/__init__.py` & `impy_array-2.2.4/impy/arrays/__init__.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/arrays/_deprecated.py` & `impy_array-2.2.4/impy/arrays/_deprecated.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/arrays/_imshow.py` & `impy_array-2.2.4/impy/arrays/_imshow.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/arrays/axesmixin.py` & `impy_array-2.2.4/impy/arrays/axesmixin.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/arrays/big.py` & `impy_array-2.2.4/impy/arrays/big.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/arrays/imgarray.py` & `impy_array-2.2.4/impy/arrays/imgarray.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/arrays/label.py` & `impy_array-2.2.4/impy/arrays/label.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/arrays/labeledarray.py` & `impy_array-2.2.4/impy/arrays/labeledarray.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/arrays/lazy.py` & `impy_array-2.2.4/impy/arrays/lazy.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/arrays/phasearray.py` & `impy_array-2.2.4/impy/arrays/phasearray.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/arrays/specials.py` & `impy_array-2.2.4/impy/arrays/specials.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/arrays/tiled.py` & `impy_array-2.2.4/impy/arrays/tiled.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,17 +107,16 @@
         
         def func(arr: np.ndarray):
             psf_ft, psf_ft_conj = _deconv.check_psf(arr.shape, scale, psf)
             return _deconv.richardson_lucy(arr, psf_ft, psf_ft_conj, niter, eps)
             
         return self._map_overlap(func)
     
-    def gaussian_filter(self, sigma: float = 1.0, fourier: bool = False) -> ImgArray:
-        filter_func = _filters.gaussian_filter_fourier if fourier else _filters.gaussian_filter
-        return self._map_overlap(filter_func, sigma=sigma)
+    def gaussian_filter(self, sigma: float, fourier: bool = False) -> ImgArray:
+        return self._map_overlap(_filters.gaussian_filter, sigma=sigma, fourier=fourier)
     
     def dog_filter(
         self,
         low_sigma: float = 1.0,
         high_sigma: float | None = None,
         fourier: bool = False,
     ) -> ImgArray:
```

### Comparing `impy_array-2.2.3/impy/arrays/_utils/_corr.py` & `impy_array-2.2.4/impy/arrays/_utils/_corr.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/arrays/_utils/_deconv.py` & `impy_array-2.2.4/impy/arrays/_utils/_deconv.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/arrays/_utils/_docs.py` & `impy_array-2.2.4/impy/arrays/_utils/_docs.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/arrays/_utils/_filters.py` & `impy_array-2.2.4/impy/arrays/_utils/_filters.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/arrays/_utils/_glcm.py` & `impy_array-2.2.4/impy/arrays/_utils/_glcm.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/arrays/_utils/_linalg.py` & `impy_array-2.2.4/impy/arrays/_utils/_linalg.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/arrays/_utils/_misc.py` & `impy_array-2.2.4/impy/arrays/_utils/_misc.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/arrays/_utils/_plot.py` & `impy_array-2.2.4/impy/arrays/_utils/_plot.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/arrays/_utils/_process_numba.py` & `impy_array-2.2.4/impy/arrays/_utils/_process_numba.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/arrays/_utils/_skimage.py` & `impy_array-2.2.4/impy/arrays/_utils/_skimage.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/arrays/_utils/_structures.py` & `impy_array-2.2.4/impy/arrays/_utils/_structures.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/arrays/_utils/_transform.py` & `impy_array-2.2.4/impy/arrays/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/arrays/bases/metaarray.py` & `impy_array-2.2.4/impy/arrays/bases/metaarray.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/arrays/bases/overload.py` & `impy_array-2.2.4/impy/arrays/bases/overload.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/axes/_axes.py` & `impy_array-2.2.4/impy/axes/_axes.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/axes/_axes_tuple.py` & `impy_array-2.2.4/impy/axes/_axes_tuple.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/axes/_axis.py` & `impy_array-2.2.4/impy/axes/_axis.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/axes/_slicer.py` & `impy_array-2.2.4/impy/axes/_slicer.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/frame/frames.py` & `impy_array-2.2.4/impy/frame/frames.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/utils/axesop.py` & `impy_array-2.2.4/impy/utils/axesop.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/utils/deco.py` & `impy_array-2.2.4/impy/utils/deco.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/utils/gauss.py` & `impy_array-2.2.4/impy/utils/gauss.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/utils/misc.py` & `impy_array-2.2.4/impy/utils/misc.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/utils/slicer.py` & `impy_array-2.2.4/impy/utils/slicer.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/viewer/utils.py` & `impy_array-2.2.4/impy/viewer/utils.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/impy/viewer/viewer.py` & `impy_array-2.2.4/impy/viewer/viewer.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/.gitignore` & `impy_array-2.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/LICENSE` & `impy_array-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/README.md` & `impy_array-2.2.4/README.md`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/pyproject.toml` & `impy_array-2.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.3/PKG-INFO` & `impy_array-2.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: impy-array
-Version: 2.2.3
+Version: 2.2.4
 Summary: Speed up coding/extending image analysis in Python.
 Project-URL: Download, https://github.com/hanjinliu/impy
 Author-email: Hanjin Liu <liuhanjin-sc@g.ecc.u-tokyo.ac.jp>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, hanjinliu
         All rights reserved.
```

