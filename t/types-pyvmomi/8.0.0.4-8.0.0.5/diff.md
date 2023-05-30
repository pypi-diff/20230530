# Comparing `tmp/types-pyvmomi-8.0.0.4.tar.gz` & `tmp/types-pyvmomi-8.0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pyvmomi-8.0.0.4.tar", last modified: Wed May 10 18:24:01 2023, max compression
+gzip compressed data, was "types-pyvmomi-8.0.0.5.tar", last modified: Tue May 30 12:31:43 2023, max compression
```

## Comparing `types-pyvmomi-8.0.0.4.tar` & `types-pyvmomi-8.0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:24:01.518108 types-pyvmomi-8.0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-10 18:23:59.000000 types-pyvmomi-8.0.0.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 18:23:59.000000 types-pyvmomi-8.0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-10 18:24:01.518108 types-pyvmomi-8.0.0.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:24:01.514108 types-pyvmomi-8.0.0.4/pyVmomi-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-10 18:23:59.000000 types-pyvmomi-8.0.0.4/pyVmomi-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 18:23:44.000000 types-pyvmomi-8.0.0.4/pyVmomi-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:24:01.518108 types-pyvmomi-8.0.0.4/pyVmomi-stubs/vim/
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-10 18:23:44.000000 types-pyvmomi-8.0.0.4/pyVmomi-stubs/vim/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-10 18:23:44.000000 types-pyvmomi-8.0.0.4/pyVmomi-stubs/vim/event.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-10 18:23:44.000000 types-pyvmomi-8.0.0.4/pyVmomi-stubs/vim/fault.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-10 18:23:44.000000 types-pyvmomi-8.0.0.4/pyVmomi-stubs/vim/option.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-10 18:23:44.000000 types-pyvmomi-8.0.0.4/pyVmomi-stubs/vim/view.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:24:01.518108 types-pyvmomi-8.0.0.4/pyVmomi-stubs/vmodl/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-10 18:23:44.000000 types-pyvmomi-8.0.0.4/pyVmomi-stubs/vmodl/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-10 18:23:44.000000 types-pyvmomi-8.0.0.4/pyVmomi-stubs/vmodl/fault.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-10 18:23:44.000000 types-pyvmomi-8.0.0.4/pyVmomi-stubs/vmodl/query.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 18:24:01.518108 types-pyvmomi-8.0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-10 18:23:59.000000 types-pyvmomi-8.0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:24:01.518108 types-pyvmomi-8.0.0.4/types_pyvmomi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-05-10 18:24:01.000000 types-pyvmomi-8.0.0.4/types_pyvmomi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-10 18:24:01.000000 types-pyvmomi-8.0.0.4/types_pyvmomi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 18:24:01.000000 types-pyvmomi-8.0.0.4/types_pyvmomi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-10 18:24:01.000000 types-pyvmomi-8.0.0.4/types_pyvmomi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:43.413128 types-pyvmomi-8.0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-30 12:31:41.000000 types-pyvmomi-8.0.0.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-30 12:31:41.000000 types-pyvmomi-8.0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-30 12:31:43.413128 types-pyvmomi-8.0.0.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:43.409129 types-pyvmomi-8.0.0.5/pyVmomi-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-30 12:31:41.000000 types-pyvmomi-8.0.0.5/pyVmomi-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:26.000000 types-pyvmomi-8.0.0.5/pyVmomi-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:43.409129 types-pyvmomi-8.0.0.5/pyVmomi-stubs/vim/
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-30 12:31:26.000000 types-pyvmomi-8.0.0.5/pyVmomi-stubs/vim/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-30 12:31:26.000000 types-pyvmomi-8.0.0.5/pyVmomi-stubs/vim/event.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-30 12:31:26.000000 types-pyvmomi-8.0.0.5/pyVmomi-stubs/vim/fault.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-30 12:31:26.000000 types-pyvmomi-8.0.0.5/pyVmomi-stubs/vim/option.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-30 12:31:26.000000 types-pyvmomi-8.0.0.5/pyVmomi-stubs/vim/view.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:43.409129 types-pyvmomi-8.0.0.5/pyVmomi-stubs/vmodl/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-30 12:31:26.000000 types-pyvmomi-8.0.0.5/pyVmomi-stubs/vmodl/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-30 12:31:26.000000 types-pyvmomi-8.0.0.5/pyVmomi-stubs/vmodl/fault.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-30 12:31:26.000000 types-pyvmomi-8.0.0.5/pyVmomi-stubs/vmodl/query.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 12:31:43.413128 types-pyvmomi-8.0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-30 12:31:41.000000 types-pyvmomi-8.0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:31:43.413128 types-pyvmomi-8.0.0.5/types_pyvmomi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-30 12:31:43.000000 types-pyvmomi-8.0.0.5/types_pyvmomi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-30 12:31:43.000000 types-pyvmomi-8.0.0.5/types_pyvmomi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:31:43.000000 types-pyvmomi-8.0.0.5/types_pyvmomi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-30 12:31:43.000000 types-pyvmomi-8.0.0.5/types_pyvmomi.egg-info/top_level.txt
```

### Comparing `types-pyvmomi-8.0.0.4/CHANGELOG.md` & `types-pyvmomi-8.0.0.5/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 8.0.0.5 (2023-05-30)
+
+[stubsabot] Mark pyvmomi as obsolete since 8.0.1.0.1 (#10172)
+
 ## 8.0.0.4 (2023-05-10)
 
 Revert "[stubsabot] Mark pyvmomi as obsolete since 8.0.1.0 (#10148)" (#10171)
 
 This reverts commit 853d01d55ef5b5c7f0733e62c2e214be1d472657.
 
 ## 8.0.0.3 (2023-05-10)
```

### Comparing `types-pyvmomi-8.0.0.4/PKG-INFO` & `types-pyvmomi-8.0.0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyvmomi
-Version: 8.0.0.4
+Version: 8.0.0.5
 Summary: Typing stubs for pyvmomi
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyvmomi.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,14 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pyvmomi`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyvmomi. All fixes for
 types and metadata should be contributed there.
 
+*Note:* The `pyvmomi` package includes type annotations or type stubs
+since version 8.0.1.0.1. Please uninstall the `types-pyvmomi`
+package if you use this or a newer version.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `ecf4e708bff2f99d3297f801e52f0ba1d7ca0436`.
+This package was generated from typeshed commit `2ec6ba979f98c3c49d3a7ac2b11f1b3459e8e95a`.
```

### Comparing `types-pyvmomi-8.0.0.4/pyVmomi-stubs/vim/__init__.pyi` & `types-pyvmomi-8.0.0.5/pyVmomi-stubs/vim/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-pyvmomi-8.0.0.4/pyVmomi-stubs/vim/view.pyi` & `types-pyvmomi-8.0.0.5/pyVmomi-stubs/vim/view.pyi`

 * *Files identical despite different names*

### Comparing `types-pyvmomi-8.0.0.4/pyVmomi-stubs/vmodl/__init__.pyi` & `types-pyvmomi-8.0.0.5/pyVmomi-stubs/vmodl/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-pyvmomi-8.0.0.4/pyVmomi-stubs/vmodl/query.pyi` & `types-pyvmomi-8.0.0.5/pyVmomi-stubs/vmodl/query.pyi`

 * *Files identical despite different names*

### Comparing `types-pyvmomi-8.0.0.4/setup.py` & `types-pyvmomi-8.0.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,20 +11,25 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pyvmomi`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyvmomi. All fixes for
 types and metadata should be contributed there.
 
+*Note:* The `pyvmomi` package includes type annotations or type stubs
+since version 8.0.1.0.1. Please uninstall the `types-pyvmomi`
+package if you use this or a newer version.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `ecf4e708bff2f99d3297f801e52f0ba1d7ca0436`.
+This package was generated from typeshed commit `2ec6ba979f98c3c49d3a7ac2b11f1b3459e8e95a`.
 '''.lstrip()
 
 setup(name=name,
-      version="8.0.0.4",
+      version="8.0.0.5",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyvmomi.md",
```

### Comparing `types-pyvmomi-8.0.0.4/types_pyvmomi.egg-info/PKG-INFO` & `types-pyvmomi-8.0.0.5/types_pyvmomi.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pyvmomi
-Version: 8.0.0.4
+Version: 8.0.0.5
 Summary: Typing stubs for pyvmomi
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pyvmomi.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,14 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pyvmomi`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pyvmomi. All fixes for
 types and metadata should be contributed there.
 
+*Note:* The `pyvmomi` package includes type annotations or type stubs
+since version 8.0.1.0.1. Please uninstall the `types-pyvmomi`
+package if you use this or a newer version.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `ecf4e708bff2f99d3297f801e52f0ba1d7ca0436`.
+This package was generated from typeshed commit `2ec6ba979f98c3c49d3a7ac2b11f1b3459e8e95a`.
```

