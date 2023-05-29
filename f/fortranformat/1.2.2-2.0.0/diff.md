# Comparing `tmp/fortranformat-1.2.2.tar.gz` & `tmp/fortranformat-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fortranformat-1.2.2.tar", last modified: Tue Aug 23 22:02:22 2022, max compression
+gzip compressed data, was "dist/fortranformat-2.0.0.tar", last modified: Mon May 29 22:54:28 2023, max compression
```

## Comparing `fortranformat-1.2.2.tar` & `fortranformat-2.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 brendan    (501) staff       (20)        0 2022-08-23 22:02:22.000000 fortranformat-1.2.2/
--rw-r--r--   0 brendan    (501) staff       (20)     1076 2021-12-28 21:20:41.000000 fortranformat-1.2.2/LICENSE
--rw-r--r--   0 brendan    (501) staff       (20)       16 2021-12-29 12:44:49.000000 fortranformat-1.2.2/MANIFEST.in
--rw-r--r--   0 brendan    (501) staff       (20)     5052 2022-08-23 22:02:22.000000 fortranformat-1.2.2/PKG-INFO
--rw-r--r--   0 brendan    (501) staff       (20)     3341 2022-07-24 06:44:21.000000 fortranformat-1.2.2/README.md
-drwxr-xr-x   0 brendan    (501) staff       (20)        0 2022-08-23 22:02:22.000000 fortranformat-1.2.2/fortranformat/
--rw-r--r--   0 brendan    (501) staff       (20)     1961 2021-12-29 14:28:06.000000 fortranformat-1.2.2/fortranformat/FortranRecordReader.py
--rw-r--r--   0 brendan    (501) staff       (20)     1744 2021-12-29 14:26:16.000000 fortranformat-1.2.2/fortranformat/FortranRecordWriter.py
--rw-r--r--   0 brendan    (501) staff       (20)      195 2022-08-23 22:01:07.000000 fortranformat-1.2.2/fortranformat/__init__.py
--rw-r--r--   0 brendan    (501) staff       (20)     8800 2021-12-22 22:30:03.000000 fortranformat-1.2.2/fortranformat/_edit_descriptors.py
--rw-r--r--   0 brendan    (501) staff       (20)       45 2021-03-14 14:32:54.000000 fortranformat-1.2.2/fortranformat/_exceptions.py
--rw-r--r--   0 brendan    (501) staff       (20)    13627 2021-12-29 14:30:36.000000 fortranformat-1.2.2/fortranformat/_input.py
--rw-r--r--   0 brendan    (501) staff       (20)     5921 2021-12-22 22:30:21.000000 fortranformat-1.2.2/fortranformat/_lexer.py
--rw-r--r--   0 brendan    (501) staff       (20)     1193 2021-03-14 15:00:44.000000 fortranformat-1.2.2/fortranformat/_misc.py
--rw-r--r--   0 brendan    (501) staff       (20)    27316 2022-08-23 21:53:59.000000 fortranformat-1.2.2/fortranformat/_output.py
--rw-r--r--   0 brendan    (501) staff       (20)    14299 2021-12-22 22:30:58.000000 fortranformat-1.2.2/fortranformat/_parser.py
--rw-r--r--   0 brendan    (501) staff       (20)     2160 2021-12-29 01:56:19.000000 fortranformat-1.2.2/fortranformat/config.py
-drwxr-xr-x   0 brendan    (501) staff       (20)        0 2022-08-23 22:02:22.000000 fortranformat-1.2.2/fortranformat.egg-info/
--rw-r--r--   0 brendan    (501) staff       (20)     5052 2022-08-23 22:02:22.000000 fortranformat-1.2.2/fortranformat.egg-info/PKG-INFO
--rw-r--r--   0 brendan    (501) staff       (20)      505 2022-08-23 22:02:22.000000 fortranformat-1.2.2/fortranformat.egg-info/SOURCES.txt
--rw-r--r--   0 brendan    (501) staff       (20)        1 2022-08-23 22:02:22.000000 fortranformat-1.2.2/fortranformat.egg-info/dependency_links.txt
--rw-r--r--   0 brendan    (501) staff       (20)       14 2022-08-23 22:02:22.000000 fortranformat-1.2.2/fortranformat.egg-info/top_level.txt
--rw-r--r--   0 brendan    (501) staff       (20)       79 2022-08-23 22:02:22.000000 fortranformat-1.2.2/setup.cfg
--rw-r--r--   0 brendan    (501) staff       (20)     1187 2022-08-23 22:00:53.000000 fortranformat-1.2.2/setup.py
+drwxr-xr-x   0 brendan    (501) staff       (20)        0 2023-05-29 22:54:28.000000 fortranformat-2.0.0/
+-rw-r--r--   0 brendan    (501) staff       (20)     1076 2021-12-28 21:20:41.000000 fortranformat-2.0.0/LICENSE
+-rw-r--r--   0 brendan    (501) staff       (20)       16 2021-12-29 12:44:49.000000 fortranformat-2.0.0/MANIFEST.in
+-rw-r--r--   0 brendan    (501) staff       (20)     5173 2023-05-29 22:54:28.000000 fortranformat-2.0.0/PKG-INFO
+-rw-r--r--   0 brendan    (501) staff       (20)     3478 2023-05-29 22:52:15.000000 fortranformat-2.0.0/README.md
+drwxr-xr-x   0 brendan    (501) staff       (20)        0 2023-05-29 22:54:28.000000 fortranformat-2.0.0/fortranformat/
+-rw-r--r--   0 brendan    (501) staff       (20)     1961 2021-12-29 14:28:06.000000 fortranformat-2.0.0/fortranformat/FortranRecordReader.py
+-rw-r--r--   0 brendan    (501) staff       (20)     1744 2021-12-29 14:26:16.000000 fortranformat-2.0.0/fortranformat/FortranRecordWriter.py
+-rw-r--r--   0 brendan    (501) staff       (20)      195 2023-05-29 22:53:40.000000 fortranformat-2.0.0/fortranformat/__init__.py
+-rw-r--r--   0 brendan    (501) staff       (20)    10747 2023-05-29 22:49:09.000000 fortranformat-2.0.0/fortranformat/_edit_descriptors.py
+-rw-r--r--   0 brendan    (501) staff       (20)       45 2021-03-14 14:32:54.000000 fortranformat-2.0.0/fortranformat/_exceptions.py
+-rw-r--r--   0 brendan    (501) staff       (20)    13236 2023-05-29 22:49:09.000000 fortranformat-2.0.0/fortranformat/_input.py
+-rw-r--r--   0 brendan    (501) staff       (20)     5933 2023-05-29 22:49:09.000000 fortranformat-2.0.0/fortranformat/_lexer.py
+-rw-r--r--   0 brendan    (501) staff       (20)     1193 2021-03-14 15:00:44.000000 fortranformat-2.0.0/fortranformat/_misc.py
+-rw-r--r--   0 brendan    (501) staff       (20)    24468 2023-05-29 22:49:09.000000 fortranformat-2.0.0/fortranformat/_output.py
+-rw-r--r--   0 brendan    (501) staff       (20)    14311 2023-05-29 22:49:09.000000 fortranformat-2.0.0/fortranformat/_parser.py
+-rw-r--r--   0 brendan    (501) staff       (20)     2160 2021-12-29 01:56:19.000000 fortranformat-2.0.0/fortranformat/config.py
+drwxr-xr-x   0 brendan    (501) staff       (20)        0 2023-05-29 22:54:28.000000 fortranformat-2.0.0/fortranformat.egg-info/
+-rw-r--r--   0 brendan    (501) staff       (20)     5173 2023-05-29 22:54:28.000000 fortranformat-2.0.0/fortranformat.egg-info/PKG-INFO
+-rw-r--r--   0 brendan    (501) staff       (20)      505 2023-05-29 22:54:28.000000 fortranformat-2.0.0/fortranformat.egg-info/SOURCES.txt
+-rw-r--r--   0 brendan    (501) staff       (20)        1 2023-05-29 22:54:28.000000 fortranformat-2.0.0/fortranformat.egg-info/dependency_links.txt
+-rw-r--r--   0 brendan    (501) staff       (20)       14 2023-05-29 22:54:28.000000 fortranformat-2.0.0/fortranformat.egg-info/top_level.txt
+-rw-r--r--   0 brendan    (501) staff       (20)       79 2023-05-29 22:54:28.000000 fortranformat-2.0.0/setup.cfg
+-rw-r--r--   0 brendan    (501) staff       (20)     1140 2023-05-29 22:53:18.000000 fortranformat-2.0.0/setup.py
```

### Comparing `fortranformat-1.2.2/LICENSE` & `fortranformat-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fortranformat-1.2.2/PKG-INFO` & `fortranformat-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortranformat
-Version: 1.2.2
+Version: 2.0.0
 Summary: Mimics Fortran textual IO in Python
 Home-page: https://github.com/brendanarnold/py-fortranformat
 Author: Brendan Arnold
 Author-email: brendanarnold@gmail.com
 License: UNKNOWN
 Description: # FORTRAN format interpreter for Python
         
