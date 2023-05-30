# Comparing `tmp/troncos-4.0.0b6.tar.gz` & `tmp/troncos-4.0.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "troncos-4.0.0b6.tar", max compression
+gzip compressed data, was "troncos-4.0.0b7.tar", max compression
```

## Comparing `troncos-4.0.0b6.tar` & `troncos-4.0.0b7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1077 2023-05-26 09:46:04.242572 troncos-4.0.0b6/LICENSE
--rw-r--r--   0        0        0     7753 2023-05-26 09:46:04.242572 troncos-4.0.0b6/README.md
--rw-r--r--   0        0        0     2389 2023-05-26 09:46:04.242572 troncos-4.0.0b6/pyproject.toml
--rw-r--r--   0        0        0      291 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/asgi/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/asgi/logging/__init__.py
--rw-r--r--   0        0        0     5058 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/asgi/logging/middleware.py
--rw-r--r--   0        0        0        0 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/asgi/profiling/__init__.py
--rw-r--r--   0        0        0      576 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/asgi/profiling/app.py
--rw-r--r--   0        0        0        0 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/celery/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/celery/logging/__init__.py
--rw-r--r--   0        0        0      949 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/celery/logging/signals.py
--rw-r--r--   0        0        0        0 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/django/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/django/logging/__init__.py
--rw-r--r--   0        0        0     2334 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/django/logging/middleware.py
--rw-r--r--   0        0        0        0 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/django/profiling/__init__.py
--rw-r--r--   0        0        0      265 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/django/profiling/views.py
--rw-r--r--   0        0        0        0 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/starlette/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/starlette/profiling/__init__.py
--rw-r--r--   0        0        0      291 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/starlette/profiling/views.py
--rw-r--r--   0        0        0     4053 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/structlog/__init__.py
--rw-r--r--   0        0        0      705 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/structlog/processors.py
--rw-r--r--   0        0        0        0 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/profiling/__init__.py
--rw-r--r--   0        0        0      192 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/profiling/auto.py
--rw-r--r--   0        0        0        0 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/profiling/bootstrap/__init__.py
--rw-r--r--   0        0        0      439 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/profiling/bootstrap/profile.py
--rw-r--r--   0        0        0      343 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/profiling/bootstrap/start.py
--rw-r--r--   0        0        0     1814 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/profiling/profiler.py
--rw-r--r--   0        0        0        0 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/py.typed
--rw-r--r--   0        0        0      690 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/tracing/__init__.py
--rw-r--r--   0        0        0       82 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/tracing/_enums.py
--rw-r--r--   0        0        0     2053 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/tracing/_otel.py
--rw-r--r--   0        0        0     4054 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/tracing/_span.py
--rw-r--r--   0        0        0     1886 2023-05-26 09:46:04.246573 troncos-4.0.0b6/troncos/tracing/_writer.py
--rw-r--r--   0        0        0     8744 1970-01-01 00:00:00.000000 troncos-4.0.0b6/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-30 07:24:45.189938 troncos-4.0.0b7/LICENSE
+-rw-r--r--   0        0        0     7753 2023-05-30 07:24:45.189938 troncos-4.0.0b7/README.md
+-rw-r--r--   0        0        0     2389 2023-05-30 07:24:45.189938 troncos-4.0.0b7/pyproject.toml
+-rw-r--r--   0        0        0      291 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/asgi/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/asgi/logging/__init__.py
+-rw-r--r--   0        0        0     5058 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/asgi/logging/middleware.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/asgi/profiling/__init__.py
+-rw-r--r--   0        0        0      576 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/asgi/profiling/app.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/celery/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/celery/logging/__init__.py
+-rw-r--r--   0        0        0      949 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/celery/logging/signals.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/django/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/django/logging/__init__.py
+-rw-r--r--   0        0        0     2334 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/django/logging/middleware.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/django/profiling/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/django/profiling/views.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/starlette/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/starlette/profiling/__init__.py
+-rw-r--r--   0        0        0      291 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/starlette/profiling/views.py
+-rw-r--r--   0        0        0     4053 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/structlog/__init__.py
+-rw-r--r--   0        0        0      705 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/contrib/structlog/processors.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/profiling/__init__.py
+-rw-r--r--   0        0        0      192 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/profiling/auto.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/profiling/bootstrap/__init__.py
+-rw-r--r--   0        0        0      439 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/profiling/bootstrap/profile.py
+-rw-r--r--   0        0        0      343 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/profiling/bootstrap/start.py
+-rw-r--r--   0        0        0     1814 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/profiling/profiler.py
+-rw-r--r--   0        0        0        0 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/py.typed
+-rw-r--r--   0        0        0      690 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/tracing/__init__.py
+-rw-r--r--   0        0        0       82 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/tracing/_enums.py
+-rw-r--r--   0        0        0     2053 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/tracing/_otel.py
+-rw-r--r--   0        0        0     4542 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/tracing/_span.py
+-rw-r--r--   0        0        0     1884 2023-05-30 07:24:45.189938 troncos-4.0.0b7/troncos/tracing/_writer.py
+-rw-r--r--   0        0        0     8744 1970-01-01 00:00:00.000000 troncos-4.0.0b7/PKG-INFO
```

### Comparing `troncos-4.0.0b6/LICENSE` & `troncos-4.0.0b7/LICENSE`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b6/README.md` & `troncos-4.0.0b7/README.md`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b6/pyproject.toml` & `troncos-4.0.0b7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "troncos"
-version = "4.0.0b6"
+version = "4.0.0b7"
 description = "Collection of Python logging, tracing and profiling tools"
 authors = [
     "Guðmundur Björn Birkisson <gudmundur.birkisson@oda.com>",
     "Karl Fredrik Haugland <karlfredrik.haugland@oda.com>",
     "Eirik Martiniussen Sylliaas <eirik.sylliaas@oda.com>",
 ]
 license = "MIT"
