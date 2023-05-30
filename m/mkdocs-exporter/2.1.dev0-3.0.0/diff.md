# Comparing `tmp/mkdocs_exporter-2.1.dev0.tar.gz` & `tmp/mkdocs_exporter-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_exporter-2.1.dev0.tar", max compression
+gzip compressed data, was "mkdocs_exporter-3.0.0.tar", max compression
```

## Comparing `mkdocs_exporter-2.1.dev0.tar` & `mkdocs_exporter-3.0.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1071 2023-05-09 09:23:22.592488 mkdocs_exporter-2.1.dev0/LICENSE
--rw-r--r--   0        0        0     4007 2023-05-30 06:07:05.064243 mkdocs_exporter-2.1.dev0/README.md
--rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-2.1.dev0/mkdocs_exporter/__init__.py
--rw-r--r--   0        0        0     1973 2023-05-30 08:02:59.092627 mkdocs_exporter-2.1.dev0/mkdocs_exporter/browser.py
--rw-r--r--   0        0        0       96 2023-05-09 09:23:22.592488 mkdocs_exporter-2.1.dev0/mkdocs_exporter/logging.py
--rw-r--r--   0        0        0      543 2023-05-30 06:07:05.064243 mkdocs_exporter-2.1.dev0/mkdocs_exporter/page.py
--rw-r--r--   0        0        0     1864 2023-05-30 06:13:17.034229 mkdocs_exporter-2.1.dev0/mkdocs_exporter/plugin.py
--rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-2.1.dev0/mkdocs_exporter/plugins/__init__.py
--rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-2.1.dev0/mkdocs_exporter/plugins/extras/__init__.py
--rw-r--r--   0        0        0      867 2023-05-30 06:10:52.764231 mkdocs_exporter-2.1.dev0/mkdocs_exporter/plugins/extras/config.py
--rw-r--r--   0        0        0     1121 2023-05-30 06:11:08.624231 mkdocs_exporter-2.1.dev0/mkdocs_exporter/plugins/extras/plugin.py
--rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-2.1.dev0/mkdocs_exporter/plugins/pdf/__init__.py
--rw-r--r--   0        0        0      526 2023-05-22 10:55:25.061256 mkdocs_exporter-2.1.dev0/mkdocs_exporter/plugins/pdf/button.py
--rw-r--r--   0        0        0     1040 2023-05-30 06:07:05.064243 mkdocs_exporter-2.1.dev0/mkdocs_exporter/plugins/pdf/config.py
--rw-r--r--   0        0        0     4852 2023-05-30 08:05:13.700839 mkdocs_exporter-2.1.dev0/mkdocs_exporter/plugins/pdf/plugin.py
--rw-r--r--   0        0        0     2215 2023-05-30 06:07:05.064243 mkdocs_exporter-2.1.dev0/mkdocs_exporter/plugins/pdf/renderer.py
--rw-r--r--   0        0        0     4115 2023-05-30 06:30:33.584215 mkdocs_exporter-2.1.dev0/mkdocs_exporter/preprocessor.py
--rw-r--r--   0        0        0      241 2023-05-09 09:23:22.592488 mkdocs_exporter-2.1.dev0/mkdocs_exporter/renderer.py
--rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-2.1.dev0/mkdocs_exporter/resources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 06:07:05.064243 mkdocs_exporter-2.1.dev0/mkdocs_exporter/resources/css/__init__.py
--rw-r--r--   0        0        0       93 2023-05-30 06:07:05.064243 mkdocs_exporter-2.1.dev0/mkdocs_exporter/resources/css/readthedocs.css
--rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-2.1.dev0/mkdocs_exporter/resources/js/__init__.py
--rw-r--r--   0        0        0   504034 2023-05-30 06:07:05.074243 mkdocs_exporter-2.1.dev0/mkdocs_exporter/resources/js/pagedjs.min.js
--rw-r--r--   0        0        0      599 2023-05-30 06:07:05.074243 mkdocs_exporter-2.1.dev0/mkdocs_exporter/theme.py
--rw-r--r--   0        0        0        0 2023-05-30 06:07:05.074243 mkdocs_exporter-2.1.dev0/mkdocs_exporter/themes/__init__.py
--rw-r--r--   0        0        0      650 2023-05-30 06:07:05.074243 mkdocs_exporter-2.1.dev0/mkdocs_exporter/themes/factory.py
--rw-r--r--   0        0        0        0 2023-05-30 06:07:05.074243 mkdocs_exporter-2.1.dev0/mkdocs_exporter/themes/material/__init__.py
--rw-r--r--   0        0        0      681 2023-05-30 06:07:05.074243 mkdocs_exporter-2.1.dev0/mkdocs_exporter/themes/material/icons.py
--rw-r--r--   0        0        0     1317 2023-05-30 06:07:05.074243 mkdocs_exporter-2.1.dev0/mkdocs_exporter/themes/material/theme.py
--rw-r--r--   0        0        0        0 2023-05-30 06:07:05.074243 mkdocs_exporter-2.1.dev0/mkdocs_exporter/themes/readthedocs/__init__.py
--rw-r--r--   0        0        0     1221 2023-05-30 06:07:05.074243 mkdocs_exporter-2.1.dev0/mkdocs_exporter/themes/readthedocs/theme.py
--rw-r--r--   0        0        0     1596 2023-05-30 08:07:01.747597 mkdocs_exporter-2.1.dev0/pyproject.toml
--rw-r--r--   0        0        0     5370 1970-01-01 00:00:00.000000 mkdocs_exporter-2.1.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-09 09:23:22.592488 mkdocs_exporter-3.0.0/LICENSE
+-rw-r--r--   0        0        0     4007 2023-05-30 06:07:05.064243 mkdocs_exporter-3.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-3.0.0/mkdocs_exporter/__init__.py
+-rw-r--r--   0        0        0     1973 2023-05-30 08:02:59.092627 mkdocs_exporter-3.0.0/mkdocs_exporter/browser.py
+-rw-r--r--   0        0        0       96 2023-05-09 09:23:22.592488 mkdocs_exporter-3.0.0/mkdocs_exporter/logging.py
+-rw-r--r--   0        0        0      543 2023-05-30 06:07:05.064243 mkdocs_exporter-3.0.0/mkdocs_exporter/page.py
+-rw-r--r--   0        0        0     1864 2023-05-30 06:13:17.034229 mkdocs_exporter-3.0.0/mkdocs_exporter/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-3.0.0/mkdocs_exporter/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-3.0.0/mkdocs_exporter/plugins/extras/__init__.py
+-rw-r--r--   0        0        0      867 2023-05-30 06:10:52.764231 mkdocs_exporter-3.0.0/mkdocs_exporter/plugins/extras/config.py
+-rw-r--r--   0        0        0     1121 2023-05-30 06:11:08.624231 mkdocs_exporter-3.0.0/mkdocs_exporter/plugins/extras/plugin.py
+-rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-3.0.0/mkdocs_exporter/plugins/pdf/__init__.py
+-rw-r--r--   0        0        0      526 2023-05-22 10:55:25.061256 mkdocs_exporter-3.0.0/mkdocs_exporter/plugins/pdf/button.py
+-rw-r--r--   0        0        0     1040 2023-05-30 06:07:05.064243 mkdocs_exporter-3.0.0/mkdocs_exporter/plugins/pdf/config.py
+-rw-r--r--   0        0        0     4852 2023-05-30 08:05:13.700839 mkdocs_exporter-3.0.0/mkdocs_exporter/plugins/pdf/plugin.py
+-rw-r--r--   0        0        0     2215 2023-05-30 06:07:05.064243 mkdocs_exporter-3.0.0/mkdocs_exporter/plugins/pdf/renderer.py
+-rw-r--r--   0        0        0     4115 2023-05-30 06:30:33.584215 mkdocs_exporter-3.0.0/mkdocs_exporter/preprocessor.py
+-rw-r--r--   0        0        0      241 2023-05-09 09:23:22.592488 mkdocs_exporter-3.0.0/mkdocs_exporter/renderer.py
+-rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-3.0.0/mkdocs_exporter/resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:07:05.064243 mkdocs_exporter-3.0.0/mkdocs_exporter/resources/css/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-30 06:07:05.064243 mkdocs_exporter-3.0.0/mkdocs_exporter/resources/css/readthedocs.css
+-rw-r--r--   0        0        0        0 2023-05-09 09:23:22.592488 mkdocs_exporter-3.0.0/mkdocs_exporter/resources/js/__init__.py
+-rw-r--r--   0        0        0   504034 2023-05-30 06:07:05.074243 mkdocs_exporter-3.0.0/mkdocs_exporter/resources/js/pagedjs.min.js
+-rw-r--r--   0        0        0      599 2023-05-30 06:07:05.074243 mkdocs_exporter-3.0.0/mkdocs_exporter/theme.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:07:05.074243 mkdocs_exporter-3.0.0/mkdocs_exporter/themes/__init__.py
+-rw-r--r--   0        0        0      650 2023-05-30 06:07:05.074243 mkdocs_exporter-3.0.0/mkdocs_exporter/themes/factory.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:07:05.074243 mkdocs_exporter-3.0.0/mkdocs_exporter/themes/material/__init__.py
+-rw-r--r--   0        0        0      681 2023-05-30 06:07:05.074243 mkdocs_exporter-3.0.0/mkdocs_exporter/themes/material/icons.py
+-rw-r--r--   0        0        0     1317 2023-05-30 06:07:05.074243 mkdocs_exporter-3.0.0/mkdocs_exporter/themes/material/theme.py
+-rw-r--r--   0        0        0        0 2023-05-30 06:07:05.074243 mkdocs_exporter-3.0.0/mkdocs_exporter/themes/readthedocs/__init__.py
+-rw-r--r--   0        0        0     1221 2023-05-30 06:07:05.074243 mkdocs_exporter-3.0.0/mkdocs_exporter/themes/readthedocs/theme.py
+-rw-r--r--   0        0        0     1593 2023-05-30 08:17:46.707916 mkdocs_exporter-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5367 1970-01-01 00:00:00.000000 mkdocs_exporter-3.0.0/PKG-INFO
```

### Comparing `mkdocs_exporter-2.1.dev0/LICENSE` & `mkdocs_exporter-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-2.1.dev0/README.md` & `mkdocs_exporter-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-2.1.dev0/mkdocs_exporter/browser.py` & `mkdocs_exporter-3.0.0/mkdocs_exporter/browser.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-2.1.dev0/mkdocs_exporter/page.py` & `mkdocs_exporter-3.0.0/mkdocs_exporter/page.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-2.1.dev0/mkdocs_exporter/plugin.py` & `mkdocs_exporter-3.0.0/mkdocs_exporter/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-2.1.dev0/mkdocs_exporter/plugins/extras/config.py` & `mkdocs_exporter-3.0.0/mkdocs_exporter/plugins/extras/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-2.1.dev0/mkdocs_exporter/plugins/extras/plugin.py` & `mkdocs_exporter-3.0.0/mkdocs_exporter/plugins/extras/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-2.1.dev0/mkdocs_exporter/plugins/pdf/button.py` & `mkdocs_exporter-3.0.0/mkdocs_exporter/plugins/pdf/button.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-2.1.dev0/mkdocs_exporter/plugins/pdf/config.py` & `mkdocs_exporter-3.0.0/mkdocs_exporter/plugins/pdf/config.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-2.1.dev0/mkdocs_exporter/plugins/pdf/plugin.py` & `mkdocs_exporter-3.0.0/mkdocs_exporter/plugins/pdf/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-2.1.dev0/mkdocs_exporter/plugins/pdf/renderer.py` & `mkdocs_exporter-3.0.0/mkdocs_exporter/plugins/pdf/renderer.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-2.1.dev0/mkdocs_exporter/preprocessor.py` & `mkdocs_exporter-3.0.0/mkdocs_exporter/preprocessor.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-2.1.dev0/mkdocs_exporter/resources/js/pagedjs.min.js` & `mkdocs_exporter-3.0.0/mkdocs_exporter/resources/js/pagedjs.min.js`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-2.1.dev0/mkdocs_exporter/theme.py` & `mkdocs_exporter-3.0.0/mkdocs_exporter/theme.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-2.1.dev0/mkdocs_exporter/themes/factory.py` & `mkdocs_exporter-3.0.0/mkdocs_exporter/themes/factory.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-2.1.dev0/mkdocs_exporter/themes/material/icons.py` & `mkdocs_exporter-3.0.0/mkdocs_exporter/themes/material/icons.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-2.1.dev0/mkdocs_exporter/themes/material/theme.py` & `mkdocs_exporter-3.0.0/mkdocs_exporter/themes/material/theme.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-2.1.dev0/mkdocs_exporter/themes/readthedocs/theme.py` & `mkdocs_exporter-3.0.0/mkdocs_exporter/themes/readthedocs/theme.py`

 * *Files identical despite different names*

