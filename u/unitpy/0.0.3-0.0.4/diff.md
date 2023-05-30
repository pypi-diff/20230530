# Comparing `tmp/unitpy-0.0.3.tar.gz` & `tmp/unitpy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitpy-0.0.3.tar", last modified: Tue Apr  4 02:22:01 2023, max compression
+gzip compressed data, was "C:\Users\nicep\Desktop\Reseach_Post\python\unitpy\dist\.tmp-qd1d4vei\unitpy-0.0.4.tar", last modified: Tue May 30 14:30:14 2023, max compression
```

## Comparing `unitpy-0.0.3.tar` & `unitpy-0.0.4.tar`

### file list

```diff
@@ -1,42 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 02:22:01.610456 unitpy-0.0.3/
--rw-rw-rw-   0        0        0     1497 2023-04-01 17:13:34.000000 unitpy-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     4288 2023-04-04 02:22:01.610456 unitpy-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3487 2023-04-03 23:31:47.000000 unitpy-0.0.3/README.md
--rw-rw-rw-   0        0        0      307 2023-04-03 23:31:47.000000 unitpy-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      969 2023-04-04 02:22:01.612455 unitpy-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0       75 2023-04-01 17:13:34.000000 unitpy-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-04 02:22:01.575819 unitpy-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-04-04 02:22:01.582824 unitpy-0.0.3/src/unitpy/
--rw-rw-rw-   0        0        0      336 2023-04-03 23:31:47.000000 unitpy-0.0.3/src/unitpy/__init__.py
--rw-rw-rw-   0        0        0      454 2023-04-03 00:17:42.000000 unitpy-0.0.3/src/unitpy/config.py
--rw-rw-rw-   0        0        0    18876 2023-04-03 23:31:47.000000 unitpy-0.0.3/src/unitpy/core.py
-drwxrwxrwx   0        0        0        0 2023-04-04 02:22:01.603945 unitpy-0.0.3/src/unitpy/definitions/
--rw-rw-rw-   0        0        0        0 2023-04-01 17:13:34.000000 unitpy-0.0.3/src/unitpy/definitions/__init__.py
--rw-rw-rw-   0        0        0     2917 2023-04-01 23:56:36.000000 unitpy-0.0.3/src/unitpy/definitions/constants.py
--rw-rw-rw-   0        0        0     7224 2023-04-03 23:31:47.000000 unitpy-0.0.3/src/unitpy/definitions/dimensions.py
--rw-rw-rw-   0        0        0     1511 2023-04-04 02:20:26.000000 unitpy-0.0.3/src/unitpy/definitions/entry.py
--rw-rw-rw-   0        0        0     5904 2023-04-04 02:21:19.000000 unitpy-0.0.3/src/unitpy/definitions/ledger.py
--rw-rw-rw-   0        0        0      797 2023-04-01 17:13:34.000000 unitpy-0.0.3/src/unitpy/definitions/metric.py
--rw-rw-rw-   0        0        0     1362 2023-04-02 20:54:32.000000 unitpy-0.0.3/src/unitpy/definitions/prefix.py
--rw-rw-rw-   0        0        0    16491 2023-04-04 02:20:26.000000 unitpy-0.0.3/src/unitpy/definitions/unit_NIST.py
--rw-rw-rw-   0        0        0     6166 2023-04-03 23:31:47.000000 unitpy-0.0.3/src/unitpy/definitions/unit_base.py
--rw-rw-rw-   0        0        0     3545 2023-04-03 23:31:47.000000 unitpy-0.0.3/src/unitpy/definitions/unit_derived.py
--rw-rw-rw-   0        0        0      925 2023-04-04 02:21:19.000000 unitpy-0.0.3/src/unitpy/definitions/unit_extra.py
-drwxrwxrwx   0        0        0        0 2023-04-04 02:22:01.606457 unitpy-0.0.3/src/unitpy/utils/
--rw-rw-rw-   0        0        0        0 2023-04-01 17:13:34.000000 unitpy-0.0.3/src/unitpy/utils/__init__.py
--rw-rw-rw-   0        0        0     1821 2023-04-03 23:31:47.000000 unitpy-0.0.3/src/unitpy/utils/equation_formating.py
--rw-rw-rw-   0        0        0     5005 2023-04-03 23:31:47.000000 unitpy-0.0.3/src/unitpy/utils/parsing.py
--rw-rw-rw-   0        0        0      356 2023-04-03 23:31:47.000000 unitpy-0.0.3/src/unitpy/utils/string_converter.py
-drwxrwxrwx   0        0        0        0 2023-04-04 02:22:01.595954 unitpy-0.0.3/src/unitpy.egg-info/
--rw-rw-rw-   0        0        0     4288 2023-04-04 02:22:01.000000 unitpy-0.0.3/src/unitpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      984 2023-04-04 02:22:01.000000 unitpy-0.0.3/src/unitpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 02:22:01.000000 unitpy-0.0.3/src/unitpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-01 23:51:15.000000 unitpy-0.0.3/src/unitpy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-04-04 02:22:01.000000 unitpy-0.0.3/src/unitpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-04 02:22:01.610456 unitpy-0.0.3/tests/
--rw-rw-rw-   0        0        0      684 2023-04-03 23:31:47.000000 unitpy-0.0.3/tests/test_define_quantity.py
--rw-rw-rw-   0        0        0     1110 2023-04-03 23:31:47.000000 unitpy-0.0.3/tests/test_define_unit.py
--rw-rw-rw-   0        0        0     1340 2023-04-03 23:31:47.000000 unitpy-0.0.3/tests/test_dimensions.py
--rw-rw-rw-   0        0        0     1927 2023-04-02 17:23:10.000000 unitpy-0.0.3/tests/test_parsing_unit.py
--rw-rw-rw-   0        0        0     2748 2023-04-03 23:31:47.000000 unitpy-0.0.3/tests/test_quanitiy_math_operations.py
--rw-rw-rw-   0        0        0      756 2023-04-02 21:11:03.000000 unitpy-0.0.3/tests/test_unit_conversion.py
+drwxrwxrwx   0        0        0        0 2023-05-30 14:30:14.000000 unitpy-0.0.4/
+-rw-rw-rw-   0        0        0     1497 2023-04-03 12:39:22.000000 unitpy-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     4288 2023-05-30 14:30:14.000000 unitpy-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3487 2023-04-03 20:27:46.000000 unitpy-0.0.4/README.md
+-rw-rw-rw-   0        0        0      307 2023-04-03 17:45:31.000000 unitpy-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      969 2023-05-30 14:30:14.000000 unitpy-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0       75 2023-04-03 12:39:22.000000 unitpy-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 14:30:14.000000 unitpy-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-30 14:30:14.000000 unitpy-0.0.4/src/unitpy/
+-rw-rw-rw-   0        0        0      336 2023-04-03 14:05:31.000000 unitpy-0.0.4/src/unitpy/__init__.py
+-rw-rw-rw-   0        0        0      454 2023-04-03 12:39:22.000000 unitpy-0.0.4/src/unitpy/config.py
+-rw-rw-rw-   0        0        0    19021 2023-05-30 14:23:24.000000 unitpy-0.0.4/src/unitpy/core.py
+drwxrwxrwx   0        0        0        0 2023-05-30 14:30:14.000000 unitpy-0.0.4/src/unitpy/definitions/
+-rw-rw-rw-   0        0        0        0 2023-04-03 12:39:22.000000 unitpy-0.0.4/src/unitpy/definitions/__init__.py
+-rw-rw-rw-   0        0        0     2917 2023-04-03 12:39:22.000000 unitpy-0.0.4/src/unitpy/definitions/constants.py
+-rw-rw-rw-   0        0        0     7224 2023-04-03 16:57:14.000000 unitpy-0.0.4/src/unitpy/definitions/dimensions.py
+-rw-rw-rw-   0        0        0     1511 2023-04-03 12:39:22.000000 unitpy-0.0.4/src/unitpy/definitions/entry.py
+-rw-rw-rw-   0        0        0     5681 2023-04-03 17:05:55.000000 unitpy-0.0.4/src/unitpy/definitions/ledger.py
+-rw-rw-rw-   0        0        0      797 2023-04-03 12:39:22.000000 unitpy-0.0.4/src/unitpy/definitions/metric.py
+-rw-rw-rw-   0        0        0     1362 2023-04-03 12:39:22.000000 unitpy-0.0.4/src/unitpy/definitions/prefix.py
+-rw-rw-rw-   0        0        0    16491 2023-04-03 12:39:22.000000 unitpy-0.0.4/src/unitpy/definitions/unit_NIST.py
+-rw-rw-rw-   0        0        0     6166 2023-04-03 14:27:27.000000 unitpy-0.0.4/src/unitpy/definitions/unit_base.py
+-rw-rw-rw-   0        0        0     3545 2023-04-03 16:16:53.000000 unitpy-0.0.4/src/unitpy/definitions/unit_derived.py
+drwxrwxrwx   0        0        0        0 2023-05-30 14:30:14.000000 unitpy-0.0.4/src/unitpy/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-03 12:39:22.000000 unitpy-0.0.4/src/unitpy/utils/__init__.py
+-rw-rw-rw-   0        0        0     1821 2023-04-03 13:22:12.000000 unitpy-0.0.4/src/unitpy/utils/equation_formating.py
+-rw-rw-rw-   0        0        0     5005 2023-04-03 15:05:13.000000 unitpy-0.0.4/src/unitpy/utils/parsing.py
+-rw-rw-rw-   0        0        0      356 2023-04-03 13:51:24.000000 unitpy-0.0.4/src/unitpy/utils/string_converter.py
+drwxrwxrwx   0        0        0        0 2023-05-30 14:30:14.000000 unitpy-0.0.4/src/unitpy.egg-info/
+-rw-rw-rw-   0        0        0     4288 2023-05-30 14:30:14.000000 unitpy-0.0.4/src/unitpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      947 2023-05-30 14:30:14.000000 unitpy-0.0.4/src/unitpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 14:30:14.000000 unitpy-0.0.4/src/unitpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-03 12:59:41.000000 unitpy-0.0.4/src/unitpy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-05-30 14:30:14.000000 unitpy-0.0.4/src/unitpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 14:30:14.000000 unitpy-0.0.4/tests/
+-rw-rw-rw-   0        0        0      684 2023-04-03 17:57:48.000000 unitpy-0.0.4/tests/test_define_quantity.py
+-rw-rw-rw-   0        0        0     1110 2023-04-03 18:03:53.000000 unitpy-0.0.4/tests/test_define_unit.py
+-rw-rw-rw-   0        0        0     1340 2023-04-03 16:57:59.000000 unitpy-0.0.4/tests/test_dimensions.py
+-rw-rw-rw-   0        0        0     1927 2023-04-03 12:39:22.000000 unitpy-0.0.4/tests/test_parsing_unit.py
+-rw-rw-rw-   0        0        0     2865 2023-05-30 14:25:13.000000 unitpy-0.0.4/tests/test_quanitiy_math_operations.py
+-rw-rw-rw-   0        0        0      756 2023-04-03 12:39:22.000000 unitpy-0.0.4/tests/test_unit_conversion.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `unitpy-0.0.3/LICENSE.txt` & `unitpy-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.3/PKG-INFO` & `unitpy-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitpy
-Version: 0.0.3
+Version: 0.0.4
 Summary: Working with scientific units in python.
 Home-page: https://github.com/dylanwal/unitpy
 Author: Dylan Walsh
 License: BSD
 Platform: any
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `unitpy-0.0.3/README.md` & `unitpy-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.3/setup.cfg` & `unitpy-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2075 6e69 7470 790d 0a76 6572 7369   = unitpy..versi
-00000020: 6f6e 203d 2030 2e30 2e33 0d0a 6465 7363  on = 0.0.3..desc
+00000020: 6f6e 203d 2030 2e30 2e34 0d0a 6465 7363  on = 0.0.4..desc
 00000030: 7269 7074 696f 6e20 3d20 576f 726b 696e  ription = Workin
 00000040: 6720 7769 7468 2073 6369 656e 7469 6669  g with scientifi
 00000050: 6320 756e 6974 7320 696e 2070 7974 686f  c units in pytho
 00000060: 6e2e 0d0a 6c6f 6e67 5f64 6573 6372 6970  n...long_descrip
 00000070: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 00000080: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
 00000090: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
