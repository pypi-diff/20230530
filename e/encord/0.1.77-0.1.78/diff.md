# Comparing `tmp/encord-0.1.77.tar.gz` & `tmp/encord-0.1.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encord-0.1.77.tar", max compression
+gzip compressed data, was "encord-0.1.78.tar", max compression
```

## Comparing `encord-0.1.77.tar` & `encord-0.1.78.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0    11330 2023-05-23 12:12:07.482519 encord-0.1.77/LICENSE
--rw-r--r--   0        0        0     2595 2023-05-23 12:12:07.482519 encord-0.1.77/README.md
--rw-r--r--   0        0        0       84 2023-05-23 12:12:07.482519 encord-0.1.77/cord/__init__.py
--rw-r--r--   0        0        0      158 2023-05-23 12:12:07.498519 encord-0.1.77/encord/__init__.py
--rw-r--r--   0        0        0      214 2023-05-23 12:12:07.498519 encord-0.1.77/encord/_version.py
--rw-r--r--   0        0        0    49201 2023-05-23 12:12:07.498519 encord-0.1.77/encord/client.py
--rw-r--r--   0        0        0    10825 2023-05-23 12:12:07.498519 encord-0.1.77/encord/configs.py
--rw-r--r--   0        0        0        0 2023-05-23 12:12:07.498519 encord-0.1.77/encord/constants/__init__.py
--rw-r--r--   0        0        0      810 2023-05-23 12:12:07.498519 encord-0.1.77/encord/constants/enums.py
--rw-r--r--   0        0        0     3211 2023-05-23 12:12:07.498519 encord-0.1.77/encord/constants/model.py
--rw-r--r--   0        0        0     6068 2023-05-23 12:12:07.498519 encord-0.1.77/encord/constants/model_weights.py
--rw-r--r--   0        0        0     1119 2023-05-23 12:12:07.498519 encord-0.1.77/encord/constants/string_constants.py
--rw-r--r--   0        0        0        0 2023-05-23 12:12:07.498519 encord-0.1.77/encord/constants/test/__init__.py
--rw-r--r--   0        0        0      634 2023-05-23 12:12:07.498519 encord-0.1.77/encord/constants/test/test_enums.py
--rw-r--r--   0        0        0    16035 2023-05-23 12:12:07.498519 encord-0.1.77/encord/dataset.py
--rw-r--r--   0        0        0     6363 2023-05-23 12:12:07.498519 encord-0.1.77/encord/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-23 12:12:07.498519 encord-0.1.77/encord/http/__init__.py
--rw-r--r--   0        0        0     5329 2023-05-23 12:12:07.498519 encord-0.1.77/encord/http/bundle.py
--rw-r--r--   0        0        0      535 2023-05-23 12:12:07.498519 encord-0.1.77/encord/http/constants.py
--rw-r--r--   0        0        0     7234 2023-05-23 12:12:07.498519 encord-0.1.77/encord/http/error_utils.py
--rw-r--r--   0        0        0      103 2023-05-23 12:12:07.498519 encord-0.1.77/encord/http/limits.py
--rw-r--r--   0        0        0     7875 2023-05-23 12:12:07.498519 encord-0.1.77/encord/http/querier.py
--rw-r--r--   0        0        0      697 2023-05-23 12:12:07.498519 encord-0.1.77/encord/http/query_methods.py
--rw-r--r--   0        0        0     1719 2023-05-23 12:12:07.498519 encord-0.1.77/encord/http/request.py
--rw-r--r--   0        0        0     6182 2023-05-23 12:12:07.498519 encord-0.1.77/encord/http/utils.py
--rw-r--r--   0        0        0      340 2023-05-23 12:12:07.498519 encord-0.1.77/encord/objects/__init__.py
--rw-r--r--   0        0        0      145 2023-05-23 12:12:07.498519 encord-0.1.77/encord/objects/classification.py
--rw-r--r--   0        0        0    29709 2023-05-23 12:12:07.498519 encord-0.1.77/encord/objects/common.py
--rw-r--r--   0        0        0      172 2023-05-23 12:12:07.498519 encord-0.1.77/encord/objects/constants.py
--rw-r--r--   0        0        0     5631 2023-05-23 12:12:07.498519 encord-0.1.77/encord/objects/coordinates.py
--rw-r--r--   0        0        0     3419 2023-05-23 12:12:07.498519 encord-0.1.77/encord/objects/frames.py
--rw-r--r--   0        0        0    21407 2023-05-23 12:12:07.498519 encord-0.1.77/encord/objects/internal_helpers.py
--rw-r--r--   0        0        0   139937 2023-05-23 12:12:07.498519 encord-0.1.77/encord/objects/ontology_labels_impl.py
--rw-r--r--   0        0        0      137 2023-05-23 12:12:07.498519 encord-0.1.77/encord/objects/ontology_object.py
--rw-r--r--   0        0        0      148 2023-05-23 12:12:07.498519 encord-0.1.77/encord/objects/ontology_structure.py
--rw-r--r--   0        0        0      549 2023-05-23 12:12:07.498519 encord-0.1.77/encord/objects/project.py
--rw-r--r--   0        0        0     1240 2023-05-23 12:12:07.498519 encord-0.1.77/encord/objects/utils.py
--rw-r--r--   0        0        0     3430 2023-05-23 12:12:07.498519 encord-0.1.77/encord/ontology.py
--rw-r--r--   0        0        0        0 2023-05-23 12:12:07.498519 encord-0.1.77/encord/orm/__init__.py
--rw-r--r--   0        0        0      982 2023-05-23 12:12:07.498519 encord-0.1.77/encord/orm/api_key.py
--rw-r--r--   0        0        0     5377 2023-05-23 12:12:07.498519 encord-0.1.77/encord/orm/base_orm.py
--rw-r--r--   0        0        0      111 2023-05-23 12:12:07.498519 encord-0.1.77/encord/orm/cloud_integration.py
--rw-r--r--   0        0        0    32206 2023-05-23 12:12:07.498519 encord-0.1.77/encord/orm/dataset.py
--rw-r--r--   0        0        0      828 2023-05-23 12:12:07.498519 encord-0.1.77/encord/orm/dataset_with_user_role.py
--rw-r--r--   0        0        0      188 2023-05-23 12:12:07.498519 encord-0.1.77/encord/orm/formatter.py
--rw-r--r--   0        0        0     1146 2023-05-23 12:12:07.498519 encord-0.1.77/encord/orm/label_log.py
--rw-r--r--   0        0        0    11869 2023-05-23 12:12:07.498519 encord-0.1.77/encord/orm/label_row.py
--rw-r--r--   0        0        0     1577 2023-05-23 12:12:07.498519 encord-0.1.77/encord/orm/labeling_algorithm.py
--rw-r--r--   0        0        0     6687 2023-05-23 12:12:07.498519 encord-0.1.77/encord/orm/model.py
--rw-r--r--   0        0        0      745 2023-05-23 12:12:07.498519 encord-0.1.77/encord/orm/ontology.py
--rw-r--r--   0        0        0     8844 2023-05-23 12:12:07.498519 encord-0.1.77/encord/orm/project.py
--rw-r--r--   0        0        0      625 2023-05-23 12:12:07.498519 encord-0.1.77/encord/orm/project_api_key.py
--rw-r--r--   0        0        0      828 2023-05-23 12:12:07.498519 encord-0.1.77/encord/orm/project_with_user_role.py
--rw-r--r--   0        0        0        0 2023-05-23 12:12:07.498519 encord-0.1.77/encord/orm/test/__init__.py
--rw-r--r--   0        0        0      570 2023-05-23 12:12:07.498519 encord-0.1.77/encord/orm/test/test_dataset.py
--rw-r--r--   0        0        0    39203 2023-05-23 12:12:07.498519 encord-0.1.77/encord/project.py
--rw-r--r--   0        0        0        0 2023-05-23 12:12:07.498519 encord-0.1.77/encord/project_ontology/__init__.py
--rw-r--r--   0        0        0     1316 2023-05-23 12:12:07.498519 encord-0.1.77/encord/project_ontology/classification_attribute.py
--rw-r--r--   0        0        0      525 2023-05-23 12:12:07.502519 encord-0.1.77/encord/project_ontology/classification_option.py
--rw-r--r--   0        0        0      357 2023-05-23 12:12:07.502519 encord-0.1.77/encord/project_ontology/classification_type.py
--rw-r--r--   0        0        0      237 2023-05-23 12:12:07.502519 encord-0.1.77/encord/project_ontology/object_type.py
--rw-r--r--   0        0        0     9676 2023-05-23 12:12:07.502519 encord-0.1.77/encord/project_ontology/ontology.py
--rw-r--r--   0        0        0      630 2023-05-23 12:12:07.502519 encord-0.1.77/encord/project_ontology/ontology_classification.py
--rw-r--r--   0        0        0      683 2023-05-23 12:12:07.502519 encord-0.1.77/encord/project_ontology/ontology_object.py
--rw-r--r--   0        0        0    27840 2023-05-23 12:12:07.502519 encord-0.1.77/encord/user_client.py
--rw-r--r--   0        0        0        0 2023-05-23 12:12:07.502519 encord-0.1.77/encord/utilities/__init__.py
--rw-r--r--   0        0        0     4282 2023-05-23 12:12:07.502519 encord-0.1.77/encord/utilities/client_utilities.py
--rw-r--r--   0        0        0      253 2023-05-23 12:12:07.502519 encord-0.1.77/encord/utilities/common.py
--rw-r--r--   0        0        0     3270 2023-05-23 12:12:07.502519 encord-0.1.77/encord/utilities/label_utilities.py
--rw-r--r--   0        0        0      343 2023-05-23 12:12:07.502519 encord-0.1.77/encord/utilities/ontology_user.py
--rw-r--r--   0        0        0      578 2023-05-23 12:12:07.502519 encord-0.1.77/encord/utilities/project_user.py
--rw-r--r--   0        0        0      467 2023-05-23 12:12:07.502519 encord-0.1.77/encord/utilities/project_utilities.py
--rw-r--r--   0        0        0     1685 2023-05-23 12:12:07.502519 encord-0.1.77/pyproject.toml
--rw-r--r--   0        0        0     3778 1970-01-01 00:00:00.000000 encord-0.1.77/PKG-INFO
+-rw-r--r--   0        0        0    11330 2023-05-30 13:19:21.437542 encord-0.1.78/LICENSE
+-rw-r--r--   0        0        0     2037 2023-05-30 13:19:21.437542 encord-0.1.78/README.md
+-rw-r--r--   0        0        0       84 2023-05-30 13:19:21.437542 encord-0.1.78/cord/__init__.py
+-rw-r--r--   0        0        0      158 2023-05-30 13:19:21.453542 encord-0.1.78/encord/__init__.py
+-rw-r--r--   0        0        0      214 2023-05-30 13:19:21.453542 encord-0.1.78/encord/_version.py
+-rw-r--r--   0        0        0    49096 2023-05-30 13:19:21.453542 encord-0.1.78/encord/client.py
+-rw-r--r--   0        0        0    10843 2023-05-30 13:19:21.453542 encord-0.1.78/encord/configs.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:19:21.453542 encord-0.1.78/encord/constants/__init__.py
+-rw-r--r--   0        0        0      810 2023-05-30 13:19:21.453542 encord-0.1.78/encord/constants/enums.py
+-rw-r--r--   0        0        0     3293 2023-05-30 13:19:21.453542 encord-0.1.78/encord/constants/model.py
+-rw-r--r--   0        0        0     6068 2023-05-30 13:19:21.453542 encord-0.1.78/encord/constants/model_weights.py
+-rw-r--r--   0        0        0     1119 2023-05-30 13:19:21.453542 encord-0.1.78/encord/constants/string_constants.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:19:21.453542 encord-0.1.78/encord/constants/test/__init__.py
+-rw-r--r--   0        0        0      634 2023-05-30 13:19:21.453542 encord-0.1.78/encord/constants/test/test_enums.py
+-rw-r--r--   0        0        0    16035 2023-05-30 13:19:21.453542 encord-0.1.78/encord/dataset.py
+-rw-r--r--   0        0        0     6351 2023-05-30 13:19:21.453542 encord-0.1.78/encord/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:19:21.453542 encord-0.1.78/encord/http/__init__.py
+-rw-r--r--   0        0        0     5315 2023-05-30 13:19:21.453542 encord-0.1.78/encord/http/bundle.py
+-rw-r--r--   0        0        0      535 2023-05-30 13:19:21.453542 encord-0.1.78/encord/http/constants.py
+-rw-r--r--   0        0        0     7234 2023-05-30 13:19:21.453542 encord-0.1.78/encord/http/error_utils.py
+-rw-r--r--   0        0        0      103 2023-05-30 13:19:21.453542 encord-0.1.78/encord/http/limits.py
+-rw-r--r--   0        0        0     7916 2023-05-30 13:19:21.453542 encord-0.1.78/encord/http/querier.py
+-rw-r--r--   0        0        0      697 2023-05-30 13:19:21.453542 encord-0.1.78/encord/http/query_methods.py
+-rw-r--r--   0        0        0     1719 2023-05-30 13:19:21.453542 encord-0.1.78/encord/http/request.py
+-rw-r--r--   0        0        0     6182 2023-05-30 13:19:21.453542 encord-0.1.78/encord/http/utils.py
+-rw-r--r--   0        0        0      340 2023-05-30 13:19:21.453542 encord-0.1.78/encord/objects/__init__.py
+-rw-r--r--   0        0        0      182 2023-05-30 13:19:21.453542 encord-0.1.78/encord/objects/classification.py
+-rw-r--r--   0        0        0    29750 2023-05-30 13:19:21.453542 encord-0.1.78/encord/objects/common.py
+-rw-r--r--   0        0        0      149 2023-05-30 13:19:21.453542 encord-0.1.78/encord/objects/constants.py
+-rw-r--r--   0        0        0     5631 2023-05-30 13:19:21.453542 encord-0.1.78/encord/objects/coordinates.py
+-rw-r--r--   0        0        0     3419 2023-05-30 13:19:21.453542 encord-0.1.78/encord/objects/frames.py
+-rw-r--r--   0        0        0    21407 2023-05-30 13:19:21.453542 encord-0.1.78/encord/objects/internal_helpers.py
+-rw-r--r--   0        0        0   140605 2023-05-30 13:19:21.453542 encord-0.1.78/encord/objects/ontology_labels_impl.py
+-rw-r--r--   0        0        0      174 2023-05-30 13:19:21.453542 encord-0.1.78/encord/objects/ontology_object.py
+-rw-r--r--   0        0        0      185 2023-05-30 13:19:21.453542 encord-0.1.78/encord/objects/ontology_structure.py
+-rw-r--r--   0        0        0      549 2023-05-30 13:19:21.453542 encord-0.1.78/encord/objects/project.py
+-rw-r--r--   0        0        0     1240 2023-05-30 13:19:21.453542 encord-0.1.78/encord/objects/utils.py
+-rw-r--r--   0        0        0     3430 2023-05-30 13:19:21.453542 encord-0.1.78/encord/ontology.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:19:21.453542 encord-0.1.78/encord/orm/__init__.py
+-rw-r--r--   0        0        0      982 2023-05-30 13:19:21.453542 encord-0.1.78/encord/orm/api_key.py
+-rw-r--r--   0        0        0     5335 2023-05-30 13:19:21.453542 encord-0.1.78/encord/orm/base_orm.py
+-rw-r--r--   0        0        0      111 2023-05-30 13:19:21.457542 encord-0.1.78/encord/orm/cloud_integration.py
+-rw-r--r--   0        0        0    32204 2023-05-30 13:19:21.457542 encord-0.1.78/encord/orm/dataset.py
+-rw-r--r--   0        0        0      828 2023-05-30 13:19:21.457542 encord-0.1.78/encord/orm/dataset_with_user_role.py
+-rw-r--r--   0        0        0      175 2023-05-30 13:19:21.457542 encord-0.1.78/encord/orm/formatter.py
+-rw-r--r--   0        0        0     1146 2023-05-30 13:19:21.457542 encord-0.1.78/encord/orm/label_log.py
+-rw-r--r--   0        0        0    11869 2023-05-30 13:19:21.457542 encord-0.1.78/encord/orm/label_row.py
+-rw-r--r--   0        0        0     1577 2023-05-30 13:19:21.457542 encord-0.1.78/encord/orm/labeling_algorithm.py
+-rw-r--r--   0        0        0     6687 2023-05-30 13:19:21.457542 encord-0.1.78/encord/orm/model.py
+-rw-r--r--   0        0        0      823 2023-05-30 13:19:21.457542 encord-0.1.78/encord/orm/ontology.py
+-rw-r--r--   0        0        0     8885 2023-05-30 13:19:21.457542 encord-0.1.78/encord/orm/project.py
+-rw-r--r--   0        0        0      625 2023-05-30 13:19:21.457542 encord-0.1.78/encord/orm/project_api_key.py
+-rw-r--r--   0        0        0      828 2023-05-30 13:19:21.457542 encord-0.1.78/encord/orm/project_with_user_role.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:19:21.457542 encord-0.1.78/encord/orm/test/__init__.py
+-rw-r--r--   0        0        0      570 2023-05-30 13:19:21.457542 encord-0.1.78/encord/orm/test/test_dataset.py
+-rw-r--r--   0        0        0    39203 2023-05-30 13:19:21.457542 encord-0.1.78/encord/project.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:19:21.457542 encord-0.1.78/encord/project_ontology/__init__.py
+-rw-r--r--   0        0        0     1316 2023-05-30 13:19:21.457542 encord-0.1.78/encord/project_ontology/classification_attribute.py
+-rw-r--r--   0        0        0      525 2023-05-30 13:19:21.457542 encord-0.1.78/encord/project_ontology/classification_option.py
+-rw-r--r--   0        0        0      357 2023-05-30 13:19:21.457542 encord-0.1.78/encord/project_ontology/classification_type.py
+-rw-r--r--   0        0        0      237 2023-05-30 13:19:21.457542 encord-0.1.78/encord/project_ontology/object_type.py
+-rw-r--r--   0        0        0     9676 2023-05-30 13:19:21.457542 encord-0.1.78/encord/project_ontology/ontology.py
+-rw-r--r--   0        0        0      630 2023-05-30 13:19:21.457542 encord-0.1.78/encord/project_ontology/ontology_classification.py
+-rw-r--r--   0        0        0      683 2023-05-30 13:19:21.457542 encord-0.1.78/encord/project_ontology/ontology_object.py
+-rw-r--r--   0        0        0    27854 2023-05-30 13:19:21.457542 encord-0.1.78/encord/user_client.py
+-rw-r--r--   0        0        0        0 2023-05-30 13:19:21.457542 encord-0.1.78/encord/utilities/__init__.py
+-rw-r--r--   0        0        0     4282 2023-05-30 13:19:21.457542 encord-0.1.78/encord/utilities/client_utilities.py
+-rw-r--r--   0        0        0      253 2023-05-30 13:19:21.457542 encord-0.1.78/encord/utilities/common.py
+-rw-r--r--   0        0        0     3270 2023-05-30 13:19:21.457542 encord-0.1.78/encord/utilities/label_utilities.py
+-rw-r--r--   0        0        0      343 2023-05-30 13:19:21.457542 encord-0.1.78/encord/utilities/ontology_user.py
+-rw-r--r--   0        0        0      578 2023-05-30 13:19:21.457542 encord-0.1.78/encord/utilities/project_user.py
+-rw-r--r--   0        0        0      467 2023-05-30 13:19:21.457542 encord-0.1.78/encord/utilities/project_utilities.py
+-rw-r--r--   0        0        0     1944 2023-05-30 13:19:21.457542 encord-0.1.78/pyproject.toml
+-rw-r--r--   0        0        0     3220 1970-01-01 00:00:00.000000 encord-0.1.78/PKG-INFO
```

### Comparing `encord-0.1.77/LICENSE` & `encord-0.1.78/LICENSE`

 * *Files identical despite different names*

### Comparing `encord-0.1.77/encord/client.py` & `encord-0.1.78/encord/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,25 +211,21 @@
 
     def __getattr__(self, name):
         """Overriding __getattr__."""
         value = self.__dict__.get(name)
         if not value:
             self_type = type(self).__name__
             if self_type == "CordClientDataset" and name in EncordClientProject.__dict__.keys():
