# Comparing `tmp/playmolecule-1.8.4.1.tar.gz` & `tmp/playmolecule-1.8.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playmolecule-1.8.4.1.tar", last modified: Tue May 30 13:47:46 2023, max compression
+gzip compressed data, was "playmolecule-1.8.4.2.tar", last modified: Tue May 30 13:51:03 2023, max compression
```

## Comparing `playmolecule-1.8.4.1.tar` & `playmolecule-1.8.4.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:46.875412 playmolecule-1.8.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-30 13:47:28.000000 playmolecule-1.8.4.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-30 13:47:28.000000 playmolecule-1.8.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-30 13:47:46.875412 playmolecule-1.8.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-30 13:47:28.000000 playmolecule-1.8.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:46.875412 playmolecule-1.8.4.1/playmolecule/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-30 13:47:28.000000 playmolecule-1.8.4.1/playmolecule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-30 13:47:28.000000 playmolecule-1.8.4.1/playmolecule/_test_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-30 13:47:46.875412 playmolecule-1.8.4.1/playmolecule/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-30 13:47:28.000000 playmolecule-1.8.4.1/playmolecule/config.ini
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-30 13:47:28.000000 playmolecule-1.8.4.1/playmolecule/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-05-30 13:47:28.000000 playmolecule-1.8.4.1/playmolecule/datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    33412 2023-05-30 13:47:28.000000 playmolecule-1.8.4.1/playmolecule/devutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-05-30 13:47:28.000000 playmolecule-1.8.4.1/playmolecule/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-05-30 13:47:28.000000 playmolecule-1.8.4.1/playmolecule/jsonlogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-05-30 13:47:28.000000 playmolecule-1.8.4.1/playmolecule/local.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-30 13:47:28.000000 playmolecule-1.8.4.1/playmolecule/logging.ini
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-30 13:47:28.000000 playmolecule-1.8.4.1/playmolecule/playqueue.py
--rw-r--r--   0 runner    (1001) docker     (123)    33414 2023-05-30 13:47:28.000000 playmolecule-1.8.4.1/playmolecule/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-05-30 13:47:28.000000 playmolecule-1.8.4.1/playmolecule/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:46.875412 playmolecule-1.8.4.1/playmolecule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-30 13:47:46.000000 playmolecule-1.8.4.1/playmolecule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-30 13:47:46.000000 playmolecule-1.8.4.1/playmolecule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:47:46.000000 playmolecule-1.8.4.1/playmolecule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:47:46.000000 playmolecule-1.8.4.1/playmolecule.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-30 13:47:46.000000 playmolecule-1.8.4.1/playmolecule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 13:47:46.000000 playmolecule-1.8.4.1/playmolecule.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-30 13:47:28.000000 playmolecule-1.8.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 13:47:46.875412 playmolecule-1.8.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-30 13:47:28.000000 playmolecule-1.8.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:47:46.875412 playmolecule-1.8.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-30 13:47:28.000000 playmolecule-1.8.4.1/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-30 13:47:28.000000 playmolecule-1.8.4.1/tests/test_app_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-30 13:47:28.000000 playmolecule-1.8.4.1/tests/test_datacenter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:51:03.938694 playmolecule-1.8.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-30 13:50:45.000000 playmolecule-1.8.4.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-30 13:50:45.000000 playmolecule-1.8.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-30 13:51:03.938694 playmolecule-1.8.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-30 13:50:45.000000 playmolecule-1.8.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:51:03.938694 playmolecule-1.8.4.2/playmolecule/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-30 13:50:45.000000 playmolecule-1.8.4.2/playmolecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-30 13:50:45.000000 playmolecule-1.8.4.2/playmolecule/_test_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-30 13:51:03.938694 playmolecule-1.8.4.2/playmolecule/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-30 13:50:45.000000 playmolecule-1.8.4.2/playmolecule/config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-30 13:50:45.000000 playmolecule-1.8.4.2/playmolecule/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-05-30 13:50:45.000000 playmolecule-1.8.4.2/playmolecule/datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33451 2023-05-30 13:50:45.000000 playmolecule-1.8.4.2/playmolecule/devutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-05-30 13:50:45.000000 playmolecule-1.8.4.2/playmolecule/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-05-30 13:50:45.000000 playmolecule-1.8.4.2/playmolecule/jsonlogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-05-30 13:50:45.000000 playmolecule-1.8.4.2/playmolecule/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-30 13:50:45.000000 playmolecule-1.8.4.2/playmolecule/logging.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-30 13:50:45.000000 playmolecule-1.8.4.2/playmolecule/playqueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33414 2023-05-30 13:50:45.000000 playmolecule-1.8.4.2/playmolecule/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-05-30 13:50:45.000000 playmolecule-1.8.4.2/playmolecule/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:51:03.938694 playmolecule-1.8.4.2/playmolecule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-30 13:51:03.000000 playmolecule-1.8.4.2/playmolecule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-30 13:51:03.000000 playmolecule-1.8.4.2/playmolecule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:51:03.000000 playmolecule-1.8.4.2/playmolecule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:51:03.000000 playmolecule-1.8.4.2/playmolecule.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-30 13:51:03.000000 playmolecule-1.8.4.2/playmolecule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 13:51:03.000000 playmolecule-1.8.4.2/playmolecule.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-30 13:50:45.000000 playmolecule-1.8.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 13:51:03.938694 playmolecule-1.8.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-30 13:50:45.000000 playmolecule-1.8.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:51:03.938694 playmolecule-1.8.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-30 13:50:45.000000 playmolecule-1.8.4.2/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-30 13:50:45.000000 playmolecule-1.8.4.2/tests/test_app_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-30 13:50:45.000000 playmolecule-1.8.4.2/tests/test_datacenter.py
```

### Comparing `playmolecule-1.8.4.1/LICENSE.md` & `playmolecule-1.8.4.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.4.1/PKG-INFO` & `playmolecule-1.8.4.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playmolecule
-Version: 1.8.4.1
+Version: 1.8.4.2
 Summary: PlayMolecule python API
 Author-email: Acellera <info@acellera.com>
 Project-URL: Homepage, https://github.com/Acellera/playmolecule-python-api
 Project-URL: Bug Tracker, https://github.com/Acellera/playmolecule-python-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
