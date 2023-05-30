# Comparing `tmp/deephaven-plugin-plotly-express-0.0.4.tar.gz` & `tmp/deephaven-plugin-plotly-express-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deephaven-plugin-plotly-express-0.0.4.tar", last modified: Fri May 26 17:07:41 2023, max compression
+gzip compressed data, was "deephaven-plugin-plotly-express-0.0.5.tar", last modified: Tue May 30 19:44:06 2023, max compression
```

## Comparing `deephaven-plugin-plotly-express-0.0.4.tar` & `deephaven-plugin-plotly-express-0.0.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:07:41.056547 deephaven-plugin-plotly-express-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-26 17:07:41.056547 deephaven-plugin-plotly-express-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-26 17:07:41.060548 deephaven-plugin-plotly-express-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:07:41.048544 deephaven-plugin-plotly-express-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:07:41.048544 deephaven-plugin-plotly-express-0.0.4/src/deephaven/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:07:41.048544 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:07:41.052545 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:07:41.052545 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/data_mapping/
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/data_mapping/DataMapping.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/data_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/data_mapping/data_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/data_mapping/data_mapping_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/data_mapping/json_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:07:41.052545 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/deephaven_figure/
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/deephaven_figure/DeephavenFigure.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/deephaven_figure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/deephaven_figure/custom_draw.py
--rw-r--r--   0 runner    (1001) docker     (123)    37445 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/deephaven_figure/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:07:41.056547 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27598 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/_private_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/area.py
--rw-r--r--   0 runner    (1001) docker     (123)    15408 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/bar.py
--rw-r--r--   0 runner    (1001) docker     (123)    25225 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/financial.py
--rw-r--r--   0 runner    (1001) docker     (123)    14004 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/hierarchial.py
--rw-r--r--   0 runner    (1001) docker     (123)    21032 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/pie.py
--rw-r--r--   0 runner    (1001) docker     (123)    20781 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/subplots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:07:41.056547 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/preprocess/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/preprocess/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:07:41.056547 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/shared/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-26 17:07:29.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/shared/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:07:41.056547 deephaven-plugin-plotly-express-0.0.4/src/deephaven_plugin_plotly_express.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-26 17:07:41.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven_plugin_plotly_express.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-26 17:07:41.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven_plugin_plotly_express.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 17:07:41.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven_plugin_plotly_express.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-26 17:07:41.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven_plugin_plotly_express.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-26 17:07:41.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven_plugin_plotly_express.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 17:07:41.000000 deephaven-plugin-plotly-express-0.0.4/src/deephaven_plugin_plotly_express.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:44:06.791420 deephaven-plugin-plotly-express-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-30 19:43:56.000000 deephaven-plugin-plotly-express-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-30 19:44:06.791420 deephaven-plugin-plotly-express-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-30 19:43:56.000000 deephaven-plugin-plotly-express-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-30 19:43:56.000000 deephaven-plugin-plotly-express-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-30 19:44:06.791420 deephaven-plugin-plotly-express-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:44:06.787420 deephaven-plugin-plotly-express-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:44:06.783420 deephaven-plugin-plotly-express-0.0.5/src/deephaven/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:44:06.783420 deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:44:06.787420 deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-30 19:43:56.000000 deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:44:06.787420 deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/data_mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-30 19:43:56.000000 deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/data_mapping/DataMapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-30 19:43:56.000000 deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/data_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-05-30 19:43:56.000000 deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/data_mapping/data_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-30 19:43:56.000000 deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/data_mapping/data_mapping_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-30 19:43:56.000000 deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/data_mapping/json_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:44:06.787420 deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/deephaven_figure/
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-05-30 19:43:56.000000 deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/deephaven_figure/DeephavenFigure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-30 19:43:56.000000 deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/deephaven_figure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-05-30 19:43:56.000000 deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/deephaven_figure/custom_draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37645 2023-05-30 19:43:56.000000 deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/deephaven_figure/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:44:06.791420 deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-30 19:43:56.000000 deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27634 2023-05-30 19:43:56.000000 deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/plots/_private_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6879 2023-05-30 19:43:56.000000 deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/plots/area.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-05-30 19:43:56.000000 deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/plots/bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25261 2023-05-30 19:43:56.000000 deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/plots/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-05-30 19:43:56.000000 deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/plots/financial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14040 2023-05-30 19:43:56.000000 deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/plots/hierarchial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21068 2023-05-30 19:43:56.000000 deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/plots/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-05-30 19:43:56.000000 deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/plots/pie.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20817 2023-05-30 19:43:56.000000 deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/plots/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-05-30 19:43:56.000000 deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/plots/subplots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:44:06.791420 deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-30 19:43:56.000000 deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13007 2023-05-30 19:43:56.000000 deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/preprocess/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:44:06.791420 deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-30 19:43:56.000000 deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-30 19:43:56.000000 deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/shared/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:44:06.791420 deephaven-plugin-plotly-express-0.0.5/src/deephaven_plugin_plotly_express.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-30 19:44:06.000000 deephaven-plugin-plotly-express-0.0.5/src/deephaven_plugin_plotly_express.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-30 19:44:06.000000 deephaven-plugin-plotly-express-0.0.5/src/deephaven_plugin_plotly_express.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 19:44:06.000000 deephaven-plugin-plotly-express-0.0.5/src/deephaven_plugin_plotly_express.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-30 19:44:06.000000 deephaven-plugin-plotly-express-0.0.5/src/deephaven_plugin_plotly_express.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-30 19:44:06.000000 deephaven-plugin-plotly-express-0.0.5/src/deephaven_plugin_plotly_express.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-30 19:44:06.000000 deephaven-plugin-plotly-express-0.0.5/src/deephaven_plugin_plotly_express.egg-info/top_level.txt
```

### Comparing `deephaven-plugin-plotly-express-0.0.4/LICENSE` & `deephaven-plugin-plotly-express-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.0.4/PKG-INFO` & `deephaven-plugin-plotly-express-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deephaven-plugin-plotly-express
-Version: 0.0.4
+Version: 0.0.5
 Summary: Deephaven Chart Plugin
 Home-page: https://github.com/deephaven/deephaven-plugin-plotly-express
 Author: Devin Smith, Vlad Babich, Joe Numainville
 Author-email: josephnumainville@deephaven.io
 Project-URL: Source Code, https://github.com/deephaven/deephaven-plugin-plotly-express
 Project-URL: Bug Tracker, https://github.com/deephaven/deephaven-plugin-plotly-express/issues
 Keywords: deephaven,plugin,graph
