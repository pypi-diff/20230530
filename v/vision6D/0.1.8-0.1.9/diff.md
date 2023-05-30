# Comparing `tmp/vision6D-0.1.8.tar.gz` & `tmp/vision6D-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vision6D-0.1.8.tar", last modified: Tue May 30 19:19:01 2023, max compression
+gzip compressed data, was "dist\vision6D-0.1.9.tar", last modified: Tue May 30 19:22:29 2023, max compression
```

## Comparing `vision6D-0.1.8.tar` & `vision6D-0.1.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 19:19:01.308982 vision6D-0.1.8/
--rw-rw-rw-   0        0        0     1086 2023-01-03 15:55:06.000000 vision6D-0.1.8/LICENSE
--rw-rw-rw-   0        0        0       33 2023-05-27 00:07:11.000000 vision6D-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1601 2023-05-30 19:19:01.309982 vision6D-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      918 2023-05-28 01:21:42.000000 vision6D-0.1.8/README.md
--rw-rw-rw-   0        0        0      406 2023-05-30 19:17:57.000000 vision6D-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0     1995 2023-05-30 19:19:01.312981 vision6D-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      283 2023-05-30 19:18:07.000000 vision6D-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 19:19:01.234979 vision6D-0.1.8/test/
--rw-rw-rw-   0        0        0    21974 2023-05-17 18:41:02.000000 vision6D-0.1.8/test/test_create_dataset.py
--rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.1.8/test/test_projection.py
-drwxrwxrwx   0        0        0        0 2023-05-30 19:19:01.264979 vision6D-0.1.8/vision6D/
--rw-rw-rw-   0        0        0    51597 2023-05-29 23:53:36.000000 vision6D-0.1.8/vision6D/GUI.py
--rw-rw-rw-   0        0        0      939 2023-05-28 01:21:42.000000 vision6D-0.1.8/vision6D/__init__.py
--rw-rw-rw-   0        0        0       58 2023-05-30 18:56:26.000000 vision6D-0.1.8/vision6D/__main__.py
--rw-rw-rw-   0        0        0    19331 2023-05-14 22:36:01.000000 vision6D-0.1.8/vision6D/app.py
--rw-rw-rw-   0        0        0    12369 2023-05-28 01:21:42.000000 vision6D-0.1.8/vision6D/config.py
-drwxrwxrwx   0        0        0        0 2023-05-30 19:19:01.305984 vision6D-0.1.8/vision6D/data/
--rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.1.8/vision6D/data/ossiclesCoordinateMapping.json
--rw-rw-rw-   0        0        0   335336 2023-05-14 22:36:02.000000 vision6D-0.1.8/vision6D/data/ossiclesCoordinateMappingv1.json
--rw-rw-rw-   0        0        0    12109 2023-05-15 22:13:50.000000 vision6D-0.1.8/vision6D/data/style.qss
--rw-rw-rw-   0        0        0    22897 2023-05-14 22:36:02.000000 vision6D-0.1.8/vision6D/interface.py
--rw-rw-rw-   0        0        0    26253 2023-05-29 23:38:16.000000 vision6D-0.1.8/vision6D/interface_gui.py
--rw-rw-rw-   0        0        0    33713 2023-05-14 22:36:02.000000 vision6D-0.1.8/vision6D/mainwindow.py
--rw-rw-rw-   0        0        0    14068 2023-05-15 23:19:36.000000 vision6D-0.1.8/vision6D/run_gui.py
--rw-rw-rw-   0        0        0      197 2023-05-14 22:53:44.000000 vision6D-0.1.8/vision6D/run_interface.py
--rw-rw-rw-   0        0        0    14911 2023-05-14 22:36:02.000000 vision6D-0.1.8/vision6D/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-30 19:19:01.293978 vision6D-0.1.8/vision6D.egg-info/
--rw-rw-rw-   0        0        0     1601 2023-05-30 19:19:01.000000 vision6D-0.1.8/vision6D.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      653 2023-05-30 19:19:01.000000 vision6D-0.1.8/vision6D.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 19:19:01.000000 vision6D-0.1.8/vision6D.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-05-30 19:19:01.000000 vision6D-0.1.8/vision6D.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      164 2023-05-30 19:19:01.000000 vision6D-0.1.8/vision6D.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-30 19:19:01.000000 vision6D-0.1.8/vision6D.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 19:22:29.532943 vision6D-0.1.9/
+-rw-rw-rw-   0        0        0     1086 2023-01-03 15:55:06.000000 vision6D-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0       33 2023-05-27 00:07:11.000000 vision6D-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1541 2023-05-30 19:22:29.532943 vision6D-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      858 2023-05-30 19:21:58.000000 vision6D-0.1.9/README.md
+-rw-rw-rw-   0        0        0      406 2023-05-30 19:17:57.000000 vision6D-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0     1995 2023-05-30 19:22:29.538948 vision6D-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      274 2023-05-30 19:21:31.000000 vision6D-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 19:22:29.440949 vision6D-0.1.9/test/
+-rw-rw-rw-   0        0        0    21974 2023-05-17 18:41:02.000000 vision6D-0.1.9/test/test_create_dataset.py
+-rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.1.9/test/test_projection.py
+drwxrwxrwx   0        0        0        0 2023-05-30 19:22:29.476944 vision6D-0.1.9/vision6D/
+-rw-rw-rw-   0        0        0    51597 2023-05-29 23:53:36.000000 vision6D-0.1.9/vision6D/GUI.py
+-rw-rw-rw-   0        0        0      939 2023-05-28 01:21:42.000000 vision6D-0.1.9/vision6D/__init__.py
+-rw-rw-rw-   0        0        0       58 2023-05-30 18:56:26.000000 vision6D-0.1.9/vision6D/__main__.py
+-rw-rw-rw-   0        0        0    19331 2023-05-14 22:36:01.000000 vision6D-0.1.9/vision6D/app.py
+-rw-rw-rw-   0        0        0    12369 2023-05-28 01:21:42.000000 vision6D-0.1.9/vision6D/config.py
+drwxrwxrwx   0        0        0        0 2023-05-30 19:22:29.528946 vision6D-0.1.9/vision6D/data/
+-rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.1.9/vision6D/data/ossiclesCoordinateMapping.json
+-rw-rw-rw-   0        0        0   335336 2023-05-14 22:36:02.000000 vision6D-0.1.9/vision6D/data/ossiclesCoordinateMappingv1.json
+-rw-rw-rw-   0        0        0    12109 2023-05-15 22:13:50.000000 vision6D-0.1.9/vision6D/data/style.qss
+-rw-rw-rw-   0        0        0    22897 2023-05-14 22:36:02.000000 vision6D-0.1.9/vision6D/interface.py
+-rw-rw-rw-   0        0        0    26253 2023-05-29 23:38:16.000000 vision6D-0.1.9/vision6D/interface_gui.py
+-rw-rw-rw-   0        0        0    33713 2023-05-14 22:36:02.000000 vision6D-0.1.9/vision6D/mainwindow.py
+-rw-rw-rw-   0        0        0    14068 2023-05-15 23:19:36.000000 vision6D-0.1.9/vision6D/run_gui.py
+-rw-rw-rw-   0        0        0      197 2023-05-14 22:53:44.000000 vision6D-0.1.9/vision6D/run_interface.py
+-rw-rw-rw-   0        0        0    14911 2023-05-14 22:36:02.000000 vision6D-0.1.9/vision6D/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-30 19:22:29.518943 vision6D-0.1.9/vision6D.egg-info/
+-rw-rw-rw-   0        0        0     1541 2023-05-30 19:22:29.000000 vision6D-0.1.9/vision6D.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      653 2023-05-30 19:22:29.000000 vision6D-0.1.9/vision6D.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 19:22:29.000000 vision6D-0.1.9/vision6D.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 19:22:29.000000 vision6D-0.1.9/vision6D.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      164 2023-05-30 19:22:29.000000 vision6D-0.1.9/vision6D.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-30 19:22:29.000000 vision6D-0.1.9/vision6D.egg-info/top_level.txt
```

### Comparing `vision6D-0.1.8/LICENSE` & `vision6D-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.8/PKG-INFO` & `vision6D-0.1.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.1.8
+Version: 0.1.9
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzky/vision6D
 License: GNU GENERAL Public License
 Project-URL: Bug Tracker, https://github.com/ykzzky/vision6D/issues
 Keywords: 6D poes estimation,registration,segmentation
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -28,19 +28,16 @@
 Install the package using pip:
 
 ```shell
 pip install vision6D
 ```
 
 ## Usage
