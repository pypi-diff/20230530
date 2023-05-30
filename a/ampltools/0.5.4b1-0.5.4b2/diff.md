# Comparing `tmp/ampltools-0.5.4b1.tar.gz` & `tmp/ampltools-0.5.4b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ampltools-0.5.4b1.tar", last modified: Tue May 30 11:18:17 2023, max compression
+gzip compressed data, was "ampltools-0.5.4b2.tar", last modified: Tue May 30 11:29:03 2023, max compression
```

## Comparing `ampltools-0.5.4b1.tar` & `ampltools-0.5.4b2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-05-30 11:18:17.619554 ampltools-0.5.4b1/
--rw-r--r--   0 fdabrandao   (501) staff       (20)     2822 2023-05-03 11:08:48.000000 ampltools-0.5.4b1/CHANGELOG.md
--rw-r--r--   0 fdabrandao   (501) staff       (20)     1522 2023-03-08 15:44:27.000000 ampltools-0.5.4b1/LICENSE
--rw-r--r--   0 fdabrandao   (501) staff       (20)       57 2023-03-08 15:44:27.000000 ampltools-0.5.4b1/MANIFEST.in
--rw-r--r--   0 fdabrandao   (501) staff       (20)     1282 2023-05-30 11:18:17.619113 ampltools-0.5.4b1/PKG-INFO
--rw-r--r--   0 fdabrandao   (501) staff       (20)      446 2023-03-08 15:44:27.000000 ampltools-0.5.4b1/README.md
-drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-05-30 11:18:17.610575 ampltools-0.5.4b1/ampltools/
--rw-r--r--   0 fdabrandao   (501) staff       (20)      409 2023-05-30 11:18:14.000000 ampltools-0.5.4b1/ampltools/__init__.py
-drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-05-30 11:18:17.616049 ampltools-0.5.4b1/ampltools/modules/
--rw-r--r--   0 fdabrandao   (501) staff       (20)      443 2023-05-30 11:18:14.000000 ampltools-0.5.4b1/ampltools/modules/__init__.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)       93 2023-03-08 15:44:27.000000 ampltools-0.5.4b1/ampltools/modules/__main__.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)    12683 2023-05-03 11:08:48.000000 ampltools-0.5.4b1/ampltools/modules/amplpypi.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     3723 2023-03-09 15:01:44.000000 ampltools-0.5.4b1/ampltools/modules/commands.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     5683 2023-05-30 11:16:46.000000 ampltools-0.5.4b1/ampltools/notebooks.py
-drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-05-30 11:18:17.618606 ampltools-0.5.4b1/ampltools/tests/
--rw-r--r--   0 fdabrandao   (501) staff       (20)      433 2023-03-08 15:44:27.000000 ampltools-0.5.4b1/ampltools/tests/TestBase.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)       24 2023-03-08 15:44:27.000000 ampltools-0.5.4b1/ampltools/tests/__init__.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)      286 2023-03-08 15:44:27.000000 ampltools-0.5.4b1/ampltools/tests/__main__.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     3566 2023-03-08 15:44:27.000000 ampltools-0.5.4b1/ampltools/tests/test_install.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     1951 2023-03-08 15:44:27.000000 ampltools-0.5.4b1/ampltools/tests/test_load.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     2411 2023-03-13 18:25:11.000000 ampltools-0.5.4b1/ampltools/tests/test_preload.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     1751 2023-03-08 15:44:27.000000 ampltools-0.5.4b1/ampltools/tests/test_run.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     3228 2023-03-09 15:37:57.000000 ampltools-0.5.4b1/ampltools/utils.py
-drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-05-30 11:18:17.613988 ampltools-0.5.4b1/ampltools.egg-info/
--rw-r--r--   0 fdabrandao   (501) staff       (20)     1282 2023-05-30 11:18:17.000000 ampltools-0.5.4b1/ampltools.egg-info/PKG-INFO
--rw-r--r--   0 fdabrandao   (501) staff       (20)      621 2023-05-30 11:18:17.000000 ampltools-0.5.4b1/ampltools.egg-info/SOURCES.txt
--rw-r--r--   0 fdabrandao   (501) staff       (20)        1 2023-05-30 11:18:17.000000 ampltools-0.5.4b1/ampltools.egg-info/dependency_links.txt
--rw-r--r--   0 fdabrandao   (501) staff       (20)        9 2023-05-30 11:18:17.000000 ampltools-0.5.4b1/ampltools.egg-info/requires.txt
--rw-r--r--   0 fdabrandao   (501) staff       (20)       10 2023-05-30 11:18:17.000000 ampltools-0.5.4b1/ampltools.egg-info/top_level.txt
--rw-r--r--   0 fdabrandao   (501) staff       (20)        8 2023-03-08 15:44:27.000000 ampltools-0.5.4b1/requirements.txt
--rw-r--r--   0 fdabrandao   (501) staff       (20)       38 2023-05-30 11:18:17.619645 ampltools-0.5.4b1/setup.cfg
--rw-r--r--   0 fdabrandao   (501) staff       (20)     1717 2023-05-30 11:18:14.000000 ampltools-0.5.4b1/setup.py
+drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-05-30 11:29:03.900523 ampltools-0.5.4b2/
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     2822 2023-05-03 11:08:48.000000 ampltools-0.5.4b2/CHANGELOG.md
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     1522 2023-03-08 15:44:27.000000 ampltools-0.5.4b2/LICENSE
+-rw-r--r--   0 fdabrandao   (501) staff       (20)       57 2023-03-08 15:44:27.000000 ampltools-0.5.4b2/MANIFEST.in
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     1282 2023-05-30 11:29:03.900143 ampltools-0.5.4b2/PKG-INFO
+-rw-r--r--   0 fdabrandao   (501) staff       (20)      446 2023-03-08 15:44:27.000000 ampltools-0.5.4b2/README.md
+drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-05-30 11:29:03.889929 ampltools-0.5.4b2/ampltools/
+-rw-r--r--   0 fdabrandao   (501) staff       (20)      409 2023-05-30 11:29:00.000000 ampltools-0.5.4b2/ampltools/__init__.py
+drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-05-30 11:29:03.895957 ampltools-0.5.4b2/ampltools/modules/
+-rw-r--r--   0 fdabrandao   (501) staff       (20)      443 2023-05-30 11:29:00.000000 ampltools-0.5.4b2/ampltools/modules/__init__.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)       93 2023-03-08 15:44:27.000000 ampltools-0.5.4b2/ampltools/modules/__main__.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)    12683 2023-05-03 11:08:48.000000 ampltools-0.5.4b2/ampltools/modules/amplpypi.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     3723 2023-03-09 15:01:44.000000 ampltools-0.5.4b2/ampltools/modules/commands.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     5737 2023-05-30 11:28:23.000000 ampltools-0.5.4b2/ampltools/notebooks.py
+drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-05-30 11:29:03.899383 ampltools-0.5.4b2/ampltools/tests/
+-rw-r--r--   0 fdabrandao   (501) staff       (20)      433 2023-03-08 15:44:27.000000 ampltools-0.5.4b2/ampltools/tests/TestBase.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)       24 2023-03-08 15:44:27.000000 ampltools-0.5.4b2/ampltools/tests/__init__.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)      286 2023-03-08 15:44:27.000000 ampltools-0.5.4b2/ampltools/tests/__main__.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     3566 2023-03-08 15:44:27.000000 ampltools-0.5.4b2/ampltools/tests/test_install.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     1951 2023-03-08 15:44:27.000000 ampltools-0.5.4b2/ampltools/tests/test_load.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     2411 2023-03-13 18:25:11.000000 ampltools-0.5.4b2/ampltools/tests/test_preload.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     1751 2023-03-08 15:44:27.000000 ampltools-0.5.4b2/ampltools/tests/test_run.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     3228 2023-03-09 15:37:57.000000 ampltools-0.5.4b2/ampltools/utils.py
+drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-05-30 11:29:03.892600 ampltools-0.5.4b2/ampltools.egg-info/
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     1282 2023-05-30 11:29:03.000000 ampltools-0.5.4b2/ampltools.egg-info/PKG-INFO
+-rw-r--r--   0 fdabrandao   (501) staff       (20)      621 2023-05-30 11:29:03.000000 ampltools-0.5.4b2/ampltools.egg-info/SOURCES.txt
+-rw-r--r--   0 fdabrandao   (501) staff       (20)        1 2023-05-30 11:29:03.000000 ampltools-0.5.4b2/ampltools.egg-info/dependency_links.txt
+-rw-r--r--   0 fdabrandao   (501) staff       (20)        9 2023-05-30 11:29:03.000000 ampltools-0.5.4b2/ampltools.egg-info/requires.txt
+-rw-r--r--   0 fdabrandao   (501) staff       (20)       10 2023-05-30 11:29:03.000000 ampltools-0.5.4b2/ampltools.egg-info/top_level.txt
+-rw-r--r--   0 fdabrandao   (501) staff       (20)        8 2023-03-08 15:44:27.000000 ampltools-0.5.4b2/requirements.txt
+-rw-r--r--   0 fdabrandao   (501) staff       (20)       38 2023-05-30 11:29:03.900607 ampltools-0.5.4b2/setup.cfg
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     1717 2023-05-30 11:29:00.000000 ampltools-0.5.4b2/setup.py
```

### Comparing `ampltools-0.5.4b1/CHANGELOG.md` & `ampltools-0.5.4b2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.4b1/LICENSE` & `ampltools-0.5.4b2/LICENSE`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.4b1/PKG-INFO` & `ampltools-0.5.4b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ampltools
-Version: 0.5.4b1
+Version: 0.5.4b2
 Summary: AMPL Python Tools
 Home-page: http://ampl.com/
 Author: Filipe Brandão
 Author-email: fdabrandao@ampl.com
 License: BSD-3
 Download-URL: https://github.com/ampl/amplpy/tree/master/ampltools
 Description:
```

