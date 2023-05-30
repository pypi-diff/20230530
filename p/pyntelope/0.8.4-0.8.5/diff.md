# Comparing `tmp/pyntelope-0.8.4.tar.gz` & `tmp/pyntelope-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyntelope-0.8.4.tar", max compression
+gzip compressed data, was "pyntelope-0.8.5.tar", max compression
```

## Comparing `pyntelope-0.8.4.tar` & `pyntelope-0.8.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1064 2023-01-09 20:18:32.312701 pyntelope-0.8.4/LICENSE
--rw-r--r--   0        0        0     4618 2023-01-09 20:18:32.328702 pyntelope-0.8.4/README.md
--rw-r--r--   0        0        0      133 2023-01-09 20:18:32.316702 pyntelope-0.8.4/pyntelope/__init__.py
--rw-r--r--   0        0        0      115 2023-01-09 20:18:32.316702 pyntelope-0.8.4/pyntelope/_version.py
--rw-r--r--   0        0        0      484 2023-01-09 20:18:32.316702 pyntelope-0.8.4/pyntelope/exc.py
--rw-r--r--   0        0        0    10454 2023-05-18 16:33:44.672961 pyntelope-0.8.4/pyntelope/net.py
--rw-r--r--   0        0        0    10203 2023-01-09 20:18:32.316702 pyntelope-0.8.4/pyntelope/transaction.py
--rw-r--r--   0        0        0      933 2023-01-09 20:18:32.316702 pyntelope-0.8.4/pyntelope/types/__init__.py
--rw-r--r--   0        0        0      875 2023-01-09 20:18:32.316702 pyntelope-0.8.4/pyntelope/types/base.py
--rw-r--r--   0        0        0    11680 2023-01-09 20:18:32.316702 pyntelope-0.8.4/pyntelope/types/compostes.py
--rw-r--r--   0        0        0    17252 2023-01-09 20:18:32.316702 pyntelope-0.8.4/pyntelope/types/primitives.py
--rw-r--r--   0        0        0     8414 2023-03-27 18:18:22.970029 pyntelope-0.8.4/pyntelope/utils.py
--rw-r--r--   0        0        0      934 2023-05-18 16:57:38.810179 pyntelope-0.8.4/pyproject.toml
--rw-r--r--   0        0        0     5287 1970-01-01 00:00:00.000000 pyntelope-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-01-09 20:18:32.312701 pyntelope-0.8.5/LICENSE
+-rw-r--r--   0        0        0     4618 2023-01-09 20:18:32.328702 pyntelope-0.8.5/README.md
+-rw-r--r--   0        0        0      133 2023-01-09 20:18:32.316702 pyntelope-0.8.5/pyntelope/__init__.py
+-rw-r--r--   0        0        0      115 2023-01-09 20:18:32.316702 pyntelope-0.8.5/pyntelope/_version.py
+-rw-r--r--   0        0        0      484 2023-01-09 20:18:32.316702 pyntelope-0.8.5/pyntelope/exc.py
+-rw-r--r--   0        0        0    10575 2023-05-30 02:49:12.304752 pyntelope-0.8.5/pyntelope/net.py
+-rw-r--r--   0        0        0    10203 2023-01-09 20:18:32.316702 pyntelope-0.8.5/pyntelope/transaction.py
+-rw-r--r--   0        0        0      933 2023-01-09 20:18:32.316702 pyntelope-0.8.5/pyntelope/types/__init__.py
+-rw-r--r--   0        0        0      875 2023-01-09 20:18:32.316702 pyntelope-0.8.5/pyntelope/types/base.py
+-rw-r--r--   0        0        0    11680 2023-01-09 20:18:32.316702 pyntelope-0.8.5/pyntelope/types/compostes.py
+-rw-r--r--   0        0        0    17252 2023-01-09 20:18:32.316702 pyntelope-0.8.5/pyntelope/types/primitives.py
+-rw-r--r--   0        0        0     8414 2023-03-27 18:18:22.970029 pyntelope-0.8.5/pyntelope/utils.py
+-rw-r--r--   0        0        0      934 2023-05-30 02:51:18.085364 pyntelope-0.8.5/pyproject.toml
+-rw-r--r--   0        0        0     5287 1970-01-01 00:00:00.000000 pyntelope-0.8.5/PKG-INFO
```

### Comparing `pyntelope-0.8.4/LICENSE` & `pyntelope-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyntelope-0.8.4/README.md` & `pyntelope-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `pyntelope-0.8.4/pyntelope/net.py` & `pyntelope-0.8.5/pyntelope/net.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,16 +249,16 @@
             if "rows" not in data:
                 return data
             rows += data["rows"]
 
             if not full or not data.get("more"):
                 break
 
-            next_key = data["next_key"]
-            payload["lower_bound"] = next_key
+            lower_bound = data["next_key"]
+            payload["lower_bound"] = lower_bound
         else:
             raise ValueError("Too many requests (>1000) for table")
 
         return rows
 
     def push_transaction(
         self,
@@ -299,14 +299,18 @@
     host: pydantic.HttpUrl = "https://kylin.eossweden.org"
 
 
 class Jungle3Testnet(Net):
     host: pydantic.HttpUrl = "https://jungle3.eossweden.org"
 
 
+class Jungle4Testnet(Net):
+    host: pydantic.HttpUrl = "https://jungle4.api.eosnation.io"
+
+
 class TelosMainnet(Net):
     host: pydantic.HttpUrl = "https://telos.caleos.io/"
 
 
 class TelosTestnet(Net):
     host: pydantic.HttpUrl = "https://testnet.telos.detroitledger.tech"
 
@@ -332,14 +336,15 @@
 
 
 __all__ = [
     "Net",
     "EosMainnet",
     "KylinTestnet",
     "Jungle3Testnet",
+    "Jungle4Testnet",
     "TelosMainnet",
     "TelosTestnet",
     "ProtonMainnet",
     "ProtonTestnet",
     "UosMainnet",
     "FioMainnet",
     "WaxTestnet",
```

