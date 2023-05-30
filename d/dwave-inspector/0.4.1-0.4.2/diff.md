# Comparing `tmp/dwave-inspector-0.4.1.tar.gz` & `tmp/dwave-inspector-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwave-inspector-0.4.1.tar", last modified: Wed Jan 25 16:54:41 2023, max compression
+gzip compressed data, was "dwave-inspector-0.4.2.tar", last modified: Tue May 30 16:12:11 2023, max compression
```

## Comparing `dwave-inspector-0.4.1.tar` & `dwave-inspector-0.4.2.tar`

### file list

```diff
@@ -1,26 +1,34 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-01-25 16:54:41.473558 dwave-inspector-0.4.1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11359 2023-01-25 16:53:50.000000 dwave-inspector-0.4.1/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4277 2023-01-25 16:54:41.473558 dwave-inspector-0.4.1/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3516 2023-01-25 16:53:50.000000 dwave-inspector-0.4.1/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-01-25 16:54:41.469558 dwave-inspector-0.4.1/dwave/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      648 2023-01-25 16:53:50.000000 dwave-inspector-0.4.1/dwave/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-01-25 16:54:41.469558 dwave-inspector-0.4.1/dwave/inspector/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6610 2023-01-25 16:53:50.000000 dwave-inspector-0.4.1/dwave/inspector/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33419 2023-01-25 16:53:50.000000 dwave-inspector-0.4.1/dwave/inspector/adapters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1339 2023-01-25 16:53:50.000000 dwave-inspector-0.4.1/dwave/inspector/config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1730 2023-01-25 16:53:50.000000 dwave-inspector-0.4.1/dwave/inspector/package_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2928 2023-01-25 16:53:50.000000 dwave-inspector-0.4.1/dwave/inspector/proxies.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9023 2023-01-25 16:53:50.000000 dwave-inspector-0.4.1/dwave/inspector/server.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4613 2023-01-25 16:53:50.000000 dwave-inspector-0.4.1/dwave/inspector/storage.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6758 2023-01-25 16:53:50.000000 dwave-inspector-0.4.1/dwave/inspector/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2698 2023-01-25 16:53:50.000000 dwave-inspector-0.4.1/dwave/inspector/viewers.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-01-25 16:54:41.473558 dwave-inspector-0.4.1/dwave_inspector.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4277 2023-01-25 16:54:41.000000 dwave-inspector-0.4.1/dwave_inspector.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      575 2023-01-25 16:54:41.000000 dwave-inspector-0.4.1/dwave_inspector.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-01-25 16:54:41.000000 dwave-inspector-0.4.1/dwave_inspector.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      355 2023-01-25 16:54:41.000000 dwave-inspector-0.4.1/dwave_inspector.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-01-25 16:54:41.000000 dwave-inspector-0.4.1/dwave_inspector.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      206 2023-01-25 16:54:41.000000 dwave-inspector-0.4.1/dwave_inspector.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-01-25 16:54:41.000000 dwave-inspector-0.4.1/dwave_inspector.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-01-25 16:54:41.473558 dwave-inspector-0.4.1/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2538 2023-01-25 16:53:50.000000 dwave-inspector-0.4.1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-30 16:12:11.520569 dwave-inspector-0.4.2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11359 2023-05-30 16:11:24.000000 dwave-inspector-0.4.2/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4227 2023-05-30 16:12:11.520569 dwave-inspector-0.4.2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3466 2023-05-30 16:11:24.000000 dwave-inspector-0.4.2/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-30 16:12:11.516569 dwave-inspector-0.4.2/dwave/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      648 2023-05-30 16:11:24.000000 dwave-inspector-0.4.2/dwave/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-30 16:12:11.516569 dwave-inspector-0.4.2/dwave/inspector/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6610 2023-05-30 16:11:24.000000 dwave-inspector-0.4.2/dwave/inspector/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33419 2023-05-30 16:11:24.000000 dwave-inspector-0.4.2/dwave/inspector/adapters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1339 2023-05-30 16:11:24.000000 dwave-inspector-0.4.2/dwave/inspector/config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1730 2023-05-30 16:11:24.000000 dwave-inspector-0.4.2/dwave/inspector/package_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2928 2023-05-30 16:11:24.000000 dwave-inspector-0.4.2/dwave/inspector/proxies.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9023 2023-05-30 16:11:24.000000 dwave-inspector-0.4.2/dwave/inspector/server.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4613 2023-05-30 16:11:24.000000 dwave-inspector-0.4.2/dwave/inspector/storage.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6758 2023-05-30 16:11:24.000000 dwave-inspector-0.4.2/dwave/inspector/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2698 2023-05-30 16:11:24.000000 dwave-inspector-0.4.2/dwave/inspector/viewers.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-30 16:12:11.520569 dwave-inspector-0.4.2/dwave_inspector.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4227 2023-05-30 16:12:11.000000 dwave-inspector-0.4.2/dwave_inspector.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      726 2023-05-30 16:12:11.000000 dwave-inspector-0.4.2/dwave_inspector.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-30 16:12:11.000000 dwave-inspector-0.4.2/dwave_inspector.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      355 2023-05-30 16:12:11.000000 dwave-inspector-0.4.2/dwave_inspector.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-30 16:12:11.000000 dwave-inspector-0.4.2/dwave_inspector.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      206 2023-05-30 16:12:11.000000 dwave-inspector-0.4.2/dwave_inspector.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-05-30 16:12:11.000000 dwave-inspector-0.4.2/dwave_inspector.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-05-30 16:12:11.524570 dwave-inspector-0.4.2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2538 2023-05-30 16:11:24.000000 dwave-inspector-0.4.2/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-30 16:12:11.520569 dwave-inspector-0.4.2/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23506 2023-05-30 16:11:24.000000 dwave-inspector-0.4.2/tests/test_adapters.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1432 2023-05-30 16:11:24.000000 dwave-inspector-0.4.2/tests/test_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3702 2023-05-30 16:11:24.000000 dwave-inspector-0.4.2/tests/test_proxies.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5488 2023-05-30 16:11:24.000000 dwave-inspector-0.4.2/tests/test_server.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1994 2023-05-30 16:11:24.000000 dwave-inspector-0.4.2/tests/test_storage.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3093 2023-05-30 16:11:24.000000 dwave-inspector-0.4.2/tests/test_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3189 2023-05-30 16:11:24.000000 dwave-inspector-0.4.2/tests/test_viewers.py
```

### Comparing `dwave-inspector-0.4.1/LICENSE` & `dwave-inspector-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dwave-inspector-0.4.1/PKG-INFO` & `dwave-inspector-0.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwave-inspector
-Version: 0.4.1
+Version: 0.4.2
 Summary: D-Wave Problem Inspector tool
 Home-page: https://github.com/dwavesystems/dwave-inspector
 Author: D-Wave Systems Inc.
 Author-email: radomir@dwavesys.com
 License: Apache 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -51,32 +51,32 @@
 
 
 Example
 =======
 
 .. example-start-marker
 
