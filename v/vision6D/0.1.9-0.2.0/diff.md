# Comparing `tmp/vision6D-0.1.9.tar.gz` & `tmp/vision6D-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vision6D-0.1.9.tar", last modified: Tue May 30 19:22:29 2023, max compression
+gzip compressed data, was "vision6D-0.2.0.tar", last modified: Tue May 30 19:32:55 2023, max compression
```

## Comparing `vision6D-0.1.9.tar` & `vision6D-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 19:22:29.532943 vision6D-0.1.9/
--rw-rw-rw-   0        0        0     1086 2023-01-03 15:55:06.000000 vision6D-0.1.9/LICENSE
--rw-rw-rw-   0        0        0       33 2023-05-27 00:07:11.000000 vision6D-0.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0     1541 2023-05-30 19:22:29.532943 vision6D-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0      858 2023-05-30 19:21:58.000000 vision6D-0.1.9/README.md
--rw-rw-rw-   0        0        0      406 2023-05-30 19:17:57.000000 vision6D-0.1.9/pyproject.toml
--rw-rw-rw-   0        0        0     1995 2023-05-30 19:22:29.538948 vision6D-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      274 2023-05-30 19:21:31.000000 vision6D-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 19:22:29.440949 vision6D-0.1.9/test/
--rw-rw-rw-   0        0        0    21974 2023-05-17 18:41:02.000000 vision6D-0.1.9/test/test_create_dataset.py
--rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.1.9/test/test_projection.py
-drwxrwxrwx   0        0        0        0 2023-05-30 19:22:29.476944 vision6D-0.1.9/vision6D/
--rw-rw-rw-   0        0        0    51597 2023-05-29 23:53:36.000000 vision6D-0.1.9/vision6D/GUI.py
--rw-rw-rw-   0        0        0      939 2023-05-28 01:21:42.000000 vision6D-0.1.9/vision6D/__init__.py
--rw-rw-rw-   0        0        0       58 2023-05-30 18:56:26.000000 vision6D-0.1.9/vision6D/__main__.py
--rw-rw-rw-   0        0        0    19331 2023-05-14 22:36:01.000000 vision6D-0.1.9/vision6D/app.py
--rw-rw-rw-   0        0        0    12369 2023-05-28 01:21:42.000000 vision6D-0.1.9/vision6D/config.py
-drwxrwxrwx   0        0        0        0 2023-05-30 19:22:29.528946 vision6D-0.1.9/vision6D/data/
--rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.1.9/vision6D/data/ossiclesCoordinateMapping.json
--rw-rw-rw-   0        0        0   335336 2023-05-14 22:36:02.000000 vision6D-0.1.9/vision6D/data/ossiclesCoordinateMappingv1.json
--rw-rw-rw-   0        0        0    12109 2023-05-15 22:13:50.000000 vision6D-0.1.9/vision6D/data/style.qss
--rw-rw-rw-   0        0        0    22897 2023-05-14 22:36:02.000000 vision6D-0.1.9/vision6D/interface.py
--rw-rw-rw-   0        0        0    26253 2023-05-29 23:38:16.000000 vision6D-0.1.9/vision6D/interface_gui.py
--rw-rw-rw-   0        0        0    33713 2023-05-14 22:36:02.000000 vision6D-0.1.9/vision6D/mainwindow.py
--rw-rw-rw-   0        0        0    14068 2023-05-15 23:19:36.000000 vision6D-0.1.9/vision6D/run_gui.py
--rw-rw-rw-   0        0        0      197 2023-05-14 22:53:44.000000 vision6D-0.1.9/vision6D/run_interface.py
--rw-rw-rw-   0        0        0    14911 2023-05-14 22:36:02.000000 vision6D-0.1.9/vision6D/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-30 19:22:29.518943 vision6D-0.1.9/vision6D.egg-info/
--rw-rw-rw-   0        0        0     1541 2023-05-30 19:22:29.000000 vision6D-0.1.9/vision6D.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      653 2023-05-30 19:22:29.000000 vision6D-0.1.9/vision6D.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 19:22:29.000000 vision6D-0.1.9/vision6D.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 19:22:29.000000 vision6D-0.1.9/vision6D.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      164 2023-05-30 19:22:29.000000 vision6D-0.1.9/vision6D.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-30 19:22:29.000000 vision6D-0.1.9/vision6D.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 19:32:55.380729 vision6D-0.2.0/
+-rw-rw-rw-   0        0        0     1086 2023-01-03 15:55:06.000000 vision6D-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0       33 2023-05-27 00:07:11.000000 vision6D-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1545 2023-05-30 19:32:55.381729 vision6D-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      858 2023-05-30 19:21:58.000000 vision6D-0.2.0/README.md
+-rw-rw-rw-   0        0        0      406 2023-05-30 19:17:57.000000 vision6D-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1923 2023-05-30 19:32:55.387726 vision6D-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      282 2023-05-30 19:29:49.000000 vision6D-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 19:32:55.153591 vision6D-0.2.0/test/
+-rw-rw-rw-   0        0        0    21974 2023-05-17 18:41:02.000000 vision6D-0.2.0/test/test_create_dataset.py
+-rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.2.0/test/test_projection.py
+drwxrwxrwx   0        0        0        0 2023-05-30 19:32:55.235593 vision6D-0.2.0/vision6D/
+-rw-rw-rw-   0        0        0    51597 2023-05-29 23:53:36.000000 vision6D-0.2.0/vision6D/GUI.py
+-rw-rw-rw-   0        0        0      913 2023-05-30 19:29:28.000000 vision6D-0.2.0/vision6D/__init__.py
+-rw-rw-rw-   0        0        0    19331 2023-05-14 22:36:01.000000 vision6D-0.2.0/vision6D/app.py
+-rw-rw-rw-   0        0        0    12369 2023-05-28 01:21:42.000000 vision6D-0.2.0/vision6D/config.py
+drwxrwxrwx   0        0        0        0 2023-05-30 19:32:55.376729 vision6D-0.2.0/vision6D/data/
+-rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.2.0/vision6D/data/ossiclesCoordinateMapping.json
+-rw-rw-rw-   0        0        0   335336 2023-05-14 22:36:02.000000 vision6D-0.2.0/vision6D/data/ossiclesCoordinateMappingv1.json
+-rw-rw-rw-   0        0        0    12109 2023-05-15 22:13:50.000000 vision6D-0.2.0/vision6D/data/style.qss
+-rw-rw-rw-   0        0        0    22897 2023-05-14 22:36:02.000000 vision6D-0.2.0/vision6D/interface.py
+-rw-rw-rw-   0        0        0    26253 2023-05-29 23:38:16.000000 vision6D-0.2.0/vision6D/interface_gui.py
+-rw-rw-rw-   0        0        0    33713 2023-05-14 22:36:02.000000 vision6D-0.2.0/vision6D/mainwindow.py
+-rw-rw-rw-   0        0        0    14068 2023-05-15 23:19:36.000000 vision6D-0.2.0/vision6D/run_gui.py
+-rw-rw-rw-   0        0        0      197 2023-05-14 22:53:44.000000 vision6D-0.2.0/vision6D/run_interface.py
+-rw-rw-rw-   0        0        0    14911 2023-05-14 22:36:02.000000 vision6D-0.2.0/vision6D/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-30 19:32:55.304720 vision6D-0.2.0/vision6D.egg-info/
+-rw-rw-rw-   0        0        0     1545 2023-05-30 19:32:54.000000 vision6D-0.2.0/vision6D.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      632 2023-05-30 19:32:55.000000 vision6D-0.2.0/vision6D.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 19:32:54.000000 vision6D-0.2.0/vision6D.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-30 19:32:54.000000 vision6D-0.2.0/vision6D.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      164 2023-05-30 19:32:54.000000 vision6D-0.2.0/vision6D.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-30 19:32:54.000000 vision6D-0.2.0/vision6D.egg-info/top_level.txt
```

### Comparing `vision6D-0.1.9/LICENSE` & `vision6D-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.9/PKG-INFO` & `vision6D-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.1.9
+Version: 0.2.0
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzky/vision6D
 License: GNU GENERAL Public License
 Project-URL: Bug Tracker, https://github.com/ykzzky/vision6D/issues
 Keywords: 6D poes estimation,registration,segmentation
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -41,7 +41,9 @@
 ![example](https://github.com/ykzzyk/vision6D/assets/55161270/b6e4b0f6-ac51-416a-a63d-0aa0de2793d0)
 
 ## License
 This project is licensed under the MIT License.
 
 ## Contact
 If you have further question, you can either open a issue on GitHub or directly connect me via email yike.zhang@vanderbilt.edu
+
+
```

### Comparing `vision6D-0.1.9/README.md` & `vision6D-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.9/setup.cfg` & `vision6D-0.2.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6973 696f 6e36 440d 0a76 6572   = vision6D..ver
-00000020: 7369 6f6e 203d 2030 2e31 2e39 0d0a 7572  sion = 0.1.9..ur
+00000020: 7369 6f6e 203d 2030 2e32 2e30 0d0a 7572  sion = 0.2.0..ur
 00000030: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
 00000040: 7562 2e63 6f6d 2f79 6b7a 7a6b 792f 7669  ub.com/ykzzky/vi
 00000050: 7369 6f6e 3644 0d0a 6465 7363 7269 7074  sion6D..descript
 00000060: 696f 6e20 3d20 7669 7369 6f6e 3644 3a20  ion = vision6D: 
 00000070: 4120 746f 6f6c 2066 6f72 2036 4420 706f  A tool for 6D po
 00000080: 7365 2065 7374 696d 6174 696f 6e20 616e  se estimation an
 00000090: 6e6f 7461 7469 6f6e 0d0a 6c6f 6e67 5f64  notation..long_d
@@ -111,15 +111,11 @@
 000006e0: 7472 7565 0d0a 6469 7361 6c6c 6f77 5f75  true..disallow_u
 000006f0: 6e74 7970 6564 5f64 6566 7320 3d20 7472  ntyped_defs = tr
 00000700: 7565 0d0a 6967 6e6f 7265 5f6d 6973 7369  ue..ignore_missi
 00000710: 6e67 5f69 6d70 6f72 7473 203d 2074 7275  ng_imports = tru
 00000720: 650d 0a77 6172 6e5f 756e 7573 6564 5f69  e..warn_unused_i
 00000730: 676e 6f72 6573 203d 2074 7275 650d 0a77  gnores = true..w
 00000740: 6172 6e5f 7265 7475 726e 5f61 6e79 203d  arn_return_any =
-00000750: 2074 7275 650d 0a0d 0a5b 6f70 7469 6f6e   true....[option
-00000760: 732e 656e 7472 795f 706f 696e 7473 5d0d  s.entry_points].
-00000770: 0a63 6f6e 736f 6c65 5f73 6372 6970 7473  .console_scripts
-00000780: 203d 200d 0a09 7669 7369 6f6e 3644 203d   = ...vision6D =
-00000790: 2076 6973 696f 6e36 443a 6578 650d 0a0d   vision6D:exe...
-000007a0: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
-000007b0: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
-000007c0: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
+00000750: 2074 7275 650d 0a0d 0a5b 6567 675f 696e   true....[egg_in
+00000760: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
+00000770: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
+00000780: 0a0d 0a                                  ...
```

### Comparing `vision6D-0.1.9/test/test_create_dataset.py` & `vision6D-0.2.0/test/test_create_dataset.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.9/test/test_projection.py` & `vision6D-0.2.0/test/test_projection.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.9/vision6D/GUI.py` & `vision6D-0.2.0/vision6D/GUI.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.9/vision6D/__init__.py` & `vision6D-0.2.0/vision6D/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,9 +28,8 @@
 
 # Setup the logging configuration
 logging.config.dictConfig(LOGGING_CONFIG)
 
 from .app import App
 from .interface import Interface
 from .interface_gui import Interface_GUI
-from . import utils
-from .run_gui import exe
+from . import utils
```

### Comparing `vision6D-0.1.9/vision6D/app.py` & `vision6D-0.2.0/vision6D/app.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.9/vision6D/config.py` & `vision6D-0.2.0/vision6D/config.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.9/vision6D/data/ossiclesCoordinateMapping.json` & `vision6D-0.2.0/vision6D/data/ossiclesCoordinateMapping.json`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.9/vision6D/data/ossiclesCoordinateMappingv1.json` & `vision6D-0.2.0/vision6D/data/ossiclesCoordinateMappingv1.json`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.9/vision6D/data/style.qss` & `vision6D-0.2.0/vision6D/data/style.qss`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.9/vision6D/interface.py` & `vision6D-0.2.0/vision6D/interface.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.9/vision6D/interface_gui.py` & `vision6D-0.2.0/vision6D/interface_gui.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.9/vision6D/mainwindow.py` & `vision6D-0.2.0/vision6D/mainwindow.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.9/vision6D/run_gui.py` & `vision6D-0.2.0/vision6D/run_gui.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.9/vision6D/utils.py` & `vision6D-0.2.0/vision6D/utils.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.9/vision6D.egg-info/PKG-INFO` & `vision6D-0.2.0/vision6D.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.1.9
+Version: 0.2.0
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzky/vision6D
 License: GNU GENERAL Public License
 Project-URL: Bug Tracker, https://github.com/ykzzky/vision6D/issues
 Keywords: 6D poes estimation,registration,segmentation
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -41,7 +41,9 @@
 ![example](https://github.com/ykzzyk/vision6D/assets/55161270/b6e4b0f6-ac51-416a-a63d-0aa0de2793d0)
 
 ## License
 This project is licensed under the MIT License.
 
 ## Contact
 If you have further question, you can either open a issue on GitHub or directly connect me via email yike.zhang@vanderbilt.edu
+
+
```

### Comparing `vision6D-0.1.9/vision6D.egg-info/SOURCES.txt` & `vision6D-0.2.0/vision6D.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 pyproject.toml
 setup.cfg
 setup.py
 test/test_create_dataset.py
 test/test_projection.py
 vision6D/GUI.py
 vision6D/__init__.py
-vision6D/__main__.py
 vision6D/app.py
 vision6D/config.py
 vision6D/interface.py
 vision6D/interface_gui.py
 vision6D/mainwindow.py
 vision6D/run_gui.py
 vision6D/run_interface.py
```

