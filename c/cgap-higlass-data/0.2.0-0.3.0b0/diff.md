# Comparing `tmp/cgap_higlass_data-0.2.0.tar.gz` & `tmp/cgap_higlass_data-0.3.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgap_higlass_data-0.2.0.tar", max compression
+gzip compressed data, was "cgap_higlass_data-0.3.0b0.tar", max compression
```

## Comparing `cgap_higlass_data-0.2.0.tar` & `cgap_higlass_data-0.3.0b0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1090 2022-10-11 17:52:02.790519 cgap_higlass_data-0.2.0/LICENSE
--rw-r--r--   0        0        0      381 2022-10-11 17:52:02.796041 cgap_higlass_data-0.2.0/README.md
--rw-r--r--   0        0        0        1 2022-07-04 15:38:47.258048 cgap_higlass_data-0.2.0/higlass_data/__init__.py
--rw-r--r--   0        0        0     1284 2023-03-31 12:32:02.123669 cgap_higlass_data-0.2.0/higlass_data/conversions.py
--rw-r--r--   0        0        0    12387 2023-03-31 11:38:01.145243 cgap_higlass_data-0.2.0/higlass_data/create_cohort_vcf.py
--rw-r--r--   0        0        0     3926 2023-03-31 10:45:17.550599 cgap_higlass_data-0.2.0/higlass_data/create_coverage_bed.py
--rw-r--r--   0        0        0     6148 2023-03-30 11:53:56.872920 cgap_higlass_data-0.2.0/higlass_data/data/.DS_Store
--rw-r--r--   0        0        0        1 2023-03-31 11:14:40.069331 cgap_higlass_data-0.2.0/higlass_data/data/__init__.py
--rw-r--r--   0        0        0    11672 2021-12-08 21:46:49.672243 cgap_higlass_data-0.2.0/higlass_data/data/hg38.chromsizes
--rw-r--r--   0        0        0      160 2023-03-30 12:48:34.735812 cgap_higlass_data-0.2.0/higlass_data/utils.py
--rw-r--r--   0        0        0     1419 2023-03-31 13:07:45.260327 cgap_higlass_data-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1698 1970-01-01 00:00:00.000000 cgap_higlass_data-0.2.0/setup.py
--rw-r--r--   0        0        0     1515 1970-01-01 00:00:00.000000 cgap_higlass_data-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2022-10-11 17:52:02.790519 cgap_higlass_data-0.3.0b0/LICENSE
+-rw-r--r--   0        0        0     2437 2023-04-04 16:01:10.419959 cgap_higlass_data-0.3.0b0/README.md
+-rw-r--r--   0        0        0        1 2022-07-04 15:38:47.258048 cgap_higlass_data-0.3.0b0/higlass_data/__init__.py
+-rw-r--r--   0        0        0     1284 2023-03-31 12:32:02.123669 cgap_higlass_data-0.3.0b0/higlass_data/conversions.py
+-rw-r--r--   0        0        0    12673 2023-05-30 19:39:08.405517 cgap_higlass_data-0.3.0b0/higlass_data/create_cohort_vcf.py
+-rw-r--r--   0        0        0     4069 2023-05-30 19:39:10.422811 cgap_higlass_data-0.3.0b0/higlass_data/create_coverage_bed.py
+-rw-r--r--   0        0        0     6148 2023-03-30 11:53:56.872920 cgap_higlass_data-0.3.0b0/higlass_data/data/.DS_Store
+-rw-r--r--   0        0        0        1 2023-03-31 11:14:40.069331 cgap_higlass_data-0.3.0b0/higlass_data/data/__init__.py
+-rw-r--r--   0        0        0    11672 2021-12-08 21:46:49.672243 cgap_higlass_data-0.3.0b0/higlass_data/data/hg38.chromsizes
+-rw-r--r--   0        0        0      364 2023-05-16 19:46:21.634852 cgap_higlass_data-0.3.0b0/higlass_data/data/hg38.mod.chromsizes
+-rw-r--r--   0        0        0      160 2023-03-30 12:48:34.735812 cgap_higlass_data-0.3.0b0/higlass_data/utils.py
+-rw-r--r--   0        0        0     1445 2023-05-30 19:42:14.576773 cgap_higlass_data-0.3.0b0/pyproject.toml
+-rw-r--r--   0        0        0     3612 1970-01-01 00:00:00.000000 cgap_higlass_data-0.3.0b0/PKG-INFO
```

### Comparing `cgap_higlass_data-0.2.0/LICENSE` & `cgap_higlass_data-0.3.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `cgap_higlass_data-0.2.0/higlass_data/conversions.py` & `cgap_higlass_data-0.3.0b0/higlass_data/conversions.py`

 * *Files identical despite different names*

