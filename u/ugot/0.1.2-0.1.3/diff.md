# Comparing `tmp/ugot-0.1.2.tar.gz` & `tmp/ugot-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ugot-0.1.2.tar", last modified: Tue May 23 07:12:23 2023, max compression
+gzip compressed data, was "ugot-0.1.3.tar", last modified: Tue May 30 02:55:46 2023, max compression
```

## Comparing `ugot-0.1.2.tar` & `ugot-0.1.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-05-23 07:12:23.741532 ugot-0.1.2/
--rw-r--r--   0 jesse      (501) staff       (20)     1103 2023-05-15 09:14:27.000000 ugot-0.1.2/LICENSE
--rw-r--r--   0 jesse      (501) staff       (20)      612 2023-05-23 07:12:23.741175 ugot-0.1.2/PKG-INFO
--rwxrwxrwx   0 jesse      (501) staff       (20)      246 2023-05-11 07:07:58.000000 ugot-0.1.2/README.md
--rwxrwxrwx   0 jesse      (501) staff       (20)      425 2023-05-11 07:31:52.000000 ugot-0.1.2/pyproject.toml
--rw-r--r--   0 jesse      (501) staff       (20)       38 2023-05-23 07:12:23.741632 ugot-0.1.2/setup.cfg
--rwxrwxrwx   0 jesse      (501) staff       (20)      558 2023-05-23 07:10:54.000000 ugot-0.1.2/setup.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-05-23 07:12:23.581520 ugot-0.1.2/ugot/
--rw-r--r--   0 jesse      (501) staff       (20)        0 2023-05-11 07:37:21.000000 ugot-0.1.2/ugot/__init__.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-05-23 07:12:23.682376 ugot-0.1.2/ugot/grpc_pb/
--rw-r--r--   0 jesse      (501) staff       (20)        0 2023-05-11 07:27:02.000000 ugot-0.1.2/ugot/grpc_pb/__init__.py
--rw-r--r--   0 jesse      (501) staff       (20)     6021 2023-05-15 03:20:28.000000 ugot-0.1.2/ugot/grpc_pb/audio_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    23990 2023-05-15 03:20:28.000000 ugot-0.1.2/ugot/grpc_pb/audio_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)     6234 2023-05-15 03:20:28.000000 ugot-0.1.2/ugot/grpc_pb/bluetooth_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    18284 2023-05-15 03:20:28.000000 ugot-0.1.2/ugot/grpc_pb/bluetooth_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)     9603 2023-05-15 03:20:28.000000 ugot-0.1.2/ugot/grpc_pb/device_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    30498 2023-05-15 03:20:28.000000 ugot-0.1.2/ugot/grpc_pb/device_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)     6103 2023-05-15 03:20:28.000000 ugot-0.1.2/ugot/grpc_pb/gpio_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    18277 2023-05-15 03:20:28.000000 ugot-0.1.2/ugot/grpc_pb/gpio_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)     8843 2023-05-15 03:20:28.000000 ugot-0.1.2/ugot/grpc_pb/model_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    23309 2023-05-15 03:20:28.000000 ugot-0.1.2/ugot/grpc_pb/model_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)     6803 2023-05-15 03:20:28.000000 ugot-0.1.2/ugot/grpc_pb/network_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    24828 2023-05-15 03:20:28.000000 ugot-0.1.2/ugot/grpc_pb/network_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)     2135 2023-05-15 03:20:28.000000 ugot-0.1.2/ugot/grpc_pb/power_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)     5561 2023-05-15 03:20:28.000000 ugot-0.1.2/ugot/grpc_pb/power_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)     5080 2023-05-15 03:20:28.000000 ugot-0.1.2/ugot/grpc_pb/sensor_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    13911 2023-05-15 03:20:28.000000 ugot-0.1.2/ugot/grpc_pb/sensor_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)    10875 2023-05-15 03:20:28.000000 ugot-0.1.2/ugot/grpc_pb/servo_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    24766 2023-05-15 03:20:28.000000 ugot-0.1.2/ugot/grpc_pb/servo_pb2_grpc.py
--rw-r--r--   0 jesse      (501) staff       (20)     5891 2023-05-15 03:20:28.000000 ugot-0.1.2/ugot/grpc_pb/vision_pb2.py
--rw-r--r--   0 jesse      (501) staff       (20)    16618 2023-05-15 03:20:28.000000 ugot-0.1.2/ugot/grpc_pb/vision_pb2_grpc.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-05-23 07:12:23.683125 ugot-0.1.2/ugot/protos/
--rw-r--r--   0 jesse      (501) staff       (20)        0 2023-05-11 07:27:02.000000 ugot-0.1.2/ugot/protos/__init__.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-05-23 07:12:23.727512 ugot-0.1.2/ugot/src/
--rw-r--r--   0 jesse      (501) staff       (20)        0 2023-05-11 07:27:02.000000 ugot-0.1.2/ugot/src/__init__.py
--rw-r--r--   0 jesse      (501) staff       (20)     2674 2023-05-11 07:27:02.000000 ugot-0.1.2/ugot/src/audio_client.py
--rw-r--r--   0 jesse      (501) staff       (20)      517 2023-05-11 07:27:02.000000 ugot-0.1.2/ugot/src/base_client.py
--rw-r--r--   0 jesse      (501) staff       (20)      615 2023-05-11 07:27:02.000000 ugot-0.1.2/ugot/src/bluetooth_client.py
--rw-r--r--   0 jesse      (501) staff       (20)     4159 2023-05-11 07:27:02.000000 ugot-0.1.2/ugot/src/device_client.py
--rw-r--r--   0 jesse      (501) staff       (20)     5085 2023-05-11 07:27:02.000000 ugot-0.1.2/ugot/src/enum.py
--rw-r--r--   0 jesse      (501) staff       (20)     3089 2023-05-11 07:27:02.000000 ugot-0.1.2/ugot/src/gpio_client.py
--rw-r--r--   0 jesse      (501) staff       (20)     8210 2023-05-11 07:27:02.000000 ugot-0.1.2/ugot/src/model_client.py
--rw-r--r--   0 jesse      (501) staff       (20)     5566 2023-05-11 07:27:02.000000 ugot-0.1.2/ugot/src/network_client.py
--rw-r--r--   0 jesse      (501) staff       (20)      592 2023-05-11 07:27:02.000000 ugot-0.1.2/ugot/src/power_client.py
--rw-r--r--   0 jesse      (501) staff       (20)     2031 2023-05-11 07:27:02.000000 ugot-0.1.2/ugot/src/scan_device.py
--rw-r--r--   0 jesse      (501) staff       (20)     1108 2023-05-11 07:27:02.000000 ugot-0.1.2/ugot/src/sensor_client.py
--rw-r--r--   0 jesse      (501) staff       (20)     2291 2023-05-11 07:27:02.000000 ugot-0.1.2/ugot/src/servo_client.py
--rw-r--r--   0 jesse      (501) staff       (20)     4110 2023-05-11 07:27:02.000000 ugot-0.1.2/ugot/src/util.py
--rw-r--r--   0 jesse      (501) staff       (20)    12490 2023-05-19 07:22:40.000000 ugot-0.1.2/ugot/src/vision_client.py
--rw-r--r--   0 jesse      (501) staff       (20)    86729 2023-05-23 06:36:29.000000 ugot-0.1.2/ugot/ugot.py
-drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-05-23 07:12:23.595019 ugot-0.1.2/ugot.egg-info/
--rw-r--r--   0 jesse      (501) staff       (20)      612 2023-05-23 07:12:23.000000 ugot-0.1.2/ugot.egg-info/PKG-INFO
--rw-r--r--   0 jesse      (501) staff       (20)     1206 2023-05-23 07:12:23.000000 ugot-0.1.2/ugot.egg-info/SOURCES.txt
--rw-r--r--   0 jesse      (501) staff       (20)        1 2023-05-23 07:12:23.000000 ugot-0.1.2/ugot.egg-info/dependency_links.txt
--rw-r--r--   0 jesse      (501) staff       (20)       67 2023-05-23 07:12:23.000000 ugot-0.1.2/ugot.egg-info/requires.txt
--rw-r--r--   0 jesse      (501) staff       (20)        5 2023-05-23 07:12:23.000000 ugot-0.1.2/ugot.egg-info/top_level.txt
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-05-30 02:55:46.218756 ugot-0.1.3/
+-rw-r--r--   0 jesse      (501) staff       (20)     1103 2023-05-15 09:14:27.000000 ugot-0.1.3/LICENSE
+-rw-r--r--   0 jesse      (501) staff       (20)      612 2023-05-30 02:55:46.218298 ugot-0.1.3/PKG-INFO
+-rwxrwxrwx   0 jesse      (501) staff       (20)      246 2023-05-11 07:07:58.000000 ugot-0.1.3/README.md
+-rwxrwxrwx   0 jesse      (501) staff       (20)      425 2023-05-30 02:54:52.000000 ugot-0.1.3/pyproject.toml
+-rw-r--r--   0 jesse      (501) staff       (20)       38 2023-05-30 02:55:46.218888 ugot-0.1.3/setup.cfg
+-rwxrwxrwx   0 jesse      (501) staff       (20)      558 2023-05-30 02:54:52.000000 ugot-0.1.3/setup.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-05-30 02:55:46.055563 ugot-0.1.3/ugot/
+-rw-r--r--   0 jesse      (501) staff       (20)        0 2023-05-11 07:37:21.000000 ugot-0.1.3/ugot/__init__.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-05-30 02:55:46.182883 ugot-0.1.3/ugot/grpc_pb/
+-rw-r--r--   0 jesse      (501) staff       (20)        0 2023-05-11 07:27:02.000000 ugot-0.1.3/ugot/grpc_pb/__init__.py
+-rw-r--r--   0 jesse      (501) staff       (20)     6021 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/audio_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    23990 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/audio_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)     6234 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/bluetooth_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    18284 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/bluetooth_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)     9603 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/device_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    30498 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/device_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)     6103 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/gpio_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    18277 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/gpio_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)     8843 2023-05-29 08:59:43.000000 ugot-0.1.3/ugot/grpc_pb/model_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    23309 2023-05-29 08:59:43.000000 ugot-0.1.3/ugot/grpc_pb/model_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)     6803 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/network_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    24828 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/network_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)     2135 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/power_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)     5561 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/power_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)     5080 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/sensor_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    13911 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/sensor_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)    10875 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/servo_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    24766 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/servo_pb2_grpc.py
+-rw-r--r--   0 jesse      (501) staff       (20)     5891 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/vision_pb2.py
+-rw-r--r--   0 jesse      (501) staff       (20)    16618 2023-05-15 03:20:28.000000 ugot-0.1.3/ugot/grpc_pb/vision_pb2_grpc.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-05-30 02:55:46.183664 ugot-0.1.3/ugot/protos/
+-rw-r--r--   0 jesse      (501) staff       (20)        0 2023-05-11 07:27:02.000000 ugot-0.1.3/ugot/protos/__init__.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-05-30 02:55:46.207967 ugot-0.1.3/ugot/src/
+-rw-r--r--   0 jesse      (501) staff       (20)        0 2023-05-11 07:27:02.000000 ugot-0.1.3/ugot/src/__init__.py
+-rw-r--r--   0 jesse      (501) staff       (20)     2674 2023-05-11 07:27:02.000000 ugot-0.1.3/ugot/src/audio_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)      517 2023-05-11 07:27:02.000000 ugot-0.1.3/ugot/src/base_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)      615 2023-05-11 07:27:02.000000 ugot-0.1.3/ugot/src/bluetooth_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)     4159 2023-05-11 07:27:02.000000 ugot-0.1.3/ugot/src/device_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)     5085 2023-05-11 07:27:02.000000 ugot-0.1.3/ugot/src/enum.py
+-rw-r--r--   0 jesse      (501) staff       (20)     3089 2023-05-11 07:27:02.000000 ugot-0.1.3/ugot/src/gpio_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)     8210 2023-05-29 08:59:43.000000 ugot-0.1.3/ugot/src/model_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)     5566 2023-05-11 07:27:02.000000 ugot-0.1.3/ugot/src/network_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)      592 2023-05-11 07:27:02.000000 ugot-0.1.3/ugot/src/power_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)     2031 2023-05-11 07:27:02.000000 ugot-0.1.3/ugot/src/scan_device.py
+-rw-r--r--   0 jesse      (501) staff       (20)     1108 2023-05-11 07:27:02.000000 ugot-0.1.3/ugot/src/sensor_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)     2291 2023-05-11 07:27:02.000000 ugot-0.1.3/ugot/src/servo_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)     4110 2023-05-11 07:27:02.000000 ugot-0.1.3/ugot/src/util.py
+-rw-r--r--   0 jesse      (501) staff       (20)    12490 2023-05-19 07:22:40.000000 ugot-0.1.3/ugot/src/vision_client.py
+-rw-r--r--   0 jesse      (501) staff       (20)    87110 2023-05-30 02:38:47.000000 ugot-0.1.3/ugot/ugot.py
+drwxr-xr-x   0 jesse      (501) staff       (20)        0 2023-05-30 02:55:46.057609 ugot-0.1.3/ugot.egg-info/
+-rw-r--r--   0 jesse      (501) staff       (20)      612 2023-05-30 02:55:46.000000 ugot-0.1.3/ugot.egg-info/PKG-INFO
+-rw-r--r--   0 jesse      (501) staff       (20)     1206 2023-05-30 02:55:46.000000 ugot-0.1.3/ugot.egg-info/SOURCES.txt
+-rw-r--r--   0 jesse      (501) staff       (20)        1 2023-05-30 02:55:46.000000 ugot-0.1.3/ugot.egg-info/dependency_links.txt
+-rw-r--r--   0 jesse      (501) staff       (20)       67 2023-05-30 02:55:46.000000 ugot-0.1.3/ugot.egg-info/requires.txt
+-rw-r--r--   0 jesse      (501) staff       (20)        5 2023-05-30 02:55:46.000000 ugot-0.1.3/ugot.egg-info/top_level.txt
```

### Comparing `ugot-0.1.2/LICENSE` & `ugot-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ugot-0.1.2/PKG-INFO` & `ugot-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ugot
-Version: 0.1.2
+Version: 0.1.3
 Summary: ugot-Python SDK
 Author-email: Jesse <jesse.huang@ubtrobot.com>
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `ugot-0.1.2/setup.py` & `ugot-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages, find_namespace_packages
 
 setup(
     name = "ugot",
-    version = "0.1.2",
+    version = "0.1.3",
     description = "ugot-Python SDK",
     long_description = "",
 
     packages = find_packages(include=["ugot","ugot.*"]),
     # package_data = {"ugot": ["*"],
     #                 },
     # packages=find_packages(),
```

