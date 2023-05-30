# Comparing `tmp/python_omnilogic_local-0.6.0.tar.gz` & `tmp/python_omnilogic_local-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_omnilogic_local-0.6.0.tar", max compression
+gzip compressed data, was "python_omnilogic_local-0.6.1.tar", max compression
```

## Comparing `python_omnilogic_local-0.6.0.tar` & `python_omnilogic_local-0.6.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1696 2023-05-30 20:29:06.407415 python_omnilogic_local-0.6.0/README.md
--rw-r--r--   0        0        0        0 2023-05-30 20:29:06.407415 python_omnilogic_local-0.6.0/pyomnilogic_local/__init__.py
--rw-r--r--   0        0        0    21453 2023-05-30 20:29:06.407415 python_omnilogic_local-0.6.0/pyomnilogic_local/api.py
--rwxr-xr-x   0        0        0     3921 2023-05-30 20:29:06.407415 python_omnilogic_local-0.6.0/pyomnilogic_local/cli.py
--rw-r--r--   0        0        0      164 2023-05-30 20:29:06.407415 python_omnilogic_local-0.6.0/pyomnilogic_local/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-30 20:29:06.407415 python_omnilogic_local-0.6.0/pyomnilogic_local/models/__init__.py
--rw-r--r--   0        0        0       51 2023-05-30 20:29:06.407415 python_omnilogic_local-0.6.0/pyomnilogic_local/models/const.py
--rw-r--r--   0        0        0     1532 2023-05-30 20:29:06.407415 python_omnilogic_local-0.6.0/pyomnilogic_local/models/filter_diagnostics.py
--rw-r--r--   0        0        0      407 2023-05-30 20:29:06.407415 python_omnilogic_local-0.6.0/pyomnilogic_local/models/leadmessage.py
--rw-r--r--   0        0        0     8352 2023-05-30 20:29:06.407415 python_omnilogic_local-0.6.0/pyomnilogic_local/models/mspconfig.py
--rw-r--r--   0        0        0     9962 2023-05-30 20:29:06.407415 python_omnilogic_local-0.6.0/pyomnilogic_local/models/telemetry.py
--rw-r--r--   0        0        0     1476 2023-05-30 20:29:06.407415 python_omnilogic_local-0.6.0/pyomnilogic_local/models/util.py
--rw-r--r--   0        0        0    10189 2023-05-30 20:29:06.407415 python_omnilogic_local-0.6.0/pyomnilogic_local/protocol.py
--rw-r--r--   0        0        0     6325 2023-05-30 20:29:06.407415 python_omnilogic_local-0.6.0/pyomnilogic_local/types.py
--rw-r--r--   0        0        0      359 2023-05-30 20:29:06.407415 python_omnilogic_local-0.6.0/pyomnilogic_local/util.py
--rw-r--r--   0        0        0     5227 2023-05-30 20:29:07.371425 python_omnilogic_local-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 python_omnilogic_local-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1696 2023-05-30 21:09:13.113471 python_omnilogic_local-0.6.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-30 21:09:13.117471 python_omnilogic_local-0.6.1/pyomnilogic_local/__init__.py
+-rw-r--r--   0        0        0    21453 2023-05-30 21:09:13.117471 python_omnilogic_local-0.6.1/pyomnilogic_local/api.py
+-rwxr-xr-x   0        0        0     3921 2023-05-30 21:09:13.117471 python_omnilogic_local-0.6.1/pyomnilogic_local/cli.py
+-rw-r--r--   0        0        0      164 2023-05-30 21:09:13.117471 python_omnilogic_local-0.6.1/pyomnilogic_local/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-30 21:09:13.117471 python_omnilogic_local-0.6.1/pyomnilogic_local/models/__init__.py
+-rw-r--r--   0        0        0       51 2023-05-30 21:09:13.117471 python_omnilogic_local-0.6.1/pyomnilogic_local/models/const.py
+-rw-r--r--   0        0        0     1532 2023-05-30 21:09:13.117471 python_omnilogic_local-0.6.1/pyomnilogic_local/models/filter_diagnostics.py
+-rw-r--r--   0        0        0      407 2023-05-30 21:09:13.117471 python_omnilogic_local-0.6.1/pyomnilogic_local/models/leadmessage.py
+-rw-r--r--   0        0        0     8352 2023-05-30 21:09:13.117471 python_omnilogic_local-0.6.1/pyomnilogic_local/models/mspconfig.py
+-rw-r--r--   0        0        0     9968 2023-05-30 21:09:13.117471 python_omnilogic_local-0.6.1/pyomnilogic_local/models/telemetry.py
+-rw-r--r--   0        0        0     1476 2023-05-30 21:09:13.117471 python_omnilogic_local-0.6.1/pyomnilogic_local/models/util.py
+-rw-r--r--   0        0        0    10189 2023-05-30 21:09:13.117471 python_omnilogic_local-0.6.1/pyomnilogic_local/protocol.py
+-rw-r--r--   0        0        0     6325 2023-05-30 21:09:13.117471 python_omnilogic_local-0.6.1/pyomnilogic_local/types.py
+-rw-r--r--   0        0        0      359 2023-05-30 21:09:13.117471 python_omnilogic_local-0.6.1/pyomnilogic_local/util.py
+-rw-r--r--   0        0        0     5227 2023-05-30 21:09:14.245502 python_omnilogic_local-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 python_omnilogic_local-0.6.1/PKG-INFO
```

### Comparing `python_omnilogic_local-0.6.0/README.md` & `python_omnilogic_local-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.6.0/pyomnilogic_local/api.py` & `python_omnilogic_local-0.6.1/pyomnilogic_local/api.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.6.0/pyomnilogic_local/cli.py` & `python_omnilogic_local-0.6.1/pyomnilogic_local/cli.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.6.0/pyomnilogic_local/models/filter_diagnostics.py` & `python_omnilogic_local-0.6.1/pyomnilogic_local/models/filter_diagnostics.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.6.0/pyomnilogic_local/models/mspconfig.py` & `python_omnilogic_local-0.6.1/pyomnilogic_local/models/mspconfig.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.6.0/pyomnilogic_local/models/telemetry.py` & `python_omnilogic_local-0.6.1/pyomnilogic_local/models/telemetry.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,15 @@
     colorlogic_light: list[TelemetryColorLogicLight] | None = Field(alias="ColorLogic-Light")
     filter: list[TelemetryFilter] | None = Field(alias="Filter")
     group: list[TelemetryGroup] | None = Field(alias="Group")
     heater: list[TelemetryHeater] | None = Field(alias="Heater")
     pump: list[TelemetryPump] | None = Field(alias="Pump")
     relay: list[TelemetryRelay] | None = Field(alias="Relay")
     valve_actuator: list[TelemetryValveActuator] | None = Field(alias="ValveActuator")
