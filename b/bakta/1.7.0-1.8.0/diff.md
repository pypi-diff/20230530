# Comparing `tmp/bakta-1.7.0.tar.gz` & `tmp/bakta-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bakta-1.7.0.tar", last modified: Fri Feb 24 15:19:20 2023, max compression
+gzip compressed data, was "bakta-1.8.0.tar", last modified: Tue May 30 14:58:34 2023, max compression
```

## Comparing `bakta-1.7.0.tar` & `bakta-1.8.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 15:19:20.096587 bakta-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-02-24 15:19:09.000000 bakta-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    47148 2023-02-24 15:19:20.096587 bakta-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    39707 2023-02-24 15:19:09.000000 bakta-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 15:19:20.084587 bakta-1.7.0/bakta/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14534 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    18456 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 15:19:20.088587 bakta-1.7.0/bakta/expert/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/expert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/expert/amrfinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/expert/protein_sequences.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 15:19:20.092587 bakta-1.7.0/bakta/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33473 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/features/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)    43977 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/features/cds.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/features/crispr.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/features/gaps.py
--rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/features/nc_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/features/nc_rna_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/features/orf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/features/ori.py
--rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/features/r_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)    16748 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/features/s_orf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/features/signal_peptides.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/features/t_rna.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/features/tm_rna.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 15:19:20.096587 bakta-1.7.0/bakta/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/io/fasta.py
--rw-r--r--   0 runner    (1001) docker     (123)    20439 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/io/gff.py
--rw-r--r--   0 runner    (1001) docker     (123)    19763 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/io/insdc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/io/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/io/tsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/ips.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29598 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    20147 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    10180 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/proteins.py
--rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/psc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/pscc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/so.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/ups.py
--rw-r--r--   0 runner    (1001) docker     (123)    28104 2023-02-24 15:19:09.000000 bakta-1.7.0/bakta/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 15:19:20.084587 bakta-1.7.0/bakta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    47148 2023-02-24 15:19:19.000000 bakta-1.7.0/bakta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-02-24 15:19:20.000000 bakta-1.7.0/bakta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 15:19:19.000000 bakta-1.7.0/bakta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-02-24 15:19:19.000000 bakta-1.7.0/bakta.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 15:19:19.000000 bakta-1.7.0/bakta.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-02-24 15:19:19.000000 bakta-1.7.0/bakta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-24 15:19:19.000000 bakta-1.7.0/bakta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 15:19:20.096587 bakta-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-02-24 15:19:09.000000 bakta-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 15:19:20.096587 bakta-1.7.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)    18485 2023-02-24 15:19:09.000000 bakta-1.7.0/test/test_args.py
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-02-24 15:19:09.000000 bakta-1.7.0/test/test_bakta.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-02-24 15:19:09.000000 bakta-1.7.0/test/test_bakta_proteins.py
--rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-02-24 15:19:09.000000 bakta-1.7.0/test/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-02-24 15:19:09.000000 bakta-1.7.0/test/test_edge_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-02-24 15:19:09.000000 bakta-1.7.0/test/test_nt_sequences.py
--rw-r--r--   0 runner    (1001) docker     (123)    13022 2023-02-24 15:19:09.000000 bakta-1.7.0/test/test_pseudo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-02-24 15:19:09.000000 bakta-1.7.0/test/test_sORF.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-02-24 15:19:09.000000 bakta-1.7.0/test/test_sig_peps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-02-24 15:19:09.000000 bakta-1.7.0/test/test_user_proteins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:34.019009 bakta-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-30 14:58:23.000000 bakta-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    47858 2023-05-30 14:58:34.019009 bakta-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    40267 2023-05-30 14:58:23.000000 bakta-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:34.015009 bakta-1.8.0/bakta/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15981 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:34.015009 bakta-1.8.0/bakta/expert/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/expert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/expert/amrfinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9134 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/expert/protein_sequences.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:34.019009 bakta-1.8.0/bakta/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33942 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/features/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43977 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/features/cds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/features/crispr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/features/gaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/features/nc_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/features/nc_rna_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/features/orf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/features/ori.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/features/r_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16748 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/features/s_orf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/features/signal_peptides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/features/t_rna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/features/tm_rna.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:34.019009 bakta-1.8.0/bakta/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/io/fasta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20462 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/io/gff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19547 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/io/insdc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/io/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/io/tsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/ips.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29754 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20401 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11516 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/proteins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/psc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/pscc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/so.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/ups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27984 2023-05-30 14:58:23.000000 bakta-1.8.0/bakta/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:34.015009 bakta-1.8.0/bakta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    47858 2023-05-30 14:58:33.000000 bakta-1.8.0/bakta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-30 14:58:33.000000 bakta-1.8.0/bakta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:58:33.000000 bakta-1.8.0/bakta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-30 14:58:33.000000 bakta-1.8.0/bakta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:58:33.000000 bakta-1.8.0/bakta.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-30 14:58:33.000000 bakta-1.8.0/bakta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 14:58:33.000000 bakta-1.8.0/bakta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 14:58:34.019009 bakta-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-30 14:58:23.000000 bakta-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:58:34.019009 bakta-1.8.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    20648 2023-05-30 14:58:23.000000 bakta-1.8.0/test/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-05-30 14:58:23.000000 bakta-1.8.0/test/test_bakta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-30 14:58:23.000000 bakta-1.8.0/test/test_bakta_proteins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7742 2023-05-30 14:58:23.000000 bakta-1.8.0/test/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-30 14:58:23.000000 bakta-1.8.0/test/test_edge_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-30 14:58:23.000000 bakta-1.8.0/test/test_nt_sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13022 2023-05-30 14:58:23.000000 bakta-1.8.0/test/test_pseudo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-30 14:58:23.000000 bakta-1.8.0/test/test_sORF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-30 14:58:23.000000 bakta-1.8.0/test/test_sig_peps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-05-30 14:58:23.000000 bakta-1.8.0/test/test_user_proteins.py
```

### Comparing `bakta-1.7.0/LICENSE` & `bakta-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bakta-1.7.0/PKG-INFO` & `bakta-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bakta
-Version: 1.7.0
+Version: 1.8.0
 Summary: Bakta: rapid & standardized annotation of bacterial genomes, MAGs & plasmids
 Home-page: https://github.com/oschwengers/bakta
 Author: Oliver Schwengers
 Author-email: oliver.schwengers@computational.bio.uni-giessen.de
 License: GPLv3
 Project-URL: Documentation, https://bakta.readthedocs.io
 Project-URL: Source, https://github.com/oschwengers/bakta
