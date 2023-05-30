# Comparing `tmp/hkkang_utils-0.1.93.tar.gz` & `tmp/hkkang_utils-0.1.94.tar.gz`

## Comparing `hkkang_utils-0.1.93.tar` & `hkkang_utils-0.1.94.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/.github/workflows/deploy_doc.yml
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/.github/workflows/unittest.yml
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/.vscode/settings.json
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/docs/make.bat
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/docs/source/conf.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/docs/source/index.rst
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/__init__.py
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/concurrent.py
--rw-r--r--   0        0        0     6525 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/file.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/io.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/list.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/logger.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/metrics.py
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/misc.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/ml.py
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/pattern.py
--rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/pg.py
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/slack.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/socket.py
--rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/sql.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/string.py
--rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/tensor.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/testing.py
--rw-r--r--   0        0        0     7607 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/src/hkkang_utils/time.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/tests/__init__.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/tests/test_concurrent.py
--rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/tests/test_file.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/tests/test_io.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/tests/test_list.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/tests/test_metrics.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/tests/test_misc.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/tests/test_pattern.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/tests/test_sql.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/tests/test_string.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/tests/test_tensor.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/tests/test_testing.py
--rw-r--r--   0        0        0     5755 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/tests/test_time.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/LICENSE
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/README.md
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/pyproject.toml
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 hkkang_utils-0.1.93/PKG-INFO
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/.github/workflows/deploy_doc.yml
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/.github/workflows/unittest.yml
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/.vscode/settings.json
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/docs/make.bat
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/docs/source/conf.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/docs/source/index.rst
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/__init__.py
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/concurrent.py
+-rw-r--r--   0        0        0     6525 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/file.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/io.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/list.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/logger.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/metrics.py
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/misc.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/ml.py
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/pattern.py
+-rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/pg.py
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/slack.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/socket.py
+-rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/sql.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/string.py
+-rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/tensor.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/testing.py
+-rw-r--r--   0        0        0     8099 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/src/hkkang_utils/time.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/tests/__init__.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/tests/test_concurrent.py
+-rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/tests/test_file.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/tests/test_io.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/tests/test_list.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/tests/test_metrics.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/tests/test_misc.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/tests/test_pattern.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/tests/test_sql.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/tests/test_string.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/tests/test_tensor.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/tests/test_testing.py
+-rw-r--r--   0        0        0     6337 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/tests/test_time.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/LICENSE
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/README.md
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/pyproject.toml
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 hkkang_utils-0.1.94/PKG-INFO
```

### Comparing `hkkang_utils-0.1.93/.github/workflows/deploy_doc.yml` & `hkkang_utils-0.1.94/.github/workflows/deploy_doc.yml`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.93/.github/workflows/unittest.yml` & `hkkang_utils-0.1.94/.github/workflows/unittest.yml`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.93/docs/Makefile` & `hkkang_utils-0.1.94/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.93/docs/make.bat` & `hkkang_utils-0.1.94/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.93/docs/source/conf.py` & `hkkang_utils-0.1.94/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.93/src/hkkang_utils/__init__.py` & `hkkang_utils-0.1.94/src/hkkang_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.93/src/hkkang_utils/concurrent.py` & `hkkang_utils-0.1.94/src/hkkang_utils/concurrent.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.93/src/hkkang_utils/file.py` & `hkkang_utils-0.1.94/src/hkkang_utils/file.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.93/src/hkkang_utils/list.py` & `hkkang_utils-0.1.94/src/hkkang_utils/list.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.93/src/hkkang_utils/metrics.py` & `hkkang_utils-0.1.94/src/hkkang_utils/metrics.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.93/src/hkkang_utils/misc.py` & `hkkang_utils-0.1.94/src/hkkang_utils/misc.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.93/src/hkkang_utils/ml.py` & `hkkang_utils-0.1.94/src/hkkang_utils/ml.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.93/src/hkkang_utils/pattern.py` & `hkkang_utils-0.1.94/src/hkkang_utils/pattern.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.93/src/hkkang_utils/pg.py` & `hkkang_utils-0.1.94/src/hkkang_utils/pg.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.93/src/hkkang_utils/slack.py` & `hkkang_utils-0.1.94/src/hkkang_utils/slack.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.93/src/hkkang_utils/sql.py` & `hkkang_utils-0.1.94/src/hkkang_utils/sql.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.93/src/hkkang_utils/string.py` & `hkkang_utils-0.1.94/src/hkkang_utils/string.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.93/src/hkkang_utils/tensor.py` & `hkkang_utils-0.1.94/src/hkkang_utils/tensor.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.93/src/hkkang_utils/time.py` & `hkkang_utils-0.1.94/src/hkkang_utils/time.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 import inspect
 import logging
