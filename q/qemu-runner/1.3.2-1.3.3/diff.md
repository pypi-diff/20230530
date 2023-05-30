# Comparing `tmp/qemu-runner-1.3.2.tar.gz` & `tmp/qemu-runner-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qemu-runner-1.3.2.tar", last modified: Sun Apr 23 18:11:20 2023, max compression
+gzip compressed data, was "qemu-runner-1.3.3.tar", last modified: Tue May 30 18:51:54 2023, max compression
```

## Comparing `qemu-runner-1.3.2.tar` & `qemu-runner-1.3.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:11:20.814919 qemu-runner-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-04-23 18:11:20.814919 qemu-runner-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 18:11:20.814919 qemu-runner-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:11:20.810919 qemu-runner-1.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:11:20.810919 qemu-runner-1.3.2/src/qemu_runner/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/src/qemu_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/src/qemu_runner/argument.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/src/qemu_runner/find_qemu.py
--rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/src/qemu_runner/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/src/qemu_runner/layer_locator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:11:20.810919 qemu-runner-1.3.2/src/qemu_runner/layers/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/src/qemu_runner/layers/virt-cortex-m.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:11:20.810919 qemu-runner-1.3.2/src/qemu_runner/make_runner/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/src/qemu_runner/make_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/src/qemu_runner/make_runner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/src/qemu_runner/make_runner/main.py.in
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/src/qemu_runner/make_runner/make.py
--rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/src/qemu_runner/make_runner/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/src/qemu_runner/variable_resolution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:11:20.810919 qemu-runner-1.3.2/src/qemu_runner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-04-23 18:11:20.000000 qemu-runner-1.3.2/src/qemu_runner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-23 18:11:20.000000 qemu-runner-1.3.2/src/qemu_runner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 18:11:20.000000 qemu-runner-1.3.2/src/qemu_runner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-23 18:11:20.000000 qemu-runner-1.3.2/src/qemu_runner.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-23 18:11:20.000000 qemu-runner-1.3.2/src/qemu_runner.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 18:11:20.814919 qemu-runner-1.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/tests/test_find_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/tests/test_find_qemu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/tests/test_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/tests/test_layer_cmdline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/tests/test_layer_equality.py
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/tests/test_layer_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/tests/test_qemu_argument.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/tests/test_qemu_argument_equality.py
--rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/tests/test_runner_flow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/tests/test_utllities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-23 18:11:08.000000 qemu-runner-1.3.2/tests/test_venv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:51:54.186870 qemu-runner-1.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-30 18:51:42.000000 qemu-runner-1.3.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-30 18:51:42.000000 qemu-runner-1.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-05-30 18:51:54.186870 qemu-runner-1.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-05-30 18:51:42.000000 qemu-runner-1.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-30 18:51:42.000000 qemu-runner-1.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 18:51:54.186870 qemu-runner-1.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-30 18:51:42.000000 qemu-runner-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:51:54.182870 qemu-runner-1.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:51:54.186870 qemu-runner-1.3.3/src/qemu_runner/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-30 18:51:42.000000 qemu-runner-1.3.3/src/qemu_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-30 18:51:42.000000 qemu-runner-1.3.3/src/qemu_runner/argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-30 18:51:42.000000 qemu-runner-1.3.3/src/qemu_runner/find_qemu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-05-30 18:51:42.000000 qemu-runner-1.3.3/src/qemu_runner/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-30 18:51:42.000000 qemu-runner-1.3.3/src/qemu_runner/layer_locator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:51:54.186870 qemu-runner-1.3.3/src/qemu_runner/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-30 18:51:42.000000 qemu-runner-1.3.3/src/qemu_runner/layers/virt-cortex-m.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:51:54.186870 qemu-runner-1.3.3/src/qemu_runner/make_runner/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:51:42.000000 qemu-runner-1.3.3/src/qemu_runner/make_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-30 18:51:42.000000 qemu-runner-1.3.3/src/qemu_runner/make_runner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-30 18:51:42.000000 qemu-runner-1.3.3/src/qemu_runner/make_runner/main.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-05-30 18:51:42.000000 qemu-runner-1.3.3/src/qemu_runner/make_runner/make.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9452 2023-05-30 18:51:42.000000 qemu-runner-1.3.3/src/qemu_runner/make_runner/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-30 18:51:42.000000 qemu-runner-1.3.3/src/qemu_runner/variable_resolution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:51:54.186870 qemu-runner-1.3.3/src/qemu_runner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9164 2023-05-30 18:51:54.000000 qemu-runner-1.3.3/src/qemu_runner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-30 18:51:54.000000 qemu-runner-1.3.3/src/qemu_runner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 18:51:54.000000 qemu-runner-1.3.3/src/qemu_runner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-30 18:51:54.000000 qemu-runner-1.3.3/src/qemu_runner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-30 18:51:54.000000 qemu-runner-1.3.3/src/qemu_runner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:51:54.186870 qemu-runner-1.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-05-30 18:51:42.000000 qemu-runner-1.3.3/tests/test_find_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-30 18:51:42.000000 qemu-runner-1.3.3/tests/test_find_qemu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-30 18:51:42.000000 qemu-runner-1.3.3/tests/test_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-30 18:51:42.000000 qemu-runner-1.3.3/tests/test_layer_cmdline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-05-30 18:51:42.000000 qemu-runner-1.3.3/tests/test_layer_equality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-30 18:51:42.000000 qemu-runner-1.3.3/tests/test_layer_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-05-30 18:51:42.000000 qemu-runner-1.3.3/tests/test_qemu_argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-30 18:51:42.000000 qemu-runner-1.3.3/tests/test_qemu_argument_equality.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13058 2023-05-30 18:51:42.000000 qemu-runner-1.3.3/tests/test_runner_flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-30 18:51:42.000000 qemu-runner-1.3.3/tests/test_utllities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-05-30 18:51:42.000000 qemu-runner-1.3.3/tests/test_venv.py
```

### Comparing `qemu-runner-1.3.2/LICENSE.txt` & `qemu-runner-1.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.2/PKG-INFO` & `qemu-runner-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qemu-runner
-Version: 1.3.2
+Version: 1.3.3
 Summary: Create self-contained wrappers around QEMU to hide & share long command-line invocations
 Home-page: https://github.com/Novakov/qemu-runner
 Author: Maciej Nowak
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `qemu-runner-1.3.2/README.md` & `qemu-runner-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.2/setup.py` & `qemu-runner-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 with open(os.path.dirname(os.path.abspath(__file__)) + '/README.md', 'r') as f:
     description = f.read()
 
 setup(
     name='qemu-runner',
-    version='1.3.2',
+    version='1.3.3',
     description='Create self-contained wrappers around QEMU to hide & share long command-line invocations',
     url='https://github.com/Novakov/qemu-runner',
     long_description=description,
     long_description_content_type='text/markdown',
     author='Maciej Nowak',
     classifiers=[
         'Development Status :: 4 - Beta',
```

