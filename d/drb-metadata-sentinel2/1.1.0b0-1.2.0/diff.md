# Comparing `tmp/drb-metadata-sentinel2-1.1.0b0.tar.gz` & `tmp/drb-metadata-sentinel2-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-metadata-sentinel2-1.1.0b0.tar", last modified: Thu Jan  5 10:19:08 2023, max compression
+gzip compressed data, was "drb-metadata-sentinel2-1.2.0.tar", last modified: Tue May 30 11:55:48 2023, max compression
```

## Comparing `drb-metadata-sentinel2-1.1.0b0.tar` & `drb-metadata-sentinel2-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,27 @@
-drwxrwxrwx   0 juju      (1000) juju      (1000)        0 2023-01-05 10:19:08.156968 drb-metadata-sentinel2-1.1.0b0/
--rwxrwxrwx   0 juju      (1000) juju      (1000)       72 2023-01-05 10:18:31.000000 drb-metadata-sentinel2-1.1.0b0/MANIFEST.in
--rwxrwxrwx   0 juju      (1000) juju      (1000)    11934 2023-01-05 10:19:08.159970 drb-metadata-sentinel2-1.1.0b0/PKG-INFO
--rwxrwxrwx   0 juju      (1000) juju      (1000)    11592 2023-01-04 15:07:10.000000 drb-metadata-sentinel2-1.1.0b0/README.md
-drwxrwxrwx   0 juju      (1000) juju      (1000)        0 2023-01-05 10:19:07.490337 drb-metadata-sentinel2-1.1.0b0/drb/
-drwxrwxrwx   0 juju      (1000) juju      (1000)        0 2023-01-05 10:19:07.495337 drb-metadata-sentinel2-1.1.0b0/drb/addons/
-drwxrwxrwx   0 juju      (1000) juju      (1000)        0 2023-01-05 10:19:07.500891 drb-metadata-sentinel2-1.1.0b0/drb/addons/metadata/
-drwxrwxrwx   0 juju      (1000) juju      (1000)        0 2023-01-05 10:19:08.184599 drb-metadata-sentinel2-1.1.0b0/drb/addons/metadata/sentinel2/
--rwxrwxrwx   0 juju      (1000) juju      (1000)       72 2023-01-05 10:18:31.000000 drb-metadata-sentinel2-1.1.0b0/drb/addons/metadata/sentinel2/__init__.py
--rwxrwxrwx   0 juju      (1000) juju      (1000)      499 2023-01-05 10:19:08.186133 drb-metadata-sentinel2-1.1.0b0/drb/addons/metadata/sentinel2/_version.py
--rwxrwxrwx   0 juju      (1000) juju      (1000)    58413 2023-01-05 10:18:31.000000 drb-metadata-sentinel2-1.1.0b0/drb/addons/metadata/sentinel2/cortex.yml
-drwxrwxrwx   0 juju      (1000) juju      (1000)        0 2023-01-05 10:19:08.118687 drb-metadata-sentinel2-1.1.0b0/drb_metadata_sentinel2.egg-info/
--rwxrwxrwx   0 juju      (1000) juju      (1000)    11934 2023-01-05 10:19:07.000000 drb-metadata-sentinel2-1.1.0b0/drb_metadata_sentinel2.egg-info/PKG-INFO
--rwxrwxrwx   0 juju      (1000) juju      (1000)      474 2023-01-05 10:19:07.000000 drb-metadata-sentinel2-1.1.0b0/drb_metadata_sentinel2.egg-info/SOURCES.txt
--rwxrwxrwx   0 juju      (1000) juju      (1000)        1 2023-01-05 10:19:07.000000 drb-metadata-sentinel2-1.1.0b0/drb_metadata_sentinel2.egg-info/dependency_links.txt
--rwxrwxrwx   0 juju      (1000) juju      (1000)       57 2023-01-05 10:19:07.000000 drb-metadata-sentinel2-1.1.0b0/drb_metadata_sentinel2.egg-info/entry_points.txt
--rwxrwxrwx   0 juju      (1000) juju      (1000)      109 2023-01-05 10:19:07.000000 drb-metadata-sentinel2-1.1.0b0/drb_metadata_sentinel2.egg-info/requires.txt
--rwxrwxrwx   0 juju      (1000) juju      (1000)        4 2023-01-05 10:19:07.000000 drb-metadata-sentinel2-1.1.0b0/drb_metadata_sentinel2.egg-info/top_level.txt
--rwxrwxrwx   0 juju      (1000) juju      (1000)      109 2023-01-05 10:18:31.000000 drb-metadata-sentinel2-1.1.0b0/requirements.txt
--rwxrwxrwx   0 juju      (1000) juju      (1000)      236 2023-01-05 10:19:08.171190 drb-metadata-sentinel2-1.1.0b0/setup.cfg
--rwxrwxrwx   0 juju      (1000) juju      (1000)      996 2023-01-05 10:18:31.000000 drb-metadata-sentinel2-1.1.0b0/setup.py
--rwxrwxrwx   0 juju      (1000) juju      (1000)    81180 2023-01-04 15:07:11.000000 drb-metadata-sentinel2-1.1.0b0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 11:55:48.781870 drb-metadata-sentinel2-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7816 2023-05-17 13:35:23.000000 drb-metadata-sentinel2-1.2.0/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-17 13:35:23.000000 drb-metadata-sentinel2-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    12077 2023-05-30 11:55:48.781870 drb-metadata-sentinel2-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    11592 2023-05-17 13:35:23.000000 drb-metadata-sentinel2-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 11:55:47.753855 drb-metadata-sentinel2-1.2.0/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 11:55:47.753855 drb-metadata-sentinel2-1.2.0/drb/addons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 11:55:47.753855 drb-metadata-sentinel2-1.2.0/drb/addons/metadata/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 11:55:48.981873 drb-metadata-sentinel2-1.2.0/drb/addons/metadata/sentinel2/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-17 13:35:23.000000 drb-metadata-sentinel2-1.2.0/drb/addons/metadata/sentinel2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-30 11:55:48.981873 drb-metadata-sentinel2-1.2.0/drb/addons/metadata/sentinel2/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    58413 2023-05-17 13:35:23.000000 drb-metadata-sentinel2-1.2.0/drb/addons/metadata/sentinel2/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 11:55:48.781870 drb-metadata-sentinel2-1.2.0/drb_metadata_sentinel2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    12077 2023-05-30 11:55:46.000000 drb-metadata-sentinel2-1.2.0/drb_metadata_sentinel2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      579 2023-05-30 11:55:47.000000 drb-metadata-sentinel2-1.2.0/drb_metadata_sentinel2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 11:55:46.000000 drb-metadata-sentinel2-1.2.0/drb_metadata_sentinel2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-05-30 11:55:47.000000 drb-metadata-sentinel2-1.2.0/drb_metadata_sentinel2.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 11:55:46.000000 drb-metadata-sentinel2-1.2.0/drb_metadata_sentinel2.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       87 2023-05-30 11:55:47.000000 drb-metadata-sentinel2-1.2.0/drb_metadata_sentinel2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-30 11:55:47.000000 drb-metadata-sentinel2-1.2.0/drb_metadata_sentinel2.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-17 13:35:23.000000 drb-metadata-sentinel2-1.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-05-17 15:46:23.000000 drb-metadata-sentinel2-1.2.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1044 2023-05-30 11:55:48.981873 drb-metadata-sentinel2-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-05-17 13:35:23.000000 drb-metadata-sentinel2-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 11:55:48.781870 drb-metadata-sentinel2-1.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     6773 2023-05-17 13:35:23.000000 drb-metadata-sentinel2-1.2.0/tests/test_sentinel2_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    81180 2023-05-17 13:35:23.000000 drb-metadata-sentinel2-1.2.0/versioneer.py
```

### Comparing `drb-metadata-sentinel2-1.1.0b0/PKG-INFO` & `drb-metadata-sentinel2-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: drb-metadata-sentinel2
-Version: 1.1.0b0
+Version: 1.2.0
 Summary: Sentinel-2 Product Metadata
