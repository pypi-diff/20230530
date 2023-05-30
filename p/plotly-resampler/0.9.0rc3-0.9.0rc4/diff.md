# Comparing `tmp/plotly_resampler-0.9.0rc3.tar.gz` & `tmp/plotly_resampler-0.9.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotly_resampler-0.9.0rc3.tar", max compression
+gzip compressed data, was "plotly_resampler-0.9.0rc4.tar", max compression
```

## Comparing `plotly_resampler-0.9.0rc3.tar` & `plotly_resampler-0.9.0rc4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1115 2023-05-03 12:32:58.928306 plotly_resampler-0.9.0rc3/LICENSE
--rw-r--r--   0        0        0    11180 2023-05-15 07:29:18.434096 plotly_resampler-0.9.0rc3/README.md
--rw-r--r--   0        0        0      853 2023-05-15 07:29:43.141241 plotly_resampler-0.9.0rc3/plotly_resampler/__init__.py
--rw-r--r--   0        0        0      796 2023-05-03 12:32:58.964305 plotly_resampler-0.9.0rc3/plotly_resampler/aggregation/__init__.py
--rw-r--r--   0        0        0     6934 2023-05-03 12:32:58.964305 plotly_resampler-0.9.0rc3/plotly_resampler/aggregation/aggregation_interface.py
--rw-r--r--   0        0        0    11877 2023-05-03 12:32:58.968305 plotly_resampler-0.9.0rc3/plotly_resampler/aggregation/aggregators.py
--rw-r--r--   0        0        0     3048 2023-05-03 12:32:58.968305 plotly_resampler-0.9.0rc3/plotly_resampler/aggregation/gap_handler_interface.py
--rw-r--r--   0        0        0     3179 2023-05-03 12:32:58.968305 plotly_resampler-0.9.0rc3/plotly_resampler/aggregation/gap_handlers.py
--rw-r--r--   0        0        0     8088 2023-05-15 07:29:18.434096 plotly_resampler-0.9.0rc3/plotly_resampler/aggregation/plotly_aggregator_parser.py
--rw-r--r--   0        0        0      473 2023-03-08 10:44:50.208394 plotly_resampler-0.9.0rc3/plotly_resampler/figure_resampler/__init__.py
--rw-r--r--   0        0        0    23690 2023-05-03 12:32:58.968305 plotly_resampler-0.9.0rc3/plotly_resampler/figure_resampler/figure_resampler.py
--rw-r--r--   0        0        0    62492 2023-05-15 07:10:55.600245 plotly_resampler-0.9.0rc3/plotly_resampler/figure_resampler/figure_resampler_interface.py
--rw-r--r--   0        0        0    13669 2023-05-03 12:32:58.968305 plotly_resampler-0.9.0rc3/plotly_resampler/figure_resampler/figurewidget_resampler.py
--rw-r--r--   0        0        0     5376 2023-05-14 08:02:19.170287 plotly_resampler-0.9.0rc3/plotly_resampler/figure_resampler/utils.py
--rw-r--r--   0        0        0     4911 2023-03-08 10:44:50.208394 plotly_resampler-0.9.0rc3/plotly_resampler/registering.py
--rw-r--r--   0        0        0     2857 2023-05-15 07:29:29.573711 plotly_resampler-0.9.0rc3/pyproject.toml
--rw-r--r--   0        0        0    13126 1970-01-01 00:00:00.000000 plotly_resampler-0.9.0rc3/PKG-INFO
+-rw-r--r--   0        0        0     1115 2023-05-04 08:48:30.616798 plotly_resampler-0.9.0rc4/LICENSE
+-rw-r--r--   0        0        0    11180 2023-05-14 08:56:23.448441 plotly_resampler-0.9.0rc4/README.md
+-rw-r--r--   0        0        0      853 2023-05-30 13:29:45.868164 plotly_resampler-0.9.0rc4/plotly_resampler/__init__.py
+-rw-r--r--   0        0        0      796 2023-05-04 08:48:30.656798 plotly_resampler-0.9.0rc4/plotly_resampler/aggregation/__init__.py
+-rw-r--r--   0        0        0     6934 2023-05-04 08:48:30.656798 plotly_resampler-0.9.0rc4/plotly_resampler/aggregation/aggregation_interface.py
+-rw-r--r--   0        0        0    11877 2023-05-04 08:48:30.656798 plotly_resampler-0.9.0rc4/plotly_resampler/aggregation/aggregators.py
+-rw-r--r--   0        0        0     3489 2023-05-30 12:53:12.547957 plotly_resampler-0.9.0rc4/plotly_resampler/aggregation/gap_handler_interface.py
+-rw-r--r--   0        0        0     3179 2023-05-04 08:48:30.656798 plotly_resampler-0.9.0rc4/plotly_resampler/aggregation/gap_handlers.py
+-rw-r--r--   0        0        0     8961 2023-05-30 13:29:12.863934 plotly_resampler-0.9.0rc4/plotly_resampler/aggregation/plotly_aggregator_parser.py
+-rw-r--r--   0        0        0      473 2022-12-28 21:53:17.053836 plotly_resampler-0.9.0rc4/plotly_resampler/figure_resampler/__init__.py
+-rw-r--r--   0        0        0    23690 2023-05-04 08:48:30.660798 plotly_resampler-0.9.0rc4/plotly_resampler/figure_resampler/figure_resampler.py
+-rw-r--r--   0        0        0    62492 2023-05-14 08:41:15.136035 plotly_resampler-0.9.0rc4/plotly_resampler/figure_resampler/figure_resampler_interface.py
+-rw-r--r--   0        0        0    13669 2023-05-04 08:48:30.660798 plotly_resampler-0.9.0rc4/plotly_resampler/figure_resampler/figurewidget_resampler.py
+-rw-r--r--   0        0        0     5376 2023-05-15 07:51:36.039672 plotly_resampler-0.9.0rc4/plotly_resampler/figure_resampler/utils.py
+-rw-r--r--   0        0        0     4911 2022-12-28 21:53:17.053836 plotly_resampler-0.9.0rc4/plotly_resampler/registering.py
+-rw-r--r--   0        0        0     2857 2023-05-30 13:29:51.208202 plotly_resampler-0.9.0rc4/pyproject.toml
+-rw-r--r--   0        0        0    12876 1970-01-01 00:00:00.000000 plotly_resampler-0.9.0rc4/PKG-INFO
```

### Comparing `plotly_resampler-0.9.0rc3/LICENSE` & `plotly_resampler-0.9.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc3/README.md` & `plotly_resampler-0.9.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc3/plotly_resampler/__init__.py` & `plotly_resampler-0.9.0rc4/plotly_resampler/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from .aggregation import LTTB, EveryNthPoint, MinMaxLTTB
 from .figure_resampler import FigureResampler, FigureWidgetResampler
 from .registering import register_plotly_resampler, unregister_plotly_resampler
 
 __docformat__ = "numpy"
 __author__ = "Jonas Van Der Donckt, Jeroen Van Der Donckt, Emiel Deprost"
