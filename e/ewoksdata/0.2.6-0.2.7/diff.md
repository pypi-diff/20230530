# Comparing `tmp/ewoksdata-0.2.6.tar.gz` & `tmp/ewoksdata-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ewoksdata-0.2.6.tar", last modified: Tue May  2 09:51:58 2023, max compression
+gzip compressed data, was "dist/ewoksdata-0.2.7.tar", last modified: Tue May 30 13:06:15 2023, max compression
```

## Comparing `ewoksdata-0.2.6.tar` & `ewoksdata-0.2.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:51:58.000000 ewoksdata-0.2.6/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2023-05-02 08:44:00.000000 ewoksdata-0.2.6/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     1020 2023-05-02 09:51:58.000000 ewoksdata-0.2.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      267 2023-05-02 08:44:00.000000 ewoksdata-0.2.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-05-02 08:44:00.000000 ewoksdata-0.2.6/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1163 2023-05-02 09:51:58.000000 ewoksdata-0.2.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-02 08:44:00.000000 ewoksdata-0.2.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:51:58.000000 ewoksdata-0.2.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:51:58.000000 ewoksdata-0.2.6/src/ewoksdata/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-02 08:58:44.000000 ewoksdata-0.2.6/src/ewoksdata/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:51:58.000000 ewoksdata-0.2.6/src/ewoksdata/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 09:51:52.000000 ewoksdata-0.2.6/src/ewoksdata/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8413 2023-05-02 09:50:16.000000 ewoksdata-0.2.6/src/ewoksdata/data/bliss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:51:58.000000 ewoksdata-0.2.6/src/ewoksdata/data/hdf5/
--rw-rw-rw-   0 root         (0) root         (0)      622 2023-05-02 08:44:00.000000 ewoksdata-0.2.6/src/ewoksdata/data/hdf5/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6086 2023-05-02 08:44:00.000000 ewoksdata-0.2.6/src/ewoksdata/data/hdf5/config.py
--rw-rw-rw-   0 root         (0) root         (0)     4017 2023-05-02 08:44:00.000000 ewoksdata-0.2.6/src/ewoksdata/data/hdf5/dataset_writer.py
--rw-rw-rw-   0 root         (0) root         (0)      474 2023-05-02 08:44:00.000000 ewoksdata-0.2.6/src/ewoksdata/data/hdf5/types.py
--rw-rw-rw-   0 root         (0) root         (0)     3065 2023-05-02 09:50:16.000000 ewoksdata-0.2.6/src/ewoksdata/data/nexus.py
--rw-rw-rw-   0 root         (0) root         (0)      619 2023-05-02 09:50:16.000000 ewoksdata-0.2.6/src/ewoksdata/data/url.py
--rw-rw-rw-   0 root         (0) root         (0)      722 2023-05-02 08:44:00.000000 ewoksdata-0.2.6/src/ewoksdata/data/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:51:58.000000 ewoksdata-0.2.6/src/ewoksdata/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-02 09:51:52.000000 ewoksdata-0.2.6/src/ewoksdata/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      508 2023-05-02 08:44:00.000000 ewoksdata-0.2.6/src/ewoksdata/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:51:58.000000 ewoksdata-0.2.6/src/ewoksdata/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-05-02 08:44:00.000000 ewoksdata-0.2.6/src/ewoksdata/tests/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3468 2023-05-02 08:44:00.000000 ewoksdata-0.2.6/src/ewoksdata/tests/data/bliss_scans.py
--rw-rw-rw-   0 root         (0) root         (0)     1600 2023-05-02 09:50:16.000000 ewoksdata-0.2.6/src/ewoksdata/tests/test_data_bliss.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-05-02 08:44:00.000000 ewoksdata-0.2.6/src/ewoksdata/tests/test_data_hdf5.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2023-05-02 09:50:16.000000 ewoksdata-0.2.6/src/ewoksdata/tests/test_data_nexus.py
--rw-rw-rw-   0 root         (0) root         (0)     1886 2023-05-02 08:44:00.000000 ewoksdata-0.2.6/src/ewoksdata/tests/test_dataset_writer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-02 09:51:58.000000 ewoksdata-0.2.6/src/ewoksdata.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1020 2023-05-02 09:51:58.000000 ewoksdata-0.2.6/src/ewoksdata.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      850 2023-05-02 09:51:58.000000 ewoksdata-0.2.6/src/ewoksdata.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-02 09:51:58.000000 ewoksdata-0.2.6/src/ewoksdata.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      207 2023-05-02 09:51:58.000000 ewoksdata-0.2.6/src/ewoksdata.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-02 09:51:58.000000 ewoksdata-0.2.6/src/ewoksdata.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:06:15.000000 ewoksdata-0.2.7/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-05-30 11:03:10.000000 ewoksdata-0.2.7/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-05-30 13:06:15.000000 ewoksdata-0.2.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      267 2023-05-30 11:03:10.000000 ewoksdata-0.2.7/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-05-30 11:03:10.000000 ewoksdata-0.2.7/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1163 2023-05-30 13:06:15.000000 ewoksdata-0.2.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-05-30 11:03:10.000000 ewoksdata-0.2.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:06:15.000000 ewoksdata-0.2.7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:06:15.000000 ewoksdata-0.2.7/src/ewoksdata/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-30 13:04:09.000000 ewoksdata-0.2.7/src/ewoksdata/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:06:15.000000 ewoksdata-0.2.7/src/ewoksdata/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 13:06:09.000000 ewoksdata-0.2.7/src/ewoksdata/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8552 2023-05-30 11:03:10.000000 ewoksdata-0.2.7/src/ewoksdata/data/bliss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:06:15.000000 ewoksdata-0.2.7/src/ewoksdata/data/hdf5/
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-05-30 11:03:10.000000 ewoksdata-0.2.7/src/ewoksdata/data/hdf5/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6086 2023-05-30 11:03:10.000000 ewoksdata-0.2.7/src/ewoksdata/data/hdf5/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     9870 2023-05-30 12:59:48.000000 ewoksdata-0.2.7/src/ewoksdata/data/hdf5/dataset_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)      474 2023-05-30 11:03:10.000000 ewoksdata-0.2.7/src/ewoksdata/data/hdf5/types.py
+-rw-rw-rw-   0 root         (0) root         (0)     3065 2023-05-30 11:03:10.000000 ewoksdata-0.2.7/src/ewoksdata/data/nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)      619 2023-05-30 11:03:10.000000 ewoksdata-0.2.7/src/ewoksdata/data/url.py
+-rw-rw-rw-   0 root         (0) root         (0)      722 2023-05-30 11:03:10.000000 ewoksdata-0.2.7/src/ewoksdata/data/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:06:15.000000 ewoksdata-0.2.7/src/ewoksdata/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 13:06:09.000000 ewoksdata-0.2.7/src/ewoksdata/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      508 2023-05-30 11:03:10.000000 ewoksdata-0.2.7/src/ewoksdata/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:06:15.000000 ewoksdata-0.2.7/src/ewoksdata/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-05-30 11:03:10.000000 ewoksdata-0.2.7/src/ewoksdata/tests/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3771 2023-05-30 11:03:10.000000 ewoksdata-0.2.7/src/ewoksdata/tests/data/bliss_scans.py
+-rw-rw-rw-   0 root         (0) root         (0)     1600 2023-05-30 11:03:10.000000 ewoksdata-0.2.7/src/ewoksdata/tests/test_data_bliss.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-05-30 11:03:10.000000 ewoksdata-0.2.7/src/ewoksdata/tests/test_data_hdf5.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2023-05-30 11:03:10.000000 ewoksdata-0.2.7/src/ewoksdata/tests/test_data_nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)     4200 2023-05-30 12:59:48.000000 ewoksdata-0.2.7/src/ewoksdata/tests/test_dataset_writer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:06:15.000000 ewoksdata-0.2.7/src/ewoksdata.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-05-30 13:06:15.000000 ewoksdata-0.2.7/src/ewoksdata.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      850 2023-05-30 13:06:15.000000 ewoksdata-0.2.7/src/ewoksdata.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 13:06:15.000000 ewoksdata-0.2.7/src/ewoksdata.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      207 2023-05-30 13:06:15.000000 ewoksdata-0.2.7/src/ewoksdata.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-30 13:06:15.000000 ewoksdata-0.2.7/src/ewoksdata.egg-info/top_level.txt
```

### Comparing `ewoksdata-0.2.6/LICENSE.md` & `ewoksdata-0.2.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.6/PKG-INFO` & `ewoksdata-0.2.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksdata
-Version: 0.2.6
+Version: 0.2.7
 Summary: Ewoks tasks for data access
 Home-page: https://gitlab.esrf.fr/workflow/ewoksapps/ewoksdata/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoksapps/ewoksdata/
 Project-URL: Documentation, https://ewoksdata.readthedocs.io
