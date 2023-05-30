# Comparing `tmp/tiledb_jupyter_bioimg-0.1.1a1.tar.gz` & `tmp/tiledb_jupyter_bioimg-0.1.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiledb_jupyter_bioimg-0.1.1a1.tar", last modified: Tue May 30 10:17:56 2023, max compression
+gzip compressed data, was "tiledb_jupyter_bioimg-0.1.1a2.tar", last modified: Tue May 30 11:37:45 2023, max compression
```

## Comparing `tiledb_jupyter_bioimg-0.1.1a1.tar` & `tiledb_jupyter_bioimg-0.1.1a2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:17:56.632812 tiledb_jupyter_bioimg-0.1.1a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-30 10:13:58.000000 tiledb_jupyter_bioimg-0.1.1a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-30 10:13:58.000000 tiledb_jupyter_bioimg-0.1.1a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-30 10:17:56.632812 tiledb_jupyter_bioimg-0.1.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-30 10:13:58.000000 tiledb_jupyter_bioimg-0.1.1a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-30 10:13:58.000000 tiledb_jupyter_bioimg-0.1.1a1/install.json
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-30 10:15:52.000000 tiledb_jupyter_bioimg-0.1.1a1/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-30 10:13:58.000000 tiledb_jupyter_bioimg-0.1.1a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 10:17:56.632812 tiledb_jupyter_bioimg-0.1.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-30 10:13:58.000000 tiledb_jupyter_bioimg-0.1.1a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:17:56.624812 tiledb_jupyter_bioimg-0.1.1a1/src/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-30 10:13:58.000000 tiledb_jupyter_bioimg-0.1.1a1/src/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-30 10:13:58.000000 tiledb_jupyter_bioimg-0.1.1a1/src/version.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-30 10:13:58.000000 tiledb_jupyter_bioimg-0.1.1a1/src/widget.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:17:56.624812 tiledb_jupyter_bioimg-0.1.1a1/style/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 10:13:58.000000 tiledb_jupyter_bioimg-0.1.1a1/style/base.css
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 10:13:58.000000 tiledb_jupyter_bioimg-0.1.1a1/style/index.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-30 10:13:58.000000 tiledb_jupyter_bioimg-0.1.1a1/style/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:17:56.624812 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-30 10:13:58.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-30 10:13:58.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-30 10:13:58.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:17:56.628812 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-30 10:17:55.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:17:56.632812 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)   189298 2023-05-30 10:17:55.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14610 2023-05-30 10:17:55.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/172.6267f3dd3063477e34ed.js
--rw-r--r--   0 runner    (1001) docker     (123)   725916 2023-05-30 10:17:55.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/344.8db93920a8ca0f0600d9.js
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-30 10:17:55.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/344.8db93920a8ca0f0600d9.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-30 10:17:55.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-30 10:17:55.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/633.770b26571c8b948a69e3.js
--rw-r--r--   0 runner    (1001) docker     (123)   516691 2023-05-30 10:17:55.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-30 10:17:55.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   172313 2023-05-30 10:17:55.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/713.44bebcfa12a45c30ff83.js
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-30 10:17:55.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/713.44bebcfa12a45c30ff83.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-05-30 10:17:55.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/744.33b070180c108b7cf8c9.js
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-30 10:17:55.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js
--rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-05-30 10:17:55.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/remoteEntry.b0daa29a1375bdb34258.js
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-30 10:17:31.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)    90733 2023-05-30 10:17:55.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-30 10:13:58.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:17:56.628812 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-30 10:17:56.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-30 10:17:56.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:17:56.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:16:49.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-30 10:17:56.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 10:17:56.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-30 10:13:58.000000 tiledb_jupyter_bioimg-0.1.1a1/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:37:45.178763 tiledb_jupyter_bioimg-0.1.1a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-30 11:32:53.000000 tiledb_jupyter_bioimg-0.1.1a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-30 11:32:53.000000 tiledb_jupyter_bioimg-0.1.1a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-30 11:37:45.178763 tiledb_jupyter_bioimg-0.1.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-30 11:32:53.000000 tiledb_jupyter_bioimg-0.1.1a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-30 11:32:53.000000 tiledb_jupyter_bioimg-0.1.1a2/install.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-30 11:35:14.000000 tiledb_jupyter_bioimg-0.1.1a2/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-30 11:32:53.000000 tiledb_jupyter_bioimg-0.1.1a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 11:37:45.178763 tiledb_jupyter_bioimg-0.1.1a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-30 11:32:53.000000 tiledb_jupyter_bioimg-0.1.1a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:37:45.174762 tiledb_jupyter_bioimg-0.1.1a2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-30 11:32:53.000000 tiledb_jupyter_bioimg-0.1.1a2/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-30 11:32:53.000000 tiledb_jupyter_bioimg-0.1.1a2/src/version.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-30 11:32:53.000000 tiledb_jupyter_bioimg-0.1.1a2/src/widget.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:37:45.174762 tiledb_jupyter_bioimg-0.1.1a2/style/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:32:53.000000 tiledb_jupyter_bioimg-0.1.1a2/style/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 11:32:53.000000 tiledb_jupyter_bioimg-0.1.1a2/style/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-30 11:32:53.000000 tiledb_jupyter_bioimg-0.1.1a2/style/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:37:45.174762 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-30 11:32:53.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-30 11:32:53.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-30 11:32:53.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:37:45.174762 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-30 11:37:43.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:37:45.178763 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   189298 2023-05-30 11:37:43.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14610 2023-05-30 11:37:43.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/172.6267f3dd3063477e34ed.js
+-rw-r--r--   0 runner    (1001) docker     (123)   725916 2023-05-30 11:37:43.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/344.8db93920a8ca0f0600d9.js
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-30 11:37:43.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/344.8db93920a8ca0f0600d9.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-30 11:37:43.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-30 11:37:43.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/633.86ebe895050415abdfba.js
+-rw-r--r--   0 runner    (1001) docker     (123)   516693 2023-05-30 11:37:43.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/635.ce138c9764842046bf90.js
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-30 11:37:43.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/635.ce138c9764842046bf90.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   172313 2023-05-30 11:37:43.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/713.44bebcfa12a45c30ff83.js
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-30 11:37:43.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/713.44bebcfa12a45c30ff83.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-05-30 11:37:43.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/744.9655cb2c54e12e1c2654.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-30 11:37:43.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-05-30 11:37:43.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/remoteEntry.f05f71ea95cf3364c4cb.js
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-30 11:37:12.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)    90733 2023-05-30 11:37:43.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-30 11:32:53.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:37:45.174762 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-30 11:37:45.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-30 11:37:45.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:37:45.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:36:21.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-30 11:37:45.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 11:37:45.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-30 11:32:53.000000 tiledb_jupyter_bioimg-0.1.1a2/tsconfig.json
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a1/LICENSE` & `tiledb_jupyter_bioimg-0.1.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a1/PKG-INFO` & `tiledb_jupyter_bioimg-0.1.1a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledb_jupyter_bioimg
-Version: 0.1.1a1
+Version: 0.1.1a2
 Summary: A jupyterlab extension to visualize bioimages in TileDB format
 Home-page: https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer
 Author: TileDB
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a1/README.md` & `tiledb_jupyter_bioimg-0.1.1a2/README.md`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a1/package.json` & `tiledb_jupyter_bioimg-0.1.1a2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9736842105263158%*

 * *Differences: {"'version'": "'0.1.1-alpha.2'"}*

```diff
@@ -67,9 +67,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.1-alpha.1"
+    "version": "0.1.1-alpha.2"
 }
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a1/setup.py` & `tiledb_jupyter_bioimg-0.1.1a2/setup.py`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a1/src/index.ts` & `tiledb_jupyter_bioimg-0.1.1a2/src/index.ts`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a1/src/version.ts` & `tiledb_jupyter_bioimg-0.1.1a2/src/version.ts`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a1/src/widget.ts` & `tiledb_jupyter_bioimg-0.1.1a2/src/widget.ts`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/_version.py` & `tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/_version.py`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/package.json` & `tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9731359649122806%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.f05f71ea95cf3364c4cb.js'}}",*

 * * "'version'": "'0.1.1-alpha.2'"}*

```diff
@@ -27,15 +27,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.b0daa29a1375bdb34258.js",
+            "load": "static/remoteEntry.f05f71ea95cf3364c4cb.js",
             "style": "./style"
         },
         "extension": "lib/index",
         "outputDir": "tiledb_jupyter_bioimg/labextension",
         "webpackConfig": "./webpack.config.js"
     },
     "keywords": [
@@ -72,9 +72,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.1-alpha.1"
+    "version": "0.1.1-alpha.2"
 }
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg` & `tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/172.6267f3dd3063477e34ed.js` & `tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/172.6267f3dd3063477e34ed.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/344.8db93920a8ca0f0600d9.js` & `tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/344.8db93920a8ca0f0600d9.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/633.770b26571c8b948a69e3.js` & `tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/633.86ebe895050415abdfba.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -45,45 +45,45 @@
                         c = e.data.axes.indexOf("X"),
                         u = e.data.axes.indexOf("Y"),
                         p = e.data.axes.indexOf("C"),
                         d = new Array(3);
                     d[c] = [i * l * a, Math.min((i + 1) * l * a, e.data.levelWidth) - 1], d[u] = [s * l * a, Math.min((s + 1) * l * a, e.data.levelHeight) - 1], d[p] = e.data.channelRanges;
                     const y = (d[c][1] - d[c][0] + 1) / a,
                         h = (d[u][1] - d[u][0] + 1) / a;
