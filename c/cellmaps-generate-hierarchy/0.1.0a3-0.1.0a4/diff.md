# Comparing `tmp/cellmaps_generate_hierarchy-0.1.0a3.tar.gz` & `tmp/cellmaps_generate_hierarchy-0.1.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellmaps_generate_hierarchy-0.1.0a3.tar", last modified: Fri May 26 18:12:10 2023, max compression
+gzip compressed data, was "dist/cellmaps_generate_hierarchy-0.1.0a4.tar", last modified: Tue May 30 21:18:55 2023, max compression
```

## Comparing `cellmaps_generate_hierarchy-0.1.0a3.tar` & `cellmaps_generate_hierarchy-0.1.0a4.tar`

### file list

```diff
@@ -1,57 +1,59 @@
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-26 18:12:10.917830 cellmaps_generate_hierarchy-0.1.0a3/
--rw-r--r--   0 churas     (504) staff       (20)      160 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/AUTHORS.rst
--rw-r--r--   0 churas     (504) staff       (20)     3761 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/CONTRIBUTING.rst
--rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-19 20:13:29.000000 cellmaps_generate_hierarchy-0.1.0a3/HISTORY.rst
--rw-r--r--   0 churas     (504) staff       (20)     1102 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/LICENSE
--rw-r--r--   0 churas     (504) staff       (20)      262 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/MANIFEST.in
--rw-r--r--   0 churas     (504) staff       (20)     6349 2023-05-26 18:12:10.917994 cellmaps_generate_hierarchy-0.1.0a3/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     4203 2023-05-25 22:06:47.000000 cellmaps_generate_hierarchy-0.1.0a3/README.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-26 18:12:10.909363 cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy/
--rw-r--r--   0 churas     (504) staff       (20)      325 2023-05-25 22:56:56.000000 cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     5400 2023-05-26 17:59:09.000000 cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy/cellmaps_generate_hierarchycmd.py
--rw-r--r--   0 churas     (504) staff       (20)      151 2023-05-10 16:59:50.000000 cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy/exceptions.py
--rw-r--r--   0 churas     (504) staff       (20)    17269 2023-05-26 18:04:18.000000 cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy/hierarchy.py
--rw-r--r--   0 churas     (504) staff       (20)     3764 2023-05-25 21:26:59.000000 cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy/ppi.py
--rw-r--r--   0 churas     (504) staff       (20)    12203 2023-05-26 18:09:44.000000 cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy/runner.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-26 18:12:10.910874 cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy.egg-info/
--rw-r--r--   0 churas     (504) staff       (20)     6349 2023-05-26 18:12:10.000000 cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy.egg-info/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     1369 2023-05-26 18:12:10.000000 cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy.egg-info/SOURCES.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-26 18:12:10.000000 cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy.egg-info/dependency_links.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-26 18:12:10.000000 cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy.egg-info/not-zip-safe
--rw-r--r--   0 churas     (504) staff       (20)       56 2023-05-26 18:12:10.000000 cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy.egg-info/requires.txt
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-05-26 18:12:10.000000 cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy.egg-info/top_level.txt
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-26 18:12:10.914943 cellmaps_generate_hierarchy-0.1.0a3/docs/
--rw-r--r--   0 churas     (504) staff       (20)      628 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/Makefile
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-26 18:12:10.903726 cellmaps_generate_hierarchy-0.1.0a3/docs/_build/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-26 18:12:10.903827 cellmaps_generate_hierarchy-0.1.0a3/docs/_build/html/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-26 18:12:10.915724 cellmaps_generate_hierarchy-0.1.0a3/docs/_build/html/_static/
--rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/_build/html/_static/file.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/_build/html/_static/minus.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/_build/html/_static/plus.png
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/authors.rst
--rw-r--r--   0 churas     (504) staff       (20)     1294 2023-05-22 23:59:36.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/cellmaps_generate_hierarchy.rst
--rwxr-xr-x   0 churas     (504) staff       (20)     6155 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/conf.py
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/contributing.rst
--rw-r--r--   0 churas     (504) staff       (20)      174 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/devbranches.rst
--rw-r--r--   0 churas     (504) staff       (20)      295 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/developer.rst
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/history.rst
--rw-r--r--   0 churas     (504) staff       (20)     1004 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/index.rst
--rw-r--r--   0 churas     (504) staff       (20)     1269 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/installation.rst
--rw-r--r--   0 churas     (504) staff       (20)      481 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/integrationtesting.rst
--rw-r--r--   0 churas     (504) staff       (20)      825 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/make.bat
--rw-r--r--   0 churas     (504) staff       (20)       86 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/modules.rst
--rw-r--r--   0 churas     (504) staff       (20)     4460 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/newrelease.rst
--rw-r--r--   0 churas     (504) staff       (20)      797 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/pypircfile.rst
--rw-r--r--   0 churas     (504) staff       (20)      757 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/usage.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/docs/versioningscheme.rst
--rw-r--r--   0 churas     (504) staff       (20)      410 2023-05-26 18:12:10.918537 cellmaps_generate_hierarchy-0.1.0a3/setup.cfg
--rw-r--r--   0 churas     (504) staff       (20)     2310 2023-05-25 23:23:13.000000 cellmaps_generate_hierarchy-0.1.0a3/setup.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-26 18:12:10.917324 cellmaps_generate_hierarchy-0.1.0a3/tests/
--rw-r--r--   0 churas     (504) staff       (20)       82 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/tests/__init__.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-26 18:12:10.917595 cellmaps_generate_hierarchy-0.1.0a3/tests/data/
--rw-r--r--   0 churas     (504) staff       (20)    10232 2023-05-10 19:56:53.000000 cellmaps_generate_hierarchy-0.1.0a3/tests/data/fake_4_node_coembedding.tsv
--rw-r--r--   0 churas     (504) staff       (20)     1182 2023-05-11 00:02:02.000000 cellmaps_generate_hierarchy-0.1.0a3/tests/test_cdapshierarchygenerator.py
--rw-r--r--   0 churas     (504) staff       (20)     1840 2023-05-19 20:32:56.000000 cellmaps_generate_hierarchy-0.1.0a3/tests/test_cellmaps_generate_hierarchycmd.py
--rw-r--r--   0 churas     (504) staff       (20)      787 2023-05-11 00:02:17.000000 cellmaps_generate_hierarchy-0.1.0a3/tests/test_cellmapsgeneratehierarchy.py
--rw-r--r--   0 churas     (504) staff       (20)     1512 2023-05-10 21:34:27.000000 cellmaps_generate_hierarchy-0.1.0a3/tests/test_cosinesimilarityppigenerator.py
--rw-r--r--   0 churas     (504) staff       (20)      842 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a3/tests/test_integration_cellmaps_generate_hierarchy.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 21:18:55.078205 cellmaps_generate_hierarchy-0.1.0a4/
+-rw-r--r--   0 churas     (504) staff       (20)      160 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/AUTHORS.rst
+-rw-r--r--   0 churas     (504) staff       (20)     3761 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/CONTRIBUTING.rst
+-rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-19 20:13:29.000000 cellmaps_generate_hierarchy-0.1.0a4/HISTORY.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1102 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/LICENSE
+-rw-r--r--   0 churas     (504) staff       (20)      262 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/MANIFEST.in
+-rw-r--r--   0 churas     (504) staff       (20)     6349 2023-05-30 21:18:55.078354 cellmaps_generate_hierarchy-0.1.0a4/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     4203 2023-05-27 00:03:19.000000 cellmaps_generate_hierarchy-0.1.0a4/README.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 21:18:55.069113 cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy/
+-rw-r--r--   0 churas     (504) staff       (20)      325 2023-05-30 21:18:21.000000 cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     5400 2023-05-26 18:13:01.000000 cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy/cellmaps_generate_hierarchycmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      151 2023-05-10 16:59:50.000000 cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy/exceptions.py
+-rw-r--r--   0 churas     (504) staff       (20)    17254 2023-05-27 00:03:19.000000 cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy/hierarchy.py
+-rw-r--r--   0 churas     (504) staff       (20)     3764 2023-05-26 18:13:01.000000 cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy/ppi.py
+-rw-r--r--   0 churas     (504) staff       (20)    12203 2023-05-26 18:13:01.000000 cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy/runner.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 21:18:55.070350 cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy.egg-info/
+-rw-r--r--   0 churas     (504) staff       (20)     6349 2023-05-30 21:18:55.000000 cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy.egg-info/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     1429 2023-05-30 21:18:55.000000 cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy.egg-info/SOURCES.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-30 21:18:55.000000 cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy.egg-info/dependency_links.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-30 21:18:55.000000 cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy.egg-info/not-zip-safe
+-rw-r--r--   0 churas     (504) staff       (20)       56 2023-05-30 21:18:55.000000 cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy.egg-info/requires.txt
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-05-30 21:18:55.000000 cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy.egg-info/top_level.txt
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 21:18:55.075042 cellmaps_generate_hierarchy-0.1.0a4/docs/
+-rw-r--r--   0 churas     (504) staff       (20)      628 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/Makefile
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 21:18:55.064921 cellmaps_generate_hierarchy-0.1.0a4/docs/_build/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 21:18:55.064990 cellmaps_generate_hierarchy-0.1.0a4/docs/_build/html/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 21:18:55.075788 cellmaps_generate_hierarchy-0.1.0a4/docs/_build/html/_static/
+-rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/_build/html/_static/file.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/_build/html/_static/minus.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/_build/html/_static/plus.png
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/authors.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1294 2023-05-22 23:59:36.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/cellmaps_generate_hierarchy.rst
+-rwxr-xr-x   0 churas     (504) staff       (20)     6155 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/conf.py
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/contributing.rst
+-rw-r--r--   0 churas     (504) staff       (20)      174 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/devbranches.rst
+-rw-r--r--   0 churas     (504) staff       (20)      295 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/developer.rst
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/history.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1004 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/index.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1269 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/installation.rst
+-rw-r--r--   0 churas     (504) staff       (20)      481 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/integrationtesting.rst
+-rw-r--r--   0 churas     (504) staff       (20)      825 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/make.bat
+-rw-r--r--   0 churas     (504) staff       (20)       86 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/modules.rst
+-rw-r--r--   0 churas     (504) staff       (20)     4460 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/newrelease.rst
+-rw-r--r--   0 churas     (504) staff       (20)      797 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/pypircfile.rst
+-rw-r--r--   0 churas     (504) staff       (20)      757 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/usage.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/docs/versioningscheme.rst
+-rw-r--r--   0 churas     (504) staff       (20)      410 2023-05-30 21:18:55.078837 cellmaps_generate_hierarchy-0.1.0a4/setup.cfg
+-rw-r--r--   0 churas     (504) staff       (20)     2310 2023-05-25 23:23:13.000000 cellmaps_generate_hierarchy-0.1.0a4/setup.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 21:18:55.077257 cellmaps_generate_hierarchy-0.1.0a4/tests/
+-rw-r--r--   0 churas     (504) staff       (20)       82 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/tests/__init__.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-30 21:18:55.078023 cellmaps_generate_hierarchy-0.1.0a4/tests/data/
+-rw-r--r--   0 churas     (504) staff       (20)    10232 2023-05-10 19:56:53.000000 cellmaps_generate_hierarchy-0.1.0a4/tests/data/fake_4_node_coembedding.tsv
+-rw-r--r--   0 churas     (504) staff       (20)       30 2023-05-27 00:03:19.000000 cellmaps_generate_hierarchy-0.1.0a4/tests/data/hidef_output.edges
+-rw-r--r--   0 churas     (504) staff       (20)       62 2023-05-27 00:03:19.000000 cellmaps_generate_hierarchy-0.1.0a4/tests/data/hidef_output.nodes
+-rw-r--r--   0 churas     (504) staff       (20)     9132 2023-05-27 00:03:19.000000 cellmaps_generate_hierarchy-0.1.0a4/tests/test_cdapshierarchygenerator.py
+-rw-r--r--   0 churas     (504) staff       (20)     1840 2023-05-19 20:32:56.000000 cellmaps_generate_hierarchy-0.1.0a4/tests/test_cellmaps_generate_hierarchycmd.py
+-rw-r--r--   0 churas     (504) staff       (20)      787 2023-05-11 00:02:17.000000 cellmaps_generate_hierarchy-0.1.0a4/tests/test_cellmapsgeneratehierarchy.py
+-rw-r--r--   0 churas     (504) staff       (20)     1512 2023-05-10 21:34:27.000000 cellmaps_generate_hierarchy-0.1.0a4/tests/test_cosinesimilarityppigenerator.py
+-rw-r--r--   0 churas     (504) staff       (20)      842 2023-04-04 22:29:37.000000 cellmaps_generate_hierarchy-0.1.0a4/tests/test_integration_cellmaps_generate_hierarchy.py
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a3/CONTRIBUTING.rst` & `cellmaps_generate_hierarchy-0.1.0a4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a3/LICENSE` & `cellmaps_generate_hierarchy-0.1.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a3/PKG-INFO` & `cellmaps_generate_hierarchy-0.1.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps_generate_hierarchy
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: A tool to generate hierarchies from protein to protein interaction networks
 Home-page: https://github.com/idekerlab/cellmaps_generate_hierarchy
 Author: Clara Hu
 Author-email: mhu@ucsd.edu
 License: MIT license
 Description: ========================
         CM4AI Generate Hierarchy
