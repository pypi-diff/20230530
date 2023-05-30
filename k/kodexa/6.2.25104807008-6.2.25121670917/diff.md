# Comparing `tmp/kodexa-6.2.25104807008.tar.gz` & `tmp/kodexa-6.2.25121670917.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa-6.2.25104807008.tar", max compression
+gzip compressed data, was "kodexa-6.2.25121670917.tar", max compression
```

## Comparing `kodexa-6.2.25104807008.tar` & `kodexa-6.2.25121670917.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    11357 2023-05-28 14:14:34.600176 kodexa-6.2.25104807008/LICENSE
--rw-r--r--   0        0        0     2804 2023-05-28 14:14:34.600176 kodexa-6.2.25104807008/README.md
--rw-r--r--   0        0        0      847 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/__init__.py
--rw-r--r--   0        0        0      171 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/assistant/__init__.py
--rw-r--r--   0        0        0    12530 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/assistant/assistant.py
--rw-r--r--   0        0        0      297 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/connectors/__init__.py
--rw-r--r--   0        0        0     7722 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/connectors/connectors.py
--rw-r--r--   0        0        0      720 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/model/__init__.py
--rw-r--r--   0        0        0      753 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/model/base.py
--rw-r--r--   0        0        0    96183 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/model/model.py
--rw-r--r--   0        0        0   116484 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/model/objects.py
--rw-r--r--   0        0        0    38334 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/model/persistence.py
--rw-r--r--   0        0        0      236 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/pipeline/__init__.py
--rw-r--r--   0        0        0    19763 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/pipeline/pipeline.py
--rw-r--r--   0        0        0      216 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/platform/__init__.py
--rw-r--r--   0        0        0   110049 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/platform/client.py
--rw-r--r--   0        0        0    28246 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/platform/kodexa.py
--rw-r--r--   0        0        0      100 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/selectors/__init__.py
--rw-r--r--   0        0        0    13499 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/selectors/ast.py
--rw-r--r--   0        0        0     3698 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/selectors/core.py
--rw-r--r--   0        0        0     3735 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/selectors/lexrules.py
--rw-r--r--   0        0        0     2354 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/selectors/lextab.py
--rw-r--r--   0        0        0       60 2023-05-28 14:14:34.612176 kodexa-6.2.25104807008/kodexa/selectors/lextab.pyi
--rw-r--r--   0        0        0     7054 2023-05-28 14:14:34.612176 kodexa-6.2.25104807008/kodexa/selectors/parserules.py
--rw-r--r--   0        0        0       60 2023-05-28 14:14:34.612176 kodexa-6.2.25104807008/kodexa/selectors/parserules.pyi
--rw-r--r--   0        0        0    21267 2023-05-28 14:14:34.612176 kodexa-6.2.25104807008/kodexa/selectors/parsetab.py
--rw-r--r--   0        0        0       60 2023-05-28 14:14:34.612176 kodexa-6.2.25104807008/kodexa/selectors/parsetab.pyi
--rw-r--r--   0        0        0        0 2023-05-28 14:14:34.612176 kodexa-6.2.25104807008/kodexa/spatial/__init__.py
--rw-r--r--   0        0        0    18991 2023-05-28 14:14:34.612176 kodexa-6.2.25104807008/kodexa/spatial/azure_models.py
--rw-r--r--   0        0        0     2738 2023-05-28 14:14:34.612176 kodexa-6.2.25104807008/kodexa/spatial/bbox_common.py
--rw-r--r--   0        0        0    34222 2023-05-28 14:14:34.612176 kodexa-6.2.25104807008/kodexa/spatial/table_form_common.py
--rw-r--r--   0        0        0      160 2023-05-28 14:14:34.612176 kodexa-6.2.25104807008/kodexa/steps/__init__.py
--rw-r--r--   0        0        0     9587 2023-05-28 14:14:34.612176 kodexa-6.2.25104807008/kodexa/steps/common.py
--rw-r--r--   0        0        0      159 2023-05-28 14:14:34.612176 kodexa-6.2.25104807008/kodexa/testing/__init__.py
--rw-r--r--   0        0        0      932 2023-05-28 14:14:34.612176 kodexa-6.2.25104807008/kodexa/testing/test_components.py
--rw-r--r--   0        0        0    13596 2023-05-28 14:14:34.612176 kodexa-6.2.25104807008/kodexa/testing/test_utils.py
--rw-r--r--   0        0        0       52 2023-05-28 14:14:34.612176 kodexa-6.2.25104807008/kodexa/training/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 14:14:34.612176 kodexa-6.2.25104807008/kodexa/training/train_utils.py
--rw-r--r--   0        0        0     1301 2023-05-28 14:15:05.039914 kodexa-6.2.25104807008/pyproject.toml
--rw-r--r--   0        0        0     4103 1970-01-01 00:00:00.000000 kodexa-6.2.25104807008/setup.py
--rw-r--r--   0        0        0     4158 1970-01-01 00:00:00.000000 kodexa-6.2.25104807008/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-30 12:50:13.316124 kodexa-6.2.25121670917/LICENSE
+-rw-r--r--   0        0        0     2804 2023-05-30 12:50:13.316124 kodexa-6.2.25121670917/README.md
+-rw-r--r--   0        0        0      847 2023-05-30 12:50:13.324124 kodexa-6.2.25121670917/kodexa/__init__.py
+-rw-r--r--   0        0        0      171 2023-05-30 12:50:13.324124 kodexa-6.2.25121670917/kodexa/assistant/__init__.py
+-rw-r--r--   0        0        0    12530 2023-05-30 12:50:13.324124 kodexa-6.2.25121670917/kodexa/assistant/assistant.py
+-rw-r--r--   0        0        0      297 2023-05-30 12:50:13.324124 kodexa-6.2.25121670917/kodexa/connectors/__init__.py
+-rw-r--r--   0        0        0     7722 2023-05-30 12:50:13.324124 kodexa-6.2.25121670917/kodexa/connectors/connectors.py
+-rw-r--r--   0        0        0      720 2023-05-30 12:50:13.324124 kodexa-6.2.25121670917/kodexa/model/__init__.py
+-rw-r--r--   0        0        0      753 2023-05-30 12:50:13.324124 kodexa-6.2.25121670917/kodexa/model/base.py
+-rw-r--r--   0        0        0    96183 2023-05-30 12:50:13.324124 kodexa-6.2.25121670917/kodexa/model/model.py
+-rw-r--r--   0        0        0   116484 2023-05-30 12:50:13.324124 kodexa-6.2.25121670917/kodexa/model/objects.py
+-rw-r--r--   0        0        0    38334 2023-05-30 12:50:13.324124 kodexa-6.2.25121670917/kodexa/model/persistence.py
+-rw-r--r--   0        0        0      236 2023-05-30 12:50:13.324124 kodexa-6.2.25121670917/kodexa/pipeline/__init__.py
+-rw-r--r--   0        0        0    19763 2023-05-30 12:50:13.324124 kodexa-6.2.25121670917/kodexa/pipeline/pipeline.py
+-rw-r--r--   0        0        0      216 2023-05-30 12:50:13.324124 kodexa-6.2.25121670917/kodexa/platform/__init__.py
+-rw-r--r--   0        0        0   110162 2023-05-30 12:50:13.324124 kodexa-6.2.25121670917/kodexa/platform/client.py
+-rw-r--r--   0        0        0    27388 2023-05-30 12:50:13.324124 kodexa-6.2.25121670917/kodexa/platform/kodexa.py
+-rw-r--r--   0        0        0      100 2023-05-30 12:50:13.324124 kodexa-6.2.25121670917/kodexa/selectors/__init__.py
+-rw-r--r--   0        0        0    13499 2023-05-30 12:50:13.324124 kodexa-6.2.25121670917/kodexa/selectors/ast.py
+-rw-r--r--   0        0        0     3698 2023-05-30 12:50:13.324124 kodexa-6.2.25121670917/kodexa/selectors/core.py
+-rw-r--r--   0        0        0     3735 2023-05-30 12:50:13.324124 kodexa-6.2.25121670917/kodexa/selectors/lexrules.py
+-rw-r--r--   0        0        0     2354 2023-05-30 12:50:13.328124 kodexa-6.2.25121670917/kodexa/selectors/lextab.py
+-rw-r--r--   0        0        0       60 2023-05-30 12:50:13.328124 kodexa-6.2.25121670917/kodexa/selectors/lextab.pyi
+-rw-r--r--   0        0        0     7054 2023-05-30 12:50:13.328124 kodexa-6.2.25121670917/kodexa/selectors/parserules.py
+-rw-r--r--   0        0        0       60 2023-05-30 12:50:13.328124 kodexa-6.2.25121670917/kodexa/selectors/parserules.pyi
+-rw-r--r--   0        0        0    21267 2023-05-30 12:50:13.328124 kodexa-6.2.25121670917/kodexa/selectors/parsetab.py
+-rw-r--r--   0        0        0       60 2023-05-30 12:50:13.328124 kodexa-6.2.25121670917/kodexa/selectors/parsetab.pyi
+-rw-r--r--   0        0        0        0 2023-05-30 12:50:13.328124 kodexa-6.2.25121670917/kodexa/spatial/__init__.py
+-rw-r--r--   0        0        0    18991 2023-05-30 12:50:13.328124 kodexa-6.2.25121670917/kodexa/spatial/azure_models.py
+-rw-r--r--   0        0        0     2738 2023-05-30 12:50:13.328124 kodexa-6.2.25121670917/kodexa/spatial/bbox_common.py
+-rw-r--r--   0        0        0    34222 2023-05-30 12:50:13.328124 kodexa-6.2.25121670917/kodexa/spatial/table_form_common.py
+-rw-r--r--   0        0        0      160 2023-05-30 12:50:13.328124 kodexa-6.2.25121670917/kodexa/steps/__init__.py
+-rw-r--r--   0        0        0     9587 2023-05-30 12:50:13.328124 kodexa-6.2.25121670917/kodexa/steps/common.py
+-rw-r--r--   0        0        0      159 2023-05-30 12:50:13.328124 kodexa-6.2.25121670917/kodexa/testing/__init__.py
+-rw-r--r--   0        0        0      932 2023-05-30 12:50:13.328124 kodexa-6.2.25121670917/kodexa/testing/test_components.py
+-rw-r--r--   0        0        0    13596 2023-05-30 12:50:13.328124 kodexa-6.2.25121670917/kodexa/testing/test_utils.py
+-rw-r--r--   0        0        0       52 2023-05-30 12:50:13.328124 kodexa-6.2.25121670917/kodexa/training/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 12:50:13.328124 kodexa-6.2.25121670917/kodexa/training/train_utils.py
+-rw-r--r--   0        0        0     1301 2023-05-30 12:50:29.632146 kodexa-6.2.25121670917/pyproject.toml
+-rw-r--r--   0        0        0     4103 1970-01-01 00:00:00.000000 kodexa-6.2.25121670917/setup.py
+-rw-r--r--   0        0        0     4158 1970-01-01 00:00:00.000000 kodexa-6.2.25121670917/PKG-INFO
```

### Comparing `kodexa-6.2.25104807008/LICENSE` & `kodexa-6.2.25121670917/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25104807008/README.md` & `kodexa-6.2.25121670917/README.md`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25104807008/kodexa/__init__.py` & `kodexa-6.2.25121670917/kodexa/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25104807008/kodexa/assistant/assistant.py` & `kodexa-6.2.25121670917/kodexa/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25104807008/kodexa/connectors/connectors.py` & `kodexa-6.2.25121670917/kodexa/connectors/connectors.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25104807008/kodexa/model/__init__.py` & `kodexa-6.2.25121670917/kodexa/model/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25104807008/kodexa/model/base.py` & `kodexa-6.2.25121670917/kodexa/model/base.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25104807008/kodexa/model/model.py` & `kodexa-6.2.25121670917/kodexa/model/model.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25104807008/kodexa/model/objects.py` & `kodexa-6.2.25121670917/kodexa/model/objects.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25104807008/kodexa/model/persistence.py` & `kodexa-6.2.25121670917/kodexa/model/persistence.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25104807008/kodexa/pipeline/pipeline.py` & `kodexa-6.2.25121670917/kodexa/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25104807008/kodexa/platform/client.py` & `kodexa-6.2.25121670917/kodexa/platform/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -2363,51 +2363,56 @@
 
         if filters is not None:
             params["filter"] = filters
 
         response = self.client.get(url)
         return PageModelTraining.parse_obj(response.json())
 
-    def upload_contents(self, metadata: ModelContentMetadata):
-        """Upload the contents of the metadata to the store"""
-        results = []
-        if metadata.contents:
-
-            import zipfile
-
-            with zipfile.ZipFile('implementation.zip', 'w', zipfile.ZIP_DEFLATED) as zipf:
+    @staticmethod
+    def build_implementation_zip(metadata: ModelContentMetadata):
+        import zipfile
+        num_hits = 0
+
+        with zipfile.ZipFile('implementation.zip', 'w', zipfile.ZIP_DEFLATED) as zipf:
+
+            ignore_files = []
+            if metadata.ignored_contents:
+                for ignore_path in metadata.ignored_contents:
+                    final_wildcard = os.path.join(metadata.base_dir,
+                                                  ignore_path) if metadata.base_dir else ignore_path
+                    for path_hit in glob.glob(final_wildcard, recursive=True):
+                        ignore_files.append(path_hit)
 
-                ignore_files = []
-                if metadata.ignored_contents:
-                    for ignore_path in metadata.ignored_contents:
-                        final_wildcard = os.path.join(metadata.base_dir,
-                                                      ignore_path) if metadata.base_dir else ignore_path
-                        for path_hit in glob.glob(final_wildcard, recursive=True):
-                            ignore_files.append(path_hit)
+            for content_path in metadata.contents:
+                final_wildcard = os.path.join(metadata.base_dir,
+                                              content_path) if metadata.base_dir else content_path
+
+                for path_hit in glob.glob(final_wildcard, recursive=True):
+                    if path_hit in ignore_files:
+                        continue
+                    relative_path = path_hit.replace(metadata.base_dir + '/',
+                                                     '') if metadata.base_dir else path_hit
+
+                    # We will put the implementation in one place
+                    if Path(path_hit).is_file():
+                        zipf.write(path_hit, relative_path)
+                        num_hits += 1
 
-                for content_path in metadata.contents:
-                    final_wildcard = os.path.join(metadata.base_dir,
-                                                  content_path) if metadata.base_dir else content_path
-                    num_hits = 0
+        return num_hits
 
-                    for path_hit in glob.glob(final_wildcard, recursive=True):
-                        if path_hit in ignore_files:
-                            continue
-                        relative_path = path_hit.replace(metadata.base_dir + '/',
-                                                         '') if metadata.base_dir else path_hit
-
-                        # We will put the implementation in one place
-                        if Path(path_hit).is_file():
-                            zipf.write(path_hit, relative_path)
-                            num_hits += 1
-            if num_hits > 0:
+    def upload_contents(self, metadata: ModelContentMetadata, dry_run=False):
+        """Upload the contents of the metadata to the store"""
+        results = []
+        if metadata.contents:
+            num_hits = self.build_implementation_zip(metadata)
+            if num_hits > 0 and not dry_run:
                 with open('implementation.zip', 'rb') as zip_content:
                     self.client.post(f"/api/stores/{self.ref.replace(':', '/')}/implementation",
                                      files={"implementation": zip_content})
-                results.append(f"{num_hits} files packaged for {final_wildcard}")
+                results.append(f"{num_hits} files packaged and deployed to {self.ref}")
         if not metadata.keep_zip:
             Path('implementation.zip').unlink()
         return results
 
 
 class TaxonomiesEndpoint(ComponentEndpoint, ClientEndpoint, OrganizationOwned):
     """Represents a taxonomies endpoint"""
```

