# Comparing `tmp/trand-23.2.20.tar.gz` & `tmp/trand-23.5.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trand-23.2.20.tar", last modified: Tue Mar 14 14:06:28 2023, max compression
+gzip compressed data, was "trand-23.5.30.tar", last modified: Tue May 30 21:17:47 2023, max compression
```

## Comparing `trand-23.2.20.tar` & `trand-23.5.30.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxrwxr-x   0 moskalenko  (1005) ufhpc     (1000)        0 2023-03-14 14:06:28.214176 trand-23.2.20/
--rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)     1127 2021-08-19 19:58:57.000000 trand-23.2.20/LICENSE
--rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)     2954 2023-03-14 14:06:28.215720 trand-23.2.20/PKG-INFO
--rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)     2207 2022-10-19 14:40:40.000000 trand-23.2.20/README.md
--rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)      104 2021-08-19 19:58:57.000000 trand-23.2.20/pyproject.toml
--rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)     1458 2023-03-14 14:06:28.219757 trand-23.2.20/setup.cfg
--rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)       94 2021-08-19 19:58:57.000000 trand-23.2.20/setup.py
-drwxrwxr-x   0 moskalenko  (1005) ufhpc     (1000)        0 2023-03-14 14:06:27.865571 trand-23.2.20/src/
-drwxrwxr-x   0 moskalenko  (1005) ufhpc     (1000)        0 2023-03-14 14:06:28.145326 trand-23.2.20/src/trand/
--rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)       37 2021-08-19 19:58:57.000000 trand-23.2.20/src/trand/__init__.py
--rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)     4460 2021-10-22 15:41:59.000000 trand-23.2.20/src/trand/bedtools.py
--rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)     4805 2021-09-23 17:42:27.000000 trand-23.2.20/src/trand/calculate_complexity.py
--rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)    22111 2022-09-19 13:03:30.000000 trand-23.2.20/src/trand/consolidation.py
--rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)    75526 2023-03-14 14:04:33.000000 trand-23.2.20/src/trand/event_analysis.py
--rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)     5299 2022-09-19 13:00:47.000000 trand-23.2.20/src/trand/io.py
--rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)    11880 2023-02-09 17:45:13.000000 trand-23.2.20/src/trand/main.py
--rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)    28118 2022-09-19 13:00:47.000000 trand-23.2.20/src/trand/minimum_distance.py
--rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)     2481 2021-08-19 19:58:57.000000 trand-23.2.20/src/trand/plot_events.py
--rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)    50712 2022-12-15 15:47:58.000000 trand-23.2.20/src/trand/plot_functions.py
--rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)     4104 2022-09-19 13:00:47.000000 trand-23.2.20/src/trand/plot_one_gtf_gene.py
--rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)     1824 2022-09-20 20:01:39.000000 trand-23.2.20/src/trand/plot_one_gtf_pairwise.py
--rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)    18111 2022-09-20 20:01:39.000000 trand-23.2.20/src/trand/plot_transcriptome.py
--rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)     9707 2022-10-13 14:42:45.000000 trand-23.2.20/src/trand/plot_two_gtf_pairwise.py
--rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)    22019 2022-12-15 15:47:58.000000 trand-23.2.20/src/trand/transcript_distance.py
-drwxrwxr-x   0 moskalenko  (1005) ufhpc     (1000)        0 2023-03-14 14:06:28.208666 trand-23.2.20/src/trand.egg-info/
--rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)     2954 2023-03-14 14:06:27.000000 trand-23.2.20/src/trand.egg-info/PKG-INFO
--rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)      699 2023-03-14 14:06:27.000000 trand-23.2.20/src/trand.egg-info/SOURCES.txt
--rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)        1 2023-03-14 14:06:27.000000 trand-23.2.20/src/trand.egg-info/dependency_links.txt
--rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)       41 2023-03-14 14:06:27.000000 trand-23.2.20/src/trand.egg-info/entry_points.txt
--rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)        1 2021-08-19 23:31:43.000000 trand-23.2.20/src/trand.egg-info/not-zip-safe
--rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)       98 2023-03-14 14:06:27.000000 trand-23.2.20/src/trand.egg-info/requires.txt
--rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)        6 2023-03-14 14:06:27.000000 trand-23.2.20/src/trand.egg-info/top_level.txt
+drwxrwxr-x   0 moskalenko  (1005) ufhpc     (1000)        0 2023-05-30 21:17:47.865136 trand-23.5.30/
+-rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)     1127 2021-08-19 19:58:57.000000 trand-23.5.30/LICENSE
+-rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)     3289 2023-05-30 21:17:47.866573 trand-23.5.30/PKG-INFO
+-rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)     2207 2022-10-19 14:40:40.000000 trand-23.5.30/README.md
+-rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)      104 2021-08-19 19:58:57.000000 trand-23.5.30/pyproject.toml
+-rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)     1458 2023-05-30 21:17:47.870128 trand-23.5.30/setup.cfg
+-rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)       94 2021-08-19 19:58:57.000000 trand-23.5.30/setup.py
+drwxrwxr-x   0 moskalenko  (1005) ufhpc     (1000)        0 2023-05-30 21:17:47.619129 trand-23.5.30/src/
+drwxrwxr-x   0 moskalenko  (1005) ufhpc     (1000)        0 2023-05-30 21:17:47.828750 trand-23.5.30/src/trand/
+-rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)       37 2021-08-19 19:58:57.000000 trand-23.5.30/src/trand/__init__.py
+-rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)     4460 2021-10-22 15:41:59.000000 trand-23.5.30/src/trand/bedtools.py
+-rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)     4805 2021-09-23 17:42:27.000000 trand-23.5.30/src/trand/calculate_complexity.py
+-rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)    71233 2023-05-30 21:15:45.000000 trand-23.5.30/src/trand/event_analysis.py
+-rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)     5299 2022-09-19 13:00:47.000000 trand-23.5.30/src/trand/io.py
+-rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)    10457 2023-05-30 21:15:45.000000 trand-23.5.30/src/trand/main.py
+-rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)    25531 2023-05-30 21:15:45.000000 trand-23.5.30/src/trand/minimum_distance.py
+-rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)     2481 2021-08-19 19:58:57.000000 trand-23.5.30/src/trand/plot_events.py
+-rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)    49963 2023-05-30 21:15:45.000000 trand-23.5.30/src/trand/plot_functions.py
+-rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)     4104 2022-09-19 13:00:47.000000 trand-23.5.30/src/trand/plot_one_gtf_gene.py
+-rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)     1824 2022-09-20 20:01:39.000000 trand-23.5.30/src/trand/plot_one_gtf_pairwise.py
+-rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)    18075 2023-05-30 21:15:45.000000 trand-23.5.30/src/trand/plot_transcriptome.py
+-rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)     9707 2022-10-13 14:42:45.000000 trand-23.5.30/src/trand/plot_two_gtf_pairwise.py
+-rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)    20790 2023-05-30 21:15:45.000000 trand-23.5.30/src/trand/transcript_distance.py
+drwxrwxr-x   0 moskalenko  (1005) ufhpc     (1000)        0 2023-05-30 21:17:47.861056 trand-23.5.30/src/trand.egg-info/
+-rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)     3289 2023-05-30 21:17:47.000000 trand-23.5.30/src/trand.egg-info/PKG-INFO
+-rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)      672 2023-05-30 21:17:47.000000 trand-23.5.30/src/trand.egg-info/SOURCES.txt
+-rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)        1 2023-05-30 21:17:47.000000 trand-23.5.30/src/trand.egg-info/dependency_links.txt
+-rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)       42 2023-05-30 21:17:47.000000 trand-23.5.30/src/trand.egg-info/entry_points.txt
+-rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)        1 2021-08-19 23:31:43.000000 trand-23.5.30/src/trand.egg-info/not-zip-safe
+-rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)       98 2023-05-30 21:17:47.000000 trand-23.5.30/src/trand.egg-info/requires.txt
+-rw-rw-r--   0 moskalenko  (1005) ufhpc     (1000)        6 2023-05-30 21:17:47.000000 trand-23.5.30/src/trand.egg-info/top_level.txt
```

### Comparing `trand-23.2.20/LICENSE` & `trand-23.5.30/LICENSE`

 * *Files identical despite different names*

### Comparing `trand-23.2.20/PKG-INFO` & `trand-23.5.30/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,64 @@
 Metadata-Version: 2.1
 Name: trand
-Version: 23.2.20
+Version: 23.5.30
 Summary: 'Transcript Distances'
 Home-page: https://github.com/McIntyre-Lab/TranD
 Author: McIntyre Lab, Universify of Florida
 Author-email: om@rc.ufl.edu
 License: MIT
+Description: # TranD: Transcript Distances
+        
+        TranD is a collection of tools to facilitate metrics of structural variation for whole genome
+        transcript annotation files (GTF) that pinpoint structural variation to the nucleotide level.
+        
+        TranD (Transcript Distances) can be used to calculate metrics of structural variation within and
+        between annotation files (GTF). Structural variation reflects organismal complexity and three
+        summary metrics for genome level complexity are calculated for every gene in a GTF file:  1) the
+        number of transcripts per gene; 2) the number of exons per transcript; and 3) the number of
+        unique exons (exons with unique genomic coordinates) per gene. From each these metrics
+        distributions a summary statistics such as mean, median, variance, inter-quartile range are
+        calculated. With 1GTF file input, gene mode can be used to generates these metrics for each gene
+        and summary statistics and distributions across genes. Distributions are visualized in a series
+        of plots.  For 1 GTF and 2GTF a pairwise mode calculates distance metrics between 2 transcripts
+        to the nucleotide.  In 1 GTF this is all possible pairs within the gene and in 2 GTF model this
+        is all possible pairs among GTF files. The distribution of these metrics across genes are
+        visualized and summary statistics for structural variations between pairs are calculated and
+        reported.  Visualizations of the distributions of the frequency of intron retention, alternative
+        exon usage, donor/acceptor variation and 5', 3' variation in UTR regions are provided as well as
+        tabular formatted nucleotide level distances for both 1GTF and 2 GTF.
+        
+        ## Installation
+        
+        The easiest way to install TranD is by using conda or mamba.
+        
+        ```
+        conda install -c bioconda trand
+        ```
+        
+        If you already have a suitable environment with bedtools installed and only want to add python
+        packages run
+        ```
+        pip install trand
+        ```
+        in an activated conda or virtualenv environment
+        
+        If you clone this repository you can use the source/requirements.txt file to pip install required dependencies with
+        ```
+        pip install -r source/requirements.txt
+        ```
+        See the [PyPI TranD page](https://pypi.org/project/trand/) for reference.
+        
+        We will add a conda trand package in the near future.
+        
 Keywords: transcript event and distance analysis
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# TranD: Transcript Distances
-
-TranD is a collection of tools to facilitate metrics of structural variation for whole genome
-transcript annotation files (GTF) that pinpoint structural variation to the nucleotide level.
-
-TranD (Transcript Distances) can be used to calculate metrics of structural variation within and
-between annotation files (GTF). Structural variation reflects organismal complexity and three
-summary metrics for genome level complexity are calculated for every gene in a GTF file:  1) the
-number of transcripts per gene; 2) the number of exons per transcript; and 3) the number of
-unique exons (exons with unique genomic coordinates) per gene. From each these metrics
-distributions a summary statistics such as mean, median, variance, inter-quartile range are
-calculated. With 1GTF file input, gene mode can be used to generates these metrics for each gene
-and summary statistics and distributions across genes. Distributions are visualized in a series
-of plots.  For 1 GTF and 2GTF a pairwise mode calculates distance metrics between 2 transcripts
-to the nucleotide.  In 1 GTF this is all possible pairs within the gene and in 2 GTF model this
-is all possible pairs among GTF files. The distribution of these metrics across genes are
-visualized and summary statistics for structural variations between pairs are calculated and
-reported.  Visualizations of the distributions of the frequency of intron retention, alternative
-exon usage, donor/acceptor variation and 5', 3' variation in UTR regions are provided as well as
-tabular formatted nucleotide level distances for both 1GTF and 2 GTF.
-
-## Installation
-
-The easiest way to install TranD is by using conda or mamba.
-
-```
-conda install -c bioconda trand
-```
-
-If you already have a suitable environment with bedtools installed and only want to add python
-packages run
-```
-pip install trand
-```
-in an activated conda or virtualenv environment
-
-If you clone this repository you can use the source/requirements.txt file to pip install required dependencies with
-```
-pip install -r source/requirements.txt
-```
-See the [PyPI TranD page](https://pypi.org/project/trand/) for reference.
-
-We will add a conda trand package in the near future.
```

### Comparing `trand-23.2.20/README.md` & `trand-23.5.30/README.md`

 * *Files identical despite different names*

### Comparing `trand-23.2.20/setup.cfg` & `trand-23.5.30/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [global]
 quiet = 0
 
 [metadata]
 name = trand
-version = 23.02.20
+version = 23.05.30
 description = 'Transcript Distances'
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/McIntyre-Lab/TranD
 author = McIntyre Lab, Universify of Florida
 author_email = om@rc.ufl.edu
 license = MIT
```

### Comparing `trand-23.2.20/src/trand/bedtools.py` & `trand-23.5.30/src/trand/bedtools.py`

 * *Files identical despite different names*

### Comparing `trand-23.2.20/src/trand/calculate_complexity.py` & `trand-23.5.30/src/trand/calculate_complexity.py`

 * *Files identical despite different names*

### Comparing `trand-23.2.20/src/trand/event_analysis.py` & `trand-23.5.30/src/trand/event_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,34 +54,28 @@
 from . import plot_two_gtf_pairwise as P2GP
 from . import plot_one_gtf_pairwise as P1GP
 from . import plot_one_gtf_gene as P1GG
 
 # Import complexity calculation function
 from . import calculate_complexity as COMP
 
-# Import consolidation function
-from . import consolidation as CONSOL
-
 # CONFIGURATION
 # Output columns
 jct_df_cols = ['gene_id', 'transcript_id', 'coords']
 er_df_cols = ['gene_id', 'er_id', 'er_chr', 'er_start', 'er_end', 'er_strand', 'er_exon_ids',
               'er_transcript_ids', 'gene_transcript_ids', 'exons_per_er', 'transcripts_per_er',
               'transcripts_per_gene',  'er_ir_flag', 'er_annotation_frequency']
 ea_df_cols = ['gene_id', 'transcript_1', 'transcript_2', 'transcript_id', 'ef_id', 'ef_chr',
               'ef_start', 'ef_end', 'ef_strand', 'ef_ir_flag', 'er_id', 'er_chr', 'er_start',
               'er_end', 'er_strand']
 ef_df_cols = ['gene_id', 'er_id', 'ef_id', 'ef_chr', 'ef_start', 'ef_end', 'ef_strand',
               'ef_exon_ids', 'ef_transcript_ids', 'exons_per_ef', 'transcripts_per_ef',
               'ef_ir_flag', 'ea_annotation_frequency']
 ir_df_cols = ['er_transcript_ids']
 ue_df_cols = ['gene_id', 'num_uniq_exon']
-consol_key_cols = ['gene_id', 'transcript_id', 'consolidation_transcript_id',
-                   "num_transcript_in_consol_transcript", "num_transcript_id_in_gene",
-                   "num_consol_transcript_id_in_gene", "flag_gene_consolidated"]
 
 # Set start method of multiprocessing to forkserver
 #set_start_method("forkserver")
 
 # Parallelization result lists
 #ea_list = []
 #jct_list = []
@@ -137,38 +131,14 @@
         list_of_lists.append(lst[element:element + splitSize])
     return list_of_lists
 
 
 def callback(result):
     print("Received result:"+result.get())
 
-#def callback_pair_results(results):
-#    # Callback function to append result to list of results for pairwise mode
-#    ea_data_cat, jct_data_cat, td_data_cat = results
-#    ea_list.append(ea_data_cat)
-#    jct_list.append(jct_data_cat)
-#    td_list.append(td_data_cat)
-
-
-#def callback_gene_results(results):
-#    # Callback function to append result to list of results for gene mode
-#    er_data_cat, ef_data_cat, jct_data_cat, ir_data_cat = results
-#    er_list.append(er_data_cat)
-#    ef_list.append(ef_data_cat)
-#    jct_list.append(jct_data_cat)
-#    ir_list.append(ir_data_cat)
-
-
-#def callback_consol_results(results):
-#    # Callback function to append results to list of results for consolidation
-#    data, genes, keys = results
-#    data_list.append(data)
-#    keys_list.append(keys)
-
-
 def _create_bed_df(tx_str):
     """Create a data structure resembling a bed record for a transcript"""
     # logger.debug("TX STR: {}", tx_str)
     bed_df = pd.DataFrame(tx_str, columns=['chrom', 'start', 'end', 'name', 'score', 'strand'])
     bed_df['start'] = bed_df['start'].astype(int)
     bed_df['end'] = bed_df['end'].astype(int)
     bed_df = bed_df.sort_values('start')
@@ -1048,16 +1018,15 @@
         ea_data, jct_data, td_data = do_ea_pair(tx_pair_data)
         ea_df = pd.concat([ea_df, ea_data], axis=0, ignore_index=True)
         jct_df = pd.concat([jct_df, jct_data], axis=0, ignore_index=True)
         td_df = pd.concat([td_df, td_data], axis=0, ignore_index=True)
     return ea_df, jct_df, td_df
 
 def process_single_file(infile, ea_mode, keep_ir, outdir, outfiles, cpu_cores,
-                        complexity_only, skip_plots, skip_interm, consolidate,
-                        consol_prefix, consol_outfiles, output_prefix):
+                        complexity_only, skip_plots, skip_interm, output_prefix):
     """
     Pairwise or full gene transcript event analysis (TranD) on a single GTF file.
     """
     logger.info("Input file: {}", infile)
     if skip_interm:
         del(outfiles['ea_fh'])
         del(outfiles['er_fh'])
