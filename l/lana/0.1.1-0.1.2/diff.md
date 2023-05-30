# Comparing `tmp/lana-0.1.1.tar.gz` & `tmp/lana-0.1.2.tar.gz`

## Comparing `lana-0.1.1.tar` & `lana-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      280 1970-01-01 00:00:00.000000 lana-0.1.1/Cargo.toml
--rw-r--r--   0      501       20      719 2023-05-29 14:30:05.000000 lana-0.1.1/.gitignore
--rw-r--r--   0      501       20     1060 2023-05-15 16:24:44.000000 lana-0.1.1/LICENSE
--rw-r--r--   0      501       20      688 2023-05-29 14:29:13.000000 lana-0.1.1/README.md
--rw-r--r--   0      501       20      161 2023-05-29 14:29:22.000000 lana-0.1.1/examples/example.py
--rw-r--r--   0      501       20       53 2023-05-29 09:44:26.000000 lana-0.1.1/lana/__init__.py
--rw-r--r--   0      501       20      635 2023-05-15 19:10:53.000000 lana-0.1.1/pyproject.toml
--rw-r--r--   0      501       20      164 2023-05-29 14:28:02.000000 lana-0.1.1/src/lib.rs
--rw-r--r--   0      501       20     1150 2023-05-29 14:28:30.000000 lana-0.1.1/src/matrix.rs
--rw-r--r--   0      501       20      441 2023-05-29 13:25:42.000000 lana-0.1.1/test/test_matrix.py
--rw-r--r--   0      501       20     7648 2023-05-29 14:28:18.000000 lana-0.1.1/Cargo.lock
--rw-r--r--   0        0        0     1229 1970-01-01 00:00:00.000000 lana-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      280 1970-01-01 00:00:00.000000 lana-0.1.2/Cargo.toml
+-rw-r--r--   0      501       20      719 2023-05-29 14:30:05.000000 lana-0.1.2/.gitignore
+-rw-r--r--   0      501       20     1060 2023-05-15 16:24:44.000000 lana-0.1.2/LICENSE
+-rw-r--r--   0      501       20      611 2023-05-30 09:01:23.000000 lana-0.1.2/README.md
+-rw-r--r--   0      501       20      165 2023-05-30 09:04:59.000000 lana-0.1.2/examples/example.py
+-rw-r--r--   0      501       20       53 2023-05-29 09:44:26.000000 lana-0.1.2/lana/__init__.py
+-rw-r--r--   0      501       20      635 2023-05-15 19:10:53.000000 lana-0.1.2/pyproject.toml
+-rw-r--r--   0      501       20      164 2023-05-29 14:28:02.000000 lana-0.1.2/src/lib.rs
+-rw-r--r--   0      501       20     1402 2023-05-30 08:54:38.000000 lana-0.1.2/src/matrix.rs
+-rw-r--r--   0      501       20      436 2023-05-30 09:01:52.000000 lana-0.1.2/test/test_matrix.py
+-rw-r--r--   0      501       20     7648 2023-05-30 08:55:16.000000 lana-0.1.2/Cargo.lock
+-rw-r--r--   0        0        0     1152 1970-01-01 00:00:00.000000 lana-0.1.2/PKG-INFO
```

### Comparing `lana-0.1.1/.gitignore` & `lana-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `lana-0.1.1/LICENSE` & `lana-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lana-0.1.1/pyproject.toml` & `lana-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lana-0.1.1/src/matrix.rs` & `lana-0.1.2/src/matrix.rs`

 * *Files 16% similar despite different names*

```diff
@@ -41,12 +41,19 @@
     #[getter]
     pub fn shape(&self) -> (usize, usize) {
         let rows = self.data.len();
         let cols = self.data[0].len();
         (rows, cols)
     }
 
+    pub fn __getitem__(&self, index: usize) -> PyResult<Vec<f64>> {
+        match self.data.get(index) {
+            Some(row) => Ok(row.clone()),
+            None => Err(pyo3::exceptions::PyIndexError::new_err("Index out of range")),
+        }
+    }
+
     fn __repr__(&self) -> PyResult<String> {
         Ok(format!("{:?}", self.data))
     }
 
 }
```

### Comparing `lana-0.1.1/Cargo.lock` & `lana-0.1.2/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "lana"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "libc"
 version = "0.2.144"
```

### Comparing `lana-0.1.1/PKG-INFO` & `lana-0.1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,24 @@
 Metadata-Version: 2.1
 Name: lana
-Version: 0.1.1
+Version: 0.1.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Linear Algebra experimental library
 Keywords: linear algebra
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Repository, https://github.com/marcosalvalaggio/lana
 
-## Lana
+## Lana 🧶
 
-```console
-    .-.'  `; `-._  __  _
-   (_,         .-:'  `; `-._
- ,'o"(        (_,           )
-(__,-'      ,'o"(            )>
-   (       (__,-'            )
-    `-'._.--._(             )
-       |||  |||`-'._.--._.-'
-                  |||  |||
-```
+[![stability-wip](https://img.shields.io/badge/stability-wip-lightgrey.svg)](https://github.com/mkenney/software-guides/blob/master/STABILITY-BADGES.md#work-in-progress) 
 
 **L***inear* **a***lgebra* *for* **n***octurnal and* **a***dventurous data scientists.*
 
 ## Install 
 
 ```console
 pip install lana
@@ -41,12 +32,12 @@
 zeros = Matrix.zeros((3,3))
 print(zeros)
 print(f"shape: {zeros.shape}, type: {type(zeros)}")
 
 mat = Matrix.matrix([[1,2,3],[4,5,6]])
 print(mat)
 print(f"shape: {mat.shape}, type: {type(mat)}")
-for rows in mat.data:
+for rows in mat:
     print(rows, type(rows))
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

