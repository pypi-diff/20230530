# Comparing `tmp/drb-topic-sentinel2-1.2.1.tar.gz` & `tmp/drb-topic-sentinel2-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-topic-sentinel2-1.2.1.tar", last modified: Wed May 17 15:45:05 2023, max compression
+gzip compressed data, was "drb-topic-sentinel2-1.2.2.tar", last modified: Tue May 30 08:46:17 2023, max compression
```

## Comparing `drb-topic-sentinel2-1.2.1.tar` & `drb-topic-sentinel2-1.2.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 15:45:05.465566 drb-topic-sentinel2-1.2.1/
--rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-19 15:45:26.000000 drb-topic-sentinel2-1.2.1/LICENCE.txt
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6040 2023-05-17 15:45:05.465566 drb-topic-sentinel2-1.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5572 2022-07-25 14:59:39.000000 drb-topic-sentinel2-1.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 15:45:05.441566 drb-topic-sentinel2-1.2.1/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 15:45:05.441566 drb-topic-sentinel2-1.2.1/drb/topics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 15:45:05.465566 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-05-17 15:45:05.465566 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 15:45:05.449566 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/aux/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/aux/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4540 2023-05-17 15:44:28.000000 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/aux/cortex.yml
--rw-rw-rw-   0 root         (0) root         (0)      503 2023-05-17 15:44:28.000000 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 15:45:05.449566 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/pdi/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/pdi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2217 2023-05-17 15:44:28.000000 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/pdi/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 15:45:05.453566 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/pdi/datastrip/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/pdi/datastrip/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5405 2023-05-17 15:44:28.000000 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/pdi/datastrip/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 15:45:05.453566 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/pdi/granule/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/pdi/granule/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5168 2023-05-17 15:44:28.000000 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/pdi/granule/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 15:45:05.453566 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/user/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/user/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3875 2023-05-17 15:44:28.000000 drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/user/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 15:45:05.453566 drb-topic-sentinel2-1.2.1/drb_topic_sentinel2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6040 2023-05-17 15:45:05.000000 drb-topic-sentinel2-1.2.1/drb_topic_sentinel2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      932 2023-05-17 15:45:05.000000 drb-topic-sentinel2-1.2.1/drb_topic_sentinel2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 15:45:05.000000 drb-topic-sentinel2-1.2.1/drb_topic_sentinel2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      268 2023-05-17 15:45:05.000000 drb-topic-sentinel2-1.2.1/drb_topic_sentinel2.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 15:45:04.000000 drb-topic-sentinel2-1.2.1/drb_topic_sentinel2.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       55 2023-05-17 15:45:05.000000 drb-topic-sentinel2-1.2.1/drb_topic_sentinel2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-17 15:45:05.000000 drb-topic-sentinel2-1.2.1/drb_topic_sentinel2.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-16 12:37:11.000000 drb-topic-sentinel2-1.2.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       55 2023-05-16 12:37:11.000000 drb-topic-sentinel2-1.2.1/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1424 2023-05-17 15:45:05.465566 drb-topic-sentinel2-1.2.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-05-16 12:37:11.000000 drb-topic-sentinel2-1.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 15:45:05.453566 drb-topic-sentinel2-1.2.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)      788 2022-07-06 15:33:55.000000 drb-topic-sentinel2-1.2.1/tests/test_sentinel2_topics.py
--rw-rw-rw-   0 root         (0) root         (0)    83607 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.1/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:46:17.842946 drb-topic-sentinel2-1.2.2/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-19 15:45:26.000000 drb-topic-sentinel2-1.2.2/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6040 2023-05-30 08:46:17.842946 drb-topic-sentinel2-1.2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5572 2022-07-25 14:59:39.000000 drb-topic-sentinel2-1.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:46:17.826946 drb-topic-sentinel2-1.2.2/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:46:17.826946 drb-topic-sentinel2-1.2.2/drb/topics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:46:17.846946 drb-topic-sentinel2-1.2.2/drb/topics/sentinel2/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.2/drb/topics/sentinel2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-30 08:46:17.846946 drb-topic-sentinel2-1.2.2/drb/topics/sentinel2/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:46:17.834946 drb-topic-sentinel2-1.2.2/drb/topics/sentinel2/aux/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.2/drb/topics/sentinel2/aux/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4592 2023-05-30 08:45:34.000000 drb-topic-sentinel2-1.2.2/drb/topics/sentinel2/aux/cortex.yml
+-rw-rw-rw-   0 root         (0) root         (0)      503 2023-05-30 08:45:34.000000 drb-topic-sentinel2-1.2.2/drb/topics/sentinel2/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:46:17.838946 drb-topic-sentinel2-1.2.2/drb/topics/sentinel2/pdi/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.2/drb/topics/sentinel2/pdi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2217 2023-05-30 08:45:34.000000 drb-topic-sentinel2-1.2.2/drb/topics/sentinel2/pdi/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:46:17.838946 drb-topic-sentinel2-1.2.2/drb/topics/sentinel2/pdi/datastrip/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.2/drb/topics/sentinel2/pdi/datastrip/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5405 2023-05-30 08:45:34.000000 drb-topic-sentinel2-1.2.2/drb/topics/sentinel2/pdi/datastrip/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:46:17.838946 drb-topic-sentinel2-1.2.2/drb/topics/sentinel2/pdi/granule/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.2/drb/topics/sentinel2/pdi/granule/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5168 2023-05-30 08:45:34.000000 drb-topic-sentinel2-1.2.2/drb/topics/sentinel2/pdi/granule/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:46:17.838946 drb-topic-sentinel2-1.2.2/drb/topics/sentinel2/user/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.2/drb/topics/sentinel2/user/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3875 2023-05-30 08:45:34.000000 drb-topic-sentinel2-1.2.2/drb/topics/sentinel2/user/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:46:17.842946 drb-topic-sentinel2-1.2.2/drb_topic_sentinel2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6040 2023-05-30 08:46:17.000000 drb-topic-sentinel2-1.2.2/drb_topic_sentinel2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      932 2023-05-30 08:46:17.000000 drb-topic-sentinel2-1.2.2/drb_topic_sentinel2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 08:46:17.000000 drb-topic-sentinel2-1.2.2/drb_topic_sentinel2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      268 2023-05-30 08:46:17.000000 drb-topic-sentinel2-1.2.2/drb_topic_sentinel2.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 08:46:17.000000 drb-topic-sentinel2-1.2.2/drb_topic_sentinel2.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       55 2023-05-30 08:46:17.000000 drb-topic-sentinel2-1.2.2/drb_topic_sentinel2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-30 08:46:17.000000 drb-topic-sentinel2-1.2.2/drb_topic_sentinel2.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-05-16 12:37:11.000000 drb-topic-sentinel2-1.2.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       55 2023-05-16 12:37:11.000000 drb-topic-sentinel2-1.2.2/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1424 2023-05-30 08:46:17.846946 drb-topic-sentinel2-1.2.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-05-16 12:37:11.000000 drb-topic-sentinel2-1.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:46:17.842946 drb-topic-sentinel2-1.2.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      788 2022-07-06 15:33:55.000000 drb-topic-sentinel2-1.2.2/tests/test_sentinel2_topics.py
+-rw-rw-rw-   0 root         (0) root         (0)    83607 2023-01-03 10:30:21.000000 drb-topic-sentinel2-1.2.2/versioneer.py
```

### Comparing `drb-topic-sentinel2-1.2.1/LICENCE.txt` & `drb-topic-sentinel2-1.2.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel2-1.2.1/PKG-INFO` & `drb-topic-sentinel2-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drb-topic-sentinel2
-Version: 1.2.1
+Version: 1.2.2
 Summary: Sentinel-2 topic for DRB Python
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: LGPLv3
 Project-URL: Source, https://gitlab.com/drb-python/topics/sentinel2
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `drb-topic-sentinel2-1.2.1/README.md` & `drb-topic-sentinel2-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/aux/cortex.yml` & `drb-topic-sentinel2-1.2.2/drb/topics/sentinel2/aux/cortex.yml`

 * *Files 9% similar despite different names*

