# Comparing `tmp/cattrs-23.1.0.tar.gz` & `tmp/cattrs-23.1.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cattrs-23.1.0.tar", max compression
+gzip compressed data, was "cattrs-23.1.0rc0.tar", max compression
```

## Comparing `cattrs-23.1.0.tar` & `cattrs-23.1.0rc0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1074 2022-02-11 01:34:09.478875 cattrs-23.1.0/LICENSE
--rw-r--r--   0        0        0     7516 2023-04-15 23:55:47.832298 cattrs-23.1.0/README.md
--rw-r--r--   0        0        0     2450 2023-05-30 15:08:37.688102 cattrs-23.1.0/pyproject.toml
--rw-r--r--   0        0        0      906 2022-04-16 01:20:23.203198 cattrs-23.1.0/src/cattr/__init__.py
--rw-r--r--   0        0        0      192 2022-04-16 01:20:23.203198 cattrs-23.1.0/src/cattr/converters.py
--rw-r--r--   0        0        0      103 2022-04-16 01:20:23.203198 cattrs-23.1.0/src/cattr/disambiguators.py
--rw-r--r--   0        0        0      125 2022-04-16 01:20:23.203198 cattrs-23.1.0/src/cattr/dispatch.py
--rw-r--r--   0        0        0      343 2022-07-06 00:23:52.229650 cattrs-23.1.0/src/cattr/errors.py
--rw-r--r--   0        0        0      520 2022-02-11 01:34:09.486876 cattrs-23.1.0/src/cattr/gen.py
--rw-r--r--   0        0        0       78 2022-04-16 01:20:23.203198 cattrs-23.1.0/src/cattr/preconf/__init__.py
--rw-r--r--   0        0        0      194 2023-03-02 01:10:10.360770 cattrs-23.1.0/src/cattr/preconf/bson.py
--rw-r--r--   0        0        0      205 2023-03-02 01:10:10.360770 cattrs-23.1.0/src/cattr/preconf/json.py
--rw-r--r--   0        0        0      206 2023-03-02 01:10:10.360770 cattrs-23.1.0/src/cattr/preconf/msgpack.py
--rw-r--r--   0        0        0      202 2023-03-02 01:10:10.360770 cattrs-23.1.0/src/cattr/preconf/orjson.py
--rw-r--r--   0        0        0      202 2023-03-02 01:10:10.360770 cattrs-23.1.0/src/cattr/preconf/pyyaml.py
--rw-r--r--   0        0        0      206 2023-03-02 01:10:10.360770 cattrs-23.1.0/src/cattr/preconf/tomlkit.py
--rw-r--r--   0        0        0      198 2023-03-02 01:10:10.360770 cattrs-23.1.0/src/cattr/preconf/ujson.py
--rw-r--r--   0        0        0        0 2022-02-11 01:34:09.486876 cattrs-23.1.0/src/cattr/py.typed
--rw-r--r--   0        0        0     1631 2023-04-15 23:55:47.836298 cattrs-23.1.0/src/cattrs/__init__.py
--rw-r--r--   0        0        0    15501 2023-05-23 23:14:04.606233 cattrs-23.1.0/src/cattrs/_compat.py
--rw-r--r--   0        0        0      678 2022-04-10 01:46:50.855243 cattrs-23.1.0/src/cattrs/_generics.py
--rw-r--r--   0        0        0    41450 2023-05-22 17:11:08.762741 cattrs-23.1.0/src/cattrs/converters.py
--rw-r--r--   0        0        0     2243 2023-03-02 01:10:10.360770 cattrs-23.1.0/src/cattrs/disambiguators.py
--rw-r--r--   0        0        0     4654 2023-03-02 01:10:10.360770 cattrs-23.1.0/src/cattrs/dispatch.py
--rw-r--r--   0        0        0     3850 2023-04-15 23:55:47.836298 cattrs-23.1.0/src/cattrs/errors.py
--rw-r--r--   0        0        0    26575 2023-05-22 17:11:08.766741 cattrs-23.1.0/src/cattrs/gen/__init__.py
--rw-r--r--   0        0        0      490 2023-05-22 17:11:08.766741 cattrs-23.1.0/src/cattrs/gen/_consts.py
--rw-r--r--   0        0        0     1503 2023-05-22 17:11:08.766741 cattrs-23.1.0/src/cattrs/gen/_generics.py
--rw-r--r--   0        0        0     1017 2023-05-22 17:11:08.766741 cattrs-23.1.0/src/cattrs/gen/_lc.py
--rw-r--r--   0        0        0     1737 2023-05-22 17:11:08.770741 cattrs-23.1.0/src/cattrs/gen/_shared.py
--rw-r--r--   0        0        0    22059 2023-05-22 17:11:08.774741 cattrs-23.1.0/src/cattrs/gen/typeddicts.py
--rw-r--r--   0        0        0      165 2022-04-16 01:20:23.203198 cattrs-23.1.0/src/cattrs/preconf/__init__.py
--rw-r--r--   0        0        0     3087 2023-05-22 17:11:08.782741 cattrs-23.1.0/src/cattrs/preconf/bson.py
--rw-r--r--   0        0        0     1290 2023-05-22 17:11:08.786741 cattrs-23.1.0/src/cattrs/preconf/cbor2.py
--rw-r--r--   0        0        0     1615 2023-05-22 17:11:08.786741 cattrs-23.1.0/src/cattrs/preconf/json.py
--rw-r--r--   0        0        0     1302 2023-05-22 17:11:08.790742 cattrs-23.1.0/src/cattrs/preconf/msgpack.py
--rw-r--r--   0        0        0     2573 2023-05-22 17:11:08.798742 cattrs-23.1.0/src/cattrs/preconf/orjson.py
--rw-r--r--   0        0        0     1320 2023-05-22 17:11:08.798742 cattrs-23.1.0/src/cattrs/preconf/pyyaml.py
--rw-r--r--   0        0        0     2534 2023-05-22 17:11:08.802742 cattrs-23.1.0/src/cattrs/preconf/tomlkit.py
--rw-r--r--   0        0        0     1525 2023-05-22 17:11:08.806742 cattrs-23.1.0/src/cattrs/preconf/ujson.py
--rw-r--r--   0        0        0        0 2022-02-11 01:34:09.486876 cattrs-23.1.0/src/cattrs/py.typed
--rw-r--r--   0        0        0      192 2023-05-22 17:11:08.810742 cattrs-23.1.0/src/cattrs/strategies/__init__.py
--rw-r--r--   0        0        0     8677 2023-05-22 17:16:50.127698 cattrs-23.1.0/src/cattrs/strategies/_subclasses.py
--rw-r--r--   0        0        0     3440 2023-05-22 17:11:08.814742 cattrs-23.1.0/src/cattrs/strategies/_unions.py
--rw-r--r--   0        0        0     4360 2023-05-22 17:11:08.814742 cattrs-23.1.0/src/cattrs/v.py
--rw-r--r--   0        0        0     9250 1970-01-01 00:00:00.000000 cattrs-23.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2022-02-11 01:34:09.478875 cattrs-23.1.0rc0/LICENSE
+-rw-r--r--   0        0        0     7516 2023-04-15 23:55:47.832298 cattrs-23.1.0rc0/README.md
+-rw-r--r--   0        0        0     2453 2023-05-25 23:51:12.412451 cattrs-23.1.0rc0/pyproject.toml
+-rw-r--r--   0        0        0      906 2022-04-16 01:20:23.203198 cattrs-23.1.0rc0/src/cattr/__init__.py
+-rw-r--r--   0        0        0      192 2022-04-16 01:20:23.203198 cattrs-23.1.0rc0/src/cattr/converters.py
+-rw-r--r--   0        0        0      103 2022-04-16 01:20:23.203198 cattrs-23.1.0rc0/src/cattr/disambiguators.py
+-rw-r--r--   0        0        0      125 2022-04-16 01:20:23.203198 cattrs-23.1.0rc0/src/cattr/dispatch.py
+-rw-r--r--   0        0        0      343 2022-07-06 00:23:52.229650 cattrs-23.1.0rc0/src/cattr/errors.py
+-rw-r--r--   0        0        0      520 2022-02-11 01:34:09.486876 cattrs-23.1.0rc0/src/cattr/gen.py
+-rw-r--r--   0        0        0       78 2022-04-16 01:20:23.203198 cattrs-23.1.0rc0/src/cattr/preconf/__init__.py
+-rw-r--r--   0        0        0      194 2023-03-02 01:10:10.360770 cattrs-23.1.0rc0/src/cattr/preconf/bson.py
+-rw-r--r--   0        0        0      205 2023-03-02 01:10:10.360770 cattrs-23.1.0rc0/src/cattr/preconf/json.py
+-rw-r--r--   0        0        0      206 2023-03-02 01:10:10.360770 cattrs-23.1.0rc0/src/cattr/preconf/msgpack.py
+-rw-r--r--   0        0        0      202 2023-03-02 01:10:10.360770 cattrs-23.1.0rc0/src/cattr/preconf/orjson.py
+-rw-r--r--   0        0        0      202 2023-03-02 01:10:10.360770 cattrs-23.1.0rc0/src/cattr/preconf/pyyaml.py
+-rw-r--r--   0        0        0      206 2023-03-02 01:10:10.360770 cattrs-23.1.0rc0/src/cattr/preconf/tomlkit.py
+-rw-r--r--   0        0        0      198 2023-03-02 01:10:10.360770 cattrs-23.1.0rc0/src/cattr/preconf/ujson.py
+-rw-r--r--   0        0        0        0 2022-02-11 01:34:09.486876 cattrs-23.1.0rc0/src/cattr/py.typed
+-rw-r--r--   0        0        0     1631 2023-04-15 23:55:47.836298 cattrs-23.1.0rc0/src/cattrs/__init__.py
+-rw-r--r--   0        0        0    15501 2023-05-23 23:14:04.606233 cattrs-23.1.0rc0/src/cattrs/_compat.py
+-rw-r--r--   0        0        0      678 2022-04-10 01:46:50.855243 cattrs-23.1.0rc0/src/cattrs/_generics.py
+-rw-r--r--   0        0        0    41450 2023-05-22 17:11:08.762741 cattrs-23.1.0rc0/src/cattrs/converters.py
+-rw-r--r--   0        0        0     2243 2023-03-02 01:10:10.360770 cattrs-23.1.0rc0/src/cattrs/disambiguators.py
+-rw-r--r--   0        0        0     4654 2023-03-02 01:10:10.360770 cattrs-23.1.0rc0/src/cattrs/dispatch.py
+-rw-r--r--   0        0        0     3850 2023-04-15 23:55:47.836298 cattrs-23.1.0rc0/src/cattrs/errors.py
+-rw-r--r--   0        0        0    26575 2023-05-22 17:11:08.766741 cattrs-23.1.0rc0/src/cattrs/gen/__init__.py
+-rw-r--r--   0        0        0      490 2023-05-22 17:11:08.766741 cattrs-23.1.0rc0/src/cattrs/gen/_consts.py
+-rw-r--r--   0        0        0     1503 2023-05-22 17:11:08.766741 cattrs-23.1.0rc0/src/cattrs/gen/_generics.py
+-rw-r--r--   0        0        0     1017 2023-05-22 17:11:08.766741 cattrs-23.1.0rc0/src/cattrs/gen/_lc.py
+-rw-r--r--   0        0        0     1737 2023-05-22 17:11:08.770741 cattrs-23.1.0rc0/src/cattrs/gen/_shared.py
+-rw-r--r--   0        0        0    22059 2023-05-22 17:11:08.774741 cattrs-23.1.0rc0/src/cattrs/gen/typeddicts.py
+-rw-r--r--   0        0        0      165 2022-04-16 01:20:23.203198 cattrs-23.1.0rc0/src/cattrs/preconf/__init__.py
+-rw-r--r--   0        0        0     3087 2023-05-22 17:11:08.782741 cattrs-23.1.0rc0/src/cattrs/preconf/bson.py
+-rw-r--r--   0        0        0     1290 2023-05-22 17:11:08.786741 cattrs-23.1.0rc0/src/cattrs/preconf/cbor2.py
+-rw-r--r--   0        0        0     1615 2023-05-22 17:11:08.786741 cattrs-23.1.0rc0/src/cattrs/preconf/json.py
+-rw-r--r--   0        0        0     1302 2023-05-22 17:11:08.790742 cattrs-23.1.0rc0/src/cattrs/preconf/msgpack.py
+-rw-r--r--   0        0        0     2573 2023-05-22 17:11:08.798742 cattrs-23.1.0rc0/src/cattrs/preconf/orjson.py
+-rw-r--r--   0        0        0     1320 2023-05-22 17:11:08.798742 cattrs-23.1.0rc0/src/cattrs/preconf/pyyaml.py
+-rw-r--r--   0        0        0     2534 2023-05-22 17:11:08.802742 cattrs-23.1.0rc0/src/cattrs/preconf/tomlkit.py
+-rw-r--r--   0        0        0     1525 2023-05-22 17:11:08.806742 cattrs-23.1.0rc0/src/cattrs/preconf/ujson.py
+-rw-r--r--   0        0        0        0 2022-02-11 01:34:09.486876 cattrs-23.1.0rc0/src/cattrs/py.typed
+-rw-r--r--   0        0        0      192 2023-05-22 17:11:08.810742 cattrs-23.1.0rc0/src/cattrs/strategies/__init__.py
+-rw-r--r--   0        0        0     8677 2023-05-22 17:16:50.127698 cattrs-23.1.0rc0/src/cattrs/strategies/_subclasses.py
+-rw-r--r--   0        0        0     3440 2023-05-22 17:11:08.814742 cattrs-23.1.0rc0/src/cattrs/strategies/_unions.py
+-rw-r--r--   0        0        0     4360 2023-05-22 17:11:08.814742 cattrs-23.1.0rc0/src/cattrs/v.py
+-rw-r--r--   0        0        0     9253 1970-01-01 00:00:00.000000 cattrs-23.1.0rc0/PKG-INFO
```

### Comparing `cattrs-23.1.0/LICENSE` & `cattrs-23.1.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.0/README.md` & `cattrs-23.1.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.0/pyproject.toml` & `cattrs-23.1.0rc0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [tool.isort]
 profile = "black"
 known_first_party = ["cattr"]
 
 [tool.poetry]
 name = "cattrs"