@@ -71,14 +71,18 @@
         
         Note that some of the F output edit descriptors fail due to limitations in floating point number representation
         
         To run a reduced test suite where time and resources are limited, use the following
         
         `make runminimaltests`
         
+        To run a performance test, which currently only covers the reading and writing of floats, use the following
+        
+        `make runperformancetests`
+        
         ### Deploying a new package version
         
         Update versions in `setup.py` and `__init__.py`
         
         Update `CHANGELOG.md`
         
         To create a local build to test run ...
@@ -108,13 +112,12 @@
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Fortran
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Text Processing :: General
 Classifier: Topic :: Software Development :: Interpreters
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
```

### Comparing `fortranformat-1.2.2/README.md` & `fortranformat-2.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -63,14 +63,18 @@
 
 Note that some of the F output edit descriptors fail due to limitations in floating point number representation
 
 To run a reduced test suite where time and resources are limited, use the following
 
 `make runminimaltests`
 
+To run a performance test, which currently only covers the reading and writing of floats, use the following
+
+`make runperformancetests`
+
 ### Deploying a new package version
 
 Update versions in `setup.py` and `__init__.py`
 
 Update `CHANGELOG.md`
 
 To create a local build to test run ...
```

### Comparing `fortranformat-1.2.2/fortranformat/FortranRecordReader.py` & `fortranformat-2.0.0/fortranformat/FortranRecordReader.py`

 * *Files identical despite different names*

### Comparing `fortranformat-1.2.2/fortranformat/FortranRecordWriter.py` & `fortranformat-2.0.0/fortranformat/FortranRecordWriter.py`

 * *Files identical despite different names*

### Comparing `fortranformat-1.2.2/fortranformat/_edit_descriptors.py` & `fortranformat-2.0.0/fortranformat/_edit_descriptors.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ._exceptions import *
+from ._exceptions import InvalidFormat
 
 def get_edit_descriptor_obj(name):
     '''Returns a new object instance from a string'''
     name = name.upper()
     if name == 'A':
         return A()
     elif name == 'B':
@@ -55,231 +55,334 @@
         return Z()
     else:
         raise InvalidFormat('Expected an edit descriptor, got %s' % name)
 
 # All the tokens defined in the F77 specification unless specified
 
 class A(object):
+    name = "A"
+    is_non_reversion = False
+    is_output = True
+
     def __init__(self):
         self.repeat = None
         self.width = None
     def __repr__(self):
         return '<A repeat=' + str(self.repeat) + \
                 ' width=' + str(self.width) + '>'
 
 class QuotedString(object):
+    name = "QuotedString"
+    is_non_reversion = False
+    is_output = False
     def __init__(self, char_string=None):
         self.char_string = char_string
     def get_width(self):
         return len(self.char_string)
     width = property(get_width)
     def __repr__(self):
         return '<QuotedString char_string=' + str(self.char_string) + '>'
 
 # Only in F95
 class B(object):
+    name = "B"
+    is_non_reversion = False
+    is_output = True
+    base = 2
+
     def __init__(self):
         self.repeat = None
         self.width = None
         self.min_digits = None
+
     def __repr__(self):
         return '<B repeat=' + str(self.repeat) + \
                 ' width=' + str(self.width) + \
                 ' min_digits=' + str(self.min_digits) + '>'
     
 class BN(object):
+    name = "BN"
+    is_non_reversion = True
+    is_output = False
     def __init__(self):
         pass
     def __repr__(self):
         return '<BN>'
 
 class BZ(object):
+    name = "BZ"
+    is_non_reversion = True
+    is_output = False
     def __init__(self):
         pass
     def __repr__(self):
         return '<BZ>'
 
 class Colon(object):
