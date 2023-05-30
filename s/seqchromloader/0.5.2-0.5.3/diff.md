# Comparing `tmp/seqchromloader-0.5.2.tar.gz` & `tmp/seqchromloader-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqchromloader-0.5.2.tar", last modified: Tue May 30 05:36:32 2023, max compression
+gzip compressed data, was "seqchromloader-0.5.3.tar", last modified: Tue May 30 17:03:04 2023, max compression
```

## Comparing `seqchromloader-0.5.2.tar` & `seqchromloader-0.5.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jmy5455  (258298369) 357253257        0 2023-05-30 05:36:32.700065 seqchromloader-0.5.2/
--rw-r--r--   0 jmy5455  (258298369) 357253257     1086 2023-05-30 05:36:32.699520 seqchromloader-0.5.2/PKG-INFO
--rw-r--r--   0 jmy5455  (258298369) 357253257      649 2023-03-27 19:08:58.000000 seqchromloader-0.5.2/README.md
-drwxr-xr-x   0 jmy5455  (258298369) 357253257        0 2023-05-30 05:36:32.692615 seqchromloader-0.5.2/seqchromloader/
--rw-r--r--   0 jmy5455  (258298369) 357253257      313 2023-05-30 03:38:50.000000 seqchromloader-0.5.2/seqchromloader/__init__.py
--rw-r--r--   0 jmy5455  (258298369) 357253257    12427 2023-05-30 04:51:02.000000 seqchromloader-0.5.2/seqchromloader/loader.py
--rw-r--r--   0 jmy5455  (258298369) 357253257    12391 2023-05-30 04:41:31.000000 seqchromloader-0.5.2/seqchromloader/utils.py
--rw-r--r--   0 jmy5455  (258298369) 357253257     6694 2023-05-30 05:32:58.000000 seqchromloader-0.5.2/seqchromloader/writer.py
-drwxr-xr-x   0 jmy5455  (258298369) 357253257        0 2023-05-30 05:36:32.697919 seqchromloader-0.5.2/seqchromloader.egg-info/
--rw-r--r--   0 jmy5455  (258298369) 357253257     1086 2023-05-30 05:36:32.000000 seqchromloader-0.5.2/seqchromloader.egg-info/PKG-INFO
--rw-r--r--   0 jmy5455  (258298369) 357253257      336 2023-05-30 05:36:32.000000 seqchromloader-0.5.2/seqchromloader.egg-info/SOURCES.txt
--rw-r--r--   0 jmy5455  (258298369) 357253257        1 2023-05-30 05:36:32.000000 seqchromloader-0.5.2/seqchromloader.egg-info/dependency_links.txt
--rw-r--r--   0 jmy5455  (258298369) 357253257      126 2023-05-30 05:36:32.000000 seqchromloader-0.5.2/seqchromloader.egg-info/requires.txt
--rw-r--r--   0 jmy5455  (258298369) 357253257       15 2023-05-30 05:36:32.000000 seqchromloader-0.5.2/seqchromloader.egg-info/top_level.txt
--rw-r--r--   0 jmy5455  (258298369) 357253257       38 2023-05-30 05:36:32.700213 seqchromloader-0.5.2/setup.cfg
--rw-r--r--   0 jmy5455  (258298369) 357253257     3368 2023-05-30 04:43:17.000000 seqchromloader-0.5.2/setup.py
-drwxr-xr-x   0 jmy5455  (258298369) 357253257        0 2023-05-30 05:36:32.698706 seqchromloader-0.5.2/tests/
--rw-r--r--   0 jmy5455  (258298369) 357253257    10950 2023-05-30 05:34:50.000000 seqchromloader-0.5.2/tests/test_writer_loader.py
+drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-05-30 17:03:04.504793 seqchromloader-0.5.3/
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1374 2023-05-30 17:03:04.504229 seqchromloader-0.5.3/PKG-INFO
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      649 2023-03-27 19:08:58.000000 seqchromloader-0.5.3/README.md
+drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-05-30 17:03:04.492703 seqchromloader-0.5.3/seqchromloader/
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      313 2023-05-30 03:38:50.000000 seqchromloader-0.5.3/seqchromloader/__init__.py
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    12427 2023-05-30 04:51:02.000000 seqchromloader-0.5.3/seqchromloader/loader.py
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    12391 2023-05-30 04:41:31.000000 seqchromloader-0.5.3/seqchromloader/utils.py
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     6693 2023-05-30 16:57:25.000000 seqchromloader-0.5.3/seqchromloader/writer.py
+drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-05-30 17:03:04.497095 seqchromloader-0.5.3/seqchromloader.egg-info/
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1374 2023-05-30 17:03:04.000000 seqchromloader-0.5.3/seqchromloader.egg-info/PKG-INFO
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      336 2023-05-30 17:03:04.000000 seqchromloader-0.5.3/seqchromloader.egg-info/SOURCES.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)        1 2023-05-30 17:03:04.000000 seqchromloader-0.5.3/seqchromloader.egg-info/dependency_links.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      126 2023-05-30 17:03:04.000000 seqchromloader-0.5.3/seqchromloader.egg-info/requires.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       15 2023-05-30 17:03:04.000000 seqchromloader-0.5.3/seqchromloader.egg-info/top_level.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       38 2023-05-30 17:03:04.504893 seqchromloader-0.5.3/setup.cfg
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     3368 2023-05-30 17:02:33.000000 seqchromloader-0.5.3/setup.py
+drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-05-30 17:03:04.503274 seqchromloader-0.5.3/tests/
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    10950 2023-05-30 05:34:50.000000 seqchromloader-0.5.3/tests/test_writer_loader.py
```

### Comparing `seqchromloader-0.5.2/PKG-INFO` & `seqchromloader-0.5.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 Metadata-Version: 2.1
 Name: seqchromloader
