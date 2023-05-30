# Comparing `tmp/clevertable-3.0.0.tar.gz` & `tmp/clevertable-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clevertable-3.0.0.tar", last modified: Mon May 29 18:30:31 2023, max compression
+gzip compressed data, was "clevertable-3.0.1.tar", last modified: Tue May 30 06:15:42 2023, max compression
```

## Comparing `clevertable-3.0.0.tar` & `clevertable-3.0.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 18:30:31.661082 clevertable-3.0.0/
--rw-rw-rw-   0        0        0     1086 2023-04-21 11:55:46.000000 clevertable-3.0.0/LICENSE
--rw-rw-rw-   0        0        0    35991 2023-05-29 18:30:31.661082 clevertable-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    34221 2023-05-29 18:29:05.000000 clevertable-3.0.0/README.md
--rw-rw-rw-   0        0        0     1306 2023-05-29 18:29:58.000000 clevertable-3.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-29 18:30:31.661082 clevertable-3.0.0/setup.cfg
--rw-rw-rw-   0        0        0      230 2023-04-21 12:00:42.000000 clevertable-3.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-29 18:30:31.617707 clevertable-3.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-29 18:30:31.661082 clevertable-3.0.0/src/clevertable/
--rw-rw-rw-   0        0        0     3518 2023-05-29 17:24:28.000000 clevertable-3.0.0/src/clevertable/Binary.py
--rw-rw-rw-   0        0        0      268 2023-05-29 17:07:53.000000 clevertable-3.0.0/src/clevertable/Const.py
--rw-rw-rw-   0        0        0     3016 2023-05-29 17:07:53.000000 clevertable-3.0.0/src/clevertable/ConversionProfile.py
--rw-rw-rw-   0        0        0     3765 2023-05-29 17:37:25.000000 clevertable-3.0.0/src/clevertable/Converter.py
--rw-rw-rw-   0        0        0     4367 2023-05-29 17:37:25.000000 clevertable-3.0.0/src/clevertable/DataFrameProfile.py
--rw-rw-rw-   0        0        0     1018 2023-05-29 18:08:53.000000 clevertable-3.0.0/src/clevertable/Enumerate.py
--rw-rw-rw-   0        0        0      291 2023-05-29 17:07:53.000000 clevertable-3.0.0/src/clevertable/Flatten.py
--rw-rw-rw-   0        0        0     3854 2023-05-29 17:24:28.000000 clevertable-3.0.0/src/clevertable/Float.py
--rw-rw-rw-   0        0        0      896 2023-05-29 17:37:25.000000 clevertable-3.0.0/src/clevertable/ForEach.py
--rw-rw-rw-   0        0        0     4976 2023-05-29 17:37:25.000000 clevertable-3.0.0/src/clevertable/Function.py
--rw-rw-rw-   0        0        0      213 2023-05-29 17:07:53.000000 clevertable-3.0.0/src/clevertable/Id.py
--rw-rw-rw-   0        0        0      369 2023-05-29 17:43:58.000000 clevertable-3.0.0/src/clevertable/Ignore.py
--rw-rw-rw-   0        0        0     3021 2023-05-29 17:55:13.000000 clevertable-3.0.0/src/clevertable/Infer.py
--rw-rw-rw-   0        0        0      398 2023-05-29 17:11:23.000000 clevertable-3.0.0/src/clevertable/Label.py
--rw-rw-rw-   0        0        0     3302 2023-05-29 17:07:53.000000 clevertable-3.0.0/src/clevertable/List.py
--rw-rw-rw-   0        0        0     1566 2023-05-29 18:13:39.000000 clevertable-3.0.0/src/clevertable/Map.py
--rw-rw-rw-   0        0        0     1558 2023-05-29 17:59:47.000000 clevertable-3.0.0/src/clevertable/OneHot.py
--rw-rw-rw-   0        0        0     1830 2023-05-29 17:43:58.000000 clevertable-3.0.0/src/clevertable/Parallel.py
--rw-rw-rw-   0        0        0     2877 2023-05-29 17:07:53.000000 clevertable-3.0.0/src/clevertable/Pipeline.py
--rw-rw-rw-   0        0        0     9269 2023-05-29 17:50:54.000000 clevertable-3.0.0/src/clevertable/RecordProfile.py
--rw-rw-rw-   0        0        0      843 2023-05-29 17:51:55.000000 clevertable-3.0.0/src/clevertable/Split.py
--rw-rw-rw-   0        0        0     3576 2023-05-29 17:18:36.000000 clevertable-3.0.0/src/clevertable/StrictFunction.py
--rw-rw-rw-   0        0        0      991 2023-05-29 17:52:36.000000 clevertable-3.0.0/src/clevertable/Strip.py
--rw-rw-rw-   0        0        0     1194 2023-05-29 17:18:36.000000 clevertable-3.0.0/src/clevertable/Transpose.py
--rw-rw-rw-   0        0        0     2769 2023-05-29 17:07:53.000000 clevertable-3.0.0/src/clevertable/Try.py
--rw-rw-rw-   0        0        0      716 2023-05-29 18:29:58.000000 clevertable-3.0.0/src/clevertable/__init__.py
--rw-rw-rw-   0        0        0     1271 2023-05-29 17:07:53.000000 clevertable-3.0.0/src/clevertable/__main__.py
--rw-rw-rw-   0        0        0     2501 2023-05-29 17:43:58.000000 clevertable-3.0.0/src/clevertable/_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-29 18:30:31.661082 clevertable-3.0.0/src/clevertable.egg-info/
--rw-rw-rw-   0        0        0    35991 2023-05-29 18:30:31.000000 clevertable-3.0.0/src/clevertable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1044 2023-05-29 18:30:31.000000 clevertable-3.0.0/src/clevertable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 18:30:31.000000 clevertable-3.0.0/src/clevertable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-05-29 18:30:31.000000 clevertable-3.0.0/src/clevertable.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       56 2023-05-29 18:30:31.000000 clevertable-3.0.0/src/clevertable.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-29 18:30:31.000000 clevertable-3.0.0/src/clevertable.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 06:15:42.807304 clevertable-3.0.1/
+-rw-rw-rw-   0        0        0     1086 2023-04-21 11:55:46.000000 clevertable-3.0.1/LICENSE
+-rw-rw-rw-   0        0        0    35991 2023-05-30 06:15:42.807304 clevertable-3.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    34221 2023-05-29 18:29:05.000000 clevertable-3.0.1/README.md
+-rw-rw-rw-   0        0        0     1292 2023-05-30 06:14:55.000000 clevertable-3.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-30 06:15:42.807304 clevertable-3.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      230 2023-04-21 12:00:42.000000 clevertable-3.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 06:15:42.744286 clevertable-3.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-30 06:15:42.791663 clevertable-3.0.1/src/clevertable/
+-rw-rw-rw-   0        0        0     3518 2023-05-29 17:24:28.000000 clevertable-3.0.1/src/clevertable/Binary.py
+-rw-rw-rw-   0        0        0      268 2023-05-29 17:07:53.000000 clevertable-3.0.1/src/clevertable/Const.py
+-rw-rw-rw-   0        0        0     3016 2023-05-29 17:07:53.000000 clevertable-3.0.1/src/clevertable/ConversionProfile.py
+-rw-rw-rw-   0        0        0     3765 2023-05-29 17:37:25.000000 clevertable-3.0.1/src/clevertable/Converter.py
+-rw-rw-rw-   0        0        0     4367 2023-05-29 17:37:25.000000 clevertable-3.0.1/src/clevertable/DataFrameProfile.py
+-rw-rw-rw-   0        0        0     1018 2023-05-29 18:08:53.000000 clevertable-3.0.1/src/clevertable/Enumerate.py
+-rw-rw-rw-   0        0        0      291 2023-05-29 17:07:53.000000 clevertable-3.0.1/src/clevertable/Flatten.py
+-rw-rw-rw-   0        0        0     3297 2023-05-30 06:09:36.000000 clevertable-3.0.1/src/clevertable/Float.py
+-rw-rw-rw-   0        0        0      896 2023-05-29 17:37:25.000000 clevertable-3.0.1/src/clevertable/ForEach.py
+-rw-rw-rw-   0        0        0     4976 2023-05-29 17:37:25.000000 clevertable-3.0.1/src/clevertable/Function.py
+-rw-rw-rw-   0        0        0      213 2023-05-29 17:07:53.000000 clevertable-3.0.1/src/clevertable/Id.py
+-rw-rw-rw-   0        0        0      369 2023-05-29 17:43:58.000000 clevertable-3.0.1/src/clevertable/Ignore.py
+-rw-rw-rw-   0        0        0     3063 2023-05-30 06:02:41.000000 clevertable-3.0.1/src/clevertable/Infer.py
+-rw-rw-rw-   0        0        0      398 2023-05-29 17:11:23.000000 clevertable-3.0.1/src/clevertable/Label.py
+-rw-rw-rw-   0        0        0     3302 2023-05-29 17:07:53.000000 clevertable-3.0.1/src/clevertable/List.py
+-rw-rw-rw-   0        0        0     1566 2023-05-29 18:13:39.000000 clevertable-3.0.1/src/clevertable/Map.py
+-rw-rw-rw-   0        0        0     1558 2023-05-29 17:59:47.000000 clevertable-3.0.1/src/clevertable/OneHot.py
+-rw-rw-rw-   0        0        0     1830 2023-05-29 17:43:58.000000 clevertable-3.0.1/src/clevertable/Parallel.py
+-rw-rw-rw-   0        0        0     2877 2023-05-29 17:07:53.000000 clevertable-3.0.1/src/clevertable/Pipeline.py
+-rw-rw-rw-   0        0        0     9269 2023-05-29 17:50:54.000000 clevertable-3.0.1/src/clevertable/RecordProfile.py
+-rw-rw-rw-   0        0        0      843 2023-05-29 17:51:55.000000 clevertable-3.0.1/src/clevertable/Split.py
+-rw-rw-rw-   0        0        0     3576 2023-05-29 17:18:36.000000 clevertable-3.0.1/src/clevertable/StrictFunction.py
+-rw-rw-rw-   0        0        0      991 2023-05-29 17:52:36.000000 clevertable-3.0.1/src/clevertable/Strip.py
+-rw-rw-rw-   0        0        0     1194 2023-05-29 17:18:36.000000 clevertable-3.0.1/src/clevertable/Transpose.py
+-rw-rw-rw-   0        0        0     2769 2023-05-29 17:07:53.000000 clevertable-3.0.1/src/clevertable/Try.py
+-rw-rw-rw-   0        0        0      716 2023-05-30 06:14:55.000000 clevertable-3.0.1/src/clevertable/__init__.py
+-rw-rw-rw-   0        0        0     1271 2023-05-29 17:07:53.000000 clevertable-3.0.1/src/clevertable/__main__.py
+-rw-rw-rw-   0        0        0     2501 2023-05-29 17:43:58.000000 clevertable-3.0.1/src/clevertable/_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-30 06:15:42.807304 clevertable-3.0.1/src/clevertable.egg-info/
+-rw-rw-rw-   0        0        0    35991 2023-05-30 06:15:42.000000 clevertable-3.0.1/src/clevertable.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1044 2023-05-30 06:15:42.000000 clevertable-3.0.1/src/clevertable.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 06:15:42.000000 clevertable-3.0.1/src/clevertable.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-05-30 06:15:42.000000 clevertable-3.0.1/src/clevertable.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       50 2023-05-30 06:15:42.000000 clevertable-3.0.1/src/clevertable.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-30 06:15:42.000000 clevertable-3.0.1/src/clevertable.egg-info/top_level.txt
```

### Comparing `clevertable-3.0.0/LICENSE` & `clevertable-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.0/PKG-INFO` & `clevertable-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clevertable
-Version: 3.0.0
+Version: 3.0.1
 Summary: Low effort conversion of tabular data into numerical values.
 Author: Tom Mohr
 License: MIT License
         
         Copyright (c) 2023 Tom Mohr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `clevertable-3.0.0/README.md` & `clevertable-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.0/pyproject.toml` & `clevertable-3.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clevertable"
-version = "3.0.0"
+version = "3.0.1"
 description = "Low effort conversion of tabular data into numerical values."
 readme = "README.md"
 authors = [{ name = "Tom Mohr" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["parser", "converter", "numerical"]
 dependencies = [
     "numpy",
     "pandas",
     "openpyxl",  # needed for xlsx support
-    "scipy",
 ]
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = ["bumpver", "twine", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/tom-mohr/clevertable"
 
 [project.scripts]
 clevertable = "clevertable.__main__:main"
 
 [tool.bumpver]
-current_version = "3.0.0"
+current_version = "3.0.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `clevertable-3.0.0/src/clevertable/Binary.py` & `clevertable-3.0.1/src/clevertable/Binary.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.0/src/clevertable/ConversionProfile.py` & `clevertable-3.0.1/src/clevertable/ConversionProfile.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.0/src/clevertable/Converter.py` & `clevertable-3.0.1/src/clevertable/Converter.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.0/src/clevertable/DataFrameProfile.py` & `clevertable-3.0.1/src/clevertable/DataFrameProfile.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.0/src/clevertable/Enumerate.py` & `clevertable-3.0.1/src/clevertable/Enumerate.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.0/src/clevertable/Float.py` & `clevertable-3.0.1/src/clevertable/Float.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,104 +1,86 @@
 from __future__ import annotations
 
