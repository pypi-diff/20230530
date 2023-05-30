# Comparing `tmp/xarray-beam-0.6.1.tar.gz` & `tmp/xarray-beam-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarray-beam-0.6.1.tar", last modified: Sun May 28 17:47:31 2023, max compression
+gzip compressed data, was "xarray-beam-0.6.2.tar", last modified: Tue May 30 15:17:22 2023, max compression
```

## Comparing `xarray-beam-0.6.1.tar` & `xarray-beam-0.6.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2023-05-28 17:47:31.147050 xarray-beam-0.6.1/
--rw-r--r--   0 shoyer   (365133) eng       (5000)    11358 2021-05-11 23:10:09.000000 xarray-beam-0.6.1/LICENSE
--rw-r--r--   0 shoyer   (365133) eng       (5000)      262 2023-05-28 17:47:31.146874 xarray-beam-0.6.1/PKG-INFO
--rw-r--r--   0 shoyer   (365133) eng       (5000)     2042 2022-09-03 04:41:09.000000 xarray-beam-0.6.1/README.md
--rw-r--r--   0 shoyer   (365133) eng       (5000)       99 2023-02-08 01:59:34.000000 xarray-beam-0.6.1/pyproject.toml
--rw-r--r--   0 shoyer   (365133) eng       (5000)       38 2023-05-28 17:47:31.147099 xarray-beam-0.6.1/setup.cfg
--rw-r--r--   0 shoyer   (365133) eng       (5000)     1477 2023-05-28 17:47:15.000000 xarray-beam-0.6.1/setup.py
-drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2023-05-28 17:47:31.143113 xarray-beam-0.6.1/xarray_beam/
--rw-r--r--   0 shoyer   (365133) eng       (5000)     1259 2023-05-28 17:47:15.000000 xarray-beam-0.6.1/xarray_beam/__init__.py
-drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2023-05-28 17:47:31.146577 xarray-beam-0.6.1/xarray_beam/_src/
--rw-r--r--   0 shoyer   (365133) eng       (5000)      575 2021-05-11 23:10:09.000000 xarray-beam-0.6.1/xarray_beam/_src/__init__.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     3676 2023-05-28 17:47:15.000000 xarray-beam-0.6.1/xarray_beam/_src/combiners.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     4708 2023-05-28 17:47:15.000000 xarray-beam-0.6.1/xarray_beam/_src/combiners_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)    17235 2023-05-28 17:47:15.000000 xarray-beam-0.6.1/xarray_beam/_src/core.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)    18487 2023-05-28 17:47:15.000000 xarray-beam-0.6.1/xarray_beam/_src/core_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     5389 2022-09-27 21:22:06.000000 xarray-beam-0.6.1/xarray_beam/_src/integration_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     4688 2022-09-27 21:22:06.000000 xarray-beam-0.6.1/xarray_beam/_src/pangeo_forge.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     6725 2022-09-27 21:22:06.000000 xarray-beam-0.6.1/xarray_beam/_src/pangeo_forge_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)    19755 2023-03-28 17:59:40.000000 xarray-beam-0.6.1/xarray_beam/_src/rechunk.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)    26966 2023-03-28 17:59:40.000000 xarray-beam-0.6.1/xarray_beam/_src/rechunk_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     3283 2023-02-08 01:59:34.000000 xarray-beam-0.6.1/xarray_beam/_src/test_util.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     3805 2022-09-27 21:22:06.000000 xarray-beam-0.6.1/xarray_beam/_src/threadmap.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)     2756 2022-09-27 21:22:06.000000 xarray-beam-0.6.1/xarray_beam/_src/threadmap_test.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)    16172 2023-05-28 17:47:15.000000 xarray-beam-0.6.1/xarray_beam/_src/zarr.py
--rw-r--r--   0 shoyer   (365133) eng       (5000)    12614 2023-05-28 17:47:15.000000 xarray-beam-0.6.1/xarray_beam/_src/zarr_test.py
-drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2023-05-28 17:47:31.144043 xarray-beam-0.6.1/xarray_beam.egg-info/
--rw-r--r--   0 shoyer   (365133) eng       (5000)      262 2023-05-28 17:47:31.000000 xarray-beam-0.6.1/xarray_beam.egg-info/PKG-INFO
--rw-r--r--   0 shoyer   (365133) eng       (5000)      707 2023-05-28 17:47:31.000000 xarray-beam-0.6.1/xarray_beam.egg-info/SOURCES.txt
--rw-r--r--   0 shoyer   (365133) eng       (5000)        1 2023-05-28 17:47:31.000000 xarray-beam-0.6.1/xarray_beam.egg-info/dependency_links.txt
--rw-r--r--   0 shoyer   (365133) eng       (5000)      193 2023-05-28 17:47:31.000000 xarray-beam-0.6.1/xarray_beam.egg-info/requires.txt
--rw-r--r--   0 shoyer   (365133) eng       (5000)       12 2023-05-28 17:47:31.000000 xarray-beam-0.6.1/xarray_beam.egg-info/top_level.txt
+drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2023-05-30 15:17:22.785824 xarray-beam-0.6.2/
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    11358 2021-05-11 23:10:09.000000 xarray-beam-0.6.2/LICENSE
+-rw-r--r--   0 shoyer   (365133) eng       (5000)      262 2023-05-30 15:17:22.785689 xarray-beam-0.6.2/PKG-INFO
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     2042 2022-09-03 04:41:09.000000 xarray-beam-0.6.2/README.md
+-rw-r--r--   0 shoyer   (365133) eng       (5000)       99 2023-02-08 01:59:34.000000 xarray-beam-0.6.2/pyproject.toml
+-rw-r--r--   0 shoyer   (365133) eng       (5000)       38 2023-05-30 15:17:22.785868 xarray-beam-0.6.2/setup.cfg
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     1477 2023-05-30 15:16:52.000000 xarray-beam-0.6.2/setup.py
+drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2023-05-30 15:17:22.782714 xarray-beam-0.6.2/xarray_beam/
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     1259 2023-05-30 15:16:52.000000 xarray-beam-0.6.2/xarray_beam/__init__.py
+drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2023-05-30 15:17:22.785488 xarray-beam-0.6.2/xarray_beam/_src/
+-rw-r--r--   0 shoyer   (365133) eng       (5000)      575 2021-05-11 23:10:09.000000 xarray-beam-0.6.2/xarray_beam/_src/__init__.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     3676 2023-05-28 17:47:15.000000 xarray-beam-0.6.2/xarray_beam/_src/combiners.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     4708 2023-05-28 17:47:15.000000 xarray-beam-0.6.2/xarray_beam/_src/combiners_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    17235 2023-05-28 17:47:15.000000 xarray-beam-0.6.2/xarray_beam/_src/core.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    18487 2023-05-28 17:47:15.000000 xarray-beam-0.6.2/xarray_beam/_src/core_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     5389 2022-09-27 21:22:06.000000 xarray-beam-0.6.2/xarray_beam/_src/integration_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     4688 2022-09-27 21:22:06.000000 xarray-beam-0.6.2/xarray_beam/_src/pangeo_forge.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     6725 2022-09-27 21:22:06.000000 xarray-beam-0.6.2/xarray_beam/_src/pangeo_forge_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    19891 2023-05-30 15:16:52.000000 xarray-beam-0.6.2/xarray_beam/_src/rechunk.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    27749 2023-05-30 15:16:52.000000 xarray-beam-0.6.2/xarray_beam/_src/rechunk_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     3283 2023-02-08 01:59:34.000000 xarray-beam-0.6.2/xarray_beam/_src/test_util.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     3805 2022-09-27 21:22:06.000000 xarray-beam-0.6.2/xarray_beam/_src/threadmap.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)     2756 2022-09-27 21:22:06.000000 xarray-beam-0.6.2/xarray_beam/_src/threadmap_test.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    16172 2023-05-28 17:47:15.000000 xarray-beam-0.6.2/xarray_beam/_src/zarr.py
+-rw-r--r--   0 shoyer   (365133) eng       (5000)    12614 2023-05-28 17:47:15.000000 xarray-beam-0.6.2/xarray_beam/_src/zarr_test.py
+drwxr-xr-x   0 shoyer   (365133) eng       (5000)        0 2023-05-30 15:17:22.783335 xarray-beam-0.6.2/xarray_beam.egg-info/
+-rw-r--r--   0 shoyer   (365133) eng       (5000)      262 2023-05-30 15:17:22.000000 xarray-beam-0.6.2/xarray_beam.egg-info/PKG-INFO
+-rw-r--r--   0 shoyer   (365133) eng       (5000)      707 2023-05-30 15:17:22.000000 xarray-beam-0.6.2/xarray_beam.egg-info/SOURCES.txt
+-rw-r--r--   0 shoyer   (365133) eng       (5000)        1 2023-05-30 15:17:22.000000 xarray-beam-0.6.2/xarray_beam.egg-info/dependency_links.txt
+-rw-r--r--   0 shoyer   (365133) eng       (5000)      193 2023-05-30 15:17:22.000000 xarray-beam-0.6.2/xarray_beam.egg-info/requires.txt
+-rw-r--r--   0 shoyer   (365133) eng       (5000)       12 2023-05-30 15:17:22.000000 xarray-beam-0.6.2/xarray_beam.egg-info/top_level.txt
```

### Comparing `xarray-beam-0.6.1/LICENSE` & `xarray-beam-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xarray-beam-0.6.1/README.md` & `xarray-beam-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `xarray-beam-0.6.1/setup.py` & `xarray-beam-0.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     'pangeo-forge-recipes',
     'scipy',
     'h5netcdf'
 ]
 
 setuptools.setup(
     name='xarray-beam',
-    version='0.6.1',
+    version='0.6.2',
     license='Apache 2.0',
     author='Google LLC',
     author_email='noreply@google.com',
     install_requires=base_requires,
     extras_require={
         'tests': tests_requires,
         'docs': docs_requires,
```

