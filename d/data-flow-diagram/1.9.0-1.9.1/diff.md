# Comparing `tmp/data-flow-diagram-1.9.0.tar.gz` & `tmp/data-flow-diagram-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-flow-diagram-1.9.0.tar", last modified: Thu Dec  8 15:34:26 2022, max compression
+gzip compressed data, was "data-flow-diagram-1.9.1.tar", last modified: Wed Mar 15 07:56:25 2023, max compression
```

## Comparing `data-flow-diagram-1.9.0.tar` & `data-flow-diagram-1.9.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 pascal    (1000) pascal    (1000)        0 2022-12-08 15:34:26.770662 data-flow-diagram-1.9.0/
--rw-rw-r--   0 pascal    (1000) pascal    (1000)     3997 2022-12-08 15:34:26.770662 data-flow-diagram-1.9.0/PKG-INFO
--rw-rw-r--   0 pascal    (1000) pascal    (1000)     3093 2022-11-24 16:50:31.000000 data-flow-diagram-1.9.0/README.md
--rw-rw-r--   0 pascal    (1000) pascal    (1000)      230 2022-10-21 13:04:27.000000 data-flow-diagram-1.9.0/pyproject.toml
--rw-rw-r--   0 pascal    (1000) pascal    (1000)       78 2022-12-08 15:34:26.770662 data-flow-diagram-1.9.0/setup.cfg
--rw-rw-r--   0 pascal    (1000) pascal    (1000)     2034 2022-12-08 15:33:51.000000 data-flow-diagram-1.9.0/setup.py
-drwxrwxr-x   0 pascal    (1000) pascal    (1000)        0 2022-12-08 15:34:26.770662 data-flow-diagram-1.9.0/src/
-drwxrwxr-x   0 pascal    (1000) pascal    (1000)        0 2022-12-08 15:34:26.770662 data-flow-diagram-1.9.0/src/data_flow_diagram/
--rw-rw-r--   0 pascal    (1000) pascal    (1000)     5837 2022-11-24 16:50:31.000000 data-flow-diagram-1.9.0/src/data_flow_diagram/__init__.py
--rw-rw-r--   0 pascal    (1000) pascal    (1000)       64 2022-11-24 16:50:31.000000 data-flow-diagram-1.9.0/src/data_flow_diagram/config.py
--rw-rw-r--   0 pascal    (1000) pascal    (1000)     2555 2022-11-24 16:50:31.000000 data-flow-diagram-1.9.0/src/data_flow_diagram/dependency_checker.py
--rw-rw-r--   0 pascal    (1000) pascal    (1000)    10092 2022-11-24 16:50:31.000000 data-flow-diagram-1.9.0/src/data_flow_diagram/dfd.py
--rw-rw-r--   0 pascal    (1000) pascal    (1000)     1193 2022-11-24 16:50:31.000000 data-flow-diagram-1.9.0/src/data_flow_diagram/dfd_dot_templates.py
--rw-rw-r--   0 pascal    (1000) pascal    (1000)     1022 2022-11-24 16:50:31.000000 data-flow-diagram-1.9.0/src/data_flow_diagram/dot.py
--rw-rw-r--   0 pascal    (1000) pascal    (1000)      148 2022-11-24 16:50:31.000000 data-flow-diagram-1.9.0/src/data_flow_diagram/error.py
--rw-rw-r--   0 pascal    (1000) pascal    (1000)     2221 2022-11-24 16:50:31.000000 data-flow-diagram-1.9.0/src/data_flow_diagram/markdown.py
--rw-rw-r--   0 pascal    (1000) pascal    (1000)     3104 2022-11-24 16:50:31.000000 data-flow-diagram-1.9.0/src/data_flow_diagram/model.py
--rw-rw-r--   0 pascal    (1000) pascal    (1000)    15332 2022-11-24 16:50:31.000000 data-flow-diagram-1.9.0/src/data_flow_diagram/parser.py
--rw-rw-r--   0 pascal    (1000) pascal    (1000)     2753 2022-12-08 15:31:33.000000 data-flow-diagram-1.9.0/src/data_flow_diagram/scanner.py
-drwxrwxr-x   0 pascal    (1000) pascal    (1000)        0 2022-12-08 15:34:26.770662 data-flow-diagram-1.9.0/src/data_flow_diagram.egg-info/
--rw-rw-r--   0 pascal    (1000) pascal    (1000)     3997 2022-12-08 15:34:26.000000 data-flow-diagram-1.9.0/src/data_flow_diagram.egg-info/PKG-INFO
--rw-rw-r--   0 pascal    (1000) pascal    (1000)      687 2022-12-08 15:34:26.000000 data-flow-diagram-1.9.0/src/data_flow_diagram.egg-info/SOURCES.txt
--rw-rw-r--   0 pascal    (1000) pascal    (1000)        1 2022-12-08 15:34:26.000000 data-flow-diagram-1.9.0/src/data_flow_diagram.egg-info/dependency_links.txt
--rw-rw-r--   0 pascal    (1000) pascal    (1000)       61 2022-12-08 15:34:26.000000 data-flow-diagram-1.9.0/src/data_flow_diagram.egg-info/entry_points.txt
--rw-rw-r--   0 pascal    (1000) pascal    (1000)       39 2022-12-08 15:34:26.000000 data-flow-diagram-1.9.0/src/data_flow_diagram.egg-info/requires.txt
--rw-rw-r--   0 pascal    (1000) pascal    (1000)       18 2022-12-08 15:34:26.000000 data-flow-diagram-1.9.0/src/data_flow_diagram.egg-info/top_level.txt
+drwxrwxr-x   0 pascal    (1000) pascal    (1000)        0 2023-03-15 07:56:25.336789 data-flow-diagram-1.9.1/
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)     4277 2023-03-15 07:56:25.336789 data-flow-diagram-1.9.1/PKG-INFO
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)     3353 2023-03-15 07:54:31.000000 data-flow-diagram-1.9.1/README.md
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)      230 2022-10-21 13:04:27.000000 data-flow-diagram-1.9.1/pyproject.toml
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)       78 2023-03-15 07:56:25.336789 data-flow-diagram-1.9.1/setup.cfg
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)     2034 2023-03-15 07:55:52.000000 data-flow-diagram-1.9.1/setup.py
+drwxrwxr-x   0 pascal    (1000) pascal    (1000)        0 2023-03-15 07:56:25.336789 data-flow-diagram-1.9.1/src/
+drwxrwxr-x   0 pascal    (1000) pascal    (1000)        0 2023-03-15 07:56:25.336789 data-flow-diagram-1.9.1/src/data_flow_diagram/
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)     5837 2022-11-24 16:50:31.000000 data-flow-diagram-1.9.1/src/data_flow_diagram/__init__.py
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)       64 2022-11-24 16:50:31.000000 data-flow-diagram-1.9.1/src/data_flow_diagram/config.py
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)     2555 2022-11-24 16:50:31.000000 data-flow-diagram-1.9.1/src/data_flow_diagram/dependency_checker.py
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)    10092 2022-11-24 16:50:31.000000 data-flow-diagram-1.9.1/src/data_flow_diagram/dfd.py
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)     1193 2022-11-24 16:50:31.000000 data-flow-diagram-1.9.1/src/data_flow_diagram/dfd_dot_templates.py
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)     1022 2022-11-24 16:50:31.000000 data-flow-diagram-1.9.1/src/data_flow_diagram/dot.py
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)      148 2022-11-24 16:50:31.000000 data-flow-diagram-1.9.1/src/data_flow_diagram/error.py
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)     2221 2022-11-24 16:50:31.000000 data-flow-diagram-1.9.1/src/data_flow_diagram/markdown.py
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)     3104 2022-11-24 16:50:31.000000 data-flow-diagram-1.9.1/src/data_flow_diagram/model.py
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)    15332 2022-11-24 16:50:31.000000 data-flow-diagram-1.9.1/src/data_flow_diagram/parser.py
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)     2753 2022-12-08 15:31:33.000000 data-flow-diagram-1.9.1/src/data_flow_diagram/scanner.py
+drwxrwxr-x   0 pascal    (1000) pascal    (1000)        0 2023-03-15 07:56:25.336789 data-flow-diagram-1.9.1/src/data_flow_diagram.egg-info/
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)     4277 2023-03-15 07:56:25.000000 data-flow-diagram-1.9.1/src/data_flow_diagram.egg-info/PKG-INFO
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)      687 2023-03-15 07:56:25.000000 data-flow-diagram-1.9.1/src/data_flow_diagram.egg-info/SOURCES.txt
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)        1 2023-03-15 07:56:25.000000 data-flow-diagram-1.9.1/src/data_flow_diagram.egg-info/dependency_links.txt
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)       62 2023-03-15 07:56:25.000000 data-flow-diagram-1.9.1/src/data_flow_diagram.egg-info/entry_points.txt
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)       39 2023-03-15 07:56:25.000000 data-flow-diagram-1.9.1/src/data_flow_diagram.egg-info/requires.txt
+-rw-rw-r--   0 pascal    (1000) pascal    (1000)       18 2023-03-15 07:56:25.000000 data-flow-diagram-1.9.1/src/data_flow_diagram.egg-info/top_level.txt
```

### Comparing `data-flow-diagram-1.9.0/PKG-INFO` & `data-flow-diagram-1.9.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: data-flow-diagram
-Version: 1.9.0
+Version: 1.9.1
 Summary: Commandline tool to generate data flow diagrams from text
 Home-page: https://github.com/pbauermeister/dfd
 Author: Pascal Bauermeister
 Author-email: pascal.bauermeister@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Bug Reports, https://github.com/pbauermeister/dfd/issues
 Project-URL: Source, https://github.com/pbauermeister/dfd
 Keywords: diagram-generator,development,tool
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Documentation
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10, <4
@@ -75,14 +76,25 @@
 
 ## Installing via pip3
 
 ```
 [sudo] pip3 install data-flow-diagram
 ```
 
