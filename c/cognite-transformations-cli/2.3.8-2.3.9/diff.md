# Comparing `tmp/cognite_transformations_cli-2.3.8.tar.gz` & `tmp/cognite_transformations_cli-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_transformations_cli-2.3.8.tar", max compression
+gzip compressed data, was "cognite_transformations_cli-2.3.9.tar", max compression
```

## Comparing `cognite_transformations_cli-2.3.8.tar` & `cognite_transformations_cli-2.3.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    10172 2023-05-26 07:57:25.336425 cognite_transformations_cli-2.3.8/LICENSE
--rw-r--r--   0        0        0     4288 2023-05-26 07:57:25.336425 cognite_transformations_cli-2.3.8/README.md
--rw-r--r--   0        0        0       22 2023-05-26 07:57:25.336425 cognite_transformations_cli-2.3.8/cognite/transformations_cli/__init__.py
--rw-r--r--   0        0        0      270 2023-05-26 07:57:25.336425 cognite_transformations_cli-2.3.8/cognite/transformations_cli/__main__.py
--rw-r--r--   0        0        0     1489 2023-05-26 07:57:25.336425 cognite_transformations_cli-2.3.8/cognite/transformations_cli/clients.py
--rw-r--r--   0        0        0        0 2023-05-26 07:57:25.336425 cognite_transformations_cli-2.3.8/cognite/transformations_cli/commands/__init__.py
--rw-r--r--   0        0        0     3615 2023-05-26 07:57:25.336425 cognite_transformations_cli-2.3.8/cognite/transformations_cli/commands/base.py
--rw-r--r--   0        0        0     1491 2023-05-26 07:57:25.336425 cognite_transformations_cli-2.3.8/cognite/transformations_cli/commands/delete.py
--rw-r--r--   0        0        0        0 2023-05-26 07:57:25.336425 cognite_transformations_cli-2.3.8/cognite/transformations_cli/commands/deploy/__init__.py
--rw-r--r--   0        0        0     6459 2023-05-26 07:57:25.336425 cognite_transformations_cli-2.3.8/cognite/transformations_cli/commands/deploy/deploy.py
--rw-r--r--   0        0        0     6754 2023-05-26 07:57:25.336425 cognite_transformations_cli-2.3.8/cognite/transformations_cli/commands/deploy/load_yaml.py
--rw-r--r--   0        0        0     4998 2023-05-26 07:57:25.336425 cognite_transformations_cli-2.3.8/cognite/transformations_cli/commands/deploy/transformation_config.py
--rw-r--r--   0        0        0     4005 2023-05-26 07:57:25.336425 cognite_transformations_cli-2.3.8/cognite/transformations_cli/commands/deploy/transformation_types.py
--rw-r--r--   0        0        0     4705 2023-05-26 07:57:25.336425 cognite_transformations_cli-2.3.8/cognite/transformations_cli/commands/deploy/transformation_types_legacy.py
--rw-r--r--   0        0        0    12723 2023-05-26 07:57:25.336425 cognite_transformations_cli-2.3.8/cognite/transformations_cli/commands/deploy/transformations_api.py
--rw-r--r--   0        0        0     2166 2023-05-26 07:57:25.336425 cognite_transformations_cli-2.3.8/cognite/transformations_cli/commands/jobs.py
--rw-r--r--   0        0        0     2438 2023-05-26 07:57:25.336425 cognite_transformations_cli-2.3.8/cognite/transformations_cli/commands/list.py
--rw-r--r--   0        0        0     1242 2023-05-26 07:57:25.336425 cognite_transformations_cli-2.3.8/cognite/transformations_cli/commands/query.py
--rw-r--r--   0        0        0     3639 2023-05-26 07:57:25.336425 cognite_transformations_cli-2.3.8/cognite/transformations_cli/commands/run.py
--rw-r--r--   0        0        0     2787 2023-05-26 07:57:25.336425 cognite_transformations_cli-2.3.8/cognite/transformations_cli/commands/show.py
--rw-r--r--   0        0        0     5792 2023-05-26 07:57:25.336425 cognite_transformations_cli-2.3.8/cognite/transformations_cli/commands/utils.py
--rw-r--r--   0        0        0     1616 2023-05-26 07:57:25.340425 cognite_transformations_cli-2.3.8/pyproject.toml
--rw-r--r--   0        0        0     5474 1970-01-01 00:00:00.000000 cognite_transformations_cli-2.3.8/PKG-INFO
+-rw-r--r--   0        0        0    10172 2023-05-30 08:35:38.321680 cognite_transformations_cli-2.3.9/LICENSE
+-rw-r--r--   0        0        0     4288 2023-05-30 08:35:38.321680 cognite_transformations_cli-2.3.9/README.md
+-rw-r--r--   0        0        0       22 2023-05-30 08:35:38.325680 cognite_transformations_cli-2.3.9/cognite/transformations_cli/__init__.py
+-rw-r--r--   0        0        0      270 2023-05-30 08:35:38.325680 cognite_transformations_cli-2.3.9/cognite/transformations_cli/__main__.py
+-rw-r--r--   0        0        0     1489 2023-05-30 08:35:38.325680 cognite_transformations_cli-2.3.9/cognite/transformations_cli/clients.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:35:38.325680 cognite_transformations_cli-2.3.9/cognite/transformations_cli/commands/__init__.py
+-rw-r--r--   0        0        0     3615 2023-05-30 08:35:38.325680 cognite_transformations_cli-2.3.9/cognite/transformations_cli/commands/base.py
+-rw-r--r--   0        0        0     1491 2023-05-30 08:35:38.325680 cognite_transformations_cli-2.3.9/cognite/transformations_cli/commands/delete.py
+-rw-r--r--   0        0        0        0 2023-05-30 08:35:38.325680 cognite_transformations_cli-2.3.9/cognite/transformations_cli/commands/deploy/__init__.py
+-rw-r--r--   0        0        0     6459 2023-05-30 08:35:38.325680 cognite_transformations_cli-2.3.9/cognite/transformations_cli/commands/deploy/deploy.py
+-rw-r--r--   0        0        0     6754 2023-05-30 08:35:38.325680 cognite_transformations_cli-2.3.9/cognite/transformations_cli/commands/deploy/load_yaml.py
+-rw-r--r--   0        0        0     5442 2023-05-30 08:35:38.325680 cognite_transformations_cli-2.3.9/cognite/transformations_cli/commands/deploy/transformation_config.py
+-rw-r--r--   0        0        0     5010 2023-05-30 08:35:38.325680 cognite_transformations_cli-2.3.9/cognite/transformations_cli/commands/deploy/transformation_types.py
+-rw-r--r--   0        0        0     4705 2023-05-30 08:35:38.325680 cognite_transformations_cli-2.3.9/cognite/transformations_cli/commands/deploy/transformation_types_legacy.py
+-rw-r--r--   0        0        0    13334 2023-05-30 08:35:38.325680 cognite_transformations_cli-2.3.9/cognite/transformations_cli/commands/deploy/transformations_api.py
+-rw-r--r--   0        0        0     2166 2023-05-30 08:35:38.325680 cognite_transformations_cli-2.3.9/cognite/transformations_cli/commands/jobs.py
+-rw-r--r--   0        0        0     2438 2023-05-30 08:35:38.325680 cognite_transformations_cli-2.3.9/cognite/transformations_cli/commands/list.py
+-rw-r--r--   0        0        0     1242 2023-05-30 08:35:38.325680 cognite_transformations_cli-2.3.9/cognite/transformations_cli/commands/query.py
+-rw-r--r--   0        0        0     3639 2023-05-30 08:35:38.325680 cognite_transformations_cli-2.3.9/cognite/transformations_cli/commands/run.py
+-rw-r--r--   0        0        0     2787 2023-05-30 08:35:38.325680 cognite_transformations_cli-2.3.9/cognite/transformations_cli/commands/show.py
+-rw-r--r--   0        0        0     5792 2023-05-30 08:35:38.325680 cognite_transformations_cli-2.3.9/cognite/transformations_cli/commands/utils.py
+-rw-r--r--   0        0        0     1617 2023-05-30 08:35:38.329681 cognite_transformations_cli-2.3.9/pyproject.toml
+-rw-r--r--   0        0        0     5474 1970-01-01 00:00:00.000000 cognite_transformations_cli-2.3.9/PKG-INFO
```

### Comparing `cognite_transformations_cli-2.3.8/LICENSE` & `cognite_transformations_cli-2.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.8/README.md` & `cognite_transformations_cli-2.3.9/README.md`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.8/cognite/transformations_cli/clients.py` & `cognite_transformations_cli-2.3.9/cognite/transformations_cli/clients.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.8/cognite/transformations_cli/commands/base.py` & `cognite_transformations_cli-2.3.9/cognite/transformations_cli/commands/base.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.8/cognite/transformations_cli/commands/delete.py` & `cognite_transformations_cli-2.3.9/cognite/transformations_cli/commands/delete.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.8/cognite/transformations_cli/commands/deploy/deploy.py` & `cognite_transformations_cli-2.3.9/cognite/transformations_cli/commands/deploy/deploy.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.8/cognite/transformations_cli/commands/deploy/load_yaml.py` & `cognite_transformations_cli-2.3.9/cognite/transformations_cli/commands/deploy/load_yaml.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.8/cognite/transformations_cli/commands/deploy/transformation_config.py` & `cognite_transformations_cli-2.3.9/cognite/transformations_cli/commands/deploy/transformation_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,19 @@
                             view external_id, view version and instance_space to be set."
             )
         if flat_destination_type == DestinationType.edges:
             raise Exception(
                 f"Error on transformation manifest with external ID {external_id}: Edges destination requires view space,  \
                             view external_id, view version, instance_space and edge_type space, edge_type external_id to be set."
             )
+        if flat_destination_type == DestinationType.instances:
+            raise Exception(
+                f"Error on transformation manifest with external ID {external_id}: Instances destination requires data model space,  \
+                            data_model space, data_model external_id, data_model version, instance_space, data_model destination_type, data_model destination_relationship_from_type optional  to be set."
+            )
         if flat_destination_type == DestinationType.sequence_rows:
             raise Exception(
                 f"Error on transformation manifest with external ID {external_id}: Sequence rows destination requires external_id to be set."
             )
     return None
```

