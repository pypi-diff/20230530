# Comparing `tmp/meshtastic-2.1.7.tar.gz` & `tmp/meshtastic-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meshtastic-2.1.7.tar", last modified: Sun May 28 14:34:01 2023, max compression
+gzip compressed data, was "meshtastic-2.1.8.tar", last modified: Tue May 30 12:46:56 2023, max compression
```

## Comparing `meshtastic-2.1.7.tar` & `meshtastic-2.1.8.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:34:01.295622 meshtastic-2.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-28 14:33:46.000000 meshtastic-2.1.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-28 14:33:46.000000 meshtastic-2.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-28 14:34:01.295622 meshtastic-2.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-28 14:33:46.000000 meshtastic-2.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:34:01.291622 meshtastic-2.1.7/meshtastic/
--rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48555 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/admin_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/apponly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/ble.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/ble_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/cannedmessages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/channel_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/clientonly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13885 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/connection_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/device_metadata_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/deviceonly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/localonly_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    37626 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/mesh_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    19667 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/mesh_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14100 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/module_config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/mqtt_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    30559 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/portnums_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/remote_hardware.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/remote_hardware_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/rtttl_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/serial_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/storeforward_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/stream_interface.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6140 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/supported_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/tcp_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/telemetry_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/tunnel.py
--rw-r--r--   0 runner    (1001) docker     (123)    19869 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-28 14:33:46.000000 meshtastic-2.1.7/meshtastic/xmodem_pb2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:34:01.295622 meshtastic-2.1.7/meshtastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-28 14:34:01.000000 meshtastic-2.1.7/meshtastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-28 14:34:01.000000 meshtastic-2.1.7/meshtastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 14:34:01.000000 meshtastic-2.1.7/meshtastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-28 14:34:01.000000 meshtastic-2.1.7/meshtastic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-28 14:34:01.000000 meshtastic-2.1.7/meshtastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-28 14:34:01.000000 meshtastic-2.1.7/meshtastic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 14:34:01.295622 meshtastic-2.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-28 14:33:46.000000 meshtastic-2.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:46:56.532436 meshtastic-2.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-30 12:46:44.000000 meshtastic-2.1.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-30 12:46:44.000000 meshtastic-2.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-30 12:46:56.532436 meshtastic-2.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-30 12:46:44.000000 meshtastic-2.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:46:56.532436 meshtastic-2.1.8/meshtastic/
+-rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48555 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/admin_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/apponly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/ble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/ble_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/cannedmessages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/channel_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/clientonly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13943 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/connection_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/device_metadata_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/deviceonly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/localonly_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37626 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/mesh_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19752 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/mesh_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14192 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/module_config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/mqtt_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30559 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/portnums_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/remote_hardware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/remote_hardware_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/rtttl_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/serial_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/storeforward_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/stream_interface.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6140 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/supported_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/tcp_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5054 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/telemetry_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19869 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-30 12:46:44.000000 meshtastic-2.1.8/meshtastic/xmodem_pb2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:46:56.532436 meshtastic-2.1.8/meshtastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-30 12:46:56.000000 meshtastic-2.1.8/meshtastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-30 12:46:56.000000 meshtastic-2.1.8/meshtastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:46:56.000000 meshtastic-2.1.8/meshtastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-30 12:46:56.000000 meshtastic-2.1.8/meshtastic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-30 12:46:56.000000 meshtastic-2.1.8/meshtastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-30 12:46:56.000000 meshtastic-2.1.8/meshtastic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 12:46:56.536436 meshtastic-2.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-30 12:46:44.000000 meshtastic-2.1.8/setup.py
```

### Comparing `meshtastic-2.1.7/LICENSE.txt` & `meshtastic-2.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.7/PKG-INFO` & `meshtastic-2.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshtastic
-Version: 2.1.7
+Version: 2.1.8
 Summary: Python API & client shell for talking to Meshtastic devices
 Home-page: https://github.com/meshtastic/python
 Author: Meshtastic Developers
 Author-email: contact@meshtastic.org
 License: GPL-3.0-only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
