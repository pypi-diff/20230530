# Comparing `tmp/qtgql-0.119.3.tar.gz` & `tmp/qtgql-0.119.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtgql-0.119.3.tar", max compression
+gzip compressed data, was "qtgql-0.119.4.tar", max compression
```

## Comparing `qtgql-0.119.3.tar` & `qtgql-0.119.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1064 2023-05-28 13:18:28.017096 qtgql-0.119.3/LICENSE
--rw-r--r--   0        0        0     1805 2023-05-28 13:18:28.017096 qtgql-0.119.3/README.md
--rw-r--r--   0        0        0     4363 2023-05-28 13:18:50.957181 qtgql-0.119.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-28 13:18:28.029096 qtgql-0.119.3/qtgqlcodegen/__init__.py
--rw-r--r--   0        0        0     1866 2023-05-28 13:18:28.029096 qtgql-0.119.3/qtgqlcodegen/cli.py
--rw-r--r--   0        0        0        0 2023-05-28 13:18:28.029096 qtgql-0.119.3/qtgqlcodegen/compiler/__init__.py
--rw-r--r--   0        0        0     1761 2023-05-28 13:18:28.029096 qtgql-0.119.3/qtgqlcodegen/compiler/builtin_scalars.py
--rw-r--r--   0        0        0    11945 2023-05-28 13:18:28.029096 qtgql-0.119.3/qtgqlcodegen/compiler/operation.py
--rw-r--r--   0        0        0     3631 2023-05-28 13:18:28.029096 qtgql-0.119.3/qtgqlcodegen/compiler/template.py
--rw-r--r--   0        0        0     2065 2023-05-28 13:18:28.029096 qtgql-0.119.3/qtgqlcodegen/config.py
--rw-r--r--   0        0        0      413 2023-05-28 13:18:28.029096 qtgql-0.119.3/qtgqlcodegen/cppref.py
--rw-r--r--   0        0        0       41 2023-05-28 13:18:28.029096 qtgql-0.119.3/qtgqlcodegen/exceptions.py
--rw-r--r--   0        0        0     3187 2023-05-28 13:18:28.029096 qtgql-0.119.3/qtgqlcodegen/graphql_ref.py
--rw-r--r--   0        0        0    17696 2023-05-28 13:18:28.033096 qtgql-0.119.3/qtgqlcodegen/introspection.py
--rw-r--r--   0        0        0    10492 2023-05-28 13:18:28.033096 qtgql-0.119.3/qtgqlcodegen/objecttype.py
--rw-r--r--   0        0        0        0 2023-05-28 13:18:28.033096 qtgql-0.119.3/qtgqlcodegen/py.typed
--rw-r--r--   0        0        0        0 2023-05-28 13:18:28.033096 qtgql-0.119.3/qtgqlcodegen/runtime/__init__.py
--rw-r--r--   0        0        0     1566 2023-05-28 13:18:28.033096 qtgql-0.119.3/qtgqlcodegen/runtime/custom_scalars.py
--rw-r--r--   0        0        0      488 2023-05-28 13:18:28.033096 qtgql-0.119.3/qtgqlcodegen/templates/CMakeLists.jinja.cmake
--rw-r--r--   0        0        0      536 2023-05-28 13:18:28.033096 qtgql-0.119.3/qtgqlcodegen/templates/config.jinja.hpp
--rw-r--r--   0        0        0     2855 2023-05-28 13:18:28.033096 qtgql-0.119.3/qtgqlcodegen/templates/macros.jinja.hpp
--rw-r--r--   0        0        0     3779 2023-05-28 13:18:28.033096 qtgql-0.119.3/qtgqlcodegen/templates/operation.jinja.hpp
--rw-r--r--   0        0        0     2072 2023-05-28 13:18:28.033096 qtgql-0.119.3/qtgqlcodegen/templates/schema.jinja.hpp
--rw-r--r--   0        0        0     1028 2023-05-28 13:18:28.033096 qtgql-0.119.3/qtgqlcodegen/utils.py
--rw-r--r--   0        0        0     2800 1970-01-01 00:00:00.000000 qtgql-0.119.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-30 11:23:46.511797 qtgql-0.119.4/LICENSE
+-rw-r--r--   0        0        0     1805 2023-05-30 11:23:46.511797 qtgql-0.119.4/README.md
+-rw-r--r--   0        0        0     4424 2023-05-30 11:24:04.336475 qtgql-0.119.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/__init__.py
+-rw-r--r--   0        0        0     1866 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/cli.py
+-rw-r--r--   0        0        0        0 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/compiler/__init__.py
+-rw-r--r--   0        0        0     1761 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/compiler/builtin_scalars.py
+-rw-r--r--   0        0        0    12381 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/compiler/operation.py
+-rw-r--r--   0        0        0     3655 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/compiler/template.py
+-rw-r--r--   0        0        0     2159 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/config.py
+-rw-r--r--   0        0        0      420 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/cppref.py
+-rw-r--r--   0        0        0       41 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/exceptions.py
+-rw-r--r--   0        0        0     3187 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/graphql_ref.py
+-rw-r--r--   0        0        0    17749 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/introspection.py
+-rw-r--r--   0        0        0    10322 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/objecttype.py
+-rw-r--r--   0        0        0        0 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/py.typed
+-rw-r--r--   0        0        0        0 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/runtime/__init__.py
+-rw-r--r--   0        0        0     1571 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/runtime/custom_scalars.py
+-rw-r--r--   0        0        0      488 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/templates/CMakeLists.jinja.cmake
+-rw-r--r--   0        0        0      536 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/templates/config.jinja.hpp
+-rw-r--r--   0        0        0     2998 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/templates/macros.jinja.hpp
+-rw-r--r--   0        0        0     4633 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/templates/operation.jinja.hpp
+-rw-r--r--   0        0        0     2086 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/templates/schema.jinja.hpp
+-rw-r--r--   0        0        0     1028 2023-05-30 11:23:46.523797 qtgql-0.119.4/qtgqlcodegen/utils.py
+-rw-r--r--   0        0        0     2800 1970-01-01 00:00:00.000000 qtgql-0.119.4/PKG-INFO
```

### Comparing `qtgql-0.119.3/LICENSE` & `qtgql-0.119.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.3/README.md` & `qtgql-0.119.4/README.md`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.3/pyproject.toml` & `qtgql-0.119.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qtgql"
-version = "0.119.3"
+version = "0.119.4"
 packages = [{ include = "qtgqlcodegen" }]
 description = "Qt framework for building graphql driven QML applications"
 authors = ["Nir <88795475+nrbnlulu@users.noreply.github.com>"]
 maintainers = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
@@ -32,14 +32,17 @@
 faker = ">=15.3.4,<19.0.0"
 mypy = "^1.0.1"
 strawberry-graphql = ">=0.158.2,<0.180.0"
 aqtinstall = "^3.1.6"
 conan = "^2.0.4"
 cmake = "3.25.0"
 pygithub = "^1.58.2"
+githubrelease = "^1.5.9"
+httpx = "0.18.2"
+autopub = "^0.2.2"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "^9.0.5"
 mike = "^1.1.2"
 markdown-include = "^0.8.0"
 mkdocstrings = {extras = ["python"], version = ">=0.19.1,<0.22.0"}
 pygments = "^2.14.0"
```

