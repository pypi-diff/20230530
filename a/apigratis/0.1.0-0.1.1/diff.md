# Comparing `tmp/apigratis-0.1.0.tar.gz` & `tmp/apigratis-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apigratis-0.1.0.tar", last modified: Tue May 30 12:37:17 2023, max compression
+gzip compressed data, was "apigratis-0.1.1.tar", last modified: Tue May 30 12:46:05 2023, max compression
```

## Comparing `apigratis-0.1.0.tar` & `apigratis-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 12:37:17.369854 apigratis-0.1.0/
--rw-rw-rw-   0        0        0      454 2023-05-30 12:37:17.368854 apigratis-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2640 2023-05-30 12:37:02.000000 apigratis-0.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-30 12:37:17.346848 apigratis-0.1.0/apigratis/
--rw-rw-rw-   0        0        0     1828 2023-05-29 23:03:05.000000 apigratis-0.1.0/apigratis/Service.py
--rw-rw-rw-   0        0        0        0 2023-05-29 19:43:41.000000 apigratis-0.1.0/apigratis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 12:37:17.366847 apigratis-0.1.0/apigratis.egg-info/
--rw-rw-rw-   0        0        0      454 2023-05-30 12:37:17.000000 apigratis-0.1.0/apigratis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-05-30 12:37:17.000000 apigratis-0.1.0/apigratis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 12:37:17.000000 apigratis-0.1.0/apigratis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-30 12:37:17.000000 apigratis-0.1.0/apigratis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-30 12:37:17.000000 apigratis-0.1.0/apigratis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 12:37:17.369854 apigratis-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      556 2023-05-30 12:36:50.000000 apigratis-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 12:46:05.933198 apigratis-0.1.1/
+-rw-rw-rw-   0        0        0      454 2023-05-30 12:46:05.932196 apigratis-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2640 2023-05-30 12:37:02.000000 apigratis-0.1.1/README
+drwxrwxrwx   0        0        0        0 2023-05-30 12:46:05.910189 apigratis-0.1.1/apigratis/
+-rw-rw-rw-   0        0        0     1828 2023-05-29 23:03:05.000000 apigratis-0.1.1/apigratis/Service.py
+-rw-rw-rw-   0        0        0        0 2023-05-29 19:43:41.000000 apigratis-0.1.1/apigratis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 12:46:05.930197 apigratis-0.1.1/apigratis.egg-info/
+-rw-rw-rw-   0        0        0      454 2023-05-30 12:46:05.000000 apigratis-0.1.1/apigratis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-05-30 12:46:05.000000 apigratis-0.1.1/apigratis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 12:46:05.000000 apigratis-0.1.1/apigratis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-30 12:46:05.000000 apigratis-0.1.1/apigratis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-30 12:46:05.000000 apigratis-0.1.1/apigratis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1198 2023-05-30 12:43:21.000000 apigratis-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-30 12:46:05.933198 apigratis-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      509 2023-05-30 12:45:45.000000 apigratis-0.1.1/setup.py
```

### Comparing `apigratis-0.1.0/README.rst` & `apigratis-0.1.1/README`

 * *Files identical despite different names*

### Comparing `apigratis-0.1.0/apigratis/Service.py` & `apigratis-0.1.1/apigratis/Service.py`

 * *Files identical despite different names*

