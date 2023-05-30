# Comparing `tmp/docopt-ng-0.8.1.tar.gz` & `tmp/docopt_ng-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docopt-ng-0.8.1.tar", last modified: Tue May 31 19:53:50 2022, max compression
+gzip compressed data, was "docopt_ng-0.9.0.tar", last modified: Tue May 30 20:44:03 2023, max compression
```

## Comparing `docopt-ng-0.8.1.tar` & `docopt_ng-0.9.0.tar`

### file list

```diff
@@ -1,39 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 19:53:50.979939 docopt-ng-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1086 2022-05-31 19:53:28.000000 docopt-ng-0.8.1/LICENSE-MIT
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-05-31 19:53:28.000000 docopt-ng-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    14057 2022-05-31 19:53:50.979939 docopt-ng-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13011 2022-05-31 19:53:28.000000 docopt-ng-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 19:53:50.975939 docopt-ng-0.8.1/docopt/
--rw-r--r--   0 runner    (1001) docker     (121)    34629 2022-05-31 19:53:28.000000 docopt-ng-0.8.1/docopt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-31 19:53:28.000000 docopt-ng-0.8.1/docopt/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 19:53:50.979939 docopt-ng-0.8.1/docopt_ng.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14057 2022-05-31 19:53:50.000000 docopt-ng-0.8.1/docopt_ng.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      829 2022-05-31 19:53:50.000000 docopt-ng-0.8.1/docopt_ng.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-31 19:53:50.000000 docopt-ng-0.8.1/docopt_ng.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-05-31 19:53:50.000000 docopt-ng-0.8.1/docopt_ng.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-05-31 19:53:50.000000 docopt-ng-0.8.1/docopt_ng.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 19:53:50.979939 docopt-ng-0.8.1/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-05-31 19:53:28.000000 docopt-ng-0.8.1/examples/arguments_example.py
--rw-r--r--   0 runner    (1001) docker     (121)      506 2022-05-31 19:53:28.000000 docopt-ng-0.8.1/examples/calculator_example.py
--rw-r--r--   0 runner    (1001) docker     (121)     2227 2022-05-31 19:53:28.000000 docopt-ng-0.8.1/examples/config_file_example.py
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-05-31 19:53:28.000000 docopt-ng-0.8.1/examples/counted_example.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-31 19:53:50.979939 docopt-ng-0.8.1/examples/git/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1834 2022-05-31 19:53:28.000000 docopt-ng-0.8.1/examples/git/git.py
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-05-31 19:53:28.000000 docopt-ng-0.8.1/examples/git/git_add.py
--rw-r--r--   0 runner    (1001) docker     (121)     1388 2022-05-31 19:53:28.000000 docopt-ng-0.8.1/examples/git/git_branch.py
--rw-r--r--   0 runner    (1001) docker     (121)      931 2022-05-31 19:53:28.000000 docopt-ng-0.8.1/examples/git/git_checkout.py
--rw-r--r--   0 runner    (1001) docker     (121)     1250 2022-05-31 19:53:28.000000 docopt-ng-0.8.1/examples/git/git_clone.py
--rw-r--r--   0 runner    (1001) docker     (121)     2133 2022-05-31 19:53:28.000000 docopt-ng-0.8.1/examples/git/git_commit.py
--rw-r--r--   0 runner    (1001) docker     (121)      904 2022-05-31 19:53:28.000000 docopt-ng-0.8.1/examples/git/git_push.py
--rw-r--r--   0 runner    (1001) docker     (121)      815 2022-05-31 19:53:28.000000 docopt-ng-0.8.1/examples/git/git_remote.py
--rw-r--r--   0 runner    (1001) docker     (121)     2062 2022-05-31 19:53:28.000000 docopt-ng-0.8.1/examples/interactive_example.py
--rw-r--r--   0 runner    (1001) docker     (121)      713 2022-05-31 19:53:28.000000 docopt-ng-0.8.1/examples/more_magic_example.py
--rw-r--r--   0 runner    (1001) docker     (121)      597 2022-05-31 19:53:28.000000 docopt-ng-0.8.1/examples/naval_fate.py
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-05-31 19:53:28.000000 docopt-ng-0.8.1/examples/odd_even_example.py
--rw-r--r--   0 runner    (1001) docker     (121)     1597 2022-05-31 19:53:28.000000 docopt-ng-0.8.1/examples/options_example.py
--rw-r--r--   0 runner    (1001) docker     (121)      572 2022-05-31 19:53:28.000000 docopt-ng-0.8.1/examples/options_shortcut_example.py
--rw-r--r--   0 runner    (1001) docker     (121)      313 2022-05-31 19:53:28.000000 docopt-ng-0.8.1/examples/quick_example.py
--rw-r--r--   0 runner    (1001) docker     (121)      977 2022-05-31 19:53:28.000000 docopt-ng-0.8.1/examples/validation_example.py
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-05-31 19:53:28.000000 docopt-ng-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1224 2022-05-31 19:53:50.979939 docopt-ng-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-05-31 19:53:28.000000 docopt-ng-0.8.1/setup.py
+-rw-r--r--   0        0        0     1086 2023-05-30 20:43:23.726644 docopt_ng-0.9.0/LICENSE-MIT
+-rw-r--r--   0        0        0    12802 2023-05-30 20:43:23.726644 docopt_ng-0.9.0/README.md
+-rw-r--r--   0        0        0    34333 2023-05-30 20:43:23.726644 docopt_ng-0.9.0/docopt/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-30 20:43:23.726644 docopt_ng-0.9.0/docopt/_version.py
+-rw-r--r--   0        0        0        0 2023-05-30 20:43:23.726644 docopt_ng-0.9.0/docopt/py.typed
+-rw-r--r--   0        0        0     1523 2023-05-30 20:44:03.550963 docopt_ng-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3831 2023-05-30 20:43:23.730644 docopt_ng-0.9.0/tests/conftest.py
+-rw-r--r--   0        0        0    37261 2023-05-30 20:43:23.730644 docopt_ng-0.9.0/tests/test_docopt.py
+-rw-r--r--   0        0        0     2504 2023-05-30 20:43:23.730644 docopt_ng-0.9.0/tests/test_docopt_ng.py
+-rw-r--r--   0        0        0    12933 2023-05-30 20:43:23.730644 docopt_ng-0.9.0/tests/testcases.docopt
+-rw-r--r--   0        0        0    13871 1970-01-01 00:00:00.000000 docopt_ng-0.9.0/PKG-INFO
```

### Comparing `docopt-ng-0.8.1/LICENSE-MIT` & `docopt_ng-0.9.0/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `docopt-ng-0.8.1/PKG-INFO` & `docopt_ng-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 Metadata-Version: 2.1
 Name: docopt-ng
-Version: 0.8.1
+Version: 0.9.0
 Summary: Jazzband-maintained fork of docopt, the humane command line arguments parser.
-Home-page: https://github.com/jazzband/docopt-ng
-Author: Nick Crews
-Author-email: nicholas.b.crews@gmail.com
+Author-Email: Nick Crews <nicholas.b.crews@gmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
+Project-URL: Homepage, https://github.com/jazzband/docopt-ng
+Project-URL: Repository, https://github.com/jazzband/docopt-ng
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE-MIT
 
-# **docopt-ng** creates *magic* command-line interfaces
+# **docopt-ng** creates *beautiful* command-line interfaces
 
 [![Test](https://github.com/jazzband/docopt-ng/actions/workflows/test.yml/badge.svg?event=push)](https://github.com/jazzband/docopt-ng/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/jazzband/docopt-ng/branch/master/graph/badge.svg)](https://codecov.io/gh/jazzband/docopt-ng)
 [![image](https://img.shields.io/pypi/v/docopt-ng.svg)](https://pypi.python.org/pypi/docopt-ng)
 [![Jazzband](https://jazzband.co/static/img/badge.svg)](https://jazzband.co/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-**docopt-ng** is a fork of the original docopt, maintained by the
-[jazzband](https://jazzband.co/) project.
+**docopt-ng** is a fork of the [original docopt](https://github.com/docopt/docopt), now maintained by the
+[jazzband](https://jazzband.co/) project. Now with maintenance, typehints, and complete test coverage!
 
-**docopt-ng** helps you create beautiful command-line interfaces *magically*:
+**docopt-ng** helps you create beautiful command-line interfaces:
 
 ```python
 """Naval Fate.
 
 Usage:
   naval_fate.py ship new <name>...
   naval_fate.py ship <name> move <x> <y> [--speed=<kn>]
@@ -103,30 +101,28 @@
 
 **docopt-ng** is tested with Python 3.7+.
 
 # API
 
 ```python
 def docopt(
-    docstring: str | None = None,
+    docstring: str,
     argv: list[str] | str | None = None,
     default_help: bool = True,
     version: Any = None,
     options_first: bool = False,
-    more_magic: bool = False,
 ) -> ParsedOptions:
 ```
 
-`docopt` takes 6 optional arguments:
+`docopt` takes a docstring, and 4 optional arguments:
 
--   `docstring` could be a module docstring (`__doc__`) or some other string
-    that contains a **help message** that will be parsed to create the
-    option parser. The simple rules of how to write such a help message
-    are given in next sections. If it is None (not provided), the calling scope
-    will be interrogated for a docstring.
+-   `docstring` is a string that contains a **help message** that will be
+    used to create the option parser.
+    The simple rules of how to write such a help message
+    are given in next sections. Typically you would just use `__doc__`.
 
 -   `argv` is an optional argument vector; by default `docopt` uses the
     argument vector passed to your program (`sys.argv[1:]`).
     Alternatively you can supply a list of strings like
     `["--verbose", "-o", "hai.txt"]`, or a single string that will be split
     on spaces like `"--verbose -o hai.txt"`.
 
@@ -151,22 +147,14 @@
 -   `options_first`, by default `False`. If set to `True` will disallow
     mixing options and positional argument. I.e. after first positional
     argument, all arguments will be interpreted as positional even if
     the look like options. This can be used for strict compatibility
     with POSIX, or if you want to dispatch your arguments to other
     programs.
 
--   `more_magic`, by default `False`. If set to `True` more advanced
-    efforts will be made to correct `--long_form` arguments, ie:
-    `--hlep` will be corrected to `--help`. Additionally, if not
-    already defined, the variable `arguments` will be created and populated
-    in the calling scope. `more_magic` is also set True if `docopt()` is
-    is aliased to a name containing `magic` ie) by built-in`from docopt import magic` or
-    user-defined `from docopt import docopt as magic_docopt_wrapper` for convenience.
-
 The **return** value is a simple dictionary with options, arguments and
 commands as keys, spelled exactly like in your help message. Long
 versions of options are given priority. Furthermore, dot notation is
 supported, with preceeding dashes (`-`) and surrounding brackets (`<>`)
 ignored, for example `arguments.drifting` or `arguments.x`.
 
 # Help message format
@@ -348,17 +336,24 @@
 [examples](https://github.com/jazzband/docopt-ng/tree/master/examples)
 which cover every aspect of functionality of **docopt-ng**. Try them
 out, read the source if in doubt.
 
 # Development
 
 We would *love* to hear what you think about **docopt-ng** on our
-[issues page](https://github.com/jazzband/docopt-ng/issues)
+[issues page](https://github.com/jazzband/docopt-ng/issues). Make pull requests, report bugs, and suggest ideas.
+
+To setup your dev environment, fork this repo and clone it locally.
+We use [pdm](https://pdm.fming.dev/latest/#installation) to
+manage the project, so install that first.
 
-Make pull requests, report bugs, suggest ideas and discuss
-**docopt-ng**.
+Then install dev requirements and the package itself as editable, then
+install the pre-commit hooks:
 
-## Testing
+    pdm sync -d -G dev
+    pdm run pre-commit install
 
-You can run unit tests using the command:
+Useful testing, linting, and formatting commands:
 
-    tox -v
+    pdm run pytest
+    pdm run black .
+    pdm run ruff .
```

### Comparing `docopt-ng-0.8.1/README.md` & `docopt_ng-0.9.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# **docopt-ng** creates *magic* command-line interfaces
+# **docopt-ng** creates *beautiful* command-line interfaces
 
 [![Test](https://github.com/jazzband/docopt-ng/actions/workflows/test.yml/badge.svg?event=push)](https://github.com/jazzband/docopt-ng/actions/workflows/test.yml)
 [![codecov](https://codecov.io/gh/jazzband/docopt-ng/branch/master/graph/badge.svg)](https://codecov.io/gh/jazzband/docopt-ng)
 [![image](https://img.shields.io/pypi/v/docopt-ng.svg)](https://pypi.python.org/pypi/docopt-ng)
 [![Jazzband](https://jazzband.co/static/img/badge.svg)](https://jazzband.co/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-**docopt-ng** is a fork of the original docopt, maintained by the
-[jazzband](https://jazzband.co/) project.
+**docopt-ng** is a fork of the [original docopt](https://github.com/docopt/docopt), now maintained by the
+[jazzband](https://jazzband.co/) project. Now with maintenance, typehints, and complete test coverage!
 
-**docopt-ng** helps you create beautiful command-line interfaces *magically*:
+**docopt-ng** helps you create beautiful command-line interfaces:
 
 ```python
 """Naval Fate.
 
 Usage:
   naval_fate.py ship new <name>...
   naval_fate.py ship <name> move <x> <y> [--speed=<kn>]
