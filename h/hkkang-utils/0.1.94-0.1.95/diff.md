# Comparing `tmp/hkkang_utils-0.1.94.tar.gz` & `tmp/hkkang_utils-0.1.95.tar.gz`

## Comparing `hkkang_utils-0.1.94.tar` & `hkkang_utils-0.1.95.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/.github/workflows/deploy_doc.yml
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/.github/workflows/unittest.yml
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/.vscode/settings.json
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/docs/make.bat
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/docs/source/conf.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/docs/source/index.rst
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/__init__.py
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/concurrent.py
--rw-r--r--   0        0        0     6525 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/file.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/io.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/list.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/logger.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/metrics.py
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/misc.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/ml.py
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/pattern.py
--rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/pg.py
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/slack.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/socket.py
--rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/sql.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/string.py
--rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/tensor.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/testing.py
--rw-r--r--   0        0        0     8099 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/time.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/tests/__init__.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/tests/test_concurrent.py
--rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/tests/test_file.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/tests/test_io.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/tests/test_list.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/tests/test_metrics.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/tests/test_misc.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/tests/test_pattern.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/tests/test_sql.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/tests/test_string.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/tests/test_tensor.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/tests/test_testing.py
--rw-r--r--   0        0        0     6337 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/tests/test_time.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/LICENSE
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/README.md
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/pyproject.toml
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/PKG-INFO
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/.github/workflows/deploy_doc.yml
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/.github/workflows/unittest.yml
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/.vscode/settings.json
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/docs/make.bat
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/docs/source/conf.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/docs/source/index.rst
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/src/hkkang_utils/__init__.py
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/src/hkkang_utils/concurrent.py
+-rw-r--r--   0        0        0     6525 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/src/hkkang_utils/file.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/src/hkkang_utils/io.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/src/hkkang_utils/list.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/src/hkkang_utils/logger.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/src/hkkang_utils/metrics.py
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/src/hkkang_utils/misc.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/src/hkkang_utils/ml.py
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/src/hkkang_utils/pattern.py
+-rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/src/hkkang_utils/pg.py
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/src/hkkang_utils/slack.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/src/hkkang_utils/socket.py
+-rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/src/hkkang_utils/sql.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/src/hkkang_utils/string.py
+-rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/src/hkkang_utils/tensor.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/src/hkkang_utils/testing.py
+-rw-r--r--   0        0        0     8453 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/src/hkkang_utils/time.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/tests/__init__.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/tests/test_concurrent.py
+-rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/tests/test_file.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/tests/test_io.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/tests/test_list.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/tests/test_metrics.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/tests/test_misc.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/tests/test_pattern.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/tests/test_sql.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/tests/test_string.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/tests/test_tensor.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/tests/test_testing.py
+-rw-r--r--   0        0        0     6337 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/tests/test_time.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/LICENSE
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/README.md
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/pyproject.toml
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 hkkang_utils-0.1.95/PKG-INFO
```

### Comparing `hkkang_utils-0.1.94/.github/workflows/deploy_doc.yml` & `hkkang_utils-0.1.95/.github/workflows/deploy_doc.yml`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.94/.github/workflows/unittest.yml` & `hkkang_utils-0.1.95/.github/workflows/unittest.yml`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.94/docs/Makefile` & `hkkang_utils-0.1.95/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.94/docs/make.bat` & `hkkang_utils-0.1.95/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.94/docs/source/conf.py` & `hkkang_utils-0.1.95/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.94/src/hkkang_utils/__init__.py` & `hkkang_utils-0.1.95/src/hkkang_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.94/src/hkkang_utils/concurrent.py` & `hkkang_utils-0.1.95/src/hkkang_utils/concurrent.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.94/src/hkkang_utils/file.py` & `hkkang_utils-0.1.95/src/hkkang_utils/file.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.94/src/hkkang_utils/list.py` & `hkkang_utils-0.1.95/src/hkkang_utils/list.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.94/src/hkkang_utils/metrics.py` & `hkkang_utils-0.1.95/src/hkkang_utils/metrics.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.94/src/hkkang_utils/misc.py` & `hkkang_utils-0.1.95/src/hkkang_utils/misc.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.94/src/hkkang_utils/ml.py` & `hkkang_utils-0.1.95/src/hkkang_utils/ml.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.94/src/hkkang_utils/pattern.py` & `hkkang_utils-0.1.95/src/hkkang_utils/pattern.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.94/src/hkkang_utils/pg.py` & `hkkang_utils-0.1.95/src/hkkang_utils/pg.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.94/src/hkkang_utils/slack.py` & `hkkang_utils-0.1.95/src/hkkang_utils/slack.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.94/src/hkkang_utils/sql.py` & `hkkang_utils-0.1.95/src/hkkang_utils/sql.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.94/src/hkkang_utils/string.py` & `hkkang_utils-0.1.95/src/hkkang_utils/string.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.94/src/hkkang_utils/tensor.py` & `hkkang_utils-0.1.95/src/hkkang_utils/tensor.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.94/src/hkkang_utils/time.py` & `hkkang_utils-0.1.95/src/hkkang_utils/time.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,24 +18,41 @@
         import subprocess
 
         subprocess.check_call([sys.executable, "-m", "pip", "install", "dataclasses"])
     finally:
         import dataclasses
 
 
