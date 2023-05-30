# Comparing `tmp/impy_array-2.2.4.tar.gz` & `tmp/impy_array-2.2.5.tar.gz`

## Comparing `impy_array-2.2.4.tar` & `impy_array-2.2.5.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/__init__.py
--rw-r--r--   0        0        0     4974 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/__main__.py
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/_const.py
--rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/_types.py
--rw-r--r--   0        0        0     4839 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/array_api.py
--rw-r--r--   0        0        0     9651 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/binder.py
--rw-r--r--   0        0        0    10946 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/collections.py
--rw-r--r--   0        0        0    29654 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/core.py
--rw-r--r--   0        0        0    28398 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/correlation.py
--rw-r--r--   0        0        0    19241 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/io.py
--rw-r--r--   0        0        0     7035 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/random.py
--rw-r--r--   0        0        0    14164 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/roi.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/__init__.py
--rw-r--r--   0        0        0    13143 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/_deprecated.py
--rw-r--r--   0        0        0     6517 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/_imshow.py
--rw-r--r--   0        0        0    10570 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/axesmixin.py
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/big.py
--rw-r--r--   0        0        0   155930 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/imgarray.py
--rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/label.py
--rw-r--r--   0        0        0    56945 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/labeledarray.py
--rw-r--r--   0        0        0    55446 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/lazy.py
--rw-r--r--   0        0        0    13937 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/phasearray.py
--rw-r--r--   0        0        0     7886 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/specials.py
--rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/tiled.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/_utils/__init__.py
--rw-r--r--   0        0        0    10031 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/_utils/_corr.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/_utils/_deconv.py
--rw-r--r--   0        0        0     4968 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/_utils/_docs.py
--rw-r--r--   0        0        0     7212 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/_utils/_filters.py
--rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/_utils/_glcm.py
--rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/_utils/_linalg.py
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/_utils/_misc.py
--rw-r--r--   0        0        0     5042 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/_utils/_plot.py
--rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/_utils/_process_numba.py
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/_utils/_skimage.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/_utils/_structures.py
--rw-r--r--   0        0        0    12762 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/_utils/_transform.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/bases/__init__.py
--rw-r--r--   0        0        0    27104 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/bases/metaarray.py
--rw-r--r--   0        0        0     9359 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/arrays/bases/overload.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/axes/__init__.py
--rw-r--r--   0        0        0    12134 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/axes/_axes.py
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/axes/_axes_tuple.py
--rw-r--r--   0        0        0     7630 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/axes/_axis.py
--rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/axes/_slicer.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/frame/__init__.py
--rw-r--r--   0        0        0    12354 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/frame/frames.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/utils/__init__.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/utils/axesop.py
--rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/utils/deco.py
--rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/utils/gauss.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/utils/misc.py
--rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/utils/slicer.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/utils/utilcls.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/viewer/__init__.py
--rw-r--r--   0        0        0    12187 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/viewer/utils.py
--rw-r--r--   0        0        0    17561 2020-02-02 00:00:00.000000 impy_array-2.2.4/impy/viewer/viewer.py
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 impy_array-2.2.4/.gitignore
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 impy_array-2.2.4/LICENSE
--rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 impy_array-2.2.4/README.md
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 impy_array-2.2.4/pyproject.toml
--rw-r--r--   0        0        0     6322 2020-02-02 00:00:00.000000 impy_array-2.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/__init__.py
+-rw-r--r--   0        0        0     4974 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/__main__.py
+-rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/_const.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/_types.py
+-rw-r--r--   0        0        0     4839 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/array_api.py
+-rw-r--r--   0        0        0     9651 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/binder.py
+-rw-r--r--   0        0        0    10946 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/collections.py
+-rw-r--r--   0        0        0    29654 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/core.py
+-rw-r--r--   0        0        0    28398 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/correlation.py
+-rw-r--r--   0        0        0    19241 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/io.py
+-rw-r--r--   0        0        0     7058 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/random.py
+-rw-r--r--   0        0        0    14164 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/roi.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/__init__.py
+-rw-r--r--   0        0        0    13143 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/_deprecated.py
+-rw-r--r--   0        0        0     6517 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/_imshow.py
+-rw-r--r--   0        0        0    10570 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/axesmixin.py
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/big.py
+-rw-r--r--   0        0        0   155930 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/imgarray.py
+-rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/label.py
+-rw-r--r--   0        0        0    56945 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/labeledarray.py
+-rw-r--r--   0        0        0    55446 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/lazy.py
+-rw-r--r--   0        0        0    13937 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/phasearray.py
+-rw-r--r--   0        0        0     7886 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/specials.py
+-rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/tiled.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/_utils/__init__.py
+-rw-r--r--   0        0        0    10031 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/_utils/_corr.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/_utils/_deconv.py
+-rw-r--r--   0        0        0     4968 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/_utils/_docs.py
+-rw-r--r--   0        0        0     7230 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/_utils/_filters.py
+-rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/_utils/_glcm.py
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/_utils/_linalg.py
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/_utils/_misc.py
+-rw-r--r--   0        0        0     5042 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/_utils/_plot.py
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/_utils/_process_numba.py
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/_utils/_skimage.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/_utils/_structures.py
+-rw-r--r--   0        0        0    12762 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/_utils/_transform.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/bases/__init__.py
+-rw-r--r--   0        0        0    27104 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/bases/metaarray.py
+-rw-r--r--   0        0        0     9359 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/arrays/bases/overload.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/axes/__init__.py
+-rw-r--r--   0        0        0    12134 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/axes/_axes.py
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/axes/_axes_tuple.py
+-rw-r--r--   0        0        0     7630 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/axes/_axis.py
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/axes/_slicer.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/frame/__init__.py
+-rw-r--r--   0        0        0    12354 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/frame/frames.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/utils/__init__.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/utils/axesop.py
+-rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/utils/deco.py
+-rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/utils/gauss.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/utils/misc.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/utils/slicer.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/utils/utilcls.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/viewer/__init__.py
+-rw-r--r--   0        0        0    12187 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/viewer/utils.py
+-rw-r--r--   0        0        0    17561 2020-02-02 00:00:00.000000 impy_array-2.2.5/impy/viewer/viewer.py
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 impy_array-2.2.5/.gitignore
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 impy_array-2.2.5/LICENSE
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 impy_array-2.2.5/README.md
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 impy_array-2.2.5/pyproject.toml
+-rw-r--r--   0        0        0     6322 2020-02-02 00:00:00.000000 impy_array-2.2.5/PKG-INFO
```

### Comparing `impy_array-2.2.4/impy/__init__.py` & `impy_array-2.2.5/impy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.2.4"
+__version__ = "2.2.5"
 __author__ = "Hanjin Liu"
 __email__ = "liuhanjin-sc@g.ecc.u-tokyo.ac.jp"
 
 import logging
 
 from ._const import Const, SetConst, use
