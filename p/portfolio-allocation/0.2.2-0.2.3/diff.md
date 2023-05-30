# Comparing `tmp/portfolio_allocation-0.2.2.tar.gz` & `tmp/portfolio_allocation-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portfolio_allocation-0.2.2.tar", last modified: Tue May 30 18:45:45 2023, max compression
+gzip compressed data, was "portfolio_allocation-0.2.3.tar", last modified: Tue May 30 18:50:31 2023, max compression
```

## Comparing `portfolio_allocation-0.2.2.tar` & `portfolio_allocation-0.2.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:45:45.883998 portfolio_allocation-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-30 18:45:45.883998 portfolio_allocation-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:45:45.879999 portfolio_allocation-0.2.2/portfolio_allocation/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/portfolio_allocation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/portfolio_allocation/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/portfolio_allocation/gnucash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:45:45.883998 portfolio_allocation-0.2.2/portfolio_allocation/instruments/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/portfolio_allocation/instruments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/portfolio_allocation/instruments/instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/portfolio_allocation/instruments/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:45:45.883998 portfolio_allocation-0.2.2/portfolio_allocation/instruments/sources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/portfolio_allocation/instruments/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/portfolio_allocation/instruments/sources/currencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/portfolio_allocation/instruments/sources/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/portfolio_allocation/instruments/sources/funds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/portfolio_allocation/instruments/sources/securities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:45:45.883998 portfolio_allocation-0.2.2/portfolio_allocation/report/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/portfolio_allocation/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/portfolio_allocation/report/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:45:45.883998 portfolio_allocation-0.2.2/portfolio_allocation/report/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/portfolio_allocation/report/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/portfolio_allocation/report/resources/main.css
--rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/portfolio_allocation/report/resources/main.js
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/portfolio_allocation/report/resources/report_template.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:45:45.879999 portfolio_allocation-0.2.2/portfolio_allocation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-30 18:45:45.000000 portfolio_allocation-0.2.2/portfolio_allocation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-30 18:45:45.000000 portfolio_allocation-0.2.2/portfolio_allocation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 18:45:45.000000 portfolio_allocation-0.2.2/portfolio_allocation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-30 18:45:45.000000 portfolio_allocation-0.2.2/portfolio_allocation.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-30 18:45:45.000000 portfolio_allocation-0.2.2/portfolio_allocation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-30 18:45:45.000000 portfolio_allocation-0.2.2/portfolio_allocation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 18:45:45.883998 portfolio_allocation-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:50:31.661543 portfolio_allocation-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-30 18:50:31.661543 portfolio_allocation-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:50:31.657543 portfolio_allocation-0.2.3/portfolio_allocation/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/portfolio_allocation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/portfolio_allocation/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/portfolio_allocation/gnucash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:50:31.661543 portfolio_allocation-0.2.3/portfolio_allocation/instruments/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/portfolio_allocation/instruments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/portfolio_allocation/instruments/instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/portfolio_allocation/instruments/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:50:31.661543 portfolio_allocation-0.2.3/portfolio_allocation/instruments/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/portfolio_allocation/instruments/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/portfolio_allocation/instruments/sources/currencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/portfolio_allocation/instruments/sources/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/portfolio_allocation/instruments/sources/funds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/portfolio_allocation/instruments/sources/securities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:50:31.661543 portfolio_allocation-0.2.3/portfolio_allocation/report/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/portfolio_allocation/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/portfolio_allocation/report/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:50:31.661543 portfolio_allocation-0.2.3/portfolio_allocation/report/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/portfolio_allocation/report/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/portfolio_allocation/report/resources/main.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/portfolio_allocation/report/resources/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/portfolio_allocation/report/resources/report_template.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:50:31.657543 portfolio_allocation-0.2.3/portfolio_allocation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-30 18:50:31.000000 portfolio_allocation-0.2.3/portfolio_allocation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-30 18:50:31.000000 portfolio_allocation-0.2.3/portfolio_allocation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 18:50:31.000000 portfolio_allocation-0.2.3/portfolio_allocation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-30 18:50:31.000000 portfolio_allocation-0.2.3/portfolio_allocation.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-30 18:50:31.000000 portfolio_allocation-0.2.3/portfolio_allocation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-30 18:50:31.000000 portfolio_allocation-0.2.3/portfolio_allocation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 18:50:31.665543 portfolio_allocation-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-05-30 18:50:22.000000 portfolio_allocation-0.2.3/setup.py
```

### Comparing `portfolio_allocation-0.2.2/LICENSE` & `portfolio_allocation-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.2/PKG-INFO` & `portfolio_allocation-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portfolio_allocation
-Version: 0.2.2
+Version: 0.2.3
 Summary: Calculates currency, country and industry allocations for portfolio of ETFs and mutual funds
 Home-page: https://github.com/fertkir/portfolio-allocation
 Author: Kirill Fertikov
 Author-email: kirill.fertikov@gmail.com
 Project-URL: Bug Reports, https://github.com/fertkir/portfolio-allocation/issues
 Project-URL: Source, https://github.com/fertkir/portfolio-allocation
 Keywords: etf allocation moex tinkoff finex gnucash
