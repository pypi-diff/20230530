# Comparing `tmp/atlantisfastapi-0.3.0.tar.gz` & `tmp/atlantisfastapi-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlantisfastapi-0.3.0.tar", last modified: Wed Feb  1 14:47:17 2023, max compression
+gzip compressed data, was "atlantisfastapi-1.0.0.tar", last modified: Tue May 30 14:01:22 2023, max compression
```

## Comparing `atlantisfastapi-0.3.0.tar` & `atlantisfastapi-1.0.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 14:47:17.545418 atlantisfastapi-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-02-01 14:47:17.545418 atlantisfastapi-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-01 14:46:48.000000 atlantisfastapi-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 14:47:17.541418 atlantisfastapi-0.3.0/atlantisfastapi/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-02-01 14:46:48.000000 atlantisfastapi-0.3.0/atlantisfastapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-01 14:47:17.545418 atlantisfastapi-0.3.0/atlantisfastapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-02-01 14:47:17.000000 atlantisfastapi-0.3.0/atlantisfastapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-02-01 14:47:17.000000 atlantisfastapi-0.3.0/atlantisfastapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-01 14:47:17.000000 atlantisfastapi-0.3.0/atlantisfastapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-02-01 14:47:17.000000 atlantisfastapi-0.3.0/atlantisfastapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-01 14:47:17.000000 atlantisfastapi-0.3.0/atlantisfastapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-02-01 14:46:48.000000 atlantisfastapi-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-01 14:47:17.545418 atlantisfastapi-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:01:22.381628 atlantisfastapi-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-30 14:01:22.381628 atlantisfastapi-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-30 14:00:48.000000 atlantisfastapi-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:01:22.377628 atlantisfastapi-1.0.0/atlantisfastapi/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-30 14:00:48.000000 atlantisfastapi-1.0.0/atlantisfastapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 14:01:22.381628 atlantisfastapi-1.0.0/atlantisfastapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-30 14:01:22.000000 atlantisfastapi-1.0.0/atlantisfastapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-30 14:01:22.000000 atlantisfastapi-1.0.0/atlantisfastapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 14:01:22.000000 atlantisfastapi-1.0.0/atlantisfastapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-30 14:01:22.000000 atlantisfastapi-1.0.0/atlantisfastapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-30 14:01:22.000000 atlantisfastapi-1.0.0/atlantisfastapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-30 14:00:48.000000 atlantisfastapi-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 14:01:22.381628 atlantisfastapi-1.0.0/setup.cfg
```

### Comparing `atlantisfastapi-0.3.0/pyproject.toml` & `atlantisfastapi-1.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = ["setuptools>=62"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "atlantisfastapi"
-version = "0.3.0"
+version = "1.0.0"
 description = "atlantisfastapi"
 readme = "README.md"
 authors = [{ name = "Atlantis Labs", email = "r00tail@protonmail.com" }]
 dependencies = [
-    'coderfastapi ~= 0.8'
+    'coderfastapi ~= 1.9'
 ]
 
 [project.optional-dependencies]
 dev = [
     'black ~= 22.10.0'
 ]
 
 [tool.bumpver]
-current_version = "0.3.0"
+current_version = "1.0.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