```

### Comparing `impy_array-2.2.4/impy/__main__.py` & `impy_array-2.2.5/impy/__main__.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/_const.py` & `impy_array-2.2.5/impy/_const.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/_types.py` & `impy_array-2.2.5/impy/_types.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/array_api.py` & `impy_array-2.2.5/impy/array_api.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/binder.py` & `impy_array-2.2.5/impy/binder.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/collections.py` & `impy_array-2.2.5/impy/collections.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/core.py` & `impy_array-2.2.5/impy/core.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/correlation.py` & `impy_array-2.2.5/impy/correlation.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/io.py` & `impy_array-2.2.5/impy/io.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/random.py` & `impy_array-2.2.5/impy/random.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 import numpy as np
-from typing import Callable, Literal, TypeVar
-import functools
+from typing import Literal
 from .arrays import ImgArray, LazyImgArray
 from .arrays.bases import MetaArray
 from .array_api import xp
 from .core import asarray
 from .axes import AxesLike
 
 def wraps(npfunc):
@@ -135,15 +134,15 @@
         name: str | None = None,
         like: MetaArray | LazyImgArray =None,
     ) -> ImgArray:
         size, name, axes = _normalize_like(size, name, axes, like)
         arr = self._rng.standard_normal(size=size, dtype=dtype)
         if np.isscalar(arr):
             return arr