+## Installation troubleshooting
+
+If you get an error at runtime like:
+```
+ModuleNotFoundError: No module named 'reportlab.graphics._renderPM'
+```
+you may have to reinstall reportlab:
+```
+[sudo] python3 -m pip install --upgrade --force-reinstall reportlab
+```
+
 ## Usage
 
 `data-flow-diagram -h` says:
 
 ```
 usage: data-flow-diagram [-h] [--output-file OUTPUT_FILE] [--markdown]
                          [--format FORMAT] [--percent-zoom PERCENT_ZOOM]
@@ -116,7 +128,9 @@
 See https://github.com/pbauermeister/dfd for information, syntax and
 examples.
 ```
 
 [src]: https://github.com/pbauermeister/dfd
 [pypi]: https://pypi.org/project/data-flow-diagram
 [doc]: https://github.com/pbauermeister/dfd/tree/master/doc/README.md
+
+
```

### Comparing `data-flow-diagram-1.9.0/README.md` & `data-flow-diagram-1.9.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -53,14 +53,25 @@
 
 ## Installing via pip3
 
 ```
 [sudo] pip3 install data-flow-diagram
 ```
 
+## Installation troubleshooting
+
+If you get an error at runtime like:
+```
+ModuleNotFoundError: No module named 'reportlab.graphics._renderPM'
+```
+you may have to reinstall reportlab:
+```
+[sudo] python3 -m pip install --upgrade --force-reinstall reportlab
+```
+
 ## Usage
 
 `data-flow-diagram -h` says:
 
 ```
 usage: data-flow-diagram [-h] [--output-file OUTPUT_FILE] [--markdown]
                          [--format FORMAT] [--percent-zoom PERCENT_ZOOM]
```

