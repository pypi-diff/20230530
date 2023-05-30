# Comparing `tmp/bugout-0.2.7.tar.gz` & `tmp/bugout-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bugout-0.2.7.tar", last modified: Wed May 24 12:48:23 2023, max compression
+gzip compressed data, was "bugout-0.2.8.tar", last modified: Tue May 30 10:05:47 2023, max compression
```

## Comparing `bugout-0.2.7.tar` & `bugout-0.2.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:48:23.644303 bugout-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-24 12:48:09.000000 bugout-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-24 12:48:23.644303 bugout-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-24 12:48:09.000000 bugout-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:48:23.644303 bugout-0.2.7/bugout/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-24 12:48:09.000000 bugout-0.2.7/bugout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-24 12:48:09.000000 bugout-0.2.7/bugout/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32500 2023-05-24 12:48:09.000000 bugout-0.2.7/bugout/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-24 12:48:09.000000 bugout-0.2.7/bugout/calls.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-05-24 12:48:09.000000 bugout-0.2.7/bugout/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-24 12:48:09.000000 bugout-0.2.7/bugout/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-05-24 12:48:09.000000 bugout-0.2.7/bugout/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-24 12:48:09.000000 bugout-0.2.7/bugout/humbug.py
--rw-r--r--   0 runner    (1001) docker     (123)    14287 2023-05-24 12:48:09.000000 bugout-0.2.7/bugout/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23739 2023-05-24 12:48:09.000000 bugout-0.2.7/bugout/journal.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 12:48:09.000000 bugout-0.2.7/bugout/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-24 12:48:09.000000 bugout-0.2.7/bugout/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-24 12:48:09.000000 bugout-0.2.7/bugout/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-05-24 12:48:09.000000 bugout-0.2.7/bugout/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:48:23.644303 bugout-0.2.7/bugout.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-24 12:48:23.000000 bugout-0.2.7/bugout.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-24 12:48:23.000000 bugout-0.2.7/bugout.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 12:48:23.000000 bugout-0.2.7/bugout.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-24 12:48:23.000000 bugout-0.2.7/bugout.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 12:48:15.000000 bugout-0.2.7/bugout.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-24 12:48:23.000000 bugout-0.2.7/bugout.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 12:48:23.000000 bugout-0.2.7/bugout.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 12:48:23.644303 bugout-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-24 12:48:09.000000 bugout-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:05:47.395813 bugout-0.2.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-30 10:05:29.000000 bugout-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-30 10:05:47.395813 bugout-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-30 10:05:29.000000 bugout-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:05:47.391814 bugout-0.2.8/bugout/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-30 10:05:29.000000 bugout-0.2.8/bugout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-30 10:05:29.000000 bugout-0.2.8/bugout/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34157 2023-05-30 10:05:29.000000 bugout-0.2.8/bugout/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-30 10:05:29.000000 bugout-0.2.8/bugout/calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-05-30 10:05:29.000000 bugout-0.2.8/bugout/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-30 10:05:29.000000 bugout-0.2.8/bugout/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-05-30 10:05:29.000000 bugout-0.2.8/bugout/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-30 10:05:29.000000 bugout-0.2.8/bugout/humbug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14287 2023-05-30 10:05:29.000000 bugout-0.2.8/bugout/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25426 2023-05-30 10:05:29.000000 bugout-0.2.8/bugout/journal.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 10:05:29.000000 bugout-0.2.8/bugout/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-05-30 10:05:29.000000 bugout-0.2.8/bugout/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-30 10:05:29.000000 bugout-0.2.8/bugout/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-05-30 10:05:29.000000 bugout-0.2.8/bugout/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:05:47.395813 bugout-0.2.8/bugout.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-30 10:05:47.000000 bugout-0.2.8/bugout.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-30 10:05:47.000000 bugout-0.2.8/bugout.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:05:47.000000 bugout-0.2.8/bugout.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-30 10:05:47.000000 bugout-0.2.8/bugout.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:05:38.000000 bugout-0.2.8/bugout.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-30 10:05:47.000000 bugout-0.2.8/bugout.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-30 10:05:47.000000 bugout-0.2.8/bugout.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 10:05:47.395813 bugout-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-30 10:05:29.000000 bugout-0.2.8/setup.py
```

### Comparing `bugout-0.2.7/LICENSE` & `bugout-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bugout-0.2.7/PKG-INFO` & `bugout-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bugout
-Version: 0.2.7
+Version: 0.2.8
 Summary: Python client library for Bugout API
 Home-page: https://github.com/bugout-dev/bugout-python
 Author: Bugout
 Author-email: engineering@bugout.dev
 License: MIT
 Platform: all
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `bugout-0.2.7/README.md` & `bugout-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `bugout-0.2.7/bugout/__main__.py` & `bugout-0.2.8/bugout/__main__.py`

 * *Files identical despite different names*

### Comparing `bugout-0.2.7/bugout/app.py` & `bugout-0.2.8/bugout/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -783,14 +783,39 @@
             journal_id=journal_id,
             entry_id=entry_id,
             tags=tags,
             auth_type=data.AuthType[auth_type],
             **kwargs,
         )
 
