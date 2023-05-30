# Comparing `tmp/brainsurf-0.0.1.tar.gz` & `tmp/brainsurf-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainsurf-0.0.1.tar", last modified: Sat Apr 29 03:37:23 2023, max compression
+gzip compressed data, was "brainsurf-0.0.3.tar", last modified: Tue May 30 16:47:13 2023, max compression
```

## Comparing `brainsurf-0.0.1.tar` & `brainsurf-0.0.3.tar`

### file list

```diff
@@ -1,53 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 03:37:22.977708 brainsurf-0.0.1/
--rw-rw-rw-   0        0        0     1098 2023-04-26 06:37:24.000000 brainsurf-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      809 2023-04-29 03:37:22.977708 brainsurf-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1311 2023-04-29 03:33:58.000000 brainsurf-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 03:37:22.785500 brainsurf-0.0.1/brainsurf/
--rw-rw-rw-   0        0        0       70 2023-04-29 03:32:35.000000 brainsurf-0.0.1/brainsurf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 03:37:22.841571 brainsurf-0.0.1/brainsurf/analysis/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:36:01.000000 brainsurf-0.0.1/brainsurf/analysis/__init__.py
--rw-rw-rw-   0        0        0     1378 2023-04-28 15:58:26.000000 brainsurf-0.0.1/brainsurf/analysis/corelation_analysis.py
--rw-rw-rw-   0        0        0     1353 2023-04-28 15:51:19.000000 brainsurf-0.0.1/brainsurf/analysis/power_spectrum.py
--rw-rw-rw-   0        0        0     1755 2023-04-28 15:57:09.000000 brainsurf-0.0.1/brainsurf/analysis/stats_analysis.py
--rw-rw-rw-   0        0        0      493 2023-04-28 15:40:11.000000 brainsurf-0.0.1/brainsurf/analysis/time_frequency.py
--rw-rw-rw-   0        0        0        0 2023-04-26 08:11:03.000000 brainsurf-0.0.1/brainsurf/analysis/wavelet_tranform.py
-drwxrwxrwx   0        0        0        0 2023-04-29 03:37:22.857568 brainsurf-0.0.1/brainsurf/cognitive_analysis_module/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:35:56.000000 brainsurf-0.0.1/brainsurf/cognitive_analysis_module/__init__.py
--rw-rw-rw-   0        0        0        0 2023-04-26 05:50:59.000000 brainsurf-0.0.1/brainsurf/cognitive_analysis_module/cognitive_comparision.py
--rw-rw-rw-   0        0        0     6115 2023-04-26 05:51:01.000000 brainsurf-0.0.1/brainsurf/cognitive_analysis_module/cognitive_indexes.py
-drwxrwxrwx   0        0        0        0 2023-04-29 03:37:22.857568 brainsurf-0.0.1/brainsurf/comparitive_analysis/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:35:51.000000 brainsurf-0.0.1/brainsurf/comparitive_analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 03:37:22.881591 brainsurf-0.0.1/brainsurf/data/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:35:47.000000 brainsurf-0.0.1/brainsurf/data/__init__.py
--rw-rw-rw-   0        0        0      166 2023-04-19 13:04:01.000000 brainsurf-0.0.1/brainsurf/data/csv.py
--rw-rw-rw-   0        0        0     1017 2023-04-26 15:59:05.000000 brainsurf-0.0.1/brainsurf/data/edf.py
--rw-rw-rw-   0        0        0      116 2023-04-20 12:31:52.000000 brainsurf-0.0.1/brainsurf/data/mff.py
--rw-rw-rw-   0        0        0     2916 2023-04-26 05:19:14.000000 brainsurf-0.0.1/brainsurf/data/task2.py
--rw-rw-rw-   0        0        0      116 2023-04-19 13:04:22.000000 brainsurf-0.0.1/brainsurf/data/xlsx.py
-drwxrwxrwx   0        0        0        0 2023-04-29 03:37:22.897625 brainsurf-0.0.1/brainsurf/preprocessing/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:35:43.000000 brainsurf-0.0.1/brainsurf/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     1497 2023-04-26 13:49:07.000000 brainsurf-0.0.1/brainsurf/preprocessing/epoching.py
--rw-rw-rw-   0        0        0      570 2023-04-21 09:48:00.000000 brainsurf-0.0.1/brainsurf/preprocessing/filtering.py
-drwxrwxrwx   0        0        0        0 2023-04-29 03:37:22.905674 brainsurf-0.0.1/brainsurf/utils/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:35:40.000000 brainsurf-0.0.1/brainsurf/utils/__init__.py
--rw-rw-rw-   0        0        0     3208 2023-04-26 14:52:25.000000 brainsurf-0.0.1/brainsurf/utils/data.py
--rw-rw-rw-   0        0        0     1123 2023-04-21 06:09:42.000000 brainsurf-0.0.1/brainsurf/utils/performance_eval.py
-drwxrwxrwx   0        0        0        0 2023-04-29 03:37:22.969692 brainsurf-0.0.1/brainsurf/visualization/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:35:36.000000 brainsurf-0.0.1/brainsurf/visualization/__init__.py
--rw-rw-rw-   0        0        0      305 2023-04-21 06:18:25.000000 brainsurf-0.0.1/brainsurf/visualization/plot_cluster.py
--rw-rw-rw-   0        0        0      570 2023-04-21 06:16:21.000000 brainsurf-0.0.1/brainsurf/visualization/plot_coherence.py
--rw-rw-rw-   0        0        0      490 2023-04-21 06:17:33.000000 brainsurf-0.0.1/brainsurf/visualization/plot_cross-correlation.py
--rw-rw-rw-   0        0        0      243 2023-04-21 09:56:59.000000 brainsurf-0.0.1/brainsurf/visualization/plot_eeg_signal.py
--rw-rw-rw-   0        0        0      310 2023-04-21 06:18:21.000000 brainsurf-0.0.1/brainsurf/visualization/plot_heatmap.py
--rw-rw-rw-   0        0        0     1905 2023-04-26 15:47:58.000000 brainsurf-0.0.1/brainsurf/visualization/plot_power_spectrum.py
--rw-rw-rw-   0        0        0     1224 2023-04-19 14:16:48.000000 brainsurf-0.0.1/brainsurf/visualization/plot_spectogram.py
--rw-rw-rw-   0        0        0     2027 2023-04-19 14:04:56.000000 brainsurf-0.0.1/brainsurf/visualization/plot_time_series.py
--rw-rw-rw-   0        0        0     1417 2023-04-19 14:02:41.000000 brainsurf-0.0.1/brainsurf/visualization/plot_topomap.py
-drwxrwxrwx   0        0        0        0 2023-04-29 03:37:22.817572 brainsurf-0.0.1/brainsurf.egg-info/
--rw-rw-rw-   0        0        0      809 2023-04-29 03:37:22.000000 brainsurf-0.0.1/brainsurf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1406 2023-04-29 03:37:22.000000 brainsurf-0.0.1/brainsurf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 03:37:22.000000 brainsurf-0.0.1/brainsurf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-04-29 03:37:22.000000 brainsurf-0.0.1/brainsurf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-29 03:37:22.000000 brainsurf-0.0.1/brainsurf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 03:37:22.977708 brainsurf-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      977 2023-04-29 03:33:02.000000 brainsurf-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 16:47:13.908710 brainsurf-0.0.3/
+-rw-rw-rw-   0        0        0     1098 2023-04-26 06:37:24.000000 brainsurf-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      809 2023-05-30 16:47:13.906576 brainsurf-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1311 2023-04-29 03:33:58.000000 brainsurf-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 16:47:13.395235 brainsurf-0.0.3/brainsurf/
+-rw-rw-rw-   0        0        0       70 2023-05-30 16:43:57.000000 brainsurf-0.0.3/brainsurf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 16:47:13.516312 brainsurf-0.0.3/brainsurf/analysis/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:36:01.000000 brainsurf-0.0.3/brainsurf/analysis/__init__.py
+-rw-rw-rw-   0        0        0     1386 2023-05-23 17:17:31.000000 brainsurf-0.0.3/brainsurf/analysis/corelation_analysis.py
+-rw-rw-rw-   0        0        0     3601 2023-04-29 05:21:32.000000 brainsurf-0.0.3/brainsurf/analysis/erp_analysis.py
+-rw-rw-rw-   0        0        0     1455 2023-05-21 15:27:09.000000 brainsurf-0.0.3/brainsurf/analysis/find_range.py
+-rw-rw-rw-   0        0        0     1532 2023-05-21 15:56:30.000000 brainsurf-0.0.3/brainsurf/analysis/multi_fractal.py
+-rw-rw-rw-   0        0        0     1367 2023-04-29 04:19:06.000000 brainsurf-0.0.3/brainsurf/analysis/power_spectrum.py
+-rw-rw-rw-   0        0        0     3087 2023-05-21 15:49:59.000000 brainsurf-0.0.3/brainsurf/analysis/stats_analysis.py
+-rw-rw-rw-   0        0        0      493 2023-04-28 15:40:11.000000 brainsurf-0.0.3/brainsurf/analysis/time_frequency.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 08:11:03.000000 brainsurf-0.0.3/brainsurf/analysis/wavelet_transform.py
+drwxrwxrwx   0        0        0        0 2023-05-30 16:47:13.544156 brainsurf-0.0.3/brainsurf/cognitive_analysis_module/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:35:56.000000 brainsurf-0.0.3/brainsurf/cognitive_analysis_module/__init__.py
+-rw-rw-rw-   0        0        0    10182 2023-05-24 17:42:19.000000 brainsurf-0.0.3/brainsurf/cognitive_analysis_module/cognitive_comparision.py
+-rw-rw-rw-   0        0        0     1028 2023-05-23 18:15:54.000000 brainsurf-0.0.3/brainsurf/cognitive_analysis_module/cognitive_indexes.py
+drwxrwxrwx   0        0        0        0 2023-05-30 16:47:13.566799 brainsurf-0.0.3/brainsurf/comparitive_analysis/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:35:51.000000 brainsurf-0.0.3/brainsurf/comparitive_analysis/__init__.py
+-rw-rw-rw-   0        0        0     1307 2023-05-14 16:53:07.000000 brainsurf-0.0.3/brainsurf/comparitive_analysis/meditation_comparision.py
+-rw-rw-rw-   0        0        0     1376 2023-05-23 17:05:32.000000 brainsurf-0.0.3/brainsurf/comparitive_analysis/t_test.py
+drwxrwxrwx   0        0        0        0 2023-05-30 16:47:13.667758 brainsurf-0.0.3/brainsurf/data/
+-rw-rw-rw-   0        0        0        0 2023-05-16 17:35:29.000000 brainsurf-0.0.3/brainsurf/data/__init__.py
+-rw-rw-rw-   0        0        0    21380 2023-05-29 16:47:53.000000 brainsurf-0.0.3/brainsurf/data/comparative_visualize.py
+-rw-rw-rw-   0        0        0      184 2023-05-17 18:40:54.000000 brainsurf-0.0.3/brainsurf/data/csv.py
+-rw-rw-rw-   0        0        0      184 2023-05-17 18:47:03.000000 brainsurf-0.0.3/brainsurf/data/edf.py
+-rw-rw-rw-   0        0        0    11884 2023-05-23 18:39:23.000000 brainsurf-0.0.3/brainsurf/data/eeg_data.py
+-rw-rw-rw-   0        0        0     2915 2023-05-21 15:27:09.000000 brainsurf-0.0.3/brainsurf/data/eeg_data_visualization.py
+-rw-rw-rw-   0        0        0     1237 2023-05-17 18:40:22.000000 brainsurf-0.0.3/brainsurf/data/mff.py
+-rw-rw-rw-   0        0        0      206 2023-05-17 18:42:46.000000 brainsurf-0.0.3/brainsurf/data/xlsx.py
+drwxrwxrwx   0        0        0        0 2023-05-30 16:47:13.740147 brainsurf-0.0.3/brainsurf/machine_learning/
+-rw-rw-rw-   0        0        0        0 2023-05-10 16:44:26.000000 brainsurf-0.0.3/brainsurf/machine_learning/__init__.py
+-rw-rw-rw-   0        0        0      743 2023-05-25 17:14:08.000000 brainsurf-0.0.3/brainsurf/machine_learning/eeg_binary_classification.py
+-rw-rw-rw-   0        0        0      764 2023-05-08 17:36:08.000000 brainsurf-0.0.3/brainsurf/machine_learning/meditative_non_meditative.py
+-rw-rw-rw-   0        0        0     2470 2023-05-10 16:29:13.000000 brainsurf-0.0.3/brainsurf/machine_learning/rnn.py
+-rw-rw-rw-   0        0        0     2428 2023-05-10 16:31:42.000000 brainsurf-0.0.3/brainsurf/machine_learning/rnn2.py
+-rw-rw-rw-   0        0        0     2445 2023-05-10 16:29:42.000000 brainsurf-0.0.3/brainsurf/machine_learning/rnn_module.py
+-rw-rw-rw-   0        0        0     2220 2023-05-08 16:44:59.000000 brainsurf-0.0.3/brainsurf/machine_learning/t2.py
+-rw-rw-rw-   0        0        0     3385 2023-05-08 17:24:37.000000 brainsurf-0.0.3/brainsurf/machine_learning/time_series.py
+drwxrwxrwx   0        0        0        0 2023-05-30 16:47:13.783781 brainsurf-0.0.3/brainsurf/preprocessing/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:35:43.000000 brainsurf-0.0.3/brainsurf/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0      491 2023-05-14 16:45:53.000000 brainsurf-0.0.3/brainsurf/preprocessing/artifact_removal.py
+-rw-rw-rw-   0        0        0     2108 2023-05-10 15:28:37.000000 brainsurf-0.0.3/brainsurf/preprocessing/baseline.py
+-rw-rw-rw-   0        0        0     1137 2023-05-10 15:30:11.000000 brainsurf-0.0.3/brainsurf/preprocessing/epoching.py
+-rw-rw-rw-   0        0        0     4216 2023-05-17 19:24:17.000000 brainsurf-0.0.3/brainsurf/preprocessing/filtering.py
+drwxrwxrwx   0        0        0        0 2023-05-30 16:47:13.805449 brainsurf-0.0.3/brainsurf/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:35:40.000000 brainsurf-0.0.3/brainsurf/utils/__init__.py
+-rw-rw-rw-   0        0        0      943 2023-05-17 20:26:04.000000 brainsurf-0.0.3/brainsurf/utils/data.py
+-rw-rw-rw-   0        0        0      879 2023-04-29 03:52:10.000000 brainsurf-0.0.3/brainsurf/utils/performance_eval.py
+drwxrwxrwx   0        0        0        0 2023-05-30 16:47:13.901580 brainsurf-0.0.3/brainsurf/visualization/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:35:36.000000 brainsurf-0.0.3/brainsurf/visualization/__init__.py
+-rw-rw-rw-   0        0        0      252 2023-04-29 03:44:58.000000 brainsurf-0.0.3/brainsurf/visualization/plot_cluster.py
+-rw-rw-rw-   0        0        0      510 2023-04-29 03:44:56.000000 brainsurf-0.0.3/brainsurf/visualization/plot_coherence.py
+-rw-rw-rw-   0        0        0      420 2023-04-29 03:45:05.000000 brainsurf-0.0.3/brainsurf/visualization/plot_cross-correlation.py
+-rw-rw-rw-   0        0        0      243 2023-05-21 15:27:09.000000 brainsurf-0.0.3/brainsurf/visualization/plot_eeg_signal.py
+-rw-rw-rw-   0        0        0      262 2023-04-29 03:45:13.000000 brainsurf-0.0.3/brainsurf/visualization/plot_heatmap.py
+-rw-rw-rw-   0        0        0     1013 2023-04-29 03:45:23.000000 brainsurf-0.0.3/brainsurf/visualization/plot_power_spectrum.py
+-rw-rw-rw-   0        0        0      465 2023-04-29 03:45:35.000000 brainsurf-0.0.3/brainsurf/visualization/plot_spectogram.py
+-rw-rw-rw-   0        0        0      606 2023-04-29 03:45:46.000000 brainsurf-0.0.3/brainsurf/visualization/plot_time_series.py
+-rw-rw-rw-   0        0        0      623 2023-04-29 03:46:07.000000 brainsurf-0.0.3/brainsurf/visualization/plot_topomap.py
+drwxrwxrwx   0        0        0        0 2023-05-30 16:47:13.432021 brainsurf-0.0.3/brainsurf.egg-info/
+-rw-rw-rw-   0        0        0      809 2023-05-30 16:47:13.000000 brainsurf-0.0.3/brainsurf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2109 2023-05-30 16:47:13.000000 brainsurf-0.0.3/brainsurf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 16:47:13.000000 brainsurf-0.0.3/brainsurf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-05-30 16:47:13.000000 brainsurf-0.0.3/brainsurf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-30 16:47:13.000000 brainsurf-0.0.3/brainsurf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 16:47:13.908710 brainsurf-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      995 2023-05-30 16:43:45.000000 brainsurf-0.0.3/setup.py
```

### Comparing `brainsurf-0.0.1/LICENSE` & `brainsurf-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `brainsurf-0.0.1/PKG-INFO` & `brainsurf-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainsurf
-Version: 0.0.1
+Version: 0.0.3
 Summary: EEG Signal Processing Library
 Home-page: https://github.com/preethihiremath/brainsurf
 Author: preethivhiremath
 Author-email: preethivhiremath.vh@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `brainsurf-0.0.1/README.md` & `brainsurf-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `brainsurf-0.0.1/brainsurf/analysis/corelation_analysis.py` & `brainsurf-0.0.3/brainsurf/analysis/corelation_analysis.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pandas as pd
 import numpy as np
 from scipy.stats import pearsonr, spearmanr
 from scipy.signal import correlate
 import numpy as np
 import statsmodels as st
-from st.tsa.stattools import grangercausalitytests
+# from st.tsa.stattools import grangercausalitytests
 from sklearn.metrics import mutual_info_score
 
 
 def calculate_correlation(data, method='pearson'):
     if method == 'pearson':
         corr_matrix = pearsonr(data)
     elif method == 'spearman':
@@ -25,18 +25,16 @@
     return xcorr, lags
 
 def calculate_phase_sync(data1, data2):
     phase_diff = np.angle(np.exp(1j * (np.angle(np.fft.fft(data1)) - np.angle(np.fft.fft(data2)))))
     return np.abs(np.mean(np.exp(1j * phase_diff)))
 
 
-
-def calculate_granger_causality(x, y, maxlag=10):
-    data = np.column_stack((x, y))
-    results = grangercausalitytests(data, maxlag=maxlag, verbose=False)
-    p_value = results[maxlag][0]['ssr_ftest'][1]
-    return p_value
+# def calculate_granger_causality(x, y, maxlag=10):
+#     data = np.column_stack((x, y))
+#     results = grangercausalitytests(data, maxlag=maxlag, verbose=False)
+#     p_value = results[maxlag][0]['ssr_ftest'][1]
+#     return p_value
 
 def calculate_mutual_information(x, y):
-
     mi = mutual_info_score(x, y)
     return mi
```

