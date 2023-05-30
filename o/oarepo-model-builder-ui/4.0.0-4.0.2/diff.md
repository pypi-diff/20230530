# Comparing `tmp/oarepo-model-builder-ui-4.0.0.tar.gz` & `tmp/oarepo-model-builder-ui-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-ui-4.0.0.tar", last modified: Mon May 22 09:50:32 2023, max compression
+gzip compressed data, was "oarepo-model-builder-ui-4.0.2.tar", last modified: Tue May 30 20:35:15 2023, max compression
```

## Comparing `oarepo-model-builder-ui-4.0.0.tar` & `oarepo-model-builder-ui-4.0.2.tar`

### file list

```diff
@@ -1,35 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:50:32.302557 oarepo-model-builder-ui-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-22 09:50:32.302557 oarepo-model-builder-ui-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:50:32.298557 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:50:32.302557 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/builders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/builders/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/builders/i18n_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/builders/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/builders/layout_setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:50:32.302557 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/datatypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:50:32.302557 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/datatypes/components/
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/datatypes/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/datatypes/components/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:50:32.302557 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/outputs/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/outputs/layout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:50:32.302557 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:50:32.302557 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-22 09:50:32.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-22 09:50:32.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 09:50:32.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-22 09:50:32.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-22 09:50:32.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-22 09:50:32.000000 oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-22 09:50:32.302557 oarepo-model-builder-ui-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 09:50:32.302557 oarepo-model-builder-ui-4.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/tests/test_facets.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-22 09:47:24.000000 oarepo-model-builder-ui-4.0.0/tests/test_translation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:35:15.401019 oarepo-model-builder-ui-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-30 20:31:42.000000 oarepo-model-builder-ui-4.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-30 20:35:15.401019 oarepo-model-builder-ui-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-30 20:31:42.000000 oarepo-model-builder-ui-4.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:35:15.401019 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 20:31:42.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:35:15.401019 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 20:31:42.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-30 20:31:42.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/builders/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-30 20:31:42.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/builders/i18n_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-30 20:31:42.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/builders/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-30 20:31:42.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/builders/layout_setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-30 20:31:42.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:35:15.401019 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 20:31:42.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/datatypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:35:15.401019 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/datatypes/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-30 20:31:42.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/datatypes/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-30 20:31:42.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/datatypes/components/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:35:15.401019 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-30 20:31:42.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/outputs/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-30 20:31:42.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/outputs/layout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:35:15.401019 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-30 20:31:42.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 20:35:15.401019 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-30 20:35:15.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-30 20:35:15.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 20:35:15.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-30 20:35:15.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-30 20:35:15.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-30 20:35:15.000000 oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-30 20:31:42.000000 oarepo-model-builder-ui-4.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-30 20:35:15.405020 oarepo-model-builder-ui-4.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 20:31:42.000000 oarepo-model-builder-ui-4.0.2/setup.py
```

### Comparing `oarepo-model-builder-ui-4.0.0/PKG-INFO` & `oarepo-model-builder-ui-4.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-ui
-Version: 4.0.0
+Version: 4.0.2
 Summary: Model builder plugin for oarepo-ui
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 <!--
  Copyright (c) 2022 CESNET
```

### Comparing `oarepo-model-builder-ui-4.0.0/README.md` & `oarepo-model-builder-ui-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/builders/i18n.py` & `oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/builders/i18n.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/builders/i18n_setup_cfg.py` & `oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/builders/i18n_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/builders/layout.py` & `oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/builders/layout.py`

 * *Files 19% similar despite different names*

```diff
@@ -31,32 +31,19 @@
     output_file_name = ["ui", "file"]
     create_parent_packages = True
 
     def build_node(self, node):
         generated = self.generate_node(node)
         self.output.merge(generated)
 
-    def generate(self, node):
-        ui: Section = node.section_ui
-        ret = {**ui.config}
-        ret.pop('marshmallow', None)
-
-        if ui.children:
-            properties = ret.setdefault("children", {})
-            for k, v in ui.children.items():
-                v = self.generate(v)
-                properties[k] = v
-        if ui.item:
-            ret["child"] = self.generate(ui.item)
-        return ret
-
     def generate_node(self, node):
         ui = {}
         section = node.section_ui
         data = node.definition
