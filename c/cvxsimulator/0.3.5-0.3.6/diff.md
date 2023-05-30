# Comparing `tmp/cvxsimulator-0.3.5.tar.gz` & `tmp/cvxsimulator-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxsimulator-0.3.5.tar", max compression
+gzip compressed data, was "cvxsimulator-0.3.6.tar", max compression
```

## Comparing `cvxsimulator-0.3.5.tar` & `cvxsimulator-0.3.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11375 2023-05-29 22:24:38.950151 cvxsimulator-0.3.5/LICENSE
--rw-r--r--   0        0        0     4911 2023-05-29 22:24:38.950151 cvxsimulator-0.3.5/README.md
--rw-r--r--   0        0        0        0 2023-05-29 22:24:39.034151 cvxsimulator-0.3.5/cvx/simulator/__init__.py
--rw-r--r--   0        0        0    13964 2023-05-29 22:24:39.034151 cvxsimulator-0.3.5/cvx/simulator/builder.py
--rw-r--r--   0        0        0     1167 2023-05-29 22:24:39.034151 cvxsimulator-0.3.5/cvx/simulator/grid.py
--rw-r--r--   0        0        0     1163 2023-05-29 22:24:39.034151 cvxsimulator-0.3.5/cvx/simulator/metrics.py
--rw-r--r--   0        0        0     1422 2023-05-29 22:24:39.034151 cvxsimulator-0.3.5/cvx/simulator/month.py
--rw-r--r--   0        0        0    18879 2023-05-29 22:24:39.034151 cvxsimulator-0.3.5/cvx/simulator/portfolio.py
--rw-r--r--   0        0        0      464 2023-05-29 22:24:39.034151 cvxsimulator-0.3.5/cvx/simulator/trading_costs.py
--rw-r--r--   0        0        0      608 2023-05-29 22:25:10.590320 cvxsimulator-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     5498 1970-01-01 00:00:00.000000 cvxsimulator-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0    11375 2023-05-30 06:57:16.794915 cvxsimulator-0.3.6/LICENSE
+-rw-r--r--   0        0        0     5040 2023-05-30 06:57:16.794915 cvxsimulator-0.3.6/README.md
+-rw-r--r--   0        0        0        0 2023-05-30 06:57:16.890915 cvxsimulator-0.3.6/cvx/simulator/__init__.py
+-rw-r--r--   0        0        0    13964 2023-05-30 06:57:16.890915 cvxsimulator-0.3.6/cvx/simulator/builder.py
+-rw-r--r--   0        0        0     1167 2023-05-30 06:57:16.890915 cvxsimulator-0.3.6/cvx/simulator/grid.py
+-rw-r--r--   0        0        0     1163 2023-05-30 06:57:16.890915 cvxsimulator-0.3.6/cvx/simulator/metrics.py
+-rw-r--r--   0        0        0     1422 2023-05-30 06:57:16.890915 cvxsimulator-0.3.6/cvx/simulator/month.py
+-rw-r--r--   0        0        0    18895 2023-05-30 06:57:16.890915 cvxsimulator-0.3.6/cvx/simulator/portfolio.py
+-rw-r--r--   0        0        0      514 2023-05-30 06:57:16.890915 cvxsimulator-0.3.6/cvx/simulator/trading_costs.py
+-rw-r--r--   0        0        0      608 2023-05-30 06:57:55.683097 cvxsimulator-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     5627 1970-01-01 00:00:00.000000 cvxsimulator-0.3.6/PKG-INFO
```

### Comparing `cvxsimulator-0.3.5/LICENSE` & `cvxsimulator-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.3.5/README.md` & `cvxsimulator-0.3.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # [cvxsimulator](http://www.cvxgrp.org/simulator/)
 
 [![PyPI version](https://badge.fury.io/py/cvxsimulator.svg)](https://badge.fury.io/py/cvxsimulator)
 [![Apache 2.0 License](https://img.shields.io/badge/License-APACHEv2-brightgreen.svg)](https://github.com/cvxgrp/simulator/blob/master/LICENSE)
 [![PyPI download month](https://img.shields.io/pypi/dm/cvxsimulator.svg)](https://pypi.python.org/pypi/cvxsimulator/)
+[![Coverage Status](https://coveralls.io/repos/github/cvxgrp/simulator/badge.svg)](https://coveralls.io/github/cvxgrp/simulator)
 
 Given a universe of $m$ assets we are given prices for each of them at time $t_1, t_2, \ldots t_n$, 
 e.g. we operate using an $n \times m$ matrix where each column corresponds to a particular asset.
 
 In a backtest we iterate in time (e.g. row by row) through the matrix and allocate positions to all or some of the assets.
 This tool shall help to simplify the accounting. It keeps track of the available cash, the profits achieved, etc.
```

### Comparing `cvxsimulator-0.3.5/cvx/simulator/builder.py` & `cvxsimulator-0.3.6/cvx/simulator/builder.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.3.5/cvx/simulator/grid.py` & `cvxsimulator-0.3.6/cvx/simulator/grid.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.3.5/cvx/simulator/metrics.py` & `cvxsimulator-0.3.6/cvx/simulator/metrics.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.3.5/cvx/simulator/month.py` & `cvxsimulator-0.3.6/cvx/simulator/month.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.3.5/cvx/simulator/portfolio.py` & `cvxsimulator-0.3.6/cvx/simulator/portfolio.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,17 +11,14 @@
     pd.testing.assert_frame_equal(portfolio1.prices, portfolio2.prices)
 
     stocks = portfolio1.stocks - portfolio2.stocks
 
     return EquityPortfolio(prices=portfolio1.prices, stocks=stocks, initial_cash=initial_cash, trading_cost_model=trading_cost_model)
 
 
-
-
-
 @dataclass(frozen=True)
 class EquityPortfolio:
     """ A class that represents an equity portfolio
     and contains dataframes for prices and stock holdings,
     as well as optional parameters for trading cost models
     and initial cash values.
 
@@ -107,15 +104,15 @@
         Notes: The function calculates the weights of various assets
         in the portfolio by dividing the equity positions
         for each asset (as represented in the equity dataframe)
         by the total portfolio value (as represented in the nav dataframe).
         Both dataframes are assumed to have the same dimensions.
         The resulting dataframe will show the relative weight
         of each asset in the portfolio at each point in time. """
-        return self.equity / self.nav
+        return self.equity.apply(lambda x: x / self.nav)
 
     def __getitem__(self, time):
         """The `__getitem__` method retrieves the stock data for a specific time in the dataframe.
         It returns the stock data for that time.
 
         The method takes one input parameter:
         - `time`: the time index for which to retrieve the stock data
```

### Comparing `cvxsimulator-0.3.5/pyproject.toml` & `cvxsimulator-0.3.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cvxsimulator"
-version = "v0.3.5"
+version = "v0.3.6"
 description = "Simple simulator for investors"
 authors = ["Thomas Schmelzer"]
 readme = "README.md"
 repository = "https://github.com/cvxgrp/simulator"
 packages = [{include = "cvx"}]
 
 [tool.poetry.dependencies]
```

### Comparing `cvxsimulator-0.3.5/PKG-INFO` & `cvxsimulator-0.3.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxsimulator
-Version: 0.3.5
+Version: 0.3.6
 Summary: Simple simulator for investors
 Home-page: https://github.com/cvxgrp/simulator
 Author: Thomas Schmelzer
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -16,14 +16,15 @@
 Description-Content-Type: text/markdown
 
 # [cvxsimulator](http://www.cvxgrp.org/simulator/)
 
 [![PyPI version](https://badge.fury.io/py/cvxsimulator.svg)](https://badge.fury.io/py/cvxsimulator)
 [![Apache 2.0 License](https://img.shields.io/badge/License-APACHEv2-brightgreen.svg)](https://github.com/cvxgrp/simulator/blob/master/LICENSE)
 [![PyPI download month](https://img.shields.io/pypi/dm/cvxsimulator.svg)](https://pypi.python.org/pypi/cvxsimulator/)
+[![Coverage Status](https://coveralls.io/repos/github/cvxgrp/simulator/badge.svg)](https://coveralls.io/github/cvxgrp/simulator)
 
 Given a universe of $m$ assets we are given prices for each of them at time $t_1, t_2, \ldots t_n$, 
 e.g. we operate using an $n \times m$ matrix where each column corresponds to a particular asset.
 
 In a backtest we iterate in time (e.g. row by row) through the matrix and allocate positions to all or some of the assets.
 This tool shall help to simplify the accounting. It keeps track of the available cash, the profits achieved, etc.
```

