# Comparing `tmp/madtypes-0.0.4.tar.gz` & `tmp/madtypes-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "madtypes-0.0.4.tar", last modified: Mon May 29 17:35:57 2023, max compression
+gzip compressed data, was "madtypes-0.0.5.tar", last modified: Tue May 30 13:31:24 2023, max compression
```

## Comparing `madtypes-0.0.4.tar` & `madtypes-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:35:57.279113 madtypes-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-05-29 17:35:57.279113 madtypes-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-29 17:35:43.000000 madtypes-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:35:57.279113 madtypes-0.0.4/madtypes/
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-05-29 17:35:43.000000 madtypes-0.0.4/madtypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:35:57.279113 madtypes-0.0.4/madtypes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-05-29 17:35:57.000000 madtypes-0.0.4/madtypes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-29 17:35:57.000000 madtypes-0.0.4/madtypes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:35:57.000000 madtypes-0.0.4/madtypes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-29 17:35:57.000000 madtypes-0.0.4/madtypes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 17:35:57.279113 madtypes-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-29 17:35:43.000000 madtypes-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:35:57.279113 madtypes-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-05-29 17:35:43.000000 madtypes-0.0.4/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:31:24.101182 madtypes-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-30 13:31:24.101182 madtypes-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-05-30 13:31:05.000000 madtypes-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:31:24.097182 madtypes-0.0.5/madtypes/
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-05-30 13:31:05.000000 madtypes-0.0.5/madtypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:31:24.097182 madtypes-0.0.5/madtypes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-30 13:31:24.000000 madtypes-0.0.5/madtypes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-30 13:31:24.000000 madtypes-0.0.5/madtypes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:31:24.000000 madtypes-0.0.5/madtypes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-30 13:31:24.000000 madtypes-0.0.5/madtypes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 13:31:24.101182 madtypes-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-30 13:31:05.000000 madtypes-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:31:24.097182 madtypes-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-05-30 13:31:05.000000 madtypes-0.0.5/tests/test_schema.py
```

### Comparing `madtypes-0.0.4/madtypes/__init__.py` & `madtypes-0.0.5/madtypes/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,85 +1,104 @@
 from typing import get_args, get_origin, Union, Type
 import inspect
+import re
 
 TYPE_TO_STRING: dict[type, str] = {
     str: "string",
     int: "integer",
     list: "array",
     float: "number",
     tuple: "array",
 }
 
 
-def is_value_compatible_with_annotation(value, annotation):
+def is_optional_type(annotation):
+    return getattr(annotation, "__origin__", None) is Union and type(
+        None
+    ) in getattr(annotation, "__args__", ())
+
+
+def remove_optional(typing_annotation):
+    return get_args(typing_annotation)[0]
+
+
+def type_check(value, annotation):
     origin = get_origin(annotation)
     args = get_args(annotation)
 
     if origin is None:
         # Non-generic type
         return isinstance(value, annotation)
-    elif origin is list:
-        # List annotation
-        if isinstance(value, list):
+    elif origin is list or origin is set or origin is Union:
+        # typing.Union cannot be used by is_instance
+        if is_optional_type(annotation):
+            inner_annotation = args[0]
+            return type_check(value, inner_annotation)
+        elif isinstance(value, origin):
             if args:
                 # Parametrized list annotation
                 inner_annotation = args[0]
                 return all(
-                    is_value_compatible_with_annotation(item, inner_annotation)
-                    for item in value
+                    type_check(item, inner_annotation) for item in value
                 )
 
 
 class Annotation(type):
     def __new__(cls, name, bases, attrs):
         # Retrieve the annotation from the class attributes
         annotation = attrs.get("annotation")
+        pattern = attrs.get("pattern", None)
 
         # Override the __new__ method of the list class
         def new_method(cls, *values, **kwargs):
-            # Check the type of each value before initializing the list
+            # Check the type of each value before initializing
+            if pattern and (annotation != str and annotation != bytes):
+                raise SyntaxError(
+                    f"pattern attribute can only be applied upon `str` or `bytes`, was `{annotation}`"
+                )
             for value in values:
-                if not is_value_compatible_with_annotation(value, annotation):
+                if not type_check(value, annotation):
                     raise TypeError(
                         f"All values must be compatible with the annotation '{annotation}'"
                     )
 
-            # Create the list instance and initialize it with the values
+                if pattern and not re.fullmatch(pattern, value):
+                    raise TypeError(
+                        f"`{values[0]}` did not match provided pattern `{pattern}`"
+                    )
+
+            # Create the instance and initialize it with the values
             instance = super(cls, cls).__new__(cls, *values, **kwargs)
             return instance
 
         # Assign the overridden __new__ method to the class
         attrs["__new__"] = new_method
         return super().__new__(cls, name, bases, attrs)
 
 
