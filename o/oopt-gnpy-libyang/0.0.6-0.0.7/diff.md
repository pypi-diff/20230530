# Comparing `tmp/oopt-gnpy-libyang-0.0.6.tar.gz` & `tmp/oopt-gnpy-libyang-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oopt-gnpy-libyang-0.0.6.tar", last modified: Wed May 10 09:54:35 2023, max compression
+gzip compressed data, was "oopt-gnpy-libyang-0.0.7.tar", last modified: Tue May 30 13:38:50 2023, max compression
```

## Comparing `oopt-gnpy-libyang-0.0.6.tar` & `oopt-gnpy-libyang-0.0.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:54:35.084817 oopt-gnpy-libyang-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:54:35.080817 oopt-gnpy-libyang-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:54:35.084817 oopt-gnpy-libyang-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)    21383 2023-05-10 09:52:25.000000 oopt-gnpy-libyang-0.0.6/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-10 09:52:25.000000 oopt-gnpy-libyang-0.0.6/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-05-10 09:52:25.000000 oopt-gnpy-libyang-0.0.6/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-10 09:52:25.000000 oopt-gnpy-libyang-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-10 09:52:25.000000 oopt-gnpy-libyang-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-05-10 09:54:35.084817 oopt-gnpy-libyang-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-05-10 09:52:25.000000 oopt-gnpy-libyang-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    10676 2023-05-10 09:52:25.000000 oopt-gnpy-libyang-0.0.6/oopt-gnpy-libyang.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:54:35.084817 oopt-gnpy-libyang-0.0.6/oopt_gnpy_libyang.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-05-10 09:54:35.000000 oopt-gnpy-libyang-0.0.6/oopt_gnpy_libyang.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-10 09:54:35.000000 oopt-gnpy-libyang-0.0.6/oopt_gnpy_libyang.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 09:54:35.000000 oopt-gnpy-libyang-0.0.6/oopt_gnpy_libyang.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 09:54:34.000000 oopt-gnpy-libyang-0.0.6/oopt_gnpy_libyang.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-10 09:54:35.000000 oopt-gnpy-libyang-0.0.6/oopt_gnpy_libyang.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-10 09:54:35.000000 oopt-gnpy-libyang-0.0.6/oopt_gnpy_libyang.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-10 09:52:25.000000 oopt-gnpy-libyang-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 09:54:35.084817 oopt-gnpy-libyang-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-05-10 09:52:25.000000 oopt-gnpy-libyang-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:54:35.084817 oopt-gnpy-libyang-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-10 09:52:25.000000 oopt-gnpy-libyang-0.0.6/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-10 09:52:25.000000 oopt-gnpy-libyang-0.0.6/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7795 2023-05-10 09:52:25.000000 oopt-gnpy-libyang-0.0.6/tests/test_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 09:54:35.084817 oopt-gnpy-libyang-0.0.6/tests/yang/
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-10 09:52:25.000000 oopt-gnpy-libyang-0.0.6/tests/yang/iana-hardware@2018-03-13.yang
--rw-r--r--   0 runner    (1001) docker     (123)    37062 2023-05-10 09:52:25.000000 oopt-gnpy-libyang-0.0.6/tests/yang/iana-if-type@2017-01-19.yang
--rw-r--r--   0 runner    (1001) docker     (123)    37325 2023-05-10 09:52:25.000000 oopt-gnpy-libyang-0.0.6/tests/yang/ietf-hardware@2018-03-13.yang
--rw-r--r--   0 runner    (1001) docker     (123)    39365 2023-05-10 09:52:25.000000 oopt-gnpy-libyang-0.0.6/tests/yang/ietf-interfaces@2018-02-20.yang
--rw-r--r--   0 runner    (1001) docker     (123)    27507 2023-05-10 09:52:25.000000 oopt-gnpy-libyang-0.0.6/tests/yang/ietf-ip@2018-02-22.yang
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:38:50.677619 oopt-gnpy-libyang-0.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:38:50.673618 oopt-gnpy-libyang-0.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:38:50.677619 oopt-gnpy-libyang-0.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)    21383 2023-05-30 13:37:10.000000 oopt-gnpy-libyang-0.0.7/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-30 13:37:10.000000 oopt-gnpy-libyang-0.0.7/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)     5816 2023-05-30 13:37:10.000000 oopt-gnpy-libyang-0.0.7/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-30 13:37:10.000000 oopt-gnpy-libyang-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-30 13:37:10.000000 oopt-gnpy-libyang-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-05-30 13:38:50.677619 oopt-gnpy-libyang-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-05-30 13:37:10.000000 oopt-gnpy-libyang-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10307 2023-05-30 13:37:10.000000 oopt-gnpy-libyang-0.0.7/oopt-gnpy-libyang.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:38:50.677619 oopt-gnpy-libyang-0.0.7/oopt_gnpy_libyang.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-05-30 13:38:50.000000 oopt-gnpy-libyang-0.0.7/oopt_gnpy_libyang.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-30 13:38:50.000000 oopt-gnpy-libyang-0.0.7/oopt_gnpy_libyang.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:38:50.000000 oopt-gnpy-libyang-0.0.7/oopt_gnpy_libyang.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:38:50.000000 oopt-gnpy-libyang-0.0.7/oopt_gnpy_libyang.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 13:38:50.000000 oopt-gnpy-libyang-0.0.7/oopt_gnpy_libyang.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-30 13:38:50.000000 oopt-gnpy-libyang-0.0.7/oopt_gnpy_libyang.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-30 13:37:10.000000 oopt-gnpy-libyang-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 13:38:50.677619 oopt-gnpy-libyang-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-05-30 13:37:10.000000 oopt-gnpy-libyang-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:38:50.677619 oopt-gnpy-libyang-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-30 13:37:10.000000 oopt-gnpy-libyang-0.0.7/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-30 13:37:10.000000 oopt-gnpy-libyang-0.0.7/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7791 2023-05-30 13:37:10.000000 oopt-gnpy-libyang-0.0.7/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:38:50.677619 oopt-gnpy-libyang-0.0.7/tests/yang/
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-30 13:37:10.000000 oopt-gnpy-libyang-0.0.7/tests/yang/iana-hardware@2018-03-13.yang
+-rw-r--r--   0 runner    (1001) docker     (123)    37062 2023-05-30 13:37:10.000000 oopt-gnpy-libyang-0.0.7/tests/yang/iana-if-type@2017-01-19.yang
+-rw-r--r--   0 runner    (1001) docker     (123)    37325 2023-05-30 13:37:10.000000 oopt-gnpy-libyang-0.0.7/tests/yang/ietf-hardware@2018-03-13.yang
+-rw-r--r--   0 runner    (1001) docker     (123)    39365 2023-05-30 13:37:10.000000 oopt-gnpy-libyang-0.0.7/tests/yang/ietf-interfaces@2018-02-20.yang
+-rw-r--r--   0 runner    (1001) docker     (123)    27507 2023-05-30 13:37:10.000000 oopt-gnpy-libyang-0.0.7/tests/yang/ietf-ip@2018-02-22.yang
```

### Comparing `oopt-gnpy-libyang-0.0.6/.github/workflows/ci.yaml` & `oopt-gnpy-libyang-0.0.7/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.6/CMakeLists.txt` & `oopt-gnpy-libyang-0.0.7/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 if(NOT MSVC)
     set(CMAKE_CXX_FLAGS_DEBUG "-Werror ${CMAKE_CXX_FLAGS_DEBUG}")
     set(CMAKE_CXX_FLAGS "-Wall -Wextra -pedantic -Woverloaded-virtual -Wimplicit-fallthrough -Wsuggest-override ${CMAKE_CXX_FLAGS}")
 endif()
 
 find_package(PkgConfig)