-```python
-import vision6D as vis
-
-# Load the interactive window
-vis.exe()
+```bash
+vision6D
 ```
 
 Usage example shown below to register computer monitor model to an image
 
 ![example](https://github.com/ykzzyk/vision6D/assets/55161270/b6e4b0f6-ac51-416a-a63d-0aa0de2793d0)
 
 ## License
```

### Comparing `vision6D-0.1.8/README.md` & `vision6D-0.1.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -10,19 +10,16 @@
 Install the package using pip:
 
 ```shell
 pip install vision6D
 ```
 
 ## Usage
-```python
-import vision6D as vis
-
-# Load the interactive window
-vis.exe()
+```bash
+vision6D
 ```
 
 Usage example shown below to register computer monitor model to an image
 
 ![example](https://github.com/ykzzyk/vision6D/assets/55161270/b6e4b0f6-ac51-416a-a63d-0aa0de2793d0)
 
 ## License
```

### Comparing `vision6D-0.1.8/setup.cfg` & `vision6D-0.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6973 696f 6e36 440d 0a76 6572   = vision6D..ver
-00000020: 7369 6f6e 203d 2030 2e31 2e38 0d0a 7572  sion = 0.1.8..ur
+00000020: 7369 6f6e 203d 2030 2e31 2e39 0d0a 7572  sion = 0.1.9..ur
 00000030: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
 00000040: 7562 2e63 6f6d 2f79 6b7a 7a6b 792f 7669  ub.com/ykzzky/vi
 00000050: 7369 6f6e 3644 0d0a 6465 7363 7269 7074  sion6D..descript
 00000060: 696f 6e20 3d20 7669 7369 6f6e 3644 3a20  ion = vision6D: 
 00000070: 4120 746f 6f6c 2066 6f72 2036 4420 706f  A tool for 6D po
 00000080: 7365 2065 7374 696d 6174 696f 6e20 616e  se estimation an
 00000090: 6e6f 7461 7469 6f6e 0d0a 6c6f 6e67 5f64  notation..long_d