+    name = "Colon"
+    is_non_reversion = False
+    is_output = False
     def __init__(self):
         pass
     def __repr__(self):
         return '<Colon>'
     
 class D(object):
+    name = "D"
+    is_non_reversion = False
+    is_output = True
+
     def __init__(self):
         self.repeat = None
         self.width = None
+        self.exponent = None
         self.decimal_places = None
     def __repr__(self):
         return '<D repeat=' + str(self.repeat) + \
                 ' width=' + str(self.width) + \
                 ' decimal_places=' + str(self.decimal_places) + '>'
 
 class E(object):
+    name = "E"
+    is_non_reversion = False
+    is_output = True
+
     def __init__(self):
         self.repeat = None
         self.width = None
         self.decimal_places = None
         self.exponent = None
     def __repr__(self):
         return '<E repeat=' + str(self.repeat) + \
                 ' width=' + str(self.width) + \
                 ' decimal_places=' + str(self.decimal_places) + \
                 ' exponent=' + str(self.exponent) + '>'
     
 # Only in F95
 class EN(object):
+    name = "EN"
+    is_non_reversion = False
+    is_output = True
+
     def __init__(self):
         self.repeat = None
         self.width = None
         self.decimal_places = None
         self.exponent = None
     def __repr__(self):
         return '<EN repeat=' + str(self.repeat) + \
                 ' width=' + str(self.width) + \
                 ' decimal_places=' + str(self.decimal_places) + \
                 ' exponent=' + str(self.exponent) + '>'
 
 # Only in F95
 class ES(object):
+    name = "ES"
+    is_non_reversion = False
+    is_output = True
+
     def __init__(self):
         self.repeat = None
         self.width = None
         self.decimal_places = None
         self.exponent = None
     def __repr__(self):
         return '<ES repeat=' + str(self.repeat) + \
                 ' width=' + str(self.width) + \
                 ' decimal_places=' + str(self.decimal_places) + \
                 ' exponent=' + str(self.exponent) + '>'
 
 class F(object):
+    name = "F"
+    is_non_reversion = False
+    is_output = True
+
     def __init__(self):
         self.repeat = None
         self.width = None
+        self.exponent = None
         self.decimal_places = None
     def __repr__(self):
         return '<F repeat=' + str(self.repeat) + \
                 ' width=' + str(self.width) + \
                 ' decimal_places=' + str(self.decimal_places) + '>'
     
 class FormatGroup(object):
+    name = "FormatGroup"
+    is_non_reversion = False
+    is_output = False
     pass
 
 class G(object):
+    name = "G"
+    is_non_reversion = False
+    is_output = True
+
     def __init__(self):
         self.repeat = None
         self.width = None
         self.decimal_places = None
         self.exponent = None
     def __repr__(self):
         return '<G repeat=' + str(self.repeat) + \
                 ' width=' + str(self.width) + \
                 ' decimal_places=' + str(self.decimal_places) + \
                 ' exponent=' + str(self.exponent) + '>'
 
 # Only in F77
 class H(object):
+    name = "H"
+    is_non_reversion = False
+    is_output = False
     def __init__(self):
         self.num_chars = None
         self.char_string = None
     def __repr__(self):
         return '<H num_chars=' + str(self.num_chars) + \
                 ' char_string=' + str(self.char_string) + '>'
     
 class I(object):
+    name = "I"
+    is_non_reversion = False
+    is_output = True
+    base = 10
+
     def __init__(self):
         self.repeat = None
         self.width = None
         self.min_digits = None
+
     def __repr__(self):
         return '<I repeat=' + str(self.repeat) + \
                 ' width=' + str(self.width) + \
                 ' min_digits=' + str(self.min_digits) + '>'
     
 class L(object):
+    name = "L"
+    is_non_reversion = False
+    is_output = True
+
     def __init__(self):
         self.repeat = None
         self.width = None
     def __repr__(self):
         return '<L repeat=' + str(self.repeat) + \
                 ' width=' + str(self.width) + '>'
 
 # Only in F95
 class O(object):
+    name = "O"
+    is_non_reversion = False
+    is_output = True
+    base = 8
+
     def __init__(self):
         self.repeat = None
         self.width = None
         self.min_digits = None
+
     def __repr__(self):
         return '<O repeat=' + str(self.repeat) + \
                 ' width=' + str(self.width) + \
                 ' min_digits=' + str(self.min_digits) + '>'
 
 class P(object):
+    name = "P"
+    is_non_reversion = True
+    is_output = False
     def __init__(self):
         self.scale = None
     def __repr__(self):
         return '<P scale=' + str(self.scale) + '>'
     
 class S(object):
+    name = "S"
+    is_non_reversion = True
+    is_output = False
     def __init__(self):
         pass
     def __repr__(self):
         return '<S>'
     
 class Slash(object):
+    name = "Slash"
+    is_non_reversion = False
+    is_output = False
     def __init__(self):
         self.repeat = None
         pass
     def __repr__(self):
         return '<Slash repeat=' + str(self.repeat) + '>'
     
 class SP(object):
+    name = "SP"
+    is_non_reversion = True
+    is_output = False
     def __init__(self):
         pass
     def __repr__(self):
         return '<SP>'
     
 class SS(object):
+    name = "SS"
+    is_non_reversion = True
+    is_output = False
     def __init__(self):
         pass
     def __repr__(self):
         return '<SS>'
     
 class T(object):
+    name = "T"
+    is_non_reversion = False
+    is_output = False
     def __init__(self):
         self.num_chars = None
     def __repr__(self):
         return '<T num_chars=' + str(self.num_chars) + '>'
     
 class TL(object):
+    name = "TL"
+    is_non_reversion = False
+    is_output = False
     def __init__(self):
         self.num_chars = None
     def __repr__(self):
         return '<TL num_chars=' + str(self.num_chars) + '>'
     
 class TR(object):
+    name = "TR"
+    is_non_reversion = False
+    is_output = False
     def __init__(self):
         self.num_chars = None
     def __repr__(self):
         return '<TR num_chars=' + str(self.num_chars) + '>'
 
 class X(object):
+    name = "X"
+    is_non_reversion = False
+    is_output = False
     def __init__(self):
         self.num_chars = None
     def __repr__(self):
         return '<X num_chars=' + str(self.num_chars) + '>'
 
 # Only in F95
 class Z(object):
