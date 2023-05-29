# Comparing `tmp/ryvencore-0.4.0a7.tar.gz` & `tmp/ryvencore-0.4.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryvencore-0.4.0a7.tar", last modified: Wed Sep 28 11:43:00 2022, max compression
+gzip compressed data, was "ryvencore-0.4.0a9.tar", last modified: Sat Oct 22 05:09:24 2022, max compression
```

## Comparing `ryvencore-0.4.0a7.tar` & `ryvencore-0.4.0a9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 11:43:00.871626 ryvencore-0.4.0a7/
--rw-r--r--   0 runner    (1001) docker     (121)    26526 2022-09-28 11:42:46.000000 ryvencore-0.4.0a7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-09-28 11:42:46.000000 ryvencore-0.4.0a7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2827 2022-09-28 11:43:00.871626 ryvencore-0.4.0a7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2284 2022-09-28 11:42:46.000000 ryvencore-0.4.0a7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 11:43:00.867625 ryvencore-0.4.0a7/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-09-28 11:42:46.000000 ryvencore-0.4.0a7/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 11:43:00.867625 ryvencore-0.4.0a7/docs/img/
--rw-r--r--   0 runner    (1001) docker     (121)    71305 2022-09-28 11:42:46.000000 ryvencore-0.4.0a7/docs/img/logo.png
--rw-r--r--   0 runner    (1001) docker     (121)      838 2022-09-28 11:42:46.000000 ryvencore-0.4.0a7/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 11:43:00.867625 ryvencore-0.4.0a7/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 11:43:00.867625 ryvencore-0.4.0a7/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-09-28 11:42:46.000000 ryvencore-0.4.0a7/docs/source/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (121)     2461 2022-09-28 11:42:46.000000 ryvencore-0.4.0a7/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-09-28 11:42:46.000000 ryvencore-0.4.0a7/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-09-28 11:42:46.000000 ryvencore-0.4.0a7/docs/source/ryvencore.addons.default.rst
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-09-28 11:42:46.000000 ryvencore-0.4.0a7/docs/source/ryvencore.addons.rst
--rw-r--r--   0 runner    (1001) docker     (121)      923 2022-09-28 11:42:46.000000 ryvencore-0.4.0a7/docs/source/ryvencore.rst
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-09-28 11:42:46.000000 ryvencore-0.4.0a7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 11:43:00.871626 ryvencore-0.4.0a7/ryvencore/
--rw-r--r--   0 runner    (1001) docker     (121)     3052 2022-09-28 11:42:46.000000 ryvencore-0.4.0a7/ryvencore/AddOn.py
--rw-r--r--   0 runner    (1001) docker     (121)     3610 2022-09-28 11:42:46.000000 ryvencore-0.4.0a7/ryvencore/Base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3336 2022-09-28 11:42:46.000000 ryvencore-0.4.0a7/ryvencore/Data.py
--rw-r--r--   0 runner    (1001) docker     (121)    11026 2022-09-28 11:42:46.000000 ryvencore-0.4.0a7/ryvencore/Flow.py
--rw-r--r--   0 runner    (1001) docker     (121)    11022 2022-09-28 11:42:46.000000 ryvencore-0.4.0a7/ryvencore/FlowExecutor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1350 2022-09-28 11:42:46.000000 ryvencore-0.4.0a7/ryvencore/InfoMsgs.py
--rw-r--r--   0 runner    (1001) docker     (121)    12873 2022-09-28 11:42:46.000000 ryvencore-0.4.0a7/ryvencore/Node.py
--rw-r--r--   0 runner    (1001) docker     (121)     1271 2022-09-28 11:42:46.000000 ryvencore-0.4.0a7/ryvencore/NodePort.py
--rw-r--r--   0 runner    (1001) docker     (121)      768 2022-09-28 11:42:46.000000 ryvencore-0.4.0a7/ryvencore/NodePortType.py
--rw-r--r--   0 runner    (1001) docker     (121)      896 2022-09-28 11:42:46.000000 ryvencore-0.4.0a7/ryvencore/RC.py
--rw-r--r--   0 runner    (1001) docker     (121)     2408 2022-09-28 11:42:46.000000 ryvencore-0.4.0a7/ryvencore/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     5707 2022-09-28 11:42:46.000000 ryvencore-0.4.0a7/ryvencore/Session.py
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-09-28 11:42:46.000000 ryvencore-0.4.0a7/ryvencore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 11:43:00.871626 ryvencore-0.4.0a7/ryvencore/addons/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-28 11:42:46.000000 ryvencore-0.4.0a7/ryvencore/addons/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 11:43:00.871626 ryvencore-0.4.0a7/ryvencore/addons/default/
--rw-r--r--   0 runner    (1001) docker     (121)     6651 2022-09-28 11:42:46.000000 ryvencore-0.4.0a7/ryvencore/addons/default/DTypes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2881 2022-09-28 11:42:46.000000 ryvencore-0.4.0a7/ryvencore/addons/default/Logging.py
--rw-r--r--   0 runner    (1001) docker     (121)     6733 2022-09-28 11:42:46.000000 ryvencore-0.4.0a7/ryvencore/addons/default/Variables.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-28 11:42:46.000000 ryvencore-0.4.0a7/ryvencore/addons/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2230 2022-09-28 11:42:46.000000 ryvencore-0.4.0a7/ryvencore/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 11:43:00.871626 ryvencore-0.4.0a7/ryvencore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2827 2022-09-28 11:43:00.000000 ryvencore-0.4.0a7/ryvencore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      874 2022-09-28 11:43:00.000000 ryvencore-0.4.0a7/ryvencore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-28 11:43:00.000000 ryvencore-0.4.0a7/ryvencore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-09-28 11:43:00.000000 ryvencore-0.4.0a7/ryvencore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-09-28 11:43:00.871626 ryvencore-0.4.0a7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-28 11:42:46.000000 ryvencore-0.4.0a7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 05:09:24.302629 ryvencore-0.4.0a9/
+-rw-r--r--   0 runner    (1001) docker     (121)    26526 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      201 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2827 2022-10-22 05:09:24.302629 ryvencore-0.4.0a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2284 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 05:09:24.298629 ryvencore-0.4.0a9/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      638 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 05:09:24.298629 ryvencore-0.4.0a9/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (121)    71305 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/docs/img/logo.png
+-rw-r--r--   0 runner    (1001) docker     (121)      838 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 05:09:24.298629 ryvencore-0.4.0a9/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 05:09:24.298629 ryvencore-0.4.0a9/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/docs/source/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (121)     2488 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      409 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      594 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/docs/source/ryvencore.addons.default.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      255 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/docs/source/ryvencore.addons.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      923 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/docs/source/ryvencore.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       99 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 05:09:24.298629 ryvencore-0.4.0a9/ryvencore/
+-rw-r--r--   0 runner    (1001) docker     (121)     3052 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/AddOn.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3610 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/Base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3336 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/Data.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14780 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/Flow.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11022 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/FlowExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1350 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/InfoMsgs.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12873 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/Node.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1271 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/NodePort.py
+-rw-r--r--   0 runner    (1001) docker     (121)      768 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/NodePortType.py
+-rw-r--r--   0 runner    (1001) docker     (121)      896 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/RC.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2408 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     5707 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/Session.py
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 05:09:24.302629 ryvencore-0.4.0a9/ryvencore/addons/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/addons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 05:09:24.302629 ryvencore-0.4.0a9/ryvencore/addons/default/
+-rw-r--r--   0 runner    (1001) docker     (121)     6651 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/addons/default/DTypes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2881 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/addons/default/Logging.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6733 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/addons/default/Variables.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/addons/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2230 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/ryvencore/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-22 05:09:24.302629 ryvencore-0.4.0a9/ryvencore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2827 2022-10-22 05:09:24.000000 ryvencore-0.4.0a9/ryvencore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      874 2022-10-22 05:09:24.000000 ryvencore-0.4.0a9/ryvencore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-22 05:09:24.000000 ryvencore-0.4.0a9/ryvencore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       10 2022-10-22 05:09:24.000000 ryvencore-0.4.0a9/ryvencore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      661 2022-10-22 05:09:24.302629 ryvencore-0.4.0a9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-22 05:09:13.000000 ryvencore-0.4.0a9/setup.py
```

### Comparing `ryvencore-0.4.0a7/LICENSE` & `ryvencore-0.4.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `ryvencore-0.4.0a7/PKG-INFO` & `ryvencore-0.4.0a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryvencore
-Version: 0.4.0a7
+Version: 0.4.0a9
 Summary: Python backend for node editor-like graph-based processing
 Home-page: https://github.com/leon-thomm/ryvencore
 Author: Leon Thomm
 Author-email: l.thomm@mailbox.org
 Project-URL: Website, https://ryven.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
```

