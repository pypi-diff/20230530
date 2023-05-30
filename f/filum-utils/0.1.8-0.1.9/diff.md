# Comparing `tmp/filum-utils-0.1.8.tar.gz` & `tmp/filum-utils-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filum-utils-0.1.8.tar", last modified: Tue May  2 21:15:11 2023, max compression
+gzip compressed data, was "filum-utils-0.1.9.tar", last modified: Thu May 18 04:31:59 2023, max compression
```

## Comparing `filum-utils-0.1.8.tar` & `filum-utils-0.1.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 hip        (502) staff       (20)        0 2023-05-02 21:15:11.821471 filum-utils-0.1.8/
--rw-r--r--   0 hip        (502) staff       (20)      373 2023-05-02 21:15:11.821335 filum-utils-0.1.8/PKG-INFO
-drwxr-xr-x   0 hip        (502) staff       (20)        0 2023-05-02 21:15:11.817937 filum-utils-0.1.8/filum_utils/
--rw-r--r--   0 hip        (502) staff       (20)      469 2023-05-02 21:14:35.000000 filum-utils-0.1.8/filum_utils/__init__.py
-drwxr-xr-x   0 hip        (502) staff       (20)        0 2023-05-02 21:15:11.821146 filum-utils-0.1.8/filum_utils/clients/
--rw-r--r--   0 hip        (502) staff       (20)        0 2023-02-16 04:07:46.000000 filum-utils-0.1.8/filum_utils/clients/__init__.py
--rw-r--r--   0 hip        (502) staff       (20)     1327 2023-02-16 04:07:46.000000 filum-utils-0.1.8/filum_utils/clients/action.py
--rw-r--r--   0 hip        (502) staff       (20)       77 2023-02-16 04:07:46.000000 filum-utils-0.1.8/filum_utils/clients/analytics.py
--rw-r--r--   0 hip        (502) staff       (20)     1200 2023-02-16 04:07:46.000000 filum-utils-0.1.8/filum_utils/clients/common.py
--rw-r--r--   0 hip        (502) staff       (20)     8680 2023-04-17 13:35:10.000000 filum-utils-0.1.8/filum_utils/clients/connection.py
--rw-r--r--   0 hip        (502) staff       (20)     2189 2023-02-16 04:07:46.000000 filum-utils-0.1.8/filum_utils/clients/filum.py
--rw-r--r--   0 hip        (502) staff       (20)      534 2023-05-02 21:14:35.000000 filum-utils-0.1.8/filum_utils/clients/iam.py
--rw-r--r--   0 hip        (502) staff       (20)     1403 2023-02-16 04:07:46.000000 filum-utils-0.1.8/filum_utils/clients/log.py
--rw-r--r--   0 hip        (502) staff       (20)     2865 2023-04-17 13:35:10.000000 filum-utils-0.1.8/filum_utils/clients/mini_app.py
--rw-r--r--   0 hip        (502) staff       (20)     1806 2023-02-16 04:07:54.000000 filum-utils-0.1.8/filum_utils/clients/notification.py
--rw-r--r--   0 hip        (502) staff       (20)     1387 2023-04-17 13:34:58.000000 filum-utils-0.1.8/filum_utils/clients/subscription.py
--rw-r--r--   0 hip        (502) staff       (20)    16721 2023-05-02 21:14:35.000000 filum-utils-0.1.8/filum_utils/clients/subscription_object.py
--rw-r--r--   0 hip        (502) staff       (20)     1374 2023-05-02 21:14:35.000000 filum-utils-0.1.8/filum_utils/config.py
--rw-r--r--   0 hip        (502) staff       (20)      483 2023-04-17 13:34:58.000000 filum-utils-0.1.8/filum_utils/enums.py
--rw-r--r--   0 hip        (502) staff       (20)      182 2023-02-16 04:07:46.000000 filum-utils-0.1.8/filum_utils/errors.py
-drwxr-xr-x   0 hip        (502) staff       (20)        0 2023-05-02 21:15:11.818664 filum-utils-0.1.8/filum_utils.egg-info/
--rw-r--r--   0 hip        (502) staff       (20)      373 2023-05-02 21:15:11.000000 filum-utils-0.1.8/filum_utils.egg-info/PKG-INFO
--rw-r--r--   0 hip        (502) staff       (20)      660 2023-05-02 21:15:11.000000 filum-utils-0.1.8/filum_utils.egg-info/SOURCES.txt
--rw-r--r--   0 hip        (502) staff       (20)        1 2023-05-02 21:15:11.000000 filum-utils-0.1.8/filum_utils.egg-info/dependency_links.txt
--rw-r--r--   0 hip        (502) staff       (20)       61 2023-05-02 21:15:11.000000 filum-utils-0.1.8/filum_utils.egg-info/requires.txt
--rw-r--r--   0 hip        (502) staff       (20)       12 2023-05-02 21:15:11.000000 filum-utils-0.1.8/filum_utils.egg-info/top_level.txt
--rw-r--r--   0 hip        (502) staff       (20)       38 2023-05-02 21:15:11.821519 filum-utils-0.1.8/setup.cfg
--rw-r--r--   0 hip        (502) staff       (20)      839 2023-05-02 21:15:01.000000 filum-utils-0.1.8/setup.py
+drwxr-xr-x   0 hip        (502) staff       (20)        0 2023-05-18 04:31:59.234910 filum-utils-0.1.9/
+-rw-r--r--   0 hip        (502) staff       (20)      373 2023-05-18 04:31:59.234759 filum-utils-0.1.9/PKG-INFO
+drwxr-xr-x   0 hip        (502) staff       (20)        0 2023-05-18 04:31:59.231128 filum-utils-0.1.9/filum_utils/
+-rw-r--r--   0 hip        (502) staff       (20)      469 2023-05-02 21:14:35.000000 filum-utils-0.1.9/filum_utils/__init__.py
+drwxr-xr-x   0 hip        (502) staff       (20)        0 2023-05-18 04:31:59.234549 filum-utils-0.1.9/filum_utils/clients/
+-rw-r--r--   0 hip        (502) staff       (20)        0 2023-02-16 04:07:46.000000 filum-utils-0.1.9/filum_utils/clients/__init__.py
+-rw-r--r--   0 hip        (502) staff       (20)     1327 2023-02-16 04:07:46.000000 filum-utils-0.1.9/filum_utils/clients/action.py
+-rw-r--r--   0 hip        (502) staff       (20)       77 2023-02-16 04:07:46.000000 filum-utils-0.1.9/filum_utils/clients/analytics.py
+-rw-r--r--   0 hip        (502) staff       (20)     1200 2023-02-16 04:07:46.000000 filum-utils-0.1.9/filum_utils/clients/common.py
+-rw-r--r--   0 hip        (502) staff       (20)     8680 2023-04-17 13:35:10.000000 filum-utils-0.1.9/filum_utils/clients/connection.py
+-rw-r--r--   0 hip        (502) staff       (20)     2189 2023-05-18 04:31:31.000000 filum-utils-0.1.9/filum_utils/clients/filum.py
+-rw-r--r--   0 hip        (502) staff       (20)      534 2023-05-02 21:14:35.000000 filum-utils-0.1.9/filum_utils/clients/iam.py
+-rw-r--r--   0 hip        (502) staff       (20)     1403 2023-02-16 04:07:46.000000 filum-utils-0.1.9/filum_utils/clients/log.py
+-rw-r--r--   0 hip        (502) staff       (20)     2865 2023-04-17 13:35:10.000000 filum-utils-0.1.9/filum_utils/clients/mini_app.py
+-rw-r--r--   0 hip        (502) staff       (20)     1806 2023-02-16 04:07:54.000000 filum-utils-0.1.9/filum_utils/clients/notification.py
+-rw-r--r--   0 hip        (502) staff       (20)     1387 2023-04-17 13:34:58.000000 filum-utils-0.1.9/filum_utils/clients/subscription.py
+-rw-r--r--   0 hip        (502) staff       (20)    17490 2023-05-18 04:31:31.000000 filum-utils-0.1.9/filum_utils/clients/subscription_object.py
+-rw-r--r--   0 hip        (502) staff       (20)     1374 2023-05-02 21:14:35.000000 filum-utils-0.1.9/filum_utils/config.py
+-rw-r--r--   0 hip        (502) staff       (20)      483 2023-04-17 13:34:58.000000 filum-utils-0.1.9/filum_utils/enums.py
+-rw-r--r--   0 hip        (502) staff       (20)      182 2023-02-16 04:07:46.000000 filum-utils-0.1.9/filum_utils/errors.py
+drwxr-xr-x   0 hip        (502) staff       (20)        0 2023-05-18 04:31:59.231984 filum-utils-0.1.9/filum_utils.egg-info/
+-rw-r--r--   0 hip        (502) staff       (20)      373 2023-05-18 04:31:59.000000 filum-utils-0.1.9/filum_utils.egg-info/PKG-INFO
+-rw-r--r--   0 hip        (502) staff       (20)      660 2023-05-18 04:31:59.000000 filum-utils-0.1.9/filum_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 hip        (502) staff       (20)        1 2023-05-18 04:31:59.000000 filum-utils-0.1.9/filum_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 hip        (502) staff       (20)       61 2023-05-18 04:31:59.000000 filum-utils-0.1.9/filum_utils.egg-info/requires.txt
+-rw-r--r--   0 hip        (502) staff       (20)       12 2023-05-18 04:31:59.000000 filum-utils-0.1.9/filum_utils.egg-info/top_level.txt
+-rw-r--r--   0 hip        (502) staff       (20)       38 2023-05-18 04:31:59.234953 filum-utils-0.1.9/setup.cfg
+-rw-r--r--   0 hip        (502) staff       (20)      839 2023-05-18 04:31:49.000000 filum-utils-0.1.9/setup.py
```

### Comparing `filum-utils-0.1.8/filum_utils/clients/action.py` & `filum-utils-0.1.9/filum_utils/clients/action.py`

 * *Files identical despite different names*

### Comparing `filum-utils-0.1.8/filum_utils/clients/common.py` & `filum-utils-0.1.9/filum_utils/clients/common.py`

 * *Files identical despite different names*

### Comparing `filum-utils-0.1.8/filum_utils/clients/connection.py` & `filum-utils-0.1.9/filum_utils/clients/connection.py`

 * *Files identical despite different names*

### Comparing `filum-utils-0.1.8/filum_utils/clients/filum.py` & `filum-utils-0.1.9/filum_utils/clients/filum.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     def get_automated_action(self, automated_action_id: int):
         return self._request(
             method="GET",
             endpoint=f"/internal/automated-actions/{automated_action_id}"
         )
 
