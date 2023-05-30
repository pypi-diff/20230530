# Comparing `tmp/ampltools-0.5.4b2.tar.gz` & `tmp/ampltools-0.5.4b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ampltools-0.5.4b2.tar", last modified: Tue May 30 11:29:03 2023, max compression
+gzip compressed data, was "ampltools-0.5.4b3.tar", last modified: Tue May 30 13:33:44 2023, max compression
```

## Comparing `ampltools-0.5.4b2.tar` & `ampltools-0.5.4b3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-05-30 11:29:03.900523 ampltools-0.5.4b2/
--rw-r--r--   0 fdabrandao   (501) staff       (20)     2822 2023-05-03 11:08:48.000000 ampltools-0.5.4b2/CHANGELOG.md
--rw-r--r--   0 fdabrandao   (501) staff       (20)     1522 2023-03-08 15:44:27.000000 ampltools-0.5.4b2/LICENSE
--rw-r--r--   0 fdabrandao   (501) staff       (20)       57 2023-03-08 15:44:27.000000 ampltools-0.5.4b2/MANIFEST.in
--rw-r--r--   0 fdabrandao   (501) staff       (20)     1282 2023-05-30 11:29:03.900143 ampltools-0.5.4b2/PKG-INFO
--rw-r--r--   0 fdabrandao   (501) staff       (20)      446 2023-03-08 15:44:27.000000 ampltools-0.5.4b2/README.md
-drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-05-30 11:29:03.889929 ampltools-0.5.4b2/ampltools/
--rw-r--r--   0 fdabrandao   (501) staff       (20)      409 2023-05-30 11:29:00.000000 ampltools-0.5.4b2/ampltools/__init__.py
-drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-05-30 11:29:03.895957 ampltools-0.5.4b2/ampltools/modules/
--rw-r--r--   0 fdabrandao   (501) staff       (20)      443 2023-05-30 11:29:00.000000 ampltools-0.5.4b2/ampltools/modules/__init__.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)       93 2023-03-08 15:44:27.000000 ampltools-0.5.4b2/ampltools/modules/__main__.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)    12683 2023-05-03 11:08:48.000000 ampltools-0.5.4b2/ampltools/modules/amplpypi.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     3723 2023-03-09 15:01:44.000000 ampltools-0.5.4b2/ampltools/modules/commands.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     5737 2023-05-30 11:28:23.000000 ampltools-0.5.4b2/ampltools/notebooks.py
-drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-05-30 11:29:03.899383 ampltools-0.5.4b2/ampltools/tests/
--rw-r--r--   0 fdabrandao   (501) staff       (20)      433 2023-03-08 15:44:27.000000 ampltools-0.5.4b2/ampltools/tests/TestBase.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)       24 2023-03-08 15:44:27.000000 ampltools-0.5.4b2/ampltools/tests/__init__.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)      286 2023-03-08 15:44:27.000000 ampltools-0.5.4b2/ampltools/tests/__main__.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     3566 2023-03-08 15:44:27.000000 ampltools-0.5.4b2/ampltools/tests/test_install.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     1951 2023-03-08 15:44:27.000000 ampltools-0.5.4b2/ampltools/tests/test_load.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     2411 2023-03-13 18:25:11.000000 ampltools-0.5.4b2/ampltools/tests/test_preload.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     1751 2023-03-08 15:44:27.000000 ampltools-0.5.4b2/ampltools/tests/test_run.py
--rw-r--r--   0 fdabrandao   (501) staff       (20)     3228 2023-03-09 15:37:57.000000 ampltools-0.5.4b2/ampltools/utils.py
-drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-05-30 11:29:03.892600 ampltools-0.5.4b2/ampltools.egg-info/
--rw-r--r--   0 fdabrandao   (501) staff       (20)     1282 2023-05-30 11:29:03.000000 ampltools-0.5.4b2/ampltools.egg-info/PKG-INFO
--rw-r--r--   0 fdabrandao   (501) staff       (20)      621 2023-05-30 11:29:03.000000 ampltools-0.5.4b2/ampltools.egg-info/SOURCES.txt
--rw-r--r--   0 fdabrandao   (501) staff       (20)        1 2023-05-30 11:29:03.000000 ampltools-0.5.4b2/ampltools.egg-info/dependency_links.txt
--rw-r--r--   0 fdabrandao   (501) staff       (20)        9 2023-05-30 11:29:03.000000 ampltools-0.5.4b2/ampltools.egg-info/requires.txt
--rw-r--r--   0 fdabrandao   (501) staff       (20)       10 2023-05-30 11:29:03.000000 ampltools-0.5.4b2/ampltools.egg-info/top_level.txt
--rw-r--r--   0 fdabrandao   (501) staff       (20)        8 2023-03-08 15:44:27.000000 ampltools-0.5.4b2/requirements.txt
--rw-r--r--   0 fdabrandao   (501) staff       (20)       38 2023-05-30 11:29:03.900607 ampltools-0.5.4b2/setup.cfg
--rw-r--r--   0 fdabrandao   (501) staff       (20)     1717 2023-05-30 11:29:00.000000 ampltools-0.5.4b2/setup.py
+drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-05-30 13:33:44.477687 ampltools-0.5.4b3/
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     2822 2023-05-03 11:08:48.000000 ampltools-0.5.4b3/CHANGELOG.md
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     1522 2023-03-08 15:44:27.000000 ampltools-0.5.4b3/LICENSE
+-rw-r--r--   0 fdabrandao   (501) staff       (20)       57 2023-03-08 15:44:27.000000 ampltools-0.5.4b3/MANIFEST.in
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     1219 2023-05-30 13:33:44.477383 ampltools-0.5.4b3/PKG-INFO
+-rw-r--r--   0 fdabrandao   (501) staff       (20)      446 2023-03-08 15:44:27.000000 ampltools-0.5.4b3/README.md
+drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-05-30 13:33:44.472104 ampltools-0.5.4b3/ampltools/
+-rw-r--r--   0 fdabrandao   (501) staff       (20)      409 2023-05-30 13:33:41.000000 ampltools-0.5.4b3/ampltools/__init__.py
+drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-05-30 13:33:44.474796 ampltools-0.5.4b3/ampltools/modules/
+-rw-r--r--   0 fdabrandao   (501) staff       (20)      443 2023-05-30 13:33:41.000000 ampltools-0.5.4b3/ampltools/modules/__init__.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)       93 2023-03-08 15:44:27.000000 ampltools-0.5.4b3/ampltools/modules/__main__.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)    12683 2023-05-03 11:08:48.000000 ampltools-0.5.4b3/ampltools/modules/amplpypi.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     3723 2023-03-09 15:01:44.000000 ampltools-0.5.4b3/ampltools/modules/commands.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     5838 2023-05-30 13:33:35.000000 ampltools-0.5.4b3/ampltools/notebooks.py
+drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-05-30 13:33:44.476912 ampltools-0.5.4b3/ampltools/tests/
+-rw-r--r--   0 fdabrandao   (501) staff       (20)      433 2023-03-08 15:44:27.000000 ampltools-0.5.4b3/ampltools/tests/TestBase.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)       24 2023-03-08 15:44:27.000000 ampltools-0.5.4b3/ampltools/tests/__init__.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)      286 2023-03-08 15:44:27.000000 ampltools-0.5.4b3/ampltools/tests/__main__.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     3566 2023-03-08 15:44:27.000000 ampltools-0.5.4b3/ampltools/tests/test_install.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     1951 2023-03-08 15:44:27.000000 ampltools-0.5.4b3/ampltools/tests/test_load.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     2411 2023-03-13 18:25:11.000000 ampltools-0.5.4b3/ampltools/tests/test_preload.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     1751 2023-03-08 15:44:27.000000 ampltools-0.5.4b3/ampltools/tests/test_run.py
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     3228 2023-03-09 15:37:57.000000 ampltools-0.5.4b3/ampltools/utils.py
+drwxr-xr-x   0 fdabrandao   (501) staff       (20)        0 2023-05-30 13:33:44.473664 ampltools-0.5.4b3/ampltools.egg-info/
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     1219 2023-05-30 13:33:44.000000 ampltools-0.5.4b3/ampltools.egg-info/PKG-INFO
+-rw-r--r--   0 fdabrandao   (501) staff       (20)      621 2023-05-30 13:33:44.000000 ampltools-0.5.4b3/ampltools.egg-info/SOURCES.txt
+-rw-r--r--   0 fdabrandao   (501) staff       (20)        1 2023-05-30 13:33:44.000000 ampltools-0.5.4b3/ampltools.egg-info/dependency_links.txt
+-rw-r--r--   0 fdabrandao   (501) staff       (20)        9 2023-05-30 13:33:44.000000 ampltools-0.5.4b3/ampltools.egg-info/requires.txt
+-rw-r--r--   0 fdabrandao   (501) staff       (20)       10 2023-05-30 13:33:44.000000 ampltools-0.5.4b3/ampltools.egg-info/top_level.txt
+-rw-r--r--   0 fdabrandao   (501) staff       (20)        8 2023-03-08 15:44:27.000000 ampltools-0.5.4b3/requirements.txt
+-rw-r--r--   0 fdabrandao   (501) staff       (20)       38 2023-05-30 13:33:44.477766 ampltools-0.5.4b3/setup.cfg
+-rw-r--r--   0 fdabrandao   (501) staff       (20)     1717 2023-05-30 13:33:41.000000 ampltools-0.5.4b3/setup.py
```

### Comparing `ampltools-0.5.4b2/CHANGELOG.md` & `ampltools-0.5.4b3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.4b2/LICENSE` & `ampltools-0.5.4b3/LICENSE`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.4b2/PKG-INFO` & `ampltools-0.5.4b3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,16 @@
 Metadata-Version: 2.1
 Name: ampltools
-Version: 0.5.4b2
+Version: 0.5.4b3
 Summary: AMPL Python Tools
 Home-page: http://ampl.com/
+Download-URL: https://github.com/ampl/amplpy/tree/master/ampltools
 Author: Filipe Brandão
 Author-email: fdabrandao@ampl.com
 License: BSD-3
-Download-URL: https://github.com/ampl/amplpy/tree/master/ampltools
-Description: 
-        # AMPL Python Tools
-        
-        This package includes tools to use with [AMPL](https://ampl.com) and [amplpy](https://amplpy.readthedocs.io).
-        
-        ## Links
-        
-        * GitHub Repository: https://github.com/ampl/amplpy/
-        * PyPI Repository: https://pypi.python.org/pypi/ampltools
-        
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -29,7 +19,18 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# AMPL Python Tools
+
+This package includes tools to use with [AMPL](https://ampl.com) and [amplpy](https://amplpy.readthedocs.io).
+
+## Links
+
+* GitHub Repository: https://github.com/ampl/amplpy/
+* PyPI Repository: https://pypi.python.org/pypi/ampltools
```

