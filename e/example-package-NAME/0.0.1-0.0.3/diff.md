# Comparing `tmp/example_package_NAME-0.0.1.tar.gz` & `tmp/example_package_NAME-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "example_package_NAME-0.0.1.tar", last modified: Tue May 30 03:12:11 2023, max compression
+gzip compressed data, was "example_package_NAME-0.0.3.tar", last modified: Tue May 30 03:58:41 2023, max compression
```

## Comparing `example_package_NAME-0.0.1.tar` & `example_package_NAME-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,35 @@
-drwxrwxr-x   0 zss       (1000) zss       (1000)        0 2023-05-30 03:12:11.686015 example_package_NAME-0.0.1/
--rw-rw-r--   0 zss       (1000) zss       (1000)     1080 2023-05-29 14:46:18.000000 example_package_NAME-0.0.1/LICENSE
--rw-rw-r--   0 zss       (1000) zss       (1000)      682 2023-05-30 03:12:11.686015 example_package_NAME-0.0.1/PKG-INFO
--rw-rw-r--   0 zss       (1000) zss       (1000)      170 2023-05-29 07:49:05.000000 example_package_NAME-0.0.1/README.md
--rw-rw-r--   0 zss       (1000) zss       (1000)      584 2023-05-29 14:50:33.000000 example_package_NAME-0.0.1/pyproject.toml
--rw-rw-r--   0 zss       (1000) zss       (1000)       38 2023-05-30 03:12:11.686015 example_package_NAME-0.0.1/setup.cfg
-drwxrwxr-x   0 zss       (1000) zss       (1000)        0 2023-05-30 03:12:11.686015 example_package_NAME-0.0.1/src/
-drwxrwxr-x   0 zss       (1000) zss       (1000)        0 2023-05-30 03:12:11.686015 example_package_NAME-0.0.1/src/example_package_NAME/
--rw-rw-r--   0 zss       (1000) zss       (1000)        0 2023-05-29 07:44:05.000000 example_package_NAME-0.0.1/src/example_package_NAME/__init__.py
--rw-rw-r--   0 zss       (1000) zss       (1000)       42 2023-05-29 07:44:24.000000 example_package_NAME-0.0.1/src/example_package_NAME/example.py
-drwxrwxr-x   0 zss       (1000) zss       (1000)        0 2023-05-30 03:12:11.686015 example_package_NAME-0.0.1/src/example_package_NAME.egg-info/
--rw-rw-r--   0 zss       (1000) zss       (1000)      682 2023-05-30 03:12:11.000000 example_package_NAME-0.0.1/src/example_package_NAME.egg-info/PKG-INFO
--rw-rw-r--   0 zss       (1000) zss       (1000)      297 2023-05-30 03:12:11.000000 example_package_NAME-0.0.1/src/example_package_NAME.egg-info/SOURCES.txt
--rw-rw-r--   0 zss       (1000) zss       (1000)        1 2023-05-30 03:12:11.000000 example_package_NAME-0.0.1/src/example_package_NAME.egg-info/dependency_links.txt
--rw-rw-r--   0 zss       (1000) zss       (1000)       21 2023-05-30 03:12:11.000000 example_package_NAME-0.0.1/src/example_package_NAME.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:58:41.814988 example_package_NAME-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:58:41.810988 example_package_NAME-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:58:41.814988 example_package_NAME-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-30 03:58:26.000000 example_package_NAME-0.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-30 03:58:26.000000 example_package_NAME-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-30 03:58:26.000000 example_package_NAME-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-30 03:58:41.814988 example_package_NAME-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-30 03:58:26.000000 example_package_NAME-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:58:41.814988 example_package_NAME-0.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-30 03:58:26.000000 example_package_NAME-0.0.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-30 03:58:26.000000 example_package_NAME-0.0.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:58:41.814988 example_package_NAME-0.0.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-05-30 03:58:26.000000 example_package_NAME-0.0.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-30 03:58:26.000000 example_package_NAME-0.0.3/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:58:41.814988 example_package_NAME-0.0.3/docs/source/main/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:58:41.814988 example_package_NAME-0.0.3/docs/source/main/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-30 03:58:26.000000 example_package_NAME-0.0.3/docs/source/main/actions/contents.md
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-30 03:58:26.000000 example_package_NAME-0.0.3/docs/source/main/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:58:41.814988 example_package_NAME-0.0.3/docs/source/main/packaging/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-30 03:58:26.000000 example_package_NAME-0.0.3/docs/source/main/packaging/contents.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:58:41.814988 example_package_NAME-0.0.3/docs/source/main/read_the_docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-30 03:58:26.000000 example_package_NAME-0.0.3/docs/source/main/read_the_docs/contents.md
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-30 03:58:26.000000 example_package_NAME-0.0.3/prac.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-30 03:58:26.000000 example_package_NAME-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 03:58:41.814988 example_package_NAME-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:58:41.810988 example_package_NAME-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:58:41.814988 example_package_NAME-0.0.3/src/example_package_NAME/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 03:58:26.000000 example_package_NAME-0.0.3/src/example_package_NAME/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-30 03:58:41.000000 example_package_NAME-0.0.3/src/example_package_NAME/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-30 03:58:26.000000 example_package_NAME-0.0.3/src/example_package_NAME/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:58:41.814988 example_package_NAME-0.0.3/src/example_package_NAME.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-30 03:58:41.000000 example_package_NAME-0.0.3/src/example_package_NAME.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-30 03:58:41.000000 example_package_NAME-0.0.3/src/example_package_NAME.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 03:58:41.000000 example_package_NAME-0.0.3/src/example_package_NAME.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-30 03:58:41.000000 example_package_NAME-0.0.3/src/example_package_NAME.egg-info/top_level.txt
```

### Comparing `example_package_NAME-0.0.1/LICENSE` & `example_package_NAME-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `example_package_NAME-0.0.1/PKG-INFO` & `example_package_NAME-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: example_package_NAME
-Version: 0.0.1
+Version: 0.0.3
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `example_package_NAME-0.0.1/src/example_package_NAME.egg-info/PKG-INFO` & `example_package_NAME-0.0.3/src/example_package_NAME.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: example-package-NAME
-Version: 0.0.1
+Version: 0.0.3
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

