# Comparing `tmp/pyquet-0.1.3.tar.gz` & `tmp/pyquet-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\github\pyquet\dist\.tmp-vk7zov7t\pyquet-0.1.3.tar", last modified: Tue May 30 08:12:53 2023, max compression
+gzip compressed data, was "C:\github\pyquet\dist\.tmp-3fj_iyet\pyquet-0.1.4.tar", last modified: Tue May 30 08:18:36 2023, max compression
```

## Comparing `pyquet-0.1.3.tar` & `pyquet-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 08:12:53.000000 pyquet-0.1.3/
--rw-rw-rw-   0        0        0     1086 2023-05-30 07:37:22.000000 pyquet-0.1.3/LICENSE
--rw-rw-rw-   0        0        0      546 2023-05-30 08:12:53.000000 pyquet-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       51 2023-05-30 07:37:22.000000 pyquet-0.1.3/README.md
--rw-rw-rw-   0        0        0      104 2023-05-30 07:42:55.000000 pyquet-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0      674 2023-05-30 08:12:53.000000 pyquet-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-30 08:12:53.000000 pyquet-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-30 08:12:53.000000 pyquet-0.1.3/src/pyquet.egg-info/
--rw-rw-rw-   0        0        0      546 2023-05-30 08:12:53.000000 pyquet-0.1.3/src/pyquet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-05-30 08:12:53.000000 pyquet-0.1.3/src/pyquet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 08:12:53.000000 pyquet-0.1.3/src/pyquet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-30 08:12:53.000000 pyquet-0.1.3/src/pyquet.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 08:12:53.000000 pyquet-0.1.3/src/pyquet.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-30 08:12:53.000000 pyquet-0.1.3/tests/
--rw-rw-rw-   0        0        0     2071 2023-05-30 08:10:41.000000 pyquet-0.1.3/tests/test_reader.py
+drwxrwxrwx   0        0        0        0 2023-05-30 08:18:36.000000 pyquet-0.1.4/
+-rw-rw-rw-   0        0        0     1086 2023-05-30 07:37:22.000000 pyquet-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0      546 2023-05-30 08:18:36.000000 pyquet-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       51 2023-05-30 07:37:22.000000 pyquet-0.1.4/README.md
+-rw-rw-rw-   0        0        0      104 2023-05-30 07:42:55.000000 pyquet-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0      674 2023-05-30 08:18:36.000000 pyquet-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-30 08:18:36.000000 pyquet-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-30 08:18:36.000000 pyquet-0.1.4/src/pyquet/
+-rw-rw-rw-   0        0        0        0 2023-05-30 08:16:35.000000 pyquet-0.1.4/src/pyquet/__init__.py
+-rw-rw-rw-   0        0        0      628 2023-05-30 07:38:36.000000 pyquet-0.1.4/src/pyquet/common.py
+-rw-rw-rw-   0        0        0     6399 2023-05-30 08:18:01.000000 pyquet-0.1.4/src/pyquet/generator.py
+-rw-rw-rw-   0        0        0     2176 2023-05-30 08:18:01.000000 pyquet-0.1.4/src/pyquet/schemas.py
+drwxrwxrwx   0        0        0        0 2023-05-30 08:18:36.000000 pyquet-0.1.4/src/pyquet.egg-info/
+-rw-rw-rw-   0        0        0      546 2023-05-30 08:18:36.000000 pyquet-0.1.4/src/pyquet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      322 2023-05-30 08:18:36.000000 pyquet-0.1.4/src/pyquet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 08:18:36.000000 pyquet-0.1.4/src/pyquet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-30 08:18:36.000000 pyquet-0.1.4/src/pyquet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-30 08:18:36.000000 pyquet-0.1.4/src/pyquet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 08:18:36.000000 pyquet-0.1.4/tests/
+-rw-rw-rw-   0        0        0     2078 2023-05-30 08:17:11.000000 pyquet-0.1.4/tests/test_reader.py
```

### Comparing `pyquet-0.1.3/LICENSE` & `pyquet-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyquet-0.1.3/PKG-INFO` & `pyquet-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyquet
-Version: 0.1.3
+Version: 0.1.4
 Summary: Text comparator UI
 Home-page: https://github.com/rmugicag/pyquet
 Author: Ricardo Mugica
 Author-email: rmugicag@gmail.com
 Project-URL: Bug Tracker, https://github.com/rmugicag/pyquet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyquet-0.1.3/setup.cfg` & `pyquet-0.1.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7971 7565 740d 0a76 6572 7369   = pyquet..versi
-00000020: 6f6e 203d 2030 2e31 2e33 0d0a 6175 7468  on = 0.1.3..auth
+00000020: 6f6e 203d 2030 2e31 2e34 0d0a 6175 7468  on = 0.1.4..auth
 00000030: 6f72 203d 2052 6963 6172 646f 204d 7567  or = Ricardo Mug
 00000040: 6963 610d 0a61 7574 686f 725f 656d 6169  ica..author_emai
 00000050: 6c20 3d20 726d 7567 6963 6167 4067 6d61  l = rmugicag@gma
 00000060: 696c 2e63 6f6d 0d0a 6465 7363 7269 7074  il.com..descript
 00000070: 696f 6e20 3d20 5465 7874 2063 6f6d 7061  ion = Text compa
 00000080: 7261 746f 7220 5549 0d0a 6c6f 6e67 5f64  rator UI..long_d
 00000090: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
```

### Comparing `pyquet-0.1.3/src/pyquet.egg-info/PKG-INFO` & `pyquet-0.1.4/src/pyquet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyquet
-Version: 0.1.3
+Version: 0.1.4
 Summary: Text comparator UI
 Home-page: https://github.com/rmugicag/pyquet
 Author: Ricardo Mugica
 Author-email: rmugicag@gmail.com
 Project-URL: Bug Tracker, https://github.com/rmugicag/pyquet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyquet-0.1.3/tests/test_reader.py` & `pyquet-0.1.4/tests/test_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import unittest
-from src.schemas import Reader
+from src.pyquet.schemas import Reader
 
 
 class ReaderTestCase(unittest.TestCase):
     def setUp(self):
         self.schemas_path = os.path.join(os.path.dirname(__file__), "test_data", "schemas")
         self.schemas_path_without_schemas = os.path.join(self.schemas_path, "data")
         self.schema_1 = os.path.join(self.schemas_path, 'schema_1.json')
```

