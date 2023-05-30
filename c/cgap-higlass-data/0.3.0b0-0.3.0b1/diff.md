# Comparing `tmp/cgap_higlass_data-0.3.0b0.tar.gz` & `tmp/cgap_higlass_data-0.3.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgap_higlass_data-0.3.0b0.tar", max compression
+gzip compressed data, was "cgap_higlass_data-0.3.0b1.tar", max compression
```

## Comparing `cgap_higlass_data-0.3.0b0.tar` & `cgap_higlass_data-0.3.0b1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1090 2022-10-11 17:52:02.790519 cgap_higlass_data-0.3.0b0/LICENSE
--rw-r--r--   0        0        0     2437 2023-04-04 16:01:10.419959 cgap_higlass_data-0.3.0b0/README.md
--rw-r--r--   0        0        0        1 2022-07-04 15:38:47.258048 cgap_higlass_data-0.3.0b0/higlass_data/__init__.py
--rw-r--r--   0        0        0     1284 2023-03-31 12:32:02.123669 cgap_higlass_data-0.3.0b0/higlass_data/conversions.py
--rw-r--r--   0        0        0    12673 2023-05-30 19:39:08.405517 cgap_higlass_data-0.3.0b0/higlass_data/create_cohort_vcf.py
--rw-r--r--   0        0        0     4069 2023-05-30 19:39:10.422811 cgap_higlass_data-0.3.0b0/higlass_data/create_coverage_bed.py
--rw-r--r--   0        0        0     6148 2023-03-30 11:53:56.872920 cgap_higlass_data-0.3.0b0/higlass_data/data/.DS_Store
--rw-r--r--   0        0        0        1 2023-03-31 11:14:40.069331 cgap_higlass_data-0.3.0b0/higlass_data/data/__init__.py
--rw-r--r--   0        0        0    11672 2021-12-08 21:46:49.672243 cgap_higlass_data-0.3.0b0/higlass_data/data/hg38.chromsizes
--rw-r--r--   0        0        0      364 2023-05-16 19:46:21.634852 cgap_higlass_data-0.3.0b0/higlass_data/data/hg38.mod.chromsizes
--rw-r--r--   0        0        0      160 2023-03-30 12:48:34.735812 cgap_higlass_data-0.3.0b0/higlass_data/utils.py
--rw-r--r--   0        0        0     1445 2023-05-30 19:42:14.576773 cgap_higlass_data-0.3.0b0/pyproject.toml
--rw-r--r--   0        0        0     3612 1970-01-01 00:00:00.000000 cgap_higlass_data-0.3.0b0/PKG-INFO
+-rw-r--r--   0        0        0     1090 2022-10-11 17:52:02.790519 cgap_higlass_data-0.3.0b1/LICENSE
+-rw-r--r--   0        0        0     2437 2023-04-04 16:01:10.419959 cgap_higlass_data-0.3.0b1/README.md
+-rw-r--r--   0        0        0        1 2022-07-04 15:38:47.258048 cgap_higlass_data-0.3.0b1/higlass_data/__init__.py
+-rw-r--r--   0        0        0     1284 2023-03-31 12:32:02.123669 cgap_higlass_data-0.3.0b1/higlass_data/conversions.py
+-rw-r--r--   0        0        0    12741 2023-05-30 20:06:10.854189 cgap_higlass_data-0.3.0b1/higlass_data/create_cohort_vcf.py
+-rw-r--r--   0        0        0     4087 2023-05-30 20:01:11.774635 cgap_higlass_data-0.3.0b1/higlass_data/create_coverage_bed.py
+-rw-r--r--   0        0        0     6148 2023-03-30 11:53:56.872920 cgap_higlass_data-0.3.0b1/higlass_data/data/.DS_Store
+-rw-r--r--   0        0        0        1 2023-03-31 11:14:40.069331 cgap_higlass_data-0.3.0b1/higlass_data/data/__init__.py
+-rw-r--r--   0        0        0    11672 2021-12-08 21:46:49.672243 cgap_higlass_data-0.3.0b1/higlass_data/data/hg38.chromsizes
+-rw-r--r--   0        0        0      364 2023-05-16 19:46:21.634852 cgap_higlass_data-0.3.0b1/higlass_data/data/hg38.mod.chromsizes
+-rw-r--r--   0        0        0      160 2023-03-30 12:48:34.735812 cgap_higlass_data-0.3.0b1/higlass_data/utils.py
+-rw-r--r--   0        0        0     1445 2023-05-30 20:07:38.009026 cgap_higlass_data-0.3.0b1/pyproject.toml
+-rw-r--r--   0        0        0     3612 1970-01-01 00:00:00.000000 cgap_higlass_data-0.3.0b1/PKG-INFO
```

### Comparing `cgap_higlass_data-0.3.0b0/LICENSE` & `cgap_higlass_data-0.3.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `cgap_higlass_data-0.3.0b0/README.md` & `cgap_higlass_data-0.3.0b1/README.md`

 * *Files identical despite different names*