-Home-page: https://gitlab.com/drb-python/metadata/add-ons/sentinel-2
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
+License: LGPLv3
+Project-URL: Source, https://gitlab.com/drb-python/add-ons/metadata/add-ons/sentinel-2
 Classifier: Programming Language :: Python :: 3.8
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # DRB Sentinel-2 Metadata AddOn
 This addon allowing to enrich the `Sentinel-2 Product` topic with its metadata
 derivative topics also. 
 
 
 Defined metadata:
```

### Comparing `drb-metadata-sentinel2-1.1.0b0/README.md` & `drb-metadata-sentinel2-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `drb-metadata-sentinel2-1.1.0b0/drb/addons/metadata/sentinel2/cortex.yml` & `drb-metadata-sentinel2-1.2.0/drb/addons/metadata/sentinel2/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-metadata-sentinel2-1.1.0b0/drb_metadata_sentinel2.egg-info/PKG-INFO` & `drb-metadata-sentinel2-1.2.0/drb_metadata_sentinel2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: drb-metadata-sentinel2
-Version: 1.1.0b0
+Version: 1.2.0
 Summary: Sentinel-2 Product Metadata
-Home-page: https://gitlab.com/drb-python/metadata/add-ons/sentinel-2
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
+License: LGPLv3
+Project-URL: Source, https://gitlab.com/drb-python/add-ons/metadata/add-ons/sentinel-2
 Classifier: Programming Language :: Python :: 3.8
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # DRB Sentinel-2 Metadata AddOn
 This addon allowing to enrich the `Sentinel-2 Product` topic with its metadata
 derivative topics also. 
 
 
 Defined metadata:
```

### Comparing `drb-metadata-sentinel2-1.1.0b0/versioneer.py` & `drb-metadata-sentinel2-1.2.0/versioneer.py`

 * *Files identical despite different names*

