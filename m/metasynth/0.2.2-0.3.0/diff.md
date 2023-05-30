# Comparing `tmp/metasynth-0.2.2.tar.gz` & `tmp/metasynth-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metasynth-0.2.2.tar", last modified: Fri Mar  3 13:47:46 2023, max compression
+gzip compressed data, was "metasynth-0.3.0.tar", last modified: Tue May 30 10:06:34 2023, max compression
```

## Comparing `metasynth-0.2.2.tar` & `metasynth-0.3.0.tar`

### file list

```diff
@@ -1,77 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 13:47:46.749350 metasynth-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 13:47:46.741350 metasynth-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 13:47:46.741350 metasynth-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-03-03 13:47:37.000000 metasynth-0.2.2/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-03-03 13:47:37.000000 metasynth-0.2.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-03-03 13:47:37.000000 metasynth-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-03-03 13:47:37.000000 metasynth-0.2.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-03-03 13:47:37.000000 metasynth-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-03-03 13:47:46.749350 metasynth-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-03-03 13:47:37.000000 metasynth-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 13:47:46.741350 metasynth-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-03 13:47:37.000000 metasynth-0.2.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-03-03 13:47:37.000000 metasynth-0.2.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-03 13:47:37.000000 metasynth-0.2.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    85618 2023-03-03 13:47:37.000000 metasynth-0.2.2/docs/soda.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 13:47:46.745350 metasynth-0.2.2/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 13:47:46.745350 metasynth-0.2.2/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-03-03 13:47:37.000000 metasynth-0.2.2/docs/source/api/metasynth.distribution.regex.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-03-03 13:47:37.000000 metasynth-0.2.2/docs/source/api/metasynth.distribution.rst
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-03-03 13:47:37.000000 metasynth-0.2.2/docs/source/api/metasynth.rst
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-03 13:47:37.000000 metasynth-0.2.2/docs/source/api/metasynth.schema.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-03-03 13:47:37.000000 metasynth-0.2.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-03-03 13:47:37.000000 metasynth-0.2.2/docs/source/developer.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-03-03 13:47:37.000000 metasynth-0.2.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-03-03 13:47:37.000000 metasynth-0.2.2/docs/source/quick_start.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 13:47:46.745350 metasynth-0.2.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    86442 2023-03-03 13:47:37.000000 metasynth-0.2.2/examples/advanced_tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-03-03 13:47:37.000000 metasynth-0.2.2/examples/basic_example.json
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-03-03 13:47:37.000000 metasynth-0.2.2/examples/basic_example.py
--rw-r--r--   0 runner    (1001) docker     (123)    81698 2023-03-03 13:47:37.000000 metasynth-0.2.2/examples/demonstration.csv
--rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-03-03 13:47:37.000000 metasynth-0.2.2/examples/descriptions.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    54216 2023-03-03 13:47:37.000000 metasynth-0.2.2/examples/titanic.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-03-03 13:47:37.000000 metasynth-0.2.2/examples/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 13:47:46.745350 metasynth-0.2.2/metasynth/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-03-03 13:47:37.000000 metasynth-0.2.2/metasynth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-03 13:47:46.000000 metasynth-0.2.2/metasynth/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10240 2023-03-03 13:47:37.000000 metasynth-0.2.2/metasynth/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 13:47:46.745350 metasynth-0.2.2/metasynth/distribution/
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-03-03 13:47:37.000000 metasynth-0.2.2/metasynth/distribution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-03-03 13:47:37.000000 metasynth-0.2.2/metasynth/distribution/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-03-03 13:47:37.000000 metasynth-0.2.2/metasynth/distribution/categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-03-03 13:47:37.000000 metasynth-0.2.2/metasynth/distribution/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-03-03 13:47:37.000000 metasynth-0.2.2/metasynth/distribution/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-03-03 13:47:37.000000 metasynth-0.2.2/metasynth/distribution/discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-03-03 13:47:37.000000 metasynth-0.2.2/metasynth/distribution/faker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 13:47:46.749350 metasynth-0.2.2/metasynth/distribution/regex/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-03 13:47:37.000000 metasynth-0.2.2/metasynth/distribution/regex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-03-03 13:47:37.000000 metasynth-0.2.2/metasynth/distribution/regex/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17577 2023-03-03 13:47:37.000000 metasynth-0.2.2/metasynth/distribution/regex/element.py
--rw-r--r--   0 runner    (1001) docker     (123)    11471 2023-03-03 13:47:37.000000 metasynth-0.2.2/metasynth/distribution/regex/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10454 2023-03-03 13:47:37.000000 metasynth-0.2.2/metasynth/disttree.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-03 13:47:37.000000 metasynth-0.2.2/metasynth/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 13:47:46.749350 metasynth-0.2.2/metasynth/schema/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-03 13:47:37.000000 metasynth-0.2.2/metasynth/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-03-03 13:47:37.000000 metasynth-0.2.2/metasynth/schema/generative_metadata_format.json
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-03-03 13:47:37.000000 metasynth-0.2.2/metasynth/testutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-03-03 13:47:37.000000 metasynth-0.2.2/metasynth/var.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 13:47:46.745350 metasynth-0.2.2/metasynth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-03-03 13:47:46.000000 metasynth-0.2.2/metasynth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-03-03 13:47:46.000000 metasynth-0.2.2/metasynth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 13:47:46.000000 metasynth-0.2.2/metasynth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-03-03 13:47:46.000000 metasynth-0.2.2/metasynth.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-03 13:47:46.000000 metasynth-0.2.2/metasynth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-03 13:47:46.000000 metasynth-0.2.2/metasynth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-03-03 13:47:37.000000 metasynth-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-03 13:47:46.749350 metasynth-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 13:47:46.749350 metasynth-0.2.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 13:47:46.749350 metasynth-0.2.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    60302 2023-03-03 13:47:37.000000 metasynth-0.2.2/tests/data/titanic.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-03-03 13:47:37.000000 metasynth-0.2.2/tests/test_continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-03-03 13:47:37.000000 metasynth-0.2.2/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-03-03 13:47:37.000000 metasynth-0.2.2/tests/test_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-03-03 13:47:37.000000 metasynth-0.2.2/tests/test_discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-03-03 13:47:37.000000 metasynth-0.2.2/tests/test_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-03-03 13:47:37.000000 metasynth-0.2.2/tests/test_faker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-03-03 13:47:37.000000 metasynth-0.2.2/tests/test_regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     8294 2023-03-03 13:47:37.000000 metasynth-0.2.2/tests/test_var.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:06:34.425552 metasynth-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:06:34.413552 metasynth-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:06:34.417552 metasynth-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-30 10:06:22.000000 metasynth-0.3.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-30 10:06:22.000000 metasynth-0.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-30 10:06:22.000000 metasynth-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-30 10:06:22.000000 metasynth-0.3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-30 10:06:22.000000 metasynth-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-05-30 10:06:34.425552 metasynth-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-05-30 10:06:22.000000 metasynth-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:06:34.417552 metasynth-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-30 10:06:22.000000 metasynth-0.3.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-30 10:06:22.000000 metasynth-0.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-30 10:06:22.000000 metasynth-0.3.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    85618 2023-05-30 10:06:22.000000 metasynth-0.3.0/docs/soda.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:06:34.417552 metasynth-0.3.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:06:34.417552 metasynth-0.3.0/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-30 10:06:22.000000 metasynth-0.3.0/docs/source/api/metasynth.distribution.regex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-30 10:06:22.000000 metasynth-0.3.0/docs/source/api/metasynth.distribution.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-30 10:06:22.000000 metasynth-0.3.0/docs/source/api/metasynth.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-30 10:06:22.000000 metasynth-0.3.0/docs/source/api/metasynth.schema.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-30 10:06:22.000000 metasynth-0.3.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-05-30 10:06:22.000000 metasynth-0.3.0/docs/source/developer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-30 10:06:22.000000 metasynth-0.3.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-30 10:06:22.000000 metasynth-0.3.0/docs/source/quick_start.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:06:34.417552 metasynth-0.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    59754 2023-05-30 10:06:22.000000 metasynth-0.3.0/examples/advanced_tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-30 10:06:22.000000 metasynth-0.3.0/examples/basic_example.json
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-30 10:06:22.000000 metasynth-0.3.0/examples/basic_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81698 2023-05-30 10:06:22.000000 metasynth-0.3.0/examples/demonstration.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12709 2023-05-30 10:06:22.000000 metasynth-0.3.0/examples/descriptions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    37464 2023-05-30 10:06:22.000000 metasynth-0.3.0/examples/titanic.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-30 10:06:22.000000 metasynth-0.3.0/examples/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:06:34.421552 metasynth-0.3.0/metasynth/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-30 10:06:34.000000 metasynth-0.3.0/metasynth/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:06:34.421552 metasynth-0.3.0/metasynth/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/demo/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81698 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/demo/demo_titanic.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:06:34.421552 metasynth-0.3.0/metasynth/distribution/
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/distribution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/distribution/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/distribution/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/distribution/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/distribution/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/distribution/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/distribution/faker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:06:34.421552 metasynth-0.3.0/metasynth/distribution/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/distribution/regex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/distribution/regex/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17577 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/distribution/regex/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11484 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/distribution/regex/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/privacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:06:34.421552 metasynth-0.3.0/metasynth/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/schema/generative_metadata_format.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10119 2023-05-30 10:06:22.000000 metasynth-0.3.0/metasynth/var.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:06:34.421552 metasynth-0.3.0/metasynth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-05-30 10:06:34.000000 metasynth-0.3.0/metasynth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-30 10:06:34.000000 metasynth-0.3.0/metasynth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:06:34.000000 metasynth-0.3.0/metasynth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-30 10:06:34.000000 metasynth-0.3.0/metasynth.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-30 10:06:34.000000 metasynth-0.3.0/metasynth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-30 10:06:34.000000 metasynth-0.3.0/metasynth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-30 10:06:22.000000 metasynth-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 10:06:34.425552 metasynth-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:06:34.421552 metasynth-0.3.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:06:34.421552 metasynth-0.3.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    60302 2023-05-30 10:06:22.000000 metasynth-0.3.0/tests/data/titanic.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-30 10:06:22.000000 metasynth-0.3.0/tests/test_builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-30 10:06:22.000000 metasynth-0.3.0/tests/test_continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-05-30 10:06:22.000000 metasynth-0.3.0/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-05-30 10:06:22.000000 metasynth-0.3.0/tests/test_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-30 10:06:22.000000 metasynth-0.3.0/tests/test_discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-30 10:06:22.000000 metasynth-0.3.0/tests/test_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-30 10:06:22.000000 metasynth-0.3.0/tests/test_faker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-30 10:06:22.000000 metasynth-0.3.0/tests/test_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-05-30 10:06:22.000000 metasynth-0.3.0/tests/test_var.py
```

### Comparing `metasynth-0.2.2/.github/workflows/python-package.yml` & `metasynth-0.3.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `metasynth-0.2.2/.github/workflows/python-publish.yml` & `metasynth-0.3.0/.github/workflows/python-publish.yml`

 * *Files 24% similar despite different names*

