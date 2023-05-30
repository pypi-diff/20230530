# Comparing `tmp/redis-metric-helper-0.2.4.tar.gz` & `tmp/redis-metric-helper-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis-metric-helper-0.2.4.tar", last modified: Mon Apr 17 10:31:03 2023, max compression
+gzip compressed data, was "redis-metric-helper-0.2.5.tar", last modified: Tue May 30 13:40:18 2023, max compression
```

## Comparing `redis-metric-helper-0.2.4.tar` & `redis-metric-helper-0.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-17 10:31:03.485906 redis-metric-helper-0.2.4/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1072 2023-04-11 07:19:47.000000 redis-metric-helper-0.2.4/LICENSE
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1005 2023-04-17 10:31:03.485906 redis-metric-helper-0.2.4/PKG-INFO
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      430 2023-04-12 08:06:26.000000 redis-metric-helper-0.2.4/README.md
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-17 10:31:03.485906 redis-metric-helper-0.2.4/metric_helper/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       22 2023-04-17 10:30:25.000000 redis-metric-helper-0.2.4/metric_helper/__init__.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     7055 2023-04-17 10:30:18.000000 redis-metric-helper-0.2.4/metric_helper/base.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      464 2023-04-14 11:03:12.000000 redis-metric-helper-0.2.4/metric_helper/conf.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1170 2023-04-14 14:07:38.000000 redis-metric-helper-0.2.4/metric_helper/connections.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      220 2023-04-06 09:20:32.000000 redis-metric-helper-0.2.4/metric_helper/exceptions.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2463 2023-04-12 14:09:16.000000 redis-metric-helper-0.2.4/metric_helper/registry.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-17 10:31:03.485906 redis-metric-helper-0.2.4/redis_metric_helper.egg-info/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1005 2023-04-17 10:31:03.000000 redis-metric-helper-0.2.4/redis_metric_helper.egg-info/PKG-INFO
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      393 2023-04-17 10:31:03.000000 redis-metric-helper-0.2.4/redis_metric_helper.egg-info/SOURCES.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-04-17 10:31:03.000000 redis-metric-helper-0.2.4/redis_metric_helper.egg-info/dependency_links.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       22 2023-04-17 10:31:03.000000 redis-metric-helper-0.2.4/redis_metric_helper.egg-info/requires.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       14 2023-04-17 10:31:03.000000 redis-metric-helper-0.2.4/redis_metric_helper.egg-info/top_level.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-04-17 10:31:03.485906 redis-metric-helper-0.2.4/setup.cfg
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1657 2023-04-12 08:10:16.000000 redis-metric-helper-0.2.4/setup.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-05-30 13:40:18.682794 redis-metric-helper-0.2.5/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1072 2023-04-11 07:19:47.000000 redis-metric-helper-0.2.5/LICENSE
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1005 2023-05-30 13:40:18.682794 redis-metric-helper-0.2.5/PKG-INFO
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      430 2023-04-12 08:06:26.000000 redis-metric-helper-0.2.5/README.md
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-05-30 13:40:18.678794 redis-metric-helper-0.2.5/metric_helper/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       22 2023-05-30 13:38:17.000000 redis-metric-helper-0.2.5/metric_helper/__init__.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     7028 2023-05-30 13:39:30.000000 redis-metric-helper-0.2.5/metric_helper/base.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      464 2023-04-14 11:03:12.000000 redis-metric-helper-0.2.5/metric_helper/conf.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1202 2023-05-30 13:37:38.000000 redis-metric-helper-0.2.5/metric_helper/connections.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      220 2023-04-06 09:20:32.000000 redis-metric-helper-0.2.5/metric_helper/exceptions.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2463 2023-05-30 12:53:52.000000 redis-metric-helper-0.2.5/metric_helper/registry.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-05-30 13:40:18.682794 redis-metric-helper-0.2.5/redis_metric_helper.egg-info/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1005 2023-05-30 13:40:18.000000 redis-metric-helper-0.2.5/redis_metric_helper.egg-info/PKG-INFO
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      393 2023-05-30 13:40:18.000000 redis-metric-helper-0.2.5/redis_metric_helper.egg-info/SOURCES.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-05-30 13:40:18.000000 redis-metric-helper-0.2.5/redis_metric_helper.egg-info/dependency_links.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       22 2023-05-30 13:40:18.000000 redis-metric-helper-0.2.5/redis_metric_helper.egg-info/requires.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       14 2023-05-30 13:40:18.000000 redis-metric-helper-0.2.5/redis_metric_helper.egg-info/top_level.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-05-30 13:40:18.682794 redis-metric-helper-0.2.5/setup.cfg
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1657 2023-04-12 08:10:16.000000 redis-metric-helper-0.2.5/setup.py
```

### Comparing `redis-metric-helper-0.2.4/LICENSE` & `redis-metric-helper-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `redis-metric-helper-0.2.4/PKG-INFO` & `redis-metric-helper-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-metric-helper
-Version: 0.2.4
+Version: 0.2.5
 Summary: A helper to make writing/reading metrics to Redis more convenient.
 Author: Armandt van Zyl
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `redis-metric-helper-0.2.4/metric_helper/base.py` & `redis-metric-helper-0.2.5/metric_helper/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,29 @@
 from metric_helper.conf import settings
 from metric_helper.connections import (
     get_redis_connection,
     get_redis_version,
 )
 from metric_helper.exceptions import MetricNotFound
 
