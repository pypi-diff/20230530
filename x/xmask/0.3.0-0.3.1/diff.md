# Comparing `tmp/xmask-0.3.0.tar.gz` & `tmp/xmask-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmask-0.3.0.tar", last modified: Sun May  7 06:54:18 2023, max compression
+gzip compressed data, was "xmask-0.3.1.tar", last modified: Tue May 30 19:23:34 2023, max compression
```

## Comparing `xmask-0.3.0.tar` & `xmask-0.3.1.tar`

### file list

```diff
@@ -1,26 +1,30 @@
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-05-07 06:54:18.010465 xmask-0.3.0/
--rw-r--r--   0 giadarol   (503) staff       (20)    11356 2023-03-23 11:05:06.000000 xmask-0.3.0/LICENSE
--rw-r--r--   0 giadarol   (503) staff       (20)      237 2023-03-23 11:05:06.000000 xmask-0.3.0/MANIFEST.in
--rw-r--r--   0 giadarol   (503) staff       (20)      520 2023-05-07 06:54:18.010324 xmask-0.3.0/PKG-INFO
--rw-r--r--   0 giadarol   (503) staff       (20)      115 2023-03-23 11:05:06.000000 xmask-0.3.0/pyproject.toml
--rw-r--r--   0 giadarol   (503) staff       (20)       38 2023-05-07 06:54:18.010511 xmask-0.3.0/setup.cfg
--rw-r--r--   0 giadarol   (503) staff       (20)     1433 2023-03-23 11:05:06.000000 xmask-0.3.0/setup.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-05-07 06:54:18.008472 xmask-0.3.0/xmask/
--rw-r--r--   0 giadarol   (503) staff       (20)      233 2023-03-23 11:05:06.000000 xmask-0.3.0/xmask/__init__.py
--rw-r--r--   0 giadarol   (503) staff       (20)       22 2023-05-07 06:54:02.000000 xmask-0.3.0/xmask/_version.py
--rw-r--r--   0 giadarol   (503) staff       (20)      225 2023-03-23 11:05:06.000000 xmask-0.3.0/xmask/env_and_links.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-05-07 06:54:18.010131 xmask-0.3.0/xmask/lhc/
--rw-r--r--   0 giadarol   (503) staff       (20)      432 2023-05-07 06:53:44.000000 xmask-0.3.0/xmask/lhc/__init__.py
--rw-r--r--   0 giadarol   (503) staff       (20)     5652 2023-05-07 06:53:44.000000 xmask-0.3.0/xmask/lhc/build_madx_and_xsuite_models.py
--rw-r--r--   0 giadarol   (503) staff       (20)     3553 2023-03-23 11:05:06.000000 xmask-0.3.0/xmask/lhc/errors.py
--rw-r--r--   0 giadarol   (503) staff       (20)     2430 2023-05-07 06:53:44.000000 xmask-0.3.0/xmask/lhc/knob_manipulations.py
--rw-r--r--   0 giadarol   (503) staff       (20)     3231 2023-05-07 06:53:44.000000 xmask-0.3.0/xmask/lhc/leveling.py
--rw-r--r--   0 giadarol   (503) staff       (20)    12355 2023-05-07 06:53:44.000000 xmask-0.3.0/xmask/madx_model.py
--rw-r--r--   0 giadarol   (503) staff       (20)     2883 2023-05-07 06:53:44.000000 xmask-0.3.0/xmask/tuning.py
--rw-r--r--   0 giadarol   (503) staff       (20)      728 2023-03-23 11:05:06.000000 xmask-0.3.0/xmask/yaml.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-05-07 06:54:18.009271 xmask-0.3.0/xmask.egg-info/
--rw-r--r--   0 giadarol   (503) staff       (20)      520 2023-05-07 06:54:17.000000 xmask-0.3.0/xmask.egg-info/PKG-INFO
--rw-r--r--   0 giadarol   (503) staff       (20)      434 2023-05-07 06:54:17.000000 xmask-0.3.0/xmask.egg-info/SOURCES.txt
--rw-r--r--   0 giadarol   (503) staff       (20)        1 2023-05-07 06:54:17.000000 xmask-0.3.0/xmask.egg-info/dependency_links.txt
--rw-r--r--   0 giadarol   (503) staff       (20)       49 2023-05-07 06:54:17.000000 xmask-0.3.0/xmask.egg-info/requires.txt
--rw-r--r--   0 giadarol   (503) staff       (20)        6 2023-05-07 06:54:17.000000 xmask-0.3.0/xmask.egg-info/top_level.txt
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-05-30 19:23:34.396993 xmask-0.3.1/
+-rw-r--r--   0 giadarol   (503) staff       (20)    11356 2023-03-23 11:05:06.000000 xmask-0.3.1/LICENSE
+-rw-r--r--   0 giadarol   (503) staff       (20)      237 2023-03-23 11:05:06.000000 xmask-0.3.1/MANIFEST.in
+-rw-r--r--   0 giadarol   (503) staff       (20)      520 2023-05-30 19:23:34.396826 xmask-0.3.1/PKG-INFO
+-rw-r--r--   0 giadarol   (503) staff       (20)      115 2023-03-23 11:05:06.000000 xmask-0.3.1/pyproject.toml
+-rw-r--r--   0 giadarol   (503) staff       (20)       38 2023-05-30 19:23:34.397040 xmask-0.3.1/setup.cfg
+-rw-r--r--   0 giadarol   (503) staff       (20)     1433 2023-03-23 11:05:06.000000 xmask-0.3.1/setup.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-05-30 19:23:34.386289 xmask-0.3.1/tests/
+-rw-r--r--   0 giadarol   (503) staff       (20)    71861 2023-05-30 19:22:48.000000 xmask-0.3.1/tests/test_hllhc14.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    21540 2023-05-30 19:22:48.000000 xmask-0.3.1/tests/test_hllhc14_b1_only.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    29755 2023-05-30 19:22:48.000000 xmask-0.3.1/tests/test_lhc_ion.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-05-30 19:23:34.388044 xmask-0.3.1/xmask/
+-rw-r--r--   0 giadarol   (503) staff       (20)      233 2023-03-23 11:05:06.000000 xmask-0.3.1/xmask/__init__.py
+-rw-r--r--   0 giadarol   (503) staff       (20)       22 2023-05-30 19:23:07.000000 xmask-0.3.1/xmask/_version.py
+-rw-r--r--   0 giadarol   (503) staff       (20)      225 2023-03-23 11:05:06.000000 xmask-0.3.1/xmask/env_and_links.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-05-30 19:23:34.396573 xmask-0.3.1/xmask/lhc/
+-rw-r--r--   0 giadarol   (503) staff       (20)      432 2023-05-07 06:53:44.000000 xmask-0.3.1/xmask/lhc/__init__.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     5652 2023-05-07 06:53:44.000000 xmask-0.3.1/xmask/lhc/build_madx_and_xsuite_models.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     3553 2023-03-23 11:05:06.000000 xmask-0.3.1/xmask/lhc/errors.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     2423 2023-05-30 19:22:48.000000 xmask-0.3.1/xmask/lhc/knob_manipulations.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     3231 2023-05-28 15:35:42.000000 xmask-0.3.1/xmask/lhc/leveling.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    12355 2023-05-07 06:53:44.000000 xmask-0.3.1/xmask/madx_model.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     2883 2023-05-07 06:53:44.000000 xmask-0.3.1/xmask/tuning.py
+-rw-r--r--   0 giadarol   (503) staff       (20)      728 2023-03-23 11:05:06.000000 xmask-0.3.1/xmask/yaml.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-05-30 19:23:34.393355 xmask-0.3.1/xmask.egg-info/
+-rw-r--r--   0 giadarol   (503) staff       (20)      520 2023-05-30 19:23:34.000000 xmask-0.3.1/xmask.egg-info/PKG-INFO
+-rw-r--r--   0 giadarol   (503) staff       (20)      508 2023-05-30 19:23:34.000000 xmask-0.3.1/xmask.egg-info/SOURCES.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)        1 2023-05-30 19:23:34.000000 xmask-0.3.1/xmask.egg-info/dependency_links.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)       49 2023-05-30 19:23:34.000000 xmask-0.3.1/xmask.egg-info/requires.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)        6 2023-05-30 19:23:34.000000 xmask-0.3.1/xmask.egg-info/top_level.txt
```

### Comparing `xmask-0.3.0/LICENSE` & `xmask-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xmask-0.3.0/PKG-INFO` & `xmask-0.3.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmask
-Version: 0.3.0
+Version: 0.3.1
 Summary: Configuration of tracking simulations for the LHC and other accelerators
 Home-page: https://github.com/xsuite/xsuite/issues
 Download-URL: https://pypi.python.org/pypi/xmask
 Author: G. Iadarola et al.
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/xsuite/xsuite/issues
 Project-URL: Source Code, https://github.com/xsuite/xmask/
