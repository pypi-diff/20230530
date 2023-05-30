# Comparing `tmp/shepherd_data-2023.5.5.tar.gz` & `tmp/shepherd_data-2023.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shepherd_data-2023.5.5.tar", last modified: Wed May  3 19:30:07 2023, max compression
+gzip compressed data, was "shepherd_data-2023.5.6.tar", last modified: Tue May 30 13:03:37 2023, max compression
```

## Comparing `shepherd_data-2023.5.5.tar` & `shepherd_data-2023.5.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:30:07.433923 shepherd_data-2023.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-05-03 19:30:07.433923 shepherd_data-2023.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-03 19:30:07.433923 shepherd_data-2023.5.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:30:07.429923 shepherd_data-2023.5.5/shepherd_data/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/shepherd_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10745 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/shepherd_data/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/shepherd_data/debug_resampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11683 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/shepherd_data/ivonne.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/shepherd_data/mppt.py
--rw-r--r--   0 runner    (1001) docker     (123)    24800 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/shepherd_data/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:30:07.433923 shepherd_data-2023.5.5/shepherd_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9994 2023-05-03 19:30:07.000000 shepherd_data-2023.5.5/shepherd_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-03 19:30:07.000000 shepherd_data-2023.5.5/shepherd_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:30:07.000000 shepherd_data-2023.5.5/shepherd_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-03 19:30:07.000000 shepherd_data-2023.5.5/shepherd_data.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-03 19:30:07.000000 shepherd_data-2023.5.5/shepherd_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-03 19:30:07.000000 shepherd_data-2023.5.5/shepherd_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:30:07.000000 shepherd_data-2023.5.5/shepherd_data.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:30:07.433923 shepherd_data-2023.5.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/tests/test_cli_downsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/tests/test_cli_extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/tests/test_cli_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/tests/test_cli_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/tests/test_ivonne.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-03 19:29:32.000000 shepherd_data-2023.5.5/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:37.808957 shepherd_data-2023.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-05-30 13:03:37.808957 shepherd_data-2023.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-05-30 13:03:04.000000 shepherd_data-2023.5.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-30 13:03:04.000000 shepherd_data-2023.5.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-30 13:03:37.812957 shepherd_data-2023.5.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:37.808957 shepherd_data-2023.5.6/shepherd_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-30 13:03:04.000000 shepherd_data-2023.5.6/shepherd_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-05-30 13:03:04.000000 shepherd_data-2023.5.6/shepherd_data/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-30 13:03:04.000000 shepherd_data-2023.5.6/shepherd_data/debug_resampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11689 2023-05-30 13:03:04.000000 shepherd_data-2023.5.6/shepherd_data/ivonne.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-05-30 13:03:04.000000 shepherd_data-2023.5.6/shepherd_data/mppt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-05-30 13:03:04.000000 shepherd_data-2023.5.6/shepherd_data/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:37.808957 shepherd_data-2023.5.6/shepherd_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-05-30 13:03:37.000000 shepherd_data-2023.5.6/shepherd_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-30 13:03:37.000000 shepherd_data-2023.5.6/shepherd_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:03:37.000000 shepherd_data-2023.5.6/shepherd_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-30 13:03:37.000000 shepherd_data-2023.5.6/shepherd_data.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-30 13:03:37.000000 shepherd_data-2023.5.6/shepherd_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 13:03:37.000000 shepherd_data-2023.5.6/shepherd_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:03:37.000000 shepherd_data-2023.5.6/shepherd_data.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:37.808957 shepherd_data-2023.5.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:03:04.000000 shepherd_data-2023.5.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-30 13:03:04.000000 shepherd_data-2023.5.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-30 13:03:04.000000 shepherd_data-2023.5.6/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-30 13:03:04.000000 shepherd_data-2023.5.6/tests/test_cli_downsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-05-30 13:03:04.000000 shepherd_data-2023.5.6/tests/test_cli_extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-30 13:03:04.000000 shepherd_data-2023.5.6/tests/test_cli_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-30 13:03:04.000000 shepherd_data-2023.5.6/tests/test_cli_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-30 13:03:04.000000 shepherd_data-2023.5.6/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-30 13:03:04.000000 shepherd_data-2023.5.6/tests/test_ivonne.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-30 13:03:04.000000 shepherd_data-2023.5.6/tests/test_reader.py
```

### Comparing `shepherd_data-2023.5.5/PKG-INFO` & `shepherd_data-2023.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shepherd_data
-Version: 2023.5.5
+Version: 2023.5.6
 Summary: Programming- and CLI-Interface for the h5-dataformat of the Shepherd-Testbed
 Home-page: https://pypi.org/project/shepherd-data/
 Author: Ingmar Splitt, Kai Geissdoerfer
 Author-email: ingmar.splitt@tu-dresden.de
 Maintainer-email: ingmar.splitt@tu-dresden.de
 License: MIT
 Project-URL: Tracker, https://github.com/orgua/shepherd-datalib/issues