### Comparing `ampltools-0.5.4b1/ampltools/modules/amplpypi.py` & `ampltools-0.5.4b2/ampltools/modules/amplpypi.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.4b1/ampltools/modules/commands.py` & `ampltools-0.5.4b2/ampltools/modules/commands.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.4b1/ampltools/notebooks.py` & `ampltools-0.5.4b2/ampltools/notebooks.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,17 @@
         ampl_lic = os.environ.get("AMPL_LICFILE", None)
         if ampl_lic is not None and platform is None:
             print("License license at {}.".format(ampl_lic))
     with version:
         if check_callback:
             check_callback()
 
-    uuid_input = widgets.Text(description="License UUID:")
+    uuid_input = widgets.Text(
+        description="License UUID:", style={"description_width": "initial"}
+    )
 
     def activate(where):
         uuid = uuid_input.value.strip()
         if where == "uuid" and len(uuid) == 0:
             return
         message.clear_output(wait=False)
         with message:
```

### Comparing `ampltools-0.5.4b1/ampltools/tests/test_install.py` & `ampltools-0.5.4b2/ampltools/tests/test_install.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.4b1/ampltools/tests/test_load.py` & `ampltools-0.5.4b2/ampltools/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.4b1/ampltools/tests/test_preload.py` & `ampltools-0.5.4b2/ampltools/tests/test_preload.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.4b1/ampltools/tests/test_run.py` & `ampltools-0.5.4b2/ampltools/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.4b1/ampltools/utils.py` & `ampltools-0.5.4b2/ampltools/utils.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.4b1/ampltools.egg-info/PKG-INFO` & `ampltools-0.5.4b2/ampltools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ampltools
-Version: 0.5.4b1
+Version: 0.5.4b2
 Summary: AMPL Python Tools
 Home-page: http://ampl.com/
 Author: Filipe Brandão
 Author-email: fdabrandao@ampl.com
 License: BSD-3
 Download-URL: https://github.com/ampl/amplpy/tree/master/ampltools
 Description:
```

### Comparing `ampltools-0.5.4b1/ampltools.egg-info/SOURCES.txt` & `ampltools-0.5.4b2/ampltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.4b1/setup.py` & `ampltools-0.5.4b2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         for (dirpath, dirnames, files) in os.walk(base_dir)
         for f in files
     ]
 
 
 setup(
     name="ampltools",
-    version="0.5.4b1",
+    version="0.5.4b2",
     description="AMPL Python Tools",
     long_description=__doc__,
     long_description_content_type="text/markdown",
     license="BSD-3",
     platforms="any",
     author="Filipe Brandão",
     author_email="fdabrandao@ampl.com",
```

