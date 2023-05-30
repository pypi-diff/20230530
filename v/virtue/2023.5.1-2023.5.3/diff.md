# Comparing `tmp/virtue-2023.5.1.tar.gz` & `tmp/virtue-2023.5.3.tar.gz`

## Comparing `virtue-2023.5.1.tar` & `virtue-2023.5.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 virtue-2023.5.1/.coveragerc
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 virtue-2023.5.1/.flake8
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 virtue-2023.5.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 virtue-2023.5.1/.readthedocs.yml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 virtue-2023.5.1/.testr.conf
--rw-r--r--   0        0        0     2691 2020-02-02 00:00:00.000000 virtue-2023.5.1/noxfile.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 virtue-2023.5.1/.github/FUNDING.yml
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 virtue-2023.5.1/.github/SECURITY.md
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 virtue-2023.5.1/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 virtue-2023.5.1/.github/release.yml
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 virtue-2023.5.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 virtue-2023.5.1/docs/Makefile
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 virtue-2023.5.1/docs/api.rst
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 virtue-2023.5.1/docs/conf.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 virtue-2023.5.1/docs/index.rst
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 virtue-2023.5.1/docs/requirements.in
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 virtue-2023.5.1/docs/requirements.txt
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 virtue-2023.5.1/docs/spelling-wordlist.txt
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 virtue-2023.5.1/virtue/__init__.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 virtue-2023.5.1/virtue/__main__.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 virtue-2023.5.1/virtue/_cli.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 virtue-2023.5.1/virtue/loaders.py
--rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 virtue-2023.5.1/virtue/locators.py
--rw-r--r--   0        0        0    13544 2020-02-02 00:00:00.000000 virtue-2023.5.1/virtue/reporters.py
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 virtue-2023.5.1/virtue/runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 virtue-2023.5.1/virtue/tests/__init__.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 virtue-2023.5.1/virtue/tests/test_cli.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 virtue-2023.5.1/virtue/tests/test_loaders.py
--rw-r--r--   0        0        0     7246 2020-02-02 00:00:00.000000 virtue-2023.5.1/virtue/tests/test_locators.py
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 virtue-2023.5.1/virtue/tests/test_reporters.py
--rw-r--r--   0        0        0    12351 2020-02-02 00:00:00.000000 virtue-2023.5.1/virtue/tests/test_runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 virtue-2023.5.1/virtue/tests/samples/__init__.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 virtue-2023.5.1/virtue/tests/samples/dynamic_test.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 virtue-2023.5.1/virtue/tests/samples/failures_and_errors.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 virtue-2023.5.1/virtue/tests/samples/failures_and_unexpected_passes.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 virtue-2023.5.1/virtue/tests/samples/mixin.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 virtue-2023.5.1/virtue/tests/samples/module_for_TestLoaders.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 virtue-2023.5.1/virtue/tests/samples/module_for_TestObjectLocator.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 virtue-2023.5.1/virtue/tests/samples/module_with_exception.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 virtue-2023.5.1/virtue/tests/samples/no_tests.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 virtue-2023.5.1/virtue/tests/samples/one_expected_failure.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 virtue-2023.5.1/virtue/tests/samples/one_expected_failure_mispassing.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 virtue-2023.5.1/virtue/tests/samples/one_successful_test.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 virtue-2023.5.1/virtue/tests/samples/one_unsuccessful_test.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 virtue-2023.5.1/virtue/tests/samples/repeated_similar_output.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 virtue-2023.5.1/virtue/tests/samples/subtests.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 virtue-2023.5.1/virtue/tests/samples/success_and_warning.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 virtue-2023.5.1/virtue/tests/samples/two_unsuccessful_tests.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 virtue-2023.5.1/COPYING
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 virtue-2023.5.1/README.rst
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 virtue-2023.5.1/pyproject.toml
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 virtue-2023.5.1/PKG-INFO
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 virtue-2023.5.3/.coveragerc
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 virtue-2023.5.3/.flake8
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 virtue-2023.5.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 virtue-2023.5.3/.readthedocs.yml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 virtue-2023.5.3/.testr.conf
+-rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 virtue-2023.5.3/noxfile.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 virtue-2023.5.3/.github/FUNDING.yml
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 virtue-2023.5.3/.github/SECURITY.md
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 virtue-2023.5.3/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 virtue-2023.5.3/.github/release.yml
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 virtue-2023.5.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 virtue-2023.5.3/docs/Makefile
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 virtue-2023.5.3/docs/api.rst
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 virtue-2023.5.3/docs/conf.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 virtue-2023.5.3/docs/index.rst
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 virtue-2023.5.3/docs/requirements.in
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 virtue-2023.5.3/docs/requirements.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 virtue-2023.5.3/docs/spelling-wordlist.txt
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/__init__.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/__main__.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/_cli.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/loaders.py
+-rw-r--r--   0        0        0     6129 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/locators.py
+-rw-r--r--   0        0        0    15025 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/reporters.py
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/__init__.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/test_cli.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/test_loaders.py
+-rw-r--r--   0        0        0     7246 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/test_locators.py
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/test_reporters.py
+-rw-r--r--   0        0        0    12351 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/test_runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/samples/__init__.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/samples/dynamic_test.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/samples/failures_and_errors.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/samples/failures_and_unexpected_passes.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/samples/mixin.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/samples/module_for_TestLoaders.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/samples/module_for_TestObjectLocator.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/samples/module_with_exception.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/samples/no_tests.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/samples/one_expected_failure.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/samples/one_expected_failure_mispassing.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/samples/one_successful_test.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/samples/one_unsuccessful_test.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/samples/repeated_similar_output.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/samples/subtests.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/samples/success_and_warning.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 virtue-2023.5.3/virtue/tests/samples/two_unsuccessful_tests.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 virtue-2023.5.3/COPYING
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 virtue-2023.5.3/README.rst
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 virtue-2023.5.3/pyproject.toml
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 virtue-2023.5.3/PKG-INFO
```

### Comparing `virtue-2023.5.1/.flake8` & `virtue-2023.5.3/.flake8`

 * *Files identical despite different names*

### Comparing `virtue-2023.5.1/.pre-commit-config.yaml` & `virtue-2023.5.3/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -7,26 +7,22 @@
       - id: check-vcs-permalinks
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
         args: [--fix, lf]
       - id: trailing-whitespace