@@ -1078,74 +1047,22 @@
     genes = data.groupby("gene_id")
     transcripts = data.groupby(["gene_id", "transcript_id"])
     logger.info("Found {} genes and {} transcripts", len(genes), len(transcripts))
 
     # Set up parallel manager for if >1 cpu provided
     with Manager() as manager1:
 
-        # If requested, consolidate transcripts with identical junctions
-        #   (remove 5'/3' variation in redundantly spliced transcripts)
-        if consolidate:
-            logger.info("Consolidation of transcript with identical junctions.")
-            # Open consolidation output files
-            if not skip_interm:
-                if output_prefix is not None:
-                    prefix_consol_outfiles = {
-                        k: "{}_{}".format(output_prefix, v) for k, v in consol_outfiles.items()
-                    }
-                    consol_fhs = open_output_files(outdir, prefix_consol_outfiles)
-                else:
-                    consol_fhs = open_output_files(outdir, consol_outfiles)
-                consol_fhs["key_fh"].write_text(",".join(consol_key_cols) + "\n")
-            # Serial consolidation
-            if cpu_cores == 1:
-                data, genes, keys = CONSOL.consolidate_transcripts(data, consol_prefix,
-                                                                   genes.groups)
-            # Parallel consolidation
-            else:
-                # Generate multiprocess Pool with specified number of cpus
-                #     to loop through genes and consolidate
-                # Create shared lists that can be accessed by multiple processes
-                data_list = manager1.list()
-                keys_list = manager1.list()
-                # Create process pool
-                pool = Pool(cpu_cores)
-                for gene in list(genes.groups):
-                    pool.apply_async(process_consol, args=(
-                            data,
-                            consol_prefix,
-                            [gene],
-                            data_list,
-                            keys_list
-                        ))
-                pool.close()
-                pool.join()
-                # Concatenate parallel consolidation output
-                data = pd.concat(data_list, ignore_index=True)
-                genes = data.groupby("gene_id")
-                keys = pd.concat(keys_list, ignore_index=True)
-    
-            # Output consolidated GTF and key file
-            if not skip_interm:
-                write_gtf(data, consol_fhs, "consol_gtf_fh")
-                write_output(keys, consol_fhs, "key_fh")
-            # Output gene and transcript counts after consolidation
-            num_tx = data.groupby(["gene_id", "transcript_id"])
-            logger.info(
-                "After consolidation: {} genes and {} transcripts", len(genes), len(num_tx)
-            )
-    
         # Output complexity measures using GTF data
         uniq_ex = COMP.calculate_complexity(outdir, data, skip_plots, output_prefix)
-    
+
         # If requested, skip all other functions
         if complexity_only:
             logger.info("Complexity only option selected. Skipping all other functions.")
             return
-    
+
         # Full processing
         if output_prefix is not None:
             prefix_outfiles = {
                 k: "{}_{}".format(output_prefix,v) for k,v in outfiles.items()
             }
             out_fhs = open_output_files(outdir, prefix_outfiles)
         else:
@@ -1187,15 +1104,15 @@
                     write_output(uniq_ex, out_fhs, 'ue_fh')
                 # Output plots for 1 GTF gene mode
                 if not skip_plots:
                     P1GG.plot_one_gtf_gene(er_data, ef_data, ir_df, uniq_ex, outdir, prefix=output_prefix)
             # Pairwise EA
             else:
                 # Set up results lists (no managers needed since on 1 cpu)
