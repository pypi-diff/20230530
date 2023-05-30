# Comparing `tmp/intel_sgx_ra-2.0a5.tar.gz` & `tmp/intel_sgx_ra-2.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intel_sgx_ra-2.0a5.tar", last modified: Thu May 25 16:15:41 2023, max compression
+gzip compressed data, was "intel_sgx_ra-2.0a6.tar", last modified: Tue May 30 12:56:03 2023, max compression
```

## Comparing `intel_sgx_ra-2.0a5.tar` & `intel_sgx_ra-2.0a6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:15:41.358536 intel_sgx_ra-2.0a5/
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-25 16:15:41.358536 intel_sgx_ra-2.0a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-25 16:15:41.358536 intel_sgx_ra-2.0a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:15:41.354536 intel_sgx_ra-2.0a5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:15:41.354536 intel_sgx_ra-2.0a5/src/intel_sgx_ra/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra/attest.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra/base64url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:15:41.358536 intel_sgx_ra-2.0a5/src/intel_sgx_ra/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra/cli/verify.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra/error.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra/globs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra/pccs.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra/quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra/ratls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra/signer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:15:41.354536 intel_sgx_ra-2.0a5/src/intel_sgx_ra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-25 16:15:41.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-25 16:15:41.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:15:41.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-25 16:15:41.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:15:41.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-25 16:15:41.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-25 16:15:41.000000 intel_sgx_ra-2.0a5/src/intel_sgx_ra.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:15:41.358536 intel_sgx_ra-2.0a5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/tests/test_pccs.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/tests/test_quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-25 16:14:56.000000 intel_sgx_ra-2.0a5/tests/test_regex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:56:03.034104 intel_sgx_ra-2.0a6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-30 12:56:03.034104 intel_sgx_ra-2.0a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-30 12:56:03.034104 intel_sgx_ra-2.0a6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:56:03.030104 intel_sgx_ra-2.0a6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:56:03.030104 intel_sgx_ra-2.0a6/src/intel_sgx_ra/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10227 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra/attest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra/base64url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:56:03.030104 intel_sgx_ra-2.0a6/src/intel_sgx_ra/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra/cli/verify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra/globs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra/pccs.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9273 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra/quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra/ratls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra/signer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:56:03.030104 intel_sgx_ra-2.0a6/src/intel_sgx_ra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-30 12:56:03.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-30 12:56:03.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:56:03.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-30 12:56:03.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:56:02.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-30 12:56:03.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 12:56:03.000000 intel_sgx_ra-2.0a6/src/intel_sgx_ra.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:56:03.030104 intel_sgx_ra-2.0a6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/tests/test_pccs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/tests/test_quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-05-30 12:55:20.000000 intel_sgx_ra-2.0a6/tests/test_regex.py
```

### Comparing `intel_sgx_ra-2.0a5/PKG-INFO` & `intel_sgx_ra-2.0a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intel_sgx_ra
-Version: 2.0a5
+Version: 2.0a6
 Summary: Intel SGX Remote Attestation verification library
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `intel_sgx_ra-2.0a5/README.md` & `intel_sgx_ra-2.0a6/README.md`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a5/setup.py` & `intel_sgx_ra-2.0a6/setup.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a5/src/intel_sgx_ra/attest.py` & `intel_sgx_ra-2.0a6/src/intel_sgx_ra/attest.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,22 +143,42 @@
 
     logging.info("%s TCB verification", globs.OK)
 
     return True
 
 
 def retrieve_collaterals(
-    fmspc: bytes, pccs_url: str, ca: Literal["processor", "platform"]
+    quote: Quote,
+    pccs_url: str,
 ) -> Tuple[
     bytes,
     x509.Certificate,
     x509.CertificateRevocationList,
     x509.CertificateRevocationList,
 ]:
     """Retrive collaterals from PCCS URL and PCK CA type."""
+    pck_cert, pck_ca_cert, _root_ca_cert = [
+        x509.load_pem_x509_certificate(raw_cert) for raw_cert in quote.certs()
+    ]  # type: x509.Certificate, x509.Certificate, x509.Certificate
+
+    sgx_pck_ext: Dict[str, Any] = sgx_pck_extension_from_cert(pck_cert)
+    fmspc: bytes = sgx_pck_ext["fmspc"]
+
+    common_name: x509.NameAttribute
+    common_name, *_ = pck_ca_cert.subject.get_attributes_for_oid(
+        x509.NameOID.COMMON_NAME
+    )
+    ca: Literal["processor", "platform"]
+    if common_name.value == "Intel SGX PCK Platform CA":
+        ca = "platform"
+    elif common_name.value == "Intel SGX PCK Processor CA":
+        ca = "processor"
+    else:
+        raise CertificateError("Unknown CN in Intel SGX PCK Platform/Processor CA")
+
     root_ca_crl: x509.CertificateRevocationList = get_root_ca_crl(pccs_url)
     pck_ca_crl: x509.CertificateRevocationList = get_pck_cert_crl(pccs_url, ca)
     tcb_info, tcb_cert = get_tcbinfo(pccs_url, fmspc)
 
     return tcb_info, tcb_cert, root_ca_crl, pck_ca_crl
 
 
