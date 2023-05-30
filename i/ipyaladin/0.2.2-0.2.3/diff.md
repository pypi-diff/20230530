# Comparing `tmp/ipyaladin-0.2.2.tar.gz` & `tmp/ipyaladin-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyaladin-0.2.2.tar", last modified: Fri May 26 13:45:09 2023, max compression
+gzip compressed data, was "ipyaladin-0.2.3.tar", last modified: Tue May 30 12:09:04 2023, max compression
```

## Comparing `ipyaladin-0.2.2.tar` & `ipyaladin-0.2.3.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:45:09.931827 ipyaladin-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-26 13:45:09.931827 ipyaladin-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/install.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:45:09.927827 ipyaladin-0.2.2/ipyaladin/
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/ipyaladin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/ipyaladin/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    14228 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/ipyaladin/aladin_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:45:09.927827 ipyaladin-0.2.2/ipyaladin/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-26 13:45:09.000000 ipyaladin-0.2.2/ipyaladin/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:45:09.927827 ipyaladin-0.2.2/ipyaladin/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-26 13:45:09.000000 ipyaladin-0.2.2/ipyaladin/labextension/static/563.b311860ae40bdaae42cf.js
--rw-r--r--   0 runner    (1001) docker     (123)    27540 2023-05-26 13:45:09.000000 ipyaladin-0.2.2/ipyaladin/labextension/static/590.9292295778c3653a0b31.js
--rw-r--r--   0 runner    (1001) docker     (123)    22071 2023-05-26 13:45:09.000000 ipyaladin-0.2.2/ipyaladin/labextension/static/794.644314dbf6493c3f7619.js
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-05-26 13:45:09.000000 ipyaladin-0.2.2/ipyaladin/labextension/static/remoteEntry.c35d9bcfb9f9c1b91ff1.js
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-26 13:45:06.000000 ipyaladin-0.2.2/ipyaladin/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-26 13:45:09.000000 ipyaladin-0.2.2/ipyaladin/labextension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:45:09.927827 ipyaladin-0.2.2/ipyaladin/nbextension/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-26 13:44:51.000000 ipyaladin-0.2.2/ipyaladin/nbextension/extension.js
--rw-r--r--   0 runner    (1001) docker     (123)    27432 2023-05-26 13:44:54.000000 ipyaladin-0.2.2/ipyaladin/nbextension/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:45:09.927827 ipyaladin-0.2.2/ipyaladin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-26 13:45:09.000000 ipyaladin-0.2.2/ipyaladin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-26 13:45:09.000000 ipyaladin-0.2.2/ipyaladin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:45:09.000000 ipyaladin-0.2.2/ipyaladin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:44:38.000000 ipyaladin-0.2.2/ipyaladin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-26 13:45:09.000000 ipyaladin-0.2.2/ipyaladin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 13:45:09.000000 ipyaladin-0.2.2/ipyaladin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/ipyaladin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:45:09.931827 ipyaladin-0.2.2/js/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/js/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/js/amd-public-path.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:45:09.931827 ipyaladin-0.2.2/js/dist/
--rw-r--r--   0 runner    (1001) docker     (123)    27432 2023-05-26 13:44:53.000000 ipyaladin-0.2.2/js/dist/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:45:09.931827 ipyaladin-0.2.2/js/lib/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/js/lib/extension.js
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/js/lib/index.js
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/js/lib/jupyter-aladin.js
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/js/lib/labplugin.js
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/js/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/js/webpack.config.js
--rw-r--r--   0 runner    (1001) docker     (123)    82531 2023-05-26 13:44:49.000000 ipyaladin-0.2.2/js/yarn.lock
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-26 13:45:09.931827 ipyaladin-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-26 13:44:06.000000 ipyaladin-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:09:04.559184 ipyaladin-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-05-30 12:09:04.559184 ipyaladin-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/install.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:09:04.555184 ipyaladin-0.2.3/ipyaladin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/ipyaladin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/ipyaladin/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14228 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/ipyaladin/aladin_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:09:04.555184 ipyaladin-0.2.3/ipyaladin/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-30 12:09:04.000000 ipyaladin-0.2.3/ipyaladin/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:09:04.555184 ipyaladin-0.2.3/ipyaladin/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-30 12:09:04.000000 ipyaladin-0.2.3/ipyaladin/labextension/static/563.9c25681782097966161a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27540 2023-05-30 12:09:04.000000 ipyaladin-0.2.3/ipyaladin/labextension/static/590.b90399830948d2f839e2.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22071 2023-05-30 12:09:04.000000 ipyaladin-0.2.3/ipyaladin/labextension/static/794.644314dbf6493c3f7619.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-05-30 12:09:04.000000 ipyaladin-0.2.3/ipyaladin/labextension/static/remoteEntry.baf7991223a7feb4e9c0.js
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-30 12:09:01.000000 ipyaladin-0.2.3/ipyaladin/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-30 12:09:04.000000 ipyaladin-0.2.3/ipyaladin/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:09:04.555184 ipyaladin-0.2.3/ipyaladin/nbextension/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-30 12:08:50.000000 ipyaladin-0.2.3/ipyaladin/nbextension/extension.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27432 2023-05-30 12:08:51.000000 ipyaladin-0.2.3/ipyaladin/nbextension/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:09:04.555184 ipyaladin-0.2.3/ipyaladin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-05-30 12:09:04.000000 ipyaladin-0.2.3/ipyaladin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-30 12:09:04.000000 ipyaladin-0.2.3/ipyaladin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:09:04.000000 ipyaladin-0.2.3/ipyaladin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:08:38.000000 ipyaladin-0.2.3/ipyaladin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-30 12:09:04.000000 ipyaladin-0.2.3/ipyaladin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-30 12:09:04.000000 ipyaladin-0.2.3/ipyaladin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/ipyaladin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:09:04.555184 ipyaladin-0.2.3/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/js/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/js/amd-public-path.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:09:04.555184 ipyaladin-0.2.3/js/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)    27432 2023-05-30 12:08:52.000000 ipyaladin-0.2.3/js/dist/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:09:04.555184 ipyaladin-0.2.3/js/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/js/lib/extension.js
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/js/lib/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/js/lib/jupyter-aladin.js
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/js/lib/labplugin.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/js/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/js/webpack.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)    82533 2023-05-30 12:08:48.000000 ipyaladin-0.2.3/js/yarn.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-30 12:09:04.559184 ipyaladin-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-30 12:08:11.000000 ipyaladin-0.2.3/setup.py
```

### Comparing `ipyaladin-0.2.2/LICENSE.md` & `ipyaladin-0.2.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ipyaladin-0.2.2/PKG-INFO` & `ipyaladin-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyaladin
-Version: 0.2.2
+Version: 0.2.3
 Summary: ipyaladin
 Home-page: https://github.com/cds-astro/ipyaladin
 Author: Jerome Desroziers, Thomas Boch & Matthieu Baumann
 Author-email: matthieu.baumann@astro.unistra.fr
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/cds-astro/ipyaladin/issues
 Project-URL: Live Testing, https://mybinder.org/v2/gh/cds-astro/ipyaladin/master