@@ -51,15 +51,15 @@
         - **Fast**
         This AFSI approach substantially accellerates the annotation process by avoiding computationally expensive homology searches for identified genes. Thus, Bakta can annotate a typical bacterial genome in 10 &plusmn;5 min on a laptop, plasmids in a couple of seconds/minutes.
         
         - **Database cross-references**
         Fostering the [FAIR](https://www.go-fair.org/fair-principles) principles, Bakta exploits its AFSI approach to annotate CDS with database cross-references (**dbxref**) to RefSeq (`WP_*`), UniRef100 (`UniRef100_*`) and UniParc (`UPI*`). By doing so, IPS allow the surveillance of distinct gene alleles and streamlining comparative analysis as well as posterior (external) annotations of `putative` & `hypothetical` protein sequences which can be mapped back to existing CDS via these exact & stable identifiers (*E. coli* gene [ymiA](https://www.uniprot.org/uniprot/P0CB62) [...more](https://www.uniprot.org/help/dubious_sequences)). Currently, Bakta identifies ~214.8 mio, ~199 mio and ~161 mio distinct protein sequences from UniParc, UniRef100 and RefSeq, respectively. Hence, for certain genomes, up to 99 % of all CDS can be identified this way, skipping computationally expensive sequence alignments.
         
         - **FAIR annotations**
-        To provide standardized annotations adhearing to FAIR principles, Bakta utilizes a versioned custom annotation database comprising UniProt's [UniRef100 & UniRef90](https://www.uniprot.org/uniref/) protein clusters (FAIR -> [DOI](http://dx.doi.org/10.1038/s41597-019-0180-9)/[DOI](https://doi.org/10.1093/nar/gkaa1100)) enriched with dbxrefs (`GO`, `COG`, `EC`) and annotated by specialized niche databases. For each db version we provide a comprehensive log file of all imported sequences and annotations.
+        To provide standardized annotations adhearing to FAIR principles, Bakta utilizes a versioned custom annotation database comprising UniProt's [UniRef100 & UniRef90](https://www.uniprot.org/uniref/) protein clusters (FAIR -> [DOI](http://dx.doi.org/10.1038/s41597-019-0180-9)/[DOI](https://doi.org/10.1093/nar/gkaa1100)) enriched with dbxrefs (`GO`, `COG`, `EC`) and annotated by specialized niche databases. For each DB version we provide a comprehensive log file of all imported sequences and annotations.
         
         - **Small proteins / short open reading frames**
         Bakta detects and annotates small proteins/short open reading frames (**sORF**) which are not predicted by tools like `Prodigal`.
         
         - **Expert annotation systems**
         To provide high quality annotations for certain proteins of higher interest, *e.g.* AMR & VF genes, Bakta includes & merges different expert annotation systems. Currently, Bakta uses NCBI's AMRFinderPlus for AMR gene annotations as well as an generalized protein sequence expert system with distinct coverage, identity and priority values for each sequence, currenlty comprising the [VFDB](http://www.mgc.ac.cn/VFs/main.htm) as well as NCBI's [BlastRules](https://ftp.ncbi.nih.gov/pub/blastrules/).
         
@@ -129,39 +129,39 @@
         - Blast+ (2.12.0) <https://www.ncbi.nlm.nih.gov/pubmed/2231712> <https://blast.ncbi.nlm.nih.gov>
         - AMRFinderPlus (3.10.23) <https://github.com/ncbi/amr>
         - DeepSig (1.2.5) <https://doi.org/10.1093/bioinformatics/btx818>
         
         ### Database download
         
         Bakta requires a mandatory database which is publicly hosted at Zenodo: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4247252.svg)](https://doi.org/10.5281/zenodo.4247252)
-        We provide 2 versions: `full` and `light`. To get best annotation results and to use all features, we recommend using the default (`full`). If you seek for maximum runtime performance or if download time/storage requirements are an issue, please try the `light` version. Further information is provided in the [database](#database) section below.
+        We provide 2 types: `full` and `light`. To get best annotation results and to use all features, we recommend using the `full` (default). If you seek for maximum runtime performance or if download time/storage requirements are an issue, please try the `light` version. Further information is provided in the [database](#database) section below.
         
-        List available DB versions:
+        List available DB versions (available as either `full` or `light`):
         
         ```bash
         bakta_db list
         ...
         ```
         
         To download the most recent compatible database version we recommend to use the internal database download & setup tool:
         
         ```bash
-        bakta_db download --output <output-path> --type light
+        bakta_db download --output <output-path> --type [light|full]
         ```
         
         Of course, the database can also be downloaded manually:
         
         ```bash
-        wget https://zenodo.org/record/7025248/files/db-light.tar.gz
+        wget https://zenodo.org/record/7669534/files/db-light.tar.gz
         tar -xzf db-light.tar.gz
         rm db-light.tar.gz
         amrfinder_update --force_update --database db-light/amrfinderplus-db/
         ```
         
-        As an additional data repository backup, we provide the most recent database version via our institute servers: [full](https://jlubox.uni-giessen.de/getlink/fiWhS6LJi8AizXvspaRxRzPN/db.tar.gz), [light](https://jlubox.uni-giessen.de/getlink/fiWhS6LJi8AizXvspaRxRzPN/db-light.tar.gz). However, the bandwith is limited. Hence, please use it with caution and only if Zenodo might be temporarily uncreachable or slow. In these cases, please also download the AMRFinderPlus database as indicated above.
+        As an additional data repository backup, we provide the most recent database version via our institute servers: [full](https://jlubox.uni-giessen.de/dl/fiKeyT1huWv9vW5cXKYkZXYB/db.tar.gz), [light](https://jlubox.uni-giessen.de/dl/fiG6AHmHA94t4v2r2vwW91WB/db-light.tar.gz). However, the bandwith is limited. Hence, please use it with caution and only if Zenodo might be temporarily uncreachable or slow. In these cases, please also download the AMRFinderPlus database as indicated above.
         
         Update an existing database:
         
         ```bash
         bakta_db update --db <existing-db-path> [--tmp-dir <tmp-directory>]
         ```
         
@@ -274,21 +274,22 @@
         - `<prefix>.gbff`: annotations & sequences in (multi) GenBank format
         - `<prefix>.embl`: annotations & sequences in (multi) EMBL format
         - `<prefix>.fna`: replicon/contig DNA sequences as FASTA
         - `<prefix>.ffn`: feature nucleotide sequences as FASTA
         - `<prefix>.faa`: CDS/sORF amino acid sequences as FASTA
         - `<prefix>.hypotheticals.tsv`: further information on hypothetical protein CDS as simple human readble tab separated values
         - `<prefix>.hypotheticals.faa`: hypothetical protein CDS amino acid sequences as FASTA
+        - `<prefix>.json`: all (internal) annotation & sequence information as JSON
         - `<prefix>.txt`: summary as TXT
         - `<prefix>.png`: circular genome annotation plot as PNG
         - `<prefix>.svg`: circular genome annotation plot as SVG
         
         The `<prefix>` can be set via `--prefix <prefix>`. If no prefix is set, Bakta uses the input file prefix.
         
-        Additionally, Bakta provides detailed information on each annotated feature in a standardized machine-readable JSON file `<prefix>.json`:
+        Of note, Bakta provides all detailed (internal) information on each annotated feature in a standardized machine-readable JSON file `<prefix>.json`:
         
         ```json
         {
             "genome": {
                 "genus": "Escherichia",
                 "species": "coli",
                 ...
@@ -350,28 +351,29 @@
           --db DB, -d DB        Database path (default = <bakta_path>/db). Can also be provided as BAKTA_DB environment variable.
           --min-contig-length MIN_CONTIG_LENGTH, -m MIN_CONTIG_LENGTH
                                 Minimum contig size (default = 1; 200 in compliant mode)
           --prefix PREFIX, -p PREFIX
                                 Prefix for output files
           --output OUTPUT, -o OUTPUT
                                 Output directory (default = current working directory)
+          --force, -f           Force overwriting existing output folder
         
         Organism:
           --genus GENUS         Genus name
           --species SPECIES     Species name
           --strain STRAIN       Strain name
           --plasmid PLASMID     Plasmid name
         
         Annotation:
           --complete            All sequences are complete replicons (chromosome/plasmid[s])
           --prodigal-tf PRODIGAL_TF
                                 Path to existing Prodigal training file to use for CDS prediction
           --translation-table {11,4}
                                 Translation table: 11/4 (default = 11)
-          --gram {+,-,?}        Gram type for signal peptide predictions: +/-/? (default = '?')
+          --gram {+,-,?}        Gram type for signal peptide predictions: +/-/? (default = ?)
           --locus LOCUS         Locus prefix (default = 'contig')
           --locus-tag LOCUS_TAG
                                 Locus tag prefix (default = autogenerated)
           --keep-contig-headers
                                 Keep original contig headers
           --replicons REPLICONS, -r REPLICONS
                                 Replicon information table (tsv/csv)
@@ -486,33 +488,32 @@
         
         1. Gaps: in-mem detection & annotation of sequence gaps
         2. oriC/oriV/oriT: Blast+ (cov=0.8, id=0.8) vs. [MOB-suite](https://github.com/phac-nml/mob-suite) oriT & [DoriC](http://tubic.org/doric/public/index.php) oriC/oriV sequences. Annotations of ori regions take into account overlapping Blast+ hits and are conducted based on a majority vote heuristic. Region edges are fuzzy - use with caution!
         
         ## Database
         
         The Bakta database comprises a set of AA & DNA sequence databases as well as HMM & covariance models.
-        At its core Bakta utilizes a compact read-only SQLite db storing protein sequence digests, lengths, pre-assigned annotations and dbxrefs of UPS, IPS and PSC from:
+        At its core Bakta utilizes a compact read-only SQLite DB storing protein sequence digests, lengths, pre-assigned annotations and dbxrefs of UPS, IPS and PSC from:
         
-        - **UPS**: UniParc / UniProtKB (241,116,844)
-        - **IPS**: UniProt UniRef100 (223,313,098)
-        - **PSC**: UniProt UniRef90 (99,555,646)
-        - **PSCC**: UniProt UniRef50 (13,398,956)
-        
-        This allows the exact protein sequences identification via MD5 digests & sequence lengths as well as the rapid subsequent lookup of related information. Protein sequence digests are checked for hash collisions while the db creation process.
-        IPS & PSC have been comprehensively pre-annotated integrating annotations & database *dbxrefs* from:
-        
-        - NCBI nonredundant proteins (IPS: 183,797,372)
-        - NCBI COG db (PSC: 3,424,142)
-        - KEGG Kofams (PSC: 17,787,347)
-        - SwissProt EC/GO terms (PSC: 336,030)
-        - NCBI NCBIfams (PSC: 13,466,827)
-        - PHROG (PSC: 0)
-        - NCBI AMRFinderPlus (IPS: 7,009)
-        - ISFinder db (IPS: 53,341, PSC: 11,412)
-        - Pfam families (PSC: 3,917,555)
+        - **UPS**: UniParc / UniProtKB (246,384,812)
+        - **IPS**: UniProt UniRef100 (228,759,203)
+        - **PSC**: UniProt UniRef90 (100,315,337)
+        - **PSCC**: UniProt UniRef50 (23,959,577)
+        
+        This allows the exact protein sequences identification via MD5 digests & sequence lengths as well as the rapid subsequent lookup of related information. Protein sequence digests are checked for hash collisions while the DB creation process. IPS & PSC have been comprehensively pre-annotated integrating annotations & database *dbxrefs* from:
+        
+        - NCBI nonredundant proteins (IPS: 192,288,757)
+        - NCBI COG DB (PSC: 3,428,564)
+        - KEGG Kofams (PSC: 16,776,225)
+        - SwissProt EC/GO terms (PSC: 336,187)
+        - NCBI NCBIfams (PSC: 14,391,965)
+        - PHROG (PSC: 4,379)
+        - NCBI AMRFinderPlus (IPS: 7,235)
+        - ISFinder DB (IPS: 125,967, PSC: 11,800)
+        - Pfam families (PSC: 248,169)
         
         To provide high quality annotations for distinct protein sequences of high importance (AMR, VF, *etc*) which cannot sufficiently be covered by the IPS/PSC approach, Bakta provides additional expert systems. For instance, AMR genes, are annotated via NCBI's AMRFinderPlus.
         An expandable alignment-based expert system supports the incorporation of high quality annotations from multiple sources. This currenlty comprises NCBI's BlastRules as well as VFDB and will be complemented with more expert annotation sources over time. Internally, this expert system is based on a Diamond DB comprising the following information in a standardized format:
         
         - source: *e.g.* BlastRules
         - rank: a precedence rank
         - min identity
@@ -520,30 +521,31 @@
         - min model coverage
         - gene lable
         - product description
         - dbxrefs
         
         Rfam covariance models:
         
-        - ncRNA: 798
+        - ncRNA: 802
         - ncRNA cis-regulatory regions: 270
         
         ori sequences:
         
-        - oriC/V: 10,878
+        - oriC/V: 6,690
         - oriT: 502
         
-        To provide FAIR annotations, the database releases are SemVer versioned (w/o patch level), *i.e.* `<major>.<minor>`. For each version we provide a comprehensive log file tracking all imported sequences as well as annotations thereof. The db schema is represented by the `<major>` digit and automatically checked at runtime by Bakta in order to ensure compatibility. Content updates are tracked by the `<minor>` digit.
+        To provide FAIR annotations, the database releases are SemVer versioned (w/o patch level), *i.e.* `<major>.<minor>`. For each version we provide a comprehensive log file tracking all imported sequences as well as annotations thereof. The DB schema is represented by the `<major>` digit and automatically checked at runtime by Bakta in order to ensure compatibility. Content updates are tracked by the `<minor>` digit.
         
-        Since this taxonomic-untargeted database is fairly demanding regarding storage consumption, we provide a lightweight version providing all non-coding feature information but only PSCC information from UniRef50 clusters for CDS. If download bandwiths or storage requirements are an issue or if faster runtimes for less-specific annotation are favored, the `light` database will do the job!
+        As this taxonomic-untargeted database is fairly demanding in terms of storage consumption, we also provide a lightweight DB type providing all non-coding feature information but only PSCC information from UniRef50 clusters for CDS. If download bandwiths or storage requirements become an issue or if shorter runtimes are favored over more-specific annotation, the `light` DB will do the job.
         
-        Latest database version 5.0:
+        Latest database version: 5.0
+        DB types:
         
-        - `full`: 31 Gb zipped, 60 Gb unzipped
-        - `light`: 1.2 Gb zipped, 2.8 Gb unzipped
+        - `light`: 1.2 Gb zipped, 2.8 Gb unzipped, MD5: a40e680b4aab7871102f31aaac91838b
+        - `full`: 31 Gb zipped, 60 Gb unzipped, MD5: 3200136a0a32b3c33d1cb348ab6b87de
         
         All database releases are hosted at Zenodo: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4247252.svg)](https://doi.org/10.5281/zenodo.4247252)
         
         ## Genome Submission
         
         Most genomes annotated with Bakta should be ready-to-submid to INSDC member databases GenBank and ENA. As a first step, please register your BioProject (e.g. PRJNA123456) and your locus_tag prefix (*e.g.* ESAKAI).
         
@@ -622,39 +624,43 @@
         ### Output
         
         Annotation results are provided in standard bioinformatics file formats:
         
         - `<prefix>.tsv`: annotations as simple human readble TSV
         - `<prefix>.faa`: protein sequences as FASTA
         - `<prefix>.hypotheticals.tsv`: further information on hypothetical proteins as simple human readble tab separated values
+        - `<prefix>.json`: all (internal) annotation & sequence information as JSON
         
         The `<prefix>` can be set via `--prefix <prefix>`. If no prefix is set, Bakta uses the input file prefix.
         
         ### Usage
         
         ```bash
-        usage: bakta_proteins [--db DB] [--output OUTPUT] [--prefix PREFIX] [--proteins PROTEINS] [--help] [--threads THREADS] [--tmp-dir TMP_DIR] [--version] <input>
+        usage: bakta_proteins [--db DB] [--output OUTPUT] [--prefix PREFIX] [--force] [--proteins PROTEINS] [--help] [--verbose] [--debug] [--threads THREADS] [--tmp-dir TMP_DIR] [--version] <input>
         
         Rapid & standardized annotation of bacterial genomes, MAGs & plasmids
         
         positional arguments:
           <input>               Protein sequences in (zipped) fasta format
         
         Input / Output:
           --db DB, -d DB        Database path (default = <bakta_path>/db). Can also be provided as BAKTA_DB environment variable.
           --output OUTPUT, -o OUTPUT
                                 Output directory (default = current working directory)
           --prefix PREFIX, -p PREFIX
                                 Prefix for output files
+          --force, -f           Force overwriting existing output folder
         
         Annotation:
           --proteins PROTEINS   Fasta file of trusted protein sequences for annotation
         
-        Runtime & auxiliary options:
+        General:
           --help, -h            Show this help message and exit
+          --verbose, -v         Print verbose information
+          --debug               Run Bakta in debug mode. Temp data will not be removed.
           --threads THREADS, -t THREADS
                                 Number of threads to use (default = number of available CPUs)
           --tmp-dir TMP_DIR     Location for temporary files (default = system dependent auto detection)
           --version, -V         show program's version number and exit
         ```
         
         ## Genome plots
@@ -792,14 +798,16 @@
         
 Keywords: bioinformatics,annotation,bacteria,plasmids
 Platform: UNKNOWN
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Requires-Python: >=3.8
```

### Comparing `bakta-1.7.0/README.md` & `bakta-1.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 - **Fast**
 This AFSI approach substantially accellerates the annotation process by avoiding computationally expensive homology searches for identified genes. Thus, Bakta can annotate a typical bacterial genome in 10 &plusmn;5 min on a laptop, plasmids in a couple of seconds/minutes.
 
 - **Database cross-references**
 Fostering the [FAIR](https://www.go-fair.org/fair-principles) principles, Bakta exploits its AFSI approach to annotate CDS with database cross-references (**dbxref**) to RefSeq (`WP_*`), UniRef100 (`UniRef100_*`) and UniParc (`UPI*`). By doing so, IPS allow the surveillance of distinct gene alleles and streamlining comparative analysis as well as posterior (external) annotations of `putative` & `hypothetical` protein sequences which can be mapped back to existing CDS via these exact & stable identifiers (*E. coli* gene [ymiA](https://www.uniprot.org/uniprot/P0CB62) [...more](https://www.uniprot.org/help/dubious_sequences)). Currently, Bakta identifies ~214.8 mio, ~199 mio and ~161 mio distinct protein sequences from UniParc, UniRef100 and RefSeq, respectively. Hence, for certain genomes, up to 99 % of all CDS can be identified this way, skipping computationally expensive sequence alignments.
 
 - **FAIR annotations**
-To provide standardized annotations adhearing to FAIR principles, Bakta utilizes a versioned custom annotation database comprising UniProt's [UniRef100 & UniRef90](https://www.uniprot.org/uniref/) protein clusters (FAIR -> [DOI](http://dx.doi.org/10.1038/s41597-019-0180-9)/[DOI](https://doi.org/10.1093/nar/gkaa1100)) enriched with dbxrefs (`GO`, `COG`, `EC`) and annotated by specialized niche databases. For each db version we provide a comprehensive log file of all imported sequences and annotations.
+To provide standardized annotations adhearing to FAIR principles, Bakta utilizes a versioned custom annotation database comprising UniProt's [UniRef100 & UniRef90](https://www.uniprot.org/uniref/) protein clusters (FAIR -> [DOI](http://dx.doi.org/10.1038/s41597-019-0180-9)/[DOI](https://doi.org/10.1093/nar/gkaa1100)) enriched with dbxrefs (`GO`, `COG`, `EC`) and annotated by specialized niche databases. For each DB version we provide a comprehensive log file of all imported sequences and annotations.
 
 - **Small proteins / short open reading frames**
 Bakta detects and annotates small proteins/short open reading frames (**sORF**) which are not predicted by tools like `Prodigal`.
 
 - **Expert annotation systems**
 To provide high quality annotations for certain proteins of higher interest, *e.g.* AMR & VF genes, Bakta includes & merges different expert annotation systems. Currently, Bakta uses NCBI's AMRFinderPlus for AMR gene annotations as well as an generalized protein sequence expert system with distinct coverage, identity and priority values for each sequence, currenlty comprising the [VFDB](http://www.mgc.ac.cn/VFs/main.htm) as well as NCBI's [BlastRules](https://ftp.ncbi.nih.gov/pub/blastrules/).
 
@@ -117,39 +117,39 @@
 - Blast+ (2.12.0) <https://www.ncbi.nlm.nih.gov/pubmed/2231712> <https://blast.ncbi.nlm.nih.gov>
 - AMRFinderPlus (3.10.23) <https://github.com/ncbi/amr>
 - DeepSig (1.2.5) <https://doi.org/10.1093/bioinformatics/btx818>
 
 ### Database download
 
 Bakta requires a mandatory database which is publicly hosted at Zenodo: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4247252.svg)](https://doi.org/10.5281/zenodo.4247252)
-We provide 2 versions: `full` and `light`. To get best annotation results and to use all features, we recommend using the default (`full`). If you seek for maximum runtime performance or if download time/storage requirements are an issue, please try the `light` version. Further information is provided in the [database](#database) section below.
+We provide 2 types: `full` and `light`. To get best annotation results and to use all features, we recommend using the `full` (default). If you seek for maximum runtime performance or if download time/storage requirements are an issue, please try the `light` version. Further information is provided in the [database](#database) section below.
 
-List available DB versions:
+List available DB versions (available as either `full` or `light`):
 
 ```bash
 bakta_db list
 ...
 ```
 
 To download the most recent compatible database version we recommend to use the internal database download & setup tool:
 
 ```bash
-bakta_db download --output <output-path> --type light
+bakta_db download --output <output-path> --type [light|full]
 ```
 
 Of course, the database can also be downloaded manually:
 
 ```bash
-wget https://zenodo.org/record/7025248/files/db-light.tar.gz
+wget https://zenodo.org/record/7669534/files/db-light.tar.gz
 tar -xzf db-light.tar.gz
 rm db-light.tar.gz
 amrfinder_update --force_update --database db-light/amrfinderplus-db/
 ```
 
-As an additional data repository backup, we provide the most recent database version via our institute servers: [full](https://jlubox.uni-giessen.de/getlink/fiWhS6LJi8AizXvspaRxRzPN/db.tar.gz), [light](https://jlubox.uni-giessen.de/getlink/fiWhS6LJi8AizXvspaRxRzPN/db-light.tar.gz). However, the bandwith is limited. Hence, please use it with caution and only if Zenodo might be temporarily uncreachable or slow. In these cases, please also download the AMRFinderPlus database as indicated above.
+As an additional data repository backup, we provide the most recent database version via our institute servers: [full](https://jlubox.uni-giessen.de/dl/fiKeyT1huWv9vW5cXKYkZXYB/db.tar.gz), [light](https://jlubox.uni-giessen.de/dl/fiG6AHmHA94t4v2r2vwW91WB/db-light.tar.gz). However, the bandwith is limited. Hence, please use it with caution and only if Zenodo might be temporarily uncreachable or slow. In these cases, please also download the AMRFinderPlus database as indicated above.
 
 Update an existing database:
 
 ```bash
 bakta_db update --db <existing-db-path> [--tmp-dir <tmp-directory>]
 ```
 
@@ -262,21 +262,22 @@
 - `<prefix>.gbff`: annotations & sequences in (multi) GenBank format
 - `<prefix>.embl`: annotations & sequences in (multi) EMBL format
 - `<prefix>.fna`: replicon/contig DNA sequences as FASTA
 - `<prefix>.ffn`: feature nucleotide sequences as FASTA
 - `<prefix>.faa`: CDS/sORF amino acid sequences as FASTA
 - `<prefix>.hypotheticals.tsv`: further information on hypothetical protein CDS as simple human readble tab separated values
 - `<prefix>.hypotheticals.faa`: hypothetical protein CDS amino acid sequences as FASTA
+- `<prefix>.json`: all (internal) annotation & sequence information as JSON
 - `<prefix>.txt`: summary as TXT
 - `<prefix>.png`: circular genome annotation plot as PNG
 - `<prefix>.svg`: circular genome annotation plot as SVG
 
 The `<prefix>` can be set via `--prefix <prefix>`. If no prefix is set, Bakta uses the input file prefix.
 
-Additionally, Bakta provides detailed information on each annotated feature in a standardized machine-readable JSON file `<prefix>.json`:
+Of note, Bakta provides all detailed (internal) information on each annotated feature in a standardized machine-readable JSON file `<prefix>.json`:
 
 ```json
 {
     "genome": {
         "genus": "Escherichia",
         "species": "coli",
         ...
@@ -338,28 +339,29 @@
   --db DB, -d DB        Database path (default = <bakta_path>/db). Can also be provided as BAKTA_DB environment variable.
   --min-contig-length MIN_CONTIG_LENGTH, -m MIN_CONTIG_LENGTH
                         Minimum contig size (default = 1; 200 in compliant mode)
   --prefix PREFIX, -p PREFIX
                         Prefix for output files
   --output OUTPUT, -o OUTPUT
                         Output directory (default = current working directory)
+  --force, -f           Force overwriting existing output folder
 
 Organism:
   --genus GENUS         Genus name
   --species SPECIES     Species name
   --strain STRAIN       Strain name
   --plasmid PLASMID     Plasmid name
 
 Annotation:
   --complete            All sequences are complete replicons (chromosome/plasmid[s])
   --prodigal-tf PRODIGAL_TF
                         Path to existing Prodigal training file to use for CDS prediction
   --translation-table {11,4}
                         Translation table: 11/4 (default = 11)
-  --gram {+,-,?}        Gram type for signal peptide predictions: +/-/? (default = '?')
+  --gram {+,-,?}        Gram type for signal peptide predictions: +/-/? (default = ?)
   --locus LOCUS         Locus prefix (default = 'contig')
   --locus-tag LOCUS_TAG
                         Locus tag prefix (default = autogenerated)
   --keep-contig-headers
                         Keep original contig headers
   --replicons REPLICONS, -r REPLICONS
                         Replicon information table (tsv/csv)
@@ -474,33 +476,32 @@
 
 1. Gaps: in-mem detection & annotation of sequence gaps
 2. oriC/oriV/oriT: Blast+ (cov=0.8, id=0.8) vs. [MOB-suite](https://github.com/phac-nml/mob-suite) oriT & [DoriC](http://tubic.org/doric/public/index.php) oriC/oriV sequences. Annotations of ori regions take into account overlapping Blast+ hits and are conducted based on a majority vote heuristic. Region edges are fuzzy - use with caution!
 
 ## Database
 
 The Bakta database comprises a set of AA & DNA sequence databases as well as HMM & covariance models.
-At its core Bakta utilizes a compact read-only SQLite db storing protein sequence digests, lengths, pre-assigned annotations and dbxrefs of UPS, IPS and PSC from:
+At its core Bakta utilizes a compact read-only SQLite DB storing protein sequence digests, lengths, pre-assigned annotations and dbxrefs of UPS, IPS and PSC from:
 
-- **UPS**: UniParc / UniProtKB (241,116,844)
-- **IPS**: UniProt UniRef100 (223,313,098)
-- **PSC**: UniProt UniRef90 (99,555,646)
-- **PSCC**: UniProt UniRef50 (13,398,956)
-
-This allows the exact protein sequences identification via MD5 digests & sequence lengths as well as the rapid subsequent lookup of related information. Protein sequence digests are checked for hash collisions while the db creation process.
-IPS & PSC have been comprehensively pre-annotated integrating annotations & database *dbxrefs* from:
-
-- NCBI nonredundant proteins (IPS: 183,797,372)
-- NCBI COG db (PSC: 3,424,142)
-- KEGG Kofams (PSC: 17,787,347)
-- SwissProt EC/GO terms (PSC: 336,030)
-- NCBI NCBIfams (PSC: 13,466,827)
-- PHROG (PSC: 0)
-- NCBI AMRFinderPlus (IPS: 7,009)
-- ISFinder db (IPS: 53,341, PSC: 11,412)
-- Pfam families (PSC: 3,917,555)
+- **UPS**: UniParc / UniProtKB (246,384,812)
+- **IPS**: UniProt UniRef100 (228,759,203)
+- **PSC**: UniProt UniRef90 (100,315,337)
+- **PSCC**: UniProt UniRef50 (23,959,577)
+
+This allows the exact protein sequences identification via MD5 digests & sequence lengths as well as the rapid subsequent lookup of related information. Protein sequence digests are checked for hash collisions while the DB creation process. IPS & PSC have been comprehensively pre-annotated integrating annotations & database *dbxrefs* from:
+
+- NCBI nonredundant proteins (IPS: 192,288,757)
+- NCBI COG DB (PSC: 3,428,564)
+- KEGG Kofams (PSC: 16,776,225)
+- SwissProt EC/GO terms (PSC: 336,187)
+- NCBI NCBIfams (PSC: 14,391,965)
+- PHROG (PSC: 4,379)
+- NCBI AMRFinderPlus (IPS: 7,235)
+- ISFinder DB (IPS: 125,967, PSC: 11,800)
+- Pfam families (PSC: 248,169)
 
 To provide high quality annotations for distinct protein sequences of high importance (AMR, VF, *etc*) which cannot sufficiently be covered by the IPS/PSC approach, Bakta provides additional expert systems. For instance, AMR genes, are annotated via NCBI's AMRFinderPlus.
 An expandable alignment-based expert system supports the incorporation of high quality annotations from multiple sources. This currenlty comprises NCBI's BlastRules as well as VFDB and will be complemented with more expert annotation sources over time. Internally, this expert system is based on a Diamond DB comprising the following information in a standardized format:
 
 - source: *e.g.* BlastRules
 - rank: a precedence rank
 - min identity
@@ -508,30 +509,31 @@
 - min model coverage
 - gene lable
 - product description
 - dbxrefs
 
 Rfam covariance models:
 
-- ncRNA: 798
+- ncRNA: 802
 - ncRNA cis-regulatory regions: 270
 
 ori sequences:
 
-- oriC/V: 10,878
+- oriC/V: 6,690
 - oriT: 502
 
-To provide FAIR annotations, the database releases are SemVer versioned (w/o patch level), *i.e.* `<major>.<minor>`. For each version we provide a comprehensive log file tracking all imported sequences as well as annotations thereof. The db schema is represented by the `<major>` digit and automatically checked at runtime by Bakta in order to ensure compatibility. Content updates are tracked by the `<minor>` digit.
+To provide FAIR annotations, the database releases are SemVer versioned (w/o patch level), *i.e.* `<major>.<minor>`. For each version we provide a comprehensive log file tracking all imported sequences as well as annotations thereof. The DB schema is represented by the `<major>` digit and automatically checked at runtime by Bakta in order to ensure compatibility. Content updates are tracked by the `<minor>` digit.
 
-Since this taxonomic-untargeted database is fairly demanding regarding storage consumption, we provide a lightweight version providing all non-coding feature information but only PSCC information from UniRef50 clusters for CDS. If download bandwiths or storage requirements are an issue or if faster runtimes for less-specific annotation are favored, the `light` database will do the job!
+As this taxonomic-untargeted database is fairly demanding in terms of storage consumption, we also provide a lightweight DB type providing all non-coding feature information but only PSCC information from UniRef50 clusters for CDS. If download bandwiths or storage requirements become an issue or if shorter runtimes are favored over more-specific annotation, the `light` DB will do the job.
 
-Latest database version 5.0:
+Latest database version: 5.0
+DB types:
 
-- `full`: 31 Gb zipped, 60 Gb unzipped
-- `light`: 1.2 Gb zipped, 2.8 Gb unzipped
+- `light`: 1.2 Gb zipped, 2.8 Gb unzipped, MD5: a40e680b4aab7871102f31aaac91838b
+- `full`: 31 Gb zipped, 60 Gb unzipped, MD5: 3200136a0a32b3c33d1cb348ab6b87de
 
 All database releases are hosted at Zenodo: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4247252.svg)](https://doi.org/10.5281/zenodo.4247252)
 
 ## Genome Submission
 
 Most genomes annotated with Bakta should be ready-to-submid to INSDC member databases GenBank and ENA. As a first step, please register your BioProject (e.g. PRJNA123456) and your locus_tag prefix (*e.g.* ESAKAI).
 
@@ -610,39 +612,43 @@
 ### Output
 
 Annotation results are provided in standard bioinformatics file formats:
 
 - `<prefix>.tsv`: annotations as simple human readble TSV
 - `<prefix>.faa`: protein sequences as FASTA
 - `<prefix>.hypotheticals.tsv`: further information on hypothetical proteins as simple human readble tab separated values
+- `<prefix>.json`: all (internal) annotation & sequence information as JSON
 
 The `<prefix>` can be set via `--prefix <prefix>`. If no prefix is set, Bakta uses the input file prefix.
 
 ### Usage
 
 ```bash
-usage: bakta_proteins [--db DB] [--output OUTPUT] [--prefix PREFIX] [--proteins PROTEINS] [--help] [--threads THREADS] [--tmp-dir TMP_DIR] [--version] <input>
+usage: bakta_proteins [--db DB] [--output OUTPUT] [--prefix PREFIX] [--force] [--proteins PROTEINS] [--help] [--verbose] [--debug] [--threads THREADS] [--tmp-dir TMP_DIR] [--version] <input>
 
 Rapid & standardized annotation of bacterial genomes, MAGs & plasmids
 
 positional arguments:
   <input>               Protein sequences in (zipped) fasta format
 
 Input / Output:
   --db DB, -d DB        Database path (default = <bakta_path>/db). Can also be provided as BAKTA_DB environment variable.
   --output OUTPUT, -o OUTPUT
                         Output directory (default = current working directory)
   --prefix PREFIX, -p PREFIX
                         Prefix for output files
+  --force, -f           Force overwriting existing output folder
 
 Annotation:
   --proteins PROTEINS   Fasta file of trusted protein sequences for annotation
 
-Runtime & auxiliary options:
+General:
   --help, -h            Show this help message and exit
+  --verbose, -v         Print verbose information
+  --debug               Run Bakta in debug mode. Temp data will not be removed.
   --threads THREADS, -t THREADS
                         Number of threads to use (default = number of available CPUs)
   --tmp-dir TMP_DIR     Location for temporary files (default = system dependent auto detection)
   --version, -V         show program's version number and exit
 ```
 
 ## Genome plots
```

### Comparing `bakta-1.7.0/bakta/config.py` & `bakta-1.8.0/bakta/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 import logging
 import multiprocessing as mp
 import os
+import re
+import shutil
 import sys
 import tempfile
 
 from argparse import Namespace
 from datetime import datetime
 from pathlib import Path
 
 import bakta.constants as bc
 
 
+PLASMID_NAME_PATTERN = re.compile(r'p[a-zA-Z0-9\._]{1,19}')
+PLASMID_UNNAMED_PATTERN = re.compile(r'unnamed[0-9]{0,3}')
+
+
 log = logging.getLogger('CONFIG')
 
 
 # runtime configurations
 env = os.environ.copy()
 threads = None
 verbose = None
@@ -24,14 +30,15 @@
 db_path = None
 db_info = None
 tmp_path = None
 genome_path = None
 min_contig_length = None
 prefix = None
 output_path = None
+force = None
 
 # organism configuration
 genus = None
 species = None
 strain = None
 plasmid = None
 taxon = None
@@ -78,15 +85,15 @@
     log.info('verbose=%s', verbose)
     debug = args.debug
     log.info('debug=%s', debug)
     if(debug):
         verbose = True
 
     # input / output path configurations
-    global db_path, db_info, tmp_path, genome_path, min_contig_length, prefix, output_path
+    global db_path, db_info, tmp_path, genome_path, min_contig_length, prefix, output_path, force
     db_path = check_db_path(args)
     tmp_path = check_tmp_path(args)
 
     try:
         if(args.genome == ''):
             raise ValueError('File path argument must be non-empty')
         genome_path = Path(args.genome).resolve()
@@ -101,14 +108,16 @@
     min_contig_length = args.min_contig_length
     if(min_contig_length <= 0):
         log.error("wrong argument for 'min-contig-length' parameter! min_contig_length=%s", min_contig_length)
         sys.exit(f"ERROR: wrong argument ({min_contig_length}) for 'min- contig-length' parameter! Value must be larger than 0")
     log.info('min_contig_length=%s', min_contig_length)
     log.info('prefix=%s', prefix)  # set in main.py before global logger config
     log.info('output-path=%s', output_path)
+    force = args.force
+    log.info('force=%s', force)
 
     # organism configurations
     global genus, species, strain, plasmid, taxon
     genus = args.genus
     if(genus is not None):
         genus = genus.strip()
         if(genus == ''):
@@ -130,14 +139,25 @@
     if(strain is not None):
         strain = strain.strip()
         if(strain == ''):
             log.error("Empty 'strain' parameter! strain=%s", species)
             sys.exit(f"ERROR: empty 'strain' parameter!")
     log.info('strain=%s', strain)
     plasmid = args.plasmid
+    if(plasmid is not None):
+        plasmid = plasmid.strip()
+        if(plasmid == ''):
+            log.error("Empty 'plasmid' parameter! plasmid=%s", plasmid)
+            sys.exit(f"ERROR: empty 'plasmid' parameter!")
+        elif('plasmid' in plasmid.lower()):
+            log.error("Wrong 'plasmid' parameter! plasmid=%s", plasmid)
+            sys.exit(f"ERROR: wrong 'plasmid' parameter! The plasmid name mustn't contain the word 'plasmid'.")
+        elif(PLASMID_NAME_PATTERN.fullmatch(plasmid) is None and PLASMID_UNNAMED_PATTERN.fullmatch(plasmid) is None):
+            log.error("Wrong 'plasmid' name! plasmid=%s", plasmid)
+            sys.exit(f"ERROR: wrong 'plasmid' name! Plasmid names must either be named as 'unnamed', 'unnamed1', ... or start with a lower 'p', contain only digits, dots, underscores and letters, and are limited to 20 characters in total.")
     log.info('plasmid=%s', plasmid)
     taxon = ' '.join([t for t in [genus, species, strain] if t is not None])
     if(taxon == ''):
         taxon = None
 
     # annotation configurations
     global complete, prodigal_tf, translation_table, keep_contig_headers, locus, locus_tag, gram, replicons, compliant, user_proteins, meta
@@ -274,29 +294,36 @@
     elif(threads > max_threads):
         log.error("wrong argument for 'threads' parameter! More threads requested than available: requested=%i, available=%i", threads, max_threads)
         sys.exit(f"ERROR: wrong argument ({threads}) for 'threads' parameter! More threads requested ({threads}) than available ({max_threads}).")
     log.info('threads=%i', threads)
     return threads
 
 
-def check_output_path(args: Namespace) -> Path:
+def check_output_path(output: str, force_override: bool) -> Path:
+    """Check provided output path
+    Args:
+        output (string): The output directory destination path
+        force_override (Bool): Whether to override existing output directories
+    """
     global output_path
-    try:
-        output_path = Path(args.output)
-        if(not output_path.exists()):
+    output_path = Path(output)
+    if(not output_path.exists()):
+        try:
             output_path.mkdir(parents=True, exist_ok=True)
+        except:
+            sys.exit(f'ERROR: could not resolve or create output directory ({output})!')
+    else:
+        if(force_override is False):
+            sys.exit(f'ERROR: output path ({output_path}) already exists! Either provide a non-existent new path or force overwriting it via \'--force\'')
         elif(not os.access(str(output_path), os.X_OK)):
             sys.exit(f'ERROR: output path ({output_path}) not accessible!')
         elif(not os.access(str(output_path), os.W_OK)):
             sys.exit(f'ERROR: output path ({output_path}) not writable!')
-        output_path = output_path.resolve()
-        log.info('output-path=%s', output_path)
-        return output_path
-    except:
-        sys.exit(f'ERROR: could not resolve or create output directory ({args.output})!')
+    output_path = output_path.resolve()
+    return output_path
 
 
 def check_db_path(args: Namespace) -> Path:
     global db_path
     env = os.environ.copy()
     if(args.db):
         db_dir = args.db
```

### Comparing `bakta-1.7.0/bakta/constants.py` & `bakta-1.8.0/bakta/constants.py`

 * *Files identical despite different names*

### Comparing `bakta-1.7.0/bakta/db.py` & `bakta-1.8.0/bakta/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,19 +169,24 @@
         versions = fetch_db_versions()
         if(not args.all):
             versions = [v for v in versions if v['major'] == bakta.__db_schema_version__]
 
         print('Available DB versions:')
         for v in sorted(versions, key=lambda v: (v['major'], v['minor'])):
             print(f"{v['major']}.{v['minor']}\t{v['date']}\t{v['doi']}")
+        
+        print("\nRun 'bakta_db download --type <TYPE>' to download the most recent version either as type 'full' (default) or 'light'.")
+        print("Run 'bakta_db download --minor <MINOR>' to download a specific minor version (either as type 'full' or 'light').")
+        print("\nType 'bakta_db download --help' for further details")
     elif(args.subcommand == 'download'):
         bu.test_dependency(bu.DEPENDENCY_AMRFINDERPLUS)
-        output_path = cfg.check_output_path(args)
+        output_path = cfg.check_output_path(args.output, True)
 
-        print('fetch DB versions...')
+        print(f'Selected DB type: {args.type}\n')
+        print('Fetch DB versions...')
         versions = fetch_db_versions()
         compatible_versions = [v for v in versions if v['major'] == bakta.__db_schema_version__]
         if(len(compatible_versions) == 0):
             sys.exit(f'Error: no compatible version available for current major db version {bakta.__db_schema_version__}')
         else:
             print(f'\t... compatible DB versions: {len(compatible_versions)}')
 
@@ -195,63 +200,63 @@
                 sys.exit(f"requested DB minor version {args.minor} is not available. Please use 'bakta_db list' to get a list of available DB versions")
         else:
             compatible_sorted = sorted(compatible_versions, key=lambda v: v['minor'], reverse=True)
             required_version = compatible_sorted[0]
 
         tarball_path = output_path.joinpath(f"{'db-light' if args.type == 'light' else 'db'}.tar.gz")
         db_url = f"https://zenodo.org/record/{required_version['record']}/files/{'db-light' if args.type == 'light' else 'db'}.tar.gz"
-        print(f"download database: v{required_version['major']}.{required_version['minor']}, type={args.type}, {required_version['date']}, DOI: {required_version['doi']}, URL: {db_url}...")
+        print(f"Download database: v{required_version['major']}.{required_version['minor']}, type={args.type}, {required_version['date']}, DOI: {required_version['doi']}, URL: {db_url}...")
         download(db_url, tarball_path)
         print('\t... done')
 
-        print('check MD5 sum...')
+        print('Check MD5 sum...')
         md5_sum = calc_md5_sum(tarball_path)
         required_md5 = required_version['md5-light' if args.type == 'light' else 'md5']
         if(md5_sum == required_md5):
             print(f'\t...database file OK: {md5_sum}')
         else:
             sys.exit(f"Error: corrupt database file! MD5 should be '{required_md5}' but is '{md5_sum}'")
 
-        print(f'extract DB tarball: file={tarball_path}, output={output_path}')
+        print(f'Extract DB tarball: file={tarball_path}, output={output_path}')
         untar(tarball_path, output_path)
         tarball_path.unlink()
 
         db_path = output_path.joinpath('db-light' if args.type == 'light' else 'db')
         db_info = check(db_path)
         if(db_info['major'] != required_version['major']):
             sys.exit(f"ERROR: wrong major db detected! required={required_version['major']}, detected={db_info['major']}")
         elif(db_info['minor'] != required_version['minor']):
             sys.exit(f"ERROR: wrong minor db detected! required={required_version['minor']}, detected={db_info['minor']}")
         elif(db_info['type'] != args.type == 'light'):
             sys.exit(f"ERROR: wrong db type detected! required={args.type}, detected={db_info['type']}")
-        print('successfully downloaded Bakta database!')
+        print('Successfully downloaded Bakta database!')
         print(f"\tversion: {required_version['major']}.{required_version['minor']}")
         print(f"\tType: {args.type}")
         print(f"\tDOI: {required_version['doi']}")
         print(f'\tpath: {db_path}')
 
         try:
             db_path.chmod(stat.S_IRUSR | stat.S_IWUSR | stat.S_IXUSR | stat.S_IRGRP | stat.S_IWGRP | stat.S_IXGRP | stat.S_IROTH | stat.S_IXOTH)  # set write permissions on old (existing) directory with updated content
             for db_file_path in db_path.iterdir():
                 db_file_path.chmod(stat.S_IRUSR | stat.S_IRGRP | stat.S_IROTH)
         except:
             sys.exit(f'ERROR: cannot set read|execute permissions on new database! path={db_path}, owner={db_path.owner()}, group={db_path.group()}, permissions={oct(db_path.stat().st_mode )[-3:]}')
 
-        print('update AMRFinderPlus database...')
+        print('Update AMRFinderPlus database...')
         update_amrfinderplus_db(db_path)
         print('\t... done')
 
         print(f"\nRun Bakta using '--db {db_path}' or set a BAKTA_DB environment variable: 'export BAKTA_DB={db_path}'")
     elif(args.subcommand == 'update'):
         bu.test_dependency(bu.DEPENDENCY_AMRFINDERPLUS)
         tmp_path = cfg.check_tmp_path(args)
         db_old_path = cfg.check_db_path(args)
         db_old_info = check(db_old_path)
-        print(f"existing database: v{db_old_info['major']}.{db_old_info['minor']}, type={db_old_info['type']}")
-        print('fetch DB versions...')
+        print(f"Existing database: v{db_old_info['major']}.{db_old_info['minor']}, type={db_old_info['type']}")
+        print('Fetch DB versions...')
         versions = fetch_db_versions()
         compatible_versions = [v for v in versions if v['major'] == bakta.__db_schema_version__]
         if(len(compatible_versions) == 0):
             sys.exit(f'Error: no compatible version available for current major db version {bakta.__db_schema_version__}')
         else:
             print(f'\t... compatible DB versions: {len(compatible_versions)}')
 
@@ -259,44 +264,44 @@
         if(compatible_sorted[0]['minor'] <= db_old_info['minor']):
             print(f"Database version {db_old_info['major']}.{db_old_info['minor']} is up-to-date")
             sys.exit()
         required_version = compatible_sorted[0]
 
         tarball_path = output_path.joinpath(f"{'db-light' if args.type == 'light' else 'db'}.tar.gz")
         db_url = f"https://zenodo.org/record/{required_version['record']}/files/{'db-light' if args.type == 'light' else 'db'}.tar.gz"
-        print(f"download database: v{required_version['major']}.{required_version['minor']}, type={db_old_info['type']}, {required_version['date']}, DOI: {required_version['doi']}, URL: {db_url}...")
+        print(f"Download database: v{required_version['major']}.{required_version['minor']}, type={db_old_info['type']}, {required_version['date']}, DOI: {required_version['doi']}, URL: {db_url}...")
         download(db_url, tarball_path)
         print('\t... done')
 
-        print('check MD5 sum...')
+        print('Check MD5 sum...')
         md5_sum = calc_md5_sum(tarball_path)
         required_md5 = required_version['md5-light' if args.type == 'light' else 'md5']
         if(md5_sum == required_md5):
             print(f'\t...database file OK: {md5_sum}')
         else:
             sys.exit(f"Error: corrupt database file! MD5 should be '{required_md5}' but is '{md5_sum}'")
 
-        print(f'extract DB tarball: file={tarball_path}, output-directory={tmp_path}')
+        print(f'Extract DB tarball: file={tarball_path}, output-directory={tmp_path}')
         untar(tarball_path, tmp_path)
         tarball_path.unlink()
 
         db_new_path = tmp_path.joinpath('db-light' if args.type == 'light' else 'db')
         db_new_info = check(db_new_path)
         if(db_new_info['major'] != required_version['major']):
             sys.exit(f"ERROR: wrong major db detected! required={required_version['major']}, detected={db_new_info['major']}")
         elif(db_new_info['minor'] != required_version['minor']):
             sys.exit(f"ERROR: wrong minor db detected! required={required_version['minor']}, detected={db_new_info['minor']}")
         elif(db_new_info['type'] != args.type == 'light'):
             sys.exit(f"ERROR: wrong db type detected! required={args.type}, detected={db_new_info['type']}")
-        print('successfully downloaded Bakta DB:')
+        print('Successfully downloaded Bakta DB:')
         print(f"\tversion: {required_version['major']}.{required_version['minor']}")
         print(f"\tType: {args.type}")
         print(f"\tDOI: {required_version['doi']}")
         print(f'\tpath: {db_new_path}')
-        print('remove old database...')
+        print('Remove old database...')
         try:
             db_old_path.chmod(stat.S_IRUSR | stat.S_IWUSR | stat.S_IXUSR)  # set write permissions on old directory
             for db_old_file_path in db_old_path.iterdir():
                 if(db_old_file_path.is_dir()):
                     db_old_file_path.chmod(stat.S_IRUSR | stat.S_IWUSR | stat.S_IXUSR)
                 else:    
                     db_old_file_path.chmod(stat.S_IRUSR | stat.S_IWUSR)
@@ -327,15 +332,15 @@
             for db_old_file_path in db_old_path.iterdir():
                 db_old_file_path.chmod(stat.S_IRUSR | stat.S_IRGRP | stat.S_IROTH)
         except:
             sys.exit(f'ERROR: cannot set read(|execute) permissions on new database! path={db_old_path}, owner={db_old_path.owner()}, group={db_old_path.group()}, permissions={oct(db_old_path.stat().st_mode )[-3:]}')
 
         print('\t... done')
 
-        print('update AMRFinderPlus database...')
+        print('Update AMRFinderPlus database...')
         update_amrfinderplus_db(db_old_path)
         print('\t... done')
 
         print(f"\nRun Bakta using '--db {db_old_path}' or set a BAKTA_DB environment variable: 'export BAKTA_DB={db_old_path}'")
     else:
         parser.print_help()
         sys.exit('Error: no subcommand provided!')
```

### Comparing `bakta-1.7.0/bakta/expert/amrfinder.py` & `bakta-1.8.0/bakta/expert/amrfinder.py`

 * *Files identical despite different names*

### Comparing `bakta-1.7.0/bakta/expert/protein_sequences.py` & `bakta-1.8.0/bakta/expert/protein_sequences.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,23 +21,21 @@
     diamond_output_path = cfg.tmp_path.joinpath('diamond.cds.expert.tsv')
     cmd = [
         'diamond',
         'blastp',
         '--query', str(cds_fasta_path),
         '--db', str(db_path),
         '--out', str(diamond_output_path),
-        '--id', str(50),  # '50',
-        '--query-cover', str(80),  # '80'
-        '--subject-cover', str(80),  # '80'
         '--max-target-seqs', '1',  # single best output
         '--outfmt', '6', 'qseqid', 'sseqid', 'slen', 'length', 'pident', 'evalue', 'bitscore', 'stitle',
         '--threads', str(cfg.threads),
         '--tmpdir', str(cfg.tmp_path),  # use tmp folder
         '--block-size', '4',  # increase block size for faster executions
-        '--index-chunks', '1'  # set index chunks to 1 for faster executions
+        '--index-chunks', '1',  # set index chunks to 1 for faster executions
+        '--sensitive'
     ]
     log.debug('cmd=%s', cmd)
     proc = sp.run(
         cmd,
         cwd=str(cfg.tmp_path),
         env=cfg.env,
         stdout=sp.PIPE,
```

### Comparing `bakta-1.7.0/bakta/features/annotation.py` & `bakta-1.8.0/bakta/features/annotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,19 +18,19 @@
 RE_PROTEIN_PUTATIVE = re.compile(r'(potential|possible|probable|predicted)', flags=re.IGNORECASE)
 RE_PROTEIN_NODE = re.compile(r'NODE_', flags=re.IGNORECASE)
 RE_PROTEIN_POTENTIAL_CONTIG_NAME = re.compile(r'(genome|shotgun)', flags=re.IGNORECASE)
 RE_PROTEIN_DOMAIN_CONTAINING = re.compile(r'domain-containing protein', flags=re.IGNORECASE)
 RE_PROTEIN_NO_LETTERS = re.compile(r'[^A-Za-z]')
 RE_PROTEIN_SUSPECT_CHARS = re.compile(r'[.@=?%]')
 RE_PROTEIN_PERIOD_SEPARATOR = re.compile(r'([a-zA-Z0-9]+)\.([a-zA-Z0-9]+)')
-RE_DOMAIN_OF_UNKNOWN_FUCTION = re.compile(r'(DUF\d{3,4})', flags=re.IGNORECASE)
-RE_UNCHARACTERIZED_PROTEIN_FAMILY = re.compile(r'(UPF\d{3,4})', flags=re.IGNORECASE)
+RE_PROTEIN_WRONG_PRIMES = re.compile(r'[\u2032\u0060\u00B4]')  # prime (′), grave accent (`), acute accent (´)
 RE_PROTEIN_WEIGHT = re.compile(r' [0-9]+(?:\.[0-9]+)? k?da ', flags=re.IGNORECASE)
 RE_PROTEIN_SYMBOL = re.compile(r'[A-Z][a-z]{2}[A-Z][0-9]?')
-
+RE_DOMAIN_OF_UNKNOWN_FUCTION = re.compile(r'(DUF\d{3,4})', flags=re.IGNORECASE)
+RE_UNCHARACTERIZED_PROTEIN_FAMILY = re.compile(r'(UPF\d{3,4})', flags=re.IGNORECASE)
 RE_GENE_CAPITALIZED = re.compile(r'^[A-Z].+', flags=re.DOTALL)
 RE_GENE_SUSPECT_CHARS = re.compile(r'[\?]', flags=re.DOTALL)
 RE_GENE_SYMBOL = re.compile(r'[a-z]{3}[A-Z][0-9]?')
 
 
 def combine_annotation(feature: dict):
     pseudogene_psc = None
@@ -489,15 +489,20 @@
     product = re.sub(RE_PROTEIN_PERIOD_SEPARATOR, r'\1-\2', product)  # replace separator periods
     if(product != old_product):
         log.info('fix product: replace separator periods. new=%s, old=%s', product, old_product)
 
     old_product = product
     product = RE_PROTEIN_SUSPECT_CHARS.sub('', product)  # remove suspect characters
     if(product != old_product):
-        log.info('fix product: replace invalid characters (.@=?%%). new=%s, old=%s', product, old_product)
+        log.info('fix product: replace invalid characters. new=%s, old=%s', product, old_product)
+
+    old_product = product
+    product = RE_PROTEIN_WRONG_PRIMES.sub('\u0027', product)  # replace wrong prime characters with single quote (U+0027) (') according to https://www.ncbi.nlm.nih.gov/genome/doc/internatprot_nomenguide/
+    if(product != old_product):
+        log.info('fix product: replace wrong prime characters. new=%s, old=%s', product, old_product)
 
     old_product = product
     product = product.replace('FOG:', '')  # remove FOG ids
     if(product != old_product):
         log.info('fix product: replace FOG ids. new=%s, old=%s', product, old_product)
 
     old_product = product
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bakta-1.7.0/bakta/features/cds.py` & `bakta-1.8.0/bakta/features/cds.py`

 * *Files identical despite different names*

### Comparing `bakta-1.7.0/bakta/features/crispr.py` & `bakta-1.8.0/bakta/features/crispr.py`

 * *Files identical despite different names*

### Comparing `bakta-1.7.0/bakta/features/gaps.py` & `bakta-1.8.0/bakta/features/gaps.py`

 * *Files identical despite different names*

### Comparing `bakta-1.7.0/bakta/features/nc_rna.py` & `bakta-1.8.0/bakta/features/nc_rna.py`

 * *Files identical despite different names*

### Comparing `bakta-1.7.0/bakta/features/nc_rna_region.py` & `bakta-1.8.0/bakta/features/nc_rna_region.py`

 * *Files identical despite different names*

### Comparing `bakta-1.7.0/bakta/features/orf.py` & `bakta-1.8.0/bakta/features/orf.py`

 * *Files identical despite different names*

### Comparing `bakta-1.7.0/bakta/features/ori.py` & `bakta-1.8.0/bakta/features/ori.py`

 * *Files identical despite different names*

### Comparing `bakta-1.7.0/bakta/features/r_rna.py` & `bakta-1.8.0/bakta/features/r_rna.py`

 * *Files identical despite different names*

### Comparing `bakta-1.7.0/bakta/features/s_orf.py` & `bakta-1.8.0/bakta/features/s_orf.py`

 * *Files identical despite different names*

### Comparing `bakta-1.7.0/bakta/features/signal_peptides.py` & `bakta-1.8.0/bakta/features/signal_peptides.py`

 * *Files identical despite different names*

### Comparing `bakta-1.7.0/bakta/features/t_rna.py` & `bakta-1.8.0/bakta/features/t_rna.py`

 * *Files identical despite different names*

### Comparing `bakta-1.7.0/bakta/features/tm_rna.py` & `bakta-1.8.0/bakta/features/tm_rna.py`

 * *Files identical despite different names*

### Comparing `bakta-1.7.0/bakta/io/fasta.py` & `bakta-1.8.0/bakta/io/fasta.py`

 * *Files identical despite different names*

### Comparing `bakta-1.7.0/bakta/io/gff.py` & `bakta-1.8.0/bakta/io/gff.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         fh.write('##feature-ontology https://github.com/The-Sequence-Ontology/SO-Ontologies/blob/v3.1/so.obo\n')  # SO feature version
 
         if(genome['taxon']):  # write organism info
             fh.write(f"# organism {genome['taxon']}\n")
 
         fh.write('# Annotated with Bakta\n')
         fh.write(f'# Software: v{bakta.__version__}\n')
-        fh.write(f"# Database: v{cfg.db_info['major']}.{cfg.db_info['minor']}\n")
+        fh.write(f"# Database: v{cfg.db_info['major']}.{cfg.db_info['minor']}, {cfg.db_info['type']}\n")
         fh.write(f'# DOI: {bc.BAKTA_DOI}\n')
         fh.write(f'# URL: {bc.BAKTA_URL}\n')
 
         for contig in genome['contigs']:  # write features
             fh.write(f"##sequence-region {contig['id']} 1 {contig['length']}\n")  # sequence region
 
             # write landmark region
```

### Comparing `bakta-1.7.0/bakta/io/insdc.py` & `bakta-1.8.0/bakta/io/insdc.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,23 +23,20 @@
 
     contig_list = []
     for contig in genome['contigs']:
         contig_features = [feat for feat in features if feat['contig'] == contig['id']]
         comment = (
             'Annotated with Bakta',
             f"Software: v{bakta.__version__}\n",
-            f"Database: v{cfg.db_info['major']}.{cfg.db_info['minor']}\n",
+            f"Database: v{cfg.db_info['major']}.{cfg.db_info['minor']}, {cfg.db_info['type']}\n",
             f'DOI: {bc.BAKTA_DOI}\n',
             f'URL: {bc.BAKTA_URL}\n',
             '\n',
             '##Genome Annotation Summary:##\n',
             f"{'Annotation Date':<30} :: {datetime.now().strftime('%m/%d/%Y, %H:%M:%S')}\n",
-            f"{'Annotation Pipeline':<30} :: Bakta\n",
-            f"{'Annotation Software version':<30} ::  v{bakta.__version__}\n",
-            f"{'Annotation Database version':<30} ::  v{cfg.db_info['major']}.{cfg.db_info['minor']}\n",
             f"{'CDSs':<30} :: {len([feat for feat in contig_features if feat['type'] == bc.FEATURE_CDS or feat['type'] == bc.FEATURE_SORF]):5,}\n",
             f"{'tRNAs':<30} :: {len([feat for feat in contig_features if feat['type'] == bc.FEATURE_T_RNA]):5,}\n",
             f"{'tmRNAs':<30} :: {len([feat for feat in contig_features if feat['type'] == bc.FEATURE_TM_RNA]):5,}\n",
             f"{'rRNAs':<30} :: {len([feat for feat in contig_features if feat['type'] == bc.FEATURE_R_RNA]):5,}\n",
             f"{'ncRNAs':<30} :: {len([feat for feat in contig_features if feat['type'] == bc.FEATURE_NC_RNA]):5,}\n",
             f"{'regulatory ncRNAs':<30} :: {len([feat for feat in contig_features if feat['type'] == bc.FEATURE_NC_RNA_REGION]):5,}\n",
             f"{'CRISPR Arrays':<30} :: {len([feat for feat in contig_features if feat['type'] == bc.FEATURE_CRISPR]):5,}",
```

### Comparing `bakta-1.7.0/bakta/io/json.py` & `bakta-1.8.0/bakta/io/json.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,42 +29,47 @@
             # remove redundant PSC Dbxrefs
             psc = feat.get('psc', None)
             if(psc):
                 psc.pop('db_xrefs')
 
     # replace features type dict by sorted feature list
     output = OrderedDict()
-    ordered_genome = OrderedDict()
-    ordered_genome['genus'] = genome['genus']
-    ordered_genome['species'] = genome['species']
-    ordered_genome['strain'] = genome['strain']
-    if('plasmid' in genome):
-        ordered_genome['plasmid'] = genome['plasmid']
-    ordered_genome['complete'] = genome['complete']
-    ordered_genome['gram'] = genome['gram']
-    ordered_genome['translation_table'] = genome['translation_table']
-    output['genome'] = ordered_genome
-
-    stats = OrderedDict()
-    stats['no_sequences'] = len(genome['contigs'])
-    stats['size'] = genome['size']
-    stats['gc'] = genome['gc']
-    stats['n_ratio'] = genome['n_ratio']
-    stats['n50'] = genome['n50']
-    stats['coding_ratio'] = genome['coding_ratio']
-    output['stats'] = stats
+    if genome is not None:
+        ordered_genome = OrderedDict()
+        ordered_genome['genus'] = genome['genus']
+        ordered_genome['species'] = genome['species']
+        ordered_genome['strain'] = genome['strain']
+        if('plasmid' in genome):
+            ordered_genome['plasmid'] = genome['plasmid']
+        ordered_genome['complete'] = genome['complete']
+        ordered_genome['gram'] = genome['gram']
+        ordered_genome['translation_table'] = genome['translation_table']
+        output['genome'] = ordered_genome
+
+        stats = OrderedDict()
+        stats['no_sequences'] = len(genome['contigs'])
+        stats['size'] = genome['size']
+        stats['gc'] = genome['gc']
+        stats['n_ratio'] = genome['n_ratio']
+        stats['n50'] = genome['n50']
+        stats['coding_ratio'] = genome['coding_ratio']
+        output['stats'] = stats
 
     output['features'] = features
-    output['sequences'] = genome['contigs']
+    if genome is not None:
+        output['sequences'] = genome['contigs']
 
     run = OrderedDict()
     run['start'] = cfg.run_start.strftime('%Y-%m-%d %H:%M:%S')
     run['end'] = cfg.run_end.strftime('%Y-%m-%d %H:%M:%S')
     output['run'] = run
 
     version = OrderedDict()
     version['bakta'] = bakta.__version__
-    version['db'] = f"{cfg.db_info['major']}.{cfg.db_info['minor']}"
+    version['db'] = {
+        'version': f"{cfg.db_info['major']}.{cfg.db_info['minor']}",
+        'type': cfg.db_info['type']
+    }
     output['version'] = version
 
     with json_path.open('wt') as fh:
         json.dump(output, fh, indent=4)
```

### Comparing `bakta-1.7.0/bakta/io/tsv.py` & `bakta-1.8.0/bakta/io/tsv.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,17 +13,21 @@
 
 
 def write_tsv(contigs: Sequence[dict], features_by_contig: Dict[str, dict], tsv_path: Path):
     """Export features in TSV format."""
     log.info('write tsv: path=%s', tsv_path)
 
     with tsv_path.open('wt') as fh:
-        fh.write(f'#Annotated with Bakta (v{bakta.__version__}): https://github.com/oschwengers/bakta\n')
-        fh.write(f"#Database (v{cfg.db_info['major']}.{cfg.db_info['minor']}): https://doi.org/10.5281/zenodo.4247252\n")
+        fh.write('# Annotated with Bakta\n')
+        fh.write(f'# Software: v{bakta.__version__}\n')
+        fh.write(f"# Database: v{cfg.db_info['major']}.{cfg.db_info['minor']}, {cfg.db_info['type']}\n")
+        fh.write(f'# DOI: {bc.BAKTA_DOI}\n')
+        fh.write(f'# URL: {bc.BAKTA_URL}\n')
         fh.write('#Sequence Id\tType\tStart\tStop\tStrand\tLocus Tag\tGene\tProduct\tDbXrefs\n')
+
         for contig in contigs:
             for feat in features_by_contig[contig['id']]:
                 feat_type = feat['type']
                 if(feat['type'] == bc.FEATURE_GAP):
                     feat_type = bc.INSDC_FEATURE_ASSEMBLY_GAP if feat['length'] >= 100 else bc.INSDC_FEATURE_GAP
 
                 gene = feat['gene'] if feat.get('gene', None) else ''
```

### Comparing `bakta-1.7.0/bakta/ips.py` & `bakta-1.8.0/bakta/ips.py`

 * *Files identical despite different names*

### Comparing `bakta-1.7.0/bakta/main.py` & `bakta-1.8.0/bakta/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 def main():
     args = bu.parse_arguments()  # parse arguments
 
     ############################################################################
     # Setup logging
     ############################################################################
     cfg.prefix = args.prefix if args.prefix else Path(args.genome).stem
-    output_path = cfg.check_output_path(args)
+    output_path = cfg.check_output_path(args.output, args.force)
     bu.setup_logger(output_path, cfg.prefix, args)
     log = logging.getLogger('MAIN')
 
     ############################################################################
     # Checks and configurations
     # - check parameters and setup global configuration
     # - test database
@@ -58,30 +58,32 @@
     bu.test_dependencies()
     if(cfg.verbose):
         print(f'Bakta v{bakta.__version__}')
         print('Options and arguments:')
         print(f'\tinput: {cfg.genome_path}')
         print(f"\tdb: {cfg.db_path}, version {cfg.db_info['major']}.{cfg.db_info['minor']}, {cfg.db_info['type']}")
         if(cfg.user_proteins): print(f'\tuser proteins: {cfg.user_proteins}')
+        if(cfg.replicons): print(f'\treplicon table: {cfg.replicons}')
+        if(cfg.prodigal_tf): print(f'\tprodigal training file: {cfg.prodigal_tf}')
         print(f'\toutput: {cfg.output_path}')
+        if(cfg.force): print(f'\tforce: {cfg.force}')
         print(f'\ttmp directory: {cfg.tmp_path}')
         print(f'\tprefix: {cfg.prefix}')
         print(f'\tthreads: {cfg.threads}')
         if(cfg.debug): print(f'\tdebug: {cfg.debug}')
-        if(cfg.complete): print(f'\tcomplete replicons: {cfg.complete}')
-        if(cfg.compliant): print(f'\tINSDC compliant: {cfg.compliant}')
-        if(cfg.keep_contig_headers): print(f'\tkeep contig headers: {cfg.keep_contig_headers}')
-        if(cfg.replicons): print(f'\treplicon table: {cfg.replicons}')
-        if(cfg.prodigal_tf): print(f'\tprodigal training file: {cfg.prodigal_tf}')
         if(cfg.meta): print(f'\tmeta mode: {cfg.meta}')
         print(f'\ttranslation table: {cfg.translation_table}')
         if(cfg.taxon): print(f'\ttaxon: {cfg.taxon}')
+        if(cfg.plasmid): print(f'\tplasmid: {cfg.plasmid}')
         if(cfg.gram != '?'): print(f'\tgram: {cfg.gram}')
         if(cfg.locus): print(f'\tlocus prefix: {cfg.locus}')
         if(cfg.locus_tag): print(f'\tlocus tag prefix: {cfg.locus_tag}')
+        if(cfg.complete): print(f'\tcomplete replicons: {cfg.complete}')
+        if(cfg.compliant): print(f'\tINSDC compliant: {cfg.compliant}')
+        if(cfg.keep_contig_headers): print(f'\tkeep contig headers: {cfg.keep_contig_headers}')
         if(cfg.skip_trna): print(f'\tskip tRNA: {cfg.skip_trna}')
         if(cfg.skip_tmrna): print(f'\tskip tmRNA: {cfg.skip_tmrna}')
         if(cfg.skip_rrna): print(f'\tskip rRNA: {cfg.skip_rrna}')
         if(cfg.skip_ncrna): print(f'\tskip ncRNA: {cfg.skip_ncrna}')
         if(cfg.skip_ncrna_region): print(f'\tskip ncRNA region: {cfg.skip_ncrna_region}')
         if(cfg.skip_crispr): print(f'\tskip CRISPR: {cfg.skip_crispr}')
         if(cfg.skip_cds): print(f'\tskip CDS: {cfg.skip_cds}')
@@ -597,15 +599,15 @@
         fh_out.write(f"sORFs: {len([f for f in features if f['type'] == bc.FEATURE_SORF])}\n")
         fh_out.write(f"gaps: {len([f for f in features if f['type'] == bc.FEATURE_GAP])}\n")
         fh_out.write(f"oriCs: {len([f for f in features if f['type'] == bc.FEATURE_ORIC])}\n")
         fh_out.write(f"oriVs: {len([f for f in features if f['type'] == bc.FEATURE_ORIV])}\n")
         fh_out.write(f"oriTs: {len([f for f in features if f['type'] == bc.FEATURE_ORIT])}\n")
         fh_out.write('\nBakta:\n')
         fh_out.write(f'Software: v{bakta.__version__}\n')
-        fh_out.write(f"Database: v{cfg.db_info['major']}.{cfg.db_info['minor']}\n")
+        fh_out.write(f"Database: v{cfg.db_info['major']}.{cfg.db_info['minor']}, {cfg.db_info['type']}\n")
         fh_out.write('DOI: 10.1099/mgen.0.000685\n')
         fh_out.write('URL: github.com/oschwengers/bakta\n')
 
     print(f'\nIf you use these results please cite Bakta: https://doi.org/{bc.BAKTA_DOI}')
     print(f'Annotation successfully finished in {int(run_duration / 60):01}:{int(run_duration % 60):02} [mm:ss].')
```

### Comparing `bakta-1.7.0/bakta/plot.py` & `bakta-1.8.0/bakta/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
     parser = bu.init_parser(sub_command='_plot')
     parser.add_argument('input', metavar='<input>', help='Bakta annotations in JSON format')
     
     arg_group_io = parser.add_argument_group('Input / Output')
     arg_group_io.add_argument('--config', '-c', action='store', default=None, help='Plotting configuration in YAML format')
     arg_group_io.add_argument('--output', '-o', action='store', default=os.getcwd(), help='Output directory (default = current working directory)')
     arg_group_io.add_argument('--prefix', '-p', action='store', default=None, help='Prefix for output files')
+    arg_group_io.add_argument('--force', '-f', action='store_true', help='Force overwriting existing output folder')
 
     arg_group_plot = parser.add_argument_group('Plotting')
     arg_group_plot.add_argument('--sequences', action='store', default='all', help='Sequences to plot: comma separated number or name (default = all, numbers one-based)')
     arg_group_plot.add_argument('--type', action='store', type=str, default=bc.PLOT_FEATURES, choices=[bc.PLOT_FEATURES, bc.PLOT_COG], help=f'Plot type (default = {bc.PLOT_FEATURES})')
 
     arg_group_general = parser.add_argument_group('General')
     arg_group_general.add_argument('--help', '-h', action='help', help='Show this help message and exit')
@@ -91,15 +92,17 @@
     arg_group_general.add_argument('--version', action='version', version=f'%(prog)s {bakta.__version__}')
     args = parser.parse_args()
 
     ############################################################################
     # Setup logging
     ############################################################################
     cfg.prefix = args.prefix if args.prefix else Path(args.input).stem
-    output_path = cfg.check_output_path(args)
+    output_path = cfg.check_output_path(args.output, args.force)
+    cfg.force = args.force
+    log.info('force=%s', args.force)
     
     bu.setup_logger(output_path, cfg.prefix, args)
     log.info('prefix=%s', cfg.prefix)
     log.info('output=%s', output_path)
 
     
     ############################################################################
@@ -145,16 +148,17 @@
     bu.test_dependencies()
     if(cfg.verbose):
         print(f'Bakta v{bakta.__version__}')
         print('Options and arguments:')
         print(f'\tinput: {annotation_path}')
         if(args.config): print(f'\tconfig: {args.config}')
         print(f'\toutput: {cfg.output_path}')
-        print(f'\tprefix: {cfg.prefix}')
+        if(cfg.force): print(f'\tforce: {cfg.force}')
         print(f'\ttmp directory: {cfg.tmp_path}')
+        print(f'\tprefix: {cfg.prefix}')
 
     if(cfg.debug):
         print(f"\nBakta runs in DEBUG mode! Temporary data will not be destroyed at: {cfg.tmp_path}")
     else:
         atexit.register(bu.cleanup, log, cfg.tmp_path)  # register cleanup exit hook
 
     ############################################################################
```

### Comparing `bakta-1.7.0/bakta/proteins.py` & `bakta-1.8.0/bakta/proteins.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import atexit
 import logging
 import os
 import sys
 
+from datetime import datetime
 from typing import Sequence
 from pathlib import Path
 
 import bakta
 import bakta.constants as bc
 import bakta.config as cfg
 import bakta.db as db
 import bakta.utils as bu
 import bakta.expert.amrfinder as exp_amr
 import bakta.expert.protein_sequences as exp_aa_seq
 import bakta.features.annotation as anno
 import bakta.features.orf as orf
 import bakta.features.cds as feat_cds
 import bakta.io.fasta as fasta
+import bakta.io.json as json
 import bakta.io.tsv as tsv
 import bakta.ups as ups
 import bakta.ips as ips
 import bakta.psc as psc
 import bakta.pscc as pscc
 
 
@@ -32,14 +34,15 @@
     parser = bu.init_parser(sub_command='_proteins')
     parser.add_argument('input', metavar='<input>', help='Protein sequences in (zipped) fasta format')
     
     arg_group_io = parser.add_argument_group('Input / Output')
     arg_group_io.add_argument('--db', '-d', action='store', default=None, help='Database path (default = <bakta_path>/db). Can also be provided as BAKTA_DB environment variable.')
     arg_group_io.add_argument('--output', '-o', action='store', default=os.getcwd(), help='Output directory (default = current working directory)')
     arg_group_io.add_argument('--prefix', '-p', action='store', default=None, help='Prefix for output files')
+    arg_group_io.add_argument('--force', '-f', action='store_true', help='Force overwriting existing output folder')
     
     arg_group_annotation = parser.add_argument_group('Annotation')
     arg_group_annotation.add_argument('--proteins', action='store', default=None, dest='proteins', help='Fasta file of trusted protein sequences for annotation')
     
     arg_group_general = parser.add_argument_group('General')
     arg_group_general.add_argument('--help', '-h', action='help', help='Show this help message and exit')
     arg_group_general.add_argument('--verbose', '-v', action='store_true', help='Print verbose information')
@@ -49,15 +52,17 @@
     arg_group_general.add_argument('--version', '-V', action='version', version=f'%(prog)s {bakta.__version__}')
     args = parser.parse_args()
 
     ############################################################################
     # Setup logging
     ############################################################################
     cfg.prefix = args.prefix if args.prefix else Path(args.input).stem
-    output_path = cfg.check_output_path(args)
+    output_path = cfg.check_output_path(args.output, args.force)
+    cfg.force = args.force
+    log.info('force=%s', args.force)
     
     bu.setup_logger(output_path, cfg.prefix, args)
     log.info('prefix=%s', cfg.prefix)
     log.info('output=%s', output_path)
 
     ############################################################################
     # Checks and configurations
@@ -90,16 +95,17 @@
     bu.test_dependencies()
     if(cfg.verbose):
         print(f'Bakta v{bakta.__version__}')
         print('Options and arguments:')
         print(f'\tinput: {aa_path}')
         print(f"\tdb: {cfg.db_path}, version {cfg.db_info['major']}.{cfg.db_info['minor']}")
         print(f'\toutput: {cfg.output_path}')
-        print(f'\tprefix: {cfg.prefix}')
+        if(cfg.force): print(f'\tforce: {cfg.force}')
         print(f'\ttmp directory: {cfg.tmp_path}')
+        print(f'\tprefix: {cfg.prefix}')
         print(f'\t# threads: {cfg.threads}')
     
     if(cfg.debug):
         print(f"\nBakta runs in DEBUG mode! Temporary data will not be destroyed at: {cfg.tmp_path}")
     else:
         atexit.register(bu.cleanup, log, cfg.tmp_path)  # register cleanup exit hook
 
@@ -122,29 +128,52 @@
         aa['start'] = mock_start
         aa['stop'] = -1
         aa['strand'] = bc.STRAND_UNKNOWN
         aa['frame'] = 1
         mock_start += 100
     print('annotate protein sequences...')
     annotate_aa(aas)
-    
+
+    for aa in aas:  # cleanup mock attributes
+        aa.pop('contig', None)
+        aa.pop('start', None)
+        aa.pop('stop', None)
+        aa.pop('strand', None)
+        aa.pop('frame', None)
+    
+    cfg.run_end = datetime.now()
+    run_duration = (cfg.run_end - cfg.run_start).total_seconds()
+
+    ############################################################################
+    # Write output files
+    # - write comprehensive annotation results as JSON
+    # - write optional output files in TSV, FAA formats
+    # - remove temp directory
+    ############################################################################
+
     print('write results...')
     annotations_path = output_path.joinpath(f'{cfg.prefix}.tsv')
     header_columns = ['ID', 'Length', 'Gene', 'Product', 'EC', 'GO', 'COG', 'RefSeq', 'UniParc', 'UniRef']
     print(f'\tfull annotations (TSV): {annotations_path}')
     tsv.write_features(aas, header_columns, map_aa_columns, annotations_path)
+    full_annotations_path = output_path.joinpath(f'{cfg.prefix}.json')
+    print(f'\tfull annotations (JSON): {full_annotations_path}')
+    json.write_json(None, aas, full_annotations_path)
     hypotheticals_path = output_path.joinpath(f'{cfg.prefix}.hypotheticals.tsv')
     header_columns = ['ID', 'Length', 'Mol Weight [kDa]', 'Iso El. Point', 'Pfam hits']
     hypotheticals = hypotheticals = [aa for aa in aas if 'hypothetical' in aa]
     print(f'\tinformation on hypotheticals (TSV): {hypotheticals_path}')
     tsv.write_features(hypotheticals, header_columns, map_hypothetical_columns, hypotheticals_path)
     aa_output_path = output_path.joinpath(f'{cfg.prefix}.faa')
     print(f'\tannotated sequences (Fasta): {aa_output_path}')
     fasta.write_faa(aas, aa_output_path)
 
+    print(f'\nIf you use these results please cite Bakta: https://doi.org/{bc.BAKTA_DOI}')
+    print(f'Annotation successfully finished in {int(run_duration / 60):01}:{int(run_duration % 60):02} [mm:ss].')
+
 
 def map_aa_columns(feat: dict) -> Sequence[str]:
     gene = feat.get('gene', None)
     if(gene is None):
         gene = ''
     return [
         feat['id'],
```

### Comparing `bakta-1.7.0/bakta/psc.py` & `bakta-1.8.0/bakta/psc.py`

 * *Files identical despite different names*

### Comparing `bakta-1.7.0/bakta/pscc.py` & `bakta-1.8.0/bakta/pscc.py`

 * *Files identical despite different names*

### Comparing `bakta-1.7.0/bakta/so.py` & `bakta-1.8.0/bakta/so.py`

 * *Files identical despite different names*

### Comparing `bakta-1.7.0/bakta/ups.py` & `bakta-1.8.0/bakta/ups.py`

 * *Files identical despite different names*

### Comparing `bakta-1.7.0/bakta/utils.py` & `bakta-1.8.0/bakta/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,23 +34,23 @@
 
 
 VERSION_MIN_DIGIT = -1
 VERSION_MAX_DIGIT = 1000000000000
 VERSION_REGEX = re.compile(r'(\d+)\.(\d+)(?:[\.-](\d+))?')  # regex to search for version number in tool output. Takes missing patch version into consideration.
 
 # List of dependencies: tuples for: min version, max version, tool name & command line parameter, dependency check exclusion options
-DEPENDENCY_TRNASCAN = (Version(2, 0, 8), Version(VERSION_MAX_DIGIT, VERSION_MAX_DIGIT, VERSION_MAX_DIGIT), VERSION_REGEX, ('tRNAscan-SE', '-h'), ['--skip-trna'])
-DEPENDENCY_ARAGORN = (Version(1, 2, 38), Version(VERSION_MAX_DIGIT, VERSION_MAX_DIGIT, VERSION_MAX_DIGIT), VERSION_REGEX, ('aragorn', '-h'), ['skip-tmrna'])
+DEPENDENCY_TRNASCAN = (Version(2, 0, 11), Version(VERSION_MAX_DIGIT, VERSION_MAX_DIGIT, VERSION_MAX_DIGIT), VERSION_REGEX, ('tRNAscan-SE', '-h'), ['--skip-trna'])
+DEPENDENCY_ARAGORN = (Version(1, 2, 41), Version(VERSION_MAX_DIGIT, VERSION_MAX_DIGIT, VERSION_MAX_DIGIT), VERSION_REGEX, ('aragorn', '-h'), ['skip-tmrna'])
 DEPENDENCY_CMSCAN = (Version(1, 1, 4), Version(VERSION_MAX_DIGIT, VERSION_MAX_DIGIT, VERSION_MAX_DIGIT), VERSION_REGEX, ('cmscan', '-h'), ['--skip-rrna', '--skip-ncrna', '--skip-ncrna-region'])
 DEPENDENCY_PILERCR = (Version(1, 6), Version(VERSION_MAX_DIGIT, VERSION_MAX_DIGIT, VERSION_MAX_DIGIT), VERSION_REGEX, ('pilercr', '-options'), ['--skip-crispr'])
 DEPENDENCY_HMMSEARCH = (Version(3, 3, 2), Version(VERSION_MAX_DIGIT, VERSION_MAX_DIGIT, VERSION_MAX_DIGIT), VERSION_REGEX, ('hmmsearch', '-h'), ['--skip-cds', '--skip-sorf'])
 DEPENDENCY_DIAMOND = (Version(2, 0, 14), Version(VERSION_MAX_DIGIT, VERSION_MAX_DIGIT, VERSION_MAX_DIGIT), VERSION_REGEX, ('diamond', 'help'), ['--skip-cds', '--skip-sorf'])
 DEPENDENCY_DEEPSIG = (Version(1, 2, 5), Version(VERSION_MAX_DIGIT, VERSION_MAX_DIGIT, VERSION_MAX_DIGIT), VERSION_REGEX, ('deepsig', '--version'), ['--gram ?'])
 DEPENDENCY_BLASTN = (Version(2, 12, 0), Version(VERSION_MAX_DIGIT, VERSION_MAX_DIGIT, VERSION_MAX_DIGIT), VERSION_REGEX, ('blastn', '-version'), ['--skip-ori'])
-DEPENDENCY_AMRFINDERPLUS = (Version(3, 10, 23), Version(VERSION_MAX_DIGIT, VERSION_MAX_DIGIT, VERSION_MAX_DIGIT), VERSION_REGEX, ('amrfinder', '--version'), ['--skip-cds'])
+DEPENDENCY_AMRFINDERPLUS = (Version(3, 11, 2), Version(VERSION_MAX_DIGIT, VERSION_MAX_DIGIT, VERSION_MAX_DIGIT), VERSION_REGEX, ('amrfinder', '--version'), ['--skip-cds'])
 DEPENDENCY_CIRCOS = (Version(0, 69, 8), Version(VERSION_MAX_DIGIT, VERSION_MAX_DIGIT, VERSION_MAX_DIGIT), VERSION_REGEX, ('circos', '--version'), ['--skip-plot'])
 
 
 def init_parser(sub_command: str=''):
     parser = argparse.ArgumentParser(
         prog=f'bakta{sub_command}',
         description='Rapid & standardized annotation of bacterial genomes, MAGs & plasmids',
@@ -66,14 +66,15 @@
     parser.add_argument('genome', metavar='<genome>', help='Genome sequences in (zipped) fasta format')
 
     arg_group_io = parser.add_argument_group('Input / Output')
     arg_group_io.add_argument('--db', '-d', action='store', default=None, help='Database path (default = <bakta_path>/db). Can also be provided as BAKTA_DB environment variable.')
     arg_group_io.add_argument('--min-contig-length', '-m', action='store', type=int, default=1, dest='min_contig_length', help='Minimum contig size (default = 1; 200 in compliant mode)')
     arg_group_io.add_argument('--prefix', '-p', action='store', default=None, help='Prefix for output files')
     arg_group_io.add_argument('--output', '-o', action='store', default=os.getcwd(), help='Output directory (default = current working directory)')
+    arg_group_io.add_argument('--force', '-f', action='store_true', help='Force overwriting existing output folder')
 
     arg_group_organism = parser.add_argument_group('Organism')
     arg_group_organism.add_argument('--genus', action='store', default=None, help='Genus name')
     arg_group_organism.add_argument('--species', action='store', default=None, help='Species name')
     arg_group_organism.add_argument('--strain', action='store', default=None, help='Strain name')
     arg_group_organism.add_argument('--plasmid', action='store', default=None, help='Plasmid name')
 
@@ -380,16 +381,14 @@
     return replicons
 
 
 def qc_contigs(contigs: Sequence[dict], replicons: Dict[str, dict]) -> Tuple[Sequence[dict], bool]:
     valid_contigs = []
     contig_counter = 1
     contig_prefix = cfg.locus if cfg.locus else 'contig'
-    organism_definition = f"[organism={cfg.taxon}]" if cfg.taxon else None
-
     complete_genome = True
     plasmid_number = 1
     contig_ids = set()
     for contig in contigs:
         if(contig['length'] >= cfg.min_contig_length):
             contig_id_generated = f'{contig_prefix}_{contig_counter}'
             contig['simple_id'] = contig_id_generated
@@ -411,73 +410,72 @@
             if('chromosome' in contig_description):
                 contig['type'] = bc.REPLICON_CHROMOSOME
                 log.debug('qc: detected chromosome replicon type via description: id=%s, description=%s', contig['id'], contig['description'])
             elif('plasmid' in contig_description):
                 contig['type'] = bc.REPLICON_PLASMID
                 log.debug('qc: detected plasmid replicon type via description: id=%s, description=%s', contig['id'], contig['description'])
 
+            contig_desc = []
             if(cfg.keep_contig_headers):
                 if(contig['id'] in contig_ids):
                     log.error('Fasta import: duplicated contig id! contig-id=%s', contig['id'])
                     sys.exit(f"ERROR: Detected duplicated contig id! Contig ID ({contig['id']}) occures multiple times!")
                 else:
                     contig_ids.add(contig['id'])
             else:
                 contig['orig_id'] = contig['id']
                 contig['id'] = contig_id_generated
                 contig['orig_description'] = contig['description']
-                contig_desc = []
-                if(organism_definition):
-                    contig_desc.append(organism_definition)
+                if(cfg.genus is not None or cfg.species is not None):
+                    organism = ' '.join([t for t in [cfg.genus, cfg.species] if t is not None])
+                    contig_desc.append(f"[organism={organism}]")
                 if(cfg.strain):
                     contig_desc.append(f'[strain={cfg.strain}]')
-                if(cfg.complete or contig['complete']):
-                    contig_desc.append('[completeness=complete]')
-                    if(contig['topology'] != bc.REPLICON_CONTIG):
-                        contig_desc.append(f"[topology={contig['topology']}]")
-                    if(contig['type'] == bc.REPLICON_CHROMOSOME):
-                        contig_desc.append('[location=chromosome]')
                 contig_desc.append(f'[gcode={cfg.translation_table}]')
-                contig['description'] = ' '.join(contig_desc)
 
             if(contig['complete'] and contig['topology'] == bc.TOPOLOGY_CIRCULAR):  # detection of chromosomes/plasmids via sequence length thresholds
                 if(contig['length'] >= bc.REPLICON_LENGTH_THRESHOLD_CHROMOSOME):
                     contig['type'] = bc.REPLICON_CHROMOSOME
                     log.debug('qc: detected replicon type via length: id=%s, type=%s, length=%i, description=%s', contig['id'], contig['type'], contig['length'], contig['description'])
                 elif(contig['length'] < bc.REPLICON_LENGTH_THRESHOLD_PLASMID):
                     contig['type'] = bc.REPLICON_PLASMID
                     log.debug('qc: detected replicon type via length: id=%s, type=%s, length=%i, description=%s', contig['id'], contig['type'], contig['length'], contig['description'])
             valid_contigs.append(contig)
 
-            if(len(contigs) == 1 and contig['type'] == bc.REPLICON_PLASMID and cfg.plasmid is not None):
+            if(len(contigs) == 1 and cfg.plasmid is not None):  # use plasmid mode
+                contig['type'] = bc.REPLICON_PLASMID
+                contig['topology'] = bc.TOPOLOGY_CIRCULAR
                 contig['name'] = cfg.plasmid
-
-            if(replicons):  # use user provided replicon table
+            elif(replicons):  # use user provided replicon table
                 contig_id = contig['orig_id'] if 'orig_id' in contig else contig['id']
                 replicon = replicons.get(contig_id, None)
                 if(replicon):
                     contig['type'] = replicon['replicon_type']
                     contig['topology'] = replicon['topology']
                     if(replicon['name']):
                         contig['name'] = replicon['name']
                     if(replicon['replicon_type'] != bc.REPLICON_CONTIG):
                         contig['complete'] = True
                     if(not cfg.keep_contig_headers):
                         contig['id'] = replicon['new_locus_id'] if replicon['new_locus_id'] else contig['simple_id']
-                        if(replicon['replicon_type'] != bc.REPLICON_CONTIG and 'completeness' not in contig['description']):
-                            contig['description'] += ' [completeness=complete]'
-                        if('topology' not in contig['description']):
-                            contig['description'] += f" [topology={replicon['topology']}]"
-                        if(replicon['replicon_type'] == bc.REPLICON_PLASMID and replicon['name']):
-                            contig['description'] += f" [plasmid-name={replicon['name']}]"
                     contig.pop('simple_id')
-
-            if(contig['complete'] and contig['type'] == bc.REPLICON_PLASMID and not contig.get('name', None)):
-                contig['name'] = f'unnamed{plasmid_number}'
-                plasmid_number += 1
+            
+            if(not cfg.keep_contig_headers):
+                if(contig['complete']):
+                    contig_desc.append('[completeness=complete]')
+                if(contig['topology'] != bc.REPLICON_CONTIG):
+                    contig_desc.append(f"[topology={contig['topology']}]")
+                if(contig['type'] == bc.REPLICON_CHROMOSOME):
+                    contig_desc.append('[location=chromosome]')
+                elif(contig['type'] == bc.REPLICON_PLASMID):
+                    if(not contig.get('name', None)):
+                        contig['name'] = f'unnamed{plasmid_number}'
+                        plasmid_number += 1
+                    contig_desc.append(f"[plasmid-name={contig['name']}]")
+                contig['description'] = ' '.join(list(dict.fromkeys(contig_desc)))  # remove duplicates remaining order
 
             if(contig['type'] == bc.REPLICON_CONTIG):
                 complete_genome = False
 
             if(cfg.compliant):  # check INSDC compliance
                 if(len(contig['id']) > 25):  # max 25 characters
                     log.error('INSDC compliance: contig id larger than 25! contig-id=%s', contig['id'])
```

### Comparing `bakta-1.7.0/bakta.egg-info/PKG-INFO` & `bakta-1.8.0/bakta.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bakta
-Version: 1.7.0
+Version: 1.8.0
 Summary: Bakta: rapid & standardized annotation of bacterial genomes, MAGs & plasmids
 Home-page: https://github.com/oschwengers/bakta
 Author: Oliver Schwengers
 Author-email: oliver.schwengers@computational.bio.uni-giessen.de
 License: GPLv3
 Project-URL: Documentation, https://bakta.readthedocs.io
 Project-URL: Source, https://github.com/oschwengers/bakta
@@ -51,15 +51,15 @@
         - **Fast**
         This AFSI approach substantially accellerates the annotation process by avoiding computationally expensive homology searches for identified genes. Thus, Bakta can annotate a typical bacterial genome in 10 &plusmn;5 min on a laptop, plasmids in a couple of seconds/minutes.
         
         - **Database cross-references**
         Fostering the [FAIR](https://www.go-fair.org/fair-principles) principles, Bakta exploits its AFSI approach to annotate CDS with database cross-references (**dbxref**) to RefSeq (`WP_*`), UniRef100 (`UniRef100_*`) and UniParc (`UPI*`). By doing so, IPS allow the surveillance of distinct gene alleles and streamlining comparative analysis as well as posterior (external) annotations of `putative` & `hypothetical` protein sequences which can be mapped back to existing CDS via these exact & stable identifiers (*E. coli* gene [ymiA](https://www.uniprot.org/uniprot/P0CB62) [...more](https://www.uniprot.org/help/dubious_sequences)). Currently, Bakta identifies ~214.8 mio, ~199 mio and ~161 mio distinct protein sequences from UniParc, UniRef100 and RefSeq, respectively. Hence, for certain genomes, up to 99 % of all CDS can be identified this way, skipping computationally expensive sequence alignments.
         
         - **FAIR annotations**
-        To provide standardized annotations adhearing to FAIR principles, Bakta utilizes a versioned custom annotation database comprising UniProt's [UniRef100 & UniRef90](https://www.uniprot.org/uniref/) protein clusters (FAIR -> [DOI](http://dx.doi.org/10.1038/s41597-019-0180-9)/[DOI](https://doi.org/10.1093/nar/gkaa1100)) enriched with dbxrefs (`GO`, `COG`, `EC`) and annotated by specialized niche databases. For each db version we provide a comprehensive log file of all imported sequences and annotations.
+        To provide standardized annotations adhearing to FAIR principles, Bakta utilizes a versioned custom annotation database comprising UniProt's [UniRef100 & UniRef90](https://www.uniprot.org/uniref/) protein clusters (FAIR -> [DOI](http://dx.doi.org/10.1038/s41597-019-0180-9)/[DOI](https://doi.org/10.1093/nar/gkaa1100)) enriched with dbxrefs (`GO`, `COG`, `EC`) and annotated by specialized niche databases. For each DB version we provide a comprehensive log file of all imported sequences and annotations.
         
         - **Small proteins / short open reading frames**
         Bakta detects and annotates small proteins/short open reading frames (**sORF**) which are not predicted by tools like `Prodigal`.
         
         - **Expert annotation systems**
         To provide high quality annotations for certain proteins of higher interest, *e.g.* AMR & VF genes, Bakta includes & merges different expert annotation systems. Currently, Bakta uses NCBI's AMRFinderPlus for AMR gene annotations as well as an generalized protein sequence expert system with distinct coverage, identity and priority values for each sequence, currenlty comprising the [VFDB](http://www.mgc.ac.cn/VFs/main.htm) as well as NCBI's [BlastRules](https://ftp.ncbi.nih.gov/pub/blastrules/).
         
@@ -129,39 +129,39 @@
         - Blast+ (2.12.0) <https://www.ncbi.nlm.nih.gov/pubmed/2231712> <https://blast.ncbi.nlm.nih.gov>
         - AMRFinderPlus (3.10.23) <https://github.com/ncbi/amr>
         - DeepSig (1.2.5) <https://doi.org/10.1093/bioinformatics/btx818>
         
         ### Database download
         
         Bakta requires a mandatory database which is publicly hosted at Zenodo: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4247252.svg)](https://doi.org/10.5281/zenodo.4247252)
-        We provide 2 versions: `full` and `light`. To get best annotation results and to use all features, we recommend using the default (`full`). If you seek for maximum runtime performance or if download time/storage requirements are an issue, please try the `light` version. Further information is provided in the [database](#database) section below.
+        We provide 2 types: `full` and `light`. To get best annotation results and to use all features, we recommend using the `full` (default). If you seek for maximum runtime performance or if download time/storage requirements are an issue, please try the `light` version. Further information is provided in the [database](#database) section below.
         
-        List available DB versions:
+        List available DB versions (available as either `full` or `light`):
         
         ```bash
         bakta_db list
         ...
         ```
         
         To download the most recent compatible database version we recommend to use the internal database download & setup tool:
         
         ```bash
-        bakta_db download --output <output-path> --type light
+        bakta_db download --output <output-path> --type [light|full]
         ```
         
         Of course, the database can also be downloaded manually:
         
         ```bash
-        wget https://zenodo.org/record/7025248/files/db-light.tar.gz
+        wget https://zenodo.org/record/7669534/files/db-light.tar.gz
         tar -xzf db-light.tar.gz
         rm db-light.tar.gz
         amrfinder_update --force_update --database db-light/amrfinderplus-db/
         ```
         
-        As an additional data repository backup, we provide the most recent database version via our institute servers: [full](https://jlubox.uni-giessen.de/getlink/fiWhS6LJi8AizXvspaRxRzPN/db.tar.gz), [light](https://jlubox.uni-giessen.de/getlink/fiWhS6LJi8AizXvspaRxRzPN/db-light.tar.gz). However, the bandwith is limited. Hence, please use it with caution and only if Zenodo might be temporarily uncreachable or slow. In these cases, please also download the AMRFinderPlus database as indicated above.
+        As an additional data repository backup, we provide the most recent database version via our institute servers: [full](https://jlubox.uni-giessen.de/dl/fiKeyT1huWv9vW5cXKYkZXYB/db.tar.gz), [light](https://jlubox.uni-giessen.de/dl/fiG6AHmHA94t4v2r2vwW91WB/db-light.tar.gz). However, the bandwith is limited. Hence, please use it with caution and only if Zenodo might be temporarily uncreachable or slow. In these cases, please also download the AMRFinderPlus database as indicated above.
         
         Update an existing database:
         
         ```bash
         bakta_db update --db <existing-db-path> [--tmp-dir <tmp-directory>]
         ```
         
@@ -274,21 +274,22 @@
         - `<prefix>.gbff`: annotations & sequences in (multi) GenBank format
         - `<prefix>.embl`: annotations & sequences in (multi) EMBL format
         - `<prefix>.fna`: replicon/contig DNA sequences as FASTA
         - `<prefix>.ffn`: feature nucleotide sequences as FASTA
         - `<prefix>.faa`: CDS/sORF amino acid sequences as FASTA
         - `<prefix>.hypotheticals.tsv`: further information on hypothetical protein CDS as simple human readble tab separated values
         - `<prefix>.hypotheticals.faa`: hypothetical protein CDS amino acid sequences as FASTA
+        - `<prefix>.json`: all (internal) annotation & sequence information as JSON
         - `<prefix>.txt`: summary as TXT
         - `<prefix>.png`: circular genome annotation plot as PNG
         - `<prefix>.svg`: circular genome annotation plot as SVG
         
         The `<prefix>` can be set via `--prefix <prefix>`. If no prefix is set, Bakta uses the input file prefix.
         
-        Additionally, Bakta provides detailed information on each annotated feature in a standardized machine-readable JSON file `<prefix>.json`:
+        Of note, Bakta provides all detailed (internal) information on each annotated feature in a standardized machine-readable JSON file `<prefix>.json`:
         
         ```json
         {
             "genome": {
                 "genus": "Escherichia",
                 "species": "coli",
                 ...
@@ -350,28 +351,29 @@
           --db DB, -d DB        Database path (default = <bakta_path>/db). Can also be provided as BAKTA_DB environment variable.
           --min-contig-length MIN_CONTIG_LENGTH, -m MIN_CONTIG_LENGTH
                                 Minimum contig size (default = 1; 200 in compliant mode)
           --prefix PREFIX, -p PREFIX
                                 Prefix for output files
           --output OUTPUT, -o OUTPUT
                                 Output directory (default = current working directory)
+          --force, -f           Force overwriting existing output folder
         
         Organism:
           --genus GENUS         Genus name
           --species SPECIES     Species name
           --strain STRAIN       Strain name
           --plasmid PLASMID     Plasmid name
         
         Annotation:
           --complete            All sequences are complete replicons (chromosome/plasmid[s])
           --prodigal-tf PRODIGAL_TF
                                 Path to existing Prodigal training file to use for CDS prediction
           --translation-table {11,4}
                                 Translation table: 11/4 (default = 11)
-          --gram {+,-,?}        Gram type for signal peptide predictions: +/-/? (default = '?')
+          --gram {+,-,?}        Gram type for signal peptide predictions: +/-/? (default = ?)
           --locus LOCUS         Locus prefix (default = 'contig')
           --locus-tag LOCUS_TAG
                                 Locus tag prefix (default = autogenerated)
           --keep-contig-headers
                                 Keep original contig headers
           --replicons REPLICONS, -r REPLICONS
                                 Replicon information table (tsv/csv)
@@ -486,33 +488,32 @@
         
         1. Gaps: in-mem detection & annotation of sequence gaps
         2. oriC/oriV/oriT: Blast+ (cov=0.8, id=0.8) vs. [MOB-suite](https://github.com/phac-nml/mob-suite) oriT & [DoriC](http://tubic.org/doric/public/index.php) oriC/oriV sequences. Annotations of ori regions take into account overlapping Blast+ hits and are conducted based on a majority vote heuristic. Region edges are fuzzy - use with caution!
         
         ## Database
         
         The Bakta database comprises a set of AA & DNA sequence databases as well as HMM & covariance models.
-        At its core Bakta utilizes a compact read-only SQLite db storing protein sequence digests, lengths, pre-assigned annotations and dbxrefs of UPS, IPS and PSC from:
+        At its core Bakta utilizes a compact read-only SQLite DB storing protein sequence digests, lengths, pre-assigned annotations and dbxrefs of UPS, IPS and PSC from:
         
-        - **UPS**: UniParc / UniProtKB (241,116,844)
-        - **IPS**: UniProt UniRef100 (223,313,098)
-        - **PSC**: UniProt UniRef90 (99,555,646)
-        - **PSCC**: UniProt UniRef50 (13,398,956)
-        
-        This allows the exact protein sequences identification via MD5 digests & sequence lengths as well as the rapid subsequent lookup of related information. Protein sequence digests are checked for hash collisions while the db creation process.
-        IPS & PSC have been comprehensively pre-annotated integrating annotations & database *dbxrefs* from:
-        
-        - NCBI nonredundant proteins (IPS: 183,797,372)
-        - NCBI COG db (PSC: 3,424,142)
-        - KEGG Kofams (PSC: 17,787,347)
-        - SwissProt EC/GO terms (PSC: 336,030)
-        - NCBI NCBIfams (PSC: 13,466,827)
-        - PHROG (PSC: 0)
-        - NCBI AMRFinderPlus (IPS: 7,009)
-        - ISFinder db (IPS: 53,341, PSC: 11,412)
-        - Pfam families (PSC: 3,917,555)
+        - **UPS**: UniParc / UniProtKB (246,384,812)
+        - **IPS**: UniProt UniRef100 (228,759,203)
+        - **PSC**: UniProt UniRef90 (100,315,337)
+        - **PSCC**: UniProt UniRef50 (23,959,577)
+        
+        This allows the exact protein sequences identification via MD5 digests & sequence lengths as well as the rapid subsequent lookup of related information. Protein sequence digests are checked for hash collisions while the DB creation process. IPS & PSC have been comprehensively pre-annotated integrating annotations & database *dbxrefs* from:
+        
+        - NCBI nonredundant proteins (IPS: 192,288,757)
+        - NCBI COG DB (PSC: 3,428,564)
+        - KEGG Kofams (PSC: 16,776,225)
+        - SwissProt EC/GO terms (PSC: 336,187)
+        - NCBI NCBIfams (PSC: 14,391,965)
+        - PHROG (PSC: 4,379)
+        - NCBI AMRFinderPlus (IPS: 7,235)
+        - ISFinder DB (IPS: 125,967, PSC: 11,800)
+        - Pfam families (PSC: 248,169)
         
         To provide high quality annotations for distinct protein sequences of high importance (AMR, VF, *etc*) which cannot sufficiently be covered by the IPS/PSC approach, Bakta provides additional expert systems. For instance, AMR genes, are annotated via NCBI's AMRFinderPlus.
         An expandable alignment-based expert system supports the incorporation of high quality annotations from multiple sources. This currenlty comprises NCBI's BlastRules as well as VFDB and will be complemented with more expert annotation sources over time. Internally, this expert system is based on a Diamond DB comprising the following information in a standardized format:
         
         - source: *e.g.* BlastRules
         - rank: a precedence rank
         - min identity
@@ -520,30 +521,31 @@
         - min model coverage
         - gene lable
         - product description
         - dbxrefs
         
         Rfam covariance models:
         
-        - ncRNA: 798
+        - ncRNA: 802
         - ncRNA cis-regulatory regions: 270
         
         ori sequences:
         
-        - oriC/V: 10,878
+        - oriC/V: 6,690
         - oriT: 502
         
-        To provide FAIR annotations, the database releases are SemVer versioned (w/o patch level), *i.e.* `<major>.<minor>`. For each version we provide a comprehensive log file tracking all imported sequences as well as annotations thereof. The db schema is represented by the `<major>` digit and automatically checked at runtime by Bakta in order to ensure compatibility. Content updates are tracked by the `<minor>` digit.
+        To provide FAIR annotations, the database releases are SemVer versioned (w/o patch level), *i.e.* `<major>.<minor>`. For each version we provide a comprehensive log file tracking all imported sequences as well as annotations thereof. The DB schema is represented by the `<major>` digit and automatically checked at runtime by Bakta in order to ensure compatibility. Content updates are tracked by the `<minor>` digit.
         
-        Since this taxonomic-untargeted database is fairly demanding regarding storage consumption, we provide a lightweight version providing all non-coding feature information but only PSCC information from UniRef50 clusters for CDS. If download bandwiths or storage requirements are an issue or if faster runtimes for less-specific annotation are favored, the `light` database will do the job!
+        As this taxonomic-untargeted database is fairly demanding in terms of storage consumption, we also provide a lightweight DB type providing all non-coding feature information but only PSCC information from UniRef50 clusters for CDS. If download bandwiths or storage requirements become an issue or if shorter runtimes are favored over more-specific annotation, the `light` DB will do the job.
         
-        Latest database version 5.0:
+        Latest database version: 5.0
+        DB types:
         
-        - `full`: 31 Gb zipped, 60 Gb unzipped
-        - `light`: 1.2 Gb zipped, 2.8 Gb unzipped
+        - `light`: 1.2 Gb zipped, 2.8 Gb unzipped, MD5: a40e680b4aab7871102f31aaac91838b
+        - `full`: 31 Gb zipped, 60 Gb unzipped, MD5: 3200136a0a32b3c33d1cb348ab6b87de
         
         All database releases are hosted at Zenodo: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4247252.svg)](https://doi.org/10.5281/zenodo.4247252)
         
         ## Genome Submission
         
         Most genomes annotated with Bakta should be ready-to-submid to INSDC member databases GenBank and ENA. As a first step, please register your BioProject (e.g. PRJNA123456) and your locus_tag prefix (*e.g.* ESAKAI).
         
@@ -622,39 +624,43 @@
         ### Output
         
         Annotation results are provided in standard bioinformatics file formats:
         
         - `<prefix>.tsv`: annotations as simple human readble TSV
         - `<prefix>.faa`: protein sequences as FASTA
         - `<prefix>.hypotheticals.tsv`: further information on hypothetical proteins as simple human readble tab separated values
+        - `<prefix>.json`: all (internal) annotation & sequence information as JSON
         
         The `<prefix>` can be set via `--prefix <prefix>`. If no prefix is set, Bakta uses the input file prefix.
         
         ### Usage
         
         ```bash
-        usage: bakta_proteins [--db DB] [--output OUTPUT] [--prefix PREFIX] [--proteins PROTEINS] [--help] [--threads THREADS] [--tmp-dir TMP_DIR] [--version] <input>
+        usage: bakta_proteins [--db DB] [--output OUTPUT] [--prefix PREFIX] [--force] [--proteins PROTEINS] [--help] [--verbose] [--debug] [--threads THREADS] [--tmp-dir TMP_DIR] [--version] <input>
         
         Rapid & standardized annotation of bacterial genomes, MAGs & plasmids
         
         positional arguments:
           <input>               Protein sequences in (zipped) fasta format
         
         Input / Output:
           --db DB, -d DB        Database path (default = <bakta_path>/db). Can also be provided as BAKTA_DB environment variable.
           --output OUTPUT, -o OUTPUT
                                 Output directory (default = current working directory)
           --prefix PREFIX, -p PREFIX
                                 Prefix for output files
+          --force, -f           Force overwriting existing output folder
         
         Annotation:
           --proteins PROTEINS   Fasta file of trusted protein sequences for annotation
         
-        Runtime & auxiliary options:
+        General:
           --help, -h            Show this help message and exit
+          --verbose, -v         Print verbose information
+          --debug               Run Bakta in debug mode. Temp data will not be removed.
           --threads THREADS, -t THREADS
                                 Number of threads to use (default = number of available CPUs)
           --tmp-dir TMP_DIR     Location for temporary files (default = system dependent auto detection)
           --version, -V         show program's version number and exit
         ```
         
         ## Genome plots
@@ -792,14 +798,16 @@
         
 Keywords: bioinformatics,annotation,bacteria,plasmids
 Platform: UNKNOWN
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Requires-Python: >=3.8
```

### Comparing `bakta-1.7.0/bakta.egg-info/SOURCES.txt` & `bakta-1.8.0/bakta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bakta-1.7.0/setup.py` & `bakta-1.8.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,29 +27,31 @@
     zip_safe=False,
     install_requires=[
         'biopython >= 1.80',
         'xopen >= 1.1.0',
         'requests >= 2.25.1',
         'alive-progress >= 3.0.1',
         'PyYAML >= 6.0',
-        'pyrodigal >= 2.0.2'
+        'pyrodigal >= 2.1.0'
     ],
     entry_points={
         'console_scripts': [
             'bakta=bakta.main:main',
             'bakta_proteins=bakta.proteins:main',
             'bakta_db=bakta.db:main',
             'bakta_plot=bakta.plot:main'
         ]
     },
     classifiers=[
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Topic :: Scientific/Engineering :: Bio-Informatics',
         'Environment :: Console',
         'Intended Audience :: Science/Research',
         'Natural Language :: English'
     ],
```

### Comparing `bakta-1.7.0/test/test_args.py` & `bakta-1.8.0/test/test_args.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         (['test/data/invalid.fasta']),  # invalid fasta DNA alphabet
         (['test/data/NC_002127.1.fna', 'foo']),  # additional argument
     ]
 )
 def test_genome_failing(parameters, tmpdir):
     # test genome arguments
     proc = run(
-        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--skip-plot'] +
+        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--force', '--skip-plot'] +
         SKIP_PARAMETERS +
         parameters
     )
     assert proc.returncode != 0
 
 
 @pytest.mark.parametrize(
@@ -40,15 +40,15 @@
         (['test/data/NC_002127.1-win.fna.gz']),  # Windows format (\r\n)
         (['test/data/valid.fasta'])  # valid minimal DNA sequences
     ]
 )
 def test_genome_ok(genome, tmpdir):
     # test genome arguments
     proc = run(
-        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--skip-plot'] +
+        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--force', '--skip-plot'] +
         SKIP_PARAMETERS +
         genome
     )
     assert proc.returncode == 0
 
 
 @pytest.mark.parametrize(
@@ -61,15 +61,15 @@
         (['--db', 'test/data/empty']),  # empty file
         (['--db', 'test/data/nonsense.txt'])  # nonsense file
     ]
 )
 def test_database_failing_parameter(parameters, tmpdir):
     # test database arguments
     proc = run(
-        ['bin/bakta', '--output', tmpdir, '--skip-plot'] +
+        ['bin/bakta', '--output', tmpdir, '--force', '--skip-plot'] +
         parameters +
         SKIP_PARAMETERS +
         ['test/data/NC_002127.1.fna']
     )
     assert proc.returncode != 0
 
 
@@ -85,15 +85,15 @@
 )
 def test_database_failing_environment(env_key, env_value, tmpdir):
     # test database arguments
 
     env = os.environ
     env[env_key] = env_value
     proc = run(
-        ['bin/bakta', '--output', tmpdir, '--skip-plot'] +
+        ['bin/bakta', '--output', tmpdir, '--force', '--skip-plot'] +
         SKIP_PARAMETERS +
         ['test/data/NC_002127.1.fna'],
         env=env
     )
     assert proc.returncode != 0
 
 
@@ -105,66 +105,63 @@
     ]
 )
 def test_database_ok(db, tmpdir):
     # test database arguments
 
     # parameter OK
     proc = run(
-        ['bin/bakta', '--db', f'test/{db}', '--output', tmpdir, '--skip-plot'] +
+        ['bin/bakta', '--db', f'test/{db}', '--output', tmpdir, '--force', '--skip-plot'] +
         SKIP_PARAMETERS +
         ['test/data/NC_002127.1.fna']
     )
     assert proc.returncode == 0
 
     # environment OK
     env = os.environ
     env['BAKTA_DB'] = f'test/{db}'
     proc = run(
-        ['bin/bakta', '--output', tmpdir, '--skip-plot'] +
+        ['bin/bakta', '--output', tmpdir, '--force', '--skip-plot'] +
         SKIP_PARAMETERS +
         ['test/data/NC_002127.1.fna']
         , env=env
     )
     assert proc.returncode == 0
 
 
 def test_output_failing():
     # test database arguments
     proc = run(
-        ['bin/bakta', '--db', 'test/db', '--output', '/', '--skip-plot'] +
+        ['bin/bakta', '--db', 'test/db', '--output', '/', '--force', '--skip-plot'] +
         SKIP_PARAMETERS +
         ['test/data/NC_002127.1.fna']
     )
     assert proc.returncode != 0
 
 
 @pytest.mark.parametrize(
     'parameters',
     [
-        (['--tmp-dir']),  # not provided
-
-# ToDo
-
+        (['--tmp-dir'])  # not provided
     ]
 )
 def test_tmp_dir_failiing(parameters, tmpdir):
     # test tmp dir arguments
     proc = run(
-        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--skip-plot'] +
+        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--force', '--skip-plot'] +
         parameters +
         SKIP_PARAMETERS +
         ['test/data/NC_002127.1.fna']
     )
     assert proc.returncode != 0
 
 
 def test_tmp_dir_ok(tmpdir):
     # test tmp dir arguments
     proc = run(
-        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--tmp-dir', '', '--skip-plot'] +
+        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--force', '--tmp-dir', '', '--skip-plot'] +
         SKIP_PARAMETERS +
         ['test/data/NC_002127.1.fna']
     )
     assert proc.returncode == 0
 
 
 @pytest.mark.parametrize(
@@ -175,27 +172,26 @@
         (['--prodigal-tf', 'foo']),  # not existing
         (['--prodigal-tf', 'test/data/empty'])  # empty file
     ]
 )
 def test_prodigal_tf_failiing(parameters, tmpdir):
     # test prodigal training file arguments
     proc = run(
-        ['bin/bakta', '--db', 'test/db', '--output', tmpdir] +
+        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--force'] +
         parameters +
         ['--skip-tmrna', '--skip-trna', '--skip-rrna', '--skip-ncrna', '--skip-ncrna-region', '--skip-crispr', '--skip-sorf', '--skip-ori', '--skip-gap', '--skip-plot'] +
         ['test/data/NC_002127.1.fna']
     )
     assert proc.returncode != 0
 
 
-@pytest.mark.slow
 def test_prodigal_tf_ok(tmpdir):
     # test prodigal training file arguments
     proc = run(
-        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--prefix', 'test', '--prodigal-tf', 'test/data/prodigal.tf'] +
+        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--force', '--prefix', 'test', '--prodigal-tf', 'test/data/prodigal.tf'] +
         SKIP_PARAMETERS +
         ['test/data/NC_002127.1.fna']
     )
     assert proc.returncode == 0
 
     tmpdir_path = Path(tmpdir)
     for file in FILES:
@@ -211,34 +207,33 @@
         (['--replicons', 'test/data/empty']),  # empty file
         (['--replicons', 'test/data/nonsense.txt'])  # nonsense file
     ]
 )
 def test_replicons_failiing(parameters, tmpdir):
     # test replicons file arguments
     proc = run(
-        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--skip-plot'] +
+        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--force', '--skip-plot'] +
         parameters +
         SKIP_PARAMETERS +
         ['test/data/NC_002127.1.fna']
     )
     assert proc.returncode != 0
 
 
-@pytest.mark.slow
 @pytest.mark.parametrize(
     'parameters',
     [
         (['--replicons', 'test/data/replicons.csv']),  # CSV
         (['--replicons', 'test/data/replicons.tsv'])  # TSV
     ]
 )
 def test_replicons_ok(parameters, tmpdir):
     # test replicons file arguments
     proc = run(
-        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--prefix', 'test'] +
+        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--force', '--prefix', 'test'] +
         parameters +
         SKIP_PARAMETERS +
         ['test/data/NC_002127.1.fna']
     )
     assert proc.returncode == 0
 
     tmpdir_path = Path(tmpdir)
@@ -255,15 +250,15 @@
         (['--proteins', 'test/data/empty']),  # empty file
         (['--proteins', 'test/data/nonsense.txt'])  # nonsense file
     ]
 )
 def test_proteins_failiing(parameters, tmpdir):
     # test proteins file arguments
     proc = run(
-        ['bin/bakta', '--db', 'test/db', '--output', tmpdir] + 
+        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--force'] + 
         parameters + 
         ['--skip-tmrna', '--skip-trna', '--skip-rrna', '--skip-ncrna', '--skip-ncrna-region', '--skip-crispr', '--skip-sorf', '--skip-ori', '--skip-gap', '--skip-plot'] +
         ['test/data/NC_002127.1.fna']
     )
     assert proc.returncode != 0
 
 
@@ -279,35 +274,34 @@
         (['--locus', 'A123#']),  # containing pound (incompatible with circos)
         (['--locus', 'ABCDEFGHIJKLMNOPQRSTU'])  # more than 20 characters
     ]
 )
 def test_locus_failiing(parameters, tmpdir):
     # test locus prefix arguments
     proc = run(
-        ['bin/bakta', '--db', 'test/db', '--output', tmpdir] +
+        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--force'] +
         parameters +
         SKIP_PARAMETERS +
         ['test/data/NC_002127.1.fna']
     )
     assert proc.returncode != 0
 
 
-@pytest.mark.slow
 @pytest.mark.parametrize(
     'parameters',
     [
         (['--locus', 'ABC']),
         (['--locus', 'ABCDEFGHIJKLMNOPQRST']),
         (['--locus', 'A123_.*-'])
     ]
 )
 def test_locus_ok(parameters, tmpdir):
     # test locus prefix arguments
     proc = run(
-        ['bin/bakta', '--db', 'test/db', '--output', tmpdir] +
+        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--force'] +
         parameters +
         SKIP_PARAMETERS +
         ['test/data/NC_002127.1.fna']
     )
     assert proc.returncode == 0
 
 
@@ -333,23 +327,22 @@
         (['--locus-tag', 'ABC=']),  # wrong characters
         (['--locus-tag', 'ABC#'])  # wrong characters
     ]
 )
 def test_locustag_failiing(parameters, tmpdir):
     # test locus-tag prefix arguments
     proc = run(
-        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--skip-plot'] +
+        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--force', '--skip-plot'] +
         parameters +
         SKIP_PARAMETERS +
         ['test/data/NC_002127.1.fna']
     )
     assert proc.returncode != 0
 
 
-@pytest.mark.slow
 @pytest.mark.parametrize(
     'parameters',
     [
         (['--locus-tag', 'A']),
         (['--locus-tag', '1']),
         (['--locus-tag', 'ABCDEFGHIJKLMNOPQRSTUVWX']),
         (['--locus-tag', 'A12']),
@@ -360,15 +353,15 @@
         (['--locus-tag', 'ASM25969v1']),
         (['--locus-tag', 'DAESDI010000001.1'])
     ]
 )
 def test_locustag_ok(parameters, tmpdir):
     # test locus-tag prefix arguments
     proc = run(
-        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--skip-plot'] +
+        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--force', '--skip-plot'] +
         parameters +
         SKIP_PARAMETERS +
         ['test/data/NC_002127.1.fna']
     )
     assert proc.returncode == 0
 
 
@@ -401,36 +394,35 @@
         (['--locus-tag', 'ABC=']),  # wrong characters
         (['--locus-tag', 'ABC#'])  # wrong characters
     ]
 )
 def test_locustag_compliant_failiing(parameters, tmpdir):
     # test locus-tag prefix arguments
     proc = run(
-        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--compliant', '--skip-plot'] +
+        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--force', '--compliant', '--skip-plot'] +
         parameters +
         SKIP_PARAMETERS +
         ['test/data/NC_002127.1.fna']
     )
     assert proc.returncode != 0
 
 
-@pytest.mark.slow
 @pytest.mark.parametrize(
     'parameters',
     [
         (['--locus-tag', 'ABC']),
         (['--locus-tag', 'ABCDEFGHIJKL']),
         (['--locus-tag', 'A12']),
         (['--locus-tag', 'A23456789012'])
     ]
 )
 def test_locustag_compliant_ok(parameters, tmpdir):
     # test locus-tag prefix arguments
     proc = run(
-        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--compliant', '--skip-plot'] +
+        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--force', '--compliant', '--skip-plot'] +
         parameters +
         SKIP_PARAMETERS +
         ['test/data/NC_002127.1.fna']
     )
     assert proc.returncode == 0
 
 
@@ -440,17 +432,17 @@
         (['--genus']),  # not provided
         (['--genus', '']),  # empty
         (['--genus', ' ']),  # whitespace only
         (['--genus', '  '])  # whitespaces only
     ]
 )
 def test_genus_failiing(parameters, tmpdir):