-pkg_check_modules(LIBYANG-CPP REQUIRED IMPORTED_TARGET libyang-cpp>=1.0.0)
+pkg_check_modules(LIBYANG-CPP REQUIRED IMPORTED_TARGET libyang-cpp>=1.0.0 libyang)
 
 set(PYBIND11_FINDPYTHON ON)
 find_package(Python 3.8 REQUIRED COMPONENTS Interpreter Development.Module)
 find_package(pybind11 2.9.1 REQUIRED CONFIG)
 message(STATUS "Using Python ${Python_VERSION}")
 
 pybind11_add_module(oopt_gnpy_libyang ${CMAKE_CURRENT_SOURCE_DIR}/oopt-gnpy-libyang.cpp)
```

### Comparing `oopt-gnpy-libyang-0.0.6/LICENSE` & `oopt-gnpy-libyang-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.6/PKG-INFO` & `oopt-gnpy-libyang-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oopt-gnpy-libyang
-Version: 0.0.6
+Version: 0.0.7
 Summary: Opinionated Python bindings for the libyang library
 Home-page: https://github.com/Telecominfraproject/oopt-gnpy-libyang
 Download-URL: https://pypi.org/project/oopt-gnpy-libyang/
 Author: Telecom Infra Project
 Author-email: jan.kundrat@telecominfraproject.com
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
@@ -77,15 +77,15 @@
         "name": "eth0",
         "type": "iana-if-type:ethernetCsmacd"
       }
     ]
   }
 }'''
 
-data = c.parse_data_str(blob,
+data = c.parse_data(blob,
     ly.DataFormat.JSON, ly.ParseOptions.Strict | ly.ParseOptions.Ordered,
     ly.ValidationOptions.Present | ly.ValidationOptions.NoState)
 ```
 ### Working with data
 
 Libyang works with forests (sets of trees), this is how to process all the data:
 ```python
@@ -118,15 +118,15 @@
 In libyang, if an operation fails, error details are available via `context.errors()`:
 ```python
 import json
 wrong = json.loads(blob)
 wrong["ietf-interfaces:interfaces"]["interface"][0]\
     ["ietf-ip:ipv6"]["address"][0]["prefix-length"] = 666
 try:
-    data = c.parse_data_str(json.dumps(wrong),
+    data = c.parse_data(json.dumps(wrong),
         ly.DataFormat.JSON, ly.ParseOptions.Strict | ly.ParseOptions.Ordered,
         ly.ValidationOptions.Present | ly.ValidationOptions.NoState)
     assert False
 except ly.Error:
     for error in c.errors():
         assert error.path == "Schema location \"/ietf-interfaces:interfaces/interface/ietf-ip:ipv6/address/prefix-length\", data location \"/ietf-ip:address[ip='::1']\", line number 1."
         assert error.message == 'Value "666" is out of type uint8 min/max bounds.'
```

### Comparing `oopt-gnpy-libyang-0.0.6/README.md` & `oopt-gnpy-libyang-0.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         "name": "eth0",
         "type": "iana-if-type:ethernetCsmacd"
       }
     ]
   }
 }'''
 