```diff
@@ -37,24 +37,26 @@
 ###############################################################################
 # Sentinel-2 AUX ECMWFD
 ###############################################################################
 id: 060054d6-f23e-11ec-b939-0242ac120002
 subClassOf: 0cacd114-0c20-11ed-861d-0242ac120002
 label: Sentinel-2 Auxiliary ECMWFD
 category: CONTAINER
+factory: tar
 signatures:
   - name: S2[AB_]_...._AUX_ECMWFD_...._[0-9]{8}T[0-9]{6}_V[0-9]{8}T[0-9]{6}_[0-9]{8}T[0-9]{6}.TGZ
 ---
 ###############################################################################
 # Sentinel-2 AUX UT1UTC
 ###############################################################################
 id: dc74378e-f23f-11ec-b939-0242ac120002
 subClassOf: 0cacd114-0c20-11ed-861d-0242ac120002
 label: Sentinel-2 Auxiliary UT1UTC
 category: CONTAINER
+factory: tar
 signatures:
   - name: S2[AB_]_...._AUX_UT1UTC_...._[0-9]{8}T[0-9]{6}_V[0-9]{8}T[0-9]{6}_[0-9]{8}T[0-9]{6}.TGZ
 ---
 ###############################################################################
 # Sentinel-2 AUX RESORB & PREORB
 ###############################################################################
 id: 8bc2ca58-0c25-11ed-861d-0242ac120002
@@ -70,24 +72,26 @@
 ###############################################################################
 # Sentinel-2 AUX RESORB
 ###############################################################################
 id: 67c1abf6-f2ee-11ec-b939-0242ac120002
 subClassOf: 8bc2ca58-0c25-11ed-861d-0242ac120002
 label: Sentinel-2 EOF Restituted Orbit File Auxiliary Product
 category: FORMATTING
+factory: xml
 signatures:
   - name: S2(A|B)_...._AUX_RESORB_...._[0-9]{8}T[0-9]{6}_V[0-9]{8}T[0-9]{6}_[0-9]{8}T[0-9]{6}.EOF
 ---
 ###############################################################################
 # Sentinel-2 AUX PREORB
 ###############################################################################
 id: 6d1db586-f2ee-11ec-b939-0242ac120002
 subClassOf: 8bc2ca58-0c25-11ed-861d-0242ac120002
 label: Sentinel-2 EOF Predicted Orbit File Auxiliary Product
 category: FORMATTING
+factory: xml
 signatures:
   - name: S2(A|B)_...._AUX_PREORB_...._[0-9]{8}T[0-9]{6}_V[0-9]{8}T[0-9]{6}_[0-9]{8}T[0-9]{6}.EOF
 ---
 ###############################################################################
 # Sentinel-2 AUX GIP product
 ###############################################################################
 id: 7de4ab0c-fd40-11ec-b939-0242ac120002
```

