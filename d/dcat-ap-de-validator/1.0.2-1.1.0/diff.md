# Comparing `tmp/dcat_ap_de_validator-1.0.2.tar.gz` & `tmp/dcat_ap_de_validator-1.1.0.tar.gz`

## Comparing `dcat_ap_de_validator-1.0.2.tar` & `dcat_ap_de_validator-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.0.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.0.2/.github/workflows/release.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.0.2/dcat_ap_de_validator/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.0.2/dcat_ap_de_validator/__init__.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.0.2/dcat_ap_de_validator/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.0.2/dcat_ap_de_validator/commands/__init__.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.0.2/dcat_ap_de_validator/commands/portal.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.0.2/dcat_ap_de_validator/metadata/__init__.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.0.2/dcat_ap_de_validator/metadata/validate.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.0.2/dcat_ap_de_validator/portals/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.0.2/dcat_ap_de_validator/tests/__init__.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.0.2/dcat_ap_de_validator/tests/conftest.py
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.0.2/dcat_ap_de_validator/tests/test_commands.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.0.2/dcat_ap_de_validator/tests/test_validation.py
--rw-r--r--   0        0        0    25948 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.0.2/dcat_ap_de_validator/tests/cassettes/heilbronn.yaml
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.0.2/LICENSE
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.0.2/Readme.md
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.1.0/Changelog.md
+-rw-r--r--   0        0        0    33769 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.1.0/screenshot.png
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.1.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.1.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.1.0/dcat_ap_de_validator/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.1.0/dcat_ap_de_validator/__init__.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.1.0/dcat_ap_de_validator/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.1.0/dcat_ap_de_validator/commands/__init__.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.1.0/dcat_ap_de_validator/commands/portal.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.1.0/dcat_ap_de_validator/metadata/__init__.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.1.0/dcat_ap_de_validator/metadata/validate.py
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.1.0/dcat_ap_de_validator/portals/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.1.0/dcat_ap_de_validator/tests/__init__.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.1.0/dcat_ap_de_validator/tests/conftest.py
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.1.0/dcat_ap_de_validator/tests/test_commands.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.1.0/dcat_ap_de_validator/tests/test_validation.py
+-rw-r--r--   0        0        0    25948 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.1.0/dcat_ap_de_validator/tests/cassettes/heilbronn.yaml
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.1.0/LICENSE
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.1.0/Readme.md
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 dcat_ap_de_validator-1.1.0/PKG-INFO
```

### Comparing `dcat_ap_de_validator-1.0.2/.github/workflows/ci.yml` & `dcat_ap_de_validator-1.1.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `dcat_ap_de_validator-1.0.2/.github/workflows/release.yml` & `dcat_ap_de_validator-1.1.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dcat_ap_de_validator-1.0.2/dcat_ap_de_validator/__main__.py` & `dcat_ap_de_validator-1.1.0/dcat_ap_de_validator/__main__.py`

 * *Files identical despite different names*

### Comparing `dcat_ap_de_validator-1.0.2/dcat_ap_de_validator/metadata/validate.py` & `dcat_ap_de_validator-1.1.0/dcat_ap_de_validator/metadata/validate.py`

 * *Files identical despite different names*

### Comparing `dcat_ap_de_validator-1.0.2/dcat_ap_de_validator/portals/__init__.py` & `dcat_ap_de_validator-1.1.0/dcat_ap_de_validator/portals/__init__.py`

 * *Files identical despite different names*

### Comparing `dcat_ap_de_validator-1.0.2/dcat_ap_de_validator/tests/test_commands.py` & `dcat_ap_de_validator-1.1.0/dcat_ap_de_validator/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `dcat_ap_de_validator-1.0.2/dcat_ap_de_validator/tests/test_validation.py` & `dcat_ap_de_validator-1.1.0/dcat_ap_de_validator/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `dcat_ap_de_validator-1.0.2/dcat_ap_de_validator/tests/cassettes/heilbronn.yaml` & `dcat_ap_de_validator-1.1.0/dcat_ap_de_validator/tests/cassettes/heilbronn.yaml`

 * *Files identical despite different names*

### Comparing `dcat_ap_de_validator-1.0.2/LICENSE` & `dcat_ap_de_validator-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dcat_ap_de_validator-1.0.2/Readme.md` & `dcat_ap_de_validator-1.1.0/Readme.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Validierung von Metadaten pro Portal 
 
 Wir können eine Portal URL (DKAN oder CKAN Portale) übergeben und dann bekommen wir eine
 JSON Datei mit der Validierung aller vorhandenen Datensätze.
 
+![console screenshot](screenshot.png)
+
 
 # Installation
 Zur Installation des Packages mit pipx (pip geht auch):
 
 ```bash
 pipx install dcat-ap-de-validator
 ```
```

### Comparing `dcat_ap_de_validator-1.0.2/pyproject.toml` & `dcat_ap_de_validator-1.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 	"Programming Language :: Python :: 3.9",
 	"Programming Language :: Python :: 3.10",
 	"Programming Language :: Python :: 3.11",
 
 ]
 dependencies = [
     "requests",
+		"rich",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://github.com/offenedatenberatung/validate-portal-metadata#readme"
 Issues = "https://github.com/offenedatenberatung/validate-portal-metadata/issues"
 Source = "https://github.com/offenedatenberatung/validate-portal-metadata"
```

### Comparing `dcat_ap_de_validator-1.0.2/PKG-INFO` & `dcat_ap_de_validator-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: dcat-ap-de-validator
-Version: 1.0.2
+Version: 1.1.0
 Project-URL: Documentation, https://github.com/offenedatenberatung/validate-portal-metadata#readme
 Project-URL: Issues, https://github.com/offenedatenberatung/validate-portal-metadata/issues
 Project-URL: Source, https://github.com/offenedatenberatung/validate-portal-metadata
 Author-email: Mila Frerichs <mila@offenedatenberatung.de>
 License-File: LICENSE
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Requires-Dist: requests
+Requires-Dist: rich
 Description-Content-Type: text/markdown
 
 # Validierung von Metadaten pro Portal 
 
 Wir können eine Portal URL (DKAN oder CKAN Portale) übergeben und dann bekommen wir eine
 JSON Datei mit der Validierung aller vorhandenen Datensätze.
 
+![console screenshot](screenshot.png)
+
 
 # Installation
 Zur Installation des Packages mit pipx (pip geht auch):
 
 ```bash
 pipx install dcat-ap-de-validator
 ```
```

