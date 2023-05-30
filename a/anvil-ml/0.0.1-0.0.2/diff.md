# Comparing `tmp/anvil_ml-0.0.1.tar.gz` & `tmp/anvil_ml-0.0.2.tar.gz`

## Comparing `anvil_ml-0.0.1.tar` & `anvil_ml-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anvil_ml-0.0.1/src/anvil-ml/__init__.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 anvil_ml-0.0.1/src/anvil-ml/example.py
--rw-r--r--   0        0        0    12077 2020-02-02 00:00:00.000000 anvil_ml-0.0.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 anvil_ml-0.0.1/LICENSE
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 anvil_ml-0.0.1/README.md
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 anvil_ml-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 anvil_ml-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 anvil_ml-0.0.2/requirements.txt
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 anvil_ml-0.0.2/src/example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anvil_ml-0.0.2/src/anvil_ml/__init__.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 anvil_ml-0.0.2/src/anvil_ml/main.py
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 anvil_ml-0.0.2/src/utils/logger.py
+-rw-r--r--   0        0        0    12077 2020-02-02 00:00:00.000000 anvil_ml-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 anvil_ml-0.0.2/LICENSE
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 anvil_ml-0.0.2/README.md
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 anvil_ml-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 anvil_ml-0.0.2/PKG-INFO
```

### Comparing `anvil_ml-0.0.1/.gitignore` & `anvil_ml-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `anvil_ml-0.0.1/LICENSE` & `anvil_ml-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `anvil_ml-0.0.1/pyproject.toml` & `anvil_ml-0.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
-name = "anvil-ml"
-version = "0.0.1"
+name = "anvil_ml"
+version = "0.0.2"
 authors = [
   { name="Dalton Walker", email="dev@daltonwalker.com" },
 ]
-description = "An ML testing tool."
+description = "Backend service for ForgeML"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `anvil_ml-0.0.1/PKG-INFO` & `anvil_ml-0.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
-Name: anvil-ml
-Version: 0.0.1
-Summary: An ML testing tool.
+Name: anvil_ml
+Version: 0.0.2
+Summary: Backend service for ForgeML
 Project-URL: Homepage, https://github.com/sigil-ml/Forge/tree/main
 Project-URL: Bug Tracker, https://github.com/sigil-ml/Forge/tree/main
 Author-email: Dalton Walker <dev@daltonwalker.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

