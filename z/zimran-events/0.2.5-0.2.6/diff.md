# Comparing `tmp/zimran-events-0.2.5.tar.gz` & `tmp/zimran-events-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zimran-events-0.2.5.tar", last modified: Thu Apr 20 06:21:01 2023, max compression
+gzip compressed data, was "zimran-events-0.2.6.tar", last modified: Tue May 30 05:02:41 2023, max compression
```

## Comparing `zimran-events-0.2.5.tar` & `zimran-events-0.2.6.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:21:01.935105 zimran-events-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-20 06:20:52.000000 zimran-events-0.2.5/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-20 06:20:52.000000 zimran-events-0.2.5/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-20 06:20:52.000000 zimran-events-0.2.5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:21:01.931105 zimran-events-0.2.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:21:01.935105 zimran-events-0.2.5/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-04-20 06:20:52.000000 zimran-events-0.2.5/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:21:01.935105 zimran-events-0.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-20 06:20:52.000000 zimran-events-0.2.5/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-20 06:20:52.000000 zimran-events-0.2.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-04-20 06:20:52.000000 zimran-events-0.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-20 06:20:52.000000 zimran-events-0.2.5/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-20 06:20:52.000000 zimran-events-0.2.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-20 06:20:52.000000 zimran-events-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-20 06:21:01.935105 zimran-events-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-20 06:20:52.000000 zimran-events-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-04-20 06:20:52.000000 zimran-events-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-20 06:20:52.000000 zimran-events-0.2.5/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 06:21:01.935105 zimran-events-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:21:01.931105 zimran-events-0.2.5/zimran/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:21:01.935105 zimran-events-0.2.5/zimran/events/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-20 06:20:52.000000 zimran-events-0.2.5/zimran/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-20 06:20:52.000000 zimran-events-0.2.5/zimran/events/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-20 06:20:52.000000 zimran-events-0.2.5/zimran/events/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-04-20 06:20:52.000000 zimran-events-0.2.5/zimran/events/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-20 06:20:52.000000 zimran-events-0.2.5/zimran/events/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-04-20 06:20:52.000000 zimran-events-0.2.5/zimran/events/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-20 06:20:52.000000 zimran-events-0.2.5/zimran/events/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-04-20 06:20:52.000000 zimran-events-0.2.5/zimran/events/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:21:01.935105 zimran-events-0.2.5/zimran_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-04-20 06:21:01.000000 zimran-events-0.2.5/zimran_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-20 06:21:01.000000 zimran-events-0.2.5/zimran_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 06:21:01.000000 zimran-events-0.2.5/zimran_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-20 06:21:01.000000 zimran-events-0.2.5/zimran_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 06:21:01.000000 zimran-events-0.2.5/zimran_events.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:02:41.695969 zimran-events-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 05:02:32.000000 zimran-events-0.2.6/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-30 05:02:32.000000 zimran-events-0.2.6/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-30 05:02:32.000000 zimran-events-0.2.6/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:02:41.687969 zimran-events-0.2.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:02:41.691969 zimran-events-0.2.6/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-05-30 05:02:32.000000 zimran-events-0.2.6/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:02:41.691969 zimran-events-0.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-30 05:02:32.000000 zimran-events-0.2.6/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-30 05:02:32.000000 zimran-events-0.2.6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-05-30 05:02:32.000000 zimran-events-0.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-30 05:02:32.000000 zimran-events-0.2.6/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-30 05:02:32.000000 zimran-events-0.2.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-30 05:02:32.000000 zimran-events-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-30 05:02:41.695969 zimran-events-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-05-30 05:02:32.000000 zimran-events-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-30 05:02:32.000000 zimran-events-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-30 05:02:32.000000 zimran-events-0.2.6/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 05:02:41.695969 zimran-events-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:02:41.691969 zimran-events-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-30 05:02:32.000000 zimran-events-0.2.6/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:02:41.687969 zimran-events-0.2.6/zimran/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:02:41.691969 zimran-events-0.2.6/zimran/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-30 05:02:32.000000 zimran-events-0.2.6/zimran/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-30 05:02:32.000000 zimran-events-0.2.6/zimran/events/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-30 05:02:32.000000 zimran-events-0.2.6/zimran/events/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-05-30 05:02:32.000000 zimran-events-0.2.6/zimran/events/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-30 05:02:32.000000 zimran-events-0.2.6/zimran/events/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-30 05:02:32.000000 zimran-events-0.2.6/zimran/events/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-05-30 05:02:32.000000 zimran-events-0.2.6/zimran/events/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-30 05:02:32.000000 zimran-events-0.2.6/zimran/events/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 05:02:41.695969 zimran-events-0.2.6/zimran_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-30 05:02:41.000000 zimran-events-0.2.6/zimran_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-30 05:02:41.000000 zimran-events-0.2.6/zimran_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 05:02:41.000000 zimran-events-0.2.6/zimran_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-30 05:02:41.000000 zimran-events-0.2.6/zimran_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-30 05:02:41.000000 zimran-events-0.2.6/zimran_events.egg-info/top_level.txt
```

### Comparing `zimran-events-0.2.5/.github/scripts/release.py` & `zimran-events-0.2.6/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.5/.gitignore` & `zimran-events-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.5/.pre-commit-config.yaml` & `zimran-events-0.2.6/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,16 @@
             --in-place,
             --remove-all-unused-imports,
             --ignore-init-module-imports,
             --remove-unused-variables,
           ]
         types: [python]
 
