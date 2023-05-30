# Comparing `tmp/flytekitplugins-dolt-1.6.1b0.tar.gz` & `tmp/flytekitplugins-dolt-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-dolt-1.6.1b0.tar", last modified: Mon May 15 22:07:03 2023, max compression
+gzip compressed data, was "flytekitplugins-dolt-1.6.2.tar", last modified: Tue May 30 15:24:15 2023, max compression
```

## Comparing `flytekitplugins-dolt-1.6.1b0.tar` & `flytekitplugins-dolt-1.6.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:03.807825 flytekitplugins-dolt-1.6.1b0/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-15 22:07:03.807825 flytekitplugins-dolt-1.6.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-15 22:06:44.000000 flytekitplugins-dolt-1.6.1b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:03.803825 flytekitplugins-dolt-1.6.1b0/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:03.803825 flytekitplugins-dolt-1.6.1b0/flytekitplugins/dolt/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-15 22:06:44.000000 flytekitplugins-dolt-1.6.1b0/flytekitplugins/dolt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-15 22:06:44.000000 flytekitplugins-dolt-1.6.1b0/flytekitplugins/dolt/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:03.807825 flytekitplugins-dolt-1.6.1b0/flytekitplugins_dolt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-15 22:07:03.000000 flytekitplugins-dolt-1.6.1b0/flytekitplugins_dolt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-15 22:07:03.000000 flytekitplugins-dolt-1.6.1b0/flytekitplugins_dolt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 22:07:03.000000 flytekitplugins-dolt-1.6.1b0/flytekitplugins_dolt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 22:07:03.000000 flytekitplugins-dolt-1.6.1b0/flytekitplugins_dolt.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-15 22:07:03.000000 flytekitplugins-dolt-1.6.1b0/flytekitplugins_dolt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 22:07:03.000000 flytekitplugins-dolt-1.6.1b0/flytekitplugins_dolt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:07:03.807825 flytekitplugins-dolt-1.6.1b0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-15 22:06:44.000000 flytekitplugins-dolt-1.6.1b0/scripts/flytekit_install_dolt.sh
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 22:07:03.807825 flytekitplugins-dolt-1.6.1b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-15 22:07:00.000000 flytekitplugins-dolt-1.6.1b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:15.333483 flytekitplugins-dolt-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-30 15:24:15.333483 flytekitplugins-dolt-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-30 15:23:56.000000 flytekitplugins-dolt-1.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:15.329482 flytekitplugins-dolt-1.6.2/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:15.333483 flytekitplugins-dolt-1.6.2/flytekitplugins/dolt/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-30 15:23:56.000000 flytekitplugins-dolt-1.6.2/flytekitplugins/dolt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-30 15:23:56.000000 flytekitplugins-dolt-1.6.2/flytekitplugins/dolt/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:15.333483 flytekitplugins-dolt-1.6.2/flytekitplugins_dolt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-30 15:24:15.000000 flytekitplugins-dolt-1.6.2/flytekitplugins_dolt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-30 15:24:15.000000 flytekitplugins-dolt-1.6.2/flytekitplugins_dolt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 15:24:15.000000 flytekitplugins-dolt-1.6.2/flytekitplugins_dolt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-30 15:24:15.000000 flytekitplugins-dolt-1.6.2/flytekitplugins_dolt.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-30 15:24:15.000000 flytekitplugins-dolt-1.6.2/flytekitplugins_dolt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-30 15:24:15.000000 flytekitplugins-dolt-1.6.2/flytekitplugins_dolt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:15.333483 flytekitplugins-dolt-1.6.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-30 15:23:56.000000 flytekitplugins-dolt-1.6.2/scripts/flytekit_install_dolt.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 15:24:15.333483 flytekitplugins-dolt-1.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-30 15:24:12.000000 flytekitplugins-dolt-1.6.2/setup.py
```

### Comparing `flytekitplugins-dolt-1.6.1b0/PKG-INFO` & `flytekitplugins-dolt-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-dolt
-Version: 1.6.1b0
+Version: 1.6.2
 Summary: Dolt plugin for flytekit
 Author: dolthub
 Author-email: max@dolthub.com
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-dolt-1.6.1b0/README.md` & `flytekitplugins-dolt-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-dolt-1.6.1b0/flytekitplugins/dolt/schema.py` & `flytekitplugins-dolt-1.6.2/flytekitplugins/dolt/schema.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-dolt-1.6.1b0/flytekitplugins_dolt.egg-info/PKG-INFO` & `flytekitplugins-dolt-1.6.2/flytekitplugins_dolt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-dolt
-Version: 1.6.1b0
+Version: 1.6.2
 Summary: Dolt plugin for flytekit
 Author: dolthub
 Author-email: max@dolthub.com
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-dolt-1.6.1b0/setup.py` & `flytekitplugins-dolt-1.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 PLUGIN_NAME = "dolt"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.3.0b2,<2.0.0", "dolt_integrations>=0.1.5"]
 dev_requires = ["pytest-mock>=3.6.1"]
 
-__version__ = "1.6.1b0"
+__version__ = "1.6.2"
 
 
 class PostDevelopCommand(develop):
     """Post-installation for development mode."""
 
     def run(self):
         develop.run(self)
```