### Comparing `kodexa-6.2.25104807008/kodexa/platform/kodexa.py` & `kodexa-6.2.25121670917/kodexa/platform/kodexa.py`

 * *Files 3% similar despite different names*

```diff
@@ -705,34 +705,14 @@
         """
         return {
             "ref": self.ref,
             "options": self.options
         }
 
 
-class ExtensionHelper:
-    """ """
-
-    @staticmethod
-    def load_metadata(path) -> dict:
-
-        if os.path.exists(os.path.join(path, 'dharma.json')):
-            dharma_metadata_file = open(os.path.join(path, 'dharma.json'))
-            dharma_metadata = json.loads(dharma_metadata_file.read())
-        elif os.path.exists(os.path.join(path, 'dharma.yml')):
-            dharma_metadata_file = open(os.path.join(path, 'dharma.yml'))
-            dharma_metadata = yaml.safe_load(dharma_metadata_file.read())
-        elif os.path.exists(os.path.join(path, 'kodexa.yml')):
-            dharma_metadata_file = open(os.path.join(path, 'kodexa.yml'))
-            dharma_metadata = yaml.safe_load(dharma_metadata_file.read())
-        else:
-            raise Exception("Unable to find a kodexa.yml file describing your extension")
-        return dharma_metadata
-
-
 class EventHelper:
 
     def __init__(self, event: ExecutionEvent):
         self.event: ExecutionEvent = event
 
     @staticmethod
     def get_base_event(event_dict: Dict):
```

