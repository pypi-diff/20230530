# Comparing `tmp/parquet2lance-0.1.3.tar.gz` & `tmp/parquet2lance-0.2.0.tar.gz`

## Comparing `parquet2lance-0.1.3.tar` & `parquet2lance-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      555 1970-01-01 00:00:00.000000 parquet2lance-0.1.3/local_dependencies/parquet2lance/Cargo.toml
--rw-r--r--   0      503       20    90731 2023-05-19 06:46:41.000000 parquet2lance-0.1.3/local_dependencies/parquet2lance/Cargo.lock
--rw-r--r--   0      503       20     1064 2023-05-06 09:51:06.000000 parquet2lance-0.1.3/local_dependencies/parquet2lance/LICENSE
--rw-r--r--   0      503       20      856 2023-05-06 10:53:28.000000 parquet2lance-0.1.3/local_dependencies/parquet2lance/README.md
--rw-r--r--   0      503       20     1513 2023-05-05 09:28:08.000000 parquet2lance-0.1.3/local_dependencies/parquet2lance/src/io/fs.rs
--rw-r--r--   0      503       20     3391 2023-05-05 09:33:32.000000 parquet2lance-0.1.3/local_dependencies/parquet2lance/src/io/gcs.rs
--rw-r--r--   0      503       20     1060 2023-05-12 10:18:46.000000 parquet2lance-0.1.3/local_dependencies/parquet2lance/src/io/reader.rs
--rw-r--r--   0      503       20     3908 2023-05-06 06:36:50.000000 parquet2lance-0.1.3/local_dependencies/parquet2lance/src/io/util.rs
--rw-r--r--   0      503       20     1081 2023-05-12 10:12:10.000000 parquet2lance-0.1.3/local_dependencies/parquet2lance/src/io.rs
--rw-r--r--   0      503       20       44 2023-05-06 08:43:19.000000 parquet2lance-0.1.3/local_dependencies/parquet2lance/src/lib.rs
--rw-r--r--   0      503       20      992 2023-05-12 10:19:52.000000 parquet2lance-0.1.3/local_dependencies/parquet2lance/src/main.rs
--rw-r--r--   0        0        0      251 1970-01-01 00:00:00.000000 parquet2lance-0.1.3/Cargo.toml
--rw-r--r--   0      503       20     1064 2023-05-06 09:51:20.000000 parquet2lance-0.1.3/LICENSE
--rw-r--r--   0      503       20       69 2023-05-06 10:22:32.000000 parquet2lance-0.1.3/README.md
--rw-r--r--   0      503       20      661 2023-05-15 08:05:34.000000 parquet2lance-0.1.3/pyproject.toml
--rw-r--r--   0      503       20      562 2023-05-06 10:15:09.000000 parquet2lance-0.1.3/src/lib.rs
--rw-r--r--   0      503       20    97303 2023-05-19 06:46:33.000000 parquet2lance-0.1.3/Cargo.lock
--rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 parquet2lance-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      555 1970-01-01 00:00:00.000000 parquet2lance-0.2.0/local_dependencies/parquet2lance/Cargo.toml
+-rw-r--r--   0      503       20    90731 2023-05-22 03:14:07.000000 parquet2lance-0.2.0/local_dependencies/parquet2lance/Cargo.lock
+-rw-r--r--   0      503       20     1064 2023-05-06 09:51:06.000000 parquet2lance-0.2.0/local_dependencies/parquet2lance/LICENSE
+-rw-r--r--   0      503       20      856 2023-05-06 10:53:28.000000 parquet2lance-0.2.0/local_dependencies/parquet2lance/README.md
+-rw-r--r--   0      503       20     1513 2023-05-05 09:28:08.000000 parquet2lance-0.2.0/local_dependencies/parquet2lance/src/io/fs.rs
+-rw-r--r--   0      503       20     3391 2023-05-05 09:33:32.000000 parquet2lance-0.2.0/local_dependencies/parquet2lance/src/io/gcs.rs
+-rw-r--r--   0      503       20     1060 2023-05-12 10:18:46.000000 parquet2lance-0.2.0/local_dependencies/parquet2lance/src/io/reader.rs
+-rw-r--r--   0      503       20     3908 2023-05-06 06:36:50.000000 parquet2lance-0.2.0/local_dependencies/parquet2lance/src/io/util.rs
+-rw-r--r--   0      503       20     1439 2023-05-29 07:13:33.000000 parquet2lance-0.2.0/local_dependencies/parquet2lance/src/io.rs
+-rw-r--r--   0      503       20       44 2023-05-06 08:43:19.000000 parquet2lance-0.2.0/local_dependencies/parquet2lance/src/lib.rs
+-rw-r--r--   0      503       20      992 2023-05-12 10:19:52.000000 parquet2lance-0.2.0/local_dependencies/parquet2lance/src/main.rs
+-rw-r--r--   0        0        0      251 1970-01-01 00:00:00.000000 parquet2lance-0.2.0/Cargo.toml
+-rw-r--r--   0      503       20     1064 2023-05-06 09:51:20.000000 parquet2lance-0.2.0/LICENSE
+-rw-r--r--   0      503       20       69 2023-05-06 10:22:32.000000 parquet2lance-0.2.0/README.md
+-rw-r--r--   0      503       20      661 2023-05-15 08:05:34.000000 parquet2lance-0.2.0/pyproject.toml
+-rw-r--r--   0      503       20      562 2023-05-06 10:15:09.000000 parquet2lance-0.2.0/src/lib.rs
+-rw-r--r--   0      503       20    97303 2023-05-30 06:52:11.000000 parquet2lance-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 parquet2lance-0.2.0/PKG-INFO
```

### Comparing `parquet2lance-0.1.3/local_dependencies/parquet2lance/Cargo.toml` & `parquet2lance-0.2.0/local_dependencies/parquet2lance/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "parquet2lance"
-version = "0.2.4"
+version = "0.2.5"
 edition = "2021"
 description = "Convert parquet files to lance"
 repository = "https://github.com/haoxins/parquet2lance"
 license-file = "LICENSE"
 keywords = ["parquet", "lance", "object_store", "gcs"]
 
 [dependencies]
