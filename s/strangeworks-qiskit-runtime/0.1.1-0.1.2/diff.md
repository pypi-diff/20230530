# Comparing `tmp/strangeworks_qiskit_runtime-0.1.1.tar.gz` & `tmp/strangeworks_qiskit_runtime-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_qiskit_runtime-0.1.1.tar", max compression
+gzip compressed data, was "strangeworks_qiskit_runtime-0.1.2.tar", max compression
```

## Comparing `strangeworks_qiskit_runtime-0.1.1.tar` & `strangeworks_qiskit_runtime-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      204 2023-05-24 16:08:06.914362 strangeworks_qiskit_runtime-0.1.1/README.md
--rw-r--r--   0        0        0      887 2023-05-24 16:08:22.338498 strangeworks_qiskit_runtime-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      389 2023-05-24 16:08:06.914362 strangeworks_qiskit_runtime-0.1.1/strangeworks_qiskit_runtime/__init__.py
--rw-r--r--   0        0        0     4753 2023-05-24 16:08:06.914362 strangeworks_qiskit_runtime-0.1.1/strangeworks_qiskit_runtime/runtime_client.py
--rw-r--r--   0        0        0    10759 2023-05-24 16:08:06.914362 strangeworks_qiskit_runtime-0.1.1/strangeworks_qiskit_runtime/service.py
--rw-r--r--   0        0        0     6805 2023-05-24 16:08:06.914362 strangeworks_qiskit_runtime-0.1.1/strangeworks_qiskit_runtime/sw_runtime_job.py
--rw-r--r--   0        0        0     5515 2023-05-24 16:08:06.914362 strangeworks_qiskit_runtime-0.1.1/strangeworks_qiskit_runtime/swestimator.py
--rw-r--r--   0        0        0     4549 2023-05-24 16:08:06.914362 strangeworks_qiskit_runtime-0.1.1/strangeworks_qiskit_runtime/swsampler.py
--rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 strangeworks_qiskit_runtime-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      204 2023-05-30 10:29:40.207283 strangeworks_qiskit_runtime-0.1.2/README.md
+-rw-r--r--   0        0        0      887 2023-05-30 10:29:54.584081 strangeworks_qiskit_runtime-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      389 2023-05-30 10:29:40.211283 strangeworks_qiskit_runtime-0.1.2/strangeworks_qiskit_runtime/__init__.py
+-rw-r--r--   0        0        0     4753 2023-05-30 10:29:40.211283 strangeworks_qiskit_runtime-0.1.2/strangeworks_qiskit_runtime/runtime_client.py
+-rw-r--r--   0        0        0    10901 2023-05-30 10:29:40.211283 strangeworks_qiskit_runtime-0.1.2/strangeworks_qiskit_runtime/service.py
+-rw-r--r--   0        0        0     6805 2023-05-30 10:29:40.211283 strangeworks_qiskit_runtime-0.1.2/strangeworks_qiskit_runtime/sw_runtime_job.py
+-rw-r--r--   0        0        0     5515 2023-05-30 10:29:40.211283 strangeworks_qiskit_runtime-0.1.2/strangeworks_qiskit_runtime/swestimator.py
+-rw-r--r--   0        0        0     4549 2023-05-30 10:29:40.211283 strangeworks_qiskit_runtime-0.1.2/strangeworks_qiskit_runtime/swsampler.py
+-rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 strangeworks_qiskit_runtime-0.1.2/PKG-INFO
```

### Comparing `strangeworks_qiskit_runtime-0.1.1/pyproject.toml` & `strangeworks_qiskit_runtime-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strangeworks-qiskit-runtime"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Your Name <you@example.com>"]
 readme = "README.md"
 packages = [{include = "strangeworks_qiskit_runtime"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `strangeworks_qiskit_runtime-0.1.1/strangeworks_qiskit_runtime/runtime_client.py` & `strangeworks_qiskit_runtime-0.1.2/strangeworks_qiskit_runtime/runtime_client.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit_runtime-0.1.1/strangeworks_qiskit_runtime/service.py` & `strangeworks_qiskit_runtime-0.1.2/strangeworks_qiskit_runtime/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,15 +161,19 @@
 
         return response.get("inputs"), response.get("outputs")
 
     def backends(
         self,
     ) -> Backend:
         """Return a list of available backends."""
-        return strangeworks.backends(backend_type_slugs=[self.channel])
+        if self._channel == "ibm_quantum":
+            slug = "ibm-quantum"
+        elif self._channel == "ibm_cloud":
+            slug = "ibm-cloud"
+        return strangeworks.backends(backend_type_slugs=[slug])
 
     def run(
         self,
         program_id: str,
         inputs: Union[Dict, ParameterNamespace],
         options: Optional[Union[RuntimeOptions, Dict]] = None,
         callback: Optional[Callable] = None,
```

### Comparing `strangeworks_qiskit_runtime-0.1.1/strangeworks_qiskit_runtime/sw_runtime_job.py` & `strangeworks_qiskit_runtime-0.1.2/strangeworks_qiskit_runtime/sw_runtime_job.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit_runtime-0.1.1/strangeworks_qiskit_runtime/swestimator.py` & `strangeworks_qiskit_runtime-0.1.2/strangeworks_qiskit_runtime/swestimator.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit_runtime-0.1.1/strangeworks_qiskit_runtime/swsampler.py` & `strangeworks_qiskit_runtime-0.1.2/strangeworks_qiskit_runtime/swsampler.py`

 * *Files identical despite different names*

### Comparing `strangeworks_qiskit_runtime-0.1.1/PKG-INFO` & `strangeworks_qiskit_runtime-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strangeworks-qiskit-runtime
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