### Comparing `data-flow-diagram-1.9.0/setup.py` & `data-flow-diagram-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="data-flow-diagram",
-    version="1.9.0",
+    version="1.9.1",
     description="Commandline tool to generate data flow diagrams from text",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pbauermeister/dfd",
     author="Pascal Bauermeister",
     author_email="pascal.bauermeister@gmail.com",
     classifiers=[
```

### Comparing `data-flow-diagram-1.9.0/src/data_flow_diagram/__init__.py` & `data-flow-diagram-1.9.1/src/data_flow_diagram/__init__.py`

 * *Files identical despite different names*

### Comparing `data-flow-diagram-1.9.0/src/data_flow_diagram/dependency_checker.py` & `data-flow-diagram-1.9.1/src/data_flow_diagram/dependency_checker.py`

 * *Files identical despite different names*

### Comparing `data-flow-diagram-1.9.0/src/data_flow_diagram/dfd.py` & `data-flow-diagram-1.9.1/src/data_flow_diagram/dfd.py`

 * *Files identical despite different names*

### Comparing `data-flow-diagram-1.9.0/src/data_flow_diagram/dfd_dot_templates.py` & `data-flow-diagram-1.9.1/src/data_flow_diagram/dfd_dot_templates.py`

 * *Files identical despite different names*

### Comparing `data-flow-diagram-1.9.0/src/data_flow_diagram/dot.py` & `data-flow-diagram-1.9.1/src/data_flow_diagram/dot.py`

 * *Files identical despite different names*

### Comparing `data-flow-diagram-1.9.0/src/data_flow_diagram/markdown.py` & `data-flow-diagram-1.9.1/src/data_flow_diagram/markdown.py`

 * *Files identical despite different names*

### Comparing `data-flow-diagram-1.9.0/src/data_flow_diagram/model.py` & `data-flow-diagram-1.9.1/src/data_flow_diagram/model.py`

 * *Files identical despite different names*

### Comparing `data-flow-diagram-1.9.0/src/data_flow_diagram/parser.py` & `data-flow-diagram-1.9.1/src/data_flow_diagram/parser.py`

 * *Files identical despite different names*

### Comparing `data-flow-diagram-1.9.0/src/data_flow_diagram/scanner.py` & `data-flow-diagram-1.9.1/src/data_flow_diagram/scanner.py`

 * *Files identical despite different names*

### Comparing `data-flow-diagram-1.9.0/src/data_flow_diagram.egg-info/PKG-INFO` & `data-flow-diagram-1.9.1/src/data_flow_diagram.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: data-flow-diagram
-Version: 1.9.0
+Version: 1.9.1
 Summary: Commandline tool to generate data flow diagrams from text
 Home-page: https://github.com/pbauermeister/dfd
 Author: Pascal Bauermeister
 Author-email: pascal.bauermeister@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Bug Reports, https://github.com/pbauermeister/dfd/issues
 Project-URL: Source, https://github.com/pbauermeister/dfd
 Keywords: diagram-generator,development,tool
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Documentation
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10, <4
@@ -75,14 +76,25 @@
 
 ## Installing via pip3
 
 ```
 [sudo] pip3 install data-flow-diagram
 ```
 
+## Installation troubleshooting
+
+If you get an error at runtime like:
+```
+ModuleNotFoundError: No module named 'reportlab.graphics._renderPM'
+```
+you may have to reinstall reportlab:
+```
+[sudo] python3 -m pip install --upgrade --force-reinstall reportlab
+```
+
 ## Usage
 
 `data-flow-diagram -h` says:
 
 ```
 usage: data-flow-diagram [-h] [--output-file OUTPUT_FILE] [--markdown]
                          [--format FORMAT] [--percent-zoom PERCENT_ZOOM]
@@ -116,7 +128,9 @@
 See https://github.com/pbauermeister/dfd for information, syntax and
 examples.
 ```
 
 [src]: https://github.com/pbauermeister/dfd
 [pypi]: https://pypi.org/project/data-flow-diagram
 [doc]: https://github.com/pbauermeister/dfd/tree/master/doc/README.md
+
+
```

### Comparing `data-flow-diagram-1.9.0/src/data_flow_diagram.egg-info/SOURCES.txt` & `data-flow-diagram-1.9.1/src/data_flow_diagram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

