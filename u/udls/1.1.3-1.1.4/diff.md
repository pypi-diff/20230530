# Comparing `tmp/udls-1.1.3.tar.gz` & `tmp/udls-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "udls-1.1.3.tar", last modified: Fri May 19 11:55:01 2023, max compression
+gzip compressed data, was "udls-1.1.4.tar", last modified: Tue May 30 09:36:05 2023, max compression
```

## Comparing `udls-1.1.3.tar` & `udls-1.1.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:55:01.629091 udls-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-19 11:54:48.000000 udls-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-19 11:54:48.000000 udls-1.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-19 11:55:01.629091 udls-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 11:54:48.000000 udls-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-19 11:54:48.000000 udls-1.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 11:55:01.629091 udls-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-19 11:54:48.000000 udls-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:55:01.625091 udls-1.1.3/udls/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-19 11:54:48.000000 udls-1.1.3/udls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-19 11:54:48.000000 udls-1.1.3/udls/audio_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-19 11:54:48.000000 udls-1.1.3/udls/audio_example_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-19 11:54:48.000000 udls-1.1.3/udls/base_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-19 11:54:48.000000 udls-1.1.3/udls/duration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:55:01.629091 udls-1.1.3/udls/generated/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-19 11:54:48.000000 udls-1.1.3/udls/generated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-05-19 11:54:48.000000 udls-1.1.3/udls/generated/audio_example_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-19 11:54:48.000000 udls-1.1.3/udls/resample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-19 11:54:48.000000 udls-1.1.3/udls/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-05-19 11:54:48.000000 udls-1.1.3/udls/simple_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-19 11:54:48.000000 udls-1.1.3/udls/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 11:55:01.629091 udls-1.1.3/udls.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-19 11:55:01.000000 udls-1.1.3/udls.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-19 11:55:01.000000 udls-1.1.3/udls.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 11:55:01.000000 udls-1.1.3/udls.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-19 11:55:01.000000 udls-1.1.3/udls.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-19 11:55:01.000000 udls-1.1.3/udls.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-19 11:55:01.000000 udls-1.1.3/udls.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:36:05.689012 udls-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-30 09:35:52.000000 udls-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-30 09:35:52.000000 udls-1.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-30 09:36:05.689012 udls-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 09:35:52.000000 udls-1.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-30 09:35:52.000000 udls-1.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 09:36:05.689012 udls-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-30 09:35:52.000000 udls-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:36:05.689012 udls-1.1.4/udls/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-30 09:35:52.000000 udls-1.1.4/udls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-30 09:35:52.000000 udls-1.1.4/udls/audio_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-30 09:35:52.000000 udls-1.1.4/udls/audio_example_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-30 09:35:52.000000 udls-1.1.4/udls/base_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-30 09:35:52.000000 udls-1.1.4/udls/duration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:36:05.689012 udls-1.1.4/udls/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-30 09:35:52.000000 udls-1.1.4/udls/generated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-05-30 09:35:52.000000 udls-1.1.4/udls/generated/audio_example_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-30 09:35:52.000000 udls-1.1.4/udls/resample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-30 09:35:52.000000 udls-1.1.4/udls/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-05-30 09:35:52.000000 udls-1.1.4/udls/simple_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-30 09:35:52.000000 udls-1.1.4/udls/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:36:05.689012 udls-1.1.4/udls.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-30 09:36:05.000000 udls-1.1.4/udls.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-30 09:36:05.000000 udls-1.1.4/udls.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 09:36:05.000000 udls-1.1.4/udls.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-30 09:36:05.000000 udls-1.1.4/udls.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-30 09:36:05.000000 udls-1.1.4/udls.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-30 09:36:05.000000 udls-1.1.4/udls.egg-info/top_level.txt
```

### Comparing `udls-1.1.3/LICENSE` & `udls-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `udls-1.1.3/setup.py` & `udls-1.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `udls-1.1.3/udls/audio_example.py` & `udls-1.1.4/udls/audio_example.py`

 * *Files identical despite different names*

### Comparing `udls-1.1.3/udls/audio_example_dataset.py` & `udls-1.1.4/udls/audio_example_dataset.py`

 * *Files identical despite different names*

### Comparing `udls-1.1.3/udls/base_dataset.py` & `udls-1.1.4/udls/base_dataset.py`

 * *Files identical despite different names*

### Comparing `udls-1.1.3/udls/generated/audio_example_pb2.py` & `udls-1.1.4/udls/generated/audio_example_pb2.py`

 * *Files identical despite different names*

### Comparing `udls-1.1.3/udls/resample.py` & `udls-1.1.4/udls/resample.py`

 * *Files identical despite different names*

### Comparing `udls-1.1.3/udls/serve.py` & `udls-1.1.4/udls/serve.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,17 +64,17 @@
     @app.route("/get/<index>")
     def get_element(index: int):
         index = int(index)
         if index >= db_length:
             return "invalid index"
 
         with env.begin() as txn:
-            ae = AudioExample(txn.get(keys[index]))
+            ae = txn.get(keys[index])
 
-        ae = base64.b64encode(bytes(ae))
+        ae = base64.b64encode(ae)
 
         return ae
 
     @app.route("/")
     def root():
         return (f"<h1>UDLS remote serving</h1>"
                 f"Current dataset: {os.path.abspath(args.db_path)}")
```

### Comparing `udls-1.1.3/udls/simple_dataset.py` & `udls-1.1.4/udls/simple_dataset.py`

 * *Files identical despite different names*

### Comparing `udls-1.1.3/udls/transforms.py` & `udls-1.1.4/udls/transforms.py`

 * *Files identical despite different names*

