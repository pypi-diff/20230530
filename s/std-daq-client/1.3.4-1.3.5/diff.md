# Comparing `tmp/std_daq_client-1.3.4.tar.gz` & `tmp/std_daq_client-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "std_daq_client-1.3.4.tar", last modified: Mon May 29 22:09:51 2023, max compression
+gzip compressed data, was "std_daq_client-1.3.5.tar", last modified: Mon May 29 22:35:04 2023, max compression
```

## Comparing `std_daq_client-1.3.4.tar` & `std_daq_client-1.3.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-29 22:09:51.400818 std_daq_client-1.3.4/
--rw-r--r--   0 babic_a    (501) staff       (20)    10407 2023-05-29 22:09:51.400632 std_daq_client-1.3.4/PKG-INFO
--rw-r--r--   0 babic_a    (501) staff       (20)    11041 2023-05-29 21:27:28.000000 std_daq_client-1.3.4/README.md
--rw-r--r--   0 babic_a    (501) staff       (20)       38 2023-05-29 22:09:51.400851 std_daq_client-1.3.4/setup.cfg
--rw-r--r--   0 babic_a    (501) staff       (20)     1281 2023-05-29 21:27:28.000000 std_daq_client-1.3.4/setup.py
--rw-r--r--   0 babic_a    (501) staff       (20)     1172 2023-05-29 22:09:37.000000 std_daq_client-1.3.4/setup_client.py
-drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-29 22:09:51.399854 std_daq_client-1.3.4/std_daq_client/
--rw-r--r--   0 babic_a    (501) staff       (20)       68 2023-05-24 22:05:07.000000 std_daq_client-1.3.4/std_daq_client/__init__.py
--rw-r--r--   0 babic_a    (501) staff       (20)     4963 2023-05-29 21:44:57.000000 std_daq_client-1.3.4/std_daq_client/cli.py
--rw-r--r--   0 babic_a    (501) staff       (20)    12094 2023-05-29 21:27:28.000000 std_daq_client-1.3.4/std_daq_client/client.py
-drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-29 22:09:51.400468 std_daq_client-1.3.4/std_daq_client.egg-info/
--rw-r--r--   0 babic_a    (501) staff       (20)    10407 2023-05-29 22:09:51.000000 std_daq_client-1.3.4/std_daq_client.egg-info/PKG-INFO
--rw-r--r--   0 babic_a    (501) staff       (20)      338 2023-05-29 22:09:51.000000 std_daq_client-1.3.4/std_daq_client.egg-info/SOURCES.txt
--rw-r--r--   0 babic_a    (501) staff       (20)        1 2023-05-29 22:09:51.000000 std_daq_client-1.3.4/std_daq_client.egg-info/dependency_links.txt
--rw-r--r--   0 babic_a    (501) staff       (20)      487 2023-05-29 22:09:51.000000 std_daq_client-1.3.4/std_daq_client.egg-info/entry_points.txt
--rw-r--r--   0 babic_a    (501) staff       (20)        9 2023-05-29 22:09:51.000000 std_daq_client-1.3.4/std_daq_client.egg-info/requires.txt
--rw-r--r--   0 babic_a    (501) staff       (20)       15 2023-05-29 22:09:51.000000 std_daq_client-1.3.4/std_daq_client.egg-info/top_level.txt
+drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-29 22:35:04.318166 std_daq_client-1.3.5/
+-rw-r--r--   0 babic_a    (501) staff       (20)    10407 2023-05-29 22:35:04.317983 std_daq_client-1.3.5/PKG-INFO
+-rw-r--r--   0 babic_a    (501) staff       (20)    11041 2023-05-29 21:27:28.000000 std_daq_client-1.3.5/README.md
+-rw-r--r--   0 babic_a    (501) staff       (20)       38 2023-05-29 22:35:04.318196 std_daq_client-1.3.5/setup.cfg
+-rw-r--r--   0 babic_a    (501) staff       (20)     1281 2023-05-29 21:27:28.000000 std_daq_client-1.3.5/setup.py
+-rw-r--r--   0 babic_a    (501) staff       (20)     1172 2023-05-29 22:34:38.000000 std_daq_client-1.3.5/setup_client.py
+drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-29 22:35:04.317236 std_daq_client-1.3.5/std_daq_client/
+-rw-r--r--   0 babic_a    (501) staff       (20)       68 2023-05-24 22:05:07.000000 std_daq_client-1.3.5/std_daq_client/__init__.py
+-rw-r--r--   0 babic_a    (501) staff       (20)     4963 2023-05-29 21:44:57.000000 std_daq_client-1.3.5/std_daq_client/cli.py
+-rw-r--r--   0 babic_a    (501) staff       (20)    12094 2023-05-29 21:27:28.000000 std_daq_client-1.3.5/std_daq_client/client.py
+drwxr-xr-x   0 babic_a    (501) staff       (20)        0 2023-05-29 22:35:04.317841 std_daq_client-1.3.5/std_daq_client.egg-info/
+-rw-r--r--   0 babic_a    (501) staff       (20)    10407 2023-05-29 22:35:04.000000 std_daq_client-1.3.5/std_daq_client.egg-info/PKG-INFO
+-rw-r--r--   0 babic_a    (501) staff       (20)      338 2023-05-29 22:35:04.000000 std_daq_client-1.3.5/std_daq_client.egg-info/SOURCES.txt
+-rw-r--r--   0 babic_a    (501) staff       (20)        1 2023-05-29 22:35:04.000000 std_daq_client-1.3.5/std_daq_client.egg-info/dependency_links.txt
+-rw-r--r--   0 babic_a    (501) staff       (20)      487 2023-05-29 22:35:04.000000 std_daq_client-1.3.5/std_daq_client.egg-info/entry_points.txt
+-rw-r--r--   0 babic_a    (501) staff       (20)        9 2023-05-29 22:35:04.000000 std_daq_client-1.3.5/std_daq_client.egg-info/requires.txt
+-rw-r--r--   0 babic_a    (501) staff       (20)       15 2023-05-29 22:35:04.000000 std_daq_client-1.3.5/std_daq_client.egg-info/top_level.txt
```

### Comparing `std_daq_client-1.3.4/PKG-INFO` & `std_daq_client-1.3.5/std_daq_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: std_daq_client
-Version: 1.3.4
+Name: std-daq-client
+Version: 1.3.5
 Summary: Python client for standard-daq
 Home-page: https://github.com/paulscherrerinstitute/std_daq_service
 Author: Paul Scherrer Institute
 Description-Content-Type: text/markdown
 
 # Standard DAQ client
