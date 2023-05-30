# Comparing `tmp/piwaterflow-0.5.6.tar.gz` & `tmp/piwaterflow-0.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piwaterflow-0.5.6.tar", last modified: Wed May 24 07:11:35 2023, max compression
+gzip compressed data, was "piwaterflow-0.5.7.tar", last modified: Tue May 30 06:16:16 2023, max compression
```

## Comparing `piwaterflow-0.5.6.tar` & `piwaterflow-0.5.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:11:35.532252 piwaterflow-0.5.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-24 07:11:35.532252 piwaterflow-0.5.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-24 07:11:23.000000 piwaterflow-0.5.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:11:35.528252 piwaterflow-0.5.6/piwaterflow/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-24 07:11:23.000000 piwaterflow-0.5.6/piwaterflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-24 07:11:23.000000 piwaterflow-0.5.6/piwaterflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-24 07:11:23.000000 piwaterflow-0.5.6/piwaterflow/config-template.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-24 07:11:23.000000 piwaterflow-0.5.6/piwaterflow/config_waterflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:11:35.532252 piwaterflow-0.5.6/piwaterflow/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 07:11:23.000000 piwaterflow-0.5.6/piwaterflow/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-24 07:11:23.000000 piwaterflow-0.5.6/piwaterflow/tests/test_000.py
--rw-r--r--   0 runner    (1001) docker     (123)    21323 2023-05-24 07:11:23.000000 piwaterflow-0.5.6/piwaterflow/waterflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:11:35.528252 piwaterflow-0.5.6/piwaterflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-24 07:11:35.000000 piwaterflow-0.5.6/piwaterflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-24 07:11:35.000000 piwaterflow-0.5.6/piwaterflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 07:11:35.000000 piwaterflow-0.5.6/piwaterflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-24 07:11:35.000000 piwaterflow-0.5.6/piwaterflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 07:11:35.000000 piwaterflow-0.5.6/piwaterflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 07:11:35.532252 piwaterflow-0.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-24 07:11:23.000000 piwaterflow-0.5.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:11:35.532252 piwaterflow-0.5.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 07:11:23.000000 piwaterflow-0.5.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-24 07:11:23.000000 piwaterflow-0.5.6/tests/test_000_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-24 07:11:23.000000 piwaterflow-0.5.6/tests/test_001_forward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-24 07:11:23.000000 piwaterflow-0.5.6/tests/test_002_reverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-24 07:11:23.000000 piwaterflow-0.5.6/tests/test_003_lock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:16:16.889270 piwaterflow-0.5.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-30 06:16:16.889270 piwaterflow-0.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-30 06:16:05.000000 piwaterflow-0.5.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:16:16.889270 piwaterflow-0.5.7/piwaterflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-30 06:16:05.000000 piwaterflow-0.5.7/piwaterflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-30 06:16:05.000000 piwaterflow-0.5.7/piwaterflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-30 06:16:05.000000 piwaterflow-0.5.7/piwaterflow/config-template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-30 06:16:05.000000 piwaterflow-0.5.7/piwaterflow/config_waterflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:16:16.889270 piwaterflow-0.5.7/piwaterflow/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:16:05.000000 piwaterflow-0.5.7/piwaterflow/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-30 06:16:05.000000 piwaterflow-0.5.7/piwaterflow/tests/test_000.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23464 2023-05-30 06:16:05.000000 piwaterflow-0.5.7/piwaterflow/waterflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:16:16.889270 piwaterflow-0.5.7/piwaterflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-30 06:16:16.000000 piwaterflow-0.5.7/piwaterflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-30 06:16:16.000000 piwaterflow-0.5.7/piwaterflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 06:16:16.000000 piwaterflow-0.5.7/piwaterflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-30 06:16:16.000000 piwaterflow-0.5.7/piwaterflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-30 06:16:16.000000 piwaterflow-0.5.7/piwaterflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 06:16:16.889270 piwaterflow-0.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-30 06:16:05.000000 piwaterflow-0.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:16:16.889270 piwaterflow-0.5.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 06:16:05.000000 piwaterflow-0.5.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-05-30 06:16:05.000000 piwaterflow-0.5.7/tests/test_000_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-30 06:16:05.000000 piwaterflow-0.5.7/tests/test_001_forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-05-30 06:16:05.000000 piwaterflow-0.5.7/tests/test_002_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-30 06:16:05.000000 piwaterflow-0.5.7/tests/test_003_lock.py
```

### Comparing `piwaterflow-0.5.6/PKG-INFO` & `piwaterflow-0.5.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piwaterflow
-Version: 0.5.6
+Version: 0.5.7
 Summary: Raspberry Pi Waterflow resilient system
 Home-page: https://github.com/Phornee/piwaterflow
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # PiWaterflow
         This is a resilient watering system, executed in a Raspberry Pi to control irrigation valves using relays.
