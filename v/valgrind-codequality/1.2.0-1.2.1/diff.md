# Comparing `tmp/valgrind_codequality-1.2.0.tar.gz` & `tmp/valgrind_codequality-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valgrind_codequality-1.2.0.tar", max compression
+gzip compressed data, was "valgrind_codequality-1.2.1.tar", max compression
```

## Comparing `valgrind_codequality-1.2.0.tar` & `valgrind_codequality-1.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0     1105 2023-02-03 17:45:59.054645 valgrind_codequality-1.2.0/LICENSE
--rwxr-xr-x   0        0        0     3526 2023-05-01 13:06:47.846935 valgrind_codequality-1.2.0/README.md
--rwxr-xr-x   0        0        0     1617 2023-05-29 12:54:37.862882 valgrind_codequality-1.2.0/pyproject.toml
--rwxr-xr-x   0        0        0    13258 2023-05-29 12:54:37.880938 valgrind_codequality-1.2.0/valgrind_codequality/__init__.py
--rwxr-xr-x   0        0        0     4535 2023-05-29 12:37:31.605726 valgrind_codequality-1.2.0/valgrind_codequality/__main__.py
--rw-r--r--   0        0        0     4448 1970-01-01 00:00:00.000000 valgrind_codequality-1.2.0/setup.py
--rw-r--r--   0        0        0     4377 1970-01-01 00:00:00.000000 valgrind_codequality-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1105 2023-05-30 11:17:04.089514 valgrind_codequality-1.2.1/LICENSE
+-rw-r--r--   0        0        0     3526 2023-05-30 11:17:04.089514 valgrind_codequality-1.2.1/README.md
+-rw-r--r--   0        0        0     1617 2023-05-30 11:17:44.637177 valgrind_codequality-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0    13305 2023-05-30 11:17:44.639177 valgrind_codequality-1.2.1/valgrind_codequality/__init__.py
+-rw-r--r--   0        0        0     4535 2023-05-30 11:17:04.090514 valgrind_codequality-1.2.1/valgrind_codequality/__main__.py
+-rw-r--r--   0        0        0     4448 1970-01-01 00:00:00.000000 valgrind_codequality-1.2.1/setup.py
+-rw-r--r--   0        0        0     4377 1970-01-01 00:00:00.000000 valgrind_codequality-1.2.1/PKG-INFO
```

### Comparing `valgrind_codequality-1.2.0/LICENSE` & `valgrind_codequality-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `valgrind_codequality-1.2.0/README.md` & `valgrind_codequality-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `valgrind_codequality-1.2.0/pyproject.toml` & `valgrind_codequality-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "valgrind-codequality"
-version = "1.2.0"
+version = "1.2.1"
 description = "Convert Valgrind XML to GitLab Code Quality JSON file."
 authors = ["Arnaud Moura <arnaudmoura@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "valgrind_codequality"}]
 
 [tool.poetry.urls]
```

### Comparing `valgrind_codequality-1.2.0/valgrind_codequality/__init__.py` & `valgrind_codequality-1.2.1/valgrind_codequality/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 import os
 import typing
 from copy import deepcopy
 
 # third-party
 import xmltodict
 
-__version__ = "1.2.0"
+__version__ = "1.2.1"
 
 log = logging.getLogger(__name__)
 
 # Source: https://github.com/codeclimate/platform/blob/master/spec/analyzers/SPEC.md#data-types
 CODE_QUAL_ELEMENT = {
     "severity": "",
     "description": "",
@@ -361,17 +361,18 @@
 
         # Check if path in "obj" contains name to exclude
         exclude_error = False
         if exclude_list:
             path_name = ""
             path_analyse = ""
             for path_name in exclude_list:
-                path_analyse = frame["obj"]
-                if path_name in path_analyse:
-                    exclude_error = True
+                if "obj" in frame:
+                    path_analyse = frame["obj"]
+                    if path_name in path_analyse:
+                        exclude_error = True
                 if "dir" in frame:
                     path_analyse = frame["dir"]
                     if path_name in path_analyse:
                         exclude_error = True
             if exclude_error:
                 log.debug(f"- Exclude because '{path_name}' in {path_analyse}")
                 break
```

### Comparing `valgrind_codequality-1.2.0/valgrind_codequality/__main__.py` & `valgrind_codequality-1.2.1/valgrind_codequality/__main__.py`

 * *Files identical despite different names*

### Comparing `valgrind_codequality-1.2.0/setup.py` & `valgrind_codequality-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 entry_points = \
 {'console_scripts': ['valgrind-codequality = '
                      'valgrind_codequality.__main__:main']}
 
 setup_kwargs = {
     'name': 'valgrind-codequality',
-    'version': '1.2.0',
+    'version': '1.2.1',
     'description': 'Convert Valgrind XML to GitLab Code Quality JSON file.',
     'long_description': '# valgrind-codequality\n\n[![badge-pypi](https://img.shields.io/pypi/v/valgrind-codequality.svg?logo=pypi)](https://pypi.python.org/pypi/valgrind-codequality/)\n&nbsp;\n[![badge-pypi-downloads](https://img.shields.io/pypi/dm/valgrind-codequality)](https://pypi.org/project/valgrind-codequality/)\n\n\n[![badge-pipeline](https://gitlab.com/echopouet/valgrind-codequality/badges/main/pipeline.svg)](https://gitlab.com/echopouet/valgrind-codequality/-/pipelines?scope=branches)\n&nbsp;\n[![badge-coverage](https://gitlab.com/echopouet/valgrind-codequality/badges/main/coverage.svg)](https://gitlab.com/echopouet/valgrind-codequality/-/pipelines?scope=branches)\n&nbsp;\n[![badge-pylint](https://gitlab.com/echopouet/valgrind-codequality/-/jobs/artifacts/main/raw/badge.svg?job=pylint)](https://gitlab.com/echopouet/valgrind-codequality/-/pipelines?scope=branches)\n&nbsp;\n[![badge-formatting](https://gitlab.com/echopouet/valgrind-codequality/-/jobs/artifacts/main/raw/badge.svg?job=format_black)](https://gitlab.com/echopouet/valgrind-codequality/-/pipelines?scope=branches)\n&nbsp;\n[![badge-issues-cnt](https://img.shields.io/badge/dynamic/json?label=issues&query=statistics.counts.opened&url=https%3A%2F%2Fgitlab.com%2Fapi%2Fv4%2Fprojects%2F19114200%2Fissues_statistics%3Fscope%3Dall)](https://gitlab.com/echopouet/valgrind-codequality/-/issues)\n\n\n## About\n\nI wanted reports from [Valgrind](https://valgrind.org/) to appear in GitLab Merge Requests as [Code Quality reports](https://docs.gitlab.com/ee/user/project/merge_requests/code_quality.html#implementing-a-custom-tool), which is a JSON file defined by the Code Quality\'s GitLab.\n\nThat\'s all this does: convert Valgrind XML report to Code Quality JSON.\n\nContributions are welcome.\n\n[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/yellow_img.png)](https://www.buymeacoffee.com/EchoPouet)\n\n### Usage\n\nIt is primarily used as a console script. As such, ensure you have Python 3\'s "scripts" directory in your `PATH` variable.\nFor example, on Linux, that might be `$HOME/.local/bin`.\n\nTo test, try the `--help` or `--version` flags:\n```bash\nvalgrind-codequality --help\n```\n\nThis script follows that example and provides similar command-line options.\nA typical workflow might look like this:\n\n```bash\n# Generate valgrind report as XML\nvalgrind --tool=memcheck --leak-check=full --show-leak-kinds=all --track-origins=yes --verbose --xml=yes --xml-file=valgrind_out.xml your_exe\n# Convert to a Code Climate JSON report\nvalgrind-codequality --input-file valgrind_out.xml --output-file valgrind.json\n```\n\nIf you wanted, you could invoke the script directly as a module, like this:\n\n```bash\n# Run as a module instead (note the underscore in the module name here)\npython -m valgrind_codequality --input-file=valgrind_out.xml --output-file=valgrind.json\n```\n\nNow, in your GitLab CI script, [upload this file](https://docs.gitlab.com/ee/ci/pipelines/job_artifacts.html#artifactsreportscodequality)\nas a Code Quality report.\n\n```yaml\nmy-code-quality:\n  script:\n    - [...]\n  artifacts:\n    reports:\n      codequality: valgrind.json\n```\n\n### Contributing\n\n* Format with [black](https://pypi.org/project/black/)\n* Check with [pylint](https://pypi.org/project/pylint/)\n\n### Credits & Trademarks\n\nvalgrind is an open-source project with a GPL v3.0 license.\n* https://valgrind.org/\n\n"GitLab" is a trademark of GitLab B.V.\n* https://gitlab.com\n* https://docs.gitlab.com/ee/user/project/merge_requests/code_quality.html\n\nAll other trademarks belong to their respective owners.\n',
     'author': 'Arnaud Moura',
     'author_email': 'arnaudmoura@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `valgrind_codequality-1.2.0/PKG-INFO` & `valgrind_codequality-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valgrind-codequality
-Version: 1.2.0
+Version: 1.2.1
 Summary: Convert Valgrind XML to GitLab Code Quality JSON file.
 License: MIT
 Author: Arnaud Moura
 Author-email: arnaudmoura@gmail.com
 Requires-Python: >=3.6.8,<=3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