-    # test genus prefix arguments
+    # test genus arguments
     proc = run(
-        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--skip-plot'] +
+        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--force', '--skip-plot'] +
         parameters +
         SKIP_PARAMETERS +
         ['test/data/NC_002127.1.fna']
     )
     assert proc.returncode != 0
 
 
@@ -461,17 +453,17 @@
         (['--species', 'sp. nov.']),
         (['--species', 'a']),
         (['--species', '1']),
         (['--species', 'az_123'])
     ]
 )
 def test_species_ok(parameters, tmpdir):
-    # test species prefix arguments
+    # test species arguments
     proc = run(
-        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--skip-plot'] +
+        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--force', '--skip-plot'] +
         parameters +
         SKIP_PARAMETERS +
         ['test/data/NC_002127.1.fna']
     )
     assert proc.returncode == 0
 
 
@@ -481,17 +473,17 @@
         (['--species']),  # not provided
         (['--species', '']),  # empty
         (['--species', ' ']),  # whitespace only
         (['--species', '  '])  # whitespaces only
     ]
 )
 def test_species_failiing(parameters, tmpdir):
-    # test species prefix arguments
+    # test species arguments
     proc = run(
-        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--skip-plot'] +
+        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--force', '--skip-plot'] +
         parameters +
         SKIP_PARAMETERS +
         ['test/data/NC_002127.1.fna']
     )
     assert proc.returncode != 0
 
 
