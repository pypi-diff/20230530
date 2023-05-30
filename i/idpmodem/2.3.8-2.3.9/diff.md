# Comparing `tmp/idpmodem-2.3.8.tar.gz` & `tmp/idpmodem-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idpmodem-2.3.8.tar", max compression
+gzip compressed data, was "idpmodem-2.3.9.tar", max compression
```

## Comparing `idpmodem-2.3.8.tar` & `idpmodem-2.3.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    10763 2021-09-26 16:07:24.162483 idpmodem-2.3.8/LICENSE
--rw-r--r--   0        0        0     2017 2022-06-21 22:15:20.012649 idpmodem-2.3.8/README.md
--rw-r--r--   0        0        0      304 2023-03-26 17:53:16.586339 idpmodem-2.3.8/idpmodem/__init__.py
--rw-r--r--   0        0        0       40 2022-07-15 21:11:00.743064 idpmodem-2.3.8/idpmodem/asyncio/__init__.py
--rw-r--r--   0        0        0     8102 2022-04-19 10:57:07.964213 idpmodem-2.3.8/idpmodem/asyncio/atcommand.py
--rw-r--r--   0        0        0    48406 2022-04-19 10:56:23.766312 idpmodem-2.3.8/idpmodem/asyncio/atcommand_async.py
--rw-r--r--   0        0        0    38915 2023-03-26 17:30:16.859025 idpmodem-2.3.8/idpmodem/asyncio/modem.py
--rw-r--r--   0        0        0      616 2022-04-18 16:50:03.044139 idpmodem-2.3.8/idpmodem/aterror.py
--rw-r--r--   0        0        0       69 2022-06-21 22:04:05.752050 idpmodem-2.3.8/idpmodem/codecs/__init__.py
--rw-r--r--   0        0        0      217 2022-12-22 22:48:50.621272 idpmodem-2.3.8/idpmodem/codecs/common_mdf.py
--rw-r--r--   0        0        0      545 2022-12-22 22:41:12.204297 idpmodem-2.3.8/idpmodem/codecs/common_message_format/__init__.py
--rw-r--r--   0        0        0     3401 2022-12-22 22:35:49.340483 idpmodem-2.3.8/idpmodem/codecs/common_message_format/base.py
--rw-r--r--   0        0        0      616 2022-12-22 20:53:20.689493 idpmodem-2.3.8/idpmodem/codecs/common_message_format/constants.py
--rw-r--r--   0        0        0      242 2022-12-22 21:17:44.284480 idpmodem-2.3.8/idpmodem/codecs/common_message_format/fields/__init__.py
--rw-r--r--   0        0        0     9064 2022-12-22 21:52:45.125084 idpmodem-2.3.8/idpmodem/codecs/common_message_format/fields/array_field.py
--rw-r--r--   0        0        0     3556 2022-12-23 13:40:54.325794 idpmodem-2.3.8/idpmodem/codecs/common_message_format/fields/base_field.py
--rw-r--r--   0        0        0     2597 2022-12-23 13:42:03.479625 idpmodem-2.3.8/idpmodem/codecs/common_message_format/fields/boolean_field.py
--rw-r--r--   0        0        0     7592 2022-12-23 13:52:28.617274 idpmodem-2.3.8/idpmodem/codecs/common_message_format/fields/data_field.py
--rw-r--r--   0        0        0     5770 2023-04-18 11:20:30.155385 idpmodem-2.3.8/idpmodem/codecs/common_message_format/fields/enum_field.py
--rw-r--r--   0        0        0     1120 2022-12-22 20:09:24.081950 idpmodem-2.3.8/idpmodem/codecs/common_message_format/fields/helpers.py
--rw-r--r--   0        0        0     9018 2022-12-23 15:07:32.713822 idpmodem-2.3.8/idpmodem/codecs/common_message_format/fields/integer_field.py
--rw-r--r--   0        0        0     4915 2022-12-23 13:52:13.860341 idpmodem-2.3.8/idpmodem/codecs/common_message_format/fields/string_field.py
--rw-r--r--   0        0        0     3198 2022-12-22 21:58:21.526690 idpmodem-2.3.8/idpmodem/codecs/common_message_format/message_definitions.py
--rw-r--r--   0        0        0     7102 2022-12-22 22:17:34.077694 idpmodem-2.3.8/idpmodem/codecs/common_message_format/messages.py
--rw-r--r--   0        0        0     4858 2022-12-22 21:59:38.807257 idpmodem-2.3.8/idpmodem/codecs/common_message_format/services.py
--rw-r--r--   0        0        0    13754 2023-03-26 17:30:20.143711 idpmodem-2.3.8/idpmodem/constants.py
--rw-r--r--   0        0        0     3194 2022-06-22 21:25:43.836758 idpmodem-2.3.8/idpmodem/crcxmodem.py
--rw-r--r--   0        0        0     2576 2022-06-22 21:23:44.104600 idpmodem-2.3.8/idpmodem/helpers.py
--rw-r--r--   0        0        0    13509 2022-04-21 01:33:30.905231 idpmodem-2.3.8/idpmodem/location.py
--rw-r--r--   0        0        0     3527 2023-03-27 15:00:37.391287 idpmodem-2.3.8/idpmodem/propertycache.py
--rw-r--r--   0        0        0     7628 2022-04-19 10:47:54.958690 idpmodem-2.3.8/idpmodem/s_registers.py
--rw-r--r--   0        0        0       57 2022-06-21 22:05:00.325962 idpmodem-2.3.8/idpmodem/threaded/__init__.py
--rw-r--r--   0        0        0    15120 2023-03-26 03:53:24.878893 idpmodem-2.3.8/idpmodem/threaded/atcommand.py
--rw-r--r--   0        0        0    61530 2023-05-26 20:32:15.362494 idpmodem-2.3.8/idpmodem/threaded/modem.py
--rw-r--r--   0        0        0      897 2023-05-26 20:32:55.699150 idpmodem-2.3.8/pyproject.toml
--rw-r--r--   0        0        0     3011 2023-05-26 20:33:03.615830 idpmodem-2.3.8/setup.py
--rw-r--r--   0        0        0     2867 2023-05-26 20:33:03.616133 idpmodem-2.3.8/PKG-INFO
+-rw-r--r--   0        0        0    10763 2021-09-26 16:07:24.162483 idpmodem-2.3.9/LICENSE
+-rw-r--r--   0        0        0     2017 2022-06-21 22:15:20.012649 idpmodem-2.3.9/README.md
+-rw-r--r--   0        0        0      304 2023-03-26 17:53:16.586339 idpmodem-2.3.9/idpmodem/__init__.py
+-rw-r--r--   0        0        0       40 2022-07-15 21:11:00.743064 idpmodem-2.3.9/idpmodem/asyncio/__init__.py
+-rw-r--r--   0        0        0     8102 2022-04-19 10:57:07.964213 idpmodem-2.3.9/idpmodem/asyncio/atcommand.py
+-rw-r--r--   0        0        0    48406 2022-04-19 10:56:23.766312 idpmodem-2.3.9/idpmodem/asyncio/atcommand_async.py
+-rw-r--r--   0        0        0    38915 2023-03-26 17:30:16.859025 idpmodem-2.3.9/idpmodem/asyncio/modem.py
+-rw-r--r--   0        0        0      616 2022-04-18 16:50:03.044139 idpmodem-2.3.9/idpmodem/aterror.py
+-rw-r--r--   0        0        0       69 2022-06-21 22:04:05.752050 idpmodem-2.3.9/idpmodem/codecs/__init__.py
+-rw-r--r--   0        0        0      217 2022-12-22 22:48:50.621272 idpmodem-2.3.9/idpmodem/codecs/common_mdf.py
+-rw-r--r--   0        0        0      545 2022-12-22 22:41:12.204297 idpmodem-2.3.9/idpmodem/codecs/common_message_format/__init__.py
+-rw-r--r--   0        0        0     3401 2022-12-22 22:35:49.340483 idpmodem-2.3.9/idpmodem/codecs/common_message_format/base.py
+-rw-r--r--   0        0        0      616 2022-12-22 20:53:20.689493 idpmodem-2.3.9/idpmodem/codecs/common_message_format/constants.py
+-rw-r--r--   0        0        0      242 2022-12-22 21:17:44.284480 idpmodem-2.3.9/idpmodem/codecs/common_message_format/fields/__init__.py
+-rw-r--r--   0        0        0     9064 2022-12-22 21:52:45.125084 idpmodem-2.3.9/idpmodem/codecs/common_message_format/fields/array_field.py
+-rw-r--r--   0        0        0     3556 2022-12-23 13:40:54.325794 idpmodem-2.3.9/idpmodem/codecs/common_message_format/fields/base_field.py
+-rw-r--r--   0        0        0     2597 2022-12-23 13:42:03.479625 idpmodem-2.3.9/idpmodem/codecs/common_message_format/fields/boolean_field.py
+-rw-r--r--   0        0        0     7592 2022-12-23 13:52:28.617274 idpmodem-2.3.9/idpmodem/codecs/common_message_format/fields/data_field.py
+-rw-r--r--   0        0        0     5770 2023-04-18 11:20:30.155385 idpmodem-2.3.9/idpmodem/codecs/common_message_format/fields/enum_field.py
+-rw-r--r--   0        0        0     1120 2022-12-22 20:09:24.081950 idpmodem-2.3.9/idpmodem/codecs/common_message_format/fields/helpers.py
+-rw-r--r--   0        0        0     9018 2022-12-23 15:07:32.713822 idpmodem-2.3.9/idpmodem/codecs/common_message_format/fields/integer_field.py
+-rw-r--r--   0        0        0     4915 2022-12-23 13:52:13.860341 idpmodem-2.3.9/idpmodem/codecs/common_message_format/fields/string_field.py
+-rw-r--r--   0        0        0     3198 2022-12-22 21:58:21.526690 idpmodem-2.3.9/idpmodem/codecs/common_message_format/message_definitions.py
+-rw-r--r--   0        0        0     7102 2022-12-22 22:17:34.077694 idpmodem-2.3.9/idpmodem/codecs/common_message_format/messages.py
+-rw-r--r--   0        0        0     4858 2022-12-22 21:59:38.807257 idpmodem-2.3.9/idpmodem/codecs/common_message_format/services.py
+-rw-r--r--   0        0        0    13831 2023-05-30 11:36:37.797638 idpmodem-2.3.9/idpmodem/constants.py
+-rw-r--r--   0        0        0     3194 2022-06-22 21:25:43.836758 idpmodem-2.3.9/idpmodem/crcxmodem.py
+-rw-r--r--   0        0        0     2576 2022-06-22 21:23:44.104600 idpmodem-2.3.9/idpmodem/helpers.py
+-rw-r--r--   0        0        0    13509 2022-04-21 01:33:30.905231 idpmodem-2.3.9/idpmodem/location.py
+-rw-r--r--   0        0        0     3527 2023-03-27 15:00:37.391287 idpmodem-2.3.9/idpmodem/propertycache.py
+-rw-r--r--   0        0        0     7628 2022-04-19 10:47:54.958690 idpmodem-2.3.9/idpmodem/s_registers.py
+-rw-r--r--   0        0        0       57 2022-06-21 22:05:00.325962 idpmodem-2.3.9/idpmodem/threaded/__init__.py
+-rw-r--r--   0        0        0    15120 2023-03-26 03:53:24.878893 idpmodem-2.3.9/idpmodem/threaded/atcommand.py
+-rw-r--r--   0        0        0    61530 2023-05-26 20:32:15.362494 idpmodem-2.3.9/idpmodem/threaded/modem.py
+-rw-r--r--   0        0        0      897 2023-05-30 11:38:06.778914 idpmodem-2.3.9/pyproject.toml
+-rw-r--r--   0        0        0     3011 2023-05-30 11:38:39.771534 idpmodem-2.3.9/setup.py
+-rw-r--r--   0        0        0     2867 2023-05-30 11:38:39.771824 idpmodem-2.3.9/PKG-INFO
```

### Comparing `idpmodem-2.3.8/LICENSE` & `idpmodem-2.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.8/README.md` & `idpmodem-2.3.9/README.md`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.8/idpmodem/asyncio/atcommand.py` & `idpmodem-2.3.9/idpmodem/asyncio/atcommand.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.8/idpmodem/asyncio/atcommand_async.py` & `idpmodem-2.3.9/idpmodem/asyncio/atcommand_async.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.8/idpmodem/asyncio/modem.py` & `idpmodem-2.3.9/idpmodem/asyncio/modem.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.8/idpmodem/aterror.py` & `idpmodem-2.3.9/idpmodem/aterror.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.8/idpmodem/codecs/common_message_format/__init__.py` & `idpmodem-2.3.9/idpmodem/codecs/common_message_format/__init__.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.8/idpmodem/codecs/common_message_format/base.py` & `idpmodem-2.3.9/idpmodem/codecs/common_message_format/base.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.8/idpmodem/codecs/common_message_format/constants.py` & `idpmodem-2.3.9/idpmodem/codecs/common_message_format/constants.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.8/idpmodem/codecs/common_message_format/fields/array_field.py` & `idpmodem-2.3.9/idpmodem/codecs/common_message_format/fields/array_field.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.8/idpmodem/codecs/common_message_format/fields/base_field.py` & `idpmodem-2.3.9/idpmodem/codecs/common_message_format/fields/base_field.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.8/idpmodem/codecs/common_message_format/fields/boolean_field.py` & `idpmodem-2.3.9/idpmodem/codecs/common_message_format/fields/boolean_field.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.8/idpmodem/codecs/common_message_format/fields/data_field.py` & `idpmodem-2.3.9/idpmodem/codecs/common_message_format/fields/data_field.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.8/idpmodem/codecs/common_message_format/fields/enum_field.py` & `idpmodem-2.3.9/idpmodem/codecs/common_message_format/fields/enum_field.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.8/idpmodem/codecs/common_message_format/fields/helpers.py` & `idpmodem-2.3.9/idpmodem/codecs/common_message_format/fields/helpers.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.8/idpmodem/codecs/common_message_format/fields/integer_field.py` & `idpmodem-2.3.9/idpmodem/codecs/common_message_format/fields/integer_field.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.8/idpmodem/codecs/common_message_format/fields/string_field.py` & `idpmodem-2.3.9/idpmodem/codecs/common_message_format/fields/string_field.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.8/idpmodem/codecs/common_message_format/message_definitions.py` & `idpmodem-2.3.9/idpmodem/codecs/common_message_format/message_definitions.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.8/idpmodem/codecs/common_message_format/messages.py` & `idpmodem-2.3.9/idpmodem/codecs/common_message_format/messages.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.8/idpmodem/codecs/common_message_format/services.py` & `idpmodem-2.3.9/idpmodem/codecs/common_message_format/services.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.8/idpmodem/constants.py` & `idpmodem-2.3.9/idpmodem/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -284,14 +284,18 @@
     UTC_TIME_SYNC = 0b000100000000
     GNSS_FIX_TIMEOUT = 0b001000000000
     EVENT_TRACE_CACHED = 0b010000000000
     NETWORK_PING_ACKNOWLEDGED = 0b100000000000
 
 
 class TransmitterStatus(IdpEnum):
+    UNKNOWN = 0
+    RX_STOPPED = 1
+    RX_SEARCHING = 2
+    RX_ACQUIRING = 3
     RX_ONLY_NOT_REGISTERED = 4
     OK = 5
     SUSPENDED = 6
     MUTED = 7
     BLOCKED = 8
```