### Comparing `qtgql-0.119.3/qtgqlcodegen/cli.py` & `qtgql-0.119.4/qtgqlcodegen/cli.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.3/qtgqlcodegen/compiler/builtin_scalars.py` & `qtgql-0.119.4/qtgqlcodegen/compiler/builtin_scalars.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.3/qtgqlcodegen/compiler/operation.py` & `qtgql-0.119.4/qtgqlcodegen/compiler/operation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import uuid
 from collections import defaultdict
 from functools import cached_property
 from typing import Optional
 from typing import TYPE_CHECKING
 
 import attrs
 import graphql
@@ -70,21 +71,27 @@
 
     @cached_property
     def type(self) -> GqlTypeHinter:
         return self.definition.type
 
     @cached_property
     def property_type(self) -> str:
-        if self.definition.type.is_object_type:
+        tp = self.definition.type
+        if tp.is_object_type:
             assert self.narrowed_type
             return self.narrowed_type.name
 
-        if cs := self.definition.is_custom_scalar:
-            return cs.property_type
-        return self.type.member_type
+        if cs := tp.is_custom_scalar:
+            return cs.type_for_proxy
+        if model_of := tp.is_model:
+            if model_of.is_object_type:
+                assert self.narrowed_type
+                return f"qtgql::bases::ListModelABC<{self.narrowed_type.name}>"
+
+        return tp.member_type
 
     @property
     def proxy_of(self) -> GqlTypeHinter:
         ret = self.definition.type
         assert ret
         return ret
 
