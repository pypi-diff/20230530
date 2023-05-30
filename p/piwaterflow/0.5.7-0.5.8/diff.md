# Comparing `tmp/piwaterflow-0.5.7.tar.gz` & `tmp/piwaterflow-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piwaterflow-0.5.7.tar", last modified: Tue May 30 06:16:16 2023, max compression
+gzip compressed data, was "piwaterflow-0.5.8.tar", last modified: Tue May 30 11:50:51 2023, max compression
```

## Comparing `piwaterflow-0.5.7.tar` & `piwaterflow-0.5.8.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:16:16.889270 piwaterflow-0.5.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-30 06:16:16.889270 piwaterflow-0.5.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-30 06:16:05.000000 piwaterflow-0.5.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:16:16.889270 piwaterflow-0.5.7/piwaterflow/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-30 06:16:05.000000 piwaterflow-0.5.7/piwaterflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-30 06:16:05.000000 piwaterflow-0.5.7/piwaterflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-30 06:16:05.000000 piwaterflow-0.5.7/piwaterflow/config-template.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-30 06:16:05.000000 piwaterflow-0.5.7/piwaterflow/config_waterflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:16:16.889270 piwaterflow-0.5.7/piwaterflow/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:16:05.000000 piwaterflow-0.5.7/piwaterflow/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-30 06:16:05.000000 piwaterflow-0.5.7/piwaterflow/tests/test_000.py
--rw-r--r--   0 runner    (1001) docker     (123)    23464 2023-05-30 06:16:05.000000 piwaterflow-0.5.7/piwaterflow/waterflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:16:16.889270 piwaterflow-0.5.7/piwaterflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-30 06:16:16.000000 piwaterflow-0.5.7/piwaterflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-30 06:16:16.000000 piwaterflow-0.5.7/piwaterflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 06:16:16.000000 piwaterflow-0.5.7/piwaterflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-30 06:16:16.000000 piwaterflow-0.5.7/piwaterflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-30 06:16:16.000000 piwaterflow-0.5.7/piwaterflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 06:16:16.889270 piwaterflow-0.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-30 06:16:05.000000 piwaterflow-0.5.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:16:16.889270 piwaterflow-0.5.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:16:05.000000 piwaterflow-0.5.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-05-30 06:16:05.000000 piwaterflow-0.5.7/tests/test_000_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-30 06:16:05.000000 piwaterflow-0.5.7/tests/test_001_forward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-30 06:16:05.000000 piwaterflow-0.5.7/tests/test_002_reverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-30 06:16:05.000000 piwaterflow-0.5.7/tests/test_003_lock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:50:51.535875 piwaterflow-0.5.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-30 11:50:51.535875 piwaterflow-0.5.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-30 11:50:41.000000 piwaterflow-0.5.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:50:51.531875 piwaterflow-0.5.8/piwaterflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-30 11:50:41.000000 piwaterflow-0.5.8/piwaterflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-30 11:50:41.000000 piwaterflow-0.5.8/piwaterflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-30 11:50:41.000000 piwaterflow-0.5.8/piwaterflow/config-template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-30 11:50:41.000000 piwaterflow-0.5.8/piwaterflow/config_waterflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:50:51.535875 piwaterflow-0.5.8/piwaterflow/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:50:41.000000 piwaterflow-0.5.8/piwaterflow/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-30 11:50:41.000000 piwaterflow-0.5.8/piwaterflow/tests/test_000.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23249 2023-05-30 11:50:41.000000 piwaterflow-0.5.8/piwaterflow/waterflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:50:51.535875 piwaterflow-0.5.8/piwaterflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-30 11:50:51.000000 piwaterflow-0.5.8/piwaterflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-30 11:50:51.000000 piwaterflow-0.5.8/piwaterflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:50:51.000000 piwaterflow-0.5.8/piwaterflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-30 11:50:51.000000 piwaterflow-0.5.8/piwaterflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-30 11:50:51.000000 piwaterflow-0.5.8/piwaterflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 11:50:51.535875 piwaterflow-0.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-30 11:50:41.000000 piwaterflow-0.5.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:50:51.535875 piwaterflow-0.5.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:50:41.000000 piwaterflow-0.5.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-30 11:50:41.000000 piwaterflow-0.5.8/tests/test_000_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-30 11:50:41.000000 piwaterflow-0.5.8/tests/test_001_forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-30 11:50:41.000000 piwaterflow-0.5.8/tests/test_002_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-30 11:50:41.000000 piwaterflow-0.5.8/tests/test_003_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-30 11:50:41.000000 piwaterflow-0.5.8/tests/test_004_events.py
```

### Comparing `piwaterflow-0.5.7/PKG-INFO` & `piwaterflow-0.5.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piwaterflow
-Version: 0.5.7
+Version: 0.5.8
 Summary: Raspberry Pi Waterflow resilient system
 Home-page: https://github.com/Phornee/piwaterflow
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # PiWaterflow
         This is a resilient watering system, executed in a Raspberry Pi to control irrigation valves using relays.
