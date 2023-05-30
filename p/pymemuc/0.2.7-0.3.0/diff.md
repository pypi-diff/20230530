# Comparing `tmp/pymemuc-0.2.7.tar.gz` & `tmp/pymemuc-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymemuc-0.2.7.tar", max compression
+gzip compressed data, was "pymemuc-0.3.0.tar", max compression
```

## Comparing `pymemuc-0.2.7.tar` & `pymemuc-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1057 2023-05-26 04:32:01.749582 pymemuc-0.2.7/LICENSE
--rw-r--r--   0        0        0     1586 2023-05-26 04:32:01.749582 pymemuc-0.2.7/README.md
--rw-r--r--   0        0        0      386 2023-05-26 04:32:01.757582 pymemuc-0.2.7/pymemuc/__init__.py
--rw-r--r--   0        0        0    22761 2023-05-26 04:32:01.757582 pymemuc-0.2.7/pymemuc/_command.py
--rw-r--r--   0        0        0      465 2023-05-26 04:32:01.757582 pymemuc-0.2.7/pymemuc/_constants.py
--rw-r--r--   0        0        0     4984 2023-05-26 04:32:01.757582 pymemuc-0.2.7/pymemuc/_control.py
--rw-r--r--   0        0        0     1150 2023-05-26 04:32:01.757582 pymemuc-0.2.7/pymemuc/_decorators.py
--rw-r--r--   0        0        0    13670 2023-05-26 04:32:01.757582 pymemuc-0.2.7/pymemuc/_manage.py
--rw-r--r--   0        0        0     3980 2023-05-26 04:32:01.757582 pymemuc-0.2.7/pymemuc/_memuc.py
--rw-r--r--   0        0        0      891 2023-05-26 04:32:01.757582 pymemuc-0.2.7/pymemuc/exceptions.py
--rw-r--r--   0        0        0     2216 2023-05-26 04:32:01.757582 pymemuc-0.2.7/pymemuc/pymemuc.py
--rw-r--r--   0        0        0      379 2023-05-26 04:32:01.757582 pymemuc-0.2.7/pymemuc/vminfo.py
--rw-r--r--   0        0        0     1665 2023-05-26 04:32:28.577600 pymemuc-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     2394 1970-01-01 00:00:00.000000 pymemuc-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-05-30 03:10:01.561799 pymemuc-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1586 2023-05-30 03:10:01.561799 pymemuc-0.3.0/README.md
+-rw-r--r--   0        0        0      386 2023-05-30 03:10:01.569799 pymemuc-0.3.0/pymemuc/__init__.py
+-rw-r--r--   0        0        0    22761 2023-05-30 03:10:01.569799 pymemuc-0.3.0/pymemuc/_command.py
+-rw-r--r--   0        0        0      465 2023-05-30 03:10:01.569799 pymemuc-0.3.0/pymemuc/_constants.py
+-rw-r--r--   0        0        0     4984 2023-05-30 03:10:01.569799 pymemuc-0.3.0/pymemuc/_control.py
+-rw-r--r--   0        0        0     1214 2023-05-30 03:10:01.569799 pymemuc-0.3.0/pymemuc/_decorators.py
+-rw-r--r--   0        0        0    13670 2023-05-30 03:10:01.569799 pymemuc-0.3.0/pymemuc/_manage.py
+-rw-r--r--   0        0        0     3958 2023-05-30 03:10:01.569799 pymemuc-0.3.0/pymemuc/_memuc.py
+-rw-r--r--   0        0        0      891 2023-05-30 03:10:01.569799 pymemuc-0.3.0/pymemuc/exceptions.py
+-rw-r--r--   0        0        0     2899 2023-05-30 03:10:01.569799 pymemuc-0.3.0/pymemuc/pymemuc.py
+-rw-r--r--   0        0        0      379 2023-05-30 03:10:01.569799 pymemuc-0.3.0/pymemuc/vminfo.py
+-rw-r--r--   0        0        0     1665 2023-05-30 03:10:24.335042 pymemuc-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2394 1970-01-01 00:00:00.000000 pymemuc-0.3.0/PKG-INFO
```

### Comparing `pymemuc-0.2.7/LICENSE` & `pymemuc-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymemuc-0.2.7/README.md` & `pymemuc-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pymemuc-0.2.7/pymemuc/_command.py` & `pymemuc-0.3.0/pymemuc/_command.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.2.7/pymemuc/_control.py` & `pymemuc-0.3.0/pymemuc/_control.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.2.7/pymemuc/_decorators.py` & `pymemuc-0.3.0/pymemuc/_decorators.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 """This module contains decorators for functions in pymemuc."""
 
 from functools import wraps
+from typing import TYPE_CHECKING
 
 from ._constants import RETRIES
 from .exceptions import PyMemucError, PyMemucTimeoutExpired
 
+if TYPE_CHECKING:
+    from pymemuc import PyMemuc
+
 
 def _retryable(func):
     """Decorator to retry a function if it raises an exception.
     The number of retries is defined in pymemuc._constants.RETRIES
     After the last retry, the exception is raised.
     """
 
     @wraps(func)
-    def wrapper(self, *args, **kwargs):
+    def wrapper(self: "PyMemuc", *args, **kwargs):
         fin_err = None  # track the last error
         for i in range(RETRIES):
             try:
                 return func(self, *args, **kwargs)
             except (PyMemucError, PyMemucTimeoutExpired) as err:
                 fin_err = err  # update the last error
