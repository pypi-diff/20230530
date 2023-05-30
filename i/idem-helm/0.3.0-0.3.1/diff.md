# Comparing `tmp/idem-helm-0.3.0.tar.gz` & `tmp/idem-helm-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem-helm-0.3.0.tar", last modified: Fri Apr 28 14:35:41 2023, max compression
+gzip compressed data, was "idem-helm-0.3.1.tar", last modified: Tue May 30 15:31:28 2023, max compression
```

## Comparing `idem-helm-0.3.0.tar` & `idem-helm-0.3.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:41.067172 idem-helm-0.3.0/
--rw-r--r--   0 root         (0) root         (0)    11345 2023-04-28 14:35:27.000000 idem-helm-0.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5330 2023-04-28 14:35:41.067172 idem-helm-0.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4526 2023-04-28 14:35:27.000000 idem-helm-0.3.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:41.067172 idem-helm-0.3.0/idem_helm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:41.067172 idem-helm-0.3.0/idem_helm/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:41.067172 idem-helm-0.3.0/idem_helm/acct/helm/
--rw-r--r--   0 root         (0) root         (0)      552 2023-04-28 14:35:27.000000 idem-helm-0.3.0/idem_helm/acct/helm/init.py
--rw-r--r--   0 root         (0) root         (0)     1275 2023-04-28 14:35:27.000000 idem-helm-0.3.0/idem_helm/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:41.067172 idem-helm-0.3.0/idem_helm/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:41.067172 idem-helm-0.3.0/idem_helm/exec/helm/
--rw-r--r--   0 root         (0) root         (0)      169 2023-04-28 14:35:27.000000 idem-helm-0.3.0/idem_helm/exec/helm/init.py
--rw-r--r--   0 root         (0) root         (0)     3672 2023-04-28 14:35:27.000000 idem-helm-0.3.0/idem_helm/exec/helm/release.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:41.067172 idem-helm-0.3.0/idem_helm/states/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 14:35:27.000000 idem-helm-0.3.0/idem_helm/states/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:41.067172 idem-helm-0.3.0/idem_helm/states/helm/
--rw-r--r--   0 root         (0) root         (0)      167 2023-04-28 14:35:27.000000 idem-helm-0.3.0/idem_helm/states/helm/init.py
--rw-r--r--   0 root         (0) root         (0)    14938 2023-04-28 14:35:27.000000 idem-helm-0.3.0/idem_helm/states/helm/release.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:41.067172 idem-helm-0.3.0/idem_helm/tool/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-28 14:35:27.000000 idem-helm-0.3.0/idem_helm/tool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:41.067172 idem-helm-0.3.0/idem_helm/tool/helm/
--rw-r--r--   0 root         (0) root         (0)     3262 2023-04-28 14:35:27.000000 idem-helm-0.3.0/idem_helm/tool/helm/command_utils.py
--rw-r--r--   0 root         (0) root         (0)     1280 2023-04-28 14:35:27.000000 idem-helm-0.3.0/idem_helm/tool/helm/comment_utils.py
--rw-r--r--   0 root         (0) root         (0)      753 2023-04-28 14:35:27.000000 idem-helm-0.3.0/idem_helm/tool/helm/release_utils.py
--rw-r--r--   0 root         (0) root         (0)     1340 2023-04-28 14:35:27.000000 idem-helm-0.3.0/idem_helm/tool/helm/test_state_utils.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-28 14:35:40.000000 idem-helm-0.3.0/idem_helm/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-28 14:35:41.067172 idem-helm-0.3.0/idem_helm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5330 2023-04-28 14:35:41.000000 idem-helm-0.3.0/idem_helm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      633 2023-04-28 14:35:41.000000 idem-helm-0.3.0/idem_helm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-28 14:35:41.000000 idem-helm-0.3.0/idem_helm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-04-28 14:35:41.000000 idem-helm-0.3.0/idem_helm.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       69 2023-04-28 14:35:41.000000 idem-helm-0.3.0/idem_helm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-28 14:35:41.000000 idem-helm-0.3.0/idem_helm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-04-28 14:35:41.071172 idem-helm-0.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2719 2023-04-28 14:35:27.000000 idem-helm-0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:31:28.362686 idem-helm-0.3.1/
+-rw-r--r--   0 root         (0) root         (0)    11345 2023-05-30 15:31:14.000000 idem-helm-0.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5330 2023-05-30 15:31:28.362686 idem-helm-0.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4526 2023-05-30 15:31:14.000000 idem-helm-0.3.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:31:28.362686 idem-helm-0.3.1/idem_helm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:31:28.362686 idem-helm-0.3.1/idem_helm/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:31:28.362686 idem-helm-0.3.1/idem_helm/acct/helm/
+-rw-r--r--   0 root         (0) root         (0)      552 2023-05-30 15:31:14.000000 idem-helm-0.3.1/idem_helm/acct/helm/init.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2023-05-30 15:31:14.000000 idem-helm-0.3.1/idem_helm/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:31:28.362686 idem-helm-0.3.1/idem_helm/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:31:28.362686 idem-helm-0.3.1/idem_helm/exec/helm/
+-rw-r--r--   0 root         (0) root         (0)      169 2023-05-30 15:31:14.000000 idem-helm-0.3.1/idem_helm/exec/helm/init.py
+-rw-r--r--   0 root         (0) root         (0)     3701 2023-05-30 15:31:14.000000 idem-helm-0.3.1/idem_helm/exec/helm/release.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:31:28.362686 idem-helm-0.3.1/idem_helm/states/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 15:31:14.000000 idem-helm-0.3.1/idem_helm/states/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:31:28.362686 idem-helm-0.3.1/idem_helm/states/helm/
+-rw-r--r--   0 root         (0) root         (0)      167 2023-05-30 15:31:14.000000 idem-helm-0.3.1/idem_helm/states/helm/init.py
+-rw-r--r--   0 root         (0) root         (0)    14946 2023-05-30 15:31:14.000000 idem-helm-0.3.1/idem_helm/states/helm/release.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:31:28.362686 idem-helm-0.3.1/idem_helm/tool/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-30 15:31:14.000000 idem-helm-0.3.1/idem_helm/tool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:31:28.362686 idem-helm-0.3.1/idem_helm/tool/helm/
+-rw-r--r--   0 root         (0) root         (0)     3403 2023-05-30 15:31:14.000000 idem-helm-0.3.1/idem_helm/tool/helm/command_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1280 2023-05-30 15:31:14.000000 idem-helm-0.3.1/idem_helm/tool/helm/comment_utils.py
+-rw-r--r--   0 root         (0) root         (0)      753 2023-05-30 15:31:14.000000 idem-helm-0.3.1/idem_helm/tool/helm/release_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1340 2023-05-30 15:31:14.000000 idem-helm-0.3.1/idem_helm/tool/helm/test_state_utils.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-30 15:31:27.000000 idem-helm-0.3.1/idem_helm/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 15:31:28.362686 idem-helm-0.3.1/idem_helm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5330 2023-05-30 15:31:28.000000 idem-helm-0.3.1/idem_helm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      633 2023-05-30 15:31:28.000000 idem-helm-0.3.1/idem_helm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 15:31:28.000000 idem-helm-0.3.1/idem_helm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-30 15:31:28.000000 idem-helm-0.3.1/idem_helm.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-05-30 15:31:28.000000 idem-helm-0.3.1/idem_helm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-30 15:31:28.000000 idem-helm-0.3.1/idem_helm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-30 15:31:28.362686 idem-helm-0.3.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2719 2023-05-30 15:31:14.000000 idem-helm-0.3.1/setup.py
```

### Comparing `idem-helm-0.3.0/LICENSE` & `idem-helm-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `idem-helm-0.3.0/PKG-INFO` & `idem-helm-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-helm
-Version: 0.3.0
+Version: 0.3.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Barnali Rakshit
 Author-email: brakshit@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `idem-helm-0.3.0/README.rst` & `idem-helm-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `idem-helm-0.3.0/idem_helm/acct/helm/init.py` & `idem-helm-0.3.1/idem_helm/acct/helm/init.py`

 * *Files identical despite different names*

