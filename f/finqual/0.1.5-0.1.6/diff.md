# Comparing `tmp/finqual-0.1.5.tar.gz` & `tmp/finqual-0.1.6.tar.gz`

## Comparing `finqual-0.1.5.tar` & `finqual-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finqual-0.1.5/finqual/__init__.py
--rw-r--r--   0        0        0   118885 2020-02-02 00:00:00.000000 finqual-0.1.5/finqual/finqual.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 finqual-0.1.5/LICENSE.txt
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 finqual-0.1.5/README.md
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 finqual-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2076 2020-02-02 00:00:00.000000 finqual-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finqual-0.1.6/finqual/__init__.py
+-rw-r--r--   0        0        0   118885 2020-02-02 00:00:00.000000 finqual-0.1.6/finqual/finqual.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 finqual-0.1.6/LICENSE.txt
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 finqual-0.1.6/README.md
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 finqual-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 finqual-0.1.6/PKG-INFO
```

### Comparing `finqual-0.1.5/finqual/finqual.py` & `finqual-0.1.6/finqual/finqual.py`

 * *Files identical despite different names*

### Comparing `finqual-0.1.5/LICENSE.txt` & `finqual-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `finqual-0.1.5/README.md` & `finqual-0.1.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 This has two key features that enable better programmatic access compared to other providers:
 - Ability to call upto 10 requests per second
 - No restriction on the number of calls within a certain timeframe
 
 ## Functions
 First, import the package using:
 ```
-import finqual as fq
+from finqual import finqual as fq
 ```
 From there, use a "Ticker" class to call the desired stock and the desired financial statement. For example:
 ```
 fq.Ticker("TSLA").income(2020,2022)
 fq.Ticker("TSLA").balance(2020,2022, quarter = True)
 fq.Ticker("TSLA").cashflow(2020,2022)
 ```
```

### Comparing `finqual-0.1.5/pyproject.toml` & `finqual-0.1.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "finqual"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Myztika"},
 ]
 description = "A package to retrieve historical fundamental financial data such as income statement, balance sheet and cashflow statement directly from the SEC with no request caps and fast request rate limits"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `finqual-0.1.5/PKG-INFO` & `finqual-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finqual
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package to retrieve historical fundamental financial data such as income statement, balance sheet and cashflow statement directly from the SEC with no request caps and fast request rate limits
 Author: Myztika
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -20,15 +20,15 @@
 This has two key features that enable better programmatic access compared to other providers:
 - Ability to call upto 10 requests per second
 - No restriction on the number of calls within a certain timeframe
 
 ## Functions
 First, import the package using:
 ```
-import finqual as fq
+from finqual import finqual as fq
 ```
 From there, use a "Ticker" class to call the desired stock and the desired financial statement. For example:
 ```
 fq.Ticker("TSLA").income(2020,2022)
 fq.Ticker("TSLA").balance(2020,2022, quarter = True)
 fq.Ticker("TSLA").cashflow(2020,2022)
 ```
```