-                    let b = 0;
-                    if ("number" == typeof d[p][0]) b = d[p][1] - d[p][0] + 1;
+                    let v = 0;
+                    if ("number" == typeof d[p][0]) v = d[p][1] - d[p][0] + 1;
                     else
-                        for (const e of d[p]) b += e[1] - e[0] + 1;
-                    const v = {
+                        for (const e of d[p]) v += e[1] - e[0] + 1;
+                    const m = {
                             layout: "row-major",
                             ranges: d,
-                            bufferSize: Math.pow(l * a, 2) * b * o[f].bytes,
+                            bufferSize: Math.pow(l * a, 2) * v * o[f].bytes,
                             attributes: ["intensity"],
                             returnRawBuffers: !0
                         },
-                        m = r.query.ReadQuery(e.data.namespace, e.data.levelUri, v),
-                        g = o[f].create(await m.next().then((e => e.value.intensity))),
-                        w = o[f].create(y * h * b),
+                        b = r.query.ReadQuery(e.data.namespace, e.data.levelUri, m),
+                        g = o[f].create(await b.next().then((e => e.value.intensity))),
+                        w = o[f].create(y * h * v),
                         E = new Array(3);
                     for (let e = 0; e < d.length; ++e) E[e] = d[e][1] - d[e][0] + 1;
                     1 === a ? self.postMessage({
                         data: g,
                         width: y,
                         height: h,
-                        channels: b
+                        channels: v
                     }, [g.buffer]) : (g.forEach(((e, t) => {
                         const r = new Array(3);
                         r[0] = ~~(t / (E[1] * E[2])), r[1] = ~~(t % (E[1] * E[2]) / E[2]), r[2] = t % E[2];
                         const n = (r[p] * h + ~~(r[u] / a)) * y + ~~(r[c] / a);
                         w[n] = e
                     })), self.postMessage({
                         data: w,
                         width: y,
                         height: h,
-                        channels: b
+                        channels: v
                     }, [w.buffer]))
                 }
             },
             8291: () => {},
             4447: () => {}
         },
         a = {};