-  - repo: https://github.com/timothycrosley/isort
-    rev: 5.10.1
+  - repo: https://github.com/PyCQA/isort
+    rev: 5.12.0
     hooks:
       - id: isort
         name: Isort
         additional_dependencies: [toml]
         args: [--sp=.isort.cfg, -p=zimran]
         stages:
           - commit
```

### Comparing `zimran-events-0.2.5/LICENSE` & `zimran-events-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.5/PKG-INFO` & `zimran-events-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zimran-events
-Version: 0.2.5
+Version: 0.2.6
 Summary: The zimran-events provides amqp interface
 Author-email: Talgat Abdraimov <abdraimov.talga@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Talgat Abdraimov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `zimran-events-0.2.5/README.md` & `zimran-events-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.5/pyproject.toml` & `zimran-events-0.2.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zimran-events"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
   { name="Talgat Abdraimov", email="abdraimov.talga@gmail.com" },
 ]
 description = "The zimran-events provides amqp interface"
 readme = "README.md"
 requires-python = ">=3.10"
 license = { file = "LICENSE" }
```

### Comparing `zimran-events-0.2.5/zimran/events/connection.py` & `zimran-events-0.2.6/zimran/events/connection.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.5/zimran/events/consumer.py` & `zimran-events-0.2.6/zimran/events/consumer.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.5/zimran/events/producer.py` & `zimran-events-0.2.6/zimran/events/producer.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.5/zimran/events/schemas.py` & `zimran-events-0.2.6/zimran/events/schemas.py`

 * *Files identical despite different names*

### Comparing `zimran-events-0.2.5/zimran/events/utils.py` & `zimran-events-0.2.6/zimran/events/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,17 @@
 def cleanup_and_normalize_queue_name(queue_name: str):
     if '*' in queue_name:
         queue_name = queue_name.replace('*', '')
 
     if '#' in queue_name:
         queue_name = queue_name.replace('#', '')
 
+    if '..' in queue_name:
+        queue_name = queue_name.replace('..', '.')
+
     if queue_name.endswith('.'):
         queue_name = queue_name[:-1]
 
     return f'{queue_name}_q'
 
 
 def retry_policy(info):
```

### Comparing `zimran-events-0.2.5/zimran_events.egg-info/PKG-INFO` & `zimran-events-0.2.6/zimran_events.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zimran-events
-Version: 0.2.5
+Version: 0.2.6
 Summary: The zimran-events provides amqp interface
 Author-email: Talgat Abdraimov <abdraimov.talga@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Talgat Abdraimov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `zimran-events-0.2.5/zimran_events.egg-info/SOURCES.txt` & `zimran-events-0.2.6/zimran_events.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 LICENSE
 README.md
 pyproject.toml
 pytest.ini
 .github/scripts/release.py
 .github/workflows/publish.yml
 .github/workflows/release.yml
+tests/test_utils.py
 zimran/events/__init__.py
 zimran/events/connection.py
 zimran/events/constants.py
 zimran/events/consumer.py
 zimran/events/exceptions.py
 zimran/events/producer.py
 zimran/events/schemas.py
```

