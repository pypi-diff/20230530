# Comparing `tmp/brainsurf-1.0.tar.gz` & `tmp/brainsurf-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainsurf-1.0.tar", last modified: Tue May 30 16:57:20 2023, max compression
+gzip compressed data, was "brainsurf-1.0.1.tar", last modified: Tue May 30 17:07:24 2023, max compression
```

## Comparing `brainsurf-1.0.tar` & `brainsurf-1.0.1.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 16:57:20.302756 brainsurf-1.0/
--rw-rw-rw-   0        0        0     1098 2023-04-26 06:37:24.000000 brainsurf-1.0/LICENSE
--rw-rw-rw-   0        0        0     2152 2023-05-30 16:57:20.301759 brainsurf-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1311 2023-04-29 03:33:58.000000 brainsurf-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 16:57:20.088487 brainsurf-1.0/brainsurf/
--rw-rw-rw-   0        0        0       68 2023-05-30 16:57:13.000000 brainsurf-1.0/brainsurf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-30 16:57:20.165185 brainsurf-1.0/brainsurf/analysis/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:36:01.000000 brainsurf-1.0/brainsurf/analysis/__init__.py
--rw-rw-rw-   0        0        0     1386 2023-05-23 17:17:31.000000 brainsurf-1.0/brainsurf/analysis/corelation_analysis.py
--rw-rw-rw-   0        0        0     3601 2023-04-29 05:21:32.000000 brainsurf-1.0/brainsurf/analysis/erp_analysis.py
--rw-rw-rw-   0        0        0     1455 2023-05-21 15:27:09.000000 brainsurf-1.0/brainsurf/analysis/find_range.py
--rw-rw-rw-   0        0        0     1532 2023-05-21 15:56:30.000000 brainsurf-1.0/brainsurf/analysis/multi_fractal.py
--rw-rw-rw-   0        0        0     1367 2023-04-29 04:19:06.000000 brainsurf-1.0/brainsurf/analysis/power_spectrum.py
--rw-rw-rw-   0        0        0     3087 2023-05-21 15:49:59.000000 brainsurf-1.0/brainsurf/analysis/stats_analysis.py
--rw-rw-rw-   0        0        0      493 2023-04-28 15:40:11.000000 brainsurf-1.0/brainsurf/analysis/time_frequency.py
--rw-rw-rw-   0        0        0        0 2023-04-26 08:11:03.000000 brainsurf-1.0/brainsurf/analysis/wavelet_transform.py
-drwxrwxrwx   0        0        0        0 2023-05-30 16:57:20.181324 brainsurf-1.0/brainsurf/cognitive_analysis_module/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:35:56.000000 brainsurf-1.0/brainsurf/cognitive_analysis_module/__init__.py
--rw-rw-rw-   0        0        0    10182 2023-05-24 17:42:19.000000 brainsurf-1.0/brainsurf/cognitive_analysis_module/cognitive_comparision.py
--rw-rw-rw-   0        0        0     1028 2023-05-23 18:15:54.000000 brainsurf-1.0/brainsurf/cognitive_analysis_module/cognitive_indexes.py
-drwxrwxrwx   0        0        0        0 2023-05-30 16:57:20.190892 brainsurf-1.0/brainsurf/comparitive_analysis/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:35:51.000000 brainsurf-1.0/brainsurf/comparitive_analysis/__init__.py
--rw-rw-rw-   0        0        0     1307 2023-05-14 16:53:07.000000 brainsurf-1.0/brainsurf/comparitive_analysis/meditation_comparision.py
--rw-rw-rw-   0        0        0     1376 2023-05-23 17:05:32.000000 brainsurf-1.0/brainsurf/comparitive_analysis/t_test.py
-drwxrwxrwx   0        0        0        0 2023-05-30 16:57:20.225128 brainsurf-1.0/brainsurf/data/
--rw-rw-rw-   0        0        0        0 2023-05-16 17:35:29.000000 brainsurf-1.0/brainsurf/data/__init__.py
--rw-rw-rw-   0        0        0    21380 2023-05-29 16:47:53.000000 brainsurf-1.0/brainsurf/data/comparative_visualize.py
--rw-rw-rw-   0        0        0      184 2023-05-17 18:40:54.000000 brainsurf-1.0/brainsurf/data/csv.py
--rw-rw-rw-   0        0        0      184 2023-05-17 18:47:03.000000 brainsurf-1.0/brainsurf/data/edf.py
--rw-rw-rw-   0        0        0    11884 2023-05-23 18:39:23.000000 brainsurf-1.0/brainsurf/data/eeg_data.py
--rw-rw-rw-   0        0        0     2915 2023-05-21 15:27:09.000000 brainsurf-1.0/brainsurf/data/eeg_data_visualization.py
--rw-rw-rw-   0        0        0     1237 2023-05-17 18:40:22.000000 brainsurf-1.0/brainsurf/data/mff.py
--rw-rw-rw-   0        0        0      206 2023-05-17 18:42:46.000000 brainsurf-1.0/brainsurf/data/xlsx.py
-drwxrwxrwx   0        0        0        0 2023-05-30 16:57:20.246193 brainsurf-1.0/brainsurf/machine_learning/
--rw-rw-rw-   0        0        0        0 2023-05-10 16:44:26.000000 brainsurf-1.0/brainsurf/machine_learning/__init__.py
--rw-rw-rw-   0        0        0      743 2023-05-25 17:14:08.000000 brainsurf-1.0/brainsurf/machine_learning/eeg_binary_classification.py
--rw-rw-rw-   0        0        0      764 2023-05-08 17:36:08.000000 brainsurf-1.0/brainsurf/machine_learning/meditative_non_meditative.py
--rw-rw-rw-   0        0        0     2470 2023-05-10 16:29:13.000000 brainsurf-1.0/brainsurf/machine_learning/rnn.py
--rw-rw-rw-   0        0        0     2428 2023-05-10 16:31:42.000000 brainsurf-1.0/brainsurf/machine_learning/rnn2.py
--rw-rw-rw-   0        0        0     2445 2023-05-10 16:29:42.000000 brainsurf-1.0/brainsurf/machine_learning/rnn_module.py
--rw-rw-rw-   0        0        0     2220 2023-05-08 16:44:59.000000 brainsurf-1.0/brainsurf/machine_learning/t2.py
--rw-rw-rw-   0        0        0     3385 2023-05-08 17:24:37.000000 brainsurf-1.0/brainsurf/machine_learning/time_series.py
-drwxrwxrwx   0        0        0        0 2023-05-30 16:57:20.263683 brainsurf-1.0/brainsurf/preprocessing/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:35:43.000000 brainsurf-1.0/brainsurf/preprocessing/__init__.py
--rw-rw-rw-   0        0        0      491 2023-05-14 16:45:53.000000 brainsurf-1.0/brainsurf/preprocessing/artifact_removal.py
--rw-rw-rw-   0        0        0     2108 2023-05-10 15:28:37.000000 brainsurf-1.0/brainsurf/preprocessing/baseline.py
--rw-rw-rw-   0        0        0     1137 2023-05-10 15:30:11.000000 brainsurf-1.0/brainsurf/preprocessing/epoching.py
--rw-rw-rw-   0        0        0     4216 2023-05-17 19:24:17.000000 brainsurf-1.0/brainsurf/preprocessing/filtering.py
-drwxrwxrwx   0        0        0        0 2023-05-30 16:57:20.270555 brainsurf-1.0/brainsurf/utils/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:35:40.000000 brainsurf-1.0/brainsurf/utils/__init__.py
--rw-rw-rw-   0        0        0      943 2023-05-17 20:26:04.000000 brainsurf-1.0/brainsurf/utils/data.py
--rw-rw-rw-   0        0        0      879 2023-04-29 03:52:10.000000 brainsurf-1.0/brainsurf/utils/performance_eval.py
-drwxrwxrwx   0        0        0        0 2023-05-30 16:57:20.298759 brainsurf-1.0/brainsurf/visualization/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:35:36.000000 brainsurf-1.0/brainsurf/visualization/__init__.py
--rw-rw-rw-   0        0        0      252 2023-04-29 03:44:58.000000 brainsurf-1.0/brainsurf/visualization/plot_cluster.py
--rw-rw-rw-   0        0        0      510 2023-04-29 03:44:56.000000 brainsurf-1.0/brainsurf/visualization/plot_coherence.py
--rw-rw-rw-   0        0        0      420 2023-04-29 03:45:05.000000 brainsurf-1.0/brainsurf/visualization/plot_cross-correlation.py
--rw-rw-rw-   0        0        0      243 2023-05-21 15:27:09.000000 brainsurf-1.0/brainsurf/visualization/plot_eeg_signal.py
--rw-rw-rw-   0        0        0      262 2023-04-29 03:45:13.000000 brainsurf-1.0/brainsurf/visualization/plot_heatmap.py
--rw-rw-rw-   0        0        0     1013 2023-04-29 03:45:23.000000 brainsurf-1.0/brainsurf/visualization/plot_power_spectrum.py
--rw-rw-rw-   0        0        0      465 2023-04-29 03:45:35.000000 brainsurf-1.0/brainsurf/visualization/plot_spectogram.py
--rw-rw-rw-   0        0        0      606 2023-04-29 03:45:46.000000 brainsurf-1.0/brainsurf/visualization/plot_time_series.py
--rw-rw-rw-   0        0        0      623 2023-04-29 03:46:07.000000 brainsurf-1.0/brainsurf/visualization/plot_topomap.py
-drwxrwxrwx   0        0        0        0 2023-05-30 16:57:20.134523 brainsurf-1.0/brainsurf.egg-info/
--rw-rw-rw-   0        0        0     2152 2023-05-30 16:57:19.000000 brainsurf-1.0/brainsurf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2109 2023-05-30 16:57:19.000000 brainsurf-1.0/brainsurf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 16:57:19.000000 brainsurf-1.0/brainsurf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-05-30 16:57:19.000000 brainsurf-1.0/brainsurf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-30 16:57:19.000000 brainsurf-1.0/brainsurf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 16:57:20.303753 brainsurf-1.0/setup.cfg
--rw-rw-rw-   0        0        0     1175 2023-05-30 16:56:59.000000 brainsurf-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 17:07:24.425881 brainsurf-1.0.1/
+-rw-rw-rw-   0        0        0     1098 2023-04-26 06:37:24.000000 brainsurf-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2154 2023-05-30 17:07:24.423886 brainsurf-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1311 2023-04-29 03:33:58.000000 brainsurf-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 17:07:24.257566 brainsurf-1.0.1/brainsurf/
+-rw-rw-rw-   0        0        0       70 2023-05-30 17:07:20.000000 brainsurf-1.0.1/brainsurf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 17:07:24.307839 brainsurf-1.0.1/brainsurf/analysis/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:36:01.000000 brainsurf-1.0.1/brainsurf/analysis/__init__.py
+-rw-rw-rw-   0        0        0     1386 2023-05-23 17:17:31.000000 brainsurf-1.0.1/brainsurf/analysis/corelation_analysis.py
+-rw-rw-rw-   0        0        0     3601 2023-04-29 05:21:32.000000 brainsurf-1.0.1/brainsurf/analysis/erp_analysis.py
+-rw-rw-rw-   0        0        0     1455 2023-05-21 15:27:09.000000 brainsurf-1.0.1/brainsurf/analysis/find_range.py
+-rw-rw-rw-   0        0        0     1532 2023-05-21 15:56:30.000000 brainsurf-1.0.1/brainsurf/analysis/multi_fractal.py
+-rw-rw-rw-   0        0        0     1367 2023-04-29 04:19:06.000000 brainsurf-1.0.1/brainsurf/analysis/power_spectrum.py
+-rw-rw-rw-   0        0        0     3087 2023-05-21 15:49:59.000000 brainsurf-1.0.1/brainsurf/analysis/stats_analysis.py
+-rw-rw-rw-   0        0        0      493 2023-04-28 15:40:11.000000 brainsurf-1.0.1/brainsurf/analysis/time_frequency.py
+-rw-rw-rw-   0        0        0        0 2023-04-26 08:11:03.000000 brainsurf-1.0.1/brainsurf/analysis/wavelet_transform.py
+drwxrwxrwx   0        0        0        0 2023-05-30 17:07:24.316375 brainsurf-1.0.1/brainsurf/cognitive_analysis_module/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:35:56.000000 brainsurf-1.0.1/brainsurf/cognitive_analysis_module/__init__.py
+-rw-rw-rw-   0        0        0    10182 2023-05-24 17:42:19.000000 brainsurf-1.0.1/brainsurf/cognitive_analysis_module/cognitive_comparision.py
+-rw-rw-rw-   0        0        0     1028 2023-05-23 18:15:54.000000 brainsurf-1.0.1/brainsurf/cognitive_analysis_module/cognitive_indexes.py
+drwxrwxrwx   0        0        0        0 2023-05-30 17:07:24.324369 brainsurf-1.0.1/brainsurf/comparitive_analysis/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:35:51.000000 brainsurf-1.0.1/brainsurf/comparitive_analysis/__init__.py
+-rw-rw-rw-   0        0        0     1307 2023-05-14 16:53:07.000000 brainsurf-1.0.1/brainsurf/comparitive_analysis/meditation_comparision.py
+-rw-rw-rw-   0        0        0     1376 2023-05-23 17:05:32.000000 brainsurf-1.0.1/brainsurf/comparitive_analysis/t_test.py
+drwxrwxrwx   0        0        0        0 2023-05-30 17:07:24.348498 brainsurf-1.0.1/brainsurf/data/
+-rw-rw-rw-   0        0        0        0 2023-05-16 17:35:29.000000 brainsurf-1.0.1/brainsurf/data/__init__.py
+-rw-rw-rw-   0        0        0    21380 2023-05-29 16:47:53.000000 brainsurf-1.0.1/brainsurf/data/comparative_visualize.py
+-rw-rw-rw-   0        0        0      184 2023-05-17 18:40:54.000000 brainsurf-1.0.1/brainsurf/data/csv.py
+-rw-rw-rw-   0        0        0      184 2023-05-17 18:47:03.000000 brainsurf-1.0.1/brainsurf/data/edf.py
+-rw-rw-rw-   0        0        0    11884 2023-05-23 18:39:23.000000 brainsurf-1.0.1/brainsurf/data/eeg_data.py
+-rw-rw-rw-   0        0        0     2915 2023-05-21 15:27:09.000000 brainsurf-1.0.1/brainsurf/data/eeg_data_visualization.py
+-rw-rw-rw-   0        0        0     1237 2023-05-17 18:40:22.000000 brainsurf-1.0.1/brainsurf/data/mff.py
+-rw-rw-rw-   0        0        0      206 2023-05-17 18:42:46.000000 brainsurf-1.0.1/brainsurf/data/xlsx.py
+drwxrwxrwx   0        0        0        0 2023-05-30 17:07:24.373558 brainsurf-1.0.1/brainsurf/machine_learning/
+-rw-rw-rw-   0        0        0        0 2023-05-10 16:44:26.000000 brainsurf-1.0.1/brainsurf/machine_learning/__init__.py
+-rw-rw-rw-   0        0        0      743 2023-05-25 17:14:08.000000 brainsurf-1.0.1/brainsurf/machine_learning/eeg_binary_classification.py
+-rw-rw-rw-   0        0        0      764 2023-05-08 17:36:08.000000 brainsurf-1.0.1/brainsurf/machine_learning/meditative_non_meditative.py
+-rw-rw-rw-   0        0        0     2470 2023-05-10 16:29:13.000000 brainsurf-1.0.1/brainsurf/machine_learning/rnn.py
+-rw-rw-rw-   0        0        0     2428 2023-05-10 16:31:42.000000 brainsurf-1.0.1/brainsurf/machine_learning/rnn2.py
+-rw-rw-rw-   0        0        0     2445 2023-05-10 16:29:42.000000 brainsurf-1.0.1/brainsurf/machine_learning/rnn_module.py
+-rw-rw-rw-   0        0        0     2220 2023-05-08 16:44:59.000000 brainsurf-1.0.1/brainsurf/machine_learning/t2.py
+-rw-rw-rw-   0        0        0     3385 2023-05-08 17:24:37.000000 brainsurf-1.0.1/brainsurf/machine_learning/time_series.py
+drwxrwxrwx   0        0        0        0 2023-05-30 17:07:24.386105 brainsurf-1.0.1/brainsurf/preprocessing/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:35:43.000000 brainsurf-1.0.1/brainsurf/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0      491 2023-05-14 16:45:53.000000 brainsurf-1.0.1/brainsurf/preprocessing/artifact_removal.py
+-rw-rw-rw-   0        0        0     2108 2023-05-10 15:28:37.000000 brainsurf-1.0.1/brainsurf/preprocessing/baseline.py
+-rw-rw-rw-   0        0        0     1137 2023-05-10 15:30:11.000000 brainsurf-1.0.1/brainsurf/preprocessing/epoching.py
+-rw-rw-rw-   0        0        0     4216 2023-05-17 19:24:17.000000 brainsurf-1.0.1/brainsurf/preprocessing/filtering.py
+drwxrwxrwx   0        0        0        0 2023-05-30 17:07:24.394672 brainsurf-1.0.1/brainsurf/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:35:40.000000 brainsurf-1.0.1/brainsurf/utils/__init__.py
+-rw-rw-rw-   0        0        0      943 2023-05-17 20:26:04.000000 brainsurf-1.0.1/brainsurf/utils/data.py
+-rw-rw-rw-   0        0        0      879 2023-04-29 03:52:10.000000 brainsurf-1.0.1/brainsurf/utils/performance_eval.py
+drwxrwxrwx   0        0        0        0 2023-05-30 17:07:24.420320 brainsurf-1.0.1/brainsurf/visualization/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:35:36.000000 brainsurf-1.0.1/brainsurf/visualization/__init__.py
+-rw-rw-rw-   0        0        0      252 2023-04-29 03:44:58.000000 brainsurf-1.0.1/brainsurf/visualization/plot_cluster.py
+-rw-rw-rw-   0        0        0      510 2023-04-29 03:44:56.000000 brainsurf-1.0.1/brainsurf/visualization/plot_coherence.py
+-rw-rw-rw-   0        0        0      420 2023-04-29 03:45:05.000000 brainsurf-1.0.1/brainsurf/visualization/plot_cross-correlation.py
+-rw-rw-rw-   0        0        0      243 2023-05-21 15:27:09.000000 brainsurf-1.0.1/brainsurf/visualization/plot_eeg_signal.py
+-rw-rw-rw-   0        0        0      262 2023-04-29 03:45:13.000000 brainsurf-1.0.1/brainsurf/visualization/plot_heatmap.py
+-rw-rw-rw-   0        0        0     1013 2023-04-29 03:45:23.000000 brainsurf-1.0.1/brainsurf/visualization/plot_power_spectrum.py
+-rw-rw-rw-   0        0        0      465 2023-04-29 03:45:35.000000 brainsurf-1.0.1/brainsurf/visualization/plot_spectogram.py
+-rw-rw-rw-   0        0        0      606 2023-04-29 03:45:46.000000 brainsurf-1.0.1/brainsurf/visualization/plot_time_series.py
+-rw-rw-rw-   0        0        0      623 2023-04-29 03:46:07.000000 brainsurf-1.0.1/brainsurf/visualization/plot_topomap.py
+drwxrwxrwx   0        0        0        0 2023-05-30 17:07:24.285246 brainsurf-1.0.1/brainsurf.egg-info/
+-rw-rw-rw-   0        0        0     2154 2023-05-30 17:07:24.000000 brainsurf-1.0.1/brainsurf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2109 2023-05-30 17:07:24.000000 brainsurf-1.0.1/brainsurf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 17:07:24.000000 brainsurf-1.0.1/brainsurf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-05-30 17:07:24.000000 brainsurf-1.0.1/brainsurf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-30 17:07:24.000000 brainsurf-1.0.1/brainsurf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 17:07:24.425881 brainsurf-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1178 2023-05-30 17:07:14.000000 brainsurf-1.0.1/setup.py
```

### Comparing `brainsurf-1.0/LICENSE` & `brainsurf-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `brainsurf-1.0/PKG-INFO` & `brainsurf-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainsurf
-Version: 1.0
+Version: 1.0.1
 Summary: EEG Signal Processing Library
 Home-page: https://github.com/preethihiremath/brainsurf
 Author: preethivhiremath
 Author-email: preethivhiremath.vh@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `brainsurf-1.0/README.md` & `brainsurf-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `brainsurf-1.0/brainsurf/analysis/corelation_analysis.py` & `brainsurf-1.0.1/brainsurf/analysis/corelation_analysis.py`

 * *Files identical despite different names*

