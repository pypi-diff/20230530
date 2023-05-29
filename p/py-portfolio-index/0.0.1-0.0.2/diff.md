# Comparing `tmp/py-portfolio-index-0.0.1.tar.gz` & `tmp/py-portfolio-index-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-portfolio-index-0.0.1.tar", last modified: Mon May 29 21:44:43 2023, max compression
+gzip compressed data, was "py-portfolio-index-0.0.2.tar", last modified: Mon May 29 23:13:55 2023, max compression
```

## Comparing `py-portfolio-index-0.0.1.tar` & `py-portfolio-index-0.0.2.tar`

### file list

```diff
@@ -1,54 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 21:44:43.561515 py-portfolio-index-0.0.1/
--rw-rw-rw-   0        0        0     1075 2023-05-22 23:55:53.000000 py-portfolio-index-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     6008 2023-05-29 21:44:43.561515 py-portfolio-index-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5366 2023-05-22 23:55:53.000000 py-portfolio-index-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 21:44:43.476000 py-portfolio-index-0.0.1/py_portfolio_index/
--rw-rw-rw-   0        0        0      663 2023-05-29 21:30:30.000000 py-portfolio-index-0.0.1/py_portfolio_index/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 21:44:43.491626 py-portfolio-index-0.0.1/py_portfolio_index/bin/
--rw-rw-rw-   0        0        0       60 2023-05-22 23:55:53.000000 py-portfolio-index-0.0.1/py_portfolio_index/bin/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 21:44:43.512665 py-portfolio-index-0.0.1/py_portfolio_index/bin/indexes/
--rw-rw-rw-   0        0        0       67 2023-05-22 23:55:53.000000 py-portfolio-index-0.0.1/py_portfolio_index/bin/indexes/__init__.py
--rw-rw-rw-   0        0        0    22537 2023-05-22 23:55:53.000000 py-portfolio-index-0.0.1/py_portfolio_index/bin/indexes/esgv_2020_q4.csv
--rw-rw-rw-   0        0        0     7503 2023-05-22 23:55:53.000000 py-portfolio-index-0.0.1/py_portfolio_index/bin/indexes/esgv_2021_q4.csv
--rw-rw-rw-   0        0        0     7529 2023-05-22 23:55:53.000000 py-portfolio-index-0.0.1/py_portfolio_index/bin/indexes/esgv_2022_q2.csv
--rw-rw-rw-   0        0        0     7526 2023-05-22 23:55:53.000000 py-portfolio-index-0.0.1/py_portfolio_index/bin/indexes/esgv_2022_q3.csv
--rw-rw-rw-   0        0        0     7481 2023-05-22 23:55:53.000000 py-portfolio-index-0.0.1/py_portfolio_index/bin/indexes/esgv_2022_q4.csv
--rw-rw-rw-   0        0        0     7400 2023-05-22 23:55:53.000000 py-portfolio-index-0.0.1/py_portfolio_index/bin/indexes/esgv_2023_q1.csv
--rw-rw-rw-   0        0        0     1741 2023-05-22 23:55:53.000000 py-portfolio-index-0.0.1/py_portfolio_index/bin/indexes/inventory.py
--rw-rw-rw-   0        0        0      668 2023-05-22 23:55:53.000000 py-portfolio-index-0.0.1/py_portfolio_index/bin/indexes/qcln_2020_q4.csv
--rw-rw-rw-   0        0        0    55272 2023-05-22 23:55:53.000000 py-portfolio-index-0.0.1/py_portfolio_index/bin/indexes/vtsmx_2020_q4.csv
-drwxrwxrwx   0        0        0        0 2023-05-29 21:44:43.547982 py-portfolio-index-0.0.1/py_portfolio_index/bin/lists/
--rw-rw-rw-   0        0        0       79 2023-05-22 23:55:53.000000 py-portfolio-index-0.0.1/py_portfolio_index/bin/lists/__init__.py
--rw-rw-rw-   0        0        0       81 2023-05-22 23:55:53.000000 py-portfolio-index-0.0.1/py_portfolio_index/bin/lists/coal.csv
--rw-rw-rw-   0        0        0       39 2023-05-22 23:55:53.000000 py-portfolio-index-0.0.1/py_portfolio_index/bin/lists/cruises.csv
--rw-rw-rw-   0        0        0       27 2023-05-22 23:55:53.000000 py-portfolio-index-0.0.1/py_portfolio_index/bin/lists/fake_meat.csv
--rw-rw-rw-   0        0        0     1176 2023-05-22 23:55:53.000000 py-portfolio-index-0.0.1/py_portfolio_index/bin/lists/inventory.py
--rw-rw-rw-   0        0        0       25 2023-05-22 23:55:53.000000 py-portfolio-index-0.0.1/py_portfolio_index/bin/lists/meat_poultry.csv
--rw-rw-rw-   0        0        0       24 2023-05-22 23:55:53.000000 py-portfolio-index-0.0.1/py_portfolio_index/bin/lists/non_ethical_conduct.csv
--rw-rw-rw-   0        0        0      519 2023-05-22 23:55:53.000000 py-portfolio-index-0.0.1/py_portfolio_index/bin/lists/oil.csv
--rw-rw-rw-   0        0        0      198 2023-05-22 23:55:53.000000 py-portfolio-index-0.0.1/py_portfolio_index/bin/lists/renewable.csv
--rw-rw-rw-   0        0        0      122 2023-05-22 23:55:53.000000 py-portfolio-index-0.0.1/py_portfolio_index/bin/lists/semiconductor.csv
--rw-rw-rw-   0        0        0       41 2023-05-22 23:55:53.000000 py-portfolio-index-0.0.1/py_portfolio_index/bin/lists/space.csv
--rw-rw-rw-   0        0        0       44 2023-05-22 23:55:53.000000 py-portfolio-index-0.0.1/py_portfolio_index/bin/lists/vice.csv
--rw-rw-rw-   0        0        0      408 2023-05-22 23:55:53.000000 py-portfolio-index-0.0.1/py_portfolio_index/common.py
--rw-rw-rw-   0        0        0      560 2023-05-29 21:40:21.000000 py-portfolio-index-0.0.1/py_portfolio_index/config.py
--rw-rw-rw-   0        0        0      100 2023-05-22 23:55:53.000000 py-portfolio-index-0.0.1/py_portfolio_index/constants.py
--rw-rw-rw-   0        0        0      353 2023-05-29 21:40:43.000000 py-portfolio-index-0.0.1/py_portfolio_index/enums.py
--rw-rw-rw-   0        0        0       43 2023-05-22 23:55:53.000000 py-portfolio-index-0.0.1/py_portfolio_index/exceptions.py
--rw-rw-rw-   0        0        0     8465 2023-05-22 23:55:53.000000 py-portfolio-index-0.0.1/py_portfolio_index/models.py
--rw-rw-rw-   0        0        0     3046 2023-05-24 01:47:42.000000 py-portfolio-index-0.0.1/py_portfolio_index/operators.py
-drwxrwxrwx   0        0        0        0 2023-05-29 21:44:43.561515 py-portfolio-index-0.0.1/py_portfolio_index/portfolio_providers/
--rw-rw-rw-   0        0        0        0 2023-05-22 23:55:53.000000 py-portfolio-index-0.0.1/py_portfolio_index/portfolio_providers/__init__.py
--rw-rw-rw-   0        0        0     3912 2023-05-24 01:43:20.000000 py-portfolio-index-0.0.1/py_portfolio_index/portfolio_providers/alpaca.py
--rw-rw-rw-   0        0        0     5637 2023-05-25 12:33:46.000000 py-portfolio-index-0.0.1/py_portfolio_index/portfolio_providers/alpaca_v2.py
--rw-rw-rw-   0        0        0     4844 2023-05-22 23:55:53.000000 py-portfolio-index-0.0.1/py_portfolio_index/portfolio_providers/base_portfolio.py
--rw-rw-rw-   0        0        0     1626 2023-05-22 23:55:53.000000 py-portfolio-index-0.0.1/py_portfolio_index/portfolio_providers/local_dict.py
--rw-rw-rw-   0        0        0     4224 2023-05-26 01:44:13.000000 py-portfolio-index-0.0.1/py_portfolio_index/portfolio_providers/robinhood.py
-drwxrwxrwx   0        0        0        0 2023-05-29 21:44:43.488593 py-portfolio-index-0.0.1/py_portfolio_index.egg-info/
--rw-rw-rw-   0        0        0     6008 2023-05-29 21:44:43.000000 py-portfolio-index-0.0.1/py_portfolio_index.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1811 2023-05-29 21:44:43.000000 py-portfolio-index-0.0.1/py_portfolio_index.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 21:44:43.000000 py-portfolio-index-0.0.1/py_portfolio_index.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-05-29 21:44:43.000000 py-portfolio-index-0.0.1/py_portfolio_index.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-29 21:44:43.000000 py-portfolio-index-0.0.1/py_portfolio_index.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 21:44:43.561515 py-portfolio-index-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1547 2023-05-29 21:44:38.000000 py-portfolio-index-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:13:55.163130 py-portfolio-index-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-05-29 23:13:55.163130 py-portfolio-index-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:13:55.163130 py-portfolio-index-0.0.2/py_portfolio_index/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:13:55.163130 py-portfolio-index-0.0.2/py_portfolio_index/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:13:55.163130 py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22537 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/esgv_2020_q4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/esgv_2021_q4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/esgv_2022_q2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/esgv_2022_q3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/esgv_2022_q4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7400 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/esgv_2023_q1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/qcln_2020_q4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    55272 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/vtsmx_2020_q4.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:13:55.163130 py-portfolio-index-0.0.2/py_portfolio_index/bin/lists/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/lists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/lists/coal.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/lists/cruises.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/lists/fake_meat.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/lists/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/lists/meat_poultry.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/lists/non_ethical_conduct.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/lists/oil.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/lists/renewable.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/lists/semiconductor.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/lists/space.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/bin/lists/vice.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:13:55.163130 py-portfolio-index-0.0.2/py_portfolio_index/portfolio_providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/portfolio_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/portfolio_providers/alpaca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/portfolio_providers/alpaca_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/portfolio_providers/base_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/portfolio_providers/local_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/portfolio_providers/robinhood.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/py_portfolio_index/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 23:13:55.163130 py-portfolio-index-0.0.2/py_portfolio_index.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-05-29 23:13:55.000000 py-portfolio-index-0.0.2/py_portfolio_index.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-29 23:13:55.000000 py-portfolio-index-0.0.2/py_portfolio_index.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 23:13:55.000000 py-portfolio-index-0.0.2/py_portfolio_index.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-29 23:13:55.000000 py-portfolio-index-0.0.2/py_portfolio_index.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-29 23:13:55.000000 py-portfolio-index-0.0.2/py_portfolio_index.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 23:13:55.163130 py-portfolio-index-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-29 23:13:42.000000 py-portfolio-index-0.0.2/setup.py
```

### Comparing `py-portfolio-index-0.0.1/LICENSE.txt` & `py-portfolio-index-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.1/PKG-INFO` & `py-portfolio-index-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,167 +1,167 @@
-Metadata-Version: 2.1
-Name: py-portfolio-index
-Version: 0.0.1
-Summary: Build index portfolios.
-Home-page: 
-Author: 
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-Provides-Extra: alpaca
-Provides-Extra: robinhood
-License-File: LICENSE.txt
-
-## Py Portfolio Index
-
-`py-portfolio-index` is a python library to make it easier to mantain a broad, index-based approach to stock investing
-while following individual ESG (Environmental, Social, and Governance) or SRI (Socially Response Investing) goals.
-
-To do that, it provides tools for constructing and managing portfolios that are modeled off indexes. These ideal
-portfolios can be efficiently converted into actual portfolios by API, using commission free platforms like Robinhood or
-Alpaca. Since constructing an index analogue typically requires many small stock purchases, a
-commission free platform is important to minimizing overhead. Robinhood has the additional benefit of allowing fractional
-share purchases, which allow an index to come closer to an ideal match with a smaller total portfolio size. 
-
-#### Install
-
-The package supports Python 3.7 plus.
-
-`pip install py-portfolio-index` [Not yet!]
-
-#### Considerations
-
-Some providers may take some time to place an order. Keep this in mind when running repeated rebalances, as the
-portfolio balance may not have updated to reflect your last order.
-
-#### Basic Example
-
-This example shows a basic example using the Alpaca API in paper trading mode.
-
-It constructs an ideal portfolio based on the composition of the Vanguard ESG index fund in Q4 2020, then uses the
-Alpaca API to construct a matching portfolio based on an initial investment of 10000 dollars.
-
-Since Alpaca doesn't support fractional shares, this portfolio will approximate an index, but cannot match it exactly, 
-especially for small total portfolio sizes.
-
-```python
-from py_portfolio_index import INDEXES, STOCK_LISTS, Logger, AlpacaProvider, PurchaseStrategy, compare_portfolios,
-
-AlpacaProvider
-
-from logging import INFO, StreamHandler
-
-Logger.addHandler(StreamHandler())
-Logger.setLevel(INFO)
-
-API_KEY = '#########'
-
-SECRET_KEY = '##########'
-
-# The size of our paper portfolio
-TARGET_PORTFOLIO_SIZE = 10000
-
-# instantiate the Alpaca provider with identity information
-# and set it to use the paper provider
-provider = AlpacaProvider(key_id=API_KEY, secret_key=SECRET_KEY, paper=True)
-
-# get an example index 
-# this one is the vanguard ESG index for Q4 202
-ideal_portfolio = INDEXES['esgv_2020_q4']
-
-# exclude all stocks from the oil, vice, and cruise lists
-ideal_portfolio.exclude(STOCK_LISTS['oil']).exclude(STOCK_LISTS['vice']).exclude(STOCK_LISTS['cruises'])
-
-# double the weighting of stocks in the renewable and semiconductor lists, and set them to a minimum weight of .1%
-ideal_portfolio.reweight(STOCK_LISTS['renewable'], weight=2.0, min_weight=.001)
-ideal_portfolio.reweight(STOCK_LISTS['semiconductor'], weight=2.0, min_weight=.001)
-
-# get actual holdings
-real_port = provider.get_holdings()
-
-# compare actual holdings to this ideal portfolio to produce a buy and sell list
-to_buy, to_sell = compare_portfolios(ideal=ideal_portfolio, real=real_port,
-                                     buy_order=PurchaseStrategy.LARGEST_DIFF_FIRST,
-                                     target_size=TARGET_PORTFOLIO_SIZE)
-
-# purchase the buy list
-provider.purchase_ticker_value_dict(to_buy, TARGET_PORTFOLIO_SIZE, fractional_shares=False, skip_errored_stocks=True)
-```
-
-### Robinhood
-
-Since robinhood supports fractional shares, it's much easier to get close to an index
-with a smaller amount of money. 
-
-
-```python
-from py_portfolio_index.bin import INDEXES, STOCK_LISTS
-from py_portfolio_index.enums import PurchaseStrategy
-from py_portfolio_index.operators import compare_portfolios
-from py_portfolio_index.portfolio_providers.robinhood import RobinhoodProvider
-from py_portfolio_index.constants import Logger
-
-from logging import INFO, StreamHandler
-Logger.addHandler(StreamHandler())
-Logger.setLevel(INFO)
-
-ideal_port = INDEXES['esgv_2020_q4']
-
-# create a stock list
-STOCK_LISTS.add_list('manual_override', ['MDLZ'])
-
-# modify the index
-ideal_port.exclude(STOCK_LISTS['oil']).exclude(STOCK_LISTS['vice']).exclude(STOCK_LISTS['cruises']).exclude(
-    STOCK_LISTS['manual_override'])
-
-# overweight on stonks
-ideal_port.reweight(STOCK_LISTS['renewable'], weight=2.0, min_weight=.001)
-ideal_port.reweight(STOCK_LISTS['semiconductor'], weight=2.0, min_weight=.001)
-
-provider = RobinhoodProvider(username='#####', password='#########')
-
-real_port = provider.get_holdings()
-
-TARGET_SIZE = 10000
-
-to_buy, to_sell = compare_portfolios(ideal=ideal_port, real=real_port, buy_order=PurchaseStrategy.CHEAPEST_FIRST,
-                                     target_size = TARGET_SIZE)
-
-
-provider.purchase_ticker_value_dict(to_buy, purchasing_power=1000, fractional_shares=True, skip_errored_stocks=True)
-
-```
-
-### Testing
-
-To avoid actually purchasing a stock, use the plan_only option to log what trades would have occurred.
-
-```python
-
-provider.purchase_ticker_value_dict(to_buy, TARGET_PORTFOLIO_SIZE, plan_only=True, fractional_shares=False,
-                                    skip_errored_stocks=True, )
-
-```
-
-### Example Scripts
-
-Can be found in the examples folder.
-
-### Logging
-
-To see messages, it's helpful to configure the logger to print messages. You can either configure the standard python
-logger or use the portfolio specific one using an example like the below.
-
-```python
-from py_portfolio_index.constants import Logger
-from logging import INFO, StreamHandler
-
-Logger.addHandler(StreamHandler())
-Logger.setLevel(INFO)
-
-```
-
-
-
+Metadata-Version: 2.1
+Name: py-portfolio-index
+Version: 0.0.2
+Summary: Build index portfolios.
+Home-page: 
+Author: 
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+Provides-Extra: alpaca
+Provides-Extra: robinhood
+License-File: LICENSE.txt
+
+## Py Portfolio Index
+
+`py-portfolio-index` is a python library to make it easier to mantain a broad, index-based approach to stock investing
+while following individual ESG (Environmental, Social, and Governance) or SRI (Socially Response Investing) goals.
+
+To do that, it provides tools for constructing and managing portfolios that are modeled off indexes. These ideal
+portfolios can be efficiently converted into actual portfolios by API, using commission free platforms like Robinhood or
+Alpaca. Since constructing an index analogue typically requires many small stock purchases, a
+commission free platform is important to minimizing overhead. Robinhood has the additional benefit of allowing fractional
+share purchases, which allow an index to come closer to an ideal match with a smaller total portfolio size. 
+
+#### Install
+
+The package supports Python 3.7 plus.
+
+`pip install py-portfolio-index` [Not yet!]
+
+#### Considerations
+
+Some providers may take some time to place an order. Keep this in mind when running repeated rebalances, as the
+portfolio balance may not have updated to reflect your last order.
+
+#### Basic Example
+
+This example shows a basic example using the Alpaca API in paper trading mode.
+
+It constructs an ideal portfolio based on the composition of the Vanguard ESG index fund in Q4 2020, then uses the
+Alpaca API to construct a matching portfolio based on an initial investment of 10000 dollars.
+
+Since Alpaca doesn't support fractional shares, this portfolio will approximate an index, but cannot match it exactly, 
+especially for small total portfolio sizes.
+
+```python
+from py_portfolio_index import INDEXES, STOCK_LISTS, Logger, AlpacaProvider, PurchaseStrategy, compare_portfolios,
+
+AlpacaProvider
+
+from logging import INFO, StreamHandler
+
+Logger.addHandler(StreamHandler())
+Logger.setLevel(INFO)
+
+API_KEY = '#########'
+
+SECRET_KEY = '##########'
+
+# The size of our paper portfolio
+TARGET_PORTFOLIO_SIZE = 10000
+
+# instantiate the Alpaca provider with identity information
+# and set it to use the paper provider
+provider = AlpacaProvider(key_id=API_KEY, secret_key=SECRET_KEY, paper=True)
+
+# get an example index 
+# this one is the vanguard ESG index for Q4 202
+ideal_portfolio = INDEXES['esgv_2020_q4']
+
+# exclude all stocks from the oil, vice, and cruise lists
+ideal_portfolio.exclude(STOCK_LISTS['oil']).exclude(STOCK_LISTS['vice']).exclude(STOCK_LISTS['cruises'])
+
+# double the weighting of stocks in the renewable and semiconductor lists, and set them to a minimum weight of .1%
+ideal_portfolio.reweight(STOCK_LISTS['renewable'], weight=2.0, min_weight=.001)
+ideal_portfolio.reweight(STOCK_LISTS['semiconductor'], weight=2.0, min_weight=.001)
+
+# get actual holdings
+real_port = provider.get_holdings()
+
+# compare actual holdings to this ideal portfolio to produce a buy and sell list
+to_buy, to_sell = compare_portfolios(ideal=ideal_portfolio, real=real_port,
+                                     buy_order=PurchaseStrategy.LARGEST_DIFF_FIRST,
+                                     target_size=TARGET_PORTFOLIO_SIZE)
+
+# purchase the buy list
+provider.purchase_ticker_value_dict(to_buy, TARGET_PORTFOLIO_SIZE, fractional_shares=False, skip_errored_stocks=True)
+```
+
+### Robinhood
+
+Since robinhood supports fractional shares, it's much easier to get close to an index
+with a smaller amount of money. 
+
+
+```python
+from py_portfolio_index.bin import INDEXES, STOCK_LISTS
+from py_portfolio_index.enums import PurchaseStrategy
+from py_portfolio_index.operators import compare_portfolios
+from py_portfolio_index.portfolio_providers.robinhood import RobinhoodProvider
+from py_portfolio_index.constants import Logger
+
+from logging import INFO, StreamHandler
+Logger.addHandler(StreamHandler())
+Logger.setLevel(INFO)
+
+ideal_port = INDEXES['esgv_2020_q4']
+
+# create a stock list
+STOCK_LISTS.add_list('manual_override', ['MDLZ'])
+
+# modify the index
+ideal_port.exclude(STOCK_LISTS['oil']).exclude(STOCK_LISTS['vice']).exclude(STOCK_LISTS['cruises']).exclude(
+    STOCK_LISTS['manual_override'])
+
+# overweight on stonks
+ideal_port.reweight(STOCK_LISTS['renewable'], weight=2.0, min_weight=.001)
+ideal_port.reweight(STOCK_LISTS['semiconductor'], weight=2.0, min_weight=.001)
+
+provider = RobinhoodProvider(username='#####', password='#########')
+
+real_port = provider.get_holdings()
+
+TARGET_SIZE = 10000
+
+to_buy, to_sell = compare_portfolios(ideal=ideal_port, real=real_port, buy_order=PurchaseStrategy.CHEAPEST_FIRST,
+                                     target_size = TARGET_SIZE)
+
+
+provider.purchase_ticker_value_dict(to_buy, purchasing_power=1000, fractional_shares=True, skip_errored_stocks=True)
+
+```
+
+### Testing
+
+To avoid actually purchasing a stock, use the plan_only option to log what trades would have occurred.
+
+```python
+
+provider.purchase_ticker_value_dict(to_buy, TARGET_PORTFOLIO_SIZE, plan_only=True, fractional_shares=False,
+                                    skip_errored_stocks=True, )
+
+```
+
+### Example Scripts
+
+Can be found in the examples folder.
+
+### Logging
+
+To see messages, it's helpful to configure the logger to print messages. You can either configure the standard python
+logger or use the portfolio specific one using an example like the below.
+
+```python
+from py_portfolio_index.constants import Logger
+from logging import INFO, StreamHandler
+
+Logger.addHandler(StreamHandler())
+Logger.setLevel(INFO)
+
+```
+
+
+
```

### Comparing `py-portfolio-index-0.0.1/README.md` & `py-portfolio-index-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.1/py_portfolio_index/__init__.py` & `py-portfolio-index-0.0.2/py_portfolio_index/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from py_portfolio_index.bin import INDEXES, STOCK_LISTS
 from py_portfolio_index.constants import Logger
 from py_portfolio_index.enums import PurchaseStrategy
 from py_portfolio_index.operators import compare_portfolios
 from py_portfolio_index.portfolio_providers.alpaca import AlpacaProviderLegacy
 from py_portfolio_index.portfolio_providers.robinhood import RobinhoodProvider
 from py_portfolio_index.portfolio_providers.alpaca_v2 import AlpacaProvider
