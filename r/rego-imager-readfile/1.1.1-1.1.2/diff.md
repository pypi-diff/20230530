# Comparing `tmp/rego_imager_readfile-1.1.1.tar.gz` & `tmp/rego_imager_readfile-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rego_imager_readfile-1.1.1.tar", max compression
+gzip compressed data, was "rego_imager_readfile-1.1.2.tar", max compression
```

## Comparing `rego_imager_readfile-1.1.1.tar` & `rego_imager_readfile-1.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1078 2021-02-25 19:14:26.000000 rego_imager_readfile-1.1.1/LICENSE
--rw-r--r--   0        0        0     2400 2023-05-05 00:57:47.375894 rego_imager_readfile-1.1.1/README.md
--rw-r--r--   0        0        0      656 2023-05-05 13:26:03.190968 rego_imager_readfile-1.1.1/pyproject.toml
--rw-r--r--   0        0        0       47 2023-05-05 13:26:03.223968 rego_imager_readfile-1.1.1/rego_imager_readfile/__init__.py
--rw-r--r--   0        0        0     7731 2021-03-29 15:25:44.000000 rego_imager_readfile-1.1.1/rego_imager_readfile/_rego.py
--rw-r--r--   0        0        0     3099 1970-01-01 00:00:00.000000 rego_imager_readfile-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2021-02-25 19:14:26.000000 rego_imager_readfile-1.1.2/LICENSE
+-rw-r--r--   0        0        0     2688 2023-05-30 20:01:33.986595 rego_imager_readfile-1.1.2/README.md
+-rw-r--r--   0        0        0      656 2023-05-30 19:42:44.551426 rego_imager_readfile-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-05-30 19:42:44.587427 rego_imager_readfile-1.1.2/rego_imager_readfile/__init__.py
+-rw-r--r--   0        0        0     7886 2023-05-30 19:54:16.486928 rego_imager_readfile-1.1.2/rego_imager_readfile/_rego.py
+-rw-r--r--   0        0        0     3387 1970-01-01 00:00:00.000000 rego_imager_readfile-1.1.2/PKG-INFO
```

### Comparing `rego_imager_readfile-1.1.1/LICENSE` & `rego_imager_readfile-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rego_imager_readfile-1.1.1/README.md` & `rego_imager_readfile-1.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 
 Example Python notebooks can be found in the "examples" directory. Further, some examples can be found in the "Usage" section below.
 
 ## Usage
 
 Import the library using `import rego_imager_readfile`
 
+**Warning**: On Windows, be sure to put any `read` calls into a `main()` method. This is because we utilize the multiprocessing library and the method of forking processes in Windows requires it. Note that if you're using Jupyter or other IPython-based interfaces, this is not required.
+
 ### Read a single file
 
 ```python
 >>> import rego_imager_readfile
 >>> filename = "path/to/data/2020/01/01/fsmi_rego-654/ut06/20200101_0600_fsmi_rego-654_6300.pgm.gz"
 >>> img, meta, problematic_files = rego_imager_readfile.read(filename)
 ```
```

### Comparing `rego_imager_readfile-1.1.1/pyproject.toml` & `rego_imager_readfile-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rego-imager-readfile"
-version = "1.1.1"
+version = "1.1.2"
 description = "Read functions for REGO ASI PGM raw files"
 readme = "README.md"
 homepage = "https://github.com/ucalgary-aurora/rego-imager-readfile"
 repository = "https://github.com/ucalgary-aurora/rego-imager-readfile"
 authors = ["Darren Chaddock <dchaddoc@ucalgary.ca>"]
 license = "MIT"
 packages = [
```

### Comparing `rego_imager_readfile-1.1.1/rego_imager_readfile/_rego.py` & `rego_imager_readfile-1.1.2/rego_imager_readfile/_rego.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-# Author: Lukas Vollmerhaus
-# Date: 2020-10-16
-
-import gzip as gzip
+import gzip
+import signal
 import numpy as np
-import signal as signal
-from multiprocessing import Pool as Pool
+from multiprocessing import Pool
 
 # globals
 REGO_IMAGE_SIZE_BYTES = 512 * 512 * 2
 REGO_DT = np.dtype("uint16")
 REGO_DT = REGO_DT.newbyteorder('>')  # force big endian byte ordering
 
 
@@ -27,17 +24,22 @@
     # pre-allocate array sizes (optimization)
     predicted_num_frames = len(file_list) * 20
     images = np.empty([512, 512, predicted_num_frames], dtype=REGO_DT)
     metadata_dict_list = [{}] * predicted_num_frames
     problematic_file_list = []
 
     # set up process pool (ignore SIGINT before spawning pool so child processes inherit SIGINT handler)
-    original_sigint_handler = signal.signal(signal.SIGINT, signal.SIG_IGN)
-    pool = Pool(processes=workers)
-    signal.signal(signal.SIGINT, original_sigint_handler)  # restore SIGINT handler
+    try:
+        original_sigint_handler = signal.signal(signal.SIGINT, signal.SIG_IGN)
+        pool = Pool(processes=workers)
+        signal.signal(signal.SIGINT, original_sigint_handler)  # restore SIGINT handler
+    except ValueError:
+        # likely the read call is being used within a context that doesn't support the usage
+        # of signals in this way, proceed without it
+        pool = Pool(processes=workers)
 
     # if input is just a single file name in a string, convert to a list to be fed to the workers
     if isinstance(file_list, str):
         file_list = [file_list]
 
     # call readfile function, run each iteration with a single input file from file_list
     # NOTE: structure of data - data[file][metadata dictionary lists = 1, images = 0][frame]
```

### Comparing `rego_imager_readfile-1.1.1/PKG-INFO` & `rego_imager_readfile-1.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rego-imager-readfile
-Version: 1.1.1
+Version: 1.1.2
 Summary: Read functions for REGO ASI PGM raw files
 Home-page: https://github.com/ucalgary-aurora/rego-imager-readfile
 License: MIT
 Author: Darren Chaddock
 Author-email: dchaddoc@ucalgary.ca
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -45,14 +45,16 @@
 
 Example Python notebooks can be found in the "examples" directory. Further, some examples can be found in the "Usage" section below.
 
 ## Usage
 
 Import the library using `import rego_imager_readfile`
 
+**Warning**: On Windows, be sure to put any `read` calls into a `main()` method. This is because we utilize the multiprocessing library and the method of forking processes in Windows requires it. Note that if you're using Jupyter or other IPython-based interfaces, this is not required.
+
 ### Read a single file
 
 ```python
 >>> import rego_imager_readfile
 >>> filename = "path/to/data/2020/01/01/fsmi_rego-654/ut06/20200101_0600_fsmi_rego-654_6300.pgm.gz"
 >>> img, meta, problematic_files = rego_imager_readfile.read(filename)
 ```
```

