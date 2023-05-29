# Comparing `tmp/apigratis-0.0.7.tar.gz` & `tmp/apigratis-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apigratis-0.0.7.tar", last modified: Mon May 29 22:26:41 2023, max compression
+gzip compressed data, was "apigratis-0.0.9.tar", last modified: Mon May 29 23:10:03 2023, max compression
```

## Comparing `apigratis-0.0.7.tar` & `apigratis-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 22:26:41.993469 apigratis-0.0.7/
--rw-rw-rw-   0        0        0      454 2023-05-29 22:26:41.992466 apigratis-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       25 2023-05-29 19:58:01.000000 apigratis-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 22:26:41.972951 apigratis-0.0.7/apigratis/
--rw-rw-rw-   0        0        0      716 2023-05-29 22:25:46.000000 apigratis-0.0.7/apigratis/Service.py
--rw-rw-rw-   0        0        0        0 2023-05-29 19:43:41.000000 apigratis-0.0.7/apigratis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 22:26:41.991470 apigratis-0.0.7/apigratis.egg-info/
--rw-rw-rw-   0        0        0      454 2023-05-29 22:26:41.000000 apigratis-0.0.7/apigratis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-05-29 22:26:41.000000 apigratis-0.0.7/apigratis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 22:26:41.000000 apigratis-0.0.7/apigratis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-29 22:26:41.000000 apigratis-0.0.7/apigratis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-29 22:26:41.000000 apigratis-0.0.7/apigratis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 22:26:41.993469 apigratis-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      556 2023-05-29 22:26:39.000000 apigratis-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 23:10:03.652634 apigratis-0.0.9/
+-rw-rw-rw-   0        0        0      454 2023-05-29 23:10:03.650635 apigratis-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1031 2023-05-29 23:06:31.000000 apigratis-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 23:10:03.635627 apigratis-0.0.9/apigratis/
+-rw-rw-rw-   0        0        0     1828 2023-05-29 23:03:05.000000 apigratis-0.0.9/apigratis/Service.py
+-rw-rw-rw-   0        0        0        0 2023-05-29 19:43:41.000000 apigratis-0.0.9/apigratis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 23:10:03.648634 apigratis-0.0.9/apigratis.egg-info/
+-rw-rw-rw-   0        0        0      454 2023-05-29 23:10:03.000000 apigratis-0.0.9/apigratis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2023-05-29 23:10:03.000000 apigratis-0.0.9/apigratis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 23:10:03.000000 apigratis-0.0.9/apigratis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-29 23:10:03.000000 apigratis-0.0.9/apigratis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-29 23:10:03.000000 apigratis-0.0.9/apigratis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 23:10:03.652634 apigratis-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      556 2023-05-29 23:09:55.000000 apigratis-0.0.9/setup.py
```

### Comparing `apigratis-0.0.7/setup.py` & `apigratis-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='apigratis',
-    version='0.0.7',
+    version='0.0.9',
     description='Transforme seus projetos em soluções inteligentes com nossa API. Com recursos como  API do WhatsApp, geolocalização, rastreamento de encomendas, verificação de CPF/CNPJ e mais, você pode criar soluções eficientes e funcionais. Comece agora.',
     author='APIBRASIL',
     author_email='contato@apibrasil.com.br',
     packages=['apigratis'],
     install_requires=[
         # Lista de dependências necessárias
         'requests',
```

