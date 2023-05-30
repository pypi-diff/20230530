# Comparing `tmp/iam_actions-1.2.20230529.tar.gz` & `tmp/iam_actions-1.2.20230530.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230529.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230530.tar", max compression
```

## Comparing `iam_actions-1.2.20230529.tar` & `iam_actions-1.2.20230530.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-05-29 02:33:18.820536 iam_actions-1.2.20230529/LICENSE
--rw-r--r--   0        0        0     2302 2023-05-29 02:33:18.820536 iam_actions-1.2.20230529/README.md
--rw-r--r--   0        0        0      228 2023-05-29 02:33:18.820536 iam_actions-1.2.20230529/iam_actions/__init__.py
--rw-r--r--   0        0        0  4275135 2023-05-29 02:34:44.127971 iam_actions-1.2.20230529/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-05-29 02:33:18.820536 iam_actions-1.2.20230529/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-05-29 02:33:18.820536 iam_actions-1.2.20230529/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-05-29 02:33:18.820536 iam_actions-1.2.20230529/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-05-29 02:33:18.820536 iam_actions-1.2.20230529/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-05-29 02:33:18.820536 iam_actions-1.2.20230529/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-05-29 02:33:18.820536 iam_actions-1.2.20230529/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-05-29 02:33:18.820536 iam_actions-1.2.20230529/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-05-29 02:33:18.820536 iam_actions-1.2.20230529/iam_actions/generate/services.py
--rw-r--r--   0        0        0   549639 2023-05-29 02:34:44.127971 iam_actions-1.2.20230529/iam_actions/policies.json
--rw-r--r--   0        0        0   194779 2023-05-29 02:34:44.127971 iam_actions-1.2.20230529/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   533181 2023-05-29 02:34:44.127971 iam_actions-1.2.20230529/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-05-29 02:34:44.895985 iam_actions-1.2.20230529/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230529/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230529/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-30 02:33:06.259876 iam_actions-1.2.20230530/LICENSE
+-rw-r--r--   0        0        0     2302 2023-05-30 02:33:06.259876 iam_actions-1.2.20230530/README.md
+-rw-r--r--   0        0        0      228 2023-05-30 02:33:06.259876 iam_actions-1.2.20230530/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4275737 2023-05-30 02:34:44.736123 iam_actions-1.2.20230530/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-05-30 02:33:06.259876 iam_actions-1.2.20230530/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-05-30 02:33:06.259876 iam_actions-1.2.20230530/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-05-30 02:33:06.259876 iam_actions-1.2.20230530/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-05-30 02:33:06.259876 iam_actions-1.2.20230530/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-05-30 02:33:06.259876 iam_actions-1.2.20230530/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-05-30 02:33:06.259876 iam_actions-1.2.20230530/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-05-30 02:33:06.259876 iam_actions-1.2.20230530/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-05-30 02:33:06.259876 iam_actions-1.2.20230530/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   549706 2023-05-30 02:34:44.736123 iam_actions-1.2.20230530/iam_actions/policies.json
+-rw-r--r--   0        0        0   194779 2023-05-30 02:34:44.736123 iam_actions-1.2.20230530/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   533245 2023-05-30 02:34:44.736123 iam_actions-1.2.20230530/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-05-30 02:34:45.508125 iam_actions-1.2.20230530/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230530/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230530/PKG-INFO
```

### Comparing `iam_actions-1.2.20230529/LICENSE` & `iam_actions-1.2.20230530/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230529/README.md` & `iam_actions-1.2.20230530/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230529/iam_actions/actions.json` & `iam_actions-1.2.20230530/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999269005847954%*

 * *Differences: {"'iq'": "{'ListAttachments': OrderedDict([('access_level', 'Undocumented'), ('action', "*

 * *         "'ListAttachments'), ('condition_keys', []), ('description', 'Not Documented by AWS'), "*

 * *         "('orphan', False), ('resources', [])]), 'DownloadAttachment': "*

 * *         "OrderedDict([('access_level', 'Undocumented'), ('action', 'DownloadAttachment'), "*

 * *         "('condition_keys', []), ('description', 'Not Documented by AWS'), ('orphan', False), "*

 * *         "('resources', [])]), 'GetRequest': OrderedDict([(' […]*

```diff
@@ -81057,14 +81057,22 @@
             "condition_keys": [],
             "description": "Grants permission to delete an existing attachment",
             "orphan": false,
             "resources": [
                 "attachment"
             ]
         },
+        "DownloadAttachment": {
+            "access_level": "Undocumented",
+            "action": "DownloadAttachment",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "EndCall": {
             "access_level": "Write",
             "action": "EndCall",
             "condition_keys": [],
             "description": "Grants permission to end a voice/video call",
             "orphan": false,
             "resources": [
@@ -81187,14 +81195,22 @@
             "condition_keys": [],
             "description": "Grants permission to read a proposal",
             "orphan": false,
             "resources": [
                 "proposal"
             ]
         },
+        "GetRequest": {
+            "access_level": "Undocumented",
+            "action": "GetRequest",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetReview": {
             "access_level": "Read",
             "action": "GetReview",
             "condition_keys": [],
             "description": "Grants permission to read a review for an expert",
             "orphan": false,
             "resources": [
@@ -81215,14 +81231,22 @@
             "access_level": "Write",
             "action": "InitiateCall",
             "condition_keys": [],
             "description": "Grants permission to start a voice/video call",
             "orphan": false,
             "resources": []
         },
+        "ListAttachments": {
+            "access_level": "Undocumented",
+            "action": "ListAttachments",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListConversations": {
             "access_level": "Read",
             "action": "ListConversations",
             "condition_keys": [],
             "description": "Grants permission to list existing conversations",
             "orphan": false,
             "resources": [
```

### Comparing `iam_actions-1.2.20230529/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230530/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230529/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230530/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230529/iam_actions/generate/generate.py` & `iam_actions-1.2.20230530/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230529/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230530/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230529/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230530/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230529/iam_actions/generate/services.py` & `iam_actions-1.2.20230530/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230529/iam_actions/policies.json` & `iam_actions-1.2.20230530/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999999301968449%*

 * *Differences: {"'serviceMap'": "{'AWS IQ': {'Actions': {insert: [(17, 'DownloadAttachment'), (31, 'GetRequest'), "*

 * *                 "(35, 'ListAttachments')]}}}"}*

```diff
@@ -4539,30 +4539,33 @@
                 "CreateProject",
                 "CreateRequest",
                 "CreateScheduledProposal",
                 "CreateSeller",
                 "CreateUpfrontProposal",
                 "DeclineCall",
                 "DeleteAttachment",
+                "DownloadAttachment",
                 "EndCall",
                 "GetBuyer",
                 "GetCall",
                 "GetChatInfo",
                 "GetChatMessages",
                 "GetChatToken",
                 "GetCompanyProfile",
                 "GetConversation",
                 "GetExpert",
                 "GetListing",
                 "GetMarketplaceSeller",
                 "GetPaymentRequest",
                 "GetProposal",
+                "GetRequest",
                 "GetReview",
                 "HideRequest",
                 "InitiateCall",
+                "ListAttachments",
                 "ListConversations",
                 "ListListings",
                 "ListPaymentRequests",
                 "ListProposals",
                 "ListRequests",
                 "ListReviews",
                 "MarkChatMessageRead",
```

### Comparing `iam_actions-1.2.20230529/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230530/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230529/iam_actions/services.json` & `iam_actions-1.2.20230530/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999939083820664%*

 * *Differences: {"'iq'": "{'Actions': {insert: [(17, 'DownloadAttachment'), (31, 'GetRequest'), (35, "*

 * *         "'ListAttachments')]}}"}*

```diff
@@ -11218,30 +11218,33 @@
             "CreateProject",
             "CreateRequest",
             "CreateScheduledProposal",
             "CreateSeller",
             "CreateUpfrontProposal",
             "DeclineCall",
             "DeleteAttachment",
+            "DownloadAttachment",
             "EndCall",
             "GetBuyer",
             "GetCall",
             "GetChatInfo",
             "GetChatMessages",
             "GetChatToken",
             "GetCompanyProfile",
             "GetConversation",
             "GetExpert",
             "GetListing",
             "GetMarketplaceSeller",
             "GetPaymentRequest",
             "GetProposal",
+            "GetRequest",
             "GetReview",
             "HideRequest",
             "InitiateCall",
+            "ListAttachments",
             "ListConversations",
             "ListListings",
             "ListPaymentRequests",
             "ListProposals",
             "ListRequests",
             "ListReviews",
             "MarkChatMessageRead",
```

### Comparing `iam_actions-1.2.20230529/pyproject.toml` & `iam_actions-1.2.20230530/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230529"
+version = "1.2.20230530"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230529/setup.py` & `iam_actions-1.2.20230530/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230529',
+    'version': '1.2.20230530',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230529/PKG-INFO` & `iam_actions-1.2.20230530/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230529
+Version: 1.2.20230530
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

