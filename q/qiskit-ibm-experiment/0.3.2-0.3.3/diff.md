# Comparing `tmp/qiskit-ibm-experiment-0.3.2.tar.gz` & `tmp/qiskit-ibm-experiment-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-ibm-experiment-0.3.2.tar", last modified: Wed May 24 12:08:38 2023, max compression
+gzip compressed data, was "qiskit-ibm-experiment-0.3.3.tar", last modified: Tue May 30 10:55:27 2023, max compression
```

## Comparing `qiskit-ibm-experiment-0.3.2.tar` & `qiskit-ibm-experiment-0.3.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:08:38.268434 qiskit-ibm-experiment-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-05-24 12:08:38.268434 qiskit-ibm-experiment-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:08:38.264434 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:08:38.264434 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/accounts/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/accounts/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/accounts/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/accounts/management.py
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/accounts/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:08:38.264434 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/client/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/client/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    15604 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/client/experiment_rest_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)    27949 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/client/local_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/client/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:08:38.264434 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/service/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/service/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/service/device_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/service/experiment_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)    69035 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/service/ibm_experiment_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/service/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:08:38.264434 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-05-24 12:08:38.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-24 12:08:38.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 12:08:38.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 12:08:38.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-24 12:08:38.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-24 12:08:38.000000 qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 12:08:38.268434 qiskit-ibm-experiment-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:08:38.264434 qiskit-ibm-experiment-0.3.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:08:38.264434 qiskit-ibm-experiment-0.3.2/test/service/
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/test/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/test/service/ibm_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/test/service/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    21605 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/test/service/test_experiment_data_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    66547 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/test/service/test_experiment_server_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    17739 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/test/service/test_local_experiment_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:08:38.268434 qiskit-ibm-experiment-0.3.2/test/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/test/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/test/utils/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/test/utils/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-24 12:08:28.000000 qiskit-ibm-experiment-0.3.2/test/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:55:27.313119 qiskit-ibm-experiment-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-05-30 10:55:27.313119 qiskit-ibm-experiment-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:55:27.301118 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:55:27.305118 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/accounts/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/accounts/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/accounts/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/accounts/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/accounts/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:55:27.305118 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/client/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15604 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/client/experiment_rest_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27949 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/client/local_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/client/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:55:27.309119 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/service/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/service/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/service/device_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/service/experiment_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69048 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/service/ibm_experiment_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/service/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:55:27.305118 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-05-30 10:55:27.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-30 10:55:27.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:55:27.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:55:27.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-30 10:55:27.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 10:55:27.000000 qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 10:55:27.313119 qiskit-ibm-experiment-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:55:27.309119 qiskit-ibm-experiment-0.3.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:55:27.309119 qiskit-ibm-experiment-0.3.3/test/service/
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/test/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/test/service/ibm_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/test/service/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21605 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/test/service/test_experiment_data_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66547 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/test/service/test_experiment_server_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18019 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/test/service/test_local_experiment_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:55:27.309119 qiskit-ibm-experiment-0.3.3/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/test/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/test/utils/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/test/utils/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-30 10:55:19.000000 qiskit-ibm-experiment-0.3.3/test/utils/utils.py
```

### Comparing `qiskit-ibm-experiment-0.3.2/LICENSE.txt` & `qiskit-ibm-experiment-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.2/PKG-INFO` & `qiskit-ibm-experiment-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-ibm-experiment
-Version: 0.3.2
+Version: 0.3.3
 Summary: Qiskit IBM Experiment service for accessing the quantum experiment interface at IBM
 Home-page: https://github.com/Qiskit/qiskit-ibm-experiment
 Author: Qiskit Development Team
 Author-email: hello@qiskit.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-ibm-experiment/issues
 Project-URL: Documentation, https://qiskit.org/documentation/
