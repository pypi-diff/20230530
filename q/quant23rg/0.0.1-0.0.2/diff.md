# Comparing `tmp/quant23rg-0.0.1.tar.gz` & `tmp/quant23rg-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quant23rg-0.0.1.tar", last modified: Tue May 30 06:42:43 2023, max compression
+gzip compressed data, was "quant23rg-0.0.2.tar", last modified: Tue May 30 07:04:56 2023, max compression
```

## Comparing `quant23rg-0.0.1.tar` & `quant23rg-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-30 06:42:43.570926 quant23rg-0.0.1/
--rw-r--r--   0 root         (0) staff       (20)     1064 2023-05-30 06:19:05.000000 quant23rg-0.0.1/LICENSE
--rw-r--r--   0 root         (0) staff       (20)     7165 2023-05-30 06:42:43.570721 quant23rg-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     6648 2023-05-30 06:39:31.000000 quant23rg-0.0.1/README.md
--rw-r--r--   0 root         (0) staff       (20)      637 2023-05-30 06:34:33.000000 quant23rg-0.0.1/pyproject.toml
--rw-r--r--   0 root         (0) staff       (20)       38 2023-05-30 06:42:43.570978 quant23rg-0.0.1/setup.cfg
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-30 06:42:43.569534 quant23rg-0.0.1/src/
--rw-r--r--   0 root         (0) staff       (20)      308 2023-05-30 00:33:36.000000 quant23rg-0.0.1/src/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     7631 2023-05-30 06:18:51.000000 quant23rg-0.0.1/src/implied_volatility.py
--rw-r--r--   0 root         (0) staff       (20)      921 2023-05-30 06:18:54.000000 quant23rg-0.0.1/src/pricingBS.py
--rw-r--r--   0 root         (0) staff       (20)     7789 2023-05-30 06:18:56.000000 quant23rg-0.0.1/src/pricingCallEuropBS.py
--rw-r--r--   0 root         (0) staff       (20)    12438 2023-05-30 06:18:58.000000 quant23rg-0.0.1/src/pricingGBM.py
--rw-r--r--   0 root         (0) staff       (20)     5233 2023-05-30 06:19:01.000000 quant23rg-0.0.1/src/pricingPutEuropBS.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-30 06:42:43.570510 quant23rg-0.0.1/src/quant23rg.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     7165 2023-05-30 06:42:43.000000 quant23rg-0.0.1/src/quant23rg.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      330 2023-05-30 06:42:43.000000 quant23rg-0.0.1/src/quant23rg.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-05-30 06:42:43.000000 quant23rg-0.0.1/src/quant23rg.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)      112 2023-05-30 06:42:43.000000 quant23rg-0.0.1/src/quant23rg.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)    21909 2023-05-30 06:19:03.000000 quant23rg-0.0.1/src/riskManagement.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-30 07:04:56.190629 quant23rg-0.0.2/
+-rw-r--r--   0 root         (0) staff       (20)     1064 2023-05-30 06:19:05.000000 quant23rg-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)     7165 2023-05-30 07:04:56.190451 quant23rg-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     6648 2023-05-30 06:39:31.000000 quant23rg-0.0.2/README.md
+-rw-r--r--   0 root         (0) staff       (20)      660 2023-05-30 07:04:31.000000 quant23rg-0.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-05-30 07:04:56.190684 quant23rg-0.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-30 07:04:56.186392 quant23rg-0.0.2/src/
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-30 07:04:56.189220 quant23rg-0.0.2/src/quant23rg/
+-rw-r--r--   0 root         (0) staff       (20)      308 2023-05-30 00:33:36.000000 quant23rg-0.0.2/src/quant23rg/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     7631 2023-05-30 06:18:51.000000 quant23rg-0.0.2/src/quant23rg/implied_volatility.py
+-rw-r--r--   0 root         (0) staff       (20)      921 2023-05-30 06:18:54.000000 quant23rg-0.0.2/src/quant23rg/pricingBS.py
+-rw-r--r--   0 root         (0) staff       (20)     7789 2023-05-30 06:18:56.000000 quant23rg-0.0.2/src/quant23rg/pricingCallEuropBS.py
+-rw-r--r--   0 root         (0) staff       (20)    12438 2023-05-30 06:18:58.000000 quant23rg-0.0.2/src/quant23rg/pricingGBM.py
+-rw-r--r--   0 root         (0) staff       (20)     5233 2023-05-30 06:19:01.000000 quant23rg-0.0.2/src/quant23rg/pricingPutEuropBS.py
+-rw-r--r--   0 root         (0) staff       (20)    21909 2023-05-30 06:19:03.000000 quant23rg-0.0.2/src/quant23rg/riskManagement.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-30 07:04:56.190248 quant23rg-0.0.2/src/quant23rg.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     7165 2023-05-30 07:04:56.000000 quant23rg-0.0.2/src/quant23rg.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      400 2023-05-30 07:04:56.000000 quant23rg-0.0.2/src/quant23rg.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-30 07:04:56.000000 quant23rg-0.0.2/src/quant23rg.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       10 2023-05-30 07:04:56.000000 quant23rg-0.0.2/src/quant23rg.egg-info/top_level.txt
```

### Comparing `quant23rg-0.0.1/LICENSE` & `quant23rg-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quant23rg-0.0.1/PKG-INFO` & `quant23rg-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quant23rg
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package for quantitative analysis
 Author-email: Adrien Calas <le23rg@icloud.com>
 Project-URL: Homepage, https://github.com/leRayGorbella/quant23rg
 Project-URL: Bug Tracker, https://github.com/leRayGorbella/quant23rg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quant23rg-0.0.1/README.md` & `quant23rg-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `quant23rg-0.0.1/pyproject.toml` & `quant23rg-0.0.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=61.0", "yfinance>=0.1.70", "plotly>=5.6.0", "pandas"]
+requires = ["setuptools>=61.0", "yfinance>=0.1.70", "plotly>=5.6.0", "pandas>=1.3.4", "scipy>=1.8.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quant23rg"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Adrien Calas", email="le23rg@icloud.com" },
 ]
 description = "Package for quantitative analysis"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `quant23rg-0.0.1/src/implied_volatility.py` & `quant23rg-0.0.2/src/quant23rg/implied_volatility.py`

 * *Files identical despite different names*

### Comparing `quant23rg-0.0.1/src/pricingBS.py` & `quant23rg-0.0.2/src/quant23rg/pricingBS.py`

 * *Files identical despite different names*

### Comparing `quant23rg-0.0.1/src/pricingCallEuropBS.py` & `quant23rg-0.0.2/src/quant23rg/pricingCallEuropBS.py`

 * *Files identical despite different names*

### Comparing `quant23rg-0.0.1/src/pricingGBM.py` & `quant23rg-0.0.2/src/quant23rg/pricingGBM.py`

 * *Files identical despite different names*

### Comparing `quant23rg-0.0.1/src/pricingPutEuropBS.py` & `quant23rg-0.0.2/src/quant23rg/pricingPutEuropBS.py`

 * *Files identical despite different names*

### Comparing `quant23rg-0.0.1/src/quant23rg.egg-info/PKG-INFO` & `quant23rg-0.0.2/src/quant23rg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quant23rg
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package for quantitative analysis
 Author-email: Adrien Calas <le23rg@icloud.com>
 Project-URL: Homepage, https://github.com/leRayGorbella/quant23rg
 Project-URL: Bug Tracker, https://github.com/leRayGorbella/quant23rg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quant23rg-0.0.1/src/riskManagement.py` & `quant23rg-0.0.2/src/quant23rg/riskManagement.py`

 * *Files identical despite different names*