```

### Comparing `troncos-4.0.0b6/troncos/contrib/asgi/logging/middleware.py` & `troncos-4.0.0b7/troncos/contrib/asgi/logging/middleware.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b6/troncos/contrib/asgi/profiling/app.py` & `troncos-4.0.0b7/troncos/contrib/asgi/profiling/app.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b6/troncos/contrib/celery/logging/signals.py` & `troncos-4.0.0b7/troncos/contrib/celery/logging/signals.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b6/troncos/contrib/django/logging/middleware.py` & `troncos-4.0.0b7/troncos/contrib/django/logging/middleware.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b6/troncos/contrib/structlog/__init__.py` & `troncos-4.0.0b7/troncos/contrib/structlog/__init__.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b6/troncos/contrib/structlog/processors.py` & `troncos-4.0.0b7/troncos/contrib/structlog/processors.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b6/troncos/profiling/profiler.py` & `troncos-4.0.0b7/troncos/profiling/profiler.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b6/troncos/tracing/__init__.py` & `troncos-4.0.0b7/troncos/tracing/__init__.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b6/troncos/tracing/_otel.py` & `troncos-4.0.0b7/troncos/tracing/_otel.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b6/troncos/tracing/_span.py` & `troncos-4.0.0b7/troncos/tracing/_span.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 from typing import Any
 
 from ddtrace import constants, ext
 from ddtrace.span import Span as DDSpan
+from opentelemetry.attributes import BoundedAttributes  # type: ignore
 from opentelemetry.sdk.resources import Resource
-from opentelemetry.sdk.trace import Event, ReadableSpan, Span
+from opentelemetry.sdk.trace import (
+    _DEFAULT_OTEL_EVENT_ATTRIBUTE_COUNT_LIMIT,
+    _DEFAULT_OTEL_SPAN_ATTRIBUTE_COUNT_LIMIT,
+    _DEFAULT_OTEL_SPAN_EVENT_COUNT_LIMIT,
+    Event,
+    ReadableSpan,
+)
+from opentelemetry.sdk.util import BoundedList
 from opentelemetry.trace import SpanContext, SpanKind, Status, StatusCode
 from opentelemetry.trace.span import TraceFlags
 
 _dd_span_ignore_attr = [
     "runtime-id",
     "_sampling_priority_v1",
     "env",
     "version",
     "span.kind",
 ]
 
 
-class _Span(Span):
-    """Class needed to allow us to make a Span outside of a tracer."""
-
-    pass
-
-
 def _span_context(span: DDSpan) -> SpanContext:
     return SpanContext(
         trace_id=span.trace_id,
         span_id=span.span_id,
         is_remote=False,
         trace_flags=TraceFlags(1),
     )
@@ -82,15 +84,23 @@
             continue
         elif otel_err_attr:
             otel_error_attrs[otel_err_attr] = v
         elif k not in ignore_attrs:
             otel_attrs[k] = v
 
     if otel_error_attrs:
-        events.append(Event("exception", attributes=otel_error_attrs))
+        events.append(
+            Event(
+                "exception",
+                BoundedAttributes(
+                    _DEFAULT_OTEL_EVENT_ATTRIBUTE_COUNT_LIMIT,
+                    attributes=otel_error_attrs,
+                ),
+            )
+        )
 
         status_exp_type = otel_error_attrs.get("exception.type", None)
         status_exp_msg = otel_error_attrs.get("exception.message", None)
 
         status = Status(
             status_code=StatusCode.ERROR,
             description=f"{status_exp_type}: {status_exp_msg}",
@@ -110,31 +120,32 @@
 
     base_attributes = dict(default_resource.attributes)
     base_attributes["service.name"] = dd_span.service
 
     return Resource.create(base_attributes)
 
 
-def transalate_span(dd_span: DDSpan, default_resource: Resource) -> ReadableSpan:
+def translate_span(dd_span: DDSpan, default_resource: Resource) -> ReadableSpan:
     """Transelate a ddtrace span to an OTEL span."""
     assert dd_span.duration_ns, "Span not finished."
 
     status, events, attributes = _span_status_and_attributes(
         dd_span,
         ignore_attrs=_dd_span_ignore_attr + list(default_resource.attributes.keys()),
     )
 
-    otel_span = _Span(
+    otel_span = ReadableSpan(
         name=dd_span.name,
         context=_span_context(dd_span),
         parent=_parent_span_context(dd_span),
         resource=_span_resource(dd_span, default_resource),
-        attributes=attributes,
-        events=events,
+        attributes=BoundedAttributes(
+            _DEFAULT_OTEL_SPAN_ATTRIBUTE_COUNT_LIMIT, attributes=attributes
+        ),
+        events=BoundedList.from_seq(_DEFAULT_OTEL_SPAN_EVENT_COUNT_LIMIT, events),
         kind=_span_kind(dd_span),
+        status=status,
+        start_time=dd_span.start_ns,
+        end_time=dd_span.start_ns + dd_span.duration_ns,
     )
 
-    otel_span.set_status(status=status)
-    otel_span.start(dd_span.start_ns)
-    otel_span.end(dd_span.start_ns + dd_span.duration_ns)
-
     return otel_span
```

### Comparing `troncos-4.0.0b6/troncos/tracing/_writer.py` & `troncos-4.0.0b7/troncos/tracing/_writer.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from ddtrace.internal.writer.writer import TraceWriter
 from ddtrace.span import Span
 from opentelemetry.sdk.resources import Resource
 
 from ._enums import Exporter
 from ._otel import get_otel_span_processors
-from ._span import transalate_span
+from ._span import translate_span
 
 
 class OTELWriter(TraceWriter):
     def __init__(
         self,
         service_name: str,
         service_attributes: dict[str, Any] | None,
@@ -34,21 +34,21 @@
             self.service_name,
             self.service_attributes,
             self.endpoint,
             exporter=self.exporter,
         )
 
     def write(self, spans: list[Span] | None = None) -> None:
-        transalated_spans = [
-            transalate_span(span, default_resource=self.otel_default_resource)
+        transelated_spans = [
+            translate_span(span, default_resource=self.otel_default_resource)
             for span in spans or []
         ]
 
         for span_processor in self.otel_span_processors:
-            for span in transalated_spans:
+            for span in transelated_spans:
                 span_processor.on_end(span)
 
     def stop(self, timeout: float | None = None) -> None:
         for span_processor in self.otel_span_processors:
             span_processor.force_flush(
                 timeout_millis=int(timeout * 1000) if timeout else 30000
             )
```

### Comparing `troncos-4.0.0b6/PKG-INFO` & `troncos-4.0.0b7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: troncos
-Version: 4.0.0b6
+Version: 4.0.0b7
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
-Metadata-Version: 2.1 Name: troncos Version: 4.0.0b6 Summary: Collection of
+Metadata-Version: 2.1 Name: troncos Version: 4.0.0b7 Summary: Collection of
 Python logging, tracing and profiling tools Home-page: https://github.com/
 kolonialno/troncos License: MIT Keywords: logs,traces,opentelemetry Author:
 GuÃ°mundur BjÃ¶rn Birkisson Author-email: gudmundur.birkisson@oda.com Requires-
 Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: grpc Requires-Dist: ddtrace (==1.13.3) Requires-Dist:
```