@@ -32,16 +32,16 @@
         ------------
         
         * `cellmaps_utils <https://pypi.org/project/cellmaps-utils>`__
         * `tqdm <https://pypi.org/project/tqdm>`__
         * `pandas <https://pypi.org/project/pandas>`__
         * `numpy <https://pypi.org/project/numpy>`__
         * `ndex2 <https://pypi.org/project/ndex2>`__
-        * `HiDef <https://github.com/fanzheng10/HiDeF>`__
-           HiDef must be built directly from source which can be done by running the following commands:
+        * `HiDeF <https://github.com/fanzheng10/HiDeF>`__
+           HiDeF must be built directly from source which can be done by running the following commands:
         
           .. code-block:: python
         
             git clone https://github.com/fanzheng10/HiDeF.git
             cd HiDeF
             make dist
             pip install dist/hidef*whl
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a3/README.rst` & `cellmaps_generate_hierarchy-0.1.0a4/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 ------------
 
 * `cellmaps_utils <https://pypi.org/project/cellmaps-utils>`__
 * `tqdm <https://pypi.org/project/tqdm>`__
 * `pandas <https://pypi.org/project/pandas>`__
 * `numpy <https://pypi.org/project/numpy>`__
 * `ndex2 <https://pypi.org/project/ndex2>`__