### Comparing `idpmodem-2.3.8/idpmodem/crcxmodem.py` & `idpmodem-2.3.9/idpmodem/crcxmodem.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.8/idpmodem/helpers.py` & `idpmodem-2.3.9/idpmodem/helpers.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.8/idpmodem/location.py` & `idpmodem-2.3.9/idpmodem/location.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.8/idpmodem/propertycache.py` & `idpmodem-2.3.9/idpmodem/propertycache.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.8/idpmodem/s_registers.py` & `idpmodem-2.3.9/idpmodem/s_registers.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.8/idpmodem/threaded/atcommand.py` & `idpmodem-2.3.9/idpmodem/threaded/atcommand.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.8/idpmodem/threaded/modem.py` & `idpmodem-2.3.9/idpmodem/threaded/modem.py`

 * *Files identical despite different names*

### Comparing `idpmodem-2.3.8/pyproject.toml` & `idpmodem-2.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "idpmodem"
-version = "2.3.8"
+version = "2.3.9"
 description = "A library for interfacing with an Inmarsat IsatData Pro satellite IoT modem using serial AT commands."
 authors = ["geoffbrucepayne <geoff.bruce-payne@inmarsat.com>"]
 license = "Apache2.0"
 repository = "https://github.com/inmarsat-enterprise.com/idpmodem"
 readme = "README.md"
 keywords = ["satellite", "iot"]