```

### Comparing `piwaterflow-0.5.6/README.md` & `piwaterflow-0.5.7/README.md`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.6/piwaterflow/config_waterflow.py` & `piwaterflow-0.5.7/piwaterflow/config_waterflow.py`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.6/piwaterflow/tests/test_000.py` & `piwaterflow-0.5.7/piwaterflow/tests/test_000.py`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.6/piwaterflow/waterflow.py` & `piwaterflow-0.5.7/piwaterflow/waterflow.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 import os
 import time
 import shutil
 from datetime import datetime, timedelta
 from pathlib import Path
 import json
+import traceback
 
 try:
     from RPi import GPIO
 except (ModuleNotFoundError, ImportError, RuntimeError):
     from fake_rpigpio.RPi import GPIO
 
 from influxdb_wrapper import influxdb_factory
@@ -24,23 +25,24 @@
         At this moment it can support up to 2 valves, and 2 different programs alnog the day.
         Those programs/valves can be switched on/off in a forced way apart from the programs.
         This is autonomous, and could be controlled by directly changing the programs´configuration in the
         config.yml file.
         However, it can work together with the piwwwwaterflow package that serves a http page to remotely control
         the waterflow system.
     """
-    def __init__(self, template_config_path: str = None, dry_run: bool = False):
+    def __init__(self, template_config_path: str = None, fake_now: datetime = None, dry_run: bool = False):
         """__init__ of the function
         Args:
             template_config_path (str, optional): Template config to use. Defaults to None.
             dry_run (bool, optional): If true, it will just simulate, and wont make any change. Defaults to False.
         """
         self.homevar = os.path.join(str(Path.home()), 'var', self.class_name())
         
         self.dry_run = dry_run
+        self.curr_time = fake_now
 
         if dry_run:
             self.homevar = os.path.join(self.homevar, 'dryrun')
             if os.path.exists(self.homevar): # Only one instance of waterflow can run at a time, so this is safe
                 shutil.rmtree(self.homevar)
             if not os.path.exists(self.homevar):
                 os.makedirs(self.homevar)
@@ -52,28 +54,30 @@
             template_config_path = os.path.join(Path(__file__).parent.resolve(), './config-template.yml')
 
         self.config = WaterflowConfig(package_name=self.class_name(),
                                       template_path=template_config_path,
                                       config_file_name="config.yml",
                                       dry_run=dry_run)
 
+        self.events = []
+
         influx_conn_type = self.config['influxdbconn'].get('type', 'influx')
         self.conn = influxdb_factory(influx_conn_type)
         self.conn.openConn(self.config['influxdbconn'])
 
     def __del__(self):
-        if self.dry_run:
+        if self.dry_run and os.path.exists(self.homevar):
             shutil.rmtree(self.homevar)
 
     @classmethod
     def class_name(cls):
         """ class name """
         return "waterflow"
 
-    def _get_homevar_path(self, rel_path):
+    def get_homevar_path(self, rel_path):
         return os.path.join(self.homevar, rel_path)
 
     def update_config(self, programs: dict):
         """Updates the config file with modified programs
         Args:
             programs (dict): New programs to be modified
         """
@@ -109,34 +113,31 @@
     def _setup_gpio(self, valves):
         GPIO.setmode(GPIO.BOARD)
         GPIO.setwarnings(False)
 
         GPIO.setup(self.config['inverter_relay_pin'], GPIO.OUT)
         GPIO.output(self.config['inverter_relay_pin'], GPIO.LOW)
         GPIO.setup(self.config['external_ac_signal_pin'], GPIO.IN)
-        for valve in valves:
+        for valve in valves.values():
             GPIO.setup(valve['pin'], GPIO.OUT)
             GPIO.output(valve['pin'], GPIO.LOW)
 
-    def _recalc_next_program(self, last_program_time: datetime, today: datetime = None):
+    def _recalc_next_program(self, last_program_time: datetime):
         """ Calculates which is the next program to be executed, depending on the one previously executed
         Args:
             last_program_time: (datetime): Time in which previous program was executed (local aware to watering system)
             today (datetime, optional): Naive time to make the calculations. Normally used just for debug/unittesting
         Returns:
             tuple: time of next program, and program name
         """
         next_program_time = None
         program_name = None
 
         # Only used to get "today"... hour and minute will be overwritten for comparations with last_program_time
-        if today:
-            current_time = today.astimezone() # Make aware
-        else:
-            current_time = datetime.now().astimezone().replace(microsecond=0)
+        current_time = self.curr_time.astimezone().replace(microsecond=0)
 
         # Transform into a list to sort them
         prog_list = []
         for key, value in self.config['programs'].items():
             temp = value
             temp['name'] = key
             prog_list.append(temp)
@@ -164,77 +165,80 @@
                                                                   second=0).astimezone()
                     program_name = program['name']
                     break
 
         return next_program_time, program_name
 
     def _last_program_path(self):
-        return self._get_homevar_path('lastprogram.yml')
+        return self.get_homevar_path('lastprogram.yml')
 
-    def _read_last_program_time(self):
+    def _read_last_program_time(self, default: datetime = None):
         last_program_path = self._last_program_path()
 
         if os.path.exists(last_program_path):
             with open(last_program_path, 'r', encoding="utf-8") as file:
                 data = file.readlines()
                 last_program_time = self.str_to_time(data[0][:-1])
         else:
-            last_program_time = datetime.now().astimezone()
+            if default:
+                last_program_time = default.astimezone()
+            else:
+                last_program_time = datetime.now().astimezone()
             with open(last_program_path, 'w', encoding="utf-8") as file:
                 time_str = self.time_to_str(last_program_time)
                 file.writelines([time_str, time_str])
         return last_program_time
 
-    def _write_last_program_time(self, timelist):
+    def _write_last_program_time(self, time_last: datetime):
         last_program_path = self._last_program_path()
         with open(last_program_path, 'w', encoding="utf-8") as file:
-            file.writelines(timelist)
+            file.write(self.time_to_str(time_last))
 
     def get_lock(self):
         """
         This is to ensure that only one execution will run from cron at the same time
         Use file as a lock... not using DB locks because we want to maximize resiliency
         """
-        lock_path = self._get_homevar_path('lock')
+        lock_path = self.get_homevar_path('lock')
 
         if not os.path.exists(lock_path):
             with open(lock_path, 'w', encoding="utf-8"):
                 return True
         else:
             modified_time = datetime.fromtimestamp(os.path.getmtime(lock_path)).astimezone()
             if (datetime.now().astimezone() - modified_time) > timedelta(minutes=self.config['max_loop_time']):
-                self.userlogger.warning('Lock expired: Last loop ended abnormally?.')
+                self._add_event('LockExpired', self.time_to_str(modified_time))
                 Path(lock_path).touch()  # Previous token expired (previous loop crashed?)... we will retouch to retry
                 return True
         return False
 
     def release_lock(self):
         """Lock the loop... so the 2 loops cannot happen at the same time
         """
-        lock_path = self._get_homevar_path('lock')
+        lock_path = self.get_homevar_path('lock')
 
         if os.path.exists(lock_path):
             os.remove(lock_path)
         else:
-            self.userlogger.error("Could not release lock.")
+            self._add_event('CannotUnlock', None)
 
     def is_looping_correctly(self):
         """ Returns if a loop has succesfully run in the last x minutes
         Returns:
            bool: 
         """
         time_now = datetime.now().astimezone()
         return (time_now - self.last_loop_time()) < timedelta(minutes=self.config['max_loop_time'])
 
     def last_loop_time(self):
         """ Returns the last time in that a loop was succesfully executed
         Returns:
            datetime: Time in which last loop was executed
         """
-        token_path = self._get_homevar_path('token')
+        token_path = self.get_homevar_path('token')
         if os.path.exists(token_path):
             mod_time_since_epoc = os.path.getmtime(token_path)
             modification_time = datetime.fromtimestamp(mod_time_since_epoc).astimezone()
         else:
             modification_time = datetime.fromtimestamp(0) # Loop never run ok. Return oldest possible date
 
         return modification_time
@@ -249,64 +253,107 @@
 
         Returns:
             bool: If forced correctly
         """
         config = self.config.get_dict()
         if (type_force == 'program' and 0 <= value < len(config['programs'])) or \
            (type_force == 'valve' and 0 <= value < len(config['valves'])):
-            with open(self._get_homevar_path('force'), 'w', encoding="utf-8") as force_file:
+            with open(self.get_homevar_path('force'), 'w', encoding="utf-8") as force_file:
                 force_file.write(f'{{"type":"{type_force}","value":{value}}}')
                 return True
         else:
             return False
 
     def stop(self):
         """ Set the Stop-flag, so that the loop will stop the forced valve or program execution
         Returns:
             _type_: _description_
         """
-        stop_req_path = self._get_homevar_path('stop')
+        stop_req_path = self.get_homevar_path('stop')
         Path(stop_req_path).touch()
         return True
 
     def stop_remove(self):
         """ Returns if a stop has already been requested
         Returns:
            bool: Return true if a stop has been requested
         """
-        stop_req_path = self._get_homevar_path('stop')
+        stop_req_path = self.get_homevar_path('stop')
         return os.remove(stop_req_path)
 
     def stop_requested(self):
         """ Returns if a stop has already been requested
         Returns:
            bool: Return true if a stop has been requested
         """
-        stop_req_path = self._get_homevar_path('stop')
+        stop_req_path = self.get_homevar_path('stop')
         return os.path.exists(stop_req_path)
 
     def get_forced_info(self):
         """ Returns the forced info of the waterflow
         Returns:
             dict: Forced info
         """
-        force_file_path = self._get_homevar_path('force')
+        force_file_path = self.get_homevar_path('force')
         if os.path.exists(force_file_path):
             with open(force_file_path, 'r', encoding="utf-8") as force_file:
                 data = json.load(force_file)
                 return data
         else:
             return None
 
+    def _add_event(self, event: str, value):
+        self.events.append((self.time_to_str(datetime.now()), event, value))
+        
+        events_file_path = self.get_homevar_path('events')
+        with open(events_file_path, 'w', encoding="utf-8") as events_file:
+            json.dump(self.events, events_file)
+
+    def _get_event_string(self, event: tuple):
+        if event[1] == 'ExecValve':
+            result = f'Executing program {event[2]}.'
+        if event[1] == 'InverterON':
+            result = 'Inverter relay ON.'
+        if event[1] == 'InverterOFF':
+            result = 'Inverter relay OFF.'
+        if event[1] == 'ValveON':
+            result = f'Valve {event[2]} ON.'
+        if event[1] == 'ValveOFF':
+            result = f'Valve {event[2]} OFF.'
+        if event[1] == 'LastProg':
+            if event[2]:
+                result = f'Next program: {event[2]}.'
+            else:
+                result = 'NO active program!'
+        if event[1] == 'LockExpired':
+            result = 'Lock expired: Last loop ended abnormally?.'
+        if event[1] == 'CannotUnlock':
+            result = "Could not release lock."
+        if event[1] == 'ForcedProg':
+            result = f'Forced program {event[2]} executing now.'
+        if event[1] == 'ForcedValve':
+            result = f'Forced valve {event[2]} executing now.'
+        if event[1] == 'Stop':
+            result = 'Activity stopped.'
+        if event[1] == 'Exception':
+            result = f'Error looping: {event[2]}'
+
+
+        return result
+
     def get_log(self):
         """ Get the user log (not the debug log). This is the one the is shown in the wwwaterflow
         Returns:
             str: The whole user logs
         """
-        return self.userlogger.get_log()
+        log = ''
+        for event in self.events:
+            log += f'{self._get_event_string(event)}\n'
+        # return self.userlogger.get_log()
+        return log
 
     def _sleep(self, time_sleep):
         """ Sleep "time_sleep" time, but checks every 5 seconds if a stop has been requested
         Args:
             time_sleep (int): Number of seconds to sleep
         """
         time_count = 0
@@ -324,27 +371,29 @@
             ]
             self.conn.insert("piwaterflow", action_body)
 
     def _execute_valve(self, valve):
         # ------------------------------------
         # inverter_enable =  not GPIO.input(self.config['external_ac_signal_pin'])
         # if inverter_enable: # If we dont have external 220V power input, then activate inverter
+        self._add_event('ExecValve', valve)
+
         GPIO.output(self.config['inverter_relay_pin'], GPIO.HIGH)
-        self.userlogger.info('Inverter relay ON.')
+        self._add_event('InverterON', None)
         valve_pin = self.config['valves'][valve]['pin']
         GPIO.output(valve_pin, GPIO.HIGH)
-        self.userlogger.info(f'Valve {valve} ON.')
+        self._add_event('ValveON', valve)
 
         self._sleep(self.config['max_valve_time']*60)
 
         GPIO.output(valve_pin, GPIO.LOW)
-        self.userlogger.info(f'Valve {valve} OFF.')
+        self._add_event('ValveOFF', valve)
         # if inverter_enable: # If we dont have external 220V power input, then activate inverter
         GPIO.output(self.config['inverter_relay_pin'], GPIO.LOW)  # INVERTER always OFF after operations
-        self.userlogger.info('Inverter relay OFF.')
+        self._add_event('InverterOFF', None)
 
     def _skip_program(self):
         # print(self.config['humidity_threshold'])
         # if self.is_raspberry_pi():
         #     import adafruit_dht
         #     dhtSensor = adafruit_dht.DHT22(self.config['pin'])
         #     humidity = dhtSensor.humidity
@@ -358,127 +407,135 @@
         #    return False
         return False
 
     def _execute_program(self, program_name: str):
         """
         Works for regular programs, or forced ones (if program number is sent)
         """
-        self.userlogger.info(f'Executing program {program_name}.')
+        self._add_event('ExecProg', program_name)
         # inverter_enable =  not GPIO.input(self.config['external_ac_signal_pin'])
         # if inverter_enable: # If we don't have external 220V power input, then activate inverter
         GPIO.output(self.config['inverter_relay_pin'], GPIO.HIGH)
-        self.userlogger.info('Inverter relay ON.')
-        program_data = self._get_program_data(self.config['programs'][program_name])
-        for idx, valve_time in enumerate(program_data['valves_times']):
+        self._add_event('InverterON', None)
+        program_data = self.config['programs'][program_name]
+        for key, valve_time in program_data['valves_times'].items():
             if valve_time > 0 and not self.stop_requested():
-                valve_pin = self.config['valves'][idx]['pin']
+                valve_pin = self.config['valves'][key]['pin']
                 GPIO.output(valve_pin, GPIO.HIGH)
-                self.userlogger.info(f'Valve {idx} ON.')
+                self._add_event('ValveON', key)
 
-                self._sleep(valve_time * 60)
+                # If dry run, then we fast forward the sleep
+                if not self.dry_run:
+                    self._sleep(valve_time * 60)
 
                 GPIO.output(valve_pin, GPIO.LOW)
-                self.userlogger.info(f'Valve {idx} OFF.')
+                self._add_event('ValveOFF', key)
             else:
-                self.userlogger.info(f'Valve {idx} Skipped.')
+                self._add_event('ValveSkip', key)
         # if inverter_enable: # If we dont have external 220V power input, then activate inverter
         GPIO.output(self.config['inverter_relay_pin'], GPIO.LOW)  # INVERTER always OFF after operations
-        self.userlogger.info('Inverter relay OFF.')
+        self._add_event('InverterOFF', None)
 
-    def _log_next_program_time(self, current_time):
+    def _log_next_program_time(self):
 
-        log = self.userlogger.get_log()
+        # log = self.userlogger.get_log()
 
-        lines = log.split('\n')
+        # lines = log.split('\n')
 
-        new_next_program_time, _ = self._recalc_next_program(current_time)
+        new_next_program_time, _ = self._recalc_next_program(self.curr_time)
 
         if new_next_program_time:
-            string_to_log = f"Next program: {self.time_to_str(new_next_program_time)}."
+            last_event_date = self.time_to_str(new_next_program_time)
+            # string_to_log = f"Next program: {self.time_to_str(new_next_program_time)}."
         else:
-            string_to_log = 'NO active program!'
+            last_event_date = None
+            # string_to_log = 'NO active program!'
 
         # If previous log empty, or if last line outputs different information... log it. (to avoid duplicated logs)
-        if len(lines) <= 1 or (lines[-2][20:] != string_to_log and string_to_log != ''):
-            self.userlogger.info(string_to_log)
+        # if len(lines) <= 1 or (lines[-2][20:] != string_to_log and string_to_log != ''):
+        #     self.userlogger.info(string_to_log)
+
+        if not self.events or self.events[-1][1] != 'LastProg' or self.events[-1][2] != last_event_date:
+            self._add_event('LastProg', last_event_date)
 
-    def _execute_forced(self, forced_info: dict, curr_time: datetime):
+    def _execute_forced(self, forced_info: dict):
         forced_type = forced_info.get("type")
         forced_value = forced_info.get("value")
         if forced_type == "program":
-            self.userlogger.info(f'Forced program {forced_value} executing now.')
+            self._add_event('ForcedProg', forced_value)
             # ------------------------
             self._emit_action_metric(f'prog{forced_value}', True)
             self._execute_program(forced_value)
-            self._write_last_program_time(self.time_to_str(curr_time))
+            self._write_last_program_time(self.curr_time)
         elif forced_type == "valve":
+            self._add_event('ForcedValve', forced_value)
             # ------------------------
-            self._emit_action_metric('valve{forced_value}', True)
+            self._emit_action_metric(f'valve{forced_value}', True)
             self._execute_valve(forced_value)
 
-    def _check_and_execute_program(self, curr_time: datetime):
-        last_program_time = self._read_last_program_time()
+    def _check_and_execute_program(self):
+        last_program_time = self._read_last_program_time(default=self.curr_time)
         new_next_program, new_program_name = self._recalc_next_program(last_program_time)
         if new_next_program:
             # ------------------------
-            time_reached = curr_time >= new_next_program
-            time_threshold_exceeded = curr_time > (new_next_program + timedelta(minutes=self.config['max_loop_time']))
+            time_reached = self.curr_time >= new_next_program
+            time_threshold_exceeded = self.curr_time > (new_next_program + timedelta(minutes=self.config['max_loop_time']))
             skip_program = self._skip_program()
             # If we have reached the time of the new_program_time, BUT not by more than 10 minutes...
             if time_reached and not time_threshold_exceeded and not skip_program:
                 self._emit_action_metric(f'prog_{new_program_name}', False)
                 self._execute_program(new_program_name)
                 program_executed = True
             else:
                 program_executed = False
 
             if program_executed or skip_program or time_threshold_exceeded:
-                self._write_last_program_time(self.time_to_str(curr_time))
+                self._write_last_program_time(self.curr_time)
 
     def loop(self, date_now: datetime = None):
         """ Loop executed every x minutes... in crontab for example.
         Args:
             date_now (datetime): Naive date to consider the execution of the loop. 
                                  Normally used only for debuggin/unittesting
         """
         if self.get_lock():  # To ensure a single execution despite of cron overlapping
             try:
                 if date_now:
-                    curr_time = date_now.astimezone() # Make aware
+                    self.curr_time = date_now.astimezone() # Make aware
                 else:
-                    curr_time = datetime.now().astimezone()
+                    self.curr_time = datetime.now().astimezone()
                 forced_info = self.get_forced_info()
 
                 if not self.stop_requested():
                     self.debuglogger.info('Looping...')
                     self._setup_gpio(self.config['valves'])
 
                     if forced_info:
-                        self._execute_forced(forced_info, curr_time)
+                        self._execute_forced(forced_info)
                     else:
-                        self._check_and_execute_program(curr_time)
+                        self._check_and_execute_program()
                 else:
                     self.debuglogger.info('Loop skipped (Stop request).')
-                    self.userlogger.info('Activity stopped.')
+                    self._add_event('Stop', None)
                     self._emit_action_metric('Stop', True)
                     self.stop_remove()
 
                 if forced_info:
                     # Remove force token file
                     os.remove(os.path.join(self.homevar, 'force'))
 
                 # Recalc next program time
-                self._log_next_program_time(curr_time)
+                self._log_next_program_time()
 
                 # Updates "modified" time AT THE END, so that we can keep track about waterflow looping SUCCESFULLY.
                 token_path = os.path.join(self.homevar, 'token')
                 Path(token_path).touch()
 
             except Exception as ex:
-                self.debuglogger.error(f'Exception looping: {str(ex)}')
-                self.userlogger.error(f'Exception looping: {str(ex)}')
+                self.debuglogger.error(f'Exception looping: {str(ex)} | Stack: {traceback.format_exc()}')
+                self._add_event('Exception', str(ex))
                 raise RuntimeError(ex) from ex
             finally:
                 GPIO.cleanup()
                 self.release_lock()
         else:
             self.debuglogger.error('Loop executed while locked by previous execution.')
```

