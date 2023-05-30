# Comparing `tmp/almgren_chriss-1.0.1.tar.gz` & `tmp/almgren_chriss-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "almgren_chriss-1.0.1.tar", max compression
+gzip compressed data, was "almgren_chriss-1.1.0.tar", max compression
```

## Comparing `almgren_chriss-1.0.1.tar` & `almgren_chriss-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2023-05-28 21:04:12.561533 almgren_chriss-1.0.1/LICENSE
--rw-r--r--   0        0        0     2102 2023-05-28 21:04:12.561533 almgren_chriss-1.0.1/README.rst
--rw-r--r--   0        0        0     1152 2023-05-28 21:04:12.561533 almgren_chriss-1.0.1/almgren_chriss/__init__.py
--rw-r--r--   0        0        0     3058 2023-05-28 21:04:12.561533 almgren_chriss-1.0.1/almgren_chriss/cost.py
--rw-r--r--   0        0        0     2754 2023-05-28 21:04:12.561533 almgren_chriss-1.0.1/almgren_chriss/decay_rate.py
--rw-r--r--   0        0        0     2528 2023-05-28 21:04:12.561533 almgren_chriss-1.0.1/almgren_chriss/trade.py
--rw-r--r--   0        0        0      836 2023-05-28 21:04:35.590162 almgren_chriss-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2887 1970-01-01 00:00:00.000000 almgren_chriss-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-30 19:19:20.905943 almgren_chriss-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2113 2023-05-30 19:19:20.905943 almgren_chriss-1.1.0/README.rst
+-rw-r--r--   0        0        0      945 2023-05-30 19:19:20.905943 almgren_chriss-1.1.0/almgren_chriss/__init__.py
+-rw-r--r--   0        0        0     3875 2023-05-30 19:19:20.905943 almgren_chriss-1.1.0/almgren_chriss/cost.py
+-rw-r--r--   0        0        0     2489 2023-05-30 19:19:20.905943 almgren_chriss-1.1.0/almgren_chriss/decay_rate.py
+-rw-r--r--   0        0        0     2186 2023-05-30 19:19:20.905943 almgren_chriss-1.1.0/almgren_chriss/trade.py
+-rw-r--r--   0        0        0      836 2023-05-30 19:19:40.765921 almgren_chriss-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2898 1970-01-01 00:00:00.000000 almgren_chriss-1.1.0/PKG-INFO
```

### Comparing `almgren_chriss-1.0.1/LICENSE` & `almgren_chriss-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `almgren_chriss-1.0.1/README.rst` & `almgren_chriss-1.1.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -43,20 +43,20 @@
    epsilon = 0.0625
    X = 1e06
    T = 5
 
 >>> trade_trajectory(lambda_, tau, sigma, gamma, eta, X, T)
 array([1000000.0, 428598.84574702, 182932.81426177, 76295.72161546, 27643.37739691, 0.0])
 
-.. image:: assets/trade_trajectory.png
+.. image:: docs/assets/trade_trajectory.png
 
 >>> trade_list(lambda_, tau, sigma, gamma, eta, X, T)
 array([571401.15425298, 245666.03148525, 106637.09264631, 48652.34421856, 27643.37739691])
 
-.. image:: assets/trade_list.png
+.. image:: docs/assets/trade_list.png
 
 >>> cost_expectation(lambda_, tau, sigma, gamma, eta, epsilon, X, T)
 1140715.1670497851
 
 >>> import math
 >>> math.sqrt(cost_variance(lambda_, tau, sigma, gamma, eta, X, T))
-449367.65254135116
+449367.65254135116
```

### Comparing `almgren_chriss-1.0.1/almgren_chriss/__init__.py` & `almgren_chriss-1.1.0/almgren_chriss/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 """
 This package provides functions for implementing the Almgren-Chriss model for optimal execution of portfolio
 transactions.
 
 Modules
 -------
 cost
-    Provides functions for calculating the expected cost and variance of the cost of trading.
+    Provides functions for calculating the expectation, variance and value-at-risk of the cost of trading.
 decay_rate
     Provides functions for calculating the trade decay rate.
 trade
     Provides functions for calculating the trading trajectory and the list of trades.
 
 Functions
 ---------
 cost_expectation
     Calculate the expected cost of trading.
 cost_variance
     Calculate the variance of the cost of trading.
