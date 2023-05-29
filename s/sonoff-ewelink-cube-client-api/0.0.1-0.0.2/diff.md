# Comparing `tmp/sonoff-ewelink-cube-client-api-0.0.1.tar.gz` & `tmp/sonoff-ewelink-cube-client-api-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sonoff-ewelink-cube-client-api-0.0.1.tar", last modified: Mon May 29 20:53:13 2023, max compression
+gzip compressed data, was "sonoff-ewelink-cube-client-api-0.0.2.tar", last modified: Mon May 29 22:07:55 2023, max compression
```

## Comparing `sonoff-ewelink-cube-client-api-0.0.1.tar` & `sonoff-ewelink-cube-client-api-0.0.2.tar`

### file list

```diff
@@ -1,48 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:53:13.738561 sonoff-ewelink-cube-client-api-0.0.1/
--rw-r--r--   0 root         (0) root         (0)     1066 2023-05-29 13:43:13.000000 sonoff-ewelink-cube-client-api-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4516 2023-05-29 20:53:13.734561 sonoff-ewelink-cube-client-api-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3462 2023-05-29 20:49:33.000000 sonoff-ewelink-cube-client-api-0.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 20:53:13.738561 sonoff-ewelink-cube-client-api-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1950 2023-05-29 20:41:57.000000 sonoff-ewelink-cube-client-api-0.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:53:13.726560 sonoff-ewelink-cube-client-api-0.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:53:13.730561 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/
--rw-r--r--   0 root         (0) root         (0)     1180 2023-05-29 16:47:41.000000 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:53:13.730561 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/api/
--rw-r--r--   0 root         (0) root         (0)       45 2023-05-29 13:44:23.000000 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3510 2023-05-29 20:16:13.000000 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/api/baseClass.py
--rw-r--r--   0 root         (0) root         (0)     3329 2023-05-29 20:18:11.000000 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/api/baseClassBridge.py
--rw-r--r--   0 root         (0) root         (0)     3340 2023-05-29 20:15:12.000000 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/api/baseClassDevice.py
--rw-r--r--   0 root         (0) root         (0)     1492 2023-05-29 20:19:31.000000 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/api/baseClassHardware.py
--rw-r--r--   0 root         (0) root         (0)     7496 2023-05-29 18:23:23.000000 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/api/baseClassSse.py
--rw-r--r--   0 root         (0) root         (0)      822 2023-05-29 20:21:30.000000 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/api/ihostClass.py
--rw-r--r--   0 root         (0) root         (0)      872 2023-05-29 20:22:09.000000 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/api/nspanelproClass.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:53:13.730561 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/config/
--rw-r--r--   0 root         (0) root         (0)     1260 2023-05-29 20:23:04.000000 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:53:13.730561 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/ts/
--rw-r--r--   0 root         (0) root         (0)       54 2023-05-29 13:44:26.000000 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/ts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:53:13.734561 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/ts/enum/
--rw-r--r--   0 root         (0) root         (0)     1555 2023-05-29 13:44:26.000000 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/ts/enum/ECapability.py
--rw-r--r--   0 root         (0) root         (0)     1241 2023-05-29 13:44:26.000000 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/ts/enum/ECategory.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-05-29 13:44:27.000000 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/ts/enum/EMethod.py
--rw-r--r--   0 root         (0) root         (0)     1263 2023-05-29 13:44:27.000000 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/ts/enum/EPath.py
--rw-r--r--   0 root         (0) root         (0)       55 2023-05-29 13:44:27.000000 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/ts/enum/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:53:13.734561 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/ts/interface/
--rw-r--r--   0 root         (0) root         (0)      879 2023-05-29 17:13:36.000000 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/ts/interface/IConfig.py
--rw-r--r--   0 root         (0) root         (0)     1143 2023-05-29 16:55:40.000000 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/ts/interface/IDebugLog.py
--rw-r--r--   0 root         (0) root         (0)     2616 2023-05-29 16:34:39.000000 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/ts/interface/IDevice.py
--rw-r--r--   0 root         (0) root         (0)      871 2023-05-29 16:33:47.000000 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/ts/interface/IHttpConfig.py
--rw-r--r--   0 root         (0) root         (0)      592 2023-05-29 13:44:29.000000 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/ts/interface/IResponse.py
--rw-r--r--   0 root         (0) root         (0)     1729 2023-05-29 13:44:30.000000 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/ts/interface/ISseEvent.py
--rw-r--r--   0 root         (0) root         (0)     1504 2023-05-29 16:30:37.000000 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/ts/interface/IThirdParty.py
--rw-r--r--   0 root         (0) root         (0)     2036 2023-05-29 16:31:52.000000 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/ts/interface/IThirdpartyDevice.py
--rw-r--r--   0 root         (0) root         (0)       52 2023-05-29 13:44:30.000000 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/ts/interface/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:53:13.734561 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/utils/
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-29 13:44:31.000000 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 13:44:31.000000 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/utils/eventsource.py
--rw-r--r--   0 root         (0) root         (0)     2739 2023-05-29 17:30:09.000000 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/utils/httpUtils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:53:13.730561 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4516 2023-05-29 20:53:13.000000 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1905 2023-05-29 20:53:13.000000 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 20:53:13.000000 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-29 20:53:13.000000 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-05-29 20:53:13.000000 sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 22:07:55.730011 sonoff-ewelink-cube-client-api-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1066 2023-05-29 13:43:13.000000 sonoff-ewelink-cube-client-api-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4581 2023-05-29 22:07:55.730011 sonoff-ewelink-cube-client-api-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3527 2023-05-29 21:57:27.000000 sonoff-ewelink-cube-client-api-0.0.2/README.md
+-rw-r--r--   0 root         (0) root         (0)      562 2023-05-29 21:48:51.000000 sonoff-ewelink-cube-client-api-0.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 22:07:55.730011 sonoff-ewelink-cube-client-api-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1916 2023-05-29 21:37:21.000000 sonoff-ewelink-cube-client-api-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 22:07:55.718011 sonoff-ewelink-cube-client-api-0.0.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 22:07:55.722010 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/
+-rw-r--r--   0 root         (0) root         (0)     1180 2023-05-29 16:47:41.000000 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 22:07:55.726010 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/api/
+-rw-r--r--   0 root         (0) root         (0)       45 2023-05-29 13:44:23.000000 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3510 2023-05-29 20:16:13.000000 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/api/baseClass.py
+-rw-r--r--   0 root         (0) root         (0)     3329 2023-05-29 20:18:11.000000 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/api/baseClassBridge.py
+-rw-r--r--   0 root         (0) root         (0)     3340 2023-05-29 20:15:12.000000 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/api/baseClassDevice.py
+-rw-r--r--   0 root         (0) root         (0)     1492 2023-05-29 20:19:31.000000 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/api/baseClassHardware.py
+-rw-r--r--   0 root         (0) root         (0)     7496 2023-05-29 18:23:23.000000 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/api/baseClassSse.py
+-rw-r--r--   0 root         (0) root         (0)      822 2023-05-29 20:21:30.000000 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/api/ihostClass.py
+-rw-r--r--   0 root         (0) root         (0)      872 2023-05-29 20:22:09.000000 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/api/nspanelproClass.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 22:07:55.726010 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/config/
+-rw-r--r--   0 root         (0) root         (0)     1260 2023-05-29 20:23:04.000000 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 22:07:55.726010 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/ts/
+-rw-r--r--   0 root         (0) root         (0)       54 2023-05-29 13:44:26.000000 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/ts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 22:07:55.726010 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/ts/enum/
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-05-29 13:44:26.000000 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/ts/enum/ECapability.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2023-05-29 13:44:26.000000 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/ts/enum/ECategory.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-05-29 13:44:27.000000 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/ts/enum/EMethod.py
+-rw-r--r--   0 root         (0) root         (0)     1263 2023-05-29 13:44:27.000000 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/ts/enum/EPath.py
+-rw-r--r--   0 root         (0) root         (0)       55 2023-05-29 13:44:27.000000 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/ts/enum/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 22:07:55.730011 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/ts/interface/
+-rw-r--r--   0 root         (0) root         (0)      879 2023-05-29 17:13:36.000000 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/ts/interface/IConfig.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-05-29 16:55:40.000000 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/ts/interface/IDebugLog.py
+-rw-r--r--   0 root         (0) root         (0)     2616 2023-05-29 16:34:39.000000 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/ts/interface/IDevice.py
+-rw-r--r--   0 root         (0) root         (0)      871 2023-05-29 16:33:47.000000 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/ts/interface/IHttpConfig.py
+-rw-r--r--   0 root         (0) root         (0)      592 2023-05-29 13:44:29.000000 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/ts/interface/IResponse.py
+-rw-r--r--   0 root         (0) root         (0)     1729 2023-05-29 13:44:30.000000 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/ts/interface/ISseEvent.py
+-rw-r--r--   0 root         (0) root         (0)     1504 2023-05-29 16:30:37.000000 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/ts/interface/IThirdParty.py
+-rw-r--r--   0 root         (0) root         (0)     2036 2023-05-29 16:31:52.000000 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/ts/interface/IThirdpartyDevice.py
+-rw-r--r--   0 root         (0) root         (0)       52 2023-05-29 13:44:30.000000 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/ts/interface/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 22:07:55.730011 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/utils/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-05-29 13:44:31.000000 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 13:44:31.000000 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/utils/eventsource.py
+-rw-r--r--   0 root         (0) root         (0)     2739 2023-05-29 17:30:09.000000 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/utils/httpUtils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 22:07:55.722010 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4581 2023-05-29 22:07:55.000000 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-05-29 22:07:55.000000 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 22:07:55.000000 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-05-29 22:07:55.000000 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-29 22:07:55.000000 sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 22:07:55.730011 sonoff-ewelink-cube-client-api-0.0.2/tests/
+-rw-r--r--   0 root         (0) root         (0)     6602 2023-05-29 14:24:53.000000 sonoff-ewelink-cube-client-api-0.0.2/tests/test_api_baseClassBridge.py
+-rw-r--r--   0 root         (0) root         (0)     3688 2023-05-29 14:24:53.000000 sonoff-ewelink-cube-client-api-0.0.2/tests/test_api_base_class_sse.py
```

### Comparing `sonoff-ewelink-cube-client-api-0.0.1/LICENSE` & `sonoff-ewelink-cube-client-api-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sonoff-ewelink-cube-client-api-0.0.1/PKG-INFO` & `sonoff-ewelink-cube-client-api-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonoff-ewelink-cube-client-api
-Version: 0.0.1
+Version: 0.0.2
 Summary: SONOFF eWelink CUBE API communication library (unofficial)
 Home-page: https://github.com/sm4rth0m3/python-pip.sonoff-ewelink-cube-client-api
 Author: sipimokus
 Author-email: sipimokus@gmail.com
 Project-URL: Bug Tracker, https://github.com/sm4rth0m3/python-pip.sonoff-ewelink-cube-client-api/issues
 Project-URL: Documentation, https://github.com/sm4rth0m3/python-pip.sonoff-ewelink-cube-client-api
 Keywords: sonoff ewelink cube api openapi ihost nspanel library asyncio
