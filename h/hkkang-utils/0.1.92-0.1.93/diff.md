# Comparing `tmp/hkkang_utils-0.1.92.tar.gz` & `tmp/hkkang_utils-0.1.93.tar.gz`

## Comparing `hkkang_utils-0.1.92.tar` & `hkkang_utils-0.1.93.tar`

### file list

```diff
@@ -1,39 +1,43 @@
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/.github/workflows/deploy_doc.yml
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/.github/workflows/unittest.yml
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/.vscode/settings.json
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/__init__.py
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/concurrent.py
--rw-r--r--   0        0        0     6525 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/file.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/io.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/list.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/logger.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/metrics.py
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/misc.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/ml.py
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/pattern.py
--rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/pg.py
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/slack.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/socket.py
--rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/sql.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/string.py
--rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/tensor.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/testing.py
--rw-r--r--   0        0        0     6913 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/time.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/tests/__init__.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/tests/test_concurrent.py
--rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/tests/test_file.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/tests/test_io.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/tests/test_list.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/tests/test_metrics.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/tests/test_misc.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/tests/test_pattern.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/tests/test_sql.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/tests/test_string.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/tests/test_tensor.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/tests/test_testing.py
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/tests/test_time.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/LICENSE
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/README.md
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/pyproject.toml
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/PKG-INFO
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/.github/workflows/deploy_doc.yml
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/.github/workflows/unittest.yml
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/.vscode/settings.json
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/docs/make.bat
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/docs/source/conf.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/docs/source/index.rst
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/__init__.py
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/concurrent.py
+-rw-r--r--   0        0        0     6525 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/file.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/io.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/list.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/logger.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/metrics.py
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/misc.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/ml.py
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/pattern.py
+-rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/pg.py
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/slack.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/socket.py
+-rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/sql.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/string.py
+-rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/tensor.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/testing.py
+-rw-r--r--   0        0        0     7607 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/time.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/tests/__init__.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/tests/test_concurrent.py
+-rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/tests/test_file.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/tests/test_io.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/tests/test_list.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/tests/test_metrics.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/tests/test_misc.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/tests/test_pattern.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/tests/test_sql.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/tests/test_string.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/tests/test_tensor.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/tests/test_testing.py
+-rw-r--r--   0        0        0     5755 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/tests/test_time.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/LICENSE
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/README.md
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/pyproject.toml
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/PKG-INFO
```

### Comparing `hkkang_utils-0.1.92/.github/workflows/deploy_doc.yml` & `hkkang_utils-0.1.93/.github/workflows/deploy_doc.yml`

 * *Files 13% similar despite different names*

```diff
@@ -34,15 +34,15 @@
                   python-version: "3.11"
                   cache: "pip" # caching pip dependencies
 
             - name: Install dependecy
               working-directory: ${{ env.working-directory }}
               run: |
                   python -m pip install --upgrade pip
-                  pip install sphinx
+                  pip install sphinx sphinx-rtd-theme
 
             - name: build sphinx
               run: |
                   cd docs 
                   sphinx-apidoc -o ./source ../src
                   make html
```

### Comparing `hkkang_utils-0.1.92/.github/workflows/unittest.yml` & `hkkang_utils-0.1.93/.github/workflows/unittest.yml`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.92/src/hkkang_utils/__init__.py` & `hkkang_utils-0.1.93/src/hkkang_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.92/src/hkkang_utils/concurrent.py` & `hkkang_utils-0.1.93/src/hkkang_utils/concurrent.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.92/src/hkkang_utils/file.py` & `hkkang_utils-0.1.93/src/hkkang_utils/file.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.92/src/hkkang_utils/list.py` & `hkkang_utils-0.1.93/src/hkkang_utils/list.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.92/src/hkkang_utils/metrics.py` & `hkkang_utils-0.1.93/src/hkkang_utils/metrics.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.92/src/hkkang_utils/misc.py` & `hkkang_utils-0.1.93/src/hkkang_utils/misc.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.92/src/hkkang_utils/ml.py` & `hkkang_utils-0.1.93/src/hkkang_utils/ml.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.92/src/hkkang_utils/pattern.py` & `hkkang_utils-0.1.93/src/hkkang_utils/pattern.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.92/src/hkkang_utils/pg.py` & `hkkang_utils-0.1.93/src/hkkang_utils/pg.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.92/src/hkkang_utils/slack.py` & `hkkang_utils-0.1.93/src/hkkang_utils/slack.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.92/src/hkkang_utils/sql.py` & `hkkang_utils-0.1.93/src/hkkang_utils/sql.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.92/src/hkkang_utils/string.py` & `hkkang_utils-0.1.93/src/hkkang_utils/string.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.92/src/hkkang_utils/tensor.py` & `hkkang_utils-0.1.93/src/hkkang_utils/tensor.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.92/src/hkkang_utils/time.py` & `hkkang_utils-0.1.93/src/hkkang_utils/time.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import inspect
 import logging
 import time as time_module
 from contextlib import contextmanager
