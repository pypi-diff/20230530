# Comparing `tmp/splicekit-0.4.1.tar.gz` & `tmp/splicekit-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splicekit-0.4.1.tar", last modified: Thu May 25 13:35:43 2023, max compression
+gzip compressed data, was "splicekit-0.4.2.tar", last modified: Tue May 30 11:38:25 2023, max compression
```

## Comparing `splicekit-0.4.1.tar` & `splicekit-0.4.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-05-25 13:35:43.224312 splicekit-0.4.1/
--rw-rw-r--   0 rotg     (2023757) games       (20)    22853 2023-05-25 13:35:43.223908 splicekit-0.4.1/PKG-INFO
--rwxrwxr-x   0 rotg     (2023757) games       (20)    22455 2023-05-25 12:17:55.000000 splicekit-0.4.1/README.md
--rw-rw-r--   0 rotg     (2023757) games       (20)       38 2023-05-25 13:35:43.224407 splicekit-0.4.1/setup.cfg
--rw-rw-r--   0 rotg     (2023757) games       (20)     1133 2023-05-25 08:08:20.000000 splicekit-0.4.1/setup.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-05-25 13:35:43.197347 splicekit-0.4.1/splicekit/
--rw-rw-r--   0 rotg     (2023757) games       (20)    13777 2023-05-25 11:18:48.000000 splicekit-0.4.1/splicekit/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-05-25 13:35:43.203411 splicekit-0.4.1/splicekit/clusterlogfc/
--rw-rw-r--   0 rotg     (2023757) games       (20)     5584 2023-05-05 11:49:03.000000 splicekit-0.4.1/splicekit/clusterlogfc/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-05-25 13:35:43.204685 splicekit-0.4.1/splicekit/config/
--rw-rw-r--   0 rotg     (2023757) games       (20)      850 2023-05-25 11:18:03.000000 splicekit-0.4.1/splicekit/config/__init__.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-05-25 13:35:43.221284 splicekit-0.4.1/splicekit/core/
--rw-rw-r--   0 rotg     (2023757) games       (20)      396 2023-01-31 12:27:24.000000 splicekit-0.4.1/splicekit/core/__init__.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     6667 2023-05-05 06:13:11.000000 splicekit-0.4.1/splicekit/core/anchors.py
--rw-rw-r--   0 rotg     (2023757) games       (20)    16752 2023-05-24 07:18:50.000000 splicekit-0.4.1/splicekit/core/annotation.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     3988 2023-01-31 12:27:24.000000 splicekit-0.4.1/splicekit/core/delta_dar.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     5407 2023-05-05 08:10:13.000000 splicekit-0.4.1/splicekit/core/exons.py
--rwxrwxr-x   0 rotg     (2023757) games       (20)    29902 2023-05-03 08:24:07.000000 splicekit-0.4.1/splicekit/core/features.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     5662 2023-05-05 06:13:26.000000 splicekit-0.4.1/splicekit/core/genes.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1061 2023-05-25 11:01:47.000000 splicekit-0.4.1/splicekit/core/jbrowse2.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     8871 2023-05-25 12:51:52.000000 splicekit-0.4.1/splicekit/core/jbrowse2_create.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     2948 2023-04-26 12:12:45.000000 splicekit-0.4.1/splicekit/core/juan.py
--rw-rw-r--   0 rotg     (2023757) games       (20)    18195 2023-05-02 17:27:43.000000 splicekit-0.4.1/splicekit/core/junctions.py
--rw-rw-r--   0 rotg     (2023757) games       (20)    37713 2023-05-04 06:56:59.000000 splicekit-0.4.1/splicekit/core/motifs.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     1663 2023-05-02 18:35:35.000000 splicekit-0.4.1/splicekit/core/patterns.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     2420 2023-05-03 10:54:22.000000 splicekit-0.4.1/splicekit/core/promisc.py
--rw-rw-r--   0 rotg     (2023757) games       (20)     9045 2023-05-03 09:57:04.000000 splicekit-0.4.1/splicekit/core/report.py
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-05-25 13:35:43.222361 splicekit-0.4.1/splicekit/judge/
--rw-rw-r--   0 rotg     (2023757) games       (20)    26830 2023-05-02 18:05:54.000000 splicekit-0.4.1/splicekit/judge/__init__.py
--rwxrwxr-x   0 rotg     (2023757) games       (20)     5402 2023-05-05 10:18:19.000000 splicekit-0.4.1/splicekit/splicecompare
--rwxrwxr-x   0 rotg     (2023757) games       (20)     4810 2023-05-25 12:10:42.000000 splicekit-0.4.1/splicekit/splicekit
--rw-rw-r--   0 rotg     (2023757) games       (20)     1670 2023-05-24 07:25:57.000000 splicekit-0.4.1/splicekit/splicekit.config.template
--rw-rw-r--   0 rotg     (2023757) games       (20)        6 2023-05-25 13:35:31.000000 splicekit-0.4.1/splicekit/version
-drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-05-25 13:35:43.202613 splicekit-0.4.1/splicekit.egg-info/
--rw-rw-r--   0 rotg     (2023757) games       (20)    22853 2023-05-25 13:35:42.000000 splicekit-0.4.1/splicekit.egg-info/PKG-INFO
--rw-rw-r--   0 rotg     (2023757) games       (20)      826 2023-05-25 13:35:42.000000 splicekit-0.4.1/splicekit.egg-info/SOURCES.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-05-25 13:35:42.000000 splicekit-0.4.1/splicekit.egg-info/dependency_links.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-05-09 07:35:55.000000 splicekit-0.4.1/splicekit.egg-info/not-zip-safe
--rw-rw-r--   0 rotg     (2023757) games       (20)       62 2023-05-25 13:35:42.000000 splicekit-0.4.1/splicekit.egg-info/requires.txt
--rw-rw-r--   0 rotg     (2023757) games       (20)       10 2023-05-25 13:35:42.000000 splicekit-0.4.1/splicekit.egg-info/top_level.txt
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-05-30 11:38:25.387109 splicekit-0.4.2/
+-rw-rw-r--   0 rotg     (2023757) games       (20)    22857 2023-05-30 11:38:25.386836 splicekit-0.4.2/PKG-INFO
+-rwxrwxr-x   0 rotg     (2023757) games       (20)    22459 2023-05-30 11:36:14.000000 splicekit-0.4.2/README.md
+-rw-rw-r--   0 rotg     (2023757) games       (20)       38 2023-05-30 11:38:25.387203 splicekit-0.4.2/setup.cfg
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1133 2023-05-25 08:08:20.000000 splicekit-0.4.2/setup.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-05-30 11:38:25.371393 splicekit-0.4.2/splicekit/
+-rw-rw-r--   0 rotg     (2023757) games       (20)    13778 2023-05-30 11:37:41.000000 splicekit-0.4.2/splicekit/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-05-30 11:38:25.375309 splicekit-0.4.2/splicekit/clusterlogfc/
+-rw-rw-r--   0 rotg     (2023757) games       (20)     5584 2023-05-05 11:49:03.000000 splicekit-0.4.2/splicekit/clusterlogfc/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-05-30 11:38:25.376013 splicekit-0.4.2/splicekit/config/
+-rw-rw-r--   0 rotg     (2023757) games       (20)      850 2023-05-25 11:18:03.000000 splicekit-0.4.2/splicekit/config/__init__.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-05-30 11:38:25.385656 splicekit-0.4.2/splicekit/core/
+-rw-rw-r--   0 rotg     (2023757) games       (20)      396 2023-01-31 12:27:24.000000 splicekit-0.4.2/splicekit/core/__init__.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     6667 2023-05-05 06:13:11.000000 splicekit-0.4.2/splicekit/core/anchors.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)    16752 2023-05-24 07:18:50.000000 splicekit-0.4.2/splicekit/core/annotation.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     3988 2023-01-31 12:27:24.000000 splicekit-0.4.2/splicekit/core/delta_dar.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     5407 2023-05-05 08:10:13.000000 splicekit-0.4.2/splicekit/core/exons.py
+-rwxrwxr-x   0 rotg     (2023757) games       (20)    29902 2023-05-03 08:24:07.000000 splicekit-0.4.2/splicekit/core/features.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     5662 2023-05-05 06:13:26.000000 splicekit-0.4.2/splicekit/core/genes.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1061 2023-05-25 11:01:47.000000 splicekit-0.4.2/splicekit/core/jbrowse2.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     8872 2023-05-30 11:34:53.000000 splicekit-0.4.2/splicekit/core/jbrowse2_create.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     2948 2023-04-26 12:12:45.000000 splicekit-0.4.2/splicekit/core/juan.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)    18195 2023-05-02 17:27:43.000000 splicekit-0.4.2/splicekit/core/junctions.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)    37713 2023-05-04 06:56:59.000000 splicekit-0.4.2/splicekit/core/motifs.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1663 2023-05-02 18:35:35.000000 splicekit-0.4.2/splicekit/core/patterns.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     2420 2023-05-03 10:54:22.000000 splicekit-0.4.2/splicekit/core/promisc.py
+-rw-rw-r--   0 rotg     (2023757) games       (20)     9045 2023-05-03 09:57:04.000000 splicekit-0.4.2/splicekit/core/report.py
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-05-30 11:38:25.386260 splicekit-0.4.2/splicekit/judge/
+-rw-rw-r--   0 rotg     (2023757) games       (20)    26830 2023-05-02 18:05:54.000000 splicekit-0.4.2/splicekit/judge/__init__.py
+-rwxrwxr-x   0 rotg     (2023757) games       (20)     5402 2023-05-05 10:18:19.000000 splicekit-0.4.2/splicekit/splicecompare
+-rwxrwxr-x   0 rotg     (2023757) games       (20)     4750 2023-05-30 11:35:14.000000 splicekit-0.4.2/splicekit/splicekit
+-rw-rw-r--   0 rotg     (2023757) games       (20)     1670 2023-05-24 07:25:57.000000 splicekit-0.4.2/splicekit/splicekit.config.template
+-rw-rw-r--   0 rotg     (2023757) games       (20)        6 2023-05-30 11:38:19.000000 splicekit-0.4.2/splicekit/version
+drwxrwxr-x   0 rotg     (2023757) games       (20)        0 2023-05-30 11:38:25.374887 splicekit-0.4.2/splicekit.egg-info/
+-rw-rw-r--   0 rotg     (2023757) games       (20)    22857 2023-05-30 11:38:25.372121 splicekit-0.4.2/splicekit.egg-info/PKG-INFO
+-rw-rw-r--   0 rotg     (2023757) games       (20)      826 2023-05-30 11:38:25.373141 splicekit-0.4.2/splicekit.egg-info/SOURCES.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-05-30 11:38:25.373461 splicekit-0.4.2/splicekit.egg-info/dependency_links.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)        1 2023-05-09 07:35:55.000000 splicekit-0.4.2/splicekit.egg-info/not-zip-safe
+-rw-rw-r--   0 rotg     (2023757) games       (20)       62 2023-05-30 11:38:25.374645 splicekit-0.4.2/splicekit.egg-info/requires.txt
+-rw-rw-r--   0 rotg     (2023757) games       (20)       10 2023-05-30 11:38:25.374963 splicekit-0.4.2/splicekit.egg-info/top_level.txt
```

### Comparing `splicekit-0.4.1/PKG-INFO` & `splicekit-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splicekit
-Version: 0.4.1
+Version: 0.4.2
 Summary: splicekit: comprehensive toolkit for splicing analysis from short-read RNA-seq
 Home-page: https://github.com/bedapub/splicekit
 Author: Roche, PMDA Spliceosome team
 Author-email: gregor.rot@gmail.com
 Keywords: splicekit,splicing,transcriptomics,bioinformatics
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -14,15 +14,15 @@
 
 [What does splicekit do?](#what_do)<br>
 [Changelog](#changelog)<br>
 [Quick start and installation](#initial_setup)<br>
 [Running Splicekit](#running_splicekit)<br>
 &nbsp;&nbsp;[Annotation and comparisons](#annot_comp)<br>
 &nbsp;&nbsp;[Preparing feature (genes, exon, junction, anchor) data tables](#make_tables)<br>
-&nbsp;&nbsp;[Running edgeR gene context analysis on junction features](#run_edgeR)<br>
+&nbsp;&nbsp;[Running edgeR gene context analysis on junction features](#id_features)<br>
 [Motif analysis](#motif)<br>
 [Scanning for RNA-protein binding with scanRBP](#scanRBP)<br>
 [juDGE plots](#judgeplot)<br>
 [Jbrowse2 visualizations](#jbrowse)<br>
 [Documentation and specifications](#filedescriptors)<br>
 
 <b>splicekit</b> is a modular platform for splicing analysis of RNA-seq datasets. The platform also integrates an JBrowse2 instance together with [pybio](https://github.com/grexor/pybio) for genomic operations and [scanRBP](https://github.com/grexor/scanRBP) for RNA-protein binding studies. The whole analysis is self-contained (one single folder) and the platform is written in Python, in a modular way.
@@ -253,15 +253,15 @@
 
 | GeneID | Start | End | Length | Symbol | 1_test | 2_test | 3_test | 4_control | 5_control | 6_control |
 |-|-|-|-|-|-|-|-|-|-|-|
 | 1 | 58347029 | 58347353 | 325 | A1BG | 42 | 31 | 109 | 75 | 86 | 33 |
 | 1 | 58347640 | 58350370 | 2731 | A1BG | 0 | 0 | 3 | 1 | 0 | 0 | 0 |
 | 1 | 58350651 | 58351391 | 741 | A1BG | 0 | 0 | 10 | 1 | 0 | 0	| 3 |
 
-## Running edgeR gene context analysis on junction features <a name="run_edgeR"></a>
+## Running edgeR gene context analysis on junction features <a name="id_features"></a>
 
 Running edgeR analysis on features (either genes, exons, junctions or anchors) consist of simply running the process script or submitting all matching job files to the cluster. This is done by the `splicekit edgeR` command.
 
 Results are stored in the files `results/results_edgeR_{feature_type}` where feature_type is one of ["genes", "exons", "junctions", "donor_anochors", "acceptor_anchors"]. Results with FDR < `splicekit.config.edgeR_FDR_thr` are reported (sorted by FDR), linked to JBrowse with URL links.
 
 ## Motif analysis <a name="motif"></a>
```

### Comparing `splicekit-0.4.1/README.md` & `splicekit-0.4.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [What does splicekit do?](#what_do)<br>
 [Changelog](#changelog)<br>
 [Quick start and installation](#initial_setup)<br>
 [Running Splicekit](#running_splicekit)<br>
 &nbsp;&nbsp;[Annotation and comparisons](#annot_comp)<br>
 &nbsp;&nbsp;[Preparing feature (genes, exon, junction, anchor) data tables](#make_tables)<br>
-&nbsp;&nbsp;[Running edgeR gene context analysis on junction features](#run_edgeR)<br>
+&nbsp;&nbsp;[Running edgeR gene context analysis on junction features](#id_features)<br>
 [Motif analysis](#motif)<br>
 [Scanning for RNA-protein binding with scanRBP](#scanRBP)<br>
 [juDGE plots](#judgeplot)<br>
 [Jbrowse2 visualizations](#jbrowse)<br>
 [Documentation and specifications](#filedescriptors)<br>
 
 <b>splicekit</b> is a modular platform for splicing analysis of RNA-seq datasets. The platform also integrates an JBrowse2 instance together with [pybio](https://github.com/grexor/pybio) for genomic operations and [scanRBP](https://github.com/grexor/scanRBP) for RNA-protein binding studies. The whole analysis is self-contained (one single folder) and the platform is written in Python, in a modular way.
@@ -243,15 +243,15 @@
 
 | GeneID | Start | End | Length | Symbol | 1_test | 2_test | 3_test | 4_control | 5_control | 6_control |
 |-|-|-|-|-|-|-|-|-|-|-|
 | 1 | 58347029 | 58347353 | 325 | A1BG | 42 | 31 | 109 | 75 | 86 | 33 |
 | 1 | 58347640 | 58350370 | 2731 | A1BG | 0 | 0 | 3 | 1 | 0 | 0 | 0 |
 | 1 | 58350651 | 58351391 | 741 | A1BG | 0 | 0 | 10 | 1 | 0 | 0	| 3 |
 
-## Running edgeR gene context analysis on junction features <a name="run_edgeR"></a>
+## Running edgeR gene context analysis on junction features <a name="id_features"></a>
 
 Running edgeR analysis on features (either genes, exons, junctions or anchors) consist of simply running the process script or submitting all matching job files to the cluster. This is done by the `splicekit edgeR` command.
 
 Results are stored in the files `results/results_edgeR_{feature_type}` where feature_type is one of ["genes", "exons", "junctions", "donor_anochors", "acceptor_anchors"]. Results with FDR < `splicekit.config.edgeR_FDR_thr` are reported (sorted by FDR), linked to JBrowse with URL links.
 
 ## Motif analysis <a name="motif"></a>
```

### Comparing `splicekit-0.4.1/setup.py` & `splicekit-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.1/splicekit/__init__.py` & `splicekit-0.4.2/splicekit/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -235,8 +235,8 @@
     annotation()
     features()
     edgeR()
     juan()
     motifs()
     promisc()
     judge_process()
-    clusterlogfc_process()
+    clusterlogfc_process()
```

### Comparing `splicekit-0.4.1/splicekit/clusterlogfc/__init__.py` & `splicekit-0.4.2/splicekit/clusterlogfc/__init__.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.1/splicekit/config/__init__.py` & `splicekit-0.4.2/splicekit/config/__init__.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.1/splicekit/core/anchors.py` & `splicekit-0.4.2/splicekit/core/anchors.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.1/splicekit/core/annotation.py` & `splicekit-0.4.2/splicekit/core/annotation.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.1/splicekit/core/delta_dar.py` & `splicekit-0.4.2/splicekit/core/delta_dar.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.1/splicekit/core/exons.py` & `splicekit-0.4.2/splicekit/core/exons.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.1/splicekit/core/features.py` & `splicekit-0.4.2/splicekit/core/features.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.1/splicekit/core/genes.py` & `splicekit-0.4.2/splicekit/core/genes.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.1/splicekit/core/jbrowse2.py` & `splicekit-0.4.2/splicekit/core/jbrowse2.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.1/splicekit/core/jbrowse2_create.py` & `splicekit-0.4.2/splicekit/core/jbrowse2_create.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
                                         bam_fname=bam_fname,cram_fname=cram_fname, bigwig_fname=bigwig_fname, genome_fa=genome_fa)
             fout.write(job_bw_out)
             fout.close()        
             job_sh_bw_out = job_sh_bw.format(container=container, sample=sample, bamCoverage_binSize=bamCoverage_binSize,
                                             bam_fname=bam_fname,cram_fname=cram_fname, bigwig_fname=bigwig_fname, genome_fa=genome_fa)
             fsh.write(job_sh_bw_out)
         else:
-            print('[jbrowse] sample {sample} already processed (.bw and .cram in results/results_jbrowse) --> use "splicekit jbrowse2_create samples -force" to overwrite')
+            print(f'[jbrowse] sample {sample} already processed (.bw and .cram in results/results_jbrowse) --> use "splicekit jbrowse2_create samples -force" to overwrite')
     fsh.close()
 
 def create_jbrowse_config(force_annotation):
     ''' We need to add reference genome, samples files and genome annotation to jbrowse's config.json and create it first'''
     if not os.path.exists('jbrowse2/splicekit_data'):
         os.system('mkdir jbrowse2/splicekit_data') # first create folder to put everything inside
```

### Comparing `splicekit-0.4.1/splicekit/core/juan.py` & `splicekit-0.4.2/splicekit/core/juan.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.1/splicekit/core/junctions.py` & `splicekit-0.4.2/splicekit/core/junctions.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.1/splicekit/core/motifs.py` & `splicekit-0.4.2/splicekit/core/motifs.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.1/splicekit/core/patterns.py` & `splicekit-0.4.2/splicekit/core/patterns.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.1/splicekit/core/promisc.py` & `splicekit-0.4.2/splicekit/core/promisc.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.1/splicekit/core/report.py` & `splicekit-0.4.2/splicekit/core/report.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.1/splicekit/judge/__init__.py` & `splicekit-0.4.2/splicekit/judge/__init__.py`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.1/splicekit/splicecompare` & `splicekit-0.4.2/splicekit/splicecompare`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.1/splicekit/splicekit` & `splicekit-0.4.2/splicekit/splicekit`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,15 @@
      promisc           promiscuity analysis: genes and their junctions changes across conditions
      clusterlogfc      log fold-change clusters of significant changes (FDR<0.05) on junction, exon, gene level
 
   -- scanRBP, motif and sequence analyses
      motifs            run motif and scanRBP analysis
 
   -- JBrowse2 genomic browser
-     jbrowse2_create   creates all required JBrowse2 files
-     jbrowse2          starts JBrowse2 web server
+     jbrowse2          creates all required JBrowse2 files and starts JBrowse2 web server
      
 """
 
 help_edgeR = """
 Usage: splicekit edgeR [sub-command]
 
 Sub-commands:
@@ -121,20 +120,19 @@
     splicekit.clusterlogfc_process()
 elif args.command[0]=="process":
     splicekit.process()
 elif args.command[0]=="judge":
     splicekit.judge_process()
 elif args.command[0]=="juan":
     splicekit.juan()
-elif args.command [0] == "jbrowse2_create":
+elif args.command [0] == "jbrowse2":
     force_samples=False; force_annotation = False
     if len(args.command)>1 and args.command[1] == 'samples':
         force_samples=args.force
     if len(args.command)>1 and args.command[1] == 'annotation':
         force_annotation=args.force
     if len(args.command)==1:
         force_annotation = args.force; force_samples = args.force
     splicekit.jbrowse2_create(force_samples=force_samples,force_annotation=force_annotation)
-elif args.command[0]=="jbrowse2":
     splicekit.core.jbrowse2.process()
 else:
     print(help_0)
```

### Comparing `splicekit-0.4.1/splicekit/splicekit.config.template` & `splicekit-0.4.2/splicekit/splicekit.config.template`

 * *Files identical despite different names*

### Comparing `splicekit-0.4.1/splicekit.egg-info/PKG-INFO` & `splicekit-0.4.2/splicekit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splicekit
-Version: 0.4.1
+Version: 0.4.2
 Summary: splicekit: comprehensive toolkit for splicing analysis from short-read RNA-seq
 Home-page: https://github.com/bedapub/splicekit
 Author: Roche, PMDA Spliceosome team
 Author-email: gregor.rot@gmail.com
 Keywords: splicekit,splicing,transcriptomics,bioinformatics
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -14,15 +14,15 @@
 
 [What does splicekit do?](#what_do)<br>
 [Changelog](#changelog)<br>
 [Quick start and installation](#initial_setup)<br>
 [Running Splicekit](#running_splicekit)<br>
 &nbsp;&nbsp;[Annotation and comparisons](#annot_comp)<br>
 &nbsp;&nbsp;[Preparing feature (genes, exon, junction, anchor) data tables](#make_tables)<br>
-&nbsp;&nbsp;[Running edgeR gene context analysis on junction features](#run_edgeR)<br>
+&nbsp;&nbsp;[Running edgeR gene context analysis on junction features](#id_features)<br>
 [Motif analysis](#motif)<br>
 [Scanning for RNA-protein binding with scanRBP](#scanRBP)<br>
 [juDGE plots](#judgeplot)<br>
 [Jbrowse2 visualizations](#jbrowse)<br>
 [Documentation and specifications](#filedescriptors)<br>
 
 <b>splicekit</b> is a modular platform for splicing analysis of RNA-seq datasets. The platform also integrates an JBrowse2 instance together with [pybio](https://github.com/grexor/pybio) for genomic operations and [scanRBP](https://github.com/grexor/scanRBP) for RNA-protein binding studies. The whole analysis is self-contained (one single folder) and the platform is written in Python, in a modular way.
@@ -253,15 +253,15 @@
 
 | GeneID | Start | End | Length | Symbol | 1_test | 2_test | 3_test | 4_control | 5_control | 6_control |
 |-|-|-|-|-|-|-|-|-|-|-|
 | 1 | 58347029 | 58347353 | 325 | A1BG | 42 | 31 | 109 | 75 | 86 | 33 |
 | 1 | 58347640 | 58350370 | 2731 | A1BG | 0 | 0 | 3 | 1 | 0 | 0 | 0 |
 | 1 | 58350651 | 58351391 | 741 | A1BG | 0 | 0 | 10 | 1 | 0 | 0	| 3 |
 
-## Running edgeR gene context analysis on junction features <a name="run_edgeR"></a>
+## Running edgeR gene context analysis on junction features <a name="id_features"></a>
 
 Running edgeR analysis on features (either genes, exons, junctions or anchors) consist of simply running the process script or submitting all matching job files to the cluster. This is done by the `splicekit edgeR` command.
 
 Results are stored in the files `results/results_edgeR_{feature_type}` where feature_type is one of ["genes", "exons", "junctions", "donor_anochors", "acceptor_anchors"]. Results with FDR < `splicekit.config.edgeR_FDR_thr` are reported (sorted by FDR), linked to JBrowse with URL links.
 
 ## Motif analysis <a name="motif"></a>
```

### Comparing `splicekit-0.4.1/splicekit.egg-info/SOURCES.txt` & `splicekit-0.4.2/splicekit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