-                raise encord.exceptions.EncordException(
-                    message=("{} is implemented in Projects, not Datasets.".format(name))
-                )
+                raise encord.exceptions.EncordException(message=f"{name} is implemented in Projects, not Datasets.")
             elif self_type == "CordClientProject" and name in EncordClientDataset.__dict__.keys():
-                raise encord.exceptions.EncordException(
-                    message=("{} is implemented in Datasets, not Projects.".format(name))
-                )
+                raise encord.exceptions.EncordException(message=f"{name} is implemented in Datasets, not Projects.")
             elif name == "items":
                 pass
             else:
-                raise encord.exceptions.EncordException(message="{} is not implemented.".format(name))
+                raise encord.exceptions.EncordException(message=f"{name} is not implemented.")
         return value
 
     def get_cloud_integrations(self) -> List[CloudIntegration]:
         return self._querier.get_multiple(CloudIntegration)
 
 
 CordClient = EncordClient
@@ -418,15 +414,15 @@
             res = upload_video_to_encord(signed_urls[0], title, self._querier)
             if res:
                 logger.info("Upload complete.")
                 return res
             else:
                 raise encord.exceptions.EncordException(message="An error has occurred during video upload.")
         else:
-            raise encord.exceptions.EncordException(message="{} does not point to a file.".format(file_path))
+            raise encord.exceptions.EncordException(message=f"{file_path} does not point to a file.")
 
     def create_image_group(
         self,
         file_paths: Iterable[str],
         max_workers: Optional[int] = None,
         cloud_upload_settings: CloudUploadSettings = CloudUploadSettings(),
         title: Optional[str] = None,
@@ -434,15 +430,15 @@
         create_video: bool = True,
     ):
         """
         This function is documented in :meth:`encord.dataset.Dataset.create_image_group`.
         """
         for file_path in file_paths:
             if not os.path.exists(file_path):
