# Comparing `tmp/apigratis-sdk-python-0.0.3.tar.gz` & `tmp/apigratis-sdk-python-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apigratis-sdk-python-0.0.3.tar", last modified: Mon May 29 21:12:24 2023, max compression
+gzip compressed data, was "apigratis-sdk-python-0.0.4.tar", last modified: Mon May 29 22:02:48 2023, max compression
```

## Comparing `apigratis-sdk-python-0.0.3.tar` & `apigratis-sdk-python-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 21:12:24.341480 apigratis-sdk-python-0.0.3/
--rw-rw-rw-   0        0        0      465 2023-05-29 21:12:24.340480 apigratis-sdk-python-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       25 2023-05-29 19:58:01.000000 apigratis-sdk-python-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 21:12:24.319480 apigratis-sdk-python-0.0.3/apigratis-sdk-python/
--rw-rw-rw-   0        0        0      769 2023-05-29 20:58:30.000000 apigratis-sdk-python-0.0.3/apigratis-sdk-python/ServiceClass.py
--rw-rw-rw-   0        0        0        0 2023-05-29 19:43:41.000000 apigratis-sdk-python-0.0.3/apigratis-sdk-python/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 21:12:24.339480 apigratis-sdk-python-0.0.3/apigratis_sdk_python.egg-info/
--rw-rw-rw-   0        0        0      465 2023-05-29 21:12:24.000000 apigratis-sdk-python-0.0.3/apigratis_sdk_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      307 2023-05-29 21:12:24.000000 apigratis-sdk-python-0.0.3/apigratis_sdk_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 21:12:24.000000 apigratis-sdk-python-0.0.3/apigratis_sdk_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-29 21:12:24.000000 apigratis-sdk-python-0.0.3/apigratis_sdk_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-29 21:12:24.000000 apigratis-sdk-python-0.0.3/apigratis_sdk_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 21:12:24.341480 apigratis-sdk-python-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      578 2023-05-29 21:11:29.000000 apigratis-sdk-python-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 22:02:48.885977 apigratis-sdk-python-0.0.4/
+-rw-rw-rw-   0        0        0      465 2023-05-29 22:02:48.884978 apigratis-sdk-python-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       25 2023-05-29 19:58:01.000000 apigratis-sdk-python-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 22:02:48.854465 apigratis-sdk-python-0.0.4/apigratis-sdk-python/
+-rw-rw-rw-   0        0        0      784 2023-05-29 22:01:03.000000 apigratis-sdk-python-0.0.4/apigratis-sdk-python/Service.py
+-rw-rw-rw-   0        0        0        0 2023-05-29 19:43:41.000000 apigratis-sdk-python-0.0.4/apigratis-sdk-python/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 22:02:48.882977 apigratis-sdk-python-0.0.4/apigratis_sdk_python.egg-info/
+-rw-rw-rw-   0        0        0      465 2023-05-29 22:02:48.000000 apigratis-sdk-python-0.0.4/apigratis_sdk_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-05-29 22:02:48.000000 apigratis-sdk-python-0.0.4/apigratis_sdk_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 22:02:48.000000 apigratis-sdk-python-0.0.4/apigratis_sdk_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-29 22:02:48.000000 apigratis-sdk-python-0.0.4/apigratis_sdk_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-29 22:02:48.000000 apigratis-sdk-python-0.0.4/apigratis_sdk_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 22:02:48.885977 apigratis-sdk-python-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      578 2023-05-29 22:02:18.000000 apigratis-sdk-python-0.0.4/setup.py
```

### Comparing `apigratis-sdk-python-0.0.3/apigratis-sdk-python/ServiceClass.py` & `apigratis-sdk-python-0.0.4/apigratis-sdk-python/Service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import requests
 import json
 
-class ServiceClass:
+class Service:
 
     def __init__(self, data):
         self.credentials = data.credentials
         self.server = "https://cluster-01.apigratis.com/api/v1/"
 
     def whatsapp(self, data):
 
         url = "whatsapp/"+data.body.action
         payload = json.dumps(data.body)
         
         headers = {
             'Content-Type': 'application/json',
             'SecretKey': self.credentials.SecretKey,
-            'PublicToken': self.PublicToken,
+            'PublicToken': self.credentials.PublicToken,
             'Authorization': 'Bearer ' + self.credentials.BearerToken,
-            'DeviceToken': self.DeviceToken
+            'DeviceToken': self.credentials.DeviceToken
         }
 
         response = requests.request("POST", url, headers=headers, data=payload)
 
-        return json.loads(response.text.encode('utf8'))
-
+        return json.loads(response.text.encode('utf8'))
```

### Comparing `apigratis-sdk-python-0.0.3/setup.py` & `apigratis-sdk-python-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='apigratis-sdk-python',
-    version='0.0.3',
+    version='0.0.4',
     description='Transforme seus projetos em soluções inteligentes com nossa API. Com recursos como  API do WhatsApp, geolocalização, rastreamento de encomendas, verificação de CPF/CNPJ e mais, você pode criar soluções eficientes e funcionais. Comece agora.',
     author='APIBRASIL',
     author_email='contato@apibrasil.com.br',
     packages=['apigratis-sdk-python'],
     install_requires=[
         # Lista de dependências necessárias
         'requests',
```

