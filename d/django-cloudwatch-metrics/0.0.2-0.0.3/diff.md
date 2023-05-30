# Comparing `tmp/django_cloudwatch_metrics-0.0.2.tar.gz` & `tmp/django_cloudwatch_metrics-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_cloudwatch_metrics-0.0.2.tar", max compression
+gzip compressed data, was "django_cloudwatch_metrics-0.0.3.tar", max compression
```

## Comparing `django_cloudwatch_metrics-0.0.2.tar` & `django_cloudwatch_metrics-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       27 2023-05-24 12:35:18.676833 django_cloudwatch_metrics-0.0.2/README.md
--rw-r--r--   0        0        0      197 2023-05-24 12:35:18.676833 django_cloudwatch_metrics-0.0.2/django_cloudwatch_metrics/apps.py
--rw-r--r--   0        0        0        0 2023-05-24 12:35:18.676833 django_cloudwatch_metrics-0.0.2/django_cloudwatch_metrics/management/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 12:35:18.680833 django_cloudwatch_metrics-0.0.2/django_cloudwatch_metrics/management/commands/__init__.py
--rw-r--r--   0        0        0      722 2023-05-24 12:35:18.680833 django_cloudwatch_metrics-0.0.2/django_cloudwatch_metrics/management/commands/increment.py
--rw-r--r--   0        0        0     1859 2023-05-24 12:35:18.680833 django_cloudwatch_metrics-0.0.2/django_cloudwatch_metrics/management/commands/publish_metrics.py
--rw-r--r--   0        0        0      834 2023-05-24 12:35:18.680833 django_cloudwatch_metrics-0.0.2/django_cloudwatch_metrics/metrics.py
--rw-r--r--   0        0        0      926 2023-05-24 12:35:18.680833 django_cloudwatch_metrics-0.0.2/django_cloudwatch_metrics/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-05-24 12:35:18.680833 django_cloudwatch_metrics-0.0.2/django_cloudwatch_metrics/migrations/__init__.py
--rw-r--r--   0        0        0      502 2023-05-24 12:35:18.680833 django_cloudwatch_metrics-0.0.2/django_cloudwatch_metrics/models.py
--rw-r--r--   0        0        0    12871 2023-05-24 12:35:18.680833 django_cloudwatch_metrics-0.0.2/django_cloudwatch_metrics/signals.py
--rw-r--r--   0        0        0      543 2023-05-24 12:35:18.680833 django_cloudwatch_metrics-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      697 1970-01-01 00:00:00.000000 django_cloudwatch_metrics-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       27 2023-05-30 07:43:23.635488 django_cloudwatch_metrics-0.0.3/README.md
+-rw-r--r--   0        0        0      197 2023-05-30 07:43:23.635488 django_cloudwatch_metrics-0.0.3/django_cloudwatch_metrics/apps.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:43:23.635488 django_cloudwatch_metrics-0.0.3/django_cloudwatch_metrics/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:43:23.635488 django_cloudwatch_metrics-0.0.3/django_cloudwatch_metrics/management/commands/__init__.py
+-rw-r--r--   0        0        0      722 2023-05-30 07:43:23.635488 django_cloudwatch_metrics-0.0.3/django_cloudwatch_metrics/management/commands/increment.py
+-rw-r--r--   0        0        0     1859 2023-05-30 07:43:23.635488 django_cloudwatch_metrics-0.0.3/django_cloudwatch_metrics/management/commands/publish_metrics.py
+-rw-r--r--   0        0        0     1244 2023-05-30 07:43:23.635488 django_cloudwatch_metrics-0.0.3/django_cloudwatch_metrics/metrics.py
+-rw-r--r--   0        0        0      926 2023-05-30 07:43:23.635488 django_cloudwatch_metrics-0.0.3/django_cloudwatch_metrics/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:43:23.639488 django_cloudwatch_metrics-0.0.3/django_cloudwatch_metrics/migrations/__init__.py
+-rw-r--r--   0        0        0      502 2023-05-30 07:43:23.639488 django_cloudwatch_metrics-0.0.3/django_cloudwatch_metrics/models.py
+-rw-r--r--   0        0        0    12871 2023-05-30 07:43:23.639488 django_cloudwatch_metrics-0.0.3/django_cloudwatch_metrics/signals.py
+-rw-r--r--   0        0        0      543 2023-05-30 07:43:23.639488 django_cloudwatch_metrics-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      697 1970-01-01 00:00:00.000000 django_cloudwatch_metrics-0.0.3/PKG-INFO
```

### Comparing `django_cloudwatch_metrics-0.0.2/django_cloudwatch_metrics/management/commands/increment.py` & `django_cloudwatch_metrics-0.0.3/django_cloudwatch_metrics/management/commands/increment.py`

 * *Files identical despite different names*

### Comparing `django_cloudwatch_metrics-0.0.2/django_cloudwatch_metrics/management/commands/publish_metrics.py` & `django_cloudwatch_metrics-0.0.3/django_cloudwatch_metrics/management/commands/publish_metrics.py`

 * *Files identical despite different names*

### Comparing `django_cloudwatch_metrics-0.0.2/django_cloudwatch_metrics/metrics.py` & `django_cloudwatch_metrics-0.0.3/django_cloudwatch_metrics/metrics.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,21 +6,32 @@
 
 from django_cloudwatch_metrics.models import MetricAggregation
 
 
 def increment(metric_name: str, value: int, dimension_name: Optional[str] = None, dimension_value: Optional[str] = None):
     """Publishes a metric increment."""
     datetime_period = datetime.now(pytz.utc).replace(second=0, microsecond=0)
