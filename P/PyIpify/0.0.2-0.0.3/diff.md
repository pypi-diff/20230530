# Comparing `tmp/PyIpify-0.0.2.tar.gz` & `tmp/PyIpify-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyIpify-0.0.2.tar", last modified: Fri May 26 11:14:28 2023, max compression
+gzip compressed data, was "PyIpify-0.0.3.tar", last modified: Tue May 30 10:20:11 2023, max compression
```

## Comparing `PyIpify-0.0.2.tar` & `PyIpify-0.0.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 11:14:28.674994 PyIpify-0.0.2/
--rw-rw-rw-   0        0        0     1061 2023-05-26 11:14:28.674994 PyIpify-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-26 11:14:28.532848 PyIpify-0.0.2/PyIpify/
--rw-rw-rw-   0        0        0       38 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/__init__.py
--rw-rw-rw-   0        0        0     1352 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 11:14:28.632495 PyIpify-0.0.2/PyIpify/asyncronous/
--rw-rw-rw-   0        0        0       68 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/asyncronous/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 11:14:28.659474 PyIpify-0.0.2/PyIpify/asyncronous/__pycache__/
--rw-rw-rw-   0        0        0      201 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/asyncronous/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      247 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/asyncronous/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      522 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/asyncronous/__pycache__/find_ipv4.cpython-310.pyc
--rw-rw-rw-   0        0        0     1294 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/asyncronous/__pycache__/find_ipv4.cpython-311.pyc
--rw-rw-rw-   0        0        0      523 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/asyncronous/__pycache__/find_ipv6.cpython-310.pyc
--rw-rw-rw-   0        0        0     1295 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/asyncronous/__pycache__/find_ipv6.cpython-311.pyc
--rw-rw-rw-   0        0        0      234 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/asyncronous/find_ipv4.py
--rw-rw-rw-   0        0        0      230 2023-05-26 11:09:37.000000 PyIpify-0.0.2/PyIpify/asyncronous/find_ipv6.py
-drwxrwxrwx   0        0        0        0 2023-05-26 11:14:28.659474 PyIpify-0.0.2/PyIpify/syncronous/
--rw-rw-rw-   0        0        0       68 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/syncronous/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 11:14:28.674994 PyIpify-0.0.2/PyIpify/syncronous/__pycache__/
--rw-rw-rw-   0        0        0      200 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/syncronous/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      246 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/syncronous/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0      373 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/syncronous/__pycache__/find_ipv4.cpython-310.pyc
--rw-rw-rw-   0        0        0      516 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/syncronous/__pycache__/find_ipv4.cpython-311.pyc
--rw-rw-rw-   0        0        0      374 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/syncronous/__pycache__/find_ipv6.cpython-310.pyc
--rw-rw-rw-   0        0        0      517 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/syncronous/__pycache__/find_ipv6.cpython-311.pyc
--rw-rw-rw-   0        0        0      169 2023-05-26 06:09:27.000000 PyIpify-0.0.2/PyIpify/syncronous/find_ipv4.py
--rw-rw-rw-   0        0        0      179 2023-05-26 11:09:54.000000 PyIpify-0.0.2/PyIpify/syncronous/find_ipv6.py
-drwxrwxrwx   0        0        0        0 2023-05-26 11:14:28.628628 PyIpify-0.0.2/PyIpify.egg-info/
--rw-rw-rw-   0        0        0     1061 2023-05-26 11:14:28.000000 PyIpify-0.0.2/PyIpify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1127 2023-05-26 11:14:28.000000 PyIpify-0.0.2/PyIpify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 11:14:28.000000 PyIpify-0.0.2/PyIpify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-05-26 11:14:28.000000 PyIpify-0.0.2/PyIpify.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-26 11:14:28.000000 PyIpify-0.0.2/PyIpify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-05-26 06:09:27.000000 PyIpify-0.0.2/README.md
--rw-rw-rw-   0        0        0    11549 2023-05-26 06:09:27.000000 PyIpify-0.0.2/license.md
--rw-rw-rw-   0        0        0      232 2023-05-26 11:10:17.000000 PyIpify-0.0.2/main.py
--rw-rw-rw-   0        0        0       28 2023-05-26 06:09:27.000000 PyIpify-0.0.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 11:14:28.674994 PyIpify-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1772 2023-05-26 11:11:20.000000 PyIpify-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 10:20:11.449116 PyIpify-0.0.3/
+-rw-rw-rw-   0        0        0     3207 2023-05-30 10:20:11.449116 PyIpify-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-30 10:20:11.305926 PyIpify-0.0.3/PyIpify/
+-rw-rw-rw-   0        0        0       38 2023-05-30 09:50:44.000000 PyIpify-0.0.3/PyIpify/__init__.py
+-rw-rw-rw-   0        0        0     1380 2023-05-30 10:03:50.000000 PyIpify-0.0.3/PyIpify/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 10:20:11.384818 PyIpify-0.0.3/PyIpify/asyncronous/
+-rw-rw-rw-   0        0        0      106 2023-05-30 10:10:28.000000 PyIpify-0.0.3/PyIpify/asyncronous/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 10:20:11.415011 PyIpify-0.0.3/PyIpify/asyncronous/__pycache__/
+-rw-rw-rw-   0        0        0      201 2023-05-30 09:50:44.000000 PyIpify-0.0.3/PyIpify/asyncronous/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      247 2023-05-30 09:50:44.000000 PyIpify-0.0.3/PyIpify/asyncronous/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      522 2023-05-30 09:50:44.000000 PyIpify-0.0.3/PyIpify/asyncronous/__pycache__/find_ipv4.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1294 2023-05-30 09:50:44.000000 PyIpify-0.0.3/PyIpify/asyncronous/__pycache__/find_ipv4.cpython-311.pyc
+-rw-rw-rw-   0        0        0      523 2023-05-30 09:50:44.000000 PyIpify-0.0.3/PyIpify/asyncronous/__pycache__/find_ipv6.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1295 2023-05-30 09:50:44.000000 PyIpify-0.0.3/PyIpify/asyncronous/__pycache__/find_ipv6.cpython-311.pyc
+-rw-rw-rw-   0        0        0      542 2023-05-30 09:54:05.000000 PyIpify-0.0.3/PyIpify/asyncronous/find_ipv4.py
+-rw-rw-rw-   0        0        0      569 2023-05-30 09:54:51.000000 PyIpify-0.0.3/PyIpify/asyncronous/find_ipv6.py
+drwxrwxrwx   0        0        0        0 2023-05-30 10:20:11.416530 PyIpify-0.0.3/PyIpify/syncronous/
+-rw-rw-rw-   0        0        0      104 2023-05-30 10:10:24.000000 PyIpify-0.0.3/PyIpify/syncronous/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 10:20:11.447807 PyIpify-0.0.3/PyIpify/syncronous/__pycache__/
+-rw-rw-rw-   0        0        0      200 2023-05-30 09:50:44.000000 PyIpify-0.0.3/PyIpify/syncronous/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      246 2023-05-30 09:50:44.000000 PyIpify-0.0.3/PyIpify/syncronous/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0      373 2023-05-30 09:50:44.000000 PyIpify-0.0.3/PyIpify/syncronous/__pycache__/find_ipv4.cpython-310.pyc
+-rw-rw-rw-   0        0        0      516 2023-05-30 09:50:44.000000 PyIpify-0.0.3/PyIpify/syncronous/__pycache__/find_ipv4.cpython-311.pyc
+-rw-rw-rw-   0        0        0      374 2023-05-30 09:50:44.000000 PyIpify-0.0.3/PyIpify/syncronous/__pycache__/find_ipv6.cpython-310.pyc
+-rw-rw-rw-   0        0        0      517 2023-05-30 09:50:44.000000 PyIpify-0.0.3/PyIpify/syncronous/__pycache__/find_ipv6.cpython-311.pyc
+-rw-rw-rw-   0        0        0      404 2023-05-30 09:55:37.000000 PyIpify-0.0.3/PyIpify/syncronous/find_ipv4.py
+-rw-rw-rw-   0        0        0      400 2023-05-30 09:56:00.000000 PyIpify-0.0.3/PyIpify/syncronous/find_ipv6.py
+drwxrwxrwx   0        0        0        0 2023-05-30 10:20:11.369198 PyIpify-0.0.3/PyIpify.egg-info/
+-rw-rw-rw-   0        0        0     3207 2023-05-30 10:20:11.000000 PyIpify-0.0.3/PyIpify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1167 2023-05-30 10:20:11.000000 PyIpify-0.0.3/PyIpify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 10:20:11.000000 PyIpify-0.0.3/PyIpify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-05-30 10:20:11.000000 PyIpify-0.0.3/PyIpify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-30 10:20:11.000000 PyIpify-0.0.3/PyIpify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2144 2023-05-30 09:51:34.000000 PyIpify-0.0.3/README.md
+-rw-rw-rw-   0        0        0    11549 2023-05-30 09:50:44.000000 PyIpify-0.0.3/license.md
+-rw-rw-rw-   0        0        0      232 2023-05-30 09:53:00.000000 PyIpify-0.0.3/main.py
+-rw-rw-rw-   0        0        0       28 2023-05-30 09:50:44.000000 PyIpify-0.0.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 10:20:11.449116 PyIpify-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1772 2023-05-30 10:19:41.000000 PyIpify-0.0.3/setup.py
```

### Comparing `PyIpify-0.0.2/PyIpify/__main__.py` & `PyIpify-0.0.3/PyIpify/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from .syncronous import find_ipv4 as sync_find_ipv4
-from .syncronous import find_ipv6 as sync_find_ipv6
-from .asyncronous import find_ipv4 as async_find_ipv4
-from .asyncronous import find_ipv6 as async_find_ipv6
+from Pyipify.syncronous import find_ipv4 as sync_find_ipv4
+from Pyipify.syncronous import find_ipv6 as sync_find_ipv6
+from Pyipify.asyncronous import find_ipv4 as async_find_ipv4
+from Pyipify.asyncronous import find_ipv6 as async_find_ipv6
 import argparse
 import asyncio
 
 parser = argparse.ArgumentParser(description = "The programm to find the ipv4 and ipv6 address of the system.")
 
 
 parser.add_argument("-v","--version", choices = ["ipv4", "ipv6"], help = "The version of the ip address to be found. Default is ipv4 use ipv4 for ipv4 address and ipv6 for ipv6 addresses", default = "ipv4")
