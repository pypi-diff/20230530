# Comparing `tmp/thoughtspot_rest_api_v1-1.5.0.tar.gz` & `tmp/thoughtspot_rest_api_v1-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thoughtspot_rest_api_v1-1.5.0.tar", last modified: Mon May 15 15:24:49 2023, max compression
+gzip compressed data, was "thoughtspot_rest_api_v1-1.5.1.tar", last modified: Tue May 30 19:45:39 2023, max compression
```

## Comparing `thoughtspot_rest_api_v1-1.5.0.tar` & `thoughtspot_rest_api_v1-1.5.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2023-05-15 15:24:49.005890 thoughtspot_rest_api_v1-1.5.0/
--rw-r--r--   0 bryant.howell (535524999) 1339924365    14780 2022-04-06 21:26:49.000000 thoughtspot_rest_api_v1-1.5.0/LICENSE
--rw-r--r--   0 bryant.howell (535524999) 1339924365    29237 2023-05-15 15:24:49.005969 thoughtspot_rest_api_v1-1.5.0/PKG-INFO
--rw-r--r--   0 bryant.howell (535524999) 1339924365    28536 2023-03-17 18:28:57.000000 thoughtspot_rest_api_v1-1.5.0/README.md
--rw-r--r--   0 bryant.howell (535524999) 1339924365       85 2022-04-04 15:39:10.000000 thoughtspot_rest_api_v1-1.5.0/pyproject.toml
--rw-r--r--   0 bryant.howell (535524999) 1339924365      884 2023-05-15 15:24:49.006297 thoughtspot_rest_api_v1-1.5.0/setup.cfg
--rw-r--r--   0 bryant.howell (535524999) 1339924365      236 2022-04-04 15:39:10.000000 thoughtspot_rest_api_v1-1.5.0/setup.py
-drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2023-05-15 15:24:49.001789 thoughtspot_rest_api_v1-1.5.0/src/
-drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2023-05-15 15:24:49.004596 thoughtspot_rest_api_v1-1.5.0/src/thoughtspot_rest_api_v1/
--rw-r--r--   0 bryant.howell (535524999) 1339924365      318 2022-09-09 16:25:24.000000 thoughtspot_rest_api_v1-1.5.0/src/thoughtspot_rest_api_v1/__init__.py
--rw-r--r--   0 bryant.howell (535524999) 1339924365       22 2023-05-15 15:24:30.000000 thoughtspot_rest_api_v1-1.5.0/src/thoughtspot_rest_api_v1/_version.py
--rw-r--r--   0 bryant.howell (535524999) 1339924365     2328 2022-09-09 16:25:24.000000 thoughtspot_rest_api_v1-1.5.0/src/thoughtspot_rest_api_v1/details_objects.py
--rw-r--r--   0 bryant.howell (535524999) 1339924365    75771 2023-05-15 15:24:30.000000 thoughtspot_rest_api_v1-1.5.0/src/thoughtspot_rest_api_v1/tsrestapiv1.py
--rw-r--r--   0 bryant.howell (535524999) 1339924365    21142 2023-03-17 18:42:45.000000 thoughtspot_rest_api_v1-1.5.0/src/thoughtspot_rest_api_v1/tsrestapiv2.py
-drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2023-05-15 15:24:49.005761 thoughtspot_rest_api_v1-1.5.0/src/thoughtspot_rest_api_v1.egg-info/
--rw-r--r--   0 bryant.howell (535524999) 1339924365    29237 2023-05-15 15:24:48.000000 thoughtspot_rest_api_v1-1.5.0/src/thoughtspot_rest_api_v1.egg-info/PKG-INFO
--rw-r--r--   0 bryant.howell (535524999) 1339924365      518 2023-05-15 15:24:48.000000 thoughtspot_rest_api_v1-1.5.0/src/thoughtspot_rest_api_v1.egg-info/SOURCES.txt
--rw-r--r--   0 bryant.howell (535524999) 1339924365        1 2023-05-15 15:24:48.000000 thoughtspot_rest_api_v1-1.5.0/src/thoughtspot_rest_api_v1.egg-info/dependency_links.txt
--rw-r--r--   0 bryant.howell (535524999) 1339924365       22 2023-05-15 15:24:48.000000 thoughtspot_rest_api_v1-1.5.0/src/thoughtspot_rest_api_v1.egg-info/requires.txt
--rw-r--r--   0 bryant.howell (535524999) 1339924365       24 2023-05-15 15:24:48.000000 thoughtspot_rest_api_v1-1.5.0/src/thoughtspot_rest_api_v1.egg-info/top_level.txt
+drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2023-05-30 19:45:39.677397 thoughtspot_rest_api_v1-1.5.1/
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    14780 2022-04-06 21:26:49.000000 thoughtspot_rest_api_v1-1.5.1/LICENSE
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    29237 2023-05-30 19:45:39.677472 thoughtspot_rest_api_v1-1.5.1/PKG-INFO
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    28536 2023-03-17 18:28:57.000000 thoughtspot_rest_api_v1-1.5.1/README.md
+-rw-r--r--   0 bryant.howell (535524999) 1339924365       85 2022-04-04 15:39:10.000000 thoughtspot_rest_api_v1-1.5.1/pyproject.toml
+-rw-r--r--   0 bryant.howell (535524999) 1339924365      884 2023-05-30 19:45:39.677800 thoughtspot_rest_api_v1-1.5.1/setup.cfg
+-rw-r--r--   0 bryant.howell (535524999) 1339924365      236 2022-04-04 15:39:10.000000 thoughtspot_rest_api_v1-1.5.1/setup.py
+drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2023-05-30 19:45:39.672979 thoughtspot_rest_api_v1-1.5.1/src/
+drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2023-05-30 19:45:39.676064 thoughtspot_rest_api_v1-1.5.1/src/thoughtspot_rest_api_v1/
+-rw-r--r--   0 bryant.howell (535524999) 1339924365      318 2022-09-09 16:25:24.000000 thoughtspot_rest_api_v1-1.5.1/src/thoughtspot_rest_api_v1/__init__.py
+-rw-r--r--   0 bryant.howell (535524999) 1339924365       22 2023-05-30 16:27:14.000000 thoughtspot_rest_api_v1-1.5.1/src/thoughtspot_rest_api_v1/_version.py
+-rw-r--r--   0 bryant.howell (535524999) 1339924365     2328 2022-09-09 16:25:24.000000 thoughtspot_rest_api_v1-1.5.1/src/thoughtspot_rest_api_v1/details_objects.py
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    75771 2023-05-15 15:24:30.000000 thoughtspot_rest_api_v1-1.5.1/src/thoughtspot_rest_api_v1/tsrestapiv1.py
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    24853 2023-05-30 19:44:47.000000 thoughtspot_rest_api_v1-1.5.1/src/thoughtspot_rest_api_v1/tsrestapiv2.py
+drwxr-xr-x   0 bryant.howell (535524999) 1339924365        0 2023-05-30 19:45:39.677267 thoughtspot_rest_api_v1-1.5.1/src/thoughtspot_rest_api_v1.egg-info/
+-rw-r--r--   0 bryant.howell (535524999) 1339924365    29237 2023-05-30 19:45:39.000000 thoughtspot_rest_api_v1-1.5.1/src/thoughtspot_rest_api_v1.egg-info/PKG-INFO
+-rw-r--r--   0 bryant.howell (535524999) 1339924365      518 2023-05-30 19:45:39.000000 thoughtspot_rest_api_v1-1.5.1/src/thoughtspot_rest_api_v1.egg-info/SOURCES.txt
+-rw-r--r--   0 bryant.howell (535524999) 1339924365        1 2023-05-30 19:45:39.000000 thoughtspot_rest_api_v1-1.5.1/src/thoughtspot_rest_api_v1.egg-info/dependency_links.txt
+-rw-r--r--   0 bryant.howell (535524999) 1339924365       22 2023-05-30 19:45:39.000000 thoughtspot_rest_api_v1-1.5.1/src/thoughtspot_rest_api_v1.egg-info/requires.txt
+-rw-r--r--   0 bryant.howell (535524999) 1339924365       24 2023-05-30 19:45:39.000000 thoughtspot_rest_api_v1-1.5.1/src/thoughtspot_rest_api_v1.egg-info/top_level.txt
```

### Comparing `thoughtspot_rest_api_v1-1.5.0/LICENSE` & `thoughtspot_rest_api_v1-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `thoughtspot_rest_api_v1-1.5.0/PKG-INFO` & `thoughtspot_rest_api_v1-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thoughtspot_rest_api_v1
-Version: 1.5.0
+Version: 1.5.1
 Summary: Library implementing the ThoughtSpot V1 REST API
 Home-page: https://github.com/thoughtspot/thoughtspot_rest_api_v1_python
 Author: Bryant Howell
 Author-email: bryant.howell@thoughtspot.com
 License: MIT
 Project-URL: Documentation, https://github.com/thoughtspot/thoughtspot_rest_api_v1_python#readme
 Project-URL: Bug Tracker, https://github.com/thoughtspot/thoughtspot_rest_api_v1_python/issues
```