### Comparing `cgap_higlass_data-0.3.0b0/higlass_data/conversions.py` & `cgap_higlass_data-0.3.0b1/higlass_data/conversions.py`

 * *Files identical despite different names*

### Comparing `cgap_higlass_data-0.3.0b0/higlass_data/create_cohort_vcf.py` & `cgap_higlass_data-0.3.0b1/higlass_data/create_cohort_vcf.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,16 +60,16 @@
                 print("  Current zoom level: ", zoom_level, ". Tile size: ", tile_size)
 
             # Don't do any aggregation, just copy the values with modified chr
             if zoom_level == 0:
                 for id in self.variants_by_id:
                     variant = self.variants_by_id[id]  # Retrieve original data
                     variant_copy = copy.copy(variant)
-                    if variant_copy.CHROM in self.chromosomes:
-                        variant_copy.CHROM = variant_copy.CHROM + "_" + str(zoom_level)
+                    if variant_copy["CHROM"] in self.chromosomes:
+                        variant_copy["CHROM"] = variant_copy["CHROM"] + "_" + str(zoom_level)
                         self.variants_multires.append(variant_copy)
                 continue
 
             current_index = 0
 
             num_tiles = 2 ** (MAX_ZOOM_LEVEL - zoom_level - 1)
             for current_index in range(0, num_tiles):
@@ -110,16 +110,16 @@
 
                         variant_in_bin_ids += list(variants_per_consequence.iloc[:, 1])
 
                 variant_in_bin_ids.sort()
                 for id in variant_in_bin_ids:
                     variant = self.variants_by_id[id]  # Retrieve original data
                     variant_copy = copy.copy(variant)
-                    if variant_copy.CHROM in self.chromosomes:
-                        variant_copy.CHROM = variant_copy.CHROM + "_" + str(zoom_level)
+                    if variant_copy["CHROM"] in self.chromosomes:
+                        variant_copy["CHROM"] = variant_copy["CHROM"] + "_" + str(zoom_level)
                         self.variants_multires.append(variant_copy)
 
     def split_variants(self):
         hierarchical_variant_data = {str(MAX_ZOOM_LEVEL - 1) + ".0": self.variants_df}
 
         for zoom_level in range((MAX_ZOOM_LEVEL - 1), 1, -1):
 
@@ -168,15 +168,16 @@
         
         if not self.quiet:
             print("Loading variants complete.")
         return variants
 
     def index_variants_by_id(self):
         for variant in self.variants:
-            self.variants_by_id[variant.ID] = variant
+            id = variant["ID"]
+            self.variants_by_id[id] = variant
 
     def importance(self, importance_value):
         # We are treating each consequence level separately, therefore we are just returning the chosen importance value here
         # We could do something more fance here and make it dependent on the consequence level
         return importance_value
 
     # Create a matrix of the data that we use for filtering
@@ -189,25 +190,25 @@
         consequence = []
 
         if not self.quiet:
             print("Creating data frame for easy querying during aggregation.")
 
         for variant in self.variants:
 
-            chromosomes.append(variant.CHROM)
-            ids.append(variant.ID)
-            pos.append(variant.POS)
+            chromosomes.append(variant["CHROM"])
+            ids.append(variant["ID"])
+            pos.append(variant["POS"])
             absPos.append(
-                nc.chr_pos_to_genome_pos(variant.CHROM, variant.POS, self.chrom_info)
+                nc.chr_pos_to_genome_pos(variant["CHROM"], variant["POS"], self.chrom_info)
             )