@@ -19,17 +19,19 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Jupyter
 Classifier: Framework :: Jupyter :: JupyterLab
 Classifier: Framework :: Jupyter :: JupyterLab :: 3
+Classifier: Framework :: Jupyter :: JupyterLab :: 4
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # ipyaladin
@@ -68,15 +70,15 @@
 And you are ready to use ipyaladin inside your notebooks!
 Additionny, for a jupyterlab usage you will need to:
 
     jupyter labextension develop ipyaladin --overwrite
 
 There is also a conda package that can be installed with:
 
-    conda install -c bmatthieu3 ipyaladin==0.2.2
+    conda install -c bmatthieu3 ipyaladin==0.2.3
 
 ## New features corner
 
 ![new_features](assets/new_features.gif)
 
 ## Development installation
```

### Comparing `ipyaladin-0.2.2/README.md` & `ipyaladin-0.2.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 And you are ready to use ipyaladin inside your notebooks!
 Additionny, for a jupyterlab usage you will need to:
 
     jupyter labextension develop ipyaladin --overwrite
 
 There is also a conda package that can be installed with:
 
-    conda install -c bmatthieu3 ipyaladin==0.2.2
+    conda install -c bmatthieu3 ipyaladin==0.2.3
 
 ## New features corner
 
 ![new_features](assets/new_features.gif)
 
 ## Development installation
```

### Comparing `ipyaladin-0.2.2/ipyaladin/__init__.py` & `ipyaladin-0.2.3/ipyaladin/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyaladin-0.2.2/ipyaladin/aladin_widget.py` & `ipyaladin-0.2.3/ipyaladin/aladin_widget.py`

 * *Files identical despite different names*

### Comparing `ipyaladin-0.2.2/ipyaladin/labextension/package.json` & `ipyaladin-0.2.3/ipyaladin/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9631696428571429%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.baf7991223a7feb4e9c0.js'}}",*

 * * "'version'": "'0.2.3'"}*

```diff
@@ -12,15 +12,15 @@
     },
     "files": [
         "dist/*.js"
     ],
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.c35d9bcfb9f9c1b91ff1.js"
+            "load": "static/remoteEntry.baf7991223a7feb4e9c0.js"
         },
         "extension": "lib/labplugin",
         "outputDir": "../ipyaladin/labextension",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -48,9 +48,9 @@
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:prod": "webpack --mode=production && yarn run build:labextension",
         "clean": "rimraf dist/ && rimraf ../ipyaladin/labextension/ && rimraf ../ipyaladin/nbextension",
         "prepublish": "yarn run clean && yarn run build:prod",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch --mode=development"
     },
-    "version": "0.2.2"
+    "version": "0.2.3"
 }
```

### Comparing `ipyaladin-0.2.2/ipyaladin/labextension/static/563.b311860ae40bdaae42cf.js` & `ipyaladin-0.2.3/ipyaladin/labextension/static/563.9c25681782097966161a.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -32,16 +32,16 @@
                 defaults() {
                     return {
                         ...super.defaults(),
                         _model_name: "AladinModel",
                         _view_name: "AladinView",
                         _model_module: "ipyaladin",
                         _view_module: "ipyaladin",
-                        _model_module_version: "0.2.2",
-                        _view_module_version: "0.2.2"
+                        _model_module_version: "0.2.3",
+                        _view_module_version: "0.2.3"
                     }
                 }
             }
             let h = 0;
             class d extends i.DOMWidgetView {
                 render() {
                     l.then((() => {
@@ -151,15 +151,15 @@
             }
             const n = {
                     id: "ipyaladin:plugin",
                     requires: [i.IJupyterWidgetRegistry],
                     activate: function(t, e) {
                         e.registerWidget({
                             name: "ipyaladin",
-                            version: "0.2.2",
+                            version: "0.2.3",
                             exports: {
                                 AladinModel: o,
                                 AladinView: d
                             }
                         })
                     },
                     autoStart: !0
```

### Comparing `ipyaladin-0.2.2/ipyaladin/labextension/static/590.9292295778c3653a0b31.js` & `ipyaladin-0.2.3/ipyaladin/labextension/static/590.b90399830948d2f839e2.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1410,16 +1410,16 @@
                         defaults() {
                             return {
                                 ...super.defaults(),
                                 _model_name: "AladinModel",
                                 _view_name: "AladinView",
                                 _model_module: "ipyaladin",
                                 _view_module: "ipyaladin",
-                                _model_module_version: "0.2.2",
-                                _view_module_version: "0.2.2"
+                                _model_module_version: "0.2.3",
+                                _view_module_version: "0.2.3"
                             }
                         }
                     }
                     let i = 0;
                     class u extends t.DOMWidgetView {
                         render() {
                             n.then((() => {
@@ -1524,14 +1524,14 @@
                             })), this.listenTo(this.model, "change:color_map_flag", (() => {
                                 const t = this.model.get("color_map_name");
                                 this.al.getBaseImageLayer().setColormap(t)
                             }))
                         }
                     }
                     const l = {
-                        i8: "0.2.2"
+                        i8: "0.2.3"
                     }
                 })(), a
             })()).apply(e, r)) || (t.exports = i)
         }
     }
 ]);