### Comparing `thoughtspot_rest_api_v1-1.5.0/README.md` & `thoughtspot_rest_api_v1-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `thoughtspot_rest_api_v1-1.5.0/setup.cfg` & `thoughtspot_rest_api_v1-1.5.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = thoughtspot_rest_api_v1
-version = 1.5.0
+version = 1.5.1
 description = Library implementing the ThoughtSpot V1 REST API
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/thoughtspot/thoughtspot_rest_api_v1_python
 author = Bryant Howell
 author_email = bryant.howell@thoughtspot.com
 license = MIT
```

### Comparing `thoughtspot_rest_api_v1-1.5.0/src/thoughtspot_rest_api_v1/details_objects.py` & `thoughtspot_rest_api_v1-1.5.1/src/thoughtspot_rest_api_v1/details_objects.py`

 * *Files identical despite different names*

### Comparing `thoughtspot_rest_api_v1-1.5.0/src/thoughtspot_rest_api_v1/tsrestapiv1.py` & `thoughtspot_rest_api_v1-1.5.1/src/thoughtspot_rest_api_v1/tsrestapiv1.py`

 * *Files identical despite different names*

### Comparing `thoughtspot_rest_api_v1-1.5.0/src/thoughtspot_rest_api_v1/tsrestapiv2.py` & `thoughtspot_rest_api_v1-1.5.1/src/thoughtspot_rest_api_v1/tsrestapiv2.py`

 * *Files 14% similar despite different names*

```diff
@@ -242,14 +242,21 @@
     # Endpoint is embedded within the method
     # If the endpoint URL itself takes an id, the id will be second argument
     # If the POST request takes simple required arguments, they will be made arguments of the method
     # If the possible arguments take complex structures or are highly variable, there will be a requestt argument
     #
 
     #
