# Comparing `tmp/metagene-0.0.0.dev4.tar.gz` & `tmp/metagene-0.0.0.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metagene-0.0.0.dev4.tar", max compression
+gzip compressed data, was "metagene-0.0.0.dev6.tar", max compression
```

## Comparing `metagene-0.0.0.dev4.tar` & `metagene-0.0.0.dev6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      507 2022-07-20 09:27:45.107276 metagene-0.0.0.dev4/README.md
--rw-r--r--   0        0        0     1298 2022-07-20 10:12:36.027264 metagene-0.0.0.dev4/metagene/cli.py
--rw-r--r--   0        0        0  2989344 2022-07-20 09:27:45.127276 metagene-0.0.0.dev4/metagene/data/GRCh38.bed.gz
--rw-r--r--   0        0        0    55130 2022-07-20 09:27:45.127276 metagene-0.0.0.dev4/metagene/data/input.bed.gz
--rw-r--r--   0        0        0     3388 2022-07-20 09:27:45.127276 metagene-0.0.0.dev4/metagene/get_features.py
--rw-r--r--   0        0        0     2458 2022-07-20 10:15:47.307263 metagene-0.0.0.dev4/metagene/overlap.py
--rw-r--r--   0        0        0      642 2022-07-20 10:18:42.467263 metagene-0.0.0.dev4/pyproject.toml
--rw-r--r--   0        0        0     1387 2022-07-20 10:18:58.779215 metagene-0.0.0.dev4/setup.py
--rw-r--r--   0        0        0     1355 2022-07-20 10:18:58.779391 metagene-0.0.0.dev4/PKG-INFO
+-rw-r--r--   0        0        0      507 2022-07-09 06:24:44.527600 metagene-0.0.0.dev6/README.md
+-rw-r--r--   0        0        0     1298 2022-07-21 01:21:05.770670 metagene-0.0.0.dev6/metagene/cli.py
+-rw-r--r--   0        0        0  2989344 2022-07-21 01:21:05.790670 metagene-0.0.0.dev6/metagene/data/GRCh38.bed.gz
+-rw-r--r--   0        0        0    55130 2022-07-21 01:21:05.790670 metagene-0.0.0.dev6/metagene/data/input.bed.gz
+-rw-r--r--   0        0        0     3388 2022-07-19 04:55:10.556067 metagene-0.0.0.dev6/metagene/get_features.py
+-rw-r--r--   0        0        0     2943 2022-07-23 00:48:10.020670 metagene-0.0.0.dev6/metagene/overlap.py
+-rw-r--r--   0        0        0      660 2022-07-21 01:21:05.800670 metagene-0.0.0.dev6/pyproject.toml
+-rw-r--r--   0        0        0     1412 2022-07-23 00:49:13.409538 metagene-0.0.0.dev6/setup.py
+-rw-r--r--   0        0        0     1394 2022-07-23 00:49:13.409730 metagene-0.0.0.dev6/PKG-INFO
```

### Comparing `metagene-0.0.0.dev4/metagene/cli.py` & `metagene-0.0.0.dev6/metagene/cli.py`

 * *Files identical despite different names*

### Comparing `metagene-0.0.0.dev4/metagene/data/GRCh38.bed.gz` & `metagene-0.0.0.dev6/metagene/data/GRCh38.bed.gz`

 * *Files identical despite different names*

### Comparing `metagene-0.0.0.dev4/metagene/data/input.bed.gz` & `metagene-0.0.0.dev6/metagene/data/input.bed.gz`

 * *Files identical despite different names*

### Comparing `metagene-0.0.0.dev4/metagene/get_features.py` & `metagene-0.0.0.dev6/metagene/get_features.py`

 * *Files identical despite different names*

### Comparing `metagene-0.0.0.dev4/pyproject.toml` & `metagene-0.0.0.dev6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
 requires = ["poetry>=1.0"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "metagene"
-version = "0.0.0.dev4"
+version = "0.0.0.dev6"
 description = "Metagene Profiling Analysis and Visualization"
 authors = ["Ye Chang <yech1990@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/y9c/metagene"
 documentation = "https://cf.readthedocs.io/"
 keywords = ["DNA", "RNA", "metagene", "biology"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-Click = "^7.0.0"
+Click = "^8.0.0"
 matplotlib = "^3.0.0"
 pyranges = "^0.0.117"
 ray = "^1.13.0"
+pandas = "^1.4.3"
 
 [tool.poetry.dev-dependencies]
 twine = "^3.1.1"
 
 [tool.poetry.scripts]
 metagene = "metagene.cli:cli"
```

### Comparing `metagene-0.0.0.dev4/setup.py` & `metagene-0.0.0.dev6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 packages = \
 ['metagene']
 
 package_data = \
 {'': ['*'], 'metagene': ['data/*']}
 
 install_requires = \
-['Click>=7.0.0,<8.0.0',
+['Click>=8.0.0,<9.0.0',
  'matplotlib>=3.0.0,<4.0.0',
+ 'pandas>=1.4.3,<2.0.0',
  'pyranges>=0.0.117,<0.0.118',
  'ray>=1.13.0,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['metagene = metagene.cli:cli']}
 
 setup_kwargs = {
     'name': 'metagene',
-    'version': '0.0.0.dev4',
+    'version': '0.0.0.dev6',
     'description': 'Metagene Profiling Analysis and Visualization',
     'long_description': '# Metagene\n\n[![Readthedocs](https://readthedocs.org/projects/metagene/badge/?version=latest)](https://metagene.readthedocs.io/en/latest/?badge=latest)\n[![Build Status](https://img.shields.io/travis/y9c/metagene.svg)](https://travis-ci.com/y9c/metagene)\n[![Pypi Releases](https://img.shields.io/pypi/v/metagene.svg)](https://pypi.python.org/pypi/metagene)\n[![Downloads](https://pepy.tech/badge/metagene)](https://pepy.tech/project/metagene)\n\n**Metagene Profiling Analysis and Visualization**\n\n(WIP)\n\n## Demo\n',
     'author': 'Ye Chang',
     'author_email': 'yech1990@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/y9c/metagene',
```

### Comparing `metagene-0.0.0.dev4/PKG-INFO` & `metagene-0.0.0.dev6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: metagene
-Version: 0.0.0.dev4
+Version: 0.0.0.dev6
 Summary: Metagene Profiling Analysis and Visualization
 Home-page: https://github.com/y9c/metagene
 License: MIT
 Keywords: DNA,RNA,metagene,biology
 Author: Ye Chang
 Author-email: yech1990@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: Click (>=7.0.0,<8.0.0)
+Requires-Dist: Click (>=8.0.0,<9.0.0)
 Requires-Dist: matplotlib (>=3.0.0,<4.0.0)
+Requires-Dist: pandas (>=1.4.3,<2.0.0)
 Requires-Dist: pyranges (>=0.0.117,<0.0.118)
 Requires-Dist: ray (>=1.13.0,<2.0.0)
 Project-URL: Documentation, https://cf.readthedocs.io/
 Project-URL: Repository, https://github.com/y9c/metagene
 Description-Content-Type: text/markdown
 
 # Metagene
```