-                raise encord.exceptions.EncordException(message="{} does not point to a file.".format(file_path))
+                raise encord.exceptions.EncordException(message=f"{file_path} does not point to a file.")
 
         successful_uploads = upload_to_signed_url_list(
             file_paths, self._config, self._querier, Images, cloud_upload_settings=cloud_upload_settings
         )
         if not successful_uploads:
             raise encord.exceptions.EncordException("All image uploads failed. Image group was not created.")
         upload_images_to_encord(successful_uploads, self._querier)
@@ -455,15 +451,15 @@
                 "image_group_title": title,
                 "create_video": create_video,
             },
         )
 
         if res:
             titles = [video_data.get("title") for video_data in res]
-            logger.info("Upload successful! {} created.".format(titles))
+            logger.info(f"Upload successful! {titles} created.")
             return res
         else:
             raise encord.exceptions.EncordException(message="An error has occurred during image group creation.")
 
     def create_dicom_series(
         self,
         file_paths: List[str],
@@ -471,15 +467,15 @@
         cloud_upload_settings: CloudUploadSettings = CloudUploadSettings(),
     ):
         """
         This function is documented in :meth:`encord.dataset.Dataset.create_dicom_series`.
         """
         for file_path in file_paths:
             if not os.path.exists(file_path):
