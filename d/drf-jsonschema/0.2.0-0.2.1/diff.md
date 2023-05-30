# Comparing `tmp/drf-jsonschema-0.2.0.tar.gz` & `tmp/drf-jsonschema-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-jsonschema-0.2.0.tar", last modified: Wed Nov 23 05:36:00 2022, max compression
+gzip compressed data, was "drf-jsonschema-0.2.1.tar", last modified: Tue May 30 00:06:27 2023, max compression
```

## Comparing `drf-jsonschema-0.2.0.tar` & `drf-jsonschema-0.2.1.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 05:36:00.744046 drf-jsonschema-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-11-23 05:35:50.000000 drf-jsonschema-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2706 2022-11-23 05:36:00.744046 drf-jsonschema-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1129 2022-11-23 05:35:50.000000 drf-jsonschema-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 05:36:00.740045 drf-jsonschema-0.2.0/drf_jsonschema/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-23 05:35:50.000000 drf-jsonschema-0.2.0/drf_jsonschema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-11-23 05:35:50.000000 drf-jsonschema-0.2.0/drf_jsonschema/_validators.py
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-11-23 05:35:50.000000 drf-jsonschema-0.2.0/drf_jsonschema/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      305 2022-11-23 05:35:50.000000 drf-jsonschema-0.2.0/drf_jsonschema/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4550 2022-11-23 05:35:50.000000 drf-jsonschema-0.2.0/drf_jsonschema/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 05:36:00.740045 drf-jsonschema-0.2.0/drf_jsonschema/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-23 05:35:50.000000 drf-jsonschema-0.2.0/drf_jsonschema/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      348 2022-11-23 05:35:50.000000 drf-jsonschema-0.2.0/drf_jsonschema/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 05:36:00.744046 drf-jsonschema-0.2.0/drf_jsonschema/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-23 05:35:50.000000 drf-jsonschema-0.2.0/drf_jsonschema/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      856 2022-11-23 05:35:50.000000 drf-jsonschema-0.2.0/drf_jsonschema/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-11-23 05:35:50.000000 drf-jsonschema-0.2.0/drf_jsonschema/tests/serializers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2012 2022-11-23 05:35:50.000000 drf-jsonschema-0.2.0/drf_jsonschema/tests/test_json_schema_field_validator.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-23 05:35:50.000000 drf-jsonschema-0.2.0/drf_jsonschema/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (121)     1516 2022-11-23 05:35:50.000000 drf-jsonschema-0.2.0/drf_jsonschema/tests/views.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-23 05:35:50.000000 drf-jsonschema-0.2.0/drf_jsonschema/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     1813 2022-11-23 05:35:50.000000 drf-jsonschema-0.2.0/drf_jsonschema/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 05:36:00.740045 drf-jsonschema-0.2.0/drf_jsonschema.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2706 2022-11-23 05:36:00.000000 drf-jsonschema-0.2.0/drf_jsonschema.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      698 2022-11-23 05:36:00.000000 drf-jsonschema-0.2.0/drf_jsonschema.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-23 05:36:00.000000 drf-jsonschema-0.2.0/drf_jsonschema.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-11-23 05:36:00.000000 drf-jsonschema-0.2.0/drf_jsonschema.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-23 05:36:00.000000 drf-jsonschema-0.2.0/drf_jsonschema.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      469 2022-11-23 05:35:50.000000 drf-jsonschema-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-23 05:36:00.744046 drf-jsonschema-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-30 00:06:27.529634 drf-jsonschema-0.2.1/
+-rw-rw-rw-   0        0        0     1101 2023-05-29 23:57:30.000000 drf-jsonschema-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     2775 2023-05-30 00:06:27.528633 drf-jsonschema-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1155 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-30 00:06:27.482591 drf-jsonschema-0.2.1/drf_jsonschema/
+-rw-rw-rw-   0        0        0        0 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.1/drf_jsonschema/__init__.py
+-rw-rw-rw-   0        0        0     1156 2023-05-30 00:02:40.000000 drf-jsonschema-0.2.1/drf_jsonschema/_validators.py
+-rw-rw-rw-   0        0        0      144 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.1/drf_jsonschema/apps.py
+-rw-rw-rw-   0        0        0      314 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.1/drf_jsonschema/exceptions.py
+-rw-rw-rw-   0        0        0     4664 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.1/drf_jsonschema/fields.py
+drwxrwxrwx   0        0        0        0 2023-05-30 00:06:27.502609 drf-jsonschema-0.2.1/drf_jsonschema/migrations/
+-rw-rw-rw-   0        0        0        0 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.1/drf_jsonschema/migrations/__init__.py
+-rw-rw-rw-   0        0        0      357 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.1/drf_jsonschema/serializers.py
+drwxrwxrwx   0        0        0        0 2023-05-30 00:06:27.527632 drf-jsonschema-0.2.1/drf_jsonschema/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.1/drf_jsonschema/tests/__init__.py
+-rw-rw-rw-   0        0        0      886 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.1/drf_jsonschema/tests/models.py
+-rw-rw-rw-   0        0        0      250 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.1/drf_jsonschema/tests/serializers.py
+-rw-rw-rw-   0        0        0     2080 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.1/drf_jsonschema/tests/test_json_schema_field_validator.py
+-rw-rw-rw-   0        0        0        0 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.1/drf_jsonschema/tests/test_views.py
+-rw-rw-rw-   0        0        0     1566 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.1/drf_jsonschema/tests/views.py
+-rw-rw-rw-   0        0        0     1862 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.1/drf_jsonschema/validators.py
+drwxrwxrwx   0        0        0        0 2023-05-30 00:06:27.501609 drf-jsonschema-0.2.1/drf_jsonschema.egg-info/
+-rw-rw-rw-   0        0        0     2775 2023-05-30 00:06:27.000000 drf-jsonschema-0.2.1/drf_jsonschema.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      675 2023-05-30 00:06:27.000000 drf-jsonschema-0.2.1/drf_jsonschema.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 00:06:27.000000 drf-jsonschema-0.2.1/drf_jsonschema.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-30 00:06:27.000000 drf-jsonschema-0.2.1/drf_jsonschema.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-30 00:06:27.000000 drf-jsonschema-0.2.1/drf_jsonschema.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      484 2023-05-30 00:00:09.000000 drf-jsonschema-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-30 00:06:27.529634 drf-jsonschema-0.2.1/setup.cfg
```

### Comparing `drf-jsonschema-0.2.0/LICENSE` & `drf-jsonschema-0.2.1/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) [year] [fullname]
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2023 Kira Technologies Pty Ltd
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `drf-jsonschema-0.2.0/PKG-INFO` & `drf-jsonschema-0.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-Metadata-Version: 2.1
-Name: drf-jsonschema
-Version: 0.2.0
-Summary: A package that constructs JsonSchema validation error into error tree for Django Rest Framework with custom error message in compliance with the DRF error message.
-License: MIT License
-        
-        Copyright (c) [year] [fullname]
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-Keywords: jsonschema,drf
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-=============================
-drf-jsonschema
-=============================
-drf-jsonschema, created by Kiratech from extending `jsonschema <https://github.com/python-jsonschema/jsonschema>`_ package.
-This package provides JsonSchemaField and constructs JsonSchema validation error into error tree for Django Rest Framework with custom error message. 
-
-This package will install `jsonschema <https://github.com/python-jsonschema/jsonschema>`_ automatically so manual installation is not necessary.
-
-Quick Start
------------
-
-1. You can use JsonSchemaFieldValidator in Django's ``models.py`` as such::
-
-    from drf_jsonschema import JsonSchemaFieldValidator
-    ...
-    ...
-    json_data = models.JSONField(validators=[JsonSchemaFieldValidator(schema=your_json_schema)])
-
-2. On ``serializers.py``, modify the serializer field mapping from ``JSONField`` to ``JSONSchemaField`` as the example below::
-
-    from drf_jsonschema.serializers import JsonSchemaModelSerializer
-
-    class YourSerializer(JsonSchemaModelSerializer):
-        ...
-
-3. For more information, visit `jsonschema <https://github.com/python-jsonschema/jsonschema>`_ 
+Metadata-Version: 2.1
+Name: drf-jsonschema
+Version: 0.2.1
+Summary: A package that constructs JsonSchema validation error into error tree for Django Rest Framework with custom error message in compliance with the DRF error message.
+License: MIT License
+        
+        Copyright (c) 2023 Kira Technologies Pty Ltd
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+Keywords: jsonschema,drf
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+=============================
+drf-jsonschema
+=============================
+drf-jsonschema, created by Kiratech from extending `jsonschema <https://github.com/python-jsonschema/jsonschema>`_ package.
+This package provides JsonSchemaField and constructs JsonSchema validation error into error tree for Django Rest Framework with custom error message. 
+
+This package will install `jsonschema <https://github.com/python-jsonschema/jsonschema>`_ automatically so manual installation is not necessary.
+
+Quick Start
+-----------
+
+1. You can use JsonSchemaFieldValidator in Django's ``models.py`` as such::
+
+    from drf_jsonschema import JsonSchemaFieldValidator
+    ...
+    ...
+    json_data = models.JSONField(validators=[JsonSchemaFieldValidator(schema=your_json_schema)])
+
+2. On ``serializers.py``, modify the serializer field mapping from ``JSONField`` to ``JSONSchemaField`` as the example below::
+
+    from drf_jsonschema.serializers import JsonSchemaModelSerializer
+
+    class YourSerializer(JsonSchemaModelSerializer):
+        ...
+
+3. For more information, visit `jsonschema <https://github.com/python-jsonschema/jsonschema>`_
```

### Comparing `drf-jsonschema-0.2.0/README.rst` & `drf-jsonschema-0.2.1/README.rst`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-=============================
-drf-jsonschema
-=============================
-drf-jsonschema, created by Kiratech from extending `jsonschema <https://github.com/python-jsonschema/jsonschema>`_ package.
-This package provides JsonSchemaField and constructs JsonSchema validation error into error tree for Django Rest Framework with custom error message. 
-
-This package will install `jsonschema <https://github.com/python-jsonschema/jsonschema>`_ automatically so manual installation is not necessary.
-
-Quick Start
------------
-
-1. You can use JsonSchemaFieldValidator in Django's ``models.py`` as such::
-
-    from drf_jsonschema import JsonSchemaFieldValidator
-    ...
-    ...
-    json_data = models.JSONField(validators=[JsonSchemaFieldValidator(schema=your_json_schema)])
-
-2. On ``serializers.py``, modify the serializer field mapping from ``JSONField`` to ``JSONSchemaField`` as the example below::
-
-    from drf_jsonschema.serializers import JsonSchemaModelSerializer
-
-    class YourSerializer(JsonSchemaModelSerializer):
-        ...
-
-3. For more information, visit `jsonschema <https://github.com/python-jsonschema/jsonschema>`_ 
+=============================
+drf-jsonschema
+=============================
+drf-jsonschema, created by Kiratech from extending `jsonschema <https://github.com/python-jsonschema/jsonschema>`_ package.
+This package provides JsonSchemaField and constructs JsonSchema validation error into error tree for Django Rest Framework with custom error message. 
+
+This package will install `jsonschema <https://github.com/python-jsonschema/jsonschema>`_ automatically so manual installation is not necessary.
+
+Quick Start
+-----------
+
+1. You can use JsonSchemaFieldValidator in Django's ``models.py`` as such::
+
+    from drf_jsonschema import JsonSchemaFieldValidator
+    ...
+    ...
+    json_data = models.JSONField(validators=[JsonSchemaFieldValidator(schema=your_json_schema)])
+
+2. On ``serializers.py``, modify the serializer field mapping from ``JSONField`` to ``JSONSchemaField`` as the example below::
+
+    from drf_jsonschema.serializers import JsonSchemaModelSerializer
+
+    class YourSerializer(JsonSchemaModelSerializer):
+        ...
+
+3. For more information, visit `jsonschema <https://github.com/python-jsonschema/jsonschema>`_
```

### Comparing `drf-jsonschema-0.2.0/drf_jsonschema/_validators.py` & `drf-jsonschema-0.2.1/drf_jsonschema/_validators.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-from jsonschema import _validators
-from jsonschema.exceptions import ValidationError
-from django.utils.translation import gettext_lazy as _
-
-
-def format_message(message):
-    """
-    Format error message to keep a consistent outcome
-    """
-    return [_(message)]
-
-
-def required(validator, required, instance, schema):
-    """
-    Error for required field not provided
-    """
-    if not validator.is_type(instance, "object"):
-        return
-    for property in required:
-        if property not in instance:
-            yield ValidationError({
-                property:
-                format_message("This field is required.", ),
-            })
-
-
-def dependentRequired(validator, dependentRequired, instance, schema):
-    if not validator.is_type(instance, "object"):
-        return
-
-    for property, dependency in dependentRequired.items():
-        if property not in instance:
-            continue
-
-        for each in dependency:
-            if each not in instance:
-                message = f"{each!r} is a dependency of {property!r}"
-                yield ValidationError({
-                    each: format_message(message),
+from jsonschema.exceptions import ValidationError
+from django.utils.translation import gettext_lazy as _
+
+
+def format_message(message):
+    """
+    Format error message to keep a consistent outcome
+    """
+    return [_(message)]
+
+
+def required(validator, required, instance, schema):
+    """
+    Error for required field not provided
+    """
+    if not validator.is_type(instance, "object"):
+        return
+    for property in required:
+        if property not in instance:
+            yield ValidationError({
+                property:
+                format_message("This field is required.", ),
+            })
+
+
+def dependentRequired(validator, dependentRequired, instance, schema):
+    if not validator.is_type(instance, "object"):
+        return
+
+    for property, dependency in dependentRequired.items():
+        if property not in instance:
+            continue
+
+        for each in dependency:
+            if each not in instance:
+                message = f"{each!r} is a dependency of {property!r}"
+                yield ValidationError({
+                    each: format_message(message),
                 })
```

### Comparing `drf-jsonschema-0.2.0/drf_jsonschema/fields.py` & `drf-jsonschema-0.2.1/drf_jsonschema/fields.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,114 +1,114 @@
-from rest_framework.exceptions import ValidationError as DRFValidationError
-from rest_framework.fields import JSONField
-from .exceptions import SchemaValidationError
-from .validators import JsonSchemaFieldValidator
-
-
-class JSONSchemaField(JSONField):
-
-    def __init__(self, *args, **kwargs):
-        self.schema = kwargs.pop('schema', None)
-        super().__init__(*args, **kwargs)
-
-    def run_validators(self, value):
-        error_list = None
-        schema_validator = None
-
-        # Find JsonSchemaFieldValidator and removed it
-        # This is to prevent DRFValidationError raised before
-        # SchemaValidationError is caught.
-        # The JsonSchemaFieldValidator will be called and run manually
-        # after other validators are run.
-        for validator in self.validators:
-            if isinstance(validator, JsonSchemaFieldValidator):
-                schema_validator = validator
-                # Remove JsonSchemaFieldValidator to prevent running twice
-                self.validators.remove(validator)
-
-        try:
-            # Run other validators except for JsonSchemaFieldValidator
-            super().run_validators(value)
-
-        # Update error_dictionary with the error if rest_framework
-        # validation_error is raised
-        except DRFValidationError as e:
-            error_list = e.detail
-
-        try:
-            # Instantiate JsonSchemaFieldValidator if the validator
-            # is not found
-            if not schema_validator:
-                # Raise Exception if json schema is not found
-                if not self.schema or self.schema is None:
-                    raise ValueError("Missing json schema")
-                schema_validator = JsonSchemaFieldValidator(self.schema)
-
-            # Run our schema validator manually
-            schema_validator(value)
-
-            if error_list:
-                raise DRFValidationError(error_list)
-
-        except SchemaValidationError as e:
-            # Construct the error dictionary if SchemaValidationError is raised
-            error_tree = self.construct_error_dictionary(e.error_iterator)
-
-            if error_list:
-                errors = self._get_error_list(error_tree)
-                # Append DRFValidation error messages if found
-                for error_message in error_list:
-                    errors.append(error_message)
-
-            raise DRFValidationError(error_tree)
-
-    # Return a dictionary of errors.
-    def construct_error_dictionary(self, error_iterator: dict):
-        result = {}
-        for error in error_iterator:
-            nested = result
-
-            # Append error message if path is empty and error message is string
-            if not error.absolute_path and not isinstance(error.message, dict):
-                errors = self._get_error_list(nested)
-                errors.append(error.message)
-                continue
-            elif not error.absolute_path and isinstance(error.message, dict):
-                errors = self._append_error_message(error.message, nested)
-                continue
-            last_index = len(error.absolute_path) - 1
-
-            for index, step in enumerate(error.absolute_path):
-                # Create nested structure if index not last
-                nested = self._get_or_create_nested_dict(nested, step)
-
-                # Append error message if it is last index
-                if index == last_index:
-
-                    # Append error message if message is string
-                    if not isinstance(error.message, dict):
-                        errors = self._get_error_list(nested)
-                        errors.append(error.message)
-                    # Pass error.message (dict) to the method for structuring
-                    # error message
-                    else:
-                        errors = self._append_error_message(
-                            error.message, nested)
-        return result
-
-    def _get_or_create_nested_dict(self, obj: dict, key: str):
-        value = obj.get(key, {})
-        obj[key] = value
-        return value
-
-    def _get_error_list(self, obj: dict):
-        value = obj.get('errors', [])
-        obj['errors'] = value
-        return value
-
-    def _append_error_message(self, error: dict, nested: dict):
-        # Loop through error.message (dict) to append error message
-        for key, error_message in error.items():
-            nested = self._get_or_create_nested_dict(nested, key)
-            errors = self._get_error_list(nested)
-            errors.append(error_message[0])
-        return errors
+from rest_framework.exceptions import ValidationError as DRFValidationError
+from rest_framework.fields import JSONField
+from .exceptions import SchemaValidationError
+from .validators import JsonSchemaFieldValidator
+
+
+class JSONSchemaField(JSONField):
+
+    def __init__(self, *args, **kwargs):
+        self.schema = kwargs.pop('schema', None)
+        super().__init__(*args, **kwargs)
+
+    def run_validators(self, value):
+        error_list = None
+        schema_validator = None
+
+        # Find JsonSchemaFieldValidator and removed it
+        # This is to prevent DRFValidationError raised before
+        # SchemaValidationError is caught.
+        # The JsonSchemaFieldValidator will be called and run manually
+        # after other validators are run.
+        for validator in self.validators:
+            if isinstance(validator, JsonSchemaFieldValidator):
+                schema_validator = validator
+                # Remove JsonSchemaFieldValidator to prevent running twice
+                self.validators.remove(validator)
+
+        try:
+            # Run other validators except for JsonSchemaFieldValidator
+            super().run_validators(value)
+
+        # Update error_dictionary with the error if rest_framework
+        # validation_error is raised
+        except DRFValidationError as e:
+            error_list = e.detail
+
+        try:
+            # Instantiate JsonSchemaFieldValidator if the validator
+            # is not found
+            if not schema_validator:
+                # Raise Exception if json schema is not found
+                if not self.schema or self.schema is None:
+                    raise ValueError("Missing json schema")
+                schema_validator = JsonSchemaFieldValidator(self.schema)
+
+            # Run our schema validator manually
+            schema_validator(value)
+
+            if error_list:
+                raise DRFValidationError(error_list)
+
+        except SchemaValidationError as e:
+            # Construct the error dictionary if SchemaValidationError is raised
+            error_tree = self.construct_error_dictionary(e.error_iterator)
+
+            if error_list:
+                errors = self._get_error_list(error_tree)
+                # Append DRFValidation error messages if found
+                for error_message in error_list:
+                    errors.append(error_message)
+
+            raise DRFValidationError(error_tree)
+
+    # Return a dictionary of errors.
+    def construct_error_dictionary(self, error_iterator: dict):
+        result = {}
+        for error in error_iterator:
+            nested = result
+
+            # Append error message if path is empty and error message is string
+            if not error.absolute_path and not isinstance(error.message, dict):
+                errors = self._get_error_list(nested)
+                errors.append(error.message)
+                continue
+            elif not error.absolute_path and isinstance(error.message, dict):
+                errors = self._append_error_message(error.message, nested)
+                continue
+            last_index = len(error.absolute_path) - 1
+
+            for index, step in enumerate(error.absolute_path):
+                # Create nested structure if index not last
+                nested = self._get_or_create_nested_dict(nested, step)
+
+                # Append error message if it is last index
+                if index == last_index:
+
+                    # Append error message if message is string
+                    if not isinstance(error.message, dict):
+                        errors = self._get_error_list(nested)
+                        errors.append(error.message)
+                    # Pass error.message (dict) to the method for structuring
+                    # error message
+                    else:
+                        errors = self._append_error_message(
+                            error.message, nested)
+        return result
+
+    def _get_or_create_nested_dict(self, obj: dict, key: str):
+        value = obj.get(key, {})
+        obj[key] = value
+        return value
+
+    def _get_error_list(self, obj: dict):
+        value = obj.get('errors', [])
+        obj['errors'] = value
+        return value
+
+    def _append_error_message(self, error: dict, nested: dict):
+        # Loop through error.message (dict) to append error message
+        for key, error_message in error.items():
+            nested = self._get_or_create_nested_dict(nested, key)
+            errors = self._get_error_list(nested)
+            errors.append(error_message[0])
+        return errors
```

### Comparing `drf-jsonschema-0.2.0/drf_jsonschema/validators.py` & `drf-jsonschema-0.2.1/drf_jsonschema/validators.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-from django.utils.deconstruct import deconstructible
-from jsonschema import validators
-from . import _validators
-from .exceptions import SchemaValidationError
-
-# Custom validator that extends existing validator
-Draft202012ValidatorExtended = validators.extend(
-    validator=validators.Draft202012Validator,
-    validators={
-        'required': _validators.required,
-        'dependentRequired': _validators.dependentRequired
-    },
-)
-
-
-# Validate if json comply with JSONSchema
-@deconstructible
-class JsonSchemaFieldValidator():
-
-    def __init__(self, schema):
-        self.schema = schema
-
-    def __call__(self, value):
-        validator = Draft202012ValidatorExtended(self.schema)
-        # Pass `bool` as key function to preserve original order
-        error_iterator = sorted(validator.iter_errors(value), key=bool)
-        # error_iterator will be empty if no error is found
-        if not error_iterator:
-            return
-        error_list = self.convert_error_list(error_iterator)
-        # get nested dictionary of errors message
-        raise SchemaValidationError(error_list, error_iterator=error_iterator)
-
-    def convert_error_list(self, error_list):
-        # loop through error_list and store jsonschema properties name
-        # with json error message as key-value pairs
-        result = []
-        for error in error_list:
-            error_string = '"'
-            error_string += error.json_path
-            error_string += '": '
-            if (error.validator == 'required'
-                    or error.validator == 'dependentRequired'):
-                for key, value in error.message.items():
-                    error_string += f"'{key}'" + " " + value[0]
-            else:
-                error_string += error.message
-            result.append(error_string)
-        return result
+from django.utils.deconstruct import deconstructible
+from jsonschema import validators
+from . import _validators
+from .exceptions import SchemaValidationError
+
+# Custom validator that extends existing validator
+Draft202012ValidatorExtended = validators.extend(
+    validator=validators.Draft202012Validator,
+    validators={
+        'required': _validators.required,
+        'dependentRequired': _validators.dependentRequired
+    },
+)
+
+
+# Validate if json comply with JSONSchema
+@deconstructible
+class JsonSchemaFieldValidator():
+
+    def __init__(self, schema):
+        self.schema = schema
+
+    def __call__(self, value):
+        validator = Draft202012ValidatorExtended(self.schema)
+        # Pass `bool` as key function to preserve original order
+        error_iterator = sorted(validator.iter_errors(value), key=bool)
+        # error_iterator will be empty if no error is found
+        if not error_iterator:
+            return
+        error_list = self.convert_error_list(error_iterator)
+        # get nested dictionary of errors message
+        raise SchemaValidationError(error_list, error_iterator=error_iterator)
+
+    def convert_error_list(self, error_list):
+        # loop through error_list and store jsonschema properties name
+        # with json error message as key-value pairs
+        result = []
+        for error in error_list:
+            error_string = '"'
+            error_string += error.json_path
+            error_string += '": '
+            if (error.validator == 'required'
+                    or error.validator == 'dependentRequired'):
+                for key, value in error.message.items():
+                    error_string += f"'{key}'" + " " + value[0]
+            else:
+                error_string += error.message
+            result.append(error_string)
+        return result
```

### Comparing `drf-jsonschema-0.2.0/drf_jsonschema.egg-info/PKG-INFO` & `drf-jsonschema-0.2.1/drf_jsonschema.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-Metadata-Version: 2.1
-Name: drf-jsonschema
-Version: 0.2.0
-Summary: A package that constructs JsonSchema validation error into error tree for Django Rest Framework with custom error message in compliance with the DRF error message.
-License: MIT License
-        
-        Copyright (c) [year] [fullname]
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-Keywords: jsonschema,drf
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-=============================
-drf-jsonschema
-=============================
-drf-jsonschema, created by Kiratech from extending `jsonschema <https://github.com/python-jsonschema/jsonschema>`_ package.
-This package provides JsonSchemaField and constructs JsonSchema validation error into error tree for Django Rest Framework with custom error message. 
-
-This package will install `jsonschema <https://github.com/python-jsonschema/jsonschema>`_ automatically so manual installation is not necessary.
-
-Quick Start
------------
-
-1. You can use JsonSchemaFieldValidator in Django's ``models.py`` as such::
-
-    from drf_jsonschema import JsonSchemaFieldValidator
-    ...
-    ...
-    json_data = models.JSONField(validators=[JsonSchemaFieldValidator(schema=your_json_schema)])
-
-2. On ``serializers.py``, modify the serializer field mapping from ``JSONField`` to ``JSONSchemaField`` as the example below::
-
-    from drf_jsonschema.serializers import JsonSchemaModelSerializer
-
-    class YourSerializer(JsonSchemaModelSerializer):
-        ...
-
-3. For more information, visit `jsonschema <https://github.com/python-jsonschema/jsonschema>`_ 
+Metadata-Version: 2.1
+Name: drf-jsonschema
+Version: 0.2.1
+Summary: A package that constructs JsonSchema validation error into error tree for Django Rest Framework with custom error message in compliance with the DRF error message.
+License: MIT License
+        
+        Copyright (c) 2023 Kira Technologies Pty Ltd
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+Keywords: jsonschema,drf
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+=============================
+drf-jsonschema
+=============================
+drf-jsonschema, created by Kiratech from extending `jsonschema <https://github.com/python-jsonschema/jsonschema>`_ package.
+This package provides JsonSchemaField and constructs JsonSchema validation error into error tree for Django Rest Framework with custom error message. 
+
+This package will install `jsonschema <https://github.com/python-jsonschema/jsonschema>`_ automatically so manual installation is not necessary.
+
+Quick Start
+-----------
+
+1. You can use JsonSchemaFieldValidator in Django's ``models.py`` as such::
+
+    from drf_jsonschema import JsonSchemaFieldValidator
+    ...
+    ...
+    json_data = models.JSONField(validators=[JsonSchemaFieldValidator(schema=your_json_schema)])
+
+2. On ``serializers.py``, modify the serializer field mapping from ``JSONField`` to ``JSONSchemaField`` as the example below::
+
+    from drf_jsonschema.serializers import JsonSchemaModelSerializer
+
+    class YourSerializer(JsonSchemaModelSerializer):
+        ...
+
+3. For more information, visit `jsonschema <https://github.com/python-jsonschema/jsonschema>`_
```

### Comparing `drf-jsonschema-0.2.0/drf_jsonschema.egg-info/SOURCES.txt` & `drf-jsonschema-0.2.1/drf_jsonschema.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 pyproject.toml
 drf_jsonschema/__init__.py
 drf_jsonschema/_validators.py
 drf_jsonschema/apps.py
 drf_jsonschema/exceptions.py
 drf_jsonschema/fields.py
 drf_jsonschema/serializers.py
-drf_jsonschema/urls.py
 drf_jsonschema/validators.py
 drf_jsonschema.egg-info/PKG-INFO
 drf_jsonschema.egg-info/SOURCES.txt
 drf_jsonschema.egg-info/dependency_links.txt
 drf_jsonschema.egg-info/requires.txt
 drf_jsonschema.egg-info/top_level.txt
 drf_jsonschema/migrations/__init__.py
```