+    def create_entries_tags(
+        self,
+        token: Union[str, uuid.UUID],
+        journal_id: Union[str, uuid.UUID],
+        entries_tags: List[Dict[str, Any]],
+        timeout: float = REQUESTS_TIMEOUT,
+        auth_type: str = data.AuthType.bearer.name,
+        **kwargs: Dict[str, Any],
+    ) -> data.BugoutJournalEntries:
+        self.journal.timeout = timeout
+
+        entries_tags_obj = data.BugoutJournalEntriesTagsRequest(
+            entries=[
+                data.BugoutJournalEntryTagsRequest(**entry_tags)
+                for entry_tags in entries_tags
+            ]
+        )
+        return self.journal.create_entries_tags(
+            token=token,
+            journal_id=journal_id,
+            entries_tags=entries_tags_obj,
+            auth_type=data.AuthType[auth_type],
+            **kwargs,
+        )
+
     def get_tags(
         self,
         token: Union[str, uuid.UUID],
         journal_id: Union[str, uuid.UUID],
         entry_id: Union[str, uuid.UUID],
         timeout: float = REQUESTS_TIMEOUT,
         auth_type: str = data.AuthType.bearer.name,
@@ -841,14 +866,38 @@
             journal_id=journal_id,
             entry_id=entry_id,
             tag=tag,
             auth_type=data.AuthType[auth_type],
             **kwargs,
         )
 
