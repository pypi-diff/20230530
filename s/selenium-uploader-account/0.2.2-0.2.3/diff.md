# Comparing `tmp/selenium_uploader_account-0.2.2.tar.gz` & `tmp/selenium_uploader_account-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/selenium_uploader_account-0.2.2.tar", last modified: Tue May 30 10:50:16 2023, max compression
+gzip compressed data, was "dist/selenium_uploader_account-0.2.3.tar", last modified: Tue May 30 10:55:42 2023, max compression
```

## Comparing `selenium_uploader_account-0.2.2.tar` & `selenium_uploader_account-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 kristofk (334975650) 1198310432        0 2023-05-30 10:50:16.000000 selenium_uploader_account-0.2.2/
--rw-r--r--   0 kristofk (334975650) 1198310432      825 2023-05-30 10:50:16.000000 selenium_uploader_account-0.2.2/PKG-INFO
--rw-r--r--   0 kristofk (334975650) 1198310432      426 2023-05-30 10:50:08.000000 selenium_uploader_account-0.2.2/README.md
-drwxr-xr-x   0 kristofk (334975650) 1198310432        0 2023-05-30 10:50:16.000000 selenium_uploader_account-0.2.2/selenium_uploader_account/
--rw-r--r--   0 kristofk (334975650) 1198310432       94 2021-09-15 21:11:08.000000 selenium_uploader_account-0.2.2/selenium_uploader_account/__init__.py
--rw-r--r--   0 kristofk (334975650) 1198310432     1150 2021-09-15 21:11:08.000000 selenium_uploader_account-0.2.2/selenium_uploader_account/selenium_uploader_account.py
-drwxr-xr-x   0 kristofk (334975650) 1198310432        0 2023-05-30 10:50:16.000000 selenium_uploader_account-0.2.2/selenium_uploader_account.egg-info/
--rw-r--r--   0 kristofk (334975650) 1198310432      825 2023-05-30 10:50:16.000000 selenium_uploader_account-0.2.2/selenium_uploader_account.egg-info/PKG-INFO
--rw-r--r--   0 kristofk (334975650) 1198310432      355 2023-05-30 10:50:16.000000 selenium_uploader_account-0.2.2/selenium_uploader_account.egg-info/SOURCES.txt
--rw-r--r--   0 kristofk (334975650) 1198310432        1 2023-05-30 10:50:16.000000 selenium_uploader_account-0.2.2/selenium_uploader_account.egg-info/dependency_links.txt
--rw-r--r--   0 kristofk (334975650) 1198310432       43 2023-05-30 10:50:16.000000 selenium_uploader_account-0.2.2/selenium_uploader_account.egg-info/requires.txt
--rw-r--r--   0 kristofk (334975650) 1198310432       26 2023-05-30 10:50:16.000000 selenium_uploader_account-0.2.2/selenium_uploader_account.egg-info/top_level.txt
--rw-r--r--   0 kristofk (334975650) 1198310432       38 2023-05-30 10:50:16.000000 selenium_uploader_account-0.2.2/setup.cfg
--rw-r--r--   0 kristofk (334975650) 1198310432      875 2023-05-30 10:50:08.000000 selenium_uploader_account-0.2.2/setup.py
+drwxr-xr-x   0 kristofk (334975650) 1198310432        0 2023-05-30 10:55:42.000000 selenium_uploader_account-0.2.3/
+-rw-r--r--   0 kristofk (334975650) 1198310432      825 2023-05-30 10:55:42.000000 selenium_uploader_account-0.2.3/PKG-INFO
+-rw-r--r--   0 kristofk (334975650) 1198310432      426 2023-05-30 10:55:36.000000 selenium_uploader_account-0.2.3/README.md
+drwxr-xr-x   0 kristofk (334975650) 1198310432        0 2023-05-30 10:55:42.000000 selenium_uploader_account-0.2.3/selenium_uploader_account/
+-rw-r--r--   0 kristofk (334975650) 1198310432       94 2021-09-15 21:11:08.000000 selenium_uploader_account-0.2.3/selenium_uploader_account/__init__.py
+-rw-r--r--   0 kristofk (334975650) 1198310432     1150 2021-09-15 21:11:08.000000 selenium_uploader_account-0.2.3/selenium_uploader_account/selenium_uploader_account.py
+drwxr-xr-x   0 kristofk (334975650) 1198310432        0 2023-05-30 10:55:42.000000 selenium_uploader_account-0.2.3/selenium_uploader_account.egg-info/
+-rw-r--r--   0 kristofk (334975650) 1198310432      825 2023-05-30 10:55:41.000000 selenium_uploader_account-0.2.3/selenium_uploader_account.egg-info/PKG-INFO
+-rw-r--r--   0 kristofk (334975650) 1198310432      355 2023-05-30 10:55:42.000000 selenium_uploader_account-0.2.3/selenium_uploader_account.egg-info/SOURCES.txt
+-rw-r--r--   0 kristofk (334975650) 1198310432        1 2023-05-30 10:55:41.000000 selenium_uploader_account-0.2.3/selenium_uploader_account.egg-info/dependency_links.txt
+-rw-r--r--   0 kristofk (334975650) 1198310432       43 2023-05-30 10:55:41.000000 selenium_uploader_account-0.2.3/selenium_uploader_account.egg-info/requires.txt
+-rw-r--r--   0 kristofk (334975650) 1198310432       26 2023-05-30 10:55:41.000000 selenium_uploader_account-0.2.3/selenium_uploader_account.egg-info/top_level.txt
+-rw-r--r--   0 kristofk (334975650) 1198310432       38 2023-05-30 10:55:42.000000 selenium_uploader_account-0.2.3/setup.cfg
+-rw-r--r--   0 kristofk (334975650) 1198310432      875 2023-05-30 10:55:36.000000 selenium_uploader_account-0.2.3/setup.py
```

### Comparing `selenium_uploader_account-0.2.2/PKG-INFO` & `selenium_uploader_account-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium_uploader_account
-Version: 0.2.2
+Version: 0.2.3
 Summary: selenium_uploader_account
 Home-page: https://github.com/kkristof200/selenium_uploader_account
 Author: Kristof
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
```

### Comparing `selenium_uploader_account-0.2.2/selenium_uploader_account/selenium_uploader_account.py` & `selenium_uploader_account-0.2.3/selenium_uploader_account/selenium_uploader_account.py`

 * *Files identical despite different names*

### Comparing `selenium_uploader_account-0.2.2/selenium_uploader_account.egg-info/PKG-INFO` & `selenium_uploader_account-0.2.3/selenium_uploader_account.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selenium-uploader-account
-Version: 0.2.2
+Version: 0.2.3
 Summary: selenium_uploader_account
 Home-page: https://github.com/kkristof200/selenium_uploader_account
 Author: Kristof
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
```

### Comparing `selenium_uploader_account-0.2.2/setup.py` & `selenium_uploader_account-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,23 @@
     with open(readme_path, "r") as f:
         long_description = f.read()
 else:
     long_description = 'selenium_uploader_account'
 
 setuptools.setup(
     name="selenium_uploader_account",
-    version="0.2.2",
+    version="0.2.3",
     author="Kristof",
     description="selenium_uploader_account",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kkristof200/selenium_uploader_account",
     packages=setuptools.find_packages(),
     install_requires=[
-        'selenium-account>=0.2.2',
+        'selenium-account>=0.2.3',
         'setuptools>=67.8.0'
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