### Comparing `idem-helm-0.3.0/idem_helm/conf.py` & `idem-helm-0.3.1/idem_helm/conf.py`

 * *Files identical despite different names*

### Comparing `idem-helm-0.3.0/idem_helm/exec/helm/release.py` & `idem-helm-0.3.1/idem_helm/exec/helm/release.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,12 +102,12 @@
         ctx, commands, flags=[], kvflags=kvflags
     )
     if not values_ret["result"] or values_ret.ret["stderr"]:
         result["comment"] = values_ret["comment"]
         result["result"] = False
         return result
 
-    if values_ret.ret["stdout"].rstrip().endswith("null"):
+    if values_ret.ret["stdout"] and values_ret.ret["stdout"].rstrip().endswith("null"):
         values_ret.ret["stdout"] = values_ret.ret["stdout"].replace("null", "")
 
     result["ret"] = values_ret.ret["stdout"]
     return result
```

### Comparing `idem-helm-0.3.0/idem_helm/states/helm/release.py` & `idem-helm-0.3.1/idem_helm/states/helm/release.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,15 +257,15 @@
             desired_state["values"] = {}
         for values_file in desired_state.get("values_files"):
             with open(values_file) as stream:
                 data = yaml.safe_load(stream)
             desired_state["values"].update(data)
         desired_state["values_files"] = None
 
