# Comparing `tmp/toolplot-0.3.3.tar.gz` & `tmp/toolplot-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolplot-0.3.3.tar", last modified: Tue May  9 04:44:52 2023, max compression
+gzip compressed data, was "toolplot-0.3.4.tar", last modified: Tue May 30 01:13:14 2023, max compression
```

## Comparing `toolplot-0.3.3.tar` & `toolplot-0.3.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0       58 2023-03-11 02:30:55.209013 toolplot-0.3.3/.gitignore
--rw-r--r--   0        0        0     1083 2023-03-11 02:30:55.209139 toolplot-0.3.3/LICENSE
--rw-r--r--   0        0        0      229 2023-03-11 02:30:55.209248 toolplot-0.3.3/README.md
--rw-r--r--   0        0        0      370 2023-05-09 04:43:43.941461 toolplot-0.3.3/pyproject.toml
--rw-r--r--   0        0        0      215 2023-05-09 04:44:13.279731 toolplot-0.3.3/toolplot/__init__.py
--rw-r--r--   0        0        0     5176 2023-03-11 02:30:55.209682 toolplot-0.3.3/toolplot/plot_create.py
--rw-r--r--   0        0        0      140 2023-03-11 02:30:55.209793 toolplot-0.3.3/toolplot/plot_fonts.py
--rw-r--r--   0        0        0     1770 2023-03-11 02:30:55.209925 toolplot-0.3.3/toolplot/plot_save.py
--rw-r--r--   0        0        0      996 2023-03-11 02:30:55.210048 toolplot-0.3.3/toolplot/plot_setup.py
--rw-r--r--   0        0        0     3364 2023-04-25 21:12:12.432572 toolplot-0.3.3/toolplot/plot_ticks.py
--rw-r--r--   0        0        0       88 2023-03-11 02:33:48.174763 toolplot-0.3.3/toolplot/special_plots/__init__.py
--rw-r--r--   0        0        0      748 2023-03-11 02:30:55.210424 toolplot-0.3.3/toolplot/special_plots/bar_plots.py
--rw-r--r--   0        0        0     1279 2023-03-11 02:30:55.210531 toolplot-0.3.3/toolplot/special_plots/candlestick_plots.py
--rw-r--r--   0        0        0      618 2023-03-15 07:40:12.774167 toolplot-0.3.3/toolplot/special_plots/log_histograms.py
--rw-r--r--   0        0        0      568 1970-01-01 00:00:00.000000 toolplot-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0       58 2023-03-11 02:30:55.209013 toolplot-0.3.4/.gitignore
+-rw-r--r--   0        0        0     1083 2023-03-11 02:30:55.209139 toolplot-0.3.4/LICENSE
+-rw-r--r--   0        0        0      229 2023-03-11 02:30:55.209248 toolplot-0.3.4/README.md
+-rw-r--r--   0        0        0      370 2023-05-09 04:43:43.941461 toolplot-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0      215 2023-05-30 01:12:36.147707 toolplot-0.3.4/toolplot/__init__.py
+-rw-r--r--   0        0        0     5176 2023-03-11 02:30:55.209682 toolplot-0.3.4/toolplot/plot_create.py
+-rw-r--r--   0        0        0      140 2023-03-11 02:30:55.209793 toolplot-0.3.4/toolplot/plot_fonts.py
+-rw-r--r--   0        0        0     1770 2023-03-11 02:30:55.209925 toolplot-0.3.4/toolplot/plot_save.py
+-rw-r--r--   0        0        0     1040 2023-05-18 23:53:32.228133 toolplot-0.3.4/toolplot/plot_setup.py
+-rw-r--r--   0        0        0     3364 2023-04-25 21:12:12.432572 toolplot-0.3.4/toolplot/plot_ticks.py
+-rw-r--r--   0        0        0        0 2023-05-10 17:08:07.737985 toolplot-0.3.4/toolplot/py.typed
+-rw-r--r--   0        0        0       88 2023-03-11 02:33:48.174763 toolplot-0.3.4/toolplot/special_plots/__init__.py
+-rw-r--r--   0        0        0      748 2023-03-11 02:30:55.210424 toolplot-0.3.4/toolplot/special_plots/bar_plots.py
+-rw-r--r--   0        0        0     1279 2023-03-11 02:30:55.210531 toolplot-0.3.4/toolplot/special_plots/candlestick_plots.py
+-rw-r--r--   0        0        0      618 2023-03-15 07:40:12.774167 toolplot-0.3.4/toolplot/special_plots/log_histograms.py
+-rw-r--r--   0        0        0      568 1970-01-01 00:00:00.000000 toolplot-0.3.4/PKG-INFO
```

### Comparing `toolplot-0.3.3/LICENSE` & `toolplot-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `toolplot-0.3.3/toolplot/plot_create.py` & `toolplot-0.3.4/toolplot/plot_create.py`

 * *Files identical despite different names*

### Comparing `toolplot-0.3.3/toolplot/plot_save.py` & `toolplot-0.3.4/toolplot/plot_save.py`

 * *Files identical despite different names*

### Comparing `toolplot-0.3.3/toolplot/plot_setup.py` & `toolplot-0.3.4/toolplot/plot_setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from __future__ import annotations
 
-def setup_plot_formatting():
+
+def setup_plot_formatting() -> None:
     """set up matplotlib plot formatting"""
 
     # TODO: load from config
 
     # adapted from https://stackoverflow.com/a/39566040
 
     import matplotlib.pyplot as plt
```

### Comparing `toolplot-0.3.3/toolplot/plot_ticks.py` & `toolplot-0.3.4/toolplot/plot_ticks.py`

 * *Files identical despite different names*

### Comparing `toolplot-0.3.3/toolplot/special_plots/bar_plots.py` & `toolplot-0.3.4/toolplot/special_plots/bar_plots.py`

 * *Files identical despite different names*

### Comparing `toolplot-0.3.3/toolplot/special_plots/candlestick_plots.py` & `toolplot-0.3.4/toolplot/special_plots/candlestick_plots.py`

 * *Files identical despite different names*

### Comparing `toolplot-0.3.3/toolplot/special_plots/log_histograms.py` & `toolplot-0.3.4/toolplot/special_plots/log_histograms.py`

 * *Files identical despite different names*

### Comparing `toolplot-0.3.3/PKG-INFO` & `toolplot-0.3.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolplot
-Version: 0.3.3
+Version: 0.3.4
 Summary: toolplot is a alternative API to plotting backends
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: tooltime>=0.2.10
 Requires-Dist: toolstr>=0.9.3
 Requires-Dist: typing-extensions>=4.0.0
 Requires-Dist: matplotlib>=3.1
```

