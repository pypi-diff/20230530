# Comparing `tmp/readlog-1.1.1.tar.gz` & `tmp/readlog-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readlog-1.1.1.tar", last modified: Tue May 30 15:54:11 2023, max compression
+gzip compressed data, was "readlog-1.1.2.tar", last modified: Tue May 30 16:07:11 2023, max compression
```

## Comparing `readlog-1.1.1.tar` & `readlog-1.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 15:54:11.010317 readlog-1.1.1/
--rw-rw-rw-   0        0        0      780 2023-05-30 15:54:11.009331 readlog-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      553 2023-05-30 14:22:34.000000 readlog-1.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-30 15:54:11.010317 readlog-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      710 2023-05-30 15:54:05.000000 readlog-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-30 15:54:10.992328 readlog-1.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-30 15:54:11.006322 readlog-1.1.1/src/readlog.egg-info/
--rw-rw-rw-   0        0        0      780 2023-05-30 15:54:10.000000 readlog-1.1.1/src/readlog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-05-30 15:54:10.000000 readlog-1.1.1/src/readlog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 15:54:10.000000 readlog-1.1.1/src/readlog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-30 15:54:10.000000 readlog-1.1.1/src/readlog.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-30 15:54:10.000000 readlog-1.1.1/src/readlog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3029 2023-05-30 13:09:29.000000 readlog-1.1.1/src/readlog.py
+drwxrwxrwx   0        0        0        0 2023-05-30 16:07:11.531870 readlog-1.1.2/
+-rw-rw-rw-   0        0        0      821 2023-05-30 16:07:11.530870 readlog-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      553 2023-05-30 14:22:34.000000 readlog-1.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-30 16:07:11.532870 readlog-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      758 2023-05-30 16:06:32.000000 readlog-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 16:07:11.513871 readlog-1.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-30 16:07:11.527865 readlog-1.1.2/src/readlog.egg-info/
+-rw-rw-rw-   0        0        0      821 2023-05-30 16:07:11.000000 readlog-1.1.2/src/readlog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2023-05-30 16:07:11.000000 readlog-1.1.2/src/readlog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 16:07:11.000000 readlog-1.1.2/src/readlog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-30 16:07:11.000000 readlog-1.1.2/src/readlog.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-30 16:07:11.000000 readlog-1.1.2/src/readlog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3029 2023-05-30 13:09:29.000000 readlog-1.1.2/src/readlog.py
```

### Comparing `readlog-1.1.1/PKG-INFO` & `readlog-1.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: readlog
-Version: 1.1.1
+Version: 1.1.2
 Summary: Read themo info from lammps output file or log file
 Home-page: https://github.com/eastsheng/readlog
 Author: CHENDONGSHENG
 Author-email: eastsheng@hotmail.com
+Description-Content-Type: text/markdown
 
 ## ReadLog
 
 - A python code to read thermo info from lammps log file 
 
 ### Installation
```

### Comparing `readlog-1.1.1/README.md` & `readlog-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `readlog-1.1.1/setup.py` & `readlog-1.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,19 +11,20 @@
 
 with open("requirements.txt","r") as f:
     required = f.read().splitlines()
 
 
 setup(
 name         = 'readlog',
-version      = '1.1.1',
+version      = '1.1.2',
 py_modules   = ['readlog'],
 author       = 'CHENDONGSHENG',
 author_email = 'eastsheng@hotmail.com',
 packages=find_packages('src'),
 package_dir={'': 'src'},
 install_requires=required,
 url          = 'https://github.com/eastsheng/readlog',
 description  = 'Read themo info from lammps output file or log file',
-long_description=long_description
+long_description=long_description,
+long_description_content_type='text/markdown'
 )
```

### Comparing `readlog-1.1.1/src/readlog.egg-info/PKG-INFO` & `readlog-1.1.2/src/readlog.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: readlog
-Version: 1.1.1
+Version: 1.1.2
 Summary: Read themo info from lammps output file or log file
 Home-page: https://github.com/eastsheng/readlog
 Author: CHENDONGSHENG
 Author-email: eastsheng@hotmail.com
+Description-Content-Type: text/markdown
 
 ## ReadLog
 
 - A python code to read thermo info from lammps log file 
 
 ### Installation
```

### Comparing `readlog-1.1.1/src/readlog.py` & `readlog-1.1.2/src/readlog.py`

 * *Files identical despite different names*