```

### Comparing `unitpy-0.0.3/src/unitpy/core.py` & `unitpy-0.0.4/src/unitpy/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import itertools
 import math
 import copy
+import typing
 
 from unitpy.definitions.dimensions import Dimension
 from unitpy.definitions.unit_base import BaseSet
 from unitpy.definitions.entry import Entry
 from unitpy.definitions.ledger import ledger
 from unitpy.utils.equation_formating import equation_formater
 
@@ -226,15 +227,15 @@
         value = value / self.multiplier - self.offset
         return value
 
 
 ## Quantity ## noqa
 #######################################################################################################################
 #######################################################################################################################
-class Quantity:
+class Quantity(typing.SupportsRound):
     _ledger = ledger
 
     __slots__ = ("_unit", "_base_value")
 
     def __new__(cls, value: str | int | float, unit: Unit | BaseSet | str = None):
         if isinstance(value, str):
             from unitpy.utils.parsing import parse_quantity
@@ -438,14 +439,17 @@
 
     def __abs__(self) -> Quantity:
         return Quantity(abs(self._value), self.unit)
 
     def __ceil__(self) -> Quantity:
         return Quantity(math.ceil(self._value), self.unit)
 
+    def __round__(self, n: int = 0) -> Quantity:
+        return Quantity(round(self._value), self.unit)
+
     @property
     def _value(self):
         return self.unit.from_base_value(self._base_value)
 
     @property
     def v(self) -> int | float:
         return self.value
