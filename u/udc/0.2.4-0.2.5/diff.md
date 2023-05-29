# Comparing `tmp/udc-0.2.4.tar.gz` & `tmp/udc-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "udc-0.2.4.tar", max compression
+gzip compressed data, was "udc-0.2.5.tar", max compression
```

## Comparing `udc-0.2.4.tar` & `udc-0.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11357 2023-05-12 01:09:39.984612 udc-0.2.4/LICENSE
--rw-r--r--   0        0        0     2527 2023-05-25 04:58:47.601734 udc-0.2.4/README.md
--rw-r--r--   0        0        0      749 2023-05-29 18:14:04.322921 udc-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      260 2023-05-30 01:15:44.000000 udc-0.2.4/udc/__init__.py
--rw-r--r--   0        0        0      340 2023-05-30 01:15:44.000000 udc-0.2.4/udc/benchling/__init__.py
--rw-r--r--   0        0        0     1248 2023-05-30 01:15:44.000000 udc-0.2.4/udc/benchling/entry.py
--rw-r--r--   0        0        0     1483 2023-05-30 01:15:44.000000 udc-0.2.4/udc/benchling/resource.py
--rw-r--r--   0        0        0     2257 2023-05-30 01:15:44.000000 udc-0.2.4/udc/benchling/root.py
--rw-r--r--   0        0        0      357 2023-05-30 01:15:44.000000 udc-0.2.4/udc/benchling/schema.py
--rw-r--r--   0        0        0      353 2023-05-30 01:15:44.000000 udc-0.2.4/udc/benchling/sequence.py
--rw-r--r--   0        0        0      331 2023-05-25 04:20:16.308186 udc-0.2.4/udc/main.py
--rw-r--r--   0        0        0       49 2023-05-25 04:58:47.606168 udc-0.2.4/udc/quilt/__init__.py
--rw-r--r--   0        0        0      275 2023-05-30 01:15:46.000000 udc-0.2.4/udc/quilt/resource.py
--rw-r--r--   0        0        0      467 2023-05-24 21:56:51.804905 udc-0.2.4/udc/types.py
--rw-r--r--   0        0        0     2502 2023-05-25 04:58:47.606836 udc-0.2.4/udc/un/cli.yaml
--rw-r--r--   0        0        0     3494 2023-05-30 01:15:46.000000 udc-0.2.4/udc/un/un_cli.py
--rw-r--r--   0        0        0     1265 2023-05-25 13:21:33.255738 udc-0.2.4/udc/un/un_uri.py
--rw-r--r--   0        0        0     2135 2023-05-30 01:24:50.000000 udc-0.2.4/udc/un/un_yaml.py
--rw-r--r--   0        0        0     3242 1970-01-01 00:00:00.000000 udc-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-12 01:09:39.984612 udc-0.2.5/LICENSE
+-rw-r--r--   0        0        0     2527 2023-05-25 04:58:47.601734 udc-0.2.5/README.md
+-rw-r--r--   0        0        0      750 2023-05-29 23:33:02.194201 udc-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      260 2023-05-29 18:47:36.753206 udc-0.2.5/udc/__init__.py
+-rw-r--r--   0        0        0      340 2023-05-29 18:47:36.753717 udc-0.2.5/udc/benchling/__init__.py
+-rw-r--r--   0        0        0     1248 2023-05-29 18:47:36.754096 udc-0.2.5/udc/benchling/entry.py
+-rw-r--r--   0        0        0     1483 2023-05-29 18:47:36.754504 udc-0.2.5/udc/benchling/resource.py
+-rw-r--r--   0        0        0     2257 2023-05-29 18:47:36.754873 udc-0.2.5/udc/benchling/root.py
+-rw-r--r--   0        0        0      357 2023-05-29 18:47:36.755234 udc-0.2.5/udc/benchling/schema.py
+-rw-r--r--   0        0        0      353 2023-05-29 18:47:36.755595 udc-0.2.5/udc/benchling/sequence.py
+-rw-r--r--   0        0        0      331 2023-05-25 04:20:16.308186 udc-0.2.5/udc/main.py
+-rw-r--r--   0        0        0       49 2023-05-25 04:58:47.606168 udc-0.2.5/udc/quilt/__init__.py
+-rw-r--r--   0        0        0      275 2023-05-29 18:47:36.755973 udc-0.2.5/udc/quilt/resource.py
+-rw-r--r--   0        0        0      467 2023-05-24 21:56:51.804905 udc-0.2.5/udc/types.py
+-rw-r--r--   0        0        0     2502 2023-05-25 04:58:47.606836 udc-0.2.5/udc/un/cli.yaml
+-rw-r--r--   0        0        0     3539 2023-05-29 23:32:28.314799 udc-0.2.5/udc/un/un_cli.py
+-rw-r--r--   0        0        0     1265 2023-05-25 13:21:33.255738 udc-0.2.5/udc/un/un_uri.py
+-rw-r--r--   0        0        0     2135 2023-05-29 18:47:36.756742 udc-0.2.5/udc/un/un_yaml.py
+-rw-r--r--   0        0        0     3185 1970-01-01 00:00:00.000000 udc-0.2.5/PKG-INFO
```

### Comparing `udc-0.2.4/LICENSE` & `udc-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `udc-0.2.4/README.md` & `udc-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `udc-0.2.4/pyproject.toml` & `udc-0.2.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "udc"
-version = "0.2.4"
+version = "0.2.5"
 description = ""
 authors = ["Ernest Prabhakar <ernest@quiltdata.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.9"
-anyio = "^3.6.2"
+python = "^3.10"
+anyio = "^3.7.0"
 trio = "^0.22.0"
 asyncclick = "^8.1.3.4"
 quilt3 = "^5.3.1"
 urllib3 = "<2"
 typing-extensions = "^4.5.0"
-quiltplus = "~0.8.1"
+quiltplus = ">0.8.0"
 #  quiltplus = {git = "https://github.com/quiltdata/quiltplus.git", rev = "main"}
 benchling-sdk = "^1.6.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest-coverage = "^0.0"
 pytest-watcher = "^0.2.6"
 pytest-asyncio = "^0.21.0"
```

### Comparing `udc-0.2.4/udc/benchling/entry.py` & `udc-0.2.5/udc/benchling/entry.py`

 * *Files identical despite different names*

### Comparing `udc-0.2.4/udc/benchling/resource.py` & `udc-0.2.5/udc/benchling/resource.py`

 * *Files identical despite different names*

### Comparing `udc-0.2.4/udc/benchling/root.py` & `udc-0.2.5/udc/benchling/root.py`

 * *Files identical despite different names*

### Comparing `udc-0.2.4/udc/un/cli.yaml` & `udc-0.2.5/udc/un/cli.yaml`

 * *Files identical despite different names*

### Comparing `udc-0.2.4/udc/un/un_cli.py` & `udc-0.2.5/udc/un/un_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,15 @@
         """Print result of calling a method."""
         [print(item, file=out) for item in results]
         return out
 
     def get_resource(self, uri: str) -> Listable:
         parsed = UnUri(uri)
         handler = self.get_handler(parsed.tool())
+        logging.debug(f"handler: {handler}")
         return handler(parsed)
 
     async def list(self, args: Namespace):
         """Return contents of a URI."""
         res = self.get_resource(args.uri)
         return await res.list()
```

### Comparing `udc-0.2.4/udc/un/un_uri.py` & `udc-0.2.5/udc/un/un_uri.py`

 * *Files identical despite different names*

### Comparing `udc-0.2.4/udc/un/un_yaml.py` & `udc-0.2.5/udc/un/un_yaml.py`

 * *Files identical despite different names*

### Comparing `udc-0.2.4/PKG-INFO` & `udc-0.2.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: udc
-Version: 0.2.4
+Version: 0.2.5
 Summary: 
 Author: Ernest Prabhakar
 Author-email: ernest@quiltdata.io
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: anyio (>=3.6.2,<4.0.0)
+Requires-Dist: anyio (>=3.7.0,<4.0.0)
 Requires-Dist: asyncclick (>=8.1.3.4,<9.0.0.0)
 Requires-Dist: benchling-sdk (>=1.6.1,<2.0.0)
 Requires-Dist: quilt3 (>=5.3.1,<6.0.0)
-Requires-Dist: quiltplus (>=0.8.1,<0.9.0)
+Requires-Dist: quiltplus (>0.8.0)
 Requires-Dist: trio (>=0.22.0,<0.23.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Requires-Dist: urllib3 (<2)
 Description-Content-Type: text/markdown
 
 # UDC
```