```

### Comparing `ipyaladin-0.2.2/ipyaladin/labextension/static/794.644314dbf6493c3f7619.js` & `ipyaladin-0.2.3/ipyaladin/labextension/static/794.644314dbf6493c3f7619.js`

 * *Files identical despite different names*

### Comparing `ipyaladin-0.2.2/ipyaladin/labextension/static/remoteEntry.c35d9bcfb9f9c1b91ff1.js` & `ipyaladin-0.2.3/ipyaladin/labextension/static/remoteEntry.baf7991223a7feb4e9c0.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,30 +1,30 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, l, d, u, s, f, c, p, h, v, g, b, m, y = {
+    var e, r, t, n, a, o, i, l, u, d, s, f, c, p, h, v, b, g, m, y = {
             460: (e, r, t) => {
                 var n = {
                         "./index": () => Promise.all([t.e(672), t.e(590)]).then((() => () => t(590))),
                         "./extension": () => Promise.all([t.e(672), t.e(563)]).then((() => () => t(563)))
                     },
-                    o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
+                    a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
-                    a = (e, r) => {
+                    o = (e, r) => {
                         if (t.S) {
                             var n = "default",
-                                o = t.S[n];
-                            if (o && o !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                                a = t.S[n];
+                            if (a && a !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
                             return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
-                    get: () => o,
-                    init: () => a
+                    get: () => a,
+                    init: () => o
                 })
             }
         },
         w = {};
 
     function S(e) {
         var r = w[e];
@@ -38,47 +38,47 @@
     }
     S.m = y, S.c = w, S.d = (e, r) => {
         for (var t in r) S.o(r, t) && !S.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, S.f = {}, S.e = e => Promise.all(Object.keys(S.f).reduce(((r, t) => (S.f[t](e, r), r)), [])), S.u = e => e + "." + {
-        563: "b311860ae40bdaae42cf",
-        590: "9292295778c3653a0b31",
+        563: "9c25681782097966161a",
+        590: "b90399830948d2f839e2",
         672: "d1c8706d8114ce8e432a",
         794: "644314dbf6493c3f7619"
     } [e] + ".js?v=" + {
-        563: "b311860ae40bdaae42cf",
-        590: "9292295778c3653a0b31",
+        563: "9c25681782097966161a",
+        590: "b90399830948d2f839e2",
         672: "d1c8706d8114ce8e432a",
         794: "644314dbf6493c3f7619"
     } [e], S.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), S.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "ipyaladin:", S.l = (t, n, o, a) => {
+    }(), S.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "ipyaladin:", S.l = (t, n, a, o) => {
         if (e[t]) e[t].push(n);
         else {
             var i, l;
-            if (void 0 !== o)
-                for (var d = document.getElementsByTagName("script"), u = 0; u < d.length; u++) {
-                    var s = d[u];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
+            if (void 0 !== a)
+                for (var u = document.getElementsByTagName("script"), d = 0; d < u.length; d++) {
+                    var s = u[d];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + a) {
                         i = s;
                         break
                     }
                 }
-            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, S.nc && i.setAttribute("nonce", S.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
+            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, S.nc && i.setAttribute("nonce", S.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
             var f = (r, n) => {
                     i.onerror = i.onload = null, clearTimeout(c);
-                    var o = e[t];
-                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
+                    var a = e[t];
+                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
                 },
                 c = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
             i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), l && document.head.appendChild(i)
         }
@@ -90,31 +90,31 @@
         })
     }, S.nmd = e => (e.paths = [], e.children || (e.children = []), e), (() => {
         S.S = {};
         var e = {},
             r = {};
         S.I = (t, n) => {
             n || (n = []);
-            var o = r[t];
-            if (o || (o = r[t] = {}), !(n.indexOf(o) >= 0)) {
-                if (n.push(o), e[t]) return e[t];
+            var a = r[t];
+            if (a || (a = r[t] = {}), !(n.indexOf(a) >= 0)) {
+                if (n.push(a), e[t]) return e[t];
                 S.o(S.S, t) || (S.S[t] = {});
-                var a = S.S[t],
+                var o = S.S[t],
                     i = "ipyaladin",
                     l = (e, r, t, n) => {
-                        var o = a[e] = a[e] || {},
-                            l = o[r];
-                        (!l || !l.loaded && (!n != !l.eager ? n : i > l.from)) && (o[r] = {
+                        var a = o[e] = o[e] || {},
+                            l = a[r];
+                        (!l || !l.loaded && (!n != !l.eager ? n : i > l.from)) && (a[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
-                    d = [];
-                return "default" === t && (l("ipyaladin", "0.2.2", (() => Promise.all([S.e(672), S.e(590)]).then((() => () => S(590))))), l("underscore", "1.13.6", (() => S.e(794).then((() => () => S(794)))))), e[t] = d.length ? Promise.all(d).then((() => e[t] = 1)) : 1
+                    u = [];
+                return "default" === t && (l("ipyaladin", "0.2.3", (() => Promise.all([S.e(672), S.e(590)]).then((() => () => S(590))))), l("underscore", "1.13.6", (() => S.e(794).then((() => () => S(794)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -129,159 +129,159 @@
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
         for (var n = 0;;) {
             if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
-            var o = e[n],
-                a = (typeof o)[0];
-            if (n >= r.length) return "u" == a;
+            var a = e[n],
+                o = (typeof a)[0];
+            if (n >= r.length) return "u" == o;
             var i = r[n],
                 l = (typeof i)[0];
-            if (a != l) return "o" == a && "n" == l || "s" == l || "u" == a;
-            if ("o" != a && "u" != a && o != i) return o < i;
+            if (o != l) return "o" == o && "n" == l || "s" == l || "u" == o;
+            if ("o" != o && "u" != o && a != i) return a < i;
             n++
         }
-    }, o = e => {
+    }, a = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, a = 1; a < e.length; a++) n--, t += "u" == (typeof(l = e[a]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, l);
+            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(l = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, l);
             return t
         }
         var i = [];
-        for (a = 1; a < e.length; a++) {
-            var l = e[a];
-            i.push(0 === l ? "not(" + d() + ")" : 1 === l ? "(" + d() + " || " + d() + ")" : 2 === l ? i.pop() + " " + i.pop() : o(l))
+        for (o = 1; o < e.length; o++) {
+            var l = e[o];
+            i.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? i.pop() + " " + i.pop() : a(l))
         }
-        return d();
+        return u();
 
-        function d() {
+        function u() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, a = (e, r) => {
+    }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
-                o = n < 0;
-            o && (n = -n - 1);
-            for (var i = 0, l = 1, d = !0;; l++, i++) {
-                var u, s, f = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (s = (typeof(u = r[i]))[0])) return !d || ("u" == f ? l > n && !o : "" == f != o);
+                a = n < 0;
+            a && (n = -n - 1);
+            for (var i = 0, l = 1, u = !0;; l++, i++) {
+                var d, s, f = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (s = (typeof(d = r[i]))[0])) return !u || ("u" == f ? l > n && !a : "" == f != a);
                 if ("u" == s) {
-                    if (!d || "u" != f) return !1
-                } else if (d)
+                    if (!u || "u" != f) return !1
+                } else if (u)
                     if (f == s)
                         if (l <= n) {
-                            if (u != e[l]) return !1
+                            if (d != e[l]) return !1
                         } else {
-                            if (o ? u > e[l] : u < e[l]) return !1;
-                            u != e[l] && (d = !1)
+                            if (a ? d > e[l] : d < e[l]) return !1;
+                            d != e[l] && (u = !1)
                         }
                 else if ("s" != f && "n" != f) {
-                    if (o || l <= n) return !1;
-                    d = !1, l--
+                    if (a || l <= n) return !1;
+                    u = !1, l--
                 } else {
-                    if (l <= n || s < f != o) return !1;
-                    d = !1
-                } else "s" != f && "n" != f && (d = !1, l--)
+                    if (l <= n || s < f != a) return !1;
+                    u = !1
+                } else "s" != f && "n" != f && (u = !1, l--)
             }
         }
         var c = [],
             p = c.pop.bind(c);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? a(h, r) : !p())
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? o(h, r) : !p())
         }
         return !!p()
     }, i = (e, r) => {
         var t = S.S[e];
         if (!t || !S.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, d = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", u = (e, r, t, n) => {
-        var o = l(e, t);
-        return a(n, o) || f(d(e, t, o, n)), c(e[t][o])
+    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", d = (e, r, t, n) => {
+        var a = l(e, t);
+        return o(n, a) || f(u(e, t, a, n)), c(e[t][a])
     }, s = (e, r, t) => {
-        var o = e[r];
-        return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
+        var a = e[r];
+        return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
     }, f = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, o) {
-        var a = S.I(r);
-        return a && a.then ? a.then(e.bind(e, r, S.S[r], t, n, o)) : e(r, S.S[r], t, n, o)
-    })(((e, r, t, n) => (i(e, t), u(r, 0, t, n)))), v = p(((e, r, t, n, o) => {
-        var a = r && S.o(r, t) && s(r, t, n);
-        return a ? c(a) : o()
-    })), g = {}, b = {
+    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, n, a) {
+        var o = S.I(r);
+        return o && o.then ? o.then(e.bind(e, r, S.S[r], t, n, a)) : e(r, S.S[r], t, n, a)
+    })(((e, r, t, n) => (i(e, t), d(r, 0, t, n)))), v = p(((e, r, t, n, a) => {
+        var o = r && S.o(r, t) && s(r, t, n);
+        return o ? c(o) : a()
+    })), b = {}, g = {
         672: () => h("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 4],
             [1, 3],
             [1, 2],
             [1, 1, 1], 1, 1, 1, 1
         ]),
         297: () => v("default", "underscore", [1, 1, 13, 6], (() => S.e(794).then((() => () => S(794)))))
     }, m = {
         563: [297],
         672: [672]
     }, S.f.consumes = (e, r) => {
         S.o(m, e) && m[e].forEach((e => {
-            if (S.o(g, e)) return r.push(g[e]);
+            if (S.o(b, e)) return r.push(b[e]);
             var t = r => {
-                    g[e] = 0, S.m[e] = t => {
+                    b[e] = 0, S.m[e] = t => {
                         delete S.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete g[e], S.m[e] = t => {
+                    delete b[e], S.m[e] = t => {
                         throw delete S.c[e], r
                     }
                 };
             try {
-                var o = b[e]();
-                o.then ? r.push(g[e] = o.then(t).catch(n)) : t(o)
+                var a = g[e]();
+                a.then ? r.push(b[e] = a.then(t).catch(n)) : t(a)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             879: 0
         };
         S.f.j = (r, t) => {
             var n = S.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
                 else if (672 != r) {
-                var o = new Promise(((t, o) => n = e[r] = [t, o]));
-                t.push(n[2] = o);
-                var a = S.p + S.u(r),
+                var a = new Promise(((t, a) => n = e[r] = [t, a]));
+                t.push(n[2] = a);
+                var o = S.p + S.u(r),
                     i = new Error;
-                S.l(a, (t => {
+                S.l(o, (t => {
                     if (S.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
-                        var o = t && ("load" === t.type ? "missing" : t.type),
-                            a = t && t.target && t.target.src;
-                        i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + a + ")", i.name = "ChunkLoadError", i.type = o, i.request = a, n[1](i)
+                        var a = t && ("load" === t.type ? "missing" : t.type),
+                            o = t && t.target && t.target.src;
+                        i.message = "Loading chunk " + r + " failed.\n(" + a + ": " + o + ")", i.name = "ChunkLoadError", i.type = a, i.request = o, n[1](i)
                     }
                 }), "chunk-" + r, r)
             } else e[r] = 0
         };
         var r = (r, t) => {
-                var n, o, [a, i, l] = t,
-                    d = 0;
-                if (a.some((r => 0 !== e[r]))) {
+                var n, a, [o, i, l] = t,
+                    u = 0;
+                if (o.some((r => 0 !== e[r]))) {
                     for (n in i) S.o(i, n) && (S.m[n] = i[n]);
                     l && l(S)
                 }
-                for (r && r(t); d < a.length; d++) o = a[d], S.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); u < o.length; u++) a = o[u], S.o(e, a) && e[a] && e[a][0](), e[a] = 0
             },
             t = self.webpackChunkipyaladin = self.webpackChunkipyaladin || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
     var E = S(460);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).ipyaladin = E
 })();
```

### Comparing `ipyaladin-0.2.2/ipyaladin/labextension/static/third-party-licenses.json` & `ipyaladin-0.2.3/ipyaladin/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `ipyaladin-0.2.2/ipyaladin/nbextension/extension.js` & `ipyaladin-0.2.3/ipyaladin/nbextension/extension.js`

 * *Files identical despite different names*

### Comparing `ipyaladin-0.2.2/ipyaladin/nbextension/index.js` & `ipyaladin-0.2.3/ipyaladin/nbextension/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1406,16 +1406,16 @@
             defaults() {
                 return {
                     ...super.defaults(),
                     _model_name: "AladinModel",
                     _view_name: "AladinView",
                     _model_module: "ipyaladin",
                     _view_module: "ipyaladin",
-                    _model_module_version: "0.2.2",
-                    _view_module_version: "0.2.2"
+                    _model_module_version: "0.2.3",
+                    _view_module_version: "0.2.3"
                 }
             }
         }
         let a = 0;
         class u extends t.DOMWidgetView {
             render() {
                 n.then((() => {
@@ -1520,11 +1520,11 @@
                 })), this.listenTo(this.model, "change:color_map_flag", (() => {
                     const t = this.model.get("color_map_name");
                     this.al.getBaseImageLayer().setColormap(t)
                 }))
             }
         }
         const l = {
-            i8: "0.2.2"
+            i8: "0.2.3"
         }
     })(), o
 })()));
```

### Comparing `ipyaladin-0.2.2/ipyaladin.egg-info/PKG-INFO` & `ipyaladin-0.2.3/ipyaladin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyaladin
-Version: 0.2.2
+Version: 0.2.3
 Summary: ipyaladin
 Home-page: https://github.com/cds-astro/ipyaladin
 Author: Jerome Desroziers, Thomas Boch & Matthieu Baumann
 Author-email: matthieu.baumann@astro.unistra.fr
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/cds-astro/ipyaladin/issues
 Project-URL: Live Testing, https://mybinder.org/v2/gh/cds-astro/ipyaladin/master
@@ -19,17 +19,19 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Framework :: Jupyter
 Classifier: Framework :: Jupyter :: JupyterLab
 Classifier: Framework :: Jupyter :: JupyterLab :: 3
+Classifier: Framework :: Jupyter :: JupyterLab :: 4
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions
 Classifier: Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # ipyaladin
@@ -68,15 +70,15 @@
 And you are ready to use ipyaladin inside your notebooks!
 Additionny, for a jupyterlab usage you will need to:
 
     jupyter labextension develop ipyaladin --overwrite
 
 There is also a conda package that can be installed with:
 
-    conda install -c bmatthieu3 ipyaladin==0.2.2
+    conda install -c bmatthieu3 ipyaladin==0.2.3
 
 ## New features corner
 
 ![new_features](assets/new_features.gif)
 
 ## Development installation
```

### Comparing `ipyaladin-0.2.2/ipyaladin.egg-info/SOURCES.txt` & `ipyaladin-0.2.3/ipyaladin.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 ipyaladin.egg-info/PKG-INFO
 ipyaladin.egg-info/SOURCES.txt
 ipyaladin.egg-info/dependency_links.txt
 ipyaladin.egg-info/not-zip-safe
 ipyaladin.egg-info/requires.txt
 ipyaladin.egg-info/top_level.txt
 ipyaladin/labextension/package.json
-ipyaladin/labextension/static/563.b311860ae40bdaae42cf.js
-ipyaladin/labextension/static/590.9292295778c3653a0b31.js
+ipyaladin/labextension/static/563.9c25681782097966161a.js
+ipyaladin/labextension/static/590.b90399830948d2f839e2.js
 ipyaladin/labextension/static/794.644314dbf6493c3f7619.js
-ipyaladin/labextension/static/remoteEntry.c35d9bcfb9f9c1b91ff1.js
+ipyaladin/labextension/static/remoteEntry.baf7991223a7feb4e9c0.js
 ipyaladin/labextension/static/style.js
 ipyaladin/labextension/static/third-party-licenses.json
 ipyaladin/nbextension/extension.js
 ipyaladin/nbextension/index.js
 js/README.md
 js/amd-public-path.js
 js/package.json
```

### Comparing `ipyaladin-0.2.2/js/amd-public-path.js` & `ipyaladin-0.2.3/js/amd-public-path.js`

 * *Files identical despite different names*

### Comparing `ipyaladin-0.2.2/js/dist/index.js` & `ipyaladin-0.2.3/js/dist/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1406,16 +1406,16 @@
             defaults() {
                 return {
                     ...super.defaults(),
                     _model_name: "AladinModel",
                     _view_name: "AladinView",
                     _model_module: "ipyaladin",
                     _view_module: "ipyaladin",
-                    _model_module_version: "0.2.2",
-                    _view_module_version: "0.2.2"
+                    _model_module_version: "0.2.3",
+                    _view_module_version: "0.2.3"
                 }
             }
         }
         let a = 0;
         class u extends t.DOMWidgetView {
             render() {
                 n.then((() => {
@@ -1520,11 +1520,11 @@
                 })), this.listenTo(this.model, "change:color_map_flag", (() => {
                     const t = this.model.get("color_map_name");
                     this.al.getBaseImageLayer().setColormap(t)
                 }))
             }
         }
         const l = {
-            i8: "0.2.2"
+            i8: "0.2.3"
         }
     })(), o
 })()));
