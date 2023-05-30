# Comparing `tmp/peakrdl_markdown-0.1.4.tar.gz` & `tmp/peakrdl_markdown-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peakrdl_markdown-0.1.4.tar", max compression
+gzip compressed data, was "peakrdl_markdown-0.1.5.tar", max compression
```

## Comparing `peakrdl_markdown-0.1.4.tar` & `peakrdl_markdown-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-03-14 12:00:46.388118 peakrdl_markdown-0.1.4/LICENSE
--rw-r--r--   0        0        0     1249 2023-03-14 12:00:46.388118 peakrdl_markdown-0.1.4/README.md
--rw-r--r--   0        0        0     1616 2023-03-14 12:00:46.388118 peakrdl_markdown-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      138 2023-03-14 12:00:46.388118 peakrdl_markdown-0.1.4/src/peakrdl_markdown/__init__.py
--rw-r--r--   0        0        0     1481 2023-03-14 12:00:46.388118 peakrdl_markdown-0.1.4/src/peakrdl_markdown/__peakrdl__.py
--rw-r--r--   0        0        0    10500 2023-03-14 12:00:46.388118 peakrdl_markdown-0.1.4/src/peakrdl_markdown/exporter.py
--rw-r--r--   0        0        0     2552 1970-01-01 00:00:00.000000 peakrdl_markdown-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-30 06:04:52.384043 peakrdl_markdown-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1249 2023-05-30 06:04:52.384043 peakrdl_markdown-0.1.5/README.md
+-rw-r--r--   0        0        0     1610 2023-05-30 06:04:52.388043 peakrdl_markdown-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      138 2023-05-30 06:04:52.388043 peakrdl_markdown-0.1.5/src/peakrdl_markdown/__init__.py
+-rw-r--r--   0        0        0     1481 2023-05-30 06:04:52.388043 peakrdl_markdown-0.1.5/src/peakrdl_markdown/__peakrdl__.py
+-rw-r--r--   0        0        0    10500 2023-05-30 06:04:52.388043 peakrdl_markdown-0.1.5/src/peakrdl_markdown/exporter.py
+-rw-r--r--   0        0        0     2546 1970-01-01 00:00:00.000000 peakrdl_markdown-0.1.5/PKG-INFO
```

### Comparing `peakrdl_markdown-0.1.4/LICENSE` & `peakrdl_markdown-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `peakrdl_markdown-0.1.4/README.md` & `peakrdl_markdown-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `peakrdl_markdown-0.1.4/pyproject.toml` & `peakrdl_markdown-0.1.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "peakrdl_markdown"
-version = "0.1.4"
+version = "0.1.5"
 description = "Export Markdown description from the systemrdl-compiler register model"
-authors = ["Marek Pikuła <marek.pikula@embevity.com>"]
-maintainers = ["Marek Pikuła <marek.pikula@embevity.com>"]
+authors = ["Marek Pikuła <marek@serenitycode.dev>"]
+maintainers = ["Marek Pikuła <marek@serenitycode.dev>"]
 license = "GPL-3.0-only"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)",
 ]
```

### Comparing `peakrdl_markdown-0.1.4/src/peakrdl_markdown/__peakrdl__.py` & `peakrdl_markdown-0.1.5/src/peakrdl_markdown/__peakrdl__.py`

 * *Files identical despite different names*

### Comparing `peakrdl_markdown-0.1.4/src/peakrdl_markdown/exporter.py` & `peakrdl_markdown-0.1.5/src/peakrdl_markdown/exporter.py`

 * *Files identical despite different names*

### Comparing `peakrdl_markdown-0.1.4/PKG-INFO` & `peakrdl_markdown-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: peakrdl-markdown
-Version: 0.1.4
+Version: 0.1.5
 Summary: Export Markdown description from the systemrdl-compiler register model
 Home-page: https://github.com/MarekPikula/PeakRDL-Markdown
 License: GPL-3.0-only
 Author: Marek Pikuła
-Author-email: marek.pikula@embevity.com
+Author-email: marek@serenitycode.dev
 Maintainer: Marek Pikuła
-Maintainer-email: marek.pikula@embevity.com
+Maintainer-email: marek@serenitycode.dev
 Requires-Python: >=3.7.0,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

