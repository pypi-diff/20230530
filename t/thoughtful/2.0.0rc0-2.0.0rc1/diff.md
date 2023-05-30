# Comparing `tmp/thoughtful-2.0.0rc0.tar.gz` & `tmp/thoughtful-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thoughtful-2.0.0rc0.tar", max compression
+gzip compressed data, was "thoughtful-2.0.0rc1.tar", max compression
```

## Comparing `thoughtful-2.0.0rc0.tar` & `thoughtful-2.0.0rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11358 2022-12-14 17:25:44.942523 thoughtful-2.0.0rc0/LICENSE
--rw-r--r--   0        0        0     2992 2023-03-22 17:30:28.308693 thoughtful-2.0.0rc0/README.md
--rw-r--r--   0        0        0     1947 2023-05-24 19:52:08.900768 thoughtful-2.0.0rc0/pyproject.toml
--rw-r--r--   0        0        0      222 2023-03-07 23:35:15.321689 thoughtful-2.0.0rc0/thoughtful/__init__.py
--rw-r--r--   0        0        0       57 2023-05-24 19:52:15.741990 thoughtful-2.0.0rc0/thoughtful/__version__.py
--rw-r--r--   0        0        0     1070 2023-05-24 14:49:11.094869 thoughtful-2.0.0rc0/thoughtful/environment_variables.py
--rw-r--r--   0        0        0      143 2022-12-14 17:25:44.949518 thoughtful-2.0.0rc0/thoughtful/supervisor/__init__.py
--rw-r--r--   0        0        0     4729 2023-05-24 14:49:11.095347 thoughtful-2.0.0rc0/thoughtful/supervisor/default_instances.py
--rw-r--r--   0        0        0     8598 2023-05-24 14:25:56.931578 thoughtful-2.0.0rc0/thoughtful/supervisor/main_context.py
--rw-r--r--   0        0        0    10567 2022-12-14 17:25:44.949966 thoughtful-2.0.0rc0/thoughtful/supervisor/manifest.py
--rw-r--r--   0        0        0        0 2022-12-14 17:25:44.949991 thoughtful-2.0.0rc0/thoughtful/supervisor/py.typed
--rw-r--r--   0        0        0        0 2022-12-14 17:25:44.950159 thoughtful-2.0.0rc0/thoughtful/supervisor/reporting/__init__.py
--rw-r--r--   0        0        0     2619 2023-05-24 14:48:54.309495 thoughtful-2.0.0rc0/thoughtful/supervisor/reporting/record.py
--rw-r--r--   0        0        0     1125 2023-05-24 14:48:54.309801 thoughtful-2.0.0rc0/thoughtful/supervisor/reporting/record_report.py
--rw-r--r--   0        0        0     2131 2023-02-23 21:00:49.643195 thoughtful-2.0.0rc0/thoughtful/supervisor/reporting/report.py
--rw-r--r--   0        0        0    10192 2023-05-24 14:48:54.310046 thoughtful-2.0.0rc0/thoughtful/supervisor/reporting/report_builder.py
--rw-r--r--   0        0        0      659 2022-12-14 17:25:44.950571 thoughtful-2.0.0rc0/thoughtful/supervisor/reporting/status.py
--rw-r--r--   0        0        0      883 2023-05-24 14:25:56.932274 thoughtful-2.0.0rc0/thoughtful/supervisor/reporting/step_report.py
--rw-r--r--   0        0        0     1541 2022-12-14 17:25:44.951007 thoughtful-2.0.0rc0/thoughtful/supervisor/reporting/timed_report.py
--rw-r--r--   0        0        0     1870 2022-12-14 17:25:44.951071 thoughtful-2.0.0rc0/thoughtful/supervisor/reporting/timer.py
--rw-r--r--   0        0        0     7643 2023-05-24 14:48:54.310467 thoughtful-2.0.0rc0/thoughtful/supervisor/step_context.py
--rw-r--r--   0        0        0     7462 2023-05-24 14:49:04.525171 thoughtful-2.0.0rc0/thoughtful/supervisor/step_decorator_factory.py
--rw-r--r--   0        0        0        0 2023-01-30 21:43:52.785761 thoughtful-2.0.0rc0/thoughtful/supervisor/streaming/__init__.py
--rw-r--r--   0        0        0      736 2023-04-06 19:41:20.157278 thoughtful-2.0.0rc0/thoughtful/supervisor/streaming/action.py
--rw-r--r--   0        0        0     3087 2023-05-24 14:49:11.095696 thoughtful-2.0.0rc0/thoughtful/supervisor/streaming/callback.py
--rw-r--r--   0        0        0     3184 2023-05-24 14:48:54.311303 thoughtful-2.0.0rc0/thoughtful/supervisor/streaming/payloads.py
--rw-r--r--   0        0        0     4233 1970-01-01 00:00:00.000000 thoughtful-2.0.0rc0/setup.py
--rw-r--r--   0        0        0     4554 1970-01-01 00:00:00.000000 thoughtful-2.0.0rc0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2022-12-14 17:25:44.942523 thoughtful-2.0.0rc1/LICENSE
+-rw-r--r--   0        0        0     2992 2023-03-22 17:30:28.308693 thoughtful-2.0.0rc1/README.md
+-rw-r--r--   0        0        0     1964 2023-05-30 13:53:35.915637 thoughtful-2.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      222 2023-03-07 23:35:15.321689 thoughtful-2.0.0rc1/thoughtful/__init__.py
+-rw-r--r--   0        0        0       57 2023-05-30 13:53:49.372018 thoughtful-2.0.0rc1/thoughtful/__version__.py
+-rw-r--r--   0        0        0     1070 2023-05-25 17:53:34.765146 thoughtful-2.0.0rc1/thoughtful/environment_variables.py
+-rw-r--r--   0        0        0      143 2022-12-14 17:25:44.949518 thoughtful-2.0.0rc1/thoughtful/supervisor/__init__.py
+-rw-r--r--   0        0        0     4464 2023-05-26 20:50:27.370219 thoughtful-2.0.0rc1/thoughtful/supervisor/default_instances.py
+-rw-r--r--   0        0        0     8598 2023-05-24 14:25:56.931578 thoughtful-2.0.0rc1/thoughtful/supervisor/main_context.py
+-rw-r--r--   0        0        0    10567 2022-12-14 17:25:44.949966 thoughtful-2.0.0rc1/thoughtful/supervisor/manifest.py
+-rw-r--r--   0        0        0        0 2022-12-14 17:25:44.949991 thoughtful-2.0.0rc1/thoughtful/supervisor/py.typed
+-rw-r--r--   0        0        0        0 2022-12-14 17:25:44.950159 thoughtful-2.0.0rc1/thoughtful/supervisor/reporting/__init__.py
+-rw-r--r--   0        0        0     2872 2023-05-26 19:04:25.164500 thoughtful-2.0.0rc1/thoughtful/supervisor/reporting/record.py
+-rw-r--r--   0        0        0     1189 2023-05-26 19:04:25.164751 thoughtful-2.0.0rc1/thoughtful/supervisor/reporting/record_report.py
+-rw-r--r--   0        0        0     2066 2023-05-26 19:04:25.164927 thoughtful-2.0.0rc1/thoughtful/supervisor/reporting/report.py
+-rw-r--r--   0        0        0    10118 2023-05-26 19:04:25.165217 thoughtful-2.0.0rc1/thoughtful/supervisor/reporting/report_builder.py
+-rw-r--r--   0        0        0      660 2023-05-26 19:04:25.165378 thoughtful-2.0.0rc1/thoughtful/supervisor/reporting/status.py
+-rw-r--r--   0        0        0      876 2023-05-26 19:04:25.165550 thoughtful-2.0.0rc1/thoughtful/supervisor/reporting/step_report.py
+-rw-r--r--   0        0        0     1541 2022-12-14 17:25:44.951007 thoughtful-2.0.0rc1/thoughtful/supervisor/reporting/timed_report.py
+-rw-r--r--   0        0        0     1754 2023-05-26 19:04:25.165733 thoughtful-2.0.0rc1/thoughtful/supervisor/reporting/timer.py
+-rw-r--r--   0        0        0     7627 2023-05-26 19:04:25.165919 thoughtful-2.0.0rc1/thoughtful/supervisor/step_context.py
+-rw-r--r--   0        0        0     7462 2023-05-25 17:53:34.765671 thoughtful-2.0.0rc1/thoughtful/supervisor/step_decorator_factory.py
+-rw-r--r--   0        0        0        0 2023-01-30 21:43:52.785761 thoughtful-2.0.0rc1/thoughtful/supervisor/streaming/__init__.py
+-rw-r--r--   0        0        0      736 2023-04-06 19:41:20.157278 thoughtful-2.0.0rc1/thoughtful/supervisor/streaming/action.py
+-rw-r--r--   0        0        0     5645 2023-05-30 13:47:08.800861 thoughtful-2.0.0rc1/thoughtful/supervisor/streaming/callback.py
+-rw-r--r--   0        0        0     3184 2023-05-24 14:48:54.311303 thoughtful-2.0.0rc1/thoughtful/supervisor/streaming/payloads.py
+-rw-r--r--   0        0        0     4257 1970-01-01 00:00:00.000000 thoughtful-2.0.0rc1/setup.py
+-rw-r--r--   0        0        0     4592 1970-01-01 00:00:00.000000 thoughtful-2.0.0rc1/PKG-INFO
```

### Comparing `thoughtful-2.0.0rc0/LICENSE` & `thoughtful-2.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc0/README.md` & `thoughtful-2.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc0/pyproject.toml` & `thoughtful-2.0.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thoughtful"
-version = "2.0.0rc0"
+version = "2.0.0rc1"
 description = "Thoughtful is a python package by Thoughtful for helping manage automations with helpful packages like supervisor"
 authors = ["Thoughtful Automation <engineering@thoughtfulautomation.com>"]
 license = "Apache-2.0"
 readme = 'README.md'
 homepage = "https://thoughtfulautomation.com"
 repository = "https://github.com/thoughtful-automation/thoughtful"
 documentation = "https://readthedocs.com/projects/thoughtful-supervisor/"
