# Comparing `tmp/spectrum_fundamentals-0.3.1.tar.gz` & `tmp/spectrum_fundamentals-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrum_fundamentals-0.3.1.tar", max compression
+gzip compressed data, was "spectrum_fundamentals-0.4.0.tar", max compression
```

## Comparing `spectrum_fundamentals-0.3.1.tar` & `spectrum_fundamentals-0.4.0.tar`

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
+-rw-r--r--   0        0        0     1073 2023-05-30 12:05:55.696123 spectrum_fundamentals-0.4.0/LICENSE
+-rw-r--r--   0        0        0     2611 2023-05-30 12:05:55.696123 spectrum_fundamentals-0.4.0/README.rst
+-rw-r--r--   0        0        0     2367 2023-05-30 12:05:55.696123 spectrum_fundamentals-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      940 2023-05-30 12:05:55.696123 spectrum_fundamentals-0.4.0/spectrum_fundamentals/__init__.py
+-rw-r--r--   0        0        0      381 2023-05-30 12:05:55.696123 spectrum_fundamentals-0.4.0/spectrum_fundamentals/__main__.py
+-rw-r--r--   0        0        0       29 2023-05-30 12:05:55.696123 spectrum_fundamentals-0.4.0/spectrum_fundamentals/annotation/__init__.py
+-rw-r--r--   0        0        0    11153 2023-05-30 12:05:55.696123 spectrum_fundamentals-0.4.0/spectrum_fundamentals/annotation/annotation.py
+-rw-r--r--   0        0        0     1372 2023-05-30 12:05:55.696123 spectrum_fundamentals-0.4.0/spectrum_fundamentals/charge.py
+-rw-r--r--   0        0        0     7807 2023-05-30 12:05:55.696123 spectrum_fundamentals-0.4.0/spectrum_fundamentals/constants.py
+-rw-r--r--   0        0        0    12452 2023-05-30 12:05:55.696123 spectrum_fundamentals-0.4.0/spectrum_fundamentals/fragments.py
+-rw-r--r--   0        0        0       26 2023-05-30 12:05:55.696123 spectrum_fundamentals-0.4.0/spectrum_fundamentals/metrics/__init__.py
+-rw-r--r--   0        0        0    14554 2023-05-30 12:05:55.696123 spectrum_fundamentals-0.4.0/spectrum_fundamentals/metrics/fragments_ratio.py
+-rw-r--r--   0        0        0     1435 2023-05-30 12:05:55.696123 spectrum_fundamentals-0.4.0/spectrum_fundamentals/metrics/metric.py
+-rw-r--r--   0        0        0    22868 2023-05-30 12:05:55.696123 spectrum_fundamentals-0.4.0/spectrum_fundamentals/metrics/percolator.py
+-rw-r--r--   0        0        0    22390 2023-05-30 12:05:55.696123 spectrum_fundamentals-0.4.0/spectrum_fundamentals/metrics/similarity.py
+-rw-r--r--   0        0        0     9443 2023-05-30 12:05:55.696123 spectrum_fundamentals-0.4.0/spectrum_fundamentals/mod_string.py
+-rw-r--r--   0        0        0        0 2023-05-30 12:05:55.696123 spectrum_fundamentals-0.4.0/spectrum_fundamentals/py.typed
+-rw-r--r--   0        0        0     3705 1970-01-01 00:00:00.000000 spectrum_fundamentals-0.4.0/PKG-INFO
```

