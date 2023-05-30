# Comparing `tmp/cerebrium-0.5.1.tar.gz` & `tmp/cerebrium-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerebrium-0.5.1.tar", max compression
+gzip compressed data, was "cerebrium-0.5.2.tar", max compression
```

## Comparing `cerebrium-0.5.1.tar` & `cerebrium-0.5.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    34594 2023-05-18 18:57:55.262934 cerebrium-0.5.1/LICENSE
--rw-r--r--   0        0        0     3055 2023-05-18 18:57:55.262934 cerebrium-0.5.1/README.md
--rw-r--r--   0        0        0      285 2023-05-18 19:02:29.891752 cerebrium-0.5.1/cerebrium/__init__.py
--rw-r--r--   0        0        0    29945 2023-05-18 18:57:55.262934 cerebrium-0.5.1/cerebrium/conduit.py
--rw-r--r--   0        0        0     4451 2023-05-18 18:57:55.262934 cerebrium-0.5.1/cerebrium/core.py
--rw-r--r--   0        0        0     2524 2023-05-18 18:57:55.262934 cerebrium-0.5.1/cerebrium/errors.py
--rw-r--r--   0        0        0    10839 2023-05-18 18:57:55.262934 cerebrium-0.5.1/cerebrium/flow.py
--rw-r--r--   0        0        0     2807 2023-05-18 18:57:55.262934 cerebrium-0.5.1/cerebrium/logging/arize.py
--rw-r--r--   0        0        0      705 2023-05-18 18:57:55.262934 cerebrium-0.5.1/cerebrium/logging/base.py
--rw-r--r--   0        0        0     3855 2023-05-18 18:57:55.262934 cerebrium-0.5.1/cerebrium/logging/censius.py
--rw-r--r--   0        0        0      801 2023-05-18 18:57:55.262934 cerebrium-0.5.1/cerebrium/models/base.py
--rw-r--r--   0        0        0      446 2023-05-18 18:57:55.262934 cerebrium-0.5.1/cerebrium/models/hf_pipeline.py
--rw-r--r--   0        0        0      418 2023-05-18 18:57:55.262934 cerebrium-0.5.1/cerebrium/models/onnx.py
--rw-r--r--   0        0        0     1116 2023-05-18 18:57:55.262934 cerebrium-0.5.1/cerebrium/models/sklearn.py
--rw-r--r--   0        0        0      244 2023-05-18 18:57:55.262934 cerebrium-0.5.1/cerebrium/models/spacy.py
--rw-r--r--   0        0        0      342 2023-05-18 18:57:55.262934 cerebrium-0.5.1/cerebrium/models/torch.py
--rw-r--r--   0        0        0     4555 2023-05-18 18:57:55.262934 cerebrium-0.5.1/cerebrium/requests.py
--rw-r--r--   0        0        0      465 2023-05-18 18:57:55.262934 cerebrium-0.5.1/cerebrium/utils.py
--rw-r--r--   0        0        0     2353 2023-05-18 19:02:29.887751 cerebrium-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     5088 1970-01-01 00:00:00.000000 cerebrium-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    34594 2023-05-30 15:25:09.283336 cerebrium-0.5.2/LICENSE
+-rw-r--r--   0        0        0     3055 2023-05-30 15:25:09.283336 cerebrium-0.5.2/README.md
+-rw-r--r--   0        0        0      285 2023-05-30 15:30:01.255157 cerebrium-0.5.2/cerebrium/__init__.py
+-rw-r--r--   0        0        0    29945 2023-05-30 15:25:09.283336 cerebrium-0.5.2/cerebrium/conduit.py
+-rw-r--r--   0        0        0     4451 2023-05-30 15:25:09.283336 cerebrium-0.5.2/cerebrium/core.py
+-rw-r--r--   0        0        0     2524 2023-05-30 15:25:09.283336 cerebrium-0.5.2/cerebrium/errors.py
+-rw-r--r--   0        0        0    10839 2023-05-30 15:25:09.283336 cerebrium-0.5.2/cerebrium/flow.py
+-rw-r--r--   0        0        0     2807 2023-05-30 15:25:09.283336 cerebrium-0.5.2/cerebrium/logging/arize.py
+-rw-r--r--   0        0        0      705 2023-05-30 15:25:09.283336 cerebrium-0.5.2/cerebrium/logging/base.py
+-rw-r--r--   0        0        0     3855 2023-05-30 15:25:09.283336 cerebrium-0.5.2/cerebrium/logging/censius.py
+-rw-r--r--   0        0        0      801 2023-05-30 15:25:09.283336 cerebrium-0.5.2/cerebrium/models/base.py
+-rw-r--r--   0        0        0      446 2023-05-30 15:25:09.283336 cerebrium-0.5.2/cerebrium/models/hf_pipeline.py
+-rw-r--r--   0        0        0      418 2023-05-30 15:25:09.283336 cerebrium-0.5.2/cerebrium/models/onnx.py
+-rw-r--r--   0        0        0     1116 2023-05-30 15:25:09.283336 cerebrium-0.5.2/cerebrium/models/sklearn.py
+-rw-r--r--   0        0        0      244 2023-05-30 15:25:09.283336 cerebrium-0.5.2/cerebrium/models/spacy.py
+-rw-r--r--   0        0        0      342 2023-05-30 15:25:09.283336 cerebrium-0.5.2/cerebrium/models/torch.py
+-rw-r--r--   0        0        0     4555 2023-05-30 15:25:09.283336 cerebrium-0.5.2/cerebrium/requests.py
+-rw-r--r--   0        0        0      465 2023-05-30 15:25:09.283336 cerebrium-0.5.2/cerebrium/utils.py
+-rw-r--r--   0        0        0     2353 2023-05-30 15:30:01.255157 cerebrium-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     5088 1970-01-01 00:00:00.000000 cerebrium-0.5.2/PKG-INFO
```

### Comparing `cerebrium-0.5.1/LICENSE` & `cerebrium-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cerebrium-0.5.1/README.md` & `cerebrium-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `cerebrium-0.5.1/cerebrium/conduit.py` & `cerebrium-0.5.2/cerebrium/conduit.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.5.1/cerebrium/core.py` & `cerebrium-0.5.2/cerebrium/core.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.5.1/cerebrium/errors.py` & `cerebrium-0.5.2/cerebrium/errors.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.5.1/cerebrium/flow.py` & `cerebrium-0.5.2/cerebrium/flow.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.5.1/cerebrium/logging/arize.py` & `cerebrium-0.5.2/cerebrium/logging/arize.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.5.1/cerebrium/logging/base.py` & `cerebrium-0.5.2/cerebrium/logging/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.5.1/cerebrium/logging/censius.py` & `cerebrium-0.5.2/cerebrium/logging/censius.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.5.1/cerebrium/models/base.py` & `cerebrium-0.5.2/cerebrium/models/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.5.1/cerebrium/models/sklearn.py` & `cerebrium-0.5.2/cerebrium/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.5.1/cerebrium/requests.py` & `cerebrium-0.5.2/cerebrium/requests.py`

 * *Files identical despite different names*

### Comparing `cerebrium-0.5.1/pyproject.toml` & `cerebrium-0.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cerebrium"
-version = "0.5.1"
+version = "0.5.2"
 description = ""
 authors = ["Elijah Roussos <elijah@cerebrium.ai>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 exclude = ["tests/*", "dist/*", "worker/*"]
 
 [tool.poetry.urls]
```

### Comparing `cerebrium-0.5.1/PKG-INFO` & `cerebrium-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerebrium
-Version: 0.5.1
+Version: 0.5.2
 Summary: 
 License: AGPL-3.0-only
 Author: Elijah Roussos
 Author-email: elijah@cerebrium.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