```

### Comparing `deephaven-plugin-plotly-express-0.0.4/README.md` & `deephaven-plugin-plotly-express-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.0.4/setup.cfg` & `deephaven-plugin-plotly-express-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/__init__.py` & `deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .deephaven_figure import DeephavenFigure, export_figure
 
 from .plots import area, bar, frequency_bar, timeline, histogram, _ecdf, box, \
     violin, strip, ohlc, candlestick, treemap, sunburst, icicle, funnel, \
     funnel_area, line, line_polar, line_ternary, line_3d, scatter, scatter_3d, \
     scatter_polar, scatter_ternary, pie, layer, make_subplots
 
-__version__ = "0.0.4"
+__version__ = "0.0.5"
 
 NAME = "deephaven.plot.express.DeephavenFigure"
 
 
 class DeephavenFigureType(ObjectType):
     """
     DeephavenFigureType for plugin registration
```

### Comparing `deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/data_mapping/DataMapping.py` & `deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/data_mapping/DataMapping.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/data_mapping/data_mapping.py` & `deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/data_mapping/data_mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from copy import deepcopy
 from itertools import cycle, product, zip_longest
 from collections.abc import Generator, Iterable
 
 from deephaven.table import Table
 
 from .DataMapping import DataMapping
```

### Comparing `deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/data_mapping/data_mapping_constants.py` & `deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/data_mapping/data_mapping_constants.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/data_mapping/json_conversion.py` & `deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/data_mapping/json_conversion.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from collections import defaultdict
 from itertools import count
 from collections.abc import Generator, Iterable
 
 
 def json_links(
         i: int,
```

### Comparing `deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/deephaven_figure/DeephavenFigure.py` & `deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/deephaven_figure/DeephavenFigure.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+
 import json
 from collections.abc import Generator
 from typing import Callable
 
 from plotly.graph_objects import Figure
 
 from deephaven.plugin.object import Exporter
```

### Comparing `deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/deephaven_figure/custom_draw.py` & `deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/deephaven_figure/custom_draw.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from itertools import zip_longest
 from typing import Callable
 
 from pandas import DataFrame
 import plotly.graph_objects as go
 from plotly.graph_objects import Figure
```

### Comparing `deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/deephaven_figure/generate.py` & `deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/deephaven_figure/generate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from itertools import cycle, count
 from collections.abc import Generator
 from math import floor, ceil
 
 from pandas import DataFrame
 from plotly.graph_objects import Figure
 
@@ -209,15 +211,18 @@
                 custom_call_args[arg] = val
                 if arg == "labels":
                     # plotly express still handles most labeling
                     new_call_args[arg] = val
             elif arg.endswith('_scene'):
                 # this scene check needs to be before the range check to
                 # ensure scene args don't get converted to a list
-                new_call_args[arg.removesuffix('_scene')] = val
+                # these are equivalent for removing _scene but removesuffix
+                # was introduced in 3.9
+                # new_call_args[arg.removesuffix('_scene')] = val
+                new_call_args[arg[:-6]] = val
             elif arg.startswith("range_"):
                 # range is a special case as ranges are a list
                 # None can be specified for no range within a list of ranges
                 custom_call_args[arg] = val if \
                     (isinstance(val[0], list) or val[0] is None) else [val]
             elif any([arg in mappable for mappable in
                       [ATTACHED_UPDATE_MAP, SEQUENCE_ARGS_MAP, CUSTOM_LIST_ARGS]]):
```

### Comparing `deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/_private_utils.py` & `deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/plots/_private_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from functools import partial
 from typing import Callable
 from collections.abc import Generator
 
 import plotly.express as px
 from plotly.graph_objects import Figure
```

### Comparing `deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/area.py` & `deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/plots/area.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from plotly import express as px
 
 from deephaven.table import Table
 
 from ._private_utils import default_callback, process_args
 from ..deephaven_figure import generate_figure, DeephavenFigure
```

### Comparing `deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/bar.py` & `deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/plots/bar.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from functools import partial
 
 from plotly import express as px
 
 from deephaven.table import Table
 
 from ._private_utils import default_callback, validate_common_args, preprocess_and_layer, process_args
```

### Comparing `deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/distribution.py` & `deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/plots/distribution.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from functools import partial
 from typing import Callable
 
 from plotly import express as px
 
 from deephaven.table import Table
```

### Comparing `deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/financial.py` & `deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/plots/financial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from deephaven.table import Table
 
 from ._private_utils import default_callback, validate_common_args, process_args
 from ..deephaven_figure import generate_figure, draw_ohlc, draw_candlestick, DeephavenFigure
 
 
 def ohlc(
```

### Comparing `deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/hierarchial.py` & `deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/plots/hierarchial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from plotly import express as px
 
 from deephaven.table import Table
 
 from ._private_utils import default_callback, process_args
 from ..deephaven_figure import generate_figure, DeephavenFigure
 from ..preprocess import preprocess_aggregate
```

### Comparing `deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/line.py` & `deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/plots/line.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from plotly import express as px
 
 from deephaven.table import Table
 
 from ._private_utils import default_callback, process_args
 from ..deephaven_figure import generate_figure, DeephavenFigure
```

### Comparing `deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/pie.py` & `deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/plots/pie.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from plotly import express as px
 
 from deephaven.table import Table
 
 from ._private_utils import default_callback, process_args
 from ..deephaven_figure import generate_figure, DeephavenFigure
 from ..preprocess import preprocess_aggregate
```

### Comparing `deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/scatter.py` & `deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/plots/scatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from plotly import express as px
 
 from deephaven.table import Table
 
 from .distribution import attach_marginals, get_marg_args
 from ._private_utils import default_callback, process_args
 from ..deephaven_figure import generate_figure, DeephavenFigure
```

### Comparing `deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/plots/subplots.py` & `deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/plots/subplots.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import math
 
 from plotly.graph_objs import Figure
 
 from ._private_utils import layer
 from .. import DeephavenFigure
```

### Comparing `deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/preprocess/preprocess.py` & `deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/preprocess/preprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from collections.abc import Generator
 
 from deephaven.table import Table
 from deephaven import agg, empty_table, new_table
 from deephaven.column import long_col
 from deephaven.time import nanos_to_millis, diff_nanos
 from deephaven.updateby import cum_sum
```

### Comparing `deephaven-plugin-plotly-express-0.0.4/src/deephaven/plot/express/shared/shared.py` & `deephaven-plugin-plotly-express-0.0.5/src/deephaven/plot/express/shared/shared.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,31 @@
+from __future__ import annotations
+
 from collections.abc import Generator
 
 from deephaven.table import Table
 
 
 def combined_generator(
         generators: list[Generator[tuple | dict]],
         fill: any = None
 ) -> Generator[dict]:
     """Combines generators into dictionary updates iteratively
     One yield of this combined generator yields one yield from each dictionary,
     combined into a new dictionary.
 
     Args:
-      generators: Generators to combine. Each should yield
-    either a tuple of a key, value pair or a dictionary.
-      fill: Optional fill when the generators are exhausted
-      generators: list[Generator[tuple | dict]]: 
+      generators: list[Generator[tuple | dict]]:
+        Generators to combine. Each should yield either a tuple of a key, value pair or a dictionary.
       fill: any:  (Default value = None)
+        Optional fill when the generators are exhausted
 
-    Returns:
 
+    Yields:
+      dict: the combined dictionary
     """
     try:
         while True:
             full_update = {}
             for generator in generators:
                 update = next(generator)
                 if isinstance(update, tuple):
@@ -36,27 +38,22 @@
             yield fill
 
 
 def get_unique_names(
         table: Table,
         orig_names: list[str]
 ) -> dict[str, str]:
-    """Calculate names that do not occur in table, starting from the names in
-    orig_names
+    """Calculate names that do not occur in table, starting from the names in orig_names
 
     Args:
-      table: The table to check against
-      orig_names: return: A dictionary that maps orig_names to new names that are not found
-    in the table
-      table: Table: 
-      orig_names: list[str]: 
+      table: Table: The table to check against
+      orig_names: list[str]: The original names to get unique versions of
 
     Returns:
-      A dictionary that maps orig_names to new names that are not found
-      in the table
+      dict[str, str]: A dictionary that maps orig_names to new names that are not found in the table
 
     """
     new_names = {}
 
     table_columns = {column.name for column in table.columns}
     for name in orig_names:
         new_name = name
```

### Comparing `deephaven-plugin-plotly-express-0.0.4/src/deephaven_plugin_plotly_express.egg-info/PKG-INFO` & `deephaven-plugin-plotly-express-0.0.5/src/deephaven_plugin_plotly_express.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deephaven-plugin-plotly-express
-Version: 0.0.4
+Version: 0.0.5
 Summary: Deephaven Chart Plugin
 Home-page: https://github.com/deephaven/deephaven-plugin-plotly-express
 Author: Devin Smith, Vlad Babich, Joe Numainville
 Author-email: josephnumainville@deephaven.io
 Project-URL: Source Code, https://github.com/deephaven/deephaven-plugin-plotly-express
 Project-URL: Bug Tracker, https://github.com/deephaven/deephaven-plugin-plotly-express/issues
 Keywords: deephaven,plugin,graph
```

### Comparing `deephaven-plugin-plotly-express-0.0.4/src/deephaven_plugin_plotly_express.egg-info/SOURCES.txt` & `deephaven-plugin-plotly-express-0.0.5/src/deephaven_plugin_plotly_express.egg-info/SOURCES.txt`

 * *Files identical despite different names*