### Comparing `cognite_transformations_cli-2.3.8/cognite/transformations_cli/commands/deploy/transformation_types.py` & `cognite_transformations_cli-2.3.9/cognite/transformations_cli/commands/deploy/transformation_types.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     labels = "labels"
     relationships = "relationships"
     raw = "raw"
     data_sets = "data_sets"
     sequence_rows = "sequence_rows"
     nodes = "nodes"
     edges = "edges"
+    instances = "instances"
 
 
 class ActionType(Enum):
     create = "create"
     abort = "abort"
     update = "update"
     upsert = "upsert"
@@ -90,14 +91,41 @@
     def __init__(self, space: str, external_id: str, version: Union[int, str]):
         self.space = space
         self.external_id = external_id
         self.version = str(version)
 
 
 @dataclass
+class DataModelInfo:
+    space: str
+    external_id: str
+    version: Union[int, str]
+    destination_type: str
+    destination_relationship_from_type: Optional[str] = None
+
+    """
+    CAST DataModel version int to string
+    """
+
+    def __init__(
+        self,
+        space: str,
+        external_id: str,
+        version: Union[int, str],
+        destination_type: str,
+        destination_relationship_from_type: Optional[str] = None,
+    ):
+        self.space = space
+        self.external_id = external_id
+        self.version = str(version)
+        self.destination_type = destination_type
+        self.destination_relationship_from_type = destination_relationship_from_type
+
+
+@dataclass
 class EdgeType:
     space: str
     external_id: str
 
 
 @dataclass
 class InstanceNodesDestinationConfig:
@@ -121,14 +149,25 @@
     edge_type: Optional[EdgeType]
     type: Literal[
         DestinationType.edges
     ] = DestinationType.edges  # DestinationType updated with  Literal[DestinationType.edges]
 
 
 @dataclass
+class InstancesDestinationConfig:
+    """
+    Valid type values are: instances
+    """
+
+    data_model: Optional[DataModelInfo]
+    instance_space: Optional[str]
+    type: Literal[DestinationType.instances] = DestinationType.instances
+
+
+@dataclass
 class SequenceRowsDestinationConfig:
     """
     Valid type values are: sequence_rows
     """
 
     external_id: str
     type: DestinationType = DestinationType.sequence_rows
@@ -137,14 +176,15 @@
 DestinationConfigType = Union[
     DestinationType,
     DestinationConfig,
     RawDestinationConfig,
     SequenceRowsDestinationConfig,
     InstanceNodesDestinationConfig,
     InstanceEdgesDestinationConfig,
+    InstancesDestinationConfig,
     RawDestinationAlternativeConfig,
 ]
 
 
 @dataclass
 class QueryConfig:
     file: str
```

### Comparing `cognite_transformations_cli-2.3.8/cognite/transformations_cli/commands/deploy/transformation_types_legacy.py` & `cognite_transformations_cli-2.3.9/cognite/transformations_cli/commands/deploy/transformation_types_legacy.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.8/cognite/transformations_cli/commands/deploy/transformations_api.py` & `cognite_transformations_cli-2.3.9/cognite/transformations_cli/commands/deploy/transformations_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,24 +7,33 @@
     OidcCredentials,
     Transformation,
     TransformationDestination,
     TransformationNotification,
     TransformationSchedule,
     TransformationUpdate,
 )
