# Comparing `tmp/p1-activity-0.2.55075241.tar.gz` & `tmp/p1-activity-0.2.55280185.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/p1-activity-0.2.55075241.tar", last modified: Tue Nov 15 20:45:42 2022, max compression
+gzip compressed data, was "dist/p1-activity-0.2.55280185.tar", last modified: Wed Dec 28 10:38:24 2022, max compression
```

## Comparing `p1-activity-0.2.55075241.tar` & `p1-activity-0.2.55280185.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2022-11-15 20:45:42.000000 p1-activity-0.2.55075241/
--rw-rw-r--   0 rof       (1001) rof       (1001)       38 2022-11-15 20:45:42.000000 p1-activity-0.2.55075241/setup.cfg
--rw-rw-r--   0 rof       (1001) rof       (1001)     1233 2022-11-15 20:45:42.000000 p1-activity-0.2.55075241/PKG-INFO
--rw-rw-r--   0 rof       (1001) rof       (1001)     1064 2022-11-15 20:45:30.000000 p1-activity-0.2.55075241/setup.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      374 2022-11-15 20:45:18.000000 p1-activity-0.2.55075241/README.rst
--rw-rw-r--   0 rof       (1001) rof       (1001)      109 2022-11-15 20:45:18.000000 p1-activity-0.2.55075241/MANIFEST.in
--rw-rw-r--   0 rof       (1001) rof       (1001)     1051 2022-11-15 20:45:18.000000 p1-activity-0.2.55075241/LICENSE
-drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2022-11-15 20:45:42.000000 p1-activity-0.2.55075241/p1_activity.egg-info/
--rw-rw-r--   0 rof       (1001) rof       (1001)        9 2022-11-15 20:45:42.000000 p1-activity-0.2.55075241/p1_activity.egg-info/top_level.txt
--rw-rw-r--   0 rof       (1001) rof       (1001)       23 2022-11-15 20:45:42.000000 p1-activity-0.2.55075241/p1_activity.egg-info/requires.txt
--rw-rw-r--   0 rof       (1001) rof       (1001)        1 2022-11-15 20:45:42.000000 p1-activity-0.2.55075241/p1_activity.egg-info/dependency_links.txt
--rw-rw-r--   0 rof       (1001) rof       (1001)      495 2022-11-15 20:45:42.000000 p1-activity-0.2.55075241/p1_activity.egg-info/SOURCES.txt
--rw-rw-r--   0 rof       (1001) rof       (1001)     1233 2022-11-15 20:45:42.000000 p1-activity-0.2.55075241/p1_activity.egg-info/PKG-INFO
-drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2022-11-15 20:45:42.000000 p1-activity-0.2.55075241/activity/
--rw-rw-r--   0 rof       (1001) rof       (1001)     5365 2022-11-15 20:45:18.000000 p1-activity-0.2.55075241/activity/views.py
--rw-rw-r--   0 rof       (1001) rof       (1001)    12990 2022-11-15 20:45:18.000000 p1-activity-0.2.55075241/activity/services.py
--rw-rw-r--   0 rof       (1001) rof       (1001)     1619 2022-11-15 20:45:18.000000 p1-activity-0.2.55075241/activity/models.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      389 2022-11-15 20:45:18.000000 p1-activity-0.2.55075241/activity/factories.py
--rw-rw-r--   0 rof       (1001) rof       (1001)     5016 2022-11-15 20:45:18.000000 p1-activity-0.2.55075241/activity/consumer.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      984 2022-11-15 20:45:18.000000 p1-activity-0.2.55075241/activity/constants.py
--rw-rw-r--   0 rof       (1001) rof       (1001)    10012 2022-11-15 20:45:18.000000 p1-activity-0.2.55075241/activity/client.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      132 2022-11-15 20:45:18.000000 p1-activity-0.2.55075241/activity/apps.py
--rw-rw-r--   0 rof       (1001) rof       (1001)     3153 2022-11-15 20:45:18.000000 p1-activity-0.2.55075241/activity/api.py
--rw-rw-r--   0 rof       (1001) rof       (1001)      667 2022-11-15 20:45:18.000000 p1-activity-0.2.55075241/activity/admin.py
--rw-rw-r--   0 rof       (1001) rof       (1001)        0 2022-11-15 20:45:18.000000 p1-activity-0.2.55075241/activity/__init__.py
-drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2022-11-15 20:45:42.000000 p1-activity-0.2.55075241/activity/migrations/
--rw-rw-r--   0 rof       (1001) rof       (1001)        0 2022-11-15 20:45:18.000000 p1-activity-0.2.55075241/activity/migrations/__init__.py
--rw-rw-r--   0 rof       (1001) rof       (1001)     2305 2022-11-15 20:45:18.000000 p1-activity-0.2.55075241/activity/migrations/0001_initial.py
+drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2022-12-28 10:38:24.000000 p1-activity-0.2.55280185/
+-rw-rw-r--   0 rof       (1001) rof       (1001)       38 2022-12-28 10:38:24.000000 p1-activity-0.2.55280185/setup.cfg
+-rw-rw-r--   0 rof       (1001) rof       (1001)     1233 2022-12-28 10:38:24.000000 p1-activity-0.2.55280185/PKG-INFO
+-rw-rw-r--   0 rof       (1001) rof       (1001)     1064 2022-12-28 10:38:06.000000 p1-activity-0.2.55280185/setup.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      374 2022-12-28 10:37:54.000000 p1-activity-0.2.55280185/README.rst
+-rw-rw-r--   0 rof       (1001) rof       (1001)      109 2022-12-28 10:37:54.000000 p1-activity-0.2.55280185/MANIFEST.in
+-rw-rw-r--   0 rof       (1001) rof       (1001)     1051 2022-12-28 10:37:54.000000 p1-activity-0.2.55280185/LICENSE
+drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2022-12-28 10:38:24.000000 p1-activity-0.2.55280185/p1_activity.egg-info/
+-rw-rw-r--   0 rof       (1001) rof       (1001)        9 2022-12-28 10:38:24.000000 p1-activity-0.2.55280185/p1_activity.egg-info/top_level.txt
+-rw-rw-r--   0 rof       (1001) rof       (1001)       23 2022-12-28 10:38:24.000000 p1-activity-0.2.55280185/p1_activity.egg-info/requires.txt
+-rw-rw-r--   0 rof       (1001) rof       (1001)        1 2022-12-28 10:38:24.000000 p1-activity-0.2.55280185/p1_activity.egg-info/dependency_links.txt
+-rw-rw-r--   0 rof       (1001) rof       (1001)      495 2022-12-28 10:38:24.000000 p1-activity-0.2.55280185/p1_activity.egg-info/SOURCES.txt
+-rw-rw-r--   0 rof       (1001) rof       (1001)     1233 2022-12-28 10:38:24.000000 p1-activity-0.2.55280185/p1_activity.egg-info/PKG-INFO
+drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2022-12-28 10:38:24.000000 p1-activity-0.2.55280185/activity/
+-rw-rw-r--   0 rof       (1001) rof       (1001)     5365 2022-12-28 10:37:54.000000 p1-activity-0.2.55280185/activity/views.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)    12990 2022-12-28 10:37:54.000000 p1-activity-0.2.55280185/activity/services.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)     1619 2022-12-28 10:37:54.000000 p1-activity-0.2.55280185/activity/models.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      389 2022-12-28 10:37:54.000000 p1-activity-0.2.55280185/activity/factories.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)     5016 2022-12-28 10:37:54.000000 p1-activity-0.2.55280185/activity/consumer.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      984 2022-12-28 10:37:54.000000 p1-activity-0.2.55280185/activity/constants.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)    10012 2022-12-28 10:37:54.000000 p1-activity-0.2.55280185/activity/client.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      132 2022-12-28 10:37:54.000000 p1-activity-0.2.55280185/activity/apps.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)     3153 2022-12-28 10:37:54.000000 p1-activity-0.2.55280185/activity/api.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)      667 2022-12-28 10:37:54.000000 p1-activity-0.2.55280185/activity/admin.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)        0 2022-12-28 10:37:54.000000 p1-activity-0.2.55280185/activity/__init__.py
+drwxrwxr-x   0 rof       (1001) rof       (1001)        0 2022-12-28 10:38:24.000000 p1-activity-0.2.55280185/activity/migrations/
+-rw-rw-r--   0 rof       (1001) rof       (1001)        0 2022-12-28 10:37:54.000000 p1-activity-0.2.55280185/activity/migrations/__init__.py
+-rw-rw-r--   0 rof       (1001) rof       (1001)     2305 2022-12-28 10:37:54.000000 p1-activity-0.2.55280185/activity/migrations/0001_initial.py
```

### Comparing `p1-activity-0.2.55075241/PKG-INFO` & `p1-activity-0.2.55280185/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: p1-activity
-Version: 0.2.55075241
+Version: 0.2.55280185
 Summary: A simple consumer Django app for Activity Service.
 Home-page: UNKNOWN
 Author: Yonas & Wisnu
 Author-email: yonazadielwiguna@gmail.com
 License: MIT
 Description: ================
         Activity
