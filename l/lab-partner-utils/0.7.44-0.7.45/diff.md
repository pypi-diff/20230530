# Comparing `tmp/lab-partner-utils-0.7.44.tar.gz` & `tmp/lab-partner-utils-0.7.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lab-partner-utils-0.7.44.tar", last modified: Mon May 29 23:28:49 2023, max compression
+gzip compressed data, was "lab-partner-utils-0.7.45.tar", last modified: Tue May 30 00:35:23 2023, max compression
```

## Comparing `lab-partner-utils-0.7.44.tar` & `lab-partner-utils-0.7.45.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 23:28:49.823373 lab-partner-utils-0.7.44/
--rw-r--r--   0 root         (0) root         (0)     1094 2023-05-29 23:28:12.000000 lab-partner-utils-0.7.44/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     2011 2023-05-29 23:28:49.823373 lab-partner-utils-0.7.44/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-29 23:28:12.000000 lab-partner-utils-0.7.44/README.md
--rw-r--r--   0 root         (0) root         (0)     1744 2023-05-29 23:28:43.000000 lab-partner-utils-0.7.44/pyproject.toml
--rwxr-xr-x   0 root         (0) root         (0)      253 2023-05-29 23:28:12.000000 lab-partner-utils-0.7.44/run.sh
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 23:28:49.823373 lab-partner-utils-0.7.44/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 23:28:49.819373 lab-partner-utils-0.7.44/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 23:28:49.823373 lab-partner-utils-0.7.44/src/lab_partner_utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 23:28:12.000000 lab-partner-utils-0.7.44/src/lab_partner_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8251 2023-05-29 23:28:12.000000 lab-partner-utils-0.7.44/src/lab_partner_utils/cli_command_factory.py
--rw-r--r--   0 root         (0) root         (0)     1706 2023-05-29 23:28:12.000000 lab-partner-utils-0.7.44/src/lab_partner_utils/command_builder.py
--rwxr-xr-x   0 root         (0) root         (0)     7252 2023-05-29 23:28:12.000000 lab-partner-utils-0.7.44/src/lab_partner_utils/commands.py
--rw-r--r--   0 root         (0) root         (0)     1164 2023-05-29 23:28:12.000000 lab-partner-utils-0.7.44/src/lab_partner_utils/kernel_launcher.py
--rw-r--r--   0 root         (0) root         (0)    13028 2023-05-29 23:28:12.000000 lab-partner-utils-0.7.44/src/lab_partner_utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 23:28:49.823373 lab-partner-utils-0.7.44/src/lab_partner_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2011 2023-05-29 23:28:49.000000 lab-partner-utils-0.7.44/src/lab_partner_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      540 2023-05-29 23:28:49.000000 lab-partner-utils-0.7.44/src/lab_partner_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 23:28:49.000000 lab-partner-utils-0.7.44/src/lab_partner_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      123 2023-05-29 23:28:49.000000 lab-partner-utils-0.7.44/src/lab_partner_utils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      210 2023-05-29 23:28:49.000000 lab-partner-utils-0.7.44/src/lab_partner_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-29 23:28:49.000000 lab-partner-utils-0.7.44/src/lab_partner_utils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:35:23.623244 lab-partner-utils-0.7.45/
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-05-30 00:34:39.000000 lab-partner-utils-0.7.45/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     2011 2023-05-30 00:35:23.623244 lab-partner-utils-0.7.45/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-30 00:34:39.000000 lab-partner-utils-0.7.45/README.md
+-rw-r--r--   0 root         (0) root         (0)     1744 2023-05-30 00:35:16.000000 lab-partner-utils-0.7.45/pyproject.toml
+-rwxr-xr-x   0 root         (0) root         (0)      253 2023-05-30 00:34:39.000000 lab-partner-utils-0.7.45/run.sh
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 00:35:23.623244 lab-partner-utils-0.7.45/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:35:23.619244 lab-partner-utils-0.7.45/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:35:23.623244 lab-partner-utils-0.7.45/src/lab_partner_utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 00:34:39.000000 lab-partner-utils-0.7.45/src/lab_partner_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8251 2023-05-30 00:34:39.000000 lab-partner-utils-0.7.45/src/lab_partner_utils/cli_command_factory.py
+-rw-r--r--   0 root         (0) root         (0)     1706 2023-05-30 00:34:39.000000 lab-partner-utils-0.7.45/src/lab_partner_utils/command_builder.py
+-rwxr-xr-x   0 root         (0) root         (0)     7252 2023-05-30 00:34:39.000000 lab-partner-utils-0.7.45/src/lab_partner_utils/commands.py
+-rw-r--r--   0 root         (0) root         (0)     1164 2023-05-30 00:34:39.000000 lab-partner-utils-0.7.45/src/lab_partner_utils/kernel_launcher.py
+-rw-r--r--   0 root         (0) root         (0)    13028 2023-05-30 00:34:39.000000 lab-partner-utils-0.7.45/src/lab_partner_utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 00:35:23.623244 lab-partner-utils-0.7.45/src/lab_partner_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2011 2023-05-30 00:35:23.000000 lab-partner-utils-0.7.45/src/lab_partner_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      540 2023-05-30 00:35:23.000000 lab-partner-utils-0.7.45/src/lab_partner_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 00:35:23.000000 lab-partner-utils-0.7.45/src/lab_partner_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      123 2023-05-30 00:35:23.000000 lab-partner-utils-0.7.45/src/lab_partner_utils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      210 2023-05-30 00:35:23.000000 lab-partner-utils-0.7.45/src/lab_partner_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-30 00:35:23.000000 lab-partner-utils-0.7.45/src/lab_partner_utils.egg-info/top_level.txt
```

### Comparing `lab-partner-utils-0.7.44/LICENSE.md` & `lab-partner-utils-0.7.45/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.44/PKG-INFO` & `lab-partner-utils-0.7.45/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lab-partner-utils
-Version: 0.7.44
+Version: 0.7.45
 Summary: Utilities used to embed Lab Partner into python projects
 Author-email: Anthony Schexnaildre <aps@enclarify.com>
 Maintainer-email: Anthony Schexnaildre <aps@enclarify.com>
 License: # Released under MIT License
         
         Copyright (c) 2021 Anthony Schexnaildre.