-from cognite.client.data_classes.transformations.common import Edges, EdgeType, Nodes, SequenceRows, ViewInfo
+from cognite.client.data_classes.transformations.common import (
+    DataModelInfo,
+    Edges,
+    EdgeType,
+    Instances,
+    Nodes,
+    SequenceRows,
+    ViewInfo,
+)
 from cognite.client.exceptions import CogniteAPIError, CogniteDuplicatedError, CogniteNotFoundError
 
 from cognite.transformations_cli.commands.deploy.transformation_types import (
     ActionType,
     AuthConfig,
     DestinationConfig,
     DestinationConfigType,
     InstanceEdgesDestinationConfig,
     InstanceNodesDestinationConfig,
+    InstancesDestinationConfig,
     QueryConfig,
     RawDestinationAlternativeConfig,
     RawDestinationConfig,
     ReadWriteAuthentication,
     ScheduleConfig,
     SequenceRowsDestinationConfig,
     TransformationConfig,
@@ -110,14 +119,25 @@
                 destination.view.version,
             )
         edge_type = None
         if destination.edge_type:
             edge_type = EdgeType(destination.edge_type.space, destination.edge_type.external_id)
         return Edges(view, destination.instance_space, edge_type)
 
+    elif isinstance(destination, InstancesDestinationConfig):
+        data_model = None
+        if destination.data_model:
+            data_model = DataModelInfo(
+                destination.data_model.space,
+                destination.data_model.external_id,
+                destination.data_model.version,
+                destination.data_model.destination_type,
+                destination.data_model.destination_relationship_from_type,
+            )
+        return Instances(data_model, destination.instance_space)
     else:
         return TransformationDestination(destination.value)
 
 
 def to_query(conf_path: str, query: Union[str, QueryConfig]) -> str:
     try:
         dir_path = os.path.dirname(conf_path)
```

### Comparing `cognite_transformations_cli-2.3.8/cognite/transformations_cli/commands/jobs.py` & `cognite_transformations_cli-2.3.9/cognite/transformations_cli/commands/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.8/cognite/transformations_cli/commands/list.py` & `cognite_transformations_cli-2.3.9/cognite/transformations_cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.8/cognite/transformations_cli/commands/query.py` & `cognite_transformations_cli-2.3.9/cognite/transformations_cli/commands/query.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.8/cognite/transformations_cli/commands/run.py` & `cognite_transformations_cli-2.3.9/cognite/transformations_cli/commands/run.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.8/cognite/transformations_cli/commands/show.py` & `cognite_transformations_cli-2.3.9/cognite/transformations_cli/commands/show.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.8/cognite/transformations_cli/commands/utils.py` & `cognite_transformations_cli-2.3.9/cognite/transformations_cli/commands/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_transformations_cli-2.3.8/pyproject.toml` & `cognite_transformations_cli-2.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [tool.poetry]
 name = "cognite-transformations-cli"
-version = "2.3.8"
+version = "2.3.9"
+
 description = "A CLI for the Transformations service in CDF"
 authors = ["Mathias Lohne <mathias.lohne@cognite.com>", "Emel Varol <emel.varol@cognite.com>", "Einar Marstrander Omang <einar.omang@cognite.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cognitedata/transformations-cli"
 
 packages = [
```

### Comparing `cognite_transformations_cli-2.3.8/PKG-INFO` & `cognite_transformations_cli-2.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-transformations-cli
-Version: 2.3.8
+Version: 2.3.9
 Summary: A CLI for the Transformations service in CDF
 Home-page: https://github.com/cognitedata/transformations-cli
 License: Apache-2.0
 Author: Mathias Lohne
 Author-email: mathias.lohne@cognite.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