-    __merge_arguments(desired_state["values"], old_state["values"])
+    __merge_arguments(desired_state.get("values"), old_state.get("values"))
 
     diff = differ.deep_diff(old_state, desired_state)
     is_change_detected = False
     for item in diff["new"]:
         new_value = diff["new"].get(item)
         if new_value:  # if value is not None
             if item == "chart":
```

### Comparing `idem-helm-0.3.0/idem_helm/tool/helm/command_utils.py` & `idem-helm-0.3.1/idem_helm/tool/helm/command_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -92,14 +92,19 @@
 
     if not context:
         context = ctx.acct.get("context")
 
     if not config_file_path:
         raise HelmConfigurationError
 
+    config_file_path = (
+        os.path.expanduser(config_file_path)
+        if "~" in config_file_path
+        else config_file_path
+    )
     return config_file_path, context
 
 
 def __set_values(cmd, key, val):
     values = __flatten_values(val, sep=".") if key == "--set" else val
     if isinstance(values, list):
         for value in values:
```

### Comparing `idem-helm-0.3.0/idem_helm/tool/helm/comment_utils.py` & `idem-helm-0.3.1/idem_helm/tool/helm/comment_utils.py`

 * *Files identical despite different names*

### Comparing `idem-helm-0.3.0/idem_helm/tool/helm/release_utils.py` & `idem-helm-0.3.1/idem_helm/tool/helm/release_utils.py`

 * *Files identical despite different names*

### Comparing `idem-helm-0.3.0/idem_helm/tool/helm/test_state_utils.py` & `idem-helm-0.3.1/idem_helm/tool/helm/test_state_utils.py`

 * *Files identical despite different names*

### Comparing `idem-helm-0.3.0/idem_helm.egg-info/PKG-INFO` & `idem-helm-0.3.1/idem_helm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-helm
-Version: 0.3.0
+Version: 0.3.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Barnali Rakshit
 Author-email: brakshit@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `idem-helm-0.3.0/idem_helm.egg-info/SOURCES.txt` & `idem-helm-0.3.1/idem_helm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idem-helm-0.3.0/setup.py` & `idem-helm-0.3.1/setup.py`

 * *Files identical despite different names*

