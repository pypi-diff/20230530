# Comparing `tmp/ovos-PHAL-plugin-homeassistant-0.0.2a3.tar.gz` & `tmp/ovos-PHAL-plugin-homeassistant-0.0.2a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-homeassistant-0.0.2a3.tar", last modified: Tue May 16 20:45:04 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-homeassistant-0.0.2a4.tar", last modified: Tue May 30 20:31:11 2023, max compression
```

## Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a3.tar` & `ovos-PHAL-plugin-homeassistant-0.0.2a4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:45:04.453076 ovos-PHAL-plugin-homeassistant-0.0.2a3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-16 20:44:51.000000 ovos-PHAL-plugin-homeassistant-0.0.2a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-16 20:45:04.453076 ovos-PHAL-plugin-homeassistant-0.0.2a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-16 20:44:51.000000 ovos-PHAL-plugin-homeassistant-0.0.2a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:45:04.449076 ovos-PHAL-plugin-homeassistant-0.0.2a3/ovos_PHAL_plugin_homeassistant/
--rw-r--r--   0 runner    (1001) docker     (123)    25743 2023-05-16 20:44:51.000000 ovos-PHAL-plugin-homeassistant-0.0.2a3/ovos_PHAL_plugin_homeassistant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-16 20:44:57.000000 ovos-PHAL-plugin-homeassistant-0.0.2a3/ovos_PHAL_plugin_homeassistant/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:45:04.453076 ovos-PHAL-plugin-homeassistant-0.0.2a3/ovos_PHAL_plugin_homeassistant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-16 20:45:03.000000 ovos-PHAL-plugin-homeassistant-0.0.2a3/ovos_PHAL_plugin_homeassistant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-16 20:45:04.000000 ovos-PHAL-plugin-homeassistant-0.0.2a3/ovos_PHAL_plugin_homeassistant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 20:45:03.000000 ovos-PHAL-plugin-homeassistant-0.0.2a3/ovos_PHAL_plugin_homeassistant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 20:45:03.000000 ovos-PHAL-plugin-homeassistant-0.0.2a3/ovos_PHAL_plugin_homeassistant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-16 20:45:03.000000 ovos-PHAL-plugin-homeassistant-0.0.2a3/ovos_PHAL_plugin_homeassistant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-16 20:45:03.000000 ovos-PHAL-plugin-homeassistant-0.0.2a3/ovos_PHAL_plugin_homeassistant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 20:45:03.000000 ovos-PHAL-plugin-homeassistant-0.0.2a3/ovos_PHAL_plugin_homeassistant.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:45:04.449076 ovos-PHAL-plugin-homeassistant-0.0.2a3/res/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:45:04.453076 ovos-PHAL-plugin-homeassistant-0.0.2a3/res/desktop/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-16 20:44:51.000000 ovos-PHAL-plugin-homeassistant-0.0.2a3/res/desktop/ovos-phal-homeassistant.desktop
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:45:04.453076 ovos-PHAL-plugin-homeassistant-0.0.2a3/res/icon/
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-16 20:44:51.000000 ovos-PHAL-plugin-homeassistant-0.0.2a3/res/icon/ovos-phal-homeassistant.svg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 20:45:04.453076 ovos-PHAL-plugin-homeassistant-0.0.2a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-16 20:44:51.000000 ovos-PHAL-plugin-homeassistant-0.0.2a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:31:11.553775 ovos-PHAL-plugin-homeassistant-0.0.2a4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-30 20:31:01.000000 ovos-PHAL-plugin-homeassistant-0.0.2a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-30 20:31:11.553775 ovos-PHAL-plugin-homeassistant-0.0.2a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-30 20:31:01.000000 ovos-PHAL-plugin-homeassistant-0.0.2a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:31:11.553775 ovos-PHAL-plugin-homeassistant-0.0.2a4/ovos_PHAL_plugin_homeassistant/
+-rw-r--r--   0 runner    (1001) docker     (123)    35559 2023-05-30 20:31:01.000000 ovos-PHAL-plugin-homeassistant-0.0.2a4/ovos_PHAL_plugin_homeassistant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-30 20:31:04.000000 ovos-PHAL-plugin-homeassistant-0.0.2a4/ovos_PHAL_plugin_homeassistant/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:31:11.553775 ovos-PHAL-plugin-homeassistant-0.0.2a4/ovos_PHAL_plugin_homeassistant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-30 20:31:11.000000 ovos-PHAL-plugin-homeassistant-0.0.2a4/ovos_PHAL_plugin_homeassistant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-30 20:31:11.000000 ovos-PHAL-plugin-homeassistant-0.0.2a4/ovos_PHAL_plugin_homeassistant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 20:31:11.000000 ovos-PHAL-plugin-homeassistant-0.0.2a4/ovos_PHAL_plugin_homeassistant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-30 20:31:11.000000 ovos-PHAL-plugin-homeassistant-0.0.2a4/ovos_PHAL_plugin_homeassistant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-30 20:31:11.000000 ovos-PHAL-plugin-homeassistant-0.0.2a4/ovos_PHAL_plugin_homeassistant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-30 20:31:11.000000 ovos-PHAL-plugin-homeassistant-0.0.2a4/ovos_PHAL_plugin_homeassistant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 20:31:11.000000 ovos-PHAL-plugin-homeassistant-0.0.2a4/ovos_PHAL_plugin_homeassistant.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:31:11.549775 ovos-PHAL-plugin-homeassistant-0.0.2a4/res/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:31:11.553775 ovos-PHAL-plugin-homeassistant-0.0.2a4/res/desktop/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-30 20:31:01.000000 ovos-PHAL-plugin-homeassistant-0.0.2a4/res/desktop/ovos-phal-homeassistant.desktop
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:31:11.553775 ovos-PHAL-plugin-homeassistant-0.0.2a4/res/icon/
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-30 20:31:01.000000 ovos-PHAL-plugin-homeassistant-0.0.2a4/res/icon/ovos-phal-homeassistant.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 20:31:11.553775 ovos-PHAL-plugin-homeassistant-0.0.2a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-30 20:31:01.000000 ovos-PHAL-plugin-homeassistant-0.0.2a4/setup.py
```

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a3/LICENSE` & `ovos-PHAL-plugin-homeassistant-0.0.2a4/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a3/PKG-INFO` & `ovos-PHAL-plugin-homeassistant-0.0.2a4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-homeassistant
-Version: 0.0.2a3
+Version: 0.0.2a4
 Summary: Notifications and Widgets plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-homeassistant
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a3/README.md` & `ovos-PHAL-plugin-homeassistant-0.0.2a4/README.md`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a3/ovos_PHAL_plugin_homeassistant/__init__.py` & `ovos-PHAL-plugin-homeassistant-0.0.2a4/ovos_PHAL_plugin_homeassistant/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,55 +1,65 @@
 import uuid
+import asyncio
+from copy import deepcopy
 from os.path import dirname, join
+from typing import Optional
+
+from pfzy import fuzzy_match
 from ovos_utils.log import LOG
-from mycroft_bus_client.message import Message
+from ovos_bus_client import Message
 from ovos_plugin_manager.phal import PHALPlugin
 from ovos_utils.gui import GUIInterface
 from ovos_PHAL_plugin_homeassistant.logic.connector import HomeAssistantRESTConnector, HomeAssistantWSConnector
 from ovos_PHAL_plugin_homeassistant.logic.device import (HomeAssistantSensor,
                                                          HomeAssistantBinarySensor,
-                                                         HomeAssistantLight,
-                                                         HomeAssistantMediaPlayer,
+                                                         HomeAssistantLight, HomeAssistantAutomation,
+                                                         HomeAssistantMediaPlayer, HomeAssistantScene,
                                                          HomeAssistantVacuum, HomeAssistantSwitch,
                                                          HomeAssistantClimate, HomeAssistantCamera)
 from ovos_PHAL_plugin_homeassistant.logic.integration import Integrator
 from ovos_PHAL_plugin_homeassistant.logic.utils import (map_entity_to_device_type,
-                                                        check_if_device_type_is_group)
+                                                        check_if_device_type_is_group,
+                                                        get_percentage_brightness_from_ha_value)
 from ovos_config.config import update_mycroft_config
 
+SUPPORTED_DEVICES = {
+            "sensor": HomeAssistantSensor,
+            "binary_sensor": HomeAssistantBinarySensor,
+            "light": HomeAssistantLight,
+            "media_player": HomeAssistantMediaPlayer,
+            "vacuum": HomeAssistantVacuum,
+            "switch": HomeAssistantSwitch,
+            "climate": HomeAssistantClimate,
+            "camera": HomeAssistantCamera,
+            "scene": HomeAssistantScene,
+            "automation": HomeAssistantAutomation,
+        }
+
 class HomeAssistantPlugin(PHALPlugin):
     def __init__(self, bus=None, config=None):
         """ Initialize the plugin
 
             Args:
                 bus (MycroftBusClient): The Mycroft bus client
                 config (dict): The plugin configuration
         """
         super().__init__(bus=bus, name="ovos-PHAL-plugin-homeassistant", config=config)
         self.oauth_client_id = None
         self.munged_id = "ovos-PHAL-plugin-homeassistant_homeassistant-phal-plugin"
         self.temporary_instance = None
         self.connector = None
-        self.registered_devices = []
+        self.registered_devices = []  # Device objects
+        self.registered_device_names = []  # Device friendly/entity names
         self.bus = bus
         self.gui = GUIInterface(bus=self.bus, skill_id=self.name)
         self.integrator = Integrator(self.bus, self.gui)
         self.instance_available = False
         self.use_ws = False
-        self.enable_debug = self.config.get("enable_debug", False)
-        self.device_types = {
-            "sensor": HomeAssistantSensor,
-            "binary_sensor": HomeAssistantBinarySensor,
-            "light": HomeAssistantLight,
-            "media_player": HomeAssistantMediaPlayer,
-            "vacuum": HomeAssistantVacuum,
-            "switch": HomeAssistantSwitch,
-            "climate": HomeAssistantClimate,
-            "camera": HomeAssistantCamera
-        }
+        self.device_types = SUPPORTED_DEVICES
 
         # BUS API FOR HOME ASSISTANT
         self.bus.on("ovos.phal.plugin.homeassistant.get.devices",
                     self.handle_get_devices)
         self.bus.on("ovos.phal.plugin.homeassistant.get.device",
                     self.handle_get_device)
         self.bus.on("ovos.phal.plugin.homeassistant.device.turn_on",
@@ -59,14 +69,21 @@
         self.bus.on("ovos.phal.plugin.homeassistant.get.device.display.model",
                     self.handle_get_device_display_model)
         self.bus.on("ovos.phal.plugin.homeassistant.get.device.display.list.model",
                     self.handle_get_device_display_list_model)
         self.bus.on("ovos.phal.plugin.homeassistant.call.supported.function",
                     self.handle_call_supported_function)
         self.bus.on("ovos.phal.plugin.homeassistant.start.oauth.flow", self.handle_start_oauth_flow)
+        self.bus.on("ovos.phal.plugin.homeassistant.assist.intent", self.handle_assist_message)
+        self.bus.on("ovos.phal.plugin.homeassistant.get.light.brightness", self.handle_get_light_brightness)
+        self.bus.on("ovos.phal.plugin.homeassistant.set.light.brightness", self.handle_set_light_brightness)
+        self.bus.on("ovos.phal.plugin.homeassistant.increase.light.brightness", self.handle_increase_light_brightness)
+        self.bus.on("ovos.phal.plugin.homeassistant.decrease.light.brightness", self.handle_decrease_light_brightness)
+        self.bus.on("ovos.phal.plugin.homeassistant.get.light.color", self.handle_get_light_color)
+        self.bus.on("ovos.phal.plugin.homeassistant.set.light.color", self.handle_set_light_color)
 
         # GUI EVENTS
         self.bus.on("ovos-PHAL-plugin-homeassistant.home",
                     self.handle_show_dashboard)
         self.bus.on("ovos-PHAL-plugin-homeassistant.close",
                     self.handle_close_dashboard)
         self.bus.on("ovos.phal.plugin.homeassistant.show.device.dashboard",
@@ -102,17 +119,17 @@
                 api_key (str): The Home Assistant API key
 
             Returns:
                 bool: True if the connection is valid, False otherwise
         """
         try:
             if self.use_ws:
-                validator = HomeAssistantWSConnector(host, api_key, self.enable_debug)
+                validator = HomeAssistantWSConnector(host, api_key)
             else:
-                validator = HomeAssistantRESTConnector(host, api_key, self.enable_debug)
+                validator = HomeAssistantRESTConnector(host, api_key)
 
             validator.get_all_devices()
 
             if self.use_ws:
                 if validator.client:
                     validator.disconnect()
 
@@ -161,19 +178,17 @@
 
         if not self.config.get("use_group_display"):
             self.config["use_group_display"] = False
 
         if configuration_host != "" and configuration_api_key != "":
             self.instance_available = True
             if self.use_ws:
-                self.connector = HomeAssistantWSConnector(configuration_host,
-                                                          configuration_api_key, self.enable_debug)
+                self.connector = HomeAssistantWSConnector(configuration_host, configuration_api_key)
             else:
-                self.connector = HomeAssistantRESTConnector(
-                    configuration_host, configuration_api_key, self.enable_debug)
+                self.connector = HomeAssistantRESTConnector(configuration_host, configuration_api_key)
             self.devices = self.connector.get_all_devices()
             self.registered_devices = []
             self.build_devices()
             self.gui["use_websocket"] = self.use_ws
             self.gui["instanceAvailable"] = True
             self.bus.emit(Message("ovos.phal.plugin.homeassistant.ready"))
         else:
@@ -191,25 +206,24 @@
                 if not device_type_is_group:
                     device_id = device["entity_id"]
                     device_name = device.get("attributes", {}).get(
                         "friendly_name", device_id)
                     device_icon = f"mdi:{device_type}"
                     device_state = device.get("state", None)
                     device_area = device.get("area_id", None)
-                    if self.enable_debug:
-                        LOG.info(
-                            f"Device added: {device_name} - {device_type} - {device_area}")
+                    LOG.debug(f"Device added: {device_name} - {device_type} - {device_area}")
 
                     device_attributes = device.get("attributes", {})
                     if device_type in self.device_types:
                         self.registered_devices.append(self.device_types[device_type](
                             self.connector, device_id, device_icon, device_name,
                             device_state, device_attributes, device_area, self.device_updated))
+                        self.registered_device_names.append(device_name)
                     else:
-                        LOG.warning(f"Device type {device_type} not supported")
+                        LOG.warning(f"Device type {device_type} not supported; please file an issue on GitHub")
                 else:
                     LOG.warning(
                         f"Device type {device_type} is a group, not supported currently")
 
     def build_display_dashboard_device_model(self):
         """ Build the dashboard model """
         device_type_model = []
@@ -310,78 +324,246 @@
                 message (Message): The message object
         """
         # build a plain list of devices
         device_list = []
         for device in self.registered_devices:
             device_list.append(device.get_device_display_model())
 
-        self.bus.emit(message.response(data=device_list))
+        self.bus.emit(message.response(data={"devices": device_list}))
+
+    def handle_get_device(self, message: Message):
+        """Handle the message to get a single device
 
-    def handle_get_device(self, message):
+        Args:
+            message (Message): The message object
+        """
+        # Device ID provided, usually GUI
         device_id = message.data.get("device_id", None)
         if device_id is not None:
-            for device in self.registered_devices:
-                if device.device_id == device_id:
-                    self.bus.emit(message.response(data=device))
-                    return
+            LOG.debug(f"Device ID provided in bus message: {device_id}")
+            return self._return_device_response(message, device_id)
+
+        # Device ID not provided, usually VUI
+        device = message.data.get("device")
+        device_result = self.fuzzy_match_name(
+                            self.registered_devices,
+                            device,
+                            self.registered_device_names
+                        )
+        LOG.debug(f"No device ID, found device result: {device_result or 'None'}")
+        if device_result:
+            return self._return_device_response(message, device_result)
+
+        # No device found
+        LOG.debug(f"No Home Assistant device exists for {device}")
+        self.bus.emit(message.response(data=None))
+
+    def _return_device_response(self, message, device_id) -> None:
+        """Return the device representation to the bus
+
+        Args:
+            message (Message): The message object to respond to
+            device_id (str): The device ID to lookup and return
+        """
+        for device in self.registered_devices:
+            if device.device_id == device_id:
+                return self.bus.emit(message.response(data=device.get_device_display_model()))
+        LOG.debug(f"No device found with device ID {device_id}")
         self.bus.emit(message.response(data=None))
 
     def handle_turn_on(self, message):
         """ Handle the turn on message
 
             Args:
                 message (Message): The message object
         """
-        device_id = message.data.get("device_id", None)
+        device_id, spoken_device = self._gather_device_id(message)
         if device_id is not None:
             for device in self.registered_devices:
                 if device.device_id == device_id:
-                    response = device.turn_on()
-                    self.bus.emit(message.response(data=response))
-                    return
-        else:
-            LOG.warning("No device id provided")
+                    device.turn_on()
+                    return self.bus.emit(message.response(data={"device": spoken_device}))
+        # No device found
+        LOG.debug(f"No Home Assistant device exists for {device_id}")
+        self.bus.emit(message.response(data=None))
 
     def handle_turn_off(self, message):
         """ Handle the turn off message
 
             Args:
                 message (Message): The message object
         """
-        device_id = message.data.get("device_id", None)
+        device_id, spoken_device = self._gather_device_id(message)
         if device_id is not None:
             for device in self.registered_devices:
                 if device.device_id == device_id:
-                    response = device.turn_off()
-                    self.bus.emit(message.response(data=response))
-                    return
-        else:
-            LOG.error("No device id provided")
+                    device.turn_off()
+                    return self.bus.emit(message.response(data={"device": spoken_device}))
+        # No device found
+        LOG.debug(f"No Home Assistant device exists for {device_id}")
+        self.bus.emit(message.response(data=None))
+
+    def _gather_device_id(self, message):
+        """Given a bus message, return the device ID and spoken device name for reference
+
+        Args:
+            message (Message): Bus message from GUI or VUI, or other source
+
+        Returns:
+            Tuple[Optional[str], str]: original device ID or device search result or None, spoken device name (str)
+        """
+        device_id = message.data.get("device_id", None)
+        device = message.data.get("device", None)
+        spoken_device = deepcopy(device) or device_id
+        if device_id is None and device is not None:
+            device_id = self.fuzzy_match_name(
+                            self.registered_devices,
+                            device,
+                            self.registered_device_names
+                        )
+            LOG.debug(f"No device ID, found device result: {device_id or 'None'}")
+        return device_id, spoken_device
 
     def handle_call_supported_function(self, message):
         """ Handle the call supported function message
 
         Args:
             message (Message): The message object
         """
-        device_id = message.data.get("device_id", None)
+        device_id, spoken_device = self._gather_device_id(message)
         function_name = message.data.get("function_name", None)
         function_args = message.data.get("function_args", None)
         if device_id is not None and function_name is not None:
             for device in self.registered_devices:
                 if device.device_id == device_id:
                     if function_args is not None:
                         response = device.call_function(
                             function_name, function_args)
                     else:
                         response = device.call_function(function_name)
-                    self.bus.emit(message.response(data=response))
-                    return
+                    return self.bus.emit(message.response(data={"device": spoken_device, "response": response}))
+        else:
+            response = "Device id or function name not provided"
+            LOG.error(response)
+            return self.bus.emit(message.response(data={"device": spoken_device, "response": response}))
+
+    def handle_get_light_brightness(self, message):
+        """ Handle the get light brightness message
+
+        Args:
+            message (Message): The message object
+        """
+        device_id, spoken_device = self._gather_device_id(message)
+        if device_id is not None:
+            for device in self.registered_devices:
+                if device.device_id == device_id:
+                    return self.bus.emit(message.response(
+                        data={
+                            "device": spoken_device,
+                            "brightness": get_percentage_brightness_from_ha_value(device.get_brightness())
+                            }))
+        else:
+            response = "Device id not provided"
+            LOG.error(response)
+            return self.bus.emit(message.response(data={"device": spoken_device, "response": response}))
+
+    def handle_get_light_color(self, message):
+        """ Handle the get light color VUI message
+
+        Args:
+            message (Message): The message object
+        """
+        device_id, spoken_device = self._gather_device_id(message)
+        if device_id is not None:
+            for device in self.registered_devices:
+                if device.device_id == device_id:
+                    color = device.get_spoken_color()
+                    return self.bus.emit(message.response(
+                        data={
+                            "device": spoken_device,
+                            "color": color
+                            }))
         else:
-            LOG.error("Device id or function name not provided")
+            response = "Device id not provided"
+            LOG.error(response)
+            return self.bus.emit(message.response(data={"device": spoken_device, "response": response}))
+
+    def handle_set_light_color(self, message):
+        """ Handle the set light color message
+
+        Args:
+            message (Message): The message object
+        """
+        device_id, spoken_device = self._gather_device_id(message)
+        color = message.data.get("color")
+        for device in self.registered_devices:
+            if device.device_id == device_id:
+                device.set_color(color)
+                return self.bus.emit(message.response(data={
+                    "device": spoken_device,
+                    "color": color
+                    }))
+        response = "Device id not provided"
+        LOG.error(response)
+        return self.bus.emit(message.response(data={"device": spoken_device, "response": response}))
+
+    def handle_set_light_brightness(self, message):
+        """ Handle the set light brightness message
+
+        Args:
+            message (Message): The message object
+        """
+        device_id, spoken_device = self._gather_device_id(message)
+        brightness = message.data.get("brightness")
+        for device in self.registered_devices:
+            if device.device_id == device_id:
+                device.set_brightness(brightness)
+                return self.bus.emit(message.response(data={
+                    "device": spoken_device,
+                    "brightness": get_percentage_brightness_from_ha_value(brightness)
+                    }))
+        response = "Device id not provided"
+        LOG.error(response)
+        return self.bus.emit(message.response(data={"device": spoken_device, "response": response}))
+
+    def handle_increase_light_brightness(self, message):
+        """ Handle the increase light brightness message
+
+        Args:
+            message (Message): The message object
+        """
+        device_id, spoken_device = self._gather_device_id(message)
+        for device in self.registered_devices:
+            if device.device_id == device_id:
+                brightness = device.increase_brightness()
+                return self.bus.emit(message.response(data={
+                    "device": spoken_device,
+                    "brightness": get_percentage_brightness_from_ha_value(brightness)
+                    }))
+        response = "Device id not provided"
+        LOG.error(response)
+        return self.bus.emit(message.response(data={"device": spoken_device, "response": response}))
+
+    def handle_decrease_light_brightness(self, message):
+        """ Handle the decrease light brightness message
+
+        Args:
+            message (Message): The message object
+        """
+        device_id, spoken_device = self._gather_device_id(message)
+        for device in self.registered_devices:
+            if device.device_id == device_id:
+                brightness = device.decrease_brightness()
+                return self.bus.emit(message.response(data={
+                    "device": spoken_device,
+                    "brightness": get_percentage_brightness_from_ha_value(brightness)
+                    }))
+        response = "Device id not provided"
+        LOG.error(response)
+        return self.bus.emit(message.response(data={"device": spoken_device, "response": response}))
 
     def handle_get_device_display_model(self, message):
         """ Handle the get device display model message
 
             Args:
                 message (Message): The message object
         """
@@ -401,14 +583,27 @@
                 message (Message): The message object
         """
         display_list_model = []
         for device in self.registered_devices:
             display_list_model.append(device.get_device_display_model())
         self.bus.emit(message.response(data=display_list_model))
 
+    def handle_assist_message(self, message):
+        """Handle a passthrough message to Home Assistant's Assist API.
+
+        Args:
+            message (Message): The message object
+        """
+        command: str = message.data.get("command")
+        LOG.debug(f"Received Assist command: {command}")
+        if self.connector and type(self.connector) in (HomeAssistantWSConnector, HomeAssistantRESTConnector):
+            self.bus.emit(message.response(data=self.connector.send_assist_command(command)))
+        else:
+            self.bus.emit(message.response(data=None))
+
 # GUI INTERFACE HANDLERS
     def handle_show_dashboard(self, message=None):
         """ Handle the show dashboard message
 
             Args:
                 message (Message): The message object
         """
@@ -433,17 +628,16 @@
             self.gui["instanceAvailable"] = False
             self.gui.send_event("ovos.phal.plugin.homeassistant.change.dashboard", {
                                 "dash_type": "main"})
             page = join(dirname(__file__), "ui", "Dashboard.qml")
             self.gui["use_group_display"] = self.config.get("use_group_display", False)
             self.gui.show_page(page, override_idle=True)
 
-        if self.enable_debug:
-            LOG.debug("Using group display")
-            LOG.debug(self.config["use_group_display"])
+        LOG.debug("Using group display")
+        LOG.debug(self.config["use_group_display"])
 
     def handle_close_dashboard(self, message):
         """ Handle the close dashboard message
 
             Args:
                 message (Message): The message object
         """
@@ -584,15 +778,15 @@
         access_token = response.get("access_token", None)
         if access_token:
             self.get_long_term_token(access_token)
 
     def get_long_term_token(self, short_term_token):
         instance = self.temporary_instance.replace("http://", "ws://").replace("https://", "wss://")
         token = short_term_token
-        wsClient = HomeAssistantWSConnector(instance, token, self.enable_debug)
+        wsClient = HomeAssistantWSConnector(instance, token)
         client_name = "ovos-PHAL-plugin-homeassistant-" + str(uuid.uuid4().hex)[:4]
         token_response = wsClient.call_command("auth/long_lived_access_token", {"client_name": client_name, "lifespan": 1825})
 
         if wsClient.client:
             wsClient.disconnect()
 
         if token_response:
@@ -608,7 +802,24 @@
 
         Args:
             device (dict): The device that was updated.
         """
         # GUI only event as we don't want to flood the GUI bus
         self.gui.send_event("ovos.phal.plugin.homeassistant.device.updated", {"device_id": device_id})
         self.bus.emit(Message("ovos.phal.plugin.homeassistant.device.state.updated"))
+
+# UTILS
+    def fuzzy_match_name(self, devices_list, spoken_name, device_names) -> Optional[str]:
+        """Given a list of device names, fuzzy match the spoken name to the most likely one.
+        Returns the device id of the most likely match or None if no match is found.
+        """
+        # https://github.com/kazhala/pfzy/issues/1 fuzzy_match mutates its haystack
+        device_names_haystack = deepcopy(device_names)
+        try:
+            result = asyncio.run(fuzzy_match(spoken_name, device_names_haystack))
+            if result:
+                return devices_list[device_names.index(result[0].get("value"))].device_id
+            else:
+                return None
+        except TypeError:
+            LOG.error(f"Failed to fuzzy match device name {spoken_name}", exc_info=True)
+            return None
```

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a3/ovos_PHAL_plugin_homeassistant.egg-info/PKG-INFO` & `ovos-PHAL-plugin-homeassistant-0.0.2a4/ovos_PHAL_plugin_homeassistant.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-homeassistant
-Version: 0.0.2a3
+Version: 0.0.2a4
 Summary: Notifications and Widgets plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-homeassistant
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a3/ovos_PHAL_plugin_homeassistant.egg-info/SOURCES.txt` & `ovos-PHAL-plugin-homeassistant-0.0.2a4/ovos_PHAL_plugin_homeassistant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a3/res/icon/ovos-phal-homeassistant.svg` & `ovos-PHAL-plugin-homeassistant-0.0.2a4/res/icon/ovos-phal-homeassistant.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.2a3/setup.py` & `ovos-PHAL-plugin-homeassistant-0.0.2a4/setup.py`

 * *Files identical despite different names*