-                raise encord.exceptions.EncordException(message="{} does not point to a file.".format(file_path))
+                raise encord.exceptions.EncordException(message=f"{file_path} does not point to a file.")
 
         successful_uploads = upload_to_signed_url_list(
             file_paths=file_paths,
             config=self._config,
             querier=self._querier,
             orm_class=DicomSeries,
             cloud_upload_settings=cloud_upload_settings,
@@ -579,21 +575,21 @@
         """
         This function is documented in :meth:`encord.dataset.Dataset.add_private_data_to_dataset_start`.
         """
         if isinstance(private_files, dict):
             files = private_files
         elif isinstance(private_files, str):
             if os.path.exists(private_files):
-                text_contents = Path(private_files).read_text()
+                text_contents = Path(private_files).read_text(encoding="utf-8")
             else:
                 text_contents = private_files
 
             files = json.loads(text_contents)
         elif isinstance(private_files, Path):
-            text_contents = private_files.read_text()
+            text_contents = private_files.read_text(encoding="utf-8")
             files = json.loads(text_contents)
         elif isinstance(private_files, typing.TextIO):
             text_contents = private_files.read()
             files = json.loads(text_contents)
         else:
             raise ValueError(f"Type [{type(private_files)}] of argument private_files is not supported")
 
@@ -652,15 +648,15 @@
 
                 files_finished_count = res.units_done_count + res.units_error_count
                 files_total_count = res.units_pending_count + res.units_done_count + res.units_error_count
 
                 if files_finished_count != files_total_count:
                     print(f"Processed {files_finished_count}/{files_total_count} files")
                 else:
-                    print(f"Processed all files, dataset data linking and task creation is performed, please wait")
+                    print("Processed all files, dataset data linking and task creation is performed, please wait")
 
                 failed_requests_count = 0
             except requests.exceptions.RequestException:
                 failed_requests_count += 1
 
                 if failed_requests_count >= LONG_POLLING_RESPONSE_RETRY_N:
                     raise
@@ -1291,15 +1287,15 @@
 
         Returns:
             bool
         """
         payload = {"editor": ontology.to_dict()}
         return self._querier.basic_setter(OrmProject, uid=None, payload=payload)
 
-    def workflow_reopen(self, label_hashes: list[str]) -> None:
+    def workflow_reopen(self, label_hashes: List[str]) -> None:
         """
         This function is documented in :meth:`encord.objects.LabelRowV2.workflow_reopen`.
         """
 
         # Workaround to make basic_setter generate proper api call
         class LabelWorkflowGraphNode:
             pass
```

### Comparing `encord-0.1.77/encord/configs.py` & `encord-0.1.78/encord/configs.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,15 +213,15 @@
         ssh_file = os.path.abspath(os.path.expanduser(ssh_file))
         if not os.path.exists(ssh_file):
             raise ResourceNotFoundError(
                 f"SSH key file `{ssh_file}` which is defined in the `{_ENCORD_SSH_KEY_FILE}` environment variable does not seem to exist. "
                 f"Failed to load private ssh key."
             )
 
-        with open(ssh_file) as f:
+        with open(ssh_file, encoding="ascii") as f:
             return f.read()
 
     # == 2. Look for raw key
     raw_ssh_key = os.environ.get(_ENCORD_SSH_KEY)
     if raw_ssh_key is None:
         raise ResourceNotFoundError(
             f"Neither of the environment variables {_ENCORD_SSH_KEY_FILE} or {_ENCORD_SSH_KEY} were found. "
```

### Comparing `encord-0.1.77/encord/constants/enums.py` & `encord-0.1.78/encord/constants/enums.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.77/encord/constants/model.py` & `encord-0.1.78/encord/constants/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 class Device(Enum):
     CUDA = "cuda"
     CPU = "cpu"
 
     @classmethod
     def has_value(cls, value) -> bool:
+        # pylint: disable-next=no-member
         return value in cls._value2member_map_
 
 
 class AutomationModels(Enum):
     FAST_AI = "fast_ai"
     RESNET18 = "resnet18"
     RESNET34 = "resnet34"
@@ -76,14 +77,15 @@
             Model types that can be used with polygon type ``<feature_node_hashes>``
             from the ``objects`` part of the project ontology.
         """
         return {AutomationModels.MASK_RCNN}
 
     @classmethod
     def has_value(cls, value) -> bool:
+        # pylint: disable-next=no-member
         return value in cls._value2member_map_
 
 
 # For backward compatibility
 FAST_AI = cast(str, AutomationModels.FAST_AI.value)
 RESNET18 = cast(str, AutomationModels.RESNET18.value)
 RESNET34 = cast(str, AutomationModels.RESNET34.value)
```

### Comparing `encord-0.1.77/encord/constants/model_weights.py` & `encord-0.1.78/encord/constants/model_weights.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.77/encord/constants/string_constants.py` & `encord-0.1.78/encord/constants/string_constants.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.77/encord/constants/test/test_enums.py` & `encord-0.1.78/encord/constants/test/test_enums.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.77/encord/dataset.py` & `encord-0.1.78/encord/dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.77/encord/exceptions.py` & `encord-0.1.78/encord/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
-import time
 from dataclasses import dataclass, field, fields
 from datetime import datetime, timezone
 from typing import Optional
 
 
 @dataclass
 class ExceptionContext:
```

### Comparing `encord-0.1.77/encord/http/bundle.py` & `encord-0.1.78/encord/http/bundle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
-from dataclasses import asdict, dataclass, field
+from dataclasses import asdict, dataclass
 from functools import reduce
-from typing import Callable, Dict, Generator, Generic, List, Optional, Tuple, TypeVar
+from typing import Callable, Dict, Generator, Generic, List, Optional, TypeVar
 
 log = logging.getLogger(__name__)
 
 T = TypeVar("T")
 R = TypeVar("R")
```

### Comparing `encord-0.1.77/encord/http/constants.py` & `encord-0.1.78/encord/http/constants.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.77/encord/http/error_utils.py` & `encord-0.1.78/encord/http/error_utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.77/encord/http/querier.py` & `encord-0.1.78/encord/http/querier.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,14 +190,15 @@
             context = self._exception_context_from_response(res)
 
             try:
                 res_json = res.json()
             except Exception as e:
                 raise RequestException(f"Error parsing JSON response: {res.text}", context=context) from e
 
+        # pylint: disable-next=no-member
         if res_json.get("status") != requests.codes.ok:
             response = res_json.get("response")
             extra_payload = res_json.get("payload")
             check_error_response(response, context, extra_payload)
 
         return res_json.get("response"), context
```

### Comparing `encord-0.1.77/encord/http/query_methods.py` & `encord-0.1.78/encord/http/query_methods.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.77/encord/http/request.py` & `encord-0.1.78/encord/http/request.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.77/encord/http/utils.py` & `encord-0.1.78/encord/http/utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.77/encord/objects/common.py` & `encord-0.1.78/encord/objects/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,14 +162,15 @@
         ret["featureNodeHash"] = self.feature_node_hash
         ret["required"] = self.required
         ret["dynamic"] = self.dynamic
 
         return ret
 
     def _encode_options(self) -> Optional[list]:
+        # pylint: disable-next=no-member
         if not self.has_options_field() or not self.options:
             return None
 
         self: OptionAttribute
 
         ret = list()
         for option in self.options:
```

### Comparing `encord-0.1.77/encord/objects/coordinates.py` & `encord-0.1.78/encord/objects/coordinates.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.77/encord/objects/frames.py` & `encord-0.1.78/encord/objects/frames.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.77/encord/objects/internal_helpers.py` & `encord-0.1.78/encord/objects/internal_helpers.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.77/encord/objects/ontology_labels_impl.py` & `encord-0.1.78/encord/objects/ontology_labels_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     Optional,
     Sequence,
     Set,
     Tuple,
     Type,
     TypeVar,
     Union,
-    overload,
 )
 from uuid import uuid4
 
 from dateutil.parser import parse
 
 from encord.client import EncordClientProject
 from encord.client import LabelRow as OrmLabelRow