### Comparing `drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/pdi/cortex.yml` & `drb-topic-sentinel2-1.2.2/drb/topics/sentinel2/pdi/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/pdi/datastrip/cortex.yml` & `drb-topic-sentinel2-1.2.2/drb/topics/sentinel2/pdi/datastrip/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/pdi/granule/cortex.yml` & `drb-topic-sentinel2-1.2.2/drb/topics/sentinel2/pdi/granule/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel2-1.2.1/drb/topics/sentinel2/user/cortex.yml` & `drb-topic-sentinel2-1.2.2/drb/topics/sentinel2/user/cortex.yml`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel2-1.2.1/drb_topic_sentinel2.egg-info/PKG-INFO` & `drb-topic-sentinel2-1.2.2/drb_topic_sentinel2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drb-topic-sentinel2
-Version: 1.2.1
+Version: 1.2.2
 Summary: Sentinel-2 topic for DRB Python
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
 License: LGPLv3
 Project-URL: Source, https://gitlab.com/drb-python/topics/sentinel2
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `drb-topic-sentinel2-1.2.1/drb_topic_sentinel2.egg-info/SOURCES.txt` & `drb-topic-sentinel2-1.2.2/drb_topic_sentinel2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel2-1.2.1/setup.cfg` & `drb-topic-sentinel2-1.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel2-1.2.1/tests/test_sentinel2_topics.py` & `drb-topic-sentinel2-1.2.2/tests/test_sentinel2_topics.py`

 * *Files identical despite different names*

### Comparing `drb-topic-sentinel2-1.2.1/versioneer.py` & `drb-topic-sentinel2-1.2.2/versioneer.py`

 * *Files identical despite different names*