### Comparing `qemu-runner-1.3.2/src/qemu_runner/argument.py` & `qemu-runner-1.3.3/src/qemu_runner/argument.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.2/src/qemu_runner/find_qemu.py` & `qemu-runner-1.3.3/src/qemu_runner/find_qemu.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.2/src/qemu_runner/layer.py` & `qemu-runner-1.3.3/src/qemu_runner/layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
                 self._general,
                 engine=other.engine if other.engine != '' else self._general.engine,
                 kernel=other.kernel if other.kernel != '' else self._general.kernel,
                 kernel_cmdline=' '.join(cmdline) if cmdline else None,
                 halted=other.halted if other.halted is not None else self._general.halted,
                 gdb=other.gdb if other.gdb is not None else self._general.gdb,
                 gdb_dev=other.gdb_dev if other.gdb_dev is not None else self._general.gdb_dev,
+                memory=other.memory if other.memory is not None else self._general.memory
             )
 
         def apply_arguments() -> Iterable[Argument]:
             remaining_other = list(addition._arguments)
 
             for arg in self._arguments:
                 arg_addition = [other_arg for other_arg in remaining_other if other_arg.id_matches(arg)]
@@ -149,14 +150,17 @@
 
         if 'gdb_dev' in section:
             result = replace(result, gdb_dev=section['gdb_dev'])
 
         if 'halted' in section:
             result = replace(result, halted=config_parser.getboolean('general', 'halted'))
 
