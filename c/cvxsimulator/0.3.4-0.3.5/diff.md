# Comparing `tmp/cvxsimulator-0.3.4.tar.gz` & `tmp/cvxsimulator-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxsimulator-0.3.4.tar", max compression
+gzip compressed data, was "cvxsimulator-0.3.5.tar", max compression
```

## Comparing `cvxsimulator-0.3.4.tar` & `cvxsimulator-0.3.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11375 2023-05-19 18:49:35.531294 cvxsimulator-0.3.4/LICENSE
--rw-r--r--   0        0        0     4907 2023-05-19 18:49:35.531294 cvxsimulator-0.3.4/README.md
--rw-r--r--   0        0        0        0 2023-05-19 18:49:35.611296 cvxsimulator-0.3.4/cvx/simulator/__init__.py
--rw-r--r--   0        0        0    14008 2023-05-19 18:49:35.611296 cvxsimulator-0.3.4/cvx/simulator/builder.py
--rw-r--r--   0        0        0      990 2023-05-19 18:49:35.611296 cvxsimulator-0.3.4/cvx/simulator/grid.py
--rw-r--r--   0        0        0     1163 2023-05-19 18:49:35.611296 cvxsimulator-0.3.4/cvx/simulator/metrics.py
--rw-r--r--   0        0        0     1422 2023-05-19 18:49:35.611296 cvxsimulator-0.3.4/cvx/simulator/month.py
--rw-r--r--   0        0        0    18879 2023-05-19 18:49:35.611296 cvxsimulator-0.3.4/cvx/simulator/portfolio.py
--rw-r--r--   0        0        0      464 2023-05-19 18:49:35.611296 cvxsimulator-0.3.4/cvx/simulator/trading_costs.py
--rw-r--r--   0        0        0      608 2023-05-19 18:50:03.515740 cvxsimulator-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     5476 1970-01-01 00:00:00.000000 cvxsimulator-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0    11375 2023-05-29 22:24:38.950151 cvxsimulator-0.3.5/LICENSE
+-rw-r--r--   0        0        0     4911 2023-05-29 22:24:38.950151 cvxsimulator-0.3.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 22:24:39.034151 cvxsimulator-0.3.5/cvx/simulator/__init__.py
+-rw-r--r--   0        0        0    13964 2023-05-29 22:24:39.034151 cvxsimulator-0.3.5/cvx/simulator/builder.py
+-rw-r--r--   0        0        0     1167 2023-05-29 22:24:39.034151 cvxsimulator-0.3.5/cvx/simulator/grid.py
+-rw-r--r--   0        0        0     1163 2023-05-29 22:24:39.034151 cvxsimulator-0.3.5/cvx/simulator/metrics.py
+-rw-r--r--   0        0        0     1422 2023-05-29 22:24:39.034151 cvxsimulator-0.3.5/cvx/simulator/month.py
+-rw-r--r--   0        0        0    18879 2023-05-29 22:24:39.034151 cvxsimulator-0.3.5/cvx/simulator/portfolio.py
+-rw-r--r--   0        0        0      464 2023-05-29 22:24:39.034151 cvxsimulator-0.3.5/cvx/simulator/trading_costs.py
+-rw-r--r--   0        0        0      608 2023-05-29 22:25:10.590320 cvxsimulator-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     5498 1970-01-01 00:00:00.000000 cvxsimulator-0.3.5/PKG-INFO
```

### Comparing `cvxsimulator-0.3.4/LICENSE` & `cvxsimulator-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.3.4/README.md` & `cvxsimulator-0.3.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -54,30 +54,30 @@
     stocks = pd.Series(index=b.assets, data=0.0)
     stocks[pair] = [state.nav, -state.nav] / state.prices[pair].values
     # update the position 
     b[t[-1]] = 0.1 * stocks
 ```
 
 Here t is the growing list of timestamps, e.g. in the first iteration
-t is $t1, t2$, in the second iteration it will be $t1, t2, t3$ etc.
+t is $t1$, in the second iteration it will be $t1, t2$ etc.
 
 A lot of magic is hidden in the state variable. 
 The state gives access to the currently available cash, the current prices and the current valuation of all holdings.
 
 Here's a slightly more realistic loop. Given a set of $4$ assets we want to implmenent the popular $1/n$ strategy.
 
 ```python
 for t, state in b:
     # each day we invest a quarter of the capital in the assets
     b[t[-1]] = 0.25 * state.nav / state.prices
 ```
 
 Note that we update the position at the last element in the t list 
 using a series of actual stocks rather than weights or cashpositions.
-The builder class also exposes setters for such conventions.
+The builder class also exposes setters for such alternative conventions.
 
 ```python
 for t, state in b:
     # each day we invest a quarter of the capital in the assets
     b.set_weights(t[-1], pd.Series(index=b.assets, data = 0.25))
 ```
```

### Comparing `cvxsimulator-0.3.4/cvx/simulator/builder.py` & `cvxsimulator-0.3.5/cvx/simulator/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,15 +161,14 @@
 
     assert isinstance(prices, pd.DataFrame)
     assert prices.index.is_monotonic_increasing
     assert prices.index.is_unique
 
     stocks = pd.DataFrame(index=prices.index, columns=prices.columns, data=0.0, dtype=float)
 