```

### Comparing `idpmodem-2.3.8/setup.py` & `idpmodem-2.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 {'': ['*']}
 
 install_requires = \
 ['aioserial==1.3.0', 'pyserial-asyncio>=0.6,<0.7', 'pyserial>=3.5,<4.0']
 
 setup_kwargs = {
     'name': 'idpmodem',
-    'version': '2.3.8',
+    'version': '2.3.9',
     'description': 'A library for interfacing with an Inmarsat IsatData Pro satellite IoT modem using serial AT commands.',
     'long_description': '# idpmodem\n\nPython library and samples for integrating with satellite Internet-of-Things \nmodems using the [Inmarsat](https://www.inmarsat.com) IsatData Pro ("IDP")\nnetwork.\n\n[Documentation](https://inmarsat-enterprise.github.io/idpmodem/)\n\n## Overview\n\nIDP is a store-and-forward satellite messaging technology with\nmessages up to 6400 bytes mobile-originated or 10000 bytes mobile-terminated.\n*Messages* are sent from or to a *Mobile* using its globally unique ID,\ntransacted through a *Mailbox* that provides authentication, encryption and\ndata segregation for cloud-based or enterprise client applications via a\nnetwork **Messaging API**.\n\nThe first byte of the message is referred to as the\n*Service Identification Number* (**SIN**) where values below 16 are reserved\nfor system use.  SIN is intended to capture the concept of embedded\nmicroservices used by an application.\n\nThe second byte of the message can optionally be defined as the\n*Message Identifier Number* (**MIN**) intended to support remote operations \nwithin each embedded microservice with defined binary formatting.\nThe MIN concept also supports the optional *Message Definition File* feature\nallowing an XML file to be applied which presents a JSON-tagged message\nstructure on the network API.\n\n### Terminology\n\n* MO = **Mobile Originated** aka *Return* aka *From-Mobile*\n  message sent from modem to cloud/enterprise application\n* MT = **Mobile Terminated** aka *Forward message* aka *To-Mobile*\n  message sent from cloud/enterprise application to modem\n\n## Modem operation\n\nUpon power-up or reset, the modem first acquires its location using \nGlobal Navigation Satellite Systems (GNSS).\nAfter getting its location, the modem tunes to the correct frequency, then\nregisters on the Inmarsat network.  Once registered it can communicate on the\nnetwork.\nProlonged obstruction of satellite signal will put the modem into a "blockage"\nstate from which it will automatically try to recover based on an algorithm\ninfluenced by its *power mode* setting.',
     'author': 'geoffbrucepayne',
     'author_email': 'geoff.bruce-payne@inmarsat.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/inmarsat-enterprise.com/idpmodem',
```

### Comparing `idpmodem-2.3.8/PKG-INFO` & `idpmodem-2.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idpmodem
-Version: 2.3.8
+Version: 2.3.9
 Summary: A library for interfacing with an Inmarsat IsatData Pro satellite IoT modem using serial AT commands.
 Home-page: https://github.com/inmarsat-enterprise.com/idpmodem
 License: Apache2.0
 Keywords: satellite,iot
 Author: geoffbrucepayne
 Author-email: geoff.bruce-payne@inmarsat.com
 Requires-Python: >=3.8,<4.0
```