-Version: 0.5.2
+Version: 0.5.3
 Summary: Sequence and chromatin dataloader for deep learning
 Home-page: https://github.com/yztxwd/seqchromloader
 Author-email: yztxwd@gmail.com
+License: UNKNOWN
+Description: # seqchromloader
+        
+        seqchromloader aims to provide versatile and ready-to-use writer/loader for applying deep learning to bioinformatics study.
+        
+        Plan to support dataset formats including:
+        - webdataset (done)
+        - tfrecord (x)
+        
+        Training framework support:
+        - pytorch dataloader (done)
+        - pytorch-lightning datamodule (done)
+        - NVIDIA-DALI (x)
+        
+        ## Installation
+        
+        ### conda (suggested):
+        
+        `mamba install -c bioconda -c conda-forge seqchromloader`
+        
+        or
+        
+        `conda install -c bioconda -c conda-forge seqchromloader`
+        
+        ### pip
+        
+        `pip install seqchromloader`
+        
+        ## Usage
+        
+        For detailed usage, please refer to [documentation](https://seqchromloader.readthedocs.io/en/latest/)
+        
 Keywords: dataloder,pytorch,webdataset
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
-
-# seqchromloader
-
-seqchromloader aims to provide versatile and ready-to-use writer/loader for applying deep learning to bioinformatics study.
-
-Plan to support dataset formats including:
-- webdataset (done)
-- tfrecord (x)
-
-Training framework support:
-- pytorch dataloader (done)
-- pytorch-lightning datamodule (done)
-- NVIDIA-DALI (x)
-
-## Installation
-
-### conda (suggested):
-
-`mamba install -c bioconda -c conda-forge seqchromloader`
-
-or
-
-`conda install -c bioconda -c conda-forge seqchromloader`
-
-### pip
-
-`pip install seqchromloader`
-
-## Usage
-
-For detailed usage, please refer to [documentation](https://seqchromloader.readthedocs.io/en/latest/)
```

### Comparing `seqchromloader-0.5.2/README.md` & `seqchromloader-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `seqchromloader-0.5.2/seqchromloader/loader.py` & `seqchromloader-0.5.3/seqchromloader/loader.py`

 * *Files identical despite different names*

### Comparing `seqchromloader-0.5.2/seqchromloader/utils.py` & `seqchromloader-0.5.3/seqchromloader/utils.py`

 * *Files identical despite different names*

### Comparing `seqchromloader-0.5.2/seqchromloader/writer.py` & `seqchromloader-0.5.3/seqchromloader/writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     pool = Pool(numProcessors)
     res = pool.starmap_async(dump_data_worker_freeze, zip(chunks, [outprefix + "_" + format(i, f'0{count_of_digits}d') for i in range(num_chunks)]))
     files = res.get()
     
     if braceexpand:
         begin = format(0, f'0{count_of_digits}d')
         end = format(range(num_chunks)[-1], f'0{count_of_digits}d')
-        return os.path.join(outdir, f"{outprefix}_{{{begin}..{end}}}.tar.gz" if compress else f"{outprefix}_{{{begin}...{end}}}.tar")
+        return os.path.join(outdir, f"{outprefix}_{{{begin}..{end}}}.tar.gz" if compress else f"{outprefix}_{{{begin}..{end}}}.tar")
     else:
         return files
 
 def dump_data_webdataset_worker(coords, 
                                 outprefix, 
                                 fasta, 
                                 bigwig_files,
```

### Comparing `seqchromloader-0.5.2/seqchromloader.egg-info/PKG-INFO` & `seqchromloader-0.5.3/seqchromloader.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 Metadata-Version: 2.1
 Name: seqchromloader
-Version: 0.5.2
+Version: 0.5.3
 Summary: Sequence and chromatin dataloader for deep learning
 Home-page: https://github.com/yztxwd/seqchromloader
 Author-email: yztxwd@gmail.com
+License: UNKNOWN
+Description: # seqchromloader
+        
+        seqchromloader aims to provide versatile and ready-to-use writer/loader for applying deep learning to bioinformatics study.
+        
+        Plan to support dataset formats including:
+        - webdataset (done)
+        - tfrecord (x)
+        
+        Training framework support:
+        - pytorch dataloader (done)
+        - pytorch-lightning datamodule (done)
+        - NVIDIA-DALI (x)
+        
+        ## Installation
+        
+        ### conda (suggested):
+        
+        `mamba install -c bioconda -c conda-forge seqchromloader`
+        
+        or
+        
+        `conda install -c bioconda -c conda-forge seqchromloader`
+        
+        ### pip
+        
+        `pip install seqchromloader`
+        
+        ## Usage
+        
+        For detailed usage, please refer to [documentation](https://seqchromloader.readthedocs.io/en/latest/)
+        
 Keywords: dataloder,pytorch,webdataset
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
-
-# seqchromloader
-
-seqchromloader aims to provide versatile and ready-to-use writer/loader for applying deep learning to bioinformatics study.
-
-Plan to support dataset formats including:
-- webdataset (done)
-- tfrecord (x)
-
-Training framework support:
-- pytorch dataloader (done)
-- pytorch-lightning datamodule (done)
-- NVIDIA-DALI (x)
-
-## Installation
-
-### conda (suggested):
-
-`mamba install -c bioconda -c conda-forge seqchromloader`
-
-or
-
-`conda install -c bioconda -c conda-forge seqchromloader`
-
-### pip
-
-`pip install seqchromloader`
-
-## Usage
-
-For detailed usage, please refer to [documentation](https://seqchromloader.readthedocs.io/en/latest/)
```

### Comparing `seqchromloader-0.5.2/setup.py` & `seqchromloader-0.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     # The version of your project.
     # Usually, it would be in the form of:
     # major.minor.patch
     # eg: 1.0.0, 1.0.1, 3.0.2, 5.0-beta, etc.
     # You CANNOT upload two versions of your package with the same version number
     # This field is REQUIRED
-    version="0.5.2",
+    version="0.5.3",
 
     # The packages that constitute your project.
     # For my project, I have only one - "pydash".
     # Either you could write the name of the package, or
     # alternatively use setuptools.findpackages()
     #
     # If you only have one file, instead of a package,
```

### Comparing `seqchromloader-0.5.2/tests/test_writer_loader.py` & `seqchromloader-0.5.3/tests/test_writer_loader.py`

 * *Files identical despite different names*

