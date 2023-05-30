# Comparing `tmp/abuscom-libs-0.1.7.tar.gz` & `tmp/abuscom-libs-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abuscom-libs-0.1.7.tar", last modified: Thu May 25 06:53:26 2023, max compression
+gzip compressed data, was "abuscom-libs-0.1.8.tar", last modified: Tue May 30 07:23:18 2023, max compression
```

## Comparing `abuscom-libs-0.1.7.tar` & `abuscom-libs-0.1.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-05-25 06:53:26.983530 abuscom-libs-0.1.7/
--rw-r--r--   0 leonhardholzer   (501) staff       (20)      434 2023-05-25 06:53:26.983093 abuscom-libs-0.1.7/PKG-INFO
--rw-r--r--   0 leonhardholzer   (501) staff       (20)      872 2023-02-22 14:35:31.000000 abuscom-libs-0.1.7/README.md
-drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-05-25 06:53:26.974801 abuscom-libs-0.1.7/abuscom/
-drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-05-25 06:53:26.979602 abuscom-libs-0.1.7/abuscom/connectors/
--rw-r--r--   0 leonhardholzer   (501) staff       (20)        0 2023-02-02 10:20:51.000000 abuscom-libs-0.1.7/abuscom/connectors/__init__.py
--rw-r--r--   0 leonhardholzer   (501) staff       (20)     1887 2023-04-19 09:17:07.000000 abuscom-libs-0.1.7/abuscom/connectors/compass.py
--rw-r--r--   0 leonhardholzer   (501) staff       (20)     8661 2023-05-25 06:52:16.000000 abuscom-libs-0.1.7/abuscom/connectors/hubspot.py
--rw-r--r--   0 leonhardholzer   (501) staff       (20)     6017 2023-04-24 10:02:05.000000 abuscom-libs-0.1.7/abuscom/connectors/oracle.py
--rw-r--r--   0 leonhardholzer   (501) staff       (20)     6775 2023-02-21 17:20:25.000000 abuscom-libs-0.1.7/abuscom/connectors/planio.py
--rw-r--r--   0 leonhardholzer   (501) staff       (20)     5759 2023-04-07 09:46:30.000000 abuscom-libs-0.1.7/abuscom/connectors/postgres.py
-drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-05-25 06:53:26.982396 abuscom-libs-0.1.7/abuscom_libs.egg-info/
--rw-r--r--   0 leonhardholzer   (501) staff       (20)      434 2023-05-25 06:53:26.000000 abuscom-libs-0.1.7/abuscom_libs.egg-info/PKG-INFO
--rw-r--r--   0 leonhardholzer   (501) staff       (20)      377 2023-05-25 06:53:26.000000 abuscom-libs-0.1.7/abuscom_libs.egg-info/SOURCES.txt
--rw-r--r--   0 leonhardholzer   (501) staff       (20)        1 2023-05-25 06:53:26.000000 abuscom-libs-0.1.7/abuscom_libs.egg-info/dependency_links.txt
--rw-r--r--   0 leonhardholzer   (501) staff       (20)       29 2023-05-25 06:53:26.000000 abuscom-libs-0.1.7/abuscom_libs.egg-info/requires.txt
--rw-r--r--   0 leonhardholzer   (501) staff       (20)        8 2023-05-25 06:53:26.000000 abuscom-libs-0.1.7/abuscom_libs.egg-info/top_level.txt
--rw-r--r--   0 leonhardholzer   (501) staff       (20)       38 2023-05-25 06:53:26.983688 abuscom-libs-0.1.7/setup.cfg
--rw-r--r--   0 leonhardholzer   (501) staff       (20)      652 2023-05-25 06:52:34.000000 abuscom-libs-0.1.7/setup.py
+drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-05-30 07:23:18.838643 abuscom-libs-0.1.8/
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)      434 2023-05-30 07:23:18.838243 abuscom-libs-0.1.8/PKG-INFO
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)      872 2023-02-22 14:35:31.000000 abuscom-libs-0.1.8/README.md
+drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-05-30 07:23:18.828916 abuscom-libs-0.1.8/abuscom/
+drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-05-30 07:23:18.834780 abuscom-libs-0.1.8/abuscom/connectors/
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)        0 2023-02-02 10:20:51.000000 abuscom-libs-0.1.8/abuscom/connectors/__init__.py
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)     2112 2023-05-30 07:21:43.000000 abuscom-libs-0.1.8/abuscom/connectors/compass.py
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)     8661 2023-05-25 06:52:16.000000 abuscom-libs-0.1.8/abuscom/connectors/hubspot.py
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)     6017 2023-04-24 10:02:05.000000 abuscom-libs-0.1.8/abuscom/connectors/oracle.py
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)     6775 2023-02-21 17:20:25.000000 abuscom-libs-0.1.8/abuscom/connectors/planio.py
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)     5759 2023-04-07 09:46:30.000000 abuscom-libs-0.1.8/abuscom/connectors/postgres.py
+drwxr-xr-x   0 leonhardholzer   (501) staff       (20)        0 2023-05-30 07:23:18.837696 abuscom-libs-0.1.8/abuscom_libs.egg-info/
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)      434 2023-05-30 07:23:18.000000 abuscom-libs-0.1.8/abuscom_libs.egg-info/PKG-INFO
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)      377 2023-05-30 07:23:18.000000 abuscom-libs-0.1.8/abuscom_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)        1 2023-05-30 07:23:18.000000 abuscom-libs-0.1.8/abuscom_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)       29 2023-05-30 07:23:18.000000 abuscom-libs-0.1.8/abuscom_libs.egg-info/requires.txt
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)        8 2023-05-30 07:23:18.000000 abuscom-libs-0.1.8/abuscom_libs.egg-info/top_level.txt
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)       38 2023-05-30 07:23:18.838758 abuscom-libs-0.1.8/setup.cfg
+-rw-r--r--   0 leonhardholzer   (501) staff       (20)      652 2023-05-30 07:22:33.000000 abuscom-libs-0.1.8/setup.py
```

### Comparing `abuscom-libs-0.1.7/README.md` & `abuscom-libs-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `abuscom-libs-0.1.7/abuscom/connectors/compass.py` & `abuscom-libs-0.1.8/abuscom/connectors/compass.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,15 +12,17 @@
         tuples= []
         for i, row in df.iterrows():
             tuple = ()
 
             for idx, column in enumerate(columns):
                 try:
                     timestamp = row[idx].getTime() / 1000
-                    tuple = tuple + (datetime.datetime.fromtimestamp(timestamp),)
+                    tuple = tuple + (datetime.datetime.fromtimestamp(timestamp).astimezone().isoformat(),)
+                    print ('formatted date: ', datetime.datetime.fromtimestamp(timestamp).astimezone().isoformat())
+                    # tuple = tuple + (datetime.datetime.fromtimestamp(timestamp),)
                 except AttributeError:
                     tuple = tuple + (row[idx],)
             tuples.append(tuple)
 
         return tuples
```

### Comparing `abuscom-libs-0.1.7/abuscom/connectors/hubspot.py` & `abuscom-libs-0.1.8/abuscom/connectors/hubspot.py`

 * *Files identical despite different names*

### Comparing `abuscom-libs-0.1.7/abuscom/connectors/oracle.py` & `abuscom-libs-0.1.8/abuscom/connectors/oracle.py`

 * *Files identical despite different names*

### Comparing `abuscom-libs-0.1.7/abuscom/connectors/planio.py` & `abuscom-libs-0.1.8/abuscom/connectors/planio.py`

 * *Files identical despite different names*

### Comparing `abuscom-libs-0.1.7/abuscom/connectors/postgres.py` & `abuscom-libs-0.1.8/abuscom/connectors/postgres.py`

 * *Files identical despite different names*

### Comparing `abuscom-libs-0.1.7/setup.py` & `abuscom-libs-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='abuscom-libs',
-    version='0.1.7',
+    version='0.1.8',
     description='Utility classes for airflow DAGs',
     url='https://abuscom.com',
     author='Leonhard Holzer',
     author_email='leonhard.holzer@abuscom.com',
     license='BSD 2-clause',
     packages=['abuscom.connectors'],
     install_requires=['apache-airflow>=2.4.3',
```

