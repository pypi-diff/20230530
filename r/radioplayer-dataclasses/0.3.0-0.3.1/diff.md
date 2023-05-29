# Comparing `tmp/radioplayer_dataclasses-0.3.0.tar.gz` & `tmp/radioplayer_dataclasses-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radioplayer_dataclasses-0.3.0.tar", max compression
+gzip compressed data, was "radioplayer_dataclasses-0.3.1.tar", max compression
```

## Comparing `radioplayer_dataclasses-0.3.0.tar` & `radioplayer_dataclasses-0.3.1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0    34520 2023-02-18 14:35:42.807119 radioplayer_dataclasses-0.3.0/LICENSE
--rw-r--r--   0        0        0     3627 2023-02-18 14:35:42.807119 radioplayer_dataclasses-0.3.0/README.md
--rw-r--r--   0        0        0     2027 2023-02-18 14:36:36.255094 radioplayer_dataclasses-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2351 2023-02-18 14:35:42.811119 radioplayer_dataclasses-0.3.0/radioplayer/dataclasses/__init__.py
--rw-r--r--   0        0        0    56147 2023-02-18 14:35:42.811119 radioplayer_dataclasses-0.3.0/radioplayer/dataclasses/dataclasses.py
--rw-r--r--   0        0        0        0 2023-02-18 14:35:42.811119 radioplayer_dataclasses-0.3.0/radioplayer/dataclasses/py.typed
--rw-r--r--   0        0        0     4463 1970-01-01 00:00:00.000000 radioplayer_dataclasses-0.3.0/setup.py
--rw-r--r--   0        0        0     4598 1970-01-01 00:00:00.000000 radioplayer_dataclasses-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    34520 2023-05-29 22:33:58.568844 radioplayer_dataclasses-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3627 2023-05-29 22:33:58.568844 radioplayer_dataclasses-0.3.1/README.md
+-rw-r--r--   0        0        0     2105 2023-05-29 22:34:21.245486 radioplayer_dataclasses-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2351 2023-05-29 22:33:58.568844 radioplayer_dataclasses-0.3.1/radioplayer/dataclasses/__init__.py
+-rw-r--r--   0        0        0    56147 2023-05-29 22:33:58.568844 radioplayer_dataclasses-0.3.1/radioplayer/dataclasses/dataclasses.py
+-rw-r--r--   0        0        0        0 2023-05-29 22:33:58.568844 radioplayer_dataclasses-0.3.1/radioplayer/dataclasses/py.typed
+-rw-r--r--   0        0        0     4497 1970-01-01 00:00:00.000000 radioplayer_dataclasses-0.3.1/PKG-INFO
```

### Comparing `radioplayer_dataclasses-0.3.0/LICENSE` & `radioplayer_dataclasses-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `radioplayer_dataclasses-0.3.0/README.md` & `radioplayer_dataclasses-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `radioplayer_dataclasses-0.3.0/pyproject.toml` & `radioplayer_dataclasses-0.3.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "radioplayer-dataclasses"
-version = "v0.3.0" # 0.0.0 placeholder is replaced on release
+version = "v0.3.1" # 0.0.0 placeholder is replaced on release
 description = "Python dataclasses for radioplayer generated from XSD"
 repository = "https://github.com/radiorabe/python-radioplayer-dataclasses"
 authors = ["RaBe IT-Reaktion <it@rabe.ch>"]
 license = "AGPL-3"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -15,36 +15,36 @@
 readme = "README.md"
 packages = [
     { include = "radioplayer/dataclasses"},
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-xsdata = "^22.12"
+xsdata = ">=22.12,<24.0"
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.12.0"
+black = ">=22.12,<24.0"
 flake8 = "^6.0.0"
 flake8-docstrings = "^1.6.0"
-flake8-isort = "^5.0.3"
+flake8-isort = ">=5.0.3,<7.0.0"
 flake8-string-format = "^0.3.0"
 flake8-tuple = "^0.4.1"
 lxml = "^4.9.2"
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 pytest-pylint = "^0.19.0"
-wheel = "^0.38.4"
+wheel = ">=0.38.4,<0.41.0"
 xmldiff = "^2.4"
-xsdata = {extras = ["cli"], version = "^22.12"}
+xsdata = {extras = ["cli"], version = ">=22.12,<24.0"}
 pytest-random-order = "^1.1.0"
 pytest-mypy = "^0.10.3"
-mkdocstrings = "^0.20.0"
-mkdocs-material = "^9.0.13"
+mkdocstrings = {extras = ["python"], version = ">=0.20,<0.23"}
+mkdocs-material = ">=8,<10"
 mkdocs = "^1.4.2"
-mkdocs-gen-files = "^0.4.0"
+mkdocs-gen-files = ">=0.4,<0.6"
 mkdocs-literate-nav = "^0.6.0"
 mkdocs-section-index = "^0.3.5"
 
 [tool.isort]
 line_length = 120
 profile = "black"
```

### Comparing `radioplayer_dataclasses-0.3.0/radioplayer/dataclasses/__init__.py` & `radioplayer_dataclasses-0.3.1/radioplayer/dataclasses/__init__.py`

 * *Files identical despite different names*

### Comparing `radioplayer_dataclasses-0.3.0/radioplayer/dataclasses/dataclasses.py` & `radioplayer_dataclasses-0.3.1/radioplayer/dataclasses/dataclasses.py`

 * *Files identical despite different names*

### Comparing `radioplayer_dataclasses-0.3.0/setup.py` & `radioplayer_dataclasses-0.3.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,142 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: radioplayer-dataclasses
+Version: 0.3.1
+Summary: Python dataclasses for radioplayer generated from XSD
+Home-page: https://github.com/radiorabe/python-radioplayer-dataclasses
+License: AGPL-3
+Author: RaBe IT-Reaktion
+Author-email: it@rabe.ch
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: xsdata (>=22.12,<24.0)
+Project-URL: Repository, https://github.com/radiorabe/python-radioplayer-dataclasses
+Description-Content-Type: text/markdown
 
-packages = \
-['dataclasses']
+# Python Radioplayer Dataclasses
 
-package_data = \
-{'': ['*']}
+Classes for generating [radioplayer](https://radioplayer.co.uk) compatible data. Generated using [xsdata](https://xsdata.readthedocs.io/).
 
-install_requires = \
-['xsdata>=22.12,<23.0']
-
-setup_kwargs = {
-    'name': 'radioplayer-dataclasses',
-    'version': '0.3.0',
-    'description': 'Python dataclasses for radioplayer generated from XSD',
-    'long_description': '# Python Radioplayer Dataclasses\n\nClasses for generating [radioplayer](https://radioplayer.co.uk) compatible data. Generated using [xsdata](https://xsdata.readthedocs.io/).\n\n## Installation\n\n```bash\npip install radioplayer-dataclasses\n```\n\n## Usage\n\nThe `radioplayer.dataclasses` module may be used to build radioplayer compatible structures.\nSerializing is done using the `xsdata` library.\n\n```python\n>>> from radioplayer.dataclasses import *\n>>> epg = Epg(lang="en")\n>>> epg\nEpg(programme_groups=[], schedule=[], alternate_source=[], lang=\'en\', system=<SystemType.DAB: \'DAB\'>)\n\n>>> from xsdata.formats.dataclass.serializers import XmlSerializer\n>>> from xsdata.formats.dataclass.serializers.config import SerializerConfig\n>>>\n>>> config = SerializerConfig(\n...     pretty_print=True,\n...     xml_declaration=False,\n... )\n>>> serializer = XmlSerializer(config=config)\n>>> xml = serializer.render(epg, ns_map={None: Epg.Meta.namespace})\n>>> print(xml.strip())\n<epg xmlns="http://www.radioplayer.co.uk/schemas/11/epgSchedule" xml:lang="en" system="DAB"/>\n\n```\n\nAdditional examples are available in the `tests/` directory.\n\n## Development\n\n### Getting Started\n\n```bash\n# setup a dev env\npython -mvenv env\n. env/bin/activate\n\n# install a modern poetry version\npython -mpip install \'poetry>=1.2.0\'\n\n# install deps and dev version\npoetry install\n```\n\n### Loading XSD files\n\n```bash\nmkdir schemas\npushd schemas/\ncurl -L -O http://www.w3.org/2001/xml.xsd\ncurl -L -O https://radioplayer.co.uk/schemas/11/epgSchedule_11.xsd\ncurl -L -O https://radioplayer.co.uk/schemas/11/epgDataTypes_11.xsd\ncurl -L -O https://radioplayer.co.uk/schemas/11/rpDataTypes_11.xsd\ncurl -L -O https://radioplayer.co.uk/schemas/11/epgSI_11.xsd\npopd\n```\n\nSome touchups where made to the files to make them validate where necessary.\n\n### Generating dataclasses\n\n```bash\npoetry run xsdata -c .xsdata.xml schemas/\n```\n\n### Running tests\n\n```bash\npoetry run pytest\n```\n\n## Release Management\n\nThe CI/CD setup uses semantic commit messages following the [conventional commits standard](https://www.conventionalcommits.org/en/v1.0.0/).\nThere is a GitHub Action in [.github/workflows/semantic-release.yaml](./.github/workflows/semantic-release.yaml)\nthat uses [go-semantic-commit](https://go-semantic-release.xyz/) to create new\nreleases.\n\nThe commit message should be structured as follows:\n\n```\n<type>[optional scope]: <description>\n\n[optional body]\n\n[optional footer(s)]\n```\n\nThe commit contains the following structural elements, to communicate intent to the consumers of your library:\n\n1. **fix:** a commit of the type `fix` patches gets released with a PATCH version bump\n1. **feat:** a commit of the type `feat` gets released as a MINOR version bump\n1. **BREAKING CHANGE:** a commit that has a footer `BREAKING CHANGE:` gets released as a MAJOR version bump\n1. types other than `fix:` and `feat:` are allowed and don\'t trigger a release\n\nIf a commit does not contain a conventional commit style message you can fix\nit during the squash and merge operation on the PR.\n\nOnce a commit has landed on the `main` branch a release will be created and automatically published to [pypi](https://pypi.org/)\nusing the GitHub Action in [.github/workflows/release.yaml](./.github/workflows/release.yaml) which uses [poetry](https://python-poetry.org/)\nto publish the package to pypi.\n\n## License\n\nThis application is free software: you can redistribute it and/or modify it under\nthe terms of the GNU Affero General Public License as published by the Free\nSoftware Foundation, version 3 of the License.\n\n## Copyright\n\nCopyright (c) 2022 [Radio Bern RaBe](http://www.rabe.ch)\n',
-    'author': 'RaBe IT-Reaktion',
-    'author_email': 'it@rabe.ch',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/radiorabe/python-radioplayer-dataclasses',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
+## Installation
 
+```bash
+pip install radioplayer-dataclasses
+```
+
+## Usage
+
+The `radioplayer.dataclasses` module may be used to build radioplayer compatible structures.
+Serializing is done using the `xsdata` library.
+
+```python
+>>> from radioplayer.dataclasses import *
+>>> epg = Epg(lang="en")
+>>> epg
+Epg(programme_groups=[], schedule=[], alternate_source=[], lang='en', system=<SystemType.DAB: 'DAB'>)
+
+>>> from xsdata.formats.dataclass.serializers import XmlSerializer
+>>> from xsdata.formats.dataclass.serializers.config import SerializerConfig
+>>>
+>>> config = SerializerConfig(
+...     pretty_print=True,
+...     xml_declaration=False,
+... )
+>>> serializer = XmlSerializer(config=config)
+>>> xml = serializer.render(epg, ns_map={None: Epg.Meta.namespace})
+>>> print(xml.strip())
+<epg xmlns="http://www.radioplayer.co.uk/schemas/11/epgSchedule" xml:lang="en" system="DAB"/>
+
+```
+
+Additional examples are available in the `tests/` directory.
+
+## Development
+
+### Getting Started
+
+```bash
+# setup a dev env
+python -mvenv env
+. env/bin/activate
+
+# install a modern poetry version
+python -mpip install 'poetry>=1.2.0'
+
+# install deps and dev version
+poetry install
+```
+
+### Loading XSD files
+
+```bash
+mkdir schemas
+pushd schemas/
+curl -L -O http://www.w3.org/2001/xml.xsd
+curl -L -O https://radioplayer.co.uk/schemas/11/epgSchedule_11.xsd
+curl -L -O https://radioplayer.co.uk/schemas/11/epgDataTypes_11.xsd
+curl -L -O https://radioplayer.co.uk/schemas/11/rpDataTypes_11.xsd
+curl -L -O https://radioplayer.co.uk/schemas/11/epgSI_11.xsd
+popd
+```
+
+Some touchups where made to the files to make them validate where necessary.
+
+### Generating dataclasses
+
+```bash
+poetry run xsdata -c .xsdata.xml schemas/
+```
+
+### Running tests
+
+```bash
+poetry run pytest
+```
+
+## Release Management
+
+The CI/CD setup uses semantic commit messages following the [conventional commits standard](https://www.conventionalcommits.org/en/v1.0.0/).
+There is a GitHub Action in [.github/workflows/semantic-release.yaml](./.github/workflows/semantic-release.yaml)
+that uses [go-semantic-commit](https://go-semantic-release.xyz/) to create new
+releases.
+
+The commit message should be structured as follows:
+
+```
+<type>[optional scope]: <description>
+
+[optional body]
+
+[optional footer(s)]
+```
+
+The commit contains the following structural elements, to communicate intent to the consumers of your library:
+
+1. **fix:** a commit of the type `fix` patches gets released with a PATCH version bump
+1. **feat:** a commit of the type `feat` gets released as a MINOR version bump
+1. **BREAKING CHANGE:** a commit that has a footer `BREAKING CHANGE:` gets released as a MAJOR version bump
+1. types other than `fix:` and `feat:` are allowed and don't trigger a release
+
+If a commit does not contain a conventional commit style message you can fix
+it during the squash and merge operation on the PR.
+
+Once a commit has landed on the `main` branch a release will be created and automatically published to [pypi](https://pypi.org/)
+using the GitHub Action in [.github/workflows/release.yaml](./.github/workflows/release.yaml) which uses [poetry](https://python-poetry.org/)
+to publish the package to pypi.
+
+## License
+
+This application is free software: you can redistribute it and/or modify it under
+the terms of the GNU Affero General Public License as published by the Free
+Software Foundation, version 3 of the License.
+
+## Copyright
+
+Copyright (c) 2022 [Radio Bern RaBe](http://www.rabe.ch)
 
-setup(**setup_kwargs)
```