-    metric_aggregation, created = MetricAggregation.objects.get_or_create(
-        datetime_period=datetime_period,
-        metric_name=metric_name,
-        dimension_name=dimension_name,
-        dimension_value=dimension_value,
-        defaults={
-            "value": value,
-        }
-    )
+    try:
+        metric_aggregation, created = MetricAggregation.objects.get_or_create(
+            datetime_period=datetime_period,
+            metric_name=metric_name,
+            dimension_name=dimension_name,
+            dimension_value=dimension_value,
+            defaults={
+                "value": value,
+            }
+        )
+    except MetricAggregation.MultipleObjectsReturned:
+        metric_aggregation = MetricAggregation.objects.filter(
+            datetime_period=datetime_period,
+            metric_name=metric_name,
+            dimension_name=dimension_name,
+            dimension_value=dimension_value,
+        ).first()
+        created = False
+
     if created:
         return
 
-    metric_aggregation.value = F("value") + value
-    metric_aggregation.save(update_fields=["value"])
+    if metric_aggregation:
+        metric_aggregation.value = F("value") + value
+        metric_aggregation.save(update_fields=["value"])
```

### Comparing `django_cloudwatch_metrics-0.0.2/django_cloudwatch_metrics/migrations/0001_initial.py` & `django_cloudwatch_metrics-0.0.3/django_cloudwatch_metrics/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_cloudwatch_metrics-0.0.2/django_cloudwatch_metrics/signals.py` & `django_cloudwatch_metrics-0.0.3/django_cloudwatch_metrics/signals.py`

 * *Files identical despite different names*

### Comparing `django_cloudwatch_metrics-0.0.2/pyproject.toml` & `django_cloudwatch_metrics-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-cloudwatch-metrics"
-version = "0.0.2"
+version = "0.0.3"
 description = "Metric tracking in Django using caching and CloudWatch"
 authors = ["Bart Machielsen <bartmachielsen@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 packages = [
     { include = "django_cloudwatch_metrics" }
```

### Comparing `django_cloudwatch_metrics-0.0.2/PKG-INFO` & `django_cloudwatch_metrics-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cloudwatch-metrics
-Version: 0.0.2
+Version: 0.0.3
 Summary: Metric tracking in Django using caching and CloudWatch
 License: MIT
 Author: Bart Machielsen
 Author-email: bartmachielsen@gmail.com
 Requires-Python: >=3.6.2
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