### Comparing `kodexa-6.2.25104807008/kodexa/selectors/ast.py` & `kodexa-6.2.25121670917/kodexa/selectors/ast.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25104807008/kodexa/selectors/core.py` & `kodexa-6.2.25121670917/kodexa/selectors/core.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25104807008/kodexa/selectors/lexrules.py` & `kodexa-6.2.25121670917/kodexa/selectors/lexrules.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25104807008/kodexa/selectors/lextab.py` & `kodexa-6.2.25121670917/kodexa/selectors/lextab.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25104807008/kodexa/selectors/parserules.py` & `kodexa-6.2.25121670917/kodexa/selectors/parserules.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25104807008/kodexa/selectors/parsetab.py` & `kodexa-6.2.25121670917/kodexa/selectors/parsetab.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25104807008/kodexa/spatial/azure_models.py` & `kodexa-6.2.25121670917/kodexa/spatial/azure_models.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25104807008/kodexa/spatial/bbox_common.py` & `kodexa-6.2.25121670917/kodexa/spatial/bbox_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25104807008/kodexa/spatial/table_form_common.py` & `kodexa-6.2.25121670917/kodexa/spatial/table_form_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25104807008/kodexa/steps/common.py` & `kodexa-6.2.25121670917/kodexa/steps/common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25104807008/kodexa/testing/test_components.py` & `kodexa-6.2.25121670917/kodexa/testing/test_components.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25104807008/kodexa/testing/test_utils.py` & `kodexa-6.2.25121670917/kodexa/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25104807008/pyproject.toml` & `kodexa-6.2.25121670917/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodexa"
-version = "6.2.25104807008"
+version = "6.2.25121670917"
 description = "Python SDK for the Kodexa Platform"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>"]
 readme = "README.md"
 
 packages = [
     { include = "kodexa" }
 ]