### Comparing `ugot-0.1.2/ugot/grpc_pb/audio_pb2.py` & `ugot-0.1.3/ugot/grpc_pb/audio_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.2/ugot/grpc_pb/audio_pb2_grpc.py` & `ugot-0.1.3/ugot/grpc_pb/audio_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.2/ugot/grpc_pb/bluetooth_pb2.py` & `ugot-0.1.3/ugot/grpc_pb/bluetooth_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.2/ugot/grpc_pb/bluetooth_pb2_grpc.py` & `ugot-0.1.3/ugot/grpc_pb/bluetooth_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.2/ugot/grpc_pb/device_pb2.py` & `ugot-0.1.3/ugot/grpc_pb/device_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.2/ugot/grpc_pb/device_pb2_grpc.py` & `ugot-0.1.3/ugot/grpc_pb/device_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.2/ugot/grpc_pb/gpio_pb2.py` & `ugot-0.1.3/ugot/grpc_pb/gpio_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.2/ugot/grpc_pb/gpio_pb2_grpc.py` & `ugot-0.1.3/ugot/grpc_pb/gpio_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.2/ugot/grpc_pb/model_pb2.py` & `ugot-0.1.3/ugot/grpc_pb/model_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.2/ugot/grpc_pb/model_pb2_grpc.py` & `ugot-0.1.3/ugot/grpc_pb/model_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.2/ugot/grpc_pb/network_pb2.py` & `ugot-0.1.3/ugot/grpc_pb/network_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.2/ugot/grpc_pb/network_pb2_grpc.py` & `ugot-0.1.3/ugot/grpc_pb/network_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.2/ugot/grpc_pb/power_pb2.py` & `ugot-0.1.3/ugot/grpc_pb/power_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.2/ugot/grpc_pb/power_pb2_grpc.py` & `ugot-0.1.3/ugot/grpc_pb/power_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.2/ugot/grpc_pb/sensor_pb2.py` & `ugot-0.1.3/ugot/grpc_pb/sensor_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.2/ugot/grpc_pb/sensor_pb2_grpc.py` & `ugot-0.1.3/ugot/grpc_pb/sensor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.2/ugot/grpc_pb/servo_pb2.py` & `ugot-0.1.3/ugot/grpc_pb/servo_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.2/ugot/grpc_pb/servo_pb2_grpc.py` & `ugot-0.1.3/ugot/grpc_pb/servo_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.2/ugot/grpc_pb/vision_pb2.py` & `ugot-0.1.3/ugot/grpc_pb/vision_pb2.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.2/ugot/grpc_pb/vision_pb2_grpc.py` & `ugot-0.1.3/ugot/grpc_pb/vision_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.2/ugot/src/audio_client.py` & `ugot-0.1.3/ugot/src/audio_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.2/ugot/src/base_client.py` & `ugot-0.1.3/ugot/src/base_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.2/ugot/src/bluetooth_client.py` & `ugot-0.1.3/ugot/src/bluetooth_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.2/ugot/src/device_client.py` & `ugot-0.1.3/ugot/src/device_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.2/ugot/src/enum.py` & `ugot-0.1.3/ugot/src/enum.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.2/ugot/src/gpio_client.py` & `ugot-0.1.3/ugot/src/gpio_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.2/ugot/src/model_client.py` & `ugot-0.1.3/ugot/src/model_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.2/ugot/src/network_client.py` & `ugot-0.1.3/ugot/src/network_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.2/ugot/src/power_client.py` & `ugot-0.1.3/ugot/src/power_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.2/ugot/src/scan_device.py` & `ugot-0.1.3/ugot/src/scan_device.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.2/ugot/src/sensor_client.py` & `ugot-0.1.3/ugot/src/sensor_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.2/ugot/src/servo_client.py` & `ugot-0.1.3/ugot/src/servo_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.2/ugot/src/util.py` & `ugot-0.1.3/ugot/src/util.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.2/ugot/src/vision_client.py` & `ugot-0.1.3/ugot/src/vision_client.py`

 * *Files identical despite different names*

