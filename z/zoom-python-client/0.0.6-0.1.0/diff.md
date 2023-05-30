# Comparing `tmp/zoom_python_client-0.0.6.tar.gz` & `tmp/zoom_python_client-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoom_python_client-0.0.6.tar", max compression
+gzip compressed data, was "zoom_python_client-0.1.0.tar", max compression
```

## Comparing `zoom_python_client-0.0.6.tar` & `zoom_python_client-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    35149 2023-05-30 07:49:07.890357 zoom_python_client-0.0.6/LICENSE
--rw-r--r--   0        0        0     3306 2023-05-30 07:49:07.890357 zoom_python_client-0.0.6/README.md
--rw-r--r--   0        0        0     1384 2023-05-30 07:49:07.890357 zoom_python_client-0.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-30 07:49:07.890357 zoom_python_client-0.0.6/zoom_python_client/__init__.py
--rw-r--r--   0        0        0     2401 2023-05-30 07:49:07.890357 zoom_python_client-0.0.6/zoom_python_client/api_client.py
--rw-r--r--   0        0        0        0 2023-05-30 07:49:07.890357 zoom_python_client-0.0.6/zoom_python_client/client_components/__init__.py
--rw-r--r--   0        0        0        0 2023-05-30 07:49:07.894357 zoom_python_client-0.0.6/zoom_python_client/client_components/meeting_livestreams/__init__.py
--rw-r--r--   0        0        0     1722 2023-05-30 07:49:07.894357 zoom_python_client-0.0.6/zoom_python_client/client_components/meeting_livestreams/meeting_livestreams_component.py
--rw-r--r--   0        0        0        0 2023-05-30 07:49:07.894357 zoom_python_client-0.0.6/zoom_python_client/client_components/meetings/__init__.py
--rw-r--r--   0        0        0      624 2023-05-30 07:49:07.894357 zoom_python_client-0.0.6/zoom_python_client/client_components/meetings/meetings_component.py
--rw-r--r--   0        0        0        0 2023-05-30 07:49:07.894357 zoom_python_client-0.0.6/zoom_python_client/client_components/users/__init__.py
--rw-r--r--   0        0        0     1286 2023-05-30 07:49:07.894357 zoom_python_client-0.0.6/zoom_python_client/client_components/users/users_component.py
--rw-r--r--   0        0        0        0 2023-05-30 07:49:07.894357 zoom_python_client-0.0.6/zoom_python_client/client_components/webinar_livestreams/__init__.py
--rw-r--r--   0        0        0     1583 2023-05-30 07:49:07.894357 zoom_python_client-0.0.6/zoom_python_client/client_components/webinar_livestreams/webinar_livestreams_component.py
--rw-r--r--   0        0        0        0 2023-05-30 07:49:07.894357 zoom_python_client-0.0.6/zoom_python_client/client_components/webinars/__init__.py
--rw-r--r--   0        0        0      401 2023-05-30 07:49:07.894357 zoom_python_client-0.0.6/zoom_python_client/client_components/webinars/webinars_component.py
--rw-r--r--   0        0        0        0 2023-05-30 07:49:07.894357 zoom_python_client-0.0.6/zoom_python_client/utils/__init__.py
--rw-r--r--   0        0        0      221 2023-05-30 07:49:07.894357 zoom_python_client-0.0.6/zoom_python_client/utils/file_system.py
--rw-r--r--   0        0        0      731 2023-05-30 07:49:07.894357 zoom_python_client-0.0.6/zoom_python_client/utils/logger.py
--rw-r--r--   0        0        0     5954 2023-05-30 07:49:07.894357 zoom_python_client-0.0.6/zoom_python_client/zoom_api_client.py
--rw-r--r--   0        0        0        0 2023-05-30 07:49:07.894357 zoom_python_client-0.0.6/zoom_python_client/zoom_auth_api/__init__.py
--rw-r--r--   0        0        0     4629 2023-05-30 07:49:07.894357 zoom_python_client-0.0.6/zoom_python_client/zoom_auth_api/zoom_auth_api_client.py
--rw-r--r--   0        0        0      817 2023-05-30 07:49:07.894357 zoom_python_client-0.0.6/zoom_python_client/zoom_client_interface.py
--rw-r--r--   0        0        0     4338 1970-01-01 00:00:00.000000 zoom_python_client-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-30 09:35:24.927101 zoom_python_client-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3306 2023-05-30 09:35:24.927101 zoom_python_client-0.1.0/README.md
+-rw-r--r--   0        0        0     1381 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/__init__.py
+-rw-r--r--   0        0        0     2401 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/api_client.py
+-rw-r--r--   0        0        0        0 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/client_components/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/client_components/meeting_livestreams/__init__.py
+-rw-r--r--   0        0        0     1722 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/client_components/meeting_livestreams/meeting_livestreams_component.py
+-rw-r--r--   0        0        0        0 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/client_components/meetings/__init__.py
+-rw-r--r--   0        0        0      624 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/client_components/meetings/meetings_component.py
+-rw-r--r--   0        0        0        0 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/client_components/users/__init__.py
+-rw-r--r--   0        0        0     1286 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/client_components/users/users_component.py
+-rw-r--r--   0        0        0        0 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/client_components/webinar_livestreams/__init__.py
+-rw-r--r--   0        0        0     1583 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/client_components/webinar_livestreams/webinar_livestreams_component.py
+-rw-r--r--   0        0        0        0 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/client_components/webinars/__init__.py
+-rw-r--r--   0        0        0      401 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/client_components/webinars/webinars_component.py
+-rw-r--r--   0        0        0        0 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/utils/__init__.py
+-rw-r--r--   0        0        0      221 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/utils/file_system.py
+-rw-r--r--   0        0        0      731 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/utils/logger.py
+-rw-r--r--   0        0        0     5954 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/zoom_api_client.py
+-rw-r--r--   0        0        0        0 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/zoom_auth_api/__init__.py
+-rw-r--r--   0        0        0     4629 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/zoom_auth_api/zoom_auth_api_client.py
+-rw-r--r--   0        0        0      817 2023-05-30 09:35:24.931101 zoom_python_client-0.1.0/zoom_python_client/zoom_client_interface.py
+-rw-r--r--   0        0        0     4348 1970-01-01 00:00:00.000000 zoom_python_client-0.1.0/PKG-INFO
```

### Comparing `zoom_python_client-0.0.6/LICENSE` & `zoom_python_client-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zoom_python_client-0.0.6/README.md` & `zoom_python_client-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `zoom_python_client-0.0.6/pyproject.toml` & `zoom_python_client-0.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zoom-python-client"
-version = "0.0.6"
+version = "0.1.0"
 authors = ["Rene Fernandez Sanchez <rene.fernandez@cern.ch>"]
 maintainers = ["Rene Fernandez Sanchez <rene.fernandez@cern.ch>"]
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
   "Operating System :: OS Independent",
 ]
@@ -15,17 +15,17 @@
 license = "GPL-3.0-only"
 packages = [{ include = "zoom_python_client" }]
 readme = "README.md"
 repository = "https://github.com/cern-vc/zoom-python-client"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-python-dotenv = "0.21.0"
-requests = "2.23.0"
-typing-extensions = "4.3.0"
+python-dotenv = "^0.21"
+requests = "^2.23"
+typing-extensions = "^4.3"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "23.3.0"
 flake8 = "6.0.0"
 isort = "5.10.1"
 pre-commit = "2.15.0"
```