### Comparing `pyntelope-0.8.4/pyntelope/transaction.py` & `pyntelope-0.8.5/pyntelope/transaction.py`

 * *Files identical despite different names*

### Comparing `pyntelope-0.8.4/pyntelope/types/__init__.py` & `pyntelope-0.8.5/pyntelope/types/__init__.py`

 * *Files identical despite different names*

### Comparing `pyntelope-0.8.4/pyntelope/types/base.py` & `pyntelope-0.8.5/pyntelope/types/base.py`

 * *Files identical despite different names*

### Comparing `pyntelope-0.8.4/pyntelope/types/compostes.py` & `pyntelope-0.8.5/pyntelope/types/compostes.py`

 * *Files identical despite different names*

### Comparing `pyntelope-0.8.4/pyntelope/types/primitives.py` & `pyntelope-0.8.5/pyntelope/types/primitives.py`

 * *Files identical despite different names*

### Comparing `pyntelope-0.8.4/pyntelope/utils.py` & `pyntelope-0.8.5/pyntelope/utils.py`

 * *Files identical despite different names*

### Comparing `pyntelope-0.8.4/pyproject.toml` & `pyntelope-0.8.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyntelope"
-version = "0.8.4"
+version = "0.8.5"
 description = "Interact with Antelope blockchains"
 authors = ["Team <pyntelope@facings.io>"]
 homepage = "https://github.com/FACINGS/pyntelope"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `pyntelope-0.8.4/PKG-INFO` & `pyntelope-0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyntelope
-Version: 0.8.4
+Version: 0.8.5
 Summary: Interact with Antelope blockchains
 Home-page: https://github.com/FACINGS/pyntelope
 Author: Team
 Author-email: pyntelope@facings.io
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

