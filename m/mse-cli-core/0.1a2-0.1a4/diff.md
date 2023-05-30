# Comparing `tmp/mse_cli_core-0.1a2.tar.gz` & `tmp/mse_cli_core-0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mse_cli_core-0.1a2.tar", last modified: Thu May 25 09:45:38 2023, max compression
+gzip compressed data, was "mse_cli_core-0.1a4.tar", last modified: Tue May 30 14:34:50 2023, max compression
```

## Comparing `mse_cli_core-0.1a2.tar` & `mse_cli_core-0.1a4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:45:38.795952 mse_cli_core-0.1a2/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-25 09:45:38.795952 mse_cli_core-0.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-25 09:44:58.000000 mse_cli_core-0.1a2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-25 09:45:38.795952 mse_cli_core-0.1a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-25 09:44:58.000000 mse_cli_core-0.1a2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:45:38.787952 mse_cli_core-0.1a2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:45:38.791952 mse_cli_core-0.1a2/src/mse_cli_core/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-25 09:44:58.000000 mse_cli_core-0.1a2/src/mse_cli_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-25 09:44:58.000000 mse_cli_core-0.1a2/src/mse_cli_core/base64.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-05-25 09:44:58.000000 mse_cli_core-0.1a2/src/mse_cli_core/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-25 09:44:58.000000 mse_cli_core-0.1a2/src/mse_cli_core/clock_tick.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-25 09:44:58.000000 mse_cli_core-0.1a2/src/mse_cli_core/enclave.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-25 09:44:58.000000 mse_cli_core-0.1a2/src/mse_cli_core/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-25 09:44:58.000000 mse_cli_core-0.1a2/src/mse_cli_core/ignore_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-25 09:44:58.000000 mse_cli_core-0.1a2/src/mse_cli_core/no_sgx_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-25 09:44:58.000000 mse_cli_core-0.1a2/src/mse_cli_core/sgx_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-25 09:44:58.000000 mse_cli_core-0.1a2/src/mse_cli_core/test_docker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:45:38.791952 mse_cli_core-0.1a2/src/mse_cli_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-25 09:45:38.000000 mse_cli_core-0.1a2/src/mse_cli_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-25 09:45:38.000000 mse_cli_core-0.1a2/src/mse_cli_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:45:38.000000 mse_cli_core-0.1a2/src/mse_cli_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-25 09:45:38.000000 mse_cli_core-0.1a2/src/mse_cli_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-25 09:45:38.000000 mse_cli_core-0.1a2/src/mse_cli_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:45:38.000000 mse_cli_core-0.1a2/src/mse_cli_core.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:45:38.795952 mse_cli_core-0.1a2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-25 09:44:58.000000 mse_cli_core-0.1a2/tests/test_base64.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-25 09:44:58.000000 mse_cli_core-0.1a2/tests/test_boostrap.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-25 09:44:58.000000 mse_cli_core-0.1a2/tests/test_ignore_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-25 09:44:58.000000 mse_cli_core-0.1a2/tests/test_no_sgx_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-05-25 09:44:58.000000 mse_cli_core-0.1a2/tests/test_sgx_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-25 09:44:58.000000 mse_cli_core-0.1a2/tests/test_test_docker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:34:50.835401 mse_cli_core-0.1a4/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-30 14:34:50.835401 mse_cli_core-0.1a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-30 14:34:50.835401 mse_cli_core-0.1a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:34:50.831401 mse_cli_core-0.1a4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:34:50.835401 mse_cli_core-0.1a4/src/mse_cli_core/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/src/mse_cli_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/src/mse_cli_core/base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/src/mse_cli_core/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/src/mse_cli_core/clock_tick.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/src/mse_cli_core/enclave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/src/mse_cli_core/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/src/mse_cli_core/ignore_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/src/mse_cli_core/no_sgx_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/src/mse_cli_core/sgx_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/src/mse_cli_core/test_docker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:34:50.835401 mse_cli_core-0.1a4/src/mse_cli_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-30 14:34:50.000000 mse_cli_core-0.1a4/src/mse_cli_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-30 14:34:50.000000 mse_cli_core-0.1a4/src/mse_cli_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:34:50.000000 mse_cli_core-0.1a4/src/mse_cli_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-30 14:34:50.000000 mse_cli_core-0.1a4/src/mse_cli_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 14:34:50.000000 mse_cli_core-0.1a4/src/mse_cli_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:34:50.000000 mse_cli_core-0.1a4/src/mse_cli_core.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:34:50.835401 mse_cli_core-0.1a4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/tests/test_base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/tests/test_boostrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/tests/test_ignore_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/tests/test_no_sgx_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/tests/test_sgx_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-30 14:34:17.000000 mse_cli_core-0.1a4/tests/test_test_docker.py
```

### Comparing `mse_cli_core-0.1a2/PKG-INFO` & `mse_cli_core-0.1a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mse_cli_core
-Version: 0.1a2
+Version: 0.1a4
 Summary: Utils for MicroService Encryption Python CLIs
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Project-URL: Documentation, https://docs.cosmian.com
 Project-URL: Source, https://github.com/Cosmian/mse-cli-core
