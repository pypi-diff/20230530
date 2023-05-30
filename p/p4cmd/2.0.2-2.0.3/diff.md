# Comparing `tmp/p4cmd-2.0.2.tar.gz` & `tmp/p4cmd-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p4cmd-2.0.2.tar", last modified: Wed Mar  8 14:03:13 2023, max compression
+gzip compressed data, was "p4cmd-2.0.3.tar", last modified: Tue May 30 08:54:16 2023, max compression
```

## Comparing `p4cmd-2.0.2.tar` & `p4cmd-2.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 14:03:13.696273 p4cmd-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-08 14:03:05.000000 p4cmd-2.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-03-08 14:03:13.696273 p4cmd-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-03-08 14:03:05.000000 p4cmd-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 14:03:13.692273 p4cmd-2.0.2/p4cmd/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-08 14:03:05.000000 p4cmd-2.0.2/p4cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37987 2023-03-08 14:03:05.000000 p4cmd-2.0.2/p4cmd/p4cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-08 14:03:05.000000 p4cmd-2.0.2/p4cmd/p4errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-03-08 14:03:05.000000 p4cmd-2.0.2/p4cmd/p4file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 14:03:13.696273 p4cmd-2.0.2/p4cmd/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-03-08 14:03:05.000000 p4cmd-2.0.2/p4cmd/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-03-08 14:03:05.000000 p4cmd-2.0.2/p4cmd/resources/perforce_DEPOT_ONLY.png
--rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-03-08 14:03:05.000000 p4cmd-2.0.2/p4cmd/resources/perforce_MOVED.png
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-03-08 14:03:05.000000 p4cmd-2.0.2/p4cmd/resources/perforce_NEED_SYNC.png
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-03-08 14:03:05.000000 p4cmd-2.0.2/p4cmd/resources/perforce_OPEN_FOR_ADD.png
--rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-03-08 14:03:05.000000 p4cmd-2.0.2/p4cmd/resources/perforce_OPEN_FOR_DELETE.png
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-03-08 14:03:05.000000 p4cmd-2.0.2/p4cmd/resources/perforce_OPEN_FOR_EDIT.png
--rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-03-08 14:03:05.000000 p4cmd-2.0.2/p4cmd/resources/perforce_UNKNOWN.png
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-03-08 14:03:05.000000 p4cmd-2.0.2/p4cmd/resources/perforce_UNTRACKED.png
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-03-08 14:03:05.000000 p4cmd-2.0.2/p4cmd/resources/perforce_UP_TO_DATE.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 14:03:13.692273 p4cmd-2.0.2/p4cmd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-03-08 14:03:13.000000 p4cmd-2.0.2/p4cmd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-08 14:03:13.000000 p4cmd-2.0.2/p4cmd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 14:03:13.000000 p4cmd-2.0.2/p4cmd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-08 14:03:13.000000 p4cmd-2.0.2/p4cmd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-08 14:03:13.696273 p4cmd-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-03-08 14:03:05.000000 p4cmd-2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:54:16.028565 p4cmd-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-30 08:54:05.000000 p4cmd-2.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-05-30 08:54:16.028565 p4cmd-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-05-30 08:54:05.000000 p4cmd-2.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:54:16.028565 p4cmd-2.0.3/p4cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-30 08:54:05.000000 p4cmd-2.0.3/p4cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38317 2023-05-30 08:54:05.000000 p4cmd-2.0.3/p4cmd/p4cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-30 08:54:05.000000 p4cmd-2.0.3/p4cmd/p4errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-05-30 08:54:05.000000 p4cmd-2.0.3/p4cmd/p4file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:54:16.028565 p4cmd-2.0.3/p4cmd/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-30 08:54:05.000000 p4cmd-2.0.3/p4cmd/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-05-30 08:54:05.000000 p4cmd-2.0.3/p4cmd/resources/perforce_DEPOT_ONLY.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-05-30 08:54:05.000000 p4cmd-2.0.3/p4cmd/resources/perforce_MOVED.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-05-30 08:54:05.000000 p4cmd-2.0.3/p4cmd/resources/perforce_NEED_SYNC.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-05-30 08:54:05.000000 p4cmd-2.0.3/p4cmd/resources/perforce_OPEN_FOR_ADD.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5952 2023-05-30 08:54:05.000000 p4cmd-2.0.3/p4cmd/resources/perforce_OPEN_FOR_DELETE.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-05-30 08:54:05.000000 p4cmd-2.0.3/p4cmd/resources/perforce_OPEN_FOR_EDIT.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-05-30 08:54:05.000000 p4cmd-2.0.3/p4cmd/resources/perforce_UNKNOWN.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-30 08:54:05.000000 p4cmd-2.0.3/p4cmd/resources/perforce_UNTRACKED.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-05-30 08:54:05.000000 p4cmd-2.0.3/p4cmd/resources/perforce_UP_TO_DATE.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:54:16.028565 p4cmd-2.0.3/p4cmd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-05-30 08:54:15.000000 p4cmd-2.0.3/p4cmd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-30 08:54:16.000000 p4cmd-2.0.3/p4cmd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 08:54:15.000000 p4cmd-2.0.3/p4cmd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 08:54:15.000000 p4cmd-2.0.3/p4cmd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 08:54:16.028565 p4cmd-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-30 08:54:05.000000 p4cmd-2.0.3/setup.py
```

### Comparing `p4cmd-2.0.2/LICENSE` & `p4cmd-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `p4cmd-2.0.2/PKG-INFO` & `p4cmd-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p4cmd
-Version: 2.0.2
+Version: 2.0.3
 Summary: Simple P4 python module
 Home-page: https://github.com/nielsvaes/p4cmd
 Author: Niels Vaes
 Author-email: nielsvaes@gmail.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `p4cmd-2.0.2/README.md` & `p4cmd-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `p4cmd-2.0.2/p4cmd/p4cmd.py` & `p4cmd-2.0.3/p4cmd/p4cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -850,14 +850,19 @@
 
             opened_by = []
             for key, value in file_dict.items():
                 other_open = "otherOpen" if sys.version_info.major == 2 else "otherOpen".encode()
                 if other_open in key and key != other_open:
                     value = self.__get_dict_value(file_dict, key)
                     opened_by.append(value)
+                action_owner = "actionOwner" if sys.version_info == 2 else "actionOwner".encode()
+                if action_owner in key:
+                    value = self.__get_dict_value(file_dict, key)
+                    value = value.decode() + "@" + self.find_p4_client()
+                    opened_by.append(value.encode())
 
             p4file.set_checked_out_by(opened_by)
 
             if allow_invalid_files:
                 p4files.append(p4file)
             else:
                 if p4file.is_valid():
```

