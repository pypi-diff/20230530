# Comparing `tmp/rstcloth-0.5.3.tar.gz` & `tmp/rstcloth-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rstcloth-0.5.3.tar", max compression
+gzip compressed data, was "rstcloth-0.5.4.tar", max compression
```

## Comparing `rstcloth-0.5.3.tar` & `rstcloth-0.5.4.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1687 2023-03-09 08:10:36.861375 rstcloth-0.5.3/LICENSE
--rw-r--r--   0        0        0     4569 2023-03-09 08:10:36.861375 rstcloth-0.5.3/README.md
--rw-r--r--   0        0        0     1819 2023-03-09 08:10:36.861375 rstcloth-0.5.3/pyproject.toml
--rw-r--r--   0        0        0       56 2023-03-09 08:10:36.861375 rstcloth-0.5.3/rstcloth/__init__.py
--rw-r--r--   0        0        0    17332 2023-03-09 08:10:36.861375 rstcloth-0.5.3/rstcloth/rstcloth.py
--rw-r--r--   0        0        0      441 2023-03-09 08:10:36.861375 rstcloth-0.5.3/rstcloth/utils.py
--rw-r--r--   0        0        0     5613 2023-03-09 08:15:17.605149 rstcloth-0.5.3/setup.py
--rw-r--r--   0        0        0     6040 2023-03-09 08:15:17.605723 rstcloth-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1687 2023-05-30 15:28:21.257196 rstcloth-0.5.4/LICENSE
+-rw-r--r--   0        0        0     4569 2023-05-30 15:28:21.257196 rstcloth-0.5.4/README.md
+-rw-r--r--   0        0        0     1828 2023-05-30 15:28:21.257196 rstcloth-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0       56 2023-05-30 15:28:21.257196 rstcloth-0.5.4/rstcloth/__init__.py
+-rw-r--r--   0        0        0    17332 2023-05-30 15:28:21.257196 rstcloth-0.5.4/rstcloth/rstcloth.py
+-rw-r--r--   0        0        0      441 2023-05-30 15:28:21.257196 rstcloth-0.5.4/rstcloth/utils.py
+-rw-r--r--   0        0        0     6241 1970-01-01 00:00:00.000000 rstcloth-0.5.4/PKG-INFO
```

### Comparing `rstcloth-0.5.3/LICENSE` & `rstcloth-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rstcloth-0.5.3/README.md` & `rstcloth-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `rstcloth-0.5.3/pyproject.toml` & `rstcloth-0.5.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rstcloth"
-version = "0.5.3"
+version = "0.5.4"
 description = "A simple Python API for generating RestructuredText."
 authors = ["Tom Clark"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
@@ -25,23 +25,23 @@
 packages = [{ include = "rstcloth" },]
 
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.12"
 sphinx = ">=2,<6"
 Pygments = "^2.12.0"
-PyYAML = "^6.0"
+PyYAML = ">=5,<7"
 # These are here as extras to allow them to be installed as extras
 # Strictly they're dev-dependencies but they don't get installed that way
 # (see https://github.com/python-poetry/poetry/issues/3348)
 sphinx-rtd-theme = {version = "1.0.0", optional = true}
 sphinx-tabs = {version = "3.2.0", optional = true}
 sphinx-charts = {version = "0.1.2", optional = true}
 sphinx-math-dollar = {version = "1.2.0", optional = true}
-tabulate = "^0.8.9"
+tabulate = ">=0.8.9,<0.10"
 
 [tool.poetry.dev-dependencies]
 coverage = "^6.2"
 pre-commit = "^2.17.0"
 pytest-sugar = "^0.9.4"
 pytest = "^6.2.5"
 # tox = "^3.24.5"
```

### Comparing `rstcloth-0.5.3/rstcloth/rstcloth.py` & `rstcloth-0.5.4/rstcloth/rstcloth.py`

 * *Files identical despite different names*

### Comparing `rstcloth-0.5.3/setup.py` & `rstcloth-0.5.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,153 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: rstcloth
+Version: 0.5.4
+Summary: A simple Python API for generating RestructuredText.
+Home-page: https://github.com/thclark/rstcloth
+License: MIT
+Keywords: sphinx,rst,restructuredtext,documentation,rest,docutils
+Author: Tom Clark
+Requires-Python: >=3.7,<3.12
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Documentation
+Classifier: Topic :: Documentation :: Sphinx
+Classifier: Topic :: Software Development :: Documentation
+Classifier: Topic :: Text Processing
+Classifier: Topic :: Utilities
+Provides-Extra: docs
+Requires-Dist: PyYAML (>=5,<7)
+Requires-Dist: Pygments (>=2.12.0,<3.0.0)
+Requires-Dist: sphinx (>=2,<6)
+Requires-Dist: sphinx-charts (==0.1.2) ; extra == "docs"
+Requires-Dist: sphinx-math-dollar (==1.2.0) ; extra == "docs"
+Requires-Dist: sphinx-rtd-theme (==1.0.0) ; extra == "docs"
+Requires-Dist: sphinx-tabs (==3.2.0) ; extra == "docs"
+Requires-Dist: tabulate (>=0.8.9,<0.10)
+Project-URL: Repository, https://github.com/thclark/rstcloth
+Description-Content-Type: text/markdown
 