+import sys
 import time as time_module
 from contextlib import contextmanager
 from typing import Callable, Dict, List, Optional, Tuple
 
-import attrs
-
 from hkkang_utils.pattern import SingletonABCMetaWithArgs
 
+# Import dataclasses according to Python version
+sys_version = sys.version_info
+if sys_version[0] == 3 and sys_version[1] >= 7:
+    import dataclasses
+else:
+    try:
+        import dataclasses
+    except:
+        import subprocess
+
+        subprocess.check_call([sys.executable, "-m", "pip", "install", "dataclasses"])
+    finally:
+        import dataclasses
+
 
-@attrs.define
+@dataclasses.dataclass
 class Period:
     start_time: float
     end_time: float
 
     @property
     def elapsed_time(self) -> float:
         return self.end_time - self.start_time
@@ -179,22 +192,23 @@
 
     def show_total_elapsed_time(self) -> None:
         self.logger.info(f"Total elapsed time: {self.total_elapsed_time:.2f} seconds")
 
     def show_avg_elapsed_time(self) -> None:
         self.logger.info(f"Average elapsed time: {self.avg_elapsed_time:.2f} seconds")
 
-    def summarize_measured_time(self) -> Tuple[str, int, float]:
+    def summarize_measured_time(self) -> Tuple[str, int, float, float]:
         self.logger.info(f"Function name: {self.name}")
         self.logger.info(f"Call count: {self.call_cnt}")
         self.logger.info(f"Average elapsed time: {self.avg_elapsed_time:.2f} seconds")
-        return self.name, self.call_cnt, self.avg_elapsed_time
+        self.logger.info(f"Total elapsed time: {self.total_elapsed_time:.2f} seconds")
+        return self.name, self.call_cnt, self.avg_elapsed_time, self.total_elapsed_time
 
     @classmethod
-    def summarize_measured_times(cls) -> List[Tuple[str, int, float]]:
+    def summarize_measured_times(cls) -> List[Tuple[str, int, float, float]]:
         return_values = []
         for timer in Timer._instances[cls].values():
             return_values.append(timer.summarize_measured_time())
         return return_values
 
 
 def measure_time(func: Callable, print_measured_time: bool = True) -> Callable:
```

### Comparing `hkkang_utils-0.1.93/tests/test_concurrent.py` & `hkkang_utils-0.1.94/tests/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.93/tests/test_file.py` & `hkkang_utils-0.1.94/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.93/tests/test_io.py` & `hkkang_utils-0.1.94/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.93/tests/test_list.py` & `hkkang_utils-0.1.94/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.93/tests/test_metrics.py` & `hkkang_utils-0.1.94/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.93/tests/test_misc.py` & `hkkang_utils-0.1.94/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.93/tests/test_pattern.py` & `hkkang_utils-0.1.94/tests/test_pattern.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.93/tests/test_string.py` & `hkkang_utils-0.1.94/tests/test_string.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.93/tests/test_testing.py` & `hkkang_utils-0.1.94/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.93/tests/test_time.py` & `hkkang_utils-0.1.94/tests/test_time.py`

 * *Files 3% similar despite different names*

```diff
@@ -109,40 +109,50 @@
     @classmethod
     def setUpClass(cls):
         timer1 = time_utils.Timer(func_name="test_timer_summary1")
         timer2 = time_utils.Timer(func_name="test_timer_summary2")
         # Measure time
         with timer1.measure():
             time_module.sleep(TEST_TIME)