### Comparing `p4cmd-2.0.2/p4cmd/p4file.py` & `p4cmd-2.0.3/p4cmd/p4file.py`

 * *Files identical despite different names*

### Comparing `p4cmd-2.0.2/p4cmd/resources/__init__.py` & `p4cmd-2.0.3/p4cmd/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `p4cmd-2.0.2/p4cmd/resources/perforce_DEPOT_ONLY.png` & `p4cmd-2.0.3/p4cmd/resources/perforce_DEPOT_ONLY.png`

 * *Files identical despite different names*

### Comparing `p4cmd-2.0.2/p4cmd/resources/perforce_MOVED.png` & `p4cmd-2.0.3/p4cmd/resources/perforce_MOVED.png`

 * *Files identical despite different names*

### Comparing `p4cmd-2.0.2/p4cmd/resources/perforce_NEED_SYNC.png` & `p4cmd-2.0.3/p4cmd/resources/perforce_NEED_SYNC.png`

 * *Files identical despite different names*

### Comparing `p4cmd-2.0.2/p4cmd/resources/perforce_OPEN_FOR_ADD.png` & `p4cmd-2.0.3/p4cmd/resources/perforce_OPEN_FOR_ADD.png`

 * *Files identical despite different names*

### Comparing `p4cmd-2.0.2/p4cmd/resources/perforce_OPEN_FOR_DELETE.png` & `p4cmd-2.0.3/p4cmd/resources/perforce_OPEN_FOR_DELETE.png`

 * *Files identical despite different names*

### Comparing `p4cmd-2.0.2/p4cmd/resources/perforce_OPEN_FOR_EDIT.png` & `p4cmd-2.0.3/p4cmd/resources/perforce_OPEN_FOR_EDIT.png`

 * *Files identical despite different names*

### Comparing `p4cmd-2.0.2/p4cmd/resources/perforce_UNKNOWN.png` & `p4cmd-2.0.3/p4cmd/resources/perforce_UNKNOWN.png`

 * *Files identical despite different names*

### Comparing `p4cmd-2.0.2/p4cmd/resources/perforce_UNTRACKED.png` & `p4cmd-2.0.3/p4cmd/resources/perforce_UNTRACKED.png`

 * *Files identical despite different names*

### Comparing `p4cmd-2.0.2/p4cmd/resources/perforce_UP_TO_DATE.png` & `p4cmd-2.0.3/p4cmd/resources/perforce_UP_TO_DATE.png`

 * *Files identical despite different names*

### Comparing `p4cmd-2.0.2/p4cmd.egg-info/PKG-INFO` & `p4cmd-2.0.3/p4cmd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p4cmd
-Version: 2.0.2
+Version: 2.0.3
 Summary: Simple P4 python module
 Home-page: https://github.com/nielsvaes/p4cmd
 Author: Niels Vaes
 Author-email: nielsvaes@gmail.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `p4cmd-2.0.2/p4cmd.egg-info/SOURCES.txt` & `p4cmd-2.0.3/p4cmd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `p4cmd-2.0.2/setup.py` & `p4cmd-2.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 data_files_to_include = ["*.png"]
 
 setuptools.setup(
     name="p4cmd",
-    version="2.0.2",
+    version="2.0.3",
     author="Niels Vaes",
     license='MIT',
     author_email="nielsvaes@gmail.com",
     description="Simple P4 python module",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nielsvaes/p4cmd",
```

