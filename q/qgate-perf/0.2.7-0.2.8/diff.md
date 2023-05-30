# Comparing `tmp/qgate_perf-0.2.7-py3-none-any.whl.zip` & `tmp/qgate_perf-0.2.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 17267 bytes, number of entries: 17
+Zip file size: 17312 bytes, number of entries: 17
 -rw-rw-rw-  2.0 fat       40 b- defN 23-Apr-29 09:53 qgate_perf/__init__.py
 -rw-rw-rw-  2.0 fat      428 b- defN 23-May-06 06:01 qgate_perf/bundle_helper.py
 -rw-rw-rw-  2.0 fat     5714 b- defN 23-May-06 17:21 qgate_perf/executor_helper.py
 -rw-rw-rw-  2.0 fat     1053 b- defN 23-May-04 18:36 qgate_perf/file_format.py
--rw-rw-rw-  2.0 fat    13102 b- defN 23-May-30 15:05 qgate_perf/parallel_executor.py
+-rw-rw-rw-  2.0 fat    13562 b- defN 23-May-30 17:30 qgate_perf/parallel_executor.py
 -rw-rw-rw-  2.0 fat     5431 b- defN 23-May-06 11:59 qgate_perf/parallel_probe.py
 -rw-rw-rw-  2.0 fat      384 b- defN 23-May-06 12:01 qgate_perf/run_return.py
--rw-rw-rw-  2.0 fat     1822 b- defN 23-May-30 15:22 qgate_perf/run_setup.py
--rw-rw-rw-  2.0 fat      215 b- defN 23-May-30 15:22 qgate_perf/version.py
+-rw-rw-rw-  2.0 fat     1824 b- defN 23-May-30 17:30 qgate_perf/run_setup.py
+-rw-rw-rw-  2.0 fat      215 b- defN 23-May-30 17:39 qgate_perf/version.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-05 17:45 tests/__init__.py
 -rw-rw-rw-  2.0 fat      731 b- defN 23-May-26 14:21 tests/test_dir.py
 -rw-rw-rw-  2.0 fat     4587 b- defN 23-May-26 18:34 tests/test_run.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-May-30 15:24 qgate_perf-0.2.7.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6964 b- defN 23-May-30 15:24 qgate_perf-0.2.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 15:24 qgate_perf-0.2.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-May-30 15:24 qgate_perf-0.2.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1359 b- defN 23-May-30 15:24 qgate_perf-0.2.7.dist-info/RECORD
-17 files, 53497 bytes uncompressed, 15043 bytes compressed:  71.9%
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-May-30 17:40 qgate_perf-0.2.8.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6964 b- defN 23-May-30 17:40 qgate_perf-0.2.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-30 17:40 qgate_perf-0.2.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-May-30 17:40 qgate_perf-0.2.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1359 b- defN 23-May-30 17:40 qgate_perf-0.2.8.dist-info/RECORD
+17 files, 53959 bytes uncompressed, 15088 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: tests/test_dir.py
 Comment: 
 
 Filename: tests/test_run.py
 Comment: 
 
-Filename: qgate_perf-0.2.7.dist-info/LICENSE
+Filename: qgate_perf-0.2.8.dist-info/LICENSE
 Comment: 
 
-Filename: qgate_perf-0.2.7.dist-info/METADATA
+Filename: qgate_perf-0.2.8.dist-info/METADATA
 Comment: 
 
-Filename: qgate_perf-0.2.7.dist-info/WHEEL
+Filename: qgate_perf-0.2.8.dist-info/WHEEL
 Comment: 
 
-Filename: qgate_perf-0.2.7.dist-info/top_level.txt
+Filename: qgate_perf-0.2.8.dist-info/top_level.txt
 Comment: 
 
-Filename: qgate_perf-0.2.7.dist-info/RECORD
+Filename: qgate_perf-0.2.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qgate_perf/parallel_executor.py

```diff
@@ -277,26 +277,32 @@
             run_setup = RunSetup(duration_second=0, start_delay=0, parameters=parameters)
 
         # run
         self.run(processes=1,
                  threads=1,
                  run_setup=run_setup)
 
-    def init_run(self, parameters=None, print_output=False):
+    def init_run(self, run_setup: RunSetup=None, parameters=None, print_output=False):
         """ Init call in current process/thread (without ability to define parallel execution and without
          write standard outputs to file). One new parametr was added '__INIT__': True
 
         :param parameters:      parameters for execution, application in case the run_setup is None
         :return:                return output from execution
         """
 
-        test_parameters = parameters.copy() if parameters else {}
-        test_parameters["__INIT__"] = True
-
-        return self.test_run(None, test_parameters, print_output)
+        if run_setup:
+            test_parameters = run_setup._parameters.copy() if run_setup._parameters else {}
+            test_parameters["__INIT__"] = True
+            test_run_setup=RunSetup(duration_second=0, start_delay=0,parameters=test_parameters)
+            test_run_setup.set_bulk(run_setup.bulk_row, run_setup.bulk_col)
+            return self.test_run(test_run_setup, None, print_output)
+        else:
+            test_parameters = parameters.copy() if parameters else {}
+            test_parameters["__INIT__"] = True
+            return self.test_run(None, test_parameters, print_output)
 
     def test_run(self, run_setup: RunSetup=None, parameters=None, print_output=False):
         """ Test call in current process/thread (without ability to define parallel execution and without
          write standard outputs to file)
 
         :param run_setup:       setting for run
         :param parameters:      parameters for execution, application in case the run_setup is None
```

