# Comparing `tmp/troncos-4.0.0b7.tar.gz` & `tmp/troncos-4.0.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "troncos-4.0.0b7.tar", max compression
+gzip compressed data, was "troncos-4.0.0b8.tar", max compression
```

## Comparing `troncos-4.0.0b7.tar` & `troncos-4.0.0b8.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1077 2023-05-30 07:24:45.189938 troncos-4.0.0b7/LICENSE
--rw-r--r--   0        0        0     7753 2023-05-30 07:24:45.189938 troncos-4.0.0b7/README.md
--rw-r--r--   0        0        0     2389 2023-05-30 07:24:45.189938 troncos-4.0.0b7/pyproject.toml
--rw-r--r--   0        0        0      291 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/asgi/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/asgi/logging/__init__.py
--rw-r--r--   0        0        0     5058 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/asgi/logging/middleware.py
--rw-r--r--   0        0        0        0 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/asgi/profiling/__init__.py
--rw-r--r--   0        0        0      576 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/asgi/profiling/app.py
--rw-r--r--   0        0        0        0 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/celery/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/celery/logging/__init__.py
--rw-r--r--   0        0        0      949 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/celery/logging/signals.py
--rw-r--r--   0        0        0        0 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/django/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/django/logging/__init__.py
--rw-r--r--   0        0        0     2334 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/django/logging/middleware.py
--rw-r--r--   0        0        0        0 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/django/profiling/__init__.py
--rw-r--r--   0        0        0      265 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/django/profiling/views.py
--rw-r--r--   0        0        0        0 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/starlette/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/starlette/profiling/__init__.py
--rw-r--r--   0        0        0      291 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/starlette/profiling/views.py
--rw-r--r--   0        0        0     4053 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/structlog/__init__.py
--rw-r--r--   0        0        0      705 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/structlog/processors.py
--rw-r--r--   0        0        0        0 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/profiling/__init__.py
--rw-r--r--   0        0        0      192 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/profiling/auto.py
--rw-r--r--   0        0        0        0 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/profiling/bootstrap/__init__.py
--rw-r--r--   0        0        0      439 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/profiling/bootstrap/profile.py
--rw-r--r--   0        0        0      343 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/profiling/bootstrap/start.py
--rw-r--r--   0        0        0     1814 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/profiling/profiler.py
--rw-r--r--   0        0        0        0 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/py.typed
--rw-r--r--   0        0        0      690 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/tracing/__init__.py
--rw-r--r--   0        0        0       82 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/tracing/_enums.py
--rw-r--r--   0        0        0     2053 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/tracing/_otel.py
--rw-r--r--   0        0        0     4542 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/tracing/_span.py
--rw-r--r--   0        0        0     1884 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/tracing/_writer.py
--rw-r--r--   0        0        0     8744 1970-01-01 00:00:00.000000 troncos-4.0.0b7/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-30 09:10:51.497222 troncos-4.0.0b8/LICENSE
+-rw-r--r--   0        0        0     7753 2023-05-30 09:10:51.497222 troncos-4.0.0b8/README.md
+-rw-r--r--   0        0        0     2389 2023-05-30 09:10:51.501222 troncos-4.0.0b8/pyproject.toml
+-rw-r--r--   0        0        0      291 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/asgi/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/asgi/logging/__init__.py
+-rw-r--r--   0        0        0     5058 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/asgi/logging/middleware.py
+-rw-r--r--   0        0        0        0 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/asgi/profiling/__init__.py
+-rw-r--r--   0        0        0      576 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/asgi/profiling/app.py
+-rw-r--r--   0        0        0        0 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/celery/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/celery/logging/__init__.py
+-rw-r--r--   0        0        0      949 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/celery/logging/signals.py
+-rw-r--r--   0        0        0        0 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/django/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/django/logging/__init__.py
+-rw-r--r--   0        0        0     2334 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/django/logging/middleware.py
+-rw-r--r--   0        0        0        0 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/django/profiling/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/django/profiling/views.py
+-rw-r--r--   0        0        0        0 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/starlette/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/starlette/profiling/__init__.py
+-rw-r--r--   0        0        0      291 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/starlette/profiling/views.py
+-rw-r--r--   0        0        0     4053 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/structlog/__init__.py
+-rw-r--r--   0        0        0      705 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/contrib/structlog/processors.py
+-rw-r--r--   0        0        0        0 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/profiling/__init__.py
+-rw-r--r--   0        0        0      192 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/profiling/auto.py
+-rw-r--r--   0        0        0        0 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/profiling/bootstrap/__init__.py
+-rw-r--r--   0        0        0      439 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/profiling/bootstrap/profile.py
+-rw-r--r--   0        0        0      343 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/profiling/bootstrap/start.py
+-rw-r--r--   0        0        0     1814 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/profiling/profiler.py
+-rw-r--r--   0        0        0        0 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/py.typed
+-rw-r--r--   0        0        0      690 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/tracing/__init__.py
+-rw-r--r--   0        0        0       82 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/tracing/_enums.py
+-rw-r--r--   0        0        0     2053 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/tracing/_otel.py
+-rw-r--r--   0        0        0     4545 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/tracing/_span.py
+-rw-r--r--   0        0        0     1884 2023-05-30 09:10:51.501222 troncos-4.0.0b8/troncos/tracing/_writer.py
+-rw-r--r--   0        0        0     8744 1970-01-01 00:00:00.000000 troncos-4.0.0b8/PKG-INFO
```

### Comparing `troncos-4.0.0b7/LICENSE` & `troncos-4.0.0b8/LICENSE`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b7/README.md` & `troncos-4.0.0b8/README.md`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b7/pyproject.toml` & `troncos-4.0.0b8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "troncos"
-version = "4.0.0b7"
+version = "4.0.0b8"
 description = "Collection of Python logging, tracing and profiling tools"
 authors = [
     "Guðmundur Björn Birkisson <gudmundur.birkisson@oda.com>",
     "Karl Fredrik Haugland <karlfredrik.haugland@oda.com>",
     "Eirik Martiniussen Sylliaas <eirik.sylliaas@oda.com>",
 ]
 license = "MIT"
