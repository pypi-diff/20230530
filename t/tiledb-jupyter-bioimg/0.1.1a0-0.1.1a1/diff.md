# Comparing `tmp/tiledb_jupyter_bioimg-0.1.1a0.tar.gz` & `tmp/tiledb_jupyter_bioimg-0.1.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiledb_jupyter_bioimg-0.1.1a0.tar", last modified: Tue May 30 08:29:51 2023, max compression
+gzip compressed data, was "tiledb_jupyter_bioimg-0.1.1a1.tar", last modified: Tue May 30 10:17:56 2023, max compression
```

## Comparing `tiledb_jupyter_bioimg-0.1.1a0.tar` & `tiledb_jupyter_bioimg-0.1.1a1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:29:51.501662 tiledb_jupyter_bioimg-0.1.1a0/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-30 08:25:42.000000 tiledb_jupyter_bioimg-0.1.1a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-30 08:25:42.000000 tiledb_jupyter_bioimg-0.1.1a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-30 08:29:51.501662 tiledb_jupyter_bioimg-0.1.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-30 08:25:42.000000 tiledb_jupyter_bioimg-0.1.1a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-30 08:25:42.000000 tiledb_jupyter_bioimg-0.1.1a0/install.json
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-30 08:27:46.000000 tiledb_jupyter_bioimg-0.1.1a0/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-30 08:25:42.000000 tiledb_jupyter_bioimg-0.1.1a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 08:29:51.501662 tiledb_jupyter_bioimg-0.1.1a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-30 08:25:42.000000 tiledb_jupyter_bioimg-0.1.1a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:29:51.497662 tiledb_jupyter_bioimg-0.1.1a0/src/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-30 08:25:42.000000 tiledb_jupyter_bioimg-0.1.1a0/src/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-30 08:25:42.000000 tiledb_jupyter_bioimg-0.1.1a0/src/version.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-30 08:25:42.000000 tiledb_jupyter_bioimg-0.1.1a0/src/widget.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:29:51.497662 tiledb_jupyter_bioimg-0.1.1a0/style/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 08:25:42.000000 tiledb_jupyter_bioimg-0.1.1a0/style/base.css
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 08:25:42.000000 tiledb_jupyter_bioimg-0.1.1a0/style/index.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-30 08:25:42.000000 tiledb_jupyter_bioimg-0.1.1a0/style/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:29:51.497662 tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-30 08:25:42.000000 tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-30 08:25:42.000000 tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-30 08:25:42.000000 tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:29:51.497662 tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-30 08:29:50.000000 tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:29:51.501662 tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)   189298 2023-05-30 08:29:50.000000 tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14610 2023-05-30 08:29:50.000000 tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/labextension/static/172.6267f3dd3063477e34ed.js
--rw-r--r--   0 runner    (1001) docker     (123)   725916 2023-05-30 08:29:50.000000 tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/labextension/static/344.8db93920a8ca0f0600d9.js
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-30 08:29:50.000000 tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/labextension/static/344.8db93920a8ca0f0600d9.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-30 08:29:50.000000 tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-30 08:29:50.000000 tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/labextension/static/633.770b26571c8b948a69e3.js
--rw-r--r--   0 runner    (1001) docker     (123)   516691 2023-05-30 08:29:50.000000 tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-30 08:29:50.000000 tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   172872 2023-05-30 08:29:50.000000 tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/labextension/static/713.75fe0d9ef4c6ff1de4d7.js
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-30 08:29:50.000000 tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/labextension/static/713.75fe0d9ef4c6ff1de4d7.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-30 08:29:50.000000 tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/labextension/static/744.fcbd28431423403c9c8b.js
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-30 08:29:50.000000 tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js
--rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-05-30 08:29:50.000000 tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/labextension/static/remoteEntry.c73b66672555e7ef21cd.js
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-30 08:29:25.000000 tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)    90733 2023-05-30 08:29:50.000000 tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-30 08:25:42.000000 tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:29:51.497662 tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-30 08:29:51.000000 tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-30 08:29:51.000000 tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 08:29:51.000000 tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 08:28:44.000000 tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-30 08:29:51.000000 tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 08:29:51.000000 tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-30 08:25:42.000000 tiledb_jupyter_bioimg-0.1.1a0/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:17:56.632812 tiledb_jupyter_bioimg-0.1.1a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-30 10:13:58.000000 tiledb_jupyter_bioimg-0.1.1a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-30 10:13:58.000000 tiledb_jupyter_bioimg-0.1.1a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-30 10:17:56.632812 tiledb_jupyter_bioimg-0.1.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-30 10:13:58.000000 tiledb_jupyter_bioimg-0.1.1a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-30 10:13:58.000000 tiledb_jupyter_bioimg-0.1.1a1/install.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-30 10:15:52.000000 tiledb_jupyter_bioimg-0.1.1a1/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-30 10:13:58.000000 tiledb_jupyter_bioimg-0.1.1a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 10:17:56.632812 tiledb_jupyter_bioimg-0.1.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-30 10:13:58.000000 tiledb_jupyter_bioimg-0.1.1a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:17:56.624812 tiledb_jupyter_bioimg-0.1.1a1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-30 10:13:58.000000 tiledb_jupyter_bioimg-0.1.1a1/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-30 10:13:58.000000 tiledb_jupyter_bioimg-0.1.1a1/src/version.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-30 10:13:58.000000 tiledb_jupyter_bioimg-0.1.1a1/src/widget.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:17:56.624812 tiledb_jupyter_bioimg-0.1.1a1/style/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 10:13:58.000000 tiledb_jupyter_bioimg-0.1.1a1/style/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 10:13:58.000000 tiledb_jupyter_bioimg-0.1.1a1/style/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-30 10:13:58.000000 tiledb_jupyter_bioimg-0.1.1a1/style/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:17:56.624812 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-30 10:13:58.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-30 10:13:58.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-30 10:13:58.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:17:56.628812 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-30 10:17:55.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:17:56.632812 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   189298 2023-05-30 10:17:55.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14610 2023-05-30 10:17:55.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/172.6267f3dd3063477e34ed.js
+-rw-r--r--   0 runner    (1001) docker     (123)   725916 2023-05-30 10:17:55.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/344.8db93920a8ca0f0600d9.js
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-30 10:17:55.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/344.8db93920a8ca0f0600d9.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-30 10:17:55.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-30 10:17:55.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/633.770b26571c8b948a69e3.js
+-rw-r--r--   0 runner    (1001) docker     (123)   516691 2023-05-30 10:17:55.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-30 10:17:55.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   172313 2023-05-30 10:17:55.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/713.44bebcfa12a45c30ff83.js
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-30 10:17:55.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/713.44bebcfa12a45c30ff83.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-05-30 10:17:55.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/744.33b070180c108b7cf8c9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-30 10:17:55.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-05-30 10:17:55.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/remoteEntry.b0daa29a1375bdb34258.js
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-30 10:17:31.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)    90733 2023-05-30 10:17:55.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-30 10:13:58.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:17:56.628812 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-30 10:17:56.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-30 10:17:56.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:17:56.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:16:49.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-30 10:17:56.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 10:17:56.000000 tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-30 10:13:58.000000 tiledb_jupyter_bioimg-0.1.1a1/tsconfig.json
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a0/LICENSE` & `tiledb_jupyter_bioimg-0.1.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a0/PKG-INFO` & `tiledb_jupyter_bioimg-0.1.1a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledb_jupyter_bioimg
-Version: 0.1.1a0
+Version: 0.1.1a1
 Summary: A jupyterlab extension to visualize bioimages in TileDB format
 Home-page: https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer
 Author: TileDB
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a0/README.md` & `tiledb_jupyter_bioimg-0.1.1a1/README.md`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a0/package.json` & `tiledb_jupyter_bioimg-0.1.1a1/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9561403508771928%*

 * *Differences: {"'dependencies'": "{'@jupyter-widgets/base': '^1.1.10 || ^2 || ^3 || ^4'}",*

 * * "'files'": "{insert: [(2, 'style/*.css'), (3, 'style/index.js')]}",*

 * * "'version'": "'0.1.1-alpha.1'"}*

```diff
@@ -1,14 +1,14 @@
 {
     "author": "TileDB",
     "bugs": {
         "url": "https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer/issues"
     },
     "dependencies": {
-        "@jupyter-widgets/base": "^1.1.10 || ^2 || ^3 || ^4 || ^5",
+        "@jupyter-widgets/base": "^1.1.10 || ^2 || ^3 || ^4",
         "@jupyterlab/application": "^3.4.5",
         "@tiledb-inc/bioimage-viewer": "^0.1.0-alpha.7"
     },
     "description": "A jupyterlab extension to visualize bioimages in TileDB format",
     "devDependencies": {
         "@jupyterlab/builder": "^3.1.0",
         "@typescript-eslint/eslint-plugin": "^2.27.0",
@@ -19,15 +19,17 @@
         "npm-run-all": "^4.1.5",
         "prettier": "^1.19.0",
         "rimraf": "^3.0.2",
         "typescript": "~4.1.3"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
-        "style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
+        "style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
+        "style/*.css",
+        "style/index.js"
     ],
     "homepage": "https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer",
     "jupyterlab": {
         "extension": "lib/index",
         "outputDir": "tiledb_jupyter_bioimg/labextension",
         "webpackConfig": "./webpack.config.js"
     },
@@ -65,9 +67,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.1-alpha.0"
+    "version": "0.1.1-alpha.1"
 }
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a0/setup.py` & `tiledb_jupyter_bioimg-0.1.1a1/setup.py`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a0/src/index.ts` & `tiledb_jupyter_bioimg-0.1.1a1/src/index.ts`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a0/src/version.ts` & `tiledb_jupyter_bioimg-0.1.1a1/src/version.ts`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a0/src/widget.ts` & `tiledb_jupyter_bioimg-0.1.1a1/src/widget.ts`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/_version.py` & `tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/_version.py`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/labextension/package.json` & `tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9555921052631577%*

 * *Differences: {"'dependencies'": "{'@jupyter-widgets/base': '^1.1.10 || ^2 || ^3 || ^4'}",*

 * * "'files'": "{insert: [(2, 'style/*.css'), (3, 'style/index.js')]}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.b0daa29a1375bdb34258.js'}}",*

 * * "'version'": "'0.1.1-alpha.1'"}*

```diff
@@ -1,14 +1,14 @@
 {
     "author": "TileDB",
     "bugs": {
         "url": "https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer/issues"
     },
     "dependencies": {
-        "@jupyter-widgets/base": "^1.1.10 || ^2 || ^3 || ^4 || ^5",
+        "@jupyter-widgets/base": "^1.1.10 || ^2 || ^3 || ^4",
         "@jupyterlab/application": "^3.4.5",
         "@tiledb-inc/bioimage-viewer": "^0.1.0-alpha.7"
     },
     "description": "A jupyterlab extension to visualize bioimages in TileDB format",
     "devDependencies": {
         "@jupyterlab/builder": "^3.1.0",
         "@typescript-eslint/eslint-plugin": "^2.27.0",
@@ -19,21 +19,23 @@
         "npm-run-all": "^4.1.5",
         "prettier": "^1.19.0",
         "rimraf": "^3.0.2",
         "typescript": "~4.1.3"
     },
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
-        "style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
+        "style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
+        "style/*.css",
+        "style/index.js"
     ],
     "homepage": "https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.c73b66672555e7ef21cd.js",
