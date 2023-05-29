# Comparing `tmp/abdal_net_py-2.6.tar.gz` & `tmp/abdal_net_py-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abdal_net_py-2.6.tar", last modified: Mon May 29 22:47:19 2023, max compression
+gzip compressed data, was "abdal_net_py-2.7.tar", last modified: Mon May 29 22:55:00 2023, max compression
```

## Comparing `abdal_net_py-2.6.tar` & `abdal_net_py-2.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 22:47:19.728202 abdal_net_py-2.6/
--rw-rw-rw-   0        0        0     1098 2023-05-29 20:51:23.000000 abdal_net_py-2.6/LICENSE
--rw-rw-rw-   0        0        0     2572 2023-05-29 22:47:19.728202 abdal_net_py-2.6/PKG-INFO
--rw-rw-rw-   0        0        0     1541 2023-05-29 22:02:04.000000 abdal_net_py-2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 22:47:19.711191 abdal_net_py-2.6/abdal_net_py/
--rw-rw-rw-   0        0        0      145 2023-05-29 20:51:23.000000 abdal_net_py-2.6/abdal_net_py/__init__.py
--rw-rw-rw-   0        0        0      531 2023-05-29 20:51:23.000000 abdal_net_py-2.6/abdal_net_py/abdal_net_py_about.py
--rw-rw-rw-   0        0        0      661 2023-05-29 21:39:00.000000 abdal_net_py-2.6/abdal_net_py/abdal_net_py_admin.py
--rw-rw-rw-   0        0        0      951 2023-05-29 20:51:23.000000 abdal_net_py-2.6/abdal_net_py/abdal_net_py_generator.py
--rw-rw-rw-   0        0        0     1340 2023-05-29 20:51:23.000000 abdal_net_py-2.6/abdal_net_py/abdal_net_py_loger.py
--rw-rw-rw-   0        0        0     1150 2023-05-29 20:51:23.000000 abdal_net_py-2.6/abdal_net_py/abdal_net_py_unit.py
-drwxrwxrwx   0        0        0        0 2023-05-29 22:47:19.725199 abdal_net_py-2.6/abdal_net_py.egg-info/
--rw-rw-rw-   0        0        0     2572 2023-05-29 22:47:19.000000 abdal_net_py-2.6/abdal_net_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      433 2023-05-29 22:47:19.000000 abdal_net_py-2.6/abdal_net_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 22:47:19.000000 abdal_net_py-2.6/abdal_net_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-29 22:47:19.000000 abdal_net_py-2.6/abdal_net_py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-29 22:47:19.000000 abdal_net_py-2.6/abdal_net_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-05-29 20:51:23.000000 abdal_net_py-2.6/pyproject.toml
--rw-rw-rw-   0        0        0      140 2023-05-29 22:47:19.730191 abdal_net_py-2.6/setup.cfg
--rw-rw-rw-   0        0        0     1469 2023-05-29 22:06:17.000000 abdal_net_py-2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 22:55:00.287481 abdal_net_py-2.7/
+-rw-rw-rw-   0        0        0     1098 2023-05-29 20:51:23.000000 abdal_net_py-2.7/LICENSE
+-rw-rw-rw-   0        0        0     2572 2023-05-29 22:55:00.287481 abdal_net_py-2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1541 2023-05-29 22:02:04.000000 abdal_net_py-2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 22:55:00.271472 abdal_net_py-2.7/abdal_net_py/
+-rw-rw-rw-   0        0        0      180 2023-05-29 22:54:35.000000 abdal_net_py-2.7/abdal_net_py/__init__.py
+-rw-rw-rw-   0        0        0      531 2023-05-29 20:51:23.000000 abdal_net_py-2.7/abdal_net_py/abdal_net_py_about.py
+-rw-rw-rw-   0        0        0      661 2023-05-29 21:39:00.000000 abdal_net_py-2.7/abdal_net_py/abdal_net_py_admin.py
+-rw-rw-rw-   0        0        0      951 2023-05-29 20:51:23.000000 abdal_net_py-2.7/abdal_net_py/abdal_net_py_generator.py
+-rw-rw-rw-   0        0        0     1340 2023-05-29 20:51:23.000000 abdal_net_py-2.7/abdal_net_py/abdal_net_py_loger.py
+-rw-rw-rw-   0        0        0     1150 2023-05-29 20:51:23.000000 abdal_net_py-2.7/abdal_net_py/abdal_net_py_unit.py
+drwxrwxrwx   0        0        0        0 2023-05-29 22:55:00.284482 abdal_net_py-2.7/abdal_net_py.egg-info/
+-rw-rw-rw-   0        0        0     2572 2023-05-29 22:55:00.000000 abdal_net_py-2.7/abdal_net_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2023-05-29 22:55:00.000000 abdal_net_py-2.7/abdal_net_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 22:55:00.000000 abdal_net_py-2.7/abdal_net_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-29 22:55:00.000000 abdal_net_py-2.7/abdal_net_py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-29 22:55:00.000000 abdal_net_py-2.7/abdal_net_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-05-29 20:51:23.000000 abdal_net_py-2.7/pyproject.toml
+-rw-rw-rw-   0        0        0      140 2023-05-29 22:55:00.289472 abdal_net_py-2.7/setup.cfg
+-rw-rw-rw-   0        0        0     1469 2023-05-29 22:54:41.000000 abdal_net_py-2.7/setup.py
```

### Comparing `abdal_net_py-2.6/LICENSE` & `abdal_net_py-2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `abdal_net_py-2.6/PKG-INFO` & `abdal_net_py-2.7/abdal_net_py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: abdal_net_py
-Version: 2.6
+Name: abdal-net-py
+Version: 2.7
 Summary: Powerful security network package
 Home-page: https://github.com/abdal-security-group/abdal-net-py
 Author: Ebrahim Shafiei (EbraSha)
 Author-email: Prof.Shafiei@Gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/abdal-security-group/abdal-net-py/issues
 Keywords: python,security,hack,network,camera stream,sockets
```

