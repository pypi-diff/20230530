# Comparing `tmp/pytest-regex-0.1.0.tar.gz` & `tmp/pytest-regex-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-regex-0.1.0.tar", last modified: Tue May 23 17:39:51 2023, max compression
+gzip compressed data, was "pytest-regex-0.2.0.tar", last modified: Mon May 29 22:07:37 2023, max compression
```

## Comparing `pytest-regex-0.1.0.tar` & `pytest-regex-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 treddy   (28751) staff       (20)        0 2023-05-23 17:39:51.000734 pytest-regex-0.1.0/
--rw-r--r--   0 treddy   (28751) staff       (20)     1068 2023-05-07 20:24:50.000000 pytest-regex-0.1.0/LICENSE
--rw-r--r--   0 treddy   (28751) staff       (20)     3459 2023-05-23 17:39:51.000610 pytest-regex-0.1.0/PKG-INFO
--rw-r--r--   0 treddy   (28751) staff       (20)     2433 2023-05-22 23:33:19.000000 pytest-regex-0.1.0/README.md
--rw-r--r--   0 treddy   (28751) staff       (20)      323 2023-05-23 00:27:04.000000 pytest-regex-0.1.0/pyproject.toml
-drwxr-xr-x   0 treddy   (28751) staff       (20)        0 2023-05-23 17:39:51.000167 pytest-regex-0.1.0/pytest_regex.egg-info/
--rw-r--r--   0 treddy   (28751) staff       (20)     3459 2023-05-23 17:39:50.000000 pytest-regex-0.1.0/pytest_regex.egg-info/PKG-INFO
--rw-r--r--   0 treddy   (28751) staff       (20)      296 2023-05-23 17:39:50.000000 pytest-regex-0.1.0/pytest_regex.egg-info/SOURCES.txt
--rw-r--r--   0 treddy   (28751) staff       (20)        1 2023-05-23 17:39:50.000000 pytest-regex-0.1.0/pytest_regex.egg-info/dependency_links.txt
--rw-r--r--   0 treddy   (28751) staff       (20)       32 2023-05-23 17:39:50.000000 pytest-regex-0.1.0/pytest_regex.egg-info/entry_points.txt
--rw-r--r--   0 treddy   (28751) staff       (20)       14 2023-05-23 17:39:50.000000 pytest-regex-0.1.0/pytest_regex.egg-info/requires.txt
--rw-r--r--   0 treddy   (28751) staff       (20)       13 2023-05-23 17:39:50.000000 pytest-regex-0.1.0/pytest_regex.egg-info/top_level.txt
--rw-r--r--   0 treddy   (28751) staff       (20)      885 2023-05-20 19:04:32.000000 pytest-regex-0.1.0/pytest_regex.py
--rw-r--r--   0 treddy   (28751) staff       (20)       38 2023-05-23 17:39:51.000779 pytest-regex-0.1.0/setup.cfg
--rw-r--r--   0 treddy   (28751) staff       (20)     1369 2023-05-07 20:48:08.000000 pytest-regex-0.1.0/setup.py
-drwxr-xr-x   0 treddy   (28751) staff       (20)        0 2023-05-23 17:39:51.000364 pytest-regex-0.1.0/tests/
--rw-r--r--   0 treddy   (28751) staff       (20)      764 2023-05-20 19:04:32.000000 pytest-regex-0.1.0/tests/test_plugin.py
+drwxr-xr-x   0 treddy   (28751) staff       (20)        0 2023-05-29 22:07:37.766297 pytest-regex-0.2.0/
+-rw-r--r--   0 treddy   (28751) staff       (20)     1068 2023-05-07 20:24:50.000000 pytest-regex-0.2.0/LICENSE
+-rw-r--r--   0 treddy   (28751) staff       (20)     3641 2023-05-29 22:07:37.766167 pytest-regex-0.2.0/PKG-INFO
+-rw-r--r--   0 treddy   (28751) staff       (20)     2565 2023-05-29 21:59:57.000000 pytest-regex-0.2.0/README.md
+-rw-r--r--   0 treddy   (28751) staff       (20)      323 2023-05-23 00:27:04.000000 pytest-regex-0.2.0/pyproject.toml
+drwxr-xr-x   0 treddy   (28751) staff       (20)        0 2023-05-29 22:07:37.765691 pytest-regex-0.2.0/pytest_regex.egg-info/
+-rw-r--r--   0 treddy   (28751) staff       (20)     3641 2023-05-29 22:07:37.000000 pytest-regex-0.2.0/pytest_regex.egg-info/PKG-INFO
+-rw-r--r--   0 treddy   (28751) staff       (20)      296 2023-05-29 22:07:37.000000 pytest-regex-0.2.0/pytest_regex.egg-info/SOURCES.txt
+-rw-r--r--   0 treddy   (28751) staff       (20)        1 2023-05-29 22:07:37.000000 pytest-regex-0.2.0/pytest_regex.egg-info/dependency_links.txt
+-rw-r--r--   0 treddy   (28751) staff       (20)       32 2023-05-29 22:07:37.000000 pytest-regex-0.2.0/pytest_regex.egg-info/entry_points.txt
+-rw-r--r--   0 treddy   (28751) staff       (20)       14 2023-05-29 22:07:37.000000 pytest-regex-0.2.0/pytest_regex.egg-info/requires.txt
+-rw-r--r--   0 treddy   (28751) staff       (20)       13 2023-05-29 22:07:37.000000 pytest-regex-0.2.0/pytest_regex.egg-info/top_level.txt
+-rw-r--r--   0 treddy   (28751) staff       (20)      885 2023-05-20 19:04:32.000000 pytest-regex-0.2.0/pytest_regex.py
+-rw-r--r--   0 treddy   (28751) staff       (20)       38 2023-05-29 22:07:37.766340 pytest-regex-0.2.0/setup.cfg
+-rw-r--r--   0 treddy   (28751) staff       (20)     1418 2023-05-29 22:07:13.000000 pytest-regex-0.2.0/setup.py
+drwxr-xr-x   0 treddy   (28751) staff       (20)        0 2023-05-29 22:07:37.765917 pytest-regex-0.2.0/tests/
+-rw-r--r--   0 treddy   (28751) staff       (20)      764 2023-05-20 19:04:32.000000 pytest-regex-0.2.0/tests/test_plugin.py
```

### Comparing `pytest-regex-0.1.0/LICENSE` & `pytest-regex-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-regex-0.1.0/PKG-INFO` & `pytest-regex-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,79 +1,79 @@
 Metadata-Version: 2.1
 Name: pytest-regex
