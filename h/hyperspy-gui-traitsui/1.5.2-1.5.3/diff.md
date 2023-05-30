# Comparing `tmp/hyperspy_gui_traitsui-1.5.2.tar.gz` & `tmp/hyperspy_gui_traitsui-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperspy_gui_traitsui-1.5.2.tar", last modified: Sat Jun 18 15:50:01 2022, max compression
+gzip compressed data, was "hyperspy_gui_traitsui-1.5.3.tar", last modified: Tue May 30 21:08:02 2023, max compression
```

## Comparing `hyperspy_gui_traitsui-1.5.2.tar` & `hyperspy_gui_traitsui-1.5.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 15:50:01.784113 hyperspy_gui_traitsui-1.5.2/
--rw-r--r--   0 runner    (1001) docker     (121)    35141 2022-06-18 15:49:53.000000 hyperspy_gui_traitsui-1.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-06-18 15:49:53.000000 hyperspy_gui_traitsui-1.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3372 2022-06-18 15:50:01.784113 hyperspy_gui_traitsui-1.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1534 2022-06-18 15:49:53.000000 hyperspy_gui_traitsui-1.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 15:50:01.780113 hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui/
--rw-r--r--   0 runner    (1001) docker     (121)     3176 2022-06-18 15:49:53.000000 hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6127 2022-06-18 15:49:53.000000 hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui/axes.py
--rw-r--r--   0 runner    (1001) docker     (121)      861 2022-06-18 15:49:53.000000 hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui/buttons.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-18 15:49:53.000000 hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     3417 2022-06-18 15:49:53.000000 hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui/hyperspy_extension.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1376 2022-06-18 15:49:53.000000 hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui/messages.py
--rw-r--r--   0 runner    (1001) docker     (121)     1771 2022-06-18 15:49:53.000000 hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui/microscope_parameters.py
--rw-r--r--   0 runner    (1001) docker     (121)      847 2022-06-18 15:49:53.000000 hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     1089 2022-06-18 15:49:53.000000 hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui/preferences.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2856 2022-06-18 15:49:53.000000 hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui/roi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 15:50:01.784113 hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-18 15:49:53.000000 hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1497 2022-06-18 15:49:53.000000 hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui/tests/test_axes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1248 2022-06-18 15:49:53.000000 hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (121)     1454 2022-06-18 15:49:53.000000 hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (121)     2554 2022-06-18 15:49:53.000000 hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui/tests/test_tools.py
--rwxr-xr-x   0 runner    (1001) docker     (121)       62 2022-06-18 15:49:53.000000 hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    21539 2022-06-18 15:49:53.000000 hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui/tools.py
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-06-18 15:49:53.000000 hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-06-18 15:50:01.000000 hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-18 15:50:01.784113 hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3372 2022-06-18 15:50:01.000000 hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1015 2022-06-18 15:50:01.000000 hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-18 15:50:01.000000 hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-06-18 15:50:01.000000 hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-06-18 15:50:01.000000 hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-06-18 15:50:01.000000 hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      218 2022-06-18 15:50:01.784113 hyperspy_gui_traitsui-1.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3457 2022-06-18 15:49:53.000000 hyperspy_gui_traitsui-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:08:02.720002 hyperspy_gui_traitsui-1.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-30 21:07:52.000000 hyperspy_gui_traitsui-1.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-30 21:07:52.000000 hyperspy_gui_traitsui-1.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-30 21:08:02.720002 hyperspy_gui_traitsui-1.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-30 21:07:52.000000 hyperspy_gui_traitsui-1.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:08:02.716002 hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui/
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-30 21:07:52.000000 hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-30 21:07:52.000000 hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui/axes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-30 21:07:52.000000 hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui/buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 21:07:52.000000 hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-05-30 21:07:52.000000 hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui/hyperspy_extension.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-30 21:07:52.000000 hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-30 21:07:52.000000 hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui/microscope_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-30 21:07:52.000000 hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-30 21:07:52.000000 hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui/preferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2856 2023-05-30 21:07:52.000000 hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui/roi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:08:02.720002 hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 21:07:52.000000 hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1497 2023-05-30 21:07:52.000000 hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui/tests/test_axes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-30 21:07:52.000000 hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-30 21:07:52.000000 hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-30 21:07:52.000000 hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui/tests/test_tools.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       62 2023-05-30 21:07:52.000000 hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21736 2023-05-30 21:07:52.000000 hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-30 21:07:52.000000 hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 21:08:01.000000 hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:08:02.716002 hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-30 21:08:02.000000 hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-30 21:08:02.000000 hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 21:08:02.000000 hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-30 21:08:02.000000 hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-30 21:08:02.000000 hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 21:08:02.000000 hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-30 21:08:02.720002 hyperspy_gui_traitsui-1.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-05-30 21:07:52.000000 hyperspy_gui_traitsui-1.5.3/setup.py
```

### Comparing `hyperspy_gui_traitsui-1.5.2/LICENSE` & `hyperspy_gui_traitsui-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_traitsui-1.5.2/PKG-INFO` & `hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hyperspy_gui_traitsui
-Version: 1.5.2
+Name: hyperspy-gui-traitsui
+Version: 1.5.3
 Summary: traitsui GUI elements for HyperSpy.
 Home-page: https://github.com/hyperspy/hyperspy_gui_traitsui
 Author: The HyperSpy Developers
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/hyperspy/hyperspy_gui_traitsui/issues
 Project-URL: Changelog, https://github.com/hyperspy/hyperspy_gui_traitsui/blob/main/CHANGES.md
 Project-URL: Conda-Forge, https://anaconda.org/conda-forge/hyperspy-gui-traitsui