@@ -31,14 +31,15 @@
 pre-commit = "^2.17.0"
 pydantic-yaml = "^0.6.3"
 isodate = "^0.6.1"
 boto3 = "^1.24.64"
 aws-requests-auth = "^0.4.3"
 moto = "^4.0.5"
 requests = "^2.28.1"
+pyjwt = "^2.7.0"
 
 [tool.poetry.dev-dependencies]
 mkdocs = "^1.2.3"
 datamodel-code-generator = "^0.11.14"
 mkdocstrings = "^0.16.2"
 pytest = "^7.2.0"
 pytest-cov = "^2.12.1"
```

### Comparing `thoughtful-2.0.0rc0/thoughtful/environment_variables.py` & `thoughtful-2.0.0rc1/thoughtful/environment_variables.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc0/thoughtful/supervisor/default_instances.py` & `thoughtful-2.0.0rc1/thoughtful/supervisor/default_instances.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,29 +3,23 @@
 
 Typically, developers will only run one digital worker on a Python
 runtime, and it is tricky to initialize an object and pass that object
 instance down into other files in a project for a custom decorator.
 This package provides a set of default instances of objects and contexts
 for dynamic runs.
 
-This file initializes a shared `ReportBuilder` and `Recorder` for
-individual steps and sub steps to share, then creates:
-
-    - a default ``MainContext`` named ``supervise``,
-    - a decorator to annotate steps called ``step``,
-    - a ``StepContext`` named ``step_context``,
-    - a function to set step statuses called ``set_step_status``,
-    - and a function to set record statuses called ``set_record_status``.
+This file initializes a shared `ReportBuilder` object, which is used
+individual steps and sub steps to share state.
 
 See the quickstart for, well, quickstarts on each of these methods.
 """
 
 import logging
 import pathlib
-from typing import Optional, Union
+from typing import Union
 
 from thoughtful.environment_variables import EnvironmentVariables
 from thoughtful.supervisor.main_context import MainContext
 from thoughtful.supervisor.manifest import Manifest
 from thoughtful.supervisor.reporting.report_builder import ReportBuilder
 from thoughtful.supervisor.step_context import StepContext
 from thoughtful.supervisor.step_decorator_factory import create_step_decorator
@@ -39,15 +33,17 @@
     run_id=EnvironmentVariables().run_id,
     callback_url=EnvironmentVariables().callback_url,
     # The JWT token is set by the user later. If steamer is set to None,
     # then the step decorators can't be updated to stream if streamer is
     # changed to a new instance.
     #
     # See CX-2368 for the proper fix by lifting the streamer out of the contexts
-    jwt_token="",
+    access_token="",
+    refresh_token="",
+    refresh_url="",
 )
 
 #: A shared ``ReportBuilder`` for steps and step contexts to add step reports
 #: to.
 report_builder = ReportBuilder()
 
 #: Use this decorator on your own functions to mark what workflow step each
```

### Comparing `thoughtful-2.0.0rc0/thoughtful/supervisor/main_context.py` & `thoughtful-2.0.0rc1/thoughtful/supervisor/main_context.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc0/thoughtful/supervisor/manifest.py` & `thoughtful-2.0.0rc1/thoughtful/supervisor/manifest.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc0/thoughtful/supervisor/reporting/record.py` & `thoughtful-2.0.0rc1/thoughtful/supervisor/reporting/record.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,37 +30,40 @@
 
 from thoughtful.supervisor.reporting.status import Status
 
 
 @dataclass
 class Record:
     """