+        if 'memory' in section:
+            result = replace(result, memory=section['memory'])
+
         return result
 
     return Layer(
         general=read_general_settings(),
         arguments=read_arguments()
     )
```

### Comparing `qemu-runner-1.3.2/src/qemu_runner/layer_locator.py` & `qemu-runner-1.3.3/src/qemu_runner/layer_locator.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.2/src/qemu_runner/make_runner/__main__.py` & `qemu-runner-1.3.3/src/qemu_runner/make_runner/__main__.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.2/src/qemu_runner/make_runner/make.py` & `qemu-runner-1.3.3/src/qemu_runner/make_runner/make.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.2/src/qemu_runner/make_runner/runner.py` & `qemu-runner-1.3.3/src/qemu_runner/make_runner/runner.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.2/src/qemu_runner/variable_resolution.py` & `qemu-runner-1.3.3/src/qemu_runner/variable_resolution.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.2/src/qemu_runner.egg-info/PKG-INFO` & `qemu-runner-1.3.3/src/qemu_runner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qemu-runner
-Version: 1.3.2
+Version: 1.3.3
 Summary: Create self-contained wrappers around QEMU to hide & share long command-line invocations
 Home-page: https://github.com/Novakov/qemu-runner
 Author: Maciej Nowak
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `qemu-runner-1.3.2/src/qemu_runner.egg-info/SOURCES.txt` & `qemu-runner-1.3.3/src/qemu_runner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.2/tests/test_find_layer.py` & `qemu-runner-1.3.3/tests/test_find_layer.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.2/tests/test_find_qemu.py` & `qemu-runner-1.3.3/tests/test_find_qemu.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.2/tests/test_layer.py` & `qemu-runner-1.3.3/tests/test_layer.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,14 +37,29 @@
     (Layer(MY_ENGINE), Layer(MY_ENGINE2), Layer(MY_ENGINE2)),
     (
         Layer(GeneralSettings(engine='e1', kernel='k1', kernel_cmdline='c1', halted=False, gdb=False, gdb_dev='gdb1')),
         Layer(GeneralSettings(engine='e2', kernel='k2', kernel_cmdline='c2', halted=True, gdb=True, gdb_dev='gdb2')),
         Layer(GeneralSettings(engine='e2', kernel='k2', kernel_cmdline='c1 c2', halted=True, gdb=True, gdb_dev='gdb2')),
     ),
     (
+        Layer(GeneralSettings(memory='12')),
+        Layer(GeneralSettings()),
+        Layer(GeneralSettings(memory='12')),
+    ),
+    (
+        Layer(GeneralSettings(memory='12')),
+        Layer(GeneralSettings(memory='24')),
+        Layer(GeneralSettings(memory='24')),
+    ),
+    (
+        Layer(GeneralSettings()),
+        Layer(GeneralSettings(memory='24')),
+        Layer(GeneralSettings(memory='24')),
+    ),
+    (
         Layer(MY_ENGINE, [Argument('device', 'd1', {'id': 'id1', 'p': 'a'})]),
         Layer(MY_ENGINE, [Argument('chardev', 'c1', {'id': 'id2', 'b': 'a'})]),
         Layer(MY_ENGINE, [
             Argument('device', 'd1', {'id': 'id1', 'p': 'a'}),
             Argument('chardev', 'c1', {'id': 'id2', 'b': 'a'})
         ]),
     ),
```