-from typing import Callable, Dict, List, Optional
+from typing import Callable, Dict, List, Optional, Tuple
 
 import attrs
 
 from hkkang_utils.pattern import SingletonABCMetaWithArgs
 
 
 @attrs.define
@@ -96,14 +96,16 @@
         # Time related variables
         self.start_time: Optional[float] = None
         self.measured_times: List[Period] = []
         self.paused_times: List[Period] = []
 
     @property
     def name(self) -> str:
+        if self.class_name is None:
+            return self.func_name
         return f"{self.class_name}.{self.func_name}"
 
     @property
     def logger(self) -> logging.Logger:
         return logging.getLogger(f"Timer.{self.name}")
 
     @property
@@ -168,23 +170,36 @@
                 "Timer has not been started. Please call start() first."
             )
         self.measured_times.append(Period(self.start_time, current_time))
         self.start_time = None
         return self.elapsed_time
 
     # Methods for printing the measured time
-    def show_elapsed_time(self):
+    def show_elapsed_time(self) -> None:
         self.logger.info(f"Elapsed time: {self.elapsed_time:.2f} seconds")
 
-    def show_total_elapsed_time(self):
+    def show_total_elapsed_time(self) -> None:
         self.logger.info(f"Total elapsed time: {self.total_elapsed_time:.2f} seconds")
 
-    def show_avg_elapsed_time(self):
+    def show_avg_elapsed_time(self) -> None:
         self.logger.info(f"Average elapsed time: {self.avg_elapsed_time:.2f} seconds")
 
+    def summarize_measured_time(self) -> Tuple[str, int, float]:
+        self.logger.info(f"Function name: {self.name}")
+        self.logger.info(f"Call count: {self.call_cnt}")
+        self.logger.info(f"Average elapsed time: {self.avg_elapsed_time:.2f} seconds")
+        return self.name, self.call_cnt, self.avg_elapsed_time
+
+    @classmethod
+    def summarize_measured_times(cls) -> List[Tuple[str, int, float]]:
+        return_values = []
+        for timer in Timer._instances[cls].values():
+            return_values.append(timer.summarize_measured_time())
+        return return_values
+
 
 def measure_time(func: Callable, print_measured_time: bool = True) -> Callable:
     """Decorator to measure the elapsed time of a function.
 
     :param func: function to be measured
     :type func: Callable
     :param print_measured_time: whether to print the measured time after the function call, defaults to True
```

### Comparing `hkkang_utils-0.1.92/tests/test_concurrent.py` & `hkkang_utils-0.1.93/tests/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.92/tests/test_file.py` & `hkkang_utils-0.1.93/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.92/tests/test_io.py` & `hkkang_utils-0.1.93/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.92/tests/test_list.py` & `hkkang_utils-0.1.93/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.92/tests/test_metrics.py` & `hkkang_utils-0.1.93/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.92/tests/test_misc.py` & `hkkang_utils-0.1.93/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.92/tests/test_pattern.py` & `hkkang_utils-0.1.93/tests/test_pattern.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.92/tests/test_string.py` & `hkkang_utils-0.1.93/tests/test_string.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.92/tests/test_testing.py` & `hkkang_utils-0.1.93/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.92/.gitignore` & `hkkang_utils-0.1.93/.gitignore`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.92/LICENSE` & `hkkang_utils-0.1.93/LICENSE`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.92/pyproject.toml` & `hkkang_utils-0.1.93/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hkkang_utils"
-version = "0.1.92"
+version = "0.1.93"
 authors = [{name="Hyukkyu Kang", email="hyukkyukang@gmail.com"}]
 description = "A collection of useful util functions"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `hkkang_utils-0.1.92/PKG-INFO` & `hkkang_utils-0.1.93/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkkang_utils
-Version: 0.1.92
+Version: 0.1.93
 Summary: A collection of useful util functions
 Project-URL: Homepage, https://github.com/hyukkyukang/python_utils
 Project-URL: Bug Tracker, https://github.com/hyukkyukang/python_utils/issues
 Author-email: Hyukkyu Kang <hyukkyukang@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -29,7 +29,9 @@
 This is a collection of python functions that I use in my projects.
 
 To install [the package](https://pypi.org/project/hkkang-utils/):
 
 ```bash
 pip install hkkang_utils
 ```
+
+Documentation is available [here](https://hyukkyukang.github.io/python_utils/).
```