+from py_portfolio_index.config import get_providers
 
-__version__ = "0.0.1"
+AVAILABLE_PROVIDERS = get_providers()
+
+__version__ = "0.0.2"
 
 __all__ = [
     "INDEXES",
     "STOCK_LISTS",
     "Logger",
     "compare_portfolios",
     "AlpacaProvider",
```

### Comparing `py-portfolio-index-0.0.1/py_portfolio_index/bin/indexes/esgv_2020_q4.csv` & `py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/esgv_2020_q4.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.1/py_portfolio_index/bin/indexes/esgv_2021_q4.csv` & `py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/esgv_2021_q4.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.1/py_portfolio_index/bin/indexes/esgv_2022_q2.csv` & `py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/esgv_2022_q2.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.1/py_portfolio_index/bin/indexes/esgv_2022_q3.csv` & `py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/esgv_2022_q3.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.1/py_portfolio_index/bin/indexes/esgv_2022_q4.csv` & `py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/esgv_2022_q4.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.1/py_portfolio_index/bin/indexes/esgv_2023_q1.csv` & `py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/esgv_2023_q1.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.1/py_portfolio_index/bin/indexes/inventory.py` & `py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/inventory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from os import listdir
 from os.path import dirname, join
 from typing import List
 import re
 from datetime import date
+from decimal import Decimal 
 
 from py_portfolio_index.models import IdealPortfolioElement, IdealPortfolio
 
 QUARTER_TO_MONTH = {1: 1, 2: 4, 3: 7, 4: 10}
 
 
-def parse_date_from_name(input: str):
+def parse_date_from_name(input: str)-> date | None:
     components = input.lower().split("_")
     year = None
     quarter = None
     for item in components:
         if re.match("[0-9]{4}", item):
             year = int(item)
         if re.match("q[1-4]", item):
@@ -43,12 +44,12 @@
 
     def get_values(self, item: str) -> IdealPortfolio:
         out = []
         with open(join(dirname(__file__), f"{item}.csv")) as f:
             contents = f.read()
             for row in contents.split("\n"):
                 ticker, weight = row.split(",", 1)
-                out.append(IdealPortfolioElement(ticker=ticker, weight=float(weight)))
+                out.append(IdealPortfolioElement(ticker=ticker, weight=Decimal(weight)))
         start_date = parse_date_from_name(item)
         if start_date:
             return IdealPortfolio(holdings=out, source_date=start_date)
         return IdealPortfolio(holdings=out)
```

### Comparing `py-portfolio-index-0.0.1/py_portfolio_index/bin/indexes/qcln_2020_q4.csv` & `py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/qcln_2020_q4.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.1/py_portfolio_index/bin/indexes/vtsmx_2020_q4.csv` & `py-portfolio-index-0.0.2/py_portfolio_index/bin/indexes/vtsmx_2020_q4.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.1/py_portfolio_index/bin/lists/inventory.py` & `py-portfolio-index-0.0.2/py_portfolio_index/bin/lists/inventory.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.1/py_portfolio_index/bin/lists/oil.csv` & `py-portfolio-index-0.0.2/py_portfolio_index/bin/lists/oil.csv`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.1/py_portfolio_index/config.py` & `py-portfolio-index-0.0.2/py_portfolio_index/config.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.1/py_portfolio_index/models.py` & `py-portfolio-index-0.0.2/py_portfolio_index/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-from dataclasses import dataclass
 from datetime import datetime, date
-from typing import List, Optional, Union, Sequence, Iterable
+from typing import List, Optional, Union, TYPE_CHECKING
 from pydantic import BaseModel, Field, validator
 from pandas import DataFrame
 from py_portfolio_index.enums import Currency
 from py_portfolio_index.constants import Logger
 from py_portfolio_index.exceptions import PriceFetchError
 from decimal import Decimal
-from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from py_portfolio_index.portfolio_providers.base_portfolio import BaseProvider
 
 
 class Money(BaseModel):
-    value: Decimal
+    value: Union[Decimal, int, float, "Money"]
     currency: Currency = Currency.USD
 
     @validator("value", pre=True)
     def coerce_to_decimal(cls, v):
         if isinstance(v, int):
             return Decimal(v)
         if isinstance(v, Money):
+            # TODO convert this
             return Decimal(v.value)
         return v
 
     def __str__(self):
         return f"{self.currency.value}{self.value}"
 
     def __repr__(self):
@@ -37,15 +36,14 @@
 
         currency = Config.default_currency
         if isinstance(val, Money):
             return val
         elif isinstance(val, (Decimal, float, int)):
             return Money(value=Decimal(val), currency=currency)
         elif isinstance(val, str):
-
             for c in Currency:
                 if c.name in val:
                     val = val.replace(c.name, "")
                     currency = c
             return Money(value=Decimal(val), currency=currency)
         raise ValueError(f"Invalid input to Money type {type(val)} {val}")
 
@@ -71,27 +69,27 @@
     def __lt__(self, other):
         return self.value < self._cmp_helper(other)
 
     def __le__(self, other):
         return self.value <= self._cmp_helper(other)
 
     # sum starts with 0
-    def __radd__(self, other):
+    def __radd__(self, other) -> "Money":
         if other == 0:
             return self
         else:
             return self.__add__(other)
 
-    def __add__(self, other):
+    def __add__(self, other) -> "Money":
         return Money(value=self.value + self._cmp_helper(other), currency=self.currency)
 
-    def __sub__(self, other):
+    def __sub__(self, other) -> "Money":
         return Money(value=self.value - self._cmp_helper(other), currency=self.currency)
 
-    def __mul__(self, other):
+    def __mul__(self, other) -> "Money":
         return Money(value=self.value * self._cmp_helper(other), currency=self.currency)
 
     def __truediv__(self, other):
         return Money(value=self.value / self._cmp_helper(other), currency=self.currency)
 
     def __float__(self):
         return float(self.value)
@@ -218,26 +216,27 @@
 
     @validator("value", pre=True)
     def value_coercion(cls, v) -> Money:
         return Money.parse(v)
 
 
 class RealPortfolio(IdealPortfolio):
-    holdings: List[RealPortfolioElement]
+    holdings: List[RealPortfolioElement]  # type: ignore
 
     @property
     def _index(self):
         return {val.ticker: val for val in self.holdings}
 
     def get_holding(self, ticker: str):
         return self._index.get(ticker)
 
     @property
     def value(self) -> Money:
-        return Money(value=sum([item.value for item in self.holdings]))
+        values: List[Money] = [item.value for item in self.holdings]
+        return Money(value=sum(values))
 
     def _reweight_portfolio(self):
         value = self.value
         for item in self.holdings:
             item.weight = Decimal(item.value / value.value)
 
     def add_holding(self, holding: RealPortfolioElement):
```

### Comparing `py-portfolio-index-0.0.1/py_portfolio_index/operators.py` & `py-portfolio-index-0.0.2/py_portfolio_index/operators.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.1/py_portfolio_index/portfolio_providers/alpaca.py` & `py-portfolio-index-0.0.2/py_portfolio_index/portfolio_providers/alpaca.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,18 +64,17 @@
                     end=end.isoformat(),
                 )
                 # take the first day after target day
                 return Decimal(raw[0].h)
             return Decimal(raw.ap)
 
     def buy_instrument(self, ticker: str, qty: Decimal):