```

### Comparing `PyIpify-0.0.2/PyIpify/asyncronous/__pycache__/find_ipv4.cpython-310.pyc` & `PyIpify-0.0.3/PyIpify/asyncronous/__pycache__/find_ipv4.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `PyIpify-0.0.2/PyIpify/asyncronous/__pycache__/find_ipv4.cpython-311.pyc` & `PyIpify-0.0.3/PyIpify/asyncronous/__pycache__/find_ipv4.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `PyIpify-0.0.2/PyIpify/asyncronous/__pycache__/find_ipv6.cpython-310.pyc` & `PyIpify-0.0.3/PyIpify/asyncronous/__pycache__/find_ipv6.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `PyIpify-0.0.2/PyIpify/asyncronous/__pycache__/find_ipv6.cpython-311.pyc` & `PyIpify-0.0.3/PyIpify/asyncronous/__pycache__/find_ipv6.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `PyIpify-0.0.2/PyIpify/syncronous/__pycache__/find_ipv4.cpython-311.pyc` & `PyIpify-0.0.3/PyIpify/syncronous/__pycache__/find_ipv4.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `PyIpify-0.0.2/PyIpify/syncronous/__pycache__/find_ipv6.cpython-311.pyc` & `PyIpify-0.0.3/PyIpify/syncronous/__pycache__/find_ipv6.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `PyIpify-0.0.2/PyIpify.egg-info/SOURCES.txt` & `PyIpify-0.0.3/PyIpify.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -23,8 +23,10 @@
 PyIpify/syncronous/find_ipv4.py
 PyIpify/syncronous/find_ipv6.py
 PyIpify/syncronous/__pycache__/__init__.cpython-310.pyc
 PyIpify/syncronous/__pycache__/__init__.cpython-311.pyc
 PyIpify/syncronous/__pycache__/find_ipv4.cpython-310.pyc
 PyIpify/syncronous/__pycache__/find_ipv4.cpython-311.pyc
 PyIpify/syncronous/__pycache__/find_ipv6.cpython-310.pyc
