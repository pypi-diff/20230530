# Comparing `tmp/ms_identity_web-0.0.1.tar.gz` & `tmp/ms_identity_web-0.0.2.tar.gz`

## Comparing `ms_identity_web-0.0.1.tar` & `ms_identity_web-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ms_identity_web-0.0.1/CHANGELOG.md
--rw-r--r--   0        0        0     4017 2020-02-02 00:00:00.000000 ms_identity_web-0.0.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 ms_identity_web-0.0.1/aad.b2c.config.json
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 ms_identity_web-0.0.1/aad.django.config.json
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 ms_identity_web-0.0.1/aad.flask.config.json
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 ms_identity_web-0.0.1/requirements.txt
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 ms_identity_web-0.0.1/setup.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 ms_identity_web-0.0.1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 ms_identity_web-0.0.1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 ms_identity_web-0.0.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0    15694 2020-02-02 00:00:00.000000 ms_identity_web-0.0.1/ms_identity_web/__init__.py
--rw-r--r--   0        0        0     9509 2020-02-02 00:00:00.000000 ms_identity_web-0.0.1/ms_identity_web/adapters.py
--rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 ms_identity_web-0.0.1/ms_identity_web/configuration.py
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 ms_identity_web-0.0.1/ms_identity_web/constants.py
--rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 ms_identity_web-0.0.1/ms_identity_web/context.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 ms_identity_web-0.0.1/ms_identity_web/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ms_identity_web-0.0.1/ms_identity_web/django/__init__.py
--rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 ms_identity_web-0.0.1/ms_identity_web/django/adapter.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 ms_identity_web-0.0.1/ms_identity_web/django/middleware.py
--rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 ms_identity_web-0.0.1/ms_identity_web/django/msal_views_and_urls.py
--rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 ms_identity_web-0.0.1/ms_identity_web/flask_blueprint/__init__.py
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 ms_identity_web-0.0.1/.gitignore
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 ms_identity_web-0.0.1/LICENSE
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 ms_identity_web-0.0.1/LICENSE.md
--rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 ms_identity_web-0.0.1/README.md
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 ms_identity_web-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     6474 2020-02-02 00:00:00.000000 ms_identity_web-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ms_identity_web-0.0.2/CHANGELOG.md
+-rw-r--r--   0        0        0     4017 2020-02-02 00:00:00.000000 ms_identity_web-0.0.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 ms_identity_web-0.0.2/aad.b2c.config.json
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 ms_identity_web-0.0.2/aad.django.config.json
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 ms_identity_web-0.0.2/aad.flask.config.json
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 ms_identity_web-0.0.2/requirements.txt
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 ms_identity_web-0.0.2/setup.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 ms_identity_web-0.0.2/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 ms_identity_web-0.0.2/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 ms_identity_web-0.0.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0    15694 2020-02-02 00:00:00.000000 ms_identity_web-0.0.2/ms_identity_web/__init__.py
+-rw-r--r--   0        0        0     9509 2020-02-02 00:00:00.000000 ms_identity_web-0.0.2/ms_identity_web/adapters.py
+-rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 ms_identity_web-0.0.2/ms_identity_web/configuration.py
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 ms_identity_web-0.0.2/ms_identity_web/constants.py
+-rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 ms_identity_web-0.0.2/ms_identity_web/context.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 ms_identity_web-0.0.2/ms_identity_web/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ms_identity_web-0.0.2/ms_identity_web/django/__init__.py
+-rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 ms_identity_web-0.0.2/ms_identity_web/django/adapter.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 ms_identity_web-0.0.2/ms_identity_web/django/middleware.py
+-rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 ms_identity_web-0.0.2/ms_identity_web/django/msal_views_and_urls.py
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 ms_identity_web-0.0.2/ms_identity_web/flask_blueprint/__init__.py
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 ms_identity_web-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 ms_identity_web-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 ms_identity_web-0.0.2/LICENSE.md
+-rw-r--r--   0        0        0     4773 2020-02-02 00:00:00.000000 ms_identity_web-0.0.2/README.md
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 ms_identity_web-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6461 2020-02-02 00:00:00.000000 ms_identity_web-0.0.2/PKG-INFO
```

### Comparing `ms_identity_web-0.0.1/CONTRIBUTING.md` & `ms_identity_web-0.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ms_identity_web-0.0.1/aad.b2c.config.json` & `ms_identity_web-0.0.2/aad.b2c.config.json`

 * *Files identical despite different names*

### Comparing `ms_identity_web-0.0.1/aad.django.config.json` & `ms_identity_web-0.0.2/aad.django.config.json`

 * *Files identical despite different names*

### Comparing `ms_identity_web-0.0.1/aad.flask.config.json` & `ms_identity_web-0.0.2/aad.flask.config.json`

 * *Files identical despite different names*

### Comparing `ms_identity_web-0.0.1/.github/ISSUE_TEMPLATE.md` & `ms_identity_web-0.0.2/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `ms_identity_web-0.0.1/.github/PULL_REQUEST_TEMPLATE.md` & `ms_identity_web-0.0.2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `ms_identity_web-0.0.1/ms_identity_web/__init__.py` & `ms_identity_web-0.0.2/ms_identity_web/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_identity_web-0.0.1/ms_identity_web/adapters.py` & `ms_identity_web-0.0.2/ms_identity_web/adapters.py`

 * *Files identical despite different names*

### Comparing `ms_identity_web-0.0.1/ms_identity_web/configuration.py` & `ms_identity_web-0.0.2/ms_identity_web/configuration.py`

 * *Files identical despite different names*

### Comparing `ms_identity_web-0.0.1/ms_identity_web/constants.py` & `ms_identity_web-0.0.2/ms_identity_web/constants.py`

 * *Files identical despite different names*

### Comparing `ms_identity_web-0.0.1/ms_identity_web/context.py` & `ms_identity_web-0.0.2/ms_identity_web/context.py`

 * *Files identical despite different names*

### Comparing `ms_identity_web-0.0.1/ms_identity_web/errors.py` & `ms_identity_web-0.0.2/ms_identity_web/errors.py`

 * *Files identical despite different names*

### Comparing `ms_identity_web-0.0.1/ms_identity_web/django/adapter.py` & `ms_identity_web-0.0.2/ms_identity_web/django/adapter.py`

 * *Files identical despite different names*

### Comparing `ms_identity_web-0.0.1/ms_identity_web/django/middleware.py` & `ms_identity_web-0.0.2/ms_identity_web/django/middleware.py`

 * *Files identical despite different names*

### Comparing `ms_identity_web-0.0.1/ms_identity_web/django/msal_views_and_urls.py` & `ms_identity_web-0.0.2/ms_identity_web/django/msal_views_and_urls.py`

 * *Files identical despite different names*

### Comparing `ms_identity_web-0.0.1/ms_identity_web/flask_blueprint/__init__.py` & `ms_identity_web-0.0.2/ms_identity_web/flask_blueprint/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_identity_web-0.0.1/.gitignore` & `ms_identity_web-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ms_identity_web-0.0.1/LICENSE` & `ms_identity_web-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_identity_web-0.0.1/LICENSE.md` & `ms_identity_web-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ms_identity_web-0.0.1/README.md` & `ms_identity_web-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ms_identity_web-0.0.1/PKG-INFO` & `ms_identity_web-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ms-identity-web
-Version: 0.0.1
-Summary: Libreria para autenticacion con Azure AD
-Project-URL: Homepage, https://github.com/aabedoya/ms-identity-web
+Version: 0.0.2
+Summary: Autenticación Azure DA
+Project-URL: Homepage, https://github.com/aabedoya/ms-identity-web/
 Project-URL: Bug Tracker, https://github.com/aabedoya/ms-identity-web/issues
-Author-email: andresbedoyagomez <andresbedoyagomez@gmail.com>
+Author-email: Alvaro Andres Bedoya <andresbedoyagomez@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alvaro Andrés Bedoya Gómez
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -27,15 +27,15 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # MS Identity Python Common
 
 This repository contains a set of code that is shared amongst the various Python samples for the Microsoft Identity Platform. This is a work in progress and we'd love to hear your feedback, comments and contributions.
 
 ## Features
```