```

### Comparing `std_daq_client-1.3.4/README.md` & `std_daq_client-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `std_daq_client-1.3.4/setup.py` & `std_daq_client-1.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `std_daq_client-1.3.4/setup_client.py` & `std_daq_client-1.3.5/setup_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 from setuptools import setup
 
-CLIENT_VERSION = "1.3.4"
+CLIENT_VERSION = "1.3.5"
 
 with open(os.path.join(os.path.dirname(__file__), 'std_daq_client/', 'README.md')) as readme:
     long_description = readme.read()
 
 setup(
     version=CLIENT_VERSION,
     name='std_daq_client',
@@ -18,16 +18,16 @@
         [console_scripts]
         std_cli_get_config=std_daq_client.cli:get_config
         std_cli_set_config=std_daq_client.cli:set_config
         std_cli_get_deploy_status=std_daq_client.cli:get_deploy_status
         std_cli_get_logs=std_daq_client.cli:get_logs
         std_cli_get_stats=std_daq_client.cli:get_stats
         std_cli_get_status=std_daq_client.cli:get_status
-        std_cli_write_async=std_daq_client.cli:write_sync
-        std_cli_write_sync=std_daq_client.cli:write_async
+        std_cli_write_async=std_daq_client.cli:write_async
+        std_cli_write_sync=std_daq_client.cli:write_sync
         std_cli_write_stop=std_daq_client.cli:write_stop
     ''',
 
     author="Paul Scherrer Institute",
     url='https://github.com/paulscherrerinstitute/std_daq_service',
     description='Python client for standard-daq',
     long_description=long_description,
```

### Comparing `std_daq_client-1.3.4/std_daq_client/cli.py` & `std_daq_client-1.3.5/std_daq_client/cli.py`

 * *Files identical despite different names*

### Comparing `std_daq_client-1.3.4/std_daq_client/client.py` & `std_daq_client-1.3.5/std_daq_client/client.py`

 * *Files identical despite different names*

### Comparing `std_daq_client-1.3.4/std_daq_client.egg-info/PKG-INFO` & `std_daq_client-1.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: std-daq-client
-Version: 1.3.4
+Name: std_daq_client
+Version: 1.3.5
 Summary: Python client for standard-daq
 Home-page: https://github.com/paulscherrerinstitute/std_daq_service
 Author: Paul Scherrer Institute
 Description-Content-Type: text/markdown
 
 # Standard DAQ client
```