```

### Comparing `playmolecule-1.8.4.1/playmolecule/__init__.py` & `playmolecule-1.8.4.2/playmolecule/__init__.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.4.1/playmolecule/_test_funcs.py` & `playmolecule-1.8.4.2/playmolecule/_test_funcs.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.4.1/playmolecule/config.py` & `playmolecule-1.8.4.2/playmolecule/config.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.4.1/playmolecule/datacenter.py` & `playmolecule-1.8.4.2/playmolecule/datacenter.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.4.1/playmolecule/devutils.py` & `playmolecule-1.8.4.2/playmolecule/devutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -520,21 +520,23 @@
         input_args[name] = newvals
 
     return input_args
 
 
 def report_alive(outdir):
     from datetime import datetime
+    import time
 
     os.makedirs(outdir, exist_ok=True)
 
     while True:
         current_date = datetime.now()
         with open(os.path.join(outdir, ".pm.alive"), "w") as f:
             f.write(current_date.isoformat())
+        time.sleep(30)
 
 
 def app_wrapper2(
     func,
     cli_arg_str=None,
     token=None,
     execid=None,
```

### Comparing `playmolecule-1.8.4.1/playmolecule/job.py` & `playmolecule-1.8.4.2/playmolecule/job.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.4.1/playmolecule/jsonlogger.py` & `playmolecule-1.8.4.2/playmolecule/jsonlogger.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.4.1/playmolecule/local.py` & `playmolecule-1.8.4.2/playmolecule/local.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.4.1/playmolecule/playqueue.py` & `playmolecule-1.8.4.2/playmolecule/playqueue.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.4.1/playmolecule/session.py` & `playmolecule-1.8.4.2/playmolecule/session.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.4.1/playmolecule/utils.py` & `playmolecule-1.8.4.2/playmolecule/utils.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.4.1/playmolecule.egg-info/PKG-INFO` & `playmolecule-1.8.4.2/playmolecule.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playmolecule
-Version: 1.8.4.1
+Version: 1.8.4.2
 Summary: PlayMolecule python API
 Author-email: Acellera <info@acellera.com>
 Project-URL: Homepage, https://github.com/Acellera/playmolecule-python-api
 Project-URL: Bug Tracker, https://github.com/Acellera/playmolecule-python-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
```

### Comparing `playmolecule-1.8.4.1/playmolecule.egg-info/SOURCES.txt` & `playmolecule-1.8.4.2/playmolecule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.4.1/pyproject.toml` & `playmolecule-1.8.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.4.1/tests/test.py` & `playmolecule-1.8.4.2/tests/test.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.4.1/tests/test_app_wrapper.py` & `playmolecule-1.8.4.2/tests/test_app_wrapper.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.4.1/tests/test_datacenter.py` & `playmolecule-1.8.4.2/tests/test_datacenter.py`

 * *Files identical despite different names*