```

### Comparing `portfolio_allocation-0.2.2/README.md` & `portfolio_allocation-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.2/portfolio_allocation/cli.py` & `portfolio_allocation-0.2.3/portfolio_allocation/cli.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.2/portfolio_allocation/gnucash.py` & `portfolio_allocation-0.2.3/portfolio_allocation/gnucash.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.2/portfolio_allocation/instruments/instruments.py` & `portfolio_allocation-0.2.3/portfolio_allocation/instruments/instruments.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.2/portfolio_allocation/instruments/sources/currencies.py` & `portfolio_allocation-0.2.3/portfolio_allocation/instruments/sources/currencies.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.2/portfolio_allocation/instruments/sources/custom.py` & `portfolio_allocation-0.2.3/portfolio_allocation/instruments/sources/custom.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.2/portfolio_allocation/instruments/sources/funds.py` & `portfolio_allocation-0.2.3/portfolio_allocation/instruments/sources/funds.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.2/portfolio_allocation/instruments/sources/securities.py` & `portfolio_allocation-0.2.3/portfolio_allocation/instruments/sources/securities.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.2/portfolio_allocation/report/report.py` & `portfolio_allocation-0.2.3/portfolio_allocation/report/report.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.2/portfolio_allocation/report/resources/main.css` & `portfolio_allocation-0.2.3/portfolio_allocation/report/resources/main.css`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.2/portfolio_allocation/report/resources/main.js` & `portfolio_allocation-0.2.3/portfolio_allocation/report/resources/main.js`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.2/portfolio_allocation.egg-info/PKG-INFO` & `portfolio_allocation-0.2.3/portfolio_allocation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portfolio-allocation
-Version: 0.2.2
+Version: 0.2.3
 Summary: Calculates currency, country and industry allocations for portfolio of ETFs and mutual funds
 Home-page: https://github.com/fertkir/portfolio-allocation
 Author: Kirill Fertikov
 Author-email: kirill.fertikov@gmail.com
 Project-URL: Bug Reports, https://github.com/fertkir/portfolio-allocation/issues
 Project-URL: Source, https://github.com/fertkir/portfolio-allocation
 Keywords: etf allocation moex tinkoff finex gnucash
```

### Comparing `portfolio_allocation-0.2.2/portfolio_allocation.egg-info/SOURCES.txt` & `portfolio_allocation-0.2.3/portfolio_allocation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.2/portfolio_allocation.egg-info/requires.txt` & `portfolio_allocation-0.2.3/portfolio_allocation.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 appdirs==1.4.4
 banal==1.0.6
 cache-to-disk==2.0.0
 cffi==1.15.1
-countrynames==1.14.3
+countrynames==1.15.0
 multitasking==0.0.11
 normality==2.4.0
 pycountry==22.3.5
 pycparser==2.21
 pytz==2023.3
-requests==2.28.2
+requests==2.31.0
 text-unidecode==1.3
 webencodings==0.5.1
-yfinance==0.2.14
+yfinance==0.2.18
 
 [:python_full_version >= "3.6.0"]
-beautifulsoup4==4.12.0
+beautifulsoup4==4.12.2
 
 [:python_full_version >= "3.7.0"]
 charset-normalizer==3.1.0
 
 [:python_version >= "2"]
 tzdata==2023.3
 