```

### Comparing `troncos-4.0.0b7/troncos/contrib/asgi/logging/middleware.py` & `troncos-4.0.0b8/troncos/contrib/asgi/logging/middleware.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b7/troncos/contrib/asgi/profiling/app.py` & `troncos-4.0.0b8/troncos/contrib/asgi/profiling/app.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b7/troncos/contrib/celery/logging/signals.py` & `troncos-4.0.0b8/troncos/contrib/celery/logging/signals.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b7/troncos/contrib/django/logging/middleware.py` & `troncos-4.0.0b8/troncos/contrib/django/logging/middleware.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b7/troncos/contrib/structlog/__init__.py` & `troncos-4.0.0b8/troncos/contrib/structlog/__init__.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b7/troncos/contrib/structlog/processors.py` & `troncos-4.0.0b8/troncos/contrib/structlog/processors.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b7/troncos/profiling/profiler.py` & `troncos-4.0.0b8/troncos/profiling/profiler.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b7/troncos/tracing/__init__.py` & `troncos-4.0.0b8/troncos/tracing/__init__.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b7/troncos/tracing/_otel.py` & `troncos-4.0.0b8/troncos/tracing/_otel.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b7/troncos/tracing/_span.py` & `troncos-4.0.0b8/troncos/tracing/_span.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any
 
 from ddtrace import constants, ext
 from ddtrace.span import Span as DDSpan
 from opentelemetry.attributes import BoundedAttributes  # type: ignore
-from opentelemetry.sdk.resources import Resource
+from opentelemetry.sdk.resources import SERVICE_NAME, Resource
 from opentelemetry.sdk.trace import (
     _DEFAULT_OTEL_EVENT_ATTRIBUTE_COUNT_LIMIT,
     _DEFAULT_OTEL_SPAN_ATTRIBUTE_COUNT_LIMIT,
     _DEFAULT_OTEL_SPAN_EVENT_COUNT_LIMIT,
     Event,
     ReadableSpan,
 )
@@ -108,24 +108,24 @@
     else:
         status = Status(StatusCode.UNSET)
 
     return (status, events, otel_attrs)
 
 
 def _span_resource(dd_span: DDSpan, default_resource: Resource) -> Resource:
-    if default_resource.attributes["service.name"] == dd_span.service:
+    if default_resource.attributes[SERVICE_NAME] == dd_span.service:
         return default_resource
 
     if not dd_span.service:
         return default_resource
 
     base_attributes = dict(default_resource.attributes)
-    base_attributes["service.name"] = dd_span.service
+    base_attributes[SERVICE_NAME] = dd_span.service
 
-    return Resource.create(base_attributes)
+    return Resource(base_attributes)
 
 
 def translate_span(dd_span: DDSpan, default_resource: Resource) -> ReadableSpan:
     """Transelate a ddtrace span to an OTEL span."""
     assert dd_span.duration_ns, "Span not finished."
 
     status, events, attributes = _span_status_and_attributes(
```

### Comparing `troncos-4.0.0b7/troncos/tracing/_writer.py` & `troncos-4.0.0b8/troncos/tracing/_writer.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b7/PKG-INFO` & `troncos-4.0.0b8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: troncos
-Version: 4.0.0b7
+Version: 4.0.0b8
 Summary: Collection of Python logging, tracing and profiling tools
 Home-page: https://github.com/kolonialno/troncos
 License: MIT
 Keywords: logs,traces,opentelemetry
 Author: Guðmundur Björn Birkisson
 Author-email: gudmundur.birkisson@oda.com
 Requires-Python: >=3.10,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: troncos Version: 4.0.0b7 Summary: Collection of
+Metadata-Version: 2.1 Name: troncos Version: 4.0.0b8 Summary: Collection of
 Python logging, tracing and profiling tools Home-page: https://github.com/
 kolonialno/troncos License: MIT Keywords: logs,traces,opentelemetry Author:
 GuÃ°mundur BjÃ¶rn Birkisson Author-email: gudmundur.birkisson@oda.com Requires-
 Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: grpc Requires-Dist: ddtrace (==1.13.3) Requires-Dist:
```

