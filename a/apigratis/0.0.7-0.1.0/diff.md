# Comparing `tmp/apigratis-0.0.7.tar.gz` & `tmp/apigratis-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apigratis-0.0.7.tar", last modified: Mon May 29 22:26:41 2023, max compression
+gzip compressed data, was "apigratis-0.1.0.tar", last modified: Tue May 30 12:37:17 2023, max compression
```

## Comparing `apigratis-0.0.7.tar` & `apigratis-0.1.0.tar`

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
+drwxrwxrwx   0        0        0        0 2023-05-30 12:37:17.369854 apigratis-0.1.0/
+-rw-rw-rw-   0        0        0      454 2023-05-30 12:37:17.368854 apigratis-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2640 2023-05-30 12:37:02.000000 apigratis-0.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-30 12:37:17.346848 apigratis-0.1.0/apigratis/
+-rw-rw-rw-   0        0        0     1828 2023-05-29 23:03:05.000000 apigratis-0.1.0/apigratis/Service.py
+-rw-rw-rw-   0        0        0        0 2023-05-29 19:43:41.000000 apigratis-0.1.0/apigratis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 12:37:17.366847 apigratis-0.1.0/apigratis.egg-info/
+-rw-rw-rw-   0        0        0      454 2023-05-30 12:37:17.000000 apigratis-0.1.0/apigratis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-05-30 12:37:17.000000 apigratis-0.1.0/apigratis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 12:37:17.000000 apigratis-0.1.0/apigratis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-30 12:37:17.000000 apigratis-0.1.0/apigratis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-30 12:37:17.000000 apigratis-0.1.0/apigratis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 12:37:17.369854 apigratis-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      556 2023-05-30 12:36:50.000000 apigratis-0.1.0/setup.py
```

### Comparing `apigratis-0.0.7/setup.py` & `apigratis-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='apigratis',
-    version='0.0.7',
+    version='0.1.0',
     description='Transforme seus projetos em soluções inteligentes com nossa API. Com recursos como  API do WhatsApp, geolocalização, rastreamento de encomendas, verificação de CPF/CNPJ e mais, você pode criar soluções eficientes e funcionais. Comece agora.',
     author='APIBRASIL',
     author_email='contato@apibrasil.com.br',
     packages=['apigratis'],
     install_requires=[
         # Lista de dependências necessárias
         'requests',
```