+    name = "Z"
+    is_non_reversion = False
+    is_output = True
+    base = 16
+
     def __init__(self):
         self.repeat = None
         self.width = None
         self.min_digits = None
+
     def __repr__(self):
         return '<Z repeat=' + str(self.repeat) + \
                 ' width=' + str(self.width) + \
                 ' min_digits=' + str(self.min_digits) + '>'
 
 # Categorise the edit descriptors depending on how they should be parsed
 
@@ -290,12 +393,10 @@
 ED5 = ['D', 'F'] # Of form Xn.m only
 ED6 = ['B', 'I', 'O', 'Z'] # Of form Xn or Xn.m
 ED7 = ['E', 'EN', 'ES', 'G'] # Of form Xn.m or Xn.mEe
 ED8 = ['P'] # Of form kX only, where k is a signed integer, may omit comma if followed by Type 5 or 7 edit descriptor
 ED9 = [':'] # Of form X only, may omit comma either side
 ED10 = ['/'] # Of form X only, may omit following comma and leading comma if no repeat
 REPEATABLE_EDS = ['L', 'A', 'D', 'F', 'B', 'I', 'O', 'Z', 'E', 'EN', 'ES', 'G', '/']
-OUTPUT_EDS = (L, A, D, F, B, I, O, Z, E, EN, ES, G)
 CONTROL_EDS = (BN, BZ, P, SP, SS, S, X, T, TR, TL, Colon, Slash)
-NON_REVERSION_EDS = (P, S, SP, SS, BN, BZ)
 ALL_ED = ED1 + ED2 + ED3 + ED4 + ED5 + ED6 + ED7 + ED8 + ED9 + ED10
```

### Comparing `fortranformat-1.2.2/fortranformat/_input.py` & `fortranformat-2.0.0/fortranformat/_input.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,37 @@
 import re
 from ._edit_descriptors import *
+from ._exceptions import InvalidFormat
 from ._misc import expand_edit_descriptors
 from . import config
 
 WIDTH_OPTIONAL_EDS = [A]
 NON_WIDTH_EDS = [BN, BZ, P, SP, SS, S, X, T, TR, TL, Colon, Slash]
 FORBIDDEN_EDS = [QuotedString, H]
 
 # Some problems without pre written input vars:
 #   Cannot say when reversion conditions are met
 #   Cannot determine width of A edit descriptor
 #   Cannot determine complex input
 #   Cannot determine proper input for G edit descriptors
 
 