@@ -185,35 +205,22 @@
     if debug:
         raise SGXDebugModeError
 
     pck_cert, pck_ca_cert, root_ca_cert = [
         x509.load_pem_x509_certificate(raw_cert) for raw_cert in quote.certs()
     ]  # type: x509.Certificate, x509.Certificate, x509.Certificate
 
-    sgx_pck_ext: Dict[str, Any] = sgx_pck_extension_from_cert(pck_cert)
-    fmspc: bytes = sgx_pck_ext["fmspc"]
-
     tcb_info: bytes
     tcb_cert: x509.Certificate
     root_ca_crl: x509.CertificateRevocationList
     pck_ca_crl: x509.CertificateRevocationList
     if pccs_url is not None:
-        common_name, *_ = pck_ca_cert.subject.get_attributes_for_oid(
-            x509.NameOID.COMMON_NAME
+        tcb_info, tcb_cert, root_ca_crl, pck_ca_crl = retrieve_collaterals(
+            quote, pccs_url
         )
-        if common_name.value == "Intel SGX PCK Platform CA":
-            (tcb_info, tcb_cert, root_ca_crl, pck_ca_crl) = retrieve_collaterals(
-                fmspc, pccs_url, "platform"
-            )
-        elif common_name.value == "Intel SGX PCK Processor CA":
-            (tcb_info, tcb_cert, root_ca_crl, pck_ca_crl) = retrieve_collaterals(
-                fmspc, pccs_url, "processor"
-            )
-        else:
-            raise CertificateError("Unknown CN in Intel SGX PCK Platform/Processor CA")
     elif collaterals is not None:
         tcb_info, tcb_cert, root_ca_crl, pck_ca_crl = collaterals
     else:
         raise CollateralsError("Collaterals or PCCS URL missing")
 
     assert verify_pck_chain(
         root_ca_cert, pck_ca_cert, pck_cert, root_ca_crl, pck_ca_crl
```

### Comparing `intel_sgx_ra-2.0a5/src/intel_sgx_ra/base64url.py` & `intel_sgx_ra-2.0a6/src/intel_sgx_ra/base64url.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a5/src/intel_sgx_ra/cli/utils.py` & `intel_sgx_ra-2.0a6/src/intel_sgx_ra/cli/utils.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a5/src/intel_sgx_ra/cli/verify.py` & `intel_sgx_ra-2.0a6/src/intel_sgx_ra/cli/verify.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a5/src/intel_sgx_ra/error.py` & `intel_sgx_ra-2.0a6/src/intel_sgx_ra/error.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a5/src/intel_sgx_ra/pccs.py` & `intel_sgx_ra-2.0a6/src/intel_sgx_ra/pccs.py`

 * *Files 12% similar despite different names*

```diff
@@ -110,28 +110,7 @@
     ]
     if others:
         raise PCCSResponseError(
             "More than 2 certifices in header SGX-Enclave-Identity-Issuer-Chain"
         )
 
     return (tcb_cert, root_ca_cert), response.json()
-
-
-def get_qve_identity(
-    pccs_url: str,
-) -> Tuple[Tuple[Certificate, Certificate], Dict[str, Any]]:
-    """Retrieve Quoting Verification Enclave Identity."""
-    response = requests.get(
-        url=f"{pccs_url}/sgx/certification/v4/qve/identity", timeout=30
-    )
-
-    cert_chain = unquote(response.headers["SGX-Enclave-Identity-Issuer-Chain"])
-    tcb_cert, root_ca_cert, *others = [
-        load_pem_x509_certificate(raw_cert)
-        for raw_cert in re.findall(RE_CERT, cert_chain.encode("utf-8"))
-    ]
-    if others:
-        raise PCCSResponseError(
-            "More than 2 certifices in header SGX-Enclave-Identity-Issuer-Chain"
-        )
-
-    return (tcb_cert, root_ca_cert), response.json()
```

### Comparing `intel_sgx_ra-2.0a5/src/intel_sgx_ra/quote.py` & `intel_sgx_ra-2.0a6/src/intel_sgx_ra/quote.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a5/src/intel_sgx_ra/ratls.py` & `intel_sgx_ra-2.0a6/src/intel_sgx_ra/ratls.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a5/src/intel_sgx_ra/signer.py` & `intel_sgx_ra-2.0a6/src/intel_sgx_ra/signer.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a5/src/intel_sgx_ra.egg-info/PKG-INFO` & `intel_sgx_ra-2.0a6/src/intel_sgx_ra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intel-sgx-ra
-Version: 2.0a5
+Version: 2.0a6
 Summary: Intel SGX Remote Attestation verification library
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `intel_sgx_ra-2.0a5/src/intel_sgx_ra.egg-info/SOURCES.txt` & `intel_sgx_ra-2.0a6/src/intel_sgx_ra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a5/tests/test_pccs.py` & `intel_sgx_ra-2.0a6/tests/test_pccs.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a5/tests/test_quote.py` & `intel_sgx_ra-2.0a6/tests/test_quote.py`

 * *Files identical despite different names*

### Comparing `intel_sgx_ra-2.0a5/tests/test_regex.py` & `intel_sgx_ra-2.0a6/tests/test_regex.py`

 * *Files identical despite different names*