@@ -162,51 +162,49 @@
   - `jogging_10m.iv`
       - 50 Hz measurement with Short-Circuit-Current and two other parameters
       - recorded with "IVonne"
 
 ### Functionality Update (WIP)
 
 - `BaseReader`
+  - `__repr__()`
   - `read_buffers`
   - `get_calibration_data`
   - `get_window_samples`
   - `get_mode`
   - `get_config`
   - `get_hostname`
   - `get_datatype`
   - `get_hrv_config`
   - `is_valid`
+  - `energy()`
+  - `check_timediffs()`
+  - `data_timediffs()`
+  - `get_metadata()`
+  - `save_metadata()`
 
 - `BaseWriter(BaseReader)`
   - `append_iv_data_raw`
   - `append_iv_data_si`
-  - `set_config`
-  - `set_window_samples`
-  - `set_hostname`
+  - `store_config`
+  - `store_hostname`
 
 - `Reader(BaseReader)`
-  - `__repr__()`
-  - `check_timediffs()`
-  - `data_timediffs()`
-  - `get_metadata()`
-  - `save_metadata()`
-  - `energy()`
   - `save_csv()`
   - `save_log()`
   - `downsample()`
   - `resample()`
   - `generate_plot_data()`
   - `assemble_plot()`
   - `plot_to_file()`
   - `multiplot_to_file()`
+
 - `Writer(BaseWriter)`
   - (no extending methods)
 
-
-
 ## CLI-Interface
 
 After installing the module the datalib offers some often needed functionality on the command line:
 
 **Validate Recordings**
 
 - takes a file or directory as an argument
```

### Comparing `shepherd_data-2023.5.5/README.md` & `shepherd_data-2023.5.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -127,51 +127,49 @@
   - `jogging_10m.iv`
       - 50 Hz measurement with Short-Circuit-Current and two other parameters
       - recorded with "IVonne"
 
 ### Functionality Update (WIP)
 
 - `BaseReader`
+  - `__repr__()`
   - `read_buffers`
   - `get_calibration_data`
   - `get_window_samples`
   - `get_mode`
   - `get_config`
   - `get_hostname`
   - `get_datatype`
   - `get_hrv_config`
   - `is_valid`
+  - `energy()`
+  - `check_timediffs()`
+  - `data_timediffs()`
+  - `get_metadata()`
+  - `save_metadata()`
 
 - `BaseWriter(BaseReader)`
   - `append_iv_data_raw`
   - `append_iv_data_si`
-  - `set_config`
-  - `set_window_samples`
-  - `set_hostname`
+  - `store_config`
+  - `store_hostname`
 
 - `Reader(BaseReader)`
-  - `__repr__()`
-  - `check_timediffs()`
-  - `data_timediffs()`
-  - `get_metadata()`
-  - `save_metadata()`
-  - `energy()`
   - `save_csv()`
   - `save_log()`
   - `downsample()`
   - `resample()`
   - `generate_plot_data()`
   - `assemble_plot()`
   - `plot_to_file()`
   - `multiplot_to_file()`
