# Comparing `tmp/hive-archeology-bot-0.1.2.tar.gz` & `tmp/hive-archeology-bot-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hive-archeology-bot-0.1.2.tar", last modified: Fri May 19 18:59:16 2023, max compression
+gzip compressed data, was "hive-archeology-bot-0.1.4.tar", last modified: Tue May 30 16:33:58 2023, max compression
```

## Comparing `hive-archeology-bot-0.1.2.tar` & `hive-archeology-bot-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-19 18:59:16.858200 hive-archeology-bot-0.1.2/
--rw-rw-r--   0 rob       (1000) rob       (1000)     1499 2023-05-19 18:51:54.000000 hive-archeology-bot-0.1.2/LICENSE
--rw-rw-r--   0 rob       (1000) rob       (1000)      754 2023-05-19 18:59:16.858200 hive-archeology-bot-0.1.2/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)       98 2023-05-19 18:51:54.000000 hive-archeology-bot-0.1.2/README.md
--rwxr-xr-x   0 rob       (1000) rob       (1000)    14371 2023-05-19 18:48:46.000000 hive-archeology-bot-0.1.2/hive_archeology.py
-drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-19 18:59:16.858200 hive-archeology-bot-0.1.2/hive_archeology_bot.egg-info/
--rw-rw-r--   0 rob       (1000) rob       (1000)      754 2023-05-19 18:59:16.000000 hive-archeology-bot-0.1.2/hive_archeology_bot.egg-info/PKG-INFO
--rw-rw-r--   0 rob       (1000) rob       (1000)      347 2023-05-19 18:59:16.000000 hive-archeology-bot-0.1.2/hive_archeology_bot.egg-info/SOURCES.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-19 18:59:16.000000 hive-archeology-bot-0.1.2/hive_archeology_bot.egg-info/dependency_links.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       62 2023-05-19 18:59:16.000000 hive-archeology-bot-0.1.2/hive_archeology_bot.egg-info/entry_points.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-19 18:53:43.000000 hive-archeology-bot-0.1.2/hive_archeology_bot.egg-info/not-zip-safe
--rw-rw-r--   0 rob       (1000) rob       (1000)       10 2023-05-19 18:59:16.000000 hive-archeology-bot-0.1.2/hive_archeology_bot.egg-info/requires.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       16 2023-05-19 18:59:16.000000 hive-archeology-bot-0.1.2/hive_archeology_bot.egg-info/top_level.txt
--rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-05-19 18:59:16.858200 hive-archeology-bot-0.1.2/setup.cfg
--rwxr-xr-x   0 rob       (1000) rob       (1000)     1089 2023-05-19 18:58:33.000000 hive-archeology-bot-0.1.2/setup.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-30 16:33:58.003673 hive-archeology-bot-0.1.4/
+-rw-rw-r--   0 rob       (1000) rob       (1000)     1499 2023-05-19 18:51:54.000000 hive-archeology-bot-0.1.4/LICENSE
+-rw-rw-r--   0 rob       (1000) rob       (1000)      773 2023-05-30 16:33:58.003673 hive-archeology-bot-0.1.4/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)     2104 2023-05-19 19:43:04.000000 hive-archeology-bot-0.1.4/README.md
+-rwxr-xr-x   0 rob       (1000) rob       (1000)    20514 2023-05-30 16:32:42.000000 hive-archeology-bot-0.1.4/hive_archeology.py
+drwxrwxr-x   0 rob       (1000) rob       (1000)        0 2023-05-30 16:33:58.003673 hive-archeology-bot-0.1.4/hive_archeology_bot.egg-info/
+-rw-rw-r--   0 rob       (1000) rob       (1000)      773 2023-05-30 16:33:57.000000 hive-archeology-bot-0.1.4/hive_archeology_bot.egg-info/PKG-INFO
+-rw-rw-r--   0 rob       (1000) rob       (1000)      347 2023-05-30 16:33:57.000000 hive-archeology-bot-0.1.4/hive_archeology_bot.egg-info/SOURCES.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-30 16:33:57.000000 hive-archeology-bot-0.1.4/hive_archeology_bot.egg-info/dependency_links.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       62 2023-05-30 16:33:57.000000 hive-archeology-bot-0.1.4/hive_archeology_bot.egg-info/entry_points.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)        1 2023-05-19 18:53:43.000000 hive-archeology-bot-0.1.4/hive_archeology_bot.egg-info/not-zip-safe
+-rw-rw-r--   0 rob       (1000) rob       (1000)       10 2023-05-30 16:33:57.000000 hive-archeology-bot-0.1.4/hive_archeology_bot.egg-info/requires.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       16 2023-05-30 16:33:57.000000 hive-archeology-bot-0.1.4/hive_archeology_bot.egg-info/top_level.txt
+-rw-rw-r--   0 rob       (1000) rob       (1000)       38 2023-05-30 16:33:58.003673 hive-archeology-bot-0.1.4/setup.cfg
+-rwxr-xr-x   0 rob       (1000) rob       (1000)     1125 2023-05-22 09:18:10.000000 hive-archeology-bot-0.1.4/setup.py
```

### Comparing `hive-archeology-bot-0.1.2/LICENSE` & `hive-archeology-bot-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hive-archeology-bot-0.1.2/PKG-INFO` & `hive-archeology-bot-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: hive-archeology-bot
-Version: 0.1.2
+Version: 0.1.4
 Summary: Hive Archeology Bot
 Home-page: https://github.com/pibara/hive-archeology
 Author: Rob Meijer
 Author-email: pibara@gmail.com
 License: BSD
 Keywords: hive web3 bot
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 License-File: LICENSE
 
 Simple HIVE bot that allows its owner to up-vote valuable timeless HIVE posts.
+
```

### Comparing `hive-archeology-bot-0.1.2/hive_archeology_bot.egg-info/PKG-INFO` & `hive-archeology-bot-0.1.4/hive_archeology_bot.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: hive-archeology-bot
-Version: 0.1.2
+Version: 0.1.4
 Summary: Hive Archeology Bot
 Home-page: https://github.com/pibara/hive-archeology
 Author: Rob Meijer
 Author-email: pibara@gmail.com
 License: BSD
 Keywords: hive web3 bot
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 License-File: LICENSE
 
 Simple HIVE bot that allows its owner to up-vote valuable timeless HIVE posts.
+
```

### Comparing `hive-archeology-bot-0.1.2/setup.py` & `hive-archeology-bot-0.1.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from setuptools import setup
+from hive_archeology import VERSION
 
 setup(
     name='hive-archeology-bot',
-    version="0.1.2",
+    version=VERSION,
     description="Hive Archeology Bot",
     long_description="Simple HIVE bot that allows its owner to up-vote valuable timeless HIVE posts.",
     author='Rob Meijer',
     author_email='pibara@gmail.com',
     url='https://github.com/pibara/hive-archeology',
     license='BSD',
     py_modules=['hive_archeology'],
```

