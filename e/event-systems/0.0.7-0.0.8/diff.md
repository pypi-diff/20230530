# Comparing `tmp/event-systems-0.0.7.tar.gz` & `tmp/event-systems-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "event-systems-0.0.7.tar", last modified: Sat Apr 29 16:00:50 2023, max compression
+gzip compressed data, was "event-systems-0.0.8.tar", last modified: Tue May 30 16:22:35 2023, max compression
```

## Comparing `event-systems-0.0.7.tar` & `event-systems-0.0.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:00:50.630689 event-systems-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-29 16:00:39.000000 event-systems-0.0.7/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-29 16:00:50.630689 event-systems-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-29 16:00:39.000000 event-systems-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:00:50.630689 event-systems-0.0.7/event_systems/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 16:00:39.000000 event-systems-0.0.7/event_systems/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:00:50.630689 event-systems-0.0.7/event_systems/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 16:00:39.000000 event-systems-0.0.7/event_systems/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-29 16:00:39.000000 event-systems-0.0.7/event_systems/base/event_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:00:50.630689 event-systems-0.0.7/event_systems/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 16:00:39.000000 event-systems-0.0.7/event_systems/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-29 16:00:39.000000 event-systems-0.0.7/event_systems/internal/event_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-29 16:00:39.000000 event-systems-0.0.7/event_systems/internal/event_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:00:50.630689 event-systems-0.0.7/event_systems/shared/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 16:00:39.000000 event-systems-0.0.7/event_systems/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-29 16:00:39.000000 event-systems-0.0.7/event_systems/shared/event_listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-29 16:00:39.000000 event-systems-0.0.7/event_systems/shared/event_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:00:50.630689 event-systems-0.0.7/event_systems.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-29 16:00:50.000000 event-systems-0.0.7/event_systems.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-29 16:00:50.000000 event-systems-0.0.7/event_systems.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 16:00:50.000000 event-systems-0.0.7/event_systems.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-29 16:00:50.000000 event-systems-0.0.7/event_systems.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-29 16:00:39.000000 event-systems-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 16:00:50.630689 event-systems-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 16:00:50.630689 event-systems-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-04-29 16:00:39.000000 event-systems-0.0.7/tests/test_internal_event_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-04-29 16:00:39.000000 event-systems-0.0.7/tests/test_shared_event_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:22:35.182108 event-systems-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-30 16:22:23.000000 event-systems-0.0.8/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-30 16:22:35.182108 event-systems-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-30 16:22:23.000000 event-systems-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:22:35.182108 event-systems-0.0.8/event_systems/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 16:22:23.000000 event-systems-0.0.8/event_systems/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:22:35.182108 event-systems-0.0.8/event_systems/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 16:22:23.000000 event-systems-0.0.8/event_systems/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-30 16:22:23.000000 event-systems-0.0.8/event_systems/base/event_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:22:35.182108 event-systems-0.0.8/event_systems/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 16:22:23.000000 event-systems-0.0.8/event_systems/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-30 16:22:23.000000 event-systems-0.0.8/event_systems/internal/event_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-30 16:22:23.000000 event-systems-0.0.8/event_systems/internal/event_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:22:35.182108 event-systems-0.0.8/event_systems/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 16:22:23.000000 event-systems-0.0.8/event_systems/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-30 16:22:23.000000 event-systems-0.0.8/event_systems/shared/event_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-30 16:22:23.000000 event-systems-0.0.8/event_systems/shared/event_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:22:35.182108 event-systems-0.0.8/event_systems.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-30 16:22:35.000000 event-systems-0.0.8/event_systems.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-30 16:22:35.000000 event-systems-0.0.8/event_systems.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 16:22:35.000000 event-systems-0.0.8/event_systems.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-30 16:22:35.000000 event-systems-0.0.8/event_systems.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-30 16:22:23.000000 event-systems-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 16:22:35.182108 event-systems-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:22:35.182108 event-systems-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-30 16:22:23.000000 event-systems-0.0.8/tests/test_internal_event_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-05-30 16:22:23.000000 event-systems-0.0.8/tests/test_shared_event_system.py
```

### Comparing `event-systems-0.0.7/LICENCE` & `event-systems-0.0.8/LICENCE`

 * *Files identical despite different names*

### Comparing `event-systems-0.0.7/PKG-INFO` & `event-systems-0.0.8/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: event-systems
-Version: 0.0.7
+Version: 0.0.8
 Summary: A collection of thread-safe event systems which components can use to subscribe and post to other components.
 Author-email: sir even <sir_even@icloud.com>
 Project-URL: Homepage, https://github.com/sirEven/event-systems.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `event-systems-0.0.7/event_systems/internal/event_system.py` & `event-systems-0.0.8/event_systems/internal/event_system.py`

 * *Files identical despite different names*

### Comparing `event-systems-0.0.7/event_systems/shared/event_system.py` & `event-systems-0.0.8/event_systems/shared/event_system.py`

 * *Files identical despite different names*

### Comparing `event-systems-0.0.7/event_systems.egg-info/PKG-INFO` & `event-systems-0.0.8/event_systems.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: event-systems
-Version: 0.0.7
+Version: 0.0.8
 Summary: A collection of thread-safe event systems which components can use to subscribe and post to other components.
 Author-email: sir even <sir_even@icloud.com>
 Project-URL: Homepage, https://github.com/sirEven/event-systems.git
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `event-systems-0.0.7/event_systems.egg-info/SOURCES.txt` & `event-systems-0.0.8/event_systems.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `event-systems-0.0.7/pyproject.toml` & `event-systems-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "event-systems"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="sir even", email="sir_even@icloud.com"},
 ]
 description = "A collection of thread-safe event systems which components can use to subscribe and post to other components."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `event-systems-0.0.7/tests/test_internal_event_system.py` & `event-systems-0.0.8/tests/test_internal_event_system.py`

 * *Files identical despite different names*

### Comparing `event-systems-0.0.7/tests/test_shared_event_system.py` & `event-systems-0.0.8/tests/test_shared_event_system.py`

 * *Files identical despite different names*