+  - repo: https://github.com/charliermarsh/ruff-pre-commit
+    rev: "v0.0.270"
+    hooks:
+      - id: ruff
   - repo: https://github.com/PyCQA/isort
     rev: 5.12.0
     hooks:
       - id: isort
-  - repo: https://github.com/pycqa/flake8
-    rev: "6.0.0"
-    hooks:
-      - id: flake8
-  - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.2
-    hooks:
-      - id: pyupgrade
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - name: black
         id: black
         args: ["--line-length", "79"]
   - repo: https://github.com/pre-commit/mirrors-prettier
```

### Comparing `virtue-2023.5.1/noxfile.py` & `virtue-2023.5.3/noxfile.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from pathlib import Path
+import os
 
 import nox
 
 ROOT = Path(__file__).parent
 PYPROJECT = ROOT / "pyproject.toml"
 DOCS = ROOT / "docs"
 PACKAGE = ROOT / "virtue"
@@ -19,18 +20,36 @@
 
     return _session
 
 
 @session(python=["3.7", "3.8", "3.9", "3.10", "3.11", "pypy3"])
 def tests(session):
     session.install(ROOT)
-    if session.posargs == ["coverage"]:
+    if session.posargs and session.posargs[0] == "coverage":
+        if len(session.posargs) > 1 and session.posargs[1] == "github":
+            posargs = session.posargs[2:]
+            github = os.environ["GITHUB_STEP_SUMMARY"]
+        else:
+            posargs, github = session.posargs[1:], None
+
         session.install("coverage[toml]")
-        session.run("coverage", "run", "-m", "virtue", "virtue")
-        session.run("coverage", "report")
+        session.run("coverage", "run", *posargs, "-m", "virtue", PACKAGE)
+
+        if github is None:
+            session.run("coverage", "report")
+        else:
+            with open(github, "a") as summary:
+                summary.write("### Coverage\n\n")
+                summary.flush()  # without a flush, output seems out of order.
+                session.run(
+                    "coverage",
+                    "report",
+                    "--format=markdown",
+                    stdout=summary,
+                )
     else:
         session.run("virtue", *session.posargs, "virtue")
 
 
 @session(python=["3.7", "3.8", "3.9", "3.10", "3.11", "pypy3"])
 def audit(session):
     session.install("pip_audit", ROOT)