```

### Comparing `ipyaladin-0.2.2/js/lib/jupyter-aladin.js` & `ipyaladin-0.2.3/js/lib/jupyter-aladin.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -67,16 +67,16 @@
             ...super.defaults(),
             _model_name: 'AladinModel',
             _view_name: 'AladinView',
 
             _model_module: 'ipyaladin',
             _view_module: 'ipyaladin',
 
-            _model_module_version: '0.2.2',
-            _view_module_version: '0.2.2',
+            _model_module_version: '0.2.3',
+            _view_module_version: '0.2.3',
         };
     }
 }
 
 
 let idxView = 0;
 export class AladinView extends DOMWidgetView {
```

### Comparing `ipyaladin-0.2.2/js/package.json` & `ipyaladin-0.2.3/js/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9642857142857143%*

 * *Differences: {"'version'": "'0.2.3'"}*

```diff
@@ -44,9 +44,9 @@
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:prod": "webpack --mode=production && yarn run build:labextension",
         "clean": "rimraf dist/ && rimraf ../ipyaladin/labextension/ && rimraf ../ipyaladin/nbextension",
         "prepublish": "yarn run clean && yarn run build:prod",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch --mode=development"
     },
-    "version": "0.2.2"
+    "version": "0.2.3"
 }
```

### Comparing `ipyaladin-0.2.2/js/webpack.config.js` & `ipyaladin-0.2.3/js/webpack.config.js`

 * *Files identical despite different names*

### Comparing `ipyaladin-0.2.2/js/yarn.lock` & `ipyaladin-0.2.3/js/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -64,17 +64,17 @@
     "@types/backbone" "1.4.14"
     "@types/lodash" "^4.14.134"
     backbone "1.4.0"
     jquery "^3.1.1"
     lodash "^4.17.4"
 
 "@jupyterlab/builder@^3.0.0 || ^4.0.0":
-  version "4.0.0"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/builder/-/builder-4.0.0.tgz#5ae27d132d4b8adaefbed747931a609c6975ca96"
-  integrity sha512-x4rbN5eSc7Dy8ZVGoJPhiYT31J8j3FmI94m/fOvlvDP7wrZG0CbFCtEUD1QfCvEG7aHyLdPZL44FQEHg4BlDqg==
+  version "4.0.1"
+  resolved "https://registry.yarnpkg.com/@jupyterlab/builder/-/builder-4.0.1.tgz#4acf37d46fa68c06849acd5970c0f94a3a835a75"
+  integrity sha512-j1UWwRfZWeDR5Z72OGI406srr2HzxYi3chwnKCSxBA4mVgoJ4+ntRL/67q9K6cRvrUOsaVLTFHG1SKJ8S7w0ZA==
   dependencies:
     "@lumino/algorithm" "^2.0.0"
     "@lumino/application" "^2.1.1"
     "@lumino/commands" "^2.1.1"
     "@lumino/coreutils" "^2.1.1"
     "@lumino/disposable" "^2.1.1"
     "@lumino/domutils" "^2.0.0"
@@ -439,17 +439,17 @@
 
 "@types/lodash@^4.14.134":
   version "4.14.195"
   resolved "https://registry.yarnpkg.com/@types/lodash/-/lodash-4.14.195.tgz#bafc975b252eb6cea78882ce8a7b6bf22a6de632"
   integrity sha512-Hwx9EUgdwf2GLarOjQp5ZH8ZmblzcbTBC2wtQWNKARBSxM9ezRIAUpeDTgoQRAFB0+8CNWXVA9+MaSOzOF3nPg==
 
 "@types/node@*":
-  version "20.2.4"
-  resolved "https://registry.yarnpkg.com/@types/node/-/node-20.2.4.tgz#e6c3345f7ed9c6df41fdc288a94e2633167bc15d"
-  integrity sha512-ni5f8Xlf4PwnT/Z3f0HURc3ZSw8UyrqMqmM3L5ysa7VjHu8c3FOmIo1nKCcLrV/OAmtf3N4kFna/aJqxsfEtnA==
+  version "20.2.5"
+  resolved "https://registry.yarnpkg.com/@types/node/-/node-20.2.5.tgz#26d295f3570323b2837d322180dfbf1ba156fefb"
+  integrity sha512-JJulVEQXmiY9Px5axXHeYGLSjhkZEnD+MDPDGbCbIAbMslkKwmygtZFy1X6s/075Yo94sf8GuSlFfPzysQrWZQ==
 
 "@types/sizzle@*":
   version "2.3.3"
   resolved "https://registry.yarnpkg.com/@types/sizzle/-/sizzle-2.3.3.tgz#ff5e2f1902969d305225a047c8a0fd5c915cebef"
   integrity sha512-JYM8x9EGF163bEyhdJBpR2QX1R5naCJHC8ucJylJ3w9/CVBaskdQ8WqBf8MmQrd1kRvp/a4TS8HJ+bxzR7ZJYQ==
 
 "@types/source-list-map@*":
@@ -700,32 +700,32 @@
   resolved "https://registry.yarnpkg.com/brace-expansion/-/brace-expansion-1.1.11.tgz#3c7fcbf529d87226f3d2f52b966ff5271eb441dd"
   integrity sha512-iCuPHDFgrHX7H2vEI/5xpz07zSHB00TpugqhmYtVmMO6518mCuRMoOYFldEBl0g187ufozdaHgWKcYFb61qGiA==
   dependencies:
     balanced-match "^1.0.0"
     concat-map "0.0.1"
 
 browserslist@^4.14.5:
-  version "4.21.5"
-  resolved "https://registry.yarnpkg.com/browserslist/-/browserslist-4.21.5.tgz#75c5dae60063ee641f977e00edd3cfb2fb7af6a7"
-  integrity sha512-tUkiguQGW7S3IhB7N+c2MV/HZPSCPAAiYBZXLsBhFB/PCy6ZKKsZrmBayHV9fdGV/ARIfJ14NkxKzRDjvp7L6w==
-  dependencies:
-    caniuse-lite "^1.0.30001449"
-    electron-to-chromium "^1.4.284"
-    node-releases "^2.0.8"
-    update-browserslist-db "^1.0.10"
+  version "4.21.7"
+  resolved "https://registry.yarnpkg.com/browserslist/-/browserslist-4.21.7.tgz#e2b420947e5fb0a58e8f4668ae6e23488127e551"
+  integrity sha512-BauCXrQ7I2ftSqd2mvKHGo85XR0u7Ru3C/Hxsy/0TkfCtjrmAbPdzLGasmoiBxplpDXlPvdjX9u7srIMfgasNA==
+  dependencies:
+    caniuse-lite "^1.0.30001489"
+    electron-to-chromium "^1.4.411"
+    node-releases "^2.0.12"
+    update-browserslist-db "^1.0.11"
 
 buffer-from@^1.0.0:
   version "1.1.2"
   resolved "https://registry.yarnpkg.com/buffer-from/-/buffer-from-1.1.2.tgz#2b146a6fd72e80b4f55d255f35ed59a3a9a41bd5"
   integrity sha512-E+XQCRwSbaaiChtv6k6Dwgc+bx+Bs6vuKJHHl5kox/BaKbhiXzqQOwK4cO22yElGp2OCmjwVhT3HmxgyPGnJfQ==
 
-caniuse-lite@^1.0.30001449:
-  version "1.0.30001489"
-  resolved "https://registry.yarnpkg.com/caniuse-lite/-/caniuse-lite-1.0.30001489.tgz#ca82ee2d4e4dbf2bd2589c9360d3fcc2c7ba3bd8"
-  integrity sha512-x1mgZEXK8jHIfAxm+xgdpHpk50IN3z3q3zP261/WS+uvePxW8izXuCu6AHz0lkuYTlATDehiZ/tNyYBdSQsOUQ==
+caniuse-lite@^1.0.30001489:
+  version "1.0.30001491"
+  resolved "https://registry.yarnpkg.com/caniuse-lite/-/caniuse-lite-1.0.30001491.tgz#eab0e0f392de6f7411751d148de9b5bd6b203e46"
+  integrity sha512-17EYIi4TLnPiTzVKMveIxU5ETlxbSO3B6iPvMbprqnKh4qJsQGk5Nh1Lp4jIMAE0XfrujsJuWZAM3oJdMHaKBA==
 
 chalk@^2.3.0:
   version "2.4.2"
   resolved "https://registry.yarnpkg.com/chalk/-/chalk-2.4.2.tgz#cd42541677a54333cf541a49108c1432b44c9424"
   integrity sha512-Mti+f9lpJNcwF4tWV8/OrTTtF1gZi+f8FqlyAdouralcFWFQWF2+NgCHShjkCb+IFBLq9buZwE1xckQU4peSuQ==
   dependencies:
     ansi-styles "^3.2.1"
@@ -789,22 +789,22 @@
   integrity sha512-iRDPJKUPVEND7dHPO8rkbOnPpyDygcDFtWjpeWNCgy8WP2rXcxXL8TskReQl6OrB2G7+UJrags1q15Fudc7G6w==
   dependencies:
     path-key "^3.1.0"
     shebang-command "^2.0.0"
     which "^2.0.1"
 
 css-loader@^6.7.1:
-  version "6.7.4"
-  resolved "https://registry.yarnpkg.com/css-loader/-/css-loader-6.7.4.tgz#a5d8ec28a73f3e0823998cfee2a1f7e564b91f9b"
-  integrity sha512-0Y5uHtK5BswfaGJ+jrO+4pPg1msFBc0pwPIE1VqfpmVn6YbDfYfXMj8rfd7nt+4goAhJueO+H/I40VWJfcP1mQ==
+  version "6.8.1"
+  resolved "https://registry.yarnpkg.com/css-loader/-/css-loader-6.8.1.tgz#0f8f52699f60f5e679eab4ec0fcd68b8e8a50a88"
+  integrity sha512-xDAXtEVGlD0gJ07iclwWVkLoZOpEvAWaSyf6W18S2pOC//K8+qUDIx8IIT3D+HjnmkJPQeesOPv5aiUaJsCM2g==
   dependencies:
     icss-utils "^5.1.0"
     postcss "^8.4.21"
     postcss-modules-extract-imports "^3.0.0"
-    postcss-modules-local-by-default "^4.0.1"
+    postcss-modules-local-by-default "^4.0.3"
     postcss-modules-scope "^3.0.0"
     postcss-modules-values "^4.0.0"
     postcss-value-parser "^4.2.0"
     semver "^7.3.8"
 
 cssesc@^3.0.0:
   version "3.0.0"
@@ -826,18 +826,18 @@
   integrity sha512-aO50/qPC7X2ChjRFniRiscxBLT/K01bALqfcDaf8Ih5OqQ1N4iT/Abx9Ofu3/ms446vHTm46FACIuJUmgUQcDQ==
   dependencies:
     chalk "^2.3.0"
     find-root "^1.0.0"
     lodash "^4.17.4"
     semver "^5.4.1"
 
-electron-to-chromium@^1.4.284:
-  version "1.4.408"
-  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.408.tgz#73e657a24bd0b7481d68c943dded0d097b0d0a52"
-  integrity sha512-vjeaj0u/UYnzA/CIdGXzzcxRLCqRwREYc9YfaWInjIEr7/XPttZ6ShpyqapchEy0S2r6LpLjDBTnNj7ZxnxJKg==
+electron-to-chromium@^1.4.411:
+  version "1.4.413"
+  resolved "https://registry.yarnpkg.com/electron-to-chromium/-/electron-to-chromium-1.4.413.tgz#0067c3122946ae234cbefb9401ecefde851cdcf2"
+  integrity sha512-Gd+/OAhRca06dkVxIQo/W7dr6Nmk9cx6lQdZ19GvFp51k5B/lUAokm6SJfNkdV8kFLsC3Z4sLTyEHWCnB1Efbw==
 
 emojis-list@^3.0.0:
   version "3.0.0"
   resolved "https://registry.yarnpkg.com/emojis-list/-/emojis-list-3.0.0.tgz#5570662046ad29e2e916e71aae260abdff4f6a78"
   integrity sha512-/kyM18EfinwXZbno9FyUGeFh87KC8HRQBQGildHZbEuRyWFOmv1U10o9BBp8XVZDVNNuQKyIGIu5ZYAAXJ0V2Q==
 
 enhanced-resolve@^5.14.1:
@@ -1206,15 +1206,15 @@
 node-fetch@^2.6.0:
   version "2.6.11"
   resolved "https://registry.yarnpkg.com/node-fetch/-/node-fetch-2.6.11.tgz#cde7fc71deef3131ef80a738919f999e6edfff25"
   integrity sha512-4I6pdBY1EthSqDmJkiNk3JIT8cswwR9nfeW/cPdUagJYEQG7R95WRH74wpz7ma8Gh/9dI9FP+OU+0E4FvtA55w==
   dependencies:
     whatwg-url "^5.0.0"
 
-node-releases@^2.0.8:
+node-releases@^2.0.12:
   version "2.0.12"
   resolved "https://registry.yarnpkg.com/node-releases/-/node-releases-2.0.12.tgz#35627cc224a23bfb06fb3380f2b3afaaa7eb1039"
   integrity sha512-QzsYKWhXTWx8h1kIvqfnC++o0pEmpRQA/aenALsL2F4pqNVr7YzcdMlDij5WBnwftRbJCNJL/O7zdKaxKPHqgQ==
 
 once@^1.3.0:
   version "1.4.0"
   resolved "https://registry.yarnpkg.com/once/-/once-1.4.0.tgz#583b1aa775961d4b113ac17d9c50baef9dd76bd1"
@@ -1279,15 +1279,15 @@
     find-up "^4.0.0"
 
 postcss-modules-extract-imports@^3.0.0:
   version "3.0.0"
   resolved "https://registry.yarnpkg.com/postcss-modules-extract-imports/-/postcss-modules-extract-imports-3.0.0.tgz#cda1f047c0ae80c97dbe28c3e76a43b88025741d"
   integrity sha512-bdHleFnP3kZ4NYDhuGlVK+CMrQ/pqUm8bx/oGL93K6gVwiclvX5x0n76fYMKuIGKzlABOy13zsvqjb0f92TEXw==
 
-postcss-modules-local-by-default@^4.0.1:
+postcss-modules-local-by-default@^4.0.3:
   version "4.0.3"
   resolved "https://registry.yarnpkg.com/postcss-modules-local-by-default/-/postcss-modules-local-by-default-4.0.3.tgz#b08eb4f083050708998ba2c6061b50c2870ca524"
   integrity sha512-2/u2zraspoACtrbFRnTijMiQtb4GW4BvatjaG/bCjYQo8kLTdevCUlwuBHx2sCnSyrI3x3qj4ZK1j5LQBgzmwA==
   dependencies:
     icss-utils "^5.0.0"
     postcss-selector-parser "^6.0.2"
     postcss-value-parser "^4.1.0"
@@ -1316,17 +1316,17 @@
 
 postcss-value-parser@^4.1.0, postcss-value-parser@^4.2.0:
   version "4.2.0"
   resolved "https://registry.yarnpkg.com/postcss-value-parser/-/postcss-value-parser-4.2.0.tgz#723c09920836ba6d3e5af019f92bc0971c02e514"
   integrity sha512-1NNCs6uurfkVbeXG4S8JFT9t19m45ICnif8zWLd5oPSZ50QnwMfK+H3jv408d4jw/7Bttv5axS5IiHoLaVNHeQ==
 
 postcss@^8.4.21:
-  version "8.4.23"
-  resolved "https://registry.yarnpkg.com/postcss/-/postcss-8.4.23.tgz#df0aee9ac7c5e53e1075c24a3613496f9e6552ab"
-  integrity sha512-bQ3qMcpF6A/YjR55xtoTr0jGOlnPOKAIMdOWiv0EIT6HVPEaJiJB4NLljSbiHoC2RX7DN5Uvjtpbg1NPdwv1oA==
+  version "8.4.24"
+  resolved "https://registry.yarnpkg.com/postcss/-/postcss-8.4.24.tgz#f714dba9b2284be3cc07dbd2fc57ee4dc972d2df"
+  integrity sha512-M0RzbcI0sO/XJNucsGjvWU9ERWxb/ytp1w6dKtxTKgixdtQDq4rmx/g8W1hnaheq9jgwL/oyEdH5Bc4WwJKMqg==
   dependencies:
     nanoid "^3.3.6"
     picocolors "^1.0.0"
     source-map-js "^1.0.2"
 
 process@^0.11.10:
   version "0.11.10"
@@ -1580,15 +1580,15 @@
   integrity sha512-+A5Sja4HP1M08MaXya7p5LvjuM7K6q/2EaC0+iovj/wOcMsTzMvDFbasi/oSapiwOlt252IqsKqPjCl7huKS0A==
 
 universalify@^2.0.0:
   version "2.0.0"
   resolved "https://registry.yarnpkg.com/universalify/-/universalify-2.0.0.tgz#75a4984efedc4b08975c5aeb73f530d02df25717"
   integrity sha512-hAZsKq7Yy11Zu1DE0OzWjw7nnLZmJZYTDZZyEFHZdUhV8FkH5MCfoU1XMaxXovpyW5nq5scPqq0ZDP9Zyl04oQ==
 
-update-browserslist-db@^1.0.10:
+update-browserslist-db@^1.0.11:
   version "1.0.11"
   resolved "https://registry.yarnpkg.com/update-browserslist-db/-/update-browserslist-db-1.0.11.tgz#9a2a641ad2907ae7b3616506f4b977851db5b940"
   integrity sha512-dCwEFf0/oT85M1fHBg4F0jtLwJrutGoHSQXCh7u4o2t1drG+c0a9Flnqww6XUKSfQMPpJBRjU8d4RXB09qtvaA==
   dependencies:
     escalade "^3.1.1"
     picocolors "^1.0.0"
```

### Comparing `ipyaladin-0.2.2/setup.cfg` & `ipyaladin-0.2.3/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -23,25 +23,27 @@
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Programming Language :: Python
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Framework :: Jupyter
 	Framework :: Jupyter :: JupyterLab
 	Framework :: Jupyter :: JupyterLab :: 3
+	Framework :: Jupyter :: JupyterLab :: 4
 	Framework :: Jupyter :: JupyterLab :: Extensions
 	Framework :: Jupyter :: JupyterLab :: Extensions :: Prebuilt
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
-	ipywidgets>=7.6.0,<9
+	ipywidgets>=8.0.6,<9
 python_requires = >=3.7
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `ipyaladin-0.2.2/setup.py` & `ipyaladin-0.2.3/setup.py`

 * *Files identical despite different names*