+value_at_risk
+    Calculate the value-at-risk of the cost of trading.
 decay_rate
     Calculate the trade decay rate.
 trade_trajectory
     Calculate the trading trajectory.
 trade_list
     Calculate the list of trades.
-
-Each function takes various parameters including risk tolerance, interval between trades, volatility, permanent impact
-slope, temporary impact slope, total number of shares, and trading duration. Please refer to the individual function
-documentation for more details on the parameters and return values.
 """
-from .cost import cost_expectation, cost_variance
+from .cost import cost_expectation, cost_variance, value_at_risk
 from .decay_rate import kappa as decay_rate
 from .trade import trade_trajectory, trade_list
```

### Comparing `almgren_chriss-1.0.1/almgren_chriss/cost.py` & `almgren_chriss-1.1.0/almgren_chriss/cost.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,47 +4,24 @@
 
 Functions
 ----------
 cost_expectation
     Calculate the expected cost of trading.
 cost_variance
     Calculate the variance of the cost of trading.
-
-Parameters
-----------
-lambda_ : float
-    Risk tolerance (lambda)
-tau : float
-    Interval between trades
-sigma : float
-    Volatility
-gamma : float
-    Permanent impact slope
-eta : float
-    Temporary impact slope
-epsilon : float
-    Temporary impact intercept
-X : float
-    Total number of shares
-T : float
-    Trading duration
-
-Returns
--------
-numpy.ndarray
-    The calculated values.
 """
 import math
 
 import numpy as np
+from scipy.stats import norm
 
 from .decay_rate import kappa, tilde_tau
 
 