-                result_managers = {"ea_list":[],  "jct_list":[], "ir_list":[]}
+                result_managers = {"ea_list":[],  "jct_list":[], "ir_list":[], "td_list":[]}
                 ea_data, jct_data, td_data = loop_over_genes(
                         list(genes.groups),
                         out_fhs,
                         "pairwise",
                         keep_ir,
                         data,
                         result_managers
@@ -1425,15 +1342,15 @@
 
     # Set up parallel manager for if >1 cpu provided
     with Manager() as manager2:
 
         # Serial processing
         if cpu_cores == 1:
             # Set up results lists (no managers needed since on 1 cpu)
-            result_managers = {"ea_list":[],  "jct_list":[], "ir_list":[]}
+            result_managers = {"ea_list":[],  "jct_list":[], "ir_list":[], "td_list":[]}
             ea_data, jct_data, td_data = loop_over_genes(
                     gene_list,
                     out_fhs,
                     "pairwise",
                     True,
                     valid_f1,
                     result_managers,
@@ -1531,27 +1448,14 @@
             for transcript in transcript_groups:
                 transcript_df = f1_data[(f1_data["gene_id"] == gene) & (f1_data['transcript_id'] == transcript)]
                 tx_data[transcript] = transcript_df
             for pair in itertools.combinations(tx_data.keys(), 2):
                 yield pair
 
 
-def process_consol(data, consol_prefix, gene, data_list, keys_list):
-    """
-    Loop over genes in given gene list and consolidate identical splice junctions
-        within each gene
-    NOTE: Currently gene must be a list with a single gene value in it since the
-        consolidation function utilizes a loop over a list of genes
-    """
-    subset_data = data[data["gene_id"] == gene[0]]
-    consol_data, consol_genes, keys = CONSOL.consolidate_transcripts(subset_data, consol_prefix, gene)
-    data_list.append(consol_data)
-    keys_list.append(keys)
-
-
 def loop_over_genes(gene_list, out_fhs, ea_mode, keep_ir, data1, result_managers,
                     data2=None, name1=None, name2=None):
     """
     Loop over genes in given gene list and process based on the files input:
         1. If data1, data2, name1, and name2 provided then do 2 GTF analysis
         2. If data1 provided and not data2 then do 1 GTF analysis based on ea_mode
     NOTE: This function should only be used for single CPU processing
@@ -1682,15 +1586,15 @@
             |(data1['transcript_id'] == pair[1])]
         ea_data, jct_data, td_data = ea_pairwise("", pair_df)
 
         # Append output to lists
         result_managers["ea_list"].append(ea_data)
         result_managers["jct_list"].append(jct_data)
         result_managers["td_list"].append(td_data)
-        
+
     # Concatenate and return outputs if result managers are lists (from single cpu)
     if type(result_managers["jct_list"]) is list:
         logger.debug("Single CPU concatenation of lists")
         ea_data_cat = pd.concat(result_managers["ea_list"], ignore_index=True)
         jct_data_cat = pd.concat(result_managers["jct_list"], ignore_index=True)
         td_data_cat = pd.concat(result_managers["td_list"], ignore_index=True)
         return [ea_data_cat, jct_data_cat, td_data_cat]
```

### Comparing `trand-23.2.20/src/trand/io.py` & `trand-23.5.30/src/trand/io.py`

 * *Files identical despite different names*

### Comparing `trand-23.2.20/src/trand/main.py` & `trand-23.5.30/src/trand/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,18 +45,14 @@
     "ue_fh": "uniq_exons_per_gene.csv",
 }
 two_gtfs_outfiles = {
     "gtf1_fh": "gtf1_only.gtf",
     "gtf2_fh": "gtf2_only.gtf",
     "md_fh": "minimum_pairwise_transcript_distance.csv",
 }
-consol_outfiles = {
-    "key_fh": "transcript_id_2_consolidation_id.csv",
-    "consol_gtf_fh": "consolidated_transcriptome.gtf",
-}
 
 
 def parse_args(print_help=False):
     """Parse command-line arguments"""
 
     class MyParser(argparse.ArgumentParser):
         """Subclass ArgumentParser for better help printing"""
@@ -101,37 +97,19 @@
         action="store",
         type=str,
         default=None,
         required=False,
         help="Log file name for logging processing events to file.",
     )
     parser.add_argument(
-        "--consolidate",
-        dest="consolidate",
-        action="store_true",
-        help="""Used with 1 GTF input file. Consolidate transcripts remove 5'/3' transcript end
-        variation in redundantly spliced transcripts) with identical junctions prior to complexity
-        calculations, events and summary plotting. Default: No consolidation""",
-    )
-    parser.add_argument(
-        "--consolPrefix",
-        dest="consol_prefix",
-        type=str,
-        default="tr",
-        help="""Used with 1 GTF input file. Requires '--consolidate' flag. Specify the prefix to use
-        for consolidated transcript_id values. Prefix must be alphanumeric with no spaces.
-        Underscore (\"_\") is the only allowed special character. Default: 'tr'""",
-    )
-    parser.add_argument(
         "-c",
         "--complexityOnly",
         dest="complexity_only",
         action="store_true",
-        help="""Used with 1 or 2 GTF input file(s). Output only complexity measures. If used in
-        presence of the '--consolidate' flag, complexity is calculated on the consolidated GTF(s).
+        help="""Used with 1 or 2 GTF input file(s). Output only transcriptome complexity measures.
         Default: Perform all analyses and comparisons including complexity calculations""",
     )
     parser.add_argument(
         "-e",
         "--ea",
         dest="ea_mode",
         type=str,
@@ -231,22 +209,14 @@
     if args.ea_mode == "gene":
         if len(args.infiles) > 1:
             logger.warning(
                 "EA 'gene' mode is ignored for two GTF files - only pairwise is done."
             )
     regex = re.compile(r"^\w+$", re.ASCII)
     # Validate prefixes
-    if not regex.match(args.consol_prefix):
-        logger.error(
-            "Invalid prefix format for consolidated transcript_id values: "
-            "Must be alphanumeric."
-            "Only '_' (underscore) special character is allowed"
-        )
-        parser.print_help()
-        sys.exit(2)
     if not regex.match(args.name1):
         logger.error(
             "Invalid name for dataset 1: Must be alphanumeric and can only "
             "include '_' special character"
         )
         parser.print_help()
         sys.exit(2)
@@ -321,17 +291,14 @@
                 args.keep_ir,
                 args.outdir,
                 outfiles,
                 args.cpu_cores,
                 args.complexity_only,
                 args.skip_plots,
                 args.skip_interm,
-                args.consolidate,
-                args.consol_prefix,
-                consol_outfiles,
                 args.prefix,
             )
         finally:
             # Only for bedtools. Remove when bedtools are refactored out.
             cleanup()
     else:
         logger.debug("Two files pairwise analysis")
```

### Comparing `trand-23.2.20/src/trand/plot_events.py` & `trand-23.5.30/src/trand/plot_events.py`

 * *Files identical despite different names*

### Comparing `trand-23.2.20/src/trand/plot_functions.py` & `trand-23.5.30/src/trand/plot_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,44 +12,44 @@
 from matplotlib.colors import ListedColormap
 import seaborn as sns
 from upsetplot import UpSet
 
 #  Plot Functions
 
 
-def plot_transcript_in_gene_split_pie(
+def plot_transcript_inGene_split_pie(
     md_data, f1_odds, f2_odds, name1, name2, legendOut
 ):
     """
     Plot pie charts for the number of genes where the transcripts are the same,
             where one dataset has more transcripts that the onther, and where
             genes are exclusive (pie chart for all genes, single transcript in
             at least one dataset, multi-transcript in at least one dataset, and
             multi-transcript in both datasets
     """
     # Get counts
-    cols = {"transcript_id": "num_transcript_in_gene_" + name1}
+    cols = {"transcript_id": "num_transcript_inGene_" + name1}
     geneF1only = (
         f1_odds.groupby("gene_id")["transcript_id"]
         .nunique()
         .reset_index()
         .rename(columns=cols)
     )
 
-    geneF1only["num_transcript_in_gene_" + name2] = 0
-    geneF1only["transcript_in_gene"] = name1 + "_only"
-    cols = {"transcript_id": "num_transcript_in_gene_" + name2}
+    geneF1only["num_transcript_inGene_" + name2] = 0
+    geneF1only["transcript_inGene"] = name1 + "_only"
+    cols = {"transcript_id": "num_transcript_inGene_" + name2}
     geneF2only = (
         f2_odds.groupby("gene_id")["transcript_id"]
         .nunique()
         .reset_index()
         .rename(columns=cols)
     )
-    geneF2only["num_transcript_in_gene_" + name1] = 0
-    geneF2only["transcript_in_gene"] = name2 + "_only"
+    geneF2only["num_transcript_inGene_" + name1] = 0
+    geneF2only["transcript_inGene"] = name2 + "_only"
 
     # Make dictionary of names for plot and order
     geneCountNameDict = {
         "match": "Match",
         name1 + "_greater": name1 + " Greater",
         name2 + "_greater": name2 + " Greater",
         name1 + "_only": name1 + " Only",
@@ -71,70 +71,70 @@
     # 4) genes with > 1 xcrpt for both
     fig = plt.figure()
     for num in range(1, 5):
         ax = plt.subplot2grid((2, 2), (abs(num % 2 - 1), int(num / 3)), fig=fig)
         if num == 1:
             geneCount = pd.concat(
                 [
-                    md_data[["gene_id", "transcript_in_gene"]].drop_duplicates(),
+                    md_data[["gene_id", "transcript_inGene"]].drop_duplicates(),
                     geneF1only,
                     geneF2only,
                 ],
                 ignore_index=True,
                 sort=False,
-            )["transcript_in_gene"].value_counts(sort=False)
+            )["transcript_inGene"].value_counts(sort=False)
             title = "All Genes (n = {})".format(geneCount.sum())
             totalGenes = geneCount.sum()
             legendLabels = geneCount.reindex(list(geneCountOrderDict)).index.map(
                 geneCountNameDict
             )
         elif num == 2:
             geneCount = pd.concat(
                 [
                     md_data[
-                        (md_data["num_transcript_in_gene_" + name1] == 1)
-                        | (md_data["num_transcript_in_gene_" + name2] == 1)
-                    ][["gene_id", "transcript_in_gene"]].drop_duplicates(),
-                    geneF1only[geneF1only["num_transcript_in_gene_" + name1] == 1],
-                    geneF2only[geneF2only["num_transcript_in_gene_" + name2] == 1],
+                        (md_data["num_transcript_inGene_" + name1] == 1)
+                        | (md_data["num_transcript_inGene_" + name2] == 1)
+                    ][["gene_id", "transcript_inGene"]].drop_duplicates(),
+                    geneF1only[geneF1only["num_transcript_inGene_" + name1] == 1],
+                    geneF2only[geneF2only["num_transcript_inGene_" + name2] == 1],
                 ],
                 ignore_index=True,
                 sort=False,
-            )["transcript_in_gene"].value_counts(sort=False)
+            )["transcript_inGene"].value_counts(sort=False)
             title = "Genes with 1 Transcript\n(in at least one dataset, n = {})".format(
                 geneCount.sum()
             )
         elif num == 3:
             geneCount = pd.concat(
                 [
-                    geneF1only[geneF1only["num_transcript_in_gene_" + name1] > 1],
-                    geneF2only[geneF2only["num_transcript_in_gene_" + name2] > 1],
+                    geneF1only[geneF1only["num_transcript_inGene_" + name1] > 1],
+                    geneF2only[geneF2only["num_transcript_inGene_" + name2] > 1],
                 ],
                 ignore_index=True,
                 sort=False,
-            )["transcript_in_gene"].value_counts(sort=False)
+            )["transcript_inGene"].value_counts(sort=False)
             title = "Genes with >1 Transcript\n(exclusive to one dataset, n = {})".format(
                 geneCount.sum()
             )
         else:
             geneCount = (
                 md_data[
-                    (md_data["num_transcript_in_gene_" + name1] > 1)
-                    & (md_data["num_transcript_in_gene_" + name2] > 1)
-                ][["gene_id", "transcript_in_gene"]]
-                .drop_duplicates()["transcript_in_gene"]
+                    (md_data["num_transcript_inGene_" + name1] > 1)
+                    & (md_data["num_transcript_inGene_" + name2] > 1)
+                ][["gene_id", "transcript_inGene"]]
+                .drop_duplicates()["transcript_inGene"]
                 .value_counts(sort=False)
             )
             title = "Genes with >1 Transcript\n(in both datasets, n = {})".format(
                 geneCount.sum()
             )
         if len(geneCount) > 0:
             geneCount.reindex(list(geneCountOrderDict)).plot(
                 kind="pie",
-                y="transcript_in_gene",
+                y="transcript_inGene",
                 labels=None,
                 figsize=(12, 6),
                 autopct=(lambda pct: get_pie_label(pct, geneCount)),
                 colormap=ListedColormap(sns.color_palette("colorblind", 15).as_hex()),
                 ax=ax,
             )
         else:
@@ -188,20 +188,20 @@
     Plot a stacked bar chart of the genes with reciprocal minimum pairs for all transcript pairs
     possible (Match: Reciprocal Pairs or Greater: Reciprocal Pairs), only some of the transcript
     pairs (Match: Partial Reciprocal Pairs or Greater: Partial Reciprocal Pairs), or none of the
     transcript pars (Match: No Reciprocal Pairs or Greater: No Reciprocal Pairs) using gene counts
     or proportions of Match or Greater genes
     """
     genePairDF = (
-        md_data.groupby(["transcript_in_gene", "recip_min_pair_in_gene"])["gene_id"]
+        md_data.groupby(["transcript_inGene", "recip_min_pair_inGene"])["gene_id"]
         .nunique()
         .reset_index()
         .pivot_table(
-            index=["transcript_in_gene"],
-            columns="recip_min_pair_in_gene",
+            index=["transcript_inGene"],
+            columns="recip_min_pair_inGene",
             values="gene_id",
         )
     )
     for col in ["reciprocal_pairs", "partial_reciprocal_pairs", "no_reciprocal_pairs"]:
         if col not in genePairDF.columns:
             genePairDF[col] = 0
     genePairDF = genePairDF.fillna(0)
@@ -292,87 +292,87 @@
             r"\b Figure. Classification of transcript pairs \b0 \line {}".format(
                 legendText
             )
         )
         end_rtf(outFile)
 
 
-def plot_transcript_in_gene_upset(md_data, f1_odds, f2_odds, name1, name2, legendOut):
+def plot_transcript_inGene_upset(md_data, f1_odds, f2_odds, name1, name2, legendOut):
     """
     UpSet plot for number of transcripts in genes
     """
     geneF1only = (
         f1_odds.groupby("gene_id")["transcript_id"]
         .nunique()
         .reset_index()
-        .rename(columns={"transcript_id": "num_transcript_in_gene_" + name1})
+        .rename(columns={"transcript_id": "num_transcript_inGene_" + name1})
     )
-    geneF1only["num_transcript_in_gene_" + name2] = 0
-    geneF1only["transcript_in_gene"] = name1 + "_only"
+    geneF1only["num_transcript_inGene_" + name2] = 0
+    geneF1only["transcript_inGene"] = name1 + "_only"
     geneF2only = (
         f2_odds.groupby("gene_id")["transcript_id"]
         .nunique()
         .reset_index()
-        .rename(columns={"transcript_id": "num_transcript_in_gene_" + name2})
+        .rename(columns={"transcript_id": "num_transcript_inGene_" + name2})
     )
-    geneF2only["num_transcript_in_gene_" + name1] = 0
-    geneF2only["transcript_in_gene"] = name2 + "_only"
+    geneF2only["num_transcript_inGene_" + name1] = 0
+    geneF2only["transcript_inGene"] = name2 + "_only"
     geneAll = pd.concat(
         [
             md_data[
                 [
                     "gene_id",
-                    "num_transcript_in_gene_" + name1,
-                    "num_transcript_in_gene_" + name2,
-                    "transcript_in_gene",
+                    "num_transcript_inGene_" + name1,
+                    "num_transcript_inGene_" + name2,
+                    "transcript_inGene",
                 ]
             ].drop_duplicates(),
             geneF1only,
             geneF2only,
         ],
         ignore_index=True,
         sort=False,
     )
     colList = []
     # Flag when genes have 1-4 transcripts
     for num in range(1, 5):
         geneAll[str(num) + " Transcript(s) " + name1] = np.where(
-            geneAll["num_transcript_in_gene_" + name1] == num, True, False
+            geneAll["num_transcript_inGene_" + name1] == num, True, False
         )
         colList.append(str(num) + " Transcript(s) " + name1)
         geneAll[str(num) + " Transcript(s) " + name2] = np.where(
-            geneAll["num_transcript_in_gene_" + name2] == num, True, False
+            geneAll["num_transcript_inGene_" + name2] == num, True, False
         )
         colList.append(str(num) + " Transcript(s) " + name2)
     # Flag when genes have 5+ transcripts
     geneAll["5+ Transcript(s) " + name1] = np.where(
-        geneAll["num_transcript_in_gene_" + name1] >= 5, True, False
+        geneAll["num_transcript_inGene_" + name1] >= 5, True, False
     )
     colList.append("5+ Transcript(s) " + name1)
     geneAll["5+ Transcript(s) " + name2] = np.where(
-        geneAll["num_transcript_in_gene_" + name2] >= 5, True, False
+        geneAll["num_transcript_inGene_" + name2] >= 5, True, False
     )
     colList.append("5+ Transcript(s) " + name2)
     legendText = (
         "Rows indicate the number of transcripts in {} and {}. Columns are "
         "separated by unique combinations of the number of transcripts in "
         "{} and {}. When a gene is not present in one of the GTF files, only "
         "a single dot will be indicated. The number of genes (N = {}) for "
         "each nonoverlapping category are displayed in a histogram.".format(
             name1,
             name2,
             name1,
             name2,
             sum(
                 [
-                    get_value_count(geneAll, "transcript_in_gene", name1 + "_only"),
-                    get_value_count(geneAll, "transcript_in_gene", name2 + "_only"),
-                    get_value_count(geneAll, "transcript_in_gene", "match"),
-                    get_value_count(geneAll, "transcript_in_gene", name1 + "_greater"),
-                    get_value_count(geneAll, "transcript_in_gene", name2 + "_greater"),                    
+                    get_value_count(geneAll, "transcript_inGene", name1 + "_only"),
+                    get_value_count(geneAll, "transcript_inGene", name2 + "_only"),
+                    get_value_count(geneAll, "transcript_inGene", "match"),
+                    get_value_count(geneAll, "transcript_inGene", name1 + "_greater"),
+                    get_value_count(geneAll, "transcript_inGene", name2 + "_greater"),                    
                 ]
             ),
         )
     )
     plot_upset(
         geneAll.set_index(colList), "Number of Genes with Each Number of Transcripts"
     )
@@ -392,20 +392,20 @@
     For all reciprocal minimum pair transcripts or minimum pair of extra transcripts:
             Upset plot for the number of transcript pairs with each kind of
             alternative splicing (AS) and the distribution of nt differences
             between the pairs plotted
     """
     if reciprocal:
         # Plot only reciprocal minimum pairs
-        minPairAS = md_data[md_data["flag_recip_min_match"] == 1].copy()
+        minPairAS = md_data[md_data["flag_RMP"] == 1].copy()
     else:
         if pairs == None:
             # Plot only minimum pairs of extras, or those without a recip min pair
             minPairAS = md_data[
-                (md_data["flag_recip_min_match"] != 1)
+                (md_data["flag_RMP"] != 1)
                 & (
                     (md_data["flag_min_match_" + name1] == 1)
                     | (md_data["flag_min_match_" + name2] == 1)
                 )
             ].copy()
         elif pairs == "all":
             minPairAS = md_data[
@@ -424,39 +424,39 @@
     if len(minPairAS) == 0:
         return
     minPairAS = minPairAS[
         [
             "transcript_1",
             "transcript_2",
             "flag_alt_exon",
-            "flag_alt_donor_acceptor",
+            "flag_alt_DA",
             "flag_IR",
-            "flag_5_variation",
-            "flag_3_variation",
-            "flag_no_shared_nt",
-            "num_nt_diff",
-            "prop_nt_diff",
+            "flag_5_var",
+            "flag_3_var",
+            "flag_no_ovlp_nt",
+            "num_nt_noOvlp",
+            "prop_nt_noOvlp",
         ]
     ]
     # Set No Shared NT genes to have np.nan nucleotide difference
-    minPairAS["num_nt_diff"] = np.where(
-        minPairAS["flag_no_shared_nt"] == 1,
+    minPairAS["num_nt_noOvlp"] = np.where(
+        minPairAS["flag_no_ovlp_nt"] == 1,
         np.nan,
-        minPairAS["num_nt_diff"]
+        minPairAS["num_nt_noOvlp"]
     )
     minPairAS = minPairAS.rename(
         columns={
             "flag_alt_exon": "Alt. Exon",
-            "flag_alt_donor_acceptor": "Alt. Donor/Acceptor",
+            "flag_alt_DA": "Alt. Donor/Acceptor",
             "flag_IR": "Intron Retention",
-            "flag_5_variation": "5' Variation",
-            "flag_3_variation": "3' Variation",
-            "flag_no_shared_nt": "No Shared NT",
-            "num_nt_diff": "# NT Different",
-            "prop_nt_diff": "Proportion\nNT Different",
+            "flag_5_var": "5' Variation",
+            "flag_3_var": "3' Variation",
+            "flag_no_ovlp_nt": "No Shared NT",
+            "num_nt_noOvlp": "# NT Different",
+            "prop_nt_noOvlp": "Proportion\nNT Different",
         }
     )
     AScols = [
         "5' Variation",
         "3' Variation",
         "Alt. Donor/Acceptor",
         "Alt. Exon",
@@ -585,65 +585,65 @@
 def plot_gene_recip_min_AS_upset(md_data, name1, name2, legendOut):
     """
     Upset plot for number of genes with each kind of AS when comparing the
             reciprocally min match pairs of the two datasets with added box plots
             of the number of min match pairs present in the gene and the number
             of transcripts in each dataset
     """
-    recipMinPairAS = md_data[md_data["flag_recip_min_match"] == 1][
+    recipMinPairAS = md_data[md_data["flag_RMP"] == 1][
         [
             "gene_id",
-            "flag_alt_exon_recip_min_match",
-            "flag_alt_donor_acceptor_recip_min_match",
-            "flag_IR_recip_min_match",
-            "flag_5_variation_recip_min_match",
-            "flag_3_variation_recip_min_match",
-            "flag_no_shared_nt_recip_min_match",
-            "num_recip_min_match_in_gene",
-            "num_transcript_in_gene_" + name1,
-            "num_transcript_in_gene_" + name2,
+            "flag_alt_exon_RMP",
+            "flag_alt_DA_RMP",
+            "flag_IR_RMP",
+            "flag_5_var_RMP",
+            "flag_3_var_RMP",
+            "flag_no_ovlp_nt_RMP",
+            "num_RMP_inGene",
+            "num_transcript_inGene_" + name1,
+            "num_transcript_inGene_" + name2,
         ]
     ].copy()
     geneRecipMatchAS = (
         recipMinPairAS.groupby("gene_id")
         .agg(
             {
-                "flag_alt_exon_recip_min_match": "max",
-                "flag_alt_donor_acceptor_recip_min_match": "max",
-                "flag_IR_recip_min_match": "max",
-                "flag_5_variation_recip_min_match": "max",
-                "flag_3_variation_recip_min_match": "max",
-                "flag_no_shared_nt_recip_min_match": "max",
-                "num_recip_min_match_in_gene": "max",
-                "num_transcript_in_gene_" + name1: "max",
-                "num_transcript_in_gene_" + name2: "max",
+                "flag_alt_exon_RMP": "max",
+                "flag_alt_DA_RMP": "max",
+                "flag_IR_RMP": "max",
+                "flag_5_var_RMP": "max",
+                "flag_3_var_RMP": "max",
+                "flag_no_ovlp_nt_RMP": "max",
+                "num_RMP_inGene": "max",
+                "num_transcript_inGene_" + name1: "max",
+                "num_transcript_inGene_" + name2: "max",
             }
         )
         .reset_index()
     )
     geneFlagCols = [
-        "flag_alt_exon_recip_min_match",
-        "flag_alt_donor_acceptor_recip_min_match",
-        "flag_IR_recip_min_match",
-        "flag_5_variation_recip_min_match",
-        "flag_3_variation_recip_min_match",
-        "flag_no_shared_nt_recip_min_match",
+        "flag_alt_exon_RMP",
+        "flag_alt_DA_RMP",
+        "flag_IR_RMP",
+        "flag_5_var_RMP",
+        "flag_3_var_RMP",
+        "flag_no_ovlp_nt_RMP",
     ]
     geneRecipMatchAS[geneFlagCols] = geneRecipMatchAS[geneFlagCols].astype(bool)
     geneRecipMatchAS = geneRecipMatchAS.rename(
         columns={
-            "flag_alt_exon_recip_min_match": "Alt. Exon",
-            "flag_alt_donor_acceptor_recip_min_match": "Alt. Donor/Acceptor",
-            "flag_IR_recip_min_match": "Intron Retention",
-            "flag_5_variation_recip_min_match": "5' Variation",
-            "flag_3_variation_recip_min_match": "3' Variation",
-            "flag_no_shared_nt_recip_min_match": "No Shared NT",
-            "num_recip_min_match_in_gene": "# Recip. Min.\nTranscript Pairs",
-            "num_transcript_in_gene_" + name1: "# Transcripts\nin " + name1,
-            "num_transcript_in_gene_" + name2: "# Transcripts\nin " + name2,
+            "flag_alt_exon_RMP": "Alt. Exon",
+            "flag_alt_DA_RMP": "Alt. Donor/Acceptor",
+            "flag_IR_RMP": "Intron Retention",
+            "flag_5_var_RMP": "5' Variation",
+            "flag_3_var_RMP": "3' Variation",
+            "flag_no_ovlp_nt_RMP": "No Shared NT",
+            "num_RMP_inGene": "# Recip. Min.\nTranscript Pairs",
+            "num_transcript_inGene_" + name1: "# Transcripts\nin " + name1,
+            "num_transcript_inGene_" + name2: "# Transcripts\nin " + name2,
         }
     )
     AScols = [
         "5' Variation",
         "3' Variation",
         "Alt. Donor/Acceptor",
         "Alt. Exon",
@@ -666,15 +666,15 @@
         "minimum pairs). Box plots represent the number of reciprocal minimum "
         "pairs (blue) and the number of transcripts in {} (orange) and {} "
         "(green). Genes with \"No Shared NT\" have a pair of "
         "transcripts with nonoverlapping coordinates.".format(
             name1,
             name2,
             len(geneRecipMatchAS),
-            len(md_data[md_data["flag_recip_min_match"] == 1]),
+            len(md_data[md_data["flag_RMP"] == 1]),
             name1,
             name2,
         )
     )
     with open(legendOut, "w") as outFile:
         start_rtf(outFile)
         outFile.write(
@@ -694,32 +694,32 @@
     """
     pairAS = td_data[
         [
             "gene_id",
             "transcript_1",
             "transcript_2",
             "flag_alt_exon",
-            "flag_alt_donor_acceptor",
+            "flag_alt_DA",
             "flag_IR",
-            "flag_5_variation",
-            "flag_3_variation",
-            "flag_no_shared_nt",
+            "flag_5_var",
+            "flag_3_var",
+            "flag_no_ovlp_nt",
         ]
     ].copy()
     # Get AS flags at the gene level
     geneAS = (
         pairAS.groupby("gene_id")
         .agg(
             {
                 "flag_alt_exon": "max",
-                "flag_alt_donor_acceptor": "max",
+                "flag_alt_DA": "max",
                 "flag_IR": "max",
-                "flag_5_variation": "max",
-                "flag_3_variation": "max",
-                "flag_no_shared_nt": "max",
+                "flag_5_var": "max",
+                "flag_3_var": "max",
+                "flag_no_ovlp_nt": "max",
             }
         )
         .reset_index()
     )
     # Get the number of transcripts per gene by getting the unique list
     #   of transcript_1 and transcript_2
     transcriptPerGene = (
@@ -742,32 +742,32 @@
     mergeASxcrptPerGene = pd.merge(
         geneAS, transcriptPerGene, how="outer", on="gene_id", indicator="merge_check"
     )
     # Set AS flags to boolean values and rename
     geneFlagCols = [
         "gene_id",
         "flag_alt_exon",
-        "flag_alt_donor_acceptor",
+        "flag_alt_DA",
         "flag_IR",
-        "flag_5_variation",
-        "flag_3_variation",
-        "flag_no_shared_nt",
+        "flag_5_var",
+        "flag_3_var",
+        "flag_no_ovlp_nt",
     ]
     mergeASxcrptPerGene[geneFlagCols] = mergeASxcrptPerGene[geneFlagCols].astype(bool)
     mergeASxcrptPerGene = mergeASxcrptPerGene.rename(
         columns={
             "flag_alt_exon": "Alt. Exon",
-            "flag_alt_donor_acceptor": "Alt. Donor/Acceptor",
+            "flag_alt_DA": "Alt. Donor/Acceptor",
             "flag_IR": "Intron Retention",
-            "flag_5_variation": "5' Variation",
-            "flag_3_variation": "3' Variation",
-            "flag_no_shared_nt": "No Shared NT",
+            "flag_5_var": "5' Variation",
+            "flag_3_var": "3' Variation",
+            "flag_no_ovlp_nt": "No Shared NT",
             "num_transcript_per_gene": "# Transcripts\nPer Gene",
-            "num_nt_diff": "Avg #\nNT Different",
-            "prop_nt_diff": "Avg Proportion\nNT Different",
+            "num_nt_noOvlp": "Avg #\nNT Different",
+            "prop_nt_noOvlp": "Avg Proportion\nNT Different",
         }
     )
     AScols = [
         "5' Variation",
         "3' Variation",
         "Alt. Donor/Acceptor",
         "Alt. Exon",
@@ -808,54 +808,54 @@
     """
     pairAS = td_data[
         [
             "gene_id",
             "transcript_1",
             "transcript_2",
             "flag_alt_exon",
-            "flag_alt_donor_acceptor",
+            "flag_alt_DA",
             "flag_IR",
-            "flag_5_variation",
-            "flag_3_variation",
-            "flag_no_shared_nt",
-            "num_nt_diff",
-            "prop_nt_diff",
+            "flag_5_var",
+            "flag_3_var",
+            "flag_no_ovlp_nt",
+            "num_nt_noOvlp",
+            "prop_nt_noOvlp",
         ]
     ].copy()
     # Ensure number of nt different are int and float values
-    pairAS["num_nt_diff"] = pairAS["num_nt_diff"].astype(int)
-    pairAS["prop_nt_diff"] = pairAS["prop_nt_diff"].astype(float)
+    pairAS["num_nt_noOvlp"] = pairAS["num_nt_noOvlp"].astype(int)
+    pairAS["prop_nt_noOvlp"] = pairAS["prop_nt_noOvlp"].astype(float)
     # Set No Shared NT pairs to have np.nan nucleotide difference
-    pairAS["num_nt_diff"] = np.where(
-        pairAS["flag_no_shared_nt"] == 1,
+    pairAS["num_nt_noOvlp"] = np.where(
+        pairAS["flag_no_ovlp_nt"] == 1,
         np.nan,
-        pairAS["num_nt_diff"]
+        pairAS["num_nt_noOvlp"]
     )
     # Make AS flags boolean values and rename
     xcrptFlagCols = [
         "transcript_1",
         "transcript_2",
         "flag_alt_exon",
-        "flag_alt_donor_acceptor",
+        "flag_alt_DA",
         "flag_IR",
-        "flag_5_variation",
-        "flag_3_variation",
-        "flag_no_shared_nt",
+        "flag_5_var",
+        "flag_3_var",
+        "flag_no_ovlp_nt",
     ]
     pairAS[xcrptFlagCols] = pairAS[xcrptFlagCols].astype(bool)
     pairAS = pairAS.rename(
         columns={
             "flag_alt_exon": "Alt. Exon",
-            "flag_alt_donor_acceptor": "Alt. Donor/Acceptor",
+            "flag_alt_DA": "Alt. Donor/Acceptor",
             "flag_IR": "Intron Retention",
-            "flag_5_variation": "5' Variation",
-            "flag_3_variation": "3' Variation",
-            "flag_no_shared_nt": "No Shared NT",
-            "num_nt_diff": "# NT Different",
-            "prop_nt_diff": "Proportion\nNT Different",
+            "flag_5_var": "5' Variation",
+            "flag_3_var": "3' Variation",
+            "flag_no_ovlp_nt": "No Shared NT",
+            "num_nt_noOvlp": "# NT Different",
+            "prop_nt_noOvlp": "Proportion\nNT Different",
         }
     )
     AScols = [
         "5' Variation",
         "3' Variation",
         "Alt. Donor/Acceptor",
         "Alt. Exon",
@@ -915,80 +915,80 @@
                 color=sns.color_palette("colorblind", 15).as_hex()[boxCols.index(col)],
             )
     upset.plot()
     plt.subplots_adjust(right=1.00001)
     plt.suptitle(title)
 
 
-def plot_gene_avg_nt_diff_pairs(md_data, name1, name2, legendOut, zoomMean=False):
+def plot_gene_avg_nt_noOvlp_pairs(md_data, name1, name2, legendOut, zoomMean=False):
     """
     Plot average number of nt different in recip. min match pairs against
             avg number of nt different in min pairs that are extra
             (either in the greater sets of in set that do not match) with the
             option to zoom in to the  mean value of non-zero nucleotide differences
             (max of the two means from recip. min pairs and extras)
     """
     minPairNT = md_data[
         [
             "gene_id",
-            "transcript_in_gene",
-            "recip_min_pair_in_gene",
-            "flag_recip_min_match",
+            "transcript_inGene",
+            "recip_min_pair_inGene",
+            "flag_RMP",
             "flag_min_match_" + name1,
             "flag_min_match_" + name2,
-            "num_nt_diff",
-            "prop_nt_diff",
+            "num_nt_noOvlp",
+            "prop_nt_noOvlp",
         ]
     ].copy()
     # Ensure number of nt different are int and float values
-    minPairNT["num_nt_diff"] = minPairNT["num_nt_diff"].astype(int)
-    minPairNT["prop_nt_diff"] = minPairNT["prop_nt_diff"].astype(float)
-    minPairNT["num_nt_diff_recip_min"] = np.where(
-        minPairNT["flag_recip_min_match"] == 1, minPairNT["num_nt_diff"], 0
+    minPairNT["num_nt_noOvlp"] = minPairNT["num_nt_noOvlp"].astype(int)
+    minPairNT["prop_nt_noOvlp"] = minPairNT["prop_nt_noOvlp"].astype(float)
+    minPairNT["num_nt_noOvlp_recip_min"] = np.where(
+        minPairNT["flag_RMP"] == 1, minPairNT["num_nt_noOvlp"], 0
     )
-    minPairNT["num_nt_diff_extra"] = np.where(
-        (minPairNT["flag_recip_min_match"] == 0)
+    minPairNT["num_nt_noOvlp_extra"] = np.where(
+        (minPairNT["flag_RMP"] == 0)
         & (
             minPairNT["flag_min_match_" + name1] + minPairNT["flag_min_match_" + name2]
             == 1
         ),
-        minPairNT["num_nt_diff"],
+        minPairNT["num_nt_noOvlp"],
         0,
     )
     minPairNTGene = (
         minPairNT.groupby("gene_id")
         .agg(
             {
-                "transcript_in_gene": "first",
-                "recip_min_pair_in_gene": "first",
-                "num_nt_diff_recip_min": "mean",
-                "num_nt_diff_extra": "mean",
+                "transcript_inGene": "first",
+                "recip_min_pair_inGene": "first",
+                "num_nt_noOvlp_recip_min": "mean",
+                "num_nt_noOvlp_extra": "mean",
             }
         )
         .reset_index()
     )
     recipConditions = [
-        (minPairNTGene["transcript_in_gene"] == "match")
-        & (minPairNTGene["recip_min_pair_in_gene"] == "reciprocal_pairs"),
-        (minPairNTGene["transcript_in_gene"] == "match")
-        & (minPairNTGene["recip_min_pair_in_gene"] == "partial_reciprocal_pairs"),
-        (minPairNTGene["transcript_in_gene"] == "match")
-        & (minPairNTGene["recip_min_pair_in_gene"] == "no_reciprocal_pairs"),
-        (minPairNTGene["transcript_in_gene"] == name1 + "_greater")
-        & (minPairNTGene["recip_min_pair_in_gene"] == "reciprocal_pairs"),
-        (minPairNTGene["transcript_in_gene"] == name1 + "_greater")
-        & (minPairNTGene["recip_min_pair_in_gene"] == "partial_reciprocal_pairs"),
-        (minPairNTGene["transcript_in_gene"] == name1 + "_greater")
-        & (minPairNTGene["recip_min_pair_in_gene"] == "no_reciprocal_pairs"),
-        (minPairNTGene["transcript_in_gene"] == name2 + "_greater")
-        & (minPairNTGene["recip_min_pair_in_gene"] == "reciprocal_pairs"),
-        (minPairNTGene["transcript_in_gene"] == name2 + "_greater")
-        & (minPairNTGene["recip_min_pair_in_gene"] == "partial_reciprocal_pairs"),
-        (minPairNTGene["transcript_in_gene"] == name2 + "_greater")
-        & (minPairNTGene["recip_min_pair_in_gene"] == "no_reciprocal_pairs"),
+        (minPairNTGene["transcript_inGene"] == "match")
+        & (minPairNTGene["recip_min_pair_inGene"] == "reciprocal_pairs"),
+        (minPairNTGene["transcript_inGene"] == "match")
+        & (minPairNTGene["recip_min_pair_inGene"] == "partial_reciprocal_pairs"),
+        (minPairNTGene["transcript_inGene"] == "match")
+        & (minPairNTGene["recip_min_pair_inGene"] == "no_reciprocal_pairs"),
+        (minPairNTGene["transcript_inGene"] == name1 + "_greater")
+        & (minPairNTGene["recip_min_pair_inGene"] == "reciprocal_pairs"),
+        (minPairNTGene["transcript_inGene"] == name1 + "_greater")
+        & (minPairNTGene["recip_min_pair_inGene"] == "partial_reciprocal_pairs"),
+        (minPairNTGene["transcript_inGene"] == name1 + "_greater")
+        & (minPairNTGene["recip_min_pair_inGene"] == "no_reciprocal_pairs"),
+        (minPairNTGene["transcript_inGene"] == name2 + "_greater")
+        & (minPairNTGene["recip_min_pair_inGene"] == "reciprocal_pairs"),
+        (minPairNTGene["transcript_inGene"] == name2 + "_greater")
+        & (minPairNTGene["recip_min_pair_inGene"] == "partial_reciprocal_pairs"),
+        (minPairNTGene["transcript_inGene"] == name2 + "_greater")
+        & (minPairNTGene["recip_min_pair_inGene"] == "no_reciprocal_pairs"),
     ]
     recipChoices = [
         "Match:Reciprocal Pairs",
         "Match:Partial Reciprocal Pairs",
         "Match:No Reciprocal Pairs",
         name1 + " Greater:Reciprocal Pairs",
         name1 + " Greater:Partial Reciprocal Pairs",
@@ -1026,40 +1026,40 @@
         name2 + " Greater:Partial Reciprocal Pairs": "#fbafe4",
         name2 + " Greater:No Reciprocal Pairs": "#ca9161",
     }
     if not zoomMean:
         limit = (
             max(
                 minPairNTGene[
-                        ["num_nt_diff_recip_min", "num_nt_diff_extra"]
+                        ["num_nt_noOvlp_recip_min", "num_nt_noOvlp_extra"]
                         ].max().max(),
                 1
             )
         )
     else:
         try:
             limit = round(
                 np.nanmax(
                     [
-                        minPairNTGene[minPairNTGene["num_nt_diff_recip_min"] > 0][
-                            "num_nt_diff_recip_min"
+                        minPairNTGene[minPairNTGene["num_nt_noOvlp_recip_min"] > 0][
+                            "num_nt_noOvlp_recip_min"
                         ].mean(),
-                        minPairNTGene[minPairNTGene["num_nt_diff_extra"] > 0][
-                            "num_nt_diff_extra"
+                        minPairNTGene[minPairNTGene["num_nt_noOvlp_extra"] > 0][
+                            "num_nt_noOvlp_extra"
                         ].mean(),
                     ]
                 )
             )
         except ValueError:
             limit = 1
     plt.figure(figsize=(8.45, 5))
     sns.scatterplot(
         data=minPairNTGene,
-        x="num_nt_diff_recip_min",
-        y="num_nt_diff_extra",
+        x="num_nt_noOvlp_recip_min",
+        y="num_nt_noOvlp_extra",
         hue="Category",
         palette=colorPalleteRecip,
     )
     plt.xlim(0, limit)
     plt.ylim(0, limit)
     plt.xlabel("Avg. # NT Different in Recip. Min. Pairs")
     plt.ylabel("Avg. # NT Different in Min. Pairs of Extras")
```

### Comparing `trand-23.2.20/src/trand/plot_one_gtf_gene.py` & `trand-23.5.30/src/trand/plot_one_gtf_gene.py`

 * *Files identical despite different names*

### Comparing `trand-23.2.20/src/trand/plot_one_gtf_pairwise.py` & `trand-23.5.30/src/trand/plot_one_gtf_pairwise.py`

 * *Files identical despite different names*

### Comparing `trand-23.2.20/src/trand/plot_transcriptome.py` & `trand-23.5.30/src/trand/plot_transcriptome.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 import matplotlib
 import seaborn as sns
 import math
 
 
 def calculate_donor_ratio_newINF(unit, feature, count_col, data):
     df = data.groupby([unit, feature])[count_col].count().reset_index().rename(columns = {count_col : "num_col_id"})
-    df["flag_donor_acceptor"] = np.where(df["num_col_id"] > 1, 1, 0)
-    df2 = df.groupby(unit).agg({feature : "count", "flag_donor_acceptor" : 'sum'})
-    res = df2["flag_donor_acceptor"]/df2[feature]
+    df["flag_DA"] = np.where(df["num_col_id"] > 1, 1, 0)
+    df2 = df.groupby(unit).agg({feature : "count", "flag_DA" : 'sum'})
+    res = df2["flag_DA"]/df2[feature]
     return res
 
 def uniqueList(test_list):
     res = []
     for i in test_list:
         if i not in res:
             res.append(i)
```

### Comparing `trand-23.2.20/src/trand/plot_two_gtf_pairwise.py` & `trand-23.5.30/src/trand/plot_two_gtf_pairwise.py`

 * *Files identical despite different names*

### Comparing `trand-23.2.20/src/trand/transcript_distance.py` & `trand-23.5.30/src/trand/transcript_distance.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,71 +10,71 @@
 import numpy as np
 
 
 td_df_cols = [
     "gene_id",
     "transcript_1",
     "transcript_2",
-    "num_junction_T1_only",
-    "num_junction_T2_only",
-    "num_junction_shared",
-    "prop_junction_diff",
-    "prop_junction_similar",
-    "junction_T1_all",
-    "junction_T2_all",
-    "junction_T1_only",
-    "junction_T2_only",
-    "junction_shared",
-    "num_ER_T1_only",
-    "num_ER_T2_only",
-    "num_ER_shared",
-    "prop_ER_diff",
-    "prop_ER_similar",
-    "ER_T1_only",
-    "ER_T2_only",
-    "ER_shared",
-    "num_fragment_T1_only",
-    "num_fragment_T2_only",
-    "num_fragment_shared",
-    "prop_fragment_diff",
-    "prop_fragment_similar",
-    "fragment_T1_only",
-    "fragment_T2_only",
-    "fragment_shared",
-    "num_fragment_singletons_T1_only",
-    "num_fragment_singletons_T2_only",
-    "num_fragment_singletons_shared",
-    "num_IR_fragment_T1",
-    "num_IR_fragment_T2",
-    "IR_fragment_T1",
-    "IR_fragment_T2",
-    "num_nt_shared",
-    "num_nt_T1_only",
-    "num_nt_T2_only",
-    "num_nt_diff",
+    "num_jxn_only_T1",
+    "num_jxn_only_T2",
+    "num_jxn_ovlp",
+    "prop_jxn_noOvlp",
+    "prop_jxn_ovlp",
+    "jxn_string_T1",
+    "jxn_string_T2",
+    "jxn_only_T1",
+    "jxn_only_T2",
+    "jxn_same",
+    "num_ER_only_T1",
+    "num_ER_only_T2",
+    "num_ER_ovlp",
+    "prop_ER_noOvlp",
+    "prop_ER_ovlp",
+    "ER_only_T1",
+    "ER_only_T2",
+    "ER_ovlp",
+    "num_EF_only_T1",
+    "num_EF_only_T2",
+    "num_EF_ovlp",
+    "prop_EF_noOvlp",
+    "prop_EF_ovlp",
+    "EF_only_T1",
+    "EF_only_T2",
+    "EF_ovlp",
+    "num_exon_only_T1",
+    "num_exon_only_T2",
+    "num_exon_ovlp",
+    "num_IR_EF_T1",
+    "num_IR_EF_T2",
+    "IR_EF_T1",
+    "IR_EF_T2",
+    "num_nt_ovlp",
+    "num_nt_only_T1",
+    "num_nt_only_T2",
+    "num_nt_noOvlp",
     "total_nt",
-    "prop_nt_diff",
-    "prop_nt_similar",
-    "num_nt_T1_only_in_shared_ER",
-    "num_nt_T2_only_in_shared_ER",
-    "num_nt_shared_in_shared_ER",
-    "total_nt_in_shared_ER",
-    "prop_nt_diff_in_shared_ER",
-    "prop_nt_similar_in_shared_ER",
-    "num_nt_T1_only_in_unique_ER",
-    "num_nt_T2_only_in_unique_ER",
+    "prop_nt_noOvlp",
+    "prop_nt_ovlp",
+    "num_nt_only_T1_in_ovlpER",
+    "num_nt_only_T2_in_ovlpER",
+    "num_nt_ovlp_in_ovlpER",
+    "total_nt_in_ovlpER",
+    "prop_nt_noOvlp_in_ovlpER",
+    "prop_nt_ovlp_in_ovlpER",
+    "num_nt_only_T1_in_uniqER",
+    "num_nt_only_T2_in_uniqER",
     "flag_FSM",
     "flag_T1_ISM_of_T2",
     "flag_T2_ISM_of_T1",
     "flag_IR",
-    "flag_5_variation",
-    "flag_3_variation",
-    "flag_alt_donor_acceptor",
+    "flag_5_var",
+    "flag_3_var",
+    "flag_alt_DA",
     "flag_alt_exon",
-    "flag_no_shared_nt",
+    "flag_no_ovlp_nt",
 ]
 
 
 def calculate_distance(out_df, junction_df, gene_id, tx1_name, tx2_name, fsm=False):
     # Check for monoexons
     has_junctions = True
     if junction_df.empty:
@@ -86,16 +86,16 @@
     singlePair = pd.Series(index=td_df_cols, dtype=object)
     singlePair[["gene_id", "transcript_1", "transcript_2"]] = (
         gene_id,
         tx1_name,
         tx2_name,
     )
 
-    # Set exon fragment and exon region ID values based on genomic coordinates
-    ef_df["fragment_id"] = (
+    # Set exon EF and exon region ID values based on genomic coordinates
+    ef_df["EF_id"] = (
         ef_df["ef_chr"].map(str)
         + ":"
         + ef_df["ef_start"].map(str)
         + ":"
         + ef_df["ef_end"].map(str)
         + ":"
         + ef_df["ef_strand"].map(str)
@@ -106,28 +106,28 @@
         + ef_df["er_start"].map(str)
         + ":"
         + ef_df["er_end"].map(str)
         + ":"
         + ef_df["er_strand"].map(str)
     )
 
-    # Flag shared fragments
-    ef_df["flag_shared"] = np.where(
+    # Flag shared EFs
+    ef_df["flag_ovlp"] = np.where(
         (ef_df["transcript_id"] == tx1_name + "|" + tx2_name)
         | (ef_df["transcript_id"] == tx2_name + "|" + tx1_name),
         1,
         0,
     )
 
-    # Flag singleton fragments (where the fragment is a full exon region)
-    ef_df["num_fragment_in_ER"] = ef_df.groupby("er_id")["ef_id"].transform("count")
-    ef_df["flag_singleton"] = np.where(ef_df["num_fragment_in_ER"] == 1, 1, 0)
+    # Flag singleton EFs (where the EF is a full exon region)
+    ef_df["num_EF_in_ER"] = ef_df.groupby("er_id")["ef_id"].transform("count")
+    ef_df["flag_singleton"] = np.where(ef_df["num_EF_in_ER"] == 1, 1, 0)
 
-    # Add fragment lengths (end - start)
-    ef_df["fragment_length"] = ef_df["ef_end"].map(int) - ef_df["ef_start"].map(int)
+    # Add EF lengths (end - start)
+    ef_df["EF_length"] = ef_df["ef_end"].map(int) - ef_df["ef_start"].map(int)
 
     # Sort junctions by chromosome and coordinates
     if has_junctions:
         sorted_junction_df = junction_df.copy()
         sorted_junction_df[["chr", "start", "end", "strand"]] = (
                 sorted_junction_df["coords"].str.split(":", expand=True)
         )
@@ -141,15 +141,15 @@
         sorted_junction_df = pd.DataFrame()
 
     # Get distance measures for junctions
     singlePair = get_junction_distance(
         singlePair, sorted_junction_df, tx1_name, tx2_name, fsm=fsm
     )
 
-    # Gt distance measures for exon regions (ER) and exon fragments (EF)
+    # Gt distance measures for exon regions (ER) and exon EFs (EF)
     singlePair, ERSharedSet = get_ER_distance(
         singlePair, ef_df, tx1_name, tx2_name, fsm=fsm
     )
     singlePair = get_EF_distance(singlePair, ef_df, tx1_name, tx2_name, ERSharedSet)
 
     # Set flags for different alternative splicing (AS) events
     singlePair = set_AS_flags(singlePair, ef_df, tx1_name, tx2_name, has_junctions)
@@ -160,397 +160,397 @@
 
 def get_junction_distance(singlePair, sorted_junction_df, tx1_name, tx2_name, fsm=False):
     # Check if transcript pair shares all junctions (FSM, full-splice match)
     if fsm:
         # Check if both transcripts are monoexon (no junctions)
         if len(sorted_junction_df) == 0:
             singlePair[
-                ["num_junction_T1_only", "num_junction_T2_only", "num_junction_shared"]
+                ["num_jxn_only_T1", "num_jxn_only_T2", "num_jxn_ovlp"]
             ] = 0
-            singlePair["prop_junction_diff"] = 0
-            singlePair["prop_junction_similar"] = 1
+            singlePair["prop_jxn_noOvlp"] = 0
+            singlePair["prop_jxn_ovlp"] = 1
             singlePair[
-                ["junction_T1_only",
-                 "junction_T2_only",
-                 "junction_shared",
-                 "junction_T1_all",
-                 "junction_T2_all"]
+                ["jxn_only_T1",
+                 "jxn_only_T2",
+                 "jxn_same",
+                 "jxn_string_T1",
+                 "jxn_string_T2"]
             ] = ""
         # FSM transcripts are multiexon
         else:
-            singlePair[["num_junction_T1_only", "num_junction_T2_only"]] = 0
-            singlePair["num_junction_shared"] = len(
+            singlePair[["num_jxn_only_T1", "num_jxn_only_T2"]] = 0
+            singlePair["num_jxn_ovlp"] = len(
                 sorted_junction_df[sorted_junction_df["transcript_id"] == tx1_name]
             )
-            singlePair["prop_junction_diff"] = 0
-            singlePair["prop_junction_similar"] = 1
-            singlePair[["junction_T1_only", "junction_T2_only"]] = ""
+            singlePair["prop_jxn_noOvlp"] = 0
+            singlePair["prop_jxn_ovlp"] = 1
+            singlePair[["jxn_only_T1", "jxn_only_T2"]] = ""
             singlePair[
-                    ["junction_shared", "junction_T1_all", "junction_T2_all"]
+                    ["jxn_same", "jxn_string_T1", "jxn_string_T2"]
                 ] = "|".join(
                     sorted_junction_df[
                             sorted_junction_df["transcript_id"] == tx1_name
                         ]["coords"]
             )
 
     # Transcript pair does not share all junctions
     else:
         # Check if both transcripts are monoexon but do not overlap (not fsm)
         if len(sorted_junction_df) == 0:
             singlePair[
-                ["num_junction_T1_only", "num_junction_T2_only", "num_junction_shared"]
+                ["num_jxn_only_T1", "num_jxn_only_T2", "num_jxn_ovlp"]
             ] = 0
-            singlePair["prop_junction_diff"] = 0
-            singlePair["prop_junction_similar"] = 1
+            singlePair["prop_jxn_noOvlp"] = 0
+            singlePair["prop_jxn_ovlp"] = 1
             singlePair[
-                ["junction_T1_only",
-                 "junction_T2_only",
-                 "junction_shared",
-                 "junction_T1_all",
-                 "junction_T2_all"]
+                ["jxn_only_T1",
+                 "jxn_only_T2",
+                 "jxn_same",
+                 "jxn_string_T1",
+                 "jxn_string_T2"]
             ] = ""
         # Check if one of the transcripts is monoexon (only junctions from one transcript and not
         # the other)
         elif sorted_junction_df["transcript_id"].nunique() == 1:
             # Only T1 is monoexon
             if tx2_name in sorted_junction_df["transcript_id"].unique():
-                singlePair[["num_junction_T1_only", "num_junction_shared"]] = 0
-                singlePair["prop_junction_similar"] = 0
-                singlePair["prop_junction_diff"] = 1
+                singlePair[["num_jxn_only_T1", "num_jxn_ovlp"]] = 0
+                singlePair["prop_jxn_ovlp"] = 0
+                singlePair["prop_jxn_noOvlp"] = 1
                 singlePair[
-                    ["junction_T1_only", "junction_T1_all", "junction_shared"]
+                    ["jxn_only_T1", "jxn_string_T1", "jxn_same"]
                 ] = ""
-                singlePair["num_junction_T2_only"] = len(sorted_junction_df)
+                singlePair["num_jxn_only_T2"] = len(sorted_junction_df)
                 singlePair[
-                    ["junction_T2_only", "junction_T2_all"]
+                    ["jxn_only_T2", "jxn_string_T2"]
                 ] = "|".join(sorted_junction_df["coords"])
             # Only T2 is monoexon
             else:
-                singlePair[["num_junction_T2_only", "num_junction_shared"]] = 0
-                singlePair["prop_junction_similar"] = 0
-                singlePair["prop_junction_diff"] = 1
+                singlePair[["num_jxn_only_T2", "num_jxn_ovlp"]] = 0
+                singlePair["prop_jxn_ovlp"] = 0
+                singlePair["prop_jxn_noOvlp"] = 1
                 singlePair[
-                    ["junction_T2_only", "junction_T2_all", "junction_shared"]
+                    ["jxn_only_T2", "jxn_string_T2", "jxn_same"]
                 ] = ""
-                singlePair["num_junction_T1_only"] = len(sorted_junction_df)
+                singlePair["num_jxn_only_T1"] = len(sorted_junction_df)
                 singlePair[
-                    ["junction_T1_only", "junction_T1_all"]
+                    ["jxn_only_T1", "jxn_string_T1"]
                 ] = "|".join(sorted_junction_df["coords"])
         # Both transcripts multi-exon
         else:
             t1Junc = sorted_junction_df[
                     sorted_junction_df["transcript_id"] == tx1_name
                 ]["coords"]
             t2Junc = sorted_junction_df[
                     sorted_junction_df["transcript_id"] == tx2_name
                 ]["coords"]
-            singlePair["junction_T1_all"] = "|".join(t1Junc)
-            singlePair["junction_T2_all"] = "|".join(t2Junc)
+            singlePair["jxn_string_T1"] = "|".join(t1Junc)
+            singlePair["jxn_string_T2"] = "|".join(t2Junc)
             juncSharedSet = set(t1Junc).intersection(set(t2Junc))
             juncT1Set = set(t1Junc).difference(set(t2Junc))
             juncT2Set = set(t2Junc).difference(set(t1Junc))
-            singlePair["num_junction_T1_only"] = len(juncT1Set)
-            singlePair["num_junction_T2_only"] = len(juncT2Set)
-            singlePair["num_junction_shared"] = len(juncSharedSet)
-            singlePair["prop_junction_diff"] = (
-                singlePair["num_junction_T1_only"] + singlePair["num_junction_T2_only"]
+            singlePair["num_jxn_only_T1"] = len(juncT1Set)
+            singlePair["num_jxn_only_T2"] = len(juncT2Set)
+            singlePair["num_jxn_ovlp"] = len(juncSharedSet)
+            singlePair["prop_jxn_noOvlp"] = (
+                singlePair["num_jxn_only_T1"] + singlePair["num_jxn_only_T2"]
             ) / (
-                singlePair["num_junction_T1_only"]
-                + singlePair["num_junction_T2_only"]
-                + singlePair["num_junction_shared"]
+                singlePair["num_jxn_only_T1"]
+                + singlePair["num_jxn_only_T2"]
+                + singlePair["num_jxn_ovlp"]
             )
-            singlePair["prop_junction_similar"] = 1 - singlePair["prop_junction_diff"]
-            singlePair["junction_T1_only"] = "|".join(
+            singlePair["prop_jxn_ovlp"] = 1 - singlePair["prop_jxn_noOvlp"]
+            singlePair["jxn_only_T1"] = "|".join(
                 sorted(juncT1Set, key=lambda x: t1Junc[t1Junc == x].index[0])
             )
-            singlePair["junction_T2_only"] = "|".join(
+            singlePair["jxn_only_T2"] = "|".join(
                 sorted(juncT2Set, key=lambda x: t2Junc[t2Junc == x].index[0])
             )
-            singlePair["junction_shared"] = "|".join(
+            singlePair["jxn_same"] = "|".join(
                 sorted(juncSharedSet, key=lambda x: t2Junc[t2Junc == x].index[0])
             )
     return singlePair
 
 
 def get_ER_distance(singlePair, ef_df, tx1_name, tx2_name, fsm=False):
     # Check if transcript pair shares all junctions (FSM, full-splice match)
     if fsm:
         # All junctions are shared, therefore all ER are shared
-        singlePair[["num_ER_T1_only", "num_ER_T2_only"]] = 0
-        singlePair["num_ER_shared"] = ef_df["er_id"].nunique()
-        singlePair["prop_ER_diff"] = 0
-        singlePair["prop_ER_similar"] = 1
-        singlePair[["ER_T1_only", "ER_T2_only"]] = ""
-        singlePair["ER_shared"] = "|".join(ef_df["region_id"].unique())
+        singlePair[["num_ER_only_T1", "num_ER_only_T2"]] = 0
+        singlePair["num_ER_ovlp"] = ef_df["er_id"].nunique()
+        singlePair["prop_ER_noOvlp"] = 0
+        singlePair["prop_ER_ovlp"] = 1
+        singlePair[["ER_only_T1", "ER_only_T2"]] = ""
+        singlePair["ER_ovlp"] = "|".join(ef_df["region_id"].unique())
         ERSharedSet = ef_df["region_id"].drop_duplicates()
     else:
         # Check for shared and unique ER
         ERall = (
             ef_df.groupby("region_id")
-            .agg({"transcript_id": (lambda x: max(x, key=len)), "flag_shared": "max"})
+            .agg({"transcript_id": (lambda x: max(x, key=len)), "flag_ovlp": "max"})
             .reset_index()
         )
-        ERSharedSet = ERall[ERall["flag_shared"] == 1]["region_id"]
+        ERSharedSet = ERall[ERall["flag_ovlp"] == 1]["region_id"]
         ERT1Set = ERall[
-            (ERall["flag_shared"] == 0) & (ERall["transcript_id"] == tx1_name)
+            (ERall["flag_ovlp"] == 0) & (ERall["transcript_id"] == tx1_name)
         ]["region_id"]
         ERT2Set = ERall[
-            (ERall["flag_shared"] == 0) & (ERall["transcript_id"] == tx2_name)
+            (ERall["flag_ovlp"] == 0) & (ERall["transcript_id"] == tx2_name)
         ]["region_id"]
-        singlePair["num_ER_T1_only"] = len(ERT1Set)
-        singlePair["num_ER_T2_only"] = len(ERT2Set)
-        singlePair["num_ER_shared"] = len(ERSharedSet)
-        singlePair["prop_ER_diff"] = (
-            singlePair["num_ER_T1_only"] + singlePair["num_ER_T2_only"]
+        singlePair["num_ER_only_T1"] = len(ERT1Set)
+        singlePair["num_ER_only_T2"] = len(ERT2Set)
+        singlePair["num_ER_ovlp"] = len(ERSharedSet)
+        singlePair["prop_ER_noOvlp"] = (
+            singlePair["num_ER_only_T1"] + singlePair["num_ER_only_T2"]
         ) / (
-            singlePair["num_ER_T1_only"]
-            + singlePair["num_ER_T2_only"]
-            + singlePair["num_ER_shared"]
-        )
-        singlePair["prop_ER_similar"] = 1 - singlePair["prop_ER_diff"]
-        singlePair["ER_T1_only"] = "|".join(ERT1Set)
-        singlePair["ER_T2_only"] = "|".join(ERT2Set)
-        singlePair["ER_shared"] = "|".join(ERSharedSet)
+            singlePair["num_ER_only_T1"]
+            + singlePair["num_ER_only_T2"]
+            + singlePair["num_ER_ovlp"]
+        )
+        singlePair["prop_ER_ovlp"] = 1 - singlePair["prop_ER_noOvlp"]
+        singlePair["ER_only_T1"] = "|".join(ERT1Set)
+        singlePair["ER_only_T2"] = "|".join(ERT2Set)
+        singlePair["ER_ovlp"] = "|".join(ERSharedSet)
     return singlePair, ERSharedSet
 
 
 def get_EF_distance(singlePair, ef_df, tx1_name, tx2_name, ERSharedSet):
-    num_shared = ef_df["flag_shared"].sum()
-    # Check if all fragments are shared (transcripts are identical)
-    if num_shared == len(ef_df):
+    num_ovlp = ef_df["flag_ovlp"].sum()
+    # Check if all EFs are shared (transcripts are identical)
+    if num_ovlp == len(ef_df):
         # All EF shared, transcripts are identical
-        singlePair[["num_fragment_T1_only", "num_fragment_T2_only"]] = 0
-        singlePair["num_fragment_shared"] = len(ef_df)
-        singlePair["prop_fragment_diff"] = 0
-        singlePair["prop_fragment_similar"] = 1
-        singlePair[["fragment_T1_only", "fragment_T2_only"]] = ""
-        singlePair["fragment_shared"] = "|".join(ef_df["fragment_id"])
+        singlePair[["num_EF_only_T1", "num_EF_only_T2"]] = 0
+        singlePair["num_EF_ovlp"] = len(ef_df)
+        singlePair["prop_EF_noOvlp"] = 0
+        singlePair["prop_EF_ovlp"] = 1
+        singlePair[["EF_only_T1", "EF_only_T2"]] = ""
+        singlePair["EF_ovlp"] = "|".join(ef_df["EF_id"])
         singlePair[
-            ["num_fragment_singletons_T1_only", "num_fragment_singletons_T2_only"]
+            ["num_exon_only_T1", "num_exon_only_T2"]
         ] = 0
-        singlePair["num_fragment_singletons_shared"] = singlePair["num_fragment_shared"]
+        singlePair["num_exon_ovlp"] = singlePair["num_EF_ovlp"]
 
         # Nucleotide differences are 0, all are shared and are in shared ER
         singlePair[
             [
                 "total_nt",
-                "total_nt_in_shared_ER",
-                "num_nt_shared",
-                "num_nt_shared_in_shared_ER",
+                "total_nt_in_ovlpER",
+                "num_nt_ovlp",
+                "num_nt_ovlp_in_ovlpER",
             ]
-        ] = ef_df["fragment_length"].sum()
+        ] = ef_df["EF_length"].sum()
         singlePair[
             [
-                "num_nt_T1_only",
-                "num_nt_T1_only_in_shared_ER",
-                "num_nt_T1_only_in_unique_ER",
-                "num_nt_T2_only",
-                "num_nt_T2_only_in_shared_ER",
-                "num_nt_T2_only_in_unique_ER",
-                "num_nt_diff",
+                "num_nt_only_T1",
+                "num_nt_only_T1_in_ovlpER",
+                "num_nt_only_T1_in_uniqER",
+                "num_nt_only_T2",
+                "num_nt_only_T2_in_ovlpER",
+                "num_nt_only_T2_in_uniqER",
+                "num_nt_noOvlp",
             ]
         ] = 0
-        singlePair[["prop_nt_diff", "prop_nt_diff_in_shared_ER"]] = 0
-        singlePair[["prop_nt_similar", "prop_nt_similar_in_shared_ER"]] = 1
+        singlePair[["prop_nt_noOvlp", "prop_nt_noOvlp_in_ovlpER"]] = 0
+        singlePair[["prop_nt_ovlp", "prop_nt_ovlp_in_ovlpER"]] = 1
 
         # No IR present between identical transcripts
-        singlePair[["num_IR_fragment_T1", "num_IR_fragment_T2"]] = 0
-        singlePair[["IR_fragment_T1", "IR_fragment_T2"]] = ""
+        singlePair[["num_IR_EF_T1", "num_IR_EF_T2"]] = 0
+        singlePair[["IR_EF_T1", "IR_EF_T2"]] = ""
     else:
         # Not all EF shared
-        fragSharedSet = ef_df[ef_df["flag_shared"] == 1]
+        fragSharedSet = ef_df[ef_df["flag_ovlp"] == 1]
         fragSharedSingSet = ef_df[
-            (ef_df["flag_shared"] == 1) & (ef_df["flag_singleton"] == 1)
+            (ef_df["flag_ovlp"] == 1) & (ef_df["flag_singleton"] == 1)
         ]
         fragT1Set = ef_df[
-            (ef_df["flag_shared"] == 0) & (ef_df["transcript_id"] == tx1_name)
+            (ef_df["flag_ovlp"] == 0) & (ef_df["transcript_id"] == tx1_name)
         ]
         fragT1SingSet = ef_df[
-            (ef_df["flag_shared"] == 0)
+            (ef_df["flag_ovlp"] == 0)
             & (ef_df["transcript_id"] == tx1_name)
             & (ef_df["flag_singleton"] == 1)
         ]
         fragT2Set = ef_df[
-            (ef_df["flag_shared"] == 0) & (ef_df["transcript_id"] == tx2_name)
+            (ef_df["flag_ovlp"] == 0) & (ef_df["transcript_id"] == tx2_name)
         ]
         fragT2SingSet = ef_df[
-            (ef_df["flag_shared"] == 0)
+            (ef_df["flag_ovlp"] == 0)
             & (ef_df["transcript_id"] == tx2_name)
             & (ef_df["flag_singleton"] == 1)
         ]
-        singlePair["num_fragment_T1_only"] = len(fragT1Set)
-        singlePair["num_fragment_T2_only"] = len(fragT2Set)
-        singlePair["num_fragment_shared"] = len(fragSharedSet)
-        singlePair["prop_fragment_diff"] = (
-            singlePair["num_fragment_T1_only"] + singlePair["num_fragment_T2_only"]
+        singlePair["num_EF_only_T1"] = len(fragT1Set)
+        singlePair["num_EF_only_T2"] = len(fragT2Set)
+        singlePair["num_EF_ovlp"] = len(fragSharedSet)
+        singlePair["prop_EF_noOvlp"] = (
+            singlePair["num_EF_only_T1"] + singlePair["num_EF_only_T2"]
         ) / (
-            singlePair["num_fragment_T1_only"]
-            + singlePair["num_fragment_T2_only"]
-            + singlePair["num_fragment_shared"]
-        )
-        singlePair["prop_fragment_similar"] = 1 - singlePair["prop_fragment_diff"]
-        singlePair["fragment_T1_only"] = "|".join(fragT1Set["fragment_id"])
-        singlePair["fragment_T2_only"] = "|".join(fragT2Set["fragment_id"])
-        singlePair["fragment_shared"] = "|".join(fragSharedSet["fragment_id"])
-        singlePair["num_fragment_singletons_T1_only"] = len(fragT1SingSet)
-        singlePair["num_fragment_singletons_T2_only"] = len(fragT2SingSet)
-        singlePair["num_fragment_singletons_shared"] = len(fragSharedSingSet)
+            singlePair["num_EF_only_T1"]
+            + singlePair["num_EF_only_T2"]
+            + singlePair["num_EF_ovlp"]
+        )
+        singlePair["prop_EF_ovlp"] = 1 - singlePair["prop_EF_noOvlp"]
+        singlePair["EF_only_T1"] = "|".join(fragT1Set["EF_id"])
+        singlePair["EF_only_T2"] = "|".join(fragT2Set["EF_id"])
+        singlePair["EF_ovlp"] = "|".join(fragSharedSet["EF_id"])
+        singlePair["num_exon_only_T1"] = len(fragT1SingSet)
+        singlePair["num_exon_only_T2"] = len(fragT2SingSet)
+        singlePair["num_exon_ovlp"] = len(fragSharedSingSet)
 
         # Count number of nt shared/different in all EF
-        singlePair["num_nt_shared"] = fragSharedSet["fragment_length"].sum()
-        singlePair["num_nt_T1_only"] = fragT1Set["fragment_length"].sum()
-        singlePair["num_nt_T2_only"] = fragT2Set["fragment_length"].sum()
-        singlePair["num_nt_diff"] = (
-            singlePair["num_nt_T1_only"] + singlePair["num_nt_T2_only"]
+        singlePair["num_nt_ovlp"] = fragSharedSet["EF_length"].sum()
+        singlePair["num_nt_only_T1"] = fragT1Set["EF_length"].sum()
+        singlePair["num_nt_only_T2"] = fragT2Set["EF_length"].sum()
+        singlePair["num_nt_noOvlp"] = (
+            singlePair["num_nt_only_T1"] + singlePair["num_nt_only_T2"]
         )
         singlePair["total_nt"] = (
-            singlePair["num_nt_shared"]
-            + singlePair["num_nt_T1_only"]
-            + singlePair["num_nt_T2_only"]
+            singlePair["num_nt_ovlp"]
+            + singlePair["num_nt_only_T1"]
+            + singlePair["num_nt_only_T2"]
         )
-        singlePair["prop_nt_diff"] = (
-            singlePair["num_nt_T1_only"] + singlePair["num_nt_T2_only"]
+        singlePair["prop_nt_noOvlp"] = (
+            singlePair["num_nt_only_T1"] + singlePair["num_nt_only_T2"]
         ) / (singlePair["total_nt"])
-        singlePair["prop_nt_similar"] = 1 - singlePair["prop_nt_diff"]
+        singlePair["prop_nt_ovlp"] = 1 - singlePair["prop_nt_noOvlp"]
 
         # Count number of nt shared/different in EF only in shared ER
-        singlePair["num_nt_T1_only_in_shared_ER"] = fragT1Set[
+        singlePair["num_nt_only_T1_in_ovlpER"] = fragT1Set[
             fragT1Set["region_id"].isin(ERSharedSet)
-        ]["fragment_length"].sum()
-        singlePair["num_nt_T2_only_in_shared_ER"] = fragT2Set[
+        ]["EF_length"].sum()
+        singlePair["num_nt_only_T2_in_ovlpER"] = fragT2Set[
             fragT2Set["region_id"].isin(ERSharedSet)
-        ]["fragment_length"].sum()
-        singlePair["num_nt_shared_in_shared_ER"] = fragSharedSet[
+        ]["EF_length"].sum()
+        singlePair["num_nt_ovlp_in_ovlpER"] = fragSharedSet[
             fragSharedSet["region_id"].isin(ERSharedSet)
-        ]["fragment_length"].sum()
-        singlePair["total_nt_in_shared_ER"] = (
-            singlePair["num_nt_shared_in_shared_ER"]
-            + singlePair["num_nt_T1_only_in_shared_ER"]
-            + singlePair["num_nt_T2_only_in_shared_ER"]
-        )
-        if singlePair["total_nt_in_shared_ER"] != 0:
-            singlePair["prop_nt_diff_in_shared_ER"] = (
-                singlePair["num_nt_T1_only_in_shared_ER"]
-                + singlePair["num_nt_T2_only_in_shared_ER"]
-            ) / (singlePair["total_nt_in_shared_ER"])
-            singlePair["prop_nt_similar_in_shared_ER"] = (
-                1 - singlePair["prop_nt_diff_in_shared_ER"]
+        ]["EF_length"].sum()
+        singlePair["total_nt_in_ovlpER"] = (
+            singlePair["num_nt_ovlp_in_ovlpER"]
+            + singlePair["num_nt_only_T1_in_ovlpER"]
+            + singlePair["num_nt_only_T2_in_ovlpER"]
+        )
+        if singlePair["total_nt_in_ovlpER"] != 0:
+            singlePair["prop_nt_noOvlp_in_ovlpER"] = (
+                singlePair["num_nt_only_T1_in_ovlpER"]
+                + singlePair["num_nt_only_T2_in_ovlpER"]
+            ) / (singlePair["total_nt_in_ovlpER"])
+            singlePair["prop_nt_ovlp_in_ovlpER"] = (
+                1 - singlePair["prop_nt_noOvlp_in_ovlpER"]
             )
         else:
-            singlePair["prop_nt_diff_in_shared_ER"] = 0
-            singlePair["prop_nt_similar_in_shared_ER"] = 0
-        singlePair["num_nt_T1_only_in_unique_ER"] = fragT1Set[
+            singlePair["prop_nt_noOvlp_in_ovlpER"] = 0
+            singlePair["prop_nt_ovlp_in_ovlpER"] = 0
+        singlePair["num_nt_only_T1_in_uniqER"] = fragT1Set[
             ~fragT1Set["region_id"].isin(ERSharedSet)
-        ]["fragment_length"].sum()
-        singlePair["num_nt_T2_only_in_unique_ER"] = fragT2Set[
+        ]["EF_length"].sum()
+        singlePair["num_nt_only_T2_in_uniqER"] = fragT2Set[
             ~fragT2Set["region_id"].isin(ERSharedSet)
-        ]["fragment_length"].sum()
+        ]["EF_length"].sum()
 
         # Get IR distance values
-        singlePair["num_IR_fragment_T1"] = len(
+        singlePair["num_IR_EF_T1"] = len(
             fragT1Set[fragT1Set["ef_ir_flag"].map(int) == 1]
         )
-        singlePair["num_IR_fragment_T2"] = len(
+        singlePair["num_IR_EF_T2"] = len(
             fragT2Set[fragT2Set["ef_ir_flag"].map(int) == 1]
         )
-        singlePair["IR_fragment_T1"] = "|".join(
-            fragT1Set[fragT1Set["ef_ir_flag"].map(int) == 1]["fragment_id"]
+        singlePair["IR_EF_T1"] = "|".join(
+            fragT1Set[fragT1Set["ef_ir_flag"].map(int) == 1]["EF_id"]
         )
-        singlePair["IR_fragment_T2"] = "|".join(
-            fragT2Set[fragT2Set["ef_ir_flag"].map(int) == 1]["fragment_id"]
+        singlePair["IR_EF_T2"] = "|".join(
+            fragT2Set[fragT2Set["ef_ir_flag"].map(int) == 1]["EF_id"]
         )
     return singlePair
 
 
 def set_AS_flags(singlePair, ef_df, tx1_name, tx2_name, has_junctions):
     # Flag alternative splicing events
 
     # Flag transcripts with no shared nucleotides (nonoverlapping)
-    singlePair["flag_no_shared_nt"] = np.where(singlePair["prop_nt_diff"] == 1, 1, 0)
+    singlePair["flag_no_ovlp_nt"] = np.where(singlePair["prop_nt_noOvlp"] == 1, 1, 0)
 
     # Flag full-splice matches (FSM, share all junctions)
     # NOTE: monoexon transcripts can be FSM
-    singlePair["flag_FSM"] = np.where(singlePair["prop_junction_diff"] == 0, 1, 0)
+    singlePair["flag_FSM"] = np.where(singlePair["prop_jxn_noOvlp"] == 0, 1, 0)
 
     # Flag incomplete-splice matches
     # (ISM, one set of junctions is a complete consecutive subset of the other)
     # NOTE: ISM flags are 0 if transcripts are FSM or if at least one is monoexon
     if has_junctions:
         if (
             singlePair["flag_FSM"] == 1
-            or singlePair["junction_T1_all"] == ""
-            or singlePair["junction_T2_all"] == ""
+            or singlePair["jxn_string_T1"] == ""
+            or singlePair["jxn_string_T2"] == ""
         ):
             singlePair[
                 ["flag_T1_ISM_of_T2", "flag_T2_ISM_of_T1"]
             ] = 0
         else:
             singlePair["flag_T1_ISM_of_T2"] = np.where(
-                singlePair["junction_T1_all"] in singlePair["junction_T2_all"],
+                singlePair["jxn_string_T1"] in singlePair["jxn_string_T2"],
                 1,
                 0
             )
             singlePair["flag_T2_ISM_of_T1"] = np.where(
-                singlePair["junction_T2_all"] in singlePair["junction_T1_all"],
+                singlePair["jxn_string_T2"] in singlePair["jxn_string_T1"],
                 1,
                 0
             )
 
     # If a pair contains at least one IR event - 5' and 3' variation calculated
-    #   but flag_alt_exon and flag_alt_donor_acceptor set to 0
+    #   but flag_alt_exon and flag_alt_DA set to 0
     # Intron retention
     singlePair["flag_IR"] = np.where(
-        singlePair["num_IR_fragment_T1"] + singlePair["num_IR_fragment_T2"] > 0, 1, 0
+        singlePair["num_IR_EF_T1"] + singlePair["num_IR_EF_T2"] > 0, 1, 0
     )
 
     # 5' and 3' end variation
     t1_min_start = ef_df[ef_df["transcript_id"].str.contains(tx1_name)][
         "ef_start"
     ].min()
     t2_min_start = ef_df[ef_df["transcript_id"].str.contains(tx2_name)][
         "ef_start"
     ].min()
     t1_max_end = ef_df[ef_df["transcript_id"].str.contains(tx1_name)]["ef_end"].max()
     t2_max_end = ef_df[ef_df["transcript_id"].str.contains(tx2_name)]["ef_end"].max()
     ef_strand = ef_df["ef_strand"].unique()[0]
     # 5' variation: where difference in start if + strand or difference in end if - strand
-    singlePair["flag_5_variation"] = np.where(
+    singlePair["flag_5_var"] = np.where(
         ((ef_strand == "+") & (t1_min_start != t2_min_start))
         | ((ef_strand == "-") & (t1_max_end != t2_max_end)),
         1,
         0,
     )
     # 3' end variation: where difference in end if + strand or difference in start if - strand
-    singlePair["flag_3_variation"] = np.where(
+    singlePair["flag_3_var"] = np.where(
         ((ef_strand == "-") & (t1_min_start != t2_min_start))
         | ((ef_strand == "+") & (t1_max_end != t2_max_end)),
         1,
         0,
     )
 
     # If a pair contains at least one IR event - 5' and 3' variation calculated
-    #   but flag_alt_exon and flag_alt_donor_acceptor set to 0
+    #   but flag_alt_exon and flag_alt_DA set to 0
     if singlePair["flag_IR"] == 1:
         singlePair["flag_alt_exon"] = 0
-        singlePair["flag_alt_donor_acceptor"] = 0
+        singlePair["flag_alt_DA"] = 0
     else:
         # Alternate exons are when not all exon regions are shared
-        singlePair["flag_alt_exon"] = np.where(singlePair["prop_ER_diff"] > 0, 1, 0)
+        singlePair["flag_alt_exon"] = np.where(singlePair["prop_ER_noOvlp"] > 0, 1, 0)
 
         # Alternate donor/acceptors in shared ER (where not all junctions are shared)
-        singlePair["flag_alt_donor_acceptor"] = np.where(
-            (singlePair["prop_nt_diff_in_shared_ER"] > 0)
+        singlePair["flag_alt_DA"] = np.where(
+            (singlePair["prop_nt_noOvlp_in_ovlpER"] > 0)
             & (singlePair["flag_FSM"] == 0),
             1,
             0,
         )
 
     # If transcripts are nonoverlapping then 5'/3' variation and alt exon flags set to 0
-    if singlePair["flag_no_shared_nt"] == 1:
+    if singlePair["flag_no_ovlp_nt"] == 1:
         singlePair["flag_alt_exon"] = 0
-        singlePair["flag_5_variation"] = 0
-        singlePair["flag_3_variation"] = 0
+        singlePair["flag_5_var"] = 0
+        singlePair["flag_3_var"] = 0
         singlePair["flag_FSM"] = 0
         singlePair["flag_T1_ISM_of_T2"] = 0
         singlePair["flag_T2_ISM_of_T1"] = 0
 
     return singlePair
```

### Comparing `trand-23.2.20/src/trand.egg-info/PKG-INFO` & `trand-23.5.30/src/trand.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,64 @@
 Metadata-Version: 2.1
 Name: trand
-Version: 23.2.20
+Version: 23.5.30
 Summary: 'Transcript Distances'
 Home-page: https://github.com/McIntyre-Lab/TranD
 Author: McIntyre Lab, Universify of Florida
 Author-email: om@rc.ufl.edu
 License: MIT
+Description: # TranD: Transcript Distances
+        
+        TranD is a collection of tools to facilitate metrics of structural variation for whole genome
+        transcript annotation files (GTF) that pinpoint structural variation to the nucleotide level.
+        
+        TranD (Transcript Distances) can be used to calculate metrics of structural variation within and
+        between annotation files (GTF). Structural variation reflects organismal complexity and three
+        summary metrics for genome level complexity are calculated for every gene in a GTF file:  1) the
+        number of transcripts per gene; 2) the number of exons per transcript; and 3) the number of
+        unique exons (exons with unique genomic coordinates) per gene. From each these metrics
+        distributions a summary statistics such as mean, median, variance, inter-quartile range are
+        calculated. With 1GTF file input, gene mode can be used to generates these metrics for each gene
+        and summary statistics and distributions across genes. Distributions are visualized in a series
+        of plots.  For 1 GTF and 2GTF a pairwise mode calculates distance metrics between 2 transcripts
+        to the nucleotide.  In 1 GTF this is all possible pairs within the gene and in 2 GTF model this
+        is all possible pairs among GTF files. The distribution of these metrics across genes are
+        visualized and summary statistics for structural variations between pairs are calculated and
+        reported.  Visualizations of the distributions of the frequency of intron retention, alternative
+        exon usage, donor/acceptor variation and 5', 3' variation in UTR regions are provided as well as
+        tabular formatted nucleotide level distances for both 1GTF and 2 GTF.
+        
+        ## Installation
+        
+        The easiest way to install TranD is by using conda or mamba.
+        
+        ```
+        conda install -c bioconda trand
+        ```
+        
+        If you already have a suitable environment with bedtools installed and only want to add python
+        packages run
+        ```
+        pip install trand
+        ```
+        in an activated conda or virtualenv environment
+        
+        If you clone this repository you can use the source/requirements.txt file to pip install required dependencies with
+        ```
+        pip install -r source/requirements.txt
+        ```
+        See the [PyPI TranD page](https://pypi.org/project/trand/) for reference.
+        
+        We will add a conda trand package in the near future.
+        
 Keywords: transcript event and distance analysis
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# TranD: Transcript Distances
-
-TranD is a collection of tools to facilitate metrics of structural variation for whole genome
-transcript annotation files (GTF) that pinpoint structural variation to the nucleotide level.
-
-TranD (Transcript Distances) can be used to calculate metrics of structural variation within and
-between annotation files (GTF). Structural variation reflects organismal complexity and three
-summary metrics for genome level complexity are calculated for every gene in a GTF file:  1) the
-number of transcripts per gene; 2) the number of exons per transcript; and 3) the number of
-unique exons (exons with unique genomic coordinates) per gene. From each these metrics
-distributions a summary statistics such as mean, median, variance, inter-quartile range are
-calculated. With 1GTF file input, gene mode can be used to generates these metrics for each gene
-and summary statistics and distributions across genes. Distributions are visualized in a series
-of plots.  For 1 GTF and 2GTF a pairwise mode calculates distance metrics between 2 transcripts
-to the nucleotide.  In 1 GTF this is all possible pairs within the gene and in 2 GTF model this
-is all possible pairs among GTF files. The distribution of these metrics across genes are
-visualized and summary statistics for structural variations between pairs are calculated and
-reported.  Visualizations of the distributions of the frequency of intron retention, alternative
-exon usage, donor/acceptor variation and 5', 3' variation in UTR regions are provided as well as
-tabular formatted nucleotide level distances for both 1GTF and 2 GTF.
-
-## Installation
-
-The easiest way to install TranD is by using conda or mamba.
-
-```
-conda install -c bioconda trand
-```
-
-If you already have a suitable environment with bedtools installed and only want to add python
-packages run
-```
-pip install trand
-```
-in an activated conda or virtualenv environment
-
-If you clone this repository you can use the source/requirements.txt file to pip install required dependencies with
-```
-pip install -r source/requirements.txt
-```
-See the [PyPI TranD page](https://pypi.org/project/trand/) for reference.
-
-We will add a conda trand package in the near future.
```

### Comparing `trand-23.2.20/src/trand.egg-info/SOURCES.txt` & `trand-23.5.30/src/trand.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 src/trand/__init__.py
 src/trand/bedtools.py
 src/trand/calculate_complexity.py
-src/trand/consolidation.py
 src/trand/event_analysis.py
 src/trand/io.py
 src/trand/main.py
 src/trand/minimum_distance.py
 src/trand/plot_events.py
 src/trand/plot_functions.py
 src/trand/plot_one_gtf_gene.py
```