```

### Comparing `meshtastic-2.1.7/README.md` & `meshtastic-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.7/meshtastic/__init__.py` & `meshtastic-2.1.8/meshtastic/__init__.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.7/meshtastic/__main__.py` & `meshtastic-2.1.8/meshtastic/__main__.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.7/meshtastic/admin_pb2.py` & `meshtastic-2.1.8/meshtastic/admin_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.7/meshtastic/apponly_pb2.py` & `meshtastic-2.1.8/meshtastic/apponly_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.7/meshtastic/ble_interface.py` & `meshtastic-2.1.8/meshtastic/ble_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.7/meshtastic/cannedmessages_pb2.py` & `meshtastic-2.1.8/meshtastic/cannedmessages_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.7/meshtastic/channel_pb2.py` & `meshtastic-2.1.8/meshtastic/channel_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.7/meshtastic/clientonly_pb2.py` & `meshtastic-2.1.8/meshtastic/clientonly_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.7/meshtastic/config_pb2.py` & `meshtastic-2.1.8/meshtastic/config_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17meshtastic/config.proto\"\x8e\x1b\n\x06\x43onfig\x12&\n\x06\x64\x65vice\x18\x01 \x01(\x0b\x32\x14.Config.DeviceConfigH\x00\x12*\n\x08position\x18\x02 \x01(\x0b\x32\x16.Config.PositionConfigH\x00\x12$\n\x05power\x18\x03 \x01(\x0b\x32\x13.Config.PowerConfigH\x00\x12(\n\x07network\x18\x04 \x01(\x0b\x32\x15.Config.NetworkConfigH\x00\x12(\n\x07\x64isplay\x18\x05 \x01(\x0b\x32\x15.Config.DisplayConfigH\x00\x12\"\n\x04lora\x18\x06 \x01(\x0b\x32\x12.Config.LoRaConfigH\x00\x12,\n\tbluetooth\x18\x07 \x01(\x0b\x32\x17.Config.BluetoothConfigH\x00\x1a\xdc\x03\n\x0c\x44\x65viceConfig\x12\'\n\x04role\x18\x01 \x01(\x0e\x32\x19.Config.DeviceConfig.Role\x12\x16\n\x0eserial_enabled\x18\x02 \x01(\x08\x12\x19\n\x11\x64\x65\x62ug_log_enabled\x18\x03 \x01(\x08\x12\x13\n\x0b\x62utton_gpio\x18\x04 \x01(\r\x12\x13\n\x0b\x62uzzer_gpio\x18\x05 \x01(\r\x12>\n\x10rebroadcast_mode\x18\x06 \x01(\x0e\x32$.Config.DeviceConfig.RebroadcastMode\x12 \n\x18node_info_broadcast_secs\x18\x07 \x01(\r\x12\"\n\x1a\x64ouble_tap_as_button_press\x18\x08 \x01(\x08\x12\x12\n\nis_managed\x18\t \x01(\x08\"i\n\x04Role\x12\n\n\x06\x43LIENT\x10\x00\x12\x0f\n\x0b\x43LIENT_MUTE\x10\x01\x12\n\n\x06ROUTER\x10\x02\x12\x11\n\rROUTER_CLIENT\x10\x03\x12\x0c\n\x08REPEATER\x10\x04\x12\x0b\n\x07TRACKER\x10\x05\x12\n\n\x06SENSOR\x10\x06\"A\n\x0fRebroadcastMode\x12\x07\n\x03\x41LL\x10\x00\x12\x15\n\x11\x41LL_SKIP_DECODING\x10\x01\x12\x0e\n\nLOCAL_ONLY\x10\x02\x1a\x80\x04\n\x0ePositionConfig\x12\x1f\n\x17position_broadcast_secs\x18\x01 \x01(\r\x12(\n position_broadcast_smart_enabled\x18\x02 \x01(\x08\x12\x16\n\x0e\x66ixed_position\x18\x03 \x01(\x08\x12\x13\n\x0bgps_enabled\x18\x04 \x01(\x08\x12\x1b\n\x13gps_update_interval\x18\x05 \x01(\r\x12\x18\n\x10gps_attempt_time\x18\x06 \x01(\r\x12\x16\n\x0eposition_flags\x18\x07 \x01(\r\x12\x0f\n\x07rx_gpio\x18\x08 \x01(\r\x12\x0f\n\x07tx_gpio\x18\t \x01(\r\x12(\n broadcast_smart_minimum_distance\x18\n \x01(\r\x12-\n%broadcast_smart_minimum_interval_secs\x18\x0b \x01(\r\"\xab\x01\n\rPositionFlags\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08\x41LTITUDE\x10\x01\x12\x10\n\x0c\x41LTITUDE_MSL\x10\x02\x12\x16\n\x12GEOIDAL_SEPARATION\x10\x04\x12\x07\n\x03\x44OP\x10\x08\x12\t\n\x05HVDOP\x10\x10\x12\r\n\tSATINVIEW\x10 \x12\n\n\x06SEQ_NO\x10@\x12\x0e\n\tTIMESTAMP\x10\x80\x01\x12\x0c\n\x07HEADING\x10\x80\x02\x12\n\n\x05SPEED\x10\x80\x04\x1a\xe5\x01\n\x0bPowerConfig\x12\x17\n\x0fis_power_saving\x18\x01 \x01(\x08\x12&\n\x1eon_battery_shutdown_after_secs\x18\x02 \x01(\r\x12\x1f\n\x17\x61\x64\x63_multiplier_override\x18\x03 \x01(\x02\x12\x1b\n\x13wait_bluetooth_secs\x18\x04 \x01(\r\x12\x1d\n\x15mesh_sds_timeout_secs\x18\x05 \x01(\r\x12\x10\n\x08sds_secs\x18\x06 \x01(\r\x12\x0f\n\x07ls_secs\x18\x07 \x01(\r\x12\x15\n\rmin_wake_secs\x18\x08 \x01(\r\x1a\xe8\x02\n\rNetworkConfig\x12\x14\n\x0cwifi_enabled\x18\x01 \x01(\x08\x12\x11\n\twifi_ssid\x18\x03 \x01(\t\x12\x10\n\x08wifi_psk\x18\x04 \x01(\t\x12\x12\n\nntp_server\x18\x05 \x01(\t\x12\x13\n\x0b\x65th_enabled\x18\x06 \x01(\x08\x12\x37\n\x0c\x61\x64\x64ress_mode\x18\x07 \x01(\x0e\x32!.Config.NetworkConfig.AddressMode\x12\x35\n\x0bipv4_config\x18\x08 \x01(\x0b\x32 .Config.NetworkConfig.IpV4Config\x12\x16\n\x0ersyslog_server\x18\t \x01(\t\x1a\x46\n\nIpV4Config\x12\n\n\x02ip\x18\x01 \x01(\x07\x12\x0f\n\x07gateway\x18\x02 \x01(\x07\x12\x0e\n\x06subnet\x18\x03 \x01(\x07\x12\x0b\n\x03\x64ns\x18\x04 \x01(\x07\"#\n\x0b\x41\x64\x64ressMode\x12\x08\n\x04\x44HCP\x10\x00\x12\n\n\x06STATIC\x10\x01\x1a\x92\x05\n\rDisplayConfig\x12\x16\n\x0escreen_on_secs\x18\x01 \x01(\r\x12=\n\ngps_format\x18\x02 \x01(\x0e\x32).Config.DisplayConfig.GpsCoordinateFormat\x12!\n\x19\x61uto_screen_carousel_secs\x18\x03 \x01(\r\x12\x19\n\x11\x63ompass_north_top\x18\x04 \x01(\x08\x12\x13\n\x0b\x66lip_screen\x18\x05 \x01(\x08\x12\x31\n\x05units\x18\x06 \x01(\x0e\x32\".Config.DisplayConfig.DisplayUnits\x12,\n\x04oled\x18\x07 \x01(\x0e\x32\x1e.Config.DisplayConfig.OledType\x12\x36\n\x0b\x64isplaymode\x18\x08 \x01(\x0e\x32!.Config.DisplayConfig.DisplayMode\x12\x14\n\x0cheading_bold\x18\t \x01(\x08\x12\x1d\n\x15wake_on_tap_or_motion\x18\n \x01(\x08\"M\n\x13GpsCoordinateFormat\x12\x07\n\x03\x44\x45\x43\x10\x00\x12\x07\n\x03\x44MS\x10\x01\x12\x07\n\x03UTM\x10\x02\x12\x08\n\x04MGRS\x10\x03\x12\x07\n\x03OLC\x10\x04\x12\x08\n\x04OSGR\x10\x05\"(\n\x0c\x44isplayUnits\x12\n\n\x06METRIC\x10\x00\x12\x0c\n\x08IMPERIAL\x10\x01\"M\n\x08OledType\x12\r\n\tOLED_AUTO\x10\x00\x12\x10\n\x0cOLED_SSD1306\x10\x01\x12\x0f\n\x0bOLED_SH1106\x10\x02\x12\x0f\n\x0bOLED_SH1107\x10\x03\"A\n\x0b\x44isplayMode\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\x0c\n\x08TWOCOLOR\x10\x01\x12\x0c\n\x08INVERTED\x10\x02\x12\t\n\x05\x43OLOR\x10\x03\x1a\xe1\x05\n\nLoRaConfig\x12\x12\n\nuse_preset\x18\x01 \x01(\x08\x12\x34\n\x0cmodem_preset\x18\x02 \x01(\x0e\x32\x1e.Config.LoRaConfig.ModemPreset\x12\x11\n\tbandwidth\x18\x03 \x01(\r\x12\x15\n\rspread_factor\x18\x04 \x01(\r\x12\x13\n\x0b\x63oding_rate\x18\x05 \x01(\r\x12\x18\n\x10\x66requency_offset\x18\x06 \x01(\x02\x12-\n\x06region\x18\x07 \x01(\x0e\x32\x1d.Config.LoRaConfig.RegionCode\x12\x11\n\thop_limit\x18\x08 \x01(\r\x12\x12\n\ntx_enabled\x18\t \x01(\x08\x12\x10\n\x08tx_power\x18\n \x01(\x05\x12\x13\n\x0b\x63hannel_num\x18\x0b \x01(\r\x12\x1b\n\x13override_duty_cycle\x18\x0c \x01(\x08\x12\x1e\n\x16sx126x_rx_boosted_gain\x18\r \x01(\x08\x12\x1a\n\x12override_frequency\x18\x0e \x01(\x02\x12\x17\n\x0fignore_incoming\x18g \x03(\r\"\xa9\x01\n\nRegionCode\x12\t\n\x05UNSET\x10\x00\x12\x06\n\x02US\x10\x01\x12\n\n\x06\x45U_433\x10\x02\x12\n\n\x06\x45U_868\x10\x03\x12\x06\n\x02\x43N\x10\x04\x12\x06\n\x02JP\x10\x05\x12\x07\n\x03\x41NZ\x10\x06\x12\x06\n\x02KR\x10\x07\x12\x06\n\x02TW\x10\x08\x12\x06\n\x02RU\x10\t\x12\x06\n\x02IN\x10\n\x12\n\n\x06NZ_865\x10\x0b\x12\x06\n\x02TH\x10\x0c\x12\x0b\n\x07LORA_24\x10\r\x12\n\n\x06UA_433\x10\x0e\x12\n\n\x06UA_868\x10\x0f\"\x94\x01\n\x0bModemPreset\x12\r\n\tLONG_FAST\x10\x00\x12\r\n\tLONG_SLOW\x10\x01\x12\x12\n\x0eVERY_LONG_SLOW\x10\x02\x12\x0f\n\x0bMEDIUM_SLOW\x10\x03\x12\x0f\n\x0bMEDIUM_FAST\x10\x04\x12\x0e\n\nSHORT_SLOW\x10\x05\x12\x0e\n\nSHORT_FAST\x10\x06\x12\x11\n\rLONG_MODERATE\x10\x07\x1a\xa2\x01\n\x0f\x42luetoothConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x31\n\x04mode\x18\x02 \x01(\x0e\x32#.Config.BluetoothConfig.PairingMode\x12\x11\n\tfixed_pin\x18\x03 \x01(\r\"8\n\x0bPairingMode\x12\x0e\n\nRANDOM_PIN\x10\x00\x12\r\n\tFIXED_PIN\x10\x01\x12\n\n\x06NO_PIN\x10\x02\x42\x11\n\x0fpayload_variantBa\n\x13\x63om.geeksville.meshB\x0c\x43onfigProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17meshtastic/config.proto\"\xb2\x1b\n\x06\x43onfig\x12&\n\x06\x64\x65vice\x18\x01 \x01(\x0b\x32\x14.Config.DeviceConfigH\x00\x12*\n\x08position\x18\x02 \x01(\x0b\x32\x16.Config.PositionConfigH\x00\x12$\n\x05power\x18\x03 \x01(\x0b\x32\x13.Config.PowerConfigH\x00\x12(\n\x07network\x18\x04 \x01(\x0b\x32\x15.Config.NetworkConfigH\x00\x12(\n\x07\x64isplay\x18\x05 \x01(\x0b\x32\x15.Config.DisplayConfigH\x00\x12\"\n\x04lora\x18\x06 \x01(\x0b\x32\x12.Config.LoRaConfigH\x00\x12,\n\tbluetooth\x18\x07 \x01(\x0b\x32\x17.Config.BluetoothConfigH\x00\x1a\xdc\x03\n\x0c\x44\x65viceConfig\x12\'\n\x04role\x18\x01 \x01(\x0e\x32\x19.Config.DeviceConfig.Role\x12\x16\n\x0eserial_enabled\x18\x02 \x01(\x08\x12\x19\n\x11\x64\x65\x62ug_log_enabled\x18\x03 \x01(\x08\x12\x13\n\x0b\x62utton_gpio\x18\x04 \x01(\r\x12\x13\n\x0b\x62uzzer_gpio\x18\x05 \x01(\r\x12>\n\x10rebroadcast_mode\x18\x06 \x01(\x0e\x32$.Config.DeviceConfig.RebroadcastMode\x12 \n\x18node_info_broadcast_secs\x18\x07 \x01(\r\x12\"\n\x1a\x64ouble_tap_as_button_press\x18\x08 \x01(\x08\x12\x12\n\nis_managed\x18\t \x01(\x08\"i\n\x04Role\x12\n\n\x06\x43LIENT\x10\x00\x12\x0f\n\x0b\x43LIENT_MUTE\x10\x01\x12\n\n\x06ROUTER\x10\x02\x12\x11\n\rROUTER_CLIENT\x10\x03\x12\x0c\n\x08REPEATER\x10\x04\x12\x0b\n\x07TRACKER\x10\x05\x12\n\n\x06SENSOR\x10\x06\"A\n\x0fRebroadcastMode\x12\x07\n\x03\x41LL\x10\x00\x12\x15\n\x11\x41LL_SKIP_DECODING\x10\x01\x12\x0e\n\nLOCAL_ONLY\x10\x02\x1a\x80\x04\n\x0ePositionConfig\x12\x1f\n\x17position_broadcast_secs\x18\x01 \x01(\r\x12(\n position_broadcast_smart_enabled\x18\x02 \x01(\x08\x12\x16\n\x0e\x66ixed_position\x18\x03 \x01(\x08\x12\x13\n\x0bgps_enabled\x18\x04 \x01(\x08\x12\x1b\n\x13gps_update_interval\x18\x05 \x01(\r\x12\x18\n\x10gps_attempt_time\x18\x06 \x01(\r\x12\x16\n\x0eposition_flags\x18\x07 \x01(\r\x12\x0f\n\x07rx_gpio\x18\x08 \x01(\r\x12\x0f\n\x07tx_gpio\x18\t \x01(\r\x12(\n broadcast_smart_minimum_distance\x18\n \x01(\r\x12-\n%broadcast_smart_minimum_interval_secs\x18\x0b \x01(\r\"\xab\x01\n\rPositionFlags\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08\x41LTITUDE\x10\x01\x12\x10\n\x0c\x41LTITUDE_MSL\x10\x02\x12\x16\n\x12GEOIDAL_SEPARATION\x10\x04\x12\x07\n\x03\x44OP\x10\x08\x12\t\n\x05HVDOP\x10\x10\x12\r\n\tSATINVIEW\x10 \x12\n\n\x06SEQ_NO\x10@\x12\x0e\n\tTIMESTAMP\x10\x80\x01\x12\x0c\n\x07HEADING\x10\x80\x02\x12\n\n\x05SPEED\x10\x80\x04\x1a\x89\x02\n\x0bPowerConfig\x12\x17\n\x0fis_power_saving\x18\x01 \x01(\x08\x12&\n\x1eon_battery_shutdown_after_secs\x18\x02 \x01(\r\x12\x1f\n\x17\x61\x64\x63_multiplier_override\x18\x03 \x01(\x02\x12\x1b\n\x13wait_bluetooth_secs\x18\x04 \x01(\r\x12\x1d\n\x15mesh_sds_timeout_secs\x18\x05 \x01(\r\x12\x10\n\x08sds_secs\x18\x06 \x01(\r\x12\x0f\n\x07ls_secs\x18\x07 \x01(\r\x12\x15\n\rmin_wake_secs\x18\x08 \x01(\r\x12\"\n\x1a\x64\x65vice_battery_ina_address\x18\t \x01(\r\x1a\xe8\x02\n\rNetworkConfig\x12\x14\n\x0cwifi_enabled\x18\x01 \x01(\x08\x12\x11\n\twifi_ssid\x18\x03 \x01(\t\x12\x10\n\x08wifi_psk\x18\x04 \x01(\t\x12\x12\n\nntp_server\x18\x05 \x01(\t\x12\x13\n\x0b\x65th_enabled\x18\x06 \x01(\x08\x12\x37\n\x0c\x61\x64\x64ress_mode\x18\x07 \x01(\x0e\x32!.Config.NetworkConfig.AddressMode\x12\x35\n\x0bipv4_config\x18\x08 \x01(\x0b\x32 .Config.NetworkConfig.IpV4Config\x12\x16\n\x0ersyslog_server\x18\t \x01(\t\x1a\x46\n\nIpV4Config\x12\n\n\x02ip\x18\x01 \x01(\x07\x12\x0f\n\x07gateway\x18\x02 \x01(\x07\x12\x0e\n\x06subnet\x18\x03 \x01(\x07\x12\x0b\n\x03\x64ns\x18\x04 \x01(\x07\"#\n\x0b\x41\x64\x64ressMode\x12\x08\n\x04\x44HCP\x10\x00\x12\n\n\x06STATIC\x10\x01\x1a\x92\x05\n\rDisplayConfig\x12\x16\n\x0escreen_on_secs\x18\x01 \x01(\r\x12=\n\ngps_format\x18\x02 \x01(\x0e\x32).Config.DisplayConfig.GpsCoordinateFormat\x12!\n\x19\x61uto_screen_carousel_secs\x18\x03 \x01(\r\x12\x19\n\x11\x63ompass_north_top\x18\x04 \x01(\x08\x12\x13\n\x0b\x66lip_screen\x18\x05 \x01(\x08\x12\x31\n\x05units\x18\x06 \x01(\x0e\x32\".Config.DisplayConfig.DisplayUnits\x12,\n\x04oled\x18\x07 \x01(\x0e\x32\x1e.Config.DisplayConfig.OledType\x12\x36\n\x0b\x64isplaymode\x18\x08 \x01(\x0e\x32!.Config.DisplayConfig.DisplayMode\x12\x14\n\x0cheading_bold\x18\t \x01(\x08\x12\x1d\n\x15wake_on_tap_or_motion\x18\n \x01(\x08\"M\n\x13GpsCoordinateFormat\x12\x07\n\x03\x44\x45\x43\x10\x00\x12\x07\n\x03\x44MS\x10\x01\x12\x07\n\x03UTM\x10\x02\x12\x08\n\x04MGRS\x10\x03\x12\x07\n\x03OLC\x10\x04\x12\x08\n\x04OSGR\x10\x05\"(\n\x0c\x44isplayUnits\x12\n\n\x06METRIC\x10\x00\x12\x0c\n\x08IMPERIAL\x10\x01\"M\n\x08OledType\x12\r\n\tOLED_AUTO\x10\x00\x12\x10\n\x0cOLED_SSD1306\x10\x01\x12\x0f\n\x0bOLED_SH1106\x10\x02\x12\x0f\n\x0bOLED_SH1107\x10\x03\"A\n\x0b\x44isplayMode\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\x0c\n\x08TWOCOLOR\x10\x01\x12\x0c\n\x08INVERTED\x10\x02\x12\t\n\x05\x43OLOR\x10\x03\x1a\xe1\x05\n\nLoRaConfig\x12\x12\n\nuse_preset\x18\x01 \x01(\x08\x12\x34\n\x0cmodem_preset\x18\x02 \x01(\x0e\x32\x1e.Config.LoRaConfig.ModemPreset\x12\x11\n\tbandwidth\x18\x03 \x01(\r\x12\x15\n\rspread_factor\x18\x04 \x01(\r\x12\x13\n\x0b\x63oding_rate\x18\x05 \x01(\r\x12\x18\n\x10\x66requency_offset\x18\x06 \x01(\x02\x12-\n\x06region\x18\x07 \x01(\x0e\x32\x1d.Config.LoRaConfig.RegionCode\x12\x11\n\thop_limit\x18\x08 \x01(\r\x12\x12\n\ntx_enabled\x18\t \x01(\x08\x12\x10\n\x08tx_power\x18\n \x01(\x05\x12\x13\n\x0b\x63hannel_num\x18\x0b \x01(\r\x12\x1b\n\x13override_duty_cycle\x18\x0c \x01(\x08\x12\x1e\n\x16sx126x_rx_boosted_gain\x18\r \x01(\x08\x12\x1a\n\x12override_frequency\x18\x0e \x01(\x02\x12\x17\n\x0fignore_incoming\x18g \x03(\r\"\xa9\x01\n\nRegionCode\x12\t\n\x05UNSET\x10\x00\x12\x06\n\x02US\x10\x01\x12\n\n\x06\x45U_433\x10\x02\x12\n\n\x06\x45U_868\x10\x03\x12\x06\n\x02\x43N\x10\x04\x12\x06\n\x02JP\x10\x05\x12\x07\n\x03\x41NZ\x10\x06\x12\x06\n\x02KR\x10\x07\x12\x06\n\x02TW\x10\x08\x12\x06\n\x02RU\x10\t\x12\x06\n\x02IN\x10\n\x12\n\n\x06NZ_865\x10\x0b\x12\x06\n\x02TH\x10\x0c\x12\x0b\n\x07LORA_24\x10\r\x12\n\n\x06UA_433\x10\x0e\x12\n\n\x06UA_868\x10\x0f\"\x94\x01\n\x0bModemPreset\x12\r\n\tLONG_FAST\x10\x00\x12\r\n\tLONG_SLOW\x10\x01\x12\x12\n\x0eVERY_LONG_SLOW\x10\x02\x12\x0f\n\x0bMEDIUM_SLOW\x10\x03\x12\x0f\n\x0bMEDIUM_FAST\x10\x04\x12\x0e\n\nSHORT_SLOW\x10\x05\x12\x0e\n\nSHORT_FAST\x10\x06\x12\x11\n\rLONG_MODERATE\x10\x07\x1a\xa2\x01\n\x0f\x42luetoothConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x31\n\x04mode\x18\x02 \x01(\x0e\x32#.Config.BluetoothConfig.PairingMode\x12\x11\n\tfixed_pin\x18\x03 \x01(\r\"8\n\x0bPairingMode\x12\x0e\n\nRANDOM_PIN\x10\x00\x12\r\n\tFIXED_PIN\x10\x01\x12\n\n\x06NO_PIN\x10\x02\x42\x11\n\x0fpayload_variantBa\n\x13\x63om.geeksville.meshB\x0c\x43onfigProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 
 
 _CONFIG = DESCRIPTOR.message_types_by_name['Config']
 _CONFIG_DEVICECONFIG = _CONFIG.nested_types_by_name['DeviceConfig']
 _CONFIG_POSITIONCONFIG = _CONFIG.nested_types_by_name['PositionConfig']
 _CONFIG_POWERCONFIG = _CONFIG.nested_types_by_name['PowerConfig']