+
 - `Writer(BaseWriter)`
   - (no extending methods)
 
-
-
 ## CLI-Interface
 
 After installing the module the datalib offers some often needed functionality on the command line:
 
 **Validate Recordings**
 
 - takes a file or directory as an argument
```

### Comparing `shepherd_data-2023.5.5/setup.cfg` & `shepherd_data-2023.5.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `shepherd_data-2023.5.5/shepherd_data/cli.py` & `shepherd_data-2023.5.6/shepherd_data/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from typing import List
 from typing import Optional
 
 import click
 
 from shepherd_core import get_verbose_level
 from shepherd_core import set_verbose_level
+from shepherd_core.commons import samplerate_sps_default
 
 from . import Reader
 from . import Writer
 from . import __version__
 
 logger = logging.getLogger("SHPData.cli")
 
@@ -119,16 +120,16 @@
                     mode=shpr.get_mode(),
                     datatype=shpr.get_datatype(),
                     window_samples=shpr.get_window_samples(),
                     cal_data=shpr.get_calibration_data(),
                     verbose=verbose_level >= 2,
                 ) as shpw:
                     shpw["ds_factor"] = ds_factor
-                    shpw.set_hostname(shpr.get_hostname())
-                    shpw.set_config(shpr.get_config())
+                    shpw.store_hostname(shpr.get_hostname())
+                    shpw.store_config(shpr.get_config())
                     shpr.downsample(
                         shpr.ds_time, shpw.ds_time, ds_factor=ds_factor, is_time=True
                     )
                     shpr.downsample(
                         shpr.ds_voltage, shpw.ds_voltage, ds_factor=ds_factor
                     )
                     shpr.downsample(
@@ -193,15 +194,16 @@
 )
 def downsample(
     in_data: Path, ds_factor: Optional[float], sample_rate: Optional[int]
 ) -> None:
     """Creates an array of downsampling-files from file
     or directory containing shepherd-recordings"""
     if ds_factor is None and sample_rate is not None and sample_rate >= 1:
-        ds_factor = int(Reader.samplerate_sps_default / sample_rate)
+        ds_factor = int(samplerate_sps_default / sample_rate)
+        # TODO: shouldn't current sps be based on file rather than default?
     if isinstance(ds_factor, (float, int)) and ds_factor >= 1:
         ds_list = [ds_factor]
     else:
         ds_list = [5, 25, 100, 500, 2_500, 10_000, 50_000, 250_000, 1_000_000]
 
     files = path_to_flist(in_data)
     verbose_level = get_verbose_level()
@@ -222,16 +224,16 @@
                     mode=shpr.get_mode(),
                     datatype=shpr.get_datatype(),
                     window_samples=shpr.get_window_samples(),
                     cal_data=shpr.get_calibration_data(),
                     verbose=verbose_level >= 2,
                 ) as shpw:
                     shpw["ds_factor"] = _factor
-                    shpw.set_hostname(shpr.get_hostname())
-                    shpw.set_config(shpr.get_config())
+                    shpw.store_hostname(shpr.get_hostname())
+                    shpw.store_config(shpr.get_config())
                     shpr.downsample(
                         shpr.ds_time, shpw.ds_time, ds_factor=_factor, is_time=True
                     )
                     shpr.downsample(shpr.ds_voltage, shpw.ds_voltage, ds_factor=_factor)
                     shpr.downsample(shpr.ds_current, shpw.ds_current, ds_factor=_factor)
```

### Comparing `shepherd_data-2023.5.5/shepherd_data/debug_resampler.py` & `shepherd_data-2023.5.6/shepherd_data/debug_resampler.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2023.5.5/shepherd_data/ivonne.py` & `shepherd_data-2023.5.6/shepherd_data/ivonne.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
             return
 
         v_proto = np.linspace(0, v_max, pts_per_curve)
 
         with Writer(
             shp_output, datatype="ivcurve", window_samples=pts_per_curve
         ) as sfw:
-            sfw.set_hostname("IVonne")
+            sfw.store_hostname("IVonne")
             curve_interval_us = round(sfw.sample_interval_ns * pts_per_curve / 1000)
             up_factor = self.sample_interval_ns // sfw.sample_interval_ns
             max_elements = math.ceil(sfw.max_elements // up_factor)
             job_iter = trange(0, df_elements_n, max_elements, desc="generate ivcurves")
 
             for idx in job_iter:
                 idx_top = min(idx + max_elements, df_elements_n)
@@ -195,15 +195,15 @@
 
         if tracker is None:
             tracker = OptimalTracker(
                 v_max,
             )
 
         with Writer(shp_output, datatype="ivsample") as sfw:
-            sfw.set_hostname("IVonne")
+            sfw.store_hostname("IVonne")
             interval_us = round(sfw.sample_interval_ns / 1000)
             up_factor = self.sample_interval_ns // sfw.sample_interval_ns
             max_elements = math.ceil(sfw.max_elements // up_factor)
             job_iter = trange(0, df_elements_n, max_elements, desc="generate ivsamples")
 
             for idx in job_iter:
                 # select (max_elements + 1) elements, so upsampling is without gaps
@@ -254,15 +254,15 @@
             df_elements_n = self._df.shape[0]
 
         if shp_output.exists():
             self._logger.warning("%s already exists, will skip", shp_output.name)
             return
 
         with Writer(shp_output, datatype="isc_voc") as sfw:
-            sfw.set_hostname("IVonne")
+            sfw.store_hostname("IVonne")
             interval_us = round(sfw.sample_interval_ns / 1000)
             up_factor = self.sample_interval_ns // sfw.sample_interval_ns
             max_elements = math.ceil(sfw.max_elements // up_factor)
             job_iter = trange(0, df_elements_n, max_elements, desc="generate upsample")
 
             for idx in job_iter:
                 # select (max_elements + 1) elements, so upsampling is without gaps
```

### Comparing `shepherd_data-2023.5.5/shepherd_data/mppt.py` & `shepherd_data-2023.5.6/shepherd_data/mppt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 Harvesters, simple and fast approach.
 Might be exchanged by shepherds py-model of pru-harvesters
 """
 import numpy as np
 import pandas as pd
 
-from shepherd_core.calibration import T_calc
+from shepherd_core import Calc_t
 
 
-def iv_model(voltages: T_calc, coeffs: pd.Series) -> T_calc:
+def iv_model(voltages: Calc_t, coeffs: pd.Series) -> Calc_t:
     """Simple diode based model of a solar panel IV curve.
 
     Args:
         :param voltages: Load voltage of the solar panel
         :param coeffs: three generic coefficients
 
     Returns:
```

### Comparing `shepherd_data-2023.5.5/shepherd_data.egg-info/PKG-INFO` & `shepherd_data-2023.5.6/shepherd_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shepherd-data
-Version: 2023.5.5
+Version: 2023.5.6
 Summary: Programming- and CLI-Interface for the h5-dataformat of the Shepherd-Testbed
 Home-page: https://pypi.org/project/shepherd-data/
 Author: Ingmar Splitt, Kai Geissdoerfer
 Author-email: ingmar.splitt@tu-dresden.de
 Maintainer-email: ingmar.splitt@tu-dresden.de
 License: MIT
 Project-URL: Tracker, https://github.com/orgua/shepherd-datalib/issues
@@ -162,51 +162,49 @@
   - `jogging_10m.iv`
       - 50 Hz measurement with Short-Circuit-Current and two other parameters
       - recorded with "IVonne"
 
 ### Functionality Update (WIP)
 
 - `BaseReader`
+  - `__repr__()`
   - `read_buffers`
   - `get_calibration_data`
   - `get_window_samples`
   - `get_mode`
   - `get_config`
   - `get_hostname`
   - `get_datatype`
   - `get_hrv_config`
   - `is_valid`
+  - `energy()`
+  - `check_timediffs()`
+  - `data_timediffs()`
+  - `get_metadata()`
+  - `save_metadata()`
 
 - `BaseWriter(BaseReader)`
   - `append_iv_data_raw`
   - `append_iv_data_si`
-  - `set_config`
-  - `set_window_samples`
-  - `set_hostname`
+  - `store_config`
+  - `store_hostname`
 
 - `Reader(BaseReader)`
-  - `__repr__()`
-  - `check_timediffs()`
-  - `data_timediffs()`
-  - `get_metadata()`
-  - `save_metadata()`
-  - `energy()`
   - `save_csv()`
   - `save_log()`
   - `downsample()`
   - `resample()`
   - `generate_plot_data()`
   - `assemble_plot()`
   - `plot_to_file()`
   - `multiplot_to_file()`
+
 - `Writer(BaseWriter)`
   - (no extending methods)
 
-
-
 ## CLI-Interface
 
 After installing the module the datalib offers some often needed functionality on the command line:
 
 **Validate Recordings**
 
 - takes a file or directory as an argument
```

### Comparing `shepherd_data-2023.5.5/shepherd_data.egg-info/SOURCES.txt` & `shepherd_data-2023.5.6/shepherd_data.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 ./tests/__init__.py
 ./tests/conftest.py
 ./tests/test_cli.py
 ./tests/test_cli_downsample.py
 ./tests/test_cli_extract.py
 ./tests/test_cli_plot.py
 ./tests/test_cli_validate.py
+./tests/test_examples.py
 ./tests/test_ivonne.py
 ./tests/test_reader.py
-./tests/test_writer.py
 shepherd_data.egg-info/PKG-INFO
 shepherd_data.egg-info/SOURCES.txt
 shepherd_data.egg-info/dependency_links.txt
 shepherd_data.egg-info/entry_points.txt
 shepherd_data.egg-info/requires.txt
 shepherd_data.egg-info/top_level.txt
 shepherd_data.egg-info/zip-safe
 tests/test_cli.py
 tests/test_cli_downsample.py
 tests/test_cli_extract.py
 tests/test_cli_plot.py
 tests/test_cli_validate.py
+tests/test_examples.py
 tests/test_ivonne.py
-tests/test_reader.py
-tests/test_writer.py
+tests/test_reader.py
```

### Comparing `shepherd_data-2023.5.5/tests/conftest.py` & `shepherd_data-2023.5.6/tests/conftest.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from pathlib import Path
 
 import numpy as np
 import pytest
 
+from shepherd_core import Compression
 from shepherd_data import Writer
 
 
 def generate_h5_file(file_path: Path, file_name: str = "harvest_example.h5") -> Path:
     store_path = file_path / file_name
 
-    with Writer(store_path, compression=1) as file:
-        file.set_hostname("artificial")
+    with Writer(store_path, compression=Compression.gzip1) as file:
+        file.store_hostname("artificial")
 
         duration_s = 2
         repetitions = 5
         timestamp_vector = np.arange(0.0, duration_s, file.sample_interval_ns / 1e9)
 
         # values in SI units
         voltages = np.linspace(3.60, 1.90, int(file.samplerate_sps * duration_s))
```

### Comparing `shepherd_data-2023.5.5/tests/test_cli_downsample.py` & `shepherd_data-2023.5.6/tests/test_cli_downsample.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2023.5.5/tests/test_cli_extract.py` & `shepherd_data-2023.5.6/tests/test_cli_extract.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2023.5.5/tests/test_cli_plot.py` & `shepherd_data-2023.5.6/tests/test_cli_plot.py`

 * *Files identical despite different names*

### Comparing `shepherd_data-2023.5.5/tests/test_ivonne.py` & `shepherd_data-2023.5.6/tests/test_ivonne.py`

 * *Files identical despite different names*