-def is_optional_type(annotation):
-    return getattr(annotation, "__origin__", None) is Union and type(
-        None
-    ) in getattr(annotation, "__args__", ())
-
-
-def remove_optional(typing_annotation):
-    return get_args(typing_annotation)[0]
-
-
 class Schema(dict):
     def __init__(self, **kwargs):
         for key, value in self.__annotations__.items():
             if key in kwargs:
-                if isinstance(kwargs[key], value):
+                if type_check(kwargs[key], value):
                     super().__setitem__(key, kwargs[key])
                 else:
                     raise TypeError(
                         f"{kwargs[key]} is not an instance of {value}"
                     )
             else:
                 optional = is_optional_type(value)
                 if not optional:
                     raise TypeError(f"{key} is a mandatory field")
+        if not self.is_valid(**kwargs):
+            raise TypeError(f"{kwargs} did not pass object validation")
+
+    def is_valid(self, **__kwargs__) -> bool:
+        """Validation at Object scope, for validation based on multiple fields."""
+        return True
 
     @classmethod
     def get_fields(cls):
         return list(cls.__annotations__.items())
 
     def __getattr__(self, name):
         if name in self:
@@ -107,47 +126,47 @@
     def __setattr__(self, __name__, __value__):
         raise TypeError("'Immutable' object does not support item assignment")
 
     def __setitem__(self, __key__, __value__):
         raise TypeError("'Immutable' object does not support item assignment")
 
 