```

### Comparing `piwaterflow-0.5.7/README.md` & `piwaterflow-0.5.8/README.md`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.7/piwaterflow/config_waterflow.py` & `piwaterflow-0.5.8/piwaterflow/config_waterflow.py`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.7/piwaterflow/tests/test_000.py` & `piwaterflow-0.5.8/piwaterflow/tests/test_000.py`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.7/piwaterflow/waterflow.py` & `piwaterflow-0.5.8/piwaterflow/waterflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             template_config_path = os.path.join(Path(__file__).parent.resolve(), './config-template.yml')
 
         self.config = WaterflowConfig(package_name=self.class_name(),
                                       template_path=template_config_path,
                                       config_file_name="config.yml",
                                       dry_run=dry_run)
 
-        self.events = []
+        self.events = self._read_events()
 
         influx_conn_type = self.config['influxdbconn'].get('type', 'influx')
         self.conn = influxdb_factory(influx_conn_type)
         self.conn.openConn(self.config['influxdbconn'])
 
     def __del__(self):
         if self.dry_run and os.path.exists(self.homevar):
@@ -299,19 +299,27 @@
                 data = json.load(force_file)
                 return data
         else:
             return None
 
     def _add_event(self, event: str, value):
         self.events.append((self.time_to_str(datetime.now()), event, value))
-        
+
         events_file_path = self.get_homevar_path('events')
         with open(events_file_path, 'w', encoding="utf-8") as events_file:
             json.dump(self.events, events_file)
 
+    def _read_events(self):
+        events = []
+        events_file_path = self.get_homevar_path('events')
+        if os.path.exists(events_file_path):
+            with open(events_file_path, 'r', encoding="utf-8") as events_file:
+                events = json.load(events_file)
+        return events
+
     def _get_event_string(self, event: tuple):
         if event[1] == 'ExecValve':
             result = f'Executing program {event[2]}.'
         if event[1] == 'InverterON':
             result = 'Inverter relay ON.'
         if event[1] == 'InverterOFF':
             result = 'Inverter relay OFF.'
@@ -344,15 +352,14 @@
         """ Get the user log (not the debug log). This is the one the is shown in the wwwaterflow
         Returns:
             str: The whole user logs
         """
         log = ''
         for event in self.events:
             log += f'{self._get_event_string(event)}\n'
-        # return self.userlogger.get_log()
         return log
 
     def _sleep(self, time_sleep):
         """ Sleep "time_sleep" time, but checks every 5 seconds if a stop has been requested
         Args:
             time_sleep (int): Number of seconds to sleep
         """
@@ -432,31 +439,20 @@
             else:
                 self._add_event('ValveSkip', key)
         # if inverter_enable: # If we dont have external 220V power input, then activate inverter
         GPIO.output(self.config['inverter_relay_pin'], GPIO.LOW)  # INVERTER always OFF after operations
         self._add_event('InverterOFF', None)
 
     def _log_next_program_time(self):
-
-        # log = self.userlogger.get_log()
-
-        # lines = log.split('\n')
-
         new_next_program_time, _ = self._recalc_next_program(self.curr_time)
 
         if new_next_program_time:
             last_event_date = self.time_to_str(new_next_program_time)
-            # string_to_log = f"Next program: {self.time_to_str(new_next_program_time)}."
         else:
             last_event_date = None
-            # string_to_log = 'NO active program!'
-
-        # If previous log empty, or if last line outputs different information... log it. (to avoid duplicated logs)
-        # if len(lines) <= 1 or (lines[-2][20:] != string_to_log and string_to_log != ''):
-        #     self.userlogger.info(string_to_log)
 
         if not self.events or self.events[-1][1] != 'LastProg' or self.events[-1][2] != last_event_date:
             self._add_event('LastProg', last_event_date)
 
     def _execute_forced(self, forced_info: dict):
         forced_type = forced_info.get("type")
         forced_value = forced_info.get("value")
```

