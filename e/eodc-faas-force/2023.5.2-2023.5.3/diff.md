# Comparing `tmp/eodc_faas_force-2023.5.2.tar.gz` & `tmp/eodc_faas_force-2023.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc_faas_force-2023.5.2.tar", max compression
+gzip compressed data, was "eodc_faas_force-2023.5.3.tar", max compression
```

## Comparing `eodc_faas_force-2023.5.2.tar` & `eodc_faas_force-2023.5.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       24 2023-05-04 07:19:47.659253 eodc_faas_force-2023.5.2/README.md
--rw-r--r--   0        0        0       93 2023-05-26 15:27:33.283253 eodc_faas_force-2023.5.2/force_processor_bindings/__init__.py
--rw-r--r--   0        0        0     1488 2023-05-16 14:30:15.567253 eodc_faas_force-2023.5.2/force_processor_bindings/model.py
--rw-r--r--   0        0        0     4754 2023-05-23 08:18:00.179253 eodc_faas_force-2023.5.2/force_processor_bindings/workflows.py
--rw-r--r--   0        0        0      692 2023-05-26 15:27:33.283253 eodc_faas_force-2023.5.2/pyproject.toml
--rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 eodc_faas_force-2023.5.2/PKG-INFO
+-rw-r--r--   0        0        0       24 2023-05-04 07:19:47.663253 eodc_faas_force-2023.5.3/README.md
+-rw-r--r--   0        0        0       93 2023-05-30 19:07:23.539253 eodc_faas_force-2023.5.3/force_processor_bindings/__init__.py
+-rw-r--r--   0        0        0     1907 2023-05-30 18:55:22.711253 eodc_faas_force-2023.5.3/force_processor_bindings/model.py
+-rw-r--r--   0        0        0     4754 2023-05-23 08:18:00.251253 eodc_faas_force-2023.5.3/force_processor_bindings/workflows.py
+-rw-r--r--   0        0        0      692 2023-05-30 19:07:23.539253 eodc_faas_force-2023.5.3/pyproject.toml
+-rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 eodc_faas_force-2023.5.3/PKG-INFO
```

### Comparing `eodc_faas_force-2023.5.2/force_processor_bindings/workflows.py` & `eodc_faas_force-2023.5.3/force_processor_bindings/workflows.py`

 * *Files identical despite different names*

### Comparing `eodc_faas_force-2023.5.2/pyproject.toml` & `eodc_faas_force-2023.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eodc-faas-force"
-version = "2023.5.2"
+version = "2023.5.3"
 description = "Bindings for the FORCE processor exposed at EODC"
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>", "Sean Hoyal <sean.hoyal@eodc.eu>", "Valentina Hutter <valentina.hutter@eodc.eu>"]
 readme = "README.md"
 packages = [{include = "force_processor_bindings"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `eodc_faas_force-2023.5.2/PKG-INFO` & `eodc_faas_force-2023.5.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodc-faas-force
-Version: 2023.5.2
+Version: 2023.5.3
 Summary: Bindings for the FORCE processor exposed at EODC
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