+        facets = node.section_facets.config['facets']
 
         ui.update({k.replace("-", "_"): v for k, v in section.config.items()})
         ui.pop('marshmallow', None)
         if "type" in data:
             t = data["type"]
             if t in ("object", "nested"):
                 t = inflect.engine().singular_noun(
@@ -67,20 +54,16 @@
 
         for fld in UI_ITEMS:
             ui[fld] = data.get(
                 f"{fld}.key",
                 node.path.replace('.', '/') + f".{fld}",
             )
 
-        # facets = get_facet_details(
-        #     self.stack, self.current_model, self.schema, set()
-        # )
-        #
-        # if len(facets):
-        #     ui["facet"] = facets[0]["path"]
+        if facets:
+            ui["facet"] = facets[0].path
 
         if node.children:
             children = ui.setdefault('children', {})
             for c in node.children.values():
                 children[c.key] = self.generate_node(c)
         if hasattr(node, 'item'):
             ui['child'] = self.generate_node(node.item)
```

### Comparing `oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/builders/layout_setup_cfg.py` & `oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/builders/layout_setup_cfg.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/datatypes/components/__init__.py` & `oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/datatypes/components/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/datatypes/components/model.py` & `oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/datatypes/components/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,28 +12,30 @@
     class Meta:
         unknown = ma.RAISE
 
     module = ma.fields.Str()
     alias = ma.fields.Str()
 
 class UISchema(ma.Schema):
+    """
+    registered in entry points to the ui.model group
+    """
     class Meta:
         unknown = ma.RAISE
 
     module = ma.fields.Str()
     file = ma.fields.Str()
     alias = ma.fields.Str()
 
 class UIModelComponent(DataTypeComponent):
     eligible_datatypes = [ModelDataType]
     depends_on=[SavedModelComponent]
 
     class ModelSchema(ma.Schema):
         translations = ma.fields.Nested(TranslationsSchema)
-        ui = ma.fields.Nested(UISchema)
 
     def before_model_prepare(self, datatype, *, context, **kwargs):
         translations = set_default(datatype, 'translations', {})
         translations.setdefault('module', f"{datatype.definition['module']['qualified']}.translations")
         translations.setdefault('alias', datatype.definition['module']['alias'])
 
         ui = set_default(datatype, 'ui', {})
```

### Comparing `oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/outputs/i18n.py` & `oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/outputs/i18n.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui/outputs/layout.py` & `oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui/outputs/layout.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui.egg-info/PKG-INFO` & `oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-ui
-Version: 4.0.0
+Version: 4.0.2
 Summary: Model builder plugin for oarepo-ui
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 <!--
  Copyright (c) 2022 CESNET
```

### Comparing `oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui.egg-info/SOURCES.txt` & `oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 oarepo_model_builder_ui/__init__.py
 oarepo_model_builder_ui/config.py
 oarepo_model_builder_ui.egg-info/PKG-INFO
@@ -16,10 +17,8 @@
 oarepo_model_builder_ui/builders/layout.py
 oarepo_model_builder_ui/builders/layout_setup_cfg.py
 oarepo_model_builder_ui/datatypes/__init__.py
 oarepo_model_builder_ui/datatypes/components/__init__.py
 oarepo_model_builder_ui/datatypes/components/model.py
 oarepo_model_builder_ui/outputs/i18n.py
 oarepo_model_builder_ui/outputs/layout.py
-oarepo_model_builder_ui/validation/__init__.py
-tests/test_facets.py
-tests/test_translation.py
+oarepo_model_builder_ui/validation/__init__.py
```

### Comparing `oarepo-model-builder-ui-4.0.0/oarepo_model_builder_ui.egg-info/entry_points.txt` & `oarepo-model-builder-ui-4.0.2/oarepo_model_builder_ui.egg-info/entry_points.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,7 +11,10 @@
 50-oarepo-ui = oarepo_model_builder_ui.model_preprocessors.layout_settings:LayoutSettingsPreprocessor
 
 [oarepo_model_builder.outputs]
 po = oarepo_model_builder_ui.outputs.i18n:POOutput
 
 [oarepo_model_builder.validation.settings]
 ui-settings = oarepo_model_builder_ui.validation:UISettingsSchema
+
+[oarepo_model_builder.validation.ui.model]
+ui-model = oarepo_model_builder.ui.datatypes.components.model:UISchema
```

### Comparing `oarepo-model-builder-ui-4.0.0/setup.cfg` & `oarepo-model-builder-ui-4.0.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 [metadata]
 name = oarepo-model-builder-ui
-version = 4.0.0
+version = 4.0.2
 description = Model builder plugin for oarepo-ui
 authors = 
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
 python = >=3.9,<4.0
 install_requires = 
 	langcodes>=3.3.0
 	oarepo-model-builder>=4.0.0
 	polib
 	inflect
 
+[options.packages.find]
+exclude = 
+	tests
+	mock_record
+
 [options.extras_require]
 tests = 
 	pytest>=7
 
 [options.package_data]
 * = *.json, *.rst, *.md, *.json5, *.jinja2
 
 [options.entry_points]
 oarepo_model_builder.validation.settings = 
 	ui-settings = oarepo_model_builder_ui.validation:UISettingsSchema
+oarepo_model_builder.validation.ui.model = 
+	ui-model = oarepo_model_builder.ui.datatypes.components.model:UISchema
 oarepo_model_builder.datatypes.components = 
 	ui-components = oarepo_model_builder_ui.datatypes.components:components
 oarepo_model_builder.builders.record = 
 	4000-oarepo-i18n = oarepo_model_builder_ui.builders.i18n:InvenioI18nBuilder
 	4010-oarepo-i18n-setup = oarepo_model_builder_ui.builders.i18n_setup_cfg:InvenioI18NSetupCfgBuilder
 	4020-oarepo-ui-layout = oarepo_model_builder_ui.builders.layout:InvenioLayoutBuilder
 	4030-oarepo-ui-layout-setup = oarepo_model_builder_ui.builders.layout_setup_cfg:InvenioLayoutSetupCfgBuilder
```

