# Comparing `tmp/apigratis-0.0.5.tar.gz` & `tmp/apigratis-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apigratis-0.0.5.tar", last modified: Mon May 29 22:06:48 2023, max compression
+gzip compressed data, was "apigratis-0.0.6.tar", last modified: Mon May 29 22:20:13 2023, max compression
```

## Comparing `apigratis-0.0.5.tar` & `apigratis-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 22:06:48.199286 apigratis-0.0.5/
--rw-rw-rw-   0        0        0      454 2023-05-29 22:06:48.196222 apigratis-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       25 2023-05-29 19:58:01.000000 apigratis-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 22:06:48.170685 apigratis-0.0.5/apigratis/
--rw-rw-rw-   0        0        0      784 2023-05-29 22:01:03.000000 apigratis-0.0.5/apigratis/Service.py
--rw-rw-rw-   0        0        0        0 2023-05-29 19:43:41.000000 apigratis-0.0.5/apigratis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 22:06:48.193223 apigratis-0.0.5/apigratis.egg-info/
--rw-rw-rw-   0        0        0      454 2023-05-29 22:06:48.000000 apigratis-0.0.5/apigratis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-05-29 22:06:48.000000 apigratis-0.0.5/apigratis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 22:06:48.000000 apigratis-0.0.5/apigratis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-29 22:06:48.000000 apigratis-0.0.5/apigratis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-29 22:06:48.000000 apigratis-0.0.5/apigratis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 22:06:48.199286 apigratis-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      556 2023-05-29 22:06:36.000000 apigratis-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 22:20:13.805217 apigratis-0.0.6/
+-rw-rw-rw-   0        0        0      454 2023-05-29 22:20:13.804216 apigratis-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       25 2023-05-29 19:58:01.000000 apigratis-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 22:20:13.770695 apigratis-0.0.6/apigratis/
+-rw-rw-rw-   0        0        0      753 2023-05-29 22:19:50.000000 apigratis-0.0.6/apigratis/Service.py
+-rw-rw-rw-   0        0        0        0 2023-05-29 19:43:41.000000 apigratis-0.0.6/apigratis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 22:20:13.801217 apigratis-0.0.6/apigratis.egg-info/
+-rw-rw-rw-   0        0        0      454 2023-05-29 22:20:13.000000 apigratis-0.0.6/apigratis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-05-29 22:20:13.000000 apigratis-0.0.6/apigratis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 22:20:13.000000 apigratis-0.0.6/apigratis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-29 22:20:13.000000 apigratis-0.0.6/apigratis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-29 22:20:13.000000 apigratis-0.0.6/apigratis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 22:20:13.806192 apigratis-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      556 2023-05-29 22:20:00.000000 apigratis-0.0.6/setup.py
```

### Comparing `apigratis-0.0.5/apigratis/Service.py` & `apigratis-0.0.6/apigratis/Service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import requests
 import json
 
 class Service:
 
     def __init__(self, data):
-        self.credentials = data.credentials
         self.server = "https://cluster-01.apigratis.com/api/v1/"
 
     def whatsapp(self, data):
 
         url = "whatsapp/"+data.body.action
         payload = json.dumps(data.body)
-        
+
+        credentials = data.credentials
+
         headers = {
             'Content-Type': 'application/json',
-            'SecretKey': self.credentials.SecretKey,
-            'PublicToken': self.credentials.PublicToken,
-            'Authorization': 'Bearer ' + self.credentials.BearerToken,
-            'DeviceToken': self.credentials.DeviceToken
+            'SecretKey': credentials.SecretKey,
+            'PublicToken': credentials.PublicToken,
+            'Authorization': 'Bearer ' + credentials.BearerToken,
+            'DeviceToken': credentials.DeviceToken
         }
 
         response = requests.request("POST", url, headers=headers, data=payload)
 
         return json.loads(response.text.encode('utf8'))
```

### Comparing `apigratis-0.0.5/setup.py` & `apigratis-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='apigratis',
-    version='0.0.5',
+    version='0.0.6',
     description='Transforme seus projetos em soluções inteligentes com nossa API. Com recursos como  API do WhatsApp, geolocalização, rastreamento de encomendas, verificação de CPF/CNPJ e mais, você pode criar soluções eficientes e funcionais. Comece agora.',
     author='APIBRASIL',
     author_email='contato@apibrasil.com.br',
     packages=['apigratis'],
     install_requires=[
         # Lista de dependências necessárias
         'requests',
```

