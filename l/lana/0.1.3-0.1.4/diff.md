# Comparing `tmp/lana-0.1.3.tar.gz` & `tmp/lana-0.1.4.tar.gz`

## Comparing `lana-0.1.3.tar` & `lana-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0      280 1970-01-01 00:00:00.000000 lana-0.1.3/Cargo.toml
--rw-r--r--   0      501       20      719 2023-05-29 14:30:05.000000 lana-0.1.3/.gitignore
--rw-r--r--   0      501       20     1060 2023-05-15 16:24:44.000000 lana-0.1.3/LICENSE
--rw-r--r--   0      501       20      640 2023-05-30 13:21:54.000000 lana-0.1.3/README.md
--rw-r--r--   0      501       20      307 2023-05-30 13:22:32.000000 lana-0.1.3/examples/example.py
--rw-r--r--   0      501       20       53 2023-05-29 09:44:26.000000 lana-0.1.3/lana/__init__.py
--rw-r--r--   0      501       20      635 2023-05-15 19:10:53.000000 lana-0.1.3/pyproject.toml
--rw-r--r--   0      501       20      164 2023-05-29 14:28:02.000000 lana-0.1.3/src/lib.rs
--rw-r--r--   0      501       20     2508 2023-05-30 13:04:44.000000 lana-0.1.3/src/matrix.rs
--rw-r--r--   0      501       20      436 2023-05-30 09:01:52.000000 lana-0.1.3/test/test_matrix.py
--rw-r--r--   0      501       20     7648 2023-05-30 10:27:45.000000 lana-0.1.3/Cargo.lock
--rw-r--r--   0        0        0     1181 1970-01-01 00:00:00.000000 lana-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      293 1970-01-01 00:00:00.000000 lana-0.1.4/Cargo.toml
+-rw-r--r--   0      501       20      719 2023-05-29 14:30:05.000000 lana-0.1.4/.gitignore
+-rw-r--r--   0      501       20     1060 2023-05-15 16:24:44.000000 lana-0.1.4/LICENSE
+-rw-r--r--   0      501       20      640 2023-05-30 15:23:21.000000 lana-0.1.4/README.md
+-rw-r--r--   0      501       20      475 2023-05-30 15:51:57.000000 lana-0.1.4/examples/competition.py
+-rw-r--r--   0      501       20      331 2023-05-30 13:28:31.000000 lana-0.1.4/examples/example.py
+-rw-r--r--   0      501       20       53 2023-05-29 09:44:26.000000 lana-0.1.4/lana/__init__.py
+-rw-r--r--   0      501       20      651 2023-05-30 15:32:41.000000 lana-0.1.4/pyproject.toml
+-rw-r--r--   0      501       20      164 2023-05-29 14:28:02.000000 lana-0.1.4/src/lib.rs
+-rw-r--r--   0      501       20     3538 2023-05-30 15:54:04.000000 lana-0.1.4/src/matrix.rs
+-rw-r--r--   0      501       20      885 2023-05-30 13:33:31.000000 lana-0.1.4/test/test_matrix.py
+-rw-r--r--   0      501       20     9870 2023-05-30 15:15:06.000000 lana-0.1.4/Cargo.lock
+-rw-r--r--   0        0        0     1197 1970-01-01 00:00:00.000000 lana-0.1.4/PKG-INFO
```

### Comparing `lana-0.1.3/.gitignore` & `lana-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `lana-0.1.3/LICENSE` & `lana-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lana-0.1.3/README.md` & `lana-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `lana-0.1.3/pyproject.toml` & `lana-0.1.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.15,<0.16"]
 build-backend = "maturin"
 
 [project]
 name = "lana"
-description = "Linear Algebra experimental library"
+description = "Experimental Linear Algebra library written in Rust"
 authors = [
   { name = "Marco Salvalaggio", email = "mar.salvalaggio@gmail.com" },
 ]
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
 keywords = ["linear algebra"]
 classifiers = [
```

### Comparing `lana-0.1.3/Cargo.lock` & `lana-0.1.4/Cargo.lock`

 * *Files 10% similar despite different names*

```diff
@@ -17,24 +17,83 @@
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "crossbeam-channel"
+version = "0.5.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
+dependencies = [
+ "cfg-if",
+ "crossbeam-utils",
+]
+
+[[package]]
+name = "crossbeam-deque"
+version = "0.8.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ce6fd6f855243022dcecf8702fef0c297d4338e226845fe067f6341ad9fa0cef"
+dependencies = [
+ "cfg-if",
+ "crossbeam-epoch",
+ "crossbeam-utils",
+]
+
+[[package]]
+name = "crossbeam-epoch"
+version = "0.9.14"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "46bd5f3f85273295a9d14aedfb86f6aadbff6d8f5295c4a9edb08e819dcf5695"
+dependencies = [
+ "autocfg",
+ "cfg-if",
+ "crossbeam-utils",
+ "memoffset",
+ "scopeguard",
+]
+
+[[package]]
+name = "crossbeam-utils"
+version = "0.8.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3c063cd8cc95f5c377ed0d4b49a4b21f632396ff690e8470c29b3359b346984b"
+dependencies = [
+ "cfg-if",
+]
+
+[[package]]
+name = "either"
+version = "1.8.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
+
+[[package]]
+name = "hermit-abi"
+version = "0.2.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
+dependencies = [
+ "libc",
+]
+
+[[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "lana"
-version = "0.1.3"
+version = "0.1.4"
 dependencies = [
  "pyo3",
+ "rayon",
 ]
 
 [[package]]
 name = "libc"
 version = "0.2.144"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
@@ -55,14 +114,24 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
+name = "num_cpus"
+version = "1.15.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
+dependencies = [
+ "hermit-abi",
+ "libc",
+]
+
+[[package]]
 name = "once_cell"
 version = "1.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
 
 [[package]]
 name = "parking_lot"
@@ -162,14 +231,36 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f4f29d145265ec1c483c7c654450edde0bfe043d3938d6972630663356d9500"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
+name = "rayon"
+version = "1.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1d2df5196e37bcc87abebc0053e20787d73847bb33134a69841207dd0a47f03b"
+dependencies = [
+ "either",
+ "rayon-core",
+]
+
+[[package]]
+name = "rayon-core"
+version = "1.11.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4b8f95bd6966f5c87776639160a66bd8ab9895d9d4ab01ddba9fc60661aebe8d"
+dependencies = [
+ "crossbeam-channel",
+ "crossbeam-deque",
+ "crossbeam-utils",
+ "num_cpus",
+]
+
+[[package]]
 name = "redox_syscall"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
 dependencies = [
  "bitflags",
 ]
```

### Comparing `lana-0.1.3/PKG-INFO` & `lana-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: lana
-Version: 0.1.3
+Version: 0.1.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
-Summary: Linear Algebra experimental library
+Summary: Experimental Linear Algebra library written in Rust
 Keywords: linear algebra
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Repository, https://github.com/marcosalvalaggio/lana
 
 ## Lana 🧶
```