@@ -26,32 +26,28 @@
 python-dateutil==2.8.2
 six==1.16.0
 
 [:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4"]
 html5lib==1.1
 lxml==4.9.2
 
-[:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5"]
-urllib3==1.26.15
-
 [:python_version >= "3.5"]
 idna==3.4
 
 [:python_version >= "3.6"]
-certifi==2022.12.7
-cryptography==40.0.1
-frozendict==2.3.6
-levenshtein==0.20.9
-python-levenshtein==0.20.9
+certifi==2023.5.7
+cryptography==40.0.2
+frozendict==2.3.8
 pyyaml==6.0
 
 [:python_version >= "3.7"]
 chardet==5.1.0
-rapidfuzz==2.15.0
-setuptools==67.6.1
-soupsieve==2.4
+jellyfish==0.11.2
+setuptools==67.8.0
+soupsieve==2.4.1
+urllib3==2.0.2
 
 [:python_version >= "3.8"]
-numpy==1.24.2
-pandas==2.0.0
+numpy==1.24.3
+pandas==2.0.2
 
 [dev]
```

### Comparing `portfolio_allocation-0.2.2/setup.py` & `portfolio_allocation-0.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     name="portfolio_allocation",
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="0.2.2",
+    version="0.2.3",
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Calculates currency, country and industry allocations for portfolio of ETFs and mutual funds",
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
@@ -122,15 +122,15 @@
     python_requires=">=3.9",
     # This field lists other packages that your project depends on to run.
     # Any package you put here will be installed by pip when your project is
     # installed, so they must be valid existing projects.
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
-    install_requires=['appdirs==1.4.4', 'banal==1.0.6', "beautifulsoup4==4.12.0; python_full_version >= '3.6.0'", 'cache-to-disk==2.0.0', "certifi==2022.12.7; python_version >= '3.6'", 'cffi==1.15.1', "chardet==5.1.0; python_version >= '3.7'", "charset-normalizer==3.1.0; python_full_version >= '3.7.0'", 'countrynames==1.14.3', "cryptography==40.0.1; python_version >= '3.6'", "frozendict==2.3.6; python_version >= '3.6'", "html5lib==1.1; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'", "idna==3.4; python_version >= '3.5'", "levenshtein==0.20.9; python_version >= '3.6'", "lxml==4.9.2; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'", 'multitasking==0.0.11', 'normality==2.4.0', "numpy==1.24.2; python_version >= '3.8'", "pandas==2.0.0; python_version >= '3.8'", 'pycountry==22.3.5', 'pycparser==2.21', "python-dateutil==2.8.2; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'", "python-levenshtein==0.20.9; python_version >= '3.6'", 'pytz==2023.3', "pyyaml==6.0; python_version >= '3.6'", "rapidfuzz==2.15.0; python_version >= '3.7'", 'requests==2.28.2', "setuptools==67.6.1; python_version >= '3.7'", "six==1.16.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'", "soupsieve==2.4; python_version >= '3.7'", 'text-unidecode==1.3', "tzdata==2023.3; python_version >= '2'", "urllib3==1.26.15; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'", 'webencodings==0.5.1', 'yfinance==0.2.14'],
+    install_requires=['appdirs==1.4.4', 'banal==1.0.6', "beautifulsoup4==4.12.2; python_full_version >= '3.6.0'", 'cache-to-disk==2.0.0', "certifi==2023.5.7; python_version >= '3.6'", 'cffi==1.15.1', "chardet==5.1.0; python_version >= '3.7'", "charset-normalizer==3.1.0; python_full_version >= '3.7.0'", 'countrynames==1.15.0', "cryptography==40.0.2; python_version >= '3.6'", "frozendict==2.3.8; python_version >= '3.6'", "html5lib==1.1; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'", "idna==3.4; python_version >= '3.5'", "jellyfish==0.11.2; python_version >= '3.7'", "lxml==4.9.2; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'", 'multitasking==0.0.11', 'normality==2.4.0', "numpy==1.24.3; python_version >= '3.8'", "pandas==2.0.2; python_version >= '3.8'", 'pycountry==22.3.5', 'pycparser==2.21', "python-dateutil==2.8.2; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'", 'pytz==2023.3', "pyyaml==6.0; python_version >= '3.6'", 'requests==2.31.0', "setuptools==67.8.0; python_version >= '3.7'", "six==1.16.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'", "soupsieve==2.4.1; python_version >= '3.7'", 'text-unidecode==1.3', "tzdata==2023.3; python_version >= '2'", "urllib3==2.0.2; python_version >= '3.7'", 'webencodings==0.5.1', 'yfinance==0.2.18'],
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
     # syntax, for example:
     #
     #   $ pip install sampleproject[dev]
     #
     # Similar to `install_requires` above, these must be valid existing
```