### Comparing `zoom_python_client-0.0.6/zoom_python_client/api_client.py` & `zoom_python_client-0.1.0/zoom_python_client/api_client.py`

 * *Files identical despite different names*

### Comparing `zoom_python_client-0.0.6/zoom_python_client/client_components/meeting_livestreams/meeting_livestreams_component.py` & `zoom_python_client-0.1.0/zoom_python_client/client_components/meeting_livestreams/meeting_livestreams_component.py`

 * *Files identical despite different names*

### Comparing `zoom_python_client-0.0.6/zoom_python_client/client_components/meetings/meetings_component.py` & `zoom_python_client-0.1.0/zoom_python_client/client_components/meetings/meetings_component.py`

 * *Files identical despite different names*

### Comparing `zoom_python_client-0.0.6/zoom_python_client/client_components/users/users_component.py` & `zoom_python_client-0.1.0/zoom_python_client/client_components/users/users_component.py`

 * *Files identical despite different names*

### Comparing `zoom_python_client-0.0.6/zoom_python_client/client_components/webinar_livestreams/webinar_livestreams_component.py` & `zoom_python_client-0.1.0/zoom_python_client/client_components/webinar_livestreams/webinar_livestreams_component.py`

 * *Files identical despite different names*

### Comparing `zoom_python_client-0.0.6/zoom_python_client/utils/logger.py` & `zoom_python_client-0.1.0/zoom_python_client/utils/logger.py`

 * *Files identical despite different names*

