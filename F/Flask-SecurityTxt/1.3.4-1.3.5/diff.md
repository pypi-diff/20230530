# Comparing `tmp/Flask-SecurityTxt-1.3.4.tar.gz` & `tmp/Flask-SecurityTxt-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-SecurityTxt-1.3.4.tar", last modified: Sun Jan 29 09:04:56 2023, max compression
+gzip compressed data, was "Flask-SecurityTxt-1.3.5.tar", last modified: Tue May 30 14:59:08 2023, max compression
```

## Comparing `Flask-SecurityTxt-1.3.4.tar` & `Flask-SecurityTxt-1.3.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 09:04:56.050604 Flask-SecurityTxt-1.3.4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 09:04:56.049604 Flask-SecurityTxt-1.3.4/Flask_SecurityTxt.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8740 2023-01-29 09:04:56.000000 Flask-SecurityTxt-1.3.4/Flask_SecurityTxt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      290 2023-01-29 09:04:56.000000 Flask-SecurityTxt-1.3.4/Flask_SecurityTxt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-29 09:04:56.000000 Flask-SecurityTxt-1.3.4/Flask_SecurityTxt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-01-29 09:04:56.000000 Flask-SecurityTxt-1.3.4/Flask_SecurityTxt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-01-29 09:04:56.000000 Flask-SecurityTxt-1.3.4/Flask_SecurityTxt.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    35075 2023-01-29 09:04:46.000000 Flask-SecurityTxt-1.3.4/LICENCE
--rw-r--r--   0 root         (0) root         (0)     8740 2023-01-29 09:04:56.049604 Flask-SecurityTxt-1.3.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7945 2023-01-29 09:04:46.000000 Flask-SecurityTxt-1.3.4/README.MD
--rw-rw-rw-   0 root         (0) root         (0)    11280 2023-01-29 09:04:46.000000 Flask-SecurityTxt-1.3.4/flask_security_txt.py
--rw-rw-rw-   0 root         (0) root         (0)      979 2023-01-29 09:04:46.000000 Flask-SecurityTxt-1.3.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-01-29 09:04:56.050604 Flask-SecurityTxt-1.3.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-29 09:04:56.049604 Flask-SecurityTxt-1.3.4/test/
--rw-rw-rw-   0 root         (0) root         (0)     1261 2023-01-29 09:04:46.000000 Flask-SecurityTxt-1.3.4/test/test_flask_security_txt.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:59:08.432989 Flask-SecurityTxt-1.3.5/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:59:08.432989 Flask-SecurityTxt-1.3.5/Flask_SecurityTxt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8740 2023-05-30 14:59:08.000000 Flask-SecurityTxt-1.3.5/Flask_SecurityTxt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      290 2023-05-30 14:59:08.000000 Flask-SecurityTxt-1.3.5/Flask_SecurityTxt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 14:59:08.000000 Flask-SecurityTxt-1.3.5/Flask_SecurityTxt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-30 14:59:08.000000 Flask-SecurityTxt-1.3.5/Flask_SecurityTxt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-30 14:59:08.000000 Flask-SecurityTxt-1.3.5/Flask_SecurityTxt.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    35075 2023-05-30 14:59:00.000000 Flask-SecurityTxt-1.3.5/LICENCE
+-rw-r--r--   0 root         (0) root         (0)     8740 2023-05-30 14:59:08.432989 Flask-SecurityTxt-1.3.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7945 2023-05-30 14:59:00.000000 Flask-SecurityTxt-1.3.5/README.MD
+-rw-rw-rw-   0 root         (0) root         (0)    11465 2023-05-30 14:59:00.000000 Flask-SecurityTxt-1.3.5/flask_security_txt.py
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2023-05-30 14:59:00.000000 Flask-SecurityTxt-1.3.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 14:59:08.432989 Flask-SecurityTxt-1.3.5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:59:08.432989 Flask-SecurityTxt-1.3.5/test/
+-rw-rw-rw-   0 root         (0) root         (0)     1261 2023-05-30 14:59:00.000000 Flask-SecurityTxt-1.3.5/test/test_flask_security_txt.py
```

### Comparing `Flask-SecurityTxt-1.3.4/Flask_SecurityTxt.egg-info/PKG-INFO` & `Flask-SecurityTxt-1.3.5/Flask_SecurityTxt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-SecurityTxt
-Version: 1.3.4
+Version: 1.3.5
 Summary: Flask-SecurityTxt is a Flask extension for creating and serving security.txt files which provide information on reporting security vulnerabilities.
 Author-email: "M. P. van de Weerd" <michael@parcifal.dev>
 License: LICENCE
 Project-URL: Homepage, https://gitlab.com/parcifal/flask-security-txt
 Project-URL: Bug Tracker, https://gitlab.com/parcifal/flask-security-txt/-/issues
 Keywords: web,security,security.txt
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Flask-SecurityTxt-1.3.4/LICENCE` & `Flask-SecurityTxt-1.3.5/LICENCE`

 * *Files identical despite different names*

### Comparing `Flask-SecurityTxt-1.3.4/PKG-INFO` & `Flask-SecurityTxt-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-SecurityTxt
-Version: 1.3.4
+Version: 1.3.5
 Summary: Flask-SecurityTxt is a Flask extension for creating and serving security.txt files which provide information on reporting security vulnerabilities.
 Author-email: "M. P. van de Weerd" <michael@parcifal.dev>
 License: LICENCE
 Project-URL: Homepage, https://gitlab.com/parcifal/flask-security-txt
 Project-URL: Bug Tracker, https://gitlab.com/parcifal/flask-security-txt/-/issues
 Keywords: web,security,security.txt
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Flask-SecurityTxt-1.3.4/README.MD` & `Flask-SecurityTxt-1.3.5/README.MD`

 * *Files identical despite different names*

### Comparing `Flask-SecurityTxt-1.3.4/flask_security_txt.py` & `Flask-SecurityTxt-1.3.5/flask_security_txt.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 from collections.abc import Iterable
 
 from datetime import datetime as dt, timedelta as td, timezone as tz
 from importlib.metadata import version
 
 from flask import Flask, Response, request, url_for, current_app