```

### Comparing `unitpy-0.0.3/src/unitpy/definitions/constants.py` & `unitpy-0.0.4/src/unitpy/definitions/constants.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.3/src/unitpy/definitions/dimensions.py` & `unitpy-0.0.4/src/unitpy/definitions/dimensions.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.3/src/unitpy/definitions/entry.py` & `unitpy-0.0.4/src/unitpy/definitions/entry.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.3/src/unitpy/definitions/ledger.py` & `unitpy-0.0.4/src/unitpy/definitions/ledger.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import unitpy.definitions.dimensions as dim_
 import unitpy.definitions.prefix as prefix_
 from unitpy.definitions.entry import Entry
 
 import unitpy.definitions.unit_base as bases
 import unitpy.definitions.unit_derived as unit_derived
 import unitpy.definitions.unit_NIST as unit_NIST
-import unitpy.definitions.unit_extra as unit_extra
 
 
 class Ledger:
     """ The leger is a grouping all units. """
     _cache = False
     dimensions = dim_.dimensions
     prefixes = prefix_.prefixes
@@ -60,15 +59,15 @@
                                  f"\nsecond one: {repr(entry)}")
 
             self.units.append(entry)
             self._lookup[entry.label] = entry
             self._lookup[entry.abbr] = entry
             for label in entry.additional_labels:
                 if label in self._lookup:
