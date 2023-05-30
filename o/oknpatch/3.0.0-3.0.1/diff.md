# Comparing `tmp/oknpatch-3.0.0.tar.gz` & `tmp/oknpatch-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oknpatch-3.0.0.tar", last modified: Sun May 28 23:50:21 2023, max compression
+gzip compressed data, was "oknpatch-3.0.1.tar", last modified: Tue May 30 04:35:04 2023, max compression
```

## Comparing `oknpatch-3.0.0.tar` & `oknpatch-3.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 23:50:21.945933 oknpatch-3.0.0/
--rw-rw-rw-   0        0        0    11558 2022-07-06 00:41:01.000000 oknpatch-3.0.0/LICENSE
--rw-rw-rw-   0        0        0      525 2023-05-28 23:50:21.945933 oknpatch-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2344 2023-02-27 04:55:12.000000 oknpatch-3.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 23:50:21.935196 oknpatch-3.0.0/oknpatch/
--rw-rw-rw-   0        0        0        0 2023-02-12 22:01:11.000000 oknpatch-3.0.0/oknpatch/__init__.py
--rw-rw-rw-   0        0        0     6263 2023-05-17 08:39:07.000000 oknpatch-3.0.0/oknpatch/gazefilters.json
--rw-rw-rw-   0        0        0    13248 2023-02-13 03:27:15.000000 oknpatch-3.0.0/oknpatch/okndetector.gaze.config
--rw-rw-rw-   0        0        0    36912 2023-05-28 23:34:44.000000 oknpatch-3.0.0/oknpatch/oknpatch.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:50:21.944172 oknpatch-3.0.0/oknpatch.egg-info/
--rw-rw-rw-   0        0        0      525 2023-05-28 23:50:21.000000 oknpatch-3.0.0/oknpatch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2023-05-28 23:50:21.000000 oknpatch-3.0.0/oknpatch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 23:50:21.000000 oknpatch-3.0.0/oknpatch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-28 23:50:21.000000 oknpatch-3.0.0/oknpatch.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-28 23:50:08.000000 oknpatch-3.0.0/oknpatch.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2023-05-28 23:50:21.000000 oknpatch-3.0.0/oknpatch.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-28 23:50:21.000000 oknpatch-3.0.0/oknpatch.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 23:50:21.945933 oknpatch-3.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1062 2023-05-28 22:12:49.000000 oknpatch-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 04:35:04.502477 oknpatch-3.0.1/
+-rw-rw-rw-   0        0        0    11558 2023-03-26 20:00:42.000000 oknpatch-3.0.1/LICENSE
+-rw-rw-rw-   0        0        0      525 2023-05-30 04:35:04.502477 oknpatch-3.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2344 2023-03-26 20:00:42.000000 oknpatch-3.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 04:35:04.502477 oknpatch-3.0.1/oknpatch/
+-rw-rw-rw-   0        0        0        0 2023-03-26 20:00:42.000000 oknpatch-3.0.1/oknpatch/__init__.py
+-rw-rw-rw-   0        0        0     6263 2023-05-30 03:34:05.000000 oknpatch-3.0.1/oknpatch/gazefilters.json
+-rw-rw-rw-   0        0        0    13248 2023-05-30 03:34:05.000000 oknpatch-3.0.1/oknpatch/okndetector.gaze.config
+-rw-rw-rw-   0        0        0    38301 2023-05-30 04:34:43.000000 oknpatch-3.0.1/oknpatch/oknpatch.py
+drwxrwxrwx   0        0        0        0 2023-05-30 04:35:04.502477 oknpatch-3.0.1/oknpatch.egg-info/
+-rw-rw-rw-   0        0        0      525 2023-05-30 04:35:04.000000 oknpatch-3.0.1/oknpatch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2023-05-30 04:35:04.000000 oknpatch-3.0.1/oknpatch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 04:35:04.000000 oknpatch-3.0.1/oknpatch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-30 04:35:04.000000 oknpatch-3.0.1/oknpatch.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-30 04:34:49.000000 oknpatch-3.0.1/oknpatch.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       35 2023-05-30 04:35:04.000000 oknpatch-3.0.1/oknpatch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-30 04:35:04.000000 oknpatch-3.0.1/oknpatch.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 04:35:04.502477 oknpatch-3.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1062 2023-05-30 04:34:43.000000 oknpatch-3.0.1/setup.py
```

### Comparing `oknpatch-3.0.0/LICENSE` & `oknpatch-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oknpatch-3.0.0/PKG-INFO` & `oknpatch-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oknpatch
-Version: 3.0.0
+Version: 3.0.1
 Summary: issues fixing program
 Home-page: https://github.com/jtur044/oknpatch
 Author: Zaw Lin Tun
 Author-email: zawlintun1511@gmail.com
 License: Apache Software
 Keywords: oknpatch
 Classifier: Programming Language :: Python :: 3
