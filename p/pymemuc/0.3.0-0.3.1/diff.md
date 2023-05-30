# Comparing `tmp/pymemuc-0.3.0.tar.gz` & `tmp/pymemuc-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymemuc-0.3.0.tar", max compression
+gzip compressed data, was "pymemuc-0.3.1.tar", max compression
```

## Comparing `pymemuc-0.3.0.tar` & `pymemuc-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1057 2023-05-30 03:10:01.561799 pymemuc-0.3.0/LICENSE
--rw-r--r--   0        0        0     1586 2023-05-30 03:10:01.561799 pymemuc-0.3.0/README.md
--rw-r--r--   0        0        0      386 2023-05-30 03:10:01.569799 pymemuc-0.3.0/pymemuc/__init__.py
--rw-r--r--   0        0        0    22761 2023-05-30 03:10:01.569799 pymemuc-0.3.0/pymemuc/_command.py
--rw-r--r--   0        0        0      465 2023-05-30 03:10:01.569799 pymemuc-0.3.0/pymemuc/_constants.py
--rw-r--r--   0        0        0     4984 2023-05-30 03:10:01.569799 pymemuc-0.3.0/pymemuc/_control.py
--rw-r--r--   0        0        0     1214 2023-05-30 03:10:01.569799 pymemuc-0.3.0/pymemuc/_decorators.py
--rw-r--r--   0        0        0    13670 2023-05-30 03:10:01.569799 pymemuc-0.3.0/pymemuc/_manage.py
--rw-r--r--   0        0        0     3958 2023-05-30 03:10:01.569799 pymemuc-0.3.0/pymemuc/_memuc.py
--rw-r--r--   0        0        0      891 2023-05-30 03:10:01.569799 pymemuc-0.3.0/pymemuc/exceptions.py
--rw-r--r--   0        0        0     2899 2023-05-30 03:10:01.569799 pymemuc-0.3.0/pymemuc/pymemuc.py
--rw-r--r--   0        0        0      379 2023-05-30 03:10:01.569799 pymemuc-0.3.0/pymemuc/vminfo.py
--rw-r--r--   0        0        0     1665 2023-05-30 03:10:24.335042 pymemuc-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2394 1970-01-01 00:00:00.000000 pymemuc-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-05-30 03:52:05.636738 pymemuc-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1586 2023-05-30 03:52:05.636738 pymemuc-0.3.1/README.md
+-rw-r--r--   0        0        0      386 2023-05-30 03:52:05.636738 pymemuc-0.3.1/pymemuc/__init__.py
+-rw-r--r--   0        0        0    22761 2023-05-30 03:52:05.636738 pymemuc-0.3.1/pymemuc/_command.py
+-rw-r--r--   0        0        0      465 2023-05-30 03:52:05.636738 pymemuc-0.3.1/pymemuc/_constants.py
+-rw-r--r--   0        0        0     4984 2023-05-30 03:52:05.636738 pymemuc-0.3.1/pymemuc/_control.py
+-rw-r--r--   0        0        0     1214 2023-05-30 03:52:05.636738 pymemuc-0.3.1/pymemuc/_decorators.py
+-rw-r--r--   0        0        0    13670 2023-05-30 03:52:05.636738 pymemuc-0.3.1/pymemuc/_manage.py
+-rw-r--r--   0        0        0     3958 2023-05-30 03:52:05.636738 pymemuc-0.3.1/pymemuc/_memuc.py
+-rw-r--r--   0        0        0      891 2023-05-30 03:52:05.636738 pymemuc-0.3.1/pymemuc/exceptions.py
+-rw-r--r--   0        0        0     2899 2023-05-30 03:52:05.636738 pymemuc-0.3.1/pymemuc/pymemuc.py
+-rw-r--r--   0        0        0      379 2023-05-30 03:52:05.636738 pymemuc-0.3.1/pymemuc/vminfo.py
+-rw-r--r--   0        0        0     1665 2023-05-30 03:52:24.932829 pymemuc-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2394 1970-01-01 00:00:00.000000 pymemuc-0.3.1/PKG-INFO
```

### Comparing `pymemuc-0.3.0/LICENSE` & `pymemuc-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.0/README.md` & `pymemuc-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.0/pymemuc/_command.py` & `pymemuc-0.3.1/pymemuc/_command.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.0/pymemuc/_control.py` & `pymemuc-0.3.1/pymemuc/_control.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.0/pymemuc/_decorators.py` & `pymemuc-0.3.1/pymemuc/_decorators.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.0/pymemuc/_manage.py` & `pymemuc-0.3.1/pymemuc/_manage.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 from .vminfo import VMInfo
 
 if TYPE_CHECKING:
     from pymemuc import PyMemuc
 
 
 @_retryable
-def create_vm(self: "PyMemuc", vm_version="76") -> int:
+def create_vm(self: "PyMemuc", vm_version="96") -> int:
     """Create a new VM
 
-    :param vm_version: Android version. Defaults to "76".
+    :param vm_version: Android version. Defaults to "96".
     :type vm_version: str, optional
     :raises PyMemucError: an error if the vm creation failed
     :return: the index of the new VM, -1 if an error occurred but no exception was raised
     :rtype: int
     """
     status, output = self.memuc_run(["create", vm_version])
     success = status == 0 and output is not None and "SUCCESS" in output
```

### Comparing `pymemuc-0.3.0/pymemuc/_memuc.py` & `pymemuc-0.3.1/pymemuc/_memuc.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.0/pymemuc/exceptions.py` & `pymemuc-0.3.1/pymemuc/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.0/pymemuc/pymemuc.py` & `pymemuc-0.3.1/pymemuc/pymemuc.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.0/pyproject.toml` & `pymemuc-0.3.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pymemuc"
-version = "v0.3.0"
+version = "v0.3.1"
 description = "A Memuc.exe wrapper for Python"
 readme = "README.md"
 authors = ["Martin Miglio <code@martinmiglio.dev>"]
 license = "MIT"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pymemuc-0.3.0/PKG-INFO` & `pymemuc-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymemuc
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Memuc.exe wrapper for Python
 Home-page: https://github.com/martinmiglio/pymemuc
 License: MIT
 Keywords: memu,memuc,wrapper,api
 Author: Martin Miglio
 Author-email: code@martinmiglio.dev
 Requires-Python: >=3.9,<4.0
```

