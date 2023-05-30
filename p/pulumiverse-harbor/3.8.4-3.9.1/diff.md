# Comparing `tmp/pulumiverse_harbor-3.8.4.tar.gz` & `tmp/pulumiverse_harbor-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_harbor-3.8.4.tar", last modified: Tue Apr  4 16:42:05 2023, max compression
+gzip compressed data, was "pulumiverse_harbor-3.9.1.tar", last modified: Tue May 30 00:26:44 2023, max compression
```

## Comparing `pulumiverse_harbor-3.8.4.tar` & `pulumiverse_harbor-3.9.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:42:05.450245 pulumiverse_harbor-3.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-04 16:42:05.450245 pulumiverse_harbor-3.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:42:05.446245 pulumiverse_harbor-3.8.4/pulumiverse_harbor/
--rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/pulumiverse_harbor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12397 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/pulumiverse_harbor/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/pulumiverse_harbor/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:42:05.450245 pulumiverse_harbor-3.8.4/pulumiverse_harbor/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/pulumiverse_harbor/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/pulumiverse_harbor/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    42516 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/pulumiverse_harbor/config_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    14192 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/pulumiverse_harbor/config_email.py
--rw-r--r--   0 runner    (1001) docker     (123)    10713 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/pulumiverse_harbor/config_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/pulumiverse_harbor/garbage_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/pulumiverse_harbor/get_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/pulumiverse_harbor/get_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/pulumiverse_harbor/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    15948 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/pulumiverse_harbor/immutable_tag_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/pulumiverse_harbor/interrogation_services.py
--rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/pulumiverse_harbor/label.py
--rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/pulumiverse_harbor/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29919 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/pulumiverse_harbor/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    13597 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/pulumiverse_harbor/project_member_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/pulumiverse_harbor/project_member_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    24576 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/pulumiverse_harbor/project_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/pulumiverse_harbor/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/pulumiverse_harbor/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/pulumiverse_harbor/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15487 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/pulumiverse_harbor/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    24011 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/pulumiverse_harbor/replication.py
--rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/pulumiverse_harbor/retention_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    22423 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/pulumiverse_harbor/robot_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/pulumiverse_harbor/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)    12154 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/pulumiverse_harbor/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 16:42:05.450245 pulumiverse_harbor-3.8.4/pulumiverse_harbor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/pulumiverse_harbor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/pulumiverse_harbor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/pulumiverse_harbor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/pulumiverse_harbor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/pulumiverse_harbor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/pulumiverse_harbor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 16:42:05.450245 pulumiverse_harbor-3.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-04 16:42:05.000000 pulumiverse_harbor-3.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:26:44.507643 pulumiverse_harbor-3.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-30 00:26:44.507643 pulumiverse_harbor-3.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:26:44.507643 pulumiverse_harbor-3.9.1/pulumiverse_harbor/
+-rw-r--r--   0 runner    (1001) docker     (123)     4281 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12397 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:26:44.507643 pulumiverse_harbor-3.9.1/pulumiverse_harbor/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42516 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/config_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14192 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/config_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10713 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/config_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/garbage_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/get_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15948 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/immutable_tag_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/interrogation_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9893 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29919 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13597 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/project_member_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/project_member_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24576 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/project_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15487 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24011 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/replication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/retention_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22423 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/robot_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12154 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 00:26:44.507643 pulumiverse_harbor-3.9.1/pulumiverse_harbor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/pulumiverse_harbor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 00:26:44.507643 pulumiverse_harbor-3.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-30 00:26:44.000000 pulumiverse_harbor-3.9.1/setup.py
```

### Comparing `pulumiverse_harbor-3.8.4/PKG-INFO` & `pulumiverse_harbor-3.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse_harbor
-Version: 3.8.4
+Version: 3.9.1
 Summary: A Pulumi package for creating and managing Harbor resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-harbor
 Keywords: pulumi harbor category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumiverse_harbor-3.8.4/README.md` & `pulumiverse_harbor-3.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.8.4/pulumiverse_harbor/__init__.py` & `pulumiverse_harbor-3.9.1/pulumiverse_harbor/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.8.4/pulumiverse_harbor/_inputs.py` & `pulumiverse_harbor-3.9.1/pulumiverse_harbor/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.8.4/pulumiverse_harbor/_utilities.py` & `pulumiverse_harbor-3.9.1/pulumiverse_harbor/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.8.4/pulumiverse_harbor/config/vars.py` & `pulumiverse_harbor-3.9.1/pulumiverse_harbor/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.8.4/pulumiverse_harbor/config_auth.py` & `pulumiverse_harbor-3.9.1/pulumiverse_harbor/config_auth.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.8.4/pulumiverse_harbor/config_email.py` & `pulumiverse_harbor-3.9.1/pulumiverse_harbor/config_email.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.8.4/pulumiverse_harbor/config_system.py` & `pulumiverse_harbor-3.9.1/pulumiverse_harbor/config_system.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.8.4/pulumiverse_harbor/garbage_collection.py` & `pulumiverse_harbor-3.9.1/pulumiverse_harbor/garbage_collection.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.8.4/pulumiverse_harbor/get_project.py` & `pulumiverse_harbor-3.9.1/pulumiverse_harbor/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.8.4/pulumiverse_harbor/get_registry.py` & `pulumiverse_harbor-3.9.1/pulumiverse_harbor/get_registry.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.8.4/pulumiverse_harbor/group.py` & `pulumiverse_harbor-3.9.1/pulumiverse_harbor/group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.8.4/pulumiverse_harbor/immutable_tag_rule.py` & `pulumiverse_harbor-3.9.1/pulumiverse_harbor/immutable_tag_rule.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.8.4/pulumiverse_harbor/interrogation_services.py` & `pulumiverse_harbor-3.9.1/pulumiverse_harbor/interrogation_services.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.8.4/pulumiverse_harbor/label.py` & `pulumiverse_harbor-3.9.1/pulumiverse_harbor/label.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.8.4/pulumiverse_harbor/outputs.py` & `pulumiverse_harbor-3.9.1/pulumiverse_harbor/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.8.4/pulumiverse_harbor/project.py` & `pulumiverse_harbor-3.9.1/pulumiverse_harbor/project.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.8.4/pulumiverse_harbor/project_member_group.py` & `pulumiverse_harbor-3.9.1/pulumiverse_harbor/project_member_group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.8.4/pulumiverse_harbor/project_member_user.py` & `pulumiverse_harbor-3.9.1/pulumiverse_harbor/project_member_user.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.8.4/pulumiverse_harbor/project_webhook.py` & `pulumiverse_harbor-3.9.1/pulumiverse_harbor/project_webhook.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.8.4/pulumiverse_harbor/provider.py` & `pulumiverse_harbor-3.9.1/pulumiverse_harbor/provider.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.8.4/pulumiverse_harbor/registry.py` & `pulumiverse_harbor-3.9.1/pulumiverse_harbor/registry.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.8.4/pulumiverse_harbor/replication.py` & `pulumiverse_harbor-3.9.1/pulumiverse_harbor/replication.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.8.4/pulumiverse_harbor/retention_policy.py` & `pulumiverse_harbor-3.9.1/pulumiverse_harbor/retention_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.8.4/pulumiverse_harbor/robot_account.py` & `pulumiverse_harbor-3.9.1/pulumiverse_harbor/robot_account.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.8.4/pulumiverse_harbor/tasks.py` & `pulumiverse_harbor-3.9.1/pulumiverse_harbor/tasks.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.8.4/pulumiverse_harbor/user.py` & `pulumiverse_harbor-3.9.1/pulumiverse_harbor/user.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.8.4/pulumiverse_harbor.egg-info/PKG-INFO` & `pulumiverse_harbor-3.9.1/pulumiverse_harbor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse-harbor
-Version: 3.8.4
+Version: 3.9.1
 Summary: A Pulumi package for creating and managing Harbor resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-harbor
 Keywords: pulumi harbor category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumiverse_harbor-3.8.4/pulumiverse_harbor.egg-info/SOURCES.txt` & `pulumiverse_harbor-3.9.1/pulumiverse_harbor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumiverse_harbor-3.8.4/setup.py` & `pulumiverse_harbor-3.9.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.8.4"
-PLUGIN_VERSION = "3.8.4"
+VERSION = "3.9.1"
+PLUGIN_VERSION = "3.9.1"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'harbor', PLUGIN_VERSION, '--server', 'github://api.github.com/pulumiverse/pulumi-harbor'])
         except OSError as error:
```