### Comparing `ampltools-0.5.4b2/ampltools/modules/amplpypi.py` & `ampltools-0.5.4b3/ampltools/modules/amplpypi.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.4b2/ampltools/modules/commands.py` & `ampltools-0.5.4b3/ampltools/modules/commands.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.4b2/ampltools/notebooks.py` & `ampltools-0.5.4b3/ampltools/notebooks.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,23 +86,21 @@
         return False
 
 
 def ampl_notebook(
     modules=[],
     license_uuid=None,
     reinstall=False,
-    g=None,
     verbose=False,
     show_license=None,
-    globals_=None,
+    **kwargs
 ):
     from IPython import get_ipython
 
-    if globals_ is None:
-        globals_ = g
+    globals_ = kwargs.get("globals_", kwargs.get("g", None))
     if globals_ is None:
         globals_ = get_ipython().user_global_ns
     show_prompt = globals_ is not None
     if show_license is None:
         show_license = True
 
     def instantiate_ampl(print_license=True):
@@ -130,15 +128,25 @@
     if modules not in (None, []):
         install_modules(modules, reinstall=reinstall, verbose=verbose)
         load_modules(modules, verbose=verbose)
     else:
         modules = []
 
     using_default_license = license_uuid in (None, "", "default", "your-license-uuid")