### Comparing `ryvencore-0.4.0a7/README.md` & `ryvencore-0.4.0a9/README.md`

 * *Files identical despite different names*

### Comparing `ryvencore-0.4.0a7/docs/Makefile` & `ryvencore-0.4.0a9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ryvencore-0.4.0a7/docs/img/logo.png` & `ryvencore-0.4.0a9/docs/img/logo.png`

 * *Files identical despite different names*

### Comparing `ryvencore-0.4.0a7/docs/make.bat` & `ryvencore-0.4.0a9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ryvencore-0.4.0a7/docs/source/conf.py` & `ryvencore-0.4.0a9/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     'sphinx.ext.autodoc',
     'sphinx.ext.napoleon',
+    'sphinx.ext.viewcode',
 ]
 
 add_module_names = False
 
 # autodoc options
 autodoc_member_order = 'bysource'
```

### Comparing `ryvencore-0.4.0a7/docs/source/ryvencore.addons.default.rst` & `ryvencore-0.4.0a9/docs/source/ryvencore.addons.default.rst`

 * *Files identical despite different names*

### Comparing `ryvencore-0.4.0a7/docs/source/ryvencore.rst` & `ryvencore-0.4.0a9/docs/source/ryvencore.rst`

 * *Files identical despite different names*

### Comparing `ryvencore-0.4.0a7/ryvencore/AddOn.py` & `ryvencore-0.4.0a9/ryvencore/AddOn.py`

 * *Files identical despite different names*

### Comparing `ryvencore-0.4.0a7/ryvencore/Base.py` & `ryvencore-0.4.0a9/ryvencore/Base.py`

 * *Files identical despite different names*

### Comparing `ryvencore-0.4.0a7/ryvencore/Data.py` & `ryvencore-0.4.0a9/ryvencore/Data.py`

 * *Files identical despite different names*

### Comparing `ryvencore-0.4.0a7/ryvencore/FlowExecutor.py` & `ryvencore-0.4.0a9/ryvencore/FlowExecutor.py`

 * *Files identical despite different names*

### Comparing `ryvencore-0.4.0a7/ryvencore/InfoMsgs.py` & `ryvencore-0.4.0a9/ryvencore/InfoMsgs.py`

 * *Files identical despite different names*

### Comparing `ryvencore-0.4.0a7/ryvencore/Node.py` & `ryvencore-0.4.0a9/ryvencore/Node.py`

 * *Files identical despite different names*

### Comparing `ryvencore-0.4.0a7/ryvencore/NodePort.py` & `ryvencore-0.4.0a9/ryvencore/NodePort.py`

 * *Files identical despite different names*

### Comparing `ryvencore-0.4.0a7/ryvencore/NodePortType.py` & `ryvencore-0.4.0a9/ryvencore/NodePortType.py`

 * *Files identical despite different names*

### Comparing `ryvencore-0.4.0a7/ryvencore/RC.py` & `ryvencore-0.4.0a9/ryvencore/RC.py`

 * *Files identical despite different names*

### Comparing `ryvencore-0.4.0a7/ryvencore/README.md` & `ryvencore-0.4.0a9/ryvencore/README.md`

 * *Files identical despite different names*

### Comparing `ryvencore-0.4.0a7/ryvencore/Session.py` & `ryvencore-0.4.0a9/ryvencore/Session.py`

 * *Files identical despite different names*

### Comparing `ryvencore-0.4.0a7/ryvencore/addons/default/DTypes.py` & `ryvencore-0.4.0a9/ryvencore/addons/default/DTypes.py`

 * *Files identical despite different names*

### Comparing `ryvencore-0.4.0a7/ryvencore/addons/default/Logging.py` & `ryvencore-0.4.0a9/ryvencore/addons/default/Logging.py`

 * *Files identical despite different names*

### Comparing `ryvencore-0.4.0a7/ryvencore/addons/default/Variables.py` & `ryvencore-0.4.0a9/ryvencore/addons/default/Variables.py`

 * *Files identical despite different names*

### Comparing `ryvencore-0.4.0a7/ryvencore/utils.py` & `ryvencore-0.4.0a9/ryvencore/utils.py`

 * *Files identical despite different names*

### Comparing `ryvencore-0.4.0a7/ryvencore.egg-info/PKG-INFO` & `ryvencore-0.4.0a9/ryvencore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryvencore
-Version: 0.4.0a7
+Version: 0.4.0a9
 Summary: Python backend for node editor-like graph-based processing
 Home-page: https://github.com/leon-thomm/ryvencore
 Author: Leon Thomm
 Author-email: l.thomm@mailbox.org
 Project-URL: Website, https://ryven.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
```

### Comparing `ryvencore-0.4.0a7/ryvencore.egg-info/SOURCES.txt` & `ryvencore-0.4.0a9/ryvencore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ryvencore-0.4.0a7/setup.cfg` & `ryvencore-0.4.0a9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ryvencore
-version = v0.4.0a7
+version = v0.4.0a9
 author = Leon Thomm
 author_email = l.thomm@mailbox.org
 description = Python backend for node editor-like graph-based processing
 long_description = file: README.md
 long_description_content_type = text/markdown
 license_file = LICENSE
 url = https://github.com/leon-thomm/ryvencore
```