-Version: 0.1.0
+Version: 0.2.0
 Summary: Select pytest tests with regular expressions
 Home-page: https://github.com/tylerjereddy/pytest-regex
 Author: Tyler Reddy
 Author-email: Tyler Reddy <tyler.je.reddy@gmail.com>
 Maintainer: Tyler Reddy
 Maintainer-email: tyler.je.reddy@gmail.com
 License: MIT
 Project-URL: Homepage, https://github.com/tylerjereddy/pytest-regex
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 License-File: LICENSE
 
-# pytest-regex
+pytest-regex
+------------
 
-## Use Python Standard Library Regular Expressions to Specify Tests to Run
+Use Python Standard Library Regular Expressions to Specify Tests to Run
+-----------------------------------------------------------------------
 
 After installing locally with i.e., `python -m pip install .` you can
 compare it with more conventional test selection techniques as follows.
 
 Consider working with SciPy development. Let's start off by selecting
 all tests with `test_3d` anywhere in their node id, using the conventional/
 built-in `-k` flag:
 
 `python dev.py test -- -v -k "test_3d"`
 
 This runs a bunch of tests with string matches as you might expect:
 
-```
-scipy/io/tests/test_idl.py::TestArrayDimensions::test_3d PASSED
-scipy/io/tests/test_idl.py::TestPointerArray::test_3d PASSED
-scipy/optimize/_trustregion_constr/tests/test_qp_subproblem.py::TestBoxBoundariesIntersections::test_3d_box_constraints PASSED
-scipy/optimize/_trustregion_constr/tests/test_qp_subproblem.py::TestBoxBoundariesIntersections::test_3d_box_constraints_entire_line PASSED
-scipy/optimize/_trustregion_constr/tests/test_qp_subproblem.py::TestModifiedDogleg::test_3d_example PASSED
-scipy/stats/tests/test_stats.py::TestGeometricStandardDeviation::test_3d_array PASSED
-scipy/stats/tests/test_stats.py::TestGeometricStandardDeviation::test_3d_array_axis_type_tuple PASSED
-scipy/stats/tests/test_stats.py::TestGeometricStandardDeviation::test_3d_array_axis_0 PASSED
-scipy/stats/tests/test_stats.py::TestGeometricStandardDeviation::test_3d_array_axis_1 PASSED
-scipy/stats/tests/test_stats.py::TestGeometricStandardDeviation::test_3d_array_axis_2 PASSED
-scipy/stats/tests/test_stats.py::TestFOneWay::test_3d_inputs PASSED
-```
+    scipy/io/tests/test_idl.py::TestArrayDimensions::test_3d PASSED
+    scipy/io/tests/test_idl.py::TestPointerArray::test_3d PASSED
+    scipy/optimize/_trustregion_constr/tests/test_qp_subproblem.py::TestBoxBoundariesIntersections::test_3d_box_constraints PASSED
+    scipy/optimize/_trustregion_constr/tests/test_qp_subproblem.py::TestBoxBoundariesIntersections::test_3d_box_constraints_entire_line PASSED
+    scipy/optimize/_trustregion_constr/tests/test_qp_subproblem.py::TestModifiedDogleg::test_3d_example PASSED
+    scipy/stats/tests/test_stats.py::TestGeometricStandardDeviation::test_3d_array PASSED
+    scipy/stats/tests/test_stats.py::TestGeometricStandardDeviation::test_3d_array_axis_type_tuple PASSED
+    scipy/stats/tests/test_stats.py::TestGeometricStandardDeviation::test_3d_array_axis_0 PASSED
+    scipy/stats/tests/test_stats.py::TestGeometricStandardDeviation::test_3d_array_axis_1 PASSED
+    scipy/stats/tests/test_stats.py::TestGeometricStandardDeviation::test_3d_array_axis_2 PASSED
+    scipy/stats/tests/test_stats.py::TestFOneWay::test_3d_inputs PASSED
 
 What if you want to run only tests with an exact match to `test_3d` or
 `test_3d_example`?
 
 Try `pytest-regex` with:
-`python dev.py test -- -v --regex "(.*test_3d$|.*test_3d_example$)"`
+    python dev.py test -- -v --regex "(.*test_3d$|.*test_3d_example$)"
 
 
-```
-scipy/io/tests/test_idl.py::TestArrayDimensions::test_3d PASSED
-scipy/io/tests/test_idl.py::TestPointerArray::test_3d PASSED
-scipy/optimize/_trustregion_constr/tests/test_qp_subproblem.py::TestModifiedDogleg::test_3d_example PASSED
-```
+    scipy/io/tests/test_idl.py::TestArrayDimensions::test_3d PASSED
+    scipy/io/tests/test_idl.py::TestPointerArray::test_3d PASSED
+    scipy/optimize/_trustregion_constr/tests/test_qp_subproblem.py::TestModifiedDogleg::test_3d_example PASSED
 
 This does what we want, and is probably more concise than the `-k` alternative. In fact,
 I'm not entirely sure how one would do this with `-k` in its current form.
 
-## How it Works
+How it Works
+------------
 
 `pytest-regex` simply passes the Python regular expression through
 to the list of node ids, where a node id is structured as follows:
 
 `path/to/test_module.py::TestClass::test_name[parameter_value]`
 
 If the regex matches the node id, the test is retained and executed.