```

### Comparing `oknpatch-3.0.0/README.md` & `oknpatch-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `oknpatch-3.0.0/oknpatch/gazefilters.json` & `oknpatch-3.0.1/oknpatch/gazefilters.json`

 * *Files identical despite different names*

### Comparing `oknpatch-3.0.0/oknpatch/okndetector.gaze.config` & `oknpatch-3.0.1/oknpatch/okndetector.gaze.config`

 * *Files identical despite different names*

### Comparing `oknpatch-3.0.0/oknpatch/oknpatch.py` & `oknpatch-3.0.1/oknpatch/oknpatch.py`

 * *Files 1% similar despite different names*

```diff
@@ -667,51 +667,73 @@
         error_string = f"Error occurred:error type:{type(error).__name__} in line number:{exc_tb.tb_lineno}."
         trial_csv_file_name = None
         output_dir_without_folder = None
 
     return trial_csv_file_name, output_dir_without_folder, success, error_string
 
 
+# This function is to replace direction column value of input csv file with given direction input 1 or -1
 def replace_with_new_direction(csv_file_input, direction_input):
-    with open(csv_file_input, "r") as trial_csv_file:
-        trial_csv_data = csv.reader(trial_csv_file, delimiter=',')
-        trial_header_array = next(trial_csv_data)
-        direction_position = get_position("direction", trial_header_array)
-        trial_rows = []
-        for data in trial_csv_data:
-            trial_rows.append(data)
-        trial_csv_file.close()
-
-    for row in trial_rows:
-        row[direction_position] = direction_input
-
-    # rewrite and replace incorrect data with correct data
-    with open(csv_file_input, mode='w', newline="") as new_destination_file:
-        csv_writer = csv.DictWriter(new_destination_file, fieldnames=trial_header_array)
-        csv_writer.writeheader()
-        for data in trial_rows:
-            data_to_write = {}
-            for ind, name in enumerate(trial_header_array):
-                data_to_write[name] = data[ind]
-            csv_writer.writerow(data_to_write)
+    replace_successful = True
+    if int(direction_input) == 1 or int(direction_input) == -1:
+        try:
+            with open(csv_file_input, "r") as trial_csv_file:
+                trial_csv_data = csv.reader(trial_csv_file, delimiter=',')
+                trial_header_array = next(trial_csv_data)
+                direction_position = get_position("direction", trial_header_array)
+                trial_rows = []
+                for data in trial_csv_data:
+                    trial_rows.append(data)
+                trial_csv_file.close()
+
+            for row in trial_rows:
+                row[direction_position] = direction_input
+
+            # rewrite and replace incorrect data with correct data
+            with open(csv_file_input, mode='w', newline="") as new_destination_file:
+                csv_writer = csv.DictWriter(new_destination_file, fieldnames=trial_header_array)
+                csv_writer.writeheader()
+                for data in trial_rows:
+                    data_to_write = {}
+                    for ind, name in enumerate(trial_header_array):
+                        data_to_write[name] = data[ind]
+                    csv_writer.writerow(data_to_write)
+
+                new_destination_file.close()
+        except Exception as error:
+            replace_successful = False
+            exc_type, exc_obj, exc_tb = sys.exc_info()
+            error_string = f"Error occurred:error type:{type(error).__name__} in line number:{exc_tb.tb_lineno}."
+            print(error_string)
+    else:
+        print(f"Direction input must be 1 or -1 but input is {direction_input}")
+        replace_successful = False
 
-        new_destination_file.close()
+    return replace_successful
 
 
+# This function is to change the direction of given csv file and rerun csv updating and okn detecting
 def change_direction_and_rerun(csv_file_input, direction_input, extra_string_input, updater_config_input,
                                detector_config_input, detector_location_input):
     success = True
     error_string = None
+    result_folder_dir = None
     try:
-        replace_with_new_direction(csv_file_input, direction_input)
-        updated_file, output_file_location, success, error = update_csv(csv_file_input,
-                                                                        extra_string_input,
-                                                                        updater_config_input)
-        updated_file_dir = os.path.join(output_file_location, updated_file)
-        result_folder_dir = detect_with_okn_detector(updated_file_dir, detector_config_input, detector_location_input)
+        replace_successful = replace_with_new_direction(csv_file_input, direction_input)
+        if replace_successful:
+            updated_file, output_file_location, success, error = update_csv(csv_file_input,
+                                                                            extra_string_input,
+                                                                            updater_config_input)
+            updated_file_dir = os.path.join(output_file_location, updated_file)
+            result_folder_dir = detect_with_okn_detector(updated_file_dir, detector_config_input,
+                                                         detector_location_input)
+        else:
+            print("okntool could not finish \"change_direction_and_rerun\" process because of error or invalid "
+                  "direction input.")
+            success = False
     except Exception as error:
         success = False
         exc_type, exc_obj, exc_tb = sys.exc_info()
         error_string = f"Error occurred:error type:{type(error).__name__} in line number:{exc_tb.tb_lineno}."
         result_folder_dir = None
 
     return result_folder_dir, success, error_string
@@ -719,16 +741,16 @@
 
 def main():
     parser = argparse.ArgumentParser(prog='oknpatch',
                                      description='OKNPATCH package.')
     # parser.add_argument("oknpatch -t trial_data_lost -i csv_to_be_fixed -gi gaze_csv_to_be_referenced")
     # parser.add_argument("oknpatch -t update -i csv_to_be_updated [-es extra_string] [-uc updater_config]")
     # parser.add_argument("oknpatch -t change_direction_and_rerun -i csv_to_be_fixed -di direction_input [-es "
-    #                     "extra_string] [-uc updater_config] [-okndc okn_detector_config] -okndl okn_detector_location")
-    parser.add_argument('--version', action='version', version='3.0.0'),
+    # "extra_string] [-uc updater_config] [-okndc okn_detector_config] -okndl okn_detector_location")
+    parser.add_argument('--version', action='version', version='3.0.1'),
     parser.add_argument("-t", dest="type_input", required=True, default=sys.stdin,
                         help="issue type to fix", metavar="issue type")
     parser.add_argument("-i", dest="input_file", required=False, default=sys.stdin,
                         metavar="input file to be fixed or updated")
     parser.add_argument("-gi", dest="gaze_input", required=False, default=sys.stdin,
                         metavar="gaze file to be referenced")
     parser.add_argument("-es", dest="extra_string", required=False, default=sys.stdin,
@@ -861,24 +883,24 @@
             else:
                 extra_string = "updated_"
                 print(f"There is no extra string input. Therefore using default extra string:{extra_string}")
             # Determine whether build-in updater config or input updater config needs to be used
             if updater_config_exist:
                 config_dir_exist = os.path.isfile(updater_config)
                 if config_dir_exist:
-                    print("Input updater config location is found.")
+                    print("Input for okn detecting config location is found.")
                     updater_config_location = updater_config
                 else:
-                    print("Input updater config does not exist.")
+                    print("Input for okn detecting config does not exist.")
                     updater_config_location = get_config_location("oknpatch", "gazefilters.json")
-                    print(f"Therefore using default updater config from package.")
+                    print(f"Therefore using default okn detecting config from package.")
             else:
-                print("There is no update config location input.")
+                print("Input for okn detecting config location is not found.")
                 updater_config_location = get_config_location("oknpatch", "gazefilters.json")
-                print(f"Therefore using default updater config from package.")
+                print(f"Therefore using default okn detecting config from package.")
             if okn_detector_config_exist:
                 okn_detector_config_dir_exist = os.path.isfile(okn_detector_config)
                 if okn_detector_config_dir_exist:
                     print("Input updater config location is found.")
                     okn_detector_config_location = updater_config
                 else:
                     print("Input updater config does not exist.")
@@ -891,15 +913,17 @@
             result_folder_dir, success, error = change_direction_and_rerun(input_file, direction_input,
                                                                            extra_string, updater_config_location,
                                                                            okn_detector_config_location,
                                                                            okn_detector_location)
             if success:
                 print(f"Rerunning is successful and result folder is created in {result_folder_dir}.")
             else:
-                print(error)
+                print(f"Rerunning is unsuccessful.")
+                if error:
+                    print(error)
         else:
             if not input_file_exist and not direction_input_exist:
                 print("")
                 print(f"Necessary arguments are missing to run oknpatch:{type_input}.")
                 print("Example Usage:")
                 print("oknpatch -t change_direction_and_rerun -i csv_to_be_fixed -di direction_input [-es "
                       "extra_string] [-uc updater_config] [-okndc okn_config] -okndl okn_location")
```

### Comparing `oknpatch-3.0.0/oknpatch.egg-info/PKG-INFO` & `oknpatch-3.0.1/oknpatch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oknpatch
-Version: 3.0.0
+Version: 3.0.1
 Summary: issues fixing program
 Home-page: https://github.com/jtur044/oknpatch
 Author: Zaw Lin Tun
 Author-email: zawlintun1511@gmail.com
 License: Apache Software
 Keywords: oknpatch
 Classifier: Programming Language :: Python :: 3
```

### Comparing `oknpatch-3.0.0/setup.py` & `oknpatch-3.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('requirements.txt') as f:
     requirements = f.readlines()
 
 long_description = 'Command line program to fix okn and pim related issues.'
 
 setup(
     name='oknpatch',
-    version='3.0.0',
+    version='3.0.1',
     author='Zaw Lin Tun',
     author_email='zawlintun1511@gmail.com',
     url='https://github.com/jtur044/oknpatch',
     description='issues fixing program',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Apache Software",
```