```diff
@@ -29,11 +29,11 @@
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install build
     - name: Build package
       run: python -m build
     - name: Publish package
-      uses: pypa/gh-action-pypi-publish@27b31702a0e7fc50959f5ad993c78deac1bdfc29
+      uses: pypa/gh-action-pypi-publish@7eb3b701d11256e583f5b49899c5e7203deab573
       with:
         user: __token__
         password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `metasynth-0.2.2/.gitignore` & `metasynth-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `metasynth-0.2.2/.readthedocs.yaml` & `metasynth-0.3.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `metasynth-0.2.2/LICENSE` & `metasynth-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metasynth-0.2.2/PKG-INFO` & `metasynth-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metasynth
-Version: 0.2.2
+Version: 0.3.0
 Summary: Package for creating synthetic datasets while preserving privacy.
 Author-email: Raoul Schram <r.d.schram@uu.nl>, Erik-Jan van Kesteren <e.vankesteren1@uu.nl>
 License: MIT License
         
         Copyright (c) 2022 SoDa
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,14 +38,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/metasynth)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sodascience/metasynth/HEAD?labpath=examples%2Fadvanced_tutorial.ipynb)
+[![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sodascience/metasynth/blob/main/examples/advanced_tutorial.ipynb)
 [![docs](https://readthedocs.org/projects/metasynth/badge/?version=latest)](https://metasynth.readthedocs.io/en/latest/index.html)
 
 # MetaSynth
 
 MetaSynth is a python package to generate synthetic data mostly geared towards code testing and reproducibility.
 Using the [ONS methodology](https://www.ons.gov.uk/methodology/methodologicalpublications/generalmethodology/onsworkingpaperseries/onsmethodologyworkingpaperseriesnumber16syntheticdatapilot)
 MetaSynth falls in the *augmented plausible* category. To generate synthetic data, MetaSynth converts a polars DataFrame
```

### Comparing `metasynth-0.2.2/README.md` & `metasynth-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/metasynth)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sodascience/metasynth/HEAD?labpath=examples%2Fadvanced_tutorial.ipynb)
+[![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sodascience/metasynth/blob/main/examples/advanced_tutorial.ipynb)
 [![docs](https://readthedocs.org/projects/metasynth/badge/?version=latest)](https://metasynth.readthedocs.io/en/latest/index.html)
 
 # MetaSynth
 
 MetaSynth is a python package to generate synthetic data mostly geared towards code testing and reproducibility.
 Using the [ONS methodology](https://www.ons.gov.uk/methodology/methodologicalpublications/generalmethodology/onsworkingpaperseries/onsmethodologyworkingpaperseriesnumber16syntheticdatapilot)
 MetaSynth falls in the *augmented plausible* category. To generate synthetic data, MetaSynth converts a polars DataFrame
```

### Comparing `metasynth-0.2.2/docs/Makefile` & `metasynth-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `metasynth-0.2.2/docs/make.bat` & `metasynth-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `metasynth-0.2.2/docs/soda.png` & `metasynth-0.3.0/docs/soda.png`

 * *Files identical despite different names*

### Comparing `metasynth-0.2.2/docs/source/api/metasynth.distribution.regex.rst` & `metasynth-0.3.0/docs/source/api/metasynth.distribution.regex.rst`

 * *Files identical despite different names*

### Comparing `metasynth-0.2.2/docs/source/api/metasynth.distribution.rst` & `metasynth-0.3.0/docs/source/api/metasynth.distribution.rst`

 * *Files identical despite different names*

### Comparing `metasynth-0.2.2/docs/source/conf.py` & `metasynth-0.3.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `metasynth-0.2.2/docs/source/developer.rst` & `metasynth-0.3.0/docs/source/developer.rst`

 * *Files identical despite different names*

### Comparing `metasynth-0.2.2/docs/source/index.rst` & `metasynth-0.3.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `metasynth-0.2.2/docs/source/quick_start.rst` & `metasynth-0.3.0/docs/source/quick_start.rst`

 * *Files identical despite different names*

### Comparing `metasynth-0.2.2/examples/basic_example.json` & `metasynth-0.3.0/examples/basic_example.json`

 * *Files identical despite different names*

### Comparing `metasynth-0.2.2/examples/basic_example.py` & `metasynth-0.3.0/examples/basic_example.py`

 * *Files identical despite different names*

### Comparing `metasynth-0.2.2/examples/demonstration.csv` & `metasynth-0.3.0/examples/demonstration.csv`

 * *Files identical despite different names*

### Comparing `metasynth-0.2.2/examples/descriptions.ipynb` & `metasynth-0.3.0/examples/descriptions.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9909931077694236%*

 * *Differences: {"'cells'": "{11: {'source': {insert: [(0, 'from metasynth.distribution import "*

 * *            'FakerDistribution\\n\'), (4, \'        "Name": {"distribution": '*

 * *            'FakerDistribution("name")},\\n\'), (8, \'        "Cabin": {"distribution": '*

 * *            'FakerDistribution("city"), "description": "The cabin number of the '*

 * *            'passenger."},\\n\')], delete: [7, 3]}}, insert: [(18, OrderedDict([(\'cell_type\', '*

 * *            "'code'), ('execution_count', None), ('id', 'c17f41a7'), ('metadata',  […]*

```diff
@@ -284,22 +284,23 @@
                     "output_type": "stream",
                     "text": [
                         "{'Cabin': 'The cabin number of the passenger.'}\n"
                     ]
                 }
             ],
             "source": [
+                "from metasynth.distribution import FakerDistribution\n",
                 "meta_dataset = MetaDataset.from_dataframe(\n",
                 "    df,\n",
                 "    spec={\n",
-                "        \"Name\": {\"distribution\": \"faker.name\"},\n",
+                "        \"Name\": {\"distribution\": FakerDistribution(\"name\")},\n",
                 "        \"Fare\": {\"distribution\": \"LogNormalDistribution\"},\n",
                 "        \"Age\": {\"distribution\": DiscreteUniformDistribution(20, 40)},\n",
                 "        \"PassengerId\": {\"unique\": True},\n",
-                "        \"Cabin\": {\"distribution\": \"faker.city\", \"description\": \"The cabin number of the passenger.\"},\n",
+                "        \"Cabin\": {\"distribution\": FakerDistribution(\"city\"), \"description\": \"The cabin number of the passenger.\"},\n",
                 "    }\n",
                 ")\n",
                 "pprint(meta_dataset.descriptions)"
             ]
         },
         {
             "cell_type": "markdown",
@@ -392,14 +393,22 @@
                     ]
                 }
             ],
             "source": [
                 "meta_dataset.descriptions = [var.name for var in meta_dataset.meta_vars]\n",
                 "pprint(meta_dataset.descriptions)"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "c17f41a7",
+            "metadata": {},
+            "outputs": [],
+            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
@@ -410,13 +419,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.4"
+            "version": "3.9.10"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `metasynth-0.2.2/examples/utils.py` & `metasynth-0.3.0/examples/utils.py`

 * *Files identical despite different names*

### Comparing `metasynth-0.2.2/metasynth/dataset.py` & `metasynth-0.3.0/metasynth/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """Conversion of pandas dataframes to MetaSynth datasets."""   # pylint: disable=invalid-name
 
 from __future__ import annotations
 
+import json
+import pathlib
 from copy import deepcopy
 from datetime import datetime
-from importlib.resources import read_text
 from importlib.metadata import version
-import json
-import pathlib
-from typing import Union, List, Dict, Any, Sequence, Optional
+from importlib.resources import read_text
+from typing import Any, Dict, List, Optional, Sequence, Union
 
+import jsonschema
 import numpy as np
 import polars as pl
-import jsonschema
 
+from metasynth.privacy import BasePrivacy, BasicPrivacy
+from metasynth.provider import BaseDistributionProvider
+from metasynth.validation import validate_gmf_dict
 from metasynth.var import MetaVar
-from metasynth.disttree import get_disttree
 
 
 class MetaDataset():
     """MetaSynth dataset consisting of variables.
 
     The MetaSynth dataset structure that is most easily created from
     a pandas dataset with the from_dataframe class method.
@@ -31,31 +33,30 @@
     n_rows:
         Number of rows in the original dataframe.
     privacy_package:
         Package that supplies the distributions.
     """
 
     def __init__(self, meta_vars: List[MetaVar],
-                 n_rows: Optional[int] = None,
-                 privacy_package: Optional[str] = None):
+                 n_rows: Optional[int] = None):
         self.meta_vars = meta_vars
         self.n_rows = n_rows
-        self.privacy_package = privacy_package
 
     @property
     def n_columns(self) -> int:
         """int: Number of columns of the original dataframe."""
         return len(self.meta_vars)
 
     @classmethod
     def from_dataframe(cls,
                        df: pl.DataFrame,
                        spec: Optional[dict[str, dict]] = None,
-                       privacy_package: Optional[str] = None,
-                       **privacy_kwargs):
+                       dist_providers: Union[str, list[str], BaseDistributionProvider,
+                                             list[BaseDistributionProvider]] = "builtin",
+                       privacy: Optional[BasePrivacy] = None):
         """Create dataset from a Pandas dataframe.
 
         The pandas dataframe should be formatted already with the correct
         datatypes.
 
         Parameters
         ----------
@@ -87,73 +88,70 @@
             assumed to be not unique, but might give a warning if it is detected that it might
             be.
 
             description
 
             Set the description of a variable: {"description": "Some description."}
 
-            fit_kwargs
+            privacy
 
-            Some distributions such as the FakerDistribution and RegexDistribution can take
-            extra fitting arguments. For example for the RegexDistribution one can set the
-            the speed of the computation by {"mode": "fast"} or {"mode": "slow"}. Be sure to set
-            the distribution as well.
+            Set the privacy level for a variable: {"privacy": DifferentialPrivacy(epsilon=10)}
 
-            Any number of the above directives may be set for any number of variables.
+            prop_missing
 
-        privacy_package:
-            Package that contains the implementations of the distributions.
+            Proportion of missing values for a variable: {"prop_missing": 0.3}
+
+            Any number of the above directives may be set for any number of variables.
+        dist_providers:
+            Distribution providers to use when fitting distributions to variables.
+            Can be a string, provider, or provider type.
+        privacy:
+            Privacy level to use by default.
 
         Returns
         -------
         MetaDataset:
             Initialized MetaSynth dataset.
         """
-        distribution_tree = get_disttree(privacy_package, **privacy_kwargs)
-
+        if privacy is None:
+            privacy = BasicPrivacy()
         if spec is None:
             spec = {}
         else:
             spec = deepcopy(spec)
 
         all_vars = []
         for col_name in df.columns:
             series = df[col_name]
             col_spec = spec.get(col_name, {})
             dist = col_spec.pop("distribution", None)
             unq = col_spec.pop("unique", None)
             description = col_spec.pop("description", None)
-            fit_kwargs = col_spec.pop("fit_kwargs", {})
             prop_missing = col_spec.pop("prop_missing", None)
-            assert "fit_kwargs" not in col_spec
-            if dist is None and len(fit_kwargs) > 0:
-                raise ValueError(f"Got fit arguments for variable '{col_name}', but no "
-                                 "distribution. Set the distribution manually to fix.")
+            cur_privacy = col_spec.pop("privacy", privacy)
+            fit_kwargs = col_spec.pop("fit_kwargs", {})
             if len(col_spec) != 0:
                 raise ValueError(f"Unknown spec items '{col_spec}' for variable '{col_name}'.")
             var = MetaVar.detect(series, description=description, prop_missing=prop_missing)
-            if dist is None:
-                var.fit(distribution_tree=distribution_tree, unique=unq, **fit_kwargs)
-            else:
-                var.fit(distribution_tree=distribution_tree, dist=dist, unique=unq, **fit_kwargs)
+            var.fit(dist=dist, dist_providers=dist_providers, unique=unq, privacy=cur_privacy,
+                    fit_kwargs=fit_kwargs)
 
             all_vars.append(var)
 
-        return cls(all_vars, len(df), privacy_package=privacy_package)
+        return cls(all_vars, len(df))
 
     def to_dict(self) -> Dict[str, Any]:
         """Create dictionary with the properties for recreation."""
         return {
             "n_rows": self.n_rows,
             "n_columns": self.n_columns,
             "provenance": {
                 "created by": {
                     "name": "MetaSynth",
                     "version": version("metasynth"),
-                    "privacy": self.privacy_package,
                 },
                 "creation time": datetime.now().isoformat()
             },
             "vars": [var.to_dict() for var in self.meta_vars],
         }
 
     def __getitem__(self, key: Union[int, str]) -> MetaVar:
@@ -205,16 +203,15 @@
         fp:
             File to write the dataset to.
         validate:
             Validate the JSON file with a schema.
         """
         self_dict = _jsonify(self.to_dict())
         if validate:
-            schema = json.loads(read_text("metasynth.schema", "generative_metadata_format.json"))
-            jsonschema.validate(instance=self_dict, schema=schema)
+            validate_gmf_dict(self_dict)
         with open(fp, "w", encoding="utf-8") as f:
             json.dump(self_dict, f, indent=4)
 
     @classmethod
     def from_json(cls, fp: Union[pathlib.Path, str], validate: bool = True) -> MetaDataset:
         """Read a MetaSynth dataset from a JSON file.
```

### Comparing `metasynth-0.2.2/metasynth/distribution/base.py` & `metasynth-0.3.0/metasynth/distribution/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 """Module for the base distribution and the scipy distribution."""
 
 from __future__ import annotations
+
 from abc import ABC, abstractmethod
 from copy import deepcopy
-from typing import List, Iterable, Dict, Sequence, Union
+from typing import Iterable, Sequence, Union
 
 import numpy as np
-import polars as pl
 import pandas as pd
+import polars as pl
 
 
 class BaseDistribution(ABC):
     """Abstract base class to define a distribution.
 
     All distributions should be derived from this class, and the following
     methods need to be implemented: _fit, draw, to_dict.
     """
 
-    aliases: List[str] = []
+    implements = "unknown"
+    provenance = "unknown"
+    privacy = "unknown"
     is_unique = False
     var_type: str = "unknown"
 
     @classmethod
     def fit(cls, series: Union[Sequence, pl.Series], *args, **kwargs) -> BaseDistribution:
         """Fit the distribution to the series.
 
@@ -66,16 +69,48 @@
         """Reset the drawing of elements to start again."""
 
     def __str__(self) -> str:
         """Create a human readable string of the object."""
         return str(self.to_dict())
 
     @abstractmethod
-    def to_dict(self) -> Dict:
+    def _param_dict(self):
+        """Get dictionary with the parameters of the distribution."""
+
+    def to_dict(self) -> dict:
         """Convert the distribution to a dictionary."""
+        return {
+            "implements": self.implements,
+            "provenance": self.provenance,
+            "class_name": self.__class__.__name__,
+            "parameters": deepcopy(self._param_dict()),
+        }
+
+    @classmethod
+    @abstractmethod
+    def _param_schema(cls):
+        """Get schema for the parameters of the distribution."""
+
+    @classmethod
+    def schema(cls) -> dict:
+        """Create sub-schema to validate GMF file."""
+        return {
+            "type": "object",
+            "properties": {
+                "implements": {"const": cls.implements},
+                "provenance": {"const": cls.provenance},
+                "class_name": {"const": cls.__name__},
+                "parameters": {
+                    "type": "object",
+                    "properties": cls._param_schema(),
+                    "required": list(cls.default_distribution()._param_dict())
+                }
+            },
+            "required": ["implements", "provenance", "class_name", "parameters"]
+        }
 
     @classmethod
     def from_dict(cls, dist_dict: dict) -> BaseDistribution:
         """Create a distribution from a dictionary."""
         return cls(**dist_dict["parameters"])
 
     def information_criterion(self, values: Iterable) -> float:  # pylint: disable=unused-argument
@@ -85,57 +120,47 @@
         ----------
         values: array_like
             Values to determine the AIC value of.
         """
         return 0.0
 
     @classmethod
-    def is_named(cls, name: str) -> bool:
+    def matches_name(cls, name: str) -> bool:
         """Check whether the name matches the distribution.
 
         Parameters
         ----------
         name: str
             Name to match to the distribution.
 
         Returns
         -------
         bool:
             Whether the name matches.
         """
-        return name in cls.aliases or name == type(cls).__name__ or name == cls.__name__
-
-    @classmethod
-    def fit_kwargs(cls, name: str) -> Dict:  # pylint: disable=unused-argument
-        """Extra fitting arguments.
-
-        Parameters
-        ----------
-        name: str
-            Name to be matched.
-
-        Returns
-        -------
-        dict:
-            Keyword arguments extracted from the name.
-        """
-        return {}
-
-    @property
-    def name(self) -> str:
-        """Return the name used in the metadata file."""
-        return self.aliases[0]
+        assert cls.implements != "unknown", f"Internal error in class {cls.__name__}"
+        return name in (cls.implements.split(".")[1],
+                        cls.implements,
+                        cls.__name__,
+                        )
 
     @classmethod
     @abstractmethod
     def default_distribution(cls) -> BaseDistribution:
         """Get a distribution with default parameters."""
         return cls()
 
 
+class CoreDistribution():  # pylint: disable=too-few-public-methods
+    """Distributions belonging to the core set."""
+
+    privacy = "none"
+    provenance = "builtin"
+
+
 class CategoricalDistribution(BaseDistribution):
     """Base Class for categorical distributions."""
 
     var_type = "categorical"
 
 
 class DiscreteDistribution(BaseDistribution):
@@ -210,19 +235,16 @@
     @classmethod
     def _fit(cls, values):
         if len(values) == 0:
             return cls.default_distribution()
         param = cls.dist_class.fit(values)
         return cls(*param)
 
-    def to_dict(self):
-        return {
-            "name": self.name,
-            "parameters": deepcopy(self.par),
-        }
+    def _param_dict(self):
+        return self.par
 
     def draw(self):
         return self.dist.rvs()
 
     def information_criterion(self, values):
         vals = self._to_series(values)
         if len(vals) == 0:
```

### Comparing `metasynth-0.2.2/metasynth/distribution/categorical.py` & `metasynth-0.3.0/metasynth/distribution/categorical.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,70 @@
 """Module containing categorical distributions."""
 
 from typing import Union
 
-import pandas as pd
 import numpy as np
 import numpy.typing as npt
+import pandas as pd
 import polars as pl
 
-from metasynth.distribution.base import CategoricalDistribution
+from metasynth.distribution.base import (CategoricalDistribution,
+                                         CoreDistribution)
 
 
-class MultinoulliDistribution(CategoricalDistribution):
+class MultinoulliDistribution(CoreDistribution, CategoricalDistribution):
     """Categorical distribution that stores category labels and probabilities.
 
     Parameters
     ----------
     labels: list of str
         List containing the label belonging to each category.
     probs: list of int
         List containing the probability of each category.
         Probabilities will be normalized, so frequencies are valid too.
     """
 
-    aliases = ["MultinoulliDistribution", "categorical"]
+    implements = "core.multinoulli"
 
     def __init__(self, labels: npt.NDArray[np.str_],
                  probs: npt.NDArray[np.float_]):
         self.labels = labels
         self.probs = probs
         if np.sum(self.probs) != 1:
             self.probs = self.probs/np.sum(self.probs)
 
     @classmethod
     def _fit(cls, values: pl.Series):
         labels, counts = np.unique(values, return_counts=True)
         probs = counts/np.sum(counts)
         return cls(labels.astype(str), probs)
 
-    @property
-    def par_dict(self):
-        """Get labels and probabilities as a dictionary."""
-        return dict(zip(self.labels, self.probs))
-
-    def to_dict(self):
-        dist_dict = {}
-        dist_dict["name"] = type(self).__name__
-        dist_dict["parameters"] = {"labels": self.labels,
-                                   "probs": self.probs}
-        return dist_dict
+    def _param_dict(self):
+        return {"labels": self.labels, "probs": self.probs}
+
+    @classmethod
+    def _param_schema(cls):
+        return {
+            "labels": {"type": "array", "items": {"type": "string"}, "uniqueItems": True},
+            "probs": {"type": "array", "items": {"type": "number"}},
+        }
 
     def __str__(self):
         return str(self.to_dict())
 
     def draw(self):
         return str(np.random.choice(self.labels, p=self.probs))
 
     def information_criterion(self,
                               values: Union[pd.Series, pl.Series, npt.NDArray[np.str_]]
                               ) -> float:
         values_array = np.array(values, dtype=str)
         labels, counts = np.unique(values_array, return_counts=True)
         log_lik = 0.0
-        pdict = self.par_dict
+        pdict = dict(zip(self.labels, self.probs))
         for lab, count in zip(labels, counts):
             # account for missing values / missing categories
             # by setting default of .get to 1 (add log(1)=0 to log_lik)
             log_lik += count * np.log(pdict.get(lab, 1))
         return 2*(len(self.probs) - 1) - 2 * log_lik
 
     @classmethod
```

### Comparing `metasynth-0.2.2/metasynth/distribution/continuous.py` & `metasynth-0.3.0/metasynth/distribution/continuous.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 """Implemented floating point distributions."""
 
 import numpy as np
 from scipy.optimize import minimize
-from scipy.stats import uniform, norm, lognorm, truncnorm, expon
+from scipy.stats import expon, lognorm, norm, truncnorm, uniform
 from scipy.stats._continuous_distns import FitDataError
 
-from metasynth.distribution.base import ScipyDistribution, ContinuousDistribution
+from metasynth.distribution.base import (ContinuousDistribution,
+                                         CoreDistribution, ScipyDistribution)
 
 
-class UniformDistribution(ScipyDistribution, ContinuousDistribution):
+class UniformDistribution(CoreDistribution, ScipyDistribution, ContinuousDistribution):
     """Uniform distribution for floating point type.
 
     This class implements the uniform distribution between a minimum
     and maximum.
 
     Parameters
     ----------
     min_val: float
         Lower bound for uniform distribution.
     max_val: float
         Upper bound for uniform distribution.
     """
 
-    aliases = ["UniformDistribution", "uniform"]
+    implements = "core.uniform"
     dist_class = uniform
 
     def __init__(self, min_val: float, max_val: float):
         self.par = {"min_val": min_val, "max_val": max_val}
         self.dist = uniform(loc=self.min_val, scale=max(self.max_val-self.min_val, 1e-8))
 
     @classmethod
@@ -40,56 +41,70 @@
             return 2*self.n_par - 100*len(values)
         return 2*self.n_par - 2*len(values)*np.log((self.max_val-self.min_val)**-1)
 
     @classmethod
     def default_distribution(cls):
         return cls(0, 1)
 
+    @classmethod
+    def _param_schema(cls):
+        return {
+            "min_val": {"type": "number"},
+            "max_val": {"type": "number"},
+        }
+
 
-class NormalDistribution(ScipyDistribution, ContinuousDistribution):
+class NormalDistribution(CoreDistribution, ScipyDistribution, ContinuousDistribution):
     """Normal distribution for floating point type.
 
     This class implements the normal/gaussian distribution and takes
     the average and standard deviation as initialization input.
 
     Parameters
     ----------
     mean: float
         Mean of the normal distribution.
 
     std_dev: float
         Standard deviation of the normal distribution.
     """
 
-    aliases = ["NormalDistribution", "normal", "gaussian"]
+    implements = "core.normal"
     dist_class = norm
 
     def __init__(self, mean: float, std_dev: float):
         self.par = {"mean": mean, "std_dev": std_dev}
         self.dist = norm(loc=mean, scale=max(std_dev, 1e-8))
 
     @classmethod
     def default_distribution(cls):
         return cls(0, 1)
 
+    @classmethod
+    def _param_schema(cls):
+        return {
+            "mean": {"type": "number"},
+            "std_dev": {"type": "number"},
+        }
 
-class LogNormalDistribution(ScipyDistribution, ContinuousDistribution):
+
+class LogNormalDistribution(CoreDistribution, ScipyDistribution, ContinuousDistribution):
     """Log-normal distribution for floating point type.
 
     This class implements the log-normal mu and sigma as initialization input.
 
     Parameters
     ----------
     sigma: float
         Controls the width of the distribution.
     mu: float
         Controls the mean of the distribution.
     """
 
-    aliases = ["LogNormalDistribution", "lognormal"]
+    implements = "core.lognormal"
     dist_class = lognorm
 
     def __init__(self, mu: float, sigma: float):  # pylint: disable=invalid-name
         self.par = {"mu": mu, "sigma": sigma}
         self.dist = lognorm(s=max(sigma, 1e-8), scale=np.exp(mu))
 
     @classmethod
@@ -100,32 +115,38 @@
             return cls(0, 1)
         return cls(np.log(scale), sigma)
 
     @classmethod
     def default_distribution(cls):
         return cls(0, 1)
 
+    @classmethod
+    def _param_schema(cls):
+        return {
+            "mu": {"type": "number"},
+            "sigma": {"type": "number"},
+        }
+
 
-class TruncatedNormalDistribution(ScipyDistribution, ContinuousDistribution):
+class TruncatedNormalDistribution(CoreDistribution, ScipyDistribution, ContinuousDistribution):
     """Truncated normal distribution for floating point type.
 
     Parameters
     ----------
     lower_bound: float
         Lower bound of the truncated normal distribution.
     upper_bound: float
         Upper bound of the truncated normal distribution.
     mu: float
         Mean of the non-truncated normal distribution.
     sigma: float
         Standard deviation of the non-truncated normal distribution.
     """
 
-    aliases = ["TruncatedNormalDistribution", "truncnormal", "boundednormal",
-               "truncatednormal"]
+    implements = "core.truncated_normal"
     dist_class = truncnorm
 
     def __init__(self, lower_bound: float, upper_bound: float,
                  mu: float, sigma: float):
         self.par = {"lower_bound": lower_bound, "upper_bound": upper_bound,
                     "mu": mu, "sigma": sigma}
         a, b = (lower_bound-mu)/sigma, (upper_bound-mu)/sigma
@@ -151,28 +172,37 @@
                                      ((upper_bound-lower_bound)/100, None)]).x
         return cls(lower_bound, upper_bound, mu, sigma)
 
     @classmethod
     def default_distribution(cls):
         return cls(-1, 2, 0, 1)
 
+    @classmethod
+    def _param_schema(cls):
+        return {
+            "lower_bound": {"type": "number"},
+            "upper_bound": {"type": "number"},
+            "mu": {"type": "number"},
+            "sigma": {"type": "number"},
+        }
+
 
-class ExponentialDistribution(ScipyDistribution, ContinuousDistribution):
+class ExponentialDistribution(CoreDistribution, ScipyDistribution, ContinuousDistribution):
     """Exponential distribution for floating point type.
 
     This class implements the exponential distribution with the rate as its
     single parameter.
 
     Parameters
     ----------
     rate: float
         Rate of the exponential distribution. This is equal to 1/mean of the distribution.
     """
 
-    aliases = ["ExponentialDistribution", "exponential"]
+    implements = "core.exponential"
     dist_class = expon
 
     def __init__(self, rate: float):
         self.par = {"rate": rate}
         self.dist = expon(loc=0, scale=1/max(rate, 1e-8))
 
     @classmethod
@@ -181,7 +211,13 @@
         if len(values) == 0:
             return cls.default_distribution()
         return cls(rate=1/expon.fit(values, floc=0)[1])
 
     @classmethod
     def default_distribution(cls):
         return cls(1.0)
+
+    @classmethod
+    def _param_schema(cls):
+        return {
+            "rate": {"type": "number"}
+        }
```

### Comparing `metasynth-0.2.2/metasynth/distribution/datetime.py` & `metasynth-0.3.0/metasynth/distribution/datetime.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Distributions for date and time types."""
 
+import datetime as dt
 from abc import abstractmethod
 from random import random
-import datetime as dt
-from typing import Dict, Any
+from typing import Any, Dict
 
 import numpy as np
 
-from metasynth.distribution.base import DateTimeDistribution, TimeDistribution
-from metasynth.distribution.base import ScipyDistribution, DateDistribution
+from metasynth.distribution.base import (CoreDistribution, DateDistribution,
+                                         DateTimeDistribution,
+                                         ScipyDistribution, TimeDistribution)
 
 
 def convert_numpy_datetime(time_obj: np.datetime64) -> dt.datetime:
     """Convert numpy datetime to python stdlib datetime.
 
     Parameters
     ----------
@@ -89,89 +90,109 @@
         return time_obj
 
     def draw(self) -> dt.datetime:
         delta = self.end-self.start + self.minimum_delta
         new_time = random()*delta + self.start
         return self.round(new_time)
 
-    def to_dict(self) -> Dict:
-        return {
-            "name": self.name,
-            "parameters": {
-                "start": self.start.isoformat(),
-                "end": self.end.isoformat(),
-                "precision": self.precision,
-            }
-        }
-
     @abstractmethod
     def fromisoformat(self, dt_obj: str):
         """Convert string to iso format."""
 
     @property
     def minimum_delta(self) -> dt.timedelta:
         """Get the minimum time delta."""
         return dt.timedelta(**{self.precision: 1})
 
     def information_criterion(self, values):
         return 0.0
 
+    def _param_dict(self):
+        return {
+            "start": self.start.isoformat(),
+            "end": self.end.isoformat(),
+            "precision": self.precision,
+        }
+
 
-class UniformDateTimeDistribution(DateTimeDistribution, BaseUniformDistribution):
+class UniformDateTimeDistribution(CoreDistribution, DateTimeDistribution, BaseUniformDistribution):
     """Uniform DateTime distribution."""
 
-    aliases = ["UniformDateTimeDistribution", "datetime_uniform"]
+    implements = "core.uniform_datetime"
 
     def fromisoformat(self, dt_obj: str) -> dt.datetime:
         return dt.datetime.fromisoformat(dt_obj)
 
     @classmethod
     def default_distribution(cls):
         return cls("2022-07-15T10:39:36", "2022-08-15T10:39:36", precision="seconds")
 
+    @classmethod
+    def _param_schema(cls):
+        return {
+            "start": {"type": "string"},
+            "end": {"type": "string"},
+            "precision": {"type": "string"},
+        }
+
 
-class UniformTimeDistribution(TimeDistribution, BaseUniformDistribution):
+class UniformTimeDistribution(CoreDistribution, TimeDistribution, BaseUniformDistribution):
     """Uniform time distribution."""
 
-    aliases = ["UniformTimeDistribution", "time_uniform"]
+    implements = "core.uniform_time"
 
     def fromisoformat(self, dt_obj: str) -> dt.time:
         return dt.time.fromisoformat(dt_obj)
 
     @classmethod
     def default_distribution(cls):
         return cls("10:39:36", "18:39:36", precision="seconds")
 
     def draw(self):
         dt_begin = dt.datetime.combine(dt.datetime.today(), self.start)
         dt_end = dt.datetime.combine(dt.datetime.today(), self.end)
         delta = dt_end-dt_begin + self.minimum_delta
         return self.round((random()*delta + dt_begin).time())
 
+    @classmethod
+    def _param_schema(cls):
+        return {
+            "start": {"type": "string"},
+            "end": {"type": "string"},
+            "precision": {"type": "string"},
+        }
+
 
-class UniformDateDistribution(DateDistribution, BaseUniformDistribution):
+class UniformDateDistribution(CoreDistribution, DateDistribution, BaseUniformDistribution):
     """Uniform date distribution."""
 
-    aliases = ["UniformDateDistribution", "date_uniform"]
+    implements = "core.uniform_date"
     precision_possibilities = ["days"]
 
     def __init__(self, start: Any, end: Any):
         super().__init__(start, end, precision="days")
 
     def fromisoformat(self, dt_obj: str) -> dt.date:
         return dt.date.fromisoformat(dt_obj)
 
     def round(self, time_obj):
         return time_obj
 
-    def to_dict(self) -> Dict:
-        date_dict = BaseUniformDistribution.to_dict(self)
-        date_dict["parameters"].pop("precision")
+    def _param_dict(self) -> Dict:
+        date_dict = BaseUniformDistribution._param_dict(self)
+        del date_dict["precision"]
         return date_dict
 
     @classmethod
     def default_distribution(cls):
         return cls("1903-07-15", "1940-07-16")
 
     @classmethod
     def _fit(cls, values):
         return cls(values.min(), values.max())
+
+    @classmethod
+    def _param_schema(cls):
+        return {
+            "start": {"type": "string"},
+            "end": {"type": "string"},
+        }
```

### Comparing `metasynth-0.2.2/metasynth/distribution/discrete.py` & `metasynth-0.3.0/metasynth/distribution/discrete.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 """Module with discrete distributions."""
 
 from typing import Set
 
 import numpy as np
-from scipy.stats import randint, poisson
+from scipy.stats import poisson, randint
 
-from metasynth.distribution.base import ScipyDistribution, DiscreteDistribution
+from metasynth.distribution.base import (CoreDistribution,
+                                         DiscreteDistribution,
+                                         ScipyDistribution)
 
 
-class DiscreteUniformDistribution(ScipyDistribution, DiscreteDistribution):
+class DiscreteUniformDistribution(CoreDistribution, ScipyDistribution, DiscreteDistribution):
     """Integer uniform distribution.
 
     It differs from the floating point uniform distribution by
     being a discrete distribution instead.
 
     Parameters
     ----------
     low: int
         Lower bound (inclusive) of the uniform distribution.
     high: int
         Upper bound (exclusive) of the uniform distribution.
     """
 
-    aliases = ["DiscreteUniformDistribution", "discrete_uniform"]
-
+    implements = "core.discrete_uniform"
     dist_class = randint
 
     def __init__(self, low: int, high: int):
         self.par = {"low": low, "high": high}
         self.dist = self.dist_class(low=low, high=high)
 
     def _information_criterion(self, values):
@@ -38,19 +39,26 @@
         param = {"low": values.min(), "high": values.max()+1}
         return cls(**param)
 
     @classmethod
     def default_distribution(cls):
         return cls(0, 10)
 
+    @classmethod
+    def _param_schema(cls):
+        return {
+            "low": {"type": "integer"},
+            "high": {"type": "integer"},
+        }
+
 
-class PoissonDistribution(ScipyDistribution, DiscreteDistribution):
+class PoissonDistribution(CoreDistribution, ScipyDistribution, DiscreteDistribution):
     """Poisson distribution."""
 
-    aliases = ["PoissonDistribution", "poisson"]
+    implements = "core.poisson"
     dist_class = poisson
 
     def __init__(self, mu: float):
         self.par = {"mu": mu}
         self.dist = self.dist_class(mu=mu)
 
     def _information_criterion(self, values):
@@ -60,29 +68,35 @@
     def _fit(cls, values):
         return cls(values.mean())
 
     @classmethod
     def default_distribution(cls):
         return cls(0.5)
 
+    @classmethod
+    def _param_schema(cls):
+        return {
+            "mu": {"type": "number"},
+        }
 
-class UniqueKeyDistribution(ScipyDistribution, DiscreteDistribution):
+
+class UniqueKeyDistribution(CoreDistribution, ScipyDistribution, DiscreteDistribution):
     """Integer distribution with unique keys.
 
     Discrete distribution that ensures the uniqueness of the drawn values.
 
     Parameters
     ----------
     low: int
         Minimum value for the keys.
     consecutive: int
         1 if keys are consecutive and increasing, 0 otherwise.
     """
 
-    aliases = ["UniqueKeyDistribution", "unique_key"]
+    implements = "core.unique_key"
     is_unique = True
 
     def __init__(self, low: int, consecutive: int):
         self.par = {"low": low, "consecutive": consecutive}
         self.last_key = low - 1
         self.key_set: Set[int] = set()
 
@@ -130,7 +144,14 @@
 
         # Probabilities go up like 1/n, 1/(n-1), 1/(n-2), ..., 1/2, 1
         return 5 - 2*np.sum(np.log(1/np.arange(n_choice, n_choice-len(values), -1)))
 
     @classmethod
     def default_distribution(cls):
         return cls(0, 0)
+
+    @classmethod
+    def _param_schema(cls):
+        return {
+            "low": {"type": "integer"},
+            "high": {"type": "integer"},
+        }
```

### Comparing `metasynth-0.2.2/metasynth/distribution/faker.py` & `metasynth-0.3.0/metasynth/distribution/faker.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Module containing an interface to the faker package."""
 from typing import Iterable
 
 from faker import Faker
 
-from metasynth.distribution.base import StringDistribution
+from metasynth.distribution.base import CoreDistribution, StringDistribution
 
 
-class FakerDistribution(StringDistribution):
+class FakerDistribution(CoreDistribution, StringDistribution):
     """Distribution for the faker package.
 
     This is mainly an interface for the faker package, so that it
     can be used within the MetaSynth package. It doesn't have any
     true fitting/statistical inference method, so it has to be manually
     selected.
 
@@ -18,15 +18,15 @@
     ----------
     faker_type: str
         The provider function in the faker package, e.g. 'city' or 'ipv4', etc.
     locale: str
         Locale used for the faker package.
     """
 
-    aliases = ["FakerDistribution", "faker"]
+    implements = "core.faker"
 
     def __init__(self, faker_type: str, locale: str = "en_US"):
         self.faker_type: str = faker_type
         self.locale: str = locale
         self.fake: Faker = Faker(locale=locale)
 
     @classmethod
@@ -34,41 +34,29 @@
             # pylint: disable=arguments-differ
         """Select the appropriate faker function and locale."""
         return cls(faker_type, locale)
 
     def __str__(self):
         return f"faker.{self.faker_type}.{self.locale}"
 
-    def to_dict(self):
-        return {
-            "name": self.name,
-            "parameters": {
-                "faker_type": self.faker_type,
-                "locale": self.locale
-            }
-        }
-
     def draw(self):
         return getattr(self.fake, self.faker_type)()
 
-    @classmethod
-    def is_named(cls, name):
-        if name == cls.__name__:
-            return True
-        return name.startswith("faker") and len(name.split(".")) >= 2
-
-    @classmethod
-    def fit_kwargs(cls, name):
-        if name == cls.__name__:
-            return {}
-        split_name = name.split(".")
-        if len(split_name) == 2:
-            return {"faker_type": split_name[1]}
-        return {"faker_type": split_name[1],
-                "locale": split_name[2]}
-
     def information_criterion(self, values: Iterable) -> float:
         return 99999
 
     @classmethod
     def default_distribution(cls):
         return cls("city")
+
+    def _param_dict(self):
+        return {
+            "faker_type": self.faker_type,
+            "locale": self.locale
+        }
+
+    @classmethod
+    def _param_schema(cls):
+        return {
+            "faker_type": {"type": "string"},
+            "locale": {"type": "string"},
+        }
```

### Comparing `metasynth-0.2.2/metasynth/distribution/regex/base.py` & `metasynth-0.3.0/metasynth/distribution/regex/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """Module containing string distributions."""
 
 from __future__ import annotations
 
-from typing import List, Union, Tuple, Type, Sequence, Set
+from typing import List, Sequence, Set, Tuple, Type, Union
 
 import numpy as np
 
-from metasynth.distribution.base import StringDistribution
-from metasynth.distribution.regex.element import BaseRegexElement
-from metasynth.distribution.regex.element import DigitRegex, AlphaNumericRegex
-from metasynth.distribution.regex.element import LettersRegex, SingleRegex, AnyRegex
-from metasynth.distribution.regex.element import UppercaseRegex, LowercaseRegex
+from metasynth.distribution.base import CoreDistribution, StringDistribution
+from metasynth.distribution.regex.element import (AlphaNumericRegex, AnyRegex,
+                                                  BaseRegexElement, DigitRegex,
+                                                  LettersRegex, LowercaseRegex,
+                                                  SingleRegex, UppercaseRegex)
 from metasynth.distribution.regex.optimizer import RegexOptimizer
 
 
 def _get_gradient_start(values: Sequence[str], new_values: Sequence[str],
                         regex_elem: BaseRegexElement) -> float:
     """Get the proportion of the characters that were resolved with the regex."""
     digits_used: List[int] = []
@@ -33,29 +33,29 @@
     new_energy = RegexOptimizer.energy_from_values(new_values)
     energy_budget = regex_elem.information_budget(regex_stat)
 
     delta_energy = old_energy - new_energy
     return delta_energy/energy_budget
 
 
-class RegexDistribution(StringDistribution):
+class RegexDistribution(CoreDistribution, StringDistribution):
     """Distribution that uses a strategy similar to regex.
 
     The idea behind this method is that for structured strings
     regexes works very well. It uses a greedy algorithm to build the
     regex. It does not implement all regexes, nor does it claim to be
     compliant with standard ones.
 
     Parameters
     ----------
     re_list: list of BaseRegexElement
         List of basic regex elements in the order that they occur.
     """
 
-    aliases = ["RegexDistribution", "regex"]
+    implements = "core.regex"
 
     def __init__(self, re_list: Union[Sequence[Union[BaseRegexElement, Tuple[str, float]]], str]):
         self.re_list = []
         if isinstance(re_list, str):
             self.re_list = self._unpack_regex(re_list)
             return
 
@@ -155,41 +155,52 @@
         for rex in self.re_list:
             cur_str += rex.draw()
         return cur_str
 
     def __str__(self):
         return "".join([str(x) for x in self.re_list])
 
-    def to_dict(self):
+    def _param_dict(self):
         return {
-            "name": self.name,
-            "parameters": {
-                    "re_list": [(str(x), x.frac_used) for x in self.re_list],
+            "re_list": [(str(x), x.frac_used) for x in self.re_list],
+        }
+
+    @classmethod
+    def _param_schema(cls):
+        return {
+            "re_list": {
+                "type": "array",
+                "items": {
+                    "type": "array",
+                    "prefixItems": [{"type": "string"}, {"type": "number"}],
+                    "minItems": 2,
+                    "additionalItems": False
                 }
+            }
         }
 
     @classmethod
     def default_distribution(cls):
         return cls([(r"\d{3,4}", 0.67)])
 
 
-class UniqueRegexDistribution(RegexDistribution):
+class UniqueRegexDistribution(RegexDistribution, CoreDistribution):
     """Unique variant of the regex distribution.
 
     Same as the normal regex distribution, but checks whether a key
     has already been used.
 
     Parameters
     ----------
     re_list: list of BaseRegexElement
         List of basic regex elements in the order that they occur.
     """
 
+    implements = "core.unique_regex"
     is_unique = True
-    aliases = ["UniqueRegexDistribution", "regex_unique"]
 
     def __init__(self, re_list: Sequence[Union[BaseRegexElement, Tuple[str, float]]]):
         super().__init__(re_list)
         self.key_set: Set[str] = set()
 
     def draw_reset(self):
         self.key_set = set()
```

### Comparing `metasynth-0.2.2/metasynth/distribution/regex/element.py` & `metasynth-0.3.0/metasynth/distribution/regex/element.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Module containing string distributions."""
 
 from __future__ import annotations
 
-from abc import abstractmethod, ABC
-import re
 import random
+import re
 import string
-from typing import Iterable, Tuple, Sequence, Dict, Optional
+from abc import ABC, abstractmethod
+from typing import Dict, Iterable, Optional, Sequence, Tuple
 
 import numpy as np
 from sklearn.feature_extraction.text import CountVectorizer
 
 from metasynth.distribution.regex.optimizer import RegexOptimizer
```

### Comparing `metasynth-0.2.2/metasynth/distribution/regex/optimizer.py` & `metasynth-0.3.0/metasynth/distribution/regex/optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Module containing the optimizer class for the regex distribution."""
 
-from typing import Sequence, Tuple, List, Dict, Any
+from typing import Any, Dict, List, Sequence, Tuple
+
 import numpy as np
 import numpy.typing as npt
 
 # Used for side assignment of values with no regex match
 SIDE_LEFT = -1
 SIDE_RIGHT = -2
 
@@ -121,15 +122,16 @@
     @property
     def energy(self) -> float:
         """Compute the energy of the current assignment/solution."""
         left_energy = np.sum(np.log(self.left_cum_dist+1))
         right_energy = np.sum(np.log(self.right_cum_dist+1))
         return left_energy + right_energy
 
-    def energy_move(self, dist: npt.NDArray[np.int_], len_src: int, len_dst: int) -> float:
+    @staticmethod
+    def energy_move(dist: npt.NDArray[np.int_], len_src: int, len_dst: int) -> float:
         """Compute the energy to change the length on one side.
 
         Parameters
         ----------
         dist:
             Cumulative distribution of the current lengths.
             (self.left_cum_dist or self.right_cum_dist)
```

### Comparing `metasynth-0.2.2/metasynth/disttree.py` & `metasynth-0.3.0/metasynth/provider.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,133 +1,201 @@
-"""Module for distribution trees.
+"""Module for distribution providers.
 
-These are used to find/fit distributions that are available. See setup.py on how the
-builtin distribution tree is registered.
+These are used to find/fit distributions that are available. See pyproject.toml on how the
+builtin distribution provider is registered.
 """
 
 from __future__ import annotations
 
-from abc import abstractmethod
-from typing import List, Union
-from typing import Type, Any, Optional
-import warnings
 import inspect
+import warnings
+from abc import ABC
+from typing import Any, List, Optional, Type, Union
+
 try:
-    from importlib_metadata import entry_points
+    from importlib_metadata import entry_points, EntryPoint
 except ImportError:
-    from importlib.metadata import entry_points  # type: ignore
+    from importlib.metadata import entry_points, EntryPoint  # type: ignore
 
-import polars as pl
 import numpy as np
+import polars as pl
 
 from metasynth.distribution.base import BaseDistribution
-from metasynth.distribution.discrete import DiscreteUniformDistribution,\
-    PoissonDistribution, UniqueKeyDistribution
-from metasynth.distribution.continuous import UniformDistribution,\
-    NormalDistribution, LogNormalDistribution, TruncatedNormalDistribution,\
-    ExponentialDistribution
 from metasynth.distribution.categorical import MultinoulliDistribution
-from metasynth.distribution.regex.base import RegexDistribution,\
-    UniqueRegexDistribution
+from metasynth.distribution.continuous import (ExponentialDistribution,
+                                               LogNormalDistribution,
+                                               NormalDistribution,
+                                               TruncatedNormalDistribution,
+                                               UniformDistribution)
+from metasynth.distribution.datetime import (UniformDateDistribution,
+                                             UniformDateTimeDistribution,
+                                             UniformTimeDistribution)
+from metasynth.distribution.discrete import (DiscreteUniformDistribution,
+                                             PoissonDistribution,
+                                             UniqueKeyDistribution)
 from metasynth.distribution.faker import FakerDistribution
-from metasynth.distribution.datetime import UniformDateDistribution,\
-    UniformTimeDistribution, UniformDateTimeDistribution
+from metasynth.distribution.regex.base import (RegexDistribution,
+                                               UniqueRegexDistribution)
+from metasynth.privacy import BasePrivacy, BasicPrivacy
 
 
-class BaseDistributionTree():
+class BaseDistributionProvider(ABC):
     """Class that encapsulates a set of distributions.
 
     It has a property {var_type}_distributions for every var_type.
     """
 
-    def __init__(self, **kwargs):
-        # Perform internal consistency check.
-        for var_type in self.all_var_types:
-            for dist in self.get_dist_list(var_type):
-                assert dist.var_type == var_type, (f"Error: Distribution tree is inconsistent for "
-                                                   f"{dist}.")
-        self.privacy_kwargs = kwargs
-
-    @property
-    @abstractmethod
-    def discrete_distributions(self) -> List[Type[BaseDistribution]]:
-        """Get the integer distributions."""
-
-    @property
-    @abstractmethod
-    def continuous_distributions(self) -> List[Type[BaseDistribution]]:
-        """Get continuous distributions."""
-
-    @property
-    @abstractmethod
-    def categorical_distributions(self) -> List[Type[BaseDistribution]]:
-        """Get categorical distributions."""
-
-    @property
-    @abstractmethod
-    def string_distributions(self) -> List[Type[BaseDistribution]]:
-        """Get categorical distributions."""
-
-    @property
-    @abstractmethod
-    def date_distributions(self) -> List[Type[BaseDistribution]]:
-        """Get categorical distributions."""
+    name = ""
+    version = ""
+    distributions: list[type[BaseDistribution]] = []
 
-    @property
-    @abstractmethod
-    def time_distributions(self) -> List[Type[BaseDistribution]]:
-        """Get categorical distributions."""
-
-    @property
-    @abstractmethod
-    def datetime_distributions(self) -> List[Type[BaseDistribution]]:
-        """Get categorical distributions."""
+    def __init__(self):
+        # Perform internal consistency check.
+        assert len(self.name) > 0
+        assert len(self.version) > 0
+        assert len(self.distributions) > 0
 
     def get_dist_list(self, var_type: str) -> List[Type[BaseDistribution]]:
         """Get all distributions for a certain variable type.
 
         Parameters
         ----------
         var_type:
             Variable type to get the distributions for.
 
         Returns
         -------
         list[Type[BaseDistribution]]:
             List of distributions with that variable type.
         """
-        prop_str = var_type + "_distributions"
-        if not hasattr(self, prop_str):
-            raise ValueError(f"Unknown variable type '{var_type}' detected.")
-        return getattr(self, prop_str)
+        return [dist_class for dist_class in self.distributions if dist_class.var_type == var_type]
+
+    @property
+    def all_var_types(self) -> List[str]:
+        """Return list of available variable types."""
+        var_type_set = set()
+        for dist in self.distributions:
+            var_type_set.add(dist.var_type)
+        return list(var_type_set)
 
-    def fit(self, series: pl.Series, var_type: str,
-            unique: Optional[bool] = False) -> BaseDistribution:
+
+class BuiltinDistributionProvider(BaseDistributionProvider):
+    """Distribution tree that includes the builtin distributions."""
+
+    name = "builtin"
+    version = "1.0"
+    distributions = [
+        DiscreteUniformDistribution, PoissonDistribution, UniqueKeyDistribution,
+        UniformDistribution, NormalDistribution, LogNormalDistribution,
+        TruncatedNormalDistribution, ExponentialDistribution,
+        MultinoulliDistribution,
+        RegexDistribution, UniqueRegexDistribution, FakerDistribution,
+        UniformDateDistribution,
+        UniformTimeDistribution,
+        UniformDateTimeDistribution,
+    ]
+
+
+class DistributionProviderList():
+    """List of DistributionProviders with functionality to fit distributions.
+
+    Arguments
+    ---------
+    dist_providers:
+        One or more distribution providers, that are denoted either with a string ("builtin")
+        , DistributionProvider (BuiltinDistributionProvider()) or DistributionProvider type
+        (BuiltinDistributionProvider).
+        The order in which distribution providers are included matters. If a provider implements
+        the same distribution at the same privacy level, then only the first will be taken into
+        account.
+    """
+
+    def __init__(
+            self,
+            dist_providers: Union[
+                None, str, type[BaseDistributionProvider], BaseDistributionProvider,
+                list[Union[str, type[BaseDistributionProvider], BaseDistributionProvider]]]):
+        if dist_providers is None:
+            self.dist_packages = _get_all_provider_list()
+            return
+
+        if isinstance(dist_providers, (str, type, BaseDistributionProvider)):
+            dist_providers = [dist_providers]
+        self.dist_packages = []
+        for provider in dist_providers:
+            if isinstance(provider, str):
+                self.dist_packages.append(get_distribution_provider(provider))
+            elif isinstance(provider, type):
+                self.dist_packages.append(provider())
+            elif isinstance(provider, BaseDistributionProvider):
+                self.dist_packages.append(provider)
+            else:
+                raise ValueError(f"Unknown distribution package type '{type(provider)}'")
+
+    def fit(self, series: pl.Series,
+            var_type: str,
+            dist: Optional[Union[str, BaseDistribution, type]] = None,
+            privacy: BasePrivacy = BasicPrivacy(),
+            unique: Optional[bool] = None,
+            fit_kwargs: Optional[dict] = None):
+        """Fit a distribution to a column/series.
+
+        Parameters
+        ----------
+        series:
+            The data to fit the distributions to.
+        var_type:
+            The variable type of the data.
+        dist:
+            Distribution to fit. If not supplied or None, the AIC information
+            criterion will be used to determine which distribution is the most
+            suitable.
+        privacy:
+            Level of privacy that will be used in the fit.
+        unique:
+            Whether the distribution should be unique or not.
+        fit_kwargs:
+            Extra options for distributions during the fitting stage.
+        """
+        if fit_kwargs is None:
+            fit_kwargs = {}
+        if dist is not None:
+            return self._fit_distribution(series, dist, privacy, **fit_kwargs)
+        if len(fit_kwargs) > 0:
+            raise ValueError(f"Got fit arguments for variable '{series.name}', but no "
+                             "distribution. Set the distribution manually to fix.")
+        return self._find_best_fit(series, var_type, unique, privacy)
+
+    def _find_best_fit(self, series: pl.Series, var_type: str,
+                       unique: Optional[bool],
+                       privacy: BasePrivacy) -> BaseDistribution:
         """Fit a distribution to a series.
 
-        Search for the distirbution within all available distributions in the tree.
+        Search for the distribution within all available distributions in the tree.
 
         Parameters
         ----------
         series:
             Series to fit a distribution to.
         var_type:
             Variable type of the series.
         unique:
             Whether the variable should be unique or not.
+        privacy:
+            Privacy level to find the best fit with.
 
         Returns
         -------
         BaseDistribution:
             Distribution fitted to the series.
         """
-        dist_list = self.get_dist_list(var_type)
+        dist_list = self._get_dist_list(privacy, var_type)
         if len(dist_list) == 0:
             raise ValueError(f"No available distributions with variable type: '{var_type}'")
-        dist_instances = [d.fit(series, **self.privacy_kwargs) for d in dist_list]
+        dist_instances = [d.fit(series, **privacy.fit_kwargs) for d in dist_list]
         dist_aic = [d.information_criterion(series) for d in dist_instances]
         i_best_dist = np.argmin(dist_aic)
         warnings.simplefilter("always")
         if dist_instances[i_best_dist].is_unique and unique is None:
             warnings.warn(f"\nVariable {series.name} seems unique, but not set to be unique.\n"
                           "Set the variable to be either unique or not unique to remove this "
                           "warning.\n")
@@ -139,155 +207,144 @@
         dist_instances = [d for d in dist_instances if d.is_unique == unique]
         if len(dist_instances) == 0:
             raise ValueError(f"No available distributions for variable '{series.name}'"
                              f" with variable type '{var_type}' "
                              f"that have unique == {unique}.")
         return dist_instances[np.argmin(dist_aic)]
 
-    @property
-    def all_var_types(self) -> List[str]:
-        """Return list of available variable types."""
-        return [p[:-14] for p in dir(self.__class__)
-                if isinstance(getattr(self.__class__, p), property) and p.endswith("_distributions")
-                ]
-
-    def find_distribution(self, dist_name: str) -> tuple[Type[BaseDistribution], dict[str, Any]]:
+    def find_distribution(self, dist_name: str, privacy: BasePrivacy = BasicPrivacy(),
+                          ) -> type[BaseDistribution]:
         """Find a distribution and fit keyword arguments from a name.
 
-        This allows us to use 'faker.city' to generate a faker instance that generates cities.
-
         Parameters
         ----------
         dist_name:
-            Name of the distribution, such as faker.city, DiscreteUniformDistribution or normal.
+            Name of the distribution, e.g., for the built-in
+            uniform distribution: "uniform", "core.uniform", "UniformDistribution".
+        privacy:
+            Type of privacy to be applied.
 
         Returns
         -------
         tuple[Type[BaseDistribution], dict[str, Any]]:
             A distribution and the arguments to create an instance.
         """
-        for var_type in self.all_var_types:
-            for dist_class in self.get_dist_list(var_type):
-                if dist_class.is_named(dist_name):
-                    return dist_class, dist_class.fit_kwargs(dist_name)
+        for dist_class in self._get_dist_list(privacy):
+            if dist_class.matches_name(dist_name) and dist_class.privacy == privacy.name:
+                return dist_class
         raise ValueError(f"Cannot find distribution with name '{dist_name}'.")
 
-    def fit_distribution(self, dist: Union[str, Type[BaseDistribution], BaseDistribution],
-                         series: pl.Series, **fit_kwargs) -> BaseDistribution:
+    def _fit_distribution(self, series: pl.Series,
+                          dist: Union[str, Type[BaseDistribution], BaseDistribution],
+                          privacy: BasePrivacy,
+                          **fit_kwargs) -> BaseDistribution:
         """Fit a specific distribution to a series.
 
         In contrast the fit method, this needs a supplied distribution(type).
 
         Parameters
         ----------
         dist:
             Distribution to fit (if it is not already fitted).
         series:
-            Series to fit the distribution to
+            Series to fit the distribution to.
+        privacy:
+            Privacy level to fit the distribution with.
         fit_kwargs:
-            Extra fitting parameters that are specific to the distribution.
+            Extra keyword arguments to modify the way the distribution is fit.
 
         Returns
         -------
         BaseDistribution:
             Fitted distribution.
         """
         dist_instance = None
-        fit_kwargs.update(self.privacy_kwargs)
 
         if isinstance(dist, str):
-            dist_class, new_fit_kwargs = self.find_distribution(dist)
-            fit_kwargs.update(new_fit_kwargs)
-            dist_instance = dist_class.fit(series, **fit_kwargs)
+            dist_class = self.find_distribution(dist, privacy=privacy)
+            dist_instance = dist_class.fit(series, **privacy.fit_kwargs, **fit_kwargs)
         elif inspect.isclass(dist) and issubclass(dist, BaseDistribution):
-            dist_instance = dist.fit(series, **fit_kwargs)
+            dist_instance = dist.fit(series, **privacy.fit_kwargs, **fit_kwargs)
         if isinstance(dist, BaseDistribution):
             dist_instance = dist
 
         if dist_instance is None:
             raise TypeError(
                 f"Distribution with type {type(dist)} is not a BaseDistribution")
 
         return dist_instance
 
+    def _get_dist_list(self, privacy: Optional[BasePrivacy] = None,
+                       var_type: Optional[str] = None) -> list[type[BaseDistribution]]:
+        dist_list = []
+        for dist_provider in self.dist_packages:
+            if var_type is None:
+                dist_list.extend(dist_provider.distributions)
+            else:
+                dist_list.extend(dist_provider.get_dist_list(var_type))
+
+        if privacy is None:
+            return dist_list
+        dist_list = [dist for dist in dist_list if dist.privacy == privacy.name]
+        return dist_list
+
     def from_dict(self, var_dict: dict[str, Any]) -> BaseDistribution:
         """Create a distribution from a dictionary.
 
         Parameters
         ----------
         var_dict:
             Variable dictionary that includes the distribution properties.
 
         Returns
         -------
         BaseDistribution:
             Distribution representing the dictionary.
         """
-        for dist_class in self.get_dist_list(var_dict["type"]):
-            if dist_class.is_named(var_dict["distribution"]["name"]):
+        for dist_class in self._get_dist_list(var_type=var_dict["type"]):
+            if dist_class.implements == var_dict["distribution"]["implements"]:
                 return dist_class.from_dict(var_dict["distribution"])
-        raise ValueError(f"Cannot find distribution with name '{var_dict['distribution']['name']}'"
+        raise ValueError(f"Cannot find distribution with name "
+                         f"'{var_dict['distribution']['implements']}'"
                          f"and type '{var_dict['type']}'.")
 
 
-class BuiltinDistributionTree(BaseDistributionTree):
-    """Distribution tree that includes the builtin distributions."""
-
-    @property
-    def discrete_distributions(self) -> List[type]:
-        return [DiscreteUniformDistribution, PoissonDistribution, UniqueKeyDistribution]
-
-    @property
-    def continuous_distributions(self) -> List[type]:
-        return [UniformDistribution, NormalDistribution, LogNormalDistribution,
-                TruncatedNormalDistribution, ExponentialDistribution]
-
-    @property
-    def categorical_distributions(self) -> List[type]:
-        return [MultinoulliDistribution]
-
-    @property
-    def string_distributions(self) -> List[type]:
-        return [RegexDistribution, UniqueRegexDistribution, FakerDistribution]
-
-    @property
-    def date_distributions(self) -> List[type]:
-        return [UniformDateDistribution]
+def _get_all_providers() -> dict[str, EntryPoint]:
+    """Get all available providers."""
+    return {
+        entry.name: entry
+        for entry in entry_points(group="metasynth.distribution_provider")
+    }
 
-    @property
-    def time_distributions(self) -> List[type]:
-        return [UniformTimeDistribution]
 
-    @property
-    def datetime_distributions(self) -> List[type]:
-        return [UniformDateTimeDistribution]
+def _get_all_provider_list() -> list[BaseDistributionProvider]:
+    return [p.load()() for p in _get_all_providers().values()]
 
 
-def get_disttree(target: Optional[Union[str, type, BaseDistributionTree]] = None, **kwargs
-                 ) -> BaseDistributionTree:
+def get_distribution_provider(
+        provider: Union[str, type[BaseDistributionProvider],
+                        BaseDistributionProvider] = "builtin"
+        ) -> BaseDistributionProvider:
     """Get a distribution tree.
 
     Parameters
     ----------
-    target:
-        Directive to get the distribution tree.
+    provider:
+        Name, class or class type of the provider to be used.
+    kwargs:
+        Extra keyword arguments for initialization of the distribution provider.
 
     Returns
     -------
-    BaseDistributionTree:
-        Distribution tree.
+    BaseDistributionProvider:
+        The distribution provider that was found.
     """
-    if target is None:
-        target = "builtin"
-    if isinstance(target, BaseDistributionTree):
-        return target
-    if isinstance(target, type):
-        return target()
+    if isinstance(provider, BaseDistributionProvider):
+        return provider
+    if isinstance(provider, type):
+        return provider()
 
-    all_disttrees = {
-        entry.name: entry
-        for entry in entry_points(group="metasynth.disttree")
-    }
+    all_providers = _get_all_providers()
     try:
-        return all_disttrees[target].load()(**kwargs)
+        return all_providers[provider].load()()
     except KeyError as exc:
-        raise ValueError(f"Cannot find distribution tree with name '{target}'.") from exc
+        raise ValueError(f"Cannot find distribution provider with name '{provider}'.") from exc
```

### Comparing `metasynth-0.2.2/metasynth/schema/generative_metadata_format.json` & `metasynth-0.3.0/metasynth/schema/generative_metadata_format.json`

 * *Files identical despite different names*

### Comparing `metasynth-0.2.2/metasynth/var.py` & `metasynth-0.3.0/metasynth/var.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,21 @@
 """Variable module that creates metadata variables."""  # pylint: disable=invalid-name
 
 from __future__ import annotations
 
-from typing import Union, Dict, Any, Optional
+from typing import Any, Dict, Optional, Union
 
-import polars as pl
-import pandas as pd
 import numpy as np
+import pandas as pd
+import polars as pl
 
 from metasynth.distribution.base import BaseDistribution
-from metasynth.disttree import BaseDistributionTree, get_disttree
-
-
-def _to_polars(series: Union[pd.Series, pl.Series]) -> pl.Series:
-    if isinstance(series, pl.Series):
-        return series
-    if len(series.dropna()) == 0:
-        series = pl.Series(name=series.name,
-                           values=[None for _ in range(len(series))])
-    else:
-        series = pl.Series(series)
-    return series
+from metasynth.privacy import BasePrivacy, BasicPrivacy
+from metasynth.provider import (BaseDistributionProvider,
+                                DistributionProviderList)
 
 
 class MetaVar():
     """Meta data variable.
 
     Acts as a base class for specific types of variables, but also as a
     launching pad for detecting its type.
@@ -161,18 +152,20 @@
             "description": self.description,
             "type": self.var_type,
             "dtype": self.dtype,
             "prop_missing": self.prop_missing,
             "distribution": str(self.distribution),
         })
 
-    def fit(self,
+    def fit(self,  # pylint: disable=too-many-arguments
             dist: Optional[Union[str, BaseDistribution, type]] = None,
-            distribution_tree: Union[str, type, BaseDistributionTree] = "builtin",
-            unique: Optional[bool] = None, **fit_kwargs):
+            dist_providers: Union[str, type, BaseDistributionProvider] = "builtin",
+            privacy: BasePrivacy = BasicPrivacy(),
+            unique: Optional[bool] = None,
+            fit_kwargs: Optional[dict] = None):
         """Fit distributions to the data.
 
         If multiple distributions are available for the current data type,
         use the one that fits the data the best.
 
         While it has no arguments or return values, it will set the
         distribution attribute to the most suitable distribution.
@@ -181,34 +174,31 @@
         ----------
         dist:
             The distribution to fit. In case of a string, search for it
             using the aliases of all distributions. Otherwise use the
             supplied distribution (class). Examples of allowed strings are:
             "normal", "uniform", "faker.city.nl_NL". If not supplied, fit
             the best available distribution for the variable type.
-        distribution_tree:
-            Distribution tree to be used.
-            By default use all distributions in metasynth.distribution.
+        dist_providers:
+            Distribution providers that are used for fitting.
+        privacy:
+            Privacy level to use for fitting the series.
         unique:
             Whether the variable should be unique. If not supplied, it will be
             inferred from the data.
+        fit_kwargs:
+            Extra options for distributions during the fitting stage.
         """
         if self.series is None:
             raise ValueError("Cannot fit distribution if we don't have the"
                              "original data.")
 
-        # Automatic detection of the distribution
-        disttree = get_disttree(distribution_tree)
-
-        # Manually supplied distribution
-        if dist is None:
-            self.distribution = disttree.fit(self.series, self.var_type, unique=unique,
-                                             **fit_kwargs)
-        else:
-            self.distribution = disttree.fit_distribution(dist, self.series, **fit_kwargs)
+        provider_list = DistributionProviderList(dist_providers)
+        self.distribution = provider_list.fit(self.series, self.var_type, dist, privacy, unique,
+                                              fit_kwargs)
 
     def draw(self) -> Any:
         """Draw a random item for the variable in whatever type is required."""
         if self.distribution is None:
             raise ValueError("Cannot draw without distribution")
 
         # Return NA's -> None
@@ -234,30 +224,48 @@
         self.distribution.draw_reset()
         value_list = [self.draw() for _ in range(n)]
         if "Categorical" in self.dtype:
             return pl.Series(value_list, dtype=pl.Categorical)
         return pl.Series(value_list)
 
     @classmethod
-    def from_dict(cls, var_dict: Dict[str, Any]) -> MetaVar:
+    def from_dict(cls,
+                  var_dict: Dict[str, Any],
+                  distribution_providers: Union[
+                      None, str, type[BaseDistributionProvider],
+                      BaseDistributionProvider] = None) -> MetaVar:
         """Restore variable from dictionary.
 
         Parameters
         ----------
+        distribution_providers:
+            Distribution providers to use to create the variable. If None,
+            use all installed/available distribution providers.
         var_dict:
             This dictionary contains all the variable and distribution
             information to recreate it from scratch.
 
         Returns
         -------
         MetaVar:
             Initialized metadata variable.
         """
-        disttree = get_disttree()
-        dist = disttree.from_dict(var_dict)
+        provider_list = DistributionProviderList(distribution_providers)
+        dist = provider_list.from_dict(var_dict)
         return cls(
             var_dict["type"],
             name=var_dict["name"],
             distribution=dist,
             prop_missing=var_dict["prop_missing"], dtype=var_dict["dtype"],
             description=var_dict.get("description", None)
-            )
+        )
+
+
+def _to_polars(series: Union[pd.Series, pl.Series]) -> pl.Series:
+    if isinstance(series, pl.Series):
+        return series
+    if len(series.dropna()) == 0:
+        series = pl.Series(name=series.name,
+                           values=[None for _ in range(len(series))])
+    else:
+        series = pl.Series(series)
+    return series
```

### Comparing `metasynth-0.2.2/metasynth.egg-info/PKG-INFO` & `metasynth-0.3.0/metasynth.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metasynth
-Version: 0.2.2
+Version: 0.3.0
 Summary: Package for creating synthetic datasets while preserving privacy.
 Author-email: Raoul Schram <r.d.schram@uu.nl>, Erik-Jan van Kesteren <e.vankesteren1@uu.nl>
 License: MIT License
         
         Copyright (c) 2022 SoDa
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -38,14 +38,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/metasynth)
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sodascience/metasynth/HEAD?labpath=examples%2Fadvanced_tutorial.ipynb)
+[![Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sodascience/metasynth/blob/main/examples/advanced_tutorial.ipynb)
 [![docs](https://readthedocs.org/projects/metasynth/badge/?version=latest)](https://metasynth.readthedocs.io/en/latest/index.html)
 
 # MetaSynth
 
 MetaSynth is a python package to generate synthetic data mostly geared towards code testing and reproducibility.
 Using the [ONS methodology](https://www.ons.gov.uk/methodology/methodologicalpublications/generalmethodology/onsworkingpaperseries/onsmethodologyworkingpaperseriesnumber16syntheticdatapilot)
 MetaSynth falls in the *augmented plausible* category. To generate synthetic data, MetaSynth converts a polars DataFrame
```

### Comparing `metasynth-0.2.2/metasynth.egg-info/SOURCES.txt` & `metasynth-0.3.0/metasynth.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -23,37 +23,43 @@
 examples/demonstration.csv
 examples/descriptions.ipynb
 examples/titanic.ipynb
 examples/utils.py
 metasynth/__init__.py
 metasynth/_version.py
 metasynth/dataset.py
-metasynth/disttree.py
+metasynth/privacy.py
+metasynth/provider.py
 metasynth/py.typed
 metasynth/testutils.py
+metasynth/validation.py
 metasynth/var.py
 metasynth.egg-info/PKG-INFO
 metasynth.egg-info/SOURCES.txt
 metasynth.egg-info/dependency_links.txt
 metasynth.egg-info/entry_points.txt
 metasynth.egg-info/requires.txt
 metasynth.egg-info/top_level.txt
+metasynth/demo/__init__.py
+metasynth/demo/dataset.py
+metasynth/demo/demo_titanic.csv
 metasynth/distribution/__init__.py
 metasynth/distribution/base.py
 metasynth/distribution/categorical.py
 metasynth/distribution/continuous.py
 metasynth/distribution/datetime.py
 metasynth/distribution/discrete.py
 metasynth/distribution/faker.py
 metasynth/distribution/regex/__init__.py
 metasynth/distribution/regex/base.py
 metasynth/distribution/regex/element.py
 metasynth/distribution/regex/optimizer.py
 metasynth/schema/__init__.py
 metasynth/schema/generative_metadata_format.json
+tests/test_builtin.py
 tests/test_continuous.py
 tests/test_dataset.py
 tests/test_datetime.py
 tests/test_discrete.py
 tests/test_distribution.py
 tests/test_faker.py
 tests/test_regex.py
```

### Comparing `metasynth-0.2.2/pyproject.toml` & `metasynth-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     "pyarrow",  # Dependency of polars since we're converting from pandas.
     "scipy",
     "numpy>=1.20",
     "faker",
     "scikit-learn",
     "jsonschema",
     "importlib-metadata;python_version<'3.10'",
+    "importlib-resources;python_version<'3.9'",
     "wget",
 ]
 
 dynamic = ["version"]
 
 [project.urls]
 GitHub = "https://github.com/sodascience/metasynth"
@@ -45,35 +46,38 @@
 
 [project.optional-dependencies]
 test = [
 	"pytest", "pylint", "pydocstyle", "mypy", "flake8", "nbval",
 	"sphinx", "sphinx-rtd-theme", "sphinxcontrib-napoleon", "sphinx-autodoc-typehints"
 ]
 
-[project.entry-points."metasynth.disttree"]
-builtin = "metasynth.disttree:BuiltinDistributionTree"
+[project.entry-points."metasynth.distribution_provider"]
+builtin = "metasynth.provider:BuiltinDistributionProvider"
 
 [tool.setuptools]
 packages = ["metasynth"]
 
 [tool.setuptools_scm]
 write_to = "metasynth/_version.py"
 
 [[tool.mypy.overrides]]
 module = [
 	"scipy.*",
 	"pandas.*",
 	"jsonschema.*",
 	"sklearn.*",
 	"importlib_metadata.*",
+	"importlib_resources.*",
+	"wget.*",
 ]
 ignore_missing_imports = true
 
 [tool.pylint.'MASTER']
 ignore-patterns="_version.py"
 
 [tool.pylint.'FORMAT']
 max-line-length=100
 max-locals=35
+max-args=10
 
 [tool.pylint.'BASIC']
 good-names=["a", "b", "mu"]
```

### Comparing `metasynth-0.2.2/tests/data/titanic.csv` & `metasynth-0.3.0/tests/data/titanic.csv`

 * *Files identical despite different names*

### Comparing `metasynth-0.2.2/tests/test_continuous.py` & `metasynth-0.3.0/tests/test_continuous.py`

 * *Files identical despite different names*

### Comparing `metasynth-0.2.2/tests/test_dataset.py` & `metasynth-0.3.0/tests/test_dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pytest
 import pandas as pd
 import polars as pl
 from pytest import mark
 
 from metasynth.dataset import MetaDataset
 from metasynth.var import MetaVar
-from metasynth.disttree import get_disttree
+from metasynth.provider import get_distribution_provider
 
 
 dtypes = {
     "PassengerId": "int",
     "Survived": "category",
     "Pclass": "category",
     "Name": "string",
@@ -92,14 +92,14 @@
         print(name, dataset.descriptions[name])
         assert dataset.descriptions[name] == name
 
 
 def test_distributions(tmp_path):
     tmp_fp = tmp_path / "tmp.json"
 
-    dist_tree = get_disttree()
-    for var_type in dist_tree.all_var_types:
-        for dist in dist_tree.get_dist_list(var_type):
+    provider = get_distribution_provider()
+    for var_type in provider.all_var_types:
+        for dist in provider.get_dist_list(var_type):
             var = MetaVar(var_type, name="None", distribution=dist.default_distribution(),
                           prop_missing=random())
             dataset = MetaDataset([var], n_rows=10)
             dataset.to_json(tmp_fp)
```

### Comparing `metasynth-0.2.2/tests/test_datetime.py` & `metasynth-0.3.0/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `metasynth-0.2.2/tests/test_discrete.py` & `metasynth-0.3.0/tests/test_discrete.py`

 * *Files identical despite different names*

### Comparing `metasynth-0.2.2/tests/test_regex.py` & `metasynth-0.3.0/tests/test_regex.py`

 * *Files identical despite different names*

### Comparing `metasynth-0.2.2/tests/test_var.py` & `metasynth-0.3.0/tests/test_var.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     with raises(ValueError):
         var_dict = var.to_dict()
         var_dict.update({"type": "unknown"})
         MetaVar.from_dict(var_dict)
 
     with raises(ValueError):
         var_dict = var.to_dict()
-        var_dict["distribution"].update({"name": "unknown"})
+        var_dict["distribution"].update({"implements": "unknown"})
         MetaVar.from_dict(var_dict)
 
     newer_series = new_var.draw_series(len(series))
     check_similar(newer_series, series)
     with raises(ValueError):
         new_var.fit()
```