```

### Comparing `p1-activity-0.2.55075241/setup.py` & `p1-activity-0.2.55280185/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,21 +5,21 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='p1-activity',
-    version='0.2.55075241',
+    version='0.2.55280185',
     packages=find_packages(),
     include_package_data=True,
     license='MIT',
     description='A simple consumer Django app for Activity Service.',
     long_description=README,
-    install_requires=['p1-queue == 0.3.55075234'],
+    install_requires=['p1-queue >= 0.3.55075234'],
     author='Yonas & Wisnu',
     author_email='yonazadielwiguna@gmail.com',
     classifiers=[
         'Environment :: Web Environment',
         'Framework :: Django',
         'Framework :: Django :: 1.11',
         'Intended Audience :: Developers',
```

### Comparing `p1-activity-0.2.55075241/LICENSE` & `p1-activity-0.2.55280185/LICENSE`

 * *Files identical despite different names*

### Comparing `p1-activity-0.2.55075241/p1_activity.egg-info/PKG-INFO` & `p1-activity-0.2.55280185/p1_activity.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: p1-activity
-Version: 0.2.55075241
+Version: 0.2.55280185
 Summary: A simple consumer Django app for Activity Service.
 Home-page: UNKNOWN
 Author: Yonas & Wisnu
 Author-email: yonazadielwiguna@gmail.com
 License: MIT
 Description: ================
         Activity
```

### Comparing `p1-activity-0.2.55075241/activity/views.py` & `p1-activity-0.2.55280185/activity/views.py`

 * *Files identical despite different names*

### Comparing `p1-activity-0.2.55075241/activity/services.py` & `p1-activity-0.2.55280185/activity/services.py`

 * *Files identical despite different names*

### Comparing `p1-activity-0.2.55075241/activity/models.py` & `p1-activity-0.2.55280185/activity/models.py`

 * *Files identical despite different names*

### Comparing `p1-activity-0.2.55075241/activity/consumer.py` & `p1-activity-0.2.55280185/activity/consumer.py`

 * *Files identical despite different names*

### Comparing `p1-activity-0.2.55075241/activity/constants.py` & `p1-activity-0.2.55280185/activity/constants.py`

 * *Files identical despite different names*

### Comparing `p1-activity-0.2.55075241/activity/client.py` & `p1-activity-0.2.55280185/activity/client.py`

 * *Files identical despite different names*

### Comparing `p1-activity-0.2.55075241/activity/api.py` & `p1-activity-0.2.55280185/activity/api.py`

 * *Files identical despite different names*

### Comparing `p1-activity-0.2.55075241/activity/admin.py` & `p1-activity-0.2.55280185/activity/admin.py`

 * *Files identical despite different names*

### Comparing `p1-activity-0.2.55075241/activity/migrations/0001_initial.py` & `p1-activity-0.2.55280185/activity/migrations/0001_initial.py`

 * *Files identical despite different names*