+    # /auth/ endpoints not involved with signin /tokens
+    #
+    def auth_session_user(self):
+        endpoint = 'auth/session/user'
+        return self.get_request(endpoint=endpoint)
+
+    #
     # /users/ endpoints
     #
     def users_search(self, request: Dict):
         endpoint = 'users/search'
         return self.post_request(endpoint=endpoint, request=request)
 
     def users_create(self, request: Dict):
@@ -334,19 +341,14 @@
     def orgs_update(self, org_identifier: str, request: Dict):
         endpoint = 'orgs/{}/update'.format(org_identifier)
         return self.post_request(endpoint=endpoint, request=request)
 
     def orgs_delete(self, org_identifier: str):
         endpoint = 'orgs/{}/delete'.format(org_identifier)
         return self.post_request(endpoint=endpoint)
-    #
-    #
-    # /metadata/ endpoints
-    #
-    #
 
     #
     # /metadata/tag endpoints
     #
     def tags_search(self, tag_identifier: Optional[str] = None, color: Optional[str] = None):
         endpoint = 'tags/search'
         if tag_identifier is None and color is None:
@@ -532,14 +534,63 @@
             'log_type': log_type,
             'start_epoch_time_in_millis': start_epoch_time_in_millis,
             'end_epoch_time_in_millis': end_epoch_time_in_millis
         }
         return self.post_request(endpoint=endpoint, request=request)
 
 #
