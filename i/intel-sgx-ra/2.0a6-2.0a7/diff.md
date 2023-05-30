# Comparing `tmp/intel_sgx_ra-2.0a6.tar.gz` & `tmp/intel_sgx_ra-2.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intel_sgx_ra-2.0a6.tar", last modified: Tue May 30 12:56:03 2023, max compression
+gzip compressed data, was "intel_sgx_ra-2.0a7.tar", last modified: Tue May 30 14:00:44 2023, max compression
```

## Comparing `intel_sgx_ra-2.0a6.tar` & `intel_sgx_ra-2.0a7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:56:03.034104 intel_sgx_ra-2.0a6/
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-30 12:56:03.034104 intel_sgx_ra-2.0a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-30 12:56:03.034104 intel_sgx_ra-2.0a6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:56:03.030104 intel_sgx_ra-2.0a6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:56:03.030104 intel_sgx_ra-2.0a6/src/intel_sgx_ra/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10227 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra/attest.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra/base64url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:56:03.030104 intel_sgx_ra-2.0a6/src/intel_sgx_ra/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra/cli/verify.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra/error.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra/globs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra/pccs.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra/quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra/ratls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra/signer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:56:03.030104 intel_sgx_ra-2.0a6/src/intel_sgx_ra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-30 12:56:03.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-30 12:56:03.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:56:03.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-30 12:56:03.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:56:02.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-30 12:56:03.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 12:56:03.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:56:03.030104 intel_sgx_ra-2.0a6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/tests/test_pccs.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/tests/test_quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/tests/test_regex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:00:44.971521 intel_sgx_ra-2.0a7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-30 14:00:44.971521 intel_sgx_ra-2.0a7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-30 14:00:07.000000 intel_sgx_ra-2.0a7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-30 14:00:44.971521 intel_sgx_ra-2.0a7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-30 14:00:07.000000 intel_sgx_ra-2.0a7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:00:44.967522 intel_sgx_ra-2.0a7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:00:44.971521 intel_sgx_ra-2.0a7/src/intel_sgx_ra/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-30 14:00:07.000000 intel_sgx_ra-2.0a7/src/intel_sgx_ra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10227 2023-05-30 14:00:07.000000 intel_sgx_ra-2.0a7/src/intel_sgx_ra/attest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-30 14:00:07.000000 intel_sgx_ra-2.0a7/src/intel_sgx_ra/base64url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:00:44.971521 intel_sgx_ra-2.0a7/src/intel_sgx_ra/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-30 14:00:07.000000 intel_sgx_ra-2.0a7/src/intel_sgx_ra/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-30 14:00:07.000000 intel_sgx_ra-2.0a7/src/intel_sgx_ra/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-05-30 14:00:07.000000 intel_sgx_ra-2.0a7/src/intel_sgx_ra/cli/verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-30 14:00:07.000000 intel_sgx_ra-2.0a7/src/intel_sgx_ra/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-30 14:00:07.000000 intel_sgx_ra-2.0a7/src/intel_sgx_ra/globs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-05-30 14:00:07.000000 intel_sgx_ra-2.0a7/src/intel_sgx_ra/pccs.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:00:07.000000 intel_sgx_ra-2.0a7/src/intel_sgx_ra/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-05-30 14:00:07.000000 intel_sgx_ra-2.0a7/src/intel_sgx_ra/quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-05-30 14:00:07.000000 intel_sgx_ra-2.0a7/src/intel_sgx_ra/ratls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-30 14:00:07.000000 intel_sgx_ra-2.0a7/src/intel_sgx_ra/signer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:00:44.971521 intel_sgx_ra-2.0a7/src/intel_sgx_ra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-30 14:00:44.000000 intel_sgx_ra-2.0a7/src/intel_sgx_ra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-30 14:00:44.000000 intel_sgx_ra-2.0a7/src/intel_sgx_ra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:00:44.000000 intel_sgx_ra-2.0a7/src/intel_sgx_ra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-30 14:00:44.000000 intel_sgx_ra-2.0a7/src/intel_sgx_ra.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:00:44.000000 intel_sgx_ra-2.0a7/src/intel_sgx_ra.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-30 14:00:44.000000 intel_sgx_ra-2.0a7/src/intel_sgx_ra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 14:00:44.000000 intel_sgx_ra-2.0a7/src/intel_sgx_ra.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:00:44.971521 intel_sgx_ra-2.0a7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-30 14:00:07.000000 intel_sgx_ra-2.0a7/tests/test_pccs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-30 14:00:07.000000 intel_sgx_ra-2.0a7/tests/test_quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-30 14:00:07.000000 intel_sgx_ra-2.0a7/tests/test_regex.py
```

### Comparing `intel_sgx_ra-2.0a6/PKG-INFO` & `intel_sgx_ra-2.0a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intel_sgx_ra
-Version: 2.0a6
+Version: 2.0a7
 Summary: Intel SGX Remote Attestation verification library
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `intel_sgx_ra-2.0a6/README.md` & `intel_sgx_ra-2.0a7/README.md`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a6/setup.py` & `intel_sgx_ra-2.0a7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     package_dir={"": "src"},
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     zip_safe=False,
     install_requires=[
         "requests>=2.28.1,<3.0.0",
         "cryptography>=40.0.2,<40.1.0",
-        "sgx-pck-extension>=0.1.2,<0.2.0",
+        "sgx-pck-extension>=0.1.4,<0.2.0",
     ],
     entry_points={
         "console_scripts": [
             "sgx-ra-verify = intel_sgx_ra.cli.verify:run",
             "sgx-ra-utils = intel_sgx_ra.cli.utils:run",
         ],
     },