-        return asarray(arr, axes=axes, name=name)
+        return asarray(xp.asnumpy(arr), axes=axes, name=name)
     
     def standard_exponential(
         self,
         size: int | tuple[int, ...] | None = None, 
         dtype = None,
         method: Literal["zig", "inv"] = None,
         *,
@@ -152,15 +151,15 @@
         like: MetaArray | LazyImgArray =None,
     ) -> ImgArray:
         size, name, axes = _normalize_like(size, name, axes, like)
     
         arr = self._rng.standard_exponential(size=size, dtype=dtype, method=method)
         if np.isscalar(arr):
             return arr
-        return asarray(arr, axes=axes, name=name)
+        return asarray(xp.asnumpy(arr), axes=axes, name=name)
     
     def random(
         self,
         size: int | tuple[int, ...] | None = None, 
         dtype = None,
         *,
         axes: AxesLike | None = None,
@@ -168,15 +167,15 @@
         like: MetaArray | LazyImgArray =None,
     ) -> ImgArray:
         size, name, axes = _normalize_like(size, name, axes, like)
     
         arr = self._rng.random(size=size, dtype=dtype)
         if np.isscalar(arr):
             return arr
-        return asarray(arr, axes=axes, name=name)
+        return asarray(xp.asnumpy(arr), axes=axes, name=name)
     
     def normal(
         self,
         loc: float | np.ndarray = 0.,
         scale: float | np.ndarray = 1.,
         size: int | tuple[int, ...] | None = None,
         *,
@@ -185,15 +184,15 @@
         like: MetaArray | LazyImgArray =None,
     ) -> ImgArray:
         size, name, axes = _normalize_like(size, name, axes, like)
     
         arr = self._rng.normal(loc=loc, scale=scale, size=size)
         if np.isscalar(arr):
             return arr
-        return asarray(arr, axes=axes, name=name)
+        return asarray(xp.asnumpy(arr), axes=axes, name=name)
 
     def poisson(
         self,
         lam: float,
         size: int | tuple[int, ...] | None = None,
         *,
         axes: AxesLike | None = None,
@@ -201,15 +200,15 @@
         like: MetaArray | LazyImgArray =None,
     ) -> ImgArray:
         size, name, axes = _normalize_like(size, name, axes, like)
     
         arr = self._rng.poisson(lam=lam, size=size)
         if np.isscalar(arr):
             return arr
