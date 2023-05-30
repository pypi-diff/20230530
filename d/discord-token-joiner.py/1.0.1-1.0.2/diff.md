# Comparing `tmp/discord-token-joiner.py-1.0.1.tar.gz` & `tmp/discord-token-joiner.py-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-token-joiner.py-1.0.1.tar", last modified: Tue May 30 12:31:35 2023, max compression
+gzip compressed data, was "discord-token-joiner.py-1.0.2.tar", last modified: Tue May 30 12:33:11 2023, max compression
```

## Comparing `discord-token-joiner.py-1.0.1.tar` & `discord-token-joiner.py-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 12:31:35.003455 discord-token-joiner.py-1.0.1/
--rw-rw-rw-   0        0        0     1051 2023-05-30 12:20:08.000000 discord-token-joiner.py-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-05-30 12:28:06.000000 discord-token-joiner.py-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      876 2023-05-30 12:31:35.002457 discord-token-joiner.py-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-05-30 12:26:05.000000 discord-token-joiner.py-1.0.1/README.txt
-drwxrwxrwx   0        0        0        0 2023-05-30 12:31:34.987508 discord-token-joiner.py-1.0.1/discord-token-joiner/
--rw-rw-rw-   0        0        0     6243 2023-05-30 12:31:12.000000 discord-token-joiner.py-1.0.1/discord-token-joiner/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 12:31:34.997475 discord-token-joiner.py-1.0.1/discord_token_joiner.py.egg-info/
--rw-rw-rw-   0        0        0      876 2023-05-30 12:31:34.000000 discord-token-joiner.py-1.0.1/discord_token_joiner.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2023-05-30 12:31:34.000000 discord-token-joiner.py-1.0.1/discord_token_joiner.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 12:31:34.000000 discord-token-joiner.py-1.0.1/discord_token_joiner.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-30 12:31:34.000000 discord-token-joiner.py-1.0.1/discord_token_joiner.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-30 12:31:34.000000 discord-token-joiner.py-1.0.1/discord_token_joiner.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 12:31:35.004451 discord-token-joiner.py-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      661 2023-05-30 12:31:25.000000 discord-token-joiner.py-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 12:33:11.096918 discord-token-joiner.py-1.0.2/
+-rw-rw-rw-   0        0        0     1051 2023-05-30 12:20:08.000000 discord-token-joiner.py-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-05-30 12:28:06.000000 discord-token-joiner.py-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      876 2023-05-30 12:33:11.094925 discord-token-joiner.py-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-05-30 12:26:05.000000 discord-token-joiner.py-1.0.2/README.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 12:33:11.092933 discord-token-joiner.py-1.0.2/discord_token_joiner.py.egg-info/
+-rw-rw-rw-   0        0        0      876 2023-05-30 12:33:10.000000 discord-token-joiner.py-1.0.2/discord_token_joiner.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2023-05-30 12:33:11.000000 discord-token-joiner.py-1.0.2/discord_token_joiner.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 12:33:10.000000 discord-token-joiner.py-1.0.2/discord_token_joiner.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-30 12:33:10.000000 discord-token-joiner.py-1.0.2/discord_token_joiner.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-30 12:33:10.000000 discord-token-joiner.py-1.0.2/discord_token_joiner.py.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 12:33:11.093928 discord-token-joiner.py-1.0.2/discordtokenjoiner/
+-rw-rw-rw-   0        0        0     6243 2023-05-30 12:31:12.000000 discord-token-joiner.py-1.0.2/discordtokenjoiner/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-30 12:33:11.096918 discord-token-joiner.py-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      661 2023-05-30 12:33:07.000000 discord-token-joiner.py-1.0.2/setup.py
```

### Comparing `discord-token-joiner.py-1.0.1/LICENSE.txt` & `discord-token-joiner.py-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `discord-token-joiner.py-1.0.1/PKG-INFO` & `discord-token-joiner.py-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-token-joiner.py
-Version: 1.0.1
+Version: 1.0.2
 Summary: This is simple discord token joiner.
 Home-page: 
 Author: maxeqx
 License: MIT
 Keywords: discord token joiner
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
```

### Comparing `discord-token-joiner.py-1.0.1/discord-token-joiner/__init__.py` & `discord-token-joiner.py-1.0.2/discordtokenjoiner/__init__.py`

 * *Files identical despite different names*

### Comparing `discord-token-joiner.py-1.0.1/discord_token_joiner.py.egg-info/PKG-INFO` & `discord-token-joiner.py-1.0.2/discord_token_joiner.py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-token-joiner.py
-Version: 1.0.1
+Version: 1.0.2
 Summary: This is simple discord token joiner.
 Home-page: 
 Author: maxeqx
 License: MIT
 Keywords: discord token joiner
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
```

### Comparing `discord-token-joiner.py-1.0.1/setup.py` & `discord-token-joiner.py-1.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='discord-token-joiner.py',
-  version='1.0.1',
+  version='1.0.2',
   description='This is simple discord token joiner.',
   long_description=open('README.txt').read() ,
   url='',  
   author='maxeqx',
   license='MIT', 
   classifiers=classifiers,
   keywords='discord token joiner',
```

