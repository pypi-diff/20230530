# Comparing `tmp/jake-3.0.0.tar.gz` & `tmp/jake-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jake-3.0.0.tar", max compression
+gzip compressed data, was "jake-3.0.1.tar", max compression
```

## Comparing `jake-3.0.0.tar` & `jake-3.0.1.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0    11357 2022-12-02 21:33:36.048608 jake-3.0.0/LICENSE
--rw-r--r--   0        0        0    30799 2022-12-02 21:33:36.048608 jake-3.0.0/README.md
--rw-r--r--   0        0        0      589 2022-12-02 21:33:36.048608 jake-3.0.0/jake/__init__.py
--rw-r--r--   0        0        0     4649 2022-12-02 21:33:36.048608 jake-3.0.0/jake/app.py
--rw-r--r--   0        0        0     1857 2022-12-02 21:33:36.048608 jake-3.0.0/jake/command/__init__.py
--rw-r--r--   0        0        0     1762 2022-12-02 21:33:36.048608 jake-3.0.0/jake/command/config.py
--rw-r--r--   0        0        0    12035 2022-12-02 21:33:36.048608 jake-3.0.0/jake/command/iq.py
--rw-r--r--   0        0        0    16853 2022-12-02 21:33:36.048608 jake-3.0.0/jake/command/oss.py
--rw-r--r--   0        0        0     3495 2022-12-02 21:33:36.048608 jake-3.0.0/jake/command/parser_selector.py
--rw-r--r--   0        0        0     5266 2022-12-02 21:33:36.048608 jake-3.0.0/jake/command/sbom.py
--rw-r--r--   0        0        0      153 2022-12-02 21:33:36.048608 jake-3.0.0/jake/py.typed
--rw-r--r--   0        0        0     2013 2022-12-02 21:33:42.656635 jake-3.0.0/pyproject.toml
--rw-r--r--   0        0        0    32603 2022-12-02 21:33:45.672479 jake-3.0.0/setup.py
--rw-r--r--   0        0        0    32520 2022-12-02 21:33:45.674419 jake-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-30 14:55:48.545441 jake-3.0.1/LICENSE
+-rw-r--r--   0        0        0    30799 2023-05-30 14:55:48.545441 jake-3.0.1/README.md
+-rw-r--r--   0        0        0      589 2023-05-30 14:55:48.549441 jake-3.0.1/jake/__init__.py
+-rw-r--r--   0        0        0     4038 2023-05-30 14:55:48.549441 jake-3.0.1/jake/app.py
+-rw-r--r--   0        0        0     1858 2023-05-30 14:55:48.549441 jake-3.0.1/jake/command/__init__.py
+-rw-r--r--   0        0        0     1177 2023-05-30 14:55:48.549441 jake-3.0.1/jake/command/config.py
+-rw-r--r--   0        0        0    11446 2023-05-30 14:55:48.549441 jake-3.0.1/jake/command/iq.py
+-rw-r--r--   0        0        0    16524 2023-05-30 14:55:48.549441 jake-3.0.1/jake/command/oss.py
+-rw-r--r--   0        0        0     4104 2023-05-30 14:55:48.549441 jake-3.0.1/jake/command/parser_selector.py
+-rw-r--r--   0        0        0     4677 2023-05-30 14:55:48.549441 jake-3.0.1/jake/command/sbom.py
+-rw-r--r--   0        0        0      153 2023-05-30 14:55:48.549441 jake-3.0.1/jake/py.typed
+-rw-r--r--   0        0        0     2556 2023-05-30 14:55:52.721471 jake-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0    32518 1970-01-01 00:00:00.000000 jake-3.0.1/PKG-INFO
```

### Comparing `jake-3.0.0/LICENSE` & `jake-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jake-3.0.0/README.md` & `jake-3.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -127,16 +127,16 @@
 conda list --explicit --md5 | jake sbom -t CONDA
 conda list --json | jake sbom -t CONDA_JSON
 cat /path/to/Pipfile.lock | python -m jake.app sbom -t PIPENV
 ```
 
 Check out these examples specifying a manifest:
 ```
-jake sbom -t PIP -i /path/to/requirements.txt
-jake sbom -t PIPENV -i /path/to/Pipfile.lock
+jake sbom -t PIP -f /path/to/requirements.txt
+jake sbom -t PIPENV -f /path/to/Pipfile.lock
 ```
 
 ### Check for vulnerabilities using OSS Index
 
 `jake` will look at the packaged installed in your current Python environment and check these against OSS Index for you.
 Optionally, it can create a CycloneDX software bill-of-materials at the same time in a format that suits you.
 
@@ -292,16 +292,16 @@
 conda list --explicit --md5 | jake ddt -t CONDA
 conda list --json | jake ddt -t CONDA_JSON
 cat /path/to/Pipfile.lock | python -m jake.app ddt -t PIPENV
 ```
 
 Check out these examples specifying a manifest:
 ```
-jake ddt -t PIP -i /path/to/requirements.txt
-jake ddt -t PIPENV -i /path/to/Pipfile.lock
+jake ddt -t PIP -f /path/to/requirements.txt
+jake ddt -t PIPENV -f /path/to/Pipfile.lock
 ```
 
 A pre-commit hook is also available for use
 
 ```Yaml
   - repo: https://github.com/sonatype-nexus-community/jake
     rev: "v1.3.0"
```

### Comparing `jake-3.0.0/jake/__init__.py` & `jake-3.0.1/jake/__init__.py`

 * *Files identical despite different names*

### Comparing `jake-3.0.0/jake/app.py` & `jake-3.0.1/jake/app.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python
 #
 # Copyright 2019-Present Sonatype Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -13,29 +12,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 # encoding: utf-8
 
-#
-# Copyright 2019-Present Sonatype Inc.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
 import argparse
 from argparse import ArgumentParser
 from datetime import datetime
 from typing import Dict
 
 from pyfiglet import figlet_format  # type: ignore
 from rich.console import Console
```

### Comparing `jake-3.0.0/jake/command/__init__.py` & `jake-3.0.1/jake/command/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# encoding: utf-8
-
 #
 # Copyright 2019-Present Sonatype Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
@@ -11,14 +9,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+
+# encoding: utf-8
+
 import sys
 from abc import ABC, abstractmethod
 from argparse import ArgumentParser, Namespace
 from typing import Optional
 
 if sys.version_info >= (3, 8):
     from importlib.metadata import version as meta_version
```

### Comparing `jake-3.0.0/jake/command/config.py` & `jake-3.0.1/jake/command/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,38 +12,23 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 # encoding: utf-8
 
-#
-# Copyright 2019-Present Sonatype Inc.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
 from argparse import ArgumentParser
 
 from . import BaseCommand
 
 
 class ConfigCommand(BaseCommand):
 
     def handle_args(self) -> int:
-        pass
+        return 0
 
     def get_argument_parser_name(self) -> str:
         return 'config'
 
     def get_argument_parser_help(self) -> str:
         return 'configure jake for OSS Index or Nexus Lifecycle access'
```

### Comparing `jake-3.0.0/jake/command/iq.py` & `jake-3.0.1/jake/command/iq.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,29 +12,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 # encoding: utf-8
 