@@ -121,15 +121,15 @@
             a: t
         }), t
     }, n.d = (e, t) => {
         for (var r in t) n.o(t, r) && !n.o(e, r) && Object.defineProperty(e, r, {
             enumerable: !0,
             get: t[r]
         })
-    }, n.f = {}, n.e = e => Promise.all(Object.keys(n.f).reduce(((t, r) => (n.f[r](e, t), t)), [])), n.u = e => e + ".024275f22a135fe53126.js?v=024275f22a135fe53126", n.g = function() {
+    }, n.f = {}, n.e = e => Promise.all(Object.keys(n.f).reduce(((t, r) => (n.f[r](e, t), t)), [])), n.u = e => e + ".ce138c9764842046bf90.js?v=ce138c9764842046bf90", n.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), n.o = (e, t) => Object.prototype.hasOwnProperty.call(e, t), n.r = e => {
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js` & `tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/635.ce138c9764842046bf90.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 635.024275f22a135fe53126.js.LICENSE.txt */
+/*! For license information please see 635.ce138c9764842046bf90.js.LICENSE.txt */
 (self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer = self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer || []).push([
     [635], {
         9757: (t, e, r) => {
             "use strict";
             r.d(e, {
                 Z: () => i
             });
@@ -13528,15 +13528,15 @@
                 }, e._capnp = {
                     displayName: "List<Float32>",
                     size: n.ListElementSize.BYTE_4
                 }, e
             }(a.List);
             e.Float32List = c
         },
-        404: (t, e, r) => {
+        5659: (t, e, r) => {
             "use strict";
             Object.defineProperty(e, "__esModule", {
                 value: !0
             });
             var i = r(655),
                 s = r(3834),
                 n = r(4064),
@@ -13575,15 +13575,15 @@
             e.CompositeList = n.CompositeList;
             var a = r(2981);
             e.Data = a.Data;
             var o = r(1738);
             e.DataList = o.DataList;
             var c = r(4951);
             e.Float32List = c.Float32List;
-            var u = r(404);
+            var u = r(5659);
             e.Float64List = u.Float64List;
             var p = r(1273);
             e.Int8List = p.Int8List;
             var d = r(1802);
             e.Int16List = d.Int16List;
             var l = r(5452);
             e.Int32List = l.Int32List;
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js.LICENSE.txt` & `tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/635.ce138c9764842046bf90.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/713.44bebcfa12a45c30ff83.js` & `tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/713.44bebcfa12a45c30ff83.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/744.33b070180c108b7cf8c9.js` & `tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/744.9655cb2c54e12e1c2654.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -53,11 +53,11 @@
                         version: r,
                         exports: l
                     })
                 }
             }
         },
         4147: e => {
-            e.exports = JSON.parse('{"name":"@tiledb-inc/jupyter-bioimage-viewer","version":"0.1.1-alpha.1","description":"A jupyterlab extension to visualize bioimages in TileDB format","keywords":["jupyter","jupyterlab","jupyterlab-extension"],"homepage":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer","bugs":{"url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer/issues"},"license":"BSD-3-Clause","author":"TileDB","files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","style/*.css","style/index.js"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","repository":{"type":"git","url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer.git"},"scripts":{"test":"echo No tests yet","build":"jlpm run build:lib && jlpm run build:labextension:dev","build:prod":"jlpm run build:lib && jlpm run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","clean":"jlpm run clean:lib","clean:lib":"rimraf lib tsconfig.tsbuildinfo","clean:labextension":"rimraf tiledb_jupyter_bioimg/labextension","clean:all":"jlpm run clean:lib && jlpm run clean:labextension","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:extension":"jupyter labextension develop --overwrite .","prepare":"jlpm run clean && jlpm run build:prod","watch":"run-p watch:src watch:labextension","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4","@jupyterlab/application":"^3.4.5","@tiledb-inc/bioimage-viewer":"^0.1.0-alpha.7"},"devDependencies":{"@jupyterlab/builder":"^3.1.0","@typescript-eslint/eslint-plugin":"^2.27.0","@typescript-eslint/parser":"^2.27.0","eslint":"^7.5.0","eslint-config-prettier":"^6.10.1","eslint-plugin-prettier":"^3.1.2","npm-run-all":"^4.1.5","prettier":"^1.19.0","rimraf":"^3.0.2","typescript":"~4.1.3"},"sideEffects":["style/*.css","style/index.js"],"styleModule":"style/index.js","jupyterlab":{"extension":"lib/index","outputDir":"tiledb_jupyter_bioimg/labextension","webpackConfig":"./webpack.config.js"}}')
+            e.exports = JSON.parse('{"name":"@tiledb-inc/jupyter-bioimage-viewer","version":"0.1.1-alpha.2","description":"A jupyterlab extension to visualize bioimages in TileDB format","keywords":["jupyter","jupyterlab","jupyterlab-extension"],"homepage":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer","bugs":{"url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer/issues"},"license":"BSD-3-Clause","author":"TileDB","files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","style/*.css","style/index.js"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","repository":{"type":"git","url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer.git"},"scripts":{"test":"echo No tests yet","build":"jlpm run build:lib && jlpm run build:labextension:dev","build:prod":"jlpm run build:lib && jlpm run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","clean":"jlpm run clean:lib","clean:lib":"rimraf lib tsconfig.tsbuildinfo","clean:labextension":"rimraf tiledb_jupyter_bioimg/labextension","clean:all":"jlpm run clean:lib && jlpm run clean:labextension","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:extension":"jupyter labextension develop --overwrite .","prepare":"jlpm run clean && jlpm run build:prod","watch":"run-p watch:src watch:labextension","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4","@jupyterlab/application":"^3.4.5","@tiledb-inc/bioimage-viewer":"^0.1.0-alpha.7"},"devDependencies":{"@jupyterlab/builder":"^3.1.0","@typescript-eslint/eslint-plugin":"^2.27.0","@typescript-eslint/parser":"^2.27.0","eslint":"^7.5.0","eslint-config-prettier":"^6.10.1","eslint-plugin-prettier":"^3.1.2","npm-run-all":"^4.1.5","prettier":"^1.19.0","rimraf":"^3.0.2","typescript":"~4.1.3"},"sideEffects":["style/*.css","style/index.js"],"styleModule":"style/index.js","jupyterlab":{"extension":"lib/index","outputDir":"tiledb_jupyter_bioimg/labextension","webpackConfig":"./webpack.config.js"}}')
         }
     }
 ]);
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js` & `tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/remoteEntry.b0daa29a1375bdb34258.js` & `tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/remoteEntry.f05f71ea95cf3364c4cb.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, n, i, o, d, l, u, s, f, c, p, h, b, v, m, g, y = {
+    var e, r, t, a, n, i, o, d, l, u, f, s, c, p, h, b, v, m, g, y = {
             5290: (e, r, t) => {
                 var a = {
                         "./index": () => t.e(744).then((() => () => t(1744))),
                         "./extension": () => t.e(744).then((() => () => t(1744))),
                         "./style": () => t.e(747).then((() => () => t(9747)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
@@ -48,28 +48,28 @@
             get: r[t]
         })
     }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
         38: "06c00f555d53e8ae5aa5",
         172: "6267f3dd3063477e34ed",
         344: "8db93920a8ca0f0600d9",
         446: "3bf34f45c93ace9c0f28",
-        633: "770b26571c8b948a69e3",
-        635: "024275f22a135fe53126",
+        633: "86ebe895050415abdfba",
+        635: "ce138c9764842046bf90",
         713: "44bebcfa12a45c30ff83",
-        744: "33b070180c108b7cf8c9",
+        744: "9655cb2c54e12e1c2654",
         747: "433530952542f03ebc71"
     } [e] + ".js?v=" + {
         38: "06c00f555d53e8ae5aa5",
         172: "6267f3dd3063477e34ed",
         344: "8db93920a8ca0f0600d9",
         446: "3bf34f45c93ace9c0f28",
-        633: "770b26571c8b948a69e3",
-        635: "024275f22a135fe53126",
+        633: "86ebe895050415abdfba",
+        635: "ce138c9764842046bf90",
         713: "44bebcfa12a45c30ff83",
-        744: "33b070180c108b7cf8c9",
+        744: "9655cb2c54e12e1c2654",
         747: "433530952542f03ebc71"
     } [e], j.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
@@ -81,31 +81,31 @@
         }
     }), e), j.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@tiledb-inc/jupyter-bioimage-viewer:", j.l = (t, a, n, i) => {
         if (e[t]) e[t].push(a);
         else {
             var o, d;
             if (void 0 !== n)
                 for (var l = document.getElementsByTagName("script"), u = 0; u < l.length; u++) {
-                    var s = l[u];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + n) {
-                        o = s;
+                    var f = l[u];
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + n) {
+                        o = f;
                         break
                     }
                 }
             o || (d = !0, (o = document.createElement("script")).charset = "utf-8", o.timeout = 120, j.nc && o.setAttribute("nonce", j.nc), o.setAttribute("data-webpack", r + n), o.src = t), e[t] = [a];
