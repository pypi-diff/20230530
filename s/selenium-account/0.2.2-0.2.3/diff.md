# Comparing `tmp/selenium_account-0.2.2.tar.gz` & `tmp/selenium_account-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/selenium_account-0.2.2.tar", last modified: Tue May 30 10:48:57 2023, max compression
+gzip compressed data, was "dist/selenium_account-0.2.3.tar", last modified: Tue May 30 10:55:04 2023, max compression
```

## Comparing `selenium_account-0.2.2.tar` & `selenium_account-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 kristofk (334975650) 1198310432        0 2023-05-30 10:48:57.000000 selenium_account-0.2.2/
--rw-r--r--   0 kristofk (334975650) 1198310432     1080 2021-09-15 21:09:31.000000 selenium_account-0.2.2/LICENSE
--rw-r--r--   0 kristofk (334975650) 1198310432      775 2023-05-30 10:48:57.000000 selenium_account-0.2.2/PKG-INFO
--rw-r--r--   0 kristofk (334975650) 1198310432      381 2023-05-30 10:48:48.000000 selenium_account-0.2.2/README.md
-drwxr-xr-x   0 kristofk (334975650) 1198310432        0 2023-05-30 10:48:57.000000 selenium_account-0.2.2/selenium_account/
--rw-r--r--   0 kristofk (334975650) 1198310432       77 2021-09-15 21:09:31.000000 selenium_account-0.2.2/selenium_account/__init__.py
--rw-r--r--   0 kristofk (334975650) 1198310432     8349 2021-09-15 21:09:31.000000 selenium_account-0.2.2/selenium_account/selenium_account.py
-drwxr-xr-x   0 kristofk (334975650) 1198310432        0 2023-05-30 10:48:57.000000 selenium_account-0.2.2/selenium_account.egg-info/
--rw-r--r--   0 kristofk (334975650) 1198310432      775 2023-05-30 10:48:57.000000 selenium_account-0.2.2/selenium_account.egg-info/PKG-INFO
--rw-r--r--   0 kristofk (334975650) 1198310432      291 2023-05-30 10:48:57.000000 selenium_account-0.2.2/selenium_account.egg-info/SOURCES.txt
--rw-r--r--   0 kristofk (334975650) 1198310432        1 2023-05-30 10:48:57.000000 selenium_account-0.2.2/selenium_account.egg-info/dependency_links.txt
--rw-r--r--   0 kristofk (334975650) 1198310432       92 2023-05-30 10:48:57.000000 selenium_account-0.2.2/selenium_account.egg-info/requires.txt
--rw-r--r--   0 kristofk (334975650) 1198310432       17 2023-05-30 10:48:57.000000 selenium_account-0.2.2/selenium_account.egg-info/top_level.txt
--rw-r--r--   0 kristofk (334975650) 1198310432       38 2023-05-30 10:48:57.000000 selenium_account-0.2.2/setup.cfg
--rw-r--r--   0 kristofk (334975650) 1198310432      921 2023-05-30 10:48:48.000000 selenium_account-0.2.2/setup.py
+drwxr-xr-x   0 kristofk (334975650) 1198310432        0 2023-05-30 10:55:04.000000 selenium_account-0.2.3/
+-rw-r--r--   0 kristofk (334975650) 1198310432     1080 2021-09-15 21:09:31.000000 selenium_account-0.2.3/LICENSE
+-rw-r--r--   0 kristofk (334975650) 1198310432      775 2023-05-30 10:55:04.000000 selenium_account-0.2.3/PKG-INFO
+-rw-r--r--   0 kristofk (334975650) 1198310432      381 2023-05-30 10:54:58.000000 selenium_account-0.2.3/README.md
+drwxr-xr-x   0 kristofk (334975650) 1198310432        0 2023-05-30 10:55:04.000000 selenium_account-0.2.3/selenium_account/
+-rw-r--r--   0 kristofk (334975650) 1198310432       77 2021-09-15 21:09:31.000000 selenium_account-0.2.3/selenium_account/__init__.py
+-rw-r--r--   0 kristofk (334975650) 1198310432     8349 2021-09-15 21:09:31.000000 selenium_account-0.2.3/selenium_account/selenium_account.py
+drwxr-xr-x   0 kristofk (334975650) 1198310432        0 2023-05-30 10:55:04.000000 selenium_account-0.2.3/selenium_account.egg-info/
+-rw-r--r--   0 kristofk (334975650) 1198310432      775 2023-05-30 10:55:04.000000 selenium_account-0.2.3/selenium_account.egg-info/PKG-INFO
+-rw-r--r--   0 kristofk (334975650) 1198310432      291 2023-05-30 10:55:04.000000 selenium_account-0.2.3/selenium_account.egg-info/SOURCES.txt
+-rw-r--r--   0 kristofk (334975650) 1198310432        1 2023-05-30 10:55:04.000000 selenium_account-0.2.3/selenium_account.egg-info/dependency_links.txt
+-rw-r--r--   0 kristofk (334975650) 1198310432       92 2023-05-30 10:55:04.000000 selenium_account-0.2.3/selenium_account.egg-info/requires.txt
+-rw-r--r--   0 kristofk (334975650) 1198310432       17 2023-05-30 10:55:04.000000 selenium_account-0.2.3/selenium_account.egg-info/top_level.txt
+-rw-r--r--   0 kristofk (334975650) 1198310432       38 2023-05-30 10:55:04.000000 selenium_account-0.2.3/setup.cfg
+-rw-r--r--   0 kristofk (334975650) 1198310432      921 2023-05-30 10:54:58.000000 selenium_account-0.2.3/setup.py
```

### Comparing `selenium_account-0.2.2/LICENSE` & `selenium_account-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `selenium_account-0.2.2/PKG-INFO` & `selenium_account-0.2.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium_account
-Version: 0.2.2
+Version: 0.2.3
 Summary: selenium_account
 Home-page: https://github.com/kkristof200/selenium_account
 Author: Kristof
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
```

### Comparing `selenium_account-0.2.2/selenium_account/selenium_account.py` & `selenium_account-0.2.3/selenium_account/selenium_account.py`

 * *Files identical despite different names*

### Comparing `selenium_account-0.2.2/selenium_account.egg-info/PKG-INFO` & `selenium_account-0.2.3/selenium_account.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-account
-Version: 0.2.2
+Version: 0.2.3
 Summary: selenium_account
 Home-page: https://github.com/kkristof200/selenium_account
 Author: Kristof
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
```

### Comparing `selenium_account-0.2.2/setup.py` & `selenium_account-0.2.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,24 +5,24 @@
     with open(readme_path, "r") as f:
         long_description = f.read()
 else:
     long_description = 'selenium_account'
 
 setuptools.setup(
     name="selenium_account",
-    version="0.2.2",
+    version="0.2.3",
     author="Kristof",
     description="selenium_account",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kkristof200/selenium_account",
     packages=setuptools.find_packages(),
     install_requires=[
         'kproxy>=0.0.1',
-        'kstopit>=0.0.13',
+        'kstopit>=0.0.16',
         'selenium-browser>=0.0.12',
         'setuptools>=67.8.0',
         'tldextract>=3.1.2'
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

