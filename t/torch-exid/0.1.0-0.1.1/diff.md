# Comparing `tmp/torch_exid-0.1.0.tar.gz` & `tmp/torch_exid-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_exid-0.1.0.tar", max compression
+gzip compressed data, was "torch_exid-0.1.1.tar", max compression
```

## Comparing `torch_exid-0.1.0.tar` & `torch_exid-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1070 2023-05-29 16:57:48.668360 torch_exid-0.1.0/LICENSE
--rw-r--r--   0        0        0      326 2023-05-30 11:48:28.587643 torch_exid-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       42 2023-05-30 11:21:53.579141 torch_exid-0.1.0/src/torch_exid/__init__.py
--rw-r--r--   0        0        0     6149 2023-05-30 11:46:38.938874 torch_exid-0.1.0/src/torch_exid/exid.py
--rw-r--r--   0        0        0      654 2023-05-30 11:52:30.438459 torch_exid-0.1.0/setup.py
--rw-r--r--   0        0        0      289 2023-05-30 11:52:30.438590 torch_exid-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-29 16:57:48.668360 torch_exid-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3500 2023-05-30 12:06:37.235950 torch_exid-0.1.1/README.md
+-rw-r--r--   0        0        0      472 2023-05-30 12:06:31.339064 torch_exid-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-05-30 11:21:53.579141 torch_exid-0.1.1/src/torch_exid/__init__.py
+-rw-r--r--   0        0        0     6149 2023-05-30 11:46:38.938874 torch_exid-0.1.1/src/torch_exid/exid.py
+-rw-r--r--   0        0        0     4395 2023-05-30 12:07:18.556105 torch_exid-0.1.1/setup.py
+-rw-r--r--   0        0        0     4056 2023-05-30 12:07:18.556279 torch_exid-0.1.1/PKG-INFO
```

### Comparing `torch_exid-0.1.0/LICENSE` & `torch_exid-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_exid-0.1.0/src/torch_exid/exid.py` & `torch_exid-0.1.1/src/torch_exid/exid.py`

 * *Files identical despite different names*