-                if self.debug:
-                    print(f"pymemuc._decorators._retryable: {err}")
-                    r_left = RETRIES - i - 1
-                    if r_left > 0:
-                        print(
-                            f"\tretrying {r_left} more time{'s' if r_left > 1 else ''}..."
-                        )
+                self.logger.debug(f"pymemuc._decorators._retryable: {err}")
+                r_left = RETRIES - i - 1
+                if r_left > 0:
+                    self.logger.debug(
+                        f"\tretrying {r_left} more time{'s' if r_left > 1 else ''}..."
+                    )
         raise PyMemucError(f"Max retries ({RETRIES}) exceeded") from fin_err
 
     return wrapper
```

### Comparing `pymemuc-0.2.7/pymemuc/_manage.py` & `pymemuc-0.3.0/pymemuc/_manage.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.2.7/pymemuc/_memuc.py` & `pymemuc-0.3.0/pymemuc/_memuc.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,17 +65,16 @@
     """
     # sourcery skip: extract-method
     args.insert(0, self.memuc_path)
     if timeout is not None and non_blocking:
         raise PyMemucException("Cannot use timeout and non_blocking at the same time")
     if non_blocking:
         args += "-t"
-    if self.debug:
-        print("pymemuc._memuc.memuc_run:")
-        print(f"\tCommand: \"{' '.join(args)}\"")
+    self.logger.debug("pymemuc._memuc.memuc_run:")
+    self.logger.debug(f"\tCommand: \"{' '.join(args)}\"")
     try:
         with Popen(
             args,
             shell=False,
             stdout=PIPE,
             stderr=STDOUT,
             close_fds=True,
@@ -83,19 +82,18 @@
         ) as process:
             try:
                 result, _ = process.communicate(timeout=timeout)
             except TimeoutExpired as err:
                 process.kill()
                 result, _ = process.communicate()
                 raise PyMemucTimeoutExpired(err) from err
-            if self.debug:
-                if lines := result.splitlines():
-                    print(f"\tOutput: {lines.pop(0)}")
-                    for line in lines:
-                        print(f"\t\t{line}")
+            if lines := result.splitlines():
+                self.logger.debug(f"\tOutput: {lines.pop(0)}")
+                for line in lines:
+                    self.logger.debug(f"\t\t{line}")
             return (0, result)
     except CalledProcessError as err:
         raise PyMemucError(err) from err
 
 
 # TODO: add output parsing
 def check_task_status(self: "PyMemuc", task_id: str) -> Tuple[int, str]:
```

### Comparing `pymemuc-0.2.7/pymemuc/exceptions.py` & `pymemuc-0.3.0/pymemuc/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.2.7/pymemuc/pymemuc.py` & `pymemuc-0.3.0/pymemuc/pymemuc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """a wrapper for memuc.exe as a library to control virual machines"""
 
+import logging
 from os.path import join
 from typing import Union
 
 from ._constants import WINREG_EN
 from .exceptions import PyMemucError
 
 
@@ -56,17 +57,36 @@
     )
     from ._memuc import _get_memu_top_level, check_task_status, memuc_run
 
     def __init__(self, memuc_path: Union[str, None] = None, debug=False) -> None:
         """initialize the class, automatically finding memuc.exe if windows registry is supported,
         otherwise a path must be specified"""
         self.debug = debug
-        if self.debug:
-            print("PyMemuc: Debug mode enabled")
+        self.logger = self._configure_logger()
+        self.logger.debug("PyMemuc: Debug mode enabled")
         if WINREG_EN:
             self.memuc_path: str = join(self._get_memu_top_level(), "memuc.exe")
         elif memuc_path is not None:
             self.memuc_path: str = memuc_path
         else:
             raise PyMemucError(
-                "Windows Registry is not supported on this platform, you must specify the path to memuc.exe manually"
+                "Windows Registry is not supported on this platform,"
+                + " you must specify the path to memuc.exe manually"
             )
+
+    def _configure_logger(self):
+        """Configure the logger for the class"""
+        logger = logging.getLogger(__name__)
+        logger.setLevel(logging.DEBUG if self.debug else logging.INFO)
+
+        # Create a handler for console output
+        console_handler = logging.StreamHandler()
+        console_handler.setLevel(logging.DEBUG)
+        formatter = logging.Formatter(
+            "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
+        )
+        console_handler.setFormatter(formatter)
+
+        # Add the handler to the logger
+        logger.addHandler(console_handler)
+
+        return logger
```

### Comparing `pymemuc-0.2.7/pyproject.toml` & `pymemuc-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pymemuc"
-version = "v0.2.7"
+version = "v0.3.0"
 description = "A Memuc.exe wrapper for Python"
 readme = "README.md"
 authors = ["Martin Miglio <code@martinmiglio.dev>"]
 license = "MIT"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pymemuc-0.2.7/PKG-INFO` & `pymemuc-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymemuc
-Version: 0.2.7
+Version: 0.3.0
 Summary: A Memuc.exe wrapper for Python
 Home-page: https://github.com/martinmiglio/pymemuc
 License: MIT
 Keywords: memu,memuc,wrapper,api
 Author: Martin Miglio
 Author-email: code@martinmiglio.dev
 Requires-Python: >=3.9,<4.0
```