-This example shows the canonical usage: samples representing physical qubits on
-a quantum processing unit (QPU).
+This example shows a typical usage: a binary quadratic model minor-embedded 
+onto a quantum processing unit (QPU).
 
 .. code-block:: python
 
-    import dwave.system
+    from dwave.system import DWaveSampler, EmbeddingComposite
+    import dimod
     import dwave.inspector
 
     # Get sampler
-    sampler = dwave.system.DWaveSampler()
+    sampler = EmbeddingComposite(DWaveSampler())
 
-    # Define a problem (actual qubits depend on the selected QPU's working graph)
-    h = {}
-    J = {(0, 4): 1, (0, 5): 1, (1, 4): 1, (1, 5): -1}
-    assert all(edge in sampler.edgelist for edge in J)
+    # Define a problem
+    x, y, z = dimod.Binaries(['x', 'y', 'z'])
+    bqm = x*y - x*z + 2*y
 
     # Sample
-    sampleset = sampler.sample_ising(h, J, num_reads=100)
+    sampleset = sampler.sample(bqm, num_reads=100)
 
     # Inspect
     dwave.inspector.show(sampleset)
 
 .. example-end-marker
```

### Comparing `dwave-inspector-0.4.1/README.rst` & `dwave-inspector-0.4.2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -30,32 +30,32 @@
 
 
 Example
 =======
 
 .. example-start-marker
 
-This example shows the canonical usage: samples representing physical qubits on
-a quantum processing unit (QPU).
+This example shows a typical usage: a binary quadratic model minor-embedded 
+onto a quantum processing unit (QPU).
 
 .. code-block:: python
 
-    import dwave.system
+    from dwave.system import DWaveSampler, EmbeddingComposite
+    import dimod
     import dwave.inspector
 
     # Get sampler
-    sampler = dwave.system.DWaveSampler()
+    sampler = EmbeddingComposite(DWaveSampler())
 
-    # Define a problem (actual qubits depend on the selected QPU's working graph)
-    h = {}
-    J = {(0, 4): 1, (0, 5): 1, (1, 4): 1, (1, 5): -1}
-    assert all(edge in sampler.edgelist for edge in J)
+    # Define a problem
+    x, y, z = dimod.Binaries(['x', 'y', 'z'])
+    bqm = x*y - x*z + 2*y
 
     # Sample
-    sampleset = sampler.sample_ising(h, J, num_reads=100)
+    sampleset = sampler.sample(bqm, num_reads=100)
 
     # Inspect
     dwave.inspector.show(sampleset)
 
 .. example-end-marker
