# Comparing `tmp/sgx_pck_extension-0.1.3.tar.gz` & `tmp/sgx_pck_extension-0.1.4.tar.gz`

## Comparing `sgx_pck_extension-0.1.3.tar` & `sgx_pck_extension-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      260 1970-01-01 00:00:00.000000 sgx_pck_extension-0.1.3/Cargo.toml
--rw-r--r--   0     1000     1000      508 2023-05-25 14:33:40.000000 sgx_pck_extension-0.1.3/pyproject.toml
--rw-r--r--   0     1000     1000      454 2023-05-25 14:36:14.000000 sgx_pck_extension-0.1.3/python/sgx_pck_extension/__init__.py
--rw-r--r--   0     1000     1000        0 2023-05-25 16:09:05.000000 sgx_pck_extension-0.1.3/python/sgx_pck_extension/py.typed
--rw-r--r--   0     1000     1000      619 2023-05-25 12:50:18.000000 sgx_pck_extension-0.1.3/src/error.rs
--rw-r--r--   0     1000     1000    14446 2023-05-25 12:50:18.000000 sgx_pck_extension-0.1.3/src/extension.rs
--rw-r--r--   0     1000     1000     1915 2023-05-25 12:54:40.000000 sgx_pck_extension-0.1.3/src/lib.rs
--rw-r--r--   0     1000     1000    14417 2023-05-30 13:15:15.000000 sgx_pck_extension-0.1.3/Cargo.lock
--rw-r--r--   0        0        0      312 1970-01-01 00:00:00.000000 sgx_pck_extension-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      260 1970-01-01 00:00:00.000000 sgx_pck_extension-0.1.4/Cargo.toml
+-rw-r--r--   0     1000     1000      508 2023-05-25 14:33:40.000000 sgx_pck_extension-0.1.4/pyproject.toml
+-rw-r--r--   0     1000     1000      454 2023-05-25 14:36:14.000000 sgx_pck_extension-0.1.4/python/sgx_pck_extension/__init__.py
+-rw-r--r--   0     1000     1000        0 2023-05-25 16:09:05.000000 sgx_pck_extension-0.1.4/python/sgx_pck_extension/py.typed
+-rw-r--r--   0     1000     1000      619 2023-05-25 12:50:18.000000 sgx_pck_extension-0.1.4/src/error.rs
+-rw-r--r--   0     1000     1000    14446 2023-05-25 12:50:18.000000 sgx_pck_extension-0.1.4/src/extension.rs
+-rw-r--r--   0     1000     1000     1915 2023-05-25 12:54:40.000000 sgx_pck_extension-0.1.4/src/lib.rs
+-rw-r--r--   0     1000     1000    14417 2023-05-30 13:53:05.000000 sgx_pck_extension-0.1.4/Cargo.lock
+-rw-r--r--   0        0        0      312 1970-01-01 00:00:00.000000 sgx_pck_extension-0.1.4/PKG-INFO
```

### Comparing `sgx_pck_extension-0.1.3/src/error.rs` & `sgx_pck_extension-0.1.4/src/error.rs`

 * *Files identical despite different names*

### Comparing `sgx_pck_extension-0.1.3/src/extension.rs` & `sgx_pck_extension-0.1.4/src/extension.rs`

 * *Files identical despite different names*

### Comparing `sgx_pck_extension-0.1.3/src/lib.rs` & `sgx_pck_extension-0.1.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `sgx_pck_extension-0.1.3/Cargo.lock` & `sgx_pck_extension-0.1.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -349,15 +349,15 @@
 name = "serde"
 version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2113ab51b87a539ae008b5c6c02dc020ffa39afd2d83cffcb3f4eb2722cebec2"
 
 [[package]]
 name = "sgx-pck-extension"
-version = "0.1.3"
+version = "0.1.4"
 dependencies = [
  "asn1",
  "asn1-rs",
  "pyo3",
  "x509-parser",
 ]
```