-version = "23.1.0"
+version = "23.1.0rc0"
 description = "Composable complex class support for attrs and dataclasses."
 authors = ["Tin Tvrtkovic <tinchester@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/python-attrs/cattrs"
 documentation = "https://catt.rs/en/stable/"
 keywords = ["attrs", "serialization", "dataclasses"]
 packages = [
```

### Comparing `cattrs-23.1.0/src/cattr/__init__.py` & `cattrs-23.1.0rc0/src/cattr/__init__.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.0/src/cattr/gen.py` & `cattrs-23.1.0rc0/src/cattr/gen.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.0/src/cattrs/__init__.py` & `cattrs-23.1.0rc0/src/cattrs/__init__.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.0/src/cattrs/_compat.py` & `cattrs-23.1.0rc0/src/cattrs/_compat.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.0/src/cattrs/_generics.py` & `cattrs-23.1.0rc0/src/cattrs/_generics.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.0/src/cattrs/converters.py` & `cattrs-23.1.0rc0/src/cattrs/converters.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.0/src/cattrs/disambiguators.py` & `cattrs-23.1.0rc0/src/cattrs/disambiguators.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.0/src/cattrs/dispatch.py` & `cattrs-23.1.0rc0/src/cattrs/dispatch.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.0/src/cattrs/errors.py` & `cattrs-23.1.0rc0/src/cattrs/errors.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.0/src/cattrs/gen/__init__.py` & `cattrs-23.1.0rc0/src/cattrs/gen/__init__.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.0/src/cattrs/gen/_generics.py` & `cattrs-23.1.0rc0/src/cattrs/gen/_generics.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.0/src/cattrs/gen/_lc.py` & `cattrs-23.1.0rc0/src/cattrs/gen/_lc.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.0/src/cattrs/gen/_shared.py` & `cattrs-23.1.0rc0/src/cattrs/gen/_shared.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.0/src/cattrs/gen/typeddicts.py` & `cattrs-23.1.0rc0/src/cattrs/gen/typeddicts.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.0/src/cattrs/preconf/bson.py` & `cattrs-23.1.0rc0/src/cattrs/preconf/bson.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.0/src/cattrs/preconf/cbor2.py` & `cattrs-23.1.0rc0/src/cattrs/preconf/cbor2.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.0/src/cattrs/preconf/json.py` & `cattrs-23.1.0rc0/src/cattrs/preconf/json.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.0/src/cattrs/preconf/msgpack.py` & `cattrs-23.1.0rc0/src/cattrs/preconf/msgpack.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.0/src/cattrs/preconf/orjson.py` & `cattrs-23.1.0rc0/src/cattrs/preconf/orjson.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.0/src/cattrs/preconf/pyyaml.py` & `cattrs-23.1.0rc0/src/cattrs/preconf/pyyaml.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.0/src/cattrs/preconf/tomlkit.py` & `cattrs-23.1.0rc0/src/cattrs/preconf/tomlkit.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.0/src/cattrs/preconf/ujson.py` & `cattrs-23.1.0rc0/src/cattrs/preconf/ujson.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.0/src/cattrs/strategies/_subclasses.py` & `cattrs-23.1.0rc0/src/cattrs/strategies/_subclasses.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.0/src/cattrs/strategies/_unions.py` & `cattrs-23.1.0rc0/src/cattrs/strategies/_unions.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.0/src/cattrs/v.py` & `cattrs-23.1.0rc0/src/cattrs/v.py`

 * *Files identical despite different names*

### Comparing `cattrs-23.1.0/PKG-INFO` & `cattrs-23.1.0rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cattrs
-Version: 23.1.0
+Version: 23.1.0rc0
 Summary: Composable complex class support for attrs and dataclasses.
 Home-page: https://github.com/python-attrs/cattrs
 License: MIT
 Keywords: attrs,serialization,dataclasses
 Author: Tin Tvrtkovic
 Author-email: tinchester@gmail.com
 Requires-Python: >=3.7
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: cattrs Version: 23.1.0 Summary: Composable complex
-class support for attrs and dataclasses. Home-page: https://github.com/python-
-attrs/cattrs License: MIT Keywords: attrs,serialization,dataclasses Author: Tin
-Tvrtkovic Author-email: tinchester@gmail.com Requires-Python: >=3.7 Classifier:
-License :: OSI Approved :: MIT License Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Provides-Extra: bson Provides-Extra:
-cbor2 Provides-Extra: msgpack Provides-Extra: orjson Provides-Extra: pyyaml
-Provides-Extra: tomlkit Provides-Extra: ujson Requires-Dist: PyYAML
-(>=6.0,<7.0) ; extra == "pyyaml" Requires-Dist: attrs (>=20) Requires-Dist:
-cbor2 (>=5.4.6,<6.0.0) ; extra == "cbor2" Requires-Dist: exceptiongroup ;
+Metadata-Version: 2.1 Name: cattrs Version: 23.1.0rc0 Summary: Composable
+complex class support for attrs and dataclasses. Home-page: https://github.com/
+python-attrs/cattrs License: MIT Keywords: attrs,serialization,dataclasses
+Author: Tin Tvrtkovic Author-email: tinchester@gmail.com Requires-Python: >=3.7
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Provides-Extra: bson
+Provides-Extra: cbor2 Provides-Extra: msgpack Provides-Extra: orjson Provides-
+Extra: pyyaml Provides-Extra: tomlkit Provides-Extra: ujson Requires-Dist:
+PyYAML (>=6.0,<7.0) ; extra == "pyyaml" Requires-Dist: attrs (>=20) Requires-
+Dist: cbor2 (>=5.4.6,<6.0.0) ; extra == "cbor2" Requires-Dist: exceptiongroup ;
 python_version < "3.11" Requires-Dist: msgpack (>=1.0.2,<2.0.0) ; extra ==
 "msgpack" Requires-Dist: orjson (>=3.5.2,<4.0.0) ; (implementation_name ==
 "cpython") and (extra == "orjson") Requires-Dist: pymongo (>=4.2.0,<5.0.0) ;
 extra == "bson" Requires-Dist: tomlkit (>=0.11.4,<0.12.0) ; (python_version <
 "4") and (extra == "tomlkit") Requires-Dist: typing_extensions ; python_version
 < "3.10" Requires-Dist: ujson (>=5.4.0,<6.0.0) ; extra == "ujson" Project-URL:
 Bug Tracker, https://github.com/python-attrs/cattrs/issues Project-URL:
```