### Comparing `qemu-runner-1.3.2/tests/test_layer_cmdline.py` & `qemu-runner-1.3.3/tests/test_layer_cmdline.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.2/tests/test_layer_equality.py` & `qemu-runner-1.3.3/tests/test_layer_equality.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.2/tests/test_layer_parsing.py` & `qemu-runner-1.3.3/tests/test_layer_parsing.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,21 @@
             engine = my-engine
             """,
             Layer(general=GeneralSettings(engine='my-engine'))
     ),
     (
             """
             [general]
+            memory = 128M
+            """,
+            Layer(general=GeneralSettings(memory='128M'))
+    ),
+    (
+            """
+            [general]
             engine = my-engine
             kernel = my-kernel.elf
             cmdline = a b c
             """,
             Layer(general=GeneralSettings(engine='my-engine', kernel='my-kernel.elf', kernel_cmdline='a b c'))
     ),
     (
```

### Comparing `qemu-runner-1.3.2/tests/test_qemu_argument.py` & `qemu-runner-1.3.3/tests/test_qemu_argument.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.2/tests/test_qemu_argument_equality.py` & `qemu-runner-1.3.3/tests/test_qemu_argument_equality.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.2/tests/test_runner_flow.py` & `qemu-runner-1.3.3/tests/test_runner_flow.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,39 +41,57 @@
     actual_args = cp.stdout.splitlines(keepends=False)
     return [
         actual_args[0].lower().replace('\\', '/'),
         *actual_args[1:],
     ]
 
 
-def test_runner_flow(tmp_path: Path):
+@pytest.fixture()
+def test_layer(tmp_path: Path) -> Path:
+    with open(tmp_path / 'test-layer', 'w') as f:
+        f.write("""
+        [general]
+        engine = qemu-system-arm
+        memory = 128M
+        
+        [machine]
+        @ = virt_cortex_m
+        flash_kb = 1024
+        """)
+
+    return tmp_path / 'test-layer'
+
+
+def test_runner_flow(tmp_path: Path, test_layer: Path):
     engine = place_echo_args(tmp_path / 'qemu' / 'qemu-system-arm')
 
-    run_make_runner('-l', 'virt-cortex-m.ini', '-o', tmp_path / 'test.pyz', cwd=tmp_path)
+    run_make_runner('-l', test_layer, '-o', tmp_path / 'test.pyz', cwd=tmp_path)
     with with_cwd(tmp_path):
         cmdline = capture_runner_cmdline(tmp_path / 'test.pyz', 'abc.elf', 'arg1', 'arg2')
 
     assert cmdline == [
         engine,
         '-machine', 'virt_cortex_m,flash_kb=1024',
+        '-m', '128M',
         '-kernel',  str(tmp_path / 'abc.elf'),
         '-append', 'arg1 arg2'
     ]
 
 
-def test_runner_flow_no_args(tmp_path: Path):
+def test_runner_flow_no_args(tmp_path: Path, test_layer: Path):
     engine = place_echo_args(tmp_path / 'qemu' / 'qemu-system-arm')
 
-    run_make_runner('-l', 'virt-cortex-m.ini', '-o', tmp_path / 'test.pyz', cwd=tmp_path)
+    run_make_runner('-l', test_layer, '-o', tmp_path / 'test.pyz', cwd=tmp_path)
     with with_cwd(tmp_path):
         cmdline = capture_runner_cmdline(tmp_path / 'test.pyz', 'abc.elf')
 
     assert cmdline == [
         engine,
         '-machine', 'virt_cortex_m,flash_kb=1024',
+        '-m', '128M',
         '-kernel',  str(tmp_path / 'abc.elf'),
     ]
 
 
 def assert_arg_set_in_cmdline(arg_set: List[str], cmdline: List[str]):
     if len(arg_set) == 1:
         assert arg_set[0] in cmdline
@@ -85,86 +103,87 @@
 
 
 @pytest.mark.parametrize(('runner_args', 'qemu_args'), [
     (['--halted'], [['-S']]),
     (['--debug'], [['-s']]),
     (['--debug', '--debug-listen', 'abc'], [['-gdb', 'abc']]),
 ])
-def test_builtin_args(tmpdir: Path, runner_args: List[str], qemu_args: List[List[str]]):
+def test_builtin_args(tmpdir: Path, runner_args: List[str], qemu_args: List[List[str]], test_layer: Path):
     place_echo_args(tmpdir / 'qemu' / 'qemu-system-arm')
 
-    run_make_runner('-l', 'virt-cortex-m.ini', '-o', tmpdir / 'test.pyz', cwd=tmpdir)
+    run_make_runner('-l', test_layer, '-o', tmpdir / 'test.pyz', cwd=tmpdir)
     cmdline = capture_runner_cmdline(tmpdir / 'test.pyz', *runner_args, 'abc.elf', 'arg1', 'arg2')
 
     for arg_set in qemu_args:
         assert_arg_set_in_cmdline(arg_set, cmdline)
 
 
-def test_debug_listen_no_debug(tmp_path: Path):
+def test_debug_listen_no_debug(tmp_path: Path, test_layer: Path):
     place_echo_args(tmp_path / 'qemu' / 'qemu-system-arm')
 
-    run_make_runner('-l', 'virt-cortex-m.ini', '-o', tmp_path / 'test.pyz', cwd=tmp_path)
+    run_make_runner('-l', test_layer, '-o', tmp_path / 'test.pyz', cwd=tmp_path)
     cmdline = capture_runner_cmdline(tmp_path / 'test.pyz', '--debug-listen', 'MARK-DEBUG', 'abc.elf', 'arg1', 'arg2')
 
     assert 'MARK-DEBUG' not in cmdline
 
 
-def test_layers_are_embbedded_in_runner(tmp_path: Path):
+def test_layers_are_embbedded_in_runner(tmp_path: Path, test_layer: Path):
     place_echo_args(tmp_path / 'qemu' / 'qemu-system-arm')
 
     with open(tmp_path / 'my-layer.ini', 'w') as f:
         f.write("""
         [device:test_id]
         @=test_device
         addr=12
         """)
 
-    run_make_runner('-l', 'virt-cortex-m.ini', 'my-layer.ini', '-o', tmp_path / 'test.pyz', cwd=tmp_path)
+    run_make_runner('-l', test_layer, 'my-layer.ini', '-o', tmp_path / 'test.pyz', cwd=tmp_path)
 
     os.unlink(tmp_path / 'my-layer.ini')
 
     cmdline = capture_runner_cmdline(tmp_path / 'test.pyz', 'abc.elf', 'arg1', 'arg2')
 
     assert_arg_set_in_cmdline(['-device', 'test_device,id=test_id,addr=12'], cmdline)
 
 
-def test_extract_base_command_line_with_kernel(tmp_path: Path):
+def test_extract_base_command_line_with_kernel(tmp_path: Path, test_layer: Path):
     with open(tmp_path / 'my-layer.ini', 'w') as f:
         f.write("""
         [device:test_id]
         @=test_device
         addr=12
         """)
 
-    run_make_runner('-l', 'virt-cortex-m.ini', 'my-layer.ini', '-o', tmp_path / 'test.pyz', cwd=tmp_path)
+    run_make_runner('-l', test_layer, 'my-layer.ini', '-o', tmp_path / 'test.pyz', cwd=tmp_path)
 
     with with_env({'QEMU_DEV': 'my-qemu'}), with_cwd(tmp_path):
         cp = execute_runner(tmp_path / 'test.pyz', ['--debug', '--dry-run', 'abc.elf', 'a', 'b', 'c'])
 
     kernel_path = tmp_path / 'abc.elf'
 
     assert cp.stdout.strip().replace("-kernel '", '-kernel ').replace("' -append", ' -append') == (
-            "my-qemu -machine virt_cortex_m,flash_kb=1024 -device test_device,id=test_id,addr=12 " +
+            "my-qemu -machine virt_cortex_m,flash_kb=1024 -device test_device,id=test_id,addr=12 -m 128M " +
             f"-s -kernel {kernel_path} -append 'a b c'")
 
 
-def test_extract_base_command_line_no_kernel(tmp_path: Path):
+def test_extract_base_command_line_no_kernel(tmp_path: Path, test_layer: Path):
     with open(tmp_path / 'my-layer.ini', 'w') as f:
         f.write("""
         [device:test_id]
         @=test_device
         addr=12
         """)
 
-    run_make_runner('-l', 'virt-cortex-m.ini', 'my-layer.ini', '-o', tmp_path / 'test.pyz', cwd=tmp_path)
+    run_make_runner('-l', test_layer, 'my-layer.ini', '-o', tmp_path / 'test.pyz', cwd=tmp_path)
 
     with with_env({'QEMU_DEV': 'my-qemu'}):
         cp = execute_runner(tmp_path / 'test.pyz', ['--debug', '--dry-run'])
 
-    assert cp.stdout.strip() == "my-qemu -machine virt_cortex_m,flash_kb=1024 -device test_device,id=test_id,addr=12 -s"
+    assert cp.stdout.strip() == ("my-qemu -machine virt_cortex_m,flash_kb=1024 -device test_device,id=test_id,addr=12 " +
+                                 "-m 128M -s")
 
 
 def test_derive_runner(tmp_path: Path):
     engine = place_echo_args(tmp_path / 'qemu' / 'my-qemu')
 
     with open(tmp_path / 'layer1.ini', 'w') as f:
         f.write("""
