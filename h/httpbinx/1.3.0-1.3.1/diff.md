# Comparing `tmp/httpbinx-1.3.0.tar.gz` & `tmp/httpbinx-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpbinx-1.3.0.tar", last modified: Thu May 25 17:54:34 2023, max compression
+gzip compressed data, was "httpbinx-1.3.1.tar", last modified: Tue May 30 17:07:50 2023, max compression
```

## Comparing `httpbinx-1.3.0.tar` & `httpbinx-1.3.1.tar`

### file list

```diff
@@ -1,53 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:54:34.754466 httpbinx-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-25 17:54:21.000000 httpbinx-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-25 17:54:21.000000 httpbinx-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-25 17:54:34.754466 httpbinx-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-25 17:54:21.000000 httpbinx-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:54:34.746466 httpbinx-1.3.0/httpbinx/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:54:34.750466 httpbinx-1.3.0/httpbinx/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:54:34.750466 httpbinx-1.3.0/httpbinx/routers/
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/routers/anything.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/routers/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/routers/cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)     6600 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/routers/dynamicdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/routers/httpmethods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/routers/images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:54:34.750466 httpbinx-1.3.0/httpbinx/routers/inspection/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/routers/inspection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/routers/inspection/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/routers/inspection/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/routers/redirects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/routers/responseformats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/routers/statuscodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:54:34.750466 httpbinx-1.3.0/httpbinx/static/
--rw-r--r--   0 runner    (1001) docker     (123)    14058 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/static/UTF-8-demo.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/static/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:54:34.750466 httpbinx-1.3.0/httpbinx/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/static/images/httbinx_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/static/images/httpbinx_cover.png
--rw-r--r--   0 runner    (1001) docker     (123)    35588 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/static/images/jackal.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/static/images/pig_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/static/images/svg_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/static/images/wolf_1.webp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:54:34.754466 httpbinx-1.3.0/httpbinx/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/templates/moby.html
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/templates/sample.xml
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/templates/trackingscripts.html
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-25 17:54:21.000000 httpbinx-1.3.0/httpbinx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:54:34.746466 httpbinx-1.3.0/httpbinx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-25 17:54:34.000000 httpbinx-1.3.0/httpbinx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-25 17:54:34.000000 httpbinx-1.3.0/httpbinx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:54:34.000000 httpbinx-1.3.0/httpbinx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-25 17:54:34.000000 httpbinx-1.3.0/httpbinx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 17:54:34.000000 httpbinx-1.3.0/httpbinx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 17:54:34.754466 httpbinx-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-25 17:54:21.000000 httpbinx-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:07:50.501426 httpbinx-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-30 17:07:39.000000 httpbinx-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-30 17:07:39.000000 httpbinx-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-30 17:07:50.501426 httpbinx-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-30 17:07:39.000000 httpbinx-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:07:50.497426 httpbinx-1.3.1/httpbinx/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 17:07:39.000000 httpbinx-1.3.1/httpbinx/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-30 17:07:39.000000 httpbinx-1.3.1/httpbinx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-30 17:07:39.000000 httpbinx-1.3.1/httpbinx/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:07:50.497426 httpbinx-1.3.1/httpbinx/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:07:39.000000 httpbinx-1.3.1/httpbinx/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-05-30 17:07:39.000000 httpbinx-1.3.1/httpbinx/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-30 17:07:39.000000 httpbinx-1.3.1/httpbinx/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:07:50.497426 httpbinx-1.3.1/httpbinx/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-30 17:07:39.000000 httpbinx-1.3.1/httpbinx/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-30 17:07:39.000000 httpbinx-1.3.1/httpbinx/routers/anything.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-30 17:07:39.000000 httpbinx-1.3.1/httpbinx/routers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-30 17:07:39.000000 httpbinx-1.3.1/httpbinx/routers/cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-05-30 17:07:39.000000 httpbinx-1.3.1/httpbinx/routers/dynamicdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-30 17:07:39.000000 httpbinx-1.3.1/httpbinx/routers/httpmethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-30 17:07:39.000000 httpbinx-1.3.1/httpbinx/routers/images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:07:50.497426 httpbinx-1.3.1/httpbinx/routers/inspection/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-30 17:07:39.000000 httpbinx-1.3.1/httpbinx/routers/inspection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-30 17:07:39.000000 httpbinx-1.3.1/httpbinx/routers/inspection/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-30 17:07:39.000000 httpbinx-1.3.1/httpbinx/routers/inspection/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-30 17:07:39.000000 httpbinx-1.3.1/httpbinx/routers/redirects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4996 2023-05-30 17:07:39.000000 httpbinx-1.3.1/httpbinx/routers/responseformats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-30 17:07:39.000000 httpbinx-1.3.1/httpbinx/routers/statuscodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-30 17:07:39.000000 httpbinx-1.3.1/httpbinx/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:07:50.497426 httpbinx-1.3.1/httpbinx/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    14058 2023-05-30 17:07:39.000000 httpbinx-1.3.1/httpbinx/static/UTF-8-demo.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-30 17:07:39.000000 httpbinx-1.3.1/httpbinx/static/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:07:50.501426 httpbinx-1.3.1/httpbinx/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-05-30 17:07:39.000000 httpbinx-1.3.1/httpbinx/static/images/httbinx_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-05-30 17:07:39.000000 httpbinx-1.3.1/httpbinx/static/images/httpbinx_cover.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35588 2023-05-30 17:07:39.000000 httpbinx-1.3.1/httpbinx/static/images/jackal.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-05-30 17:07:39.000000 httpbinx-1.3.1/httpbinx/static/images/pig_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-05-30 17:07:39.000000 httpbinx-1.3.1/httpbinx/static/images/svg_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10568 2023-05-30 17:07:39.000000 httpbinx-1.3.1/httpbinx/static/images/wolf_1.webp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:07:50.501426 httpbinx-1.3.1/httpbinx/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-05-30 17:07:39.000000 httpbinx-1.3.1/httpbinx/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-05-30 17:07:39.000000 httpbinx-1.3.1/httpbinx/templates/moby.html
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-30 17:07:39.000000 httpbinx-1.3.1/httpbinx/templates/sample.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-30 17:07:39.000000 httpbinx-1.3.1/httpbinx/templates/trackingscripts.html
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-30 17:07:39.000000 httpbinx-1.3.1/httpbinx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:07:50.497426 httpbinx-1.3.1/httpbinx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-30 17:07:50.000000 httpbinx-1.3.1/httpbinx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-30 17:07:50.000000 httpbinx-1.3.1/httpbinx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 17:07:50.000000 httpbinx-1.3.1/httpbinx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-30 17:07:50.000000 httpbinx-1.3.1/httpbinx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-30 17:07:50.000000 httpbinx-1.3.1/httpbinx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 17:07:50.501426 httpbinx-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-30 17:07:39.000000 httpbinx-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:07:50.501426 httpbinx-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-30 17:07:39.000000 httpbinx-1.3.1/tests/test_anything.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-30 17:07:39.000000 httpbinx-1.3.1/tests/test_dynamic_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-30 17:07:39.000000 httpbinx-1.3.1/tests/test_http_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-30 17:07:39.000000 httpbinx-1.3.1/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-30 17:07:39.000000 httpbinx-1.3.1/tests/test_redirects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-30 17:07:39.000000 httpbinx-1.3.1/tests/test_request_inspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-30 17:07:39.000000 httpbinx-1.3.1/tests/test_response_formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-30 17:07:39.000000 httpbinx-1.3.1/tests/test_status_codes.py
```

### Comparing `httpbinx-1.3.0/LICENSE` & `httpbinx-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.0/PKG-INFO` & `httpbinx-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpbinx
-Version: 1.3.0
+Version: 1.3.1
 Summary: HTTP Request & Response Service, written in Python + FastAPI.
 Home-page: https://github.com/imleowoo/httpbinx
 Author: Leo
 Author-email: imleowoo@outlook.com
 Maintainer: Leo
 Maintainer-email: imleowoo@outlook.com
 License: MIT