-__version__ = "0.9.0rc3"
+__version__ = "0.9.0rc4"
 
 __all__ = [
     "__version__",
     "FigureResampler",
     "FigureWidgetResampler",
     "MinMaxLTTB",
     "LTTB",
```

### Comparing `plotly_resampler-0.9.0rc3/plotly_resampler/aggregation/__init__.py` & `plotly_resampler-0.9.0rc4/plotly_resampler/aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc3/plotly_resampler/aggregation/aggregation_interface.py` & `plotly_resampler-0.9.0rc4/plotly_resampler/aggregation/aggregation_interface.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc3/plotly_resampler/aggregation/aggregators.py` & `plotly_resampler-0.9.0rc4/plotly_resampler/aggregation/aggregators.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc3/plotly_resampler/aggregation/gap_handler_interface.py` & `plotly_resampler-0.9.0rc4/plotly_resampler/aggregation/gap_handler_interface.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,27 @@
 from abc import ABC, abstractmethod
 from typing import Optional, Tuple
 
 import numpy as np
 
 
 class AbstractGapHandler(ABC):
+    def __init__(self, fill_value: Optional[float] = None):
+        """Constructor of AbstractGapHandler.
+
+        Parameters
+        ----------
+        fill_value: float, optional
+            The value to fill the gaps with, by default None.
+            Note that setting this value to 0 for filled area plots is particularly
+            useful.
+
+        """
+        self.fill_value = fill_value
+
     @abstractmethod
     def _get_gap_mask(self, x_agg: np.ndarray) -> Optional[np.ndarray]:
         """Get a boolean mask indicating the indices where there are gaps.
 
         If you require custom gap handling, you can implement this method to return a
         boolean mask indicating the indices where there are gaps.
 
@@ -28,31 +41,31 @@
         Optional[np.ndarray]
             A boolean mask indicating the indices where there are gaps. If there are no
             gaps, None is returned.
 
         """
         pass
 
-    def insert_none_between_gaps(
+    def insert_fill_value_between_gaps(
         self,
         x_agg: np.ndarray,
         y_agg: np.ndarray,
         idxs: np.ndarray,
     ) -> Tuple[np.ndarray, np.ndarray]:
-        """Insert None values in the y_agg array when there are gaps.
+        """Insert the fill_value in the y_agg array where there are gaps.
 
         Gaps are determined by the x_agg array. The `_get_gap_mask` method is used to
         determine a boolean mask indicating the indices where there are gaps.
 
         Parameters
         ----------
         x_agg: np.ndarray
             The x array. This is used to determine the gaps.
         y_agg: np.ndarray
-            The y array. A copy of this array will be expanded with None values where
+            The y array. A copy of this array will be expanded with fill_values where
             there are gaps.
         idxs: np.ndarray
             The index array. This is relevant aggregators that perform data point
             selection (e.g., max, min, etc.) - this array will be expanded with the
             same indices where there are gaps.
 
         Returns
@@ -79,10 +92,12 @@
             y_agg_exp_nan.dtype.type, np.bool_
         ):
             y_agg_exp_nan = y_agg_exp_nan.astype("float")
 
         # Set the NaN values
         # We add the gap index offset (via the np.arange) to the indices to account for
         # the repeats (i.e., expanded y_agg array).
-        y_agg_exp_nan[np.where(gap_mask)[0] + np.arange(gap_mask.sum())] = None
+        y_agg_exp_nan[
+            np.where(gap_mask)[0] + np.arange(gap_mask.sum())
+        ] = self.fill_value
 
         return y_agg_exp_nan, idx_exp_nan
```

### Comparing `plotly_resampler-0.9.0rc3/plotly_resampler/aggregation/gap_handlers.py` & `plotly_resampler-0.9.0rc4/plotly_resampler/aggregation/gap_handlers.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc3/plotly_resampler/aggregation/plotly_aggregator_parser.py` & `plotly_resampler-0.9.0rc4/plotly_resampler/aggregation/plotly_aggregator_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -84,14 +84,66 @@
 
         # Search the index-positions
         start_idx = bisect.bisect_left(hf_trace_data["x"], start)
         end_idx = bisect.bisect_right(hf_trace_data["x"], end)
         return start_idx, end_idx
 
     @staticmethod
+    def _handle_gaps(
+        hf_trace_data: dict,
+        hf_x: np.ndarray,
+        agg_x: np.ndarray,
+        agg_y: np.ndarray,
+        indices: np.ndarray,
+    ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+        """Handle the gaps in the aggregated data.
+
+        Returns:
+            - agg_x: the aggregated x-values
+            - agg_y: the aggregated y-values
+            - indices: the indices of the hf_data data that were aggregated
+
+        """
+        gap_handler: AbstractGapHandler = hf_trace_data["gap_handler"]
+        downsampler = hf_trace_data["downsampler"]
+
+        # TODO check for trace mode (markers, lines, etc.) and only perform the
+        # gap insertion methodology when the mode is lines.
+        # if trace.get("connectgaps") != True and
+        if (
+            isinstance(gap_handler, NoGapHandler)
+            # rangeIndex | datetimeIndex with freq -> equally spaced x; so no gaps
+            or isinstance(hf_trace_data["x"], pd.RangeIndex)
+            or (
+                isinstance(hf_trace_data["x"], pd.DatetimeIndex)
+                and hf_trace_data["x"].freq is not None
+            )
+        ):
+            return agg_x, agg_y, indices
+
+        # Interleave the gaps
+        # View the data as an int64 when we have a DatetimeIndex
+        # We only want to detect gaps, so we only want to compare values.
+        agg_x_parsed = PlotlyAggregatorParser.parse_hf_data(agg_x)
+        xdt = agg_x_parsed.dtype
+        if np.issubdtype(xdt, np.timedelta64) or np.issubdtype(xdt, np.datetime64):
+            agg_x_parsed = agg_x_parsed.view("int64")
+
+        agg_y, indices = gap_handler.insert_fill_value_between_gaps(
+            agg_x_parsed, agg_y, indices
+        )
+        if isinstance(downsampler, DataPointSelector):
+            agg_x = hf_x[indices]
+        elif isinstance(downsampler, DataAggregator):
+            # The indices are in this case a repeat
+            agg_x = agg_x[indices]
+
+        return agg_x, agg_y, indices
+
+    @staticmethod
     def aggregate(
         hf_trace_data: dict,
         start_idx: int,
         end_idx: int,
     ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
         """Aggregate the data in `hf_trace_data` between `start_idx` and `end_idx`.
 
@@ -103,20 +155,22 @@
             These indices are useful to select the corresponding hf_data from
             non `x` and `y` data (e.g. `text`, `marker_size`, `marker_color`).
 
         """
         hf_x = hf_trace_data["x"][start_idx:end_idx]
         hf_y = hf_trace_data["y"][start_idx:end_idx]
 
-        # No downsampling needed ; we show the raw data as is, no gap detection
+        # No downsampling needed ; we show the raw data as is, but with gap-detection
         if (end_idx - start_idx) <= hf_trace_data["max_n_samples"]:
-            return hf_x, hf_y, np.arange(len(hf_y))
+            indices = np.arange(len(hf_y))  # no downsampling - all values are selected
+            return PlotlyAggregatorParser._handle_gaps(
+                hf_trace_data, hf_x=hf_x, agg_x=hf_x, agg_y=hf_y, indices=indices
+            )
 
         downsampler = hf_trace_data["downsampler"]
-        gap_handler: AbstractGapHandler = hf_trace_data["gap_handler"]
 
         hf_x_parsed = PlotlyAggregatorParser.parse_hf_data(hf_x)
         hf_y_parsed = PlotlyAggregatorParser.parse_hf_data(hf_y)
 
         if isinstance(downsampler, DataPointSelector):
             s_v = hf_y_parsed
             if isinstance(s_v, pd.Categorical):  # pd.Categorical (has no .values)
@@ -157,39 +211,10 @@
             indices = np.arange(len(agg_x))
         else:
             raise ValueError(
                 "Invalid downsampler instance, must be either a "
                 + f"DataAggregator or a DataPointSelector, got {type(downsampler)}"
             )
 
-        # TODO check for trace mode (markers, lines, etc.) and only perform the
-        # gap insertion methodology when the mode is lines.
-        # if trace.get("connectgaps") != True and
-        if (
-            isinstance(gap_handler, NoGapHandler)
-            # rangeIndex | datetimeIndex with freq -> equally spaced x; so no gaps
-            or isinstance(hf_trace_data["x"], pd.RangeIndex)
-            or (
-                isinstance(hf_trace_data["x"], pd.DatetimeIndex)
-                and hf_trace_data["x"].freq is not None
-            )
-        ):
-            return agg_x, agg_y, indices
-
-        # Interleave the gaps
-        # View the data as an int64 when we have a DatetimeIndex
-        # We only want to detect gaps, so we only want to compare values.
-        agg_x_parsed = PlotlyAggregatorParser.parse_hf_data(agg_x)
-        xdt = agg_x_parsed.dtype
-        if np.issubdtype(xdt, np.timedelta64) or np.issubdtype(xdt, np.datetime64):
-            agg_x_parsed = agg_x_parsed.view("int64")
-
-        agg_y, indices = gap_handler.insert_none_between_gaps(
-            agg_x_parsed, agg_y, indices
+        return PlotlyAggregatorParser._handle_gaps(
+            hf_trace_data, hf_x=hf_x, agg_x=agg_x, agg_y=agg_y, indices=indices
         )
-        if isinstance(downsampler, DataPointSelector):
-            agg_x = hf_x[indices]
-        elif isinstance(downsampler, DataAggregator):
-            # The indices are in this case a repeat
-            agg_x = agg_x[indices]
-
-        return agg_x, agg_y, indices
```

### Comparing `plotly_resampler-0.9.0rc3/plotly_resampler/figure_resampler/figure_resampler.py` & `plotly_resampler-0.9.0rc4/plotly_resampler/figure_resampler/figure_resampler.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc3/plotly_resampler/figure_resampler/figure_resampler_interface.py` & `plotly_resampler-0.9.0rc4/plotly_resampler/figure_resampler/figure_resampler_interface.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc3/plotly_resampler/figure_resampler/figurewidget_resampler.py` & `plotly_resampler-0.9.0rc4/plotly_resampler/figure_resampler/figurewidget_resampler.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc3/plotly_resampler/figure_resampler/utils.py` & `plotly_resampler-0.9.0rc4/plotly_resampler/figure_resampler/utils.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc3/plotly_resampler/registering.py` & `plotly_resampler-0.9.0rc4/plotly_resampler/registering.py`

 * *Files identical despite different names*

### Comparing `plotly_resampler-0.9.0rc3/pyproject.toml` & `plotly_resampler-0.9.0rc4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "plotly-resampler"  # Do not forget to update the __init__.py __version__ variable
-version = "0.9.0rc3"
+version = "0.9.0rc4"
 description = "Visualizing large time series with plotly"
 authors = ["Jonas Van Der Donckt", "Jeroen Van Der Donckt", "Emiel Deprost"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/predict-idlab/plotly-resampler"
 documentation = "https://predict-idlab.github.io/plotly-resampler"
 keywords = ["time-series", "visualization", "resampling", "plotly", "plotly-dash"]
```

### Comparing `plotly_resampler-0.9.0rc3/PKG-INFO` & `plotly_resampler-0.9.0rc4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plotly-resampler
-Version: 0.9.0rc3
+Version: 0.9.0rc4
 Summary: Visualizing large time series with plotly
 Home-page: https://github.com/predict-idlab/plotly-resampler
 License: MIT
 Keywords: time-series,visualization,resampling,plotly,plotly-dash
 Author: Jonas Van Der Donckt
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,20 +15,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: inline-persistent
 Requires-Dist: Flask-Cors (>=3.0.10,<4.0.0) ; extra == "inline-persistent"
 Requires-Dist: dash (>=2.2.0,<3.0.0)
 Requires-Dist: jupyter-dash (>=0.4.2)
 Requires-Dist: kaleido (==0.2.1) ; extra == "inline-persistent"
 Requires-Dist: numpy (>=1.14) ; python_version < "3.11"
 Requires-Dist: numpy (>=1.24) ; python_version >= "3.11"
```

#### html2text {}

```diff
@@ -1,34 +1,30 @@
-Metadata-Version: 2.1 Name: plotly-resampler Version: 0.9.0rc3 Summary:
+Metadata-Version: 2.1 Name: plotly-resampler Version: 0.9.0rc4 Summary:
 Visualizing large time series with plotly Home-page: https://github.com/
 predict-idlab/plotly-resampler License: MIT Keywords: time-
 series,visualization,resampling,plotly,plotly-dash Author: Jonas Van Der Donckt
 Requires-Python: >=3.7.1,<4.0.0 Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: POSIX :: Linux Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Provides-Extra: inline-persistent Requires-Dist:
-Flask-Cors (>=3.0.10,<4.0.0) ; extra == "inline-persistent" Requires-Dist: dash
-(>=2.2.0,<3.0.0) Requires-Dist: jupyter-dash (>=0.4.2) Requires-Dist: kaleido
-(==0.2.1) ; extra == "inline-persistent" Requires-Dist: numpy (>=1.14) ;
-python_version < "3.11" Requires-Dist: numpy (>=1.24) ; python_version >=
-"3.11" Requires-Dist: orjson (>=3.8.0,<4.0.0) Requires-Dist: pandas (>=1)
-Requires-Dist: plotly (>=5.5.0,<6.0.0) Requires-Dist: trace-updater (>=0.0.8)
-Requires-Dist: tsdownsample (==0.1.2) Project-URL: Documentation, https://
-predict-idlab.github.io/plotly-resampler Project-URL: Repository, https://
-github.com/predict-idlab/plotly-resampler Description-Content-Type: text/
-markdown
+Provides-Extra: inline-persistent Requires-Dist: Flask-Cors (>=3.0.10,<4.0.0) ;
+extra == "inline-persistent" Requires-Dist: dash (>=2.2.0,<3.0.0) Requires-
+Dist: jupyter-dash (>=0.4.2) Requires-Dist: kaleido (==0.2.1) ; extra ==
+"inline-persistent" Requires-Dist: numpy (>=1.14) ; python_version < "3.11"
+Requires-Dist: numpy (>=1.24) ; python_version >= "3.11" Requires-Dist: orjson
+(>=3.8.0,<4.0.0) Requires-Dist: pandas (>=1) Requires-Dist: plotly
+(>=5.5.0,<6.0.0) Requires-Dist: trace-updater (>=0.0.8) Requires-Dist:
+tsdownsample (==0.1.2) Project-URL: Documentation, https://predict-
+idlab.github.io/plotly-resampler Project-URL: Repository, https://github.com/
+predict-idlab/plotly-resampler Description-Content-Type: text/markdown
                             [Plotly-Resampler_logo]
 [![PyPI Latest Release](https://img.shields.io/pypi/v/plotly-resampler.svg)]
 (https://pypi.org/project/plotly-resampler/) [![support-version](https://
 img.shields.io/pypi/pyversions/plotly-resampler)](https://img.shields.io/pypi/
 pyversions/plotly-resampler) [![codecov](https://img.shields.io/codecov/c/
 github/predict-idlab/plotly-resampler?logo=codecov)](https://codecov.io/gh/
 predict-idlab/plotly-resampler) [![Downloads](https://pepy.tech/badge/plotly-
```