+# Dataclass
 @dataclasses.dataclass
 class Period:
     start_time: float
     end_time: float
 
     @property
     def elapsed_time(self) -> float:
         return self.end_time - self.start_time
 
 
+# Utility functions
+def prettify_time(time_in_sec: float) -> str:
+    if time_in_sec < 60:
+        return f"{time_in_sec:.2f} seconds"
+    return f"{minute(time_in_sec):.0f}min {second(time_in_sec):.2f}sec"
+
+
+def minute(time_in_sec: float) -> float:
+    return time_in_sec / 60
+
+
+def second(time_in_sec: float) -> float:
+    return time_in_sec % 60
+
+
+# Timer class
 class TimerMeta(SingletonABCMetaWithArgs):
     _call_cnt: Dict[str, Dict[str, int]] = dict()
 
     def __call__(cls, class_name=None, func_name=None):
         # Figure out the class name and function name of the caller
         if class_name is None and func_name is None:
             stack = inspect.stack()
@@ -184,37 +201,42 @@
             )
         self.measured_times.append(Period(self.start_time, current_time))
         self.start_time = None
         return self.elapsed_time
 
     # Methods for printing the measured time
     def show_elapsed_time(self) -> None:
-        self.logger.info(f"Elapsed time: {self.elapsed_time:.2f} seconds")
+        self.logger.info(f"Elapsed time: {prettify_time(self.elapsed_time)}")
 
     def show_total_elapsed_time(self) -> None:
-        self.logger.info(f"Total elapsed time: {self.total_elapsed_time:.2f} seconds")
+        self.logger.info(
+            f"Total elapsed time: {prettify_time(self.total_elapsed_time)}"
+        )
 
     def show_avg_elapsed_time(self) -> None:
-        self.logger.info(f"Average elapsed time: {self.avg_elapsed_time:.2f} seconds")
+        self.logger.info(
+            f"Average elapsed time: {prettify_time(self.avg_elapsed_time)}"
+        )
 
     def summarize_measured_time(self) -> Tuple[str, int, float, float]:
         self.logger.info(f"Function name: {self.name}")
         self.logger.info(f"Call count: {self.call_cnt}")
-        self.logger.info(f"Average elapsed time: {self.avg_elapsed_time:.2f} seconds")
-        self.logger.info(f"Total elapsed time: {self.total_elapsed_time:.2f} seconds")
+        self.show_avg_elapsed_time()
+        self.show_total_elapsed_time()
         return self.name, self.call_cnt, self.avg_elapsed_time, self.total_elapsed_time
 
     @classmethod
     def summarize_measured_times(cls) -> List[Tuple[str, int, float, float]]:
         return_values = []
         for timer in Timer._instances[cls].values():
             return_values.append(timer.summarize_measured_time())
         return return_values
 
 
+# Decorator for timer
 def measure_time(func: Callable, print_measured_time: bool = True) -> Callable:
     """Decorator to measure the elapsed time of a function.
 
     :param func: function to be measured
     :type func: Callable
     :param print_measured_time: whether to print the measured time after the function call, defaults to True
     :type print_measured_time: bool, optional
```

### Comparing `hkkang_utils-0.1.94/tests/test_concurrent.py` & `hkkang_utils-0.1.95/tests/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.94/tests/test_file.py` & `hkkang_utils-0.1.95/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.94/tests/test_io.py` & `hkkang_utils-0.1.95/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.94/tests/test_list.py` & `hkkang_utils-0.1.95/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.94/tests/test_metrics.py` & `hkkang_utils-0.1.95/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.94/tests/test_misc.py` & `hkkang_utils-0.1.95/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.94/tests/test_pattern.py` & `hkkang_utils-0.1.95/tests/test_pattern.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.94/tests/test_string.py` & `hkkang_utils-0.1.95/tests/test_string.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.94/tests/test_testing.py` & `hkkang_utils-0.1.95/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.94/tests/test_time.py` & `hkkang_utils-0.1.95/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.94/.gitignore` & `hkkang_utils-0.1.95/.gitignore`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.94/LICENSE` & `hkkang_utils-0.1.95/LICENSE`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.94/pyproject.toml` & `hkkang_utils-0.1.95/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hkkang_utils"
-version = "0.1.94"
+version = "0.1.95"
 authors = [{name="Hyukkyu Kang", email="hyukkyukang@gmail.com"}]
 description = "A collection of useful util functions"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `hkkang_utils-0.1.94/PKG-INFO` & `hkkang_utils-0.1.95/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkkang_utils
-Version: 0.1.94
+Version: 0.1.95
 Summary: A collection of useful util functions
 Project-URL: Homepage, https://github.com/hyukkyukang/python_utils
 Project-URL: Bug Tracker, https://github.com/hyukkyukang/python_utils/issues
 Author-email: Hyukkyu Kang <hyukkyukang@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

