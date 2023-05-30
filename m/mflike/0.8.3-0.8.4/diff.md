# Comparing `tmp/mflike-0.8.3.tar.gz` & `tmp/mflike-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mflike-0.8.3.tar", last modified: Tue Apr 25 08:52:52 2023, max compression
+gzip compressed data, was "mflike-0.8.4.tar", last modified: Tue May 30 14:51:08 2023, max compression
```

## Comparing `mflike-0.8.3.tar` & `mflike-0.8.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:52:52.383547 mflike-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-04-25 08:52:49.000000 mflike-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-25 08:52:49.000000 mflike-0.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-04-25 08:52:52.383547 mflike-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-04-25 08:52:49.000000 mflike-0.8.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:52:52.383547 mflike-0.8.3/mflike/
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-04-25 08:52:49.000000 mflike-0.8.3/mflike/MFLike.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-25 08:52:49.000000 mflike-0.8.3/mflike/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-25 08:52:52.383547 mflike-0.8.3/mflike/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    13792 2023-04-25 08:52:49.000000 mflike-0.8.3/mflike/mflike.py
--rw-r--r--   0 runner    (1001) docker     (123)    18505 2023-04-25 08:52:49.000000 mflike-0.8.3/mflike/theoryforge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 08:52:52.383547 mflike-0.8.3/mflike.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-04-25 08:52:52.000000 mflike-0.8.3/mflike.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-25 08:52:52.000000 mflike-0.8.3/mflike.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:52:52.000000 mflike-0.8.3/mflike.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-25 08:52:52.000000 mflike-0.8.3/mflike.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-25 08:52:52.000000 mflike-0.8.3/mflike.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 08:52:52.000000 mflike-0.8.3/mflike.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-25 08:52:52.383547 mflike-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-25 08:52:49.000000 mflike-0.8.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-25 08:52:49.000000 mflike-0.8.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:51:08.155874 mflike-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-30 14:51:04.000000 mflike-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-30 14:51:04.000000 mflike-0.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-05-30 14:51:08.155874 mflike-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-30 14:51:04.000000 mflike-0.8.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:51:08.155874 mflike-0.8.4/mflike/
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-05-30 14:51:04.000000 mflike-0.8.4/mflike/MFLike.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-30 14:51:04.000000 mflike-0.8.4/mflike/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-30 14:51:08.155874 mflike-0.8.4/mflike/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13750 2023-05-30 14:51:04.000000 mflike-0.8.4/mflike/mflike.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18505 2023-05-30 14:51:04.000000 mflike-0.8.4/mflike/theoryforge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:51:08.155874 mflike-0.8.4/mflike.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-05-30 14:51:08.000000 mflike-0.8.4/mflike.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-30 14:51:08.000000 mflike-0.8.4/mflike.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:51:08.000000 mflike-0.8.4/mflike.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-30 14:51:08.000000 mflike-0.8.4/mflike.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-30 14:51:08.000000 mflike-0.8.4/mflike.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:51:08.000000 mflike-0.8.4/mflike.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-30 14:51:08.155874 mflike-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-30 14:51:04.000000 mflike-0.8.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-05-30 14:51:04.000000 mflike-0.8.4/versioneer.py
```

### Comparing `mflike-0.8.3/LICENSE` & `mflike-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mflike-0.8.3/PKG-INFO` & `mflike-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mflike
-Version: 0.8.3
+Version: 0.8.4
 Summary: SO LAT multi-frequency likelihood for cobaya
 Home-page: https://github.com/simonsobs/LAT_MFLike
 Author: Simons Observatory Collaboration Power Spectrum Group aka so_ps 1 & 2
 License: BSD license
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `mflike-0.8.3/README.rst` & `mflike-0.8.4/README.rst`

 * *Files identical despite different names*

### Comparing `mflike-0.8.3/mflike/MFLike.yaml` & `mflike-0.8.4/mflike/MFLike.yaml`

 * *Files identical despite different names*

### Comparing `mflike-0.8.3/mflike/mflike.py` & `mflike-0.8.4/mflike/mflike.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     foregrounds: dict
     top_hat_band: dict
     systematics_template: dict
 
     def initialize(self):
         # Set default values to data member not initialized via yaml file
         self.l_bpws = None
-        self.freqs = None
         self.spec_meta = []
 
         # Set path to data
         if (not getattr(self, "path", None)) and (not getattr(self, packages_path_input, None)):
             raise LoggedError(
                 self.log,
                 "No path given to MFLike data. Set the likelihood property "
@@ -287,15 +286,15 @@
                     # will all be sampled at the same ells.
                     self.l_bpws = ws.values
 
                 # Symmetrize if needed.
                 if (pol in ["TE", "ET"]) and symm:
                     pol2 = pol[::-1]
                     pols.remove(pol2)
-                    tname_1, tname_2, dtype = get_sacc_names(pol2, exp_1, exp_2, freq_1, freq_2)
+                    tname_1, tname_2, dtype = get_sacc_names(pol2, exp_1, exp_2)
                     ind2 = s.indices(dtype, (tname_1, tname_2))
                     cls2 = s.get_ell_cl(dtype, tname_1, tname_2)[1]
                     cls = 0.5 * (cls + cls2)
 
                     for i, (j1, j2) in enumerate(zip(ind, ind2)):
                         mat_compress[index_sofar + i, j1] = 0.5
                         mat_compress[index_sofar + i, j2] = 0.5
```

### Comparing `mflike-0.8.3/mflike/theoryforge.py` & `mflike-0.8.4/mflike/theoryforge.py`

 * *Files identical despite different names*

### Comparing `mflike-0.8.3/mflike.egg-info/PKG-INFO` & `mflike-0.8.4/mflike.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mflike
-Version: 0.8.3
+Version: 0.8.4
 Summary: SO LAT multi-frequency likelihood for cobaya
 Home-page: https://github.com/simonsobs/LAT_MFLike
 Author: Simons Observatory Collaboration Power Spectrum Group aka so_ps 1 & 2
 License: BSD license
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `mflike-0.8.3/setup.py` & `mflike-0.8.4/setup.py`

 * *Files identical despite different names*

### Comparing `mflike-0.8.3/versioneer.py` & `mflike-0.8.4/versioneer.py`

 * *Files identical despite different names*

