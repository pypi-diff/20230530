# Comparing `tmp/pyquet-0.1.1.tar.gz` & `tmp/pyquet-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyquet-0.1.1.tar", last modified: Sat May 27 09:34:28 2023, max compression
+gzip compressed data, was "C:\github\pyquet\dist\.tmp-pudo2kc9\pyquet-0.1.2.tar", last modified: Tue May 30 07:57:05 2023, max compression
```

## Comparing `pyquet-0.1.1.tar` & `pyquet-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 09:34:28.878184 pyquet-0.1.1/
--rw-rw-rw-   0        0        0     1086 2023-05-26 12:18:55.000000 pyquet-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      546 2023-05-27 09:34:28.878184 pyquet-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       51 2023-05-26 12:18:55.000000 pyquet-0.1.1/README.md
--rw-rw-rw-   0        0        0      108 2023-05-27 09:31:18.000000 pyquet-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      674 2023-05-27 09:34:28.881680 pyquet-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-27 09:34:28.858672 pyquet-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-27 09:34:28.866173 pyquet-0.1.1/src/pyquet/
--rw-rw-rw-   0        0        0        0 2023-05-26 10:40:59.000000 pyquet-0.1.1/src/pyquet/__init__.py
--rw-rw-rw-   0        0        0      628 2023-05-26 11:30:34.000000 pyquet-0.1.1/src/pyquet/common.py
--rw-rw-rw-   0        0        0     6399 2023-05-27 09:33:39.000000 pyquet-0.1.1/src/pyquet/generator.py
--rw-rw-rw-   0        0        0     2176 2023-05-27 09:33:39.000000 pyquet-0.1.1/src/pyquet/schemas.py
-drwxrwxrwx   0        0        0        0 2023-05-27 09:34:28.876189 pyquet-0.1.1/src/pyquet.egg-info/
--rw-rw-rw-   0        0        0      546 2023-05-27 09:34:28.000000 pyquet-0.1.1/src/pyquet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2023-05-27 09:34:28.000000 pyquet-0.1.1/src/pyquet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 09:34:28.000000 pyquet-0.1.1/src/pyquet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-27 09:34:28.000000 pyquet-0.1.1/src/pyquet.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-27 09:34:28.000000 pyquet-0.1.1/src/pyquet.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-27 09:34:28.877187 pyquet-0.1.1/tests/
--rw-rw-rw-   0        0        0     2078 2023-05-27 09:31:42.000000 pyquet-0.1.1/tests/test_reader.py
+drwxrwxrwx   0        0        0        0 2023-05-30 07:57:05.000000 pyquet-0.1.2/
+-rw-rw-rw-   0        0        0     1086 2023-05-30 07:37:22.000000 pyquet-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      546 2023-05-30 07:57:05.000000 pyquet-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       51 2023-05-30 07:37:22.000000 pyquet-0.1.2/README.md
+-rw-rw-rw-   0        0        0      104 2023-05-30 07:42:55.000000 pyquet-0.1.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-30 07:57:05.000000 pyquet-0.1.2/pyquet/
+drwxrwxrwx   0        0        0        0 2023-05-30 07:57:05.000000 pyquet-0.1.2/pyquet/pyquet.egg-info/
+-rw-rw-rw-   0        0        0      546 2023-05-30 07:57:05.000000 pyquet-0.1.2/pyquet/pyquet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-05-30 07:57:05.000000 pyquet-0.1.2/pyquet/pyquet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 07:57:05.000000 pyquet-0.1.2/pyquet/pyquet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-30 07:57:05.000000 pyquet-0.1.2/pyquet/pyquet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 07:57:05.000000 pyquet-0.1.2/pyquet/pyquet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      680 2023-05-30 07:57:05.000000 pyquet-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-30 07:57:05.000000 pyquet-0.1.2/tests/
+-rw-rw-rw-   0        0        0     2074 2023-05-30 07:38:36.000000 pyquet-0.1.2/tests/test_reader.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pyquet-0.1.1/LICENSE` & `pyquet-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyquet-0.1.1/PKG-INFO` & `pyquet-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyquet
-Version: 0.1.1
+Version: 0.1.2
 Summary: Text comparator UI
 Home-page: https://github.com/rmugicag/pyquet
 Author: Ricardo Mugica
 Author-email: rmugicag@gmail.com
 Project-URL: Bug Tracker, https://github.com/rmugicag/pyquet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyquet-0.1.1/setup.cfg` & `pyquet-0.1.2/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7971 7565 740d 0a76 6572 7369   = pyquet..versi
