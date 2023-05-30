# Comparing `tmp/spectrum_fundamentals-0.3.1.tar.gz` & `tmp/spectrum_fundamentals-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrum_fundamentals-0.3.1.tar", max compression
+gzip compressed data, was "spectrum_fundamentals-0.3.2.tar", max compression
```

## Comparing `spectrum_fundamentals-0.3.1.tar` & `spectrum_fundamentals-0.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1073 2023-04-30 18:37:48.694880 spectrum_fundamentals-0.3.1/LICENSE
--rw-r--r--   0        0        0     2611 2023-04-30 18:37:48.694880 spectrum_fundamentals-0.3.1/README.rst
--rw-r--r--   0        0        0     2367 2023-04-30 18:37:48.698880 spectrum_fundamentals-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      940 2023-04-30 18:37:48.698880 spectrum_fundamentals-0.3.1/spectrum_fundamentals/__init__.py
--rw-r--r--   0        0        0      381 2023-04-30 18:37:48.698880 spectrum_fundamentals-0.3.1/spectrum_fundamentals/__main__.py
--rw-r--r--   0        0        0       29 2023-04-30 18:37:48.698880 spectrum_fundamentals-0.3.1/spectrum_fundamentals/annotation/__init__.py
--rw-r--r--   0        0        0    11153 2023-04-30 18:37:48.698880 spectrum_fundamentals-0.3.1/spectrum_fundamentals/annotation/annotation.py
--rw-r--r--   0        0        0     1372 2023-04-30 18:37:48.698880 spectrum_fundamentals-0.3.1/spectrum_fundamentals/charge.py
--rw-r--r--   0        0        0     7819 2023-04-30 18:37:48.698880 spectrum_fundamentals-0.3.1/spectrum_fundamentals/constants.py
--rw-r--r--   0        0        0    12452 2023-04-30 18:37:48.698880 spectrum_fundamentals-0.3.1/spectrum_fundamentals/fragments.py
--rw-r--r--   0        0        0       26 2023-04-30 18:37:48.698880 spectrum_fundamentals-0.3.1/spectrum_fundamentals/metrics/__init__.py
--rw-r--r--   0        0        0    14554 2023-04-30 18:37:48.698880 spectrum_fundamentals-0.3.1/spectrum_fundamentals/metrics/fragments_ratio.py
--rw-r--r--   0        0        0     1435 2023-04-30 18:37:48.698880 spectrum_fundamentals-0.3.1/spectrum_fundamentals/metrics/metric.py
--rw-r--r--   0        0        0    22213 2023-04-30 18:37:48.698880 spectrum_fundamentals-0.3.1/spectrum_fundamentals/metrics/percolator.py
--rw-r--r--   0        0        0    22378 2023-04-30 18:37:48.698880 spectrum_fundamentals-0.3.1/spectrum_fundamentals/metrics/similarity.py
--rw-r--r--   0        0        0     9443 2023-04-30 18:37:48.698880 spectrum_fundamentals-0.3.1/spectrum_fundamentals/mod_string.py
--rw-r--r--   0        0        0        0 2023-04-30 18:37:48.698880 spectrum_fundamentals-0.3.1/spectrum_fundamentals/py.typed
--rw-r--r--   0        0        0     3856 1970-01-01 00:00:00.000000 spectrum_fundamentals-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-30 08:42:44.965094 spectrum_fundamentals-0.3.2/LICENSE
+-rw-r--r--   0        0        0     2611 2023-05-30 08:42:44.965094 spectrum_fundamentals-0.3.2/README.rst
+-rw-r--r--   0        0        0     2367 2023-05-30 08:42:44.969094 spectrum_fundamentals-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      940 2023-05-30 08:42:44.969094 spectrum_fundamentals-0.3.2/spectrum_fundamentals/__init__.py
+-rw-r--r--   0        0        0      381 2023-05-30 08:42:44.969094 spectrum_fundamentals-0.3.2/spectrum_fundamentals/__main__.py
+-rw-r--r--   0        0        0       29 2023-05-30 08:42:44.969094 spectrum_fundamentals-0.3.2/spectrum_fundamentals/annotation/__init__.py
+-rw-r--r--   0        0        0    11153 2023-05-30 08:42:44.969094 spectrum_fundamentals-0.3.2/spectrum_fundamentals/annotation/annotation.py
+-rw-r--r--   0        0        0     1372 2023-05-30 08:42:44.969094 spectrum_fundamentals-0.3.2/spectrum_fundamentals/charge.py
+-rw-r--r--   0        0        0     7807 2023-05-30 08:42:44.969094 spectrum_fundamentals-0.3.2/spectrum_fundamentals/constants.py
+-rw-r--r--   0        0        0    12452 2023-05-30 08:42:44.969094 spectrum_fundamentals-0.3.2/spectrum_fundamentals/fragments.py
+-rw-r--r--   0        0        0       26 2023-05-30 08:42:44.969094 spectrum_fundamentals-0.3.2/spectrum_fundamentals/metrics/__init__.py
+-rw-r--r--   0        0        0    14554 2023-05-30 08:42:44.969094 spectrum_fundamentals-0.3.2/spectrum_fundamentals/metrics/fragments_ratio.py
+-rw-r--r--   0        0        0     1435 2023-05-30 08:42:44.969094 spectrum_fundamentals-0.3.2/spectrum_fundamentals/metrics/metric.py
+-rw-r--r--   0        0        0    22674 2023-05-30 08:42:44.969094 spectrum_fundamentals-0.3.2/spectrum_fundamentals/metrics/percolator.py
+-rw-r--r--   0        0        0    22390 2023-05-30 08:42:44.969094 spectrum_fundamentals-0.3.2/spectrum_fundamentals/metrics/similarity.py
+-rw-r--r--   0        0        0     9443 2023-05-30 08:42:44.969094 spectrum_fundamentals-0.3.2/spectrum_fundamentals/mod_string.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:42:44.969094 spectrum_fundamentals-0.3.2/spectrum_fundamentals/py.typed
+-rw-r--r--   0        0        0     3705 1970-01-01 00:00:00.000000 spectrum_fundamentals-0.3.2/PKG-INFO
```

### Comparing `spectrum_fundamentals-0.3.1/LICENSE` & `spectrum_fundamentals-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.3.1/README.rst` & `spectrum_fundamentals-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.3.1/pyproject.toml` & `spectrum_fundamentals-0.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spectrum_fundamentals"
-version = "0.3.1"  # <<COOKIETEMPLE_FORCE_BUMP>>
+version = "0.3.2"  # <<COOKIETEMPLE_FORCE_BUMP>>
 description = "Fundamentals public repo"
 authors = ["WassimG <wassim.gabriel@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/wilhelm-lab/spectrum_fundamentals"
 repository = "https://github.com/wilhelm-lab/spectrum_fundamentals"
 documentation = "https://spectrum_fundamentals.readthedocs.io"
```

### Comparing `spectrum_fundamentals-0.3.1/spectrum_fundamentals/__init__.py` & `spectrum_fundamentals-0.3.2/spectrum_fundamentals/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Initialize fundamentals."""
 __author__ = "Victor Giurcoiu"
 __email__ = "victor.giurcoiu@tum.de"
-__version__ = "0.3.1"
+__version__ = "0.3.2"
 
 import logging
 import logging.handlers
 import sys
 import time
 
 CONSOLE_LOG_LEVEL = logging.INFO
```

### Comparing `spectrum_fundamentals-0.3.1/spectrum_fundamentals/annotation/annotation.py` & `spectrum_fundamentals-0.3.2/spectrum_fundamentals/annotation/annotation.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.3.1/spectrum_fundamentals/charge.py` & `spectrum_fundamentals-0.3.2/spectrum_fundamentals/charge.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.3.1/spectrum_fundamentals/constants.py` & `spectrum_fundamentals-0.3.2/spectrum_fundamentals/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,25 +199,22 @@
 TRIPLE_CHARGED_MASK = np.tile([0, 0, 1, 0, 0, 1], SEQ_LEN - 1)
 
 
 SHARED_DATA_COLUMNS = ["RAW_FILE", "SCAN_NUMBER"]
 META_DATA_ONLY_COLUMNS = [
     "MODIFIED_SEQUENCE",
     "PRECURSOR_CHARGE",
-    "FRAGMENTATION",
-    "MASS_ANALYZER",
     "MASS",
     "SCAN_EVENT_NUMBER",
     "PRECURSOR_MASS_EXP",
     "SCORE",
     "REVERSE",
-    "RETENTION_TIME",
 ]
 META_DATA_COLUMNS = SHARED_DATA_COLUMNS + META_DATA_ONLY_COLUMNS
-MZML_ONLY_DATA_COLUMNS = ["INTENSITIES", "MZ", "MZ_RANGE"]
+MZML_ONLY_DATA_COLUMNS = ["INTENSITIES", "MZ", "MZ_RANGE", "RETENTION_TIME", "MASS_ANALYZER", "FRAGMENTATION"]
 MZML_DATA_COLUMNS = SHARED_DATA_COLUMNS + MZML_ONLY_DATA_COLUMNS
 
 TMT_MODS = {
     "tmt": "[UNIMOD:737]",
     "tmtpro": "[UNIMOD:2016]",
     "itraq4": "[UNIMOD:214]",
     "itraq8": "[UNIMOD:730]",
```

### Comparing `spectrum_fundamentals-0.3.1/spectrum_fundamentals/fragments.py` & `spectrum_fundamentals-0.3.2/spectrum_fundamentals/fragments.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.3.1/spectrum_fundamentals/metrics/fragments_ratio.py` & `spectrum_fundamentals-0.3.2/spectrum_fundamentals/metrics/fragments_ratio.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.3.1/spectrum_fundamentals/metrics/metric.py` & `spectrum_fundamentals-0.3.2/spectrum_fundamentals/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.3.1/spectrum_fundamentals/metrics/percolator.py` & `spectrum_fundamentals-0.3.2/spectrum_fundamentals/metrics/percolator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import enum
 import hashlib
 import logging
+import re
+import subprocess
 from typing import Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 import scipy.optimize as opt
 import scipy.stats
 from moepy import lowess
@@ -281,19 +283,27 @@
         spec_id_cols = ["RAW_FILE", "SCAN_NUMBER", "MODIFIED_SEQUENCE", "PRECURSOR_CHARGE"]
         if "SCAN_EVENT_NUMBER" in self.metadata.columns:
             spec_id_cols.append("SCAN_EVENT_NUMBER")
         self.metrics_val["SpecId"] = self.metadata[spec_id_cols].apply(Percolator.get_specid, axis=1)
         self.metrics_val["Label"] = self.target_decoy_labels
         self.metrics_val["ScanNr"] = self.metadata[["RAW_FILE", "SCAN_NUMBER"]].apply(Percolator.get_scannr, axis=1)
 
-        # self.metrics_val['ExpMass'] = self.metadata['MASS']
         self.metrics_val["Peptide"] = self.metadata["MODIFIED_SEQUENCE"].apply(lambda x: "_." + x + "._")
-        self.metrics_val["Protein"] = self.metadata[
-            "MODIFIED_SEQUENCE"
-        ]  # we don't need the protein ID to get PSM / peptide results, fill with peptide sequence
+
+        result = subprocess.run(["percolator", "-h"], capture_output=True, text=True)
+        output_lines = result.stderr.splitlines()
+        version_line = output_lines[0].strip()
+        version = version_line.split("version ")[1]
+        version_major = float(re.sub(r"\.[^.]+$", "", version))
+        if version_major >= 3.06:
+            self.metrics_val["Proteins"] = self.metadata[
+                "MODIFIED_SEQUENCE"
+            ]  # we don't need the protein ID to get PSM / peptide results, fill with peptide sequence
+        else:
+            self.metrics_val["Protein"] = self.metadata["MODIFIED_SEQUENCE"]
 
     def apply_lda_and_get_indices_below_fdr(
         self, initial_scoring_feature: str = "spectral_angle", fdr_cutoff: float = 0.01
     ):
         """
         Applies a linear discriminant analysis on the features calculated so far (before retention time alignment) \
         to estimate false discovery rates (FDRs).
@@ -381,15 +391,15 @@
             for i in range(len(fdrs) - 2, -1, -1):
                 qvals[i] = min(qvals[i + 1], fdrs[i])
         return qvals
 
     def _reorder_columns_for_percolator(self):
         all_columns = self.metrics_val.columns
         first_columns = ["SpecId", "Label", "ScanNr"]
-        last_columns = ["Peptide", "Protein"]
+        last_columns = ["Peptide", "Protein"] if "Protein" in all_columns else ["Peptide", "Proteins"]
         mid_columns = list(set(all_columns) - set(first_columns) - set(last_columns))
         new_columns = first_columns + sorted(mid_columns) + last_columns
         self.metrics_val = self.metrics_val[new_columns]
 
     def calc(self):
         """Adds percolator metadata and feature columns to metrics_val based on PSM metadata."""
         self.add_common_features()
```

### Comparing `spectrum_fundamentals-0.3.1/spectrum_fundamentals/metrics/similarity.py` & `spectrum_fundamentals-0.3.2/spectrum_fundamentals/metrics/similarity.py`

 * *Files 0% similar despite different names*

```diff
@@ -413,18 +413,18 @@
         """
         self.metrics_val["spectral_angle"] = SimilarityMetrics.spectral_angle(
             self.true_intensities, self.pred_intensities, 0
         )
         self.metrics_val["pearson_corr"] = SimilarityMetrics.correlation(
             self.true_intensities, self.pred_intensities, 0, "pearson"
         )
-        self.metrics_val["modified_cosine"] = SimilarityMetrics.modified_cosine(
-            self.true_intensities, self.pred_intensities, self.mz, self.mz
-        )
         if all_features:
+            self.metrics_val["modified_cosine"] = SimilarityMetrics.modified_cosine(
+                self.true_intensities, self.pred_intensities, self.mz, self.mz
+            )
             self.metrics_val["spectral_entropy_similarity"] = SimilarityMetrics.spectral_entropy_similarity(
                 self.true_intensities, self.pred_intensities
             )
 
             col_names_spectral_angle = [
                 f"spectral_angle_{amount}_charge" for amount in ["single", "double", "triple"]
             ] + ["spectral_angle_b_ions", "spectral_angle_y_ions"]
```

### Comparing `spectrum_fundamentals-0.3.1/spectrum_fundamentals/mod_string.py` & `spectrum_fundamentals-0.3.2/spectrum_fundamentals/mod_string.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.3.1/PKG-INFO` & `spectrum_fundamentals-0.3.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 Metadata-Version: 2.1
 Name: spectrum-fundamentals
-Version: 0.3.1
+Version: 0.3.2
 Summary: Fundamentals public repo
 Home-page: https://github.com/wilhelm-lab/spectrum_fundamentals
 License: MIT
 Author: WassimG
 Author-email: wassim.gabriel@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: PyYAML (>=5.4.1)
 Requires-Dist: click (>=8.0.0)
 Requires-Dist: joblib (>=1.0.1,<2.0.0)
 Requires-Dist: moepy (>=1.1.4,<2.0.0)
 Requires-Dist: numpy (>=1.24.1,<2.0.0)
 Requires-Dist: pandas (>=1.3.0,<2.0.0)
 Requires-Dist: rich (>=10.3.0)
```

