# Comparing `tmp/naapc-1.6.0.tar.gz` & `tmp/naapc-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naapc-1.6.0.tar", last modified: Mon May 29 13:35:58 2023, max compression
+gzip compressed data, was "naapc-1.6.1.tar", last modified: Tue May 30 00:29:29 2023, max compression
```

## Comparing `naapc-1.6.0.tar` & `naapc-1.6.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0 ei        (1000) ei        (1000)        0 2023-05-29 13:35:58.191321 naapc-1.6.0/
--rwxrwxrwx   0 ei        (1000) ei        (1000)     1067 2023-05-29 12:45:29.000000 naapc-1.6.0/LICENSE
--rwxrwxrwx   0 ei        (1000) ei        (1000)     6400 2023-05-29 13:35:58.190321 naapc-1.6.0/PKG-INFO
--rwxrwxrwx   0 ei        (1000) ei        (1000)     4642 2023-05-29 13:32:11.000000 naapc-1.6.0/README.md
--rwxrwxrwx   0 ei        (1000) ei        (1000)     1003 2023-05-29 13:27:44.000000 naapc-1.6.0/pyproject.toml
--rwxrwxrwx   0 ei        (1000) ei        (1000)       38 2023-05-29 13:35:58.192320 naapc-1.6.0/setup.cfg
-drwxrwxrwx   0 ei        (1000) ei        (1000)        0 2023-05-29 13:35:57.993888 naapc-1.6.0/src/
-drwxrwxrwx   0 ei        (1000) ei        (1000)        0 2023-05-29 13:35:58.088390 naapc-1.6.0/src/naapc/
--rwxrwxrwx   0 ei        (1000) ei        (1000)      129 2023-05-29 13:27:44.000000 naapc-1.6.0/src/naapc/__init__.py
--rwxrwxrwx   0 ei        (1000) ei        (1000)     5995 2023-05-29 13:12:19.000000 naapc-1.6.0/src/naapc/nconfig.py
--rwxrwxrwx   0 ei        (1000) ei        (1000)     6661 2023-05-29 13:20:05.000000 naapc-1.6.0/src/naapc/ndict.py
-drwxrwxrwx   0 ei        (1000) ei        (1000)        0 2023-05-29 13:35:58.163250 naapc-1.6.0/src/naapc.egg-info/
--rwxrwxrwx   0 ei        (1000) ei        (1000)     6400 2023-05-29 13:35:57.000000 naapc-1.6.0/src/naapc.egg-info/PKG-INFO
--rwxrwxrwx   0 ei        (1000) ei        (1000)      271 2023-05-29 13:35:57.000000 naapc-1.6.0/src/naapc.egg-info/SOURCES.txt
--rwxrwxrwx   0 ei        (1000) ei        (1000)        1 2023-05-29 13:35:57.000000 naapc-1.6.0/src/naapc.egg-info/dependency_links.txt
--rwxrwxrwx   0 ei        (1000) ei        (1000)        7 2023-05-29 13:35:57.000000 naapc-1.6.0/src/naapc.egg-info/requires.txt
--rwxrwxrwx   0 ei        (1000) ei        (1000)        6 2023-05-29 13:35:57.000000 naapc-1.6.0/src/naapc.egg-info/top_level.txt
-drwxrwxrwx   0 ei        (1000) ei        (1000)        0 2023-05-29 13:35:58.175260 naapc-1.6.0/test/
--rwxrwxrwx   0 ei        (1000) ei        (1000)    16019 2023-05-29 13:20:42.000000 naapc-1.6.0/test/test.py
+drwxrwxrwx   0 ei        (1000) ei        (1000)        0 2023-05-30 00:29:29.258334 naapc-1.6.1/
+-rwxrwxrwx   0 ei        (1000) ei        (1000)     1067 2023-05-29 12:45:29.000000 naapc-1.6.1/LICENSE
+-rwxrwxrwx   0 ei        (1000) ei        (1000)     6400 2023-05-30 00:29:29.256334 naapc-1.6.1/PKG-INFO
+-rwxrwxrwx   0 ei        (1000) ei        (1000)     4642 2023-05-29 13:32:11.000000 naapc-1.6.1/README.md
+-rwxrwxrwx   0 ei        (1000) ei        (1000)     1003 2023-05-30 00:28:46.000000 naapc-1.6.1/pyproject.toml
+-rwxrwxrwx   0 ei        (1000) ei        (1000)       38 2023-05-30 00:29:29.258334 naapc-1.6.1/setup.cfg
+drwxrwxrwx   0 ei        (1000) ei        (1000)        0 2023-05-30 00:29:29.123611 naapc-1.6.1/src/
+drwxrwxrwx   0 ei        (1000) ei        (1000)        0 2023-05-30 00:29:29.179113 naapc-1.6.1/src/naapc/
+-rwxrwxrwx   0 ei        (1000) ei        (1000)      129 2023-05-30 00:28:46.000000 naapc-1.6.1/src/naapc/__init__.py
+-rwxrwxrwx   0 ei        (1000) ei        (1000)     5995 2023-05-29 13:12:19.000000 naapc-1.6.1/src/naapc/nconfig.py
+-rwxrwxrwx   0 ei        (1000) ei        (1000)     6711 2023-05-30 00:28:30.000000 naapc-1.6.1/src/naapc/ndict.py
+drwxrwxrwx   0 ei        (1000) ei        (1000)        0 2023-05-30 00:29:29.236334 naapc-1.6.1/src/naapc.egg-info/
+-rwxrwxrwx   0 ei        (1000) ei        (1000)     6400 2023-05-30 00:29:29.000000 naapc-1.6.1/src/naapc.egg-info/PKG-INFO
+-rwxrwxrwx   0 ei        (1000) ei        (1000)      271 2023-05-30 00:29:29.000000 naapc-1.6.1/src/naapc.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ei        (1000) ei        (1000)        1 2023-05-30 00:29:29.000000 naapc-1.6.1/src/naapc.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ei        (1000) ei        (1000)        7 2023-05-30 00:29:29.000000 naapc-1.6.1/src/naapc.egg-info/requires.txt
+-rwxrwxrwx   0 ei        (1000) ei        (1000)        6 2023-05-30 00:29:29.000000 naapc-1.6.1/src/naapc.egg-info/top_level.txt
+drwxrwxrwx   0 ei        (1000) ei        (1000)        0 2023-05-30 00:29:29.245335 naapc-1.6.1/test/
+-rwxrwxrwx   0 ei        (1000) ei        (1000)    16019 2023-05-29 13:20:42.000000 naapc-1.6.1/test/test.py
```

### Comparing `naapc-1.6.0/LICENSE` & `naapc-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `naapc-1.6.0/PKG-INFO` & `naapc-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naapc
-Version: 1.6.0
+Version: 1.6.1
 Summary: Nested Automated Argument Parsing Configuration (NAAPC).
 Author-email: Bai Huanyu <eiphnix@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Bai Huanyu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `naapc-1.6.0/README.md` & `naapc-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `naapc-1.6.0/pyproject.toml` & `naapc-1.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["wheel", "setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "naapc"
-version = "1.6.0"
+version = "1.6.1"
 description = "Nested Automated Argument Parsing Configuration (NAAPC)."
 readme = "README.md"
 authors = [{name = "Bai Huanyu", email = "eiphnix@gmail.com"}]
 license = {file = "LICENSE"}
 
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -19,15 +19,15 @@
 dependencies = ["pyyaml"]
 requires-python = "==3.10.*"
 
 [project.urls]
 repository = "https://github.com/eiphy/naapc"
 
 [tool.bumpver]
-current_version = "1.6.0"
+current_version = "1.6.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = false
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `naapc-1.6.0/src/naapc/nconfig.py` & `naapc-1.6.1/src/naapc/nconfig.py`

 * *Files identical despite different names*

### Comparing `naapc-1.6.0/src/naapc/ndict.py` & `naapc-1.6.1/src/naapc/ndict.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,21 +41,22 @@
     def from_list_of_dict(cls, ls: list, delimiter=";") -> ndict:
         """Generate nested from a list of dictionaries."""
         res = cls()
         for d in ls:
             res.update(d)
         return res
 
-    def is_matched(self, query: dict, missing_method: str = "ignore") -> bool:
+    def is_matched(self, query: dict, missing_method: str = "ignore", **kwargs) -> bool:
         """Test if the dictionary is the queried one.
 
         Syntax:
             1. Normal path-value pair: {path: value}.
             2. Query expression: {path: !QUERY [python expression returns boolean results]}. The
-                expression can use d: the dictionary and path: the query path.
+                expression can use d: the dictionary, path: the query path and any other input
+                kwargs.
 
         Args:
             query (dict): query dictionary.
             missing_method (str): actions when the path is missing from the dictionary. Support:
             ['ignore', 'false', 'error'].
         Returns:
             (bool): if the dictionary is the queried one.
```

### Comparing `naapc-1.6.0/src/naapc.egg-info/PKG-INFO` & `naapc-1.6.1/src/naapc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naapc
-Version: 1.6.0
+Version: 1.6.1
 Summary: Nested Automated Argument Parsing Configuration (NAAPC).
 Author-email: Bai Huanyu <eiphnix@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Bai Huanyu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `naapc-1.6.0/test/test.py` & `naapc-1.6.1/test/test.py`

 * *Files identical despite different names*