### Comparing `brainsurf-1.0/brainsurf/analysis/erp_analysis.py` & `brainsurf-1.0.1/brainsurf/analysis/erp_analysis.py`

 * *Files identical despite different names*

### Comparing `brainsurf-1.0/brainsurf/analysis/find_range.py` & `brainsurf-1.0.1/brainsurf/analysis/find_range.py`

 * *Files identical despite different names*

### Comparing `brainsurf-1.0/brainsurf/analysis/multi_fractal.py` & `brainsurf-1.0.1/brainsurf/analysis/multi_fractal.py`

 * *Files identical despite different names*

### Comparing `brainsurf-1.0/brainsurf/analysis/power_spectrum.py` & `brainsurf-1.0.1/brainsurf/analysis/power_spectrum.py`

 * *Files identical despite different names*

### Comparing `brainsurf-1.0/brainsurf/analysis/stats_analysis.py` & `brainsurf-1.0.1/brainsurf/analysis/stats_analysis.py`

 * *Files identical despite different names*

### Comparing `brainsurf-1.0/brainsurf/cognitive_analysis_module/cognitive_comparision.py` & `brainsurf-1.0.1/brainsurf/cognitive_analysis_module/cognitive_comparision.py`

 * *Files identical despite different names*

### Comparing `brainsurf-1.0/brainsurf/cognitive_analysis_module/cognitive_indexes.py` & `brainsurf-1.0.1/brainsurf/cognitive_analysis_module/cognitive_indexes.py`

 * *Files identical despite different names*