-    A record can refer to any object that is being processed by a step. It
-    is here represented by its ID and its status.
+    A record can refer to any object that is being processed by a step. If a
+    step in your workflow is repeating many times for different items, then
+    each item you're iterating over can be a record.
     """
 
     record_id: str
     """
     str: The status of the record.
     """
 
     status: Status
     """
     Status: The status of the record.
     """
 
     message: Optional[str] = field(default_factory=str)
     """
-    Message: Place to store a message about the record. limit 120 characters
+    Message: A message that can provide additional information about the record,
+    such as a (short) description of why the record is in a certain state.
     """
 
     # make required default = {} ?
     metadata: Optional[dict] = field(default_factory=dict)
     """
-    Metadata: Place to store metadata about the record.
+    Metadata: A dictionary of additional information about the record. This is
+    mostly meant to "tag" the record for later analysis and grouping.
     """
 
     def __post_init__(self):
         """
         Validate the record message length
         """
         if len(self.message) > 120:
```

### Comparing `thoughtful-2.0.0rc0/thoughtful/supervisor/reporting/record_report.py` & `thoughtful-2.0.0rc1/thoughtful/supervisor/reporting/record_report.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 from __future__ import annotations
 
-from dataclasses import dataclass, field
+from dataclasses import dataclass
 from typing import Any, Dict
 
 from thoughtful.supervisor.reporting.record import Record
 from thoughtful.supervisor.reporting.status import Status
 from thoughtful.supervisor.reporting.step_report import StepReport
 from thoughtful.supervisor.reporting.timed_report import TimedReport
 
 
 @dataclass
 class RecordReport(TimedReport):
-
     step_id: str
     """
     str: The ID of the step.
     """
 
     status: Status
     """
     Status: The status of the step.
     """
+
     record: Record
+    """
+    Record: The record that was processed by the step.
+    """
 
     @classmethod
     def from_step_report(cls, step_report: StepReport, record: Record) -> RecordReport:
         return cls(
             start_time=step_report.start_time,
             end_time=step_report.end_time,
             step_id=step_report.step_id,
```

### Comparing `thoughtful-2.0.0rc0/thoughtful/supervisor/reporting/report.py` & `thoughtful-2.0.0rc1/thoughtful/supervisor/reporting/report.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,18 +17,17 @@
 from thoughtful.supervisor.reporting.step_report import StepReport
 from thoughtful.supervisor.reporting.timed_report import TimedReport
 
 
 @dataclass
 class Report(TimedReport):
     """
