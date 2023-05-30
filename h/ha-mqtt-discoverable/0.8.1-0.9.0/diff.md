# Comparing `tmp/ha_mqtt_discoverable-0.8.1.tar.gz` & `tmp/ha_mqtt_discoverable-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ha_mqtt_discoverable-0.8.1.tar", max compression
+gzip compressed data, was "ha_mqtt_discoverable-0.9.0.tar", max compression
```

## Comparing `ha_mqtt_discoverable-0.8.1.tar` & `ha_mqtt_discoverable-0.9.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-03-26 22:44:16.004461 ha_mqtt_discoverable-0.8.1/LICENSE
--rw-r--r--   0        0        0     7958 2023-03-26 22:44:16.004461 ha_mqtt_discoverable-0.8.1/README.md
--rw-r--r--   0        0        0    34426 2023-03-26 22:44:16.004461 ha_mqtt_discoverable-0.8.1/ha_mqtt_discoverable/__init__.py
--rw-r--r--   0        0        0     2550 2023-03-26 22:44:16.004461 ha_mqtt_discoverable-0.8.1/ha_mqtt_discoverable/cli/__init__.py
--rw-r--r--   0        0        0     5969 2023-03-26 22:44:16.004461 ha_mqtt_discoverable-0.8.1/ha_mqtt_discoverable/sensors.py
--rw-r--r--   0        0        0     4950 2023-03-26 22:44:16.004461 ha_mqtt_discoverable-0.8.1/ha_mqtt_discoverable/settings.py
--rw-r--r--   0        0        0     1373 2023-03-26 22:44:16.004461 ha_mqtt_discoverable-0.8.1/ha_mqtt_discoverable/utils.py
--rw-r--r--   0        0        0      617 2023-03-26 22:44:28.108591 ha_mqtt_discoverable-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     8519 1970-01-01 00:00:00.000000 ha_mqtt_discoverable-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-30 02:44:59.207970 ha_mqtt_discoverable-0.9.0/LICENSE
+-rw-r--r--   0        0        0     9149 2023-05-30 02:44:59.207970 ha_mqtt_discoverable-0.9.0/README.md
+-rw-r--r--   0        0        0    34518 2023-05-30 02:44:59.207970 ha_mqtt_discoverable-0.9.0/ha_mqtt_discoverable/__init__.py
+-rw-r--r--   0        0        0     2550 2023-05-30 02:44:59.207970 ha_mqtt_discoverable-0.9.0/ha_mqtt_discoverable/cli/__init__.py
+-rw-r--r--   0        0        0     7301 2023-05-30 02:44:59.207970 ha_mqtt_discoverable-0.9.0/ha_mqtt_discoverable/sensors.py
+-rw-r--r--   0        0        0     4950 2023-05-30 02:44:59.207970 ha_mqtt_discoverable-0.9.0/ha_mqtt_discoverable/settings.py
+-rw-r--r--   0        0        0     1373 2023-05-30 02:44:59.207970 ha_mqtt_discoverable-0.9.0/ha_mqtt_discoverable/utils.py
+-rw-r--r--   0        0        0      617 2023-05-30 02:45:14.528197 ha_mqtt_discoverable-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     9710 1970-01-01 00:00:00.000000 ha_mqtt_discoverable-0.9.0/PKG-INFO
```

### Comparing `ha_mqtt_discoverable-0.8.1/LICENSE` & `ha_mqtt_discoverable-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ha_mqtt_discoverable-0.8.1/README.md` & `ha_mqtt_discoverable-0.9.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: ha-mqtt-discoverable
+Version: 0.9.0
+Summary: 
+Author: Joe Block
+Author-email: jpb@unixorn.net
+Requires-Python: >=3.10.0,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: gitlike-commands (>=0.2.1,<0.3.0)
+Requires-Dist: paho-mqtt (>=1.6.1,<2.0.0)
+Requires-Dist: pyaml (>=21.10.1,<22.0.0)
+Requires-Dist: pydantic (>=1.10.5,<2.0.0)
+Requires-Dist: thelogrus (>=0.7.0,<0.8.0)
+Description-Content-Type: text/markdown
+
 # ha-mqtt-discoverable
 
 [![License](https://img.shields.io/github/license/unixorn/ha-mqtt-discoverable.svg)](https://opensource.org/license/apache-2-0/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![GitHub last commit (branch)](https://img.shields.io/github/last-commit/unixorn/ha-mqtt-discoverable/main.svg)](https://github.com/unixorn/ha-mqtt-discoverable)
 [![Downloads](https://static.pepy.tech/badge/ha-mqtt-discoverable)](https://pepy.tech/project/ha-mqtt-discoverable)
 
@@ -16,18 +33,20 @@
 - [Installing](#installing)
   - [Python](#python)
 - [Supported entities](#supported-entities)
   - [Binary sensor](#binary-sensor)
     - [Usage](#usage)
   - [Switch](#switch)
     - [Usage](#usage-1)
+  - [Text](#text)
+    - [Usage](#usage-2)
 - [Device](#device)
-  - [Usage](#usage-2)
+  - [Usage](#usage-3)
   - [Device trigger](#device-trigger)
-    - [Usage](#usage-3)
+    - [Usage](#usage-4)
 - [Contributing](#contributing)
 - [Users of ha-mqtt-discoverable](#users-of-ha-mqtt-discoverable)
 - [Contributors](#contributors)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 
 ## Installing
@@ -44,14 +63,16 @@
 
 - Sensor
 - Binary sensor
 - Switch
 - Button
 - Device trigger
 
+Each entity can associated to a device. See below for details.
+
 ### Binary sensor
 
 #### Usage
 
 The following example creates a binary sensor and sets its state:
 
 ```py
@@ -91,16 +112,15 @@
 from ha_mqtt_discoverable.sensors import Switch, SwitchInfo
 from paho.mqtt.client import Client, MQTTMessage
 
 # Configure the required parameters for the MQTT broker
 mqtt_settings = Settings.MQTT(host="localhost")
 
 # Information about the switch
-# If `command_topic` is defined, it will receive state updates from HA
-switch_info = SwitchInfo(name="test", command_topic="command")
+switch_info = SwitchInfo(name="test")
 
 settings = Settings(mqtt=mqtt_settings, entity=switch_info)
 
 # To receive state commands from HA, define a callback function:
 def my_callback(client: Client, user_data, message: MQTTMessage):
     payload = message.payload.decode()
     logging.info(f"Received {payload} from HA")
@@ -114,14 +134,51 @@
 
 # Change the state of the sensor, publishing an MQTT message that gets picked up by HA
 my_switch.on()
 my_switch.off()
 
 ```
 
+### Text
+
+The text is an `helper entity`, showing an input field in the HA UI that the user can interact with.
+It is possible to act upon reception of the inputted text by defining a `callback` function, as the following example shows:
+
+#### Usage
+
+```py
+from ha_mqtt_discoverable import Settings
+from ha_mqtt_discoverable.sensors import Text, TextInfo
+from paho.mqtt.client import Client, MQTTMessage
+
+# Configure the required parameters for the MQTT broker
+mqtt_settings = Settings.MQTT(host="localhost")
+
+# Information about the `text` entity
+text_info = TextInfo(name="test")
+
+settings = Settings(mqtt=mqtt_settings, entity=switch_info)
+
+# To receive text updates from HA, define a callback function:
+def my_callback(client: Client, user_data, message: MQTTMessage):
+    text = message.payload.decode()
+    logging.info(f"Received {text} from HA")
+    # Your custom code...
+
+# Define an optional object to be passed back to the callback
+user_data = "Some custom data"
+
+# Instantiate the text
+my_text = Text(settings, my_callback, user_data)
+
+# Change the text displayed in HA UI, publishing an MQTT message that gets picked up by HA
+my_text.set_text("Some awesome text")
+
+```
+
 ## Device
 From the [Home Assistant documentation](https://developers.home-assistant.io/docs/device_registry_index):
 > A device is a special entity in Home Assistant that is represented by one or more entities.
 A device is automatically created when an entity defines its `device` property.
 A device will be matched up with an existing device via supplied identifiers or connections, like serial numbers or MAC addresses.
 
 ### Usage
@@ -204,7 +261,8 @@
 ## Contributors
 
 <a href="https://github.com/unixorn/ha-mqtt-discoverable/graphs/contributors">
   <img src="https://contributors-img.web.app/image?repo=unixorn/ha-mqtt-discoverable" />
 </a>
 
 Made with [contributors-img](https://contributors-img.web.app).
+
```

### Comparing `ha_mqtt_discoverable-0.8.1/ha_mqtt_discoverable/__init__.py` & `ha_mqtt_discoverable-0.9.0/ha_mqtt_discoverable/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -500,14 +500,16 @@
     """Information about the sensor"""
     device: Optional[DeviceInfo] = None
     """Information about the device this sensor belongs to"""
     device_class: Optional[str] = None
     """Sets the class of the device, changing the device state and icon that is displayed on the frontend."""
     enabled_by_default: Optional[bool] = None
     """Flag which defines if the entity should be enabled when first added."""
+    entity_category: Optional[str] = None
+    """Classification of a non-primary entity."""
     expire_after: Optional[int] = None
     """If set, it defines the number of seconds after the sensor’s state expires, if it’s not updated.\
     After expiry, the sensor’s state becomes unavailable. Default the sensors state never expires."""
     force_update: Optional[bool] = None
     """Sends update events even if the value hasn’t changed.\
     Useful if you want to have meaningful value graphs in history."""
     icon: Optional[str] = None
```

### Comparing `ha_mqtt_discoverable-0.8.1/ha_mqtt_discoverable/cli/__init__.py` & `ha_mqtt_discoverable-0.9.0/ha_mqtt_discoverable/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ha_mqtt_discoverable-0.8.1/ha_mqtt_discoverable/sensors.py` & `ha_mqtt_discoverable-0.9.0/ha_mqtt_discoverable/sensors.py`

 * *Files 12% similar despite different names*

```diff
@@ -77,14 +77,32 @@
 
     payload_press: str = "PRESS"
     """The payload to send to trigger the button."""
     retain: Optional[bool] = None
     """If the published message should have the retain flag on or not"""
 
 
+class TextInfo(EntityInfo):
+    """Information about the `text` entity"""
+
+    component: str = "text"
+
+    max: int = 255
+    """The maximum size of a text being set or received (maximum is 255)."""
+    min: int = 0
+    """The minimum size of a text being set or received."""
+    mode: Optional[str] = "text"
+    """The mode off the text entity. Must be either text or password."""
+    pattern: Optional[str] = None
+    """A valid regular expression the text being set or received must match with."""
+
+    retain: Optional[bool] = None
+    """If the published message should have the retain flag on or not"""
+
+
 class DeviceTriggerInfo(EntityInfo):
     """Information about the device trigger"""
 
     component: str = "device_automation"
     automation_type: str = "trigger"
     """The type of automation, must be ‘trigger’."""
 
@@ -186,7 +204,28 @@
         Generate a device trigger event
 
         Args:
             payload: custom payload to send in the trigger topic
 
         """
         return self._state_helper(payload, self.state_topic, retain=False)
+
+
+class Text(Subscriber[TextInfo]):
+    """Implements an MQTT text:
+    https://www.home-assistant.io/integrations/text.mqtt/
+    """
+
+    def set_text(self, text: str) -> None:
+        """
+        Update the text displayed by this sensor. Check that it is of acceptable length.
+
+        Args:
+            text(str): Value of the text configured for this entity
+        """
+        if not self._entity.min <= len(text) <= self._entity.max:
+            raise RuntimeError(
+                f"Text is not within configured length boundaries [{self._entity.min}, {self._entity.max}]"
+            )
+
+        logger.info(f"Setting {self._entity.name} to {text} using {self.state_topic}")
+        self._state_helper(str(text))
```

### Comparing `ha_mqtt_discoverable-0.8.1/ha_mqtt_discoverable/settings.py` & `ha_mqtt_discoverable-0.9.0/ha_mqtt_discoverable/settings.py`

 * *Files identical despite different names*

### Comparing `ha_mqtt_discoverable-0.8.1/ha_mqtt_discoverable/utils.py` & `ha_mqtt_discoverable-0.9.0/ha_mqtt_discoverable/utils.py`

 * *Files identical despite different names*

### Comparing `ha_mqtt_discoverable-0.8.1/pyproject.toml` & `ha_mqtt_discoverable-0.9.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ha-mqtt-discoverable"
-version = "0.8.1"
+version = "0.9.0"
 description = ""
 authors = ["Joe Block <jpb@unixorn.net>"]
 readme = "README.md"
 packages = [{include = "ha_mqtt_discoverable"}]
 
 [tool.poetry.dependencies]
 python = ">=3.10.0,<4.0"
```

### Comparing `ha_mqtt_discoverable-0.8.1/PKG-INFO` & `ha_mqtt_discoverable-0.9.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: ha-mqtt-discoverable
-Version: 0.8.1
-Summary: 
-Author: Joe Block
-Author-email: jpb@unixorn.net
-Requires-Python: >=3.10.0,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: gitlike-commands (>=0.2.1,<0.3.0)
-Requires-Dist: paho-mqtt (>=1.6.1,<2.0.0)
-Requires-Dist: pyaml (>=21.10.1,<22.0.0)
-Requires-Dist: pydantic (>=1.10.5,<2.0.0)
-Requires-Dist: thelogrus (>=0.7.0,<0.8.0)
-Description-Content-Type: text/markdown
-
 # ha-mqtt-discoverable
 
 [![License](https://img.shields.io/github/license/unixorn/ha-mqtt-discoverable.svg)](https://opensource.org/license/apache-2-0/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![GitHub last commit (branch)](https://img.shields.io/github/last-commit/unixorn/ha-mqtt-discoverable/main.svg)](https://github.com/unixorn/ha-mqtt-discoverable)
 [![Downloads](https://static.pepy.tech/badge/ha-mqtt-discoverable)](https://pepy.tech/project/ha-mqtt-discoverable)
 
@@ -33,18 +16,20 @@
 - [Installing](#installing)
   - [Python](#python)
 - [Supported entities](#supported-entities)
   - [Binary sensor](#binary-sensor)
     - [Usage](#usage)
   - [Switch](#switch)
     - [Usage](#usage-1)
+  - [Text](#text)
+    - [Usage](#usage-2)
 - [Device](#device)
-  - [Usage](#usage-2)
+  - [Usage](#usage-3)
   - [Device trigger](#device-trigger)
-    - [Usage](#usage-3)
+    - [Usage](#usage-4)
 - [Contributing](#contributing)
 - [Users of ha-mqtt-discoverable](#users-of-ha-mqtt-discoverable)
 - [Contributors](#contributors)
 
 <!-- END doctoc generated TOC please keep comment here to allow auto update -->
 
 ## Installing
@@ -61,14 +46,16 @@
 
 - Sensor
 - Binary sensor
 - Switch
 - Button
 - Device trigger
 
+Each entity can associated to a device. See below for details.
+
 ### Binary sensor
 
 #### Usage
 
 The following example creates a binary sensor and sets its state:
 
 ```py
@@ -108,16 +95,15 @@
 from ha_mqtt_discoverable.sensors import Switch, SwitchInfo
 from paho.mqtt.client import Client, MQTTMessage
 
 # Configure the required parameters for the MQTT broker
 mqtt_settings = Settings.MQTT(host="localhost")
 
 # Information about the switch
-# If `command_topic` is defined, it will receive state updates from HA
-switch_info = SwitchInfo(name="test", command_topic="command")
+switch_info = SwitchInfo(name="test")
 
 settings = Settings(mqtt=mqtt_settings, entity=switch_info)
 
 # To receive state commands from HA, define a callback function:
 def my_callback(client: Client, user_data, message: MQTTMessage):
     payload = message.payload.decode()
     logging.info(f"Received {payload} from HA")
@@ -131,14 +117,51 @@
 
 # Change the state of the sensor, publishing an MQTT message that gets picked up by HA
 my_switch.on()
 my_switch.off()
 
 ```
 
+### Text
+
+The text is an `helper entity`, showing an input field in the HA UI that the user can interact with.
+It is possible to act upon reception of the inputted text by defining a `callback` function, as the following example shows:
+
+#### Usage
+
+```py
+from ha_mqtt_discoverable import Settings
+from ha_mqtt_discoverable.sensors import Text, TextInfo
+from paho.mqtt.client import Client, MQTTMessage
+
+# Configure the required parameters for the MQTT broker
+mqtt_settings = Settings.MQTT(host="localhost")
+
+# Information about the `text` entity
+text_info = TextInfo(name="test")
+
+settings = Settings(mqtt=mqtt_settings, entity=switch_info)
+
+# To receive text updates from HA, define a callback function:
+def my_callback(client: Client, user_data, message: MQTTMessage):
+    text = message.payload.decode()
+    logging.info(f"Received {text} from HA")
+    # Your custom code...
+
+# Define an optional object to be passed back to the callback
+user_data = "Some custom data"
+
+# Instantiate the text
+my_text = Text(settings, my_callback, user_data)
+
+# Change the text displayed in HA UI, publishing an MQTT message that gets picked up by HA
+my_text.set_text("Some awesome text")
+
+```
+
 ## Device
 From the [Home Assistant documentation](https://developers.home-assistant.io/docs/device_registry_index):
 > A device is a special entity in Home Assistant that is represented by one or more entities.
 A device is automatically created when an entity defines its `device` property.
 A device will be matched up with an existing device via supplied identifiers or connections, like serial numbers or MAC addresses.
 
 ### Usage
@@ -221,8 +244,7 @@
 ## Contributors
 
 <a href="https://github.com/unixorn/ha-mqtt-discoverable/graphs/contributors">
   <img src="https://contributors-img.web.app/image?repo=unixorn/ha-mqtt-discoverable" />
 </a>
 
 Made with [contributors-img](https://contributors-img.web.app).
-
```