@@ -501,17 +493,17 @@
         (['--strain', 'a']),
         (['--strain', '1']),
         (['--strain', 'az. 123-123_234/123 = 123']),  # full blown crazy strain designation
         (['--strain', "0123456789'azAZ/.,#+* -_:(1)[]"])  # all RefSeq bacterial strain characters
     ]
 )
 def test_strain_ok(parameters, tmpdir):
-    # test strain prefix arguments
+    # test strain arguments
     proc = run(
-        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--skip-plot'] +
+        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--force', '--skip-plot'] +
         parameters +
         SKIP_PARAMETERS +
         ['test/data/NC_002127.1.fna']
     )
     assert proc.returncode == 0
 
 
@@ -521,17 +513,72 @@
         (['--strain']),  # not provided
         (['--strain', '']),  # empty
         (['--strain', ' ']),  # whitespace only
         (['--strain', '  '])  # whitespaces only
     ]
 )
 def test_strain_failiing(parameters, tmpdir):
-    # test strain prefix arguments
+    # test strain arguments
+    proc = run(
+        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--force', '--skip-plot'] +
+        parameters +
+        SKIP_PARAMETERS +
+        ['test/data/NC_002127.1.fna']
+    )
+    assert proc.returncode != 0
+
+
+@pytest.mark.parametrize(
+    'parameters',
+    [
+        (['--plasmid', 'unnamed']),  # unnamed example
+        (['--plasmid', 'unnamed1']),  # unnamed example
+        (['--plasmid', 'unnamed12']),  # unnamed example
+        (['--plasmid', 'unnamed123']),  # unnamed example
+        (['--plasmid', 'pA']),  # minimal set
+        (['--plasmid', 'pZ']),  # minimal set
+        (['--plasmid', 'p1']),  # minimal set
+        (['--plasmid', 'p2']),  # minimal set
+        (['--plasmid', 'p.']),  # minimal set
+        (['--plasmid', 'p_']),  # minimal set
+        (['--plasmid', 'pAZ.az_09'])  # full blown plasmid designation
+    ]
+)
+def test_plasmid_ok(parameters, tmpdir):
+    # test plasmid arguments
+    proc = run(
+        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--force', '--skip-plot'] +
+        parameters +
+        SKIP_PARAMETERS +
+        ['test/data/NC_002127.1.fna']
+    )
+    assert proc.returncode == 0
+
+
+@pytest.mark.parametrize(
+    'parameters',
+    [
+        (['--plasmid', '']),  # empty
+        (['--plasmid', 'unnamed1234']),  # wrong unnamed example
+        (['--plasmid', 'unname']),  # wrong unnamed example
+        (['--plasmid', 'p']),  # p only
+        (['--plasmid', 'pABCDEFGHIJKLMNOPQRST']),  # longer than 20 chars
+        (['--plasmid', 'pAZ 123']),  # contains whitespace
+        (['--plasmid', 'pAZ-123']),  # contains dash
+        (['--plasmid', 'pAZ/123']),  # contains slash
+        (['--plasmid', 'pAZ\\123']),  # contains backslash
+        (['--plasmid', 'pAZ=123']),  # contains equals
+        (['--plasmid', 'plasmid123']),  # contains word plasmid
+        (['--plasmid', 'pPlasmidA1'])  # contains word plasmid
+    ]
+)
+def test_plasmid_failiing(parameters, tmpdir):
+    # test plasmid arguments
     proc = run(
-        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--skip-plot'] +
+        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--force', '--skip-plot'] +
         parameters +
         SKIP_PARAMETERS +
         ['test/data/NC_002127.1.fna']
     )
     assert proc.returncode != 0
 
 