-from typing import Literal
+import math
+from collections import Counter
+from typing import Literal, Iterable
 
-from numpy import mean, median, isinf, isnan, isfinite, number
-from scipy.stats import mode
+from numpy import mean, median
+from math import isfinite
 
 from .Converter import Converter
 
 
-def _try_float(val: any) -> float | None:
-    try:
-        x = float(val)
-    except (TypeError, ValueError, OverflowError):
-        return None
-
-    # x is a float, but is it a "good" float?
-    if isinf(x):
-        return None
-    if isnan(x):
-        return None
-
-    # all checks passed
-    return x
-
-
-def _is_number(val: any):
-    try:
-        _check_number(val)
-        return True
-    except ValueError:
-        return False
-
-
-def _check_number(val: any) -> any:
-    """Returns the given value if it is a number, otherwise raises a ValueError."""
-    if not isinstance(val, (int, float, number)):
-        raise ValueError(f"Value '{val}' is not a number")
-    if not isfinite(val):
-        raise ValueError(f"Value '{val}' is not a finite number")
-    return val
+def _mode(a: Iterable[float]) -> float:
+    counter = Counter(a)
+    mode, freq = counter.most_common(1)[0]
+    return mode
 
 
 class Float(Converter):
 
     def __init__(self, default: float | Literal["mean", "median", "mode"] = None):
         """
         Simple conversion to floats.
 
         - If a string is encountered, it tries to parse it.
         - If a number is encountered, it simply ensures that it is of type float.
         - If an infinite number is encountered, it is replaced with the given default value.
         - If any other value is encountered, it is replaced with the given default value.
         """
