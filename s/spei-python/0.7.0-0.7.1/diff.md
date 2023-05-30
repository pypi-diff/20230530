# Comparing `tmp/spei_python-0.7.0.tar.gz` & `tmp/spei_python-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spei_python-0.7.0.tar", max compression
+gzip compressed data, was "spei_python-0.7.1.tar", max compression
```

## Comparing `spei_python-0.7.0.tar` & `spei_python-0.7.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      999 2023-02-15 18:15:34.283809 spei_python-0.7.0/README.md
--rw-r--r--   0        0        0      856 2023-05-30 01:04:48.825748 spei_python-0.7.0/pyproject.toml
--rw-r--r--   0        0        0       49 2022-07-27 23:08:37.464131 spei_python-0.7.0/spei/__init__.py
--rw-r--r--   0        0        0     2733 2023-05-30 00:46:55.019167 spei_python-0.7.0/spei/client.py
--rw-r--r--   0        0        0       66 2023-02-28 22:07:27.969521 spei_python-0.7.0/spei/resources/__init__.py
--rw-r--r--   0        0        0     4559 2023-05-30 00:59:08.634556 spei_python-0.7.0/spei/resources/ordenes.py
--rw-r--r--   0        0        0     1791 2023-05-30 00:27:21.381550 spei_python-0.7.0/spei/types.py
--rw-r--r--   0        0        0     2272 2023-05-30 01:00:59.645173 spei_python-0.7.0/spei/utils.py
--rw-r--r--   0        0        0     1710 1970-01-01 00:00:00.000000 spei_python-0.7.0/setup.py
--rw-r--r--   0        0        0     1643 1970-01-01 00:00:00.000000 spei_python-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      999 2023-02-15 18:15:34.283809 spei_python-0.7.1/README.md
+-rw-r--r--   0        0        0      856 2023-05-30 01:27:38.547447 spei_python-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0       49 2022-07-27 23:08:37.464131 spei_python-0.7.1/spei/__init__.py
+-rw-r--r--   0        0        0     2733 2023-05-30 00:46:55.019167 spei_python-0.7.1/spei/client.py
+-rw-r--r--   0        0        0       66 2023-02-28 22:07:27.969521 spei_python-0.7.1/spei/resources/__init__.py
+-rw-r--r--   0        0        0     4559 2023-05-30 00:59:08.634556 spei_python-0.7.1/spei/resources/ordenes.py
+-rw-r--r--   0        0        0     1791 2023-05-30 01:26:04.772295 spei_python-0.7.1/spei/types.py
+-rw-r--r--   0        0        0     2272 2023-05-30 01:00:59.645173 spei_python-0.7.1/spei/utils.py
+-rw-r--r--   0        0        0     1710 1970-01-01 00:00:00.000000 spei_python-0.7.1/setup.py
+-rw-r--r--   0        0        0     1643 1970-01-01 00:00:00.000000 spei_python-0.7.1/PKG-INFO
```

### Comparing `spei_python-0.7.0/README.md` & `spei_python-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `spei_python-0.7.0/pyproject.toml` & `spei_python-0.7.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spei-python"
-version = "0.7.0"
+version = "0.7.1"
 description = ""
 authors = ["gonz <gonzasestopal@gmail.com>"]
 readme = "README.md"
 packages = [{include = "spei"}]
 
 [tool.poetry.dependencies]
 python = "^3.7"
@@ -27,13 +27,13 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.7.0"
+version = "0.7.1"
 tag_format = "v$version"
 bump_message = "bump: Semantic Release Bot: Release Version: $new_version 🤖🚀 [skip ci]"
 version_files = [
     "pyproject.toml:version",
 ]
```

### Comparing `spei_python-0.7.0/spei/client.py` & `spei_python-0.7.1/spei/client.py`

 * *Files identical despite different names*

### Comparing `spei_python-0.7.0/spei/resources/ordenes.py` & `spei_python-0.7.1/spei/resources/ordenes.py`

 * *Files identical despite different names*

### Comparing `spei_python-0.7.0/spei/types.py` & `spei_python-0.7.1/spei/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,10 +66,10 @@
     htvf = '9'
     dtp = '10'
     ifai = '13'
     swift = '17'
     nomina = '18'
 
 
-class CodigoError(str, Enum):
+class CodigoError(int, Enum):
     exitoso = 0
     categoria_incorrecta = -1
```

### Comparing `spei_python-0.7.0/spei/utils.py` & `spei_python-0.7.1/spei/utils.py`

 * *Files identical despite different names*

### Comparing `spei_python-0.7.0/setup.py` & `spei_python-0.7.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['cryptography==3.4.7',
  'lxml>=4.9.1,<5.0.0',
  'pydantic>=1.8.2,<2.0.0',
  'requests>=2.27.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'spei-python',
-    'version': '0.7.0',
+    'version': '0.7.1',
     'description': '',
     'long_description': '[![wemake-python-styleguide](https://img.shields.io/badge/style-wemake-000000.svg)](https://github.com/wemake-services/wemake-python-styleguide)\n\nspei-python\n===========\n\nA library for accessing the SPEI API for python.\n\n\n## Installation\nUse the package manager [poetry](https://pypi.org/project/poetry/) to install.\n\n    poetry install spei-python\n\n## Test\nTested with [mamba](https://mamba-framework.readthedocs.io/en/latest/), install poetry dev packages and then run tests.\n\n    poetry run make test\n\n## Contributing\nPull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.\n\nPlease make sure to update tests as appropriate.\n\n## License\n[MIT](https://choosealicense.com/licenses/mit/)\n\n## Checksum Generator\nThis repo includes a utility to generate [firma digital aplicada](https://www.notion.so/fondeadoraroot/Algoritmo-de-Firma-e-Karpay-SPEI-02e6c25b7c5943bea054ae37c9605bdc)\n\n```sh\npython bin/generate_checksum.py bin/message.json\n```\n',
     'author': 'gonz',
     'author_email': 'gonzasestopal@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `spei_python-0.7.0/PKG-INFO` & `spei_python-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spei-python
-Version: 0.7.0
+Version: 0.7.1
 Summary: 
 Author: gonz
 Author-email: gonzasestopal@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