```

### Comparing `pytest-regex-0.1.0/README.md` & `pytest-regex-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,52 @@
-# pytest-regex
+pytest-regex
+------------
 
-## Use Python Standard Library Regular Expressions to Specify Tests to Run
+Use Python Standard Library Regular Expressions to Specify Tests to Run
+-----------------------------------------------------------------------
 
 After installing locally with i.e., `python -m pip install .` you can
 compare it with more conventional test selection techniques as follows.
 
 Consider working with SciPy development. Let's start off by selecting
 all tests with `test_3d` anywhere in their node id, using the conventional/
 built-in `-k` flag:
 
 `python dev.py test -- -v -k "test_3d"`
 
 This runs a bunch of tests with string matches as you might expect:
 
-```
-scipy/io/tests/test_idl.py::TestArrayDimensions::test_3d PASSED
-scipy/io/tests/test_idl.py::TestPointerArray::test_3d PASSED
-scipy/optimize/_trustregion_constr/tests/test_qp_subproblem.py::TestBoxBoundariesIntersections::test_3d_box_constraints PASSED
-scipy/optimize/_trustregion_constr/tests/test_qp_subproblem.py::TestBoxBoundariesIntersections::test_3d_box_constraints_entire_line PASSED
-scipy/optimize/_trustregion_constr/tests/test_qp_subproblem.py::TestModifiedDogleg::test_3d_example PASSED
-scipy/stats/tests/test_stats.py::TestGeometricStandardDeviation::test_3d_array PASSED
-scipy/stats/tests/test_stats.py::TestGeometricStandardDeviation::test_3d_array_axis_type_tuple PASSED
-scipy/stats/tests/test_stats.py::TestGeometricStandardDeviation::test_3d_array_axis_0 PASSED
-scipy/stats/tests/test_stats.py::TestGeometricStandardDeviation::test_3d_array_axis_1 PASSED
-scipy/stats/tests/test_stats.py::TestGeometricStandardDeviation::test_3d_array_axis_2 PASSED
-scipy/stats/tests/test_stats.py::TestFOneWay::test_3d_inputs PASSED
-```
+    scipy/io/tests/test_idl.py::TestArrayDimensions::test_3d PASSED
+    scipy/io/tests/test_idl.py::TestPointerArray::test_3d PASSED
+    scipy/optimize/_trustregion_constr/tests/test_qp_subproblem.py::TestBoxBoundariesIntersections::test_3d_box_constraints PASSED
+    scipy/optimize/_trustregion_constr/tests/test_qp_subproblem.py::TestBoxBoundariesIntersections::test_3d_box_constraints_entire_line PASSED
+    scipy/optimize/_trustregion_constr/tests/test_qp_subproblem.py::TestModifiedDogleg::test_3d_example PASSED
+    scipy/stats/tests/test_stats.py::TestGeometricStandardDeviation::test_3d_array PASSED
+    scipy/stats/tests/test_stats.py::TestGeometricStandardDeviation::test_3d_array_axis_type_tuple PASSED
+    scipy/stats/tests/test_stats.py::TestGeometricStandardDeviation::test_3d_array_axis_0 PASSED
+    scipy/stats/tests/test_stats.py::TestGeometricStandardDeviation::test_3d_array_axis_1 PASSED
+    scipy/stats/tests/test_stats.py::TestGeometricStandardDeviation::test_3d_array_axis_2 PASSED
+    scipy/stats/tests/test_stats.py::TestFOneWay::test_3d_inputs PASSED
 
 What if you want to run only tests with an exact match to `test_3d` or
 `test_3d_example`?
 
 Try `pytest-regex` with:
-`python dev.py test -- -v --regex "(.*test_3d$|.*test_3d_example$)"`
+    python dev.py test -- -v --regex "(.*test_3d$|.*test_3d_example$)"
 
 
-```
-scipy/io/tests/test_idl.py::TestArrayDimensions::test_3d PASSED
-scipy/io/tests/test_idl.py::TestPointerArray::test_3d PASSED
-scipy/optimize/_trustregion_constr/tests/test_qp_subproblem.py::TestModifiedDogleg::test_3d_example PASSED
-```
+    scipy/io/tests/test_idl.py::TestArrayDimensions::test_3d PASSED
+    scipy/io/tests/test_idl.py::TestPointerArray::test_3d PASSED
+    scipy/optimize/_trustregion_constr/tests/test_qp_subproblem.py::TestModifiedDogleg::test_3d_example PASSED
 
 This does what we want, and is probably more concise than the `-k` alternative. In fact,
 I'm not entirely sure how one would do this with `-k` in its current form.
 
-## How it Works
+How it Works
+------------
 
 `pytest-regex` simply passes the Python regular expression through
 to the list of node ids, where a node id is structured as follows:
 
 `path/to/test_module.py::TestClass::test_name[parameter_value]`
 
 If the regex matches the node id, the test is retained and executed.
```

### Comparing `pytest-regex-0.1.0/pytest_regex.egg-info/PKG-INFO` & `pytest-regex-0.2.0/pytest_regex.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,79 +1,79 @@
 Metadata-Version: 2.1
 Name: pytest-regex
-Version: 0.1.0
+Version: 0.2.0
 Summary: Select pytest tests with regular expressions
 Home-page: https://github.com/tylerjereddy/pytest-regex
 Author: Tyler Reddy
 Author-email: Tyler Reddy <tyler.je.reddy@gmail.com>
 Maintainer: Tyler Reddy
 Maintainer-email: tyler.je.reddy@gmail.com
 License: MIT
 Project-URL: Homepage, https://github.com/tylerjereddy/pytest-regex
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 License-File: LICENSE
 
-# pytest-regex
+pytest-regex
+------------
 
-## Use Python Standard Library Regular Expressions to Specify Tests to Run
+Use Python Standard Library Regular Expressions to Specify Tests to Run
+-----------------------------------------------------------------------
 
 After installing locally with i.e., `python -m pip install .` you can
 compare it with more conventional test selection techniques as follows.
 
 Consider working with SciPy development. Let's start off by selecting
 all tests with `test_3d` anywhere in their node id, using the conventional/
 built-in `-k` flag:
 
 `python dev.py test -- -v -k "test_3d"`
 
 This runs a bunch of tests with string matches as you might expect:
 
-```
-scipy/io/tests/test_idl.py::TestArrayDimensions::test_3d PASSED
-scipy/io/tests/test_idl.py::TestPointerArray::test_3d PASSED
-scipy/optimize/_trustregion_constr/tests/test_qp_subproblem.py::TestBoxBoundariesIntersections::test_3d_box_constraints PASSED
-scipy/optimize/_trustregion_constr/tests/test_qp_subproblem.py::TestBoxBoundariesIntersections::test_3d_box_constraints_entire_line PASSED
-scipy/optimize/_trustregion_constr/tests/test_qp_subproblem.py::TestModifiedDogleg::test_3d_example PASSED
-scipy/stats/tests/test_stats.py::TestGeometricStandardDeviation::test_3d_array PASSED
-scipy/stats/tests/test_stats.py::TestGeometricStandardDeviation::test_3d_array_axis_type_tuple PASSED
-scipy/stats/tests/test_stats.py::TestGeometricStandardDeviation::test_3d_array_axis_0 PASSED
-scipy/stats/tests/test_stats.py::TestGeometricStandardDeviation::test_3d_array_axis_1 PASSED
-scipy/stats/tests/test_stats.py::TestGeometricStandardDeviation::test_3d_array_axis_2 PASSED
-scipy/stats/tests/test_stats.py::TestFOneWay::test_3d_inputs PASSED
-```
+    scipy/io/tests/test_idl.py::TestArrayDimensions::test_3d PASSED
+    scipy/io/tests/test_idl.py::TestPointerArray::test_3d PASSED
+    scipy/optimize/_trustregion_constr/tests/test_qp_subproblem.py::TestBoxBoundariesIntersections::test_3d_box_constraints PASSED
+    scipy/optimize/_trustregion_constr/tests/test_qp_subproblem.py::TestBoxBoundariesIntersections::test_3d_box_constraints_entire_line PASSED
+    scipy/optimize/_trustregion_constr/tests/test_qp_subproblem.py::TestModifiedDogleg::test_3d_example PASSED
+    scipy/stats/tests/test_stats.py::TestGeometricStandardDeviation::test_3d_array PASSED
+    scipy/stats/tests/test_stats.py::TestGeometricStandardDeviation::test_3d_array_axis_type_tuple PASSED
+    scipy/stats/tests/test_stats.py::TestGeometricStandardDeviation::test_3d_array_axis_0 PASSED
+    scipy/stats/tests/test_stats.py::TestGeometricStandardDeviation::test_3d_array_axis_1 PASSED
+    scipy/stats/tests/test_stats.py::TestGeometricStandardDeviation::test_3d_array_axis_2 PASSED
+    scipy/stats/tests/test_stats.py::TestFOneWay::test_3d_inputs PASSED
 
 What if you want to run only tests with an exact match to `test_3d` or
 `test_3d_example`?
 
 Try `pytest-regex` with:
-`python dev.py test -- -v --regex "(.*test_3d$|.*test_3d_example$)"`
+    python dev.py test -- -v --regex "(.*test_3d$|.*test_3d_example$)"
 
 
-```
-scipy/io/tests/test_idl.py::TestArrayDimensions::test_3d PASSED
-scipy/io/tests/test_idl.py::TestPointerArray::test_3d PASSED
-scipy/optimize/_trustregion_constr/tests/test_qp_subproblem.py::TestModifiedDogleg::test_3d_example PASSED
-```
+    scipy/io/tests/test_idl.py::TestArrayDimensions::test_3d PASSED
+    scipy/io/tests/test_idl.py::TestPointerArray::test_3d PASSED
+    scipy/optimize/_trustregion_constr/tests/test_qp_subproblem.py::TestModifiedDogleg::test_3d_example PASSED
 
 This does what we want, and is probably more concise than the `-k` alternative. In fact,
 I'm not entirely sure how one would do this with `-k` in its current form.
 
-## How it Works
+How it Works
+------------
 
 `pytest-regex` simply passes the Python regular expression through
 to the list of node ids, where a node id is structured as follows:
 
 `path/to/test_module.py::TestClass::test_name[parameter_value]`
 
 If the regex matches the node id, the test is retained and executed.
```

### Comparing `pytest-regex-0.1.0/pytest_regex.py` & `pytest-regex-0.2.0/pytest_regex.py`

 * *Files identical despite different names*

### Comparing `pytest-regex-0.1.0/setup.py` & `pytest-regex-0.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,32 +6,33 @@
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return codecs.open(file_path, encoding='utf-8').read()
 
 
 setup(
     name='pytest-regex',
-    version='0.1.0',
+    version='0.2.0',
     author='Tyler Reddy',
     author_email='tyler.je.reddy@gmail.com',
     maintainer='Tyler Reddy',
     maintainer_email='tyler.je.reddy@gmail.com',
     license='MIT',
     url='https://github.com/tylerjereddy/pytest-regex',
     description='Select tests with Python regex',
     long_description=read('README.md'),
     py_modules=['pytest_regex'],
-    python_requires='>=3.9',
+    python_requires='>=3.8',
     install_requires=['pytest>=3.5.0'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Framework :: Pytest',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Testing',
         'Programming Language :: Python',
+        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: Implementation :: CPython',
         'Operating System :: OS Independent',
         'License :: OSI Approved :: MIT License',
```

### Comparing `pytest-regex-0.1.0/tests/test_plugin.py` & `pytest-regex-0.2.0/tests/test_plugin.py`

 * *Files identical despite different names*

