# Comparing `tmp/duplex_tools-0.3.2.tar.gz` & `tmp/duplex_tools-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/duplex_tools-0.3.2.tar", last modified: Thu Mar 16 13:03:10 2023, max compression
+gzip compressed data, was "dist/duplex_tools-0.3.3.tar", last modified: Tue May 30 14:54:11 2023, max compression
```

## Comparing `duplex_tools-0.3.2.tar` & `duplex_tools-0.3.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 13:03:10.000000 duplex_tools-0.3.2/
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-03-16 13:02:34.000000 duplex_tools-0.3.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     6841 2023-03-16 13:03:10.000000 duplex_tools-0.3.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 13:03:10.000000 duplex_tools-0.3.2/duplex_tools/
--rw-rw-rw-   0 root         (0) root         (0)    15028 2023-03-16 13:02:34.000000 duplex_tools-0.3.2/duplex_tools/split_on_adapter.py
--rw-rw-rw-   0 root         (0) root         (0)     2140 2023-03-16 13:02:34.000000 duplex_tools-0.3.2/duplex_tools/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    12786 2023-03-16 13:02:34.000000 duplex_tools-0.3.2/duplex_tools/filter_pairs.py
--rw-rw-rw-   0 root         (0) root         (0)      335 2023-03-16 13:02:34.000000 duplex_tools-0.3.2/duplex_tools/utils.py
--rwxrwxrwx   0 root         (0) root         (0)    14830 2023-03-16 13:02:34.000000 duplex_tools-0.3.2/duplex_tools/pairs_from_summary.py
--rw-rw-rw-   0 root         (0) root         (0)     7745 2023-03-16 13:02:34.000000 duplex_tools-0.3.2/duplex_tools/split_pairs_steps.py
--rw-rw-rw-   0 root         (0) root         (0)     4632 2023-03-16 13:02:34.000000 duplex_tools-0.3.2/duplex_tools/pair.py
--rw-rw-rw-   0 root         (0) root         (0)     4527 2023-03-16 13:02:34.000000 duplex_tools-0.3.2/duplex_tools/dorado_stereo.sh
--rw-rw-rw-   0 root         (0) root         (0)     4655 2023-03-16 13:02:34.000000 duplex_tools-0.3.2/duplex_tools/assess_split_on_adapter.py
--rw-rw-rw-   0 root         (0) root         (0)     4719 2023-03-16 13:02:34.000000 duplex_tools-0.3.2/duplex_tools/split_pairs.py
--rw-rw-rw-   0 root         (0) root         (0)     3363 2023-03-16 13:02:34.000000 duplex_tools-0.3.2/duplex_tools/split_pairs_utils.py
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-03-16 13:02:34.000000 duplex_tools-0.3.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-16 13:03:10.000000 duplex_tools-0.3.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-16 13:03:10.000000 duplex_tools-0.3.2/duplex_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6841 2023-03-16 13:03:10.000000 duplex_tools-0.3.2/duplex_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      638 2023-03-16 13:03:10.000000 duplex_tools-0.3.2/duplex_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-16 13:03:10.000000 duplex_tools-0.3.2/duplex_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-16 13:03:10.000000 duplex_tools-0.3.2/duplex_tools.egg-info/zip-safe
--rw-r--r--   0 root         (0) root         (0)       99 2023-03-16 13:03:10.000000 duplex_tools-0.3.2/duplex_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-03-16 13:03:10.000000 duplex_tools-0.3.2/duplex_tools.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-03-16 13:03:10.000000 duplex_tools-0.3.2/duplex_tools.egg-info/entry_points.txt
--rw-rw-rw-   0 root         (0) root         (0)    15821 2023-03-16 13:02:34.000000 duplex_tools-0.3.2/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)     2724 2023-03-16 13:02:34.000000 duplex_tools-0.3.2/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     6482 2023-03-16 13:02:34.000000 duplex_tools-0.3.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:54:11.000000 duplex_tools-0.3.3/
+-rw-rw-rw-   0 root         (0) root         (0)     2724 2023-05-30 14:34:59.000000 duplex_tools-0.3.3/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-05-30 14:34:59.000000 duplex_tools-0.3.3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 14:54:11.000000 duplex_tools-0.3.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     7152 2023-05-30 14:54:11.000000 duplex_tools-0.3.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-05-30 14:34:59.000000 duplex_tools-0.3.3/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:54:11.000000 duplex_tools-0.3.3/duplex_tools/
+-rw-rw-rw-   0 root         (0) root         (0)     2140 2023-05-30 14:34:59.000000 duplex_tools-0.3.3/duplex_tools/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    12786 2023-05-30 14:34:59.000000 duplex_tools-0.3.3/duplex_tools/filter_pairs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4655 2023-05-30 14:34:59.000000 duplex_tools-0.3.3/duplex_tools/assess_split_on_adapter.py
+-rw-rw-rw-   0 root         (0) root         (0)     7745 2023-05-30 14:34:59.000000 duplex_tools-0.3.3/duplex_tools/split_pairs_steps.py
+-rw-rw-rw-   0 root         (0) root         (0)    15028 2023-05-30 14:34:59.000000 duplex_tools-0.3.3/duplex_tools/split_on_adapter.py
+-rw-rw-rw-   0 root         (0) root         (0)      335 2023-05-30 14:34:59.000000 duplex_tools-0.3.3/duplex_tools/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4527 2023-05-30 14:34:59.000000 duplex_tools-0.3.3/duplex_tools/dorado_stereo.sh
+-rw-rw-rw-   0 root         (0) root         (0)     3363 2023-05-30 14:34:59.000000 duplex_tools-0.3.3/duplex_tools/split_pairs_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4632 2023-05-30 14:34:59.000000 duplex_tools-0.3.3/duplex_tools/pair.py
+-rw-rw-rw-   0 root         (0) root         (0)     4719 2023-05-30 14:34:59.000000 duplex_tools-0.3.3/duplex_tools/split_pairs.py
+-rwxrwxrwx   0 root         (0) root         (0)    14830 2023-05-30 14:34:59.000000 duplex_tools-0.3.3/duplex_tools/pairs_from_summary.py
+-rw-rw-rw-   0 root         (0) root         (0)    15821 2023-05-30 14:34:59.000000 duplex_tools-0.3.3/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)     6793 2023-05-30 14:34:59.000000 duplex_tools-0.3.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 14:54:11.000000 duplex_tools-0.3.3/duplex_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 14:54:11.000000 duplex_tools-0.3.3/duplex_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     7152 2023-05-30 14:54:11.000000 duplex_tools-0.3.3/duplex_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      638 2023-05-30 14:54:11.000000 duplex_tools-0.3.3/duplex_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-05-30 14:54:11.000000 duplex_tools-0.3.3/duplex_tools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       99 2023-05-30 14:54:11.000000 duplex_tools-0.3.3/duplex_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-30 14:54:11.000000 duplex_tools-0.3.3/duplex_tools.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 14:54:11.000000 duplex_tools-0.3.3/duplex_tools.egg-info/zip-safe
```

### Comparing `duplex_tools-0.3.2/PKG-INFO` & `duplex_tools-0.3.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: duplex_tools
-Version: 0.3.2
+Version: 0.3.3
 Summary: Range of tools to support operations on Duplex Sequencing read pairs.
 Home-page: https://github.com/nanoporetech/duplex-tools
 Author: ont-research
 Author-email: ont-research@nanoporetech.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 ![Oxford Nanopore Technologies logo](https://github.com/nanoporetech/medaka/raw/master/images/ONT_logo_590x106.png)
 
+> **Deprecation notice**
+> Please note that the functionality in this repository is superseded by integrated pairing in [Dorado](https://github.com/nanoporetech/dorado/tree/master/dorado).
+> This means it's no longer necessary to use pairing or dorado_stereo.sh in order to perform end-to-end duplex calling. 
+
 # Duplex Tools
 
 Duplex Tools contains a set of utilities for dealing with Duplex sequencing
 data. Tools are provided to identify and prepare duplex pairs for basecalling
 by Dorado (recommended) and Guppy, and for recovering simplex basecalls from incorrectly concatenated
 pairs.
 
@@ -66,15 +70,15 @@
 3) Duplex-basecall reads
 
 
 ### 1a) Simplex basecall with dorado
 This will create an (unmapped) .sam file which has a mapping between the signal and bases.
 `--emit-moves` allows for additional pairs to be found in step 2b.
 
-    $ dorado basecaller dna_r10.4.1_e8.2_400bps_fast@v4.0.0 pod5s/ --emit-moves > unmapped_reads_with_moves.sam
+    $ dorado basecaller dna_r10.4.1_e8.2_400bps_fast@v4.0.0 pod5s/ --emit-moves > unmapped_reads_with_moves.bam
 
 ### 2a) Find duplex pairs for Dorado stereo/basespace basecalling
 This will detect the majority of pairs and put them in the `pairs_from_bam` directory.
 
     duplex_tools pair --output_dir pairs_from_bam unmapped_reads_with_moves.bam
```

### Comparing `duplex_tools-0.3.2/duplex_tools/split_on_adapter.py` & `duplex_tools-0.3.3/duplex_tools/split_on_adapter.py`

 * *Files identical despite different names*

### Comparing `duplex_tools-0.3.2/duplex_tools/__init__.py` & `duplex_tools-0.3.3/duplex_tools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     assess_split_on_adapter, filter_pairs, pair, pairs_from_summary, \
     split_on_adapter, split_pairs  # noqa: F401
 
 modules = [
     "split_on_adapter", "assess_split_on_adapter",
     "pairs_from_summary", "filter_pairs", "pair", "split_pairs"]
 
-__version__ = '0.3.2'
+__version__ = '0.3.3'
 
 
 def main():
     """Entry point."""
     parser = ArgumentParser(
         "Duplex Sequencing Tools",
         formatter_class=ArgumentDefaultsHelpFormatter)
```

### Comparing `duplex_tools-0.3.2/duplex_tools/filter_pairs.py` & `duplex_tools-0.3.3/duplex_tools/filter_pairs.py`

 * *Files identical despite different names*

### Comparing `duplex_tools-0.3.2/duplex_tools/pairs_from_summary.py` & `duplex_tools-0.3.3/duplex_tools/pairs_from_summary.py`

 * *Files identical despite different names*

### Comparing `duplex_tools-0.3.2/duplex_tools/split_pairs_steps.py` & `duplex_tools-0.3.3/duplex_tools/split_pairs_steps.py`

 * *Files identical despite different names*

### Comparing `duplex_tools-0.3.2/duplex_tools/pair.py` & `duplex_tools-0.3.3/duplex_tools/pair.py`

 * *Files identical despite different names*

### Comparing `duplex_tools-0.3.2/duplex_tools/dorado_stereo.sh` & `duplex_tools-0.3.3/duplex_tools/dorado_stereo.sh`

 * *Files identical despite different names*

### Comparing `duplex_tools-0.3.2/duplex_tools/assess_split_on_adapter.py` & `duplex_tools-0.3.3/duplex_tools/assess_split_on_adapter.py`

 * *Files identical despite different names*

### Comparing `duplex_tools-0.3.2/duplex_tools/split_pairs.py` & `duplex_tools-0.3.3/duplex_tools/split_pairs.py`

 * *Files identical despite different names*

### Comparing `duplex_tools-0.3.2/duplex_tools/split_pairs_utils.py` & `duplex_tools-0.3.3/duplex_tools/split_pairs_utils.py`

 * *Files identical despite different names*

### Comparing `duplex_tools-0.3.2/duplex_tools.egg-info/PKG-INFO` & `duplex_tools-0.3.3/duplex_tools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: duplex-tools
-Version: 0.3.2
+Version: 0.3.3
 Summary: Range of tools to support operations on Duplex Sequencing read pairs.
 Home-page: https://github.com/nanoporetech/duplex-tools
 Author: ont-research
 Author-email: ont-research@nanoporetech.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 ![Oxford Nanopore Technologies logo](https://github.com/nanoporetech/medaka/raw/master/images/ONT_logo_590x106.png)
 
+> **Deprecation notice**
+> Please note that the functionality in this repository is superseded by integrated pairing in [Dorado](https://github.com/nanoporetech/dorado/tree/master/dorado).
+> This means it's no longer necessary to use pairing or dorado_stereo.sh in order to perform end-to-end duplex calling. 
+
 # Duplex Tools
 
 Duplex Tools contains a set of utilities for dealing with Duplex sequencing
 data. Tools are provided to identify and prepare duplex pairs for basecalling
 by Dorado (recommended) and Guppy, and for recovering simplex basecalls from incorrectly concatenated
 pairs.
 
@@ -66,15 +70,15 @@
 3) Duplex-basecall reads
 
 
 ### 1a) Simplex basecall with dorado
 This will create an (unmapped) .sam file which has a mapping between the signal and bases.
 `--emit-moves` allows for additional pairs to be found in step 2b.
 
-    $ dorado basecaller dna_r10.4.1_e8.2_400bps_fast@v4.0.0 pod5s/ --emit-moves > unmapped_reads_with_moves.sam
+    $ dorado basecaller dna_r10.4.1_e8.2_400bps_fast@v4.0.0 pod5s/ --emit-moves > unmapped_reads_with_moves.bam
 
 ### 2a) Find duplex pairs for Dorado stereo/basespace basecalling
 This will detect the majority of pairs and put them in the `pairs_from_bam` directory.
 
     duplex_tools pair --output_dir pairs_from_bam unmapped_reads_with_moves.bam
```

### Comparing `duplex_tools-0.3.2/duplex_tools.egg-info/SOURCES.txt` & `duplex_tools-0.3.3/duplex_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duplex_tools-0.3.2/LICENSE.md` & `duplex_tools-0.3.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `duplex_tools-0.3.2/setup.py` & `duplex_tools-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `duplex_tools-0.3.2/README.md` & `duplex_tools-0.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 ![Oxford Nanopore Technologies logo](https://github.com/nanoporetech/medaka/raw/master/images/ONT_logo_590x106.png)
 
+> **Deprecation notice**
+> Please note that the functionality in this repository is superseded by integrated pairing in [Dorado](https://github.com/nanoporetech/dorado/tree/master/dorado).
+> This means it's no longer necessary to use pairing or dorado_stereo.sh in order to perform end-to-end duplex calling. 
+
 # Duplex Tools
 
 Duplex Tools contains a set of utilities for dealing with Duplex sequencing
 data. Tools are provided to identify and prepare duplex pairs for basecalling
 by Dorado (recommended) and Guppy, and for recovering simplex basecalls from incorrectly concatenated
 pairs.
 
@@ -54,15 +58,15 @@
 3) Duplex-basecall reads
 
 
 ### 1a) Simplex basecall with dorado
 This will create an (unmapped) .sam file which has a mapping between the signal and bases.
 `--emit-moves` allows for additional pairs to be found in step 2b.
 
-    $ dorado basecaller dna_r10.4.1_e8.2_400bps_fast@v4.0.0 pod5s/ --emit-moves > unmapped_reads_with_moves.sam
+    $ dorado basecaller dna_r10.4.1_e8.2_400bps_fast@v4.0.0 pod5s/ --emit-moves > unmapped_reads_with_moves.bam
 
 ### 2a) Find duplex pairs for Dorado stereo/basespace basecalling
 This will detect the majority of pairs and put them in the `pairs_from_bam` directory.
 
     duplex_tools pair --output_dir pairs_from_bam unmapped_reads_with_moves.bam
```