```

### Comparing `xmask-0.3.0/setup.py` & `xmask-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `xmask-0.3.0/xmask/lhc/build_madx_and_xsuite_models.py` & `xmask-0.3.1/xmask/lhc/build_madx_and_xsuite_models.py`

 * *Files identical despite different names*

### Comparing `xmask-0.3.0/xmask/lhc/errors.py` & `xmask-0.3.1/xmask/lhc/errors.py`

 * *Files identical despite different names*

### Comparing `xmask-0.3.0/xmask/lhc/knob_manipulations.py` & `xmask-0.3.1/xmask/lhc/knob_manipulations.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,12 +50,12 @@
             line.vars['kmax_mo']
             * line.vars[f'i_oct_b{beamn}'] / line.vars['imax_mo']
             / line.vars[f'brho0_b{beamn}'])
 
 def add_correction_term_to_dipole_correctors(line):
     # Add correction term to all dipole correctors
     line.vars['on_corr_co'] = 1
-    for kk in list(line.vars._owner.keys()):
+    for kk in list(line.vars.keys()):
         if kk.startswith('acb'):
             line.vars['corr_co_'+kk] = 0
             line.vars[kk] += (line.vars['corr_co_'+kk] * line.vars['on_corr_co'])
```

### Comparing `xmask-0.3.0/xmask/lhc/leveling.py` & `xmask-0.3.1/xmask/lhc/leveling.py`

 * *Files identical despite different names*

### Comparing `xmask-0.3.0/xmask/madx_model.py` & `xmask-0.3.1/xmask/madx_model.py`

 * *Files identical despite different names*

### Comparing `xmask-0.3.0/xmask/tuning.py` & `xmask-0.3.1/xmask/tuning.py`

 * *Files identical despite different names*

### Comparing `xmask-0.3.0/xmask/yaml.py` & `xmask-0.3.1/xmask/yaml.py`

 * *Files identical despite different names*

### Comparing `xmask-0.3.0/xmask.egg-info/PKG-INFO` & `xmask-0.3.1/xmask.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmask
-Version: 0.3.0
+Version: 0.3.1
 Summary: Configuration of tracking simulations for the LHC and other accelerators
 Home-page: https://github.com/xsuite/xsuite/issues
 Download-URL: https://pypi.python.org/pypi/xmask
 Author: G. Iadarola et al.
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/xsuite/xsuite/issues
 Project-URL: Source Code, https://github.com/xsuite/xmask/
```