@@ -352,36 +371,36 @@
     # ['--inspect', '--debug'],
     # ['--inspect', '--debug-listen', 'abc'],
 
     ['--halted'],
     ['--debug'],
     ['--debug-listen', 'abc']
 ])
-def test_invalid_args(tmp_path: Path, args: List[str]) -> None:
-    run_make_runner('-l', 'virt-cortex-m.ini', '-o', tmp_path / 'test.pyz', cwd=tmp_path)
+def test_invalid_args(tmp_path: Path, args: List[str], test_layer: Path) -> None:
+    run_make_runner('-l', test_layer, '-o', tmp_path / 'test.pyz', cwd=tmp_path)
 
     cp = execute_runner(tmp_path / 'test.pyz', args, check=False, cwd=tmp_path)
     assert 'test.pyz: error:' in cp.stderr
     assert cp.returncode != 0
 
 
-def test_explicit_qemu_dir(tmp_path: Path) -> None:
+def test_explicit_qemu_dir(tmp_path: Path, test_layer: Path) -> None:
     engine = place_echo_args(tmp_path / 'my-qemu' / 'qemu-system-arm')
 
-    run_make_runner('-l', 'virt-cortex-m.ini', '-o', tmp_path / 'test.pyz', cwd=tmp_path)
+    run_make_runner('-l', test_layer, '-o', tmp_path / 'test.pyz', cwd=tmp_path)
 
     args = capture_runner_cmdline(tmp_path / 'test.pyz', '--qemu-dir', tmp_path / 'my-qemu', 'abc.elf')
 
     assert args[0] == engine
 
 
-def test_explicit_qemu_executable(tmp_path: Path) -> None:
+def test_explicit_qemu_executable(tmp_path: Path, test_layer: Path) -> None:
     engine = place_echo_args(tmp_path / 'my-qemu' / 'qemu')
 
-    run_make_runner('-l', 'virt-cortex-m.ini', '-o', tmp_path / 'test.pyz', cwd=tmp_path)
+    run_make_runner('-l', test_layer, '-o', tmp_path / 'test.pyz', cwd=tmp_path)
 
     args = capture_runner_cmdline(tmp_path / 'test.pyz', '--qemu', engine, 'abc.elf')
 
     assert args[0] == engine
 
 
 def test_resolve_kernel_dir_to_absolute_path(tmp_path: Path) -> None:
```

### Comparing `qemu-runner-1.3.2/tests/test_utllities.py` & `qemu-runner-1.3.3/tests/test_utllities.py`

 * *Files identical despite different names*

### Comparing `qemu-runner-1.3.2/tests/test_venv.py` & `qemu-runner-1.3.3/tests/test_venv.py`

 * *Files identical despite different names*