-        if default is not None:
-            # check type of default value
-            if default not in ("mean", "median", "mode"):
-                if not _is_number(default):
-                    raise ValueError(f"Invalid default value '{default}'.")
-
         self.__default_value = default
 
     @property
     def default(self):
         return self.__default_value
 
     def fit(self, rows: list[tuple]):
 
         values = [row[0] for row in rows]  # unpack 1-element rows
 
         if self.__default_value in ("mean", "median", "mode"):
             # replace default value with the corresponding number
 
             # collect all numbers that can be parsed
-            parsed_values = []
+            usable_numbers = []
             for val in values:
                 try:
-                    number = float(val)
-                except:
+                    val = float(val)
+                except (ValueError, TypeError):
+                    continue
+                except OverflowError:
+                    # todo: issue warning
+                    continue
+
+                if not isfinite(val):
                     continue
-                parsed_values.append(number)
 
-            if len(parsed_values) == 0:
+                usable_numbers.append(val)
+
+            if len(usable_numbers) == 0:
                 raise ValueError(f"Cannot compute {self.__default_value},"
-                                 f" because parsing failed for all numbers.")
+                                 f" because no usable numbers were found in the given data.")
             if self.__default_value == "mean":
-                self.__default_value = float(mean(parsed_values))
+                self.__default_value = float(mean(usable_numbers))
             elif self.__default_value == "median":