### Comparing `brainsurf-0.0.1/brainsurf/analysis/power_spectrum.py` & `brainsurf-0.0.3/brainsurf/analysis/power_spectrum.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from scipy.signal import welch, coherence, correlate
 import astropy as ast 
-from scipy.signal import periodogram , multitaper
+# from scipy.signal import periodogram , multitaper
 
 def psd_fft(data, sfreq, freq_range=(0, 100)):
     n_freqs = int(sfreq/2) + 1
     fft_data = np.fft.rfft(data)
     power_spectrum = np.abs(fft_data)**2 / len(data)
     freqs = np.fft.rfftfreq(len(data), 1.0/sfreq)
     mask = (freqs >= freq_range[0]) & (freqs <= freq_range[1])
@@ -20,21 +20,21 @@
     return freqs, psd
 
 def psd_lombscargle(signal, fs):
     time = np.arange(len(signal))/fs
     frequency, power = ast.timeseries.LombScargle(time, signal).autopower(normalization='psd')
     return frequency, power
 
-def psd_multitaper(signal, fs, nperseg=256, NW=3):
-    f, Pxx = multitaper(signal, fs, nperseg=nperseg, NW=NW, adaptive=True)
-    return f, Pxx.mean(axis=1)
-
-def psd_periodogram(signal, fs, nfft=None):
-    f, Pxx = periodogram(signal, fs, nfft=nfft)
-    return f, Pxx
+# def psd_multitaper(signal, fs, nperseg=256, NW=3):
+#     f, Pxx = multitaper(signal, fs, nperseg=nperseg, NW=NW, adaptive=True)
+#     return f, Pxx.mean(axis=1)
+
+# def psd_periodogram(signal, fs, nfft=None):
+#     f, Pxx = periodogram(signal, fs, nfft=nfft)
+#     return f, Pxx
 
 def calculate_nperseg(data):
     n = len(data)
     if n < 256:
         nperseg = n
     elif n < 2048:
         nperseg = 256
