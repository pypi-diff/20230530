# Comparing `tmp/tencentcloud-dlc-provider-0.0.1.tar.gz` & `tmp/tencentcloud-dlc-provider-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tencentcloud-dlc-provider-0.0.1.tar", last modified: Tue May 30 02:58:45 2023, max compression
+gzip compressed data, was "tencentcloud-dlc-provider-0.0.2.tar", last modified: Tue May 30 08:35:03 2023, max compression
```

## Comparing `tencentcloud-dlc-provider-0.0.1.tar` & `tencentcloud-dlc-provider-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-30 02:58:45.373496 tencentcloud-dlc-provider-0.0.1/
--rw-r--r--   0 huangzheng   (501) staff       (20)       69 2023-05-30 02:58:45.373130 tencentcloud-dlc-provider-0.0.1/PKG-INFO
--rw-r--r--   0 huangzheng   (501) staff       (20)       38 2023-05-30 02:58:45.373610 tencentcloud-dlc-provider-0.0.1/setup.cfg
--rw-r--r--   0 huangzheng   (501) staff       (20)      401 2023-05-30 02:29:55.000000 tencentcloud-dlc-provider-0.0.1/setup.py
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-30 02:58:45.367381 tencentcloud-dlc-provider-0.0.1/tencentcloud_dlc_provider/
--rw-r--r--   0 huangzheng   (501) staff       (20)      362 2023-05-29 11:55:16.000000 tencentcloud-dlc-provider-0.0.1/tencentcloud_dlc_provider/__init__.py
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-30 02:58:45.371362 tencentcloud-dlc-provider-0.0.1/tencentcloud_dlc_provider/hooks/
--rw-r--r--   0 huangzheng   (501) staff       (20)        0 2023-05-10 03:24:15.000000 tencentcloud-dlc-provider-0.0.1/tencentcloud_dlc_provider/hooks/__init__.py
--rw-r--r--   0 huangzheng   (501) staff       (20)     7840 2023-05-30 02:28:26.000000 tencentcloud-dlc-provider-0.0.1/tencentcloud_dlc_provider/hooks/dlc_hook.py
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-30 02:58:45.372431 tencentcloud-dlc-provider-0.0.1/tencentcloud_dlc_provider/operators/
--rw-r--r--   0 huangzheng   (501) staff       (20)        0 2023-05-10 03:24:27.000000 tencentcloud-dlc-provider-0.0.1/tencentcloud_dlc_provider/operators/__init__.py
--rw-r--r--   0 huangzheng   (501) staff       (20)     2679 2023-05-30 02:28:45.000000 tencentcloud-dlc-provider-0.0.1/tencentcloud_dlc_provider/operators/dlc_operator.py
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-30 02:58:45.370418 tencentcloud-dlc-provider-0.0.1/tencentcloud_dlc_provider.egg-info/
--rw-r--r--   0 huangzheng   (501) staff       (20)       69 2023-05-30 02:58:45.000000 tencentcloud-dlc-provider-0.0.1/tencentcloud_dlc_provider.egg-info/PKG-INFO
--rw-r--r--   0 huangzheng   (501) staff       (20)      530 2023-05-30 02:58:45.000000 tencentcloud-dlc-provider-0.0.1/tencentcloud_dlc_provider.egg-info/SOURCES.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)        1 2023-05-30 02:58:45.000000 tencentcloud-dlc-provider-0.0.1/tencentcloud_dlc_provider.egg-info/dependency_links.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)       95 2023-05-30 02:58:45.000000 tencentcloud-dlc-provider-0.0.1/tencentcloud_dlc_provider.egg-info/entry_points.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)       55 2023-05-30 02:58:45.000000 tencentcloud-dlc-provider-0.0.1/tencentcloud_dlc_provider.egg-info/requires.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)       26 2023-05-30 02:58:45.000000 tencentcloud-dlc-provider-0.0.1/tencentcloud_dlc_provider.egg-info/top_level.txt
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-30 08:35:03.157075 tencentcloud-dlc-provider-0.0.2/
+-rw-r--r--   0 huangzheng   (501) staff       (20)       69 2023-05-30 08:35:03.156746 tencentcloud-dlc-provider-0.0.2/PKG-INFO
+-rw-r--r--   0 huangzheng   (501) staff       (20)       38 2023-05-30 08:35:03.157175 tencentcloud-dlc-provider-0.0.2/setup.cfg
+-rw-r--r--   0 huangzheng   (501) staff       (20)      401 2023-05-30 08:34:32.000000 tencentcloud-dlc-provider-0.0.2/setup.py
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-30 08:35:03.151569 tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider/
+-rw-r--r--   0 huangzheng   (501) staff       (20)      362 2023-05-29 11:55:16.000000 tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider/__init__.py
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-30 08:35:03.154976 tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider/hooks/
+-rw-r--r--   0 huangzheng   (501) staff       (20)        0 2023-05-10 03:24:15.000000 tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider/hooks/__init__.py
+-rw-r--r--   0 huangzheng   (501) staff       (20)     7840 2023-05-30 02:28:26.000000 tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider/hooks/dlc_hook.py
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-30 08:35:03.156029 tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider/operators/
+-rw-r--r--   0 huangzheng   (501) staff       (20)        0 2023-05-10 03:24:27.000000 tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider/operators/__init__.py
+-rw-r--r--   0 huangzheng   (501) staff       (20)     2746 2023-05-30 08:03:13.000000 tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider/operators/dlc_operator.py
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-30 08:35:03.154257 tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider.egg-info/
+-rw-r--r--   0 huangzheng   (501) staff       (20)       69 2023-05-30 08:35:03.000000 tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider.egg-info/PKG-INFO
+-rw-r--r--   0 huangzheng   (501) staff       (20)      530 2023-05-30 08:35:03.000000 tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)        1 2023-05-30 08:35:03.000000 tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)       95 2023-05-30 08:35:03.000000 tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider.egg-info/entry_points.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)       55 2023-05-30 08:35:03.000000 tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider.egg-info/requires.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)       26 2023-05-30 08:35:03.000000 tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider.egg-info/top_level.txt
```

### Comparing `tencentcloud-dlc-provider-0.0.1/tencentcloud_dlc_provider/hooks/dlc_hook.py` & `tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider/hooks/dlc_hook.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-dlc-provider-0.0.1/tencentcloud_dlc_provider/operators/dlc_operator.py` & `tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider/operators/dlc_operator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-from typing import Any
+from typing import Any, Sequence
 
 from airflow.models.baseoperator import BaseOperator
 from airflow.utils.context import Context
 from tencentcloud_dlc_provider.hooks.dlc_hook import DLCHook
 import logging
 LOG = logging.getLogger(__name__)
 
 
 class DLCOperator(BaseOperator):
+    template_fields: Sequence[str] = ("sql", "cmd_args")
+
     def __init__(
             self,
             *,
             dlc_conn_id: str,
             sql="",
             engine="",
             job_name="",
-            cmd_args ="",
+            cmd_args="",
             executor_size="",
             driver_size="",
             executor_numbers=0,
             **kwargs
     ) -> None:
         super().__init__(**kwargs)
         self.sql = sql
```

### Comparing `tencentcloud-dlc-provider-0.0.1/tencentcloud_dlc_provider.egg-info/SOURCES.txt` & `tencentcloud-dlc-provider-0.0.2/tencentcloud_dlc_provider.egg-info/SOURCES.txt`

 * *Files identical despite different names*

