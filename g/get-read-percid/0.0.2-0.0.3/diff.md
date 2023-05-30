# Comparing `tmp/get-read-percid-0.0.2.tar.gz` & `tmp/get-read-percid-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "get-read-percid-0.0.2.tar", last modified: Mon May 29 18:59:41 2023, max compression
+gzip compressed data, was "get-read-percid-0.0.3.tar", last modified: Tue May 30 07:57:02 2023, max compression
```

## Comparing `get-read-percid-0.0.2.tar` & `get-read-percid-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 18:59:41.032050 get-read-percid-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-05-29 18:59:37.000000 get-read-percid-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      462 2023-05-29 18:59:41.032050 get-read-percid-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4117 2023-05-29 18:59:37.000000 get-read-percid-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 18:59:41.032050 get-read-percid-0.0.2/get_read_percid/
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-05-29 18:59:37.000000 get-read-percid-0.0.2/get_read_percid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5714 2023-05-29 18:59:37.000000 get-read-percid-0.0.2/get_read_percid/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-05-29 18:59:41.032050 get-read-percid-0.0.2/get_read_percid/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     2759 2023-05-29 18:59:37.000000 get-read-percid-0.0.2/get_read_percid/defaults.py
--rw-r--r--   0 runner    (1001) docker     (122)     5763 2023-05-29 18:59:37.000000 get-read-percid-0.0.2/get_read_percid/extract.py
--rw-r--r--   0 runner    (1001) docker     (122)     2972 2023-05-29 18:59:37.000000 get-read-percid-0.0.2/get_read_percid/lib.py
--rw-r--r--   0 runner    (1001) docker     (122)    11015 2023-05-29 18:59:37.000000 get-read-percid-0.0.2/get_read_percid/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 18:59:41.032050 get-read-percid-0.0.2/get_read_percid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      462 2023-05-29 18:59:41.000000 get-read-percid-0.0.2/get_read_percid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      459 2023-05-29 18:59:41.000000 get-read-percid-0.0.2/get_read_percid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 18:59:41.000000 get-read-percid-0.0.2/get_read_percid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       62 2023-05-29 18:59:41.000000 get-read-percid-0.0.2/get_read_percid.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       71 2023-05-29 18:59:41.000000 get-read-percid-0.0.2/get_read_percid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-29 18:59:41.000000 get-read-percid-0.0.2/get_read_percid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      707 2023-05-29 18:59:41.032050 get-read-percid-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      999 2023-05-29 18:59:37.000000 get-read-percid-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:57:02.421044 get-read-percid-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-05-30 07:56:56.000000 get-read-percid-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      462 2023-05-30 07:57:02.421044 get-read-percid-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4332 2023-05-30 07:56:56.000000 get-read-percid-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:57:02.421044 get-read-percid-0.0.3/get_read_percid/
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-05-30 07:56:56.000000 get-read-percid-0.0.3/get_read_percid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5714 2023-05-30 07:56:56.000000 get-read-percid-0.0.3/get_read_percid/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-05-30 07:57:02.421044 get-read-percid-0.0.3/get_read_percid/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2759 2023-05-30 07:56:56.000000 get-read-percid-0.0.3/get_read_percid/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6304 2023-05-30 07:56:56.000000 get-read-percid-0.0.3/get_read_percid/extract.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2972 2023-05-30 07:56:56.000000 get-read-percid-0.0.3/get_read_percid/lib.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11015 2023-05-30 07:56:56.000000 get-read-percid-0.0.3/get_read_percid/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-30 07:57:02.421044 get-read-percid-0.0.3/get_read_percid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      462 2023-05-30 07:57:02.000000 get-read-percid-0.0.3/get_read_percid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      459 2023-05-30 07:57:02.000000 get-read-percid-0.0.3/get_read_percid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-30 07:57:02.000000 get-read-percid-0.0.3/get_read_percid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-05-30 07:57:02.000000 get-read-percid-0.0.3/get_read_percid.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       71 2023-05-30 07:57:02.000000 get-read-percid-0.0.3/get_read_percid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-30 07:57:02.000000 get-read-percid-0.0.3/get_read_percid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      707 2023-05-30 07:57:02.421044 get-read-percid-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      999 2023-05-30 07:56:56.000000 get-read-percid-0.0.3/setup.py
```

### Comparing `get-read-percid-0.0.2/LICENSE` & `get-read-percid-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `get-read-percid-0.0.2/README.md` & `get-read-percid-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -55,27 +55,29 @@
 getRPercId will take a BAM file and/or a list in the references in a BAM file and calculate the identity to the reference. In addition, if the set of references has been listed it will be extracted in an individual BAM file. The reference file can have an extra column in case the reference name has to be renamed, i.e., we want to profile it in [anvi'o](https://anvio.org/).
 
 For a complete list of options:
 
 ```bash
 $ getRPercId --help
 