@@ -110,47 +110,47 @@
 _sym_db.RegisterMessage(Config.BluetoothConfig)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\014ConfigProtosZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
   _CONFIG._serialized_start=28
-  _CONFIG._serialized_end=3498
+  _CONFIG._serialized_end=3534
   _CONFIG_DEVICECONFIG._serialized_start=327
   _CONFIG_DEVICECONFIG._serialized_end=803
   _CONFIG_DEVICECONFIG_ROLE._serialized_start=631
   _CONFIG_DEVICECONFIG_ROLE._serialized_end=736
   _CONFIG_DEVICECONFIG_REBROADCASTMODE._serialized_start=738
   _CONFIG_DEVICECONFIG_REBROADCASTMODE._serialized_end=803
   _CONFIG_POSITIONCONFIG._serialized_start=806
   _CONFIG_POSITIONCONFIG._serialized_end=1318
   _CONFIG_POSITIONCONFIG_POSITIONFLAGS._serialized_start=1147
   _CONFIG_POSITIONCONFIG_POSITIONFLAGS._serialized_end=1318
   _CONFIG_POWERCONFIG._serialized_start=1321
-  _CONFIG_POWERCONFIG._serialized_end=1550
-  _CONFIG_NETWORKCONFIG._serialized_start=1553
-  _CONFIG_NETWORKCONFIG._serialized_end=1913
-  _CONFIG_NETWORKCONFIG_IPV4CONFIG._serialized_start=1806
-  _CONFIG_NETWORKCONFIG_IPV4CONFIG._serialized_end=1876
-  _CONFIG_NETWORKCONFIG_ADDRESSMODE._serialized_start=1878
-  _CONFIG_NETWORKCONFIG_ADDRESSMODE._serialized_end=1913
-  _CONFIG_DISPLAYCONFIG._serialized_start=1916
-  _CONFIG_DISPLAYCONFIG._serialized_end=2574
-  _CONFIG_DISPLAYCONFIG_GPSCOORDINATEFORMAT._serialized_start=2309
-  _CONFIG_DISPLAYCONFIG_GPSCOORDINATEFORMAT._serialized_end=2386
-  _CONFIG_DISPLAYCONFIG_DISPLAYUNITS._serialized_start=2388
-  _CONFIG_DISPLAYCONFIG_DISPLAYUNITS._serialized_end=2428
-  _CONFIG_DISPLAYCONFIG_OLEDTYPE._serialized_start=2430
-  _CONFIG_DISPLAYCONFIG_OLEDTYPE._serialized_end=2507
-  _CONFIG_DISPLAYCONFIG_DISPLAYMODE._serialized_start=2509
-  _CONFIG_DISPLAYCONFIG_DISPLAYMODE._serialized_end=2574
-  _CONFIG_LORACONFIG._serialized_start=2577
-  _CONFIG_LORACONFIG._serialized_end=3314
-  _CONFIG_LORACONFIG_REGIONCODE._serialized_start=2994
-  _CONFIG_LORACONFIG_REGIONCODE._serialized_end=3163
-  _CONFIG_LORACONFIG_MODEMPRESET._serialized_start=3166
-  _CONFIG_LORACONFIG_MODEMPRESET._serialized_end=3314
-  _CONFIG_BLUETOOTHCONFIG._serialized_start=3317
-  _CONFIG_BLUETOOTHCONFIG._serialized_end=3479
-  _CONFIG_BLUETOOTHCONFIG_PAIRINGMODE._serialized_start=3423
-  _CONFIG_BLUETOOTHCONFIG_PAIRINGMODE._serialized_end=3479
+  _CONFIG_POWERCONFIG._serialized_end=1586
+  _CONFIG_NETWORKCONFIG._serialized_start=1589
+  _CONFIG_NETWORKCONFIG._serialized_end=1949
+  _CONFIG_NETWORKCONFIG_IPV4CONFIG._serialized_start=1842
+  _CONFIG_NETWORKCONFIG_IPV4CONFIG._serialized_end=1912
+  _CONFIG_NETWORKCONFIG_ADDRESSMODE._serialized_start=1914
+  _CONFIG_NETWORKCONFIG_ADDRESSMODE._serialized_end=1949
+  _CONFIG_DISPLAYCONFIG._serialized_start=1952
+  _CONFIG_DISPLAYCONFIG._serialized_end=2610
+  _CONFIG_DISPLAYCONFIG_GPSCOORDINATEFORMAT._serialized_start=2345
+  _CONFIG_DISPLAYCONFIG_GPSCOORDINATEFORMAT._serialized_end=2422
+  _CONFIG_DISPLAYCONFIG_DISPLAYUNITS._serialized_start=2424
+  _CONFIG_DISPLAYCONFIG_DISPLAYUNITS._serialized_end=2464
+  _CONFIG_DISPLAYCONFIG_OLEDTYPE._serialized_start=2466
+  _CONFIG_DISPLAYCONFIG_OLEDTYPE._serialized_end=2543
+  _CONFIG_DISPLAYCONFIG_DISPLAYMODE._serialized_start=2545
+  _CONFIG_DISPLAYCONFIG_DISPLAYMODE._serialized_end=2610
+  _CONFIG_LORACONFIG._serialized_start=2613
+  _CONFIG_LORACONFIG._serialized_end=3350
+  _CONFIG_LORACONFIG_REGIONCODE._serialized_start=3030
+  _CONFIG_LORACONFIG_REGIONCODE._serialized_end=3199
+  _CONFIG_LORACONFIG_MODEMPRESET._serialized_start=3202
+  _CONFIG_LORACONFIG_MODEMPRESET._serialized_end=3350
+  _CONFIG_BLUETOOTHCONFIG._serialized_start=3353
+  _CONFIG_BLUETOOTHCONFIG._serialized_end=3515
+  _CONFIG_BLUETOOTHCONFIG_PAIRINGMODE._serialized_start=3459
+  _CONFIG_BLUETOOTHCONFIG_PAIRINGMODE._serialized_end=3515
 # @@protoc_insertion_point(module_scope)
