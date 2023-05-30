# Comparing `tmp/cvxsimulator-0.3.6.tar.gz` & `tmp/cvxsimulator-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxsimulator-0.3.6.tar", max compression
+gzip compressed data, was "cvxsimulator-0.4.0.tar", max compression
```

## Comparing `cvxsimulator-0.3.6.tar` & `cvxsimulator-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11375 2023-05-30 06:57:16.794915 cvxsimulator-0.3.6/LICENSE
--rw-r--r--   0        0        0     5040 2023-05-30 06:57:16.794915 cvxsimulator-0.3.6/README.md
--rw-r--r--   0        0        0        0 2023-05-30 06:57:16.890915 cvxsimulator-0.3.6/cvx/simulator/__init__.py
--rw-r--r--   0        0        0    13964 2023-05-30 06:57:16.890915 cvxsimulator-0.3.6/cvx/simulator/builder.py
--rw-r--r--   0        0        0     1167 2023-05-30 06:57:16.890915 cvxsimulator-0.3.6/cvx/simulator/grid.py
--rw-r--r--   0        0        0     1163 2023-05-30 06:57:16.890915 cvxsimulator-0.3.6/cvx/simulator/metrics.py
--rw-r--r--   0        0        0     1422 2023-05-30 06:57:16.890915 cvxsimulator-0.3.6/cvx/simulator/month.py
--rw-r--r--   0        0        0    18895 2023-05-30 06:57:16.890915 cvxsimulator-0.3.6/cvx/simulator/portfolio.py
--rw-r--r--   0        0        0      514 2023-05-30 06:57:16.890915 cvxsimulator-0.3.6/cvx/simulator/trading_costs.py
--rw-r--r--   0        0        0      608 2023-05-30 06:57:55.683097 cvxsimulator-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     5627 1970-01-01 00:00:00.000000 cvxsimulator-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0    11375 2023-05-30 15:25:14.769701 cvxsimulator-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5064 2023-05-30 15:25:14.769701 cvxsimulator-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-30 15:25:14.845701 cvxsimulator-0.4.0/cvx/simulator/__init__.py
+-rw-r--r--   0        0        0    14005 2023-05-30 15:25:14.845701 cvxsimulator-0.4.0/cvx/simulator/builder.py
+-rw-r--r--   0        0        0     1552 2023-05-30 15:25:14.845701 cvxsimulator-0.4.0/cvx/simulator/grid.py
+-rw-r--r--   0        0        0     1163 2023-05-30 15:25:14.845701 cvxsimulator-0.4.0/cvx/simulator/metrics.py
+-rw-r--r--   0        0        0     1422 2023-05-30 15:25:14.845701 cvxsimulator-0.4.0/cvx/simulator/month.py
+-rw-r--r--   0        0        0    17965 2023-05-30 15:25:14.845701 cvxsimulator-0.4.0/cvx/simulator/portfolio.py
+-rw-r--r--   0        0        0      514 2023-05-30 15:25:14.845701 cvxsimulator-0.4.0/cvx/simulator/trading_costs.py
+-rw-r--r--   0        0        0      608 2023-05-30 15:25:39.242008 cvxsimulator-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5651 1970-01-01 00:00:00.000000 cvxsimulator-0.4.0/PKG-INFO
```

### Comparing `cvxsimulator-0.3.6/LICENSE` & `cvxsimulator-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.3.6/README.md` & `cvxsimulator-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # [cvxsimulator](http://www.cvxgrp.org/simulator/)
 
 [![PyPI version](https://badge.fury.io/py/cvxsimulator.svg)](https://badge.fury.io/py/cvxsimulator)
 [![Apache 2.0 License](https://img.shields.io/badge/License-APACHEv2-brightgreen.svg)](https://github.com/cvxgrp/simulator/blob/master/LICENSE)
 [![PyPI download month](https://img.shields.io/pypi/dm/cvxsimulator.svg)](https://pypi.python.org/pypi/cvxsimulator/)
-[![Coverage Status](https://coveralls.io/repos/github/cvxgrp/simulator/badge.svg)](https://coveralls.io/github/cvxgrp/simulator)
+[![Coverage Status](https://coveralls.io/repos/github/cvxgrp/simulator/badge.png?branch=main)](https://coveralls.io/github/cvxgrp/simulator?branch=main)
 
 Given a universe of $m$ assets we are given prices for each of them at time $t_1, t_2, \ldots t_n$, 
 e.g. we operate using an $n \times m$ matrix where each column corresponds to a particular asset.
 
 In a backtest we iterate in time (e.g. row by row) through the matrix and allocate positions to all or some of the assets.
 This tool shall help to simplify the accounting. It keeps track of the available cash, the profits achieved, etc.
```

### Comparing `cvxsimulator-0.3.6/cvx/simulator/builder.py` & `cvxsimulator-0.4.0/cvx/simulator/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,17 +128,18 @@
         position: the new position of the portfolio.
         cash: the new amount of cash in the portfolio after any trades and trading costs are applied.
 
         Note that the method does not return any value: instead,
         it updates the internal state of the _State instance.
         """
         if self.position is None:
-            trades = position
-        else:
-            trades = position - self.position
+            self.position = 0.0 * position
+            #trades = position
+        #else:
+        trades = position - self.position
 
         self.position = position
         self.cash -= (trades * self.prices).sum()
 
         if model is not None:
             self.cash -= model.eval(self.prices,  trades=trades, **kwargs).sum()
```

### Comparing `cvxsimulator-0.3.6/cvx/simulator/grid.py` & `cvxsimulator-0.4.0/cvx/simulator/grid.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,22 @@
 import pandas as pd
 import numpy as np
 
+def iron_frame(frame, rule):
+    """
+    The iron_frame function takes a pandas DataFrame
+    and keeps it constant on a coarser grid.
+
+    :param frame: The frame to be ironed
+    :param rule: The rule to be used for the construction of the grid
+    :return: the ironed frame
+    """
+    s_index = resample_index(frame.index, rule)
+    return _project_frame_to_grid(frame, s_index)
+
 
 def resample_index(index, rule):
     """
     The resample_index function resamples a pandas DatetimeIndex object
     to a lower frequency using a specified rule.
 
 
@@ -12,15 +24,15 @@
     but rather returns a pandas DatetimeIndex
     """
     series = pd.Series(index=index, data=index)
     a = series.resample(rule=rule).first()
     return pd.DatetimeIndex(a.values)
 
 
-def project_frame_to_grid(frame, grid):
+def _project_frame_to_grid(frame, grid):
     """
     The project_frame_to_grid function projects a pandas DataFrame
     to a coarser grid while still sharing the same index.
     It does that by taking over values of the frame from the coarser
     grid that are then forward filled.
     An application would be monthly rebalancing of a portfolio.
     E.g. on days in a particular grid we adjust the position and keep
```

### Comparing `cvxsimulator-0.3.6/cvx/simulator/metrics.py` & `cvxsimulator-0.4.0/cvx/simulator/metrics.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.3.6/cvx/simulator/month.py` & `cvxsimulator-0.4.0/cvx/simulator/month.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.3.6/cvx/simulator/portfolio.py` & `cvxsimulator-0.4.0/cvx/simulator/portfolio.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 
 import pandas as pd
 
-from cvx.simulator.grid import resample_index, project_frame_to_grid
+from cvx.simulator.grid import iron_frame
 from cvx.simulator.trading_costs import TradingCostModel
 
 
 def diff(portfolio1, portfolio2, initial_cash=1e6, trading_cost_model=None):
     # check both portfolios are on the same price grid
     pd.testing.assert_frame_equal(portfolio1.prices, portfolio2.prices)
 
@@ -297,16 +297,16 @@
 
         Returns: EquityPortfolio: A new EquityPortfolio object multiplied by the scalar constant.
 
         Notes: The rmul method allows multiplication of a scalar
         constant with an EquityPortfolio object in a reversed order"""
         return self.__mul__(scalar)
 
-    def __sub__(self, other):
-        return self.__add__(-1 * other)
+    # def __sub__(self, other):
+    #     return self.__add__(-1 * other)
 
     def __add__(self, port_new):
         assert isinstance(port_new, EquityPortfolio)
 
         assets = self.assets.union(port_new.assets)
         index = self.index.union(port_new.index)
 
@@ -352,46 +352,29 @@
         :return:
         """
         return EquityPortfolio(prices=self.prices.truncate(before=before, after=after),
                                stocks=self.stocks.truncate(before=before, after=after),
                                trading_cost_model=self.trading_cost_model,
                                initial_cash=self.nav.truncate(before=before, after=after).values[0])
 
-    @property
-    def start(self):
-        """first index with a profit that is not zero"""
-        return self.profit.ne(0).idxmax()
+    # @property
+    # def start(self):
+    #     """first index with a profit that is not zero"""
+    #     return self.profit.ne(0).idxmax()
 
-    def resample(self, rule, truncate=False):
+    def resample(self, rule):
         """The resample method resamples an EquityPortfolio object to a new frequency
         specified by the rule argument.
-        The method returns a new EquityPortfolio object with the resampled stocks, but prices stay the same.
-
-        If the truncate parameter is set to True, the method first trims the original data
-        to start from the beginning of the EquityPortfolio object's timeline using the truncate method.
-        Otherwise, the original EquityPortfolio timescale is used. The start of trading may be missed
-        as the first point may not be in the resampled grid.
-
-        The function uses a utility function resample_index to create a new DatetimeIndex
-        with the specified resampled rule. The new index is used in the project_frame_to_grid
-        function to translate the stocks DataFrame onto the new grid.
-
-        Finally, a new EquityPortfolio object is created with the original prices
+        A new EquityPortfolio object is created with the original prices
         DataFrame and the resampled stocks DataFrame. The objects trading cost model and initial cash value
         are also copied into the new object.
 
         Note that the resample method does not modify the original EquityPortfolio object,
         but rather returns a new object.
         """
-        if truncate:
-            portfolio = self.truncate(before=self.start)
-        else:
-            portfolio = self
-
-        grid = resample_index(portfolio.index, rule=rule)
-
-        stocks = project_frame_to_grid(portfolio.stocks, grid=grid)
+        # iron out the stocks index
+        stocks = iron_frame(self.stocks, rule=rule)
 
-        return EquityPortfolio(prices=portfolio.prices,
+        return EquityPortfolio(prices=self.prices,
                                stocks=stocks,
                                trading_cost_model=self.trading_cost_model,
                                initial_cash=self.initial_cash)
```

### Comparing `cvxsimulator-0.3.6/cvx/simulator/trading_costs.py` & `cvxsimulator-0.4.0/cvx/simulator/trading_costs.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.3.6/pyproject.toml` & `cvxsimulator-0.4.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cvxsimulator"
-version = "v0.3.6"
+version = "v0.4.0"
 description = "Simple simulator for investors"
 authors = ["Thomas Schmelzer"]
 readme = "README.md"
 repository = "https://github.com/cvxgrp/simulator"
 packages = [{include = "cvx"}]
 
 [tool.poetry.dependencies]
```

### Comparing `cvxsimulator-0.3.6/PKG-INFO` & `cvxsimulator-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxsimulator
-Version: 0.3.6
+Version: 0.4.0
 Summary: Simple simulator for investors
 Home-page: https://github.com/cvxgrp/simulator
 Author: Thomas Schmelzer
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -16,15 +16,15 @@
 Description-Content-Type: text/markdown
 
 # [cvxsimulator](http://www.cvxgrp.org/simulator/)
 
 [![PyPI version](https://badge.fury.io/py/cvxsimulator.svg)](https://badge.fury.io/py/cvxsimulator)
 [![Apache 2.0 License](https://img.shields.io/badge/License-APACHEv2-brightgreen.svg)](https://github.com/cvxgrp/simulator/blob/master/LICENSE)
 [![PyPI download month](https://img.shields.io/pypi/dm/cvxsimulator.svg)](https://pypi.python.org/pypi/cvxsimulator/)
-[![Coverage Status](https://coveralls.io/repos/github/cvxgrp/simulator/badge.svg)](https://coveralls.io/github/cvxgrp/simulator)
+[![Coverage Status](https://coveralls.io/repos/github/cvxgrp/simulator/badge.png?branch=main)](https://coveralls.io/github/cvxgrp/simulator?branch=main)
 
 Given a universe of $m$ assets we are given prices for each of them at time $t_1, t_2, \ldots t_n$, 
 e.g. we operate using an $n \times m$ matrix where each column corresponds to a particular asset.
 
 In a backtest we iterate in time (e.g. row by row) through the matrix and allocate positions to all or some of the assets.
 This tool shall help to simplify the accounting. It keeps track of the available cash, the profits achieved, etc.
```