@@ -36,16 +35,14 @@
     LABEL_ROW_BUNDLE_SAVE_LIMIT,
 )
 from encord.objects.common import (
     Attribute,
     AttributeClasses,
     AttributeTypes,
     ChecklistAttribute,
-    FlatOption,
-    NestableOption,
     Option,
     OptionClasses,
     OptionTypes,
     RadioAttribute,
     Shape,
     TextAttribute,
     _add_attribute,
@@ -389,25 +386,36 @@
         self._static_answer_map: Dict[str, Answer] = _get_static_answer_map(self._ontology_classification.attributes)
         # feature_node_hash of attribute to the answer.
 
         self._frames_to_data: Dict[int, ClassificationInstance.FrameData] = defaultdict(self.FrameData)
 
     @property
     def classification_hash(self) -> str:
+        """A unique identifier for the classification instance."""
         return self._classification_hash
 
     @classification_hash.setter
     def classification_hash(self, v: Any) -> NoReturn:
         raise LabelRowError("Cannot set the object hash on an instantiated label object.")
 
     @property
     def ontology_item(self) -> Classification:
         return deepcopy(self._ontology_classification)
 
     @property
+    def classification_name(self) -> str:
+        """Classification name from the project ontology"""
+        return self._ontology_classification.attributes[0].name
+
+    @property
+    def feature_hash(self) -> str:
+        """Feature node hash from the project ontology"""
+        return self._ontology_classification.feature_node_hash
+
+    @property
     def _last_frame(self) -> Union[int, float]:
         if self._parent is None or self._parent.data_type is DataType.DICOM:
             return float("inf")
         else:
             return self._parent.number_of_frames
 
     def is_assigned_to_label_row(self) -> bool:
@@ -856,15 +864,15 @@
                 f"frame per LabelRowV2."
             )
 
     def __repr__(self):
         return (
             f"ClassificationInstance(classification_hash={self.classification_hash}, "
             f"classification_name={self._ontology_classification.attributes[0].name}, "
-            f"object_feature_hash={self._ontology_classification.feature_node_hash})"
+            f"feature_hash={self._ontology_classification.feature_node_hash})"
         )
 
     def __lt__(self, other) -> bool:
         return self.classification_hash < other.classification_hash
 
 
 @dataclass
@@ -2132,15 +2140,15 @@
         elif "polygon" in frame_object_label:
             return PolygonCoordinates.from_dict(frame_object_label)
         elif "point" in frame_object_label:
             return PointCoordinate.from_dict(frame_object_label)
         elif "polyline" in frame_object_label:
             return PolylineCoordinates.from_dict(frame_object_label)
         elif "skeleton" in frame_object_label:
-            raise NotImplementedError(f"Got a skeleton object, which is not supported yet")
+            raise NotImplementedError("Got a skeleton object, which is not supported yet")
         else:
             raise NotImplementedError(f"Getting coordinates for `{frame_object_label}` is not supported yet.")
 
     def _add_classification_instances_from_classifications(
         self, classifications_list: List[dict], classification_answers: dict, frame: int
     ):
         for frame_classification_label in classifications_list:
@@ -2247,14 +2255,24 @@
         return self._object_hash
 
     @property
     def ontology_item(self) -> Any:
         return deepcopy(self._ontology_object)
 
     @property
+    def feature_hash(self) -> str:
+        """Feature node hash from the project ontology"""
+        return self._ontology_object.feature_node_hash
+
+    @property
+    def object_name(self) -> str:
+        """Object name from the project ontology"""
+        return self._ontology_object.name
+
+    @property
     def _last_frame(self) -> Union[int, float]:
         if self._parent is None or self._parent.data_type is DataType.DICOM:
             return float("inf")
         else:
             return self._parent.number_of_frames
 
     def get_answer(
@@ -2790,15 +2808,15 @@
 
     def _get_all_dynamic_answers(self) -> List[Tuple[Answer, Ranges]]:
         return self._dynamic_answer_manager.get_all_answers()
 
     def __repr__(self):
         return (
             f"ObjectInstance(object_hash={self._object_hash}, object_name={self._ontology_object.name}, "
-            f"object_feature_hash={self._ontology_object.feature_node_hash})"
+            f"feature_hash={self._ontology_object.feature_node_hash})"
         )
 
     def __hash__(self) -> int:
         return hash(id(self))
 
     def __lt__(self, other: ObjectInstance) -> bool:
         return self._object_hash < other._object_hash
@@ -2941,15 +2959,15 @@
 
     def __hash__(self) -> int:
         return hash(id(self))
 
 
 def check_coordinate_type(coordinates: Coordinates, ontology_object: Object) -> None:
     expected_coordinate_type = ACCEPTABLE_COORDINATES_FOR_ONTOLOGY_ITEMS[ontology_object.shape]
-    if type(coordinates) != expected_coordinate_type:
+    if not isinstance(coordinates, expected_coordinate_type):
         raise LabelRowError(
             f"Expected a coordinate of type `{expected_coordinate_type}`, but got type `{type(coordinates)}`."
         )
 
 
 AVAILABLE_COLORS = (
     "#D33115",
```

### Comparing `encord-0.1.77/encord/objects/project.py` & `encord-0.1.78/encord/objects/project.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.77/encord/objects/utils.py` & `encord-0.1.78/encord/objects/utils.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.77/encord/ontology.py` & `encord-0.1.78/encord/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.77/encord/orm/api_key.py` & `encord-0.1.78/encord/orm/api_key.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.77/encord/orm/base_orm.py` & `encord-0.1.78/encord/orm/base_orm.py`

 * *Files 10% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                         real_v = datetime.datetime.strptime(v, "%Y-%m-%d %H:%M:%S")
                         value[k] = real_v
                     elif dict in types:
                         value[k] = v
             super().__init__(**value)
         except Exception as e:
             logger.error("Error init", exc_info=True)
-            raise Exception("Convert failed {}".format(str(e)))
+            raise Exception(f"Convert failed {e}")
 
     def __getattr__(self, name):
         """
         Override attribute method for easy access of field value.
         To be used instead of ["attr"].
         Return None if there is no such attribute
         :param name:
@@ -74,27 +74,27 @@
         """
         if name in self:
             try:
                 return self[name]
             except KeyError:
                 return None
         else:
-            raise AttributeError("Attribute does not exist: {}".format(name))
+            raise AttributeError(f"Attribute does not exist: {name}")
 
     def __setattr__(self, name, value):
         """
         Strict attribute name and type check.
         :param name:
         :param value:
         :return:
         """
         if name in self.DB_FIELDS and (value is None or isinstance(value, self.DB_FIELDS[name])):
             self[name] = value
         else:
-            raise AttributeError("Attribute name or type not match: {}".format(name))
+            raise AttributeError(f"Attribute name or type not match: {name}")
 
     def __delattr__(self, name):
         if name in self and name in self.DB_FIELDS:
             del self[name]
         else:
             super().__delattr__(self, name)
 
@@ -151,9 +151,9 @@
         values = []
         for item in iter_:
             try:
                 v = self.BASE_ORM_TYPE(item)
                 values.append(v)
             except Exception as e:
                 logger.error("Error init", exc_info=True)
-                raise Exception("Convert failed {}".format(str(e)))
+                raise Exception(f"Convert failed {e}")
         super().__init__(values)
```

### Comparing `encord-0.1.77/encord/orm/dataset.py` & `encord-0.1.78/encord/orm/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -419,15 +419,15 @@
                     "client_metadata": client_metadata,
                 }
             }
             res = self["_querier"].basic_getter(DataRow, uid=self.uid, payload=payload)
             self._update_current_class(res)
 
         else:
-            raise EncordException(f"Could not fetch data. The DataRow is in an invalid state.")
+            raise EncordException("Could not fetch data. The DataRow is in an invalid state.")
 
     def save(self) -> None:
         """
         Sync local state to the server, if updates are made. This is a blocking function.
 
         The newest values from the Encord server will update the current :class:`.DataRow` object.
         """
@@ -441,15 +441,15 @@
             if res:
                 self._compare_upload_payload(res, payload)
                 data_row_dict = res["data_row"]
                 self._update_current_class(DataRow.from_dict(data_row_dict))
             else:
                 raise EncordException(f"Could not upload data for DataRow with uid: {self.uid}")
         else:
-            raise EncordException(f"Could not upload data. The DataRow is in an invalid state.")
+            raise EncordException("Could not upload data. The DataRow is in an invalid state.")
 
     @classmethod
     def from_dict(cls, json_dict: Dict) -> DataRow:
         data_type = DataType.from_upper_case_string(json_dict["data_type"])
 
         return DataRow(
             uid=json_dict["data_hash"],
```

### Comparing `encord-0.1.77/encord/orm/dataset_with_user_role.py` & `encord-0.1.78/encord/orm/dataset_with_user_role.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.77/encord/orm/label_log.py` & `encord-0.1.78/encord/orm/label_log.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.77/encord/orm/label_row.py` & `encord-0.1.78/encord/orm/label_row.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.77/encord/orm/labeling_algorithm.py` & `encord-0.1.78/encord/orm/labeling_algorithm.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.77/encord/orm/model.py` & `encord-0.1.78/encord/orm/model.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.77/encord/orm/ontology.py` & `encord-0.1.78/encord/orm/ontology.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,12 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 from __future__ import annotations
 
+# pylint: disable=unused-import
 from encord.objects.ontology_labels_impl import (
     DATETIME_STRING_FORMAT,
     Ontology,
     OntologyUserRole,
 )
+
+# Importing here for backwards compatibility
```

### Comparing `encord-0.1.77/encord/orm/project.py` & `encord-0.1.78/encord/orm/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,14 +257,15 @@
 class StringEnum(Enum):
     """
     Use this enum class if you need the helper that creates the enum instance from a string.
     """
 
     @classmethod
     def from_string(cls, string: str) -> Optional["StringEnum"]:
+        # pylint: disable-next=no-member
         return cls._value2member_map_.get(string)
 
 
 class ReviewMode(StringEnum):
     """
     UNLABELLED:
         The labels are added to the images. However, the one person must still go over
```

### Comparing `encord-0.1.77/encord/orm/project_api_key.py` & `encord-0.1.78/encord/orm/project_api_key.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.77/encord/orm/project_with_user_role.py` & `encord-0.1.78/encord/orm/project_with_user_role.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.77/encord/orm/test/test_dataset.py` & `encord-0.1.78/encord/orm/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.77/encord/project.py` & `encord-0.1.78/encord/project.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.77/encord/project_ontology/classification_attribute.py` & `encord-0.1.78/encord/project_ontology/classification_attribute.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.77/encord/project_ontology/classification_option.py` & `encord-0.1.78/encord/project_ontology/classification_option.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.77/encord/project_ontology/ontology.py` & `encord-0.1.78/encord/project_ontology/ontology.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.77/encord/project_ontology/ontology_classification.py` & `encord-0.1.78/encord/project_ontology/ontology_classification.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.77/encord/project_ontology/ontology_object.py` & `encord-0.1.78/encord/project_ontology/ontology_object.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.77/encord/user_client.py` & `encord-0.1.78/encord/user_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from enum import Enum
 from pathlib import Path
 from typing import Dict, List, Optional, Tuple, Union
 
 import dateutil
 
 # add this for backward compatible class comparisons
+# pylint: disable-next=import-error
 from cord.utilities.client_utilities import LocalImport as CordLocalImport
 from encord.client import EncordClient, EncordClientDataset, EncordClientProject
 from encord.configs import SshConfig, UserConfig, get_env_ssh_key
 from encord.constants.string_constants import TYPE_DATASET, TYPE_ONTOLOGY, TYPE_PROJECT
 from encord.dataset import Dataset
 from encord.http.constants import DEFAULT_REQUESTS_SETTINGS, RequestsSettings
 from encord.http.querier import Querier
@@ -391,15 +392,15 @@
             CvatImporterSuccess: If the project was successfully imported.
             CvatImporterError: If the project could not be imported.
 
         Raises:
             ValueError:
                 If the CVAT directory has an invalid format.
         """
-        if not (type(import_method) == LocalImport or type(import_method) == CordLocalImport):
+        if not isinstance(import_method, (LocalImport, CordLocalImport)):
             raise ValueError("Only local imports are currently supported ")
 
         cvat_directory_path = import_method.file_path
 
         directory_path = Path(cvat_directory_path)
         images_directory_path = directory_path.joinpath("images")
         if images_directory_path not in list(directory_path.iterdir()):
@@ -468,15 +469,15 @@
             images = self.__get_recursive_image_paths(images_directory_path)
         else:
             raise ValueError(
                 f"Received an unexpected response `{project_info}` from the server. Project import aborted."
             )
 
         if not images:
-            raise ValueError(f"No images found in the provided data folder.")
+            raise ValueError("No images found in the provided data folder.")
         return images, used_base_path
 
     @staticmethod
     def __get_recursive_image_paths(images_directory_path: Path) -> List[Path]:
         """Recursively get all the images in all the sub folders."""
         ret = []
         for file in images_directory_path.glob("**/*"):
```

### Comparing `encord-0.1.77/encord/utilities/client_utilities.py` & `encord-0.1.78/encord/utilities/client_utilities.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.77/encord/utilities/label_utilities.py` & `encord-0.1.78/encord/utilities/label_utilities.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.77/encord/utilities/project_user.py` & `encord-0.1.78/encord/utilities/project_user.py`

 * *Files identical despite different names*

### Comparing `encord-0.1.77/pyproject.toml` & `encord-0.1.78/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "encord"
-version = "0.1.77"
+version = "0.1.78"
 description = "Encord Python SDK Client"
 authors = ["Cord Technologies Limited <hello@encord.com>"]
 license = "Apache Software License"
 keywords = ["cord", "encord"]
 packages = [
     { include = "cord"},
     { include = "encord"},
@@ -38,14 +38,16 @@
 prettyprinter = "0.18.0"
 isort = "^5.10.1"
 pydata-sphinx-theme = "^0.8.1"
 Pillow = "^9.1.0"
 sphinx-gallery = "^0.10.1"
 deepdiff = "^6.2.1"
 types-requests = "^2.25.0"
+pylint = "^2.13.9"
+autoflake = "^2.1.1"
 
 [build-system]
 requires = ["poetry-core>=1.3.2"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
@@ -59,7 +61,17 @@
 [tool.pylint.'MASTER']
 ignore = "tests"
 
 [tool.pylint.'MESSAGES CONTROL']
 max-line-length = 120
 disable = "all"
 enable = "C0123, C0200, C0209, E0401, E0602, E1101, E1205, W0611, W0621, W1309, W1404, W1514"
+
+[tool.autoflake]
+check = false
+expand-star-imports = true
+ignore-init-module-imports = true
+in-place = true
+recursive = true
+remove-all-unused-imports = true
+remove-duplicate-keys = true
+remove-unused-variables = true
```

### Comparing `encord-0.1.77/PKG-INFO` & `encord-0.1.78/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encord
-Version: 0.1.77
+Version: 0.1.78
 Summary: Encord Python SDK Client
 Home-page: https://github.com/encord-team/encord-client-python
 License: Apache Software License
 Keywords: cord,encord
 Author: Cord Technologies Limited
 Author-email: hello@encord.com
 Requires-Python: >=3.7,<4.0
@@ -24,80 +24,66 @@
 Requires-Dist: tqdm (>=4.32.1,<5.0.0)
 Project-URL: Documentation, https://python.docs.encord.com/
 Project-URL: Repository, https://github.com/encord-team/encord-client-python
 Description-Content-Type: text/markdown
 
 <h1 align="center">
   <p align="center">Encord Python API Client</p>
-  <a href="https://encord.com"><img src="./docs/_static/logo.svg" width="100" alt="Cord logo"/></a>
+  <a href="https://encord.com">
+    <img src="./docs/_static/logo.svg" width="100" alt="Cord logo"/>
+  </a>
 </h1>
 
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
-***The data engine for computer vision***
+# The data engine for computer vision
 
 ## 💻 Features
 
 - Minimal low-level Python client that allows you to interact with Encord's API
-- Supports Python: `3.7`, `3.8`, `3.9`, and `3.10`
+- Supports Python: `3.7`, `3.8`, `3.9`, `3.10` and `3.11`
 
 ## ✨ Relevant Links
+
 * [Encord website](https://encord.com)
 * [Encord web app](https://app.encord.com)
 * [Encord documentation](https://docs.encord.com)
 
 ## 💡 Getting Started
 
 For full documentation, please visit [Encord Python SDK](https://python.docs.encord.com/).
 
 First, install Encord Python API Client using the [pip](https://pip.pypa.io/en/stable/installing) package manager:
 
 ```bash
 pip install encord
 ```
 
-Then, create an API key for authentication via the [Encord web app](https://app.encord.com). Pass the resource ID and API key as environment variables or pass them explicitly when you initialise the EncordClient object.
-
-```bash
-export ENCORD_PROJECT_ID="<project_id>"
-export ENCORD_API_KEY="<project_api_key>"
-```
-
-Passing the resource ID and API key as environment variables, you can initialise the Encord client directly.
-
-```python
-from encord.client import EncordClient
-
-client = EncordClient.initialise()
-```
+Then, generate an public-private key pair, and upload the public key to [Encord website](https://www.encord.com/).
+Detailed guide can be found in the [dedicated manual](https://docs.encord.com/admins/settings/public-keys/).
 
-If you want to avoid setting environment variables, you can initialise the Encord client by passing the resource ID and API key as strings.
+Passing the private key to the factory, you can initialise the Encord client directly.
 
 ```python
-from encord.client import EncordClient
+from encord import EncordUserClient
 
-client = EncordClient.initialise("<resource_id>", "<resource_api_key>")
+user_client = EncordUserClient.create_with_ssh_private_key(
+    "<your_private_key_content>",
+    password="<your_private_key_password_if_set_on_key_generation>",
+)
 ```
 
-If you wish to instantiate several client objects and avoid passing parameters each time, you can instantiate a EncordConfig object, pass the resource ID and API key as strings, and initialise the client with the config object.
+Once you have instantiated an Encord client, it is easy to fetch a project information and start
+working with the platform.
 
 ```py
-from encord.client import EncordClient
-from encord.client import EncordConfig
-
-config = EncordConfig("<resource_id>", "<resource_api_key>")
-client = EncordClient.initialise_with_config(config)
+project = user_client.get_project("<project_hash>")
+label_rows = project.list_label_rows_v2()
 ```
 
-Once you have instantiated an Encord client, it is easy to fetch information associated with the given resource ID.
-
-```py
-from encord.client import EncordClient
-
-client = EncordClient.initialise()
-project = client.get_project()
-```
+For detailed examples and API reference please refer to [Encord SDK documentation](https://python.docs.encord.com/)
 
 ## 🐛 Troubleshooting
 
-Please report bugs to [GitHub Issues](https://github.com/encord-team/encord-client-python/issues). Just make sure you read the [Encord documentation](https://docs.encord.com) and search for related issues first.
+Please report bugs to the [GitHub Issues](https://github.com/encord-team/encord-client-python/issues).
+Just make sure you read the [Encord documentation](https://docs.encord.com) and search for related issues first.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: encord Version: 0.1.77 Summary: Encord Python SDK
+Metadata-Version: 2.1 Name: encord Version: 0.1.78 Summary: Encord Python SDK
 Client Home-page: https://github.com/encord-team/encord-client-python License:
 Apache Software License Keywords: cord,encord Author: Cord Technologies Limited
 Author-email: hello@encord.com Requires-Python: >=3.7,<4.0 Classifier: License
 :: OSI Approved :: Apache Software License Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
@@ -12,37 +12,29 @@
 (>=6.1.0,<7.0.0) ; python_version < "3.8" Requires-Dist: python-dateutil
 (>=2.8.2,<3.0.0) Requires-Dist: requests (>=2.25.0,<3.0.0) Requires-Dist: tqdm
 (>=4.32.1,<5.0.0) Project-URL: Documentation, https://python.docs.encord.com/
 Project-URL: Repository, https://github.com/encord-team/encord-client-python
 Description-Content-Type: text/markdown
                ****** Encord Python API Client[Cord_logo] ******
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https:
-//opensource.org/licenses/Apache-2.0) ***The data engine for computer vision***
-## ð» Features - Minimal low-level Python client that allows you to interact
-with Encord's API - Supports Python: `3.7`, `3.8`, `3.9`, and `3.10` ## â¨
-Relevant Links * [Encord website](https://encord.com) * [Encord web app](https:
-//app.encord.com) * [Encord documentation](https://docs.encord.com) ## ð¡
-Getting Started For full documentation, please visit [Encord Python SDK](https:
-//python.docs.encord.com/). First, install Encord Python API Client using the
-[pip](https://pip.pypa.io/en/stable/installing) package manager: ```bash pip
-install encord ``` Then, create an API key for authentication via the [Encord
-web app](https://app.encord.com). Pass the resource ID and API key as
-environment variables or pass them explicitly when you initialise the
-EncordClient object. ```bash export ENCORD_PROJECT_ID="" export
-ENCORD_API_KEY="" ``` Passing the resource ID and API key as environment
-variables, you can initialise the Encord client directly. ```python from
-encord.client import EncordClient client = EncordClient.initialise() ``` If you
-want to avoid setting environment variables, you can initialise the Encord
-client by passing the resource ID and API key as strings. ```python from
-encord.client import EncordClient client = EncordClient.initialise("", "") ```
-If you wish to instantiate several client objects and avoid passing parameters
-each time, you can instantiate a EncordConfig object, pass the resource ID and
-API key as strings, and initialise the client with the config object. ```py
-from encord.client import EncordClient from encord.client import EncordConfig
-config = EncordConfig("", "") client = EncordClient.initialise_with_config
-(config) ``` Once you have instantiated an Encord client, it is easy to fetch
-information associated with the given resource ID. ```py from encord.client
-import EncordClient client = EncordClient.initialise() project =
-client.get_project() ``` ## ð Troubleshooting Please report bugs to [GitHub
-Issues](https://github.com/encord-team/encord-client-python/issues). Just make
-sure you read the [Encord documentation](https://docs.encord.com) and search
-for related issues first.
+//opensource.org/licenses/Apache-2.0) # The data engine for computer vision ##
+ð» Features - Minimal low-level Python client that allows you to interact
+with Encord's API - Supports Python: `3.7`, `3.8`, `3.9`, `3.10` and `3.11` ##
+â¨ Relevant Links * [Encord website](https://encord.com) * [Encord web app]
+(https://app.encord.com) * [Encord documentation](https://docs.encord.com) ##
+ð¡ Getting Started For full documentation, please visit [Encord Python SDK]
+(https://python.docs.encord.com/). First, install Encord Python API Client
+using the [pip](https://pip.pypa.io/en/stable/installing) package manager:
+```bash pip install encord ``` Then, generate an public-private key pair, and
+upload the public key to [Encord website](https://www.encord.com/). Detailed
+guide can be found in the [dedicated manual](https://docs.encord.com/admins/
+settings/public-keys/). Passing the private key to the factory, you can
+initialise the Encord client directly. ```python from encord import
+EncordUserClient user_client = EncordUserClient.create_with_ssh_private_key
+( "", password="", ) ``` Once you have instantiated an Encord client, it is
+easy to fetch a project information and start working with the platform. ```py
+project = user_client.get_project("") label_rows = project.list_label_rows_v2()
+``` For detailed examples and API reference please refer to [Encord SDK
+documentation](https://python.docs.encord.com/) ## ð Troubleshooting Please
+report bugs to the [GitHub Issues](https://github.com/encord-team/encord-
+client-python/issues). Just make sure you read the [Encord documentation]
+(https://docs.encord.com) and search for related issues first.
```

