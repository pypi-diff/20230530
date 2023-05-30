# Comparing `tmp/seqchromloader-0.5.1.tar.gz` & `tmp/seqchromloader-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqchromloader-0.5.1.tar", last modified: Mon May 29 21:13:35 2023, max compression
+gzip compressed data, was "seqchromloader-0.5.2.tar", last modified: Tue May 30 05:36:32 2023, max compression
```

## Comparing `seqchromloader-0.5.1.tar` & `seqchromloader-0.5.2.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-05-29 21:13:35.871455 seqchromloader-0.5.1/
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1086 2023-05-29 21:13:35.871112 seqchromloader-0.5.1/PKG-INFO
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      649 2023-03-27 19:08:58.000000 seqchromloader-0.5.1/README.md
-drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-05-29 21:13:35.866532 seqchromloader-0.5.1/seqchromloader/
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      280 2023-05-29 18:55:42.000000 seqchromloader-0.5.1/seqchromloader/__init__.py
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    12427 2023-04-12 19:57:21.000000 seqchromloader-0.5.1/seqchromloader/loader.py
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     9899 2023-05-29 19:56:30.000000 seqchromloader-0.5.1/seqchromloader/utils.py
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     6666 2023-05-29 21:12:24.000000 seqchromloader-0.5.1/seqchromloader/writer.py
-drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-05-29 21:13:35.870646 seqchromloader-0.5.1/seqchromloader.egg-info/
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1086 2023-05-29 21:13:35.000000 seqchromloader-0.5.1/seqchromloader.egg-info/PKG-INFO
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      308 2023-05-29 21:13:35.000000 seqchromloader-0.5.1/seqchromloader.egg-info/SOURCES.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)        1 2023-05-29 21:13:35.000000 seqchromloader-0.5.1/seqchromloader.egg-info/dependency_links.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      126 2023-05-29 21:13:35.000000 seqchromloader-0.5.1/seqchromloader.egg-info/requires.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       15 2023-05-29 21:13:35.000000 seqchromloader-0.5.1/seqchromloader.egg-info/top_level.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       38 2023-05-29 21:13:35.871541 seqchromloader-0.5.1/setup.cfg
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     3368 2023-05-29 21:13:04.000000 seqchromloader-0.5.1/setup.py
+drwxr-xr-x   0 jmy5455  (258298369) 357253257        0 2023-05-30 05:36:32.700065 seqchromloader-0.5.2/
+-rw-r--r--   0 jmy5455  (258298369) 357253257     1086 2023-05-30 05:36:32.699520 seqchromloader-0.5.2/PKG-INFO
+-rw-r--r--   0 jmy5455  (258298369) 357253257      649 2023-03-27 19:08:58.000000 seqchromloader-0.5.2/README.md
+drwxr-xr-x   0 jmy5455  (258298369) 357253257        0 2023-05-30 05:36:32.692615 seqchromloader-0.5.2/seqchromloader/
+-rw-r--r--   0 jmy5455  (258298369) 357253257      313 2023-05-30 03:38:50.000000 seqchromloader-0.5.2/seqchromloader/__init__.py
+-rw-r--r--   0 jmy5455  (258298369) 357253257    12427 2023-05-30 04:51:02.000000 seqchromloader-0.5.2/seqchromloader/loader.py
+-rw-r--r--   0 jmy5455  (258298369) 357253257    12391 2023-05-30 04:41:31.000000 seqchromloader-0.5.2/seqchromloader/utils.py
+-rw-r--r--   0 jmy5455  (258298369) 357253257     6694 2023-05-30 05:32:58.000000 seqchromloader-0.5.2/seqchromloader/writer.py
+drwxr-xr-x   0 jmy5455  (258298369) 357253257        0 2023-05-30 05:36:32.697919 seqchromloader-0.5.2/seqchromloader.egg-info/
+-rw-r--r--   0 jmy5455  (258298369) 357253257     1086 2023-05-30 05:36:32.000000 seqchromloader-0.5.2/seqchromloader.egg-info/PKG-INFO
+-rw-r--r--   0 jmy5455  (258298369) 357253257      336 2023-05-30 05:36:32.000000 seqchromloader-0.5.2/seqchromloader.egg-info/SOURCES.txt
+-rw-r--r--   0 jmy5455  (258298369) 357253257        1 2023-05-30 05:36:32.000000 seqchromloader-0.5.2/seqchromloader.egg-info/dependency_links.txt
+-rw-r--r--   0 jmy5455  (258298369) 357253257      126 2023-05-30 05:36:32.000000 seqchromloader-0.5.2/seqchromloader.egg-info/requires.txt
+-rw-r--r--   0 jmy5455  (258298369) 357253257       15 2023-05-30 05:36:32.000000 seqchromloader-0.5.2/seqchromloader.egg-info/top_level.txt
+-rw-r--r--   0 jmy5455  (258298369) 357253257       38 2023-05-30 05:36:32.700213 seqchromloader-0.5.2/setup.cfg
+-rw-r--r--   0 jmy5455  (258298369) 357253257     3368 2023-05-30 04:43:17.000000 seqchromloader-0.5.2/setup.py
+drwxr-xr-x   0 jmy5455  (258298369) 357253257        0 2023-05-30 05:36:32.698706 seqchromloader-0.5.2/tests/
+-rw-r--r--   0 jmy5455  (258298369) 357253257    10950 2023-05-30 05:34:50.000000 seqchromloader-0.5.2/tests/test_writer_loader.py
```

### Comparing `seqchromloader-0.5.1/PKG-INFO` & `seqchromloader-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqchromloader
-Version: 0.5.1
+Version: 0.5.2
 Summary: Sequence and chromatin dataloader for deep learning
 Home-page: https://github.com/yztxwd/seqchromloader
 Author-email: yztxwd@gmail.com
 Keywords: dataloder,pytorch,webdataset
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `seqchromloader-0.5.1/README.md` & `seqchromloader-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `seqchromloader-0.5.1/seqchromloader/loader.py` & `seqchromloader-0.5.2/seqchromloader/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     Given bed file, return sequence and chromatin info
 """
 
 import logging
 import torch
 import random
 import pysam
-import pyfasta
+import pyfaidx
 import pyBigWig
 import numpy as np
 import pandas as pd
 import webdataset as wds
 from math import sqrt, ceil
 from itertools import islice
 from torch.utils.data import Dataset, IterableDataset, DataLoader
@@ -116,28 +116,28 @@
                  bigwig_filelist:list, 
                  target_bam=None, 
                  transforms:dict=None, 
                  initialize_first=False):
         
         self.dataframe = dataframe        
         self.genome_fasta = genome_fasta
-        self.genome_pyfasta = None
+        self.genome_pyfaidx = None
         self.bigwig_filelist = bigwig_filelist
         self.bigwigs = None
         self.target_bam = target_bam
         self.target_pysam = None
 
         self.transforms = transforms
 
         if initialize_first: self.initialize()
     
     def initialize(self):
         # create the stream handler after child processes spawned to enable parallel reading
         # this function will be called by worker_init_function in DataLoader
-        self.genome_pyfasta = pyfasta.Fasta(self.genome_fasta)
+        self.genome_pyfaidx = pyfaidx.Fasta(self.genome_fasta)
         self.bigwigs = [pyBigWig.open(bw) for bw in self.bigwig_filelist]
         if self.target_bam is not None:
             self.target_pysam = pysam.AlignmentFile(self.target_bam)
     
     def __len__(self):
         return len(self.dataframe)
 
@@ -145,15 +145,15 @@
         item = self.dataframe.iloc[idx,]
         try:
             feature = utils.extract_info(
                 item.chrom,
                 item.start,
                 item.end,
                 item.label,
-                genome_pyfasta=self.genome_pyfasta,
+                genome_pyfaidx=self.genome_pyfaidx,
                 bigwigs=self.bigwigs,
                 target_bam=self.target_pysam,
                 strand=item.strand,
                 transforms=self.transforms
             )
         except utils.BigWigInaccessible as e:
             raise e
```

### Comparing `seqchromloader-0.5.1/seqchromloader/writer.py` & `seqchromloader-0.5.2/seqchromloader/writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import numpy as np
 import functools
 import math
 import logging
 from collections import defaultdict
 from multiprocessing import Pool
 
-import pyfasta
+import pyfaidx
 import pysam
 import pyBigWig
 import webdataset as wds
 
 from . import utils
 from .loader import _SeqChromDatasetByWds
 
@@ -49,15 +49,15 @@
     
 def dump_data_webdataset(coords, genome_fasta, bigwig_filelist,
                         target_bam=None, 
                         outdir="dataset/", outprefix="seqchrom", 
                         compress=True, 
                         numProcessors=1,
                         transforms=None,
-                        braceexpand=True,
+                        braceexpand=False,
                         DALI=False):
     """
     Given coordinates dataframe, extract the sequence and chromatin signal, save in webdataset format
 
     :param coords: pandas DataFrame containing genomic coordinates with columns **[chrom, start, end, label]**
     :type coords: pandas DataFrame
     :param genome_fasta: Genome fasta file.
