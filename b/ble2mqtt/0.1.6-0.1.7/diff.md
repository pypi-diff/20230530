# Comparing `tmp/ble2mqtt-0.1.6.tar.gz` & `tmp/ble2mqtt-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ble2mqtt-0.1.6.tar", last modified: Mon May 22 09:19:07 2023, max compression
+gzip compressed data, was "ble2mqtt-0.1.7.tar", last modified: Tue May 30 10:18:21 2023, max compression
```

## Comparing `ble2mqtt-0.1.6.tar` & `ble2mqtt-0.1.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-05-22 09:19:07.948243 ble2mqtt-0.1.6/
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1086 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/LICENSE
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)       55 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/MANIFEST.in
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     9910 2023-05-22 09:19:07.948306 ble2mqtt-0.1.6/PKG-INFO
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     9346 2023-05-22 09:03:15.000000 ble2mqtt-0.1.6/README.md
-drwxr-xr-x   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-05-22 09:19:07.944147 ble2mqtt-0.1.6/ble2mqtt/
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/__init__.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     4599 2023-05-21 11:18:54.000000 ble2mqtt-0.1.6/ble2mqtt/__main__.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)       18 2023-05-22 09:12:57.000000 ble2mqtt-0.1.6/ble2mqtt/__version__.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    39758 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/ble2mqtt.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)      574 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/compat.py
-drwxr-xr-x   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-05-22 09:19:07.947111 ble2mqtt-0.1.6/ble2mqtt/devices/
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)      911 2023-05-22 09:03:15.000000 ble2mqtt-0.1.6/ble2mqtt/devices/__init__.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1901 2023-05-22 09:03:15.000000 ble2mqtt-0.1.6/ble2mqtt/devices/atom_fast.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    27177 2023-05-22 09:03:15.000000 ble2mqtt-0.1.6/ble2mqtt/devices/base.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     4834 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/devices/bulb_avea.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    11419 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/devices/cooker_redmond.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     4603 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/devices/cover_am43.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     7158 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/devices/cover_soma.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    11248 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/devices/kettle_redmond.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     6571 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/devices/kettle_xiaomi.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     2579 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/devices/presence.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1526 2023-05-22 09:03:15.000000 ble2mqtt-0.1.6/ble2mqtt/devices/qingping_cgdk2.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     7154 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/devices/thermostat_ensto.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)      349 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/devices/uuids.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1571 2023-05-22 09:03:15.000000 ble2mqtt-0.1.6/ble2mqtt/devices/voltage_bm2.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     3438 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/devices/vson_air_wp6003.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1434 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/devices/xiaomi_base.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     2568 2023-05-22 09:03:15.000000 ble2mqtt-0.1.6/ble2mqtt/devices/xiaomi_ht.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1076 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/devices/xiaomi_lywsd03.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     2273 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/devices/xiaomi_lywsd03_atc.py
-drwxr-xr-x   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-05-22 09:19:07.948128 ble2mqtt-0.1.6/ble2mqtt/protocols/
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/protocols/__init__.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     4624 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/protocols/am43.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     5266 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/protocols/avea.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     3819 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/protocols/base.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     6596 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/protocols/ensto.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    16297 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/protocols/redmond.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     6441 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/protocols/soma.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     2618 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/protocols/wp6003.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    10322 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/protocols/xiaomi.py
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1692 2023-05-13 11:58:13.000000 ble2mqtt-0.1.6/ble2mqtt/utils.py
-drwxr-xr-x   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-05-22 09:19:07.944849 ble2mqtt-0.1.6/ble2mqtt.egg-info/
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     9910 2023-05-22 09:19:07.000000 ble2mqtt-0.1.6/ble2mqtt.egg-info/PKG-INFO
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1232 2023-05-22 09:19:07.000000 ble2mqtt-0.1.6/ble2mqtt.egg-info/SOURCES.txt
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)        1 2023-05-22 09:19:07.000000 ble2mqtt-0.1.6/ble2mqtt.egg-info/dependency_links.txt
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)       52 2023-05-22 09:19:07.000000 ble2mqtt-0.1.6/ble2mqtt.egg-info/entry_points.txt
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)       55 2023-05-22 09:19:07.000000 ble2mqtt-0.1.6/ble2mqtt.egg-info/requires.txt
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)        9 2023-05-22 09:19:07.000000 ble2mqtt-0.1.6/ble2mqtt.egg-info/top_level.txt
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)       99 2023-05-22 09:19:07.948546 ble2mqtt-0.1.6/setup.cfg
--rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1089 2023-05-22 09:03:15.000000 ble2mqtt-0.1.6/setup.py
+drwxr-xr-x   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-05-30 10:18:21.165963 ble2mqtt-0.1.7/
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1086 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/LICENSE
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)       55 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/MANIFEST.in
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     9910 2023-05-30 10:18:21.166038 ble2mqtt-0.1.7/PKG-INFO
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     9346 2023-05-22 09:03:15.000000 ble2mqtt-0.1.7/README.md
+drwxr-xr-x   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-05-30 10:18:21.161230 ble2mqtt-0.1.7/ble2mqtt/
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/__init__.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     4599 2023-05-21 11:18:54.000000 ble2mqtt-0.1.7/ble2mqtt/__main__.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)       18 2023-05-30 10:16:34.000000 ble2mqtt-0.1.7/ble2mqtt/__version__.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    39910 2023-05-30 10:17:41.000000 ble2mqtt-0.1.7/ble2mqtt/ble2mqtt.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)      574 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/compat.py
+drwxr-xr-x   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-05-30 10:18:21.164582 ble2mqtt-0.1.7/ble2mqtt/devices/
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)      911 2023-05-22 09:03:15.000000 ble2mqtt-0.1.7/ble2mqtt/devices/__init__.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1901 2023-05-22 09:03:15.000000 ble2mqtt-0.1.7/ble2mqtt/devices/atom_fast.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    27177 2023-05-22 09:03:15.000000 ble2mqtt-0.1.7/ble2mqtt/devices/base.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     4834 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/devices/bulb_avea.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    11419 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/devices/cooker_redmond.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     4603 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/devices/cover_am43.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     7158 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/devices/cover_soma.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    11248 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/devices/kettle_redmond.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     6571 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/devices/kettle_xiaomi.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     2579 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/devices/presence.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1526 2023-05-22 09:03:15.000000 ble2mqtt-0.1.7/ble2mqtt/devices/qingping_cgdk2.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     7154 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/devices/thermostat_ensto.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)      349 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/devices/uuids.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1571 2023-05-22 09:03:15.000000 ble2mqtt-0.1.7/ble2mqtt/devices/voltage_bm2.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     3438 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/devices/vson_air_wp6003.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1434 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/devices/xiaomi_base.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     2568 2023-05-22 09:03:15.000000 ble2mqtt-0.1.7/ble2mqtt/devices/xiaomi_ht.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1076 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/devices/xiaomi_lywsd03.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     2273 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/devices/xiaomi_lywsd03_atc.py
+drwxr-xr-x   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-05-30 10:18:21.165832 ble2mqtt-0.1.7/ble2mqtt/protocols/
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/protocols/__init__.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     4624 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/protocols/am43.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     5266 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/protocols/avea.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     3819 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/protocols/base.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     6596 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/protocols/ensto.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    16297 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/protocols/redmond.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     6441 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/protocols/soma.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     2618 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/protocols/wp6003.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)    10322 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/protocols/xiaomi.py
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1692 2023-05-13 11:58:13.000000 ble2mqtt-0.1.7/ble2mqtt/utils.py
+drwxr-xr-x   0 ivan.belokobylskiy   (501) staff       (20)        0 2023-05-30 10:18:21.162031 ble2mqtt-0.1.7/ble2mqtt.egg-info/
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     9910 2023-05-30 10:18:21.000000 ble2mqtt-0.1.7/ble2mqtt.egg-info/PKG-INFO
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1232 2023-05-30 10:18:21.000000 ble2mqtt-0.1.7/ble2mqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)        1 2023-05-30 10:18:21.000000 ble2mqtt-0.1.7/ble2mqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)       52 2023-05-30 10:18:21.000000 ble2mqtt-0.1.7/ble2mqtt.egg-info/entry_points.txt
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)       55 2023-05-30 10:18:21.000000 ble2mqtt-0.1.7/ble2mqtt.egg-info/requires.txt
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)        9 2023-05-30 10:18:21.000000 ble2mqtt-0.1.7/ble2mqtt.egg-info/top_level.txt
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)       99 2023-05-30 10:18:21.166316 ble2mqtt-0.1.7/setup.cfg
+-rw-r--r--   0 ivan.belokobylskiy   (501) staff       (20)     1089 2023-05-22 09:03:15.000000 ble2mqtt-0.1.7/setup.py
```

### Comparing `ble2mqtt-0.1.6/LICENSE` & `ble2mqtt-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.6/PKG-INFO` & `ble2mqtt-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ble2mqtt
-Version: 0.1.6
+Version: 0.1.7
 Summary: BLE to MQTT bridge
 Home-page: https://github.com/devbis/ble2mqtt/
 Author: Ivan Belokobylskiy
 Author-email: belokobylskij@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ble2mqtt-0.1.6/README.md` & `ble2mqtt-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.6/ble2mqtt/__main__.py` & `ble2mqtt-0.1.7/ble2mqtt/__main__.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.6/ble2mqtt/ble2mqtt.py` & `ble2mqtt-0.1.7/ble2mqtt/ble2mqtt.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,22 +216,25 @@
         return self.manage_task
 
     async def publish_topic_callback(self, topic, value, nowait=False):
         _LOGGER.debug(f'call publish callback topic={topic} value={value}')
         if not self._mqtt_client.is_connected():
             _LOGGER.warning(f'{self.device} mqtt is disconnected')
             return