```

### Comparing `intel_sgx_ra-2.0a6/src/intel_sgx_ra/attest.py` & `intel_sgx_ra-2.0a7/src/intel_sgx_ra/attest.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a6/src/intel_sgx_ra/base64url.py` & `intel_sgx_ra-2.0a7/src/intel_sgx_ra/base64url.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a6/src/intel_sgx_ra/cli/utils.py` & `intel_sgx_ra-2.0a7/src/intel_sgx_ra/cli/utils.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a6/src/intel_sgx_ra/cli/verify.py` & `intel_sgx_ra-2.0a7/src/intel_sgx_ra/cli/verify.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a6/src/intel_sgx_ra/error.py` & `intel_sgx_ra-2.0a7/src/intel_sgx_ra/error.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a6/src/intel_sgx_ra/pccs.py` & `intel_sgx_ra-2.0a7/src/intel_sgx_ra/pccs.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a6/src/intel_sgx_ra/quote.py` & `intel_sgx_ra-2.0a7/src/intel_sgx_ra/quote.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a6/src/intel_sgx_ra/ratls.py` & `intel_sgx_ra-2.0a7/src/intel_sgx_ra/ratls.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a6/src/intel_sgx_ra/signer.py` & `intel_sgx_ra-2.0a7/src/intel_sgx_ra/signer.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a6/src/intel_sgx_ra.egg-info/PKG-INFO` & `intel_sgx_ra-2.0a7/src/intel_sgx_ra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intel-sgx-ra
-Version: 2.0a6
+Version: 2.0a7
 Summary: Intel SGX Remote Attestation verification library
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `intel_sgx_ra-2.0a6/src/intel_sgx_ra.egg-info/SOURCES.txt` & `intel_sgx_ra-2.0a7/src/intel_sgx_ra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a6/tests/test_pccs.py` & `intel_sgx_ra-2.0a7/tests/test_pccs.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a6/tests/test_quote.py` & `intel_sgx_ra-2.0a7/tests/test_quote.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a6/tests/test_regex.py` & `intel_sgx_ra-2.0a7/tests/test_regex.py`

 * *Files identical despite different names*

