# Comparing `tmp/django_cloudwatch_metrics-0.0.4.tar.gz` & `tmp/django_cloudwatch_metrics-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_cloudwatch_metrics-0.0.4.tar", max compression
+gzip compressed data, was "django_cloudwatch_metrics-0.0.5.tar", max compression
```

## Comparing `django_cloudwatch_metrics-0.0.4.tar` & `django_cloudwatch_metrics-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       27 2023-05-30 08:08:47.682022 django_cloudwatch_metrics-0.0.4/README.md
--rw-r--r--   0        0        0      197 2023-05-30 08:08:47.682022 django_cloudwatch_metrics-0.0.4/django_cloudwatch_metrics/apps.py
--rw-r--r--   0        0        0        0 2023-05-30 08:08:47.682022 django_cloudwatch_metrics-0.0.4/django_cloudwatch_metrics/management/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 08:08:47.682022 django_cloudwatch_metrics-0.0.4/django_cloudwatch_metrics/management/commands/__init__.py
--rw-r--r--   0        0        0      722 2023-05-30 08:08:47.682022 django_cloudwatch_metrics-0.0.4/django_cloudwatch_metrics/management/commands/increment.py
--rw-r--r--   0        0        0     1975 2023-05-30 08:08:47.682022 django_cloudwatch_metrics-0.0.4/django_cloudwatch_metrics/management/commands/publish_metrics.py
--rw-r--r--   0        0        0     1244 2023-05-30 08:08:47.682022 django_cloudwatch_metrics-0.0.4/django_cloudwatch_metrics/metrics.py
--rw-r--r--   0        0        0      926 2023-05-30 08:08:47.682022 django_cloudwatch_metrics-0.0.4/django_cloudwatch_metrics/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-05-30 08:08:47.682022 django_cloudwatch_metrics-0.0.4/django_cloudwatch_metrics/migrations/__init__.py
--rw-r--r--   0        0        0      502 2023-05-30 08:08:47.682022 django_cloudwatch_metrics-0.0.4/django_cloudwatch_metrics/models.py
--rw-r--r--   0        0        0    12871 2023-05-30 08:08:47.682022 django_cloudwatch_metrics-0.0.4/django_cloudwatch_metrics/signals.py
--rw-r--r--   0        0        0      543 2023-05-30 08:08:47.682022 django_cloudwatch_metrics-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      697 1970-01-01 00:00:00.000000 django_cloudwatch_metrics-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       27 2023-05-30 08:14:48.686224 django_cloudwatch_metrics-0.0.5/README.md
+-rw-r--r--   0        0        0      197 2023-05-30 08:14:48.686224 django_cloudwatch_metrics-0.0.5/django_cloudwatch_metrics/apps.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:14:48.686224 django_cloudwatch_metrics-0.0.5/django_cloudwatch_metrics/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:14:48.686224 django_cloudwatch_metrics-0.0.5/django_cloudwatch_metrics/management/commands/__init__.py
+-rw-r--r--   0        0        0      722 2023-05-30 08:14:48.686224 django_cloudwatch_metrics-0.0.5/django_cloudwatch_metrics/management/commands/increment.py
+-rw-r--r--   0        0        0     2310 2023-05-30 08:14:48.686224 django_cloudwatch_metrics-0.0.5/django_cloudwatch_metrics/management/commands/publish_metrics.py
+-rw-r--r--   0        0        0     1244 2023-05-30 08:14:48.686224 django_cloudwatch_metrics-0.0.5/django_cloudwatch_metrics/metrics.py
+-rw-r--r--   0        0        0      926 2023-05-30 08:14:48.686224 django_cloudwatch_metrics-0.0.5/django_cloudwatch_metrics/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:14:48.686224 django_cloudwatch_metrics-0.0.5/django_cloudwatch_metrics/migrations/__init__.py
+-rw-r--r--   0        0        0      502 2023-05-30 08:14:48.686224 django_cloudwatch_metrics-0.0.5/django_cloudwatch_metrics/models.py
+-rw-r--r--   0        0        0    12871 2023-05-30 08:14:48.686224 django_cloudwatch_metrics-0.0.5/django_cloudwatch_metrics/signals.py
+-rw-r--r--   0        0        0      543 2023-05-30 08:14:48.686224 django_cloudwatch_metrics-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      697 1970-01-01 00:00:00.000000 django_cloudwatch_metrics-0.0.5/PKG-INFO
```

### Comparing `django_cloudwatch_metrics-0.0.4/django_cloudwatch_metrics/management/commands/increment.py` & `django_cloudwatch_metrics-0.0.5/django_cloudwatch_metrics/management/commands/increment.py`

 * *Files identical despite different names*

### Comparing `django_cloudwatch_metrics-0.0.4/django_cloudwatch_metrics/management/commands/publish_metrics.py` & `django_cloudwatch_metrics-0.0.5/django_cloudwatch_metrics/management/commands/publish_metrics.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import time
 from datetime import datetime, timedelta
 
 import boto3
 import pytz
 from django.conf import settings
 from django.core.management import BaseCommand
 
@@ -53,9 +54,22 @@
     metric_aggregations.delete()
     logger.info("Published metrics to CloudWatch")
 
 
 class Command(BaseCommand):
     help = 'Publishes metrics to CloudWatch'
 
+    def add_arguments(self, parser):
+        parser.add_argument(
+            '--continuously',
+            action='store_true',
+            help='Continuously publish metrics to CloudWatch',
+        )
+
     def handle(self, *args, **options):
-        publish_metrics()
+        while True:
+            publish_metrics()
+
+            if not options['continuously']:
+                break
+
+            time.sleep(60)
```

### Comparing `django_cloudwatch_metrics-0.0.4/django_cloudwatch_metrics/metrics.py` & `django_cloudwatch_metrics-0.0.5/django_cloudwatch_metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `django_cloudwatch_metrics-0.0.4/django_cloudwatch_metrics/migrations/0001_initial.py` & `django_cloudwatch_metrics-0.0.5/django_cloudwatch_metrics/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_cloudwatch_metrics-0.0.4/django_cloudwatch_metrics/signals.py` & `django_cloudwatch_metrics-0.0.5/django_cloudwatch_metrics/signals.py`

 * *Files identical despite different names*

### Comparing `django_cloudwatch_metrics-0.0.4/pyproject.toml` & `django_cloudwatch_metrics-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-cloudwatch-metrics"
-version = "0.0.4"
+version = "0.0.5"
 description = "Metric tracking in Django using caching and CloudWatch"
 authors = ["Bart Machielsen <bartmachielsen@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 packages = [
     { include = "django_cloudwatch_metrics" }
```

### Comparing `django_cloudwatch_metrics-0.0.4/PKG-INFO` & `django_cloudwatch_metrics-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cloudwatch-metrics
-Version: 0.0.4
+Version: 0.0.5
 Summary: Metric tracking in Django using caching and CloudWatch
 License: MIT
 Author: Bart Machielsen
 Author-email: bartmachielsen@gmail.com
 Requires-Python: >=3.6.2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

