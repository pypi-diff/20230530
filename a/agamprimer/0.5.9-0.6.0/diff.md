# Comparing `tmp/AgamPrimer-0.5.9.tar.gz` & `tmp/agamprimer-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AgamPrimer-0.5.9.tar", max compression
+gzip compressed data, was "agamprimer-0.6.0.tar", max compression
```

## Comparing `AgamPrimer-0.5.9.tar` & `agamprimer-0.6.0.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0    31190 2022-10-22 17:25:24.757208 AgamPrimer-0.5.9/AgamPrimer/AgamPrimer.py
--rw-r--r--   0        0        0       66 2022-10-08 12:28:16.376117 AgamPrimer-0.5.9/AgamPrimer/__init__.py
--rw-r--r--   0        0        0      761 2022-10-08 11:18:21.612054 AgamPrimer-0.5.9/AgamPrimer/agamPrimer.egg-info/PKG-INFO
--rw-r--r--   0        0        0        0 2022-06-16 14:07:08.758739 AgamPrimer-0.5.9/AgamPrimer/agamPrimer.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        0 2022-10-08 11:18:21.612054 AgamPrimer-0.5.9/AgamPrimer/agamPrimer.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       11 2022-06-16 14:07:53.402854 AgamPrimer-0.5.9/AgamPrimer/agamPrimer.egg-info/top_level.txt
--rw-r--r--   0        0        0     1079 2022-10-08 11:18:21.612054 AgamPrimer-0.5.9/LICENSE
--rw-r--r--   0        0        0      696 2022-10-22 17:34:47.077232 AgamPrimer-0.5.9/pyproject.toml
--rw-r--r--   0        0        0      806 2022-10-22 17:39:19.521051 AgamPrimer-0.5.9/setup.py
--rw-r--r--   0        0        0      629 2022-10-22 17:39:19.521269 AgamPrimer-0.5.9/PKG-INFO
+-rw-r--r--   0        0        0    35049 2023-05-30 16:51:46.998781 agamprimer-0.6.0/AgamPrimer/AgamPrimer.py
+-rw-r--r--   0        0        0       66 2022-12-19 20:36:15.048061 agamprimer-0.6.0/AgamPrimer/__init__.py
+-rw-r--r--   0        0        0      761 2023-05-30 16:51:46.998781 agamprimer-0.6.0/AgamPrimer/agamPrimer.egg-info/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-30 16:51:46.998781 agamprimer-0.6.0/AgamPrimer/agamPrimer.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        0 2023-05-30 16:51:46.998781 agamprimer-0.6.0/AgamPrimer/agamPrimer.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       11 2023-05-30 16:51:46.998781 agamprimer-0.6.0/AgamPrimer/agamPrimer.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1079 2022-10-08 11:18:21.612054 agamprimer-0.6.0/LICENSE
+-rw-r--r--   0        0        0      726 2023-05-30 17:24:09.942962 agamprimer-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      729 1970-01-01 00:00:00.000000 agamprimer-0.6.0/PKG-INFO
```

### Comparing `AgamPrimer-0.5.9/AgamPrimer/AgamPrimer.py` & `agamprimer-0.6.0/AgamPrimer/AgamPrimer.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,35 +20,36 @@
     assay_name,
     assay_type,
     probe_exclude_region_size=20,
 ):
     """
     Extracts sequence of interest from genome sequence
     """
+    target = int(target_loc)
     # Set up range for the input sequence, we'll take the max range
     # of the amplicon size and add that either side of the target SNP
     amp_size_range = int(np.max(amplicon_size_range))
-    start = target_loc - amp_size_range
-    end = target_loc + amp_size_range
+    start = target - amp_size_range
+    end = target + amp_size_range
     # join array into be one character string, and store the positions
     # of these sequences for later
     target_sequence = "".join(genome_seq[start : end - 1].compute().astype(str))
     gdna_pos = np.arange(start, end).astype(int) + 1
     print(f"The target sequence is {len(target_sequence)} bases long")
 
     # We need the target snp indices within the region of interest
