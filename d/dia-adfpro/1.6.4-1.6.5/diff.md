# Comparing `tmp/dia-adfpro-1.6.4.tar.gz` & `tmp/dia-adfpro-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dia-adfpro-1.6.4.tar", last modified: Mon May 29 15:06:50 2023, max compression
+gzip compressed data, was "dia-adfpro-1.6.5.tar", last modified: Tue May 30 12:04:22 2023, max compression
```

## Comparing `dia-adfpro-1.6.4.tar` & `dia-adfpro-1.6.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 15:06:49.993913 dia-adfpro-1.6.4/
--rw-rw-rw-   0        0        0     1089 2023-05-18 08:28:18.000000 dia-adfpro-1.6.4/LICENSE.txt
--rw-rw-rw-   0        0        0       17 2023-05-18 08:28:18.000000 dia-adfpro-1.6.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1046 2023-05-29 15:06:49.994913 dia-adfpro-1.6.4/PKG-INFO
--rw-rw-rw-   0        0        0      685 2021-02-11 11:49:55.000000 dia-adfpro-1.6.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 15:06:49.639890 dia-adfpro-1.6.4/dia_adfpro.egg-info/
--rw-rw-rw-   0        0        0     1046 2023-05-29 15:06:49.000000 dia-adfpro-1.6.4/dia_adfpro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      959 2023-05-29 15:06:49.000000 dia-adfpro-1.6.4/dia_adfpro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 15:06:49.000000 dia-adfpro-1.6.4/dia_adfpro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-29 15:06:49.000000 dia-adfpro-1.6.4/dia_adfpro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-29 15:06:49.000000 dia-adfpro-1.6.4/dia_adfpro.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-29 15:06:49.643886 dia-adfpro-1.6.4/diaadfpro/
--rw-rw-rw-   0        0        0      295 2023-05-29 15:06:01.000000 dia-adfpro-1.6.4/diaadfpro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:06:49.841902 dia-adfpro-1.6.4/diaadfpro/adfpro/
--rw-rw-rw-   0        0        0      270 2022-08-01 06:46:08.000000 dia-adfpro-1.6.4/diaadfpro/adfpro/__init__.py
--rw-rw-rw-   0        0        0    10059 2023-05-18 08:28:18.000000 dia-adfpro-1.6.4/diaadfpro/adfpro/classify.py
--rw-rw-rw-   0        0        0    13958 2023-05-26 14:18:50.000000 dia-adfpro-1.6.4/diaadfpro/adfpro/configuration.py
--rw-rw-rw-   0        0        0     3268 2022-10-24 07:17:27.000000 dia-adfpro-1.6.4/diaadfpro/adfpro/constants.py
--rw-rw-rw-   0        0        0     1334 2022-08-01 06:46:08.000000 dia-adfpro-1.6.4/diaadfpro/adfpro/explain.py
--rw-rw-rw-   0        0        0    31018 2023-05-29 15:05:41.000000 dia-adfpro-1.6.4/diaadfpro/adfpro/feature_extract.py
--rw-rw-rw-   0        0        0    16597 2023-03-27 10:16:17.000000 dia-adfpro-1.6.4/diaadfpro/adfpro/feature_extractors.py
--rw-rw-rw-   0        0        0    10096 2022-08-01 06:46:08.000000 dia-adfpro-1.6.4/diaadfpro/adfpro/golden.py
--rw-rw-rw-   0        0        0    14313 2023-04-28 12:40:42.000000 dia-adfpro-1.6.4/diaadfpro/adfpro/model.py
--rw-rw-rw-   0        0        0     7455 2022-10-24 07:17:27.000000 dia-adfpro-1.6.4/diaadfpro/adfpro/offload.py
--rw-rw-rw-   0        0        0     7607 2023-04-28 12:40:42.000000 dia-adfpro-1.6.4/diaadfpro/adfpro/train.py
--rw-rw-rw-   0        0        0    54884 2023-05-18 08:28:18.000000 dia-adfpro-1.6.4/diaadfpro/adfpro/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:06:49.991914 dia-adfpro-1.6.4/diaadfpro/adfpro_ui/
--rw-rw-rw-   0        0        0      268 2022-08-01 06:46:08.000000 dia-adfpro-1.6.4/diaadfpro/adfpro_ui/__init__.py
--rw-rw-rw-   0        0        0     4014 2023-05-29 15:06:01.000000 dia-adfpro-1.6.4/diaadfpro/adfpro_ui/constants.py
--rw-rw-rw-   0        0        0     6149 2022-08-02 08:08:38.000000 dia-adfpro-1.6.4/diaadfpro/adfpro_ui/ui_anomaly_plots.py
--rw-rw-rw-   0        0        0    11741 2022-10-24 07:17:27.000000 dia-adfpro-1.6.4/diaadfpro/adfpro_ui/ui_app.py
--rw-rw-rw-   0        0        0    20412 2022-10-24 07:17:27.000000 dia-adfpro-1.6.4/diaadfpro/adfpro_ui/ui_components.py
--rw-rw-rw-   0        0        0     1167 2021-09-23 15:24:24.000000 dia-adfpro-1.6.4/diaadfpro/adfpro_ui/ui_env_cfg.py
--rw-rw-rw-   0        0        0     1243 2022-08-01 06:46:08.000000 dia-adfpro-1.6.4/diaadfpro/adfpro_ui/ui_env_cfg.sample.py
--rw-rw-rw-   0        0        0     3677 2022-08-02 08:08:38.000000 dia-adfpro-1.6.4/diaadfpro/adfpro_ui/ui_ohlc_plots.py
--rw-rw-rw-   0        0        0     6925 2022-10-24 07:17:27.000000 dia-adfpro-1.6.4/diaadfpro/adfpro_ui/ui_retrain.py
--rw-rw-rw-   0        0        0    10252 2022-08-02 08:08:38.000000 dia-adfpro-1.6.4/diaadfpro/adfpro_ui/ui_summary_table.py
--rw-rw-rw-   0        0        0      115 2023-05-29 15:06:49.996911 dia-adfpro-1.6.4/setup.cfg
--rw-rw-rw-   0        0        0     1239 2023-05-18 08:28:18.000000 dia-adfpro-1.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 12:04:22.057431 dia-adfpro-1.6.5/
+-rw-rw-rw-   0        0        0     1089 2023-05-18 08:28:18.000000 dia-adfpro-1.6.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       17 2023-05-18 08:28:18.000000 dia-adfpro-1.6.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1046 2023-05-30 12:04:22.058423 dia-adfpro-1.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0      685 2021-02-11 11:49:55.000000 dia-adfpro-1.6.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 12:04:21.715392 dia-adfpro-1.6.5/dia_adfpro.egg-info/
+-rw-rw-rw-   0        0        0     1046 2023-05-30 12:04:21.000000 dia-adfpro-1.6.5/dia_adfpro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      959 2023-05-30 12:04:21.000000 dia-adfpro-1.6.5/dia_adfpro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 12:04:21.000000 dia-adfpro-1.6.5/dia_adfpro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-30 12:04:21.000000 dia-adfpro-1.6.5/dia_adfpro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-30 12:04:21.000000 dia-adfpro-1.6.5/dia_adfpro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 12:04:21.717398 dia-adfpro-1.6.5/diaadfpro/
+-rw-rw-rw-   0        0        0      295 2023-05-30 12:03:55.000000 dia-adfpro-1.6.5/diaadfpro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 12:04:21.910416 dia-adfpro-1.6.5/diaadfpro/adfpro/
+-rw-rw-rw-   0        0        0      270 2022-08-01 06:46:08.000000 dia-adfpro-1.6.5/diaadfpro/adfpro/__init__.py
+-rw-rw-rw-   0        0        0    10059 2023-05-18 08:28:18.000000 dia-adfpro-1.6.5/diaadfpro/adfpro/classify.py
+-rw-rw-rw-   0        0        0    13958 2023-05-26 14:18:50.000000 dia-adfpro-1.6.5/diaadfpro/adfpro/configuration.py
+-rw-rw-rw-   0        0        0     3268 2022-10-24 07:17:27.000000 dia-adfpro-1.6.5/diaadfpro/adfpro/constants.py
+-rw-rw-rw-   0        0        0     1334 2022-08-01 06:46:08.000000 dia-adfpro-1.6.5/diaadfpro/adfpro/explain.py
+-rw-rw-rw-   0        0        0    31088 2023-05-30 11:55:47.000000 dia-adfpro-1.6.5/diaadfpro/adfpro/feature_extract.py
+-rw-rw-rw-   0        0        0    16597 2023-03-27 10:16:17.000000 dia-adfpro-1.6.5/diaadfpro/adfpro/feature_extractors.py
+-rw-rw-rw-   0        0        0    10096 2022-08-01 06:46:08.000000 dia-adfpro-1.6.5/diaadfpro/adfpro/golden.py
+-rw-rw-rw-   0        0        0    14313 2023-04-28 12:40:42.000000 dia-adfpro-1.6.5/diaadfpro/adfpro/model.py
+-rw-rw-rw-   0        0        0     7455 2022-10-24 07:17:27.000000 dia-adfpro-1.6.5/diaadfpro/adfpro/offload.py
+-rw-rw-rw-   0        0        0     7607 2023-04-28 12:40:42.000000 dia-adfpro-1.6.5/diaadfpro/adfpro/train.py
+-rw-rw-rw-   0        0        0    54884 2023-05-18 08:28:18.000000 dia-adfpro-1.6.5/diaadfpro/adfpro/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-30 12:04:22.055427 dia-adfpro-1.6.5/diaadfpro/adfpro_ui/
+-rw-rw-rw-   0        0        0      268 2022-08-01 06:46:08.000000 dia-adfpro-1.6.5/diaadfpro/adfpro_ui/__init__.py
+-rw-rw-rw-   0        0        0     4014 2023-05-30 12:03:46.000000 dia-adfpro-1.6.5/diaadfpro/adfpro_ui/constants.py
+-rw-rw-rw-   0        0        0     6149 2022-08-02 08:08:38.000000 dia-adfpro-1.6.5/diaadfpro/adfpro_ui/ui_anomaly_plots.py
+-rw-rw-rw-   0        0        0    11741 2022-10-24 07:17:27.000000 dia-adfpro-1.6.5/diaadfpro/adfpro_ui/ui_app.py
+-rw-rw-rw-   0        0        0    20412 2022-10-24 07:17:27.000000 dia-adfpro-1.6.5/diaadfpro/adfpro_ui/ui_components.py
+-rw-rw-rw-   0        0        0     1167 2021-09-23 15:24:24.000000 dia-adfpro-1.6.5/diaadfpro/adfpro_ui/ui_env_cfg.py
+-rw-rw-rw-   0        0        0     1243 2022-08-01 06:46:08.000000 dia-adfpro-1.6.5/diaadfpro/adfpro_ui/ui_env_cfg.sample.py
+-rw-rw-rw-   0        0        0     3677 2022-08-02 08:08:38.000000 dia-adfpro-1.6.5/diaadfpro/adfpro_ui/ui_ohlc_plots.py
+-rw-rw-rw-   0        0        0     6925 2022-10-24 07:17:27.000000 dia-adfpro-1.6.5/diaadfpro/adfpro_ui/ui_retrain.py
+-rw-rw-rw-   0        0        0    10252 2022-08-02 08:08:38.000000 dia-adfpro-1.6.5/diaadfpro/adfpro_ui/ui_summary_table.py
+-rw-rw-rw-   0        0        0      115 2023-05-30 12:04:22.065421 dia-adfpro-1.6.5/setup.cfg
+-rw-rw-rw-   0        0        0     1239 2023-05-18 08:28:18.000000 dia-adfpro-1.6.5/setup.py
```

### Comparing `dia-adfpro-1.6.4/LICENSE.txt` & `dia-adfpro-1.6.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.4/PKG-INFO` & `dia-adfpro-1.6.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dia-adfpro
-Version: 1.6.4
+Version: 1.6.5
 Summary: A Python application for anomaly detection
 Home-page: https://github.com/EliLillyCo/MQIT_DIA_ADFPRO
 Author: Francesco Gabbanini, Manjunath Bagewadi, Henson Tauro
 Author-email: fgabbanini@yahoo.it
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `dia-adfpro-1.6.4/README.md` & `dia-adfpro-1.6.5/README.md`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.4/dia_adfpro.egg-info/PKG-INFO` & `dia-adfpro-1.6.5/dia_adfpro.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dia-adfpro
-Version: 1.6.4
+Version: 1.6.5
 Summary: A Python application for anomaly detection
 Home-page: https://github.com/EliLillyCo/MQIT_DIA_ADFPRO
 Author: Francesco Gabbanini, Manjunath Bagewadi, Henson Tauro
 Author-email: fgabbanini@yahoo.it
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `dia-adfpro-1.6.4/dia_adfpro.egg-info/SOURCES.txt` & `dia-adfpro-1.6.5/dia_adfpro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.4/diaadfpro/adfpro/classify.py` & `dia-adfpro-1.6.5/diaadfpro/adfpro/classify.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.4/diaadfpro/adfpro/configuration.py` & `dia-adfpro-1.6.5/diaadfpro/adfpro/configuration.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.4/diaadfpro/adfpro/constants.py` & `dia-adfpro-1.6.5/diaadfpro/adfpro/constants.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.4/diaadfpro/adfpro/explain.py` & `dia-adfpro-1.6.5/diaadfpro/adfpro/explain.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.4/diaadfpro/adfpro/feature_extract.py` & `dia-adfpro-1.6.5/diaadfpro/adfpro/feature_extract.py`

 * *Files 0% similar despite different names*