```

### Comparing `vision6D-0.1.8/test/test_create_dataset.py` & `vision6D-0.1.9/test/test_create_dataset.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.8/test/test_projection.py` & `vision6D-0.1.9/test/test_projection.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.8/vision6D/GUI.py` & `vision6D-0.1.9/vision6D/GUI.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.8/vision6D/__init__.py` & `vision6D-0.1.9/vision6D/__init__.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.8/vision6D/app.py` & `vision6D-0.1.9/vision6D/app.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.8/vision6D/config.py` & `vision6D-0.1.9/vision6D/config.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.8/vision6D/data/ossiclesCoordinateMapping.json` & `vision6D-0.1.9/vision6D/data/ossiclesCoordinateMapping.json`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.8/vision6D/data/ossiclesCoordinateMappingv1.json` & `vision6D-0.1.9/vision6D/data/ossiclesCoordinateMappingv1.json`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.8/vision6D/data/style.qss` & `vision6D-0.1.9/vision6D/data/style.qss`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.8/vision6D/interface.py` & `vision6D-0.1.9/vision6D/interface.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.8/vision6D/interface_gui.py` & `vision6D-0.1.9/vision6D/interface_gui.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.8/vision6D/mainwindow.py` & `vision6D-0.1.9/vision6D/mainwindow.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.8/vision6D/run_gui.py` & `vision6D-0.1.9/vision6D/run_gui.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.8/vision6D/utils.py` & `vision6D-0.1.9/vision6D/utils.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.8/vision6D.egg-info/PKG-INFO` & `vision6D-0.1.9/vision6D.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.1.8
+Version: 0.1.9
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzky/vision6D
 License: GNU GENERAL Public License
 Project-URL: Bug Tracker, https://github.com/ykzzky/vision6D/issues
 Keywords: 6D poes estimation,registration,segmentation
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -28,19 +28,16 @@
 Install the package using pip:
 
 ```shell
 pip install vision6D
 ```
 
 ## Usage
-```python
-import vision6D as vis
-
-# Load the interactive window
-vis.exe()
+```bash
+vision6D
 ```
 
 Usage example shown below to register computer monitor model to an image
 
 ![example](https://github.com/ykzzyk/vision6D/assets/55161270/b6e4b0f6-ac51-416a-a63d-0aa0de2793d0)
 
 ## License
```

### Comparing `vision6D-0.1.8/vision6D.egg-info/SOURCES.txt` & `vision6D-0.1.9/vision6D.egg-info/SOURCES.txt`

 * *Files identical despite different names*