@@ -77,30 +77,28 @@
 
 **docopt-ng** is tested with Python 3.7+.
 
 # API
 
 ```python
 def docopt(
-    docstring: str | None = None,
+    docstring: str,
     argv: list[str] | str | None = None,
     default_help: bool = True,
     version: Any = None,
     options_first: bool = False,
-    more_magic: bool = False,
 ) -> ParsedOptions:
 ```
 
-`docopt` takes 6 optional arguments:
+`docopt` takes a docstring, and 4 optional arguments:
 
--   `docstring` could be a module docstring (`__doc__`) or some other string
-    that contains a **help message** that will be parsed to create the
-    option parser. The simple rules of how to write such a help message
-    are given in next sections. If it is None (not provided), the calling scope
-    will be interrogated for a docstring.
+-   `docstring` is a string that contains a **help message** that will be
+    used to create the option parser.
+    The simple rules of how to write such a help message
+    are given in next sections. Typically you would just use `__doc__`.
 
 -   `argv` is an optional argument vector; by default `docopt` uses the
     argument vector passed to your program (`sys.argv[1:]`).
     Alternatively you can supply a list of strings like
     `["--verbose", "-o", "hai.txt"]`, or a single string that will be split
     on spaces like `"--verbose -o hai.txt"`.
 