```diff
@@ -453,16 +453,16 @@
 def reset_time_interval_start(start_ts, end_ts, max_ti_len_hrs):
     new_start_ts = start_ts
     diff = end_ts - new_start_ts
     if diff.total_seconds() > max_ti_len_hrs * 3600:
         new_start_ts = end_ts - timedelta(hours=max_ti_len_hrs)
         logger.warning("Time interval duration exceeds limit ({} hrs). Risk of overloading PI server.".format(
             max_ti_len_hrs))
-        logger.warning("RE-SETTING INTERVAL START TO {}.".format(str(start_ts)))
-        logger.warning("NEW TIME INTERVAL IS: ({}, {})".format(start_ts, end_ts))
+        logger.warning("RE-SETTING INTERVAL START TO {}.".format(str(new_start_ts)))
+        logger.warning("NEW TIME INTERVAL IS: ({}, {})".format(new_start_ts, end_ts))
     return new_start_ts
 
 def main(argv):
     if len(argv) < 1:
         logger.error("Not enough input arguments")
         sys.exit(1)
 
@@ -629,14 +629,15 @@
                 logger.error("Details: {}".format(e))
 
         if 'dump csv' in cfg_dict:
             p = pathlib.Path(cfg_dict['dump csv'], cmp_name + '.csv')
             logger.info("Dump features to csv file ({})".format(str(p)))
             df_feat.to_csv(p)
 
+        exit_codes.append(FeatureExtractExitCodes.NO_ERRORS)
         logger.info("===Component {} completed".format(cmp_name))
         tsecs = round(time.time() - start_cmp_calc, 2)
         logger.info(f"===Time: {tsecs}s (includes writing if enabled).")
     logger.info(">>> Feature calculation completed for all components in configuration file <<<")
     logger.info(">>> Count of exit codes <<<")
     logger.info(f">>> Total: {len(exit_codes)}")
     c = Counter(exit_codes)
```