### Comparing `brainsurf-1.0/brainsurf/comparitive_analysis/meditation_comparision.py` & `brainsurf-1.0.1/brainsurf/comparitive_analysis/meditation_comparision.py`

 * *Files identical despite different names*

### Comparing `brainsurf-1.0/brainsurf/comparitive_analysis/t_test.py` & `brainsurf-1.0.1/brainsurf/comparitive_analysis/t_test.py`

 * *Files identical despite different names*

### Comparing `brainsurf-1.0/brainsurf/data/comparative_visualize.py` & `brainsurf-1.0.1/brainsurf/data/comparative_visualize.py`

 * *Files identical despite different names*

### Comparing `brainsurf-1.0/brainsurf/data/eeg_data.py` & `brainsurf-1.0.1/brainsurf/data/eeg_data.py`

 * *Files identical despite different names*

### Comparing `brainsurf-1.0/brainsurf/data/eeg_data_visualization.py` & `brainsurf-1.0.1/brainsurf/data/eeg_data_visualization.py`

 * *Files identical despite different names*

### Comparing `brainsurf-1.0/brainsurf/data/mff.py` & `brainsurf-1.0.1/brainsurf/data/mff.py`

 * *Files identical despite different names*

### Comparing `brainsurf-1.0/brainsurf/machine_learning/eeg_binary_classification.py` & `brainsurf-1.0.1/brainsurf/machine_learning/eeg_binary_classification.py`

 * *Files identical despite different names*