### Comparing `xarray-beam-0.6.1/xarray_beam/__init__.py` & `xarray-beam-0.6.2/xarray_beam/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,8 +41,8 @@
 from xarray_beam._src.zarr import (
     open_zarr,
     make_template,
     ChunksToZarr,
     DatasetToZarr,
 )
 
-__version__ = '0.6.1'
+__version__ = '0.6.2'
```

### Comparing `xarray-beam-0.6.1/xarray_beam/_src/__init__.py` & `xarray-beam-0.6.2/xarray_beam/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `xarray-beam-0.6.1/xarray_beam/_src/combiners.py` & `xarray-beam-0.6.2/xarray_beam/_src/combiners.py`

 * *Files identical despite different names*

### Comparing `xarray-beam-0.6.1/xarray_beam/_src/combiners_test.py` & `xarray-beam-0.6.2/xarray_beam/_src/combiners_test.py`

 * *Files identical despite different names*

### Comparing `xarray-beam-0.6.1/xarray_beam/_src/core.py` & `xarray-beam-0.6.2/xarray_beam/_src/core.py`

 * *Files identical despite different names*

### Comparing `xarray-beam-0.6.1/xarray_beam/_src/core_test.py` & `xarray-beam-0.6.2/xarray_beam/_src/core_test.py`

 * *Files identical despite different names*

