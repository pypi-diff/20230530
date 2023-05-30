# Comparing `tmp/flytekitplugins-whylogs-1.6.1b0.tar.gz` & `tmp/flytekitplugins-whylogs-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-whylogs-1.6.1b0.tar", last modified: Mon May 15 22:07:11 2023, max compression
+gzip compressed data, was "flytekitplugins-whylogs-1.6.2.tar", last modified: Tue May 30 15:24:23 2023, max compression
```

## Comparing `flytekitplugins-whylogs-1.6.1b0.tar` & `flytekitplugins-whylogs-1.6.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:11.539773 flytekitplugins-whylogs-1.6.1b0/
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-15 22:07:11.539773 flytekitplugins-whylogs-1.6.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-15 22:06:44.000000 flytekitplugins-whylogs-1.6.1b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:11.539773 flytekitplugins-whylogs-1.6.1b0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:11.539773 flytekitplugins-whylogs-1.6.1b0/flytekitplugins/whylogs/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-15 22:06:44.000000 flytekitplugins-whylogs-1.6.1b0/flytekitplugins/whylogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-05-15 22:06:44.000000 flytekitplugins-whylogs-1.6.1b0/flytekitplugins/whylogs/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-15 22:06:44.000000 flytekitplugins-whylogs-1.6.1b0/flytekitplugins/whylogs/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:11.539773 flytekitplugins-whylogs-1.6.1b0/flytekitplugins_whylogs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-15 22:07:11.000000 flytekitplugins-whylogs-1.6.1b0/flytekitplugins_whylogs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-15 22:07:11.000000 flytekitplugins-whylogs-1.6.1b0/flytekitplugins_whylogs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 22:07:11.000000 flytekitplugins-whylogs-1.6.1b0/flytekitplugins_whylogs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-15 22:07:11.000000 flytekitplugins-whylogs-1.6.1b0/flytekitplugins_whylogs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 22:07:11.000000 flytekitplugins-whylogs-1.6.1b0/flytekitplugins_whylogs.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-15 22:07:11.000000 flytekitplugins-whylogs-1.6.1b0/flytekitplugins_whylogs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 22:07:11.000000 flytekitplugins-whylogs-1.6.1b0/flytekitplugins_whylogs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 22:07:11.539773 flytekitplugins-whylogs-1.6.1b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-15 22:07:00.000000 flytekitplugins-whylogs-1.6.1b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:23.125524 flytekitplugins-whylogs-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-30 15:24:23.125524 flytekitplugins-whylogs-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-30 15:23:56.000000 flytekitplugins-whylogs-1.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:23.125524 flytekitplugins-whylogs-1.6.2/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:23.125524 flytekitplugins-whylogs-1.6.2/flytekitplugins/whylogs/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-30 15:23:56.000000 flytekitplugins-whylogs-1.6.2/flytekitplugins/whylogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-05-30 15:23:56.000000 flytekitplugins-whylogs-1.6.2/flytekitplugins/whylogs/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-30 15:23:56.000000 flytekitplugins-whylogs-1.6.2/flytekitplugins/whylogs/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:23.125524 flytekitplugins-whylogs-1.6.2/flytekitplugins_whylogs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-30 15:24:23.000000 flytekitplugins-whylogs-1.6.2/flytekitplugins_whylogs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-30 15:24:23.000000 flytekitplugins-whylogs-1.6.2/flytekitplugins_whylogs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 15:24:23.000000 flytekitplugins-whylogs-1.6.2/flytekitplugins_whylogs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-30 15:24:23.000000 flytekitplugins-whylogs-1.6.2/flytekitplugins_whylogs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-30 15:24:23.000000 flytekitplugins-whylogs-1.6.2/flytekitplugins_whylogs.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-30 15:24:23.000000 flytekitplugins-whylogs-1.6.2/flytekitplugins_whylogs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-30 15:24:23.000000 flytekitplugins-whylogs-1.6.2/flytekitplugins_whylogs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 15:24:23.125524 flytekitplugins-whylogs-1.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-30 15:24:12.000000 flytekitplugins-whylogs-1.6.2/setup.py
```

### Comparing `flytekitplugins-whylogs-1.6.1b0/PKG-INFO` & `flytekitplugins-whylogs-1.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-whylogs
-Version: 1.6.1b0
+Version: 1.6.2
 Summary: Enable the use of whylogs profiles to be used in flyte tasks to get aggregate statistics about data.
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-whylogs
 Author: whylabs
 Author-email: support@whylabs.ai
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `flytekitplugins-whylogs-1.6.1b0/README.md` & `flytekitplugins-whylogs-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-whylogs-1.6.1b0/flytekitplugins/whylogs/renderer.py` & `flytekitplugins-whylogs-1.6.2/flytekitplugins/whylogs/renderer.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-whylogs-1.6.1b0/flytekitplugins/whylogs/schema.py` & `flytekitplugins-whylogs-1.6.2/flytekitplugins/whylogs/schema.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-whylogs-1.6.1b0/flytekitplugins_whylogs.egg-info/PKG-INFO` & `flytekitplugins-whylogs-1.6.2/flytekitplugins_whylogs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-whylogs
-Version: 1.6.1b0
+Version: 1.6.2
 Summary: Enable the use of whylogs profiles to be used in flyte tasks to get aggregate statistics about data.
 Home-page: https://github.com/flyteorg/flytekit/tree/master/plugins/flytekit-whylogs
 Author: whylabs
 Author-email: support@whylabs.ai
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `flytekitplugins-whylogs-1.6.1b0/setup.py` & `flytekitplugins-whylogs-1.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "whylogs"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "whylogs[viz]>=1.1.16"]
 
-__version__ = "1.6.1b0"
+__version__ = "1.6.2"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="whylabs",
     author_email="support@whylabs.ai",
     description="Enable the use of whylogs profiles to be used in flyte tasks to get aggregate statistics about data.",
```