+from flask_babel import get_babel
 from pgpy import PGPKey, PGPMessage
 from werkzeug.routing import BuildError
 
 DEFAULT_HEADER = None
 
 DEFAULT_FOOTER = """
 #
@@ -36,26 +37,28 @@
     """
 
     # pylint: disable=too-many-arguments
     def __init__(self, app: Flask = None,
                  default_endpoint: str = "security_txt",
                  default_contact_mailbox: str = "security",
                  default_expires_offset: tuple = (0, 0, 0, 0, 0, 0, 1),
+                 default_preferred_languages: tuple = ("en", ),
                  default_canonical: str = None,
                  default_dir: str = ".well-known",
                  default_file_name: str = "security.txt",
                  default_sign_key: str = None,
                  default_header: str = DEFAULT_HEADER,
                  default_footer: str = DEFAULT_FOOTER):
         self.app = app
         self.sign_key = None
 
         self._default_endpoint = default_endpoint
         self._default_contact_mailbox = default_contact_mailbox
         self._default_expires_offset = default_expires_offset
+        self._default_preferred_languages = default_preferred_languages
         self._default_canonical = default_canonical or default_endpoint
         self._default_dir = default_dir
         self._default_file_name = default_file_name
         self._default_sign_key = default_sign_key
         self._default_header = default_header
         self._default_footer = default_footer
 
@@ -277,25 +280,25 @@
     def _get_field_value_preferred_languages(self):
         """
         @return:
             The value of the preferred languages field.
         """
         value = current_app.config.get("SECURITY_TXT_PREFERRED_LANGUAGES")
 
+        if "babel" not in current_app.extensions:
+            value = self._default_preferred_languages or ""
         if isinstance(value, str):
             return value
         if isinstance(value, (list, tuple)):
             return ", ".join(value)
-        if not hasattr(current_app, "babel_instance"):
-            return ""
 
-        babel = getattr(current_app, "babel_instance")
+        babel = get_babel()
 
         return ", ".join([
-            t.language for t in getattr(babel, "list_translations")()
+            t.language for t in getattr(babel.instance, "list_translations")()
         ])
 
     def _get_field_value_canonical(self):
         """
         @return:
             The value of the canonical field.
         """
```

### Comparing `Flask-SecurityTxt-1.3.4/pyproject.toml` & `Flask-SecurityTxt-1.3.5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires       = [ "setuptools>=61.0" ]
 build-backend  = "setuptools.build_meta"
 
 [project]
 name          = "Flask-SecurityTxt"
-version       = "1.3.4"
+version       = "1.3.5"
 description   = "Flask-SecurityTxt is a Flask extension for creating and serving security.txt files which provide information on reporting security vulnerabilities."
 readme        = "README.MD"
 authors       = [
     { name = "M. P. van de Weerd", email = "michael@parcifal.dev" }
 ]
-dependencies  = [ "flask", "pgpy" ]
-keywords      = [ "web", "security", "security.txt" ]
-license       = { text = "LICENCE" }
-classifiers   = [
+dependencies           = [ "flask", "flask-babel", "pgpy" ]
+keywords               = [ "web", "security", "security.txt" ]
+license                = { text = "LICENCE" }
+classifiers            = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Framework :: Flask",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)"
 ]
```

### Comparing `Flask-SecurityTxt-1.3.4/test/test_flask_security_txt.py` & `Flask-SecurityTxt-1.3.5/test/test_flask_security_txt.py`

 * *Files identical despite different names*