-__all__ = ['cost_expectation', 'cost_variance']
+__all__ = ['cost_expectation', 'cost_variance', 'value_at_risk']
 
 
 def cost_expectation(lambda_: float, tau: float, sigma: float, gamma: float, eta: float, epsilon: float,
                      X: float, T: float) -> np.ndarray:
     r"""
     Compute the expected cost of trading in the Almgren-Chriss model.
 
@@ -58,22 +35,24 @@
         Interval between trades
     sigma : float
         Volatility
     gamma : float
         Permanent impact slope
     eta : float
         Temporary impact slope
+    epsilon: float
+        Temporary impact intercept
     X : float
         Total number of shares
     T : float
         Trading duration
 
     Returns
     -------
-    np.ndarray
+    float
         The expected cost of trading
     """
     kappa_ = kappa(lambda_, tau, sigma, gamma, eta)
     a = math.tanh(kappa_ * tau / 2) * (tau * math.sinh(2 * kappa_ * T) + 2 * T * math.sinh(kappa_ * tau))
     b = 2 * tau ** 2 * math.sinh(kappa_ * T) ** 2
     return ((gamma * X ** 2) / 2
             + epsilon * X
@@ -102,14 +81,53 @@
     X : float
         Total number of shares
     T : float
         Trading duration
 
     Returns
     -------
-    np.ndarray
+    float
         The variance of the cost of trading
     """
     kappa_ = kappa(lambda_, tau, sigma, gamma, eta)
     a = tau * math.sinh(kappa_ * T) * math.cosh(kappa_ * (T - tau)) - T * math.sinh(kappa_ * tau)
     b = math.sinh(kappa_ * T) ** 2 * math.sinh(kappa_ * tau)
     return (sigma ** 2 * X ** 2 / 2) * (a / b)
+
+
+def value_at_risk(lambda_: float, tau: float, sigma: float, gamma: float, eta: float, epsilon: float,
+                  X: float, T: float,
+                  probability: float = .95) -> np.ndarray:
+    r"""
+    Compute the value-at-risk of the cost of trading in the Almgren-Chriss model.
+
+    .. math:: Var_p(x) = E(x) + \lambda_v \sqrt{V(x)}
+
+    Parameters
+    ----------
+    lambda_ : float
+        Risk tolerance
+    tau : float
+        Interval between trades
+    sigma : float
+        Volatility
+    gamma : float
+        Permanent impact slope
+    eta : float
+        Temporary impact slope
+    epsilon: float
+        Temporary impact intercept
+    X : float
+        Total number of shares
+    T : float
+        Trading duration
+    probability : float
+        Probability that the cost won't exceed the value-at-risk.
+
+    Returns
+    -------
+    float
+        The value-at-risk of the cost of trading
+    """
+    E_x = cost_expectation(lambda_, tau, sigma, gamma, eta, epsilon, X, T)
+    V_x = cost_variance(lambda_, tau, sigma, gamma, eta, X, T)
+    return E_x + norm.ppf(probability) * math.sqrt(V_x)
```

### Comparing `almgren_chriss-1.0.1/almgren_chriss/decay_rate.py` & `almgren_chriss-1.1.0/almgren_chriss/decay_rate.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,32 +5,14 @@
 ---------
 tilde_kappa_squared
     Calculate the square of the adjusted trade decay rate.
 tilde_tau
     Calculate the adjusted interval between trades.
 kappa
     Calculate the trade decay rate.
-
-Parameters
-----------
-lambda_ : float
-    Risk tolerance (lambda)
-tau : float
-    Interval between trades
-sigma : float
-    Volatility
-gamma : float
-    Permanent impact slope
-eta : float
-    Temporary impact slope
-
-Returns
--------
-float
-    The calculated value.
 """
 import math
 
 
 __all__ = ['tilde_kappa_squared', 'tilde_tau', 'kappa']
```

### Comparing `almgren_chriss-1.0.1/almgren_chriss/trade.py` & `almgren_chriss-1.1.0/almgren_chriss/trade.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,36 +3,14 @@
 
 Functions
 ---------
 trade_trajectory
     Calculate the trading trajectory.
 trade_list
     Calculate the list of trades.
-
-Parameters
-----------
-lambda_ : float
-    Risk tolerance (lambda)
-tau : float
-    Interval between trades
-sigma : float
-    Volatility
-gamma : float
-    Permanent impact slope
-eta : float
-    Temporary impact slope
-X : float
-    Total number of shares
-T : float
-    Trading duration
-
-Returns
--------
-numpy.ndarray
-    The calculated values.
 """
 import math
 
 import numpy as np
 
 from .decay_rate import kappa
```

### Comparing `almgren_chriss-1.0.1/pyproject.toml` & `almgren_chriss-1.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "almgren_chriss"
-version = "1.0.1"
+version = "1.1.0"
 description = "functions for implementing the Almgren-Chriss model for optimal execution of portfolio transactions."
 authors = ["Bernardo Paulsen <paulsen.bernardo@gmail.com>"]
 license = "GNU General Public License"
 readme = "README.rst"
 packages = [{ include = "almgren_chriss" }]
 keywords = ["optimal exeuction", "quantitative finance", "Almgren Chriss"]
```

### Comparing `almgren_chriss-1.0.1/PKG-INFO` & `almgren_chriss-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almgren-chriss
-Version: 1.0.1
+Version: 1.1.0
 Summary: functions for implementing the Almgren-Chriss model for optimal execution of portfolio transactions.
 License: GNU General Public License
 Keywords: optimal exeuction,quantitative finance,Almgren Chriss
 Author: Bernardo Paulsen
 Author-email: paulsen.bernardo@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
@@ -61,20 +61,21 @@
    epsilon = 0.0625
    X = 1e06
    T = 5
 
 >>> trade_trajectory(lambda_, tau, sigma, gamma, eta, X, T)
 array([1000000.0, 428598.84574702, 182932.81426177, 76295.72161546, 27643.37739691, 0.0])
 
-.. image:: assets/trade_trajectory.png
+.. image:: docs/assets/trade_trajectory.png
 
 >>> trade_list(lambda_, tau, sigma, gamma, eta, X, T)
 array([571401.15425298, 245666.03148525, 106637.09264631, 48652.34421856, 27643.37739691])
 
-.. image:: assets/trade_list.png
+.. image:: docs/assets/trade_list.png
 
 >>> cost_expectation(lambda_, tau, sigma, gamma, eta, epsilon, X, T)
 1140715.1670497851
 
 >>> import math
 >>> math.sqrt(cost_variance(lambda_, tau, sigma, gamma, eta, X, T))
 449367.65254135116
+
```

