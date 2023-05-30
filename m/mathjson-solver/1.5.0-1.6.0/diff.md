# Comparing `tmp/mathjson-solver-1.5.0.tar.gz` & `tmp/mathjson-solver-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathjson-solver-1.5.0.tar", last modified: Wed May 24 10:47:47 2023, max compression
+gzip compressed data, was "mathjson-solver-1.6.0.tar", last modified: Tue May 30 10:10:05 2023, max compression
```

## Comparing `mathjson-solver-1.5.0.tar` & `mathjson-solver-1.6.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2023-05-24 10:47:47.459472 mathjson-solver-1.5.0/
--rw-rw-r--   0 martins   (1000) martins   (1000)     1071 2023-05-24 10:25:32.000000 mathjson-solver-1.5.0/LICENSE
--rw-rw-r--   0 martins   (1000) martins   (1000)     7111 2023-05-24 10:47:47.459472 mathjson-solver-1.5.0/PKG-INFO
--rw-rw-r--   0 martins   (1000) martins   (1000)     6582 2023-05-24 10:25:32.000000 mathjson-solver-1.5.0/README.md
--rw-rw-r--   0 martins   (1000) martins   (1000)       85 2023-05-24 10:25:32.000000 mathjson-solver-1.5.0/pyproject.toml
--rw-rw-r--   0 martins   (1000) martins   (1000)      654 2023-05-24 10:47:47.463472 mathjson-solver-1.5.0/setup.cfg
--rw-rw-r--   0 martins   (1000) martins   (1000)      829 2023-05-24 10:45:23.000000 mathjson-solver-1.5.0/setup.py
-drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2023-05-24 10:47:47.459472 mathjson-solver-1.5.0/src/
-drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2023-05-24 10:47:47.459472 mathjson-solver-1.5.0/src/mathjson_solver/
--rw-rw-r--   0 martins   (1000) martins   (1000)      102 2023-05-24 10:25:32.000000 mathjson-solver-1.5.0/src/mathjson_solver/__init__.py
--rw-rw-r--   0 martins   (1000) martins   (1000)     6822 2023-05-24 10:39:53.000000 mathjson-solver-1.5.0/src/mathjson_solver/__main__.py
-drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2023-05-24 10:47:47.459472 mathjson-solver-1.5.0/src/mathjson_solver.egg-info/
--rw-rw-r--   0 martins   (1000) martins   (1000)     7111 2023-05-24 10:47:47.000000 mathjson-solver-1.5.0/src/mathjson_solver.egg-info/PKG-INFO
--rw-rw-r--   0 martins   (1000) martins   (1000)      313 2023-05-24 10:47:47.000000 mathjson-solver-1.5.0/src/mathjson_solver.egg-info/SOURCES.txt
--rw-rw-r--   0 martins   (1000) martins   (1000)        1 2023-05-24 10:47:47.000000 mathjson-solver-1.5.0/src/mathjson_solver.egg-info/dependency_links.txt
--rw-rw-r--   0 martins   (1000) martins   (1000)       16 2023-05-24 10:47:47.000000 mathjson-solver-1.5.0/src/mathjson_solver.egg-info/top_level.txt
-drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2023-05-24 10:47:47.459472 mathjson-solver-1.5.0/tests/
--rw-rw-r--   0 martins   (1000) martins   (1000)     5283 2023-05-24 10:44:43.000000 mathjson-solver-1.5.0/tests/test_with_pytest.py
+drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2023-05-30 10:10:05.405115 mathjson-solver-1.6.0/
+-rw-rw-r--   0 martins   (1000) martins   (1000)     1071 2022-05-02 08:10:45.000000 mathjson-solver-1.6.0/LICENSE
+-rw-rw-r--   0 martins   (1000) martins   (1000)     7111 2023-05-30 10:10:05.405115 mathjson-solver-1.6.0/PKG-INFO
+-rw-rw-r--   0 martins   (1000) martins   (1000)     6582 2023-05-22 07:13:26.000000 mathjson-solver-1.6.0/README.md
+-rw-rw-r--   0 martins   (1000) martins   (1000)       85 2022-05-02 14:01:31.000000 mathjson-solver-1.6.0/pyproject.toml
+-rw-rw-r--   0 martins   (1000) martins   (1000)      654 2023-05-30 10:10:05.405115 mathjson-solver-1.6.0/setup.cfg
+-rw-rw-r--   0 martins   (1000) martins   (1000)      829 2023-05-30 10:07:07.000000 mathjson-solver-1.6.0/setup.py
+drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2023-05-30 10:10:05.405115 mathjson-solver-1.6.0/src/
+drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2023-05-30 10:10:05.405115 mathjson-solver-1.6.0/src/mathjson_solver/
+-rw-rw-r--   0 martins   (1000) martins   (1000)      102 2022-05-23 07:31:11.000000 mathjson-solver-1.6.0/src/mathjson_solver/__init__.py
+-rw-rw-r--   0 martins   (1000) martins   (1000)     8486 2023-05-30 10:04:14.000000 mathjson-solver-1.6.0/src/mathjson_solver/__main__.py
+drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2023-05-30 10:10:05.405115 mathjson-solver-1.6.0/src/mathjson_solver.egg-info/
+-rw-rw-r--   0 martins   (1000) martins   (1000)     7111 2023-05-30 10:10:05.000000 mathjson-solver-1.6.0/src/mathjson_solver.egg-info/PKG-INFO
+-rw-rw-r--   0 martins   (1000) martins   (1000)      313 2023-05-30 10:10:05.000000 mathjson-solver-1.6.0/src/mathjson_solver.egg-info/SOURCES.txt
+-rw-rw-r--   0 martins   (1000) martins   (1000)        1 2023-05-30 10:10:05.000000 mathjson-solver-1.6.0/src/mathjson_solver.egg-info/dependency_links.txt
+-rw-rw-r--   0 martins   (1000) martins   (1000)       16 2023-05-30 10:10:05.000000 mathjson-solver-1.6.0/src/mathjson_solver.egg-info/top_level.txt
+drwxrwxr-x   0 martins   (1000) martins   (1000)        0 2023-05-30 10:10:05.405115 mathjson-solver-1.6.0/tests/
+-rw-rw-r--   0 martins   (1000) martins   (1000)     7571 2023-05-30 10:06:48.000000 mathjson-solver-1.6.0/tests/test_with_pytest.py
```

### Comparing `mathjson-solver-1.5.0/LICENSE` & `mathjson-solver-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mathjson-solver-1.5.0/PKG-INFO` & `mathjson-solver-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathjson-solver
-Version: 1.5.0
+Version: 1.6.0
 Summary: Utilities for MathJSON evaluation
 Home-page: https://github.com/LongenesisLtd/mathjson-solver
 Author: Martins Mednis
 Author-email: mrt@mednis.info
 Project-URL: Bug Tracker, https://github.com/LongenesisLtd/mathjson-solver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mathjson-solver-1.5.0/README.md` & `mathjson-solver-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `mathjson-solver-1.5.0/setup.cfg` & `mathjson-solver-1.6.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mathjson-solver