+        with timer1.measure():
+            time_module.sleep(TEST_TIME)
+        with timer2.measure():
+            time_module.sleep(TEST_TIME)
         with timer2.measure():
             time_module.sleep(TEST_TIME)
 
     def test_timer_summary_for_single_instance(self):
         timer = time_utils.Timer(func_name="test_timer_summary1")
         # Get statistics
-        fname, call_cnt, avg_time = timer.summarize_measured_time()
+        fname, call_cnt, avg_time, total_time = timer.summarize_measured_time()
         # Check
         self.assertEqual(fname, "test_timer_summary1")
-        self.assertEqual(call_cnt, 1)
+        self.assertEqual(call_cnt, 2)
         self.assertGreater(avg_time, TEST_TIME)
         self.assertLess(avg_time, TEST_TIME + 1)
+        self.assertGreater(total_time, TEST_TIME * 2)
+        self.assertLess(total_time, TEST_TIME * 2 + 1)
 
     def test_timer_summary_for_all_instances(self):
         infos: List[
-            Tuple[str, int, float]
+            Tuple[str, int, float, float]
         ] = time_utils.Timer.summarize_measured_times()
         fnames = list(map(lambda k: k[0], infos))
         self.assertGreaterEqual(len(infos), 2)
         self.assertIn("test_timer_summary1", fnames)
         test_timer_summary1_idx = fnames.index("test_timer_summary1")
-        self.assertEqual(infos[test_timer_summary1_idx][1], 1)
+        self.assertEqual(infos[test_timer_summary1_idx][1], 2)
         self.assertGreater(infos[test_timer_summary1_idx][2], TEST_TIME)
         self.assertLess(infos[test_timer_summary1_idx][2], TEST_TIME + 1)
+        self.assertGreater(infos[test_timer_summary1_idx][3], TEST_TIME * 2)
+        self.assertLess(infos[test_timer_summary1_idx][3], TEST_TIME * 2 + 1)
         self.assertIn("test_timer_summary2", fnames)
         test_timer_summary2_idx = fnames.index("test_timer_summary2")
-        self.assertEqual(infos[test_timer_summary2_idx][1], 1)
+        self.assertEqual(infos[test_timer_summary2_idx][1], 2)
         self.assertGreater(infos[test_timer_summary2_idx][2], TEST_TIME)
         self.assertLess(infos[test_timer_summary2_idx][2], TEST_TIME + 1)
+        self.assertGreater(infos[test_timer_summary2_idx][3], TEST_TIME * 2)
+        self.assertLess(infos[test_timer_summary2_idx][3], TEST_TIME * 2 + 1)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `hkkang_utils-0.1.93/.gitignore` & `hkkang_utils-0.1.94/.gitignore`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.93/LICENSE` & `hkkang_utils-0.1.94/LICENSE`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.93/pyproject.toml` & `hkkang_utils-0.1.94/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hkkang_utils"
-version = "0.1.93"
+version = "0.1.94"
 authors = [{name="Hyukkyu Kang", email="hyukkyukang@gmail.com"}]
 description = "A collection of useful util functions"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `hkkang_utils-0.1.93/PKG-INFO` & `hkkang_utils-0.1.94/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkkang_utils
-Version: 0.1.93
+Version: 0.1.94
 Summary: A collection of useful util functions
 Project-URL: Homepage, https://github.com/hyukkyukang/python_utils
 Project-URL: Bug Tracker, https://github.com/hyukkyukang/python_utils/issues
 Author-email: Hyukkyu Kang <hyukkyukang@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