@@ -247,24 +254,32 @@
             "\n   ".join(self.fields.keys()),
         )
 
     @cached_property
     def references(self) -> list[QtGqlQueriedField]:
         return [f for f in self.fields.values() if f.type.is_object_type]
 
+    @cached_property
+    def models(self) -> list[QtGqlQueriedField]:
+        return [f for f in self.fields.values() if f.type.is_model]
+
 
 @define(slots=False)
 class QtGqlOperationDefinition:
     operation_def: gql_def.OperationDefinitionNode
     evaluator: SchemaEvaluator
     directives: list[str] = attrs.Factory(list)
     fragments: list[str] = attrs.Factory(list)
     variables: list[QtGqlVariableDefinition] = attrs.Factory(list)
     narrowed_types_map: dict[str, QtGqlQueriedObjectType] = attrs.Factory(dict)
 
+    @cached_property
+    def operation_id(self) -> str:
+        return uuid.uuid4().hex
+
     def __attrs_post_init__(self) -> None:
         # instantiating the queried fields here, they build the narrowed types.
         self.root_field  # noqa
 
     @property
     def operation_config(self) -> str:
         return self.root_field.as_conf_string()
```

### Comparing `qtgql-0.119.3/qtgqlcodegen/compiler/template.py` & `qtgql-0.119.4/qtgqlcodegen/compiler/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
         return [scalar.graphql_name for scalar in self.config.custom_scalars.values()]
 
 
 @define(slots=False)
 class OperationTemplateContext:
     operation: QtGqlOperationDefinition
     config: QtGqlConfig
+    debug: bool = False
 
     @property
     def ns(self) -> str:
         return self.operation.name.lower()
 
     @property
     def schema_ns(self) -> str:
```

### Comparing `qtgql-0.119.3/qtgqlcodegen/config.py` & `qtgql-0.119.4/qtgqlcodegen/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,16 @@
     """
     evaluator: Type[SchemaEvaluator] = SchemaEvaluator
     """evaluates the schema and generates types."""
     custom_scalars: CustomScalarMap = {}
     """mapping of custom scalars, respected by the schema evaluator."""
     template_class: Callable[[SchemaTemplateContext], str] = schema_types_template
     """jinja template."""
+    debug: bool = False
+    """Templates would render some additional helpers for testing."""
 
     @cached_property
     def schema_path(self) -> Path:
         return self.graphql_dir / "schema.graphql"
 
     @cached_property
     def operations_dir(self) -> Path:
```

### Comparing `qtgql-0.119.3/qtgqlcodegen/graphql_ref.py` & `qtgql-0.119.4/qtgqlcodegen/graphql_ref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.3/qtgqlcodegen/introspection.py` & `qtgql-0.119.4/qtgqlcodegen/introspection.py`

 * *Files 1% similar despite different names*

```diff
@@ -397,14 +397,15 @@
         for op_name, op in self._operations.items():
             operations.append(
                 FileSpec(
                     content=operation_template(
                         OperationTemplateContext(
                             operation=op,
                             config=self.config,
+                            debug=self.config.debug,
                         ),
                     ),
                     path=self.config.generated_dir / f"{op_name}.hpp",
                 ),
             )
         schema = FileSpec(
             content=schema_types_template(context),
```

### Comparing `qtgql-0.119.3/qtgqlcodegen/objecttype.py` & `qtgql-0.119.4/qtgqlcodegen/objecttype.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 import attrs
 from attrs import define
 from typingref import TypeHinter
 from typingref import UNSET
 
 from qtgqlcodegen.compiler.builtin_scalars import BuiltinScalar
 from qtgqlcodegen.compiler.operation import QtGqlQueriedObjectType
-from qtgqlcodegen.cppref import QtGqlTypes
 from qtgqlcodegen.utils import AntiForwardRef
 
 if TYPE_CHECKING:
     from qtgqlcodegen.runtime.custom_scalars import CustomScalarDefinition
     from qtgqlcodegen.runtime.custom_scalars import CustomScalarMap
 
 
@@ -96,38 +95,38 @@
         if builtin_scalar := self.type.is_builtin_scalar:
             return builtin_scalar.default_value
         if self.type.is_object_type:
             return "{}"
 
         if self.type.is_model:
             # this would just generate the model without data.
-            raise NotImplementedError
+            return "{}"
 
         if self.type.is_custom_scalar:
             return "{}"
 
         if enum_def := self.type.is_enum:
             raise NotImplementedError
 
         raise NotImplementedError
 
     @cached_property
     def fget_annotation(self) -> str:
         """This annotates the value that is QML-compatible."""
         if custom_scalar := self.type.is_custom_scalar:
             return TypeHinter.from_annotations(
-                custom_scalar.property_type,
+                custom_scalar.type_for_proxy,
             ).stringify()
         if self.type.is_enum:
             return "int"
 
         return self.member_type
 
     @cached_property
-    def property_type(self) -> str:
+    def type_for_proxy(self) -> str:
         if self.type.is_builtin_scalar or self.type.is_custom_scalar:
             return self.fget_annotation
         else:
             if self.type.is_enum:
                 # QEnum value must be int
                 return "int"
             # might be a model, which is also QObject
@@ -142,15 +141,15 @@
 
     @cached_property
     def getter_name(self) -> str:
         return f"get_{self.name}"
 
     @cached_property
     def setter_name(self) -> str:
-        return f"{self.name}_setter"
+        return f"set_{self.name}"
 
     @cached_property
     def signal_name(self) -> str:
         return f"{self.name}Changed"
 
     @cached_property
     def private_name(self) -> str:
@@ -303,31 +302,29 @@
         t_self = self.optional_maybe.type
         if t_self in self.scalars.values():
             return t_self
 
     @cached_property
     def member_type(self) -> str:
         """