-version = 1.5.0
+version = 1.6.0
 author = Martins Mednis
 author_email = mrt@mednis.info
 description = Utilities for MathJSON evaluation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/LongenesisLtd/mathjson-solver
 project_urls =
```

### Comparing `mathjson-solver-1.5.0/setup.py` & `mathjson-solver-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mathjson-solver",
-    version="1.5.0",
+    version="1.6.0",
     author="Martins Mednis",
     author_email="mrt@mednis.info",
     description="Utilities for MathJSON evaluation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LongenesisLtd/mathjson-solver",
     project_urls={
```

### Comparing `mathjson-solver-1.5.0/src/mathjson_solver/__main__.py` & `mathjson-solver-1.6.0/src/mathjson_solver/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -126,26 +126,68 @@
                     if f(x[0], c):
                         return f(x[1], c)
                 return f(s[-1], c)
 
             def In(s):
                 if len(s) != 3:
                     raise ValueError(f"Wrong parameters for 'In'")
-                if type(s[2]) != list and s[2][0] != "Array":
+                if type(s[2]) == list and s[2][0] == "Array":
+                    return f(s[1], c) in [f(x, c) for x in s[2][1:]]
+
+                elif type(s[2]) == str:
+                    return f(s[1], c) in f(s[2], c)
+                else:
                     raise ValueError(
                         f"Wrong parameters for 'In'. Parameter 2 must be a list."
                     )
 
-                return f(s[1], c) in [f(x, c) for x in s[2][1:]]
+            def Not_in(s):
+                return not In(s)
+
+            def Contains_any_of(s):
+                if type(s[1]) == list and s[1][0] == "Array":
+                    list1 = [f(x, c) for x in s[1][1:]]
+                elif type(s[1]) == str:
+                    list1 = f(s[1], c)
+
+                if type(s[2]) == list and s[2][0] == "Array":
+                    list2 = [f(x, c) for x in s[2][1:]]
+                elif type(s[2]) == str:
+                    list2 = f(s[2], c)
+
+                if any(x in list1 for x in list2):
+                    return True
+                return False
+
+            def Contains_all_of(s):
+                if type(s[1]) == list and s[1][0] == "Array":
+                    list1 = [f(x, c) for x in s[1][1:]]
+                elif type(s[1]) == str:
+                    list1 = f(s[1], c)
+
+                if type(s[2]) == list and s[2][0] == "Array":
+                    list2 = [f(x, c) for x in s[2][1:]]
+                elif type(s[2]) == str:
+                    list2 = f(s[2], c)
+
+                if all(x in list1 for x in list2):
+                    return True
+                return False
+
+            def Contains_none_of(s):
+                return not Contains_any_of(s)
 
             def Str(s):
                 if len(s) < 2:
                     raise ValueError(f"Wrong parameters for 'Str'")
                 return f"{f(s[1])}"
 
+            def Not(s):
+                return not f(s[1])
+
             constructs = {
                 "Add": lambda s: sum([f(x, c) for x in s[1:]]),
                 "Sum": lambda s: sum([f(x, c) for x in s[1:]]),
                 "Subtract": lambda s: reduce(
                     lambda a, b: a - b, [f(x, c) for x in s[1:]]
                 ),
                 "Constants": Constants,
@@ -179,27 +221,33 @@
                 "Average": Average,
                 "Median": Median,
                 "Length": Length,
                 "Any": Any,
                 "All": All,
                 "Array": Arr,
                 "In": In,
+                "Not_in": Not_in,
+                "Contains_any_of": Contains_any_of,
+                "Contains_all_of": Contains_all_of,
+                "Contains_none_of": Contains_none_of,
                 "Int": Int,
                 "Float": Float,
                 "Str": Str,
+                "Not": Not,
             }
             if s[0] in constructs:
                 try:
                     return constructs[s[0]](s)
                 except Exception as e:
                     raise MathJSONException(e, s, mathjson_construct=s[0])
             else:
-                raise MathJSONException(
-                    NotImplementedError(f"'{s[0]}' is not supported"), s
-                )
+                # raise MathJSONException(
+                #     NotImplementedError(f"'{s[0]}' is not supported"), s
+                # )
+                return s
         elif s in solver_parameters:
             return f(solver_parameters[s], c)
         elif s in c:
             return f(c[s], c)
         else:
             return s
```

### Comparing `mathjson-solver-1.5.0/src/mathjson_solver.egg-info/PKG-INFO` & `mathjson-solver-1.6.0/src/mathjson_solver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathjson-solver
-Version: 1.5.0
+Version: 1.6.0
 Summary: Utilities for MathJSON evaluation
 Home-page: https://github.com/LongenesisLtd/mathjson-solver
 Author: Martins Mednis
 Author-email: mrt@mednis.info
 Project-URL: Bug Tracker, https://github.com/LongenesisLtd/mathjson-solver/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

