# Comparing `tmp/keyauth-tech-0.0.3.tar.gz` & `tmp/keyauth-tech-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyauth-tech-0.0.3.tar", last modified: Thu May 25 15:16:22 2023, max compression
+gzip compressed data, was "keyauth-tech-0.0.4.tar", last modified: Tue May 30 15:02:13 2023, max compression
```

## Comparing `keyauth-tech-0.0.3.tar` & `keyauth-tech-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ecom       (502) staff       (20)        0 2023-05-25 15:16:22.863857 keyauth-tech-0.0.3/
--rw-r--r--   0 ecom       (502) staff       (20)       84 2023-05-25 15:15:38.000000 keyauth-tech-0.0.3/CHANGELOG.txt
--rw-r--r--   0 ecom       (502) staff       (20)     1046 2023-05-24 11:06:49.000000 keyauth-tech-0.0.3/LICENSE.txt
--rw-r--r--   0 ecom       (502) staff       (20)       25 2023-05-24 11:06:11.000000 keyauth-tech-0.0.3/MANIFEST.in
--rw-r--r--   0 ecom       (502) staff       (20)      805 2023-05-25 15:16:22.863722 keyauth-tech-0.0.3/PKG-INFO
--rw-r--r--   0 ecom       (502) staff       (20)      116 2023-05-24 11:09:48.000000 keyauth-tech-0.0.3/README.txt
-drwxr-xr-x   0 ecom       (502) staff       (20)        0 2023-05-25 15:16:22.862862 keyauth-tech-0.0.3/keyauth/
--rw-r--r--   0 ecom       (502) staff       (20)     2487 2023-05-25 15:13:23.000000 keyauth-tech-0.0.3/keyauth/__init__.py
-drwxr-xr-x   0 ecom       (502) staff       (20)        0 2023-05-25 15:16:22.863519 keyauth-tech-0.0.3/keyauth_tech.egg-info/
--rw-r--r--   0 ecom       (502) staff       (20)      805 2023-05-25 15:16:22.000000 keyauth-tech-0.0.3/keyauth_tech.egg-info/PKG-INFO
--rw-r--r--   0 ecom       (502) staff       (20)      264 2023-05-25 15:16:22.000000 keyauth-tech-0.0.3/keyauth_tech.egg-info/SOURCES.txt
--rw-r--r--   0 ecom       (502) staff       (20)        1 2023-05-25 15:16:22.000000 keyauth-tech-0.0.3/keyauth_tech.egg-info/dependency_links.txt
--rw-r--r--   0 ecom       (502) staff       (20)       18 2023-05-25 15:16:22.000000 keyauth-tech-0.0.3/keyauth_tech.egg-info/requires.txt
--rw-r--r--   0 ecom       (502) staff       (20)        8 2023-05-25 15:16:22.000000 keyauth-tech-0.0.3/keyauth_tech.egg-info/top_level.txt
--rw-r--r--   0 ecom       (502) staff       (20)       38 2023-05-25 15:16:22.863898 keyauth-tech-0.0.3/setup.cfg
--rw-r--r--   0 ecom       (502) staff       (20)      811 2023-05-25 15:16:19.000000 keyauth-tech-0.0.3/setup.py
--rw-r--r--   0 ecom       (502) staff       (20)      232 2023-05-24 11:31:31.000000 keyauth-tech-0.0.3/test.py
+drwxr-xr-x   0 ecom       (502) staff       (20)        0 2023-05-30 15:02:13.485990 keyauth-tech-0.0.4/
+-rw-r--r--   0 ecom       (502) staff       (20)      262 2023-05-30 14:59:42.000000 keyauth-tech-0.0.4/CHANGELOG.txt
+-rw-r--r--   0 ecom       (502) staff       (20)     1046 2023-05-24 11:06:49.000000 keyauth-tech-0.0.4/LICENSE.txt
+-rw-r--r--   0 ecom       (502) staff       (20)       25 2023-05-24 11:06:11.000000 keyauth-tech-0.0.4/MANIFEST.in
+-rw-r--r--   0 ecom       (502) staff       (20)     1564 2023-05-30 15:02:13.485838 keyauth-tech-0.0.4/PKG-INFO
+-rw-r--r--   0 ecom       (502) staff       (20)      559 2023-05-30 15:01:43.000000 keyauth-tech-0.0.4/README.md
+drwxr-xr-x   0 ecom       (502) staff       (20)        0 2023-05-30 15:02:13.484898 keyauth-tech-0.0.4/keyauth/
+-rw-r--r--   0 ecom       (502) staff       (20)     2487 2023-05-25 15:13:23.000000 keyauth-tech-0.0.4/keyauth/__init__.py
+drwxr-xr-x   0 ecom       (502) staff       (20)        0 2023-05-30 15:02:13.485623 keyauth-tech-0.0.4/keyauth_tech.egg-info/
+-rw-r--r--   0 ecom       (502) staff       (20)     1564 2023-05-30 15:02:13.000000 keyauth-tech-0.0.4/keyauth_tech.egg-info/PKG-INFO
+-rw-r--r--   0 ecom       (502) staff       (20)      263 2023-05-30 15:02:13.000000 keyauth-tech-0.0.4/keyauth_tech.egg-info/SOURCES.txt
+-rw-r--r--   0 ecom       (502) staff       (20)        1 2023-05-30 15:02:13.000000 keyauth-tech-0.0.4/keyauth_tech.egg-info/dependency_links.txt
+-rw-r--r--   0 ecom       (502) staff       (20)       18 2023-05-30 15:02:13.000000 keyauth-tech-0.0.4/keyauth_tech.egg-info/requires.txt
+-rw-r--r--   0 ecom       (502) staff       (20)        8 2023-05-30 15:02:13.000000 keyauth-tech-0.0.4/keyauth_tech.egg-info/top_level.txt
+-rw-r--r--   0 ecom       (502) staff       (20)       38 2023-05-30 15:02:13.486033 keyauth-tech-0.0.4/setup.cfg
+-rw-r--r--   0 ecom       (502) staff       (20)     1240 2023-05-30 15:02:03.000000 keyauth-tech-0.0.4/setup.py
+-rw-r--r--   0 ecom       (502) staff       (20)      232 2023-05-26 15:27:52.000000 keyauth-tech-0.0.4/test.py
```

### Comparing `keyauth-tech-0.0.3/LICENSE.txt` & `keyauth-tech-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `keyauth-tech-0.0.3/keyauth/__init__.py` & `keyauth-tech-0.0.4/keyauth/__init__.py`

 * *Files identical despite different names*