-    trading_cost_model = trading_cost_model
     builder = _Builder(stocks=stocks, prices=prices.ffill(), initial_cash=float(initial_cash),
                     trading_cost_model=trading_cost_model)
 
     if weights is not None:
         for t, state in builder:
             builder.set_weights(time=t[-1], weights=weights.loc[t[-1]])
```

### Comparing `cvxsimulator-0.3.4/cvx/simulator/grid.py` & `cvxsimulator-0.3.5/cvx/simulator/grid.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,18 +13,23 @@
     """
     series = pd.Series(index=index, data=index)
     a = series.resample(rule=rule).first()
     return pd.DatetimeIndex(a.values)
 
 
 def project_frame_to_grid(frame, grid):
-    """The project_frame_to_grid function projects a pandas
-    DataFrame object onto a given index grid.
-
-    The function returns a new DataFrame that is only updated for times in the grid,
-    otherwise the previous values carry over.
+    """
+    The project_frame_to_grid function projects a pandas DataFrame
+    to a coarser grid while still sharing the same index.
+    It does that by taking over values of the frame from the coarser
+    grid that are then forward filled.
+    An application would be monthly rebalancing of a portfolio.
+    E.g. on days in a particular grid we adjust the position and keep
+    it constant for the rest of the month.
 
-    Note that the function does not modify the input frame object, but rather returns a new object.
+    :param frame: the frame (existing on a finer grid)
+    :param grid: the coarse grid
+    :return: a frame changing only values on days in the grid
     """
-    sample = pd.DataFrame(index=frame.index, columns=frame.columns, data=np.NaN)
+    sample = np.NaN * frame
     sample.loc[grid] = frame.loc[grid]
     return sample.ffill()
```

### Comparing `cvxsimulator-0.3.4/cvx/simulator/metrics.py` & `cvxsimulator-0.3.5/cvx/simulator/metrics.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.3.4/cvx/simulator/month.py` & `cvxsimulator-0.3.5/cvx/simulator/month.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.3.4/cvx/simulator/portfolio.py` & `cvxsimulator-0.3.5/cvx/simulator/portfolio.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.3.4/pyproject.toml` & `cvxsimulator-0.3.5/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "cvxsimulator"
-version = "v0.3.4"
+version = "v0.3.5"
 description = "Simple simulator for investors"
 authors = ["Thomas Schmelzer"]
 readme = "README.md"
 repository = "https://github.com/cvxgrp/simulator"
 packages = [{include = "cvx"}]
 
 [tool.poetry.dependencies]
-python = "^3.9"
-numpy = "^1.24.2"
-pandas = "<2.0.0"   # unfortunately otherwise crash with quantstats
+python = ">=3.8"
+numpy = "*"
+pandas = "*"   # unfortunately crash with quantstats for pandas >= 2.0.0
 
 [tool.poetry.dev-dependencies]
 pytest = "7.2.0"
 pytest-cov = "4.0.0"
 yfinance = "*"
 quantstats = "*"
 plotly = "*"
```

### Comparing `cvxsimulator-0.3.4/PKG-INFO` & `cvxsimulator-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: cvxsimulator
-Version: 0.3.4
+Version: 0.3.5
 Summary: Simple simulator for investors
 Home-page: https://github.com/cvxgrp/simulator
 Author: Thomas Schmelzer
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: numpy (>=1.24.2,<2.0.0)
-Requires-Dist: pandas (<2.0.0)
+Requires-Dist: numpy
+Requires-Dist: pandas
 Project-URL: Repository, https://github.com/cvxgrp/simulator
 Description-Content-Type: text/markdown
 
 # [cvxsimulator](http://www.cvxgrp.org/simulator/)
 
 [![PyPI version](https://badge.fury.io/py/cvxsimulator.svg)](https://badge.fury.io/py/cvxsimulator)
 [![Apache 2.0 License](https://img.shields.io/badge/License-APACHEv2-brightgreen.svg)](https://github.com/cvxgrp/simulator/blob/master/LICENSE)
@@ -70,30 +71,30 @@
     stocks = pd.Series(index=b.assets, data=0.0)
     stocks[pair] = [state.nav, -state.nav] / state.prices[pair].values
     # update the position 
     b[t[-1]] = 0.1 * stocks
 ```
 
 Here t is the growing list of timestamps, e.g. in the first iteration
-t is $t1, t2$, in the second iteration it will be $t1, t2, t3$ etc.
+t is $t1$, in the second iteration it will be $t1, t2$ etc.
 
 A lot of magic is hidden in the state variable. 
 The state gives access to the currently available cash, the current prices and the current valuation of all holdings.
 
 Here's a slightly more realistic loop. Given a set of $4$ assets we want to implmenent the popular $1/n$ strategy.
 
 ```python
 for t, state in b:
     # each day we invest a quarter of the capital in the assets
     b[t[-1]] = 0.25 * state.nav / state.prices
 ```
 
 Note that we update the position at the last element in the t list 
 using a series of actual stocks rather than weights or cashpositions.
-The builder class also exposes setters for such conventions.
+The builder class also exposes setters for such alternative conventions.
 
 ```python
 for t, state in b:
     # each day we invest a quarter of the capital in the assets
     b.set_weights(t[-1], pd.Series(index=b.assets, data = 0.25))
 ```
```

