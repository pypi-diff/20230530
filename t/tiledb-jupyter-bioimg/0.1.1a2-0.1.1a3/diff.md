# Comparing `tmp/tiledb_jupyter_bioimg-0.1.1a2.tar.gz` & `tmp/tiledb_jupyter_bioimg-0.1.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tiledb_jupyter_bioimg-0.1.1a2.tar", last modified: Tue May 30 11:37:45 2023, max compression
+gzip compressed data, was "tiledb_jupyter_bioimg-0.1.1a3.tar", last modified: Tue May 30 12:32:10 2023, max compression
```

## Comparing `tiledb_jupyter_bioimg-0.1.1a2.tar` & `tiledb_jupyter_bioimg-0.1.1a3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:37:45.178763 tiledb_jupyter_bioimg-0.1.1a2/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-30 11:32:53.000000 tiledb_jupyter_bioimg-0.1.1a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-30 11:32:53.000000 tiledb_jupyter_bioimg-0.1.1a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-30 11:37:45.178763 tiledb_jupyter_bioimg-0.1.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-30 11:32:53.000000 tiledb_jupyter_bioimg-0.1.1a2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-30 11:32:53.000000 tiledb_jupyter_bioimg-0.1.1a2/install.json
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-05-30 11:35:14.000000 tiledb_jupyter_bioimg-0.1.1a2/package.json
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-30 11:32:53.000000 tiledb_jupyter_bioimg-0.1.1a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 11:37:45.178763 tiledb_jupyter_bioimg-0.1.1a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-30 11:32:53.000000 tiledb_jupyter_bioimg-0.1.1a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:37:45.174762 tiledb_jupyter_bioimg-0.1.1a2/src/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-30 11:32:53.000000 tiledb_jupyter_bioimg-0.1.1a2/src/index.ts
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-30 11:32:53.000000 tiledb_jupyter_bioimg-0.1.1a2/src/version.ts
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-30 11:32:53.000000 tiledb_jupyter_bioimg-0.1.1a2/src/widget.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:37:45.174762 tiledb_jupyter_bioimg-0.1.1a2/style/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:32:53.000000 tiledb_jupyter_bioimg-0.1.1a2/style/base.css
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 11:32:53.000000 tiledb_jupyter_bioimg-0.1.1a2/style/index.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-30 11:32:53.000000 tiledb_jupyter_bioimg-0.1.1a2/style/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:37:45.174762 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-30 11:32:53.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-30 11:32:53.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-30 11:32:53.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:37:45.174762 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-30 11:37:43.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:37:45.178763 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/
--rw-r--r--   0 runner    (1001) docker     (123)   189298 2023-05-30 11:37:43.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14610 2023-05-30 11:37:43.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/172.6267f3dd3063477e34ed.js
--rw-r--r--   0 runner    (1001) docker     (123)   725916 2023-05-30 11:37:43.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/344.8db93920a8ca0f0600d9.js
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-30 11:37:43.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/344.8db93920a8ca0f0600d9.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-30 11:37:43.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-30 11:37:43.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/633.86ebe895050415abdfba.js
--rw-r--r--   0 runner    (1001) docker     (123)   516693 2023-05-30 11:37:43.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/635.ce138c9764842046bf90.js
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-30 11:37:43.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/635.ce138c9764842046bf90.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   172313 2023-05-30 11:37:43.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/713.44bebcfa12a45c30ff83.js
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-30 11:37:43.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/713.44bebcfa12a45c30ff83.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-05-30 11:37:43.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/744.9655cb2c54e12e1c2654.js
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-30 11:37:43.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js
--rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-05-30 11:37:43.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/remoteEntry.f05f71ea95cf3364c4cb.js
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-30 11:37:12.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/style.js
--rw-r--r--   0 runner    (1001) docker     (123)    90733 2023-05-30 11:37:43.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-30 11:32:53.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/render.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:37:45.174762 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-30 11:37:45.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-30 11:37:45.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:37:45.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:36:21.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-30 11:37:45.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 11:37:45.000000 tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-30 11:32:53.000000 tiledb_jupyter_bioimg-0.1.1a2/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:32:10.431654 tiledb_jupyter_bioimg-0.1.1a3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-30 12:26:54.000000 tiledb_jupyter_bioimg-0.1.1a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-30 12:26:54.000000 tiledb_jupyter_bioimg-0.1.1a3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-30 12:32:10.431654 tiledb_jupyter_bioimg-0.1.1a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-30 12:26:54.000000 tiledb_jupyter_bioimg-0.1.1a3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-30 12:26:54.000000 tiledb_jupyter_bioimg-0.1.1a3/install.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-30 12:29:24.000000 tiledb_jupyter_bioimg-0.1.1a3/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-30 12:26:54.000000 tiledb_jupyter_bioimg-0.1.1a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 12:32:10.431654 tiledb_jupyter_bioimg-0.1.1a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-30 12:26:54.000000 tiledb_jupyter_bioimg-0.1.1a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:32:10.423653 tiledb_jupyter_bioimg-0.1.1a3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-30 12:26:54.000000 tiledb_jupyter_bioimg-0.1.1a3/src/index.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-30 12:26:54.000000 tiledb_jupyter_bioimg-0.1.1a3/src/version.ts
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-30 12:26:54.000000 tiledb_jupyter_bioimg-0.1.1a3/src/widget.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:32:10.423653 tiledb_jupyter_bioimg-0.1.1a3/style/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:26:54.000000 tiledb_jupyter_bioimg-0.1.1a3/style/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 12:26:54.000000 tiledb_jupyter_bioimg-0.1.1a3/style/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-30 12:26:54.000000 tiledb_jupyter_bioimg-0.1.1a3/style/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:32:10.423653 tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-30 12:26:54.000000 tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-30 12:26:54.000000 tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-30 12:26:54.000000 tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:32:10.423653 tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/labextension/
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-30 12:32:09.000000 tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/labextension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:32:10.431654 tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/labextension/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   189298 2023-05-30 12:32:09.000000 tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14610 2023-05-30 12:32:09.000000 tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/labextension/static/172.6267f3dd3063477e34ed.js
+-rw-r--r--   0 runner    (1001) docker     (123)   725862 2023-05-30 12:32:09.000000 tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/labextension/static/344.8d6b91ad4356dae38b22.js
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-30 12:32:09.000000 tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/labextension/static/344.8d6b91ad4356dae38b22.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-30 12:32:09.000000 tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-30 12:32:09.000000 tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/labextension/static/633.770b26571c8b948a69e3.js
+-rw-r--r--   0 runner    (1001) docker     (123)   516691 2023-05-30 12:32:09.000000 tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-30 12:32:09.000000 tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   172313 2023-05-30 12:32:09.000000 tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/labextension/static/713.44bebcfa12a45c30ff83.js
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-30 12:32:09.000000 tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/labextension/static/713.44bebcfa12a45c30ff83.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-30 12:32:09.000000 tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/labextension/static/744.3b4d2f36290dd421bc4f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-30 12:32:09.000000 tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-05-30 12:32:09.000000 tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/labextension/static/remoteEntry.ad93eef0e33172dacb16.js
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-30 12:31:35.000000 tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/labextension/static/style.js
+-rw-r--r--   0 runner    (1001) docker     (123)    90733 2023-05-30 12:32:09.000000 tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-30 12:26:54.000000 tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/render.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:32:10.423653 tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-05-30 12:32:10.000000 tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-30 12:32:10.000000 tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:32:10.000000 tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:30:40.000000 tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-30 12:32:10.000000 tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 12:32:10.000000 tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-30 12:26:54.000000 tiledb_jupyter_bioimg-0.1.1a3/tsconfig.json
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a2/LICENSE` & `tiledb_jupyter_bioimg-0.1.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a2/PKG-INFO` & `tiledb_jupyter_bioimg-0.1.1a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledb_jupyter_bioimg
-Version: 0.1.1a2
+Version: 0.1.1a3
 Summary: A jupyterlab extension to visualize bioimages in TileDB format
 Home-page: https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer
 Author: TileDB
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a2/README.md` & `tiledb_jupyter_bioimg-0.1.1a3/README.md`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a2/package.json` & `tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/labextension/package.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.91875%*

 * *Differences: {"'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.ad93eef0e33172dacb16.js'), "*

 * *                 "('extension', './extension'), ('style', './style')])}",*

 * * "'resolutions'": "OrderedDict([('@luma.gl/constants', '8.5.16'), ('@luma.gl/core', '8.5.16'), "*

 * *                  "('@luma.gl/engine', '8.5.16'), ('@luma.gl/gltools', '8.5.16'), "*

 * *                  "('@luma.gl/shadertools', '8.5.16'), ('@luma.gl/webgl', '8.5.16'), "*

 * *                  "('@luma.gl/experimental', '8.5.16')])",*

 * * "'version' […]*

```diff
@@ -25,14 +25,19 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.ad93eef0e33172dacb16.js",
+            "style": "./style"
+        },
         "extension": "lib/index",
         "outputDir": "tiledb_jupyter_bioimg/labextension",
         "webpackConfig": "./webpack.config.js"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
@@ -41,14 +46,23 @@
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
     "name": "@tiledb-inc/jupyter-bioimage-viewer",
     "repository": {
         "type": "git",
         "url": "https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer.git"
     },
+    "resolutions": {
+        "@luma.gl/constants": "8.5.16",
+        "@luma.gl/core": "8.5.16",
+        "@luma.gl/engine": "8.5.16",
+        "@luma.gl/experimental": "8.5.16",
+        "@luma.gl/gltools": "8.5.16",
+        "@luma.gl/shadertools": "8.5.16",
+        "@luma.gl/webgl": "8.5.16"
+    },
     "scripts": {
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc",
         "build:prod": "jlpm run build:lib && jlpm run build:labextension",
         "clean": "jlpm run clean:lib",
@@ -67,9 +81,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.1-alpha.2"
+    "version": "0.1.1-alpha.3"
 }
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a2/setup.py` & `tiledb_jupyter_bioimg-0.1.1a3/setup.py`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a2/src/index.ts` & `tiledb_jupyter_bioimg-0.1.1a3/src/index.ts`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a2/src/version.ts` & `tiledb_jupyter_bioimg-0.1.1a3/src/version.ts`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a2/src/widget.ts` & `tiledb_jupyter_bioimg-0.1.1a3/src/widget.ts`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/_version.py` & `tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/_version.py`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/package.json` & `tiledb_jupyter_bioimg-0.1.1a3/package.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.91875%*

 * *Differences: {"'jupyterlab'": "{delete: ['_build']}",*

 * * "'resolutions'": "OrderedDict([('@luma.gl/constants', '8.5.16'), ('@luma.gl/core', '8.5.16'), "*

 * *                  "('@luma.gl/engine', '8.5.16'), ('@luma.gl/gltools', '8.5.16'), "*

 * *                  "('@luma.gl/shadertools', '8.5.16'), ('@luma.gl/webgl', '8.5.16'), "*

 * *                  "('@luma.gl/experimental', '8.5.16')])",*

 * * "'version'": "'0.1.1-alpha.3'"}*

```diff
@@ -25,19 +25,14 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.f05f71ea95cf3364c4cb.js",
-            "style": "./style"
-        },
         "extension": "lib/index",
         "outputDir": "tiledb_jupyter_bioimg/labextension",
         "webpackConfig": "./webpack.config.js"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
@@ -46,14 +41,23 @@
     "license": "BSD-3-Clause",
     "main": "lib/index.js",
     "name": "@tiledb-inc/jupyter-bioimage-viewer",
     "repository": {
         "type": "git",
         "url": "https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer.git"
     },
+    "resolutions": {
+        "@luma.gl/constants": "8.5.16",
+        "@luma.gl/core": "8.5.16",
+        "@luma.gl/engine": "8.5.16",
+        "@luma.gl/experimental": "8.5.16",
+        "@luma.gl/gltools": "8.5.16",
+        "@luma.gl/shadertools": "8.5.16",
+        "@luma.gl/webgl": "8.5.16"
+    },
     "scripts": {
         "build": "jlpm run build:lib && jlpm run build:labextension:dev",
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc",
         "build:prod": "jlpm run build:lib && jlpm run build:labextension",
         "clean": "jlpm run clean:lib",
@@ -72,9 +76,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.1-alpha.2"
+    "version": "0.1.1-alpha.3"
 }
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg` & `tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/172.6267f3dd3063477e34ed.js` & `tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/labextension/static/172.6267f3dd3063477e34ed.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/344.8db93920a8ca0f0600d9.js` & `tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/labextension/static/344.8d6b91ad4356dae38b22.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 344.8db93920a8ca0f0600d9.js.LICENSE.txt */
+/*! For license information please see 344.8d6b91ad4356dae38b22.js.LICENSE.txt */
 (self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer = self.webpackChunk_tiledb_inc_jupyter_bioimage_viewer || []).push([
     [344], {
         597: (t, e, n) => {
             "use strict";
             var i, r = Object.assign || function(t) {
                     for (var e = 1; e < arguments.length; e++) {
                         var n = arguments[e];
@@ -76,15 +76,15 @@
                     d: "M12,18.17L8.83,15L7.42,16.41L12,21L16.59,16.41L15.17,15M12,5.83L15.17,9L16.58,7.59L12,3L7.41,7.59L8.83,9L12,5.83Z"
                 }))
             }
         },
         344: (t, e, n) => {
             "use strict";
             n.r(e), n.d(e, {
-                default: () => rE
+                default: () => sE
             });
             var i = n(3379),
                 r = n.n(i),
                 s = n(4272);
             r()(s.Z, {
                 insert: "head",
                 singleton: !1
@@ -10657,17 +10657,18 @@
             }
 
             function dd(t) {
                 const {
                     luma: e
                 } = t;
                 if (t.canvas && e) {
-                    const n = e.canvasSizeInfo,
-                        i = "clientWidth" in n ? n.clientWidth : t.canvas.clientWidth;
-                    return i ? t.drawingBufferWidth / i : 1
+                    const {
+                        clientWidth: n
+                    } = e.canvasSizeInfo;
+                    return n ? t.drawingBufferWidth / n : 1
                 }
                 return 1
             }
 
             function pd(t, e) {
                 let n = !(arguments.length > 2 && void 0 !== arguments[2]) || arguments[2];
                 return function(t, e, n, i, r) {
@@ -10783,99 +10784,100 @@
                     copyState: !1,
                     log: function() {
                         for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
                         return Tu.log(1, ...e)()
                     }
                 }), md && i && (globalThis.makeDebugContext ? (t = globalThis.makeDebugContext(t, e), Tu.level = Math.max(Tu.level, 1)) : Tu.warn('WebGL debug mode not activated. import "@luma.gl/debug" to enable.')()), t._instrumented = !0, t
             }
-            const xd = "8.5.20",
-                wd = new class {
-                    constructor() {
-                        this.stats = new Map
-                    }
-                    get(t) {
-                        return this.stats.has(t) || this.stats.set(t, new da({
-                            id: t
-                        })), this.stats.get(t)
-                    }
-                };
+            const xd = "8.5.16";
+            class wd {
+                constructor() {
+                    this.stats = new Map
+                }
+                get(t) {
+                    return this.stats.has(t) || this.stats.set(t, new da({
+                        id: t
+                    })), this.stats.get(t)
+                }
+            }
+            const Ed = new wd;
             if (globalThis.luma && globalThis.luma.VERSION !== xd) throw new Error("luma.gl - multiple VERSIONs detected: ".concat(globalThis.luma.VERSION, " vs ").concat(xd));
 
-            function Ed(t, e) {
+            function Pd(t, e) {
                 if (!t) throw new Error(e || "luma.gl: assertion failed.")
             }
 
-            function Pd(t, e) {
+            function Sd(t, e) {
                 if ("string" != typeof e) return e;
                 const n = Number(e);
                 if (!isNaN(n)) return n;
                 const i = t[e = e.replace(/^.*\./, "")];
-                return Ed(void 0 !== i, "Accessing undefined constant GL.".concat(e)), i
+                return Pd(void 0 !== i, "Accessing undefined constant GL.".concat(e)), i
             }
 
-            function Sd(t, e) {
+            function Cd(t, e) {
                 e = Number(e);
                 for (const n in t)
                     if (t[n] === e) return "GL.".concat(n);
                 return String(e)
             }
             globalThis.luma || (jo() && Tu.log(1, "luma.gl ".concat(xd, " - ").concat("set luma.log.level=1 (or higher) to trace rendering"))(), globalThis.luma = globalThis.luma || {
                 VERSION: xd,
                 version: xd,
                 log: Tu,
-                stats: wd,
+                stats: Ed,
                 globals: {
                     modules: {},
                     nodeIO: {}
                 }
             }), globalThis.luma;
-            const Cd = {};
+            const Td = {};
 
-            function Td() {
+            function Ad() {
                 let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : "id";
-                Cd[t] = Cd[t] || 1;
-                const e = Cd[t]++;
+                Td[t] = Td[t] || 1;
+                const e = Td[t]++;
                 return "".concat(t, "-").concat(e)
             }
 
-            function Ad(t) {
-                return Ed("number" == typeof t, "Input must be a number"), t && 0 == (t & t - 1)
+            function Md(t) {
+                return Pd("number" == typeof t, "Input must be a number"), t && 0 == (t & t - 1)
             }
 
-            function Md(t) {
+            function Od(t) {
                 let e = !0;
                 for (const n in t) {
                     e = !1;
                     break
                 }
                 return e
             }
 
-            function Od(t, e, n, i) {
+            function Ld(t, e, n, i) {
                 const r = "See luma.gl ".concat(n, " Upgrade Guide at https://luma.gl/docs/upgrade-guide"),
                     s = Object.getPrototypeOf(t);
                 i.forEach((t => {
                     s.methodName || (s[t] = () => {
                         throw Tu.removed("Calling removed method ".concat(e, ".").concat(t, ": "), r)(), new Error(t)
                     })
                 }))
             }
-            const Ld = "Resource subclass must define virtual methods";
-            class Rd {
+            const Rd = "Resource subclass must define virtual methods";
+            class Id {
                 get[Symbol.toStringTag]() {
                     return "Resource"
                 }
                 constructor(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                     Ru(t);
                     const {
                         id: n,
                         userData: i = {}
                     } = e;
-                    this.gl = t, this.gl2 = t, this.id = n || Td(this[Symbol.toStringTag]), this.userData = i, this._bound = !1, this._handle = e.handle, void 0 === this._handle && (this._handle = this._createHandle()), this.byteLength = 0, this._addStats()
+                    this.gl = t, this.gl2 = t, this.id = n || Ad(this[Symbol.toStringTag]), this.userData = i, this._bound = !1, this._handle = e.handle, void 0 === this._handle && (this._handle = this._createHandle()), this.byteLength = 0, this._initStats(), this._addStats()
                 }
                 toString() {
                     return "".concat(this[Symbol.toStringTag] || this.constructor.name, "(").concat(this.id, ")")
                 }
                 get handle() {
                     return this._handle
                 }
@@ -10891,15 +10893,15 @@
                     return "function" != typeof e ? (this._bindHandle(e), this) : (this._bound ? t = e() : (this._bindHandle(this.handle), this._bound = !0, t = e(), this._bound = !1, this._bindHandle(null)), t)
                 }
                 unbind() {
                     this.bind(null)
                 }
                 getParameter(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
-                    Ed(t = Pd(this.gl, t));
+                    Pd(t = Sd(this.gl, t));
                     const n = (this.constructor.PARAMETERS || {})[t];
                     if (n) {
                         const t = Lu(this.gl);
                         if ("webgl2" in n && !t || "extension" in n && !this.gl.getExtension(n.extension)) {
                             const e = n.webgl1,
                                 i = "webgl2" in n ? n.webgl2 : n.webgl1;
                             return t ? i : e
@@ -10912,92 +10914,93 @@
                     const {
                         parameters: e,
                         keys: n
                     } = t, i = this.constructor.PARAMETERS || {}, r = Lu(this.gl), s = {}, o = e || Object.keys(i);
                     for (const e of o) {
                         const o = i[e];
                         if (o && (!("webgl2" in o) || r) && (!("extension" in o) || this.gl.getExtension(o.extension))) {
-                            const i = n ? Sd(this.gl, e) : e;
-                            s[i] = this.getParameter(e, t), n && "GLenum" === o.type && (s[i] = Sd(this.gl, s[i]))
+                            const i = n ? Cd(this.gl, e) : e;
+                            s[i] = this.getParameter(e, t), n && "GLenum" === o.type && (s[i] = Cd(this.gl, s[i]))
                         }
                     }
                     return s
                 }
                 setParameter(t, e) {
-                    Ed(t = Pd(this.gl, t));
+                    Pd(t = Sd(this.gl, t));
                     const n = (this.constructor.PARAMETERS || {})[t];
                     if (n) {
                         const t = Lu(this.gl);
                         if ("webgl2" in n && !t || "extension" in n && !this.gl.getExtension(n.extension)) throw new Error("Parameter not available on this platform");
-                        "GLenum" === n.type && (e = Pd(e))
+                        "GLenum" === n.type && (e = Sd(e))
                     }
                     return this._setParameter(t, e), this
                 }
                 setParameters(t) {
                     for (const e in t) this.setParameter(e, t[e]);
                     return this
                 }
                 stubRemovedMethods(t, e, n) {
-                    return Od(this, t, e, n)
+                    return Ld(this, t, e, n)
                 }
                 initialize(t) {}
                 _createHandle() {
-                    throw new Error(Ld)
+                    throw new Error(Rd)
                 }
                 _deleteHandle() {
-                    throw new Error(Ld)
+                    throw new Error(Rd)
                 }
                 _bindHandle(t) {
-                    throw new Error(Ld)
+                    throw new Error(Rd)
                 }
                 _getOptsFromHandle() {
-                    throw new Error(Ld)
+                    throw new Error(Rd)
                 }
                 _getParameter(t, e) {
-                    throw new Error(Ld)
+                    throw new Error(Rd)
                 }
                 _setParameter(t, e) {
-                    throw new Error(Ld)
+                    throw new Error(Rd)
                 }
                 _context() {
                     return this.gl.luma = this.gl.luma || {}, this.gl.luma
                 }
+                _initStats() {
+                    this.gl.stats = this.gl.stats || new wd
+                }
                 _addStats() {
                     const t = this[Symbol.toStringTag],
-                        e = wd.get("Resource Counts");
+                        e = Ed.get("Resource Counts");
                     e.get("Resources Created").incrementCount(), e.get("".concat(t, "s Created")).incrementCount(), e.get("".concat(t, "s Active")).incrementCount()
                 }
                 _removeStats() {
                     const t = this[Symbol.toStringTag];
-                    wd.get("Resource Counts").get("".concat(t, "s Active")).decrementCount()
+                    Ed.get("Resource Counts").get("".concat(t, "s Active")).decrementCount()
                 }
                 _trackAllocatedMemory(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this[Symbol.toStringTag];
-                    this._trackAllocatedMemoryForContext(t, e), this._trackAllocatedMemoryForContext(t, e, this.gl.canvas && this.gl.canvas.id), this.byteLength = t
+                    this._doTrackAllocatedMemory(t, e), this._doTrackAllocatedMemory(t, e, this.gl.stats.get("Memory Usage"))
                 }
-                _trackAllocatedMemoryForContext(t) {
+                _doTrackAllocatedMemory(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this[Symbol.toStringTag],
-                        n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : "";
-                    const i = wd.get("Memory Usage".concat(n));
-                    i.get("GPU Memory").addCount(t), i.get("".concat(e, " Memory")).addCount(t)
+                        n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : Ed.get("Memory Usage");
+                    n.get("GPU Memory").addCount(t), n.get("".concat(e, " Memory")).addCount(t), this.byteLength = t
                 }
                 _trackDeallocatedMemory() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : this[Symbol.toStringTag];
-                    this._trackDeallocatedMemoryForContext(t), this._trackDeallocatedMemoryForContext(t, this.gl.canvas && this.gl.canvas.id), this.byteLength = 0
+                    this._doTrackDeallocatedMemory(t), this._doTrackDeallocatedMemory(t, this.gl.stats.get("Memory Usage"))
                 }
-                _trackDeallocatedMemoryForContext() {
+                _doTrackDeallocatedMemory() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : this[Symbol.toStringTag],
-                        e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "";
-                    const n = wd.get("Memory Usage".concat(e));
-                    n.get("GPU Memory").subtractCount(this.byteLength), n.get("".concat(t, " Memory")).subtractCount(this.byteLength)
+                        e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : Ed.get("Memory Usage");
+                    e.get("GPU Memory").subtractCount(this.byteLength), e.get("".concat(t, " Memory")).subtractCount(this.byteLength), this.byteLength = 0
                 }
             }
-            const Id = "Failed to deduce GL constant from typed array";
+            const kd = "Failed to deduce GL constant from typed array";
 
-            function kd(t) {
+            function jd(t) {
                 switch (ArrayBuffer.isView(t) ? t.constructor : t) {
                     case Float32Array:
                         return 5126;
                     case Uint16Array:
                         return 5123;
                     case Uint32Array:
                         return 5125;
@@ -11007,19 +11010,19 @@
                     case Int8Array:
                         return 5120;
                     case Int16Array:
                         return 5122;
                     case Int32Array:
                         return 5124;
                     default:
-                        throw new Error(Id)
+                        throw new Error(kd)
                 }
             }
 
-            function jd(t) {
+            function Fd(t) {
                 let {
                     clamped: e = !0
                 } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                 switch (t) {
                     case 5126:
                         return Float32Array;
                     case 5123:
@@ -11038,15 +11041,15 @@
                     case 5124:
                         return Int32Array;
                     default:
                         throw new Error("Failed to deduce typed array type from GL constant")
                 }
             }
 
-            function Fd(t) {
+            function zd(t) {
                 let {
                     data: e,
                     width: n,
                     height: i
                 } = t;
                 const r = Math.round(n / 2),
                     s = Math.round(i / 2),
@@ -11057,15 +11060,15 @@
                 return {
                     data: o,
                     width: r,
                     height: s
                 }
             }
 
-            function zd(t, e, n) {
+            function Bd(t, e, n) {
                 const {
                     removedProps: i = {},
                     deprecatedProps: r = {},
                     replacedProps: s = {}
                 } = n;
                 for (const n in i)
                     if (n in e) {
@@ -11078,108 +11081,108 @@
                     } let o = null;
                 for (const n in s)
                     if (n in e) {
                         const i = s[n];
                         Tu.deprecated("".concat(t, ".").concat(n), "".concat(t, ".").concat(i))(), o = o || Object.assign({}, e), o[i] = e[n], delete o[n]
                     } return o || e
             }
-            const Bd = {
+            const Dd = {
                     offset: 0,
                     stride: 0,
                     type: 5126,
                     size: 1,
                     divisor: 0,
                     normalized: !1,
                     integer: !1
                 },
-                Dd = {
+                Nd = {
                     deprecatedProps: {
                         instanced: "divisor",
                         isInstanced: "divisor"
                     }
                 };
-            class Nd {
+            class Vd {
                 static getBytesPerElement(t) {
-                    return jd(t.type || 5126).BYTES_PER_ELEMENT
+                    return Fd(t.type || 5126).BYTES_PER_ELEMENT
                 }
                 static getBytesPerVertex(t) {
-                    return Ed(t.size), jd(t.type || 5126).BYTES_PER_ELEMENT * t.size
+                    return Pd(t.size), Fd(t.type || 5126).BYTES_PER_ELEMENT * t.size
                 }
                 static resolve() {
                     for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
-                    return new Nd(...[Bd, ...e])
+                    return new Vd(...[Dd, ...e])
                 }
                 constructor() {
                     for (var t = arguments.length, e = new Array(t), n = 0; n < t; n++) e[n] = arguments[n];
                     e.forEach((t => this._assign(t))), Object.freeze(this)
                 }
                 toString() {
                     return JSON.stringify(this)
                 }
                 get BYTES_PER_ELEMENT() {
-                    return Nd.getBytesPerElement(this)
+                    return Vd.getBytesPerElement(this)
                 }
                 get BYTES_PER_VERTEX() {
-                    return Nd.getBytesPerVertex(this)
+                    return Vd.getBytesPerVertex(this)
                 }
                 _assign() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
-                    return t = zd("Accessor", t, Dd), void 0 !== t.type && (this.type = t.type, 5124 !== t.type && 5125 !== t.type || (this.integer = !0)), void 0 !== t.size && (this.size = t.size), void 0 !== t.offset && (this.offset = t.offset), void 0 !== t.stride && (this.stride = t.stride), void 0 !== t.normalized && (this.normalized = t.normalized), void 0 !== t.integer && (this.integer = t.integer), void 0 !== t.divisor && (this.divisor = t.divisor), void 0 !== t.buffer && (this.buffer = t.buffer), void 0 !== t.index && ("boolean" == typeof t.index ? this.index = t.index ? 1 : 0 : this.index = t.index), void 0 !== t.instanced && (this.divisor = t.instanced ? 1 : 0), void 0 !== t.isInstanced && (this.divisor = t.isInstanced ? 1 : 0), this
+                    return t = Bd("Accessor", t, Nd), void 0 !== t.type && (this.type = t.type, 5124 !== t.type && 5125 !== t.type || (this.integer = !0)), void 0 !== t.size && (this.size = t.size), void 0 !== t.offset && (this.offset = t.offset), void 0 !== t.stride && (this.stride = t.stride), void 0 !== t.normalized && (this.normalized = t.normalized), void 0 !== t.integer && (this.integer = t.integer), void 0 !== t.divisor && (this.divisor = t.divisor), void 0 !== t.buffer && (this.buffer = t.buffer), void 0 !== t.index && ("boolean" == typeof t.index ? this.index = t.index ? 1 : 0 : this.index = t.index), void 0 !== t.instanced && (this.divisor = t.instanced ? 1 : 0), void 0 !== t.isInstanced && (this.divisor = t.isInstanced ? 1 : 0), this
                 }
             }
-            const Vd = {
+            const Ud = {
                     offset: "accessor.offset",
                     stride: "accessor.stride",
                     type: "accessor.type",
                     size: "accessor.size",
                     divisor: "accessor.divisor",
                     normalized: "accessor.normalized",
                     integer: "accessor.integer",
                     instanced: "accessor.divisor",
                     isInstanced: "accessor.divisor"
                 },
-                Ud = {
+                Gd = {
                     removedProps: {},
                     replacedProps: {
                         bytes: "byteLength"
                     },
-                    deprecatedProps: Vd
+                    deprecatedProps: Ud
                 },
-                Gd = {
-                    removedProps: Vd
+                Wd = {
+                    removedProps: Ud
                 };
-            class Wd extends Rd {
+            class Hd extends Id {
                 get[Symbol.toStringTag]() {
                     return "Buffer"
                 }
                 constructor(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                     super(t, e), this.stubRemovedMethods("Buffer", "v6.0", ["layout", "setLayout", "getIndexedParameter"]), this.target = e.target || (this.gl.webgl2 ? 36662 : 34962), this.initialize(e), Object.seal(this)
                 }
                 getElementCount() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : this.accessor;
-                    return Math.round(this.byteLength / Nd.getBytesPerElement(t))
+                    return Math.round(this.byteLength / Vd.getBytesPerElement(t))
                 }
                 getVertexCount() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : this.accessor;
-                    return Math.round(this.byteLength / Nd.getBytesPerVertex(t))
+                    return Math.round(this.byteLength / Vd.getBytesPerVertex(t))
                 }
                 initialize() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     return ArrayBuffer.isView(t) && (t = {
                         data: t
                     }), Number.isFinite(t) && (t = {
                         byteLength: t
-                    }), t = zd("Buffer", t, Ud), this.usage = t.usage || 35044, this.debugData = null, this.setAccessor(Object.assign({}, t, t.accessor)), t.data ? this._setData(t.data, t.offset, t.byteLength) : this._setByteLength(t.byteLength || 0), this
+                    }), t = Bd("Buffer", t, Gd), this.usage = t.usage || 35044, this.debugData = null, this.setAccessor(Object.assign({}, t, t.accessor)), t.data ? this._setData(t.data, t.offset, t.byteLength) : this._setByteLength(t.byteLength || 0), this
                 }
                 setProps(t) {
-                    return "accessor" in (t = zd("Buffer", t, Gd)) && this.setAccessor(t.accessor), this
+                    return "accessor" in (t = Bd("Buffer", t, Wd)) && this.setAccessor(t.accessor), this
                 }
                 setAccessor(t) {
-                    return delete(t = Object.assign({}, t)).buffer, this.accessor = new Nd(t), this
+                    return delete(t = Object.assign({}, t)).buffer, this.accessor = new Vd(t), this
                 }
                 reallocate(t) {
                     return t > this.byteLength ? (this._setByteLength(t), !0) : (this.bytesUsed = t, !1)
                 }
                 setData(t) {
                     return this.initialize(t)
                 }
@@ -11188,15 +11191,15 @@
                         data: t
                     });
                     const {
                         data: e,
                         offset: n = 0,
                         srcOffset: i = 0
                     } = t, r = t.byteLength || t.length;
-                    Ed(e);
+                    Pd(e);
                     const s = this.gl.webgl2 ? 36663 : this.target;
                     return this.gl.bindBuffer(s, this.handle), 0 !== i || void 0 !== r ? (Iu(this.gl), this.gl.bufferSubData(this.target, n, e, i, r)) : this.gl.bufferSubData(s, n, e), this.gl.bindBuffer(s, null), this.debugData = null, this._inferType(e), this
                 }
                 copyData(t) {
                     let {
                         sourceBuffer: e,
                         readOffset: n = 0,
@@ -11212,32 +11215,32 @@
                     let {
                         dstData: t = null,
                         srcByteOffset: e = 0,
                         dstOffset: n = 0,
                         length: i = 0
                     } = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     Iu(this.gl);
-                    const r = jd(this.accessor.type || 5126, {
+                    const r = Fd(this.accessor.type || 5126, {
                             clamped: !1
                         }),
                         s = this._getAvailableElementCount(e),
                         o = n;
                     let a, l;
                     t ? (l = t.length, a = l - o) : (a = Math.min(s, i || s), l = o + a);
                     const c = Math.min(s, a);
-                    return i = i || c, Ed(i <= c), t = t || new r(l), this.gl.bindBuffer(36662, this.handle), this.gl.getBufferSubData(36662, e, t, n, i), this.gl.bindBuffer(36662, null), t
+                    return i = i || c, Pd(i <= c), t = t || new r(l), this.gl.bindBuffer(36662, this.handle), this.gl.getBufferSubData(36662, e, t, n, i), this.gl.bindBuffer(36662, null), t
                 }
                 bind() {
                     let {
                         target: t = this.target,
                         index: e = this.accessor && this.accessor.index,
                         offset: n = 0,
                         size: i
                     } = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
-                    return 35345 === t || 35982 === t ? void 0 !== i ? this.gl.bindBufferRange(t, e, this.handle, n, i) : (Ed(0 === n), this.gl.bindBufferBase(t, e, this.handle)) : this.gl.bindBuffer(t, this.handle), this
+                    return 35345 === t || 35982 === t ? void 0 !== i ? this.gl.bindBufferRange(t, e, this.handle, n, i) : (Pd(0 === n), this.gl.bindBufferBase(t, e, this.handle)) : this.gl.bindBuffer(t, this.handle), this
                 }
                 unbind() {
                     let {
                         target: t = this.target,
                         index: e = this.accessor && this.accessor.index
                     } = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     return 35345 === t || 35982 === t ? this.gl.bindBufferBase(t, e, null) : this.gl.bindBuffer(t, null), this
@@ -11255,42 +11258,42 @@
                 }
                 invalidateDebugData() {
                     this.debugData = null
                 }
                 _setData(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 0,
                         n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : t.byteLength + e;
-                    Ed(ArrayBuffer.isView(t)), this._trackDeallocatedMemory();
+                    Pd(ArrayBuffer.isView(t)), this._trackDeallocatedMemory();
                     const i = this._getTarget();
                     this.gl.bindBuffer(i, this.handle), this.gl.bufferData(i, n, this.usage), this.gl.bufferSubData(i, e, t), this.gl.bindBuffer(i, null), this.debugData = t.slice(0, 10), this.bytesUsed = n, this._trackAllocatedMemory(n);
-                    const r = kd(t);
-                    return Ed(r), this.setAccessor(new Nd(this.accessor, {
+                    const r = jd(t);
+                    return Pd(r), this.setAccessor(new Vd(this.accessor, {
                         type: r
                     })), this
                 }
                 _setByteLength(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : this.usage;
-                    Ed(t >= 0), this._trackDeallocatedMemory();
+                    Pd(t >= 0), this._trackDeallocatedMemory();
                     let n = t;
                     0 === t && (n = new Float32Array(0));
                     const i = this._getTarget();
                     return this.gl.bindBuffer(i, this.handle), this.gl.bufferData(i, n, e), this.gl.bindBuffer(i, null), this.usage = e, this.debugData = null, this.bytesUsed = t, this._trackAllocatedMemory(t), this
                 }
                 _getTarget() {
                     return this.gl.webgl2 ? 36663 : this.target
                 }
                 _getAvailableElementCount(t) {
-                    const e = t / jd(this.accessor.type || 5126, {
+                    const e = t / Fd(this.accessor.type || 5126, {
                         clamped: !1
                     }).BYTES_PER_ELEMENT;
                     return this.getElementCount() - e
                 }
                 _inferType(t) {
-                    this.accessor.type || this.setAccessor(new Nd(this.accessor, {
-                        type: kd(t)
+                    this.accessor.type || this.setAccessor(new Vd(this.accessor, {
+                        type: jd(t)
                     }))
                 }
                 _createHandle() {
                     return this.gl.createBuffer()
                 }
                 _deleteHandle() {
                     this.gl.deleteBuffer(this.handle), this._trackDeallocatedMemory()
@@ -11306,18 +11309,18 @@
                 get bytes() {
                     return Tu.deprecated("Buffer.bytes", "Buffer.byteLength")(), this.byteLength
                 }
                 setByteLength(t) {
                     return Tu.deprecated("setByteLength", "reallocate")(), this.reallocate(t)
                 }
                 updateAccessor(t) {
-                    return Tu.deprecated("updateAccessor(...)", "setAccessor(new Accessor(buffer.accessor, ...)")(), this.accessor = new Nd(this.accessor, t), this
+                    return Tu.deprecated("updateAccessor(...)", "setAccessor(new Accessor(buffer.accessor, ...)")(), this.accessor = new Vd(this.accessor, t), this
                 }
             }
-            const Hd = {
+            const Zd = {
                     6407: {
                         dataFormat: 6407,
                         types: [5121, 33635]
                     },
                     6408: {
                         dataFormat: 6408,
                         types: [5121, 32819, 32820]
@@ -11351,73 +11354,73 @@
                     },
                     34836: {
                         dataFormat: 6408,
                         types: [5126],
                         gl2: !0
                     }
                 },
-                Zd = {
+                qd = {
                     6403: 1,
                     36244: 1,
                     33319: 2,
                     33320: 2,
                     6407: 3,
                     36248: 3,
                     6408: 4,
                     36249: 4,
                     6402: 1,
                     34041: 1,
                     6406: 1,
                     6409: 1,
                     6410: 2
                 },
-                qd = {
+                Xd = {
                     5126: 4,
                     5125: 4,
                     5124: 4,
                     5123: 2,
                     5122: 2,
                     5131: 2,
                     5120: 1,
                     5121: 1
                 },
-                Xd = [9729, 9728],
-                Yd = globalThis.WebGLBuffer || function() {};
-            class Kd extends Rd {
+                Yd = [9729, 9728],
+                Kd = globalThis.WebGLBuffer || function() {};
+            class Qd extends Id {
                 get[Symbol.toStringTag]() {
                     return "Texture"
                 }
                 static isSupported(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                     const {
                         format: n,
                         linearFiltering: i
                     } = e;
                     let r = !0;
                     return n && (r = r && function(t, e) {
-                        const n = Hd[e];
+                        const n = Zd[e];
                         if (!n) return !1;
                         if (void 0 === n.gl1 && void 0 === n.gl2) return !0;
                         const i = Lu(t) && n.gl2 || n.gl1;
                         return "string" == typeof i ? t.getExtension(i) : i
                     }(t, n), r = r && (!i || function(t, e) {
-                        const n = Hd[e];
+                        const n = Zd[e];
                         switch (n && n.types[0]) {
                             case 5126:
                                 return t.getExtension("OES_texture_float_linear");
                             case 5131:
                                 return t.getExtension("OES_texture_half_float_linear");
                             default:
                                 return !0
                         }
                     }(t, n))), r
                 }
                 constructor(t, e) {
                     const {
-                        id: n = Td("texture"),
+                        id: n = Ad("texture"),
                         handle: i,
                         target: r
                     } = e;
                     super(t, {
                         id: n,
                         handle: i
                     }), this.target = r, this.textureUnit = void 0, this.loaded = !1, this.width = void 0, this.height = void 0, this.depth = void 0, this.format = void 0, this.type = void 0, this.dataFormat = void 0, this.border = void 0, this.textureUnit = void 0, this.mipmaps = void 0
@@ -11584,21 +11587,21 @@
                                 case "browser-object":
                                     Lu(f) ? f.texImage2D(e, i, r, h, u, s, d, c, l) : f.texImage2D(e, i, r, d, c, l);
                                     break;
                                 case "compressed":
                                     for (const [t, n] of l.entries()) f.compressedTexImage2D(e, t, n.format, n.width, n.height, s, n.data), v += n.levelSize;
                                     break;
                                 default:
-                                    Ed(!1, "Unknown image data type")
+                                    Pd(!1, "Unknown image data type")
                             }
                         })), "compressed" === m) this._trackAllocatedMemory(v, "Texture");
                     else if (l && l.byteLength) this._trackAllocatedMemory(l.byteLength, "Texture");
                     else {
-                        const t = Zd[this.dataFormat] || 4,
-                            e = qd[this.type] || 1;
+                        const t = qd[this.dataFormat] || 4,
+                            e = Xd[this.type] || 1;
                         this._trackAllocatedMemory(this.width * this.height * t * e, "Texture")
                     }
                     return this.loaded = !0, this
                 }
                 setSubImageData(t) {
                     let {
                         target: e = this.target,
@@ -11627,23 +11630,23 @@
                             format: c,
                             type: h,
                             dataFormat: u,
                             compressed: d,
                             data: i,
                             width: o,
                             height: a
-                        })), Ed(0 === this.depth, "texSubImage not supported for 3D textures"), i || (i = n), i && i.data) {
+                        })), Pd(0 === this.depth, "texSubImage not supported for 3D textures"), i || (i = n), i && i.data) {
                         const t = i;
                         i = t.data, o = t.shape[0], a = t.shape[1]
                     }
-                    i instanceof Wd && (i = i.handle), this.gl.bindTexture(this.target, this.handle), ud(this.gl, g, (() => {
+                    i instanceof Hd && (i = i.handle), this.gl.bindTexture(this.target, this.handle), ud(this.gl, g, (() => {
                         if (d) this.gl.compressedTexSubImage2D(e, l, r, s, o, a, c, i);
                         else if (null === i) this.gl.texSubImage2D(e, l, r, s, o, a, u, h, null);
                         else if (ArrayBuffer.isView(i)) this.gl.texSubImage2D(e, l, r, s, o, a, u, h, i, p);
-                        else if (i instanceof Yd) {
+                        else if (i instanceof Kd) {
                             const t = Iu(this.gl);
                             t.bindBuffer(35052, i), t.texSubImage2D(e, l, r, s, o, a, u, h, p), t.bindBuffer(35052, null)
                         } else Lu(this.gl) ? Iu(this.gl).texSubImage2D(e, l, r, s, o, a, u, h, i) : this.gl.texSubImage2D(e, l, r, s, u, h, i)
                     })), this.gl.bindTexture(this.target, null)
                 }
                 copyFramebuffer() {
                     return Tu.error("Texture.copyFramebuffer({...}) is no logner supported, use copyToTexture(source, target, opts})")(), null
@@ -11675,18 +11678,18 @@
                         dataType: "compressed"
                     } : null === e ? {
                         data: e,
                         dataType: "null"
                     } : ArrayBuffer.isView(e) ? {
                         data: e,
                         dataType: "typed-array"
-                    } : e instanceof Wd ? {
+                    } : e instanceof Hd ? {
                         data: e.handle,
                         dataType: "buffer"
-                    } : e instanceof Yd ? {
+                    } : e instanceof Kd ? {
                         data: e,
                         dataType: "buffer"
                     } : {
                         data: e,
                         dataType: "browser-object"
                     }
                 }
@@ -11698,15 +11701,15 @@
                     let {
                         width: i,
                         height: r,
                         dataFormat: s,
                         type: o,
                         compressed: a
                     } = t;
-                    const l = Hd[e];
+                    const l = Zd[e];
                     return s = s || l && l.dataFormat, o = o || l && l.types[0], a = a || l && l.compressed, ({
                         width: i,
                         height: r
                     } = this._deduceImageSize(n, i, r)), {
                         dataFormat: s,
                         type: o,
                         compressed: a,
@@ -11732,15 +11735,15 @@
                         height: t.videoHeight
                     } : t ? {
                         width: e,
                         height: n
                     } : {
                         width: e >= 0 ? e : 1,
                         height: n >= 0 ? n : 1
-                    }, Ed(i, "Could not deduced texture size"), Ed(void 0 === e || i.width === e, "Deduced texture width does not match supplied width"), Ed(void 0 === n || i.height === n, "Deduced texture height does not match supplied height"), i
+                    }, Pd(i, "Could not deduced texture size"), Pd(void 0 === e || i.width === e, "Deduced texture width does not match supplied width"), Pd(void 0 === n || i.height === n, "Deduced texture height does not match supplied height"), i
                 }
                 _createHandle() {
                     return this.gl.createTexture()
                 }
                 _deleteHandle() {
                     this.gl.deleteTexture(this.handle), this._trackDeallocatedMemory("Texture")
                 }
@@ -11760,67 +11763,67 @@
                     switch (this.gl.bindTexture(this.target, this.handle), e = this._getNPOTParam(t, e), t) {
                         case 33082:
                         case 33083:
                             this.gl.texParameterf(this.handle, t, e);
                             break;
                         case 4096:
                         case 4097:
-                            Ed(!1);
+                            Pd(!1);
                             break;
                         default:
                             this.gl.texParameteri(this.target, t, e)
                     }
                     return this.gl.bindTexture(this.target, null), this
                 }
                 _isNPOT() {
-                    return !(Lu(this.gl) || !this.width || !this.height || Ad(this.width) && Ad(this.height))
+                    return !(Lu(this.gl) || !this.width || !this.height || Md(this.width) && Md(this.height))
                 }
                 _updateForNPOT(t) {
                     void 0 === t[this.gl.TEXTURE_MIN_FILTER] && (t[this.gl.TEXTURE_MIN_FILTER] = this.gl.LINEAR), void 0 === t[this.gl.TEXTURE_WRAP_S] && (t[this.gl.TEXTURE_WRAP_S] = this.gl.CLAMP_TO_EDGE), void 0 === t[this.gl.TEXTURE_WRAP_T] && (t[this.gl.TEXTURE_WRAP_T] = this.gl.CLAMP_TO_EDGE)
                 }
                 _getNPOTParam(t, e) {
                     if (this._isNPOT()) switch (t) {
                         case 10241:
-                            -1 === Xd.indexOf(e) && (e = 9729);
+                            -1 === Yd.indexOf(e) && (e = 9729);
                             break;
                         case 10242:
                         case 10243:
                             33071 !== e && (e = 33071)
                     }
                     return e
                 }
             }
-            class Qd extends Kd {
+            class Jd extends Qd {
                 get[Symbol.toStringTag]() {
                     return "Texture2D"
                 }
                 static isSupported(t, e) {
-                    return Kd.isSupported(t, e)
+                    return Qd.isSupported(t, e)
                 }
                 constructor(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                     var n;
                     Ru(t), (e instanceof Promise || "string" == typeof e) && (e = {
                         data: e
                     }), "string" == typeof e.data && (e = Object.assign({}, e, {
-                        data: (n = e.data, Ed("string" == typeof n), n = "" + n, new Promise(((t, e) => {
+                        data: (n = e.data, Pd("string" == typeof n), n = "" + n, new Promise(((t, e) => {
                             try {
                                 const i = new Image;
                                 i.onload = () => t(i), i.onerror = () => e(new Error("Could not load image ".concat(n, "."))), i.crossOrigin = "anonymous", i.src = n
                             } catch (t) {
                                 e(t)
                             }
                         })))
                     })), super(t, Object.assign({}, e, {
                         target: 3553
                     })), this.initialize(e), Object.seal(this)
                 }
             }
-            const Jd = "EXT_color_buffer_float",
-                $d = {
+            const $d = "EXT_color_buffer_float",
+                tp = {
                     33189: {
                         bpp: 2
                     },
                     33190: {
                         gl2: !0,
                         bpp: 3
                     },
@@ -11944,58 +11947,58 @@
                         bpp: 16
                     },
                     36208: {
                         gl2: !0,
                         bpp: 16
                     },
                     33325: {
-                        gl2: Jd,
+                        gl2: $d,
                         bpp: 2
                     },
                     33327: {
-                        gl2: Jd,
+                        gl2: $d,
                         bpp: 4
                     },
                     34842: {
-                        gl2: Jd,
+                        gl2: $d,
                         bpp: 8
                     },
                     33326: {
-                        gl2: Jd,
+                        gl2: $d,
                         bpp: 4
                     },
                     33328: {
-                        gl2: Jd,
+                        gl2: $d,
                         bpp: 8
                     },
                     34836: {
-                        gl2: Jd,
+                        gl2: $d,
                         bpp: 16
                     },
                     35898: {
-                        gl2: Jd,
+                        gl2: $d,
                         bpp: 4
                     }
                 };
-            class tp extends Rd {
+            class ep extends Id {
                 get[Symbol.toStringTag]() {
                     return "Renderbuffer"
                 }
                 static isSupported(t) {
                     let {
                         format: e
                     } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {
                         format: null
                     };
                     return !e || function(t, e, n) {
                         const i = n[e];
                         if (!i) return !1;
                         const r = Lu(t) && i.gl2 || i.gl1;
                         return "string" == typeof r ? t.getExtension(r) : r
-                    }(t, e, $d)
+                    }(t, e, tp)
                 }
                 static getSamplesForFormat(t, e) {
                     let {
                         format: n
                     } = e;
                     return t.getInternalformatParameter(36161, n, 32937)
                 }
@@ -12006,15 +12009,15 @@
                 initialize(t) {
                     let {
                         format: e,
                         width: n = 1,
                         height: i = 1,
                         samples: r = 0
                     } = t;
-                    return Ed(e, "Needs format"), this._trackDeallocatedMemory(), this.gl.bindRenderbuffer(36161, this.handle), 0 !== r && Lu(this.gl) ? this.gl.renderbufferStorageMultisample(36161, r, e, n, i) : this.gl.renderbufferStorage(36161, e, n, i), this.format = e, this.width = n, this.height = i, this.samples = r, this._trackAllocatedMemory(this.width * this.height * (this.samples || 1) * $d[this.format].bpp), this
+                    return Pd(e, "Needs format"), this._trackDeallocatedMemory(), this.gl.bindRenderbuffer(36161, this.handle), 0 !== r && Lu(this.gl) ? this.gl.renderbufferStorageMultisample(36161, r, e, n, i) : this.gl.renderbufferStorage(36161, e, n, i), this.format = e, this.width = n, this.height = i, this.samples = r, this._trackAllocatedMemory(this.width * this.height * (this.samples || 1) * tp[this.format].bpp), this
                 }
                 resize(t) {
                     let {
                         width: e,
                         height: n
                     } = t;
                     return e !== this.width || n !== this.height ? this.initialize({
@@ -12036,33 +12039,33 @@
                 _syncHandle(t) {
                     this.format = this.getParameter(36164), this.width = this.getParameter(36162), this.height = this.getParameter(36163), this.samples = this.getParameter(36011)
                 }
                 _getParameter(t) {
                     return this.gl.bindRenderbuffer(36161, this.handle), this.gl.getRenderbufferParameter(36161, t)
                 }
             }
-            const ep = 6144,
-                np = "clear: bad arguments";
+            const np = 6144,
+                ip = "clear: bad arguments";
 
-            function ip(t) {
+            function rp(t) {
                 let {
                     framebuffer: e = null,
                     color: n = null,
                     depth: i = null,
                     stencil: r = null
                 } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                 const s = {};
                 e && (s.framebuffer = e);
                 let o = 0;
-                n && (o |= 16384, !0 !== n && (s.clearColor = n)), i && (o |= 256, !0 !== i && (s.clearDepth = i)), r && (o |= 1024, !0 !== i && (s.clearStencil = i)), Ed(0 !== o, np), ud(t, s, (() => {
+                n && (o |= 16384, !0 !== n && (s.clearColor = n)), i && (o |= 256, !0 !== i && (s.clearDepth = i)), r && (o |= 1024, !0 !== i && (s.clearStencil = i)), Pd(0 !== o, ip), ud(t, s, (() => {
                     t.clear(o)
                 }))
             }
-            const rp = [34069, 34070, 34071, 34072, 34073, 34074];
-            class sp extends Kd {
+            const sp = [34069, 34070, 34071, 34072, 34073, 34074];
+            class op extends Qd {
                 get[Symbol.toStringTag]() {
                     return "TextureCube"
                 }
                 constructor(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                     Ru(t), super(t, Object.assign({}, e, {
                         target: 34067
@@ -12102,19 +12105,19 @@
                         data: r,
                         border: s = 0,
                         format: o = 6408,
                         type: a = 5121
                     } = t;
                     const {
                         gl: l
-                    } = this, c = i || r, h = await Promise.all(rp.map((t => {
+                    } = this, c = i || r, h = await Promise.all(sp.map((t => {
                         const e = c[t];
                         return Promise.all(Array.isArray(e) ? e : [e])
                     })));
-                    this.bind(), rp.forEach(((t, i) => {
+                    this.bind(), sp.forEach(((t, i) => {
                         h[i].length > 1 && !1 !== this.opts.mipmaps && Tu.warn("".concat(this.id, " has mipmap and multiple LODs."))(), h[i].forEach(((i, r) => {
                             e && n ? l.texImage2D(t, r, o, e, n, s, o, a, i) : l.texImage2D(t, r, o, o, a, i)
                         }))
                     })), this.unbind()
                 }
                 setImageDataForFace(t) {
                     const {
@@ -12132,16 +12135,16 @@
                     return this.bind(), h instanceof Promise ? h.then((n => this.setImageDataForFace(Object.assign({}, t, {
                         face: e,
                         data: n,
                         pixels: n
                     })))) : this.width || this.height ? c.texImage2D(e, 0, a, n, i, o, a, l, h) : c.texImage2D(e, 0, a, a, l, h), this
                 }
             }
-            sp.FACES = rp;
-            class op extends Kd {
+            op.FACES = sp;
+            class ap extends Qd {
                 get[Symbol.toStringTag]() {
                     return "Texture3D"
                 }
                 static isSupported(t) {
                     return Lu(t)
                 }
                 constructor(t) {
@@ -12164,43 +12167,43 @@
                         format: a,
                         type: l = 5121,
                         offset: c = 0,
                         data: h,
                         parameters: u = {}
                     } = t;
                     if (this._trackDeallocatedMemory("Texture"), this.gl.bindTexture(this.target, this.handle), ud(this.gl, u, (() => {
-                            ArrayBuffer.isView(h) && this.gl.texImage3D(this.target, e, n, i, r, s, o, a, l, h), h instanceof Wd && (this.gl.bindBuffer(35052, h.handle), this.gl.texImage3D(this.target, e, n, i, r, s, o, a, l, c))
+                            ArrayBuffer.isView(h) && this.gl.texImage3D(this.target, e, n, i, r, s, o, a, l, h), h instanceof Hd && (this.gl.bindBuffer(35052, h.handle), this.gl.texImage3D(this.target, e, n, i, r, s, o, a, l, c))
                         })), h && h.byteLength) this._trackAllocatedMemory(h.byteLength, "Texture");
                     else {
-                        const t = Zd[this.dataFormat] || 4,
-                            e = qd[this.type] || 1;
+                        const t = qd[this.dataFormat] || 4,
+                            e = Xd[this.type] || 1;
                         this._trackAllocatedMemory(this.width * this.height * this.depth * t * e, "Texture")
                     }
                     return this.loaded = !0, this
                 }
             }
 
-            function ap(t, e) {
+            function lp(t, e) {
                 const {
                     gl: n,
                     width: i,
                     height: r,
                     id: s
                 } = t;
-                return new bp(n, Object.assign({}, e, {
+                return new yp(n, Object.assign({}, e, {
                     id: "framebuffer-for-".concat(s),
                     width: i,
                     height: r,
                     attachments: {
                         36064: t
                     }
                 }))
             }
 
-            function lp(t) {
+            function cp(t) {
                 let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                 const {
                     sourceX: n = 0,
                     sourceY: i = 0,
                     sourceFormat: r = 6408
                 } = e;
                 let {
@@ -12209,24 +12212,24 @@
                     sourceWidth: a,
                     sourceHeight: l,
                     sourceType: c
                 } = e;
                 const {
                     framebuffer: h,
                     deleteFramebuffer: u
-                } = hp(t);
-                Ed(h);
+                } = up(t);
+                Pd(h);
                 const {
                     gl: d,
                     handle: p,
                     attachments: f
                 } = h;
-                a = a || h.width, l = l || h.height, 36064 === s && null === p && (s = 1028), Ed(f[s]), c = c || f[s].type, o = function(t, e, n, i, r) {
+                a = a || h.width, l = l || h.height, 36064 === s && null === p && (s = 1028), Pd(f[s]), c = c || f[s].type, o = function(t, e, n, i, r) {
                     if (t) return t;
-                    const s = jd(e = e || 5121, {
+                    const s = Fd(e = e || 5121, {
                             clamped: !1
                         }),
                         o = function(t) {
                             switch (t) {
                                 case 6406:
                                 case 33326:
                                 case 6403:
@@ -12237,38 +12240,38 @@
                                 case 6407:
                                 case 34837:
                                     return 3;
                                 case 6408:
                                 case 34836:
                                     return 4;
                                 default:
-                                    return Ed(!1), 0
+                                    return Pd(!1), 0
                             }
                         }(n);
                     return new s(i * r * o)
-                }(o, c, r, a, l), c = c || kd(o);
+                }(o, c, r, a, l), c = c || jd(o);
                 const g = d.bindFramebuffer(36160, p);
                 return d.readPixels(n, i, a, l, r, c, o), d.bindFramebuffer(36160, g || null), u && h.delete(), o
             }
 
-            function cp(t) {
+            function hp(t) {
                 let {
                     sourceAttachment: e = 36064,
                     targetMaxHeight: n = Number.MAX_SAFE_INTEGER
-                } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {}, i = lp(t, {
+                } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {}, i = cp(t, {
                     sourceAttachment: e
                 }), {
                     width: r,
                     height: s
                 } = t;
                 for (; s > n;)({
                     data: i,
                     width: r,
                     height: s
-                } = Fd({
+                } = zd({
                     data: i,
                     width: r,
                     height: s
                 }));
                 ! function(t) {
                     let {
                         data: e,
@@ -12292,48 +12295,48 @@
                 const o = document.createElement("canvas");
                 o.width = r, o.height = s;
                 const a = o.getContext("2d"),
                     l = a.createImageData(r, s);
                 return l.data.set(i), a.putImageData(l, 0, 0), o.toDataURL()
             }
 
-            function hp(t) {
-                return t instanceof bp ? {
+            function up(t) {
+                return t instanceof yp ? {
                     framebuffer: t,
                     deleteFramebuffer: !1
                 } : {
-                    framebuffer: ap(t),
+                    framebuffer: lp(t),
                     deleteFramebuffer: !0
                 }
             }
-            const up = "TIMER_QUERY",
-                dp = "ELEMENT_INDEX_UINT32",
-                pp = {
+            const dp = "TIMER_QUERY",
+                pp = "ELEMENT_INDEX_UINT32",
+                fp = {
                     WEBGL2: [!1, !0],
                     VERTEX_ARRAY_OBJECT: ["OES_vertex_array_object", !0],
-                    [up]: ["EXT_disjoint_timer_query", "EXT_disjoint_timer_query_webgl2"],
+                    [dp]: ["EXT_disjoint_timer_query", "EXT_disjoint_timer_query_webgl2"],
                     INSTANCED_RENDERING: ["ANGLE_instanced_arrays", !0],
                     MULTIPLE_RENDER_TARGETS: ["WEBGL_draw_buffers", !0],
-                    [dp]: ["OES_element_index_uint", !0],
+                    [pp]: ["OES_element_index_uint", !0],
                     BLEND_EQUATION_MINMAX: ["EXT_blend_minmax", !0],
                     FLOAT_BLEND: ["EXT_float_blend"],
                     COLOR_ENCODING_SRGB: ["EXT_sRGB", !0],
                     TEXTURE_DEPTH: ["WEBGL_depth_texture", !0],
                     TEXTURE_FLOAT: ["OES_texture_float", !0],
                     TEXTURE_HALF_FLOAT: ["OES_texture_half_float", !0],
                     TEXTURE_FILTER_LINEAR_FLOAT: ["OES_texture_float_linear"],
                     TEXTURE_FILTER_LINEAR_HALF_FLOAT: ["OES_texture_half_float_linear"],
                     TEXTURE_FILTER_ANISOTROPIC: ["EXT_texture_filter_anisotropic"],
                     COLOR_ATTACHMENT_RGBA32F: [function(t) {
-                        const e = new Qd(t, {
+                        const e = new Jd(t, {
                                 format: 6408,
                                 type: 5126,
                                 dataFormat: 6408
                             }),
-                            n = new bp(t, {
+                            n = new yp(t, {
                                 id: "test-framebuffer",
                                 check: !1,
                                 attachments: {
                                     36064: e
                                 }
                             }),
                             i = n.getStatus();
@@ -12342,50 +12345,50 @@
                     COLOR_ATTACHMENT_FLOAT: [!1, "EXT_color_buffer_float"],
                     COLOR_ATTACHMENT_HALF_FLOAT: ["EXT_color_buffer_half_float"],
                     GLSL_FRAG_DATA: ["WEBGL_draw_buffers", !0],
                     GLSL_FRAG_DEPTH: ["EXT_frag_depth", !0],
                     GLSL_DERIVATIVES: ["OES_standard_derivatives", !0],
                     GLSL_TEXTURE_LOD: ["EXT_shader_texture_lod", !0]
                 },
-                fp = 2;
+                gp = 2;
 
-            function gp(t, e) {
-                return (e = Array.isArray(e) ? e : [e]).every((e => mp(t, e)))
+            function mp(t, e) {
+                return (e = Array.isArray(e) ? e : [e]).every((e => vp(t, e)))
             }
 
-            function mp(t, e) {
+            function vp(t, e) {
                 return t.luma = t.luma || {}, t.luma.caps = t.luma.caps || {}, void 0 === t.luma.caps[e] && (t.luma.caps[e] = function(t, e) {
-                    const n = pp[e];
+                    const n = fp[e];
                     let i;
-                    Ed(n, e);
+                    Pd(n, e);
                     const r = Lu(t) && n[1] || n[0];
                     if ("function" == typeof r) i = r(t);
                     else if (Array.isArray(r)) {
                         i = !0;
                         for (const e of r) i = i && Boolean(t.getExtension(e))
-                    } else "string" == typeof r ? i = Boolean(t.getExtension(r)) : "boolean" == typeof r ? i = r : Ed(!1);
+                    } else "string" == typeof r ? i = Boolean(t.getExtension(r)) : "boolean" == typeof r ? i = r : Pd(!1);
                     return i
-                }(t, e)), t.luma.caps[e] || Tu.log(fp, "Feature: ".concat(e, " not supported"))(), t.luma.caps[e]
+                }(t, e)), t.luma.caps[e] || Tu.log(gp, "Feature: ".concat(e, " not supported"))(), t.luma.caps[e]
             }
-            const vp = "Multiple render targets not supported";
-            class bp extends Rd {
+            const bp = "Multiple render targets not supported";
+            class yp extends Id {
                 get[Symbol.toStringTag]() {
                     return "Framebuffer"
                 }
                 static isSupported(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                     const {
                         colorBufferFloat: n,
                         colorBufferHalfFloat: i
                     } = e;
                     let r = !0;
                     return n && (r = Boolean(t.getExtension("EXT_color_buffer_float") || t.getExtension("WEBGL_color_buffer_float") || t.getExtension("OES_texture_float"))), i && (r = r && Boolean(t.getExtension("EXT_color_buffer_float") || t.getExtension("EXT_color_buffer_half_float"))), r
                 }
                 static getDefaultFramebuffer(t) {
-                    return t.luma = t.luma || {}, t.luma.defaultFramebuffer = t.luma.defaultFramebuffer || new bp(t, {
+                    return t.luma = t.luma || {}, t.luma.defaultFramebuffer = t.luma.defaultFramebuffer || new yp(t, {
                         id: "default-framebuffer",
                         handle: null,
                         attachments: {}
                     }), t.luma.defaultFramebuffer
                 }
                 get MAX_COLOR_ATTACHMENTS() {
                     const t = Iu(this.gl);
@@ -12419,15 +12422,15 @@
                         color: r = !0,
                         depth: s = !0,
                         stencil: o = !1,
                         check: a = !0,
                         readBuffer: l,
                         drawBuffers: c
                     } = t;
-                    if (Ed(e >= 0 && n >= 0, "Width and height need to be integers"), this.width = e, this.height = n, i)
+                    if (Pd(e >= 0 && n >= 0, "Width and height need to be integers"), this.width = e, this.height = n, i)
                         for (const t in i) {
                             const r = i[t];
                             (Array.isArray(r) ? r[0] : r).resize({
                                 width: e,
                                 height: n
                             })
                         } else i = this._createDefaultAttachments(r, s, o, e, n);
@@ -12461,15 +12464,15 @@
                 }
                 resize() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {},
                         {
                             width: e,
                             height: n
                         } = t;
-                    if (null === this.handle) return Ed(void 0 === e && void 0 === n), this.width = this.gl.drawingBufferWidth, this.height = this.gl.drawingBufferHeight, this;
+                    if (null === this.handle) return Pd(void 0 === e && void 0 === n), this.width = this.gl.drawingBufferWidth, this.height = this.gl.drawingBufferHeight, this;
                     void 0 === e && (e = this.gl.drawingBufferWidth), void 0 === n && (n = this.gl.drawingBufferHeight), e !== this.width && n !== this.height && Tu.log(2, "Resizing framebuffer ".concat(this.id, " to ").concat(e, "x").concat(n))();
                     for (const t in this.attachments) this.attachments[t].resize({
                         width: e,
                         height: n
                     });
                     return this.width = e, this.height = n, this
                 }
@@ -12480,20 +12483,20 @@
                     } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                     const i = {};
                     e && Object.keys(this.attachments).forEach((t => {
                         i[t] = null
                     })), Object.assign(i, t);
                     const r = this.gl.bindFramebuffer(36160, this.handle);
                     for (const t in i) {
-                        Ed(void 0 !== t, "Misspelled framebuffer binding point?");
+                        Pd(void 0 !== t, "Misspelled framebuffer binding point?");
                         const e = Number(t),
                             r = i[e];
                         let s = r;
                         if (s)
-                            if (s instanceof tp) this._attachRenderbuffer({
+                            if (s instanceof ep) this._attachRenderbuffer({
                                 attachment: e,
                                 renderbuffer: s
                             });
                             else if (Array.isArray(r)) {
                             const [t, n = 0, i = 0] = r;
                             s = t, this._attachTexture({
                                 attachment: e,
@@ -12518,15 +12521,15 @@
                     }))
                 }
                 checkStatus() {
                     const {
                         gl: t
                     } = this, e = this.getStatus();
                     if (36053 !== e) throw new Error(function(t) {
-                        return (bp.STATUS || {})[t] || "Framebuffer error ".concat(t)
+                        return (yp.STATUS || {})[t] || "Framebuffer error ".concat(t)
                     }(e));
                     return this
                 }
                 getStatus() {
                     const {
                         gl: t
                     } = this, e = t.bindFramebuffer(36160, this.handle), n = t.checkFramebufferStatus(36160);
@@ -12536,31 +12539,31 @@
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     const {
                         color: e,
                         depth: n,
                         stencil: i,
                         drawBuffers: r = []
                     } = t, s = this.gl.bindFramebuffer(36160, this.handle);
-                    return (e || n || i) && ip(this.gl, {
+                    return (e || n || i) && rp(this.gl, {
                         color: e,
                         depth: n,
                         stencil: i
                     }), r.forEach(((t, e) => {
                         ! function(t) {
                             let {
                                 framebuffer: e = null,
-                                buffer: n = ep,
+                                buffer: n = np,
                                 drawBuffer: i = 0,
                                 value: r = [0, 0, 0, 0]
                             } = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                             Iu(t), ud(t, {
                                 framebuffer: e
                             }, (() => {
                                 switch (n) {
-                                    case ep:
+                                    case np:
                                         switch (r.constructor) {
                                             case Int32Array:
                                                 t.clearBufferiv(n, i, r);
                                                 break;
                                             case Uint32Array:
                                                 t.clearBufferuiv(n, i, r);
                                                 break;
@@ -12576,15 +12579,15 @@
                                         t.clearBufferiv(6146, 0, [r]);
                                         break;
                                     case 34041:
                                         const [e, s] = r;
                                         t.clearBufferfi(34041, 0, e, s);
                                         break;
                                     default:
-                                        Ed(!1, np)
+                                        Pd(!1, ip)
                                 }
                             }))
                         }(this.gl, {
                             drawBuffer: e,
                             value: t
                         })
                     })), this.gl.bindFramebuffer(36160, s || null), this
@@ -12617,43 +12620,43 @@
                     } = t;
                     const o = Iu(this.gl),
                         a = o.bindFramebuffer(36008, this.handle);
                     return 0 === n && 0 === i && void 0 === r && void 0 === s ? o.invalidateFramebuffer(36008, e) : o.invalidateFramebuffer(36008, e, n, i, r, s), o.bindFramebuffer(36008, a), this
                 }
                 getAttachmentParameter(t, e, n) {
                     let i = this._getAttachmentParameterFallback(e);
-                    return null === i && (this.gl.bindFramebuffer(36160, this.handle), i = this.gl.getFramebufferAttachmentParameter(36160, t, e), this.gl.bindFramebuffer(36160, null)), n && i > 1e3 && (i = Sd(this.gl, i)), i
+                    return null === i && (this.gl.bindFramebuffer(36160, this.handle), i = this.gl.getFramebufferAttachmentParameter(36160, t, e), this.gl.bindFramebuffer(36160, null)), n && i > 1e3 && (i = Cd(this.gl, i)), i
                 }
                 getAttachmentParameters() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : 36064,
                         e = arguments.length > 1 ? arguments[1] : void 0,
                         n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : this.constructor.ATTACHMENT_PARAMETERS || [];
                     const i = {};
-                    for (const r of n) i[e ? Sd(this.gl, r) : r] = this.getAttachmentParameter(t, r, e);
+                    for (const r of n) i[e ? Cd(this.gl, r) : r] = this.getAttachmentParameter(t, r, e);
                     return i
                 }
                 getParameters() {
                     let t = !(arguments.length > 0 && void 0 !== arguments[0]) || arguments[0];
                     const e = Object.keys(this.attachments),
                         n = {};
                     for (const i of e) {
                         const e = Number(i);
-                        n[t ? Sd(this.gl, e) : e] = this.getAttachmentParameters(e, t)
+                        n[t ? Cd(this.gl, e) : e] = this.getAttachmentParameters(e, t)
                     }
                     return n
                 }
                 show() {
-                    return "undefined" != typeof window && window.open(cp(this), "luma-debug-texture"), this
+                    return "undefined" != typeof window && window.open(hp(this), "luma-debug-texture"), this
                 }
                 log() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : 0,
                         e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "";
                     if (t > Tu.level || "undefined" == typeof window) return this;
                     e = e || "Framebuffer ".concat(this.id);
-                    const n = cp(this, {
+                    const n = hp(this, {
                         targetMaxHeight: 100
                     });
                     return Tu.image({
                         logLevel: t,
                         message: e,
                         image: n
                     }, e)(), this
@@ -12668,43 +12671,43 @@
                     let {
                         target: t = 36160
                     } = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     return this.gl.bindFramebuffer(t, null), this
                 }
                 _createDefaultAttachments(t, e, n, i, r) {
                     let s = null;
-                    return t && (s = s || {}, s[36064] = new Qd(this.gl, {
+                    return t && (s = s || {}, s[36064] = new Jd(this.gl, {
                         id: "".concat(this.id, "-color0"),
                         pixels: null,
                         format: 6408,
                         type: 5121,
                         width: i,
                         height: r,
                         mipmaps: !1,
                         parameters: {
                             10241: 9729,
                             10240: 9729,
                             10242: 33071,
                             10243: 33071
                         }
-                    }), this.ownResources.push(s[36064])), e && n ? (s = s || {}, s[33306] = new tp(this.gl, {
+                    }), this.ownResources.push(s[36064])), e && n ? (s = s || {}, s[33306] = new ep(this.gl, {
                         id: "".concat(this.id, "-depth-stencil"),
                         format: 35056,
                         width: i,
                         height: 111
-                    }), this.ownResources.push(s[33306])) : e ? (s = s || {}, s[36096] = new tp(this.gl, {
+                    }), this.ownResources.push(s[33306])) : e ? (s = s || {}, s[36096] = new ep(this.gl, {
                         id: "".concat(this.id, "-depth"),
                         format: 33189,
                         width: i,
                         height: r
-                    }), this.ownResources.push(s[36096])) : n && Ed(!1), s
+                    }), this.ownResources.push(s[36096])) : n && Pd(!1), s
                 }
                 _unattach(t) {
                     const e = this.attachments[t];
-                    e && (e instanceof tp ? this.gl.framebufferRenderbuffer(36160, t, 36161, null) : this.gl.framebufferTexture2D(36160, t, 3553, null, 0), delete this.attachments[t])
+                    e && (e instanceof ep ? this.gl.framebufferRenderbuffer(36160, t, 36161, null) : this.gl.framebufferTexture2D(36160, t, 3553, null, 0), delete this.attachments[t])
                 }
                 _attachRenderbuffer(t) {
                     let {
                         attachment: e = 36064,
                         renderbuffer: n
                     } = t;
                     const {
@@ -12733,38 +12736,38 @@
                             }(i);
                             s.framebufferTexture2D(36160, e, t, n.handle, r);
                             break;
                         case 3553:
                             s.framebufferTexture2D(36160, e, 3553, n.handle, r);
                             break;
                         default:
-                            Ed(!1, "Illegal texture type")
+                            Pd(!1, "Illegal texture type")
                     }
                     s.bindTexture(n.target, null), this.attachments[e] = n
                 }
                 _setReadBuffer(t) {
                     const e = Lu(n = this.gl) ? n : null;
                     var n;
-                    e ? e.readBuffer(t) : Ed(36064 === t || 1029 === t, vp), this.readBuffer = t
+                    e ? e.readBuffer(t) : Pd(36064 === t || 1029 === t, bp), this.readBuffer = t
                 }
                 _setDrawBuffers(t) {
                     const {
                         gl: e
                     } = this, n = Iu(e);
                     if (n) n.drawBuffers(t);
                     else {
                         const n = e.getExtension("WEBGL_draw_buffers");
-                        n ? n.drawBuffersWEBGL(t) : Ed(1 === t.length && (36064 === t[0] || 1029 === t[0]), vp)
+                        n ? n.drawBuffersWEBGL(t) : Pd(1 === t.length && (36064 === t[0] || 1029 === t[0]), bp)
                     }
                     this.drawBuffers = t
                 }
                 _getAttachmentParameterFallback(t) {
                     const e = function(t) {
                         t.luma = t.luma || {}, t.luma.caps = t.luma.caps || {};
-                        for (const e in pp) void 0 === t.luma.caps[e] && (t.luma.caps[e] = mp(t, e));
+                        for (const e in fp) void 0 === t.luma.caps[e] && (t.luma.caps[e] = vp(t, e));
                         return t.luma.caps
                     }(this.gl);
                     switch (t) {
                         case 36052:
                             return e.WEBGL2 ? null : 0;
                         case 33298:
                         case 33299:
@@ -12787,223 +12790,223 @@
                 _deleteHandle() {
                     this.gl.deleteFramebuffer(this.handle)
                 }
                 _bindHandle(t) {
                     return this.gl.bindFramebuffer(36160, t)
                 }
             }
-            bp.ATTACHMENT_PARAMETERS = [36049, 36048, 33296, 33298, 33299, 33300, 33301, 33302, 33303];
-            const yp = {
-                    5126: Ip.bind(null, "uniform1fv", Sp, 1, kp),
-                    35664: Ip.bind(null, "uniform2fv", Sp, 2, kp),
-                    35665: Ip.bind(null, "uniform3fv", Sp, 3, kp),
-                    35666: Ip.bind(null, "uniform4fv", Sp, 4, kp),
-                    5124: Ip.bind(null, "uniform1iv", Cp, 1, kp),
-                    35667: Ip.bind(null, "uniform2iv", Cp, 2, kp),
-                    35668: Ip.bind(null, "uniform3iv", Cp, 3, kp),
-                    35669: Ip.bind(null, "uniform4iv", Cp, 4, kp),
-                    35670: Ip.bind(null, "uniform1iv", Cp, 1, kp),
-                    35671: Ip.bind(null, "uniform2iv", Cp, 2, kp),
-                    35672: Ip.bind(null, "uniform3iv", Cp, 3, kp),
-                    35673: Ip.bind(null, "uniform4iv", Cp, 4, kp),
-                    35674: Ip.bind(null, "uniformMatrix2fv", Sp, 4, jp),
-                    35675: Ip.bind(null, "uniformMatrix3fv", Sp, 9, jp),
-                    35676: Ip.bind(null, "uniformMatrix4fv", Sp, 16, jp),
-                    35678: Rp,
-                    35680: Rp,
-                    5125: Ip.bind(null, "uniform1uiv", Tp, 1, kp),
-                    36294: Ip.bind(null, "uniform2uiv", Tp, 2, kp),
-                    36295: Ip.bind(null, "uniform3uiv", Tp, 3, kp),
-                    36296: Ip.bind(null, "uniform4uiv", Tp, 4, kp),
-                    35685: Ip.bind(null, "uniformMatrix2x3fv", Sp, 6, jp),
-                    35686: Ip.bind(null, "uniformMatrix2x4fv", Sp, 8, jp),
-                    35687: Ip.bind(null, "uniformMatrix3x2fv", Sp, 6, jp),
-                    35688: Ip.bind(null, "uniformMatrix3x4fv", Sp, 12, jp),
-                    35689: Ip.bind(null, "uniformMatrix4x2fv", Sp, 8, jp),
-                    35690: Ip.bind(null, "uniformMatrix4x3fv", Sp, 12, jp),
-                    35678: Rp,
-                    35680: Rp,
-                    35679: Rp,
-                    35682: Rp,
-                    36289: Rp,
-                    36292: Rp,
-                    36293: Rp,
-                    36298: Rp,
-                    36299: Rp,
-                    36300: Rp,
-                    36303: Rp,
-                    36306: Rp,
-                    36307: Rp,
-                    36308: Rp,
-                    36311: Rp
+            yp.ATTACHMENT_PARAMETERS = [36049, 36048, 33296, 33298, 33299, 33300, 33301, 33302, 33303];
+            const _p = {
+                    5126: kp.bind(null, "uniform1fv", Cp, 1, jp),
+                    35664: kp.bind(null, "uniform2fv", Cp, 2, jp),
+                    35665: kp.bind(null, "uniform3fv", Cp, 3, jp),
+                    35666: kp.bind(null, "uniform4fv", Cp, 4, jp),
+                    5124: kp.bind(null, "uniform1iv", Tp, 1, jp),
+                    35667: kp.bind(null, "uniform2iv", Tp, 2, jp),
+                    35668: kp.bind(null, "uniform3iv", Tp, 3, jp),
+                    35669: kp.bind(null, "uniform4iv", Tp, 4, jp),
+                    35670: kp.bind(null, "uniform1iv", Tp, 1, jp),
+                    35671: kp.bind(null, "uniform2iv", Tp, 2, jp),
+                    35672: kp.bind(null, "uniform3iv", Tp, 3, jp),
+                    35673: kp.bind(null, "uniform4iv", Tp, 4, jp),
+                    35674: kp.bind(null, "uniformMatrix2fv", Cp, 4, Fp),
+                    35675: kp.bind(null, "uniformMatrix3fv", Cp, 9, Fp),
+                    35676: kp.bind(null, "uniformMatrix4fv", Cp, 16, Fp),
+                    35678: Ip,
+                    35680: Ip,
+                    5125: kp.bind(null, "uniform1uiv", Ap, 1, jp),
+                    36294: kp.bind(null, "uniform2uiv", Ap, 2, jp),
+                    36295: kp.bind(null, "uniform3uiv", Ap, 3, jp),
+                    36296: kp.bind(null, "uniform4uiv", Ap, 4, jp),
+                    35685: kp.bind(null, "uniformMatrix2x3fv", Cp, 6, Fp),
+                    35686: kp.bind(null, "uniformMatrix2x4fv", Cp, 8, Fp),
+                    35687: kp.bind(null, "uniformMatrix3x2fv", Cp, 6, Fp),
+                    35688: kp.bind(null, "uniformMatrix3x4fv", Cp, 12, Fp),
+                    35689: kp.bind(null, "uniformMatrix4x2fv", Cp, 8, Fp),
+                    35690: kp.bind(null, "uniformMatrix4x3fv", Cp, 12, Fp),
+                    35678: Ip,
+                    35680: Ip,
+                    35679: Ip,
+                    35682: Ip,
+                    36289: Ip,
+                    36292: Ip,
+                    36293: Ip,
+                    36298: Ip,
+                    36299: Ip,
+                    36300: Ip,
+                    36303: Ip,
+                    36306: Ip,
+                    36307: Ip,
+                    36308: Ip,
+                    36311: Ip
                 },
-                _p = {},
                 xp = {},
                 wp = {},
-                Ep = [0];
+                Ep = {},
+                Pp = [0];
 
-            function Pp(t, e, n, i) {
-                1 === e && "boolean" == typeof t && (t = t ? 1 : 0), Number.isFinite(t) && (Ep[0] = t, t = Ep);
+            function Sp(t, e, n, i) {
+                1 === e && "boolean" == typeof t && (t = t ? 1 : 0), Number.isFinite(t) && (Pp[0] = t, t = Pp);
                 const r = t.length;
                 if (r % e && Tu.warn("Uniform size should be multiples of ".concat(e), t)(), t instanceof n) return t;
                 let s = i[r];
                 s || (s = new n(r), i[r] = s);
                 for (let e = 0; e < r; e++) s[e] = t[e];
                 return s
             }
 
-            function Sp(t, e) {
-                return Pp(t, e, Float32Array, _p)
-            }
-
             function Cp(t, e) {
-                return Pp(t, e, Int32Array, xp)
+                return Sp(t, e, Float32Array, xp)
             }
 
             function Tp(t, e) {
-                return Pp(t, e, Uint32Array, wp)
+                return Sp(t, e, Int32Array, wp)
             }
 
-            function Ap(t, e, n) {
-                const i = yp[n.type];
+            function Ap(t, e) {
+                return Sp(t, e, Uint32Array, Ep)
+            }
+
+            function Mp(t, e, n) {
+                const i = _p[n.type];
                 if (!i) throw new Error("Unknown GLSL uniform type ".concat(n.type));
                 return i().bind(null, t, e)
             }
 
-            function Mp(t) {
+            function Op(t) {
                 if ("]" !== t[t.length - 1]) return {
                     name: t,
                     length: 1,
                     isArray: !1
                 };
                 const e = t.match(/([^[]*)(\[[0-9]+\])?/);
                 if (!e || e.length < 2) throw new Error("Failed to parse GLSL uniform name ".concat(t));
                 return {
                     name: e[1],
                     length: e[2] || 1,
                     isArray: Boolean(e[2])
                 }
             }
 
-            function Op(t) {
+            function Lp(t) {
                 return Array.isArray(t) || ArrayBuffer.isView(t) ? function(t) {
                     if (0 === t.length) return !1;
                     const e = Math.min(t.length, 16);
                     for (let n = 0; n < e; ++n)
                         if (!Number.isFinite(t[n])) return !1;
                     return !0
-                }(t) : !!isFinite(t) || !0 === t || !1 === t || t instanceof Kd || t instanceof tp || t instanceof bp && Boolean(t.texture)
+                }(t) : !!isFinite(t) || !0 === t || !1 === t || t instanceof Qd || t instanceof ep || t instanceof yp && Boolean(t.texture)
             }
 
-            function Lp(t, e, n) {
+            function Rp(t, e, n) {
                 if (Array.isArray(n) || ArrayBuffer.isView(n))
                     if (t[e]) {
                         const i = t[e];
                         for (let t = 0, e = n.length; t < e; ++t) i[t] = n[t]
                     } else t[e] = n.slice();
                 else t[e] = n
             }
 
-            function Rp() {
+            function Ip() {
                 let t = null;
                 return (e, n, i) => {
                     const r = t !== i;
                     return r && (e.uniform1i(n, i), t = i), r
                 }
             }
 
-            function Ip(t, e, n, i) {
+            function kp(t, e, n, i) {
                 let r = null,
                     s = null;
                 return (o, a, l) => {
                     const c = e(l, n),
                         h = c.length;
                     let u = !1;
                     if (null === r) r = new Float32Array(h), s = h, u = !0;
                     else {
-                        Ed(s === h, "Uniform length cannot change.");
+                        Pd(s === h, "Uniform length cannot change.");
                         for (let t = 0; t < h; ++t)
                             if (c[t] !== r[t]) {
                                 u = !0;
                                 break
                             }
                     }
                     return u && (i(o, t, a, c), r.set(c)), u
                 }
             }
 
-            function kp(t, e, n, i) {
+            function jp(t, e, n, i) {
                 t[e](n, i)
             }
 
-            function jp(t, e, n, i) {
+            function Fp(t, e, n, i) {
                 t[e](n, !1, i)
             }
 
-            function Fp(t) {
+            function zp(t) {
                 let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "unnamed";
                 const n = t.match(/#define[\s*]SHADER_NAME[\s*]([A-Za-z0-9_-]+)[\s*]/);
                 return n ? n[1] : e
             }
 
-            function zp(t, e) {
+            function Bp(t, e) {
                 let n = "";
                 for (let i = 0; i < e.length; i++) {
                     const r = e[i];
                     if ((t[i + 3] || t[i + 2] || t[i + 1]) && (n += "".concat(r, "\n"), t[i + 1])) {
                         const e = t[i + 1],
                             r = e.split(":", 3),
                             s = r[0],
                             o = parseInt(r[1], 10) || 0,
                             a = e.substring(r.join(":").length + 1).trim();
-                        n += Bp("^^^ ".concat(s, ": ").concat(a, "\n\n"), o)
+                        n += Dp("^^^ ".concat(s, ": ").concat(a, "\n\n"), o)
                     }
                 }
                 return n
             }
 
-            function Bp(t, e) {
+            function Dp(t, e) {
                 let n = "";
                 for (let t = 0; t < e; ++t) n += " ";
                 return "".concat(n).concat(t)
             }
-            class Dp extends Rd {
+            class Np extends Id {
                 get[Symbol.toStringTag]() {
                     return "Shader"
                 }
                 static getTypeName(t) {
                     switch (t) {
                         case 35633:
                             return "vertex-shader";
                         case 35632:
                             return "fragment-shader";
                         default:
-                            return Ed(!1), "unknown"
+                            return Pd(!1), "unknown"
                     }
                 }
                 constructor(t, e) {
-                    Ru(t), Ed("string" == typeof e.source, "Shader: GLSL source code must be a JavaScript string"), super(t, {
-                        id: Fp(e.source, null) || e.id || Td("unnamed ".concat(Dp.getTypeName(e.shaderType)))
+                    Ru(t), Pd("string" == typeof e.source, "Shader: GLSL source code must be a JavaScript string"), super(t, {
+                        id: zp(e.source, null) || e.id || Ad("unnamed ".concat(Np.getTypeName(e.shaderType)))
                     }), this.shaderType = e.shaderType, this.source = e.source, this.initialize(e)
                 }
                 initialize(t) {
                     let {
                         source: e
                     } = t;
-                    const n = Fp(e, null);
-                    n && (this.id = Td(n)), this._compile(e)
+                    const n = zp(e, null);
+                    n && (this.id = Ad(n)), this._compile(e)
                 }
                 getParameter(t) {
                     return this.gl.getShaderParameter(this.handle, t)
                 }
                 toString() {
-                    return "".concat(Dp.getTypeName(this.shaderType), ":").concat(this.id)
+                    return "".concat(Np.getTypeName(this.shaderType), ":").concat(this.id)
                 }
                 getName() {
-                    return Fp(this.source) || "unnamed-shader"
+                    return zp(this.source) || "unnamed-shader"
                 }
                 getSource() {
                     return this.gl.getShaderSource(this.handle)
                 }
                 getTranslatedSource() {
                     const t = this.gl.getExtension("WEBGL_debug_shaders");
                     return t ? t.getTranslatedShaderSource(this.handle) : "No translated source available. WEBGL_debug_shaders not implemented"
@@ -13016,15 +13019,15 @@
                                 shaderName: e,
                                 errors: n,
                                 warnings: i
                             } = function(t, e, n, i) {
                                 const r = t.split(/\r?\n/),
                                     s = {},
                                     o = {},
-                                    a = i || Fp(e) || "(unnamed)",
+                                    a = i || zp(e) || "(unnamed)",
                                     l = "".concat(function(t) {
                                         switch (t) {
                                             case 35632:
                                                 return "fragment";
                                             case 35633:
                                                 return "vertex";
                                             default:
@@ -13044,21 +13047,21 @@
                                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : 1,
                                         n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : ": ";
                                     const i = t.split(/\r?\n/),
                                         r = String(i.length + e - 1).length;
                                     return i.map(((t, i) => {
                                         const s = String(i + e),
                                             o = s.length;
-                                        return Bp(s, r - o) + n + t
+                                        return Dp(s, r - o) + n + t
                                     }))
                                 }(e);
                                 return {
                                     shaderName: l,
-                                    errors: zp(s, c),
-                                    warnings: zp(o, c)
+                                    errors: Bp(s, c),
+                                    warnings: Bp(o, c)
                                 }
                             }(t, this.source, this.shaderType, this.id);
                         throw Tu.error("GLSL compilation errors in ".concat(e, "\n").concat(n))(), Tu.warn("GLSL compilation warnings in ".concat(e, "\n").concat(i))(), new Error("GLSL compilation errors in ".concat(e))
                     }
                 }
                 _deleteHandle() {
                     this.gl.deleteShader(this.handle)
@@ -13066,107 +13069,107 @@
                 _getOptsFromHandle() {
                     return {
                         type: this.getParameter(35663),
                         source: this.getSource()
                     }
                 }
             }
-            class Np extends Dp {
+            class Vp extends Np {
                 get[Symbol.toStringTag]() {
                     return "VertexShader"
                 }
                 constructor(t, e) {
                     "string" == typeof e && (e = {
                         source: e
                     }), super(t, Object.assign({}, e, {
                         shaderType: 35633
                     }))
                 }
                 _createHandle() {
                     return this.gl.createShader(35633)
                 }
             }
-            class Vp extends Dp {
+            class Up extends Np {
                 get[Symbol.toStringTag]() {
                     return "FragmentShader"
                 }
                 constructor(t, e) {
                     "string" == typeof e && (e = {
                         source: e
                     }), super(t, Object.assign({}, e, {
                         shaderType: 35632
                     }))
                 }
                 _createHandle() {
                     return this.gl.createShader(35632)
                 }
             }
-            const Up = 5120,
-                Gp = 5121,
-                Wp = 5122,
-                Hp = 5123,
-                Zp = 5126,
-                qp = 5124,
-                Xp = 5125,
-                Yp = {
-                    [Zp]: [Zp, 1, "float"],
-                    35664: [Zp, 2, "vec2"],
-                    35665: [Zp, 3, "vec3"],
-                    35666: [Zp, 4, "vec4"],
-                    [qp]: [qp, 1, "int"],
-                    35667: [qp, 2, "ivec2"],
-                    35668: [qp, 3, "ivec3"],
-                    35669: [qp, 4, "ivec4"],
-                    [Xp]: [Xp, 1, "uint"],
-                    36294: [Xp, 2, "uvec2"],
-                    36295: [Xp, 3, "uvec3"],
-                    36296: [Xp, 4, "uvec4"],
-                    35670: [Zp, 1, "bool"],
-                    35671: [Zp, 2, "bvec2"],
-                    35672: [Zp, 3, "bvec3"],
-                    35673: [Zp, 4, "bvec4"],
-                    35674: [Zp, 8, "mat2"],
-                    35685: [Zp, 8, "mat2x3"],
-                    35686: [Zp, 8, "mat2x4"],
-                    35675: [Zp, 12, "mat3"],
-                    35687: [Zp, 12, "mat3x2"],
-                    35688: [Zp, 12, "mat3x4"],
-                    35676: [Zp, 16, "mat4"],
-                    35689: [Zp, 16, "mat4x2"],
-                    35690: [Zp, 16, "mat4x3"]
+            const Gp = 5120,
+                Wp = 5121,
+                Hp = 5122,
+                Zp = 5123,
+                qp = 5126,
+                Xp = 5124,
+                Yp = 5125,
+                Kp = {
+                    [qp]: [qp, 1, "float"],
+                    35664: [qp, 2, "vec2"],
+                    35665: [qp, 3, "vec3"],
+                    35666: [qp, 4, "vec4"],
+                    [Xp]: [Xp, 1, "int"],
+                    35667: [Xp, 2, "ivec2"],
+                    35668: [Xp, 3, "ivec3"],
+                    35669: [Xp, 4, "ivec4"],
+                    [Yp]: [Yp, 1, "uint"],
+                    36294: [Yp, 2, "uvec2"],
+                    36295: [Yp, 3, "uvec3"],
+                    36296: [Yp, 4, "uvec4"],
+                    35670: [qp, 1, "bool"],
+                    35671: [qp, 2, "bvec2"],
+                    35672: [qp, 3, "bvec3"],
+                    35673: [qp, 4, "bvec4"],
+                    35674: [qp, 8, "mat2"],
+                    35685: [qp, 8, "mat2x3"],
+                    35686: [qp, 8, "mat2x4"],
+                    35675: [qp, 12, "mat3"],
+                    35687: [qp, 12, "mat3x2"],
+                    35688: [qp, 12, "mat3x4"],
+                    35676: [qp, 16, "mat4"],
+                    35689: [qp, 16, "mat4x2"],
+                    35690: [qp, 16, "mat4x3"]
                 };
 
-            function Kp(t) {
-                const e = Yp[t];
+            function Qp(t) {
+                const e = Kp[t];
                 if (!e) return null;
                 const [n, i] = e;
                 return {
                     type: n,
                     components: i
                 }
             }
 
-            function Qp(t, e) {
+            function Jp(t, e) {
                 switch (t) {
-                    case Up:
                     case Gp:
                     case Wp:
                     case Hp:
-                        t = Zp
+                    case Zp:
+                        t = qp
                 }
-                for (const n in Yp) {
-                    const [i, r, s] = Yp[n];
+                for (const n in Kp) {
+                    const [i, r, s] = Kp[n];
                     if (i === t && r === e) return {
                         glType: n,
                         name: s
                     }
                 }
                 return null
             }
-            class Jp {
+            class $p {
                 constructor(t) {
                     this.id = t.id, this.attributeInfos = [], this.attributeInfosByName = {}, this.attributeInfosByLocation = [], this.varyingInfos = [], this.varyingInfosByName = {}, Object.seal(this), this._readAttributesFromProgram(t), this._readVaryingsFromProgram(t)
                 }
                 getAttributeInfo(t) {
                     const e = Number(t);
                     return Number.isFinite(e) ? this.attributeInfosByLocation[e] : this.attributeInfosByName[t] || null
                 }
@@ -13220,70 +13223,70 @@
                     }
                     this.varyingInfos.sort(((t, e) => t.location - e.location))
                 }
                 _addAttribute(t, e, n, i) {
                     const {
                         type: r,
                         components: s
-                    } = Kp(n), o = {
+                    } = Qp(n), o = {
                         type: r,
                         size: i * s
                     };
                     this._inferProperties(t, e, o);
                     const a = {
                         location: t,
                         name: e,
-                        accessor: new Nd(o)
+                        accessor: new Vd(o)
                     };
                     this.attributeInfos.push(a), this.attributeInfosByLocation[t] = a, this.attributeInfosByName[a.name] = a
                 }
                 _inferProperties(t, e, n) {
                     /instance/i.test(e) && (n.divisor = 1)
                 }
                 _addVarying(t, e, n, i) {
                     const {
                         type: r,
                         components: s
-                    } = Kp(n), o = {
+                    } = Qp(n), o = {
                         location: t,
                         name: e,
-                        accessor: new Nd({
+                        accessor: new Vd({
                             type: r,
                             size: i * s
                         })
                     };
                     this.varyingInfos.push(o), this.varyingInfosByName[o.name] = o
                 }
             }
-            const $p = 35981,
-                tf = ["setVertexArray", "setAttributes", "setBuffers", "unsetBuffers", "use", "getUniformCount", "getUniformInfo", "getUniformLocation", "getUniformValue", "getVarying", "getFragDataLocation", "getAttachedShaders", "getAttributeCount", "getAttributeLocation", "getAttributeInfo"];
-            class ef extends Rd {
+            const tf = 35981,
+                ef = ["setVertexArray", "setAttributes", "setBuffers", "unsetBuffers", "use", "getUniformCount", "getUniformInfo", "getUniformLocation", "getUniformValue", "getVarying", "getFragDataLocation", "getAttachedShaders", "getAttributeCount", "getAttributeLocation", "getAttributeInfo"];
+            class nf extends Id {
                 get[Symbol.toStringTag]() {
                     return "Program"
                 }
                 constructor(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
-                    super(t, e), this.stubRemovedMethods("Program", "v6.0", tf), this._isCached = !1, this.initialize(e), Object.seal(this), this._setId(e.id)
+                    super(t, e), this.stubRemovedMethods("Program", "v6.0", ef), this._isCached = !1, this.initialize(e), Object.seal(this), this._setId(e.id)
                 }
                 initialize() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     const {
                         hash: e,
                         vs: n,
                         fs: i,
                         varyings: r,
-                        bufferMode: s = $p
+                        bufferMode: s = tf
                     } = t;
-                    return this.hash = e || "", this.vs = "string" == typeof n ? new Np(this.gl, {
+                    return this.hash = e || "", this.vs = "string" == typeof n ? new Vp(this.gl, {
                         id: "".concat(t.id, "-vs"),
                         source: n
-                    }) : n, this.fs = "string" == typeof i ? new Vp(this.gl, {
+                    }) : n, this.fs = "string" == typeof i ? new Up(this.gl, {
                         id: "".concat(t.id, "-fs"),
                         source: i
-                    }) : i, Ed(this.vs instanceof Np), Ed(this.fs instanceof Vp), this.uniforms = {}, this._textureUniforms = {}, r && r.length > 0 && (Iu(this.gl), this.varyings = r, this.gl2.transformFeedbackVaryings(this.handle, r, s)), this._compileAndLink(), this._readUniformLocationsFromLinkedProgram(), this.configuration = new Jp(this), this.setProps(t)
+                    }) : i, Pd(this.vs instanceof Vp), Pd(this.fs instanceof Up), this.uniforms = {}, this._textureUniforms = {}, r && r.length > 0 && (Iu(this.gl), this.varyings = r, this.gl2.transformFeedbackVaryings(this.handle, r, s)), this._compileAndLink(), this._readUniformLocationsFromLinkedProgram(), this.configuration = new $p(this), this.setProps(t)
                 }
                 delete() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     return this._isCached ? this : super.delete(t)
                 }
                 setProps(t) {
                     return "uniforms" in t && this.setUniforms(t.uniforms), this
@@ -13305,18 +13308,18 @@
                         framebuffer: p,
                         parameters: f = {},
                         uniforms: g,
                         samplers: m
                     } = t;
                     if ((g || m) && (Tu.deprecated("Program.draw({uniforms})", "Program.setUniforms(uniforms)")(), this.setUniforms(g || {})), Tu.priority >= e) {
                         const t = p ? p.id : "default",
-                            r = "mode=".concat(Sd(this.gl, n), " verts=").concat(i, " ") + "instances=".concat(c, " indexType=").concat(Sd(this.gl, l), " ") + "isInstanced=".concat(h, " isIndexed=").concat(a, " ") + "Framebuffer=".concat(t);
+                            r = "mode=".concat(Cd(this.gl, n), " verts=").concat(i, " ") + "instances=".concat(c, " indexType=").concat(Cd(this.gl, l), " ") + "isInstanced=".concat(h, " isIndexed=").concat(a, " ") + "Framebuffer=".concat(t);
                         Tu.log(e, r)()
                     }
-                    return Ed(u), this.gl.useProgram(this.handle), !(!this._areTexturesRenderable() || 0 === i || h && 0 === c || (u.bindForDraw(i, c, (() => {
+                    return Pd(u), this.gl.useProgram(this.handle), !(!this._areTexturesRenderable() || 0 === i || h && 0 === c || (u.bindForDraw(i, c, (() => {
                         if (void 0 !== p && (f = Object.assign({}, f, {
                                 framebuffer: p
                             })), d) {
                             const t = function(t) {
                                 switch (t) {
                                     case 0:
                                         return 0;
@@ -13325,49 +13328,49 @@
                                     case 2:
                                         return 1;
                                     case 4:
                                     case 5:
                                     case 6:
                                         return 4;
                                     default:
-                                        return Ed(!1), 0
+                                        return Pd(!1), 0
                                 }
                             }(n);
                             d.begin(t)
                         }
                         this._bindTextures(), ud(this.gl, f, (() => {
                             a && h ? this.gl2.drawElementsInstanced(n, i, l, r, c) : a && Lu(this.gl) && !isNaN(s) && !isNaN(o) ? this.gl2.drawRangeElements(n, s, o, i, l, r) : a ? this.gl.drawElements(n, i, l, r) : h ? this.gl2.drawArraysInstanced(n, r, i, c) : this.gl.drawArrays(n, r, i)
                         })), d && d.end()
                     })), 0))
                 }
                 setUniforms() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     Tu.priority >= 2 && function(t, e, n) {
                         for (const i in t) {
                             const r = t[i];
-                            if ((!n || Boolean(n[i])) && !Op(r)) throw e = e ? "".concat(e, " ") : "", console.error("".concat(e, " Bad uniform ").concat(i), r), new Error("".concat(e, " Bad uniform ").concat(i))
+                            if ((!n || Boolean(n[i])) && !Lp(r)) throw e = e ? "".concat(e, " ") : "", console.error("".concat(e, " Bad uniform ").concat(i), r), new Error("".concat(e, " Bad uniform ").concat(i))
                         }
                     }(t, this.id, this._uniformSetters), this.gl.useProgram(this.handle);
                     for (const e in t) {
                         const n = t[e],
                             i = this._uniformSetters[e];
                         if (i) {
                             let t = n,
                                 r = !1;
-                            if (t instanceof bp && (t = t.texture), t instanceof Kd)
+                            if (t instanceof yp && (t = t.texture), t instanceof Qd)
                                 if (r = this.uniforms[e] !== n, r) {
                                     void 0 === i.textureIndex && (i.textureIndex = this._textureIndexCounter++);
                                     const n = t,
                                         {
                                             textureIndex: r
                                         } = i;
                                     n.bind(r), t = r, this._textureUniforms[e] = n
                                 } else t = i.textureIndex;
                             else this._textureUniforms[e] && delete this._textureUniforms[e];
-                            (i(t) || r) && Lp(this.uniforms, e, n)
+                            (i(t) || r) && Rp(this.uniforms, e, n)
                         }
                     }
                     return this
                 }
                 _areTexturesRenderable() {
                     let t = !0;
                     for (const e in this._textureUniforms) {
@@ -13389,32 +13392,32 @@
                     this.gl.deleteProgram(this.handle)
                 }
                 _getOptionsFromHandle(t) {
                     const e = this.gl.getAttachedShaders(t),
                         n = {};
                     for (const t of e) switch (this.gl.getShaderParameter(this.handle, 35663)) {
                         case 35633:
-                            n.vs = new Np({
+                            n.vs = new Vp({
                                 handle: t
                             });
                             break;
                         case 35632:
-                            n.fs = new Vp({
+                            n.fs = new Up({
                                 handle: t
                             })
                     }
                     return n
                 }
                 _getParameter(t) {
                     return this.gl.getProgramParameter(this.handle, t)
                 }
                 _setId(t) {
                     if (!t) {
                         const t = this._getName();
-                        this.id = Td(t)
+                        this.id = Ad(t)
                     }
                 }
                 _getName() {
                     let t = this.vs.getName() || this.fs.getName();
                     return t = t.replace(/shader/i, ""), t = t ? "".concat(t, "-program") : "program", t
                 }
                 _compileAndLink() {
@@ -13431,18 +13434,18 @@
                         gl: t
                     } = this;
                     this._uniformSetters = {}, this._uniformCount = this._getParameter(35718);
                     for (let e = 0; e < this._uniformCount; e++) {
                         const n = this.gl.getActiveUniform(this.handle, e),
                             {
                                 name: i
-                            } = Mp(n.name);
+                            } = Op(n.name);
                         let r = t.getUniformLocation(this.handle, i);
-                        if (this._uniformSetters[i] = Ap(t, r, n), n.size > 1)
-                            for (let e = 0; e < n.size; e++) r = t.getUniformLocation(this.handle, "".concat(i, "[").concat(e, "]")), this._uniformSetters["".concat(i, "[").concat(e, "]")] = Ap(t, r, n)
+                        if (this._uniformSetters[i] = Mp(t, r, n), n.size > 1)
+                            for (let e = 0; e < n.size; e++) r = t.getUniformLocation(this.handle, "".concat(i, "[").concat(e, "]")), this._uniformSetters["".concat(i, "[").concat(e, "]")] = Mp(t, r, n)
                     }
                     this._textureIndexCounter = 0
                 }
                 getActiveUniforms(t, e) {
                     return this.gl2.getActiveUniforms(this.handle, t, e)
                 }
                 getUniformBlockIndex(t) {
@@ -13451,17 +13454,17 @@
                 getActiveUniformBlockParameter(t, e) {
                     return this.gl2.getActiveUniformBlockParameter(this.handle, t, e)
                 }
                 uniformBlockBinding(t, e) {
                     this.gl2.uniformBlockBinding(this.handle, t, e)
                 }
             }
-            class nf {
+            class rf {
                 static getDefaultProgramManager(t) {
-                    return t.luma = t.luma || {}, t.luma.defaultProgramManager = t.luma.defaultProgramManager || new nf(t), t.luma.defaultProgramManager
+                    return t.luma = t.luma || {}, t.luma.defaultProgramManager = t.luma.defaultProgramManager || new rf(t), t.luma.defaultProgramManager
                 }
                 constructor(t) {
                     this.gl = t, this._programCache = {}, this._getUniforms = {}, this._registeredModules = {}, this._hookFunctions = [], this._defaultModules = [], this._hashes = {}, this._hashCounter = 0, this.stateHash = 0, this._useCounts = {}
                 }
                 addDefaultModule(t) {
                     this._defaultModules.find((e => e.name === t.name)) || this._defaultModules.push(t), this.stateHash++
                 }
@@ -13513,15 +13516,15 @@
                             fs: n,
                             modules: l,
                             inject: r,
                             defines: i,
                             hookFunctions: this._hookFunctions,
                             transpileToGLSL100: a
                         });
-                        this._programCache[v] = new ef(this.gl, {
+                        this._programCache[v] = new nf(this.gl, {
                             hash: v,
                             vs: t.vs,
                             fs: t.fs,
                             varyings: s,
                             bufferMode: o
                         }), this._getUniforms[v] = t.getUniforms || (t => {}), this._useCounts[v] = 0
                     }
@@ -13551,53 +13554,53 @@
                         const s = t[r],
                             o = s.name;
                         n[o] || (e[i++] = s, n[o] = !0)
                     }
                     return e.length = i, e
                 }
             }
-            const rf = "#define SMOOTH_EDGE_RADIUS 0.5",
-                sf = {
+            const sf = "#define SMOOTH_EDGE_RADIUS 0.5",
+                of = {
                     name: "geometry",
-                    vs: "\n".concat(rf, "\n\nstruct VertexGeometry {\n  vec4 position;\n  vec3 worldPosition;\n  vec3 worldPositionAlt;\n  vec3 normal;\n  vec2 uv;\n  vec3 pickingColor;\n} geometry = VertexGeometry(\n  vec4(0.0, 0.0, 1.0, 0.0),\n  vec3(0.0),\n  vec3(0.0),\n  vec3(0.0),\n  vec2(0.0),\n  vec3(0.0)\n);\n"),
-                    fs: "\n".concat(rf, "\n\nstruct FragmentGeometry {\n  vec2 uv;\n} geometry;\n\nfloat smoothedge(float edge, float x) {\n  return smoothstep(edge - SMOOTH_EDGE_RADIUS, edge + SMOOTH_EDGE_RADIUS, x);\n}\n")
+                    vs: "\n".concat(sf, "\n\nstruct VertexGeometry {\n  vec4 position;\n  vec3 worldPosition;\n  vec3 worldPositionAlt;\n  vec3 normal;\n  vec2 uv;\n  vec3 pickingColor;\n} geometry = VertexGeometry(\n  vec4(0.0, 0.0, 1.0, 0.0),\n  vec3(0.0),\n  vec3(0.0),\n  vec3(0.0),\n  vec2(0.0),\n  vec3(0.0)\n);\n"),
+                    fs: "\n".concat(sf, "\n\nstruct FragmentGeometry {\n  vec2 uv;\n} geometry;\n\nfloat smoothedge(float edge, float x) {\n  return smoothstep(edge - SMOOTH_EDGE_RADIUS, edge + SMOOTH_EDGE_RADIUS, x);\n}\n")
                 },
-                of = Object.keys(Lh).map((t => "const int COORDINATE_SYSTEM_".concat(t, " = ").concat(Lh[t], ";"))).join(""),
-                af = Object.keys(Rh).map((t => "const int PROJECTION_MODE_".concat(t, " = ").concat(Rh[t], ";"))).join(""),
-                lf = Object.keys(Ih).map((t => "const int UNIT_".concat(t.toUpperCase(), " = ").concat(Ih[t], ";"))).join(""),
-                cf = "".concat(of, "\n").concat(af, "\n").concat(lf, "\n\nuniform int project_uCoordinateSystem;\nuniform int project_uProjectionMode;\nuniform float project_uScale;\nuniform bool project_uWrapLongitude;\nuniform vec3 project_uCommonUnitsPerMeter;\nuniform vec3 project_uCommonUnitsPerWorldUnit;\nuniform vec3 project_uCommonUnitsPerWorldUnit2;\nuniform vec4 project_uCenter;\nuniform mat4 project_uModelMatrix;\nuniform mat4 project_uViewProjectionMatrix;\nuniform vec2 project_uViewportSize;\nuniform float project_uDevicePixelRatio;\nuniform float project_uFocalDistance;\nuniform vec3 project_uCameraPosition;\nuniform vec3 project_uCoordinateOrigin;\nuniform vec3 project_uCommonOrigin;\nuniform bool project_uPseudoMeters;\n\nconst float TILE_SIZE = 512.0;\nconst float PI = 3.1415926536;\nconst float WORLD_SCALE = TILE_SIZE / (PI * 2.0);\nconst vec3 ZERO_64_LOW = vec3(0.0);\nconst float EARTH_RADIUS = 6370972.0;\nconst float GLOBE_RADIUS = 256.0;\nfloat project_size_at_latitude(float lat) {\n  float y = clamp(lat, -89.9, 89.9);\n  return 1.0 / cos(radians(y));\n}\n\nfloat project_size() {\n  if (project_uProjectionMode == PROJECTION_MODE_WEB_MERCATOR &&\n    project_uCoordinateSystem == COORDINATE_SYSTEM_LNGLAT &&\n    project_uPseudoMeters == false) {\n    \n    if (geometry.position.w == 0.0) {\n      return project_size_at_latitude(geometry.worldPosition.y);\n    }\n  \n    float y = geometry.position.y / TILE_SIZE * 2.0 - 1.0;\n    float y2 = y * y;\n    float y4 = y2 * y2;\n    float y6 = y4 * y2;\n    return 1.0 + 4.9348 * y2 + 4.0587 * y4 + 1.5642 * y6;\n  }\n  return 1.0;\n}\n\nfloat project_size_at_latitude(float meters, float lat) {\n  return meters * project_uCommonUnitsPerMeter.z * project_size_at_latitude(lat);\n}\nfloat project_size(float meters) {\n  return meters * project_uCommonUnitsPerMeter.z * project_size();\n}\n\nvec2 project_size(vec2 meters) {\n  return meters * project_uCommonUnitsPerMeter.xy * project_size();\n}\n\nvec3 project_size(vec3 meters) {\n  return meters * project_uCommonUnitsPerMeter * project_size();\n}\n\nvec4 project_size(vec4 meters) {\n  return vec4(meters.xyz * project_uCommonUnitsPerMeter, meters.w);\n}\nmat3 project_get_orientation_matrix(vec3 up) {\n  vec3 uz = normalize(up);\n  vec3 ux = abs(uz.z) == 1.0 ? vec3(1.0, 0.0, 0.0) : normalize(vec3(uz.y, -uz.x, 0));\n  vec3 uy = cross(uz, ux);\n  return mat3(ux, uy, uz);\n}\n\nbool project_needs_rotation(vec3 commonPosition, out mat3 transform) {\n  if (project_uProjectionMode == PROJECTION_MODE_GLOBE) {\n    transform = project_get_orientation_matrix(commonPosition);\n    return true;\n  }\n  return false;\n}\nvec3 project_normal(vec3 vector) {\n  vec4 normal_modelspace = project_uModelMatrix * vec4(vector, 0.0);\n  vec3 n = normalize(normal_modelspace.xyz * project_uCommonUnitsPerMeter);\n  mat3 rotation;\n  if (project_needs_rotation(geometry.position.xyz, rotation)) {\n    n = rotation * n;\n  }\n  return n;\n}\n\nvec4 project_offset_(vec4 offset) {\n  float dy = offset.y;\n  vec3 commonUnitsPerWorldUnit = project_uCommonUnitsPerWorldUnit + project_uCommonUnitsPerWorldUnit2 * dy;\n  return vec4(offset.xyz * commonUnitsPerWorldUnit, offset.w);\n}\nvec2 project_mercator_(vec2 lnglat) {\n  float x = lnglat.x;\n  if (project_uWrapLongitude) {\n    x = mod(x + 180., 360.0) - 180.;\n  }\n  float y = clamp(lnglat.y, -89.9, 89.9);\n  return vec2(\n    radians(x) + PI,\n    PI + log(tan_fp32(PI * 0.25 + radians(y) * 0.5))\n  ) * WORLD_SCALE;\n}\n\nvec3 project_globe_(vec3 lnglatz) {\n  float lambda = radians(lnglatz.x);\n  float phi = radians(lnglatz.y);\n  float cosPhi = cos(phi);\n  float D = (lnglatz.z / EARTH_RADIUS + 1.0) * GLOBE_RADIUS;\n\n  return vec3(\n    sin(lambda) * cosPhi,\n    -cos(lambda) * cosPhi,\n    sin(phi)\n  ) * D;\n}\nvec4 project_position(vec4 position, vec3 position64Low) {\n  vec4 position_world = project_uModelMatrix * position;\n  if (project_uProjectionMode == PROJECTION_MODE_WEB_MERCATOR) {\n    if (project_uCoordinateSystem == COORDINATE_SYSTEM_LNGLAT) {\n      return vec4(\n        project_mercator_(position_world.xy),\n        project_size_at_latitude(position_world.z, position_world.y),\n        position_world.w\n      );\n    }\n    if (project_uCoordinateSystem == COORDINATE_SYSTEM_CARTESIAN) {\n      position_world.xyz += project_uCoordinateOrigin;\n    }\n  }\n  if (project_uProjectionMode == PROJECTION_MODE_GLOBE) {\n    if (project_uCoordinateSystem == COORDINATE_SYSTEM_LNGLAT) {\n      return vec4(\n        project_globe_(position_world.xyz),\n        position_world.w\n      );\n    }\n  }\n  if (project_uProjectionMode == PROJECTION_MODE_WEB_MERCATOR_AUTO_OFFSET) {\n    if (project_uCoordinateSystem == COORDINATE_SYSTEM_LNGLAT) {\n      if (abs(position_world.y - project_uCoordinateOrigin.y) > 0.25) {\n        return vec4(\n          project_mercator_(position_world.xy) - project_uCommonOrigin.xy,\n          project_size(position_world.z),\n          position_world.w\n        );\n      }\n    }\n  }\n  if (project_uProjectionMode == PROJECTION_MODE_IDENTITY ||\n    (project_uProjectionMode == PROJECTION_MODE_WEB_MERCATOR_AUTO_OFFSET &&\n    (project_uCoordinateSystem == COORDINATE_SYSTEM_LNGLAT ||\n     project_uCoordinateSystem == COORDINATE_SYSTEM_CARTESIAN))) {\n    position_world.xyz -= project_uCoordinateOrigin;\n  }\n  return project_offset_(position_world + project_uModelMatrix * vec4(position64Low, 0.0));\n}\n\nvec4 project_position(vec4 position) {\n  return project_position(position, ZERO_64_LOW);\n}\n\nvec3 project_position(vec3 position, vec3 position64Low) {\n  vec4 projected_position = project_position(vec4(position, 1.0), position64Low);\n  return projected_position.xyz;\n}\n\nvec3 project_position(vec3 position) {\n  vec4 projected_position = project_position(vec4(position, 1.0), ZERO_64_LOW);\n  return projected_position.xyz;\n}\n\nvec2 project_position(vec2 position) {\n  vec4 projected_position = project_position(vec4(position, 0.0, 1.0), ZERO_64_LOW);\n  return projected_position.xy;\n}\n\nvec4 project_common_position_to_clipspace(vec4 position, mat4 viewProjectionMatrix, vec4 center) {\n  return viewProjectionMatrix * position + center;\n}\nvec4 project_common_position_to_clipspace(vec4 position) {\n  return project_common_position_to_clipspace(position, project_uViewProjectionMatrix, project_uCenter);\n}\nvec2 project_pixel_size_to_clipspace(vec2 pixels) {\n  vec2 offset = pixels / project_uViewportSize * project_uDevicePixelRatio * 2.0;\n  return offset * project_uFocalDistance;\n}\n\nfloat project_size_to_pixel(float meters) {\n  return project_size(meters) * project_uScale;\n}\nfloat project_size_to_pixel(float size, int unit) {\n  if (unit == UNIT_METERS) return project_size_to_pixel(size);\n  if (unit == UNIT_COMMON) return size * project_uScale;\n  return size;\n}\nfloat project_pixel_size(float pixels) {\n  return pixels / project_uScale;\n}\nvec2 project_pixel_size(vec2 pixels) {\n  return pixels / project_uScale;\n}\n");
+                af = Object.keys(Lh).map((t => "const int COORDINATE_SYSTEM_".concat(t, " = ").concat(Lh[t], ";"))).join(""),
+                lf = Object.keys(Rh).map((t => "const int PROJECTION_MODE_".concat(t, " = ").concat(Rh[t], ";"))).join(""),
+                cf = Object.keys(Ih).map((t => "const int UNIT_".concat(t.toUpperCase(), " = ").concat(Ih[t], ";"))).join(""),
+                hf = "".concat(af, "\n").concat(lf, "\n").concat(cf, "\n\nuniform int project_uCoordinateSystem;\nuniform int project_uProjectionMode;\nuniform float project_uScale;\nuniform bool project_uWrapLongitude;\nuniform vec3 project_uCommonUnitsPerMeter;\nuniform vec3 project_uCommonUnitsPerWorldUnit;\nuniform vec3 project_uCommonUnitsPerWorldUnit2;\nuniform vec4 project_uCenter;\nuniform mat4 project_uModelMatrix;\nuniform mat4 project_uViewProjectionMatrix;\nuniform vec2 project_uViewportSize;\nuniform float project_uDevicePixelRatio;\nuniform float project_uFocalDistance;\nuniform vec3 project_uCameraPosition;\nuniform vec3 project_uCoordinateOrigin;\nuniform vec3 project_uCommonOrigin;\nuniform bool project_uPseudoMeters;\n\nconst float TILE_SIZE = 512.0;\nconst float PI = 3.1415926536;\nconst float WORLD_SCALE = TILE_SIZE / (PI * 2.0);\nconst vec3 ZERO_64_LOW = vec3(0.0);\nconst float EARTH_RADIUS = 6370972.0;\nconst float GLOBE_RADIUS = 256.0;\nfloat project_size_at_latitude(float lat) {\n  float y = clamp(lat, -89.9, 89.9);\n  return 1.0 / cos(radians(y));\n}\n\nfloat project_size() {\n  if (project_uProjectionMode == PROJECTION_MODE_WEB_MERCATOR &&\n    project_uCoordinateSystem == COORDINATE_SYSTEM_LNGLAT &&\n    project_uPseudoMeters == false) {\n    \n    if (geometry.position.w == 0.0) {\n      return project_size_at_latitude(geometry.worldPosition.y);\n    }\n  \n    float y = geometry.position.y / TILE_SIZE * 2.0 - 1.0;\n    float y2 = y * y;\n    float y4 = y2 * y2;\n    float y6 = y4 * y2;\n    return 1.0 + 4.9348 * y2 + 4.0587 * y4 + 1.5642 * y6;\n  }\n  return 1.0;\n}\n\nfloat project_size_at_latitude(float meters, float lat) {\n  return meters * project_uCommonUnitsPerMeter.z * project_size_at_latitude(lat);\n}\nfloat project_size(float meters) {\n  return meters * project_uCommonUnitsPerMeter.z * project_size();\n}\n\nvec2 project_size(vec2 meters) {\n  return meters * project_uCommonUnitsPerMeter.xy * project_size();\n}\n\nvec3 project_size(vec3 meters) {\n  return meters * project_uCommonUnitsPerMeter * project_size();\n}\n\nvec4 project_size(vec4 meters) {\n  return vec4(meters.xyz * project_uCommonUnitsPerMeter, meters.w);\n}\nmat3 project_get_orientation_matrix(vec3 up) {\n  vec3 uz = normalize(up);\n  vec3 ux = abs(uz.z) == 1.0 ? vec3(1.0, 0.0, 0.0) : normalize(vec3(uz.y, -uz.x, 0));\n  vec3 uy = cross(uz, ux);\n  return mat3(ux, uy, uz);\n}\n\nbool project_needs_rotation(vec3 commonPosition, out mat3 transform) {\n  if (project_uProjectionMode == PROJECTION_MODE_GLOBE) {\n    transform = project_get_orientation_matrix(commonPosition);\n    return true;\n  }\n  return false;\n}\nvec3 project_normal(vec3 vector) {\n  vec4 normal_modelspace = project_uModelMatrix * vec4(vector, 0.0);\n  vec3 n = normalize(normal_modelspace.xyz * project_uCommonUnitsPerMeter);\n  mat3 rotation;\n  if (project_needs_rotation(geometry.position.xyz, rotation)) {\n    n = rotation * n;\n  }\n  return n;\n}\n\nvec4 project_offset_(vec4 offset) {\n  float dy = offset.y;\n  vec3 commonUnitsPerWorldUnit = project_uCommonUnitsPerWorldUnit + project_uCommonUnitsPerWorldUnit2 * dy;\n  return vec4(offset.xyz * commonUnitsPerWorldUnit, offset.w);\n}\nvec2 project_mercator_(vec2 lnglat) {\n  float x = lnglat.x;\n  if (project_uWrapLongitude) {\n    x = mod(x + 180., 360.0) - 180.;\n  }\n  float y = clamp(lnglat.y, -89.9, 89.9);\n  return vec2(\n    radians(x) + PI,\n    PI + log(tan_fp32(PI * 0.25 + radians(y) * 0.5))\n  ) * WORLD_SCALE;\n}\n\nvec3 project_globe_(vec3 lnglatz) {\n  float lambda = radians(lnglatz.x);\n  float phi = radians(lnglatz.y);\n  float cosPhi = cos(phi);\n  float D = (lnglatz.z / EARTH_RADIUS + 1.0) * GLOBE_RADIUS;\n\n  return vec3(\n    sin(lambda) * cosPhi,\n    -cos(lambda) * cosPhi,\n    sin(phi)\n  ) * D;\n}\nvec4 project_position(vec4 position, vec3 position64Low) {\n  vec4 position_world = project_uModelMatrix * position;\n  if (project_uProjectionMode == PROJECTION_MODE_WEB_MERCATOR) {\n    if (project_uCoordinateSystem == COORDINATE_SYSTEM_LNGLAT) {\n      return vec4(\n        project_mercator_(position_world.xy),\n        project_size_at_latitude(position_world.z, position_world.y),\n        position_world.w\n      );\n    }\n    if (project_uCoordinateSystem == COORDINATE_SYSTEM_CARTESIAN) {\n      position_world.xyz += project_uCoordinateOrigin;\n    }\n  }\n  if (project_uProjectionMode == PROJECTION_MODE_GLOBE) {\n    if (project_uCoordinateSystem == COORDINATE_SYSTEM_LNGLAT) {\n      return vec4(\n        project_globe_(position_world.xyz),\n        position_world.w\n      );\n    }\n  }\n  if (project_uProjectionMode == PROJECTION_MODE_WEB_MERCATOR_AUTO_OFFSET) {\n    if (project_uCoordinateSystem == COORDINATE_SYSTEM_LNGLAT) {\n      if (abs(position_world.y - project_uCoordinateOrigin.y) > 0.25) {\n        return vec4(\n          project_mercator_(position_world.xy) - project_uCommonOrigin.xy,\n          project_size(position_world.z),\n          position_world.w\n        );\n      }\n    }\n  }\n  if (project_uProjectionMode == PROJECTION_MODE_IDENTITY ||\n    (project_uProjectionMode == PROJECTION_MODE_WEB_MERCATOR_AUTO_OFFSET &&\n    (project_uCoordinateSystem == COORDINATE_SYSTEM_LNGLAT ||\n     project_uCoordinateSystem == COORDINATE_SYSTEM_CARTESIAN))) {\n    position_world.xyz -= project_uCoordinateOrigin;\n  }\n  return project_offset_(position_world + project_uModelMatrix * vec4(position64Low, 0.0));\n}\n\nvec4 project_position(vec4 position) {\n  return project_position(position, ZERO_64_LOW);\n}\n\nvec3 project_position(vec3 position, vec3 position64Low) {\n  vec4 projected_position = project_position(vec4(position, 1.0), position64Low);\n  return projected_position.xyz;\n}\n\nvec3 project_position(vec3 position) {\n  vec4 projected_position = project_position(vec4(position, 1.0), ZERO_64_LOW);\n  return projected_position.xyz;\n}\n\nvec2 project_position(vec2 position) {\n  vec4 projected_position = project_position(vec4(position, 0.0, 1.0), ZERO_64_LOW);\n  return projected_position.xy;\n}\n\nvec4 project_common_position_to_clipspace(vec4 position, mat4 viewProjectionMatrix, vec4 center) {\n  return viewProjectionMatrix * position + center;\n}\nvec4 project_common_position_to_clipspace(vec4 position) {\n  return project_common_position_to_clipspace(position, project_uViewProjectionMatrix, project_uCenter);\n}\nvec2 project_pixel_size_to_clipspace(vec2 pixels) {\n  vec2 offset = pixels / project_uViewportSize * project_uDevicePixelRatio * 2.0;\n  return offset * project_uFocalDistance;\n}\n\nfloat project_size_to_pixel(float meters) {\n  return project_size(meters) * project_uScale;\n}\nfloat project_size_to_pixel(float size, int unit) {\n  if (unit == UNIT_METERS) return project_size_to_pixel(size);\n  if (unit == UNIT_COMMON) return size * project_uScale;\n  return size;\n}\nfloat project_pixel_size(float pixels) {\n  return pixels / project_uScale;\n}\nvec2 project_pixel_size(vec2 pixels) {\n  return pixels / project_uScale;\n}\n");
 
-            function hf(t, e) {
+            function uf(t, e) {
                 if (t === e) return !0;
                 if (Array.isArray(t)) {
                     const n = t.length;
                     if (!e || e.length !== n) return !1;
                     for (let i = 0; i < n; i++)
                         if (t[i] !== e[i]) return !1;
                     return !0
                 }
                 return !1
             }
 
-            function uf(t) {
+            function df(t) {
                 let e, n = {};
                 return i => {
                     for (const r in i)
-                        if (!hf(i[r], n[r])) {
+                        if (!uf(i[r], n[r])) {
                             e = t(i), n = i;
                             break
                         } return e
                 }
             }
-            const df = [0, 0, 0, 0],
-                pf = [1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0],
-                ff = [1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1],
-                gf = [0, 0, 0],
+            const pf = [0, 0, 0, 0],
+                ff = [1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0],
+                gf = [1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1],
                 mf = [0, 0, 0],
-                vf = uf((function({
+                vf = [0, 0, 0],
+                bf = df((function({
                     viewport: t,
                     devicePixelRatio: e,
                     coordinateSystem: n,
                     coordinateOrigin: i
                 }) {
                     const {
                         projectionCenter: r,
@@ -13610,21 +13613,21 @@
                         const {
                             viewMatrixUncentered: i,
                             projectionMatrix: r
                         } = t;
                         let {
                             viewMatrix: s,
                             viewProjectionMatrix: o
-                        } = t, a = df, l = df, c = t.cameraPosition;
+                        } = t, a = pf, l = pf, c = t.cameraPosition;
                         const {
                             geospatialOrigin: h,
                             shaderCoordinateOrigin: u,
                             offsetMode: d
-                        } = bf(t, e, n);
-                        return d && (l = t.projectPosition(h || u), c = [c[0] - l[0], c[1] - l[1], c[2] - l[2]], l[3] = 1, a = Qc([], l, o), s = i || s, o = Vc([], r, s), o = Vc([], o, pf)), {
+                        } = yf(t, e, n);
+                        return d && (l = t.projectPosition(h || u), c = [c[0] - l[0], c[1] - l[1], c[2] - l[2]], l[3] = 1, a = Qc([], l, o), s = i || s, o = Vc([], r, s), o = Vc([], o, ff)), {
                             viewMatrix: s,
                             viewProjectionMatrix: o,
                             projectionCenter: a,
                             originCommon: l,
                             cameraPosCommon: c,
                             shaderCoordinateOrigin: u,
                             geospatialOrigin: h
@@ -13637,19 +13640,19 @@
                         project_uCenter: r,
                         project_uPseudoMeters: Boolean(t._pseudoMeters),
                         project_uViewportSize: u,
                         project_uDevicePixelRatio: e,
                         project_uFocalDistance: d,
                         project_uCommonUnitsPerMeter: h.unitsPerMeter,
                         project_uCommonUnitsPerWorldUnit: h.unitsPerMeter,
-                        project_uCommonUnitsPerWorldUnit2: gf,
+                        project_uCommonUnitsPerWorldUnit2: mf,
                         project_uScale: t.scale,
                         project_uWrapLongitude: !1,
                         project_uViewProjectionMatrix: s,
-                        project_uModelMatrix: ff,
+                        project_uModelMatrix: gf,
                         project_uCameraPosition: a
                     };
                     if (c) {
                         const e = t.getDistanceScales(c);
                         switch (n) {
                             case Lh.METER_OFFSETS:
                                 p.project_uCommonUnitsPerWorldUnit = e.unitsPerMeter, p.project_uCommonUnitsPerWorldUnit2 = e.unitsPerMeter2;
@@ -13661,15 +13664,15 @@
                             case Lh.CARTESIAN:
                                 p.project_uCommonUnitsPerWorldUnit = [1, 1, e.unitsPerMeter[2]], p.project_uCommonUnitsPerWorldUnit2 = [0, 0, e.unitsPerMeter2[2]]
                         }
                     }
                     return p
                 }));
 
-            function bf(t, e, n = mf) {
+            function yf(t, e, n = vf) {
                 n.length < 3 && (n = [n[0], n[1], 0]);
                 let i, r = n,
                     s = !0;
                 switch (i = e === Lh.LNGLAT_OFFSETS || e === Lh.METER_OFFSETS ? n : t.isGeospatial ? [Math.fround(t.longitude), Math.fround(t.latitude), 0] : null, t.projectionMode) {
                     case Rh.WEB_MERCATOR:
                         e !== Lh.LNGLAT && e !== Lh.CARTESIAN || (i = [0, 0, 0], s = !1);
                         break;
@@ -13687,53 +13690,53 @@
                 }
                 return {
                     geospatialOrigin: i,
                     shaderCoordinateOrigin: r,
                     offsetMode: s
                 }
             }
-            const yf = {},
-                _f = {
+            const _f = {},
+                xf = {
                     name: "project",
                     dependencies: [{
                         name: "fp32",
                         vs: "#ifdef LUMA_FP32_TAN_PRECISION_WORKAROUND\nconst float TWO_PI = 6.2831854820251465;\nconst float PI_2 = 1.5707963705062866;\nconst float PI_16 = 0.1963495463132858;\n\nconst float SIN_TABLE_0 = 0.19509032368659973;\nconst float SIN_TABLE_1 = 0.3826834261417389;\nconst float SIN_TABLE_2 = 0.5555702447891235;\nconst float SIN_TABLE_3 = 0.7071067690849304;\n\nconst float COS_TABLE_0 = 0.9807852506637573;\nconst float COS_TABLE_1 = 0.9238795042037964;\nconst float COS_TABLE_2 = 0.8314695954322815;\nconst float COS_TABLE_3 = 0.7071067690849304;\n\nconst float INVERSE_FACTORIAL_3 = 1.666666716337204e-01;\nconst float INVERSE_FACTORIAL_5 = 8.333333767950535e-03;\nconst float INVERSE_FACTORIAL_7 = 1.9841270113829523e-04;\nconst float INVERSE_FACTORIAL_9 = 2.75573188446287533e-06;\n\nfloat sin_taylor_fp32(float a) {\n  float r, s, t, x;\n\n  if (a == 0.0) {\n    return 0.0;\n  }\n\n  x = -a * a;\n  s = a;\n  r = a;\n\n  r = r * x;\n  t = r * INVERSE_FACTORIAL_3;\n  s = s + t;\n\n  r = r * x;\n  t = r * INVERSE_FACTORIAL_5;\n  s = s + t;\n\n  r = r * x;\n  t = r * INVERSE_FACTORIAL_7;\n  s = s + t;\n\n  r = r * x;\n  t = r * INVERSE_FACTORIAL_9;\n  s = s + t;\n\n  return s;\n}\n\nvoid sincos_taylor_fp32(float a, out float sin_t, out float cos_t) {\n  if (a == 0.0) {\n    sin_t = 0.0;\n    cos_t = 1.0;\n  }\n  sin_t = sin_taylor_fp32(a);\n  cos_t = sqrt(1.0 - sin_t * sin_t);\n}\n\nfloat tan_taylor_fp32(float a) {\n    float sin_a;\n    float cos_a;\n\n    if (a == 0.0) {\n        return 0.0;\n    }\n    float z = floor(a / TWO_PI);\n    float r = a - TWO_PI * z;\n\n    float t;\n    float q = floor(r / PI_2 + 0.5);\n    int j = int(q);\n\n    if (j < -2 || j > 2) {\n        return 1.0 / 0.0;\n    }\n\n    t = r - PI_2 * q;\n\n    q = floor(t / PI_16 + 0.5);\n    int k = int(q);\n    int abs_k = int(abs(float(k)));\n\n    if (abs_k > 4) {\n        return 1.0 / 0.0;\n    } else {\n        t = t - PI_16 * q;\n    }\n\n    float u = 0.0;\n    float v = 0.0;\n\n    float sin_t, cos_t;\n    float s, c;\n    sincos_taylor_fp32(t, sin_t, cos_t);\n\n    if (k == 0) {\n        s = sin_t;\n        c = cos_t;\n    } else {\n        if (abs(float(abs_k) - 1.0) < 0.5) {\n            u = COS_TABLE_0;\n            v = SIN_TABLE_0;\n        } else if (abs(float(abs_k) - 2.0) < 0.5) {\n            u = COS_TABLE_1;\n            v = SIN_TABLE_1;\n        } else if (abs(float(abs_k) - 3.0) < 0.5) {\n            u = COS_TABLE_2;\n            v = SIN_TABLE_2;\n        } else if (abs(float(abs_k) - 4.0) < 0.5) {\n            u = COS_TABLE_3;\n            v = SIN_TABLE_3;\n        }\n        if (k > 0) {\n            s = u * sin_t + v * cos_t;\n            c = u * cos_t - v * sin_t;\n        } else {\n            s = u * sin_t - v * cos_t;\n            c = u * cos_t + v * sin_t;\n        }\n    }\n\n    if (j == 0) {\n        sin_a = s;\n        cos_a = c;\n    } else if (j == 1) {\n        sin_a = c;\n        cos_a = -s;\n    } else if (j == -1) {\n        sin_a = -c;\n        cos_a = s;\n    } else {\n        sin_a = -s;\n        cos_a = -c;\n    }\n    return sin_a / cos_a;\n}\n#endif\n\nfloat tan_fp32(float a) {\n#ifdef LUMA_FP32_TAN_PRECISION_WORKAROUND\n  return tan_taylor_fp32(a);\n#else\n  return tan(a);\n#endif\n}\n",
                         fs: null
-                    }, sf],
-                    vs: cf,
-                    getUniforms: function(t = yf) {
+                    }, of],
+                    vs: hf,
+                    getUniforms: function(t = _f) {
                         return "viewport" in t ? function({
                             viewport: t,
                             devicePixelRatio: e = 1,
                             modelMatrix: n = null,
                             coordinateSystem: i = Lh.DEFAULT,
-                            coordinateOrigin: r = mf,
+                            coordinateOrigin: r = vf,
                             autoWrapLongitude: s = !1
                         }) {
                             i === Lh.DEFAULT && (i = t.isGeospatial ? Lh.LNGLAT : Lh.CARTESIAN);
-                            const o = vf({
+                            const o = bf({
                                 viewport: t,
                                 devicePixelRatio: e,
                                 coordinateSystem: i,
                                 coordinateOrigin: r
                             });
-                            return o.project_uWrapLongitude = s, o.project_uModelMatrix = n || ff, o
+                            return o.project_uWrapLongitude = s, o.project_uModelMatrix = n || gf, o
                         }(t) : {}
                     }
                 },
-                xf = [_f],
-                wf = ["vs:DECKGL_FILTER_SIZE(inout vec3 size, VertexGeometry geometry)", "vs:DECKGL_FILTER_GL_POSITION(inout vec4 position, VertexGeometry geometry)", "vs:DECKGL_FILTER_COLOR(inout vec4 color, VertexGeometry geometry)", "fs:DECKGL_FILTER_COLOR(inout vec4 color, FragmentGeometry geometry)"];
+                wf = [xf],
+                Ef = ["vs:DECKGL_FILTER_SIZE(inout vec3 size, VertexGeometry geometry)", "vs:DECKGL_FILTER_GL_POSITION(inout vec4 position, VertexGeometry geometry)", "vs:DECKGL_FILTER_COLOR(inout vec4 color, VertexGeometry geometry)", "fs:DECKGL_FILTER_COLOR(inout vec4 color, FragmentGeometry geometry)"];
 
-            function Ef(t) {
-                const e = nf.getDefaultProgramManager(t);
-                for (const t of xf) e.addDefaultModule(t);
-                for (const t of wf) e.addShaderHook(t);
+            function Pf(t) {
+                const e = rf.getDefaultProgramManager(t);
+                for (const t of wf) e.addDefaultModule(t);
+                for (const t of Ef) e.addShaderHook(t);
                 return e
             }
-            class Pf {
+            class Sf {
                 constructor(t, {
                     deck: e,
                     stats: n,
                     viewport: i,
                     timeline: r
                 } = {}) {
                     wo(this, "layers", void 0), wo(this, "context", void 0), wo(this, "resourceManager", void 0), wo(this, "_lastRenderedLayers", []), wo(this, "_needsRedraw", !1), wo(this, "_needsUpdate", !1), wo(this, "_nextLayers", null), wo(this, "_debug", !1), wo(this, "activateViewport", (t => {
@@ -13743,15 +13746,15 @@
                         protocol: "deck://"
                     }), this.context = {
                         mousePosition: null,
                         userData: {},
                         layerManager: this,
                         gl: t,
                         deck: e,
-                        programManager: t && Ef(t),
+                        programManager: t && Pf(t),
                         stats: n || new da({
                             id: "deck.gl"
                         }),
                         viewport: i || new Dh({
                             id: "DEFAULT-INITIAL-VIEWPORT"
                         }),
                         timeline: r || new So,
@@ -13859,37 +13862,37 @@
                         t._finalize(), t.lifecycle = "Finalized! Awaiting garbage collection"
                     } catch (e) {
                         this._handleError("finalization", e, t)
                     }
                 }
             }
 
-            function Sf(t, e, n) {
+            function Cf(t, e, n) {
                 if (t === e) return !0;
                 if (!n || !t || !e) return !1;
                 if (Array.isArray(t)) {
                     if (!Array.isArray(e) || t.length !== e.length) return !1;
                     for (let i = 0; i < t.length; i++)
-                        if (!Sf(t[i], e[i], n - 1)) return !1;
+                        if (!Cf(t[i], e[i], n - 1)) return !1;
                     return !0
                 }
                 if (Array.isArray(e)) return !1;
                 if ("object" == typeof t && "object" == typeof e) {
                     const i = Object.keys(t),
                         r = Object.keys(e);
                     if (i.length !== r.length) return !1;
                     for (const r of i) {
                         if (!e.hasOwnProperty(r)) return !1;
-                        if (!Sf(t[r], e[r], n - 1)) return !1
+                        if (!Cf(t[r], e[r], n - 1)) return !1
                     }
                     return !0
                 }
                 return !1
             }
-            class Cf {
+            class Tf {
                 constructor(t) {
                     wo(this, "width", void 0), wo(this, "height", void 0), wo(this, "views", void 0), wo(this, "viewState", void 0), wo(this, "controllers", void 0), wo(this, "timeline", void 0), wo(this, "_viewports", void 0), wo(this, "_viewportMap", void 0), wo(this, "_isUpdating", void 0), wo(this, "_needsRedraw", void 0), wo(this, "_needsUpdate", void 0), wo(this, "_eventManager", void 0), wo(this, "_eventCallbacks", void 0), this.views = [], this.width = 100, this.height = 100, this.viewState = {}, this.controllers = {}, this.timeline = t.timeline, this._viewports = [], this._viewportMap = {}, this._isUpdating = !1, this._needsRedraw = "First render", this._needsUpdate = "Initialize", this._eventManager = t.eventManager, this._eventCallbacks = {
                         onViewStateChange: t.onViewStateChange,
                         onInteractionStateChange: t.onInteractionStateChange
                     }, Object.seal(this), this.setProps(t)
                 }
                 finalize() {
@@ -13958,15 +13961,15 @@
                 _setSize(t, e) {
                     t === this.width && e === this.height || (this.width = t, this.height = e, this.setNeedsUpdate("Size changed"))
                 }
                 _setViews(t) {
                     t = oa(t, Boolean), this._diffViews(t, this.views) && this.setNeedsUpdate("views changed"), this.views = t
                 }
                 _setViewState(t) {
-                    t ? (!Sf(t, this.viewState, 3) && this.setNeedsUpdate("viewState changed"), this.viewState = t) : na.warn("missing `viewState` or `initialViewState`")()
+                    t ? (!Cf(t, this.viewState, 3) && this.setNeedsUpdate("viewState changed"), this.viewState = t) : na.warn("missing `viewState` or `initialViewState`")()
                 }
                 _onViewStateChange(t, e) {
                     this._eventCallbacks.onViewStateChange && this._eventCallbacks.onViewStateChange({
                         ...e,
                         viewId: t
                     })
                 }
@@ -14031,68 +14034,68 @@
                         t.id && (this._viewportMap[t.id] = this._viewportMap[t.id] || t)
                     }))
                 }
                 _diffViews(t, e) {
                     return t.length !== e.length || t.some(((n, i) => !t[i].equals(e[i])))
                 }
             }
-            const Tf = /([0-9]+\.?[0-9]*)(%|px)/;
+            const Af = /([0-9]+\.?[0-9]*)(%|px)/;
 
-            function Af(t) {
+            function Mf(t) {
                 switch (typeof t) {
                     case "number":
                         return {
                             position: t, relative: !1
                         };
                     case "string":
-                        const e = Tf.exec(t);
+                        const e = Af.exec(t);
                         if (e && e.length >= 3) {
                             const t = "%" === e[2],
                                 n = parseFloat(e[1]);
                             return {
                                 position: t ? n / 100 : n,
                                 relative: t
                             }
                         }
                     default:
                         throw new Error("Could not parse position string ".concat(t))
                 }
             }
 
-            function Mf(t, e) {
+            function Of(t, e) {
                 return t.relative ? Math.round(t.position * e) : t.position
             }
 
-            function Of(t, e) {
+            function Lf(t, e) {
                 if (!t) throw new Error(e || "deck.gl: assertion failed.")
             }
-            class Lf {
+            class Rf {
                 constructor(t) {
                     wo(this, "id", void 0), wo(this, "viewportInstance", void 0), wo(this, "_x", void 0), wo(this, "_y", void 0), wo(this, "_width", void 0), wo(this, "_height", void 0), wo(this, "_padding", void 0), wo(this, "props", void 0);
                     const {
                         id: e,
                         x: n = 0,
                         y: i = 0,
                         width: r = "100%",
                         height: s = "100%",
                         padding: o = null,
                         viewportInstance: a
                     } = t || {};
-                    Of(!a || a instanceof Dh), this.viewportInstance = a, this.id = e || this.constructor.displayName || "view", this.props = {
+                    Lf(!a || a instanceof Dh), this.viewportInstance = a, this.id = e || this.constructor.displayName || "view", this.props = {
                         ...t,
                         id: this.id
-                    }, this._x = Af(n), this._y = Af(i), this._width = Af(r), this._height = Af(s), this._padding = o && {
-                        left: Af(o.left || 0),
-                        right: Af(o.right || 0),
-                        top: Af(o.top || 0),
-                        bottom: Af(o.bottom || 0)
+                    }, this._x = Mf(n), this._y = Mf(i), this._width = Mf(r), this._height = Mf(s), this._padding = o && {
+                        left: Mf(o.left || 0),
+                        right: Mf(o.right || 0),
+                        top: Mf(o.top || 0),
+                        bottom: Mf(o.bottom || 0)
                     }, this.equals = this.equals.bind(this), Object.seal(this)
                 }
                 equals(t) {
-                    return this === t || (this.viewportInstance ? !!t.viewportInstance && this.viewportInstance.equals(t.viewportInstance) : this.ViewportType === t.ViewportType && Sf(this.props, t.props, 2))
+                    return this === t || (this.viewportInstance ? !!t.viewportInstance && this.viewportInstance.equals(t.viewportInstance) : this.ViewportType === t.ViewportType && Cf(this.props, t.props, 2))
                 }
                 makeViewport({
                     width: t,
                     height: e,
                     viewState: n
                 }) {
                     if (this.viewportInstance) return this.viewportInstance;
@@ -14125,39 +14128,39 @@
                     return t
                 }
                 getDimensions({
                     width: t,
                     height: e
                 }) {
                     const n = {
-                        x: Mf(this._x, t),
-                        y: Mf(this._y, e),
-                        width: Mf(this._width, t),
-                        height: Mf(this._height, e)
+                        x: Of(this._x, t),
+                        y: Of(this._y, e),
+                        width: Of(this._width, t),
+                        height: Of(this._height, e)
                     };
                     return this._padding && (n.padding = {
-                        left: Mf(this._padding.left, t),
-                        top: Mf(this._padding.top, e),
-                        right: Mf(this._padding.right, t),
-                        bottom: Mf(this._padding.bottom, e)
+                        left: Of(this._padding.left, t),
+                        top: Of(this._padding.top, e),
+                        right: Of(this._padding.right, t),
+                        bottom: Of(this._padding.bottom, e)
                     }), n
                 }
                 get controller() {
                     const t = this.props.controller;
                     return t ? !0 === t ? {
                         type: this.ControllerType
                     } : "function" == typeof t ? {
                         type: t
                     } : {
                         type: this.ControllerType,
                         ...t
                     } : null
                 }
             }
-            class Rf extends Dh {
+            class If extends Dh {
                 constructor(t = {}) {
                     const {
                         latitude: e = 0,
                         longitude: n = 0,
                         zoom: i = 0,
                         pitch: r = 0,
                         bearing: s = 0,
@@ -14269,15 +14272,15 @@
                 }
                 get subViewports() {
                     if (this._subViewports && !this._subViewports.length) {
                         const t = this.getBounds(),
                             e = Math.floor((t[0] + 180) / 360),
                             n = Math.ceil((t[2] - 180) / 360);
                         for (let t = e; t <= n; t++) {
-                            const e = t ? new Rf({
+                            const e = t ? new If({
                                 ...this,
                                 worldOffset: t
                             }) : this;
                             this._subViewports.push(e)
                         }
                     }
                     return this._subViewports
@@ -14360,25 +14363,25 @@
                         }
                     }({
                         width: n,
                         height: i,
                         bounds: t,
                         ...e
                     });
-                    return new Rf({
+                    return new If({
                         width: n,
                         height: i,
                         longitude: r,
                         latitude: s,
                         zoom: o
                     })
                 }
             }
-            wo(Rf, "displayName", "WebMercatorViewport");
-            class If {
+            wo(If, "displayName", "WebMercatorViewport");
+            class kf {
                 constructor(t) {
                     wo(this, "_inProgress", void 0), wo(this, "_handle", void 0), wo(this, "_timeline", void 0), wo(this, "time", void 0), wo(this, "settings", void 0), this._inProgress = !1, this._handle = null, this._timeline = t, this.time = 0, this.settings = {
                         duration: 0
                     }
                 }
                 get inProgress() {
                     return this._inProgress
@@ -14408,17 +14411,17 @@
                             duration: e.duration
                         })
                     }
                     return this.time = this._timeline.getTime(this._handle), this._onUpdate(), null === (t = (e = this.settings).onUpdate) || void 0 === t || t.call(e, this), this._timeline.isFinished(this._handle) && this.end(), !0
                 }
                 _onUpdate() {}
             }
-            const kf = () => {},
-                jf = t => t;
-            class Ff {
+            const jf = () => {},
+                Ff = t => t;
+            class zf {
                 constructor(t) {
                     wo(this, "getControllerState", void 0), wo(this, "props", void 0), wo(this, "propsInTransition", void 0), wo(this, "transition", void 0), wo(this, "onViewStateChange", void 0), wo(this, "onStateChange", void 0), wo(this, "_onTransitionUpdate", (t => {
                         const {
                             time: e,
                             settings: {
                                 interpolator: n,
                                 startProps: i,
@@ -14430,15 +14433,15 @@
                         this.propsInTransition = this.getControllerState({
                             ...this.props,
                             ...l
                         }).getViewportProps(), this.onViewStateChange({
                             viewState: this.propsInTransition,
                             oldViewState: this.props
                         })
-                    })), this.getControllerState = t.getControllerState, this.propsInTransition = null, this.transition = new If(t.timeline), this.onViewStateChange = t.onViewStateChange || kf, this.onStateChange = t.onStateChange || kf
+                    })), this.getControllerState = t.getControllerState, this.propsInTransition = null, this.transition = new kf(t.timeline), this.onViewStateChange = t.onViewStateChange || jf, this.onStateChange = t.onStateChange || jf
                 }
                 finalize() {
                     this.transition.cancel()
                 }
                 getViewportInTransition() {
                     return this.propsInTransition
                 }
@@ -14484,15 +14487,15 @@
                         r = e.transitionInterpolator,
                         s = r.getDuration ? r.getDuration(t, e) : e.transitionDuration;
                     if (0 === s) return;
                     const o = r.initializeProps(t, i);
                     this.propsInTransition = {};
                     const a = {
                         duration: s,
-                        easing: e.transitionEasing || jf,
+                        easing: e.transitionEasing || Ff,
                         interpolator: r,
                         interruption: e.transitionInterruption || 1,
                         startProps: o.start,
                         endProps: o.end,
                         onStart: e.onTransitionStart,
                         onUpdate: this._onTransitionUpdate,
                         onInterrupt: this._onTransitionEnd(e.onTransitionInterrupt),
@@ -14509,15 +14512,15 @@
                             isZooming: !1,
                             isPanning: !1,
                             isRotating: !1
                         }), null == t || t(e)
                     }
                 }
             }
-            class zf {
+            class Bf {
                 constructor(t) {
                     wo(this, "_propsToCompare", void 0), wo(this, "_propsToExtract", void 0), wo(this, "_requiredProps", void 0);
                     const {
                         compare: e,
                         extract: n,
                         required: i
                     } = t;
@@ -14539,30 +14542,30 @@
                 }
                 getDuration(t, e) {
                     return e.transitionDuration
                 }
                 _checkRequiredProps(t) {
                     this._requiredProps && this._requiredProps.forEach((e => {
                         const n = t[e];
-                        Of(Number.isFinite(n) || Array.isArray(n), "".concat(e, " is required for transition"))
+                        Lf(Number.isFinite(n) || Array.isArray(n), "".concat(e, " is required for transition"))
                     }))
                 }
             }
-            const Bf = ["longitude", "latitude", "zoom", "bearing", "pitch"],
-                Df = ["longitude", "latitude", "zoom"];
-            class Nf extends zf {
+            const Df = ["longitude", "latitude", "zoom", "bearing", "pitch"],
+                Nf = ["longitude", "latitude", "zoom"];
+            class Vf extends Bf {
                 constructor(t = {}) {
                     const e = Array.isArray(t) ? t : t.transitionProps,
                         n = Array.isArray(t) ? {} : t;
                     n.transitionProps = Array.isArray(e) ? {
                         compare: e,
                         required: e
                     } : e || {
-                        compare: Bf,
-                        required: Df
+                        compare: Df,
+                        required: Nf
                     }, super(n.transitionProps), wo(this, "opts", void 0), this.opts = n
                 }
                 initializeProps(t, e) {
                     const n = super.initializeProps(t, e),
                         {
                             makeViewport: i,
                             around: r
@@ -14589,30 +14592,30 @@
                             ...i
                         });
                         Object.assign(i, r.panByPosition(e.aroundPosition, hc(t.around, e.around, n)))
                     }
                     return i
                 }
             }
-            const Vf = {
+            const Uf = {
                     transitionDuration: 0
                 },
-                Uf = t => 1 - (1 - t) * (1 - t),
-                Gf = ["wheel"],
-                Wf = ["panstart", "panmove", "panend"],
-                Hf = ["pinchstart", "pinchmove", "pinchend"],
-                Zf = ["tripanstart", "tripanmove", "tripanend"],
-                qf = ["doubletap"],
-                Xf = ["keydown"],
-                Yf = {};
-            class Kf {
+                Gf = t => 1 - (1 - t) * (1 - t),
+                Wf = ["wheel"],
+                Hf = ["panstart", "panmove", "panend"],
+                Zf = ["pinchstart", "pinchmove", "pinchend"],
+                qf = ["tripanstart", "tripanmove", "tripanend"],
+                Xf = ["doubletap"],
+                Yf = ["keydown"],
+                Kf = {};
+            class Qf {
                 constructor(t) {
                     wo(this, "props", void 0), wo(this, "state", {}), wo(this, "transitionManager", void 0), wo(this, "eventManager", void 0), wo(this, "onViewStateChange", void 0), wo(this, "onStateChange", void 0), wo(this, "makeViewport", void 0), wo(this, "_controllerState", void 0), wo(this, "_events", {}), wo(this, "_interactionState", {
                         isDragging: !1
-                    }), wo(this, "_customEvents", []), wo(this, "_eventStartBlocked", null), wo(this, "_panMove", !1), wo(this, "invertPan", !1), wo(this, "dragMode", "rotate"), wo(this, "inertia", 0), wo(this, "scrollZoom", !0), wo(this, "dragPan", !0), wo(this, "dragRotate", !0), wo(this, "doubleClickZoom", !0), wo(this, "touchZoom", !0), wo(this, "touchRotate", !1), wo(this, "keyboard", !0), this.transitionManager = new Ff({
+                    }), wo(this, "_customEvents", []), wo(this, "_eventStartBlocked", null), wo(this, "_panMove", !1), wo(this, "invertPan", !1), wo(this, "dragMode", "rotate"), wo(this, "inertia", 0), wo(this, "scrollZoom", !0), wo(this, "dragPan", !0), wo(this, "dragRotate", !0), wo(this, "doubleClickZoom", !0), wo(this, "touchZoom", !0), wo(this, "touchRotate", !1), wo(this, "keyboard", !0), this.transitionManager = new zf({
                         ...t,
                         getControllerState: t => new this.ControllerState(t),
                         onViewStateChange: this._onTransition.bind(this),
                         onStateChange: this._setInteractionState.bind(this)
                     }), this.handleEvent = this.handleEvent.bind(this), this.eventManager = t.eventManager, this.onViewStateChange = t.onViewStateChange || (() => {}), this.onStateChange = t.onStateChange || (() => {}), this.makeViewport = t.makeViewport
                 }
                 set events(t) {
@@ -14708,15 +14711,15 @@
                         dragPan: i = !0,
                         dragRotate: r = !0,
                         doubleClickZoom: s = !0,
                         touchZoom: o = !0,
                         touchRotate: a = !1,
                         keyboard: l = !0
                     } = t, c = Boolean(this.onViewStateChange);
-                    this.toggleEvents(Gf, c && n), this.toggleEvents(Wf, c && (i || r)), this.toggleEvents(Hf, c && (o || a)), this.toggleEvents(Zf, c && a), this.toggleEvents(qf, c && s), this.toggleEvents(Xf, c && l), this.scrollZoom = n, this.dragPan = i, this.dragRotate = r, this.doubleClickZoom = s, this.touchZoom = o, this.touchRotate = a, this.keyboard = l
+                    this.toggleEvents(Wf, c && n), this.toggleEvents(Hf, c && (i || r)), this.toggleEvents(Zf, c && (o || a)), this.toggleEvents(qf, c && a), this.toggleEvents(Xf, c && s), this.toggleEvents(Yf, c && l), this.scrollZoom = n, this.dragPan = i, this.dragRotate = r, this.doubleClickZoom = s, this.touchZoom = o, this.touchRotate = a, this.keyboard = l
                 }
                 updateTransition() {
                     this.transitionManager.updateTransition()
                 }
                 toggleEvents(t, e) {
                     this.eventManager && t.forEach((t => {
                         this._events[t] !== e && (this._events[t] = e, e ? this.eventManager.on(t, this.handleEvent) : this.eventManager.off(t, this.handleEvent))
@@ -14750,15 +14753,15 @@
                     const e = this.getCenter(t);
                     if (!this.isPointInBounds(e, t)) return !1;
                     let n = this.isFunctionKeyPressed(t) || t.rightButton || !1;
                     (this.invertPan || "pan" === this.dragMode) && (n = !n);
                     const i = this.controllerState[n ? "panStart" : "rotateStart"]({
                         pos: e
                     });
-                    return this._panMove = n, this.updateViewport(i, Vf, {
+                    return this._panMove = n, this.updateViewport(i, Uf, {
                         isDragging: !0
                     }), !0
                 }
                 _onPan(t) {
                     return !!this.isDragging() && (this._panMove ? this._onPanMove(t) : this._onPanRotate(t))
                 }
                 _onPanEnd(t) {
@@ -14766,15 +14769,15 @@
                 }
                 _onPanMove(t) {
                     if (!this.dragPan) return !1;
                     const e = this.getCenter(t),
                         n = this.controllerState.pan({
                             pos: e
                         });
-                    return this.updateViewport(n, Vf, {
+                    return this.updateViewport(n, Uf, {
                         isDragging: !0,
                         isPanning: !0
                     }), !0
                 }
                 _onPanMoveEnd(t) {
                     const {
                         inertia: e
@@ -14784,15 +14787,15 @@
                             i = [n[0] + t.velocityX * e / 2, n[1] + t.velocityY * e / 2],
                             r = this.controllerState.pan({
                                 pos: i
                             }).panEnd();
                         this.updateViewport(r, {
                             ...this._getTransitionProps(),
                             transitionDuration: e,
-                            transitionEasing: Uf
+                            transitionEasing: Gf
                         }, {
                             isDragging: !1,
                             isPanning: !0
                         })
                     } else {
                         const t = this.controllerState.panEnd();
                         this.updateViewport(t, null, {
@@ -14804,15 +14807,15 @@
                 }
                 _onPanRotate(t) {
                     if (!this.dragRotate) return !1;
                     const e = this.getCenter(t),
                         n = this.controllerState.rotate({
                             pos: e
                         });
-                    return this.updateViewport(n, Vf, {
+                    return this.updateViewport(n, Uf, {
                         isDragging: !0,
                         isRotating: !0
                     }), !0
                 }
                 _onPanRotateEnd(t) {
                     const {
                         inertia: e
@@ -14822,15 +14825,15 @@
                             i = [n[0] + t.velocityX * e / 2, n[1] + t.velocityY * e / 2],
                             r = this.controllerState.rotate({
                                 pos: i
                             }).rotateEnd();
                         this.updateViewport(r, {
                             ...this._getTransitionProps(),
                             transitionDuration: e,
-                            transitionEasing: Uf
+                            transitionEasing: Gf
                         }, {
                             isDragging: !1,
                             isRotating: !0
                         })
                     } else {
                         const t = this.controllerState.rotateEnd();
                         this.updateViewport(t, null, {
@@ -14869,27 +14872,27 @@
                 }
                 _onTriplePanStart(t) {
                     const e = this.getCenter(t);
                     if (!this.isPointInBounds(e, t)) return !1;
                     const n = this.controllerState.rotateStart({
                         pos: e
                     });
-                    return this.updateViewport(n, Vf, {
+                    return this.updateViewport(n, Uf, {
                         isDragging: !0
                     }), !0
                 }
                 _onTriplePan(t) {
                     if (!this.touchRotate) return !1;
                     if (!this.isDragging()) return !1;
                     const e = this.getCenter(t);
                     e[0] -= t.deltaX;
                     const n = this.controllerState.rotate({
                         pos: e
                     });
-                    return this.updateViewport(n, Vf, {
+                    return this.updateViewport(n, Uf, {
                         isDragging: !0,
                         isRotating: !0
                     }), !0
                 }
                 _onTriplePanEnd(t) {
                     if (!this.isDragging()) return !1;
                     const {
@@ -14900,15 +14903,15 @@
                             i = [n[0], n[1] += t.velocityY * e / 2],
                             r = this.controllerState.rotate({
                                 pos: i
                             });
                         this.updateViewport(r, {
                             ...this._getTransitionProps(),
                             transitionDuration: e,
-                            transitionEasing: Uf
+                            transitionEasing: Gf
                         }, {
                             isDragging: !1,
                             isRotating: !0
                         }), this.blockEvents(e)
                     } else {
                         const t = this.controllerState.rotateEnd();
                         this.updateViewport(t, null, {
@@ -14922,15 +14925,15 @@
                     const e = this.getCenter(t);
                     if (!this.isPointInBounds(e, t)) return !1;
                     const n = this.controllerState.zoomStart({
                         pos: e
                     }).rotateStart({
                         pos: e
                     });
-                    return Yf._startPinchRotation = t.rotation, Yf._lastPinchEvent = t, this.updateViewport(n, Vf, {
+                    return Kf._startPinchRotation = t.rotation, Kf._lastPinchEvent = t, this.updateViewport(n, Uf, {
                         isDragging: !0
                     }), !0
                 }
                 _onPinch(t) {
                     if (!this.touchZoom && !this.touchRotate) return !1;
                     if (!this.isDragging()) return !1;
                     let e = this.controllerState;
@@ -14944,46 +14947,46 @@
                         })
                     }
                     if (this.touchRotate) {
                         const {
                             rotation: n
                         } = t;
                         e = e.rotate({
-                            deltaAngleX: Yf._startPinchRotation - n
+                            deltaAngleX: Kf._startPinchRotation - n
                         })
                     }
-                    return this.updateViewport(e, Vf, {
+                    return this.updateViewport(e, Uf, {
                         isDragging: !0,
                         isPanning: this.touchZoom,
                         isZooming: this.touchZoom,
                         isRotating: this.touchRotate
-                    }), Yf._lastPinchEvent = t, !0
+                    }), Kf._lastPinchEvent = t, !0
                 }
                 _onPinchEnd(t) {
                     if (!this.isDragging()) return !1;
                     const {
                         inertia: e
                     } = this, {
                         _lastPinchEvent: n
-                    } = Yf;
+                    } = Kf;
                     if (this.touchZoom && e && n && t.scale !== n.scale) {
                         const i = this.getCenter(t);
                         let r = this.controllerState.rotateEnd();
                         const s = Math.log2(t.scale),
                             o = (s - Math.log2(n.scale)) / (t.deltaTime - n.deltaTime),
                             a = Math.pow(2, s + o * e / 2);
                         r = r.zoom({
                             pos: i,
                             scale: a
                         }).zoomEnd(), this.updateViewport(r, {
                             ...this._getTransitionProps({
                                 around: i
                             }),
                             transitionDuration: e,
-                            transitionEasing: Uf
+                            transitionEasing: Gf
                         }, {
                             isDragging: !1,
                             isPanning: this.touchZoom,
                             isZooming: this.touchZoom,
                             isRotating: !1
                         }), this.blockEvents(e)
                     } else {
@@ -14991,15 +14994,15 @@
                         this.updateViewport(t, null, {
                             isDragging: !1,
                             isPanning: !1,
                             isZooming: !1,
                             isRotating: !1
                         })
                     }
-                    return Yf._startPinchRotation = null, Yf._lastPinchEvent = null, !0
+                    return Kf._startPinchRotation = null, Kf._lastPinchEvent = null, !0
                 }
                 _onDoubleTap(t) {
                     if (!this.doubleClickZoom) return !1;
                     const e = this.getCenter(t);
                     if (!this.isPointInBounds(e, t)) return !1;
                     const n = this.isFunctionKeyPressed(t),
                         i = this.controllerState.zoom({
@@ -15053,34 +15056,34 @@
                 }
                 _getTransitionProps(t) {
                     const {
                         transition: e
                     } = this;
                     return e && e.transitionInterpolator ? t ? {
                         ...e,
-                        transitionInterpolator: new Nf({
+                        transitionInterpolator: new Vf({
                             ...t,
                             ...e.transitionInterpolator.opts,
                             makeViewport: this.controllerState.makeViewport
                         })
-                    } : e : Vf
+                    } : e : Uf
                 }
             }
-            class Qf {
+            class Jf {
                 constructor(t, e) {
                     wo(this, "_viewportProps", void 0), wo(this, "_state", void 0), this._viewportProps = this.applyConstraints(t), this._state = e
                 }
                 getViewportProps() {
                     return this._viewportProps
                 }
                 getState() {
                     return this._state
                 }
             }
-            class Jf extends Qf {
+            class $f extends Jf {
                 constructor(t) {
                     const {
                         width: e,
                         height: n,
                         latitude: i,
                         longitude: r,
                         zoom: s,
@@ -15096,15 +15099,15 @@
                         startZoomLngLat: g,
                         startRotatePos: m,
                         startBearing: v,
                         startPitch: b,
                         startZoom: y,
                         normalize: _ = !0
                     } = t;
-                    Of(Number.isFinite(r)), Of(Number.isFinite(i)), Of(Number.isFinite(s)), super({
+                    Lf(Number.isFinite(r)), Lf(Number.isFinite(i)), Lf(Number.isFinite(s)), super({
                         width: e,
                         height: n,
                         latitude: i,
                         longitude: r,
                         zoom: s,
                         bearing: o,
                         pitch: a,
@@ -15367,19 +15370,19 @@
                     let f = n;
                     return u > 0 ? f = n + u * (p - n) : u < 0 && (f = n - u * (d - n)), {
                         pitch: f,
                         bearing: i + 180 * h
                     }
                 }
             }
-            class $f extends Kf {
+            class tg extends Qf {
                 constructor(...t) {
-                    super(...t), wo(this, "ControllerState", Jf), wo(this, "transition", {
+                    super(...t), wo(this, "ControllerState", $f), wo(this, "transition", {
                         transitionDuration: 300,
-                        transitionInterpolator: new Nf({
+                        transitionInterpolator: new Vf({
                             transitionProps: {
                                 compare: ["longitude", "latitude", "zoom", "bearing", "pitch", "position"],
                                 required: ["longitude", "latitude", "zoom"]
                             }
                         })
                     }), wo(this, "dragMode", "pan")
                 }
@@ -15389,60 +15392,60 @@
                     super.setProps(t), (!e || e.height !== t.height) && this.updateViewport(new this.ControllerState({
                         makeViewport: this.makeViewport,
                         ...t,
                         ...this.state
                     }))
                 }
             }
-            class tg extends Lf {
+            class eg extends Rf {
                 get ViewportType() {
-                    return Rf
+                    return If
                 }
                 get ControllerType() {
-                    return $f
+                    return tg
                 }
             }
-            wo(tg, "displayName", "MapView");
-            const eg = [255, 255, 255],
-                ng = 1;
-            let ig = 0;
-            class rg {
+            wo(eg, "displayName", "MapView");
+            const ng = [255, 255, 255],
+                ig = 1;
+            let rg = 0;
+            class sg {
                 constructor(t = {}) {
                     wo(this, "id", void 0), wo(this, "color", void 0), wo(this, "intensity", void 0), wo(this, "type", "ambient");
                     const {
-                        color: e = eg
+                        color: e = ng
                     } = t, {
-                        intensity: n = ng
+                        intensity: n = ig
                     } = t;
-                    this.id = t.id || "ambient-".concat(ig++), this.color = e, this.intensity = n
+                    this.id = t.id || "ambient-".concat(rg++), this.color = e, this.intensity = n
                 }
             }
-            const sg = [255, 255, 255],
-                og = 1,
-                ag = [0, 0, -1];
-            let lg = 0;
-            class cg {
+            const og = [255, 255, 255],
+                ag = 1,
+                lg = [0, 0, -1];
+            let cg = 0;
+            class hg {
                 constructor(t = {}) {
                     wo(this, "id", void 0), wo(this, "color", void 0), wo(this, "intensity", void 0), wo(this, "type", "directional"), wo(this, "direction", void 0), wo(this, "shadow", void 0);
                     const {
-                        color: e = sg
+                        color: e = og
                     } = t, {
-                        intensity: n = og
+                        intensity: n = ag
                     } = t, {
-                        direction: i = ag
+                        direction: i = lg
                     } = t, {
                         _shadow: r = !1
                     } = t;
-                    this.id = t.id || "directional-".concat(lg++), this.color = e, this.intensity = n, this.type = "directional", this.direction = new Ic(i).normalize().toArray(), this.shadow = r
+                    this.id = t.id || "directional-".concat(cg++), this.color = e, this.intensity = n, this.type = "directional", this.direction = new Ic(i).normalize().toArray(), this.shadow = r
                 }
                 getProjectedLight(t) {
                     return this
                 }
             }
-            class hg {
+            class ug {
                 constructor(t, e = {
                     id: "pass"
                 }) {
                     wo(this, "id", void 0), wo(this, "gl", void 0), wo(this, "props", void 0);
                     const {
                         id: n
                     } = e;
@@ -15452,15 +15455,15 @@
                 }
                 setProps(t) {
                     Object.assign(this.props, t)
                 }
                 render(t) {}
                 cleanup() {}
             }
-            class ug extends hg {
+            class dg extends ug {
                 constructor(...t) {
                     super(...t), wo(this, "_lastRenderIndex", -1)
                 }
                 render(t) {
                     return hd(this.gl, {
                         framebuffer: t.target
                     }), this._drawLayers(t)
@@ -15508,15 +15511,15 @@
                     isPicking: i = !1,
                     layerFilter: r,
                     cullRect: s,
                     effects: o,
                     moduleParameters: a
                 }, l = !1) {
                     const c = [],
-                        h = dg(this._lastRenderIndex + 1),
+                        h = pg(this._lastRenderIndex + 1),
                         u = {
                             layer: e[0],
                             viewport: t,
                             isPicking: i,
                             renderPass: n,
                             cullRect: s
                         },
@@ -15558,15 +15561,15 @@
                         const e = !0 === o.props.clear ? {
                             color: !0,
                             depth: !0
                         } : o.props.clear;
                         ud(t, {
                             scissorTest: !0,
                             scissor: l
-                        }, (() => ip(t, e)))
+                        }, (() => rp(t, e)))
                     }
                     const c = {
                         totalCount: e.length,
                         visibleCount: 0,
                         compositeCount: 0,
                         pickableCount: 0
                     };
@@ -15636,45 +15639,45 @@
                             var o;
                             Object.assign(s, null === (o = n.getModuleParameters) || void 0 === o ? void 0 : o.call(n, t))
                         }
                     return Object.assign(s, this.getModuleParameters(t, e), i)
                 }
             }
 
-            function dg(t = 0, e = {}) {
+            function pg(t = 0, e = {}) {
                 const n = {},
                     i = (r, s) => {
                         const o = r.props._offset,
                             a = r.id,
                             l = r.parent && r.parent.id;
                         let c;
                         if (l && !(l in e) && i(r.parent, !1), l in n) {
-                            const t = n[l] = n[l] || dg(e[l], e);
+                            const t = n[l] = n[l] || pg(e[l], e);
                             c = t(r, s), n[a] = t
                         } else Number.isFinite(o) ? (c = o + (e[l] || 0), n[a] = null) : c = t;
                         return s && c >= t && (t = c + 1), e[a] = c, c
                     };
                 return i
             }
-            class pg extends ug {
+            class fg extends dg {
                 constructor(t, e) {
-                    super(t, e), wo(this, "shadowMap", void 0), wo(this, "depthBuffer", void 0), wo(this, "fbo", void 0), this.shadowMap = new Qd(t, {
+                    super(t, e), wo(this, "shadowMap", void 0), wo(this, "depthBuffer", void 0), wo(this, "fbo", void 0), this.shadowMap = new Jd(t, {
                         width: 1,
                         height: 1,
                         parameters: {
                             10241: 9729,
                             10240: 9729,
                             10242: 33071,
                             10243: 33071
                         }
-                    }), this.depthBuffer = new tp(t, {
+                    }), this.depthBuffer = new ep(t, {
                         format: 33189,
                         width: 1,
                         height: 1
-                    }), this.fbo = new bp(t, {
+                    }), this.fbo = new yp(t, {
                         id: "shadowmap",
                         width: 1,
                         height: 1,
                         attachments: {
                             36064: this.shadowMap,
                             36096: this.depthBuffer
                         }
@@ -15710,21 +15713,21 @@
                         drawToShadowMap: !0
                     }
                 }
                 delete() {
                     this.fbo && (this.fbo.delete(), this.fbo = null), this.shadowMap && (this.shadowMap.delete(), this.shadowMap = null), this.depthBuffer && (this.depthBuffer.delete(), this.depthBuffer = null)
                 }
             }
-            const fg = uf((function({
+            const gg = df((function({
                     viewport: t,
                     center: e
                 }) {
                     return new ih(t.viewProjectionMatrix).invert().transform(e)
                 })),
-                gg = uf((function({
+                mg = df((function({
                     viewport: t,
                     shadowMatrices: e
                 }) {
                     const n = [],
                         i = t.pixelUnprojectionMatrix,
                         r = t.isGeospatial ? void 0 : 1,
                         s = [
@@ -15751,19 +15754,19 @@
                                 near: Math.min(...r.map((t => -t[2]))),
                                 far: Math.max(...r.map((t => -t[2])))
                             });
                         n.push(o.multiplyRight(i))
                     }
                     return n
                 })),
-                mg = [0, 0, 0, 1],
-                vg = [1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0],
-                bg = {
+                vg = [0, 0, 0, 1],
+                bg = [1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 1, 0, 0, 0, 0, 0],
+                yg = {
                     name: "shadow",
-                    dependencies: [_f],
+                    dependencies: [xf],
                     vs: "\nconst int max_lights = 2;\nuniform mat4 shadow_uViewProjectionMatrices[max_lights];\nuniform vec4 shadow_uProjectCenters[max_lights];\nuniform bool shadow_uDrawShadowMap;\nuniform bool shadow_uUseShadowMap;\nuniform int shadow_uLightId;\nuniform float shadow_uLightCount;\n\nvarying vec3 shadow_vPosition[max_lights];\n\nvec4 shadow_setVertexPosition(vec4 position_commonspace) {\n  if (shadow_uDrawShadowMap) {\n    return project_common_position_to_clipspace(position_commonspace, shadow_uViewProjectionMatrices[shadow_uLightId], shadow_uProjectCenters[shadow_uLightId]);\n  }\n  if (shadow_uUseShadowMap) {\n    for (int i = 0; i < max_lights; i++) {\n      if(i < int(shadow_uLightCount)) {\n        vec4 shadowMap_position = project_common_position_to_clipspace(position_commonspace, shadow_uViewProjectionMatrices[i], shadow_uProjectCenters[i]);\n        shadow_vPosition[i] = (shadowMap_position.xyz / shadowMap_position.w + 1.0) / 2.0;\n      }\n    }\n  }\n  return gl_Position;\n}\n",
                     fs: "\nconst int max_lights = 2;\nuniform bool shadow_uDrawShadowMap;\nuniform bool shadow_uUseShadowMap;\nuniform sampler2D shadow_uShadowMap0;\nuniform sampler2D shadow_uShadowMap1;\nuniform vec4 shadow_uColor;\nuniform float shadow_uLightCount;\n\nvarying vec3 shadow_vPosition[max_lights];\n\nconst vec4 bitPackShift = vec4(1.0, 255.0, 65025.0, 16581375.0);\nconst vec4 bitUnpackShift = 1.0 / bitPackShift;\nconst vec4 bitMask = vec4(1.0 / 255.0, 1.0 / 255.0, 1.0 / 255.0,  0.0);\n\nfloat shadow_getShadowWeight(vec3 position, sampler2D shadowMap) {\n  vec4 rgbaDepth = texture2D(shadowMap, position.xy);\n\n  float z = dot(rgbaDepth, bitUnpackShift);\n  return smoothstep(0.001, 0.01, position.z - z);\n}\n\nvec4 shadow_filterShadowColor(vec4 color) {\n  if (shadow_uDrawShadowMap) {\n    vec4 rgbaDepth = fract(gl_FragCoord.z * bitPackShift);\n    rgbaDepth -= rgbaDepth.gbaa * bitMask;\n    return rgbaDepth;\n  }\n  if (shadow_uUseShadowMap) {\n    float shadowAlpha = 0.0;\n    shadowAlpha += shadow_getShadowWeight(shadow_vPosition[0], shadow_uShadowMap0);\n    if(shadow_uLightCount > 1.0) {\n      shadowAlpha += shadow_getShadowWeight(shadow_vPosition[1], shadow_uShadowMap1);\n    }\n    shadowAlpha *= shadow_uColor.a / shadow_uLightCount;\n    float blendedAlpha = shadowAlpha + color.a * (1.0 - shadowAlpha);\n\n    return vec4(\n      mix(color.rgb, shadow_uColor.rgb, shadowAlpha / blendedAlpha),\n      blendedAlpha\n    );\n  }\n  return color;\n}\n",
                     inject: {
                         "vs:DECKGL_FILTER_GL_POSITION": "\n    position = shadow_setVertexPosition(geometry.position);\n    ",
                         "fs:DECKGL_FILTER_COLOR": "\n    color = shadow_filterShadowColor(color);\n    "
                     },
                     getUniforms: (t = {}, e = {}) => "viewport" in t && (t.drawToShadowMap || t.shadowMaps && t.shadowMaps.length > 0) ? function(t, e) {
@@ -15773,53 +15776,53 @@
                         if (!n || !t.shadowMatrices || !t.shadowMatrices.length) return {
                             shadow_uDrawShadowMap: !1,
                             shadow_uUseShadowMap: !1
                         };
                         const i = {
                                 shadow_uDrawShadowMap: Boolean(t.drawToShadowMap),
                                 shadow_uUseShadowMap: !!t.shadowMaps && t.shadowMaps.length > 0,
-                                shadow_uColor: t.shadowColor || mg,
+                                shadow_uColor: t.shadowColor || vg,
                                 shadow_uLightId: t.shadowLightId || 0,
                                 shadow_uLightCount: t.shadowMatrices.length
                             },
-                            r = fg({
+                            r = gg({
                                 viewport: t.viewport,
                                 center: e.project_uCenter
                             }),
                             s = [],
-                            o = gg({
+                            o = mg({
                                 shadowMatrices: t.shadowMatrices,
                                 viewport: t.viewport
                             }).slice();
                         for (let n = 0; n < t.shadowMatrices.length; n++) {
                             const i = o[n],
                                 a = i.clone().translate(new Ic(t.viewport.center).negate());
-                            e.project_uCoordinateSystem === Lh.LNGLAT && e.project_uProjectionMode === Rh.WEB_MERCATOR ? (o[n] = a, s[n] = r) : (o[n] = i.clone().multiplyRight(vg), s[n] = a.transform(r))
+                            e.project_uCoordinateSystem === Lh.LNGLAT && e.project_uProjectionMode === Rh.WEB_MERCATOR ? (o[n] = a, s[n] = r) : (o[n] = i.clone().multiplyRight(bg), s[n] = a.transform(r))
                         }
                         for (let e = 0; e < o.length; e++) i["shadow_uViewProjectionMatrices[".concat(e, "]")] = o[e], i["shadow_uProjectCenters[".concat(e, "]")] = s[e], t.shadowMaps && t.shadowMaps.length > 0 ? i["shadow_uShadowMap".concat(e)] = t.shadowMaps[e] : i["shadow_uShadowMap".concat(e)] = t.dummyShadowMap;
                         return i
                     }(t, e) : {}
                 },
-                yg = {
+                _g = {
                     color: [255, 255, 255],
                     intensity: 1
                 },
-                _g = [{
+                xg = [{
                     color: [255, 255, 255],
                     intensity: 1,
                     direction: [-1, 3, -1]
                 }, {
                     color: [255, 255, 255],
                     intensity: .9,
                     direction: [1, -8, -2.5]
                 }],
-                xg = [0, 0, 0, 200 / 255];
-            class wg {
+                wg = [0, 0, 0, 200 / 255];
+            class Eg {
                 constructor(t = {}) {
-                    wo(this, "id", "lighting-effect"), wo(this, "props", void 0), wo(this, "shadowColor", xg), wo(this, "shadow", void 0), wo(this, "ambientLight", void 0), wo(this, "directionalLights", void 0), wo(this, "pointLights", void 0), wo(this, "shadowPasses", []), wo(this, "shadowMaps", []), wo(this, "dummyShadowMap", null), wo(this, "programManager", void 0), wo(this, "shadowMatrices", void 0), this.setProps(t)
+                    wo(this, "id", "lighting-effect"), wo(this, "props", void 0), wo(this, "shadowColor", wg), wo(this, "shadow", void 0), wo(this, "ambientLight", void 0), wo(this, "directionalLights", void 0), wo(this, "pointLights", void 0), wo(this, "shadowPasses", []), wo(this, "shadowMaps", []), wo(this, "dummyShadowMap", null), wo(this, "programManager", void 0), wo(this, "shadowMatrices", void 0), this.setProps(t)
                 }
                 setProps(t) {
                     this.ambientLight = null, this.directionalLights = [], this.pointLights = [];
                     for (const e in t) {
                         const n = t[e];
                         switch (n.type) {
                             case "ambient":
@@ -15838,15 +15841,15 @@
                     layers: e,
                     layerFilter: n,
                     viewports: i,
                     onViewportActive: r,
                     views: s
                 }) {
                     if (this.shadow) {
-                        this.shadowMatrices = this._calculateMatrices(), 0 === this.shadowPasses.length && this._createShadowPasses(t), this.programManager || (this.programManager = nf.getDefaultProgramManager(t), bg && this.programManager.addDefaultModule(bg)), this.dummyShadowMap || (this.dummyShadowMap = new Qd(t, {
+                        this.shadowMatrices = this._calculateMatrices(), 0 === this.shadowPasses.length && this._createShadowPasses(t), this.programManager || (this.programManager = rf.getDefaultProgramManager(t), yg && this.programManager.addDefaultModule(yg)), this.dummyShadowMap || (this.dummyShadowMap = new Jd(t, {
                             width: 1,
                             height: 1
                         }));
                         for (let t = 0; t < this.shadowPasses.length; t++) this.shadowPasses[t].render({
                             layers: e,
                             layerFilter: n,
                             viewports: i,
@@ -15875,58 +15878,58 @@
                         pointLights: this.pointLights.map((e => e.getProjectedLight({
                             layer: t
                         })))
                     }, e
                 }
                 cleanup() {
                     for (const t of this.shadowPasses) t.delete();
-                    this.shadowPasses.length = 0, this.shadowMaps.length = 0, this.dummyShadowMap && (this.dummyShadowMap.delete(), this.dummyShadowMap = null), this.shadow && this.programManager && (this.programManager.removeDefaultModule(bg), this.programManager = null)
+                    this.shadowPasses.length = 0, this.shadowMaps.length = 0, this.dummyShadowMap && (this.dummyShadowMap.delete(), this.dummyShadowMap = null), this.shadow && this.programManager && (this.programManager.removeDefaultModule(yg), this.programManager = null)
                 }
                 _calculateMatrices() {
                     const t = [];
                     for (const e of this.directionalLights) {
                         const n = (new ih).lookAt({
                             eye: new Ic(e.direction).negate()
                         });
                         t.push(n)
                     }
                     return t
                 }
                 _createShadowPasses(t) {
                     for (let e = 0; e < this.directionalLights.length; e++) {
-                        const n = new pg(t);
+                        const n = new fg(t);
                         this.shadowPasses[e] = n, this.shadowMaps[e] = n.shadowMap
                     }
                 }
                 _applyDefaultLights() {
                     const {
                         ambientLight: t,
                         pointLights: e,
                         directionalLights: n
                     } = this;
-                    t || 0 !== e.length || 0 !== n.length || (this.ambientLight = new rg(yg), this.directionalLights.push(new cg(_g[0]), new cg(_g[1])))
+                    t || 0 !== e.length || 0 !== n.length || (this.ambientLight = new sg(_g), this.directionalLights.push(new hg(xg[0]), new hg(xg[1])))
                 }
             }
-            const Eg = new wg;
-            class Pg {
+            const Pg = new Eg;
+            class Sg {
                 constructor() {
                     wo(this, "effects", void 0), wo(this, "_resolvedEffects", []), wo(this, "_defaultEffects", []), wo(this, "_needsRedraw", void 0), this.effects = [], this._needsRedraw = "Initial render", this._setEffects([])
                 }
                 addDefaultEffect(t) {
                     const e = this._defaultEffects;
                     if (!e.find((e => e.id === t.id))) {
                         const n = e.findIndex((e => {
                             return n = t, (null !== (i = e.order) && void 0 !== i ? i : 1 / 0) - (null !== (r = n.order) && void 0 !== r ? r : 1 / 0) > 0;
                             var n, i, r
                         }));
                         n < 0 ? e.push(t) : e.splice(n, 0, t), this._setEffects(this.effects)
                     }
                 }
                 setProps(t) {
-                    "effects" in t && (Sf(t.effects, this.effects, 1) || this._setEffects(t.effects))
+                    "effects" in t && (Cf(t.effects, this.effects, 1) || this._setEffects(t.effects))
                 }
                 needsRedraw(t = {
                     clearRedrawFlags: !1
                 }) {
                     const e = this._needsRedraw;
                     return t.clearRedrawFlags && (this._needsRedraw = !1), e
                 }
@@ -15938,34 +15941,34 @@
                     for (const t of this.effects) e[t.id] = t;
                     const n = [];
                     for (const i of t) {
                         const t = e[i.id];
                         t && t !== i ? t.setProps ? (t.setProps(i.props), n.push(t)) : (t.cleanup(), n.push(i)) : n.push(i), delete e[i.id]
                     }
                     for (const t in e) e[t].cleanup();
-                    this.effects = n, this._resolvedEffects = n.concat(this._defaultEffects), t.some((t => t instanceof wg)) || this._resolvedEffects.push(Eg), this._needsRedraw = "effects changed"
+                    this.effects = n, this._resolvedEffects = n.concat(this._defaultEffects), t.some((t => t instanceof Eg)) || this._resolvedEffects.push(Pg), this._needsRedraw = "effects changed"
                 }
                 finalize() {
                     for (const t of this._resolvedEffects) t.cleanup();
                     this.effects.length = 0, this._resolvedEffects.length = 0, this._defaultEffects.length = 0
                 }
             }
-            class Sg extends ug {
+            class Cg extends dg {
                 shouldDrawLayer(t) {
                     const {
                         operation: e
                     } = t.props;
                     return e.includes("draw") || e.includes("terrain")
                 }
             }
-            const Cg = {
+            const Tg = {
                 blendFunc: [1, 0, 32771, 0],
                 blendEquation: 32774
             };
-            class Tg extends ug {
+            class Ag extends dg {
                 constructor(...t) {
                     super(...t), wo(this, "pickZ", void 0), wo(this, "_colorEncoderState", null)
                 }
                 render(t) {
                     return "pickingFBO" in t ? this._drawPickingBuffer(t) : super.render(t)
                 }
                 _drawPickingBuffer({
@@ -15994,15 +15997,15 @@
                             scissorTest: !0,
                             scissor: [o, a, l, c],
                             clearColor: [0, 0, 0, 0],
                             depthMask: !0,
                             depthTest: !0,
                             depthRange: [0, 1],
                             colorMask: [!0, !0, !0, !0],
-                            ...Cg,
+                            ...Tg,
                             blend: !p
                         }, (() => super.render({
                             target: s,
                             layers: t,
                             layerFilter: e,
                             views: n,
                             viewports: i,
@@ -16010,15 +16013,15 @@
                             cullRect: h,
                             effects: null == u ? void 0 : u.filter((t => t.useInPicking)),
                             pass: d,
                             isPicking: !0,
                             moduleParameters: f
                         })));
                     return this._colorEncoderState = null, {
-                        decodePickingColor: m && Ag.bind(null, m),
+                        decodePickingColor: m && Mg.bind(null, m),
                         stats: v
                     }
                 }
                 shouldDrawLayer(t) {
                     const {
                         pickable: e,
                         operation: n
@@ -16036,15 +16039,15 @@
                     const i = {
                             ...t.props.parameters
                         },
                         {
                             pickable: r,
                             operation: s
                         } = t.props;
-                    return this._colorEncoderState ? r && s.includes("draw") && (Object.assign(i, Cg), i.blend = !0, i.blendColor = function(t, e, n) {
+                    return this._colorEncoderState ? r && s.includes("draw") && (Object.assign(i, Tg), i.blend = !0, i.blendColor = function(t, e, n) {
                         const {
                             byLayer: i,
                             byAlpha: r
                         } = t;
                         let s, o = i.get(e);
                         return o ? (o.viewports.push(n), s = o.a) : (s = i.size + 1, s <= 255 ? (o = {
                             a: s,
@@ -16057,36 +16060,36 @@
                     return this._colorEncoderState = t ? null : {
                         byLayer: new Map,
                         byAlpha: []
                     }, this._colorEncoderState
                 }
             }
 
-            function Ag(t, e) {
+            function Mg(t, e) {
                 const n = t.byAlpha[e[3]];
                 return n && {
                     pickedLayer: n.layer,
                     pickedViewports: n.viewports,
                     pickedObjectIndex: n.layer.decodePickingColor(e)
                 }
             }
-            class Mg {
+            class Og {
                 constructor(t) {
-                    wo(this, "gl", void 0), wo(this, "layerFilter", void 0), wo(this, "drawPickingColors", void 0), wo(this, "drawLayersPass", void 0), wo(this, "pickLayersPass", void 0), wo(this, "renderCount", void 0), wo(this, "_needsRedraw", void 0), wo(this, "renderBuffers", void 0), wo(this, "lastPostProcessEffect", void 0), this.gl = t, this.layerFilter = null, this.drawPickingColors = !1, this.drawLayersPass = new Sg(t), this.pickLayersPass = new Tg(t), this.renderCount = 0, this._needsRedraw = "Initial render", this.renderBuffers = [], this.lastPostProcessEffect = null
+                    wo(this, "gl", void 0), wo(this, "layerFilter", void 0), wo(this, "drawPickingColors", void 0), wo(this, "drawLayersPass", void 0), wo(this, "pickLayersPass", void 0), wo(this, "renderCount", void 0), wo(this, "_needsRedraw", void 0), wo(this, "renderBuffers", void 0), wo(this, "lastPostProcessEffect", void 0), this.gl = t, this.layerFilter = null, this.drawPickingColors = !1, this.drawLayersPass = new Cg(t), this.pickLayersPass = new Ag(t), this.renderCount = 0, this._needsRedraw = "Initial render", this.renderBuffers = [], this.lastPostProcessEffect = null
                 }
                 setProps(t) {
                     this.layerFilter !== t.layerFilter && (this.layerFilter = t.layerFilter, this._needsRedraw = "layerFilter changed"), this.drawPickingColors !== t.drawPickingColors && (this.drawPickingColors = t.drawPickingColors, this._needsRedraw = "drawPickingColors changed")
                 }
                 renderLayers(t) {
                     const e = this.drawPickingColors ? this.pickLayersPass : this.drawLayersPass,
                         n = {
                             layerFilter: this.layerFilter,
                             isPicking: this.drawPickingColors,
                             ...t,
-                            target: t.target || bp.getDefaultFramebuffer(this.gl)
+                            target: t.target || yp.getDefaultFramebuffer(this.gl)
                         };
                     n.effects && this._preRender(n.effects, n);
                     const i = this.lastPostProcessEffect ? this.renderBuffers[0] : n.target,
                         r = e.render({
                             ...n,
                             target: i
                         });
@@ -16110,15 +16113,15 @@
                     for (const n of t) e.preRenderStats[n.id] = n.preRender(this.gl, e), n.postRender && (this.lastPostProcessEffect = n.id);
                     this.lastPostProcessEffect && this._resizeRenderBuffers()
                 }
                 _resizeRenderBuffers() {
                     const {
                         renderBuffers: t
                     } = this;
-                    0 === t.length && t.push(new bp(this.gl), new bp(this.gl));
+                    0 === t.length && t.push(new yp(this.gl), new yp(this.gl));
                     for (const e of t) e.resize()
                 }
                 _postRender(t, e) {
                     const {
                         renderBuffers: n
                     } = this, i = {
                         ...e,
@@ -16133,20 +16136,20 @@
                                 break
                             }
                             const t = r.postRender(this.gl, i);
                             i.inputBuffer = t, i.swapBuffer = t === n[0] ? n[1] : n[0]
                         }
                 }
             }
-            const Og = {
+            const Lg = {
                 pickedColor: null,
                 pickedObjectIndex: -1
             };
 
-            function Lg({
+            function Rg({
                 pickedColors: t,
                 decodePickingColor: e,
                 deviceX: n,
                 deviceY: i,
                 deviceRadius: r,
                 deviceRect: s
             }) {
@@ -16184,18 +16187,18 @@
                             pickedColor: n,
                             pickedX: o + e,
                             pickedY: a + t
                         }
                     }
                     na.error("Picked non-existent layer. Is picking buffer corrupt?")()
                 }
-                return Og
+                return Lg
             }
 
-            function Rg({
+            function Ig({
                 pickInfo: t,
                 viewports: e,
                 pixelRatio: n,
                 x: i,
                 y: r,
                 z: s
             }) {
@@ -16224,15 +16227,15 @@
                     pixel: [i, r],
                     coordinate: o,
                     devicePixel: t && "pickedX" in t ? [t.pickedX, t.pickedY] : void 0,
                     pixelRatio: n
                 }
             }
 
-            function Ig(t) {
+            function kg(t) {
                 const {
                     pickInfo: e,
                     lastPickedInfo: n,
                     mode: i,
                     layers: r
                 } = t, {
                     pickedColor: s,
@@ -16247,48 +16250,48 @@
                         if (i !== e) {
                             const t = r.find((t => t.props.id === e));
                             t && l.unshift(t)
                         }
                         n.layerId = i, n.index = a, n.info = null
                     }
                 }
-                const c = Rg(t),
+                const c = Ig(t),
                     h = new Map;
                 return h.set(null, c), l.forEach((t => {
                     let e = {
                         ...c
                     };
-                    t === o && (e.color = s, e.index = a, e.picked = !0), e = kg({
+                    t === o && (e.color = s, e.index = a, e.picked = !0), e = jg({
                         layer: t,
                         info: e,
                         mode: i
                     });
                     const r = e.layer;
                     t === o && "hover" === i && (n.info = e), h.set(r.id, e), "hover" === i && r.updateAutoHighlight(e)
                 })), h
             }
 
-            function kg({
+            function jg({
                 layer: t,
                 info: e,
                 mode: n
             }) {
                 for (; t && e;) {
                     const i = e.layer || null;
                     e.sourceLayer = i, e.layer = t, e = t.getPickingInfo({
                         info: e,
                         mode: n,
                         sourceLayer: i
                     }), t = t.parent
                 }
                 return e
             }
-            class jg {
+            class Fg {
                 constructor(t) {
-                    wo(this, "gl", void 0), wo(this, "pickingFBO", void 0), wo(this, "depthFBO", void 0), wo(this, "pickLayersPass", void 0), wo(this, "layerFilter", void 0), wo(this, "lastPickedInfo", void 0), wo(this, "_pickable", !0), this.gl = t, this.pickLayersPass = new Tg(t), this.lastPickedInfo = {
+                    wo(this, "gl", void 0), wo(this, "pickingFBO", void 0), wo(this, "depthFBO", void 0), wo(this, "pickLayersPass", void 0), wo(this, "layerFilter", void 0), wo(this, "lastPickedInfo", void 0), wo(this, "_pickable", !0), this.gl = t, this.pickLayersPass = new Ag(t), this.lastPickedInfo = {
                         index: -1,
                         layerId: null,
                         info: null
                     }
                 }
                 setProps(t) {
                     "layerFilter" in t && (this.layerFilter = t.layerFilter), "_pickable" in t && (this._pickable = t._pickable)
@@ -16326,20 +16329,20 @@
                     }
                 }
                 _resizeBuffer() {
                     var t, e;
                     const {
                         gl: n
                     } = this;
-                    if (!this.pickingFBO && (this.pickingFBO = new bp(n), bp.isSupported(n, {
+                    if (!this.pickingFBO && (this.pickingFBO = new yp(n), yp.isSupported(n, {
                             colorBufferFloat: !0
                         }))) {
-                        const t = new bp(n);
+                        const t = new yp(n);
                         t.attach({
-                            36064: new Qd(n, {
+                            36064: new Jd(n, {
                                 format: Lu(n) ? 34836 : 6408,
                                 type: 5126
                             })
                         }), this.depthFBO = t
                     }
                     null === (t = this.pickingFBO) || void 0 === t || t.resize({
                         width: n.canvas.width,
@@ -16367,15 +16370,15 @@
                     onViewportActive: c,
                     effects: h
                 }) {
                     const u = this._getPickable(t),
                         d = dd(this.gl);
                     if (!u) return {
                         result: [],
-                        emptyInfo: Rg({
+                        emptyInfo: Ig({
                             viewports: n,
                             x: i,
                             y: r,
                             pixelRatio: d
                         })
                     };
                     this._resizeBuffer();
@@ -16400,15 +16403,15 @@
                             height: 2 * s + 1
                         };
                     let _;
                     const x = [],
                         w = new Set;
                     for (let t = 0; t < o; t++) {
                         let s, p;
-                        if (s = b ? Lg({
+                        if (s = b ? Rg({
                                 ...this._drawAndSample({
                                     layers: u,
                                     views: e,
                                     viewports: n,
                                     onViewportActive: c,
                                     deviceRect: b,
                                     cullRect: y,
@@ -16438,15 +16441,15 @@
                                 },
                                 cullRect: y,
                                 effects: h,
                                 pass: "picking:".concat(a, ":z")
                             }, !0);
                             t[3] && (p = t[0])
                         }
-                        s.pickedLayer && t + 1 < o && (w.add(s.pickedLayer), s.pickedLayer.disablePickingIndex(s.pickedObjectIndex)), _ = Ig({
+                        s.pickedLayer && t + 1 < o && (w.add(s.pickedLayer), s.pickedLayer.disablePickingIndex(s.pickedObjectIndex)), _ = kg({
                             pickInfo: s,
                             lastPickedInfo: this.lastPickedInfo,
                             mode: a,
                             layers: u,
                             viewports: n,
                             x: i,
                             y: r,
@@ -16533,15 +16536,15 @@
                             layer: null,
                             index: e.pickedObjectIndex,
                             picked: !0,
                             x: i,
                             y: r,
                             pixelRatio: d
                         };
-                        n = kg({
+                        n = jg({
                             layer: e.pickedLayer,
                             info: n,
                             mode: a
                         }), x.has(n.object) || x.set(n.object, n)
                     }
                     return Array.from(x.values())
                 }
@@ -16575,15 +16578,15 @@
                         decodePickingColor: u
                     } = this.pickLayersPass.render(h), {
                         x: d,
                         y: p,
                         width: f,
                         height: g
                     } = r, m = new(l ? Float32Array : Uint8Array)(f * g * 4);
-                    return lp(c, {
+                    return cp(c, {
                         sourceX: d,
                         sourceY: p,
                         sourceWidth: f,
                         sourceHeight: g,
                         target: m
                     }), {
                         pickedColors: m,
@@ -16605,30 +16608,30 @@
                         x: s,
                         y: o,
                         width: a,
                         height: l
                     }
                 }
             }
-            const Fg = {
+            const zg = {
                 zIndex: "1",
                 position: "absolute",
                 pointerEvents: "none",
                 color: "#a0a7b4",
                 backgroundColor: "#29323c",
                 padding: "10px",
                 top: "0",
                 left: "0",
                 display: "none"
             };
-            class zg {
+            class Bg {
                 constructor(t) {
                     wo(this, "el", null), wo(this, "isVisible", !1);
                     const e = t.parentElement;
-                    e && (this.el = document.createElement("div"), this.el.className = "deck-tooltip", Object.assign(this.el.style, Fg), e.appendChild(this.el))
+                    e && (this.el = document.createElement("div"), this.el.className = "deck-tooltip", Object.assign(this.el.style, zg), e.appendChild(this.el))
                 }
                 setTooltip(t, e, n) {
                     const i = this.el;
                     if (i) {
                         if ("string" == typeof t) i.innerText = t;
                         else {
                             if (!t) return this.isVisible = !1, void(i.style.display = "none");
@@ -16638,47 +16641,47 @@
                     }
                 }
                 remove() {
                     this.el && (this.el.remove(), this.el = null)
                 }
             }
             const {
-                _parseImageNode: Bg
-            } = globalThis, Dg = "undefined" != typeof Image, Ng = "undefined" != typeof ImageBitmap, Vg = Boolean(Bg), Ug = !!ol || Vg;
+                _parseImageNode: Dg
+            } = globalThis, Ng = "undefined" != typeof Image, Vg = "undefined" != typeof ImageBitmap, Ug = Boolean(Dg), Gg = !!ol || Ug;
 
-            function Gg(t) {
+            function Wg(t) {
                 const e = function(t) {
                     return "undefined" != typeof ImageBitmap && t instanceof ImageBitmap ? "imagebitmap" : "undefined" != typeof Image && t instanceof Image ? "image" : t && "object" == typeof t && t.data && t.width && t.height ? "data" : null
                 }(t);
                 if (!e) throw new Error("Not an image");
                 return e
             }
-            const Wg = /^data:image\/svg\+xml/,
-                Hg = /\.svg((\?|#).*)?$/;
+            const Hg = /^data:image\/svg\+xml/,
+                Zg = /\.svg((\?|#).*)?$/;
 
-            function Zg(t) {
-                return t && (Wg.test(t) || Hg.test(t))
+            function qg(t) {
+                return t && (Hg.test(t) || Zg.test(t))
             }
 
-            function qg(t, e) {
-                if (Zg(e)) throw new Error("SVG cannot be parsed directly to imagebitmap");
+            function Xg(t, e) {
+                if (qg(e)) throw new Error("SVG cannot be parsed directly to imagebitmap");
                 return new Blob([new Uint8Array(t)])
             }
-            async function Xg(t, e, n) {
+            async function Yg(t, e, n) {
                 const i = function(t, e) {
-                        if (Zg(e)) {
+                        if (qg(e)) {
                             let e = (new TextDecoder).decode(t);
                             try {
                                 "function" == typeof unescape && "function" == typeof encodeURIComponent && (e = unescape(encodeURIComponent(e)))
                             } catch (t) {
                                 throw new Error(t.message)
                             }
                             return "data:image/svg+xml;base64,".concat(btoa(e))
                         }
-                        return qg(t, e)
+                        return Xg(t, e)
                     }(t, n),
                     r = self.URL || self.webkitURL,
                     s = "string" != typeof i && r.createObjectURL(i);
                 try {
                     return await async function(t, e) {
                         const n = new Image;
                         return n.src = t, e.image && e.image.decode && n.decode ? (await n.decode(), n) : await new Promise(((e, i) => {
@@ -16689,67 +16692,67 @@
                             }
                         }))
                     }(s || i, e)
                 } finally {
                     s && r.revokeObjectURL(s)
                 }
             }
-            const Yg = {};
-            let Kg = !0;
-            const Qg = !1,
-                Jg = !0;
+            const Kg = {};
+            let Qg = !0;
+            const Jg = !1,
+                $g = !0;
 
-            function $g(t) {
-                const e = tm(t);
+            function tm(t) {
+                const e = em(t);
                 return function(t) {
-                    const e = tm(t);
-                    return e.byteLength >= 24 && 2303741511 === e.getUint32(0, Qg) ? {
+                    const e = em(t);
+                    return e.byteLength >= 24 && 2303741511 === e.getUint32(0, Jg) ? {
                         mimeType: "image/png",
-                        width: e.getUint32(16, Qg),
-                        height: e.getUint32(20, Qg)
+                        width: e.getUint32(16, Jg),
+                        height: e.getUint32(20, Jg)
                     } : null
                 }(e) || function(t) {
-                    const e = tm(t);
-                    if (!(e.byteLength >= 3 && 65496 === e.getUint16(0, Qg) && 255 === e.getUint8(2))) return null;
+                    const e = em(t);
+                    if (!(e.byteLength >= 3 && 65496 === e.getUint16(0, Jg) && 255 === e.getUint8(2))) return null;
                     const {
                         tableMarkers: n,
                         sofMarkers: i
                     } = function() {
                         const t = new Set([65499, 65476, 65484, 65501, 65534]);
                         for (let e = 65504; e < 65520; ++e) t.add(e);
                         return {
                             tableMarkers: t,
                             sofMarkers: new Set([65472, 65473, 65474, 65475, 65477, 65478, 65479, 65481, 65482, 65483, 65485, 65486, 65487, 65502])
                         }
                     }();
                     let r = 2;
                     for (; r + 9 < e.byteLength;) {
-                        const t = e.getUint16(r, Qg);
+                        const t = e.getUint16(r, Jg);
                         if (i.has(t)) return {
                             mimeType: "image/jpeg",
-                            height: e.getUint16(r + 5, Qg),
-                            width: e.getUint16(r + 7, Qg)
+                            height: e.getUint16(r + 5, Jg),
+                            width: e.getUint16(r + 7, Jg)
                         };
                         if (!n.has(t)) return null;
-                        r += 2, r += e.getUint16(r, Qg)
+                        r += 2, r += e.getUint16(r, Jg)
                     }
                     return null
                 }(e) || function(t) {
-                    const e = tm(t);
-                    return e.byteLength >= 10 && 1195984440 === e.getUint32(0, Qg) ? {
+                    const e = em(t);
+                    return e.byteLength >= 10 && 1195984440 === e.getUint32(0, Jg) ? {
                         mimeType: "image/gif",
-                        width: e.getUint16(6, Jg),
-                        height: e.getUint16(8, Jg)
+                        width: e.getUint16(6, $g),
+                        height: e.getUint16(8, $g)
                     } : null
                 }(e) || function(t) {
-                    const e = tm(t);
-                    return e.byteLength >= 14 && 16973 === e.getUint16(0, Qg) && e.getUint32(2, Jg) === e.byteLength ? {
+                    const e = em(t);
+                    return e.byteLength >= 14 && 16973 === e.getUint16(0, Jg) && e.getUint32(2, $g) === e.byteLength ? {
                         mimeType: "image/bmp",
-                        width: e.getUint32(18, Jg),
-                        height: e.getUint32(22, Jg)
+                        width: e.getUint32(18, $g),
+                        height: e.getUint32(22, $g)
                     } : null
                 }(e) || function(t) {
                     const e = function(t) {
                         return function(t, e) {
                             let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : 0;
                             const i = (r = e, [...r].map((t => t.charCodeAt(0))));
                             var r;
@@ -16773,21 +16776,21 @@
                         mimeType: e.mimeType,
                         width: 0,
                         height: 0
                     } : null
                 }(e)
             }
 
-            function tm(t) {
+            function em(t) {
                 if (t instanceof DataView) return t;
                 if (ArrayBuffer.isView(t)) return new DataView(t.buffer);
                 if (t instanceof ArrayBuffer) return new DataView(t);
                 throw new Error("toDataView")
             }
-            const em = {
+            const nm = {
                     id: "image",
                     module: "images",
                     name: "Images",
                     version: "3.4.4",
                     mimeTypes: ["image/png", "image/jpeg", "image/gif", "image/webp", "image/avif", "image/bmp", "image/vnd.microsoft.icon", "image/svg+xml"],
                     extensions: ["png", "jpg", "jpeg", "gif", "webp", "bmp", "ico", "svg", "avif"],
                     parse: async function(t, e, n) {
@@ -16797,108 +16800,108 @@
                             } = n || {};
                         let s;
                         switch (function(t) {
                                 switch (t) {
                                     case "auto":
                                     case "data":
                                         return function() {
-                                            if (Ng) return "imagebitmap";
-                                            if (Dg) return "image";
-                                            if (Ug) return "data";
+                                            if (Vg) return "imagebitmap";
+                                            if (Ng) return "image";
+                                            if (Gg) return "data";
                                             throw new Error("Install '@loaders.gl/polyfills' to parse images under Node.js")
                                         }();
                                     default:
                                         return function(t) {
                                             switch (t) {
                                                 case "auto":
-                                                    return Ng || Dg || Ug;
+                                                    return Vg || Ng || Gg;
                                                 case "imagebitmap":
-                                                    return Ng;
+                                                    return Vg;
                                                 case "image":
-                                                    return Dg;
+                                                    return Ng;
                                                 case "data":
-                                                    return Ug;
+                                                    return Gg;
                                                 default:
                                                     throw new Error("@loaders.gl/images: image ".concat(t, " not supported in this environment"))
                                             }
                                         }(t), t
                                 }
                             }(i)) {
                             case "imagebitmap":
                                 s = await async function(t, e, n) {
                                     let i;
-                                    i = Zg(n) ? await Xg(t, e, n) : qg(t, n);
+                                    i = qg(n) ? await Yg(t, e, n) : Xg(t, n);
                                     const r = e && e.imagebitmap;
                                     return await async function(t) {
                                         let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : null;
                                         if (! function(t) {
-                                                for (const e in t || Yg) return !1;
+                                                for (const e in t || Kg) return !1;
                                                 return !0
-                                            }(e) && Kg || (e = null), e) try {
+                                            }(e) && Qg || (e = null), e) try {
                                             return await createImageBitmap(t, e)
                                         } catch (t) {
-                                            console.warn(t), Kg = !1
+                                            console.warn(t), Qg = !1
                                         }
                                         return await createImageBitmap(t)
                                     }(i, r)
                                 }(t, e, r);
                                 break;
                             case "image":
-                                s = await Xg(t, e, r);
+                                s = await Yg(t, e, r);
                                 break;
                             case "data":
                                 s = await async function(t, e) {
                                     const {
                                         mimeType: n
-                                    } = $g(t) || {}, i = globalThis._parseImageNode;
+                                    } = tm(t) || {}, i = globalThis._parseImageNode;
                                     return wa(i), await i(t, n)
                                 }(t);
                                 break;
                             default:
                                 wa(!1)
                         }
                         return "data" === i && (s = function(t) {
-                            switch (Gg(t)) {
+                            switch (Wg(t)) {
                                 case "data":
                                     return t;
                                 case "image":
                                 case "imagebitmap":
                                     const e = document.createElement("canvas"),
                                         n = e.getContext("2d");
                                     if (!n) throw new Error("getImageData");
                                     return e.width = t.width, e.height = t.height, n.drawImage(t, 0, 0), n.getImageData(0, 0, t.width, t.height);
                                 default:
                                     throw new Error("getImageData")
                             }
                         }(s)), s
                     },
-                    tests: [t => Boolean($g(new DataView(t)))],
+                    tests: [t => Boolean(tm(new DataView(t)))],
                     options: {
                         image: {
                             type: "auto",
                             decode: !0
                         }
                     }
                 },
-                nm = {
+                im = {
                     id: "JSON",
                     name: "JSON",
                     module: "",
                     version: "",
                     options: {},
                     extensions: ["json", "geojson"],
                     mimeTypes: ["application/json", "application/geo+json"],
                     testText: function(t) {
                         const e = t[0],
                             n = t[t.length - 1];
                         return "{" === e && "}" === n || "[" === e && "]" === n
                     },
                     parseTextSync: JSON.parse
                 },
-                im = function() {
+                rm = function() {
                     const t = "8.9.16",
                         e = globalThis.deck && globalThis.deck.VERSION;
                     if (e && e !== t) throw new Error("deck.gl - multiple versions detected: ".concat(e, " vs ").concat(t));
                     return e || (na.log(1, "deck.gl ".concat(t))(), globalThis.deck = {
                         ...globalThis.deck,
                         VERSION: t,
                         version: t,
@@ -16907,50 +16910,50 @@
                     }, function(t) {
                         const e = Hl();
                         t = Array.isArray(t) ? t : [t];
                         for (const n of t) {
                             const t = Pa(n);
                             e.find((e => t === e)) || e.unshift(t)
                         }
-                    }([nm, [em, {
+                    }([im, [nm, {
                         imagebitmap: {
                             premultiplyAlpha: "none"
                         }
                     }]])), t
                 }(),
-                rm = globalThis;
+                sm = globalThis;
 
-            function sm(t) {
+            function om(t) {
                 if (!t && !jo()) return "Node";
                 if (Io(t)) return "Electron";
                 const e = "undefined" != typeof navigator ? navigator : {},
                     n = t || e.userAgent || "";
                 if (n.indexOf("Edge") > -1) return "Edge";
                 const i = -1 !== n.indexOf("MSIE "),
                     r = -1 !== n.indexOf("Trident/");
-                return i || r ? "IE" : rm.chrome ? "Chrome" : rm.safari ? "Safari" : rm.mozInnerScreenX ? "Firefox" : "Unknown"
+                return i || r ? "IE" : sm.chrome ? "Chrome" : sm.safari ? "Safari" : sm.mozInnerScreenX ? "Firefox" : "Unknown"
             }
-            class om extends Rd {
+            class am extends Id {
                 get[Symbol.toStringTag]() {
                     return "Query"
                 }
                 static isSupported(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : [];
                     const n = Lu(t),
-                        i = gp(t, up);
+                        i = mp(t, dp);
                     let r = n || i;
                     for (const t of e) switch (t) {
                         case "queries":
                             r = r && n;
                             break;
                         case "timers":
                             r = r && i;
                             break;
                         default:
-                            Ed(!1)
+                            Pd(!1)
                     }
                     return r
                 }
                 constructor(t) {
                     super(t, arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {}), this.target = null, this._queryPending = !1, this._pollingPromise = null, Object.seal(this)
                 }
                 beginTimeElapsedQuery() {
@@ -16993,23 +16996,23 @@
                         const r = () => {
                             this.isResultAvailable() ? (n(this.getResult()), this._pollingPromise = null) : e++ > t ? (i("Timed out"), this._pollingPromise = null) : requestAnimationFrame(r)
                         };
                         requestAnimationFrame(r)
                     })), this._pollingPromise
                 }
                 _createHandle() {
-                    return om.isSupported(this.gl) ? this.gl2.createQuery() : null
+                    return am.isSupported(this.gl) ? this.gl2.createQuery() : null
                 }
                 _deleteHandle() {
                     this.gl2.deleteQuery(this.handle)
                 }
             }
-            const am = jo() && "undefined" != typeof document;
-            let lm = 0;
-            class cm {
+            const lm = jo() && "undefined" != typeof document;
+            let cm = 0;
+            class hm {
                 constructor() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     const {
                         onCreateContext: e = (t => yd(t)),
                         onAddHTML: n = null,
                         onInitialize: i = (() => {}),
                         onRender: r = (() => {}),
@@ -17017,15 +17020,15 @@
                         onError: o,
                         gl: a = null,
                         glOptions: l = {},
                         debug: c = !1,
                         createFramebuffer: h = !1,
                         autoResizeViewport: u = !0,
                         autoResizeDrawingBuffer: d = !0,
-                        stats: p = wd.get("animation-loop-".concat(lm++))
+                        stats: p = Ed.get("animation-loop-".concat(cm++))
                     } = t;
                     let {
                         useDevicePixels: f = !0
                     } = t;
                     "useDevicePixelRatio" in t && (Tu.deprecated("useDevicePixelRatio", "useDevicePixels")(), f = t.useDevicePixelRatio), this.props = {
                         onCreateContext: e,
                         onAddHTML: n,
@@ -17043,24 +17046,24 @@
                         useDevicePixels: f
                     }), this.start = this.start.bind(this), this.stop = this.stop.bind(this), this._pageLoadPromise = null, this._onMousemove = this._onMousemove.bind(this), this._onMouseleave = this._onMouseleave.bind(this)
                 }
                 delete() {
                     this.stop(), this._setDisplay(null)
                 }
                 setNeedsRedraw(t) {
-                    return Ed("string" == typeof t), this.needsRedraw = this.needsRedraw || t, this
+                    return Pd("string" == typeof t), this.needsRedraw = this.needsRedraw || t, this
                 }
                 setProps(t) {
                     return "autoResizeViewport" in t && (this.autoResizeViewport = t.autoResizeViewport), "autoResizeDrawingBuffer" in t && (this.autoResizeDrawingBuffer = t.autoResizeDrawingBuffer), "useDevicePixels" in t && (this.useDevicePixels = t.useDevicePixels), this
                 }
                 start() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     if (this._running) return this;
                     this._running = !0;
-                    const e = this._getPageLoadPromise().then((() => !this._running || this._initialized ? null : (this._createWebGLContext(t), this._createFramebuffer(), this._startEventHandling(), this._initializeCallbackData(), this._updateCallbackData(), this._resizeCanvasDrawingBuffer(), this._resizeViewport(), this._gpuTimeQuery = om.isSupported(this.gl, ["timers"]) ? new om(this.gl) : null, this._initialized = !0, this.onInitialize(this.animationProps)))).then((t => {
+                    const e = this._getPageLoadPromise().then((() => !this._running || this._initialized ? null : (this._createWebGLContext(t), this._createFramebuffer(), this._startEventHandling(), this._initializeCallbackData(), this._updateCallbackData(), this._resizeCanvasDrawingBuffer(), this._resizeViewport(), this._gpuTimeQuery = am.isSupported(this.gl, ["timers"]) ? new am(this.gl) : null, this._initialized = !0, this.onInitialize(this.animationProps)))).then((t => {
                         this._running && (this._addCallbackData(t || {}), !1 !== t && this._startLoop())
                     }));
                     return this.props.onError && e.catch(this.props.onError), this
                 }
                 redraw() {
                     return this.isContextLost() || (this._beginTimers(), this._setupFrame(), this._updateCallbackData(), this._renderFrame(this.animationProps), this._clearNeedsRedraw(), this.offScreen && this.gl.commit && this.gl.commit(), this._resolveNextFrame && (this._resolveNextFrame(this), this._nextFramePromise = null, this._resolveNextFrame = null), this._endTimers()), this
                 }
@@ -17107,16 +17110,16 @@
                 _startLoop() {
                     const t = () => {
                         this._running && (this.redraw(), this._animationFrameId = this._requestAnimationFrame(t))
                     };
                     this._cancelAnimationFrame(this._animationFrameId), this._animationFrameId = this._requestAnimationFrame(t)
                 }
                 _getPageLoadPromise() {
-                    return this._pageLoadPromise || (this._pageLoadPromise = am ? new Promise(((t, e) => {
-                        am && "complete" === document.readyState ? t(document) : window.addEventListener("load", (() => {
+                    return this._pageLoadPromise || (this._pageLoadPromise = lm ? new Promise(((t, e) => {
+                        lm && "complete" === document.readyState ? t(document) : window.addEventListener("load", (() => {
                             t(document)
                         }))
                     })) : Promise.resolve({})), this._pageLoadPromise
                 }
                 _setDisplay(t) {
                     this.display && (this.display.delete(), this.display.animationLoop = null), t && (t.animationLoop = this), this.display = t
                 }
@@ -17226,15 +17229,15 @@
                         const n = t.getExtension("STACKGL_resize_drawingbuffer");
                         n && "width" in e && "height" in e && n.resize(e.width, e.height)
                     }(this.gl, {
                         useDevicePixels: this.useDevicePixels
                     })
                 }
                 _createFramebuffer() {
-                    this.props.createFramebuffer && (this.framebuffer = new bp(this.gl))
+                    this.props.createFramebuffer && (this.framebuffer = new yp(this.gl))
                 }
                 _resizeFramebuffer() {
                     this.framebuffer && this.framebuffer.resize({
                         width: this.gl.drawingBufferWidth,
                         height: this.gl.drawingBufferHeight
                     })
                 }
@@ -17253,113 +17256,113 @@
                 _onMousemove(t) {
                     this.animationProps._mousePosition = [t.offsetX, t.offsetY]
                 }
                 _onMouseleave(t) {
                     this.animationProps._mousePosition = null
                 }
             }
-            var hm = n(840);
-            const um = {
+            var um = n(840);
+            const dm = {
                 mousedown: 1,
                 mousemove: 2,
                 mouseup: 4
             };
             ! function(t) {
                 const e = t.prototype.handler;
                 t.prototype.handler = function(t) {
                     const n = this.store;
                     t.button > 0 && "pointerdown" === t.type && (function(e, n) {
                         for (let n = 0; n < e.length; n++)
                             if (e[n].pointerId === t.pointerId) return !0;
                         return !1
                     }(n) || n.push(t)), e.call(this, t)
                 }
-            }(hm.PointerEventInput), hm.MouseInput.prototype.handler = function(t) {
-                let e = um[t.type];
+            }(um.PointerEventInput), um.MouseInput.prototype.handler = function(t) {
+                let e = dm[t.type];
                 1 & e && t.button >= 0 && (this.pressed = !0), 2 & e && 0 === t.which && (e = 4), this.pressed && (4 & e && (this.pressed = !1), this.callback(this.manager, e, {
                     pointers: [t],
                     changedPointers: [t],
                     pointerType: "mouse",
                     srcEvent: t
                 }))
             };
-            const dm = hm.Manager,
-                pm = hm;
-            class fm {
+            const pm = um.Manager,
+                fm = um;
+            class gm {
                 constructor(t, e, n) {
                     this.element = t, this.callback = e, this.options = {
                         enable: !0,
                         ...n
                     }
                 }
             }
-            const gm = pm ? [
-                    [pm.Pan, {
+            const mm = fm ? [
+                    [fm.Pan, {
                         event: "tripan",
                         pointers: 3,
                         threshold: 0,
                         enable: !1
                     }],
-                    [pm.Rotate, {
+                    [fm.Rotate, {
                         enable: !1
                     }],
-                    [pm.Pinch, {
+                    [fm.Pinch, {
                         enable: !1
                     }],
-                    [pm.Swipe, {
+                    [fm.Swipe, {
                         enable: !1
                     }],
-                    [pm.Pan, {
+                    [fm.Pan, {
                         threshold: 0,
                         enable: !1
                     }],
-                    [pm.Press, {
+                    [fm.Press, {
                         enable: !1
                     }],
-                    [pm.Tap, {
+                    [fm.Tap, {
                         event: "doubletap",
                         taps: 2,
                         enable: !1
                     }],
-                    [pm.Tap, {
+                    [fm.Tap, {
                         event: "anytap",
                         enable: !1
                     }],
-                    [pm.Tap, {
+                    [fm.Tap, {
                         enable: !1
                     }]
                 ] : null,
-                mm = {
+                vm = {
                     tripan: ["rotate", "pinch", "pan"],
                     rotate: ["pinch"],
                     pinch: ["pan"],
                     pan: ["press", "doubletap", "anytap", "tap"],
                     doubletap: ["anytap"],
                     anytap: ["tap"]
                 },
-                vm = {
+                bm = {
                     doubletap: ["tap"]
                 },
-                bm = {
+                ym = {
                     pointerdown: "pointerdown",
                     pointermove: "pointermove",
                     pointerup: "pointerup",
                     touchstart: "pointerdown",
                     touchmove: "pointermove",
                     touchend: "pointerup",
                     mousedown: "pointerdown",
                     mousemove: "pointermove",
                     mouseup: "pointerup"
                 },
-                ym = {
+                _m = {
                     KEY_EVENTS: ["keydown", "keyup"],
                     MOUSE_EVENTS: ["mousedown", "mousemove", "mouseup", "mouseover", "mouseout", "mouseleave"],
                     WHEEL_EVENTS: ["wheel", "mousewheel"]
                 },
-                _m = {
+                xm = {
                     tap: "tap",
                     anytap: "anytap",
                     doubletap: "doubletap",
                     press: "press",
                     pinch: "pinch",
                     pinchin: "pinch",
                     pinchout: "pinch",
@@ -17392,110 +17395,110 @@
                     pancancel: "pan",
                     swipe: "swipe",
                     swipeleft: "swipe",
                     swiperight: "swipe",
                     swipeup: "swipe",
                     swipedown: "swipe"
                 },
-                xm = {
+                wm = {
                     click: "tap",
                     anyclick: "anytap",
                     dblclick: "doubletap",
                     mousedown: "pointerdown",
                     mousemove: "pointermove",
                     mouseup: "pointerup",
                     mouseover: "pointerover",
                     mouseout: "pointerout",
                     mouseleave: "pointerleave"
                 },
-                wm = "undefined" != typeof navigator && navigator.userAgent ? navigator.userAgent.toLowerCase() : "",
-                Em = "undefined" != typeof window ? window : n.g;
+                Em = "undefined" != typeof navigator && navigator.userAgent ? navigator.userAgent.toLowerCase() : "",
+                Pm = "undefined" != typeof window ? window : n.g;
             void 0 !== n.g ? n.g : window, "undefined" != typeof document && document;
-            let Pm = !1;
+            let Sm = !1;
             try {
                 const t = {
                     get passive() {
-                        return Pm = !0, !0
+                        return Sm = !0, !0
                     }
                 };
-                Em.addEventListener("test", null, t), Em.removeEventListener("test", null)
+                Pm.addEventListener("test", null, t), Pm.removeEventListener("test", null)
             } catch (t) {
-                Pm = !1
+                Sm = !1
             }
-            const Sm = -1 !== wm.indexOf("firefox"),
+            const Cm = -1 !== Em.indexOf("firefox"),
                 {
-                    WHEEL_EVENTS: Cm
-                } = ym,
-                Tm = "wheel",
-                Am = 4.000244140625;
-            class Mm extends fm {
+                    WHEEL_EVENTS: Tm
+                } = _m,
+                Am = "wheel",
+                Mm = 4.000244140625;
+            class Om extends gm {
                 constructor(t, e, n) {
                     super(t, e, n), this.handleEvent = t => {
                         if (!this.options.enable) return;
                         let e = t.deltaY;
-                        Em.WheelEvent && (Sm && t.deltaMode === Em.WheelEvent.DOM_DELTA_PIXEL && (e /= Em.devicePixelRatio), t.deltaMode === Em.WheelEvent.DOM_DELTA_LINE && (e *= 40)), 0 !== e && e % Am == 0 && (e = Math.floor(e / Am)), t.shiftKey && e && (e *= .25), this.callback({
-                            type: Tm,
+                        Pm.WheelEvent && (Cm && t.deltaMode === Pm.WheelEvent.DOM_DELTA_PIXEL && (e /= Pm.devicePixelRatio), t.deltaMode === Pm.WheelEvent.DOM_DELTA_LINE && (e *= 40)), 0 !== e && e % Mm == 0 && (e = Math.floor(e / Mm)), t.shiftKey && e && (e *= .25), this.callback({
+                            type: Am,
                             center: {
                                 x: t.clientX,
                                 y: t.clientY
                             },
                             delta: -e,
                             srcEvent: t,
                             pointerType: "mouse",
                             target: t.target
                         })
-                    }, this.events = (this.options.events || []).concat(Cm), this.events.forEach((e => t.addEventListener(e, this.handleEvent, !!Pm && {
+                    }, this.events = (this.options.events || []).concat(Tm), this.events.forEach((e => t.addEventListener(e, this.handleEvent, !!Sm && {
                         passive: !1
                     })))
                 }
                 destroy() {
                     this.events.forEach((t => this.element.removeEventListener(t, this.handleEvent)))
                 }
                 enableEventType(t, e) {
-                    t === Tm && (this.options.enable = e)
+                    t === Am && (this.options.enable = e)
                 }
             }
             const {
-                MOUSE_EVENTS: Om
-            } = ym, Lm = "pointermove", Rm = "pointerover", Im = "pointerout", km = "pointerenter", jm = "pointerleave";
-            class Fm extends fm {
+                MOUSE_EVENTS: Lm
+            } = _m, Rm = "pointermove", Im = "pointerover", km = "pointerout", jm = "pointerenter", Fm = "pointerleave";
+            class zm extends gm {
                 constructor(t, e, n) {
                     super(t, e, n), this.handleEvent = t => {
                         this.handleOverEvent(t), this.handleOutEvent(t), this.handleEnterEvent(t), this.handleLeaveEvent(t), this.handleMoveEvent(t)
                     }, this.pressed = !1;
                     const {
                         enable: i
                     } = this.options;
-                    this.enableMoveEvent = i, this.enableLeaveEvent = i, this.enableEnterEvent = i, this.enableOutEvent = i, this.enableOverEvent = i, this.events = (this.options.events || []).concat(Om), this.events.forEach((e => t.addEventListener(e, this.handleEvent)))
+                    this.enableMoveEvent = i, this.enableLeaveEvent = i, this.enableEnterEvent = i, this.enableOutEvent = i, this.enableOverEvent = i, this.events = (this.options.events || []).concat(Lm), this.events.forEach((e => t.addEventListener(e, this.handleEvent)))
                 }
                 destroy() {
                     this.events.forEach((t => this.element.removeEventListener(t, this.handleEvent)))
                 }
                 enableEventType(t, e) {
-                    t === Lm && (this.enableMoveEvent = e), t === Rm && (this.enableOverEvent = e), t === Im && (this.enableOutEvent = e), t === km && (this.enableEnterEvent = e), t === jm && (this.enableLeaveEvent = e)
+                    t === Rm && (this.enableMoveEvent = e), t === Im && (this.enableOverEvent = e), t === km && (this.enableOutEvent = e), t === jm && (this.enableEnterEvent = e), t === Fm && (this.enableLeaveEvent = e)
                 }
                 handleOverEvent(t) {
-                    this.enableOverEvent && "mouseover" === t.type && this._emit(Rm, t)
+                    this.enableOverEvent && "mouseover" === t.type && this._emit(Im, t)
                 }
                 handleOutEvent(t) {
-                    this.enableOutEvent && "mouseout" === t.type && this._emit(Im, t)
+                    this.enableOutEvent && "mouseout" === t.type && this._emit(km, t)
                 }
                 handleEnterEvent(t) {
-                    this.enableEnterEvent && "mouseenter" === t.type && this._emit(km, t)
+                    this.enableEnterEvent && "mouseenter" === t.type && this._emit(jm, t)
                 }
                 handleLeaveEvent(t) {
-                    this.enableLeaveEvent && "mouseleave" === t.type && this._emit(jm, t)
+                    this.enableLeaveEvent && "mouseleave" === t.type && this._emit(Fm, t)
                 }
                 handleMoveEvent(t) {
                     if (this.enableMoveEvent) switch (t.type) {
                         case "mousedown":
                             t.button >= 0 && (this.pressed = !0);
                             break;
                         case "mousemove":
-                            0 === t.which && (this.pressed = !1), this.pressed || this._emit(Lm, t);
+                            0 === t.which && (this.pressed = !1), this.pressed || this._emit(Rm, t);
                             break;
                         case "mouseup":
                             this.pressed = !1
                     }
                 }
                 _emit(t, e) {
                     this.callback({
@@ -17507,74 +17510,74 @@
                         srcEvent: e,
                         pointerType: "mouse",
                         target: e.target
                     })
                 }
             }
             const {
-                KEY_EVENTS: zm
-            } = ym, Bm = "keydown", Dm = "keyup";
-            class Nm extends fm {
+                KEY_EVENTS: Bm
+            } = _m, Dm = "keydown", Nm = "keyup";
+            class Vm extends gm {
                 constructor(t, e, n) {
                     super(t, e, n), this.handleEvent = t => {
                         const e = t.target || t.srcElement;
                         "INPUT" === e.tagName && "text" === e.type || "TEXTAREA" === e.tagName || (this.enableDownEvent && "keydown" === t.type && this.callback({
-                            type: Bm,
+                            type: Dm,
                             srcEvent: t,
                             key: t.key,
                             target: t.target
                         }), this.enableUpEvent && "keyup" === t.type && this.callback({
-                            type: Dm,
+                            type: Nm,
                             srcEvent: t,
                             key: t.key,
                             target: t.target
                         }))
-                    }, this.enableDownEvent = this.options.enable, this.enableUpEvent = this.options.enable, this.events = (this.options.events || []).concat(zm), t.tabIndex = this.options.tabIndex || 0, t.style.outline = "none", this.events.forEach((e => t.addEventListener(e, this.handleEvent)))
+                    }, this.enableDownEvent = this.options.enable, this.enableUpEvent = this.options.enable, this.events = (this.options.events || []).concat(Bm), t.tabIndex = this.options.tabIndex || 0, t.style.outline = "none", this.events.forEach((e => t.addEventListener(e, this.handleEvent)))
                 }
                 destroy() {
                     this.events.forEach((t => this.element.removeEventListener(t, this.handleEvent)))
                 }
                 enableEventType(t, e) {
-                    t === Bm && (this.enableDownEvent = e), t === Dm && (this.enableUpEvent = e)
+                    t === Dm && (this.enableDownEvent = e), t === Nm && (this.enableUpEvent = e)
                 }
             }
-            const Vm = "contextmenu";
-            class Um extends fm {
+            const Um = "contextmenu";
+            class Gm extends gm {
                 constructor(t, e, n) {
                     super(t, e, n), this.handleEvent = t => {
                         this.options.enable && this.callback({
-                            type: Vm,
+                            type: Um,
                             center: {
                                 x: t.clientX,
                                 y: t.clientY
                             },
                             srcEvent: t,
                             pointerType: "mouse",
                             target: t.target
                         })
                     }, t.addEventListener("contextmenu", this.handleEvent)
                 }
                 destroy() {
                     this.element.removeEventListener("contextmenu", this.handleEvent)
                 }
                 enableEventType(t, e) {
-                    t === Vm && (this.options.enable = e)
+                    t === Um && (this.options.enable = e)
                 }
             }
-            const Gm = {
+            const Wm = {
                 pointerdown: 1,
                 pointermove: 2,
                 pointerup: 4,
                 mousedown: 1,
                 mousemove: 2,
                 mouseup: 4
             };
 
-            function Wm(t) {
-                const e = Gm[t.srcEvent.type];
+            function Hm(t) {
+                const e = Wm[t.srcEvent.type];
                 if (!e) return null;
                 const {
                     buttons: n,
                     button: i,
                     which: r
                 } = t.srcEvent;
                 let s = !1,
@@ -17583,33 +17586,33 @@
                 return 4 === e || 2 === e && !Number.isFinite(n) ? (s = 1 === r, o = 2 === r, a = 3 === r) : 2 === e ? (s = Boolean(1 & n), o = Boolean(4 & n), a = Boolean(2 & n)) : 1 === e && (s = 0 === i, o = 1 === i, a = 2 === i), {
                     leftButton: s,
                     middleButton: o,
                     rightButton: a
                 }
             }
 
-            function Hm(t, e) {
+            function Zm(t, e) {
                 const n = t.center;
                 if (!n) return null;
                 const i = e.getBoundingClientRect(),
                     r = i.width / e.offsetWidth || 1,
                     s = i.height / e.offsetHeight || 1;
                 return {
                     center: n,
                     offsetCenter: {
                         x: (n.x - i.left - e.clientLeft) / r,
                         y: (n.y - i.top - e.clientTop) / s
                     }
                 }
             }
-            const Zm = {
+            const qm = {
                 srcElement: "root",
                 priority: 0
             };
-            class qm {
+            class Xm {
                 constructor(t) {
                     this.handleEvent = t => {
                         if (this.isEmpty()) return;
                         const e = this._normalizeEvent(t);
                         let n = t.srcEvent.target;
                         for (; n && n !== e.rootElement;) {
                             if (this._emit(e, n), e.handled) return;
@@ -17622,20 +17625,20 @@
                     return !this._active
                 }
                 add(t, e, n, i = !1, r = !1) {
                     const {
                         handlers: s,
                         handlersByElement: o
                     } = this;
-                    let a = Zm;
+                    let a = qm;
                     "string" == typeof n || n && n.addEventListener ? a = {
-                        ...Zm,
+                        ...qm,
                         srcElement: n
                     } : n && (a = {
-                        ...Zm,
+                        ...qm,
                         ...n
                     });
                     let l = o.get(a.srcElement);
                     l || (l = [], o.set(a.srcElement, l));
                     const c = {
                         type: t,
                         handler: e,
@@ -17695,45 +17698,45 @@
                         }
                     }
                 }
                 _normalizeEvent(t) {
                     const e = this.eventManager.getElement();
                     return {
                         ...t,
-                        ...Wm(t),
-                        ...Hm(t, e),
+                        ...Hm(t),
+                        ...Zm(t, e),
                         preventDefault: () => {
                             t.srcEvent.preventDefault()
                         },
                         stopImmediatePropagation: null,
                         stopPropagation: null,
                         handled: !1,
                         rootElement: e
                     }
                 }
             }
-            const Xm = {
+            const Ym = {
                 events: null,
                 recognizers: null,
                 recognizerOptions: {},
-                Manager: dm,
+                Manager: pm,
                 touchAction: "none",
                 tabIndex: 0
             };
-            class Ym {
+            class Km {
                 constructor(t = null, e) {
                     this._onBasicInput = t => {
                         const {
                             srcEvent: e
-                        } = t, n = bm[e.type];
+                        } = t, n = ym[e.type];
                         n && this.manager.emit(n, t)
                     }, this._onOtherEvent = t => {
                         this.manager.emit(t.type, t)
                     }, this.options = {
-                        ...Xm,
+                        ...Ym,
                         ...e
                     }, this.events = new Map, this.setElement(t);
                     const {
                         events: n
                     } = this.options;
                     n && this.on(n)
                 }
@@ -17743,36 +17746,36 @@
                 setElement(t) {
                     if (this.element && this.destroy(), this.element = t, !t) return;
                     const {
                         options: e
                     } = this, n = e.Manager;
                     this.manager = new n(t, {
                         touchAction: e.touchAction,
-                        recognizers: e.recognizers || gm
-                    }).on("hammer.input", this._onBasicInput), e.recognizers || Object.keys(mm).forEach((t => {
+                        recognizers: e.recognizers || mm
+                    }).on("hammer.input", this._onBasicInput), e.recognizers || Object.keys(vm).forEach((t => {
                         const e = this.manager.get(t);
-                        e && mm[t].forEach((t => {
+                        e && vm[t].forEach((t => {
                             e.recognizeWith(t)
                         }))
                     }));
                     for (const t in e.recognizerOptions) {
                         const n = this.manager.get(t);
                         if (n) {
                             const i = e.recognizerOptions[t];
                             delete i.enable, n.set(i)
                         }
                     }
-                    this.wheelInput = new Mm(t, this._onOtherEvent, {
+                    this.wheelInput = new Om(t, this._onOtherEvent, {
                         enable: !1
-                    }), this.moveInput = new Fm(t, this._onOtherEvent, {
+                    }), this.moveInput = new zm(t, this._onOtherEvent, {
                         enable: !1
-                    }), this.keyInput = new Nm(t, this._onOtherEvent, {
+                    }), this.keyInput = new Vm(t, this._onOtherEvent, {
                         enable: !1,
                         tabIndex: e.tabIndex
-                    }), this.contextmenuInput = new Um(t, this._onOtherEvent, {
+                    }), this.contextmenuInput = new Gm(t, this._onOtherEvent, {
                         enable: !1
                     });
                     for (const [t, e] of this.events) e.isEmpty() || (this._toggleRecognizer(e.recognizerName, !0), this.manager.on(t, e.handleEvent))
                 }
                 destroy() {
                     this.element && (this.wheelInput.destroy(), this.moveInput.destroy(), this.keyInput.destroy(), this.contextmenuInput.destroy(), this.manager.destroy(), this.wheelInput = null, this.moveInput = null, this.keyInput = null, this.contextmenuInput = null, this.manager = null, this.element = null)
                 }
@@ -17794,15 +17797,15 @@
                     } = this;
                     if (!n) return;
                     const i = n.get(t);
                     if (i && i.options.enable !== e) {
                         i.set({
                             enable: e
                         });
-                        const r = vm[t];
+                        const r = bm[t];
                         r && !this.options.recognizers && r.forEach((r => {
                             const s = n.get(r);
                             e ? (s.requireFailure(t), i.dropRequireFailure(r)) : s.dropRequireFailure(t)
                         }))
                     }
                     this.wheelInput.enableEventType(t, e), this.moveInput.enableEventType(t, e), this.keyInput.enableEventType(t, e), this.contextmenuInput.enableEventType(t, e)
                 }
@@ -17811,42 +17814,42 @@
                         n = e;
                         for (const e in t) this._addEventHandler(e, t[e], n, i, r);
                         return
                     }
                     const {
                         manager: s,
                         events: o
-                    } = this, a = xm[t] || t;
+                    } = this, a = wm[t] || t;
                     let l = o.get(a);
-                    l || (l = new qm(this), o.set(a, l), l.recognizerName = _m[a] || a, s && s.on(a, l.handleEvent)), l.add(t, e, n, i, r), l.isEmpty() || this._toggleRecognizer(l.recognizerName, !0)
+                    l || (l = new Xm(this), o.set(a, l), l.recognizerName = xm[a] || a, s && s.on(a, l.handleEvent)), l.add(t, e, n, i, r), l.isEmpty() || this._toggleRecognizer(l.recognizerName, !0)
                 }
                 _removeEventHandler(t, e) {
                     if ("string" != typeof t) {
                         for (const e in t) this._removeEventHandler(e, t[e]);
                         return
                     }
                     const {
                         events: n
-                    } = this, i = xm[t] || t, r = n.get(i);
+                    } = this, i = wm[t] || t, r = n.get(i);
                     if (r && (r.remove(t, e), r.isEmpty())) {
                         const {
                             recognizerName: t
                         } = r;
                         let e = !1;
                         for (const i of n.values())
                             if (i.recognizerName === t && !i.isEmpty()) {
                                 e = !0;
                                 break
                             } e || this._toggleRecognizer(t, !1)
                     }
                 }
             }
 
-            function Km() {}
-            const Qm = {
+            function Qm() {}
+            const Jm = {
                 id: "",
                 width: "100%",
                 height: "100%",
                 style: null,
                 viewState: null,
                 initialViewState: null,
                 pickingRadius: 0,
@@ -17864,36 +17867,36 @@
                 touchAction: "none",
                 eventRecognizerOptions: {},
                 _framebuffer: null,
                 _animate: !1,
                 _pickable: !0,
                 _typedArrayManagerProps: {},
                 _customRender: null,
-                onWebGLInitialized: Km,
-                onResize: Km,
-                onViewStateChange: Km,
-                onInteractionStateChange: Km,
-                onBeforeRender: Km,
-                onAfterRender: Km,
-                onLoad: Km,
+                onWebGLInitialized: Qm,
+                onResize: Qm,
+                onViewStateChange: Qm,
+                onInteractionStateChange: Qm,
+                onBeforeRender: Qm,
+                onAfterRender: Qm,
+                onLoad: Qm,
                 onError: t => na.error(t.message)(),
                 onHover: null,
                 onClick: null,
                 onDragStart: null,
                 onDrag: null,
                 onDragEnd: null,
                 _onMetrics: null,
                 getCursor: ({
                     isDragging: t
                 }) => t ? "grabbing" : "grab",
                 getTooltip: null,
                 debug: !1,
                 drawPickingColors: !1
             };
-            class Jm {
+            class $m {
                 constructor(t) {
                     wo(this, "props", void 0), wo(this, "width", 0), wo(this, "height", 0), wo(this, "userData", {}), wo(this, "canvas", null), wo(this, "viewManager", null), wo(this, "layerManager", null), wo(this, "effectManager", null), wo(this, "deckRenderer", null), wo(this, "deckPicker", null), wo(this, "eventManager", null), wo(this, "tooltip", null), wo(this, "metrics", void 0), wo(this, "animationLoop", void 0), wo(this, "stats", void 0), wo(this, "viewState", void 0), wo(this, "cursorState", void 0), wo(this, "_needsRedraw", void 0), wo(this, "_pickRequest", void 0), wo(this, "_lastPointerDownInfo", null), wo(this, "_metricsCounter", void 0), wo(this, "_onPointerMove", (t => {
                         const {
                             _pickRequest: e
                         } = this;
                         if ("pointerleave" === t.type) e.x = -1, e.y = -1, e.radius = 0;
                         else {
@@ -17930,26 +17933,26 @@
                             n = this._pick("pickObject", "pickObject Time", {
                                 x: e.x,
                                 y: e.y,
                                 radius: this.props.pickingRadius
                             });
                         this._lastPointerDownInfo = n.result[0] || n.emptyInfo
                     })), this.props = {
-                        ...Qm,
+                        ...Jm,
                         ...t
                     }, t = this.props, this._needsRedraw = "Initial render", this._pickRequest = {
                         mode: "hover",
                         x: -1,
                         y: -1,
                         radius: 0,
                         event: null
                     }, this.cursorState = {
                         isHovering: !1,
                         isDragging: !1
-                    }, t.viewState && t.initialViewState && na.warn("View state tracking is disabled. Use either `initialViewState` for auto update or `viewState` for manual update.")(), "IE" === sm() && na.warn("IE 11 is not supported")(), this.viewState = t.initialViewState, t.gl || "undefined" != typeof document && (this.canvas = this._createCanvas(t)), this.animationLoop = this._createAnimationLoop(t), this.stats = new da({
+                    }, t.viewState && t.initialViewState && na.warn("View state tracking is disabled. Use either `initialViewState` for auto update or `viewState` for manual update.")(), "IE" === om() && na.warn("IE 11 is not supported")(), this.viewState = t.initialViewState, t.gl || "undefined" != typeof document && (this.canvas = this._createCanvas(t)), this.animationLoop = this._createAnimationLoop(t), this.stats = new da({
                         id: "deck.gl"
                     }), this.metrics = {
                         fps: 0,
                         setPropsTime: 0,
                         updateAttributesTime: 0,
                         framesRedrawn: 0,
                         pickTime: 0,
@@ -17965,15 +17968,15 @@
                     }, this._metricsCounter = 0, this.setProps(t), t._typedArrayManagerProps && sc.setOptions(t._typedArrayManagerProps), this.animationLoop.start()
                 }
                 finalize() {
                     var t, e, n, i, r, s, o, a, l;
                     null === (t = this.animationLoop) || void 0 === t || t.stop(), this.animationLoop = null, this._lastPointerDownInfo = null, null === (e = this.layerManager) || void 0 === e || e.finalize(), this.layerManager = null, null === (n = this.viewManager) || void 0 === n || n.finalize(), this.viewManager = null, null === (i = this.effectManager) || void 0 === i || i.finalize(), this.effectManager = null, null === (r = this.deckRenderer) || void 0 === r || r.finalize(), this.deckRenderer = null, null === (s = this.deckPicker) || void 0 === s || s.finalize(), this.deckPicker = null, null === (o = this.eventManager) || void 0 === o || o.destroy(), this.eventManager = null, null === (a = this.tooltip) || void 0 === a || a.remove(), this.tooltip = null, this.props.canvas || this.props.gl || !this.canvas || (null === (l = this.canvas.parentElement) || void 0 === l || l.removeChild(this.canvas), this.canvas = null)
                 }
                 setProps(t) {
-                    this.stats.get("setProps Time").timeStart(), "onLayerHover" in t && na.removed("onLayerHover", "onHover")(), "onLayerClick" in t && na.removed("onLayerClick", "onClick")(), t.initialViewState && !Sf(this.props.initialViewState, t.initialViewState, 3) && (this.viewState = t.initialViewState), Object.assign(this.props, t), this._setCanvasSize(this.props);
+                    this.stats.get("setProps Time").timeStart(), "onLayerHover" in t && na.removed("onLayerHover", "onHover")(), "onLayerClick" in t && na.removed("onLayerClick", "onClick")(), t.initialViewState && !Cf(this.props.initialViewState, t.initialViewState, 3) && (this.viewState = t.initialViewState), Object.assign(this.props, t), this._setCanvasSize(this.props);
                     const e = Object.create(this.props);
                     Object.assign(e, {
                         views: this._getViews(),
                         width: this.width,
                         height: this.height,
                         viewState: this._getViewState()
                     }), this.animationLoop.setProps(e), this.layerManager && (this.viewManager.setProps(e), this.layerManager.activateViewport(this.getViewports()[0]), this.layerManager.setProps(e), this.effectManager.setProps(e), this.deckRenderer.setProps(e), this.deckPicker.setProps(e)), this.stats.get("setProps Time").timeEnd()
@@ -17998,18 +18001,18 @@
                     });
                     e = t || e, e && (this.stats.get("Redraw Count").incrementCount(), this.props._customRender ? this.props._customRender(e) : this._drawLayers(e))
                 }
                 get isInitialized() {
                     return null !== this.viewManager
                 }
                 getViews() {
-                    return Of(this.viewManager), this.viewManager.views
+                    return Lf(this.viewManager), this.viewManager.views
                 }
                 getViewports(t) {
-                    return Of(this.viewManager), this.viewManager.getViewports(t)
+                    return Lf(this.viewManager), this.viewManager.getViewports(t)
                 }
                 pickObject(t) {
                     const e = this._pick("pickObject", "pickObject Time", t).result;
                     return e.length ? e[0] : null
                 }
                 pickMultipleObjects(t) {
                     return t.depth = t.depth || 10, this._pick("pickObject", "pickMultipleObjects Time", t).result
@@ -18027,15 +18030,15 @@
                 _removeResources(t) {
                     for (const e of t) this.layerManager.resourceManager.remove(e)
                 }
                 _addDefaultEffect(t) {
                     this.effectManager.addDefaultEffect(t)
                 }
                 _pick(t, e, n) {
-                    Of(this.deckPicker);
+                    Lf(this.deckPicker);
                     const {
                         stats: i
                     } = this;
                     i.get("Pick Count").incrementCount(), i.get(e).timeStart();
                     const r = this.deckPicker[t]({
                         layers: this.layerManager.getLayers(n),
                         views: this.viewManager.getViews(),
@@ -18044,15 +18047,15 @@
                         effects: this.effectManager.getEffects(),
                         ...n
                     });
                     return i.get(e).timeEnd(), r
                 }
                 _createCanvas(t) {
                     let e = t.canvas;
-                    return "string" == typeof e && (e = document.getElementById(e), Of(e)), e || (e = document.createElement("canvas"), e.id = t.id || "deckgl-overlay", (t.parent || document.body).appendChild(e)), Object.assign(e.style, t.style), e
+                    return "string" == typeof e && (e = document.getElementById(e), Lf(e)), e || (e = document.createElement("canvas"), e.id = t.id || "deckgl-overlay", (t.parent || document.body).appendChild(e)), Object.assign(e.style, t.style), e
                 }
                 _setCanvasSize(t) {
                     if (!this.canvas) return;
                     const {
                         width: e,
                         height: n
                     } = t;
@@ -18091,15 +18094,15 @@
                         glOptions: r,
                         debug: s,
                         onError: o,
                         onBeforeRender: a,
                         onAfterRender: l,
                         useDevicePixels: c
                     } = t;
-                    return new cm({
+                    return new hm({
                         width: e,
                         height: n,
                         useDevicePixels: c,
                         autoResizeDrawingBuffer: !i,
                         autoResizeViewport: !1,
                         gl: i,
                         onCreateContext: t => yd({
@@ -18116,15 +18119,15 @@
                         onError: o
                     })
                 }
                 _getViewState() {
                     return this.props.viewState || this.viewState
                 }
                 _getViews() {
-                    let t = this.props.views || [new tg({
+                    let t = this.props.views || [new eg({
                         id: "default-view"
                     })];
                     return t = Array.isArray(t) ? t : [t], t.length && this.props.controller && (t[0].props.controller = this.props.controller), t
                 }
                 _onContextLost() {
                     const {
                         onError: t
@@ -18159,49 +18162,49 @@
                     t && (t.style.cursor = this.props.getCursor(this.cursorState))
                 }
                 _setGLContext(t) {
                     if (this.layerManager) return;
                     this.canvas || (this.canvas = t.canvas, _d(t, {
                         enable: !0,
                         copyState: !0
-                    })), this.tooltip = new zg(this.canvas), hd(t, {
+                    })), this.tooltip = new Bg(this.canvas), hd(t, {
                         blend: !0,
                         blendFunc: [770, 771, 1, 771],
                         polygonOffsetFill: !0,
                         depthTest: !0,
                         depthFunc: 515
                     }), this.props.onWebGLInitialized(t);
                     const e = new So;
-                    e.play(), this.animationLoop.attachTimeline(e), this.eventManager = new Ym(this.props.parent || t.canvas, {
+                    e.play(), this.animationLoop.attachTimeline(e), this.eventManager = new Km(this.props.parent || t.canvas, {
                         touchAction: this.props.touchAction,
                         recognizerOptions: this.props.eventRecognizerOptions,
                         events: {
                             pointerdown: this._onPointerDown,
                             pointermove: this._onPointerMove,
                             pointerleave: this._onPointerMove
                         }
                     });
                     for (const t in kh) this.eventManager.on(t, this._onEvent);
-                    this.viewManager = new Cf({
+                    this.viewManager = new Tf({
                         timeline: e,
                         eventManager: this.eventManager,
                         onViewStateChange: this._onViewStateChange.bind(this),
                         onInteractionStateChange: this._onInteractionStateChange.bind(this),
                         views: this._getViews(),
                         viewState: this._getViewState(),
                         width: this.width,
                         height: this.height
                     });
                     const n = this.viewManager.getViewports()[0];
-                    this.layerManager = new Pf(t, {
+                    this.layerManager = new Sf(t, {
                         deck: this,
                         stats: this.stats,
                         viewport: n,
                         timeline: e
-                    }), this.effectManager = new Pg, this.deckRenderer = new Mg(t), this.deckPicker = new jg(t), this.setProps(this.props), this._updateCanvasSize(), this.props.onLoad()
+                    }), this.effectManager = new Sg, this.deckRenderer = new Og(t), this.deckPicker = new Fg(t), this.setProps(this.props), this._updateCanvasSize(), this.props.onLoad()
                 }
                 _drawLayers(t, e) {
                     const {
                         gl: n
                     } = this.layerManager.context;
                     hd(n, this.props.parameters), this.props.onBeforeRender({
                         gl: n
@@ -18243,29 +18246,29 @@
                 }
                 _getMetrics() {
                     const {
                         metrics: t,
                         stats: e
                     } = this;
                     t.fps = e.get("frameRate").getHz(), t.setPropsTime = e.get("setProps Time").time, t.updateAttributesTime = e.get("Update Attributes").time, t.framesRedrawn = e.get("Redraw Count").count, t.pickTime = e.get("pickObject Time").time + e.get("pickMultipleObjects Time").time + e.get("pickObjects Time").time, t.pickCount = e.get("Pick Count").count, t.gpuTime = e.get("GPU Time").time, t.cpuTime = e.get("CPU Time").time, t.gpuTimePerFrame = e.get("GPU Time").getAverageTime(), t.cpuTimePerFrame = e.get("CPU Time").getAverageTime();
-                    const n = wd.get("Memory Usage");
+                    const n = Ed.get("Memory Usage");
                     t.bufferMemory = n.get("Buffer Memory").count, t.textureMemory = n.get("Texture Memory").count, t.renderbufferMemory = n.get("Renderbuffer Memory").count, t.gpuMemory = n.get("GPU Memory").count
                 }
             }
-            wo(Jm, "defaultProps", Qm), wo(Jm, "VERSION", im);
-            const $m = "undefined" != typeof window ? c.useLayoutEffect : c.useEffect;
+            wo($m, "defaultProps", Jm), wo($m, "VERSION", rm);
+            const tv = "undefined" != typeof window ? c.useLayoutEffect : c.useEffect;
 
-            function tv(t, e) {
+            function ev(t, e) {
                 for (; t;) {
                     if (t === e) return !0;
                     t = Object.getPrototypeOf(t)
                 }
                 return !1
             }
-            class ev {
+            class nv {
                 constructor(t, e) {
                     wo(this, "opts", void 0), wo(this, "source", void 0), this.opts = e, this.source = t
                 }
                 get value() {
                     return this.source.value
                 }
                 getValue() {
@@ -18289,39 +18292,39 @@
                     return {
                         ...this.source.getAccessor(),
                         ...this.opts
                     }
                 }
             }
 
-            function nv(t) {
+            function iv(t) {
                 return t.stride || t.size * t.bytesPerElement
             }
 
-            function iv(t, e) {
+            function rv(t, e) {
                 e.offset && na.removed("shaderAttribute.offset", "vertexOffset, elementOffset")();
-                const n = nv(t),
+                const n = iv(t),
                     i = (void 0 !== e.vertexOffset ? e.vertexOffset : t.vertexOffset || 0) * n + (e.elementOffset || 0) * t.bytesPerElement + (t.offset || 0);
                 return {
                     ...e,
                     offset: i,
                     stride: n
                 }
             }
-            class rv {
+            class sv {
                 constructor(t, e, n) {
                     wo(this, "gl", void 0), wo(this, "id", void 0), wo(this, "size", void 0), wo(this, "settings", void 0), wo(this, "value", void 0), wo(this, "doublePrecision", void 0), wo(this, "_buffer", void 0), wo(this, "state", void 0), this.gl = t, this.id = e.id || "", this.size = e.size || 1;
                     const i = e.logicalType || e.type,
                         r = 5130 === i;
                     let s, {
                         defaultValue: o
                     } = e;
                     o = Number.isFinite(o) ? [o] : o || new Array(this.size).fill(0), s = r ? 5126 : !i && e.isIndexed ? t && function(t, e) {
-                        return gp(t, e)
-                    }(t, dp) ? 5125 : 5123 : i || 5126;
+                        return mp(t, e)
+                    }(t, pp) ? 5125 : 5123 : i || 5126;
                     let a = function(t) {
                         switch (t) {
                             case 5126:
                                 return Float32Array;
                             case 5130:
                                 return Float64Array;
                             case 5123:
@@ -18366,27 +18369,27 @@
                 }
                 get buffer() {
                     if (!this._buffer) {
                         const {
                             isIndexed: t,
                             type: e
                         } = this.settings;
-                        this._buffer = new Wd(this.gl, {
+                        this._buffer = new Hd(this.gl, {
                             id: this.id,
                             target: t ? 34963 : 34962,
                             accessor: {
                                 type: e
                             }
                         })
                     }
                     return this._buffer
                 }
                 get byteOffset() {
                     const t = this.getAccessor();
-                    return t.vertexOffset ? t.vertexOffset * nv(t) : 0
+                    return t.vertexOffset ? t.vertexOffset * iv(t) : 0
                 }
                 get numInstances() {
                     return this.state.numInstances
                 }
                 set numInstances(t) {
                     this.state.numInstances = t
                 }
@@ -18394,29 +18397,29 @@
                     this._buffer && (this._buffer.delete(), this._buffer = null), sc.release(this.state.allocatedValue)
                 }
                 getShaderAttributes(t, e) {
                     if (this.doublePrecision) {
                         const n = {},
                             i = this.value instanceof Float64Array,
                             r = function(t, e) {
-                                const n = iv(t, e);
+                                const n = rv(t, e);
                                 return {
                                     high: n,
                                     low: {
                                         ...n,
                                         offset: n.offset + 4 * t.size
                                     }
                                 }
                             }(this.getAccessor(), e || {});
-                        return n[t] = new ev(this, r.high), n["".concat(t, "64Low")] = i ? new ev(this, r.low) : new Float32Array(this.size), n
+                        return n[t] = new nv(this, r.high), n["".concat(t, "64Low")] = i ? new nv(this, r.low) : new Float32Array(this.size), n
                     }
                     if (e) {
-                        const n = iv(this.getAccessor(), e);
+                        const n = rv(this.getAccessor(), e);
                         return {
-                            [t]: new ev(this, n)
+                            [t]: new nv(this, n)
                         }
                     }
                     return {
                         [t]: this
                     }
                 }
                 getBuffer() {
@@ -18456,34 +18459,34 @@
                 setData(t) {
                     const {
                         state: e
                     } = this;
                     let n;
                     n = ArrayBuffer.isView(t) ? {
                         value: t
-                    } : t instanceof Wd ? {
+                    } : t instanceof Hd ? {
                         buffer: t
                     } : t;
                     const i = {
                         ...this.settings,
                         ...n
                     };
                     if (e.bufferAccessor = i, e.bounds = null, n.constant) {
                         let t = n.value;
                         if (t = this._normalizeValue(t, [], 0), this.settings.normalized && (t = this.normalizeConstant(t)), e.constant && this._areValuesEqual(t, this.value)) return !1;
                         e.externalBuffer = null, e.constant = !0, this.value = t
                     } else if (n.buffer) {
                         const t = n.buffer;
                         e.externalBuffer = t, e.constant = !1, this.value = n.value || null;
                         const r = n.value instanceof Float64Array;
-                        i.type = n.type || t.accessor.type, i.bytesPerElement = t.accessor.BYTES_PER_ELEMENT * (r ? 2 : 1), i.stride = nv(i)
+                        i.type = n.type || t.accessor.type, i.bytesPerElement = t.accessor.BYTES_PER_ELEMENT * (r ? 2 : 1), i.stride = iv(i)
                     } else if (n.value) {
                         this._checkExternalBuffer(n);
                         let t = n.value;
-                        e.externalBuffer = null, e.constant = !1, this.value = t, i.bytesPerElement = t.BYTES_PER_ELEMENT, i.stride = nv(i);
+                        e.externalBuffer = null, e.constant = !1, this.value = t, i.bytesPerElement = t.BYTES_PER_ELEMENT, i.stride = iv(i);
                         const {
                             buffer: r,
                             byteOffset: s
                         } = this;
                         this.doublePrecision && t instanceof Float64Array && (t = zc(t, i));
                         const o = t.byteLength + s + 2 * i.stride;
                         r.byteLength < o && r.reallocate(o), r.setAccessor(null), r.subData({
@@ -18584,35 +18587,35 @@
                         size: n
                     } = this;
                     for (let i = 0; i < n; i++)
                         if (t[i] !== e[i]) return !1;
                     return !0
                 }
             }
-            const sv = [],
-                ov = [];
+            const ov = [],
+                av = [];
 
-            function av(t, e = 0, n = 1 / 0) {
-                let i = sv;
+            function lv(t, e = 0, n = 1 / 0) {
+                let i = ov;
                 const r = {
                     index: -1,
                     data: t,
                     target: []
                 };
-                return t ? "function" == typeof t[Symbol.iterator] ? i = t : t.length > 0 && (ov.length = t.length, i = ov) : i = sv, (e > 0 || Number.isFinite(n)) && (i = (Array.isArray(i) ? i : Array.from(i)).slice(e, n), r.index = e - 1), {
+                return t ? "function" == typeof t[Symbol.iterator] ? i = t : t.length > 0 && (av.length = t.length, i = av) : i = ov, (e > 0 || Number.isFinite(n)) && (i = (Array.isArray(i) ? i : Array.from(i)).slice(e, n), r.index = e - 1), {
                     iterable: i,
                     objectInfo: r
                 }
             }
 
-            function lv(t) {
+            function cv(t) {
                 return t && t[Symbol.asyncIterator]
             }
 
-            function cv(t, e) {
+            function hv(t, e) {
                 const {
                     size: n,
                     stride: i,
                     offset: r,
                     startIndices: s,
                     nested: o
                 } = e, a = t.BYTES_PER_ELEMENT, l = i ? i / a : n, c = r ? r / a : 0, h = Math.floor((t.length - c) / l);
@@ -18644,20 +18647,20 @@
                             const r = i * l + c;
                             for (let i = 0; i < n; i++) d[e++] = t[r + i]
                         }
                     }
                     return d
                 }
             }
-            const hv = [],
-                uv = [
+            const uv = [],
+                dv = [
                     [0, 1 / 0]
                 ];
 
-            function dv(t) {
+            function pv(t) {
                 const {
                     source: e,
                     target: n,
                     start: i = 0,
                     size: r,
                     getData: s
                 } = t, o = t.end || n.length, a = e.length, l = o - i;
@@ -18665,92 +18668,92 @@
                 if (n.set(e, i), !s) return;
                 let c = a;
                 for (; c < l;) {
                     const t = s(c, e);
                     for (let e = 0; e < r; e++) n[i + c] = t[e] || 0, c++
                 }
             }
-            const pv = {
+            const fv = {
                 interpolation: {
                     duration: 0,
                     easing: t => t
                 },
                 spring: {
                     stiffness: .05,
                     damping: .5
                 }
             };
 
-            function fv(t, e) {
+            function gv(t, e) {
                 if (!t) return null;
                 Number.isFinite(t) && (t = {
                     type: "interpolation",
                     duration: t
                 });
                 const n = t.type || "interpolation";
                 return {
-                    ...pv[n],
+                    ...fv[n],
                     ...e,
                     ...t,
                     type: n
                 }
             }
 
-            function gv(t, e) {
+            function mv(t, e) {
                 const n = e.getBuffer();
                 return n ? [n, {
                     divisor: 0,
                     size: e.size,
                     normalized: e.settings.normalized
                 }] : e.value
             }
 
-            function mv(t) {
+            function vv(t) {
                 switch (t) {
                     case 1:
                         return "float";
                     case 2:
                         return "vec2";
                     case 3:
                         return "vec3";
                     case 4:
                         return "vec4";
                     default:
                         throw new Error('No defined attribute type for size "'.concat(t, '"'))
                 }
             }
 
-            function vv(t) {
+            function bv(t) {
                 t.push(t.shift())
             }
 
-            function bv(t, e) {
+            function yv(t, e) {
                 const {
                     doublePrecision: n,
                     settings: i,
                     value: r,
                     size: s
                 } = t, o = n && r instanceof Float64Array ? 2 : 1;
                 return (i.noAlloc ? r.length : e * s) * o
             }
 
-            function yv({
+            function _v({
                 buffer: t,
                 numInstances: e,
                 attribute: n,
                 fromLength: i,
                 fromStartIndices: r,
                 getData: s = (t => t)
             }) {
                 const o = n.doublePrecision && n.value instanceof Float64Array ? 2 : 1,
                     a = n.size * o,
                     l = n.byteOffset,
                     c = n.startIndices,
                     h = r && c,
-                    u = bv(n, e),
+                    u = yv(n, e),
                     d = n.isConstant;
                 if (!h && i >= u) return;
                 const p = d ? n.value : n.getBuffer().getData({
                     srcByteOffset: l
                 });
                 if (n.settings.normalized && !d) {
                     const t = s;
@@ -18765,37 +18768,37 @@
                     source: t,
                     target: e,
                     size: n,
                     getData: i,
                     sourceStartIndices: r,
                     targetStartIndices: s
                 }) {
-                    if (!Array.isArray(s)) return dv({
+                    if (!Array.isArray(s)) return pv({
                         source: t,
                         target: e,
                         size: n,
                         getData: i
                     }), e;
                     let o = 0,
                         a = 0;
                     const l = i && ((t, e) => i(t + a, e)),
                         c = Math.min(r.length, s.length);
                     for (let i = 1; i < c; i++) {
                         const c = r[i] * n,
                             h = s[i] * n;
-                        dv({
+                        pv({
                             source: t.subarray(o, c),
                             target: e,
                             start: a,
                             end: h,
                             size: n,
                             getData: l
                         }), o = c, a = h
                     }
-                    a < e.length && dv({
+                    a < e.length && pv({
                         source: [],
                         target: e,
                         start: a,
                         size: n,
                         getData: l
                     })
                 }({
@@ -18806,24 +18809,24 @@
                     size: a,
                     getData: f
                 }), t.byteLength < m.byteLength + l && t.reallocate(m.byteLength + l), t.subData({
                     data: m,
                     offset: l
                 })
             }
-            class _v extends rv {
+            class xv extends sv {
                 constructor(t, e) {
                     super(t, e, {
                         startIndices: null,
                         lastExternalBuffer: null,
                         binaryValue: null,
                         binaryAccessor: null,
                         needsUpdate: !0,
                         needsRedraw: !1,
-                        updateRanges: uv
+                        updateRanges: dv
                     }), wo(this, "constant", !1), this.settings.update = e.update || (e.accessor ? this._autoUpdater : void 0), Object.seal(this.settings), Object.seal(this.state), this._validateAttributeUpdaters()
                 }
                 get startIndices() {
                     return this.state.startIndices
                 }
                 set startIndices(t) {
                     this.state.startIndices = t
@@ -18847,48 +18850,48 @@
                     return Boolean(this.settings.transition)
                 }
                 getTransitionSetting(t) {
                     if (!t || !this.supportsTransition()) return null;
                     const {
                         accessor: e
                     } = this.settings, n = this.settings.transition;
-                    return fv(Array.isArray(e) ? t[e.find((e => t[e]))] : t[e], n)
+                    return gv(Array.isArray(e) ? t[e.find((e => t[e]))] : t[e], n)
                 }
                 setNeedsUpdate(t = this.id, e) {
                     if (this.state.needsUpdate = this.state.needsUpdate || t, this.setNeedsRedraw(t), e) {
                         const {
                             startRow: t = 0,
                             endRow: n = 1 / 0
                         } = e;
                         this.state.updateRanges = function(t, e) {
-                            if (t === uv) return t;
+                            if (t === dv) return t;
                             if (e[0] < 0 && (e[0] = 0), e[0] >= e[1]) return t;
                             const n = [],
                                 i = t.length;
                             let r = 0;
                             for (let s = 0; s < i; s++) {
                                 const i = t[s];
                                 i[1] < e[0] ? (n.push(i), r = s + 1) : i[0] > e[1] ? n.push(i) : e = [Math.min(i[0], e[0]), Math.max(i[1], e[1])]
                             }
                             return n.splice(r, 0, e), n
                         }(this.state.updateRanges, [t, n])
-                    } else this.state.updateRanges = uv
+                    } else this.state.updateRanges = dv
                 }
                 clearNeedsUpdate() {
-                    this.state.needsUpdate = !1, this.state.updateRanges = hv
+                    this.state.needsUpdate = !1, this.state.updateRanges = uv
                 }
                 setNeedsRedraw(t = this.id) {
                     this.state.needsRedraw = this.state.needsRedraw || t
                 }
                 allocate(t) {
                     const {
                         state: e,
                         settings: n
                     } = this;
-                    return !n.noAlloc && !!n.update && (super.allocate(t, e.updateRanges !== uv), !0)
+                    return !n.noAlloc && !!n.update && (super.allocate(t, e.updateRanges !== dv), !0)
                 }
                 updateBuffer({
                     numInstances: t,
                     data: e,
                     props: n,
                     context: i
                 }) {
@@ -18950,17 +18953,17 @@
                     if (i.noAlloc) return !1;
                     if (n.binaryValue === t) return this.clearNeedsUpdate(), !0;
                     if (n.binaryValue = t, this.setNeedsRedraw(), i.transform || e !== this.startIndices) {
                         ArrayBuffer.isView(t) && (t = {
                             value: t
                         });
                         const r = t;
-                        Of(ArrayBuffer.isView(r.value), "invalid ".concat(i.accessor));
+                        Lf(ArrayBuffer.isView(r.value), "invalid ".concat(i.accessor));
                         const s = Boolean(r.size) && r.size !== this.size;
-                        return n.binaryAccessor = cv(r.value, {
+                        return n.binaryAccessor = hv(r.value, {
                             size: r.size || this.size,
                             stride: r.stride,
                             offset: r.offset,
                             startIndices: e,
                             nested: s
                         }), !1
                     }
@@ -18994,20 +18997,20 @@
                         value: l,
                         size: c,
                         startIndices: h
                     } = t, {
                         accessor: u,
                         transform: d
                     } = o, p = a.binaryAccessor || ("function" == typeof u ? u : r[u]);
-                    Of("function" == typeof p, 'accessor "'.concat(u, '" is not a function'));
+                    Lf("function" == typeof p, 'accessor "'.concat(u, '" is not a function'));
                     let f = t.getVertexOffset(n);
                     const {
                         iterable: g,
                         objectInfo: m
-                    } = av(e, n, i);
+                    } = lv(e, n, i);
                     for (const e of g) {
                         m.index++;
                         let n = p(e, m);
                         if (d && (n = d.call(this, n)), h) {
                             const e = (m.index < h.length - 1 ? h[m.index + 1] : s) - h[m.index];
                             if (n && Array.isArray(n[0])) {
                                 let e = f;
@@ -19047,37 +19050,37 @@
                             default:
                                 n = !1
                         }
                         if (!n) throw new Error("Illegal attribute generated for ".concat(this.id))
                     }
                 }
             }
-            const xv = "out vec4 transform_output;\nvoid main() {\n  transform_output = vec4(0);\n}",
-                wv = "#version 300 es\n".concat(xv);
+            const wv = "out vec4 transform_output;\nvoid main() {\n  transform_output = vec4(0);\n}",
+                Ev = "#version 300 es\n".concat(wv);
 
-            function Ev(t, e) {
+            function Pv(t, e) {
                 e = Array.isArray(e) ? e : [e];
                 const n = t.replace(/^\s+/, "").split(/\s+/),
                     [i, r, s] = n;
                 return e.includes(i) && r && s ? {
                     qualifier: i,
                     type: r,
                     name: s.split(";")[0]
                 } : null
             }
 
-            function Pv() {
+            function Sv() {
                 let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                 const {
                     version: e = 100,
                     input: n,
                     inputType: i,
                     output: r
                 } = t;
-                if (!n) return 300 === e ? wv : e > 300 ? "#version ".concat(e, "\n").concat(xv) : "void main() {gl_FragColor = vec4(0);}";
+                if (!n) return 300 === e ? Ev : e > 300 ? "#version ".concat(e, "\n").concat(wv) : "void main() {gl_FragColor = vec4(0);}";
                 const s = function(t, e) {
                     switch (e) {
                         case "float":
                             return "vec4(".concat(t, ", 0.0, 0.0, 1.0)");
                         case "vec2":
                             return "vec4(".concat(t, ", 0.0, 1.0)");
                         case "vec3":
@@ -19086,28 +19089,28 @@
                             return t;
                         default:
                             return Uh(!1), null
                     }
                 }(n, i);
                 return e >= 300 ? "#version ".concat(e, " ").concat(300 === e ? "es" : "", "\nin ").concat(i, " ").concat(n, ";\nout vec4 ").concat(r, ";\nvoid main() {\n  ").concat(r, " = ").concat(s, ";\n}") : "varying ".concat(i, " ").concat(n, ";\nvoid main() {\n  gl_FragColor = ").concat(s, ";\n}")
             }
-            class Sv extends Rd {
+            class Cv extends Id {
                 get[Symbol.toStringTag]() {
                     return "TransformFeedback"
                 }
                 static isSupported(t) {
                     return Lu(t)
                 }
                 constructor(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                     Iu(t), super(t, e), this.initialize(e), this.stubRemovedMethods("TransformFeedback", "v6.0", ["pause", "resume"]), Object.seal(this)
                 }
                 initialize() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
-                    return this.buffers = {}, this.unused = {}, this.configuration = null, this.bindOnUse = !0, Md(this.buffers) || this.bind((() => this._unbindBuffers())), this.setProps(t), this
+                    return this.buffers = {}, this.unused = {}, this.configuration = null, this.bindOnUse = !0, Od(this.buffers) || this.bind((() => this._unbindBuffers())), this.setProps(t), this
                 }
                 setProps(t) {
                     "program" in t && (this.configuration = t.program && t.program.configuration), "configuration" in t && (this.configuration = t.configuration), "bindOnUse" in t && (t = t.bindOnUse), "buffers" in t && this.setBuffers(t.buffers)
                 }
                 setBuffers() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     return this.bind((() => {
@@ -19128,15 +19131,15 @@
                     return this.gl.bindTransformFeedback(36386, this.handle), this._bindBuffers(), this.gl.beginTransformFeedback(t), this
                 }
                 end() {
                     return this.gl.endTransformFeedback(), this._unbindBuffers(), this.gl.bindTransformFeedback(36386, null), this
                 }
                 _getBufferParams(t) {
                     let e, n, i;
-                    return t instanceof Wd == 0 ? (i = t.buffer, n = t.byteSize, e = t.byteOffset) : i = t, void 0 === e && void 0 === n || (e = e || 0, n = n || i.byteLength - e), {
+                    return t instanceof Hd == 0 ? (i = t.buffer, n = t.byteSize, e = t.byteOffset) : i = t, void 0 === e && void 0 === n || (e = e || 0, n = n || i.byteLength - e), {
                         buffer: i,
                         byteOffset: e,
                         byteSize: n
                     }
                 }
                 _getVaryingInfo(t) {
                     return this.configuration && this.configuration.getVaryingInfo(t)
@@ -19173,15 +19176,15 @@
                 _deleteHandle() {
                     this.gl.deleteTransformFeedback(this.handle)
                 }
                 _bindHandle(t) {
                     this.gl.bindTransformFeedback(36386, this.handle)
                 }
             }
-            class Cv {
+            class Tv {
                 constructor(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                     this.gl = t, this.currentIndex = 0, this.feedbackMap = {}, this.varyings = null, this.bindings = [], this.resources = {}, this._initialize(e), Object.seal(this)
                 }
                 setupResources(t) {
                     for (const e of this.bindings) this._setupTransformFeedback(e, t)
                 }
@@ -19213,29 +19216,29 @@
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     this._setupBuffers(t)
                 }
                 getBuffer(t) {
                     const {
                         feedbackBuffers: e
                     } = this.bindings[this.currentIndex], n = t ? e[t] : null;
-                    return n ? n instanceof Wd ? n : n.buffer : null
+                    return n ? n instanceof Hd ? n : n.buffer : null
                 }
                 getData() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     const {
                         varyingName: e
                     } = t, n = this.getBuffer(e);
                     return n ? n.getData() : null
                 }
                 delete() {
                     for (const t in this.resources) this.resources[t].delete()
                 }
                 _initialize() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
-                    this._setupBuffers(t), this.varyings = t.varyings || Object.keys(this.bindings[this.currentIndex].feedbackBuffers), this.varyings.length > 0 && Ed(Lu(this.gl))
+                    this._setupBuffers(t), this.varyings = t.varyings || Object.keys(this.bindings[this.currentIndex].feedbackBuffers), this.varyings.length > 0 && Pd(Lu(this.gl))
                 }
                 _getFeedbackBuffers(t) {
                     const {
                         sourceBuffers: e = {}
                     } = t, n = {};
                     if (this.bindings[this.currentIndex] && Object.assign(n, this.bindings[this.currentIndex].feedbackBuffers), this.feedbackMap)
                         for (const t in this.feedbackMap) {
@@ -19276,15 +19279,15 @@
                 _setupTransformFeedback(t, e) {
                     let {
                         model: n
                     } = e;
                     const {
                         program: i
                     } = n;
-                    t.transformFeedback = new Sv(this.gl, {
+                    t.transformFeedback = new Cv(this.gl, {
                         program: i,
                         buffers: t.feedbackBuffers
                     })
                 }
                 _updateBindings(t) {
                     if (this.bindings[this.currentIndex] = this._updateBinding(this.bindings[this.currentIndex], t), this.feedbackMap) {
                         const {
@@ -19305,53 +19308,53 @@
                 }
                 _swapBuffers(t) {
                     if (!this.feedbackMap) return null;
                     const e = Object.assign({}, t.sourceBuffers),
                         n = Object.assign({}, t.feedbackBuffers);
                     for (const i in this.feedbackMap) {
                         const r = this.feedbackMap[i];
-                        e[i] = t.feedbackBuffers[r], n[r] = t.sourceBuffers[i], Ed(n[r] instanceof Wd)
+                        e[i] = t.feedbackBuffers[r], n[r] = t.sourceBuffers[i], Pd(n[r] instanceof Hd)
                     }
                     return {
                         sourceBuffers: e,
                         feedbackBuffers: n
                     }
                 }
                 _createNewBuffer(t, e) {
-                    const n = new Wd(this.gl, e);
+                    const n = new Hd(this.gl, e);
                     return this.resources[t] && this.resources[t].delete(), this.resources[t] = n, n
                 }
                 _getNextIndex() {
                     return (this.currentIndex + 1) % 2
                 }
             }
 
-            function Tv(t) {
+            function Av(t) {
                 let e = 100;
                 const n = t.match(/[^\s]+/g);
                 if (n.length >= 2 && "#version" === n[0]) {
                     const t = parseInt(n[1], 10);
                     Number.isFinite(t) && (e = t)
                 }
                 return e
             }
-            const Av = {
+            const Mv = {
                     name: "transform",
                     vs: "attribute float transform_elementID;\nvec2 transform_getPixelSizeHalf(vec2 size) {\n  return vec2(1.) / (2. * size);\n}\n\nvec2 transform_getPixelIndices(vec2 texSize, vec2 pixelSizeHalf) {\n  float yIndex = floor((transform_elementID / texSize[0]) + pixelSizeHalf[1]);\n  float xIndex = transform_elementID - (yIndex * texSize[0]);\n  return vec2(xIndex, yIndex);\n}\nvec2 transform_getTexCoord(vec2 size) {\n  vec2 pixelSizeHalf = transform_getPixelSizeHalf(size);\n  vec2 indices = transform_getPixelIndices(size, pixelSizeHalf);\n  vec2 coord = indices / size + pixelSizeHalf;\n  return coord;\n}\nvec2 transform_getPos(vec2 size) {\n  vec2 texCoord = transform_getTexCoord(size);\n  vec2 pos = (texCoord * (2.0, 2.0)) - (1., 1.);\n  return pos;\n}\nvec4 transform_getInput(sampler2D texSampler, vec2 size) {\n  vec2 texCoord = transform_getTexCoord(size);\n  vec4 textureColor = texture2D(texSampler, texCoord);\n  return textureColor;\n}\n",
                     fs: null
                 },
-                Mv = "transform_uSize_",
-                Ov = "transform_position";
-            const Lv = {
+                Ov = "transform_uSize_",
+                Lv = "transform_position";
+            const Rv = {
                 10241: 9728,
                 10240: 9728,
                 10242: 33071,
                 10243: 33071
             };
-            class Rv {
+            class Iv {
                 constructor(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                     this.gl = t, this.id = this.currentIndex = 0, this._swapTexture = null, this.targetTextureVarying = null, this.targetTextureType = null, this.samplerTextureMap = null, this.bindings = [], this.resources = {}, this._initialize(e), Object.seal(this)
                 }
                 updateModelProps() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     const e = this._processVertexShader(t);
@@ -19380,19 +19383,19 @@
                                 targetTexture: i
                             } = t;
                             const r = {};
                             let s, o;
                             n && (({
                                 width: s,
                                 height: o
-                            } = i), r["".concat(Mv).concat(n)] = [s, o]);
+                            } = i), r["".concat(Ov).concat(n)] = [s, o]);
                             for (const t in e)({
                                 width: s,
                                 height: o
-                            } = e[t]), r["".concat(Mv).concat(t)] = [s, o];
+                            } = e[t]), r["".concat(Ov).concat(t)] = [s, o];
                             return r
                         }({
                             sourceTextureMap: n,
                             targetTextureVarying: this.targetTextureVarying,
                             targetTexture: r
                         });
                         Object.assign(o, t)
@@ -19420,15 +19423,15 @@
                 }
                 getData() {
                     let {
                         packed: t = !1
                     } = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     const {
                         framebuffer: e
-                    } = this.bindings[this.currentIndex], n = lp(e);
+                    } = this.bindings[this.currentIndex], n = cp(e);
                     if (!t) return n;
                     const i = n.constructor,
                         r = function(t) {
                             switch (t) {
                                 case "float":
                                     return 1;
                                 case "vec2":
@@ -19462,15 +19465,15 @@
                     this._swapTexture = n, this.targetTextureVarying = e, this.hasTargetTexture = e, this._setupTextures(t)
                 }
                 _createTargetTexture(t) {
                     const {
                         sourceTextures: e,
                         textureOrReference: n
                     } = t;
-                    if (n instanceof Qd) return n;
+                    if (n instanceof Jd) return n;
                     const i = e[n];
                     return i ? (this._targetRefTexName = n, this._createNewTexture(i)) : null
                 }
                 _setupTextures() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     const {
                         sourceBuffers: e,
@@ -19489,15 +19492,15 @@
                 _updateElementIDBuffer(t) {
                     if ("number" != typeof t || this.elementCount >= t) return;
                     const e = new Float32Array(t);
                     e.forEach(((t, e, n) => {
                         n[e] = e
                     })), this.elementIDBuffer ? this.elementIDBuffer.setData({
                         data: e
-                    }) : this.elementIDBuffer = new Wd(this.gl, {
+                    }) : this.elementIDBuffer = new Hd(this.gl, {
                         data: e,
                         accessor: {
                             size: 1
                         }
                     }), this.elementCount = t
                 }
                 _updateBindings(t) {
@@ -19534,15 +19537,15 @@
                             attachments: {
                                 36064: r
                             },
                             resizeAttachments: !1
                         }), i.resize({
                             width: e,
                             height: n
-                        })) : t.framebuffer = new bp(this.gl, {
+                        })) : t.framebuffer = new yp(this.gl, {
                             id: "transform-framebuffer",
                             width: e,
                             height: n,
                             attachments: {
                                 36064: r
                             }
                         })
@@ -19550,27 +19553,27 @@
                     return t
                 }
                 _setSourceTextureParameters() {
                     const t = this.currentIndex,
                         {
                             sourceTextures: e
                         } = this.bindings[t];
-                    for (const t in e) e[t].setParameters(Lv)
+                    for (const t in e) e[t].setParameters(Rv)
                 }
                 _swapTextures(t) {
                     if (!this._swapTexture) return null;
                     const e = Object.assign({}, t.sourceTextures);
                     return e[this._swapTexture] = t.targetTexture, {
                         sourceTextures: e,
                         targetTexture: t.sourceTextures[this._swapTexture]
                     }
                 }
                 _createNewTexture(t) {
                     const e = function(t, e) {
-                        Ed(t instanceof Qd || t instanceof sp || t instanceof op);
+                        Pd(t instanceof Jd || t instanceof op || t instanceof ap);
                         const n = t.constructor,
                             {
                                 gl: i,
                                 width: r,
                                 height: s,
                                 format: o,
                                 type: a,
@@ -19628,30 +19631,30 @@
                             const t = l.split("\n"),
                                 e = t.slice();
                             if (t.forEach(((t, r, l) => {
                                     if (s > 0) {
                                         const i = function(t, e) {
                                             const n = {},
                                                 i = function(t) {
-                                                    return Ev(t, ["attribute", "in"])
+                                                    return Pv(t, ["attribute", "in"])
                                                 }(t);
                                             if (!i) return null;
                                             const {
                                                 type: r,
                                                 name: s
                                             } = i;
                                             if (s && e[s]) {
                                                 const e = "// ".concat(t, " => Replaced by Transform with a sampler"),
                                                     {
                                                         samplerName: i,
                                                         sizeName: o,
                                                         uniformDeclerations: a
                                                     } = function(t) {
                                                         const e = "".concat("transform_uSampler_").concat(t),
-                                                            n = "".concat(Mv).concat(t);
+                                                            n = "".concat(Ov).concat(t);
                                                         return {
                                                             samplerName: e,
                                                             sizeName: n,
                                                             uniformDeclerations: "  uniform sampler2D ".concat(e, ";\n  uniform vec2 ").concat(n, ";")
                                                         }
                                                     }(s),
                                                     l = function(t) {
@@ -19685,22 +19688,22 @@
                                                 updatedLine: t,
                                                 inject: n
                                             } = i;
                                             e[r] = t, c = uu([c, n]), Object.assign(a, i.samplerTextureMap), s--
                                         }
                                     }
                                     i && !o && (o = function(t, e) {
-                                        const n = Ev(t, ["varying", "out"]);
+                                        const n = Pv(t, ["varying", "out"]);
                                         return n && n.name === e ? n.type : null
                                     }(t, i))
                                 })), i) {
-                                Ed(r);
-                                const t = "".concat(Mv).concat(i),
+                                Pd(r);
+                                const t = "".concat(Ov).concat(i),
                                     e = "uniform vec2 ".concat(t, ";\n"),
-                                    n = "     vec2 ".concat(Ov, " = transform_getPos(").concat(t, ");\n     gl_Position = vec4(").concat(Ov, ", 0, 1.);\n");
+                                    n = "     vec2 ".concat(Lv, " = transform_getPos(").concat(t, ");\n     gl_Position = vec4(").concat(Lv, ", 0, 1.);\n");
                                 c = uu([c, {
                                     "vs:#decl": e,
                                     "vs:#main-start": n
                                 }])
                             }
                             l = e.join("\n")
                         }
@@ -19714,81 +19717,81 @@
                         vs: t.vs,
                         sourceTextureMap: e,
                         targetTextureVarying: this.targetTextureVarying,
                         targetTexture: n
                     }), l = uu([t.inject || {}, o]);
                     return this.targetTextureType = s, this.samplerTextureMap = a, {
                         vs: i,
-                        fs: t._fs || Pv({
-                            version: Tv(i),
+                        fs: t._fs || Sv({
+                            version: Av(i),
                             input: this.targetTextureVarying,
                             inputType: s,
                             output: "transform_output"
                         }),
-                        modules: this.hasSourceTextures || this.targetTextureVarying ? [Av].concat(t.modules || []) : t.modules,
+                        modules: this.hasSourceTextures || this.targetTextureVarying ? [Mv].concat(t.modules || []) : t.modules,
                         uniforms: r,
                         inject: l
                     }
                 }
             }
-            let Iv = null;
-            class kv extends Rd {
+            let kv = null;
+            class jv extends Id {
                 get[Symbol.toStringTag]() {
                     return "VertexArrayObject"
                 }
                 static isSupported(t) {
-                    return !(arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {}).constantAttributeZero || Lu(t) || "Chrome" === sm()
+                    return !(arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {}).constantAttributeZero || Lu(t) || "Chrome" === om()
                 }
                 static getDefaultArray(t) {
-                    return t.luma = t.luma || {}, t.luma.defaultVertexArray || (t.luma.defaultVertexArray = new kv(t, {
+                    return t.luma = t.luma || {}, t.luma.defaultVertexArray || (t.luma.defaultVertexArray = new jv(t, {
                         handle: null,
                         isDefaultArray: !0
                     })), t.luma.defaultVertexArray
                 }
                 static getMaxAttributes(t) {
-                    return kv.MAX_ATTRIBUTES = kv.MAX_ATTRIBUTES || t.getParameter(34921), kv.MAX_ATTRIBUTES
+                    return jv.MAX_ATTRIBUTES = jv.MAX_ATTRIBUTES || t.getParameter(34921), jv.MAX_ATTRIBUTES
                 }
                 static setConstant(t, e, n) {
                     switch (n.constructor) {
                         case Float32Array:
-                            kv._setConstantFloatArray(t, e, n);
+                            jv._setConstantFloatArray(t, e, n);
                             break;
                         case Int32Array:
-                            kv._setConstantIntArray(t, e, n);
+                            jv._setConstantIntArray(t, e, n);
                             break;
                         case Uint32Array:
-                            kv._setConstantUintArray(t, e, n);
+                            jv._setConstantUintArray(t, e, n);
                             break;
                         default:
-                            Ed(!1)
+                            Pd(!1)
                     }
                 }
                 constructor(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                     const n = e.id || e.program && e.program.id;
                     super(t, Object.assign({}, e, {
                         id: n
                     })), this.buffer = null, this.bufferValue = null, this.isDefaultArray = e.isDefaultArray || !1, this.gl2 = t, this.initialize(e), Object.seal(this)
                 }
                 delete() {
                     return super.delete(), this.buffer && this.buffer.delete(), this
                 }
                 get MAX_ATTRIBUTES() {
-                    return kv.getMaxAttributes(this.gl)
+                    return jv.getMaxAttributes(this.gl)
                 }
                 initialize() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     return this.setProps(t)
                 }
                 setProps(t) {
                     return this
                 }
                 setElementBuffer() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : null;
-                    return Ed(!t || 34963 === t.target, "elements must be GL.ELEMENT_ARRAY_BUFFER"), this.bind((() => {
+                    return Pd(!t || 34963 === t.target, "elements must be GL.ELEMENT_ARRAY_BUFFER"), this.bind((() => {
                         this.gl.bindBuffer(34963, t ? t.handle : null)
                     })), this
                 }
                 setBuffer(t, e, n) {
                     if (34963 === e.target) return this.setElementBuffer(e, n);
                     const {
                         size: i,
@@ -19799,32 +19802,32 @@
                         integer: l,
                         divisor: c
                     } = n, {
                         gl: h,
                         gl2: u
                     } = this;
                     return t = Number(t), this.bind((() => {
-                        h.bindBuffer(34962, e.handle), l ? (Ed(Lu(h)), u.vertexAttribIPointer(t, i, r, s, o)) : h.vertexAttribPointer(t, i, r, a, s, o), h.enableVertexAttribArray(t), u.vertexAttribDivisor(t, c || 0)
+                        h.bindBuffer(34962, e.handle), l ? (Pd(Lu(h)), u.vertexAttribIPointer(t, i, r, s, o)) : h.vertexAttribPointer(t, i, r, a, s, o), h.enableVertexAttribArray(t), u.vertexAttribDivisor(t, c || 0)
                     })), this
                 }
                 enable(t) {
                     let e = !(arguments.length > 1 && void 0 !== arguments[1]) || arguments[1];
-                    return !e && 0 === t && !kv.isSupported(this.gl, {
+                    return !e && 0 === t && !jv.isSupported(this.gl, {
                         constantAttributeZero: !0
                     }) || (t = Number(t), this.bind((() => e ? this.gl.enableVertexAttribArray(t) : this.gl.disableVertexAttribArray(t)))), this
                 }
                 getConstantBuffer(t, e) {
                     const n = this._normalizeConstantArrayValue(e),
                         i = n.byteLength * t,
                         r = n.length * t;
                     let s = !this.buffer;
-                    if (this.buffer = this.buffer || new Wd(this.gl, i), s = s || this.buffer.reallocate(i), s = s || !this._compareConstantArrayValues(n, this.bufferValue), s) {
+                    if (this.buffer = this.buffer || new Hd(this.gl, i), s = s || this.buffer.reallocate(i), s = s || !this._compareConstantArrayValues(n, this.bufferValue), s) {
                         const t = function(t, e) {
                             var n;
-                            return new t((n = t.BYTES_PER_ELEMENT * e, (!Iv || Iv.byteLength < n) && (Iv = new ArrayBuffer(n)), Iv), 0, e)
+                            return new t((n = t.BYTES_PER_ELEMENT * e, (!kv || kv.byteLength < n) && (kv = new ArrayBuffer(n)), kv), 0, e)
                         }(e.constructor, r);
                         ! function(t) {
                             let {
                                 target: e,
                                 source: n,
                                 start: i = 0,
                                 count: r = 1
@@ -19863,51 +19866,51 @@
                         case 3:
                             t.vertexAttrib3fv(e, n);
                             break;
                         case 4:
                             t.vertexAttrib4fv(e, n);
                             break;
                         default:
-                            Ed(!1)
+                            Pd(!1)
                     }
                 }
                 static _setConstantIntArray(t, e, n) {
-                    switch (Ed(Lu(t)), n.length) {
+                    switch (Pd(Lu(t)), n.length) {
                         case 1:
                             t.vertexAttribI1iv(e, n);
                             break;
                         case 2:
                             t.vertexAttribI2iv(e, n);
                             break;
                         case 3:
                             t.vertexAttribI3iv(e, n);
                             break;
                         case 4:
                             t.vertexAttribI4iv(e, n);
                             break;
                         default:
-                            Ed(!1)
+                            Pd(!1)
                     }
                 }
                 static _setConstantUintArray(t, e, n) {
-                    switch (Ed(Lu(t)), n.length) {
+                    switch (Pd(Lu(t)), n.length) {
                         case 1:
                             t.vertexAttribI1uiv(e, n);
                             break;
                         case 2:
                             t.vertexAttribI2uiv(e, n);
                             break;
                         case 3:
                             t.vertexAttribI3uiv(e, n);
                             break;
                         case 4:
                             t.vertexAttribI4uiv(e, n);
                             break;
                         default:
-                            Ed(!1)
+                            Pd(!1)
                     }
                 }
                 _createHandle() {
                     return this.gl.createVertexArray()
                 }
                 _deleteHandle(t) {
                     return this.gl2.deleteVertexArray(t), [this.elements]
@@ -19915,24 +19918,24 @@
                 _bindHandle(t) {
                     this.gl2.bindVertexArray(t)
                 }
                 _getParameter(t, e) {
                     let {
                         location: n
                     } = e;
-                    return Ed(Number.isFinite(n)), this.bind((() => 34373 === t ? this.gl.getVertexAttribOffset(n, t) : this.gl.getVertexAttrib(n, t)))
+                    return Pd(Number.isFinite(n)), this.bind((() => 34373 === t ? this.gl.getVertexAttribOffset(n, t) : this.gl.getVertexAttrib(n, t)))
                 }
             }
-            const jv = /^(.+)__LOCATION_([0-9]+)$/,
-                Fv = ["setBuffers", "setGeneric", "clearBindings", "setLocations", "setGenericValues", "setDivisor", "enable", "disable"];
-            class zv {
+            const Fv = /^(.+)__LOCATION_([0-9]+)$/,
+                zv = ["setBuffers", "setGeneric", "clearBindings", "setLocations", "setGenericValues", "setDivisor", "enable", "disable"];
+            class Bv {
                 constructor(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                     const n = e.id || e.program && e.program.id;
-                    this.id = n, this.gl = t, this.configuration = null, this.elements = null, this.elementsAccessor = null, this.values = null, this.accessors = null, this.unused = null, this.drawParams = null, this.buffer = null, this.attributes = {}, this.vertexArrayObject = new kv(t), Od(this, "VertexArray", "v6.0", Fv), this.initialize(e), Object.seal(this)
+                    this.id = n, this.gl = t, this.configuration = null, this.elements = null, this.elementsAccessor = null, this.values = null, this.accessors = null, this.unused = null, this.drawParams = null, this.buffer = null, this.attributes = {}, this.vertexArrayObject = new jv(t), Ld(this, "VertexArray", "v6.0", zv), this.initialize(e), Object.seal(this)
                 }
                 delete() {
                     this.buffer && this.buffer.delete(), this.vertexArrayObject.delete()
                 }
                 initialize() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     return this.reset(), this.configuration = null, this.bindOnUse = !1, this.setProps(t)
@@ -19984,28 +19987,28 @@
                     } = this._resolveLocationAndAccessor(t, e, Object.assign({
                         size: e.length
                     }, n));
                     return i >= 0 && (e = this.vertexArrayObject._normalizeConstantArrayValue(e), this.values[i] = e, this.accessors[i] = r, this.clearDrawParams(), this.vertexArrayObject.enable(i, !1)), this
                 }
                 unbindBuffers() {
                     return this.vertexArrayObject.bind((() => {
-                        this.elements && this.vertexArrayObject.setElementBuffer(null), this.buffer = this.buffer || new Wd(this.gl, {
+                        this.elements && this.vertexArrayObject.setElementBuffer(null), this.buffer = this.buffer || new Hd(this.gl, {
                             accessor: {
                                 size: 4
                             }
                         });
-                        for (let t = 0; t < this.vertexArrayObject.MAX_ATTRIBUTES; t++) this.values[t] instanceof Wd && (this.gl.disableVertexAttribArray(t), this.gl.bindBuffer(34962, this.buffer.handle), this.gl.vertexAttribPointer(t, 1, 5126, !1, 0, 0))
+                        for (let t = 0; t < this.vertexArrayObject.MAX_ATTRIBUTES; t++) this.values[t] instanceof Hd && (this.gl.disableVertexAttribArray(t), this.gl.bindBuffer(34962, this.buffer.handle), this.gl.vertexAttribPointer(t, 1, 5126, !1, 0, 0))
                     })), this
                 }
                 bindBuffers() {
                     return this.vertexArrayObject.bind((() => {
                         this.elements && this.setElementBuffer(this.elements);
                         for (let t = 0; t < this.vertexArrayObject.MAX_ATTRIBUTES; t++) {
                             const e = this.values[t];
-                            e instanceof Wd && this.setBuffer(t, e)
+                            e instanceof Hd && this.setBuffer(t, e)
                         }
                     })), this
                 }
                 bindForDraw(t, e, n) {
                     let i;
                     return this.vertexArrayObject.bind((() => {
                         this._setConstantAttributes(t, e), i = n()
@@ -20020,73 +20023,73 @@
                             location: s,
                             name: o
                         } = this._getAttributeIndex(t);
                     if (!Number.isFinite(s) || s < 0) return this.unused[t] = e, Tu.once(3, (() => "unused value ".concat(t, " in ").concat(this.id)))(), r;
                     const a = this._getAttributeInfo(o || s);
                     if (!a) return r;
                     const l = this.accessors[s] || {},
-                        c = Nd.resolve(a.accessor, l, n, i),
+                        c = Vd.resolve(a.accessor, l, n, i),
                         {
                             size: h,
                             type: u
                         } = c;
-                    return Ed(Number.isFinite(h) && Number.isFinite(u)), {
+                    return Pd(Number.isFinite(h) && Number.isFinite(u)), {
                         location: s,
                         accessor: c
                     }
                 }
                 _getAttributeInfo(t) {
                     return this.configuration && this.configuration.getAttributeInfo(t)
                 }
                 _getAttributeIndex(t) {
                     const e = Number(t);
                     if (Number.isFinite(e)) return {
                         location: e
                     };
-                    const n = jv.exec(t),
+                    const n = Fv.exec(t),
                         i = n ? n[1] : t,
                         r = n ? Number(n[2]) : 0;
                     return this.configuration ? {
                         location: this.configuration.getAttributeLocation(i) + r,
                         name: i
                     } : {
                         location: -1
                     }
                 }
                 _setAttribute(t, e) {
-                    if (e instanceof Wd) this.setBuffer(t, e);
-                    else if (Array.isArray(e) && e.length && e[0] instanceof Wd) {
+                    if (e instanceof Hd) this.setBuffer(t, e);
+                    else if (Array.isArray(e) && e.length && e[0] instanceof Hd) {
                         const n = e[0],
                             i = e[1];
                         this.setBuffer(t, n, i)
                     } else if (ArrayBuffer.isView(e) || Array.isArray(e)) {
                         const n = e;
                         this.setConstant(t, n)
                     } else {
-                        if (!(e.buffer instanceof Wd)) throw new Error("VertexArray: attributes must be Buffers or constants (i.e. typed array)"); {
+                        if (!(e.buffer instanceof Hd)) throw new Error("VertexArray: attributes must be Buffers or constants (i.e. typed array)"); {
                             const n = e;
                             this.setBuffer(t, n.buffer, n)
                         }
                     }
                 }
                 _setConstantAttributes(t, e) {
                     const n = Math.max(0 | t, 0 | e);
                     let i = this.values[0];
                     ArrayBuffer.isView(i) && this._setConstantAttributeZero(i, n);
                     for (let t = 1; t < this.vertexArrayObject.MAX_ATTRIBUTES; t++) i = this.values[t], ArrayBuffer.isView(i) && this._setConstantAttribute(t, i)
                 }
                 _setConstantAttributeZero(t, e) {
-                    if (kv.isSupported(this.gl, {
+                    if (jv.isSupported(this.gl, {
                             constantAttributeZero: !0
                         })) return void this._setConstantAttribute(0, t);
                     const n = this.vertexArrayObject.getConstantBuffer(e, t);
                     this.vertexArrayObject.setBuffer(0, n, this.accessors[0])
                 }
                 _setConstantAttribute(t, e) {
-                    kv.setConstant(this.gl, t, e)
+                    jv.setConstant(this.gl, t, e)
                 }
                 _updateDrawParams() {
                     const t = {
                         isIndexed: !1,
                         isInstanced: !1,
                         indexCount: 1 / 0,
                         vertexCount: 1 / 0,
@@ -20098,15 +20101,15 @@
                 _updateDrawParamsForLocation(t, e) {
                     const n = this.values[e],
                         i = this.accessors[e];
                     if (!n) return;
                     const {
                         divisor: r
                     } = i, s = r > 0;
-                    if (t.isInstanced = t.isInstanced || s, n instanceof Wd) {
+                    if (t.isInstanced = t.isInstanced || s, n instanceof Hd) {
                         const e = n;
                         if (s) {
                             const n = e.getVertexCount(i);
                             t.instanceCount = Math.min(t.instanceCount, n)
                         } else {
                             const n = e.getVertexCount(i);
                             t.vertexCount = Math.min(t.vertexCount, n)
@@ -20116,179 +20119,179 @@
                 setElements() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : null,
                         e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                     return Tu.deprecated("setElements", "setElementBuffer")(), this.setElementBuffer(t, e)
                 }
             }
 
-            function Bv(t) {
+            function Dv(t) {
                 let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                 const {
                     isInteger: n = !1
                 } = e;
                 if (Array.isArray(t) || ArrayBuffer.isView(t)) return function(t, e) {
                     const {
                         maxElts: n = 16,
                         size: i = 1
                     } = e;
                     let r = "[";
-                    for (let s = 0; s < t.length && s < n; ++s) s > 0 && (r += ",".concat(s % i == 0 ? " " : "")), r += Bv(t[s], e);
+                    for (let s = 0; s < t.length && s < n; ++s) s > 0 && (r += ",".concat(s % i == 0 ? " " : "")), r += Dv(t[s], e);
                     const s = t.length > n ? "..." : "]";
                     return "".concat(r).concat(s)
                 }(t, e);
                 if (!Number.isFinite(t)) return String(t);
                 if (Math.abs(t) < 1e-16) return n ? "0" : "0.";
                 if (n) return t.toFixed(0);
                 if (Math.abs(t) > 100 && Math.abs(t) < 1e4) return t.toFixed(0);
                 const i = t.toPrecision(2);
                 return i.indexOf(".0") === i.length - 2 ? i.slice(0, -1) : i
             }
 
-            function Dv(t, e, n, i) {
+            function Nv(t, e, n, i) {
                 const {
                     gl: r
                 } = t;
                 if (!e) return {
                     [i]: "null",
                     "Format ": "N/A"
                 };
                 let s, o, a, l = "NOT PROVIDED",
                     c = 1,
                     h = 0,
                     u = 0;
-                if (n && (l = n.type, c = n.size, l = String(l).replace("Array", ""), s = -1 !== l.indexOf("nt")), e instanceof Wd) {
+                if (n && (l = n.type, c = n.size, l = String(l).replace("Array", ""), s = -1 !== l.indexOf("nt")), e instanceof Hd) {
                     const t = e,
                         {
                             data: d,
                             changed: p
                         } = t.getDebugData();
                     let f;
                     if (o = p ? "*" : "", a = d, u = t.byteLength, h = u / d.BYTES_PER_ELEMENT / c, n) {
                         const t = n.divisor > 0;
-                        f = "".concat(t ? "I " : "P ", " ").concat(h, " (x").concat(c, "=").concat(u, " bytes ").concat(Sd(r, l), ")")
+                        f = "".concat(t ? "I " : "P ", " ").concat(h, " (x").concat(c, "=").concat(u, " bytes ").concat(Cd(r, l), ")")
                     } else s = !0, f = "".concat(u, " bytes");
                     return {
-                        [i]: "".concat(o).concat(Bv(a, {
+                        [i]: "".concat(o).concat(Dv(a, {
                             size: c,
                             isInteger: s
                         })),
                         "Format ": f
                     }
                 }
                 return a = e, c = e.length, l = String(e.constructor.name).replace("Array", ""), s = -1 !== l.indexOf("nt"), {
-                    [i]: "".concat(Bv(a, {
+                    [i]: "".concat(Dv(a, {
                         size: c,
                         isInteger: s
                     }), " (constant)"),
                     "Format ": "".concat(c, "x").concat(l, " (constant)")
                 }
             }
 
-            function Nv(t, e) {
+            function Vv(t, e) {
                 const {
                     type: n,
                     size: i
-                } = e, r = Qp(n, i);
+                } = e, r = Jp(n, i);
                 return r ? "".concat(t, " (").concat(r.name, ")") : t
             }
 
-            function Vv(t) {
+            function Uv(t) {
                 let {
                     header: e = "Uniforms",
                     program: n,
                     uniforms: i,
                     undefinedOnly: r = !1
                 } = t;
-                Ed(n);
+                Pd(n);
                 const s = ".*Matrix",
                     o = n._uniformSetters,
                     a = {},
                     l = Object.keys(o).sort();
                 let c = 0;
-                for (const t of l) t.match(".*_.*") || t.match(s) || Uv({
+                for (const t of l) t.match(".*_.*") || t.match(s) || Gv({
                     table: a,
                     header: e,
                     uniforms: i,
                     uniformName: t,
                     undefinedOnly: r
                 }) && c++;
-                for (const t of l) t.match(s) && Uv({
+                for (const t of l) t.match(s) && Gv({
                     table: a,
                     header: e,
                     uniforms: i,
                     uniformName: t,
                     undefinedOnly: r
                 }) && c++;
-                for (const t of l) a[t] || Uv({
+                for (const t of l) a[t] || Gv({
                     table: a,
                     header: e,
                     uniforms: i,
                     uniformName: t,
                     undefinedOnly: r
                 }) && c++;
                 let h = 0;
                 const u = {};
                 if (!r)
                     for (const t in i) {
                         const n = i[t];
                         a[t] || (h++, u[t] = {
                             Type: "NOT USED: ".concat(n),
-                            [e]: Bv(n)
+                            [e]: Dv(n)
                         })
                     }
                 return {
                     table: a,
                     count: c,
                     unusedTable: u,
                     unusedCount: h
                 }
             }
 
-            function Uv(t) {
+            function Gv(t) {
                 let {
                     table: e,
                     header: n,
                     uniforms: i,
                     uniformName: r,
                     undefinedOnly: s
                 } = t;
                 const o = i[r],
                     a = function(t) {
                         return null != t
                     }(o);
                 return !(s && a || (e[r] = {
-                    [n]: a ? Bv(o) : "N/A",
+                    [n]: a ? Dv(o) : "N/A",
                     "Uniform Type": a ? o : "NOT PROVIDED"
                 }, 0))
             }
 
-            function Gv(t) {
+            function Wv(t) {
                 const {
                     type: e,
                     size: n
-                } = t.accessor, i = Qp(e, n);
+                } = t.accessor, i = Jp(e, n);
                 return i ? "".concat(i.name, " ").concat(t.name) : t.name
             }
-            const Wv = {
+            const Hv = {
                 POSITION: "positions",
                 NORMAL: "normals",
                 COLOR_0: "colors",
                 TEXCOORD_0: "texCoords",
                 TEXCOORD_1: "texCoords1",
                 TEXCOORD_2: "texCoords2"
             };
 
-            function Hv(t, e) {
+            function Zv(t, e) {
                 const {
-                    attributeMap: n = Wv
+                    attributeMap: n = Hv
                 } = e || {};
                 return n && n[t] || t
             }
 
-            function Zv(t, e) {
+            function qv(t, e) {
                 let n;
                 switch (t) {
                     case "texCoords":
                     case "texCoord1":
                     case "texCoord2":
                     case "texCoord3":
                         n = "uvs";
@@ -20302,28 +20305,28 @@
                 switch (n) {
                     case "vectors":
                         e.size = e.size || 3;
                         break;
                     case "uvs":
                         e.size = e.size || 2
                 }
-                Ed(Number.isFinite(e.size), "attribute ".concat(t, " needs size"))
+                Pd(Number.isFinite(e.size), "attribute ".concat(t, " needs size"))
             }
-            const qv = () => {},
-                Xv = {};
-            class Yv {
+            const Xv = () => {},
+                Yv = {};
+            class Kv {
                 constructor(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                     const {
-                        id: n = Td("model")
+                        id: n = Ad("model")
                     } = e;
-                    Ed(Ou(t)), this.id = n, this.gl = t, this.id = e.id || Td("Model"), this.lastLogTime = 0, this.animated = !1, this.initialize(e)
+                    Pd(Ou(t)), this.id = n, this.gl = t, this.id = e.id || Ad("Model"), this.lastLogTime = 0, this.animated = !1, this.initialize(e)
                 }
                 initialize(t) {
-                    this.props = {}, this.programManager = t.programManager || nf.getDefaultProgramManager(this.gl), this._programManagerState = -1, this._managedProgram = !1;
+                    this.props = {}, this.programManager = t.programManager || rf.getDefaultProgramManager(this.gl), this._programManagerState = -1, this._managedProgram = !1;
                     const {
                         program: e = null,
                         vs: n,
                         fs: i,
                         modules: r,
                         defines: s,
                         inject: o,
@@ -20337,15 +20340,15 @@
                         fs: i,
                         modules: r,
                         defines: s,
                         inject: o,
                         varyings: a,
                         bufferMode: l,
                         transpileToGLSL100: c
-                    }, this.program = null, this.vertexArray = null, this._programDirty = !0, this.userData = {}, this.needsRedraw = !0, this._attributes = {}, this.attributes = {}, this.uniforms = {}, this.pickable = !0, this._checkProgram(), this.setUniforms(Object.assign({}, this.getModuleUniforms(t.moduleSettings))), this.drawMode = void 0 !== t.drawMode ? t.drawMode : 4, this.vertexCount = t.vertexCount || 0, this.geometryBuffers = {}, this.isInstanced = t.isInstanced || t.instanced || t.instanceCount > 0, this._setModelProps(t), this.geometry = {}, Ed(void 0 !== this.drawMode && Number.isFinite(this.vertexCount), "Model needs drawMode and vertexCount")
+                    }, this.program = null, this.vertexArray = null, this._programDirty = !0, this.userData = {}, this.needsRedraw = !0, this._attributes = {}, this.attributes = {}, this.uniforms = {}, this.pickable = !0, this._checkProgram(), this.setUniforms(Object.assign({}, this.getModuleUniforms(t.moduleSettings))), this.drawMode = void 0 !== t.drawMode ? t.drawMode : 4, this.vertexCount = t.vertexCount || 0, this.geometryBuffers = {}, this.isInstanced = t.isInstanced || t.instanced || t.instanceCount > 0, this._setModelProps(t), this.geometry = {}, Pd(void 0 !== this.drawMode && Number.isFinite(this.vertexCount), "Model needs drawMode and vertexCount")
                 }
                 setProps(t) {
                     this._setModelProps(t)
                 }
                 delete() {
                     for (const t in this._attributes) this._attributes[t] !== this.attributes[t] && this._attributes[t].delete();
                     this._managedProgram && (this.programManager.release(this.program), this._managedProgram = !1), this.vertexArray.delete(), this._deleteGeometryBuffers()
@@ -20392,54 +20395,54 @@
                 getUniforms() {
                     return this.uniforms
                 }
                 setDrawMode(t) {
                     return this.drawMode = t, this
                 }
                 setVertexCount(t) {
-                    return Ed(Number.isFinite(t)), this.vertexCount = t, this
+                    return Pd(Number.isFinite(t)), this.vertexCount = t, this
                 }
                 setInstanceCount(t) {
-                    return Ed(Number.isFinite(t)), this.instanceCount = t, this
+                    return Pd(Number.isFinite(t)), this.instanceCount = t, this
                 }
                 setGeometry(t) {
                     return this.drawMode = t.drawMode, this.vertexCount = t.getVertexCount(), this._deleteGeometryBuffers(), this.geometryBuffers = function(t, e, n) {
                         const i = {};
                         let r = e.indices;
                         for (const n in e.attributes) {
                             const s = e.attributes[n],
-                                o = Hv(n, undefined);
+                                o = Zv(n, undefined);
                             if ("indices" === n) r = s;
                             else if (s.constant) i[o] = s.value;
                             else {
                                 const e = s.value,
                                     r = {
                                         ...s
                                     };
-                                delete r.value, i[o] = [new Wd(t, e), r], Zv(n, r)
+                                delete r.value, i[o] = [new Hd(t, e), r], qv(n, r)
                             }
                         }
                         if (r) {
                             const e = r.value || r;
-                            Ed(e instanceof Uint16Array || e instanceof Uint32Array, 'attribute array for "indices" must be of integer type');
+                            Pd(e instanceof Uint16Array || e instanceof Uint32Array, 'attribute array for "indices" must be of integer type');
                             const n = {
                                 size: 1,
                                 isIndexed: void 0 === r.isIndexed || r.isIndexed
                             };
-                            i.indices = [new Wd(t, {
+                            i.indices = [new Hd(t, {
                                 data: e,
                                 target: 34963
                             }), n]
                         }
                         return i
                     }(this.gl, t), this.vertexArray.setAttributes(this.geometryBuffers), this
                 }
                 setAttributes() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
-                    if (Md(t)) return this;
+                    if (Od(t)) return this;
                     const e = {};
                     for (const n in t) {
                         const i = t[n];
                         e[n] = i.getValue ? i.getValue() : i
                     }
                     return this.vertexArray.setAttributes(e), this
                 }
@@ -20453,15 +20456,15 @@
                     return e ? e(t) : {}
                 }
                 updateModuleSettings(t) {
                     const e = this.getModuleUniforms(t || {});
                     return this.setUniforms(e)
                 }
                 clear(t) {
-                    return ip(this.program.gl, t), this
+                    return rp(this.program.gl, t), this
                 }
                 draw() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     this._checkProgram();
                     const {
                         moduleSettings: e = null,
                         framebuffer: n,
@@ -20481,19 +20484,19 @@
                             vertexArrayInstanced: p = c.isInstanced
                         } = this.props;
                     p && !this.isInstanced && Tu.warn("Found instanced attributes on non-instanced model", this.id)();
                     const {
                         isInstanced: f,
                         instanceCount: g
                     } = this, {
-                        onBeforeRender: m = qv,
-                        onAfterRender: v = qv
+                        onBeforeRender: m = Xv,
+                        onAfterRender: v = Xv
                     } = this.props;
                     m(), this.program.setUniforms(this.uniforms);
-                    const b = this.program.draw(Object.assign(Xv, t, {
+                    const b = this.program.draw(Object.assign(Yv, t, {
                         logPriority: l,
                         uniforms: null,
                         framebuffer: n,
                         parameters: o,
                         drawMode: this.getDrawMode(),
                         vertexCount: this.getVertexCount(),
                         vertexArray: a,
@@ -20559,37 +20562,37 @@
                             inject: r,
                             defines: s,
                             varyings: o,
                             bufferMode: a,
                             transpileToGLSL100: l
                         }), this.program && this._managedProgram && this.programManager.release(this.program), this._programManagerState = this.programManager.stateHash, this._managedProgram = !0
                     }
-                    Ed(t instanceof ef, "Model needs a program"), this._programDirty = !1, t !== this.program && (this.program = t, this.vertexArray ? this.vertexArray.setProps({
+                    Pd(t instanceof nf, "Model needs a program"), this._programDirty = !1, t !== this.program && (this.program = t, this.vertexArray ? this.vertexArray.setProps({
                         program: this.program,
                         attributes: this.vertexArray.attributes
-                    }) : this.vertexArray = new zv(this.gl, {
+                    }) : this.vertexArray = new Bv(this.gl, {
                         program: this.program
                     }), this.setUniforms(Object.assign({}, this.getModuleUniforms())))
                 }
                 _deleteGeometryBuffers() {
                     for (const t in this.geometryBuffers) {
                         const e = this.geometryBuffers[t][0] || this.geometryBuffers[t];
-                        e instanceof Wd && e.delete()
+                        e instanceof Hd && e.delete()
                     }
                 }
                 _setAnimationProps(t) {
-                    this.animated && Ed(t, "Model.draw(): animated uniforms but no animationProps")
+                    this.animated && Pd(t, "Model.draw(): animated uniforms but no animationProps")
                 }
                 _setFeedbackBuffers() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
-                    if (Md(t)) return this;
+                    if (Od(t)) return this;
                     const {
                         gl: e
                     } = this.program;
-                    return this.transformFeedback = this.transformFeedback || new Sv(e, {
+                    return this.transformFeedback = this.transformFeedback || new Cv(e, {
                         program: this.program
                     }), this.transformFeedback.setBuffers(t), this
                 }
                 _logDrawCallStart(t) {
                     const e = t > 3 ? 0 : 1e4;
                     if (!(Date.now() - this.lastLogTime < e)) return this.lastLogTime = Date.now(), Tu.group(2, ">>> DRAWING MODEL ".concat(this.id), {
                         collapsed: Tu.level <= 2
@@ -20600,73 +20603,73 @@
                     const r = function(t) {
                             let {
                                 vertexArray: e,
                                 header: n = "Attributes"
                             } = t;
                             if (!e.configuration) return {};
                             const i = {};
-                            e.elements && (i.ELEMENT_ARRAY_BUFFER = Dv(e, e.elements, null, n));
+                            e.elements && (i.ELEMENT_ARRAY_BUFFER = Nv(e, e.elements, null, n));
                             const r = e.values;
                             for (const t in r) {
                                 const s = e._getAttributeInfo(t);
                                 if (s) {
                                     let o = "".concat(t, ": ").concat(s.name);
                                     const a = e.accessors[s.location];
-                                    a && (o = "".concat(t, ": ").concat(Nv(s.name, a))), i[o] = Dv(e, r[t], a, n)
+                                    a && (o = "".concat(t, ": ").concat(Vv(s.name, a))), i[o] = Nv(e, r[t], a, n)
                                 }
                             }
                             return i
                         }({
                             vertexArray: e,
                             header: "".concat(this.id, " attributes"),
                             attributes: this._attributes
                         }),
                         {
                             table: s,
                             unusedTable: o,
                             unusedCount: a
-                        } = Vv({
+                        } = Uv({
                             header: "".concat(this.id, " uniforms"),
                             program: this.program,
                             uniforms: Object.assign({}, this.program.uniforms, n)
                         }),
                         {
                             table: l,
                             count: c
-                        } = Vv({
+                        } = Uv({
                             header: "".concat(this.id, " uniforms"),
                             program: this.program,
                             uniforms: Object.assign({}, this.program.uniforms, n),
                             undefinedOnly: !0
                         });
                     c > 0 && Tu.log("MISSING UNIFORMS", Object.keys(l))(), a > 0 && Tu.log("UNUSED UNIFORMS", Object.keys(o))();
                     const h = function(t) {
                         const e = {},
                             n = "Accessors for ".concat(t.id);
                         for (const i of t.attributeInfos)
                             if (i) {
-                                const t = Gv(i);
+                                const t = Wv(i);
                                 e["in ".concat(t)] = {
                                     [n]: JSON.stringify(i.accessor)
                                 }
                             } for (const i of t.varyingInfos)
                             if (i) {
-                                const t = Gv(i);
+                                const t = Wv(i);
                                 e["out ".concat(t)] = {
                                     [n]: JSON.stringify(i.accessor)
                                 }
                             } return e
                     }(this.vertexArray.configuration);
                     Tu.table(t, r)(), Tu.table(t, s)(), Tu.table(t + 1, h)(), i && i.log({
                         logLevel: 2,
                         message: "Rendered to ".concat(i.id)
                     }), Tu.groupEnd(2)()
                 }
             }
-            class Kv {
+            class Qv {
                 static isSupported(t) {
                     return Lu(t)
                 }
                 constructor(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : {};
                     this.gl = t, this.model = null, this.elementCount = 0, this.bufferTransform = null, this.textureTransform = null, this.elementIDBuffer = null, this._initialize(e), Object.seal(this)
                 }
@@ -20687,15 +20690,15 @@
                         color: !0
                     }), this.model.transform(n)
                 }
                 swap() {
                     let t = !1;
                     const e = [this.bufferTransform, this.textureTransform].filter(Boolean);
                     for (const n of e) t = t || n.swap();
-                    Ed(t, "Nothing to swap")
+                    Pd(t, "Nothing to swap")
                 }
                 getBuffer() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : null;
                     return this.bufferTransform && this.bufferTransform.getBuffer(t)
                 }
                 getData() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
@@ -20716,17 +20719,17 @@
                     for (const n of e) n.update(t)
                 }
                 _initialize() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     const {
                         gl: e
                     } = this;
-                    this._buildResourceTransforms(e, t), t = this._updateModelProps(t), this.model = new Yv(e, Object.assign({}, t, {
-                        fs: t.fs || Pv({
-                            version: Tv(t.vs)
+                    this._buildResourceTransforms(e, t), t = this._updateModelProps(t), this.model = new Kv(e, Object.assign({}, t, {
+                        fs: t.fs || Sv({
+                            version: Av(t.vs)
                         }),
                         id: t.id || "transform-model",
                         drawMode: t.drawMode || 0,
                         vertexCount: t.elementCount
                     })), this.bufferTransform && this.bufferTransform.setupResources({
                         model: this.model
                     })
@@ -20735,81 +20738,81 @@
                     let e = Object.assign({}, t);
                     const n = [this.bufferTransform, this.textureTransform].filter(Boolean);
                     for (const t of n) e = t.updateModelProps(e);
                     return e
                 }
                 _buildResourceTransforms(t, e) {
                     (function(t) {
-                        return !(Md(t.feedbackBuffers) && Md(t.feedbackMap) && !(t.varyings && t.varyings.length > 0))
-                    })(e) && (this.bufferTransform = new Cv(t, e)),
+                        return !(Od(t.feedbackBuffers) && Od(t.feedbackMap) && !(t.varyings && t.varyings.length > 0))
+                    })(e) && (this.bufferTransform = new Tv(t, e)),
                     function(t) {
-                        return !(Md(t._sourceTextures) && !t._targetTexture && !t._targetTextureVarying)
-                    }(e) && (this.textureTransform = new Rv(t, e)), Ed(this.bufferTransform || this.textureTransform, "must provide source/feedback buffers or source/target textures")
+                        return !(Od(t._sourceTextures) && !t._targetTexture && !t._targetTextureVarying)
+                    }(e) && (this.textureTransform = new Iv(t, e)), Pd(this.bufferTransform || this.textureTransform, "must provide source/feedback buffers or source/target textures")
                 }
                 _updateDrawOptions(t) {
                     let e = Object.assign({}, t);
                     const n = [this.bufferTransform, this.textureTransform].filter(Boolean);
                     for (const t of n) e = Object.assign(e, t.getDrawOptions(e));
                     return e
                 }
             }
-            const Qv = {
+            const Jv = {
                 interpolation: class {
                     constructor({
                         gl: t,
                         attribute: e,
                         timeline: n
                     }) {
-                        wo(this, "gl", void 0), wo(this, "type", "interpolation"), wo(this, "attributeInTransition", void 0), wo(this, "settings", void 0), wo(this, "attribute", void 0), wo(this, "transition", void 0), wo(this, "currentStartIndices", void 0), wo(this, "currentLength", void 0), wo(this, "transform", void 0), wo(this, "buffers", void 0), this.gl = t, this.transition = new If(n), this.attribute = e, this.attributeInTransition = new _v(t, e.settings), this.currentStartIndices = e.startIndices, this.currentLength = 0, this.transform = function(t, e) {
-                            const n = mv(e.size);
-                            return new Kv(t, {
+                        wo(this, "gl", void 0), wo(this, "type", "interpolation"), wo(this, "attributeInTransition", void 0), wo(this, "settings", void 0), wo(this, "attribute", void 0), wo(this, "transition", void 0), wo(this, "currentStartIndices", void 0), wo(this, "currentLength", void 0), wo(this, "transform", void 0), wo(this, "buffers", void 0), this.gl = t, this.transition = new kf(n), this.attribute = e, this.attributeInTransition = new xv(t, e.settings), this.currentStartIndices = e.startIndices, this.currentLength = 0, this.transform = function(t, e) {
+                            const n = vv(e.size);
+                            return new Qv(t, {
                                 vs: "\n#define SHADER_NAME interpolation-transition-vertex-shader\n\nuniform float time;\nattribute ATTRIBUTE_TYPE aFrom;\nattribute ATTRIBUTE_TYPE aTo;\nvarying ATTRIBUTE_TYPE vCurrent;\n\nvoid main(void) {\n  vCurrent = mix(aFrom, aTo, time);\n  gl_Position = vec4(0.0);\n}\n",
                                 defines: {
                                     ATTRIBUTE_TYPE: n
                                 },
                                 varyings: ["vCurrent"]
                             })
                         }(t, e);
                         const i = {
                             byteLength: 0,
                             usage: 35050
                         };
-                        this.buffers = [new Wd(t, i), new Wd(t, i)]
+                        this.buffers = [new Hd(t, i), new Hd(t, i)]
                     }
                     get inProgress() {
                         return this.transition.inProgress
                     }
                     start(t, e) {
                         if (t.duration <= 0) return void this.transition.cancel();
                         this.settings = t;
                         const {
                             gl: n,
                             buffers: i,
                             attribute: r
                         } = this;
-                        vv(i);
+                        bv(i);
                         const s = {
                             numInstances: e,
                             attribute: r,
                             fromLength: this.currentLength,
                             fromStartIndices: this.currentStartIndices,
                             getData: t.enter
                         };
-                        for (const t of i) yv({
+                        for (const t of i) _v({
                             buffer: t,
                             ...s
                         });
-                        this.currentStartIndices = r.startIndices, this.currentLength = bv(r, e), this.attributeInTransition.setData({
+                        this.currentStartIndices = r.startIndices, this.currentLength = yv(r, e), this.attributeInTransition.setData({
                             buffer: i[1],
                             value: r.value
                         }), this.transition.start(t), this.transform.update({
                             elementCount: Math.floor(this.currentLength / r.size),
                             sourceBuffers: {
                                 aFrom: i[0],
-                                aTo: gv(0, r)
+                                aTo: mv(0, r)
                             },
                             feedbackBuffers: {
                                 vCurrent: i[1]
                             }
                         })
                     }
                     update() {
@@ -20838,54 +20841,54 @@
                 },
                 spring: class {
                     constructor({
                         gl: t,
                         attribute: e,
                         timeline: n
                     }) {
-                        wo(this, "gl", void 0), wo(this, "type", "spring"), wo(this, "attributeInTransition", void 0), wo(this, "settings", void 0), wo(this, "attribute", void 0), wo(this, "transition", void 0), wo(this, "currentStartIndices", void 0), wo(this, "currentLength", void 0), wo(this, "texture", void 0), wo(this, "framebuffer", void 0), wo(this, "transform", void 0), wo(this, "buffers", void 0), this.gl = t, this.type = "spring", this.transition = new If(n), this.attribute = e, this.attributeInTransition = new _v(t, {
+                        wo(this, "gl", void 0), wo(this, "type", "spring"), wo(this, "attributeInTransition", void 0), wo(this, "settings", void 0), wo(this, "attribute", void 0), wo(this, "transition", void 0), wo(this, "currentStartIndices", void 0), wo(this, "currentLength", void 0), wo(this, "texture", void 0), wo(this, "framebuffer", void 0), wo(this, "transform", void 0), wo(this, "buffers", void 0), this.gl = t, this.type = "spring", this.transition = new kf(n), this.attribute = e, this.attributeInTransition = new xv(t, {
                             ...e.settings,
                             normalized: !1
                         }), this.currentStartIndices = e.startIndices, this.currentLength = 0, this.texture = function(t) {
-                            return new Qd(t, {
+                            return new Jd(t, {
                                 data: new Uint8Array(4),
                                 format: 6408,
                                 type: 5121,
                                 border: 0,
                                 mipmaps: !1,
                                 dataFormat: 6408,
                                 width: 1,
                                 height: 1
                             })
                         }(t), this.framebuffer = function(t, e) {
-                            return new bp(t, {
+                            return new yp(t, {
                                 id: "spring-transition-is-transitioning-framebuffer",
                                 width: 1,
                                 height: 1,
                                 attachments: {
                                     36064: e
                                 }
                             })
                         }(t, this.texture), this.transform = function(t, e, n) {
-                            const i = mv(e.size);
-                            return new Kv(t, {
+                            const i = vv(e.size);
+                            return new Qv(t, {
                                 framebuffer: n,
                                 vs: "\n#define SHADER_NAME spring-transition-vertex-shader\n\n#define EPSILON 0.00001\n\nuniform float stiffness;\nuniform float damping;\nattribute ATTRIBUTE_TYPE aPrev;\nattribute ATTRIBUTE_TYPE aCur;\nattribute ATTRIBUTE_TYPE aTo;\nvarying ATTRIBUTE_TYPE vNext;\nvarying float vIsTransitioningFlag;\n\nATTRIBUTE_TYPE getNextValue(ATTRIBUTE_TYPE cur, ATTRIBUTE_TYPE prev, ATTRIBUTE_TYPE dest) {\n  ATTRIBUTE_TYPE velocity = cur - prev;\n  ATTRIBUTE_TYPE delta = dest - cur;\n  ATTRIBUTE_TYPE spring = delta * stiffness;\n  ATTRIBUTE_TYPE damper = velocity * -1.0 * damping;\n  return spring + damper + velocity + cur;\n}\n\nvoid main(void) {\n  bool isTransitioning = length(aCur - aPrev) > EPSILON || length(aTo - aCur) > EPSILON;\n  vIsTransitioningFlag = isTransitioning ? 1.0 : 0.0;\n\n  vNext = getNextValue(aCur, aPrev, aTo);\n  gl_Position = vec4(0, 0, 0, 1);\n  gl_PointSize = 100.0;\n}\n",
                                 fs: "\n#define SHADER_NAME spring-transition-is-transitioning-fragment-shader\n\nvarying float vIsTransitioningFlag;\n\nvoid main(void) {\n  if (vIsTransitioningFlag == 0.0) {\n    discard;\n  }\n  gl_FragColor = vec4(1.0);\n}",
                                 defines: {
                                     ATTRIBUTE_TYPE: i
                                 },
                                 varyings: ["vNext"]
                             })
                         }(t, e, this.framebuffer);
                         const i = {
                             byteLength: 0,
                             usage: 35050
                         };
-                        this.buffers = [new Wd(t, i), new Wd(t, i), new Wd(t, i)]
+                        this.buffers = [new Hd(t, i), new Hd(t, i), new Hd(t, i)]
                     }
                     get inProgress() {
                         return this.transition.inProgress
                     }
                     start(t, e) {
                         const {
                             gl: n,
@@ -20894,28 +20897,28 @@
                         } = this, s = {
                             numInstances: e,
                             attribute: r,
                             fromLength: this.currentLength,
                             fromStartIndices: this.currentStartIndices,
                             getData: t.enter
                         };
-                        for (const t of i) yv({
+                        for (const t of i) _v({
                             buffer: t,
                             ...s
                         });
-                        this.settings = t, this.currentStartIndices = r.startIndices, this.currentLength = bv(r, e), this.attributeInTransition.setData({
+                        this.settings = t, this.currentStartIndices = r.startIndices, this.currentLength = yv(r, e), this.attributeInTransition.setData({
                             buffer: i[1],
                             value: r.value
                         }), this.transition.start({
                             ...t,
                             duration: 1 / 0
                         }), this.transform.update({
                             elementCount: Math.floor(this.currentLength / r.size),
                             sourceBuffers: {
-                                aTo: gv(0, r)
+                                aTo: mv(0, r)
                             }
                         })
                     }
                     update() {
                         const {
                             buffers: t,
                             transform: e,
@@ -20943,32 +20946,32 @@
                             parameters: {
                                 depthTest: !1,
                                 blend: !0,
                                 viewport: [0, 0, 1, 1],
                                 blendFunc: [1, 1],
                                 blendEquation: [32776, 32776]
                             }
-                        }), vv(t), this.attributeInTransition.setData({
+                        }), bv(t), this.attributeInTransition.setData({
                             buffer: t[1],
                             value: this.attribute.value
-                        }), lp(n)[0] > 0 || i.end(), !0
+                        }), cp(n)[0] > 0 || i.end(), !0
                     }
                     cancel() {
                         this.transition.cancel(), this.transform.delete();
                         for (const t of this.buffers) t.delete();
                         this.buffers.length = 0, this.texture.delete(), this.framebuffer.delete()
                     }
                 }
             };
-            class Jv {
+            class $v {
                 constructor(t, {
                     id: e,
                     timeline: n
                 }) {
-                    wo(this, "id", void 0), wo(this, "isSupported", void 0), wo(this, "gl", void 0), wo(this, "timeline", void 0), wo(this, "transitions", void 0), wo(this, "needsRedraw", void 0), wo(this, "numInstances", void 0), this.id = e, this.gl = t, this.timeline = n, this.transitions = {}, this.needsRedraw = !1, this.numInstances = 1, this.isSupported = Kv.isSupported(t)
+                    wo(this, "id", void 0), wo(this, "isSupported", void 0), wo(this, "gl", void 0), wo(this, "timeline", void 0), wo(this, "transitions", void 0), wo(this, "needsRedraw", void 0), wo(this, "numInstances", void 0), this.id = e, this.gl = t, this.timeline = n, this.transitions = {}, this.needsRedraw = !1, this.numInstances = 1, this.isSupported = Qv.isSupported(t)
                 }
                 finalize() {
                     for (const t in this.transitions) this._removeTransition(t)
                 }
                 update({
                     attributes: t,
                     transitions: e,
@@ -21008,31 +21011,31 @@
                 }
                 _updateAttribute(t, e, n) {
                     const i = this.transitions[t];
                     let r = !i || i.type !== n.type;
                     if (r) {
                         if (!this.isSupported) return void na.warn("WebGL2 not supported by this browser. Transition for ".concat(t, " is disabled."))();
                         i && this._removeTransition(t);
-                        const s = Qv[n.type];
+                        const s = Jv[n.type];
                         s ? this.transitions[t] = new s({
                             attribute: e,
                             timeline: this.timeline,
                             gl: this.gl
                         }) : (na.error("unsupported transition type '".concat(n.type, "'"))(), r = !1)
                     }(r || e.needsRedraw()) && (this.needsRedraw = !0, this.transitions[t].start(n, this.numInstances))
                 }
             }
-            const $v = "attributeManager.invalidate";
-            class tb {
+            const tb = "attributeManager.invalidate";
+            class eb {
                 constructor(t, {
                     id: e = "attribute-manager",
                     stats: n,
                     timeline: i
                 } = {}) {
-                    wo(this, "id", void 0), wo(this, "gl", void 0), wo(this, "attributes", void 0), wo(this, "updateTriggers", void 0), wo(this, "needsRedraw", void 0), wo(this, "userData", void 0), wo(this, "stats", void 0), wo(this, "attributeTransitionManager", void 0), wo(this, "mergeBoundsMemoized", uf(Bc)), this.id = e, this.gl = t, this.attributes = {}, this.updateTriggers = {}, this.needsRedraw = !0, this.userData = {}, this.stats = n, this.attributeTransitionManager = new Jv(t, {
+                    wo(this, "id", void 0), wo(this, "gl", void 0), wo(this, "attributes", void 0), wo(this, "updateTriggers", void 0), wo(this, "needsRedraw", void 0), wo(this, "userData", void 0), wo(this, "stats", void 0), wo(this, "attributeTransitionManager", void 0), wo(this, "mergeBoundsMemoized", df(Bc)), this.id = e, this.gl = t, this.attributes = {}, this.updateTriggers = {}, this.needsRedraw = !0, this.userData = {}, this.stats = n, this.attributeTransitionManager = new $v(t, {
                         id: "".concat(e, "-transitions"),
                         timeline: i
                     }), Object.seal(this)
                 }
                 finalize() {
                     for (const t in this.attributes) this.attributes[t].delete();
                     this.attributeTransitionManager.finalize()
@@ -21055,19 +21058,19 @@
                     })
                 }
                 remove(t) {
                     for (const e of t) void 0 !== this.attributes[e] && (this.attributes[e].delete(), delete this.attributes[e])
                 }
                 invalidate(t, e) {
                     const n = this._invalidateTrigger(t, e);
-                    sa($v, this, t, n)
+                    sa(tb, this, t, n)
                 }
                 invalidateAll(t) {
                     for (const e in this.attributes) this.attributes[e].setNeedsUpdate(e, t);
-                    sa($v, this, "all")
+                    sa(tb, this, "all")
                 }
                 update({
                     data: t,
                     numInstances: e,
                     startIndices: n = null,
                     transitions: i,
                     props: r = {},
@@ -21140,15 +21143,15 @@
                 _createAttribute(t, e, n) {
                     const i = {
                         ...e,
                         id: t,
                         size: (e.isIndexed ? 1 : e.size) || 1,
                         divisor: n.instanced ? 1 : e.divisor || 0
                     };
-                    return new _v(this.gl, i)
+                    return new xv(this.gl, i)
                 }
                 _mapUpdateTriggersToAttributes() {
                     const t = {};
                     for (const e in this.attributes) this.attributes[e].getUpdateTriggers().forEach((n => {
                         t[n] || (t[n] = []), t[n].push(e)
                     }));
                     this.updateTriggers = t
@@ -21167,34 +21170,34 @@
                     const {
                         attribute: e,
                         numInstances: n
                     } = t;
                     sa("attribute.updateStart", e), e.constant ? e.setConstantValue(e.value) : (e.allocate(n) && sa("attribute.allocate", e, n), e.updateBuffer(t) && (this.needsRedraw = !0, sa("attribute.updateEnd", e, n)))
                 }
             }
-            const eb = 1e-5;
+            const nb = 1e-5;
 
-            function nb(t, e, n, i, r) {
+            function ib(t, e, n, i, r) {
                 const s = e - t;
                 return (n - e) * r + -s * i + s + e
             }
 
-            function ib(t, e) {
+            function rb(t, e) {
                 if (Array.isArray(t)) {
                     let n = 0;
                     for (let i = 0; i < t.length; i++) {
                         const r = t[i] - e[i];
                         n += r * r
                     }
                     return Math.sqrt(n)
                 }
                 return Math.abs(t - e)
             }
-            const rb = {
-                interpolation: class extends If {
+            const sb = {
+                interpolation: class extends kf {
                     get value() {
                         return this._value
                     }
                     _onUpdate() {
                         const {
                             time: t,
                             settings: {
@@ -21203,15 +21206,15 @@
                                 duration: i,
                                 easing: r
                             }
                         } = this, s = r(t / i);
                         this._value = hc(e, n, s)
                     }
                 },
-                spring: class extends If {
+                spring: class extends kf {
                     get value() {
                         return this._currValue
                     }
                     _onUpdate() {
                         const {
                             fromValue: t,
                             toValue: e,
@@ -21220,26 +21223,26 @@
                         } = this.settings, {
                             _prevValue: r = t,
                             _currValue: s = t
                         } = this;
                         let o = function(t, e, n, i, r) {
                             if (Array.isArray(n)) {
                                 const s = [];
-                                for (let o = 0; o < n.length; o++) s[o] = nb(t[o], e[o], n[o], i, r);
+                                for (let o = 0; o < n.length; o++) s[o] = ib(t[o], e[o], n[o], i, r);
                                 return s
                             }
-                            return nb(t, e, n, i, r)
+                            return ib(t, e, n, i, r)
                         }(r, s, e, n, i);
-                        const a = ib(o, e),
-                            l = ib(o, s);
-                        a < eb && l < eb && (o = e, this.end()), this._prevValue = s, this._currValue = o
+                        const a = rb(o, e),
+                            l = rb(o, s);
+                        a < nb && l < nb && (o = e, this.end()), this._prevValue = s, this._currValue = o
                     }
                 }
             };
-            class sb {
+            class ob {
                 constructor(t) {
                     this.transitions = new Map, this.timeline = t
                 }
                 get active() {
                     return this.transitions.size > 0
                 }
                 add(t, e, n, i) {
@@ -21249,16 +21252,16 @@
                     if (r.has(t)) {
                         const n = r.get(t),
                             {
                                 value: i = n.settings.fromValue
                             } = n;
                         e = i, this.remove(t)
                     }
-                    if (!(i = fv(i))) return;
-                    const s = rb[i.type];
+                    if (!(i = gv(i))) return;
+                    const s = sb[i.type];
                     if (!s) return void na.error("unsupported transition type '".concat(i.type, "'"))();
                     const o = new s(this.timeline);
                     o.start({
                         ...i,
                         fromValue: e,
                         toValue: n
                     }), r.set(t, o)
@@ -21275,83 +21278,83 @@
                     return t
                 }
                 clear() {
                     for (const t of this.transitions.keys()) this.remove(t)
                 }
             }
 
-            function ob(t, e) {
+            function ab(t, e) {
                 if (!t.transitions) return !1;
                 const n = {},
                     i = t[To];
                 let r = !1;
                 for (const s in t.transitions) {
                     const o = i[s],
                         a = o && o.type;
-                    ("number" === a || "color" === a || "array" === a) && lb(t[s], e[s], o) && (n[s] = !0, r = !0)
+                    ("number" === a || "color" === a || "array" === a) && cb(t[s], e[s], o) && (n[s] = !0, r = !0)
                 }
                 return !!r && n
             }
 
-            function ab({
+            function lb({
                 newProps: t,
                 oldProps: e,
                 ignoreProps: n = {},
                 propTypes: i = {},
                 triggerName: r = "props"
             }) {
                 if (e === t) return !1;
                 if ("object" != typeof t || null === t) return "".concat(r, " changed shallowly");
                 if ("object" != typeof e || null === e) return "".concat(r, " changed shallowly");
                 for (const s of Object.keys(t))
                     if (!(s in n)) {
                         if (!(s in e)) return "".concat(r, ".").concat(s, " added");
-                        const n = lb(t[s], e[s], i[s]);
+                        const n = cb(t[s], e[s], i[s]);
                         if (n) return "".concat(r, ".").concat(s, " ").concat(n)
                     } for (const s of Object.keys(e))
                     if (!(s in n)) {
                         if (!(s in t)) return "".concat(r, ".").concat(s, " dropped");
                         if (!Object.hasOwnProperty.call(t, s)) {
-                            const n = lb(t[s], e[s], i[s]);
+                            const n = cb(t[s], e[s], i[s]);
                             if (n) return "".concat(r, ".").concat(s, " ").concat(n)
                         }
                     } return !1
             }
 
-            function lb(t, e, n) {
+            function cb(t, e, n) {
                 let i = n && n.equal;
                 return i && !i(t, e, n) ? "changed deeply" : i || (i = t && e && t.equals, !i || i.call(t, e)) ? i || e === t ? null : "changed shallowly" : "changed deeply"
             }
 
-            function cb(t, e) {
+            function hb(t, e) {
                 if (null === e) return !0;
                 const n = e.extensions,
                     {
                         extensions: i
                     } = t;
                 if (i === n) return !1;
                 if (!n || !i) return !0;
                 if (i.length !== n.length) return !0;
                 for (let t = 0; t < i.length; t++)
                     if (!i[t].equals(n[t])) return !0;
                 return !1
             }
 
-            function hb(t, e, n) {
+            function ub(t, e, n) {
                 let i = t.updateTriggers[n];
                 i = null == i ? {} : i;
                 let r = e.updateTriggers[n];
-                return r = null == r ? {} : r, ab({
+                return r = null == r ? {} : r, lb({
                     oldProps: r,
                     newProps: i,
                     triggerName: n
                 })
             }
 
-            function ub(t, e) {
+            function db(t, e) {
                 if (!e) return t;
                 const n = {
                     ...t,
                     ...e
                 };
                 if ("defines" in e && (n.defines = {
                         ...t.defines,
@@ -21366,87 +21369,87 @@
                             ...t.inject
                         };
                         for (const t in e.inject) i[t] = (i[t] || "") + e.inject[t];
                         n.inject = i
                     } else n.inject = e.inject;
                 return n
             }
-            const db = [0, 0, 0];
+            const pb = [0, 0, 0];
 
-            function pb(t, e, n = !1) {
+            function fb(t, e, n = !1) {
                 const i = e.projectPosition(t);
-                if (n && e instanceof Rf) {
+                if (n && e instanceof If) {
                     const [n, r, s = 0] = t, o = e.getDistanceScales([n, r]);
                     i[2] = s * o.unitsPerMeter[2]
                 }
                 return i
             }
 
-            function fb(t, {
+            function gb(t, {
                 viewport: e,
                 modelMatrix: n,
                 coordinateSystem: i,
                 coordinateOrigin: r,
                 offsetMode: s
             }) {
                 let [o, a, l = 0] = t;
                 switch (n && ([o, a, l] = Qc([], [o, a, l, 1], n)), i) {
                     case Lh.LNGLAT:
-                        return pb([o, a, l], e, s);
+                        return fb([o, a, l], e, s);
                     case Lh.LNGLAT_OFFSETS:
-                        return pb([o + r[0], a + r[1], l + (r[2] || 0)], e, s);
+                        return fb([o + r[0], a + r[1], l + (r[2] || 0)], e, s);
                     case Lh.METER_OFFSETS:
-                        return pb(Ph(r, [o, a, l]), e, s);
+                        return fb(Ph(r, [o, a, l]), e, s);
                     case Lh.CARTESIAN:
                     default:
                         return e.isGeospatial ? [o + r[0], a + r[1], l + r[2]] : e.projectPosition([o, a, l])
                 }
             }
-            const gb = {
+            const mb = {
                     10241: 9987,
                     10240: 9729,
                     10242: 33071,
                     10243: 33071
                 },
-                mb = {},
-                vb = {
+                vb = {},
+                bb = {
                     boolean: {
                         validate: (t, e) => !0,
                         equal: (t, e, n) => Boolean(t) === Boolean(e)
                     },
                     number: {
                         validate: (t, e) => Number.isFinite(t) && (!("max" in e) || t <= e.max) && (!("min" in e) || t >= e.min)
                     },
                     color: {
-                        validate: (t, e) => e.optional && !t || _b(t) && (3 === t.length || 4 === t.length),
-                        equal: (t, e, n) => Sf(t, e, 1)
+                        validate: (t, e) => e.optional && !t || xb(t) && (3 === t.length || 4 === t.length),
+                        equal: (t, e, n) => Cf(t, e, 1)
                     },
                     accessor: {
                         validate(t, e) {
-                            const n = xb(t);
-                            return "function" === n || n === xb(e.value)
+                            const n = wb(t);
+                            return "function" === n || n === wb(e.value)
                         },
-                        equal: (t, e, n) => "function" == typeof e || Sf(t, e, 1)
+                        equal: (t, e, n) => "function" == typeof e || Cf(t, e, 1)
                     },
                     array: {
-                        validate: (t, e) => e.optional && !t || _b(t),
+                        validate: (t, e) => e.optional && !t || xb(t),
                         equal(t, e, n) {
                             const {
                                 compare: i
                             } = n, r = Number.isInteger(i) ? i : i ? 1 : 0;
-                            return i ? Sf(t, e, r) : t === e
+                            return i ? Cf(t, e, r) : t === e
                         }
                     },
                     object: {
                         equal(t, e, n) {
                             if (n.ignore) return !0;
                             const {
                                 compare: i
                             } = n, r = Number.isInteger(i) ? i : i ? 1 : 0;
-                            return i ? Sf(t, e, r) : t === e
+                            return i ? Cf(t, e, r) : t === e
                         }
                     },
                     function: {
                         validate: (t, e) => e.optional && !t || "function" == typeof t,
                         equal: (t, e, n) => !n.compare && !1 !== n.ignore || t === e
                     },
                     data: {
@@ -21457,133 +21460,133 @@
                             return i && t ? i(t) : t
                         }
                     },
                     image: {
                         transform: (t, e, n) => {
                             const i = n.context;
                             return i && i.gl ? function(t, e, n, i) {
-                                if (n instanceof Qd) return n;
+                                if (n instanceof Jd) return n;
                                 n.constructor && "Object" !== n.constructor.name && (n = {
                                     data: n
                                 });
                                 let r = null;
                                 n.compressed && (r = {
                                     10241: n.data.length > 1 ? 9985 : 9729
                                 });
-                                const s = new Qd(e, {
+                                const s = new Jd(e, {
                                     ...n,
                                     parameters: {
-                                        ...gb,
+                                        ...mb,
                                         ...r,
                                         ...i
                                     }
                                 });
-                                return mb[s.id] = t, s
+                                return vb[s.id] = t, s
                             }(n.id, i.gl, t, {
                                 ...e.parameters,
                                 ...n.props.textureParameters
                             }) : null
                         },
                         release: (t, e, n) => {
                             var i, r;
-                            i = n.id, (r = t) && r instanceof Qd && mb[r.id] === i && (r.delete(), delete mb[r.id])
+                            i = n.id, (r = t) && r instanceof Jd && vb[r.id] === i && (r.delete(), delete vb[r.id])
                         }
                     }
                 };
 
-            function bb(t, e) {
-                switch (xb(e)) {
+            function yb(t, e) {
+                switch (wb(e)) {
                     case "object":
-                        return yb(t, e);
+                        return _b(t, e);
                     case "array":
-                        return yb(t, {
+                        return _b(t, {
                             type: "array",
                             value: e,
                             compare: !1
                         });
                     case "boolean":
-                        return yb(t, {
+                        return _b(t, {
                             type: "boolean",
                             value: e
                         });
                     case "number":
-                        return yb(t, {
+                        return _b(t, {
                             type: "number",
                             value: e
                         });
                     case "function":
-                        return yb(t, {
+                        return _b(t, {
                             type: "function",
                             value: e,
                             compare: !0
                         });
                     default:
                         return {
                             name: t, type: "unknown", value: e
                         }
                 }
             }
 
-            function yb(t, e) {
+            function _b(t, e) {
                 return "type" in e ? {
                     name: t,
-                    ...vb[e.type],
+                    ...bb[e.type],
                     ...e
                 } : "value" in e ? {
                     name: t,
-                    type: xb(e.value),
+                    type: wb(e.value),
                     ...e
                 } : {
                     name: t,
                     type: "object",
                     value: e
                 }
             }
 
-            function _b(t) {
+            function xb(t) {
                 return Array.isArray(t) || ArrayBuffer.isView(t)
             }
 
-            function xb(t) {
-                return _b(t) ? "array" : null === t ? "null" : typeof t
+            function wb(t) {
+                return xb(t) ? "array" : null === t ? "null" : typeof t
             }
 
-            function wb(t, e) {
+            function Eb(t, e) {
                 let n = "_mergedDefaultProps";
                 if (e)
                     for (const t of e) {
                         const e = t.constructor;
                         e && (n += ":".concat(e.extensionName || e.name))
                     }
-                return Sb(t, n) || (t[n] = function(t, e) {
+                return Cb(t, n) || (t[n] = function(t, e) {
                     if (!t.prototype) return null;
-                    const n = wb(Object.getPrototypeOf(t)),
+                    const n = Eb(Object.getPrototypeOf(t)),
                         i = function(t) {
                             const e = {},
                                 n = {},
                                 i = {};
                             for (const [r, s] of Object.entries(t)) {
                                 const t = null == s ? void 0 : s.deprecatedFor;
                                 if (t) i[r] = Array.isArray(t) ? t : [t];
                                 else {
-                                    const t = bb(r, s);
+                                    const t = yb(r, s);
                                     e[r] = t, n[r] = t.value
                                 }
                             }
                             return {
                                 propTypes: e,
                                 defaultProps: n,
                                 deprecatedProps: i
                             }
-                        }(Sb(t, "defaultProps") || {}),
+                        }(Cb(t, "defaultProps") || {}),
                         r = Object.assign(Object.create(null), n, i.defaultProps),
                         s = Object.assign(Object.create(null), null == n ? void 0 : n[To], i.propTypes),
                         o = Object.assign(Object.create(null), null == n ? void 0 : n[Ao], i.deprecatedProps);
                     for (const t of e) {
-                        const e = wb(t.constructor);
+                        const e = Eb(t.constructor);
                         e && (Object.assign(r, e), Object.assign(s, e[To]), Object.assign(o, e[Ao]))
                     }
                     return function(t, e) {
                             const n = function(t) {
                                 const e = t.componentName;
                                 return e || na.warn("".concat(t.name, ".componentName not specified"))(), e || t.name
                             }(e);
@@ -21599,103 +21602,103 @@
                                 i = {};
                             for (const t in e) {
                                 const r = e[t],
                                     {
                                         name: s,
                                         value: o
                                     } = r;
-                                r.async && (n[s] = o, i[s] = Eb(s))
+                                r.async && (n[s] = o, i[s] = Pb(s))
                             }
                             t[Mo] = n, t[Oo] = {}, Object.defineProperties(t, i)
                         }(r, s),
                         function(t, e) {
                             for (const n in e) Object.defineProperty(t, n, {
                                 enumerable: !1,
                                 set(t) {
                                     const i = "".concat(this.id, ": ").concat(n);
-                                    for (const i of e[n]) Pb(this, i) || (this[i] = t);
+                                    for (const i of e[n]) Sb(this, i) || (this[i] = t);
                                     na.deprecated(i, e[n].join("/"))()
                                 }
                             })
-                        }(r, o), r[To] = s, r[Ao] = o, 0 !== e.length || Pb(t, "_propTypes") || (t._propTypes = s), r
+                        }(r, o), r[To] = s, r[Ao] = o, 0 !== e.length || Sb(t, "_propTypes") || (t._propTypes = s), r
                 }(t, e || []))
             }
 
-            function Eb(t) {
+            function Pb(t) {
                 return {
                     enumerable: !0,
                     set(e) {
-                        "string" == typeof e || e instanceof Promise || lv(e) ? this[Oo][t] = e : this[Lo][t] = e
+                        "string" == typeof e || e instanceof Promise || cv(e) ? this[Oo][t] = e : this[Lo][t] = e
                     },
                     get() {
                         if (this[Lo]) {
                             if (t in this[Lo]) return this[Lo][t] || this[Mo][t];
                             if (t in this[Oo]) {
                                 const e = this[Co] && this[Co].internalState;
                                 if (e && e.hasAsyncProp(t)) return e.getAsyncProp(t) || this[Mo][t]
                             }
                         }
                         return this[Mo][t]
                     }
                 }
             }
 
-            function Pb(t, e) {
+            function Sb(t, e) {
                 return Object.prototype.hasOwnProperty.call(t, e)
             }
 
-            function Sb(t, e) {
-                return Pb(t, e) && t[e]
+            function Cb(t, e) {
+                return Sb(t, e) && t[e]
             }
-            let Cb = 0;
-            class Tb {
+            let Tb = 0;
+            class Ab {
                 constructor(...t) {
                     wo(this, "id", void 0), wo(this, "props", void 0), wo(this, "count", void 0), this.props = function(t, e) {
                         let n;
                         for (let t = e.length - 1; t >= 0; t--) {
                             const i = e[t];
                             "extensions" in i && (n = i.extensions)
                         }
-                        const i = wb(t.constructor, n),
+                        const i = Eb(t.constructor, n),
                             r = Object.create(i);
                         r[Co] = t, r[Oo] = {}, r[Lo] = {};
                         for (let t = 0; t < e.length; ++t) {
                             const n = e[t];
                             for (const t in n) r[t] = n[t]
                         }
                         return Object.freeze(r), r
-                    }(this, t), this.id = this.props.id, this.count = Cb++
+                    }(this, t), this.id = this.props.id, this.count = Tb++
                 }
                 clone(t) {
                     const {
                         props: e
                     } = this, n = {};
                     for (const t in e[Mo]) t in e[Lo] ? n[t] = e[Lo][t] : t in e[Oo] && (n[t] = e[Oo][t]);
                     return new this.constructor({
                         ...e,
                         ...n,
                         ...t
                     })
                 }
             }
-            wo(Tb, "componentName", "Component"), wo(Tb, "defaultProps", {});
-            const Ab = Object.freeze({});
-            class Mb {
+            wo(Ab, "componentName", "Component"), wo(Ab, "defaultProps", {});
+            const Mb = Object.freeze({});
+            class Ob {
                 constructor(t) {
                     wo(this, "component", void 0), wo(this, "onAsyncPropUpdated", void 0), wo(this, "asyncProps", void 0), wo(this, "oldProps", void 0), wo(this, "oldAsyncProps", void 0), this.component = t, this.asyncProps = {}, this.onAsyncPropUpdated = () => {}, this.oldProps = null, this.oldAsyncProps = null
                 }
                 finalize() {
                     for (const t in this.asyncProps) {
                         const e = this.asyncProps[t];
                         e && e.type && e.type.release && e.type.release(e.resolvedValue, e.type, this.component)
                     }
                     this.asyncProps = {}, this.component = null, this.resetOldProps()
                 }
                 getOldProps() {
-                    return this.oldAsyncProps || this.oldProps || Ab
+                    return this.oldAsyncProps || this.oldProps || Mb
                 }
                 resetOldProps() {
                     this.oldAsyncProps = null, this.oldProps = this.component ? this.component.props : null
                 }
                 hasAsyncProp(t) {
                     return t in this.asyncProps
                 }
@@ -21731,15 +21734,15 @@
                 }
                 _fetch(t, e) {
                     return null
                 }
                 _onResolve(t, e) {}
                 _onError(t, e) {}
                 _updateAsyncProp(t, e) {
-                    this._didAsyncInputValueChange(t, e) && ("string" == typeof e && (e = this._fetch(t, e)), e instanceof Promise ? this._watchPromise(t, e) : lv(e) ? this._resolveAsyncIterable(t, e) : this._setPropValue(t, e))
+                    this._didAsyncInputValueChange(t, e) && ("string" == typeof e && (e = this._fetch(t, e)), e instanceof Promise ? this._watchPromise(t, e) : cv(e) ? this._resolveAsyncIterable(t, e) : this._setPropValue(t, e))
                 }
                 _freezeAsyncOldProps() {
                     if (!this.oldAsyncProps && this.oldProps) {
                         this.oldAsyncProps = Object.create(this.oldProps);
                         for (const t in this.asyncProps) Object.defineProperty(this.oldAsyncProps, t, {
                             enumerable: !0,
                             value: this.oldProps[t]
@@ -21807,15 +21810,15 @@
                             resolvedValue: e,
                             pendingLoadCount: 0,
                             resolvedLoadCount: 0
                         }
                     }
                 }
             }
-            class Ob extends Mb {
+            class Lb extends Ob {
                 constructor({
                     attributeManager: t,
                     layer: e
                 }) {
                     super(e), wo(this, "attributeManager", void 0), wo(this, "needsRedraw", void 0), wo(this, "needsUpdate", void 0), wo(this, "subLayers", void 0), wo(this, "usesPickingColorCache", void 0), wo(this, "hasPickingBuffer", void 0), wo(this, "changeFlags", void 0), wo(this, "viewport", void 0), wo(this, "uniformTransitions", void 0), wo(this, "propsInTransition", void 0), this.attributeManager = t, this.needsRedraw = !0, this.needsUpdate = !0, this.subLayers = null, this.usesPickingColorCache = !1
                 }
                 get layer() {
@@ -21840,25 +21843,25 @@
                     }
                 }
                 _onError(t, e) {
                     const n = this.layer;
                     n && n.raiseError(e, "loading ".concat(t, " of ").concat(this.layer))
                 }
             }
-            const Lb = 2 ** 24 - 1,
-                Rb = Object.freeze([]),
-                Ib = uf((({
+            const Rb = 2 ** 24 - 1,
+                Ib = Object.freeze([]),
+                kb = df((({
                     oldViewport: t,
                     viewport: e
                 }) => t.equals(e)));
-            let kb = new Uint8ClampedArray(0);
-            const jb = {
+            let jb = new Uint8ClampedArray(0);
+            const Fb = {
                 data: {
                     type: "data",
-                    value: Rb,
+                    value: Ib,
                     async: !0
                 },
                 dataComparator: {
                     type: "function",
                     value: null,
                     optional: !0
                 },
@@ -21997,15 +22000,15 @@
                 highlightedObjectIndex: null,
                 autoHighlight: !1,
                 highlightColor: {
                     type: "accessor",
                     value: [0, 0, 128, 128]
                 }
             };
-            class Fb extends Tb {
+            class zb extends Ab {
                 constructor(...t) {
                     super(...t), wo(this, "internalState", null), wo(this, "lifecycle", "Awaiting state"), wo(this, "context", void 0), wo(this, "state", void 0), wo(this, "parent", null)
                 }
                 static get componentName() {
                     return Object.prototype.hasOwnProperty.call(this, "layerName") ? this.layerName : ""
                 }
                 get root() {
@@ -22014,30 +22017,30 @@
                     return t
                 }
                 toString() {
                     const t = this.constructor.layerName || this.constructor.name;
                     return "".concat(t, "({id: '").concat(this.props.id, "'})")
                 }
                 project(t) {
-                    Of(this.internalState);
+                    Lf(this.internalState);
                     const e = this.internalState.viewport || this.context.viewport,
-                        n = fb(t, {
+                        n = gb(t, {
                             viewport: e,
                             modelMatrix: this.props.modelMatrix,
                             coordinateOrigin: this.props.coordinateOrigin,
                             coordinateSystem: this.props.coordinateSystem
                         }),
                         [i, r, s] = Th(n, e.pixelProjectionMatrix);
                     return 2 === t.length ? [i, r] : [i, r, s]
                 }
                 unproject(t) {
-                    return Of(this.internalState), (this.internalState.viewport || this.context.viewport).unproject(t)
+                    return Lf(this.internalState), (this.internalState.viewport || this.context.viewport).unproject(t)
                 }
                 projectPosition(t, e) {
-                    return Of(this.internalState),
+                    return Lf(this.internalState),
                         function(t, e) {
                             const {
                                 viewport: n,
                                 coordinateSystem: i,
                                 coordinateOrigin: r,
                                 modelMatrix: s,
                                 fromCoordinateSystem: o,
@@ -22060,18 +22063,18 @@
                                     modelMatrix: n,
                                     fromCoordinateSystem: s,
                                     fromCoordinateOrigin: o
                                 }
                             }(e), {
                                 autoOffset: l = !0
                             } = e, {
-                                geospatialOrigin: c = db,
-                                shaderCoordinateOrigin: h = db,
+                                geospatialOrigin: c = pb,
+                                shaderCoordinateOrigin: h = pb,
                                 offsetMode: u = !1
-                            } = l ? bf(n, i, r) : {}, d = fb(t, {
+                            } = l ? yf(n, i, r) : {}, d = gb(t, {
                                 viewport: n,
                                 modelMatrix: s,
                                 coordinateSystem: o,
                                 coordinateOrigin: a,
                                 offsetMode: u
                             });
                             if (u) {
@@ -22140,15 +22143,15 @@
                 nullPickingColor() {
                     return [0, 0, 0]
                 }
                 encodePickingColor(t, e = []) {
                     return e[0] = t + 1 & 255, e[1] = t + 1 >> 8 & 255, e[2] = t + 1 >> 8 >> 8 & 255, e
                 }
                 decodePickingColor(t) {
-                    Of(t instanceof Uint8Array);
+                    Lf(t instanceof Uint8Array);
                     const [e, n, i] = t;
                     return e + 256 * n + 65536 * i - 1
                 }
                 getNumInstances() {
                     return Number.isFinite(this.props.numInstances) ? this.props.numInstances : this.state && void 0 !== this.state.numInstances ? this.state.numInstances : function(t) {
                         if (null === (e = t) || "object" != typeof e) throw new Error("count(): argument not an object");
                         var e;
@@ -22165,15 +22168,15 @@
                     return this.props.startIndices ? this.props.startIndices : this.state && this.state.startIndices ? this.state.startIndices : null
                 }
                 getBounds() {
                     var t;
                     return null === (t = this.getAttributeManager()) || void 0 === t ? void 0 : t.getBounds(["positions", "instancePositions"])
                 }
                 getShaders(t) {
-                    for (const e of this.props.extensions) t = ub(t, e.getShaders.call(this, e));
+                    for (const e of this.props.extensions) t = db(t, e.getShaders.call(this, e));
                     return t
                 }
                 shouldUpdateState(t) {
                     return t.changeFlags.propsOrDataChanged
                 }
                 updateState(t) {
                     const e = this.getAttributeManager(),
@@ -22233,15 +22236,15 @@
                 hasUniformTransition() {
                     var t;
                     return (null === (t = this.internalState) || void 0 === t ? void 0 : t.uniformTransitions.active) || !1
                 }
                 activateViewport(t) {
                     if (!this.internalState) return;
                     const e = this.internalState.viewport;
-                    this.internalState.viewport = t, e && Ib({
+                    this.internalState.viewport = t, e && kb({
                         oldViewport: e,
                         viewport: t
                     }) || (this.setChangeFlags({
                         viewportChanged: !0
                     }), this.isComposite ? this.needsUpdate() && this.setNeedsUpdate() : this._update())
                 }
                 invalidateAttribute(t = "all") {
@@ -22289,26 +22292,26 @@
                     }
                     return this.props
                 }
                 calculateInstancePickingColors(t, {
                     numInstances: e
                 }) {
                     if (t.constant) return;
-                    const n = Math.floor(kb.length / 3);
+                    const n = Math.floor(jb.length / 3);
                     if (this.internalState.usesPickingColorCache = !0, n < e) {
-                        e > Lb && na.warn("Layer has too many data objects. Picking might not be able to distinguish all objects.")(), kb = sc.allocate(kb, e, {
+                        e > Rb && na.warn("Layer has too many data objects. Picking might not be able to distinguish all objects.")(), jb = sc.allocate(jb, e, {
                             size: 3,
                             copy: !0,
-                            maxCount: Math.max(e, Lb)
+                            maxCount: Math.max(e, Rb)
                         });
-                        const t = Math.floor(kb.length / 3),
+                        const t = Math.floor(jb.length / 3),
                             i = [];
-                        for (let e = n; e < t; e++) this.encodePickingColor(e, i), kb[3 * e + 0] = i[0], kb[3 * e + 1] = i[1], kb[3 * e + 2] = i[2]
+                        for (let e = n; e < t; e++) this.encodePickingColor(e, i), jb[3 * e + 0] = i[0], jb[3 * e + 1] = i[1], jb[3 * e + 2] = i[2]
                     }
-                    t.value = kb.subarray(0, 3 * e)
+                    t.value = jb.subarray(0, 3 * e)
                 }
                 _setModelAttributes(t, e) {
                     const n = this.getAttributeManager(),
                         i = t.userData.excludeAttributes || {},
                         r = n.getShaderAttributes(e, i);
                     t.setAttributes(r)
                 }
@@ -22342,34 +22345,34 @@
                     })
                 }
                 restorePickingColors() {
                     const {
                         pickingColors: t,
                         instancePickingColors: e
                     } = this.getAttributeManager().attributes, n = t || e;
-                    n && (this.internalState.usesPickingColorCache && n.value.buffer !== kb.buffer && (n.value = kb.subarray(0, n.value.length)), n.updateSubBuffer({
+                    n && (this.internalState.usesPickingColorCache && n.value.buffer !== jb.buffer && (n.value = jb.subarray(0, n.value.length)), n.updateSubBuffer({
                         startOffset: 0
                     }))
                 }
                 _initialize() {
-                    Of(!this.internalState), Of(Number.isFinite(this.props.coordinateSystem)), sa("layer.initialize", this);
+                    Lf(!this.internalState), Lf(Number.isFinite(this.props.coordinateSystem)), sa("layer.initialize", this);
                     const t = this._getAttributeManager();
                     t && t.addInstanced({
                         instancePickingColors: {
                             type: 5121,
                             size: 3,
                             noAlloc: !0,
                             update: this.calculateInstancePickingColors
                         }
-                    }), this.internalState = new Ob({
+                    }), this.internalState = new Lb({
                         attributeManager: t,
                         layer: this
                     }), this._clearChangeFlags(), this.state = {}, Object.defineProperty(this.state, "attributeManager", {
                         get: () => (na.deprecated("layer.state.attributeManager", "layer.getAttributeManager()")(), t)
-                    }), this.internalState.uniformTransitions = new sb(this.context.timeline), this.internalState.onAsyncPropUpdated = this._onAsyncPropUpdated.bind(this), this.internalState.setAsyncProps(this.props), this.initializeState(this.context);
+                    }), this.internalState.uniformTransitions = new ob(this.context.timeline), this.internalState.onAsyncPropUpdated = this._onAsyncPropUpdated.bind(this), this.internalState.setAsyncProps(this.props), this.initializeState(this.context);
                     for (const t of this.props.extensions) t.initializeState.call(this, this.context, t);
                     this.setChangeFlags({
                         dataChanged: "init",
                         propsChanged: "init",
                         viewportChanged: !0,
                         extensionsChanged: !0
                     }), this._update()
@@ -22472,15 +22475,15 @@
                         extensionsChanged: !1,
                         propsOrDataChanged: !1,
                         somethingChanged: !1
                     }
                 }
                 _diffProps(t, e) {
                     const n = function(t, e) {
-                        const n = ab({
+                        const n = lb({
                                 newProps: t,
                                 oldProps: e,
                                 propTypes: t[To],
                                 ignoreProps: {
                                     data: null,
                                     updateTriggers: null,
                                     extensions: null,
@@ -22497,27 +22500,27 @@
                                 return i ? i(t.data, e.data) || (n = "Data comparator detected a change") : t.data !== e.data && (n = "A new data container was supplied"), n && r && (n = r(t.data, e.data) || n), n
                             }(t, e);
                         let r = !1;
                         return i || (r = function(t, e) {
                             if (null === e) return {
                                 all: !0
                             };
-                            if ("all" in t.updateTriggers && hb(t, e, "all")) return {
+                            if ("all" in t.updateTriggers && ub(t, e, "all")) return {
                                 all: !0
                             };
                             const n = {};
                             let i = !1;
-                            for (const r in t.updateTriggers) "all" !== r && hb(t, e, r) && (n[r] = !0, i = !0);
+                            for (const r in t.updateTriggers) "all" !== r && ub(t, e, r) && (n[r] = !0, i = !0);
                             return !!i && n
                         }(t, e)), {
                             dataChanged: i,
                             propsChanged: n,
                             updateTriggersChanged: r,
-                            extensionsChanged: cb(t, e),
-                            transitionsChanged: ob(t, e)
+                            extensionsChanged: hb(t, e),
+                            transitionsChanged: ab(t, e)
                         }
                     }(t, e);
                     if (n.updateTriggersChanged)
                         for (const t in n.updateTriggersChanged) n.updateTriggersChanged[t] && this.invalidateAttribute(t);
                     if (n.transitionsChanged)
                         for (const r in n.transitionsChanged) {
                             var i;
@@ -22547,15 +22550,15 @@
                         {
                             highlightColor: n
                         } = this.props;
                     t.picked && "function" == typeof n && (e.pickingHighlightColor = n(t)), this.setModuleParameters(e), this.setNeedsRedraw()
                 }
                 _getAttributeManager() {
                     const t = this.context;
-                    return new tb(t.gl, {
+                    return new eb(t.gl, {
                         id: this.props.id,
                         stats: t.stats,
                         timeline: t.timeline
                     })
                 }
                 _postUpdate(t, e) {
                     const {
@@ -22595,83 +22598,83 @@
                         for (const t of this.props.extensions) t.onNeedsRedraw.call(this, t);
                     return this.internalState.needsRedraw = this.internalState.needsRedraw && !t.clearRedrawFlags, e
                 }
                 _onAsyncPropUpdated() {
                     this._diffProps(this.props, this.internalState.getOldProps()), this.setNeedsUpdate()
                 }
             }
-            wo(Fb, "defaultProps", jb), wo(Fb, "layerName", "Layer");
-            const zb = {
+            wo(zb, "defaultProps", Fb), wo(zb, "layerName", "Layer");
+            const Bb = {
                 position: "absolute",
                 zIndex: -1
             };
 
-            function Bb(t, e) {
+            function Db(t, e) {
                 if ("function" == typeof t) return t(e);
-                if (Array.isArray(t)) return t.map((t => Bb(t, e)));
-                if (Db(t)) {
+                if (Array.isArray(t)) return t.map((t => Db(t, e)));
+                if (Nb(t)) {
                     if (function(t) {
                             const e = t.type,
                                 n = e && e.defaultProps;
                             return n && n.mapStyle
-                        }(t)) return e.style = zb, (0, c.cloneElement)(t, e);
+                        }(t)) return e.style = Bb, (0, c.cloneElement)(t, e);
                     if (function(t) {
                             const e = t.type;
                             return e && e.deckGLViewProps
                         }(t)) return (0, c.cloneElement)(t, e)
                 }
                 return t
             }
 
-            function Db(t) {
+            function Nb(t) {
                 return t && "object" == typeof t && "type" in t || !1
             }
 
-            function Nb(t) {
-                if ("function" == typeof t) return (0, c.createElement)(Lf, {}, t);
-                if (Array.isArray(t)) return t.map(Nb);
-                if (Db(t)) {
-                    if (t.type === c.Fragment) return Nb(t.props.children);
-                    if (tv(t.type, Lf)) return t
+            function Vb(t) {
+                if ("function" == typeof t) return (0, c.createElement)(Rf, {}, t);
+                if (Array.isArray(t)) return t.map(Vb);
+                if (Nb(t)) {
+                    if (t.type === c.Fragment) return Vb(t.props.children);
+                    if (ev(t.type, Rf)) return t
                 }
                 return t
             }
-            const Vb = {
+            const Ub = {
                 mixBlendMode: null
             };
 
-            function Ub(t) {
+            function Gb(t) {
                 t.redrawReason && (t.deck._drawLayers(t.redrawReason), t.redrawReason = null)
             }
-            const Gb = (0, c.forwardRef)(((t, e) => {
+            const Wb = (0, c.forwardRef)(((t, e) => {
                 const [n, i] = (0, c.useState)(0), r = (0, c.useRef)({
                     control: null,
                     version: n,
                     forceUpdate: () => i((t => t + 1))
                 }).current, s = (0, c.useRef)(null), o = (0, c.useRef)(null), a = (0, c.useMemo)((() => function({
                     children: t,
                     layers: e = [],
                     views: n = null
                 }) {
                     const i = [],
                         r = [],
                         s = {};
-                    return c.Children.forEach(Nb(t), (t => {
-                        if (Db(t)) {
+                    return c.Children.forEach(Vb(t), (t => {
+                        if (Nb(t)) {
                             const e = t.type;
-                            if (tv(e, Fb)) {
+                            if (ev(e, zb)) {
                                 const n = function(t, e) {
                                     const n = {},
                                         i = t.defaultProps || {};
                                     for (const t in e) i[t] !== e[t] && (n[t] = e[t]);
                                     return new t(n)
                                 }(e, t.props);
                                 r.push(n)
                             } else i.push(t);
-                            if (tv(e, Lf) && e !== Lf && t.props.id) {
+                            if (ev(e, Rf) && e !== Rf && t.props.id) {
                                 const n = new e(t.props);
                                 s[n.id] = n
                             }
                         } else t && i.push(t)
                     })), Object.keys(s).length > 0 && (Array.isArray(n) ? n.forEach((t => {
                         s[t.id] = t
                     })) : n && (s[n.id] = n), n = Object.values(s)), {
@@ -22701,35 +22704,35 @@
                             views: a.views,
                             onViewStateChange: h,
                             onInteractionStateChange: u
                         };
                         return delete e._customRender, r.deck && r.deck.setProps(e), e
                     }), [t]);
                 (0, c.useEffect)((() => {
-                    const e = t.Deck || Jm;
+                    const e = t.Deck || $m;
                     return r.deck = function(t, e, n) {
                         const i = new e({
                             ...n,
                             _customRender: e => {
                                 t.redrawReason = e;
                                 const n = i.getViewports();
-                                t.lastRenderedViewports !== n ? t.forceUpdate() : Ub(t)
+                                t.lastRenderedViewports !== n ? t.forceUpdate() : Gb(t)
                             }
                         });
                         return i
                     }(r, e, {
                         ...d,
                         parent: s.current,
                         canvas: o.current
                     }), () => {
                         var t;
                         return null === (t = r.deck) || void 0 === t ? void 0 : t.finalize()
                     }
-                }), []), $m((() => {
-                    Ub(r);
+                }), []), tv((() => {
+                    Gb(r);
                     const {
                         viewStateUpdateRequested: t,
                         interactionStateUpdateRequested: e
                     } = r;
                     t && h(t), e && u(e)
                 })), (0, c.useImperativeHandle)(e, (() => function(t) {
                     return {
@@ -22766,15 +22769,15 @@
                                 height: e
                             },
                             r = {
                                 left: 0,
                                 top: 0
                             };
                         if (n)
-                            for (const t in n) t in Vb ? r[t] = n[t] : i[t] = n[t];
+                            for (const t in n) t in Ub ? r[t] = n[t] : i[t] = n[t];
                         return {
                             containerStyle: i,
                             canvasStyle: r
                         }
                     }({
                         width: g,
                         height: m,
@@ -22792,26 +22795,26 @@
                             } = e || {};
                             if (!i || !i.views.length) return [];
                             const r = {},
                                 s = i.views[0].id;
                             for (const e of t) {
                                 let t = s,
                                     n = e;
-                                Db(e) && tv(e.type, Lf) && (t = e.props.id || s, n = e.props.children);
+                                Nb(e) && ev(e.type, Rf) && (t = e.props.id || s, n = e.props.children);
                                 const o = i.getViewport(t),
                                     a = i.getViewState(t);
                                 if (o) {
                                     a.padding = o.padding;
                                     const {
                                         x: e,
                                         y: i,
                                         width: s,
                                         height: l
                                     } = o;
-                                    n = Bb(n, {
+                                    n = Db(n, {
                                         x: e,
                                         y: i,
                                         width: s,
                                         height: l,
                                         viewport: o,
                                         viewState: a
                                     }), r[t] || (r[t] = {
@@ -22871,21 +22874,21 @@
                         id: "".concat(v || "deckgl", "-wrapper"),
                         ref: s,
                         style: y
                     }, [e, t])
                 }
                 return l = !1, r.control
             }));
-            Gb.defaultProps = Jm.defaultProps;
-            const Wb = Gb,
-                Hb = (new ih).lookAt({
+            Wb.defaultProps = $m.defaultProps;
+            const Hb = Wb,
+                Zb = (new ih).lookAt({
                     eye: [0, 0, 1]
                 });
 
-            function Zb({
+            function qb({
                 width: t,
                 height: e,
                 near: n,
                 far: i,
                 padding: r
             }) {
                 let s = -t / 2,
@@ -22906,15 +22909,15 @@
                     right: o,
                     bottom: a,
                     top: l,
                     near: n,
                     far: i
                 })
             }
-            class qb extends Dh {
+            class Xb extends Dh {
                 constructor(t) {
                     const {
                         width: e,
                         height: n,
                         near: i = .1,
                         far: r = 1e3,
                         zoom: s = 0,
@@ -22931,16 +22934,16 @@
                             metersPerUnit: [d / t, d / e, 1]
                         }
                     }
                     super({
                         ...t,
                         longitude: void 0,
                         position: o,
-                        viewMatrix: Hb.clone().scale([d, d * (l ? -1 : 1), d]),
-                        projectionMatrix: Zb({
+                        viewMatrix: Zb.clone().scale([d, d * (l ? -1 : 1), d]),
+                        projectionMatrix: qb({
                             width: e || 1,
                             height: n || 1,
                             padding: a,
                             near: i,
                             far: r
                         }),
                         zoom: u,
@@ -22964,15 +22967,15 @@
                         i = qc([], this.projectFlat(t), Xc([], n)),
                         r = qc([], this.center, i);
                     return {
                         target: this.unprojectFlat(r)
                     }
                 }
             }
-            class Xb extends Qf {
+            class Yb extends Jf {
                 constructor(t) {
                     const {
                         width: e,
                         height: n,
                         rotationX: i = 0,
                         rotationOrbit: r = 0,
                         target: s = [0, 0, 0],
@@ -23208,15 +23211,15 @@
                     } = t;
                     return t.zoom = Array.isArray(i) ? [cc(i[0], n, e), cc(i[1], n, e)] : cc(i, n, e), t.rotationX = cc(t.rotationX, s, r), (o < -180 || o > 180) && (t.rotationOrbit = function(t, e) {
                         const n = t % 360;
                         return n < 0 ? 360 + n : n
                     }(o + 180) - 180), t
                 }
             }
-            class Yb extends Xb {
+            class Kb extends Yb {
                 constructor(t) {
                     super(t), wo(this, "zoomAxis", void 0), this.zoomAxis = t.zoomAxis || "all"
                 }
                 _calculateNewZoom({
                     scale: t,
                     startZoom: e
                 }) {
@@ -23240,35 +23243,35 @@
                                 e < i && (r += i - e), e = Math.max(t + r, s + r), e > n && (r += n - e), t += r, s += r
                         }
                         return [t, s]
                     }
                     return cc(e + r, i, n)
                 }
             }
-            class Kb extends Kf {
+            class Qb extends Qf {
                 constructor(...t) {
-                    super(...t), wo(this, "ControllerState", Yb), wo(this, "transition", {
+                    super(...t), wo(this, "ControllerState", Kb), wo(this, "transition", {
                         transitionDuration: 300,
-                        transitionInterpolator: new Nf(["target", "zoom"])
+                        transitionInterpolator: new Vf(["target", "zoom"])
                     }), wo(this, "dragMode", "pan")
                 }
                 _onPanRotate() {
                     return !1
                 }
             }
-            class Qb extends Lf {
+            class Jb extends Rf {
                 get ViewportType() {
-                    return qb
+                    return Xb
                 }
                 get ControllerType() {
-                    return Kb
+                    return Qb
                 }
             }
-            wo(Qb, "displayName", "OrthographicView");
-            class Jb extends Fb {
+            wo(Jb, "displayName", "OrthographicView");
+            class $b extends zb {
                 get isComposite() {
                     return !0
                 }
                 get isLoaded() {
                     return super.isLoaded && this.getSubLayers().every((t => t.isLoaded))
                 }
                 getSubLayers() {
@@ -23387,15 +23390,15 @@
                     let n = this.internalState.subLayers;
                     const i = !n || this.needsUpdate();
                     i && (n = oa(this.renderLayers(), Boolean), this.internalState.subLayers = n), sa("compositeLayer.renderLayers", this, i, n);
                     for (const t of n) t.parent = this
                 }
             }
 
-            function $b({
+            function ty({
                 data: t,
                 getIndex: e,
                 dataRange: n,
                 replace: i
             }) {
                 const {
                     startRow: r = 0,
@@ -23418,72 +23421,72 @@
                     t.length = c
                 }
                 return {
                     startRow: a,
                     endRow: a + i.length
                 }
             }
-            wo(Jb, "layerName", "CompositeLayer");
-            const ty = {
+            wo($b, "layerName", "CompositeLayer");
+            const ey = {
                     name: "project32",
-                    dependencies: [_f],
+                    dependencies: [xf],
                     vs: "\nvec4 project_position_to_clipspace(\n  vec3 position, vec3 position64Low, vec3 offset, out vec4 commonPosition\n) {\n  vec3 projectedPosition = project_position(position, position64Low);\n  mat3 rotation;\n  if (project_needs_rotation(projectedPosition, rotation)) {\n    // offset is specified as ENU\n    // when in globe projection, rotate offset so that the ground alighs with the surface of the globe\n    offset = rotation * offset;\n  }\n  commonPosition = vec4(projectedPosition + offset, 1.0);\n  return project_common_position_to_clipspace(commonPosition);\n}\n\nvec4 project_position_to_clipspace(\n  vec3 position, vec3 position64Low, vec3 offset\n) {\n  vec4 commonPosition;\n  return project_position_to_clipspace(position, position64Low, offset, commonPosition);\n}\n"
                 },
-                ey = {
+                ny = {
                     pickingSelectedColor: null,
                     pickingHighlightColor: new Uint8Array([0, 255, 255, 255]),
                     pickingActive: !1,
                     pickingAttribute: !1
                 },
-                ny = {
+                iy = {
                     inject: {
                         "vs:DECKGL_FILTER_GL_POSITION": "\n    // for picking depth values\n    picking_setPickingAttribute(position.z / position.w);\n  ",
                         "vs:DECKGL_FILTER_COLOR": "\n  picking_setPickingColor(geometry.pickingColor);\n  ",
                         "fs:#decl": "\nuniform bool picking_uAttribute;\n  ",
                         "fs:DECKGL_FILTER_COLOR": {
                             order: 99,
                             injection: "\n  // use highlight color if this fragment belongs to the selected object.\n  color = picking_filterHighlightColor(color);\n\n  // use picking color if rendering to picking FBO.\n  color = picking_filterPickingColor(color);\n    "
                         }
                     },
                     name: "picking",
                     vs: "uniform bool picking_uActive;\nuniform bool picking_uAttribute;\nuniform vec3 picking_uSelectedColor;\nuniform bool picking_uSelectedColorValid;\n\nout vec4 picking_vRGBcolor_Avalid;\n\nconst float COLOR_SCALE = 1. / 255.;\n\nbool picking_isColorValid(vec3 color) {\n  return dot(color, vec3(1.0)) > 0.001;\n}\n\nbool isVertexPicked(vec3 vertexColor) {\n  return\n    picking_uSelectedColorValid &&\n    !picking_isColorValid(abs(vertexColor - picking_uSelectedColor));\n}\n\nvoid picking_setPickingColor(vec3 pickingColor) {\n  if (picking_uActive) {\n    picking_vRGBcolor_Avalid.a = float(picking_isColorValid(pickingColor));\n\n    if (!picking_uAttribute) {\n      picking_vRGBcolor_Avalid.rgb = pickingColor * COLOR_SCALE;\n    }\n  } else {\n    picking_vRGBcolor_Avalid.a = float(isVertexPicked(pickingColor));\n  }\n}\n\nvoid picking_setPickingAttribute(float value) {\n  if (picking_uAttribute) {\n    picking_vRGBcolor_Avalid.r = value;\n  }\n}\nvoid picking_setPickingAttribute(vec2 value) {\n  if (picking_uAttribute) {\n    picking_vRGBcolor_Avalid.rg = value;\n  }\n}\nvoid picking_setPickingAttribute(vec3 value) {\n  if (picking_uAttribute) {\n    picking_vRGBcolor_Avalid.rgb = value;\n  }\n}\n",
                     fs: "uniform bool picking_uActive;\nuniform vec3 picking_uSelectedColor;\nuniform vec4 picking_uHighlightColor;\n\nin vec4 picking_vRGBcolor_Avalid;\nvec4 picking_filterHighlightColor(vec4 color) {\n  if (picking_uActive) {\n    return color;\n  }\n  bool selected = bool(picking_vRGBcolor_Avalid.a);\n\n  if (selected) {\n    float highLightAlpha = picking_uHighlightColor.a;\n    float blendedAlpha = highLightAlpha + color.a * (1.0 - highLightAlpha);\n    float highLightRatio = highLightAlpha / blendedAlpha;\n\n    vec3 blendedRGB = mix(color.rgb, picking_uHighlightColor.rgb, highLightRatio);\n    return vec4(blendedRGB, blendedAlpha);\n  } else {\n    return color;\n  }\n}\nvec4 picking_filterPickingColor(vec4 color) {\n  if (picking_uActive) {\n    if (picking_vRGBcolor_Avalid.a == 0.0) {\n      discard;\n    }\n    return picking_vRGBcolor_Avalid;\n  }\n  return color;\n}\nvec4 picking_filterColor(vec4 color) {\n  vec4 highightColor = picking_filterHighlightColor(color);\n  return picking_filterPickingColor(highightColor);\n}\n\n",
                     getUniforms: function() {
-                        let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : ey;
+                        let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : ny;
                         const e = {};
                         if (void 0 !== t.pickingSelectedColor)
                             if (t.pickingSelectedColor) {
                                 const n = t.pickingSelectedColor.slice(0, 3);
                                 e.picking_uSelectedColorValid = 1, e.picking_uSelectedColor = n
                             } else e.picking_uSelectedColorValid = 0;
                         if (t.pickingHighlightColor) {
                             const n = Array.from(t.pickingHighlightColor, (t => t / 255));
                             Number.isFinite(n[3]) || (n[3] = 1), e.picking_uHighlightColor = n
                         }
                         return void 0 !== t.pickingActive && (e.picking_uActive = Boolean(t.pickingActive), e.picking_uAttribute = Boolean(t.pickingAttribute)), e
                     }
                 },
-                iy = {
+                ry = {
                     POINTS: 0,
                     LINES: 1,
                     LINE_LOOP: 2,
                     LINE_STRIP: 3,
                     TRIANGLES: 4,
                     TRIANGLE_STRIP: 5,
                     TRIANGLE_FAN: 6
                 };
-            class ry {
+            class sy {
                 static get DRAW_MODE() {
-                    return iy
+                    return ry
                 }
                 constructor() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     const {
-                        id: e = Td("geometry"),
-                        drawMode: n = iy.TRIANGLES,
+                        id: e = Ad("geometry"),
+                        drawMode: n = ry.TRIANGLES,
                         attributes: i = {},
                         indices: r = null,
                         vertexCount: s = null
                     } = t;
                     this.id = e, this.drawMode = 0 | n, this.attributes = {}, this.userData = {}, this._setAttributes(i, r), this.vertexCount = s || this._calculateVertexCount(this.attributes, this.indices)
                 }
                 get mode() {
@@ -23506,15 +23509,15 @@
                         value: e,
                         size: 1
                     } : e);
                     for (const e in t) {
                         let n = t[e];
                         n = ArrayBuffer.isView(n) ? {
                             value: n
-                        } : n, Ed(ArrayBuffer.isView(n.value), "".concat(this._print(e), ": must be typed array or object with value as typed array")), "POSITION" !== e && "positions" !== e || n.size || (n.size = 3), "indices" === e ? (Ed(!this.indices), this.indices = n) : this.attributes[e] = n
+                        } : n, Pd(ArrayBuffer.isView(n.value), "".concat(this._print(e), ": must be typed array or object with value as typed array")), "POSITION" !== e && "positions" !== e || n.size || (n.size = 3), "indices" === e ? (Pd(!this.indices), this.indices = n) : this.attributes[e] = n
                     }
                     return this.indices && void 0 !== this.indices.isIndexed && (this.indices = Object.assign({}, this.indices), delete this.indices.isIndexed), this
                 }
                 _calculateVertexCount(t, e) {
                     if (e) return e.value.length;
                     let n = 1 / 0;
                     for (const e in t) {
@@ -23522,73 +23525,73 @@
                             {
                                 value: r,
                                 size: s,
                                 constant: o
                             } = i;
                         !o && r && s >= 1 && (n = Math.min(n, r.length / s))
                     }
-                    return Ed(Number.isFinite(n)), n
+                    return Pd(Number.isFinite(n)), n
                 }
             }
-            const sy = () => {},
-                oy = {
+            const oy = () => {},
+                ay = {
                     10241: 9987,
                     10240: 9729,
                     10242: 33071,
                     10243: 33071
                 };
 
-            function ay(t, e, n, i) {
+            function ly(t, e, n, i) {
                 const r = Math.min(n / e.width, i / e.height),
                     s = Math.floor(e.width * r),
                     o = Math.floor(e.height * r);
                 return 1 === r ? {
                     data: e,
                     width: s,
                     height: o
                 } : (t.canvas.height = o, t.canvas.width = s, t.clearRect(0, 0, s, o), t.drawImage(e, 0, 0, e.width, e.height, 0, 0, s, o), {
                     data: t.canvas,
                     width: s,
                     height: o
                 })
             }
 
-            function ly(t) {
+            function cy(t) {
                 return t && (t.id || t.url)
             }
 
-            function cy(t, e, n) {
+            function hy(t, e, n) {
                 for (let i = 0; i < e.length; i++) {
                     const {
                         icon: r,
                         xOffset: s
                     } = e[i];
-                    t[ly(r)] = {
+                    t[cy(r)] = {
                         ...r,
                         x: s,
                         y: n
                     }
                 }
             }
-            class hy {
+            class uy {
                 constructor(t, {
-                    onUpdate: e = sy,
-                    onError: n = sy
+                    onUpdate: e = oy,
+                    onError: n = oy
                 }) {
                     wo(this, "gl", void 0), wo(this, "onUpdate", void 0), wo(this, "onError", void 0), wo(this, "_loadOptions", null), wo(this, "_texture", null), wo(this, "_externalTexture", null), wo(this, "_mapping", {}), wo(this, "_textureParameters", null), wo(this, "_pendingCount", 0), wo(this, "_autoPacking", !1), wo(this, "_xOffset", 0), wo(this, "_yOffset", 0), wo(this, "_rowHeight", 0), wo(this, "_buffer", 4), wo(this, "_canvasWidth", 1024), wo(this, "_canvasHeight", 0), wo(this, "_canvas", null), this.gl = t, this.onUpdate = e, this.onError = n
                 }
                 finalize() {
                     var t;
                     null === (t = this._texture) || void 0 === t || t.delete()
                 }
                 getTexture() {
                     return this._texture || this._externalTexture
                 }
                 getIconMapping(t) {
-                    const e = this._autoPacking ? ly(t) : t;
+                    const e = this._autoPacking ? cy(t) : t;
                     return this._mapping[e] || {}
                 }
                 setProps({
                     loadOptions: t,
                     autoPacking: e,
                     iconAtlas: n,
                     iconMapping: i,
@@ -23605,19 +23608,19 @@
                     const n = Object.values(function(t, e, n) {
                         if (!t || !e) return null;
                         n = n || {};
                         const i = {},
                             {
                                 iterable: r,
                                 objectInfo: s
-                            } = av(t);
+                            } = lv(t);
                         for (const t of r) {
                             s.index++;
                             const r = e(t, s),
-                                o = ly(r);
+                                o = cy(r);
                             if (!r) throw new Error("Icon is missing.");
                             if (!r.url) throw new Error("Icon url is missing.");
                             i[o] || n[o] && r.url === n[o].url || (i[o] = {
                                 ...r,
                                 source: t,
                                 sourceIndex: s.index
                             })
@@ -23639,26 +23642,26 @@
                             yOffset: r = 0,
                             rowHeight: s = 0,
                             canvasWidth: o
                         }) {
                             let a = [];
                             for (let l = 0; l < t.length; l++) {
                                 const c = t[l];
-                                if (!n[ly(c)]) {
+                                if (!n[cy(c)]) {
                                     const {
                                         height: t,
                                         width: l
                                     } = c;
-                                    i + l + e > o && (cy(n, a, r), i = 0, r = s + r + e, s = 0, a = []), a.push({
+                                    i + l + e > o && (hy(n, a, r), i = 0, r = s + r + e, s = 0, a = []), a.push({
                                         icon: c,
                                         xOffset: i
                                     }), i = i + l + e, s = Math.max(s, t)
                                 }
                             }
-                            return a.length > 0 && cy(n, a, r), {
+                            return a.length > 0 && hy(n, a, r), {
                                 mapping: n,
                                 rowHeight: s,
                                 xOffset: i,
                                 yOffset: r,
                                 canvasWidth: o,
                                 canvasHeight: (l = s + r + e, Math.pow(2, Math.ceil(Math.log2(l))))
                             };
@@ -23668,22 +23671,22 @@
                             buffer: this._buffer,
                             canvasWidth: this._canvasWidth,
                             mapping: this._mapping,
                             rowHeight: this._rowHeight,
                             xOffset: this._xOffset,
                             yOffset: this._yOffset
                         });
-                        this._rowHeight = r, this._mapping = t, this._xOffset = e, this._yOffset = i, this._canvasHeight = s, this._texture || (this._texture = new Qd(this.gl, {
+                        this._rowHeight = r, this._mapping = t, this._xOffset = e, this._yOffset = i, this._canvasHeight = s, this._texture || (this._texture = new Jd(this.gl, {
                             width: this._canvasWidth,
                             height: this._canvasHeight,
-                            parameters: this._textureParameters || oy
+                            parameters: this._textureParameters || ay
                         })), this._texture.height !== this._canvasHeight && (this._texture = function(t, e, n, i) {
                             const r = t.width,
                                 s = t.height,
-                                o = new Qd(t.gl, {
+                                o = new Jd(t.gl, {
                                     width: e,
                                     height: n,
                                     parameters: i
                                 });
                             return function(t, e) {
                                 let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : {};
                                 const {
@@ -23698,60 +23701,60 @@
                                     targetZ: c,
                                     width: h,
                                     height: u
                                 } = n;
                                 const {
                                     framebuffer: d,
                                     deleteFramebuffer: p
-                                } = hp(t);
-                                Ed(d);
+                                } = up(t);
+                                Pd(d);
                                 const {
                                     gl: f,
                                     handle: g
                                 } = d, m = void 0 !== a || void 0 !== l || void 0 !== c;
                                 a = a || 0, l = l || 0, c = c || 0;
                                 const v = f.bindFramebuffer(36160, g);
-                                Ed(e);
+                                Pd(e);
                                 let b = null;
-                                if (e instanceof Kd && (b = e, h = Number.isFinite(h) ? h : b.width, u = Number.isFinite(u) ? u : b.height, b.bind(0), e = b.target), m) switch (e) {
+                                if (e instanceof Qd && (b = e, h = Number.isFinite(h) ? h : b.width, u = Number.isFinite(u) ? u : b.height, b.bind(0), e = b.target), m) switch (e) {
                                     case 3553:
                                     case 34067:
                                         f.copyTexSubImage2D(e, s, a, l, i, r, h, u);
                                         break;
                                     case 35866:
                                     case 32879:
                                         Iu(f).copyTexSubImage3D(e, s, a, l, c, i, r, h, u)
                                 } else f.copyTexImage2D(e, s, o, i, r, h, u, 0);
                                 b && b.unbind(), f.bindFramebuffer(36160, v || null), p && d.delete()
                             }(t, o, {
                                 targetY: 0,
                                 width: r,
                                 height: s
                             }), t.delete(), o
-                        }(this._texture, this._canvasWidth, this._canvasHeight, this._textureParameters || oy)), this.onUpdate(), this._canvas = this._canvas || document.createElement("canvas"), this._loadIcons(n)
+                        }(this._texture, this._canvasWidth, this._canvasHeight, this._textureParameters || ay)), this.onUpdate(), this._canvas = this._canvas || document.createElement("canvas"), this._loadIcons(n)
                     }
                 }
                 _loadIcons(t) {
                     const e = this._canvas.getContext("2d", {
                         willReadFrequently: !0
                     });
                     for (const n of t) this._pendingCount++, nc(n.url, this._loadOptions).then((t => {
-                        const i = ly(n),
+                        const i = cy(n),
                             r = this._mapping[i],
                             {
                                 x: s,
                                 y: o,
                                 width: a,
                                 height: l
                             } = r,
                             {
                                 data: c,
                                 width: h,
                                 height: u
-                            } = ay(e, t, a, l);
+                            } = ly(e, t, a, l);
                         this._texture.setSubImageData({
                             data: c,
                             x: s + (a - h) / 2,
                             y: o + (l - u) / 2,
                             width: h,
                             height: u
                         }), r.width = h, r.height = u, this._texture.generateMipmap(), this.onUpdate()
@@ -23764,16 +23767,16 @@
                             error: t
                         })
                     })).finally((() => {
                         this._pendingCount--
                     }))
                 }
             }
-            const uy = [0, 0, 0, 255],
-                dy = {
+            const dy = [0, 0, 0, 255],
+                py = {
                     iconAtlas: {
                         type: "image",
                         value: null,
                         async: !0
                     },
                     iconMapping: {
                         type: "object",
@@ -23809,15 +23812,15 @@
                     },
                     getIcon: {
                         type: "accessor",
                         value: t => t.icon
                     },
                     getColor: {
                         type: "accessor",
-                        value: uy
+                        value: dy
                     },
                     getSize: {
                         type: "accessor",
                         value: 1
                     },
                     getAngle: {
                         type: "accessor",
@@ -23833,28 +23836,28 @@
                         optional: !0
                     },
                     textureParameters: {
                         type: "object",
                         ignore: !0
                     }
                 };
-            class py extends Fb {
+            class fy extends zb {
                 constructor(...t) {
                     super(...t), wo(this, "state", void 0)
                 }
                 getShaders() {
                     return super.getShaders({
                         vs: "#define SHADER_NAME icon-layer-vertex-shader\n\nattribute vec2 positions;\n\nattribute vec3 instancePositions;\nattribute vec3 instancePositions64Low;\nattribute float instanceSizes;\nattribute float instanceAngles;\nattribute vec4 instanceColors;\nattribute vec3 instancePickingColors;\nattribute vec4 instanceIconFrames;\nattribute float instanceColorModes;\nattribute vec2 instanceOffsets;\nattribute vec2 instancePixelOffset;\n\nuniform float sizeScale;\nuniform vec2 iconsTextureDim;\nuniform float sizeMinPixels;\nuniform float sizeMaxPixels;\nuniform bool billboard;\nuniform int sizeUnits;\n\nvarying float vColorMode;\nvarying vec4 vColor;\nvarying vec2 vTextureCoords;\nvarying vec2 uv;\n\nvec2 rotate_by_angle(vec2 vertex, float angle) {\n  float angle_radian = angle * PI / 180.0;\n  float cos_angle = cos(angle_radian);\n  float sin_angle = sin(angle_radian);\n  mat2 rotationMatrix = mat2(cos_angle, -sin_angle, sin_angle, cos_angle);\n  return rotationMatrix * vertex;\n}\n\nvoid main(void) {\n  geometry.worldPosition = instancePositions;\n  geometry.uv = positions;\n  geometry.pickingColor = instancePickingColors;\n  uv = positions;\n\n  vec2 iconSize = instanceIconFrames.zw;\n  float sizePixels = clamp(\n    project_size_to_pixel(instanceSizes * sizeScale, sizeUnits), \n    sizeMinPixels, sizeMaxPixels\n  );\n  float instanceScale = iconSize.y == 0.0 ? 0.0 : sizePixels / iconSize.y;\n  vec2 pixelOffset = positions / 2.0 * iconSize + instanceOffsets;\n  pixelOffset = rotate_by_angle(pixelOffset, instanceAngles) * instanceScale;\n  pixelOffset += instancePixelOffset;\n  pixelOffset.y *= -1.0;\n\n  if (billboard)  {\n    gl_Position = project_position_to_clipspace(instancePositions, instancePositions64Low, vec3(0.0), geometry.position);\n    DECKGL_FILTER_GL_POSITION(gl_Position, geometry);\n    vec3 offset = vec3(pixelOffset, 0.0);\n    DECKGL_FILTER_SIZE(offset, geometry);\n    gl_Position.xy += project_pixel_size_to_clipspace(offset.xy);\n\n  } else {\n    vec3 offset_common = vec3(project_pixel_size(pixelOffset), 0.0);\n    DECKGL_FILTER_SIZE(offset_common, geometry);\n    gl_Position = project_position_to_clipspace(instancePositions, instancePositions64Low, offset_common, geometry.position); \n    DECKGL_FILTER_GL_POSITION(gl_Position, geometry);\n  }\n\n  vTextureCoords = mix(\n    instanceIconFrames.xy,\n    instanceIconFrames.xy + iconSize,\n    (positions.xy + 1.0) / 2.0\n  ) / iconsTextureDim;\n\n  vColor = instanceColors;\n  DECKGL_FILTER_COLOR(vColor, geometry);\n\n  vColorMode = instanceColorModes;\n}\n",
                         fs: "#define SHADER_NAME icon-layer-fragment-shader\n\nprecision highp float;\n\nuniform float opacity;\nuniform sampler2D iconsTexture;\nuniform float alphaCutoff;\n\nvarying float vColorMode;\nvarying vec4 vColor;\nvarying vec2 vTextureCoords;\nvarying vec2 uv;\n\nvoid main(void) {\n  geometry.uv = uv;\n\n  vec4 texColor = texture2D(iconsTexture, vTextureCoords);\n  vec3 color = mix(texColor.rgb, vColor.rgb, vColorMode);\n  float a = texColor.a * opacity * vColor.a;\n\n  if (a < alphaCutoff) {\n    discard;\n  }\n\n  gl_FragColor = vec4(color, a);\n  DECKGL_FILTER_COLOR(gl_FragColor, geometry);\n}\n",
-                        modules: [ty, ny]
+                        modules: [ey, iy]
                     })
                 }
                 initializeState() {
                     this.state = {
-                        iconManager: new hy(this.context.gl, {
+                        iconManager: new uy(this.context.gl, {
                             onUpdate: this._onUpdate.bind(this),
                             onError: this._onError.bind(this)
                         })
                     }, this.getAttributeManager().addInstanced({
                         instancePositions: {
                             size: 3,
                             type: 5130,
@@ -23886,15 +23889,15 @@
                         },
                         instanceColors: {
                             size: this.props.colorFormat.length,
                             type: 5121,
                             normalized: !0,
                             transition: !0,
                             accessor: "getColor",
-                            defaultValue: uy
+                            defaultValue: dy
                         },
                         instanceAngles: {
                             size: 1,
                             transition: !0,
                             accessor: "getAngle"
                         },
                         instancePixelOffset: {
@@ -23960,18 +23963,18 @@
                         sizeMinPixels: n,
                         sizeMaxPixels: i,
                         billboard: s,
                         alphaCutoff: o
                     }).draw()
                 }
                 _getModel(t) {
-                    return new Yv(t, {
+                    return new Kv(t, {
                         ...this.getShaders(),
                         id: this.props.id,
-                        geometry: new ry({
+                        geometry: new sy({
                             drawMode: 6,
                             attributes: {
                                 positions: {
                                     size: 2,
                                     value: new Float32Array([-1, -1, -1, 1, 1, 1, 1, -1])
                                 }
                             }
@@ -24005,17 +24008,17 @@
                         y: n,
                         width: i,
                         height: r
                     } = this.state.iconManager.getIconMapping(t);
                     return [e, n, i, r]
                 }
             }
-            wo(py, "defaultProps", dy), wo(py, "layerName", "IconLayer");
-            const fy = [0, 0, 0, 255],
-                gy = {
+            wo(fy, "defaultProps", py), wo(fy, "layerName", "IconLayer");
+            const gy = [0, 0, 0, 255],
+                my = {
                     radiusUnits: "meters",
                     radiusScale: {
                         type: "number",
                         min: 0,
                         value: 1
                     },
                     radiusMinPixels: {
@@ -24054,19 +24057,19 @@
                     },
                     getRadius: {
                         type: "accessor",
                         value: 1
                     },
                     getFillColor: {
                         type: "accessor",
-                        value: fy
+                        value: gy
                     },
                     getLineColor: {
                         type: "accessor",
-                        value: fy
+                        value: gy
                     },
                     getLineWidth: {
                         type: "accessor",
                         value: 1
                     },
                     strokeWidth: {
                         deprecatedFor: "getLineWidth"
@@ -24074,20 +24077,20 @@
                     outline: {
                         deprecatedFor: "stroked"
                     },
                     getColor: {
                         deprecatedFor: ["getFillColor", "getLineColor"]
                     }
                 };
-            class my extends Fb {
+            class vy extends zb {
                 getShaders() {
                     return super.getShaders({
                         vs: "#define SHADER_NAME scatterplot-layer-vertex-shader\n\nattribute vec3 positions;\n\nattribute vec3 instancePositions;\nattribute vec3 instancePositions64Low;\nattribute float instanceRadius;\nattribute float instanceLineWidths;\nattribute vec4 instanceFillColors;\nattribute vec4 instanceLineColors;\nattribute vec3 instancePickingColors;\n\nuniform float opacity;\nuniform float radiusScale;\nuniform float radiusMinPixels;\nuniform float radiusMaxPixels;\nuniform float lineWidthScale;\nuniform float lineWidthMinPixels;\nuniform float lineWidthMaxPixels;\nuniform float stroked;\nuniform bool filled;\nuniform bool antialiasing;\nuniform bool billboard;\nuniform int radiusUnits;\nuniform int lineWidthUnits;\n\nvarying vec4 vFillColor;\nvarying vec4 vLineColor;\nvarying vec2 unitPosition;\nvarying float innerUnitRadius;\nvarying float outerRadiusPixels;\n\n\nvoid main(void) {\n  geometry.worldPosition = instancePositions;\n  outerRadiusPixels = clamp(\n    project_size_to_pixel(radiusScale * instanceRadius, radiusUnits),\n    radiusMinPixels, radiusMaxPixels\n  );\n  float lineWidthPixels = clamp(\n    project_size_to_pixel(lineWidthScale * instanceLineWidths, lineWidthUnits),\n    lineWidthMinPixels, lineWidthMaxPixels\n  );\n  outerRadiusPixels += stroked * lineWidthPixels / 2.0;\n  float edgePadding = antialiasing ? (outerRadiusPixels + SMOOTH_EDGE_RADIUS) / outerRadiusPixels : 1.0;\n  unitPosition = edgePadding * positions.xy;\n  geometry.uv = unitPosition;\n  geometry.pickingColor = instancePickingColors;\n\n  innerUnitRadius = 1.0 - stroked * lineWidthPixels / outerRadiusPixels;\n  \n  if (billboard) {\n    gl_Position = project_position_to_clipspace(instancePositions, instancePositions64Low, vec3(0.0), geometry.position);\n    DECKGL_FILTER_GL_POSITION(gl_Position, geometry);\n    vec3 offset = edgePadding * positions * outerRadiusPixels;\n    DECKGL_FILTER_SIZE(offset, geometry);\n    gl_Position.xy += project_pixel_size_to_clipspace(offset.xy);\n  } else {\n    vec3 offset = edgePadding * positions * project_pixel_size(outerRadiusPixels);\n    DECKGL_FILTER_SIZE(offset, geometry);\n    gl_Position = project_position_to_clipspace(instancePositions, instancePositions64Low, offset, geometry.position);\n    DECKGL_FILTER_GL_POSITION(gl_Position, geometry);\n  }\n  vFillColor = vec4(instanceFillColors.rgb, instanceFillColors.a * opacity);\n  DECKGL_FILTER_COLOR(vFillColor, geometry);\n  vLineColor = vec4(instanceLineColors.rgb, instanceLineColors.a * opacity);\n  DECKGL_FILTER_COLOR(vLineColor, geometry);\n}\n",
                         fs: "#define SHADER_NAME scatterplot-layer-fragment-shader\n\nprecision highp float;\n\nuniform bool filled;\nuniform float stroked;\nuniform bool antialiasing;\n\nvarying vec4 vFillColor;\nvarying vec4 vLineColor;\nvarying vec2 unitPosition;\nvarying float innerUnitRadius;\nvarying float outerRadiusPixels;\n\nvoid main(void) {\n  geometry.uv = unitPosition;\n\n  float distToCenter = length(unitPosition) * outerRadiusPixels;\n  float inCircle = antialiasing ? \n    smoothedge(distToCenter, outerRadiusPixels) : \n    step(distToCenter, outerRadiusPixels);\n\n  if (inCircle == 0.0) {\n    discard;\n  }\n\n  if (stroked > 0.5) {\n    float isLine = antialiasing ? \n      smoothedge(innerUnitRadius * outerRadiusPixels, distToCenter) :\n      step(innerUnitRadius * outerRadiusPixels, distToCenter);\n\n    if (filled) {\n      gl_FragColor = mix(vFillColor, vLineColor, isLine);\n    } else {\n      if (isLine == 0.0) {\n        discard;\n      }\n      gl_FragColor = vec4(vLineColor.rgb, vLineColor.a * isLine);\n    }\n  } else if (filled) {\n    gl_FragColor = vFillColor;\n  } else {\n    discard;\n  }\n\n  gl_FragColor.a *= inCircle;\n  DECKGL_FILTER_COLOR(gl_FragColor, geometry);\n}\n",
-                        modules: [ty, ny]
+                        modules: [ey, iy]
                     })
                 }
                 initializeState() {
                     this.getAttributeManager().addInstanced({
                         instancePositions: {
                             size: 3,
                             type: 5130,
@@ -24163,35 +24166,35 @@
                         lineWidthUnits: Ih[c],
                         lineWidthScale: h,
                         lineWidthMinPixels: u,
                         lineWidthMaxPixels: d
                     }).draw()
                 }
                 _getModel(t) {
-                    return new Yv(t, {
+                    return new Kv(t, {
                         ...this.getShaders(),
                         id: this.props.id,
-                        geometry: new ry({
+                        geometry: new sy({
                             drawMode: 6,
                             vertexCount: 4,
                             attributes: {
                                 positions: {
                                     size: 3,
                                     value: new Float32Array([-1, -1, 0, 1, -1, 0, 1, 1, 0, -1, 1, 0])
                                 }
                             }
                         }),
                         isInstanced: !0
                     })
                 }
             }
-            wo(my, "defaultProps", gy), wo(my, "layerName", "ScatterplotLayer");
-            const vy = .75,
-                by = [];
-            class yy extends py {
+            wo(vy, "defaultProps", my), wo(vy, "layerName", "ScatterplotLayer");
+            const by = .75,
+                yy = [];
+            class _y extends fy {
                 constructor(...t) {
                     super(...t), wo(this, "state", void 0)
                 }
                 getShaders() {
                     return {
                         ...super.getShaders(),
                         fs: "#define SHADER_NAME multi-icon-layer-fragment-shader\n\nprecision highp float;\n\nuniform float opacity;\nuniform sampler2D iconsTexture;\nuniform float gamma;\nuniform bool sdf;\nuniform float alphaCutoff;\nuniform float sdfBuffer;\nuniform float outlineBuffer;\nuniform vec4 outlineColor;\n\nvarying vec4 vColor;\nvarying vec2 vTextureCoords;\nvarying vec2 uv;\n\nvoid main(void) {\n  geometry.uv = uv;\n\n  if (!picking_uActive) {\n    float alpha = texture2D(iconsTexture, vTextureCoords).a;\n    vec4 color = vColor;\n    if (sdf) {\n      float distance = alpha;\n      alpha = smoothstep(sdfBuffer - gamma, sdfBuffer + gamma, distance);\n\n      if (outlineBuffer > 0.0) {\n        float inFill = alpha;\n        float inBorder = smoothstep(outlineBuffer - gamma, outlineBuffer + gamma, distance);\n        color = mix(outlineColor, vColor, inFill);\n        alpha = inBorder;\n      }\n    }\n    float a = alpha * color.a;\n    \n    if (a < alphaCutoff) {\n      discard;\n    }\n\n    gl_FragColor = vec4(color.rgb, a * opacity);\n  }\n\n  DECKGL_FILTER_COLOR(gl_FragColor, geometry);\n}\n"
@@ -24229,58 +24232,58 @@
                 draw(t) {
                     const {
                         sdf: e,
                         smoothing: n,
                         outlineWidth: i
                     } = this.props, {
                         outlineColor: r
-                    } = this.state, s = i ? Math.max(n, vy * (1 - i)) : -1;
+                    } = this.state, s = i ? Math.max(n, by * (1 - i)) : -1;
                     if (t.uniforms = {
                             ...t.uniforms,
-                            sdfBuffer: vy,
+                            sdfBuffer: by,
                             outlineBuffer: s,
                             gamma: n,
                             sdf: Boolean(e),
                             outlineColor: r
                         }, super.draw(t), e && i) {
                         const {
                             iconManager: t
                         } = this.state;
                         t.getTexture() && this.state.model.draw({
                             uniforms: {
-                                outlineBuffer: vy
+                                outlineBuffer: by
                             }
                         })
                     }
                 }
                 getInstanceOffset(t) {
-                    return t ? Array.from(t).flatMap((t => super.getInstanceOffset(t))) : by
+                    return t ? Array.from(t).flatMap((t => super.getInstanceOffset(t))) : yy
                 }
                 getInstanceColorMode(t) {
                     return 1
                 }
                 getInstanceIconFrame(t) {
-                    return t ? Array.from(t).flatMap((t => super.getInstanceIconFrame(t))) : by
+                    return t ? Array.from(t).flatMap((t => super.getInstanceIconFrame(t))) : yy
                 }
             }
-            wo(yy, "defaultProps", {
+            wo(_y, "defaultProps", {
                 getIconOffsets: {
                     type: "accessor",
                     value: t => t.offsets
                 },
                 alphaCutoff: .001,
                 smoothing: .1,
                 outlineWidth: 0,
                 outlineColor: {
                     type: "color",
                     value: [0, 0, 0, 255]
                 }
-            }), wo(yy, "layerName", "MultiIconLayer");
-            const _y = 1e20;
-            class xy {
+            }), wo(_y, "layerName", "MultiIconLayer");
+            const xy = 1e20;
+            class wy {
                 constructor({
                     fontSize: t = 24,
                     buffer: e = 3,
                     radius: n = 8,
                     cutoff: i = .25,
                     fontFamily: r = "sans-serif",
                     fontWeight: s = "normal",
@@ -24320,106 +24323,106 @@
                         ctx: f,
                         buffer: g,
                         gridInner: m,
                         gridOuter: v
                     } = this;
                     f.clearRect(g, g, a, l), f.fillText(t, g, g + o);
                     const b = f.getImageData(g, g, a, l);
-                    v.fill(_y, 0, u), m.fill(0, 0, u);
+                    v.fill(xy, 0, u), m.fill(0, 0, u);
                     for (let t = 0; t < l; t++)
                         for (let e = 0; e < a; e++) {
                             const n = b.data[4 * (t * a + e) + 3] / 255;
                             if (0 === n) continue;
                             const i = (t + g) * c + e + g;
-                            if (1 === n) v[i] = 0, m[i] = _y;
+                            if (1 === n) v[i] = 0, m[i] = xy;
                             else {
                                 const t = .5 - n;
                                 v[i] = t > 0 ? t * t : 0, m[i] = t < 0 ? t * t : 0
                             }
                         }
-                    wy(v, 0, 0, c, h, c, this.f, this.v, this.z), wy(m, g, g, a, l, c, this.f, this.v, this.z);
+                    Ey(v, 0, 0, c, h, c, this.f, this.v, this.z), Ey(m, g, g, a, l, c, this.f, this.v, this.z);
                     for (let t = 0; t < u; t++) {
                         const e = Math.sqrt(v[t]) - Math.sqrt(m[t]);
                         d[t] = Math.round(255 - 255 * (e / this.radius + this.cutoff))
                     }
                     return p
                 }
             }
 
-            function wy(t, e, n, i, r, s, o, a, l) {
-                for (let c = e; c < e + i; c++) Ey(t, n * s + c, s, r, o, a, l);
-                for (let c = n; c < n + r; c++) Ey(t, c * s + e, 1, i, o, a, l)
+            function Ey(t, e, n, i, r, s, o, a, l) {
+                for (let c = e; c < e + i; c++) Py(t, n * s + c, s, r, o, a, l);
+                for (let c = n; c < n + r; c++) Py(t, c * s + e, 1, i, o, a, l)
             }
 
-            function Ey(t, e, n, i, r, s, o) {
-                s[0] = 0, o[0] = -_y, o[1] = _y, r[0] = t[e];
+            function Py(t, e, n, i, r, s, o) {
+                s[0] = 0, o[0] = -xy, o[1] = xy, r[0] = t[e];
                 for (let a = 1, l = 0, c = 0; a < i; a++) {
                     r[a] = t[e + a * n];
                     const i = a * a;
                     do {
                         const t = s[l];
                         c = (r[a] - r[t] + i - t * t) / (a - t) / 2
                     } while (c <= o[l] && --l > -1);
-                    l++, s[l] = a, o[l] = c, o[l + 1] = _y
+                    l++, s[l] = a, o[l] = c, o[l + 1] = xy
                 }
                 for (let a = 0, l = 0; a < i; a++) {
                     for (; o[l + 1] < a;) l++;
                     const i = s[l],
                         c = a - i;
                     t[e + a * n] = r[i] + c * c
                 }
             }
-            const Py = [];
+            const Sy = [];
 
-            function Sy(t, e, n, i) {
+            function Cy(t, e, n, i) {
                 let r = 0;
                 for (let o = e; o < n; o++) {
                     var s;
                     r += (null === (s = i[t[o]]) || void 0 === s ? void 0 : s.layoutWidth) || 0
                 }
                 return r
             }
 
-            function Cy(t, e, n, i, r, s) {
+            function Ty(t, e, n, i, r, s) {
                 let o = e,
                     a = 0;
                 for (let l = e; l < n; l++) {
-                    const e = Sy(t, l, l + 1, r);
+                    const e = Cy(t, l, l + 1, r);
                     a + e > i && (o < l && s.push(l), o = l, a = 0), a += e
                 }
                 return a
             }
 
-            function Ty(t, e, n, i, r = 0, s) {
+            function Ay(t, e, n, i, r = 0, s) {
                 void 0 === s && (s = t.length);
                 const o = [];
-                return "break-all" === e ? Cy(t, r, s, n, i, o) : function(t, e, n, i, r, s) {
+                return "break-all" === e ? Ty(t, r, s, n, i, o) : function(t, e, n, i, r, s) {
                     let o = e,
                         a = e,
                         l = e,
                         c = 0;
                     for (let h = e; h < n; h++)
                         if (" " === t[h] ? l = h + 1 : " " !== t[h + 1] && h + 1 !== n || (l = h + 1), l > a) {
-                            let e = Sy(t, a, l, r);
-                            c + e > i && (o < a && (s.push(a), o = a, c = 0), e > i && (e = Cy(t, a, l, i, r, s), o = s[s.length - 1])), a = l, c += e
+                            let e = Cy(t, a, l, r);
+                            c + e > i && (o < a && (s.push(a), o = a, c = 0), e > i && (e = Ty(t, a, l, i, r, s), o = s[s.length - 1])), a = l, c += e
                         }
                 }(t, r, s, n, i, o), o
             }
 
-            function Ay(t, e, n, i, r, s) {
+            function My(t, e, n, i, r, s) {
                 let o = 0,
                     a = 0;
                 for (let s = e; s < n; s++) {
                     const e = t[s],
                         n = i[e];
                     n ? (a || (a = n.layoutHeight), r[s] = o + n.layoutWidth / 2, o += n.layoutWidth) : (na.warn("Missing character: ".concat(e, " (").concat(e.codePointAt(0), ")"))(), r[s] = o, o += 32)
                 }
                 s[0] = o, s[1] = a
             }
-            class My {
+            class Oy {
                 constructor(t = 5) {
                     wo(this, "limit", void 0), wo(this, "_cache", {}), wo(this, "_order", []), this.limit = t
                 }
                 get(t) {
                     const e = this._cache[t];
                     return e && (this._deleteOrder(t), this._appendOrder(t)), e
                 }
@@ -24433,42 +24436,42 @@
                     const e = this._order.indexOf(t);
                     e >= 0 && this._order.splice(e, 1)
                 }
                 _appendOrder(t) {
                     this._order.push(t)
                 }
             }
-            const Oy = {
+            const Ly = {
                 fontFamily: "Monaco, monospace",
                 fontWeight: "normal",
                 characterSet: function() {
                     const t = [];
                     for (let e = 32; e < 128; e++) t.push(String.fromCharCode(e));
                     return t
                 }(),
                 fontSize: 64,
                 buffer: 4,
                 sdf: !1,
                 cutoff: .25,
                 radius: 12,
                 smoothing: .1
             };
-            let Ly = new My(3);
+            let Ry = new Oy(3);
 
-            function Ry(t, e) {
+            function Iy(t, e) {
                 for (let n = 0; n < t.length; n++) e.data[4 * n + 3] = t[n]
             }
 
-            function Iy(t, e, n, i) {
+            function ky(t, e, n, i) {
                 t.font = "".concat(i, " ").concat(n, "px ").concat(e), t.fillStyle = "#000", t.textBaseline = "alphabetic", t.textAlign = "left"
             }
-            class ky {
+            class jy {
                 constructor() {
                     wo(this, "props", {
-                        ...Oy
+                        ...Ly
                     }), wo(this, "_key", void 0), wo(this, "_atlas", void 0)
                 }
                 get texture() {
                     return this._atlas
                 }
                 get mapping() {
                     return this._atlas && this._atlas.mapping
@@ -24481,23 +24484,23 @@
                     return (1.2 * t + 2 * e) / t
                 }
                 setProps(t = {}) {
                     Object.assign(this.props, t), this._key = this._getKey();
                     const e = function(t, e) {
                             let n;
                             n = "string" == typeof e ? new Set(Array.from(e)) : new Set(e);
-                            const i = Ly.get(t);
+                            const i = Ry.get(t);
                             if (!i) return n;
                             for (const t in i.mapping) n.has(t) && n.delete(t);
                             return n
                         }(this._key, this.props.characterSet),
-                        n = Ly.get(this._key);
+                        n = Ry.get(this._key);
                     if (n && 0 === e.size) return void(this._atlas !== n && (this._atlas = n));
                     const i = this._generateFontAtlas(e, n);
-                    this._atlas = i, Ly.set(this._key, i)
+                    this._atlas = i, Ry.set(this._key, i)
                 }
                 _generateFontAtlas(t, e) {
                     const {
                         fontFamily: n,
                         fontWeight: i,
                         fontSize: r,
                         buffer: s,
@@ -24506,15 +24509,15 @@
                         cutoff: l
                     } = this.props;
                     let c = e && e.data;
                     c || (c = document.createElement("canvas"), c.width = 1024);
                     const h = c.getContext("2d", {
                         willReadFrequently: !0
                     });
-                    Iy(h, n, r, i);
+                    ky(h, n, r, i);
                     const {
                         mapping: u,
                         canvasHeight: d,
                         xOffset: p,
                         yOffset: f
                     } = function({
                         characterSet: t,
@@ -24559,16 +24562,16 @@
                             yOffset: e.yOffset
                         }
                     });
                     if (c.height !== d) {
                         const t = h.getImageData(0, 0, c.width, c.height);
                         c.height = d, h.putImageData(t, 0, 0)
                     }
-                    if (Iy(h, n, r, i), o) {
-                        const e = new xy({
+                    if (ky(h, n, r, i), o) {
+                        const e = new wy({
                             fontSize: r,
                             buffer: s,
                             radius: a,
                             cutoff: l,
                             fontFamily: n,
                             fontWeight: "".concat(i)
                         });
@@ -24577,15 +24580,15 @@
                                 data: t,
                                 width: i,
                                 height: s,
                                 glyphTop: o
                             } = e.draw(n);
                             u[n].width = i, u[n].layoutOffsetY = .9 * r - o;
                             const a = h.createImageData(i, s);
-                            Ry(t, a), h.putImageData(a, u[n].x, u[n].y)
+                            Iy(t, a), h.putImageData(a, u[n].x, u[n].y)
                         }
                     } else
                         for (const e of t) h.fillText(e, u[e].x, u[e].y + s + .9 * r);
                     return {
                         xOffset: p,
                         yOffset: f,
                         mapping: u,
@@ -24603,15 +24606,15 @@
                         sdf: r,
                         radius: s,
                         cutoff: o
                     } = this.props;
                     return r ? "".concat(t, " ").concat(e, " ").concat(n, " ").concat(i, " ").concat(s, " ").concat(o) : "".concat(t, " ").concat(e, " ").concat(n, " ").concat(i)
                 }
             }
-            const jy = {
+            const Fy = {
                 billboard: !0,
                 sizeScale: 1,
                 sizeUnits: "pixels",
                 sizeMinPixels: 0,
                 sizeMaxPixels: Number.MAX_SAFE_INTEGER,
                 padding: {
                     type: "array",
@@ -24646,23 +24649,23 @@
                     value: [0, 0, 0, 255]
                 },
                 getLineWidth: {
                     type: "accessor",
                     value: 1
                 }
             };
-            class Fy extends Fb {
+            class zy extends zb {
                 constructor(...t) {
                     super(...t), wo(this, "state", void 0)
                 }
                 getShaders() {
                     return super.getShaders({
                         vs: "#define SHADER_NAME text-background-layer-vertex-shader\n\nattribute vec2 positions;\n\nattribute vec3 instancePositions;\nattribute vec3 instancePositions64Low;\nattribute vec4 instanceRects;\nattribute float instanceSizes;\nattribute float instanceAngles;\nattribute vec2 instancePixelOffsets;\nattribute float instanceLineWidths;\nattribute vec4 instanceFillColors;\nattribute vec4 instanceLineColors;\nattribute vec3 instancePickingColors;\n\nuniform bool billboard;\nuniform float opacity;\nuniform float sizeScale;\nuniform float sizeMinPixels;\nuniform float sizeMaxPixels;\nuniform vec4 padding;\nuniform int sizeUnits;\n\nvarying vec4 vFillColor;\nvarying vec4 vLineColor;\nvarying float vLineWidth;\nvarying vec2 uv;\nvarying vec2 dimensions;\n\nvec2 rotate_by_angle(vec2 vertex, float angle) {\n  float angle_radian = radians(angle);\n  float cos_angle = cos(angle_radian);\n  float sin_angle = sin(angle_radian);\n  mat2 rotationMatrix = mat2(cos_angle, -sin_angle, sin_angle, cos_angle);\n  return rotationMatrix * vertex;\n}\n\nvoid main(void) {\n  geometry.worldPosition = instancePositions;\n  geometry.uv = positions;\n  geometry.pickingColor = instancePickingColors;\n  uv = positions;\n  vLineWidth = instanceLineWidths;\n  float sizePixels = clamp(\n    project_size_to_pixel(instanceSizes * sizeScale, sizeUnits),\n    sizeMinPixels, sizeMaxPixels\n  );\n\n  dimensions = instanceRects.zw * sizePixels + padding.xy + padding.zw;\n\n  vec2 pixelOffset = (positions * instanceRects.zw + instanceRects.xy) * sizePixels + mix(-padding.xy, padding.zw, positions);\n  pixelOffset = rotate_by_angle(pixelOffset, instanceAngles);\n  pixelOffset += instancePixelOffsets;\n  pixelOffset.y *= -1.0;\n\n  if (billboard)  {\n    gl_Position = project_position_to_clipspace(instancePositions, instancePositions64Low, vec3(0.0), geometry.position);\n    DECKGL_FILTER_GL_POSITION(gl_Position, geometry);\n    vec3 offset = vec3(pixelOffset, 0.0);\n    DECKGL_FILTER_SIZE(offset, geometry);\n    gl_Position.xy += project_pixel_size_to_clipspace(offset.xy);\n  } else {\n    vec3 offset_common = vec3(project_pixel_size(pixelOffset), 0.0);\n    DECKGL_FILTER_SIZE(offset_common, geometry);\n    gl_Position = project_position_to_clipspace(instancePositions, instancePositions64Low, offset_common, geometry.position);\n    DECKGL_FILTER_GL_POSITION(gl_Position, geometry);\n  }\n  vFillColor = vec4(instanceFillColors.rgb, instanceFillColors.a * opacity);\n  DECKGL_FILTER_COLOR(vFillColor, geometry);\n  vLineColor = vec4(instanceLineColors.rgb, instanceLineColors.a * opacity);\n  DECKGL_FILTER_COLOR(vLineColor, geometry);\n}\n",
                         fs: "#define SHADER_NAME text-background-layer-fragment-shader\n\nprecision highp float;\n\nuniform bool stroked;\n\nvarying vec4 vFillColor;\nvarying vec4 vLineColor;\nvarying float vLineWidth;\nvarying vec2 uv;\nvarying vec2 dimensions;\n\nvoid main(void) {\n  geometry.uv = uv;\n\n  vec2 pixelPosition = uv * dimensions;\n  if (stroked) {\n    float distToEdge = min(\n      min(pixelPosition.x, dimensions.x - pixelPosition.x),\n      min(pixelPosition.y, dimensions.y - pixelPosition.y)\n    );\n    float isBorder = smoothedge(distToEdge, vLineWidth);\n    gl_FragColor = mix(vFillColor, vLineColor, isBorder);\n  } else {\n    gl_FragColor = vFillColor;\n  }\n\n  DECKGL_FILTER_COLOR(gl_FragColor, geometry);\n}\n",
-                        modules: [ty, ny]
+                        modules: [ey, iy]
                     })
                 }
                 initializeState() {
                     this.getAttributeManager().addInstanced({
                         instancePositions: {
                             size: 3,
                             type: 5130,
@@ -24748,81 +24751,81 @@
                         sizeUnits: Ih[i],
                         sizeScale: n,
                         sizeMinPixels: r,
                         sizeMaxPixels: s
                     }).draw()
                 }
                 _getModel(t) {
-                    return new Yv(t, {
+                    return new Kv(t, {
                         ...this.getShaders(),
                         id: this.props.id,
-                        geometry: new ry({
+                        geometry: new sy({
                             drawMode: 6,
                             vertexCount: 4,
                             attributes: {
                                 positions: {
                                     size: 2,
                                     value: new Float32Array([0, 0, 1, 0, 1, 1, 0, 1])
                                 }
                             }
                         }),
                         isInstanced: !0
                     })
                 }
             }
-            wo(Fy, "defaultProps", jy), wo(Fy, "layerName", "TextBackgroundLayer");
-            const zy = {
+            wo(zy, "defaultProps", Fy), wo(zy, "layerName", "TextBackgroundLayer");
+            const By = {
                     start: 1,
                     middle: 0,
                     end: -1
                 },
-                By = {
+                Dy = {
                     top: 1,
                     center: 0,
                     bottom: -1
                 },
-                Dy = [0, 0, 0, 255],
-                Ny = {
+                Ny = [0, 0, 0, 255],
+                Vy = {
                     billboard: !0,
                     sizeScale: 1,
                     sizeUnits: "pixels",
                     sizeMinPixels: 0,
                     sizeMaxPixels: Number.MAX_SAFE_INTEGER,
                     background: !1,
                     getBackgroundColor: {
                         type: "accessor",
                         value: [255, 255, 255, 255]
                     },
                     getBorderColor: {
                         type: "accessor",
-                        value: Dy
+                        value: Ny
                     },
                     getBorderWidth: {
                         type: "accessor",
                         value: 0
                     },
                     backgroundPadding: {
                         type: "array",
                         value: [0, 0, 0, 0]
                     },
                     characterSet: {
                         type: "object",
-                        value: Oy.characterSet
+                        value: Ly.characterSet
                     },
-                    fontFamily: Oy.fontFamily,
-                    fontWeight: Oy.fontWeight,
+                    fontFamily: Ly.fontFamily,
+                    fontWeight: Ly.fontWeight,
                     lineHeight: 1,
                     outlineWidth: {
                         type: "number",
                         value: 0,
                         min: 0
                     },
                     outlineColor: {
                         type: "color",
-                        value: Dy
+                        value: Ny
                     },
                     fontSettings: {
                         type: "object",
                         value: {},
                         compare: 1
                     },
                     wordBreak: "break-word",
@@ -24836,15 +24839,15 @@
                     },
                     getPosition: {
                         type: "accessor",
                         value: t => t.position
                     },
                     getColor: {
                         type: "accessor",
-                        value: Dy
+                        value: Ny
                     },
                     getSize: {
                         type: "accessor",
                         value: 32
                     },
                     getAngle: {
                         type: "accessor",
@@ -24862,51 +24865,51 @@
                         type: "accessor",
                         value: [0, 0]
                     },
                     backgroundColor: {
                         deprecatedFor: ["background", "getBackgroundColor"]
                     }
                 };
-            class Vy extends Jb {
+            class Uy extends $b {
                 constructor(...t) {
                     super(...t), wo(this, "state", void 0), wo(this, "getBoundingRect", ((t, e) => {
                         let {
                             size: [n, i]
                         } = this.transformParagraph(t, e);
                         const {
                             fontSize: r
                         } = this.state.fontAtlasManager.props;
                         n /= r, i /= r;
                         const {
                             getTextAnchor: s,
                             getAlignmentBaseline: o
                         } = this.props;
-                        return [(zy["function" == typeof s ? s(t, e) : s] - 1) * n / 2, (By["function" == typeof o ? o(t, e) : o] - 1) * i / 2, n, i]
+                        return [(By["function" == typeof s ? s(t, e) : s] - 1) * n / 2, (Dy["function" == typeof o ? o(t, e) : o] - 1) * i / 2, n, i]
                     })), wo(this, "getIconOffsets", ((t, e) => {
                         const {
                             getTextAnchor: n,
                             getAlignmentBaseline: i
                         } = this.props, {
                             x: r,
                             y: s,
                             rowWidth: o,
                             size: [a, l]
-                        } = this.transformParagraph(t, e), c = zy["function" == typeof n ? n(t, e) : n], h = By["function" == typeof i ? i(t, e) : i], u = r.length, d = new Array(2 * u);
+                        } = this.transformParagraph(t, e), c = By["function" == typeof n ? n(t, e) : n], h = Dy["function" == typeof i ? i(t, e) : i], u = r.length, d = new Array(2 * u);
                         let p = 0;
                         for (let t = 0; t < u; t++) {
                             const e = (1 - c) * (a - o[t]) / 2;
                             d[p++] = (c - 1) * a / 2 + e + r[t], d[p++] = (h - 1) * l / 2 + s[t]
                         }
                         return d
                     }))
                 }
                 initializeState() {
                     this.state = {
                         styleVersion: 0,
-                        fontAtlasManager: new ky
+                        fontAtlasManager: new jy
                     }, this.props.maxWidth > 0 && na.warn("v8.9 breaking change: TextLayer maxWidth is now relative to text size")()
                 }
                 updateState(t) {
                     const {
                         props: e,
                         oldProps: n,
                         changeFlags: i
@@ -24996,15 +24999,15 @@
                         r = n, s = (e, {
                             index: n
                         }) => t[n]
                     } else {
                         const {
                             iterable: t,
                             objectInfo: n
-                        } = av(e);
+                        } = lv(e);
                         o = [0], r = 0;
                         for (const e of t) {
                             n.index++;
                             const t = Array.from(s(e, n) || "");
                             a && t.forEach(a.add, a), r += t.length, o.push(r)
                         }
                     }
@@ -25034,19 +25037,19 @@
                             d = [0, 0];
                         let p = 0,
                             f = 0,
                             g = 0;
                         for (let t = 0; t <= o; t++) {
                             const v = s[t];
                             if ("\n" !== v && t !== o || (g = t), g > f) {
-                                const t = h ? Ty(s, n, i, r, f, g) : Py;
+                                const t = h ? Ay(s, n, i, r, f, g) : Sy;
                                 for (let n = 0; n <= t.length; n++) {
                                     const i = 0 === n ? f : t[n - 1],
                                         o = n < t.length ? t[n] : g;
-                                    Ay(s, i, o, r, a, d);
+                                    My(s, i, o, r, a, d);
                                     for (let t = i; t < o; t++) {
                                         var m;
                                         const e = (null === (m = r[s[t]]) || void 0 === m ? void 0 : m.layoutOffsetY) || 0;
                                         l[t] = p + d[1] / 2 + e, c[t] = d[0]
                                     }
                                     p += d[1] * e, u[0] = Math.max(u[0], d[0])
                                 }
@@ -25092,15 +25095,15 @@
                         outlineColor: w,
                         sizeScale: E,
                         sizeUnits: P,
                         sizeMinPixels: S,
                         sizeMaxPixels: C,
                         transitions: T,
                         updateTriggers: A
-                    } = this.props, M = this.getSubLayerClass("characters", yy), O = this.getSubLayerClass("background", Fy);
+                    } = this.props, M = this.getSubLayerClass("characters", _y), O = this.getSubLayerClass("background", zy);
                     return [b && new O({
                         getFillColor: f,
                         getLineColor: g,
                         getLineWidth: m,
                         padding: v,
                         getPosition: c,
                         getSize: u,
@@ -25143,16 +25146,16 @@
                             attributes: a.attributes.background
                         } : a,
                         _dataDiff: l,
                         autoHighlight: !1,
                         getBoundingRect: this.getBoundingRect
                     }), new M({
                         sdf: _.sdf,
-                        smoothing: Number.isFinite(_.smoothing) ? _.smoothing : Oy.smoothing,
-                        outlineWidth: x / (_.radius || Oy.radius),
+                        smoothing: Number.isFinite(_.smoothing) ? _.smoothing : Ly.smoothing,
+                        outlineWidth: x / (_.radius || Ly.radius),
                         outlineColor: w,
                         iconAtlas: r,
                         iconMapping: s,
                         getPosition: c,
                         getColor: h,
                         getSize: u,
                         getAngle: d,
@@ -25191,20 +25194,20 @@
                         numInstances: e,
                         getIconOffsets: this.getIconOffsets,
                         getIcon: n
                     })]
                 }
                 static set fontAtlasCacheLimit(t) {
                     ! function(t) {
-                        na.assert(Number.isFinite(t) && t >= 3, "Invalid cache limit"), Ly = new My(t)
+                        na.assert(Number.isFinite(t) && t >= 3, "Invalid cache limit"), Ry = new Oy(t)
                     }(t)
                 }
             }
-            wo(Vy, "defaultProps", Ny), wo(Vy, "layerName", "TextLayer");
-            class Uy {
+            wo(Uy, "defaultProps", Vy), wo(Uy, "layerName", "TextLayer");
+            class Gy {
                 constructor(t) {
                     wo(this, "opts", void 0), wo(this, "typedArrayManager", void 0), wo(this, "indexStarts", [0]), wo(this, "vertexStarts", [0]), wo(this, "vertexCount", 0), wo(this, "instanceCount", 0), wo(this, "attributes", void 0), wo(this, "_attributeDefs", void 0), wo(this, "data", void 0), wo(this, "getGeometry", void 0), wo(this, "geometryBuffer", void 0), wo(this, "buffers", void 0), wo(this, "positionSize", void 0), wo(this, "normalize", void 0);
                     const {
                         attributes: e = {}
                     } = t;
                     this.typedArrayManager = sc, this.attributes = {}, this._attributeDefs = e, this.opts = t, this.updateGeometry(t)
                 }
@@ -25215,30 +25218,30 @@
                         buffers: n = {},
                         getGeometry: i,
                         geometryBuffer: r,
                         positionFormat: s,
                         dataChanged: o,
                         normalize: a = !0
                     } = this.opts;
-                    if (this.data = e, this.getGeometry = i, this.positionSize = r && r.size || ("XY" === s ? 2 : 3), this.buffers = n, this.normalize = a, r && (Of(e.startIndices), this.getGeometry = this.getGeometryFromBuffer(r), a || (n.positions = r)), this.geometryBuffer = n.positions, Array.isArray(o))
+                    if (this.data = e, this.getGeometry = i, this.positionSize = r && r.size || ("XY" === s ? 2 : 3), this.buffers = n, this.normalize = a, r && (Lf(e.startIndices), this.getGeometry = this.getGeometryFromBuffer(r), a || (n.positions = r)), this.geometryBuffer = n.positions, Array.isArray(o))
                         for (const t of o) this._rebuildGeometry(t);
                     else this._rebuildGeometry()
                 }
                 updatePartialGeometry({
                     startRow: t,
                     endRow: e
                 }) {
                     this._rebuildGeometry({
                         startRow: t,
                         endRow: e
                     })
                 }
                 getGeometryFromBuffer(t) {
                     const e = t.value || t;
-                    return ArrayBuffer.isView(e) ? cv(e, {
+                    return ArrayBuffer.isView(e) ? hv(e, {
                         size: this.positionSize,
                         offset: t.offset,
                         stride: t.stride,
                         startIndices: this.data.startIndices
                     }) : null
                 }
                 _allocate(t, e) {
@@ -25258,15 +25261,15 @@
                 _forEachGeometry(t, e, n) {
                     const {
                         data: i,
                         getGeometry: r
                     } = this, {
                         iterable: s,
                         objectInfo: o
-                    } = av(i, e, n);
+                    } = lv(i, e, n);
                     for (const e of s) o.index++, t(r ? r(e, o) : null, o.index)
                 }
                 _rebuildGeometry(t) {
                     if (!this.data) return;
                     let {
                         indexStarts: e,
                         vertexStarts: n,
@@ -25280,15 +25283,15 @@
                         endRow: a = 1 / 0
                     } = t || {}, l = {};
                     if (t || (e = [0], n = [0]), this.normalize || !s) this._forEachGeometry(((t, e) => {
                         const i = t && this.normalizeGeometry(t);
                         l[e] = i, n[e + 1] = n[e] + (i ? this.getGeometrySize(i) : 0)
                     }), o, a), i = n[n.length - 1];
                     else if (n = r.startIndices, i = n[r.length] || 0, ArrayBuffer.isView(s)) i = i || s.length / this.positionSize;
-                    else if (s instanceof Wd) {
+                    else if (s instanceof Hd) {
                         const t = s.accessor.stride || 4 * this.positionSize;
                         i = i || s.byteLength / t
                     } else if (s.buffer) {
                         const t = s.stride || 4 * this.positionSize;
                         i = i || s.buffer.byteLength / t
                     } else if (s.value) {
                         const t = s.value,
@@ -25302,15 +25305,15 @@
                         c.vertexStart = n[r], c.indexStart = e[r];
                         const o = r < n.length - 1 ? n[r + 1] : i;
                         c.geometrySize = o - n[r], c.geometryIndex = r, this.updateGeometryAttributes(s, c)
                     }), o, a), this.vertexCount = e[e.length - 1]
                 }
             }
 
-            function Gy(t, e, n = {}) {
+            function Wy(t, e, n = {}) {
                 const i = function(t, e = {}) {
                     return Math.sign(function(t, e = {}) {
                         const {
                             start: n = 0,
                             end: i = t.length
                         } = e, r = e.size || 2;
                         let s = 0;
@@ -25331,92 +25334,92 @@
                             const n = t[i + e];
                             t[i + e] = t[o + e], t[o + e] = n
                         }
                     }
                 }(t, n), !0)
             }
 
-            function Wy(t, e, n, i, r = []) {
+            function Hy(t, e, n, i, r = []) {
                 let s, o;
                 if (8 & n) s = (i[3] - t[1]) / (e[1] - t[1]), o = 3;
                 else if (4 & n) s = (i[1] - t[1]) / (e[1] - t[1]), o = 1;
                 else if (2 & n) s = (i[2] - t[0]) / (e[0] - t[0]), o = 2;
                 else {
                     if (!(1 & n)) return null;
                     s = (i[0] - t[0]) / (e[0] - t[0]), o = 0
                 }
                 for (let n = 0; n < t.length; n++) r[n] = (1 & o) === n ? i[o] : s * (e[n] - t[n]) + t[n];
                 return r
             }
 
-            function Hy(t, e) {
+            function Zy(t, e) {
                 let n = 0;
                 return t[0] < e[0] ? n |= 1 : t[0] > e[2] && (n |= 2), t[1] < e[1] ? n |= 4 : t[1] > e[3] && (n |= 8), n
             }
 
-            function Zy(t, e) {
+            function qy(t, e) {
                 const n = e.length,
                     i = t.length;
                 if (i > 0) {
                     let r = !0;
                     for (let s = 0; s < n; s++)
                         if (t[i - n + s] !== e[s]) {
                             r = !1;
                             break
                         } if (r) return !1
                 }
                 for (let r = 0; r < n; r++) t[i + r] = e[r];
                 return !0
             }
 
-            function qy(t, e) {
+            function Xy(t, e) {
                 const n = e.length;
                 for (let i = 0; i < n; i++) t[i] = e[i]
             }
 
-            function Xy(t, e, n, i, r = []) {
+            function Yy(t, e, n, i, r = []) {
                 const s = i + e * n;
                 for (let e = 0; e < n; e++) r[e] = t[s + e];
                 return r
             }
 
-            function Yy(t, e) {
+            function Ky(t, e) {
                 const {
                     size: n = 2,
                     broken: i = !1,
                     gridResolution: r = 10,
                     gridOffset: s = [0, 0],
                     startIndex: o = 0,
                     endIndex: a = t.length
                 } = e || {}, l = (a - o) / n;
                 let c = [];
                 const h = [c],
-                    u = Xy(t, 0, n, o);
+                    u = Yy(t, 0, n, o);
                 let d, p;
-                const f = t_(u, r, s, []),
+                const f = e_(u, r, s, []),
                     g = [];
-                Zy(c, u);
+                qy(c, u);
                 for (let e = 1; e < l; e++) {
-                    for (d = Xy(t, e, n, o, d), p = Hy(d, f); p;) {
-                        Wy(u, d, p, f, g);
-                        const t = Hy(g, f);
-                        t && (Wy(u, g, t, f, g), p = t), Zy(c, g), qy(u, g), e_(f, r, p), i && c.length > n && (c = [], h.push(c), Zy(c, u)), p = Hy(d, f)
+                    for (d = Yy(t, e, n, o, d), p = Zy(d, f); p;) {
+                        Hy(u, d, p, f, g);
+                        const t = Zy(g, f);
+                        t && (Hy(u, g, t, f, g), p = t), qy(c, g), Xy(u, g), n_(f, r, p), i && c.length > n && (c = [], h.push(c), qy(c, u)), p = Zy(d, f)
                     }
-                    Zy(c, d), qy(u, d)
+                    qy(c, d), Xy(u, d)
                 }
                 return i ? h : h[0]
             }
-            const Ky = 0;
+            const Qy = 0;
 
-            function Qy(t, e) {
+            function Jy(t, e) {
                 for (let n = 0; n < e.length; n++) t.push(e[n]);
                 return t
             }
 
-            function Jy(t, e = null, n) {
+            function $y(t, e = null, n) {
                 if (!t.length) return [];
                 const {
                     size: i = 2,
                     gridResolution: r = 10,
                     gridOffset: s = [0, 0],
                     edgeTypes: o = !1
                 } = n || {}, a = [], l = [{
@@ -25430,123 +25433,123 @@
                 let h = [];
                 for (; l.length;) {
                     const {
                         pos: t,
                         types: e,
                         holes: n
                     } = l.shift();
-                    n_(t, i, n[0] || t.length, c), h = t_(c[0], r, s, h);
-                    const u = Hy(c[1], h);
+                    i_(t, i, n[0] || t.length, c), h = e_(c[0], r, s, h);
+                    const u = Zy(c[1], h);
                     if (u) {
-                        let r = $y(t, e, i, 0, n[0] || t.length, h, u);
+                        let r = t_(t, e, i, 0, n[0] || t.length, h, u);
                         const s = {
                                 pos: r[0].pos,
                                 types: r[0].types,
                                 holes: []
                             },
                             a = {
                                 pos: r[1].pos,
                                 types: r[1].types,
                                 holes: []
                             };
                         l.push(s, a);
-                        for (let l = 0; l < n.length; l++) r = $y(t, e, i, n[l], n[l + 1] || t.length, h, u), r[0] && (s.holes.push(s.pos.length), s.pos = Qy(s.pos, r[0].pos), o && (s.types = Qy(s.types, r[0].types))), r[1] && (a.holes.push(a.pos.length), a.pos = Qy(a.pos, r[1].pos), o && (a.types = Qy(a.types, r[1].types)))
+                        for (let l = 0; l < n.length; l++) r = t_(t, e, i, n[l], n[l + 1] || t.length, h, u), r[0] && (s.holes.push(s.pos.length), s.pos = Jy(s.pos, r[0].pos), o && (s.types = Jy(s.types, r[0].types))), r[1] && (a.holes.push(a.pos.length), a.pos = Jy(a.pos, r[1].pos), o && (a.types = Jy(a.types, r[1].types)))
                     } else {
                         const i = {
                             positions: t
                         };
                         o && (i.edgeTypes = e), n.length && (i.holeIndices = n), a.push(i)
                     }
                 }
                 return a
             }
 
-            function $y(t, e, n, i, r, s, o) {
+            function t_(t, e, n, i, r, s, o) {
                 const a = (r - i) / n,
                     l = [],
                     c = [],
                     h = [],
                     u = [],
                     d = [];
                 let p, f, g;
-                const m = Xy(t, a - 1, n, i);
+                const m = Yy(t, a - 1, n, i);
                 let v = Math.sign(8 & o ? m[1] - s[3] : m[0] - s[2]),
                     b = e && e[a - 1],
                     y = 0,
                     _ = 0;
-                for (let r = 0; r < a; r++) p = Xy(t, r, n, i, p), f = Math.sign(8 & o ? p[1] - s[3] : p[0] - s[2]), g = e && e[i / n + r], f && v && v !== f && (Wy(m, p, o, s, d), Zy(l, d) && h.push(b), Zy(c, d) && u.push(b)), f <= 0 ? (Zy(l, p) && h.push(g), y -= f) : h.length && (h[h.length - 1] = Ky), f >= 0 ? (Zy(c, p) && u.push(g), _ += f) : u.length && (u[u.length - 1] = Ky), qy(m, p), v = f, b = g;
+                for (let r = 0; r < a; r++) p = Yy(t, r, n, i, p), f = Math.sign(8 & o ? p[1] - s[3] : p[0] - s[2]), g = e && e[i / n + r], f && v && v !== f && (Hy(m, p, o, s, d), qy(l, d) && h.push(b), qy(c, d) && u.push(b)), f <= 0 ? (qy(l, p) && h.push(g), y -= f) : h.length && (h[h.length - 1] = Qy), f >= 0 ? (qy(c, p) && u.push(g), _ += f) : u.length && (u[u.length - 1] = Qy), Xy(m, p), v = f, b = g;
                 return [y ? {
                     pos: l,
                     types: e && h
                 } : null, _ ? {
                     pos: c,
                     types: e && u
                 } : null]
             }
 
-            function t_(t, e, n, i) {
+            function e_(t, e, n, i) {
                 const r = Math.floor((t[0] - n[0]) / e) * e + n[0],
                     s = Math.floor((t[1] - n[1]) / e) * e + n[1];
                 return i[0] = r, i[1] = s, i[2] = r + e, i[3] = s + e, i
             }
 
-            function e_(t, e, n) {
+            function n_(t, e, n) {
                 8 & n ? (t[1] += e, t[3] += e) : 4 & n ? (t[1] -= e, t[3] -= e) : 2 & n ? (t[0] += e, t[2] += e) : 1 & n && (t[0] -= e, t[2] -= e)
             }
 
-            function n_(t, e, n, i) {
+            function i_(t, e, n, i) {
                 let r = 1 / 0,
                     s = -1 / 0,
                     o = 1 / 0,
                     a = -1 / 0;
                 for (let i = 0; i < n; i += e) {
                     const e = t[i],
                         n = t[i + 1];
                     r = e < r ? e : r, s = e > s ? e : s, o = n < o ? n : o, a = n > a ? n : a
                 }
                 return i[0][0] = r, i[0][1] = o, i[1][0] = s, i[1][1] = a, i
             }
 
-            function i_(t, e, n, i) {
+            function r_(t, e, n, i) {
                 let r = -1,
                     s = -1;
                 for (let o = n + 1; o < i; o += e) {
                     const e = Math.abs(t[o]);
                     e > r && (r = e, s = o - 1)
                 }
                 return s
             }
 
-            function r_(t, e, n, i, r = 85.051129) {
+            function s_(t, e, n, i, r = 85.051129) {
                 const s = t[n],
                     o = t[i - e];
                 if (Math.abs(s - o) > 180) {
-                    const i = Xy(t, 0, e, n);
-                    i[0] += 360 * Math.round((o - s) / 360), Zy(t, i), i[1] = Math.sign(i[1]) * r, Zy(t, i), i[0] = s, Zy(t, i)
+                    const i = Yy(t, 0, e, n);
+                    i[0] += 360 * Math.round((o - s) / 360), qy(t, i), i[1] = Math.sign(i[1]) * r, qy(t, i), i[0] = s, qy(t, i)
                 }
             }
 
-            function s_(t, e, n, i) {
+            function o_(t, e, n, i) {
                 let r, s = t[0];
                 for (let o = n; o < i; o += e) {
                     r = t[o];
                     const e = r - s;
                     (e > 180 || e < -180) && (r -= 360 * Math.round(e / 360)), t[o] = s = r
                 }
             }
 
-            function o_(t, e) {
+            function a_(t, e) {
                 let n;
                 const i = t.length / e;
                 for (let r = 0; r < i && (n = t[r * e], (n + 180) % 360 == 0); r++);
                 const r = 360 * -Math.round(n / 360);
                 if (0 !== r)
                     for (let n = 0; n < i; n++) t[n * e] += r
             }
-            class a_ extends Uy {
+            class l_ extends Gy {
                 constructor(t) {
                     super({
                         ...t,
                         attributes: {
                             positions: {
                                 size: 3,
                                 padding: 18,
@@ -25571,51 +25574,51 @@
                         let r;
                         if (Array.isArray(t[0])) {
                             const n = t.length * e;
                             r = new Array(n);
                             for (let n = 0; n < t.length; n++)
                                 for (let i = 0; i < e; i++) r[n * e + i] = t[n][i] || 0
                         } else r = t;
-                        return n ? Yy(r, {
+                        return n ? Ky(r, {
                             size: e,
                             gridResolution: n
                         }) : i ? function(t, e) {
                             const {
                                 size: n = 2,
                                 startIndex: i = 0,
                                 endIndex: r = t.length,
                                 normalize: s = !0
                             } = e || {}, o = t.slice(i, r);
-                            s_(o, n, 0, r - i);
-                            const a = Yy(o, {
+                            o_(o, n, 0, r - i);
+                            const a = Ky(o, {
                                 size: n,
                                 broken: !0,
                                 gridResolution: 360,
                                 gridOffset: [-180, -180]
                             });
                             if (s)
-                                for (const t of a) o_(t, n);
+                                for (const t of a) a_(t, n);
                             return a
                         }(r, {
                             size: e
                         }) : r
                     }(t, this.positionSize, this.opts.resolution, this.opts.wrapLongitude) : t
                 }
                 getGeometrySize(t) {
-                    if (l_(t)) {
+                    if (c_(t)) {
                         let e = 0;
                         for (const n of t) e += this.getGeometrySize(n);
                         return e
                     }
                     const e = this.getPathLength(t);
                     return e < 2 ? 0 : this.isClosed(t) ? e < 3 ? 0 : e + 2 : e
                 }
                 updateGeometryAttributes(t, e) {
                     if (0 !== e.geometrySize)
-                        if (t && l_(t))
+                        if (t && c_(t))
                             for (const n of t) {
                                 const t = this.getGeometrySize(n);
                                 e.geometrySize = t, this.updateGeometryAttributes(n, e), e.vertexStart += t
                             } else this._updateSegmentTypes(t, e), this._updatePositions(t, e)
                 }
                 _updateSegmentTypes(t, e) {
                     const n = this.attributes.segmentTypes,
@@ -25653,19 +25656,19 @@
                     const {
                         positionSize: e
                     } = this, n = t.length - e;
                     return t[0] === t[n] && t[1] === t[n + 1] && (2 === e || t[2] === t[n + 2])
                 }
             }
 
-            function l_(t) {
+            function c_(t) {
                 return Array.isArray(t[0])
             }
-            const c_ = [0, 0, 0, 255],
-                h_ = {
+            const h_ = [0, 0, 0, 255],
+                u_ = {
                     widthUnits: "meters",
                     widthScale: {
                         type: "number",
                         min: 0,
                         value: 1
                     },
                     widthMinPixels: {
@@ -25689,49 +25692,49 @@
                     _pathType: null,
                     getPath: {
                         type: "accessor",
                         value: t => t.path
                     },
                     getColor: {
                         type: "accessor",
-                        value: c_
+                        value: h_
                     },
                     getWidth: {
                         type: "accessor",
                         value: 1
                     },
                     rounded: {
                         deprecatedFor: ["jointRounded", "capRounded"]
                     }
                 },
-                u_ = {
+                d_ = {
                     enter: (t, e) => e.length ? e.subarray(e.length - t.length) : t
                 };
-            class d_ extends Fb {
+            class p_ extends zb {
                 constructor(...t) {
                     super(...t), wo(this, "state", void 0)
                 }
                 getShaders() {
                     return super.getShaders({
                         vs: "#define SHADER_NAME path-layer-vertex-shader\n\nattribute vec2 positions;\n\nattribute float instanceTypes;\nattribute vec3 instanceStartPositions;\nattribute vec3 instanceEndPositions;\nattribute vec3 instanceLeftPositions;\nattribute vec3 instanceRightPositions;\nattribute vec3 instanceLeftPositions64Low;\nattribute vec3 instanceStartPositions64Low;\nattribute vec3 instanceEndPositions64Low;\nattribute vec3 instanceRightPositions64Low;\nattribute float instanceStrokeWidths;\nattribute vec4 instanceColors;\nattribute vec3 instancePickingColors;\n\nuniform float widthScale;\nuniform float widthMinPixels;\nuniform float widthMaxPixels;\nuniform float jointType;\nuniform float capType;\nuniform float miterLimit;\nuniform bool billboard;\nuniform int widthUnits;\n\nuniform float opacity;\n\nvarying vec4 vColor;\nvarying vec2 vCornerOffset;\nvarying float vMiterLength;\nvarying vec2 vPathPosition;\nvarying float vPathLength;\nvarying float vJointType;\n\nconst float EPSILON = 0.001;\nconst vec3 ZERO_OFFSET = vec3(0.0);\n\nfloat flipIfTrue(bool flag) {\n  return -(float(flag) * 2. - 1.);\n}\nvec3 getLineJoinOffset(\n  vec3 prevPoint, vec3 currPoint, vec3 nextPoint,\n  vec2 width\n) {\n  bool isEnd = positions.x > 0.0;\n  float sideOfPath = positions.y;\n  float isJoint = float(sideOfPath == 0.0);\n\n  vec3 deltaA3 = (currPoint - prevPoint);\n  vec3 deltaB3 = (nextPoint - currPoint);\n\n  mat3 rotationMatrix;\n  bool needsRotation = !billboard && project_needs_rotation(currPoint, rotationMatrix);\n  if (needsRotation) {\n    deltaA3 = deltaA3 * rotationMatrix;\n    deltaB3 = deltaB3 * rotationMatrix;\n  }\n  vec2 deltaA = deltaA3.xy / width;\n  vec2 deltaB = deltaB3.xy / width;\n\n  float lenA = length(deltaA);\n  float lenB = length(deltaB);\n\n  vec2 dirA = lenA > 0. ? normalize(deltaA) : vec2(0.0, 0.0);\n  vec2 dirB = lenB > 0. ? normalize(deltaB) : vec2(0.0, 0.0);\n\n  vec2 perpA = vec2(-dirA.y, dirA.x);\n  vec2 perpB = vec2(-dirB.y, dirB.x);\n  vec2 tangent = dirA + dirB;\n  tangent = length(tangent) > 0. ? normalize(tangent) : perpA;\n  vec2 miterVec = vec2(-tangent.y, tangent.x);\n  vec2 dir = isEnd ? dirA : dirB;\n  vec2 perp = isEnd ? perpA : perpB;\n  float L = isEnd ? lenA : lenB;\n  float sinHalfA = abs(dot(miterVec, perp));\n  float cosHalfA = abs(dot(dirA, miterVec));\n  float turnDirection = flipIfTrue(dirA.x * dirB.y >= dirA.y * dirB.x);\n  float cornerPosition = sideOfPath * turnDirection;\n\n  float miterSize = 1.0 / max(sinHalfA, EPSILON);\n  miterSize = mix(\n    min(miterSize, max(lenA, lenB) / max(cosHalfA, EPSILON)),\n    miterSize,\n    step(0.0, cornerPosition)\n  );\n\n  vec2 offsetVec = mix(miterVec * miterSize, perp, step(0.5, cornerPosition))\n    * (sideOfPath + isJoint * turnDirection);\n  bool isStartCap = lenA == 0.0 || (!isEnd && (instanceTypes == 1.0 || instanceTypes == 3.0));\n  bool isEndCap = lenB == 0.0 || (isEnd && (instanceTypes == 2.0 || instanceTypes == 3.0));\n  bool isCap = isStartCap || isEndCap;\n  if (isCap) {\n    offsetVec = mix(perp * sideOfPath, dir * capType * 4.0 * flipIfTrue(isStartCap), isJoint);\n    vJointType = capType;\n  } else {\n    vJointType = jointType;\n  }\n  vPathLength = L;\n  vCornerOffset = offsetVec;\n  vMiterLength = dot(vCornerOffset, miterVec * turnDirection);\n  vMiterLength = isCap ? isJoint : vMiterLength;\n\n  vec2 offsetFromStartOfPath = vCornerOffset + deltaA * float(isEnd);\n  vPathPosition = vec2(\n    dot(offsetFromStartOfPath, perp),\n    dot(offsetFromStartOfPath, dir)\n  );\n  geometry.uv = vPathPosition;\n\n  float isValid = step(instanceTypes, 3.5);\n  vec3 offset = vec3(offsetVec * width * isValid, 0.0);\n\n  if (needsRotation) {\n    offset = rotationMatrix * offset;\n  }\n  return offset;\n}\nvoid clipLine(inout vec4 position, vec4 refPosition) {\n  if (position.w < EPSILON) {\n    float r = (EPSILON - refPosition.w) / (position.w - refPosition.w);\n    position = refPosition + (position - refPosition) * r;\n  }\n}\n\nvoid main() {\n  geometry.pickingColor = instancePickingColors;\n\n  vColor = vec4(instanceColors.rgb, instanceColors.a * opacity);\n\n  float isEnd = positions.x;\n\n  vec3 prevPosition = mix(instanceLeftPositions, instanceStartPositions, isEnd);\n  vec3 prevPosition64Low = mix(instanceLeftPositions64Low, instanceStartPositions64Low, isEnd);\n\n  vec3 currPosition = mix(instanceStartPositions, instanceEndPositions, isEnd);\n  vec3 currPosition64Low = mix(instanceStartPositions64Low, instanceEndPositions64Low, isEnd);\n\n  vec3 nextPosition = mix(instanceEndPositions, instanceRightPositions, isEnd);\n  vec3 nextPosition64Low = mix(instanceEndPositions64Low, instanceRightPositions64Low, isEnd);\n\n  geometry.worldPosition = currPosition;\n  vec2 widthPixels = vec2(clamp(\n    project_size_to_pixel(instanceStrokeWidths * widthScale, widthUnits),\n    widthMinPixels, widthMaxPixels) / 2.0);\n  vec3 width;\n\n  if (billboard) {\n    vec4 prevPositionScreen = project_position_to_clipspace(prevPosition, prevPosition64Low, ZERO_OFFSET);\n    vec4 currPositionScreen = project_position_to_clipspace(currPosition, currPosition64Low, ZERO_OFFSET, geometry.position);\n    vec4 nextPositionScreen = project_position_to_clipspace(nextPosition, nextPosition64Low, ZERO_OFFSET);\n\n    clipLine(prevPositionScreen, currPositionScreen);\n    clipLine(nextPositionScreen, currPositionScreen);\n    clipLine(currPositionScreen, mix(nextPositionScreen, prevPositionScreen, isEnd));\n\n    width = vec3(widthPixels, 0.0);\n    DECKGL_FILTER_SIZE(width, geometry);\n\n    vec3 offset = getLineJoinOffset(\n      prevPositionScreen.xyz / prevPositionScreen.w,\n      currPositionScreen.xyz / currPositionScreen.w,\n      nextPositionScreen.xyz / nextPositionScreen.w,\n      project_pixel_size_to_clipspace(width.xy)\n    );\n\n    DECKGL_FILTER_GL_POSITION(currPositionScreen, geometry);\n    gl_Position = vec4(currPositionScreen.xyz + offset * currPositionScreen.w, currPositionScreen.w);\n  } else {\n    prevPosition = project_position(prevPosition, prevPosition64Low);\n    currPosition = project_position(currPosition, currPosition64Low);\n    nextPosition = project_position(nextPosition, nextPosition64Low);\n\n    width = vec3(project_pixel_size(widthPixels), 0.0);\n    DECKGL_FILTER_SIZE(width, geometry);\n\n    vec3 offset = getLineJoinOffset(prevPosition, currPosition, nextPosition, width.xy);\n    geometry.position = vec4(currPosition + offset, 1.0);\n    gl_Position = project_common_position_to_clipspace(geometry.position);\n    DECKGL_FILTER_GL_POSITION(gl_Position, geometry);\n  }\n  DECKGL_FILTER_COLOR(vColor, geometry);\n}\n",
                         fs: "#define SHADER_NAME path-layer-fragment-shader\n\nprecision highp float;\n\nuniform float miterLimit;\n\nvarying vec4 vColor;\nvarying vec2 vCornerOffset;\nvarying float vMiterLength;\nvarying vec2 vPathPosition;\nvarying float vPathLength;\nvarying float vJointType;\n\nvoid main(void) {\n  geometry.uv = vPathPosition;\n\n  if (vPathPosition.y < 0.0 || vPathPosition.y > vPathLength) {\n    if (vJointType > 0.5 && length(vCornerOffset) > 1.0) {\n      discard;\n    }\n    if (vJointType < 0.5 && vMiterLength > miterLimit + 1.0) {\n      discard;\n    }\n  }\n  gl_FragColor = vColor;\n\n  DECKGL_FILTER_COLOR(gl_FragColor, geometry);\n}\n",
-                        modules: [ty, ny]
+                        modules: [ey, iy]
                     })
                 }
                 get wrapLongitude() {
                     return !1
                 }
                 initializeState() {
                     this.getAttributeManager().addInstanced({
                         positions: {
                             size: 3,
                             vertexOffset: 1,
                             type: 5130,
                             fp64: this.use64bitPositions(),
-                            transition: u_,
+                            transition: d_,
                             accessor: "getPath",
                             update: this.calculatePositions,
                             noAlloc: !0,
                             shaderAttributes: {
                                 instanceLeftPositions: {
                                     vertexOffset: 0
                                 },
@@ -25751,35 +25754,35 @@
                             type: 5121,
                             update: this.calculateSegmentTypes,
                             noAlloc: !0
                         },
                         instanceStrokeWidths: {
                             size: 1,
                             accessor: "getWidth",
-                            transition: u_,
+                            transition: d_,
                             defaultValue: 1
                         },
                         instanceColors: {
                             size: this.props.colorFormat.length,
                             type: 5121,
                             normalized: !0,
                             accessor: "getColor",
-                            transition: u_,
-                            defaultValue: c_
+                            transition: d_,
+                            defaultValue: h_
                         },
                         instancePickingColors: {
                             size: 3,
                             type: 5121,
                             accessor: (t, {
                                 index: e,
                                 target: n
                             }) => this.encodePickingColor(t && t.__source ? t.__source.index : e, n)
                         }
                     }), this.setState({
-                        pathTesselator: new a_({
+                        pathTesselator: new l_({
                             fp64: this.use64bitPositions()
                         })
                     })
                 }
                 updateState(t) {
                     super.updateState(t);
                     const {
@@ -25853,18 +25856,18 @@
                         widthScale: o,
                         miterLimit: r,
                         widthMinPixels: a,
                         widthMaxPixels: l
                     }).draw()
                 }
                 _getModel(t) {
-                    return new Yv(t, {
+                    return new Kv(t, {
                         ...this.getShaders(),
                         id: this.props.id,
-                        geometry: new ry({
+                        geometry: new sy({
                             drawMode: 4,
                             attributes: {
                                 indices: new Uint16Array([0, 1, 2, 1, 4, 2, 1, 3, 4, 3, 5, 4]),
                                 positions: {
                                     value: new Float32Array([0, 0, 0, -1, 0, 1, 1, -1, 1, 1, 1, 0]),
                                     size: 2
                                 }
@@ -25882,53 +25885,53 @@
                 calculateSegmentTypes(t) {
                     const {
                         pathTesselator: e
                     } = this.state;
                     t.startIndices = e.vertexStarts, t.value = e.get("segmentTypes")
                 }
             }
-            wo(d_, "defaultProps", h_), wo(d_, "layerName", "PathLayer");
-            const p_ = "#if (defined(SHADER_TYPE_FRAGMENT) && defined(LIGHTING_FRAGMENT)) || (defined(SHADER_TYPE_VERTEX) && defined(LIGHTING_VERTEX))\n\nstruct AmbientLight {\n vec3 color;\n};\n\nstruct PointLight {\n vec3 color;\n vec3 position;\n vec3 attenuation;\n};\n\nstruct DirectionalLight {\n  vec3 color;\n  vec3 direction;\n};\n\nuniform AmbientLight lighting_uAmbientLight;\nuniform PointLight lighting_uPointLight[MAX_LIGHTS];\nuniform DirectionalLight lighting_uDirectionalLight[MAX_LIGHTS];\nuniform int lighting_uPointLightCount;\nuniform int lighting_uDirectionalLightCount;\n\nuniform bool lighting_uEnabled;\n\nfloat getPointLightAttenuation(PointLight pointLight, float distance) {\n  return pointLight.attenuation.x\n       + pointLight.attenuation.y * distance\n       + pointLight.attenuation.z * distance * distance;\n}\n\n#endif\n",
-                f_ = {
+            wo(p_, "defaultProps", u_), wo(p_, "layerName", "PathLayer");
+            const f_ = "#if (defined(SHADER_TYPE_FRAGMENT) && defined(LIGHTING_FRAGMENT)) || (defined(SHADER_TYPE_VERTEX) && defined(LIGHTING_VERTEX))\n\nstruct AmbientLight {\n vec3 color;\n};\n\nstruct PointLight {\n vec3 color;\n vec3 position;\n vec3 attenuation;\n};\n\nstruct DirectionalLight {\n  vec3 color;\n  vec3 direction;\n};\n\nuniform AmbientLight lighting_uAmbientLight;\nuniform PointLight lighting_uPointLight[MAX_LIGHTS];\nuniform DirectionalLight lighting_uDirectionalLight[MAX_LIGHTS];\nuniform int lighting_uPointLightCount;\nuniform int lighting_uDirectionalLightCount;\n\nuniform bool lighting_uEnabled;\n\nfloat getPointLightAttenuation(PointLight pointLight, float distance) {\n  return pointLight.attenuation.x\n       + pointLight.attenuation.y * distance\n       + pointLight.attenuation.z * distance * distance;\n}\n\n#endif\n",
+                g_ = {
                     lightSources: {}
                 };
 
-            function g_() {
+            function m_() {
                 let {
                     color: t = [0, 0, 0],
                     intensity: e = 1
                 } = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                 return t.map((t => t * e / 255))
             }
-            const m_ = {};
-            const v_ = {
+            const v_ = {};
+            const b_ = {
                 name: "gouraud-lighting",
                 dependencies: [{
                     name: "lights",
-                    vs: p_,
-                    fs: p_,
+                    vs: f_,
+                    fs: f_,
                     getUniforms: function t() {
-                        let e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : f_;
+                        let e = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : g_;
                         if ("lightSources" in e) {
                             const {
                                 ambientLight: t,
                                 pointLights: n,
                                 directionalLights: i
                             } = e.lightSources || {};
                             return t || n && n.length > 0 || i && i.length > 0 ? Object.assign({}, function(t) {
                                 let {
                                     ambientLight: e,
                                     pointLights: n = [],
                                     directionalLights: i = []
                                 } = t;
                                 const r = {};
-                                return r["lighting_uAmbientLight.color"] = e ? g_(e) : [0, 0, 0], n.forEach(((t, e) => {
-                                    r["lighting_uPointLight[".concat(e, "].color")] = g_(t), r["lighting_uPointLight[".concat(e, "].position")] = t.position, r["lighting_uPointLight[".concat(e, "].attenuation")] = t.attenuation || [1, 0, 0]
+                                return r["lighting_uAmbientLight.color"] = e ? m_(e) : [0, 0, 0], n.forEach(((t, e) => {
+                                    r["lighting_uPointLight[".concat(e, "].color")] = m_(t), r["lighting_uPointLight[".concat(e, "].position")] = t.position, r["lighting_uPointLight[".concat(e, "].attenuation")] = t.attenuation || [1, 0, 0]
                                 })), r.lighting_uPointLightCount = n.length, i.forEach(((t, e) => {
-                                    r["lighting_uDirectionalLight[".concat(e, "].color")] = g_(t), r["lighting_uDirectionalLight[".concat(e, "].direction")] = t.direction
+                                    r["lighting_uDirectionalLight[".concat(e, "].color")] = m_(t), r["lighting_uDirectionalLight[".concat(e, "].direction")] = t.direction
                                 })), r.lighting_uDirectionalLightCount = i.length, r
                             }({
                                 ambientLight: t,
                                 pointLights: n,
                                 directionalLights: i
                             }), {
                                 lighting_uEnabled: !0
@@ -25962,15 +25965,15 @@
                     }
                 }],
                 vs: "\nuniform float lighting_uAmbient;\nuniform float lighting_uDiffuse;\nuniform float lighting_uShininess;\nuniform vec3  lighting_uSpecularColor;\n\nvec3 lighting_getLightColor(vec3 surfaceColor, vec3 light_direction, vec3 view_direction, vec3 normal_worldspace, vec3 color) {\n    vec3 halfway_direction = normalize(light_direction + view_direction);\n    float lambertian = dot(light_direction, normal_worldspace);\n    float specular = 0.0;\n    if (lambertian > 0.0) {\n      float specular_angle = max(dot(normal_worldspace, halfway_direction), 0.0);\n      specular = pow(specular_angle, lighting_uShininess);\n    }\n    lambertian = max(lambertian, 0.0);\n    return (lambertian * lighting_uDiffuse * surfaceColor + specular * lighting_uSpecularColor) * color;\n}\n\nvec3 lighting_getLightColor(vec3 surfaceColor, vec3 cameraPosition, vec3 position_worldspace, vec3 normal_worldspace) {\n  vec3 lightColor = surfaceColor;\n\n  if (lighting_uEnabled) {\n    vec3 view_direction = normalize(cameraPosition - position_worldspace);\n    lightColor = lighting_uAmbient * surfaceColor * lighting_uAmbientLight.color;\n\n    for (int i = 0; i < MAX_LIGHTS; i++) {\n      if (i >= lighting_uPointLightCount) {\n        break;\n      }\n      PointLight pointLight = lighting_uPointLight[i];\n      vec3 light_position_worldspace = pointLight.position;\n      vec3 light_direction = normalize(light_position_worldspace - position_worldspace);\n      lightColor += lighting_getLightColor(surfaceColor, light_direction, view_direction, normal_worldspace, pointLight.color);\n    }\n\n    for (int i = 0; i < MAX_LIGHTS; i++) {\n      if (i >= lighting_uDirectionalLightCount) {\n        break;\n      }\n      DirectionalLight directionalLight = lighting_uDirectionalLight[i];\n      lightColor += lighting_getLightColor(surfaceColor, -directionalLight.direction, view_direction, normal_worldspace, directionalLight.color);\n    }\n  }\n  return lightColor;\n}\n\nvec3 lighting_getSpecularLightColor(vec3 cameraPosition, vec3 position_worldspace, vec3 normal_worldspace) {\n  vec3 lightColor = vec3(0, 0, 0);\n  vec3 surfaceColor = vec3(0, 0, 0);\n\n  if (lighting_uEnabled) {\n    vec3 view_direction = normalize(cameraPosition - position_worldspace);\n\n    for (int i = 0; i < MAX_LIGHTS; i++) {\n      if (i >= lighting_uPointLightCount) {\n        break;\n      }\n      PointLight pointLight = lighting_uPointLight[i];\n      vec3 light_position_worldspace = pointLight.position;\n      vec3 light_direction = normalize(light_position_worldspace - position_worldspace);\n      lightColor += lighting_getLightColor(surfaceColor, light_direction, view_direction, normal_worldspace, pointLight.color);\n    }\n\n    for (int i = 0; i < MAX_LIGHTS; i++) {\n      if (i >= lighting_uDirectionalLightCount) {\n        break;\n      }\n      DirectionalLight directionalLight = lighting_uDirectionalLight[i];\n      lightColor += lighting_getLightColor(surfaceColor, -directionalLight.direction, view_direction, normal_worldspace, directionalLight.color);\n    }\n  }\n  return lightColor;\n}\n",
                 defines: {
                     LIGHTING_VERTEX: 1
                 },
                 getUniforms: function() {
-                    let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : m_;
+                    let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : v_;
                     if (!("material" in t)) return {};
                     const {
                         material: e
                     } = t;
                     return e ? function(t) {
                         const {
                             ambient: e = .35,
@@ -25985,77 +25988,77 @@
                             lighting_uSpecularColor: r.map((t => t / 255))
                         }
                     }(e) : {
                         lighting_uEnabled: !1
                     }
                 }
             };
-            var b_ = n(9187),
-                y_ = n.n(b_);
-            const __ = {
+            var y_ = n(9187),
+                __ = n.n(y_);
+            const x_ = {
                 isClosed: !0
             };
 
-            function x_(t) {
+            function w_(t) {
                 return "positions" in t ? t.positions : t
             }
 
-            function w_(t) {
+            function E_(t) {
                 return "holeIndices" in t ? t.holeIndices : null
             }
 
-            function E_(t, e, n, i, r) {
+            function P_(t, e, n, i, r) {
                 let s = e;
                 const o = n.length;
                 for (let e = 0; e < o; e++)
                     for (let r = 0; r < i; r++) t[s++] = n[e][r] || 0;
                 if (! function(t) {
                         const e = t[0],
                             n = t[t.length - 1];
                         return e[0] === n[0] && e[1] === n[1] && e[2] === n[2]
                     }(n))
                     for (let e = 0; e < i; e++) t[s++] = n[0][e] || 0;
-                return __.start = e, __.end = s, __.size = i, Gy(t, r, __), s
+                return x_.start = e, x_.end = s, x_.size = i, Wy(t, r, x_), s
             }
 
-            function P_(t, e, n, i, r = 0, s, o) {
+            function S_(t, e, n, i, r = 0, s, o) {
                 const a = (s = s || n.length) - r;
                 if (a <= 0) return e;
                 let l = e;
                 for (let e = 0; e < a; e++) t[l++] = n[r + e];
                 if (! function(t, e, n, i) {
                         for (let r = 0; r < e; r++)
                             if (t[n + r] !== t[i - e + r]) return !1;
                         return !0
                     }(n, i, r, s))
                     for (let e = 0; e < i; e++) t[l++] = n[r + e];
-                return __.start = e, __.end = l, __.size = i, Gy(t, o, __), l
+                return x_.start = e, x_.end = l, x_.size = i, Wy(t, o, x_), l
             }
 
-            function S_(t, e, n) {
+            function C_(t, e, n) {
                 const i = t.length / 3;
                 let r = 0;
                 for (let s = 0; s < i; s++) {
                     const o = (s + 1) % i;
                     r += t[3 * s + e] * t[3 * o + n], r -= t[3 * o + e] * t[3 * s + n]
                 }
                 return Math.abs(r / 2)
             }
 
-            function C_(t, e, n, i) {
+            function T_(t, e, n, i) {
                 const r = t.length / 3;
                 for (let s = 0; s < r; s++) {
                     const r = 3 * s,
                         o = t[r + 0],
                         a = t[r + 1],
                         l = t[r + 2];
                     t[r + e] = o, t[r + n] = a, t[r + i] = l
                 }
             }
-            class T_ extends Uy {
+            class A_ extends Gy {
                 constructor(t) {
                     const {
                         fp64: e,
                         IndexType: n = Uint32Array
                     } = t;
                     super({
                         ...t,
@@ -26098,38 +26101,38 @@
                             if ("positions" in t) {
                                 const {
                                     positions: r,
                                     holeIndices: s
                                 } = t;
                                 if (s) {
                                     let t = 0;
-                                    for (let o = 0; o <= s.length; o++) t = P_(n, t, r, e, s[o - 1], s[o], 0 === o ? 1 : -1), i.push(t);
+                                    for (let o = 0; o <= s.length; o++) t = S_(n, t, r, e, s[o - 1], s[o], 0 === o ? 1 : -1), i.push(t);
                                     return i.pop(), {
                                         positions: n,
                                         holeIndices: i
                                     }
                                 }
                                 t = r
                             }
                             if (! function(t) {
                                     return Array.isArray(t[0])
-                                }(t)) return P_(n, 0, t, e, 0, n.length, 1), n;
+                                }(t)) return S_(n, 0, t, e, 0, n.length, 1), n;
                             if (! function(t) {
                                     return t.length >= 1 && t[0].length >= 2 && Number.isFinite(t[0][0])
                                 }(t)) {
                                 let r = 0;
-                                for (const [s, o] of t.entries()) r = E_(n, r, o, e, 0 === s ? 1 : -1), i.push(r);
+                                for (const [s, o] of t.entries()) r = P_(n, r, o, e, 0 === s ? 1 : -1), i.push(r);
                                 return i.pop(), {
                                     positions: n,
                                     holeIndices: i
                                 }
                             }
-                            return E_(n, 0, t, e, 1), n
+                            return P_(n, 0, t, e, 1), n
                         }(t, this.positionSize);
-                        return this.opts.resolution ? Jy(x_(e), w_(e), {
+                        return this.opts.resolution ? $y(w_(e), E_(e), {
                             size: this.positionSize,
                             gridResolution: this.opts.resolution,
                             edgeTypes: !0
                         }) : this.opts.wrapLongitude ? function(t, e = null, n) {
                             const {
                                 size: i = 2,
                                 normalize: r = !0,
@@ -26139,50 +26142,50 @@
                             const o = [],
                                 a = [];
                             let l = 0,
                                 c = 0;
                             for (let r = 0; r <= e.length; r++) {
                                 const s = e[r] || t.length,
                                     h = c,
-                                    u = i_(t, i, l, s);
+                                    u = r_(t, i, l, s);
                                 for (let e = u; e < s; e++) o[c++] = t[e];
                                 for (let e = l; e < u; e++) o[c++] = t[e];
-                                s_(o, i, h, c), r_(o, i, h, c, null == n ? void 0 : n.maxLatitude), l = s, a[r] = c
+                                o_(o, i, h, c), s_(o, i, h, c, null == n ? void 0 : n.maxLatitude), l = s, a[r] = c
                             }
                             a.pop();
-                            const h = Jy(o, a, {
+                            const h = $y(o, a, {
                                 size: i,
                                 gridResolution: 360,
                                 gridOffset: [-180, -180],
                                 edgeTypes: s
                             });
                             if (r)
-                                for (const t of h) o_(t.positions, i);
+                                for (const t of h) a_(t.positions, i);
                             return h
-                        }(x_(e), w_(e), {
+                        }(w_(e), E_(e), {
                             size: this.positionSize,
                             maxLatitude: 86,
                             edgeTypes: !0
                         }) : e
                     }
                     return t
                 }
                 getGeometrySize(t) {
-                    if (A_(t)) {
+                    if (M_(t)) {
                         let e = 0;
                         for (const n of t) e += this.getGeometrySize(n);
                         return e
                     }
-                    return x_(t).length / this.positionSize
+                    return w_(t).length / this.positionSize
                 }
                 getGeometryFromBuffer(t) {
                     return this.normalize || !this.buffers.indices ? super.getGeometryFromBuffer(t) : null
                 }
                 updateGeometryAttributes(t, e) {
-                    if (t && A_(t))
+                    if (t && M_(t))
                         for (const n of t) {
                             const t = this.getGeometrySize(n);
                             e.geometrySize = t, this.updateGeometryAttributes(n, e), e.vertexStart += t, e.indexStart = this.indexStarts[e.geometryIndex + 1]
                         } else this._updateIndices(t, e), this._updatePositions(t, e), this._updateVertexValid(t, e)
                 }
                 _updateIndices(t, {
                     geometryIndex: e,
@@ -26194,36 +26197,36 @@
                         indexStarts: s,
                         typedArrayManager: o
                     } = this;
                     let a = r.indices;
                     if (!a || !t) return;
                     let l = i;
                     const c = function(t, e, n, i) {
-                        let r = w_(t);
+                        let r = E_(t);
                         r && (r = r.map((t => t / e)));
-                        let s = x_(t);
+                        let s = w_(t);
                         const o = i && 3 === e;
                         if (n) {
                             const t = s.length;
                             s = s.slice();
                             const i = [];
                             for (let r = 0; r < t; r += e) {
                                 i[0] = s[r], i[1] = s[r + 1], o && (i[2] = s[r + 2]);
                                 const t = n(i);
                                 s[r] = t[0], s[r + 1] = t[1], o && (s[r + 2] = t[2])
                             }
                         }
                         if (o) {
-                            const t = S_(s, 0, 1),
-                                e = S_(s, 0, 2),
-                                i = S_(s, 1, 2);
+                            const t = C_(s, 0, 1),
+                                e = C_(s, 0, 2),
+                                i = C_(s, 1, 2);
                             if (!t && !e && !i) return [];
-                            t > e && t > i || (e > i ? (n || (s = s.slice()), C_(s, 0, 2, 1)) : (n || (s = s.slice()), C_(s, 2, 0, 1)))
+                            t > e && t > i || (e > i ? (n || (s = s.slice()), T_(s, 0, 2, 1)) : (n || (s = s.slice()), T_(s, 2, 0, 1)))
                         }
-                        return y_()(s, r, e)
+                        return __()(s, r, e)
                     }(t, this.positionSize, this.opts.preproject, this.opts.full3d);
                     a = o.allocate(a, i + c.length, {
                         copy: !0
                     });
                     for (let t = 0; t < c.length; t++) a[l++] = c[t] + n;
                     s[e + 1] = i + c.length, r.indices = a
                 }
@@ -26234,43 +26237,43 @@
                     const {
                         attributes: {
                             positions: i
                         },
                         positionSize: r
                     } = this;
                     if (!i || !t) return;
-                    const s = x_(t);
+                    const s = w_(t);
                     for (let t = e, o = 0; o < n; t++, o++) {
                         const e = s[o * r],
                             n = s[o * r + 1],
                             a = r > 2 ? s[o * r + 2] : 0;
                         i[3 * t] = e, i[3 * t + 1] = n, i[3 * t + 2] = a
                     }
                 }
                 _updateVertexValid(t, {
                     vertexStart: e,
                     geometrySize: n
                 }) {
                     const {
                         positionSize: i
-                    } = this, r = this.attributes.vertexValid, s = t && w_(t);
+                    } = this, r = this.attributes.vertexValid, s = t && E_(t);
                     if (t && t.edgeTypes ? r.set(t.edgeTypes, e) : r.fill(1, e, e + n), s)
                         for (let t = 0; t < s.length; t++) r[e + s[t] / i - 1] = 0;
                     r[e + n - 1] = 0
                 }
             }
 
-            function A_(t) {
+            function M_(t) {
                 return Array.isArray(t) && t.length > 0 && !Number.isFinite(t[0])
             }
-            const M_ = "\nattribute vec2 vertexPositions;\nattribute float vertexValid;\n\nuniform bool extruded;\nuniform bool isWireframe;\nuniform float elevationScale;\nuniform float opacity;\n\nvarying vec4 vColor;\n\nstruct PolygonProps {\n  vec4 fillColors;\n  vec4 lineColors;\n  vec3 positions;\n  vec3 nextPositions;\n  vec3 pickingColors;\n  vec3 positions64Low;\n  vec3 nextPositions64Low;\n  float elevations;\n};\n\nvec3 project_offset_normal(vec3 vector) {\n  if (project_uCoordinateSystem == COORDINATE_SYSTEM_LNGLAT ||\n    project_uCoordinateSystem == COORDINATE_SYSTEM_LNGLAT_OFFSETS) {\n    return normalize(vector * project_uCommonUnitsPerWorldUnit);\n  }\n  return project_normal(vector);\n}\n\nvoid calculatePosition(PolygonProps props) {\n#ifdef IS_SIDE_VERTEX\n  if(vertexValid < 0.5){\n    gl_Position = vec4(0.);\n    return;\n  }\n#endif\n\n  vec3 pos;\n  vec3 pos64Low;\n  vec3 normal;\n  vec4 colors = isWireframe ? props.lineColors : props.fillColors;\n\n  geometry.worldPosition = props.positions;\n  geometry.worldPositionAlt = props.nextPositions;\n  geometry.pickingColor = props.pickingColors;\n\n#ifdef IS_SIDE_VERTEX\n  pos = mix(props.positions, props.nextPositions, vertexPositions.x);\n  pos64Low = mix(props.positions64Low, props.nextPositions64Low, vertexPositions.x);\n#else\n  pos = props.positions;\n  pos64Low = props.positions64Low;\n#endif\n\n  if (extruded) {\n    pos.z += props.elevations * vertexPositions.y * elevationScale;\n  }\n  gl_Position = project_position_to_clipspace(pos, pos64Low, vec3(0.), geometry.position);\n\n  DECKGL_FILTER_GL_POSITION(gl_Position, geometry);\n\n  if (extruded) {\n  #ifdef IS_SIDE_VERTEX\n    normal = vec3(\n      props.positions.y - props.nextPositions.y + (props.positions64Low.y - props.nextPositions64Low.y),\n      props.nextPositions.x - props.positions.x + (props.nextPositions64Low.x - props.positions64Low.x),\n      0.0);\n    normal = project_offset_normal(normal);\n  #else\n    normal = project_normal(vec3(0.0, 0.0, 1.0));\n  #endif\n    geometry.normal = normal;\n    vec3 lightColor = lighting_getLightColor(colors.rgb, project_uCameraPosition, geometry.position.xyz, normal);\n    vColor = vec4(lightColor, colors.a * opacity);\n  } else {\n    vColor = vec4(colors.rgb, colors.a * opacity);\n  }\n  DECKGL_FILTER_COLOR(vColor, geometry);\n}\n",
-                O_ = "#define SHADER_NAME solid-polygon-layer-vertex-shader\n\nattribute vec3 positions;\nattribute vec3 positions64Low;\nattribute float elevations;\nattribute vec4 fillColors;\nattribute vec4 lineColors;\nattribute vec3 pickingColors;\n\n".concat(M_, "\n\nvoid main(void) {\n  PolygonProps props;\n\n  props.positions = positions;\n  props.positions64Low = positions64Low;\n  props.elevations = elevations;\n  props.fillColors = fillColors;\n  props.lineColors = lineColors;\n  props.pickingColors = pickingColors;\n\n  calculatePosition(props);\n}\n"),
-                L_ = "#define SHADER_NAME solid-polygon-layer-vertex-shader-side\n#define IS_SIDE_VERTEX\n\n\nattribute vec3 instancePositions;\nattribute vec3 nextPositions;\nattribute vec3 instancePositions64Low;\nattribute vec3 nextPositions64Low;\nattribute float instanceElevations;\nattribute vec4 instanceFillColors;\nattribute vec4 instanceLineColors;\nattribute vec3 instancePickingColors;\n\n".concat(M_, "\n\nvoid main(void) {\n  PolygonProps props;\n\n  #if RING_WINDING_ORDER_CW == 1\n    props.positions = instancePositions;\n    props.positions64Low = instancePositions64Low;\n    props.nextPositions = nextPositions;\n    props.nextPositions64Low = nextPositions64Low;\n  #else\n    props.positions = nextPositions;\n    props.positions64Low = nextPositions64Low;\n    props.nextPositions = instancePositions;\n    props.nextPositions64Low = instancePositions64Low;\n  #endif\n  props.elevations = instanceElevations;\n  props.fillColors = instanceFillColors;\n  props.lineColors = instanceLineColors;\n  props.pickingColors = instancePickingColors;\n\n  calculatePosition(props);\n}\n"),
-                R_ = [0, 0, 0, 255],
-                I_ = {
+            const O_ = "\nattribute vec2 vertexPositions;\nattribute float vertexValid;\n\nuniform bool extruded;\nuniform bool isWireframe;\nuniform float elevationScale;\nuniform float opacity;\n\nvarying vec4 vColor;\n\nstruct PolygonProps {\n  vec4 fillColors;\n  vec4 lineColors;\n  vec3 positions;\n  vec3 nextPositions;\n  vec3 pickingColors;\n  vec3 positions64Low;\n  vec3 nextPositions64Low;\n  float elevations;\n};\n\nvec3 project_offset_normal(vec3 vector) {\n  if (project_uCoordinateSystem == COORDINATE_SYSTEM_LNGLAT ||\n    project_uCoordinateSystem == COORDINATE_SYSTEM_LNGLAT_OFFSETS) {\n    return normalize(vector * project_uCommonUnitsPerWorldUnit);\n  }\n  return project_normal(vector);\n}\n\nvoid calculatePosition(PolygonProps props) {\n#ifdef IS_SIDE_VERTEX\n  if(vertexValid < 0.5){\n    gl_Position = vec4(0.);\n    return;\n  }\n#endif\n\n  vec3 pos;\n  vec3 pos64Low;\n  vec3 normal;\n  vec4 colors = isWireframe ? props.lineColors : props.fillColors;\n\n  geometry.worldPosition = props.positions;\n  geometry.worldPositionAlt = props.nextPositions;\n  geometry.pickingColor = props.pickingColors;\n\n#ifdef IS_SIDE_VERTEX\n  pos = mix(props.positions, props.nextPositions, vertexPositions.x);\n  pos64Low = mix(props.positions64Low, props.nextPositions64Low, vertexPositions.x);\n#else\n  pos = props.positions;\n  pos64Low = props.positions64Low;\n#endif\n\n  if (extruded) {\n    pos.z += props.elevations * vertexPositions.y * elevationScale;\n  }\n  gl_Position = project_position_to_clipspace(pos, pos64Low, vec3(0.), geometry.position);\n\n  DECKGL_FILTER_GL_POSITION(gl_Position, geometry);\n\n  if (extruded) {\n  #ifdef IS_SIDE_VERTEX\n    normal = vec3(\n      props.positions.y - props.nextPositions.y + (props.positions64Low.y - props.nextPositions64Low.y),\n      props.nextPositions.x - props.positions.x + (props.nextPositions64Low.x - props.positions64Low.x),\n      0.0);\n    normal = project_offset_normal(normal);\n  #else\n    normal = project_normal(vec3(0.0, 0.0, 1.0));\n  #endif\n    geometry.normal = normal;\n    vec3 lightColor = lighting_getLightColor(colors.rgb, project_uCameraPosition, geometry.position.xyz, normal);\n    vColor = vec4(lightColor, colors.a * opacity);\n  } else {\n    vColor = vec4(colors.rgb, colors.a * opacity);\n  }\n  DECKGL_FILTER_COLOR(vColor, geometry);\n}\n",
+                L_ = "#define SHADER_NAME solid-polygon-layer-vertex-shader\n\nattribute vec3 positions;\nattribute vec3 positions64Low;\nattribute float elevations;\nattribute vec4 fillColors;\nattribute vec4 lineColors;\nattribute vec3 pickingColors;\n\n".concat(O_, "\n\nvoid main(void) {\n  PolygonProps props;\n\n  props.positions = positions;\n  props.positions64Low = positions64Low;\n  props.elevations = elevations;\n  props.fillColors = fillColors;\n  props.lineColors = lineColors;\n  props.pickingColors = pickingColors;\n\n  calculatePosition(props);\n}\n"),
+                R_ = "#define SHADER_NAME solid-polygon-layer-vertex-shader-side\n#define IS_SIDE_VERTEX\n\n\nattribute vec3 instancePositions;\nattribute vec3 nextPositions;\nattribute vec3 instancePositions64Low;\nattribute vec3 nextPositions64Low;\nattribute float instanceElevations;\nattribute vec4 instanceFillColors;\nattribute vec4 instanceLineColors;\nattribute vec3 instancePickingColors;\n\n".concat(O_, "\n\nvoid main(void) {\n  PolygonProps props;\n\n  #if RING_WINDING_ORDER_CW == 1\n    props.positions = instancePositions;\n    props.positions64Low = instancePositions64Low;\n    props.nextPositions = nextPositions;\n    props.nextPositions64Low = nextPositions64Low;\n  #else\n    props.positions = nextPositions;\n    props.positions64Low = nextPositions64Low;\n    props.nextPositions = instancePositions;\n    props.nextPositions64Low = instancePositions64Low;\n  #endif\n  props.elevations = instanceElevations;\n  props.fillColors = instanceFillColors;\n  props.lineColors = instanceLineColors;\n  props.pickingColors = instancePickingColors;\n\n  calculatePosition(props);\n}\n"),
+                I_ = [0, 0, 0, 255],
+                k_ = {
                     filled: !0,
                     extruded: !1,
                     wireframe: !1,
                     _normalize: !0,
                     _windingOrder: "CW",
                     _full3d: !1,
                     elevationScale: {
@@ -26284,37 +26287,37 @@
                     },
                     getElevation: {
                         type: "accessor",
                         value: 1e3
                     },
                     getFillColor: {
                         type: "accessor",
-                        value: R_
+                        value: I_
                     },
                     getLineColor: {
                         type: "accessor",
-                        value: R_
+                        value: I_
                     },
                     material: !0
                 },
-                k_ = {
+                j_ = {
                     enter: (t, e) => e.length ? e.subarray(e.length - t.length) : t
                 };
-            class j_ extends Fb {
+            class F_ extends zb {
                 constructor(...t) {
                     super(...t), wo(this, "state", void 0)
                 }
                 getShaders(t) {
                     return super.getShaders({
-                        vs: "top" === t ? O_ : L_,
+                        vs: "top" === t ? L_ : R_,
                         fs: "#define SHADER_NAME solid-polygon-layer-fragment-shader\n\nprecision highp float;\n\nvarying vec4 vColor;\n\nvoid main(void) {\n  gl_FragColor = vColor;\n\n  DECKGL_FILTER_COLOR(gl_FragColor, geometry);\n}\n",
                         defines: {
                             RING_WINDING_ORDER_CW: this.props._normalize || "CCW" !== this.props._windingOrder ? 1 : 0
                         },
-                        modules: [ty, v_, ny]
+                        modules: [ey, b_, iy]
                     })
                 }
                 get wrapLongitude() {
                     return !1
                 }
                 initializeState() {
                     const {
@@ -26326,18 +26329,18 @@
                     } = this.props;
                     const {
                         _full3d: i
                     } = this.props;
                     let r;
                     e.isGeospatial && n === Lh.DEFAULT && (n = Lh.LNGLAT), n === Lh.LNGLAT && (r = i ? e.projectPosition.bind(e) : e.projectFlat.bind(e)), this.setState({
                         numInstances: 0,
-                        polygonTesselator: new T_({
+                        polygonTesselator: new A_({
                             preproject: r,
                             fp64: this.use64bitPositions(),
-                            IndexType: !t || gp(t, dp) ? Uint32Array : Uint16Array
+                            IndexType: !t || mp(t, pp) ? Uint32Array : Uint16Array
                         })
                     });
                     const s = this.getAttributeManager(),
                         o = !0;
                     s.remove(["instancePickingColors"]), s.add({
                         indices: {
                             size: 1,
@@ -26345,15 +26348,15 @@
                             update: this.calculateIndices,
                             noAlloc: o
                         },
                         positions: {
                             size: 3,
                             type: 5130,
                             fp64: this.use64bitPositions(),
-                            transition: k_,
+                            transition: j_,
                             accessor: "getPolygon",
                             update: this.calculatePositions,
                             noAlloc: o,
                             shaderAttributes: {
                                 positions: {
                                     vertexOffset: 0,
                                     divisor: 0
@@ -26373,48 +26376,48 @@
                             divisor: 1,
                             type: 5121,
                             update: this.calculateVertexValid,
                             noAlloc: o
                         },
                         elevations: {
                             size: 1,
-                            transition: k_,
+                            transition: j_,
                             accessor: "getElevation",
                             shaderAttributes: {
                                 elevations: {
                                     divisor: 0
                                 },
                                 instanceElevations: {
                                     divisor: 1
                                 }
                             }
                         },
                         fillColors: {
                             size: this.props.colorFormat.length,
                             type: 5121,
                             normalized: !0,
-                            transition: k_,
+                            transition: j_,
                             accessor: "getFillColor",
-                            defaultValue: R_,
+                            defaultValue: I_,
                             shaderAttributes: {
                                 fillColors: {
                                     divisor: 0
                                 },
                                 instanceFillColors: {
                                     divisor: 1
                                 }
                             }
                         },
                         lineColors: {
                             size: this.props.colorFormat.length,
                             type: 5121,
                             normalized: !0,
-                            transition: k_,
+                            transition: j_,
                             accessor: "getLineColor",
-                            defaultValue: R_,
+                            defaultValue: I_,
                             shaderAttributes: {
                                 lineColors: {
                                     divisor: 0
                                 },
                                 instanceLineColors: {
                                     divisor: 1
                                 }
@@ -26521,33 +26524,33 @@
                         id: e,
                         filled: n,
                         extruded: i
                     } = this.props;
                     let r, s;
                     if (n) {
                         const n = this.getShaders("top");
-                        n.defines.NON_INSTANCED_MODEL = 1, r = new Yv(t, {
+                        n.defines.NON_INSTANCED_MODEL = 1, r = new Kv(t, {
                             ...n,
                             id: "".concat(e, "-top"),
                             drawMode: 4,
                             attributes: {
                                 vertexPositions: new Float32Array([0, 1])
                             },
                             uniforms: {
                                 isWireframe: !1,
                                 isSideVertex: !1
                             },
                             vertexCount: 0,
                             isIndexed: !0
                         })
                     }
-                    return i && (s = new Yv(t, {
+                    return i && (s = new Kv(t, {
                         ...this.getShaders("side"),
                         id: "".concat(e, "-side"),
-                        geometry: new ry({
+                        geometry: new sy({
                             drawMode: 1,
                             vertexCount: 4,
                             attributes: {
                                 vertexPositions: {
                                     size: 2,
                                     value: new Float32Array([1, 0, 0, 0, 0, 1, 1, 1])
                                 }
@@ -26575,18 +26578,18 @@
                     } = this.state;
                     t.startIndices = e.vertexStarts, t.value = e.get("positions")
                 }
                 calculateVertexValid(t) {
                     t.value = this.state.polygonTesselator.get("vertexValid")
                 }
             }
-            wo(j_, "defaultProps", I_), wo(j_, "layerName", "SolidPolygonLayer");
-            const F_ = {
+            wo(F_, "defaultProps", k_), wo(F_, "layerName", "SolidPolygonLayer");
+            const z_ = {
                     circle: {
-                        type: my,
+                        type: vy,
                         props: {
                             filled: "filled",
                             stroked: "stroked",
                             lineWidthMaxPixels: "lineWidthMaxPixels",
                             lineWidthMinPixels: "lineWidthMinPixels",
                             lineWidthScale: "lineWidthScale",
                             lineWidthUnits: "lineWidthUnits",
@@ -26599,15 +26602,15 @@
                             getFillColor: "getFillColor",
                             getLineColor: "getLineColor",
                             getLineWidth: "getLineWidth",
                             getPointRadius: "getRadius"
                         }
                     },
                     icon: {
-                        type: py,
+                        type: fy,
                         props: {
                             iconAtlas: "iconAtlas",
                             iconMapping: "iconMapping",
                             iconSizeMaxPixels: "sizeMaxPixels",
                             iconSizeMinPixels: "sizeMinPixels",
                             iconSizeScale: "sizeScale",
                             iconSizeUnits: "sizeUnits",
@@ -26617,15 +26620,15 @@
                             getIconAngle: "getAngle",
                             getIconColor: "getColor",
                             getIconPixelOffset: "getPixelOffset",
                             getIconSize: "getSize"
                         }
                     },
                     text: {
-                        type: Vy,
+                        type: Uy,
                         props: {
                             textSizeMaxPixels: "sizeMaxPixels",
                             textSizeMinPixels: "sizeMinPixels",
                             textSizeScale: "sizeScale",
                             textSizeUnits: "sizeUnits",
                             textBackground: "background",
                             textBackgroundPadding: "backgroundPadding",
@@ -26648,54 +26651,54 @@
                             getTextAlignmentBaseline: "getAlignmentBaseline",
                             getTextBackgroundColor: "getBackgroundColor",
                             getTextBorderColor: "getBorderColor",
                             getTextBorderWidth: "getBorderWidth"
                         }
                     }
                 },
-                z_ = {
-                    type: d_,
+                B_ = {
+                    type: p_,
                     props: {
                         lineWidthUnits: "widthUnits",
                         lineWidthScale: "widthScale",
                         lineWidthMinPixels: "widthMinPixels",
                         lineWidthMaxPixels: "widthMaxPixels",
                         lineJointRounded: "jointRounded",
                         lineCapRounded: "capRounded",
                         lineMiterLimit: "miterLimit",
                         lineBillboard: "billboard",
                         getLineColor: "getColor",
                         getLineWidth: "getWidth"
                     }
                 },
-                B_ = {
-                    type: j_,
+                D_ = {
+                    type: F_,
                     props: {
                         extruded: "extruded",
                         filled: "filled",
                         wireframe: "wireframe",
                         elevationScale: "elevationScale",
                         material: "material",
                         _full3d: "_full3d",
                         getElevation: "getElevation",
                         getFillColor: "getFillColor",
                         getLineColor: "getLineColor"
                     }
                 };
 
-            function D_({
+            function N_({
                 type: t,
                 props: e
             }) {
                 const n = {};
                 for (const i in e) n[i] = t.defaultProps[e[i]];
                 return n
             }
 
-            function N_(t, e) {
+            function V_(t, e) {
                 const {
                     transitions: n,
                     updateTriggers: i
                 } = t.props, r = {
                     updateTriggers: {},
                     transitions: n && {
                         getPosition: n.geometry
@@ -26705,15 +26708,15 @@
                     const o = e[s];
                     let a = t.props[s];
                     s.startsWith("get") && (a = t.getSubLayerAccessor(a), r.updateTriggers[o] = i[s], n && (r.transitions[o] = n[s])), r[o] = a
                 }
                 return r
             }
 
-            function V_(t, e, n = {}) {
+            function U_(t, e, n = {}) {
                 const i = {
                         pointFeatures: [],
                         lineFeatures: [],
                         polygonFeatures: [],
                         polygonOutlineFeatures: []
                     },
                     {
@@ -26727,32 +26730,32 @@
                         } = r;
                     if (s)
                         if ("GeometryCollection" === s.type) {
                             na.assert(Array.isArray(s.geometries), "GeoJSON does not have geometries array");
                             const {
                                 geometries: t
                             } = s;
-                            for (let s = 0; s < t.length; s++) U_(t[s], i, e, r, n)
-                        } else U_(s, i, e, r, n)
+                            for (let s = 0; s < t.length; s++) G_(t[s], i, e, r, n)
+                        } else G_(s, i, e, r, n)
                 }
                 return i
             }
 
-            function U_(t, e, n, i, r) {
+            function G_(t, e, n, i, r) {
                 const {
                     type: s,
                     coordinates: o
                 } = t, {
                     pointFeatures: a,
                     lineFeatures: l,
                     polygonFeatures: c,
                     polygonOutlineFeatures: h
                 } = e;
                 if (function(t, e) {
-                        let n = G_[t];
+                        let n = W_[t];
                         for (na.assert(n, "Unknown GeoJSON type ".concat(t)); e && --n > 0;) e = e[0];
                         return e && Number.isFinite(e[0])
                     }(s, o)) switch (s) {
                     case "Point":
                         a.push(n({
                             geometry: t
                         }, i, r));
@@ -26808,33 +26811,33 @@
                                         coordinates: t
                                     }
                                 }, i, r))
                             }))
                         }))
                 } else na.warn("".concat(s, " coordinates are malformed"))()
             }
-            const G_ = {
+            const W_ = {
                 Point: 1,
                 MultiPoint: 2,
                 LineString: 2,
                 MultiLineString: 3,
                 Polygon: 3,
                 MultiPolygon: 4
             };
 
-            function W_(t) {
+            function H_(t) {
                 return t.geometry.coordinates
             }
-            const H_ = ["points", "linestrings", "polygons"],
-                Z_ = {
-                    ...D_(F_.circle),
-                    ...D_(F_.icon),
-                    ...D_(F_.text),
-                    ...D_(z_),
-                    ...D_(B_),
+            const Z_ = ["points", "linestrings", "polygons"],
+                q_ = {
+                    ...N_(z_.circle),
+                    ...N_(z_.icon),
+                    ...N_(z_.text),
+                    ...N_(B_),
+                    ...N_(D_),
                     stroked: !0,
                     filled: !0,
                     extruded: !1,
                     wireframe: !1,
                     _full3d: !1,
                     iconAtlas: {
                         type: "object",
@@ -26853,15 +26856,15 @@
                         value: t => t.properties.text
                     },
                     pointType: "circle",
                     getRadius: {
                         deprecatedFor: "getPointRadius"
                     }
                 };
-            class q_ extends Jb {
+            class X_ extends $b {
                 initializeState() {
                     this.state = {
                         layerProps: {},
                         features: {}
                     }
                 }
                 updateState({
@@ -26993,83 +26996,83 @@
                         i = this.getSubLayerRow.bind(this);
                     let r = {};
                     const s = {};
                     if (Array.isArray(e.dataChanged)) {
                         const t = this.state.features;
                         for (const e in t) r[e] = t[e].slice(), s[e] = [];
                         for (const o of e.dataChanged) {
-                            const e = V_(n, i, o);
-                            for (const n in t) s[n].push($b({
+                            const e = U_(n, i, o);
+                            for (const n in t) s[n].push(ty({
                                 data: r[n],
                                 getIndex: t => t.__source.index,
                                 dataRange: o,
                                 replace: e[n]
                             }))
                         }
-                    } else r = V_(n, i);
+                    } else r = U_(n, i);
                     const o = function(t, e) {
                         const n = {
                                 points: {},
                                 lines: {},
                                 polygons: {},
                                 polygonsOutline: {}
                             },
                             {
                                 pointFeatures: i,
                                 lineFeatures: r,
                                 polygonFeatures: s,
                                 polygonOutlineFeatures: o
                             } = t;
-                        return n.points.data = i, n.points._dataDiff = e.pointFeatures && (() => e.pointFeatures), n.points.getPosition = W_, n.lines.data = r, n.lines._dataDiff = e.lineFeatures && (() => e.lineFeatures), n.lines.getPath = W_, n.polygons.data = s, n.polygons._dataDiff = e.polygonFeatures && (() => e.polygonFeatures), n.polygons.getPolygon = W_, n.polygonsOutline.data = o, n.polygonsOutline._dataDiff = e.polygonOutlineFeatures && (() => e.polygonOutlineFeatures), n.polygonsOutline.getPath = W_, n
+                        return n.points.data = i, n.points._dataDiff = e.pointFeatures && (() => e.pointFeatures), n.points.getPosition = H_, n.lines.data = r, n.lines._dataDiff = e.lineFeatures && (() => e.lineFeatures), n.lines.getPath = H_, n.polygons.data = s, n.polygons._dataDiff = e.polygonFeatures && (() => e.polygonFeatures), n.polygons.getPolygon = H_, n.polygonsOutline.data = o, n.polygonsOutline._dataDiff = e.polygonOutlineFeatures && (() => e.polygonOutlineFeatures), n.polygonsOutline.getPath = H_, n
                     }(r, s);
                     this.setState({
                         features: r,
                         featuresDiff: s,
                         layerProps: o
                     })
                 }
                 getPickingInfo(t) {
                     const e = super.getPickingInfo(t),
                         {
                             index: n,
                             sourceLayer: i
                         } = e;
-                    return e.featureType = H_.find((t => i.id.startsWith("".concat(this.id, "-").concat(t, "-")))), n >= 0 && i.id.startsWith("".concat(this.id, "-points-text")) && this.state.binary && (e.index = this.props.data.points.globalFeatureIds.value[n]), e
+                    return e.featureType = Z_.find((t => i.id.startsWith("".concat(this.id, "-").concat(t, "-")))), n >= 0 && i.id.startsWith("".concat(this.id, "-points-text")) && this.state.binary && (e.index = this.props.data.points.globalFeatureIds.value[n]), e
                 }
                 _updateAutoHighlight(t) {
                     const e = "".concat(this.id, "-points-"),
                         n = "points" === t.featureType;
                     for (const i of this.getSubLayers()) i.id.startsWith(e) === n && i.updateAutoHighlight(t)
                 }
                 _renderPolygonLayer() {
                     const {
                         extruded: t,
                         wireframe: e
                     } = this.props, {
                         layerProps: n
-                    } = this.state, i = "polygons-fill", r = this.shouldRenderSubLayer(i, n.polygons.data) && this.getSubLayerClass(i, B_.type);
+                    } = this.state, i = "polygons-fill", r = this.shouldRenderSubLayer(i, n.polygons.data) && this.getSubLayerClass(i, D_.type);
                     if (r) {
-                        const s = N_(this, B_.props),
+                        const s = V_(this, D_.props),
                             o = t && e;
                         return o || delete s.getLineColor, s.updateTriggers.lineColors = o, new r(s, this.getSubLayerProps({
                             id: i,
                             updateTriggers: s.updateTriggers
                         }), n.polygons)
                     }
                     return null
                 }
                 _renderLineLayers() {
                     const {
                         extruded: t,
                         stroked: e
                     } = this.props, {
                         layerProps: n
-                    } = this.state, i = "polygons-stroke", r = "linestrings", s = !t && e && this.shouldRenderSubLayer(i, n.polygonsOutline.data) && this.getSubLayerClass(i, z_.type), o = this.shouldRenderSubLayer(r, n.lines.data) && this.getSubLayerClass(r, z_.type);
+                    } = this.state, i = "polygons-stroke", r = "linestrings", s = !t && e && this.shouldRenderSubLayer(i, n.polygonsOutline.data) && this.getSubLayerClass(i, B_.type), o = this.shouldRenderSubLayer(r, n.lines.data) && this.getSubLayerClass(r, B_.type);
                     if (s || o) {
-                        const t = N_(this, z_.props);
+                        const t = V_(this, B_.props);
                         return [s && new s(t, this.getSubLayerProps({
                             id: i,
                             updateTriggers: t.updateTriggers
                         }), n.polygonsOutline), o && new o(t, this.getSubLayerProps({
                             id: r,
                             updateTriggers: t.updateTriggers
                         }), n.lines)]
@@ -27087,18 +27090,18 @@
                         highlightedObjectIndex: i
                     } = this.props;
                     !n && Number.isFinite(i) && (i = e.points.data.findIndex((t => t.__source.index === i)));
                     const r = new Set(t.split("+")),
                         s = [];
                     for (const t of r) {
                         const r = "points-".concat(t),
-                            o = F_[t],
+                            o = z_[t],
                             a = o && this.shouldRenderSubLayer(r, e.points.data) && this.getSubLayerClass(r, o.type);
                         if (a) {
-                            const l = N_(this, o.props);
+                            const l = V_(this, o.props);
                             let c = e.points;
                             if ("text" === t && n) {
                                 const {
                                     instancePickingColors: t,
                                     ...e
                                 } = c.data.attributes;
                                 c = {
@@ -27146,27 +27149,27 @@
                                 return i
                             }(t, i, n) : null
                         }(i, r);
                         return t(s, n)
                     } : super.getSubLayerAccessor(t)
                 }
             }
-            wo(q_, "layerName", "GeoJsonLayer"), wo(q_, "defaultProps", Z_);
-            var X_ = n(4155);
+            wo(X_, "layerName", "GeoJsonLayer"), wo(X_, "defaultProps", q_);
+            var Y_ = n(4155);
 
-            function Y_() {
+            function K_() {
                 let t;
                 if ("undefined" != typeof window && window.performance) t = window.performance.now();
-                else if (void 0 !== X_ && X_.hrtime) {
-                    const e = X_.hrtime();
+                else if (void 0 !== Y_ && Y_.hrtime) {
+                    const e = Y_.hrtime();
                     t = 1e3 * e[0] + e[1] / 1e6
                 } else t = Date.now();
                 return t
             }
-            class K_ {
+            class Q_ {
                 constructor(t, e) {
                     wo(this, "name", void 0), wo(this, "type", void 0), wo(this, "sampleSize", 1), wo(this, "time", 0), wo(this, "count", 0), wo(this, "samples", 0), wo(this, "lastTiming", 0), wo(this, "lastSampleTime", 0), wo(this, "lastSampleCount", 0), wo(this, "_count", 0), wo(this, "_time", 0), wo(this, "_samples", 0), wo(this, "_startTime", 0), wo(this, "_timerPending", !1), this.name = t, this.type = e, this.reset()
                 }
                 reset() {
                     return this.time = 0, this.count = 0, this.samples = 0, this.lastTiming = 0, this.lastSampleTime = 0, this.lastSampleCount = 0, this._count = 0, this._time = 0, this._samples = 0, this._startTime = 0, this._timerPending = !1, this
                 }
                 setSampleSize(t) {
@@ -27184,18 +27187,18 @@
                 subtractCount(t) {
                     return this._count -= t, this._samples++, this._checkSampling(), this
                 }
                 addTime(t) {
                     return this._time += t, this.lastTiming = t, this._samples++, this._checkSampling(), this
                 }
                 timeStart() {
-                    return this._startTime = Y_(), this._timerPending = !0, this
+                    return this._startTime = K_(), this._timerPending = !0, this
                 }
                 timeEnd() {
-                    return this._timerPending ? (this.addTime(Y_() - this._startTime), this._timerPending = !1, this._checkSampling(), this) : this
+                    return this._timerPending ? (this.addTime(K_() - this._startTime), this._timerPending = !1, this._checkSampling(), this) : this
                 }
                 getSampleAverageCount() {
                     return this.sampleSize > 0 ? this.lastSampleCount / this.sampleSize : 0
                 }
                 getSampleAverageTime() {
                     return this.sampleSize > 0 ? this.lastSampleTime / this.sampleSize : 0
                 }
@@ -27211,15 +27214,15 @@
                 getHz() {
                     return this.time > 0 ? this.samples / (this.time / 1e3) : 0
                 }
                 _checkSampling() {
                     this._samples === this.sampleSize && (this.lastSampleTime = this._time, this.lastSampleCount = this._count, this.count += this._count, this.time += this._time, this.samples += this._samples, this._time = 0, this._count = 0, this._samples = 0)
                 }
             }
-            class Q_ {
+            class J_ {
                 constructor(t) {
                     wo(this, "id", void 0), wo(this, "stats", {}), this.id = t.id, this.stats = {}, this._initializeStats(t.stats), Object.seal(this)
                 }
                 get(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "count";
                     return this._getOrCreate({
                         name: t,
@@ -27252,29 +27255,29 @@
                 }
                 _getOrCreate(t) {
                     const {
                         name: e,
                         type: n
                     } = t;
                     let i = this.stats[e];
-                    return i || (i = t instanceof K_ ? t : new K_(e, n), this.stats[e] = i), i
+                    return i || (i = t instanceof Q_ ? t : new Q_(e, n), this.stats[e] = i), i
                 }
             }
-            const J_ = {
+            const $_ = {
                 id: "request-scheduler",
                 throttleRequests: !0,
                 maxRequests: 6
             };
-            class $_ {
+            class tx {
                 constructor() {
                     let t = arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : {};
                     wo(this, "props", void 0), wo(this, "stats", void 0), wo(this, "activeRequestCount", 0), wo(this, "requestQueue", []), wo(this, "requestMap", new Map), wo(this, "deferredUpdate", null), this.props = {
-                        ...J_,
+                        ...$_,
                         ...t
-                    }, this.stats = new Q_({
+                    }, this.stats = new J_({
                         id: this.props.id
                     }), this.stats.get("Queued Requests"), this.stats.get("Active Requests"), this.stats.get("Cancelled Requests"), this.stats.get("Queued Requests Ever"), this.stats.get("Active Requests Ever")
                 }
                 scheduleRequest(t) {
                     let e = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : () => 0;
                     if (!this.props.throttleRequests) return Promise.resolve({
                         done: () => {}
@@ -27325,15 +27328,15 @@
                     }
                     t.sort(((t, e) => t.priority - e.priority))
                 }
                 _updateRequest(t) {
                     return t.priority = t.getPriority(t.handle), !(t.priority < 0 && (t.resolve(null), 1))
                 }
             }
-            class tx {
+            class ex {
                 constructor(t) {
                     wo(this, "index", void 0), wo(this, "isVisible", void 0), wo(this, "isSelected", void 0), wo(this, "parent", void 0), wo(this, "children", void 0), wo(this, "content", void 0), wo(this, "state", void 0), wo(this, "layers", void 0), wo(this, "id", void 0), wo(this, "zoom", void 0), wo(this, "userData", void 0), wo(this, "boundingBox", void 0), wo(this, "_abortController", void 0), wo(this, "_loader", void 0), wo(this, "_loaderId", void 0), wo(this, "_isLoaded", void 0), wo(this, "_isCancelled", void 0), wo(this, "_needsReload", void 0), wo(this, "_bbox", void 0), this.index = t, this.isVisible = !1, this.isSelected = !1, this.parent = null, this.children = [], this.content = null, this._loader = void 0, this._abortController = null, this._loaderId = 0, this._isLoaded = !1, this._isCancelled = !1, this._needsReload = !1
                 }
                 get bbox() {
                     return this._bbox
                 }
                 set bbox(t) {
@@ -27404,32 +27407,32 @@
                     this.isLoading && (this.abort(), this._loader = void 0), this._needsReload = !0
                 }
                 abort() {
                     var t;
                     this.isLoaded || (this._isCancelled = !0, null === (t = this._abortController) || void 0 === t || t.abort())
                 }
             }
-            const ex = Math.PI / 180,
-                nx = 180 / Math.PI,
-                ix = 6370972,
-                rx = 256;
+            const nx = Math.PI / 180,
+                ix = 180 / Math.PI,
+                rx = 6370972,
+                sx = 256;
 
-            function sx() {
+            function ox() {
                 const t = 4018225162502676e-20,
-                    e = Math.PI / 180 * rx;
+                    e = Math.PI / 180 * sx;
                 return {
                     unitsPerMeter: [t, t, t],
                     unitsPerMeter2: [0, 0, 0],
                     metersPerUnit: [24886.609375, 24886.609375, 24886.609375],
                     unitsPerDegree: [e, e, t],
                     unitsPerDegree2: [0, 0, 0],
                     degreesPerUnit: [1 / e, 1 / e, 24886.609375]
                 }
             }
-            class ox extends Dh {
+            class ax extends Dh {
                 constructor(t = {}) {
                     const {
                         latitude: e = 0,
                         longitude: n = 0,
                         zoom: i = 0,
                         nearZMultiplier: r = .1,
                         farZMultiplier: s = 2,
@@ -27441,25 +27444,25 @@
                     } = t;
                     a = a || 1, l = Math.max(.75, l);
                     const c = (new ih).lookAt({
                             eye: [0, -l, 0],
                             up: [0, 0, 1]
                         }),
                         h = Math.pow(2, i);
-                    c.rotateX(e * ex), c.rotateZ(-n * ex), c.scale(h / a);
+                    c.rotateX(e * nx), c.rotateZ(-n * nx), c.scale(h / a);
                     const u = Math.atan(.5 / l),
                         d = 512 * h / a;
                     super({
                         ...t,
                         height: a,
                         viewMatrix: c,
                         longitude: n,
                         latitude: e,
                         zoom: i,
-                        distanceScales: sx(),
+                        distanceScales: ox(),
                         fovyRadians: 2 * u,
                         focalDistance: l,
                         near: r,
                         far: Math.min(2, 1 / d + 1) * l * s
                     }), wo(this, "longitude", void 0), wo(this, "latitude", void 0), wo(this, "resolution", void 0), this.latitude = e, this.longitude = n, this.resolution = o
                 }
                 get projectionMode() {
@@ -27482,19 +27485,19 @@
                     topLeft: e = !0,
                     targetZ: n
                 } = {}) {
                     const [i, r, s] = t, o = e ? r : this.height - r, {
                         pixelUnprojectionMatrix: a
                     } = this;
                     let l;
-                    if (Number.isFinite(s)) l = ax(a, [i, o, s, 1]);
+                    if (Number.isFinite(s)) l = lx(a, [i, o, s, 1]);
                     else {
-                        const t = ax(a, [i, o, -1, 1]),
-                            e = ax(a, [i, o, 1, 1]),
-                            r = ((n || 0) / ix + 1) * rx,
+                        const t = lx(a, [i, o, -1, 1]),
+                            e = lx(a, [i, o, 1, 1]),
+                            r = ((n || 0) / rx + 1) * sx,
                             s = Ac(Cc([], t, e)),
                             c = Ac(t),
                             h = Ac(e),
                             u = (4 * c * h - (s - c - h) ** 2) / 16 * 4 / s;
                         l = function(t, e, n, i) {
                             var r = e[0],
                                 s = e[1],
@@ -27502,20 +27505,20 @@
                             return t[0] = r + i * (n[0] - r), t[1] = s + i * (n[1] - s), t[2] = o + i * (n[2] - o), t
                         }([], t, e, (Math.sqrt(c - u) - Math.sqrt(Math.max(0, r * r - u))) / Math.sqrt(s))
                     }
                     const [c, h, u] = this.unprojectPosition(l);
                     return Number.isFinite(s) ? [c, h, u] : Number.isFinite(n) ? [c, h, n] : [c, h]
                 }
                 projectPosition(t) {
-                    const [e, n, i = 0] = t, r = e * ex, s = n * ex, o = Math.cos(s), a = (i / ix + 1) * rx;
+                    const [e, n, i = 0] = t, r = e * nx, s = n * nx, o = Math.cos(s), a = (i / rx + 1) * sx;
                     return [Math.sin(r) * o * a, -Math.cos(r) * o * a, Math.sin(s) * a]
                 }
                 unprojectPosition(t) {
                     const [e, n, i] = t, r = Tc(t), s = Math.asin(i / r);
-                    return [Math.atan2(e, -n) * nx, s * nx, (r / rx - 1) * ix]
+                    return [Math.atan2(e, -n) * ix, s * ix, (r / sx - 1) * rx]
                 }
                 projectFlat(t) {
                     return t
                 }
                 unprojectFlat(t) {
                     return t
                 }
@@ -27524,84 +27527,84 @@
                     return {
                         longitude: t[0] - n[0] + this.longitude,
                         latitude: t[1] - n[1] + this.latitude
                     }
                 }
             }
 
-            function ax(t, e) {
+            function lx(t, e) {
                 const n = Qc([], e, t);
                 return Kc(n, n, 1 / n[3]), n
             }
-            const lx = -1,
-                cx = new Ic,
-                hx = new Ic;
-            class ux {
+            const cx = -1,
+                hx = new Ic,
+                ux = new Ic;
+            class dx {
                 constructor(t = [0, 0, 0], e = [0, 0, 0], n) {
-                    wo(this, "center", void 0), wo(this, "halfDiagonal", void 0), wo(this, "minimum", void 0), wo(this, "maximum", void 0), n = n || cx.copy(t).add(e).scale(.5), this.center = new Ic(n), this.halfDiagonal = new Ic(e).subtract(this.center), this.minimum = new Ic(t), this.maximum = new Ic(e)
+                    wo(this, "center", void 0), wo(this, "halfDiagonal", void 0), wo(this, "minimum", void 0), wo(this, "maximum", void 0), n = n || hx.copy(t).add(e).scale(.5), this.center = new Ic(n), this.halfDiagonal = new Ic(e).subtract(this.center), this.minimum = new Ic(t), this.maximum = new Ic(e)
                 }
                 clone() {
-                    return new ux(this.minimum, this.maximum, this.center)
+                    return new dx(this.minimum, this.maximum, this.center)
                 }
                 equals(t) {
                     return this === t || Boolean(t) && this.minimum.equals(t.minimum) && this.maximum.equals(t.maximum)
                 }
                 transform(t) {
                     return this.center.transformAsPoint(t), this.halfDiagonal.transform(t), this.minimum.transform(t), this.maximum.transform(t), this
                 }
                 intersectPlane(t) {
                     const {
                         halfDiagonal: e
-                    } = this, n = hx.from(t.normal), i = e.x * Math.abs(n.x) + e.y * Math.abs(n.y) + e.z * Math.abs(n.z), r = this.center.dot(n) + t.distance;
-                    return r - i > 0 ? 1 : r + i < 0 ? lx : 0
+                    } = this, n = ux.from(t.normal), i = e.x * Math.abs(n.x) + e.y * Math.abs(n.y) + e.z * Math.abs(n.z), r = this.center.dot(n) + t.distance;
+                    return r - i > 0 ? 1 : r + i < 0 ? cx : 0
                 }
                 distanceTo(t) {
                     return Math.sqrt(this.distanceSquaredTo(t))
                 }
                 distanceSquaredTo(t) {
-                    const e = cx.from(t).subtract(this.center),
+                    const e = hx.from(t).subtract(this.center),
                         {
                             halfDiagonal: n
                         } = this;
                     let i, r = 0;
                     return i = Math.abs(e.x) - n.x, i > 0 && (r += i * i), i = Math.abs(e.y) - n.y, i > 0 && (r += i * i), i = Math.abs(e.z) - n.z, i > 0 && (r += i * i), r
                 }
             }
-            const dx = new Ic,
-                px = new Ic;
-            class fx {
+            const px = new Ic,
+                fx = new Ic;
+            class gx {
                 constructor(t = [0, 0, 0], e = 0) {
                     wo(this, "center", void 0), wo(this, "radius", void 0), this.radius = -0, this.center = new Ic, this.fromCenterRadius(t, e)
                 }
                 fromCenterRadius(t, e) {
                     return this.center.from(t), this.radius = e, this
                 }
                 fromCornerPoints(t, e) {
-                    return e = dx.from(e), this.center = (new Ic).from(t).add(e).scale(.5), this.radius = this.center.distance(e), this
+                    return e = px.from(e), this.center = (new Ic).from(t).add(e).scale(.5), this.radius = this.center.distance(e), this
                 }
                 equals(t) {
                     return this === t || Boolean(t) && this.center.equals(t.center) && this.radius === t.radius
                 }
                 clone() {
-                    return new fx(this.center, this.radius)
+                    return new gx(this.center, this.radius)
                 }
                 union(t) {
                     const e = this.center,
                         n = this.radius,
                         i = t.center,
                         r = t.radius,
-                        s = dx.copy(i).subtract(e),
+                        s = px.copy(i).subtract(e),
                         o = s.magnitude();
                     if (n >= o + r) return this.clone();
                     if (r >= o + n) return t.clone();
                     const a = .5 * (n + o + r);
-                    return px.copy(s).scale((-n + a) / o).add(e), this.center.copy(px), this.radius = a, this
+                    return fx.copy(s).scale((-n + a) / o).add(e), this.center.copy(fx), this.radius = a, this
                 }
                 expand(t) {
-                    const e = dx.from(t).subtract(this.center).magnitude();
+                    const e = px.from(t).subtract(this.center).magnitude();
                     return e > this.radius && (this.radius = e), this
                 }
                 transform(t) {
                     this.center.transform(t);
                     const e = function(t, e) {
                         var n = e[0],
                             i = e[1],
@@ -27609,34 +27612,34 @@
                             s = e[4],
                             o = e[5],
                             a = e[6],
                             l = e[8],
                             c = e[9],
                             h = e[10];
                         return t[0] = Math.hypot(n, i, r), t[1] = Math.hypot(s, o, a), t[2] = Math.hypot(l, c, h), t
-                    }(dx, t);
+                    }(px, t);
                     return this.radius = Math.max(e[0], Math.max(e[1], e[2])) * this.radius, this
                 }
                 distanceSquaredTo(t) {
                     const e = this.distanceTo(t);
                     return e * e
                 }
                 distanceTo(t) {
-                    const e = dx.from(t).subtract(this.center);
+                    const e = px.from(t).subtract(this.center);
                     return Math.max(0, e.len() - this.radius)
                 }
                 intersectPlane(t) {
                     const e = this.center,
                         n = this.radius,
                         i = t.normal.dot(e) + t.distance;
-                    return i < -n ? lx : i < n ? 0 : 1
+                    return i < -n ? cx : i < n ? 0 : 1
                 }
             }
 
-            function gx(t, e, n) {
+            function mx(t, e, n) {
                 var i = e[0],
                     r = e[1],
                     s = e[2],
                     o = e[3],
                     a = e[4],
                     l = e[5],
                     c = e[6],
@@ -27650,48 +27653,48 @@
                     v = n[5],
                     b = n[6],
                     y = n[7],
                     _ = n[8];
                 return t[0] = d * i + p * o + f * c, t[1] = d * r + p * a + f * h, t[2] = d * s + p * l + f * u, t[3] = g * i + m * o + v * c, t[4] = g * r + m * a + v * h, t[5] = g * s + m * l + v * u, t[6] = b * i + y * o + _ * c, t[7] = b * r + y * a + _ * h, t[8] = b * s + y * l + _ * u, t
             }
 
-            function mx(t, e, n) {
+            function vx(t, e, n) {
                 var i = n[0],
                     r = n[1];
                 return t[0] = i * e[0], t[1] = i * e[1], t[2] = i * e[2], t[3] = r * e[3], t[4] = r * e[4], t[5] = r * e[5], t[6] = e[6], t[7] = e[7], t[8] = e[8], t
             }
-            var vx;
+            var bx;
             ! function(t) {
                 t[t.COL0ROW0 = 0] = "COL0ROW0", t[t.COL0ROW1 = 1] = "COL0ROW1", t[t.COL0ROW2 = 2] = "COL0ROW2", t[t.COL1ROW0 = 3] = "COL1ROW0", t[t.COL1ROW1 = 4] = "COL1ROW1", t[t.COL1ROW2 = 5] = "COL1ROW2", t[t.COL2ROW0 = 6] = "COL2ROW0", t[t.COL2ROW1 = 7] = "COL2ROW1", t[t.COL2ROW2 = 8] = "COL2ROW2"
-            }(vx || (vx = {}));
-            const bx = Object.freeze([1, 0, 0, 0, 1, 0, 0, 0, 1]);
-            class yx extends Dc {
+            }(bx || (bx = {}));
+            const yx = Object.freeze([1, 0, 0, 0, 1, 0, 0, 0, 1]);
+            class _x extends Dc {
                 static get IDENTITY() {
-                    return xx || (xx = new yx, Object.freeze(xx)), xx
+                    return wx || (wx = new _x, Object.freeze(wx)), wx
                 }
                 static get ZERO() {
-                    return _x || (_x = new yx([0, 0, 0, 0, 0, 0, 0, 0, 0]), Object.freeze(_x)), _x
+                    return xx || (xx = new _x([0, 0, 0, 0, 0, 0, 0, 0, 0]), Object.freeze(xx)), xx
                 }
                 get ELEMENTS() {
                     return 9
                 }
                 get RANK() {
                     return 3
                 }
                 get INDICES() {
-                    return vx
+                    return bx
                 }
                 constructor(t, ...e) {
                     super(-0, -0, -0, -0, -0, -0, -0, -0, -0), 1 === arguments.length && Array.isArray(t) ? this.copy(t) : e.length > 0 ? this.copy([t, ...e]) : this.identity()
                 }
                 copy(t) {
                     return this[0] = t[0], this[1] = t[1], this[2] = t[2], this[3] = t[3], this[4] = t[4], this[5] = t[5], this[6] = t[6], this[7] = t[7], this[8] = t[8], this.check()
                 }
                 identity() {
-                    return this.copy(bx)
+                    return this.copy(yx)
                 }
                 fromObject(t) {
                     return this.check()
                 }
                 fromQuaternion(t) {
                     return function(t, e) {
                         var n = e[0],
@@ -27734,25 +27737,25 @@
                     }(this, this), this.check()
                 }
                 invert() {
                     var t, e, n, i, r, s, o, a, l, c, h, u, d, p, f;
                     return t = this, n = (e = this)[0], i = e[1], r = e[2], s = e[3], o = e[4], a = e[5], l = e[6], c = e[7], (f = n * (u = (h = e[8]) * o - a * c) + i * (d = -h * s + a * l) + r * (p = c * s - o * l)) && (f = 1 / f, t[0] = u * f, t[1] = (-h * i + r * c) * f, t[2] = (a * i - r * o) * f, t[3] = d * f, t[4] = (h * n - r * l) * f, t[5] = (-a * n + r * s) * f, t[6] = p * f, t[7] = (-c * n + i * l) * f, t[8] = (o * n - i * s) * f), this.check()
                 }
                 multiplyLeft(t) {
-                    return gx(this, t, this), this.check()
+                    return mx(this, t, this), this.check()
                 }
                 multiplyRight(t) {
-                    return gx(this, this, t), this.check()
+                    return mx(this, this, t), this.check()
                 }
                 rotate(t) {
                     var e, n, i, r, s, o, a, l, c, h, u, d, p, f;
                     return e = this, i = t, r = (n = this)[0], s = n[1], o = n[2], a = n[3], l = n[4], c = n[5], h = n[6], u = n[7], d = n[8], p = Math.sin(i), f = Math.cos(i), e[0] = f * r + p * a, e[1] = f * s + p * l, e[2] = f * o + p * c, e[3] = f * a - p * r, e[4] = f * l - p * s, e[5] = f * c - p * o, e[6] = h, e[7] = u, e[8] = d, this.check()
                 }
                 scale(t) {
-                    return Array.isArray(t) ? mx(this, this, t) : mx(this, this, [t, t]), this.check()
+                    return Array.isArray(t) ? vx(this, this, t) : vx(this, this, [t, t]), this.check()
                 }
                 translate(t) {
                     var e, n, i, r, s, o, a, l, c, h, u, d, p, f;
                     return e = this, i = t, r = (n = this)[0], s = n[1], o = n[2], a = n[3], l = n[4], c = n[5], h = n[6], u = n[7], d = n[8], p = i[0], f = i[1], e[0] = r, e[1] = s, e[2] = o, e[3] = a, e[4] = l, e[5] = c, e[6] = p * r + f * a + h, e[7] = p * s + f * l + u, e[8] = p * o + f * c + d, this.check()
                 }
                 transform(t, e) {
                     let n;
@@ -27781,18 +27784,18 @@
                 transformVector2(t, e) {
                     return this.transform(t, e)
                 }
                 transformVector3(t, e) {
                     return this.transform(t, e)
                 }
             }
-            let _x, xx, wx;
-            class Ex extends mc {
+            let xx, wx, Ex;
+            class Px extends mc {
                 static get ZERO() {
-                    return wx || (wx = new Ex(0, 0, 0, 0), Object.freeze(wx)), wx
+                    return Ex || (Ex = new Px(0, 0, 0, 0), Object.freeze(Ex)), Ex
                 }
                 constructor(t = 0, e = 0, n = 0, i = 0) {
                     super(-0, -0, -0, -0), lc(t) && 1 === arguments.length ? this.copy(t) : (oc.debug && (pc(t), pc(e), pc(n), pc(i)), this[0] = t, this[1] = e, this[2] = n, this[3] = i)
                 }
                 set(t, e, n, i) {
                     return this[0] = t, this[1] = e, this[2] = n, this[3] = i, this.check()
                 }
@@ -27837,71 +27840,71 @@
                     return Sc(this, this, t), this.check()
                 }
                 applyMatrix4(t) {
                     return t.transform(this, this), this
                 }
             }
 
-            function Px() {
+            function Sx() {
                 var t = new bc(4);
                 return bc != Float32Array && (t[0] = 0, t[1] = 0, t[2] = 0), t[3] = 1, t
             }
 
-            function Sx(t, e, n) {
+            function Cx(t, e, n) {
                 n *= .5;
                 var i = Math.sin(n);
                 return t[0] = i * e[0], t[1] = i * e[1], t[2] = i * e[2], t[3] = Math.cos(n), t
             }
 
-            function Cx(t, e, n) {
+            function Tx(t, e, n) {
                 var i = e[0],
                     r = e[1],
                     s = e[2],
                     o = e[3],
                     a = n[0],
                     l = n[1],
                     c = n[2],
                     h = n[3];
                 return t[0] = i * h + o * a + r * c - s * l, t[1] = r * h + o * l + s * a - i * c, t[2] = s * h + o * c + i * l - r * a, t[3] = o * h - i * a - r * l - s * c, t
             }
-            var Tx, Ax, Mx, Ox, Lx = Kc,
-                Rx = function(t) {
+            var Ax, Mx, Ox, Lx, Rx = Kc,
+                Ix = function(t) {
                     var e = t[0],
                         n = t[1],
                         i = t[2],
                         r = t[3];
                     return Math.hypot(e, n, i, r)
                 },
-                Ix = function(t) {
+                kx = function(t) {
                     var e = t[0],
                         n = t[1],
                         i = t[2],
                         r = t[3];
                     return e * e + n * n + i * i + r * r
                 },
-                kx = (Tx = yc(), Ax = _c(1, 0, 0), Mx = _c(0, 1, 0), function(t, e, n) {
+                jx = (Ax = yc(), Mx = _c(1, 0, 0), Ox = _c(0, 1, 0), function(t, e, n) {
                     var i = xc(e, n);
-                    return i < -.999999 ? (wc(Tx, Ax, e), Tc(Tx) < 1e-6 && wc(Tx, Mx, e), function(t, e) {
+                    return i < -.999999 ? (wc(Ax, Mx, e), Tc(Ax) < 1e-6 && wc(Ax, Ox, e), function(t, e) {
                         var n = e[0],
                             i = e[1],
                             r = e[2],
                             s = n * n + i * i + r * r;
                         s > 0 && (s = 1 / Math.sqrt(s)), t[0] = e[0] * s, t[1] = e[1] * s, t[2] = e[2] * s
-                    }(Tx, Tx), Sx(t, Tx, Math.PI), t) : i > .999999 ? (t[0] = 0, t[1] = 0, t[2] = 0, t[3] = 1, t) : (wc(Tx, e, n), t[0] = Tx[0], t[1] = Tx[1], t[2] = Tx[2], t[3] = 1 + i, function(t, e) {
+                    }(Ax, Ax), Cx(t, Ax, Math.PI), t) : i > .999999 ? (t[0] = 0, t[1] = 0, t[2] = 0, t[3] = 1, t) : (wc(Ax, e, n), t[0] = Ax[0], t[1] = Ax[1], t[2] = Ax[2], t[3] = 1 + i, function(t, e) {
                         var n = e[0],
                             i = e[1],
                             r = e[2],
                             s = e[3],
                             o = n * n + i * i + r * r + s * s;
                         return o > 0 && (o = 1 / Math.sqrt(o)), t[0] = n * o, t[1] = i * o, t[2] = r * o, t[3] = s * o, t
                     }(t, t))
                 });
-            Px(), Px(), Ox = new bc(9), bc != Float32Array && (Ox[1] = 0, Ox[2] = 0, Ox[3] = 0, Ox[5] = 0, Ox[6] = 0, Ox[7] = 0), Ox[0] = 1, Ox[4] = 1, Ox[8] = 1;
-            const jx = [0, 0, 0, 1];
-            class Fx extends dc {
+            Sx(), Sx(), Lx = new bc(9), bc != Float32Array && (Lx[1] = 0, Lx[2] = 0, Lx[3] = 0, Lx[5] = 0, Lx[6] = 0, Lx[7] = 0), Lx[0] = 1, Lx[4] = 1, Lx[8] = 1;
+            const Fx = [0, 0, 0, 1];
+            class zx extends dc {
                 constructor(t = 0, e = 0, n = 0, i = 1) {
                     super(-0, -0, -0, -0), Array.isArray(t) && 1 === arguments.length ? this.copy(t) : this.set(t, e, n, i)
                 }
                 copy(t) {
                     return this[0] = t[0], this[1] = t[1], this[2] = t[2], this[3] = t[3], this.check()
                 }
                 set(t, e, n, i) {
@@ -27920,15 +27923,15 @@
                             var s = (r + 1) % 3,
                                 o = (r + 2) % 3;
                             n = Math.sqrt(e[3 * r + r] - e[3 * s + s] - e[3 * o + o] + 1), t[r] = .5 * n, n = .5 / n, t[3] = (e[3 * s + o] - e[3 * o + s]) * n, t[s] = (e[3 * s + r] + e[3 * r + s]) * n, t[o] = (e[3 * o + r] + e[3 * r + o]) * n
                         }
                     }(this, t), this.check()
                 }
                 fromAxisRotation(t, e) {
-                    return Sx(this, t, e), this.check()
+                    return Cx(this, t, e), this.check()
                 }
                 identity() {
                     return function(t) {
                         t[0] = 0, t[1] = 0, t[2] = 0, t[3] = 1
                     }(this), this.check()
                 }
                 setAxisAngle(t, e) {
@@ -27958,26 +27961,26 @@
                 get w() {
                     return this[3]
                 }
                 set w(t) {
                     this[3] = pc(t)
                 }
                 len() {
-                    return Rx(this)
+                    return Ix(this)
                 }
                 lengthSquared() {
-                    return Ix(this)
+                    return kx(this)
                 }
                 dot(t) {
                     return function(t, e) {
                         return t[0] * e[0] + t[1] * e[1] + t[2] * e[2] + t[3] * e[3]
                     }(this, t)
                 }
                 rotationTo(t, e) {
-                    return kx(this, t, e), this.check()
+                    return jx(this, t, e), this.check()
                 }
                 add(t) {
                     return function(t, e, n) {
                         t[0] = e[0] + n[0], t[1] = e[1] + n[1], t[2] = e[2] + n[2], t[3] = e[3] + n[3]
                     }(this, this, t), this.check()
                 }
                 calculateW() {
@@ -28010,18 +28013,18 @@
                             s = e[1],
                             o = e[2],
                             a = e[3];
                         t[0] = r + i * (n[0] - r), t[1] = s + i * (n[1] - s), t[2] = o + i * (n[2] - o), t[3] = a + i * (n[3] - a)
                     }(this, t, e, n), this.check())
                 }
                 multiplyRight(t) {
-                    return Cx(this, this, t), this.check()
+                    return Tx(this, this, t), this.check()
                 }
                 multiplyLeft(t) {
-                    return Cx(this, t, this), this.check()
+                    return Tx(this, t, this), this.check()
                 }
                 normalize() {
                     const t = this.len(),
                         e = t > 0 ? 1 / t : 0;
                     return this[0] = this[0] * e, this[1] = this[1] * e, this[2] = this[2] * e, this[3] = this[3] * e, 0 === t && (this[3] = 1), this.check()
                 }
                 rotateX(t) {
@@ -28057,22 +28060,22 @@
                             o = e[3],
                             a = Math.sin(n),
                             l = Math.cos(n);
                         t[0] = i * l + r * a, t[1] = r * l - i * a, t[2] = s * l + o * a, t[3] = o * l - s * a
                     }(this, this, t), this.check()
                 }
                 scale(t) {
-                    return Lx(this, this, t), this.check()
+                    return Rx(this, this, t), this.check()
                 }
                 slerp(t, e, n) {
                     let i, r, s;
                     switch (arguments.length) {
                         case 1:
                             ({
-                                start: i = jx,
+                                start: i = Fx,
                                 target: r,
                                 ratio: s
                             } = t);
                             break;
                         case 2:
                             i = this, r = t, s = e;
                             break;
@@ -28087,15 +28090,15 @@
                             p = n[0],
                             f = n[1],
                             g = n[2],
                             m = n[3];
                         (s = c * p + h * f + u * g + d * m) < 0 && (s = -s, p = -p, f = -f, g = -g, m = -m), 1 - s > vc ? (r = Math.acos(s), o = Math.sin(r), a = Math.sin((1 - i) * r) / o, l = Math.sin(i * r) / o) : (a = 1 - i, l = i), t[0] = a * c + l * p, t[1] = a * h + l * f, t[2] = a * u + l * g, t[3] = a * d + l * m
                     }(this, i, r, s), this.check()
                 }
-                transformVector4(t, e = new Ex) {
+                transformVector4(t, e = new Px) {
                     return function(t, e, n) {
                         var i = e[0],
                             r = e[1],
                             s = e[2],
                             o = n[0],
                             a = n[1],
                             l = n[2],
@@ -28116,202 +28119,202 @@
                 premultiply(t) {
                     return this.multiplyLeft(t)
                 }
                 multiply(t) {
                     return this.multiplyRight(t)
                 }
             }
-            const zx = new Ic,
-                Bx = new Ic,
+            const Bx = new Ic,
                 Dx = new Ic,
                 Nx = new Ic,
                 Vx = new Ic,
                 Ux = new Ic,
-                Gx = new Ic;
-            class Wx {
+                Gx = new Ic,
+                Wx = new Ic;
+            class Hx {
                 constructor(t = [0, 0, 0], e = [0, 0, 0, 0, 0, 0, 0, 0, 0]) {
-                    wo(this, "center", void 0), wo(this, "halfAxes", void 0), this.center = (new Ic).from(t), this.halfAxes = new yx(e)
+                    wo(this, "center", void 0), wo(this, "halfAxes", void 0), this.center = (new Ic).from(t), this.halfAxes = new _x(e)
                 }
                 get halfSize() {
                     const t = this.halfAxes.getColumn(0),
                         e = this.halfAxes.getColumn(1),
                         n = this.halfAxes.getColumn(2);
                     return [new Ic(t).len(), new Ic(e).len(), new Ic(n).len()]
                 }
                 get quaternion() {
                     const t = this.halfAxes.getColumn(0),
                         e = this.halfAxes.getColumn(1),
                         n = this.halfAxes.getColumn(2),
                         i = new Ic(t).normalize(),
                         r = new Ic(e).normalize(),
                         s = new Ic(n).normalize();
-                    return (new Fx).fromMatrix3(new yx([...i, ...r, ...s]))
+                    return (new zx).fromMatrix3(new _x([...i, ...r, ...s]))
                 }
                 fromCenterHalfSizeQuaternion(t, e, n) {
-                    const i = new Fx(n),
-                        r = (new yx).fromQuaternion(i);
+                    const i = new zx(n),
+                        r = (new _x).fromQuaternion(i);
                     return r[0] = r[0] * e[0], r[1] = r[1] * e[0], r[2] = r[2] * e[0], r[3] = r[3] * e[1], r[4] = r[4] * e[1], r[5] = r[5] * e[1], r[6] = r[6] * e[2], r[7] = r[7] * e[2], r[8] = r[8] * e[2], this.center = (new Ic).from(t), this.halfAxes = r, this
                 }
                 clone() {
-                    return new Wx(this.center, this.halfAxes)
+                    return new Hx(this.center, this.halfAxes)
                 }
                 equals(t) {
                     return this === t || Boolean(t) && this.center.equals(t.center) && this.halfAxes.equals(t.halfAxes)
                 }
-                getBoundingSphere(t = new fx) {
+                getBoundingSphere(t = new gx) {
                     const e = this.halfAxes,
-                        n = e.getColumn(0, Dx),
-                        i = e.getColumn(1, Nx),
-                        r = e.getColumn(2, Vx),
-                        s = zx.copy(n).add(i).add(r);
+                        n = e.getColumn(0, Nx),
+                        i = e.getColumn(1, Vx),
+                        r = e.getColumn(2, Ux),
+                        s = Bx.copy(n).add(i).add(r);
                     return t.center.copy(this.center), t.radius = s.magnitude(), t
                 }
                 intersectPlane(t) {
                     const e = this.center,
                         n = t.normal,
                         i = this.halfAxes,
                         r = n.x,
                         s = n.y,
                         o = n.z,
                         a = Math.abs(r * i[0] + s * i[1] + o * i[2]) + Math.abs(r * i[3] + s * i[4] + o * i[5]) + Math.abs(r * i[6] + s * i[7] + o * i[8]),
                         l = n.dot(e) + t.distance;
-                    return l <= -a ? lx : l >= a ? 1 : 0
+                    return l <= -a ? cx : l >= a ? 1 : 0
                 }
                 distanceTo(t) {
                     return Math.sqrt(this.distanceSquaredTo(t))
                 }
                 distanceSquaredTo(t) {
-                    const e = Bx.from(t).subtract(this.center),
+                    const e = Dx.from(t).subtract(this.center),
                         n = this.halfAxes,
-                        i = n.getColumn(0, Dx),
-                        r = n.getColumn(1, Nx),
-                        s = n.getColumn(2, Vx),
+                        i = n.getColumn(0, Nx),
+                        r = n.getColumn(1, Vx),
+                        s = n.getColumn(2, Ux),
                         o = i.magnitude(),
                         a = r.magnitude(),
                         l = s.magnitude();
                     i.normalize(), r.normalize(), s.normalize();
                     let c, h = 0;
                     return c = Math.abs(e.dot(i)) - o, c > 0 && (h += c * c), c = Math.abs(e.dot(r)) - a, c > 0 && (h += c * c), c = Math.abs(e.dot(s)) - l, c > 0 && (h += c * c), h
                 }
                 computePlaneDistances(t, e, n = [-0, -0]) {
                     let i = Number.POSITIVE_INFINITY,
                         r = Number.NEGATIVE_INFINITY;
                     const s = this.center,
                         o = this.halfAxes,
-                        a = o.getColumn(0, Dx),
-                        l = o.getColumn(1, Nx),
-                        c = o.getColumn(2, Vx),
-                        h = Ux.copy(a).add(l).add(c).add(s),
-                        u = Gx.copy(h).subtract(t);
+                        a = o.getColumn(0, Nx),
+                        l = o.getColumn(1, Vx),
+                        c = o.getColumn(2, Ux),
+                        h = Gx.copy(a).add(l).add(c).add(s),
+                        u = Wx.copy(h).subtract(t);
                     let d = e.dot(u);
                     return i = Math.min(d, i), r = Math.max(d, r), h.copy(s).add(a).add(l).subtract(c), u.copy(h).subtract(t), d = e.dot(u), i = Math.min(d, i), r = Math.max(d, r), h.copy(s).add(a).subtract(l).add(c), u.copy(h).subtract(t), d = e.dot(u), i = Math.min(d, i), r = Math.max(d, r), h.copy(s).add(a).subtract(l).subtract(c), u.copy(h).subtract(t), d = e.dot(u), i = Math.min(d, i), r = Math.max(d, r), s.copy(h).subtract(a).add(l).add(c), u.copy(h).subtract(t), d = e.dot(u), i = Math.min(d, i), r = Math.max(d, r), s.copy(h).subtract(a).add(l).subtract(c), u.copy(h).subtract(t), d = e.dot(u), i = Math.min(d, i), r = Math.max(d, r), s.copy(h).subtract(a).subtract(l).add(c), u.copy(h).subtract(t), d = e.dot(u), i = Math.min(d, i), r = Math.max(d, r), s.copy(h).subtract(a).subtract(l).subtract(c), u.copy(h).subtract(t), d = e.dot(u), i = Math.min(d, i), r = Math.max(d, r), n[0] = i, n[1] = r, n
                 }
                 transform(t) {
                     this.center.transformAsPoint(t);
-                    const e = this.halfAxes.getColumn(0, Dx);
+                    const e = this.halfAxes.getColumn(0, Nx);
                     e.transformAsPoint(t);
-                    const n = this.halfAxes.getColumn(1, Nx);
+                    const n = this.halfAxes.getColumn(1, Vx);
                     n.transformAsPoint(t);
-                    const i = this.halfAxes.getColumn(2, Vx);
-                    return i.transformAsPoint(t), this.halfAxes = new yx([...e, ...n, ...i]), this
+                    const i = this.halfAxes.getColumn(2, Ux);
+                    return i.transformAsPoint(t), this.halfAxes = new _x([...e, ...n, ...i]), this
                 }
                 getTransform() {
                     throw new Error("not implemented")
                 }
             }
-            const Hx = new Ic,
-                Zx = new Ic;
-            class qx {
+            const Zx = new Ic,
+                qx = new Ic;
+            class Xx {
                 constructor(t = [0, 0, 1], e = 0) {
                     wo(this, "normal", void 0), wo(this, "distance", void 0), this.normal = new Ic, this.distance = -0, this.fromNormalDistance(t, e)
                 }
                 fromNormalDistance(t, e) {
                     return gc(Number.isFinite(e)), this.normal.from(t).normalize(), this.distance = e, this
                 }
                 fromPointNormal(t, e) {
-                    t = Hx.from(t), this.normal.from(e).normalize();
+                    t = Zx.from(t), this.normal.from(e).normalize();
                     const n = -this.normal.dot(t);
                     return this.distance = n, this
                 }
                 fromCoefficients(t, e, n, i) {
                     return this.normal.set(t, e, n), gc(uc(this.normal.len(), 1)), this.distance = i, this
                 }
                 clone() {
-                    return new qx(this.normal, this.distance)
+                    return new Xx(this.normal, this.distance)
                 }
                 equals(t) {
                     return uc(this.distance, t.distance) && uc(this.normal, t.normal)
                 }
                 getPointDistance(t) {
                     return this.normal.dot(t) + this.distance
                 }
                 transform(t) {
-                    const e = Zx.copy(this.normal).transformAsVector(t).normalize(),
+                    const e = qx.copy(this.normal).transformAsVector(t).normalize(),
                         n = this.normal.scale(-this.distance).transform(t);
                     return this.fromPointNormal(n, e)
                 }
                 projectPointOntoPlane(t, e = [0, 0, 0]) {
-                    t = Hx.from(t);
+                    t = Zx.from(t);
                     const n = this.getPointDistance(t),
-                        i = Zx.copy(this.normal).scale(n);
+                        i = qx.copy(this.normal).scale(n);
                     return t.subtract(i).to(e)
                 }
             }
-            const Xx = [new Ic([1, 0, 0]), new Ic([0, 1, 0]), new Ic([0, 0, 1])],
-                Yx = new Ic,
-                Kx = new Ic;
-            new qx(new Ic(1, 0, 0), 0);
-            class Qx {
+            const Yx = [new Ic([1, 0, 0]), new Ic([0, 1, 0]), new Ic([0, 0, 1])],
+                Kx = new Ic,
+                Qx = new Ic;
+            new Xx(new Ic(1, 0, 0), 0);
+            class Jx {
                 constructor(t = []) {
                     wo(this, "planes", void 0), this.planes = t
                 }
                 fromBoundingSphere(t) {
-                    this.planes.length = 2 * Xx.length;
+                    this.planes.length = 2 * Yx.length;
                     const e = t.center,
                         n = t.radius;
                     let i = 0;
-                    for (const t of Xx) {
+                    for (const t of Yx) {
                         let r = this.planes[i],
                             s = this.planes[i + 1];
-                        r || (r = this.planes[i] = new qx), s || (s = this.planes[i + 1] = new qx);
-                        const o = Yx.copy(t).scale(-n).add(e);
+                        r || (r = this.planes[i] = new Xx), s || (s = this.planes[i + 1] = new Xx);
+                        const o = Kx.copy(t).scale(-n).add(e);
                         t.dot(o), r.fromPointNormal(o, t);
-                        const a = Yx.copy(t).scale(n).add(e),
-                            l = Kx.copy(t).negate();
+                        const a = Kx.copy(t).scale(n).add(e),
+                            l = Qx.copy(t).negate();
                         l.dot(a), s.fromPointNormal(a, l), i += 2
                     }
                     return this
                 }
                 computeVisibility(t) {
                     let e = 1;
                     for (const n of this.planes) switch (t.intersectPlane(n)) {
-                        case lx:
-                            return lx;
+                        case cx:
+                            return cx;
                         case 0:
                             e = 0
                     }
                     return e
                 }
                 computeVisibilityWithPlaneMask(t, e) {
-                    if (gc(Number.isFinite(e), "parentPlaneMask is required."), e === Qx.MASK_OUTSIDE || e === Qx.MASK_INSIDE) return e;
-                    let n = Qx.MASK_INSIDE;
+                    if (gc(Number.isFinite(e), "parentPlaneMask is required."), e === Jx.MASK_OUTSIDE || e === Jx.MASK_INSIDE) return e;
+                    let n = Jx.MASK_INSIDE;
                     const i = this.planes;
                     for (let r = 0; r < this.planes.length; ++r) {
                         const s = r < 31 ? 1 << r : 0;
                         if (r < 31 && 0 == (e & s)) continue;
                         const o = i[r],
                             a = t.intersectPlane(o);
-                        if (a === lx) return Qx.MASK_OUTSIDE;
+                        if (a === cx) return Jx.MASK_OUTSIDE;
                         0 === a && (n |= s)
                     }
                     return n
                 }
             }
-            wo(Qx, "MASK_OUTSIDE", 4294967295), wo(Qx, "MASK_INSIDE", 0), wo(Qx, "MASK_INDETERMINATE", 2147483647), new Ic, new Ic, new Ic, new Ic, new Ic, new Ic, new Ic, new Ic, new Ic, new Ic, new Ic, new Ic, new Ic, new Ic, new Ic, new Ic, new Ic, Math.PI;
-            const Jx = {
+            wo(Jx, "MASK_OUTSIDE", 4294967295), wo(Jx, "MASK_INSIDE", 0), wo(Jx, "MASK_INDETERMINATE", 2147483647), new Ic, new Ic, new Ic, new Ic, new Ic, new Ic, new Ic, new Ic, new Ic, new Ic, new Ic, new Ic, new Ic, new Ic, new Ic, new Ic, new Ic, Math.PI;
+            const $x = {
                     EPSILON1: .1,
                     EPSILON2: .01,
                     EPSILON3: .001,
                     EPSILON4: 1e-4,
                     EPSILON5: 1e-5,
                     EPSILON6: 1e-6,
                     EPSILON7: 1e-7,
@@ -28329,88 +28332,88 @@
                     EPSILON19: 1e-19,
                     EPSILON20: 1e-20,
                     PI_OVER_TWO: Math.PI / 2,
                     PI_OVER_FOUR: Math.PI / 4,
                     PI_OVER_SIX: Math.PI / 6,
                     TWO_PI: 2 * Math.PI
                 },
-                $x = new yx,
-                tw = new yx,
-                ew = new yx,
-                nw = new yx,
-                iw = new yx;
-            const rw = [1, 0, 0],
-                sw = [2, 2, 1];
+                tw = new _x,
+                ew = new _x,
+                nw = new _x,
+                iw = new _x,
+                rw = new _x;
+            const sw = [1, 0, 0],
+                ow = [2, 2, 1];
 
-            function ow(t) {
+            function aw(t) {
                 let e = 0;
                 for (let n = 0; n < 3; ++n) {
-                    const i = t[$x.getElementIndex(sw[n], rw[n])];
+                    const i = t[tw.getElementIndex(ow[n], sw[n])];
                     e += 2 * i * i
                 }
                 return Math.sqrt(e)
             }
 
-            function aw(t, e) {
-                const n = Jx.EPSILON15;
+            function lw(t, e) {
+                const n = $x.EPSILON15;
                 let i = 0,
                     r = 1;
                 for (let e = 0; e < 3; ++e) {
-                    const n = Math.abs(t[$x.getElementIndex(sw[e], rw[e])]);
+                    const n = Math.abs(t[tw.getElementIndex(ow[e], sw[e])]);
                     n > i && (r = e, i = n)
                 }
-                const s = rw[r],
-                    o = sw[r];
+                const s = sw[r],
+                    o = ow[r];
                 let a = 1,
                     l = 0;
-                if (Math.abs(t[$x.getElementIndex(o, s)]) > n) {
-                    const e = (t[$x.getElementIndex(o, o)] - t[$x.getElementIndex(s, s)]) / 2 / t[$x.getElementIndex(o, s)];
+                if (Math.abs(t[tw.getElementIndex(o, s)]) > n) {
+                    const e = (t[tw.getElementIndex(o, o)] - t[tw.getElementIndex(s, s)]) / 2 / t[tw.getElementIndex(o, s)];
                     let n;
                     n = e < 0 ? -1 / (-e + Math.sqrt(1 + e * e)) : 1 / (e + Math.sqrt(1 + e * e)), a = 1 / Math.sqrt(1 + n * n), l = n * a
                 }
-                return yx.IDENTITY.to(e), e[$x.getElementIndex(s, s)] = e[$x.getElementIndex(o, o)] = a, e[$x.getElementIndex(o, s)] = l, e[$x.getElementIndex(s, o)] = -l, e
+                return _x.IDENTITY.to(e), e[tw.getElementIndex(s, s)] = e[tw.getElementIndex(o, o)] = a, e[tw.getElementIndex(o, s)] = l, e[tw.getElementIndex(s, o)] = -l, e
             }
-            const lw = new Ic,
-                cw = new Ic,
+            const cw = new Ic,
                 hw = new Ic,
                 uw = new Ic,
                 dw = new Ic,
-                pw = new yx,
-                fw = {
-                    diagonal: new yx,
-                    unitary: new yx
+                pw = new Ic,
+                fw = new _x,
+                gw = {
+                    diagonal: new _x,
+                    unitary: new _x
                 },
-                gw = 512,
-                mw = [
+                mw = 512,
+                vw = [
                     [.5, .5],
                     [0, 0],
                     [0, 1],
                     [1, 0],
                     [1, 1]
                 ],
-                vw = mw.concat([
+                bw = vw.concat([
                     [0, .5],
                     [.5, 0],
                     [1, .5],
                     [.5, 1]
                 ]),
-                bw = vw.concat([
+                yw = bw.concat([
                     [.25, .5],
                     [.75, .5]
                 ]);
-            class yw {
+            class _w {
                 constructor(t, e, n) {
                     wo(this, "x", void 0), wo(this, "y", void 0), wo(this, "z", void 0), wo(this, "childVisible", void 0), wo(this, "selected", void 0), wo(this, "_children", void 0), this.x = t, this.y = e, this.z = n
                 }
                 get children() {
                     if (!this._children) {
                         const t = 2 * this.x,
                             e = 2 * this.y,
                             n = this.z + 1;
-                        this._children = [new yw(t, e, n), new yw(t, e + 1, n), new yw(t + 1, e, n), new yw(t + 1, e + 1, n)]
+                        this._children = [new _w(t, e, n), new _w(t, e + 1, n), new _w(t + 1, e, n), new _w(t + 1, e + 1, n)]
                     }
                     return this._children
                 }
                 update(t) {
                     const {
                         viewport: e,
                         cullingVolume: n,
@@ -28440,119 +28443,119 @@
                 getSelected(t = []) {
                     if (this.selected && t.push(this), this._children)
                         for (const e of this._children) e.getSelected(t);
                     return t
                 }
                 insideBounds([t, e, n, i]) {
                     const r = Math.pow(2, this.z),
-                        s = gw / r;
+                        s = mw / r;
                     return this.x * s < n && this.y * s < i && (this.x + 1) * s > t && (this.y + 1) * s > e
                 }
                 getBoundingVolume(t, e, n) {
                     if (n) {
-                        const e = this.z < 1 ? bw : this.z < 2 ? vw : mw,
+                        const e = this.z < 1 ? yw : this.z < 2 ? bw : vw,
                             i = [];
                         for (const r of e) {
-                            const e = Tw(this.x + r[0], this.y + r[1], this.z);
+                            const e = Aw(this.x + r[0], this.y + r[1], this.z);
                             e[2] = t[0], i.push(n(e)), t[0] !== t[1] && (e[2] = t[1], i.push(n(e)))
                         }
-                        return function(t, e = new Wx) {
-                            if (!t || 0 === t.length) return e.halfAxes = new yx([0, 0, 0, 0, 0, 0, 0, 0, 0]), e.center = new Ic, e;
+                        return function(t, e = new Hx) {
+                            if (!t || 0 === t.length) return e.halfAxes = new _x([0, 0, 0, 0, 0, 0, 0, 0, 0]), e.center = new Ic, e;
                             const n = t.length,
                                 i = new Ic(0, 0, 0);
                             for (const e of t) i.add(e);
                             const r = 1 / n;
                             i.multiplyByScalar(r);
                             let s = 0,
                                 o = 0,
                                 a = 0,
                                 l = 0,
                                 c = 0,
                                 h = 0;
                             for (const e of t) {
-                                const t = lw.copy(e).subtract(i);
+                                const t = cw.copy(e).subtract(i);
                                 s += t.x * t.x, o += t.x * t.y, a += t.x * t.z, l += t.y * t.y, c += t.y * t.z, h += t.z * t.z
                             }
                             s *= r, o *= r, a *= r, l *= r, c *= r, h *= r;
-                            const u = pw;
+                            const u = fw;
                             u[0] = s, u[1] = o, u[2] = a, u[3] = o, u[4] = l, u[5] = c, u[6] = a, u[7] = c, u[8] = h;
                             const {
                                 unitary: d
                             } = function(t, e = {}) {
-                                const n = Jx.EPSILON20;
+                                const n = $x.EPSILON20;
                                 let i = 0,
                                     r = 0;
-                                const s = tw,
-                                    o = ew;
+                                const s = ew,
+                                    o = nw;
                                 s.identity(), o.copy(t);
                                 const a = n * function(t) {
                                     let e = 0;
                                     for (let n = 0; n < 9; ++n) {
                                         const i = t[n];
                                         e += i * i
                                     }
                                     return Math.sqrt(e)
                                 }(o);
-                                for (; r < 10 && ow(o) > a;) aw(o, nw), iw.copy(nw).transpose(), o.multiplyRight(nw), o.multiplyLeft(iw), s.multiplyRight(nw), ++i > 2 && (++r, i = 0);
+                                for (; r < 10 && aw(o) > a;) lw(o, iw), rw.copy(iw).transpose(), o.multiplyRight(iw), o.multiplyLeft(rw), s.multiplyRight(iw), ++i > 2 && (++r, i = 0);
                                 return e.unitary = s.toTarget(e.unitary), e.diagonal = o.toTarget(e.diagonal), e
-                            }(u, fw), p = e.halfAxes.copy(d);
-                            let f = p.getColumn(0, hw),
-                                g = p.getColumn(1, uw),
-                                m = p.getColumn(2, dw),
+                            }(u, gw), p = e.halfAxes.copy(d);
+                            let f = p.getColumn(0, uw),
+                                g = p.getColumn(1, dw),
+                                m = p.getColumn(2, pw),
                                 v = -Number.MAX_VALUE,
                                 b = -Number.MAX_VALUE,
                                 y = -Number.MAX_VALUE,
                                 _ = Number.MAX_VALUE,
                                 x = Number.MAX_VALUE,
                                 w = Number.MAX_VALUE;
-                            for (const e of t) lw.copy(e), v = Math.max(lw.dot(f), v), b = Math.max(lw.dot(g), b), y = Math.max(lw.dot(m), y), _ = Math.min(lw.dot(f), _), x = Math.min(lw.dot(g), x), w = Math.min(lw.dot(m), w);
+                            for (const e of t) cw.copy(e), v = Math.max(cw.dot(f), v), b = Math.max(cw.dot(g), b), y = Math.max(cw.dot(m), y), _ = Math.min(cw.dot(f), _), x = Math.min(cw.dot(g), x), w = Math.min(cw.dot(m), w);
                             f = f.multiplyByScalar(.5 * (_ + v)), g = g.multiplyByScalar(.5 * (x + b)), m = m.multiplyByScalar(.5 * (w + y)), e.center.copy(f).add(g).add(m);
-                            const E = cw.set(v - _, b - x, y - w).multiplyByScalar(.5),
-                                P = new yx([E[0], 0, 0, 0, E[1], 0, 0, 0, E[2]]);
+                            const E = hw.set(v - _, b - x, y - w).multiplyByScalar(.5),
+                                P = new _x([E[0], 0, 0, 0, E[1], 0, 0, 0, E[2]]);
                             return e.halfAxes.multiplyRight(P), e
                         }(i)
                     }
                     const i = Math.pow(2, this.z),
-                        r = gw / i,
-                        s = this.x * r + e * gw,
-                        o = gw - (this.y + 1) * r;
-                    return new ux([s, o, t[0]], [s + r, o + r, t[1]])
+                        r = mw / i,
+                        s = this.x * r + e * mw,
+                        o = mw - (this.y + 1) * r;
+                    return new dx([s, o, t[0]], [s + r, o + r, t[1]])
                 }
             }
-            const _w = 512,
-                xw = [-1 / 0, -1 / 0, 1 / 0, 1 / 0],
-                ww = {
+            const xw = 512,
+                ww = [-1 / 0, -1 / 0, 1 / 0, 1 / 0],
+                Ew = {
                     type: "object",
                     value: null,
                     validate: (t, e) => e.optional && null === t || "string" == typeof t || Array.isArray(t) && t.every((t => "string" == typeof t)),
                     equal: (t, e) => {
                         if (t === e) return !0;
                         if (!Array.isArray(t) || !Array.isArray(e)) return !1;
                         const n = t.length;
                         if (n !== e.length) return !1;
                         for (let i = 0; i < n; i++)
                             if (t[i] !== e[i]) return !1;
                         return !0
                     }
                 };
 
-            function Ew(t, e) {
+            function Pw(t, e) {
                 const n = [e.transformAsPoint([t[0], t[1]]), e.transformAsPoint([t[2], t[1]]), e.transformAsPoint([t[0], t[3]]), e.transformAsPoint([t[2], t[3]])];
                 return [Math.min(...n.map((t => t[0]))), Math.min(...n.map((t => t[1]))), Math.max(...n.map((t => t[0]))), Math.max(...n.map((t => t[1])))]
             }
 
-            function Pw({
+            function Sw({
                 viewport: t,
                 z: e = 0,
                 cullRect: n
             }) {
-                return (t.subViewports || [t]).map((t => Sw(t, e, n)))
+                return (t.subViewports || [t]).map((t => Cw(t, e, n)))
             }
 
-            function Sw(t, e, n) {
+            function Cw(t, e, n) {
                 if (!Array.isArray(e)) {
                     const i = n.x - t.x,
                         r = n.y - t.y,
                         {
                             width: s,
                             height: o
                         } = n,
@@ -28561,153 +28564,153 @@
                         },
                         l = t.unproject([i, r], a),
                         c = t.unproject([i + s, r], a),
                         h = t.unproject([i, r + o], a),
                         u = t.unproject([i + s, r + o], a);
                     return [Math.min(l[0], c[0], h[0], u[0]), Math.min(l[1], c[1], h[1], u[1]), Math.max(l[0], c[0], h[0], u[0]), Math.max(l[1], c[1], h[1], u[1])]
                 }
-                const i = Sw(t, e[0], n),
-                    r = Sw(t, e[1], n);
+                const i = Cw(t, e[0], n),
+                    r = Cw(t, e[1], n);
                 return [Math.min(i[0], r[0]), Math.min(i[1], r[1]), Math.max(i[2], r[2]), Math.max(i[3], r[3])]
             }
 
-            function Cw(t, e) {
-                return Math.pow(2, t) * _w / e
+            function Tw(t, e) {
+                return Math.pow(2, t) * xw / e
             }
 
-            function Tw(t, e, n) {
-                const i = Cw(n, _w),
+            function Aw(t, e, n) {
+                const i = Tw(n, xw),
                     r = t / i * 360 - 180,
                     s = Math.PI - 2 * Math.PI * e / i;
                 return [r, 180 / Math.PI * Math.atan(.5 * (Math.exp(s) - Math.exp(-s)))]
             }
 
-            function Aw(t, e, n, i) {
-                const r = Cw(n, i);
-                return [t / r * _w, e / r * _w]
+            function Mw(t, e, n, i) {
+                const r = Tw(n, i);
+                return [t / r * xw, e / r * xw]
             }
 
-            function Mw(t, e, n, i, r = _w) {
+            function Ow(t, e, n, i, r = xw) {
                 if (t.isGeospatial) {
-                    const [t, r] = Tw(e, n, i), [s, o] = Tw(e + 1, n + 1, i);
+                    const [t, r] = Aw(e, n, i), [s, o] = Aw(e + 1, n + 1, i);
                     return {
                         west: t,
                         north: r,
                         east: s,
                         south: o
                     }
                 }
-                const [s, o] = Aw(e, n, i, r), [a, l] = Aw(e + 1, n + 1, i, r);
+                const [s, o] = Mw(e, n, i, r), [a, l] = Mw(e + 1, n + 1, i, r);
                 return {
                     left: s,
                     top: o,
                     right: a,
                     bottom: l
                 }
             }
 
-            function Ow({
+            function Lw({
                 viewport: t,
                 maxZoom: e,
                 minZoom: n,
                 zRange: i,
                 extent: r,
-                tileSize: s = _w,
+                tileSize: s = xw,
                 modelMatrix: o,
                 modelMatrixInverse: a,
                 zoomOffset: l = 0
             }) {
-                let c = t.isGeospatial ? Math.round(t.zoom + Math.log2(_w / s)) + l : Math.ceil(t.zoom) + l;
+                let c = t.isGeospatial ? Math.round(t.zoom + Math.log2(xw / s)) + l : Math.ceil(t.zoom) + l;
                 if ("number" == typeof n && Number.isFinite(n) && c < n) {
                     if (!r) return [];
                     c = n
                 }
                 "number" == typeof e && Number.isFinite(e) && c > e && (c = e);
                 let h = r;
-                return o && a && r && !t.isGeospatial && (h = Ew(r, o)), t.isGeospatial ? function(t, e, n, i) {
-                    const r = t instanceof ox && t.resolution ? t.projectPosition : null,
+                return o && a && r && !t.isGeospatial && (h = Pw(r, o)), t.isGeospatial ? function(t, e, n, i) {
+                    const r = t instanceof ax && t.resolution ? t.projectPosition : null,
                         s = Object.values(t.getFrustumPlanes()).map((({
                             normal: t,
                             distance: e
-                        }) => new qx(t.clone().negate(), e))),
-                        o = new Qx(s),
+                        }) => new Xx(t.clone().negate(), e))),
+                        o = new Jx(s),
                         a = t.distanceScales.unitsPerMeter[2],
                         l = n && n[0] * a || 0,
                         c = n && n[1] * a || 0,
-                        h = t instanceof Rf && t.pitch <= 60 ? e : 0;
+                        h = t instanceof If && t.pitch <= 60 ? e : 0;
                     if (i) {
                         const [t, e, n, r] = i, s = _h([t, r]), o = _h([n, e]);
-                        i = [s[0], gw - s[1], o[0], gw - o[1]]
+                        i = [s[0], mw - s[1], o[0], mw - o[1]]
                     }
-                    const u = new yw(0, 0, 0),
+                    const u = new _w(0, 0, 0),
                         d = {
                             viewport: t,
                             project: r,
                             cullingVolume: o,
                             elevationBounds: [l, c],
                             minZ: h,
                             maxZ: e,
                             bounds: i,
                             offset: 0
                         };
-                    if (u.update(d), t instanceof Rf && t.subViewports && t.subViewports.length > 1) {
+                    if (u.update(d), t instanceof If && t.subViewports && t.subViewports.length > 1) {
                         for (d.offset = -1; u.update(d) && !(--d.offset < -3););
                         for (d.offset = 1; u.update(d) && !(++d.offset > 3););
                     }
                     return u.getSelected()
                 }(t, c, i, r) : function(t, e, n, i, r) {
                     const s = function(t, e, n) {
                             let i;
                             return i = t.getBounds(), t.isGeospatial ? [Math.max(i[0], n[0]), Math.max(i[1], n[1]), Math.min(i[2], n[2]), Math.min(i[3], n[3])] : [Math.max(Math.min(i[0], n[2]), n[0]), Math.max(Math.min(i[1], n[3]), n[1]), Math.min(Math.max(i[2], n[0]), n[2]), Math.min(Math.max(i[3], n[1]), n[3])]
                         }(t, 0, i),
-                        o = Cw(e, n),
+                        o = Tw(e, n),
                         [a, l, c, h] = function(t, e, n) {
-                            return n ? Ew(t, n).map((t => t * e / _w)) : t.map((t => t * e / _w))
+                            return n ? Pw(t, n).map((t => t * e / xw)) : t.map((t => t * e / xw))
                         }(s, o, r),
                         u = [];
                     for (let t = Math.floor(a); t < c; t++)
                         for (let n = Math.floor(l); n < h; n++) u.push({
                             x: t,
                             y: n,
                             z: e
                         });
                     return u
-                }(t, c, s, h || xw, a)
+                }(t, c, s, h || ww, a)
             }
 
-            function Lw(t, e) {
+            function Rw(t, e) {
                 if (t === e) return !0;
                 if (Array.isArray(t)) {
                     const n = t.length;
                     if (!e || e.length !== n) return !1;
                     for (let i = 0; i < n; i++)
                         if (t[i] !== e[i]) return !1;
                     return !0
                 }
                 return !1
             }
-            const Rw = "best-available",
-                Iw = {
-                    [Rw]: function(t) {
+            const Iw = "best-available",
+                kw = {
+                    [Iw]: function(t) {
                         for (const e of t) e.state = 0;
-                        for (const e of t) e.isSelected && !jw(e) && Fw(e);
+                        for (const e of t) e.isSelected && !Fw(e) && zw(e);
                         for (const e of t) e.isVisible = Boolean(2 & e.state)
                     },
                     "no-overlap": function(t) {
                         for (const e of t) e.state = 0;
-                        for (const e of t) e.isSelected && jw(e);
+                        for (const e of t) e.isSelected && Fw(e);
                         const e = Array.from(t).sort(((t, e) => t.zoom - e.zoom));
                         for (const t of e)
                             if (t.isVisible = Boolean(2 & t.state), t.children && (t.isVisible || 1 & t.state))
                                 for (const e of t.children) e.state = 1;
-                            else t.isSelected && Fw(t)
+                            else t.isSelected && zw(t)
                     },
                     never: () => {}
                 },
-                kw = {
+                jw = {
                     extent: null,
                     tileSize: 512,
                     maxZoom: null,
                     minZoom: null,
                     maxCacheSize: null,
                     maxCacheByteSize: null,
                     refinementStrategy: "best-available",
@@ -28715,45 +28718,45 @@
                     maxRequests: 6,
                     zoomOffset: 0,
                     onTileLoad: () => {},
                     onTileUnload: () => {},
                     onTileError: () => {}
                 };
 
-            function jw(t) {
+            function Fw(t) {
                 let e = t;
                 for (; e;) {
                     if (e.isLoaded || e.content) return e.state |= 2, !0;
                     e = e.parent
                 }
                 return !1
             }
 
-            function Fw(t) {
-                for (const e of t.children) e.isLoaded || e.content ? e.state |= 2 : Fw(e)
+            function zw(t) {
+                for (const e of t.children) e.isLoaded || e.content ? e.state |= 2 : zw(e)
             }
-            const zw = {
+            const Bw = {
                 TilesetClass: class {
                     constructor(t) {
                         wo(this, "opts", void 0), wo(this, "_requestScheduler", void 0), wo(this, "_cache", void 0), wo(this, "_dirty", void 0), wo(this, "_tiles", void 0), wo(this, "_cacheByteSize", void 0), wo(this, "_viewport", void 0), wo(this, "_zRange", void 0), wo(this, "_selectedTiles", void 0), wo(this, "_frameNumber", void 0), wo(this, "_modelMatrix", void 0), wo(this, "_modelMatrixInverse", void 0), wo(this, "_maxZoom", void 0), wo(this, "_minZoom", void 0), wo(this, "onTileLoad", void 0), wo(this, "_getCullBounds", function(t) {
                             let e, n = {};
                             return i => {
                                 for (const r in i)
-                                    if (!Lw(i[r], n[r])) {
+                                    if (!Rw(i[r], n[r])) {
                                         e = t(i), n = i;
                                         break
                                     } return e
                             }
-                        }(Pw)), this.opts = {
-                            ...kw,
+                        }(Sw)), this.opts = {
+                            ...jw,
                             ...t
                         }, this.onTileLoad = t => {
                             var e, n;
                             null === (e = (n = this.opts).onTileLoad) || void 0 === e || e.call(n, t), this.opts.maxCacheByteSize && (this._cacheByteSize += t.byteLength, this._resizeCache())
-                        }, this._requestScheduler = new $_({
+                        }, this._requestScheduler = new tx({
                             maxRequests: t.maxRequests,
                             throttleRequests: Boolean(t.maxRequests && t.maxRequests > 0)
                         }), this._cache = new Map, this._tiles = [], this._dirty = !1, this._cacheByteSize = 0, this._viewport = null, this._selectedTiles = null, this._frameNumber = 0, this._modelMatrix = new ih, this._modelMatrixInverse = new ih, this.setOptions(t)
                     }
                     get tiles() {
                         return this._tiles
                     }
@@ -28835,15 +28838,15 @@
                         modelMatrixInverse: s
                     }) {
                         const {
                             tileSize: o,
                             extent: a,
                             zoomOffset: l
                         } = this.opts;
-                        return Ow({
+                        return Lw({
                             viewport: t,
                             maxZoom: e,
                             minZoom: n,
                             zRange: i,
                             tileSize: o,
                             extent: a,
                             modelMatrix: r,
@@ -28858,31 +28861,31 @@
                         return t.z
                     }
                     getTileMetadata(t) {
                         const {
                             tileSize: e
                         } = this.opts;
                         return {
-                            bbox: Mw(this._viewport, t.x, t.y, t.z, e)
+                            bbox: Ow(this._viewport, t.x, t.y, t.z, e)
                         }
                     }
                     getParentIndex(t) {
                         return {
                             x: Math.floor(t.x / 2),
                             y: Math.floor(t.y / 2),
                             z: t.z - 1
                         }
                     }
                     updateTileStates() {
-                        const t = this.opts.refinementStrategy || Rw,
+                        const t = this.opts.refinementStrategy || Iw,
                             e = new Array(this._cache.size);
                         let n = 0;
                         for (const t of this._cache.values()) e[n++] = t.isVisible, t.isSelected = !1, t.isVisible = !1;
                         for (const t of this._selectedTiles) t.isSelected = !0, t.isVisible = !0;
-                        ("function" == typeof t ? t : Iw[t])(Array.from(this._cache.values())), n = 0;
+                        ("function" == typeof t ? t : kw[t])(Array.from(this._cache.values())), n = 0;
                         for (const t of this._cache.values())
                             if (e[n++] !== t.isVisible) return !0;
                         return !1
                     }
                     _pruneRequests() {
                         const {
                             maxRequests: t = 0
@@ -28915,15 +28918,15 @@
                         }
                         this._dirty && (this._tiles = Array.from(this._cache.values()).sort(((t, e) => t.zoom - e.zoom)), this._dirty = !1)
                     }
                     _getTile(t, e) {
                         const n = this.getTileId(t);
                         let i = this._cache.get(n),
                             r = !1;
-                        return !i && e ? (i = new tx(t), Object.assign(i, this.getTileMetadata(i.index)), Object.assign(i, {
+                        return !i && e ? (i = new ex(t), Object.assign(i, this.getTileMetadata(i.index)), Object.assign(i, {
                             id: n,
                             zoom: this.getTileZoom(i.index)
                         }), r = !0, this._cache.set(n, i), this._dirty = !0) : i && i.needsReload && (r = !0), i && r && i.loadData({
                             getData: this.opts.getTileData,
                             requestScheduler: this._requestScheduler,
                             onLoad: this.onTileLoad,
                             onError: this.opts.onTileError
@@ -28942,18 +28945,18 @@
                         return null
                     }
                 },
                 data: {
                     type: "data",
                     value: []
                 },
-                dataComparator: ww.equal,
+                dataComparator: Ew.equal,
                 renderSubLayers: {
                     type: "function",
-                    value: t => new q_(t)
+                    value: t => new X_(t)
                 },
                 getTileData: {
                     type: "function",
                     optional: !0,
                     value: null
                 },
                 onViewportLoad: {
@@ -28980,20 +28983,20 @@
                     compare: !0
                 },
                 tileSize: 512,
                 maxZoom: null,
                 minZoom: 0,
                 maxCacheSize: null,
                 maxCacheByteSize: null,
-                refinementStrategy: Rw,
+                refinementStrategy: Iw,
                 zRange: null,
                 maxRequests: 6,
                 zoomOffset: 0
             };
-            class Bw extends Jb {
+            class Dw extends $b {
                 initializeState() {
                     this.state = {
                         tileset: null,
                         isLoaded: !1
                     }
                 }
                 finalizeState() {
@@ -29156,17 +29159,17 @@
                 }) {
                     const {
                         tile: n
                     } = t.props;
                     return this.state.tileset.isTileVisible(n, e)
                 }
             }
-            wo(Bw, "defaultProps", zw), wo(Bw, "layerName", "TileLayer");
-            var Dw = n(9757),
-                Nw = t => {
+            wo(Dw, "defaultProps", Bw), wo(Dw, "layerName", "TileLayer");
+            var Nw = n(9757),
+                Vw = t => {
                     const [e, n] = (0, c.useState)({
                         displayColorPicker: !1
                     });
                     return (0, o.jsxs)("div", {
                         className: "BioImageViewer-Slider",
                         children: [(0, o.jsxs)("div", {
                             className: "BioImageViewer-Slider__main",
@@ -29253,15 +29256,15 @@
                                 t.onChannelUpdate(Number((e?.target)?.value), t.channel.color, t.channel.visible, t.channel.id)
                             },
                             min: t.channel.min,
                             max: t.channel.max
                         })]
                     })
                 },
-                Vw = t => t.channels.length ? (0, o.jsxs)("div", {
+                Uw = t => t.channels.length ? (0, o.jsxs)("div", {
                     className: "BioImageViewer-ControlPanel",
                     children: [(0, o.jsxs)("h6", {
                         className: "BioImageViewer-ControlPanel__title",
                         children: [(0, o.jsxs)("svg", {
                             width: "20",
                             height: "20",
                             viewBox: "0 0 20 20",
@@ -29290,81 +29293,81 @@
                                 })
                             })]
                         }), "Channel Blending"]
                     }), (0, o.jsx)("ul", {
                         className: "BioImageViewer-ControlPanel__list",
                         children: t.channels.map(((e, n) => (0, o.jsx)("li", {
                             className: "BioImageViewer-ControlPanel__item",
-                            children: (0, o.jsx)(Nw, {
+                            children: (0, o.jsx)(Vw, {
                                 channel: e,
                                 id: n,
                                 onChannelUpdate: t.onChannelUpdate
                             })
                         }, e.id)))
                     })]
                 }) : null;
-            const Uw = {
+            const Gw = {
                     uint8: {
                         bytes: Uint8Array.BYTES_PER_ELEMENT,
-                        format: Dw.Z.RED_INTEGER,
-                        internalFormat: Dw.Z.R8UI,
-                        type: Dw.Z.UNSIGNED_BYTE,
-                        filtering: Dw.Z.NEAREST,
+                        format: Nw.Z.RED_INTEGER,
+                        internalFormat: Nw.Z.R8UI,
+                        type: Nw.Z.UNSIGNED_BYTE,
+                        filtering: Nw.Z.NEAREST,
                         samplerType: "usampler2DArray",
                         max: 255,
                         create: function(t) {
                             return new Uint8Array(t)
                         }
                     },
                     uint16: {
                         bytes: Uint16Array.BYTES_PER_ELEMENT,
-                        format: Dw.Z.RED_INTEGER,
-                        internalFormat: Dw.Z.R16UI,
-                        type: Dw.Z.UNSIGNED_SHORT,
-                        filtering: Dw.Z.NEAREST,
+                        format: Nw.Z.RED_INTEGER,
+                        internalFormat: Nw.Z.R16UI,
+                        type: Nw.Z.UNSIGNED_SHORT,
+                        filtering: Nw.Z.NEAREST,
                         samplerType: "usampler2DArray",
                         max: 65535,
                         create: function(t) {
                             return new Uint16Array(t)
                         }
                     }
                 },
-                Gw = {
+                Ww = {
                     fs: "#version 300 es\n#define SHADER_NAME image-layer-fragment-shader\n#define num_channels CHANNEL_NUMBER\n#define sampler_type SAMPLER_TYPE\n#define normalization_value NORMALIZATION_VALUE\n\nprecision highp sampler_type;\nprecision highp float;\nprecision highp int;\n\nuniform sampler_type texture_arr;\nuniform float intensities[num_channels];\nuniform int channelMapping[num_channels];\nuniform vec4 colors[num_channels];\n\nin vec2 vTexCoord;\n\nvoid main() {\n  vec4 color = vec4(0);\n\n  for (int i = 0; i < num_channels; ++i)\n  {\n    if (channelMapping[i] == -1) continue;\n\n    color += colors[i] * float(texture(texture_arr, vec3(vTexCoord.xy, channelMapping[i])).r) / normalization_value / 255.0 * intensities[i];\n  }\n\n  gl_FragColor = vec4(color.rgb, 1.0);\n  \n  geometry.uv = vTexCoord;\n  DECKGL_FILTER_COLOR(gl_FragColor, geometry);\n}\n",
                     vs: "#version 300 es\n#define SHADER_NAME image-layer-vertex-shader\n\nattribute vec2 texCoords;\nattribute vec3 positions;\nattribute vec3 positions64Low;\nattribute vec3 instancePickingColors;\nvarying vec2 vTexCoord;\n\nvoid main(void) {\n  geometry.worldPosition = positions;\n  geometry.uv = texCoords;\n  geometry.pickingColor = instancePickingColors;\n  gl_Position = project_position_to_clipspace(positions, positions64Low, vec3(0.), geometry.position);\n  DECKGL_FILTER_GL_POSITION(gl_Position, geometry);\n  vTexCoord = texCoords;\n  vec4 color = vec4(0.);\n  DECKGL_FILTER_COLOR(color, geometry);\n}\n"
                 };
-            class Ww extends Fb {
+            class Hw extends zb {
                 constructor(t) {
                     super(t), this.state = {
                         texture: null
                     }
                 }
                 getShaders() {
                     const t = {
-                        ...Gw
+                        ...Ww
                     };
-                    return t.fs = t.fs.replace("CHANNEL_NUMBER", `${this.props.channels.length}`), t.fs = t.fs.replace("SAMPLER_TYPE", Uw[this.props.format].samplerType), t.fs = t.fs.replace("NORMALIZATION_VALUE", Uw[this.props.format].max.toFixed(1)), super.getShaders({
+                    return t.fs = t.fs.replace("CHANNEL_NUMBER", `${this.props.channels.length}`), t.fs = t.fs.replace("SAMPLER_TYPE", Gw[this.props.format].samplerType), t.fs = t.fs.replace("NORMALIZATION_VALUE", Gw[this.props.format].max.toFixed(1)), super.getShaders({
                         ...t,
-                        modules: [ty, ny]
+                        modules: [ey, iy]
                     })
                 }
                 generateTexture(t) {
                     const e = t.createTexture();
-                    return t.activeTexture(t.TEXTURE0), t.bindTexture(t.TEXTURE_2D_ARRAY, e), t.texParameteri(t.TEXTURE_2D_ARRAY, t.TEXTURE_MAG_FILTER, Uw[this.props.format].filtering), t.texParameteri(t.TEXTURE_2D_ARRAY, t.TEXTURE_MIN_FILTER, Uw[this.props.format].filtering), t.texParameteri(t.TEXTURE_2D_ARRAY, t.TEXTURE_WRAP_S, t.CLAMP_TO_EDGE), t.texParameteri(t.TEXTURE_2D_ARRAY, t.TEXTURE_WRAP_T, t.CLAMP_TO_EDGE), t.texImage3D(t.TEXTURE_2D_ARRAY, 0, Uw[this.props.format].internalFormat, this.props.width, this.props.height, this.props.activeChannels, 0, Uw[this.props.format].format, Uw[this.props.format].type, this.props.data), e
+                    return t.activeTexture(t.TEXTURE0), t.bindTexture(t.TEXTURE_2D_ARRAY, e), t.texParameteri(t.TEXTURE_2D_ARRAY, t.TEXTURE_MAG_FILTER, Gw[this.props.format].filtering), t.texParameteri(t.TEXTURE_2D_ARRAY, t.TEXTURE_MIN_FILTER, Gw[this.props.format].filtering), t.texParameteri(t.TEXTURE_2D_ARRAY, t.TEXTURE_WRAP_S, t.CLAMP_TO_EDGE), t.texParameteri(t.TEXTURE_2D_ARRAY, t.TEXTURE_WRAP_T, t.CLAMP_TO_EDGE), t.texImage3D(t.TEXTURE_2D_ARRAY, 0, Gw[this.props.format].internalFormat, this.props.width, this.props.height, this.props.activeChannels, 0, Gw[this.props.format].format, Gw[this.props.format].type, this.props.data), e
                 }
                 initializeState() {
                     const {
                         gl: t
                     } = this.context;
-                    t.pixelStorei(Dw.Z.UNPACK_ALIGNMENT, 1), t.pixelStorei(Dw.Z.PACK_ALIGNMENT, 1);
+                    t.pixelStorei(Nw.Z.UNPACK_ALIGNMENT, 1), t.pixelStorei(Nw.Z.PACK_ALIGNMENT, 1);
                     const e = this.getAttributeManager();
                     e?.add({
                         positions: {
                             size: 3,
-                            type: Dw.Z.DOUBLE,
+                            type: Nw.Z.DOUBLE,
                             fp64: this.use64bitPositions(),
                             update: this.calculatePositions,
                             noAlloc: !0
                         }
                     }), this.setState({
                         numInstances: 1,
                         positions: new Float64Array(12)
@@ -29402,19 +29405,19 @@
                             model: this._getModel(t)
                         }), this.getAttributeManager()?.invalidateAll()
                     }
                     const r = this.getAttributeManager();
                     t.bounds !== e.bounds && r?.invalidate("positions")
                 }
                 _getModel(t) {
-                    return t ? new Yv(t, {
+                    return t ? new Kv(t, {
                         ...this.getShaders(),
                         id: this.props.id,
-                        geometry: new ry({
-                            drawMode: Dw.Z.TRIANGLE_FAN,
+                        geometry: new sy({
+                            drawMode: Nw.Z.TRIANGLE_FAN,
                             vertexCount: 4,
                             attributes: {
                                 texCoords: new Float32Array([0, 1, 0, 0, 1, 0, 1, 1])
                             }
                         }),
                         isInstanced: !1
                     }) : null
@@ -29440,28 +29443,28 @@
                             intensities: this.props.channels.map((t => t.intensity)),
                             channelMapping: this.props.channelMapping,
                             colors: this.props.channels.map((t => t.color)).flat()
                         }).draw()
                     }
                 }
             }
-            Ww.layerName = "ImageLayer", Ww.defaultProps = {
+            Hw.layerName = "ImageLayer", Hw.defaultProps = {
                 bounds: [],
                 pickable: !1,
                 coordinateSystem: Lh.CARTESIAN,
                 data: null,
                 width: 0,
                 height: 0,
                 format: "uint8",
                 channels: [],
                 channelMapping: [],
                 activeChannels: 0
             };
-            var Hw = Ww;
-            class Zw extends Bw {
+            var Zw = Hw;
+            class qw extends Dw {
                 constructor(t) {
                     super(t)
                 }
                 shouldUpdateState({
                     props: t,
                     oldProps: e,
                     context: n,
@@ -29511,66 +29514,66 @@
                 renderSubLayers(t) {
                     const {
                         left: e,
                         bottom: n,
                         right: i,
                         top: r
                     } = t.tile.bbox;
-                    return new Hw({
+                    return new Zw({
                         id: t.id,
                         data: t.data?.data,
                         width: t.data?.width,
                         height: t.data?.height,
                         format: this.props.format,
                         channels: this.props.channels,
                         activeChannels: t.data.channels,
                         channelMapping: this.props.channelMapping,
                         bounds: [cc(e, 0, t.extent[2]), cc(n, 0, t.extent[3]), cc(i, 0, t.extent[2]), cc(r, 0, t.extent[3])]
                     })
                 }
             }
-            Zw.defaultProps = {
+            qw.defaultProps = {
                 api: "",
                 namespace: "",
                 metadata: [],
                 channels: [],
                 channelRanges: [],
                 channelMapping: [],
                 format: "uint8"
             };
-            var qw = Zw,
-                Xw = class {
+            var Xw = qw,
+                Yw = class {
                     constructor(t, e) {
                         this.baseAxes = t, this.targetAxes = e
                     }
                     reshape(t) {
                         const e = new Array(this.baseAxes.length);
                         for (let n = 0; n < this.baseAxes.length; ++n) e[this.targetAxes.indexOf(this.baseAxes[n])] = t[n];
                         return e
                     }
                 },
-                Yw = class {
+                Kw = class {
                     constructor(t, e, n, i, r, s) {
                         this.downsample = t, this.width = e, this.height = n, this.id = i, this.axes = r, this.zoom_level = s
                     }
                 },
-                Kw = t => {
+                Qw = t => {
                     const {
                         tooltipText: e,
                         children: n
                     } = t;
                     return (0, o.jsxs)("div", {
                         className: "BIV-Tooltip",
                         children: [n, (0, o.jsx)("div", {
                             className: "BIV-Tooltip__content",
                             children: e
                         })]
                     })
                 },
-                Qw = t => {
+                Jw = t => {
                     const {
                         setZoom: e,
                         zoom: n,
                         resetControls: i
                     } = t, r = (0, c.useCallback)((() => {
                         e(n + .1)
                     }), [e]), s = (0, c.useCallback)((() => {
@@ -29578,15 +29581,15 @@
                     }), [e]), a = (0, c.useMemo)((() => (t => {
                         if (void 0 === t) return "-";
                         const e = 100 * Math.pow(2, t);
                         return `${Math.floor(e)}%`
                     })(n)), [n]);
                     return (0, o.jsxs)("div", {
                         className: "BIV-ZoomControls",
-                        children: [(0, o.jsx)(Kw, {
+                        children: [(0, o.jsx)(Qw, {
                             tooltipText: "Zoom in +",
                             children: (0, o.jsx)("button", {
                                 className: "BIV-ZoomControls__button",
                                 onClick: r,
                                 children: (0, o.jsx)("svg", {
                                     width: "20",
                                     height: "20",
@@ -29596,15 +29599,15 @@
                                     children: (0, o.jsx)("path", {
                                         d: "M10.0261 18.3333C10.2671 18.3333 10.4851 18.2732 10.6803 18.1529C10.8754 18.0325 11.034 17.8776 11.156 17.6881C11.2749 17.4986 11.3344 17.2941 11.3344 17.0745V11.2949H17.0524C17.2811 11.2949 17.493 11.2362 17.6882 11.1189C17.8834 11.0016 18.0404 10.8452 18.1593 10.6497C18.2752 10.4542 18.3332 10.2376 18.3332 9.99999C18.3332 9.76538 18.2737 9.55182 18.1548 9.35931C18.0358 9.1638 17.8773 9.00589 17.679 8.88557C17.4808 8.76526 17.2673 8.7051 17.0386 8.7051H11.3161V2.93448C11.3161 2.70588 11.2551 2.49683 11.1331 2.30734C11.0112 2.11483 10.851 1.95992 10.6528 1.84262C10.4546 1.72531 10.235 1.66666 9.99412 1.66666C9.76235 1.66666 9.54736 1.72381 9.34914 1.83811C9.14786 1.95241 8.98776 2.10581 8.86883 2.29831C8.7499 2.48781 8.69043 2.69535 8.69043 2.92095V8.68705H2.95876C2.73309 8.68705 2.52343 8.74571 2.32979 8.86301C2.13156 8.98032 1.97146 9.13673 1.84948 9.33224C1.7275 9.52475 1.6665 9.7368 1.6665 9.96841C1.6665 10.206 1.72597 10.4211 1.8449 10.6136C1.96384 10.8061 2.12241 10.961 2.32064 11.0783C2.51581 11.1926 2.72547 11.2498 2.94961 11.2498H8.67671V17.0249C8.67671 17.2445 8.73465 17.4475 8.85053 17.634C8.96641 17.8205 9.12499 17.9739 9.32626 18.0942C9.52449 18.2115 9.73796 18.2702 9.96667 18.2702L10.0261 18.3333Z",
                                         fill: "black",
                                         fillOpacity: "0.7"
                                     })
                                 })
                             })
-                        }), (0, o.jsx)(Kw, {
+                        }), (0, o.jsx)(Qw, {
                             tooltipText: "Zoom out -",
                             children: (0, o.jsx)("button", {
                                 className: "BIV-ZoomControls__button",
                                 onClick: s,
                                 children: (0, o.jsxs)("svg", {
                                     width: "20",
                                     height: "20",
@@ -29630,15 +29633,15 @@
                                         })
                                     })]
                                 })
                             })
                         }), (0, o.jsx)("p", {
                             className: "BIV-ZoomControls__label",
                             children: a
-                        }), (0, o.jsx)(Kw, {
+                        }), (0, o.jsx)(Qw, {
                             tooltipText: "Reset zoom level",
                             children: (0, o.jsx)("button", {
                                 className: "BIV-ZoomControls__button",
                                 onClick: i,
                                 children: (0, o.jsx)("svg", {
                                     width: "20",
                                     height: "20",
@@ -29651,24 +29654,24 @@
                                         fillOpacity: "0.7"
                                     })
                                 })
                             })
                         })]
                     })
                 },
-                Jw = (t, e, n = !1) => {
+                $w = (t, e, n = !1) => {
                     let i;
                     return (...r) => {
                         const s = n && !i;
                         clearTimeout(i), i = setTimeout((function() {
                             i = null, n || t(...r)
                         }), e), s && t(...r)
                     }
                 },
-                $w = t => {
+                tE = t => {
                     const {
                         groupNamespace: e,
                         groupID: n,
                         client: i,
                         onLoad: r
                     } = t, s = (0, c.useRef)(null), [a, l] = (0, c.useState)({
                         loaded: !1,
@@ -29697,73 +29700,73 @@
                                 type: e.type,
                                 value: e.value
                             }, t)), {}))), t.groups.API.getGroupContents(e, n).then((t => t.data.entries)).then((t => t.reduce(((t, e) => (t[e.array.name] = e.array.id, t)), {})))]);
                             let o = 0,
                                 a = 0;
                             const l = [];
                             for (const t of JSON.parse(String.fromCharCode(...r.levels.value)).reverse()) {
-                                const e = new Xw(t.axes, "XYC"),
+                                const e = new Yw(t.axes, "XYC"),
                                     [n, i] = e.reshape(t.shape);
                                 let r = 2;
                                 o > 0 && (r = Math.round(n / o)), o = n;
                                 const c = Math.log2(r);
                                 if (c !== Math.round(c)) return alert("Only power of two zoom factors are supported"), [];
                                 for (const e of Array.from({
                                         length: c
-                                    }, ((t, e) => Math.pow(2, e))).reverse()) l.push(new Yw(e, n, i, s[t.name], t.axes, a)), a += 1
+                                    }, ((t, e) => Math.pow(2, e))).reverse()) l.push(new Kw(e, n, i, s[t.name], t.axes, a)), a += 1
                             }
                             return i(JSON.parse(String.fromCharCode(...r.channels.value))), l
                         })(i, e, n, t.onChannelsLoaded).then((t => {
                             l((e => ({
                                 ...e,
                                 metadata: t,
                                 target: [t[0].width / 2, t[0].height / 2, 0],
                                 loaded: !0
                             }))), r?.(), s.current = a
                         })).catch((e => {
                             t.errorHandler?.(e)
                         })))
                     }), [e, n]);
-                    const h = (0, c.useMemo)((() => new Qb({
+                    const h = (0, c.useMemo)((() => new Jb({
                             id: "ortho",
                             controller: {
                                 scrollZoom: {
                                     speed: .01,
                                     smooth: !0
                                 },
                                 inertia: !0,
                                 doubleClickZoom: !1
                             }
-                        })), [Qb]),
-                        u = (0, c.useMemo)((() => Jw((t => {
+                        })), [Jb]),
+                        u = (0, c.useMemo)((() => $w((t => {
                             l((e => ({
                                 ...e,
                                 ...t.viewState
                             })))
-                        }), 200)), [Jw]);
+                        }), 200)), [$w]);
                     return t.channels.length ? (0, o.jsxs)("div", {
                         className: "BioImageViewer__main",
-                        children: [(0, o.jsx)(Qw, {
+                        children: [(0, o.jsx)(Jw, {
                             resetControls: () => {
                                 s.current && l((t => ({
                                     ...t,
                                     zoom: s.current?.zoom
                                 })))
                             },
                             orthographicView: h,
                             zoom: a.zoom,
                             setZoom: t => {
                                 l((e => ({
                                     ...e,
                                     zoom: t
                                 })))
                             }
-                        }), a.loaded && (0, o.jsx)(Wb, {
+                        }), a.loaded && (0, o.jsx)(Hb, {
                             views: [h],
-                            layers: [new qw({
+                            layers: [new Xw({
                                 tileSize: 1024,
                                 minZoom: a.metadata[0].zoom_level,
                                 maxZoom: a.metadata.at(-1)?.zoom_level,
                                 coordinateSystem: Lh.CARTESIAN,
                                 extent: [0, 0, a.metadata[0].width, a.metadata[0].height],
                                 metadata: a.metadata,
                                 namespace: t.groupNamespace,
@@ -29781,19 +29784,19 @@
                                 zoom: a.zoom,
                                 minZoom: -2,
                                 maxZoom: a.metadata.at(-1)?.zoom_level
                             }
                         })]
                     }) : null
                 };
-            const tE = "https://api.tiledb.com";
-            var eE = t => {
+            const eE = "https://api.tiledb.com";
+            var nE = t => {
                 const {
                     apiKey: e,
-                    basePath: n = tE,
+                    basePath: n = eE,
                     namespace: i,
                     groupID: r,
                     onLoad: s,
                     onError: a
                 } = t, [l, h] = (0, c.useState)({
                     format: null,
                     channels: [],
@@ -29803,15 +29806,15 @@
                     apiKey: e,
                     basePath: n
                 }, p = new(d())(u);
                 return (0, o.jsxs)("div", {
                     className: "BioImageViewer__container",
                     children: [(0, o.jsx)("div", {
                         className: "BioImageViewer__controls",
-                        children: (0, o.jsx)(Vw, {
+                        children: (0, o.jsx)(Uw, {
                             channels: l.channels,
                             onChannelUpdate: (t, e, n, i) => {
                                 let r = !1;
                                 const s = l.channels.map((s => s.id === i ? (s.visible !== n && (r = !0), s.intensity = t, s.color = e, s.visible = n, s) : s));
                                 if (r) {
                                     const t = [],
                                         e = [];
@@ -29826,15 +29829,15 @@
                                 }
                                 h((t => ({
                                     ...t,
                                     channels: s
                                 })))
                             }
                         })
-                    }), (0, o.jsx)($w, {
+                    }), (0, o.jsx)(tE, {
                         onLoad: s,
                         client: p,
                         groupNamespace: i,
                         groupID: r,
                         basePath: n,
                         channels: l.channels,
                         channelRanges: l.channelRanges,
@@ -29849,15 +29852,15 @@
                                 channelMapping: Array.from(Array(t.channels.length).keys())
                             })))
                         },
                         errorHandler: a
                     })]
                 })
             };
-            class nE extends h().Component {
+            class iE extends h().Component {
                 constructor(t) {
                     super(t), this.state = {
                         error: void 0
                     }
                 }
                 static getDerivedStateFromError(t) {
                     return {
@@ -29867,20 +29870,20 @@
                 componentDidCatch(t, e) {
                     this.props.errorHandler?.(t)
                 }
                 render() {
                     return this.state.error && this.props.errorState ? this.props.errorState(this.state.error) : this.props.children
                 }
             }
-            var iE = nE,
-                rE = t => {
+            var rE = iE,
+                sE = t => {
                     let e;
-                    e = "string" == typeof t.rootElement ? document.getElementById(t.rootElement) : t.rootElement, l().render((0, o.jsx)(iE, {
+                    e = "string" == typeof t.rootElement ? document.getElementById(t.rootElement) : t.rootElement, l().render((0, o.jsx)(rE, {
                         errorHandler: t.onError,
-                        children: (0, o.jsx)(eE, {
+                        children: (0, o.jsx)(nE, {
                             apiKey: t.apiKey,
                             groupID: t.groupID,
                             namespace: t.namespace,
                             onError: t.onError,
                             basePath: t.basePath,
                             onLoad: t.onLoad
                         })
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/633.86ebe895050415abdfba.js` & `tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/labextension/static/633.770b26571c8b948a69e3.js`

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
-                    let v = 0;
-                    if ("number" == typeof d[p][0]) v = d[p][1] - d[p][0] + 1;
+                    let b = 0;
+                    if ("number" == typeof d[p][0]) b = d[p][1] - d[p][0] + 1;
                     else
-                        for (const e of d[p]) v += e[1] - e[0] + 1;
-                    const m = {
+                        for (const e of d[p]) b += e[1] - e[0] + 1;
+                    const v = {
                             layout: "row-major",
                             ranges: d,
-                            bufferSize: Math.pow(l * a, 2) * v * o[f].bytes,
+                            bufferSize: Math.pow(l * a, 2) * b * o[f].bytes,
                             attributes: ["intensity"],
                             returnRawBuffers: !0
                         },
-                        b = r.query.ReadQuery(e.data.namespace, e.data.levelUri, m),
-                        g = o[f].create(await b.next().then((e => e.value.intensity))),
-                        w = o[f].create(y * h * v),
+                        m = r.query.ReadQuery(e.data.namespace, e.data.levelUri, v),
+                        g = o[f].create(await m.next().then((e => e.value.intensity))),
+                        w = o[f].create(y * h * b),
                         E = new Array(3);
                     for (let e = 0; e < d.length; ++e) E[e] = d[e][1] - d[e][0] + 1;
                     1 === a ? self.postMessage({
                         data: g,
                         width: y,
                         height: h,
-                        channels: v
+                        channels: b
                     }, [g.buffer]) : (g.forEach(((e, t) => {
                         const r = new Array(3);
                         r[0] = ~~(t / (E[1] * E[2])), r[1] = ~~(t % (E[1] * E[2]) / E[2]), r[2] = t % E[2];
                         const n = (r[p] * h + ~~(r[u] / a)) * y + ~~(r[c] / a);
                         w[n] = e
                     })), self.postMessage({
                         data: w,
                         width: y,
                         height: h,
-                        channels: v
+                        channels: b
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
-    }, n.f = {}, n.e = e => Promise.all(Object.keys(n.f).reduce(((t, r) => (n.f[r](e, t), t)), [])), n.u = e => e + ".ce138c9764842046bf90.js?v=ce138c9764842046bf90", n.g = function() {
+    }, n.f = {}, n.e = e => Promise.all(Object.keys(n.f).reduce(((t, r) => (n.f[r](e, t), t)), [])), n.u = e => e + ".024275f22a135fe53126.js?v=024275f22a135fe53126", n.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), n.o = (e, t) => Object.prototype.hasOwnProperty.call(e, t), n.r = e => {
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/635.ce138c9764842046bf90.js` & `tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 635.ce138c9764842046bf90.js.LICENSE.txt */
+/*! For license information please see 635.024275f22a135fe53126.js.LICENSE.txt */
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
-        5659: (t, e, r) => {
+        404: (t, e, r) => {
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
-            var u = r(5659);
+            var u = r(404);
             e.Float64List = u.Float64List;
             var p = r(1273);
             e.Int8List = p.Int8List;
             var d = r(1802);
             e.Int16List = d.Int16List;
             var l = r(5452);
             e.Int32List = l.Int32List;
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/635.ce138c9764842046bf90.js.LICENSE.txt` & `tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/713.44bebcfa12a45c30ff83.js` & `tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/labextension/static/713.44bebcfa12a45c30ff83.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/744.9655cb2c54e12e1c2654.js` & `tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/labextension/static/744.3b4d2f36290dd421bc4f.js`

 * *Files 15% similar despite different names*

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
-            e.exports = JSON.parse('{"name":"@tiledb-inc/jupyter-bioimage-viewer","version":"0.1.1-alpha.2","description":"A jupyterlab extension to visualize bioimages in TileDB format","keywords":["jupyter","jupyterlab","jupyterlab-extension"],"homepage":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer","bugs":{"url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer/issues"},"license":"BSD-3-Clause","author":"TileDB","files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","style/*.css","style/index.js"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","repository":{"type":"git","url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer.git"},"scripts":{"test":"echo No tests yet","build":"jlpm run build:lib && jlpm run build:labextension:dev","build:prod":"jlpm run build:lib && jlpm run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","clean":"jlpm run clean:lib","clean:lib":"rimraf lib tsconfig.tsbuildinfo","clean:labextension":"rimraf tiledb_jupyter_bioimg/labextension","clean:all":"jlpm run clean:lib && jlpm run clean:labextension","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:extension":"jupyter labextension develop --overwrite .","prepare":"jlpm run clean && jlpm run build:prod","watch":"run-p watch:src watch:labextension","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4","@jupyterlab/application":"^3.4.5","@tiledb-inc/bioimage-viewer":"^0.1.0-alpha.7"},"devDependencies":{"@jupyterlab/builder":"^3.1.0","@typescript-eslint/eslint-plugin":"^2.27.0","@typescript-eslint/parser":"^2.27.0","eslint":"^7.5.0","eslint-config-prettier":"^6.10.1","eslint-plugin-prettier":"^3.1.2","npm-run-all":"^4.1.5","prettier":"^1.19.0","rimraf":"^3.0.2","typescript":"~4.1.3"},"sideEffects":["style/*.css","style/index.js"],"styleModule":"style/index.js","jupyterlab":{"extension":"lib/index","outputDir":"tiledb_jupyter_bioimg/labextension","webpackConfig":"./webpack.config.js"}}')
+            e.exports = JSON.parse('{"name":"@tiledb-inc/jupyter-bioimage-viewer","version":"0.1.1-alpha.3","description":"A jupyterlab extension to visualize bioimages in TileDB format","keywords":["jupyter","jupyterlab","jupyterlab-extension"],"homepage":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer","bugs":{"url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer/issues"},"license":"BSD-3-Clause","author":"TileDB","files":["lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}","style/**/*.{css,.js,eot,gif,html,jpg,json,png,svg,woff2,ttf}","style/*.css","style/index.js"],"main":"lib/index.js","types":"lib/index.d.ts","style":"style/index.css","repository":{"type":"git","url":"https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer.git"},"scripts":{"test":"echo No tests yet","build":"jlpm run build:lib && jlpm run build:labextension:dev","build:prod":"jlpm run build:lib && jlpm run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","clean":"jlpm run clean:lib","clean:lib":"rimraf lib tsconfig.tsbuildinfo","clean:labextension":"rimraf tiledb_jupyter_bioimg/labextension","clean:all":"jlpm run clean:lib && jlpm run clean:labextension","eslint":"eslint . --ext .ts,.tsx --fix","eslint:check":"eslint . --ext .ts,.tsx","install:extension":"jupyter labextension develop --overwrite .","prepare":"jlpm run clean && jlpm run build:prod","watch":"run-p watch:src watch:labextension","watch:src":"tsc -w","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4","@jupyterlab/application":"^3.4.5","@tiledb-inc/bioimage-viewer":"^0.1.0-alpha.7"},"devDependencies":{"@jupyterlab/builder":"^3.1.0","@typescript-eslint/eslint-plugin":"^2.27.0","@typescript-eslint/parser":"^2.27.0","eslint":"^7.5.0","eslint-config-prettier":"^6.10.1","eslint-plugin-prettier":"^3.1.2","npm-run-all":"^4.1.5","prettier":"^1.19.0","rimraf":"^3.0.2","typescript":"~4.1.3"},"resolutions":{"@luma.gl/constants":"8.5.16","@luma.gl/core":"8.5.16","@luma.gl/engine":"8.5.16","@luma.gl/gltools":"8.5.16","@luma.gl/shadertools":"8.5.16","@luma.gl/webgl":"8.5.16","@luma.gl/experimental":"8.5.16"},"sideEffects":["style/*.css","style/index.js"],"styleModule":"style/index.js","jupyterlab":{"extension":"lib/index","outputDir":"tiledb_jupyter_bioimg/labextension","webpackConfig":"./webpack.config.js"}}')
         }
     }
 ]);
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js` & `tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/remoteEntry.f05f71ea95cf3364c4cb.js` & `tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/labextension/static/remoteEntry.ad93eef0e33172dacb16.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, n, i, o, d, l, u, f, s, c, p, h, b, v, m, g, y = {
+    var e, r, t, a, n, i, o, d, l, u, s, c, f, p, b, h, v, m, g, y = {
             5290: (e, r, t) => {
                 var a = {
                         "./index": () => t.e(744).then((() => () => t(1744))),
                         "./extension": () => t.e(744).then((() => () => t(1744))),
                         "./style": () => t.e(747).then((() => () => t(9747)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
@@ -46,30 +46,30 @@
         for (var t in r) j.o(r, t) && !j.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
         38: "06c00f555d53e8ae5aa5",
         172: "6267f3dd3063477e34ed",
-        344: "8db93920a8ca0f0600d9",
+        344: "8d6b91ad4356dae38b22",
         446: "3bf34f45c93ace9c0f28",
-        633: "86ebe895050415abdfba",
-        635: "ce138c9764842046bf90",
+        633: "770b26571c8b948a69e3",
+        635: "024275f22a135fe53126",
         713: "44bebcfa12a45c30ff83",
-        744: "9655cb2c54e12e1c2654",
+        744: "3b4d2f36290dd421bc4f",
         747: "433530952542f03ebc71"
     } [e] + ".js?v=" + {
         38: "06c00f555d53e8ae5aa5",
         172: "6267f3dd3063477e34ed",
-        344: "8db93920a8ca0f0600d9",
+        344: "8d6b91ad4356dae38b22",
         446: "3bf34f45c93ace9c0f28",
-        633: "86ebe895050415abdfba",
-        635: "ce138c9764842046bf90",
+        633: "770b26571c8b948a69e3",
+        635: "024275f22a135fe53126",
         713: "44bebcfa12a45c30ff83",
-        744: "9655cb2c54e12e1c2654",
+        744: "3b4d2f36290dd421bc4f",
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
-                    var f = l[u];
-                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + n) {
-                        o = f;
+                    var s = l[u];
+                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + n) {
+                        o = s;
                         break
                     }
                 }
             o || (d = !0, (o = document.createElement("script")).charset = "utf-8", o.timeout = 120, j.nc && o.setAttribute("nonce", j.nc), o.setAttribute("data-webpack", r + n), o.src = t), e[t] = [a];
-            var s = (r, a) => {
-                    o.onerror = o.onload = null, clearTimeout(c);
+            var c = (r, a) => {
+                    o.onerror = o.onload = null, clearTimeout(f);
                     var n = e[t];
                     if (delete e[t], o.parentNode && o.parentNode.removeChild(o), n && n.forEach((e => e(a))), r) return r(a)
                 },
-                c = setTimeout(s.bind(null, void 0, {
+                f = setTimeout(c.bind(null, void 0, {
                     type: "timeout",
                     target: o
                 }), 12e4);
-            o.onerror = s.bind(null, o.onerror), o.onload = s.bind(null, o.onload), d && document.head.appendChild(o)
+            o.onerror = c.bind(null, o.onerror), o.onload = c.bind(null, o.onload), d && document.head.appendChild(o)
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
-                return "default" === t && (d("@jupyter-widgets/base", "4.1.1", (() => Promise.all([j.e(172), j.e(713), j.e(38)]).then((() => () => j(2713))))), d("@tiledb-inc/bioimage-viewer", "0.1.0-alpha.7", (() => Promise.all([j.e(635), j.e(172), j.e(344), j.e(446)]).then((() => () => j(344))))), d("@tiledb-inc/jupyter-bioimage-viewer", "0.1.1-alpha.2", (() => j.e(744).then((() => () => j(1744)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (d("@jupyter-widgets/base", "4.1.1", (() => Promise.all([j.e(172), j.e(713), j.e(38)]).then((() => () => j(2713))))), d("@tiledb-inc/bioimage-viewer", "0.1.0-alpha.7", (() => Promise.all([j.e(635), j.e(172), j.e(344), j.e(446)]).then((() => () => j(344))))), d("@tiledb-inc/jupyter-bioimage-viewer", "0.1.1-alpha.3", (() => j.e(744).then((() => () => j(1744)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -185,75 +185,75 @@
     }, i = (e, r) => {
         if (0 in e) {
             r = t(r);
             var a = e[0],
                 n = a < 0;
             n && (a = -a - 1);
             for (var o = 0, d = 1, l = !0;; d++, o++) {
-                var u, f, s = d < e.length ? (typeof e[d])[0] : "";
-                if (o >= r.length || "o" == (f = (typeof(u = r[o]))[0])) return !l || ("u" == s ? d > a && !n : "" == s != n);
-                if ("u" == f) {
-                    if (!l || "u" != s) return !1
+                var u, s, c = d < e.length ? (typeof e[d])[0] : "";
+                if (o >= r.length || "o" == (s = (typeof(u = r[o]))[0])) return !l || ("u" == c ? d > a && !n : "" == c != n);
+                if ("u" == s) {
+                    if (!l || "u" != c) return !1
                 } else if (l)
-                    if (s == f)
+                    if (c == s)
                         if (d <= a) {
                             if (u != e[d]) return !1
                         } else {
                             if (n ? u > e[d] : u < e[d]) return !1;
                             u != e[d] && (l = !1)
                         }
-                else if ("s" != s && "n" != s) {
+                else if ("s" != c && "n" != c) {
                     if (n || d <= a) return !1;
                     l = !1, d--
                 } else {
-                    if (d <= a || f < s != n) return !1;
+                    if (d <= a || s < c != n) return !1;
                     l = !1
-                } else "s" != s && "n" != s && (l = !1, d--)
+                } else "s" != c && "n" != c && (l = !1, d--)
             }
         }
-        var c = [],
-            p = c.pop.bind(c);
+        var f = [],
+            p = f.pop.bind(f);
         for (o = 1; o < e.length; o++) {
-            var h = e[o];
-            c.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? i(h, r) : !p())
+            var b = e[o];
+            f.push(1 == b ? p() | p() : 2 == b ? p() & p() : b ? i(b, r) : !p())
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
-        return i(a, n) || s(l(e, t, n, a)), c(e[t][n])
-    }, f = (e, r, t) => {
+        return i(a, n) || c(l(e, t, n, a)), f(e[t][n])
+    }, s = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !i(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
-    }, s = e => {
+    }, c = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, c = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, a, n) {
+    }, f = e => (e.loaded = 1, e.get()), b = (p = e => function(r, t, a, n) {
         var i = j.I(r);
         return i && i.then ? i.then(e.bind(e, r, j.S[r], t, a, n)) : e(r, j.S[r], t, a, n)
-    })(((e, r, t, a) => (o(e, t), u(r, 0, t, a)))), b = p(((e, r, t, a, n) => {
-        var i = r && j.o(r, t) && f(r, t, a);
-        return i ? c(i) : n()
+    })(((e, r, t, a) => (o(e, t), u(r, 0, t, a)))), h = p(((e, r, t, a, n) => {
+        var i = r && j.o(r, t) && s(r, t, a);
+        return i ? f(i) : n()
     })), v = {}, m = {
-        2832: () => b("default", "@tiledb-inc/bioimage-viewer", [2, 0, 1, 0, , "alpha", 7], (() => Promise.all([j.e(635), j.e(172), j.e(344), j.e(446)]).then((() => () => j(344))))),
-        8233: () => b("default", "@jupyter-widgets/base", [, [1, 4],
+        2832: () => h("default", "@tiledb-inc/bioimage-viewer", [2, 0, 1, 0, , "alpha", 7], (() => Promise.all([j.e(635), j.e(172), j.e(344), j.e(446)]).then((() => () => j(344))))),
+        8233: () => h("default", "@jupyter-widgets/base", [, [1, 4],
             [1, 3],
             [1, 2],
             [1, 1, 1, 10], 1, 1, 1
         ], (() => Promise.all([j.e(172), j.e(713), j.e(38)]).then((() => () => j(2713))))),
-        1526: () => h("default", "@lumino/coreutils", [1, 1, 11, 0]),
-        2720: () => h("default", "@lumino/messaging", [1, 1, 10, 0]),
-        8832: () => h("default", "@lumino/widgets", [1, 1, 37, 2]),
-        4456: () => h("default", "react-dom", [1, 17, 0, 1]),
-        6271: () => h("default", "react", [1, 17, 0, 1])
+        1526: () => b("default", "@lumino/coreutils", [1, 1, 11, 0]),
+        2720: () => b("default", "@lumino/messaging", [1, 1, 10, 0]),
+        8832: () => b("default", "@lumino/widgets", [1, 1, 37, 2]),
+        4456: () => b("default", "react-dom", [1, 17, 0, 1]),
+        6271: () => b("default", "react", [1, 17, 0, 1])
     }, g = {
         38: [1526, 2720, 8832],
         446: [4456, 6271],
         744: [2832, 8233]
     }, j.f.consumes = (e, r) => {
         j.o(g, e) && g[e].forEach((e => {
             if (j.o(v, e)) return r.push(v[e]);
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json` & `tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9949596774193548%*

 * *Differences: {"'packages'": "{11: {'versionInfo': '8.5.16'}, 12: {'versionInfo': '8.5.16'}, 13: {'versionInfo': "*

 * *               "'8.5.16'}, 14: {'versionInfo': '8.5.16'}, 15: {'versionInfo': '8.5.16'}}"}*

```diff
@@ -66,39 +66,39 @@
             "name": "@loaders.gl/worker-utils",
             "versionInfo": "3.4.4"
         },
         {
             "extractedText": "Copyright (c) 2015 Uber Technologies, Inc.\n\nThis software includes parts of PhiloGL (https://github.com/philogb/philogl)\nunder MIT license. PhiloGL parts Copyright \u00a9 2013 Sencha Labs.\n\nThis software includes adaptations of postprocessing code from THREE.js (https://github.com/mrdoob/three.js/) under MIT license. Additional attribution given in specific source files. THREE.js parts Copyright \u00a9 2010-2018 three.js authors.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN\nTHE SOFTWARE.\n\n",
             "licenseId": "MIT",
             "name": "@luma.gl/constants",
-            "versionInfo": "8.5.20"
+            "versionInfo": "8.5.16"
         },
         {
             "extractedText": "Copyright (c) 2015 Uber Technologies, Inc.\n\nThis software includes parts of PhiloGL (https://github.com/philogb/philogl)\nunder MIT license. PhiloGL parts Copyright \u00a9 2013 Sencha Labs.\n\nThis software includes adaptations of postprocessing code from THREE.js (https://github.com/mrdoob/three.js/) under MIT license. Additional attribution given in specific source files. THREE.js parts Copyright \u00a9 2010-2018 three.js authors.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN\nTHE SOFTWARE.\n\n",
             "licenseId": "MIT",
             "name": "@luma.gl/engine",
-            "versionInfo": "8.5.20"
+            "versionInfo": "8.5.16"
         },
         {
             "extractedText": "Copyright (c) 2015 Uber Technologies, Inc.\n\nThis software includes parts of PhiloGL (https://github.com/philogb/philogl)\nunder MIT license. PhiloGL parts Copyright \u00a9 2013 Sencha Labs.\n\nThis software includes adaptations of postprocessing code from THREE.js (https://github.com/mrdoob/three.js/) under MIT license. Additional attribution given in specific source files. THREE.js parts Copyright \u00a9 2010-2018 three.js authors.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN\nTHE SOFTWARE.\n\n",
             "licenseId": "MIT",
             "name": "@luma.gl/gltools",
-            "versionInfo": "8.5.20"
+            "versionInfo": "8.5.16"
         },
         {
             "extractedText": "Copyright (c) 2015 Uber Technologies, Inc.\n\nThis software includes parts of PhiloGL (https://github.com/philogb/philogl)\nunder MIT license. PhiloGL parts Copyright \u00a9 2013 Sencha Labs.\n\nThis software includes adaptations of postprocessing code from THREE.js (https://github.com/mrdoob/three.js/) under MIT license. Additional attribution given in specific source files. THREE.js parts Copyright \u00a9 2010-2018 three.js authors.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN\nTHE SOFTWARE.\n\n",
             "licenseId": "MIT",
             "name": "@luma.gl/shadertools",
-            "versionInfo": "8.5.20"
+            "versionInfo": "8.5.16"
         },
         {
             "extractedText": "Copyright (c) 2015 Uber Technologies, Inc.\n\nThis software includes parts of PhiloGL (https://github.com/philogb/philogl)\nunder MIT license. PhiloGL parts Copyright \u00a9 2013 Sencha Labs.\n\nThis software includes adaptations of postprocessing code from THREE.js (https://github.com/mrdoob/three.js/) under MIT license. Additional attribution given in specific source files. THREE.js parts Copyright \u00a9 2010-2018 three.js authors.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN\nTHE SOFTWARE.\n\n",
             "licenseId": "MIT",
             "name": "@luma.gl/webgl",
-            "versionInfo": "8.5.20"
+            "versionInfo": "8.5.16"
         },
         {
             "extractedText": "BSD-2-Clause\nCopyright (c) 2016-2022 Mapbox, Inc.\n\nRedistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:\n\n1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.\n2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.\n\nTHIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS \u201cAS IS\u201d AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.\n",
             "licenseId": "BSD-2-Clause",
             "name": "@mapbox/tiny-sdf",
             "versionInfo": "2.0.6"
         },
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg/render.py` & `tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg/render.py`

 * *Files identical despite different names*

### Comparing `tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg.egg-info/PKG-INFO` & `tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tiledb-jupyter-bioimg
-Version: 0.1.1a2
+Version: 0.1.1a3
 Summary: A jupyterlab extension to visualize bioimages in TileDB format
 Home-page: https://github.com/TileDB-Inc/TileDB-Jupyter-BioImage-Viewer
 Author: TileDB
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a2/tiledb_jupyter_bioimg.egg-info/SOURCES.txt` & `tiledb_jupyter_bioimg-0.1.1a3/tiledb_jupyter_bioimg.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -21,20 +21,20 @@
 tiledb_jupyter_bioimg.egg-info/dependency_links.txt
 tiledb_jupyter_bioimg.egg-info/not-zip-safe
 tiledb_jupyter_bioimg.egg-info/requires.txt
 tiledb_jupyter_bioimg.egg-info/top_level.txt
 tiledb_jupyter_bioimg/labextension/package.json
 tiledb_jupyter_bioimg/labextension/static/08450fe724517d116eb4ec755231ced4eb5bf019b478cb080efd58ad83c5e211.svg
 tiledb_jupyter_bioimg/labextension/static/172.6267f3dd3063477e34ed.js
-tiledb_jupyter_bioimg/labextension/static/344.8db93920a8ca0f0600d9.js
-tiledb_jupyter_bioimg/labextension/static/344.8db93920a8ca0f0600d9.js.LICENSE.txt
+tiledb_jupyter_bioimg/labextension/static/344.8d6b91ad4356dae38b22.js
+tiledb_jupyter_bioimg/labextension/static/344.8d6b91ad4356dae38b22.js.LICENSE.txt
 tiledb_jupyter_bioimg/labextension/static/446.3bf34f45c93ace9c0f28.js
-tiledb_jupyter_bioimg/labextension/static/633.86ebe895050415abdfba.js
-tiledb_jupyter_bioimg/labextension/static/635.ce138c9764842046bf90.js
-tiledb_jupyter_bioimg/labextension/static/635.ce138c9764842046bf90.js.LICENSE.txt
+tiledb_jupyter_bioimg/labextension/static/633.770b26571c8b948a69e3.js
+tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js
+tiledb_jupyter_bioimg/labextension/static/635.024275f22a135fe53126.js.LICENSE.txt
 tiledb_jupyter_bioimg/labextension/static/713.44bebcfa12a45c30ff83.js
 tiledb_jupyter_bioimg/labextension/static/713.44bebcfa12a45c30ff83.js.LICENSE.txt
-tiledb_jupyter_bioimg/labextension/static/744.9655cb2c54e12e1c2654.js
+tiledb_jupyter_bioimg/labextension/static/744.3b4d2f36290dd421bc4f.js
 tiledb_jupyter_bioimg/labextension/static/747.433530952542f03ebc71.js
-tiledb_jupyter_bioimg/labextension/static/remoteEntry.f05f71ea95cf3364c4cb.js
+tiledb_jupyter_bioimg/labextension/static/remoteEntry.ad93eef0e33172dacb16.js
 tiledb_jupyter_bioimg/labextension/static/style.js
 tiledb_jupyter_bioimg/labextension/static/third-party-licenses.json
```

### Comparing `tiledb_jupyter_bioimg-0.1.1a2/tsconfig.json` & `tiledb_jupyter_bioimg-0.1.1a3/tsconfig.json`

 * *Files identical despite different names*