```

### Comparing `qiskit-ibm-experiment-0.3.2/README.md` & `qiskit-ibm-experiment-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/__init__.py` & `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/accounts/__init__.py` & `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/accounts/account.py` & `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/accounts/account.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/accounts/configuration.py` & `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/accounts/configuration.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/accounts/exceptions.py` & `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/accounts/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/accounts/management.py` & `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/accounts/management.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/accounts/storage.py` & `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/accounts/storage.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/client/__init__.py` & `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/client/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/client/experiment.py` & `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/client/experiment.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/client/experiment_rest_adapter.py` & `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/client/experiment_rest_adapter.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/client/local_client.py` & `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/client/local_client.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/client/session.py` & `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/client/session.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/exceptions.py` & `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/service/__init__.py` & `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/service/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/service/constants.py` & `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/service/constants.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/service/device_component.py` & `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/service/device_component.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/service/experiment_dataclasses.py` & `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/service/experiment_dataclasses.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/service/ibm_experiment_service.py` & `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/service/ibm_experiment_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1509,20 +1509,21 @@
         if not figure_name.endswith(".svg"):
             figure_name += ".svg"
 
         if isinstance(figure, str):
             with open(figure, "rb") as file:
                 figure = file.read()
 
+        response = None
         with map_api_error(f"Figure {figure_name} update failed."):
             response = self._api_client.experiment_plot_update(
                 experiment_id, figure, figure_name
             )
 
-        if response.status_code != 200:
+        if response is None:
             return None
         return figure_name, len(figure)
 
     def create_or_update_figure(
         self,
         experiment_id: str,
         figure: Union[str, bytes],
```

### Comparing `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/service/utils.py` & `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/service/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment/version.py` & `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment/version.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment.egg-info/PKG-INFO` & `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-ibm-experiment
-Version: 0.3.2
+Version: 0.3.3
 Summary: Qiskit IBM Experiment service for accessing the quantum experiment interface at IBM
 Home-page: https://github.com/Qiskit/qiskit-ibm-experiment
 Author: Qiskit Development Team
 Author-email: hello@qiskit.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-ibm-experiment/issues
 Project-URL: Documentation, https://qiskit.org/documentation/
```

### Comparing `qiskit-ibm-experiment-0.3.2/qiskit_ibm_experiment.egg-info/SOURCES.txt` & `qiskit-ibm-experiment-0.3.3/qiskit_ibm_experiment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.2/setup.py` & `qiskit-ibm-experiment-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.2/test/__init__.py` & `qiskit-ibm-experiment-0.3.3/test/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.2/test/service/ibm_test_case.py` & `qiskit-ibm-experiment-0.3.3/test/service/ibm_test_case.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.2/test/service/test_experiment.py` & `qiskit-ibm-experiment-0.3.3/test/service/test_experiment.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.2/test/service/test_experiment_data_integration.py` & `qiskit-ibm-experiment-0.3.3/test/service/test_experiment_data_integration.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.2/test/service/test_experiment_server_integration.py` & `qiskit-ibm-experiment-0.3.3/test/service/test_experiment_server_integration.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.2/test/service/test_local_experiment_client.py` & `qiskit-ibm-experiment-0.3.3/test/service/test_local_experiment_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,14 +253,20 @@
         hello_bytes = str.encode("hello world")
         figure_name = "hello.svg"
         self.service.create_figure(
             experiment_id=exp_id, figure=hello_bytes, figure_name=figure_name
         )
         fig = self.service.figure(exp_id, figure_name)
         self.assertEqual(fig, hello_bytes)
+        hello_bytes = str.encode("hello world version 2")
+        self.service.update_figure(
+            experiment_id=exp_id, figure=hello_bytes, figure_name=figure_name
+        )
+        fig = self.service.figure(exp_id, figure_name)
+        self.assertEqual(fig, hello_bytes)
 
     def test_files(self):
         """Test upload and download of files"""
         exp_id = self.service.create_experiment(
             ExperimentData(
                 experiment_type="test_experiment", backend="ibmq_qasm_simulator"
             )
```

### Comparing `qiskit-ibm-experiment-0.3.2/test/utils/program.py` & `qiskit-ibm-experiment-0.3.3/test/utils/program.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.2/test/utils/templates.py` & `qiskit-ibm-experiment-0.3.3/test/utils/templates.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-experiment-0.3.2/test/utils/utils.py` & `qiskit-ibm-experiment-0.3.3/test/utils/utils.py`

 * *Files identical despite different names*