### Comparing `piwaterflow-0.5.6/piwaterflow.egg-info/PKG-INFO` & `piwaterflow-0.5.7/piwaterflow.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piwaterflow
-Version: 0.5.6
+Version: 0.5.7
 Summary: Raspberry Pi Waterflow resilient system
 Home-page: https://github.com/Phornee/piwaterflow
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # PiWaterflow
         This is a resilient watering system, executed in a Raspberry Pi to control irrigation valves using relays.
```

### Comparing `piwaterflow-0.5.6/setup.py` & `piwaterflow-0.5.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="piwaterflow",
-    version="0.5.6",
+    version="0.5.7",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Raspberry Pi Waterflow resilient system",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/piwaterflow",
     packages=setuptools.find_packages(),
```

### Comparing `piwaterflow-0.5.6/tests/test_001_forward.py` & `piwaterflow-0.5.7/tests/test_001_forward.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,38 +7,39 @@
 
 
 class Testing(unittest.TestCase):
     """ Unittesting class
     """
     def setUp(self):
         template_config_path = f'{Path(__file__).parent}/data/config-template.yml'
-        self.waterflow = Waterflow(template_config_path=template_config_path, dry_run=True)
+        self.waterflow = Waterflow(template_config_path=template_config_path,
+                                   fake_now = Waterflow.str_to_time('2023-04-27 00:01:00'),
+                                   dry_run=True)
 
     def test_0011_recalc_next_program(self):
         """ Test the recalc_next_program function
         """
         last_program_time = Waterflow.str_to_time('2023-04-26 23:30:27')