-usage: getRPercId [-h] -b FILE [-r FILE] [--prefix STR] [--sort-memory STR] [--threads INT]
-                  [--chunk-size INT] [--debug] [--version]
+usage: getRPercId [-h] -b FILE [--reference-list FILE] [--read-list FILE] [--prefix STR]
+                  [--sort-memory STR] [--threads INT] [--chunk-size INT] [--debug] [--version]
 
 A simple tool to extract references from BAM files and get read statistics
 
 options:
   -h, --help            show this help message and exit
 
 required arguments:
   -b FILE, --bam FILE   The BAM file used to generate the metaDMG results (default: None)
-  -r FILE, --reference-list FILE
+  --reference-list FILE
                         A list of references that we want to extract from the BAM file
                         (default: None)
+  --read-list FILE      A list of reads that we want to extract from the BAM file (default:
+                        None)
 
 optional arguments:
   --prefix STR          Prefix used for the output files (default: None)
   --sort-memory STR     Set maximum memory per thread for sorting; suffix K/M/G recognized
                         (default: 1G)
   --threads INT         Number of threads (default: 1)
   --chunk-size INT      Chunk size for parallel processing (default: None)
@@ -92,24 +94,25 @@
 The reference list file is a CSV file with the following format:
 
 ```bash
 $ cat ref-list.csv
 3300025461_7,c_000000000001
 ```
 
-The program will output a CSV file with the following format when using a reference list:
 
-```bash
-$ gzcat 3e3ce8e9f7___c_000000000001--percid.csv.gz | head -n 2
-M_A00706:51:HK27GDSXX:1:1342:26467:11694,99.03846153846155
-M_A00706:51:HK27GDSXX:3:2465:29243:32690,97.45222929936305
-```
-
-And a CSV file with the following format when not using a reference list:
-
-```bash
-$ gzcat 3e3ce8e9f7.percid.csv.gz | head -n 2
-M_A00706:51:HK27GDSXX:1:2134:16495:25582,3300000854_1,95.1219512195122
-M_A00706:51:HK27GDSXX:3:1640:27950:10410,3300000854_1,97.5609756097561
+For each read, the program will generate the following stats:
+- read_name
+- reference_name (if the reference list is provided)
+- read length
+- percent identity
+- %GC content
+
+One can also can provide a list of reads to extract from the BAM file. The read list file is a CSV file with the following format:
+
+```txt
+3300025461_7,M_A00706:51:HK27GDSXX:1:1101:10031:18865,c_000000000001
+3300025461_7,M_A00706:51:HK27GDSXX:1:1101:10113:5384,c_000000000001
+3300025461_7,M_A00706:51:HK27GDSXX:1:1101:10321:28573,c_000000000001
+3300025461_7,M_A00706:51:HK27GDSXX:1:1101:10484:13510,c_000000000001
 ```
 
-where the first column is the read name, the second column is the reference name, and the third column is the identity to the reference.
+Where the first column is the reference, the second column is the read name, and the third column is the new reference name we want to give. This last column is optional.
```