@@ -90,26 +90,26 @@
 
 
 # Run the main function
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
-See more in the [examples](examples) directory.
+See more in the [examples](https://github.com/sm4rth0m3/python-pip.sonoff-ewelink-cube-client-api/tree/main/examples) directory.
 
 
 ---
 ## Development and testing
 
 ```sh
 # Start docker container (or use virtualenv)
-docker run -it -v "$(pwd)":/app -w /app python:3.11-slim /bin/bash
+docker run -rm -it -v "$(pwd)":/app -w /app python:3.11-slim /bin/bash
 
 # Install packages and repository
-pip3 install -r requirements.txt -r requirements-dev.txt
+pip3 install -r requirements-dev.txt
 pip3 install .
 
 # Pylint checks
 pylint --recursive=y ./setup.py ./src ./examples
 
 # Try examples
 export LOG_LEVEL=DEBUG
```

### Comparing `sonoff-ewelink-cube-client-api-0.0.1/README.md` & `sonoff-ewelink-cube-client-api-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -67,26 +67,26 @@
 
 
 # Run the main function
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
-See more in the [examples](examples) directory.
+See more in the [examples](https://github.com/sm4rth0m3/python-pip.sonoff-ewelink-cube-client-api/tree/main/examples) directory.
 
 
 ---
 ## Development and testing
 
 ```sh
 # Start docker container (or use virtualenv)
-docker run -it -v "$(pwd)":/app -w /app python:3.11-slim /bin/bash
+docker run -rm -it -v "$(pwd)":/app -w /app python:3.11-slim /bin/bash
 
 # Install packages and repository
-pip3 install -r requirements.txt -r requirements-dev.txt
+pip3 install -r requirements-dev.txt
 pip3 install .
 
 # Pylint checks
 pylint --recursive=y ./setup.py ./src ./examples
 
 # Try examples
 export LOG_LEVEL=DEBUG
```

### Comparing `sonoff-ewelink-cube-client-api-0.0.1/setup.py` & `sonoff-ewelink-cube-client-api-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 """Setup file for installing and configuring the sonoff-ewelink-cube-client-api package."""
 from setuptools import setup, find_packages
 
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-with open("requirements.txt", "r", encoding="utf-8") as fh:
-    requirements = fh.read().splitlines()
-
 setup(
     name="sonoff-ewelink-cube-client-api",
     version=VERSION,
     author="sipimokus",
     author_email="sipimokus@gmail.com",
     description="SONOFF eWelink CUBE API communication library (unofficial)",
     long_description=long_description,
@@ -40,9 +37,13 @@
         "Topic :: System :: Networking",
         "Topic :: Utilities",
     ],
     keywords="sonoff ewelink cube api openapi ihost nspanel library asyncio",
     packages=find_packages("src"),
     package_dir={"": "src"},
     python_requires=">=3.6",
-    install_requires=requirements,
+    install_requires=[
+        "aiohttp>=3.0.0",
+        "asyncio>=3.4.3",
+        "setuptools",
+    ],
 )
```

### Comparing `sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/__init__.py` & `sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/__init__.py`

 * *Files identical despite different names*

### Comparing `sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/api/baseClass.py` & `sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/api/baseClass.py`

 * *Files identical despite different names*

### Comparing `sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/api/baseClassBridge.py` & `sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/api/baseClassBridge.py`

 * *Files identical despite different names*

### Comparing `sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/api/baseClassDevice.py` & `sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/api/baseClassDevice.py`

 * *Files identical despite different names*

### Comparing `sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/api/baseClassHardware.py` & `sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/api/baseClassHardware.py`

 * *Files identical despite different names*

### Comparing `sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/api/baseClassSse.py` & `sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/api/baseClassSse.py`

 * *Files identical despite different names*

### Comparing `sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/api/ihostClass.py` & `sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/api/ihostClass.py`

 * *Files identical despite different names*

### Comparing `sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/api/nspanelproClass.py` & `sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/api/nspanelproClass.py`

 * *Files identical despite different names*

### Comparing `sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/config/__init__.py` & `sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/ts/enum/ECapability.py` & `sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/ts/enum/ECapability.py`

 * *Files identical despite different names*

### Comparing `sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/ts/enum/ECategory.py` & `sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/ts/enum/ECategory.py`

 * *Files identical despite different names*

### Comparing `sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/ts/enum/EPath.py` & `sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/ts/enum/EPath.py`

 * *Files identical despite different names*

### Comparing `sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/ts/interface/IConfig.py` & `sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/ts/interface/IConfig.py`

 * *Files identical despite different names*

### Comparing `sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/ts/interface/IDebugLog.py` & `sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/ts/interface/IDebugLog.py`

 * *Files identical despite different names*

### Comparing `sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/ts/interface/IDevice.py` & `sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/ts/interface/IDevice.py`

 * *Files identical despite different names*

### Comparing `sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/ts/interface/IHttpConfig.py` & `sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/ts/interface/IHttpConfig.py`

 * *Files identical despite different names*

### Comparing `sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/ts/interface/IResponse.py` & `sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/ts/interface/IResponse.py`

 * *Files identical despite different names*

### Comparing `sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/ts/interface/ISseEvent.py` & `sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/ts/interface/ISseEvent.py`

 * *Files identical despite different names*

### Comparing `sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/ts/interface/IThirdParty.py` & `sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/ts/interface/IThirdParty.py`

 * *Files identical despite different names*

### Comparing `sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/ts/interface/IThirdpartyDevice.py` & `sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/ts/interface/IThirdpartyDevice.py`

 * *Files identical despite different names*

### Comparing `sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api/utils/httpUtils.py` & `sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api/utils/httpUtils.py`

 * *Files identical despite different names*

### Comparing `sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api.egg-info/PKG-INFO` & `sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonoff-ewelink-cube-client-api
-Version: 0.0.1
+Version: 0.0.2
 Summary: SONOFF eWelink CUBE API communication library (unofficial)
 Home-page: https://github.com/sm4rth0m3/python-pip.sonoff-ewelink-cube-client-api
 Author: sipimokus
 Author-email: sipimokus@gmail.com
 Project-URL: Bug Tracker, https://github.com/sm4rth0m3/python-pip.sonoff-ewelink-cube-client-api/issues
 Project-URL: Documentation, https://github.com/sm4rth0m3/python-pip.sonoff-ewelink-cube-client-api
 Keywords: sonoff ewelink cube api openapi ihost nspanel library asyncio
@@ -90,26 +90,26 @@
 
 
 # Run the main function
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
-See more in the [examples](examples) directory.
+See more in the [examples](https://github.com/sm4rth0m3/python-pip.sonoff-ewelink-cube-client-api/tree/main/examples) directory.
 
 
 ---
 ## Development and testing
 
 ```sh
 # Start docker container (or use virtualenv)
-docker run -it -v "$(pwd)":/app -w /app python:3.11-slim /bin/bash
+docker run -rm -it -v "$(pwd)":/app -w /app python:3.11-slim /bin/bash
 
 # Install packages and repository
-pip3 install -r requirements.txt -r requirements-dev.txt
+pip3 install -r requirements-dev.txt
 pip3 install .
 
 # Pylint checks
 pylint --recursive=y ./setup.py ./src ./examples
 
 # Try examples
 export LOG_LEVEL=DEBUG
```

### Comparing `sonoff-ewelink-cube-client-api-0.0.1/src/sonoff_ewelink_cube_client_api.egg-info/SOURCES.txt` & `sonoff-ewelink-cube-client-api-0.0.2/src/sonoff_ewelink_cube_client_api.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+pyproject.toml
 setup.py
 src/sonoff_ewelink_cube_client_api/__init__.py
 src/sonoff_ewelink_cube_client_api.egg-info/PKG-INFO
 src/sonoff_ewelink_cube_client_api.egg-info/SOURCES.txt
 src/sonoff_ewelink_cube_client_api.egg-info/dependency_links.txt
 src/sonoff_ewelink_cube_client_api.egg-info/requires.txt
 src/sonoff_ewelink_cube_client_api.egg-info/top_level.txt
@@ -29,8 +30,10 @@
 src/sonoff_ewelink_cube_client_api/ts/interface/IResponse.py
 src/sonoff_ewelink_cube_client_api/ts/interface/ISseEvent.py
 src/sonoff_ewelink_cube_client_api/ts/interface/IThirdParty.py
 src/sonoff_ewelink_cube_client_api/ts/interface/IThirdpartyDevice.py
 src/sonoff_ewelink_cube_client_api/ts/interface/__init__.py
 src/sonoff_ewelink_cube_client_api/utils/__init__.py
 src/sonoff_ewelink_cube_client_api/utils/eventsource.py
-src/sonoff_ewelink_cube_client_api/utils/httpUtils.py
+src/sonoff_ewelink_cube_client_api/utils/httpUtils.py
+tests/test_api_baseClassBridge.py
+tests/test_api_base_class_sse.py
```

