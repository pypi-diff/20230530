# Comparing `tmp/django_cloudwatch_metrics-0.0.3.tar.gz` & `tmp/django_cloudwatch_metrics-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_cloudwatch_metrics-0.0.3.tar", max compression
+gzip compressed data, was "django_cloudwatch_metrics-0.0.4.tar", max compression
```

## Comparing `django_cloudwatch_metrics-0.0.3.tar` & `django_cloudwatch_metrics-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       27 2023-05-30 07:43:23.635488 django_cloudwatch_metrics-0.0.3/README.md
--rw-r--r--   0        0        0      197 2023-05-30 07:43:23.635488 django_cloudwatch_metrics-0.0.3/django_cloudwatch_metrics/apps.py
--rw-r--r--   0        0        0        0 2023-05-30 07:43:23.635488 django_cloudwatch_metrics-0.0.3/django_cloudwatch_metrics/management/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 07:43:23.635488 django_cloudwatch_metrics-0.0.3/django_cloudwatch_metrics/management/commands/__init__.py
--rw-r--r--   0        0        0      722 2023-05-30 07:43:23.635488 django_cloudwatch_metrics-0.0.3/django_cloudwatch_metrics/management/commands/increment.py
--rw-r--r--   0        0        0     1859 2023-05-30 07:43:23.635488 django_cloudwatch_metrics-0.0.3/django_cloudwatch_metrics/management/commands/publish_metrics.py
--rw-r--r--   0        0        0     1244 2023-05-30 07:43:23.635488 django_cloudwatch_metrics-0.0.3/django_cloudwatch_metrics/metrics.py
--rw-r--r--   0        0        0      926 2023-05-30 07:43:23.635488 django_cloudwatch_metrics-0.0.3/django_cloudwatch_metrics/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-05-30 07:43:23.639488 django_cloudwatch_metrics-0.0.3/django_cloudwatch_metrics/migrations/__init__.py
--rw-r--r--   0        0        0      502 2023-05-30 07:43:23.639488 django_cloudwatch_metrics-0.0.3/django_cloudwatch_metrics/models.py
--rw-r--r--   0        0        0    12871 2023-05-30 07:43:23.639488 django_cloudwatch_metrics-0.0.3/django_cloudwatch_metrics/signals.py
--rw-r--r--   0        0        0      543 2023-05-30 07:43:23.639488 django_cloudwatch_metrics-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      697 1970-01-01 00:00:00.000000 django_cloudwatch_metrics-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       27 2023-05-30 08:08:47.682022 django_cloudwatch_metrics-0.0.4/README.md
+-rw-r--r--   0        0        0      197 2023-05-30 08:08:47.682022 django_cloudwatch_metrics-0.0.4/django_cloudwatch_metrics/apps.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:08:47.682022 django_cloudwatch_metrics-0.0.4/django_cloudwatch_metrics/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:08:47.682022 django_cloudwatch_metrics-0.0.4/django_cloudwatch_metrics/management/commands/__init__.py
+-rw-r--r--   0        0        0      722 2023-05-30 08:08:47.682022 django_cloudwatch_metrics-0.0.4/django_cloudwatch_metrics/management/commands/increment.py
+-rw-r--r--   0        0        0     1975 2023-05-30 08:08:47.682022 django_cloudwatch_metrics-0.0.4/django_cloudwatch_metrics/management/commands/publish_metrics.py
+-rw-r--r--   0        0        0     1244 2023-05-30 08:08:47.682022 django_cloudwatch_metrics-0.0.4/django_cloudwatch_metrics/metrics.py
+-rw-r--r--   0        0        0      926 2023-05-30 08:08:47.682022 django_cloudwatch_metrics-0.0.4/django_cloudwatch_metrics/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:08:47.682022 django_cloudwatch_metrics-0.0.4/django_cloudwatch_metrics/migrations/__init__.py
+-rw-r--r--   0        0        0      502 2023-05-30 08:08:47.682022 django_cloudwatch_metrics-0.0.4/django_cloudwatch_metrics/models.py
+-rw-r--r--   0        0        0    12871 2023-05-30 08:08:47.682022 django_cloudwatch_metrics-0.0.4/django_cloudwatch_metrics/signals.py
+-rw-r--r--   0        0        0      543 2023-05-30 08:08:47.682022 django_cloudwatch_metrics-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      697 1970-01-01 00:00:00.000000 django_cloudwatch_metrics-0.0.4/PKG-INFO
```

### Comparing `django_cloudwatch_metrics-0.0.3/django_cloudwatch_metrics/management/commands/increment.py` & `django_cloudwatch_metrics-0.0.4/django_cloudwatch_metrics/management/commands/increment.py`

 * *Files identical despite different names*

### Comparing `django_cloudwatch_metrics-0.0.3/django_cloudwatch_metrics/management/commands/publish_metrics.py` & `django_cloudwatch_metrics-0.0.4/django_cloudwatch_metrics/management/commands/publish_metrics.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,18 +39,20 @@
                 ] if dimension_name and dimension_value else [],
                 "Timestamp": datetime_period,
                 "Value": value
             }
         )
 
     if metric_data:
-        cloudwatch.put_metric_data(
-            Namespace=NAMESPACE,
-            MetricData=metric_data
-        )
+        # split in batches of max 1000
+        for i in range(0, len(metric_data), 1000):
+            cloudwatch.put_metric_data(
+                Namespace=NAMESPACE,
+                MetricData=metric_data[i:i+1000]
+            )
 
     metric_aggregations.delete()
     logger.info("Published metrics to CloudWatch")
 
 
 class Command(BaseCommand):
     help = 'Publishes metrics to CloudWatch'
```

### Comparing `django_cloudwatch_metrics-0.0.3/django_cloudwatch_metrics/metrics.py` & `django_cloudwatch_metrics-0.0.4/django_cloudwatch_metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `django_cloudwatch_metrics-0.0.3/django_cloudwatch_metrics/migrations/0001_initial.py` & `django_cloudwatch_metrics-0.0.4/django_cloudwatch_metrics/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_cloudwatch_metrics-0.0.3/django_cloudwatch_metrics/signals.py` & `django_cloudwatch_metrics-0.0.4/django_cloudwatch_metrics/signals.py`

 * *Files identical despite different names*

### Comparing `django_cloudwatch_metrics-0.0.3/pyproject.toml` & `django_cloudwatch_metrics-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-cloudwatch-metrics"
-version = "0.0.3"
+version = "0.0.4"
 description = "Metric tracking in Django using caching and CloudWatch"
 authors = ["Bart Machielsen <bartmachielsen@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 packages = [
     { include = "django_cloudwatch_metrics" }
```

### Comparing `django_cloudwatch_metrics-0.0.3/PKG-INFO` & `django_cloudwatch_metrics-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cloudwatch-metrics
-Version: 0.0.3
+Version: 0.0.4
 Summary: Metric tracking in Django using caching and CloudWatch
 License: MIT
 Author: Bart Machielsen
 Author-email: bartmachielsen@gmail.com
 Requires-Python: >=3.6.2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