```

### Comparing `mse_cli_core-0.1a2/setup.cfg` & `mse_cli_core-0.1a4/setup.cfg`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a2/setup.py` & `mse_cli_core-0.1a4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     description="Utils for MicroService Encryption Python CLIs",
     packages=find_packages("src"),
     package_dir={"": "src"},
     zip_safe=True,
     install_requires=[
         "cryptography>=40.0.2,<41.0",
         "docker>=6.0.1,<7.0.0",
-        "intel-sgx-ra==2.0a4",
+        "intel-sgx-ra==2.0a7",
         "pydantic>=1.10.2,<2.0.0",
         "requests>=2.28.1,<2.29.0",
         "toml>=0.10.2,<0.11.0",
     ],
     setup_requires=["wheel"],
     tests_require=["pytest>=7.2.0,<7.3.0"],
     classifiers=[
```

### Comparing `mse_cli_core-0.1a2/src/mse_cli_core/base64.py` & `mse_cli_core-0.1a4/src/mse_cli_core/base64.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a2/src/mse_cli_core/bootstrap.py` & `mse_cli_core-0.1a4/src/mse_cli_core/bootstrap.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 class ConfigurationPayload(BaseModel):
     """Definition of the bootstrap server payload."""
 
     app_id: UUID
     secrets: Optional[Any]
     sealed_secrets: Optional[bytes]
     code_secret_key: Optional[bytes]
+    ssl_private_key: Optional[str]
 
     def payload(self) -> Dict[str, Any]:
         """Build the payload to send to the configuration server."""
         data: Dict[str, Any] = {
             "uuid": str(self.app_id),
         }
 
@@ -29,14 +30,17 @@
 
         if self.sealed_secrets:
             data["app_sealed_secrets"] = base64url_encode(self.sealed_secrets)
 
         if self.code_secret_key:
             data["code_secret_key"] = self.code_secret_key.hex()
 
+        if self.ssl_private_key:
+            data["ssl_private_key"] = self.ssl_private_key
+
         return data
 
 
 def configure_app(url: str, data: Dict[str, Any], verify: Union[bool, str] = True):
     """Send the secrets to the configuration server."""
     r = requests.post(
         url=url,
```

### Comparing `mse_cli_core-0.1a2/src/mse_cli_core/clock_tick.py` & `mse_cli_core-0.1a4/src/mse_cli_core/clock_tick.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a2/src/mse_cli_core/enclave.py` & `mse_cli_core-0.1a4/src/mse_cli_core/enclave.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """mse_cli_core.enclave module."""
 
 import re
 from pathlib import Path
-from typing import Optional, Tuple
+from typing import Optional, Tuple, Union
 
 from cryptography.hazmat.primitives.asymmetric.rsa import RSAPublicKey
 from cryptography.x509 import Certificate, CertificateRevocationList
 from docker.client import DockerClient
 from intel_sgx_ra.attest import verify_quote
 from intel_sgx_ra.ratls import ratls_verify
 from intel_sgx_ra.signer import mr_signer_from_pk
@@ -53,19 +53,19 @@
             f"Fail to compute mr_enclave! See {docker_path_log} for more details."
         )
 
     return str(m.group(1).decode("utf-8"))
 
 
 def verify_enclave(
-    signer_pk: RSAPublicKey,
-    ratls_certificate: Certificate,
-    fingerprint: str,
+    signer_pk: Union[RSAPublicKey, Path, bytes],
+    ratls_certificate: Union[str, bytes, Path, Certificate],
+    fingerprint: Optional[str],
     collaterals: Optional[
-        Tuple[CertificateRevocationList, CertificateRevocationList]
+        Tuple[bytes, Certificate, CertificateRevocationList, CertificateRevocationList]
     ] = None,
     pccs_url: Optional[str] = None,
 ):
     """Verify an enclave trustworthiness."""
     # Compute MRSIGNER value from public key
     mrsigner = mr_signer_from_pk(signer_pk)
 