@@ -545,15 +592,15 @@
         (['--gram', '0']),  # number
         (['--gram', '1.1']),  # number
     ]
 )
 def test_threads_failing(parameters, tmpdir):
     # test gram arguments
     proc = run(
-        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--skip-plot'] +
+        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--force', '--skip-plot'] +
         parameters +
         SKIP_PARAMETERS +
         ['test/data/NC_002127.1.fna']
     )
     assert proc.returncode != 0
 
 
@@ -567,15 +614,15 @@
         (['--threads', '1.1']),  # float
         (['--threads', '1000'])  # larger than available threads
     ]
 )
 def test_threads_failing(parameters, tmpdir):
     # test threads arguments
     proc = run(
-        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--skip-plot'] +
+        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--force', '--skip-plot'] +
         parameters +
         SKIP_PARAMETERS +
         ['test/data/NC_002127.1.fna']
     )
     assert proc.returncode != 0
 
 
@@ -589,15 +636,15 @@
         (['--min-contig-length', '0']),  # zero
         (['--min-contig-length', '1.1']),  # float
     ]
 )
 def test_min_contig_length_failing(parameters, tmpdir):
     # test min-contig-length arguments
     proc = run(
-        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--skip-plot'] +
+        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--force', '--skip-plot'] +
         parameters +
         SKIP_PARAMETERS +
         ['test/data/NC_002127.1.fna']
     )
     assert proc.returncode != 0
 
 