```

### Comparing `kodexa-6.2.25104807008/setup.py` & `kodexa-6.2.25121670917/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
  'pyyaml>=6.0,<7.0',
  'requests>=2.28.1,<3.0.0',
  'simpleeval==0.9.12',
  'urllib3>=1.26.14,<2.0.0']
 
 setup_kwargs = {
     'name': 'kodexa',
-    'version': '6.2.25104807008',
+    'version': '6.2.25121670917',
     'description': 'Python SDK for the Kodexa Platform',
     'long_description': '# Kodexa\n\n[![Build and Package with Poetry](https://github.com/kodexa-ai/kodexa/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/kodexa-ai/kodexa/actions/workflows/main.yml)\n\n![img.png](https://docs.kodexa.com/img.png)\n\nKodexa is a platform for building intelligent document processing pipelines. It is a set of tools and services that\nallow you to build a pipeline that can take a document, extract the content, and then process it to extract the\ninformation you need.\n\nIt is built on a set of core principles:\n\n* **Document Centric** - Kodexa is built around the idea of a document. A document is a collection of content\n  nodes that are connected together. This is a powerful model that allows you to build pipelines that can\n  extract content from a wide range of sources.\n\n* **Pipeline Oriented** - Kodexa is built around the idea of a pipeline. A pipeline is a series of steps that\n  can be executed on a document. This allows you to build a pipeline that can extract content from a wide range\n  of sources.\n\n* **Extensible** - Kodexa is built around the idea of a pipeline. A pipeline is a series of steps that can be executed\n  on a document. This allows you to build a pipeline that can extract content from a wide range of sources.\n\n* **Label Driven** - Kodexa focuses on the idea of labels. Labels are a way to identify content within a document\n  and then use that content to drive the processing of the document.\n\n# Python SDK\n\nThis repository contains the Python SDK for Kodexa. The SDK is the primary way to interact with Kodexa. It allows you to\ndefine actions, models, and pipelines that can be executed on Kodexa. It also includes a complete SDK client for\nworking with a Kodexa platform instance.\n\n## Documentation & Examples\n\nDocumentation is available at the [Kodexa Documentation Portal](https://docs.kodexa.com)\n\n## Current Development\n\n[//]: # (Replace it with the diagrams and descriptions for build releases)\n**BUILD VERSION FLOW**\n![build-version-flow.png](docs%2Fbuild-version-flow.png)\nBuild version will differ based on the branches that are published to pypi.\n\n**GITHUB PROCESS**\n![github-process.png](docs%2Fgithub-process.png)\nChanges that contain bugs, features, and fixes should first be pushed to the test branch. \nOnce these changes are thoroughly tested, they can be submitted as a pull request to the main branch. The pull request should be reviewed and approved by an appropriate person before the changes can be merged.\n\n## Set-up\n\nWe use poetry to manage our dependencies, so you can install them with:\n\n    poetry install\n\nYou can then run the tests with:\n\n    poetry run pytest\n\n# Contributing\n\nWe welcome contributions to the Kodexa platform. Please see our [contributing guide](CONTRIBUTING.md) for more details.\n\n# License\n\nApache 2.0\n\n',
     'author': 'Austin Redenbaugh',
     'author_email': 'austin@kodexa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `kodexa-6.2.25104807008/PKG-INFO` & `kodexa-6.2.25121670917/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodexa
-Version: 6.2.25104807008
+Version: 6.2.25121670917
 Summary: Python SDK for the Kodexa Platform
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