-def schema(
+def json_schema(
     annotation: Union[Type["Type"], Type["Annotation"], Type["Schema"]],
     **kwargs,
 ) -> dict:
     result = kwargs
     origin = get_origin(annotation)
     origin = annotation if not origin else origin
     args = get_args(annotation)
     if origin in TYPE_TO_STRING:
         result.update({"type": TYPE_TO_STRING[origin]})
     if origin == list:
-        result.update({"items": schema(args[0])})
+        result.update({"items": json_schema(args[0])})
     if origin == tuple:
-        result.update({"items": [schema(arg) for arg in args]})
+        result.update({"items": [json_schema(arg) for arg in args]})
     if isinstance(origin, str):
         raise SyntaxError("A typing annotation has been written as Literal")
     if inspect.isclass(origin):
         if issubclass(origin, Schema):
             result.update(
                 {
                     "type": "object",
                     "properties": {
-                        name: schema(field)
+                        name: json_schema(field)
                         for name, field in origin.get_fields()
                     },
                 }
             )
             required = origin.required_fields()
             if len(required) > 0:
                 result.update({"required": required})
         if getattr(origin, "annotation", False):
             extra = {
                 key: value
                 for key, value in origin.__dict__.items()
                 if not callable(value) and not key.startswith("__")
             }
-            return schema(origin.annotation, **extra)
+            return json_schema(origin.annotation, **extra)
     if is_optional_type(annotation):
-        return schema(remove_optional(annotation))
+        return json_schema(remove_optional(annotation))
     return result
```

### Comparing `madtypes-0.0.4/setup.py` & `madtypes-0.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="madtypes",
-    version="0.0.4",
+    version="0.0.5",
     author="6r17",
     author_email="patrick.borowy@proton.me",
     description="Python typing that raise TypeError at runtime",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/6r17/madtypes",
     packages=find_packages(include=["madtypes"]),
```

### Comparing `madtypes-0.0.4/tests/test_schema.py` & `madtypes-0.0.5/tests/test_schema.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Optional
-from madtypes import schema, Schema, Annotation, Immutable
+from madtypes import json_schema, Schema, Annotation, Immutable, type_check
 import pytest
 import json
 
 
 class Gender(Schema):
     female: int
     male: int
@@ -63,48 +63,51 @@
     a = Item(name="bob", gender=Gender(male=20, female=30))
     a.gender = Gender(male=30, female=10)
     assert a.gender.male == 30
     with pytest.raises(TypeError):
         a.gender.male = "foo"
 
 
-def test_int_schema():
-    assert schema(int) == {"type": "integer"}
+def test_int_json_schema():
+    assert json_schema(int) == {"type": "integer"}
 
 
-def test_array_schema():
-    assert schema(list[int]) == {"type": "array", "items": {"type": "integer"}}
+def test_array_json_schema():
+    assert json_schema(list[int]) == {
+        "type": "array",
+        "items": {"type": "integer"},
+    }
 
 
-def test_tuple_schema():
-    assert schema(tuple[int, int]) == {
+def test_tuple_json_schema():
+    assert json_schema(tuple[int, int]) == {
         "type": "array",
         "items": [{"type": "integer"}, {"type": "integer"}],
     }
 
 
-def test_object_schema():
+def test_object_json_schema():
     class Item(Schema):
         name: str
 
-    assert schema(Item) == {
+    assert json_schema(Item) == {
         "type": "object",
         "properties": {"name": {"type": "string"}},
         "required": ["name"],
     }
 
 
-def test_array_of_object_schema():
+def test_array_of_object_json_schema():
     class Item(Schema):
         name: str
 
     class Basket(Schema):
         items: list[Item]
 
-    schem = schema(Basket)
+    schem = json_schema(Basket)
     print(schem)
     assert schem == {
         "type": "object",
         "properties": {
             "items": {
                 "type": "array",
                 "items": {
@@ -114,22 +117,22 @@
                 },
             }
         },
         "required": ["items"],
     }
 
 
-def test_tuple_of_object_schema():
+def test_tuple_of_object_json_schema():
     class Item(Schema):
         name: str
 
     class Basket(Schema):
         some_items: tuple[Item, Item]
 
-    schem = schema(Basket)
+    schem = json_schema(Basket)
     print(schem)
     assert schem == {
         "type": "object",
         "properties": {
             "some_items": {
                 "type": "array",
                 "items": [
@@ -146,17 +149,17 @@
                 ],
             }
         },
         "required": ["some_items"],
     }
 
 
-def test_object_with_object_schema():
-    print(schema(Item))
-    assert schema(Item) == {
+def test_object_with_object_json_schema():
+    print(json_schema(Item))
+    assert json_schema(Item) == {
         "type": "object",
         "properties": {
             "name": {"type": "string"},
             "gender": {
                 "type": "object",
                 "properties": {
                     "female": {"type": "integer"},
@@ -170,15 +173,15 @@
 
 
 class PrimitiveArray(Schema):
     items: list[str]
 
 
 def test_annotation_array():
-    assert schema(PrimitiveArray) == {
+    assert json_schema(PrimitiveArray) == {
         "type": "object",
         "properties": {
             "items": {"type": "array", "items": {"type": "string"}}
         },
         "required": ["items"],
     }
 
@@ -189,15 +192,15 @@
 
 
 class PrimitiveDescriptedArray(Schema):
     descripted_array: PrimitiveDescriptiveArray
 
 
 def test_descriptive_primitive_array():
-    result = schema(PrimitiveDescriptedArray)
+    result = json_schema(PrimitiveDescriptedArray)
     print(result)
     assert result == {
         "type": "object",
         "properties": {
             "descripted_array": {
                 "type": "array",
                 "items": {"type": "integer"},
@@ -213,15 +216,15 @@
 
 
 class ObjectArray(Schema):
     persons: list[Person]
 
 
 def test_object_array():
-    result = schema(ObjectArray)
+    result = json_schema(ObjectArray)
     print(result)
     assert result == {
         "type": "object",
         "properties": {
             "persons": {
                 "type": "array",
                 "items": {
@@ -249,16 +252,16 @@
     description = "Lots of beers"
 
 
 class ObjectDescriptedArray(Schema):
     descripted_array: ObjectDescriptiveArray
 
 
-def test_descriptive_object_array():
-    result = schema(ObjectDescriptedArray)
+def test_descriptive_object_array_json_schema():
+    result = json_schema(ObjectDescriptedArray)
     print(result)
     assert result == {
         "type": "object",
         "properties": {
             "descripted_array": {
                 "description": "Lots of beers",
                 "type": "array",
@@ -278,16 +281,16 @@
     }
 
 
 class PrimitiveTuple(Schema):
     tupled: tuple[int, str]
 
 
-def test_annotation_tuple_schema():
-    result = schema(PrimitiveTuple)
+def test_annotation_tuple_json_schema():
+    result = json_schema(PrimitiveTuple)
     print(result)
     assert result == {
         "type": "object",
         "properties": {
             "tupled": {
                 "type": "array",
                 "items": [{"type": "integer"}, {"type": "string"}],
@@ -330,15 +333,15 @@
 
 
 def test_schemas_expect_types():
     class Item(Schema):
         value: "str"
 
     with pytest.raises(SyntaxError):
-        schema(Item)
+        json_schema(Item)
 
 
 def test_immutable():
     class SomeImmutable(Immutable):
         name: str
 
     e = SomeImmutable(name="foo")
@@ -375,32 +378,32 @@
 
         def method(self) -> str:
             return self.name
 
     assert SomeClass(name="foo").method() == "foo"
 
 
-def test_optional_json_schema():
+def test_optional_json_json_schema():
     class SomeClassWithOptional(Schema):
         name: Optional[str]
 
     SomeClassWithOptional()
-    schem = schema(SomeClassWithOptional)
+    schem = json_schema(SomeClassWithOptional)
     assert schem == {
         "type": "object",
         "properties": {"name": {"type": "string"}},
     }
 
 
 def test_optional_json_schema_with_array():
     class SomeClassWithOptional(Schema):
         elements: Optional[list[int]]
 
     SomeClassWithOptional()
-    schem = schema(SomeClassWithOptional)
+    schem = json_schema(SomeClassWithOptional)
     assert schem == {
         "type": "object",
         "properties": {
             "elements": {"type": "array", "items": {"type": "integer"}}
         },
     }
 
@@ -452,26 +455,122 @@
         annotation = Foo
 
     DescriptedFoo(name="foo")
     with pytest.raises(TypeError):
         DescriptedFoo(name=2)
 
 
-def test_descripted_json_schema():
+def test_descripted_json_json_schema():
     class DescriptedString(str, metaclass=Annotation):
         description = "Some description"
         annotation = str
 
     class DescriptedItem(Schema):
         descripted: DescriptedString
 
-    print(schema(DescriptedItem))
-    assert schema(DescriptedItem) == {
+    print(json_schema(DescriptedItem))
+    assert json_schema(DescriptedItem) == {
         "type": "object",
         "properties": {
             "descripted": {
                 "type": "string",
                 "description": "Some description",
             },
         },
         "required": ["descripted"],
     }
+
+
+def test_object_validation():
+    class Item(Schema):
+        title: Optional[str]
+        content: Optional[str]
+
+        def is_valid(self, **kwargs):
+            """title is mandatory if content is absent"""
+            return (
+                False
+                if not kwargs.get("content", None)
+                and not kwargs.get("title", None)
+                else True
+            )
+
+    Item(
+        title="foo"
+    )  # we should be able to create with only one of title or content
+    Item(content="foo")
+    with pytest.raises(TypeError):
+        Item()
+
+
+def test_set_set():
+    class Basket(Schema):
+        content: set[int]
+
+    Basket(content={1, 2, 3})
+
+
+def test_type_check_primitive():
+    assert type_check(1, int)
+
+
+def test_type_check_list_of_primitive():
+    assert type_check([1, 2], list[int])
+
+
+def test_type_check_set_of_primitive():
+    assert type_check({1}, set[int])
+
+
+def test_type_check_optional_primitive():
+    assert type_check(1, Optional[int])
+    assert type_check("foo", Optional[int]) == False
+
+
+def test_pattern_definition_with_incorect_type():
+    class PhoneNumber(int, metaclass=Annotation):
+        annotation = int
+        pattern = r"\b\d{3}-\d{3}-\d{4}\b"
+
+    with pytest.raises(SyntaxError):
+        PhoneNumber(2)
+
+
+def test_pattern_definition_allows_normal_usage():
+    class PhoneNumber(str, metaclass=Annotation):
+        annotation = str
+        pattern = r"\d{3}-\d{3}-\d{4}"  # Regex pattern to match a phone number in the format XXX-XXX-XXXX
+
+    PhoneNumber("000-000-0000")
+
+
+def test_pattern_raise_type_error():
+    class PhoneNumber(str, metaclass=Annotation):
+        annotation = str
+        pattern = r"\d{3}-\d{3}-\d{4}"  # Regex pattern to match a phone number in the format XXX-XXX-XXXX
+
+    with pytest.raises(TypeError):
+        PhoneNumber("oops")
+
+
+def test_pattern_is_rendered_in_json_schema():
+    class PhoneNumber(str, metaclass=Annotation):
+        annotation = str
+        pattern = r"^\d{3}-\d{3}-\d{4}$"
+        description = "A phone number in the format XXX-XXX-XXXX"
+
+    class Contact(Schema):
+        phone: PhoneNumber
+
+    schema = json_schema(Contact)
+    print(json.dumps(schema, indent=4))
+    assert schema == {
+        "type": "object",
+        "properties": {
+            "phone": {
+                "pattern": "^\\d{3}-\\d{3}-\\d{4}$",
+                "description": "A phone number in the format XXX-XXX-XXXX",
+                "type": "string",
+            }
+        },
+        "required": ["phone"],
+    }
```

