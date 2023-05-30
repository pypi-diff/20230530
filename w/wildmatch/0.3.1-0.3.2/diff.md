# Comparing `tmp/wildmatch-0.3.1.tar.gz` & `tmp/wildmatch-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wildmatch-0.3.1.tar", last modified: Mon Feb 27 03:35:56 2023, max compression
+gzip compressed data, was "wildmatch-0.3.2.tar", max compression
```

## Comparing `wildmatch-0.3.1.tar` & `wildmatch-0.3.2.tar`

### file list

```diff
@@ -1,21 +1,7 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-27 03:35:56.381394 wildmatch-0.3.1/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1454 2023-02-27 03:35:56.000000 wildmatch-0.3.1/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)       41 2023-02-27 03:35:56.000000 wildmatch-0.3.1/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1553 2023-02-27 03:35:56.381394 wildmatch-0.3.1/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1083 2023-02-27 03:35:56.000000 wildmatch-0.3.1/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      173 2023-02-27 03:35:56.000000 wildmatch-0.3.1/pyproject.toml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      881 2023-02-27 03:35:56.000000 wildmatch-0.3.1/requirements.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       74 2023-02-27 03:35:56.381394 wildmatch-0.3.1/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1115 2023-02-27 03:35:56.000000 wildmatch-0.3.1/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-27 03:35:56.377394 wildmatch-0.3.1/src/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-27 03:35:56.000000 wildmatch-0.3.1/src/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-27 03:35:56.377394 wildmatch-0.3.1/src/wildmatch/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-27 03:35:56.000000 wildmatch-0.3.1/src/wildmatch/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2635 2023-02-27 03:35:56.000000 wildmatch-0.3.1/src/wildmatch/filter.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-27 03:35:56.381394 wildmatch-0.3.1/src/wildmatch.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1553 2023-02-27 03:35:56.000000 wildmatch-0.3.1/src/wildmatch.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      370 2023-02-27 03:35:56.000000 wildmatch-0.3.1/src/wildmatch.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-02-27 03:35:56.000000 wildmatch-0.3.1/src/wildmatch.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       53 2023-02-27 03:35:56.000000 wildmatch-0.3.1/src/wildmatch.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       16 2023-02-27 03:35:56.000000 wildmatch-0.3.1/src/wildmatch.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       10 2023-02-27 03:35:56.000000 wildmatch-0.3.1/src/wildmatch.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1454 2023-05-30 15:13:44.770452 wildmatch-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1125 2023-05-30 15:13:44.770452 wildmatch-0.3.2/README.md
+-rw-r--r--   0        0        0      762 2023-05-30 15:13:58.938559 wildmatch-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-30 15:13:44.770452 wildmatch-0.3.2/src/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 15:13:44.770452 wildmatch-0.3.2/src/wildmatch/__init__.py
+-rw-r--r--   0        0        0     2680 2023-05-30 15:13:44.770452 wildmatch-0.3.2/src/wildmatch/filter.py
+-rw-r--r--   0        0        0     1756 1970-01-01 00:00:00.000000 wildmatch-0.3.2/PKG-INFO
```

### Comparing `wildmatch-0.3.1/LICENSE` & `wildmatch-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wildmatch-0.3.1/PKG-INFO` & `wildmatch-0.3.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: wildmatch
-Version: 0.3.1
-Summary: A pathspec wrapper/CLI for use in CI/pipelines
-Home-page: https://github.com/bjd2385/wildmatch
-Author: Emma Doyle
-Author-email: bjd2385.linux@gmail.com
-License: UNKNOWN
-Project-URL: Bug Reports, https://github.com/bjd2385/wildmatch/issues
-Project-URL: Source, https://github.com/bjd2385/wildmatch
-Platform: UNKNOWN
-Requires-Python: >=3.10, <4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # `wildmatch`
 
 [![PyPI version](https://img.shields.io/pypi/v/wildmatch.svg?logo=pypi&style=flat-square)](https://pypi.org/project/wildmatch/)
 [![PyPI downloads](https://img.shields.io/pypi/dm/wildmatch?style=flat-square)](https://pypistats.org/packages/wildmatch)
 
 
 
@@ -26,23 +11,21 @@
 
 ```shell
 $ wildmatch --help
 usage: wildmatch [-h] [-c CONF] [-i INPUT]
 
 Filter lists of paths by arbitrary .gitignore-like configuration files.
 
-options:
+optional arguments:
   -h, --help            show this help message and exit
-  -c CONF, --conf CONF  optionally set the configuration file to filter by, defaults to .diffignore
+  -c CONF, --conf CONF  optionally set the configuration file to filter by, defaults to .diffignore (default: .diffignore)
   -i INPUT, --input INPUT
-                        optionally specify an input file to filter by the configuration file
+                        optionally specify an input file to filter by the configuration file (default: None)
 ```
 
 ## Install
 
-Installation requires Python v3.10 or later.
+Installation requires Python `>=3.9`.
 
 ```shell
 pip install wildmatch
-```
-
-
+```
```

### Comparing `wildmatch-0.3.1/src/wildmatch/filter.py` & `wildmatch-0.3.2/src/wildmatch/filter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Filter input files or stdin lines by a wildmatch filter/config file.
 """
 
-from argparse import ArgumentParser
+from argparse import ArgumentParser, ArgumentDefaultsHelpFormatter
 
 import sys
 import pathlib
 import pathspec
 
 
 def print_error(message: str, exit_code: int = 1) -> None:
@@ -61,15 +61,16 @@
 
 
 def main() -> None:
     """
     Run argparse.
     """
     parser = ArgumentParser(
-        description='Filter lists of paths by arbitrary .gitignore-like configuration files.'
+        description='Filter lists of paths by arbitrary .gitignore-like configuration files.',
+        formatter_class=ArgumentDefaultsHelpFormatter
     )
 
     parser.add_argument('-c', '--conf', type=str, default='.diffignore',
         help='optionally set the configuration file to filter by, defaults to .diffignore'
     )
 
     parser.add_argument('-i', '--input', type=str, default=None,
@@ -83,12 +84,8 @@
 
     if not args.input and sys.stdin.isatty():
         print_error('Must provide either an input file or piped values to consume.')
     elif args.input:
         # Read this file's lines, one at a time, for processing.
         input_file(args.input, args.conf)
     else:
-        input_piped(args.conf)
-
-
-if __name__ == '__main__':
-    main()
+        input_piped(args.conf)
```