### Comparing `brainsurf-1.0/brainsurf/machine_learning/meditative_non_meditative.py` & `brainsurf-1.0.1/brainsurf/machine_learning/meditative_non_meditative.py`

 * *Files identical despite different names*

### Comparing `brainsurf-1.0/brainsurf/machine_learning/rnn.py` & `brainsurf-1.0.1/brainsurf/machine_learning/rnn.py`

 * *Files identical despite different names*

### Comparing `brainsurf-1.0/brainsurf/machine_learning/rnn2.py` & `brainsurf-1.0.1/brainsurf/machine_learning/rnn2.py`

 * *Files identical despite different names*

### Comparing `brainsurf-1.0/brainsurf/machine_learning/rnn_module.py` & `brainsurf-1.0.1/brainsurf/machine_learning/rnn_module.py`

 * *Files identical despite different names*

### Comparing `brainsurf-1.0/brainsurf/machine_learning/t2.py` & `brainsurf-1.0.1/brainsurf/machine_learning/t2.py`

 * *Files identical despite different names*

### Comparing `brainsurf-1.0/brainsurf/machine_learning/time_series.py` & `brainsurf-1.0.1/brainsurf/machine_learning/time_series.py`

 * *Files identical despite different names*

### Comparing `brainsurf-1.0/brainsurf/preprocessing/baseline.py` & `brainsurf-1.0.1/brainsurf/preprocessing/baseline.py`

 * *Files identical despite different names*