+            "load": "static/remoteEntry.b0daa29a1375bdb34258.js",
             "style": "./style"
         },
         "extension": "lib/index",
         "outputDir": "tiledb_jupyter_bioimg/labextension",
         "webpackConfig": "./webpack.config.js"
     },
     "keywords": [
@@ -70,9 +72,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.1-alpha.0"
+    "version": "0.1.1-alpha.1"
 }
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg` & `tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/labextension/static/172.6267f3dd3063477e34ed.js` & `tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/172.6267f3dd3063477e34ed.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/labextension/static/344.8db93920a8ca0f0600d9.js` & `tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/344.8db93920a8ca0f0600d9.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/labextension/static/633.770b26571c8b948a69e3.js` & `tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/633.770b26571c8b948a69e3.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js` & `tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js.LICENSE.txt` & `tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/labextension/static/713.75fe0d9ef4c6ff1de4d7.js` & `tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/713.44bebcfa12a45c30ff83.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,47 +1,46 @@
-/*! For license information please see 713.75fe0d9ef4c6ff1de4d7.js.LICENSE.txt */
+/*! For license information please see 713.44bebcfa12a45c30ff83.js.LICENSE.txt */
 (self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer = self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer || []).push([
     [713], {
         2713: (e, t, n) => {
             "use strict";
             n.r(t), n.d(t, {
                 CONTROL_COMM_PROTOCOL_VERSION: () => N,
                 CONTROL_COMM_TARGET: () => P,
                 CONTROL_COMM_TIMEOUT: () => M,
-                DOMWidgetModel: () => re,
-                DOMWidgetView: () => ae,
-                IJupyterWidgetRegistry: () => ve,
+                DOMWidgetModel: () => Z,
+                DOMWidgetView: () => re,
+                IJupyterWidgetRegistry: () => he,
                 JUPYTER_WIDGETS_VERSION: () => k,
-                JupyterPhosphorPanelWidget: () => se,
-                JupyterPhosphorWidget: () => oe,
-                LayoutModel: () => ce,
-                LayoutView: () => fe,
+                JupyterPhosphorPanelWidget: () => ne,
+                JupyterPhosphorWidget: () => te,
+                LayoutModel: () => se,
+                LayoutView: () => ae,
                 ManagerBase: () => L,
                 PROTOCOL_VERSION: () => j,
-                StyleModel: () => de,
-                StyleView: () => pe,
-                ViewList: () => me,
-                WidgetModel: () => ne,
-                WidgetView: () => ie,
+                StyleModel: () => le,
+                StyleView: () => ce,
+                ViewList: () => fe,
+                WidgetModel: () => Q,
+                WidgetView: () => ee,
                 WrappedError: () => v,
                 assign: () => p,
                 base64ToBuffer: () => C,
                 bufferToBase64: () => T,
                 bufferToHex: () => x,
                 difference: () => h,
                 hexToBuffer: () => E,
                 isEqual: () => d,
-                pack_models: () => ee,
                 put_buffers: () => _,
                 reject: () => y,
                 remove_buffers: () => b,
                 resolvePromisesDict: () => g,
                 serialize_state: () => I,
-                shims: () => te,
-                unpack_models: () => Z,
+                shims: () => Y,
+                unpack_models: () => K,
                 uuid: () => m
             });
             var r, i = n(9742),
                 o = n(1526),
                 s = n(8446),
                 a = n.n(s),
                 u = n(8630),
@@ -156,22 +155,22 @@
             }
 
             function C(e) {
                 return (0, i.b$)(e).buffer
             }
             var k = "1.2.0",
                 j = "2.1.0",
-                A = function() {
-                    return A = Object.assign || function(e) {
+                S = function() {
+                    return S = Object.assign || function(e) {
                         for (var t, n = 1, r = arguments.length; n < r; n++)
                             for (var i in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, i) && (e[i] = t[i]);
                         return e
-                    }, A.apply(this, arguments)
+                    }, S.apply(this, arguments)
                 },
-                S = function(e, t, n, r) {
+                A = function(e, t, n, r) {
                     return new(n || (n = Promise))((function(i, o) {
                         function s(e) {
                             try {
                                 u(r.next(e))
                             } catch (e) {
                                 o(e)
                             }
@@ -338,15 +337,15 @@
                                 _view_module: e.view_module,
                                 _view_module_version: e.view_module_version,
                                 _view_name: e.view_name
                             }
                         }, {
                             version: j
                         });
-                        var i = A({}, e);
+                        var i = S({}, e);
                         return n.then((function(e) {
                             return i.comm = e, r.new_model(i, t).then((function(e) {
                                 return e.sync("create", e), e
                             }))
                         }), (function() {
                             return i.model_id || (i.model_id = m()), r.new_model(i, t)
                         }))
@@ -354,15 +353,15 @@
                         var n = this;
                         this._models[e] = t, t.then((function(t) {
                             t.once("comm:close", (function() {
                                 delete n._models[e]
                             }))
                         }))
                     }, e.prototype.new_model = function(e, t) {
-                        return void 0 === t && (t = {}), S(this, void 0, void 0, (function() {
+                        return void 0 === t && (t = {}), A(this, void 0, void 0, (function() {
                             var n, r;
                             return O(this, (function(i) {
                                 switch (i.label) {
                                     case 0:
                                         if (e.model_id) n = e.model_id;
                                         else {
                                             if (!e.comm) throw new Error("Neither comm nor model_id provided in options object. At least one must exist.");
@@ -371,15 +370,15 @@
                                         return r = this._make_model(e, t), this.register_model(n, r), [4, r];
                                     case 1:
                                         return [2, i.sent()]
                                 }
                             }))
                         }))
                     }, e.prototype._make_model = function(e, t) {
-                        return void 0 === t && (t = {}), S(this, void 0, void 0, (function() {
+                        return void 0 === t && (t = {}), A(this, void 0, void 0, (function() {
                             var n, r, i, o, s, a, u;
                             return O(this, (function(l) {
                                 switch (l.label) {
                                     case 0:
                                         n = e.model_id, r = this.loadClass(e.model_name, e.model_module, e.model_module_version), l.label = 1;
                                     case 1:
                                         return l.trys.push([1, 3, , 4]), [4, r];
@@ -396,15 +395,15 @@
                                             model_id: n,
                                             comm: e.comm
                                         }, (u = new i(s, a)).name = e.model_name, u.module = e.model_module, [2, u]
                                 }
                             }))
                         }))
                     }, e.prototype._loadFromKernel = function() {
-                        return S(this, void 0, void 0, (function() {
+                        return A(this, void 0, void 0, (function() {
                             var e, t, n, r, i, o, s, a, u, l, c, f, h, d = this;
                             return O(this, (function(p) {
                                 switch (p.label) {
                                     case 0:
                                         return p.trys.push([0, 3, , 4]), [4, this._create_comm(P, m(), {}, {
                                             version: N
                                         })];
@@ -425,15 +424,15 @@
                                     case 2:
                                         return p.sent(), n.close(), [3, 4];
                                     case 3:
                                         return r = p.sent(), console.warn('Failed to fetch ipywidgets through the "jupyter.widget.control" comm channel, fallback to fetching individual model state. Reason:', r), [2, this._loadFromKernelModels()];
                                     case 4:
                                         for (i = e.states, o = {}, s = {}, a = 0; a < e.buffer_paths.length; a++) u = e.buffer_paths[a], l = u[0], c = u.slice(1), f = t[a], o[l] || (o[l] = [], s[l] = []), o[l].push(c), s[l].push(f);
                                         return [4, Promise.all(Object.keys(i).map((function(e) {
-                                            return S(d, void 0, void 0, (function() {
+                                            return A(d, void 0, void 0, (function() {
                                                 var t;
                                                 return O(this, (function(n) {
                                                     switch (n.label) {
                                                         case 0:
                                                             return this.has_model(e) ? (t = void 0, [3, 3]) : [3, 1];
                                                         case 1:
                                                             return [4, this._create_comm("jupyter.widget", e)];
@@ -448,61 +447,59 @@
                                                 }))
                                             }))
                                         })))];
                                     case 5:
                                         return h = p.sent(), [4, Promise.all(h.map((function(e) {
                                             var t = e.widget_id,
                                                 n = e.comm;
-                                            return S(d, void 0, void 0, (function() {
-                                                var e, r, a, u;
-                                                return O(this, (function(l) {
-                                                    switch (l.label) {
+                                            return A(d, void 0, void 0, (function() {
+                                                var e, r;
+                                                return O(this, (function(a) {
+                                                    switch (a.label) {
                                                         case 0:
-                                                            e = i[t], t in o && _(e, o[t], s[t]), l.label = 1;
+                                                            e = i[t], t in o && _(e, o[t], s[t]), a.label = 1;
                                                         case 1:
-                                                            return l.trys.push([1, 7, , 8]), n ? [4, this.new_model({
+                                                            return a.trys.push([1, 6, , 7]), n ? [4, this.new_model({
                                                                 model_name: e.model_name,
                                                                 model_module: e.model_module,
                                                                 model_module_version: e.model_module_version,
                                                                 model_id: t,
                                                                 comm: n
                                                             }, e.state)] : [3, 3];
                                                         case 2:
-                                                            return l.sent(), [3, 6];
+                                                            return a.sent(), [3, 5];
                                                         case 3:
                                                             return [4, this.get_model(t)];
                                                         case 4:
-                                                            return [4, (r = l.sent()).constructor._deserialize_state(e.state, this)];
+                                                            a.sent().set_state(e.state), a.label = 5;
                                                         case 5:
-                                                            a = l.sent(), r.set_state(a), l.label = 6;
+                                                            return [3, 7];
                                                         case 6:
-                                                            return [3, 8];
+                                                            return r = a.sent(), console.error(r), [3, 7];
                                                         case 7:
-                                                            return u = l.sent(), console.error(u), [3, 8];
-                                                        case 8:
                                                             return [2]
                                                     }
                                                 }))
                                             }))
                                         })))];
                                     case 6:
                                         return p.sent(), [2]
                                 }
                             }))
                         }))
                     }, e.prototype._loadFromKernelModels = function() {
-                        return S(this, void 0, void 0, (function() {
+                        return A(this, void 0, void 0, (function() {
                             var e, t, n = this;
                             return O(this, (function(r) {
                                 switch (r.label) {
                                     case 0:
                                         return [4, this._get_comm_info()];
                                     case 1:
                                         return e = r.sent(), [4, Promise.all(Object.keys(e).map((function(e) {
-                                            return S(n, void 0, void 0, (function() {
+                                            return A(n, void 0, void 0, (function() {
                                                 var t, n, r;
                                                 return O(this, (function(i) {
                                                     switch (i.label) {
                                                         case 0:
                                                             return this.has_model(e) ? [2] : [4, this._create_comm(this.comm_target_name, e)];
                                                         case 1:
                                                             return t = i.sent(), n = "", r = new o.PromiseDelegate, t.on_msg((function(e) {
@@ -520,15 +517,15 @@
                                                             }, this.callbacks(void 0)), [2, r.promise]
                                                     }
                                                 }))
                                             }))
                                         })))];
                                     case 2:
                                         return t = r.sent(), [4, Promise.all(t.map((function(e) {
-                                            return S(n, void 0, void 0, (function() {
+                                            return A(n, void 0, void 0, (function() {
                                                 var t;
                                                 return O(this, (function(n) {
                                                     switch (n.label) {
                                                         case 0:
                                                             return e ? (t = e.msg.content, [4, this.new_model({
                                                                 model_name: t.data.state._model_name,
                                                                 model_module: t.data.state._model_module,
@@ -611,15 +608,15 @@
                     }, e.prototype.filterExistingModelState = function(e) {
                         var t = this,
                             n = e.state;
                         return n = Object.keys(n).filter((function(e) {
                             return !t.has_model(e)
                         })).reduce((function(e, t) {
                             return e[t] = n[t], e
-                        }), {}), A(A({}, e), {
+                        }), {}), S(S({}, e), {
                             state: n
                         })
                     }, e
                 }();
 
             function I(e, t) {
                 void 0 === t && (t = {});
@@ -770,53 +767,32 @@
                 }(),
                 G = function() {
                     return G = Object.assign || function(e) {
                         for (var t, n = 1, r = arguments.length; n < r; n++)
                             for (var i in t = arguments[n]) Object.prototype.hasOwnProperty.call(t, i) && (e[i] = t[i]);
                         return e
                     }, G.apply(this, arguments)
-                },
-                K = "IPY_MODEL_",
-                Y = function(e) {
-                    return JSON.parse(JSON.stringify(e))
-                },
-                Q = globalThis.structuredClone || Y;
+                };
 
-            function Z(e, t) {
+            function K(e, t) {
                 if (Array.isArray(e)) {
                     var n = [];
                     return e.forEach((function(e, r) {
-                        n.push(Z(e, t))
+                        n.push(K(e, t))
                     })), Promise.all(n)
                 }
                 if (e instanceof Object) {
                     var r = {};
                     return Object.keys(e).forEach((function(n) {
-                        r[n] = Z(e[n], t)
+                        r[n] = K(e[n], t)
                     })), g(r)
                 }
                 return "string" == typeof e && "IPY_MODEL_" === e.slice(0, 10) ? t.get_model(e.slice(10, e.length)) : Promise.resolve(e)
             }
-
-            function ee(e, t) {
-                if (Array.isArray(e)) {
-                    for (var n = [], r = 0, i = e; r < i.length; r++) {
-                        var o = i[r];
-                        n.push(ee(o, t))
-                    }
-                    return n
-                }
-                if (e instanceof ne) return "" + K + e.model_id;
-                if (!(e instanceof Object && "string" != typeof e)) return e;
-                var s = {};
-                Object.keys(e).forEach((function(n) {
-                    s[n] = ee(e[n], t)
-                }))
-            }
-            var te, ne = function(e) {
+            var Y, Q = function(e) {
                     function t() {
                         return null !== e && e.apply(this, arguments) || this
                     }
                     return X(t, e), t.prototype.defaults = function() {
                         return {
                             _model_module: "@jupyter-widgets/base",
                             _model_name: "WidgetModel",
@@ -964,22 +940,20 @@
                         }
                     }, t.prototype.rememberLastUpdateFor = function(e) {
                         var t = this;
                         Object.keys(this._attrsToUpdate).forEach((function(n) {
                             t._expectedEchoMsgIds[n] = e
                         })), this._attrsToUpdate = {}
                     }, t.prototype.serialize = function(e) {
-                        for (var t, n, r = this.constructor.serializers || {}, i = 0, o = Object.keys(e); i < o.length; i++) {
-                            var s = o[i];
+                        for (var t = this.constructor.serializers || {}, n = 0, r = Object.keys(e); n < r.length; n++) {
+                            var i = r[n];
                             try {
-                                var a = r[s] || null,
-                                    u = (null === (t = a) || void 0 === t ? void 0 : t.serialize) || null;
-                                null == u && (null === (n = a) || void 0 === n ? void 0 : n.deserialize) === Z && (u = Y), e[s] = u ? u(e[s], this) : Q(e[s]), e[s] && e[s].toJSON && (e[s] = e[s].toJSON())
+                                t[i] && t[i].serialize ? e[i] = t[i].serialize(e[i], this) : e[i] = JSON.parse(JSON.stringify(e[i])), e[i] && e[i].toJSON && (e[i] = e[i].toJSON())
                             } catch (e) {
-                                throw console.error("Error serializing widget state attribute: ", s), e
+                                throw console.error("Error serializing widget state attribute: ", i), e
                             }
                         }
                         return e
                     }, t.prototype.send_sync_message = function(e, t) {
                         var n = this;
                         if (void 0 === t && (t = {}), !this.comm) return "";
                         try {
@@ -1020,32 +994,32 @@
                         var n, r = this.serializers;
                         if (r)
                             for (var i in n = {}, e) r[i] && r[i].deserialize ? n[i] = r[i].deserialize(e[i], t) : n[i] = e[i];
                         else n = e;
                         return g(n)
                     }, t
                 }(R.Model),
-                re = function(e) {
+                Z = function(e) {
                     function t() {
                         return null !== e && e.apply(this, arguments) || this
                     }
                     return X(t, e), t.prototype.defaults = function() {
                         return p(e.prototype.defaults.call(this), {
                             _dom_classes: []
                         })
-                    }, t.serializers = G(G({}, ne.serializers), {
+                    }, t.serializers = G(G({}, Q.serializers), {
                         layout: {
-                            deserialize: Z
+                            deserialize: K
                         },
                         style: {
-                            deserialize: Z
+                            deserialize: K
                         }
                     }), t
-                }(ne),
-                ie = function(e) {
+                }(Q),
+                ee = function(e) {
                     function t(t) {
                         return e.call(this, t) || this
                     }
                     return X(t, e), t.prototype.initialize = function(e) {
                         var t = this;
                         this.listenTo(this.model, "change", (function() {
                             var e = Object.keys(t.model.changedAttributes() || {});
@@ -1067,39 +1041,39 @@
                         this.model.send(e, this.callbacks(), t)
                     }, t.prototype.touch = function() {
                         this.model.save_changes(this.callbacks())
                     }, t.prototype.remove = function() {
                         return e.prototype.remove.call(this), this.trigger("remove"), this
                     }, t
                 }(U),
-                oe = function(e) {
+                te = function(e) {
                     function t(t) {
                         var n = this,
                             r = t.view;
                         return delete t.view, (n = e.call(this, t) || this)._view = r, n
                     }
                     return X(t, e), t.prototype.dispose = function() {
                         this.isDisposed || (e.prototype.dispose.call(this), this._view && this._view.remove(), this._view = null)
                     }, t.prototype.processMessage = function(t) {
                         e.prototype.processMessage.call(this, t), this._view.processPhosphorMessage(t)
                     }, t
                 }(V.Widget),
-                se = function(e) {
+                ne = function(e) {
                     function t(t) {
                         var n = this,
                             r = t.view;
                         return delete t.view, (n = e.call(this, t) || this)._view = r, n
                     }
                     return X(t, e), t.prototype.processMessage = function(t) {
                         e.prototype.processMessage.call(this, t), this._view.processPhosphorMessage(t)
                     }, t.prototype.dispose = function() {
                         this.isDisposed || (e.prototype.dispose.call(this), this._view && this._view.remove(), this._view = null)
                     }, t
                 }(V.Panel),
-                ae = function(e) {
+                re = function(e) {
                     function t() {
                         return null !== e && e.apply(this, arguments) || this
                     }
                     return X(t, e), t.prototype.initialize = function(t) {
                         var n = this;
                         e.prototype.initialize.call(this, t), this.listenTo(this.model, "change:_dom_classes", (function(e, t) {
                             var r = e.previous("_dom_classes");
@@ -1145,27 +1119,27 @@
                             o = e[r = this.model.get(t)] ? e[r] : [];
                         this.update_classes(i, o, n || this.el)
                     }, t.prototype.set_mapped_classes = function(e, t, n) {
                         var r = this.model.get(t),
                             i = e[r] ? e[r] : [];
                         this.update_classes([], i, n || this.el)
                     }, t.prototype._setElement = function(e) {
-                        this.pWidget && this.pWidget.dispose(), this.$el = e instanceof F() ? e : F()(e), this.el = this.$el[0], this.pWidget = new oe({
+                        this.pWidget && this.pWidget.dispose(), this.$el = e instanceof F() ? e : F()(e), this.el = this.$el[0], this.pWidget = new te({
                             node: e,
                             view: this
                         })
                     }, t.prototype.remove = function() {
                         return this.pWidget && this.pWidget.dispose(), e.prototype.remove.call(this)
                     }, t.prototype.processPhosphorMessage = function(e) {
                         "after-attach" === e.type && this.trigger("displayed")
                     }, t.prototype._comm_live_update = function() {
                         this.model.comm_live ? this.pWidget.removeClass("jupyter-widgets-disconnected") : this.pWidget.addClass("jupyter-widgets-disconnected")
                     }, t
-                }(ie),
-                ue = function() {
+                }(ee),
+                ie = function() {
                     var e = function(t, n) {
                         return e = Object.setPrototypeOf || {
                             __proto__: []
                         }
                         instanceof Array && function(e, t) {
                             e.__proto__ = t
                         } || function(e, t) {
@@ -1175,15 +1149,15 @@
                     return function(t, n) {
                         function r() {
                             this.constructor = t
                         }
                         e(t, n), t.prototype = null === n ? Object.create(n) : (r.prototype = n.prototype, new r)
                     }
                 }(),
-                le = {
+                oe = {
                     align_content: null,
                     align_items: null,
                     align_self: null,
                     border: null,
                     bottom: null,
                     display: null,
                     flex: null,
@@ -1215,32 +1189,32 @@
                     grid_template_rows: null,
                     grid_template_columns: null,
                     grid_template_areas: null,
                     grid_row: null,
                     grid_column: null,
                     grid_area: null
                 },
-                ce = function(e) {
+                se = function(e) {
                     function t() {
                         return null !== e && e.apply(this, arguments) || this
                     }
-                    return ue(t, e), t.prototype.defaults = function() {
+                    return ie(t, e), t.prototype.defaults = function() {
                         return p(e.prototype.defaults.call(this), {
                             _model_name: "LayoutModel",
                             _view_name: "LayoutView"
-                        }, le)
+                        }, oe)
                     }, t
-                }(ne),
-                fe = function(e) {
+                }(Q),
+                ae = function(e) {
                     function t() {
                         return null !== e && e.apply(this, arguments) || this
                     }
-                    return ue(t, e), t.prototype.initialize = function(t) {
+                    return ie(t, e), t.prototype.initialize = function(t) {
                         this._traitNames = [], e.prototype.initialize.call(this, t);
-                        for (var n = 0, r = Object.keys(le); n < r.length; n++) {
+                        for (var n = 0, r = Object.keys(oe); n < r.length; n++) {
                             var i = r[n];
                             this.registerTrait(i)
                         }
                     }, t.prototype.registerTrait = function(e) {
                         var t = this;
                         if (this._traitNames.push(e), "overflow_x" === e || "overflow_y" === e) return this.listenTo(this.model, "change:" + e, (function(n, r) {
                             t.handleOverflowChange(e, r)
@@ -1259,16 +1233,16 @@
                     }, t.prototype.unlayout = function() {
                         var e = this,
                             t = this.options.parent;
                         this._traitNames.forEach((function(n) {
                             t ? t.el.style.removeProperty(e.css_name(n)) : console.warn("Style not removed because a parent view does not exist")
                         }), this)
                     }, t
-                }(ie),
-                he = function() {
+                }(ee),
+                ue = function() {
                     var e = function(t, n) {
                         return e = Object.setPrototypeOf || {
                             __proto__: []
                         }
                         instanceof Array && function(e, t) {
                             e.__proto__ = t
                         } || function(e, t) {
@@ -1278,33 +1252,33 @@
                     return function(t, n) {
                         function r() {
                             this.constructor = t
                         }
                         e(t, n), t.prototype = null === n ? Object.create(n) : (r.prototype = n.prototype, new r)
                     }
                 }(),
-                de = function(e) {
+                le = function(e) {
                     function t() {
                         return null !== e && e.apply(this, arguments) || this
                     }
-                    return he(t, e), t.prototype.defaults = function() {
+                    return ue(t, e), t.prototype.defaults = function() {
                         var t = this.constructor;
                         return p(e.prototype.defaults.call(this), {
                             _model_name: "StyleModel",
                             _view_name: "StyleView"
                         }, Object.keys(t.styleProperties).reduce((function(e, n) {
                             return e[n] = t.styleProperties[n].default, e
                         }), {}))
                     }, t.styleProperties = {}, t
-                }(ne),
-                pe = function(e) {
+                }(Q),
+                ce = function(e) {
                     function t() {
                         return null !== e && e.apply(this, arguments) || this
                     }
-                    return he(t, e), t.prototype.initialize = function(t) {
+                    return ue(t, e), t.prototype.initialize = function(t) {
                         this._traitNames = [], e.prototype.initialize.call(this, t);
                         for (var n = this.model.constructor, r = 0, i = Object.keys(n.styleProperties); r < i.length; r++) {
                             var o = i[r];
                             this.registerTrait(o)
                         }
                         this.style()
                     }, t.prototype.registerTrait = function(e) {
@@ -1334,15 +1308,15 @@
                             t = this.model.constructor.styleProperties;
                         this._traitNames.forEach((function(n) {
                             if (e)
                                 for (var r = t[n].attribute, i = t[n].selector, o = i ? e.el.querySelectorAll(i) : [e.el], s = 0; s !== o.length; ++s) o[s].style.removeProperty(r);
                             else console.warn("Style not removed because a parent view does not exist")
                         }), this)
                     }, t
-                }(ie);
+                }(ee);
             ! function(e) {
                 ! function(e) {
                     var t = function() {
                         function e(e) {
                             this.targets = Object.create(null), this.comms = Object.create(null), this.kernel = null, this.jsServicesKernel = null, this.init_kernel(e)
                         }
                         return e.prototype.init_kernel = function(e) {
@@ -1518,16 +1492,16 @@
                                         t.iopub.output(e)
                                 }
                             })
                         }, e
                     }();
                     e.Comm = n
                 }(e.services || (e.services = {}))
-            }(te || (te = {}));
-            var me = function() {
+            }(Y || (Y = {}));
+            var fe = function() {
                     function e(e, t, n) {
                         this.initialize(e, t, n)
                     }
                     return e.prototype.initialize = function(e, t, n) {
                         this._handler_context = n || this, this._models = [], this.views = [], this._create_view = e, this._remove_view = t || function(e) {
                             e.remove()
                         }
@@ -1548,15 +1522,15 @@
                                 return e._remove_view.call(e._handler_context, t)
                             })), e.views = [], e._models = []
                         }))
                     }, e.prototype.dispose = function() {
                         this.views = null, this._models = null
                     }, e
                 }(),
-                ve = new o.Token("jupyter.extensions.jupyterWidgetRegistry")
+                he = new o.Token("jupyter.extensions.jupyterWidgetRegistry")
         },
         2316: (e, t, n) => {
             var r, i, o;
             o = "object" == typeof self && self.self == self && self || "object" == typeof n.g && n.g.global == n.g && n.g, r = [n(7794), n(9755), t], i = function(e, t, n) {
                 o.Backbone = function(e, t, n, r) {
                     var i = e.Backbone,
                         o = Array.prototype.slice;
@@ -2264,16 +2238,16 @@
                     };
                     t.ajax = function() {
                         return t.$.ajax.apply(t.$, arguments)
                     };
                     var j = t.Router = function(e) {
                             e || (e = {}), e.routes && (this.routes = e.routes), this._bindRoutes(), this.initialize.apply(this, arguments)
                         },
-                        A = /\((.*?)\)/g,
-                        S = /(\(\?)?:\w+/g,
+                        S = /\((.*?)\)/g,
+                        A = /(\(\?)?:\w+/g,
                         O = /\*\w+/g,
                         D = /[\-{}\[\]+?.,\\\^$|#\s]/g;
                     n.extend(j.prototype, l, {
                         initialize: function() {},
                         route: function(e, r, i) {
                             n.isRegExp(e) || (e = this._routeToRegExp(e)), n.isFunction(r) && (i = r, r = ""), i || (i = this[r]);
                             var o = this;
@@ -2291,15 +2265,15 @@
                         _bindRoutes: function() {
                             if (this.routes) {
                                 this.routes = n.result(this, "routes");
                                 for (var e, t = n.keys(this.routes); null != (e = t.pop());) this.route(e, this.routes[e])
                             }
                         },
                         _routeToRegExp: function(e) {
-                            return e = e.replace(D, "\\$&").replace(A, "(?:$1)?").replace(S, (function(e, t) {
+                            return e = e.replace(D, "\\$&").replace(S, "(?:$1)?").replace(A, (function(e, t) {
                                 return t ? e : "([^/?]+)"
                             })).replace(O, "([^?]*?)"), new RegExp("^" + e + "(?:\\?([\\s\\S]*))?$")
                         },
                         _extractParameters: function(e, t) {
                             var r = e.exec(t).slice(1);
                             return n.map(r, (function(e, t) {
                                 return t === r.length - 1 ? e || null : e ? decodeURIComponent(e) : null
@@ -2661,16 +2635,16 @@
                         return u(s)
                     },
                     guid: 1,
                     support: v
                 }), "function" == typeof Symbol && (C.fn[Symbol.iterator] = o[Symbol.iterator]), C.each("Boolean Number String Function Array Date RegExp Object Error Symbol".split(" "), (function(e, t) {
                     f["[object " + t + "]"] = t.toLowerCase()
                 }));
-                var A = o.pop,
-                    S = o.sort,
+                var S = o.pop,
+                    A = o.sort,
                     O = o.splice,
                     D = "[\\x20\\t\\r\\n\\f]",
                     P = new RegExp("^" + D + "+|((?:^|[^\\\\])(?:\\\\.)*)" + D + "+$", "g");
                 C.contains = function(e, t) {
                     var n = t && t.parentNode;
                     return e === n || !(!n || 1 !== n.nodeType || !(e.contains ? e.contains(n) : e.compareDocumentPosition && 16 & e.compareDocumentPosition(n)))
                 };
@@ -2902,15 +2876,15 @@
                             return void 0 !== i ? i : e.getAttribute(n)
                         }, Z.error = function(e) {
                             throw new Error("Syntax error, unrecognized expression: " + e)
                         }, C.uniqueSort = function(e) {
                             var t, n = [],
                                 r = 0,
                                 o = 0;
-                            if (s = !v.sortStable, i = !v.sortStable && a.call(e, 0), S.call(e, T), s) {
+                            if (s = !v.sortStable, i = !v.sortStable && a.call(e, 0), A.call(e, T), s) {
                                 for (; t = e[o++];) t === e[o] && (r = n.push(o));
                                 for (; r--;) O.call(e, n[r], 1)
                             }
                             return i = null, e
                         }, C.fn.uniqueSort = function() {
                             return this.pushStack(C.uniqueSort(a.apply(this)))
                         }, t = C.expr = {
@@ -3261,15 +3235,15 @@
                                             }
                                             i && ((d = !v && d) && g--, s && b.push(d))
                                         }
                                         if (g += _, i && _ !== g) {
                                             for (p = 0; v = r[p++];) v(b, w, a, l);
                                             if (s) {
                                                 if (g > 0)
-                                                    for (; _--;) b[_] || w[_] || (w[_] = A.call(c));
+                                                    for (; _--;) b[_] || w[_] || (w[_] = S.call(c));
                                                 w = pe(w)
                                             }
                                             m.apply(c, w), h && !s && w.length > 0 && g + r.length > 1 && C.uniqueSort(c)
                                         }
                                         return h && (y = T, n = x), b
                                     };
                                 return i ? te(s) : s
@@ -3875,44 +3849,44 @@
                         }))
                     }
                 });
                 var Ee, Te, Ce = /^(?:checkbox|radio)$/i,
                     ke = /<([a-z][^\/\0>\x20\t\r\n\f]*)/i,
                     je = /^$|^module$|\/(?:java|ecma)script/i;
                 Ee = _.createDocumentFragment().appendChild(_.createElement("div")), (Te = _.createElement("input")).setAttribute("type", "radio"), Te.setAttribute("checked", "checked"), Te.setAttribute("name", "t"), Ee.appendChild(Te), v.checkClone = Ee.cloneNode(!0).cloneNode(!0).lastChild.checked, Ee.innerHTML = "<textarea>x</textarea>", v.noCloneChecked = !!Ee.cloneNode(!0).lastChild.defaultValue, Ee.innerHTML = "<option></option>", v.option = !!Ee.lastChild;
-                var Ae = {
+                var Se = {
                     thead: [1, "<table>", "</table>"],
                     col: [2, "<table><colgroup>", "</colgroup></table>"],
                     tr: [2, "<table><tbody>", "</tbody></table>"],
                     td: [3, "<table><tbody><tr>", "</tr></tbody></table>"],
                     _default: [0, "", ""]
                 };
 
-                function Se(e, t) {
+                function Ae(e, t) {
                     var n;
                     return n = void 0 !== e.getElementsByTagName ? e.getElementsByTagName(t || "*") : void 0 !== e.querySelectorAll ? e.querySelectorAll(t || "*") : [], void 0 === t || t && j(e, t) ? C.merge([e], n) : n
                 }
 
                 function Oe(e, t) {
                     for (var n = 0, r = e.length; n < r; n++) ae.set(e[n], "globalEval", !t || ae.get(t[n], "globalEval"))
                 }
-                Ae.tbody = Ae.tfoot = Ae.colgroup = Ae.caption = Ae.thead, Ae.th = Ae.td, v.option || (Ae.optgroup = Ae.option = [1, "<select multiple='multiple'>", "</select>"]);
+                Se.tbody = Se.tfoot = Se.colgroup = Se.caption = Se.thead, Se.th = Se.td, v.option || (Se.optgroup = Se.option = [1, "<select multiple='multiple'>", "</select>"]);
                 var De = /<|&#?\w+;/;
 
                 function Pe(e, t, n, r, i) {
                     for (var o, s, a, u, l, c, f = t.createDocumentFragment(), h = [], d = 0, p = e.length; d < p; d++)
                         if ((o = e[d]) || 0 === o)
                             if ("object" === x(o)) C.merge(h, o.nodeType ? [o] : o);
                             else if (De.test(o)) {
-                        for (s = s || f.appendChild(t.createElement("div")), a = (ke.exec(o) || ["", ""])[1].toLowerCase(), u = Ae[a] || Ae._default, s.innerHTML = u[1] + C.htmlPrefilter(o) + u[2], c = u[0]; c--;) s = s.lastChild;
+                        for (s = s || f.appendChild(t.createElement("div")), a = (ke.exec(o) || ["", ""])[1].toLowerCase(), u = Se[a] || Se._default, s.innerHTML = u[1] + C.htmlPrefilter(o) + u[2], c = u[0]; c--;) s = s.lastChild;
                         C.merge(h, s.childNodes), (s = f.firstChild).textContent = ""
                     } else h.push(t.createTextNode(o));
                     for (f.textContent = "", d = 0; o = h[d++];)
                         if (r && C.inArray(o, r) > -1) i && i.push(o);
-                        else if (l = ve(o), s = Se(f.appendChild(o), "script"), l && Oe(s), n)
+                        else if (l = ve(o), s = Ae(f.appendChild(o), "script"), l && Oe(s), n)
                         for (c = 0; o = s[c++];) je.test(o.type || "") && n.push(o);
                     return f
                 }
                 var Ne = /^([^.]*)(?:\.(.+)|)/;
 
                 function Me() {
                     return !0
@@ -4227,41 +4201,41 @@
                         p = t[0],
                         m = g(p);
                     if (m || h > 1 && "string" == typeof p && !v.checkClone && Re.test(p)) return e.each((function(i) {
                         var o = e.eq(i);
                         m && (t[0] = p.call(this, i, o.html())), Ve(o, t, n, r)
                     }));
                     if (h && (o = (i = Pe(t, e[0].ownerDocument, !1, e, r)).firstChild, 1 === i.childNodes.length && (i = o), o || r)) {
-                        for (a = (s = C.map(Se(i, "script"), We)).length; f < h; f++) l = i, f !== d && (l = C.clone(l, !0, !0), a && C.merge(s, Se(l, "script"))), n.call(e[f], l, f);
+                        for (a = (s = C.map(Ae(i, "script"), We)).length; f < h; f++) l = i, f !== d && (l = C.clone(l, !0, !0), a && C.merge(s, Ae(l, "script"))), n.call(e[f], l, f);
                         if (a)
                             for (c = s[s.length - 1].ownerDocument, C.map(s, $e), f = 0; f < a; f++) l = s[f], je.test(l.type || "") && !ae.access(l, "globalEval") && C.contains(c, l) && (l.src && "module" !== (l.type || "").toLowerCase() ? C._evalUrl && !l.noModule && C._evalUrl(l.src, {
                                 nonce: l.nonce || l.getAttribute("nonce")
                             }, c) : w(l.textContent.replace(Be, ""), l, c))
                     }
                     return e
                 }
 
                 function Je(e, t, n) {
-                    for (var r, i = t ? C.filter(t, e) : e, o = 0; null != (r = i[o]); o++) n || 1 !== r.nodeType || C.cleanData(Se(r)), r.parentNode && (n && ve(r) && Oe(Se(r, "script")), r.parentNode.removeChild(r));
+                    for (var r, i = t ? C.filter(t, e) : e, o = 0; null != (r = i[o]); o++) n || 1 !== r.nodeType || C.cleanData(Ae(r)), r.parentNode && (n && ve(r) && Oe(Ae(r, "script")), r.parentNode.removeChild(r));
                     return e
                 }
                 C.extend({
                     htmlPrefilter: function(e) {
                         return e
                     },
                     clone: function(e, t, n) {
                         var r, i, o, s, a = e.cloneNode(!0),
                             u = ve(e);
                         if (!(v.noCloneChecked || 1 !== e.nodeType && 11 !== e.nodeType || C.isXMLDoc(e)))
-                            for (s = Se(a), r = 0, i = (o = Se(e)).length; r < i; r++) Ue(o[r], s[r]);
+                            for (s = Ae(a), r = 0, i = (o = Ae(e)).length; r < i; r++) Ue(o[r], s[r]);
                         if (t)
                             if (n)
-                                for (o = o || Se(e), s = s || Se(a), r = 0, i = o.length; r < i; r++) ze(o[r], s[r]);
+                                for (o = o || Ae(e), s = s || Ae(a), r = 0, i = o.length; r < i; r++) ze(o[r], s[r]);
                             else ze(e, a);
-                        return (s = Se(a, "script")).length > 0 && Oe(s, !u && Se(e, "script")), a
+                        return (s = Ae(a, "script")).length > 0 && Oe(s, !u && Ae(e, "script")), a
                     },
                     cleanData: function(e) {
                         for (var t, n, r, i = C.event.special, o = 0; void 0 !== (n = e[o]); o++)
                             if (oe(n)) {
                                 if (t = n[ae.expando]) {
                                     if (t.events)
                                         for (r in t.events) i[r] ? C.event.remove(n, r) : C.removeEvent(n, r, t.handle);
@@ -4304,43 +4278,43 @@
                     },
                     after: function() {
                         return Ve(this, arguments, (function(e) {
                             this.parentNode && this.parentNode.insertBefore(e, this.nextSibling)
                         }))
                     },
                     empty: function() {
-                        for (var e, t = 0; null != (e = this[t]); t++) 1 === e.nodeType && (C.cleanData(Se(e, !1)), e.textContent = "");
+                        for (var e, t = 0; null != (e = this[t]); t++) 1 === e.nodeType && (C.cleanData(Ae(e, !1)), e.textContent = "");
                         return this
                     },
                     clone: function(e, t) {
                         return e = null != e && e, t = null == t ? e : t, this.map((function() {
                             return C.clone(this, e, t)
                         }))
                     },
                     html: function(e) {
                         return ee(this, (function(e) {
                             var t = this[0] || {},
                                 n = 0,
                                 r = this.length;
                             if (void 0 === e && 1 === t.nodeType) return t.innerHTML;
-                            if ("string" == typeof e && !He.test(e) && !Ae[(ke.exec(e) || ["", ""])[1].toLowerCase()]) {
+                            if ("string" == typeof e && !He.test(e) && !Se[(ke.exec(e) || ["", ""])[1].toLowerCase()]) {
                                 e = C.htmlPrefilter(e);
                                 try {
-                                    for (; n < r; n++) 1 === (t = this[n] || {}).nodeType && (C.cleanData(Se(t, !1)), t.innerHTML = e);
+                                    for (; n < r; n++) 1 === (t = this[n] || {}).nodeType && (C.cleanData(Ae(t, !1)), t.innerHTML = e);
                                     t = 0
                                 } catch (e) {}
                             }
                             t && this.empty().append(e)
                         }), null, e, arguments.length)
                     },
                     replaceWith: function() {
                         var e = [];
                         return Ve(this, arguments, (function(t) {
                             var n = this.parentNode;
-                            C.inArray(this, e) < 0 && (C.cleanData(Se(this)), n && n.replaceChild(t, this))
+                            C.inArray(this, e) < 0 && (C.cleanData(Ae(this)), n && n.replaceChild(t, this))
                         }), e)
                     }
                 }), C.each({
                     appendTo: "append",
                     prependTo: "prepend",
                     insertBefore: "before",
                     insertAfter: "after",
@@ -4956,24 +4930,24 @@
                     hasClass: function(e) {
                         var t, n, r = 0;
                         for (t = " " + e + " "; n = this[r++];)
                             if (1 === n.nodeType && (" " + Ct(kt(n)) + " ").indexOf(t) > -1) return !0;
                         return !1
                     }
                 });
-                var At = /\r/g;
+                var St = /\r/g;
                 C.fn.extend({
                     val: function(e) {
                         var t, n, r, i = this[0];
                         return arguments.length ? (r = g(e), this.each((function(n) {
                             var i;
                             1 === this.nodeType && (null == (i = r ? e.call(this, n, C(this).val()) : e) ? i = "" : "number" == typeof i ? i += "" : Array.isArray(i) && (i = C.map(i, (function(e) {
                                 return null == e ? "" : e + ""
                             }))), (t = C.valHooks[this.type] || C.valHooks[this.nodeName.toLowerCase()]) && "set" in t && void 0 !== t.set(this, i, "value") || (this.value = i))
-                        }))) : i ? (t = C.valHooks[i.type] || C.valHooks[i.nodeName.toLowerCase()]) && "get" in t && void 0 !== (n = t.get(i, "value")) ? n : "string" == typeof(n = i.value) ? n.replace(At, "") : null == n ? "" : n : void 0
+                        }))) : i ? (t = C.valHooks[i.type] || C.valHooks[i.nodeName.toLowerCase()]) && "get" in t && void 0 !== (n = t.get(i, "value")) ? n : "string" == typeof(n = i.value) ? n.replace(St, "") : null == n ? "" : n : void 0
                     }
                 }), C.extend({
                     valHooks: {
                         option: {
                             get: function(e) {
                                 var t = C.find.attr(e, "value");
                                 return null != t ? t : Ct(C.text(e))
@@ -5003,15 +4977,15 @@
                         set: function(e, t) {
                             if (Array.isArray(t)) return e.checked = C.inArray(C(e).val(), t) > -1
                         }
                     }, v.checkOn || (C.valHooks[this].get = function(e) {
                         return null === e.getAttribute("value") ? "on" : e.value
                     })
                 }));
-                var St = r.location,
+                var At = r.location,
                     Ot = {
                         guid: Date.now()
                     },
                     Dt = /\?/;
                 C.parseXML = function(e) {
                     var t, n;
                     if (!e || "string" != typeof e) return null;
@@ -5147,22 +5121,22 @@
                 }
 
                 function Yt(e, t) {
                     var n, r, i = C.ajaxSettings.flatOptions || {};
                     for (n in t) void 0 !== t[n] && ((i[n] ? e : r || (r = {}))[n] = t[n]);
                     return r && C.extend(!0, e, r), e
                 }
-                Xt.href = St.href, C.extend({
+                Xt.href = At.href, C.extend({
                     active: 0,
                     lastModified: {},
                     etag: {},
                     ajaxSettings: {
-                        url: St.href,
+                        url: At.href,
                         type: "GET",
-                        isLocal: /^(?:about|app|app-storage|.+-extension|file|res|widget):$/.test(St.protocol),
+                        isLocal: /^(?:about|app|app-storage|.+-extension|file|res|widget):$/.test(At.protocol),
                         global: !0,
                         processData: !0,
                         async: !0,
                         contentType: "application/x-www-form-urlencoded; charset=UTF-8",
                         accepts: {
                             "*": Jt,
                             text: "text/plain",
@@ -5236,15 +5210,15 @@
                                     return this
                                 },
                                 abort: function(e) {
                                     var t = e || x;
                                     return n && n.abort(t), T(0, t), this
                                 }
                             };
-                        if (v.promise(E), d.url = ((e || d.url || St.href) + "").replace(zt, St.protocol + "//"), d.type = t.method || t.type || d.method || d.type, d.dataTypes = (d.dataType || "*").toLowerCase().match(J) || [""], null == d.crossDomain) {
+                        if (v.promise(E), d.url = ((e || d.url || At.href) + "").replace(zt, At.protocol + "//"), d.type = t.method || t.type || d.method || d.type, d.dataTypes = (d.dataType || "*").toLowerCase().match(J) || [""], null == d.crossDomain) {
                             u = _.createElement("a");
                             try {
                                 u.href = d.url, u.href = u.href, d.crossDomain = Xt.protocol + "//" + Xt.host != u.protocol + "//" + u.host
                             } catch (e) {
                                 d.crossDomain = !0
                             }
                         }
@@ -5651,32 +5625,32 @@
                 constant: () => Q,
                 contains: () => nn,
                 countBy: () => gn,
                 create: () => qe,
                 debounce: () => Ot,
                 default: () => $n,
                 defaults: () => Le,
-                defer: () => At,
+                defer: () => St,
                 delay: () => jt,
                 detect: () => Ut,
-                difference: () => Sn,
+                difference: () => An,
                 drop: () => Cn,
                 each: () => Jt,
                 escape: () => st,
                 every: () => en,
                 extend: () => Ne,
                 extendOwn: () => Me,
                 filter: () => Qt,
                 find: () => Ut,
                 findIndex: () => Rt,
                 findKey: () => qt,
                 findLastIndex: () => Bt,
                 findWhere: () => Vt,
                 first: () => Tn,
-                flatten: () => An,
+                flatten: () => Sn,
                 foldl: () => Kt,
                 foldr: () => Yt,
                 forEach: () => Jt,
                 functions: () => De,
                 get: () => $e,
                 groupBy: () => mn,
                 has: () => ze,
@@ -5690,18 +5664,18 @@
                 inject: () => Kt,
                 intersection: () => Nn,
                 invert: () => Oe,
                 invoke: () => rn,
                 isArguments: () => G,
                 isArray: () => V,
                 isArrayBuffer: () => q,
-                isBoolean: () => A,
+                isBoolean: () => S,
                 isDataView: () => U,
                 isDate: () => N,
-                isElement: () => S,
+                isElement: () => A,
                 isEmpty: () => ue,
                 isEqual: () => me,
                 isError: () => L,
                 isFinite: () => K,
                 isFunction: () => B,
                 isMap: () => Te,
                 isMatch: () => le,
@@ -5732,15 +5706,15 @@
                 mixin: () => Bn,
                 negate: () => Pt,
                 noop: () => Ze,
                 now: () => rt,
                 object: () => In,
                 omit: () => xn,
                 once: () => It,
-                pairs: () => Se,
+                pairs: () => Ae,
                 partial: () => wt,
                 partition: () => yn,
                 pick: () => wn,
                 pluck: () => on,
                 property: () => Je,
                 propertyOf: () => et,
                 random: () => nt,
@@ -5759,26 +5733,26 @@
                 sortBy: () => dn,
                 sortedIndex: () => Ft,
                 tail: () => Cn,
                 take: () => Tn,
                 tap: () => Re,
                 template: () => pt,
                 templateSettings: () => ut,
-                throttle: () => St,
+                throttle: () => At,
                 times: () => tt,
                 toArray: () => cn,
                 toPath: () => Be,
                 transpose: () => Mn,
                 unescape: () => at,
                 union: () => Pn,
                 uniq: () => Dn,
                 unique: () => Dn,
                 uniqueId: () => gt,
                 unzip: () => Mn,
-                values: () => Ae,
+                values: () => Se,
                 where: () => sn,
                 without: () => On,
                 wrap: () => Dt,
                 zip: () => Ln
             });
             var r = {};
             n.r(r), n.d(r, {
@@ -5800,32 +5774,32 @@
                 constant: () => Q,
                 contains: () => nn,
                 countBy: () => gn,
                 create: () => qe,
                 debounce: () => Ot,
                 default: () => Fn,
                 defaults: () => Le,
-                defer: () => At,
+                defer: () => St,
                 delay: () => jt,
                 detect: () => Ut,
-                difference: () => Sn,
+                difference: () => An,
                 drop: () => Cn,
                 each: () => Jt,
                 escape: () => st,
                 every: () => en,
                 extend: () => Ne,
                 extendOwn: () => Me,
                 filter: () => Qt,
                 find: () => Ut,
                 findIndex: () => Rt,
                 findKey: () => qt,
                 findLastIndex: () => Bt,
                 findWhere: () => Vt,
                 first: () => Tn,
-                flatten: () => An,
+                flatten: () => Sn,
                 foldl: () => Kt,
                 foldr: () => Yt,
                 forEach: () => Jt,
                 functions: () => De,
                 get: () => $e,
                 groupBy: () => mn,
                 has: () => ze,
@@ -5839,18 +5813,18 @@
                 inject: () => Kt,
                 intersection: () => Nn,
                 invert: () => Oe,
                 invoke: () => rn,
                 isArguments: () => G,
                 isArray: () => V,
                 isArrayBuffer: () => q,
-                isBoolean: () => A,
+                isBoolean: () => S,
                 isDataView: () => U,
                 isDate: () => N,
-                isElement: () => S,
+                isElement: () => A,
                 isEmpty: () => ue,
                 isEqual: () => me,
                 isError: () => L,
                 isFinite: () => K,
                 isFunction: () => B,
                 isMap: () => Te,
                 isMatch: () => le,
@@ -5881,15 +5855,15 @@
                 mixin: () => Bn,
                 negate: () => Pt,
                 noop: () => Ze,
                 now: () => rt,
                 object: () => In,
                 omit: () => xn,
                 once: () => It,
-                pairs: () => Se,
+                pairs: () => Ae,
                 partial: () => wt,
                 partition: () => yn,
                 pick: () => wn,
                 pluck: () => on,
                 property: () => Je,
                 propertyOf: () => et,
                 random: () => nt,
@@ -5908,26 +5882,26 @@
                 sortBy: () => dn,
                 sortedIndex: () => Ft,
                 tail: () => Cn,
                 take: () => Tn,
                 tap: () => Re,
                 template: () => pt,
                 templateSettings: () => ut,
-                throttle: () => St,
+                throttle: () => At,
                 times: () => tt,
                 toArray: () => cn,
                 toPath: () => Be,
                 transpose: () => Mn,
                 unescape: () => at,
                 union: () => Pn,
                 uniq: () => Dn,
                 unique: () => Dn,
                 uniqueId: () => gt,
                 unzip: () => Mn,
-                values: () => Ae,
+                values: () => Se,
                 where: () => sn,
                 without: () => On,
                 wrap: () => Dt,
                 zip: () => Ln
             });
             var i = "1.13.6",
                 o = "object" == typeof self && self.self === self && self || "object" == typeof n.g && n.g.global === n.g && n.g || Function("return this")() || {},
@@ -5979,19 +5953,19 @@
                 return null === e
             }
 
             function j(e) {
                 return void 0 === e
             }
 
-            function A(e) {
+            function S(e) {
                 return !0 === e || !1 === e || "[object Boolean]" === f.call(e)
             }
 
-            function S(e) {
+            function A(e) {
                 return !(!e || 1 !== e.nodeType)
             }
 
             function O(e) {
                 var t = "[object " + e + "]";
                 return function(e) {
                     return f.call(e) === t
@@ -6210,20 +6184,20 @@
                 xe = _e.concat(be),
                 Ee = ["add"].concat(_e, ye, "has");
             const Te = $ ? ge(we) : O("Map"),
                 Ce = $ ? ge(xe) : O("WeakMap"),
                 ke = $ ? ge(Ee) : O("Set"),
                 je = O("WeakSet");
 
-            function Ae(e) {
+            function Se(e) {
                 for (var t = ae(e), n = t.length, r = Array(n), i = 0; i < n; i++) r[i] = e[t[i]];
                 return r
             }
 
-            function Se(e) {
+            function Ae(e) {
                 for (var t = ae(e), n = t.length, r = Array(n), i = 0; i < n; i++) r[i] = [t[i], e[t[i]]];
                 return r
             }
 
             function Oe(e) {
                 for (var t = {}, n = ae(e), r = 0, i = n.length; r < i; r++) t[e[n[r]]] = n[r];
                 return t
@@ -6532,17 +6506,17 @@
                 return n.cache = {}, n
             }
             const jt = T((function(e, t, n) {
                     return setTimeout((function() {
                         return e.apply(null, n)
                     }), t)
                 })),
-                At = wt(jt, ce, 1);
+                St = wt(jt, ce, 1);
 
-            function St(e, t, n) {
+            function At(e, t, n) {
                 var r, i, o, s, a = 0;
                 n || (n = {});
                 var u = function() {
                         a = !1 === n.leading ? 0 : rt(), r = null, s = e.apply(i, o), r || (i = o = null)
                     },
                     l = function() {
                         var l = rt();
@@ -6714,15 +6688,15 @@
                     var s = r ? r[o] : o;
                     if (t(e[s], s, e)) return !0
                 }
                 return !1
             }
 
             function nn(e, t, n, r) {
-                return Et(e) || (e = Ae(e)), ("number" != typeof n || r) && (n = 0), $t(e, t, n) >= 0
+                return Et(e) || (e = Se(e)), ("number" != typeof n || r) && (n = 0), $t(e, t, n) >= 0
             }
             const rn = T((function(e, t, n) {
                 var r, i;
                 return B(t) ? i = t : (t = Fe(t), r = t.slice(0, -1), t = t[t.length - 1]), Xt(e, (function(e) {
                     var o = i;
                     if (!o) {
                         if (r && r.length && (e = We(e, r)), null == e) return;
@@ -6740,39 +6714,39 @@
                 return Qt(e, Ve(t))
             }
 
             function an(e, t, n) {
                 var r, i, o = -1 / 0,
                     s = -1 / 0;
                 if (null == t || "number" == typeof t && "object" != typeof e[0] && null != e)
-                    for (var a = 0, u = (e = Et(e) ? e : Ae(e)).length; a < u; a++) null != (r = e[a]) && r > o && (o = r);
+                    for (var a = 0, u = (e = Et(e) ? e : Se(e)).length; a < u; a++) null != (r = e[a]) && r > o && (o = r);
                 else t = Ye(t, n), Jt(e, (function(e, n, r) {
                     ((i = t(e, n, r)) > s || i === -1 / 0 && o === -1 / 0) && (o = e, s = i)
                 }));
                 return o
             }
 
             function un(e, t, n) {
                 var r, i, o = 1 / 0,
                     s = 1 / 0;
                 if (null == t || "number" == typeof t && "object" != typeof e[0] && null != e)
-                    for (var a = 0, u = (e = Et(e) ? e : Ae(e)).length; a < u; a++) null != (r = e[a]) && r < o && (o = r);
+                    for (var a = 0, u = (e = Et(e) ? e : Se(e)).length; a < u; a++) null != (r = e[a]) && r < o && (o = r);
                 else t = Ye(t, n), Jt(e, (function(e, n, r) {
                     ((i = t(e, n, r)) < s || i === 1 / 0 && o === 1 / 0) && (o = e, s = i)
                 }));
                 return o
             }
             var ln = /[^\ud800-\udfff]|[\ud800-\udbff][\udc00-\udfff]|[\ud800-\udfff]/g;
 
             function cn(e) {
-                return e ? V(e) ? c.call(e) : D(e) ? e.match(ln) : Et(e) ? Xt(e, Ue) : Ae(e) : []
+                return e ? V(e) ? c.call(e) : D(e) ? e.match(ln) : Et(e) ? Xt(e, Ue) : Se(e) : []
             }
 
             function fn(e, t, n) {
-                if (null == t || n) return Et(e) || (e = Ae(e)), e[nt(e.length - 1)];
+                if (null == t || n) return Et(e) || (e = Se(e)), e[nt(e.length - 1)];
                 var r = cn(e),
                     i = oe(r);
                 t = Math.max(Math.min(t, i), 0);
                 for (var o = i - 1, s = 0; s < t; s++) {
                     var a = nt(s, o),
                         u = r[s];
                     r[s] = r[a], r[a] = u
@@ -6870,28 +6844,28 @@
                 return null == e || e.length < 1 ? null == t || n ? void 0 : [] : null == t || n ? e[e.length - 1] : Cn(e, Math.max(0, e.length - t))
             }
 
             function jn(e) {
                 return Qt(e, Boolean)
             }
 
-            function An(e, t) {
+            function Sn(e, t) {
                 return Tt(e, t, !1)
             }
-            const Sn = T((function(e, t) {
+            const An = T((function(e, t) {
                     return t = Tt(t, !0, !0), Qt(e, (function(e) {
                         return !nn(t, e)
                     }))
                 })),
                 On = T((function(e, t) {
-                    return Sn(e, t)
+                    return An(e, t)
                 }));
 
             function Dn(e, t, n, r) {
-                A(t) || (r = n, n = t, t = !1), null != n && (n = Ye(n, r));
+                S(t) || (r = n, n = t, t = !1), null != n && (n = Ye(n, r));
                 for (var i = [], o = [], s = 0, a = oe(e); s < a; s++) {
                     var u = e[s],
                         l = n ? n(u, s, e) : u;
                     t && !n ? (s && o === l || i.push(u), o = l) : n ? nn(o, l) || (o.push(l), i.push(u)) : nn(i, u) || i.push(u)
                 }
                 return i
             }
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/labextension/static/744.fcbd28431423403c9c8b.js` & `tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/744.33b070180c108b7cf8c9.js`

 * *Files 13% similar despite different names*

#### js-beautify {}

```diff
@@ -3,37 +3,37 @@
     [744], {
         1744: (e, i, t) => {
             t.r(i), t.d(i, {
                 default: () => m
             });
             var l = {};
             t.r(l), t.d(l, {
-                BioImageViewerModel: () => p,
-                BioImageViewerView: () => d
+                BioImageViewerModel: () => d,
+                BioImageViewerView: () => p
             });
-            var s = t(6704);
+            var s = t(8233);
             const n = t(4147),
                 r = n.version,
                 o = n.name;
             var a = t(2832),
                 u = t.n(a);
-            class p extends s.DOMWidgetModel {
+            class d extends s.DOMWidgetModel {
                 defaults() {
                     return Object.assign(Object.assign({}, super.defaults()), {
-                        _model_name: p.model_name,
-                        _model_module: p.model_module,
-                        _model_module_version: p.model_module_version,
-                        _view_name: p.view_name,
-                        _view_module: p.view_module,
-                        _view_module_version: p.view_module_version
+                        _model_name: d.model_name,
+                        _model_module: d.model_module,
+                        _model_module_version: d.model_module_version,
+                        _view_name: d.view_name,
+                        _view_module: d.view_module,
+                        _view_module_version: d.view_module_version
                     })
                 }
             }
-            p.model_module = o, p.model_module_version = r, p.view_module = o, p.view_module_version = r, p.serializers = Object.assign({}, s.DOMWidgetModel.serializers), p.model_name = "BioImageViewerModel", p.view_name = "BioImageViewerView";
-            class d extends s.DOMWidgetView {
+            d.model_module = o, d.model_module_version = r, d.view_module = o, d.view_module_version = r, d.serializers = Object.assign({}, s.DOMWidgetModel.serializers), d.model_name = "BioImageViewerModel", d.view_name = "BioImageViewerView";
+            class p extends s.DOMWidgetView {
                 constructor() {
                     super(...arguments), this.values = this.model.get("value")
                 }
                 render() {
                     const e = document.createElement("div");
                     this.el.appendChild(e), u()({
                         rootElement: e,
@@ -53,11 +53,11 @@
                         version: r,
                         exports: l
                     })
                 }
             }
         },
         4147: e => {
-            e.exports = JSON.parse('{"name":"@tiledb-inc/jupyter-bioimage-viewer","version":"0.1.1-alpha.0","description":"A jupyterlab extension to visualize bioimages in TileDB format","keywords":["jupyter","jupyterlab","jupyterlab-extension"],"homepage":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer","bugs":{"url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer/issues"},"license":"BSD-3-Clause","author":"TileDB","files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","repository":{"type":"git","url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer.git"},"scripts":{"test":"echo No tests yet","build":"jlpm run build:lib && jlpm run build:labextension:dev","build:prod":"jlpm run build:lib && jlpm run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","clean":"jlpm run clean:lib","clean:lib":"rimraf lib tsconfig.tsbuildinfo","clean:labextension":"rimraf tiledb_jupyter_bioimg/labextension","clean:all":"jlpm run clean:lib && jlpm run clean:labextension","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:extension":"jupyter labextension develop --overwrite .","prepare":"jlpm run clean && jlpm run build:prod","watch":"run-p watch:src watch:labextension","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5","@jupyterlab/application":"^3.4.5","@tiledb-inc/bioimage-viewer":"^0.1.0-alpha.7"},"devDependencies":{"@jupyterlab/builder":"^3.1.0","@typescript-eslint/eslint-plugin":"^2.27.0","@typescript-eslint/parser":"^2.27.0","eslint":"^7.5.0","eslint-config-prettier":"^6.10.1","eslint-plugin-prettier":"^3.1.2","npm-run-all":"^4.1.5","prettier":"^1.19.0","rimraf":"^3.0.2","typescript":"~4.1.3"},"sideEffects":["style/*.css","style/index.js"],"styleModule":"style/index.js","jupyterlab":{"extension":"lib/index","outputDir":"tiledb_jupyter_bioimg/labextension","webpackConfig":"./webpack.config.js"}}')
+            e.exports = JSON.parse('{"name":"@tiledb-inc/jupyter-bioimage-viewer","version":"0.1.1-alpha.1","description":"A jupyterlab extension to visualize bioimages in TileDB format","keywords":["jupyter","jupyterlab","jupyterlab-extension"],"homepage":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer","bugs":{"url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer/issues"},"license":"BSD-3-Clause","author":"TileDB","files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","style/*.css","style/index.js"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","repository":{"type":"git","url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer.git"},"scripts":{"test":"echo No tests yet","build":"jlpm run build:lib && jlpm run build:labextension:dev","build:prod":"jlpm run build:lib && jlpm run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","clean":"jlpm run clean:lib","clean:lib":"rimraf lib tsconfig.tsbuildinfo","clean:labextension":"rimraf tiledb_jupyter_bioimg/labextension","clean:all":"jlpm run clean:lib && jlpm run clean:labextension","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:extension":"jupyter labextension develop --overwrite .","prepare":"jlpm run clean && jlpm run build:prod","watch":"run-p watch:src watch:labextension","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4","@jupyterlab/application":"^3.4.5","@tiledb-inc/bioimage-viewer":"^0.1.0-alpha.7"},"devDependencies":{"@jupyterlab/builder":"^3.1.0","@typescript-eslint/eslint-plugin":"^2.27.0","@typescript-eslint/parser":"^2.27.0","eslint":"^7.5.0","eslint-config-prettier":"^6.10.1","eslint-plugin-prettier":"^3.1.2","npm-run-all":"^4.1.5","prettier":"^1.19.0","rimraf":"^3.0.2","typescript":"~4.1.3"},"sideEffects":["style/*.css","style/index.js"],"styleModule":"style/index.js","jupyterlab":{"extension":"lib/index","outputDir":"tiledb_jupyter_bioimg/labextension","webpackConfig":"./webpack.config.js"}}')
         }
     }
 ]);
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js` & `tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/labextension/static/remoteEntry.c73b66672555e7ef21cd.js` & `tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/remoteEntry.b0daa29a1375bdb34258.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, n, i, o, d, l, u, s, c, f, p, h, b, v, m, g, y = {
+    var e, r, t, a, n, i, o, d, l, u, s, f, c, p, h, b, v, m, g, y = {
             5290: (e, r, t) => {
                 var a = {
                         "./index": () => t.e(744).then((() => () => t(1744))),
                         "./extension": () => t.e(744).then((() => () => t(1744))),
                         "./style": () => t.e(747).then((() => () => t(9747)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
@@ -50,26 +50,26 @@
     }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
         38: "06c00f555d53e8ae5aa5",
         172: "6267f3dd3063477e34ed",
         344: "8db93920a8ca0f0600d9",
         446: "3bf34f45c93ace9c0f28",
         633: "770b26571c8b948a69e3",
         635: "024275f22a135fe53126",
-        713: "75fe0d9ef4c6ff1de4d7",
-        744: "fcbd28431423403c9c8b",
+        713: "44bebcfa12a45c30ff83",
+        744: "33b070180c108b7cf8c9",
         747: "433530952542f03ebc71"
     } [e] + ".js?v=" + {
         38: "06c00f555d53e8ae5aa5",
         172: "6267f3dd3063477e34ed",
         344: "8db93920a8ca0f0600d9",
         446: "3bf34f45c93ace9c0f28",
         633: "770b26571c8b948a69e3",
         635: "024275f22a135fe53126",
-        713: "75fe0d9ef4c6ff1de4d7",
-        744: "fcbd28431423403c9c8b",
+        713: "44bebcfa12a45c30ff83",
+        744: "33b070180c108b7cf8c9",
         747: "433530952542f03ebc71"
     } [e], j.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
@@ -88,24 +88,24 @@
                     var s = l[u];
                     if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + n) {
                         o = s;
                         break
                     }
                 }
             o || (d = !0, (o = document.createElement("script")).charset = "utf-8", o.timeout = 120, j.nc && o.setAttribute("nonce", j.nc), o.setAttribute("data-webpack", r + n), o.src = t), e[t] = [a];
-            var c = (r, a) => {
-                    o.onerror = o.onload = null, clearTimeout(f);
+            var f = (r, a) => {
+                    o.onerror = o.onload = null, clearTimeout(c);
                     var n = e[t];
                     if (delete e[t], o.parentNode && o.parentNode.removeChild(o), n && n.forEach((e => e(a))), r) return r(a)
                 },
-                f = setTimeout(c.bind(null, void 0, {
+                c = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: o
                 }), 12e4);
-            o.onerror = c.bind(null, o.onerror), o.onload = c.bind(null, o.onload), d && document.head.appendChild(o)
+            o.onerror = f.bind(null, o.onerror), o.onload = f.bind(null, o.onload), d && document.head.appendChild(o)
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
-                return "default" === t && (d("@jupyter-widgets/base", "4.1.4", (() => Promise.all([j.e(172), j.e(713), j.e(38)]).then((() => () => j(2713))))), d("@tiledb-inc/bioimage-viewer", "0.1.0-alpha.7", (() => Promise.all([j.e(635), j.e(172), j.e(344), j.e(446)]).then((() => () => j(344))))), d("@tiledb-inc/jupyter-bioimage-viewer", "0.1.1-alpha.0", (() => j.e(744).then((() => () => j(1744)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (d("@jupyter-widgets/base", "4.1.1", (() => Promise.all([j.e(172), j.e(713), j.e(38)]).then((() => () => j(2713))))), d("@tiledb-inc/bioimage-viewer", "0.1.0-alpha.7", (() => Promise.all([j.e(635), j.e(172), j.e(344), j.e(446)]).then((() => () => j(344))))), d("@tiledb-inc/jupyter-bioimage-viewer", "0.1.1-alpha.1", (() => j.e(744).then((() => () => j(1744)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -185,80 +185,79 @@
     }, i = (e, r) => {
         if (0 in e) {
             r = t(r);
             var a = e[0],
                 n = a < 0;
             n && (a = -a - 1);
             for (var o = 0, d = 1, l = !0;; d++, o++) {
-                var u, s, c = d < e.length ? (typeof e[d])[0] : "";
-                if (o >= r.length || "o" == (s = (typeof(u = r[o]))[0])) return !l || ("u" == c ? d > a && !n : "" == c != n);
+                var u, s, f = d < e.length ? (typeof e[d])[0] : "";
+                if (o >= r.length || "o" == (s = (typeof(u = r[o]))[0])) return !l || ("u" == f ? d > a && !n : "" == f != n);
                 if ("u" == s) {
-                    if (!l || "u" != c) return !1
+                    if (!l || "u" != f) return !1
                 } else if (l)
-                    if (c == s)
+                    if (f == s)
                         if (d <= a) {
                             if (u != e[d]) return !1
                         } else {
                             if (n ? u > e[d] : u < e[d]) return !1;
                             u != e[d] && (l = !1)
                         }
-                else if ("s" != c && "n" != c) {
+                else if ("s" != f && "n" != f) {
                     if (n || d <= a) return !1;
                     l = !1, d--
                 } else {
-                    if (d <= a || s < c != n) return !1;
+                    if (d <= a || s < f != n) return !1;
                     l = !1
-                } else "s" != c && "n" != c && (l = !1, d--)
+                } else "s" != f && "n" != f && (l = !1, d--)
             }
         }
-        var f = [],
-            p = f.pop.bind(f);
+        var c = [],
+            p = c.pop.bind(c);
         for (o = 1; o < e.length; o++) {
             var h = e[o];
-            f.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? i(h, r) : !p())
+            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? i(h, r) : !p())
         }
         return !!p()
     }, o = (e, r) => {
         var t = j.S[e];
         if (!t || !j.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, d = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
     }, l = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", u = (e, r, t, a) => {
         var n = d(e, t);
-        return i(a, n) || c(l(e, t, n, a)), f(e[t][n])
+        return i(a, n) || f(l(e, t, n, a)), c(e[t][n])
     }, s = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !i(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
-    }, c = e => {
+    }, f = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, f = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, a, n) {
+    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, a, n) {
         var i = j.I(r);
         return i && i.then ? i.then(e.bind(e, r, j.S[r], t, a, n)) : e(r, j.S[r], t, a, n)
     })(((e, r, t, a) => (o(e, t), u(r, 0, t, a)))), b = p(((e, r, t, a, n) => {
         var i = r && j.o(r, t) && s(r, t, a);
-        return i ? f(i) : n()
+        return i ? c(i) : n()
     })), v = {}, m = {
         2832: () => b("default", "@tiledb-inc/bioimage-viewer", [2, 0, 1, 0, , "alpha", 7], (() => Promise.all([j.e(635), j.e(172), j.e(344), j.e(446)]).then((() => () => j(344))))),
-        6704: () => b("default", "@jupyter-widgets/base", [, [1, 5],
-            [1, 4],
+        8233: () => b("default", "@jupyter-widgets/base", [, [1, 4],
             [1, 3],
             [1, 2],
-            [1, 1, 1, 10], 1, 1, 1, 1
+            [1, 1, 1, 10], 1, 1, 1
         ], (() => Promise.all([j.e(172), j.e(713), j.e(38)]).then((() => () => j(2713))))),
         1526: () => h("default", "@lumino/coreutils", [1, 1, 11, 0]),
         2720: () => h("default", "@lumino/messaging", [1, 1, 10, 0]),
         8832: () => h("default", "@lumino/widgets", [1, 1, 37, 2]),
         4456: () => h("default", "react-dom", [1, 17, 0, 1]),
         6271: () => h("default", "react", [1, 17, 0, 1])
     }, g = {
         38: [1526, 2720, 8832],
         446: [4456, 6271],
-        744: [2832, 6704]
+        744: [2832, 8233]
     }, j.f.consumes = (e, r) => {
         j.o(g, e) && g[e].forEach((e => {
             if (j.o(v, e)) return r.push(v[e]);
             var t = r => {
                     v[e] = 0, j.m[e] = t => {
                         delete j.c[e], t.exports = r()
                     }
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json` & `tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998991935483871%*

 * *Differences: {"'packages'": "{6: {'versionInfo': '4.1.1'}}"}*

```diff
@@ -36,15 +36,15 @@
             "name": "@icons/material",
             "versionInfo": "0.2.4"
         },
         {
             "extractedText": "Copyright (c) 2015 Project Jupyter Contributors\nAll rights reserved.\n\nRedistribution and use in source and binary forms, with or without\nmodification, are permitted provided that the following conditions are met:\n\n1. Redistributions of source code must retain the above copyright notice, this\n   list of conditions and the following disclaimer.\n\n2. Redistributions in binary form must reproduce the above copyright notice,\n   this list of conditions and the following disclaimer in the documentation\n   and/or other materials provided with the distribution.\n\n3. Neither the name of the copyright holder nor the names of its\n   contributors may be used to endorse or promote products derived from\n   this software without specific prior written permission.\n\nTHIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS \"AS IS\"\nAND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE\nIMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE\nDISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE\nFOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL\nDAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR\nSERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER\nCAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,\nOR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE\nOF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.\n",
             "licenseId": "BSD-3-Clause",
             "name": "@jupyter-widgets/base",
-            "versionInfo": "4.1.4"
+            "versionInfo": "4.1.1"
         },
         {
             "extractedText": "Copyright (c) 2015 Uber Technologies, Inc.\n\nThis software includes parts of PhiloGL (https://github.com/philogb/philogl)\nunder MIT license. PhiloGL parts Copyright \u00a9 2013 Sencha Labs.\n\nThis software includes adaptations of postprocessing code from THREE.js (https://github.com/mrdoob/three.js/) under MIT license. Additional attribution given in specific source files. THREE.js parts Copyright \u00a9 2010-2018 three.js authors.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN\nTHE SOFTWARE.\n\n\nloaders.gl includes certain files from Cesium (https://github.com/AnalyticalGraphicsInc/cesium) under the Apache 2 License:\n\nCopyright 2011-2018 CesiumJS Contributors\n\nLicensed under the Apache License, Version 2.0 (the \"License\");\nyou may not use this file except in compliance with the License.\nYou may obtain a copy of the License at\nhttp://www.apache.org/licenses/LICENSE-2.0\n\nUnless required by applicable law or agreed to in writing, software\ndistributed under the License is distributed on an \"AS IS\" BASIS,\nWITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.\nSee the License for the specific language governing permissions and limitations under the License.\n\nCesium-derived code can be found in the submodule: modules/3d-tiles\n",
             "licenseId": "MIT",
             "name": "@loaders.gl/core",
             "versionInfo": "3.4.4"
         },
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg/render.py` & `tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg/render.py`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg.egg-info/PKG-INFO` & `tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledb-jupyter-bioimg
-Version: 0.1.1a0
+Version: 0.1.1a1
 Summary: A jupyterlab extension to visualize bioimages in TileDB format
 Home-page: https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer
 Author: TileDB
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a0/tiledb_jupyter_bioimg.egg-info/SOURCES.txt` & `tiledb_jupyter_bioimg-0.1.1a1/tiledb_jupyter_bioimg.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,14 @@
 tiledb_jupyter_bioimg/labextension/static/172.6267f3dd3063477e34ed.js
 tiledb_jupyter_bioimg/labextension/static/344.8db93920a8ca0f0600d9.js
 tiledb_jupyter_bioimg/labextension/static/344.8db93920a8ca0f0600d9.js.LICENSE.txt
 tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
 tiledb_jupyter_bioimg/labextension/static/633.770b26571c8b948a69e3.js
 tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js
 tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js.LICENSE.txt
-tiledb_jupyter_bioimg/labextension/static/713.75fe0d9ef4c6ff1de4d7.js
-tiledb_jupyter_bioimg/labextension/static/713.75fe0d9ef4c6ff1de4d7.js.LICENSE.txt
-tiledb_jupyter_bioimg/labextension/static/744.fcbd28431423403c9c8b.js
+tiledb_jupyter_bioimg/labextension/static/713.44bebcfa12a45c30ff83.js
+tiledb_jupyter_bioimg/labextension/static/713.44bebcfa12a45c30ff83.js.LICENSE.txt
+tiledb_jupyter_bioimg/labextension/static/744.33b070180c108b7cf8c9.js
 tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js
-tiledb_jupyter_bioimg/labextension/static/remoteEntry.c73b66672555e7ef21cd.js
+tiledb_jupyter_bioimg/labextension/static/remoteEntry.b0daa29a1375bdb34258.js
 tiledb_jupyter_bioimg/labextension/static/style.js
 tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a0/tsconfig.json` & `tiledb_jupyter_bioimg-0.1.1a1/tsconfig.json`

 * *Files identical despite different names*

