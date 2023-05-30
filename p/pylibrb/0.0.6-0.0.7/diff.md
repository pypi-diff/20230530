# Comparing `tmp/pylibrb-0.0.6.tar.gz` & `tmp/pylibrb-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylibrb-0.0.6.tar", last modified: Sun May 28 22:06:38 2023, max compression
+gzip compressed data, was "pylibrb-0.0.7.tar", last modified: Tue May 30 10:56:07 2023, max compression
```

## Comparing `pylibrb-0.0.6.tar` & `pylibrb-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 22:06:38.151258 pylibrb-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    18091 2023-05-28 22:06:21.000000 pylibrb-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-28 22:06:21.000000 pylibrb-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-28 22:06:38.151258 pylibrb-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-28 22:06:21.000000 pylibrb-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-28 22:06:21.000000 pylibrb-0.0.6/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-28 22:06:21.000000 pylibrb-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-28 22:06:38.151258 pylibrb-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-28 22:06:21.000000 pylibrb-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 22:06:38.147258 pylibrb-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 22:06:38.151258 pylibrb-0.0.6/src/pylibrb/
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-28 22:06:21.000000 pylibrb-0.0.6/src/pylibrb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 22:06:21.000000 pylibrb-0.0.6/src/pylibrb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    36591 2023-05-28 22:06:21.000000 pylibrb-0.0.6/src/pylibrb/pylibrb_ext.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 22:06:38.151258 pylibrb-0.0.6/src/pylibrb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-28 22:06:38.000000 pylibrb-0.0.6/src/pylibrb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-28 22:06:38.000000 pylibrb-0.0.6/src/pylibrb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 22:06:38.000000 pylibrb-0.0.6/src/pylibrb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-28 22:06:38.000000 pylibrb-0.0.6/src/pylibrb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-28 22:06:38.000000 pylibrb-0.0.6/src/pylibrb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 22:06:38.151258 pylibrb-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-05-28 22:06:21.000000 pylibrb-0.0.6/tests/test_stretcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-28 22:06:21.000000 pylibrb-0.0.6/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:56:07.871985 pylibrb-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    18091 2023-05-30 10:55:55.000000 pylibrb-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-30 10:55:55.000000 pylibrb-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-30 10:56:07.871985 pylibrb-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-30 10:55:55.000000 pylibrb-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-30 10:55:55.000000 pylibrb-0.0.7/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-30 10:55:55.000000 pylibrb-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-30 10:56:07.871985 pylibrb-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-30 10:55:55.000000 pylibrb-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:56:07.867985 pylibrb-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:56:07.871985 pylibrb-0.0.7/src/pylibrb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-30 10:55:55.000000 pylibrb-0.0.7/src/pylibrb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 10:55:55.000000 pylibrb-0.0.7/src/pylibrb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    36591 2023-05-30 10:55:55.000000 pylibrb-0.0.7/src/pylibrb/pylibrb_ext.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:56:07.871985 pylibrb-0.0.7/src/pylibrb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-30 10:56:07.000000 pylibrb-0.0.7/src/pylibrb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-30 10:56:07.000000 pylibrb-0.0.7/src/pylibrb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:56:07.000000 pylibrb-0.0.7/src/pylibrb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 10:56:07.000000 pylibrb-0.0.7/src/pylibrb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-30 10:56:07.000000 pylibrb-0.0.7/src/pylibrb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:56:07.871985 pylibrb-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9298 2023-05-30 10:55:55.000000 pylibrb-0.0.7/tests/test_stretcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-30 10:55:55.000000 pylibrb-0.0.7/tests/test_utils.py
```

### Comparing `pylibrb-0.0.6/LICENSE` & `pylibrb-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pylibrb-0.0.6/PKG-INFO` & `pylibrb-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylibrb
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python bindings for the RubberBand library
 Home-page: https://github.com/pawel-glomski/pylibrb
 Author: Paweł Głomski
 Author-email: pglomski.dev@gmail.com
 License: 'GPLv2'
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Intended Audience :: Developers
```

### Comparing `pylibrb-0.0.6/README.md` & `pylibrb-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pylibrb-0.0.6/setup.cfg` & `pylibrb-0.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `pylibrb-0.0.6/setup.py` & `pylibrb-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `pylibrb-0.0.6/src/pylibrb/__init__.py` & `pylibrb-0.0.7/src/pylibrb/__init__.py`

 * *Files identical despite different names*

### Comparing `pylibrb-0.0.6/src/pylibrb/pylibrb_ext.pyi` & `pylibrb-0.0.7/src/pylibrb/pylibrb_ext.pyi`

 * *Files identical despite different names*

### Comparing `pylibrb-0.0.6/src/pylibrb.egg-info/PKG-INFO` & `pylibrb-0.0.7/src/pylibrb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylibrb
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python bindings for the RubberBand library
 Home-page: https://github.com/pawel-glomski/pylibrb
 Author: Paweł Głomski
 Author-email: pglomski.dev@gmail.com
 License: 'GPLv2'
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Intended Audience :: Developers
```

### Comparing `pylibrb-0.0.6/tests/test_stretcher.py` & `pylibrb-0.0.7/tests/test_stretcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pylibrb import RubberBandStretcher, Option
 
 
 @pytest.fixture
 def realtime_stretcher():
   yield RubberBandStretcher(sample_rate=16000,
                             channels=1,
-                            options=Option.PROCESS_REALTIME | Option.ENGINE_FINER)
+                            options=Option.PROCESS_REALTIME | Option.ENGINE_FASTER)
 
 
 class TestStretcherInit:
 
   @pytest.mark.parametrize('sample_rate, expected_exc', [
       (-1, TypeError),
       (pylibrb.MIN_SAMPLE_RATE - 1, ValueError),
@@ -146,15 +146,15 @@
 
   @pytest.mark.parametrize('time_ratio', [1.0, 0.5])
   def test_retrieve_should_return_expected_number_of_samples_for_given_time_ratio(
       self, time_ratio: float, realtime_stretcher: RubberBandStretcher):
     stretcher = realtime_stretcher
 
     audio_data = pylibrb.create_audio_array(stretcher.channels,
-                                            stretcher.get_samples_required(),
+                                            88000,
                                             init_value=1)
     audio_samples = audio_data.shape[pylibrb.SAMPLES_AXIS]
 
     expected_samples = 0.0
     observed_samples = 0
     iters = 10
```

### Comparing `pylibrb-0.0.6/tests/test_utils.py` & `pylibrb-0.0.7/tests/test_utils.py`

 * *Files identical despite different names*