-                    raise ValueError(f"Duplicate ledger entry: {label}."
+                    raise ValueError(f"Duplicate ledger entry."
                                      f"\nexisting: {repr(self._lookup[entry.label])} "
                                      f"\nsecond one: {repr(entry)}")
                 self._lookup[label] = entry
 
     def _save_cache(self):
         a = self.symbols  # cause it to build
 
@@ -165,24 +164,16 @@
 add_derived_quantities()
 add_core()
 
 
 ## add unofficial NIST units ## noqa
 #######################################################################################################################
 
-def add_extra_quantities():
-    for entry in unit_extra.extra_quantities.values():
-        ledger.add_unit(entry)
-
-
-add_extra_quantities()
-
 additional_units_with_prefix = {
-    "liter",
-    "molar",
+    "liter"
 }
 
 
 def add_additional_units_with_prefix():
     for unit in additional_units_with_prefix:
         entry = ledger.get_entry(unit)
         add_with_prefix(entry)
```

### Comparing `unitpy-0.0.3/src/unitpy/definitions/metric.py` & `unitpy-0.0.4/src/unitpy/definitions/metric.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.3/src/unitpy/definitions/prefix.py` & `unitpy-0.0.4/src/unitpy/definitions/prefix.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.3/src/unitpy/definitions/unit_NIST.py` & `unitpy-0.0.4/src/unitpy/definitions/unit_NIST.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.3/src/unitpy/definitions/unit_base.py` & `unitpy-0.0.4/src/unitpy/definitions/unit_base.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.3/src/unitpy/definitions/unit_derived.py` & `unitpy-0.0.4/src/unitpy/definitions/unit_derived.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.3/src/unitpy/utils/equation_formating.py` & `unitpy-0.0.4/src/unitpy/utils/equation_formating.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.3/src/unitpy/utils/parsing.py` & `unitpy-0.0.4/src/unitpy/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.3/src/unitpy.egg-info/PKG-INFO` & `unitpy-0.0.4/src/unitpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitpy
-Version: 0.0.3
+Version: 0.0.4
 Summary: Working with scientific units in python.
 Home-page: https://github.com/dylanwal/unitpy
 Author: Dylan Walsh
 License: BSD
 Platform: any
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `unitpy-0.0.3/src/unitpy.egg-info/SOURCES.txt` & `unitpy-0.0.4/src/unitpy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 src/unitpy/definitions/entry.py
 src/unitpy/definitions/ledger.py
 src/unitpy/definitions/metric.py
 src/unitpy/definitions/prefix.py
 src/unitpy/definitions/unit_NIST.py
 src/unitpy/definitions/unit_base.py
 src/unitpy/definitions/unit_derived.py
-src/unitpy/definitions/unit_extra.py
 src/unitpy/utils/__init__.py
 src/unitpy/utils/equation_formating.py
 src/unitpy/utils/parsing.py
 src/unitpy/utils/string_converter.py
 tests/test_define_quantity.py
 tests/test_define_unit.py
 tests/test_dimensions.py
```

### Comparing `unitpy-0.0.3/tests/test_define_quantity.py` & `unitpy-0.0.4/tests/test_define_quantity.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.3/tests/test_define_unit.py` & `unitpy-0.0.4/tests/test_define_unit.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.3/tests/test_dimensions.py` & `unitpy-0.0.4/tests/test_dimensions.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.3/tests/test_parsing_unit.py` & `unitpy-0.0.4/tests/test_parsing_unit.py`

 * *Files identical despite different names*

### Comparing `unitpy-0.0.3/tests/test_quanitiy_math_operations.py` & `unitpy-0.0.4/tests/test_quanitiy_math_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,48 +10,48 @@
     (("1.1 cm**3", "1 ml"), "L", 0.0021, 0.0001),
     (("1 degC", "1 K"), "K", 275.15, 273.15),
 
 )
 
 
 @pytest.mark.parametrize("case", cases)