@@ -611,13 +658,13 @@
         (['--translation-table', '0']),  # zero
         (['--translation-table', '1.1']),  # float
     ]
 )
 def test_min_contig_length_failing(parameters, tmpdir):
     # test min-contig-length arguments
     proc = run(
-        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--skip-plot'] +
+        ['bin/bakta', '--db', 'test/db', '--output', tmpdir, '--force', '--skip-plot'] +
         parameters +
         SKIP_PARAMETERS +
         ['test/data/NC_002127.1.fna']
     )
     assert proc.returncode != 0
```

### Comparing `bakta-1.7.0/test/test_bakta.py` & `bakta-1.8.0/test/test_bakta.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,43 +17,41 @@
         sp.check_output(command, stderr=sp.STDOUT)  # stderr must be added in case the tool output is not piped into stdout
         is_available = True
     except:
         print(f"WARNING: {command[0]} not found or not executable! Skip dependen test.")
     return is_available
 
 
-@pytest.mark.slow
 @pytest.mark.parametrize(
     'db',
     [
         ('db'),  # full DB
         ('db-light')  # light DB
     ]
 )
 def test_bakta_mock_skipped_features(db, tmpdir):
     # fast test full features
     proc = run(
-        ['bin/bakta', '--db', f'test/{db}', '--output', tmpdir, '--prefix', 'test', '--min-contig-length', '200', '--proteins', 'test/data/user-proteins.faa'] +
+        ['bin/bakta', '--db', f'test/{db}', '--output', tmpdir, '--force', '--prefix', 'test', '--min-contig-length', '200', '--proteins', 'test/data/user-proteins.faa'] +
         ['--genus', 'Foo gen. nov.', '--species', 'bar sp. nov.', '--strain', 'test 1'] +
         SKIP_PARAMETERS +
         ['test/data/NC_002127.1.fna']
     )
     assert proc.returncode == 0
 
     tmpdir_path = Path(tmpdir)
     for file in FILES:
         assert Path.exists(tmpdir_path.joinpath(file))
 
 