### Comparing `cgap_higlass_data-0.2.0/higlass_data/create_cohort_vcf.py` & `cgap_higlass_data-0.3.0b0/higlass_data/create_cohort_vcf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import click
+from granite.lib import vcf_parser
 import vcf
 import pandas as pd
 import copy
 import negspy.coordinates as nc
 
 TILE_SIZE = 1024  # Higlass tile size for 1D tracks
 MAX_ZOOM_LEVEL = 23
@@ -151,19 +152,24 @@
 
         self.variants_df_hierarchical = hierarchical_variant_data
 
     def load_variants(self):
         if not self.quiet:
             print("Loading variants...")
         variants = []
-        vcf_reader = vcf.Reader(open(self.input_filepath, "r"))
-
-        for record in vcf_reader:
-            variants.append(record)
-
+        vcf_obj = vcf_parser.Vcf(self.input_filepath)
+        for record in vcf_obj.parse_variants():
+            variants.append({
+                "ID": record.ID,
+                "CHROM": record.CHROM,
+                "POS": record.POS,
+                "IMPORTANCE_VALUE": record.get_tag_value(self.importance_column),
+                "CONSEQUENCE": record.get_tag_value("level_most_severe_consequence"),
+            })
+        
         if not self.quiet:
             print("Loading variants complete.")
         return variants
 
     def index_variants_by_id(self):
         for variant in self.variants:
             self.variants_by_id[variant.ID] = variant
@@ -189,19 +195,19 @@
 
             chromosomes.append(variant.CHROM)
             ids.append(variant.ID)
             pos.append(variant.POS)
             absPos.append(
                 nc.chr_pos_to_genome_pos(variant.CHROM, variant.POS, self.chrom_info)
             )
-            importance_value = variant.INFO[self.importance_column][0]
+            importance_value = variant.IMPORTANCE_VALUE
             if importance_value == None or importance_value == "NA":
                 importance_value = 0.0
             importance_value = float(importance_value)
-            conseq = variant.INFO["level_most_severe_consequence"][0]
+            conseq = variant.CONSEQUENCE
 
             if conseq not in CONSEQUENCE_LEVELS:
                 print(f"Warning: Consequence level {conseq} not expected.")
             consequence.append(conseq)
 
             importance.append(self.importance(importance_value))
```

### Comparing `cgap_higlass_data-0.2.0/higlass_data/create_coverage_bed.py` & `cgap_higlass_data-0.3.0b0/higlass_data/create_coverage_bed.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import click
 import pandas as pd
-import vcf
+from granite.lib import vcf_parser
 import negspy.coordinates as nc
 
 TILE_SIZE = 1024  # Higlass tile size for 1D tracks
 MAX_ZOOM_LEVEL = 23
 
 
 class Coverage:
@@ -35,18 +35,21 @@
         self.tile_sizes = [TILE_SIZE * (2**i) for i in range(0, MAX_ZOOM_LEVEL)]
         self.chrom_info = nc.get_chrominfo(assembly)
 
     def load_variants(self):
         if not self.quiet:
             print("Loading variants...")
         variants = []
-        vcf_reader = vcf.Reader(open(self.input_filepath, "r"))
-
-        for record in vcf_reader:
-            variants.append(record)
+        vcf_obj = vcf_parser.Vcf(self.input_filepath)
+        for record in vcf_obj.parse_variants():
+            variants.append({
+                "ID": record.ID,
+                "CHROM": record.CHROM,
+                "POS": record.POS,
+            })
 
         if not self.quiet:
             print("Loading variants complete.")
         return variants
 
     # Create a matrix of the data that we use for filtering
     def create_variants_dataframe(self):
```

### Comparing `cgap_higlass_data-0.2.0/higlass_data/data/.DS_Store` & `cgap_higlass_data-0.3.0b0/higlass_data/data/.DS_Store`

 * *Files identical despite different names*

### Comparing `cgap_higlass_data-0.2.0/higlass_data/data/hg38.chromsizes` & `cgap_higlass_data-0.3.0b0/higlass_data/data/hg38.chromsizes`

 * *Files identical despite different names*

### Comparing `cgap_higlass_data-0.2.0/pyproject.toml` & `cgap_higlass_data-0.3.0b0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cgap-higlass-data"
-version = "0.2.0"
+version = "0.3.0b0"
 description = "Data file generation for CGAP's Higlass browsers"
 authors = ["Alexander Veit <alexander_veit@hms.harvard.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/dbmi-bgm/higlass-data"
 repository = "https://github.com/dbmi-bgm/higlass-data"
 packages = [
@@ -26,14 +26,15 @@
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
 click = "^8.1.3"
 pandas = "^1.4.3"
 negspy = "^0.2.24"
+granite-suite = "0.2.0"
 PyVCF3 = "^1.0.3"
 importlib-resources = "^5.12.0"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=7.1.2"
 
 [build-system]
```