-    Report: A report is a representation of a run's execution. This dataclass
-    contains all the information that will be stored in the run report,
-    including a list of the steps that were executed. This is the parent
-    class of the run report, and as such will only ever be one per run report.
+    A report is a representation of a run's execution, and it includes metadata
+    about the run, a list of the steps that were executed, and records that
+    were processed in each step (if any). There will only be one report per run.
     """
 
     supervisor_version = str(__version__)
     """
     str: The version of the supervisor that generated the report.
     """
```

### Comparing `thoughtful-2.0.0rc0/thoughtful/supervisor/reporting/report_builder.py` & `thoughtful-2.0.0rc1/thoughtful/supervisor/reporting/report_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,18 +4,16 @@
 to a ``Report`` object containing the list of ``StepReport`` objects.
 
 It returns this ``Report`` object as the final product of the run.
 """
 
 from __future__ import annotations
 
-import copy
 import datetime
 import time
-import warnings
 from collections import OrderedDict, defaultdict
 from dataclasses import dataclass, field
 from typing import Dict, Iterable, List, Optional, Tuple, Union
 
 from thoughtful.supervisor.manifest import StepId
 from thoughtful.supervisor.reporting.record import Record
 from thoughtful.supervisor.reporting.record_report import RecordReport
@@ -23,14 +21,18 @@
 from thoughtful.supervisor.reporting.status import Status
 from thoughtful.supervisor.reporting.step_report import StepReport
 from thoughtful.supervisor.reporting.timer import Timer
 
 
 @dataclass
 class RecordAccumulator:
+    """
+    Manages a list of records that are being processed by a step.
+    """
+
     records_by_id: Dict[RecordId, Record] = field(default_factory=OrderedDict)
 
     def upsert(self, record: Record):
         """Insert a new Record, or update the record if it already exists."""
         self.records_by_id[record.record_id] = record
 
     def exists(self, _id: RecordId) -> bool:
@@ -57,18 +59,17 @@
     def __iter__(self) -> Iterable[Record]:
         return iter(self.records_by_id.values())
 
 
 @dataclass
 class StepReportBuilder:
     """
-    Builds a dynamic digital worker step. This is similar to the ``StepReport``
-    except that this is higher level in that it contains unflattened data
-    structures, such as ``Record`` objects. It has functionality
-    to produce a ``StepReport`` from itself.
+    Builds a step report during the lifecycle of a step's execution. Once a step
+    has finished executing, you can call ``_to_report`` to get the final
+    ``StepReport``.
     """
 
     step_id: str
     """
     str: The ID of the step.
     """
 
@@ -88,23 +89,21 @@
     """
 
     _record_accumulator: RecordAccumulator = field(default_factory=RecordAccumulator)
     """
     RecordAccumulator: Holds records that were processed by this step.
     """
 
-    def to_reports(self) -> List[StepReport]:
+    def to_reports(self) -> List[Union[StepReport, RecordReport]]:
         step_report = self._to_report()
-        record_reports: List[StepReport] = self._record_accumulator.to_reports(
-            step_report
-        )
+        record_reports: List[
+            Union[StepReport, RecordReport]
+        ] = self._record_accumulator.to_reports(step_report)
         return record_reports + [step_report]
 
-    # NOTE: optional fields for message & metadata
-    # use **metadata instead?
     def set_record_status(
         self,
         record_id: RecordId,
         status: Status,
         message: Optional[str] = None,
         metadata: Optional[dict] = None,
         is_soft_update: bool = False,
```

### Comparing `thoughtful-2.0.0rc0/thoughtful/supervisor/reporting/status.py` & `thoughtful-2.0.0rc1/thoughtful/supervisor/reporting/status.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,9 +26,9 @@
     WARNING = "warning"
     """
     The item requires attention.
     """
 
     RUNNING = "running"
     """
