# Comparing `tmp/autovf-0.0.1.tar.gz` & `tmp/autovf-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autovf-0.0.1.tar", last modified: Tue May 30 14:15:17 2023, max compression
+gzip compressed data, was "/Users/cabukela/Documents/open-source/autovf/dist/.tmp-helinl3s/autovf-0.0.2.tar", last modified: Tue May 30 14:38:02 2023, max compression
```

## Comparing `autovf-0.0.1.tar` & `autovf-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)        0 2023-05-30 14:15:17.299487 autovf-0.0.1/
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)    11356 2023-05-30 14:11:45.000000 autovf-0.0.1/LICENSE
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     5821 2023-05-30 14:15:17.299758 autovf-0.0.1/PKG-INFO
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     5487 2023-05-30 14:11:45.000000 autovf-0.0.1/README.md
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)      386 2023-05-30 14:15:17.304767 autovf-0.0.1/setup.cfg
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     1073 2023-05-30 14:11:45.000000 autovf-0.0.1/setup.py
-drwxr-xr-x   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)        0 2023-05-30 14:15:17.169990 autovf-0.0.1/src/
-drwxr-xr-x   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)        0 2023-05-30 14:15:17.255071 autovf-0.0.1/src/autovf/
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)       51 2023-05-30 14:11:45.000000 autovf-0.0.1/src/autovf/__init__.py
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)      319 2023-05-30 14:11:45.000000 autovf-0.0.1/src/autovf/api.py
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)    12114 2023-05-30 14:11:45.000000 autovf-0.0.1/src/autovf/autovf.py
-drwxr-xr-x   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)        0 2023-05-30 14:15:17.283167 autovf-0.0.1/src/autovf/cli/
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)      305 2023-05-30 14:11:45.000000 autovf-0.0.1/src/autovf/cli/__init__.py
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)      994 2023-05-30 14:11:45.000000 autovf-0.0.1/src/autovf/cli/autovf.py
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     1300 2023-05-30 14:11:45.000000 autovf-0.0.1/src/autovf/cli/predict.py
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     1658 2023-05-30 14:11:45.000000 autovf-0.0.1/src/autovf/cli/serve.py
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     4174 2023-05-30 14:11:45.000000 autovf-0.0.1/src/autovf/cli/train.py
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     1297 2023-05-30 14:11:45.000000 autovf-0.0.1/src/autovf/enums.py
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)      225 2023-05-30 14:11:45.000000 autovf-0.0.1/src/autovf/logger.py
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     2934 2023-05-30 14:11:45.000000 autovf-0.0.1/src/autovf/metrics.py
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     1326 2023-05-30 14:11:45.000000 autovf-0.0.1/src/autovf/params.py
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     4547 2023-05-30 14:11:45.000000 autovf-0.0.1/src/autovf/predict.py
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)      459 2023-05-30 14:11:45.000000 autovf-0.0.1/src/autovf/schemas.py
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)    13961 2023-05-30 14:11:45.000000 autovf-0.0.1/src/autovf/utils.py
-drwxr-xr-x   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)        0 2023-05-30 14:15:17.266014 autovf-0.0.1/src/autovf.egg-info/
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     5821 2023-05-30 14:15:17.000000 autovf-0.0.1/src/autovf.egg-info/PKG-INFO
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)      578 2023-05-30 14:15:17.000000 autovf-0.0.1/src/autovf.egg-info/SOURCES.txt
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)        1 2023-05-30 14:15:17.000000 autovf-0.0.1/src/autovf.egg-info/dependency_links.txt
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)       50 2023-05-30 14:15:17.000000 autovf-0.0.1/src/autovf.egg-info/entry_points.txt
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)      187 2023-05-30 14:15:17.000000 autovf-0.0.1/src/autovf.egg-info/requires.txt
--rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)        7 2023-05-30 14:15:17.000000 autovf-0.0.1/src/autovf.egg-info/top_level.txt
+drwxr-xr-x   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)        0 2023-05-30 14:38:02.000000 autovf-0.0.2/
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)    11356 2023-05-30 14:11:45.000000 autovf-0.0.2/LICENSE
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     5821 2023-05-30 14:38:02.000000 autovf-0.0.2/PKG-INFO
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     5487 2023-05-30 14:11:45.000000 autovf-0.0.2/README.md
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)      386 2023-05-30 14:38:02.000000 autovf-0.0.2/setup.cfg
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     1073 2023-05-30 14:34:26.000000 autovf-0.0.2/setup.py
+drwxr-xr-x   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)        0 2023-05-30 14:38:02.000000 autovf-0.0.2/src/
+drwxr-xr-x   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)        0 2023-05-30 14:38:02.000000 autovf-0.0.2/src/autovf/
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)       51 2023-05-30 14:37:39.000000 autovf-0.0.2/src/autovf/__init__.py
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)      319 2023-05-30 14:11:45.000000 autovf-0.0.2/src/autovf/api.py
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)    12114 2023-05-30 14:11:45.000000 autovf-0.0.2/src/autovf/autovf.py
+drwxr-xr-x   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)        0 2023-05-30 14:38:02.000000 autovf-0.0.2/src/autovf/cli/
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)      305 2023-05-30 14:11:45.000000 autovf-0.0.2/src/autovf/cli/__init__.py
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)      994 2023-05-30 14:11:45.000000 autovf-0.0.2/src/autovf/cli/autovf.py
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     1300 2023-05-30 14:11:45.000000 autovf-0.0.2/src/autovf/cli/predict.py
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     1658 2023-05-30 14:11:45.000000 autovf-0.0.2/src/autovf/cli/serve.py
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     4174 2023-05-30 14:11:45.000000 autovf-0.0.2/src/autovf/cli/train.py
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     1297 2023-05-30 14:11:45.000000 autovf-0.0.2/src/autovf/enums.py
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)      225 2023-05-30 14:11:45.000000 autovf-0.0.2/src/autovf/logger.py
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     2934 2023-05-30 14:11:45.000000 autovf-0.0.2/src/autovf/metrics.py
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     1326 2023-05-30 14:11:45.000000 autovf-0.0.2/src/autovf/params.py
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     4547 2023-05-30 14:11:45.000000 autovf-0.0.2/src/autovf/predict.py
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)      459 2023-05-30 14:11:45.000000 autovf-0.0.2/src/autovf/schemas.py
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)    13961 2023-05-30 14:11:45.000000 autovf-0.0.2/src/autovf/utils.py
+drwxr-xr-x   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)        0 2023-05-30 14:38:02.000000 autovf-0.0.2/src/autovf.egg-info/
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)     5821 2023-05-30 14:38:02.000000 autovf-0.0.2/src/autovf.egg-info/PKG-INFO
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)      578 2023-05-30 14:38:02.000000 autovf-0.0.2/src/autovf.egg-info/SOURCES.txt
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)        1 2023-05-30 14:38:02.000000 autovf-0.0.2/src/autovf.egg-info/dependency_links.txt
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)       50 2023-05-30 14:38:02.000000 autovf-0.0.2/src/autovf.egg-info/entry_points.txt
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)      187 2023-05-30 14:38:02.000000 autovf-0.0.2/src/autovf.egg-info/requires.txt
+-rw-r--r--   0 cabukela (315871821) VF-ROOT\Domain Users (653490579)        7 2023-05-30 14:38:02.000000 autovf-0.0.2/src/autovf.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `autovf-0.0.1/LICENSE` & `autovf-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autovf-0.0.1/PKG-INFO` & `autovf-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autovf
-Version: 0.0.1
+Version: 0.0.2
 Summary: autovf: tuning xgboost with optuna
 Home-page: https://github.com/alicabukel/autovf
 Author: Ali Cabukel
 Author-email: alicabukel@proton.me
 License: Apache 2.0
 Platform: linux
 Platform: unix
```