-        import alpaca_trade_api as tradeapi
 
         qty_float = float(qty)
-        order = self.api.submit_order(
+        self.api.submit_order(
             symbol=ticker,
             qty=qty_float,
             side="buy",
             type="market",
             time_in_force="day",
         )
         return True
```

### Comparing `py-portfolio-index-0.0.1/py_portfolio_index/portfolio_providers/alpaca_v2.py` & `py-portfolio-index-0.0.2/py_portfolio_index/portfolio_providers/alpaca_v2.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,140 +1,137 @@
-from py_portfolio_index.models import RealPortfolio, RealPortfolioElement
-from .base_portfolio import BaseProvider
-from decimal import Decimal
-from typing import Optional
-from datetime import date, datetime, timezone, timedelta
-from functools import lru_cache
-
-from os import environ
-
-
-class AlpacaProvider(BaseProvider):
-    def __init__(
-        self,
-        key_id: str | None = None,
-        secret_key: str | None = None,
-        paper: bool = False,
-    ):
-        from alpaca.trading.client import TradingClient
-        from alpaca.data.historical import StockHistoricalDataClient
-
-        if not key_id:
-            key_id = environ.get("ALPACA_API_KEY", None)
-        if not secret_key:
-            secret_key = environ.get("ALPACA_API_SECRET", None)
-        if not (key_id and secret_key):
-            raise ValueError(
-                "Must provide key_id and secret_key or set environment variables ALPACA_API_KEY and ALPACA_API_SECRET "
-            )
-        self.trading_client = TradingClient(
-            api_key=key_id, secret_key=secret_key, paper=False
-        )
-        self.historical_client = StockHistoricalDataClient(
-            api_key=key_id, secret_key=secret_key
-        )
-        # tradeapi.REST(
-        #     key_id=key_id, secret_key=secret_key, base_url=URL(TARGET_URL)
-        # )
-        BaseProvider.__init__(self)
-
-    @lru_cache(maxsize=None)
-    def _get_instrument_price(
-        self, ticker: str, at_day: Optional[date] = None
-    ) -> Optional[Decimal]:
-        from alpaca.data.timeframe import TimeFrame, TimeFrameUnit
-        from alpaca.data.requests import StockBarsRequest, StockLatestQuoteRequest
-
-        if at_day:
-            start = datetime(at_day.year, at_day.month, at_day.day, tzinfo=timezone.utc)
-            end = start + timedelta(days=7)
-            # end = datetime(at_day.year, at_day.month, at_day.day+7, hour=23, tzinfo=timezone.utc)
-            raw = self.historical_client.get_stock_bars(
-                StockBarsRequest(
-                    symbol_or_symbols=ticker,
-                    start=start,
-                    end=end,
-                    timeframe=TimeFrame(amount=1, unit=TimeFrameUnit.Day),
-                    limit=100,
-                    adjustment=None,
-                    feed=None,
-                )
-                # [ticker],
-                # timeframe=TimeFrame(amount=1, unit=TimeFrameUnit.Day),
-                # start=start.isoformat(),
-                # end=end.isoformat(),
-            )
-            # take the first day after target day
-            return Decimal(raw[ticker][0].high)
-        else:
-            raw = self.historical_client.get_stock_latest_quote(
-                StockLatestQuoteRequest(symbol_or_symbols=ticker, feed=None)
-            )
-            # if we don't have a value for the current day
-            # expand out
-            # this is requuired on weekends
-            if not raw[ticker].ask_price:
-                default = datetime.now(tz=timezone.utc) - timedelta(hours=1)
-                start = default - timedelta(days=7)
-                end = default
-                raw = self.historical_client.get_stock_bars(
-                    StockBarsRequest(
-                        symbol_or_symbols=ticker,
-                        start=start,
-                        end=end,
-                        timeframe=TimeFrame(amount=1, unit=TimeFrameUnit.Day),
-                        feed=None,
-                        adjustment=None,
-                        limit=1000,
-                    )
-                    # [ticker],
-                    # timeframe=TimeFrame(amount=1, unit=TimeFrameUnit.Day),
-                    # start=start.isoformat(),
-                    # end=end.isoformat(),
-                )
-                # take the first day after target day
-                return Decimal(raw[ticker][0].high)
-            return Decimal(raw[ticker].ask_price)
-
-    def buy_instrument(self, ticker: str, qty: Decimal):
-        from alpaca.trading.client import TradingClient
-        from alpaca.trading.requests import MarketOrderRequest
-        from alpaca.trading.enums import OrderSide, TimeInForce
-
-        market_order_data = MarketOrderRequest(
-            symbol=ticker,
-            qty=float(qty),
-            side=OrderSide.BUY,
-            time_in_force=TimeInForce.DAY,
-        )
-        market_order = self.trading_client.submit_order(order_data=market_order_data)
-
-        return True
-
-    def get_unsettled_instruments(self):
-        from alpaca.trading.client import TradingClient
-        from alpaca.trading.requests import GetOrdersRequest, QueryOrderStatus
-        from alpaca.trading.enums import OrderSide, TimeInForce
-
-        open_orders = self.trading_client.get_orders(
-            filter=GetOrdersRequest(status=QueryOrderStatus.OPEN)
-        )
-        return set([o.symbol for o in open_orders])
-
-    def get_holdings(self):
-        from decimal import Decimal
-
-        my_stocks = self.trading_client.get_all_positions()
-        # df = pd.DataFrame(my_stocks)
-        if not my_stocks:
-            return RealPortfolio(holdings=[])
-        total_value = sum([Decimal(item.market_value) for item in my_stocks])
-        out = [
-            RealPortfolioElement(
-                ticker=row.symbol,
-                units=row.qty,
-                value=Decimal(row.market_value),
-                weight=Decimal(row.market_value) / total_value,
-            )
-            for row in my_stocks
-        ]
-        return RealPortfolio(holdings=out)
+from py_portfolio_index.models import RealPortfolio, RealPortfolioElement
+from .base_portfolio import BaseProvider
+from decimal import Decimal
+from typing import Optional
+from datetime import date, datetime, timezone, timedelta
+from functools import lru_cache
+
+from os import environ
+
+
+class AlpacaProvider(BaseProvider):
+    def __init__(
+        self,
+        key_id: str | None = None,
+        secret_key: str | None = None,
+        paper: bool = False,
+    ):
+        from alpaca.trading.client import TradingClient
+        from alpaca.data.historical import StockHistoricalDataClient
+
+        if not key_id:
+            key_id = environ.get("ALPACA_API_KEY", None)
+        if not secret_key:
+            secret_key = environ.get("ALPACA_API_SECRET", None)
+        if not (key_id and secret_key):
+            raise ValueError(
+                "Must provide key_id and secret_key or set environment variables ALPACA_API_KEY and ALPACA_API_SECRET "
+            )
+        self.trading_client = TradingClient(
+            api_key=key_id, secret_key=secret_key, paper=False
+        )
+        self.historical_client = StockHistoricalDataClient(
+            api_key=key_id, secret_key=secret_key
+        )
+        # tradeapi.REST(
+        #     key_id=key_id, secret_key=secret_key, base_url=URL(TARGET_URL)
+        # )
+        BaseProvider.__init__(self)
+
+    @lru_cache(maxsize=None)
+    def _get_instrument_price(
+        self, ticker: str, at_day: Optional[date] = None
+    ) -> Optional[Decimal]:
+        from alpaca.data.timeframe import TimeFrame, TimeFrameUnit
+        from alpaca.data.requests import StockBarsRequest, StockLatestQuoteRequest
+
+        if at_day:
+            start = datetime(at_day.year, at_day.month, at_day.day, tzinfo=timezone.utc)
+            end = start + timedelta(days=7)
+            # end = datetime(at_day.year, at_day.month, at_day.day+7, hour=23, tzinfo=timezone.utc)
+            raw = self.historical_client.get_stock_bars(
+                StockBarsRequest(
+                    symbol_or_symbols=ticker,
+                    start=start,
+                    end=end,
+                    timeframe=TimeFrame(amount=1, unit=TimeFrameUnit.Day),
+                    limit=100,
+                    adjustment=None,
+                    feed=None,
+                )
+                # [ticker],
+                # timeframe=TimeFrame(amount=1, unit=TimeFrameUnit.Day),
+                # start=start.isoformat(),
+                # end=end.isoformat(),
+            )
+            # take the first day after target day
+            return Decimal(raw[ticker][0].high)
+        else:
+            raw = self.historical_client.get_stock_latest_quote(
+                StockLatestQuoteRequest(symbol_or_symbols=ticker, feed=None)
+            )
+            # if we don't have a value for the current day
+            # expand out
+            # this is requuired on weekends
+            if not raw[ticker].ask_price:
+                default = datetime.now(tz=timezone.utc) - timedelta(hours=1)
+                start = default - timedelta(days=7)
+                end = default
+                raw = self.historical_client.get_stock_bars(
+                    StockBarsRequest(
+                        symbol_or_symbols=ticker,
+                        start=start,
+                        end=end,
+                        timeframe=TimeFrame(amount=1, unit=TimeFrameUnit.Day),
+                        feed=None,
+                        adjustment=None,
+                        limit=1000,
+                    )
+                    # [ticker],
+                    # timeframe=TimeFrame(amount=1, unit=TimeFrameUnit.Day),
+                    # start=start.isoformat(),
+                    # end=end.isoformat(),
+                )
+                # take the first day after target day
+                return Decimal(raw[ticker][0].high)
+            return Decimal(raw[ticker].ask_price)
+
+    def buy_instrument(self, ticker: str, qty: Decimal):
+        from alpaca.trading.requests import MarketOrderRequest
+        from alpaca.trading.enums import OrderSide, TimeInForce
+
+        market_order_data = MarketOrderRequest(
+            symbol=ticker,
+            qty=float(qty),
+            side=OrderSide.BUY,
+            time_in_force=TimeInForce.DAY,
+        )
+        self.trading_client.submit_order(order_data=market_order_data)
+
+        return True
+
+    def get_unsettled_instruments(self):
+        from alpaca.trading.requests import GetOrdersRequest, QueryOrderStatus
+
+        open_orders = self.trading_client.get_orders(
+            filter=GetOrdersRequest(status=QueryOrderStatus.OPEN)
+        )
+        return set([o.symbol for o in open_orders])
+
+    def get_holdings(self):
+        from decimal import Decimal
+
+        my_stocks = self.trading_client.get_all_positions()
+        # df = pd.DataFrame(my_stocks)
+        if not my_stocks:
+            return RealPortfolio(holdings=[])
+        total_value = sum([Decimal(item.market_value) for item in my_stocks])
+        out = [
+            RealPortfolioElement(
+                ticker=row.symbol,
+                units=row.qty,
+                value=Decimal(row.market_value),
+                weight=Decimal(row.market_value) / total_value,
+            )
+            for row in my_stocks
+        ]
+        return RealPortfolio(holdings=out)
```

### Comparing `py-portfolio-index-0.0.1/py_portfolio_index/portfolio_providers/base_portfolio.py` & `py-portfolio-index-0.0.2/py_portfolio_index/portfolio_providers/base_portfolio.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,36 +32,39 @@
     def get_unsettled_instruments(self) -> Set[str]:
 
         raise NotImplementedError
 
     def purchase_ticker_value_dict(
         self,
         to_buy: Dict[str, Money],
-        purchasing_power: Union[Money, float],
+        purchasing_power: Union[Money, Decimal, int, float], 
         plan_only: bool = False,
         fractional_shares: bool = True,
         skip_errored_stocks=False,
         rounding_strategy=RoundingStrategy.CLOSEST,
         ignore_unsettled: bool = True,
     ):
         purchased = Money(value=0)
-        purchasing_power = Money(value=purchasing_power)
-        target_value: Money = sum([v for k, v in to_buy.items()])
+        purchasing_power_resolved = Money(value=purchasing_power)
+        target_value: Money = Money(value=sum([v for k, v in to_buy.items()]))
         diff = Money(value=0)
         if ignore_unsettled:
             unsettled = self.get_unsettled_instruments()
         else:
             unsettled = set()
         break_flag = False
         for key, value in to_buy.items():
             if key in unsettled:
                 Logger.info(f"Skipping {key} with unsettled orders.")
                 continue
             try:
-                price = self.get_instrument_price(key)
+                raw_price = self.get_instrument_price(key)
+                if not raw_price:
+                    raise ValueError(f"No price found for this instrument: {key}")
+                price:Money = Money(value=raw_price)
                 Logger.info(f"got price of {price} for {key}")
             except Exception as e:
                 if not skip_errored_stocks:
                     raise e
                 else:
                     continue
             if not price:
@@ -86,30 +89,30 @@
                     )
             if not to_buy_units:
                 Logger.info(f"skipping {key} because no units to buy")
                 continue
             purchasing = to_buy_units * price
 
             Logger.info(f"Need to buy {to_buy_units} units of {key}.")
