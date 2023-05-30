# Comparing `tmp/hubmap-commons-2.1.5.tar.gz` & `tmp/hubmap-commons-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hubmap-commons-2.1.5.tar", last modified: Wed Mar  8 20:36:09 2023, max compression
+gzip compressed data, was "hubmap-commons-2.1.6.tar", last modified: Tue May 30 14:59:25 2023, max compression
```

## Comparing `hubmap-commons-2.1.5.tar` & `hubmap-commons-2.1.6.tar`

### file list

```diff
@@ -1,40 +1,48 @@
-drwxrwxr-x   0 zhy19     (1000) zhy19     (1000)        0 2023-03-08 20:36:09.653150 hubmap-commons-2.1.5/
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)     3354 2023-03-08 20:36:09.653150 hubmap-commons-2.1.5/PKG-INFO
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)     2893 2023-03-08 20:35:24.000000 hubmap-commons-2.1.5/README.md
-drwxrwxr-x   0 zhy19     (1000) zhy19     (1000)        0 2023-03-08 20:36:09.652150 hubmap-commons-2.1.5/hubmap_commons/
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)    15722 2023-03-08 20:35:24.000000 hubmap-commons-2.1.5/hubmap_commons/21f293b0-globus-groups.json
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)     3095 2023-03-08 20:35:24.000000 hubmap-commons-2.1.5/hubmap_commons/21f293b0-process-user.json
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)     3665 2023-03-08 20:35:24.000000 hubmap-commons-2.1.5/hubmap_commons/S3_worker.py
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)     5788 2023-03-08 20:35:24.000000 hubmap-commons-2.1.5/hubmap_commons/activity.py
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)      221 2023-03-08 20:35:24.000000 hubmap-commons-2.1.5/hubmap_commons/autherror.py
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)    12776 2023-03-08 20:35:24.000000 hubmap-commons-2.1.5/hubmap_commons/c4018852-globus-groups.json
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)     3095 2023-03-08 20:35:24.000000 hubmap-commons-2.1.5/hubmap_commons/c4018852-process-user.json
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)    59930 2023-03-08 20:35:24.000000 hubmap-commons-2.1.5/hubmap_commons/entity.py
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)      567 2023-03-08 20:35:24.000000 hubmap-commons-2.1.5/hubmap_commons/exceptions.py
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)     6278 2023-03-08 20:35:24.000000 hubmap-commons-2.1.5/hubmap_commons/file_helper.py
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)     3066 2023-03-08 20:35:24.000000 hubmap-commons-2.1.5/hubmap_commons/globus_file_helper.py
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)    40463 2023-03-08 20:35:24.000000 hubmap-commons-2.1.5/hubmap_commons/hm_auth.py
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)      318 2023-03-08 20:35:24.000000 hubmap-commons-2.1.5/hubmap_commons/hubmap-globus-roles.json
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)    13204 2023-03-08 20:35:24.000000 hubmap-commons-2.1.5/hubmap_commons/hubmap_const.py
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)      471 2023-03-08 20:35:24.000000 hubmap-commons-2.1.5/hubmap_commons/hubmap_error.py
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)     7813 2023-03-08 20:35:24.000000 hubmap-commons-2.1.5/hubmap_commons/metadata.py
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)    14445 2023-03-08 20:35:24.000000 hubmap-commons-2.1.5/hubmap_commons/neo4j_connection.py
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)     1165 2023-03-08 20:35:24.000000 hubmap-commons-2.1.5/hubmap_commons/neo4j_driver.py
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)     1178 2023-03-08 20:35:24.000000 hubmap-commons-2.1.5/hubmap_commons/net_helper.py
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)     2269 2023-03-08 20:35:24.000000 hubmap-commons-2.1.5/hubmap_commons/properties.py
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)    31839 2023-03-08 20:35:24.000000 hubmap-commons-2.1.5/hubmap_commons/provenance.py
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)     5461 2023-03-08 20:35:24.000000 hubmap-commons-2.1.5/hubmap_commons/schema_tools.py
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)     1034 2023-03-08 20:35:24.000000 hubmap-commons-2.1.5/hubmap_commons/singleton_metaclass.py
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)     1681 2023-03-08 20:35:24.000000 hubmap-commons-2.1.5/hubmap_commons/string_helper.py
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)     1112 2023-03-08 20:35:24.000000 hubmap-commons-2.1.5/hubmap_commons/test_helper.py
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)     5728 2023-03-08 20:35:24.000000 hubmap-commons-2.1.5/hubmap_commons/test_ws.py
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)    13275 2023-03-08 20:35:24.000000 hubmap-commons-2.1.5/hubmap_commons/type_client.py
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)     5896 2023-03-08 20:35:24.000000 hubmap-commons-2.1.5/hubmap_commons/uuid_generator.py
-drwxrwxr-x   0 zhy19     (1000) zhy19     (1000)        0 2023-03-08 20:36:09.653150 hubmap-commons-2.1.5/hubmap_commons.egg-info/
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)     3354 2023-03-08 20:36:09.000000 hubmap-commons-2.1.5/hubmap_commons.egg-info/PKG-INFO
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)     1109 2023-03-08 20:36:09.000000 hubmap-commons-2.1.5/hubmap_commons.egg-info/SOURCES.txt
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)        1 2023-03-08 20:36:09.000000 hubmap-commons-2.1.5/hubmap_commons.egg-info/dependency_links.txt
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)      162 2023-03-08 20:36:09.000000 hubmap-commons-2.1.5/hubmap_commons.egg-info/requires.txt
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)       15 2023-03-08 20:36:09.000000 hubmap-commons-2.1.5/hubmap_commons.egg-info/top_level.txt
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)       38 2023-03-08 20:36:09.653150 hubmap-commons-2.1.5/setup.cfg
--rw-rw-r--   0 zhy19     (1000) zhy19     (1000)     1433 2023-03-08 20:35:24.000000 hubmap-commons-2.1.5/setup.py
+drwxr-xr-x   0 zhy19     (1000) zhy19     (1000)        0 2023-05-30 14:59:25.469057 hubmap-commons-2.1.6/
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     3354 2023-05-30 14:59:25.469057 hubmap-commons-2.1.6/PKG-INFO
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     2893 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/README.md
+drwxr-xr-x   0 zhy19     (1000) zhy19     (1000)        0 2023-05-30 14:59:25.465057 hubmap-commons-2.1.6/hubmap_commons/
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)    16182 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/hubmap_commons/21f293b0-globus-groups.json
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     3095 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/hubmap_commons/21f293b0-process-user.json
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     3665 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/hubmap_commons/S3_worker.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     5788 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/hubmap_commons/activity.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)      221 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/hubmap_commons/autherror.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)    12776 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/hubmap_commons/c4018852-globus-groups.json
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     3095 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/hubmap_commons/c4018852-process-user.json
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)    59930 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/hubmap_commons/entity.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)      567 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/hubmap_commons/exceptions.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     6278 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/hubmap_commons/file_helper.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     3066 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/hubmap_commons/globus_file_helper.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)    40463 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/hubmap_commons/hm_auth.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)      318 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/hubmap_commons/hubmap-globus-roles.json
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)    13204 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/hubmap_commons/hubmap_const.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)      471 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/hubmap_commons/hubmap_error.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     7813 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/hubmap_commons/metadata.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)    14445 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/hubmap_commons/neo4j_connection.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     1165 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/hubmap_commons/neo4j_driver.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     1178 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/hubmap_commons/net_helper.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     2269 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/hubmap_commons/properties.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)    31839 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/hubmap_commons/provenance.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     5461 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/hubmap_commons/schema_tools.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     1034 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/hubmap_commons/singleton_metaclass.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     1681 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/hubmap_commons/string_helper.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     1112 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/hubmap_commons/test_helper.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     5728 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/hubmap_commons/test_ws.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)    13275 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/hubmap_commons/type_client.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     5896 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/hubmap_commons/uuid_generator.py
+drwxr-xr-x   0 zhy19     (1000) zhy19     (1000)        0 2023-05-30 14:59:25.466057 hubmap-commons-2.1.6/hubmap_commons.egg-info/
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     3354 2023-05-30 14:59:25.000000 hubmap-commons-2.1.6/hubmap_commons.egg-info/PKG-INFO
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     1311 2023-05-30 14:59:25.000000 hubmap-commons-2.1.6/hubmap_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)        1 2023-05-30 14:59:25.000000 hubmap-commons-2.1.6/hubmap_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)      162 2023-05-30 14:59:25.000000 hubmap-commons-2.1.6/hubmap_commons.egg-info/requires.txt
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)       15 2023-05-30 14:59:25.000000 hubmap-commons-2.1.6/hubmap_commons.egg-info/top_level.txt
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)       38 2023-05-30 14:59:25.469057 hubmap-commons-2.1.6/setup.cfg
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     1433 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/setup.py
+drwxr-xr-x   0 zhy19     (1000) zhy19     (1000)        0 2023-05-30 14:59:25.468057 hubmap-commons-2.1.6/tests/
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)      250 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/tests/test_dummy_type_client.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     2847 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/tests/test_group_write_check.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     3580 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/tests/test_neo4j_connection.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     2119 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/tests/test_provenance.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     6152 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/tests/test_schema_tools.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     1048 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/tests/test_singleton_meta.py
+-rw-r--r--   0 zhy19     (1000) zhy19     (1000)     8065 2023-05-30 14:57:39.000000 hubmap-commons-2.1.6/tests/test_type_client.py
```

### Comparing `hubmap-commons-2.1.5/PKG-INFO` & `hubmap-commons-2.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubmap-commons
-Version: 2.1.5
+Version: 2.1.6
 Summary: The common utilities used by the HuMBAP web services
 Home-page: https://github.com/hubmapconsortium/commons
 Author: HuBMAP Consortium
 Author-email: api-developers@hubmapconsortium.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hubmap-commons-2.1.5/README.md` & `hubmap-commons-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.5/hubmap_commons/21f293b0-globus-groups.json` & `hubmap-commons-2.1.6/hubmap_commons/21f293b0-globus-groups.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.972972972972973%*

 * *Differences: {'insert': "[(36, OrderedDict([('description', 'Users who have write access to the Lurie Childrens "*

 * *           "Hospital Demonstration Project directory'), ('data_provider', True), ('has_subgroups', "*

 * *           "False), ('identity_set_properties', None), ('uuid', "*

 * *           "'f2e660d1-f3fd-11ed-bcea-5b6c9dc23028'), ('group_type', 'regular'), ('name', "*

 * *           "'HuBMAP-Lurie-DP'), ('displayname', 'Lurie Childrens Hospital DP'), ('shortname', 'DP "*

 * *           "- Lurie'), ('generateuuid', True), ('tmc_ […]*

```diff
@@ -450,9 +450,22 @@
         "group_type": "regular",
         "has_subgroups": false,
         "identity_set_properties": null,
         "name": "HuBMAP-JHU-TMC",
         "shortname": "TMC - JHU",
         "tmc_prefix": "JHU",
         "uuid": "c14ba151-547c-11ed-bd9a-0db7472df7d6"
+    },
+    {
+        "data_provider": true,
+        "description": "Users who have write access to the Lurie Childrens Hospital Demonstration Project directory",
+        "displayname": "Lurie Childrens Hospital DP",
+        "generateuuid": true,
+        "group_type": "regular",
+        "has_subgroups": false,
+        "identity_set_properties": null,
+        "name": "HuBMAP-Lurie-DP",
+        "shortname": "DP - Lurie",
+        "tmc_prefix": "LURIE",
+        "uuid": "f2e660d1-f3fd-11ed-bcea-5b6c9dc23028"
     }
 ]
```

### Comparing `hubmap-commons-2.1.5/hubmap_commons/21f293b0-process-user.json` & `hubmap-commons-2.1.6/hubmap_commons/21f293b0-process-user.json`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.5/hubmap_commons/S3_worker.py` & `hubmap-commons-2.1.6/hubmap_commons/S3_worker.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.5/hubmap_commons/activity.py` & `hubmap-commons-2.1.6/hubmap_commons/activity.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.5/hubmap_commons/c4018852-globus-groups.json` & `hubmap-commons-2.1.6/hubmap_commons/c4018852-globus-groups.json`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.5/hubmap_commons/c4018852-process-user.json` & `hubmap-commons-2.1.6/hubmap_commons/c4018852-process-user.json`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.5/hubmap_commons/entity.py` & `hubmap-commons-2.1.6/hubmap_commons/entity.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.5/hubmap_commons/exceptions.py` & `hubmap-commons-2.1.6/hubmap_commons/exceptions.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.5/hubmap_commons/file_helper.py` & `hubmap-commons-2.1.6/hubmap_commons/file_helper.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.5/hubmap_commons/globus_file_helper.py` & `hubmap-commons-2.1.6/hubmap_commons/globus_file_helper.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.5/hubmap_commons/hm_auth.py` & `hubmap-commons-2.1.6/hubmap_commons/hm_auth.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.5/hubmap_commons/hubmap_const.py` & `hubmap-commons-2.1.6/hubmap_commons/hubmap_const.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.5/hubmap_commons/metadata.py` & `hubmap-commons-2.1.6/hubmap_commons/metadata.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.5/hubmap_commons/neo4j_connection.py` & `hubmap-commons-2.1.6/hubmap_commons/neo4j_connection.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.5/hubmap_commons/neo4j_driver.py` & `hubmap-commons-2.1.6/hubmap_commons/neo4j_driver.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.5/hubmap_commons/net_helper.py` & `hubmap-commons-2.1.6/hubmap_commons/net_helper.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.5/hubmap_commons/properties.py` & `hubmap-commons-2.1.6/hubmap_commons/properties.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.5/hubmap_commons/provenance.py` & `hubmap-commons-2.1.6/hubmap_commons/provenance.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.5/hubmap_commons/schema_tools.py` & `hubmap-commons-2.1.6/hubmap_commons/schema_tools.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.5/hubmap_commons/singleton_metaclass.py` & `hubmap-commons-2.1.6/hubmap_commons/singleton_metaclass.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.5/hubmap_commons/string_helper.py` & `hubmap-commons-2.1.6/hubmap_commons/string_helper.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.5/hubmap_commons/test_helper.py` & `hubmap-commons-2.1.6/hubmap_commons/test_helper.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.5/hubmap_commons/test_ws.py` & `hubmap-commons-2.1.6/hubmap_commons/test_ws.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.5/hubmap_commons/type_client.py` & `hubmap-commons-2.1.6/hubmap_commons/type_client.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.5/hubmap_commons/uuid_generator.py` & `hubmap-commons-2.1.6/hubmap_commons/uuid_generator.py`

 * *Files identical despite different names*

### Comparing `hubmap-commons-2.1.5/hubmap_commons.egg-info/PKG-INFO` & `hubmap-commons-2.1.6/hubmap_commons.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hubmap-commons
-Version: 2.1.5
+Version: 2.1.6
 Summary: The common utilities used by the HuMBAP web services
 Home-page: https://github.com/hubmapconsortium/commons
 Author: HuBMAP Consortium
 Author-email: api-developers@hubmapconsortium.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hubmap-commons-2.1.5/hubmap_commons.egg-info/SOURCES.txt` & `hubmap-commons-2.1.6/hubmap_commons.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -28,8 +28,15 @@
 hubmap_commons/test_ws.py
 hubmap_commons/type_client.py
 hubmap_commons/uuid_generator.py
 hubmap_commons.egg-info/PKG-INFO
 hubmap_commons.egg-info/SOURCES.txt
 hubmap_commons.egg-info/dependency_links.txt
 hubmap_commons.egg-info/requires.txt
-hubmap_commons.egg-info/top_level.txt
+hubmap_commons.egg-info/top_level.txt
+tests/test_dummy_type_client.py
+tests/test_group_write_check.py
+tests/test_neo4j_connection.py
+tests/test_provenance.py
+tests/test_schema_tools.py
+tests/test_singleton_meta.py
+tests/test_type_client.py
```

### Comparing `hubmap-commons-2.1.5/setup.py` & `hubmap-commons-2.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="hubmap-commons",
-    version="2.1.5",
+    version="2.1.6",
     author="HuBMAP Consortium",
     author_email="api-developers@hubmapconsortium.org",
     description="The common utilities used by the HuMBAP web services",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hubmapconsortium/commons",
     packages=['hubmap_commons'],
```

