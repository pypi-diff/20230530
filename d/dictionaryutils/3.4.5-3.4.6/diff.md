# Comparing `tmp/dictionaryutils-3.4.5.tar.gz` & `tmp/dictionaryutils-3.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dictionaryutils-3.4.5.tar", max compression
+gzip compressed data, was "dictionaryutils-3.4.6.tar", max compression
```

## Comparing `dictionaryutils-3.4.5.tar` & `dictionaryutils-3.4.6.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-01-30 20:27:29.813398 dictionaryutils-3.4.5/LICENSE
--rw-r--r--   0        0        0     3234 2023-01-30 20:27:29.813398 dictionaryutils-3.4.5/README.md
--rw-r--r--   0        0        0     9496 2023-01-30 20:27:29.813398 dictionaryutils-3.4.5/dictionaryutils/__init__.py
--rw-r--r--   0        0        0     1790 2023-01-30 20:27:29.813398 dictionaryutils-3.4.5/dictionaryutils/dictionary.py
--rw-r--r--   0        0        0       92 2023-01-30 20:27:29.813398 dictionaryutils-3.4.5/dictionaryutils/errors.py
--rw-r--r--   0        0        0     1203 2023-01-30 20:27:29.813398 dictionaryutils-3.4.5/dictionaryutils/json_load.py
--rw-r--r--   0        0        0     7632 2023-01-30 20:27:29.813398 dictionaryutils-3.4.5/dictionaryutils/schema_test.py
--rw-r--r--   0        0        0     1408 2023-01-30 20:27:29.813398 dictionaryutils-3.4.5/dictionaryutils/schemas/data_release.yaml
--rw-r--r--   0        0        0     2869 2023-01-30 20:27:29.813398 dictionaryutils-3.4.5/dictionaryutils/schemas/metaschema.yaml
--rw-r--r--   0        0        0      409 2023-01-30 20:27:29.813398 dictionaryutils-3.4.5/dictionaryutils/schemas/root.yaml
--rw-r--r--   0        0        0       89 2023-01-30 20:27:29.813398 dictionaryutils-3.4.5/dictionaryutils/version_data.py
--rw-r--r--   0        0        0      698 2023-01-30 20:27:29.813398 dictionaryutils-3.4.5/pyproject.toml
--rw-r--r--   0        0        0     4103 1970-01-01 00:00:00.000000 dictionaryutils-3.4.5/setup.py
--rw-r--r--   0        0        0     4084 1970-01-01 00:00:00.000000 dictionaryutils-3.4.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-30 19:05:53.231377 dictionaryutils-3.4.6/LICENSE
+-rw-r--r--   0        0        0     3234 2023-05-30 19:05:53.231377 dictionaryutils-3.4.6/README.md
+-rw-r--r--   0        0        0     9580 2023-05-30 19:05:53.231377 dictionaryutils-3.4.6/dictionaryutils/__init__.py
+-rw-r--r--   0        0        0     1790 2023-05-30 19:05:53.231377 dictionaryutils-3.4.6/dictionaryutils/dictionary.py
+-rw-r--r--   0        0        0       92 2023-05-30 19:05:53.231377 dictionaryutils-3.4.6/dictionaryutils/errors.py
+-rw-r--r--   0        0        0     1203 2023-05-30 19:05:53.231377 dictionaryutils-3.4.6/dictionaryutils/json_load.py
+-rw-r--r--   0        0        0     7632 2023-05-30 19:05:53.231377 dictionaryutils-3.4.6/dictionaryutils/schema_test.py
+-rw-r--r--   0        0        0     1408 2023-05-30 19:05:53.231377 dictionaryutils-3.4.6/dictionaryutils/schemas/data_release.yaml
+-rw-r--r--   0        0        0     2869 2023-05-30 19:05:53.231377 dictionaryutils-3.4.6/dictionaryutils/schemas/metaschema.yaml
+-rw-r--r--   0        0        0      409 2023-05-30 19:05:53.231377 dictionaryutils-3.4.6/dictionaryutils/schemas/root.yaml
+-rw-r--r--   0        0        0       89 2023-05-30 19:05:53.231377 dictionaryutils-3.4.6/dictionaryutils/version_data.py
+-rw-r--r--   0        0        0      698 2023-05-30 19:05:53.231377 dictionaryutils-3.4.6/pyproject.toml
+-rw-r--r--   0        0        0     4084 1970-01-01 00:00:00.000000 dictionaryutils-3.4.6/PKG-INFO
```

### Comparing `dictionaryutils-3.4.5/LICENSE` & `dictionaryutils-3.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dictionaryutils-3.4.5/README.md` & `dictionaryutils-3.4.6/README.md`

 * *Files identical despite different names*

### Comparing `dictionaryutils-3.4.5/dictionaryutils/__init__.py` & `dictionaryutils-3.4.6/dictionaryutils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -274,11 +274,11 @@
                         prop["type"] = [prop["type"]]
                     prop["type"].append("null")
                 elif "enum" in prop and None not in prop["enum"]:
                     # add null type to optional enums
                     if not isinstance(prop["enum"], list):
                         prop["enum"] = [prop["enum"]]
                     prop["enum"].append(None)