-    def get_campaign(self, campaign_id: int):
+    def get_campaign(self, campaign_id: str):
         return self._request(
             method="GET",
             endpoint=f"/internal/survey-campaigns/{campaign_id}"
         )
 
     def get_segment(self, segment_id: str, organization: Organization):
         return self._request(
```

### Comparing `filum-utils-0.1.8/filum_utils/clients/iam.py` & `filum-utils-0.1.9/filum_utils/clients/iam.py`

 * *Files identical despite different names*

### Comparing `filum-utils-0.1.8/filum_utils/clients/log.py` & `filum-utils-0.1.9/filum_utils/clients/log.py`

 * *Files identical despite different names*

### Comparing `filum-utils-0.1.8/filum_utils/clients/mini_app.py` & `filum-utils-0.1.9/filum_utils/clients/mini_app.py`

 * *Files identical despite different names*

### Comparing `filum-utils-0.1.8/filum_utils/clients/notification.py` & `filum-utils-0.1.9/filum_utils/clients/notification.py`

 * *Files identical despite different names*

### Comparing `filum-utils-0.1.8/filum_utils/clients/subscription.py` & `filum-utils-0.1.9/filum_utils/clients/subscription.py`

 * *Files identical despite different names*

### Comparing `filum-utils-0.1.8/filum_utils/clients/subscription_object.py` & `filum-utils-0.1.9/filum_utils/clients/subscription_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,21 +14,17 @@
 )
 from filum_utils.clients.subscription import SubscriptionClient
 from filum_utils.config import config
 from filum_utils.enums import ParentType, Object
 from filum_utils.errors import BaseError
 
 