-#
-# Copyright 2019-Present Sonatype Inc.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
 import logging
 from argparse import ArgumentParser
 from typing import Any, Dict, Optional, Union
 from urllib.parse import urlparse
 
 import requests
 from cyclonedx.model.bom import Bom
```

### Comparing `jake-3.0.0/jake/command/oss.py` & `jake-3.0.1/jake/command/oss.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-#
-# Copyright 2019-Present Sonatype Inc.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-
 # encoding: utf-8
 
 #
 # Copyright 2019-Present Sonatype Inc.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
@@ -27,14 +11,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+
 import json
 import os
 from argparse import ArgumentParser
 from decimal import Decimal
 from pathlib import Path
 from typing import cast, Iterable, List, Set
 
@@ -159,22 +144,28 @@
                                     ) if oic_vulnerability.cvss_score else None,
                                     method=VulnerabilityScoreSource.get_from_vector(
                                         vector=oic_vulnerability.cvss_vector
                                     ) if oic_vulnerability.cvss_vector else None,
                                     vector=oic_vulnerability.cvss_vector
                                 )
                             )
+                        cwes = None
+                        if oic_vulnerability.cwe:
+                            try:
+                                cwes = [int(oic_vulnerability.cwe[4:])]
+                            except ValueError:
+                                pass    # ignore cases where conversion to int fails
 
                         vulnerability: Vulnerability = Vulnerability(
                             bom_ref=oic_vulnerability.id,
                             id=oic_vulnerability.id,
                             source=VulnerabilitySource(
                                 name='OSS Index', url=XsUri(oic_vulnerability.reference)
                             ),
-                            cwes=[int(oic_vulnerability.cwe[4:])] if oic_vulnerability.cwe else None,
+                            cwes=cwes,
                             description=oic_vulnerability.title,
                             detail=oic_vulnerability.description,
                             ratings=ratings,
                             references=[
                                 VulnerabilityReference(
                                     id=oic_vulnerability.display_name, source=VulnerabilitySource(
                                         name='OSS Index', url=XsUri(oic_vulnerability.reference)
```

### Comparing `jake-3.0.0/jake/command/parser_selector.py` & `jake-3.0.1/jake/command/parser_selector.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+#
+# Copyright 2019-Present Sonatype Inc.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+
+# encoding: utf-8
+
 import sys
 from argparse import ArgumentParser
 from argparse import FileType
 from typing import Optional
 from typing import TextIO
 
 from cyclonedx.parser import BaseParser
```

### Comparing `jake-3.0.0/jake/command/sbom.py` & `jake-3.0.1/jake/command/sbom.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,29 +12,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 # encoding: utf-8
 
-#
-# Copyright 2019-Present Sonatype Inc.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
 from argparse import ArgumentParser
 
 from cyclonedx.model import ExternalReference
 from cyclonedx.model import ExternalReferenceType
 from cyclonedx.model import Tool
 from cyclonedx.model import XsUri
 from cyclonedx.model.bom import Bom
```

### Comparing `jake-3.0.0/pyproject.toml` & `jake-3.0.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,26 @@
+#
+# Copyright 2019-Present Sonatype Inc.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+
 [tool.poetry]
 name = "jake"
-version = "3.0.0"
+version = "3.0.1"
 description = "An OSS Index integration to check for vulnerabilities in your Python environments"
 authors = ["Sonatype Community <community-group@sonatype.com>"]
 maintainers = ["Sonatype Community <community-group@sonatype.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/sonatype-nexus-community/jake"
 repository = "https://github.com/sonatype-nexus-community/jake"
@@ -20,15 +36,14 @@
     'Intended Audience :: Information Technology',
     'Intended Audience :: Legal Industry',
     'Intended Audience :: System Administrators',
     'Topic :: Security',
     'Topic :: Software Development',
     'Topic :: System :: Software Distribution',
     'License :: OSI Approved :: Apache Software License',
-    'Programming Language :: Python :: 3.6',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Typing :: Typed'
 ]
 keywords = [
@@ -38,21 +53,21 @@
 [tool.poetry.scripts]
 jake = 'jake.app:main'
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/sonatype-nexus-community/jake/issues"
 
 [tool.poetry.dependencies]
-python = "^3.6.2"
+python = "^3.7"
 cyclonedx-bom = "^3.0.0"
-importlib-metadata = { version = ">= 3.4", python = "< 3.8" }
+importlib-metadata = { version = ">= 3.7", python = "< 3.8" }
 ossindex-lib = "^1.0.0"
 polling2 = "^0.5.0"
 pyfiglet = ">= 0.7.6, < 1.0.0"
-requests = "^2.20.0"
+requests = "^2.31.0"
 rich = "^10.10.0"
 
 [tool.poetry.dev-dependencies]
 tox = "^3.24.3"
 coverage = "^6.2"
 flake8 = "^4.0.1"
 mypy = ">= 0.920, < 1.00"
```

### Comparing `jake-3.0.0/setup.py` & `jake-3.0.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,487 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: jake
+Version: 3.0.1
+Summary: An OSS Index integration to check for vulnerabilities in your Python environments
+Home-page: https://github.com/sonatype-nexus-community/jake
+License: Apache-2.0
+Keywords: BOM,SBOM,SCA,OWASP
+Author: Sonatype Community
+Author-email: community-group@sonatype.com
+Maintainer: Sonatype Community
+Maintainer-email: community-group@sonatype.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: Legal Industry
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Security
+Classifier: Topic :: Software Development
+Classifier: Topic :: System :: Software Distribution
+Classifier: Typing :: Typed
+Requires-Dist: cyclonedx-bom (>=3.0.0,<4.0.0)
+Requires-Dist: importlib-metadata (>=3.7) ; python_version < "3.8"
+Requires-Dist: ossindex-lib (>=1.0.0,<2.0.0)
+Requires-Dist: polling2 (>=0.5.0,<0.6.0)
+Requires-Dist: pyfiglet (>=0.7.6,<1.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: rich (>=10.10.0,<11.0.0)
+Project-URL: Bug Tracker, https://github.com/sonatype-nexus-community/jake/issues
+Project-URL: Repository, https://github.com/sonatype-nexus-community/jake
+Description-Content-Type: text/markdown
 
-packages = \
-['jake', 'jake.command']
+<!--
 
-package_data = \
-{'': ['*']}
+    Copyright 2019-Present Sonatype Inc.
 
-install_requires = \
-['cyclonedx-bom>=3.0.0,<4.0.0',
- 'ossindex-lib>=1.0.0,<2.0.0',
- 'polling2>=0.5.0,<0.6.0',
- 'pyfiglet>=0.7.6,<1.0.0',
- 'requests>=2.20.0,<3.0.0',
- 'rich>=10.10.0,<11.0.0']
-
-extras_require = \
-{':python_version < "3.8"': ['importlib-metadata>=3.4']}
-
-entry_points = \
-{'console_scripts': ['jake = jake.app:main']}
-
-setup_kwargs = {
-    'name': 'jake',
-    'version': '3.0.0',
-    'description': 'An OSS Index integration to check for vulnerabilities in your Python environments',
-    'long_description': '<!--\n\n    Copyright 2019-Present Sonatype Inc.\n\n    Licensed under the Apache License, Version 2.0 (the "License");\n    you may not use this file except in compliance with the License.\n    You may obtain a copy of the License at\n\n        http://www.apache.org/licenses/LICENSE-2.0\n\n    Unless required by applicable law or agreed to in writing, software\n    distributed under the License is distributed on an "AS IS" BASIS,\n    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.\n    See the License for the specific language governing permissions and\n    limitations under the License.\n\n-->\n\n<p align="center">\n    <img src="https://raw.githubusercontent.com/sonatype-nexus-community/jake/main/docs/images/jake.png" width="350" alt="jake icon"/>\n</p>\n\n# Jake\n\n[![CircleCI](https://circleci.com/gh/sonatype-nexus-community/jake/tree/main.svg?style=svg)](https://circleci.com/gh/sonatype-nexus-community/jake/tree/main)\n![Python Version Support](https://img.shields.io/badge/python-3.6+-blue)\n[![PyPI Version](https://img.shields.io/pypi/v/jake?label=PyPI&logo=pypi)](https://pypi.org/project/jake)\n[![GitHub license](https://img.shields.io/github/license/sonatype-nexus-community/jake)](https://github.com/sonatype-nexus-community/jake/blob/main/LICENSE)\n[![GitHub issues](https://img.shields.io/github/issues/sonatype-nexus-community/jake)](https://github.com/sonatype-nexus-community/jake/issues)\n[![GitHub forks](https://img.shields.io/github/forks/sonatype-nexus-community/jake)](https://github.com/sonatype-nexus-community/jake/network)\n[![GitHub stars](https://img.shields.io/github/stars/sonatype-nexus-community/jake)](https://github.com/sonatype-nexus-community/jake/stargazers)\n\n----\n\n`jake` is a tool to check for your Python environments and applications that can:\n- produce CycloneDX software bill-of-materials\n- report on known vulnerabilities\n\n`jake` is powered by [Sonatype OSS Index](https://ossindex.sonatype.org) and can also be used with \n[Sonatype\'s Nexus IQ Server](https://www.sonatype.com/product-nexus-lifecycle).\n\n## Installation\n\nInstall from pypi.org as you would any other Python module:\n\n```\npip install jake\n```\n\nor \n\n```\npoetry add jake\n```\n\n_Other Python package managers are available._\n\n## Usage\n\n### Getting Started\n\n`jake` can guide you...\n\n```\n> jake --help\nusage: jake [-h] [-v] [-w] [-X]  ...\n\nPut your Python dependencies in a chokehold\n\noptional arguments:\n  -h, --help       show this help message and exit\n  -v, --version    show which version of jake you are running\n  -w, --warn-only  prevents exit with non-zero code when issues have been\n                   detected\n  -X               enable debug output\n\nJake sub-commands:\n  \n    iq             perform a scan backed by Nexus Lifecycle\n    ddt            perform a scan backed by OSS Index\n    sbom           generate a CycloneDX software-bill-of-materials (no\n                   vulnerabilities)\n```\n\n`jake` will exit with code `0` under normal operation and `1` if vulnerabilities are found (OssIndex) or Policy \nViolations are detected (Nexus IQ), unless you pass the `-w` flag in which case `jake` will always exit with code `0`....\n\n### Generating an SBOM\n\n`jake` can take data from various inputs (or just look at your current Python environment) and produce a CycloneDX for \nyou.\n\n```\n> jake sbom --help\n\nusage: jake sbom [-h] [-f FILE_PATH] [-t TYPE] [-o PATH/TO/FILE]\n                   [--output-format {json,xml}]\n                   [--schema-version {1.0,1.1,1.2,1.3}]\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -f FILE_PATH, --input FILE_PATH\n                        Where to get input data from. If a path to a file is\n                        not specified directly here,then we will attempt to\n                        read data from STDIN. If there is no data on STDIN, we\n                        will then fall back to looking for standard files in\n                        the current directory that relate to the type of input\n                        indicated by the -t flag.\n  -t TYPE, --type TYPE, -it TYPE, --input-type TYPE\n                        how jake should find the packages from which to\n                        generate your SBOM.ENV = Read from the current Python\n                        Environment; CONDA = Read output from `conda list\n                        --explicit`; CONDA_JSON = Read output from `conda list\n                        --json`; PIP = read from a requirements.txt; PIPENV =\n                        read from Pipfile.lock; POETRY = read from a\n                        poetry.lock. (Default = ENV)\n  -o PATH/TO/FILE, --output-file PATH/TO/FILE\n                        Specify a file to output the SBOM to\n  --output-format {json,xml}\n                        SBOM output format (default = xml)\n  --schema-version {1.0,1.1,1.2,1.3}\n                        CycloneDX schema version to use (default = 1.3)\n```\n\nCheck out these examples using STDIN:\n```\nconda list --explicit --md5 | jake sbom -t CONDA\nconda list --json | jake sbom -t CONDA_JSON\ncat /path/to/Pipfile.lock | python -m jake.app sbom -t PIPENV\n```\n\nCheck out these examples specifying a manifest:\n```\njake sbom -t PIP -i /path/to/requirements.txt\njake sbom -t PIPENV -i /path/to/Pipfile.lock\n```\n\n### Check for vulnerabilities using OSS Index\n\n`jake` will look at the packaged installed in your current Python environment and check these against OSS Index for you.\nOptionally, it can create a CycloneDX software bill-of-materials at the same time in a format that suits you.\n\n```\n> jake ddt --help\n\nusage: jake ddt [-h] [-f FILE_PATH] [-t TYPE] [--clear-cache] [-o PATH/TO/FILE] \n                   [--output-format {xml,json}]\n                   [--schema-version {1.2,1.1,1.0,1.3}]\n                   [--whitelist OSS_WHITELIST_JSON_FILE]\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -f FILE_PATH, --input-file FILE_PATH\n                        Where to get input data from. If a path to a file is\n                        not specified directly here,then we will attempt to\n                        read data from STDIN. If there is no data on STDIN, we\n                        will then fall back to looking for standard files in\n                        the current directory that relate to the type of input\n                        indicated by the -t flag.\n  -t TYPE, --type TYPE, -it TYPE, --input-type TYPE\n                        how jake should find the packages from which to\n                        generate your SBOM.ENV = Read from the current Python\n                        Environment; CONDA = Read output from `conda list\n                        --explicit`; CONDA_JSON = Read output from `conda list\n                        --json`; PIP = read from a requirements.txt; PIPENV =\n                        read from Pipfile.lock; POETRY = read from a\n                        poetry.lock. (Default = ENV)\n  --clear-cache         Clears any local cached OSS Index data prior to execution\n  -o PATH/TO/FILE, --output-file PATH/TO/FILE\n                        Specify a file to output the SBOM to. If not specified the report will be output to the console. STDOUT is not supported.\n  --output-format {xml,json}\n                        SBOM output format (default = xml)\n  --schema-version {1.2,1.1,1.0,1.3}\n                        CycloneDX schema version to use (default = 1.3)\n  --whitelist OSS_WHITELIST_JSON_FILE\n                        Set path to whitelist json file\n```\n\nSo you can quickly get a report by running:\n\n```\n> jake ddt\n\n                   ___           ___           ___     \n       ___        /  /\\         /  /\\         /  /\\    \n      /__/\\      /  /::\\       /  /:/        /  /::\\   \n      \\__\\:\\    /  /:/\\:\\     /  /:/        /  /:/\\:\\  \n  ___ /  /::\\  /  /::\\ \\:\\   /  /::\\____   /  /::\\ \\:\\ \n /__/\\  /:/\\/ /__/:/\\:\\_\\:\\ /__/:/\\:::::\\ /__/:/\\:\\ \\:\\\n \\  \\:\\/:/~~  \\__\\/  \\:\\/:/ \\__\\/~|:|~~~~ \\  \\:\\ \\:\\_\\/\n  \\  \\::/          \\__\\::/     |  |:|      \\  \\:\\ \\:\\  \n   \\__\\/           /  /:/      |  |:|       \\  \\:\\_\\/  \n                  /__/:/       |__|:|        \\  \\:\\    \n                  \\__\\/         \\__\\|         \\__\\/    \n\n                                                  \n            /)                     /)             \n        _/_(/    _     _  __   _  (/_   _         \n o   o  (__/ )__(/_   /_)_/ (_(_(_/(___(/_ o   o  \n                                                  \n                                                  \n\nJake Version: 1.1.0\nPut your Python dependencies in a chokehold.\n\n🐍 Collected 42 packages from your environment (0:00:00.10)\n🐍 Successfully queried OSS Index for package and vulnerability info (0:00:00.59)\n🐍 Sane number of results from OSS Index\n\n\n╔Summary═══════════════╦════╗\n║ Audited Dependencies ║ 42 ║\n╠══════════════════════╬════╣\n║ Vulnerablities Found ║ 0  ║\n╚══════════════════════╩════╝\n```\n\n...and this is what `jake` will output if any bad things are found:\n```\n                   ___           ___           ___     \n       ___        /  /\\         /  /\\         /  /\\    \n      /__/\\      /  /::\\       /  /:/        /  /::\\   \n      \\__\\:\\    /  /:/\\:\\     /  /:/        /  /:/\\:\\  \n  ___ /  /::\\  /  /::\\ \\:\\   /  /::\\____   /  /::\\ \\:\\ \n /__/\\  /:/\\/ /__/:/\\:\\_\\:\\ /__/:/\\:::::\\ /__/:/\\:\\ \\:\\\n \\  \\:\\/:/~~  \\__\\/  \\:\\/:/ \\__\\/~|:|~~~~ \\  \\:\\ \\:\\_\\/\n  \\  \\::/          \\__\\::/     |  |:|      \\  \\:\\ \\:\\  \n   \\__\\/           /  /:/      |  |:|       \\  \\:\\_\\/  \n                  /__/:/       |__|:|        \\  \\:\\    \n                  \\__\\/         \\__\\|         \\__\\/    \n\n                                                  \n            /)                     /)             \n        _/_(/    _     _  __   _  (/_   _         \n o   o  (__/ )__(/_   /_)_/ (_(_(_/(___(/_ o   o  \n                                                  \n                                                  \n\nJake Version: 1.1.5\nPut your Python dependencies in a chokehold\n\n🐍 Collected 69 packages from your environment                       ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 100% -:--:--\n🐍 Successfully queried OSS Index for package and vulnerability info ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 100% -:--:--\n🐍 Sane number of results from OSS Index                             ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 100% -:--:--\n\n[59/69] - pkg:pypi/cryptography@2.2 [VULNERABLE]\nVulnerability Details for pkg:pypi/cryptography@2.2                                                                                                                                                                                                                                                                     \n├── ⚠  ID: 333aca51-7375-4a9d-be64-16d316ab9274                                                                                                                                                                                                                                                                         \n│   └── ╭─ CVE-2020-36242 ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮\n│       │                                                                                                                                                                                                                                                                                                              │\n│       │ In the cryptography package before 3.3.2 for Python, certain sequences of update calls to symmetrically encrypt multi-GB values could result in an integer overflow and buffer overflow, as demonstrated by the Fernet class.                                                                                │\n│       │                                                                                                                                                                                                                                                                                                              │\n│       │ Details:                                                                                                                                                                                                                                                                                                     │\n│       │   - CVSS Score: 9.1 - Critical                                                                                                                                                                                                                                                                               │\n│       │   - CVSS Vector: CVSS:3.0/AV:N/AC:L/PR:N/UI:N/S:U/C:H/I:N/A:H                                                                                                                                                                                                                                                │\n│       │   - CWE: Unknown                                                                                                                                                                                                                                                                                             │\n│       │                                                                                                                                                                                                                                                                                                              │\n│       │ References:                                                                                                                                                                                                                                                                                                  │\n│       │   - https://ossindex.sonatype.org/vulnerability/333aca51-7375-4a9d-be64-16d316ab9274?component-type=pypi&component-name=cryptography&utm_source=python-oss-index-lib%400.2.1&utm_medium=integration                                                                                                          │\n│       │   - https://nvd.nist.gov/vuln/detail/CVE-2020-36242                                                                                                                                                                                                                                                          │\n│       │                                                                                                                                                                                                                                                                                                              │\n│       ╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯\n└── ⚠  ID: f19ff95c-cec5-4263-8d3b-e3e64698881e                                                                                                                                                                                                                                                                         \n    └── ╭─ CVE-2018-10903 ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮\n        │                                                                                                                                                                                                                                                                                                              │\n        │ A flaw was found in python-cryptography versions between >=1.9.0 and <2.3. The finalize_with_tag API did not enforce a minimum tag length. If a user did not validate the input length prior to passing it to finalize_with_tag an attacker could craft an invalid payload with a shortened tag (e.g. 1      │\n        │ byte) such that they would have a 1 in 256 chance of passing the MAC check. GCM tag forgeries can cause key leakage.                                                                                                                                                                                         │\n        │                                                                                                                                                                                                                                                                                                              │\n        │ Details:                                                                                                                                                                                                                                                                                                     │\n        │   - CVSS Score: 7.5 - High                                                                                                                                                                                                                                                                                   │\n        │   - CVSS Vector: CVSS:3.0/AV:N/AC:L/PR:N/UI:N/S:U/C:H/I:N/A:N                                                                                                                                                                                                                                                │\n        │   - CWE: Unknown                                                                                                                                                                                                                                                                                             │\n        │                                                                                                                                                                                                                                                                                                              │\n        │ References:                                                                                                                                                                                                                                                                                                  │\n        │   - https://ossindex.sonatype.org/vulnerability/f19ff95c-cec5-4263-8d3b-e3e64698881e?component-type=pypi&component-name=cryptography&utm_source=python-oss-index-lib%400.2.1&utm_medium=integration                                                                                                          │\n        │   - https://bugzilla.redhat.com/show_bug.cgi?id=CVE-2018-10903                                                                                                                                                                                                                                               │\n        │   - https://github.com/pyca/cryptography/pull/4342/commits/688e0f673bfbf43fa898994326c6877f00ab19ef                                                                                                                                                                                                          │\n        │   - https://nvd.nist.gov/vuln/detail/CVE-2018-10903                                                                                                                                                                                                                                                          │\n        │                                                                                                                                                                                                                                                                                                              │\n        ╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯\n\n                    Summary                     \n┏━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━┓\n┃ Audited Dependencies ┃ Vulnerabilities Found ┃\n┡━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━┩\n│ 69                   │ 2                     │\n└──────────────────────┴───────────────────────┘\n```\n\nCheck out these examples using STDIN:\n```\nconda list --explicit --md5 | jake ddt -t CONDA\nconda list --json | jake ddt -t CONDA_JSON\ncat /path/to/Pipfile.lock | python -m jake.app ddt -t PIPENV\n```\n\nCheck out these examples specifying a manifest:\n```\njake ddt -t PIP -i /path/to/requirements.txt\njake ddt -t PIPENV -i /path/to/Pipfile.lock\n```\n\nA pre-commit hook is also available for use\n\n```Yaml\n  - repo: https://github.com/sonatype-nexus-community/jake\n    rev: "v1.3.0"\n    hooks:\n      - id: scan\n```\n\n#### Whitelisting\n\nWhitelisting of vulnerabilities can be done! To whitelist vulnerabilities add the `--whitelist` argument and pass a json file like this:\n\n```\n> jake ddt --whitelist jake-whitelist.json\n\n```\n\nThe file should look like this:\n\n```json\n{"ignore": [{"id": "f19ff95c-cec5-4263-8d3b-e3e64698881e", "reason": "Insert reason here"}]}\n```\n\nThe only field that actually matters is id and that is the ID you receive from OSS Index for a vulnerability.\nYou can add fields such as reason so that you later can understand why you whitelisted a vulnerability.\n\nAny id that is whitelisted will be squelched from the results, and not cause a failure.\n\n### Check for vulnerabilities using Sonatype Nexus Lifecycle\n\nAccess Sonatype\'s proprietary vulnerability data using `jake`:\n\n```\n> jake iq --help\n\nusage: jake iq [-h] [-f FILE_PATH] [-t TYPE] -s https://localhost:8070 -i APP_ID -u USER_ID -p PASSWORD [-st STAGE]\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -f FILE_PATH, --input-file FILE_PATH\n                        Where to get input data from. If a path to a file is\n                        not specified directly here,then we will attempt to\n                        read data from STDIN. If there is no data on STDIN, we\n                        will then fall back to looking for standard files in\n                        the current directory that relate to the type of input\n                        indicated by the -t flag.\n  -t TYPE, --type TYPE, -it TYPE, --input-type TYPE\n                        how jake should find the packages from which to\n                        generate your SBOM.ENV = Read from the current Python\n                        Environment; CONDA = Read output from `conda list\n                        --explicit`; CONDA_JSON = Read output from `conda list\n                        --json`; PIP = read from a requirements.txt; PIPENV =\n                        read from Pipfile.lock; POETRY = read from a\n                        poetry.lock. (Default = ENV)\n  -s https://localhost:8070, --server-url https://localhost:8070\n                        Full http(s):// URL to your Nexus Lifecycle server\n  -i APP_ID, --application-id APP_ID\n                        Public Application ID in Nexus Lifecycle\n  -u USER_ID, --username USER_ID\n                        Username for authentication to Nexus Lifecycle\n  -p PASSWORD, --password PASSWORD\n                        Password for authentication to Nexus Lifecycle\n  -st STAGE, --stage STAGE\n                        The stage for the report\n```\n\nSo passing parameters that suit your Nexus Lifecycle environment you can get a report:\n\n```\n> jake iq -s https://my-nexus-lifecyle -i APP_ID -u USERNAME -p PASSWORD\n\n                   ___           ___           ___     \n       ___        /  /\\         /  /\\         /  /\\    \n      /__/\\      /  /::\\       /  /:/        /  /::\\   \n      \\__\\:\\    /  /:/\\:\\     /  /:/        /  /:/\\:\\  \n  ___ /  /::\\  /  /::\\ \\:\\   /  /::\\____   /  /::\\ \\:\\ \n /__/\\  /:/\\/ /__/:/\\:\\_\\:\\ /__/:/\\:::::\\ /__/:/\\:\\ \\:\\\n \\  \\:\\/:/~~  \\__\\/  \\:\\/:/ \\__\\/~|:|~~~~ \\  \\:\\ \\:\\_\\/\n  \\  \\::/          \\__\\::/     |  |:|      \\  \\:\\ \\:\\  \n   \\__\\/           /  /:/      |  |:|       \\  \\:\\_\\/  \n                  /__/:/       |__|:|        \\  \\:\\    \n                  \\__\\/         \\__\\|         \\__\\/    \n\n                                                  \n            /)                     /)             \n        _/_(/    _     _  __   _  (/_   _         \n o   o  (__/ )__(/_   /_)_/ (_(_(_/(___(/_ o   o  \n                                                  \n                                                  \n\nJake Version: 1.0.1\nPut your Python dependencies in a chokehold\n\n🐍 IQ Server at https://my-nexus-lifecyle is up and accessible (0:00:00.14)\n🐍 Collected 42 packages from your environment (0:00:00.09)\n🧨 Something slithers around your ankle! There are policy warnings from Sonatype Nexus IQ. (0:00:11.50)\n\nYour Sonatype Nexus IQ Lifecycle Report is available here:\n  HTML: https://my-nexus-lifecyle/ui/links/application/APP_ID/report/4831bcb7fbaa45c3a2481048e446b598\n  PDF:  https://my-nexus-lifecyle/ui/links/application/APP_ID/report/4831bcb7fbaa45c3a2481048e446b598/pdf\n```\n\n## Why Jake?\n\nJake The Snake was scared of Snakes. The finishing move was DDT. He finishes the Snake with DDT.\n\nWho better to wrangle those slippery dependencies in any virtual or real environment.\n\n## Python Support\n\nWe endeavour to support all functionality for all [current actively supported Python versions](https://www.python.org/downloads/).\nHowever, some features may not be possible/present in older Python versions due to their lack of support.\n\n## Changelog\n\nSee our [CHANGELOG](./CHANGELOG.md).\n\n## Releasing\n\nWe perform releases manually by clicking the "On Hold" button in the CircleCI web page.\n\nIf you see a feature in the code that we have not released, please speak up, and we\'ll be sure to click the magic button.\n\nWe use [python-semantic-release](https://python-semantic-release.readthedocs.io/en/latest/) to generate releases\nfrom commits to the `main` branch.\n\nFor example, to perform a "patch" release, add a commit to `main` with a comment like below. The `fix: ` prefix matters.\n\n```\nfix: Resolve vulnerability: CVE-2020-27783 in lxml\n```\n\n## The Fine Print\n\nRemember:\n\nIt is worth noting that this is **NOT SUPPORTED** by Sonatype, and is a contribution of ours to the open source\ncommunity (read: you!)\n\n* Use this contribution at the risk tolerance that you have\n* Do NOT file Sonatype support tickets related to `ossindex-lib`\n* DO file issues here on GitHub, so that the community can pitch in\n\nPhew, that was easier than I thought. Last but not least of all - have fun!\n',
-    'author': 'Sonatype Community',
-    'author_email': 'community-group@sonatype.com',
-    'maintainer': 'Sonatype Community',
-    'maintainer_email': 'community-group@sonatype.com',
-    'url': 'https://github.com/sonatype-nexus-community/jake',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.6.2,<4.0.0',
-}
+    Licensed under the Apache License, Version 2.0 (the "License");
+    you may not use this file except in compliance with the License.
+    You may obtain a copy of the License at
 
+        http://www.apache.org/licenses/LICENSE-2.0
+
+    Unless required by applicable law or agreed to in writing, software
+    distributed under the License is distributed on an "AS IS" BASIS,
+    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+    See the License for the specific language governing permissions and
+    limitations under the License.
+
+-->
+
+<p align="center">
+    <img src="https://raw.githubusercontent.com/sonatype-nexus-community/jake/main/docs/images/jake.png" width="350" alt="jake icon"/>
+</p>
+
+# Jake
+
+[![CircleCI](https://circleci.com/gh/sonatype-nexus-community/jake/tree/main.svg?style=svg)](https://circleci.com/gh/sonatype-nexus-community/jake/tree/main)
+![Python Version Support](https://img.shields.io/badge/python-3.6+-blue)
+[![PyPI Version](https://img.shields.io/pypi/v/jake?label=PyPI&logo=pypi)](https://pypi.org/project/jake)
+[![GitHub license](https://img.shields.io/github/license/sonatype-nexus-community/jake)](https://github.com/sonatype-nexus-community/jake/blob/main/LICENSE)
+[![GitHub issues](https://img.shields.io/github/issues/sonatype-nexus-community/jake)](https://github.com/sonatype-nexus-community/jake/issues)
+[![GitHub forks](https://img.shields.io/github/forks/sonatype-nexus-community/jake)](https://github.com/sonatype-nexus-community/jake/network)
+[![GitHub stars](https://img.shields.io/github/stars/sonatype-nexus-community/jake)](https://github.com/sonatype-nexus-community/jake/stargazers)
+
+----
+
+`jake` is a tool to check for your Python environments and applications that can:
+- produce CycloneDX software bill-of-materials
+- report on known vulnerabilities
+
+`jake` is powered by [Sonatype OSS Index](https://ossindex.sonatype.org) and can also be used with 
+[Sonatype's Nexus IQ Server](https://www.sonatype.com/product-nexus-lifecycle).
+
+## Installation
+
+Install from pypi.org as you would any other Python module:
+
+```
+pip install jake
+```
+
+or 
+
+```
+poetry add jake
+```
+
+_Other Python package managers are available._
+
+## Usage
+
+### Getting Started
+
+`jake` can guide you...
+
+```
+> jake --help
+usage: jake [-h] [-v] [-w] [-X]  ...
+
+Put your Python dependencies in a chokehold
+
+optional arguments:
+  -h, --help       show this help message and exit
+  -v, --version    show which version of jake you are running
+  -w, --warn-only  prevents exit with non-zero code when issues have been
+                   detected
+  -X               enable debug output
+
+Jake sub-commands:
+  
+    iq             perform a scan backed by Nexus Lifecycle
+    ddt            perform a scan backed by OSS Index
+    sbom           generate a CycloneDX software-bill-of-materials (no
+                   vulnerabilities)
+```
+
+`jake` will exit with code `0` under normal operation and `1` if vulnerabilities are found (OssIndex) or Policy 
+Violations are detected (Nexus IQ), unless you pass the `-w` flag in which case `jake` will always exit with code `0`....
+
+### Generating an SBOM
+
+`jake` can take data from various inputs (or just look at your current Python environment) and produce a CycloneDX for 
+you.
+
+```
+> jake sbom --help
+
+usage: jake sbom [-h] [-f FILE_PATH] [-t TYPE] [-o PATH/TO/FILE]
+                   [--output-format {json,xml}]
+                   [--schema-version {1.0,1.1,1.2,1.3}]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -f FILE_PATH, --input FILE_PATH
+                        Where to get input data from. If a path to a file is
+                        not specified directly here,then we will attempt to
+                        read data from STDIN. If there is no data on STDIN, we
+                        will then fall back to looking for standard files in
+                        the current directory that relate to the type of input
+                        indicated by the -t flag.
+  -t TYPE, --type TYPE, -it TYPE, --input-type TYPE
+                        how jake should find the packages from which to
+                        generate your SBOM.ENV = Read from the current Python
+                        Environment; CONDA = Read output from `conda list
+                        --explicit`; CONDA_JSON = Read output from `conda list
+                        --json`; PIP = read from a requirements.txt; PIPENV =
+                        read from Pipfile.lock; POETRY = read from a
+                        poetry.lock. (Default = ENV)
+  -o PATH/TO/FILE, --output-file PATH/TO/FILE
+                        Specify a file to output the SBOM to
+  --output-format {json,xml}
+                        SBOM output format (default = xml)
+  --schema-version {1.0,1.1,1.2,1.3}
+                        CycloneDX schema version to use (default = 1.3)
+```
+
+Check out these examples using STDIN:
+```
+conda list --explicit --md5 | jake sbom -t CONDA
+conda list --json | jake sbom -t CONDA_JSON
+cat /path/to/Pipfile.lock | python -m jake.app sbom -t PIPENV
+```
+
+Check out these examples specifying a manifest:
+```
+jake sbom -t PIP -f /path/to/requirements.txt
+jake sbom -t PIPENV -f /path/to/Pipfile.lock
+```
+
+### Check for vulnerabilities using OSS Index
+
+`jake` will look at the packaged installed in your current Python environment and check these against OSS Index for you.
+Optionally, it can create a CycloneDX software bill-of-materials at the same time in a format that suits you.
+
+```
+> jake ddt --help
+
+usage: jake ddt [-h] [-f FILE_PATH] [-t TYPE] [--clear-cache] [-o PATH/TO/FILE] 
+                   [--output-format {xml,json}]
+                   [--schema-version {1.2,1.1,1.0,1.3}]
+                   [--whitelist OSS_WHITELIST_JSON_FILE]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -f FILE_PATH, --input-file FILE_PATH
+                        Where to get input data from. If a path to a file is
+                        not specified directly here,then we will attempt to
+                        read data from STDIN. If there is no data on STDIN, we
+                        will then fall back to looking for standard files in
+                        the current directory that relate to the type of input
+                        indicated by the -t flag.
+  -t TYPE, --type TYPE, -it TYPE, --input-type TYPE
+                        how jake should find the packages from which to
+                        generate your SBOM.ENV = Read from the current Python
+                        Environment; CONDA = Read output from `conda list
+                        --explicit`; CONDA_JSON = Read output from `conda list
+                        --json`; PIP = read from a requirements.txt; PIPENV =
+                        read from Pipfile.lock; POETRY = read from a
+                        poetry.lock. (Default = ENV)
+  --clear-cache         Clears any local cached OSS Index data prior to execution
+  -o PATH/TO/FILE, --output-file PATH/TO/FILE
+                        Specify a file to output the SBOM to. If not specified the report will be output to the console. STDOUT is not supported.
+  --output-format {xml,json}
+                        SBOM output format (default = xml)
+  --schema-version {1.2,1.1,1.0,1.3}
+                        CycloneDX schema version to use (default = 1.3)
+  --whitelist OSS_WHITELIST_JSON_FILE
+                        Set path to whitelist json file
+```
+
+So you can quickly get a report by running:
+
+```
+> jake ddt
+
+                   ___           ___           ___     
+       ___        /  /\         /  /\         /  /\    
+      /__/\      /  /::\       /  /:/        /  /::\   
+      \__\:\    /  /:/\:\     /  /:/        /  /:/\:\  
+  ___ /  /::\  /  /::\ \:\   /  /::\____   /  /::\ \:\ 
+ /__/\  /:/\/ /__/:/\:\_\:\ /__/:/\:::::\ /__/:/\:\ \:\
+ \  \:\/:/~~  \__\/  \:\/:/ \__\/~|:|~~~~ \  \:\ \:\_\/
+  \  \::/          \__\::/     |  |:|      \  \:\ \:\  
+   \__\/           /  /:/      |  |:|       \  \:\_\/  
+                  /__/:/       |__|:|        \  \:\    
+                  \__\/         \__\|         \__\/    
+
+                                                  
+            /)                     /)             
+        _/_(/    _     _  __   _  (/_   _         
+ o   o  (__/ )__(/_   /_)_/ (_(_(_/(___(/_ o   o  
+                                                  
+                                                  
+
+Jake Version: 1.1.0
+Put your Python dependencies in a chokehold.
+
+🐍 Collected 42 packages from your environment (0:00:00.10)
+🐍 Successfully queried OSS Index for package and vulnerability info (0:00:00.59)
+🐍 Sane number of results from OSS Index
+
+
+╔Summary═══════════════╦════╗
+║ Audited Dependencies ║ 42 ║
+╠══════════════════════╬════╣
+║ Vulnerablities Found ║ 0  ║
+╚══════════════════════╩════╝
+```
+
+...and this is what `jake` will output if any bad things are found:
+```
+                   ___           ___           ___     
+       ___        /  /\         /  /\         /  /\    
+      /__/\      /  /::\       /  /:/        /  /::\   
+      \__\:\    /  /:/\:\     /  /:/        /  /:/\:\  
+  ___ /  /::\  /  /::\ \:\   /  /::\____   /  /::\ \:\ 
+ /__/\  /:/\/ /__/:/\:\_\:\ /__/:/\:::::\ /__/:/\:\ \:\
+ \  \:\/:/~~  \__\/  \:\/:/ \__\/~|:|~~~~ \  \:\ \:\_\/
+  \  \::/          \__\::/     |  |:|      \  \:\ \:\  
+   \__\/           /  /:/      |  |:|       \  \:\_\/  
+                  /__/:/       |__|:|        \  \:\    
+                  \__\/         \__\|         \__\/    
+
+                                                  
+            /)                     /)             
+        _/_(/    _     _  __   _  (/_   _         
+ o   o  (__/ )__(/_   /_)_/ (_(_(_/(___(/_ o   o  
+                                                  
+                                                  
+
+Jake Version: 1.1.5
+Put your Python dependencies in a chokehold
+
+🐍 Collected 69 packages from your environment                       ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 100% -:--:--
+🐍 Successfully queried OSS Index for package and vulnerability info ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 100% -:--:--
+🐍 Sane number of results from OSS Index                             ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━ 100% -:--:--
+
+[59/69] - pkg:pypi/cryptography@2.2 [VULNERABLE]
+Vulnerability Details for pkg:pypi/cryptography@2.2                                                                                                                                                                                                                                                                     
+├── ⚠  ID: 333aca51-7375-4a9d-be64-16d316ab9274                                                                                                                                                                                                                                                                         
+│   └── ╭─ CVE-2020-36242 ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+│       │                                                                                                                                                                                                                                                                                                              │
+│       │ In the cryptography package before 3.3.2 for Python, certain sequences of update calls to symmetrically encrypt multi-GB values could result in an integer overflow and buffer overflow, as demonstrated by the Fernet class.                                                                                │
+│       │                                                                                                                                                                                                                                                                                                              │
+│       │ Details:                                                                                                                                                                                                                                                                                                     │
+│       │   - CVSS Score: 9.1 - Critical                                                                                                                                                                                                                                                                               │
+│       │   - CVSS Vector: CVSS:3.0/AV:N/AC:L/PR:N/UI:N/S:U/C:H/I:N/A:H                                                                                                                                                                                                                                                │
+│       │   - CWE: Unknown                                                                                                                                                                                                                                                                                             │
+│       │                                                                                                                                                                                                                                                                                                              │
+│       │ References:                                                                                                                                                                                                                                                                                                  │
+│       │   - https://ossindex.sonatype.org/vulnerability/333aca51-7375-4a9d-be64-16d316ab9274?component-type=pypi&component-name=cryptography&utm_source=python-oss-index-lib%400.2.1&utm_medium=integration                                                                                                          │
+│       │   - https://nvd.nist.gov/vuln/detail/CVE-2020-36242                                                                                                                                                                                                                                                          │
+│       │                                                                                                                                                                                                                                                                                                              │
+│       ╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+└── ⚠  ID: f19ff95c-cec5-4263-8d3b-e3e64698881e                                                                                                                                                                                                                                                                         
+    └── ╭─ CVE-2018-10903 ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
+        │                                                                                                                                                                                                                                                                                                              │
+        │ A flaw was found in python-cryptography versions between >=1.9.0 and <2.3. The finalize_with_tag API did not enforce a minimum tag length. If a user did not validate the input length prior to passing it to finalize_with_tag an attacker could craft an invalid payload with a shortened tag (e.g. 1      │
+        │ byte) such that they would have a 1 in 256 chance of passing the MAC check. GCM tag forgeries can cause key leakage.                                                                                                                                                                                         │
+        │                                                                                                                                                                                                                                                                                                              │
+        │ Details:                                                                                                                                                                                                                                                                                                     │
+        │   - CVSS Score: 7.5 - High                                                                                                                                                                                                                                                                                   │
+        │   - CVSS Vector: CVSS:3.0/AV:N/AC:L/PR:N/UI:N/S:U/C:H/I:N/A:N                                                                                                                                                                                                                                                │
+        │   - CWE: Unknown                                                                                                                                                                                                                                                                                             │
+        │                                                                                                                                                                                                                                                                                                              │
+        │ References:                                                                                                                                                                                                                                                                                                  │
+        │   - https://ossindex.sonatype.org/vulnerability/f19ff95c-cec5-4263-8d3b-e3e64698881e?component-type=pypi&component-name=cryptography&utm_source=python-oss-index-lib%400.2.1&utm_medium=integration                                                                                                          │
+        │   - https://bugzilla.redhat.com/show_bug.cgi?id=CVE-2018-10903                                                                                                                                                                                                                                               │
+        │   - https://github.com/pyca/cryptography/pull/4342/commits/688e0f673bfbf43fa898994326c6877f00ab19ef                                                                                                                                                                                                          │
+        │   - https://nvd.nist.gov/vuln/detail/CVE-2018-10903                                                                                                                                                                                                                                                          │
+        │                                                                                                                                                                                                                                                                                                              │
+        ╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
+
+                    Summary                     
+┏━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━┓
+┃ Audited Dependencies ┃ Vulnerabilities Found ┃
+┡━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━┩
+│ 69                   │ 2                     │
+└──────────────────────┴───────────────────────┘
+```
+
+Check out these examples using STDIN:
+```
+conda list --explicit --md5 | jake ddt -t CONDA
+conda list --json | jake ddt -t CONDA_JSON
+cat /path/to/Pipfile.lock | python -m jake.app ddt -t PIPENV
+```
+
+Check out these examples specifying a manifest:
+```
+jake ddt -t PIP -f /path/to/requirements.txt
+jake ddt -t PIPENV -f /path/to/Pipfile.lock
+```
+
+A pre-commit hook is also available for use
+
+```Yaml
+  - repo: https://github.com/sonatype-nexus-community/jake
+    rev: "v1.3.0"
+    hooks:
+      - id: scan
+```
+
+#### Whitelisting
+
+Whitelisting of vulnerabilities can be done! To whitelist vulnerabilities add the `--whitelist` argument and pass a json file like this:
+
+```
+> jake ddt --whitelist jake-whitelist.json
+
+```
+
+The file should look like this:
+
+```json
+{"ignore": [{"id": "f19ff95c-cec5-4263-8d3b-e3e64698881e", "reason": "Insert reason here"}]}
+```
+
+The only field that actually matters is id and that is the ID you receive from OSS Index for a vulnerability.
+You can add fields such as reason so that you later can understand why you whitelisted a vulnerability.
+
+Any id that is whitelisted will be squelched from the results, and not cause a failure.
+
+### Check for vulnerabilities using Sonatype Nexus Lifecycle
+
+Access Sonatype's proprietary vulnerability data using `jake`:
+
+```
+> jake iq --help
+
+usage: jake iq [-h] [-f FILE_PATH] [-t TYPE] -s https://localhost:8070 -i APP_ID -u USER_ID -p PASSWORD [-st STAGE]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -f FILE_PATH, --input-file FILE_PATH
+                        Where to get input data from. If a path to a file is
+                        not specified directly here,then we will attempt to
+                        read data from STDIN. If there is no data on STDIN, we
+                        will then fall back to looking for standard files in
+                        the current directory that relate to the type of input
+                        indicated by the -t flag.
+  -t TYPE, --type TYPE, -it TYPE, --input-type TYPE
+                        how jake should find the packages from which to
+                        generate your SBOM.ENV = Read from the current Python
+                        Environment; CONDA = Read output from `conda list
+                        --explicit`; CONDA_JSON = Read output from `conda list
+                        --json`; PIP = read from a requirements.txt; PIPENV =
+                        read from Pipfile.lock; POETRY = read from a
+                        poetry.lock. (Default = ENV)
+  -s https://localhost:8070, --server-url https://localhost:8070
+                        Full http(s):// URL to your Nexus Lifecycle server
+  -i APP_ID, --application-id APP_ID
+                        Public Application ID in Nexus Lifecycle
+  -u USER_ID, --username USER_ID
+                        Username for authentication to Nexus Lifecycle
+  -p PASSWORD, --password PASSWORD
+                        Password for authentication to Nexus Lifecycle
+  -st STAGE, --stage STAGE
+                        The stage for the report
+```
+
+So passing parameters that suit your Nexus Lifecycle environment you can get a report:
+
+```
+> jake iq -s https://my-nexus-lifecyle -i APP_ID -u USERNAME -p PASSWORD
+
+                   ___           ___           ___     
+       ___        /  /\         /  /\         /  /\    
+      /__/\      /  /::\       /  /:/        /  /::\   
+      \__\:\    /  /:/\:\     /  /:/        /  /:/\:\  
+  ___ /  /::\  /  /::\ \:\   /  /::\____   /  /::\ \:\ 
+ /__/\  /:/\/ /__/:/\:\_\:\ /__/:/\:::::\ /__/:/\:\ \:\
+ \  \:\/:/~~  \__\/  \:\/:/ \__\/~|:|~~~~ \  \:\ \:\_\/
+  \  \::/          \__\::/     |  |:|      \  \:\ \:\  
+   \__\/           /  /:/      |  |:|       \  \:\_\/  
+                  /__/:/       |__|:|        \  \:\    
+                  \__\/         \__\|         \__\/    
+
+                                                  
+            /)                     /)             
+        _/_(/    _     _  __   _  (/_   _         
+ o   o  (__/ )__(/_   /_)_/ (_(_(_/(___(/_ o   o  
+                                                  
+                                                  
+
+Jake Version: 1.0.1
+Put your Python dependencies in a chokehold
+
+🐍 IQ Server at https://my-nexus-lifecyle is up and accessible (0:00:00.14)
+🐍 Collected 42 packages from your environment (0:00:00.09)
+🧨 Something slithers around your ankle! There are policy warnings from Sonatype Nexus IQ. (0:00:11.50)
+
+Your Sonatype Nexus IQ Lifecycle Report is available here:
+  HTML: https://my-nexus-lifecyle/ui/links/application/APP_ID/report/4831bcb7fbaa45c3a2481048e446b598
+  PDF:  https://my-nexus-lifecyle/ui/links/application/APP_ID/report/4831bcb7fbaa45c3a2481048e446b598/pdf
+```
+
+## Why Jake?
+
+Jake The Snake was scared of Snakes. The finishing move was DDT. He finishes the Snake with DDT.
+
+Who better to wrangle those slippery dependencies in any virtual or real environment.
+
+## Python Support
+
+We endeavour to support all functionality for all [current actively supported Python versions](https://www.python.org/downloads/).
+However, some features may not be possible/present in older Python versions due to their lack of support.
+
+## Changelog
+
+See our [CHANGELOG](./CHANGELOG.md).
+
+## Releasing
+
+We perform releases manually by clicking the "On Hold" button in the CircleCI web page.
+
+If you see a feature in the code that we have not released, please speak up, and we'll be sure to click the magic button.
+
+We use [python-semantic-release](https://python-semantic-release.readthedocs.io/en/latest/) to generate releases
+from commits to the `main` branch.
+
+For example, to perform a "patch" release, add a commit to `main` with a comment like below. The `fix: ` prefix matters.
+
+```
+fix: Resolve vulnerability: CVE-2020-27783 in lxml
+```
+
+## The Fine Print
+
+Remember:
+
+It is worth noting that this is **NOT SUPPORTED** by Sonatype, and is a contribution of ours to the open source
+community (read: you!)
+
+* Use this contribution at the risk tolerance that you have
+* Do NOT file Sonatype support tickets related to `ossindex-lib`
+* DO file issues here on GitHub, so that the community can pitch in
+
+Phew, that was easier than I thought. Last but not least of all - have fun!
 
-setup(**setup_kwargs)
```

