# Comparing `tmp/drf-jsonschema-0.2.1.tar.gz` & `tmp/drf-jsonschema-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-jsonschema-0.2.1.tar", last modified: Tue May 30 00:06:27 2023, max compression
+gzip compressed data, was "drf-jsonschema-0.2.2.tar", last modified: Tue May 30 08:23:19 2023, max compression
```

## Comparing `drf-jsonschema-0.2.1.tar` & `drf-jsonschema-0.2.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 00:06:27.529634 drf-jsonschema-0.2.1/
--rw-rw-rw-   0        0        0     1101 2023-05-29 23:57:30.000000 drf-jsonschema-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     2775 2023-05-30 00:06:27.528633 drf-jsonschema-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1155 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-30 00:06:27.482591 drf-jsonschema-0.2.1/drf_jsonschema/
--rw-rw-rw-   0        0        0        0 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.1/drf_jsonschema/__init__.py
--rw-rw-rw-   0        0        0     1156 2023-05-30 00:02:40.000000 drf-jsonschema-0.2.1/drf_jsonschema/_validators.py
--rw-rw-rw-   0        0        0      144 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.1/drf_jsonschema/apps.py
--rw-rw-rw-   0        0        0      314 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.1/drf_jsonschema/exceptions.py
--rw-rw-rw-   0        0        0     4664 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.1/drf_jsonschema/fields.py
-drwxrwxrwx   0        0        0        0 2023-05-30 00:06:27.502609 drf-jsonschema-0.2.1/drf_jsonschema/migrations/
--rw-rw-rw-   0        0        0        0 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.1/drf_jsonschema/migrations/__init__.py
--rw-rw-rw-   0        0        0      357 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.1/drf_jsonschema/serializers.py
-drwxrwxrwx   0        0        0        0 2023-05-30 00:06:27.527632 drf-jsonschema-0.2.1/drf_jsonschema/tests/
--rw-rw-rw-   0        0        0        0 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.1/drf_jsonschema/tests/__init__.py
--rw-rw-rw-   0        0        0      886 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.1/drf_jsonschema/tests/models.py
--rw-rw-rw-   0        0        0      250 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.1/drf_jsonschema/tests/serializers.py
--rw-rw-rw-   0        0        0     2080 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.1/drf_jsonschema/tests/test_json_schema_field_validator.py
--rw-rw-rw-   0        0        0        0 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.1/drf_jsonschema/tests/test_views.py
--rw-rw-rw-   0        0        0     1566 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.1/drf_jsonschema/tests/views.py
--rw-rw-rw-   0        0        0     1862 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.1/drf_jsonschema/validators.py
-drwxrwxrwx   0        0        0        0 2023-05-30 00:06:27.501609 drf-jsonschema-0.2.1/drf_jsonschema.egg-info/
--rw-rw-rw-   0        0        0     2775 2023-05-30 00:06:27.000000 drf-jsonschema-0.2.1/drf_jsonschema.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      675 2023-05-30 00:06:27.000000 drf-jsonschema-0.2.1/drf_jsonschema.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 00:06:27.000000 drf-jsonschema-0.2.1/drf_jsonschema.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-05-30 00:06:27.000000 drf-jsonschema-0.2.1/drf_jsonschema.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-30 00:06:27.000000 drf-jsonschema-0.2.1/drf_jsonschema.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      484 2023-05-30 00:00:09.000000 drf-jsonschema-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-30 00:06:27.529634 drf-jsonschema-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-30 08:23:19.763620 drf-jsonschema-0.2.2/
+-rw-rw-rw-   0        0        0     1101 2023-05-29 23:57:30.000000 drf-jsonschema-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     2775 2023-05-30 08:23:19.762618 drf-jsonschema-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1155 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-30 08:23:19.734594 drf-jsonschema-0.2.2/drf_jsonschema/
+-rw-rw-rw-   0        0        0        0 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.2/drf_jsonschema/__init__.py
+-rw-rw-rw-   0        0        0     1156 2023-05-30 00:02:40.000000 drf-jsonschema-0.2.2/drf_jsonschema/_validators.py
+-rw-rw-rw-   0        0        0      144 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.2/drf_jsonschema/apps.py
+-rw-rw-rw-   0        0        0      314 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.2/drf_jsonschema/exceptions.py
+-rw-rw-rw-   0        0        0     4664 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.2/drf_jsonschema/fields.py
+drwxrwxrwx   0        0        0        0 2023-05-30 08:23:19.755613 drf-jsonschema-0.2.2/drf_jsonschema/migrations/
+-rw-rw-rw-   0        0        0        0 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.2/drf_jsonschema/migrations/__init__.py
+-rw-rw-rw-   0        0        0      357 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.2/drf_jsonschema/serializers.py
+drwxrwxrwx   0        0        0        0 2023-05-30 08:23:19.761617 drf-jsonschema-0.2.2/drf_jsonschema/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.2/drf_jsonschema/tests/__init__.py
+-rw-rw-rw-   0        0        0      886 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.2/drf_jsonschema/tests/models.py
+-rw-rw-rw-   0        0        0      250 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.2/drf_jsonschema/tests/serializers.py
+-rw-rw-rw-   0        0        0     2080 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.2/drf_jsonschema/tests/test_json_schema_field_validator.py
+-rw-rw-rw-   0        0        0        0 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.2/drf_jsonschema/tests/test_views.py
+-rw-rw-rw-   0        0        0     1566 2023-05-29 23:52:19.000000 drf-jsonschema-0.2.2/drf_jsonschema/tests/views.py
+-rw-rw-rw-   0        0        0     1177 2023-05-30 07:17:04.000000 drf-jsonschema-0.2.2/drf_jsonschema/validators.py
+drwxrwxrwx   0        0        0        0 2023-05-30 08:23:19.754611 drf-jsonschema-0.2.2/drf_jsonschema.egg-info/
+-rw-rw-rw-   0        0        0     2775 2023-05-30 08:23:19.000000 drf-jsonschema-0.2.2/drf_jsonschema.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      675 2023-05-30 08:23:19.000000 drf-jsonschema-0.2.2/drf_jsonschema.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 08:23:19.000000 drf-jsonschema-0.2.2/drf_jsonschema.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-05-30 08:23:19.000000 drf-jsonschema-0.2.2/drf_jsonschema.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-30 08:23:19.000000 drf-jsonschema-0.2.2/drf_jsonschema.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      664 2023-05-30 08:22:06.000000 drf-jsonschema-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-30 08:23:19.763620 drf-jsonschema-0.2.2/setup.cfg
```

### Comparing `drf-jsonschema-0.2.1/LICENSE` & `drf-jsonschema-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-jsonschema-0.2.1/PKG-INFO` & `drf-jsonschema-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-jsonschema
-Version: 0.2.1
+Version: 0.2.2
 Summary: A package that constructs JsonSchema validation error into error tree for Django Rest Framework with custom error message in compliance with the DRF error message.
 License: MIT License
         
         Copyright (c) 2023 Kira Technologies Pty Ltd
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `drf-jsonschema-0.2.1/README.rst` & `drf-jsonschema-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `drf-jsonschema-0.2.1/drf_jsonschema/_validators.py` & `drf-jsonschema-0.2.2/drf_jsonschema/_validators.py`

 * *Files identical despite different names*

### Comparing `drf-jsonschema-0.2.1/drf_jsonschema/fields.py` & `drf-jsonschema-0.2.2/drf_jsonschema/fields.py`

 * *Files identical despite different names*

### Comparing `drf-jsonschema-0.2.1/drf_jsonschema/tests/models.py` & `drf-jsonschema-0.2.2/drf_jsonschema/tests/models.py`

 * *Files identical despite different names*

### Comparing `drf-jsonschema-0.2.1/drf_jsonschema/tests/test_json_schema_field_validator.py` & `drf-jsonschema-0.2.2/drf_jsonschema/tests/test_json_schema_field_validator.py`

 * *Files identical despite different names*

### Comparing `drf-jsonschema-0.2.1/drf_jsonschema/tests/views.py` & `drf-jsonschema-0.2.2/drf_jsonschema/tests/views.py`

 * *Files identical despite different names*

### Comparing `drf-jsonschema-0.2.1/drf_jsonschema.egg-info/PKG-INFO` & `drf-jsonschema-0.2.2/drf_jsonschema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-jsonschema
-Version: 0.2.1
+Version: 0.2.2
 Summary: A package that constructs JsonSchema validation error into error tree for Django Rest Framework with custom error message in compliance with the DRF error message.
 License: MIT License
         
         Copyright (c) 2023 Kira Technologies Pty Ltd
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `drf-jsonschema-0.2.1/drf_jsonschema.egg-info/SOURCES.txt` & `drf-jsonschema-0.2.2/drf_jsonschema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