-data = c.parse_data_str(blob,
+data = c.parse_data(blob,
     ly.DataFormat.JSON, ly.ParseOptions.Strict | ly.ParseOptions.Ordered,
     ly.ValidationOptions.Present | ly.ValidationOptions.NoState)
 ```
 ### Working with data
 
 Libyang works with forests (sets of trees), this is how to process all the data:
 ```python
@@ -92,15 +92,15 @@
 In libyang, if an operation fails, error details are available via `context.errors()`:
 ```python
 import json
 wrong = json.loads(blob)
 wrong["ietf-interfaces:interfaces"]["interface"][0]\
     ["ietf-ip:ipv6"]["address"][0]["prefix-length"] = 666
 try:
-    data = c.parse_data_str(json.dumps(wrong),
+    data = c.parse_data(json.dumps(wrong),
         ly.DataFormat.JSON, ly.ParseOptions.Strict | ly.ParseOptions.Ordered,
         ly.ValidationOptions.Present | ly.ValidationOptions.NoState)
     assert False
 except ly.Error:
     for error in c.errors():
         assert error.path == "Schema location \"/ietf-interfaces:interfaces/interface/ietf-ip:ipv6/address/prefix-length\", data location \"/ietf-ip:address[ip='::1']\", line number 1."
         assert error.message == 'Value "666" is out of type uint8 min/max bounds.'
```

### Comparing `oopt-gnpy-libyang-0.0.6/oopt_gnpy_libyang.egg-info/PKG-INFO` & `oopt-gnpy-libyang-0.0.7/oopt_gnpy_libyang.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oopt-gnpy-libyang
-Version: 0.0.6
+Version: 0.0.7
 Summary: Opinionated Python bindings for the libyang library
 Home-page: https://github.com/Telecominfraproject/oopt-gnpy-libyang
 Download-URL: https://pypi.org/project/oopt-gnpy-libyang/
 Author: Telecom Infra Project
 Author-email: jan.kundrat@telecominfraproject.com
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
@@ -77,15 +77,15 @@
         "name": "eth0",
         "type": "iana-if-type:ethernetCsmacd"
       }
     ]
   }
 }'''
 
-data = c.parse_data_str(blob,
+data = c.parse_data(blob,
     ly.DataFormat.JSON, ly.ParseOptions.Strict | ly.ParseOptions.Ordered,
     ly.ValidationOptions.Present | ly.ValidationOptions.NoState)
 ```
 ### Working with data
 
 Libyang works with forests (sets of trees), this is how to process all the data:
 ```python
@@ -118,15 +118,15 @@
 In libyang, if an operation fails, error details are available via `context.errors()`:
 ```python
 import json
 wrong = json.loads(blob)
 wrong["ietf-interfaces:interfaces"]["interface"][0]\
     ["ietf-ip:ipv6"]["address"][0]["prefix-length"] = 666
 try:
-    data = c.parse_data_str(json.dumps(wrong),
+    data = c.parse_data(json.dumps(wrong),
         ly.DataFormat.JSON, ly.ParseOptions.Strict | ly.ParseOptions.Ordered,
         ly.ValidationOptions.Present | ly.ValidationOptions.NoState)
     assert False
 except ly.Error:
     for error in c.errors():
         assert error.path == "Schema location \"/ietf-interfaces:interfaces/interface/ietf-ip:ipv6/address/prefix-length\", data location \"/ietf-ip:address[ip='::1']\", line number 1."
         assert error.message == 'Value "666" is out of type uint8 min/max bounds.'
```

### Comparing `oopt-gnpy-libyang-0.0.6/oopt_gnpy_libyang.egg-info/SOURCES.txt` & `oopt-gnpy-libyang-0.0.7/oopt_gnpy_libyang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.6/pyproject.toml` & `oopt-gnpy-libyang-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.6/setup.py` & `oopt-gnpy-libyang-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.6/tests/conftest.py` & `oopt-gnpy-libyang-0.0.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.6/tests/test_context.py` & `oopt-gnpy-libyang-0.0.7/tests/test_context.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import pytest
 import oopt_gnpy_libyang as ly
+from pathlib import Path
 
 def test_no_module(context_no_libyang):
     with pytest.raises(ly.Error, match="Can't load module 'yay'"):
         context_no_libyang.load_module('yay')
 
 def test_empty():
     c = ly.Context()
@@ -25,7 +26,21 @@
         assert m.feature_enabled(feature.name) == (feature.name == 'arbitrary-names')
     m.set_implemented_all_features()
     for feature in m.features:
         assert m.feature_enabled(feature.name)
 
 def test_no_shared_errors(context_no_libyang):
     assert context_no_libyang.errors() == []
+
+def test_explicit_loading(context_no_libyang):
+    TEST_ROOT = Path(__file__).parent
+    with pytest.raises(ly.Error, match="Can't parse module: LY_ESYS"):
+        context_no_libyang.parse_module(TEST_ROOT / 'no-such-path.yang', ly.SchemaFormat.YANG)
+    m1 = context_no_libyang.parse_module(TEST_ROOT / 'yang' / 'iana-if-type@2017-01-19.yang', ly.SchemaFormat.YANG)
+    assert m1.name == 'iana-if-type'
+    m2 = context_no_libyang.parse_module((TEST_ROOT / 'yang' / 'iana-hardware@2018-03-13.yang').read_text(), ly.SchemaFormat.YANG)
+    assert m2.name == 'iana-hardware'
+
+def test_version():
+    assert len(ly.libyang_version_info()) == 3
+    assert ly.libyang_version_info()[0] == 2
+    assert ly.libyang_version()[0:2] == '2.'
```

### Comparing `oopt-gnpy-libyang-0.0.6/tests/test_validation.py` & `oopt-gnpy-libyang-0.0.7/tests/test_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
       }
     ]
   },
   "ietf-hardware:hardware": {
   }
 }
     '''