## qgate_perf/run_setup.py

```diff
@@ -17,14 +17,15 @@
 
         # collection of specific keys for project such as project_name, feature_set_name, etc.
         self._parameters=parameters
 
     @property
     def bulk_row(self):
         return self._bulk_row
+
     @property
     def bulk_col(self):
         return self._bulk_col
 
     @property
     def when_start(self):
         return self._when_start
```

## qgate_perf/version.py

```diff
@@ -1,5 +1,5 @@
 # Store the version here so:
 # 1) we don't load dependencies by storing it in __init__.py
 # 2) we can import it in setup.py for the same reason
 # 3) we can import it into your module module
-__version__ = '0.2.7'
+__version__ = '0.2.8'
```

## Comparing `qgate_perf-0.2.7.dist-info/LICENSE` & `qgate_perf-0.2.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `qgate_perf-0.2.7.dist-info/METADATA` & `qgate_perf-0.2.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qgate-perf
-Version: 0.2.7
+Version: 0.2.8
 Summary: Performance test generator, part of Quality Gate
 Home-page: https://github.com/george0st/qgate-perf/
 Download-URL: https://pypi.org/project/qgate_perf/
 Author: Jiri Steuer
 Author-email: steuer.jiri@gmail.com
 License: MIT
 Keywords: PerformanceTest,Performance,QualityGate
```

## Comparing `qgate_perf-0.2.7.dist-info/RECORD` & `qgate_perf-0.2.8.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 qgate_perf/__init__.py,sha256=1_WzwjEn3Ro-VrDe9uO1r2TbTq6YPSaErStlN5aF3_4,40
 qgate_perf/bundle_helper.py,sha256=utcDeo0unCzru68FJnl5tRBjumv56dNEg6Kdc6SHGkg,428
 qgate_perf/executor_helper.py,sha256=kGCih4ZnCgdzYcTXuhAUbPt-_hHyMzE5f7OzB6L4HVQ,5714
 qgate_perf/file_format.py,sha256=D8j13sUIXkhe0vZDVAuvEoRJEvf3RXzrTzymTIbkYWw,1053
-qgate_perf/parallel_executor.py,sha256=Kx9rANvHKtnXsPFhshzQPKZVspO2C6fkjiBmNR60-BU,13102
+qgate_perf/parallel_executor.py,sha256=eCjSAFwP_SkXZ8LbSW4qW2hrYrPo77168kDW1mFhO10,13562
 qgate_perf/parallel_probe.py,sha256=FatAtL9aeFby4JtVEfvHfl2YH6AyP2uNrsCUhvRiukY,5431
 qgate_perf/run_return.py,sha256=3hFZ5cH47R1nq7_13JG2WLhwdipBCao-qDtdfeuoXx4,384
-qgate_perf/run_setup.py,sha256=kMvgTeo89fnzV0suHEYNwztkqGArACmwWUYdDEuXzyI,1822
-qgate_perf/version.py,sha256=xNzZr5XhfOlgGXNzTc4746uqMz4sgoir0urlMhrjMbg,215
+qgate_perf/run_setup.py,sha256=hCpvZak-7VEyuDRgh_IqJx6VYcUDqTkXi1a27V8ddsI,1824
+qgate_perf/version.py,sha256=bBIENHlouRrMMv0LXT_sGmoD7UWHaQVBi8MmaJRsq6c,215
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_dir.py,sha256=NFNu4S6gZhJ7F_wuiYfl_pAXlgx8bUbwNr6UYMKG7e8,731
 tests/test_run.py,sha256=TZzHiy02r0reYxB2bfoEKsDmtwAEBBXy9ZUy2UCK_9g,4587
-qgate_perf-0.2.7.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
-qgate_perf-0.2.7.dist-info/METADATA,sha256=WU3O0Ei0_JNpJZEhHQ7YO_RFp1rGAN2kmieevABbVYw,6964
-qgate_perf-0.2.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-qgate_perf-0.2.7.dist-info/top_level.txt,sha256=z6ZySajXAxnXAu93K07L8dyGjn_qiYpr8FppLP0r4Rk,17
-qgate_perf-0.2.7.dist-info/RECORD,,
+qgate_perf-0.2.8.dist-info/LICENSE,sha256=HrhfyXIkWY2tGFK11kg7vPCqhgh5DcxleloqdhrpyMY,11558
+qgate_perf-0.2.8.dist-info/METADATA,sha256=9sBabIE1qd92hvKP6770-fp4TP832SsMw49lfoIahOs,6964
+qgate_perf-0.2.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+qgate_perf-0.2.8.dist-info/top_level.txt,sha256=z6ZySajXAxnXAu93K07L8dyGjn_qiYpr8FppLP0r4Rk,17
+qgate_perf-0.2.8.dist-info/RECORD,,
```