-            if (purchasing_power - purchasing) < Money(value=0):
+            if (purchasing_power_resolved - purchasing) < Money(value=0):
                 Logger.info("Out of money, buying what is possible and exiting")
                 break_flag = True
-                purchasing = purchasing_power
+                purchasing = purchasing_power_resolved
                 to_buy_units = Decimal(round(purchasing / price, 4).value)
             if to_buy_units > Decimal(0):
                 Logger.info(f"going to buy {to_buy_units} of {key}")
                 try:
                     if not plan_only:
                         purchased = self.buy_instrument(key, to_buy_units)
                     if purchased:
-                        purchasing_power = purchasing_power - purchasing
+                        purchasing_power_resolved = purchasing_power_resolved - purchasing
                         purchased += purchasing
                         diff += abs(value - purchasing)
                         Logger.info(
-                            f"bought {to_buy_units} of {key}, {purchasing_power} left"
+                            f"bought {to_buy_units} of {key}, {purchasing_power_resolved} left"
                         )
                 except Exception as e:
                     print(e)
                     if not skip_errored_stocks:
                         raise e
             if break_flag:
                 Logger.info(
```

### Comparing `py-portfolio-index-0.0.1/py_portfolio_index/portfolio_providers/local_dict.py` & `py-portfolio-index-0.0.2/py_portfolio_index/portfolio_providers/local_dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import random
 from typing import List, Dict, Optional
 from datetime import date
 from py_portfolio_index.models import (
     RealPortfolio,
     RealPortfolioElement,
-    IdealPortfolio,
 )
+from py_portfolio_index.models import Money
 from decimal import Decimal
 from .base_portfolio import BaseProvider
 
 
 class FixedGen:
     def __init__(self, value: float):
         self.value = value
@@ -47,12 +47,12 @@
         return value
 
     def buy_instrument(self, ticker: str, qty: Decimal):
         price = self.get_instrument_price(ticker)
         if not price:
             raise ValueError("No available price for this instrument")
         self._portfolio += RealPortfolioElement(
-            ticker=ticker, units=qty, value=qty * price
+            ticker=ticker, units=qty, value=Money(value=qty * price)
         )
 
     def get_holdings(self):
         return self._portfolio
```

### Comparing `py-portfolio-index-0.0.1/py_portfolio_index/portfolio_providers/robinhood.py` & `py-portfolio-index-0.0.2/py_portfolio_index/portfolio_providers/robinhood.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-index-0.0.1/py_portfolio_index.egg-info/PKG-INFO` & `py-portfolio-index-0.0.2/py_portfolio_index.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,167 +1,167 @@
-Metadata-Version: 2.1
-Name: py-portfolio-index
-Version: 0.0.1
-Summary: Build index portfolios.
-Home-page: 
-Author: 
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-Provides-Extra: alpaca
-Provides-Extra: robinhood
-License-File: LICENSE.txt
-
-## Py Portfolio Index
-
-`py-portfolio-index` is a python library to make it easier to mantain a broad, index-based approach to stock investing
-while following individual ESG (Environmental, Social, and Governance) or SRI (Socially Response Investing) goals.
-
-To do that, it provides tools for constructing and managing portfolios that are modeled off indexes. These ideal
-portfolios can be efficiently converted into actual portfolios by API, using commission free platforms like Robinhood or
-Alpaca. Since constructing an index analogue typically requires many small stock purchases, a
-commission free platform is important to minimizing overhead. Robinhood has the additional benefit of allowing fractional
-share purchases, which allow an index to come closer to an ideal match with a smaller total portfolio size. 
-
-#### Install
-
-The package supports Python 3.7 plus.
-
-`pip install py-portfolio-index` [Not yet!]
-
-#### Considerations
-
-Some providers may take some time to place an order. Keep this in mind when running repeated rebalances, as the
-portfolio balance may not have updated to reflect your last order.
-
-#### Basic Example
-
-This example shows a basic example using the Alpaca API in paper trading mode.
-
-It constructs an ideal portfolio based on the composition of the Vanguard ESG index fund in Q4 2020, then uses the
-Alpaca API to construct a matching portfolio based on an initial investment of 10000 dollars.
-
-Since Alpaca doesn't support fractional shares, this portfolio will approximate an index, but cannot match it exactly, 
-especially for small total portfolio sizes.
-
-```python
-from py_portfolio_index import INDEXES, STOCK_LISTS, Logger, AlpacaProvider, PurchaseStrategy, compare_portfolios,
-
-AlpacaProvider
-
-from logging import INFO, StreamHandler
-
-Logger.addHandler(StreamHandler())
-Logger.setLevel(INFO)
-
-API_KEY = '#########'
-
-SECRET_KEY = '##########'
-
-# The size of our paper portfolio
-TARGET_PORTFOLIO_SIZE = 10000
-
-# instantiate the Alpaca provider with identity information
-# and set it to use the paper provider
-provider = AlpacaProvider(key_id=API_KEY, secret_key=SECRET_KEY, paper=True)
-
-# get an example index 
-# this one is the vanguard ESG index for Q4 202
-ideal_portfolio = INDEXES['esgv_2020_q4']
-
-# exclude all stocks from the oil, vice, and cruise lists
-ideal_portfolio.exclude(STOCK_LISTS['oil']).exclude(STOCK_LISTS['vice']).exclude(STOCK_LISTS['cruises'])
-
-# double the weighting of stocks in the renewable and semiconductor lists, and set them to a minimum weight of .1%
-ideal_portfolio.reweight(STOCK_LISTS['renewable'], weight=2.0, min_weight=.001)
-ideal_portfolio.reweight(STOCK_LISTS['semiconductor'], weight=2.0, min_weight=.001)
-
-# get actual holdings
-real_port = provider.get_holdings()
-
-# compare actual holdings to this ideal portfolio to produce a buy and sell list
-to_buy, to_sell = compare_portfolios(ideal=ideal_portfolio, real=real_port,
-                                     buy_order=PurchaseStrategy.LARGEST_DIFF_FIRST,
-                                     target_size=TARGET_PORTFOLIO_SIZE)
-
-# purchase the buy list
-provider.purchase_ticker_value_dict(to_buy, TARGET_PORTFOLIO_SIZE, fractional_shares=False, skip_errored_stocks=True)
-```
-
-### Robinhood
-
-Since robinhood supports fractional shares, it's much easier to get close to an index
-with a smaller amount of money. 
-
-
-```python
-from py_portfolio_index.bin import INDEXES, STOCK_LISTS
-from py_portfolio_index.enums import PurchaseStrategy
-from py_portfolio_index.operators import compare_portfolios
-from py_portfolio_index.portfolio_providers.robinhood import RobinhoodProvider
-from py_portfolio_index.constants import Logger
-
-from logging import INFO, StreamHandler
-Logger.addHandler(StreamHandler())
-Logger.setLevel(INFO)
-
-ideal_port = INDEXES['esgv_2020_q4']
-
-# create a stock list
-STOCK_LISTS.add_list('manual_override', ['MDLZ'])
-
-# modify the index
-ideal_port.exclude(STOCK_LISTS['oil']).exclude(STOCK_LISTS['vice']).exclude(STOCK_LISTS['cruises']).exclude(
-    STOCK_LISTS['manual_override'])
-
-# overweight on stonks
-ideal_port.reweight(STOCK_LISTS['renewable'], weight=2.0, min_weight=.001)
-ideal_port.reweight(STOCK_LISTS['semiconductor'], weight=2.0, min_weight=.001)
-
-provider = RobinhoodProvider(username='#####', password='#########')
-
-real_port = provider.get_holdings()
-
-TARGET_SIZE = 10000
-
-to_buy, to_sell = compare_portfolios(ideal=ideal_port, real=real_port, buy_order=PurchaseStrategy.CHEAPEST_FIRST,
-                                     target_size = TARGET_SIZE)
-
-
-provider.purchase_ticker_value_dict(to_buy, purchasing_power=1000, fractional_shares=True, skip_errored_stocks=True)
-
-```
-
-### Testing
-
-To avoid actually purchasing a stock, use the plan_only option to log what trades would have occurred.
-
-```python
-
-provider.purchase_ticker_value_dict(to_buy, TARGET_PORTFOLIO_SIZE, plan_only=True, fractional_shares=False,
-                                    skip_errored_stocks=True, )
-
-```
-
-### Example Scripts
-
-Can be found in the examples folder.
-
-### Logging
-
-To see messages, it's helpful to configure the logger to print messages. You can either configure the standard python
-logger or use the portfolio specific one using an example like the below.
-
-```python
-from py_portfolio_index.constants import Logger
-from logging import INFO, StreamHandler
-
-Logger.addHandler(StreamHandler())
-Logger.setLevel(INFO)
-
-```
-
-
-
+Metadata-Version: 2.1
+Name: py-portfolio-index
+Version: 0.0.2
+Summary: Build index portfolios.
+Home-page: 
+Author: 
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+Provides-Extra: alpaca
+Provides-Extra: robinhood
+License-File: LICENSE.txt
+
+## Py Portfolio Index
+
+`py-portfolio-index` is a python library to make it easier to mantain a broad, index-based approach to stock investing
+while following individual ESG (Environmental, Social, and Governance) or SRI (Socially Response Investing) goals.
+
+To do that, it provides tools for constructing and managing portfolios that are modeled off indexes. These ideal
+portfolios can be efficiently converted into actual portfolios by API, using commission free platforms like Robinhood or
+Alpaca. Since constructing an index analogue typically requires many small stock purchases, a
+commission free platform is important to minimizing overhead. Robinhood has the additional benefit of allowing fractional
+share purchases, which allow an index to come closer to an ideal match with a smaller total portfolio size. 
+
+#### Install
+
+The package supports Python 3.7 plus.
+
+`pip install py-portfolio-index` [Not yet!]
+
+#### Considerations
+
+Some providers may take some time to place an order. Keep this in mind when running repeated rebalances, as the
+portfolio balance may not have updated to reflect your last order.
+
+#### Basic Example
+
+This example shows a basic example using the Alpaca API in paper trading mode.
+
+It constructs an ideal portfolio based on the composition of the Vanguard ESG index fund in Q4 2020, then uses the
+Alpaca API to construct a matching portfolio based on an initial investment of 10000 dollars.
+
+Since Alpaca doesn't support fractional shares, this portfolio will approximate an index, but cannot match it exactly, 
+especially for small total portfolio sizes.
+
+```python
+from py_portfolio_index import INDEXES, STOCK_LISTS, Logger, AlpacaProvider, PurchaseStrategy, compare_portfolios,
+
+AlpacaProvider
+
+from logging import INFO, StreamHandler
+
+Logger.addHandler(StreamHandler())
+Logger.setLevel(INFO)
+
+API_KEY = '#########'
+
+SECRET_KEY = '##########'
+
+# The size of our paper portfolio
+TARGET_PORTFOLIO_SIZE = 10000
+
+# instantiate the Alpaca provider with identity information
+# and set it to use the paper provider
+provider = AlpacaProvider(key_id=API_KEY, secret_key=SECRET_KEY, paper=True)
+
+# get an example index 
+# this one is the vanguard ESG index for Q4 202
+ideal_portfolio = INDEXES['esgv_2020_q4']
+
+# exclude all stocks from the oil, vice, and cruise lists
+ideal_portfolio.exclude(STOCK_LISTS['oil']).exclude(STOCK_LISTS['vice']).exclude(STOCK_LISTS['cruises'])
+
+# double the weighting of stocks in the renewable and semiconductor lists, and set them to a minimum weight of .1%
+ideal_portfolio.reweight(STOCK_LISTS['renewable'], weight=2.0, min_weight=.001)
+ideal_portfolio.reweight(STOCK_LISTS['semiconductor'], weight=2.0, min_weight=.001)
+
+# get actual holdings
+real_port = provider.get_holdings()
+
+# compare actual holdings to this ideal portfolio to produce a buy and sell list
+to_buy, to_sell = compare_portfolios(ideal=ideal_portfolio, real=real_port,
+                                     buy_order=PurchaseStrategy.LARGEST_DIFF_FIRST,
+                                     target_size=TARGET_PORTFOLIO_SIZE)
+
+# purchase the buy list
+provider.purchase_ticker_value_dict(to_buy, TARGET_PORTFOLIO_SIZE, fractional_shares=False, skip_errored_stocks=True)
+```
+
+### Robinhood
+
+Since robinhood supports fractional shares, it's much easier to get close to an index
+with a smaller amount of money. 
+
+
+```python
+from py_portfolio_index.bin import INDEXES, STOCK_LISTS
+from py_portfolio_index.enums import PurchaseStrategy
+from py_portfolio_index.operators import compare_portfolios
+from py_portfolio_index.portfolio_providers.robinhood import RobinhoodProvider
+from py_portfolio_index.constants import Logger
+
+from logging import INFO, StreamHandler
+Logger.addHandler(StreamHandler())
+Logger.setLevel(INFO)
+
+ideal_port = INDEXES['esgv_2020_q4']
+
+# create a stock list
+STOCK_LISTS.add_list('manual_override', ['MDLZ'])
+
+# modify the index
+ideal_port.exclude(STOCK_LISTS['oil']).exclude(STOCK_LISTS['vice']).exclude(STOCK_LISTS['cruises']).exclude(
+    STOCK_LISTS['manual_override'])
+
+# overweight on stonks
+ideal_port.reweight(STOCK_LISTS['renewable'], weight=2.0, min_weight=.001)
+ideal_port.reweight(STOCK_LISTS['semiconductor'], weight=2.0, min_weight=.001)
+
+provider = RobinhoodProvider(username='#####', password='#########')
+
+real_port = provider.get_holdings()
+
+TARGET_SIZE = 10000
+
+to_buy, to_sell = compare_portfolios(ideal=ideal_port, real=real_port, buy_order=PurchaseStrategy.CHEAPEST_FIRST,
+                                     target_size = TARGET_SIZE)
+
+
+provider.purchase_ticker_value_dict(to_buy, purchasing_power=1000, fractional_shares=True, skip_errored_stocks=True)
+
+```
+
+### Testing
+
+To avoid actually purchasing a stock, use the plan_only option to log what trades would have occurred.
+
+```python
+
+provider.purchase_ticker_value_dict(to_buy, TARGET_PORTFOLIO_SIZE, plan_only=True, fractional_shares=False,
+                                    skip_errored_stocks=True, )
+
+```
+
+### Example Scripts
+
+Can be found in the examples folder.
+
+### Logging
+
+To see messages, it's helpful to configure the logger to print messages. You can either configure the standard python
+logger or use the portfolio specific one using an example like the below.
+
+```python
+from py_portfolio_index.constants import Logger
+from logging import INFO, StreamHandler
+
+Logger.addHandler(StreamHandler())
+Logger.setLevel(INFO)
+
+```
+
+
+
```

### Comparing `py-portfolio-index-0.0.1/py_portfolio_index.egg-info/SOURCES.txt` & `py-portfolio-index-0.0.2/py_portfolio_index.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 LICENSE.txt
 README.md
+pyproject.toml
 setup.py
 py_portfolio_index/__init__.py
 py_portfolio_index/common.py
 py_portfolio_index/config.py
 py_portfolio_index/constants.py
 py_portfolio_index/enums.py
 py_portfolio_index/exceptions.py
 py_portfolio_index/models.py
 py_portfolio_index/operators.py
+py_portfolio_index/py.typed
 py_portfolio_index.egg-info/PKG-INFO
 py_portfolio_index.egg-info/SOURCES.txt
 py_portfolio_index.egg-info/dependency_links.txt
 py_portfolio_index.egg-info/requires.txt
 py_portfolio_index.egg-info/top_level.txt
 py_portfolio_index/bin/__init__.py
 py_portfolio_index/bin/indexes/__init__.py
```

### Comparing `py-portfolio-index-0.0.1/setup.py` & `py-portfolio-index-0.0.2/setup.py`

 * *Files identical despite different names*