```

### Comparing `parquet2lance-0.1.3/local_dependencies/parquet2lance/Cargo.lock` & `parquet2lance-0.2.0/local_dependencies/parquet2lance/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -2288,15 +2288,15 @@
  "tokio",
  "twox-hash",
  "zstd",
 ]
 
 [[package]]
 name = "parquet2lance"
-version = "0.2.4"
+version = "0.2.5"
 dependencies = [
  "arrow",
  "arrow-array",
  "clap",
  "futures",
  "lance",
  "object_store",
```

### Comparing `parquet2lance-0.1.3/local_dependencies/parquet2lance/LICENSE` & `parquet2lance-0.2.0/local_dependencies/parquet2lance/LICENSE`

 * *Files identical despite different names*

### Comparing `parquet2lance-0.1.3/local_dependencies/parquet2lance/README.md` & `parquet2lance-0.2.0/local_dependencies/parquet2lance/README.md`

 * *Files identical despite different names*

### Comparing `parquet2lance-0.1.3/local_dependencies/parquet2lance/src/io/fs.rs` & `parquet2lance-0.2.0/local_dependencies/parquet2lance/src/io/fs.rs`

 * *Files identical despite different names*

### Comparing `parquet2lance-0.1.3/local_dependencies/parquet2lance/src/io/gcs.rs` & `parquet2lance-0.2.0/local_dependencies/parquet2lance/src/io/gcs.rs`

 * *Files identical despite different names*

### Comparing `parquet2lance-0.1.3/local_dependencies/parquet2lance/src/io/reader.rs` & `parquet2lance-0.2.0/local_dependencies/parquet2lance/src/io/reader.rs`

 * *Files identical despite different names*

### Comparing `parquet2lance-0.1.3/local_dependencies/parquet2lance/src/io/util.rs` & `parquet2lance-0.2.0/local_dependencies/parquet2lance/src/io/util.rs`

 * *Files identical despite different names*

### Comparing `parquet2lance-0.1.3/local_dependencies/parquet2lance/src/io.rs` & `parquet2lance-0.2.0/local_dependencies/parquet2lance/src/io.rs`

 * *Files 21% similar despite different names*

```diff
@@ -19,17 +19,28 @@
     let mut initialized = false;
 
     while let Some(mut f) = reader.next().await {
         let output_dir = output_dir.to_str().unwrap();
 
         let write_params = get_write_params(initialized, overwrite);
 
-        Dataset::write(&mut f, output_dir, Some(write_params))
-            .await
-            .unwrap();
+        let result = Dataset::write(&mut f, output_dir, Some(write_params)).await;
+
+        match result {
+            Ok(_) => (),
+            Err(e) => {
+                if e.to_string()
+                    .contains("Attempt to write empty record batches")
+                {
+                    println!("Empty record, skipping");
+                    continue;
+                }
+                panic!("Error writing record: {:?}", e);
+            }
+        }
 
         initialized = true;
     }
 }
 
 fn get_write_params(initialized: bool, overwrite: bool) -> WriteParams {
     let mut params = WriteParams::default();
```

### Comparing `parquet2lance-0.1.3/local_dependencies/parquet2lance/src/main.rs` & `parquet2lance-0.2.0/local_dependencies/parquet2lance/src/main.rs`

 * *Files identical despite different names*

### Comparing `parquet2lance-0.1.3/LICENSE` & `parquet2lance-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `parquet2lance-0.1.3/pyproject.toml` & `parquet2lance-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `parquet2lance-0.1.3/src/lib.rs` & `parquet2lance-0.2.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `parquet2lance-0.1.3/Cargo.lock` & `parquet2lance-0.2.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -2299,15 +2299,15 @@
 name = "outref"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4030760ffd992bef45b0ae3f10ce1aba99e33464c90d14dd7c039884963ddc7a"
 
 [[package]]
 name = "p2l"
-version = "0.1.3"
+version = "0.2.0"
 dependencies = [
  "parquet2lance",
  "pyo3",
  "tokio",
 ]
 
 [[package]]
@@ -2364,15 +2364,15 @@
  "tokio",
  "twox-hash",
  "zstd",
 ]
 
 [[package]]
 name = "parquet2lance"
-version = "0.2.4"
+version = "0.2.5"
 dependencies = [
  "arrow",
  "arrow-array",
  "clap",
  "futures",
  "lance",
  "object_store",
```

### Comparing `parquet2lance-0.1.3/PKG-INFO` & `parquet2lance-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parquet2lance
-Version: 0.1.3
+Version: 0.2.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE
 Summary: The Python wrapper for the Rust parquet2lance
 Keywords: arrow,lance,parquet
```

