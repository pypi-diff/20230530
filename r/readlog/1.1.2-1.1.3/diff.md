# Comparing `tmp/readlog-1.1.2.tar.gz` & `tmp/readlog-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readlog-1.1.2.tar", last modified: Tue May 30 16:07:11 2023, max compression
+gzip compressed data, was "readlog-1.1.3.tar", last modified: Tue May 30 16:27:25 2023, max compression
```

## Comparing `readlog-1.1.2.tar` & `readlog-1.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 16:07:11.531870 readlog-1.1.2/
--rw-rw-rw-   0        0        0      821 2023-05-30 16:07:11.530870 readlog-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      553 2023-05-30 14:22:34.000000 readlog-1.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-30 16:07:11.532870 readlog-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      758 2023-05-30 16:06:32.000000 readlog-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 16:07:11.513871 readlog-1.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-30 16:07:11.527865 readlog-1.1.2/src/readlog.egg-info/
--rw-rw-rw-   0        0        0      821 2023-05-30 16:07:11.000000 readlog-1.1.2/src/readlog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-05-30 16:07:11.000000 readlog-1.1.2/src/readlog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 16:07:11.000000 readlog-1.1.2/src/readlog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-30 16:07:11.000000 readlog-1.1.2/src/readlog.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-30 16:07:11.000000 readlog-1.1.2/src/readlog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3029 2023-05-30 13:09:29.000000 readlog-1.1.2/src/readlog.py
+drwxrwxrwx   0        0        0        0 2023-05-30 16:27:25.271020 readlog-1.1.3/
+-rw-rw-rw-   0        0        0      823 2023-05-30 16:27:25.269018 readlog-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      555 2023-05-30 16:19:07.000000 readlog-1.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-30 16:27:25.271020 readlog-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      775 2023-05-30 16:27:13.000000 readlog-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 16:27:25.252026 readlog-1.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-30 16:27:25.266034 readlog-1.1.3/src/readlog.egg-info/
+-rw-rw-rw-   0        0        0      823 2023-05-30 16:27:24.000000 readlog-1.1.3/src/readlog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2023-05-30 16:27:25.000000 readlog-1.1.3/src/readlog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 16:27:24.000000 readlog-1.1.3/src/readlog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-30 16:27:24.000000 readlog-1.1.3/src/readlog.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-30 16:27:24.000000 readlog-1.1.3/src/readlog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3029 2023-05-30 13:09:29.000000 readlog-1.1.3/src/readlog.py
```

### Comparing `readlog-1.1.2/PKG-INFO` & `readlog-1.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readlog
-Version: 1.1.2
+Version: 1.1.3
 Summary: Read themo info from lammps output file or log file
 Home-page: https://github.com/eastsheng/readlog
 Author: CHENDONGSHENG
 Author-email: eastsheng@hotmail.com
 Description-Content-Type: text/markdown
 
 ## ReadLog
@@ -28,13 +28,13 @@
 
 ### Usage 
 
 ```python
 import readlog as RLog
 rl = RLog.ReadLog(logfile)
 thermou_list,thermod_list = rl.ReadUD(path+logfile)
-pd_thermo = rl.ReadThermo(path+logfile,thermou_list,thermod_list,nf_log)
+pd_thermo = rl.ReadThermo(path+logfile,thermou_list,thermod_list,nf_log=0)
 step = pd_thermo["Step"]
 P = pd_thermo["Press"]
 T = pd_thermo["Temp"]
 ```
```

### Comparing `readlog-1.1.2/README.md` & `readlog-1.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,13 +19,13 @@
 
 ### Usage 
 
 ```python
 import readlog as RLog
 rl = RLog.ReadLog(logfile)
 thermou_list,thermod_list = rl.ReadUD(path+logfile)
-pd_thermo = rl.ReadThermo(path+logfile,thermou_list,thermod_list,nf_log)
+pd_thermo = rl.ReadThermo(path+logfile,thermou_list,thermod_list,nf_log=0)
 step = pd_thermo["Step"]
 P = pd_thermo["Press"]
 T = pd_thermo["Temp"]
 ```
```

### Comparing `readlog-1.1.2/setup.py` & `readlog-1.1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 
 # from distutils.core import setup
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
-with open("requirements.txt","r") as f:
+with open("src/readlog.egg-info/requires.txt","r") as f:
     required = f.read().splitlines()
 
 
 setup(
 name         = 'readlog',
-version      = '1.1.2',
+version      = '1.1.3',
 py_modules   = ['readlog'],
 author       = 'CHENDONGSHENG',
 author_email = 'eastsheng@hotmail.com',
 packages=find_packages('src'),
 package_dir={'': 'src'},
 install_requires=required,
 url          = 'https://github.com/eastsheng/readlog',
```

### Comparing `readlog-1.1.2/src/readlog.egg-info/PKG-INFO` & `readlog-1.1.3/src/readlog.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readlog
-Version: 1.1.2
+Version: 1.1.3
 Summary: Read themo info from lammps output file or log file
 Home-page: https://github.com/eastsheng/readlog
 Author: CHENDONGSHENG
 Author-email: eastsheng@hotmail.com
 Description-Content-Type: text/markdown
 
 ## ReadLog
@@ -28,13 +28,13 @@
 
 ### Usage 
 
 ```python
 import readlog as RLog
 rl = RLog.ReadLog(logfile)
 thermou_list,thermod_list = rl.ReadUD(path+logfile)
-pd_thermo = rl.ReadThermo(path+logfile,thermou_list,thermod_list,nf_log)
+pd_thermo = rl.ReadThermo(path+logfile,thermou_list,thermod_list,nf_log=0)
 step = pd_thermo["Step"]
 P = pd_thermo["Press"]
 T = pd_thermo["Temp"]
 ```
```

### Comparing `readlog-1.1.2/src/readlog.py` & `readlog-1.1.3/src/readlog.py`

 * *Files identical despite different names*

