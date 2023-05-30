# Comparing `tmp/lana-0.1.2.tar.gz` & `tmp/lana-0.1.3.tar.gz`

## Comparing `lana-0.1.2.tar` & `lana-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      280 1970-01-01 00:00:00.000000 lana-0.1.2/Cargo.toml
--rw-r--r--   0      501       20      719 2023-05-29 14:30:05.000000 lana-0.1.2/.gitignore
--rw-r--r--   0      501       20     1060 2023-05-15 16:24:44.000000 lana-0.1.2/LICENSE
--rw-r--r--   0      501       20      611 2023-05-30 09:01:23.000000 lana-0.1.2/README.md
--rw-r--r--   0      501       20      165 2023-05-30 09:04:59.000000 lana-0.1.2/examples/example.py
--rw-r--r--   0      501       20       53 2023-05-29 09:44:26.000000 lana-0.1.2/lana/__init__.py
--rw-r--r--   0      501       20      635 2023-05-15 19:10:53.000000 lana-0.1.2/pyproject.toml
--rw-r--r--   0      501       20      164 2023-05-29 14:28:02.000000 lana-0.1.2/src/lib.rs
--rw-r--r--   0      501       20     1402 2023-05-30 08:54:38.000000 lana-0.1.2/src/matrix.rs
--rw-r--r--   0      501       20      436 2023-05-30 09:01:52.000000 lana-0.1.2/test/test_matrix.py
--rw-r--r--   0      501       20     7648 2023-05-30 08:55:16.000000 lana-0.1.2/Cargo.lock
--rw-r--r--   0        0        0     1152 1970-01-01 00:00:00.000000 lana-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      280 1970-01-01 00:00:00.000000 lana-0.1.3/Cargo.toml
+-rw-r--r--   0      501       20      719 2023-05-29 14:30:05.000000 lana-0.1.3/.gitignore
+-rw-r--r--   0      501       20     1060 2023-05-15 16:24:44.000000 lana-0.1.3/LICENSE
+-rw-r--r--   0      501       20      640 2023-05-30 13:21:54.000000 lana-0.1.3/README.md
+-rw-r--r--   0      501       20      307 2023-05-30 13:22:32.000000 lana-0.1.3/examples/example.py
+-rw-r--r--   0      501       20       53 2023-05-29 09:44:26.000000 lana-0.1.3/lana/__init__.py
+-rw-r--r--   0      501       20      635 2023-05-15 19:10:53.000000 lana-0.1.3/pyproject.toml
+-rw-r--r--   0      501       20      164 2023-05-29 14:28:02.000000 lana-0.1.3/src/lib.rs
+-rw-r--r--   0      501       20     2508 2023-05-30 13:04:44.000000 lana-0.1.3/src/matrix.rs
+-rw-r--r--   0      501       20      436 2023-05-30 09:01:52.000000 lana-0.1.3/test/test_matrix.py
+-rw-r--r--   0      501       20     7648 2023-05-30 10:27:45.000000 lana-0.1.3/Cargo.lock
+-rw-r--r--   0        0        0     1181 1970-01-01 00:00:00.000000 lana-0.1.3/PKG-INFO
```

### Comparing `lana-0.1.2/.gitignore` & `lana-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `lana-0.1.2/LICENSE` & `lana-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lana-0.1.2/README.md` & `lana-0.1.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 ```python
 from lana import Matrix
 
 zeros = Matrix.zeros((3,3))
 print(zeros)
 print(f"shape: {zeros.shape}, type: {type(zeros)}")
+print(zeros[0], zeros[0][0])
 
 mat = Matrix.matrix([[1,2,3],[4,5,6]])
 print(mat)
 print(f"shape: {mat.shape}, type: {type(mat)}")
 for rows in mat:
     print(rows, type(rows))
 ```
```

### Comparing `lana-0.1.2/pyproject.toml` & `lana-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lana-0.1.2/Cargo.lock` & `lana-0.1.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "lana"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "libc"
 version = "0.2.144"
```

### Comparing `lana-0.1.2/PKG-INFO` & `lana-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lana
-Version: 0.1.2
+Version: 0.1.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Linear Algebra experimental library
 Keywords: linear algebra
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
@@ -28,14 +28,15 @@
 
 ```python
 from lana import Matrix
 
 zeros = Matrix.zeros((3,3))
 print(zeros)
 print(f"shape: {zeros.shape}, type: {type(zeros)}")
+print(zeros[0], zeros[0][0])
 
 mat = Matrix.matrix([[1,2,3],[4,5,6]])
 print(mat)
 print(f"shape: {mat.shape}, type: {type(mat)}")
 for rows in mat:
     print(rows, type(rows))
 ```
```

