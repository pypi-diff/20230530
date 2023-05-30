# Comparing `tmp/ezyquant-execution-0.1.0.tar.gz` & `tmp/ezyquant-execution-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezyquant-execution-0.1.0.tar", last modified: Mon May 29 09:34:13 2023, max compression
+gzip compressed data, was "ezyquant-execution-0.1.1.tar", last modified: Tue May 30 09:06:56 2023, max compression
```

## Comparing `ezyquant-execution-0.1.0.tar` & `ezyquant-execution-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:34:13.259866 ezyquant-execution-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-29 09:33:48.000000 ezyquant-execution-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-29 09:34:13.259866 ezyquant-execution-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-29 09:33:48.000000 ezyquant-execution-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:34:13.259866 ezyquant-execution-0.1.0/ezyquant_execution/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-29 09:33:48.000000 ezyquant-execution-0.1.0/ezyquant_execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-29 09:33:48.000000 ezyquant-execution-0.1.0/ezyquant_execution/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-29 09:33:48.000000 ezyquant-execution-0.1.0/ezyquant_execution/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)    20311 2023-05-29 09:33:48.000000 ezyquant-execution-0.1.0/ezyquant_execution/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-05-29 09:33:48.000000 ezyquant-execution-0.1.0/ezyquant_execution/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-29 09:33:48.000000 ezyquant-execution-0.1.0/ezyquant_execution/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-29 09:33:48.000000 ezyquant-execution-0.1.0/ezyquant_execution/executing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-29 09:33:48.000000 ezyquant-execution-0.1.0/ezyquant_execution/realtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-05-29 09:33:48.000000 ezyquant-execution-0.1.0/ezyquant_execution/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:34:13.259866 ezyquant-execution-0.1.0/ezyquant_execution.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-29 09:34:13.000000 ezyquant-execution-0.1.0/ezyquant_execution.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-29 09:34:13.000000 ezyquant-execution-0.1.0/ezyquant_execution.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 09:34:13.000000 ezyquant-execution-0.1.0/ezyquant_execution.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-29 09:34:13.000000 ezyquant-execution-0.1.0/ezyquant_execution.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-29 09:34:13.000000 ezyquant-execution-0.1.0/ezyquant_execution.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-29 09:34:13.259866 ezyquant-execution-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-29 09:33:48.000000 ezyquant-execution-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:06:56.143711 ezyquant-execution-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-30 09:06:39.000000 ezyquant-execution-0.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-30 09:06:56.143711 ezyquant-execution-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-30 09:06:39.000000 ezyquant-execution-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:06:56.143711 ezyquant-execution-0.1.1/ezyquant_execution/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-30 09:06:39.000000 ezyquant-execution-0.1.1/ezyquant_execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 09:06:39.000000 ezyquant-execution-0.1.1/ezyquant_execution/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-30 09:06:39.000000 ezyquant-execution-0.1.1/ezyquant_execution/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20382 2023-05-30 09:06:39.000000 ezyquant-execution-0.1.1/ezyquant_execution/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-05-30 09:06:39.000000 ezyquant-execution-0.1.1/ezyquant_execution/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-30 09:06:39.000000 ezyquant-execution-0.1.1/ezyquant_execution/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-30 09:06:39.000000 ezyquant-execution-0.1.1/ezyquant_execution/executing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-30 09:06:39.000000 ezyquant-execution-0.1.1/ezyquant_execution/realtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-05-30 09:06:39.000000 ezyquant-execution-0.1.1/ezyquant_execution/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:06:56.143711 ezyquant-execution-0.1.1/ezyquant_execution.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-30 09:06:56.000000 ezyquant-execution-0.1.1/ezyquant_execution.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-30 09:06:56.000000 ezyquant-execution-0.1.1/ezyquant_execution.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 09:06:56.000000 ezyquant-execution-0.1.1/ezyquant_execution.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-30 09:06:56.000000 ezyquant-execution-0.1.1/ezyquant_execution.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-30 09:06:56.000000 ezyquant-execution-0.1.1/ezyquant_execution.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-30 09:06:56.143711 ezyquant-execution-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-30 09:06:39.000000 ezyquant-execution-0.1.1/setup.py
```

### Comparing `ezyquant-execution-0.1.0/LICENSE.txt` & `ezyquant-execution-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ezyquant-execution-0.1.0/PKG-INFO` & `ezyquant-execution-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezyquant-execution
-Version: 0.1.0
+Version: 0.1.1
 Summary: Ezyquant execution
 Home-page: https://pydoc.ezyquant.com/
 Author: Fintech (Thailand) Company Limited
 Author-email: admin@fintech.co.th
 Maintainer: Fintech (Thailand) Company Limited
 Maintainer-email: admin@fintech.co.th
 License: The MIT License (MIT)
```

### Comparing `ezyquant-execution-0.1.0/ezyquant_execution/constant.py` & `ezyquant-execution-0.1.1/ezyquant_execution/constant.py`

 * *Files identical despite different names*

### Comparing `ezyquant-execution-0.1.0/ezyquant_execution/context.py` & `ezyquant-execution-0.1.1/ezyquant_execution/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,14 +307,16 @@
 
         Round volume to 100. If volume is 0, return None.
         """
         volume = utils.round_100(volume, is_round_up_volume)
         if volume == 0:
             return
 
+        logger.info(f"Place order: {side} {symbol} {volume} {price}")
+
         res = self._settrade_equity.place_order(
             symbol=symbol,
             side=side,
             volume=volume,
             price=price,
             qty_open=qty_open,
             trustee_id_type=trustee_id_type,
```

### Comparing `ezyquant-execution-0.1.0/ezyquant_execution/entity.py` & `ezyquant-execution-0.1.1/ezyquant_execution/entity.py`

 * *Files identical despite different names*

### Comparing `ezyquant-execution-0.1.0/ezyquant_execution/environment.py` & `ezyquant-execution-0.1.1/ezyquant_execution/environment.py`

 * *Files identical despite different names*

### Comparing `ezyquant-execution-0.1.0/ezyquant_execution/executing.py` & `ezyquant-execution-0.1.1/ezyquant_execution/executing.py`

 * *Files identical despite different names*

### Comparing `ezyquant-execution-0.1.0/ezyquant_execution/realtime.py` & `ezyquant-execution-0.1.1/ezyquant_execution/realtime.py`

 * *Files identical despite different names*

### Comparing `ezyquant-execution-0.1.0/ezyquant_execution/utils.py` & `ezyquant-execution-0.1.1/ezyquant_execution/utils.py`

 * *Files identical despite different names*

### Comparing `ezyquant-execution-0.1.0/ezyquant_execution.egg-info/PKG-INFO` & `ezyquant-execution-0.1.1/ezyquant_execution.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezyquant-execution
-Version: 0.1.0
+Version: 0.1.1
 Summary: Ezyquant execution
 Home-page: https://pydoc.ezyquant.com/
 Author: Fintech (Thailand) Company Limited
 Author-email: admin@fintech.co.th
 Maintainer: Fintech (Thailand) Company Limited
 Maintainer-email: admin@fintech.co.th
 License: The MIT License (MIT)
```

### Comparing `ezyquant-execution-0.1.0/ezyquant_execution.egg-info/SOURCES.txt` & `ezyquant-execution-0.1.1/ezyquant_execution.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ezyquant-execution-0.1.0/setup.py` & `ezyquant-execution-0.1.1/setup.py`

 * *Files identical despite different names*