-                self.__default_value = float(median(parsed_values))
+                self.__default_value = float(median(usable_numbers))
             elif self.__default_value == "mode":
-                mode_, count = mode(parsed_values, keepdims=False)
-                self.__default_value = float(mode_)
+                self.__default_value = _mode(usable_numbers)
 
     def transform(self, row: tuple) -> tuple:
         val = row[0]  # unpack 1-element tuple
-        num = _try_float(val)
-        if num is not None:
+        try:
+            num = float(val)
+        except (ValueError, TypeError):
+            num = float("nan")
+        except OverflowError:
+            # todo: issue warning
+            num = float("nan")
+
+        if math.isfinite(num):
             return (num,)
 
         # conversion / parsing failed.
         # ensure that a usable default value exists
         if self.__default_value is None:
             raise ValueError(f"Cannot transform value '{val}' to float,"
                              f" because parsing failed and no default value was specified.")
```

### Comparing `clevertable-3.0.0/src/clevertable/ForEach.py` & `clevertable-3.0.1/src/clevertable/ForEach.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.0/src/clevertable/Function.py` & `clevertable-3.0.1/src/clevertable/Function.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.0/src/clevertable/Infer.py` & `clevertable-3.0.1/src/clevertable/Infer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import numbers
 import re
 
 from .Converter import Converter
 from .Ignore import Ignore
 
 
 class Infer(Converter):