```

### Comparing `ewoksdata-0.2.6/setup.cfg` & `ewoksdata-0.2.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.6/src/ewoksdata/data/bliss.py` & `ewoksdata-0.2.7/src/ewoksdata/data/bliss.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,17 +185,20 @@
             if first_lima_acq_nb != current_lima_acq_nb:
                 logger.warning("lima is already acquiring the next scan")
                 continue
             try:
                 data = list(dataview)
             except ImageNotSaved:
                 logger.warning(
-                    "cannot read lima data from file because it is not saving"
+                    "cannot read lima data from file because images are not being saved"
                 )
                 continue
+            except Exception as e:
+                logger.warning("cannot read lima data (%s)", str(e))
+                continue
             indices[name] += len(data)
             buffers[name].extend(data)
         elif node.type == "channel":
             name = node.db_name.split(":")[-1]
             if name not in counter_names:
                 continue
             if event_data:
```

### Comparing `ewoksdata-0.2.6/src/ewoksdata/data/hdf5/__init__.py` & `ewoksdata-0.2.7/src/ewoksdata/data/hdf5/__init__.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.6/src/ewoksdata/data/hdf5/config.py` & `ewoksdata-0.2.7/src/ewoksdata/data/hdf5/config.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.6/src/ewoksdata/data/nexus.py` & `ewoksdata-0.2.7/src/ewoksdata/data/nexus.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.6/src/ewoksdata/data/url.py` & `ewoksdata-0.2.7/src/ewoksdata/data/url.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.6/src/ewoksdata/data/utils.py` & `ewoksdata-0.2.7/src/ewoksdata/data/utils.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.6/src/ewoksdata/tests/data/bliss_scans.py` & `ewoksdata-0.2.7/src/ewoksdata/tests/data/bliss_scans.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import os
 from datetime import datetime