-@pytest.mark.slow
 @pytest.mark.skipif(check_deepsig() == False, reason=f'Skip on unavailable DeepSig')
 def test_bakta_plasmid(tmpdir):
     # full test on plasmid
     proc = run(
-        ['bin/bakta', '--db', 'test/db', '--verbose', '--output', tmpdir, '--prefix', 'test', '--min-contig-length', '200', '--complete', '--gram', '-', '--proteins', 'test/data/user-proteins.faa'] +
+        ['bin/bakta', '--db', 'test/db', '--verbose', '--output', tmpdir, '--force', '--prefix', 'test', '--min-contig-length', '200', '--complete', '--gram', '-', '--proteins', 'test/data/user-proteins.faa'] +
         ['--genus', 'Foo gen. nov.', '--species', 'bar sp. nov.', '--strain', 'test 1', 'test/data/NC_002127.1.fna.gz']
     )
     assert proc.returncode == 0
 
     tmpdir_path = Path(tmpdir)
     for file in FILES:
         output_path = tmpdir_path.joinpath(file)
@@ -76,25 +74,24 @@
         'oriT': 0,
         'cds': 3
     }
     for type in feature_counts:
         assert feature_counts[type] == feature_counts_expected[type]
 
 
-@pytest.mark.slow
 @pytest.mark.parametrize(
     'db',
     [
         ('db'),  # full DB
         ('db-light')  # light DB
     ]
 )
 def test_bakta_genome(db, tmpdir):
     # full test on complete genome in compliant mode