### Comparing `spectrum_fundamentals-0.3.1/LICENSE` & `spectrum_fundamentals-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.3.1/README.rst` & `spectrum_fundamentals-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.3.1/pyproject.toml` & `spectrum_fundamentals-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spectrum_fundamentals"
-version = "0.3.1"  # <<COOKIETEMPLE_FORCE_BUMP>>
+version = "0.4.0"  # <<COOKIETEMPLE_FORCE_BUMP>>
 description = "Fundamentals public repo"
 authors = ["WassimG <wassim.gabriel@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/wilhelm-lab/spectrum_fundamentals"
 repository = "https://github.com/wilhelm-lab/spectrum_fundamentals"
 documentation = "https://spectrum_fundamentals.readthedocs.io"
```

### Comparing `spectrum_fundamentals-0.3.1/spectrum_fundamentals/__init__.py` & `spectrum_fundamentals-0.4.0/spectrum_fundamentals/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Initialize fundamentals."""
 __author__ = "Victor Giurcoiu"
 __email__ = "victor.giurcoiu@tum.de"
-__version__ = "0.3.1"
+__version__ = "0.4.0"
 
 import logging
 import logging.handlers
 import sys
 import time
 
 CONSOLE_LOG_LEVEL = logging.INFO
```

### Comparing `spectrum_fundamentals-0.3.1/spectrum_fundamentals/annotation/annotation.py` & `spectrum_fundamentals-0.4.0/spectrum_fundamentals/annotation/annotation.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.3.1/spectrum_fundamentals/charge.py` & `spectrum_fundamentals-0.4.0/spectrum_fundamentals/charge.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.3.1/spectrum_fundamentals/constants.py` & `spectrum_fundamentals-0.4.0/spectrum_fundamentals/constants.py`

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

### Comparing `spectrum_fundamentals-0.3.1/spectrum_fundamentals/fragments.py` & `spectrum_fundamentals-0.4.0/spectrum_fundamentals/fragments.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.3.1/spectrum_fundamentals/metrics/fragments_ratio.py` & `spectrum_fundamentals-0.4.0/spectrum_fundamentals/metrics/fragments_ratio.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.3.1/spectrum_fundamentals/metrics/metric.py` & `spectrum_fundamentals-0.4.0/spectrum_fundamentals/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.3.1/spectrum_fundamentals/metrics/percolator.py` & `spectrum_fundamentals-0.4.0/spectrum_fundamentals/metrics/percolator.py`

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
@@ -54,23 +56,34 @@
         input_type: str,
         pred_intensities: Optional[Union[np.ndarray, scipy.sparse.csr_matrix]] = None,
         true_intensities: Optional[Union[np.ndarray, scipy.sparse.csr_matrix]] = None,
         mz: Optional[Union[np.ndarray, scipy.sparse.csr_matrix]] = None,
         all_features_flag: bool = False,
         regression_method: str = "lowess",
         fdr_cutoff: float = 0.01,
+        percolator_version: Optional[float] = 3.05,
     ):
         """Initialize a Percolator obj."""
         self.metadata = metadata
         self.input_type = input_type
         self.all_features_flag = all_features_flag
         self.regression_method = regression_method
         self.fdr_cutoff = fdr_cutoff
+
+        self._resolve_percolator_compatibility(percolator_version)
         super().__init__(pred_intensities, true_intensities, mz)
 
+    def _resolve_percolator_compatibility(self, percolator_version: Optional[float] = None):
+        if percolator_version is None:
+            result = subprocess.run(["percolator", "-h"], capture_output=True, text=True)
+            version_line = result.stderr.splitlines()[0].strip()
+            version = version_line.split("version ")[1]
+            percolator_version = float(re.sub(r"\.[^.]+$", "", version))
+        self.prot_col_name = "Proteins" if percolator_version >= 3.06 else "Protein"
+
     @staticmethod
     def sample_balanced_over_bins(retention_time_df: pd.DataFrame, sample_size: int = 5000) -> pd.Index:
         """
         Sample balanced over bins.
 
         :param retention_time_df: DataFrame with observed and predicted retention times
         :param sample_size: number of samples
@@ -281,17 +294,17 @@
         spec_id_cols = ["RAW_FILE", "SCAN_NUMBER", "MODIFIED_SEQUENCE", "PRECURSOR_CHARGE"]
         if "SCAN_EVENT_NUMBER" in self.metadata.columns:
             spec_id_cols.append("SCAN_EVENT_NUMBER")
         self.metrics_val["SpecId"] = self.metadata[spec_id_cols].apply(Percolator.get_specid, axis=1)
         self.metrics_val["Label"] = self.target_decoy_labels
         self.metrics_val["ScanNr"] = self.metadata[["RAW_FILE", "SCAN_NUMBER"]].apply(Percolator.get_scannr, axis=1)
 
-        # self.metrics_val['ExpMass'] = self.metadata['MASS']
         self.metrics_val["Peptide"] = self.metadata["MODIFIED_SEQUENCE"].apply(lambda x: "_." + x + "._")
-        self.metrics_val["Protein"] = self.metadata[
+
+        self.metrics_val[self.prot_col_name] = self.metadata[
             "MODIFIED_SEQUENCE"
         ]  # we don't need the protein ID to get PSM / peptide results, fill with peptide sequence
 
     def apply_lda_and_get_indices_below_fdr(
         self, initial_scoring_feature: str = "spectral_angle", fdr_cutoff: float = 0.01
     ):
         """
@@ -381,15 +394,15 @@
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

### Comparing `spectrum_fundamentals-0.3.1/spectrum_fundamentals/metrics/similarity.py` & `spectrum_fundamentals-0.4.0/spectrum_fundamentals/metrics/similarity.py`

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

### Comparing `spectrum_fundamentals-0.3.1/spectrum_fundamentals/mod_string.py` & `spectrum_fundamentals-0.4.0/spectrum_fundamentals/mod_string.py`

 * *Files identical despite different names*

### Comparing `spectrum_fundamentals-0.3.1/PKG-INFO` & `spectrum_fundamentals-0.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 Metadata-Version: 2.1
 Name: spectrum-fundamentals
-Version: 0.3.1
+Version: 0.4.0
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