### Comparing `get-read-percid-0.0.2/get_read_percid/__main__.py` & `get-read-percid-0.0.3/get_read_percid/__main__.py`

 * *Files identical despite different names*

### Comparing `get-read-percid-0.0.2/get_read_percid/defaults.py` & `get-read-percid-0.0.3/get_read_percid/defaults.py`

 * *Files identical despite different names*

### Comparing `get-read-percid-0.0.2/get_read_percid/extract.py` & `get-read-percid-0.0.3/get_read_percid/extract.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,28 @@
 
 # import cProfile as profile
 # import pstats
 
 log = logging.getLogger("my_logger")
 
 
+# function to calculate GC content
+def calc_gc_content(seq):
+    """Calculate GC content of a sequence
+
+    Args:
+        seq (str): DNA sequence
+
+    Returns:
+        int: Number of GC content
+    """
+    gc = seq.count("G") + seq.count("C")
+    return gc
+
+
 def get_percid(bam, prefix=None, threads=1):
     samfile = pysam.AlignmentFile(bam, "rb", threads=threads)
     # write results to csv file
     if prefix is not None:
         ofname = f"{prefix}.percid.csv.gz"
     else:
         ofname = "sample.percid.csv.gz"
@@ -30,17 +44,19 @@
         for aln in tqdm.tqdm(
             samfile.fetch(until_eof=True),
             total=n_reads,
             desc="Processing",
             disable=is_debug(),
             unit=" reads",
         ):
+            if aln.is_unmapped:
+                continue
             ani_read = (1 - ((aln.get_tag("NM") / aln.infer_query_length()))) * 100
             f.write(
-                f"{aln.query_name},{aln.reference_name},{aln.infer_query_length()},{ani_read}\n"
+                f"{aln.query_name},{aln.reference_name},{aln.infer_query_length()},{ani_read},{calc_gc_content(aln.query_sequence)}\n"
             )
     samfile.close()
 
 
 def get_ids_and_filter(params, refs, reads, prefix, threads=1):
     bam, references = params
 
@@ -86,29 +102,33 @@
         )
 
         _open = partial(gzip.open, mode="wt") if ofname.endswith(".gz") else open
         with _open(ofname) as f:
             for aln in samfile.fetch(
                 contig=reference, multiple_iterators=False, until_eof=True
             ):
+                if aln.is_unmapped:
+                    continue
                 if reads is None:
                     ani_read = (
                         1 - ((aln.get_tag("NM") / aln.infer_query_length()))
                     ) * 100
-                    f.write(f"{aln.query_name},{aln.infer_query_length()},{ani_read}\n")
+                    f.write(
+                        f"{aln.query_name},{aln.infer_query_length()},{ani_read},{calc_gc_content(aln.query_sequence)}\n"
+                    )
                     aln.reference_id = refs_idx[ref_name]
                     out_bam_file.write(aln)
                 else:
                     if aln.query_name in reads:
                         if reads[aln.query_name] == reference:
                             ani_read = (
                                 1 - ((aln.get_tag("NM") / aln.infer_query_length()))
                             ) * 100
                             f.write(
-                                f"{aln.query_name},{aln.infer_query_length()},{ani_read}\n"
+                                f"{aln.query_name},{aln.infer_query_length()},{ani_read},{calc_gc_content(aln.query_sequence)}\n"
                             )
                             aln.reference_id = refs_idx[ref_name]
                             out_bam_file.write(aln)
         out_bam_file.close()
 
     samfile.close()
```

### Comparing `get-read-percid-0.0.2/get_read_percid/lib.py` & `get-read-percid-0.0.3/get_read_percid/lib.py`

 * *Files identical despite different names*

### Comparing `get-read-percid-0.0.2/get_read_percid/utils.py` & `get-read-percid-0.0.3/get_read_percid/utils.py`

 * *Files identical despite different names*

### Comparing `get-read-percid-0.0.2/setup.cfg` & `get-read-percid-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `get-read-percid-0.0.2/setup.py` & `get-read-percid-0.0.3/setup.py`

 * *Files identical despite different names*