-    proc = run(['bin/bakta', '--db', f'test/{db}', '--verbose', '--output', tmpdir, '--prefix', 'test', '--min-contig-length', '200', '--complete', '--compliant', '--proteins', 'test/data/user-proteins.faa', '--genus', 'Foo gen. nov.', '--species', 'bar sp. nov.', '--strain', 'test 1', 'test/data/GCF_000008865.2.fna.gz'])
+    proc = run(['bin/bakta', '--db', f'test/{db}', '--verbose', '--output', tmpdir, '--force', '--force', '--prefix', 'test', '--min-contig-length', '200', '--complete', '--compliant', '--proteins', 'test/data/user-proteins.faa', '--genus', 'Foo gen. nov.', '--species', 'bar sp. nov.', '--strain', 'test 1', 'test/data/GCF_000008865.2.fna.gz'])
     assert proc.returncode == 0
 
     tmpdir_path = Path(tmpdir)
     for file in FILES:
         output_path = tmpdir_path.joinpath(file)
         assert Path.exists(output_path)
         assert output_path.stat().st_size > 0
```

### Comparing `bakta-1.7.0/test/test_bakta_proteins.py` & `bakta-1.8.0/test/test_bakta_proteins.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 FILES = [
     'test.tsv',
     'test.hypotheticals.tsv',
     'test.faa'
 ]
 
 
-@pytest.mark.slow
 @pytest.mark.parametrize(
     "user_proteins",
     [
         'test/data/user-proteins.faa',
         'test/data/user-proteins.gbff'
     ]
 )
@@ -23,15 +22,15 @@
     [
         'test/data/GCF_000008865.2.faa',
         'test/data/GCF_000008865.2.faa.gz'
     ]
 )
 def test_bakta_genome(user_proteins, input, tmpdir):
     # full test on complete genome in compliant mode
-    proc = run(['bin/bakta_proteins', '--db', 'test/db', '--output', tmpdir, '--prefix', 'test', '--proteins', user_proteins, input])
+    proc = run(['bin/bakta_proteins', '--db', 'test/db', '--output', tmpdir, '--force', '--prefix', 'test', '--proteins', user_proteins, input])
     assert proc.returncode == 0
 
     tmpdir_path = Path(tmpdir)
     for file in FILES:
         output_path = tmpdir_path.joinpath(file)
         assert Path.exists(output_path)
         assert output_path.stat().st_size > 0
```

### Comparing `bakta-1.7.0/test/test_dependencies.py` & `bakta-1.8.0/test/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `bakta-1.7.0/test/test_edge_features.py` & `bakta-1.8.0/test/test_edge_features.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,19 @@
 from subprocess import run
 
 import pytest
 
 from bakta import constants as bc
 
 
-@pytest.mark.slow
 def test_bakta_edge_features(tmpdir):
     # test edge lable on mock CDS contig
     proc = run(
         [
-            'bin/bakta', '--db', 'test/db', '--output', tmpdir, '--prefix', 'test',
+            'bin/bakta', '--db', 'test/db', '--output', tmpdir, '--force', '--prefix', 'test',
             '--skip-tmrna', '--skip-trna', '--skip-rrna', '--skip-ncrna', '--skip-ncrna-region', '--skip-crispr', '--skip-sorf', '--skip-ori', '--skip-gap', '--skip-plot',
             '--keep-contig-headers', '--complete', 'test/data/cds.fna'
         ]
     )
     assert proc.returncode == 0
 
     tmpdir_path = Path(tmpdir)
```

### Comparing `bakta-1.7.0/test/test_nt_sequences.py` & `bakta-1.8.0/test/test_nt_sequences.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,20 +5,19 @@
 
 import pytest
 
 cds = 'TTGACTACGCCATTGAAAAAGATTGTGATTGTCGGCGGCGGTGCTGGTGGGCTGGAAATGGCAACACAGCTGGGGCATAAGCTGGGACGCAAGAAAAAAGCCAAAATTACGCTGGTCGATCGTAACCACAGCCATCTGTGGAAACCGCTGCTGCACGAAGTGGCGACTGGCTCGCTTGATGAAGGCGTCGATGCGTTGAGCTATCTGGCCCATGCGCGCAATCATGGTTTCCAGTTCCAGCTGGGTTCCGTCATTGATATTGATCGTGAAGCGAAAACAATCACTATTGCAGAACTGCGCGATGAGAAAGGTGAACTGCTGGTTCCGGAACGTAAAATCGCCTATGACACCCTGGTAATGGCGCTGGGTAGCACCTCTAACGATTTCAATACGCCAGGTGTCAAAGAGAACTGCATTTTCCTCGATAACCCGCACCAGGCGCGTCGCTTTCACCAGGAGATGCTGAATCTCTTCCTGAAATACTCCGCCAACCTGGGCGCAAATGGCAAAGTGAACATTGCGATTGTCGGCGGCGGCGCGACGGGTGTAGAACTCTCCGCTGAATTGCACAACGCGGTCAAGCAACTGCACAGCTACGGTTACAAAGGCCTGACCAACGAAGCCCTGAACGTAACGCTGGTAGAAGCGGGAGAACGTATTTTGCCTGCATTACCGCCACGTATCTCTGCTGCGGCCCACAACGAGCTAACGAAACTTGGCGTTCGCGTGCTGACGCAAACCATGGTCACCAGTGCTGATGAAGGCGGCCTGCACACTAAAGATGGCGAATATATTGAGGCTGATCTGATGGTGTGGGCAGCCGGGATCAAAGCGCCAGACTTCCTGAAAGATATCGGTGGTCTTGAAACTAACCGTATCAACCAGCTGGTGGTGGAACCGACGCTGCAAACCACCCGCGATCCAGACATTTACGCTATTGGCGACTGCGCGTCATGCCCGCGTCCGGAAGGGGGCTTTGTTCCGCCGCGTGCTCAGGCTGCACACCAGATGGCGACTTGCGCAATGAACAACATTCTGGCGCAGATGAATGGTAAGCCGCTGAAAAATTATCAGTATAAAGATCATGGTTCGCTGGTATCGCTGTCGAACTTCTCCACCGTTGGTAGCCTGATGGGTAACCTGACGCGCGGCTCAATGATGATTGAAGGACGAATTGCGCGCTTTGTATATATCTCGCTATACCGAATGCATCAGATTGCGCTGCATGGTTACTTTAAAACCGGATTAATGATGCTGGTGGGGAGTATTAACCGCGTTATCCGTCCGCGTTTGAAGTTGCATTAA'
 sorf = 'ATGGTGAATACCGGCGGCAATAAACGTCAGGTGCCGGCGAAACGTCAGAATCGTGGCTCCCGTAATTCCAAAGATGATGGCGGCTAA'
 
 
-@pytest.mark.slow
 def test_bakta_cds_nt_sequence(tmpdir):
     # test extracted nucleotide sequences of cds
     proc = run(
         [
-            'bin/bakta', '--db', 'test/db', '--output', tmpdir, '--prefix', 'test',
+            'bin/bakta', '--db', 'test/db', '--output', tmpdir, '--force', '--prefix', 'test',
             '--skip-tmrna', '--skip-trna', '--skip-rrna', '--skip-ncrna', '--skip-ncrna-region', '--skip-crispr', '--skip-sorf', '--skip-ori', '--skip-gap', '--skip-plot',
             '--keep-contig-headers', '--complete', 'test/data/cds.fna'
         ]
     )
     assert proc.returncode == 0
 
     tmpdir_path = Path(tmpdir)
@@ -30,20 +29,19 @@
         results = json.load(fh)
 
     for feat in results['features']:
         if(feat['contig'] != 'dummy'):
             assert feat['nt'] == cds
 
 
-@pytest.mark.slow
 def test_bakta_sorf_nt_sequence(tmpdir):
     # test extracted nucleotide sequences of sorfs
     proc = run(
         [
-            'bin/bakta', '--db', 'test/db', '--output', tmpdir, '--prefix', 'test',
+            'bin/bakta', '--db', 'test/db', '--output', tmpdir, '--force', '--prefix', 'test',
             '--skip-tmrna', '--skip-trna', '--skip-rrna', '--skip-ncrna', '--skip-ncrna-region', '--skip-crispr', '--skip-cds', '--skip-ori', '--skip-gap', '--skip-plot',
             '--keep-contig-headers', '--complete', 'test/data/sorf.fna'
         ]
     )
     assert proc.returncode == 0
 
     tmpdir_path = Path(tmpdir)
```

### Comparing `bakta-1.7.0/test/test_pseudo.py` & `bakta-1.8.0/test/test_pseudo.py`

 * *Files identical despite different names*

### Comparing `bakta-1.7.0/test/test_sORF.py` & `bakta-1.8.0/test/test_sORF.py`

 * *Files identical despite different names*

### Comparing `bakta-1.7.0/test/test_sig_peps.py` & `bakta-1.8.0/test/test_sig_peps.py`

 * *Files identical despite different names*

### Comparing `bakta-1.7.0/test/test_user_proteins.py` & `bakta-1.8.0/test/test_user_proteins.py`

 * *Files 8% similar despite different names*

```diff
@@ -131,29 +131,28 @@
 
 
 def write_tmp_faa(aa, aa_path):
     with aa_path.open('w') as fh:
         fh.write(f">{aa['id']} {aa['description']}\n{aa['sequence']}\n")
 
 
-@pytest.mark.slow
 @pytest.mark.parametrize(
     "parameters",
     [
         'test/data/user-proteins.faa',
         'test/data/user-proteins.faa.gz',
         'test/data/user-proteins.gbff',
         'test/data/user-proteins.gbff.gz'
     ]
 )
 def test_user_proteins(parameters, tmpdir):
     # fast test skipping all feature detections
     proc = run(
         [
-            'bin/bakta', '--db', 'test/db', '--output', tmpdir, '--prefix', 'test', '--proteins', parameters,
+            'bin/bakta', '--db', 'test/db', '--output', tmpdir, '--force', '--prefix', 'test', '--proteins', parameters,
             '--skip-tmrna', '--skip-trna', '--skip-rrna', '--skip-ncrna', '--skip-ncrna-region', '--skip-crispr', '--skip-sorf', '--skip-ori', '--skip-gap', '--skip-plot',
             'test/data/NC_002127.1.fna'
         ]
     )
     assert proc.returncode == 0
 
     tmpdir_path = Path(tmpdir)
```

