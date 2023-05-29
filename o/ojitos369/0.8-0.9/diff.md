# Comparing `tmp/ojitos369-0.8.tar.gz` & `tmp/ojitos369-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ojitos369-0.8.tar", last modified: Wed Oct  5 02:43:33 2022, max compression
+gzip compressed data, was "ojitos369-0.9.tar", last modified: Wed Oct  5 18:32:37 2022, max compression
```

## Comparing `ojitos369-0.8.tar` & `ojitos369-0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ojitos369  (1000) ojitos369  (1000)        0 2022-10-05 02:43:33.149840 ojitos369-0.8/
--rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)        0 2022-10-05 02:30:05.000000 ojitos369-0.8/LICENSE.txt
--rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)       29 2022-10-05 02:30:05.000000 ojitos369-0.8/MANIFEST.in
--rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)      693 2022-10-05 02:43:33.149840 ojitos369-0.8/PKG-INFO
--rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)     3398 2022-10-05 02:42:30.000000 ojitos369-0.8/README.md
-drwxrwxr-x   0 ojitos369  (1000) ojitos369  (1000)        0 2022-10-05 02:43:33.149840 ojitos369-0.8/ojitos369/
--rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)        0 2022-10-05 02:30:05.000000 ojitos369-0.8/ojitos369/__init__.py
--rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)     2090 2022-10-05 02:30:05.000000 ojitos369-0.8/ojitos369/errors.py
--rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)     3500 2022-10-05 02:30:05.000000 ojitos369-0.8/ojitos369/text_format.py
--rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)     1177 2022-10-05 02:30:05.000000 ojitos369-0.8/ojitos369/utils.py
-drwxrwxr-x   0 ojitos369  (1000) ojitos369  (1000)        0 2022-10-05 02:43:33.149840 ojitos369-0.8/ojitos369.egg-info/
--rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)      693 2022-10-05 02:43:33.000000 ojitos369-0.8/ojitos369.egg-info/PKG-INFO
--rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)      270 2022-10-05 02:43:33.000000 ojitos369-0.8/ojitos369.egg-info/SOURCES.txt
--rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)        1 2022-10-05 02:43:33.000000 ojitos369-0.8/ojitos369.egg-info/dependency_links.txt
--rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)       10 2022-10-05 02:43:33.000000 ojitos369-0.8/ojitos369.egg-info/top_level.txt
--rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)       38 2022-10-05 02:43:33.149840 ojitos369-0.8/setup.cfg
--rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)     1258 2022-10-05 02:40:38.000000 ojitos369-0.8/setup.py
+drwxrwxr-x   0 ojitos369  (1000) ojitos369  (1000)        0 2022-10-05 18:32:37.318541 ojitos369-0.9/
+-rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)        0 2022-10-05 17:06:15.000000 ojitos369-0.9/LICENSE.txt
+-rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)       29 2022-10-05 17:06:15.000000 ojitos369-0.9/MANIFEST.in
+-rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)      674 2022-10-05 18:32:37.318541 ojitos369-0.9/PKG-INFO
+-rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)     3515 2022-10-05 17:06:15.000000 ojitos369-0.9/README.md
+drwxrwxr-x   0 ojitos369  (1000) ojitos369  (1000)        0 2022-10-05 18:32:37.314541 ojitos369-0.9/ojitos369/
+-rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)        0 2022-10-05 17:06:15.000000 ojitos369-0.9/ojitos369/__init__.py
+-rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)     2090 2022-10-05 17:06:15.000000 ojitos369-0.9/ojitos369/errors.py
+-rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)     3754 2022-10-05 18:32:07.000000 ojitos369-0.9/ojitos369/text_format.py
+-rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)     1177 2022-10-05 17:06:15.000000 ojitos369-0.9/ojitos369/utils.py
+drwxrwxr-x   0 ojitos369  (1000) ojitos369  (1000)        0 2022-10-05 18:32:37.314541 ojitos369-0.9/ojitos369.egg-info/
+-rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)      674 2022-10-05 18:32:36.000000 ojitos369-0.9/ojitos369.egg-info/PKG-INFO
+-rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)      270 2022-10-05 18:32:36.000000 ojitos369-0.9/ojitos369.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)        1 2022-10-05 18:32:36.000000 ojitos369-0.9/ojitos369.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)       10 2022-10-05 18:32:36.000000 ojitos369-0.9/ojitos369.egg-info/top_level.txt
+-rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)       38 2022-10-05 18:32:37.318541 ojitos369-0.9/setup.cfg
+-rw-rw-r--   0 ojitos369  (1000) ojitos369  (1000)     1258 2022-10-05 18:32:23.000000 ojitos369-0.9/setup.py
```

### Comparing `ojitos369-0.8/PKG-INFO` & `ojitos369-0.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: ojitos369
-Version: 0.8
+Version: 0.9
 Summary: Funciones de utilidades de ojitos369
 Home-page: https://github.com/Ojitos369/ojitos369-pip
 Author: Ojitos369
 Author-email: ojitos369@gmail.com
 License: LGPL v3
 Keywords: Utilidades de ojitos369
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE.txt
 
 Funciones de utilidades de ojitos369
 Revizar README en:
 https://github.com/Ojitos369/ojitos369-pip