-00000020: 6f6e 203d 2030 2e31 2e31 0d0a 6175 7468  on = 0.1.1..auth
+00000020: 6f6e 203d 2030 2e31 2e32 0d0a 6175 7468  on = 0.1.2..auth
 00000030: 6f72 203d 2052 6963 6172 646f 204d 7567  or = Ricardo Mug
 00000040: 6963 610d 0a61 7574 686f 725f 656d 6169  ica..author_emai
 00000050: 6c20 3d20 726d 7567 6963 6167 4067 6d61  l = rmugicag@gma
 00000060: 696c 2e63 6f6d 0d0a 6465 7363 7269 7074  il.com..descript
 00000070: 696f 6e20 3d20 5465 7874 2063 6f6d 7061  ion = Text compa
 00000080: 7261 746f 7220 5549 0d0a 6c6f 6e67 5f64  rator UI..long_d
 00000090: 6573 6372 6970 7469 6f6e 203d 2066 696c  escription = fil
@@ -25,19 +25,19 @@
 00000180: 6e20 3a3a 2033 0d0a 094c 6963 656e 7365  n :: 3...License
 00000190: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
 000001a0: 203a 3a20 4d49 5420 4c69 6365 6e73 650d   :: MIT License.
 000001b0: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
 000001c0: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
 000001d0: 6465 6e74 0d0a 0d0a 5b6f 7074 696f 6e73  dent....[options
 000001e0: 5d0d 0a70 6163 6b61 6765 5f64 6972 203d  ]..package_dir =
-000001f0: 200d 0a09 3d20 7372 630d 0a70 6163 6b61   ...= src..packa
-00000200: 6765 7320 3d20 6669 6e64 3a0d 0a70 7974  ges = find:..pyt
-00000210: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
-00000220: 3d33 2e36 0d0a 696e 7374 616c 6c5f 7265  =3.6..install_re
-00000230: 7175 6972 6573 203d 200d 0a09 7061 6e64  quires = ...pand
-00000240: 6173 0d0a 0970 7961 7272 6f77 0d0a 0d0a  as...pyarrow....
-00000250: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
-00000260: 732e 6669 6e64 5d0d 0a77 6865 7265 203d  s.find]..where =
-00000270: 2073 7263 0d0a 0d0a 5b65 6767 5f69 6e66   src....[egg_inf
-00000280: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
-00000290: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
-000002a0: 0d0a                                     ..
+000001f0: 200d 0a09 3d20 7079 7175 6574 0d0a 7061   ...= pyquet..pa
+00000200: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
+00000210: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
+00000220: 3d20 3e3d 332e 360d 0a69 6e73 7461 6c6c  = >=3.6..install
+00000230: 5f72 6571 7569 7265 7320 3d20 0d0a 0970  _requires = ...p
+00000240: 616e 6461 730d 0a09 7079 6172 726f 770d  andas...pyarrow.
+00000250: 0a0d 0a5b 6f70 7469 6f6e 732e 7061 636b  ...[options.pack
+00000260: 6167 6573 2e66 696e 645d 0d0a 7768 6572  ages.find]..wher
+00000270: 6520 3d20 7079 7175 6574 0d0a 0d0a 5b65  e = pyquet....[e
+00000280: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
+00000290: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
+000002a0: 203d 2030 0d0a 0d0a                       = 0....
```

### Comparing `pyquet-0.1.1/src/pyquet.egg-info/PKG-INFO` & `pyquet-0.1.2/pyquet/pyquet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyquet
-Version: 0.1.1
+Version: 0.1.2
 Summary: Text comparator UI
 Home-page: https://github.com/rmugicag/pyquet
 Author: Ricardo Mugica
 Author-email: rmugicag@gmail.com
 Project-URL: Bug Tracker, https://github.com/rmugicag/pyquet/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyquet-0.1.1/tests/test_reader.py` & `pyquet-0.1.2/tests/test_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 import unittest
-from src.pyquet.schemas import Reader
+from pyquet.schemas import Reader
 
 
 class ReaderTestCase(unittest.TestCase):
     def setUp(self):
         self.schemas_path = os.path.join(os.path.dirname(__file__), "test_data", "schemas")
         self.schemas_path_without_schemas = os.path.join(self.schemas_path, "data")
         self.schema_1 = os.path.join(self.schemas_path, 'schema_1.json')
```