+redis_version = get_redis_version()
+
 
 
 
 class Metric:
 
     unsupported_operation = 'This metric does not support this operation.'
 
 
     def __init__(self, name):
         self.key = name
         self.name = name
         self.redis = get_redis_connection()
         self.ts = self.redis.ts()
-        self.redis_version = get_redis_version(self.redis)
         self.retention_msecs = int(settings.TIMESERIES_RETENTION_MSECS)
         self.retention_seconds = int(self.retention_msecs / 1000)
 
 
     def handle_write_kwargs(self, **kwargs):
         value = kwargs.get('value', None)
         if not value:
@@ -59,15 +60,15 @@
         }
 
 
     def expire(self):
         if not self.retention_seconds:
             return
         if (
-            self.redis_version >= 7
+            redis_version >= 7
             and self.retention_seconds
         ):
             self.redis.expire(
                 name=self.key,
                 time=self.retention_seconds,
                 nx=True, # Set expiry only when the key has no expiry.
             )
```

### Comparing `redis-metric-helper-0.2.4/metric_helper/connections.py` & `redis-metric-helper-0.2.5/metric_helper/connections.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,27 +32,30 @@
 
 
 
 
 redis = RedisWrapper()
 
 
+
+
 def get_redis_connection(decode_responses=True):
     redis.connect()
     return redis.get_connection()
 
 
 
 
-def get_redis_version(conn):
+def get_redis_version():
     """
     Returns the major version of the Redis instance for the connection.
 
     :rtype: int
     """
+    conn = get_redis_connection()
     version = conn.info()['redis_version']
     version = version[0]
     try:
         version = int(version)
     except ValueError:
         # If first character of version
         # cannot be cast to an integer;
```

### Comparing `redis-metric-helper-0.2.4/metric_helper/registry.py` & `redis-metric-helper-0.2.5/metric_helper/registry.py`

 * *Files identical despite different names*

### Comparing `redis-metric-helper-0.2.4/redis_metric_helper.egg-info/PKG-INFO` & `redis-metric-helper-0.2.5/redis_metric_helper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-metric-helper
-Version: 0.2.4
+Version: 0.2.5
 Summary: A helper to make writing/reading metrics to Redis more convenient.
 Author: Armandt van Zyl
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `redis-metric-helper-0.2.4/setup.py` & `redis-metric-helper-0.2.5/setup.py`

 * *Files identical despite different names*