-* `HiDef <https://github.com/fanzheng10/HiDeF>`__
-   HiDef must be built directly from source which can be done by running the following commands:
+* `HiDeF <https://github.com/fanzheng10/HiDeF>`__
+   HiDeF must be built directly from source which can be done by running the following commands:
 
   .. code-block:: python
 
     git clone https://github.com/fanzheng10/HiDeF.git
     cd HiDeF
     make dist
     pip install dist/hidef*whl
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy/cellmaps_generate_hierarchycmd.py` & `cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy/cellmaps_generate_hierarchycmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy/hierarchy.py` & `cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy/hierarchy.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,14 @@
         Constructor
         """
         super().__init__(provenance_utils=provenance_utils,
                          author=author,
                          version=version)
         self._hidef_cmd = hidef_cmd
 
-
     def _get_max_node_id(self, nodes_file):
         """
         Examines the 'nodes_file' passed in and finds the value of
         highest node id.
 
         It is assumed the 'nodes_file' a tab delimited
         file of format:
@@ -327,15 +326,15 @@
 
             # find the largest network by edge count
             if edge_count >= max_edge_count:
                 largest_network = net
 
                 # register edgelist file with fairscape
                 data_dict = {'name': os.path.basename(dest_path) +
-                                     ' PPI id edgelist file',
+                             ' PPI id edgelist file',
                              'description': 'PPI id edgelist file',
                              'data-format': 'tsv',
                              'author': self._author,
                              'version': self._version,
                              'date-published': date.today().strftime('%m-%d-%Y')}
                 dataset_id = self._provenance_utils.register_dataset(os.path.dirname(dest_path),
                                                                      source_file=dest_path,
@@ -435,13 +434,7 @@
 
             cd = cdapsutil.CommunityDetection(runner=cdapsutil.ExternalResultsRunner())
             return cd.run_community_detection(largest_net, algorithm=cdaps_out_file)
 
         except FileNotFoundError as fe:
             logger.error('No output from hidef: ' + str(fe) + '\n')
         return None
-
-
-
-
-
-
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy/ppi.py` & `cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy/ppi.py`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy/runner.py` & `cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy/runner.py`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy.egg-info/PKG-INFO` & `cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps-generate-hierarchy
-Version: 0.1.0a3
+Version: 0.1.0a4
 Summary: A tool to generate hierarchies from protein to protein interaction networks
 Home-page: https://github.com/idekerlab/cellmaps_generate_hierarchy
 Author: Clara Hu
 Author-email: mhu@ucsd.edu
 License: MIT license
 Description: ========================
         CM4AI Generate Hierarchy
@@ -32,16 +32,16 @@
         ------------
         
         * `cellmaps_utils <https://pypi.org/project/cellmaps-utils>`__
         * `tqdm <https://pypi.org/project/tqdm>`__
         * `pandas <https://pypi.org/project/pandas>`__
         * `numpy <https://pypi.org/project/numpy>`__
         * `ndex2 <https://pypi.org/project/ndex2>`__
-        * `HiDef <https://github.com/fanzheng10/HiDeF>`__
-           HiDef must be built directly from source which can be done by running the following commands:
+        * `HiDeF <https://github.com/fanzheng10/HiDeF>`__
+           HiDeF must be built directly from source which can be done by running the following commands:
         
           .. code-block:: python
         
             git clone https://github.com/fanzheng10/HiDeF.git
             cd HiDeF
             make dist
             pip install dist/hidef*whl
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a3/cellmaps_generate_hierarchy.egg-info/SOURCES.txt` & `cellmaps_generate_hierarchy-0.1.0a4/cellmaps_generate_hierarchy.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -40,8 +40,10 @@
 docs/_build/html/_static/plus.png
 tests/__init__.py
 tests/test_cdapshierarchygenerator.py
 tests/test_cellmaps_generate_hierarchycmd.py
 tests/test_cellmapsgeneratehierarchy.py
 tests/test_cosinesimilarityppigenerator.py
 tests/test_integration_cellmaps_generate_hierarchy.py
-tests/data/fake_4_node_coembedding.tsv
+tests/data/fake_4_node_coembedding.tsv
+tests/data/hidef_output.edges
+tests/data/hidef_output.nodes
```

### Comparing `cellmaps_generate_hierarchy-0.1.0a3/docs/Makefile` & `cellmaps_generate_hierarchy-0.1.0a4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a3/docs/cellmaps_generate_hierarchy.rst` & `cellmaps_generate_hierarchy-0.1.0a4/docs/cellmaps_generate_hierarchy.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a3/docs/conf.py` & `cellmaps_generate_hierarchy-0.1.0a4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a3/docs/index.rst` & `cellmaps_generate_hierarchy-0.1.0a4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a3/docs/installation.rst` & `cellmaps_generate_hierarchy-0.1.0a4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a3/docs/make.bat` & `cellmaps_generate_hierarchy-0.1.0a4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a3/docs/newrelease.rst` & `cellmaps_generate_hierarchy-0.1.0a4/docs/newrelease.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a3/docs/pypircfile.rst` & `cellmaps_generate_hierarchy-0.1.0a4/docs/pypircfile.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a3/docs/usage.rst` & `cellmaps_generate_hierarchy-0.1.0a4/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a3/docs/versioningscheme.rst` & `cellmaps_generate_hierarchy-0.1.0a4/docs/versioningscheme.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a3/setup.py` & `cellmaps_generate_hierarchy-0.1.0a4/setup.py`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a3/tests/data/fake_4_node_coembedding.tsv` & `cellmaps_generate_hierarchy-0.1.0a4/tests/data/fake_4_node_coembedding.tsv`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a3/tests/test_cellmaps_generate_hierarchycmd.py` & `cellmaps_generate_hierarchy-0.1.0a4/tests/test_cellmaps_generate_hierarchycmd.py`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a3/tests/test_cellmapsgeneratehierarchy.py` & `cellmaps_generate_hierarchy-0.1.0a4/tests/test_cellmapsgeneratehierarchy.py`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a3/tests/test_cosinesimilarityppigenerator.py` & `cellmaps_generate_hierarchy-0.1.0a4/tests/test_cosinesimilarityppigenerator.py`

 * *Files identical despite different names*

### Comparing `cellmaps_generate_hierarchy-0.1.0a3/tests/test_integration_cellmaps_generate_hierarchy.py` & `cellmaps_generate_hierarchy-0.1.0a4/tests/test_integration_cellmaps_generate_hierarchy.py`

 * *Files identical despite different names*

