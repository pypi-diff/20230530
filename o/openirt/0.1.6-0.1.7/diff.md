# Comparing `tmp/openirt-0.1.6.tar.gz` & `tmp/openirt-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openirt-0.1.6.tar", last modified: Tue May 30 09:08:52 2023, max compression
+gzip compressed data, was "openirt-0.1.7.tar", last modified: Tue May 30 12:30:57 2023, max compression
```

## Comparing `openirt-0.1.6.tar` & `openirt-0.1.7.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 09:08:52.019738 openirt-0.1.6/
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-05-30 09:08:34.000000 openirt-0.1.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      256 2023-05-30 09:08:52.019738 openirt-0.1.6/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-05-30 09:08:34.000000 openirt-0.1.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 09:08:52.017738 openirt-0.1.6/openirt/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 09:08:34.000000 openirt-0.1.6/openirt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6938 2023-05-30 09:08:34.000000 openirt-0.1.6/openirt/bayes3PL.py
--rw-rw-rw-   0 root         (0) root         (0)     2081 2023-05-30 09:08:34.000000 openirt-0.1.6/openirt/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     3932 2023-05-30 09:08:34.000000 openirt-0.1.6/openirt/irt_instance.py
--rw-rw-rw-   0 root         (0) root         (0)     1488 2023-05-30 09:08:34.000000 openirt-0.1.6/openirt/item_model.py
--rw-rw-rw-   0 root         (0) root         (0)     3387 2023-05-30 09:08:34.000000 openirt-0.1.6/openirt/norm_model.py
--rw-rw-rw-   0 root         (0) root         (0)     2745 2023-05-30 09:08:34.000000 openirt-0.1.6/openirt/pl1.py
--rw-rw-rw-   0 root         (0) root         (0)     4615 2023-05-30 09:08:34.000000 openirt-0.1.6/openirt/pl2.py
--rw-rw-rw-   0 root         (0) root         (0)     5984 2023-05-30 09:08:34.000000 openirt-0.1.6/openirt/pl3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 09:08:52.018738 openirt-0.1.6/openirt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      256 2023-05-30 09:08:52.000000 openirt-0.1.6/openirt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      337 2023-05-30 09:08:52.000000 openirt-0.1.6/openirt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 09:08:52.000000 openirt-0.1.6/openirt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-30 09:08:52.000000 openirt-0.1.6/openirt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 09:08:52.019738 openirt-0.1.6/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      555 2023-05-30 09:08:34.000000 openirt-0.1.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 09:08:52.018738 openirt-0.1.6/tests/
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-05-30 09:08:34.000000 openirt-0.1.6/tests/test_func.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 12:30:57.089722 openirt-0.1.7/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-05-30 12:30:36.000000 openirt-0.1.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      256 2023-05-30 12:30:57.089722 openirt-0.1.7/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-05-30 12:30:36.000000 openirt-0.1.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 12:30:57.088722 openirt-0.1.7/openirt/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 12:30:36.000000 openirt-0.1.7/openirt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6938 2023-05-30 12:30:36.000000 openirt-0.1.7/openirt/bayes3PL.py
+-rw-rw-rw-   0 root         (0) root         (0)     2081 2023-05-30 12:30:36.000000 openirt-0.1.7/openirt/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     3932 2023-05-30 12:30:36.000000 openirt-0.1.7/openirt/irt_instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     1488 2023-05-30 12:30:36.000000 openirt-0.1.7/openirt/item_model.py
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-05-30 12:30:36.000000 openirt-0.1.7/openirt/newclass.py
+-rw-rw-rw-   0 root         (0) root         (0)     3387 2023-05-30 12:30:36.000000 openirt-0.1.7/openirt/norm_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2745 2023-05-30 12:30:36.000000 openirt-0.1.7/openirt/pl1.py
+-rw-rw-rw-   0 root         (0) root         (0)     4615 2023-05-30 12:30:36.000000 openirt-0.1.7/openirt/pl2.py
+-rw-rw-rw-   0 root         (0) root         (0)     5984 2023-05-30 12:30:36.000000 openirt-0.1.7/openirt/pl3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 12:30:57.089722 openirt-0.1.7/openirt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      256 2023-05-30 12:30:57.000000 openirt-0.1.7/openirt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      357 2023-05-30 12:30:57.000000 openirt-0.1.7/openirt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 12:30:57.000000 openirt-0.1.7/openirt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-30 12:30:57.000000 openirt-0.1.7/openirt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 12:30:57.089722 openirt-0.1.7/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      555 2023-05-30 12:30:36.000000 openirt-0.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 12:30:57.089722 openirt-0.1.7/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-05-30 12:30:36.000000 openirt-0.1.7/tests/test_func.py
```

### Comparing `openirt-0.1.6/LICENSE` & `openirt-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `openirt-0.1.6/openirt/bayes3PL.py` & `openirt-0.1.7/openirt/bayes3PL.py`

 * *Files identical despite different names*

### Comparing `openirt-0.1.6/openirt/cli.py` & `openirt-0.1.7/openirt/cli.py`

 * *Files identical despite different names*

### Comparing `openirt-0.1.6/openirt/irt_instance.py` & `openirt-0.1.7/openirt/irt_instance.py`

 * *Files identical despite different names*

### Comparing `openirt-0.1.6/openirt/item_model.py` & `openirt-0.1.7/openirt/item_model.py`

 * *Files identical despite different names*

### Comparing `openirt-0.1.6/openirt/norm_model.py` & `openirt-0.1.7/openirt/norm_model.py`

 * *Files identical despite different names*

### Comparing `openirt-0.1.6/openirt/pl1.py` & `openirt-0.1.7/openirt/pl1.py`

 * *Files identical despite different names*

### Comparing `openirt-0.1.6/openirt/pl2.py` & `openirt-0.1.7/openirt/pl2.py`

 * *Files identical despite different names*

### Comparing `openirt-0.1.6/openirt/pl3.py` & `openirt-0.1.7/openirt/pl3.py`

 * *Files identical despite different names*

### Comparing `openirt-0.1.6/setup.py` & `openirt-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,13 +10,13 @@
 
 setup(
     name='openirt',
     packages = find_packages(include=['openirt']),
     long_description=get_long_description(),
     long_description_content_type='text/markdown',
     url='https://gitlab.com/pleased/...',
-    version='0.1.6',
+    version='0.1.7',
     description='Item response theory toolkit',
     author='Johan Hay',
     license='MIT',
 )
```