### Comparing `autovf-0.0.1/README.md` & `autovf-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `autovf-0.0.1/setup.py` & `autovf-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 INSTALL_REQUIRES = [
     "fastapi==0.70.0",
     "numpy==1.21.3",
     "optuna==2.10.0",
     "pyarrow==6.0.0",
     "pydantic==1.8.2",
-    "joblib==1.1.0",
+    "joblib==1.1.1",
     "pandas==1.3.4",
     "scikit-learn==1.0.1",
     "uvicorn==0.15.0",
     "xgboost==1.5.0",
     "google-cloud-aiplatform==1.25.0",
 ]
```

### Comparing `autovf-0.0.1/src/autovf/autovf.py` & `autovf-0.0.2/src/autovf/autovf.py`

 * *Files identical despite different names*

### Comparing `autovf-0.0.1/src/autovf/cli/autovf.py` & `autovf-0.0.2/src/autovf/cli/autovf.py`

 * *Files identical despite different names*

### Comparing `autovf-0.0.1/src/autovf/cli/predict.py` & `autovf-0.0.2/src/autovf/cli/predict.py`

 * *Files identical despite different names*

### Comparing `autovf-0.0.1/src/autovf/cli/serve.py` & `autovf-0.0.2/src/autovf/cli/serve.py`

 * *Files identical despite different names*

### Comparing `autovf-0.0.1/src/autovf/cli/train.py` & `autovf-0.0.2/src/autovf/cli/train.py`

 * *Files identical despite different names*

### Comparing `autovf-0.0.1/src/autovf/enums.py` & `autovf-0.0.2/src/autovf/enums.py`

 * *Files identical despite different names*

### Comparing `autovf-0.0.1/src/autovf/metrics.py` & `autovf-0.0.2/src/autovf/metrics.py`

 * *Files identical despite different names*

### Comparing `autovf-0.0.1/src/autovf/params.py` & `autovf-0.0.2/src/autovf/params.py`

 * *Files identical despite different names*

### Comparing `autovf-0.0.1/src/autovf/predict.py` & `autovf-0.0.2/src/autovf/predict.py`

 * *Files identical despite different names*

### Comparing `autovf-0.0.1/src/autovf/utils.py` & `autovf-0.0.2/src/autovf/utils.py`

 * *Files identical despite different names*

### Comparing `autovf-0.0.1/src/autovf.egg-info/PKG-INFO` & `autovf-0.0.2/src/autovf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autovf
-Version: 0.0.1
+Version: 0.0.2
 Summary: autovf: tuning xgboost with optuna
 Home-page: https://github.com/alicabukel/autovf
 Author: Ali Cabukel
 Author-email: alicabukel@proton.me
 License: Apache 2.0
 Platform: linux
 Platform: unix
```

### Comparing `autovf-0.0.1/src/autovf.egg-info/SOURCES.txt` & `autovf-0.0.2/src/autovf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

