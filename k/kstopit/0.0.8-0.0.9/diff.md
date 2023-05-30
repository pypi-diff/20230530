# Comparing `tmp/kstopit-0.0.8.tar.gz` & `tmp/kstopit-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kstopit-0.0.8.tar", last modified: Sun Jan 10 22:50:24 2021, max compression
+gzip compressed data, was "dist/kstopit-0.0.9.tar", last modified: Mon Jan 11 14:45:01 2021, max compression
```

## Comparing `kstopit-0.0.8.tar` & `kstopit-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 kristofk (334975650) 1198310432        0 2021-01-10 22:50:24.694988 kstopit-0.0.8/
--rw-r--r--   0 kristofk (334975650) 1198310432      819 2021-01-10 22:50:24.694591 kstopit-0.0.8/PKG-INFO
--rw-r--r--   0 kristofk (334975650) 1198310432      336 2021-01-10 20:28:36.000000 kstopit-0.0.8/README.md
-drwxr-xr-x   0 kristofk (334975650) 1198310432        0 2021-01-10 22:50:24.691570 kstopit-0.0.8/kstopit/
--rw-r--r--   0 kristofk (334975650) 1198310432       99 2021-01-10 20:40:39.000000 kstopit-0.0.8/kstopit/__init__.py
--rw-r--r--   0 kristofk (334975650) 1198310432     4137 2021-01-10 22:50:10.000000 kstopit-0.0.8/kstopit/kstopit.py
-drwxr-xr-x   0 kristofk (334975650) 1198310432        0 2021-01-10 22:50:24.693941 kstopit-0.0.8/kstopit.egg-info/
--rw-r--r--   0 kristofk (334975650) 1198310432      819 2021-01-10 22:50:24.000000 kstopit-0.0.8/kstopit.egg-info/PKG-INFO
--rw-r--r--   0 kristofk (334975650) 1198310432      211 2021-01-10 22:50:24.000000 kstopit-0.0.8/kstopit.egg-info/SOURCES.txt
--rw-r--r--   0 kristofk (334975650) 1198310432        1 2021-01-10 22:50:24.000000 kstopit-0.0.8/kstopit.egg-info/dependency_links.txt
--rw-r--r--   0 kristofk (334975650) 1198310432        7 2021-01-10 22:50:24.000000 kstopit-0.0.8/kstopit.egg-info/requires.txt
--rw-r--r--   0 kristofk (334975650) 1198310432        8 2021-01-10 22:50:24.000000 kstopit-0.0.8/kstopit.egg-info/top_level.txt
--rw-r--r--   0 kristofk (334975650) 1198310432       38 2021-01-10 22:50:24.695100 kstopit-0.0.8/setup.cfg
--rw-r--r--   0 kristofk (334975650) 1198310432      745 2021-01-10 22:50:22.000000 kstopit-0.0.8/setup.py
+drwxr-xr-x   0 kristofk (334975650) TELENAV\Domain Users (1198310432)        0 2021-01-11 14:45:01.572039 kstopit-0.0.9/
+-rw-r--r--   0 kristofk (334975650) TELENAV\Domain Users (1198310432)      819 2021-01-11 14:45:01.571545 kstopit-0.0.9/PKG-INFO
+-rw-r--r--   0 kristofk (334975650) TELENAV\Domain Users (1198310432)      336 2021-01-10 20:28:36.000000 kstopit-0.0.9/README.md
+drwxr-xr-x   0 kristofk (334975650) TELENAV\Domain Users (1198310432)        0 2021-01-11 14:45:01.569090 kstopit-0.0.9/kstopit/
+-rw-r--r--   0 kristofk (334975650) TELENAV\Domain Users (1198310432)       99 2021-01-10 20:40:39.000000 kstopit-0.0.9/kstopit/__init__.py
+-rw-r--r--   0 kristofk (334975650) TELENAV\Domain Users (1198310432)     4140 2021-01-11 14:44:53.000000 kstopit-0.0.9/kstopit/kstopit.py
+drwxr-xr-x   0 kristofk (334975650) TELENAV\Domain Users (1198310432)        0 2021-01-11 14:45:01.570928 kstopit-0.0.9/kstopit.egg-info/
+-rw-r--r--   0 kristofk (334975650) TELENAV\Domain Users (1198310432)      819 2021-01-11 14:45:01.000000 kstopit-0.0.9/kstopit.egg-info/PKG-INFO
+-rw-r--r--   0 kristofk (334975650) TELENAV\Domain Users (1198310432)      211 2021-01-11 14:45:01.000000 kstopit-0.0.9/kstopit.egg-info/SOURCES.txt
+-rw-r--r--   0 kristofk (334975650) TELENAV\Domain Users (1198310432)        1 2021-01-11 14:45:01.000000 kstopit-0.0.9/kstopit.egg-info/dependency_links.txt
+-rw-r--r--   0 kristofk (334975650) TELENAV\Domain Users (1198310432)        7 2021-01-11 14:45:01.000000 kstopit-0.0.9/kstopit.egg-info/requires.txt
+-rw-r--r--   0 kristofk (334975650) TELENAV\Domain Users (1198310432)        8 2021-01-11 14:45:01.000000 kstopit-0.0.9/kstopit.egg-info/top_level.txt
+-rw-r--r--   0 kristofk (334975650) TELENAV\Domain Users (1198310432)       38 2021-01-11 14:45:01.572191 kstopit-0.0.9/setup.cfg
+-rw-r--r--   0 kristofk (334975650) TELENAV\Domain Users (1198310432)      745 2021-01-11 14:44:59.000000 kstopit-0.0.9/setup.py
```

### Comparing `kstopit-0.0.8/PKG-INFO` & `kstopit-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kstopit
-Version: 0.0.8
+Version: 0.0.9
 Summary: kstopit
 Home-page: https://github.com/kkristof200/py_kstopit
 Author: Kristof
 License: UNKNOWN
 Description: # kstopit
         ![python_version](https://img.shields.io/static/v1?label=Python&message=3.5%20|%203.6%20|%203.7&color=blue) [![PyPI downloads/month](https://img.shields.io/pypi/dm/kstopit?logo=pypi&logoColor=white)](https://pypi.python.org/pypi/kstopit)
```

### Comparing `kstopit-0.0.8/kstopit/kstopit.py` & `kstopit-0.0.9/kstopit/kstopit.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         Union[stopit.TimeoutException, Any]: [description]
     """
 
     def real_decorator(function):
         def wrapper(*args, **kwargs):
             return __run_with_timeout(
                 function,
-                stopit.SignalTimeout,
+                stopit.ThreadingTimeout,
                 name,
                 function_name,
                 timeout_param,
                 *args,
                 **kwargs
             )
```

### Comparing `kstopit-0.0.8/kstopit.egg-info/PKG-INFO` & `kstopit-0.0.9/kstopit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kstopit
-Version: 0.0.8
+Version: 0.0.9
 Summary: kstopit
 Home-page: https://github.com/kkristof200/py_kstopit
 Author: Kristof
 License: UNKNOWN
 Description: # kstopit
         ![python_version](https://img.shields.io/static/v1?label=Python&message=3.5%20|%203.6%20|%203.7&color=blue) [![PyPI downloads/month](https://img.shields.io/pypi/dm/kstopit?logo=pypi&logoColor=white)](https://pypi.python.org/pypi/kstopit)
```

### Comparing `kstopit-0.0.8/setup.py` & `kstopit-0.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open(readme_path, "r") as f:
         long_description = f.read()
 else:
     long_description = 'kstopit'
 
 setuptools.setup(
     name="kstopit",
-    version="0.0.8",
+    version="0.0.9",
     author="Kristof",
     description="kstopit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kkristof200/py_kstopit",
     packages=setuptools.find_packages(),
     install_requires=["stopit"],
```

