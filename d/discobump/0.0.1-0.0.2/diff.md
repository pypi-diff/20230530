# Comparing `tmp/discobump-0.0.1.tar.gz` & `tmp/discobump-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discobump-0.0.1.tar", last modified: Tue May 30 18:33:44 2023, max compression
+gzip compressed data, was "discobump-0.0.2.tar", last modified: Tue May 30 18:56:27 2023, max compression
```

## Comparing `discobump-0.0.1.tar` & `discobump-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 18:33:44.713169 discobump-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-05-22 20:21:15.000000 discobump-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      432 2023-05-30 18:33:44.708172 discobump-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       78 2023-05-28 21:31:32.000000 discobump-0.0.1/README.md
--rw-rw-rw-   0        0        0      427 2023-05-30 18:32:18.000000 discobump-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-30 18:33:44.713169 discobump-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-30 18:33:44.266339 discobump-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-30 18:33:44.328133 discobump-0.0.1/src/discobump/
--rw-rw-rw-   0        0        0       20 2023-05-22 22:25:13.000000 discobump-0.0.1/src/discobump/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 18:33:44.690338 discobump-0.0.1/src/discobump/utils/
--rw-rw-rw-   0        0        0      773 2023-05-28 21:28:13.000000 discobump-0.0.1/src/discobump/utils/Api.py
--rw-rw-rw-   0        0        0      938 2023-05-28 21:29:12.000000 discobump-0.0.1/src/discobump/utils/Bumper.py
--rw-rw-rw-   0        0        0       41 2023-05-28 20:17:46.000000 discobump-0.0.1/src/discobump/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 18:33:44.589403 discobump-0.0.1/src/discobump.egg-info/
--rw-rw-rw-   0        0        0      432 2023-05-30 18:33:43.000000 discobump-0.0.1/src/discobump.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2023-05-30 18:33:44.000000 discobump-0.0.1/src/discobump.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 18:33:43.000000 discobump-0.0.1/src/discobump.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-30 18:33:43.000000 discobump-0.0.1/src/discobump.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-30 18:33:44.702179 discobump-0.0.1/tests/
--rw-rw-rw-   0        0        0      368 2023-05-28 21:23:53.000000 discobump-0.0.1/tests/testy.py
+drwxrwxrwx   0        0        0        0 2023-05-30 18:56:27.923882 discobump-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-05-22 20:21:15.000000 discobump-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      432 2023-05-30 18:56:27.915901 discobump-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       78 2023-05-28 21:31:32.000000 discobump-0.0.2/README.md
+-rw-rw-rw-   0        0        0      427 2023-05-30 18:55:13.000000 discobump-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-30 18:56:27.924883 discobump-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-30 18:56:27.764297 discobump-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-30 18:56:27.809042 discobump-0.0.2/src/discobump/
+-rw-rw-rw-   0        0        0       20 2023-05-22 22:25:13.000000 discobump-0.0.2/src/discobump/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 18:56:27.900276 discobump-0.0.2/src/discobump/utils/
+-rw-rw-rw-   0        0        0      773 2023-05-28 21:28:13.000000 discobump-0.0.2/src/discobump/utils/Api.py
+-rw-rw-rw-   0        0        0     1006 2023-05-30 18:54:32.000000 discobump-0.0.2/src/discobump/utils/Bumper.py
+-rw-rw-rw-   0        0        0       41 2023-05-28 20:17:46.000000 discobump-0.0.2/src/discobump/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 18:56:27.876119 discobump-0.0.2/src/discobump.egg-info/
+-rw-rw-rw-   0        0        0      432 2023-05-30 18:56:27.000000 discobump-0.0.2/src/discobump.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2023-05-30 18:56:27.000000 discobump-0.0.2/src/discobump.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 18:56:27.000000 discobump-0.0.2/src/discobump.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-30 18:56:27.000000 discobump-0.0.2/src/discobump.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 18:56:27.909655 discobump-0.0.2/tests/
+-rw-rw-rw-   0        0        0      885 2023-05-30 18:49:45.000000 discobump-0.0.2/tests/testy.py
```

### Comparing `discobump-0.0.1/LICENSE` & `discobump-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `discobump-0.0.1/src/discobump/utils/Api.py` & `discobump-0.0.2/src/discobump/utils/Api.py`

 * *Files identical despite different names*

### Comparing `discobump-0.0.1/src/discobump/utils/Bumper.py` & `discobump-0.0.2/src/discobump/utils/Bumper.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import requests, os
 from pyotp import TOTP
 
-def cls():
+if os.name == 'nt':
+  def cls():
     os.system('cls')
+else:
+  def cls():
+    os.system('clear')
 
 baseurl = 'https://discord.com/api/v9/interactions'
 
 class Bump:
     def __init__(self, token, guildid, channelid, **kwargs):
         token = token
         data = {
```