+CONTROL_COMMANDS = {
+    "BN": lambda position, ed, record: {'blanks_as_zeros': False},
+    "BZ": lambda position, ed, record: {'blanks_as_zeros': True},
+    "P": lambda position, ed, record: {'scale': ed.scale},
+    "SP": lambda position, ed, record: {'incl_plus': True},
+    "SS": lambda position, ed, record: {'incl_plus': False},
+    "S": lambda position, ed, record: {'incl_plus': config.PROC_INCL_PLUS},
+    "X": lambda position, ed, record: {'position': min(position + ed.num_chars, len(record))},
+    "TR": lambda position, ed, record: {'position': min(position + ed.num_chars, len(record))},
+    "TL": lambda position, ed, record: {'position': max(position - ed.num_chars, 0)},
+    "T": lambda position, ed, record: {'position': max(0, min(ed.num_chars - 1, len(record)))},
+}
+
 def input(eds, reversion_eds, records, num_vals=None):
 
     state = {
         'position': 0,
         'scale': 0,
         'incl_plus': False,
         'blanks_as_zeros': config.PROC_BLANKS_AS_ZEROS,
@@ -33,40 +47,36 @@
             raise InvalidFormat("%d edit descriptor not permitted on input")
 
     # Expand repeated edit decriptors
     eds = expand_edit_descriptors(eds)
     reversion_eds = expand_edit_descriptors(reversion_eds)
     # Assume one-to-one correspondance between edit descriptors and output
     # values if number of output values is not defined
-    num_out_eds = 0
-    for ed in eds:
-        if isinstance(ed, OUTPUT_EDS):
-            num_out_eds += 1
-    num_rev_out_eds = 0
+    num_out_eds = sum((ed.is_output for ed in eds))
+    num_rev_out_eds = sum((ed.is_output for ed in reversion_eds))
     if num_vals is None:
         num_vals = num_out_eds
-    for ed in reversion_eds:
-        if isinstance(ed, OUTPUT_EDS):
-            num_rev_out_eds += 1
 
     # Will loop forever is no output edit descriptors
     if (num_out_eds == 0):
         return []
     # Will loop forever if no output eds in reversion format and is more values
     # requested than in the format
     if (num_vals > num_out_eds) and (num_rev_out_eds == 0):
         raise ValueError(
             'Not enough output edit descriptors in reversion format to output %d values' % num_vals)
 
     # May need to process multiple records, down to a higher function to supply
     # appropriate string for format
     if not hasattr(records, 'next'):
-        records = iter(re.split('\r\n|\r|\n', records))
-    record = next_with_default(records, None)
-    if record is None:
+        records = iter(records.splitlines() or [""])
+
+    try:
+        record = next(records)
+    except StopIteration:
         return []
 
     # if a_widths is not None:
     #     a_widths = itertools.cycle(a_widths)
 
     vals = []
     finish_up = False
@@ -86,41 +96,20 @@
             if finish_up and (rev_ed_ind == 0):
                 break
             ed = reversion_eds[rev_ed_ind]
 
         if isinstance(ed, QuotedString):
             raise InvalidFormat(
                 'Cannot have string literal in an input format')
-        elif isinstance(ed, BN):
-            state['blanks_as_zeros'] = False
-        elif isinstance(ed, BZ):
-            state['blanks_as_zeros'] = True
-        elif isinstance(ed, P):
-            state['scale'] = ed.scale
-        elif isinstance(ed, SP):
-            state['incl_plus'] = True
-        elif isinstance(ed, SS):
-            state['incl_plus'] = False
-        elif isinstance(ed, S):
-            state['incl_plus'] = config.PROC_INCL_PLUS
-        elif isinstance(ed, (X, TR)):
-            state['position'] = min(
-                state['position'] + ed.num_chars, len(record))
-        elif isinstance(ed, TL):
-            state['position'] = max(state['position'] - ed.num_chars, 0)
-        elif isinstance(ed, T):
-            if (ed.num_chars - 1) < 0:
-                state['position'] = 0
-            elif ed.num_chars > len(record):
-                state['position'] = len(record)
-            else:
-                state['position'] = ed.num_chars - 1
+        elif ed.name in CONTROL_COMMANDS:
+            func = CONTROL_COMMANDS[ed.name]
+            state.update(func(state["position"], ed, record))
         elif isinstance(ed, Slash):
             # End of record
-            record = next_with_default(records, None)
+            record = next(records, None)
             state['position'] = 0
             if record is None:
                 break
         elif isinstance(ed, Colon):
             # Break if input value satisfied
             if finish_up:
                 break
@@ -141,15 +130,15 @@
             # Use the G_INPUT_TRIAL_EDS variable to try the variables
             # until one sticks
             # n.b. vals and state do not get written to if
             # exception id raised
             resolved = False
             g_trial_eds = iter(config.G_INPUT_TRIAL_EDS)
             while not resolved:
-                ed_name = next_with_default(g_trial_eds, None)
+                ed_name = next(g_trial_eds, None)
                 if ed_name is None:
                     raise ValueError(
                         'No suitable edit descriptor in config.G_INPUT_TRIAL_EDS')
                 elif ed_name.upper() in ('F', 'E', 'D', 'EN', 'ES'):
                     trial_ed = F()
                     trial_ed.width = ed.width
                     trial_ed.decimal_places = ed.decimal_places
@@ -226,22 +215,14 @@
     #     w = 0
     # else:
     substr = record[start:end]
     state['position'] = min(state['position'] + w, len(record))
     return substr, state
 
 
-def next_with_default(it, default=None):
-    try:
-        val = next(it)
-    except StopIteration:
-        val = default
-    return val
-
-
 def read_string(ed, state, record):
     if ed.width is None:
         # Will assume rest of record is fair game for the
         # unsized A edit descriptor
         ed.width = len(record) - state['position']
     substr, state = _get_substr(ed.width, record, state)
     val = substr.ljust(ed.width, config.PROC_PAD_CHAR)
@@ -252,22 +233,14 @@
     substr, state = _get_substr(ed.width, record, state)
     if ('-' in substr) and (not config.PROC_ALLOW_NEG_BOZ) and isinstance(ed, (Z, O, B)):
         if state['exception_on_fail']:
             raise ValueError(
                 'Negative numbers not permitted for binary, octal or hex')
         else:
             return (None, state)
-    if isinstance(ed, Z):
-        base = 16
-    elif isinstance(ed, I):
-        base = 10
-    elif isinstance(ed, O):
-        base = 8
-    elif isinstance(ed, B):
-        base = 2
     # If a negative is followed by blanks, Gfortran and ifort
     # interpret as a zero
     if re.match(r'^ *- +$', substr):
         substr = '0'
     # If a negative or negative and blanks, ifort interprets as
     # zero for an I edit descriptor
     if config.PROC_NEG_AS_ZERO and isinstance(ed, I) and re.match(r'^( *- *| +)$', substr):
@@ -278,15 +251,15 @@
     if substr == '':
         if config.RET_UNWRITTEN_VARS_NONE or config.RET_WRITTEN_VARS_ONLY:
             return (None, state)
         else:
             substr = '0'
     teststr = _interpret_blanks(substr, state)
     try:
-        val = int(teststr, base)
+        val = int(teststr, ed.base)
     except ValueError:
         if state['exception_on_fail']:
             raise ValueError(
                 '%s is not a valid input for one of integer, octal, hex or binary' % substr)
         else:
             return (None, state)
     return (val, state)
@@ -313,14 +286,18 @@
         if state['exception_on_fail']:
             raise ValueError('%s is not a valid boolean input' % substr)
         else:
             val = None
     return (val, state)
 
 
+DECIMAL_RE = re.compile(r"^ *\. *$")
+MINUS_RE = re.compile(r"^ *- *$")
+EXPONENT_RE = re.compile(r"(.*)E[-+]?$")
+
 def read_float(ed, state, record):
     substr, state = _get_substr(ed.width, record, state)
     teststr = _interpret_blanks(substr, state)
     # When reading off end of record, get empty string,
     # interpret as 0
     if teststr == '':
         if config.RET_UNWRITTEN_VARS_NONE or config.RET_WRITTEN_VARS_ONLY:
@@ -330,22 +307,22 @@
     # Python only understands 'E' as an exponential letter
     teststr = teststr.upper().replace('D', 'E')
     # Prepend an exponential letter if only a '-' or '+' denotes an exponent
     if 'E' not in teststr:
         teststr = teststr[0] + \
             teststr[1:].replace('+', 'E+').replace('-', 'E-')
     # ifort allows '.' to be interpreted as 0
-    if re.match(r'^ *\. *$', teststr):
+    if DECIMAL_RE.match(teststr):
         teststr = '0'
     # ifort allows '-' to be interpreted as 0
-    if re.match(r'^ *- *$', teststr):
+    if MINUS_RE.match(teststr):
         teststr = '0'
     # ifort allows numbers to end with 'E', 'E+', 'E-' and 'D'
     # equivalents
-    res = re.match(r'(.*)(E|E\+|E\-)$', teststr)
+    res = EXPONENT_RE.match(teststr)
     if res:
         teststr = res.group(1)
     try:
         val = float(teststr)
     except ValueError:
         if state['exception_on_fail']:
             raise ValueError(
```

### Comparing `fortranformat-1.2.2/fortranformat/_lexer.py` & `fortranformat-2.0.0/fortranformat/_lexer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from ._edit_descriptors import *
-from ._exceptions import *
+from ._exceptions import InvalidFormat
 
 # Some lexer tokens to look out for
 DIGITS = ['1', '2', '3', '4', '5', '6', '7', '8', '9', '0']
 SIGNS = ['+', '-']
 COMMA = [',']
 DOT = ['.']
 WHITESPACE = [' ', '\t', '\n']
```

### Comparing `fortranformat-1.2.2/fortranformat/_misc.py` & `fortranformat-2.0.0/fortranformat/_misc.py`

 * *Files identical despite different names*

### Comparing `fortranformat-1.2.2/fortranformat/_output.py` & `fortranformat-2.0.0/fortranformat/_output.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import math
+from io import StringIO
+
 from ._edit_descriptors import *
+from ._exceptions import InvalidFormat
 from ._misc import expand_edit_descriptors, has_next_iterator
 from . import config
 
 
 PROC_SIGN_ZERO = config.PROC_SIGN_ZERO
 PROC_MIN_FIELD_WIDTH = config.PROC_MIN_FIELD_WIDTH
 PROC_DECIMAL_CHAR = config.PROC_DECIMAL_CHAR
@@ -12,30 +15,30 @@
 
 
 def output(eds, reversion_eds, values):
     '''
     a function to take a list of valid f77 edit descriptors and respective values
     and output the corresponding string
     '''
-    record = ''
+    record = StringIO()
     state = {
         'position': 0,
         'scale': 0,
         'incl_plus': False,
         'blanks_as_zeros': False,
         'halt_if_no_vals': False,
     }
 
     # if format is empty with no values specified, then output blank record -
     # see section 13.3
 
     # check that if there is a reversion, that values can be output
     reversion_contains_output_ed = False
     for ed in reversion_eds:
-        if isinstance(ed, OUTPUT_EDS):
+        if ed.is_output:
             reversion_contains_output_ed = True
             break
     # Get full list of edit descriptors
     eds = expand_edit_descriptors(eds)
     reversion_eds = expand_edit_descriptors(reversion_eds)
     # use iterators
     get_ed = has_next_iterator(eds)
@@ -57,147 +60,95 @@
                 # take from reversion edit descriptors if there is a value
                 # requiring output still
 
                 while True:
                     if len(tmp_reversion_eds):
                         ed = tmp_reversion_eds.pop()
                         # these edit descriptors are ignored in reversion state
-                        if not isinstance(ed, NON_REVERSION_EDS):
+                        if not ed.is_non_reversion:
                             break
                     else:
                         # Regardless of where cursor is, is moved to the
                         # next record
-                        record = record + config.RECORD_SEPARATOR
-                        state['position'] = len(record)
+                        record.write(config.RECORD_SEPARATOR)
+                        state['position'] = record.tell()
                         if get_value.has_next():
                             # Only reset the reversion if we have more values to output
                             tmp_reversion_eds = reversion_eds[::-1]
                         else:
                             # ... otherwise we are done
                             is_complete = True
                             break
                 if is_complete:
                     break
             else:
                 # ignore the revsersion edit descriptors as cannot output the
                 # final value
                 break
         # check if edit descriptor requires a value
-        if isinstance(ed, OUTPUT_EDS):
+        if ed.is_output:
             if get_value.has_next():
                 val = next(get_value)
             else:
                 # is a edit descriptor that requires a value but no value
                 # we simply ignore at this point - likely this is an incomplete reversion
                 break
-            if isinstance(ed, I):
+            if ed.name == "I":
                 if val is None:
                     val = 0
                 sub_string = _compose_i_string(
                     ed.width, ed.min_digits, state, val)
-            elif isinstance(ed, B):
-                if val is None:
-                    val = 0
-                w = ed.width
-                m = ed.min_digits
-                sub_string = _compose_boz_string(w, m, state, val, 'B')
-            if isinstance(ed, O):
-                if val is None:
-                    val = 0
-                w = ed.width
-                m = ed.min_digits
-                sub_string = _compose_boz_string(w, m, state, val, 'O')
-            if isinstance(ed, Z):
+            elif ed.name in ("B", "O", "Z"):
                 if val is None:
                     val = 0
-                w = ed.width
-                m = ed.min_digits
-                sub_string = _compose_boz_string(w, m, state, val, 'Z')
-            elif isinstance(ed, F):
+                sub_string = _compose_boz_string(ed.width, ed.min_digits, state, val, ed.name)
+            elif ed.name in ("D", "E", "EN", "ES", "F", "G"):
                 if val is None:
                     val = 0.0
-                w = ed.width
-                e = None
-                d = ed.decimal_places
-                sub_string = _compose_float_string(w, e, d, state, val, 'F')
-            elif isinstance(ed, E):
-                if val is None:
-                    val = 0.0
-                w = ed.width
-                e = ed.exponent
-                d = ed.decimal_places
-                sub_string = _compose_float_string(w, e, d, state, val, 'E')
-            elif isinstance(ed, D):
-                if val is None:
-                    val = 0.0
-                w = ed.width
-                e = None
-                d = ed.decimal_places
-                sub_string = _compose_float_string(w, e, d, state, val, 'D')
-            elif isinstance(ed, G):
-                if val is None:
-                    val = 0.0
-                w = ed.width
-                e = ed.exponent
-                d = ed.decimal_places
-                sub_string = _compose_float_string(w, e, d, state, val, 'G')
-            elif isinstance(ed, EN):
-                if val is None:
-                    val = 0.0
-                w = ed.width
-                e = ed.exponent
-                d = ed.decimal_places
-                sub_string = _compose_float_string(w, e, d, state, val, 'EN')
-            elif isinstance(ed, ES):
-                if val is None:
-                    val = 0.0
-                w = ed.width
-                e = ed.exponent
-                d = ed.decimal_places
-                sub_string = _compose_float_string(w, e, d, state, val, 'ES')
-            elif isinstance(ed, L):
+                sub_string = _compose_float_string(ed.width, ed.exponent, ed.decimal_places, state, val, ed.name)
+            elif ed.name == "L":
                 if val is None:
                     val = True
                 sub_string = _compose_l_string(ed.width, state, val)
-            elif isinstance(ed, A):
+            elif ed.name == "A":
                 if val is None:
                     val = ''
                 sub_string = _compose_a_string(ed.width, state, val)
             state['position'], record = _write_string(
                 record, sub_string, state['position'])
         else:
             # token does not require a value
-            if isinstance(ed, (S, SS)):
+            if ed.name in ("S", "SS"):
                 state['incl_plus'] = False
-            if isinstance(ed, SP):
+            if ed.name == "SP":
                 state['incl_plus'] = True
-            elif isinstance(ed, P):
+            elif ed.name == "P":
                 state['scale'] = ed.scale
-            elif isinstance(ed, BN):
+            elif ed.name == "BN":
                 # This is moot since for output, this does not do anything
                 state['blanks_as_zeros'] = False
-            elif isinstance(ed, BZ):
+            elif ed.name == "BZ":
                 state['blanks_as_zeros'] = True
-            elif isinstance(ed, Colon):
+            elif ed.name == "Colon":
                 state['halt_if_no_vals'] = True
-            elif isinstance(ed, Slash):
+            elif ed.name == "Slash":
                 state['position'], record = _write_string(
                     record, config.RECORD_SEPARATOR, state['position'])
-            elif isinstance(ed, (X, TR)):
+            elif ed.name in ("X", "TR"):
                 state['position'] = state['position'] + ed.num_chars
-            elif isinstance(ed, TL):
+            elif ed.name == "TL":
                 state['position'] = state['position'] - ed.num_chars
-            elif isinstance(ed, T):
+            elif ed.name == "T":
                 state['position'] = ed.num_chars - 1
-            elif isinstance(ed, QuotedString):
+            elif ed.name == "QuotedString":
                 sub_string = ed.char_string
                 state['position'], record = _write_string(
                     record, sub_string, state['position'])
     # output the final record
-    return record
+    return record.getvalue()
 
 
 def _compose_nan_string(w, ftype):
     if ftype in ['B', 'O', 'Z']:
         return ''
     else:
         # Allow at least 'NaN' to be printed
@@ -285,20 +236,15 @@
     # Round the input if the input is less than 1
     if (ftype == 'F') and (d == state['scale']) and (d == 0):
         if tmp < 1.0:
             tmp = round(tmp)
     zero_flag = (tmp == 0)
     # === DTOA === (macro)
     # write the tmp value to the string buffer
-    # sprintf seems to allow negative number of decimal places, need to correct for this
-    if ndigits <= 0:
-        fmt = '%+-#' + str(PROC_MIN_FIELD_WIDTH) + 'e'
-    else:
-        fmt = '%+-#' + str(PROC_MIN_FIELD_WIDTH) + '.' + str(ndigits - 1) + 'e'
-    buff = fmt % tmp
+    buff = f"{tmp:<+#{PROC_MIN_FIELD_WIDTH}.{max(0, ndigits - 1)}e}"
     # === WRITE_FLOAT === (macro)
     if ftype != 'G':
         return _output_float(w, d, e, state, ftype, buff, sign_bit, zero_flag, ndigits, edigits)
     else:
         # Perform different actions for G edit descriptors depending on value
         #
         # Generate corresponding I/O format for FMT_G and output.
@@ -375,21 +321,19 @@
 
     # Some hacks to change None to -1 (C convention)
     if w is None:
         w = -1
     if e is None:
         e = -1
     nzero_real = -1
-    sign = _calculate_sign(state, sign_bit)
+
     # Some debug
     if d != 0:
         assert(buff[2] in ['.', ','])
         assert(buff[ndigits + 2] == 'e')
-    # Read in the exponent
-    ex = int(buff[ndigits + 3:]) + 1
     # Handle zero case
     if zero_flag:
         ex = 0
         if PROC_SIGN_ZERO:
             sign = _calculate_sign(state, sign_bit)
         else:
             sign = _calculate_sign(state, False)
@@ -398,14 +342,19 @@
             w = d + 2
         # This case does not include a decimal point
         if (w == 1) and (ft == 'F'):
             if state['incl_plus']:
                 return '*'  # This is ifort behaviour
             else:
                 return '.'  # CHANGED: Was '0'
+    else:
+        # Read in the exponent
+        ex = int(buff[ndigits + 3:]) + 1
+        sign = _calculate_sign(state, sign_bit)
+
     # Get rid of the decimal and the initial sign i.e. normalise the digits
     digits = buff[1] + buff[3:]
     # Find out where to place the decimal point
     if ft == 'F':
         nbefore = ex + state['scale']
         if nbefore < 0:
             nzero = -nbefore
@@ -478,18 +427,18 @@
         i = ndigits
         if int(digits[i]) >= 5:
             # Propagate the carry
             i = i - 1
             while i >= 0:
                 digit = int(digits[i])
                 if digit != 9:
-                    digits = _swapchar(digits, i, str(digit + 1))
+                    digits = _swapchar(digits, i, digit + 1)
                     break
                 else:
-                    digits = _swapchar(digits, i, '0')
+                    digits = _swapchar(digits, i, 0)
                 i = i - 1
             # Did the carry overflow?
             if i < 0:
                 digits = '1' + digits
                 if ft == 'F':
                     if nzero > 0:
                         nzero = nzero - 1
@@ -523,26 +472,15 @@
             # Exponenet width specified, check it is wide enough
             if edigits > e:
                 edigits = -1
             else:
                 edigits = e + 2
     else:
         edigits = 0
-    # Zero values always output as positive, even if the value was egative before rounding
-    i = 0
-    while i < ndigits:
-        if digits[i] != '0':
-            break
-        i = i + 1
-    if i == ndigits:
-        # The output is zero so set sign accordingly
-        if PROC_SIGN_ZERO:
-            sign = _calculate_sign(state, sign_bit)
-        else:
-            sign = _calculate_sign(state, False)
+
     # Pick a field size if none was specified
     if w <= 0:
         w = nbefore + nzero + nafter + 1 + len(sign)
     # Work out how much padding is needed
     nblanks = w - (nbefore + nzero + nafter + edigits + 1)
     if sign != '':
         nblanks = nblanks - 1
@@ -550,86 +488,78 @@
     if G0_NO_BLANKS:  # dtp->u.p.g0_no_blanks
         w = w - nblanks
         nblanks = 0
     # Check value fits in specified width
     if (nblanks < 0) or (edigits == -1):
         return '*' * w
     # See if we have space for a zero before the decimal point
-    if (nbefore == 0) and (nblanks > 0):
-        leadzero = True
+    leadzero = (nbefore == 0) and (nblanks > 0)
+    if leadzero:
         nblanks = nblanks - 1
-    else:
-        leadzero = False
-    out = ''
+
+    out = StringIO()
     # Pad to full field width
     if (nblanks > 0) and not PROC_NO_LEADING_BLANK:  # dtp->u.p.no_leading_blank
-        out = out + ' ' * nblanks
+        out.write(' ' * nblanks)
     # Attach the sign
-    out = out + sign
+    out.write(sign)
     # Add the lead zero if necessary
     if leadzero:
-        out = out + '0'
+        out.write('0')
     # Output portion before the decimal point padded with zeros
     if nbefore > 0:
         if nbefore > ndigits:
-            out = out + digits[:ndigits] + (' ' * (nbefore - ndigits))
+            out.write(digits[:ndigits] + (' ' * (nbefore - ndigits)))
             digits = digits[ndigits:]
             ndigits = 0
         else:
             i = nbefore
-            out = out + digits[:i]
+            out.write(digits[:i])
             digits = digits[i:]
             ndigits = ndigits - i
+
     # Output the decimal point
-    out = out + PROC_DECIMAL_CHAR
+    out.write(PROC_DECIMAL_CHAR)
+
     # Output the leading zeros after the decimal point
     if nzero > 0:
-        out = out + ('0' * nzero)
+        out.write(('0' * nzero))
+
     # Output the digits after the decimal point, padded with zeros
     if nafter > 0:
-        if nafter > ndigits:
-            i = ndigits
-        else:
-            i = nafter
-        zeros = '0' * (nafter - i)
-        out = out + digits[:i] + zeros
-        digits = digits[nafter:]
-        ndigits = ndigits - nafter
+        i = min(nafter, ndigits)
+        out.write(digits[:i])
+        out.write('0' * (nafter - i))
+
     # Output the exponent
     if expchar is not None:
         if expchar != ' ':
-            out = out + expchar
+            out.write(expchar)
             edigits = edigits - 1
-        fmt = '%+0' + str(edigits) + 'd'
-        tmp_buff = fmt % ex
+        tmp_buff = f'{ex:+0{edigits}d}'
         # if not state['blanks_as_zeros']:
         if PROC_NO_LEADING_BLANK:
-            tmp_buf = tmp_buff + (nblanks * ' ')
-        out = out + tmp_buff
-    return out
+            tmp_buff = tmp_buff + (nblanks * ' ')
+        out.write(tmp_buff)
+    return out.getvalue()
 
 
 def _calculate_sign(state, negative_flag):
-    s = ''
     if negative_flag:
-        s = '-'
-    elif state['incl_plus']:
-        s = '+'
-    else:
-        s = ''
-    return s
+        return '-'
+    if state['incl_plus']:
+        return '+'
+    return ''
 
 
-def _swapchar(s, ind, newch):
+def _swapchar(s: str, ind: int, newch: int):
     '''
     Helper function to make chars in a string mutableish
     '''
-    if 0 < ind >= len(s):
-        raise IndexError('index out of range')
-    return s[:ind] + newch + s[ind+1:]
+    return f"{s[:ind]}{newch}{s[ind+1:]}"
 
 
 def _compose_a_string(w, state, val):
     # f77 spec 13.5.11 covers a editing
     val = str(val)
     if w is None:
         output = val
@@ -748,26 +678,26 @@
         s = left_pad(s, m, '0').rjust(w)
     if len(s) > w:
         return w * '*'
     else:
         return s
 
 
-def _write_string(record, sub_string, pos):
+def _write_string(record: StringIO, sub_string: str, pos: int):
     '''Function that actually writes the generated strings to a 'stream'''''
-    new_pos = pos + len(sub_string)
     # pad if required with blanks - i.e. input after a tr edit descriptor - see
     # f77 format sec. 13.5.3
-    if pos > len(record):
-        record = record.ljust(pos)
-        out = record + sub_string
-    elif pos == len(record):
-        out = record + sub_string
-    elif pos < len(record):
-        out = record[:pos] + sub_string + record[new_pos:]
-    return (new_pos, out)
+    record_len = record.tell()
+    if pos > record_len:
+        blanks = " " * (pos - record_len)
+        record.write(blanks)
+    elif pos < record_len:
+        record.seek(max(0, pos))
+
+    record.write(sub_string)
+    return (record.tell(), record)
 
 
 def left_pad(sub_string, width, pad_char):
     # Python 2.3 does not have the character argument to rjust
     padding = pad_char * (width - len(sub_string))
     return padding + sub_string
```

### Comparing `fortranformat-1.2.2/fortranformat/_parser.py` & `fortranformat-2.0.0/fortranformat/_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ._lexer import Token
 from ._edit_descriptors import *
-from ._exceptions import *
+from ._exceptions import InvalidFormat
 from . import config
 
 def parser(tokens, version=None):
     # Parse the full edit descriptors
     eds = _parse_tokens(tokens, reversion=False, version=None)
     # Parse the edit descriptors used for the reversion of format control 
     # (F95 format 12.2.2)
```

### Comparing `fortranformat-1.2.2/fortranformat/config.py` & `fortranformat-2.0.0/fortranformat/config.py`

 * *Files identical despite different names*

### Comparing `fortranformat-1.2.2/fortranformat.egg-info/PKG-INFO` & `fortranformat-2.0.0/fortranformat.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fortranformat
-Version: 1.2.2
+Version: 2.0.0
 Summary: Mimics Fortran textual IO in Python
 Home-page: https://github.com/brendanarnold/py-fortranformat
 Author: Brendan Arnold
 Author-email: brendanarnold@gmail.com
 License: UNKNOWN
 Description: # FORTRAN format interpreter for Python
         
@@ -71,14 +71,18 @@
         
         Note that some of the F output edit descriptors fail due to limitations in floating point number representation
         
         To run a reduced test suite where time and resources are limited, use the following
         
         `make runminimaltests`
         
+        To run a performance test, which currently only covers the reading and writing of floats, use the following
+        
+        `make runperformancetests`
+        
         ### Deploying a new package version
         
         Update versions in `setup.py` and `__init__.py`
         
         Update `CHANGELOG.md`
         
         To create a local build to test run ...
@@ -108,13 +112,12 @@
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Fortran
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Text Processing :: General
 Classifier: Topic :: Software Development :: Interpreters
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
```

### Comparing `fortranformat-1.2.2/setup.py` & `fortranformat-2.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,30 +5,29 @@
 README = ''
 with open(HERE + '/README.md') as fh:
     README = fh.read()
 
 setup(
     name='fortranformat',
     packages=['fortranformat'],
-    version='1.2.2',
+    version='2.0.0',
     description='Mimics Fortran textual IO in Python',
     author='Brendan Arnold',
     author_email='brendanarnold@gmail.com',
     url='https://github.com/brendanarnold/py-fortranformat',
     keywords=['fortran', 'io', 'interface', 'format'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Environment :: Console',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Programming Language :: Fortran',
-        'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 3',
         'Topic :: Text Processing :: General',
         'Topic :: Software Development :: Interpreters',
         'Topic :: Scientific/Engineering',
     ],
     long_description=README,
     long_description_content_type="text/markdown"
```