-                elif "anyOf" in prop:
+                elif "anyOf" in prop and {"type": "null"} not in prop["anyOf"]:
                     prop["anyOf"].append({"type": "null"})
-                elif "oneOf" in prop:
+                elif "oneOf" in prop and {"type": "null"} not in prop["oneOf"]:
                     prop["oneOf"].append({"type": "null"})
```

### Comparing `dictionaryutils-3.4.5/dictionaryutils/dictionary.py` & `dictionaryutils-3.4.6/dictionaryutils/dictionary.py`

 * *Files identical despite different names*

### Comparing `dictionaryutils-3.4.5/dictionaryutils/json_load.py` & `dictionaryutils-3.4.6/dictionaryutils/json_load.py`

 * *Files identical despite different names*

### Comparing `dictionaryutils-3.4.5/dictionaryutils/schema_test.py` & `dictionaryutils-3.4.6/dictionaryutils/schema_test.py`

 * *Files identical despite different names*

### Comparing `dictionaryutils-3.4.5/dictionaryutils/schemas/data_release.yaml` & `dictionaryutils-3.4.6/dictionaryutils/schemas/data_release.yaml`

 * *Files identical despite different names*

### Comparing `dictionaryutils-3.4.5/dictionaryutils/schemas/metaschema.yaml` & `dictionaryutils-3.4.6/dictionaryutils/schemas/metaschema.yaml`

 * *Files identical despite different names*

### Comparing `dictionaryutils-3.4.5/pyproject.toml` & `dictionaryutils-3.4.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dictionaryutils"
-version = "3.4.5"
+version = "3.4.6"
 description = "Python wrapper and metaschema for datadictionary."
 authors = ["CTDS UChicago <cdis@uchicago.edu>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/uc-cdis/dictionaryutils"
 
 [tool.poetry.dependencies]
```

### Comparing `dictionaryutils-3.4.5/setup.py` & `dictionaryutils-3.4.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,88 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: dictionaryutils
+Version: 3.4.6
+Summary: Python wrapper and metaschema for datadictionary.
+Home-page: https://github.com/uc-cdis/dictionaryutils
+License: Apache-2.0
+Author: CTDS UChicago
+Author-email: cdis@uchicago.edu
+Requires-Python: >=3.6,<3.10
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: PyYAML (>=5.1,<6.0)
+Requires-Dist: cdislogging (>=1.0.0,<2.0.0)
+Requires-Dist: jsonschema (>=2.5,<4)
+Requires-Dist: requests (>=2.18,<3.0)
+Project-URL: Repository, https://github.com/uc-cdis/dictionaryutils
+Description-Content-Type: text/markdown
+
+# dictionaryutils
+
+python wrapper and metaschema for datadictionary.
+It can be used to:
+- load a local dictionary to a python object.
+- dump schemas to a file that can be uploaded to s3 as an artifact.
+- load schema file from an url to a python object that can be used by services
+
+## Test for dictionary validity with Docker
+Say you have a dictionary you are building locally and you want to see if it will pass the tests.
+
+You can add a simple alias to your `.bash_profile` to enable a quick test command:
+```
+testdict() { docker run --rm -v $(pwd):/dictionary quay.io/cdis/dictionaryutils:master; }
+```
+
+Then from the directory containing the `gdcdictionary` directory run `testdict`.
+
+
+## Generate simulated data with Docker
+If you wish to generate fake simulated data you can also do that with dictionaryutils and the data-simulator.
+
+```
+simdata() { docker run --rm -v $(pwd):/dictionary -v $(pwd)/simdata:/simdata quay.io/cdis/dictionaryutils:master /bin/sh -c "cd /dictionary && python setup.py install --force; python /src/datasimulator/bin/data-simulator simulate --path /simdata/ $*; export SUCCESS=$?; rm -rf build dictionaryutils dist gdcdictionary.egg-info; chmod -R a+rwX /simdata; exit $SUCCESS"; }
+simdataurl() { docker run --rm -v $(pwd):/dictionary -v $(pwd)/simdata:/simdata quay.io/cdis/dictionaryutils:master /bin/sh -c "python /src/datasimulator/bin/data-simulator simulate --path /simdata/ $*; chmod -R a+rwX /simdata"; }
+
+```
+
+Then from the directory containing the `gdcdictionary` directory run `simdata` and a folder will be created called `simdata` with the results of the simulator run. You can also pass in additional arguments to the data-simulator script such as `simdata --max_samples 10`.
+
+The `--max_samples` argument will define a default number of nodes to simulate, but you can override it using the `--node_num_instances_file` argument. For example, if you create the following `instances.json`:
+
+```
+{
+        "case": 100,
+        "demographic": 100
+}
 
-packages = \
-['dictionaryutils']
+```
+Then run the following:
+```
+docker run --rm -v $(pwd):/dictionary -v $(pwd)/simdata:/simdata quay.io/cdis/dictionaryutils:master /bin/sh -c "cd /dictionary && python setup.py install --force; python /src/datasimulator/bin/data-simulator simulate --path /simdata/ --program workshop --project project1 --max_samples 10 --node_num_instances_file instances.json; export SUCCESS=$?; rm -rf build dictionaryutils dist gdcdictionary.egg-info; chmod -R a+rwX /simdata; exit $SUCCESS";
+```
+Then you'll get 100 each of `case` and `demographic` nodes and 10 each of everything else. Note that the above example also defines `program` and `project` names.
 
-package_data = \
-{'': ['*'], 'dictionaryutils': ['schemas/*']}
+You can also run the simulator for an arbitrary json url by using `simdataurl --url https://datacommons.example.com/schema.json`.
 
-install_requires = \
-['PyYAML>=5.1,<6.0',
- 'cdislogging>=1.0.0,<2.0.0',
- 'jsonschema>=2.5,<4',
- 'requests>=2.18,<3.0']
-
-setup_kwargs = {
-    'name': 'dictionaryutils',
-    'version': '3.4.5',
-    'description': 'Python wrapper and metaschema for datadictionary.',
-    'long_description': '# dictionaryutils\n\npython wrapper and metaschema for datadictionary.\nIt can be used to:\n- load a local dictionary to a python object.\n- dump schemas to a file that can be uploaded to s3 as an artifact.\n- load schema file from an url to a python object that can be used by services\n\n## Test for dictionary validity with Docker\nSay you have a dictionary you are building locally and you want to see if it will pass the tests.\n\nYou can add a simple alias to your `.bash_profile` to enable a quick test command:\n```\ntestdict() { docker run --rm -v $(pwd):/dictionary quay.io/cdis/dictionaryutils:master; }\n```\n\nThen from the directory containing the `gdcdictionary` directory run `testdict`.\n\n\n## Generate simulated data with Docker\nIf you wish to generate fake simulated data you can also do that with dictionaryutils and the data-simulator.\n\n```\nsimdata() { docker run --rm -v $(pwd):/dictionary -v $(pwd)/simdata:/simdata quay.io/cdis/dictionaryutils:master /bin/sh -c "cd /dictionary && python setup.py install --force; python /src/datasimulator/bin/data-simulator simulate --path /simdata/ $*; export SUCCESS=$?; rm -rf build dictionaryutils dist gdcdictionary.egg-info; chmod -R a+rwX /simdata; exit $SUCCESS"; }\nsimdataurl() { docker run --rm -v $(pwd):/dictionary -v $(pwd)/simdata:/simdata quay.io/cdis/dictionaryutils:master /bin/sh -c "python /src/datasimulator/bin/data-simulator simulate --path /simdata/ $*; chmod -R a+rwX /simdata"; }\n\n```\n\nThen from the directory containing the `gdcdictionary` directory run `simdata` and a folder will be created called `simdata` with the results of the simulator run. You can also pass in additional arguments to the data-simulator script such as `simdata --max_samples 10`.\n\nThe `--max_samples` argument will define a default number of nodes to simulate, but you can override it using the `--node_num_instances_file` argument. For example, if you create the following `instances.json`:\n\n```\n{\n        "case": 100,\n        "demographic": 100\n}\n\n```\nThen run the following:\n```\ndocker run --rm -v $(pwd):/dictionary -v $(pwd)/simdata:/simdata quay.io/cdis/dictionaryutils:master /bin/sh -c "cd /dictionary && python setup.py install --force; python /src/datasimulator/bin/data-simulator simulate --path /simdata/ --program workshop --project project1 --max_samples 10 --node_num_instances_file instances.json; export SUCCESS=$?; rm -rf build dictionaryutils dist gdcdictionary.egg-info; chmod -R a+rwX /simdata; exit $SUCCESS";\n```\nThen you\'ll get 100 each of `case` and `demographic` nodes and 10 each of everything else. Note that the above example also defines `program` and `project` names.\n\nYou can also run the simulator for an arbitrary json url by using `simdataurl --url https://datacommons.example.com/schema.json`.\n\n\n## Use dictionaryutils to load a dictionary\n```\nfrom dictionaryutils import DataDictionary\n\ndict_fetch_from_remote = DataDictionary(url=URL_FOR_THE_JSON)\n\ndict_loaded_locally = DataDictionary(root_dir=PATH_TO_SCHEMA_DIR)\n```\n\n## Use dictionaryutils to dump a dictionary\n```\nimport json\nfrom dictionaryutils import dump_schemas_from_dir\n\nwith open(\'dump.json\', \'w\') as f:\n    json.dump(dump_schemas_from_dir(\'../datadictionary/gdcdictionary/schemas/\'), f)\n```\n',
-    'author': 'CTDS UChicago',
-    'author_email': 'cdis@uchicago.edu',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/uc-cdis/dictionaryutils',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6,<3.10',
-}
 
+## Use dictionaryutils to load a dictionary
+```
+from dictionaryutils import DataDictionary
+
+dict_fetch_from_remote = DataDictionary(url=URL_FOR_THE_JSON)
+
+dict_loaded_locally = DataDictionary(root_dir=PATH_TO_SCHEMA_DIR)
+```
+
+## Use dictionaryutils to dump a dictionary
+```
+import json
+from dictionaryutils import dump_schemas_from_dir
+
+with open('dump.json', 'w') as f:
+    json.dump(dump_schemas_from_dir('../datadictionary/gdcdictionary/schemas/'), f)
+```
 
-setup(**setup_kwargs)
```

