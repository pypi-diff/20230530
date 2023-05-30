# Comparing `tmp/SalesforceMinu-0.0.7.tar.gz` & `tmp/SalesforceMinu-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SalesforceMinu-0.0.7.tar", last modified: Mon May 22 17:33:00 2023, max compression
+gzip compressed data, was "SalesforceMinu-0.0.8.tar", last modified: Tue May 30 15:28:33 2023, max compression
```

## Comparing `SalesforceMinu-0.0.7.tar` & `SalesforceMinu-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 17:33:00.979843 SalesforceMinu-0.0.7/
--rw-rw-rw-   0        0        0      610 2023-05-22 17:33:00.979843 SalesforceMinu-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-05-22 17:31:27.000000 SalesforceMinu-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 17:33:00.969870 SalesforceMinu-0.0.7/SalesforceMinu/
--rw-rw-rw-   0        0        0     4759 2023-05-22 17:32:52.000000 SalesforceMinu-0.0.7/SalesforceMinu/Funciones.py
--rw-rw-rw-   0        0        0        0 2023-04-25 17:16:47.000000 SalesforceMinu-0.0.7/SalesforceMinu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 17:33:00.978846 SalesforceMinu-0.0.7/SalesforceMinu.egg-info/
--rw-rw-rw-   0        0        0      610 2023-05-22 17:33:00.000000 SalesforceMinu-0.0.7/SalesforceMinu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-05-22 17:33:00.000000 SalesforceMinu-0.0.7/SalesforceMinu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 17:33:00.000000 SalesforceMinu-0.0.7/SalesforceMinu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-22 17:33:00.000000 SalesforceMinu-0.0.7/SalesforceMinu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-22 17:33:00.000000 SalesforceMinu-0.0.7/SalesforceMinu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 17:33:00.980841 SalesforceMinu-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1080 2023-05-22 17:31:10.000000 SalesforceMinu-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:28:33.714981 SalesforceMinu-0.0.8/
+-rw-rw-rw-   0        0        0      610 2023-05-30 15:28:33.713983 SalesforceMinu-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-05-30 15:16:29.000000 SalesforceMinu-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 15:28:33.694036 SalesforceMinu-0.0.8/SalesforceMinu/
+-rw-rw-rw-   0        0        0     4813 2023-05-30 15:15:35.000000 SalesforceMinu-0.0.8/SalesforceMinu/Funciones.py
+-rw-rw-rw-   0        0        0        0 2023-04-25 17:16:47.000000 SalesforceMinu-0.0.8/SalesforceMinu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:28:33.713017 SalesforceMinu-0.0.8/SalesforceMinu.egg-info/
+-rw-rw-rw-   0        0        0      610 2023-05-30 15:28:33.000000 SalesforceMinu-0.0.8/SalesforceMinu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-05-30 15:28:33.000000 SalesforceMinu-0.0.8/SalesforceMinu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 15:28:33.000000 SalesforceMinu-0.0.8/SalesforceMinu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-30 15:28:33.000000 SalesforceMinu-0.0.8/SalesforceMinu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-30 15:28:33.000000 SalesforceMinu-0.0.8/SalesforceMinu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 15:28:33.714981 SalesforceMinu-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1080 2023-05-30 15:16:19.000000 SalesforceMinu-0.0.8/setup.py
```

### Comparing `SalesforceMinu-0.0.7/PKG-INFO` & `SalesforceMinu-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: SalesforceMinu
-Version: 0.0.7
+Version: 0.0.8
 Summary: Librería para extraer datos de minu en salesforce
 Home-page: https://github.com/BalamCor?tab=repositories
 Author: Corchado Ramos Itzae Balam
 Author-email: g7_corc18@ens.cnyn.unam.mx
 License: MIT
 Description-Content-Type: text/markdown
 
 Pasos obtenidos de: https://antonio-fernandez-troyano.medium.com/crear-una-libreria-python-4e841fbd154f
 
 Corremos en carpeta de libreria el comando:
 python setup.py sdist bdist_wheel
 
 Subimos a PyPi:
-twine upload dist/SalesforceMinu-0.0.7.tar.gz dist/SalesforceMinu-0.0.7-py3-none-any.whl
+twine upload dist/SalesforceMinu-0.0.8.tar.gz dist/SalesforceMinu-0.0.8-py3-none-any.whl
```

### Comparing `SalesforceMinu-0.0.7/SalesforceMinu/Funciones.py` & `SalesforceMinu-0.0.8/SalesforceMinu/Funciones.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,16 @@
         trans_tab = dict.fromkeys(map(ord, u'\u0301\u0308'), None)
         name = normalize('NFKC', normalize('NFKD', name).translate(trans_tab))
         where = f"Name IN ({name})"
         case = 1
     
     query = f"""SELECT Id, Name, NumberOfEmployees
     FROM Account
-    WHERE {where}"""
+    WHERE {where}
+    AND Etapa_de_Oportunidad__c LIKE '%TyC firmado%'"""
     
     records = sf.query_all(query)
     # Obtenemos el orden de los nombres y sus IDs
     Names_order = [ row['Name'] for row in records['records']]
     IDs = [ row['Id'] for row in records['records']]
     
     # Ver si no encontro alguno, es decir que el tamaño sea menor que la entrada
```

### Comparing `SalesforceMinu-0.0.7/SalesforceMinu.egg-info/PKG-INFO` & `SalesforceMinu-0.0.8/SalesforceMinu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: SalesforceMinu
-Version: 0.0.7
+Version: 0.0.8
 Summary: Librería para extraer datos de minu en salesforce
 Home-page: https://github.com/BalamCor?tab=repositories
 Author: Corchado Ramos Itzae Balam
 Author-email: g7_corc18@ens.cnyn.unam.mx
 License: MIT
 Description-Content-Type: text/markdown
 
 Pasos obtenidos de: https://antonio-fernandez-troyano.medium.com/crear-una-libreria-python-4e841fbd154f
 
 Corremos en carpeta de libreria el comando:
 python setup.py sdist bdist_wheel
 
 Subimos a PyPi:
-twine upload dist/SalesforceMinu-0.0.7.tar.gz dist/SalesforceMinu-0.0.7-py3-none-any.whl
+twine upload dist/SalesforceMinu-0.0.8.tar.gz dist/SalesforceMinu-0.0.8-py3-none-any.whl
```

### Comparing `SalesforceMinu-0.0.7/setup.py` & `SalesforceMinu-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 PACKAGE_NAME = 'SalesforceMinu' 
 AUTHOR = 'Corchado Ramos Itzae Balam' #Modificar con vuestros datos
 AUTHOR_EMAIL = 'g7_corc18@ens.cnyn.unam.mx' 
 URL = 'https://github.com/BalamCor?tab=repositories' 
 
 LICENSE = 'MIT' #Tipo de licencia
 DESCRIPTION = 'Librería para extraer datos de minu en salesforce'
```