```

### Comparing `meshtastic-2.1.7/meshtastic/connection_status_pb2.py` & `meshtastic-2.1.8/meshtastic/connection_status_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.7/meshtastic/device_metadata_pb2.py` & `meshtastic-2.1.8/meshtastic/device_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.7/meshtastic/deviceonly_pb2.py` & `meshtastic-2.1.8/meshtastic/deviceonly_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.7/meshtastic/globals.py` & `meshtastic-2.1.8/meshtastic/globals.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.7/meshtastic/localonly_pb2.py` & `meshtastic-2.1.8/meshtastic/localonly_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.7/meshtastic/mesh_interface.py` & `meshtastic-2.1.8/meshtastic/mesh_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.7/meshtastic/mesh_pb2.py` & `meshtastic-2.1.8/meshtastic/mesh_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from meshtastic import config_pb2 as meshtastic_dot_config__pb2
 from meshtastic import module_config_pb2 as meshtastic_dot_module__config__pb2
 from meshtastic import portnums_pb2 as meshtastic_dot_portnums__pb2
 from meshtastic import telemetry_pb2 as meshtastic_dot_telemetry__pb2
 from meshtastic import xmodem_pb2 as meshtastic_dot_xmodem__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15meshtastic/mesh.proto\x1a\x18meshtastic/channel.proto\x1a\x17meshtastic/config.proto\x1a\x1emeshtastic/module_config.proto\x1a\x19meshtastic/portnums.proto\x1a\x1ameshtastic/telemetry.proto\x1a\x17meshtastic/xmodem.proto\"\xb7\x05\n\x08Position\x12\x12\n\nlatitude_i\x18\x01 \x01(\x0f\x12\x13\n\x0blongitude_i\x18\x02 \x01(\x0f\x12\x10\n\x08\x61ltitude\x18\x03 \x01(\x05\x12\x0c\n\x04time\x18\x04 \x01(\x07\x12,\n\x0flocation_source\x18\x05 \x01(\x0e\x32\x13.Position.LocSource\x12,\n\x0f\x61ltitude_source\x18\x06 \x01(\x0e\x32\x13.Position.AltSource\x12\x11\n\ttimestamp\x18\x07 \x01(\x07\x12\x1f\n\x17timestamp_millis_adjust\x18\x08 \x01(\x05\x12\x14\n\x0c\x61ltitude_hae\x18\t \x01(\x11\x12#\n\x1b\x61ltitude_geoidal_separation\x18\n \x01(\x11\x12\x0c\n\x04PDOP\x18\x0b \x01(\r\x12\x0c\n\x04HDOP\x18\x0c \x01(\r\x12\x0c\n\x04VDOP\x18\r \x01(\r\x12\x14\n\x0cgps_accuracy\x18\x0e \x01(\r\x12\x14\n\x0cground_speed\x18\x0f \x01(\r\x12\x14\n\x0cground_track\x18\x10 \x01(\r\x12\x13\n\x0b\x66ix_quality\x18\x11 \x01(\r\x12\x10\n\x08\x66ix_type\x18\x12 \x01(\r\x12\x14\n\x0csats_in_view\x18\x13 \x01(\r\x12\x11\n\tsensor_id\x18\x14 \x01(\r\x12\x13\n\x0bnext_update\x18\x15 \x01(\r\x12\x12\n\nseq_number\x18\x16 \x01(\r\"N\n\tLocSource\x12\r\n\tLOC_UNSET\x10\x00\x12\x0e\n\nLOC_MANUAL\x10\x01\x12\x10\n\x0cLOC_INTERNAL\x10\x02\x12\x10\n\x0cLOC_EXTERNAL\x10\x03\"b\n\tAltSource\x12\r\n\tALT_UNSET\x10\x00\x12\x0e\n\nALT_MANUAL\x10\x01\x12\x10\n\x0c\x41LT_INTERNAL\x10\x02\x12\x10\n\x0c\x41LT_EXTERNAL\x10\x03\x12\x12\n\x0e\x41LT_BAROMETRIC\x10\x04\"\x81\x01\n\x04User\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tlong_name\x18\x02 \x01(\t\x12\x12\n\nshort_name\x18\x03 \x01(\t\x12\x0f\n\x07macaddr\x18\x04 \x01(\x0c\x12 \n\x08hw_model\x18\x05 \x01(\x0e\x32\x0e.HardwareModel\x12\x13\n\x0bis_licensed\x18\x06 \x01(\x08\"\x1f\n\x0eRouteDiscovery\x12\r\n\x05route\x18\x01 \x03(\x07\"\xdb\x02\n\x07Routing\x12(\n\rroute_request\x18\x01 \x01(\x0b\x32\x0f.RouteDiscoveryH\x00\x12&\n\x0broute_reply\x18\x02 \x01(\x0b\x32\x0f.RouteDiscoveryH\x00\x12&\n\x0c\x65rror_reason\x18\x03 \x01(\x0e\x32\x0e.Routing.ErrorH\x00\"\xca\x01\n\x05\x45rror\x12\x08\n\x04NONE\x10\x00\x12\x0c\n\x08NO_ROUTE\x10\x01\x12\x0b\n\x07GOT_NAK\x10\x02\x12\x0b\n\x07TIMEOUT\x10\x03\x12\x10\n\x0cNO_INTERFACE\x10\x04\x12\x12\n\x0eMAX_RETRANSMIT\x10\x05\x12\x0e\n\nNO_CHANNEL\x10\x06\x12\r\n\tTOO_LARGE\x10\x07\x12\x0f\n\x0bNO_RESPONSE\x10\x08\x12\x14\n\x10\x44UTY_CYCLE_LIMIT\x10\t\x12\x0f\n\x0b\x42\x41\x44_REQUEST\x10 \x12\x12\n\x0eNOT_AUTHORIZED\x10!B\t\n\x07variant\"\x9c\x01\n\x04\x44\x61ta\x12\x19\n\x07portnum\x18\x01 \x01(\x0e\x32\x08.PortNum\x12\x0f\n\x07payload\x18\x02 \x01(\x0c\x12\x15\n\rwant_response\x18\x03 \x01(\x08\x12\x0c\n\x04\x64\x65st\x18\x04 \x01(\x07\x12\x0e\n\x06source\x18\x05 \x01(\x07\x12\x12\n\nrequest_id\x18\x06 \x01(\x07\x12\x10\n\x08reply_id\x18\x07 \x01(\x07\x12\r\n\x05\x65moji\x18\x08 \x01(\x07\"\x93\x01\n\x08Waypoint\x12\n\n\x02id\x18\x01 \x01(\r\x12\x12\n\nlatitude_i\x18\x02 \x01(\x0f\x12\x13\n\x0blongitude_i\x18\x03 \x01(\x0f\x12\x0e\n\x06\x65xpire\x18\x04 \x01(\r\x12\x11\n\tlocked_to\x18\x05 \x01(\r\x12\x0c\n\x04name\x18\x06 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12\x0c\n\x04icon\x18\x08 \x01(\x07\"\xcb\x03\n\nMeshPacket\x12\x0c\n\x04\x66rom\x18\x01 \x01(\x07\x12\n\n\x02to\x18\x02 \x01(\x07\x12\x0f\n\x07\x63hannel\x18\x03 \x01(\r\x12\x18\n\x07\x64\x65\x63oded\x18\x04 \x01(\x0b\x32\x05.DataH\x00\x12\x13\n\tencrypted\x18\x05 \x01(\x0cH\x00\x12\n\n\x02id\x18\x06 \x01(\x07\x12\x0f\n\x07rx_time\x18\x07 \x01(\x07\x12\x0e\n\x06rx_snr\x18\x08 \x01(\x02\x12\x11\n\thop_limit\x18\t \x01(\r\x12\x10\n\x08want_ack\x18\n \x01(\x08\x12&\n\x08priority\x18\x0b \x01(\x0e\x32\x14.MeshPacket.Priority\x12\x0f\n\x07rx_rssi\x18\x0c \x01(\x05\x12$\n\x07\x64\x65layed\x18\r \x01(\x0e\x32\x13.MeshPacket.Delayed\"[\n\x08Priority\x12\t\n\x05UNSET\x10\x00\x12\x07\n\x03MIN\x10\x01\x12\x0e\n\nBACKGROUND\x10\n\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10@\x12\x0c\n\x08RELIABLE\x10\x46\x12\x07\n\x03\x41\x43K\x10x\x12\x07\n\x03MAX\x10\x7f\"B\n\x07\x44\x65layed\x12\x0c\n\x08NO_DELAY\x10\x00\x12\x15\n\x11\x44\x45LAYED_BROADCAST\x10\x01\x12\x12\n\x0e\x44\x45LAYED_DIRECT\x10\x02\x42\x11\n\x0fpayload_variant\"\xa3\x01\n\x08NodeInfo\x12\x0b\n\x03num\x18\x01 \x01(\r\x12\x13\n\x04user\x18\x02 \x01(\x0b\x32\x05.User\x12\x1b\n\x08position\x18\x03 \x01(\x0b\x32\t.Position\x12\x0b\n\x03snr\x18\x04 \x01(\x02\x12\x12\n\nlast_heard\x18\x05 \x01(\x07\x12&\n\x0e\x64\x65vice_metrics\x18\x06 \x01(\x0b\x32\x0e.DeviceMetrics\x12\x0f\n\x07\x63hannel\x18\x07 \x01(\r\"\x86\x03\n\nMyNodeInfo\x12\x13\n\x0bmy_node_num\x18\x01 \x01(\r\x12\x0f\n\x07has_gps\x18\x02 \x01(\x08\x12\x14\n\x0cmax_channels\x18\x03 \x01(\r\x12\x18\n\x10\x66irmware_version\x18\x04 \x01(\t\x12&\n\nerror_code\x18\x05 \x01(\x0e\x32\x12.CriticalErrorCode\x12\x15\n\rerror_address\x18\x06 \x01(\r\x12\x13\n\x0b\x65rror_count\x18\x07 \x01(\r\x12\x14\n\x0creboot_count\x18\x08 \x01(\r\x12\x0f\n\x07\x62itrate\x18\t \x01(\x02\x12\x1c\n\x14message_timeout_msec\x18\n \x01(\r\x12\x17\n\x0fmin_app_version\x18\x0b \x01(\r\x12\x15\n\rair_period_tx\x18\x0c \x03(\r\x12\x15\n\rair_period_rx\x18\r \x03(\r\x12\x10\n\x08has_wifi\x18\x0e \x01(\x08\x12\x1b\n\x13\x63hannel_utilization\x18\x0f \x01(\x02\x12\x13\n\x0b\x61ir_util_tx\x18\x10 \x01(\x02\"\xb5\x01\n\tLogRecord\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x0c\n\x04time\x18\x02 \x01(\x07\x12\x0e\n\x06source\x18\x03 \x01(\t\x12\x1f\n\x05level\x18\x04 \x01(\x0e\x32\x10.LogRecord.Level\"X\n\x05Level\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08\x43RITICAL\x10\x32\x12\t\n\x05\x45RROR\x10(\x12\x0b\n\x07WARNING\x10\x1e\x12\x08\n\x04INFO\x10\x14\x12\t\n\x05\x44\x45\x42UG\x10\n\x12\t\n\x05TRACE\x10\x05\"P\n\x0bQueueStatus\x12\x0b\n\x03res\x18\x01 \x01(\x05\x12\x0c\n\x04\x66ree\x18\x02 \x01(\r\x12\x0e\n\x06maxlen\x18\x03 \x01(\r\x12\x16\n\x0emesh_packet_id\x18\x04 \x01(\r\"\xa7\x03\n\tFromRadio\x12\n\n\x02id\x18\x01 \x01(\r\x12\x1d\n\x06packet\x18\x02 \x01(\x0b\x32\x0b.MeshPacketH\x00\x12\x1e\n\x07my_info\x18\x03 \x01(\x0b\x32\x0b.MyNodeInfoH\x00\x12\x1e\n\tnode_info\x18\x04 \x01(\x0b\x32\t.NodeInfoH\x00\x12\x19\n\x06\x63onfig\x18\x05 \x01(\x0b\x32\x07.ConfigH\x00\x12 \n\nlog_record\x18\x06 \x01(\x0b\x32\n.LogRecordH\x00\x12\x1c\n\x12\x63onfig_complete_id\x18\x07 \x01(\rH\x00\x12\x12\n\x08rebooted\x18\x08 \x01(\x08H\x00\x12%\n\x0cmoduleConfig\x18\t \x01(\x0b\x32\r.ModuleConfigH\x00\x12\x1b\n\x07\x63hannel\x18\n \x01(\x0b\x32\x08.ChannelH\x00\x12#\n\x0bqueueStatus\x18\x0b \x01(\x0b\x32\x0c.QueueStatusH\x00\x12\x1f\n\x0cxmodemPacket\x18\x0c \x01(\x0b\x32\x07.XModemH\x00\x12#\n\x08metadata\x18\r \x01(\x0b\x32\x0f.DeviceMetadataH\x00\x42\x11\n\x0fpayload_variant\"\x8c\x01\n\x07ToRadio\x12\x1d\n\x06packet\x18\x01 \x01(\x0b\x32\x0b.MeshPacketH\x00\x12\x18\n\x0ewant_config_id\x18\x03 \x01(\rH\x00\x12\x14\n\ndisconnect\x18\x04 \x01(\x08H\x00\x12\x1f\n\x0cxmodemPacket\x18\x05 \x01(\x0b\x32\x07.XModemH\x00\x42\x11\n\x0fpayload_variant\"5\n\nCompressed\x12\x19\n\x07portnum\x18\x01 \x01(\x0e\x32\x08.PortNum\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"V\n\x0cNeighborInfo\x12\x0f\n\x07node_id\x18\x01 \x01(\r\x12\x17\n\x0flast_sent_by_id\x18\x02 \x01(\r\x12\x1c\n\tneighbors\x18\x03 \x03(\x0b\x32\t.Neighbor\"(\n\x08Neighbor\x12\x0f\n\x07node_id\x18\x01 \x01(\r\x12\x0b\n\x03snr\x18\x02 \x01(\x02\"\x97\x02\n\x0e\x44\x65viceMetadata\x12\x18\n\x10\x66irmware_version\x18\x01 \x01(\t\x12\x1c\n\x14\x64\x65vice_state_version\x18\x02 \x01(\r\x12\x13\n\x0b\x63\x61nShutdown\x18\x03 \x01(\x08\x12\x0f\n\x07hasWifi\x18\x04 \x01(\x08\x12\x14\n\x0chasBluetooth\x18\x05 \x01(\x08\x12\x13\n\x0bhasEthernet\x18\x06 \x01(\x08\x12\'\n\x04role\x18\x07 \x01(\x0e\x32\x19.Config.DeviceConfig.Role\x12\x16\n\x0eposition_flags\x18\x08 \x01(\r\x12 \n\x08hw_model\x18\t \x01(\x0e\x32\x0e.HardwareModel\x12\x19\n\x11hasRemoteHardware\x18\n \x01(\x08*\xce\x04\n\rHardwareModel\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08TLORA_V2\x10\x01\x12\x0c\n\x08TLORA_V1\x10\x02\x12\x12\n\x0eTLORA_V2_1_1P6\x10\x03\x12\t\n\x05TBEAM\x10\x04\x12\x0f\n\x0bHELTEC_V2_0\x10\x05\x12\x0e\n\nTBEAM_V0P7\x10\x06\x12\n\n\x06T_ECHO\x10\x07\x12\x10\n\x0cTLORA_V1_1P3\x10\x08\x12\x0b\n\x07RAK4631\x10\t\x12\x0f\n\x0bHELTEC_V2_1\x10\n\x12\r\n\tHELTEC_V1\x10\x0b\x12\x18\n\x14LILYGO_TBEAM_S3_CORE\x10\x0c\x12\x0c\n\x08RAK11200\x10\r\x12\x0b\n\x07NANO_G1\x10\x0e\x12\x12\n\x0eTLORA_V2_1_1P8\x10\x0f\x12\x0f\n\x0bTLORA_T3_S3\x10\x10\x12\x14\n\x10NANO_G1_EXPLORER\x10\x11\x12\x0e\n\nSTATION_G1\x10\x19\x12\x11\n\rLORA_RELAY_V1\x10 \x12\x0e\n\nNRF52840DK\x10!\x12\x07\n\x03PPR\x10\"\x12\x0f\n\x0bGENIEBLOCKS\x10#\x12\x11\n\rNRF52_UNKNOWN\x10$\x12\r\n\tPORTDUINO\x10%\x12\x0f\n\x0b\x41NDROID_SIM\x10&\x12\n\n\x06\x44IY_V1\x10\'\x12\x15\n\x11NRF52840_PCA10059\x10(\x12\n\n\x06\x44R_DEV\x10)\x12\x0b\n\x07M5STACK\x10*\x12\r\n\tHELTEC_V3\x10+\x12\x11\n\rHELTEC_WSL_V3\x10,\x12\x13\n\x0f\x42\x45TAFPV_2400_TX\x10-\x12\x17\n\x13\x42\x45TAFPV_900_NANO_TX\x10.\x12\x0f\n\nPRIVATE_HW\x10\xff\x01*,\n\tConstants\x12\x08\n\x04ZERO\x10\x00\x12\x15\n\x10\x44\x41TA_PAYLOAD_LEN\x10\xed\x01*\xee\x01\n\x11\x43riticalErrorCode\x12\x08\n\x04NONE\x10\x00\x12\x0f\n\x0bTX_WATCHDOG\x10\x01\x12\x14\n\x10SLEEP_ENTER_WAIT\x10\x02\x12\x0c\n\x08NO_RADIO\x10\x03\x12\x0f\n\x0bUNSPECIFIED\x10\x04\x12\x15\n\x11UBLOX_UNIT_FAILED\x10\x05\x12\r\n\tNO_AXP192\x10\x06\x12\x19\n\x15INVALID_RADIO_SETTING\x10\x07\x12\x13\n\x0fTRANSMIT_FAILED\x10\x08\x12\x0c\n\x08\x42ROWNOUT\x10\t\x12\x12\n\x0eSX1262_FAILURE\x10\n\x12\x11\n\rRADIO_SPI_BUG\x10\x0b\x42_\n\x13\x63om.geeksville.meshB\nMeshProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15meshtastic/mesh.proto\x1a\x18meshtastic/channel.proto\x1a\x17meshtastic/config.proto\x1a\x1emeshtastic/module_config.proto\x1a\x19meshtastic/portnums.proto\x1a\x1ameshtastic/telemetry.proto\x1a\x17meshtastic/xmodem.proto\"\xb7\x05\n\x08Position\x12\x12\n\nlatitude_i\x18\x01 \x01(\x0f\x12\x13\n\x0blongitude_i\x18\x02 \x01(\x0f\x12\x10\n\x08\x61ltitude\x18\x03 \x01(\x05\x12\x0c\n\x04time\x18\x04 \x01(\x07\x12,\n\x0flocation_source\x18\x05 \x01(\x0e\x32\x13.Position.LocSource\x12,\n\x0f\x61ltitude_source\x18\x06 \x01(\x0e\x32\x13.Position.AltSource\x12\x11\n\ttimestamp\x18\x07 \x01(\x07\x12\x1f\n\x17timestamp_millis_adjust\x18\x08 \x01(\x05\x12\x14\n\x0c\x61ltitude_hae\x18\t \x01(\x11\x12#\n\x1b\x61ltitude_geoidal_separation\x18\n \x01(\x11\x12\x0c\n\x04PDOP\x18\x0b \x01(\r\x12\x0c\n\x04HDOP\x18\x0c \x01(\r\x12\x0c\n\x04VDOP\x18\r \x01(\r\x12\x14\n\x0cgps_accuracy\x18\x0e \x01(\r\x12\x14\n\x0cground_speed\x18\x0f \x01(\r\x12\x14\n\x0cground_track\x18\x10 \x01(\r\x12\x13\n\x0b\x66ix_quality\x18\x11 \x01(\r\x12\x10\n\x08\x66ix_type\x18\x12 \x01(\r\x12\x14\n\x0csats_in_view\x18\x13 \x01(\r\x12\x11\n\tsensor_id\x18\x14 \x01(\r\x12\x13\n\x0bnext_update\x18\x15 \x01(\r\x12\x12\n\nseq_number\x18\x16 \x01(\r\"N\n\tLocSource\x12\r\n\tLOC_UNSET\x10\x00\x12\x0e\n\nLOC_MANUAL\x10\x01\x12\x10\n\x0cLOC_INTERNAL\x10\x02\x12\x10\n\x0cLOC_EXTERNAL\x10\x03\"b\n\tAltSource\x12\r\n\tALT_UNSET\x10\x00\x12\x0e\n\nALT_MANUAL\x10\x01\x12\x10\n\x0c\x41LT_INTERNAL\x10\x02\x12\x10\n\x0c\x41LT_EXTERNAL\x10\x03\x12\x12\n\x0e\x41LT_BAROMETRIC\x10\x04\"\x81\x01\n\x04User\x12\n\n\x02id\x18\x01 \x01(\t\x12\x11\n\tlong_name\x18\x02 \x01(\t\x12\x12\n\nshort_name\x18\x03 \x01(\t\x12\x0f\n\x07macaddr\x18\x04 \x01(\x0c\x12 \n\x08hw_model\x18\x05 \x01(\x0e\x32\x0e.HardwareModel\x12\x13\n\x0bis_licensed\x18\x06 \x01(\x08\"\x1f\n\x0eRouteDiscovery\x12\r\n\x05route\x18\x01 \x03(\x07\"\xdb\x02\n\x07Routing\x12(\n\rroute_request\x18\x01 \x01(\x0b\x32\x0f.RouteDiscoveryH\x00\x12&\n\x0broute_reply\x18\x02 \x01(\x0b\x32\x0f.RouteDiscoveryH\x00\x12&\n\x0c\x65rror_reason\x18\x03 \x01(\x0e\x32\x0e.Routing.ErrorH\x00\"\xca\x01\n\x05\x45rror\x12\x08\n\x04NONE\x10\x00\x12\x0c\n\x08NO_ROUTE\x10\x01\x12\x0b\n\x07GOT_NAK\x10\x02\x12\x0b\n\x07TIMEOUT\x10\x03\x12\x10\n\x0cNO_INTERFACE\x10\x04\x12\x12\n\x0eMAX_RETRANSMIT\x10\x05\x12\x0e\n\nNO_CHANNEL\x10\x06\x12\r\n\tTOO_LARGE\x10\x07\x12\x0f\n\x0bNO_RESPONSE\x10\x08\x12\x14\n\x10\x44UTY_CYCLE_LIMIT\x10\t\x12\x0f\n\x0b\x42\x41\x44_REQUEST\x10 \x12\x12\n\x0eNOT_AUTHORIZED\x10!B\t\n\x07variant\"\x9c\x01\n\x04\x44\x61ta\x12\x19\n\x07portnum\x18\x01 \x01(\x0e\x32\x08.PortNum\x12\x0f\n\x07payload\x18\x02 \x01(\x0c\x12\x15\n\rwant_response\x18\x03 \x01(\x08\x12\x0c\n\x04\x64\x65st\x18\x04 \x01(\x07\x12\x0e\n\x06source\x18\x05 \x01(\x07\x12\x12\n\nrequest_id\x18\x06 \x01(\x07\x12\x10\n\x08reply_id\x18\x07 \x01(\x07\x12\r\n\x05\x65moji\x18\x08 \x01(\x07\"\x93\x01\n\x08Waypoint\x12\n\n\x02id\x18\x01 \x01(\r\x12\x12\n\nlatitude_i\x18\x02 \x01(\x0f\x12\x13\n\x0blongitude_i\x18\x03 \x01(\x0f\x12\x0e\n\x06\x65xpire\x18\x04 \x01(\r\x12\x11\n\tlocked_to\x18\x05 \x01(\r\x12\x0c\n\x04name\x18\x06 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x07 \x01(\t\x12\x0c\n\x04icon\x18\x08 \x01(\x07\"\xcb\x03\n\nMeshPacket\x12\x0c\n\x04\x66rom\x18\x01 \x01(\x07\x12\n\n\x02to\x18\x02 \x01(\x07\x12\x0f\n\x07\x63hannel\x18\x03 \x01(\r\x12\x18\n\x07\x64\x65\x63oded\x18\x04 \x01(\x0b\x32\x05.DataH\x00\x12\x13\n\tencrypted\x18\x05 \x01(\x0cH\x00\x12\n\n\x02id\x18\x06 \x01(\x07\x12\x0f\n\x07rx_time\x18\x07 \x01(\x07\x12\x0e\n\x06rx_snr\x18\x08 \x01(\x02\x12\x11\n\thop_limit\x18\t \x01(\r\x12\x10\n\x08want_ack\x18\n \x01(\x08\x12&\n\x08priority\x18\x0b \x01(\x0e\x32\x14.MeshPacket.Priority\x12\x0f\n\x07rx_rssi\x18\x0c \x01(\x05\x12$\n\x07\x64\x65layed\x18\r \x01(\x0e\x32\x13.MeshPacket.Delayed\"[\n\x08Priority\x12\t\n\x05UNSET\x10\x00\x12\x07\n\x03MIN\x10\x01\x12\x0e\n\nBACKGROUND\x10\n\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10@\x12\x0c\n\x08RELIABLE\x10\x46\x12\x07\n\x03\x41\x43K\x10x\x12\x07\n\x03MAX\x10\x7f\"B\n\x07\x44\x65layed\x12\x0c\n\x08NO_DELAY\x10\x00\x12\x15\n\x11\x44\x45LAYED_BROADCAST\x10\x01\x12\x12\n\x0e\x44\x45LAYED_DIRECT\x10\x02\x42\x11\n\x0fpayload_variant\"\xa3\x01\n\x08NodeInfo\x12\x0b\n\x03num\x18\x01 \x01(\r\x12\x13\n\x04user\x18\x02 \x01(\x0b\x32\x05.User\x12\x1b\n\x08position\x18\x03 \x01(\x0b\x32\t.Position\x12\x0b\n\x03snr\x18\x04 \x01(\x02\x12\x12\n\nlast_heard\x18\x05 \x01(\x07\x12&\n\x0e\x64\x65vice_metrics\x18\x06 \x01(\x0b\x32\x0e.DeviceMetrics\x12\x0f\n\x07\x63hannel\x18\x07 \x01(\r\"\x86\x03\n\nMyNodeInfo\x12\x13\n\x0bmy_node_num\x18\x01 \x01(\r\x12\x0f\n\x07has_gps\x18\x02 \x01(\x08\x12\x14\n\x0cmax_channels\x18\x03 \x01(\r\x12\x18\n\x10\x66irmware_version\x18\x04 \x01(\t\x12&\n\nerror_code\x18\x05 \x01(\x0e\x32\x12.CriticalErrorCode\x12\x15\n\rerror_address\x18\x06 \x01(\r\x12\x13\n\x0b\x65rror_count\x18\x07 \x01(\r\x12\x14\n\x0creboot_count\x18\x08 \x01(\r\x12\x0f\n\x07\x62itrate\x18\t \x01(\x02\x12\x1c\n\x14message_timeout_msec\x18\n \x01(\r\x12\x17\n\x0fmin_app_version\x18\x0b \x01(\r\x12\x15\n\rair_period_tx\x18\x0c \x03(\r\x12\x15\n\rair_period_rx\x18\r \x03(\r\x12\x10\n\x08has_wifi\x18\x0e \x01(\x08\x12\x1b\n\x13\x63hannel_utilization\x18\x0f \x01(\x02\x12\x13\n\x0b\x61ir_util_tx\x18\x10 \x01(\x02\"\xb5\x01\n\tLogRecord\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x0c\n\x04time\x18\x02 \x01(\x07\x12\x0e\n\x06source\x18\x03 \x01(\t\x12\x1f\n\x05level\x18\x04 \x01(\x0e\x32\x10.LogRecord.Level\"X\n\x05Level\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08\x43RITICAL\x10\x32\x12\t\n\x05\x45RROR\x10(\x12\x0b\n\x07WARNING\x10\x1e\x12\x08\n\x04INFO\x10\x14\x12\t\n\x05\x44\x45\x42UG\x10\n\x12\t\n\x05TRACE\x10\x05\"P\n\x0bQueueStatus\x12\x0b\n\x03res\x18\x01 \x01(\x05\x12\x0c\n\x04\x66ree\x18\x02 \x01(\r\x12\x0e\n\x06maxlen\x18\x03 \x01(\r\x12\x16\n\x0emesh_packet_id\x18\x04 \x01(\r\"\xa7\x03\n\tFromRadio\x12\n\n\x02id\x18\x01 \x01(\r\x12\x1d\n\x06packet\x18\x02 \x01(\x0b\x32\x0b.MeshPacketH\x00\x12\x1e\n\x07my_info\x18\x03 \x01(\x0b\x32\x0b.MyNodeInfoH\x00\x12\x1e\n\tnode_info\x18\x04 \x01(\x0b\x32\t.NodeInfoH\x00\x12\x19\n\x06\x63onfig\x18\x05 \x01(\x0b\x32\x07.ConfigH\x00\x12 \n\nlog_record\x18\x06 \x01(\x0b\x32\n.LogRecordH\x00\x12\x1c\n\x12\x63onfig_complete_id\x18\x07 \x01(\rH\x00\x12\x12\n\x08rebooted\x18\x08 \x01(\x08H\x00\x12%\n\x0cmoduleConfig\x18\t \x01(\x0b\x32\r.ModuleConfigH\x00\x12\x1b\n\x07\x63hannel\x18\n \x01(\x0b\x32\x08.ChannelH\x00\x12#\n\x0bqueueStatus\x18\x0b \x01(\x0b\x32\x0c.QueueStatusH\x00\x12\x1f\n\x0cxmodemPacket\x18\x0c \x01(\x0b\x32\x07.XModemH\x00\x12#\n\x08metadata\x18\r \x01(\x0b\x32\x0f.DeviceMetadataH\x00\x42\x11\n\x0fpayload_variant\"\x8c\x01\n\x07ToRadio\x12\x1d\n\x06packet\x18\x01 \x01(\x0b\x32\x0b.MeshPacketH\x00\x12\x18\n\x0ewant_config_id\x18\x03 \x01(\rH\x00\x12\x14\n\ndisconnect\x18\x04 \x01(\x08H\x00\x12\x1f\n\x0cxmodemPacket\x18\x05 \x01(\x0b\x32\x07.XModemH\x00\x42\x11\n\x0fpayload_variant\"5\n\nCompressed\x12\x19\n\x07portnum\x18\x01 \x01(\x0e\x32\x08.PortNum\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\"V\n\x0cNeighborInfo\x12\x0f\n\x07node_id\x18\x01 \x01(\r\x12\x17\n\x0flast_sent_by_id\x18\x02 \x01(\r\x12\x1c\n\tneighbors\x18\x03 \x03(\x0b\x32\t.Neighbor\"(\n\x08Neighbor\x12\x0f\n\x07node_id\x18\x01 \x01(\r\x12\x0b\n\x03snr\x18\x02 \x01(\x02\"\x97\x02\n\x0e\x44\x65viceMetadata\x12\x18\n\x10\x66irmware_version\x18\x01 \x01(\t\x12\x1c\n\x14\x64\x65vice_state_version\x18\x02 \x01(\r\x12\x13\n\x0b\x63\x61nShutdown\x18\x03 \x01(\x08\x12\x0f\n\x07hasWifi\x18\x04 \x01(\x08\x12\x14\n\x0chasBluetooth\x18\x05 \x01(\x08\x12\x13\n\x0bhasEthernet\x18\x06 \x01(\x08\x12\'\n\x04role\x18\x07 \x01(\x0e\x32\x19.Config.DeviceConfig.Role\x12\x16\n\x0eposition_flags\x18\x08 \x01(\r\x12 \n\x08hw_model\x18\t \x01(\x0e\x32\x0e.HardwareModel\x12\x19\n\x11hasRemoteHardware\x18\n \x01(\x08*\xea\x04\n\rHardwareModel\x12\t\n\x05UNSET\x10\x00\x12\x0c\n\x08TLORA_V2\x10\x01\x12\x0c\n\x08TLORA_V1\x10\x02\x12\x12\n\x0eTLORA_V2_1_1P6\x10\x03\x12\t\n\x05TBEAM\x10\x04\x12\x0f\n\x0bHELTEC_V2_0\x10\x05\x12\x0e\n\nTBEAM_V0P7\x10\x06\x12\n\n\x06T_ECHO\x10\x07\x12\x10\n\x0cTLORA_V1_1P3\x10\x08\x12\x0b\n\x07RAK4631\x10\t\x12\x0f\n\x0bHELTEC_V2_1\x10\n\x12\r\n\tHELTEC_V1\x10\x0b\x12\x18\n\x14LILYGO_TBEAM_S3_CORE\x10\x0c\x12\x0c\n\x08RAK11200\x10\r\x12\x0b\n\x07NANO_G1\x10\x0e\x12\x12\n\x0eTLORA_V2_1_1P8\x10\x0f\x12\x0f\n\x0bTLORA_T3_S3\x10\x10\x12\x14\n\x10NANO_G1_EXPLORER\x10\x11\x12\x0e\n\nSTATION_G1\x10\x19\x12\x0c\n\x08RAK11310\x10\x1a\x12\x11\n\rLORA_RELAY_V1\x10 \x12\x0e\n\nNRF52840DK\x10!\x12\x07\n\x03PPR\x10\"\x12\x0f\n\x0bGENIEBLOCKS\x10#\x12\x11\n\rNRF52_UNKNOWN\x10$\x12\r\n\tPORTDUINO\x10%\x12\x0f\n\x0b\x41NDROID_SIM\x10&\x12\n\n\x06\x44IY_V1\x10\'\x12\x15\n\x11NRF52840_PCA10059\x10(\x12\n\n\x06\x44R_DEV\x10)\x12\x0b\n\x07M5STACK\x10*\x12\r\n\tHELTEC_V3\x10+\x12\x11\n\rHELTEC_WSL_V3\x10,\x12\x13\n\x0f\x42\x45TAFPV_2400_TX\x10-\x12\x17\n\x13\x42\x45TAFPV_900_NANO_TX\x10.\x12\x0c\n\x08RPI_PICO\x10/\x12\x0f\n\nPRIVATE_HW\x10\xff\x01*,\n\tConstants\x12\x08\n\x04ZERO\x10\x00\x12\x15\n\x10\x44\x41TA_PAYLOAD_LEN\x10\xed\x01*\xee\x01\n\x11\x43riticalErrorCode\x12\x08\n\x04NONE\x10\x00\x12\x0f\n\x0bTX_WATCHDOG\x10\x01\x12\x14\n\x10SLEEP_ENTER_WAIT\x10\x02\x12\x0c\n\x08NO_RADIO\x10\x03\x12\x0f\n\x0bUNSPECIFIED\x10\x04\x12\x15\n\x11UBLOX_UNIT_FAILED\x10\x05\x12\r\n\tNO_AXP192\x10\x06\x12\x19\n\x15INVALID_RADIO_SETTING\x10\x07\x12\x13\n\x0fTRANSMIT_FAILED\x10\x08\x12\x0c\n\x08\x42ROWNOUT\x10\t\x12\x12\n\x0eSX1262_FAILURE\x10\n\x12\x11\n\rRADIO_SPI_BUG\x10\x0b\x42_\n\x13\x63om.geeksville.meshB\nMeshProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 _HARDWAREMODEL = DESCRIPTOR.enum_types_by_name['HardwareModel']
 HardwareModel = enum_type_wrapper.EnumTypeWrapper(_HARDWAREMODEL)
 _CONSTANTS = DESCRIPTOR.enum_types_by_name['Constants']
 Constants = enum_type_wrapper.EnumTypeWrapper(_CONSTANTS)
 _CRITICALERRORCODE = DESCRIPTOR.enum_types_by_name['CriticalErrorCode']
 CriticalErrorCode = enum_type_wrapper.EnumTypeWrapper(_CRITICALERRORCODE)
@@ -44,14 +44,15 @@
 LILYGO_TBEAM_S3_CORE = 12
 RAK11200 = 13
 NANO_G1 = 14
 TLORA_V2_1_1P8 = 15
 TLORA_T3_S3 = 16
 NANO_G1_EXPLORER = 17
 STATION_G1 = 25
+RAK11310 = 26
 LORA_RELAY_V1 = 32
 NRF52840DK = 33
 PPR = 34
 GENIEBLOCKS = 35
 NRF52_UNKNOWN = 36
 PORTDUINO = 37
 ANDROID_SIM = 38
@@ -59,14 +60,15 @@
 NRF52840_PCA10059 = 40
 DR_DEV = 41
 M5STACK = 42
 HELTEC_V3 = 43
 HELTEC_WSL_V3 = 44
 BETAFPV_2400_TX = 45
 BETAFPV_900_NANO_TX = 46
+RPI_PICO = 47
 PRIVATE_HW = 255
 ZERO = 0
 DATA_PAYLOAD_LEN = 237
 NONE = 0
 TX_WATCHDOG = 1
 SLEEP_ENTER_WAIT = 2
 NO_RADIO = 3
@@ -223,19 +225,19 @@
 _sym_db.RegisterMessage(DeviceMetadata)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\nMeshProtosZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
   _HARDWAREMODEL._serialized_start=4034
-  _HARDWAREMODEL._serialized_end=4624
-  _CONSTANTS._serialized_start=4626
-  _CONSTANTS._serialized_end=4670
-  _CRITICALERRORCODE._serialized_start=4673
-  _CRITICALERRORCODE._serialized_end=4911
+  _HARDWAREMODEL._serialized_end=4652
+  _CONSTANTS._serialized_start=4654
+  _CONSTANTS._serialized_end=4698
+  _CRITICALERRORCODE._serialized_start=4701
+  _CRITICALERRORCODE._serialized_end=4939
   _POSITION._serialized_start=189
   _POSITION._serialized_end=884
   _POSITION_LOCSOURCE._serialized_start=706
   _POSITION_LOCSOURCE._serialized_end=784
   _POSITION_ALTSOURCE._serialized_start=786
   _POSITION_ALTSOURCE._serialized_end=884
   _USER._serialized_start=887
```

### Comparing `meshtastic-2.1.7/meshtastic/module_config_pb2.py` & `meshtastic-2.1.8/meshtastic/module_config_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1emeshtastic/module_config.proto\"\x88\x18\n\x0cModuleConfig\x12(\n\x04mqtt\x18\x01 \x01(\x0b\x32\x18.ModuleConfig.MQTTConfigH\x00\x12,\n\x06serial\x18\x02 \x01(\x0b\x32\x1a.ModuleConfig.SerialConfigH\x00\x12I\n\x15\x65xternal_notification\x18\x03 \x01(\x0b\x32(.ModuleConfig.ExternalNotificationConfigH\x00\x12\x39\n\rstore_forward\x18\x04 \x01(\x0b\x32 .ModuleConfig.StoreForwardConfigH\x00\x12\x33\n\nrange_test\x18\x05 \x01(\x0b\x32\x1d.ModuleConfig.RangeTestConfigH\x00\x12\x32\n\ttelemetry\x18\x06 \x01(\x0b\x32\x1d.ModuleConfig.TelemetryConfigH\x00\x12;\n\x0e\x63\x61nned_message\x18\x07 \x01(\x0b\x32!.ModuleConfig.CannedMessageConfigH\x00\x12*\n\x05\x61udio\x18\x08 \x01(\x0b\x32\x19.ModuleConfig.AudioConfigH\x00\x12=\n\x0fremote_hardware\x18\t \x01(\x0b\x32\".ModuleConfig.RemoteHardwareConfigH\x00\x1a\xa7\x01\n\nMQTTConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07\x61\x64\x64ress\x18\x02 \x01(\t\x12\x10\n\x08username\x18\x03 \x01(\t\x12\x10\n\x08password\x18\x04 \x01(\t\x12\x1a\n\x12\x65ncryption_enabled\x18\x05 \x01(\x08\x12\x14\n\x0cjson_enabled\x18\x06 \x01(\x08\x12\x13\n\x0btls_enabled\x18\x07 \x01(\x08\x12\x0c\n\x04root\x18\x08 \x01(\t\x1aw\n\x14RemoteHardwareConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\"\n\x1a\x61llow_undefined_pin_access\x18\x02 \x01(\x08\x12*\n\x0e\x61vailable_pins\x18\x03 \x03(\x0b\x32\x12.RemoteHardwarePin\x1a\xd9\x02\n\x0b\x41udioConfig\x12\x16\n\x0e\x63odec2_enabled\x18\x01 \x01(\x08\x12\x0f\n\x07ptt_pin\x18\x02 \x01(\r\x12\x35\n\x07\x62itrate\x18\x03 \x01(\x0e\x32$.ModuleConfig.AudioConfig.Audio_Baud\x12\x0e\n\x06i2s_ws\x18\x04 \x01(\r\x12\x0e\n\x06i2s_sd\x18\x05 \x01(\r\x12\x0f\n\x07i2s_din\x18\x06 \x01(\r\x12\x0f\n\x07i2s_sck\x18\x07 \x01(\r\"\xa7\x01\n\nAudio_Baud\x12\x12\n\x0e\x43ODEC2_DEFAULT\x10\x00\x12\x0f\n\x0b\x43ODEC2_3200\x10\x01\x12\x0f\n\x0b\x43ODEC2_2400\x10\x02\x12\x0f\n\x0b\x43ODEC2_1600\x10\x03\x12\x0f\n\x0b\x43ODEC2_1400\x10\x04\x12\x0f\n\x0b\x43ODEC2_1300\x10\x05\x12\x0f\n\x0b\x43ODEC2_1200\x10\x06\x12\x0e\n\nCODEC2_700\x10\x07\x12\x0f\n\x0b\x43ODEC2_700B\x10\x08\x1a\x9b\x04\n\x0cSerialConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04\x65\x63ho\x18\x02 \x01(\x08\x12\x0b\n\x03rxd\x18\x03 \x01(\r\x12\x0b\n\x03txd\x18\x04 \x01(\r\x12\x34\n\x04\x62\x61ud\x18\x05 \x01(\x0e\x32&.ModuleConfig.SerialConfig.Serial_Baud\x12\x0f\n\x07timeout\x18\x06 \x01(\r\x12\x34\n\x04mode\x18\x07 \x01(\x0e\x32&.ModuleConfig.SerialConfig.Serial_Mode\"\x8a\x02\n\x0bSerial_Baud\x12\x10\n\x0c\x42\x41UD_DEFAULT\x10\x00\x12\x0c\n\x08\x42\x41UD_110\x10\x01\x12\x0c\n\x08\x42\x41UD_300\x10\x02\x12\x0c\n\x08\x42\x41UD_600\x10\x03\x12\r\n\tBAUD_1200\x10\x04\x12\r\n\tBAUD_2400\x10\x05\x12\r\n\tBAUD_4800\x10\x06\x12\r\n\tBAUD_9600\x10\x07\x12\x0e\n\nBAUD_19200\x10\x08\x12\x0e\n\nBAUD_38400\x10\t\x12\x0e\n\nBAUD_57600\x10\n\x12\x0f\n\x0b\x42\x41UD_115200\x10\x0b\x12\x0f\n\x0b\x42\x41UD_230400\x10\x0c\x12\x0f\n\x0b\x42\x41UD_460800\x10\r\x12\x0f\n\x0b\x42\x41UD_576000\x10\x0e\x12\x0f\n\x0b\x42\x41UD_921600\x10\x0f\"H\n\x0bSerial_Mode\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\n\n\x06SIMPLE\x10\x01\x12\t\n\x05PROTO\x10\x02\x12\x0b\n\x07TEXTMSG\x10\x03\x12\x08\n\x04NMEA\x10\x04\x1a\xce\x02\n\x1a\x45xternalNotificationConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\toutput_ms\x18\x02 \x01(\r\x12\x0e\n\x06output\x18\x03 \x01(\r\x12\x14\n\x0coutput_vibra\x18\x08 \x01(\r\x12\x15\n\routput_buzzer\x18\t \x01(\r\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12\x15\n\ralert_message\x18\x05 \x01(\x08\x12\x1b\n\x13\x61lert_message_vibra\x18\n \x01(\x08\x12\x1c\n\x14\x61lert_message_buzzer\x18\x0b \x01(\x08\x12\x12\n\nalert_bell\x18\x06 \x01(\x08\x12\x18\n\x10\x61lert_bell_vibra\x18\x0c \x01(\x08\x12\x19\n\x11\x61lert_bell_buzzer\x18\r \x01(\x08\x12\x0f\n\x07use_pwm\x18\x07 \x01(\x08\x12\x13\n\x0bnag_timeout\x18\x0e \x01(\r\x1a\x84\x01\n\x12StoreForwardConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\theartbeat\x18\x02 \x01(\x08\x12\x0f\n\x07records\x18\x03 \x01(\r\x12\x1a\n\x12history_return_max\x18\x04 \x01(\r\x12\x1d\n\x15history_return_window\x18\x05 \x01(\r\x1a@\n\x0fRangeTestConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0e\n\x06sender\x18\x02 \x01(\r\x12\x0c\n\x04save\x18\x03 \x01(\x08\x1a\x86\x02\n\x0fTelemetryConfig\x12\x1e\n\x16\x64\x65vice_update_interval\x18\x01 \x01(\r\x12#\n\x1b\x65nvironment_update_interval\x18\x02 \x01(\r\x12\'\n\x1f\x65nvironment_measurement_enabled\x18\x03 \x01(\x08\x12\"\n\x1a\x65nvironment_screen_enabled\x18\x04 \x01(\x08\x12&\n\x1e\x65nvironment_display_fahrenheit\x18\x05 \x01(\x08\x12\x1b\n\x13\x61ir_quality_enabled\x18\x06 \x01(\x08\x12\x1c\n\x14\x61ir_quality_interval\x18\x07 \x01(\r\x1a\xb5\x04\n\x13\x43\x61nnedMessageConfig\x12\x17\n\x0frotary1_enabled\x18\x01 \x01(\x08\x12\x19\n\x11inputbroker_pin_a\x18\x02 \x01(\r\x12\x19\n\x11inputbroker_pin_b\x18\x03 \x01(\r\x12\x1d\n\x15inputbroker_pin_press\x18\x04 \x01(\r\x12N\n\x14inputbroker_event_cw\x18\x05 \x01(\x0e\x32\x30.ModuleConfig.CannedMessageConfig.InputEventChar\x12O\n\x15inputbroker_event_ccw\x18\x06 \x01(\x0e\x32\x30.ModuleConfig.CannedMessageConfig.InputEventChar\x12Q\n\x17inputbroker_event_press\x18\x07 \x01(\x0e\x32\x30.ModuleConfig.CannedMessageConfig.InputEventChar\x12\x17\n\x0fupdown1_enabled\x18\x08 \x01(\x08\x12\x0f\n\x07\x65nabled\x18\t \x01(\x08\x12\x1a\n\x12\x61llow_input_source\x18\n \x01(\t\x12\x11\n\tsend_bell\x18\x0b \x01(\x08\"c\n\x0eInputEventChar\x12\x08\n\x04NONE\x10\x00\x12\x06\n\x02UP\x10\x11\x12\x08\n\x04\x44OWN\x10\x12\x12\x08\n\x04LEFT\x10\x13\x12\t\n\x05RIGHT\x10\x14\x12\n\n\x06SELECT\x10\n\x12\x08\n\x04\x42\x41\x43K\x10\x1b\x12\n\n\x06\x43\x41NCEL\x10\x18\x42\x11\n\x0fpayload_variant\"Y\n\x11RemoteHardwarePin\x12\x10\n\x08gpio_pin\x18\x01 \x01(\r\x12\x0c\n\x04name\x18\x02 \x01(\t\x12$\n\x04type\x18\x03 \x01(\x0e\x32\x16.RemoteHardwarePinType*I\n\x15RemoteHardwarePinType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x10\n\x0c\x44IGITAL_READ\x10\x01\x12\x11\n\rDIGITAL_WRITE\x10\x02\x42g\n\x13\x63om.geeksville.meshB\x12ModuleConfigProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1emeshtastic/module_config.proto\"\xbb\x18\n\x0cModuleConfig\x12(\n\x04mqtt\x18\x01 \x01(\x0b\x32\x18.ModuleConfig.MQTTConfigH\x00\x12,\n\x06serial\x18\x02 \x01(\x0b\x32\x1a.ModuleConfig.SerialConfigH\x00\x12I\n\x15\x65xternal_notification\x18\x03 \x01(\x0b\x32(.ModuleConfig.ExternalNotificationConfigH\x00\x12\x39\n\rstore_forward\x18\x04 \x01(\x0b\x32 .ModuleConfig.StoreForwardConfigH\x00\x12\x33\n\nrange_test\x18\x05 \x01(\x0b\x32\x1d.ModuleConfig.RangeTestConfigH\x00\x12\x32\n\ttelemetry\x18\x06 \x01(\x0b\x32\x1d.ModuleConfig.TelemetryConfigH\x00\x12;\n\x0e\x63\x61nned_message\x18\x07 \x01(\x0b\x32!.ModuleConfig.CannedMessageConfigH\x00\x12*\n\x05\x61udio\x18\x08 \x01(\x0b\x32\x19.ModuleConfig.AudioConfigH\x00\x12=\n\x0fremote_hardware\x18\t \x01(\x0b\x32\".ModuleConfig.RemoteHardwareConfigH\x00\x1a\xa7\x01\n\nMQTTConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0f\n\x07\x61\x64\x64ress\x18\x02 \x01(\t\x12\x10\n\x08username\x18\x03 \x01(\t\x12\x10\n\x08password\x18\x04 \x01(\t\x12\x1a\n\x12\x65ncryption_enabled\x18\x05 \x01(\x08\x12\x14\n\x0cjson_enabled\x18\x06 \x01(\x08\x12\x13\n\x0btls_enabled\x18\x07 \x01(\x08\x12\x0c\n\x04root\x18\x08 \x01(\t\x1aw\n\x14RemoteHardwareConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\"\n\x1a\x61llow_undefined_pin_access\x18\x02 \x01(\x08\x12*\n\x0e\x61vailable_pins\x18\x03 \x03(\x0b\x32\x12.RemoteHardwarePin\x1a\xd9\x02\n\x0b\x41udioConfig\x12\x16\n\x0e\x63odec2_enabled\x18\x01 \x01(\x08\x12\x0f\n\x07ptt_pin\x18\x02 \x01(\r\x12\x35\n\x07\x62itrate\x18\x03 \x01(\x0e\x32$.ModuleConfig.AudioConfig.Audio_Baud\x12\x0e\n\x06i2s_ws\x18\x04 \x01(\r\x12\x0e\n\x06i2s_sd\x18\x05 \x01(\r\x12\x0f\n\x07i2s_din\x18\x06 \x01(\r\x12\x0f\n\x07i2s_sck\x18\x07 \x01(\r\"\xa7\x01\n\nAudio_Baud\x12\x12\n\x0e\x43ODEC2_DEFAULT\x10\x00\x12\x0f\n\x0b\x43ODEC2_3200\x10\x01\x12\x0f\n\x0b\x43ODEC2_2400\x10\x02\x12\x0f\n\x0b\x43ODEC2_1600\x10\x03\x12\x0f\n\x0b\x43ODEC2_1400\x10\x04\x12\x0f\n\x0b\x43ODEC2_1300\x10\x05\x12\x0f\n\x0b\x43ODEC2_1200\x10\x06\x12\x0e\n\nCODEC2_700\x10\x07\x12\x0f\n\x0b\x43ODEC2_700B\x10\x08\x1a\xce\x04\n\x0cSerialConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0c\n\x04\x65\x63ho\x18\x02 \x01(\x08\x12\x0b\n\x03rxd\x18\x03 \x01(\r\x12\x0b\n\x03txd\x18\x04 \x01(\r\x12\x34\n\x04\x62\x61ud\x18\x05 \x01(\x0e\x32&.ModuleConfig.SerialConfig.Serial_Baud\x12\x0f\n\x07timeout\x18\x06 \x01(\r\x12\x34\n\x04mode\x18\x07 \x01(\x0e\x32&.ModuleConfig.SerialConfig.Serial_Mode\x12$\n\x1coverride_console_serial_port\x18\x08 \x01(\x08\"\x8a\x02\n\x0bSerial_Baud\x12\x10\n\x0c\x42\x41UD_DEFAULT\x10\x00\x12\x0c\n\x08\x42\x41UD_110\x10\x01\x12\x0c\n\x08\x42\x41UD_300\x10\x02\x12\x0c\n\x08\x42\x41UD_600\x10\x03\x12\r\n\tBAUD_1200\x10\x04\x12\r\n\tBAUD_2400\x10\x05\x12\r\n\tBAUD_4800\x10\x06\x12\r\n\tBAUD_9600\x10\x07\x12\x0e\n\nBAUD_19200\x10\x08\x12\x0e\n\nBAUD_38400\x10\t\x12\x0e\n\nBAUD_57600\x10\n\x12\x0f\n\x0b\x42\x41UD_115200\x10\x0b\x12\x0f\n\x0b\x42\x41UD_230400\x10\x0c\x12\x0f\n\x0b\x42\x41UD_460800\x10\r\x12\x0f\n\x0b\x42\x41UD_576000\x10\x0e\x12\x0f\n\x0b\x42\x41UD_921600\x10\x0f\"U\n\x0bSerial_Mode\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\n\n\x06SIMPLE\x10\x01\x12\t\n\x05PROTO\x10\x02\x12\x0b\n\x07TEXTMSG\x10\x03\x12\x08\n\x04NMEA\x10\x04\x12\x0b\n\x07\x43\x41LTOPO\x10\x05\x1a\xce\x02\n\x1a\x45xternalNotificationConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\toutput_ms\x18\x02 \x01(\r\x12\x0e\n\x06output\x18\x03 \x01(\r\x12\x14\n\x0coutput_vibra\x18\x08 \x01(\r\x12\x15\n\routput_buzzer\x18\t \x01(\r\x12\x0e\n\x06\x61\x63tive\x18\x04 \x01(\x08\x12\x15\n\ralert_message\x18\x05 \x01(\x08\x12\x1b\n\x13\x61lert_message_vibra\x18\n \x01(\x08\x12\x1c\n\x14\x61lert_message_buzzer\x18\x0b \x01(\x08\x12\x12\n\nalert_bell\x18\x06 \x01(\x08\x12\x18\n\x10\x61lert_bell_vibra\x18\x0c \x01(\x08\x12\x19\n\x11\x61lert_bell_buzzer\x18\r \x01(\x08\x12\x0f\n\x07use_pwm\x18\x07 \x01(\x08\x12\x13\n\x0bnag_timeout\x18\x0e \x01(\r\x1a\x84\x01\n\x12StoreForwardConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x11\n\theartbeat\x18\x02 \x01(\x08\x12\x0f\n\x07records\x18\x03 \x01(\r\x12\x1a\n\x12history_return_max\x18\x04 \x01(\r\x12\x1d\n\x15history_return_window\x18\x05 \x01(\r\x1a@\n\x0fRangeTestConfig\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x0e\n\x06sender\x18\x02 \x01(\r\x12\x0c\n\x04save\x18\x03 \x01(\x08\x1a\x86\x02\n\x0fTelemetryConfig\x12\x1e\n\x16\x64\x65vice_update_interval\x18\x01 \x01(\r\x12#\n\x1b\x65nvironment_update_interval\x18\x02 \x01(\r\x12\'\n\x1f\x65nvironment_measurement_enabled\x18\x03 \x01(\x08\x12\"\n\x1a\x65nvironment_screen_enabled\x18\x04 \x01(\x08\x12&\n\x1e\x65nvironment_display_fahrenheit\x18\x05 \x01(\x08\x12\x1b\n\x13\x61ir_quality_enabled\x18\x06 \x01(\x08\x12\x1c\n\x14\x61ir_quality_interval\x18\x07 \x01(\r\x1a\xb5\x04\n\x13\x43\x61nnedMessageConfig\x12\x17\n\x0frotary1_enabled\x18\x01 \x01(\x08\x12\x19\n\x11inputbroker_pin_a\x18\x02 \x01(\r\x12\x19\n\x11inputbroker_pin_b\x18\x03 \x01(\r\x12\x1d\n\x15inputbroker_pin_press\x18\x04 \x01(\r\x12N\n\x14inputbroker_event_cw\x18\x05 \x01(\x0e\x32\x30.ModuleConfig.CannedMessageConfig.InputEventChar\x12O\n\x15inputbroker_event_ccw\x18\x06 \x01(\x0e\x32\x30.ModuleConfig.CannedMessageConfig.InputEventChar\x12Q\n\x17inputbroker_event_press\x18\x07 \x01(\x0e\x32\x30.ModuleConfig.CannedMessageConfig.InputEventChar\x12\x17\n\x0fupdown1_enabled\x18\x08 \x01(\x08\x12\x0f\n\x07\x65nabled\x18\t \x01(\x08\x12\x1a\n\x12\x61llow_input_source\x18\n \x01(\t\x12\x11\n\tsend_bell\x18\x0b \x01(\x08\"c\n\x0eInputEventChar\x12\x08\n\x04NONE\x10\x00\x12\x06\n\x02UP\x10\x11\x12\x08\n\x04\x44OWN\x10\x12\x12\x08\n\x04LEFT\x10\x13\x12\t\n\x05RIGHT\x10\x14\x12\n\n\x06SELECT\x10\n\x12\x08\n\x04\x42\x41\x43K\x10\x1b\x12\n\n\x06\x43\x41NCEL\x10\x18\x42\x11\n\x0fpayload_variant\"Y\n\x11RemoteHardwarePin\x12\x10\n\x08gpio_pin\x18\x01 \x01(\r\x12\x0c\n\x04name\x18\x02 \x01(\t\x12$\n\x04type\x18\x03 \x01(\x0e\x32\x16.RemoteHardwarePinType*I\n\x15RemoteHardwarePinType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x10\n\x0c\x44IGITAL_READ\x10\x01\x12\x11\n\rDIGITAL_WRITE\x10\x02\x42g\n\x13\x63om.geeksville.meshB\x12ModuleConfigProtosZ\"github.com/meshtastic/go/generated\xaa\x02\x14Meshtastic.Protobufs\xba\x02\x00\x62\x06proto3')
 
 _REMOTEHARDWAREPINTYPE = DESCRIPTOR.enum_types_by_name['RemoteHardwarePinType']
 RemoteHardwarePinType = enum_type_wrapper.EnumTypeWrapper(_REMOTEHARDWAREPINTYPE)
 UNKNOWN = 0
 DIGITAL_READ = 1
 DIGITAL_WRITE = 2
 
@@ -125,40 +125,40 @@
   })
 _sym_db.RegisterMessage(RemoteHardwarePin)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\023com.geeksville.meshB\022ModuleConfigProtosZ\"github.com/meshtastic/go/generated\252\002\024Meshtastic.Protobufs\272\002\000'
-  _REMOTEHARDWAREPINTYPE._serialized_start=3208
-  _REMOTEHARDWAREPINTYPE._serialized_end=3281
+  _REMOTEHARDWAREPINTYPE._serialized_start=3259
+  _REMOTEHARDWAREPINTYPE._serialized_end=3332
   _MODULECONFIG._serialized_start=35
-  _MODULECONFIG._serialized_end=3115
+  _MODULECONFIG._serialized_end=3166
   _MODULECONFIG_MQTTCONFIG._serialized_start=547
   _MODULECONFIG_MQTTCONFIG._serialized_end=714
   _MODULECONFIG_REMOTEHARDWARECONFIG._serialized_start=716
   _MODULECONFIG_REMOTEHARDWARECONFIG._serialized_end=835
   _MODULECONFIG_AUDIOCONFIG._serialized_start=838
   _MODULECONFIG_AUDIOCONFIG._serialized_end=1183
   _MODULECONFIG_AUDIOCONFIG_AUDIO_BAUD._serialized_start=1016
   _MODULECONFIG_AUDIOCONFIG_AUDIO_BAUD._serialized_end=1183
   _MODULECONFIG_SERIALCONFIG._serialized_start=1186
-  _MODULECONFIG_SERIALCONFIG._serialized_end=1725
-  _MODULECONFIG_SERIALCONFIG_SERIAL_BAUD._serialized_start=1385
-  _MODULECONFIG_SERIALCONFIG_SERIAL_BAUD._serialized_end=1651
-  _MODULECONFIG_SERIALCONFIG_SERIAL_MODE._serialized_start=1653
-  _MODULECONFIG_SERIALCONFIG_SERIAL_MODE._serialized_end=1725
-  _MODULECONFIG_EXTERNALNOTIFICATIONCONFIG._serialized_start=1728
-  _MODULECONFIG_EXTERNALNOTIFICATIONCONFIG._serialized_end=2062
-  _MODULECONFIG_STOREFORWARDCONFIG._serialized_start=2065
-  _MODULECONFIG_STOREFORWARDCONFIG._serialized_end=2197
-  _MODULECONFIG_RANGETESTCONFIG._serialized_start=2199
-  _MODULECONFIG_RANGETESTCONFIG._serialized_end=2263
-  _MODULECONFIG_TELEMETRYCONFIG._serialized_start=2266
-  _MODULECONFIG_TELEMETRYCONFIG._serialized_end=2528
-  _MODULECONFIG_CANNEDMESSAGECONFIG._serialized_start=2531
-  _MODULECONFIG_CANNEDMESSAGECONFIG._serialized_end=3096
-  _MODULECONFIG_CANNEDMESSAGECONFIG_INPUTEVENTCHAR._serialized_start=2997
-  _MODULECONFIG_CANNEDMESSAGECONFIG_INPUTEVENTCHAR._serialized_end=3096
-  _REMOTEHARDWAREPIN._serialized_start=3117
-  _REMOTEHARDWAREPIN._serialized_end=3206
+  _MODULECONFIG_SERIALCONFIG._serialized_end=1776
+  _MODULECONFIG_SERIALCONFIG_SERIAL_BAUD._serialized_start=1423
+  _MODULECONFIG_SERIALCONFIG_SERIAL_BAUD._serialized_end=1689
+  _MODULECONFIG_SERIALCONFIG_SERIAL_MODE._serialized_start=1691
+  _MODULECONFIG_SERIALCONFIG_SERIAL_MODE._serialized_end=1776
+  _MODULECONFIG_EXTERNALNOTIFICATIONCONFIG._serialized_start=1779
+  _MODULECONFIG_EXTERNALNOTIFICATIONCONFIG._serialized_end=2113
+  _MODULECONFIG_STOREFORWARDCONFIG._serialized_start=2116
+  _MODULECONFIG_STOREFORWARDCONFIG._serialized_end=2248
+  _MODULECONFIG_RANGETESTCONFIG._serialized_start=2250
+  _MODULECONFIG_RANGETESTCONFIG._serialized_end=2314
+  _MODULECONFIG_TELEMETRYCONFIG._serialized_start=2317
+  _MODULECONFIG_TELEMETRYCONFIG._serialized_end=2579
+  _MODULECONFIG_CANNEDMESSAGECONFIG._serialized_start=2582
+  _MODULECONFIG_CANNEDMESSAGECONFIG._serialized_end=3147
+  _MODULECONFIG_CANNEDMESSAGECONFIG_INPUTEVENTCHAR._serialized_start=3048
+  _MODULECONFIG_CANNEDMESSAGECONFIG_INPUTEVENTCHAR._serialized_end=3147
+  _REMOTEHARDWAREPIN._serialized_start=3168
+  _REMOTEHARDWAREPIN._serialized_end=3257
 # @@protoc_insertion_point(module_scope)
```

### Comparing `meshtastic-2.1.7/meshtastic/mqtt_pb2.py` & `meshtastic-2.1.8/meshtastic/mqtt_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.7/meshtastic/node.py` & `meshtastic-2.1.8/meshtastic/node.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.7/meshtastic/portnums_pb2.py` & `meshtastic-2.1.8/meshtastic/portnums_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.7/meshtastic/remote_hardware.py` & `meshtastic-2.1.8/meshtastic/remote_hardware.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.7/meshtastic/remote_hardware_pb2.py` & `meshtastic-2.1.8/meshtastic/remote_hardware_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.7/meshtastic/rtttl_pb2.py` & `meshtastic-2.1.8/meshtastic/rtttl_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.7/meshtastic/serial_interface.py` & `meshtastic-2.1.8/meshtastic/serial_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.7/meshtastic/storeforward_pb2.py` & `meshtastic-2.1.8/meshtastic/storeforward_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.7/meshtastic/stream_interface.py` & `meshtastic-2.1.8/meshtastic/stream_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.7/meshtastic/supported_device.py` & `meshtastic-2.1.8/meshtastic/supported_device.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.7/meshtastic/tcp_interface.py` & `meshtastic-2.1.8/meshtastic/tcp_interface.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.7/meshtastic/telemetry_pb2.py` & `meshtastic-2.1.8/meshtastic/telemetry_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.7/meshtastic/test.py` & `meshtastic-2.1.8/meshtastic/test.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.7/meshtastic/tunnel.py` & `meshtastic-2.1.8/meshtastic/tunnel.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.7/meshtastic/util.py` & `meshtastic-2.1.8/meshtastic/util.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.7/meshtastic/xmodem_pb2.py` & `meshtastic-2.1.8/meshtastic/xmodem_pb2.py`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.7/meshtastic.egg-info/PKG-INFO` & `meshtastic-2.1.8/meshtastic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meshtastic
-Version: 2.1.7
+Version: 2.1.8
 Summary: Python API & client shell for talking to Meshtastic devices
 Home-page: https://github.com/meshtastic/python
 Author: Meshtastic Developers
 Author-email: contact@meshtastic.org
 License: GPL-3.0-only
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
```

### Comparing `meshtastic-2.1.7/meshtastic.egg-info/SOURCES.txt` & `meshtastic-2.1.8/meshtastic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `meshtastic-2.1.7/setup.py` & `meshtastic-2.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 # This call to setup() does all the work
 setup(
     name="meshtastic",
-    version="2.1.7",
+    version="2.1.8",
     description="Python API & client shell for talking to Meshtastic devices",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/meshtastic/python",
     author="Meshtastic Developers",
     author_email="contact@meshtastic.org",
     license="GPL-3.0-only",
```