-packages = \
-['rstcloth']
+![cd](https://github.com/thclark/rstcloth/actions/workflows/cd.yml/badge.svg)
+[![codecov](https://codecov.io/gh/thclark/rstcloth/branch/main/graph/badge.svg)](https://codecov.io/gh/thclark/rstcloth)
+[![PyPI version](https://badge.fury.io/py/rstcloth.svg)](https://badge.fury.io/py/rstcloth)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+[![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
+[![Documentation Status](https://readthedocs.org/projects/rstcloth/badge/?version=latest)](https://rstcloth.readthedocs.io/en/latest/?badge=latest)
 
-package_data = \
-{'': ['*']}
+# RstCloth
 
-install_requires = \
-['PyYAML>=6.0,<7.0',
- 'Pygments>=2.12.0,<3.0.0',
- 'sphinx>=2,<6',
- 'tabulate>=0.8.9,<0.9.0']
-
-extras_require = \
-{'docs': ['sphinx-rtd-theme==1.0.0',
-          'sphinx-tabs==3.2.0',
-          'sphinx-charts==0.1.2',
-          'sphinx-math-dollar==1.2.0']}
-
-setup_kwargs = {
-    'name': 'rstcloth',
-    'version': '0.5.3',
-    'description': 'A simple Python API for generating RestructuredText.',
-    'long_description': '![cd](https://github.com/thclark/rstcloth/actions/workflows/cd.yml/badge.svg)\n[![codecov](https://codecov.io/gh/thclark/rstcloth/branch/main/graph/badge.svg)](https://codecov.io/gh/thclark/rstcloth)\n[![PyPI version](https://badge.fury.io/py/rstcloth.svg)](https://badge.fury.io/py/rstcloth)\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)\n[![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n[![Documentation Status](https://readthedocs.org/projects/rstcloth/badge/?version=latest)](https://rstcloth.readthedocs.io/en/latest/?badge=latest)\n\n# RstCloth\n\nreStructuredText is a powerful human-centric markup language that is\nwell defined, flexible, with powerful tools that make writing and\nmaintaining text easy and pleasurable. Humans can edit\nreStructuredText without the aide of complex editing tools, and the\nresulting source is easy to manipulate and process.\n\nAs an alternative and a supplement, RstCloth is a Python API for\nwriting well formed reStructuredText programatically.\n\nFind the [project documentation here](https://rstcloth.readthedocs.io)\n\n## Developer notes\n\nRepo is based on [thclark/python-library-template](https://github.com/thclark/python-library-template):\n\n- vscode `.devcontainer`\n- black style\n- sphinx docs with some examples and automatic build\n- pre-commit hooks\n- tox tests\n- github actions ci + cd\n- code coverage\n\n### Using VSCode\n\nCheck out the repo and use the remote `.devcontainer` to start developing, with everything installed out of the box.\n\n### In other IDEs\n\nUse `poetry --extras docs` to install the project and get started. You also You need to install pre-commit to get the hooks working. Do:\n\n```\npip install pre-commit\npre-commit install && pre-commit install -t commit-msg\n```\n\nOnce that\'s done, each time you make a commit, a wide range of checks are made and the project file formats are applied.\n\nUpon failure, the commit will halt. **Re-running the commit will automatically fix most issues** except:\n\n- The flake8 checks... hopefully over time Black (which fixes most things automatically already) will negate need for it.\n- You\'ll have to fix documentation yourself prior to a successful commit (there\'s no auto fix for that!!).\n\nYou can run pre-commit hooks without making a commit, too, like:\n\n```\npre-commit run black --all-files\n```\n\nor\n\n```\n# -v gives verbose output, useful for figuring out why docs won\'t build\npre-commit run build-docs -v\n```\n\n### Contributing\n\n- Please raise an issue on the board (or add your \\$0.02 to an existing issue) so the maintainers know\n  what\'s happening and can advise / steer you.\n\n- Create a fork of rstcloth, undertake your changes on a new branch, (see `.pre-commit-config.yaml` for branch naming conventions).\n\n- To make life easy for us, use our conventional commits pattern (if you\'ve got pre-commit installed correctly, it\'ll guide you on your first commit) to make your commits (if not, we\'ll try to preserve your history, but might have to squashmerge which would lose your contribution history)\n\n- Adopt a Test Driven Development approach to implementing new features or fixing bugs.\n\n- Ask the `rstcloth` maintainers _where_ to make your pull request. We\'ll create a version branch, according to the\n  roadmap, into which you can make your PR. We\'ll help review the changes and improve the PR.\n\n- Once checks have passed, test coverage of the new code is >=95%, documentation is updated and the Review is passed, we\'ll merge into the version branch.\n\n### Release process\n\nReleases are automated using conventional-commits and GitHub Actions.\n\n## Documents\n\n### Building documents automatically\n\nIn the VSCode `.devcontainer`, the RestructuredText extension should build the docs live for you (right click the `.rst` file and hit "Open Preview").\n\nOn each commit, the documentation will build automatically in a pre-configured environment. The way pre-commit works, you won\'t be allowed to make the commit unless the documentation builds,\nthis way we avoid getting broken documentation pushed to the main repository on any commit sha, so we can rely on\nbuilds working.\n\n### Building documents manually\n\n**If you did need to build the documentation**\n\nInstall `doxgen`. On a mac, that\'s `brew install doxygen`; other systems may differ.\n\nInstall sphinx and other requirements for building the docs:\n\n```\npoetry install --extras docs\n```\n\nRun the build process:\n\n```\nsphinx-build -b html docs/source docs/build\n```\n',
-    'author': 'Tom Clark',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/thclark/rstcloth',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7,<3.12',
-}
+reStructuredText is a powerful human-centric markup language that is
+well defined, flexible, with powerful tools that make writing and
+maintaining text easy and pleasurable. Humans can edit
+reStructuredText without the aide of complex editing tools, and the
+resulting source is easy to manipulate and process.
 
+As an alternative and a supplement, RstCloth is a Python API for
+writing well formed reStructuredText programatically.
+
+Find the [project documentation here](https://rstcloth.readthedocs.io)
+
+## Developer notes
+
+Repo is based on [thclark/python-library-template](https://github.com/thclark/python-library-template):
+
+- vscode `.devcontainer`
+- black style
+- sphinx docs with some examples and automatic build
+- pre-commit hooks
+- tox tests
+- github actions ci + cd
+- code coverage
+
+### Using VSCode
+
+Check out the repo and use the remote `.devcontainer` to start developing, with everything installed out of the box.
+
+### In other IDEs
+
+Use `poetry --extras docs` to install the project and get started. You also You need to install pre-commit to get the hooks working. Do:
+
+```
+pip install pre-commit
+pre-commit install && pre-commit install -t commit-msg
+```
+
+Once that's done, each time you make a commit, a wide range of checks are made and the project file formats are applied.
+
+Upon failure, the commit will halt. **Re-running the commit will automatically fix most issues** except:
+
+- The flake8 checks... hopefully over time Black (which fixes most things automatically already) will negate need for it.
+- You'll have to fix documentation yourself prior to a successful commit (there's no auto fix for that!!).
+
+You can run pre-commit hooks without making a commit, too, like:
+
+```
+pre-commit run black --all-files
+```
+
+or
+
+```
+# -v gives verbose output, useful for figuring out why docs won't build
+pre-commit run build-docs -v
+```
+
+### Contributing
+
+- Please raise an issue on the board (or add your \$0.02 to an existing issue) so the maintainers know
+  what's happening and can advise / steer you.
+
+- Create a fork of rstcloth, undertake your changes on a new branch, (see `.pre-commit-config.yaml` for branch naming conventions).
+
+- To make life easy for us, use our conventional commits pattern (if you've got pre-commit installed correctly, it'll guide you on your first commit) to make your commits (if not, we'll try to preserve your history, but might have to squashmerge which would lose your contribution history)
+
+- Adopt a Test Driven Development approach to implementing new features or fixing bugs.
+
+- Ask the `rstcloth` maintainers _where_ to make your pull request. We'll create a version branch, according to the
+  roadmap, into which you can make your PR. We'll help review the changes and improve the PR.
+
+- Once checks have passed, test coverage of the new code is >=95%, documentation is updated and the Review is passed, we'll merge into the version branch.
+
+### Release process
+
+Releases are automated using conventional-commits and GitHub Actions.
+
+## Documents
+
+### Building documents automatically
+
+In the VSCode `.devcontainer`, the RestructuredText extension should build the docs live for you (right click the `.rst` file and hit "Open Preview").
+
+On each commit, the documentation will build automatically in a pre-configured environment. The way pre-commit works, you won't be allowed to make the commit unless the documentation builds,
+this way we avoid getting broken documentation pushed to the main repository on any commit sha, so we can rely on
+builds working.
+
+### Building documents manually
+
+**If you did need to build the documentation**
+
+Install `doxgen`. On a mac, that's `brew install doxygen`; other systems may differ.
+
+Install sphinx and other requirements for building the docs:
+
+```
+poetry install --extras docs
+```
+
+Run the build process:
+
+```
+sphinx-build -b html docs/source docs/build
+```
 
-setup(**setup_kwargs)
```