@@ -57,14 +57,15 @@
 Keywords: hyperspy traitsui
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `hyperspy_gui_traitsui-1.5.2/README.md` & `hyperspy_gui_traitsui-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui/__init__.py` & `hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui/axes.py` & `hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui/axes.py`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui/buttons.py` & `hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui/buttons.py`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui/hyperspy_extension.yaml` & `hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui/hyperspy_extension.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         module: hyperspy_gui_traitsui.tools
         function: smooth_tv_traitsui
       hyperspy.Signal1D.smooth_butterworth:
         module: hyperspy_gui_traitsui.tools
         function: smooth_butterworth
       hyperspy.Signal1D.contrast_editor:
         module: hyperspy_gui_traitsui.tools
-        function: image_constast_editor_traitsui
+        function: image_contrast_editor_traitsui
       hyperspy.Signal1D.integrate_in_range:
         module: hyperspy_gui_traitsui.tools
         function: integrate_in_range_traitsui
       hyperspy.Signal1D.remove_background:
         module: hyperspy_gui_traitsui.tools
         function: remove_background_traitsui
       hyperspy.SimpleMessage:
```

### Comparing `hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui/messages.py` & `hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui/messages.py`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui/microscope_parameters.py` & `hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui/microscope_parameters.py`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui/model.py` & `hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui/model.py`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui/preferences.py` & `hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui/preferences.py`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui/roi.py` & `hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui/roi.py`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui/tests/test_axes.py` & `hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui/tests/test_axes.py`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui/tests/test_import.py` & `hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui/tests/test_import.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,16 @@
         else:
             # As ipywidgets is not installed it should raise an import error
             with pytest.raises(ImportError):
                 hs.preferences.gui(toolkit="traitsui")
 
 
 def test_import_version():
-    from hyperspy_gui_traitsui import __version__
+    import hyperspy_gui_traitsui
+    hyperspy_gui_traitsui.__version__
 
 
 def test_import():
     import hyperspy_gui_traitsui
     for obj_name in hyperspy_gui_traitsui.__all__:
         getattr(hyperspy_gui_traitsui, obj_name)
```

### Comparing `hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui/tests/test_model.py` & `hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui/tests/test_tools.py` & `hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui/tools.py` & `hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,17 +323,21 @@
         kind='livemodal',
         buttons=[OKButton, CancelButton],
         title='Load file')
     return obj, {"view": view}
 
 
 @add_display_arg
-def image_constast_editor_traitsui(obj, **kwargs):
-    from traitsui.qt4.extra.bounds_editor import BoundsEditor
-    
+def image_contrast_editor_traitsui(obj, **kwargs):
+    # In traitsui 8.0.0, traitsui.qt4 was changed to traitsui.qt
+    if Version(traitsui.__version__) >= Version('8.0.0'):
+        from traitsui.qt.extra.bounds_editor import BoundsEditor
+    else:
+        from traitsui.qt4.extra.bounds_editor import BoundsEditor
+
     # format has been deprecated in Release 7.3.0, replaced by format_str
     # https://github.com/enthought/traitsui/pull/1684
     # Remove and simplify when minimum traitsui version is 7.3.0
     FORMAT_STR = 'format' if Version(traitsui.__version__) < Version('7.0.0') \
         else 'format_str'
     def get_format_dict(formatting):
         return {FORMAT_STR:formatting}
@@ -411,15 +415,15 @@
             ),
         tu.Item('_'),
         handler=ImageContrastHandler,
         buttons=[OKButton,
                  HelpButton,
                  OurApplyButton,
                  OurResetButton,],
-        title='Constrast adjustment tool',
+        title='Contrast adjustment tool',
         resizable=True)
     return obj, {"view": view}
 
 
 @add_display_arg
 def integrate_in_range_traitsui(obj, **kwargs):
     view = tu.View(
```

### Comparing `hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui.egg-info/PKG-INFO` & `hyperspy_gui_traitsui-1.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hyperspy-gui-traitsui
-Version: 1.5.2
+Name: hyperspy_gui_traitsui
+Version: 1.5.3
 Summary: traitsui GUI elements for HyperSpy.
 Home-page: https://github.com/hyperspy/hyperspy_gui_traitsui
 Author: The HyperSpy Developers
 License: GPLv3
 Project-URL: Bug Tracker, https://github.com/hyperspy/hyperspy_gui_traitsui/issues
 Project-URL: Changelog, https://github.com/hyperspy/hyperspy_gui_traitsui/blob/main/CHANGES.md
 Project-URL: Conda-Forge, https://anaconda.org/conda-forge/hyperspy-gui-traitsui
@@ -57,14 +57,15 @@
 Keywords: hyperspy traitsui
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `hyperspy_gui_traitsui-1.5.2/hyperspy_gui_traitsui.egg-info/SOURCES.txt` & `hyperspy_gui_traitsui-1.5.3/hyperspy_gui_traitsui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyperspy_gui_traitsui-1.5.2/setup.py` & `hyperspy_gui_traitsui-1.5.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering",
@@ -79,15 +80,15 @@
     #   py_modules=["my_module"],
 
     # List run-time dependencies here.  These will be installed by pip when
     # your project is installed. For an analysis of "install_requires" vs pip's
     # requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
     python_requires='~=3.7',
-    install_requires=['traits>=5.0', 'hyperspy>=1.7.0', 'traitsui>=6.1'],
+    install_requires=['traits>=5.0', 'hyperspy>=1.7.0', 'traitsui>=6.1,!=8.0.0'],
     extras_require={
         'tests': ['pytest'],
         'coverage':["pytest-cov", "codecov"]},
     entry_points={'hyperspy.extensions': 'hyperspy-gui-traitsui = hyperspy_gui_traitsui'},
     package_data={  # Optional
         'hyperspy_gui_traitsui': ['hyperspy_extension.yaml'], },
         )
```

