# Comparing `tmp/portfolio_allocation-0.2.1.tar.gz` & `tmp/portfolio_allocation-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portfolio_allocation-0.2.1.tar", last modified: Sat Apr 29 06:19:29 2023, max compression
+gzip compressed data, was "portfolio_allocation-0.2.2.tar", last modified: Tue May 30 18:45:45 2023, max compression
```

## Comparing `portfolio_allocation-0.2.1.tar` & `portfolio_allocation-0.2.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:19:29.043043 portfolio_allocation-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-04-29 06:19:29.043043 portfolio_allocation-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:19:29.035043 portfolio_allocation-0.2.1/portfolio_allocation/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/portfolio_allocation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/portfolio_allocation/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/portfolio_allocation/gnucash.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:19:29.039044 portfolio_allocation-0.2.1/portfolio_allocation/instruments/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/portfolio_allocation/instruments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/portfolio_allocation/instruments/instruments.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/portfolio_allocation/instruments/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:19:29.043043 portfolio_allocation-0.2.1/portfolio_allocation/instruments/sources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/portfolio_allocation/instruments/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/portfolio_allocation/instruments/sources/currencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/portfolio_allocation/instruments/sources/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/portfolio_allocation/instruments/sources/funds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/portfolio_allocation/instruments/sources/securities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:19:29.043043 portfolio_allocation-0.2.1/portfolio_allocation/report/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/portfolio_allocation/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/portfolio_allocation/report/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:19:29.043043 portfolio_allocation-0.2.1/portfolio_allocation/report/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/portfolio_allocation/report/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/portfolio_allocation/report/resources/main.css
--rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/portfolio_allocation/report/resources/main.js
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/portfolio_allocation/report/resources/report_template.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 06:19:29.039044 portfolio_allocation-0.2.1/portfolio_allocation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-04-29 06:19:29.000000 portfolio_allocation-0.2.1/portfolio_allocation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-29 06:19:29.000000 portfolio_allocation-0.2.1/portfolio_allocation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 06:19:29.000000 portfolio_allocation-0.2.1/portfolio_allocation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-29 06:19:29.000000 portfolio_allocation-0.2.1/portfolio_allocation.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-29 06:19:29.000000 portfolio_allocation-0.2.1/portfolio_allocation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-29 06:19:29.000000 portfolio_allocation-0.2.1/portfolio_allocation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 06:19:29.043043 portfolio_allocation-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-04-29 06:19:17.000000 portfolio_allocation-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:45:45.883998 portfolio_allocation-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-30 18:45:45.883998 portfolio_allocation-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:45:45.879999 portfolio_allocation-0.2.2/portfolio_allocation/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/portfolio_allocation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/portfolio_allocation/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/portfolio_allocation/gnucash.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:45:45.883998 portfolio_allocation-0.2.2/portfolio_allocation/instruments/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/portfolio_allocation/instruments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/portfolio_allocation/instruments/instruments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/portfolio_allocation/instruments/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:45:45.883998 portfolio_allocation-0.2.2/portfolio_allocation/instruments/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/portfolio_allocation/instruments/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/portfolio_allocation/instruments/sources/currencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/portfolio_allocation/instruments/sources/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/portfolio_allocation/instruments/sources/funds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/portfolio_allocation/instruments/sources/securities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:45:45.883998 portfolio_allocation-0.2.2/portfolio_allocation/report/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/portfolio_allocation/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/portfolio_allocation/report/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:45:45.883998 portfolio_allocation-0.2.2/portfolio_allocation/report/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/portfolio_allocation/report/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/portfolio_allocation/report/resources/main.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7189 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/portfolio_allocation/report/resources/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/portfolio_allocation/report/resources/report_template.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:45:45.879999 portfolio_allocation-0.2.2/portfolio_allocation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-30 18:45:45.000000 portfolio_allocation-0.2.2/portfolio_allocation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-30 18:45:45.000000 portfolio_allocation-0.2.2/portfolio_allocation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 18:45:45.000000 portfolio_allocation-0.2.2/portfolio_allocation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-30 18:45:45.000000 portfolio_allocation-0.2.2/portfolio_allocation.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-30 18:45:45.000000 portfolio_allocation-0.2.2/portfolio_allocation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-30 18:45:45.000000 portfolio_allocation-0.2.2/portfolio_allocation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 18:45:45.883998 portfolio_allocation-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-05-30 18:45:34.000000 portfolio_allocation-0.2.2/setup.py
```

### Comparing `portfolio_allocation-0.2.1/LICENSE` & `portfolio_allocation-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.1/PKG-INFO` & `portfolio_allocation-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portfolio_allocation
-Version: 0.2.1
+Version: 0.2.2
 Summary: Calculates currency, country and industry allocations for portfolio of ETFs and mutual funds
 Home-page: https://github.com/fertkir/portfolio-allocation
 Author: Kirill Fertikov
 Author-email: kirill.fertikov@gmail.com
 Project-URL: Bug Reports, https://github.com/fertkir/portfolio-allocation/issues
 Project-URL: Source, https://github.com/fertkir/portfolio-allocation
 Keywords: etf allocation moex tinkoff finex gnucash