### Comparing `abdal_net_py-2.6/README.md` & `abdal_net_py-2.7/README.md`

 * *Files identical despite different names*

### Comparing `abdal_net_py-2.6/abdal_net_py/abdal_net_py_about.py` & `abdal_net_py-2.7/abdal_net_py/abdal_net_py_about.py`

 * *Files identical despite different names*

### Comparing `abdal_net_py-2.6/abdal_net_py/abdal_net_py_admin.py` & `abdal_net_py-2.7/abdal_net_py/abdal_net_py_admin.py`

 * *Files identical despite different names*

### Comparing `abdal_net_py-2.6/abdal_net_py/abdal_net_py_generator.py` & `abdal_net_py-2.7/abdal_net_py/abdal_net_py_generator.py`

 * *Files identical despite different names*

### Comparing `abdal_net_py-2.6/abdal_net_py/abdal_net_py_loger.py` & `abdal_net_py-2.7/abdal_net_py/abdal_net_py_loger.py`

 * *Files identical despite different names*

### Comparing `abdal_net_py-2.6/abdal_net_py/abdal_net_py_unit.py` & `abdal_net_py-2.7/abdal_net_py/abdal_net_py_unit.py`

 * *Files identical despite different names*

### Comparing `abdal_net_py-2.6/abdal_net_py.egg-info/PKG-INFO` & `abdal_net_py-2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: abdal-net-py
-Version: 2.6
+Name: abdal_net_py
+Version: 2.7
 Summary: Powerful security network package
 Home-page: https://github.com/abdal-security-group/abdal-net-py
 Author: Ebrahim Shafiei (EbraSha)
 Author-email: Prof.Shafiei@Gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/abdal-security-group/abdal-net-py/issues
 Keywords: python,security,hack,network,camera stream,sockets
```

### Comparing `abdal_net_py-2.6/setup.py` & `abdal_net_py-2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "2.6"
+VERSION = "2.7"
 DESCRIPTION = 'Powerful security network package'
 LONG_DESCRIPTION = 'Powerful security network package for hackers and all security experts'
 
 # Setting up
 setup(
     name="abdal_net_py",
     version=VERSION,
```