### Comparing `zoom_python_client-0.0.6/zoom_python_client/zoom_api_client.py` & `zoom_python_client-0.1.0/zoom_python_client/zoom_api_client.py`

 * *Files identical despite different names*

### Comparing `zoom_python_client-0.0.6/zoom_python_client/zoom_auth_api/zoom_auth_api_client.py` & `zoom_python_client-0.1.0/zoom_python_client/zoom_auth_api/zoom_auth_api_client.py`

 * *Files identical despite different names*

### Comparing `zoom_python_client-0.0.6/zoom_python_client/zoom_client_interface.py` & `zoom_python_client-0.1.0/zoom_python_client/zoom_client_interface.py`

 * *Files identical despite different names*

### Comparing `zoom_python_client-0.0.6/PKG-INFO` & `zoom_python_client-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zoom-python-client
-Version: 0.0.6
+Version: 0.1.0
 Summary: Zoom API client for Python using server to server tokens
 Home-page: https://github.com/cern-vc/zoom-python-client
 License: GPL-3.0-only
 Keywords: zoom,api
 Author: Rene Fernandez Sanchez
 Author-email: rene.fernandez@cern.ch
 Maintainer: Rene Fernandez Sanchez
@@ -12,17 +12,17 @@
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: python-dotenv (==0.21.0)
-Requires-Dist: requests (==2.23.0)
-Requires-Dist: typing-extensions (==4.3.0)
+Requires-Dist: python-dotenv (>=0.21,<0.22)
+Requires-Dist: requests (>=2.23,<3.0)
+Requires-Dist: typing-extensions (>=4.3,<5.0)
 Project-URL: Bug Tracker, https://github.com/cern-vc/zoom-python-client/issues
 Project-URL: Repository, https://github.com/cern-vc/zoom-python-client
 Description-Content-Type: text/markdown
 
 # Zoom Python client
 
 [![Python tests](https://github.com/cern-vc/zoom-python-client/actions/workflows/python-tests.yml/badge.svg)](https://github.com/cern-vc/zoom-python-client/actions/workflows/python-tests.yml) [![pre-commit](https://github.com/cern-vc/zoom-python-client/actions/workflows/pre-commit.yaml/badge.svg)](https://github.com/cern-vc/zoom-python-client/actions/workflows/pre-commit.yaml) [![CodeQL](https://github.com/cern-vc/zoom-python-client/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/cern-vc/zoom-python-client/actions/workflows/codeql-analysis.yml) [![codecov](https://codecov.io/gh/cern-vc/zoom-python-client/branch/main/graph/badge.svg?token=04EY0K0P2S)](https://codecov.io/gh/cern-vc/zoom-python-client)
```