@@ -125,22 +123,14 @@
 -   `options_first`, by default `False`. If set to `True` will disallow
     mixing options and positional argument. I.e. after first positional
     argument, all arguments will be interpreted as positional even if
     the look like options. This can be used for strict compatibility
     with POSIX, or if you want to dispatch your arguments to other
     programs.
 
--   `more_magic`, by default `False`. If set to `True` more advanced
-    efforts will be made to correct `--long_form` arguments, ie:
-    `--hlep` will be corrected to `--help`. Additionally, if not
-    already defined, the variable `arguments` will be created and populated
-    in the calling scope. `more_magic` is also set True if `docopt()` is
-    is aliased to a name containing `magic` ie) by built-in`from docopt import magic` or
-    user-defined `from docopt import docopt as magic_docopt_wrapper` for convenience.
-
 The **return** value is a simple dictionary with options, arguments and
 commands as keys, spelled exactly like in your help message. Long
 versions of options are given priority. Furthermore, dot notation is
 supported, with preceeding dashes (`-`) and surrounding brackets (`<>`)
 ignored, for example `arguments.drifting` or `arguments.x`.
 
 # Help message format
@@ -322,17 +312,24 @@
 [examples](https://github.com/jazzband/docopt-ng/tree/master/examples)
 which cover every aspect of functionality of **docopt-ng**. Try them
 out, read the source if in doubt.
 
 # Development
 
 We would *love* to hear what you think about **docopt-ng** on our
-[issues page](https://github.com/jazzband/docopt-ng/issues)
+[issues page](https://github.com/jazzband/docopt-ng/issues). Make pull requests, report bugs, and suggest ideas.
+
+To setup your dev environment, fork this repo and clone it locally.
+We use [pdm](https://pdm.fming.dev/latest/#installation) to
+manage the project, so install that first.
 
-Make pull requests, report bugs, suggest ideas and discuss
-**docopt-ng**.
+Then install dev requirements and the package itself as editable, then
+install the pre-commit hooks:
 
-## Testing
+    pdm sync -d -G dev
+    pdm run pre-commit install
 
-You can run unit tests using the command:
+Useful testing, linting, and formatting commands:
 
-    tox -v
+    pdm run pytest
+    pdm run black .
+    pdm run ruff .
```

### Comparing `docopt-ng-0.8.1/docopt/__init__.py` & `docopt_ng-0.9.0/docopt/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,22 +19,27 @@
  * Copyright (c) 2017 Oleg Bulkin <o.bulkin@gmail.com>
  * Copyright (c) 2018 Iain Barnett <iainspeed@gmail.com>
  * Copyright (c) 2019 itdaniher, itdaniher@gmail.com
 
 """
 from __future__ import annotations
 
-import sys
 import re
-import inspect
+import sys
+from typing import Any
+from typing import Callable
+from typing import NamedTuple
+from typing import Tuple
+from typing import Type
+from typing import Union
+from typing import cast
 
-from typing import Any, Callable, cast, Type, Tuple, Union
+from ._version import __version__ as __version__
 
-__all__ = ["docopt", "magic_docopt", "magic", "DocoptExit"]
-__version__ = "0.8.1"
+__all__ = ["docopt", "DocoptExit"]
 
 
 def levenshtein_norm(source: str, target: str) -> float:
     """Calculates the normalized Levenshtein distance between two string
     arguments. The result will be a float in the range [0.0, 1.0], with 1.0
     signifying the biggest possible distance between strings with these lengths
     """
@@ -109,16 +114,16 @@
     """Exit in case user invoked program with incorrect arguments."""
 
     usage = ""
 
     def __init__(
         self,
         message: str = "",
-        collected: list[Pattern] = None,
-        left: list[Pattern] = None,
+        collected: list[Pattern] | None = None,
+        left: list[Pattern] | None = None,
     ) -> None:
         self.collected = collected if collected is not None else []
         self.left = left if left is not None else []
         SystemExit.__init__(self, (message + "\n" + self.usage).strip())
 
 
 class Pattern:
@@ -178,15 +183,15 @@
     def single_match(self, left: list[LeafPattern]) -> TSingleMatch:
         raise NotImplementedError  # pragma: no cover
 
     def flat(self, *types) -> list[LeafPattern]:
         return [self] if not types or type(self) in types else []
 
     def match(
-        self, left: list[LeafPattern], collected: list[Pattern] = None
+        self, left: list[LeafPattern], collected: list[Pattern] | None = None
     ) -> tuple[bool, list[LeafPattern], list[Pattern]]:
         collected = [] if collected is None else collected
         increment: Any | None = None
         pos, match = self.single_match(left)
         if match is None or pos is None:
             return False, left, collected
         left_ = left[:pos] + left[(pos + 1) :]
@@ -215,15 +220,15 @@
 class BranchPattern(Pattern):
 
     """Branch/inner node of a pattern tree."""
 
     def __init__(self, *children) -> None:
         self.children = list(children)
 
-    def match(self, left: list[Pattern], collected: list[Pattern] = None) -> Any:
+    def match(self, left: list[Pattern], collected: list[Pattern] | None = None) -> Any:
         raise NotImplementedError  # pragma: no cover
 
     def fix(self) -> "BranchPattern":
         self.fix_identities()
         self.fix_repeating_arguments()
         return self
 
@@ -299,15 +304,17 @@
         assert argcount in (0, 1)
         self.short, self.longer, self.argcount = short, longer, argcount
         self.value = None if value is False and argcount else value
 
     @classmethod
     def parse(class_, option_description: str) -> Option:
         short, longer, argcount, value = None, None, 0, False
-        options, _, description = option_description.strip().partition("  ")
+        options, description = re.split(
+            r"(?:  )|$", option_description.strip(), flags=re.M, maxsplit=1
+        )
         options = options.replace(",", " ").replace("=", " ")
         for s in options.split():
             if s.startswith("--"):
                 longer = s
             elif s.startswith("-"):
                 short = s
             else:
@@ -345,28 +352,28 @@
             matched, left, collected = pattern.match(left, collected)
             if not matched:
                 return False, original_left, original_collected
         return True, left, collected
 
 
 class NotRequired(BranchPattern):
-    def match(self, left: list[Pattern], collected: list[Pattern] = None) -> Any:
+    def match(self, left: list[Pattern], collected: list[Pattern] | None = None) -> Any:
         collected = [] if collected is None else collected
         for pattern in self.children:
             _, left, collected = pattern.match(left, collected)
         return True, left, collected
 
 
 class OptionsShortcut(NotRequired):
 
     """Marker/placeholder for [options] shortcut."""
 
 
 class OneOrMore(BranchPattern):
-    def match(self, left: list[Pattern], collected: list[Pattern] = None) -> Any:
+    def match(self, left: list[Pattern], collected: list[Pattern] | None = None) -> Any:
         assert len(self.children) == 1
         collected = [] if collected is None else collected
         original_collected = collected
         original_left = left
         last_left = None
         matched = True
         times = 0
@@ -378,15 +385,15 @@
             last_left = left
         if times >= 1:
             return True, left, collected
         return False, original_left, original_collected
 
 
 class Either(BranchPattern):
-    def match(self, left: list[Pattern], collected: list[Pattern] = None) -> Any:
+    def match(self, left: list[Pattern], collected: list[Pattern] | None = None) -> Any:
         collected = [] if collected is None else collected
         outcomes = []
         for pattern in self.children:
             matched, _, _ = outcome = pattern.match(left, collected)
             if matched:
                 outcomes.append(outcome)
         if outcomes:
@@ -421,17 +428,17 @@
 
 def parse_longer(
     tokens: Tokens, options: list[Option], argv: bool = False, more_magic: bool = False
 ) -> list[Pattern]:
     """longer ::= '--' chars [ ( ' ' | '=' ) chars ] ;"""
     current_token = tokens.move()
     if current_token is None or not current_token.startswith("--"):
-        raise tokens.error(
+        raise ValueError(
             f"parse_longer got what appears to be an invalid token: {current_token}"
-        )  # pragma: no cover
+        )
     longer, maybe_eq, maybe_value = current_token.partition("=")
     if maybe_eq == maybe_value == "":
         value = None
     else:
         value = maybe_value
     similar = [o for o in options if o.longer and longer == o.longer]
     start_collision = (
@@ -457,17 +464,15 @@
             for o in options
             if o.longer and levenshtein_norm(longer, o.longer) < 0.25
         ]
         if corrected:
             print(f"NB: Corrected {corrected[0][0]} to {corrected[0][1].longer}")
         similar = [correct for (original, correct) in corrected]
     if len(similar) > 1:
-        raise tokens.error(
-            f"{longer} is not a unique prefix: {similar}?"
-        )  # pragma: no cover
+        raise DocoptLanguageError(f"{longer} is not a unique prefix: {similar}?")
     elif len(similar) < 1:
         argcount = 1 if maybe_eq == "=" else 0
         o = Option(None, longer, argcount)
         options.append(o)
         if tokens.error is DocoptExit:
             o = Option(None, longer, argcount, value if argcount else True)
     else:
@@ -491,15 +496,15 @@
     tokens: Tokens, options: list[Option], more_magic: bool = False
 ) -> list[Pattern]:
     """shorts ::= '-' ( chars )* [ [ ' ' ] chars ] ;"""
     token = tokens.move()
     if token is None or not token.startswith("-") or token.startswith("--"):
         raise ValueError(
             f"parse_shorts got what appears to be an invalid token: {token}"
-        )  # pragma: no cover
+        )
     left = token.lstrip("-")
     parsed: list[Pattern] = []
     while left != "":
         short, left = "-" + left[0], left[1:]
         transformations: dict[str | None, Callable[[str], str]] = {None: lambda x: x}
         if more_magic:
             transformations["lowercase"] = lambda x: x.lower()
@@ -558,16 +563,16 @@
                                 f"via abbreviation (case change: {transform_name})"
                             )
                             break
                 if len(similar):
                     de_abbreviated = True
                     break
         if len(similar) > 1:
-            raise tokens.error(
-                "%s is specified ambiguously %d times" % (short, len(similar))
+            raise DocoptLanguageError(
+                f"{short} is specified ambiguously {len(similar)} times"
             )
         elif len(similar) < 1:
             o = Option(short, None, 0)
             options.append(o)
             if tokens.error is DocoptExit:
                 o = Option(short, None, 0, True)
         else:
@@ -705,47 +710,109 @@
             return parsed + [Argument(None, v) for v in tokens]
         else:
             parsed.append(Argument(None, tokens.move()))
         current_token = tokens.current()
     return parsed
 
 
-def parse_defaults(docstring: str) -> list[Option]:
-    defaults = []
-    for s in parse_section("options:", docstring):
-        options_literal, _, s = s.partition(":")
-        if " " in options_literal:
-            _, _, options_literal = options_literal.partition(" ")
-        assert options_literal.lower().strip() == "options"
-        split = re.split(r"\n[ \t]*(-\S+?)", "\n" + s)[1:]
-        split = [s1 + s2 for s1, s2 in zip(split[::2], split[1::2])]
-        for s in split:
-            if s.startswith("-"):
-                arg, _, description = s.partition("  ")
-                flag, _, var = arg.replace("=", " ").partition(" ")
-                option = Option.parse(s)
-                defaults.append(option)
-    return defaults
-
-
-def parse_section(name: str, source: str) -> list[str]:
-    pattern = re.compile(
-        "^([^\n]*" + name + "[^\n]*\n?(?:[ \t].*?(?:\n|$))*)",
-        re.IGNORECASE | re.MULTILINE,
+class DocSections(NamedTuple):
+    before_usage: str
+    usage_header: str
+    usage_body: str
+    after_usage: str
+
+
+def parse_docstring_sections(docstring: str) -> DocSections:
+    """Partition the docstring into the main sections.
+
+    The docstring is returned, split into a tuple of 4 pieces: text before the
+    usage section, the usage section header, the usage section body and text
+    following the usage section.
+    """
+    usage_pattern = r"""
+    # Any number of lines (that don't include usage:) precede the usage section
+    \A(?P<before_usage>(?:(?!.*\busage:).*\n)*)
+    # The `usage:` section header.
+    ^(?P<usage_header>.*\busage:)
+    (?P<usage_body>
+        # The first line of the body may follow the header without a line break:
+        (?:.*(?:\n|\Z))
+        # Any number of additional indented lines
+        (?:[ \t].*(?:\n|\Z))*
     )
-    r = [
-        s.strip() for s in pattern.findall(source) if s.strip().lower() != name.lower()
+    # Everything else
+    (?P<after_usage>(?:.|\n)*)\Z
+    """
+    match = re.match(usage_pattern, docstring, flags=re.M | re.I | re.VERBOSE)
+    if not match:
+        raise DocoptLanguageError(
+            'Failed to parse doc: "usage:" section (case-insensitive) not found. '
+            "Check http://docopt.org/ for examples of how your doc should look."
+        )
+    before, header, body, after = match.groups()
+    return DocSections(before, header, body, after)
+
+
+def parse_options(docstring: str) -> list[Option]:
+    """Parse the option descriptions from the help text.
+
+    `docstring` is the sub-section of the overall docstring that option
+    descriptions should be parsed from. It must not contain the "usage:"
+    section, as wrapped lines in the usage pattern can be misinterpreted as
+    option descriptions.
+
+    Option descriptions appear below the usage patterns, They define synonymous
+    long and short options, options that have arguments, and the default values
+    of options' arguments. They look like this:
+
+    ```
+        -v, --verbose             Be more verbose
+        -n COUNT, --number COUNT  The number of times to
+                                do the thing  [default: 42]
+    ```
+    """
+    option_start = r"""
+    # Option descriptions begin on a new line
+    ^
+    # They may occur on the same line as an options: section heading
+    (?:.*options:)?
+    # They can be indented with whitespace
+    [ \t]*
+    # The description itself starts with the short or long flag (-x or --xxx)
+    (-\S)
+    """
+    parts = re.split(option_start, docstring, flags=re.M | re.I | re.VERBOSE)[1:]
+    return [
+        Option.parse(start + rest) for (start, rest) in zip(parts[0::2], parts[1::2])
     ]
-    return r
 
 
-def formal_usage(section: str) -> str:
-    _, _, section = section.partition(":")  # drop "usage:"
-    pu = section.split()
-    return "( " + " ".join(") | (" if s == pu[0] else s for s in pu[1:]) + " )"
+def lint_docstring(sections: DocSections):
+    """Report apparent mistakes in the docstring format."""
+    if re.search("options:", sections.usage_body, flags=re.I):
+        raise DocoptLanguageError(
+            'Failed to parse docstring: "options:" (case-insensitive) was '
+            'found in "usage:" section. Use a blank line after the usage, or '
+            "start the next section without leading whitespace."
+        )
+    if re.search("usage:", sections.usage_body + sections.after_usage, flags=re.I):
+        raise DocoptLanguageError(
+            'Failed to parse docstring: More than one "usage:" '
+            "(case-insensitive) section found."
+        )
+    if sections.usage_body.strip() == "":
+        raise DocoptLanguageError(
+            'Failed to parse docstring: "usage:" section is empty.'
+            "Check http://docopt.org/ for examples of how your doc should look."
+        )
+
+
+def formal_usage(usage: str) -> str:
+    program_name, *tokens = usage.split()
+    return "( " + " ".join(") | (" if s == program_name else s for s in tokens) + " )"
 
 
 def extras(
     default_help: bool, version: None, options: list[Pattern], docstring: str
 ) -> None:
     if default_help and any(
         (o.name in ("-h", "--help")) and o.value
@@ -770,55 +837,50 @@
             name: self.get(k)
             for k in self.keys()
             if name in [k.lstrip("-").replace("-", "_"), k.lstrip("<").rstrip(">")]
         }.get(name)
 
 
 def docopt(
-    docstring: str | None = None,
+    docstring: str,
     argv: list[str] | str | None = None,
     default_help: bool = True,
     version: Any = None,
     options_first: bool = False,
-    more_magic: bool = False,
 ) -> ParsedOptions:
-    """Parse `argv` based on command-line interface described in `doc`.
+    """Parse `argv` based on command-line interface described in `docstring`.
 
     `docopt` creates your command-line interface based on its
     description that you pass as `docstring`. Such description can contain
     --options, <positional-argument>, commands, which could be
     [optional], (required), (mutually | exclusive) or repeated...
 
     Parameters
     ----------
-    docstring : str (default: first __doc__ in parent scope)
+    docstring : str
         Description of your command-line interface.
-    argv : list of str, optional
+    argv : list of str or str, optional
         Argument vector to be parsed. sys.argv[1:] is used if not
-        provided.
+        provided. If str is passed, the string is split on whitespace.
     default_help : bool (default: True)
         Set to False to disable automatic help on -h or --help
         options.
     version : any object
         If passed, the object will be printed if --version is in
         `argv`.
     options_first : bool (default: False)
         Set to True to require options precede positional arguments,
         i.e. to forbid options and positional arguments intermix.
-    more_magic : bool (default: False)
-        Try to be extra-helpful; pull results into globals() of caller as 'arguments',
-        offer advanced pattern-matching and spellcheck.
-        Also activates if `docopt` aliased to a name containing 'magic'.
 
     Returns
     -------
     arguments: dict-like
         A dictionary, where keys are names of command-line elements
         such as e.g. "--verbose" and "<path>", and values are the
-        parsed values of those elements. Also supports dot acccess.
+        parsed values of those elements. Also supports dot access.
 
     Example
     -------
     >>> from docopt import docopt
     >>> doc = '''
     ... Usage:
     ...     my_program tcp <host> <port> [--timeout=<seconds>]
@@ -835,92 +897,30 @@
      '--help': False,
      '--timeout': '30',
      '--version': False,
      '<host>': '127.0.0.1',
      '<port>': '80',
      'serial': False,
      'tcp': True}
-
     """
     argv = sys.argv[1:] if argv is None else argv
-    maybe_frame = inspect.currentframe()
-    if maybe_frame:
-        parent_frame = doc_parent_frame = magic_parent_frame = maybe_frame.f_back
-    if not more_magic:  # make sure 'magic' isn't in the calling name
-        while not more_magic and magic_parent_frame:
-            imported_as = {
-                v: k
-                for k, v in magic_parent_frame.f_globals.items()
-                if hasattr(v, "__name__") and v.__name__ == docopt.__name__
-            }.get(docopt)
-            if imported_as and "magic" in imported_as:
-                more_magic = True
-            else:
-                magic_parent_frame = magic_parent_frame.f_back
-    if not docstring:  # go look for one, if none exists, raise Exception
-        while not docstring and doc_parent_frame:
-            docstring = doc_parent_frame.f_locals.get("__doc__")
-            if not docstring:
-                doc_parent_frame = doc_parent_frame.f_back
-        if not docstring:
-            raise DocoptLanguageError(
-                "Either __doc__ must be defined in the scope of a parent "
-                "or passed as the first argument."
-            )
-    output_value_assigned = False
-    if more_magic and parent_frame:
-        import dis
-
-        instrs = dis.get_instructions(parent_frame.f_code)
-        for instr in instrs:
-            if instr.offset == parent_frame.f_lasti:
-                break
-        assert instr.opname.startswith("CALL_")
-        MAYBE_STORE = next(instrs)
-        if MAYBE_STORE and (
-            MAYBE_STORE.opname.startswith("STORE")
-            or MAYBE_STORE.opname.startswith("RETURN")
-        ):
-            output_value_assigned = True
-    usage_sections = parse_section("usage:", docstring)
-    if len(usage_sections) == 0:
-        raise DocoptLanguageError(
-            '"usage:" section (case-insensitive) not found. '
-            "Perhaps missing indentation?"
-        )
-    if len(usage_sections) > 1:
-        raise DocoptLanguageError('More than one "usage:" (case-insensitive).')
-    options_pattern = re.compile(r"\n\s*?options:", re.IGNORECASE)
-    if options_pattern.search(usage_sections[0]):
-        raise DocoptExit(
-            "Warning: options (case-insensitive) was found in usage."
-            "Use a blank line between each section.."
-        )
-    DocoptExit.usage = usage_sections[0]
-    options = parse_defaults(docstring)
-    pattern = parse_pattern(formal_usage(DocoptExit.usage), options)
+    sections = parse_docstring_sections(docstring)
+    lint_docstring(sections)
+    DocoptExit.usage = sections.usage_header + sections.usage_body
+    options = [
+        *parse_options(sections.before_usage),
+        *parse_options(sections.after_usage),
+    ]
+    pattern = parse_pattern(formal_usage(sections.usage_body), options)
     pattern_options = set(pattern.flat(Option))
     for options_shortcut in pattern.flat(OptionsShortcut):
-        doc_options = parse_defaults(docstring)
         options_shortcut.children = [
-            opt for opt in doc_options if opt not in pattern_options
+            opt for opt in options if opt not in pattern_options
         ]
-    parsed_arg_vector = parse_argv(
-        Tokens(argv), list(options), options_first, more_magic
-    )
+    parsed_arg_vector = parse_argv(Tokens(argv), list(options), options_first)
     extras(default_help, version, parsed_arg_vector, docstring)
     matched, left, collected = pattern.fix().match(parsed_arg_vector)
     if matched and left == []:
-        output_obj = ParsedOptions(
-            (a.name, a.value) for a in (pattern.flat() + collected)
-        )
-        target_parent_frame = parent_frame or magic_parent_frame or doc_parent_frame
-        if more_magic and target_parent_frame and not output_value_assigned:
-            if not target_parent_frame.f_globals.get("arguments"):
-                target_parent_frame.f_globals["arguments"] = output_obj
-        return output_obj
+        return ParsedOptions((a.name, a.value) for a in (pattern.flat() + collected))
     if left:
         raise DocoptExit(f"Warning: found unmatched (duplicate?) arguments {left}")
     raise DocoptExit(collected=collected, left=left)
-
-
-magic = magic_docopt = docopt
```

### Comparing `docopt-ng-0.8.1/setup.cfg` & `docopt_ng-0.9.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,55 +1,69 @@
-[metadata]
-name = docopt-ng
-version = attr: docopt.__version__
-url = https://github.com/jazzband/docopt-ng
-license = MIT
-author = Nick Crews
-author_email = nicholas.b.crews@gmail.com
-description = Jazzband-maintained fork of docopt, the humane command line arguments parser.
-long_description = file: README.md
-long_description_content_type = text/markdown
-classifiers = 
-	Development Status :: 4 - Beta
-	Intended Audience :: Developers
-	License :: OSI Approved :: MIT License
-	Operating System :: OS Independent
-	Programming Language :: Python
-	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
-	Programming Language :: Python :: 3.9
-	Programming Language :: Python :: 3.10
-	Programming Language :: Python :: Implementation :: CPython
-	Programming Language :: Python :: Implementation :: PyPy
-
-[options]
-python_requires = >=3.7
-packages = find:
-
-[options.package_data]
-* = py.typed
-
-[options.extras_require]
-dev = 
-	black
-	build
-	flake8
-	mypy
-	pre-commit
-	pytest
-	pytest-mypy
-	pytest-cov
-	twine
-
-[bdist_wheel]
-universal = 1
-
-[flake8]
-max-line-length = 88
-extend-ignore = E203
-
-[egg_info]
-tag_build = 
-tag_date = 0
+[build-system]
+requires = [
+    "pdm-backend",
+]
+build-backend = "pdm.backend"
+
+[project]
+name = "docopt-ng"
+dynamic = []
+description = "Jazzband-maintained fork of docopt, the humane command line arguments parser."
+authors = [
+    { name = "Nick Crews", email = "nicholas.b.crews@gmail.com" },
+]
+dependencies = []
+requires-python = ">=3.7"
+readme = "README.md"
+classifiers = [
+    "Development Status :: 4 - Beta",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: Implementation :: CPython",
+    "Programming Language :: Python :: Implementation :: PyPy",
+]
+version = "0.9.0"
+
+[project.license]
+text = "MIT"
+
+[project.urls]
+Homepage = "https://github.com/jazzband/docopt-ng"
+Repository = "https://github.com/jazzband/docopt-ng"
+
+[tool.pdm.version]
+source = "file"
+path = "docopt/_version.py"
+
+[tool.pdm.dev-dependencies]
+dev = [
+    "black",
+    "mypy",
+    "ruff",
+    "pre-commit",
+    "pytest",
+    "pytest-cov",
+    "pytest-mypy",
+]
+
+[tool.pytest.ini_options]
+testpaths = [
+    "./tests",
+]
+
+[tool.ruff]
+select = [
+    "E",
+    "F",
+    "I",
+]
 
+[tool.ruff.isort]
+force-single-line = true
```