-        fake_now = Waterflow.str_to_time('2023-04-27 00:01:00')
-        time_prog, program_name = self.waterflow._recalc_next_program(last_program_time, fake_now) # pylint: disable=protected-access
+        time_prog, program_name = self.waterflow._recalc_next_program(last_program_time) # pylint: disable=protected-access
         self.assertTrue(time_prog == datetime(2023, 4, 27, 9, 51).astimezone())
         self.assertTrue(program_name == 'first')
 
         # Checks if _recalc_next_program works fine if last_program is today before first program
         last_program_time = Waterflow.str_to_time('2023-04-27 00:30:00')
-        time_prog, program_name = self.waterflow._recalc_next_program(last_program_time, fake_now) # pylint: disable=protected-access
+        time_prog, program_name = self.waterflow._recalc_next_program(last_program_time) # pylint: disable=protected-access
         self.assertTrue(time_prog == datetime(2023, 4, 27, 9, 51).astimezone())
         self.assertTrue(program_name == 'first')
 
         # Checks if _recalc_next_program works fine if last_program is between two programs
         last_program_time = Waterflow.str_to_time('2023-04-27 10:30:00')
-        time_prog, program_name = self.waterflow._recalc_next_program(last_program_time, fake_now) # pylint: disable=protected-access
+        time_prog, program_name = self.waterflow._recalc_next_program(last_program_time) # pylint: disable=protected-access
         self.assertTrue(time_prog == datetime(2023, 4, 27, 19, 4).astimezone())
         self.assertTrue(program_name == 'second')
 
         # Checks if _recalc_next_program works fine if last_program is after all  programs
         last_program_time = Waterflow.str_to_time('2023-04-27 23:59:00')