```

### Comparing `dwave-inspector-0.4.1/dwave/__init__.py` & `dwave-inspector-0.4.2/dwave/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave-inspector-0.4.1/dwave/inspector/__init__.py` & `dwave-inspector-0.4.2/dwave/inspector/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave-inspector-0.4.1/dwave/inspector/adapters.py` & `dwave-inspector-0.4.2/dwave/inspector/adapters.py`

 * *Files identical despite different names*

### Comparing `dwave-inspector-0.4.1/dwave/inspector/config.py` & `dwave-inspector-0.4.2/dwave/inspector/config.py`

 * *Files identical despite different names*

### Comparing `dwave-inspector-0.4.1/dwave/inspector/package_info.py` & `dwave-inspector-0.4.2/dwave/inspector/package_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     '__package_name__', '__title__', '__version__',
     '__author__', '__author_email__', '__description__',
     '__url__', '__license__', '__copyright__'
 ]
 
 __package_name__ = 'dwave-inspector'
 __title__ = 'D-Wave Problem Inspector'
-__version__ = '0.4.1'
+__version__ = '0.4.2'
 __author__ = 'D-Wave Systems Inc.'
 __author_email__ = 'radomir@dwavesys.com'
 __description__ = 'D-Wave Problem Inspector tool'
 __url__ = 'https://github.com/dwavesystems/dwave-inspector'
 __license__ = 'Apache 2.0'
 __copyright__ = '2019, D-Wave Systems Inc.'
```

### Comparing `dwave-inspector-0.4.1/dwave/inspector/proxies.py` & `dwave-inspector-0.4.2/dwave/inspector/proxies.py`

 * *Files identical despite different names*

### Comparing `dwave-inspector-0.4.1/dwave/inspector/server.py` & `dwave-inspector-0.4.2/dwave/inspector/server.py`

 * *Files identical despite different names*

### Comparing `dwave-inspector-0.4.1/dwave/inspector/storage.py` & `dwave-inspector-0.4.2/dwave/inspector/storage.py`

 * *Files identical despite different names*

### Comparing `dwave-inspector-0.4.1/dwave/inspector/utils.py` & `dwave-inspector-0.4.2/dwave/inspector/utils.py`

 * *Files identical despite different names*

### Comparing `dwave-inspector-0.4.1/dwave/inspector/viewers.py` & `dwave-inspector-0.4.2/dwave/inspector/viewers.py`

 * *Files identical despite different names*

### Comparing `dwave-inspector-0.4.1/dwave_inspector.egg-info/PKG-INFO` & `dwave-inspector-0.4.2/dwave_inspector.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwave-inspector
-Version: 0.4.1
+Version: 0.4.2
 Summary: D-Wave Problem Inspector tool
 Home-page: https://github.com/dwavesystems/dwave-inspector
 Author: D-Wave Systems Inc.
 Author-email: radomir@dwavesys.com
 License: Apache 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -51,32 +51,32 @@
 
 
 Example
 =======
 
 .. example-start-marker
 
-This example shows the canonical usage: samples representing physical qubits on
-a quantum processing unit (QPU).
+This example shows a typical usage: a binary quadratic model minor-embedded 
+onto a quantum processing unit (QPU).
 
 .. code-block:: python
 
-    import dwave.system
+    from dwave.system import DWaveSampler, EmbeddingComposite
+    import dimod
     import dwave.inspector
 
     # Get sampler
-    sampler = dwave.system.DWaveSampler()
+    sampler = EmbeddingComposite(DWaveSampler())
 
-    # Define a problem (actual qubits depend on the selected QPU's working graph)
-    h = {}
-    J = {(0, 4): 1, (0, 5): 1, (1, 4): 1, (1, 5): -1}
-    assert all(edge in sampler.edgelist for edge in J)
+    # Define a problem
+    x, y, z = dimod.Binaries(['x', 'y', 'z'])
+    bqm = x*y - x*z + 2*y
 
     # Sample
-    sampleset = sampler.sample_ising(h, J, num_reads=100)
+    sampleset = sampler.sample(bqm, num_reads=100)
 
     # Inspect
     dwave.inspector.show(sampleset)
 
 .. example-end-marker
```

### Comparing `dwave-inspector-0.4.1/dwave_inspector.egg-info/SOURCES.txt` & `dwave-inspector-0.4.2/dwave_inspector.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -14,8 +14,15 @@
 dwave/inspector/viewers.py
 dwave_inspector.egg-info/PKG-INFO
 dwave_inspector.egg-info/SOURCES.txt
 dwave_inspector.egg-info/dependency_links.txt
 dwave_inspector.egg-info/entry_points.txt
 dwave_inspector.egg-info/not-zip-safe
 dwave_inspector.egg-info/requires.txt
-dwave_inspector.egg-info/top_level.txt
+dwave_inspector.egg-info/top_level.txt
+tests/test_adapters.py
+tests/test_config.py
+tests/test_proxies.py
+tests/test_server.py
+tests/test_storage.py
+tests/test_utils.py
+tests/test_viewers.py
```

### Comparing `dwave-inspector-0.4.1/setup.py` & `dwave-inspector-0.4.2/setup.py`

 * *Files identical despite different names*