+from pathlib import Path
+from typing import Tuple
 import numpy
 import h5py
 
 
 __all__ = ["save_bliss_scan"]
 
 
 def save_bliss_scan(
-    tmpdir,
-    image,
-    npoints_per_file,
-    npoints,
-    scannr,
-    subscannr=1,
-    sequence="add",
-    lima_names=("p3",),
-    counter_names=("diode1", "diode2"),
-):
-    dataset_filename = tmpdir / "sample_dataset.5"
+    tmpdir: Path,
+    image: numpy.ndarray,
+    npoints_per_file: int,
+    npoints: int,
+    scannr: int,
+    subscannr: int = 1,
+    sequence: str = "add",
+    lima_names: Tuple[str, ...] = ("p3",),
+    counter_names: Tuple[str, ...] = ("diode1", "diode2"),
+) -> Path:
+    dataset_filename = tmpdir / "sample_dataset.h5"
     lima_dirname = tmpdir / f"scan{scannr:04d}"
     lima_dirname.mkdir()
     with h5py.File(str(dataset_filename), mode="w") as root:
         root.attrs["NX_class"] = "NXroot"
         root.attrs["creator"] = "bliss"
         scan = root.create_group(f"{scannr}.{subscannr}")
         scan.attrs["NX_class"] = "NXentry"
@@ -45,22 +47,29 @@
                 lima_dirname,
                 scannr,
                 sequence,
             )
     return dataset_filename
 
 
-def _save_counter(scan, name, npoints):
+def _save_counter(scan: h5py.Group, name: str, npoints: int) -> None:
     diode = _add_detector(scan, name)
     diode["data"] = numpy.arange(npoints)
 
 
 def _save_lima(
-    scan, name, image, npoints, npoints_per_file, lima_dirname, scannr, sequence
-):
+    scan: h5py.Group,
+    name: str,
+    image: numpy.ndarray,
+    npoints: int,
+    npoints_per_file: int,
+    lima_dirname: Path,
+    scannr: int,
+    sequence: str,
+) -> None:
     tot_shape = (npoints,) + image.shape
     lima_shape = (npoints_per_file,) + image.shape
     nlima = npoints // npoints_per_file + bool(npoints % npoints_per_file)
     lima_dtype = float
     layout = h5py.VirtualLayout(tot_shape, dtype=lima_dtype)
     for i in range(nlima):
         with h5py.File(str(lima_dirname / f"{name}_{i}.h5"), mode="w") as limaroot:
@@ -91,12 +100,12 @@
             vsource = h5py.VirtualSource(spath, sdset, shape=sshape, dtype=lima_dtype)
 
             layout[i0:i1] = vsource
     detector = _add_detector(scan, name)
     detector.create_virtual_dataset("data", layout, fillvalue=numpy.nan)
 
 
-def _add_detector(scan, name):
+def _add_detector(scan: h5py.Group, name: str) -> h5py.Group:
     grp = scan["instrument"].create_group(name)
     grp.attrs["NX_class"] = "NXdetector"
     scan["measurement"][name] = h5py.SoftLink(f"{grp.name}/data")
     return grp
```

### Comparing `ewoksdata-0.2.6/src/ewoksdata/tests/test_data_bliss.py` & `ewoksdata-0.2.7/src/ewoksdata/tests/test_data_bliss.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.6/src/ewoksdata/tests/test_data_nexus.py` & `ewoksdata-0.2.7/src/ewoksdata/tests/test_data_nexus.py`

 * *Files identical despite different names*

### Comparing `ewoksdata-0.2.6/src/ewoksdata.egg-info/PKG-INFO` & `ewoksdata-0.2.7/src/ewoksdata.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ewoksdata
-Version: 0.2.6
+Version: 0.2.7
 Summary: Ewoks tasks for data access
 Home-page: https://gitlab.esrf.fr/workflow/ewoksapps/ewoksdata/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoksapps/ewoksdata/
 Project-URL: Documentation, https://ewoksdata.readthedocs.io
```

### Comparing `ewoksdata-0.2.6/src/ewoksdata.egg-info/SOURCES.txt` & `ewoksdata-0.2.7/src/ewoksdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