```

### Comparing `brainsurf-0.0.1/brainsurf/utils/performance_eval.py` & `brainsurf-0.0.3/brainsurf/utils/performance_eval.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 import pandas as pd
 import os
 import numpy as np
 
 
 def calculate_mse(y_true, y_pred):
-    """Calculates mean squared error between true and predicted values."""
-    return np.mean((y_true - y_pred) ** 2)
+     return np.mean((y_true - y_pred) ** 2)
 
 def calculate_r_squared(y_true, y_pred):
-    """Calculates R^2 coefficient of determination between true and predicted values."""
     ss_res = np.sum((y_true - y_pred) ** 2)
     ss_tot = np.sum((y_true - np.mean(y_true)) ** 2)
     return 1 - (ss_res / ss_tot)
 
 def k_fold_cross_validation(X, y, model, k):
-    """Performs k-fold cross validation and returns mean validation score."""
     scores = []
     n_samples = len(X)
     fold_size = n_samples // k
     for i in range(k):
         start = i * fold_size
         end = start + fold_size
         X_train = np.concatenate((X[:start], X[end:]))
```

### Comparing `brainsurf-0.0.1/brainsurf/visualization/plot_power_spectrum.py` & `brainsurf-0.0.3/brainsurf/visualization/plot_power_spectrum.py`

 * *Files 25% similar despite different names*

```diff
@@ -25,38 +25,14 @@
     ax.set_xlabel('Frequency (Hz)')
     ax.set_ylabel('Power ($\mu V^2$/Hz)')
     ax.legend()
     plt.show()
 
 
 def welch_power_spectrum(freqs, psd, nperseg=1024):