@@ -43,26 +42,30 @@
 def _infer_converter_from_data(rows: list[tuple]) -> Converter:
     """Tries to infer the best converter from the given data.
     If no converter can be inferred, a ValueError is raised."""
     # dynamic imports in order to break circular dependency
     from .Binary import Binary
     from .Enumerate import Enumerate
     from .Float import Float
-    from .Float import _try_float
     from .List import List, ListAndOr
     from .OneHot import OneHot
 
     # if only contains 1-element rows:
     if all(len(row) == 1 for row in rows):
 
         values = [row[0] for row in rows]  # unpack 1-element rows
 
-        # if only contains numbers:
-        if all(isinstance(val, numbers.Number) or val in (None, "") or _try_float(val) is not None
-               for val in values):
+        def _is_parseable_float(val: any) -> bool:
+            try:
+                float(val)
+            except (ValueError, TypeError, OverflowError):
+                return False
+            return True
+
+        if all(map(_is_parseable_float, values)):
             return Float()
 
         # since numerical approach failed,
         # we now try categorical approaches
         string_values = [val for val in values if isinstance(val, str)]
 
         # check if it can be split according to List()
```

### Comparing `clevertable-3.0.0/src/clevertable/List.py` & `clevertable-3.0.1/src/clevertable/List.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.0/src/clevertable/Map.py` & `clevertable-3.0.1/src/clevertable/Map.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.0/src/clevertable/OneHot.py` & `clevertable-3.0.1/src/clevertable/OneHot.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.0/src/clevertable/Parallel.py` & `clevertable-3.0.1/src/clevertable/Parallel.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.0/src/clevertable/Pipeline.py` & `clevertable-3.0.1/src/clevertable/Pipeline.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.0/src/clevertable/RecordProfile.py` & `clevertable-3.0.1/src/clevertable/RecordProfile.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.0/src/clevertable/Split.py` & `clevertable-3.0.1/src/clevertable/Split.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.0/src/clevertable/StrictFunction.py` & `clevertable-3.0.1/src/clevertable/StrictFunction.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.0/src/clevertable/Strip.py` & `clevertable-3.0.1/src/clevertable/Strip.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.0/src/clevertable/Transpose.py` & `clevertable-3.0.1/src/clevertable/Transpose.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.0/src/clevertable/Try.py` & `clevertable-3.0.1/src/clevertable/Try.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.0/src/clevertable/__init__.py` & `clevertable-3.0.1/src/clevertable/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "3.0.0"
+__version__ = "3.0.1"
 
 from .Binary import Binary
 from .Const import Const
 from .ConversionProfile import ConversionProfile
 from .Converter import Converter
 from .Enumerate import Enumerate
 from .Flatten import Flatten
```

### Comparing `clevertable-3.0.0/src/clevertable/__main__.py` & `clevertable-3.0.1/src/clevertable/__main__.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.0/src/clevertable/_utils.py` & `clevertable-3.0.1/src/clevertable/_utils.py`

 * *Files identical despite different names*

### Comparing `clevertable-3.0.0/src/clevertable.egg-info/PKG-INFO` & `clevertable-3.0.1/src/clevertable.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clevertable
-Version: 3.0.0
+Version: 3.0.1
 Summary: Low effort conversion of tabular data into numerical values.
 Author: Tom Mohr
 License: MIT License
         
         Copyright (c) 2023 Tom Mohr
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `clevertable-3.0.0/src/clevertable.egg-info/SOURCES.txt` & `clevertable-3.0.1/src/clevertable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

