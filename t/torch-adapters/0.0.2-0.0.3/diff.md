# Comparing `tmp/torch_adapters-0.0.2.tar.gz` & `tmp/torch_adapters-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_adapters-0.0.2.tar", max compression
+gzip compressed data, was "torch_adapters-0.0.3.tar", max compression
```

## Comparing `torch_adapters-0.0.2.tar` & `torch_adapters-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0     1062 2023-05-29 03:00:27.152099 torch_adapters-0.0.2/LICENSE
--rw-r--r--   0        0        0       16 2023-05-29 03:00:27.152099 torch_adapters-0.0.2/README.md
--rw-r--r--   0        0        0      344 2023-05-29 03:32:14.756743 torch_adapters-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-29 03:01:19.456108 torch_adapters-0.0.2/src/torch_adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 03:03:05.272210 torch_adapters-0.0.2/src/torch_adapters/adapters/__init__.py
--rw-r--r--   0        0        0      856 2023-05-29 03:15:43.714839 torch_adapters-0.0.2/src/torch_adapters/adapters/lora.py
--rw-r--r--   0        0        0      831 2023-05-29 03:28:01.368234 torch_adapters-0.0.2/src/torch_adapters/utils.py
--rw-r--r--   0        0        0      702 1970-01-01 00:00:00.000000 torch_adapters-0.0.2/setup.py
--rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 torch_adapters-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-29 03:00:27.152099 torch_adapters-0.0.3/LICENSE
+-rw-r--r--   0        0        0      223 2023-05-30 00:02:18.733760 torch_adapters-0.0.3/README.md
+-rw-r--r--   0        0        0      576 2023-05-29 22:43:21.437313 torch_adapters-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 03:01:19.456108 torch_adapters-0.0.3/src/torch_adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 03:03:05.272210 torch_adapters-0.0.3/src/torch_adapters/adapters/__init__.py
+-rw-r--r--   0        0        0     1146 2023-05-30 14:37:46.194482 torch_adapters-0.0.3/src/torch_adapters/adapters/lora.py
+-rw-r--r--   0        0        0      193 2023-05-30 14:23:42.706006 torch_adapters-0.0.3/src/torch_adapters/adapters/mixin.py
+-rw-r--r--   0        0        0     3078 2023-05-30 14:31:33.729317 torch_adapters-0.0.3/src/torch_adapters/adapters/prefix_tuning_embedding.py
+-rw-r--r--   0        0        0     3033 2023-05-30 14:37:46.906561 torch_adapters-0.0.3/src/torch_adapters/utils.py
+-rw-r--r--   0        0        0     1001 1970-01-01 00:00:00.000000 torch_adapters-0.0.3/setup.py
+-rw-r--r--   0        0        0      969 1970-01-01 00:00:00.000000 torch_adapters-0.0.3/PKG-INFO
```

### Comparing `torch_adapters-0.0.2/LICENSE` & `torch_adapters-0.0.3/LICENSE`

 * *Files identical despite different names*