+# Version Control /vcs/ endpoints
+#
+    def vcs_git_config_search(self, request: Dict):
+        endpoint = 'vcs/git/config/search'
+        return self.post_request(endpoint=endpoint, request=request)
+
+    def vcs_git_commits_search(self, request: Dict):
+        endpoint = 'vcs/git/commits/search'
+        return self.post_request(endpoint=endpoint, request=request)
+
+    def vcs_git_config_create(self, request: Dict):
+        endpoint = 'vcs/git/config/create'
+        return self.post_request(endpoint=endpoint, request=request)
+
+    def vcs_git_config_update(self, request: Dict):
+        endpoint = 'vcs/git/config/update'
+        return self.post_request(endpoint=endpoint, request=request)
+
+    def vcs_git_config_delete(self, request: Dict):
+        endpoint = 'vcs/git/config/delete'
+        return self.post_request(endpoint=endpoint, request=request)
+
+    # Possibly will change?
+    def vcs_git_branches_pull(self, branch_name: str):
+        endpoint = 'vcs/git/branches/{}/pull'.format(branch_name)
+        request = {'branch_name': branch_name}
+        return self.post_request(endpoint=endpoint, request=request)
+
+    def vcs_git_branches_commit(self, request: Dict):
+        endpoint = 'vcs/git/branches/commit'
+        return self.post_request(endpoint=endpoint, request=request)
+
+    def vcs_git_commits_revert(self, commit_id: str, request: Dict):
+        endpoint = 'vcs/git/commits/{}/revert'.format(commit_id)
+        return self.post_request(endpoint=endpoint, request=request)
+
+    def vcs_git_branches_validate(self, source_branch_name: str, target_branch_name: str):
+        endpoint = 'vcs/git/branches/validate'
+        request = {
+            'source_branch_name': source_branch_name,
+            'target_branch_name': target_branch_name
+        }
+        return self.post_request(endpoint=endpoint, request=request)
+
+    def vcs_git_commits_deploy(self, request: Dict):
+        endpoint = 'vcs/git/commits/deploy'
+        return self.post_request(endpoint=endpoint, request=request)
+
+#
 # /connection/ endpoints
 #
     def connection_search(self, request: Dict):
         endpoint = 'connection/search'
         return self.post_request(endpoint=endpoint, request=request)
 
     def connection_create(self, request: Dict):
@@ -550,7 +601,47 @@
         endpoint = 'connection/delete'
         request = {'connection_identifier': connection_identifier}
         return self.post_request(endpoint=endpoint, request=request)
 
     def connection_update(self, request: Dict):
         endpoint = 'connection/update'
         return self.post_request(endpoint=endpoint, request=request)
+
+#
+# /roles/ endpoints
+#
+    def roles_search(self, request: Dict):
+        endpoint = 'roles/search'
+        return self.post_request(endpoint=endpoint, request=request)
+
+    def roles_create(self, request: Dict):
+        endpoint = 'roles/create'
+        return self.post_request(endpoint=endpoint, request=request)
+
+    def roles_update(self, role_identifier: str, request: Dict):
+        endpoint = 'roles/{}/update'.format(role_identifier)
+        return self.post_request(endpoint=endpoint, request=request)
+
+    def roles_delete(self, role_identifier: str):
+        endpoint = 'roles/{}/delete'.format(role_identifier)
+        request = { 'role_identifier': role_identifier}
+        return self.post_request(endpoint=endpoint, request=request)
+
+#
+# /schedules/ endpoints
+#
+    def schedules_search(self, request: Dict):
+        endpoint = 'schedules/search'
+        return self.post_request(endpoint=endpoint, request=request)
+
+    def schedules_create(self, request: Dict):
+        endpoint = 'schedules'
+        return self.post_request(endpoint=endpoint, request=request)
+
+    def schedules_update(self, schedule_identifier: str, request: Dict):
+        endpoint = 'schedules/{}/update'.format(schedule_identifier)
+        return self.post_request(endpoint=endpoint, request=request)
+
+    def schedules_delete(self, schedule_identifier: str):
+        endpoint = 'schedules/{}/delete'.format(schedule_identifier)
+        request = { 'schedule_identifier': schedule_identifier}
+        return self.post_request(endpoint=endpoint, request=request)
```

### Comparing `thoughtspot_rest_api_v1-1.5.0/src/thoughtspot_rest_api_v1.egg-info/PKG-INFO` & `thoughtspot_rest_api_v1-1.5.1/src/thoughtspot_rest_api_v1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thoughtspot-rest-api-v1
-Version: 1.5.0
+Version: 1.5.1
 Summary: Library implementing the ThoughtSpot V1 REST API
 Home-page: https://github.com/thoughtspot/thoughtspot_rest_api_v1_python
 Author: Bryant Howell
 Author-email: bryant.howell@thoughtspot.com
 License: MIT
 Project-URL: Documentation, https://github.com/thoughtspot/thoughtspot_rest_api_v1_python#readme
 Project-URL: Bug Tracker, https://github.com/thoughtspot/thoughtspot_rest_api_v1_python/issues
```

### Comparing `thoughtspot_rest_api_v1-1.5.0/src/thoughtspot_rest_api_v1.egg-info/SOURCES.txt` & `thoughtspot_rest_api_v1-1.5.1/src/thoughtspot_rest_api_v1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