-    The item is running
+    The item is running.
     """
```

### Comparing `thoughtful-2.0.0rc0/thoughtful/supervisor/reporting/step_report.py` & `thoughtful-2.0.0rc1/thoughtful/supervisor/reporting/step_report.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from dataclasses import dataclass, field
+from dataclasses import dataclass
 from typing import Any, Dict
 
 from thoughtful.supervisor.reporting.status import Status
 from thoughtful.supervisor.reporting.timed_report import TimedReport
 
 
 @dataclass
```

### Comparing `thoughtful-2.0.0rc0/thoughtful/supervisor/reporting/timed_report.py` & `thoughtful-2.0.0rc1/thoughtful/supervisor/reporting/timed_report.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc0/thoughtful/supervisor/reporting/timer.py` & `thoughtful-2.0.0rc1/thoughtful/supervisor/reporting/timer.py`

 * *Files 13% similar despite different names*

```diff
@@ -50,21 +50,18 @@
     """
 
     duration: Optional[datetime.timedelta] = None
     """
     datetime.timedelta, optional: The duration of the timer.
     """
 
-    _perf_counter_start_value: Optional[float] = None
-
     def start(self) -> datetime.datetime:
         """
         Starts the timer.
         """
-        self._perf_counter_start_value = time.perf_counter()
         self.start_time = datetime.datetime.now()
         return self.start_time
 
     def end(self) -> TimerResult:
         """
         Ends the timer and records the duration.
```

### Comparing `thoughtful-2.0.0rc0/thoughtful/supervisor/step_context.py` & `thoughtful-2.0.0rc1/thoughtful/supervisor/step_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 the ``self`` object from a context manager, we can use this to update
 attributes such as the record status, the step status, and is even a bit
 cleaner when setting the record ID.
 """
 
 from __future__ import annotations
 
-import warnings
 from types import TracebackType
 from typing import Optional, Type, Union
 
 from thoughtful.supervisor.reporting.report_builder import ReportBuilder
 from thoughtful.supervisor.reporting.report_builder import StepReportBuilder
 from thoughtful.supervisor.reporting.status import Status
 from thoughtful.supervisor.reporting.timer import Timer
```

### Comparing `thoughtful-2.0.0rc0/thoughtful/supervisor/step_decorator_factory.py` & `thoughtful-2.0.0rc1/thoughtful/supervisor/step_decorator_factory.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc0/thoughtful/supervisor/streaming/action.py` & `thoughtful-2.0.0rc1/thoughtful/supervisor/streaming/action.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc0/thoughtful/supervisor/streaming/payloads.py` & `thoughtful-2.0.0rc1/thoughtful/supervisor/streaming/payloads.py`

 * *Files identical despite different names*

### Comparing `thoughtful-2.0.0rc0/setup.py` & `thoughtful-2.0.0rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,21 @@
  'chevron>=0.14.0,<0.15.0',
  'isodate>=0.6.1,<0.7.0',
  'moto>=4.0.5,<5.0.0',
  'pre-commit>=2.17.0,<3.0.0',
  'pyconfs>=0.5.5,<0.6.0',
  'pydantic-yaml>=0.6.3,<0.7.0',
  'pydantic>=1.8.2,<2.0.0',
+ 'pyjwt>=2.7.0,<3.0.0',
  'pyyaml>=5.4.1',
  'requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'thoughtful',