-    target_loc_primer3 = int(np.where(gdna_pos == target_loc)[0])
+    target_loc_primer3 = int(np.where(gdna_pos == target)[0])
     target_loc_primer3 = [target_loc_primer3, 10]
     print(f"the target snp is {target_loc_primer3[0]} bp into our target sequence")
 
     seq_parameters = {
         "SEQUENCE_ID": assay_name,
         "SEQUENCE_TEMPLATE": target_sequence,
         "SEQUENCE_TARGET": target_loc_primer3,
-        "GENOMIC_SEQUENCE_TARGET": target_loc,
+        "GENOMIC_TARGET": target,
     }
 
     if "probe" in assay_type:
         seq_parameters["SEQUENCE_INTERNAL_EXCLUDED_REGION"] = [
             [1, target_loc_primer3[0] - probe_exclude_region_size],
             [
                 target_loc_primer3[0] + probe_exclude_region_size,
@@ -56,19 +57,20 @@
                 - (target_loc_primer3[0] + probe_exclude_region_size),
             ],
         ]
 
     return (target_sequence, gdna_pos, seq_parameters)
 
 
-def prepare_cDNA_sequence(transcript, gff, genome_seq, assay_name):
+def prepare_cDNA_sequence(transcript, genome_seq, assay_name, cDNA_exon_junction):
     """
     Extract exonic sequence for our transcript and record exon-exon junctions
     """
     # subset gff to your gene
+    gff = ag3.geneset()
     gff = gff.query("type == 'exon' & Parent == @transcript")
     # Get fasta sequence for each of our exons, and remember gDNA position
     seq = dict()
     gdna_pos = dict()
     for i, exon in enumerate(zip(gff.start, gff.end)):
         seq[i] = "".join(np.array(genome_seq)[exon[0] - 1 : exon[1]].astype(str))
         gdna_pos[i] = np.arange(exon[0] - 1, exon[1])
@@ -80,19 +82,56 @@
     exon_junctions = np.array(np.cumsum(gff.end - gff.start))[:-1]
     exon_sizes = np.array(gff.end - gff.start)[:-1]
     exon_junctions_pos = [ex + gff.iloc[i, 3] for i, ex in enumerate(exon_sizes)]
     print(f"Exon junctions for {transcript}:", exon_junctions, exon_junctions_pos, "\n")
     seq_parameters = {
         "SEQUENCE_ID": assay_name,
         "SEQUENCE_TEMPLATE": target_mRNA_seq,
-        "SEQUENCE_OVERLAP_JUNCTION_LIST": list(map(int, exon_junctions)),
-        "TRANSCRIPT": transcript,
+        "GENOMIC_TARGET": transcript,
     }
 