### Comparing `xarray-beam-0.6.1/xarray_beam/_src/integration_test.py` & `xarray-beam-0.6.2/xarray_beam/_src/integration_test.py`

 * *Files identical despite different names*

### Comparing `xarray-beam-0.6.1/xarray_beam/_src/pangeo_forge.py` & `xarray-beam-0.6.2/xarray_beam/_src/pangeo_forge.py`

 * *Files identical despite different names*

### Comparing `xarray-beam-0.6.1/xarray_beam/_src/pangeo_forge_test.py` & `xarray-beam-0.6.2/xarray_beam/_src/pangeo_forge_test.py`

 * *Files identical despite different names*

### Comparing `xarray-beam-0.6.1/xarray_beam/_src/rechunk.py` & `xarray-beam-0.6.2/xarray_beam/_src/rechunk.py`

 * *Files 1% similar despite different names*

```diff
@@ -456,15 +456,18 @@
     key: core.Key,
     dataset: xarray.Dataset,
 ) -> Iterator[Tuple[core.Key, xarray.Dataset]]:
   """Split a single (Key, xarray.Dataset) pair into separate variables."""
   # TODO(shoyer): add support for partial splitting, into explicitly provided
   # sets of variables
   for var_name in dataset:
-    yield key.replace(vars={var_name}), dataset[[var_name]]
+    new_dataset = dataset[[var_name]]
+    offsets = {k: v for k, v in key.offsets.items() if k in new_dataset.dims}
+    new_key = core.Key(offsets, vars={var_name})
+    yield new_key, new_dataset
 
 
 @dataclasses.dataclass
 class SplitVariables(beam.PTransform):
   """Split existing chunks into a separate chunk per data variable."""
 
   def expand(self, pcoll):
```