-class ProcessFunctionResponse(TypedDict):
-    success_count: int
-    errors: List[Dict[str, Any]]
-
-
 class TriggerFunctionResponse(TypedDict):
     is_finished: bool
+    success_count: Optional[int]
 
 
 ActionType = Dict[str, Any]
 AutomatedActionType = Dict[str, Any]
 CampaignType = Dict[str, Any]
 EventType = Optional[Dict[str, Any]]
 ObjectType = Optional[Dict[str, Any]]
@@ -193,35 +189,43 @@
                 subtitle=error.get("notification_message") or NOTIFICATION_ERROR_MESSAGE_MAPPINGS[error["type"]],
             )
 
     def handle_transactional_trigger(
         self,
         process_transactional_fn: Callable[
             [ActionType, AutomatedActionType, EventType, SubscriptionDataType, ConnectionsType, OrganizationType],
-            ProcessFunctionResponse
+            bool
         ],
         events: List[Dict[str, Any]],
         connections: List[Dict[str, Any]] = None,
         organization: Dict[str, Any] = None
     ) -> TriggerFunctionResponse:
+        success_count = 0
+
         for event in events:
-            self._handle_trigger(
+            result = self._handle_trigger(
                 process_fn=process_transactional_fn,
                 data=event,
                 connections=connections,
                 organization=organization
             )
 
-        return {"is_finished": True}
+            if result:
+                success_count += 1
+
+        return {
+            "is_finished": True,
+            "success_count": success_count
+        }
 
     def handle_segment_users_on_demand_trigger(
         self,
         process_segment_user_fn: Callable[
             [ActionType, AutomatedActionType, UserType, SubscriptionDataType, ConnectionsType, OrganizationType],
-            ProcessFunctionResponse
+            bool
         ],
         properties: List[str] = None,
         required_properties: List[List[str]] = None,
         last_current_index: int = None,
         connections: List[Dict[str, Any]] = None,
         organization: Dict[str, Any] = None
     ) -> TriggerFunctionResponse:
@@ -247,41 +251,51 @@
             organization=self.subscription_client.get_organization(),
             required_properties=required_properties,
             offset=current_index,
             limit=config.SEGMENT_RECORD_LIMIT
         )
 
         total_processed_users = 0
