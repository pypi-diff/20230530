# Comparing `tmp/mypy-boto3-polly-1.26.61.tar.gz` & `tmp/mypy-boto3-polly-1.26.69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-polly-1.26.61.tar", last modified: Tue Jan 31 20:49:57 2023, max compression
+gzip compressed data, was "mypy-boto3-polly-1.26.69.tar", last modified: Fri Feb 10 20:27:29 2023, max compression
```

## Comparing `mypy-boto3-polly-1.26.61.tar` & `mypy-boto3-polly-1.26.69.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:57.166170 mypy-boto3-polly-1.26.61/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-31 20:48:56.000000 mypy-boto3-polly-1.26.61/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13899 2023-01-31 20:49:57.162170 mypy-boto3-polly-1.26.61/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-01-31 20:48:56.000000 mypy-boto3-polly-1.26.61/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:57.158170 mypy-boto3-polly-1.26.61/mypy_boto3_polly/
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-01-31 20:48:56.000000 mypy-boto3-polly-1.26.61/mypy_boto3_polly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-01-31 20:48:56.000000 mypy-boto3-polly-1.26.61/mypy_boto3_polly/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-01-31 20:48:56.000000 mypy-boto3-polly-1.26.61/mypy_boto3_polly/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-01-31 20:48:56.000000 mypy-boto3-polly-1.26.61/mypy_boto3_polly/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-01-31 20:48:56.000000 mypy-boto3-polly-1.26.61/mypy_boto3_polly/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10280 2023-01-31 20:48:56.000000 mypy-boto3-polly-1.26.61/mypy_boto3_polly/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10278 2023-01-31 20:48:56.000000 mypy-boto3-polly-1.26.61/mypy_boto3_polly/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-01-31 20:48:56.000000 mypy-boto3-polly-1.26.61/mypy_boto3_polly/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-01-31 20:48:56.000000 mypy-boto3-polly-1.26.61/mypy_boto3_polly/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 20:48:56.000000 mypy-boto3-polly-1.26.61/mypy_boto3_polly/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8900 2023-01-31 20:48:56.000000 mypy-boto3-polly-1.26.61/mypy_boto3_polly/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-01-31 20:48:56.000000 mypy-boto3-polly-1.26.61/mypy_boto3_polly/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-31 20:48:56.000000 mypy-boto3-polly-1.26.61/mypy_boto3_polly/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 20:49:57.162170 mypy-boto3-polly-1.26.61/mypy_boto3_polly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13899 2023-01-31 20:49:56.000000 mypy-boto3-polly-1.26.61/mypy_boto3_polly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-01-31 20:49:56.000000 mypy-boto3-polly-1.26.61/mypy_boto3_polly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 20:49:56.000000 mypy-boto3-polly-1.26.61/mypy_boto3_polly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 20:49:56.000000 mypy-boto3-polly-1.26.61/mypy_boto3_polly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-31 20:49:56.000000 mypy-boto3-polly-1.26.61/mypy_boto3_polly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-31 20:49:56.000000 mypy-boto3-polly-1.26.61/mypy_boto3_polly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 20:49:57.166170 mypy-boto3-polly-1.26.61/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-01-31 20:48:55.000000 mypy-boto3-polly-1.26.61/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 20:27:29.498390 mypy-boto3-polly-1.26.69/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-10 20:26:53.000000 mypy-boto3-polly-1.26.69/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13899 2023-02-10 20:27:29.490389 mypy-boto3-polly-1.26.69/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12420 2023-02-10 20:26:53.000000 mypy-boto3-polly-1.26.69/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 20:27:29.490389 mypy-boto3-polly-1.26.69/mypy_boto3_polly/
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-02-10 20:26:53.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-02-10 20:26:53.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-02-10 20:26:53.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11430 2023-02-10 20:26:53.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11411 2023-02-10 20:26:53.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10308 2023-02-10 20:26:54.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-02-10 20:26:53.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-02-10 20:26:53.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-02-10 20:26:53.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 20:26:53.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8900 2023-02-10 20:26:54.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-02-10 20:26:54.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-10 20:26:53.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 20:27:29.490389 mypy-boto3-polly-1.26.69/mypy_boto3_polly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13899 2023-02-10 20:27:29.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-02-10 20:27:29.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 20:27:29.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 20:27:29.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-10 20:27:29.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-10 20:27:29.000000 mypy-boto3-polly-1.26.69/mypy_boto3_polly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-10 20:27:29.498390 mypy-boto3-polly-1.26.69/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-02-10 20:26:53.000000 mypy-boto3-polly-1.26.69/setup.py
```

### Comparing `mypy-boto3-polly-1.26.61/LICENSE` & `mypy-boto3-polly-1.26.69/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.26.61/PKG-INFO` & `mypy-boto3-polly-1.26.69/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-polly
-Version: 1.26.61
-Summary: Type annotations for boto3.Polly 1.26.61 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.69
+Summary: Type annotations for boto3.Polly 1.26.69 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-polly.svg?color=blue)](https://pypi.org/project/mypy-boto3-polly)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-polly?color=blue)](https://pypistats.org/packages/mypy-boto3-polly)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Polly 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
+[boto3.Polly 1.26.69](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-polly-1.26.61/README.md` & `mypy-boto3-polly-1.26.69/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-polly.svg?color=blue)](https://pypi.org/project/mypy-boto3-polly)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-polly?color=blue)](https://pypistats.org/packages/mypy-boto3-polly)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Polly 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
+[boto3.Polly 1.26.69](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-polly-1.26.61/mypy_boto3_polly/__init__.py` & `mypy-boto3-polly-1.26.69/mypy_boto3_polly/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.26.61/mypy_boto3_polly/__init__.pyi` & `mypy-boto3-polly-1.26.69/mypy_boto3_polly/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.26.61/mypy_boto3_polly/__main__.py` & `mypy-boto3-polly-1.26.69/mypy_boto3_polly/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Polly 1.26.61\nVersion:         1.26.61\nBuilder version:"
+        "Type annotations for boto3.Polly 1.26.69\nVersion:         1.26.69\nBuilder version:"
         " 7.12.3\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.61")
+    print("1.26.69")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-polly-1.26.61/mypy_boto3_polly/client.py` & `mypy-boto3-polly-1.26.69/mypy_boto3_polly/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.26.61/mypy_boto3_polly/client.pyi` & `mypy-boto3-polly-1.26.69/mypy_boto3_polly/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.26.61/mypy_boto3_polly/literals.py` & `mypy-boto3-polly-1.26.69/mypy_boto3_polly/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,14 +126,15 @@
     "Jacek",
     "Jan",
     "Joanna",
     "Joey",
     "Justin",
     "Kajal",
     "Karl",
+    "Kazuha",
     "Kendra",
     "Kevin",
     "Kimberly",
     "Laura",
     "Lea",
     "Liam",
     "Liv",
@@ -165,14 +166,15 @@
     "Seoyeon",
     "Sergio",
     "Stephen",
     "Suvi",
     "Takumi",
     "Tatyana",
     "Thiago",
+    "Tomoko",
     "Vicki",
     "Vitoria",
     "Zeina",
     "Zhiyu",
 ]
 PollyServiceName = Literal["polly"]
 ServiceName = Literal[
```

### Comparing `mypy-boto3-polly-1.26.61/mypy_boto3_polly/literals.pyi` & `mypy-boto3-polly-1.26.69/mypy_boto3_polly/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -124,14 +124,15 @@
     "Jacek",
     "Jan",
     "Joanna",
     "Joey",
     "Justin",
     "Kajal",
     "Karl",
+    "Kazuha",
     "Kendra",
     "Kevin",
     "Kimberly",
     "Laura",
     "Lea",
     "Liam",
     "Liv",
@@ -163,14 +164,15 @@
     "Seoyeon",
     "Sergio",
     "Stephen",
     "Suvi",
     "Takumi",
     "Tatyana",
     "Thiago",
+    "Tomoko",
     "Vicki",
     "Vitoria",
     "Zeina",
     "Zhiyu",
 ]
 PollyServiceName = Literal["polly"]
 ServiceName = Literal[
```

### Comparing `mypy-boto3-polly-1.26.61/mypy_boto3_polly/paginator.py` & `mypy-boto3-polly-1.26.69/mypy_boto3_polly/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.26.61/mypy_boto3_polly/paginator.pyi` & `mypy-boto3-polly-1.26.69/mypy_boto3_polly/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.26.61/mypy_boto3_polly/type_defs.py` & `mypy-boto3-polly-1.26.69/mypy_boto3_polly/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.26.61/mypy_boto3_polly/type_defs.pyi` & `mypy-boto3-polly-1.26.69/mypy_boto3_polly/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.26.61/mypy_boto3_polly.egg-info/PKG-INFO` & `mypy-boto3-polly-1.26.69/mypy_boto3_polly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-polly
-Version: 1.26.61
-Summary: Type annotations for boto3.Polly 1.26.61 service generated with mypy-boto3-builder 7.12.3
+Version: 1.26.69
+Summary: Type annotations for boto3.Polly 1.26.69 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_polly/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-polly.svg?color=blue)](https://pypi.org/project/mypy-boto3-polly)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-polly?color=blue)](https://pypistats.org/packages/mypy-boto3-polly)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Polly 1.26.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
+[boto3.Polly 1.26.69](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-polly-1.26.61/mypy_boto3_polly.egg-info/SOURCES.txt` & `mypy-boto3-polly-1.26.69/mypy_boto3_polly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-polly-1.26.61/setup.py` & `mypy-boto3-polly-1.26.69/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-polly",
-    version="1.26.61",
+    version="1.26.69",
     packages=["mypy_boto3_polly"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Polly 1.26.61 service generated with mypy-boto3-builder 7.12.3"
+        "Type annotations for boto3.Polly 1.26.69 service generated with mypy-boto3-builder 7.12.3"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