-    """
-    Calculate the power spectrum of EEG data using the Welch method.
-    
-    Parameters
-    ----------
-    data : array-like, shape (n_channels, n_samples)
-        The EEG data.
-    sfreq : float
-        The sampling frequency of the data, in Hz.
-    nperseg : int
-        The length of each segment for the Welch method (default=256).
-    noverlap : int or None
-        The number of samples to overlap between segments for the Welch method (default=None, which sets noverlap to nperseg // 2).
-    
-    Returns
-    -------
-    freqs : array-like, shape (n_freqs,)
-        The frequency values for the power spectrum.
-    power_spectrum : array-like, shape (n_channels, n_freqs)
-        The power spectrum of the EEG data.
-    """
-    # n_channels, n_samples = data.shape
-    # eeg=data.iloc[:, 1]
-    # freqs, psd = signal.welch(eeg, sfreq, nperseg=nperseg)
     plt.figure()
     plt.plot(freqs, psd)
     plt.xlabel('Frequency (Hz)')
     plt.ylabel('PSD')
     plt.title('Frequency-Domain EEG Signal')
     plt.show()
```

### Comparing `brainsurf-0.0.1/brainsurf.egg-info/PKG-INFO` & `brainsurf-0.0.3/brainsurf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainsurf
-Version: 0.0.1
+Version: 0.0.3
 Summary: EEG Signal Processing Library
 Home-page: https://github.com/preethihiremath/brainsurf
 Author: preethivhiremath
 Author-email: preethivhiremath.vh@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `brainsurf-0.0.1/brainsurf.egg-info/SOURCES.txt` & `brainsurf-0.0.3/brainsurf.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -5,29 +5,46 @@
 brainsurf.egg-info/PKG-INFO
 brainsurf.egg-info/SOURCES.txt
 brainsurf.egg-info/dependency_links.txt
 brainsurf.egg-info/requires.txt
 brainsurf.egg-info/top_level.txt
 brainsurf/analysis/__init__.py
 brainsurf/analysis/corelation_analysis.py
+brainsurf/analysis/erp_analysis.py
+brainsurf/analysis/find_range.py
+brainsurf/analysis/multi_fractal.py
 brainsurf/analysis/power_spectrum.py
 brainsurf/analysis/stats_analysis.py
 brainsurf/analysis/time_frequency.py
-brainsurf/analysis/wavelet_tranform.py
+brainsurf/analysis/wavelet_transform.py
 brainsurf/cognitive_analysis_module/__init__.py
 brainsurf/cognitive_analysis_module/cognitive_comparision.py
 brainsurf/cognitive_analysis_module/cognitive_indexes.py
 brainsurf/comparitive_analysis/__init__.py
+brainsurf/comparitive_analysis/meditation_comparision.py
+brainsurf/comparitive_analysis/t_test.py
 brainsurf/data/__init__.py
+brainsurf/data/comparative_visualize.py
 brainsurf/data/csv.py
 brainsurf/data/edf.py
+brainsurf/data/eeg_data.py
+brainsurf/data/eeg_data_visualization.py
 brainsurf/data/mff.py
-brainsurf/data/task2.py
 brainsurf/data/xlsx.py
+brainsurf/machine_learning/__init__.py
+brainsurf/machine_learning/eeg_binary_classification.py
+brainsurf/machine_learning/meditative_non_meditative.py
+brainsurf/machine_learning/rnn.py
+brainsurf/machine_learning/rnn2.py
+brainsurf/machine_learning/rnn_module.py
+brainsurf/machine_learning/t2.py
+brainsurf/machine_learning/time_series.py
 brainsurf/preprocessing/__init__.py
+brainsurf/preprocessing/artifact_removal.py
+brainsurf/preprocessing/baseline.py
 brainsurf/preprocessing/epoching.py
 brainsurf/preprocessing/filtering.py
 brainsurf/utils/__init__.py
 brainsurf/utils/data.py
 brainsurf/utils/performance_eval.py
 brainsurf/visualization/__init__.py
 brainsurf/visualization/plot_cluster.py
```

### Comparing `brainsurf-0.0.1/setup.py` & `brainsurf-0.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name='brainsurf',
-    version='0.0.1',
+    version='0.0.3',
     description='EEG Signal Processing Library',
     author='preethivhiremath',
     author_email='preethivhiremath.vh@gmail.com',
     url='https://github.com/preethihiremath/brainsurf',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'scipy',
         'matplotlib',
         'mne',
-        'nolds'
+        'pyabf'
+        'nolds',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
```