### Comparing `dia-adfpro-1.6.4/diaadfpro/adfpro/feature_extractors.py` & `dia-adfpro-1.6.5/diaadfpro/adfpro/feature_extractors.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.4/diaadfpro/adfpro/golden.py` & `dia-adfpro-1.6.5/diaadfpro/adfpro/golden.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.4/diaadfpro/adfpro/model.py` & `dia-adfpro-1.6.5/diaadfpro/adfpro/model.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.4/diaadfpro/adfpro/offload.py` & `dia-adfpro-1.6.5/diaadfpro/adfpro/offload.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.4/diaadfpro/adfpro/train.py` & `dia-adfpro-1.6.5/diaadfpro/adfpro/train.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.4/diaadfpro/adfpro/utils.py` & `dia-adfpro-1.6.5/diaadfpro/adfpro/utils.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.4/diaadfpro/adfpro_ui/constants.py` & `dia-adfpro-1.6.5/diaadfpro/adfpro_ui/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
             Manjunath C Bagewadi <bagewadi_manjunath_c@lilly.com>, 
             Henson Tauro <tauro_henson@lilly.com> 
             (MQ IDS - Data Integration and Analytics)
 License:    MIT
 """
 
 class ADFPCUI:
-    REPORT_VERSION = "1.6.4 (2023-05-29)"
+    REPORT_VERSION = "1.6.5 (2023-05-30)"
 
     #use for html id's
     ID_REFRESH = "btn-refresh"                                       #Refresh tab1
     ID_LATESTFETCH = "lbl-latestfetch"                               # latestfetch tab1
     ID_SUMMARY_TBL_CONTAINER = "div-summary-tbl-container"
     
     RETRAIN_YML = "/mnt/py/cfg.jobs/temp_retrain_job.yml"
```

### Comparing `dia-adfpro-1.6.4/diaadfpro/adfpro_ui/ui_anomaly_plots.py` & `dia-adfpro-1.6.5/diaadfpro/adfpro_ui/ui_anomaly_plots.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.4/diaadfpro/adfpro_ui/ui_app.py` & `dia-adfpro-1.6.5/diaadfpro/adfpro_ui/ui_app.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.4/diaadfpro/adfpro_ui/ui_components.py` & `dia-adfpro-1.6.5/diaadfpro/adfpro_ui/ui_components.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.4/diaadfpro/adfpro_ui/ui_env_cfg.py` & `dia-adfpro-1.6.5/diaadfpro/adfpro_ui/ui_env_cfg.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.4/diaadfpro/adfpro_ui/ui_env_cfg.sample.py` & `dia-adfpro-1.6.5/diaadfpro/adfpro_ui/ui_env_cfg.sample.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.4/diaadfpro/adfpro_ui/ui_ohlc_plots.py` & `dia-adfpro-1.6.5/diaadfpro/adfpro_ui/ui_ohlc_plots.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.4/diaadfpro/adfpro_ui/ui_retrain.py` & `dia-adfpro-1.6.5/diaadfpro/adfpro_ui/ui_retrain.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.4/diaadfpro/adfpro_ui/ui_summary_table.py` & `dia-adfpro-1.6.5/diaadfpro/adfpro_ui/ui_summary_table.py`

 * *Files identical despite different names*

### Comparing `dia-adfpro-1.6.4/setup.py` & `dia-adfpro-1.6.5/setup.py`

 * *Files identical despite different names*