### Comparing `brainsurf-1.0/brainsurf/preprocessing/epoching.py` & `brainsurf-1.0.1/brainsurf/preprocessing/epoching.py`

 * *Files identical despite different names*

### Comparing `brainsurf-1.0/brainsurf/preprocessing/filtering.py` & `brainsurf-1.0.1/brainsurf/preprocessing/filtering.py`

 * *Files identical despite different names*

### Comparing `brainsurf-1.0/brainsurf/utils/data.py` & `brainsurf-1.0.1/brainsurf/utils/data.py`

 * *Files identical despite different names*

### Comparing `brainsurf-1.0/brainsurf/utils/performance_eval.py` & `brainsurf-1.0.1/brainsurf/utils/performance_eval.py`

 * *Files identical despite different names*

### Comparing `brainsurf-1.0/brainsurf/visualization/plot_power_spectrum.py` & `brainsurf-1.0.1/brainsurf/visualization/plot_power_spectrum.py`

 * *Files identical despite different names*

### Comparing `brainsurf-1.0/brainsurf/visualization/plot_time_series.py` & `brainsurf-1.0.1/brainsurf/visualization/plot_time_series.py`

 * *Files identical despite different names*

### Comparing `brainsurf-1.0/brainsurf/visualization/plot_topomap.py` & `brainsurf-1.0.1/brainsurf/visualization/plot_topomap.py`

 * *Files identical despite different names*

### Comparing `brainsurf-1.0/brainsurf.egg-info/PKG-INFO` & `brainsurf-1.0.1/brainsurf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainsurf
-Version: 1.0
+Version: 1.0.1
 Summary: EEG Signal Processing Library
 Home-page: https://github.com/preethihiremath/brainsurf
 Author: preethivhiremath
 Author-email: preethivhiremath.vh@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `brainsurf-1.0/brainsurf.egg-info/SOURCES.txt` & `brainsurf-1.0.1/brainsurf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brainsurf-1.0/setup.py` & `brainsurf-1.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='brainsurf',
-    version='1.0',
+    version='1.0.1',
     description='EEG Signal Processing Library',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='preethivhiremath',
     author_email='preethivhiremath.vh@gmail.com',
     url='https://github.com/preethihiremath/brainsurf',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'scipy',
         'matplotlib',
         'mne',
-        'pyabf'
+        'pyabf',
         'nolds',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'Operating System :: OS Independent',
```