```

### Comparing `lab-partner-utils-0.7.44/pyproject.toml` & `lab-partner-utils-0.7.45/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=45", "wheel", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lab-partner-utils"
-version = "0.7.44"
+version = "0.7.45"
 description = "Utilities used to embed Lab Partner into python projects"
 dynamic = ["readme"]
 #dynamic = ["version", "readme"]
 authors = [
     {name = "Anthony Schexnaildre", email = "aps@enclarify.com"},
 ]
 maintainers = [
```

### Comparing `lab-partner-utils-0.7.44/src/lab_partner_utils/cli_command_factory.py` & `lab-partner-utils-0.7.45/src/lab_partner_utils/cli_command_factory.py`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.44/src/lab_partner_utils/command_builder.py` & `lab-partner-utils-0.7.45/src/lab_partner_utils/command_builder.py`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.44/src/lab_partner_utils/commands.py` & `lab-partner-utils-0.7.45/src/lab_partner_utils/commands.py`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.44/src/lab_partner_utils/kernel_launcher.py` & `lab-partner-utils-0.7.45/src/lab_partner_utils/kernel_launcher.py`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.44/src/lab_partner_utils/utils.py` & `lab-partner-utils-0.7.45/src/lab_partner_utils/utils.py`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.44/src/lab_partner_utils.egg-info/PKG-INFO` & `lab-partner-utils-0.7.45/src/lab_partner_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lab-partner-utils
-Version: 0.7.44
+Version: 0.7.45
 Summary: Utilities used to embed Lab Partner into python projects
 Author-email: Anthony Schexnaildre <aps@enclarify.com>
 Maintainer-email: Anthony Schexnaildre <aps@enclarify.com>
 License: # Released under MIT License
         
         Copyright (c) 2021 Anthony Schexnaildre.
```

### Comparing `lab-partner-utils-0.7.44/src/lab_partner_utils.egg-info/SOURCES.txt` & `lab-partner-utils-0.7.45/src/lab_partner_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

