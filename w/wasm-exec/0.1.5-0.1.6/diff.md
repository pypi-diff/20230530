# Comparing `tmp/wasm_exec-0.1.5.tar.gz` & `tmp/wasm_exec-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wasm_exec-0.1.5.tar", max compression
+gzip compressed data, was "wasm_exec-0.1.6.tar", max compression
```

## Comparing `wasm_exec-0.1.5.tar` & `wasm_exec-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0     1069 2023-05-29 05:27:38.625179 wasm_exec-0.1.5/LICENSE
--rw-r--r--   0        0        0     3058 2023-05-29 05:27:38.625179 wasm_exec-0.1.5/README.md
--rw-r--r--   0        0        0      818 2023-05-29 05:27:38.625179 wasm_exec-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3519 2023-05-29 05:27:38.625179 wasm_exec-0.1.5/wasm_exec/__init__.py
--rw-r--r--   0        0        0 20538911 2023-05-29 05:27:38.733183 wasm_exec-0.1.5/wasm_runtime/python-3.11.3.wasm
--rw-r--r--   0        0        0      121 2023-05-29 05:27:38.733183 wasm_exec-0.1.5/wasm_runtime/python-3.11.3.wasm.sha256sum
--rw-r--r--   0        0        0     1424 2023-05-29 05:27:38.733183 wasm_exec-0.1.5/wasm_runtime/wasm_runtime.py
--rw-r--r--   0        0        0     3757 1970-01-01 00:00:00.000000 wasm_exec-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-30 05:27:52.549963 wasm_exec-0.1.6/LICENSE
+-rw-r--r--   0        0        0     3083 2023-05-30 05:27:52.549963 wasm_exec-0.1.6/README.md
+-rw-r--r--   0        0        0      818 2023-05-30 05:27:52.549963 wasm_exec-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3881 2023-05-30 05:27:52.549963 wasm_exec-0.1.6/wasm_exec/__init__.py
+-rw-r--r--   0        0        0       41 2023-05-30 05:27:52.549963 wasm_exec-0.1.6/wasm_exec/exceptions.py
+-rw-r--r--   0        0        0      215 2023-05-30 05:27:52.549963 wasm_exec-0.1.6/wasm_exec/schema.py
+-rw-r--r--   0        0        0 20538911 2023-05-30 05:27:52.669962 wasm_exec-0.1.6/wasm_runtime/python-3.11.3.wasm
+-rw-r--r--   0        0        0      121 2023-05-30 05:27:52.669962 wasm_exec-0.1.6/wasm_runtime/python-3.11.3.wasm.sha256sum
+-rw-r--r--   0        0        0     1424 2023-05-30 05:27:52.669962 wasm_exec-0.1.6/wasm_runtime/wasm_runtime.py
+-rw-r--r--   0        0        0     3782 1970-01-01 00:00:00.000000 wasm_exec-0.1.6/PKG-INFO
```

### Comparing `wasm_exec-0.1.5/LICENSE` & `wasm_exec-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wasm_exec-0.1.5/README.md` & `wasm_exec-0.1.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 
 ## Install 
 
 ```pip install wasm_exec```
 
 ## Usage
 ```
-from wasm_exec import wasm_exec
+from wasm_exec import WasmExecutor
 
+wasm = WasmExecutor()
 code = "print('Hello World!')"
-print(wasm_exec(code).text)
+print(wasm.exec(code).text)
 
 >> Hello World!
 ```
 
 ## How does this work? 
 
 - Arbitrary Python code is passed to the `wasm_exec` function
```

### Comparing `wasm_exec-0.1.5/pyproject.toml` & `wasm_exec-0.1.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wasm-exec"
-version = "0.1.5"
+version = "0.1.6"
 description = "WASM-powered, sandboxed version of `exec()` for running dynamic code."
 authors = ["Justin Flick"]
 license = "MIT"
 readme = "README.md"
 repository = "https://www.github.com/jflick58/wasm_exec"
 packages = [
     { include = "wasm_exec" },
```

### Comparing `wasm_exec-0.1.5/wasm_runtime/python-3.11.3.wasm` & `wasm_exec-0.1.6/wasm_runtime/python-3.11.3.wasm`

 * *Files identical despite different names*

### Comparing `wasm_exec-0.1.5/wasm_runtime/wasm_runtime.py` & `wasm_exec-0.1.6/wasm_runtime/wasm_runtime.py`

 * *Files identical despite different names*

### Comparing `wasm_exec-0.1.5/PKG-INFO` & `wasm_exec-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wasm-exec
-Version: 0.1.5
+Version: 0.1.6
 Summary: WASM-powered, sandboxed version of `exec()` for running dynamic code.
 Home-page: https://www.github.com/jflick58/wasm_exec
 License: MIT
 Author: Justin Flick
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -25,18 +25,19 @@
 
 ## Install 
 
 ```pip install wasm_exec```
 
 ## Usage
 ```
-from wasm_exec import wasm_exec
+from wasm_exec import WasmExecutor
 
+wasm = WasmExecutor()
 code = "print('Hello World!')"
-print(wasm_exec(code).text)
+print(wasm.exec(code).text)
 
 >> Hello World!
 ```
 
 ## How does this work? 
 
 - Arbitrary Python code is passed to the `wasm_exec` function
```