-        await self._mqtt_client.publish(
-            aio_mqtt.PublishableMessage(
-                topic_name='/'.join((self._base_topic, topic)),
-                payload=value,
-                qos=aio_mqtt.QOSLevel.QOS_1,
-            ),
-            nowait=nowait,
-        )
+        try:
+            await self._mqtt_client.publish(
+                aio_mqtt.PublishableMessage(
+                    topic_name='/'.join((self._base_topic, topic)),
+                    payload=value,
+                    qos=aio_mqtt.QOSLevel.QOS_1,
+                ),
+                nowait=nowait,
+            )
+        except ListOfMQTTConnectionErrors:
+            _LOGGER.exception('Error while publishing to MQTT')
 
     def _get_topic(self, dev_id, subtopic, *args):
         return '/'.join(
             filter(None, (self._base_topic, dev_id, subtopic, *args)),
         )
 
     @property
```

### Comparing `ble2mqtt-0.1.6/ble2mqtt/compat.py` & `ble2mqtt-0.1.7/ble2mqtt/compat.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.6/ble2mqtt/devices/__init__.py` & `ble2mqtt-0.1.7/ble2mqtt/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.6/ble2mqtt/devices/atom_fast.py` & `ble2mqtt-0.1.7/ble2mqtt/devices/atom_fast.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.6/ble2mqtt/devices/base.py` & `ble2mqtt-0.1.7/ble2mqtt/devices/base.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.6/ble2mqtt/devices/bulb_avea.py` & `ble2mqtt-0.1.7/ble2mqtt/devices/bulb_avea.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.6/ble2mqtt/devices/cooker_redmond.py` & `ble2mqtt-0.1.7/ble2mqtt/devices/cooker_redmond.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.6/ble2mqtt/devices/cover_am43.py` & `ble2mqtt-0.1.7/ble2mqtt/devices/cover_am43.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.6/ble2mqtt/devices/cover_soma.py` & `ble2mqtt-0.1.7/ble2mqtt/devices/cover_soma.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.6/ble2mqtt/devices/kettle_redmond.py` & `ble2mqtt-0.1.7/ble2mqtt/devices/kettle_redmond.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.6/ble2mqtt/devices/kettle_xiaomi.py` & `ble2mqtt-0.1.7/ble2mqtt/devices/kettle_xiaomi.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.6/ble2mqtt/devices/presence.py` & `ble2mqtt-0.1.7/ble2mqtt/devices/presence.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.6/ble2mqtt/devices/qingping_cgdk2.py` & `ble2mqtt-0.1.7/ble2mqtt/devices/qingping_cgdk2.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.6/ble2mqtt/devices/thermostat_ensto.py` & `ble2mqtt-0.1.7/ble2mqtt/devices/thermostat_ensto.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.6/ble2mqtt/devices/voltage_bm2.py` & `ble2mqtt-0.1.7/ble2mqtt/devices/voltage_bm2.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.6/ble2mqtt/devices/vson_air_wp6003.py` & `ble2mqtt-0.1.7/ble2mqtt/devices/vson_air_wp6003.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.6/ble2mqtt/devices/xiaomi_base.py` & `ble2mqtt-0.1.7/ble2mqtt/devices/xiaomi_base.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.6/ble2mqtt/devices/xiaomi_ht.py` & `ble2mqtt-0.1.7/ble2mqtt/devices/xiaomi_ht.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.6/ble2mqtt/devices/xiaomi_lywsd03.py` & `ble2mqtt-0.1.7/ble2mqtt/devices/xiaomi_lywsd03.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.6/ble2mqtt/devices/xiaomi_lywsd03_atc.py` & `ble2mqtt-0.1.7/ble2mqtt/devices/xiaomi_lywsd03_atc.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.6/ble2mqtt/protocols/am43.py` & `ble2mqtt-0.1.7/ble2mqtt/protocols/am43.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.6/ble2mqtt/protocols/avea.py` & `ble2mqtt-0.1.7/ble2mqtt/protocols/avea.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.6/ble2mqtt/protocols/base.py` & `ble2mqtt-0.1.7/ble2mqtt/protocols/base.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.6/ble2mqtt/protocols/ensto.py` & `ble2mqtt-0.1.7/ble2mqtt/protocols/ensto.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.6/ble2mqtt/protocols/redmond.py` & `ble2mqtt-0.1.7/ble2mqtt/protocols/redmond.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.6/ble2mqtt/protocols/soma.py` & `ble2mqtt-0.1.7/ble2mqtt/protocols/soma.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.6/ble2mqtt/protocols/wp6003.py` & `ble2mqtt-0.1.7/ble2mqtt/protocols/wp6003.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.6/ble2mqtt/protocols/xiaomi.py` & `ble2mqtt-0.1.7/ble2mqtt/protocols/xiaomi.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.6/ble2mqtt/utils.py` & `ble2mqtt-0.1.7/ble2mqtt/utils.py`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.6/ble2mqtt.egg-info/PKG-INFO` & `ble2mqtt-0.1.7/ble2mqtt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ble2mqtt
-Version: 0.1.6
+Version: 0.1.7
 Summary: BLE to MQTT bridge
 Home-page: https://github.com/devbis/ble2mqtt/
 Author: Ivan Belokobylskiy
 Author-email: belokobylskij@gmail.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `ble2mqtt-0.1.6/ble2mqtt.egg-info/SOURCES.txt` & `ble2mqtt-0.1.7/ble2mqtt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ble2mqtt-0.1.6/setup.py` & `ble2mqtt-0.1.7/setup.py`

 * *Files identical despite different names*