-def test_math_add(case):
+def test_math_add(case: tuple):
     text, unit, value, _ = case
     quantities = [Q(t) for t in text]
     sum_ = quantities[0]
     for quant in quantities[1:]:
         sum_ = sum_ + quant
 
     assert math.isclose(sum_.to(unit).v, value, rel_tol=1e-5)
 
 
 @pytest.mark.parametrize("case", cases)
-def test_math_add_inplace(case):
+def test_math_add_inplace(case: tuple):
     text, unit, value, _ = case
     quantities = [Q(t) for t in text]
     sum_ = quantities[0]
     for quant in quantities[1:]:
         sum_ += quant
 
     assert math.isclose(sum_.to(unit).v, value, rel_tol=1e-5)
 
 
 @pytest.mark.parametrize("case", cases)
-def test_math_sub(case):
+def test_math_sub(case: tuple):
     text, unit, _, value = case
     quantities = [Q(t) for t in text]
     sum_ = quantities[0]
     for quant in quantities[1:]:
         sum_ -= quant
 
     assert math.isclose(sum_.to(unit).v, value, rel_tol=1e-5)
 
 
 @pytest.mark.parametrize("case", cases)
-def test_math_sub_inplace(case):
+def test_math_sub_inplace(case: tuple):
     text, unit, _, value = case
     quantities = [Q(t) for t in text]
     sum_ = quantities[0]
     for quant in quantities[1:]:
         sum_ = sum_ - quant
 
     assert math.isclose(sum_.to(unit).v, value, rel_tol=1e-5)
@@ -117,7 +117,11 @@
         Q("1 m") <= Q("1 s")
 
 
 def test_compare_error_e():
     with pytest.raises(ValueError) as _:
         Q("1 m") == Q("1 s")
 
+
+def test_round():
+    q = Q("1.2345 ft")
+    assert (round(q) == Q("1 ft")) is True
```

### Comparing `unitpy-0.0.3/tests/test_unit_conversion.py` & `unitpy-0.0.4/tests/test_unit_conversion.py`

 * *Files identical despite different names*