-    open_modules = ["highs", "cbc", "coin", "open", "plugins", "ampl"]
+    open_modules = [
+        "highs",
+        "cbc",
+        "coin",
+        "gecode",
+        "scip",
+        "gcg",
+        "open",
+        "plugins",
+        "ampl",
+    ]
     open_source_only = len(set(modules) - set(open_modules)) == 0
 
     if using_default_license:
         using_default_license = _handle_default_uuid()
     if using_default_license:
         if show_prompt and open_source_only:
             show_prompt = False
```

### Comparing `ampltools-0.5.4b2/ampltools/tests/test_install.py` & `ampltools-0.5.4b3/ampltools/tests/test_install.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.4b2/ampltools/tests/test_load.py` & `ampltools-0.5.4b3/ampltools/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.4b2/ampltools/tests/test_preload.py` & `ampltools-0.5.4b3/ampltools/tests/test_preload.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.4b2/ampltools/tests/test_run.py` & `ampltools-0.5.4b3/ampltools/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.4b2/ampltools/utils.py` & `ampltools-0.5.4b3/ampltools/utils.py`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.4b2/ampltools.egg-info/PKG-INFO` & `ampltools-0.5.4b3/ampltools.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,16 @@
 Metadata-Version: 2.1
 Name: ampltools
-Version: 0.5.4b2
+Version: 0.5.4b3
 Summary: AMPL Python Tools
 Home-page: http://ampl.com/
+Download-URL: https://github.com/ampl/amplpy/tree/master/ampltools
 Author: Filipe Brandão
 Author-email: fdabrandao@ampl.com
 License: BSD-3
-Download-URL: https://github.com/ampl/amplpy/tree/master/ampltools
-Description: 
-        # AMPL Python Tools
-        
-        This package includes tools to use with [AMPL](https://ampl.com) and [amplpy](https://amplpy.readthedocs.io).
-        
-        ## Links
-        
-        * GitHub Repository: https://github.com/ampl/amplpy/
-        * PyPI Repository: https://pypi.python.org/pypi/ampltools
-        
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -29,7 +19,18 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# AMPL Python Tools
+
+This package includes tools to use with [AMPL](https://ampl.com) and [amplpy](https://amplpy.readthedocs.io).
+
+## Links
+
+* GitHub Repository: https://github.com/ampl/amplpy/
+* PyPI Repository: https://pypi.python.org/pypi/ampltools
```

### Comparing `ampltools-0.5.4b2/ampltools.egg-info/SOURCES.txt` & `ampltools-0.5.4b3/ampltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ampltools-0.5.4b2/setup.py` & `ampltools-0.5.4b3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         for (dirpath, dirnames, files) in os.walk(base_dir)
         for f in files
     ]
 
 
 setup(
     name="ampltools",
-    version="0.5.4b2",
+    version="0.5.4b3",
     description="AMPL Python Tools",
     long_description=__doc__,
     long_description_content_type="text/markdown",
     license="BSD-3",
     platforms="any",
     author="Filipe Brandão",
     author_email="fdabrandao@ampl.com",
```