-            var f = (r, a) => {
+            var s = (r, a) => {
                     o.onerror = o.onload = null, clearTimeout(c);
                     var n = e[t];
                     if (delete e[t], o.parentNode && o.parentNode.removeChild(o), n && n.forEach((e => e(a))), r) return r(a)
                 },
-                c = setTimeout(f.bind(null, void 0, {
+                c = setTimeout(s.bind(null, void 0, {
                     type: "timeout",
                     target: o
                 }), 12e4);
-            o.onerror = f.bind(null, o.onerror), o.onload = f.bind(null, o.onload), d && document.head.appendChild(o)
+            o.onerror = s.bind(null, o.onerror), o.onload = s.bind(null, o.onload), d && document.head.appendChild(o)
         }
     }, j.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -127,15 +127,15 @@
                         (!d || !d.loaded && (!a != !d.eager ? a : o > d.from)) && (n[r] = {
                             get: t,
                             from: o,
                             eager: !!a
                         })
                     },
                     l = [];
-                return "default" === t && (d("@jupyter-widgets/base", "4.1.1", (() => Promise.all([j.e(172), j.e(713), j.e(38)]).then((() => () => j(2713))))), d("@tiledb-inc/bioimage-viewer", "0.1.0-alpha.7", (() => Promise.all([j.e(635), j.e(172), j.e(344), j.e(446)]).then((() => () => j(344))))), d("@tiledb-inc/jupyter-bioimage-viewer", "0.1.1-alpha.1", (() => j.e(744).then((() => () => j(1744)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (d("@jupyter-widgets/base", "4.1.1", (() => Promise.all([j.e(172), j.e(713), j.e(38)]).then((() => () => j(2713))))), d("@tiledb-inc/bioimage-viewer", "0.1.0-alpha.7", (() => Promise.all([j.e(635), j.e(172), j.e(344), j.e(446)]).then((() => () => j(344))))), d("@tiledb-inc/jupyter-bioimage-viewer", "0.1.1-alpha.2", (() => j.e(744).then((() => () => j(1744)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -185,33 +185,33 @@
     }, i = (e, r) => {
         if (0 in e) {
             r = t(r);
             var a = e[0],
                 n = a < 0;
             n && (a = -a - 1);
             for (var o = 0, d = 1, l = !0;; d++, o++) {
-                var u, s, f = d < e.length ? (typeof e[d])[0] : "";
-                if (o >= r.length || "o" == (s = (typeof(u = r[o]))[0])) return !l || ("u" == f ? d > a && !n : "" == f != n);
-                if ("u" == s) {
-                    if (!l || "u" != f) return !1
+                var u, f, s = d < e.length ? (typeof e[d])[0] : "";
+                if (o >= r.length || "o" == (f = (typeof(u = r[o]))[0])) return !l || ("u" == s ? d > a && !n : "" == s != n);
+                if ("u" == f) {
+                    if (!l || "u" != s) return !1
                 } else if (l)
-                    if (f == s)
+                    if (s == f)
                         if (d <= a) {
                             if (u != e[d]) return !1
                         } else {
                             if (n ? u > e[d] : u < e[d]) return !1;
                             u != e[d] && (l = !1)
                         }
-                else if ("s" != f && "n" != f) {
+                else if ("s" != s && "n" != s) {
                     if (n || d <= a) return !1;
                     l = !1, d--
                 } else {
-                    if (d <= a || s < f != n) return !1;
+                    if (d <= a || f < s != n) return !1;
                     l = !1
-                } else "s" != f && "n" != f && (l = !1, d--)
+                } else "s" != s && "n" != s && (l = !1, d--)
             }
         }
         var c = [],
             p = c.pop.bind(c);
         for (o = 1; o < e.length; o++) {
             var h = e[o];
             c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? i(h, r) : !p())
@@ -222,25 +222,25 @@
         if (!t || !j.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, d = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
     }, l = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", u = (e, r, t, a) => {
         var n = d(e, t);
-        return i(a, n) || f(l(e, t, n, a)), c(e[t][n])
-    }, s = (e, r, t) => {
+        return i(a, n) || s(l(e, t, n, a)), c(e[t][n])
+    }, f = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !i(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
-    }, f = e => {
+    }, s = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, a, n) {
         var i = j.I(r);
         return i && i.then ? i.then(e.bind(e, r, j.S[r], t, a, n)) : e(r, j.S[r], t, a, n)
     })(((e, r, t, a) => (o(e, t), u(r, 0, t, a)))), b = p(((e, r, t, a, n) => {
-        var i = r && j.o(r, t) && s(r, t, a);
+        var i = r && j.o(r, t) && f(r, t, a);
         return i ? c(i) : n()
     })), v = {}, m = {
         2832: () => b("default", "@tiledb-inc/bioimage-viewer", [2, 0, 1, 0, , "alpha", 7], (() => Promise.all([j.e(635), j.e(172), j.e(344), j.e(446)]).then((() => () => j(344))))),
         8233: () => b("default", "@jupyter-widgets/base", [, [1, 4],
             [1, 3],
             [1, 2],
             [1, 1, 1, 10], 1, 1, 1
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json` & `tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/render.py` & `tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/render.py`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg.egg-info/PKG-INFO` & `tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledb-jupyter-bioimg
-Version: 0.1.1a1
+Version: 0.1.1a2
 Summary: A jupyterlab extension to visualize bioimages in TileDB format
 Home-page: https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer
 Author: TileDB
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg.egg-info/SOURCES.txt` & `tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 tiledb_jupyter_bioimg.egg-info/top_level.txt
 tiledb_jupyter_bioimg/labextension/package.json
 tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg
 tiledb_jupyter_bioimg/labextension/static/172.6267f3dd3063477e34ed.js
 tiledb_jupyter_bioimg/labextension/static/344.8db93920a8ca0f0600d9.js
 tiledb_jupyter_bioimg/labextension/static/344.8db93920a8ca0f0600d9.js.LICENSE.txt
 tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
-tiledb_jupyter_bioimg/labextension/static/633.770b26571c8b948a69e3.js
-tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js
-tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js.LICENSE.txt
+tiledb_jupyter_bioimg/labextension/static/633.86ebe895050415abdfba.js
+tiledb_jupyter_bioimg/labextension/static/635.ce138c9764842046bf90.js
+tiledb_jupyter_bioimg/labextension/static/635.ce138c9764842046bf90.js.LICENSE.txt
 tiledb_jupyter_bioimg/labextension/static/713.44bebcfa12a45c30ff83.js
 tiledb_jupyter_bioimg/labextension/static/713.44bebcfa12a45c30ff83.js.LICENSE.txt
-tiledb_jupyter_bioimg/labextension/static/744.33b070180c108b7cf8c9.js
+tiledb_jupyter_bioimg/labextension/static/744.9655cb2c54e12e1c2654.js
 tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js
-tiledb_jupyter_bioimg/labextension/static/remoteEntry.b0daa29a1375bdb34258.js
+tiledb_jupyter_bioimg/labextension/static/remoteEntry.f05f71ea95cf3364c4cb.js
 tiledb_jupyter_bioimg/labextension/static/style.js
 tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a1/tsconfig.json` & `tiledb_jupyter_bioimg-0.1.1a2/tsconfig.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6547619047619048%*

 * *Differences: {"'compilerOptions'": "{'strictNullChecks': True, delete: ['lib']}",*

 * * "'exclude'": "['src/**/__tests__']"}*

```diff
@@ -2,30 +2,29 @@
     "compilerOptions": {
         "allowSyntheticDefaultImports": true,
         "composite": true,
         "declaration": true,
         "esModuleInterop": true,
         "incremental": true,
         "jsx": "react",
-        "lib": [
-            "ESNext",
-            "DOM"
-        ],
         "module": "esnext",
         "moduleResolution": "node",
         "noEmitOnError": true,
         "noImplicitAny": true,
         "noUnusedLocals": true,
         "outDir": "lib",
         "preserveWatchOutput": true,
         "resolveJsonModule": true,
         "rootDir": "src",
         "skipLibCheck": true,
         "strict": true,
-        "strictNullChecks": false,
+        "strictNullChecks": true,
         "target": "es2017",
         "types": []
     },
+    "exclude": [
+        "src/**/__tests__"
+    ],
     "include": [
         "src/*"
     ]
 }
```

