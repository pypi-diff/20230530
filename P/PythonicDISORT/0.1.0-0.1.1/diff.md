# Comparing `tmp/PythonicDISORT-0.1.0.tar.gz` & `tmp/PythonicDISORT-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonicDISORT-0.1.0.tar", last modified: Tue May 30 10:14:07 2023, max compression
+gzip compressed data, was "PythonicDISORT-0.1.1.tar", last modified: Tue May 30 10:20:47 2023, max compression
```

## Comparing `PythonicDISORT-0.1.0.tar` & `PythonicDISORT-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:14:07.553220 PythonicDISORT-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-05-30 10:14:07.553220 PythonicDISORT-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-05-30 10:13:47.000000 PythonicDISORT-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-30 10:13:48.000000 PythonicDISORT-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 10:14:07.553220 PythonicDISORT-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:14:07.549219 PythonicDISORT-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:14:07.549219 PythonicDISORT-0.1.0/src/PythonicDISORT/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-30 10:13:48.000000 PythonicDISORT-0.1.0/src/PythonicDISORT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12306 2023-05-30 10:13:48.000000 PythonicDISORT-0.1.0/src/PythonicDISORT/_loop_and_assemble_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-05-30 10:13:48.000000 PythonicDISORT-0.1.0/src/PythonicDISORT/_one_Fourier_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    20125 2023-05-30 10:13:48.000000 PythonicDISORT-0.1.0/src/PythonicDISORT/pydisort.py
--rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-05-30 10:13:48.000000 PythonicDISORT-0.1.0/src/PythonicDISORT/subroutines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:14:07.553220 PythonicDISORT-0.1.0/src/PythonicDISORT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-05-30 10:14:07.000000 PythonicDISORT-0.1.0/src/PythonicDISORT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-30 10:14:07.000000 PythonicDISORT-0.1.0/src/PythonicDISORT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:14:07.000000 PythonicDISORT-0.1.0/src/PythonicDISORT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-30 10:14:07.000000 PythonicDISORT-0.1.0/src/PythonicDISORT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-30 10:14:07.000000 PythonicDISORT-0.1.0/src/PythonicDISORT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:20:47.358224 PythonicDISORT-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-05-30 10:20:47.358224 PythonicDISORT-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-05-30 10:20:26.000000 PythonicDISORT-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-30 10:20:27.000000 PythonicDISORT-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 10:20:47.358224 PythonicDISORT-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:20:47.354223 PythonicDISORT-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:20:47.358224 PythonicDISORT-0.1.1/src/PythonicDISORT/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-30 10:20:27.000000 PythonicDISORT-0.1.1/src/PythonicDISORT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12306 2023-05-30 10:20:27.000000 PythonicDISORT-0.1.1/src/PythonicDISORT/_loop_and_assemble_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-05-30 10:20:27.000000 PythonicDISORT-0.1.1/src/PythonicDISORT/_one_Fourier_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-05-30 10:20:27.000000 PythonicDISORT-0.1.1/src/PythonicDISORT/pydisort.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10195 2023-05-30 10:20:27.000000 PythonicDISORT-0.1.1/src/PythonicDISORT/subroutines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:20:47.358224 PythonicDISORT-0.1.1/src/PythonicDISORT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-05-30 10:20:47.000000 PythonicDISORT-0.1.1/src/PythonicDISORT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-30 10:20:47.000000 PythonicDISORT-0.1.1/src/PythonicDISORT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:20:47.000000 PythonicDISORT-0.1.1/src/PythonicDISORT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-30 10:20:47.000000 PythonicDISORT-0.1.1/src/PythonicDISORT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-30 10:20:47.000000 PythonicDISORT-0.1.1/src/PythonicDISORT.egg-info/top_level.txt
```

### Comparing `PythonicDISORT-0.1.0/PKG-INFO` & `PythonicDISORT-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonicDISORT
-Version: 0.1.0
+Version: 0.1.1
 Summary: Discrete Ordinates Solver for the (1D) Radiative Transfer Equation in a single or multi-layer atmosphere.
 Author-email: Dion HO Jia Xu <dh3065@columbia.edu>
 Project-URL: Homepage, https://github.com/LDEO-CREW/PythonicDISORT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `PythonicDISORT-0.1.0/README.md` & `PythonicDISORT-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `PythonicDISORT-0.1.0/pyproject.toml` & `PythonicDISORT-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 dependencies = [
   "numpy>=1.17.3",
   "scipy>=1.8.0",
 ]
 name = "PythonicDISORT"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Dion HO Jia Xu", email="dh3065@columbia.edu" },
 ]
 description = "Discrete Ordinates Solver for the (1D) Radiative Transfer Equation in a single or multi-layer atmosphere."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `PythonicDISORT-0.1.0/src/PythonicDISORT/_loop_and_assemble_results.py` & `PythonicDISORT-0.1.1/src/PythonicDISORT/_loop_and_assemble_results.py`

 * *Files identical despite different names*

### Comparing `PythonicDISORT-0.1.0/src/PythonicDISORT/_one_Fourier_mode.py` & `PythonicDISORT-0.1.1/src/PythonicDISORT/_one_Fourier_mode.py`

 * *Files identical despite different names*

### Comparing `PythonicDISORT-0.1.0/src/PythonicDISORT/pydisort.py` & `PythonicDISORT-0.1.1/src/PythonicDISORT/pydisort.py`

 * *Files 1% similar despite different names*

```diff
@@ -393,19 +393,19 @@
             tau = np.atleast_1d(tau)
             phi = np.atleast_1d(phi)
             NT_corrections = TMS_correction(tau, phi)
 
             # We provide two options below, comment and uncomment as desired.
             # Option 2 is more computationally efficient but would prevent the use of autograd for testing.
 
-            NT_corrections = NT_corrections + np.concatenate(
-                [np.zeros((N, len(tau), len(phi))), IMS_correction(tau, phi)], axis=0
-            )  # Option 1
+            #NT_corrections = NT_corrections + np.concatenate(
+            #    [np.zeros((N, len(tau), len(phi))), IMS_correction(tau, phi)], axis=0
+            #)  # Option 1
 
-            #NT_corrections[N:, :, :] += IMS_correction(tau, phi)  # Option 2
+            NT_corrections[N:, :, :] += IMS_correction(tau, phi)  # Option 2
 
             if return_Fourier_error:
                 u_star_outputs = u_star(tau, phi, True)
                 return (
                     u_star_outputs[0] + np.squeeze(NT_corrections),
                     u_star_outputs[1],
                 )
```

### Comparing `PythonicDISORT-0.1.0/src/PythonicDISORT/subroutines.py` & `PythonicDISORT-0.1.1/src/PythonicDISORT/subroutines.py`

 * *Files identical despite different names*

### Comparing `PythonicDISORT-0.1.0/src/PythonicDISORT.egg-info/PKG-INFO` & `PythonicDISORT-0.1.1/src/PythonicDISORT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonicDISORT
-Version: 0.1.0
+Version: 0.1.1
 Summary: Discrete Ordinates Solver for the (1D) Radiative Transfer Equation in a single or multi-layer atmosphere.
 Author-email: Dion HO Jia Xu <dh3065@columbia.edu>
 Project-URL: Homepage, https://github.com/LDEO-CREW/PythonicDISORT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