+    def delete_entries_tags(
+        self,
+        token: Union[str, uuid.UUID],
+        journal_id: Union[str, uuid.UUID],
+        entries_tags: List[Dict[str, Any]],
+        timeout: float = REQUESTS_TIMEOUT,
+        auth_type: str = data.AuthType.bearer.name,
+        **kwargs: Dict[str, Any],
+    ) -> data.BugoutJournalEntries:
+        self.journal.timeout = timeout
+        entries_tags_obj = data.BugoutJournalEntriesTagsRequest(
+            entries=[
+                data.BugoutJournalEntryTagsRequest(**entry_tags)
+                for entry_tags in entries_tags
+            ]
+        )
+        return self.journal.delete_entries_tags(
+            token=token,
+            journal_id=journal_id,
+            entries_tags=entries_tags_obj,
+            auth_type=data.AuthType[auth_type],
+            **kwargs,
+        )
+
     # Search
     def search(
         self,
         token: Union[str, uuid.UUID],
         journal_id: Union[str, uuid.UUID],
         query: str,
         filters: Optional[List[str]] = None,
```

### Comparing `bugout-0.2.7/bugout/calls.py` & `bugout-0.2.8/bugout/calls.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Dict
 
-import requests
+import requests  # type: ignore
 
 from .data import Method
 from .exceptions import BugoutResponseException, BugoutUnexpectedResponse
 
 
 def make_request(method: Method, url: str, **kwargs) -> Any:
     try:
```

### Comparing `bugout-0.2.7/bugout/data.py` & `bugout-0.2.8/bugout/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,14 +235,28 @@
 
 class BugoutJournalEntryTags(BaseModel):
     journal_id: uuid.UUID
     entry_id: uuid.UUID
     tags: List[str]
 
 
+class BugoutJournalEntryTagsRequest(BaseModel):
+    journal_entry_id: uuid.UUID = Field(alias="entry_id")
+    tags: List[str]
+
+    class Config:
+        # Required configuration because in Spire we use "journal_entry_id" instead of "entry_id"
+        # during creation and deletion of new tags for journal entry
+        allow_population_by_field_name = True
+
+
+class BugoutJournalEntriesTagsRequest(BaseModel):
+    entries: List[BugoutJournalEntryTagsRequest] = Field(default_factory=list)
+
+
 class BugoutSearchResult(BaseModel):
     entry_url: str
     content_url: str
     title: str
     content: Optional[str]
     tags: List[str]
     created_at: str
```

### Comparing `bugout-0.2.7/bugout/exceptions.py` & `bugout-0.2.8/bugout/exceptions.py`

 * *Files identical despite different names*

### Comparing `bugout-0.2.7/bugout/group.py` & `bugout-0.2.8/bugout/group.py`

 * *Files identical despite different names*

### Comparing `bugout-0.2.7/bugout/humbug.py` & `bugout-0.2.8/bugout/humbug.py`

 * *Files identical despite different names*

### Comparing `bugout-0.2.7/bugout/jobs.py` & `bugout-0.2.8/bugout/jobs.py`

 * *Files identical despite different names*

### Comparing `bugout-0.2.7/bugout/journal.py` & `bugout-0.2.8/bugout/journal.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import uuid
 from enum import Enum
+import json
 from typing import Any, Dict, List, Optional, Union
 
 from .calls import make_request
 from .data import (
     AuthType,
     BugoutJournal,
     BugoutJournalEntries,
     BugoutJournalEntriesRequest,
     BugoutJournalEntry,
     BugoutJournalEntryContent,
     BugoutJournalEntryTags,
+    BugoutJournalEntriesTagsRequest,
     BugoutJournalPermissions,
     BugoutJournals,
     BugoutJournalScopeSpecs,
     BugoutScopes,
     BugoutSearchResults,
     HolderType,
     JournalTypes,
@@ -460,14 +462,37 @@
         if "headers" in kwargs.keys():
             headers.update(kwargs["headers"])
         result = self._call(
             method=Method.post, path=tags_path, headers=headers, json=json
         )
         return result
 
+    def create_entries_tags(
+        self,
+        token: Union[str, uuid.UUID],
+        journal_id: Union[str, uuid.UUID],
+        entries_tags: BugoutJournalEntriesTagsRequest,
+        auth_type: AuthType = AuthType.bearer,
+        **kwargs: Dict[str, Any],
+    ) -> BugoutJournalEntries:
+        tags_path = f"journals/{journal_id}/bulk_entries_tags"
+        headers = {
+            "Authorization": f"{auth_type.value} {token}",
+        }
+        json_body = json.loads(entries_tags.json())
+        if "headers" in kwargs.keys():
+            headers.update(kwargs["headers"])
+        result = self._call(
+            method=Method.post, path=tags_path, headers=headers, json=json_body
+        )
+
+        return BugoutJournalEntries(
+            entries=[BugoutJournalEntry(**entry) for entry in result]
+        )
+
     def get_tags(
         self,
         token: Union[str, uuid.UUID],
         journal_id: Union[str, uuid.UUID],
         entry_id: Union[str, uuid.UUID],
         auth_type: AuthType = AuthType.bearer,
         **kwargs: Dict[str, Any],
@@ -519,14 +544,37 @@
         if "headers" in kwargs.keys():
             headers.update(kwargs["headers"])
         result = self._call(
             method=Method.delete, path=tags_path, headers=headers, json=json
         )
         return BugoutJournalEntryTags(**result)
 
+    def delete_entries_tags(
+        self,
+        token: Union[str, uuid.UUID],
+        journal_id: Union[str, uuid.UUID],
+        entries_tags: BugoutJournalEntriesTagsRequest,
+        auth_type: AuthType = AuthType.bearer,
+        **kwargs: Dict[str, Any],
+    ) -> BugoutJournalEntries:
+        tags_path = f"journals/{journal_id}/bulk_entries_tags"
+        headers = {
+            "Authorization": f"{auth_type.value} {token}",
+        }
+        json_body = json.loads(entries_tags.json())
+        if "headers" in kwargs.keys():
+            headers.update(kwargs["headers"])
+        result = self._call(
+            method=Method.delete, path=tags_path, headers=headers, json=json_body
+        )
+
+        return BugoutJournalEntries(
+            entries=[BugoutJournalEntry(**entry) for entry in result]
+        )
+
     # Search module
     def search(
         self,
         token: Union[str, uuid.UUID],
         journal_id: Union[str, uuid.UUID],
         query: str,
         filters: Optional[List[str]] = None,
```

### Comparing `bugout-0.2.7/bugout/resource.py` & `bugout-0.2.8/bugout/resource.py`

 * *Files identical despite different names*

### Comparing `bugout-0.2.7/bugout/settings.py` & `bugout-0.2.8/bugout/settings.py`

 * *Files identical despite different names*

### Comparing `bugout-0.2.7/bugout/user.py` & `bugout-0.2.8/bugout/user.py`

 * *Files identical despite different names*

### Comparing `bugout-0.2.7/bugout.egg-info/PKG-INFO` & `bugout-0.2.8/bugout.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bugout
-Version: 0.2.7
+Version: 0.2.8
 Summary: Python client library for Bugout API
 Home-page: https://github.com/bugout-dev/bugout-python
 Author: Bugout
 Author-email: engineering@bugout.dev
 License: MIT
 Platform: all
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `bugout-0.2.7/setup.py` & `bugout-0.2.8/setup.py`

 * *Files identical despite different names*

