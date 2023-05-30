# Comparing `tmp/prompthub_py-3.0.0.tar.gz` & `tmp/prompthub_py-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompthub_py-3.0.0.tar", max compression
+gzip compressed data, was "prompthub_py-3.0.1.tar", max compression
```

## Comparing `prompthub_py-3.0.0.tar` & `prompthub_py-3.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11343 2023-05-27 16:38:40.125084 prompthub_py-3.0.0/LICENSE
--rw-r--r--   0        0        0     1639 2023-05-27 16:38:40.125084 prompthub_py-3.0.0/README.md
--rw-r--r--   0        0        0       65 2023-05-27 16:38:40.125084 prompthub_py-3.0.0/prompthub/__init__.py
--rw-r--r--   0        0        0     1670 2023-05-27 16:38:40.125084 prompthub_py-3.0.0/prompthub/prompt.py
--rw-r--r--   0        0        0      439 2023-05-27 16:38:40.125084 prompthub_py-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     2204 1970-01-01 00:00:00.000000 prompthub_py-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11343 2023-05-30 09:19:30.067541 prompthub_py-3.0.1/LICENSE
+-rw-r--r--   0        0        0     1639 2023-05-30 09:19:30.067541 prompthub_py-3.0.1/README.md
+-rw-r--r--   0        0        0       65 2023-05-30 09:19:30.067541 prompthub_py-3.0.1/prompthub/__init__.py
+-rw-r--r--   0        0        0     1903 2023-05-30 09:19:30.067541 prompthub_py-3.0.1/prompthub/prompt.py
+-rw-r--r--   0        0        0      439 2023-05-30 09:19:30.067541 prompthub_py-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2204 1970-01-01 00:00:00.000000 prompthub_py-3.0.1/PKG-INFO
```

### Comparing `prompthub_py-3.0.0/LICENSE` & `prompthub_py-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prompthub_py-3.0.0/README.md` & `prompthub_py-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `prompthub_py-3.0.0/prompthub/prompt.py` & `prompthub_py-3.0.1/prompthub/prompt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Dict, List
-from dataclasses import dataclass
+from dataclasses import dataclass, asdict
 import json
 import os
 
 import yaml
 import requests
 
 
@@ -20,14 +20,24 @@
     tags: List[str]
     meta: Dict[str, str]
     version: str
     text: str
     description: str
 
 
+    def to_yaml(self, file: str):
+        with open(file, 'w') as f:
+            yaml.safe_dump(asdict(self), f)
+
+
+    def to_json(self, file: str):
+        with open(file, 'w') as f:
+            json.dump(asdict(self), f)
+
+
 def from_json(file: str):
     with open(file) as f:
         data = json.load(f)
         return Prompt(
             data["name"],
             data["tags"],
             data["meta"],
```

### Comparing `prompthub_py-3.0.0/PKG-INFO` & `prompthub_py-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompthub-py
-Version: 3.0.0
+Version: 3.0.1
 Summary: 
 License: Apache-2.0
 Author: deepset.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