```

### Comparing `httpbinx-1.3.0/httpbinx/constants.py` & `httpbinx-1.3.1/httpbinx/constants.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.0/httpbinx/helpers.py` & `httpbinx-1.3.1/httpbinx/helpers.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.0/httpbinx/main.py` & `httpbinx-1.3.1/httpbinx/main.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.0/httpbinx/routers/__init__.py` & `httpbinx-1.3.1/httpbinx/routers/__init__.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.0/httpbinx/routers/anything.py` & `httpbinx-1.3.1/httpbinx/routers/anything.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.0/httpbinx/routers/auth.py` & `httpbinx-1.3.1/httpbinx/routers/auth.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.0/httpbinx/routers/cookies.py` & `httpbinx-1.3.1/httpbinx/routers/cookies.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.0/httpbinx/routers/dynamicdata.py` & `httpbinx-1.3.1/httpbinx/routers/dynamicdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
     body = ''
     link = '<a href="{href}">{text}</a> '
     for i in range(n):
         if i == offset:
             body += f'{i} '
         else:
             body += link.format(
-                href=f'/api/links/{n}/{i}',  # TODO how to use router.url_path_for?
+                href=f'/links/{n}/{i}',  # TODO how to use router.url_path_for?
                 text=i
             )
     return HTMLResponse(content=html.format(body=body))
 
 
 @router.get(
     '/range/{numbytes}',
```

### Comparing `httpbinx-1.3.0/httpbinx/routers/httpmethods.py` & `httpbinx-1.3.1/httpbinx/routers/httpmethods.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.0/httpbinx/routers/images.py` & `httpbinx-1.3.1/httpbinx/routers/images.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.0/httpbinx/routers/inspection/request.py` & `httpbinx-1.3.1/httpbinx/routers/inspection/request.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.0/httpbinx/routers/inspection/response.py` & `httpbinx-1.3.1/httpbinx/routers/inspection/response.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.0/httpbinx/routers/redirects.py` & `httpbinx-1.3.1/httpbinx/routers/redirects.py`

 * *Files 5% similar despite different names*

```diff
@@ -87,18 +87,18 @@
 async def relative_redirect_n_times(
         *,
         n: int = Path(..., title='Redirects n times.', gt=0, le=10),
         request: Request
 ):
     resp = Response(status_code=status.HTTP_302_FOUND)
     if n == 1:
-        resp.headers['Location'] = request.url_for('get')
+        resp.headers['Location'] = str(request.url_for('get'))
         return resp
     redirect_name = relative_redirect_n_times.__name__
-    resp.headers['Location'] = request.url_for(redirect_name, n=n - 1)
+    resp.headers['Location'] = str(request.url_for(redirect_name, n=n - 1))
     return resp
 
 
 def _redirect(request: Request, type_: RedirectTypes, n: int):
     # TODO external
     # "absolute_redirect" and "relative_redirect" options are not effective.
     func_prefix = f'{type_}_n_times'
```

### Comparing `httpbinx-1.3.0/httpbinx/routers/responseformats.py` & `httpbinx-1.3.1/httpbinx/routers/responseformats.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.0/httpbinx/routers/statuscodes.py` & `httpbinx-1.3.1/httpbinx/routers/statuscodes.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.0/httpbinx/schemas.py` & `httpbinx-1.3.1/httpbinx/schemas.py`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.0/httpbinx/static/UTF-8-demo.txt` & `httpbinx-1.3.1/httpbinx/static/UTF-8-demo.txt`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.0/httpbinx/static/favicon.png` & `httpbinx-1.3.1/httpbinx/static/favicon.png`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.0/httpbinx/static/images/httbinx_logo.png` & `httpbinx-1.3.1/httpbinx/static/images/httbinx_logo.png`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.0/httpbinx/static/images/httpbinx_cover.png` & `httpbinx-1.3.1/httpbinx/static/images/httpbinx_cover.png`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.0/httpbinx/static/images/jackal.jpg` & `httpbinx-1.3.1/httpbinx/static/images/jackal.jpg`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.0/httpbinx/static/images/pig_icon.png` & `httpbinx-1.3.1/httpbinx/static/images/pig_icon.png`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.0/httpbinx/static/images/svg_logo.svg` & `httpbinx-1.3.1/httpbinx/static/images/svg_logo.svg`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.0/httpbinx/static/images/wolf_1.webp` & `httpbinx-1.3.1/httpbinx/static/images/wolf_1.webp`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.0/httpbinx/templates/index.html` & `httpbinx-1.3.1/httpbinx/templates/index.html`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.0/httpbinx/templates/moby.html` & `httpbinx-1.3.1/httpbinx/templates/moby.html`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.0/httpbinx/templates/sample.xml` & `httpbinx-1.3.1/httpbinx/templates/sample.xml`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.0/httpbinx/templates/trackingscripts.html` & `httpbinx-1.3.1/httpbinx/templates/trackingscripts.html`

 * *Files identical despite different names*

### Comparing `httpbinx-1.3.0/httpbinx.egg-info/PKG-INFO` & `httpbinx-1.3.1/httpbinx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpbinx
-Version: 1.3.0
+Version: 1.3.1
 Summary: HTTP Request & Response Service, written in Python + FastAPI.
 Home-page: https://github.com/imleowoo/httpbinx
 Author: Leo
 Author-email: imleowoo@outlook.com
 Maintainer: Leo
 Maintainer-email: imleowoo@outlook.com
 License: MIT
```

### Comparing `httpbinx-1.3.0/httpbinx.egg-info/SOURCES.txt` & `httpbinx-1.3.1/httpbinx.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -35,8 +35,16 @@
 httpbinx/static/images/jackal.jpg
 httpbinx/static/images/pig_icon.png
 httpbinx/static/images/svg_logo.svg
 httpbinx/static/images/wolf_1.webp
 httpbinx/templates/index.html
 httpbinx/templates/moby.html
 httpbinx/templates/sample.xml
-httpbinx/templates/trackingscripts.html
+httpbinx/templates/trackingscripts.html
+tests/test_anything.py
+tests/test_dynamic_data.py
+tests/test_http_methods.py
+tests/test_images.py
+tests/test_redirects.py
+tests/test_request_inspection.py
+tests/test_response_formats.py
+tests/test_status_codes.py
```

### Comparing `httpbinx-1.3.0/setup.py` & `httpbinx-1.3.1/setup.py`

 * *Files identical despite different names*