-            importance_value = variant.IMPORTANCE_VALUE
+            importance_value = variant["IMPORTANCE_VALUE"]
             if importance_value == None or importance_value == "NA":
                 importance_value = 0.0
             importance_value = float(importance_value)
-            conseq = variant.CONSEQUENCE
+            conseq = variant["CONSEQUENCE"]
 
             if conseq not in CONSEQUENCE_LEVELS:
                 print(f"Warning: Consequence level {conseq} not expected.")
             consequence.append(conseq)
 
             importance.append(self.importance(importance_value))
 
@@ -230,26 +231,26 @@
             for variant in self.variants_multires:
                 vcf_writer.write_record(variant)
                 vcf_writer.flush()
 
     def get_chromosomes(self):
         if not self.quiet:
             print("Extracting chromosomes...")
-        chrs = list(set(map(lambda v: v.CHROM, self.variants)))
+        chrs = list(set(map(lambda v: v["CHROM"], self.variants)))
         if "chrM" in chrs:
             chrs.remove("chrM")
         chrs.sort()
         if not self.quiet:
             print("Chromosomes used: ", chrs)
         return chrs
 
     def assign_ids(self):
         id = 0
         for variant in self.variants:
-            variant.ID = id
+            variant["ID"] = id
             id = id + 1
 
     
     # Currently unused. The idea was to not repeat variants on low zoom levels, if there is o aggregation.
     # This would have needed to be handled by the Higlass Cohort track accordingly. It's too complicated
     # and not worth it for now.
     def get_min_zoom_level(self):
```

### Comparing `cgap_higlass_data-0.3.0b0/higlass_data/create_coverage_bed.py` & `cgap_higlass_data-0.3.0b1/higlass_data/create_coverage_bed.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,33 +59,33 @@
         absPos = []
 
         if not self.quiet:
             print("Creating data frame for easy querying during aggregation.")
 
         for variant in self.variants:
 
-            chromosomes.append(variant.CHROM)
-            ids.append(variant.ID)
-            pos.append(variant.POS)
+            chromosomes.append(variant["CHROM"])
+            ids.append(variant["ID"])
+            pos.append(variant["POS"])
             absPos.append(
-                nc.chr_pos_to_genome_pos(variant.CHROM, variant.POS, self.chrom_info)
+                nc.chr_pos_to_genome_pos(variant["CHROM"], variant["POS"], self.chrom_info)
             )
 
         d = {
             "chr": chromosomes,
             "id": ids,
             "pos": pos,
             "absPos": absPos
         }
         self.variants_df = pd.DataFrame(data=d)
 
     def get_chromosomes(self):
         if not self.quiet:
             print("Extracting chromosomes...")
-        chrs = list(set(map(lambda v: v.CHROM, self.variants)))
+        chrs = list(set(map(lambda v: v["CHROM"], self.variants)))
         if "chrM" in chrs:
             chrs.remove("chrM")
         chrs.sort()
         if not self.quiet:
             print("Chromosomes used: ", chrs)
         return chrs
```

### Comparing `cgap_higlass_data-0.3.0b0/higlass_data/data/.DS_Store` & `cgap_higlass_data-0.3.0b1/higlass_data/data/.DS_Store`

 * *Files identical despite different names*

### Comparing `cgap_higlass_data-0.3.0b0/higlass_data/data/hg38.chromsizes` & `cgap_higlass_data-0.3.0b1/higlass_data/data/hg38.chromsizes`

 * *Files identical despite different names*

### Comparing `cgap_higlass_data-0.3.0b0/pyproject.toml` & `cgap_higlass_data-0.3.0b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cgap-higlass-data"
-version = "0.3.0b0"
+version = "0.3.0b1"
 description = "Data file generation for CGAP's Higlass browsers"
 authors = ["Alexander Veit <alexander_veit@hms.harvard.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/dbmi-bgm/higlass-data"
 repository = "https://github.com/dbmi-bgm/higlass-data"
 packages = [
```

### Comparing `cgap_higlass_data-0.3.0b0/PKG-INFO` & `cgap_higlass_data-0.3.0b1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgap-higlass-data
-Version: 0.3.0b0
+Version: 0.3.0b1
 Summary: Data file generation for CGAP's Higlass browsers
 Home-page: https://github.com/dbmi-bgm/higlass-data
 License: MIT
 Author: Alexander Veit
 Author-email: alexander_veit@hms.harvard.edu
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

