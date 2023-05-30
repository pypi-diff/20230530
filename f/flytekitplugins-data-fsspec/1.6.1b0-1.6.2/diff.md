# Comparing `tmp/flytekitplugins-data-fsspec-1.6.1b0.tar.gz` & `tmp/flytekitplugins-data-fsspec-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-data-fsspec-1.6.1b0.tar", last modified: Mon May 15 22:07:02 2023, max compression
+gzip compressed data, was "flytekitplugins-data-fsspec-1.6.2.tar", last modified: Tue May 30 15:24:14 2023, max compression
```

## Comparing `flytekitplugins-data-fsspec-1.6.1b0.tar` & `flytekitplugins-data-fsspec-1.6.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:02.703832 flytekitplugins-data-fsspec-1.6.1b0/
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-15 22:07:02.703832 flytekitplugins-data-fsspec-1.6.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-15 22:06:44.000000 flytekitplugins-data-fsspec-1.6.1b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:02.703832 flytekitplugins-data-fsspec-1.6.1b0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:02.703832 flytekitplugins-data-fsspec-1.6.1b0/flytekitplugins/fsspec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 22:06:44.000000 flytekitplugins-data-fsspec-1.6.1b0/flytekitplugins/fsspec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:02.703832 flytekitplugins-data-fsspec-1.6.1b0/flytekitplugins_data_fsspec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-15 22:07:02.000000 flytekitplugins-data-fsspec-1.6.1b0/flytekitplugins_data_fsspec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-15 22:07:02.000000 flytekitplugins-data-fsspec-1.6.1b0/flytekitplugins_data_fsspec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 22:07:02.000000 flytekitplugins-data-fsspec-1.6.1b0/flytekitplugins_data_fsspec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 22:07:02.000000 flytekitplugins-data-fsspec-1.6.1b0/flytekitplugins_data_fsspec.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 22:07:02.000000 flytekitplugins-data-fsspec-1.6.1b0/flytekitplugins_data_fsspec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 22:07:02.000000 flytekitplugins-data-fsspec-1.6.1b0/flytekitplugins_data_fsspec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 22:07:02.703832 flytekitplugins-data-fsspec-1.6.1b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-15 22:07:00.000000 flytekitplugins-data-fsspec-1.6.1b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:14.237477 flytekitplugins-data-fsspec-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-30 15:24:14.237477 flytekitplugins-data-fsspec-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-30 15:23:56.000000 flytekitplugins-data-fsspec-1.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:14.233477 flytekitplugins-data-fsspec-1.6.2/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:14.233477 flytekitplugins-data-fsspec-1.6.2/flytekitplugins/fsspec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 15:23:56.000000 flytekitplugins-data-fsspec-1.6.2/flytekitplugins/fsspec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:14.233477 flytekitplugins-data-fsspec-1.6.2/flytekitplugins_data_fsspec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-30 15:24:14.000000 flytekitplugins-data-fsspec-1.6.2/flytekitplugins_data_fsspec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-30 15:24:14.000000 flytekitplugins-data-fsspec-1.6.2/flytekitplugins_data_fsspec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 15:24:14.000000 flytekitplugins-data-fsspec-1.6.2/flytekitplugins_data_fsspec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-30 15:24:14.000000 flytekitplugins-data-fsspec-1.6.2/flytekitplugins_data_fsspec.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 15:24:14.000000 flytekitplugins-data-fsspec-1.6.2/flytekitplugins_data_fsspec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-30 15:24:14.000000 flytekitplugins-data-fsspec-1.6.2/flytekitplugins_data_fsspec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 15:24:14.237477 flytekitplugins-data-fsspec-1.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-30 15:24:12.000000 flytekitplugins-data-fsspec-1.6.2/setup.py
```

### Comparing `flytekitplugins-data-fsspec-1.6.1b0/PKG-INFO` & `flytekitplugins-data-fsspec-1.6.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-data-fsspec
-Version: 1.6.1b0
+Version: 1.6.2
 Summary: This is a deprecated plugin as of flytekit 1.5
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-data-fsspec
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `flytekitplugins-data-fsspec-1.6.1b0/flytekitplugins_data_fsspec.egg-info/PKG-INFO` & `flytekitplugins-data-fsspec-1.6.2/flytekitplugins_data_fsspec.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-data-fsspec
-Version: 1.6.1b0
+Version: 1.6.2
 Summary: This is a deprecated plugin as of flytekit 1.5
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-data-fsspec
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `flytekitplugins-data-fsspec-1.6.1b0/setup.py` & `flytekitplugins-data-fsspec-1.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "fsspec"
 
 microlib_name = f"flytekitplugins-data-{PLUGIN_NAME}"
 
 plugin_requires = []
 
-__version__ = "1.6.1b0"
+__version__ = "1.6.2"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This is a deprecated plugin as of flytekit 1.5",
```

