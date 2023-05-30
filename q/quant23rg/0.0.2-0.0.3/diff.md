# Comparing `tmp/quant23rg-0.0.2.tar.gz` & `tmp/quant23rg-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quant23rg-0.0.2.tar", last modified: Tue May 30 07:04:56 2023, max compression
+gzip compressed data, was "quant23rg-0.0.3.tar", last modified: Tue May 30 07:15:25 2023, max compression
```

## Comparing `quant23rg-0.0.2.tar` & `quant23rg-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-30 07:04:56.190629 quant23rg-0.0.2/
--rw-r--r--   0 root         (0) staff       (20)     1064 2023-05-30 06:19:05.000000 quant23rg-0.0.2/LICENSE
--rw-r--r--   0 root         (0) staff       (20)     7165 2023-05-30 07:04:56.190451 quant23rg-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     6648 2023-05-30 06:39:31.000000 quant23rg-0.0.2/README.md
--rw-r--r--   0 root         (0) staff       (20)      660 2023-05-30 07:04:31.000000 quant23rg-0.0.2/pyproject.toml
--rw-r--r--   0 root         (0) staff       (20)       38 2023-05-30 07:04:56.190684 quant23rg-0.0.2/setup.cfg
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-30 07:04:56.186392 quant23rg-0.0.2/src/
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-30 07:04:56.189220 quant23rg-0.0.2/src/quant23rg/
--rw-r--r--   0 root         (0) staff       (20)      308 2023-05-30 00:33:36.000000 quant23rg-0.0.2/src/quant23rg/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     7631 2023-05-30 06:18:51.000000 quant23rg-0.0.2/src/quant23rg/implied_volatility.py
--rw-r--r--   0 root         (0) staff       (20)      921 2023-05-30 06:18:54.000000 quant23rg-0.0.2/src/quant23rg/pricingBS.py
--rw-r--r--   0 root         (0) staff       (20)     7789 2023-05-30 06:18:56.000000 quant23rg-0.0.2/src/quant23rg/pricingCallEuropBS.py
--rw-r--r--   0 root         (0) staff       (20)    12438 2023-05-30 06:18:58.000000 quant23rg-0.0.2/src/quant23rg/pricingGBM.py
--rw-r--r--   0 root         (0) staff       (20)     5233 2023-05-30 06:19:01.000000 quant23rg-0.0.2/src/quant23rg/pricingPutEuropBS.py
--rw-r--r--   0 root         (0) staff       (20)    21909 2023-05-30 06:19:03.000000 quant23rg-0.0.2/src/quant23rg/riskManagement.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-30 07:04:56.190248 quant23rg-0.0.2/src/quant23rg.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     7165 2023-05-30 07:04:56.000000 quant23rg-0.0.2/src/quant23rg.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      400 2023-05-30 07:04:56.000000 quant23rg-0.0.2/src/quant23rg.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-05-30 07:04:56.000000 quant23rg-0.0.2/src/quant23rg.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       10 2023-05-30 07:04:56.000000 quant23rg-0.0.2/src/quant23rg.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-30 07:15:25.840557 quant23rg-0.0.3/
+-rw-r--r--   0 root         (0) staff       (20)     1064 2023-05-30 06:19:05.000000 quant23rg-0.0.3/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)     7132 2023-05-30 07:15:25.840263 quant23rg-0.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     6615 2023-05-30 07:14:35.000000 quant23rg-0.0.3/README.md
+-rw-r--r--   0 root         (0) staff       (20)      660 2023-05-30 07:14:54.000000 quant23rg-0.0.3/pyproject.toml
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-05-30 07:15:25.840627 quant23rg-0.0.3/setup.cfg
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-30 07:15:25.833937 quant23rg-0.0.3/src/
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-30 07:15:25.838848 quant23rg-0.0.3/src/quant23rg/
+-rw-r--r--   0 root         (0) staff       (20)      308 2023-05-30 00:33:36.000000 quant23rg-0.0.3/src/quant23rg/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     7631 2023-05-30 06:18:51.000000 quant23rg-0.0.3/src/quant23rg/implied_volatility.py
+-rw-r--r--   0 root         (0) staff       (20)      921 2023-05-30 06:18:54.000000 quant23rg-0.0.3/src/quant23rg/pricingBS.py
+-rw-r--r--   0 root         (0) staff       (20)     7789 2023-05-30 06:18:56.000000 quant23rg-0.0.3/src/quant23rg/pricingCallEuropBS.py
+-rw-r--r--   0 root         (0) staff       (20)    12438 2023-05-30 06:18:58.000000 quant23rg-0.0.3/src/quant23rg/pricingGBM.py
+-rw-r--r--   0 root         (0) staff       (20)     5233 2023-05-30 06:19:01.000000 quant23rg-0.0.3/src/quant23rg/pricingPutEuropBS.py
+-rw-r--r--   0 root         (0) staff       (20)    21909 2023-05-30 06:19:03.000000 quant23rg-0.0.3/src/quant23rg/riskManagement.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-30 07:15:25.840028 quant23rg-0.0.3/src/quant23rg.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     7132 2023-05-30 07:15:25.000000 quant23rg-0.0.3/src/quant23rg.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      400 2023-05-30 07:15:25.000000 quant23rg-0.0.3/src/quant23rg.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-30 07:15:25.000000 quant23rg-0.0.3/src/quant23rg.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       10 2023-05-30 07:15:25.000000 quant23rg-0.0.3/src/quant23rg.egg-info/top_level.txt
```

### Comparing `quant23rg-0.0.2/LICENSE` & `quant23rg-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `quant23rg-0.0.2/PKG-INFO` & `quant23rg-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quant23rg
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package for quantitative analysis
 Author-email: Adrien Calas <le23rg@icloud.com>
 Project-URL: Homepage, https://github.com/leRayGorbella/quant23rg
 Project-URL: Bug Tracker, https://github.com/leRayGorbella/quant23rg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 # Welcome on the quant23rg package
 
 ## quant23rg is python package for quantitative analysis
 
 ## Install it by typing this command in your command prompt 
 
 ```