### Comparing `xarray-beam-0.6.1/xarray_beam/_src/rechunk_test.py` & `xarray-beam-0.6.2/xarray_beam/_src/rechunk_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,14 +253,41 @@
     with self.subTest('ConsolidateVariables'):
       actual = split | xbeam.ConsolidateVariables()
       self.assertIdenticalChunks(actual, consolidated)
     with self.subTest('SplitVariables'):
       actual = consolidated | xbeam.SplitVariables()
       self.assertIdenticalChunks(actual, split)
 
+  def test_split_variables_with_different_dims(self):
+    inputs = [
+        (
+            xbeam.Key({'x': 0, 'y': 0}, vars=None),
+            xarray.Dataset({
+                'foo': ('x', np.array([1, 2])),
+                'bar': (('x', 'y'), np.array([[1, 2, 3], [4, 5, 6]])),
+            }),
+        ),
+    ]
+    expected = [
+        (
+            xbeam.Key({'x': 0}, vars={'foo'}),
+            xarray.Dataset({
+                'foo': ('x', np.array([1, 2])),
+            }),
+        ),
+        (
+            xbeam.Key({'x': 0, 'y': 0}, vars={'bar'}),
+            xarray.Dataset({
+                'bar': (('x', 'y'), np.array([[1, 2, 3], [4, 5, 6]])),
+            }),
+        ),
+    ]
+    actual = inputs | xbeam.SplitVariables()
+    self.assertIdenticalChunks(actual, expected)
+
   def test_consolidate_chunks_not_fully_shared_dims(self):
     inputs = [
         (
             xbeam.Key({'x': 0}, {'foo'}),
             xarray.Dataset({'foo': ('x', np.arange(0, 5))}),
         ),
         (
```

### Comparing `xarray-beam-0.6.1/xarray_beam/_src/test_util.py` & `xarray-beam-0.6.2/xarray_beam/_src/test_util.py`

 * *Files identical despite different names*

### Comparing `xarray-beam-0.6.1/xarray_beam/_src/threadmap.py` & `xarray-beam-0.6.2/xarray_beam/_src/threadmap.py`

 * *Files identical despite different names*

### Comparing `xarray-beam-0.6.1/xarray_beam/_src/threadmap_test.py` & `xarray-beam-0.6.2/xarray_beam/_src/threadmap_test.py`

 * *Files identical despite different names*

### Comparing `xarray-beam-0.6.1/xarray_beam/_src/zarr.py` & `xarray-beam-0.6.2/xarray_beam/_src/zarr.py`

 * *Files identical despite different names*

### Comparing `xarray-beam-0.6.1/xarray_beam/_src/zarr_test.py` & `xarray-beam-0.6.2/xarray_beam/_src/zarr_test.py`

 * *Files identical despite different names*

### Comparing `xarray-beam-0.6.1/xarray_beam.egg-info/SOURCES.txt` & `xarray-beam-0.6.2/xarray_beam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