```

### Comparing `portfolio_allocation-0.2.1/README.md` & `portfolio_allocation-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.1/portfolio_allocation/cli.py` & `portfolio_allocation-0.2.2/portfolio_allocation/cli.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.1/portfolio_allocation/gnucash.py` & `portfolio_allocation-0.2.2/portfolio_allocation/gnucash.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.1/portfolio_allocation/instruments/instruments.py` & `portfolio_allocation-0.2.2/portfolio_allocation/instruments/instruments.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.1/portfolio_allocation/instruments/sources/currencies.py` & `portfolio_allocation-0.2.2/portfolio_allocation/instruments/sources/currencies.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.1/portfolio_allocation/instruments/sources/custom.py` & `portfolio_allocation-0.2.2/portfolio_allocation/instruments/sources/custom.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.1/portfolio_allocation/instruments/sources/funds.py` & `portfolio_allocation-0.2.2/portfolio_allocation/instruments/sources/funds.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 def _tinkoff(instrument: str) -> dict:
     url = "https://www.tinkoff.ru/invest/etfs/" + instrument
     print("Sending request GET " + url)
     start = time.time()
     r = requests.get(url)
     print("Got response in " + str(time.time() - start) + " seconds")
     r.encoding = 'UTF-8'
-    group = re.search("<script>window\\['__REACT_QUERY_STATE__invest'] = '(.*)'</script>", r.text).group(1) \
+    group = re.search("<script id=\"__REACT_QUERY_STATE__invest\" type=\"application/json\">(.*)</script><script>", r.text).group(1) \
         .replace('\\\\"', '')
     data = json.loads(group)
     try:
         response_data = data['queries'][0]['state']['data']['detail']
     except IndexError:
         raise _InstrumentMissingException
     return asdict(InstrumentData(
```

### Comparing `portfolio_allocation-0.2.1/portfolio_allocation/instruments/sources/securities.py` & `portfolio_allocation-0.2.2/portfolio_allocation/instruments/sources/securities.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.1/portfolio_allocation/report/report.py` & `portfolio_allocation-0.2.2/portfolio_allocation/report/report.py`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.1/portfolio_allocation/report/resources/main.css` & `portfolio_allocation-0.2.2/portfolio_allocation/report/resources/main.css`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.1/portfolio_allocation/report/resources/main.js` & `portfolio_allocation-0.2.2/portfolio_allocation/report/resources/main.js`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.1/portfolio_allocation.egg-info/PKG-INFO` & `portfolio_allocation-0.2.2/portfolio_allocation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portfolio-allocation
-Version: 0.2.1
+Version: 0.2.2
 Summary: Calculates currency, country and industry allocations for portfolio of ETFs and mutual funds
 Home-page: https://github.com/fertkir/portfolio-allocation
 Author: Kirill Fertikov
 Author-email: kirill.fertikov@gmail.com
 Project-URL: Bug Reports, https://github.com/fertkir/portfolio-allocation/issues
 Project-URL: Source, https://github.com/fertkir/portfolio-allocation
 Keywords: etf allocation moex tinkoff finex gnucash
```

### Comparing `portfolio_allocation-0.2.1/portfolio_allocation.egg-info/SOURCES.txt` & `portfolio_allocation-0.2.2/portfolio_allocation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.1/portfolio_allocation.egg-info/requires.txt` & `portfolio_allocation-0.2.2/portfolio_allocation.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `portfolio_allocation-0.2.1/setup.py` & `portfolio_allocation-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     name="portfolio_allocation",
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="0.2.1",
+    version="0.2.2",
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Calculates currency, country and industry allocations for portfolio of ETFs and mutual funds",
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