-    data = context_with_modules.parse_data_str(blob, ly.DataFormat.JSON, ly.ParseOptions.Strict | ly.ParseOptions.Ordered, ly.ValidationOptions.Present | ly.ValidationOptions.NoState)
+    data = context_with_modules.parse_data(blob, ly.DataFormat.JSON, ly.ParseOptions.Strict | ly.ParseOptions.Ordered, ly.ValidationOptions.Present | ly.ValidationOptions.NoState)
     assert data.path == '/ietf-interfaces:interfaces'
 
     assert [x.path for x in data.siblings()] == ['/ietf-interfaces:interfaces', '/ietf-hardware:hardware']
     assert [inner.path for top in data.siblings() for inner in top.childrenDfs()] == [
         '/ietf-interfaces:interfaces',
         "/ietf-interfaces:interfaces/interface[name='lo']",
         "/ietf-interfaces:interfaces/interface[name='lo']/name",
```

### Comparing `oopt-gnpy-libyang-0.0.6/tests/yang/iana-hardware@2018-03-13.yang` & `oopt-gnpy-libyang-0.0.7/tests/yang/iana-hardware@2018-03-13.yang`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.6/tests/yang/iana-if-type@2017-01-19.yang` & `oopt-gnpy-libyang-0.0.7/tests/yang/iana-if-type@2017-01-19.yang`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.6/tests/yang/ietf-hardware@2018-03-13.yang` & `oopt-gnpy-libyang-0.0.7/tests/yang/ietf-hardware@2018-03-13.yang`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.6/tests/yang/ietf-interfaces@2018-02-20.yang` & `oopt-gnpy-libyang-0.0.7/tests/yang/ietf-interfaces@2018-02-20.yang`

 * *Files identical despite different names*

### Comparing `oopt-gnpy-libyang-0.0.6/tests/yang/ietf-ip@2018-02-22.yang` & `oopt-gnpy-libyang-0.0.7/tests/yang/ietf-ip@2018-02-22.yang`

 * *Files identical despite different names*