-pip install quant23rg
+pip install quant23rg==0.0.3
 ```
 
 ## The package is still in progress
 
 ### Author : Adrien Calas - Le23RayGorbella (Freelancer)
 
 ### [Click here to contact by mail](mailto:le23rg@icloud.com?subject=[From%20quant23rg%20package]), Location : Paris and Nice, France
@@ -31,22 +31,17 @@
 ### [Linkedin](https://www.linkedin.com/in/adrien-calas-881132151/)
 
 ## Available : european options pricing, implied volatilities, geometrical brownian motion for assets and portfolios, value at risk & conditional value at risk (work in progress for portfolio)
 
 ### European options pricing
 
 ```python
-from pricingCallEuropBS import PricingCallEuropBS
-from pricingPutEuropBS import PricingPutEuropBS
-
-
 import pandas as pd
-from implied_volatility import ImpliedVolatility
-from pricingCallEuropBS import PricingCallEuropBS
-from pricingPutEuropBS import PricingPutEuropBS
+from quant23rg.pricingCallEuropBS import PricingCallEuropBS
+from quant23rg.pricingPutEuropBS import PricingPutEuropBS
 
 spy_opt = pd.read_csv(
     "spy-options.csv",
 ).dropna()
 spy_opt.columns = [
     col + "_call" if ".1" not in col and col != "Strike" else col
     for col in spy_opt.columns
@@ -100,14 +95,15 @@
 
 ```
 
 ### Implied volatilities
 
 ```python
 ### See volatility smile (Strike -> IV(Strike)) ###
+from quant23rg.implied_volatility import ImpliedVolatility
 
 ivs = ImpliedVolatility(
     s0=s0,
     strike=call_example.Strike,
     dt=dt,
     interest_rate=0.05 * dt,  # fed rate  multiplied by our period of time
     volatility=0.1326,
@@ -122,15 +118,15 @@
 
 
 ```
 
 ### Geometrical Brownian Motion for assets and portfolios
 
 ```python
-from pricingGBM import PricingGBM, PricingGBMPortfolio
+from quant23rg.pricingGBM import PricingGBM, PricingGBMPortfolio
 import yfinance as yf
 
 
 sp500 = yf.Ticker("^GSPC")
 hist_sp500 = sp500.history("1y")
 hist_sp500["returns"] = hist_sp500.Close / hist_sp500.Close.shift(1) - 1
 returns_serie = hist_sp500.dropna().returns
@@ -151,15 +147,15 @@
 
 ### Value at Risk & Conditional Value at Risk (work in progress for portfolio)
 
 ```python
 
 
 ### Value at Risk (one asset) ###
-from riskManagement import RiskManagementOneAsset
+from quant23rg.riskManagement import RiskManagementOneAsset
 
 rkManageHistoric = RiskManagementOneAsset(returns_serie, input_type="returns")
 rkManageNormal = RiskManagementOneAsset(
     returns_serie,
     mode="normal",
 )
 rkManageMonteCarlo = RiskManagementOneAsset(
@@ -190,15 +186,15 @@
 #################################################
 
 
 ### Value at Risk multiple assets (Cholesky) ###
 
 import yfinance as yf
 import numpy as np
-from riskManagement import RiskManagementPortfolio
+from quant23rg.riskManagement import RiskManagementPortfolio
 
 ## Datas for the test
 sp500 = yf.Ticker("^GSPC")
 hist_sp500 = sp500.history("1y")
 aapl = yf.Ticker("AAPL")
 hist_aapl = aapl.history("1y")
 hist_sp500["returns"] = hist_sp500.Close / hist_sp500.Close.shift(1) - 1
```

### Comparing `quant23rg-0.0.2/README.md` & `quant23rg-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Welcome on the quant23rg package
 
 ## quant23rg is python package for quantitative analysis
 
 ## Install it by typing this command in your command prompt 
 
 ```
-pip install quant23rg
+pip install quant23rg==0.0.3
 ```
 
 ## The package is still in progress
 
 ### Author : Adrien Calas - Le23RayGorbella (Freelancer)
 
 ### [Click here to contact by mail](mailto:le23rg@icloud.com?subject=[From%20quant23rg%20package]), Location : Paris and Nice, France
@@ -17,22 +17,17 @@
 ### [Linkedin](https://www.linkedin.com/in/adrien-calas-881132151/)
 
 ## Available : european options pricing, implied volatilities, geometrical brownian motion for assets and portfolios, value at risk & conditional value at risk (work in progress for portfolio)
 
 ### European options pricing
 
 ```python
-from pricingCallEuropBS import PricingCallEuropBS
-from pricingPutEuropBS import PricingPutEuropBS
-
-
 import pandas as pd
-from implied_volatility import ImpliedVolatility
-from pricingCallEuropBS import PricingCallEuropBS
-from pricingPutEuropBS import PricingPutEuropBS
+from quant23rg.pricingCallEuropBS import PricingCallEuropBS
+from quant23rg.pricingPutEuropBS import PricingPutEuropBS
 
 spy_opt = pd.read_csv(
     "spy-options.csv",
 ).dropna()
 spy_opt.columns = [
     col + "_call" if ".1" not in col and col != "Strike" else col
     for col in spy_opt.columns
@@ -86,14 +81,15 @@
 
 ```
 
 ### Implied volatilities
 
 ```python
 ### See volatility smile (Strike -> IV(Strike)) ###
+from quant23rg.implied_volatility import ImpliedVolatility
 
 ivs = ImpliedVolatility(
     s0=s0,
     strike=call_example.Strike,
     dt=dt,
     interest_rate=0.05 * dt,  # fed rate  multiplied by our period of time
     volatility=0.1326,
@@ -108,15 +104,15 @@
 
 
 ```
 
 ### Geometrical Brownian Motion for assets and portfolios
 
 ```python
-from pricingGBM import PricingGBM, PricingGBMPortfolio
+from quant23rg.pricingGBM import PricingGBM, PricingGBMPortfolio
 import yfinance as yf
 
 
 sp500 = yf.Ticker("^GSPC")
 hist_sp500 = sp500.history("1y")
 hist_sp500["returns"] = hist_sp500.Close / hist_sp500.Close.shift(1) - 1
 returns_serie = hist_sp500.dropna().returns
@@ -137,15 +133,15 @@
 
 ### Value at Risk & Conditional Value at Risk (work in progress for portfolio)
 
 ```python
 
 
 ### Value at Risk (one asset) ###
-from riskManagement import RiskManagementOneAsset
+from quant23rg.riskManagement import RiskManagementOneAsset
 
 rkManageHistoric = RiskManagementOneAsset(returns_serie, input_type="returns")
 rkManageNormal = RiskManagementOneAsset(
     returns_serie,
     mode="normal",
 )
 rkManageMonteCarlo = RiskManagementOneAsset(
@@ -176,15 +172,15 @@
 #################################################
 
 
 ### Value at Risk multiple assets (Cholesky) ###
 
 import yfinance as yf
 import numpy as np
-from riskManagement import RiskManagementPortfolio
+from quant23rg.riskManagement import RiskManagementPortfolio
 
 ## Datas for the test
 sp500 = yf.Ticker("^GSPC")
 hist_sp500 = sp500.history("1y")
 aapl = yf.Ticker("AAPL")
 hist_aapl = aapl.history("1y")
 hist_sp500["returns"] = hist_sp500.Close / hist_sp500.Close.shift(1) - 1
```

### Comparing `quant23rg-0.0.2/pyproject.toml` & `quant23rg-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "yfinance>=0.1.70", "plotly>=5.6.0", "pandas>=1.3.4", "scipy>=1.8.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quant23rg"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Adrien Calas", email="le23rg@icloud.com" },
 ]
 description = "Package for quantitative analysis"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `quant23rg-0.0.2/src/quant23rg/implied_volatility.py` & `quant23rg-0.0.3/src/quant23rg/implied_volatility.py`

 * *Files identical despite different names*

### Comparing `quant23rg-0.0.2/src/quant23rg/pricingBS.py` & `quant23rg-0.0.3/src/quant23rg/pricingBS.py`

 * *Files identical despite different names*

### Comparing `quant23rg-0.0.2/src/quant23rg/pricingCallEuropBS.py` & `quant23rg-0.0.3/src/quant23rg/pricingCallEuropBS.py`

 * *Files identical despite different names*

### Comparing `quant23rg-0.0.2/src/quant23rg/pricingGBM.py` & `quant23rg-0.0.3/src/quant23rg/pricingGBM.py`

 * *Files identical despite different names*

### Comparing `quant23rg-0.0.2/src/quant23rg/pricingPutEuropBS.py` & `quant23rg-0.0.3/src/quant23rg/pricingPutEuropBS.py`

 * *Files identical despite different names*

### Comparing `quant23rg-0.0.2/src/quant23rg/riskManagement.py` & `quant23rg-0.0.3/src/quant23rg/riskManagement.py`

 * *Files identical despite different names*

### Comparing `quant23rg-0.0.2/src/quant23rg.egg-info/PKG-INFO` & `quant23rg-0.0.3/src/quant23rg.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quant23rg
-Version: 0.0.2
+Version: 0.0.3
 Summary: Package for quantitative analysis
 Author-email: Adrien Calas <le23rg@icloud.com>
 Project-URL: Homepage, https://github.com/leRayGorbella/quant23rg
 Project-URL: Bug Tracker, https://github.com/leRayGorbella/quant23rg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,15 +15,15 @@
 # Welcome on the quant23rg package
 
 ## quant23rg is python package for quantitative analysis
 
 ## Install it by typing this command in your command prompt 
 
 ```
-pip install quant23rg
+pip install quant23rg==0.0.3
 ```
 
 ## The package is still in progress
 
 ### Author : Adrien Calas - Le23RayGorbella (Freelancer)
 
 ### [Click here to contact by mail](mailto:le23rg@icloud.com?subject=[From%20quant23rg%20package]), Location : Paris and Nice, France
@@ -31,22 +31,17 @@
 ### [Linkedin](https://www.linkedin.com/in/adrien-calas-881132151/)
 
 ## Available : european options pricing, implied volatilities, geometrical brownian motion for assets and portfolios, value at risk & conditional value at risk (work in progress for portfolio)
 
 ### European options pricing
 
 ```python
-from pricingCallEuropBS import PricingCallEuropBS
-from pricingPutEuropBS import PricingPutEuropBS
-
-
 import pandas as pd
-from implied_volatility import ImpliedVolatility
-from pricingCallEuropBS import PricingCallEuropBS
-from pricingPutEuropBS import PricingPutEuropBS
+from quant23rg.pricingCallEuropBS import PricingCallEuropBS
+from quant23rg.pricingPutEuropBS import PricingPutEuropBS
 
 spy_opt = pd.read_csv(
     "spy-options.csv",
 ).dropna()
 spy_opt.columns = [
     col + "_call" if ".1" not in col and col != "Strike" else col
     for col in spy_opt.columns
@@ -100,14 +95,15 @@
 
 ```
 
 ### Implied volatilities
 
 ```python
 ### See volatility smile (Strike -> IV(Strike)) ###
+from quant23rg.implied_volatility import ImpliedVolatility
 
 ivs = ImpliedVolatility(
     s0=s0,
     strike=call_example.Strike,
     dt=dt,
     interest_rate=0.05 * dt,  # fed rate  multiplied by our period of time
     volatility=0.1326,
@@ -122,15 +118,15 @@
 
 
 ```
 
 ### Geometrical Brownian Motion for assets and portfolios
 
 ```python
-from pricingGBM import PricingGBM, PricingGBMPortfolio
+from quant23rg.pricingGBM import PricingGBM, PricingGBMPortfolio
 import yfinance as yf
 
 
 sp500 = yf.Ticker("^GSPC")
 hist_sp500 = sp500.history("1y")
 hist_sp500["returns"] = hist_sp500.Close / hist_sp500.Close.shift(1) - 1
 returns_serie = hist_sp500.dropna().returns
@@ -151,15 +147,15 @@
 
 ### Value at Risk & Conditional Value at Risk (work in progress for portfolio)
 
 ```python
 
 
 ### Value at Risk (one asset) ###
-from riskManagement import RiskManagementOneAsset
+from quant23rg.riskManagement import RiskManagementOneAsset
 
 rkManageHistoric = RiskManagementOneAsset(returns_serie, input_type="returns")
 rkManageNormal = RiskManagementOneAsset(
     returns_serie,
     mode="normal",
 )
 rkManageMonteCarlo = RiskManagementOneAsset(
@@ -190,15 +186,15 @@
 #################################################
 
 
 ### Value at Risk multiple assets (Cholesky) ###
 
 import yfinance as yf
 import numpy as np
-from riskManagement import RiskManagementPortfolio
+from quant23rg.riskManagement import RiskManagementPortfolio
 
 ## Datas for the test
 sp500 = yf.Ticker("^GSPC")
 hist_sp500 = sp500.history("1y")
 aapl = yf.Ticker("AAPL")
 hist_aapl = aapl.history("1y")
 hist_sp500["returns"] = hist_sp500.Close / hist_sp500.Close.shift(1) - 1
```