### Comparing `piwaterflow-0.5.7/piwaterflow.egg-info/PKG-INFO` & `piwaterflow-0.5.8/piwaterflow.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piwaterflow
-Version: 0.5.7
+Version: 0.5.8
 Summary: Raspberry Pi Waterflow resilient system
 Home-page: https://github.com/Phornee/piwaterflow
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # PiWaterflow
         This is a resilient watering system, executed in a Raspberry Pi to control irrigation valves using relays.
```

### Comparing `piwaterflow-0.5.7/setup.py` & `piwaterflow-0.5.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="piwaterflow",
-    version="0.5.7",
+    version="0.5.8",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Raspberry Pi Waterflow resilient system",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/piwaterflow",
     packages=setuptools.find_packages(),
@@ -24,11 +24,11 @@
         "Topic :: Home Automation",
     ],
     install_requires=[
         'log_mgr>=0.0.2',
         'config_yml>=0.3.0',
         'RPi.GPIO>=0.7.0',
         'fake-rpigpio>=0.1.1',
-        'influxdb_wrapper>=0.0.3'
+        'influxdb_wrapper>=0.0.4'
     ],
     python_requires='>=3.6',
 )
```

### Comparing `piwaterflow-0.5.7/tests/test_000_loop.py` & `piwaterflow-0.5.8/tests/test_000_loop.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """ Unittesting """
 import unittest
 from pathlib import Path
 import gc
-import json
 
 from piwaterflow import Waterflow
 
 
 class Testing(unittest.TestCase):
     """ Unittesting class
     """
@@ -14,40 +13,33 @@
         template_config_path = f'{Path(__file__).parent}/data/config-template.yml'
         self.waterflow = Waterflow(template_config_path=template_config_path, dry_run=True)
 
     def tearDown(self):
         del self.waterflow
         gc.collect()
 
-    def _get_events(self):
-        events = None
-        events_file_path = self.waterflow.get_homevar_path('events')
-        with open(events_file_path, 'r', encoding="utf-8") as events_file:
-            events = json.load(events_file)
-        return events
-
     def test_0000_loop(self):
         """ Test the loop and main high-level functionalities. No program will run at that time
         """
         self.waterflow.loop(Waterflow.str_to_time('2023-05-27 08:30:00'))
 
-        events = self._get_events()
+        events = self.waterflow._read_events() # pylint: disable=protected-access
         if events:
             self.assertEqual(len(events), 1)
             self.assertTrue(events[0][1] == "LastProg" and events[0][2] == "2023-05-27 09:51:00")
         else:
             self.fail("not the right events generated.")
 
     def test_0001_loop(self):
         """ Test the loop and main high-level functionalities. Program will run at that time
         """
         self.waterflow._write_last_program_time(Waterflow.str_to_time('2023-05-26 23:59:00')) # pylint: disable=protected-access
         self.waterflow.loop(Waterflow.str_to_time('2023-05-27 09:52:00'))
 
-        events = self._get_events()
+        events = self.waterflow._read_events() # pylint: disable=protected-access
         if events:
             self.assertEqual(len(events), 8)
             self.assertTrue(events[0][1] == "ExecProg" and events[0][2] == "first")
             self.assertTrue(events[1][1] == "InverterON" and events[1][2] is None)
             self.assertTrue(events[2][1] == "ValveON" and events[2][2] == "main")
             self.assertTrue(events[3][1] == "ValveOFF" and events[3][2] == "main")
             self.assertTrue(events[4][1] == "ValveON" and events[4][2] == "grass")
```

### Comparing `piwaterflow-0.5.7/tests/test_001_forward.py` & `piwaterflow-0.5.8/tests/test_001_forward.py`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.7/tests/test_002_reverse.py` & `piwaterflow-0.5.8/tests/test_002_reverse.py`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.7/tests/test_003_lock.py` & `piwaterflow-0.5.8/tests/test_003_lock.py`

 * *Files identical despite different names*