-PyIpify/syncronous/__pycache__/find_ipv6.cpython-311.pyc
+PyIpify/syncronous/__pycache__/find_ipv6.cpython-311.pyc
+Pyipify/__init__.py
+Pyipify/__main__.py
```

### Comparing `PyIpify-0.0.2/license.md` & `PyIpify-0.0.3/license.md`

 * *Files identical despite different names*

### Comparing `PyIpify-0.0.2/setup.py` & `PyIpify-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
     with open(str(pathlib.Path(dir_path) / "requirements.txt"), "r") as f:
         requirements = [line.strip() for line in f]
         return requirements
 
 
 setup(
     name="PyIpify",
-    packages=['PyIpify', 'PyIpify.syncronous', 'PyIpify.asyncronous'],
-    version="0.0.2",
+    packages=['Pyipify', 'PyIpify.syncronous', 'PyIpify.asyncronous'],
+    version="0.0.3",
     setup_requires=['setuptools_scm'],
     license="MIT",
     description="A simple python library to find the public ip address of the system.",
     author="SigireddyBalasai",
     author_email="sigireddybalasai@gmail.com",
     url="https://github.com/SigireddyBalasai/ipify",
     download_url="https://github.com/SigireddyBalasai/AsyncPywhatKit/archive/refs/tags/1.0.tar.gz",
```