-
```

### Comparing `ojitos369-0.8/README.md` & `ojitos369-0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -141,14 +141,15 @@
 ### Databases
 
 * For this you need install ojitos369_db_connections
 
 ```py
 pip install ojitos369_db_connections
 ```
+[REPO: https://github.com/Ojitos369/ojitos369_db_connections](https://github.com/Ojitos369/ojitos369_db_connections)
 
 
 #### Oracle
 
 ```py
 
 from ojitos369_db_connections.oracle_db import ConexionOracle
```

### Comparing `ojitos369-0.8/ojitos369/errors.py` & `ojitos369-0.9/ojitos369/errors.py`

 * *Files identical despite different names*

### Comparing `ojitos369-0.8/ojitos369/text_format.py` & `ojitos369-0.9/ojitos369/text_format.py`

 * *Files 11% similar despite different names*

```diff
@@ -37,14 +37,18 @@
             text = text.replace('  ', ' ')
             if not '  ' in text: break
         for special_space in special_spaces:
             text = text.replace(special_space, special_spaces[special_space])
         return text
     
     def unique_string_no_space(self, items: list) -> str:
+        if type(items) == str:
+            items = items.split()
+        elif type(items) != list:
+            items = [items]
         text = ''
         for item in items:
             if not item:
                 continue
             item = str(item)
             item = self.without_acute(item)
             text += item.lower().replace(' ','')
@@ -58,14 +62,18 @@
             item = self.without_acute(item)
             item = self.normalize_spaces(item)
             text += item.lower() + ' '
         text = text[:-1]
         return text
     
     def normal_text(self, items: list) -> str:
+        if type(items) == str:
+            items = items.split()
+        elif type(items) != list:
+            items = [items]
         text = ''
         for item in items:
             if not item:
                 continue
             item = self.normalize_spaces(item)
             text += item + ' '
         text = text[:-1]
```

### Comparing `ojitos369-0.8/ojitos369/utils.py` & `ojitos369-0.9/ojitos369/utils.py`

 * *Files identical despite different names*

### Comparing `ojitos369-0.8/ojitos369.egg-info/PKG-INFO` & `ojitos369-0.9/ojitos369.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: ojitos369
-Version: 0.8
+Version: 0.9
 Summary: Funciones de utilidades de ojitos369
 Home-page: https://github.com/Ojitos369/ojitos369-pip
 Author: Ojitos369
 Author-email: ojitos369@gmail.com
 License: LGPL v3
 Keywords: Utilidades de ojitos369
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE.txt
 
 Funciones de utilidades de ojitos369
 Revizar README en:
 https://github.com/Ojitos369/ojitos369-pip
-
```

### Comparing `ojitos369-0.8/setup.py` & `ojitos369-0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
  
 # download_url='https://github.com/RDCH106/parallel_foreach_submodule/archive/v0.1.tar.gz', # Te lo explico a continuación
 setup(
     name='ojitos369',
     packages=['ojitos369'], # Mismo nombre que en la estructura de carpetas de arriba
     include_package_data=True,
-    version='0.8',
+    version='0.9',
     license='LGPL v3', # La licencia que tenga tu paquete
     description='Funciones de utilidades de ojitos369',
     long_description='Funciones de utilidades de ojitos369\nRevizar README en:\nhttps://github.com/Ojitos369/ojitos369-pip',
     author='Ojitos369',
     author_email='ojitos369@gmail.com',
     url='https://github.com/Ojitos369/ojitos369-pip', # Usa la URL del repositorio de GitHub
     keywords='Utilidades de ojitos369', # Palabras que definan tu paquete
```

