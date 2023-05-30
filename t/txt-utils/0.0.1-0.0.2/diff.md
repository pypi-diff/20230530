# Comparing `tmp/txt-utils-0.0.1.tar.gz` & `tmp/txt-utils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txt-utils-0.0.1.tar", last modified: Mon May 30 11:13:43 2022, max compression
+gzip compressed data, was "txt-utils-0.0.2.tar", last modified: Tue May 30 14:59:44 2023, max compression
```

## Comparing `txt-utils-0.0.1.tar` & `txt-utils-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2022-05-30 11:13:43.541101 txt-utils-0.0.1/
--rw-rw-r--   0 mi        (1000) mi        (1000)     1070 2022-05-11 07:15:48.000000 txt-utils-0.0.1/LICENSE
--rw-rw-r--   0 mi        (1000) mi        (1000)     2744 2022-05-30 11:13:43.541101 txt-utils-0.0.1/PKG-INFO
--rw-rw-r--   0 mi        (1000) mi        (1000)     1464 2022-05-30 11:10:01.000000 txt-utils-0.0.1/README.md
--rw-rw-r--   0 mi        (1000) mi        (1000)     2392 2022-05-30 10:51:00.000000 txt-utils-0.0.1/pyproject.toml
--rw-rw-r--   0 mi        (1000) mi        (1000)       38 2022-05-30 11:13:43.541101 txt-utils-0.0.1/setup.cfg
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2022-05-30 11:13:43.541101 txt-utils-0.0.1/src/
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2022-05-30 11:13:43.541101 txt-utils-0.0.1/src/txt_utils.egg-info/
--rw-rw-r--   0 mi        (1000) mi        (1000)     2744 2022-05-30 11:13:43.000000 txt-utils-0.0.1/src/txt_utils.egg-info/PKG-INFO
--rw-rw-r--   0 mi        (1000) mi        (1000)      740 2022-05-30 11:13:43.000000 txt-utils-0.0.1/src/txt_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 mi        (1000) mi        (1000)        1 2022-05-30 11:13:43.000000 txt-utils-0.0.1/src/txt_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 mi        (1000) mi        (1000)       61 2022-05-30 11:13:43.000000 txt-utils-0.0.1/src/txt_utils.egg-info/entry_points.txt
--rw-rw-r--   0 mi        (1000) mi        (1000)       63 2022-05-30 11:13:43.000000 txt-utils-0.0.1/src/txt_utils.egg-info/requires.txt
--rw-rw-r--   0 mi        (1000) mi        (1000)       24 2022-05-30 11:13:43.000000 txt-utils-0.0.1/src/txt_utils.egg-info/top_level.txt
-drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2022-05-30 11:13:43.541101 txt-utils-0.0.1/src/txt_utils_cli/
--rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-05-30 10:50:25.000000 txt-utils-0.0.1/src/txt_utils_cli/__init__.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     6022 2022-05-30 11:13:11.000000 txt-utils-0.0.1/src/txt_utils_cli/cli.py
--rw-rw-r--   0 mi        (1000) mi        (1000)      858 2022-05-30 11:12:07.000000 txt-utils-0.0.1/src/txt_utils_cli/default_args.py
--rw-rw-r--   0 mi        (1000) mi        (1000)      742 2022-05-30 11:12:08.000000 txt-utils-0.0.1/src/txt_utils_cli/globals.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     7264 2022-05-30 11:12:09.000000 txt-utils-0.0.1/src/txt_utils_cli/helper.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2034 2022-05-30 11:12:10.000000 txt-utils-0.0.1/src/txt_utils_cli/line_replacement.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     5164 2022-05-30 11:12:11.000000 txt-utils-0.0.1/src/txt_utils_cli/logging_configuration.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2609 2022-05-30 11:12:13.000000 txt-utils-0.0.1/src/txt_utils_cli/merging.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2070 2022-05-30 11:12:12.000000 txt-utils-0.0.1/src/txt_utils_cli/replacement.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2171 2022-05-30 11:12:14.000000 txt-utils-0.0.1/src/txt_utils_cli/statistics_unit_counts.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     7041 2022-05-30 11:12:15.000000 txt-utils-0.0.1/src/txt_utils_cli/transcription.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     2444 2022-05-30 11:12:17.000000 txt-utils-0.0.1/src/txt_utils_cli/trimming.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     1928 2022-05-30 11:12:18.000000 txt-utils-0.0.1/src/txt_utils_cli/unit_removal.py
--rw-rw-r--   0 mi        (1000) mi        (1000)     3596 2022-05-30 11:12:20.000000 txt-utils-0.0.1/src/txt_utils_cli/vocabulary_exporting.py
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 14:59:44.072992 txt-utils-0.0.2/
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1070 2023-05-30 13:53:01.000000 txt-utils-0.0.2/LICENSE
+-rw-rw-r--   0 mi        (1000) mi        (1000)     3032 2023-05-30 14:59:44.072992 txt-utils-0.0.2/PKG-INFO
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1802 2023-05-30 14:56:29.000000 txt-utils-0.0.2/README.md
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2435 2023-05-30 14:02:28.000000 txt-utils-0.0.2/pyproject.toml
+-rw-rw-r--   0 mi        (1000) mi        (1000)       38 2023-05-30 14:59:44.072992 txt-utils-0.0.2/setup.cfg
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 14:59:44.072992 txt-utils-0.0.2/src/
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 14:59:44.072992 txt-utils-0.0.2/src/txt_utils.egg-info/
+-rw-rw-r--   0 mi        (1000) mi        (1000)     3032 2023-05-30 14:59:44.000000 txt-utils-0.0.2/src/txt_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 mi        (1000) mi        (1000)      740 2023-05-30 14:59:44.000000 txt-utils-0.0.2/src/txt_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 mi        (1000) mi        (1000)        1 2023-05-30 14:59:44.000000 txt-utils-0.0.2/src/txt_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 mi        (1000) mi        (1000)       61 2023-05-30 14:59:44.000000 txt-utils-0.0.2/src/txt_utils.egg-info/entry_points.txt
+-rw-rw-r--   0 mi        (1000) mi        (1000)       63 2023-05-30 14:59:44.000000 txt-utils-0.0.2/src/txt_utils.egg-info/requires.txt
+-rw-rw-r--   0 mi        (1000) mi        (1000)       14 2023-05-30 14:59:44.000000 txt-utils-0.0.2/src/txt_utils.egg-info/top_level.txt
+drwxrwxr-x   0 mi        (1000) mi        (1000)        0 2023-05-30 14:59:44.072992 txt-utils-0.0.2/src/txt_utils_cli/
+-rw-rw-r--   0 mi        (1000) mi        (1000)        2 2022-05-30 10:50:25.000000 txt-utils-0.0.2/src/txt_utils_cli/__init__.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     6020 2023-05-30 13:42:00.000000 txt-utils-0.0.2/src/txt_utils_cli/cli.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)      858 2022-05-30 11:12:07.000000 txt-utils-0.0.2/src/txt_utils_cli/default_args.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)      742 2022-05-30 11:12:08.000000 txt-utils-0.0.2/src/txt_utils_cli/globals.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     7264 2022-05-30 11:12:09.000000 txt-utils-0.0.2/src/txt_utils_cli/helper.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2163 2022-11-30 09:47:49.000000 txt-utils-0.0.2/src/txt_utils_cli/line_replacement.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     5164 2022-05-30 11:12:11.000000 txt-utils-0.0.2/src/txt_utils_cli/logging_configuration.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2509 2023-05-30 13:41:31.000000 txt-utils-0.0.2/src/txt_utils_cli/merging.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2209 2022-12-23 12:48:55.000000 txt-utils-0.0.2/src/txt_utils_cli/replacement.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2171 2022-05-30 11:12:14.000000 txt-utils-0.0.2/src/txt_utils_cli/statistics_unit_counts.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     7108 2022-11-28 17:42:02.000000 txt-utils-0.0.2/src/txt_utils_cli/transcription.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     2444 2022-05-30 11:12:17.000000 txt-utils-0.0.2/src/txt_utils_cli/trimming.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     1928 2022-05-30 11:12:18.000000 txt-utils-0.0.2/src/txt_utils_cli/unit_removal.py
+-rw-rw-r--   0 mi        (1000) mi        (1000)     3596 2022-06-30 07:23:53.000000 txt-utils-0.0.2/src/txt_utils_cli/vocabulary_exporting.py
```

### Comparing `txt-utils-0.0.1/LICENSE` & `txt-utils-0.0.2/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Stefan Taubert
+Copyright (c) 2023 Stefan Taubert
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `txt-utils-0.0.1/PKG-INFO` & `txt-utils-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 Metadata-Version: 2.1
 Name: txt-utils
-Version: 0.0.1
+Version: 0.0.2
 Summary: CLI to modify text files.
-Author-email: Stefan Taubert <stefan.taubert@posteo.me>
-Maintainer-email: Stefan Taubert <stefan.taubert@posteo.me>
+Author-email: Stefan Taubert <pypi@stefantaubert.com>
+Maintainer-email: Stefan Taubert <pypi@stefantaubert.com>
 License: MIT
 Project-URL: Homepage, https://github.com/stefantaubert/txt-utils
 Project-URL: Issues, https://github.com/stefantaubert/txt-utils/issues
 Keywords: Preprocessing,Processing,Text-to-speech,Speech synthesis,Utils,Language,Linguistics
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: BSD
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
+Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # txt-utils
 
 [![PyPI](https://img.shields.io/pypi/v/txt-utils.svg)](https://pypi.python.org/pypi/txt-utils)
 [![PyPI](https://img.shields.io/pypi/pyversions/txt-utils.svg)](https://pypi.python.org/pypi/txt-utils)
-[![MIT](https://img.shields.io/github/license/stefantaubert/txt-utils.svg)](https://github.com/stefantaubert/txt-utils/blob/main/LICENSE)
+[![MIT](https://img.shields.io/github/license/stefantaubert/txt-utils.svg)](https://github.com/stefantaubert/txt-utils/blob/master/LICENSE)
+[![PyPI](https://img.shields.io/github/commits-since/stefantaubert/txt-utils/latest/master.svg)](https://github.com/stefantaubert/txt-utils/compare/v0.0.3...master)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7986310.svg)](https://doi.org/10.5281/zenodo.7986310)
 
 CLI to modify text files.
 
 ## Features
 
 - `merge`: merge multiple text files into one
 - `extract-vocabulary`: extract unit vocabulary
@@ -63,14 +64,18 @@
 
 ## Usage
 
 ```sh
 txt-utils-cli
 ```
 
+## Contributing
+
+If you notice an error, please don't hesitate to open an issue.
+
 ## Dependencies
 
 - pandas
 - tqdm
 - ordered-set >=4.1.0
 - pronunciation-dictionary >=0.0.4
 
@@ -80,19 +85,17 @@
 
 ## Acknowledgments
 
 Funded by the Deutsche Forschungsgemeinschaft (DFG, German Research Foundation) – Project-ID 416228727 – CRC 1410
 
 ## Citation
 
-If you want to cite this repo, you can use this BibTeX-entry:
+If you want to cite this repo, you can use this BibTeX-entry generated by GitHub (see *About => Cite this repository*).
 
-```bibtex
-@misc{tstu22,
-  author = {Taubert, Stefan},
-  title = {txt-utils},
-  year = {2022},
-  publisher = {GitHub},
-  journal = {GitHub repository},
-  howpublished = {\url{https://github.com/stefantaubert/txt-utils}}
-}
-```
+## Changelog
+
+- 0.0.2 (2023-05-30)
+  - Bugfix: Merge multiple files
+  - Added:
+    - Support for Python 3.11
+- 0.0.1 (2022-05-30)
+  - Initial release
```

### Comparing `txt-utils-0.0.1/pyproject.toml` & `txt-utils-0.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "txt-utils"
-version = "0.0.1"
+version = "0.0.2"
 description = "CLI to modify text files."
 readme = "README.md"
-requires-python = ">=3.6"
+requires-python = ">=3.8, <4"
 license = {text = "MIT"}
 authors = [
-  {name = "Stefan Taubert", email = "stefan.taubert@posteo.me"}
+  {name = "Stefan Taubert", email = "pypi@stefantaubert.com"}
 ]
 maintainers = [
-  {name = "Stefan Taubert", email = "stefan.taubert@posteo.me"},
+  {name = "Stefan Taubert", email = "pypi@stefantaubert.com"},
 ]
 keywords = [
   "Preprocessing",
   "Processing",
   "Text-to-speech",
   "Speech synthesis",
   "Utils",
@@ -27,54 +27,48 @@
   "Operating System :: POSIX",
   "Operating System :: POSIX :: BSD",
   "Operating System :: POSIX :: Linux",
   "Operating System :: Unix",
   "Operating System :: Microsoft :: Windows",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.6",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "License :: OSI Approved :: MIT License",
 ]
 dependencies = [
   "pandas",
   "tqdm",
   "ordered_set>=4.1.0",
-  "pronunciation_dictionary>=0.0.4",
+  "pronunciation_dictionary>=0.0.5",
 ]
 
 [project.urls]
 Homepage = "https://github.com/stefantaubert/txt-utils"
 Issues = "https://github.com/stefantaubert/txt-utils/issues"
 
 [project.scripts]
 txt-utils-cli = "txt_utils_cli.cli:run_prod"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 include = [
-  "txt_utils",
   "txt_utils_cli"
 ]
 exclude = [
-  "txt_utils_tests",
   "txt_utils_debug",
-  "txt_utils_cli_debug",
-  "txt_utils_cli_tests",
 ]
 namespaces = true
 
 [tool.pytest.ini_options]
 log_cli = true
 log_level = "DEBUG"
 testpaths = [
-  "src/txt_utils_tests",
   "src/txt_utils_cli_tests"
 ]
 
 [tool.autopep8]
 indent-size = 2
 ignore = ["E121"]
 max_line_length = 100
@@ -105,13 +99,29 @@
   "**/__pycache__",
   ".git",
   "**/*.egg-info",
   "**/*_debug"
 ]
 useLibraryCodeForTypes = true
 
+[tool.tox]
+legacy_tox_ini = """
+[tox]
+envlist = py{38,39,310,311}
+isolated_build = True
+
+[testenv]
+deps = 
+  pytest
+commands = 
+  pytest
+  txt-utils-cli
+  txt-utils-cli -v
+  txt-utils-cli -h
+"""
+
 [build-system]
 requires = [
   "setuptools >= 40.9.0",
   "wheel",
 ]
 build-backend = "setuptools.build_meta"
```

### Comparing `txt-utils-0.0.1/src/txt_utils.egg-info/PKG-INFO` & `txt-utils-0.0.2/src/txt_utils.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 Metadata-Version: 2.1
 Name: txt-utils
-Version: 0.0.1
+Version: 0.0.2
 Summary: CLI to modify text files.
-Author-email: Stefan Taubert <stefan.taubert@posteo.me>
-Maintainer-email: Stefan Taubert <stefan.taubert@posteo.me>
+Author-email: Stefan Taubert <pypi@stefantaubert.com>
+Maintainer-email: Stefan Taubert <pypi@stefantaubert.com>
 License: MIT
 Project-URL: Homepage, https://github.com/stefantaubert/txt-utils
 Project-URL: Issues, https://github.com/stefantaubert/txt-utils/issues
 Keywords: Preprocessing,Processing,Text-to-speech,Speech synthesis,Utils,Language,Linguistics
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: BSD
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.6
+Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # txt-utils
 
 [![PyPI](https://img.shields.io/pypi/v/txt-utils.svg)](https://pypi.python.org/pypi/txt-utils)
 [![PyPI](https://img.shields.io/pypi/pyversions/txt-utils.svg)](https://pypi.python.org/pypi/txt-utils)
-[![MIT](https://img.shields.io/github/license/stefantaubert/txt-utils.svg)](https://github.com/stefantaubert/txt-utils/blob/main/LICENSE)
+[![MIT](https://img.shields.io/github/license/stefantaubert/txt-utils.svg)](https://github.com/stefantaubert/txt-utils/blob/master/LICENSE)
+[![PyPI](https://img.shields.io/github/commits-since/stefantaubert/txt-utils/latest/master.svg)](https://github.com/stefantaubert/txt-utils/compare/v0.0.3...master)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7986310.svg)](https://doi.org/10.5281/zenodo.7986310)
 
 CLI to modify text files.
 
 ## Features
 
 - `merge`: merge multiple text files into one
 - `extract-vocabulary`: extract unit vocabulary
@@ -63,14 +64,18 @@
 
 ## Usage
 
 ```sh
 txt-utils-cli
 ```
 
+## Contributing
+
+If you notice an error, please don't hesitate to open an issue.
+
 ## Dependencies
 
 - pandas
 - tqdm
 - ordered-set >=4.1.0
 - pronunciation-dictionary >=0.0.4
 
@@ -80,19 +85,17 @@
 
 ## Acknowledgments
 
 Funded by the Deutsche Forschungsgemeinschaft (DFG, German Research Foundation) – Project-ID 416228727 – CRC 1410
 
 ## Citation
 
-If you want to cite this repo, you can use this BibTeX-entry:
+If you want to cite this repo, you can use this BibTeX-entry generated by GitHub (see *About => Cite this repository*).
 
-```bibtex
-@misc{tstu22,
-  author = {Taubert, Stefan},
-  title = {txt-utils},
-  year = {2022},
-  publisher = {GitHub},
-  journal = {GitHub repository},
-  howpublished = {\url{https://github.com/stefantaubert/txt-utils}}
-}
-```
+## Changelog
+
+- 0.0.2 (2023-05-30)
+  - Bugfix: Merge multiple files
+  - Added:
+    - Support for Python 3.11
+- 0.0.1 (2022-05-30)
+  - Initial release
```

### Comparing `txt-utils-0.0.1/src/txt_utils.egg-info/SOURCES.txt` & `txt-utils-0.0.2/src/txt_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `txt-utils-0.0.1/src/txt_utils_cli/cli.py` & `txt-utils-0.0.2/src/txt_utils_cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,16 +137,16 @@
           "Not everything was successful! See log for details.")
       else:
         logger.error(
           "Not everything was successful!")
       flogger.error("Not everything was successful!")
 
     if changed_anything is not None and not changed_anything:
-      logger.info("Didn't changed anything.")
-      flogger.info("Didn't changed anything.")
+      logger.info("Didn't change anything.")
+      flogger.info("Didn't change anything.")
 
     duration = perf_counter() - start
     flogger.debug(f"Total duration (s): {duration}")
 
     if log_to_file:
       logger.info(f"Written log to: {ns.log.absolute()}")
```

### Comparing `txt-utils-0.0.1/src/txt_utils_cli/default_args.py` & `txt-utils-0.0.2/src/txt_utils_cli/default_args.py`

 * *Files identical despite different names*

### Comparing `txt-utils-0.0.1/src/txt_utils_cli/globals.py` & `txt-utils-0.0.2/src/txt_utils_cli/globals.py`

 * *Files identical despite different names*

### Comparing `txt-utils-0.0.1/src/txt_utils_cli/helper.py` & `txt-utils-0.0.2/src/txt_utils_cli/helper.py`

 * *Files identical despite different names*

### Comparing `txt-utils-0.0.1/src/txt_utils_cli/line_replacement.py` & `txt-utils-0.0.2/src/txt_utils_cli/line_replacement.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 from txt_utils_cli.helper import parse_non_empty
 from txt_utils_cli.logging_configuration import get_file_logger, init_and_get_console_logger
 
 
 def get_line_replacement_parser(parser: ArgumentParser):
   parser.description = "This command replaces a regex pattern for each line."
   add_file_arguments(parser)
-  parser.add_argument("pattern", type=parse_non_empty,
+  parser.add_argument("pattern", type=parse_non_empty, metavar="PATTERN",
                       help="replace regex pattern")
-  parser.add_argument("replace_with", type=str, metavar="replace-with",
+  parser.add_argument("replace_with", type=str, metavar="REPLACE-WITH",
                       help="replace pattern with this text")
   return line_replace_ns
 
 
 def line_replace_ns(ns: Namespace) -> ExecutionResult:
   logger = init_and_get_console_logger(__name__)
   flogger = get_file_logger()
@@ -40,14 +40,16 @@
   del content
 
   pattern = re.compile(ns.pattern)
   changed_counter = 0
   for line_nr, line in enumerate(tqdm(lines, desc="Replacing", unit=" line(s)")):
     line_new = pattern.sub(ns.replace_with, line)
     if line_new != line:
+      # Logging of this takes too much time
+      # logger.debug(f"Replaced \"{line}\" with \"{line_new}\".")
       lines[line_nr] = line_new
       changed_counter += 1
 
   if changed_counter == 0:
     logger.info("Didn't changed anything.")
     return True, False
```

### Comparing `txt-utils-0.0.1/src/txt_utils_cli/logging_configuration.py` & `txt-utils-0.0.2/src/txt_utils_cli/logging_configuration.py`

 * *Files identical despite different names*

### Comparing `txt-utils-0.0.1/src/txt_utils_cli/merging.py` & `txt-utils-0.0.2/src/txt_utils_cli/merging.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from argparse import ArgumentParser, Namespace
 from pathlib import Path
 from typing import cast
 
 from tqdm import tqdm
 
 from txt_utils_cli.globals import ExecutionResult
-from txt_utils_cli.helper import (ConvertToOrderedSetAction, add_encoding_argument,
-                                  parse_existing_file, parse_path)
+from txt_utils_cli.helper import add_encoding_argument, parse_existing_file, parse_path
 from txt_utils_cli.logging_configuration import get_file_logger, init_and_get_console_logger
 
 
 def get_merging_parser(parser: ArgumentParser):
   parser.description = "This command merges multiple text files into a single file."
   parser.add_argument("files", type=parse_existing_file,
-                      metavar="INPUT-FILE-PATH", nargs="+", help="text files that should be merged together", action=ConvertToOrderedSetAction)
+                      metavar="INPUT-FILE-PATH", nargs="+", help="text files that should be merged together")
   parser.add_argument("output", type=parse_path,
                       metavar="OUTPUT-FILE-PATH", help="output text file")
   parser.add_argument("--sep", type=str, default="\n", metavar="STRING",
                       help="separate file contents with this text while merging")
   add_encoding_argument(parser, "encoding of the input files and the output file")
   return merge_ns
 
@@ -32,23 +31,23 @@
   #   file
   #   for folder in ns.directories
   #   for file in get_all_files_in_all_subfolders(folder)
   #   if file.suffix.lower() in file_types
   # )
 
   texts = []
-  all_successfull = True
+  all_successful = True
   for path in tqdm(ns.files, desc="Reading text files", unit=" file(s)"):
     try:
       text = path.read_text(ns.encoding)
     except Exception as ex:
       flogger(f"File: {cast(Path, path).absolute()}")
       flogger.error("File couldn't be loaded!")
       flogger.exception(ex)
-      all_successfull = False
+      all_successful = False
       continue
     texts.append(text)
 
   logger.info("Merging files...")
   text = ns.sep.join(texts)
 
   logger.info("Saving merged output...")
@@ -59,15 +58,15 @@
     output.write_text(text, "UTF-8")
   except Exception as ex:
     logger.error("Output couldn't be saved!")
     flogger.exception(ex)
     return False, None
 
   logger.info(f"Written output to: {output.absolute()}")
-  return all_successfull, None
+  return all_successful, None
 
 
 # def get_all_files_in_all_subfolders(directory: Path) -> Generator[Path, None, None]:
 #   for root, _, files in os.walk(directory):
 #     for name in files:
 #       file_path = Path(root) / name
 #       yield file_path
```

### Comparing `txt-utils-0.0.1/src/txt_utils_cli/replacement.py` & `txt-utils-0.0.2/src/txt_utils_cli/replacement.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,27 +35,33 @@
   try:
     content = path.read_text(ns.encoding)
   except Exception as ex:
     logger.error("File couldn't be loaded!")
     flogger.exception(ex)
     return False, False
 
+  old_content = content
   logger.info("Replacing...")
   if ns.disable_regex:
     if ns.text not in content:
-      logger.info("File did not contained text. Nothing to replace.")
+      logger.info("File did not contained TEXT. Nothing to replace.")
       return True, False
     content = content.replace(ns.text, ns.replace_with)
   else:
     pattern = re.compile(ns.text)
     content = re.sub(pattern, ns.replace_with, content)
 
-  logger.info("Saving...")
-  try:
-    path.parent.mkdir(parents=True, exist_ok=True)
-    path.write_text(content, ns.encoding)
-  except Exception as ex:
-    logger.error("File couldn't be saved!")
-    flogger.exception(ex)
-    return False, False
+  changed_anything = content != old_content
+  del old_content
+
+  if changed_anything:
+    logger.info("Saving...")
+    try:
+      path.parent.mkdir(parents=True, exist_ok=True)
+      path.write_text(content, ns.encoding)
+    except Exception as ex:
+      logger.error("File couldn't be saved!")
+      flogger.exception(ex)
+      return False, False
   del content
-  return True, True
+
+  return True, changed_anything
```

### Comparing `txt-utils-0.0.1/src/txt_utils_cli/statistics_unit_counts.py` & `txt-utils-0.0.2/src/txt_utils_cli/statistics_unit_counts.py`

 * *Files identical despite different names*

### Comparing `txt-utils-0.0.1/src/txt_utils_cli/transcription.py` & `txt-utils-0.0.2/src/txt_utils_cli/transcription.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                       help="pronunciations separator", default="|")
   parser.add_argument("--seed", type=get_optional(parse_non_negative_integer),
                       help="seed for choosing the pronunciation from the dictionary regarding their weights (only useful if there exist words with multiple pronunciations)", default=None)
   parser.add_argument("--ignore-missing", action="store_true",
                       help="keep marks missing in dictionary unchanged")
   mp_group = add_mp_group(parser)
   mp_group.add_argument("-sd", "--chunksize-dictionary", type=parse_positive_integer,
-                        metavar="NUMBER", help="amount of lines to chunk into one job", default=100000)
+                        metavar="NUMBER", help="amount of lines to chunk into one job while parsing the dictionary", default=100000)
   add_deserialization_group(parser)
   return transcribe_ns
 
 
 def add_deserialization_group(parser: ArgumentParser) -> None:
   group = parser.add_argument_group('deserialization arguments')
   add_encoding_argument(group, "encoding of the dictionary", "--dict-encoding")
@@ -152,30 +152,30 @@
   global process_chunks
   global process_dict
   chunk = process_chunks[chunk_nr]
   return chunk_nr, get_vocab(chunk, wsep, process_dict, seed, ignore_missing, psep)
 
 
 def get_vocab(lines: List[str], wsep: str, dictionary: PronunciationDict, seed: Optional[int], ignore_missing: bool, psep: str) -> Set[str]:
-
+  new_wsep = f"{psep}{wsep}{psep}"
   new_lines = []
   for line in lines:
     words = line.split(wsep)
     words_transcribed = []
     for word in words:
       pronunciation = word
       if word not in dictionary:
         if not ignore_missing:
           continue
 
       pronunciations = dictionary[word]
       pronunciation = get_weighted_pronunciation(pronunciations, seed)
       pronunciation_str = psep.join(pronunciation)
       words_transcribed.append(pronunciation_str)
-    new_line = wsep.join(words_transcribed)
+    new_line = new_wsep.join(words_transcribed)
     if new_line != line:
       new_lines.append(new_line)
     else:
       new_lines.append(None)
 
   return new_lines
```

### Comparing `txt-utils-0.0.1/src/txt_utils_cli/trimming.py` & `txt-utils-0.0.2/src/txt_utils_cli/trimming.py`

 * *Files identical despite different names*

### Comparing `txt-utils-0.0.1/src/txt_utils_cli/unit_removal.py` & `txt-utils-0.0.2/src/txt_utils_cli/unit_removal.py`

 * *Files identical despite different names*

### Comparing `txt-utils-0.0.1/src/txt_utils_cli/vocabulary_exporting.py` & `txt-utils-0.0.2/src/txt_utils_cli/vocabulary_exporting.py`

 * *Files identical despite different names*