-        time_prog, program_name = self.waterflow._recalc_next_program(last_program_time, fake_now) # pylint: disable=protected-access
+        time_prog, program_name = self.waterflow._recalc_next_program(last_program_time) # pylint: disable=protected-access
         self.assertTrue(time_prog == datetime(2023, 4, 28, 9, 51).astimezone())
         self.assertTrue(program_name == 'first')
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `piwaterflow-0.5.6/tests/test_002_reverse.py` & `piwaterflow-0.5.7/tests/test_002_reverse.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,39 +7,40 @@
 
 
 class Testing(unittest.TestCase):
     """ Unittesting class
     """
     def setUp(self):
         template_config_path = f'{Path(__file__).parent}/data/config-template_reverse.yml'
-        self.waterflow = Waterflow(template_config_path=template_config_path, dry_run=True)
+        self.waterflow = Waterflow(template_config_path=template_config_path, 
+                                   fake_now=Waterflow.str_to_time('2023-04-27 00:01:00'),
+                                   dry_run=True)
 
     def test_0021_recalc_next_program(self):
         """ Test the recalc_next_program function
         """
         # Checks if _recalc_next_program works fine if last_program was "yesterday"
         last_program_time_utc = Waterflow.str_to_time('2023-04-26 23:30:27')
-        fake_now = Waterflow.str_to_time('2023-04-27 00:01:00')
-        time_utc, program_name = self.waterflow._recalc_next_program(last_program_time_utc, fake_now) # pylint: disable=protected-access
+        time_utc, program_name = self.waterflow._recalc_next_program(last_program_time_utc) # pylint: disable=protected-access
         self.assertTrue(time_utc == datetime(2023, 4, 27, 5, 6).astimezone())
         self.assertTrue(program_name == 'second')
 
         # Checks if _recalc_next_program works fine if last_program is today before first program
         last_program_time_utc = Waterflow.str_to_time('2023-04-27 00:30:00') # pylint: disable=protected-access
-        time_utc, program_name = self.waterflow._recalc_next_program(last_program_time_utc, fake_now) # pylint: disable=protected-access
+        time_utc, program_name = self.waterflow._recalc_next_program(last_program_time_utc) # pylint: disable=protected-access
         self.assertTrue(time_utc == datetime(2023, 4, 27, 5, 6).astimezone())
         self.assertTrue(program_name == 'second')
 
         # Checks if _recalc_next_program works fine if last_program is between two programs
         last_program_time_utc = Waterflow.str_to_time('2023-04-27 10:30:00') # pylint: disable=protected-access
-        time_utc, program_name = self.waterflow._recalc_next_program(last_program_time_utc, fake_now) # pylint: disable=protected-access
+        time_utc, program_name = self.waterflow._recalc_next_program(last_program_time_utc) # pylint: disable=protected-access
         self.assertTrue(time_utc == datetime(2023, 4, 27, 23, 30).astimezone())
         self.assertTrue(program_name == 'first')
 
         # Checks if _recalc_next_program works fine if last_program is after all  programs
         last_program_time_utc = Waterflow.str_to_time('2023-04-27 23:59:00') # pylint: disable=protected-access
-        time_utc, program_name = self.waterflow._recalc_next_program(last_program_time_utc, fake_now) # pylint: disable=protected-access
+        time_utc, program_name = self.waterflow._recalc_next_program(last_program_time_utc) # pylint: disable=protected-access
         self.assertTrue(time_utc == datetime(2023, 4, 28, 5, 6,).astimezone())
         self.assertTrue(program_name == 'second')
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `piwaterflow-0.5.6/tests/test_003_lock.py` & `piwaterflow-0.5.7/tests/test_003_lock.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         first_lock = self.waterflow.get_lock()
         self.assertTrue(first_lock)
 
         second_lock = self.waterflow.get_lock()
         self.assertFalse(second_lock)
 
         # Simulate lock expiring
-        lock_path = self.waterflow._get_homevar_path('lock') # pylint: disable=protected-access
+        lock_path = self.waterflow.get_homevar_path('lock')
         past_epoch = time.time() - 1260
         os.utime(lock_path, (past_epoch, past_epoch) ) # 21 minutes before to simulate expiring
         third_lock = self.waterflow.get_lock()
         self.assertTrue(third_lock)
 
 
 if __name__ == '__main__':
```

