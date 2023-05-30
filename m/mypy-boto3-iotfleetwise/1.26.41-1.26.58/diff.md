# Comparing `tmp/mypy-boto3-iotfleetwise-1.26.41.tar.gz` & `tmp/mypy-boto3-iotfleetwise-1.26.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotfleetwise-1.26.41.tar", last modified: Fri Dec 30 20:24:34 2022, max compression
+gzip compressed data, was "mypy-boto3-iotfleetwise-1.26.58.tar", last modified: Thu Jan 26 20:25:02 2023, max compression
```

## Comparing `mypy-boto3-iotfleetwise-1.26.41.tar` & `mypy-boto3-iotfleetwise-1.26.58.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 20:24:34.909745 mypy-boto3-iotfleetwise-1.26.41/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2022-12-30 20:24:23.000000 mypy-boto3-iotfleetwise-1.26.41/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21301 2022-12-30 20:24:34.901745 mypy-boto3-iotfleetwise-1.26.41/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19794 2022-12-30 20:24:23.000000 mypy-boto3-iotfleetwise-1.26.41/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 20:24:34.901745 mypy-boto3-iotfleetwise-1.26.41/mypy_boto3_iotfleetwise/
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2022-12-30 20:24:23.000000 mypy-boto3-iotfleetwise-1.26.41/mypy_boto3_iotfleetwise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2022-12-30 20:24:23.000000 mypy-boto3-iotfleetwise-1.26.41/mypy_boto3_iotfleetwise/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2022-12-30 20:24:23.000000 mypy-boto3-iotfleetwise-1.26.41/mypy_boto3_iotfleetwise/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40949 2022-12-30 20:24:23.000000 mypy-boto3-iotfleetwise-1.26.41/mypy_boto3_iotfleetwise/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40879 2022-12-30 20:24:23.000000 mypy-boto3-iotfleetwise-1.26.41/mypy_boto3_iotfleetwise/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10972 2022-12-30 20:24:23.000000 mypy-boto3-iotfleetwise-1.26.41/mypy_boto3_iotfleetwise/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10970 2022-12-30 20:24:23.000000 mypy-boto3-iotfleetwise-1.26.41/mypy_boto3_iotfleetwise/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15488 2022-12-30 20:24:23.000000 mypy-boto3-iotfleetwise-1.26.41/mypy_boto3_iotfleetwise/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15473 2022-12-30 20:24:23.000000 mypy-boto3-iotfleetwise-1.26.41/mypy_boto3_iotfleetwise/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-30 20:24:23.000000 mypy-boto3-iotfleetwise-1.26.41/mypy_boto3_iotfleetwise/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    57068 2022-12-30 20:24:25.000000 mypy-boto3-iotfleetwise-1.26.41/mypy_boto3_iotfleetwise/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    56968 2022-12-30 20:24:24.000000 mypy-boto3-iotfleetwise-1.26.41/mypy_boto3_iotfleetwise/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-30 20:24:23.000000 mypy-boto3-iotfleetwise-1.26.41/mypy_boto3_iotfleetwise/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-30 20:24:34.901745 mypy-boto3-iotfleetwise-1.26.41/mypy_boto3_iotfleetwise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21301 2022-12-30 20:24:34.000000 mypy-boto3-iotfleetwise-1.26.41/mypy_boto3_iotfleetwise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2022-12-30 20:24:34.000000 mypy-boto3-iotfleetwise-1.26.41/mypy_boto3_iotfleetwise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-30 20:24:34.000000 mypy-boto3-iotfleetwise-1.26.41/mypy_boto3_iotfleetwise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-30 20:24:34.000000 mypy-boto3-iotfleetwise-1.26.41/mypy_boto3_iotfleetwise.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2022-12-30 20:24:34.000000 mypy-boto3-iotfleetwise-1.26.41/mypy_boto3_iotfleetwise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2022-12-30 20:24:34.000000 mypy-boto3-iotfleetwise-1.26.41/mypy_boto3_iotfleetwise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-30 20:24:34.909745 mypy-boto3-iotfleetwise-1.26.41/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2022-12-30 20:24:22.000000 mypy-boto3-iotfleetwise-1.26.41/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 20:25:02.583779 mypy-boto3-iotfleetwise-1.26.58/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-26 20:24:36.000000 mypy-boto3-iotfleetwise-1.26.58/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21301 2023-01-26 20:25:02.583779 mypy-boto3-iotfleetwise-1.26.58/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19794 2023-01-26 20:24:36.000000 mypy-boto3-iotfleetwise-1.26.58/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 20:25:02.583779 mypy-boto3-iotfleetwise-1.26.58/mypy_boto3_iotfleetwise/
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-01-26 20:24:36.000000 mypy-boto3-iotfleetwise-1.26.58/mypy_boto3_iotfleetwise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-01-26 20:24:36.000000 mypy-boto3-iotfleetwise-1.26.58/mypy_boto3_iotfleetwise/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-01-26 20:24:36.000000 mypy-boto3-iotfleetwise-1.26.58/mypy_boto3_iotfleetwise/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40949 2023-01-26 20:24:36.000000 mypy-boto3-iotfleetwise-1.26.58/mypy_boto3_iotfleetwise/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40879 2023-01-26 20:24:36.000000 mypy-boto3-iotfleetwise-1.26.58/mypy_boto3_iotfleetwise/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-01-26 20:24:36.000000 mypy-boto3-iotfleetwise-1.26.58/mypy_boto3_iotfleetwise/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11010 2023-01-26 20:24:36.000000 mypy-boto3-iotfleetwise-1.26.58/mypy_boto3_iotfleetwise/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15488 2023-01-26 20:24:36.000000 mypy-boto3-iotfleetwise-1.26.58/mypy_boto3_iotfleetwise/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15473 2023-01-26 20:24:36.000000 mypy-boto3-iotfleetwise-1.26.58/mypy_boto3_iotfleetwise/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-26 20:24:36.000000 mypy-boto3-iotfleetwise-1.26.58/mypy_boto3_iotfleetwise/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    57068 2023-01-26 20:24:39.000000 mypy-boto3-iotfleetwise-1.26.58/mypy_boto3_iotfleetwise/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56968 2023-01-26 20:24:37.000000 mypy-boto3-iotfleetwise-1.26.58/mypy_boto3_iotfleetwise/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-26 20:24:36.000000 mypy-boto3-iotfleetwise-1.26.58/mypy_boto3_iotfleetwise/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 20:25:02.583779 mypy-boto3-iotfleetwise-1.26.58/mypy_boto3_iotfleetwise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21301 2023-01-26 20:25:02.000000 mypy-boto3-iotfleetwise-1.26.58/mypy_boto3_iotfleetwise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-01-26 20:25:02.000000 mypy-boto3-iotfleetwise-1.26.58/mypy_boto3_iotfleetwise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 20:25:02.000000 mypy-boto3-iotfleetwise-1.26.58/mypy_boto3_iotfleetwise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 20:25:02.000000 mypy-boto3-iotfleetwise-1.26.58/mypy_boto3_iotfleetwise.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-26 20:25:02.000000 mypy-boto3-iotfleetwise-1.26.58/mypy_boto3_iotfleetwise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-26 20:25:02.000000 mypy-boto3-iotfleetwise-1.26.58/mypy_boto3_iotfleetwise.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-26 20:25:02.583779 mypy-boto3-iotfleetwise-1.26.58/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-01-26 20:24:35.000000 mypy-boto3-iotfleetwise-1.26.58/setup.py
```

### Comparing `mypy-boto3-iotfleetwise-1.26.41/LICENSE` & `mypy-boto3-iotfleetwise-1.26.58/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.26.41/PKG-INFO` & `mypy-boto3-iotfleetwise-1.26.58/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotfleetwise
-Version: 1.26.41
-Summary: Type annotations for boto3.IoTFleetWise 1.26.41 service generated with mypy-boto3-builder 7.12.2
+Version: 1.26.58
+Summary: Type annotations for boto3.IoTFleetWise 1.26.58 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotfleetwise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotfleetwise)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotfleetwise?color=blue)](https://pypistats.org/packages/mypy-boto3-iotfleetwise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTFleetWise 1.26.41](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
+[boto3.IoTFleetWise 1.26.58](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iotfleetwise docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iotfleetwise-1.26.41/README.md` & `mypy-boto3-iotfleetwise-1.26.58/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotfleetwise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotfleetwise)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotfleetwise?color=blue)](https://pypistats.org/packages/mypy-boto3-iotfleetwise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTFleetWise 1.26.41](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
+[boto3.IoTFleetWise 1.26.58](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iotfleetwise docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iotfleetwise-1.26.41/mypy_boto3_iotfleetwise/__init__.py` & `mypy-boto3-iotfleetwise-1.26.58/mypy_boto3_iotfleetwise/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.26.41/mypy_boto3_iotfleetwise/__init__.pyi` & `mypy-boto3-iotfleetwise-1.26.58/mypy_boto3_iotfleetwise/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.26.41/mypy_boto3_iotfleetwise/__main__.py` & `mypy-boto3-iotfleetwise-1.26.58/mypy_boto3_iotfleetwise/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTFleetWise 1.26.41\nVersion:         1.26.41\nBuilder"
-        " version: 7.12.2\nDocs:           "
+        "Type annotations for boto3.IoTFleetWise 1.26.58\nVersion:         1.26.58\nBuilder"
+        " version: 7.12.3\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.41")
+    print("1.26.58")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-iotfleetwise-1.26.41/mypy_boto3_iotfleetwise/client.py` & `mypy-boto3-iotfleetwise-1.26.58/mypy_boto3_iotfleetwise/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.26.41/mypy_boto3_iotfleetwise/client.pyi` & `mypy-boto3-iotfleetwise-1.26.58/mypy_boto3_iotfleetwise/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.26.41/mypy_boto3_iotfleetwise/literals.py` & `mypy-boto3-iotfleetwise-1.26.58/mypy_boto3_iotfleetwise/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,14 +156,15 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
@@ -281,14 +282,15 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
```

### Comparing `mypy-boto3-iotfleetwise-1.26.41/mypy_boto3_iotfleetwise/literals.pyi` & `mypy-boto3-iotfleetwise-1.26.58/mypy_boto3_iotfleetwise/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,15 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
@@ -279,14 +280,15 @@
     "iottwinmaker",
     "iotwireless",
     "ivs",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
     "kinesis-video-webrtc-storage",
     "kinesisanalytics",
```

### Comparing `mypy-boto3-iotfleetwise-1.26.41/mypy_boto3_iotfleetwise/paginator.py` & `mypy-boto3-iotfleetwise-1.26.58/mypy_boto3_iotfleetwise/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.26.41/mypy_boto3_iotfleetwise/paginator.pyi` & `mypy-boto3-iotfleetwise-1.26.58/mypy_boto3_iotfleetwise/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.26.41/mypy_boto3_iotfleetwise/type_defs.py` & `mypy-boto3-iotfleetwise-1.26.58/mypy_boto3_iotfleetwise/type_defs.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.26.41/mypy_boto3_iotfleetwise/type_defs.pyi` & `mypy-boto3-iotfleetwise-1.26.58/mypy_boto3_iotfleetwise/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.26.41/mypy_boto3_iotfleetwise.egg-info/PKG-INFO` & `mypy-boto3-iotfleetwise-1.26.58/mypy_boto3_iotfleetwise.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotfleetwise
-Version: 1.26.41
-Summary: Type annotations for boto3.IoTFleetWise 1.26.41 service generated with mypy-boto3-builder 7.12.2
+Version: 1.26.58
+Summary: Type annotations for boto3.IoTFleetWise 1.26.58 service generated with mypy-boto3-builder 7.12.3
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotfleetwise.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotfleetwise)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-iotfleetwise?color=blue)](https://pypistats.org/packages/mypy-boto3-iotfleetwise)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTFleetWise 1.26.41](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
+[boto3.IoTFleetWise 1.26.58](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.12.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.3](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iotfleetwise docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleetwise/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-iotfleetwise-1.26.41/mypy_boto3_iotfleetwise.egg-info/SOURCES.txt` & `mypy-boto3-iotfleetwise-1.26.58/mypy_boto3_iotfleetwise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleetwise-1.26.41/setup.py` & `mypy-boto3-iotfleetwise-1.26.58/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-iotfleetwise",
-    version="1.26.41",
+    version="1.26.58",
     packages=["mypy_boto3_iotfleetwise"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTFleetWise 1.26.41 service generated with mypy-boto3-builder"
-        " 7.12.2"
+        "Type annotations for boto3.IoTFleetWise 1.26.58 service generated with mypy-boto3-builder"
+        " 7.12.3"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