### Comparing `mkdocs_exporter-2.1.dev0/pyproject.toml` & `mkdocs_exporter-3.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "mkdocs-exporter"
-version = "2.1.dev0"
+version = "3.0.0"
 repository = "https://github.com/adrienbrignon/mkdocs-exporter"
 keywords = ["mkdocs", "pdf", "exporter"]
 description = "A highly-configurable plugin for MkDocs that exports your pages to PDF files."
 authors = ["Adrien Brignon <adrien@brignon.dev>"]
 readme = "README.md"
 classifiers = [
   "License :: OSI Approved :: MIT License",
```

### Comparing `mkdocs_exporter-2.1.dev0/PKG-INFO` & `mkdocs_exporter-3.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-exporter
-Version: 2.1.dev0
+Version: 3.0.0
 Summary: A highly-configurable plugin for MkDocs that exports your pages to PDF files.
 Home-page: https://github.com/adrienbrignon/mkdocs-exporter
 Keywords: mkdocs,pdf,exporter
 Author: Adrien Brignon
 Author-email: adrien@brignon.dev
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: mkdocs-exporter Version: 2.1.dev0 Summary: A
-highly-configurable plugin for MkDocs that exports your pages to PDF files.
-Home-page: https://github.com/adrienbrignon/mkdocs-exporter Keywords:
-mkdocs,pdf,exporter Author: Adrien Brignon Author-email: adrien@brignon.dev
-Requires-Python: >=3.7 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3 Classifier: Topic :: Documentation Classifier: Topic :: Software
-Development :: Documentation Classifier: Topic :: Text Processing :: Markup ::
-HTML Requires-Dist: beautifulsoup4 (>=4.12.2) Requires-Dist: importlib-metadata
-(<5.0) Requires-Dist: importlib-resources (>=5.0) Requires-Dist: libsass
-(>=0.22.0) Requires-Dist: lxml (>=4.9) Requires-Dist: mkdocs (>=1.4) Requires-
-Dist: playwright (>=1.33) Project-URL: Bug Tracker, https://github.com/
-adrienbrignon/mkdocs-exporter/issues Project-URL: Repository, https://
-github.com/adrienbrignon/mkdocs-exporter Description-Content-Type: text/
-markdown # MkDocs Exporter
+Metadata-Version: 2.1 Name: mkdocs-exporter Version: 3.0.0 Summary: A highly-
+configurable plugin for MkDocs that exports your pages to PDF files. Home-page:
+https://github.com/adrienbrignon/mkdocs-exporter Keywords: mkdocs,pdf,exporter
+Author: Adrien Brignon Author-email: adrien@brignon.dev Requires-Python: >=3.7
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.7 Classifier: Programming Language ::
+Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Classifier: Programming Language :: Python :: 3 Classifier:
+Topic :: Documentation Classifier: Topic :: Software Development ::
+Documentation Classifier: Topic :: Text Processing :: Markup :: HTML Requires-
+Dist: beautifulsoup4 (>=4.12.2) Requires-Dist: importlib-metadata (<5.0)
+Requires-Dist: importlib-resources (>=5.0) Requires-Dist: libsass (>=0.22.0)
+Requires-Dist: lxml (>=4.9) Requires-Dist: mkdocs (>=1.4) Requires-Dist:
+playwright (>=1.33) Project-URL: Bug Tracker, https://github.com/adrienbrignon/
+mkdocs-exporter/issues Project-URL: Repository, https://github.com/
+adrienbrignon/mkdocs-exporter Description-Content-Type: text/markdown # MkDocs
+Exporter
 [https://img.shields.io/pypi/v/mkdocs-exporter?color=blue] [https://
 img.shields.io/pypi/pyversions/mkdocs-exporter?color=blue] [https://
 img.shields.io/pypi/dm/mkdocs-exporter?color=cactus] [https://img.shields.io/
 github/license/adrienbrignon/mkdocs-exporter?color=white]
 
 A highly-configurable plugin for [*MkDocs*](https://github.com/mkdocs/mkdocs)
 that exports your pages to PDF files. - [Documentation](https://
```