-        return asarray(arr, axes=axes, name=name)
+        return asarray(xp.asnumpy(arr), axes=axes, name=name)
     
     def random_uint8(
         self,
         size: int | tuple[int], 
         *, 
         name: str = None,
         axes: str = None,
```

### Comparing `impy_array-2.2.4/impy/roi.py` & `impy_array-2.2.5/impy/roi.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/arrays/__init__.py` & `impy_array-2.2.5/impy/arrays/__init__.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/arrays/_deprecated.py` & `impy_array-2.2.5/impy/arrays/_deprecated.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/arrays/_imshow.py` & `impy_array-2.2.5/impy/arrays/_imshow.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/arrays/axesmixin.py` & `impy_array-2.2.5/impy/arrays/axesmixin.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/arrays/big.py` & `impy_array-2.2.5/impy/arrays/big.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/arrays/imgarray.py` & `impy_array-2.2.5/impy/arrays/imgarray.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/arrays/label.py` & `impy_array-2.2.5/impy/arrays/label.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/arrays/labeledarray.py` & `impy_array-2.2.5/impy/arrays/labeledarray.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/arrays/lazy.py` & `impy_array-2.2.5/impy/arrays/lazy.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/arrays/phasearray.py` & `impy_array-2.2.5/impy/arrays/phasearray.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/arrays/specials.py` & `impy_array-2.2.5/impy/arrays/specials.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/arrays/tiled.py` & `impy_array-2.2.5/impy/arrays/tiled.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,16 @@
         self._img = weakref.ref(img)
         self._chunks = chunks
         self._depth = depth
         self._boundary = boundary
 
     @property
     def chunks(self) -> tuple[int, ...]:
-        return self.chunks
+        """Chunksize of the tiled image."""
+        return self._chunks
 
     @property
     def depth(self) -> tuple[int, ...]:
         return self._depth
 
     @property
     def boundary(self) -> str:
@@ -78,23 +79,26 @@
         if img is None:
             raise RuntimeError("Image has been deleted")
         return img
     
     def _map_overlap(self, func: Callable[[np.ndarray], np.ndarray], *args, **kwargs) -> np.ndarray:
         img = self._deref_image()
         input = da.from_array(img.value, chunks=self._chunks)
-        out: np.ndarray = da.map_overlap(
-            func, 
-            input,
-            *args,
-            depth=self.depth,
-            boundary=self.boundary,
-            dtype=img.dtype,
-            **kwargs,
-        ).compute()
+        out: np.ndarray = xp.asnumpy(
+            da.map_overlap(
+                func, 
+                input,
+                *args,
+                depth=self.depth,
+                boundary=self.boundary,
+                dtype=img.dtype,
+                **kwargs,
+            ).compute()
+        )
+        
         return out.view(img.__class__)._set_info(img, img.axes)
 
     def lowpass_filter(self, cutoff: float = 0.2, order: int = 2) -> ImgArray:
         return self._map_overlap(_lowpass, cutoff=cutoff, order=order)
     
     def lucy(
         self,
@@ -107,16 +111,17 @@
         
         def func(arr: np.ndarray):
             psf_ft, psf_ft_conj = _deconv.check_psf(arr.shape, scale, psf)
             return _deconv.richardson_lucy(arr, psf_ft, psf_ft_conj, niter, eps)
             
         return self._map_overlap(func)
     
-    def gaussian_filter(self, sigma: float, fourier: bool = False) -> ImgArray:
-        return self._map_overlap(_filters.gaussian_filter, sigma=sigma, fourier=fourier)
+    def gaussian_filter(self, sigma: float = 1.0, fourier: bool = False) -> ImgArray:
+        filter_func = _filters.gaussian_filter_fourier if fourier else _filters.gaussian_filter
+        return self._map_overlap(filter_func, sigma=sigma)
     
     def dog_filter(
         self,
         low_sigma: float = 1.0,
         high_sigma: float | None = None,
         fourier: bool = False,
     ) -> ImgArray:
```

### Comparing `impy_array-2.2.4/impy/arrays/_utils/_corr.py` & `impy_array-2.2.5/impy/arrays/_utils/_corr.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/arrays/_utils/_deconv.py` & `impy_array-2.2.5/impy/arrays/_utils/_deconv.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/arrays/_utils/_docs.py` & `impy_array-2.2.5/impy/arrays/_utils/_docs.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/arrays/_utils/_filters.py` & `impy_array-2.2.5/impy/arrays/_utils/_filters.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,17 +88,17 @@
         else:
             kalman_gain = predicted_var / (predicted_var + noise_var)
             estimate = gain*estimate + (1.0 - gain)*img + kalman_gain*(img - estimate)
             predicted_var *= 1 - kalman_gain
         out[t] = estimate
     return out
 
-def gaussian_filter_fourier(img: np.ndarray, sigma: float):
-    img_ft = xp.fft.fftn(img)
-    out_ft = _fourier_gaussian(img_ft, sigma)
+def gaussian_filter_fourier(img, sigma: float):
+    img_ft = xp.fft.fftn(xp.asarray(img))
+    out_ft = xp.ndi.fourier_gaussian(img_ft, sigma)
     return xp.fft.ifftn(out_ft).real
 
 def fill_hole(img: np.ndarray, mask: np.ndarray):
     from skimage.morphology import reconstruction
     seed = np.copy(img)
     seed[1:-1, 1:-1] = img.max()
     return reconstruction(seed, mask, method="erosion")
@@ -127,18 +127,18 @@
     return out
     
 def dog_filter(img, low_sigma, high_sigma, mode="reflect", cval=0.0):
     filt_l = gaussian_filter(img, low_sigma, mode=mode, cval=cval)
     filt_h = gaussian_filter(img, high_sigma, mode=mode, cval=cval)
     return filt_l - filt_h
 
-def dog_filter_fourier(img: np.ndarray, low_sigma: float, high_sigma: float):
-    img_ft = xp.fft.fftn(img)
-    filt_l = _fourier_gaussian(img_ft, low_sigma)
-    filt_h = _fourier_gaussian(img_ft, high_sigma)
+def dog_filter_fourier(img, low_sigma: float, high_sigma: float):
+    img_ft = xp.fft.fftn(xp.asarray(img))
+    filt_l = xp.ndi.fourier_gaussian(img_ft, low_sigma)
+    filt_h = xp.ndi.fourier_gaussian(img_ft, high_sigma)
     return xp.fft.ifftn(filt_l - filt_h).real
 
 def doh_filter(img, sigma, pxsize):
     eigval = hessian_eigval(img, sigma, pxsize)
     eigval[eigval>0] = 0
     det = xp.abs(xp.prod(eigval, axis=-1))
     return det
```

### Comparing `impy_array-2.2.4/impy/arrays/_utils/_glcm.py` & `impy_array-2.2.5/impy/arrays/_utils/_glcm.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/arrays/_utils/_linalg.py` & `impy_array-2.2.5/impy/arrays/_utils/_linalg.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/arrays/_utils/_misc.py` & `impy_array-2.2.5/impy/arrays/_utils/_misc.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/arrays/_utils/_plot.py` & `impy_array-2.2.5/impy/arrays/_utils/_plot.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/arrays/_utils/_process_numba.py` & `impy_array-2.2.5/impy/arrays/_utils/_process_numba.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/arrays/_utils/_skimage.py` & `impy_array-2.2.5/impy/arrays/_utils/_skimage.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/arrays/_utils/_structures.py` & `impy_array-2.2.5/impy/arrays/_utils/_structures.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/arrays/_utils/_transform.py` & `impy_array-2.2.5/impy/arrays/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/arrays/bases/metaarray.py` & `impy_array-2.2.5/impy/arrays/bases/metaarray.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/arrays/bases/overload.py` & `impy_array-2.2.5/impy/arrays/bases/overload.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/axes/_axes.py` & `impy_array-2.2.5/impy/axes/_axes.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/axes/_axes_tuple.py` & `impy_array-2.2.5/impy/axes/_axes_tuple.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/axes/_axis.py` & `impy_array-2.2.5/impy/axes/_axis.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/axes/_slicer.py` & `impy_array-2.2.5/impy/axes/_slicer.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/frame/frames.py` & `impy_array-2.2.5/impy/frame/frames.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/utils/axesop.py` & `impy_array-2.2.5/impy/utils/axesop.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/utils/deco.py` & `impy_array-2.2.5/impy/utils/deco.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/utils/gauss.py` & `impy_array-2.2.5/impy/utils/gauss.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/utils/misc.py` & `impy_array-2.2.5/impy/utils/misc.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/utils/slicer.py` & `impy_array-2.2.5/impy/utils/slicer.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/viewer/utils.py` & `impy_array-2.2.5/impy/viewer/utils.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/impy/viewer/viewer.py` & `impy_array-2.2.5/impy/viewer/viewer.py`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/.gitignore` & `impy_array-2.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/LICENSE` & `impy_array-2.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/README.md` & `impy_array-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/pyproject.toml` & `impy_array-2.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `impy_array-2.2.4/PKG-INFO` & `impy_array-2.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: impy-array
-Version: 2.2.4
+Version: 2.2.5
 Summary: Speed up coding/extending image analysis in Python.
 Project-URL: Download, https://github.com/hanjinliu/impy
 Author-email: Hanjin Liu <liuhanjin-sc@g.ecc.u-tokyo.ac.jp>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, hanjinliu
         All rights reserved.
```