@@ -80,13 +80,14 @@
             f"but should be {bytes(mrsigner).hex()})"
         )
 
     # Check enclave certificates and information
     verify_quote(quote=quote, collaterals=collaterals, pccs_url=pccs_url)
 
     # Check MRENCLAVE
-    if quote.report_body.mr_enclave != bytes.fromhex(fingerprint):
-        raise WrongMREnclave(
-            "Code fingerprint is wrong "
-            f"(read {bytes(quote.report_body.mr_enclave).hex()} "
-            f"but should be {fingerprint})"
-        )
+    if fingerprint:
+        if quote.report_body.mr_enclave != bytes.fromhex(fingerprint):
+            raise WrongMREnclave(
+                "Code fingerprint is wrong "
+                f"(read {bytes(quote.report_body.mr_enclave).hex()} "
+                f"but should be {fingerprint})"
+            )
```

### Comparing `mse_cli_core-0.1a2/src/mse_cli_core/fs.py` & `mse_cli_core-0.1a4/src/mse_cli_core/fs.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a2/src/mse_cli_core/ignore_file.py` & `mse_cli_core-0.1a4/src/mse_cli_core/ignore_file.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a2/src/mse_cli_core/no_sgx_docker.py` & `mse_cli_core-0.1a4/src/mse_cli_core/no_sgx_docker.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a2/src/mse_cli_core/sgx_docker.py` & `mse_cli_core-0.1a4/src/mse_cli_core/sgx_docker.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a2/src/mse_cli_core/test_docker.py` & `mse_cli_core-0.1a4/src/mse_cli_core/test_docker.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a2/src/mse_cli_core.egg-info/PKG-INFO` & `mse_cli_core-0.1a4/src/mse_cli_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mse-cli-core
-Version: 0.1a2
+Version: 0.1a4
 Summary: Utils for MicroService Encryption Python CLIs
 Home-page: https://cosmian.com
 Author: Cosmian Tech
 Author-email: tech@cosmian.com
 License: MIT
 Project-URL: Documentation, https://docs.cosmian.com
 Project-URL: Source, https://github.com/Cosmian/mse-cli-core
```

### Comparing `mse_cli_core-0.1a2/src/mse_cli_core.egg-info/SOURCES.txt` & `mse_cli_core-0.1a4/src/mse_cli_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a2/tests/test_base64.py` & `mse_cli_core-0.1a4/tests/test_base64.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a2/tests/test_boostrap.py` & `mse_cli_core-0.1a4/tests/test_boostrap.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a2/tests/test_ignore_file.py` & `mse_cli_core-0.1a4/tests/test_ignore_file.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a2/tests/test_no_sgx_docker.py` & `mse_cli_core-0.1a4/tests/test_no_sgx_docker.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a2/tests/test_sgx_docker.py` & `mse_cli_core-0.1a4/tests/test_sgx_docker.py`

 * *Files identical despite different names*

### Comparing `mse_cli_core-0.1a2/tests/test_test_docker.py` & `mse_cli_core-0.1a4/tests/test_test_docker.py`

 * *Files identical despite different names*