@@ -45,34 +64,32 @@
 
 
 @session(tags=["style"])
 def readme(session):
     session.install("build", "twine")
     tmpdir = session.create_tmp()
     session.run("python", "-m", "build", ROOT, "--outdir", tmpdir)
-    session.run("python", "-m", "twine", "check", tmpdir + "/*")
+    session.run("python", "-m", "twine", "check", "--strict", tmpdir + "/*")
+
+
+@session()
+def secrets(session):
+    session.install("detect-secrets")
+    session.run("detect-secrets", "scan", ROOT)
 
 
 @session(tags=["style"])
 def style(session):
-    session.install(
-        "flake8",
-        "flake8-broken-line",
-        "flake8-bugbear",
-        "flake8-commas",
-        "flake8-docstrings",
-        "flake8-quotes",
-        "flake8-tidy-imports",
-    )
-    session.run("python", "-m", "flake8", PACKAGE, DOCS, __file__)
+    session.install("ruff")
+    session.run("ruff", "check", ROOT)
 
 
 @session()
 def typing(session):
-    session.install("mypy", ROOT, "types-colorama")
+    session.install("mypy", "types-colorama", ROOT)
     session.run("mypy", "--config", PYPROJECT, PACKAGE)
 
 
 @session(tags=["docs"])
 @nox.parametrize(
     "builder",
     [
@@ -108,7 +125,13 @@
 def docs_style(session):
     session.install(
         "doc8",
         "pygments",
         "pygments-github-lexers",
     )
     session.run("python", "-m", "doc8", "--config", PYPROJECT, DOCS)
+
+
+@session(default=False)
+def bandit(session):
+    session.install("bandit")
+    session.run("bandit", "--recursive", PACKAGE)
```

### Comparing `virtue-2023.5.1/.github/SECURITY.md` & `virtue-2023.5.3/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `virtue-2023.5.1/.github/workflows/ci.yml` & `virtue-2023.5.3/.github/workflows/ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -44,31 +44,36 @@
     needs: list
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [macos-latest, ubuntu-latest]
         noxenv: ${{ fromJson(needs.list.outputs.noxenvs) }}
+        posargs: [""]
+        include:
+          - os: ubuntu-latest
+            noxenv: tests-3.11
+            posargs: coverage github
 
     steps:
       - uses: actions/checkout@v3
       - name: Install dependencies
-        run: sudo apt-get install -y libenchant-2-dev
+        run: sudo apt-get update && sudo apt-get install -y libenchant-2-dev
         if: runner.os == 'Linux' && startsWith(matrix.noxenv, 'docs')
       - name: Install dependencies
         run: brew install enchant
         if: runner.os == 'macOS' && startsWith(matrix.noxenv, 'docs')
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: "3.x"
       - name: Set up nox
         uses: wntrblm/nox@2023.04.22
       - name: Run nox
-        run: nox -s "${{ matrix.noxenv }}"
+        run: nox -s "${{ matrix.noxenv }}" -- ${{ matrix.posargs }}
 
   packaging:
     needs: ci
     runs-on: ubuntu-latest
     environment:
       name: PyPI
       url: https://pypi.org/p/virtue
```

### Comparing `virtue-2023.5.1/docs/Makefile` & `virtue-2023.5.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `virtue-2023.5.1/docs/conf.py` & `virtue-2023.5.3/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import importlib.metadata
 import re
 
 project = "Virtue"
 author = "Julian Berman"
-copyright = "2014, " + author
+copyright = f"2014, {author}"
 
 release = importlib.metadata.version("virtue")
 version = release.partition("-")[0]
 
 language = "en"
 default_role = "any"
 
@@ -15,30 +15,24 @@
     "sphinx.ext.autodoc",
     "sphinx.ext.autosectionlabel",
     "sphinx.ext.coverage",
     "sphinx.ext.doctest",
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
     "sphinx.ext.viewcode",
+    "sphinx_copybutton",
     "sphinxcontrib.spelling",
+    "sphinxext.opengraph",
 ]
 
 pygments_style = "lovelace"
 pygments_dark_style = "one-dark"
 
 html_theme = "furo"
 
-# = Builders =
-
-nitpick_ignore = [
-    # Missing from pyrsistent docs
-    ("py:class", "pyrsistent.typing.PMap"),
-    ("py:class", "pyrsistent.typing.PVector"),
-]
-
 
 def entire_domain(host):
     return r"http.?://" + re.escape(host) + r"($|/.*)"
 
 
 linkcheck_ignore = [
     entire_domain("img.shields.io"),
```

### Comparing `virtue-2023.5.1/virtue/_cli.py` & `virtue-2023.5.3/virtue/_cli.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.5.1/virtue/loaders.py` & `virtue-2023.5.3/virtue/loaders.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.5.1/virtue/locators.py` & `virtue-2023.5.3/virtue/locators.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.5.1/virtue/reporters.py` & `virtue-2023.5.3/virtue/reporters.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,14 +28,18 @@
         yield self.status
         yield "\n"
         if self.body:
             yield self.body
 
 
 class Outputter:
+    """
+    An outputter converts test results to renderable strings.
+    """
+
     _last_test_class = None
     _last_test_module = None
     _current_subtests_test = None
 
     FAILED, PASSED = "FAILED", "PASSED"
     ERROR, FAIL, OK, SKIPPED = "[ERROR]", "[FAIL]", "[OK]", "[SKIPPED]"
     EXPECTED_FAILURE, UNEXPECTED_SUCCESS = "[XFAIL]", "[UNEXPECTED SUCCESS]"
@@ -78,17 +82,22 @@
         }
 
     def _show_later(self, **kwargs):
         message = _DelayedMessage(width=self.line_width, **kwargs)
         self._later[message.status][message.body].append(message)
 
     def run_started(self):
-        pass
+        """
+        Output nothing.
+        """
 
     def run_stopped(self, recorder, runtime):
+        """
+        Output all the messages stored for later, as well as a final summary.
+        """
         for status in self._later.values():
             for messages in status.values():
                 if not messages:
                     continue
                 yield "\n"
                 yield from messages[0].lines()
                 for message in messages:
@@ -132,14 +141,17 @@
                     summary.append(f"{attribute}={subcount}")
             yield ", ".join(summary)
             yield ")"
 
         yield "\n"
 
     def test_started(self, test):
+        """
+        Output the test name.
+        """
         cls = test.__class__
         module = cls.__module__
 
         if self._last_test_module != module:
             self._last_test_module = module
             yield module
             yield "\n"
@@ -147,71 +159,99 @@
         if self._last_test_class != cls:
             self._last_test_class = cls
             yield self.indent
             yield cls.__name__
             yield "\n"
 
     def test_stopped(self, test):
-        pass
+        """
+        Output nothing.
+        """
 
     def test_errored(self, test, exc_info):
+        """
+        Output an error.
+        """
         self._show_later(
             status=self.ERROR,
             body="".join(format_exception(*exc_info)),
             subject=test,
         )
-        return self.format_line(test, self._error)
+        return self._format_line(test, self._error)
 
     def test_failed(self, test, exc_info):
+        """
+        Output a failure.
+        """
         self._show_later(
             status=self.FAIL,
             body="".join(format_exception(*exc_info)),
             subject=test,
         )
-        return self.format_line(test, self._fail)
+        return self._format_line(test, self._fail)
 
     def test_skipped(self, test, reason):
+        """
+        Output a skip.
+        """
         self._show_later(status=self.SKIPPED, body=reason, subject=test)
-        return self.format_line(test, self._skipped)
+        return self._format_line(test, self._skipped)
 
     def test_expectedly_failed(self, test, exc_info):
+        """
+        Output an expected failure.
+        """
         self._show_later(status=self.EXPECTED_FAILURE, subject=test)
-        return self.format_line(test, self._expected_failure)
+        return self._format_line(test, self._expected_failure)
 
     def test_unexpectedly_succeeded(self, test):
+        """
+        Output an unexpected success.
+        """
         self._show_later(status=self.UNEXPECTED_SUCCESS, subject=test)
-        return self.format_line(test, self._unexpected_success)
+        return self._format_line(test, self._unexpected_success)
 
     def test_succeeded(self, test):
-        return self.format_line(test, self._ok)
+        """
+        Output a success.
+        """
+        return self._format_line(test, self._ok)
 
     def subtest_succeeded(self, test, subtest):
-        pass
+        """
+        Output nothing.
+        """
 
     def subtest_failed(self, test, subtest, exc_info):
+        """
+        Output a failed subtest.
+        """
         self._show_later(
             status=self.FAIL,
             body="".join(format_exception(*exc_info)),
             subject=subtest,
         )
-        return self.format_subtest_result(test, subtest, self._fail)
+        return self._format_subtest_result(test, subtest, self._fail)
 
     def subtest_errored(self, test, subtest, exc_info):
+        """
+        Output an errored subtest.
+        """
         self._show_later(
             status=self.ERROR,
             body="".join(format_exception(*exc_info)),
             subject=subtest,
         )
-        return self.format_subtest_result(test, subtest, self._error)
+        return self._format_subtest_result(test, subtest, self._error)
 
-    def format_line(self, test, result):
+    def _format_line(self, test, result):
         before = f"{self.indent}{self.indent}{test._testMethodName} ..."
         return self._pad_center(left=before, right=result) + "\n"
 
-    def format_subtest_result(self, test, subtest, result):
+    def _format_subtest_result(self, test, subtest, result):
         if self._current_subtests_test != test.id():
             before = f"{self.indent}{self.indent}{test._testMethodName}\n"
         else:
             before = ""
         self._current_subtests_test = test.id()
         line = f"{self.indent * 3}{subtest._subDescription()[1:-1]} ..."
         return f"{before}{self._pad_center(left=line, right=result)}\n"
@@ -237,120 +277,127 @@
     subtest_failures: int = 0
     subtest_errors: int = 0
 
     shouldStop = False
 
     @property
     def count(self):
+        """
+        Return a total count of all tests.
+        """
         return sum(attrs.astuple(self))
 
     testsRun = count
 
-    def startTest(self, test):
+    def startTest(self, test):  # noqa: D102
         pass
 
-    def stopTest(self, test):
+    def stopTest(self, test):  # noqa: D102
         pass
 
-    def addError(self, test, exc_info):
+    def addError(self, test, exc_info):  # noqa: D102
         self.errors += 1
 
-    def addFailure(self, test, exc_info):
+    def addFailure(self, test, exc_info):  # noqa: D102
         self.failures += 1
 
-    def addExpectedFailure(self, *args, **kwargs):
+    def addExpectedFailure(self, *args, **kwargs):  # noqa: D102
         self.expected_failures += 1
 
-    def addUnexpectedSuccess(self, test):
+    def addUnexpectedSuccess(self, test):  # noqa: D102
         self.unexpected_successes += 1
 
-    def addSuccess(self, test):
+    def addSuccess(self, test):  # noqa: D102
         self.successes += 1
 
-    def addSubTest(self, test, subtest, outcome):
+    def addSubTest(self, test, subtest, outcome):  # noqa: D102
         if outcome is None:
             self.subtest_successes += 1
         elif issubclass(outcome[0], test.failureException):
             self.subtest_failures += 1
         else:
             self.subtest_errors += 1
 
 
 @attrs.define(slots=False)
 class Recorder:
+    """
+    Record test results for later inspection.
+    """
+
     errors: PVector = v()
     failures: PVector = v()
     skips: PVector = v()
     successes: PVector = v()
     expected_failures: PVector = v()
     unexpected_successes: PVector = v()
 
     subtest_successes: PMap = m()
     subtest_failures: PMap = m()
     subtest_errors: PMap = m()
 
     shouldStop = False
 
     @property
-    def testsRun(self):
+    def testsRun(self):  # noqa: D102
         fields = attrs.astuple(
             self,
             filter=lambda f, _: not f.name.startswith("subtest_"),
         )
         # It seems addSuccess is called for tests with all passing subtests
         # but the reverse isn't true if a subtest fails...
         tests_with_subtests = len(self.subtest_failures | self.subtest_errors)
         return sum(len(each) for each in fields) + tests_with_subtests
 
     @property
-    def subtests(self):
+    def subtests(self):  # noqa: D102
         return sum(
             1
             for each in (
                 self.subtest_successes,
                 self.subtest_failures,
                 self.subtest_errors,
             )
             for value in each.values()
             for _ in value
         )
 
-    def startTestRun(self):
+    def startTestRun(self):  # noqa: D102
         pass
 
-    def stopTestRun(self):
+    def stopTestRun(self):  # noqa: D102
         pass
 
-    def startTest(self, test):
+    def startTest(self, test):  # noqa: D102
         pass
 
-    def stopTest(self, test):
+    def stopTest(self, test):  # noqa: D102
         pass
 
-    def addError(self, test, exc_info):
+    def addError(self, test, exc_info):  # noqa: D102
         self.errors = self.errors.append((test, exc_info))
 
-    def addFailure(self, test, exc_info):
+    def addFailure(self, test, exc_info):  # noqa: D102
         self.failures = self.failures.append((test, exc_info))
 
-    def addExpectedFailure(self, test, exc_info):
+    def addExpectedFailure(self, test, exc_info):  # noqa: D102
         self.expected_failures = self.expected_failures.append(
             (test, exc_info),
         )
 
-    def addSkip(self, test, reason):
+    def addSkip(self, test, reason):  # noqa: D102
         self.skips = self.skips.append(test)
 
-    def addUnexpectedSuccess(self, test):
+    def addUnexpectedSuccess(self, test):  # noqa: D102
         self.unexpected_successes = self.unexpected_successes.append(test)
 
-    def addSuccess(self, test):
+    def addSuccess(self, test):  # noqa: D102
         self.successes = self.successes.append(test)
 
-    def addSubTest(self, test, subtest, outcome):
+    def addSubTest(self, test, subtest, outcome):  # noqa: D102
         if outcome is None:
             self.subtest_successes = self.subtest_successes.set(
                 test,
                 self.subtest_successes.get(test, v()).append(subtest),
             )
         elif issubclass(outcome[0], test.failureException):
             self.subtest_failures = self.subtest_failures.set(
@@ -359,95 +406,99 @@
             )
         else:
             self.subtest_errors = self.subtest_errors.set(
                 test,
                 self.subtest_errors.get(test, v()).append(subtest),
             )
 
-    def wasSuccessful(self):
+    def wasSuccessful(self):  # noqa: D102
         return not (
             self.errors
             or self.failures
             or self.unexpected_successes
             or self.subtest_failures
             or self.subtest_errors
         )
 
 
 @attrs.define(slots=False)
 class ComponentizedReporter:
+    """
+    Combine together outputting and recording capabilities.
+    """
+
     outputter: Outputter = attrs.field(factory=Outputter)
     recorder = attrs.field(factory=Recorder, repr=False)
     stream = attrs.field(default=sys.stdout)
     _time = attrs.field(default=time.time, repr=False)
 
     failfast = False  # FIXME: needed for subtests?
     shouldStop = False
 
     @property
-    def testsRun(self):
+    def testsRun(self):  # noqa: D102
         return self.recorder.testsRun
 
-    def startTestRun(self):
+    def startTestRun(self):  # noqa: D102
         self._start_time = self._time()
         self.recorder.startTestRun()
         self.stream.writelines(self.outputter.run_started() or "")
 
-    def stopTestRun(self):
+    def stopTestRun(self):  # noqa: D102
         self.recorder.stopTestRun()
         runtime = self._time() - self._start_time
         self.stream.writelines(
             self.outputter.run_stopped(self.recorder, runtime) or "",
         )
 
-    def startTest(self, test):
+    def startTest(self, test):  # noqa: D102
         self.recorder.startTest(test)
         self.stream.writelines(self.outputter.test_started(test) or "")
 
-    def stopTest(self, test):
+    def stopTest(self, test):  # noqa: D102
         self.recorder.stopTest(test)
         self.stream.writelines(self.outputter.test_stopped(test) or "")
 
-    def addError(self, test, exc_info):
+    def addError(self, test, exc_info):  # noqa: D102
         self.recorder.addError(test, exc_info)
         self.stream.writelines(
             self.outputter.test_errored(test, exc_info) or "",
         )
 
-    def addFailure(self, test, exc_info):
+    def addFailure(self, test, exc_info):  # noqa: D102
         self.recorder.addFailure(test, exc_info)
         self.stream.writelines(
             self.outputter.test_failed(test, exc_info) or "",
         )
 
-    def addSkip(self, test, reason):
+    def addSkip(self, test, reason):  # noqa: D102
         self.recorder.addSkip(test, reason)
         self.stream.writelines(self.outputter.test_skipped(test, reason) or "")
 
-    def addExpectedFailure(self, test, exc_info):
+    def addExpectedFailure(self, test, exc_info):  # noqa: D102
         self.recorder.addExpectedFailure(test, exc_info)
         self.stream.writelines(
             self.outputter.test_expectedly_failed(test, exc_info) or "",
         )
 
-    def addUnexpectedSuccess(self, test):
+    def addUnexpectedSuccess(self, test):  # noqa: D102
         self.recorder.addUnexpectedSuccess(test)
         self.stream.writelines(
             self.outputter.test_unexpectedly_succeeded(test) or "",
         )
 
-    def addSuccess(self, test):
+    def addSuccess(self, test):  # noqa: D102
         self.recorder.addSuccess(test)
         self.stream.writelines(self.outputter.test_succeeded(test) or "")
 
-    def addSubTest(self, test, subtest, outcome):
+    def addSubTest(self, test, subtest, outcome):  # noqa: D102
         self.recorder.addSubTest(test, subtest, outcome)
         if outcome is None:
             output = self.outputter.subtest_succeeded(test, subtest)
         elif issubclass(outcome[0], test.failureException):
             output = self.outputter.subtest_failed(test, subtest, outcome)
         else:
             output = self.outputter.subtest_errored(test, subtest, outcome)
         self.stream.writelines(output or "")
 
-    def wasSuccessful(self):
+    def wasSuccessful(self):  # noqa: D102
         return self.recorder.wasSuccessful()
```

### Comparing `virtue-2023.5.1/virtue/runner.py` & `virtue-2023.5.3/virtue/runner.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.5.1/virtue/tests/test_cli.py` & `virtue-2023.5.3/virtue/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.5.1/virtue/tests/test_loaders.py` & `virtue-2023.5.3/virtue/tests/test_loaders.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.5.1/virtue/tests/test_locators.py` & `virtue-2023.5.3/virtue/tests/test_locators.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.5.1/virtue/tests/test_reporters.py` & `virtue-2023.5.3/virtue/tests/test_reporters.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.5.1/virtue/tests/test_runner.py` & `virtue-2023.5.3/virtue/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.5.1/virtue/tests/samples/subtests.py` & `virtue-2023.5.3/virtue/tests/samples/subtests.py`

 * *Files identical despite different names*

### Comparing `virtue-2023.5.1/COPYING` & `virtue-2023.5.3/COPYING`

 * *Files identical despite different names*

### Comparing `virtue-2023.5.1/README.rst` & `virtue-2023.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `virtue-2023.5.1/PKG-INFO` & `virtue-2023.5.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: virtue
-Version: 2023.5.1
+Version: 2023.5.3
 Summary: After trial comes virtue. A test runner for good.
-Project-URL: homepage, https://github.com/Julian/Virtue
-Project-URL: documentation, https://virtue.readthedocs.io/
-Project-URL: issues, https://github.com/Julian/Virtue/issues/
-Project-URL: funding, https://github.com/sponsors/Julian
-Project-URL: source, https://github.com/Julian/Virtue
+Project-URL: Homepage, https://github.com/Julian/Virtue
+Project-URL: Documentation, https://virtue.readthedocs.io/
+Project-URL: Issues, https://github.com/Julian/Virtue/issues/
+Project-URL: Funding, https://github.com/sponsors/Julian
+Project-URL: Source, https://github.com/Julian/Virtue
 Author: Julian Berman
 Author-email: Julian+Virtue@GrayVines.com
 License: MIT
 License-File: COPYING
 Keywords: test runner,testing,tests,unittest
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