-    return (target_mRNA_seq, list(map(int, exon_junctions)), gdna_pos, seq_parameters)
+    if cDNA_exon_junction:
+        seq_parameters["SEQUENCE_OVERLAP_JUNCTION_LIST"] = list(
+            map(int, exon_junctions)
+        )
+
+    return (target_mRNA_seq, gdna_pos, seq_parameters)
+
+
+def prepare_sequence(
+    target,
+    assay_type,
+    assay_name,
+    genome_seq,
+    amplicon_size_range,
+    cDNA_exon_junction=True,
+):
+    """
+    Prepare the sequence for primer3, depending on cDNA or gDNA input type
+    """
+
+    if any(item in assay_type for item in ["gDNA", "probe"]):
+        # genomic DNA
+        target_sequence, gdna_pos, seq_parameters = prepare_gDNA_sequence(
+            target_loc=target,
+            amplicon_size_range=amplicon_size_range,
+            genome_seq=genome_seq,
+            assay_name=assay_name,
+            assay_type=assay_type,
+        )
+    elif assay_type == "cDNA primers":
+        # quantitative PCR
+        target_sequence, gdna_pos, seq_parameters = prepare_cDNA_sequence(
+            transcript=target,
+            genome_seq=genome_seq,
+            assay_name=assay_name,
+            cDNA_exon_junction=cDNA_exon_junction,
+        )
+
+    return (target_sequence, gdna_pos, seq_parameters)
 
 
 def primer_params(
     assay_type,
     primer_parameters=None,
     n_primer_pairs=None,
     amplicon_size_range=None,
@@ -206,86 +245,77 @@
     return primer_df
 
 
 def plot_primer_ag3_frequencies(
     primer_df,
     gdna_pos,
     contig,
-    sample_set,
+    sample_sets,
     assay_type,
     seq_parameters,
     out_dir=None,
     sample_query=None,
 ):
     """
     Loop through n primer pairs, retrieving frequency data and plot allele frequencies
     """
 
     if sample_query is not None:
         print(f"Subsetting allele frequencies to {sample_query}")
 
     name = seq_parameters["SEQUENCE_ID"]
-    # exon_junctions = (
-    #     seq_parameters["SEQUENCE_OVERLAP_JUNCTION_LIST"]
-    #     if assay_type == "cDNA primers"
-    #     else None
-    # )
-    transcript = seq_parameters["TRANSCRIPT"] if assay_type == "cDNA primers" else None
-    target_loc = (
-        seq_parameters["GENOMIC_SEQUENCE_TARGET"]
-        if any(item in assay_type for item in ["gDNA", "probe"])
-        else None
-    )
+    target = seq_parameters["GENOMIC_TARGET"]
+
     res_dict = {}
     # Loop through each primer pair and get the frequencies of alternate alleles, storing in dict
     for i in range(len(primer_df.columns)):
         res_dict[i] = _get_primer_alt_frequencies(
-            primer_df, gdna_pos, i, sample_set, assay_type, contig, sample_query
+            primer_df, gdna_pos, i, sample_sets, assay_type, contig, sample_query
         )
 
     # Plot data with plotly
     _plotly_primers(
         primer_df=primer_df,
         res_dict=res_dict,
         name=name,
         assay_type=assay_type,
-        sample_set=sample_set,
-        target_loc=target_loc,
-        transcript=transcript,
+        sample_sets=sample_sets,
+        target=target,
         out_dir=out_dir,
     )
 
     return res_dict
 
 
 def plot_primer_locs(
     primer_res_dict,
     primer_df,
-    gff,
     contig,
     seq_parameters,
     assay_type,
     legend_loc="best",
     out_dir=None,
 ):
     """
     Plot the position of the primer sets in relation to any nearby exons
     """
     oligos, _ = _return_oligo_list(assay_type)
     assay_name = seq_parameters["SEQUENCE_ID"]
     # Load geneset (gff)
+    gff = ag3.geneset()
     if any(item in assay_type for item in ["gDNA", "probe"]):
-        start = seq_parameters["GENOMIC_SEQUENCE_TARGET"] - 500
-        end = seq_parameters["GENOMIC_SEQUENCE_TARGET"] + 500
+        start = seq_parameters["GENOMIC_TARGET"] - 500
+        end = seq_parameters["GENOMIC_TARGET"] + 500
         locgff, min_, max_, genegff = _get_gDNA_locs(gff, contig, start, end)
         min_ = np.min([min_, start])
         max_ = np.max([max_, end])
     elif assay_type == "cDNA primers":
-        transcript = seq_parameters["TRANSCRIPT"]
-        locgff, min_, max_, genegff = _get_qPCR_locs(gff, contig, transcript)
+        locgff, min_, max_, genegff = _get_qPCR_locs(
+            gff, contig, seq_parameters["GENOMIC_TARGET"]
+        )
 
     if locgff.empty:
         print("No exons in close proximity for loc plot")
         return
 
     fig, ax = plt.subplots(1, 1, figsize=[16, 4])
     # configure axes
@@ -442,32 +472,104 @@
 
     if pair_dict:
         return pd.concat(pair_dict)
     else:
         print("No HITs found for these primer pairs")
 
 
+def check_and_split_target(target, assay_type):
+    # split contig from target
+    if target.startswith("AGAP"):
+        assert (
+            assay_type == "cDNA primers"
+        ), "an AGAP identifier is specified, but the assay type is not cDNA primers. Please provide a contig:position identifier for gDNA primers."
+        gff = ag3.geneset()
+        assert (
+            target in gff["ID"].to_list()
+        ), f"requested target {target} not in ag3 transcript set"
+        contig = gff.query("ID == @target")["contig"].unique()[0]
+        return (contig, target)
+    else:
+        assert isinstance(
+            target, str
+        ), "For genomic DNA the target should be a string, such as '2L:28545767'"
+        contig, target = target.split(":")
+        assert contig in [
+            "2L",
+            "2R",
+            "3L",
+            "3R",
+            "X",
+        ], "target contig not recognised, should be 2L, 2R, 3L, 3R or X"
+        return (contig, int(target))
+
+
 def designPrimers(
     assay_type,
     assay_name,
     min_amplicon_size,
     max_amplicon_size,
     n_primer_pairs,
-    contig,
     target,
     primer_parameters,
-    sample_set,
+    sample_sets,
     sample_query=None,
     out_dir=None,
+    cDNA_exon_junction=True,
 ):
     """
     Run whole AgamPrimer workflow to design primers/probes with in one function
+
+    Parameters
+    ----------
+    assay_type: {'gDNA primers', 'cDNA primers', 'gDNA primers + probe', 'probe}, str
+        The type of oligos we wish to design. If 'gDNA primers' or 'cDNA primers' are specified,
+        then only primers will be designed. If 'gDNA primers + probe' is specified, then primers
+        and a probe will be designed. If 'probe' is specified, then only an internal probe will
+        be designed.
+    assay_name : str
+        A name to give the assay, used for naming output files.
+    min_amplicon_size : int
+        The minimum size of the amplicon we wish to design primers for.
+    max_amplicon_size : int
+        The maximum size of the amplicon we wish to design primers for. cDNA primers for gene
+        expression assays should be designed with a max amplicon size of ~120.
+    n_primer_pairs : int
+        The number of primer pairs to design.
+    target : str
+        The target to design primers for. For gDNA primers, this should be a contig:position string,
+        for example '2L:28545767'. For cDNA primers, this should be an AGAP identifier.
+    primer_parameters : dict or 'default'
+        A dictionary of primer3 parameters to use for primer design. If 'default' is specified, default
+        primer3 parameters will be generated.
+    sample_sets : str or list of str, optional
+        Can be a sample set identifier (e.g., "AG1000G-AO") or a list of
+        sample set identifiers (e.g., ["AG1000G-BF-A", "AG1000G-BF-B"]) or a
+        release identifier (e.g., "3.0") or a list of release identifiers.
+    sample_query: str, optional
+        A pandas query string which will be evaluated against the sample
+        metadata e.g., "taxon == 'coluzzii' and country == 'Burkina Faso'".
+    out_dir : str, optional
+        The directory to write output files to. If not specified, outputs will not be written to file.
+    cDNA_exon_junction : bool, optional
+        If True, cDNA primers will be designed to span an exon-exon junction. We strongly recommend
+        that this is set to True. In the case of gDNA primers, this parameter is ignored.
+
+        Returns
+        -------
+        primer_df : pandas.DataFrame
+            A pandas DataFrame containing the primer sequences and their information.
+        blat_df : pandas.DataFrame
+            A pandas DataFrame containing the BLAT alignment information for the primers.
     """
 
+    # check target is valid for assay type and find contig
+    contig, target = check_and_split_target(target=target, assay_type=assay_type)
     amplicon_size_range = [[min_amplicon_size, max_amplicon_size]]
+
     # adds some necessary parameters depending on assay type
     if primer_parameters == "default":
         primer_parameters = primer_params(
             primer_parameters=None,
             assay_type=assay_type,
             n_primer_pairs=n_primer_pairs,
             amplicon_size_range=amplicon_size_range,
@@ -477,112 +579,96 @@
         primer_parameters = primer_params(
             primer_parameters=primer_parameters,
             assay_type=assay_type,
             n_primer_pairs=n_primer_pairs,
             amplicon_size_range=amplicon_size_range,
             generate_defaults=False,
         )
-
-    if assay_type == "cDNA primers":
-        assert not isinstance(
-            target, int
-        ), "cDNA primers chosen but an AGAP identifier is not provided as the target"
-        assert target.startswith(
-            "AGAP"
-        ), "cDNA primers chosen but an AGAP identifier is not provided as the target"
-        transcript = target
-        target_loc = ""
-    else:
-        assert isinstance(
-            target, int
-        ), "For genomic DNA the target should be an integer within the contig"
-        transcript = ""
-        target_loc = target
-
+    # load genome sequence
     genome_seq = ag3.genome_sequence(region=contig)
     print(f"Our genome sequence for {contig} is {genome_seq.shape[0]} bp long")
 
-    if any(item in assay_type for item in ["gDNA", "probe"]):
-        # genomic DNA
-        target_sequence, gdna_pos, seq_parameters = prepare_gDNA_sequence(
-            target_loc=target_loc,
-            amplicon_size_range=amplicon_size_range,
-            genome_seq=genome_seq,
-            assay_name=assay_name,
-            assay_type=assay_type,
-        )
-    elif assay_type == "cDNA primers":
-        # RT-quantitative PCR, cDNA
-        (
-            target_sequence,
-            exon_junctions,
-            gdna_pos,
-            seq_parameters,
-        ) = prepare_cDNA_sequence(
-            transcript=transcript,
-            gff=ag3.geneset(),
-            genome_seq=genome_seq,
-            assay_name=assay_name,
-        )
+    target_sequence, gdna_pos, seq_parameters = prepare_sequence(
+        target=target,
+        assay_type=assay_type,
+        assay_name=assay_name,
+        genome_seq=genome_seq,
+        amplicon_size_range=amplicon_size_range,
+        cDNA_exon_junction=cDNA_exon_junction,
+    )
 
+    # run primer3
     primer_dict = primer3.designPrimers(
         seq_args=seq_parameters, global_args=primer_parameters
     )
+
+    if assay_type != "probe":
+        # check if primer3 has returned any primers
+        if int(primer_dict["PRIMER_PAIR_EXPLAIN"][-1]) == 0:
+            print(
+                f"No primers found for {assay_name}. For cDNA primers, this is more likely to occur if the target contains only one exon-exon junction. see troubleshooting below for more information. We suggest relaxing the primer parameters \n"
+            )
+            print(primer3_run_statistics(primer_dict, assay_type))
+            return (None, None)
+
     # AgamPrimer.primer3_run_statistics(primer_dict, assay_type)
     primer_df = primer3_to_pandas(primer_dict=primer_dict, assay_type=assay_type)
 
+    # write primer3 output to file
     if out_dir:
         primer_df.to_csv(f"{out_dir}/{assay_name}.{assay_type}.tsv", sep="\t")
         primer_df.to_excel(f"{out_dir}/{assay_name}.{assay_type}.xlsx")
 
+    # plot frequencies of alleles in primer pairs
     results_dict = plot_primer_ag3_frequencies(
         primer_df=primer_df,
         gdna_pos=gdna_pos,
         contig=contig,
-        sample_set=sample_set,
+        sample_sets=sample_sets,
         sample_query=sample_query,
         assay_type=assay_type,
         seq_parameters=seq_parameters,
         out_dir=out_dir,
     )
+    # plot primer locations on genome
     plot_primer_locs(
         primer_res_dict=results_dict,
         primer_df=primer_df,
         assay_type=assay_type,
-        gff=ag3.geneset(),
         contig=contig,
         seq_parameters=seq_parameters,
         legend_loc="lower left",
         out_dir=out_dir,
     )
+    # check primers for specificity against the genome and write to file
     blat_df = gget_blat_genome(primer_df, assay_type, assembly="anoGam3")
     blat_df.to_csv(f"{out_dir}/{assay_name}.{assay_type}.blat.tsv", sep="\t")
     return (primer_df, blat_df)
 
 
-def _get_primer_arrays(contig, gdna_pos, sample_set, assay_type, sample_query=None):
+def _get_primer_arrays(contig, gdna_pos, sample_sets, assay_type, sample_query=None):
 
     if any(item in assay_type for item in ["gDNA", "probe"]):
         span_str = f"{contig}:{gdna_pos.min()}-{gdna_pos.max()}"
         snps = ag3.snp_calls(
-            region=span_str, sample_sets=sample_set, sample_query=sample_query
+            region=span_str, sample_sets=sample_sets, sample_query=sample_query
         )  # get genotypes
         ref_alt_arr = snps["variant_allele"].compute().values
         geno = snps["call_genotype"]
         freq_arr = allel.GenotypeArray(geno).count_alleles().to_frequencies()
         pos_arr = gdna_pos
     elif assay_type == "cDNA primers":
         freq_arr = []
         ref_alt_arr = []
         pos_arr = np.array([])
         exon_spans = np.array(_consecutive(gdna_pos)) + 1
         for span in exon_spans:
             span_str = f"{contig}:{span[0]}-{span[1]}"
             snps = ag3.snp_calls(
-                region=span_str, sample_sets=sample_set, sample_query=sample_query
+                region=span_str, sample_sets=sample_sets, sample_query=sample_query
             )  # get genotypes
             ref_alts = snps["variant_allele"]
             geno = snps["call_genotype"]
             freqs = (
                 allel.GenotypeArray(geno).count_alleles().to_frequencies()
             )  # calculate allele frequencies
             freqs = _addZeroCols(freqs)
@@ -592,26 +678,26 @@
         freq_arr = np.concatenate(freq_arr)
         ref_alt_arr = np.concatenate(ref_alt_arr)
 
     return (freq_arr, ref_alt_arr.astype("U13"), pos_arr)
 
 
 def _get_primer_alt_frequencies(
-    primer_df, gdna_pos, pair, sample_set, assay_type, contig, sample_query
+    primer_df, gdna_pos, pair, sample_sets, assay_type, contig, sample_query
 ):
     """
     Find the genomic locations of pairs of primers, and runs span_to_freq
     to get allele frequencies at those locations
     """
 
     oligos, _ = _return_oligo_list(assay_type)
     base_freqs, ref_alt_arr, pos_arr = _get_primer_arrays(
         contig=contig,
         gdna_pos=gdna_pos,
-        sample_set=sample_set,
+        sample_sets=sample_sets,
         assay_type=assay_type,
         sample_query=sample_query,
     )
 
     freq_arr = base_freqs[:, 1:].sum(axis=1)
 
     di = {}
@@ -650,17 +736,16 @@
 
 
 def _plotly_primers(
     primer_df,
     res_dict,
     name,
     assay_type,
-    sample_set,
-    target_loc,
-    transcript,
+    sample_sets,
+    target,
     out_dir=None,
 ):
 
     oligos, _ = _return_oligo_list(assay_type)
     if len(oligos) == 2:
         plt_title = ["Forward primer", "Reverse primer"]
     elif len(oligos) == 3:
@@ -797,19 +882,19 @@
                     mirror=True,
                 )
 
             if ((row_i % 2) == 0) & (idx == 1):
                 fig.update_yaxes(row=row_i, col=idx, title="Alternate allele frequency")
 
     if any(item in assay_type for item in ["gDNA"]):
-        title_text = f"{name} primer pairs | {sample_set} | target {target_loc} bp"
+        title_text = f"{name} primer pairs | {sample_sets} | target {target} bp"
     elif assay_type == "probe":
-        title_text = f"{name} probe | {sample_set} | target {target_loc} bp"
+        title_text = f"{name} probe | {sample_sets} | target {target} bp"
     elif assay_type == "cDNA primers":
-        title_text = f"{name} primer pairs | {sample_set} | target {transcript}"
+        title_text = f"{name} primer pairs | {sample_sets} | target {target}"
 
     # fig.update_traces(customdata=customdata, hovertemplate=hovertemplate)
     fig.update_layout(
         height=200 * len(primer_df.columns),
         width=500 * len(oligos),
         title_text=title_text,
         title_x=0.5,
```

### Comparing `AgamPrimer-0.5.9/AgamPrimer/agamPrimer.egg-info/PKG-INFO` & `agamprimer-0.6.0/AgamPrimer/agamPrimer.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `AgamPrimer-0.5.9/LICENSE` & `agamprimer-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `AgamPrimer-0.5.9/pyproject.toml` & `agamprimer-0.6.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 [tool.poetry]
 name = "AgamPrimer"
-version = "0.5.9"
+version = "0.6.0"
 description = "A package to design primers in Anopheles gambiae whilst considering genetic variation with malariagen_data"
 authors = [
     "Sanjay Nagi <sanjay.nagi@lstmed.ac.uk>",
     ]
 packages = [
     { include = "AgamPrimer" }
 ]
 license = "MIT"
 
 [tool.poetry.dependencies]
-python = ">=3.7.1,<3.10"
+python = ">=3.8,<3.12"
 primer3-py = "*"
 malariagen_data = "*"
 openpyxl = "*"
 gget = "*"
 seaborn = "*"
 kaleido = "0.2.1"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "*"
 black = "*"
 pytest = "*"
 notebook = "*"
 jupyterlab = "*"
 snakeviz = "*"
+papermill = "*"
+ipykernel = "*"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