+        success_count = 0
         for user in users:
             current_index += 1
             total_processed_users += 1
 
-            self._handle_trigger(
+            result = self._handle_trigger(
                 process_fn=process_segment_user_fn,
                 data=user,
                 connections=connections,
                 organization=organization
             )
 
+            if result:
+                success_count += 1
+
         if total_processed_users >= config.SEGMENT_RECORD_LIMIT:
             self.update_subscription_data({"last_current_index": current_index})
             self.action_client.sync({
                 "subscription_id": self.subscription_client.subscription["id"],
                 "last_current_index": last_current_index
             })
 
-            return {"is_finished": False}
+            return {
+                "is_finished": False,
+                "success_count": success_count
+            }
 
-        return {"is_finished": True}
+        return {
+            "is_finished": True,
+            "success_count": success_count
+        }
 
     def handle_object_on_demand_trigger(
         self,
         process_segment_fn: Callable[
             [ActionType, AutomatedActionType, ObjectType, SubscriptionDataType, ConnectionsType, OrganizationType],
-            ProcessFunctionResponse
+            bool
         ],
         connections: List[Dict[str, Any]] = None,
         organization: Dict[str, Any] = None
     ) -> TriggerFunctionResponse:
 
         context_type = self.get_context_type()
 
@@ -290,22 +304,27 @@
             data = self.filum_client.get_segment(
                 segment_id=self.get_context_id(),
                 organization=self.subscription_client.get_organization()
             )
         elif context_type == Object.CAMPAIGN:
             data = self.filum_client.get_campaign(campaign_id=self.get_context_id())
 
-        self._handle_trigger(
+        result = self._handle_trigger(
             process_fn=process_segment_fn,
             data=data,
             connections=connections,
             organization=organization
         )
 
-        return {"is_finished": True}
+        success_count = 1 if result else 0
+
+        return {
+            "is_finished": True,
+            "success_count": success_count
+        }
 
     def _handle_trigger(
         self,
         process_fn: Callable,
         data: Dict[str, Any],
         connections: List[Dict[str, Any]] = None,
         organization: Dict[str, Any] = None
@@ -318,15 +337,15 @@
             "automated_action": self.automated_action,
             "data": data,
             "subscription_data": self.get_subscription_data(),
             "connections": connections,
             "organization": organization
         }
 
-        process_fn(**params)
+        return process_fn(**params)
 
     def _get_object_route(self):
         return {
             "path": RoutePath.AUTOMATED_ACTIONS_DETAIL,
             "params": {
                 "automatedActionId": self.automated_action["id"]
             }
@@ -401,33 +420,41 @@
                 subtitle=error.get("notification_message") or NOTIFICATION_ERROR_MESSAGE_MAPPINGS[error["type"]],
             )
 
     def handle_transactional_trigger(
         self,
         process_transactional_fn: [
             [ActionType, CampaignType, EventType, SubscriptionDataType, ConnectionsType],
-            ProcessFunctionResponse
+            bool
         ],
         events: List[Dict[str, Any]],
         connections: List[Dict[str, Any]] = None
     ) -> TriggerFunctionResponse:
+        success_count = 0
+
         for event in events:
-            self._handle_trigger(
+            result = self._handle_trigger(
                 process_fn=process_transactional_fn,
                 data=event,
                 connections=connections
             )
 
-        return {"is_finished": True}
+            if result:
+                success_count += 1
+
+        return {
+            "is_finished": True,
+            "success_count": success_count
+        }
 
     def handle_segment_users_on_demand_trigger(
         self,
         process_segment_user_fn: [
             [ActionType, CampaignType, UserType, SubscriptionDataType, ConnectionsType],
-            ProcessFunctionResponse
+            bool
         ],
         properties: List[str] = None,
         required_properties: List[List[str]] = None,
         connections: List[Dict[str, Any]] = None,
         last_current_index: int = None
     ) -> TriggerFunctionResponse:
         if not last_current_index:
@@ -452,32 +479,42 @@
             organization=self.subscription_client.get_organization(),
             required_properties=required_properties,
             offset=current_index,
             limit=config.SEGMENT_RECORD_LIMIT
         )
 
         total_processed_users = 0
+        success_count = 0
         for user in users:
             current_index += 1
             total_processed_users += 1
-            self._handle_trigger(
+            result = self._handle_trigger(
                 process_fn=process_segment_user_fn,
                 data=user,
                 connections=connections
             )
+            if result:
+                success_count += 1
+
         if total_processed_users >= config.SEGMENT_RECORD_LIMIT:
             self.update_subscription_data({"last_current_index": current_index})
             self.action_client.sync({
                 "subscription_id": self.subscription_client.subscription["id"],
                 "last_current_index": current_index
             })
 
-            return {"is_finished": False}
+            return {
+                "is_finished": False,
+                "success_count": success_count
+            }
 
-        return {"is_finished": True}
+        return {
+            "is_finished": True,
+            "success_count": success_count
+        }
 
     def handle_object_on_demand_trigger(self, process_segment_fn: Callable) -> TriggerFunctionResponse:
         ...
 
     def _handle_trigger(self, process_fn: Callable, data: Dict[str, Any], connections: List[Dict[str, Any]] = None):
         if not connections:
             connections = []
@@ -486,15 +523,15 @@
             "action": self.action_client.action,
             "campaign": self.campaign,
             "data": data,
             "subscription_data": self.get_subscription_data(),
             "connections": connections
         }
 
-        process_fn(**params)
+        return process_fn(**params)
 
     def _get_object_route(self):
         return {
             "path": RoutePath.CAMPAIGNS_DETAIL,
             "params": {
                 "solutionGroup": "cx",
                 "solutionId": "dynamic_feedback",
```

### Comparing `filum-utils-0.1.8/filum_utils/config.py` & `filum-utils-0.1.9/filum_utils/config.py`

 * *Files identical despite different names*

### Comparing `filum-utils-0.1.8/filum_utils.egg-info/SOURCES.txt` & `filum-utils-0.1.9/filum_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `filum-utils-0.1.8/setup.py` & `filum-utils-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import sys
 
 from setuptools import setup, find_packages
 
 sys.path.insert(0, os.path.join(os.path.dirname(__file__), 'filum_analytics'))
 
-VERSION = "0.1.8"
+VERSION = "0.1.9"
 DESCRIPTION = "Filum Utils"
 LONG_DESCRIPTION = "Filum Utils"
 
 install_requires = [
     "requests==2.25.1",
     "filum-analytics-python==1.1.1",
     "glom==20.11.0",
```