### Comparing `ugot-0.1.2/ugot/ugot.py` & `ugot-0.1.3/ugot/ugot.py`

 * *Files 0% similar despite different names*

```diff
@@ -292,15 +292,23 @@
             position (int): 角度，单位 度
             time (int): 时长，单位 ms
 
         Returns:
             无
 
         """
-        self.MODEL.transform_arm_control(joint, position, int(time / 20))
+        if not 1 <= joint <= 4:
+            typestr = 'invalid value of joint id, expected 1/2/3/4, got {}'.format(joint)
+            func_name = sys._getframe().f_code.co_name
+            error_msg = 'TypeError: {}(): {}'.format(func_name, typestr)
+            print(error_msg)
+            return
+        position = num_normal(position, 180, -180)
+        time = num_normal(time, 5000, 20)
+        self.MODEL.transform_arm_control(joint, position, time)
 
     def transform_adaption_control(self, option):
         """
         开启/关闭自适应，变形车可以根据不同地形调整姿态
 
         Args:
             option (bool): 开关状态 True表示开，False表示关
```

### Comparing `ugot-0.1.2/ugot.egg-info/PKG-INFO` & `ugot-0.1.3/ugot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ugot
-Version: 0.1.2
+Version: 0.1.3
 Summary: ugot-Python SDK
 Author-email: Jesse <jesse.huang@ubtrobot.com>
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `ugot-0.1.2/ugot.egg-info/SOURCES.txt` & `ugot-0.1.3/ugot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

