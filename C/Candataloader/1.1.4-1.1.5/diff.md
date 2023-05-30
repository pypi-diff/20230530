# Comparing `tmp/Candataloader-1.1.4.tar.gz` & `tmp/Candataloader-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Candataloader-1.1.4.tar", last modified: Sat May 27 09:28:40 2023, max compression
+gzip compressed data, was "dist/Candataloader-1.1.5.tar", last modified: Tue May 30 13:09:12 2023, max compression
```

## Comparing `Candataloader-1.1.4.tar` & `Candataloader-1.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-05-27 09:28:40.000000 Candataloader-1.1.4/
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)     1729 2023-05-25 12:52:06.000000 Candataloader-1.1.4/README.md
-drwxr-xr-x   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-05-27 09:28:40.000000 Candataloader-1.1.4/Candataloader/
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-05-23 03:31:46.000000 Candataloader-1.1.4/Candataloader/__init__.py
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)     1441 2023-05-27 09:25:37.000000 Candataloader-1.1.4/Candataloader/download.py
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)       38 2023-05-27 09:28:40.000000 Candataloader-1.1.4/setup.cfg
-drwxr-xr-x   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-05-27 09:28:40.000000 Candataloader-1.1.4/Candataloader.egg-info/
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)        1 2023-05-27 09:28:40.000000 Candataloader-1.1.4/Candataloader.egg-info/dependency_links.txt
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      218 2023-05-27 09:28:40.000000 Candataloader-1.1.4/Candataloader.egg-info/SOURCES.txt
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)       23 2023-05-27 09:28:40.000000 Candataloader-1.1.4/Candataloader.egg-info/top_level.txt
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      227 2023-05-27 09:28:40.000000 Candataloader-1.1.4/Candataloader.egg-info/PKG-INFO
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      299 2023-05-27 09:25:43.000000 Candataloader-1.1.4/setup.py
--rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      227 2023-05-27 09:28:40.000000 Candataloader-1.1.4/PKG-INFO
+drwxr-xr-x   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-05-30 13:09:12.000000 Candataloader-1.1.5/
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)     1729 2023-05-25 12:52:06.000000 Candataloader-1.1.5/README.md
+drwxr-xr-x   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-05-30 13:09:12.000000 Candataloader-1.1.5/Candataloader/
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-05-23 03:31:46.000000 Candataloader-1.1.5/Candataloader/__init__.py
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)     1441 2023-05-30 13:08:02.000000 Candataloader-1.1.5/Candataloader/download.py
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)       38 2023-05-30 13:09:12.000000 Candataloader-1.1.5/setup.cfg
+drwxr-xr-x   0 iec_phatphong  (1014) iec_phatphong  (1014)        0 2023-05-30 13:09:12.000000 Candataloader-1.1.5/Candataloader.egg-info/
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)        1 2023-05-30 13:09:12.000000 Candataloader-1.1.5/Candataloader.egg-info/dependency_links.txt
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      218 2023-05-30 13:09:12.000000 Candataloader-1.1.5/Candataloader.egg-info/SOURCES.txt
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)       23 2023-05-30 13:09:12.000000 Candataloader-1.1.5/Candataloader.egg-info/top_level.txt
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      227 2023-05-30 13:09:12.000000 Candataloader-1.1.5/Candataloader.egg-info/PKG-INFO
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      299 2023-05-30 13:08:09.000000 Candataloader-1.1.5/setup.py
+-rw-r--r--   0 iec_phatphong  (1014) iec_phatphong  (1014)      227 2023-05-30 13:09:12.000000 Candataloader-1.1.5/PKG-INFO
```

### Comparing `Candataloader-1.1.4/README.md` & `Candataloader-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `Candataloader-1.1.4/Candataloader/download.py` & `Candataloader-1.1.5/Candataloader/download.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 import requests
 
 def download_dataset(dataset_name):
     dataset_mapping = {
-        'Survival': 'https://ceca-203-205-29-5.ngrok-free.app/Survival Analysis Dataset for automobile IDS.csv',
-        'SynCAN': 'https://ceca-203-205-29-5.ngrok-free.app/SynCAN.csv',
-        'ROAD': 'https://ceca-203-205-29-5.ngrok-free.app/ROAD.csv',
-        'Car Hacking': 'https://ceca-203-205-29-5.ngrok-free.app/Car Hacking.csv',
-        'OTIDS': 'https://ceca-203-205-29-5.ngrok-free.app/OTIDS.csv',
-        'Automotive': 'https://ceca-203-205-29-5.ngrok-free.app/autoCAN_Prototype.csv',
+        'Survival': 'https://39a2-203-205-29-5.ngrok-free.app/Survival Analysis Dataset for automobile IDS.csv',
+        'SynCAN': 'https://39a2-203-205-29-5.ngrok-free.app/SynCAN.csv',
+        'ROAD': 'https://39a2-203-205-29-5.ngrok-free.app/ROAD.csv',
+        'Car Hacking': 'https://39a2-203-205-29-5.ngrok-free.app/Car Hacking.csv',
+        'OTIDS': 'https://39a2-203-205-29-5.ngrok-free.app/OTIDS.csv',
+        'Automotive': 'https://39a2-203-205-29-5.ngrok-free.app/autoCAN_Prototype.csv',
     }
 
     if dataset_name not in dataset_mapping:
         print(f"Dataset '{dataset_name}' is not available for download.")
         return
 
     url = dataset_mapping[dataset_name]
```

