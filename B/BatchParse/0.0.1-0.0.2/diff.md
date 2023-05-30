# Comparing `tmp/BatchParse-0.0.1.tar.gz` & `tmp/BatchParse-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BatchParse-0.0.1.tar", last modified: Mon May 29 23:50:11 2023, max compression
+gzip compressed data, was "BatchParse-0.0.2.tar", last modified: Tue May 30 00:32:39 2023, max compression
```

## Comparing `BatchParse-0.0.1.tar` & `BatchParse-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:50:11.688527 BatchParse-0.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:50:11.688527 BatchParse-0.0.1/BatchParse/
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-29 23:49:56.000000 BatchParse-0.0.1/BatchParse/BatchParse.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-29 23:49:56.000000 BatchParse-0.0.1/BatchParse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:50:11.688527 BatchParse-0.0.1/BatchParse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-29 23:50:11.000000 BatchParse-0.0.1/BatchParse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-29 23:50:11.000000 BatchParse-0.0.1/BatchParse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 23:50:11.000000 BatchParse-0.0.1/BatchParse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-29 23:50:11.000000 BatchParse-0.0.1/BatchParse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-29 23:50:11.000000 BatchParse-0.0.1/BatchParse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-29 23:49:56.000000 BatchParse-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-29 23:50:11.688527 BatchParse-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 23:49:56.000000 BatchParse-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 23:50:11.688527 BatchParse-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-29 23:49:56.000000 BatchParse-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:32:39.471039 BatchParse-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:32:39.471039 BatchParse-0.0.2/BatchParse/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-30 00:32:21.000000 BatchParse-0.0.2/BatchParse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-30 00:32:21.000000 BatchParse-0.0.2/BatchParse/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:32:39.471039 BatchParse-0.0.2/BatchParse/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 00:32:21.000000 BatchParse-0.0.2/BatchParse/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-30 00:32:21.000000 BatchParse-0.0.2/BatchParse/util/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-30 00:32:21.000000 BatchParse-0.0.2/BatchParse/util/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-30 00:32:21.000000 BatchParse-0.0.2/BatchParse/util/splitting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:32:39.471039 BatchParse-0.0.2/BatchParse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-30 00:32:39.000000 BatchParse-0.0.2/BatchParse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-30 00:32:39.000000 BatchParse-0.0.2/BatchParse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 00:32:39.000000 BatchParse-0.0.2/BatchParse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-30 00:32:39.000000 BatchParse-0.0.2/BatchParse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-30 00:32:39.000000 BatchParse-0.0.2/BatchParse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-30 00:32:21.000000 BatchParse-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-30 00:32:39.471039 BatchParse-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-30 00:32:21.000000 BatchParse-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 00:32:39.471039 BatchParse-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-30 00:32:21.000000 BatchParse-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:32:39.471039 BatchParse-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-30 00:32:21.000000 BatchParse-0.0.2/test/test.py
```

### Comparing `BatchParse-0.0.1/BatchParse/BatchParse.py` & `BatchParse-0.0.2/BatchParse/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,27 +21,36 @@
 else:
     logging.basicConfig(
         level=logging.INFO, format="%(message)s", datefmt="[%X]", handlers=[handler]
     )
 logger = logging.getLogger("rich")
 
 
-def parse(code: str, split_and: bool = False) -> list:
+def parse(code: str, bsplit_and: bool = True, bsplit_carrot: bool = True) -> list:
     """Parse initial Batch Code
 
     Args:
         code (str): Inital Batch Code to Parse
 
     Returns:
         list: Returns Parsed Batch Code as an Array
     """
     code_to_array = code.split("\n")
 
-    if split_and:
-        code_to_array = parse_and(code_to_array)
+    initial_split_methods = {
+        bsplit_and: parse_and,
+        bsplit_carrot: parse_carrot,
+    }
+
+    # if split_and:
+    #    code_to_array = parse_and(code_to_array)
+
+    for method in initial_split_methods:
+        if method:
+            code_to_array = initial_split_methods[method](code_to_array)
 
     parsed_code = []
 
     allowed_methods = Settings.allowed_methods
 
     ignorable_lines = Settings.ignorable_lines
 
@@ -60,27 +69,27 @@
                     break
         else:
             parsed_code.append(line)
 
     return parsed_code
 
 
-def parse_heavy(code: str, split_and: bool = False) -> list:
+def parse_heavy(code: str, bsplit_and: bool = True) -> list:
     """Parses code and returns a dict with all the elements of the code and different infot that the user might want to know
 
     Args:
         code (str): Code to Parse
         parse_and (bool, optional): if user wants to parse and Defaults to False.
     Returns:
         list: Parsed code as a list with [[code, dict], [code, dict], [code, dict]] (EXAMPLE)
     """
 
     final_arr = []
 
-    initial_parse = parse(code, split_and=split_and)
+    initial_parse = parse(code, bsplit_and=bsplit_and)
     logger.debug(f"Initial Parse: {initial_parse}")
     for array in track(initial_parse, description="Parsing Batch Code HEAVY..."):
         logger.debug(f"Array: {array}")
         dict_parse = info_gather(array)
         logger.debug(f"Dict Parse: {dict_parse}")
         final_arr.append([array, dict_parse])
```

### Comparing `BatchParse-0.0.1/LICENSE` & `BatchParse-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `BatchParse-0.0.1/setup.py` & `BatchParse-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 DESCRIPTION = "A Batch Parser"
 LONG_DESCRIPTION = "Easy Way to Parse Batch Code in Python"
 
 setup(
     name="BatchParse",
     version=VERSION,
     description=DESCRIPTION,
```