-    virtual_heater: TelemetryVirtualHeater | None = Field(alias="VirtualHeater")
+    virtual_heater: list[TelemetryVirtualHeater] | None = Field(alias="VirtualHeater")
 
     class Config:
         orm_mode = True
 
     @staticmethod
     def load_xml(xml: str) -> Telemetry:
```

### Comparing `python_omnilogic_local-0.6.0/pyomnilogic_local/models/util.py` & `python_omnilogic_local-0.6.1/pyomnilogic_local/models/util.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.6.0/pyomnilogic_local/protocol.py` & `python_omnilogic_local-0.6.1/pyomnilogic_local/protocol.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.6.0/pyomnilogic_local/types.py` & `python_omnilogic_local-0.6.1/pyomnilogic_local/types.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.6.0/pyproject.toml` & `python_omnilogic_local-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-omnilogic-local"
-version = "0.6.0"
+version = "0.6.1"
 description = "A library for local control of Hayward OmniHub/OmniLogic pool controllers using their local API"
 authors = ["cryptk <cryptk@users.noreply.github.com>", "djtimca", "garionphx"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cryptk/python-omnilogic-local"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `python_omnilogic_local-0.6.0/PKG-INFO` & `python_omnilogic_local-0.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-omnilogic-local
-Version: 0.6.0
+Version: 0.6.1
 Summary: A library for local control of Hayward OmniHub/OmniLogic pool controllers using their local API
 Home-page: https://github.com/cryptk/python-omnilogic-local
 License: Apache-2.0
 Author: cryptk
 Author-email: cryptk@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.6.0 Summary: A
+Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.6.1 Summary: A
 library for local control of Hayward OmniHub/OmniLogic pool controllers using
 their local API Home-page: https://github.com/cryptk/python-omnilogic-local
 License: Apache-2.0 Author: cryptk Author-email:
 cryptk@users.noreply.github.com Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
```