-        :returns: Annotation of the field based on the real type,
-        meaning that the private attribute would be of that type.
-        this goes for init and the property setter. They are optional by default,
-        (at the template) so unwrap optional first
+        :returns: Annotation of the field at the concrete type (for the type of the proxy use property type)
         """
         t_self = self.optional_maybe
 
         # int, str, float etc...
         if builtin_scalar := t_self.is_builtin_scalar:
             return builtin_scalar.tp
 
         if scalar := t_self.is_custom_scalar:
             return scalar.type_name
         if gql_enum := t_self.is_enum:
             return gql_enum.name
         if model_of := t_self.is_model:
-            return f"{QtGqlTypes.QGraphQLList.name}[{model_of.member_type}]"
+            # map of instances based on operation hash.
+            return f"QMap<QUuid, QList<{model_of.member_type}>>"
         if object_def := t_self.is_object_type or t_self.is_interface:
             return f"std::shared_ptr<{object_def.name}>"
         if q_object_def := t_self.is_queried_object_type:
             return f"{q_object_def.name}"
         if t_self.is_union:
             return "std::variant<" + ", ".join(th.member_type for th in t_self.of_type) + ">"
         if input_obj := t_self.is_input_object_type:
```

### Comparing `qtgql-0.119.3/qtgqlcodegen/runtime/custom_scalars.py` & `qtgql-0.119.4/qtgqlcodegen/runtime/custom_scalars.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,46 +2,46 @@
 
 
 @define
 class CustomScalarDefinition:
     type_name: str
     graphql_name: str
     deserialized_type: str
-    property_type: str
+    type_for_proxy: str
     include_path: str
 
 
 # An ISO-8601 encoded datetime.
 DateTimeScalarDefinition = CustomScalarDefinition(
     type_name="qtgql::customscalars::DateTimeScalar",
     graphql_name="DateTime",
     deserialized_type="QDateTime",
-    property_type="QString",
+    type_for_proxy="QString",
     include_path="<qtgql/customscalars/customscalars.hpp>",
 )
 DateScalarDefinition = CustomScalarDefinition(
     type_name="qtgql::customscalars::DateScalar",
     graphql_name="Date",
     deserialized_type="QDate",
-    property_type="QString",
+    type_for_proxy="QString",
     include_path="<qtgql/customscalars/customscalars.hpp>",
 )
 TimeScalarDefinition = CustomScalarDefinition(
     type_name="qtgql::customscalars::TimeScalar",
     graphql_name="Time",
     deserialized_type="QTime",
-    property_type="QString",
+    type_for_proxy="QString",
     include_path="<qtgql/customscalars/customscalars.hpp>",
 )
 
 DecimalScalarDefinition = CustomScalarDefinition(
     type_name="qtgql::customscalars::DecimalScalar",
     graphql_name="Decimal",
     deserialized_type="QString",
-    property_type="QString",
+    type_for_proxy="QString",
     include_path="<qtgql/customscalars/customscalars.hpp>",
 )
 
 
 CustomScalarMap = dict[str, CustomScalarDefinition]
 CUSTOM_SCALARS: CustomScalarMap = {
     DateTimeScalarDefinition.graphql_name: DateTimeScalarDefinition,
```

### Comparing `qtgql-0.119.3/qtgqlcodegen/templates/config.jinja.hpp` & `qtgql-0.119.4/qtgqlcodegen/templates/config.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.3/qtgqlcodegen/templates/macros.jinja.hpp` & `qtgql-0.119.4/qtgqlcodegen/templates/macros.jinja.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 {% macro deserialize_field(f, assign_to, include_selection_check = True) -%}
 
 if ({% if include_selection_check %}config.selections.contains("👉f.name👈") && {% endif %} !data.value("👉f.name👈").isNull()){
 {% if f.type.is_object_type -%}
 
-👉 assign_to 👈 = 👉f.type.is_object_type.name👈::from_json(data.value("👉f.name👈").toObject(), config.selections.value("person"), metadata);
+👉 assign_to 👈 = 👉f.type.is_object_type.name👈::from_json(data.value("👉f.name👈").toObject(), config.selections.value("👉f.name👈"), metadata);
 
 {% elif f.type.is_interface -%}
 if field_data:
         👉 assign_to 👈 = 👉f.type.is_interface.name👈.from_dict(
         parent,
         field_data,
         inner_config,
         metadata,
     )
 {% elif f.type.is_model -%}
 {% if f.type.is_model.is_object_type -%}
-👉 assign_to 👈 = qtgql::ListModel(
-  parent=parent,
-  data=[👉f.type.is_model.is_object_type.name👈.from_dict(parent, data=node, config=inner_config, metadata=metadata) for
-        node in field_data],
-)
+QList<👉f.type.is_model.member_type👈> obj_list;
+for (const auto& node: data.value("👉f.name👈").toArray()){
+    obj_list.append(👉 f.type.is_model.is_object_type.name 👈::from_json(node.toObject(), config.selections.value("👉f.name👈"), metadata));
+};
+👉 assign_to 👈.insert(metadata.operation_id, obj_list);
+
 {% elif f.type.is_model.is_interface -%}
 👉 assign_to 👈 = qtgql::ListModel(
     parent=parent,
     data=[👉f.type.is_model.is_interface.name👈.from_dict(parent, data=node, config=inner_config, metadata=metadata) for
           node in field_data],
 )
 {% elif f.type.is_model.is_union -%}
@@ -50,35 +51,36 @@
 👉 assign_to 👈 = __TYPE_MAP__[type_name].from_dict(parent, field_data, choice, metadata);
 {% endif -%}
 };
 {%- endmacro %}
 
 
 
-{% macro props(type) -%}
+{% macro concrete_type_fields(type) -%}
 protected:
 {% for f in type.fields -%}
 👉 f.member_type 👈 👉 f.private_name 👈 = 👉 f.default_value 👈;
 {% endfor %}
 signals:
 {%for f in type.fields -%}
 void 👉 f.signal_name 👈();
 {% endfor %}
 
 public:
 {%for f in type.fields %}
 {% if f.is_custom_scalar %}
-const 👉 f.is_custom_scalar.property_type 👈 & 👉 f.getter_name 👈() {
+const 👉 f.is_custom_scalar.type_for_proxy 👈 & 👉 f.getter_name 👈() {
 return 👉 f.private_name 👈.to_qt();
 }
 {% else %}
 const 👉 f.member_type 👈 & 👉 f.getter_name 👈() const {
 return 👉 f.private_name 👈;
 }
 {% endif %}
 void 👉 f.setter_name 👈(const 👉 f.member_type 👈 &v)
 {
 👉 f.private_name 👈 = v;
 emit 👉 f.signal_name 👈();
 };
 {% endfor %}
 {% endmacro -%}
+
```

### Comparing `qtgql-0.119.3/qtgqlcodegen/templates/operation.jinja.hpp` & `qtgql-0.119.4/qtgqlcodegen/templates/operation.jinja.hpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,61 @@
 {% import "macros.jinja.hpp" as macros -%}
 #pragma once
 #include "./schema.hpp"
 #include <qtgql/gqlwstransport/gqlwstransport.hpp>
+#include <QObject>
 
 namespace 👉 context.config.env_name 👈{
 namespace 👉context.ns👈{
-
-inline const qtgql::bases::OperationMetadata OPERATION_METADATA = qtgql::bases::OperationMetadata{
-        "👉 context.operation.name 👈",
-        {👉 context.operation.root_field.as_conf_string() 👈}
-};
-
+const auto OPERATION_ID = QUuid::fromString("👉 context.operation.operation_id👈");
 
 {% for t in context.operation.narrowed_types %}
-class 👉 t.name 👈{
+class 👉 t.name 👈: public QObject{
 /*
 👉 t.doc_fields 👈
  */
-    Q_GADGET
+    Q_OBJECT
+{# members #}
+{% if context.debug -%}
+public: // WARNING: members are public because you have debug=True in your config file.
+{% endif %}
 std::shared_ptr<👉context.schema_ns👈::👉 t.definition.name 👈> m_inst;
 {% for ref in t.references -%}
-std::unique_ptr<👉ref.narrowed_type.name👈> m_👉ref.name👈;
+👉ref.narrowed_type.name👈 *m_👉ref.name👈 = nullptr;
+{% endfor %}
+{%- for model_field in t.models -%}
+👉 model_field.property_type 👈 *m_👉model_field.name👈 = nullptr;
 {% endfor %}
 
 public:
-👉 t.name 👈(const std::shared_ptr<👉 t.definition.name 👈> &inst ): m_inst{inst}{
+👉 t.name 👈(QObject* parent, const std::shared_ptr<👉 t.definition.name 👈> &inst ): m_inst{inst}, QObject::QObject(parent){
 {% for ref in t.references -%}
 {% if ref.type.is_optional() %}
 if (m_inst->👉ref.definition.getter_name 👈()){
-m_👉ref.name👈 = std::make_unique<👉ref.narrowed_type.name👈>(m_inst->👉ref.definition.getter_name 👈());
+m_👉ref.name👈 = new 👉ref.narrowed_type.name👈(this, m_inst->👉ref.definition.getter_name 👈());
 }
 else{
-m_👉ref.name👈 = std::unique_ptr<👉ref.narrowed_type.name👈>();
+m_👉ref.name👈 = nullptr;
 }
 {% else %}
-m_👉ref.name👈 = std::make_unique<👉ref.narrowed_type.name👈>(m_inst->👉ref.definition.getter_name 👈());
+m_👉ref.name👈 = new 👉ref.narrowed_type.name👈(this, m_inst->👉ref.definition.getter_name 👈());
 {% endif %}
 {% endfor %}
+{%- for model_field in t.models -%}
+auto init_list_👉 model_field.name 👈 =  std::make_unique<QList<👉model_field.narrowed_type.name👈*>>();
+for (const auto & node: m_inst->👉model_field.definition.getter_name 👈().value(OPERATION_ID)){
+    init_list_👉 model_field.name 👈->append(new 👉model_field.narrowed_type.name👈(this, node));
+}
+m_👉model_field.name👈 = new 👉 model_field.property_type 👈(this, std::move(init_list_👉 model_field.name 👈));
+{% endfor -%}
 }
 {%- for f in t.fields.values() %}
-{% if f.type.is_optional() and f.type.is_object_type %}
+{% if f.type.is_object_type or f.type.is_model %}
 [[nodiscard]] inline const 👉 f.property_type 👈 * 👉 f.definition.getter_name 👈() const {
-    return m_👉f.name👈.get();
+    return m_👉f.name👈;
 {% else %}
 [[nodiscard]] inline const 👉 f.property_type 👈 & 👉 f.definition.getter_name 👈() const {
     {% if f.type.is_object_type %}
     return *m_👉f.name👈;
     {% else %}
     return m_inst->👉 f.definition.getter_name 👈();
     {% endif %}
@@ -55,44 +65,51 @@
 };
 {% endfor %}
 
 class 👉 context.operation.name 👈: public qtgql::gqlwstransport::OperationHandlerABC {
     Q_OBJECT
 Q_PROPERTY(const 👉 context.operation.root_field.property_type 👈* data READ get_data NOTIFY dataChanged);
 
-std::unique_ptr<👉 context.operation.root_field.property_type 👈> m_data;
+👉 context.operation.root_field.property_type 👈 *m_data = nullptr;
 
 inline const QString &ENV_NAME() override{
     static const auto ret = QString("👉 context.config.env_name 👈");
     return ret;
     }
-public:
 
+inline const qtgql::bases::OperationMetadata & OPERATION_METADATA() override{
+auto static ret = qtgql::bases::OperationMetadata{
+        OPERATION_ID,
+        {👉 context.operation.root_field.as_conf_string() 👈}
+};
+return ret;
+};
+public:
 👉 context.operation.name 👈(): qtgql::gqlwstransport::OperationHandlerABC(qtgql::gqlwstransport::GqlWsTrnsMsgWithID(qtgql::gqlwstransport::OperationPayload(
         {%- for line in context.operation.query.splitlines() %}"👉 line 👈"{% endfor -%}
-        ))){};
+        ), OPERATION_ID)){};
 
 inline const QUuid &operation_id() const override{
-return m_message_template.op_id;
+return OPERATION_ID;
 }
 
 
 void on_next(const QJsonObject &message) override{
     if (!m_data && message.contains("data")){
         auto data = message.value("data").toObject();
         if (data.contains("👉 context.operation.root_field.name 👈")){
-            m_data = std::make_unique<👉 context.operation.root_field.property_type 👈>(
+            m_data = new 👉 context.operation.root_field.property_type 👈(this,
 👉context.schema_ns👈::👉 context.operation.root_field.definition.type.is_object_type.name 👈::from_json(
-        data.value("👉 context.operation.root_field.name 👈").toObject(), OPERATION_METADATA.selections, OPERATION_METADATA)
+        data.value("👉 context.operation.root_field.name 👈").toObject(), OPERATION_METADATA().selections, OPERATION_METADATA())
 );
         }
     }
 }
 inline const 👉 context.operation.root_field.property_type 👈* get_data(){
-    return m_data.get();
+    return m_data;
 }
 
 {% if context.operation.variables %}
 void setVariables(
 {% for var in context.operation.variables -%}
 const std::optional<👉 var.type.member_type 👈>  👉 var.name 👈 {% if not loop.last %},{% endif %}
 {% endfor -%}){
```

### Comparing `qtgql-0.119.3/qtgqlcodegen/templates/schema.jinja.hpp` & `qtgql-0.119.4/qtgqlcodegen/templates/schema.jinja.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -17,17 +17,18 @@
 class 👉 type.name 👈 : public qtgql::bases::👉 base_class 👈{
 protected:
 static auto & INST_STORE() {
     static qtgql::bases::ObjectStore<👉 type.name 👈> _store;
     return _store;
 }
 
-👉 macros.props(type) 👈
+👉 macros.concrete_type_fields(type) 👈
 public:
 inline static const QString TYPE_NAME = "👉 type.name 👈";
+
 explicit 👉 type.name 👈 (QObject* parent = nullptr)
 : qtgql::bases::👉 base_class 👈::👉 base_class 👈(parent) {};
 
 
 static std::shared_ptr<👉 type.name 👈> from_json(const QJsonObject& data,
                                  const qtgql::bases::SelectionsConfig &config,
                                  const qtgql::bases::OperationMetadata& metadata){
@@ -43,15 +44,15 @@
 if (inst->id) {
   auto record = qtgql::bases::NodeRecord(node = inst, retainers = set())
                     .retain(metadata.operation_name)
                         cls.INST_STORE.add_record(record)
 }
 {% elif type.has_id_field and not type.id_is_optional %}
 auto record = std::make_shared<qtgql::bases::NodeRecord<👉 type.name 👈>>(inst);
-record->retain(metadata.operation_name);
+record->retain(metadata.operation_id);
 INST_STORE().add_record(record);
 {% endif %}
 return inst;
 };
 
 void loose(const qtgql::bases::OperationMetadata &metadata){throw "not implemented";};
 void update(const QJsonObject &data,
```

### Comparing `qtgql-0.119.3/qtgqlcodegen/utils.py` & `qtgql-0.119.4/qtgqlcodegen/utils.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.3/PKG-INFO` & `qtgql-0.119.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtgql
-Version: 0.119.3
+Version: 0.119.4
 Summary: Qt framework for building graphql driven QML applications
 License: MIT
 Author: Nir
 Author-email: 88795475+nrbnlulu@users.noreply.github.com
 Maintainer: Nir.J Benlulu
 Maintainer-email: nrbnlulu@gmail.com
 Requires-Python: >=3.9,<3.12
```