-    'version': '2.0.0rc0',
+    'version': '2.0.0rc1',
     'description': 'Thoughtful is a python package by Thoughtful for helping manage automations with helpful packages like supervisor',
     'long_description': '**thoughtful** is a collection of open-source libraries and tools for Robot Process\nAutomation (RPA) development. The goal of this project is to provide a set of\nfor supervising bot execution, and enabling these bots to do more.\n\n[![PyPi version](https://badgen.net/pypi/v/thoughtful/)](https://pypi.org/project/thoughtful/)\n![Main Branch Tests](https://github.com/Thoughtful-Automation/supervisor/actions/workflows/main-push.yml/badge.svg?branch=main)\n[![Supported Versions](https://img.shields.io/pypi/pyversions/thoughtful.svg)](https://pypi.org/project/thoughtful)\n[![Downloads](https://pepy.tech/badge/thoughtful/month)](https://pepy.tech/project/thoughtful)\n\n[//]: # ([![GitHub release]&#40;https://img.shields.io/github/release/Thoughtful-Automation/supervisor.svg&#41;]&#40;https://GitHub.com/Naereen/StrapDown.js/releases/&#41;)\n\n\nThis project is:\n* Open-source: [GitHub][url:gh]\n* Owned by [thoughtful][url:ta]\n* Licensed under the [Apache License 2.0][url:al]\n\nLinks:\n* [Homepage][url:gh]\n* [Documentation][url:readthedocs]\n* [PyPI][url:pypi]\n\n**thoughtful** is available on [PyPI][url:pypi] and can be installed using pip:\n\n```sh\npip install thoughtful\n```\n\n---\n\n**thoughtful** officially supports Python 3.7+.\n\n---\n\n# Libraries\n\nThis is a list of the available libraries in this project. API Reference\nand User Guide available on [docs][url:readthedocs].\n\n## Supervisor\n\nSupervisor is a Workflow Engine for Digital Workers that constructs\nand broadcasts a detailed and structured telemetric log, called the Run Report.\n\n```python\nfrom thoughtful.supervisor import step, step_scope, supervise, set_step_status\n\n\n# using the step decorator\n@step("2")\ndef step_2(name: str) -> bool:\n    print(f\'Hello {name}\')\n    return True  # some condition\n\ndef main() -> None:\n    # using the step_scope context manager\n    with step_scope(\'1\') as step_context:\n        try:\n            print("Getting credentials")\n            # ...\n        except Exception as e:\n            # set step status using method\n            step_context.set_status("warning")\n\n    if not step_2():\n        # set step status using function\n        set_step_status("2", "fail")\n\nif __name__ == \'__main__\':\n    with supervise():\n        main()\n```\n\n## Contributing\n\nContributions to **thoughtful** are welcome!\n\nTo get started, see the [contributing guide](CONTRIBUTING.md).\n\n---\n\n  Made with ❤️ by\n\n  [![Thoughtful](https://user-images.githubusercontent.com/1096881/141985289-317c2e72-3c2d-4e6b-800a-0def1a05f599.png)][url:ta]\n\n---\n\nThis project is open-source and licensed under the terms of the [Apache License 2.0][url:al].\n\n\n<!--  Link References -->\n\n[url:ta]: https://www.thoughtful.ai/\n[url:gh]: https://github.com/Thoughtful-Automation/supervisor\n[url:pypi]: https://pypi.org/project/thoughtful/\n[git:issues]: https://github.com/Thoughtful-Automation/supervisor/issues\n[url:readthedocs]: https://thoughtful-supervisor.readthedocs-hosted.com/en/latest/\n[url:al]: http://www.apache.org/licenses/LICENSE-2.0\n',
     'author': 'Thoughtful Automation',
     'author_email': 'engineering@thoughtfulautomation.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://thoughtfulautomation.com',
```

### Comparing `thoughtful-2.0.0rc0/PKG-INFO` & `thoughtful-2.0.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thoughtful
-Version: 2.0.0rc0
+Version: 2.0.0rc1
 Summary: Thoughtful is a python package by Thoughtful for helping manage automations with helpful packages like supervisor
 Home-page: https://thoughtfulautomation.com
 License: Apache-2.0
 Keywords: rpa,robot-framework,robocorp,automation
 Author: Thoughtful Automation
 Author-email: engineering@thoughtfulautomation.com
 Requires-Python: >=3.8,<3.12
@@ -23,14 +23,15 @@
 Requires-Dist: chevron (>=0.14.0,<0.15.0)
 Requires-Dist: isodate (>=0.6.1,<0.7.0)
 Requires-Dist: moto (>=4.0.5,<5.0.0)
 Requires-Dist: pre-commit (>=2.17.0,<3.0.0)
 Requires-Dist: pyconfs (>=0.5.5,<0.6.0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: pydantic-yaml (>=0.6.3,<0.7.0)
+Requires-Dist: pyjwt (>=2.7.0,<3.0.0)
 Requires-Dist: pyyaml (>=5.4.1)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Project-URL: Documentation, https://readthedocs.com/projects/thoughtful-supervisor/
 Project-URL: Repository, https://github.com/thoughtful-automation/thoughtful
 Description-Content-Type: text/markdown
 
 **thoughtful** is a collection of open-source libraries and tools for Robot Process
```