@@ -81,54 +81,55 @@
     :param DALI: Set to True if you want to use the dataset for NVIDIA DALI, it would save all arrays in bytes, which results in losing the array shape info
     :param DALI: boolean
     """
 
     # split coordinates and assign chunks to workers
     num_chunks = math.ceil(len(coords) / 7000)
     chunks = np.array_split(coords, num_chunks)
-
+    
     # freeze the common parameters
     ## create a scaler to get statistics for normalizing chromatin marks input
     ## also create a multiprocessing lock
     dump_data_worker_freeze = functools.partial(dump_data_webdataset_worker, 
                                                     fasta=genome_fasta, 
                                                     bigwig_files=bigwig_filelist,
                                                     target_bam=target_bam,
                                                     compress=compress,
                                                     outdir=outdir,
                                                     transforms=transforms,
                                                     DALI=DALI)
     
     count_of_digits = 0
-    while num_chunks > 0:
-       num_chunks = int(num_chunks/10)
+    nc = num_chunks
+    while nc > 0:
+       nc = int(nc/10)
        count_of_digits += 1
 
     pool = Pool(numProcessors)
     res = pool.starmap_async(dump_data_worker_freeze, zip(chunks, [outprefix + "_" + format(i, f'0{count_of_digits}d') for i in range(num_chunks)]))
     files = res.get()
     
     if braceexpand:
-        begin = f'0{count_of_digits}d'.format(0)
-        end = f'0{count_of_digits}d'.format(range(num_chunks)[-1])
-        return f"outprefix_{{{begin}...{end}}}.tar.gz" if compress else f"outprefix_{{{begin}...{end}}}.tar"
+        begin = format(0, f'0{count_of_digits}d')
+        end = format(range(num_chunks)[-1], f'0{count_of_digits}d')
+        return os.path.join(outdir, f"{outprefix}_{{{begin}..{end}}}.tar.gz" if compress else f"{outprefix}_{{{begin}...{end}}}.tar")
     else:
         return files
 
 def dump_data_webdataset_worker(coords, 
                                 outprefix, 
                                 fasta, 
                                 bigwig_files,
                                 target_bam=None, 
                                 outdir="dataset/", 
                                 compress=True,
                                 transforms=None,
                                 DALI=False):
     # get handlers
-    genome_pyfasta = pyfasta.Fasta(fasta)
+    genome_pyfaidx = pyfaidx.Fasta(fasta)
     bigwigs = [pyBigWig.open(bw) for bw in bigwig_files]
     target_pysam = pysam.AlignmentFile(target_bam) if target_bam is not None else None
 
     # iterate all records
     filename = os.path.join(outdir, f"{outprefix}.tar.gz" if compress else f"{outprefix}.tar")
     sink = wds.TarWriter(filename, compress=compress)
     for rindex, item in enumerate(coords.itertuples()):
@@ -137,15 +138,15 @@
 
         try:
             feature = utils.extract_info(
                 item.chrom,
                 item.start,
                 item.end,
                 item.label,
-                genome_pyfasta=genome_pyfasta,
+                genome_pyfaidx=genome_pyfaidx,
                 bigwigs=bigwigs,
                 target_bam=target_pysam,
                 strand=item.strand,
                 transforms=transforms,
             )
         except utils.BigWigInaccessible as e:
             continue
```

### Comparing `seqchromloader-0.5.1/seqchromloader.egg-info/PKG-INFO` & `seqchromloader-0.5.2/seqchromloader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqchromloader
-Version: 0.5.1
+Version: 0.5.2
 Summary: Sequence and chromatin dataloader for deep learning
 Home-page: https://github.com/yztxwd/seqchromloader
 Author-email: yztxwd@gmail.com
 Keywords: dataloder,pytorch,webdataset
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `seqchromloader-0.5.1/setup.py` & `seqchromloader-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     # The version of your project.
     # Usually, it would be in the form of:
     # major.minor.patch
     # eg: 1.0.0, 1.0.1, 3.0.2, 5.0-beta, etc.
     # You CANNOT upload two versions of your package with the same version number
     # This field is REQUIRED
-    version="0.5.1",
+    version="0.5.2",
 
     # The packages that constitute your project.
     # For my project, I have only one - "pydash".
     # Either you could write the name of the package, or
     # alternatively use setuptools.findpackages()
     #
     # If you only have one file, instead of a package,
@@ -33,15 +33,15 @@
     packages=find_packages(exclude='tests'),
 
     # dependencies
     install_requires=[
         'numpy',
         'pandas',
         'webdataset>=0.2.0',
-        'pyfasta>=0.5.0',
+        'pyfaidx>=0.7.0',
         'pybedtools>=0.9.0',
         'pysam>=0.19.0',
         'pybigwig>=0.3.0',
         'torch>=1.10.0',
         'pytorch-lightning',
     ],
```

