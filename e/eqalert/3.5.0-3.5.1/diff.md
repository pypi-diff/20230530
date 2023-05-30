# Comparing `tmp/eqalert-3.5.0.tar.gz` & `tmp/eqalert-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eqalert-3.5.0.tar", last modified: Sat May 27 02:24:26 2023, max compression
+gzip compressed data, was "eqalert-3.5.1.tar", last modified: Tue May 30 16:07:51 2023, max compression
```

## Comparing `eqalert-3.5.0.tar` & `eqalert-3.5.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:24:26.231595 eqalert-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11481 2023-05-27 02:24:26.231595 eqalert-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11196 2023-05-27 02:24:14.000000 eqalert-3.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:24:26.227595 eqalert-3.5.0/eqa/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:24:14.000000 eqalert-3.5.0/eqa/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    64902 2023-05-27 02:24:14.000000 eqalert-3.5.0/eqa/eqalert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:24:26.231595 eqalert-3.5.0/eqa/lib/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:24:14.000000 eqalert-3.5.0/eqa/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   102643 2023-05-27 02:24:14.000000 eqalert-3.5.0/eqa/lib/action.py
--rw-r--r--   0 runner    (1001) docker     (123)   469697 2023-05-27 02:24:14.000000 eqalert-3.5.0/eqa/lib/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    75113 2023-05-27 02:24:14.000000 eqalert-3.5.0/eqa/lib/curses.py
--rw-r--r--   0 runner    (1001) docker     (123)    84988 2023-05-27 02:24:14.000000 eqalert-3.5.0/eqa/lib/encounter.py
--rw-r--r--   0 runner    (1001) docker     (123)    33342 2023-05-27 02:24:14.000000 eqalert-3.5.0/eqa/lib/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-27 02:24:14.000000 eqalert-3.5.0/eqa/lib/log.py
--rw-r--r--   0 runner    (1001) docker     (123)   488406 2023-05-27 02:24:14.000000 eqalert-3.5.0/eqa/lib/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-27 02:24:14.000000 eqalert-3.5.0/eqa/lib/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-05-27 02:24:14.000000 eqalert-3.5.0/eqa/lib/sound.py
--rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-05-27 02:24:14.000000 eqalert-3.5.0/eqa/lib/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-27 02:24:14.000000 eqalert-3.5.0/eqa/lib/struct.py
--rw-r--r--   0 runner    (1001) docker     (123)    15533 2023-05-27 02:24:14.000000 eqalert-3.5.0/eqa/lib/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-27 02:24:14.000000 eqalert-3.5.0/eqa/lib/watch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:24:26.231595 eqalert-3.5.0/eqa/sound/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:24:14.000000 eqalert-3.5.0/eqa/sound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   192980 2023-05-27 02:24:14.000000 eqalert-3.5.0/eqa/sound/tick.wav
--rw-r--r--   0 runner    (1001) docker     (123)   192980 2023-05-27 02:24:14.000000 eqalert-3.5.0/eqa/sound/tock.wav
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 02:24:26.231595 eqalert-3.5.0/eqalert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11481 2023-05-27 02:24:26.000000 eqalert-3.5.0/eqalert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-27 02:24:26.000000 eqalert-3.5.0/eqalert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 02:24:26.000000 eqalert-3.5.0/eqalert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-27 02:24:26.000000 eqalert-3.5.0/eqalert.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-27 02:24:26.000000 eqalert-3.5.0/eqalert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-27 02:24:26.000000 eqalert-3.5.0/eqalert.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-27 02:24:26.231595 eqalert-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-27 02:24:14.000000 eqalert-3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:07:51.440298 eqalert-3.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11586 2023-05-30 16:07:51.440298 eqalert-3.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11301 2023-05-30 16:07:40.000000 eqalert-3.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:07:51.436298 eqalert-3.5.1/eqa/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:07:40.000000 eqalert-3.5.1/eqa/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    61839 2023-05-30 16:07:40.000000 eqalert-3.5.1/eqa/eqalert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:07:51.440298 eqalert-3.5.1/eqa/lib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:07:40.000000 eqalert-3.5.1/eqa/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102346 2023-05-30 16:07:40.000000 eqalert-3.5.1/eqa/lib/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)   468186 2023-05-30 16:07:40.000000 eqalert-3.5.1/eqa/lib/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76369 2023-05-30 16:07:40.000000 eqalert-3.5.1/eqa/lib/curses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85313 2023-05-30 16:07:40.000000 eqalert-3.5.1/eqa/lib/encounter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31696 2023-05-30 16:07:40.000000 eqalert-3.5.1/eqa/lib/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-30 16:07:40.000000 eqalert-3.5.1/eqa/lib/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)   488406 2023-05-30 16:07:40.000000 eqalert-3.5.1/eqa/lib/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-30 16:07:40.000000 eqalert-3.5.1/eqa/lib/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17117 2023-05-30 16:07:40.000000 eqalert-3.5.1/eqa/lib/sound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-05-30 16:07:40.000000 eqalert-3.5.1/eqa/lib/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-30 16:07:40.000000 eqalert-3.5.1/eqa/lib/struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15420 2023-05-30 16:07:40.000000 eqalert-3.5.1/eqa/lib/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-30 16:07:40.000000 eqalert-3.5.1/eqa/lib/watch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:07:51.440298 eqalert-3.5.1/eqa/sound/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:07:40.000000 eqalert-3.5.1/eqa/sound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   192980 2023-05-30 16:07:40.000000 eqalert-3.5.1/eqa/sound/tick.wav
+-rw-r--r--   0 runner    (1001) docker     (123)   192980 2023-05-30 16:07:40.000000 eqalert-3.5.1/eqa/sound/tock.wav
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:07:51.440298 eqalert-3.5.1/eqalert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11586 2023-05-30 16:07:51.000000 eqalert-3.5.1/eqalert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-30 16:07:51.000000 eqalert-3.5.1/eqalert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 16:07:51.000000 eqalert-3.5.1/eqalert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-30 16:07:51.000000 eqalert-3.5.1/eqalert.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-30 16:07:51.000000 eqalert-3.5.1/eqalert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-30 16:07:51.000000 eqalert-3.5.1/eqalert.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-30 16:07:51.440298 eqalert-3.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-30 16:07:40.000000 eqalert-3.5.1/setup.py
```

### Comparing `eqalert-3.5.0/PKG-INFO` & `eqalert-3.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eqalert
-Version: 3.5.0
+Version: 3.5.1
 Summary: Configurable and Context Driven Project 1999 Log Parser
 Home-page: https://github.com/mgeitz/eqalert
 Author: M Geitz
 Author-email: git@geitz.xyz
 License: GPL2
 Requires-Python: >=3.9.2
 Description-Content-Type: text/markdown
@@ -234,16 +234,16 @@
 
 ### Line Types
 
 Example configuration for a line type:
 ```
     "line_type_name": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
 ```
 
 #### Reaction Values
 
 ##### General
 - `false`: Disable alerting for this line type
@@ -267,15 +267,15 @@
 
 ###### Example 1
 Alert for the word `hey` when someone else `/says` it:
 
 ```
     "say": {
       "alert": {
-        "hey": "true"
+        "hey": true
       },
       "reaction": "alert",
       "sound": "hey"
     },
 ```
 
 ###### Example 2
@@ -294,25 +294,25 @@
 ###### Example 4
 Alert for a spell not taking hold only when grouped:
 
 ```
     "spell_not_hold": {
       "alert": {},
       "reaction": "group_only",
-      "sound": "true"
+      "sound": true
     },
 ```
 
 ###### Example 4
 Alert for the item `Hand Made Backpack` when someone else `/auctions` it and is selling:
 
 ```
     "auction_wts": {
       "alert": {
-        "Hand Made Backpack": "true"
+        "Hand Made Backpack": true
       },
       "reaction": "alert",
       "sound": "wow buy that"
     },
 ```
 
 > More examples can be referenced in the default config
@@ -320,27 +320,27 @@
 #### Alert Values
 
 ##### General
 - `false`: Disable alerting for the string (does not negate line type reactions)
 - `true`: Alert for the string
 
 ##### Context Driven
-- `solo`: Alert when solo, grouped, and raiding
-- `solo_only`: Alert only when solo
-- `group`: Alert when in a group and raiding
-- `group_only`: Alert only when grouped
-- `solo_group_only`: Alert only when not raiding
-- `raid`: Alert when in a raid
-- `afk`: Alert only when afk
+- `"solo"`: Alert when solo, grouped, and raiding
+- `"solo_only"`: Alert only when solo
+- `"group"`: Alert when in a group and raiding
+- `"group_only"`: Alert only when grouped
+- `"solo_group_only"`: Alert only when not raiding
+- `"raid"`: Alert when in a raid
+- `"afk"`: Alert only when afk
 
 #### Sound Values
 - `true`: When an alert is raised speak the entire line
 - `false`: Play no sound when an alert is raised
 
-> Any other sound value will be spoken as the audio trigger for that line type
+> Any other sound value (as a string) will be spoken as the audio trigger for that line type
 
 #### The all Line Type
 
 This line type behaves the same as any specific line type configuration, but configuration here will be used against all log lines.
 
 For example, the below configuration will alert if the word `help` is found in any line while in a raid context, even if that line isn't matched to a type by the parser.
 
@@ -355,14 +355,17 @@
 ```
 
 This can be helpful if you would like to alert for something not yet matched by the parser, though your [contribution](CONTRIBUTING.md#pull-requests) to a new line type match in the parser would also be welcome!
 
 ### Zones
 Zone data is stored in `config/zones.json`
 
+#### indoors
+Whether or not this zone is considered indoors.  Currently does nothing.
+
 #### raid_mode
 - `false`: If enabled, auto-disable raid mode in this zone
 - `true`: If enabled, auto-enable raid mode in this zone
 
 #### timer
 - `#`: The value in seconds to associate to a default timer in a given zone
```

### Comparing `eqalert-3.5.0/README.md` & `eqalert-3.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -223,16 +223,16 @@
 
 ### Line Types
 
 Example configuration for a line type:
 ```
     "line_type_name": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
 ```
 
 #### Reaction Values
 
 ##### General
 - `false`: Disable alerting for this line type
@@ -256,15 +256,15 @@
 
 ###### Example 1
 Alert for the word `hey` when someone else `/says` it:
 
 ```
     "say": {
       "alert": {
-        "hey": "true"
+        "hey": true
       },
       "reaction": "alert",
       "sound": "hey"
     },
 ```
 
 ###### Example 2
@@ -283,25 +283,25 @@
 ###### Example 4
 Alert for a spell not taking hold only when grouped:
 
 ```
     "spell_not_hold": {
       "alert": {},
       "reaction": "group_only",
-      "sound": "true"
+      "sound": true
     },
 ```
 
 ###### Example 4
 Alert for the item `Hand Made Backpack` when someone else `/auctions` it and is selling:
 
 ```
     "auction_wts": {
       "alert": {
-        "Hand Made Backpack": "true"
+        "Hand Made Backpack": true
       },
       "reaction": "alert",
       "sound": "wow buy that"
     },
 ```
 
 > More examples can be referenced in the default config
@@ -309,27 +309,27 @@
 #### Alert Values
 
 ##### General
 - `false`: Disable alerting for the string (does not negate line type reactions)
 - `true`: Alert for the string
 
 ##### Context Driven
-- `solo`: Alert when solo, grouped, and raiding
-- `solo_only`: Alert only when solo
-- `group`: Alert when in a group and raiding
-- `group_only`: Alert only when grouped
-- `solo_group_only`: Alert only when not raiding
-- `raid`: Alert when in a raid
-- `afk`: Alert only when afk
+- `"solo"`: Alert when solo, grouped, and raiding
+- `"solo_only"`: Alert only when solo
+- `"group"`: Alert when in a group and raiding
+- `"group_only"`: Alert only when grouped
+- `"solo_group_only"`: Alert only when not raiding
+- `"raid"`: Alert when in a raid
+- `"afk"`: Alert only when afk
 
 #### Sound Values
 - `true`: When an alert is raised speak the entire line
 - `false`: Play no sound when an alert is raised
 
-> Any other sound value will be spoken as the audio trigger for that line type
+> Any other sound value (as a string) will be spoken as the audio trigger for that line type
 
 #### The all Line Type
 
 This line type behaves the same as any specific line type configuration, but configuration here will be used against all log lines.
 
 For example, the below configuration will alert if the word `help` is found in any line while in a raid context, even if that line isn't matched to a type by the parser.
 
@@ -344,14 +344,17 @@
 ```
 
 This can be helpful if you would like to alert for something not yet matched by the parser, though your [contribution](CONTRIBUTING.md#pull-requests) to a new line type match in the parser would also be welcome!
 
 ### Zones
 Zone data is stored in `config/zones.json`
 
+#### indoors
+Whether or not this zone is considered indoors.  Currently does nothing.
+
 #### raid_mode
 - `false`: If enabled, auto-disable raid mode in this zone
 - `true`: If enabled, auto-enable raid mode in this zone
 
 #### timer
 - `#`: The value in seconds to associate to a default timer in a given zone
```

### Comparing `eqalert-3.5.0/eqa/eqalert.py` & `eqalert-3.5.1/eqa/eqalert.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,36 +40,40 @@
 import eqa.lib.sound as eqa_sound
 import eqa.lib.state as eqa_state
 import eqa.lib.struct as eqa_struct
 import eqa.lib.timer as eqa_timer
 import eqa.lib.watch as eqa_watch
 
 
-def startup(base_path):
+def startup(base_path, version):
     """Start things up"""
 
     try:
         # Make the main folder
         if not os.path.exists(base_path):
             print("Bootstrapping for first run . . .")
-            print("    - putting this stuff in " + base_path)
+            print("  Thanks for trying out EQ Alert")
+            print(
+                "  Please submit any bugs or issues to https://github.com/mgeitz/eqalert/issues"
+            )
+            print("    - putting everything in " + base_path)
             os.makedirs(base_path)
 
         # Make the config directory
         if not os.path.exists(base_path + "config/"):
-            print("    - making a place for way too many config files")
+            print("    - creating config directory")
             os.makedirs(base_path + "config/")
 
         # Make the config line alerts directory
         if not os.path.exists(base_path + "config/line-alerts/"):
-            print("    - what should we do with these lines?")
+            print("    - creating line alert config directory")
             os.makedirs(base_path + "config/line-alerts/")
 
         # Make Any Missing Config Files
-        eqa_config.init(base_path)
+        eqa_config.init(base_path, version)
 
         # Read config paths
         configs = eqa_config.read_config(base_path)
         log_path = configs.settings.config["settings"]["paths"]["eqalert_log"]
         data_path = configs.settings.config["settings"]["paths"]["data"]
         encounter_path = configs.settings.config["settings"]["paths"]["encounter"]
         sound_path = configs.settings.config["settings"]["paths"]["sound"]
@@ -83,78 +87,81 @@
                 "Please review paths in config/settings.json. Cannot find a character log: "
                 + str(configs.settings.config["settings"]["paths"]["everquest_logs"])
             )
             exit(1)
 
         # Make the log directory
         if not os.path.exists(log_path):
-            print("    - making a place for logs")
+            print("    - creating log directory")
             os.makedirs(log_path)
 
         # Set log file
         logging.basicConfig(filename=log_path + "eqalert.log", level=logging.INFO)
 
         # Make the debug directory
         if not os.path.exists(log_path + "debug/"):
-            print("    - making a place for optional debug logs")
+            print("    - creating debug log directory")
             os.makedirs(log_path + "debug/")
 
         # Make the sound directory
         if not os.path.exists(sound_path):
-            print("    - making a home for alert sounds")
+            print("    - creating sound directory")
             os.makedirs(sound_path)
         if not os.path.exists(sound_path + "tock.wav"):
             tock_path = pkg_resources.resource_filename("eqa", "sound/tock.wav")
             shutil.move(tock_path, sound_path + "tock.wav")
         if not os.path.exists(sound_path + "tick.wav"):
             tick_path = pkg_resources.resource_filename("eqa", "sound/tick.wav")
             shutil.move(tick_path, sound_path + "tick.wav")
 
         # Make the tmp sound directory
         if not os.path.exists(tmp_sound_path):
             os.makedirs(tmp_sound_path)
 
         # Make the data directory
         if not os.path.exists(data_path):
-            print("    - making a place for data")
+            print("    - creating data directory")
             os.makedirs(data_path)
 
         # Generate timers directory
         timers_save_directory = data_path + "timers/"
         if not os.path.exists(timers_save_directory):
+            print("    - creating timer data directory")
             os.makedirs(timers_save_directory)
 
         # Generate Spell Timers
         eq_spells_file_path = eq_files_path + "spells_us.txt"
         if os.path.isfile(eq_spells_file_path):
             eqa_config.update_spell_timers(data_path, eq_spells_file_path)
         else:
             print(
                 "Please review paths in config/settings.json. Unable to find spells_us.txt in "
                 + eq_spells_file_path
             )
 
         # Generate spell-lines.json
-        eqa_config.update_spell_lines(data_path)
+        eqa_config.update_spell_lines(data_path, version)
 
         # Generate spell-casters.json
-        eqa_config.update_spell_casters(data_path)
+        eqa_config.update_spell_casters(data_path, version)
 
-        # Generate Players File
+        # Generate Players List File
         player_data_file = data_path + "players.json"
         if not os.path.isfile(player_data_file):
-            eqa_config.generate_players_file(player_data_file)
+            eqa_config.generate_players_file(player_data_file, version)
+        else:
+            eqa_config.validate_players_file(player_data_file, version)
 
         # Make the encounter directory
         if not os.path.exists(encounter_path):
-            print("    - making a place for encounter logs")
+            print("    - creating encounter directory")
             os.makedirs(encounter_path)
 
         # Update config char_logs
-        eqa_config.update_logs(configs)
+        eqa_config.update_logs(configs, version)
 
         server = configs.settings.config["last_state"]["server"]
         char = configs.settings.config["last_state"]["character"]
         char_log = (
             configs.settings.config["settings"]["paths"]["everquest_logs"]
             + configs.characters.config["char_logs"][char + "_" + server]["file_name"]
         )
@@ -177,217 +184,225 @@
         )
         exit(1)
 
 
 def main():
     """Main method, does the good stuff"""
 
-    # Paths
-    home = os.path.expanduser("~")
-    base_path = home + "/.eqa/"
-
-    # Validate start
-    startup(base_path)
-
-    # Read in config and state
-    configs = eqa_config.read_config(base_path)
-    server = configs.settings.config["last_state"]["server"]
-    char = configs.settings.config["last_state"]["character"]
-    state = eqa_config.get_last_state(configs, char, server)
-    char_log = (
-        configs.settings.config["settings"]["paths"]["everquest_logs"]
-        + configs.characters.config["char_logs"][char + "_" + server]["file_name"]
-    )
+    try:
+        # Version string
+        version = str(pkg_resources.get_distribution("eqalert").version)
 
-    # Initialize curses
-    screen = eqa_curses.init(state)
+        # Paths
+        home = os.path.expanduser("~")
+        base_path = home + "/.eqa/"
 
-    # Thread Events
-    cfg_reload = threading.Event()
-    exit_flag = threading.Event()
-    change_char = threading.Event()
-
-    # Queues
-    action_q = queue.Queue()
-    display_q = queue.Queue()
-    encounter_q = queue.Queue()
-    keyboard_q = queue.Queue()
-    log_q = queue.Queue()
-    sound_q = queue.Queue()
-    system_q = queue.Queue()
-    timer_q = queue.Queue()
-
-    # Watch Log Directory
-    ## Consume log directory for newest log
-    ## Produce character update to system_q
-    process_watch = threading.Thread(
-        target=eqa_watch.process,
-        args=(state, configs, system_q, exit_flag, cfg_reload),
-    )
-    process_watch.daemon = True
-    process_watch.start()
+        # Validate start
+        startup(base_path, version)
 
-    # Read Log File
-    ## Consume char_log
-    ## Produce log_q
-    process_log = threading.Thread(
-        target=eqa_log.process,
-        args=(change_char, exit_flag, char_log, log_q),
-    )
-    process_log.daemon = True
-    process_log.start()
+        # Read in config and state
+        configs = eqa_config.read_config(base_path)
+        server = configs.settings.config["last_state"]["server"]
+        char = configs.settings.config["last_state"]["character"]
+        state = eqa_config.get_last_state(configs, char, server)
+        char_log = (
+            configs.settings.config["settings"]["paths"]["everquest_logs"]
+            + configs.characters.config["char_logs"][char + "_" + server]["file_name"]
+        )
 
-    # Parse Log Lines to Determine Line Type
-    ## Process log_q
-    ## Produce action_q
-    process_parse = threading.Thread(
-        target=eqa_parser.process, args=(exit_flag, log_q, action_q)
-    )
-    process_parse.daemon = True
-    process_parse.start()
+        # Initialize curses
+        screen = eqa_curses.init(state, version)
 
-    # Read Keyboard Events
-    ## Consume keyboard events
-    ## Produce keyboard_q
-    read_keys = threading.Thread(
-        target=eqa_keys.read, args=(exit_flag, keyboard_q, screen)
-    )
-    read_keys.daemon = True
-    read_keys.start()
+        # Thread Events
+        cfg_reload = threading.Event()
+        exit_flag = threading.Event()
+        change_char = threading.Event()
+
+        # Queues
+        action_q = queue.Queue()
+        display_q = queue.Queue()
+        encounter_q = queue.Queue()
+        keyboard_q = queue.Queue()
+        log_q = queue.Queue()
+        sound_q = queue.Queue()
+        system_q = queue.Queue()
+        timer_q = queue.Queue()
+
+        # Watch Log Directory
+        ## Consume log directory for newest log
+        ## Produce character update to system_q
+        process_watch = threading.Thread(
+            target=eqa_watch.process,
+            args=(state, configs, system_q, exit_flag, cfg_reload),
+        )
+        process_watch.daemon = True
+        process_watch.start()
 
-    # Act on Keyboard Events
-    ## Process keyboard_q
-    ## Produce display_q, system_q
-    process_keys = threading.Thread(
-        target=eqa_keys.process,
-        args=(
-            state,
-            configs,
-            display_q,
-            keyboard_q,
-            system_q,
-            cfg_reload,
-            exit_flag,
-        ),
-    )
-    process_keys.daemon = True
-    process_keys.start()
+        # Read Log File
+        ## Consume char_log
+        ## Produce log_q
+        process_log = threading.Thread(
+            target=eqa_log.process,
+            args=(change_char, exit_flag, char_log, log_q),
+        )
+        process_log.daemon = True
+        process_log.start()
 
-    # Act on Parsed Log Lines
-    ## Consume action_q
-    ## Produce display_q, encounter_q, sound_q, system_q, timer_q
-
-    ### Mute List
-    mute_list = []
-
-    process_action = threading.Thread(
-        target=eqa_action.process,
-        args=(
-            configs,
-            base_path,
-            state,
-            action_q,
-            encounter_q,
-            timer_q,
-            system_q,
-            display_q,
-            sound_q,
-            exit_flag,
-            cfg_reload,
-            mute_list,
-            change_char,
-        ),
-    )
-    process_action.daemon = True
-    process_action.start()
+        # Parse Log Lines to Determine Line Type
+        ## Process log_q
+        ## Produce action_q
+        process_parse = threading.Thread(
+            target=eqa_parser.process, args=(exit_flag, log_q, action_q)
+        )
+        process_parse.daemon = True
+        process_parse.start()
 
-    # Create Encounter Reports
-    ## Consume encounter_q
-    ## Produce display_q, system_q
-    process_encounter = threading.Thread(
-        target=eqa_encounter.process,
-        args=(
-            configs,
-            base_path,
-            encounter_q,
-            system_q,
-            display_q,
-            exit_flag,
-            cfg_reload,
-            state,
-        ),
-    )
-    process_encounter.daemon = True
-    process_encounter.start()
+        # Read Keyboard Events
+        ## Consume keyboard events
+        ## Produce keyboard_q
+        read_keys = threading.Thread(
+            target=eqa_keys.read, args=(exit_flag, keyboard_q, screen)
+        )
+        read_keys.daemon = True
+        read_keys.start()
 
-    # Create (many) Sounds
-    ## Consume sound_q
-    ## Produce sounds
-
-    ### Thread 1
-    process_sound_1 = threading.Thread(
-        target=eqa_sound.process, args=(configs, sound_q, exit_flag, cfg_reload, state)
-    )
-    process_sound_1.daemon = True
-    process_sound_1.start()
+        # Act on Keyboard Events
+        ## Process keyboard_q
+        ## Produce display_q, system_q
+        process_keys = threading.Thread(
+            target=eqa_keys.process,
+            args=(
+                state,
+                configs,
+                display_q,
+                keyboard_q,
+                system_q,
+                cfg_reload,
+                exit_flag,
+            ),
+        )
+        process_keys.daemon = True
+        process_keys.start()
 
-    ### Thread 2
-    process_sound_2 = threading.Thread(
-        target=eqa_sound.process, args=(configs, sound_q, exit_flag, cfg_reload, state)
-    )
-    process_sound_2.daemon = True
-    process_sound_2.start()
+        # Act on Parsed Log Lines
+        ## Consume action_q
+        ## Produce display_q, encounter_q, sound_q, system_q, timer_q
+
+        ### Mute List
+        mute_list = []
+
+        process_action = threading.Thread(
+            target=eqa_action.process,
+            args=(
+                configs,
+                base_path,
+                state,
+                action_q,
+                encounter_q,
+                timer_q,
+                system_q,
+                display_q,
+                sound_q,
+                exit_flag,
+                cfg_reload,
+                mute_list,
+                change_char,
+                version,
+            ),
+        )
+        process_action.daemon = True
+        process_action.start()
 
-    ### Thread 3
-    process_sound_3 = threading.Thread(
-        target=eqa_sound.process, args=(configs, sound_q, exit_flag, cfg_reload, state)
-    )
-    process_sound_3.daemon = True
-    process_sound_3.start()
+        # Create Encounter Reports
+        ## Consume encounter_q
+        ## Produce display_q, system_q
+        process_encounter = threading.Thread(
+            target=eqa_encounter.process,
+            args=(
+                configs,
+                base_path,
+                encounter_q,
+                system_q,
+                display_q,
+                exit_flag,
+                cfg_reload,
+                state,
+                version,
+            ),
+        )
+        process_encounter.daemon = True
+        process_encounter.start()
 
-    # Draw the TUI
-    ## Consume display_q
-    ## Produce pretty pictures
-    process_display = threading.Thread(
-        target=eqa_curses.display,
-        args=(screen, display_q, state, configs, exit_flag, cfg_reload),
-    )
-    process_display.daemon = True
-    process_display.start()
+        # Create (many) Sounds
+        ## Consume sound_q
+        ## Produce sounds
+
+        ### Thread 1
+        process_sound_1 = threading.Thread(
+            target=eqa_sound.process,
+            args=(configs, sound_q, exit_flag, cfg_reload, state),
+        )
+        process_sound_1.daemon = True
+        process_sound_1.start()
 
-    # Count Down the Time
-    ## Consume timer_q
-    ## Produce sound_q, display_q
-    process_timer = threading.Thread(
-        target=eqa_timer.process,
-        args=(
-            configs,
-            state,
-            timer_q,
-            sound_q,
-            display_q,
-            exit_flag,
-            cfg_reload,
-            change_char,
-        ),
-    )
-    process_timer.daemon = True
-    process_timer.start()
+        ### Thread 2
+        process_sound_2 = threading.Thread(
+            target=eqa_sound.process,
+            args=(configs, sound_q, exit_flag, cfg_reload, state),
+        )
+        process_sound_2.daemon = True
+        process_sound_2.start()
 
-    # Manage State and Config
-    ## Consume system_q
-    ## Produce a pleasant experience
-    try:
+        ### Thread 3
+        process_sound_3 = threading.Thread(
+            target=eqa_sound.process,
+            args=(configs, sound_q, exit_flag, cfg_reload, state),
+        )
+        process_sound_3.daemon = True
+        process_sound_3.start()
+
+        # Draw the TUI
+        ## Consume display_q
+        ## Produce pretty pictures
+        process_display = threading.Thread(
+            target=eqa_curses.display,
+            args=(screen, display_q, state, configs, exit_flag, cfg_reload, version),
+        )
+        process_display.daemon = True
+        process_display.start()
+
+        # Count Down the Time
+        ## Consume timer_q
+        ## Produce sound_q, display_q
+        process_timer = threading.Thread(
+            target=eqa_timer.process,
+            args=(
+                configs,
+                state,
+                timer_q,
+                sound_q,
+                display_q,
+                exit_flag,
+                cfg_reload,
+                change_char,
+            ),
+        )
+        process_timer.daemon = True
+        process_timer.start()
+
+        # Manage State and Config
+        ## Consume system_q
+        ## Produce a pleasant experience
         while not exit_flag.is_set():
             # Sleep between empty checks
             queue_size = system_q.qsize()
             if queue_size < 1:
                 time.sleep(0.01)
             else:
-                if state.debug == "true":
+                if state.debug:
                     eqa_settings.log("system_q depth: " + str(queue_size))
 
             # Check queue for message
             if not system_q.empty():
                 ## Read new message
                 new_message = system_q.get()
 
@@ -397,33 +412,33 @@
                     if new_message.tx == "zone":
                         state.set_zone(new_message.payload)
                         state.set_direction("unavailable")
                         state.set_loc([0.00, 0.00, 0.00])
                         eqa_config.set_last_state(state, configs)
                         display_q.put(
                             eqa_struct.display(
-                                eqa_settings.eqa_time(), "draw", "redraw", "null"
+                                eqa_settings.eqa_time(), "draw", "redraw", None
                             )
                         )
                     ### Update location
                     elif new_message.tx == "loc":
                         state.set_loc(new_message.payload)
                         eqa_config.set_last_state(state, configs)
                         display_q.put(
                             eqa_struct.display(
-                                eqa_settings.eqa_time(), "draw", "redraw", "null"
+                                eqa_settings.eqa_time(), "draw", "redraw", None
                             )
                         )
                     ### Update direction
                     elif new_message.tx == "direction":
                         state.set_direction(new_message.payload)
                         eqa_config.set_last_state(state, configs)
                         display_q.put(
                             eqa_struct.display(
-                                eqa_settings.eqa_time(), "draw", "redraw", "null"
+                                eqa_settings.eqa_time(), "draw", "redraw", None
                             )
                         )
                     ### Update afk status
                     elif new_message.tx == "afk":
                         system_afk(configs, state, display_q, new_message)
 
                     ### Update raid status
@@ -456,35 +471,35 @@
 
                     ### Update group status
                     elif new_message.tx == "group":
                         state.set_group(new_message.payload)
                         eqa_config.set_last_state(state, configs)
                         display_q.put(
                             eqa_struct.display(
-                                eqa_settings.eqa_time(), "draw", "redraw", "null"
+                                eqa_settings.eqa_time(), "draw", "redraw", None
                             )
                         )
 
                     ### Update group leader status
                     elif new_message.tx == "leader":
                         state.set_leader(new_message.payload)
                         eqa_config.set_last_state(state, configs)
                         display_q.put(
                             eqa_struct.display(
-                                eqa_settings.eqa_time(), "draw", "redraw", "null"
+                                eqa_settings.eqa_time(), "draw", "redraw", None
                             )
                         )
 
                     ### Update encumbered status
                     elif new_message.tx == "encumbered":
                         state.set_encumbered(new_message.payload)
                         eqa_config.set_last_state(state, configs)
                         display_q.put(
                             eqa_struct.display(
-                                eqa_settings.eqa_time(), "draw", "redraw", "null"
+                                eqa_settings.eqa_time(), "draw", "redraw", None
                             )
                         )
 
                     ### Update automatic timer status
                     elif new_message.tx == "timer":
                         system_timer(configs, state, display_q, sound_q, new_message)
 
@@ -496,42 +511,42 @@
 
                     ### Update bind status
                     elif new_message.tx == "bind":
                         state.set_bind(new_message.payload)
                         eqa_config.set_last_state(state, configs)
                         display_q.put(
                             eqa_struct.display(
-                                eqa_settings.eqa_time(), "draw", "redraw", "null"
+                                eqa_settings.eqa_time(), "draw", "redraw", None
                             )
                         )
                     ### Update level status
                     elif new_message.tx == "level":
                         state.set_level(new_message.payload)
                         eqa_config.set_last_state(state, configs)
                         display_q.put(
                             eqa_struct.display(
-                                eqa_settings.eqa_time(), "draw", "redraw", "null"
+                                eqa_settings.eqa_time(), "draw", "redraw", None
                             )
                         )
                     ### Update class status
                     elif new_message.tx == "class":
                         state.set_class(new_message.payload)
                         eqa_config.set_last_state(state, configs)
                         display_q.put(
                             eqa_struct.display(
-                                eqa_settings.eqa_time(), "draw", "redraw", "null"
+                                eqa_settings.eqa_time(), "draw", "redraw", None
                             )
                         )
                     ### Update guild status
                     elif new_message.tx == "guild":
                         state.set_guild(new_message.payload)
                         eqa_config.set_last_state(state, configs)
                         display_q.put(
                             eqa_struct.display(
-                                eqa_settings.eqa_time(), "draw", "redraw", "null"
+                                eqa_settings.eqa_time(), "draw", "redraw", None
                             )
                         )
                     ### Update mute status
                     elif new_message.tx == "mute":
                         system_mute(configs, state, display_q, sound_q, new_message)
 
                     ### Update character
@@ -641,14 +656,15 @@
                                     system_q,
                                     display_q,
                                     sound_q,
                                     exit_flag,
                                     cfg_reload,
                                     mute_list,
                                     change_char,
+                                    version,
                                 ),
                             )
                             process_action.daemon = True
                             process_action.start()
 
                             # Display notification
                             display_q.put(
@@ -660,15 +676,15 @@
                                     + state.char
                                     + " on "
                                     + state.server,
                                 )
                             )
                             display_q.put(
                                 eqa_struct.display(
-                                    eqa_settings.eqa_time(), "draw", "redraw", "null"
+                                    eqa_settings.eqa_time(), "draw", "redraw", None
                                 )
                             )
                         else:
                             display_q.put(
                                 eqa_struct.display(
                                     eqa_settings.eqa_time(),
                                     "event",
@@ -737,14 +753,15 @@
                             args=(
                                 screen,
                                 display_q,
                                 state,
                                 configs,
                                 exit_flag,
                                 cfg_reload,
+                                version,
                             ),
                         )
                         process_display.daemon = True
                         process_display.start()
 
                         #### Restart process_keys
                         process_keys = threading.Thread(
@@ -792,14 +809,15 @@
                                 base_path,
                                 encounter_q,
                                 system_q,
                                 display_q,
                                 exit_flag,
                                 cfg_reload,
                                 state,
+                                version,
                             ),
                         )
                         process_encounter.daemon = True
                         process_encounter.start()
 
                         #### Restart process_sound
 
@@ -906,107 +924,101 @@
 
 
 def system_raid(configs, state, display_q, sound_q, new_message):
     """Perform system tasks for raid behavior"""
 
     try:
         # Toggle raid state to true
-        if state.raid == "false" and new_message.rx == "toggle":
-            state.set_raid("true")
-            eqa_config.set_last_state(state, configs)
-            display_q.put(
-                eqa_struct.display(
-                    eqa_settings.eqa_time(),
-                    "event",
-                    "events",
-                    "Raid mode enabled",
+        if new_message.rx == "toggle":
+            if not state.raid:
+                state.set_raid(True)
+                eqa_config.set_last_state(state, configs)
+                display_q.put(
+                    eqa_struct.display(
+                        eqa_settings.eqa_time(),
+                        "event",
+                        "events",
+                        "Raid mode enabled",
+                    )
                 )
-            )
-            sound_q.put(eqa_struct.sound("speak", "Raid mode enabled"))
-        # Toggle raid state to false
-        elif state.raid == "true" and new_message.rx == "toggle":
-            state.set_raid("false")
-            eqa_config.set_last_state(state, configs)
-            display_q.put(
-                eqa_struct.display(
-                    eqa_settings.eqa_time(),
-                    "event",
-                    "events",
-                    "Raid mode disabled",
+                sound_q.put(eqa_struct.sound("speak", "Raid mode enabled"))
+            # Toggle raid state to false
+            else:
+                state.set_raid(False)
+                eqa_config.set_last_state(state, configs)
+                display_q.put(
+                    eqa_struct.display(
+                        eqa_settings.eqa_time(),
+                        "event",
+                        "events",
+                        "Raid mode disabled",
+                    )
                 )
-            )
-            sound_q.put(eqa_struct.sound("speak", "Raid mode disabled"))
+                sound_q.put(eqa_struct.sound("speak", "Raid mode disabled"))
         # Set raid state to true
-        elif state.raid == "false" and new_message.rx == "true":
-            state.set_raid("true")
+        elif not state.raid and new_message.rx == True:
+            state.set_raid(True)
             eqa_config.set_last_state(state, configs)
             display_q.put(
                 eqa_struct.display(
                     eqa_settings.eqa_time(),
                     "event",
                     "events",
                     new_message.payload,
                 )
             )
         # Set raid state to false
-        elif state.raid == "true" and new_message.rx == "false":
-            state.set_raid("false")
+        elif state.raid and not new_message.rx == True:
+            state.set_raid(False)
             eqa_config.set_last_state(state, configs)
             display_q.put(
                 eqa_struct.display(
                     eqa_settings.eqa_time(),
                     "event",
                     "events",
                     new_message.payload,
                 )
             )
         # Auto-set raid state to true
-        elif (
-            new_message.rx == "auto"
-            and new_message.payload == "true"
-            and state.auto_raid == "false"
-        ):
-            state.set_auto_raid("true")
-            eqa_config.set_last_state(state, configs)
-            display_q.put(
-                eqa_struct.display(
-                    eqa_settings.eqa_time(),
-                    "event",
-                    "events",
-                    "Raid context will be automatically set by zone",
+        elif new_message.rx == "auto":
+            if new_message.payload and not state.auto_raid:
+                state.set_auto_raid(True)
+                eqa_config.set_last_state(state, configs)
+                display_q.put(
+                    eqa_struct.display(
+                        eqa_settings.eqa_time(),
+                        "event",
+                        "events",
+                        "Raid context will be automatically set by zone",
+                    )
                 )
-            )
-            sound_q.put(
-                eqa_struct.sound(
-                    "speak", "Raid context will be automatically set by zone"
+                sound_q.put(
+                    eqa_struct.sound(
+                        "speak", "Raid context will be automatically set by zone"
+                    )
                 )
-            )
-        # Auto-set raid state to false
-        elif (
-            new_message.rx == "auto"
-            and new_message.payload == "false"
-            and state.auto_raid == "true"
-        ):
-            state.set_auto_raid("false")
-            eqa_config.set_last_state(state, configs)
-            display_q.put(
-                eqa_struct.display(
-                    eqa_settings.eqa_time(),
-                    "event",
-                    "events",
-                    "Raid context will not be automatically updated",
+            # Auto-set raid state to false
+            elif not new_message.payload and state.auto_raid:
+                state.set_auto_raid(False)
+                eqa_config.set_last_state(state, configs)
+                display_q.put(
+                    eqa_struct.display(
+                        eqa_settings.eqa_time(),
+                        "event",
+                        "events",
+                        "Raid context will not be automatically updated",
+                    )
                 )
-            )
-            sound_q.put(
-                eqa_struct.sound(
-                    "speak", "Raid context will not be automatically updated"
+                sound_q.put(
+                    eqa_struct.sound(
+                        "speak", "Raid context will not be automatically updated"
+                    )
                 )
-            )
         display_q.put(
-            eqa_struct.display(eqa_settings.eqa_time(), "draw", "redraw", "null")
+            eqa_struct.display(eqa_settings.eqa_time(), "draw", "redraw", None)
         )
 
     except Exception as e:
         eqa_settings.log(
             "system raid: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
             + ": "
@@ -1015,39 +1027,39 @@
 
 
 def system_afk(configs, state, display_q, new_message):
     """Perform system tasks for afk behavior"""
 
     try:
         # Set afk state to true
-        if new_message.payload == "true" and state.afk == "false":
+        if new_message.payload and not state.afk:
             state.set_afk(new_message.payload)
             eqa_config.set_last_state(state, configs)
             display_q.put(
                 eqa_struct.display(
                     eqa_settings.eqa_time(),
                     "event",
                     "events",
                     "You are now AFK",
                 )
             )
         # Set afk state to false
-        elif new_message.payload == "false" and state.afk == "true":
+        elif not new_message.payload and state.afk:
             state.set_afk(new_message.payload)
             eqa_config.set_last_state(state, configs)
             display_q.put(
                 eqa_struct.display(
                     eqa_settings.eqa_time(),
                     "event",
                     "events",
                     "You are no longer AFK",
                 )
             )
         display_q.put(
-            eqa_struct.display(eqa_settings.eqa_time(), "draw", "redraw", "null")
+            eqa_struct.display(eqa_settings.eqa_time(), "draw", "redraw", None)
         )
 
     except Exception as e:
         eqa_settings.log(
             "system afk: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
             + ": "
@@ -1058,31 +1070,31 @@
 def system_timer(configs, state, display_q, sound_q, new_message):
     """Perform system tasks for auto timer behavior"""
 
     try:
         # If timer setting is mob related
         if new_message.rx == "mob":
             # Set auto-mob timer to true
-            if state.auto_mob_timer == "false" and new_message.payload == "true":
-                state.set_auto_mob_timer("true")
+            if not state.auto_mob_timer and new_message.payload:
+                state.set_auto_mob_timer(True)
                 eqa_config.set_last_state(state, configs)
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         "Automatic mob respawn timers enabled",
                     )
                 )
                 sound_q.put(
                     eqa_struct.sound("speak", "Automatic mob respawn timers enabled")
                 )
             # Set auto-mob timer to false
-            elif state.auto_mob_timer == "true" and new_message.payload == "false":
-                state.set_auto_mob_timer("false")
+            elif state.auto_mob_timer and not new_message.payload:
+                state.set_auto_mob_timer(False)
                 eqa_config.set_last_state(state, configs)
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         "Automatic mob respawn timers disabled",
@@ -1091,15 +1103,15 @@
                 sound_q.put(
                     eqa_struct.sound("speak", "Automatic mob respawn timers disabled")
                 )
         # If timer setting is spell related
         elif new_message.rx == "spell":
             pass
         display_q.put(
-            eqa_struct.display(eqa_settings.eqa_time(), "draw", "redraw", "null")
+            eqa_struct.display(eqa_settings.eqa_time(), "draw", "redraw", None)
         )
 
     except Exception as e:
         eqa_settings.log(
             "system timers: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
             + ": "
@@ -1108,16 +1120,16 @@
 
 
 def system_spell_timer(configs, state, display_q, sound_q, new_message):
     """Update spell timer states"""
 
     try:
         if new_message.rx == "self":
-            if state.spell_timer_self == "true":
-                state.set_spell_timer_self("false")
+            if state.spell_timer_self:
+                state.set_spell_timer_self(False)
                 eqa_config.set_last_state(state, configs)
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         "Spell timers disabled for spells targetting you",
@@ -1125,15 +1137,15 @@
                 )
                 sound_q.put(
                     eqa_struct.sound(
                         "speak", "Spell timers disabled for spells targetting you"
                     )
                 )
             else:
-                state.set_spell_timer_self("true")
+                state.set_spell_timer_self(True)
                 eqa_config.set_last_state(state, configs)
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         "Spell timers enabled for spells targetting you",
@@ -1141,16 +1153,16 @@
                 )
                 sound_q.put(
                     eqa_struct.sound(
                         "speak", "Spell timers enabled for spells targetting you"
                     )
                 )
         elif new_message.rx == "other":
-            if state.spell_timer_other == "true":
-                state.set_spell_timer_other("false")
+            if state.spell_timer_other:
+                state.set_spell_timer_other(False)
                 eqa_config.set_last_state(state, configs)
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         "Spell timers disabled for spells targetting others",
@@ -1158,15 +1170,15 @@
                 )
                 sound_q.put(
                     eqa_struct.sound(
                         "speak", "Spell timers disabled for spells targetting others"
                     )
                 )
             else:
-                state.set_spell_timer_other("true")
+                state.set_spell_timer_other(True)
                 eqa_config.set_last_state(state, configs)
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         "Spell timers enabled for spells targetting others",
@@ -1174,16 +1186,16 @@
                 )
                 sound_q.put(
                     eqa_struct.sound(
                         "speak", "Spell timers enabled for spells targetting others"
                     )
                 )
         elif new_message.rx == "guild":
-            if state.spell_timer_guild_only == "true":
-                state.set_spell_timer_guild_only("false")
+            if state.spell_timer_guild_only:
+                state.set_spell_timer_guild_only(False)
                 eqa_config.set_last_state(state, configs)
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         "Spell timers will no longer filter for guild members",
@@ -1191,15 +1203,15 @@
                 )
                 sound_q.put(
                     eqa_struct.sound(
                         "speak", "Spell timers will no longer filter for guild members"
                     )
                 )
             else:
-                state.set_spell_timer_guild_only("true")
+                state.set_spell_timer_guild_only(True)
                 eqa_config.set_last_state(state, configs)
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         "Spell timers will filter for guild members",
@@ -1207,16 +1219,16 @@
                 )
                 sound_q.put(
                     eqa_struct.sound(
                         "speak", "Spell timers will filter for guild members"
                     )
                 )
         elif new_message.rx == "yours":
-            if state.spell_timer_yours_only == "true":
-                state.set_spell_timer_yours_only("false")
+            if state.spell_timer_yours_only:
+                state.set_spell_timer_yours_only(False)
                 eqa_config.set_last_state(state, configs)
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         "Spell timers will no longer filter only your spells",
@@ -1224,15 +1236,15 @@
                 )
                 sound_q.put(
                     eqa_struct.sound(
                         "speak", "Spell timers will no longer filter only your spells"
                     )
                 )
             else:
-                state.set_spell_timer_yours_only("true")
+                state.set_spell_timer_yours_only(True)
                 eqa_config.set_last_state(state, configs)
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         "Spell timers will filter for only your spells",
@@ -1240,16 +1252,16 @@
                 )
                 sound_q.put(
                     eqa_struct.sound(
                         "speak", "Spell timers will filter for only your spells"
                     )
                 )
         elif new_message.rx == "guess":
-            if state.spell_timer_guess == "true":
-                state.set_spell_timer_guess("false")
+            if state.spell_timer_guess:
+                state.set_spell_timer_guess(False)
                 eqa_config.set_last_state(state, configs)
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         "Spell timers will no longer guess some uncertain spell timers",
@@ -1258,15 +1270,15 @@
                 sound_q.put(
                     eqa_struct.sound(
                         "speak",
                         "Spell timers will no longer guess some uncertain spell timers",
                     )
                 )
             else:
-                state.set_spell_timer_guess("true")
+                state.set_spell_timer_guess(True)
                 eqa_config.set_last_state(state, configs)
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         "Spell timers will guess some uncertain spell timers",
@@ -1274,15 +1286,15 @@
                 )
                 sound_q.put(
                     eqa_struct.sound(
                         "speak", "Spell timers will guess some uncertain spell timers"
                     )
                 )
         display_q.put(
-            eqa_struct.display(eqa_settings.eqa_time(), "draw", "redraw", "null")
+            eqa_struct.display(eqa_settings.eqa_time(), "draw", "redraw", None)
         )
 
     except Exception as e:
         eqa_settings.log(
             "system spell timers: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
             + ": "
@@ -1291,41 +1303,41 @@
 
 
 def system_consider(configs, state, display_q, sound_q, new_message):
     """Perform system tasks for consider eval behavior"""
 
     try:
         # Toggle consider eval state to true
-        if state.consider_eval == "false" and new_message.payload == "true":
-            state.set_consider_eval("true")
+        if not state.consider_eval and new_message.payload:
+            state.set_consider_eval(True)
             eqa_config.set_last_state(state, configs)
             display_q.put(
                 eqa_struct.display(
                     eqa_settings.eqa_time(),
                     "event",
                     "events",
                     "Consider evaluation enabled",
                 )
             )
             sound_q.put(eqa_struct.sound("speak", "Consider evaluation enabled"))
         # Toggle consider eval state to false
-        elif state.consider_eval == "true" and new_message.payload == "false":
-            state.set_consider_eval("false")
+        elif state.consider_eval and not new_message.payload:
+            state.set_consider_eval(False)
             eqa_config.set_last_state(state, configs)
             display_q.put(
                 eqa_struct.display(
                     eqa_settings.eqa_time(),
                     "event",
                     "events",
                     "Consider evaluation disabled",
                 )
             )
             sound_q.put(eqa_struct.sound("speak", "Consider evaluation disabled"))
         display_q.put(
-            eqa_struct.display(eqa_settings.eqa_time(), "draw", "redraw", "null")
+            eqa_struct.display(eqa_settings.eqa_time(), "draw", "redraw", None)
         )
 
     except Exception as e:
         eqa_settings.log(
             "system consider: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
             + ": "
@@ -1334,45 +1346,45 @@
 
 
 def system_detect_char(configs, state, display_q, sound_q, new_message):
     """Perform system tasks for automatic character detection"""
 
     try:
         # Toggle detect char state to true
-        if state.detect_char == "false" and new_message.payload == "true":
-            state.set_detect_char("true")
+        if not state.detect_char and new_message.payload:
+            state.set_detect_char(True)
             eqa_config.set_last_state(state, configs)
             display_q.put(
                 eqa_struct.display(
                     eqa_settings.eqa_time(),
                     "event",
                     "events",
                     "Automatic character detection enabled",
                 )
             )
             sound_q.put(
                 eqa_struct.sound("speak", "Automatic character detection enabled")
             )
         # Toggle detect char state to false
-        elif state.detect_char == "true" and new_message.payload == "false":
-            state.set_detect_char("false")
+        elif state.detect_char and not new_message.payload:
+            state.set_detect_char(False)
             eqa_config.set_last_state(state, configs)
             display_q.put(
                 eqa_struct.display(
                     eqa_settings.eqa_time(),
                     "event",
                     "events",
                     "Automatic character detection disabled",
                 )
             )
             sound_q.put(
                 eqa_struct.sound("speak", "Automatic character detection disabled")
             )
         display_q.put(
-            eqa_struct.display(eqa_settings.eqa_time(), "draw", "redraw", "null")
+            eqa_struct.display(eqa_settings.eqa_time(), "draw", "redraw", None)
         )
 
     except Exception as e:
         eqa_settings.log(
             "system consider: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
             + ": "
@@ -1381,43 +1393,43 @@
 
 
 def system_debug(configs, state, display_q, sound_q, new_message):
     """Perform system tasks for debug behavior"""
 
     try:
         # Toggle debug state to true
-        if state.debug == "false" and new_message.rx == "toggle":
-            state.set_debug("true")
+        if not state.debug and new_message.rx == "toggle":
+            state.set_debug(True)
             eqa_config.set_last_state(state, configs)
             display_q.put(
                 eqa_struct.display(
                     eqa_settings.eqa_time(),
                     "event",
                     "events",
                     "Debug mode enabled",
                 )
             )
             sound_q.put(
                 eqa_struct.sound("speak", "Displaying and logging all parser output")
             )
         # Toggle debug state to false
-        elif state.debug == "true" and new_message.rx == "toggle":
-            state.set_debug("false")
+        elif state.debug and new_message.rx == "toggle":
+            state.set_debug(False)
             eqa_config.set_last_state(state, configs)
             display_q.put(
                 eqa_struct.display(
                     eqa_settings.eqa_time(),
                     "event",
                     "events",
                     "Debug mode disabled",
                 )
             )
             sound_q.put(eqa_struct.sound("speak", "Debug mode disabled"))
         display_q.put(
-            eqa_struct.display(eqa_settings.eqa_time(), "draw", "redraw", "null")
+            eqa_struct.display(eqa_settings.eqa_time(), "draw", "redraw", None)
         )
 
     except Exception as e:
         eqa_settings.log(
             "system debug: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
             + ": "
@@ -1426,260 +1438,146 @@
 
 
 def system_encounter(configs, state, display_q, sound_q, encounter_q, new_message):
     """Perform system tasks for encounter parse behavior"""
 
     try:
         # Toggle encounter parse to true
-        if state.encounter_parse == "false" and new_message.rx == "toggle":
-            state.set_encounter_parse("true")
-            eqa_config.set_last_state(state, configs)
-            display_q.put(
-                eqa_struct.display(
-                    eqa_settings.eqa_time(),
-                    "event",
-                    "events",
-                    "Encounter Parse Enabled",
-                )
-            )
-            encounter_q.put(
-                eqa_struct.message(
-                    eqa_settings.eqa_time(), "null", "clear", "null", "null"
-                )
-            )
-            sound_q.put(eqa_struct.sound("speak", "Encounter Parse Enabled"))
-        # Toggle encounter parse to false
-        elif state.encounter_parse == "true" and new_message.rx == "toggle":
-            state.set_encounter_parse("false")
-            eqa_config.set_last_state(state, configs)
-            display_q.put(
-                eqa_struct.display(
-                    eqa_settings.eqa_time(),
-                    "event",
-                    "events",
-                    "Encounter Parse Disabled",
-                )
-            )
-            sound_q.put(eqa_struct.sound("speak", "Encounter Parse Disabled"))
-        # Set encounter parse save to false
-        elif (
-            state.save_parse == "true"
-            and new_message.rx == "save"
-            and new_message.payload == "false"
-        ):
-            state.set_encounter_parse_save("false")
-            eqa_config.set_last_state(state, configs)
-            display_q.put(
-                eqa_struct.display(
-                    eqa_settings.eqa_time(),
-                    "event",
-                    "events",
-                    "Encounter parse will not save to a file",
-                )
-            )
-            sound_q.put(
-                eqa_struct.sound("speak", "Encounter parser will not save to a file")
-            )
-        # Set encounter parse save to true
-        elif (
-            state.save_parse == "false"
-            and new_message.rx == "save"
-            and new_message.payload == "true"
-        ):
-            state.set_encounter_parse_save("true")
-            eqa_config.set_last_state(state, configs)
-            display_q.put(
-                eqa_struct.display(
-                    eqa_settings.eqa_time(),
-                    "event",
-                    "events",
-                    "Encounter parse will automatically save to a file",
-                )
-            )
-            sound_q.put(
-                eqa_struct.sound(
-                    "speak", "Encounter parser will automatically save to a file"
-                )
-            )
-        # Clear encounter parse stack
-        elif new_message.rx == "clear":
-            encounter_q.put(
-                eqa_struct.message(
-                    eqa_settings.eqa_time(), "null", "clear", "null", "null"
-                )
-            )
-        # End encounter parse and resolve stack
-        elif new_message.rx == "end":
-            encounter_q.put(
-                eqa_struct.message(
-                    eqa_settings.eqa_time(), "null", "end", "null", "null"
-                )
-            )
-        display_q.put(
-            eqa_struct.display(eqa_settings.eqa_time(), "draw", "redraw", "null")
-        )
-
-    except Exception as e:
-        eqa_settings.log(
-            "system encounter: Error on line "
-            + str(sys.exc_info()[-1].tb_lineno)
-            + ": "
-            + str(e)
-        )
-
-
-def system_mute(configs, state, display_q, sound_q, new_message):
-    """Perform system tasks for mute behavior"""
-
-    try:
-        # Toggle mute
-        if new_message.rx == "toggle" and new_message.payload == "all":
-            # to true
-            if state.mute == "false":
-                sound_q.put(eqa_struct.sound("mute_speak", "true"))
-                sound_q.put(eqa_struct.sound("mute_alert", "true"))
-                state.set_mute("true")
+        if new_message.rx == "toggle":
+            if not state.encounter_parse:
+                state.set_encounter_parse(True)
                 eqa_config.set_last_state(state, configs)
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
-                        "Mute Enabled",
+                        "Encounter Parse Enabled",
                     )
                 )
-            # to false
-            else:
-                sound_q.put(eqa_struct.sound("mute_speak", "false"))
-                sound_q.put(eqa_struct.sound("mute_alert", "false"))
-                state.set_mute("false")
-                eqa_config.set_last_state(state, configs)
-                display_q.put(
-                    eqa_struct.display(
-                        eqa_settings.eqa_time(),
-                        "event",
-                        "events",
-                        "Mute Disabled",
+                encounter_q.put(
+                    eqa_struct.message(
+                        eqa_settings.eqa_time(), None, "clear", None, None
                     )
                 )
-                sound_q.put(eqa_struct.sound("speak", "Mute disabled"))
-        # Toggle mute speak
-        elif new_message.rx == "toggle" and new_message.payload == "speak":
-            # to speak
-            if state.mute == "false":
-                sound_q.put(eqa_struct.sound("mute_speak", "true"))
-                state.set_mute("speak")
+                sound_q.put(eqa_struct.sound("speak", "Encounter Parse Enabled"))
+            # Toggle encounter parse to false
+            else:
+                state.set_encounter_parse(False)
                 eqa_config.set_last_state(state, configs)
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
-                        "Mute Speak Enabled",
+                        "Encounter Parse Disabled",
                     )
                 )
-            # to true
-            elif state.mute == "alert":
-                sound_q.put(eqa_struct.sound("mute_speak", "true"))
-                state.set_mute("true")
+                sound_q.put(eqa_struct.sound("speak", "Encounter Parse Disabled"))
+        # Set encounter parse save to false
+        elif new_message.rx == "save":
+            if state.save_parse and not new_message.payload:
+                state.set_encounter_parse_save(False)
                 eqa_config.set_last_state(state, configs)
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
-                        "Mute Enabled",
+                        "Encounter parse will not save to a file",
                     )
                 )
-            # to alert
-            elif state.mute == "true":
-                sound_q.put(eqa_struct.sound("mute_speak", "false"))
-                state.set_mute("alert")
-                eqa_config.set_last_state(state, configs)
-                display_q.put(
-                    eqa_struct.display(
-                        eqa_settings.eqa_time(),
-                        "event",
-                        "events",
-                        "Mute Speak Disabled",
+                sound_q.put(
+                    eqa_struct.sound(
+                        "speak", "Encounter parser will not save to a file"
                     )
                 )
-                sound_q.put(eqa_struct.sound("speak", "Mute speak disabled"))
-            # to false
-            else:
-                sound_q.put(eqa_struct.sound("mute_speak", "false"))
-                state.set_mute("false")
+            # Set encounter parse save to true
+            elif not state.save_parse and new_message.payload:
+                state.set_encounter_parse_save(True)
                 eqa_config.set_last_state(state, configs)
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
-                        "Mute Disabled",
+                        "Encounter parse will automatically save to a file",
                     )
                 )
-                sound_q.put(eqa_struct.sound("speak", "Mute disabled"))
-        # Toggle mute alert
-        elif new_message.rx == "toggle" and new_message.payload == "alert":
-            # to alert
-            if state.mute == "false":
-                sound_q.put(eqa_struct.sound("mute_alert", "true"))
-                state.set_mute("alert")
-                eqa_config.set_last_state(state, configs)
-                display_q.put(
-                    eqa_struct.display(
-                        eqa_settings.eqa_time(),
-                        "event",
-                        "events",
-                        "Mute Alert Enabled",
+                sound_q.put(
+                    eqa_struct.sound(
+                        "speak", "Encounter parser will automatically save to a file"
                     )
                 )
+        # Clear encounter parse stack
+        elif new_message.rx == "clear":
+            encounter_q.put(
+                eqa_struct.message(eqa_settings.eqa_time(), None, "clear", None, None)
+            )
+        # End encounter parse and resolve stack
+        elif new_message.rx == "end":
+            encounter_q.put(
+                eqa_struct.message(eqa_settings.eqa_time(), None, "end", None, None)
+            )
+        display_q.put(
+            eqa_struct.display(eqa_settings.eqa_time(), "draw", "redraw", None)
+        )
+
+    except Exception as e:
+        eqa_settings.log(
+            "system encounter: Error on line "
+            + str(sys.exc_info()[-1].tb_lineno)
+            + ": "
+            + str(e)
+        )
+
+
+def system_mute(configs, state, display_q, sound_q, new_message):
+    """Perform system tasks for mute behavior"""
+
+    try:
+        # Toggle mute
+        if new_message.rx == "toggle" and new_message.payload == "all":
             # to true
-            elif state.mute == "speak":
-                sound_q.put(eqa_struct.sound("mute_alert", "true"))
-                state.set_mute("true")
+            if not state.mute:
+                sound_q.put(eqa_struct.sound("mute_speak", True))
+                sound_q.put(eqa_struct.sound("mute_alert", True))
+                state.set_mute(True)
                 eqa_config.set_last_state(state, configs)
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         "Mute Enabled",
                     )
                 )
-            # to speak
-            elif state.mute == "true":
-                sound_q.put(eqa_struct.sound("mute_alert", "false"))
-                state.set_mute("speak")
-                eqa_config.set_last_state(state, configs)
-                display_q.put(
-                    eqa_struct.display(
-                        eqa_settings.eqa_time(),
-                        "event",
-                        "events",
-                        "Mute Alert Disabled",
-                    )
-                )
-                sound_q.put(eqa_struct.sound("speak", "Mute alert disabled"))
             # to false
             else:
-                sound_q.put(eqa_struct.sound("mute_alert", "false"))
-                state.set_mute("false")
+                sound_q.put(eqa_struct.sound("mute_speak", False))
+                sound_q.put(eqa_struct.sound("mute_alert", False))
+                state.set_mute(False)
                 eqa_config.set_last_state(state, configs)
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         "Mute Disabled",
                     )
                 )
                 sound_q.put(eqa_struct.sound("speak", "Mute disabled"))
+        # Toggle mute speak
+        elif new_message.rx == "toggle" and new_message.payload == "speak":
+            sound_q.put(eqa_struct.sound("mute_speak", "toggle"))
+        # Toggle mute alert
+        elif new_message.rx == "toggle" and new_message.payload == "alert":
+            sound_q.put(eqa_struct.sound("mute_alert", "toggle"))
         display_q.put(
-            eqa_struct.display(eqa_settings.eqa_time(), "draw", "redraw", "null")
+            eqa_struct.display(eqa_settings.eqa_time(), "draw", "redraw", None)
         )
 
     except Exception as e:
         eqa_settings.log(
             "system mute: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
             + ": "
```

### Comparing `eqalert-3.5.0/eqa/lib/action.py` & `eqalert-3.5.1/eqa/lib/action.py`

 * *Files 21% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 
 from collections import deque
 import datetime
 import sys
 import time
 import re
 import os
-import pkg_resources
 
 import eqa.lib.config as eqa_config
 import eqa.lib.settings as eqa_settings
 import eqa.lib.sound as eqa_sound
 import eqa.lib.struct as eqa_struct
 
 
@@ -42,14 +41,15 @@
     system_q,
     display_q,
     sound_q,
     exit_flag,
     cfg_reload,
     mute_list,
     change_char,
+    version,
 ):
     """
     Process: action_q
     Produce: sound_q, display_q, system_q, encounter_q
     """
 
     try:
@@ -73,183 +73,218 @@
         )
 
         # Player Data
         player_list = eqa_config.get_players_file(
             configs.settings.config["settings"]["paths"]["data"], state.server
         )
 
+        # Class Mapping
+        class_mapping = {
+            "bard": "bard",
+            "minstrel": "bard",
+            "troubadour": "bard",
+            "virtuoso": "bard",
+            "cleric": "cleric",
+            "vicar": "cleric",
+            "templar": "cleric",
+            "high priest": "cleric",
+            "druid": "druid",
+            "wanderer": "druid",
+            "preserver": "druid",
+            "hierophant": "druid",
+            "enchanter": "enchanter",
+            "illusionist": "enchanter",
+            "beguiler": "enchanter",
+            "phantasmist": "enchanter",
+            "magician": "magician",
+            "elementalist": "magician",
+            "conjurer": "magician",
+            "arch mage": "magician",
+            "monk": "monk",
+            "disciple": "monk",
+            "master": "monk",
+            "grandmaster": "monk",
+            "necromancer": "necromancer",
+            "heretic": "necromancer",
+            "defiler": "necromancer",
+            "warlock": "necromancer",
+            "paladin": "paladin",
+            "cavalier": "paladin",
+            "knight": "paladin",
+            "crusader": "paladin",
+            "ranger": "ranger",
+            "pathfinder": "ranger",
+            "outrider": "ranger",
+            "warder": "ranger",
+            "rogue": "rogue",
+            "rake": "rogue",
+            "blackguard": "rogue",
+            "assassin": "rogue",
+            "shadow knight": "shadow knight",
+            "reaver": "shadow knight",
+            "revenant": "shadow knight",
+            "grave lord": "shadow knight",
+            "shaman": "shaman",
+            "mystic": "shaman",
+            "luminary": "shaman",
+            "oracle": "shaman",
+            "warrior": "warrior",
+            "champion": "warrior",
+            "myrmidon": "warrior",
+            "warlord": "warrior",
+            "wizard": "wizard",
+            "channeler": "wizard",
+            "evoker": "wizard",
+            "sorcerer": "wizard",
+        }
+
         while (
             not exit_flag.is_set()
             and not cfg_reload.is_set()
             and not change_char.is_set()
         ):
             # Sleep between empty checks
-            queue_size = action_q.qsize()
-            if queue_size < 1:
+            if action_q.qsize() < 1:
                 time.sleep(0.01)
-            else:
-                if state.debug == "true":
-                    eqa_settings.log("action_q depth: " + str(queue_size))
+            elif state.debug:
+                eqa_settings.log("action_q depth: " + str(action_q.qsize()))
 
             # Check queue for message
             if not action_q.empty():
                 ## Read new message
                 new_message = action_q.get()
                 line_type = new_message.type
                 line_time = new_message.timestamp
                 line_tx = new_message.tx
                 line_rx = new_message.rx
                 check_line = new_message.payload
 
                 ## Debug: Log line match type
-                if state.debug == "true":
-                    action_matched(line_type, check_line, base_path)
+                if state.debug:
+                    action_matched(line_type, check_line, base_path, version)
                     display_q.put(
                         eqa_struct.display(
                             eqa_settings.eqa_time(),
                             "event",
                             "debug",
                             (line_type, check_line),
                         )
                     )
 
                 ## Encounter Parsing
-                if state.encounter_parse == "true":
-                    if re.fullmatch(r"^combat\_.+", line_type) is not None:
+                if state.encounter_parse:
+                    if "combat_" in line_type:
                         encounter_q.put(
                             eqa_struct.message(
                                 line_time,
                                 line_type,
                                 "combat",
-                                "null",
+                                None,
                                 check_line,
                             )
                         )
-                    elif re.fullmatch(r"^you\_auto\_attack\_.+", line_type) is not None:
+                    elif "you_auto_attack_" in line_type:
                         encounter_q.put(
                             eqa_struct.message(
                                 line_time,
                                 line_type,
                                 "combat",
-                                "null",
+                                None,
                                 check_line,
                             )
                         )
-                    elif re.fullmatch(r"^mob\_slain\_.+", line_type) is not None:
+                    elif "mob_slain_" in line_type:
                         encounter_q.put(
                             eqa_struct.message(
                                 line_time,
                                 line_type,
                                 "stop",
-                                "null",
+                                None,
                                 check_line,
                             )
                         )
                     elif line_type == "spells_cast_other":
                         encounter_q.put(
                             eqa_struct.message(
                                 line_time,
                                 line_type,
                                 "spell",
-                                "null",
+                                None,
                                 check_line,
                             )
                         )
                     elif line_type == "spells_cast_you":
                         encounter_q.put(
                             eqa_struct.message(
                                 line_time,
                                 line_type,
                                 "spell",
-                                "null",
+                                None,
                                 check_line,
                             )
                         )
                     elif line_type == "you_new_zone":
                         encounter_q.put(
                             eqa_struct.message(
                                 line_time,
                                 line_type,
                                 "stop",
-                                "null",
+                                None,
                                 check_line,
                             )
                         )
-                    elif re.fullmatch(r"^experience\_.+", line_type) is not None:
+                    elif "experience_" in line_type:
                         encounter_q.put(
                             eqa_struct.message(
                                 line_time,
                                 line_type,
                                 "stop",
-                                "null",
+                                None,
                                 check_line,
                             )
                         )
                     elif line_type == "faction_line":
                         encounter_q.put(
                             eqa_struct.message(
                                 line_time,
                                 line_type,
                                 "stop",
-                                "null",
+                                None,
                                 check_line,
                             )
                         )
-                    elif re.fullmatch(r"^spells\_.+", line_type) is not None:
+                    elif "spells_" in line_type:
                         encounter_q.put(
                             eqa_struct.message(
                                 line_time,
                                 line_type,
                                 "spell",
-                                "null",
+                                None,
                                 check_line,
                             )
                         )
                 ## Mob Timers
-                if state.auto_mob_timer == "true":
+                if state.auto_mob_timer:
                     if (
                         line_type == "experience_solo"
                         or line_type == "experience_group"
                     ):
-                        action_mob_timer(
-                            timer_q,
-                            configs.zones.config["zones"][str(state.zone)]["timer"],
-                            state.auto_mob_timer_delay,
-                            state.zone,
-                        )
-
-                ## TODO: Spell Casting Item Buffer
-                # Interesting note, these only show up for the active player for any non-instant cast item.  Other plays get the normal casting message.
-                # if line_type == "spells_cast_item_you":
-                #    action_spell_casting(
-                #        check_line, line_type, line_time, spell_casting_buffer_other, spell_casting_buffer_you
-                #    )
-
-                ## Spell Casting Buffer Other
-                if re.fullmatch(r"^spells\_cast\_other", line_type) is not None:
-                    action_spell_casting_other(
-                        check_line,
-                        line_type,
-                        line_time,
-                        spell_casting_buffer_other,
-                    )
-                ## Spell Casting Buffer You
-                if re.fullmatch(r"^spells\_cast\_you", line_type) is not None:
-                    spell_casting_buffer_you = action_spell_casting_you(
-                        check_line,
-                        line_type,
-                        line_time,
-                        spell_casting_buffer_you,
-                    )
+                        if state.zone is not None:
+                            action_mob_timer(
+                                timer_q,
+                                configs.zones.config["zones"][state.zone]["timer"],
+                                state.auto_mob_timer_delay,
+                                state.zone,
+                            )
 
                 ## Self Spell Timers
                 if (
-                    state.spell_timer_self == "true"
-                    or state.spell_timer_guild_only == "true"
-                    or state.spell_timer_yours_only == "true"
+                    state.spell_timer_self
+                    or state.spell_timer_guild_only
+                    or state.spell_timer_yours_only
                 ):
                     if re.fullmatch(r"^spell\_.+\_you_on$", line_type) is not None:
                         action_spell_timer(
                             state,
                             timer_q,
                             line_type,
                             line_time,
@@ -264,17 +299,17 @@
                     elif re.fullmatch(r"^spell\_.+\_you_off$", line_type) is not None:
                         action_spell_remove_timer(
                             state, timer_q, spell_lines, line_type
                         )
 
                 ## Other Spell Timers
                 if (
-                    state.spell_timer_other == "true"
-                    or state.spell_timer_guild_only == "true"
-                    or state.spell_timer_guild_only == "true"
+                    state.spell_timer_other
+                    or state.spell_timer_guild_only
+                    or state.spell_timer_yours_only
                 ):
                     if re.fullmatch(r"^spell\_.+\_other_on$", line_type) is not None:
                         action_spell_timer(
                             state,
                             timer_q,
                             line_type,
                             line_time,
@@ -284,29 +319,57 @@
                             spell_timers,
                             spell_lines,
                             spell_casters,
                             player_list,
                         )
 
                 ## Consider Evaluation
-                if state.consider_eval == "true" and line_type == "consider":
-                    action_consider_evaluation(sound_q, check_line)
-
-                if line_type == "zoning":
+                if state.consider_eval:
+                    if line_type == "consider":
+                        action_consider_evaluation(sound_q, check_line)
+
+                ## Always on line_type specific actions
+                if line_type == "who_player":
+                    action_who_player(
+                        configs, system_q, state, check_line, player_list, class_mapping
+                    )
+                ### Spell Casting Buffer Other
+                elif line_type == "spells_cast_other":
+                    action_spell_casting_other(
+                        check_line,
+                        line_type,
+                        line_time,
+                        spell_casting_buffer_other,
+                    )
+                ### Spell Casting Buffer You
+                elif line_type == "spells_cast_you":
+                    spell_casting_buffer_you = action_spell_casting_you(
+                        check_line,
+                        line_type,
+                        line_time,
+                        spell_casting_buffer_you,
+                    )
+                ### TODO: Spell Casting Item Buffer
+                # Interesting note, these only show up for the active player for any non-instant cast item.  Other plays get the normal casting message.
+                # elif line_type == "spells_cast_item_you":
+                #    action_spell_casting(
+                #        check_line, line_type, line_time, spell_casting_buffer_other, spell_casting_buffer_you
+                #    )
+                ### Spell timer zone drift
+                elif line_type == "zoning":
                     timer_q.put(
                         eqa_struct.timer(
                             datetime.datetime.now(),
                             "zoning",
                             None,
                             None,
                         )
                     )
-
-                ## State Building Line Types
-                if line_type == "location":
+                ### State building line types
+                elif line_type == "location":
                     action_location(system_q, check_line)
                 elif line_type == "direction":
                     action_direction(system_q, check_line)
                 elif line_type == "motd_welcome":
                     action_motd_welcome(system_q)
                 elif line_type == "group_join_notify":
                     action_group_join_notify(system_q, check_line)
@@ -328,16 +391,15 @@
                     action_you_char_bound(system_q, check_line)
                 elif line_type == "spell_bind_you":
                     action_spell_bind_you(system_q, state)
                 elif line_type == "you_afk_off":
                     action_you_afk_off(system_q)
                 elif line_type == "you_afk_on":
                     action_you_afk_on(system_q)
-                elif line_type == "who_player":
-                    action_who_player(configs, system_q, state, check_line, player_list)
+                ### Parser say commands
                 elif line_type == "say_you":
                     if (
                         re.fullmatch(r"^You say, \'parser .+\'$", check_line)
                         is not None
                     ):
                         action_you_say_commands(
                             timer_q,
@@ -346,14 +408,15 @@
                             display_q,
                             check_line,
                             configs,
                             mute_list,
                             state,
                             player_list,
                         )
+                ### You new zone
                 elif line_type == "you_new_zone":
                     action_you_new_zone(
                         base_path,
                         system_q,
                         display_q,
                         sound_q,
                         timer_q,
@@ -375,15 +438,15 @@
                             sound_q,
                             display_q,
                             state,
                             mute_list,
                         )
 
                     ### Handle Context Reactions
-                    elif reaction != "false":
+                    elif reaction != False:
                         reaction_context(
                             line_type,
                             check_line,
                             configs,
                             sound_q,
                             display_q,
                             state,
@@ -400,15 +463,15 @@
                             sound_q,
                             display_q,
                             state,
                             mute_list,
                         )
 
                     ### Handle context reaction for all lines
-                    elif configs.alerts.config["line"]["all"]["reaction"] != "false":
+                    elif configs.alerts.config["line"]["all"]["reaction"] != False:
                         reaction_context(
                             "all",
                             check_line,
                             configs,
                             sound_q,
                             display_q,
                             state,
@@ -429,23 +492,23 @@
                         )
                     )
                     system_q.put(
                         eqa_struct.message(
                             eqa_settings.eqa_time(),
                             "system",
                             "reload_config",
-                            "null",
-                            "null",
+                            None,
+                            None,
                         )
                     )
 
                 action_q.task_done()
 
         # Save any new player data collected to file
-        if configs.settings.config["settings"]["player_data"]["persist"] == "true":
+        if configs.settings.config["settings"]["player_data"]["persist"]:
             eqa_config.update_players_file(
                 configs.settings.config["settings"]["paths"]["data"],
                 state.server,
                 player_list,
             )
 
     except Exception as e:
@@ -591,35 +654,35 @@
             if line_type in spell_lines["spell_lines"].keys():
                 for spell in spell_lines["spell_lines"][line_type].keys():
                     # Submit timer removal
                     timer_q.put(
                         eqa_struct.spell_timer(
                             (datetime.datetime.now()),
                             "remove_spell_timer",
-                            "null",
+                            None,
                             state.char.lower(),
                             spell,
-                            "null",
-                            "null",
-                            "null",
+                            None,
+                            None,
+                            None,
                         )
                     )
         else:
             spell = re.findall(r"(?<=spell\_)[a-zA-Z\s\_]+(?=\_you\_off)", line_type)[0]
             # Submit timer removal
             timer_q.put(
                 eqa_struct.spell_timer(
                     (datetime.datetime.now()),
                     "remove_spell_timer",
-                    "null",
+                    None,
                     state.char.lower(),
                     spell,
-                    "null",
-                    "null",
-                    "null",
+                    None,
+                    None,
+                    None,
                 )
             )
 
     except Exception as e:
         eqa_settings.log(
             "acton spell remove timer: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
@@ -669,20 +732,20 @@
             spell = re.findall(r"(?<=spell\_)[a-zA-Z\s\_]+(?=\_other\_on)", line_type)[
                 0
             ]
             target = re.findall(r"(?:^|(?:[.!?]\s))(\w+)", line)[0].lower()
 
         # If this is a spell cast line output shared by more than one spell
         if is_spell_line:
-            if state.debug == "true":
+            if state.debug:
                 eqa_settings.log("spell line found: " + line_type)
             # Determine possible spells
             if line_type in spell_lines["spell_lines"].keys():
                 possible_spells = spell_lines["spell_lines"][line_type].keys()
-                if state.debug == "true":
+                if state.debug:
                     eqa_settings.log("possible spells: " + str(possible_spells))
                 check_for_spells = []
                 # Retrieve casting requirements for each possible spell
                 for possible_spell in possible_spells:
                     if possible_spell in spell_casters["spells"].keys():
                         # Validate a player cast this spell
                         ## TODO: later try and guess npc/item only spells with vague messages, for now thats too much guessing
@@ -693,23 +756,23 @@
                                     "classes": spell_casters["spells"][possible_spell][
                                         "classes"
                                     ].keys(),
                                 }
                             )
 
                 # First check if the player could have cast this
-                if spell_casting_buffer_you:
+                if spell_casting_buffer_you and state.char_level is not None:
                     # If the most recent player cast spell is in the possible spell list
                     if (
                         spell_casting_buffer_you["spell"]
                         in spell_lines["spell_lines"][line_type].keys()
                         and spell_casting_buffer_you["spell"]
                         in spell_casters["spells"].keys()
                     ):
-                        if state.debug == "true":
+                        if state.debug:
                             eqa_settings.log(
                                 "Checking if cast for: "
                                 + spell_casting_buffer_you["spell"]
                                 + " occurred "
                                 + spell_timers["spells"][
                                     spell_casting_buffer_you["spell"]
                                 ]["cast_time"]
@@ -772,81 +835,89 @@
                                 == 0
                             ):
                                 # Check if caster is able to cast potential spell
                                 if recent_cast_event["caster"] in player_list.keys():
                                     player_class = player_list[
                                         recent_cast_event["caster"]
                                     ]["class"]
-                                    # If the player class can cast it
-                                    if (
-                                        player_class
-                                        in spell_casters["spells"][
-                                            spell_caster["spell"]
-                                        ]["classes"].keys()
-                                    ):
-                                        player_level = int(
-                                            player_list[recent_cast_event["caster"]][
-                                                "level"
-                                            ]
-                                        )
-                                        # If that players level can cast it
+                                    player_level = player_list[
+                                        recent_cast_event["caster"]
+                                    ]["level"]
+                                    # If we know this players class and level
+                                    if player_class is not None and player_level > 0:
+                                        # If the player class can cast this spell
                                         if (
-                                            int(
-                                                spell_casters["spells"][
-                                                    spell_caster["spell"]
-                                                ]["classes"][player_class]
-                                            )
-                                            <= player_level
+                                            player_class
+                                            in spell_casters["spells"][
+                                                spell_caster["spell"]
+                                            ]["classes"].keys()
                                         ):
-                                            if not find_time:
-                                                identified_spell_caster = (
-                                                    recent_cast_event["caster"]
+                                            # If that players level can cast this spell
+                                            if (
+                                                int(
+                                                    spell_casters["spells"][
+                                                        spell_caster["spell"]
+                                                    ]["classes"][player_class]
                                                 )
-                                                identified_spell_level = player_list[
-                                                    identified_spell_caster
-                                                ]["level"]
-                                                identified_spell = spell_caster["spell"]
-                                                identified_spell_target = target
-                                                find_time = True
-                                            # Favor matched spell with highest level casting requirements
-                                            elif int(
-                                                spell_casters["spells"][
-                                                    identified_spell
-                                                ]["classes"][
-                                                    player_list[
-                                                        identified_spell_caster
-                                                    ]["class"]
-                                                ]
-                                            ) < int(
-                                                spell_casters["spells"][
-                                                    identified_spell
-                                                ]["classes"][
-                                                    player_list[
-                                                        recent_cast_event["caster"]
-                                                    ]["class"]
-                                                ]
+                                                <= player_level
                                             ):
-                                                identified_spell_caster = (
-                                                    recent_cast_event["caster"]
-                                                )
-                                                identified_spell_level = player_list[
-                                                    identified_spell_caster
-                                                ]["level"]
-                                                identified_spell = spell_caster["spell"]
-                                                identified_spell_target = target
+                                                if not find_time:
+                                                    identified_spell_caster = (
+                                                        recent_cast_event["caster"]
+                                                    )
+                                                    identified_spell_level = (
+                                                        player_list[
+                                                            identified_spell_caster
+                                                        ]["level"]
+                                                    )
+                                                    identified_spell = spell_caster[
+                                                        "spell"
+                                                    ]
+                                                    identified_spell_target = target
+                                                    find_time = True
+                                                # Favor matched spell with highest level casting requirements
+                                                elif int(
+                                                    spell_casters["spells"][
+                                                        identified_spell
+                                                    ]["classes"][
+                                                        player_list[
+                                                            identified_spell_caster
+                                                        ]["class"]
+                                                    ]
+                                                ) < int(
+                                                    spell_casters["spells"][
+                                                        identified_spell
+                                                    ]["classes"][
+                                                        player_list[
+                                                            recent_cast_event["caster"]
+                                                        ]["class"]
+                                                    ]
+                                                ):
+                                                    identified_spell_caster = (
+                                                        recent_cast_event["caster"]
+                                                    )
+                                                    identified_spell_level = (
+                                                        player_list[
+                                                            identified_spell_caster
+                                                        ]["level"]
+                                                    )
+                                                    identified_spell = spell_caster[
+                                                        "spell"
+                                                    ]
+                                                    identified_spell_target = target
                                 # TODO: Maybe add an option to assume your player level if player data is not found and your level is sufficient to cast the identified spell?
 
         # We know the spell which landed
         else:
-            if state.debug == "true":
+            if state.debug:
                 eqa_settings.log("Checking for spell: " + spell)
             # If we have spell_caster info on this spell
             if spell in spell_casters["spells"].keys():
                 # Check if player has cast anything
-                if spell_casting_buffer_you:
+                if spell_casting_buffer_you and state.char_level is not None:
                     # If the spell cast by the player is in the spell casters file
                     if (
                         spell_casting_buffer_you["spell"]
                         in spell_casters["spells"].keys()
                     ):
                         # If most recent player cast spell occurred spell time ago to this spell landing
                         if (
@@ -871,39 +942,39 @@
                             identified_spell_level = state.char_level
                             identified_spell = spell_casting_buffer_you["spell"]
                             identified_spell_target = target
                             find_time = True
                         # This spell has no listed classes listed and can be an item cast and you cast it
                         elif (
                             not spell_casters["spells"][spell]["classes"]
-                            and spell_casters["spells"][spell]["item"] == "true"
+                            and spell_casters["spells"][spell]["item"]
                         ):
                             identified_spell_caster = state.char.lower()
                             identified_spell_level = state.char_level
                             identified_spell = spell_casting_buffer_you["spell"]
                             identified_spell_target = target
                             find_time = True
                         # The spell cannot be cast by your class and can be an item cast and you cast it but not spell cast time ago
                         # elif (
                         #    state.char_class.lower()
                         #    not in spell_casters["spells"][spell]["classes"].keys()
-                        #    and spell_casters["spells"][spell]["item"] == "true"
+                        #    and spell_casters["spells"][spell]["item"]
                         # ):
                         #    # TODO: This is where item cast durations would be checked
-                        #    if state.spell_timer_guess == "true":
+                        #    if state.spell_timer_guess:
                         #        identified_spell_caster = state.char.lower()
                         #        identified_spell_level = state.char_level
                         #        identified_spell = spell_casting_buffer_you["spell"]
                         #        identified_spell_target = target
                         #        find_time = True
 
                 # Check for matching spell cast event
                 if not find_time:
                     for recent_cast_event in spell_casting_buffer_other:
-                        if state.debug == "true":
+                        if state.debug:
                             eqa_settings.log("Checking " + recent_cast_event["caster"])
                         if (
                             int(
                                 (
                                     datetime.datetime.strptime(line_time, "%H:%M:%S.%f")
                                     - datetime.datetime.strptime(
                                         recent_cast_event["time"], "%H:%M:%S.%f"
@@ -913,99 +984,109 @@
                                             spell_timers["spells"][spell]["cast_time"]
                                         )
                                     )
                                 ).total_seconds()
                             )
                             == 0
                         ):
-                            if state.debug == "true":
+                            if state.debug:
                                 eqa_settings.log(
                                     "Checking player info for "
                                     + recent_cast_event["caster"]
                                 )
                             # Do we have player info on the likely caster?
                             if recent_cast_event["caster"] in player_list.keys():
                                 player_class = player_list[recent_cast_event["caster"]][
                                     "class"
                                 ]
-                                if (
-                                    player_class
-                                    in spell_casters["spells"][spell]["classes"].keys()
-                                ):
-                                    player_level = int(
-                                        player_list[recent_cast_event["caster"]][
-                                            "level"
-                                        ]
-                                    )
+                                player_level = player_list[recent_cast_event["caster"]][
+                                    "level"
+                                ]
+                                if player_class is not None and player_level > 0:
                                     if (
-                                        int(
-                                            spell_casters["spells"][spell]["classes"][
-                                                player_class
+                                        player_class
+                                        in spell_casters["spells"][spell][
+                                            "classes"
+                                        ].keys()
+                                    ):
+                                        player_level = int(
+                                            player_list[recent_cast_event["caster"]][
+                                                "level"
                                             ]
                                         )
-                                        <= player_level
-                                    ):
-                                        identified_spell_caster = recent_cast_event[
-                                            "caster"
-                                        ]
-                                        identified_spell_level = player_list[
-                                            identified_spell_caster
-                                        ]["level"]
-                                        identified_spell = spell
-                                        identified_spell_target = target
-                                        find_time = True
-                                        if state.debug == "true":
-                                            eqa_settings.log(
-                                                "Found spell cast by "
-                                                + identified_spell_caster
+                                        if (
+                                            int(
+                                                spell_casters["spells"][spell][
+                                                    "classes"
+                                                ][player_class]
                                             )
+                                            <= player_level
+                                        ):
+                                            identified_spell_caster = recent_cast_event[
+                                                "caster"
+                                            ]
+                                            identified_spell_level = player_list[
+                                                identified_spell_caster
+                                            ]["level"]
+                                            identified_spell = spell
+                                            identified_spell_target = target
+                                            find_time = True
+                                            if state.debug:
+                                                eqa_settings.log(
+                                                    "Found spell cast by "
+                                                    + identified_spell_caster
+                                                )
                             # Time to guess the spell level
-                            elif state.spell_timer_guess == "true":
-                                if state.debug == "true":
+                            elif state.spell_timer_guess:
+                                if state.debug:
                                     eqa_settings.log("Into spell guessing territory")
                                 player_level_could_cast = False
                                 # If a player could cast this
                                 if spell_casters["spells"][spell]["classes"]:
                                     # Check if the current player level could cast this (assuming it is a grouped peer or target mob)
                                     for caster_class in spell_casters["spells"][spell][
                                         "classes"
                                     ]:
-                                        if int(state.char_level) >= int(
-                                            spell_casters["spells"][spell]["classes"][
-                                                caster_class
-                                            ]
-                                        ):
-                                            player_level_could_cast = True
+                                        if state.char_level is not None:
+                                            if state.char_level >= int(
+                                                spell_casters["spells"][spell][
+                                                    "classes"
+                                                ][caster_class]
+                                            ):
+                                                player_level_could_cast = True
 
                                     if player_level_could_cast:
                                         identified_spell_level = state.char_level
                                     else:
                                         identified_spell_level = 60
 
                                     identified_spell_caster = recent_cast_event[
                                         "caster"
                                     ]
                                     identified_spell = spell
                                     identified_spell_target = target
                                     find_time = True
 
                                 # If this is a known npc only spell, just set to current player level
-                                elif spell_casters["spells"][spell]["npc"] == "true":
+                                elif (
+                                    spell_casters["spells"][spell]["npc"]
+                                    and state.char_level is not None
+                                ):
                                     identified_spell_caster = recent_cast_event[
                                         "caster"
                                     ]
                                     identified_spell_level = state.char_level
                                     identified_spell = spell
                                     identified_spell_target = target
                                     find_time = True
 
         if find_time:
             make_timer = True
             # If we only want self or guild spell timers
-            if state.spell_timer_guild_only == "true":
+            if state.spell_timer_guild_only and state.char_guild is not None:
                 # If this was cast by myself or another player
                 if identified_spell_caster in player_list.keys():
                     # If a guildie didn't cast it
                     if (
                         not player_list[str(identified_spell_caster)]["guild"]
                         == state.char_guild.lower()
                     ):
@@ -1016,38 +1097,38 @@
                                 == state.char_guild.lower()
                             ):
                                 make_timer = False
                 # If we don't know anything about the identified caster
                 else:
                     make_timer = False
 
-            if state.spell_timer_yours_only == "true":
+            if state.spell_timer_yours_only:
                 if identified_spell_caster != state.char.lower():
                     make_timer = False
 
             # See if this is a timer which will at least last longer than spell timer delay
             spell_duration = spell_formulas(
                 spell_timers["spells"][identified_spell]["formula"],
                 identified_spell_level,
                 spell_timers["spells"][identified_spell]["duration"],
             )
-            if int(spell_duration) <= int(state.spell_timer_delay):
-                if state.debug == "true":
+            if spell_duration <= state.spell_timer_delay:
+                if state.debug:
                     eqa_settings.log("Spell duration too short for timer")
                 make_timer = False
 
             # Set timer message
             if make_timer:
                 if identified_spell_target == state.char.lower():
-                    if int(state.spell_timer_delay) <= 0:
+                    if state.spell_timer_delay <= 0:
                         message = identified_spell.replace("_", " ") + " has worn off"
                     else:
                         message = identified_spell.replace("_", " ") + " is wearing off"
                 else:
-                    if int(state.spell_timer_delay) <= 0:
+                    if state.spell_timer_delay <= 0:
                         message = (
                             identified_spell.replace("_", " ")
                             + " on "
                             + identified_spell_target
                             + " has worn off"
                         )
                     else:
@@ -1056,16 +1137,16 @@
                             + " on "
                             + identified_spell_target
                             + " is wearing off"
                         )
 
                 spell_timer_expire = (
                     datetime.datetime.now()
-                    + datetime.timedelta(seconds=int(spell_duration))
-                    - datetime.timedelta(seconds=int(state.spell_timer_delay))
+                    + datetime.timedelta(seconds=spell_duration)
+                    - datetime.timedelta(seconds=state.spell_timer_delay)
                 )
 
                 # Submit timer
                 timer_q.put(
                     eqa_struct.spell_timer(
                         spell_timer_expire,
                         "spell",
@@ -1075,15 +1156,15 @@
                         spell_duration,
                         datetime.datetime.now(),
                         message,
                     )
                 )
 
                 # Debug logging
-                if state.debug == "true":
+                if state.debug:
                     eqa_settings.log(
                         "Spell timer created for "
                         + identified_spell
                         + " "
                         + identified_spell_caster
                         + "->"
                         + identified_spell_target
@@ -1100,41 +1181,41 @@
             + str(e)
         )
 
 
 def action_mob_timer(timer_q, timer_seconds, auto_mob_timer_delay, zone):
     """Set timer for mob spawn using default zone timer value"""
 
-    timer_seconds = str(int(timer_seconds) - int(auto_mob_timer_delay))
-    if int(timer_seconds) < 0:
-        timer_seconds = "0"
-    if int(auto_mob_timer_delay) <= 0:
+    timer_seconds = timer_seconds - auto_mob_timer_delay
+    if timer_seconds < 0:
+        timer_seconds = 0
+    if auto_mob_timer_delay <= 0:
         pop_message = "Pop " + str(zone)
     else:
         pop_message = (
             "Pop " + str(zone) + " in " + str(auto_mob_timer_delay) + " seconds."
         )
     timer_q.put(
         eqa_struct.timer(
-            (datetime.datetime.now() + datetime.timedelta(seconds=int(timer_seconds))),
+            (datetime.datetime.now() + datetime.timedelta(seconds=timer_seconds)),
             "timer",
             str(timer_seconds),
             pop_message,
         )
     )
 
 
 def send_alerts(line_type, check_line, configs, sound_q, display_q, mute_list):
     """Send messages to sound and display queues"""
 
     try:
         # Check Sender
         sender = re.findall(r"^([\w\-]+)", check_line)
 
-        if configs.alerts.config["line"][line_type]["sound"] == "true":
+        if configs.alerts.config["line"][line_type]["sound"] == True:
             if (
                 not (line_type, sender[0].lower()) in mute_list
                 and not (line_type, "all") in mute_list
             ):
                 sound_q.put(eqa_struct.sound("speak", check_line))
                 display_q.put(
                     eqa_struct.display(
@@ -1150,15 +1231,15 @@
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         line_type + " (MUTED): " + check_line,
                     )
                 )
 
-        elif configs.alerts.config["line"][line_type]["sound"] != "false":
+        elif configs.alerts.config["line"][line_type]["sound"] != False:
             if (
                 not (line_type, sender[0].lower()) in mute_list
                 and not (line_type, "all") in mute_list
             ):
                 sound_q.put(eqa_struct.sound("alert", line_type))
                 display_q.put(
                     eqa_struct.display(
@@ -1192,26 +1273,26 @@
 ):
     """Send keyphrase messages to sound and display queues"""
 
     try:
         # Check Sender
         sender = re.findall(r"^([\w\-]+)", check_line)
 
-        if configs.alerts.config["line"][line_type]["sound"] == "true":
+        if configs.alerts.config["line"][line_type]["sound"] == True:
             if keyphrase == "assist" or keyphrase == "rampage" or keyphrase == "spot":
                 payload = keyphrase + " on " + sender[0]
             else:
                 payload = keyphrase
             if (
                 not (line_type, sender[0].lower()) in mute_list
                 and not (line_type, "all") in mute_list
             ):
-                if context == "true":
+                if context == True:
                     sound_q.put(eqa_struct.sound("speak", check_line))
-                elif context != "false":
+                elif context != False:
                     sound_q.put(eqa_struct.sound("speak", payload))
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         line_type + ": [" + payload + "] " + check_line,
@@ -1223,26 +1304,26 @@
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         line_type + " (MUTED): [" + payload + "] " + check_line,
                     )
                 )
 
-        elif configs.alerts.config["line"][line_type]["sound"] != "false":
+        elif configs.alerts.config["line"][line_type]["sound"] != False:
             if keyphrase == "assist" or keyphrase == "rampage" or keyphrase == "spot":
                 payload = keyphrase + " on " + sender[0]
             else:
                 payload = keyphrase
             if (
                 not (line_type, sender[0].lower()) in mute_list
                 and not (line_type, "all") in mute_list
             ):
-                if context == "true":
+                if context == True:
                     sound_q.put(eqa_struct.sound("alert", line_type))
-                elif context != "false":
+                elif context != False:
                     sound_q.put(eqa_struct.sound("speak", payload))
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
                         "events",
                         line_type + ": [" + payload + "] " + check_line,
@@ -1281,118 +1362,114 @@
                 configs,
                 sound_q,
                 display_q,
                 mute_list,
             )
 
         # Or if line_type reaction is solo_only and you are solo and not in a raid
-        elif (
-            reaction == "solo_only" and state.group == "false" and state.raid == "false"
-        ):
+        elif reaction == "solo_only" and not state.group and not state.raid:
             send_alerts(
                 line_type,
                 check_line,
                 configs,
                 sound_q,
                 display_q,
                 mute_list,
             )
 
         # Or if line_type reaction is solo and you are solo and not in a raid
-        elif reaction == "solo" and state.group == "false" and state.raid == "false":
+        elif reaction == "solo" and not state.group and not state.raid:
             send_alerts(
                 line_type,
                 check_line,
                 configs,
                 sound_q,
                 display_q,
                 mute_list,
             )
 
         # Or if line_type reaction is solo and you are grouped but not in a raid
-        elif reaction == "solo" and state.group == "true" and state.raid == "false":
+        elif reaction == "solo" and state.group and not state.raid:
             send_alerts(
                 line_type,
                 check_line,
                 configs,
                 sound_q,
                 display_q,
                 mute_list,
             )
 
         # Or if line_type reaction is solo_group_only and you are not in a raid
-        elif reaction == "solo_group_only" and state.raid == "false":
+        elif reaction == "solo_group_only" and not state.raid:
             send_alerts(
                 line_type,
                 check_line,
                 configs,
                 sound_q,
                 display_q,
                 mute_list,
             )
 
         # Or if line_type reaction group_only and you are grouped but not in a raid
-        elif (
-            reaction == "group_only" and state.group == "true" and state.raid == "false"
-        ):
+        elif reaction == "group_only" and state.group and not state.raid:
             send_alerts(
                 line_type,
                 check_line,
                 configs,
                 sound_q,
                 display_q,
                 mute_list,
             )
 
         # Or if line_type reaction is group and you are grouped but not in a raid
-        elif reaction == "group" and state.group == "true" and state.raid == "false":
+        elif reaction == "group" and state.group and not state.raid:
             send_alerts(
                 line_type,
                 check_line,
                 configs,
                 sound_q,
                 display_q,
                 mute_list,
             )
 
         # Or if line_type reaction is solo regardless of group state and in a raid
-        elif reaction == "solo" and state.raid == "true":
+        elif reaction == "solo" and state.raid:
             send_alerts(
                 line_type,
                 check_line,
                 configs,
                 sound_q,
                 display_q,
                 mute_list,
             )
 
         # Or if line_type reaction is group regardless of group state and in a raid
-        elif reaction == "group" and state.raid == "true":
+        elif reaction == "group" and state.raid:
             send_alerts(
                 line_type,
                 check_line,
                 configs,
                 sound_q,
                 display_q,
                 mute_list,
             )
 
         # Or if line_type reaction is raid regardless of group state and in a raid
-        elif reaction == "raid" and state.raid == "true":
+        elif reaction == "raid" and state.raid:
             send_alerts(
                 line_type,
                 check_line,
                 configs,
                 sound_q,
                 display_q,
                 mute_list,
             )
 
         # Or if line_type reaction is afk and you are afk
-        elif reaction == "afk" and state.afk == "true":
+        elif reaction == "afk" and state.afk:
             send_alerts(
                 line_type,
                 check_line,
                 configs,
                 sound_q,
                 display_q,
                 mute_list,
@@ -1414,137 +1491,123 @@
 
     try:
         for keyphrase, value in configs.alerts.config["line"][line_type][
             "alert"
         ].items():
             # If the alert value is true
             if str(keyphrase).lower() in check_line.lower():
-                if value == "true":
+                if value == True:
                     send_keyphrase_alerts(
                         line_type,
                         check_line,
                         configs,
                         sound_q,
                         display_q,
                         keyphrase,
                         value,
                         mute_list,
                     )
                 # If the alert value is solo_only
-                elif (
-                    value == "solo_only"
-                    and state.group == "false"
-                    and state.raid == "false"
-                ):
+                elif value == "solo_only" and not state.group and not state.raid:
                     send_keyphrase_alerts(
                         line_type,
                         check_line,
                         configs,
                         sound_q,
                         display_q,
                         keyphrase,
                         value,
                         mute_list,
                     )
                 # If the alert value is solo
-                elif (
-                    value == "solo" and state.group == "false" and state.raid == "false"
-                ):
+                elif value == "solo" and not state.group and not state.raid:
                     send_keyphrase_alerts(
                         line_type,
                         check_line,
                         configs,
                         sound_q,
                         display_q,
                         keyphrase,
                         value,
                         mute_list,
                     )
                 # If the alert value is group
-                elif (
-                    value == "group" and state.group == "true" and state.raid == "false"
-                ):
+                elif value == "group" and state.group and not state.raid:
                     send_keyphrase_alerts(
                         line_type,
                         check_line,
                         configs,
                         sound_q,
                         display_q,
                         keyphrase,
                         value,
                         mute_list,
                     )
                 # If the alert value is group_only
-                elif (
-                    value == "group_only"
-                    and state.group == "true"
-                    and state.raid == "false"
-                ):
+                elif value == "group_only" and state.group and not state.raid:
                     send_keyphrase_alerts(
                         line_type,
                         check_line,
                         configs,
                         sound_q,
                         display_q,
                         keyphrase,
                         value,
                         mute_list,
                     )
                 # If the alert value is solo, but you are grouped
-                elif (
-                    value == "solo" and state.group == "true" and state.raid == "false"
-                ):
+                elif value == "solo" and state.group and not state.raid:
                     send_keyphrase_alerts(
                         line_type,
                         check_line,
                         configs,
                         sound_q,
                         display_q,
                         keyphrase,
                         value,
                         mute_list,
                     )
                 # If the alert value is solo_group_only
-                elif value == "solo_group_only" and state.raid == "false":
+                elif value == "solo_group_only" and not state.raid:
                     send_keyphrase_alerts(
                         line_type,
                         check_line,
                         configs,
                         sound_q,
                         display_q,
                         keyphrase,
                         value,
                         mute_list,
                     )
                 # If the alert value is raid
-                elif value == "raid" and state.raid == "true":
+                elif value == "raid" and state.raid:
                     send_keyphrase_alerts(
                         line_type,
                         check_line,
                         configs,
                         sound_q,
                         display_q,
                         keyphrase,
                         value,
                         mute_list,
                     )
                 # If the alert value is group, but you are in a raid
-                elif value == "group" and state.raid == "true":
+                elif value == "group" and state.raid:
                     send_keyphrase_alerts(
                         line_type,
                         check_line,
                         configs,
                         sound_q,
                         display_q,
                         keyphrase,
                         value,
                         mute_list,
                     )
                 # If the alert value is solo, but you are in a raid
-                elif value == "solo" and state.raid == "true":
+                elif value == "solo" and state.raid:
                     send_keyphrase_alerts(
                         line_type,
                         check_line,
                         configs,
                         sound_q,
                         display_q,
                         keyphrase,
@@ -1599,36 +1662,36 @@
     try:
         # Remove group
         system_q.put(
             eqa_struct.message(
                 eqa_settings.eqa_time(),
                 "system",
                 "group",
-                "null",
-                "false",
+                None,
+                False,
             )
         )
         # Remove group leader
         system_q.put(
             eqa_struct.message(
                 eqa_settings.eqa_time(),
                 "system",
                 "leader",
-                "null",
-                "false",
+                None,
+                False,
             )
         )
         # Remove AFK
         system_q.put(
             eqa_struct.message(
                 eqa_settings.eqa_time(),
                 "system",
                 "afk",
-                "null",
-                "false",
+                None,
+                False,
             )
         )
 
     except Exception as e:
         eqa_settings.log(
             "action motd welcome: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
@@ -1642,24 +1705,24 @@
 
     try:
         system_q.put(
             eqa_struct.message(
                 eqa_settings.eqa_time(),
                 "system",
                 "group",
-                "null",
-                "true",
+                None,
+                True,
             )
         )
         system_q.put(
             eqa_struct.message(
                 eqa_settings.eqa_time(),
                 "system",
                 "leader",
-                "null",
+                None,
                 "you",
             )
         )
 
     except Exception as e:
         eqa_settings.log(
             "action group created: Error on line "
@@ -1674,25 +1737,25 @@
 
     try:
         system_q.put(
             eqa_struct.message(
                 eqa_settings.eqa_time(),
                 "system",
                 "group",
-                "null",
-                "false",
+                None,
+                False,
             )
         )
         system_q.put(
             eqa_struct.message(
                 eqa_settings.eqa_time(),
                 "system",
                 "leader",
-                "null",
-                "false",
+                None,
+                False,
             )
         )
 
     except Exception as e:
         eqa_settings.log(
             "action group removed: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
@@ -1706,25 +1769,25 @@
 
     try:
         system_q.put(
             eqa_struct.message(
                 eqa_settings.eqa_time(),
                 "system",
                 "group",
-                "null",
-                "false",
+                None,
+                False,
             )
         )
         system_q.put(
             eqa_struct.message(
                 eqa_settings.eqa_time(),
                 "system",
                 "leader",
-                "null",
-                "false",
+                None,
+                False,
             )
         )
 
     except Exception as e:
         eqa_settings.log(
             "action group disbanded: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
@@ -1739,24 +1802,24 @@
     try:
         leader = re.findall(r"(?<=You notify )\w+", check_line)
         system_q.put(
             eqa_struct.message(
                 eqa_settings.eqa_time(),
                 "system",
                 "group",
-                "null",
-                "true",
+                None,
+                True,
             )
         )
         system_q.put(
             eqa_struct.message(
                 eqa_settings.eqa_time(),
                 "system",
                 "leader",
-                "null",
+                None,
                 leader[0],
             )
         )
 
     except Exception as e:
         eqa_settings.log(
             "action group joined: Error on line "
@@ -1771,15 +1834,15 @@
 
     try:
         system_q.put(
             eqa_struct.message(
                 eqa_settings.eqa_time(),
                 "system",
                 "leader",
-                "null",
+                None,
                 "you",
             )
         )
 
     except Exception as e:
         eqa_settings.log(
             "action group leader you: Error on line "
@@ -1795,15 +1858,15 @@
     try:
         leader = re.findall(r"^\w+", check_line)
         system_q.put(
             eqa_struct.message(
                 eqa_settings.eqa_time(),
                 "system",
                 "leader",
-                "null",
+                None,
                 leader[0].lower(),
             )
         )
 
     except Exception as e:
         eqa_settings.log(
             "action group leader other: Error on line "
@@ -1818,16 +1881,16 @@
 
     try:
         system_q.put(
             eqa_struct.message(
                 eqa_settings.eqa_time(),
                 "system",
                 "encumbered",
-                "null",
-                "false",
+                None,
+                False,
             )
         )
 
     except Exception as e:
         eqa_settings.log(
             "action encumbered off: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
@@ -1841,16 +1904,16 @@
 
     try:
         system_q.put(
             eqa_struct.message(
                 eqa_settings.eqa_time(),
                 "system",
                 "encumbered",
-                "null",
-                "true",
+                None,
+                True,
             )
         )
 
     except Exception as e:
         eqa_settings.log(
             "action encumbered on: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
@@ -1868,15 +1931,15 @@
             check_line,
         )
         system_q.put(
             eqa_struct.message(
                 eqa_settings.eqa_time(),
                 "system",
                 "direction",
-                "null",
+                None,
                 direction[0],
             )
         )
 
     except Exception as e:
         eqa_settings.log(
             "action direction: Error on line "
@@ -1889,15 +1952,15 @@
 def action_location(system_q, check_line):
     """Perform actions for direction line types"""
 
     try:
         y, x, z = re.findall("[-]?(?:\d*\.)?\d+", check_line)
         loc = [y, x, z]
         system_q.put(
-            eqa_struct.message(eqa_settings.eqa_time(), "system", "loc", "null", loc)
+            eqa_struct.message(eqa_settings.eqa_time(), "system", "loc", None, loc)
         )
 
     except Exception as e:
         eqa_settings.log(
             "action location: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
             + ": "
@@ -2045,149 +2108,149 @@
             elif args[0] == "raid":
                 system_q.put(
                     eqa_struct.message(
                         eqa_settings.eqa_time(),
                         "system",
                         "raid",
                         "toggle",
-                        "null",
+                        None,
                     )
                 )
             elif args[0] == "consider":
-                if state.consider_eval == "true":
+                if state.consider_eval:
                     system_q.put(
                         eqa_struct.message(
                             eqa_settings.eqa_time(),
                             "system",
                             "consider",
                             "eval",
-                            "false",
+                            False,
                         )
                     )
-                elif state.consider_eval == "false":
+                else:
                     system_q.put(
                         eqa_struct.message(
                             eqa_settings.eqa_time(),
                             "system",
                             "consider",
                             "eval",
-                            "true",
+                            True,
                         )
                     )
             elif args[0] == "debug":
                 system_q.put(
                     eqa_struct.message(
                         eqa_settings.eqa_time(),
                         "system",
                         "debug",
                         "toggle",
-                        "null",
+                        None,
                     )
                 )
             elif args[0] == "reload":
                 system_q.put(
                     eqa_struct.message(
                         eqa_settings.eqa_time(),
                         "system",
                         "reload_config",
-                        "null",
-                        "null",
+                        None,
+                        None,
                     )
                 )
             elif args[0] == "encounter":
                 if len(args) == 1:
                     system_q.put(
                         eqa_struct.message(
                             eqa_settings.eqa_time(),
                             "system",
                             "encounter",
                             "toggle",
-                            "null",
+                            None,
                         )
                     )
                 elif args[1] == "clear":
                     system_q.put(
                         eqa_struct.message(
                             eqa_settings.eqa_time(),
                             "system",
                             "encounter",
                             "clear",
-                            "null",
+                            None,
                         )
                     )
                 elif args[1] == "end":
                     system_q.put(
                         eqa_struct.message(
                             eqa_settings.eqa_time(),
                             "system",
                             "encounter",
                             "end",
-                            "null",
+                            None,
                         )
                     )
                 elif args[1] == "start":
                     system_q.put(
                         eqa_struct.message(
                             eqa_settings.eqa_time(),
                             "system",
                             "encounter",
                             "start",
-                            "null",
+                            None,
                         )
                     )
             elif args[0] == "what":
                 if len(args) == 1:
                     sound_q.put(eqa_struct.sound("speak", "What what?"))
                 elif args[1] == "state":
                     sound_q.put(
                         eqa_struct.sound(
                             "speak",
                             "Current State: Playing on: "
                             + state.server
                             + " as "
                             + state.char
                             + " level "
-                            + state.char_level
+                            + str(state.char_level)
                             + " "
-                            + state.char_class
+                            + str(state.char_class)
                             + " of "
-                            + state.char_guild
+                            + str(state.char_guild)
                             + ". Bound in "
-                            + state.bind
+                            + str(state.bind)
                             + " and currently in "
-                            + state.zone
+                            + str(state.zone)
                             + " facing "
-                            + state.direction
+                            + str(state.direction)
                             + " around "
                             + str(state.loc)
                             + ". Group state is "
-                            + state.group
+                            + str(state.group)
                             + ". Leader state is "
-                            + state.leader
+                            + str(state.leader)
                             + ". Raid state is "
-                            + state.raid
+                            + str(state.raid)
                             + ". AFK state is "
-                            + state.afk
+                            + str(state.afk)
                             + ". Encumbered state is "
-                            + state.encumbered
+                            + str(state.encumbered)
                             + ". Debug state is "
-                            + state.debug
+                            + str(state.debug)
                             + ". Encounter parser state is "
-                            + state.encounter_parse,
+                            + str(state.encounter_parse),
                         )
                     )
                 elif args[1] == "context":
-                    if state.afk == "true":
-                        context = "afk"
-                    elif state.group == "false" and state.raid == "false":
+                    if not state.group and not state.raid:
                         context = "solo"
-                    elif state.group == "true" and state.raid == "false":
+                    elif state.group and not state.raid:
                         context = "group"
-                    elif state.raid == "raid":
+                    elif state.raid:
                         context = "raid"
+                    elif state.afk:
+                        context = "afk"
                     sound_q.put(
                         eqa_struct.sound("You are in a " + context + " context.")
                     )
             elif args[0] == "test":
                 if len(args) == 1:
                     sound_q.put(
                         eqa_struct.sound(
@@ -2213,57 +2276,57 @@
                     )
             elif args[0] == "where":
                 if len(args) == 1:
                     sound_q.put(
                         eqa_struct.sound(
                             "speak",
                             "I think you're still in "
-                            + state.zone
+                            + str(state.zone)
                             + ", but considering the circumstances you could be anywhere.",
                         )
                     )
             elif args[0] == "who":
                 if len(args) == 1:
                     sound_q.put(
                         eqa_struct.sound(
                             "speak",
                             "You are " + state.char + ", right?",
                         )
                     )
                 elif args[1] in player_list.keys():
                     if (
-                        player_list[args[1]]["class"] == "unknown"
-                        and player_list[args[1]]["guild"] == "none"
-                        and player_list[args[1]]["level"] == "0"
+                        player_list[args[1]]["class"] == None
+                        and player_list[args[1]]["guild"] == None
+                        and player_list[args[1]]["level"] == 0
                     ):
                         message = "I only know their name"
                     else:
                         message = args[1] + " is "
-                        if int(player_list[args[1]]["level"]) > 0:
+                        if player_list[args[1]]["level"] > 0:
                             message = (
                                 message + " a level " + player_list[args[1]]["level"]
                             )
-                        if not player_list[args[1]]["class"] == "unknown":
+                        if player_list[args[1]]["class"] is not None:
                             message = message + " " + player_list[args[1]]["class"]
                         else:
                             message = message + " character"
-                        if not player_list[args[1]]["guild"] == "none":
+                        if player_list[args[1]]["guild"] is not None:
                             message = message + " in " + player_list[args[1]]["guild"]
                     sound_q.put(eqa_struct.sound("speak", message))
-                elif not args[1] in player_list.keys():
+                else:
                     sound_q.put(eqa_struct.sound("speak", "I'm not sure who that is"))
             elif args[0] == "why":
                 if len(args) == 1:
                     sound_q.put(
                         eqa_struct.sound(
                             "speak",
                             "Did you choose the "
-                            + state.char_class
+                            + str(state.char_class)
                             + " life, or did the "
-                            + state.char_class
+                            + str(state.char_class)
                             + " life choose you?",
                         )
                     )
             elif args[0] == "ping":
                 if len(args) == 1:
                     sound_q.put(
                         eqa_struct.sound(
@@ -2332,15 +2395,15 @@
                     elif args[1] == "respawn":
                         system_q.put(
                             eqa_struct.message(
                                 eqa_settings.eqa_time(),
                                 "system",
                                 "timer",
                                 "mob",
-                                "true",
+                                True,
                             )
                         )
                     else:
                         sound_q.put(
                             eqa_struct.sound(
                                 "speak",
                                 "Something wasn't quite right with that",
@@ -2350,15 +2413,15 @@
                     if args[1] == "respawn" and args[2] == "stop":
                         system_q.put(
                             eqa_struct.message(
                                 eqa_settings.eqa_time(),
                                 "system",
                                 "timer",
                                 "mob",
-                                "false",
+                                False,
                             )
                         )
             else:
                 display_q.put(
                     eqa_struct.display(
                         eqa_settings.eqa_time(),
                         "event",
@@ -2382,16 +2445,16 @@
 
     try:
         system_q.put(
             eqa_struct.message(
                 eqa_settings.eqa_time(),
                 "system",
                 "afk",
-                "null",
-                "false",
+                None,
+                False,
             )
         )
 
     except Exception as e:
         eqa_settings.log(
             "action you afk: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
@@ -2405,16 +2468,16 @@
 
     try:
         system_q.put(
             eqa_struct.message(
                 eqa_settings.eqa_time(),
                 "system",
                 "afk",
-                "null",
-                "true",
+                None,
+                True,
             )
         )
 
     except Exception as e:
         eqa_settings.log(
             "action you afk: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
@@ -2428,15 +2491,15 @@
 
     try:
         system_q.put(
             eqa_struct.message(
                 eqa_settings.eqa_time(),
                 "system",
                 "bind",
-                "null",
+                None,
                 str(state.zone),
             )
         )
 
     except Exception as e:
         eqa_settings.log(
             "action you char bound: Error on line "
@@ -2454,185 +2517,105 @@
             "(?<=You are currently bound in\: )[a-zA-Z\s]+", check_line
         )
         system_q.put(
             eqa_struct.message(
                 eqa_settings.eqa_time(),
                 "system",
                 "bind",
-                "null",
+                None,
                 bound_zone[0],
             )
         )
 
     except Exception as e:
         eqa_settings.log(
             "action you char bound: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
             + ": "
             + str(e)
         )
 
 
-def action_who_player(configs, system_q, state, line, player_list):
-    """Perform actions for who_player line types"""
+def action_who_player(configs, system_q, state, line, player_list, class_mapping):
+    """Parse who_player to determine name, level, class, and guild to update players_list"""
 
     try:
-        if state.char.lower() in line.lower():
-            if re.findall(r"\d+ [a-zA-Z\s]+", line) is not None:
-                char_level, char_class = re.findall(r"\d+ [a-zA-Z\s]+", line)[0].split(
-                    " ", 1
-                )
+        char_level = 0
+        char_class = None
+        char_guild = None
+
+        # Find level and class
+        if re.findall(r"\[\d+ [a-zA-Z\s]+\]", line):
+            char_level, char_class = re.findall(r"\d+ [a-zA-Z\s]+", line)[0].split(
+                " ", 1
+            )
+            char_level = int(char_level)
+            char_class = class_mapping[char_class.lower()]
+
+        # Find guild
+        if re.fullmatch(r".+\<[a-zA-Z\s]+\>(.+|)", line) is not None:
+            char_guild = re.findall(r"(?<=\<)[a-zA-Z\s]+", line)[0].lower()
+
+        # Find name
+        char_name = re.findall(r"(?<=\]\ )[a-zA-Z]+", line)[0].lower()
+
+        # Update players_list
+        if char_name in player_list.keys():
+            if char_guild is not None:
+                if char_guild != player_list[char_name]["guild"]:
+                    player_list[char_name]["guild"] = char_guild
+            if char_level > 0:
+                if char_level != player_list[char_name]["level"]:
+                    player_list[char_name]["level"] = char_level
+            if char_class is not None:
+                if char_class != player_list[char_name]["class"]:
+                    player_list[char_name]["class"] = char_class
+        else:
+            player_list[char_name] = {
+                "class": char_class,
+                "level": char_level,
+                "guild": char_guild,
+            }
+
+        # Update internal character state
+        if state.char.lower() == char_name:
+            if char_level > 0:
                 system_q.put(
                     eqa_struct.message(
                         eqa_settings.eqa_time(),
                         "system",
                         "level",
-                        "null",
+                        None,
                         char_level,
                     )
                 )
+
+            if char_class is not None:
                 system_q.put(
                     eqa_struct.message(
                         eqa_settings.eqa_time(),
                         "system",
                         "class",
-                        "null",
-                        char_class,
+                        None,
+                        char_class.title(),
                     )
                 )
 
-            if re.fullmatch(r".+\<[a-zA-Z\s]+\>(.+|)", line) is not None:
+            if char_guild is not None:
                 char_guild = re.findall(r"(?<=\<)[a-zA-Z\s]+", line)[0]
                 system_q.put(
                     eqa_struct.message(
                         eqa_settings.eqa_time(),
                         "system",
                         "guild",
-                        "null",
+                        None,
                         char_guild,
                     )
                 )
 
-        char_level = "0"
-        char_class = "unknown"
-        char_guild = "none"
-
-        # Parse who_player to determine name, level, guild
-        if re.findall(r"\[\d+ [a-zA-Z\s]+\]", line):
-            char_level, char_class = re.findall(r"\d+ [a-zA-Z\s]+", line)[0].split(
-                " ", 1
-            )
-
-        if re.fullmatch(r".+\<[a-zA-Z\s]+\>(.+|)", line) is not None:
-            char_guild = re.findall(r"(?<=\<)[a-zA-Z\s]+", line)[0].lower()
-
-        char_name = re.findall(r"(?<=\]\ )[a-zA-Z]+", line)[0].lower()
-
-        char_class = char_class.lower()
-
-        if (
-            char_class == "minstrel"
-            or char_class == "troubadour"
-            or char_class == "virtuoso"
-        ):
-            char_class = "bard"
-        elif (
-            char_class == "vicar"
-            or char_class == "templar"
-            or char_class == "high priest"
-        ):
-            char_class = "cleric"
-        elif (
-            char_class == "wanderer"
-            or char_class == "preserver"
-            or char_class == "hierophant"
-        ):
-            char_class = "druid"
-        elif (
-            char_class == "illusionist"
-            or char_class == "beguiler"
-            or char_class == "phantasmist"
-        ):
-            char_class = "enchanter"
-        elif (
-            char_class == "elementalist"
-            or char_class == "conjurer"
-            or char_class == "arch mage"
-        ):
-            char_class = "magician"
-        elif (
-            char_class == "disciple"
-            or char_class == "master"
-            or char_class == "grandmaster"
-        ):
-            char_class = "monk"
-        elif (
-            char_class == "heretic"
-            or char_class == "defiler"
-            or char_class == "warlock"
-        ):
-            char_class = "necromancer"
-        elif (
-            char_class == "cavalier"
-            or char_class == "knight"
-            or char_class == "crusader"
-        ):
-            char_class = "paladin"
-        elif (
-            char_class == "pathfinder"
-            or char_class == "outrider"
-            or char_class == "warder"
-        ):
-            char_class = "ranger"
-        elif (
-            char_class == "rake"
-            or char_class == "blackguard"
-            or char_class == "assassin"
-        ):
-            char_class = "rogue"
-        elif (
-            char_class == "reaver"
-            or char_class == "revenant"
-            or char_class == "grave lord"
-        ):
-            char_class = "shadow knight"
-        elif (
-            char_class == "mystic" or char_class == "luminary" or char_class == "oracle"
-        ):
-            char_class = "shaman"
-        elif (
-            char_class == "champion"
-            or char_class == "myrmidon"
-            or char_class == "warlord"
-        ):
-            char_class = "warrior"
-        elif (
-            char_class == "channeler"
-            or char_class == "evoker"
-            or char_class == "sorcerer"
-        ):
-            char_class = "wizard"
-
-        if char_name in player_list.keys():
-            if char_guild != "none" and char_guild != player_list[char_name]["guild"]:
-                player_list[char_name]["guild"] = char_guild
-            if char_level != "0" and char_level != player_list[char_name]["level"]:
-                player_list[char_name]["level"] = char_level
-            if (
-                char_class != "unknown"
-                and char_class != player_list[char_name]["class"]
-            ):
-                player_list[char_name]["class"] = char_class
-        else:
-            player_list[char_name] = {
-                "class": char_class,
-                "level": char_level,
-                "guild": char_guild,
-            }
-
     except Exception as e:
         eqa_settings.log(
             "action who player: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
             + ": "
             + str(e)
         )
@@ -2646,70 +2629,62 @@
     try:
         current_zone = re.findall("(?<=You have entered )[a-zA-Z\-'\s]+", check_line)
         system_q.put(
             eqa_struct.message(
                 eqa_settings.eqa_time(),
                 "system",
                 "afk",
-                "null",
-                "false",
+                None,
+                False,
             )
         )
 
         if current_zone[0] != state.zone:
             display_q.put(
                 eqa_struct.display(
                     eqa_settings.eqa_time(), "update", "zone", current_zone[0]
                 )
             )
             system_q.put(
                 eqa_struct.message(
                     eqa_settings.eqa_time(),
                     "system",
                     "zone",
-                    "null",
+                    None,
                     current_zone[0],
                 )
             )
 
         if current_zone[0] not in configs.zones.config["zones"].keys():
             eqa_config.add_zone(current_zone[0], base_path)
-        elif (
-            current_zone[0] in configs.zones.config["zones"].keys()
-            and not state.raid == "true"
-        ):
+        elif current_zone[0] in configs.zones.config["zones"].keys() and not state.raid:
             if (
-                configs.zones.config["zones"][current_zone[0]]["raid_mode"] == "true"
-                and configs.settings.config["settings"]["raid_mode"]["auto_set"]
-                == "true"
+                configs.zones.config["zones"][current_zone[0]]["raid_mode"]
+                and state.auto_raid
             ):
                 system_q.put(
                     eqa_struct.message(
                         eqa_settings.eqa_time(),
                         "system",
                         "raid",
-                        "true",
+                        True,
                         "Raid mode auto-enabled",
                     )
                 )
-        elif (
-            current_zone[0] in configs.zones.config["zones"].keys()
-            and state.raid == "true"
-        ):
+        elif current_zone[0] in configs.zones.config["zones"].keys() and state.raid:
             if (
-                configs.zones.config["zones"][current_zone[0]]["raid_mode"] == "false"
-                and configs.settings.config["settings"]["raid_mode"]["auto_set"]
-                == "true"
+                not configs.zones.config["zones"][current_zone[0]]["raid_mode"]
+                and state.auto_raid
             ):
                 system_q.put(
                     eqa_struct.message(
                         eqa_settings.eqa_time(),
                         "system",
                         "raid",
-                        "false",
+                        False,
                         "Raid mode auto-disabled",
                     )
                 )
 
         timer_q.put(
             eqa_struct.timer(
                 datetime.datetime.now(),
@@ -2724,25 +2699,23 @@
             "action you new zone: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
             + ": "
             + str(e)
         )
 
 
-def action_matched(line_type, line, base_path):
+def action_matched(line_type, line, base_path, version):
     """Debug function to log all log lines and matches log lines"""
 
     try:
         matched_log = base_path + "log/debug/matched-lines.txt"
         if os.path.exists(matched_log):
             file_size = os.path.getsize(matched_log)
             if file_size >= 10000000:
-                version = str(
-                    pkg_resources.get_distribution("eqalert").version
-                ).replace(".", "-")
+                version = version.replace(".", "-")
                 archived_log = (
                     base_path
                     + "log/debug/matched-lines_"
                     + version
                     + "_"
                     + str(datetime.datetime.now().date())
                     + ".txt"
```

### Comparing `eqalert-3.5.0/eqa/lib/config.py` & `eqalert-3.5.1/eqa/lib/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,27 +17,26 @@
    with this program; if not, write to the Free Software Foundation, Inc.,
    51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 """
 
 import json
 import os
 import sys
-import pkg_resources
 import re
 import hashlib
 
 import eqa.lib.settings as eqa_settings
 import eqa.lib.state as eqa_state
 import eqa.lib.struct as eqa_struct
 
 
-def init(base_path):
+def init(base_path, version):
     """Create any missing config files"""
     try:
-        generated = build_config(base_path)
+        generated = build_config(base_path, version)
 
         if generated:
             print("One or more new versioned configuration files have been generated.")
             print("Older files have been archived under config/archive/\n")
             print("Please validate your config/settings.json and relaunch eqalert.")
             exit(0)
 
@@ -213,15 +212,15 @@
             "config read: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
             + ": "
             + str(e)
         )
 
 
-def update_logs(configs):
+def update_logs(configs, version):
     """Add characters and servers of eqemu_ prefixed files in the log path"""
 
     try:
         log_files = [
             f
             for f in os.listdir(
                 configs.settings.config["settings"]["paths"]["everquest_logs"]
@@ -240,14 +239,16 @@
                 char_name = middle
                 char_server = char_name + "_" + server_name
                 if char_server not in configs.characters.config["char_logs"].keys():
                     add_char_log(char_name, server_name, configs)
                 if len(configs.settings.config["last_state"].keys()) == 0:
                     bootstrap_state(configs, char_name, server_name)
 
+        validate_char_log(configs, version)
+
     except Exception as e:
         print(
             "set config chars: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
             + ": "
             + str(e)
         )
@@ -267,24 +268,24 @@
 
         configs.characters.config["char_logs"].update(
             {
                 char_server: {
                     "character": char,
                     "server": server,
                     "file_name": char_log,
-                    "disabled": "false",
+                    "disabled": False,
                     "char_state": {
                         "location": {"x": "0.00", "y": "0.00", "z": "0.00"},
-                        "direction": "unavailable",
-                        "zone": "unavailable",
-                        "encumbered": "false",
-                        "bind": "unavailable",
-                        "level": "unavailable",
-                        "class": "unavailable",
-                        "guild": "unavailable",
+                        "direction": None,
+                        "zone": None,
+                        "encumbered": False,
+                        "bind": None,
+                        "level": None,
+                        "class": None,
+                        "guild": None,
                     },
                 }
             }
         )
         json_data = open(configs.characters.path, "w", encoding="utf-8")
         json.dump(configs.characters.config, json_data, sort_keys=True, indent=2)
         json_data.close()
@@ -300,27 +301,131 @@
             "add char: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
             + ": "
             + str(e)
         )
 
 
+def validate_char_log(configs, version):
+    """Validate characters.json"""
+
+    try:
+        json_data = open(configs.characters.path, "r", encoding="utf-8")
+        characters_json_data = json.load(json_data)
+        json_data.close()
+
+        if "version" in characters_json_data.keys():
+            # For any future needed changes
+            pass
+        else:
+            # no version
+            for char_log in characters_json_data["char_logs"].keys():
+                if (
+                    characters_json_data["char_logs"][char_log]["char_state"]["bind"]
+                    == "unavailable"
+                ):
+                    characters_json_data["char_logs"][char_log]["char_state"][
+                        "bind"
+                    ] = None
+                if (
+                    characters_json_data["char_logs"][char_log]["char_state"]["class"]
+                    == "unavailable"
+                ):
+                    characters_json_data["char_logs"][char_log]["char_state"][
+                        "class"
+                    ] = None
+                if (
+                    characters_json_data["char_logs"][char_log]["char_state"][
+                        "direction"
+                    ]
+                    == "unavailable"
+                ):
+                    characters_json_data["char_logs"][char_log]["char_state"][
+                        "direction"
+                    ] = None
+                if (
+                    characters_json_data["char_logs"][char_log]["char_state"][
+                        "encumbered"
+                    ]
+                    == "false"
+                ):
+                    characters_json_data["char_logs"][char_log]["char_state"][
+                        "encumbered"
+                    ] = False
+                if (
+                    characters_json_data["char_logs"][char_log]["char_state"][
+                        "encumbered"
+                    ]
+                    == "true"
+                ):
+                    characters_json_data["char_logs"][char_log]["char_state"][
+                        "encumbered"
+                    ] = True
+                if (
+                    characters_json_data["char_logs"][char_log]["char_state"]["guild"]
+                    == "unavailable"
+                ):
+                    characters_json_data["char_logs"][char_log]["char_state"][
+                        "guild"
+                    ] = None
+                if (
+                    characters_json_data["char_logs"][char_log]["char_state"]["level"]
+                    == "unavailable"
+                ):
+                    characters_json_data["char_logs"][char_log]["char_state"][
+                        "level"
+                    ] = None
+                else:
+                    characters_json_data["char_logs"][char_log]["char_state"][
+                        "level"
+                    ] = int(
+                        characters_json_data["char_logs"][char_log]["char_state"][
+                            "level"
+                        ]
+                    )
+                if (
+                    characters_json_data["char_logs"][char_log]["char_state"]["zone"]
+                    == "unavailable"
+                ):
+                    characters_json_data["char_logs"][char_log]["char_state"][
+                        "zone"
+                    ] = None
+                if characters_json_data["char_logs"][char_log]["disabled"] == "false":
+                    characters_json_data["char_logs"][char_log]["disabled"] = False
+                if characters_json_data["char_logs"][char_log]["disabled"] == "true":
+                    characters_json_data["char_logs"][char_log]["disabled"] = True
+
+            characters_json_data["version"] = version
+
+            json_data = open(configs.characters.path, "w", encoding="utf-8")
+            json.dump(characters_json_data, json_data, sort_keys=True, indent=2)
+            json_data.close()
+
+    except Exception as e:
+        eqa_settings.log(
+            "validate char log: Error on line "
+            + str(sys.exc_info()[-1].tb_lineno)
+            + ": "
+            + str(e)
+        )
+
+
 def bootstrap_state(configs, char, server):
     """Generate and save state to config"""
 
     try:
         data = configs.settings.config
         data["last_state"].update(
             {
                 "server": server,
                 "character": char,
-                "afk": "false",
-                "group": "false",
-                "leader": "false",
-                "raid": "false",
+                "afk": False,
+                "group": False,
+                "leader": False,
+                "raid": False,
             }
         )
         json_data = open(configs.settings.path, "w", encoding="utf-8")
         json.dump(data, json_data, sort_keys=True, indent=2)
         json_data.close()
 
     except Exception as e:
@@ -333,18 +438,15 @@
 
 
 def get_config_chars(configs):
     """Return each unique character log"""
     try:
         chars = []
         for char_server in configs.characters.config["char_logs"].keys():
-            if (
-                configs.characters.config["char_logs"][char_server]["disabled"]
-                == "false"
-            ):
+            if not configs.characters.config["char_logs"][char_server]["disabled"]:
                 chars.append(char_server)
 
         return chars
 
     except Exception as e:
         eqa_settings.log(
             "get config chars: Error on line "
@@ -390,4718 +492,4719 @@
             "get spell casters: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
             + ": "
             + str(e)
         )
 
 
-def update_spell_casters(data_path):
+def update_spell_casters(data_path, version):
     """Update data/spell-casters.json"""
 
     new_spell_caster_data = """
+
 {
   "spells": {
     "aanyas_quickening": {
       "classes": {
         "enchanter": "53"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "accuracy": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "acid_jet": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "acumen": {
       "classes": {
         "shaman": 56
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "adorning_grace": {
       "classes": {
         "enchanter": "49"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "adroitness": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "aegis": {
       "classes": {
         "cleric": 57
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "aegis_of_bathezid": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "aegis_of_ro": {
       "classes": {
         "magician": 60
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "aegolism": {
       "classes": {
         "cleric": 60
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "affliction": {
       "classes": {
         "shaman": 19
       },
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "agility": {
       "classes": {
         "shaman": 44
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "agilmentes_aria_of_eagles": {
       "classes": {
         "bard": 31
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "alacrity": {
       "classes": {
         "enchanter": "24",
         "shaman": 44
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "allure": {
       "classes": {
         "enchanter": "49"
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "allure_of_death": {
       "classes": {
         "necromancer": 20
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "allure_of_the_wild": {
       "classes": {
         "druid": 44
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "alluring_aura": {
       "classes": {
         "shaman": 29
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "alluring_whispers": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "aloe_sweat": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "ancient_breath": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "anthem_de_arms": {
       "classes": {
         "bard": 10
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "arch_lich": {
       "classes": {
         "necromancer": 60
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "arch_shielding": {
       "classes": {
         "enchanter": "44",
         "magician": 44,
         "necromancer": 44,
         "wizard": 44
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "armor_of_faith": {
       "classes": {
         "cleric": 39,
         "paladin": 49
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "armor_of_protection": {
       "classes": {
         "cleric": 34
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "asphyxiate": {
       "classes": {
         "enchanter": "59"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "assiduous_vision": {
       "classes": {
         "shaman": 39
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "asystole": {
       "classes": {
         "necromancer": 44,
         "shadow knight": 60
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "atols_spectral_shackles": {
       "classes": {
         "wizard": 51
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "augment": {
       "classes": {
         "enchanter": "56"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "augment_death": {
       "classes": {
         "necromancer": 39
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "augmentation": {
       "classes": {
         "enchanter": "29"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "augmentation_of_death": {
       "classes": {
         "necromancer": 55
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "aura_of_antibody": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "aura_of_battle": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "aura_of_black_petals": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "aura_of_blue_petals": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "aura_of_cold": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "aura_of_green_petals": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "aura_of_heat": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "aura_of_marr": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "aura_of_purity": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "aura_of_red_petals": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "aura_of_white_petals": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "avatar": {
       "classes": {
         "shaman": "60"
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "avatar_snare": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "bane_of_nife": {
       "classes": {
         "shaman": 56
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "banshee_aura": {
       "classes": {
         "necromancer": 16,
         "shadow knight": 54
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "barbcoat": {
       "classes": {
         "druid": 19,
         "ranger": 30
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "barrier_of_combustion": {
       "classes": {
         "magician": 39
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "barrier_of_force": {
       "classes": {},
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "battery_vision": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "bedlam": {
       "classes": {
         "enchanter": "58"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "befriend_animal": {
       "classes": {
         "druid": 14,
         "shaman": 29
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "beguile": {
       "classes": {
         "enchanter": "24"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "beguile_animals": {
       "classes": {
         "druid": 34
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "beguile_plants": {
       "classes": {
         "druid": 29
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "beguile_undead": {
       "classes": {
         "necromancer": 34
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "bellowing_winds": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "berserker_madness_i": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "berserker_madness_ii": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "berserker_madness_iii": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "berserker_madness_iv": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "berserker_spirit": {
       "classes": {
         "enchanter": "49"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "berserker_strength": {
       "classes": {
         "enchanter": "20"
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "bind_sight": {
       "classes": {
         "enchanter": "8",
         "ranger": 22,
         "wizard": 16
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "bladecoat": {
       "classes": {
         "druid": 56
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "blessing_of_nature": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "blessing_of_the_grove": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "blinding_fear": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "blinding_luminance": {
       "classes": {
         "cleric": 34,
         "shaman": 39
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "blinding_poison_i": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "blinding_poison_iii": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "blinding_step": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "blood_claw": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "bobbing_corpse": {
       "classes": {
         "shadow knight": 55
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "boil_blood": {
       "classes": {
         "necromancer": 29,
         "shadow knight": 53
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "boiling_blood": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "boltrans_agacerie": {
       "classes": {
         "enchanter": "53"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "bond_of_death": {
       "classes": {
         "necromancer": 49
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "bonds_of_force": {
       "classes": {
         "wizard": 29
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "bonds_of_tunare": {
       "classes": {
         "druid": 57
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "bone_melt": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "boon_of_immolation": {
       "classes": {
         "magician": 53
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "boon_of_the_clear_mind": {
       "classes": {
         "enchanter": "52"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "boon_of_the_garou": {
       "classes": {
         "enchanter": "44"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "bramblecoat": {
       "classes": {
         "druid": 29,
         "ranger": 39
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "bravery": {
       "classes": {
         "cleric": 24
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "breath_of_ro": {
       "classes": {
         "druid": 52
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "breath_of_the_dead": {
       "classes": {
         "necromancer": 24,
         "shadow knight": 49
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "breath_of_the_sea": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "breeze": {
       "classes": {
         "enchanter": "16"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "brilliance": {
       "classes": {
         "enchanter": "44"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "brittle_haste_i": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "brittle_haste_ii": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "brittle_haste_iii": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "brittle_haste_iv": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "bulwark_of_faith": {
       "classes": {
         "cleric": 57
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "burnout": {
       "classes": {
         "magician": 255
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "burnout_ii": {
       "classes": {
         "magician": 29
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "burnout_iii": {
       "classes": {
         "magician": 49
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "burnout_iv": {
       "classes": {
         "magician": 55
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "burrowing_scarab": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "burst_of_strength": {
       "classes": {
         "shaman": 14
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "cadeau_of_flame": {
       "classes": {
         "magician": 56
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "cajole_undead": {
       "classes": {
         "necromancer": 49
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "calimony": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "call_of_bones": {
       "classes": {
         "necromancer": 34
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "call_of_earth": {
       "classes": {
         "ranger": 50
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "call_of_karana": {
       "classes": {
         "druid": 52
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "call_of_sky": {
       "classes": {
         "ranger": 39
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "call_of_the_predator": {
       "classes": {
         "ranger": 60
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "calm": {
       "classes": {
         "cleric": 19,
         "enchanter": "20",
         "paladin": 49
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "calm_animal": {
       "classes": {
         "druid": 19,
         "ranger": 39
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "camouflage": {
       "classes": {
         "druid": 5,
         "ranger": 15
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "captain_nalots_quickening": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "cascading_darkness": {
       "classes": {
         "necromancer": 49,
         "shadow knight": 59
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "cassindras_chant_of_clarity": {
       "classes": {
         "bard": 20
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "cassindras_elegy": {
       "classes": {
         "bard": 44
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "cassindras_insipid_ditty": {
       "classes": {
         "bard": 57
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "cast_sight": {
       "classes": {
         "enchanter": "34"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "celerity": {
       "classes": {
         "enchanter": "39",
         "shaman": 56
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "celestial_cleansing": {
       "classes": {
         "paladin": 59
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "celestial_healing": {
       "classes": {
         "cleric": 44
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "celestial_tranquility": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "center": {
       "classes": {
         "cleric": 9,
         "paladin": 22
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "cessation_of_cor": {
       "classes": {
         "necromancer": 56
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "chant_of_battle": {
       "classes": {
         "bard": 1
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "charisma": {
       "classes": {
         "shaman": 49
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "chase_the_moon": {
       "classes": {
         "enchanter": "16"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "chill_bones": {
       "classes": {
         "necromancer": 55
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "chill_of_unlife": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "chill_sight": {
       "classes": {
         "ranger": 56,
         "wizard": 39
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "chilling_embrace": {
       "classes": {
         "necromancer": 39
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "chloroplast": {
       "classes": {
         "druid": 44,
         "ranger": 55,
         "shaman": 39
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "choke": {
       "classes": {
         "enchanter": "12"
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "chords_of_dissonance": {
       "classes": {
         "bard": 2
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "cindas_charismatic_carillon": {
       "classes": {
         "bard": 11
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "circle_of_summer": {
       "classes": {
         "druid": 52
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "circle_of_winter": {
       "classes": {
         "druid": 51
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "clarity": {
       "classes": {
         "enchanter": "29"
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "clarity_ii": {
       "classes": {
         "enchanter": "54"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "clinging_darkness": {
       "classes": {
         "necromancer": 4,
         "shadow knight": 15
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "clockwork_poison": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "cloud": {
       "classes": {
         "enchanter": "20"
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "cloud_of_disempowerment": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "cloud_of_fear": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "cloud_of_silence": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "cog_boost": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "cohesion": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "composition_of_ervaj": {
       "classes": {
         "bard": 60
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "courage": {
       "classes": {
         "cleric": 1,
         "paladin": 9
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "creeping_crud": {
       "classes": {
         "druid": 24
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "creeping_vision": {
       "classes": {
         "shaman": 24
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "cripple": {
       "classes": {
         "enchanter": "53",
         "shaman": 53
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "crissions_pixie_strike": {
       "classes": {
         "bard": 28
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "curse_of_the_simple_mind": {
       "classes": {
         "enchanter": "29"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "curse_of_the_spirits": {
       "classes": {},
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "dance_of_the_blade": {
       "classes": {},
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "daring": {
       "classes": {
         "cleric": 19,
         "paladin": 39
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "dark_pact": {
       "classes": {
         "necromancer": 8
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "dawncall": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "dazzle": {
       "classes": {
         "enchanter": "49"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "dead_man_floating": {
       "classes": {
         "necromancer": 44
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "dead_men_floating": {
       "classes": {
         "necromancer": 49
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "deadeye": {
       "classes": {
         "necromancer": 8,
         "shadow knight": 22
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "deadly_poison": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "deadly_velium_poison": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "death_pact": {
       "classes": {
         "cleric": 51
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "deftness": {
       "classes": {
         "shaman": 39
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "deliriously_nimble": {
       "classes": {
         "shaman": 53
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "demi_lich": {
       "classes": {
         "necromancer": 60
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "denons_bereavement": {
       "classes": {
         "bard": 59
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "denons_disruptive_discord": {
       "classes": {
         "bard": 18
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "desperate_hope": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "devouring_darkness": {
       "classes": {
         "necromancer": 59
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "dexterity": {
       "classes": {
         "shaman": 49
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "dexterous_aura": {
       "classes": {
         "shaman": 1
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "diamondskin": {
       "classes": {
         "necromancer": 44,
         "shadow knight": 59,
         "wizard": 44
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "dictate": {
       "classes": {
         "enchanter": "60"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "disease": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "disease_cloud": {
       "classes": {
         "necromancer": 1,
         "shadow knight": 9
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "diseased_cloud": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "disempower": {
       "classes": {
         "enchanter": "16",
         "shaman": 14
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "divine_aura": {
       "classes": {
         "cleric": 1,
         "paladin": 55
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "divine_barrier": {
       "classes": {
         "cleric": 29
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "divine_favor": {
       "classes": {
         "paladin": 55
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "divine_glory": {
       "classes": {
         "paladin": 53
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "divine_intervention": {
       "classes": {
         "cleric": 60
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "divine_might": {
       "classes": {
         "paladin": 49
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "divine_purpose": {
       "classes": {
         "paladin": 39
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "divine_strength": {
       "classes": {
         "paladin": 60
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "dizzy_i": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "dizzy_ii": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "dizzy_iii": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "dizzy_iv": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "dominate_undead": {
       "classes": {
         "necromancer": 20
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "dooming_darkness": {
       "classes": {
         "necromancer": 29,
         "shadow knight": 49
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "draconic_rage": {
       "classes": {},
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "dragon_charm": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "dragon_roar": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "drifting_death": {
       "classes": {
         "druid": 44
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "drones_of_doom": {
       "classes": {
         "druid": 34,
         "ranger": 54
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "drowsy": {
       "classes": {
         "shaman": 5
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "dulsehound": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "dyns_dizzying_draught": {
       "classes": {
         "enchanter": "29"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "earthcall": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "earthelementalattack": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "ebbing_strength": {
       "classes": {
         "enchanter": "12"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "echinacea_infusion": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "elemental_armor": {
       "classes": {
         "magician": 44,
         "wizard": 44
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "elemental_maelstrom": {
       "classes": {
         "magician": 44
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "elemental_rhythms": {
       "classes": {
         "bard": 9
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "elemental_shield": {
       "classes": {
         "magician": 20,
         "wizard": 20
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "embrace_of_the_kelpmaiden": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "endure_cold": {
       "classes": {
         "cleric": 14,
         "druid": 9,
         "necromancer": 4,
         "ranger": 22,
         "shadow knight": 15,
         "shaman": 1
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "endure_disease": {
       "classes": {
         "cleric": 14,
         "druid": 19,
         "paladin": 39,
         "shadow knight": 30,
         "shaman": 9,
         "necromancer": 12
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "endure_fire": {
       "classes": {
         "cleric": 9,
         "druid": 1,
         "ranger": 9,
         "shaman": 5
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "endure_magic": {
       "classes": {
         "cleric": 19,
         "druid": 34,
         "enchanter": "20",
         "paladin": 30,
         "shaman": 19
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "endure_poison": {
       "classes": {
         "cleric": 9,
         "druid": 19,
         "paladin": 22,
         "shaman": 14
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "enduring_breath": {
       "classes": {
         "druid": 9,
         "enchanter": "12",
         "ranger": 22,
         "shaman": 14
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "energy_sap": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "enfeeblement": {
       "classes": {
         "enchanter": "4"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "engulfing_darkness": {
       "classes": {
         "necromancer": 12,
         "shadow knight": 22
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "enlightenment": {
       "classes": {
         "enchanter": "57"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "enslave_death": {
       "classes": {
         "necromancer": 60
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "ensnare": {
       "classes": {
         "druid": 29,
         "ranger": 51
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "enthrall": {
       "classes": {
         "enchanter": "16"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "entrance": {
       "classes": {
         "enchanter": "34"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "envenomed_bolt": {
       "classes": {
         "necromancer": 51,
         "shaman": 49
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "envenomed_breath": {
       "classes": {
         "shaman": 24
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "everlasting_breath": {
       "classes": {},
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "expedience": {
       "classes": {
         "magician": 29
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "extended_regeneration": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "eye_of_confusion": {
       "classes": {
         "enchanter": "8"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "eye_of_tallon": {
       "classes": {
         "magician": 57,
         "wizard": 57
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "eye_of_zomm": {
       "classes": {
         "magician": 8,
         "wizard": 8
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "eyes_of_the_cat": {
       "classes": {
         "ranger": 30
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "fascination": {
       "classes": {
         "enchanter": "52"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "feast_of_blood": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "feckless_might": {
       "classes": {
         "enchanter": "20"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "feeble_poison": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "feedback": {
       "classes": {
         "enchanter": "29"
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "feet_like_cat": {
       "classes": {
         "ranger": 15,
         "shaman": 5
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "fellspine": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "feral_spirit": {
       "classes": {
         "druid": 19
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "fetter": {
       "classes": {
         "enchanter": "58",
         "wizard": 58
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "fiery_might": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "fire": {
       "classes": {
         "druid": 49
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "firefist": {
       "classes": {
         "druid": 9,
         "ranger": 22
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "fist_of_water": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "fixation_of_ro": {
       "classes": {
         "druid": 44
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "flame_lick": {
       "classes": {
         "druid": 1,
         "ranger": 9
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "flash_of_light": {
       "classes": {
         "cleric": 1,
         "paladin": 9,
         "shaman": 1
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "fleeting_fury": {
       "classes": {
         "shaman": 5
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "flesh_rot_i": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "flesh_rot_ii": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "flesh_rot_iii": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "flurry": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "focus_of_spirit": {
       "classes": {
         "shaman": 60
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "forlorn_deeds": {
       "classes": {
         "enchanter": "57"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "form_of_the_great_bear": {
       "classes": {
         "shaman": 55
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "form_of_the_great_wolf": {
       "classes": {
         "druid": 44
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "form_of_the_howler": {
       "classes": {
         "druid": 54
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "form_of_the_hunter": {
       "classes": {
         "druid": 60
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "fortitude": {
       "classes": {
         "cleric": 55
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "freezing_breath": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "frenzied_strength": {
       "classes": {
         "cleric": 34,
         "paladin": 52
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "frenzy": {
       "classes": {
         "shaman": 19
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "froglok_poison": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "frost_storm": {
       "classes": {
         "wizard": 44
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "frostbite": {
       "classes": {},
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "frostreavers_blessing": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "fufils_curtailing_chant": {
       "classes": {
         "bard": "30"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "fungal_regrowth": {
       "classes": {},
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "fungus_spores": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "furious_strength": {
       "classes": {
         "shaman": 39
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "fury": {
       "classes": {
         "shaman": 34
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "garzicors_vengeance": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "gasping_embrace": {
       "classes": {
         "enchanter": "49"
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "gaze": {
       "classes": {
         "wizard": 12
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "gift_of_brilliance": {
       "classes": {
         "enchanter": "60"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "gift_of_insight": {
       "classes": {
         "enchanter": "55"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "gift_of_magic": {
       "classes": {
         "enchanter": "34"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "gift_of_pure_thought": {
       "classes": {
         "enchanter": "59"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "girdle_of_karana": {
       "classes": {
         "druid": 55
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "glamour": {
       "classes": {
         "shaman": 39
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "glamour_of_kintaz": {
       "classes": {
         "enchanter": "54"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "glamour_of_tunare": {
       "classes": {
         "druid": 53
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "glimpse": {
       "classes": {
         "druid": 4,
         "ranger": 9
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "graveyard_dust": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "grease_injection": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "greater_shielding": {
       "classes": {
         "enchanter": "34",
         "magician": 34,
         "necromancer": 34,
         "wizard": 34
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "greater_wolf_form": {
       "classes": {
         "druid": 34,
         "ranger": 56
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "greenmist": {
       "classes": {},
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "grim_aura": {
       "classes": {
         "necromancer": 4,
         "shadow knight": 22
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "group_resist_magic": {
       "classes": {
         "enchanter": "49"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "guard": {
       "classes": {
         "cleric": 29,
         "paladin": 39
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "guardian": {
       "classes": {
         "shaman": 44
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "guardian_rhythms": {
       "classes": {
         "bard": 17
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "harmony": {
       "classes": {
         "druid": 5,
         "ranger": 22
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "harmshield": {
       "classes": {
         "necromancer": 20
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "harpy_voice": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "haste": {
       "classes": {},
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "haze": {
       "classes": {
         "enchanter": "4"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "health": {
       "classes": {
         "shaman": 34
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "heart_flutter": {
       "classes": {
         "necromancer": 16,
         "shadow knight": 39
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "heat_blood": {
       "classes": {
         "necromancer": 12,
         "shadow knight": 30
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "heat_sight": {
       "classes": {
         "wizard": 16
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "heroic_bond": {
       "classes": {
         "cleric": 52
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "heroism": {
       "classes": {
         "cleric": 52
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "holy_armor": {
       "classes": {
         "cleric": 5,
         "paladin": 15
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "hug": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "hymn_of_restoration": {
       "classes": {
         "bard": 6
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "ice": {
       "classes": {
         "druid": 49
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "ice_breath": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "ice_strike": {
       "classes": {
         "shaman": 54
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "ignite_blood": {
       "classes": {
         "necromancer": 49
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "ignite_bones": {
       "classes": {
         "necromancer": 44
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "ikatiars_revenge": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "immolate": {
       "classes": {
         "druid": 29,
         "ranger": 49
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "immolating_breath": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "impart_strength": {
       "classes": {
         "necromancer": 8
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "incapacitate": {
       "classes": {
         "enchanter": "44",
         "shaman": 44
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "infectious_cloud": {
       "classes": {
         "necromancer": 16,
         "shaman": 19
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "inferno_shield": {
       "classes": {
         "magician": 29
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "inner_fire": {
       "classes": {
         "shaman": 1
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "insidious_decay": {
       "classes": {
         "shaman": 52
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "insidious_fever": {
       "classes": {
         "shaman": 19
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "insidious_malady": {
       "classes": {
         "shaman": 39
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "insight": {
       "classes": {
         "enchanter": "255"
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "insipid_weakness": {
       "classes": {
         "enchanter": "34"
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "inspire_fear": {
       "classes": {
         "cleric": 24
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "intensify_death": {
       "classes": {
         "necromancer": 24
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "invigor": {
       "classes": {
         "cleric": 9,
         "druid": 14,
         "enchanter": "24",
         "paladin": 22,
         "ranger": 30,
         "shaman": 24
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "jonthans_inspiration": {
       "classes": {
         "bard": 58
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "jonthans_provocation": {
       "classes": {
         "bard": 45
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "jonthans_whistling_warsong": {
       "classes": {
         "bard": 7
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "kazumis_note_of_preservation": {
       "classes": {
         "bard": 60
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "kelins_lucid_lullaby": {
       "classes": {
         "bard": 15
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "kelins_lugubrious_lament": {
       "classes": {
         "bard": 8
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "kilvas_skin_of_flame": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "kylies_venom": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "languid_pace": {
       "classes": {
         "enchanter": "12"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "largarns_lamentation": {
       "classes": {
         "enchanter": "55"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "largos_absonant_binding": {
       "classes": {
         "bard": 51
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "largos_melodic_binding": {
       "classes": {
         "bard": 20
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "leach": {
       "classes": {
         "necromancer": 12
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "leatherskin": {
       "classes": {
         "necromancer": 24,
         "wizard": 24
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "legacy_of_spike": {
       "classes": {
         "druid": 51
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "legacy_of_thorn": {
       "classes": {
         "druid": 59
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "lesser_shielding": {
       "classes": {
         "enchanter": "8",
         "magician": 8,
         "necromancer": 8,
         "wizard": 8
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "levitate": {
       "classes": {
         "druid": 14,
         "enchanter": "16",
         "ranger": 39,
         "shaman": 14,
         "wizard": 24
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "levitation": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "lich": {
       "classes": {
         "necromancer": 49
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "listless_power": {
       "classes": {
         "enchanter": "29",
         "shaman": 29
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "lower_resists_i": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "lower_resists_ii": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "lower_resists_iii": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "lower_resists_iv": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "lull": {
       "classes": {
         "cleric": 1,
         "enchanter": "1",
         "paladin": 15
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "lull_animal": {
       "classes": {
         "druid": 1,
         "ranger": 9
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "lyssas_solidarity_of_vision": {
       "classes": {
         "bard": 34
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "lyssas_veracious_concord": {
       "classes": {
         "bard": 24
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "magi_curse": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "magnify": {
       "classes": {
         "wizard": 29
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "major_shielding": {
       "classes": {
         "enchanter": "24",
         "magician": 24,
         "necromancer": 24,
         "wizard": 24
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "mala": {
       "classes": {
         "magician": 60
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "malevolent_grasp": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "malo": {
       "classes": {
         "shaman": 60
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "malosi": {
       "classes": {
         "magician": 51,
         "shaman": 49
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "malosini": {
       "classes": {
         "magician": 58,
         "shaman": 57
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "mana_flare": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "mana_shroud": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "manasink": {
       "classes": {
         "wizard": 58
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "manaskin": {
       "classes": {
         "necromancer": 52,
         "wizard": 52
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "maniacal_strength": {
       "classes": {
         "shaman": 57
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "manticore_poison": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "mark_of_karn": {
       "classes": {
         "cleric": 56
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "mask_of_the_hunter": {
       "classes": {
         "druid": 60
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "mcvaxius_berserker_crescendo": {
       "classes": {
         "bard": 42
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "mcvaxius_rousing_rondo": {
       "classes": {
         "bard": 57
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "melody_of_ervaj": {
       "classes": {
         "bard": 50
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "mesmerization": {
       "classes": {
         "enchanter": "16"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "mesmerize": {
       "classes": {
         "enchanter": "4"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "mesmerizing_breath": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "mind_cloud": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "minion_of_hate": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "minor_shielding": {
       "classes": {
         "enchanter": "1",
         "magician": 1,
         "necromancer": 1,
         "wizard": 1
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "mist": {
       "classes": {
         "enchanter": "12"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "mortal_deftness": {
       "classes": {
         "shaman": 58
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "muscle_lock_i": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "muscle_lock_ii": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "muscle_lock_iii": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "muscle_lock_iv": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "mystic_precision": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "naltrons_mark": {
       "classes": {
         "cleric": 58
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "natures_melody": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "natureskin": {
       "classes": {
         "druid": 57
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "nillipus_march_of_the_wee": {
       "classes": {
         "bard": 52
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "nimble": {
       "classes": {
         "shaman": 34
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "nivs_harmonic": {
       "classes": {
         "bard": 58
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "nivs_melody_of_preservation": {
       "classes": {
         "bard": 47
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "null_aura": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "numb_the_dead": {
       "classes": {
         "necromancer": 4,
         "shadow knight": 15
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "obscure": {
       "classes": {
         "enchanter": "29"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "obsidian_shatter": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "occlusion_of_sound": {
       "classes": {
         "bard": 55
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "okeils_flickering_flame": {
       "classes": {
         "wizard": 34
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "okeils_radiation": {
       "classes": {
         "wizard": 4
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "one_hundred_blows": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "overwhelming_splendor": {
       "classes": {
         "enchanter": "56"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "pacify": {
       "classes": {
         "cleric": 39,
         "enchanter": "39",
         "paladin": 51
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "pack_chloroplast": {
       "classes": {
         "druid": 49
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "pack_regeneration": {
       "classes": {
         "druid": 39
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "pack_spirit": {
       "classes": {
         "druid": 39
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "pact_of_shadow": {
       "classes": {
         "necromancer": 44
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "panic": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "panic_animal": {
       "classes": {
         "druid": 1,
         "ranger": 22
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "panic_the_dead": {
       "classes": {
         "cleric": 29,
         "necromancer": 29,
         "shadow knight": 54
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "paralyzing_poison_i": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "paralyzing_poison_ii": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "paralyzing_poison_iii": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "phantom_armor": {
       "classes": {
         "magician": 52
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "phantom_chain": {
       "classes": {
         "magician": 29
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "phantom_leather": {
       "classes": {
         "magician": 16
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "phantom_plate": {
       "classes": {
         "magician": 44
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "plague": {
       "classes": {
         "necromancer": 52,
         "shaman": 49
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "plagueratdisease": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "plainsight": {
       "classes": {
         "wizard": 55
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "poison": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "poison_bolt": {
       "classes": {
         "necromancer": 4
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "poison_breath": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "power": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "pox_of_bertoxxulous": {
       "classes": {
         "shaman": 59
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "primal_avatar": {
       "classes": {
         "shaman": 60
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "primal_essence": {
       "classes": {},
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "prime_healers_blessing": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "protect": {
       "classes": {
         "shaman": 24
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "protection_of_the_glades": {
       "classes": {
         "druid": 60
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "psalm_of_cooling": {
       "classes": {
         "bard": 33
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "psalm_of_mystic_shielding": {
       "classes": {
         "bard": 41
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "psalm_of_purity": {
       "classes": {
         "bard": 37
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "psalm_of_vitality": {
       "classes": {
         "bard": 29
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "psalm_of_warmth": {
       "classes": {
         "bard": 25
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "purifying_rhythms": {
       "classes": {
         "bard": 13
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "putrefy_flesh": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "putrid_breath": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "pyrocruor": {
       "classes": {
         "necromancer": 58
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "quickness": {
       "classes": {
         "enchanter": "16",
         "shaman": 29
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "quivering_veil_of_xarn": {
       "classes": {
         "necromancer": 58
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "rabies": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "radiant_visage": {
       "classes": {
         "enchanter": "34"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "rage": {
       "classes": {
         "shaman": 49
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "rage_of_tallon": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "rage_of_vallon": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "rage_of_zek": {
       "classes": {},
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "rampage": {
       "classes": {
         "enchanter": "39"
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "rapture": {
       "classes": {
         "enchanter": "59"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "reckless_health": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "reckless_strength": {
       "classes": {
         "cleric": 5,
         "paladin": 22
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "regeneration": {
       "classes": {
         "druid": 34,
         "shaman": 24
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "regrowth": {
       "classes": {
         "druid": 54,
         "shaman": 52
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "regrowth_of_the_grove": {
       "classes": {
         "druid": 58
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "rejuvenation": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "repulse_animal": {
       "classes": {
         "druid": 51
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "resist_cold": {
       "classes": {
         "cleric": 39,
         "druid": 34,
         "necromancer": 24,
         "ranger": 55,
         "shadow knight": 39,
         "shaman": 24
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "resist_disease": {
       "classes": {
         "cleric": 39,
         "druid": 44,
         "necromancer": 34,
         "paladin": 51,
         "shaman": 34
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "resist_fire": {
       "classes": {
         "cleric": 34,
         "druid": 24,
         "ranger": 49,
         "shaman": 29
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "resist_magic": {
       "classes": {
         "cleric": 44,
         "druid": 49,
         "enchanter": "39",
         "paladin": 55,
         "shaman": 44
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "resist_poison": {
       "classes": {
         "cleric": 34,
         "druid": 44,
         "shaman": 39
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "resistance_to_magic": {
       "classes": {},
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "resistant_skin": {
       "classes": {
         "wizard": 12
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "resolution": {
       "classes": {
         "cleric": 44,
         "paladin": 60
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "rest_the_dead": {
       "classes": {
         "necromancer": 24,
         "shadow knight": 52
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "resurrection_effects": {
       "classes": {},
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "riotous_health": {
       "classes": {
         "shaman": 54
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "rising_dexterity": {
       "classes": {
         "shaman": 29
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "rodricks_gift": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "ros_fiery_sundering": {
       "classes": {
         "druid": 39
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "rotting_flesh": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "rubicite_aura": {
       "classes": {},
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "rune_i": {
       "classes": {
         "enchanter": "16"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "rune_ii": {
       "classes": {
         "enchanter": "24"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "rune_iii": {
       "classes": {
         "enchanter": "34"
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "rune_iv": {
       "classes": {
         "enchanter": "44"
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "rune_v": {
       "classes": {
         "enchanter": "52"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "savage_spirit": {
       "classes": {
         "druid": 44
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "scale_of_wolf": {
       "classes": {
         "druid": 24,
         "shaman": 24
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "scale_skin": {
       "classes": {
         "shaman": 5
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "scarab_storm": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "scent_of_darkness": {
       "classes": {
         "necromancer": 39
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "scent_of_dusk": {
       "classes": {
         "necromancer": 12
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "scent_of_shadow": {
       "classes": {
         "necromancer": 24
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "scent_of_terris": {
       "classes": {
         "necromancer": 52
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "scorching_skin": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "scourge": {
       "classes": {
         "necromancer": 39,
         "shaman": 34
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "screaming_mace": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "screaming_terror": {
       "classes": {
         "necromancer": 24
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "sear": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "sebilite_pox": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "see_invisible": {
       "classes": {
         "druid": 14,
         "enchanter": "8",
         "magician": 16,
         "ranger": 39,
         "wizard": 4
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "seething_fury": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "selos_accelerando": {
       "classes": {
         "bard": 4
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "selos_assonant_strane": {
       "classes": {
         "bard": 54
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "selos_chords_of_cessation": {
       "classes": {
         "bard": 48
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "selos_consonant_chain": {
       "classes": {
         "bard": 23
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "selos_song_of_travel": {
       "classes": {
         "bard": 51
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "serpent_sight": {
       "classes": {
         "enchanter": "12",
         "shaman": 9
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "shade": {
       "classes": {
         "enchanter": "39"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "shadow": {
       "classes": {
         "enchanter": "49"
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "shadow_compact": {
       "classes": {
         "necromancer": 20
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "shadow_sight": {
       "classes": {
         "necromancer": 24,
         "shadow knight": 49
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "shadow_vortex": {
       "classes": {
         "necromancer": 20,
         "shadow knight": 39
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "shadowbond": {
       "classes": {
         "necromancer": 54
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "shallow_breath": {
       "classes": {
         "enchanter": "1"
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "share_wolf_form": {
       "classes": {
         "druid": 39
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "shauris_sonorous_clouding": {
       "classes": {
         "bard": 19
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "shield_of_barbs": {
       "classes": {
         "druid": 19
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "shield_of_blades": {
       "classes": {
         "druid": 58
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "shield_of_brambles": {
       "classes": {
         "druid": 29,
         "ranger": 49
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "shield_of_fire": {
       "classes": {
         "magician": 8
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "shield_of_flame": {
       "classes": {
         "magician": 20
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "shield_of_lava": {
       "classes": {
         "magician": 49
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "shield_of_song": {
       "classes": {
         "bard": 49
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "shield_of_spikes": {
       "classes": {
         "druid": 39,
         "ranger": 58
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "shield_of_the_magi": {
       "classes": {
         "enchanter": "54",
         "magician": 54,
         "necromancer": 54,
         "wizard": 54
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "shield_of_thistles": {
       "classes": {
         "druid": 9,
         "ranger": 30
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "shield_of_words": {
       "classes": {
         "cleric": 49,
         "paladin": 60
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "shielding": {
       "classes": {
         "enchanter": "16",
         "magician": 16,
         "necromancer": 16,
         "wizard": 16
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "shieldskin": {
       "classes": {
         "necromancer": 16,
         "shadow knight": 34,
         "wizard": 16
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "shifting_shield": {
       "classes": {
         "shaman": 34
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "shifting_sight": {
       "classes": {
         "enchanter": "20",
         "wizard": 39
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "shiftless_deeds": {
       "classes": {
         "enchanter": "44"
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "shroud_of_death": {
       "classes": {
         "shadow knight": 55
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "shroud_of_hate": {
       "classes": {
         "shadow knight": 39
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "shroud_of_pain": {
       "classes": {
         "shadow knight": 50
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "shroud_of_the_spirits": {
       "classes": {
         "shaman": 54
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "shroud_of_undeath": {
       "classes": {
         "shadow knight": 55
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "sicken": {
       "classes": {
         "shaman": 5
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "sight": {
       "classes": {
         "wizard": 20
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "sight_graft": {
       "classes": {
         "necromancer": 12
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "silver_skin": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "siphon_strength": {
       "classes": {
         "necromancer": 1,
         "shadow knight": 9
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "siphon_strength_recourse": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "skin_like_diamond": {
       "classes": {
         "druid": 39,
         "ranger": 54
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "skin_like_nature": {
       "classes": {
         "druid": 49,
         "ranger": 59
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "skin_like_rock": {
       "classes": {
         "druid": 14,
         "ranger": 22
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "skin_like_steel": {
       "classes": {
         "druid": 24,
         "ranger": 39
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "skin_like_wood": {
       "classes": {
         "druid": 1,
         "ranger": 9
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "skin_of_the_shadow": {
       "classes": {
         "necromancer": 55
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "skunkspray": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "slime_mist": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "snare": {
       "classes": {
         "druid": 1,
         "ranger": 9
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "solons_bewitching_bravura": {
       "classes": {
         "bard": 39
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "solons_charismatic_concord": {
       "classes": {
         "bard": 59
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "solons_song_of_the_sirens": {
       "classes": {
         "bard": 27
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "song_of_midnight": {
       "classes": {
         "bard": 56
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "song_of_the_deep_seas": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "song_of_twilight": {
       "classes": {
         "bard": 53
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "soothe": {
       "classes": {
         "cleric": 9,
         "enchanter": "8",
         "paladin": 30
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "soul_bond": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "soul_consumption": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "soul_well": {
       "classes": {},
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "speed_of_the_shissar": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "spikecoat": {
       "classes": {
         "druid": 39,
         "ranger": 49
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "spin_the_bottle": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "spirit_armor": {
       "classes": {
         "cleric": 19,
         "necromancer": 16,
         "paladin": 30
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "spirit_of_bear": {
       "classes": {
         "shaman": 9
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "spirit_of_cat": {
       "classes": {
         "shaman": 19
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "spirit_of_cheetah": {
       "classes": {
         "druid": 24,
         "shaman": 24
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "spirit_of_monkey": {
       "classes": {
         "shaman": 24
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "spirit_of_oak": {
       "classes": {
         "druid": 59
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "spirit_of_ox": {
       "classes": {
         "shaman": 24
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "spirit_of_scale": {
       "classes": {
         "druid": 53,
         "shaman": 52
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "spirit_of_snake": {
       "classes": {
         "shaman": 14
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "spirit_of_wolf": {
       "classes": {
         "druid": 14,
         "ranger": 30,
         "shaman": 9
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "spirit_quickening": {
       "classes": {
         "shaman": 50
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "spirit_sight": {
       "classes": {
         "shaman": 9
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "spirit_strength": {
       "classes": {
         "shaman": 19
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "splurt": {
       "classes": {
         "necromancer": 51
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "spook_the_dead": {
       "classes": {
         "cleric": 1,
         "necromancer": 12,
         "paladin": 9,
         "shadow knight": 22
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "stability": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "stalking_probe": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "stalwart_regeneration": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "stamina": {
       "classes": {
         "shaman": 44
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "steal_strength": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "steam_overload": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "steelskin": {
       "classes": {
         "necromancer": 34,
         "shadow knight": 56,
         "wizard": 34
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "stinging_swarm": {
       "classes": {
         "druid": 14,
         "ranger": 30
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "storm_strength": {
       "classes": {
         "druid": 44,
         "ranger": 53
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "stream_of_acid": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "strength": {
       "classes": {
         "shaman": 49
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "strength_of_earth": {
       "classes": {
         "druid": 9,
         "ranger": 30
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "strength_of_nature": {
       "classes": {
         "ranger": 51
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "strength_of_stone": {
       "classes": {
         "druid": 34
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "strength_of_the_kunzar": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "strengthen": {
       "classes": {
         "enchanter": "1",
         "shaman": 1
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "strengthen_death": {
       "classes": {
         "shadow knight": 29
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "strike_of_thunder": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "strong_disease": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "strong_poison": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "suffocate": {
       "classes": {
         "enchanter": "29"
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "suffocating_sphere": {
       "classes": {
         "enchanter": "4"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "sunbeam": {
       "classes": {
         "druid": 24
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "sunskin": {
       "classes": {
         "cleric": 51
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "surge_of_enfeeblement": {
       "classes": {
         "necromancer": 34
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "swarm_of_retribution": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "swarming_pain": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "swift_like_the_wind": {
       "classes": {
         "enchanter": "49"
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "swift_spirit": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "sympathetic_aura": {
       "classes": {
         "enchanter": "20"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "tagars_insects": {
       "classes": {
         "shaman": 29
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "tainted_breath": {
       "classes": {
         "shaman": 9
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "talisman_of_altuna": {
       "classes": {
         "shaman": 44
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "talisman_of_jasinth": {
       "classes": {
         "shaman": 51
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "talisman_of_kragg": {
       "classes": {
         "shaman": 55
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "talisman_of_shadoo": {
       "classes": {
         "shaman": 53
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "talisman_of_the_brute": {
       "classes": {
         "shaman": 57
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "talisman_of_the_cat": {
       "classes": {
         "shaman": 57
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "talisman_of_the_raptor": {
       "classes": {
         "shaman": 59
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "talisman_of_the_rhino": {
       "classes": {
         "shaman": 58
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "talisman_of_the_serpent": {
       "classes": {
         "shaman": 58
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "talisman_of_tnarg": {
       "classes": {
         "shaman": 34
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "tarews_aquatic_ayre": {
       "classes": {
         "bard": 16
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "tashan": {
       "classes": {
         "enchanter": "4"
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "tashani": {
       "classes": {
         "enchanter": "20"
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "tashania": {
       "classes": {
         "enchanter": "44"
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "tashanian": {
       "classes": {
         "enchanter": "255"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "telescope": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "tepid_deeds": {
       "classes": {
         "enchanter": "24"
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "terrorize_animal": {
       "classes": {
         "druid": 19
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "the_unspoken_word": {
       "classes": {
         "cleric": 59
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "thistlecoat": {
       "classes": {
         "druid": 9,
         "ranger": 15
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "thorncoat": {
       "classes": {
         "druid": 49,
         "ranger": 60
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "thorny_shield": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "thrall_of_bones": {
       "classes": {
         "necromancer": 54
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "thunder_blast": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "tigirs_insects": {
       "classes": {
         "shaman": 58
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "torment": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "torment_of_argli": {
       "classes": {
         "enchanter": "56"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "torment_of_shadows": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "torpor": {
       "classes": {
         "shaman": 60
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "track_corpse": {
       "classes": {
         "necromancer": 20
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "travelerboots": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "treeform": {
       "classes": {
         "druid": 9
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "trepidation": {
       "classes": {
         "cleric": 57,
         "enchanter": "56",
         "necromancer": 56
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "tumultuous_strength": {
       "classes": {
         "shaman": 39
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "tunares_request": {
       "classes": {
         "druid": 55
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "turgurs_insects": {
       "classes": {
         "shaman": 51
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "turning_of_the_unnatural": {
       "classes": {
         "cleric": 255
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "tuyens_chant_of_flame": {
       "classes": {
         "bard": 38
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "tuyens_chant_of_frost": {
       "classes": {
         "bard": 46
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "ultravision": {
       "classes": {
         "enchanter": "29",
         "shaman": 29
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "umbra": {
       "classes": {
         "enchanter": "57"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "unfailing_reverence": {
       "classes": {
         "shaman": 59
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "valiant_companion": {
       "classes": {
         "magician": 59
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "valor": {
       "classes": {
         "cleric": 34,
         "paladin": 49
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "vampire_charm": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "velocity": {
       "classes": {
         "magician": 58
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "vengeance_of_the_glades": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "venom_of_the_snake": {
       "classes": {
         "necromancer": 34,
         "shaman": 39
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "vexing_mordinia": {
       "classes": {
         "necromancer": 57
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "vigor": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "vision": {
       "classes": {
         "shaman": 19
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "visions_of_grandeur": {
       "classes": {
         "enchanter": "60"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "voice_graft": {
       "classes": {
         "necromancer": 16
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "voice_of_the_berserker": {
       "classes": {
         "shaman": 59
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "wake_of_tranquility": {
       "classes": {
         "cleric": 55,
         "enchanter": "51"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "walking_sleep": {
       "classes": {
         "shaman": 14
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "wandering_mind": {
       "classes": {
         "enchanter": "39"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "wave_of_enfeeblement": {
       "classes": {
         "necromancer": 12,
         "shadow knight": 30
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "wave_of_fear": {
       "classes": {
         "cleric": 24
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "wave_of_heat": {
       "classes": {},
-      "npc": "true",
-      "item": "false"
+      "npc": true,
+      "item": false
     },
     "waves_of_the_deep_sea": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "weak_poison": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "weaken": {
       "classes": {
         "enchanter": "1"
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "weakness": {
       "classes": {
         "enchanter": "44"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "whirl_till_you_hurl": {
       "classes": {
         "enchanter": "12"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "whirlwind": {
       "classes": {},
-      "npc": "true",
-      "item": "true"
+      "npc": true,
+      "item": true
     },
     "wind_of_tishani": {
       "classes": {
         "enchanter": "55"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "wind_of_tishanian": {
       "classes": {
         "enchanter": "60"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "winged_death": {
       "classes": {
         "druid": 53
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "wolf_form": {
       "classes": {
         "druid": 24,
         "ranger": 49
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "wonderous_rapidity": {
       "classes": {
         "enchanter": "58"
       },
-      "npc": "false",
-      "item": "false"
+      "npc": false,
+      "item": false
     },
     "wrath_of_nature": {
       "classes": {},
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "yaulp": {
       "classes": {
         "cleric": 1,
         "paladin": 9
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "yaulp_ii": {
       "classes": {
         "cleric": 19,
         "paladin": 39
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "yaulp_iii": {
       "classes": {
         "cleric": 44,
         "paladin": 56
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     },
     "yaulp_iv": {
       "classes": {
         "cleric": 53,
         "paladin": 60
       },
-      "npc": "false",
-      "item": "true"
+      "npc": false,
+      "item": true
     }
   },
   "version": "%s"
 }
 """
 
     try:
-        version = str(pkg_resources.get_distribution("eqalert").version)
         spell_casters_path = data_path + "spell-casters.json"
         generate = True
 
         if os.path.isfile(spell_casters_path):
             json_data = open(spell_casters_path, "r", encoding="utf-8")
             spell_casters = json.load(json_data)
             json_data.close()
 
             if spell_casters["version"] == version:
                 generate = False
 
         if generate:
+            print("    - generating spell-casters.json")
             f = open(spell_casters_path, "w", encoding="utf-8")
             f.write(new_spell_caster_data % (version))
             f.close()
 
     except Exception as e:
         eqa_settings.log(
             "update spell casters: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
             + ": "
             + str(e)
         )
 
 
-def update_spell_lines(data_path):
+def update_spell_lines(data_path, version):
     """Update data/spell-lines.json"""
 
     new_spell_lines_data = """
 {
   "spell_lines": {
     "spell_line_potion_you_on": {
       "accuracy": {},
@@ -6407,27 +6510,27 @@
     }
   },
   "version": "%s"
 }
 """
 
     try:
-        version = str(pkg_resources.get_distribution("eqalert").version)
         spell_lines_path = data_path + "spell-lines.json"
         generate = True
 
         if os.path.isfile(spell_lines_path):
             json_data = open(spell_lines_path, "r", encoding="utf-8")
             spell_lines = json.load(json_data)
             json_data.close()
 
             if spell_lines["version"] == version:
                 generate = False
 
         if generate:
+            print("    - generating spell-lines.json")
             f = open(spell_lines_path, "w", encoding="utf-8")
             f.write(new_spell_lines_data % (version))
             f.close()
 
     except Exception as e:
         eqa_settings.log(
             "update spell lines: Error on line "
@@ -7984,15 +8087,15 @@
                 spells_timer_hash = file_hash.hexdigest()
                 if spells_timer_hash == "5f6460b226f5f765de13f3f758fff4d9":
                     generate_spell_timer_file = True
                 else:
                     generate_spell_timer_file = False
 
             if generate_spell_timer_file:
-                print("Generating new spell-timers.json. This may take a minute . . .")
+                print("    - generating spell-timers.json (this may take a minute)")
                 # Bootstrap new spell-timers.json
                 spell_timer_json = {"spells": {}, "hash": spells_hash}
 
                 # Read spells_us.txt line
                 for line in eq_spells_file_lines:
                     modified_line = line.split("^")
 
@@ -8074,101 +8177,101 @@
     """Save state to config"""
 
     try:
         configs.settings.config["last_state"].update(
             {
                 "server": str(state.server),
                 "character": str(state.char),
-                "afk": str(state.afk),
-                "group": str(state.group),
-                "leader": str(state.leader),
-                "raid": str(state.raid),
+                "afk": state.afk,
+                "group": state.group,
+                "leader": state.leader,
+                "raid": state.raid,
             }
         )
         configs.settings.config["settings"]["encounter_parsing"].update(
-            {"auto_save": str(state.save_parse), "enabled": str(state.encounter_parse)}
+            {"auto_save": state.save_parse, "enabled": state.encounter_parse}
         )
         configs.settings.config["settings"]["raid_mode"].update(
             {
-                "auto_set": str(state.auto_raid),
+                "auto_set": state.auto_raid,
             }
         )
-        configs.settings.config["settings"]["timers"].update(
+        configs.settings.config["settings"]["timers"]["mob"].update(
             {
-                "auto_mob_timer": str(state.auto_mob_timer),
+                "auto": state.auto_mob_timer,
             }
         )
-        configs.settings.config["settings"]["timers"].update(
+        configs.settings.config["settings"]["timers"]["mob"].update(
             {
-                "auto_mob_timer_delay": str(state.auto_mob_timer_delay),
+                "auto_delay": state.auto_mob_timer_delay,
             }
         )
-        configs.settings.config["settings"]["timers"].update(
+        configs.settings.config["settings"]["timers"]["spell"].update(
             {
-                "spell_timer_delay": str(state.spell_timer_delay),
+                "delay": state.spell_timer_delay,
             }
         )
-        configs.settings.config["settings"]["timers"].update(
+        configs.settings.config["settings"]["timers"]["spell"].update(
             {
-                "spell_timer_guess": str(state.spell_timer_guess),
+                "guess": state.spell_timer_guess,
             }
         )
-        configs.settings.config["settings"]["timers"].update(
+        configs.settings.config["settings"]["timers"]["spell"].update(
             {
-                "spell_timer_guild_only": str(state.spell_timer_guild_only),
+                "guild_only": state.spell_timer_guild_only,
             }
         )
-        configs.settings.config["settings"]["timers"].update(
+        configs.settings.config["settings"]["timers"]["spell"].update(
             {
-                "spell_timer_yours_only": str(state.spell_timer_yours_only),
+                "yours_only": state.spell_timer_yours_only,
             }
         )
-        configs.settings.config["settings"]["timers"].update(
+        configs.settings.config["settings"]["timers"]["spell"].update(
             {
-                "spell_timer_other": str(state.spell_timer_other),
+                "other": str(state.spell_timer_other),
             }
         )
-        configs.settings.config["settings"]["timers"].update(
+        configs.settings.config["settings"]["timers"]["spell"].update(
             {
-                "spell_timer_self": str(state.spell_timer_self),
+                "self": state.spell_timer_self,
             }
         )
         configs.settings.config["settings"]["consider_eval"].update(
-            {"enabled": str(state.consider_eval)}
+            {"enabled": state.consider_eval}
         )
         configs.settings.config["settings"]["debug_mode"].update(
-            {"enabled": str(state.debug)}
+            {"enabled": state.debug}
         )
         configs.settings.config["settings"]["detect_character"].update(
-            {"enabled": str(state.detect_char)}
+            {"enabled": state.detect_char}
         )
-        configs.settings.config["settings"]["mute"].update({"enabled": str(state.mute)})
+        configs.settings.config["settings"]["mute"].update({"enabled": state.mute})
         configs.characters.config["char_logs"][state.char + "_" + state.server].update(
             {
                 "char": str(state.char),
-                "disabled": "false",
+                "disabled": False,
                 "file_name": "eqlog_"
                 + str(state.char)
                 + "_"
                 + str(state.server)
                 + ".txt",
                 "server": str(state.server),
                 "char_state": {
-                    "direction": str(state.direction),
+                    "direction": state.direction,
                     "location": {
-                        "x": str(state.loc[1]),
-                        "y": str(state.loc[0]),
-                        "z": str(state.loc[2]),
+                        "x": state.loc[1],
+                        "y": state.loc[0],
+                        "z": state.loc[2],
                     },
-                    "zone": str(state.zone),
-                    "encumbered": str(state.encumbered),
-                    "bind": str(state.bind),
-                    "level": str(state.char_level),
-                    "class": str(state.char_class),
-                    "guild": str(state.char_guild),
+                    "zone": state.zone,
+                    "encumbered": state.encumbered,
+                    "bind": state.bind,
+                    "level": state.char_level,
+                    "class": state.char_class,
+                    "guild": state.char_guild,
                 },
             }
         )
         json_data = open(configs.settings.path, "w", encoding="utf-8")
         json.dump(
             configs.settings.config,
             json_data,
@@ -8253,35 +8356,35 @@
         debug = configs.settings.config["settings"]["debug_mode"]["enabled"]
         detect_char = configs.settings.config["settings"]["detect_character"]["enabled"]
         mute = configs.settings.config["settings"]["mute"]["enabled"]
         save_parse = configs.settings.config["settings"]["encounter_parsing"][
             "auto_save"
         ]
         auto_raid = configs.settings.config["settings"]["raid_mode"]["auto_set"]
-        auto_mob_timer = configs.settings.config["settings"]["timers"]["auto_mob_timer"]
-        auto_mob_timer_delay = configs.settings.config["settings"]["timers"][
-            "auto_mob_timer_delay"
+        auto_mob_timer = configs.settings.config["settings"]["timers"]["mob"]["auto"]
+        auto_mob_timer_delay = configs.settings.config["settings"]["timers"]["mob"][
+            "auto_delay"
         ]
-        spell_timer_delay = configs.settings.config["settings"]["timers"][
-            "spell_timer_delay"
+        spell_timer_delay = configs.settings.config["settings"]["timers"]["spell"][
+            "delay"
         ]
-        spell_timer_guess = configs.settings.config["settings"]["timers"][
-            "spell_timer_guess"
+        spell_timer_guess = configs.settings.config["settings"]["timers"]["spell"][
+            "guess"
         ]
-        spell_timer_other = configs.settings.config["settings"]["timers"][
-            "spell_timer_other"
+        spell_timer_other = configs.settings.config["settings"]["timers"]["spell"][
+            "other"
         ]
-        spell_timer_guild_only = configs.settings.config["settings"]["timers"][
-            "spell_timer_guild_only"
+        spell_timer_guild_only = configs.settings.config["settings"]["timers"]["spell"][
+            "guild_only"
         ]
-        spell_timer_yours_only = configs.settings.config["settings"]["timers"][
-            "spell_timer_yours_only"
+        spell_timer_yours_only = configs.settings.config["settings"]["timers"]["spell"][
+            "yours_only"
         ]
-        spell_timer_self = configs.settings.config["settings"]["timers"][
-            "spell_timer_self"
+        spell_timer_self = configs.settings.config["settings"]["timers"]["spell"][
+            "self"
         ]
         mute = configs.settings.config["settings"]["mute"]["enabled"]
 
         # Get chars
         chars = get_config_chars(configs)
 
         # Populate and return a new state
@@ -8335,15 +8438,15 @@
     try:
         json_data = open(
             base_path + "config/line-alerts/other.json", "r", encoding="utf-8"
         )
         data = json.load(json_data)
         json_data.close()
         data["line"].update(
-            {line_type: {"sound": "false", "reaction": "false", "alert": {}}}
+            {line_type: {"sound": False, "reaction": False, "alert": {}}}
         )
         json_data = open(
             base_path + "config/line-alerts/other.json", "w", encoding="utf-8"
         )
         json.dump(data, json_data, sort_keys=True, indent=2)
         json_data.close()
 
@@ -8359,15 +8462,17 @@
 def add_zone(zone, base_path):
     """Adds default setting values for new zones"""
 
     try:
         json_data = open(base_path + "config/zones.json", "r", encoding="utf-8")
         data = json.load(json_data)
         json_data.close()
-        data["zones"].update({str(zone): {"raid_mode": "false", "timer": "0"}})
+        data["zones"].update(
+            {str(zone): {"indoors": False, "raid_mode": False, "timer": 0}}
+        )
         json_data = open(base_path + "config/zones.json", "w", encoding="utf-8")
         json.dump(data, json_data, sort_keys=True, indent=2)
         json_data.close()
 
     except Exception as e:
         eqa_settings.log(
             "add zone: Error on line "
@@ -8422,523 +8527,691 @@
             "update players file: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
             + ": "
             + str(e)
         )
 
 
-def generate_players_file(player_data_file):
+def generate_players_file(player_data_file, version):
     """Bootstrap Player Data File"""
 
     new_players_data = """
 {
   "server": {
     "P1999Green": {
       "players": {}
     },
     "project1999": {
       "players": {}
     }
-  }
+  },
+  "version": "%s"
 }
 """
 
     try:
+        print("    - generating players.json")
         f = open(player_data_file, "w", encoding="utf-8")
-        f.write(new_players_data)
+        f.write(new_players_data % (version))
         f.close()
 
     except Exception as e:
         eqa_settings.log(
             "generate players file: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
             + ": "
             + str(e)
         )
 
 
-def build_config(base_path):
+def validate_players_file(player_data_file, version):
+    """Validate Player Data File"""
+
+    try:
+        json_data = open(player_data_file, "r", encoding="utf-8")
+        player_json_data = json.load(json_data)
+        json_data.close()
+
+        if "version" in player_json_data.keys():
+            # For any future needed changes
+            pass
+        else:
+            # no version
+            updated_player_list = {"server": {}, "version": version}
+            for server in player_json_data["server"].keys():
+                updated_player_list["server"][server] = {"players": {}}
+                for player in player_json_data["server"][server]["players"].keys():
+                    if (
+                        player_json_data["server"][server]["players"][player]["guild"]
+                        != "none"
+                    ):
+                        char_guild = player_json_data["server"][server]["players"][
+                            player
+                        ]["guild"]
+                    else:
+                        char_guild = None
+                    if (
+                        player_json_data["server"][server]["players"][player]["class"]
+                        != "unknown"
+                    ):
+                        char_class = player_json_data["server"][server]["players"][
+                            player
+                        ]["class"]
+                    else:
+                        char_class = None
+                    char_level = int(
+                        player_json_data["server"][server]["players"][player]["level"]
+                    )
+
+                    updated_player_list["server"][server]["players"][player] = {
+                        "class": char_class,
+                        "guild": char_guild,
+                        "level": char_level,
+                    }
+
+            json_data = open(player_data_file, "w", encoding="utf-8")
+            json.dump(updated_player_list, json_data, sort_keys=True, indent=2)
+            json_data.close()
+
+    except Exception as e:
+        eqa_settings.log(
+            "validate players file: Error on line "
+            + str(sys.exc_info()[-1].tb_lineno)
+            + ": "
+            + str(e)
+        )
+
+
+def build_config(base_path, version):
     """Build a default config"""
 
     new_char_config = """
 {
-  "char_logs": {}
+  "char_logs": {},
+  "version": "%s"
 }
 """
 
     new_settings_config = """
 {
   "last_state": {},
   "settings": {
     "consider_eval": {
-      "enabled": "false"
+      "enabled": true
     },
     "debug_mode": {
-      "enabled": "false"
+      "enabled": false
     },
     "detect_character": {
-      "enabled": "true"
+      "enabled": true
     },
     "encounter_parsing": {
-      "auto_save": "false",
-      "enabled": "true"
+      "auto_save": false,
+      "enabled": true
     },
     "mute": {
-      "enabled": "false"
+      "enabled": false
     },
     "paths": {
       "eqalert_log": "%slog/",
       "data": "%sdata/",
       "encounter": "%sencounters/",
       "everquest_logs": "%s/.wine/drive_c/Program Files/Sony/EverQuest/Logs/",
       "everquest_files": "%s/.wine/drive_c/Program Files/Sony/EverQuest/",
       "sound": "%ssound/",
       "tmp_sound": "/tmp/eqa/sound/"
     },
     "player_data": {
-      "persist": "true"
+      "persist": true
     },
     "raid_mode": {
-      "auto_set": "true"
+      "auto_set": true
     },
     "speech": {
-      "expand_lingo": "true",
+      "expand_lingo": true,
       "tld": "com",
       "lang": "en"
     },
     "timers": {
-      "auto_mob_timer": "false",
-      "auto_mob_timer_delay": "10",
-      "spell_timer_delay": "24",
-      "spell_timer_guess": "true",
-      "spell_timer_other": "true",
-      "spell_timer_guild_only": "false",
-      "spell_timer_yours_only": "true",
-      "spell_timer_self": "true",
-      "spell_timer_zone_drift": "true"
+      "mob": {
+        "auto": false,
+        "auto_delay": 10
+      },
+      "spell": {
+        "delay": 24,
+        "guess": true,
+        "other": true,
+        "guild_only": false,
+        "yours_only": true,
+        "self": true,
+        "zone_drift": true
+      }
     }
   },
   "version": "%s"
 }
 """
 
     new_zones_config = """
 {
   "zones": {
     "An Arena (PVP) Area": {
-      "raid_mode": "false",
-      "timer": "0"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 0
     },
     "Befallen": {
-      "raid_mode": "false",
-      "timer": "1140"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 1120
     },
     "Blackburrow": {
-      "raid_mode": "false",
-      "timer": "1320"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 1320
     },
     "Butcherblock Mountains": {
-      "raid_mode": "false",
-      "timer": "600"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 900
     },
     "Castle Mistmoore": {
-      "raid_mode": "false",
-      "timer": "1320"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 1320
     },
     "Chardok": {
-      "raid_mode": "false",
-      "timer": "1200"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 1080
     },
     "City of Thurgadin": {
-      "raid_mode": "false",
-      "timer": "420"
+      "indoors": true,
+      "raid_mode": false,
+      "timer": 420
     },
     "Cobalt Scar": {
-      "raid_mode": "false",
-      "timer": "1200"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 1200
     },
     "Crushbone": {
-      "raid_mode": "false",
-      "timer": "540"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 540
     },
     "Crystal Caverns": {
-      "raid_mode": "false",
-      "timer": "885"
+      "indoors": true,
+      "raid_mode": false,
+      "timer": 885
     },
     "Dagnor's Cauldron": {
-      "raid_mode": "false",
-      "timer": "0"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 0
     },
     "Dalnir": {
-      "raid_mode": "false",
-      "timer": "720"
+      "indoors": true,
+      "raid_mode": false,
+      "timer": 720
     },
     "Dragon Necropolis": {
-      "raid_mode": "false",
-      "timer": "1620"
+      "indoors": true,
+      "raid_mode": false,
+      "timer": 1620
     },
     "Dreadlands": {
-      "raid_mode": "false",
-      "timer": "400"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 400
     },
     "East Commonlands": {
-      "raid_mode": "false",
-      "timer": "400"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 400
     },
     "East Freeport": {
-      "raid_mode": "false",
-      "timer": "1440"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 1440
     },
     "Eastern Plains of Karana": {
-      "raid_mode": "false",
-      "timer": "400"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 400
     },
     "Eastern Wastelands": {
-      "raid_mode": "false",
-      "timer": "400"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 400
     },
     "Erudin": {
-      "raid_mode": "false",
-      "timer": "400"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 400
     },
     "Erudin Palace": {
-      "raid_mode": "false",
-      "timer": "1500"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 1500
     },
     "Estate of Unrest": {
-      "raid_mode": "false",
-      "timer": "1320"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 1320
     },
     "Everfrost": {
-      "raid_mode": "false",
-      "timer": "400"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 400
     },
     "Field of Bone": {
-      "raid_mode": "false",
-      "timer": "400"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 400
     },
     "Firiona Vie": {
-      "raid_mode": "false",
-      "timer": "400"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 400
     },
     "Frontier Mountains": {
-      "raid_mode": "false",
-      "timer": "400"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 400
     },
     "Gorge of King Xorbb": {
-      "raid_mode": "false",
-      "timer": "360"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 360
     },
     "Great Divide": {
-      "raid_mode": "false",
-      "timer": "640"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 640
     },
     "Greater Faydark": {
-      "raid_mode": "false",
-      "timer": "425"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 425
     },
     "Guk": {
-      "raid_mode": "false",
-      "timer": "990"
+      "indoors": true,
+      "raid_mode": false,
+      "timer": 990
     },
     "High Keep": {
-      "raid_mode": "false",
-      "timer": "600"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 600
     },
     "Highpass Hold": {
-      "raid_mode": "false",
-      "timer": "300"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 300
     },
     "Howling Stones": {
-      "raid_mode": "false",
-      "timer": "1230"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 1230
     },
     "Iceclad Ocean": {
-      "raid_mode": "false",
-      "timer": "400"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 400
     },
     "Icewell Keep": {
-      "raid_mode": "true",
-      "timer": "1260"
+      "indoors": true,
+      "raid_mode": true,
+      "timer": 1260
     },
     "Infected Paw": {
-      "raid_mode": "false",
-      "timer": "1320"
+      "indoors": true,
+      "raid_mode": false,
+      "timer": 1320
     },
     "Innothule Swamp": {
-      "raid_mode": "false",
-      "timer": "400"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 400
     },
     "Kael Drakkel": {
-      "raid_mode": "true",
-      "timer": "1680"
+      "indoors": true,
+      "raid_mode": true,
+      "timer": 1680
     },
     "Kaesora": {
-      "raid_mode": "false",
-      "timer": "1080"
+      "indoors": true,
+      "raid_mode": false,
+      "timer": 1080
     },
     "Karnor's Castle": {
-      "raid_mode": "false",
-      "timer": "1620"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 1620
     },
     "Kedge Keep": {
-      "raid_mode": "false",
-      "timer": "1320"
+      "indoors": true,
+      "raid_mode": false,
+      "timer": 1320
     },
     "Kithicor Woods": {
-      "raid_mode": "false",
-      "timer": "400"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 400
     },
     "Kurn's Tower": {
-      "raid_mode": "false",
-      "timer": "1100"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 1100
     },
     "Lake Rathetear": {
-      "raid_mode": "false",
-      "timer": "400"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 400
     },
     "Lake of Ill Omen": {
-      "raid_mode": "false",
-      "timer": "400"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 400
     },
     "Lavastorm Mountains": {
-      "raid_mode": "false",
-      "timer": "400"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 400
     },
     "Lesser Faydark": {
-      "raid_mode": "false",
-      "timer": "390"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 390
     },
     "Lost Temple of Cazic-Thule": {
-      "raid_mode": "false",
-      "timer": "1320"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 1320
     },
     "Mines of Nurga": {
-      "raid_mode": "false",
-      "timer": "1230"
+      "indoors": true,
+      "raid_mode": false,
+      "timer": 1230
     },
     "Misty Thicket": {
-      "raid_mode": "false",
-      "timer": "400"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 400
     },
     "Nagafen's Lair": {
-      "raid_mode": "false",
-      "timer": "1320"
+      "indoors": true,
+      "raid_mode": false,
+      "timer": 1320
     },
     "Najena": {
-      "raid_mode": "false",
-      "timer": "1110"
+      "indoors": true,
+      "raid_mode": false,
+      "timer": 1110
     },
     "North Freeport": {
-      "raid_mode": "false",
-      "timer": "1440"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 1440
     },
     "Northern Desert of Ro": {
-      "raid_mode": "false",
-      "timer": "400"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 400
     },
     "Northern Felwithe": {
-      "raid_mode": "false",
-      "timer": "1440"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 1440
     },
     "Northern Plains of Karana": {
-      "raid_mode": "false",
-      "timer": "400"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 400
     },
     "Oasis of Marr": {
-      "raid_mode": "false",
-      "timer": "990"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 990
     },
     "Ocean of Tears": {
-      "raid_mode": "false",
-      "timer": "360"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 360
     },
     "Old Sebilis": {
-      "raid_mode": "false",
-      "timer": "1620"
+      "indoors": true,
+      "raid_mode": false,
+      "timer": 1620
     },
     "Paineel": {
-      "raid_mode": "false",
-      "timer": "630"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 630
     },
     "Permafrost Caverns": {
-      "raid_mode": "false",
-      "timer": "1320"
+      "indoors": true,
+      "raid_mode": false,
+      "timer": 1320
     },
     "Plane of Air": {
-      "raid_mode": "true",
-      "timer": "28800"
+      "indoors": false,
+      "raid_mode": true,
+      "timer": 28800
     },
     "Plane of Fear": {
-      "raid_mode": "true",
-      "timer": "28800"
+      "indoors": false,
+      "raid_mode": true,
+      "timer": 28800
     },
     "Plane of Growth": {
-      "raid_mode": "true",
-      "timer": "43200"
+      "indoors": false,
+      "raid_mode": true,
+      "timer": 43200
     },
     "Plane of Hate": {
-      "raid_mode": "true",
-      "timer": "28800"
+      "indoors": false,
+      "raid_mode": true,
+      "timer": 28800
     },
     "Plane of Mischief": {
-      "raid_mode": "false",
-      "timer": "4210"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 4210
     },
     "Qeynos Hills": {
-      "raid_mode": "false",
-      "timer": "400"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 400
     },
     "Rathe Mountains": {
-      "raid_mode": "false",
-      "timer": "400"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 400
     },
     "Rivervale": {
-      "raid_mode": "false",
-      "timer": "1320"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 1320
     },
     "Ruins of Old Guk": {
-      "raid_mode": "false",
-      "timer": "1680"
+      "indoors": true,
+      "raid_mode": false,
+      "timer": 1680
     },
     "Sirens Grotto": {
-      "raid_mode": "false",
-      "timer": "1680"
+      "indoors": true,
+      "raid_mode": false,
+      "timer": 1680
     },
     "Skyfire Mountains": {
-      "raid_mode": "false",
-      "timer": "780"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 780
     },
     "Skyshrine": {
-      "raid_mode": "true",
-      "timer": "1800"
+      "indoors": false,
+      "raid_mode": true,
+      "timer": 1800
     },
     "Sleepers Tomb": {
-      "raid_mode": "true",
-      "timer": "28800"
+      "indoors": false,
+      "raid_mode": true,
+      "timer": 28800
     },
     "South Kaladim": {
-      "raid_mode": "false",
-      "timer": "400"
+      "indoors": true,
+      "raid_mode": false,
+      "timer": 400
     },
     "Southern Desert of Ro": {
-      "raid_mode": "false",
-      "timer": "400"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 400
     },
     "Southern Felwithe": {
-      "raid_mode": "false",
-      "timer": "1440"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 1440
     },
     "Southern Plains of Karana": {
-      "raid_mode": "false",
-      "timer": "400"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 400
     },
     "Steamfont Mountains": {
-      "raid_mode": "false",
-      "timer": "400"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 400
     },
     "Surefall Glade": {
-      "raid_mode": "false",
-      "timer": "0"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 0
     },
     "Temple of Droga": {
-      "raid_mode": "false",
-      "timer": "1230"
+      "indoors": true,
+      "raid_mode": false,
+      "timer": 1230
     },
     "Temple of Solusek Ro": {
-      "raid_mode": "false",
-      "timer": "0"
+      "indoors": true,
+      "raid_mode": false,
+      "timer": 0
     },
     "Temple of Veeshan": {
-      "raid_mode": "true",
-      "timer": "4398"
+      "indoors": true,
+      "raid_mode": true,
+      "timer": 4398
     },
     "The Arena": {
-      "raid_mode": "false",
-      "timer": "0"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 0
     },
     "The Burning Wood": {
-      "raid_mode": "false",
-      "timer": "400"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 400
     },
     "The City of Mist": {
-      "raid_mode": "false",
-      "timer": "1320"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 1320
     },
     "The Emerald Jungle": {
-      "raid_mode": "false",
-      "timer": "0"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 0
     },
     "The Feerrott": {
-      "raid_mode": "false",
-      "timer": "400"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 400
     },
     "The Hole": {
-      "raid_mode": "false",
-      "timer": "1290"
+      "indoors": true,
+      "raid_mode": false,
+      "timer": 1290
     },
     "The Nektulos Forest": {
-      "raid_mode": "false",
-      "timer": "400"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 400
     },
     "The Overthere": {
-      "raid_mode": "false",
-      "timer": "400"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 400
     },
     "The Wakening Lands": {
-      "raid_mode": "false",
-      "timer": "400"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 400
     },
     "Tower of Frozen Shadow": {
-      "raid_mode": "false",
-      "timer": "1200"
+      "indoors": true,
+      "raid_mode": false,
+      "timer": 1200
     },
     "Timorous Deep": {
-      "raid_mode": "false",
-      "timer": "720"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 720
     },
     "Toxxulia Forest": {
-      "raid_mode": "false",
-      "timer": "400"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 400
     },
     "Trakanon's Teeth": {
-      "raid_mode": "false",
-      "timer": "400"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 400
     },
     "Veeshan's Peak": {
-      "raid_mode": "true",
-      "timer": "0"
+      "indoors": false,
+      "raid_mode": true,
+      "timer": 0
     },
     "Velketor's Labyrinth": {
-      "raid_mode": "false",
-      "timer": "1972"
+      "indoors": true,
+      "raid_mode": false,
+      "timer": 1972
     },
     "Warrens": {
-      "raid_mode": "false",
-      "timer": "400"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 400
     },
     "West Commonlands": {
-      "raid_mode": "false",
-      "timer": "400"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 400
     },
     "West Freeport": {
-      "raid_mode": "false",
-      "timer": "1440"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 1440
     },
     "Western Plains of Karana": {
-      "raid_mode": "false",
-      "timer": "1320"
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 1320
     },
     "Western Wastes": {
-      "raid_mode": "true",
-      "timer": "0"
-    },
-    "unavailable": {
-      "raid_mode": "false",
-      "timer": "0"
+      "indoors": false,
+      "raid_mode": true,
+      "timer": 0
+    },
+    "Unavailable": {
+      "indoors": false,
+      "raid_mode": false,
+      "timer": 0
     }
   },
   "version": "%s"
 }
 """
 
     new_line_combat_config = """
@@ -8947,81 +9220,81 @@
     "combat_no_target": {
       "alert": {},
       "reaction": "solo",
       "sound": "no target"
     },
     "combat_other_ds_fire_damage": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "combat_other_ds_thorns_damage": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "combat_other_flurry": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "combat_other_melee": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "combat_other_melee_block": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "combat_other_melee_crip_blow": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "combat_other_melee_crit": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "combat_other_melee_crit_kick": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "combat_other_melee_dodge": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "combat_other_melee_invulnerable": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "combat_other_melee_miss": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "combat_other_melee_parry": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "combat_other_melee_riposte": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "combat_other_rune_damage": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "combat_ranger_drake": {
       "alert": {},
       "reaction": "solo",
       "sound": "ranger drake"
     },
     "combat_you_cannot_hit": {
@@ -9032,101 +9305,101 @@
     "combat_you_cannot_see": {
       "alert": {},
       "reaction": "solo",
       "sound": "can't see"
     },
     "combat_you_ds_fire_damage": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "combat_you_ds_thorns_damage": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "combat_you_melee": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "combat_you_melee_dodge": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "combat_you_melee_dodge": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "combat_you_melee_invulnerable": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "combat_your_melee_invulnerable": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "combat_you_melee_parry": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "combat_you_melee_riposte": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "combat_you_melee_miss": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "combat_you_receive_melee": {
       "alert": {},
       "reaction": "afk",
       "sound": "danger will robinson"
     },
     "combat_you_rune_damage": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "combat_your_rune_damage": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "experience_group": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "experience_lost": {
       "alert": {},
       "reaction": "all",
       "sound": "oh no!"
     },
     "experience_solo": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "experience_solo_resurrection": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "mob_enrage_off": {
       "alert": {},
       "reaction": "group",
-      "sound": "true"
+      "sound": true
     },
     "mob_enrage_on": {
       "alert": {},
       "reaction": "group",
       "sound": "enrage"
     },
     "mob_out_of_range": {
@@ -9138,108 +9411,108 @@
       "alert": {},
       "reaction": "group",
       "sound": "rampage"
     },
     "mob_slain_other": {
       "alert": {},
       "reaction": "solo_group_only",
-      "sound": "true"
+      "sound": true
     },
     "mob_slain_you": {
       "alert": {},
       "reaction": "solo_group_only",
-      "sound": "true"
+      "sound": true
     },
     "unconscious": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "you_slain": {
       "alert": {},
       "reaction": "solo_only",
-      "sound": "true"
+      "sound": true
     }
   },
   "version": "%s"
 }
 """
 
     new_line_spell_general_config = """
 {
   "line": {
     "songs_interrupted_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spells_bind_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spells_cast_item_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spells_cast_oom": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spells_cast_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spells_cast_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spells_cooldown_active": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spells_cured_other": {
       "alert": {},
       "reaction": "solo",
       "sound": "cured"
     },
     "spells_damage_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spells_damage_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spells_distracted": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spells_fizzle_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spells_fizzle_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spells_forget": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spells_gate_collapse": {
       "alert": {},
       "reaction": "solo",
       "sound": "gate collapse"
     },
     "spells_gate_npc_casting": {
@@ -9250,41 +9523,41 @@
     "spells_gated_npc": {
       "alert": {},
       "reaction": "solo",
       "sound": "mob gated"
     },
     "spells_heal_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spells_heal_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spells_illusion_dropping_you": {
       "alert": {},
       "reaction": "solo",
       "sound": "illusion is dropping"
     },
     "spells_interrupt_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spells_interrupt_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spells_invis_already": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spells_invis_dropping_you": {
       "alert": {},
       "reaction": "solo",
       "sound": "invis is dropping"
     },
     "spells_levitate_block": {
@@ -9295,106 +9568,106 @@
     "spells_levitate_dropping_you": {
       "alert": {},
       "reaction": "solo",
       "sound": "levitate is dropping"
     },
     "spells_memorize_abort": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spells_memorize_already": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spells_memorize_begin": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spells_memorize_finish": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spells_memorize_too_high": {
       "alert": {},
       "reaction": "solo",
       "sound": "I need more experience before learning that"
     },
     "spells_no_target": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spells_not_hold": {
       "alert": {},
       "reaction": "raid",
       "sound": "did not hold"
     },
     "spells_protected_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spells_protected_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spells_recover_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spells_recover_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spells_resist_other": {
       "alert": {},
       "reaction": "solo",
       "sound": "resist"
     },
     "spells_resist_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spells_scribe_begin": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spells_scribe_finish": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spells_scribe_swap": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spells_scribe_swap_instruction": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spells_sitting": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spells_song_end": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spells_stun_cast_block": {
       "alert": {},
       "reaction": "solo",
       "sound": "cant cast"
     },
     "spells_summoned_you": {
@@ -9406,348 +9679,348 @@
       "alert": {},
       "reaction": "solo",
       "sound": "too powerful"
     },
     "spells_worn_off": {
       "alert": {},
       "reaction": "solo",
-      "sound": "true"
+      "sound": true
     }
   },
   "version": "%s"
 }
 """
 
     new_line_spell_specific_config = """
 {
   "line": {
     "spell_aanyas_quickening_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_aanyas_quickening_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_abolish_enchantment_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_abolish_enchantment_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_acid_jet_other_casts": {
       "alert": {},
       "reaction": "solo",
       "sound": "acid jet"
     },
     "spell_acid_jet_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_adorning_grace_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_adorning_grace_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_aegis_of_bathezid_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_aegis_of_bathezid_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "aegis of bathezid dropped"
     },
     "spell_aegis_of_bathezid_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_aegis_of_ro_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_aegis_of_ro_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "aegis of ro dropped"
     },
     "spell_aegis_of_ro_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_aegis_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_aegis_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_aegolism_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_aegolism_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "aegolism dropped"
     },
     "spell_aegolism_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_agility_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_agilmentes_aria_of_eagles_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_agilmentes_aria_of_eagles_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "agilementes aria of eagles dropped"
     },
     "spell_agilmentes_aria_of_eagles_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_allure_of_death_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_alluring_aura_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_alluring_aura_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_aloe_sweat_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_aloe_sweat_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "aloe swear dropped"
     },
     "spell_aloe_sweat_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_anarchy_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_anarchy_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_ancient_breath_you_on": {
       "alert": {},
       "reaction": "solo",
       "sound": "get a disease cure"
     },
     "spell_annul_magic_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_annul_magic_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_anthem_de_arms_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_armor_of_protection_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_asystole_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "asystole dropped"
     },
     "spell_asystole_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_atols_spectral_shackles_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_atols_spectral_shackles_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_atone_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_atone_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_aura_of_black_petals_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_aura_of_black_petals_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "aura of black petals dropped"
     },
     "spell_aura_of_black_petals_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_aura_of_blue_petals_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_aura_of_blue_petals_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "aura of blue petals dropped"
     },
     "spell_aura_of_blue_petals_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_aura_of_green_petals_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_aura_of_green_petals_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "aura of green petals dropped"
     },
     "spell_aura_of_green_petals_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_aura_of_marr_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_aura_of_marr_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "aura of marr dropped"
     },
     "spell_aura_of_red_petals_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_aura_of_red_petals_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "aura of red petals dropped"
     },
     "spell_aura_of_red_petals_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_aura_of_white_petals_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_aura_of_white_petals_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "aura of white petals dropped"
     },
     "spell_aura_of_white_petals_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_avalanche_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_avalanche_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_avatar_other_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_avatar_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_avatar_power_you_on": {
       "alert": {},
       "reaction": "raid",
       "sound": "avatar power"
     },
     "spell_avatar_snare_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_avatar_snare_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "avatar snare dropped"
     },
     "spell_avatar_snare_you_on": {
@@ -9758,426 +10031,426 @@
     "spell_avatar_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "avatar dropped"
     },
     "spell_avatar_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_bane_of_nife_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_bane_of_nife_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_banshee_aura_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_banshee_aura_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "banshee aura dropped"
     },
     "spell_banshee_aura_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_barbcoat_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_barbcoat_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_barrier_of_combustion_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_barrier_of_force_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_barrier_of_force_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "barrier of force dropped"
     },
     "spell_barrier_of_force_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_battery_vision_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_battery_vision_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "battery vision dropped"
     },
     "spell_battery_vision_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_bedlam_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_bedlam_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "bedlam dropped"
     },
     "spell_bedlam_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_berserker_spirit_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "berserker spirit dropped"
     },
     "spell_berserker_spirit_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_berserker_strength_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_berserker_strength_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "berserker strength dropped"
     },
     "spell_berserker_strength_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_bind_affinity_other_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_bind_affinity_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_bind_affinity_you_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_bind_affinity_you_on": {
       "alert": {},
       "reaction": "solo",
       "sound": "character bind updated"
     },
     "spell_bind_sight_you_off": {
       "alert": {},
       "reaction": "spell",
       "sound": "bind sight dropped"
     },
     "spell_bind_sight_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_bladecoat_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_bladecoat_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_blast_of_cold_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_blast_of_cold_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_blessing_of_nature_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_blessing_of_nature_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_blessing_of_the_blackstar_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_blessing_of_the_blackstar_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_blessing_of_the_theurgist_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_blinding_fear_other_cast": {
       "alert": {},
       "reaction": "raid",
       "sound": "blinding fear"
     },
     "spell_blinding_fear_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_blizzard_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_blizzard_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_blood_claw_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_blood_claw_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "blood claw dropped"
     },
     "spell_blood_claw_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_bobbing_corpse_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_bobbing_corpse_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_boil_blood_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_boil_blood_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_bonds_of_force_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_bonds_of_force_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_bonds_of_tunare_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_bonds_of_tunare_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_bone_shatter_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_boneshear_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_boon_of_the_garou_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_boon_of_the_garou_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_bramblecoat_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_bramblecoat_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_bravery_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_bravery_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "bravery dropped"
     },
     "spell_bravery_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_breath_of_karana_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_breath_of_karana_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_breath_of_the_dead_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_breath_of_the_dead_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_breath_of_the_sea_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_breath_of_the_sea_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "breath of the sea dropped"
     },
     "spell_breath_of_the_sea_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_breeze_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_breeze_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "breeze dropped"
     },
     "spell_breeze_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_brilliance_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_brilliance_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "brilliance dropped"
     },
     "spell_bruscos_boastful_bellow_other_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_bruscos_boastful_bellow_you_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_bruscos_bombastic_bellow_other_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_bruscos_bombastic_bellow_you_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_bulwark_of_faith_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_bulwark_of_faith_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_burn_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_burn_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_burning_vengeance_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_burning_vengeance_you_on": {
       "alert": {},
       "reaction": "group",
       "sound": "burning vengeance"
     },
     "spell_burrowing_scarab_other_cast": {
@@ -10188,146 +10461,146 @@
     "spell_burrowing_scarab_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "burrowing scarab dropped"
     },
     "spell_burrowing_scarab_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_burst_of_fire_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_burst_of_fire_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_burst_of_flame_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_burst_of_flame_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_burst_of_strength_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_cadeau_of_flame_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_cadeau_of_flame_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_calefaction_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_calefaction_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_calimony_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_calimony_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "calimony dropped"
     },
     "spell_calimony_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_call_of_earth_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_call_of_earth_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "call of earth dropped"
     },
     "spell_call_of_earth_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_call_of_flame_other_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_call_of_flame_you_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_call_of_sky_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_call_of_sky_strike_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_call_of_sky_strike_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_call_of_sky_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "call of sky dropped"
     },
     "spell_call_of_sky_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_call_of_the_hero_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_call_of_the_predator_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_call_of_the_predator_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "call of the predator dropped"
     },
     "spell_call_of_the_predator_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_call_of_the_zero_other_on": {
       "alert": {},
       "reaction": "raid",
       "sound": "call of the zero"
     },
     "spell_call_of_the_zero_you_on": {
@@ -10338,2036 +10611,2036 @@
     "spell_camouflage_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "camouflage dropped"
     },
     "spell_camouflage_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_cancel_magic_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_cancel_magic_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_captain_nalots_quickening_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_captain_nalots_quickening_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "captain nalots quickening dropped"
     },
     "spell_captain_nalots_quickening_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_cascade_of_hail_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_cascade_of_hail_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_cassindras_chorus_of_clarity_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_cassindras_chorus_of_clarity_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_cassindras_elegy_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_cassindras_elegy_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_cassindras_insipid_ditty_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_cassindras_insipid_ditty_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "cassindras insipid ditty dropped"
     },
     "spell_cassindras_insipid_ditty_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_cast_force_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_cast_force_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_cast_sight_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "cast sight dropped"
     },
     "spell_cast_sight_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_center_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_center_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "center dropped"
     },
     "spell_center_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_cessation_of_cor_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_cessation_of_cor_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "cessation of cor dropped"
     },
     "spell_cessation_of_cor_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_ceticious_cloud_other_cast": {
       "alert": {},
       "reaction": "raid",
       "sound": "sev poison"
     },
     "spell_ceticious_cloud_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_ceticious_cloud_you_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_ceticious_cloud_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_chant_of_battle_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_chant_of_battle_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_chaos_flux_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_chaos_flux_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_chaotic_feedback_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_chaotic_feedback_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_char_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_char_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_chase_the_moon_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_chase_the_moon_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "chase the moon dropped"
     },
     "spell_chase_the_moon_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_chill_bones_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_chill_bones_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_chill_of_unlife_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_chill_of_unlife_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "chill of unlife dropped"
     },
     "spell_chill_of_unlife_you_on": {
       "alert": {},
       "reaction": "group",
       "sound": "chill of unlife"
     },
     "spell_chilling_embrace_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_chilling_embrace_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "chilling embrace dropped"
     },
     "spell_chilling_embrace_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_chloroblast_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_chloroblast_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_cindas_charismatic_carillon_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "cindas charismatic carillion dropped"
     },
     "spell_cindas_charismatic_carillon_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_circle_of_force_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_circle_of_force_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_circle_of_summer_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_circle_of_summer_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "circle of summer dropped"
     },
     "spell_circle_of_summer_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_circle_of_the_combines_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_circle_of_winter_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_circle_of_winter_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "circle of winter dropped"
     },
     "spell_circle_of_winter_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_cleanse_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_clinging_darkness_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_clinging_darkness_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_clockwork_poison_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_clockwork_poison_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "clockwork poison dropped"
     },
     "spell_clockwork_poison_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_cloud_of_fear_you_on": {
       "alert": {},
       "reaction": "raid",
       "sound": "silence"
     },
     "spell_cloud_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_cloud_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_cog_boost_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_cog_boost_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "cog boost dropped"
     },
     "spell_cog_boost_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_coldlight_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_coldlight_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_color_slant_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_color_slant_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_column_of_fire_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_column_of_fire_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_column_of_lightning_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_column_of_lightning_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_combust_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_companion_spirit_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_complete_healing_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_complete_healing_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_concussion_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_concussion_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_conglaciation_of_bone_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_conglaciation_of_bone_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_courage_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_courage_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "courage dropped"
     },
     "spell_courage_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_creeping_vision_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_creeping_vision_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_cripple_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_cripple_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_crissions_pixie_strike_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_cure_blindness_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_curse_of_the_simple_mind_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_curse_of_the_simple_mind_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "curse of the simple mind dropped"
     },
     "spell_curse_of_the_simple_mind_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_curse_of_the_spirits_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_curse_of_the_spirits_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "curse of the spirits dropped"
     },
     "spell_curse_of_the_spirits_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_dance_of_the_blade_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "dance of the blade dropped"
     },
     "spell_dance_of_the_blade_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_dance_of_the_fireflies_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_dance_of_the_fireflies_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_daring_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_daring_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "daring dropped"
     },
     "spell_daring_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_dark_empathy_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_dark_empathy_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_dark_pact_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_dawncall_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_dawncall_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "dawncall dropped"
     },
     "spell_dawncall_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_dead_man_floating_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_dead_man_floating_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "dead man floating dropped"
     },
     "spell_dead_man_floating_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_deadly_lifetap_other_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_deadly_lifetap_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_deadly_velium_poison_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_deadly_velium_poison_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "deadly velium poison dropped"
     },
     "spell_deadly_velium_poison_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_death_pact_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_death_pact_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_deliriously_nimble_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_deliriously_nimble_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_dementia_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_dementia_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_dementing_visions_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_dementing_visions_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_denons_bereavement_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_denons_bereavement_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_denons_desperate_dirge_other_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_denons_desperate_dirge_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_denons_desperate_dirge_you_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_denons_desperate_dirge_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_desperate_hope_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_desperate_hope_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "desperate hope dropped"
     },
     "spell_desperate_hope_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_devouring_darkness_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_devouring_darkness_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_dexterous_aura_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_dexterous_aura_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "dexterous aura dropped"
     },
     "spell_diamondskin_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_diamondskin_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_discordant_mind_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_discordant_mind_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_disease_cloud_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_disease_cloud_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "disease cloud dropped"
     },
     "spell_disease_cloud_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_diseased_cloud_other_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_diseased_cloud_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_diseased_cloud_you_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_diseased_cloud_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_disintegrate_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_distraction_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_distraction_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_divine_aura_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_divine_barrier_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_divine_barrier_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "divine barrier dropped"
     },
     "spell_divine_barrier_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_divine_favor_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_divine_favor_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "divine favor dropped"
     },
     "spell_divine_favor_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_divine_glory_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_divine_glory_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "divine glory dropped"
     },
     "spell_divine_glory_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_divine_intervention_other_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_divine_intervention_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_divine_intervention_you_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_divine_intervention_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "divine intervention dropped"
     },
     "spell_divine_intervention_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_divine_light_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_divine_light_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_divine_might_effect_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_divine_might_effect_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_divine_might_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_divine_might_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "divine might dropped"
     },
     "spell_divine_might_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_divine_purpose_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_divine_purpose_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "divine purpose dropped"
     },
     "spell_divine_purpose_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_divine_strength_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_divine_strength_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "divine strength dropped"
     },
     "spell_divine_strength_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_divine_wrath_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_dizzy_i_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_dizzy_iv_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_doljons_rage_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_doljons_rage_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_dot_nec_heart_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_draconic_rage_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_draconic_rage_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "draconic rage dropped"
     },
     "spell_draconic_rage_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_dragon_roar_other_cast": {
       "alert": {},
       "reaction": "raid",
       "sound": "roar"
     },
     "spell_dragon_roar_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_draught_of_fire_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_draught_of_fire_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_draught_of_ice_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_draught_of_ice_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_draught_of_jiva_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_draught_of_jiva_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_drybonefireburst_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_drybonefireburst_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_dulsehound_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_dulsehound_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_earthcall_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_earthcall_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "earthcall dropped"
     },
     "spell_earthcall_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_earthelementalattack_other_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_earthelementalattack_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_earthquake_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_earthquake_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_echinacea_infusion_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_echinacea_infusion_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "echinacea infusion dropped"
     },
     "spell_echinacea_infusion_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_efreeti_fire_you_on": {
       "alert": {},
       "reaction": "group",
       "sound": "efreeti fire"
     },
     "spell_egress_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_electric_blast_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_electric_blast_you_on": {
       "alert": {},
       "reaction": "raid",
       "sound": "electric blast"
     },
     "spell_elemental_armor_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "elemental armor dropped"
     },
     "spell_elemental_maelstrom_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_elemental_maelstrom_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "elemental maelstrom dropped"
     },
     "spell_elemental_maelstrom_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_elemental_rhythms_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_elemental_shield_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "elemental shield dropped"
     },
     "spell_embrace_of_the_kelpmaiden_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_embrace_of_the_kelpmaiden_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "embrace of the kelp maiden dropped"
     },
     "spell_embrace_of_the_kelpmaiden_you_on": {
       "alert": {},
       "reaction": "solo",
       "sound": "kelp maiden snare"
     },
     "spell_endure_cold_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_endure_cold_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "endure cold dropped"
     },
     "spell_endure_disease_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_endure_disease_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "endure disease dropped"
     },
     "spell_endure_fire_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_endure_fire_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "endure fire dropped"
     },
     "spell_endure_magic_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_endure_magic_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "endure magic dropped"
     },
     "spell_endure_poison_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_endure_poison_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "endure poison dropped"
     },
     "spell_energy_sap_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_energy_sap_you_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_energy_sap_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "energy sap dropped"
     },
     "spell_energy_sap_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_energy_storm_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_energy_storm_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_enfeeblement_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_enfeeblement_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_enforced_reverence_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_enforced_reverence_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_engorging_roots_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_engorging_roots_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_enlightenment_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_enlightenment_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "enlightenment dropped"
     },
     "spell_enlightenment_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_ensnare_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "ensnare dropped"
     },
     "spell_enthrall_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_enthrall_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "enthrall dropped"
     },
     "spell_enthrall_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_enticement_of_flame_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_enticement_of_flame_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_entomb_in_ice_other_cast": {
       "alert": {},
       "reaction": "raid",
       "sound": "ice"
     },
     "spell_entomb_in_ice_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "entomb in ice dropped"
     },
     "spell_entrance_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_entrance_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "entrance dropped"
     },
     "spell_entrance_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_envenomed_breath_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_envenomed_heal_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_envenomed_heal_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_essence_drain_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_essence_tap_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_eye_of_confusion_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_eye_of_confusion_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "eye of confusion dropped"
     },
     "spell_eye_of_confusion_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_eye_of_tallon_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "eye of tallon dropped"
     },
     "spell_eyes_of_the_cat_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_fade_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_fade_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "fade dropped"
     },
     "spell_fade_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_fangols_breath_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_fangols_breath_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_fascination_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_fascination_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "fascination dropped"
     },
     "spell_fascination_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_fatigue_drain_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_fatigue_drain_you_on": {
       "alert": {},
       "reaction": "solo",
       "sound": "fatigue drain"
     },
     "spell_fear_other_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_fear_you_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_feeble_mind_iv_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_feedback_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_feedback_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "feedback dropped"
     },
     "spell_feedback_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_feet_like_cat_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_feet_like_cat_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_feign_death_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_feign_death_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "feign death dropped"
     },
     "spell_fellspine_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_fellspine_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "fellspine dropped"
     },
     "spell_fellspine_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_fiery_might_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_fiery_might_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "fiery might dropped"
     },
     "spell_fiery_might_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_fingers_of_fire_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_fire_spiral_of_alkabor_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_fire_spiral_of_alkabor_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_firefist_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_firefist_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "firefist dropped"
     },
     "spell_firefist_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_firestorm_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_fist_of_karana_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_fist_of_karana_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_fist_of_sentience_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_fist_of_sentience_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "fist of sentience dropped"
     },
     "spell_fist_of_sentience_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_fist_of_water_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_fist_of_water_you_on": {
       "alert": {},
       "reaction": "solo",
       "sound": "fist of water"
     },
     "spell_fixation_of_ro_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_fixation_of_ro_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "fixation of ro dropped"
     },
     "spell_fixation_of_ro_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_flame_jet_other_cast": {
       "alert": {},
       "reaction": "group",
       "sound": "flame jet"
     },
     "spell_flame_jet_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_flame_lick_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_flame_lick_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "flame lick dropped"
     },
     "spell_flame_lick_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_flame_of_light_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_flame_of_light_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_flame_of_the_efreeti_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_flame_of_the_efreeti_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_flames_of_ro_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_flames_of_ro_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_flavor_nec_hp": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_fleeting_fury_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_fleeting_fury_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_flurry_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_flurry_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "flurry dropped"
     },
     "spell_flurry_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_focus_of_spirit_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_focus_of_spirit_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "focus of spirit dropped"
     },
     "spell_focus_of_spirit_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_force_spiral_of_alkabor_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_force_spiral_of_alkabor_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_form_of_the_great_bear_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_form_of_the_great_bear_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "form of the great bear dropped"
     },
     "spell_form_of_the_great_bear_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_fortitude_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_fortitude_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_freezing_breath_other_cast": {
       "alert": {},
       "reaction": "raid",
       "sound": "freezing breath"
     },
     "spell_freezing_breath_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_freezing_breath_you_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_freezing_breath_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_frenzied_spirit_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_frenzied_spirit_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_frenzied_strength_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_frenzied_strength_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_frost_bolt_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_frost_bolt_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_frost_breath_other_cast": {
       "alert": {},
       "reaction": "raid",
       "sound": "frost breath"
     },
     "spell_frost_breath_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_frost_breath_you_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_frost_breath_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_frost_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_frost_rift_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_frost_rift_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_frost_storm_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_frost_storm_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "frost storm dropped"
     },
     "spell_frost_storm_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_frost_strike_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_frost_strike_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_frost_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_frostbite_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_frostbite_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_frostreavers_blessing_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_frostreavers_blessing_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "frostreavers blessing dropped"
     },
     "spell_frostreavers_blessing_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_frosty_death_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_frosty_death_you_on": {
       "alert": {},
       "reaction": "solo",
       "sound": "frosty death"
     },
     "spell_fufils_curtailing_chant_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_fufils_curtailing_chant_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "fufils curtailing chant dropped"
     },
     "spell_fufils_curtailing_chant_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_fungal_regrowth_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_fungal_regrowth_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_fungus_spores_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_fungus_spores_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "fungus spores dropped"
     },
     "spell_fungus_spores_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_furor_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_furor_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_gangrenous_touch_of_zumuul_other_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_gangrenous_touch_of_zumuul_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_gangrenous_touch_of_zumuul_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_garzicors_vengeance_other_on": {
       "alert": {},
       "reaction": "solo",
       "sound": "garzicor is not happy"
     },
     "spell_garzicors_vengeance_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "garzicors vengeance dropped"
     },
     "spell_gather_shadows_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_gather_shadows_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "gather shadows dropped"
     },
     "spell_gather_shadows_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_gaze_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "gaze dropped"
     },
     "spell_gaze_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_gelatroot_other_cast": {
       "alert": {},
       "reaction": "solo",
       "sound": "gel root"
     },
     "spell_gelatroot_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "gelatinous root dropped"
     },
     "spell_gelatroot_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_ghoul_root_other_cast": {
       "alert": {},
       "reaction": "solo",
       "sound": "ghoul root"
     },
     "spell_ghoul_root_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "ghoul root dropped"
     },
     "spell_ghoul_root_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_gift_of_aerr_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_gift_of_aerr_you_on": {
       "alert": {},
       "reaction": "raid",
       "sound": "lifetap a.e."
     },
     "spell_gift_of_brilliance_you_off": {
@@ -12388,826 +12661,826 @@
     "spell_girdle_of_karana_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "girdle of karana dropped"
     },
     "spell_girdle_of_karana_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_glamour_of_kintaz_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_glamour_of_kintaz_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_glamour_of_tunare_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_glamour_of_tunare_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "glamour of tunare dropped"
     },
     "spell_graveyard_dust_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_graveyard_dust_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_grease_injection_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_grease_injection_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "grease injection dropped"
     },
     "spell_grease_injection_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_greenmist_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_greenmist_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_grim_aura_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_grim_aura_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "grim aura dropped"
     },
     "spell_grim_aura_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_guardian_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_guardian_rhythms_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_guardian_spirit_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_guardian_spirit_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_guardian_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "guardian dropped"
     },
     "spell_guardian_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_halo_of_light_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_halo_of_light_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_harmshield_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_harpy_voice_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "harpy voice dropped"
     },
     "spell_harpy_voice_you_on": {
       "alert": {},
       "reaction": "raid",
       "sound": "you have been mesmerized"
     },
     "spell_harvest_leaves_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_harvest_leaves_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_harvest_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_harvest_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_haste_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "haste dropped"
     },
     "spell_health_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_health_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_heart_flutter_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "heart flutter dropped"
     },
     "spell_heart_flutter_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_heat_blood_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_heat_blood_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_holy_shock_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_holy_shock_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_hug_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_hug_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "hug dropped"
     },
     "spell_hug_you_on": {
       "alert": {},
       "reaction": "solo",
       "sound": "hug"
     },
     "spell_ice_breath_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_ice_breath_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "ice breath dropped"
     },
     "spell_ice_breath_you_on": {
       "alert": {},
       "reaction": "solo",
       "sound": "ice breath"
     },
     "spell_ice_rend_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_ice_rend_you_on": {
       "alert": {},
       "reaction": "solo",
       "sound": "ice rend"
     },
     "spell_ice_spear_of_solist_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_ice_spear_of_solist_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_ice_strike_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_ice_strike_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "ice strike dropped"
     },
     "spell_ice_strike_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_icestrike_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_icestrike_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_ignite_bones_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_ignite_bones_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_immolate_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_immolate_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "immolate dropped"
     },
     "spell_immolate_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_immolating_breath_other_cast": {
       "alert": {},
       "reaction": "raid",
       "sound": "immolating breath"
     },
     "spell_immolating_breath_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_immolating_breath_you_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_immolating_breath_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_impart_strength_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "impart strength dropped"
     },
     "spell_incinerate_bones_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_incinerate_bones_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_infectious_cloud_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_infectious_cloud_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_inferno_of_alkabor_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_inferno_of_alkabor_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_infusion_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_infusion_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_inner_fire_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "inner fire dropped"
     },
     "spell_insight_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_insight_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "insight dropped"
     },
     "spell_insight_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_inspire_fear_other_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_invert_gravity_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_invigorate_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_invisibility_cloak_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_invisibility_cloak_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_invoke_fear_other_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_jonthans_inspiration_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "jonthans inspiration dropped"
     },
     "spell_jonthans_inspiration_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_jonthans_provocation_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_jonthans_provocation_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "jonthans provocation dropped"
     },
     "spell_jonthans_provocation_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_jonthans_whistling_warsong_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "jonthans whistling warsong dropped"
     },
     "spell_jonthans_whistling_warsong_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_jylls_static_pulse_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_jylls_static_pulse_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_jylls_wave_of_heat_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_jylls_wave_of_heat_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_jylls_zephyr_of_ice_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_jylls_zephyr_of_ice_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_kazumis_note_of_preservation_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "kazumis note of preservation dropped"
     },
     "spell_kelins_lucid_lullaby_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_kelins_lucid_lullaby_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "kelins lucis lullaby dropped"
     },
     "spell_kelins_lucid_lullaby_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_kelins_lugubrious_lament_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_kelins_lugubrious_lament_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "kelins lugubrious lament dropped"
     },
     "spell_kelins_lugubrious_lament_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_knockback_other_cast": {
       "alert": {},
       "reaction": "solo",
       "sound": "knockback"
     },
     "spell_knockback_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_knockback_you_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_knockback_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_kylies_venom_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_kylies_venom_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_largarns_lamentation_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_largarns_lamentation_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "largarns lamentation dropped"
     },
     "spell_largarns_lamentation_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_largos_absonant_binding_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "largos absonant binding dropped"
     },
     "spell_lava_breath_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_lava_breath_you_on": {
       "alert": {},
       "reaction": "group",
       "sound": "lava breath"
     },
     "spell_lava_storm_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_leach_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_leach_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_leatherskin_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_leatherskin_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_levant_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_levitate_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_levitate_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "levitate dropped"
     },
     "spell_levitate_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_life_leech_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_light_healing_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_lightning_bolt_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_lightning_bolt_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_lightning_breath_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_lightning_breath_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_lightning_shock_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_lightning_storm_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_lightning_storm_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_lightning_strike_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_lightning_strike_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_agility_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_agility_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "agility spell dropped"
     },
     "spell_line_aura_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "aura spell dropped"
     },
     "spell_line_bard_cancel_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_berserk_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_berserk_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "berserk spell dropped"
     },
     "spell_line_berserk_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_berserker_madness_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_berserker_madness_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "berserker madness spell dropped"
     },
     "spell_line_berserker_madness_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_bind_sight_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_blind_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_blind_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "blind spell dropped"
     },
     "spell_line_blind_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_blinding_poison_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_blinding_poison_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_blizzard_blast_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_blizzard_blast_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_boil_blood_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "boil blood spell dropped"
     },
     "spell_line_bolt_of_flame_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_bolt_of_flame_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_bolt_of_karana_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_bolt_of_karana_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_brd_bruscos_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_brd_bruscos_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_brd_cc_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_brd_charm_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "bard charm dropped"
     },
     "spell_line_brd_dd_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_brd_haste_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_brd_resists_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "bard resist dropped"
     },
     "spell_line_brd_slow_other_on": {
@@ -13223,1136 +13496,1136 @@
     "spell_line_brd_strands_fade_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "lyssas solidarity of vision dropped"
     },
     "spell_line_brd_tuyen_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_brd_tuyen_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "bard tuyen dropped"
     },
     "spell_line_brd_tuyen_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_brittle_haste_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "brittle haste spell dropped"
     },
     "spell_line_brittle_haste_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_cannibalize_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_cat_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_charisma_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_charisma_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "charisma spell dropped"
     },
     "spell_line_charisma_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_charm_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_charm_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "charm spell dropped"
     },
     "spell_line_charm_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_clarity_ii_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_clarity_ii_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "clarity two dropped"
     },
     "spell_line_clarity_ii_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_clarity_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_clarity_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "clarity dropped"
     },
     "spell_line_clarity_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_cold_resist_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_combust_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_combusts_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_debuff_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_debuff_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "debuff spell dropped"
     },
     "spell_line_debuff_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_defoliation_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_dexterity_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_dexterity_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "dexterity spell dropped"
     },
     "spell_line_dexterity_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_disease_resist_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_dizzy_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_dot_disease_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_dot_disease_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "disease dot spell dropped"
     },
     "spell_line_dot_disease_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_dot_enc_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_dot_enc_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "enchanter dot spell dropped"
     },
     "spell_line_dot_enc_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_dru_best_hp_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_dru_best_hp_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_dru_ds_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_dru_ds_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "druid damage shield dropped"
     },
     "spell_line_dru_ds_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_dru_fire_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_dru_fire_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_dru_root_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_dru_root_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "i'm free!"
     },
     "spell_line_dru_root_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_dru_skyfire_or_ej_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_dru_skyfire_or_ej_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_dru_tree_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_dru_tree_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "leaf me out of this"
     },
     "spell_line_dru_tree_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_enc_ac_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_enc_ac_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "enchanter armor spell dropped"
     },
     "spell_line_enc_ac_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_enc_cancel_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_enc_cancel_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_enc_charisma_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "enchanter charisma spell dropped"
     },
     "spell_line_enc_debuff_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_enc_debuff_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_enc_mana_buff_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_enc_mana_buff_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_enc_slow_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_enc_slow_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "enchanter slow spell dropped"
     },
     "spell_line_enc_slow_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_enc_stun_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_enc_stun_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "enchanter stun spell dropped"
     },
     "spell_line_enc_stun_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_endurance_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_endurance_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_enduring_breath_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_enduring_breath_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "you can't breath"
     },
     "spell_line_enduring_breath_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_faction_increase_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_faction_increase_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "faction increase spell dropped"
     },
     "spell_line_faction_increase_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_fade_away_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_fear_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_fear_undead_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_fear_undead_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_fear_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "fear spell dropped"
     },
     "spell_line_fear_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_feeble_mind_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_feel_better_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "that was nice"
     },
     "spell_line_fire_ds_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "fire damage shield dropped"
     },
     "spell_line_fire_flame_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_fire_flame_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_fire_flames_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_fire_flames_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_fire_ignite_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_fire_ignite_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_fire_resist_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_flesh_rot_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_flesh_rot_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "flesh rot spell dropped"
     },
     "spell_line_flesh_rot_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_force_strike_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_force_strike_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_fragile_sow_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_fragile_sow_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_frost_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_frost_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_fury_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "fury spell dropped"
     },
     "spell_line_grav_flux_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_grav_flux_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_group_portal_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_group_portal_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "let's go"
     },
     "spell_line_hammer_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_haste_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_haste_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "haste spell dropped"
     },
     "spell_line_haste_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_haste_stats_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_npc_item_haste_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_healing_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_healing_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_heroic_valor_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_heroic_valor_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "heroic valor spell dropped"
     },
     "spell_line_heroic_valor_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_holy_armor_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_holy_armor_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "holy armor spell dropped"
     },
     "spell_line_holy_armor_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_holy_ds_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "holy damage shield spell dropped"
     },
     "spell_line_holy_guard_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "holy guard spell dropped"
     },
     "spell_line_hot_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_hot_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "heal over time spell dropped"
     },
     "spell_line_hot_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_hungry_earth_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_illusion_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_illusion_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "illusion dropped"
     },
     "spell_line_illusion_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_infravision_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_infravision_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "infravision spell dropped"
     },
     "spell_line_infravision_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_int_caster_shield_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "caster shield spell dropped"
     },
     "spell_line_int_caster_shield_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_int_resists_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_int_resists_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_invis_animal_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_invis_animal_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "invis against animals spell dropped"
     },
     "spell_line_invis_animal_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_invis_undead_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_invis_undead_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "invis against undead spell dropped"
     },
     "spell_line_invis_undead_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_invis_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "invis dropped"
     },
     "spell_line_invis_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_invulnerable_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "invulnerable dropped"
     },
     "spell_line_koi_or_trident_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_lava_storm_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_leach_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_liquid_silver_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_liquid_silver_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_low_nec_mana_regen_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_low_tash_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_lower_resists_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_mag_armor_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "magician armor dropped"
     },
     "spell_line_mag_ds_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_high_mag_ds_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_low_mag_ds_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_mag_shock_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_mag_shock_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_mag_sow_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_magic_resist_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_magic_resist_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_magnify_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_magnify_you_off": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_magnify_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_malo_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_malo_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "malo spell dropped"
     },
     "spell_line_malo_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_memblur_other_on": {
       "alert": {},
       "reaction": "raid",
       "sound": "memblur"
     },
     "spell_line_memblur_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_mez_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_mez_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "mesmerization spell dropped"
     },
     "spell_line_mez_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_mind_clears_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_minor_shielding_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "minor shielding spell dropped"
     },
     "spell_line_muscle_lock_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_nec_charm_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_nec_fire_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_nec_fire_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_nec_haste_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_nec_heal_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_nec_heal_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "necromancer heal spell dropped"
     },
     "spell_line_nec_hp_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "necromancer hp spell dropped"
     },
     "spell_line_nec_hp_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_nec_pet_heal_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_nec_pet_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_nec_regen_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_nec_regen_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "necromancer regeneration spell dropped"
     },
     "spell_line_nec_regen_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_nec_scent_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_nec_snare_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_nec_snare_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "necromancer snare spell dropped"
     },
     "spell_line_nec_snare_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_nec_twitch_other_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_nec_twitch_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_nec_twitch_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_npc_buff_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "how did you do that?"
     },
     "spell_line_npc_disease_other_cast": {
       "alert": {},
       "reaction": "solo",
       "sound": "disease"
     },
     "spell_line_npc_disease_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_npc_disease_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "disease spell dropped"
     },
     "spell_line_npc_disease_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_npc_fire_you_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_npc_fire_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "fire spell dropped"
     },
     "spell_line_npc_item_poison_other_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_npc_port_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_npc_root_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_npc_sick_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_npc_thunder_other_cast": {
       "alert": {},
       "reaction": "solo",
       "sound": "thunder"
     },
     "spell_line_npc_thunder_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_pacify_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_pacify_undead_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_pacify_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_paralyzing_poison_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_paralyzing_poison_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_peace_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_pet_haste_or_rabies_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_poison_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_poison_resist_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_poison_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "poison spell dropped"
     },
     "spell_line_poison_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_portal_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_potion_ds_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_potion_ds_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "potion damage shield dropped"
     },
     "spell_line_potion_ds_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_potion_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_potion_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "potion effect has worn off"
     },
     "spell_line_potion_you_on": {
@@ -14363,211 +14636,211 @@
     "spell_line_protection_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "protection spell dropped"
     },
     "spell_line_protection_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_raid_ae_other_cast": {
       "alert": {},
       "reaction": "raid",
       "sound": "a.e."
     },
     "spell_line_raid_silence_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_raid_silence_you_on": {
       "alert": {},
       "reaction": "raid",
       "sound": "silence"
     },
     "spell_line_regen_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_regen_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "regeneration spell dropped"
     },
     "spell_line_regen_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_rng_aggro_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_rng_aggro_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_root_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_root_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "root spell dropped"
     },
     "spell_line_root_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_rune_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_rune_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "rune spell dropped"
     },
     "spell_line_rune_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_scarab_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_see_invis_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_see_invis_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "see invis dropped"
     },
     "spell_line_see_invis_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_shm_dis_dd_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_shm_dis_dd_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_shm_dr_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "shaman disease resist spell dropped"
     },
     "spell_line_shm_hp_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_shm_hp_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "shaman HP buff spell dropped"
     },
     "spell_line_shm_hp_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_shm_insidious_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_shm_pet_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_shm_poison_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_shm_poison_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_shm_sta_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_shm_sta_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "shaman stamina spell dropped"
     },
     "spell_line_shm_str_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_shrink_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_shrink_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "did i get taller?"
     },
     "spell_line_shrink_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_siphon_strength_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_siphon_strength_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "siphon strength spell dropped"
     },
     "spell_line_siphon_strength_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_skin_freeze_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_skin_freeze_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_skin_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "skin spell dropped"
     },
     "spell_line_slow_other_on": {
@@ -14583,3331 +14856,3331 @@
     "spell_line_slow_you_on": {
       "alert": {},
       "reaction": "solo",
       "sound": "slow"
     },
     "spell_line_snare_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_snare_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_spin_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_spin_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "spin spell dropped"
     },
     "spell_line_spin_you_on": {
       "alert": {},
       "reaction": "solo",
       "sound": "like a record"
     },
     "spell_line_stagger_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_strength_burst_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "strength burst spell dropped"
     },
     "spell_line_strength_debuff_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_strength_debuff_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "strength debuff spell dropped"
     },
     "spell_line_strength_debuff_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_strength_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_strength_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "strength spell dropped"
     },
     "spell_line_strength_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_stun_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_stun_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "stun spell dropped"
     },
     "spell_line_stun_you_on": {
       "alert": {},
       "reaction": "solo",
       "sound": "stunned"
     },
     "spell_line_swarm_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_swarm_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "swarm spell dropped"
     },
     "spell_line_swarms_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_system_shock_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_target_vision_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_target_vision_you_off": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_target_vision_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_tash_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_tash_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "tash spell dropped"
     },
     "spell_line_tash_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_ultravision_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_ultravision_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "ultravision spell dropped"
     },
     "spell_line_wince_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_wiz_alkabor_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_wiz_alkabor_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_wiz_ds_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_wiz_ds_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "wizard damage shield dropped"
     },
     "spell_line_wiz_ds_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_wiz_ice_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_wiz_ice_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_wiz_plane_port_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_wolf_form_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_wolf_form_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "wolf form spell dropped"
     },
     "spell_line_wolf_form_you_on": {
       "alert": {},
       "reaction": "solo_only",
       "sound": "woof"
     },
     "spell_line_word_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_word_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_yaulp_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_line_yaulp_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_locate_corpse_you_off": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_lower_resists_i_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_lull_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_lure_of_flame_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_lure_of_flame_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_lure_of_frost_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_lure_of_frost_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_lure_of_ice_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_lure_of_ice_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_lure_of_lightning_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_lure_of_lightning_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_lyssas_cataloging_libretto_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_lyssas_locating_lyric_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_lyssas_locating_lyric_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_lyssas_solidarity_of_vision_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_lyssas_solidarity_of_vision_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_lyssas_veracious_concord_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "see invis dropped"
     },
     "spell_lyssas_veracious_concord_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_magi_curse_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_magi_curse_you_on": {
       "alert": {},
       "reaction": "solo",
       "sound": "stun more"
     },
     "spell_malevolent_grasp_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_malevolent_grasp_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "malevolent grasp dropped"
     },
     "spell_malevolent_grasp_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_mana_conversion_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_mana_flare_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_mana_flare_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "mana flare dropped"
     },
     "spell_mana_flare_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_mana_sieve_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_mana_sieve_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_mana_sink_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_manasink_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_manasink_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_manaskin_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_manaskin_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_manastorm_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_manastorm_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_maniacal_strength_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_maniacal_strength_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_manifest_elements_other_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_manifest_elements_you_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_manticore_poison_other_cast": {
       "alert": {},
       "reaction": "solo",
       "sound": "manticore poison"
     },
     "spell_mark_of_karn_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_mark_of_karn_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_mask_of_the_hunter_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_mask_of_the_hunter_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "mask of the hunter dropped"
     },
     "spell_mask_of_the_hunter_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_mcvaxius_berserker_crescendo_you_off": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_mcvaxius_rousing_rondo_you_off": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_mcvaxius_rousing_rondo_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_melanies_mellifluous_motion_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_melanies_mellifluous_motion_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "melanies mellifluous motion dropped"
     },
     "spell_melanies_mellifluous_motion_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_melody_of_ervaj_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "melody of ervaj dropped"
     },
     "spell_mesmerizing_breath_other_cast": {
       "alert": {},
       "reaction": "raid",
       "sound": "silence"
     },
     "spell_mesmerizing_breath_you_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_mind_cloud_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_mind_cloud_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "mind cloud dropped"
     },
     "spell_mind_cloud_you_on": {
       "alert": {},
       "reaction": "solo",
       "sound": "mind cloud"
     },
     "spell_minor_healing_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_minor_healing_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_minor_shielding_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_mistwalker_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_mistwalker_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_modulation_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_modulation_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_mortal_deftness_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_mortal_deftness_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "mortal deftness"
     },
     "spell_mortal_deftness_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_mystic_precision_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_mystic_precision_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "mystic precision dropped"
     },
     "spell_mystic_precision_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_naltrons_mark_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_naltrons_mark_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "naltrons mark dropped"
     },
     "spell_naltrons_mark_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_nature_walkers_behest_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_nature_walkers_behest_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_natures_holy_wrath_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_natures_holy_wrath_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_natures_melody_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_natures_melody_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_natures_wrath_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_natures_wrath_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_nillipus_march_of_the_wee_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_nillipus_march_of_the_wee_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_nimble_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_nimble_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_nivs_harmonic_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "nivs harmonic dropped"
     },
     "spell_nivs_harmonic_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_nivs_melody_of_preservation_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_nullify_magic_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_nullify_magic_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_numbing_cold_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_numbing_cold_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_obscure_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_obscure_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_occlusion_of_sound_other_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_occlusion_of_sound_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_occlusion_of_sound_you_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_one_hundred_blows_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_one_hundred_blows_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "one hundred blows dropped"
     },
     "spell_one_hundred_blows_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_open_black_box_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_open_black_box_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_overwhelming_splendor_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_overwhelming_splendor_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_panic_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_panic_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_phantom_armor_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_phantom_armor_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_phantom_chain_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_phantom_chain_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_phantom_leather_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_phantom_leather_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_phantom_plate_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_phantom_plate_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_pillar_of_frost_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_pillar_of_frost_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_pillar_of_lightning_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_pillar_of_lightning_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_plagueratdisease_other_cast": {
       "alert": {},
       "reaction": "solo",
       "sound": "rat disease"
     },
     "spell_plainsight_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "plainsight dropped"
     },
     "spell_pogonip_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_pogonip_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_poison_breath_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_poisonous_chill_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_poisonous_chill_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_porlos_fury_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_porlos_fury_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_power_of_the_forests_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_power_of_the_forests_you_on": {
       "alert": {},
       "reaction": "raid",
       "sound": "tunare nuked you"
     },
     "spell_pox_of_bertoxxulous_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_pox_of_bertoxxulous_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "pox of bertoxxulous dropped"
     },
     "spell_pox_of_bertoxxulous_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_primal_essence_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_primal_essence_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "primal essence dropped"
     },
     "spell_primal_essence_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_prime_healers_blessing_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_prime_healers_blessing_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "prime healers blessing dropped"
     },
     "spell_prime_healers_blessing_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_project_lightning_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_project_lightning_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_protect_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_protect_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_purifying_rhythms_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_putrefy_flesh_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_putrefy_flesh_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_putrid_breath_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_quivering_veil_of_xarn_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_quivering_veil_of_xarn_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_radiant_visage_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_radiant_visage_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "radiant visage dropped"
     },
     "spell_radiant_visage_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_rage_of_tallon_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_rage_of_tallon_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "rage of tallon dropped"
     },
     "spell_rage_of_tallon_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_rage_of_vallon_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_rage_of_vallon_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "rage of vallon dropped"
     },
     "spell_rage_of_vallon_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_rage_of_zek_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_rage_of_zek_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "rage of zek dropped"
     },
     "spell_rage_of_zek_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_rage_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_rage_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "rage dropped"
     },
     "spell_rage_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_rain_of_molten_lava_you_on": {
       "alert": {},
       "reaction": "raid",
       "sound": "rain of molten lava"
     },
     "spell_rapture_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_rapture_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "rapture dropped"
     },
     "spell_rapture_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_recant_magic_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_recant_magic_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_reckless_health_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_reckless_health_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "reckless health dropped"
     },
     "spell_reckless_health_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_reckless_strength_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_reckless_strength_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_reckoning_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_reckoning_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_reclaim_energy_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_reclaim_energy_you_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_remedy_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_remedy_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_rend_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_rend_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_renew_elements_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_renew_summoning_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_resist_cold_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_resist_cold_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "resist cold dropped"
     },
     "spell_resist_cold_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_resist_disease_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_resist_disease_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "resist disease dropped"
     },
     "spell_resist_disease_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_resist_fire_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_resist_fire_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "resist fire dropped"
     },
     "spell_resist_fire_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_resist_magic_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "resist magic dropped"
     },
     "spell_resist_magic_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_resist_poison_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_resist_poison_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "resist poison dropped"
     },
     "spell_resist_poison_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_resistant_skin_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_resistant_skin_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "resistant skin dropped"
     },
     "spell_resistant_skin_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_resolution_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_resolution_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "resolution dropped"
     },
     "spell_resolution_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_resurrection_effects_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_retribution_of_alkabor_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_retribution_of_alkabor_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_retribution_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_retribution_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_riotous_health_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_riotous_health_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_rotting_flesh_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_rubicite_aura_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_rubicite_aura_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "rubicite aura dropped"
     },
     "spell_rubicite_aura_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_rune_i_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_rune_ii_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_rune_iii_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_savage_spirit_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_savage_spirit_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "savage spirit dropped"
     },
     "spell_savage_spirit_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_scale_of_wolf_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "scale of wolf dropped"
     },
     "spell_scale_skin_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_scale_skin_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "scale skin dropped"
     },
     "spell_scale_skin_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_scarab_storm_other_cast": {
       "alert": {},
       "reaction": "solo",
       "sound": "scarab storm"
     },
     "spell_scarab_storm_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "scarab storm dropped"
     },
     "spell_scarab_storm_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_scars_of_sigil_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_scars_of_sigil_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_scent_of_darkness_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "scent of darkness dropped"
     },
     "spell_scent_of_darkness_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_scent_of_dusk_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_scent_of_dusk_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "scent of dusk dropped"
     },
     "spell_scent_of_dusk_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_scent_of_shadow_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_scent_of_shadow_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "scent of shadow dropped"
     },
     "spell_scent_of_shadow_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_scent_of_terris_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "scent of terris dropped"
     },
     "spell_scent_of_terris_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_scintillation_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_scintillation_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_scoriae_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_scoriae_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_screaming_mace_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_screaming_terror_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_screaming_terror_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "screaming terror dropped"
     },
     "spell_screaming_terror_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_sear_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "sear dropped"
     },
     "spell_sear_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_seeking_flame_of_seukor_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_seeking_flame_of_seukor_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_seething_fury_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_seething_fury_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "seething fury dropped"
     },
     "spell_seething_fury_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_selos_accelerando_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_selos_assonant_strane_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_selos_assonant_strane_you_off": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_selos_assonant_strane_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_selos_chords_of_cessation_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_selos_chords_of_cessation_you_off": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_selos_chords_of_cessation_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_selos_consonant_chain_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_selos_consonant_chain_you_off": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_selos_consonant_chain_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_selos_song_of_travel_you_off": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_selos_song_of_travel_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_sentinel_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shade_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shade_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shadow_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shadow_sight_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "shadow sight dropped"
     },
     "spell_shadow_sight_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shadow_vortex_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shadow_vortex_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "shadow vortex dropped"
     },
     "spell_shadow_vortex_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shadow_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shadowbond_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "shadowbond dropped"
     },
     "spell_shards_of_sorrow_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shards_of_sorrow_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shauris_sonorous_clouding_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "shauris sonorous clouding dropped"
     },
     "spell_shauris_sonorous_clouding_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shield_of_blades_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shield_of_blades_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "shield of blades dropped"
     },
     "spell_shield_of_blades_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shield_of_song_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shield_of_song_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shield_of_the_magi_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "shield of the magi dropped"
     },
     "spell_shieldskin_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shieldskin_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shifting_shield_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shifting_shield_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "shifting shield dropped"
     },
     "spell_shifting_shield_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shifting_sight_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "shifting sight dropped"
     },
     "spell_shifting_sight_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shock_of_lightning_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shock_of_lightning_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shock_of_poison_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shock_of_poison_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shock_of_steel_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shock_of_steel_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shock_spiral_of_alkabor_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shock_spiral_of_alkabor_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shrieking_howl_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shrieking_howl_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shroud_of_death_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shroud_of_death_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shroud_of_hate_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shroud_of_hate_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "shroud of hate dropped"
     },
     "spell_shroud_of_hate_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shroud_of_pain_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shroud_of_pain_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "shroud of pain dropped"
     },
     "spell_shroud_of_pain_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shroud_of_the_spirits_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shroud_of_the_spirits_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "shroud of the spirits dropped"
     },
     "spell_shroud_of_the_spirits_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shroud_of_undeath_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_shroud_of_undeath_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_silver_skin_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_silver_skin_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "silver skin dropped"
     },
     "spell_silver_skin_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_sirocco_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_sirocco_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_skin_like_diamond_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_skin_like_diamond_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_skin_like_nature_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_skin_like_nature_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_skin_like_rock_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_skin_like_rock_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_skin_like_steel_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_skin_like_steel_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_skin_like_wood_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_skin_like_wood_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_skin_of_the_shadow_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_skin_of_the_shadow_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_skunkspray_other_cast": {
       "alert": {},
       "reaction": "solo",
       "sound": "skunk spray"
     },
     "spell_skunkspray_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_skunkspray_you_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_skunkspray_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "you smell a bit better now"
     },
     "spell_skunkspray_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_slime_mist_other_cast": {
       "alert": {},
       "reaction": "solo",
       "sound": "slime mist"
     },
     "spell_slime_mist_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_smite_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_smite_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_smolder_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_smolder_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_snakeelefireburst_other_cast": {
       "alert": {},
       "reaction": "solo",
       "sound": "snake fire"
     },
     "spell_solons_bewitching_bravura_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_solons_song_of_the_sirens_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_song_of_dawn_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_song_of_dawn_you_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_song_of_midnight_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_song_of_midnight_you_off": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_song_of_midnight_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_song_of_the_deep_seas_you_off": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_song_of_the_deep_seas_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_song_of_twilight_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_song_of_twilight_you_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_song_of_twilight_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_soul_devour_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_soul_devour_you_on": {
       "alert": {},
       "reaction": "solo",
       "sound": "soul devour"
     },
     "spell_soul_leech_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_speed_of_the_shissar_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_speed_of_the_shissar_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "speed of the shissar dropped"
     },
     "spell_speed_of_the_shissar_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_spikecoat_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_spikecoat_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_spin_the_bottle_other_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_spirit_armor_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_spirit_armor_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "spirit armor dropped"
     },
     "spell_spirit_armor_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_spirit_of_bear_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_spirit_of_bear_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "spirit of bear dropped"
     },
     "spell_spirit_of_bear_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_spirit_of_cat_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "spirit of cat dropped"
     },
     "spell_spirit_of_cat_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_spirit_of_cheetah_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "spirit of cheetah dropped"
     },
     "spell_spirit_of_cheetah_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_spirit_of_monkey_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_spirit_of_monkey_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "spirit of monkey dropped"
     },
     "spell_spirit_of_monkey_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_spirit_of_ox_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_spirit_of_ox_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "spirit of ox dropped"
     },
     "spell_spirit_of_ox_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_spirit_of_scale_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "spirit of scale dropped"
     },
     "spell_spirit_of_snake_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_spirit_of_snake_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "spirit of snake dropped"
     },
     "spell_spirit_of_snake_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_spirit_of_the_howler_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_spirit_of_the_howler_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_spirit_of_wolf_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_spirit_of_wolf_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "spirit of wolf dropped"
     },
     "spell_spirit_of_wolf_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_splurt_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_splurt_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "splurt dropped"
     },
     "spell_splurt_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_stalking_probe_you_off": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_stalwart_regeneration_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_stalwart_regeneration_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_stamina_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "stamina dropped"
     },
     "spell_stamina_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_starfire_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_starfire_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_starshine_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_starshine_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_static_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_static_strike_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_static_strike_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_static_you_on": {
       "alert": {},
       "reaction": "group",
       "sound": "static"
     },
     "spell_steam_overload_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_steam_overload_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "steam overload dropped"
     },
     "spell_steam_overload_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_steelskin_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_steelskin_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_stone_breath_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_stone_breath_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_stream_of_acid_other_cast": {
       "alert": {},
       "reaction": "raid",
       "sound": "stream of acid"
     },
     "spell_stream_of_acid_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_stream_of_acid_you_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_stream_of_acid_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_strength_of_nature_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_strength_of_nature_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "strength of nature dropped"
     },
     "spell_strength_of_nature_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_strength_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_strike_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_strike_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_stun_breath_other_cast": {
       "alert": {},
       "reaction": "raid",
       "sound": "stun breath"
     },
     "spell_stun_breath_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_stun_breath_you_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_stun_breath_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_stunning_blow_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_stunning_blow_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_suffocating_sphere_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_suffocating_sphere_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "suffocating sphere dropped"
     },
     "spell_suffocating_sphere_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_summon_companion_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_summon_companion_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_summon_orb_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_summon_orb_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_summon_wisp_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_summon_wisp_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_sunbeam_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_sunbeam_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_sunstrike_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_sunstrike_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_swarm_of_retribution_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_swarm_of_retribution_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_swarming_pain_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_swarming_pain_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_sympathetic_aura_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_sympathetic_aura_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "sympathetic aura dropped"
     },
     "spell_sympathetic_aura_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_symphonic_harmony_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_system_shock_i_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_system_shock_v_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_syvelians_antimagic_aria_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_tainted_breath_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "tainted breath dropped"
     },
     "spell_talisman_of_jasinth_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_talisman_of_jasinth_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_talisman_of_shadoo_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_talisman_of_shadoo_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_talisman_of_the_brute_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "talisman of the brute dropped"
     },
     "spell_talisman_of_the_brute_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_talisman_of_the_cat_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "meow"
     },
     "spell_talisman_of_the_cat_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_talisman_of_the_raptor_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "talisman of the raptor dropped"
     },
     "spell_talisman_of_the_raptor_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_talisman_of_the_rhino_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "talisman of the rhino dropped"
     },
     "spell_talisman_of_the_rhino_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_talisman_of_the_serpent_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "talisman of the serpent dropped"
     },
     "spell_talisman_of_the_serpent_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_taper_enchantment_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_taper_enchantment_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_tarews_aquatic_ayre_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "tarews aquatic ayre dropped"
     },
     "spell_tarews_aquatic_ayre_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_tashan_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_tears_of_druzzil_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_tears_of_druzzil_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_tears_of_solusek_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_tears_of_solusek_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_telescope_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_telescope_you_off": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_telescope_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_the_dains_justice_other_on": {
       "alert": {},
       "reaction": "raid",
       "sound": "teleport"
     },
     "spell_the_dains_justice_you_on": {
       "alert": {},
       "reaction": "raid",
       "sound": "teleport"
     },
     "spell_the_unspoken_word_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_the_unspoken_word_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "the unspoken word dropped"
     },
     "spell_the_unspoken_word_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_theft_of_thought_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_thistlecoat_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_thistlecoat_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_thorncoat_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_thorncoat_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_thunder_strike_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_thunder_strike_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_thunderbold_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_thunderbold_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_thunderclap_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_thunderclap_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_torbas_acid_blast_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_torbas_acid_blast_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_torment_of_argli_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_torment_of_argli_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_torment_of_shadows_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_torment_of_shadows_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "torment of shadows dropped"
     },
     "spell_torment_of_shadows_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_torment_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_torment_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "torment dropped"
     },
     "spell_torment_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_torpor_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_torpor_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "torpor dropped"
     },
     "spell_torpor_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_torrent_of_poison_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_torrent_of_poison_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_touch_of_night_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_track_corpse_you_off": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_travelerboots_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_travelerboots_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "journeyman boots dropped"
     },
     "spell_travelerboots_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_tremor_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_trepidation_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_trepidation_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "trepidation dropped"
     },
     "spell_trepidation_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_true_north_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_tsunami_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_turning_of_the_unnatural_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_turning_of_the_unnatural_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "turning of the unnatural dropped"
     },
     "spell_turning_of_the_unnatural_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_umbra_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_umbra_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_unfailing_reverence_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_unfailing_reverence_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_upheaval_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_upheaval_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_valiant_companion_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_valor_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_valor_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "valor dropped"
     },
     "spell_valor_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_vengeance_of_alkabor_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_vengeance_of_alkabor_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_vengeance_of_the_glades_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_verlekarnorms_disaster_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_verlekarnorms_disaster_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_vexing_mordinia_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_vexing_mordinia_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "vexing mordinia dropped"
     },
     "spell_vexing_mordinia_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_vigilant_spirit_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_visions_of_grandeur_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_visions_of_grandeur_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "visions of the grandeur dropped"
     },
     "spell_visions_of_grandeur_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_voice_graft_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_voice_of_the_berserker_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_wake_of_karana_other_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_wake_of_karana_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_wandering_mind_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_wandering_mind_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "wandering mind dropped"
     },
     "spell_wandering_mind_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_wave_of_cold_you_on": {
       "alert": {},
       "reaction": "raid",
       "sound": "wave of cold"
     },
     "spell_wave_of_fire_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_wave_of_fire_you_on": {
       "alert": {},
       "reaction": "raid",
       "sound": "wave of fire"
     },
     "spell_wave_of_flame_other_cast": {
       "alert": {},
       "reaction": "raid",
       "sound": "wave of flame"
     },
     "spell_wave_of_flame_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_wave_of_healing_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_wave_of_healing_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_wave_of_heat_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_wave_of_heat_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_waves_of_the_deep_sea_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_whirlwind_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_whirlwind_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_wildfire_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_wildfire_you_on": {
       "alert": {},
       "reaction": "solo",
       "sound": "the druids are clearly upset"
     },
     "spell_winds_of_gelid_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_winds_of_gelid_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_winged_death_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_winged_death_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_wonderous_rapidity_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_wonderous_rapidity_you_on": {
       "alert": {},
       "reaction": "solo",
       "sound": "gotta go fast"
     },
     "spell_word_of_redemption:_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_word_of_redemption:_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_word_of_restoration_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_word_of_restoration_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_word_of_vigor_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_word_of_vigor_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_wrath_of_nature_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_wrath_of_nature_you_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "wrath of nature dropped"
     },
     "spell_wrath_of_nature_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_wrath_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_wrath_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_ykesha_other_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "spell_ykesha_you_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     }
   },
   "version": "%s"
 }
 """
 
     new_line_pets_config = """
 {
   "line": {
     "pet_attack": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "pet_back": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "pet_dead": {
       "alert": {},
       "reaction": "solo",
       "sound": "pet dead"
     },
     "pet_follow": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "pet_guard": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "pet_illegal_target": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "pet_sit_stand": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "pet_spawn": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "pet_taunt_off": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     }
   },
   "version": "%s"
 }
 """
 
     new_line_chat_recieved_npc_config = """
 {
   "line": {
     "say_npc": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "shout_npc": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "tell_npc": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "tell_npc_bank_closed": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "tell_npc_bank_open": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     }
   },
   "version": "%s"
 }
 """
 
     new_line_chat_recieved_config = """
 {
   "line": {
     "auction": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "auction_wtb": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "auction_wts": {
       "alert": {
-        "shiny brass idol": "true"
+        "shiny brass idol": true
       },
       "reaction": "alert",
       "sound": "look at auction"
     },
     "auction_unknown_tongue": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "broadcast": {
       "alert": {},
       "reaction": "solo",
-      "sound": "true"
+      "sound": true
     },
     "group": {
       "alert": {
         "drop": "raid",
         "help": "raid",
-        "inc": "true",
+        "inc": true,
         "invis": "raid",
         "invite": "raid",
-        "oom": "true"
+        "oom": true
       },
       "reaction": "alert",
       "sound": "look at group"
     },
     "guild": {
       "alert": {
         "assist": "raid",
         "bump": "raid",
         "crippled": "raid",
         "dispelled": "raid",
         "feared": "raid",
         "fixated": "raid",
         "fixation": "raid",
         "harmony": "raid",
-        "help": "true",
+        "help": true,
         "incoming": "raid",
         "logs": "raid",
         "malo": "raid",
         "malosini": "raid",
         "occlusion": "raid",
         "off-tanking": "raid",
         "pop": "raid",
@@ -17921,97 +18194,97 @@
         "tash": "raid"
       },
       "reaction": "alert",
       "sound": "look at guild"
     },
     "ooc": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "say": {
       "alert": {
-        "help": "true",
+        "help": true,
         "spot": "raid"
       },
       "reaction": "alert",
       "sound": "look at say"
     },
     "say_unknown_tongue": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "shout": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "shout_unknown_tongue": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "tell": {
       "alert": {},
       "reaction": "solo",
-      "sound": "true"
+      "sound": true
     },
     "tell_unknown_tongue": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     }
   },
   "version": "%s"
 }
 """
 
     new_line_chat_sent_config = """
 {
   "line": {
     "auction_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "group_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "guild_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "ooc_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "petition_you": {
       "alert": {},
       "reaction": "solo",
       "sound": "fingers crossed"
     },
     "say_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "shout_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "tell_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     }
   },
   "version": "%s"
 }
 """
 
     new_line_command_output_config = """
@@ -18025,231 +18298,231 @@
     "birthdate": {
       "alert": {},
       "reaction": "solo",
       "sound": "ah, the memories"
     },
     "client_ui_load": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "corpse_consent": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "command_block": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "command_block_casting": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "command_block_moving": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "command_block_spellbook": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "command_invalid": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "direction": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "direction_miss": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "drink_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "drink_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "drink_you_finish": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "eat_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "eat_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "eat_you_finish": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "eat_you_full": {
       "alert": {},
       "reaction": "solo",
       "sound": "I'm stuffed!"
     },
     "friend_add": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "friend_empty": {
       "alert": {},
       "reaction": "solo",
       "sound": "It's OK! I'll be your friend!"
     },
     "friend_list_header": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "friend_list_line": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "friend_list_total": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "friend_remove": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "forage_attacking": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "forage_cursor_empty": {
       "alert": {},
       "reaction": "solo",
       "sound": "remove items from cursor"
     },
     "forage_edible": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "forage_fail": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "forage_not_edible": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "forage_standing": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "help_command_chat": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "help_command_emote": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "help_command_format": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "help_command_guild": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "help_command_header": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "help_command_line": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "help_command_normal": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "help_command_output": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "help_command_voice": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "hide_corpse_all": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "hide_corpse_looted": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "hide_corpse_none": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "ignore_add": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "ignore_list_header": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "inspect_toggle_off": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "inspect_toggle_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "list_added": {
       "alert": {},
       "reaction": "solo",
       "sound": "good luck"
     },
     "list_leaving": {
@@ -18260,189 +18533,189 @@
     "list_leaving_zone": {
       "alert": {},
       "reaction": "solo",
       "sound": "Toto, I have a feeling we're not in Kansas anymore."
     },
     "list_none": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "list_out_of_range": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "list_position": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "list_removed_range": {
       "alert": {},
       "reaction": "solo",
       "sound": "removed from list"
     },
     "list_re_entered": {
       "alert": {},
       "reaction": "solo",
       "sound": "back in list area"
     },
     "location": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "motd_game": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "motd_guild": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "player_linkdead": {
       "alert": {},
       "reaction": "group",
-      "sound": "true"
+      "sound": true
     },
     "played_session": {
       "alert": {},
       "reaction": "solo",
-      "sound": "false"
+      "sound": false
     },
     "played_total": {
       "alert": {},
       "reaction": "solo",
-      "sound": "false"
+      "sound": false
     },
     "random": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "reply_empty": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "server_message": {
       "alert": {},
       "reaction": "all",
-      "sound": "true"
+      "sound": true
     },
     "skill_max": {
       "alert": {},
       "reaction": "solo",
       "sound": "the power!"
     },
     "skill_max_tradeskill": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "skill_up": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "summon_corpse": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "summon_corpse_no_consent": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "summon_corpse_none": {
       "alert": {},
       "reaction": "solo",
       "sound": "well thats a good thing, right?"
     },
     "summon_corpse_too_far": {
       "alert": {},
       "reaction": "solo",
       "sound": "too far"
     },
     "target": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "target_command_format": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "time_earth": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "time_game": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "you_afk_off": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "you_afk_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "you_camping": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "you_camping_abandoned": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "you_camping_standing": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "you_lfg_off": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "you_lfg_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     }
   },
   "version": "%s"
 }
 """
 
     new_line_system_messages_config = """
 {
   "line": {
     "achievement_first": {
       "alert": {},
       "reaction": "solo",
-      "sound": "true"
+      "sound": true
     },
     "anon_off": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "anon_on": {
       "alert": {},
       "reaction": "raid",
       "sound": "you must be up to no good!"
     },
     "assist_self": {
@@ -18463,256 +18736,256 @@
     "auto_inventory_full": {
       "alert": {},
       "reaction": "solo",
       "sound": "inventory full"
     },
     "autofollow_advice": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "autofollow_no_target": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "autofollow_off": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "autofollow_on": {
       "alert": {},
       "reaction": "solo",
       "sound": "onward my steed"
     },
     "bandage_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "bandage_cap": {
       "alert": {},
       "reaction": "solo",
       "sound": "bandage cap"
     },
     "boat_operator": {
       "alert": {},
       "reaction": "solo",
       "sound": "aye, aye, captain!"
     },
     "cast_animal_only": {
       "alert": {},
       "reaction": "solo",
-      "sound": "true"
+      "sound": true
     },
     "cast_change_form_block": {
       "alert": {},
       "reaction": "solo",
       "sound": "I can't do that here"
     },
     "cast_night_only": {
       "alert": {},
       "reaction": "solo",
-      "sound": "true"
+      "sound": true
     },
     "cast_outdoors_only": {
       "alert": {},
       "reaction": "solo",
-      "sound": "true"
+      "sound": true
     },
     "chat_disconnected": {
       "alert": {},
       "reaction": "solo",
       "sound": "chat disconnected"
     },
     "command_error": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "command_usage": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "concious_you": {
       "alert": {},
       "reaction": "solo",
       "sound": "you got this!"
     },
     "consider": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "consider_dead": {
       "alert": {},
       "reaction": "solo",
       "sound": "she's dead, jim"
     },
     "consider_no_target": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "container_container": {
       "alert": {},
       "reaction": "solo",
       "sound": "It's bigger on the inside"
     },
     "corpse_decay_timer": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "corpse_res_timer": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "corpse_too_old": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "dead_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "dead_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "ding_down": {
       "alert": {},
       "reaction": "all",
-      "sound": "true"
+      "sound": true
     },
     "ding_up": {
       "alert": {},
       "reaction": "all",
       "sound": "congratulations"
     },
     "drag_permission_received": {
       "alert": {},
       "reaction": "solo",
-      "sound": "true"
+      "sound": true
     },
     "duel_accept_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "duel_challenge": {
       "alert": {},
       "reaction": "solo",
       "sound": "Now witness the firepower of this fully ARMED and OPERATIONAL battle station!"
     },
     "duel_end_fled": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "earthquake": {
       "alert": {},
       "reaction": "solo",
       "sound": "earthquake!"
     },
     "effect_removal_block": {
       "alert": {},
       "reaction": "solo",
       "sound": "I'm sorry, Dave. I'm afraid I can't do that."
     },
     "encumbered_off": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "encumbered_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "engage": {
       "alert": {},
       "reaction": "all",
-      "sound": "true"
+      "sound": true
     },
     "equip_block": {
       "alert": {},
       "reaction": "solo",
       "sound": "I can't wear that"
     },
     "faction_line": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "fall_damage_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "fall_damage_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "feign_failure_other": {
       "alert": {},
       "reaction": "solo",
-      "sound": "true"
+      "sound": true
     },
     "fishing_cast": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "fishing_caught_nothing": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "fishing_caught_something": {
       "alert": {},
       "reaction": "solo",
       "sound": "yay"
     },
     "fishing_creatively": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "fishing_holding": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "fishing_lost_bait": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "fishing_no_pole": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "fishing_no_water": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "fishing_pole_broke": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "fishing_spill_beer": {
       "alert": {},
       "reaction": "solo",
       "sound": "not again!"
     },
     "gm_reset_ability": {
@@ -18723,51 +18996,51 @@
     "gm_reset_discipline": {
       "alert": {},
       "reaction": "solo",
       "sound": "Disciplines reset"
     },
     "hide_attacking": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "hide_disabled": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "hide_drop": {
       "alert": {},
       "reaction": "solo",
       "sound": "hide drop"
     },
     "hide_enabled": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "hide_moving": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "item_too_big": {
       "alert": {},
       "reaction": "solo",
       "sound": "thats too big"
     },
     "inspect_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "inspect_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "item_dropped": {
       "alert": {},
       "reaction": "solo",
       "sound": "item dropped"
     },
     "item_dropped_no_room": {
@@ -18778,66 +19051,66 @@
     "item_must_equip": {
       "alert": {},
       "reaction": "solo",
       "sound": "must equip"
     },
     "item_no_drop": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "jump_fatigue": {
       "alert": {},
       "reaction": "solo",
       "sound": "no stamina"
     },
     "lore_pickup": {
       "alert": {},
       "reaction": "solo",
       "sound": "I already have this"
     },
     "npc_guild_wrong": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "motd_welcome": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "required_pick": {
       "alert": {},
       "reaction": "solo",
       "sound": "let me in!"
     },
     "rewind_output": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "rewind_output_wait": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "roleplay_off": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "roleplay_on": {
       "alert": {},
       "reaction": "solo",
       "sound": "bravo six, going dark"
     },
     "target_attack_sitting": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "target_attack_too_far": {
       "alert": {},
       "reaction": "solo",
       "sound": "too far"
     },
     "target_cannot_see": {
@@ -18848,206 +19121,206 @@
     "target_group_member": {
       "alert": {},
       "reaction": "solo",
       "sound": "target group member"
     },
     "target_lost": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "tell_offline": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "tell_yourself": {
       "alert": {},
       "reaction": "solo",
-      "sound": "true"
+      "sound": true
     },
     "tell_queued_offline": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "titanium_client_help_message": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "too_many_pets": {
       "alert": {},
       "reaction": "solo",
       "sound": "You already have a pet"
     },
     "tracking": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "tracking_begin": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "tracking_player_off": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "tracking_player_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "tracking_target_lost": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "use_block": {
       "alert": {},
       "reaction": "solo",
       "sound": "I can't use that"
     },
     "walk_of_shame": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "warrior_berserk_off": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "warrior_berserk_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "weather_start_rain": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "weather_start_snow": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "wrong_key": {
       "alert": {},
       "reaction": "all",
       "sound": "wrong key or place"
     },
     "yell_help": {
       "alert": {},
       "reaction": "solo",
       "sound": "help"
     },
     "yell_help_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "you_auto_attack_off": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "you_auto_attack_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "you_cannot_reach": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "you_char_bound": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "you_hungry": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "you_lowdrink": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "you_lowfood": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "you_lowfoodlowdrink": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "you_new_zone": {
       "alert": {},
       "reaction": "all",
-      "sound": "true"
+      "sound": true
     },
     "you_outdrink": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "you_outdrinklowfood": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "you_outfood": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "you_outfooddrink": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "you_outfoodlowdrink": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "you_stun_off": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "you_stun_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "you_thirsty": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "zone_message": {
       "alert": {},
       "reaction": "all",
-      "sound": "true"
+      "sound": true
     },
     "zoning": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     }
   },
   "version": "%s"
 }
 """
 
     new_line_group_system_messages_config = """
@@ -19056,201 +19329,201 @@
     "group_alone": {
       "alert": {},
       "reaction": "solo",
       "sound": "is anyone there?"
     },
     "group_already": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "group_considering": {
       "alert": {},
       "reaction": "solo",
       "sound": "considering"
     },
     "group_created": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "group_disbanded": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "group_invite_already": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "group_invite_instruction": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "group_invite_not_lead": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "group_invite_npc": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "group_invite_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "group_invite_you": {
       "alert": {},
       "reaction": "solo",
-      "sound": "true"
+      "sound": true
     },
     "group_invite_yourself": {
       "alert": {},
       "reaction": "solo",
-      "sound": "true"
+      "sound": true
     },
     "group_invite_you_cancel": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "group_join_notify": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "group_join_reject": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "group_joined": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "group_joined_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "group_leader_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "group_leader_you": {
       "alert": {},
       "reaction": "group",
-      "sound": "true"
+      "sound": true
     },
     "group_leave_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "group_removed": {
       "alert": {},
       "reaction": "solo",
-      "sound": "true"
+      "sound": true
     },
     "group_removed_other": {
       "alert": {},
       "reaction": "solo",
-      "sound": "true"
+      "sound": true
     },
     "guild_invite_instructions": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "guild_invite_other_decline": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "guild_member_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "guild_member_other_accept": {
       "alert": {},
       "reaction": "solo",
       "sound": "welcome"
     },
     "guild_member_other_invite": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "guild_member_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "guild_member_you_accept": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "guild_motd_wrong_command": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "guild_officer_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "guild_officer_you": {
       "alert": {},
       "reaction": "solo",
       "sound": "movin on up"
     },
     "guild_remove_fail": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "guild_remove_you": {
       "alert": {},
       "reaction": "solo",
       "sound": "not like this"
     },
     "guild_remove_you_attempt": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "guild_status_instructions": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "guild_status_none": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "guild_status_officer": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "invite_no_target": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     }
   },
   "version": "%s"
 }
 """
 
     new_line_loot_trade_config = """
@@ -19284,61 +19557,61 @@
     "loot_wait": {
       "alert": {},
       "reaction": "solo",
       "sound": "can't loot"
     },
     "looted_item_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "looted_item_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "looted_money_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "looted_money_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "looted_money_you_split": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "split_format": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "split_format_example": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "split_invalid": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "split_off": {
       "alert": {},
       "reaction": "solo",
       "sound": "helping the monks"
     },
     "split_on": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "split_shared": {
       "alert": {},
       "reaction": "solo",
       "sound": "ka-ching"
     },
     "trade_error": {
@@ -19350,40 +19623,40 @@
       "alert": {},
       "reaction": "solo",
       "sound": "lore item in trade"
     },
     "tradeskill_create_other": {
       "alert": {},
       "reaction": "solo_group_only",
-      "sound": "false"
+      "sound": false
     },
     "tradeskill_create_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "tradeskill_fail_other": {
       "alert": {},
       "reaction": "solo_group_only",
-      "sound": "false"
+      "sound": false
     },
     "tradeskill_fail_you": {
       "alert": {},
       "reaction": "solo_group_only",
       "sound": "womp"
     },
     "tradeskill_hands_full": {
       "alert": {},
       "reaction": "solo",
       "sound": "empty cursor"
     },
     "tradeskill_skill_cap": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "tradeskill_wrong_container": {
       "alert": {},
       "reaction": "solo",
       "sound": "wrong container"
     },
     "trade_cancel_other": {
@@ -19399,41 +19672,41 @@
     "trade_interest": {
       "alert": {},
       "reaction": "solo",
       "sound": "let's trade"
     },
     "trade_item": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "trade_money": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "trade_money_add": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "trade_npc_item_price": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "trade_npc_item_sold": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "trade_npc_payment": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "trade_too_far": {
       "alert": {},
       "reaction": "solo",
       "sound": "too far"
     }
   },
@@ -19442,761 +19715,760 @@
 """
 
     new_line_emotes_config = """
 {
   "line": {
     "emote_agree_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_agree_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_amaze_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_apologize_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_bird_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_bird_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_bite_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_bite_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_bleed_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_bleed_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_blink_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_blush_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_blush_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_boggle_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_bonk_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_bonk_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_bored_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_bounce_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_bow_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_bow_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_brb_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_burp_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_burp_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_bye_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_bye_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_cackle_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_calm_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_cheer_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_cheer_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_chuckle_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_chuckle_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_clap_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_clap_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_comfort_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_comfort_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_congratulate_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_congratulate_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_cough_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_cringe_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_cry_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_cry_you": {
       "alert": {},
       "reaction": "solo",
       "sound": "there there"
     },
     "emote_curious_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_dance_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_dance_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_drool_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_duck_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_eye_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_fidget_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_flex_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_flex_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_frown_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_frown_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_gasp_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_gasp_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_giggle_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_giggle_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_glare_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_grin_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_grin_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_groan_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_grovel_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_happy_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_hug_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_hug_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_hungry_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_introduce_other": {
       "alert": {},
       "reaction": "all",
       "sound": "why, hello there"
     },
     "emote_introduce_you": {
       "alert": {},
       "reaction": "all",
       "sound": "why, hello there"
     },
     "emote_jk_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_kiss_other": {
       "alert": {},
       "reaction": "solo",
       "sound": "love is in the air"
     },
     "emote_kiss_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_kneel_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_kneel_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_laugh_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_laugh_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_lost_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_massage_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_moan_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_mourn_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_mourn_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_nod_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_nod_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_nudge_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_panic_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_pat_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_pat_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_peer_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_peer_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_plead_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_plead_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_point_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_point_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_poke_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_poke_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_ponder_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_ponder_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_purr_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_puzzle_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_raise_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_ready_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_roar_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_roar_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_rofl_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_rofl_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_salute_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_salute_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_shiver_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_shiver_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_shrug_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_shrug_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_sigh_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_sigh_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_smack_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_smile_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_smile_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_smirk_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_smirk_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_snarl_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_snicker_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_stare_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_tap_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_tap_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_tease_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_thank_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_thank_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_thirsty_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_veto_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_veto_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_wave_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_wave_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_whine_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_whistle_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_yawn_other": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "emote_yawn_you": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     }
   },
   "version": "%s"
 }
 """
 
     new_line_who_config = """
 {
   "line": {
     "who_etc": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "who_line": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "who_line_friends": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "who_player": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "who_top": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "who_top_friends": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "who_top_lfg": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "who_total": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "who_total_empty": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "who_total_local_empty": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     }
   },
   "version": "%s"
 }
 """
 
     new_line_other_config = """
 {
   "line": {
     "all": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
     "undetermined": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     }
   },
   "version": "%s"
 }
 """
 
     try:
         home = os.path.expanduser("~")
-        version = str(pkg_resources.get_distribution("eqalert").version)
         generated = False
 
         # Check for old config.yml
         legacy_config_json_path = base_path + "config.json"
         if os.path.isfile(legacy_config_json_path):
             json_data = open(legacy_config_json_path, "r", encoding="utf-8")
             legacy_config_json = json.load(json_data)
@@ -20214,15 +20486,15 @@
             os.rename(legacy_config_json_path, archive_config)
 
         # Generate Default Files if Needed
         ## Characters File
         characters_json_path = base_path + "config/characters.json"
         if not os.path.isfile(characters_json_path):
             f = open(characters_json_path, "w", encoding="utf-8")
-            f.write(new_char_config)
+            f.write(new_char_config % (version))
             f.close()
             generated = True
 
         ## Settings
         generated_settings = write_config(
             base_path, "settings", version, new_settings_config
         )
```

### Comparing `eqalert-3.5.0/eqa/lib/curses.py` & `eqalert-3.5.1/eqa/lib/curses.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,25 +19,24 @@
 """
 
 import curses
 import os
 import sys
 import time
 import math
-import pkg_resources
 import random
 import re
 from datetime import datetime
 
 import eqa.lib.struct as eqa_struct
 import eqa.lib.state as eqa_state
 import eqa.lib.settings as eqa_settings
 
 
-def display(stdscr, display_q, state, configs, exit_flag, cfg_reload):
+def display(stdscr, display_q, state, configs, exit_flag, cfg_reload, version):
     """
     Process: display_q
     Produce: display event
     """
     events = []
     debug_events = []
     page = "events"
@@ -86,14 +85,15 @@
                         state,
                         configs,
                         s_setting,
                         s_char,
                         s_opt,
                         s_line,
                         encounter_report,
+                        version,
                     )
 
                 ## Display Draw
                 elif display_event.type == "draw":
                     if display_event.screen == "help":
                         if page == "help":
                             page = last_page
@@ -110,14 +110,15 @@
                                 state,
                                 configs,
                                 s_setting,
                                 s_char,
                                 s_opt,
                                 s_line,
                                 encounter_report,
+                                version,
                             )
                     else:
                         page = display_event.screen
 
                     draw_page(
                         stdscr,
                         page,
@@ -126,14 +127,15 @@
                         state,
                         configs,
                         s_setting,
                         s_char,
                         s_opt,
                         s_line,
                         encounter_report,
+                        version,
                     )
 
                 ## Draw Update
                 elif display_event.type == "event":
                     if display_event.screen == "events":
                         events.append(display_event)
                         if page == "events":
@@ -145,14 +147,15 @@
                                 state,
                                 configs,
                                 s_setting,
                                 s_char,
                                 s_opt,
                                 s_line,
                                 encounter_report,
+                                version,
                             )
                     elif display_event.screen == "debug":
                         debug_events.append(display_event)
                         draw_page(
                             stdscr,
                             page,
                             events,
@@ -160,14 +163,15 @@
                             state,
                             configs,
                             s_setting,
                             s_char,
                             s_opt,
                             s_line,
                             encounter_report,
+                            version,
                         )
                     elif display_event.screen == "clear":
                         events = []
                         debug_events = []
                         draw_page(
                             stdscr,
                             page,
@@ -176,14 +180,15 @@
                             state,
                             configs,
                             s_setting,
                             s_char,
                             s_opt,
                             s_line,
                             encounter_report,
+                            version,
                         )
                 display_q.task_done()
 
     except Exception as e:
         eqa_settings.log(
             "display: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
@@ -202,40 +207,45 @@
     state,
     configs,
     s_setting,
     s_char,
     s_opt,
     s_line,
     encounter_report,
+    version,
 ):
     y, x = stdscr.getmaxyx()
     try:
         if x >= 80 and y >= 40:
             if page == "events":
-                draw_events_frame(stdscr, state, events, debug_events, encounter_report)
+                draw_events_frame(
+                    stdscr, state, events, debug_events, encounter_report, version
+                )
             elif page == "state":
-                draw_state(stdscr, state)
+                draw_state(stdscr, state, version)
             elif page == "settings":
-                draw_settings(stdscr, state, configs, s_setting, s_char, s_opt, s_line)
+                draw_settings(
+                    stdscr, state, configs, s_setting, s_char, s_opt, s_line, version
+                )
             elif page == "parse":
-                draw_parse(stdscr, state, encounter_report)
+                draw_parse(stdscr, state, encounter_report, version)
             elif page == "help":
                 draw_help(stdscr)
         else:
             draw_toosmall(stdscr)
     except Exception as e:
         eqa_settings.log(
             "draw_page: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
             + ": "
             + str(e)
         )
 
 
-def init(state):
+def init(state, version):
     try:
         """Create new stdscr in terminal"""
         stdscr = curses.initscr()
         os.system("setterm -cursor off")
         curses.start_color()
         curses.use_default_colors()
         curses.noecho()
@@ -244,15 +254,15 @@
         stdscr.timeout(100)
         curses.init_pair(1, curses.COLOR_WHITE, -1)  # Title
         curses.init_pair(2, curses.COLOR_YELLOW, -1)  # Header
         curses.init_pair(3, curses.COLOR_CYAN, -1)  # Subtext
         curses.init_pair(4, curses.COLOR_MAGENTA, -1)  # Highlight
         curses.init_pair(5, curses.COLOR_GREEN, -1)  # Dunno
         curses.init_pair(6, curses.COLOR_RED, -1)  # Dunno
-        draw_events_frame(stdscr, state, [], [], None)
+        draw_events_frame(stdscr, state, [], [], None, version)
         return stdscr
 
     except Exception as e:
         eqa_settings.log(
             "draw init: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
             + ": "
@@ -265,15 +275,15 @@
     os.system("setterm -cursor on")
     curses.nocbreak()
     stdscr.keypad(0)
     curses.echo()
     curses.endwin()
 
 
-def draw_tabs(stdscr, tab):
+def draw_tabs(stdscr, tab, version):
     """Draw top row tab selection"""
 
     try:
         y, x = stdscr.getmaxyx()
         center_y = int(y / 2)
         center_x = int(x / 2)
 
@@ -324,50 +334,49 @@
         else:
             stdscr.addstr(1, x - 10, "settings", curses.color_pair(2))
         stdscr.addch(0, x - 15, curses.ACS_TTEE)
         stdscr.addch(1, x - 15, curses.ACS_VLINE)
         stdscr.addch(2, x - 15, curses.ACS_BTEE)
 
         # Center title
-        version = str(pkg_resources.get_distribution("eqalert").version)
         offset = math.ceil(len(version) / 2)
         stdscr.addstr(
             1, center_x - 4 - offset, "EQ ALERT " + version, curses.color_pair(2)
         )
 
     except Exception as e:
         eqa_settings.log(
             "draw tabs: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
             + ": "
             + str(e)
         )
 
 
-def draw_events_frame(stdscr, state, events, debug_events, encounter_report):
+def draw_events_frame(stdscr, state, events, debug_events, encounter_report, version):
     """Draw events"""
 
     try:
         # Clear and box
         stdscr.clear()
         stdscr.box()
 
         # Draw tabs
-        draw_tabs(stdscr, "events")
+        draw_tabs(stdscr, "events", version)
 
         # Draw status
         draw_events_status_bar(stdscr, state)
 
         # Draw events panel
         draw_events(stdscr, events)
 
         # Draw lower panel
-        if state.debug == "true":
+        if state.debug:
             draw_events_debug(stdscr, debug_events)
-        elif state.encounter_parse == "true" and encounter_report is not None:
+        elif state.encounter_parse and encounter_report is not None:
             draw_events_encounter(stdscr, encounter_report)
         else:
             draw_events_default_lower(stdscr)
 
     except Exception as e:
         eqa_settings.log(
             "draw events frame: Error on line "
@@ -392,65 +401,65 @@
         for c in range(x - 2):
             stdscr.addch(center_y - 1, c + 1, curses.ACS_HLINE)
 
         ## Character
         stdscr.addstr(center_y, 2, state.char.title(), curses.color_pair(2))
 
         ## Guild
-        if state.char_guild != "unavailable":
+        if state.char_guild is not None:
             stdscr.addstr(
                 center_y,
                 3 + len(state.char),
                 state.char_guild.title(),
                 curses.color_pair(2),
             )
 
         ## Level
-        if state.char_level != "unavailable":
-            stdscr.addstr(center_y + 1, 2, state.char_level, curses.color_pair(2))
+        if state.char_level is not None:
+            stdscr.addstr(center_y + 1, 2, str(state.char_level), curses.color_pair(2))
 
         ## Class
-        if state.char_class != "unavailable":
+        if state.char_class is not None:
             stdscr.addstr(
                 center_y + 1,
-                3 + len(state.char_level),
+                3 + len(str(state.char_level)),
                 state.char_class.title(),
                 curses.color_pair(2),
             )
 
         ## Zone
-        if state.zone != "unavailable":
+        if state.zone is not None:
             stdscr.addstr(
                 center_y,
                 x - len(state.zone) - 2,
                 state.zone.title(),
                 curses.color_pair(2),
             )
 
         ## Direction
-        if state.direction != "unavailable":
+        if state.direction is not None:
             stdscr.addstr(
                 center_y + 1,
                 x - len(state.direction) - 2,
                 state.direction.title(),
                 curses.color_pair(2),
             )
 
         ## Location
         if state.loc != ["0.00", "0.00", "0.00"]:
-            if state.direction == "unavailable":
+            if state.direction is not None:
                 offset = (
-                    len(str(state.loc[0]))
+                    len(str(state.direction))
+                    + len(str(state.loc[0]))
                     + len(str(state.loc[1]))
                     + len(str(state.loc[2]))
                 )
             else:
                 offset = (
-                    len(state.direction)
-                    + len(str(state.loc[0]))
+                    len(str(state.loc[0]))
                     + len(str(state.loc[1]))
                     + len(str(state.loc[2]))
                 )
             stdscr.addstr(
                 center_y + 1,
                 x - offset - 7,
                 str(state.loc[0]) + ", " + str(state.loc[1]) + ", " + str(state.loc[2]),
@@ -458,22 +467,22 @@
             )
 
         ## Server
         offset = math.ceil(len(str(state.server)) / 2)
         stdscr.addstr(center_y, center_x - offset, state.server, curses.color_pair(2))
 
         ## Context
-        if state.afk == "true":
-            stdscr.addstr(center_y + 1, center_x - 1, "AFK", curses.color_pair(2))
-        elif state.group == "false" and state.raid == "false":
+        if not state.group and not state.raid:
             stdscr.addstr(center_y + 1, center_x - 2, "Solo", curses.color_pair(2))
-        elif state.group == "true" and state.raid == "false":
+        elif state.group and not state.raid:
             stdscr.addstr(center_y + 1, center_x - 3, "Group", curses.color_pair(2))
-        elif state.raid == "true":
+        elif state.raid:
             stdscr.addstr(center_y + 1, center_x - 2, "Raid", curses.color_pair(2))
+        elif state.afk:
+            stdscr.addstr(center_y + 1, center_x - 1, "AFK", curses.color_pair(2))
 
         ## Bottom of stats bar
         stdscr.addch(center_y + 2, 0, curses.ACS_LTEE)
         stdscr.addch(center_y + 2, x - 1, curses.ACS_RTEE)
         for c in range(x - 2):
             stdscr.addch(center_y + 2, c + 1, curses.ACS_HLINE)
 
@@ -904,24 +913,24 @@
             "draw ftime: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
             + ": "
             + str(e)
         )
 
 
-def draw_parse(stdscr, state, encounter_report):
+def draw_parse(stdscr, state, encounter_report, version):
     """Draw parse"""
     y, x = stdscr.getmaxyx()
 
     # Clear and box
     stdscr.clear()
     stdscr.box()
 
     # Draw tabs
-    draw_tabs(stdscr, "parse")
+    draw_tabs(stdscr, "parse", version)
 
     try:
         encounterscr = stdscr.derwin(int(y / 2) - 3, x - 2, 3, 1)
         encounterscr.clear()
         encounter_y, encounter_x = encounterscr.getmaxyx()
         center_y = int(encounter_y / 2)
         center_x = int(encounter_x / 2)
@@ -930,15 +939,15 @@
         first_third = int(encounter_x / 3)
         second_third = first_third + first_third
         playerscr = stdscr.derwin(int(y / 2) - 1, encounter_x, int(y / 2), 1)
         playerscr_y, playerscr_x = playerscr.getmaxyx()
         playerscr.clear()
 
         # If we're parsing encounters
-        if state.encounter_parse == "true":
+        if state.encounter_parse:
             ## If we have a report to show
             if encounter_report is not None:
                 target_name = encounter_report["target"]["name"].title()
 
                 # Target Line
                 underline = 3
                 while underline < (center_x - 2):
@@ -1121,26 +1130,26 @@
             "draw parse: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
             + ": "
             + str(e)
         )
 
 
-def draw_state(stdscr, state):
+def draw_state(stdscr, state, version):
     """Draw state"""
     y, x = stdscr.getmaxyx()
     center_y = int(y / 2)
     center_x = int(x / 2)
 
     # Clear and box
     stdscr.clear()
     stdscr.box()
 
     # Draw tabs
-    draw_tabs(stdscr, "state")
+    draw_tabs(stdscr, "state", version)
 
     # Show some state
     try:
         # server state
         stdscr.addstr(5, 5, "Server", curses.color_pair(2))
         stdscr.addstr(5, 16, ": ", curses.color_pair(1))
         stdscr.addstr(5, 18, state.server.title(), curses.color_pair(3))
@@ -1149,116 +1158,134 @@
         stdscr.addstr(6, 5, "Character", curses.color_pair(2))
         stdscr.addstr(6, 16, ": ", curses.color_pair(1))
         stdscr.addstr(6, 18, state.char.title(), curses.color_pair(3))
 
         # class
         stdscr.addstr(8, 5, "Class", curses.color_pair(2))
         stdscr.addstr(8, 16, ": ", curses.color_pair(1))
-        stdscr.addstr(8, 18, state.char_class.title(), curses.color_pair(3))
+        if state.char_class is not None:
+            stdscr.addstr(8, 18, state.char_class.title(), curses.color_pair(3))
+        else:
+            stdscr.addstr(8, 18, "Unavailable", curses.color_pair(3))
 
         # level
         stdscr.addstr(9, 5, "Level", curses.color_pair(2))
         stdscr.addstr(9, 16, ": ", curses.color_pair(1))
-        stdscr.addstr(9, 18, state.char_level.title(), curses.color_pair(3))
+        if state.char_level is not None:
+            stdscr.addstr(9, 18, str(state.char_level).title(), curses.color_pair(3))
+        else:
+            stdscr.addstr(9, 18, "Unavailable", curses.color_pair(3))
 
         # guild
         stdscr.addstr(10, 5, "Guild", curses.color_pair(2))
         stdscr.addstr(10, 16, ": ", curses.color_pair(1))
-        stdscr.addstr(10, 18, state.char_guild.title(), curses.color_pair(3))
+        if state.char_guild is not None:
+            stdscr.addstr(10, 18, state.char_guild.title(), curses.color_pair(3))
+        else:
+            stdscr.addstr(10, 18, "Unavailable", curses.color_pair(3))
 
         # bind state
         stdscr.addstr(12, 5, "Bind", curses.color_pair(2))
         stdscr.addstr(12, 16, ": ", curses.color_pair(1))
-        stdscr.addstr(12, 18, state.bind.title(), curses.color_pair(3))
+        if state.bind is not None:
+            stdscr.addstr(12, 18, state.bind.title(), curses.color_pair(3))
+        else:
+            stdscr.addstr(12, 18, "Unavailable", curses.color_pair(3))
 
         # encumbered state
         stdscr.addstr(13, 5, "Encumbered", curses.color_pair(2))
         stdscr.addstr(13, 16, ": ", curses.color_pair(1))
-        stdscr.addstr(13, 18, state.encumbered.title(), curses.color_pair(3))
+        stdscr.addstr(13, 18, str(state.encumbered), curses.color_pair(3))
 
         # afk state
         stdscr.addstr(14, 5, "AFK", curses.color_pair(2))
         stdscr.addstr(14, 16, ": ", curses.color_pair(1))
-        stdscr.addstr(14, 18, state.afk.title(), curses.color_pair(3))
+        stdscr.addstr(14, 18, str(state.afk), curses.color_pair(3))
 
         # group state
         stdscr.addstr(16, 5, "Group", curses.color_pair(2))
         stdscr.addstr(16, 16, ": ", curses.color_pair(1))
-        stdscr.addstr(16, 18, state.group.title(), curses.color_pair(3))
+        stdscr.addstr(16, 18, str(state.group), curses.color_pair(3))
 
         # leader state
-        if state.group == "true":
+        if state.group:
             stdscr.addstr(16, 25, "Leader", curses.color_pair(2))
             stdscr.addstr(16, 32, ": ", curses.color_pair(1))
-            stdscr.addstr(16, 34, state.leader.title(), curses.color_pair(3))
+            stdscr.addstr(16, 34, str(state.leader), curses.color_pair(3))
 
         # raid state
         stdscr.addstr(17, 5, "Raid", curses.color_pair(2))
         stdscr.addstr(17, 16, ": ", curses.color_pair(1))
-        stdscr.addstr(17, 18, state.raid.title(), curses.color_pair(3))
+        stdscr.addstr(17, 18, str(state.raid), curses.color_pair(3))
 
         # zone
         stdscr.addstr(19, 5, "Zone", curses.color_pair(2))
         stdscr.addstr(19, 16, ": ", curses.color_pair(1))
-        stdscr.addstr(19, 18, state.zone.title(), curses.color_pair(3))
+        if state.zone is not None:
+            stdscr.addstr(19, 18, state.zone.title(), curses.color_pair(3))
+        else:
+            stdscr.addstr(19, 18, "Unavailable", curses.color_pair(3))
 
         # loc
         stdscr.addstr(20, 5, "Location", curses.color_pair(2))
         stdscr.addstr(20, 16, ": ", curses.color_pair(1))
         stdscr.addstr(20, 18, str(state.loc[0]), curses.color_pair(3))
         stdscr.addstr(20, 24, " : ", curses.color_pair(2))
         stdscr.addstr(20, 26, str(state.loc[1]), curses.color_pair(3))
         stdscr.addstr(20, 32, " : ", curses.color_pair(2))
         stdscr.addstr(20, 34, str(state.loc[2]), curses.color_pair(3))
 
         # direction
         stdscr.addstr(21, 5, "Direction", curses.color_pair(2))
         stdscr.addstr(21, 16, ": ", curses.color_pair(1))
-        stdscr.addstr(21, 18, state.direction.title(), curses.color_pair(3))
+        if state.direction is not None:
+            stdscr.addstr(21, 18, state.direction.title(), curses.color_pair(3))
+        else:
+            stdscr.addstr(21, 18, "Unavailable", curses.color_pair(3))
 
         # debug state
         stdscr.addstr(23, 5, "Debug", curses.color_pair(2))
         stdscr.addstr(23, 16, ": ", curses.color_pair(1))
-        stdscr.addstr(23, 18, state.debug.title(), curses.color_pair(3))
+        stdscr.addstr(23, 18, str(state.debug), curses.color_pair(3))
 
         # mute state
         stdscr.addstr(24, 5, "Mute", curses.color_pair(2))
         stdscr.addstr(24, 16, ": ", curses.color_pair(1))
-        stdscr.addstr(24, 18, state.mute.title(), curses.color_pair(3))
+        stdscr.addstr(24, 18, str(state.mute), curses.color_pair(3))
 
         # enounter parse state
         stdscr.addstr(25, 5, "Encounter", curses.color_pair(2))
         stdscr.addstr(25, 16, ": ", curses.color_pair(1))
-        stdscr.addstr(25, 18, state.encounter_parse.title(), curses.color_pair(3))
+        stdscr.addstr(25, 18, str(state.encounter_parse), curses.color_pair(3))
 
         # consider evaluation state
         stdscr.addstr(26, 5, "Consider", curses.color_pair(2))
         stdscr.addstr(26, 16, ": ", curses.color_pair(1))
-        stdscr.addstr(26, 18, state.consider_eval.title(), curses.color_pair(3))
+        stdscr.addstr(26, 18, str(state.consider_eval), curses.color_pair(3))
 
     except Exception as e:
         eqa_settings.log(
             "draw state: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
             + ": "
             + str(e)
         )
 
 
-def draw_settings(stdscr, state, configs, s_setting, s_char, s_opt, s_line):
+def draw_settings(stdscr, state, configs, s_setting, s_char, s_opt, s_line, version):
     """Draw settings"""
 
     try:
         # Clear and box
         stdscr.clear()
         stdscr.box()
         y, x = stdscr.getmaxyx()
 
         # Draw tabs
-        draw_tabs(stdscr, "settings")
+        draw_tabs(stdscr, "settings", version)
 
         # Char Select Window
         charscr = stdscr.derwin(int(y / 2) - 4, int(x / 2) - 4, 4, 4)
         char_y, char_x = charscr.getmaxyx()
         charscr.box()
 
         ## Char Select Title
@@ -1366,56 +1393,81 @@
             charscr.addch(7, first_q + 3, curses.ACS_DARROW, curses.color_pair(2))
         else:
             charscr.addch(5, first_q + 3, curses.ACS_UARROW, curses.color_pair(2))
             charscr.addch(7, first_q + 3, curses.ACS_DARROW, curses.color_pair(2))
 
         # Character Select Stats
         charscr.addstr(10, first_q, "Class:", curses.color_pair(1))
+        selected_char_class = configs.characters.config["char_logs"][
+            state.chars[s_char]
+        ]["char_state"]["class"]
+        if selected_char_class is not None:
+            message = selected_char_class.title()
+        else:
+            message = "Unavailable"
         charscr.addstr(
             10,
             first_q + 7,
-            configs.characters.config["char_logs"][state.chars[s_char]]["char_state"][
-                "class"
-            ].title(),
+            message,
             curses.color_pair(3),
         )
         charscr.addstr(11, first_q, "Level:", curses.color_pair(1))
+        selected_char_level = configs.characters.config["char_logs"][
+            state.chars[s_char]
+        ]["char_state"]["level"]
+        if selected_char_level is not None:
+            message = str(selected_char_level)
+        else:
+            message = "Unavailable"
         charscr.addstr(
             11,
             first_q + 7,
-            configs.characters.config["char_logs"][state.chars[s_char]]["char_state"][
-                "level"
-            ],
+            message,
             curses.color_pair(3),
         )
         charscr.addstr(12, first_q, "Guild:", curses.color_pair(1))
+        selected_char_guild = configs.characters.config["char_logs"][
+            state.chars[s_char]
+        ]["char_state"]["guild"]
+        if selected_char_guild is not None:
+            message = selected_char_guild.title()
+        else:
+            message = "Unavailable"
         charscr.addstr(
             12,
             first_q + 7,
-            configs.characters.config["char_logs"][state.chars[s_char]]["char_state"][
-                "guild"
-            ].title(),
+            message,
             curses.color_pair(3),
         )
         charscr.addstr(13, first_q, "Zone:", curses.color_pair(1))
+        selected_char_zone = configs.characters.config["char_logs"][
+            state.chars[s_char]
+        ]["char_state"]["zone"]
+        if selected_char_zone is not None:
+            message = selected_char_zone.title()
+        else:
+            message = "Unavailable"
         charscr.addstr(
             13,
             first_q + 7,
-            configs.characters.config["char_logs"][state.chars[s_char]]["char_state"][
-                "zone"
-            ].title(),
+            message,
             curses.color_pair(3),
         )
         charscr.addstr(14, first_q, "Bind:", curses.color_pair(1))
+        selected_char_bind = configs.characters.config["char_logs"][
+            state.chars[s_char]
+        ]["char_state"]["bind"]
+        if selected_char_bind is not None:
+            message = selected_char_bind.title()
+        else:
+            message = "Unavailable"
         charscr.addstr(
             14,
             first_q + 7,
-            configs.characters.config["char_logs"][state.chars[s_char]]["char_state"][
-                "bind"
-            ].title(),
+            message,
             curses.color_pair(3),
         )
 
     except Exception as e:
         eqa_settings.log(
             "draw settings char select: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
@@ -1440,45 +1492,45 @@
                 first_q - 2,
                 "Log and display all parser output",
                 curses.color_pair(3),
             )
         else:
             optscr.addstr(5, first_q, "Debug Mode", curses.color_pair(1))
         optscr.addstr(5, second_third, "[", curses.color_pair(3))
-        if state.debug == "true":
+        if state.debug:
             optscr.addstr(5, second_third + 1, "on", curses.color_pair(5))
-        elif state.debug == "false":
+        else:
             optscr.addstr(5, second_third + 4, "off", curses.color_pair(6))
         optscr.addstr(5, second_third + 7, "]", curses.color_pair(3))
 
         # Mute
         if s_option == "mute" and s_setting == "option":
             optscr.addstr(6, first_q - 1, "Mute", curses.color_pair(4))
             optscr.addstr(2, first_q - 2, "Mute all audio alerts", curses.color_pair(3))
         else:
             optscr.addstr(6, first_q, "Mute", curses.color_pair(1))
         optscr.addstr(6, second_third, "[", curses.color_pair(3))
-        if state.mute == "true":
+        if state.mute:
             optscr.addstr(6, second_third + 1, "on", curses.color_pair(5))
-        elif state.mute == "false":
+        else:
             optscr.addstr(6, second_third + 4, "off", curses.color_pair(6))
         optscr.addstr(6, second_third + 7, "]", curses.color_pair(3))
 
         # Raid
         if s_option == "raid" and s_setting == "option":
             optscr.addstr(7, first_q - 1, "Raid Mode", curses.color_pair(4))
             optscr.addstr(
                 2, first_q - 2, "Manually toggle raid context", curses.color_pair(3)
             )
         else:
             optscr.addstr(7, first_q, "Raid Mode", curses.color_pair(1))
         optscr.addstr(7, second_third, "[", curses.color_pair(3))
-        if state.raid == "true":
+        if state.raid:
             optscr.addstr(7, second_third + 1, "on", curses.color_pair(5))
-        elif state.raid == "false":
+        else:
             optscr.addstr(7, second_third + 4, "off", curses.color_pair(6))
         optscr.addstr(7, second_third + 7, "]", curses.color_pair(3))
 
         # Raid Auto
         if s_option == "autoraid" and s_setting == "option":
             optscr.addstr(8, first_q - 1, "Auto-set Raid Mode", curses.color_pair(4))
             optscr.addstr(
@@ -1486,17 +1538,17 @@
                 first_q - 2,
                 "Automatically set raid context by zone",
                 curses.color_pair(3),
             )
         else:
             optscr.addstr(8, first_q, "Auto-set Raid Mode", curses.color_pair(1))
         optscr.addstr(8, second_third, "[", curses.color_pair(3))
-        if state.auto_raid == "true":
+        if state.auto_raid:
             optscr.addstr(8, second_third + 1, "on", curses.color_pair(5))
-        elif state.auto_raid == "false":
+        else:
             optscr.addstr(8, second_third + 4, "off", curses.color_pair(6))
         optscr.addstr(8, second_third + 7, "]", curses.color_pair(3))
 
         # Encounter
         if s_option == "encounter" and s_setting == "option":
             optscr.addstr(9, first_q - 1, "Encounter Parse", curses.color_pair(4))
             optscr.addstr(
@@ -1504,17 +1556,17 @@
                 first_q - 2,
                 "Automatically parse combat encounters",
                 curses.color_pair(3),
             )
         else:
             optscr.addstr(9, first_q, "Encounter Parse", curses.color_pair(1))
         optscr.addstr(9, second_third, "[", curses.color_pair(3))
-        if state.encounter_parse == "true":
+        if state.encounter_parse:
             optscr.addstr(9, second_third + 1, "on", curses.color_pair(5))
-        elif state.encounter_parse == "false":
+        else:
             optscr.addstr(9, second_third + 4, "off", curses.color_pair(6))
         optscr.addstr(9, second_third + 7, "]", curses.color_pair(3))
 
         # Encounter Save
         if s_option == "saveencounter" and s_setting == "option":
             optscr.addstr(10, first_q - 1, "Save Encounter Parse", curses.color_pair(4))
             optscr.addstr(
@@ -1522,17 +1574,17 @@
                 first_q - 2,
                 "Save combat encounters to a .json file",
                 curses.color_pair(3),
             )
         else:
             optscr.addstr(10, first_q, "Save Encounter Parse", curses.color_pair(1))
         optscr.addstr(10, second_third, "[", curses.color_pair(3))
-        if state.save_parse == "true":
+        if state.save_parse:
             optscr.addstr(10, second_third + 1, "on", curses.color_pair(5))
-        elif state.save_parse == "false":
+        else:
             optscr.addstr(10, second_third + 4, "off", curses.color_pair(6))
         optscr.addstr(10, second_third + 7, "]", curses.color_pair(3))
 
         # Default Timer
         if s_option == "defaulttimer" and s_setting == "option":
             optscr.addstr(
                 11, first_q - 1, "Auto-set Respawn Timer", curses.color_pair(4)
@@ -1542,17 +1594,17 @@
                 first_q - 2,
                 "Automatically set mob respawn timers",
                 curses.color_pair(3),
             )
         else:
             optscr.addstr(11, first_q, "Auto-set Respawn Timer", curses.color_pair(1))
         optscr.addstr(11, second_third, "[", curses.color_pair(3))
-        if state.auto_mob_timer == "true":
+        if state.auto_mob_timer:
             optscr.addstr(11, second_third + 1, "on", curses.color_pair(5))
-        elif state.auto_mob_timer == "false":
+        else:
             optscr.addstr(11, second_third + 4, "off", curses.color_pair(6))
         optscr.addstr(11, second_third + 7, "]", curses.color_pair(3))
 
         # Consider
         if s_option == "consider" and s_setting == "option":
             optscr.addstr(12, first_q - 1, "Consider Evaluation", curses.color_pair(4))
             optscr.addstr(
@@ -1560,17 +1612,17 @@
                 first_q - 2,
                 "Evaluate mob consider output",
                 curses.color_pair(3),
             )
         else:
             optscr.addstr(12, first_q, "Consider Evaluation", curses.color_pair(1))
         optscr.addstr(12, second_third, "[", curses.color_pair(3))
-        if state.consider_eval == "true":
+        if state.consider_eval:
             optscr.addstr(12, second_third + 1, "on", curses.color_pair(5))
-        elif state.consider_eval == "false":
+        else:
             optscr.addstr(12, second_third + 4, "off", curses.color_pair(6))
         optscr.addstr(12, second_third + 7, "]", curses.color_pair(3))
 
         # Detect Character
         if s_option == "detect_char" and s_setting == "option":
             optscr.addstr(
                 13, first_q - 1, "Auto-Detect Character", curses.color_pair(4)
@@ -1580,17 +1632,17 @@
                 first_q - 2,
                 "Automatically detect character log",
                 curses.color_pair(3),
             )
         else:
             optscr.addstr(13, first_q, "Auto-Detect Character", curses.color_pair(1))
         optscr.addstr(13, second_third, "[", curses.color_pair(3))
-        if state.detect_char == "true":
+        if state.detect_char:
             optscr.addstr(13, second_third + 1, "on", curses.color_pair(5))
-        elif state.detect_char == "false":
+        else:
             optscr.addstr(13, second_third + 4, "off", curses.color_pair(6))
         optscr.addstr(13, second_third + 7, "]", curses.color_pair(3))
 
         # Spell Timer Self
         if s_option == "spell_self" and s_setting == "option":
             optscr.addstr(14, first_q - 1, "Self Spell Timers", curses.color_pair(4))
             optscr.addstr(
@@ -1598,17 +1650,17 @@
                 first_q - 2,
                 "Spells targetting you",
                 curses.color_pair(3),
             )
         else:
             optscr.addstr(14, first_q, "Self Spell Timers", curses.color_pair(1))
         optscr.addstr(14, second_third, "[", curses.color_pair(3))
-        if state.spell_timer_self == "true":
+        if state.spell_timer_self:
             optscr.addstr(14, second_third + 1, "on", curses.color_pair(5))
-        elif state.spell_timer_self == "false":
+        else:
             optscr.addstr(14, second_third + 4, "off", curses.color_pair(6))
         optscr.addstr(14, second_third + 7, "]", curses.color_pair(3))
 
         # Spell Timer Other
         if s_option == "spell_other" and s_setting == "option":
             optscr.addstr(15, first_q - 1, "Other Spell Timers", curses.color_pair(4))
             optscr.addstr(
@@ -1616,17 +1668,17 @@
                 first_q - 2,
                 "Spells targetting others",
                 curses.color_pair(3),
             )
         else:
             optscr.addstr(15, first_q, "Other Spell Timers", curses.color_pair(1))
         optscr.addstr(15, second_third, "[", curses.color_pair(3))
-        if state.spell_timer_other == "true":
+        if state.spell_timer_other:
             optscr.addstr(15, second_third + 1, "on", curses.color_pair(5))
-        elif state.spell_timer_other == "false":
+        else:
             optscr.addstr(15, second_third + 4, "off", curses.color_pair(6))
         optscr.addstr(15, second_third + 7, "]", curses.color_pair(3))
 
         # Spell Timer Guild Only
         if s_option == "spell_guild" and s_setting == "option":
             optscr.addstr(16, first_q - 1, "Guild Timer Filter", curses.color_pair(4))
             optscr.addstr(
@@ -1634,17 +1686,17 @@
                 first_q - 2,
                 "Filter for spells on guildies",
                 curses.color_pair(3),
             )
         else:
             optscr.addstr(16, first_q, "Guild Timer Filter", curses.color_pair(1))
         optscr.addstr(16, second_third, "[", curses.color_pair(3))
-        if state.spell_timer_guild_only == "true":
+        if state.spell_timer_guild_only:
             optscr.addstr(16, second_third + 1, "on", curses.color_pair(5))
-        elif state.spell_timer_guild_only == "false":
+        else:
             optscr.addstr(16, second_third + 4, "off", curses.color_pair(6))
         optscr.addstr(16, second_third + 7, "]", curses.color_pair(3))
 
         # Spell Timer Guessing
         if s_option == "spell_guess" and s_setting == "option":
             optscr.addstr(17, first_q - 1, "Guess Spells", curses.color_pair(4))
             optscr.addstr(
@@ -1652,17 +1704,17 @@
                 first_q - 2,
                 "Make a guess instead of nothing",
                 curses.color_pair(3),
             )
         else:
             optscr.addstr(17, first_q, "Guess Spells", curses.color_pair(1))
         optscr.addstr(17, second_third, "[", curses.color_pair(3))
-        if state.spell_timer_guess == "true":
+        if state.spell_timer_guess:
             optscr.addstr(17, second_third + 1, "on", curses.color_pair(5))
-        elif state.spell_timer_guess == "false":
+        else:
             optscr.addstr(17, second_third + 4, "off", curses.color_pair(6))
         optscr.addstr(17, second_third + 7, "]", curses.color_pair(3))
 
         # Spell Timer Yours Only
         if s_option == "spell_yours" and s_setting == "option":
             optscr.addstr(18, first_q - 1, "Your Timer Filter", curses.color_pair(4))
             optscr.addstr(
@@ -1670,17 +1722,17 @@
                 first_q - 2,
                 "Filter for only your spells",
                 curses.color_pair(3),
             )
         else:
             optscr.addstr(18, first_q, "Your Timer Filter", curses.color_pair(1))
         optscr.addstr(18, second_third, "[", curses.color_pair(3))
-        if state.spell_timer_yours_only == "true":
+        if state.spell_timer_yours_only:
             optscr.addstr(18, second_third + 1, "on", curses.color_pair(5))
-        elif state.spell_timer_yours_only == "false":
+        else:
             optscr.addstr(18, second_third + 4, "off", curses.color_pair(6))
         optscr.addstr(18, second_third + 7, "]", curses.color_pair(3))
 
     except Exception as e:
         eqa_settings.log(
             "draw settings options: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
```

### Comparing `eqalert-3.5.0/eqa/lib/encounter.py` & `eqalert-3.5.1/eqa/lib/encounter.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,22 +23,29 @@
 import re
 import sys
 import time
 import os
 import json
 from datetime import datetime
 from collections import deque
-import pkg_resources
 
 import eqa.lib.settings as eqa_settings
 import eqa.lib.struct as eqa_struct
 
 
 def process(
-    configs, base_path, encounter_q, system_q, display_q, exit_flag, cfg_reload, state
+    configs,
+    base_path,
+    encounter_q,
+    system_q,
+    display_q,
+    exit_flag,
+    cfg_reload,
+    state,
+    version,
 ):
     """
     Process: encounter_q
     Produce: display_q, system_q, files
     """
 
     encounter_stack = deque([])
@@ -70,15 +77,18 @@
                         interaction == "combat"
                         or line_type == "spell_damage"
                         or line_type == "spell_resist_you"
                         or line_type == "you_auto_attack_on"
                     ):
                         #### Set active encounter
                         active_encounter = True
-                        encounter_zone = re.sub(r"[^\w\s]", "", state.zone)
+                        if state.zone is not None:
+                            encounter_zone = re.sub(r"[^\w\s]", "", state.zone)
+                        else:
+                            encounter_zone = re.sub(r"[^\w\s]", "", "Unavailable")
                 ## Or if active encounter
                 else:
                     ### And we see a line that indicates an encounter ends
                     if interaction == "stop":
                         #### Disable active encounter
                         active_encounter = False
                         #### Generate combat report and reset encounter stack
@@ -92,14 +102,15 @@
                                     line_time,
                                     line,
                                     encounter_stack,
                                     state,
                                     configs,
                                     display_q,
                                     encounter_zone,
+                                    version,
                                 )
                             else:
                                 encounter_stack.append(
                                     (
                                         line_time,
                                         source.title(),
                                         target.title(),
@@ -113,14 +124,15 @@
                                 line_time,
                                 line,
                                 encounter_stack,
                                 state,
                                 configs,
                                 display_q,
                                 encounter_zone,
+                                version,
                             )
 
                     if line_type == "you_new_zone":
                         encounter_stack.clear()
 
                     elif interaction == "end":
                         encounter_analysis(
@@ -128,20 +140,24 @@
                             line_time,
                             line,
                             encounter_stack,
                             state,
                             configs,
                             display_q,
                             encounter_zone,
+                            version,
                         )
 
                     elif interaction == "start":
                         #### Set active encounter
                         active_encounter = True
-                        encounter_zone = re.sub(r"[^\w\s]", "", state.zone)
+                        if state.zone is not None:
+                            encounter_zone = re.sub(r"[^\w\s]", "", state.zone)
+                        else:
+                            encounter_zone = re.sub(r"[^\w\s]", "", "Unavailable")
 
                 ## If we're in an encounter
                 if active_encounter == True:
                     ### Add combat or spell events to the stack
                     if interaction == "combat":
                         encounter_combat(
                             line_type, line_time, line, encounter_stack, state
@@ -1094,15 +1110,15 @@
             and target is not None
             and mode is not None
             and result is not None
         ):
             encounter_stack.append(
                 (line_time, source.title(), target.title(), mode, result)
             )
-        elif state.debug == "true":
+        elif state.debug:
             eqa_settings.log(
                 "encounter combat ["
                 + line_type
                 + "] not added to encounter stack: "
                 + line
             )
 
@@ -1225,15 +1241,15 @@
             and target is not None
             and mode is not None
             and result is not None
         ):
             encounter_stack.append(
                 (line_time, source.title(), target.title(), mode, result)
             )
-        elif state.debug == "true":
+        elif state.debug:
             eqa_settings.log(
                 "encounter spell ["
                 + line_type
                 + "] not added to encounter stack: "
                 + line
             )
 
@@ -1251,14 +1267,15 @@
     line_time,
     line,
     encounter_stack,
     state,
     configs,
     display_q,
     encounter_zone,
+    version,
 ):
     """Analyze encounter stack before reporting"""
 
     try:
         ## Uncommenting this will print the contents of the encounter stack, update the path
         # import time
 
@@ -1398,16 +1415,17 @@
                 encounter_target,
                 encounter_duration,
                 encounter_stack,
                 state,
                 configs,
                 display_q,
                 encounter_zone,
+                version,
             )
-        elif state.debug == "true":
+        elif state.debug:
             eqa_settings.log("Encounter Report: Unable to determine encounter target")
 
         # Prune old events
         if encounter_end_time is not None:
             prune_encounter_stack(encounter_end_time, encounter_stack)
 
     except Exception as e:
@@ -1423,14 +1441,15 @@
     encounter_target,
     encounter_duration,
     encounter_stack,
     state,
     configs,
     display_q,
     encounter_zone,
+    version,
 ):
     """Report encounter stats"""
 
     try:
         this_encounter = deque([])
         not_this_encounter = deque([])
 
@@ -1660,32 +1679,30 @@
         ### Encounter Summary
         encounter_report = {
             "header": {},
             "encounter_summary": {},
             "target": {},
             "participants": {},
         }
-        encounter_report["header"]["version"] = str(
-            pkg_resources.get_distribution("eqalert").version
-        )
+        encounter_report["header"]["version"] = version
         encounter_report["header"]["date"] = str(encounter_parse_date)
         encounter_report["header"]["time"] = str(encounter_parse_time)
         encounter_report["encounter_summary"]["character"] = str(state.char)
         encounter_report["encounter_summary"]["server"] = str(state.server)
         encounter_report["encounter_summary"]["zone"] = str(encounter_zone)
         if state.loc != ["0.00", "0.00", "0.00"]:
             encounter_report["encounter_summary"]["location"] = str(state.loc)
-        if state.afk == "true":
-            encounter_report["encounter_summary"]["context"] = "afk"
-        elif state.group == "false" and state.raid == "false":
+        if not state.group and not state.raid:
             encounter_report["encounter_summary"]["context"] = "solo"
-        elif state.group == "true" and state.raid == "false":
+        elif state.group and not state.raid:
             encounter_report["encounter_summary"]["context"] = "group"
-        elif state.group == "true" and state.raid == "true":
+        elif state.group and state.raid:
             encounter_report["encounter_summary"]["context"] = "raid"
+        elif state.afk:
+            encounter_report["encounter_summary"]["context"] = "afk"
         encounter_report["encounter_summary"]["target"] = str(encounter_target)
         encounter_report["encounter_summary"]["total_events"] = str(
             this_encounter_events
         )
         encounter_report["encounter_summary"]["duration"] = str(encounter_duration)
         if pet_and_target_same:
             encounter_report["encounter_summary"][
@@ -1892,18 +1909,15 @@
         display_q.put(
             eqa_struct.display(
                 eqa_settings.eqa_time(), "update", "encounter", encounter_report
             )
         )
 
         ## Write Encounter to File
-        if (
-            configs.settings.config["settings"]["encounter_parsing"]["auto_save"]
-            == "true"
-        ):
+        if configs.settings.config["settings"]["encounter_parsing"]["auto_save"]:
             encounter_report_json_string = json.dumps(encounter_report, indent=2)
             encounter_report_file = open(
                 encounter_zone_date_path + encounter_filename, "w"
             )
             encounter_report_file.write(encounter_report_json_string)
             encounter_report_file.close()
```

### Comparing `eqalert-3.5.0/eqa/lib/keys.py` & `eqalert-3.5.1/eqa/lib/keys.py`

 * *Files 24% similar despite different names*

```diff
@@ -64,152 +64,152 @@
                 if key == ord("q") or key == 27:
                     exit_flag.set()
 
                 ## Handle resize event
                 if key == curses.KEY_RESIZE:
                     display_q.put(
                         eqa_struct.display(
-                            eqa_settings.eqa_time(), "draw", "redraw", "null"
+                            eqa_settings.eqa_time(), "draw", "redraw", None
                         )
                     )
 
                 ## Handle tab keys
                 if key == ord("1"):
                     display_q.put(
                         eqa_struct.display(
-                            eqa_settings.eqa_time(), "draw", "events", "null"
+                            eqa_settings.eqa_time(), "draw", "events", None
                         )
                     )
                     page = "events"
                 elif key == ord("2"):
                     display_q.put(
                         eqa_struct.display(
-                            eqa_settings.eqa_time(), "draw", "state", "null"
+                            eqa_settings.eqa_time(), "draw", "state", None
                         )
                     )
                     page = "state"
                 elif key == ord("3"):
                     display_q.put(
                         eqa_struct.display(
-                            eqa_settings.eqa_time(), "draw", "parse", "null"
+                            eqa_settings.eqa_time(), "draw", "parse", None
                         )
                     )
                     page = "parse"
                 elif key == ord("4"):
                     display_q.put(
                         eqa_struct.display(
-                            eqa_settings.eqa_time(), "draw", "settings", "null"
+                            eqa_settings.eqa_time(), "draw", "settings", None
                         )
                     )
                     page = "settings"
                 elif key == ord("h"):
                     display_q.put(
                         eqa_struct.display(
-                            eqa_settings.eqa_time(), "draw", "help", "null"
+                            eqa_settings.eqa_time(), "draw", "help", None
                         )
                     )
                 elif key == ord("0"):
                     system_q.put(
                         eqa_struct.message(
                             eqa_settings.eqa_time(),
                             "system",
                             "reload_config",
-                            "null",
-                            "null",
+                            None,
+                            None,
                         )
                     )
 
                 ## Events keys
                 if page == "events":
                     if key == ord("c"):
                         display_q.put(
                             eqa_struct.display(
-                                eqa_settings.eqa_time(), "event", "clear", "null"
+                                eqa_settings.eqa_time(), "event", "clear", None
                             )
                         )
                     elif key == ord("r"):
                         system_q.put(
                             eqa_struct.message(
                                 eqa_settings.eqa_time(),
                                 "system",
                                 "raid",
                                 "toggle",
-                                "null",
+                                None,
                             )
                         )
                     elif key == ord("d"):
                         system_q.put(
                             eqa_struct.message(
                                 eqa_settings.eqa_time(),
                                 "system",
                                 "debug",
                                 "toggle",
-                                "null",
+                                None,
                             )
                         )
                     elif key == ord("e"):
                         system_q.put(
                             eqa_struct.message(
                                 eqa_settings.eqa_time(),
                                 "system",
                                 "encounter",
                                 "toggle",
-                                "null",
+                                None,
                             )
                         )
                     elif key == ord("m"):
                         system_q.put(
                             eqa_struct.message(
                                 eqa_settings.eqa_time(),
                                 "system",
                                 "mute",
                                 "toggle",
                                 "all",
                             )
                         )
                     elif key == ord("t"):
-                        if state.auto_mob_timer == "false":
+                        if not state.auto_mob_timer:
                             system_q.put(
                                 eqa_struct.message(
                                     eqa_settings.eqa_time(),
                                     "system",
                                     "timer",
                                     "mob",
-                                    "true",
+                                    True,
                                 )
                             )
-                        elif state.auto_mob_timer == "true":
+                        else:
                             system_q.put(
                                 eqa_struct.message(
                                     eqa_settings.eqa_time(),
                                     "system",
                                     "timer",
                                     "mob",
-                                    "false",
+                                    False,
                                 )
                             )
                     elif key == ord("p"):
-                        if state.save_parse == "false":
+                        if not state.save_parse:
                             system_q.put(
                                 eqa_struct.message(
                                     eqa_settings.eqa_time(),
                                     "system",
                                     "encounter",
                                     "save",
-                                    "true",
+                                    True,
                                 )
                             )
-                        elif state.save_parse == "true":
+                        else:
                             system_q.put(
                                 eqa_struct.message(
                                     eqa_settings.eqa_time(),
                                     "system",
                                     "encounter",
                                     "save",
-                                    "false",
+                                    False,
                                 )
                             )
 
                 ## State keys
                 elif page == "state":
                     pass
 
@@ -240,15 +240,15 @@
                                 )
                         elif key == ord("\n") or key == ord(" "):
                             system_q.put(
                                 eqa_struct.message(
                                     eqa_settings.eqa_time(),
                                     "system",
                                     "new_character",
-                                    "null",
+                                    None,
                                     chars[selected_char],
                                 )
                             )
                         elif key == ord("\t") or key == ord("`"):
                             settings = "option"
                             display_q.put(
                                 eqa_struct.display(
@@ -331,346 +331,307 @@
                                     eqa_settings.eqa_time(),
                                     "update",
                                     "option",
                                     option,
                                 )
                             )
                         elif key == curses.KEY_RIGHT or key == ord("d"):
-                            if option == "debug" and state.debug == "true":
+                            if option == "debug" and state.debug:
                                 system_q.put(
                                     eqa_struct.message(
                                         eqa_settings.eqa_time(),
                                         "system",
                                         "debug",
                                         "toggle",
-                                        "null",
+                                        None,
                                     )
                                 )
-                            elif option == "mute" and state.mute == "true":
+                            elif option == "mute" and state.mute:
                                 system_q.put(
                                     eqa_struct.message(
                                         eqa_settings.eqa_time(),
                                         "system",
                                         "mute",
                                         "toggle",
                                         "all",
                                     )
                                 )
-                            elif option == "raid" and state.raid == "true":
+                            elif option == "raid" and state.raid:
                                 system_q.put(
                                     eqa_struct.message(
                                         eqa_settings.eqa_time(),
                                         "system",
                                         "raid",
                                         "toggle",
-                                        "null",
+                                        None,
                                     )
                                 )
-                            elif option == "autoraid" and state.auto_raid == "true":
+                            elif option == "autoraid" and state.auto_raid:
                                 system_q.put(
                                     eqa_struct.message(
                                         eqa_settings.eqa_time(),
                                         "system",
                                         "raid",
                                         "auto",
-                                        "false",
+                                        False,
                                     )
                                 )
-                            elif (
-                                option == "encounter"
-                                and state.encounter_parse == "true"
-                            ):
+                            elif option == "encounter" and state.encounter_parse:
                                 system_q.put(
                                     eqa_struct.message(
                                         eqa_settings.eqa_time(),
                                         "system",
                                         "encounter",
                                         "toggle",
-                                        "null",
+                                        None,
                                     )
                                 )
-                            elif (
-                                option == "saveencounter" and state.save_parse == "true"
-                            ):
+                            elif option == "saveencounter" and state.save_parse:
                                 system_q.put(
                                     eqa_struct.message(
                                         eqa_settings.eqa_time(),
                                         "system",
                                         "encounter",
                                         "save",
-                                        "false",
+                                        False,
                                     )
                                 )
-                            elif (
-                                option == "defaulttimer"
-                                and state.auto_mob_timer == "true"
-                            ):
+                            elif option == "defaulttimer" and state.auto_mob_timer:
                                 system_q.put(
                                     eqa_struct.message(
                                         eqa_settings.eqa_time(),
                                         "system",
                                         "timer",
                                         "mob",
-                                        "false",
+                                        False,
                                     )
                                 )
-                            elif option == "consider" and state.consider_eval == "true":
+                            elif option == "consider" and state.consider_eval:
                                 system_q.put(
                                     eqa_struct.message(
                                         eqa_settings.eqa_time(),
                                         "system",
                                         "consider",
                                         "eval",
-                                        "false",
+                                        False,
                                     )
                                 )
-                            elif (
-                                option == "detect_char" and state.detect_char == "true"
-                            ):
+                            elif option == "detect_char" and state.detect_char:
                                 system_q.put(
                                     eqa_struct.message(
                                         eqa_settings.eqa_time(),
                                         "system",
                                         "detect_char",
-                                        "null",
-                                        "false",
+                                        None,
+                                        False,
                                     )
                                 )
-                            elif (
-                                option == "spell_self"
-                                and state.spell_timer_self == "true"
-                            ):
+                            elif option == "spell_self" and state.spell_timer_self:
                                 system_q.put(
                                     eqa_struct.message(
                                         eqa_settings.eqa_time(),
                                         "system",
                                         "spell",
                                         "self",
-                                        "false",
+                                        False,
                                     )
                                 )
-                            elif (
-                                option == "spell_other"
-                                and state.spell_timer_other == "true"
-                            ):
+                            elif option == "spell_other" and state.spell_timer_other:
                                 system_q.put(
                                     eqa_struct.message(
                                         eqa_settings.eqa_time(),
                                         "system",
                                         "spell",
                                         "other",
-                                        "false",
+                                        False,
                                     )
                                 )
                             elif (
-                                option == "spell_guild"
-                                and state.spell_timer_guild_only == "true"
+                                option == "spell_guild" and state.spell_timer_guild_only
                             ):
                                 system_q.put(
                                     eqa_struct.message(
                                         eqa_settings.eqa_time(),
                                         "system",
                                         "spell",
                                         "guild",
-                                        "false",
+                                        False,
                                     )
                                 )
-                            elif (
-                                option == "spell_guess"
-                                and state.spell_timer_guess == "true"
-                            ):
+                            elif option == "spell_guess" and state.spell_timer_guess:
                                 system_q.put(
                                     eqa_struct.message(
                                         eqa_settings.eqa_time(),
                                         "system",
                                         "spell",
                                         "guess",
-                                        "false",
+                                        False,
                                     )
                                 )
                             elif (
-                                option == "spell_yours"
-                                and state.spell_timer_yours_only == "true"
+                                option == "spell_yours" and state.spell_timer_yours_only
                             ):
                                 system_q.put(
                                     eqa_struct.message(
                                         eqa_settings.eqa_time(),
                                         "system",
                                         "spell",
                                         "yours",
-                                        "false",
+                                        False,
                                     )
                                 )
                         elif key == curses.KEY_LEFT or key == ord("a"):
-                            if option == "debug" and state.debug == "false":
+                            if option == "debug" and not state.debug:
                                 system_q.put(
                                     eqa_struct.message(
                                         eqa_settings.eqa_time(),
                                         "system",
                                         "debug",
                                         "toggle",
-                                        "null",
+                                        None,
                                     )
                                 )
-                            elif option == "mute" and state.mute == "false":
+                            elif option == "mute" and not state.mute:
                                 system_q.put(
                                     eqa_struct.message(
                                         eqa_settings.eqa_time(),
                                         "system",
                                         "mute",
                                         "toggle",
                                         "all",
                                     )
                                 )
-                            elif option == "raid" and state.raid == "false":
+                            elif option == "raid" and not state.raid:
                                 system_q.put(
                                     eqa_struct.message(
                                         eqa_settings.eqa_time(),
                                         "system",
                                         "raid",
                                         "toggle",
                                         "all",
                                     )
                                 )
-                            elif option == "autoraid" and state.auto_raid == "false":
+                            elif option == "autoraid" and not state.auto_raid:
                                 system_q.put(
                                     eqa_struct.message(
                                         eqa_settings.eqa_time(),
                                         "system",
                                         "raid",
                                         "auto",
-                                        "true",
+                                        True,
                                     )
                                 )
-                            elif (
-                                option == "encounter"
-                                and state.encounter_parse == "false"
-                            ):
+                            elif option == "encounter" and not state.encounter_parse:
                                 system_q.put(
                                     eqa_struct.message(
                                         eqa_settings.eqa_time(),
                                         "system",
                                         "encounter",
                                         "toggle",
-                                        "null",
+                                        None,
                                     )
                                 )
-                            elif (
-                                option == "saveencounter"
-                                and state.save_parse == "false"
-                            ):
+                            elif option == "saveencounter" and not state.save_parse:
                                 system_q.put(
                                     eqa_struct.message(
                                         eqa_settings.eqa_time(),
                                         "system",
                                         "encounter",
                                         "save",
-                                        "true",
+                                        True,
                                     )
                                 )
-                            elif (
-                                option == "defaulttimer"
-                                and state.auto_mob_timer == "false"
-                            ):
+                            elif option == "defaulttimer" and not state.auto_mob_timer:
                                 system_q.put(
                                     eqa_struct.message(
                                         eqa_settings.eqa_time(),
                                         "system",
                                         "timer",
                                         "mob",
-                                        "true",
+                                        True,
                                     )
                                 )
-                            elif (
-                                option == "consider" and state.consider_eval == "false"
-                            ):
+                            elif option == "consider" and not state.consider_eval:
                                 system_q.put(
                                     eqa_struct.message(
                                         eqa_settings.eqa_time(),
                                         "system",
                                         "consider",
                                         "eval",
-                                        "true",
+                                        True,
                                     )
                                 )
-                            elif (
-                                option == "detect_char" and state.detect_char == "false"
-                            ):
+                            elif option == "detect_char" and not state.detect_char:
                                 system_q.put(
                                     eqa_struct.message(
                                         eqa_settings.eqa_time(),
                                         "system",
                                         "detect_char",
-                                        "null",
-                                        "true",
+                                        None,
+                                        True,
                                     )
                                 )
-                            elif (
-                                option == "spell_self"
-                                and state.spell_timer_self == "false"
-                            ):
+                            elif option == "spell_self" and not state.spell_timer_self:
                                 system_q.put(
                                     eqa_struct.message(
                                         eqa_settings.eqa_time(),
                                         "system",
                                         "spell",
                                         "self",
-                                        "true",
+                                        True,
                                     )
                                 )
                             elif (
-                                option == "spell_other"
-                                and state.spell_timer_other == "false"
+                                option == "spell_other" and not state.spell_timer_other
                             ):
                                 system_q.put(
                                     eqa_struct.message(
                                         eqa_settings.eqa_time(),
                                         "system",
                                         "spell",
                                         "other",
-                                        "true",
+                                        True,
                                     )
                                 )
                             elif (
                                 option == "spell_guild"
-                                and state.spell_timer_guild_only == "false"
+                                and not state.spell_timer_guild_only
                             ):
                                 system_q.put(
                                     eqa_struct.message(
                                         eqa_settings.eqa_time(),
                                         "system",
                                         "spell",
                                         "guild",
-                                        "true",
+                                        True,
                                     )
                                 )
                             elif (
-                                option == "spell_guess"
-                                and state.spell_timer_guess == "false"
+                                option == "spell_guess" and not state.spell_timer_guess
                             ):
                                 system_q.put(
                                     eqa_struct.message(
                                         eqa_settings.eqa_time(),
                                         "system",
                                         "spell",
                                         "guess",
-                                        "true",
+                                        True,
                                     )
                                 )
                             elif (
                                 option == "spell_yours"
-                                and state.spell_timer_yours_only == "false"
+                                and not state.spell_timer_yours_only
                             ):
                                 system_q.put(
                                     eqa_struct.message(
                                         eqa_settings.eqa_time(),
                                         "system",
                                         "spell",
                                         "yours",
-                                        "true",
+                                        True,
                                     )
                                 )
                         elif key == ord("\t") or key == ord("`"):
                             settings = "line"
                             display_q.put(
                                 eqa_struct.display(
                                     eqa_settings.eqa_time(),
```

### Comparing `eqalert-3.5.0/eqa/lib/log.py` & `eqalert-3.5.1/eqa/lib/log.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.0/eqa/lib/parser.py` & `eqalert-3.5.1/eqa/lib/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,84 +196,84 @@
 00000c30: 2020 2020 2320 5370 656c 6c0a 2020 2020      # Spell.    
 00000c40: 2020 2020 6c69 6e65 5f74 7970 6520 3d20      line_type = 
 00000c50: 6368 6563 6b5f 7370 656c 6c28 6c69 6e65  check_spell(line
 00000c60: 290a 2020 2020 2020 2020 6966 206c 696e  ).        if lin
 00000c70: 655f 7479 7065 2069 7320 6e6f 7420 4e6f  e_type is not No
 00000c80: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
 00000c90: 7265 7475 726e 206c 696e 655f 7479 7065  return line_type
-00000ca0: 0a0a 2020 2020 2020 2020 2320 5065 7473  ..        # Pets
-00000cb0: 0a20 2020 2020 2020 206c 696e 655f 7479  .        line_ty
-00000cc0: 7065 203d 2063 6865 636b 5f70 6574 7328  pe = check_pets(
-00000cd0: 6c69 6e65 290a 2020 2020 2020 2020 6966  line).        if
-00000ce0: 206c 696e 655f 7479 7065 2069 7320 6e6f   line_type is no
-00000cf0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00000d00: 2020 2020 7265 7475 726e 206c 696e 655f      return line_
-00000d10: 7479 7065 0a0a 2020 2020 2020 2020 2320  type..        # 
-00000d20: 5265 6365 6976 6564 2050 6c61 7965 7220  Received Player 
-00000d30: 4368 6174 0a20 2020 2020 2020 206c 696e  Chat.        lin
-00000d40: 655f 7479 7065 203d 2063 6865 636b 5f72  e_type = check_r
-00000d50: 6563 6569 7665 645f 6368 6174 286c 696e  eceived_chat(lin
-00000d60: 6529 0a20 2020 2020 2020 2069 6620 6c69  e).        if li
-00000d70: 6e65 5f74 7970 6520 6973 206e 6f74 204e  ne_type is not N
-00000d80: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00000d90: 2072 6574 7572 6e20 6c69 6e65 5f74 7970   return line_typ
-00000da0: 650a 0a20 2020 2020 2020 2023 2053 656e  e..        # Sen
-00000db0: 7420 506c 6179 6572 2043 6861 740a 2020  t Player Chat.  
-00000dc0: 2020 2020 2020 6c69 6e65 5f74 7970 6520        line_type 
-00000dd0: 3d20 6368 6563 6b5f 7365 6e74 5f63 6861  = check_sent_cha
-00000de0: 7428 6c69 6e65 290a 2020 2020 2020 2020  t(line).        
-00000df0: 6966 206c 696e 655f 7479 7065 2069 7320  if line_type is 
-00000e00: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00000e10: 2020 2020 2020 7265 7475 726e 206c 696e        return lin
-00000e20: 655f 7479 7065 0a0a 2020 2020 2020 2020  e_type..        
-00000e30: 2320 436f 6d6d 616e 6420 4f75 7470 7574  # Command Output
-00000e40: 0a20 2020 2020 2020 206c 696e 655f 7479  .        line_ty
-00000e50: 7065 203d 2063 6865 636b 5f63 6f6d 6d61  pe = check_comma
-00000e60: 6e64 5f6f 7574 7075 7428 6c69 6e65 290a  nd_output(line).
-00000e70: 2020 2020 2020 2020 6966 206c 696e 655f          if line_
-00000e80: 7479 7065 2069 7320 6e6f 7420 4e6f 6e65  type is not None
-00000e90: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00000ea0: 7475 726e 206c 696e 655f 7479 7065 0a0a  turn line_type..
-00000eb0: 2020 2020 2020 2020 2320 5379 7374 656d          # System
-00000ec0: 204d 6573 7361 6765 730a 2020 2020 2020   Messages.      
-00000ed0: 2020 6c69 6e65 5f74 7970 6520 3d20 6368    line_type = ch
-00000ee0: 6563 6b5f 7379 7374 656d 5f6d 6573 7361  eck_system_messa
-00000ef0: 6765 7328 6c69 6e65 290a 2020 2020 2020  ges(line).      
-00000f00: 2020 6966 206c 696e 655f 7479 7065 2069    if line_type i
-00000f10: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00000f20: 2020 2020 2020 2020 7265 7475 726e 206c          return l
-00000f30: 696e 655f 7479 7065 0a0a 2020 2020 2020  ine_type..      
-00000f40: 2020 2320 4772 6f75 7020 5379 7374 656d    # Group System
-00000f50: 204d 6573 7361 6765 730a 2020 2020 2020   Messages.      
-00000f60: 2020 6c69 6e65 5f74 7970 6520 3d20 6368    line_type = ch
-00000f70: 6563 6b5f 6772 6f75 705f 7379 7374 656d  eck_group_system
-00000f80: 5f6d 6573 7361 6765 7328 6c69 6e65 290a  _messages(line).
-00000f90: 2020 2020 2020 2020 6966 206c 696e 655f          if line_
-00000fa0: 7479 7065 2069 7320 6e6f 7420 4e6f 6e65  type is not None
-00000fb0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00000fc0: 7475 726e 206c 696e 655f 7479 7065 0a0a  turn line_type..
-00000fd0: 2020 2020 2020 2020 2320 4c6f 6f74 2054          # Loot T
-00000fe0: 7261 6465 204d 6573 7361 6765 730a 2020  rade Messages.  
-00000ff0: 2020 2020 2020 6c69 6e65 5f74 7970 6520        line_type 
-00001000: 3d20 6368 6563 6b5f 6c6f 6f74 5f74 7261  = check_loot_tra
-00001010: 6465 286c 696e 6529 0a20 2020 2020 2020  de(line).       
-00001020: 2069 6620 6c69 6e65 5f74 7970 6520 6973   if line_type is
-00001030: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00001040: 2020 2020 2020 2072 6574 7572 6e20 6c69         return li
-00001050: 6e65 5f74 7970 650a 0a20 2020 2020 2020  ne_type..       
-00001060: 2023 2045 6d6f 7465 730a 2020 2020 2020   # Emotes.      
-00001070: 2020 6c69 6e65 5f74 7970 6520 3d20 6368    line_type = ch
-00001080: 6563 6b5f 656d 6f74 6573 286c 696e 6529  eck_emotes(line)
-00001090: 0a20 2020 2020 2020 2069 6620 6c69 6e65  .        if line
-000010a0: 5f74 7970 6520 6973 206e 6f74 204e 6f6e  _type is not Non
-000010b0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-000010c0: 6574 7572 6e20 6c69 6e65 5f74 7970 650a  eturn line_type.
-000010d0: 0a20 2020 2020 2020 2023 2057 686f 0a20  .        # Who. 
-000010e0: 2020 2020 2020 206c 696e 655f 7479 7065         line_type
-000010f0: 203d 2063 6865 636b 5f77 686f 286c 696e   = check_who(lin
+00000ca0: 0a0a 2020 2020 2020 2020 2320 5768 6f0a  ..        # Who.
+00000cb0: 2020 2020 2020 2020 6c69 6e65 5f74 7970          line_typ
+00000cc0: 6520 3d20 6368 6563 6b5f 7768 6f28 6c69  e = check_who(li
+00000cd0: 6e65 290a 2020 2020 2020 2020 6966 206c  ne).        if l
+00000ce0: 696e 655f 7479 7065 2069 7320 6e6f 7420  ine_type is not 
+00000cf0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00000d00: 2020 7265 7475 726e 206c 696e 655f 7479    return line_ty
+00000d10: 7065 0a0a 2020 2020 2020 2020 2320 5065  pe..        # Pe
+00000d20: 7473 0a20 2020 2020 2020 206c 696e 655f  ts.        line_
+00000d30: 7479 7065 203d 2063 6865 636b 5f70 6574  type = check_pet
+00000d40: 7328 6c69 6e65 290a 2020 2020 2020 2020  s(line).        
+00000d50: 6966 206c 696e 655f 7479 7065 2069 7320  if line_type is 
+00000d60: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00000d70: 2020 2020 2020 7265 7475 726e 206c 696e        return lin
+00000d80: 655f 7479 7065 0a0a 2020 2020 2020 2020  e_type..        
+00000d90: 2320 5265 6365 6976 6564 2050 6c61 7965  # Received Playe
+00000da0: 7220 4368 6174 0a20 2020 2020 2020 206c  r Chat.        l
+00000db0: 696e 655f 7479 7065 203d 2063 6865 636b  ine_type = check
+00000dc0: 5f72 6563 6569 7665 645f 6368 6174 286c  _received_chat(l
+00000dd0: 696e 6529 0a20 2020 2020 2020 2069 6620  ine).        if 
+00000de0: 6c69 6e65 5f74 7970 6520 6973 206e 6f74  line_type is not
+00000df0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00000e00: 2020 2072 6574 7572 6e20 6c69 6e65 5f74     return line_t
+00000e10: 7970 650a 0a20 2020 2020 2020 2023 2053  ype..        # S
+00000e20: 656e 7420 506c 6179 6572 2043 6861 740a  ent Player Chat.
+00000e30: 2020 2020 2020 2020 6c69 6e65 5f74 7970          line_typ
+00000e40: 6520 3d20 6368 6563 6b5f 7365 6e74 5f63  e = check_sent_c
+00000e50: 6861 7428 6c69 6e65 290a 2020 2020 2020  hat(line).      
+00000e60: 2020 6966 206c 696e 655f 7479 7065 2069    if line_type i
+00000e70: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00000e80: 2020 2020 2020 2020 7265 7475 726e 206c          return l
+00000e90: 696e 655f 7479 7065 0a0a 2020 2020 2020  ine_type..      
+00000ea0: 2020 2320 436f 6d6d 616e 6420 4f75 7470    # Command Outp
+00000eb0: 7574 0a20 2020 2020 2020 206c 696e 655f  ut.        line_
+00000ec0: 7479 7065 203d 2063 6865 636b 5f63 6f6d  type = check_com
+00000ed0: 6d61 6e64 5f6f 7574 7075 7428 6c69 6e65  mand_output(line
+00000ee0: 290a 2020 2020 2020 2020 6966 206c 696e  ).        if lin
+00000ef0: 655f 7479 7065 2069 7320 6e6f 7420 4e6f  e_type is not No
+00000f00: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00000f10: 7265 7475 726e 206c 696e 655f 7479 7065  return line_type
+00000f20: 0a0a 2020 2020 2020 2020 2320 5379 7374  ..        # Syst
+00000f30: 656d 204d 6573 7361 6765 730a 2020 2020  em Messages.    
+00000f40: 2020 2020 6c69 6e65 5f74 7970 6520 3d20      line_type = 
+00000f50: 6368 6563 6b5f 7379 7374 656d 5f6d 6573  check_system_mes
+00000f60: 7361 6765 7328 6c69 6e65 290a 2020 2020  sages(line).    
+00000f70: 2020 2020 6966 206c 696e 655f 7479 7065      if line_type
+00000f80: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00000f90: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00000fa0: 206c 696e 655f 7479 7065 0a0a 2020 2020   line_type..    
+00000fb0: 2020 2020 2320 4772 6f75 7020 5379 7374      # Group Syst
+00000fc0: 656d 204d 6573 7361 6765 730a 2020 2020  em Messages.    
+00000fd0: 2020 2020 6c69 6e65 5f74 7970 6520 3d20      line_type = 
+00000fe0: 6368 6563 6b5f 6772 6f75 705f 7379 7374  check_group_syst
+00000ff0: 656d 5f6d 6573 7361 6765 7328 6c69 6e65  em_messages(line
+00001000: 290a 2020 2020 2020 2020 6966 206c 696e  ).        if lin
+00001010: 655f 7479 7065 2069 7320 6e6f 7420 4e6f  e_type is not No
+00001020: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00001030: 7265 7475 726e 206c 696e 655f 7479 7065  return line_type
+00001040: 0a0a 2020 2020 2020 2020 2320 4c6f 6f74  ..        # Loot
+00001050: 2054 7261 6465 204d 6573 7361 6765 730a   Trade Messages.
+00001060: 2020 2020 2020 2020 6c69 6e65 5f74 7970          line_typ
+00001070: 6520 3d20 6368 6563 6b5f 6c6f 6f74 5f74  e = check_loot_t
+00001080: 7261 6465 286c 696e 6529 0a20 2020 2020  rade(line).     
+00001090: 2020 2069 6620 6c69 6e65 5f74 7970 6520     if line_type 
+000010a0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000010b0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000010c0: 6c69 6e65 5f74 7970 650a 0a20 2020 2020  line_type..     
+000010d0: 2020 2023 2045 6d6f 7465 730a 2020 2020     # Emotes.    
+000010e0: 2020 2020 6c69 6e65 5f74 7970 6520 3d20      line_type = 
+000010f0: 6368 6563 6b5f 656d 6f74 6573 286c 696e  check_emotes(lin
 00001100: 6529 0a20 2020 2020 2020 2069 6620 6c69  e).        if li
 00001110: 6e65 5f74 7970 6520 6973 206e 6f74 204e  ne_type is not N
 00001120: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
 00001130: 2072 6574 7572 6e20 6c69 6e65 5f74 7970   return line_typ
 00001140: 650a 0a20 2020 2020 2020 2023 2053 7065  e..        # Spe
 00001150: 6c6c 2053 7065 6369 6669 630a 2020 2020  ll Specific.    
 00001160: 2020 2020 6c69 6e65 5f74 7970 6520 3d20      line_type =
```

### Comparing `eqalert-3.5.0/eqa/lib/settings.py` & `eqalert-3.5.1/eqa/lib/settings.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.0/eqa/lib/sound.py` & `eqalert-3.5.1/eqa/lib/sound.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,16 +34,16 @@
     """
     Process: sound_q
     Produce: sound event
     """
 
     sound_file_path = configs.settings.config["settings"]["paths"]["sound"]
     tmp_sound_file_path = configs.settings.config["settings"]["paths"]["tmp_sound"]
-    mute_speak = "false"
-    mute_alert = "false"
+    mute_speak = False
+    mute_alert = False
 
     if not os.path.exists(tmp_sound_file_path):
         os.makedirs(tmp_sound_file_path)
 
     try:
         while not exit_flag.is_set() and not cfg_reload.is_set():
             # Sleep between empty checks
@@ -51,30 +51,34 @@
                 time.sleep(0.01)
 
             # Check queue for message
             if not sound_q.empty():
                 ## Read new message
                 sound_event = sound_q.get()
 
-                if sound_event.sound == "mute_speak":
-                    mute_speak = sound_event.payload
-                elif sound_event.sound == "mute_alert":
-                    mute_alert = sound_event.payload
-                elif (
-                    sound_event.sound == "speak"
-                    and not mute_speak == "true"
-                    and not state.mute == "true"
-                ):
-                    speak(configs, sound_event.payload, "true", tmp_sound_file_path)
-                elif (
-                    sound_event.sound == "alert"
-                    and not mute_alert == "true"
-                    and not state.mute == "true"
-                ):
+                if sound_event.sound == "speak" and not mute_speak and not state.mute:
+                    speak(configs, sound_event.payload, True, tmp_sound_file_path)
+                elif sound_event.sound == "alert" and not mute_alert and not state.mute:
                     alert(configs, sound_event.payload)
+                elif sound_event.sound == "mute_speak":
+                    if sound_event.payload == "toggle":
+                        if mute_speak:
+                            mute_speak = False
+                        else:
+                            mute_speak = True
+                    else:
+                        mute_speak = sound_event.payload
+                elif sound_event.sound == "mute_alert":
+                    if sound_event.payload == "toggle":
+                        if mute_alert:
+                            mute_alert = False
+                        else:
+                            mute_alert = True
+                    else:
+                        mute_alert = sound_event.payload
                 elif sound_event.sound == "tick":
                     sound_tick(sound_file_path, sound_event)
                 elif sound_event.sound == "tock":
                     sound_tock(sound_file_path, sound_event)
 
                 sound_q.task_done()
 
@@ -144,14 +148,15 @@
     line = re.sub(r"(?<=[^A-z])guk(?=[^A-z])", "guck", line, flags=re.I)
     line = re.sub(r"(?<=[^A-z])hh(?=[^A-z])", "hammer hill", line, flags=re.I)
     line = re.sub(r"(?<=[^A-z])hmu(?=[^A-z])", "hit me up", line, flags=re.I)
     line = re.sub(r"(?<=[^A-z])hp(?=[^A-z])", "hit points", line, flags=re.I)
     line = re.sub(r"(?<=[^A-z])hs(?=[^A-z])", "howling stones", line, flags=re.I)
     line = re.sub(r"(?<=[^A-z])ic(?=[^A-z])", "iceclad ocean", line, flags=re.I)
     line = re.sub(r"(?<=[^A-z])idc(?=[^A-z])", "I don't care", line, flags=re.I)
+    line = re.sub(r"(?<=[^A-z])ii(?=[^A-z])", "two", line, flags=re.I)
     line = re.sub(r"(?<=[^A-z])imo(?=[^A-z])", "in my opinion", line, flags=re.I)
     line = re.sub(r"(?<=[^A-z])inc(?=[^A-z])", "incoming", line, flags=re.I)
     line = re.sub(r"(?<=[^A-z])inv(?=[^A-z])", "invite", line, flags=re.I)
     line = re.sub(r"(?<=[^A-z])irl(?=[^A-z])", "in real life", line, flags=re.I)
     line = re.sub(r"(?<=[^A-z])kc(?=[^A-z])", "karnors castle", line, flags=re.I)
     line = re.sub(r"(?<=[^A-z])ld(?=[^A-z])", "link dead", line, flags=re.I)
     line = re.sub(r"(?<=[^A-z])lev(?=[^A-z])", "levitate", line, flags=re.I)
@@ -180,14 +185,17 @@
     line = re.sub(r"(?<=[^A-z])ph(?=[^A-z])", "place holder", line, flags=re.I)
     line = re.sub(r"(?<=[^A-z])pl(?=[^A-z])", "power level", line, flags=re.I)
     line = re.sub(r"(?<=[^A-z])pls(?=[^A-z])", "please", line, flags=re.I)
     line = re.sub(r"(?<=[^A-z])plz(?=[^A-z])", "please", line, flags=re.I)
     line = re.sub(r"(?<=[^A-z])pof(?=[^A-z])", "plane of fear", line, flags=re.I)
     line = re.sub(r"(?<=[^A-z])poh(?=[^A-z])", "plane of hate", line, flags=re.I)
     line = re.sub(r"(?<=[^A-z])pom(?=[^A-z])", "plane of mischief", line, flags=re.I)
+    line = re.sub(
+        r"(?<=[^A-z])potg(?=[^A-z])", "protection of the glades", line, flags=re.I
+    )
     line = re.sub(r"(?<=[^A-z])pov(?=[^A-z])", "point of view", line, flags=re.I)
     line = re.sub(r"(?<=[^A-z])pst(?=[^A-z])", "please send tell", line, flags=re.I)
     line = re.sub(r"(?<=[^A-z])rh(?=[^A-z])", "right here", line, flags=re.I)
     line = re.sub(r"(?<=[^A-z])rl(?=[^A-z])", "real life", line, flags=re.I)
     line = re.sub(r"(?<=[^A-z])rn(?=[^A-z])", "right now", line, flags=re.I)
     line = re.sub(r"(?<=[^A-z])rog(?=[^A-z])", "rog", line, flags=re.I)
     line = re.sub(r"(?<=[^A-z])rw(?=[^A-z])", "ring war", line, flags=re.I)
@@ -215,50 +223,55 @@
     line = re.sub(r"(?<=[^A-z])wru(?=[^A-z])", "where are you", line, flags=re.I)
     line = re.sub(r"(?<=[^A-z])wtb(?=[^A-z])", "want to buy", line, flags=re.I)
     line = re.sub(r"(?<=[^A-z])wtf(?=[^A-z])", "what the f", line, flags=re.I)
     line = re.sub(r"(?<=[^A-z])wts(?=[^A-z])", "want to sell", line, flags=re.I)
     line = re.sub(r"(?<=[^A-z])wtt(?=[^A-z])", "want to trade", line, flags=re.I)
     line = re.sub(r"(?<=[^A-z])xfer(?=[^A-z])", "transfer", line, flags=re.I)
     line = re.sub(r"(?<=[^A-z])yw(?=[^A-z])", "you're welcome", line, flags=re.I)
+    line = re.sub(r"(?<=[^A-z])\=D(?=[^A-z])", "smiley face", line, flags=re.I)
     line = re.sub(r"(?<=[^A-z])<3(?=[^A-z])", "heart", line, flags=re.I)
+    line = re.sub(r"(?<=[^A-z])>\.<(?=[^A-z])", "squinting face", line, flags=re.I)
+    line = re.sub(
+        r"(?<=[^A-z])>\_<(?=[^A-z])", "serious squinting face", line, flags=re.I
+    )
     line = re.sub(r"(\d+)p(?![A-z])", r"\1 platinum", line, flags=re.I)
     line = re.sub(r"(\d+)m(?![A-z])", r"\1 mana", line, flags=re.I)
 
     return line
 
 
 def speak(configs, line, play, sound_file_path):
     """Play a spoken phrase"""
     try:
-        if configs.settings.config["settings"]["speech"]["expand_lingo"] == "true":
+        if configs.settings.config["settings"]["speech"]["expand_lingo"]:
             phrase = eq_lingo(line)
         else:
             phrase = line
         phrase_hash = hashlib.md5(phrase.encode())
         if not os.path.exists(sound_file_path + phrase_hash.hexdigest() + ".wav"):
             gtts_tld = configs.settings.config["settings"]["speech"]["tld"]
             gtts_lang = configs.settings.config["settings"]["speech"]["lang"]
             tts = gtts.gTTS(text=phrase, lang=gtts_lang, tld=gtts_tld)
             tts.save(sound_file_path + phrase_hash.hexdigest() + ".wav")
-        if play == "true":
+        if play:
             play_sound(sound_file_path + phrase_hash.hexdigest() + ".wav")
 
     except Exception as e:
         eqa_settings.log(
             "sound_speak: Error on line "
             + str(sys.exc_info()[-1].tb_lineno)
             + ": "
             + str(e)
         )
 
 
 def alert(configs, line_type):
     """Play configured sounds"""
     try:
-        if not configs.alerts.config["line"][line_type]["sound"] == "false":
+        if not configs.alerts.config["line"][line_type]["sound"] == False:
             phrase = configs.alerts.config["line"][line_type]["sound"]
             sound_file_path = configs.settings.config["settings"]["paths"]["sound"]
             if not os.path.exists(sound_file_path + phrase + ".wav"):
                 gtts_tld = configs.settings.config["settings"]["speech"]["tld"]
                 gtts_lang = configs.settings.config["settings"]["speech"]["lang"]
                 tts = gtts.gTTS(text=phrase, lang=gtts_lang, tld=gtts_tld)
                 tts.save(sound_file_path + phrase + ".wav")
```

### Comparing `eqalert-3.5.0/eqa/lib/state.py` & `eqalert-3.5.1/eqa/lib/state.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.0/eqa/lib/struct.py` & `eqalert-3.5.1/eqa/lib/struct.py`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.0/eqa/lib/timer.py` & `eqalert-3.5.1/eqa/lib/timer.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,20 +165,17 @@
                     timers = remove_spell_timer(state, timers, timer_event)
                 elif timer_event.type == "metronome_stop":
                     if len(timers) == 0:
                         metronome_stop = False
                     elif metronome_stop == False:
                         metronome_stop = True
                 elif timer_event.type == "new_zone":
-                    if (
-                        configs.settings.config["settings"]["timers"][
-                            "spell_timer_zone_drift"
-                        ]
-                        == "true"
-                    ):
+                    if configs.settings.config["settings"]["timers"]["spell"][
+                        "zone_drift"
+                    ]:
                         if zoning_start_time is not None:
                             adjustment = (
                                 timer_event.time - zoning_start_time
                             ).total_seconds()
                             # If the zone duration is more than a minute, give up something is wrong
                             if adjustment <= 45:
                                 timers = self_spell_timer_drift(
@@ -301,15 +298,15 @@
         new_timers = []
         for timer_event in timers:
             if timer_event.type == "spell":
                 if (
                     remove_timer.target == timer_event.target
                     and remove_timer.spell == timer_event.spell
                 ):
-                    if state.debug == "true":
+                    if state.debug:
                         eqa_settings.log(
                             "Removing timer: "
                             + timer_event.spell
                             + " on "
                             + timer_event.target
                         )
                 else:
@@ -335,15 +332,15 @@
         new_timers = []
         for timer_event in timers:
             if timer_event.type == "spell":
                 if (
                     new_timer_event.target == timer_event.target
                     and new_timer_event.spell == timer_event.spell
                 ):
-                    if state.debug == "true":
+                    if state.debug:
                         eqa_settings.log(
                             "Removing old timer: "
                             + timer_event.spell
                             + " on "
                             + timer_event.target
                         )
                 else:
```

### Comparing `eqalert-3.5.0/eqa/lib/watch.py` & `eqalert-3.5.1/eqa/lib/watch.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         logs_directory = configs.settings.config["settings"]["paths"]["everquest_logs"]
 
         # Watch log directory
         while not exit_flag.is_set() and not cfg_reload.is_set():
             time.sleep(1)
 
             ## Only check when enabled
-            if state.detect_char == "true":
+            if state.detect_char:
                 ### Find newest eqlog_ prefixed file
                 for log_file in os.listdir(logs_directory):
                     if log_file.startswith("eqlog_"):
                         modified_time = os.stat(logs_directory + log_file).st_mtime
                         if modified_time > most_recent:
                             most_recent = modified_time
                             game, char, server_dirty = log_file.split("_")
@@ -55,15 +55,15 @@
                 if char != state.char or server != state.server:
                     char_server = char + "_" + server
                     system_q.put(
                         eqa_struct.message(
                             eqa_settings.eqa_time(),
                             "system",
                             "new_character",
-                            "null",
+                            None,
                             char_server,
                         )
                     )
 
     except Exception as e:
         eqa_settings.log(
             "watch_process: Error on line "
```

### Comparing `eqalert-3.5.0/eqa/sound/tick.wav` & `eqalert-3.5.1/eqa/sound/tick.wav`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.0/eqa/sound/tock.wav` & `eqalert-3.5.1/eqa/sound/tock.wav`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.0/eqalert.egg-info/PKG-INFO` & `eqalert-3.5.1/eqalert.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eqalert
-Version: 3.5.0
+Version: 3.5.1
 Summary: Configurable and Context Driven Project 1999 Log Parser
 Home-page: https://github.com/mgeitz/eqalert
 Author: M Geitz
 Author-email: git@geitz.xyz
 License: GPL2
 Requires-Python: >=3.9.2
 Description-Content-Type: text/markdown
@@ -234,16 +234,16 @@
 
 ### Line Types
 
 Example configuration for a line type:
 ```
     "line_type_name": {
       "alert": {},
-      "reaction": "false",
-      "sound": "false"
+      "reaction": false,
+      "sound": false
     },
 ```
 
 #### Reaction Values
 
 ##### General
 - `false`: Disable alerting for this line type
@@ -267,15 +267,15 @@
 
 ###### Example 1
 Alert for the word `hey` when someone else `/says` it:
 
 ```
     "say": {
       "alert": {
-        "hey": "true"
+        "hey": true
       },
       "reaction": "alert",
       "sound": "hey"
     },
 ```
 
 ###### Example 2
@@ -294,25 +294,25 @@
 ###### Example 4
 Alert for a spell not taking hold only when grouped:
 
 ```
     "spell_not_hold": {
       "alert": {},
       "reaction": "group_only",
-      "sound": "true"
+      "sound": true
     },
 ```
 
 ###### Example 4
 Alert for the item `Hand Made Backpack` when someone else `/auctions` it and is selling:
 
 ```
     "auction_wts": {
       "alert": {
-        "Hand Made Backpack": "true"
+        "Hand Made Backpack": true
       },
       "reaction": "alert",
       "sound": "wow buy that"
     },
 ```
 
 > More examples can be referenced in the default config
@@ -320,27 +320,27 @@
 #### Alert Values
 
 ##### General
 - `false`: Disable alerting for the string (does not negate line type reactions)
 - `true`: Alert for the string
 
 ##### Context Driven
-- `solo`: Alert when solo, grouped, and raiding
-- `solo_only`: Alert only when solo
-- `group`: Alert when in a group and raiding
-- `group_only`: Alert only when grouped
-- `solo_group_only`: Alert only when not raiding
-- `raid`: Alert when in a raid
-- `afk`: Alert only when afk
+- `"solo"`: Alert when solo, grouped, and raiding
+- `"solo_only"`: Alert only when solo
+- `"group"`: Alert when in a group and raiding
+- `"group_only"`: Alert only when grouped
+- `"solo_group_only"`: Alert only when not raiding
+- `"raid"`: Alert when in a raid
+- `"afk"`: Alert only when afk
 
 #### Sound Values
 - `true`: When an alert is raised speak the entire line
 - `false`: Play no sound when an alert is raised
 
-> Any other sound value will be spoken as the audio trigger for that line type
+> Any other sound value (as a string) will be spoken as the audio trigger for that line type
 
 #### The all Line Type
 
 This line type behaves the same as any specific line type configuration, but configuration here will be used against all log lines.
 
 For example, the below configuration will alert if the word `help` is found in any line while in a raid context, even if that line isn't matched to a type by the parser.
 
@@ -355,14 +355,17 @@
 ```
 
 This can be helpful if you would like to alert for something not yet matched by the parser, though your [contribution](CONTRIBUTING.md#pull-requests) to a new line type match in the parser would also be welcome!
 
 ### Zones
 Zone data is stored in `config/zones.json`
 
+#### indoors
+Whether or not this zone is considered indoors.  Currently does nothing.
+
 #### raid_mode
 - `false`: If enabled, auto-disable raid mode in this zone
 - `true`: If enabled, auto-enable raid mode in this zone
 
 #### timer
 - `#`: The value in seconds to associate to a default timer in a given zone
```

### Comparing `eqalert-3.5.0/eqalert.egg-info/SOURCES.txt` & `eqalert-3.5.1/eqalert.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eqalert-3.5.0/setup.py` & `eqalert-3.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="eqalert",
-    version="3.5.0",
+    version="3.5.1",
     author="M Geitz",
     author_email="git@geitz.xyz",
     install_requires=[
         "playsound>=1.3.0",
         "gtts>=2.3.1",
     ],
     python_requires=">=3.9.2",
```

