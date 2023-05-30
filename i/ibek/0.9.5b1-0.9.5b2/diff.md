# Comparing `tmp/ibek-0.9.5b1.tar.gz` & `tmp/ibek-0.9.5b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibek-0.9.5b1.tar", last modified: Wed Mar  8 10:39:40 2023, max compression
+gzip compressed data, was "ibek-0.9.5b2.tar", last modified: Wed Mar  8 12:09:25 2023, max compression
```

## Comparing `ibek-0.9.5b1.tar` & `ibek-0.9.5b2.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 10:39:40.793657 ibek-0.9.5b1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 10:39:40.785657 ibek-0.9.5b1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-03-08 10:39:27.000000 ibek-0.9.5b1/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-03-08 10:39:27.000000 ibek-0.9.5b1/.devcontainer/devcontainer.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      537 2023-03-08 10:39:27.000000 ibek-0.9.5b1/.devcontainer/local_build.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 10:39:40.785657 ibek-0.9.5b1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-03-08 10:39:27.000000 ibek-0.9.5b1/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 10:39:40.781657 ibek-0.9.5b1/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 10:39:40.785657 ibek-0.9.5b1/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-03-08 10:39:27.000000 ibek-0.9.5b1/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-03-08 10:39:27.000000 ibek-0.9.5b1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 10:39:40.785657 ibek-0.9.5b1/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-08 10:39:27.000000 ibek-0.9.5b1/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-03-08 10:39:27.000000 ibek-0.9.5b1/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 10:39:40.785657 ibek-0.9.5b1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6501 2023-03-08 10:39:27.000000 ibek-0.9.5b1/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-03-08 10:39:27.000000 ibek-0.9.5b1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-03-08 10:39:27.000000 ibek-0.9.5b1/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-08 10:39:27.000000 ibek-0.9.5b1/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-03-08 10:39:27.000000 ibek-0.9.5b1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-08 10:39:27.000000 ibek-0.9.5b1/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-08 10:39:27.000000 ibek-0.9.5b1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 10:39:40.785657 ibek-0.9.5b1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-08 10:39:27.000000 ibek-0.9.5b1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-03-08 10:39:27.000000 ibek-0.9.5b1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-03-08 10:39:27.000000 ibek-0.9.5b1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-08 10:39:27.000000 ibek-0.9.5b1/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-03-08 10:39:27.000000 ibek-0.9.5b1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-08 10:39:27.000000 ibek-0.9.5b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-03-08 10:39:40.793657 ibek-0.9.5b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    61767 2023-03-08 10:39:27.000000 ibek-0.9.5b1/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-03-08 10:39:27.000000 ibek-0.9.5b1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 10:39:40.785657 ibek-0.9.5b1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-03-08 10:39:27.000000 ibek-0.9.5b1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 10:39:40.785657 ibek-0.9.5b1/docs/developer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 10:39:40.785657 ibek-0.9.5b1/docs/developer/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 10:39:40.785657 ibek-0.9.5b1/docs/developer/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-08 10:39:27.000000 ibek-0.9.5b1/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-08 10:39:27.000000 ibek-0.9.5b1/docs/developer/explanations/decisions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-03-08 10:39:27.000000 ibek-0.9.5b1/docs/developer/explanations/entities.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 10:39:40.785657 ibek-0.9.5b1/docs/developer/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-03-08 10:39:27.000000 ibek-0.9.5b1/docs/developer/how-to/build-docs.rst
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-08 10:39:27.000000 ibek-0.9.5b1/docs/developer/how-to/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-03-08 10:39:27.000000 ibek-0.9.5b1/docs/developer/how-to/lint.rst
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-03-08 10:39:27.000000 ibek-0.9.5b1/docs/developer/how-to/make-release.rst
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-03-08 10:39:27.000000 ibek-0.9.5b1/docs/developer/how-to/run-tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-08 10:39:27.000000 ibek-0.9.5b1/docs/developer/how-to/static-analysis.rst
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-03-08 10:39:27.000000 ibek-0.9.5b1/docs/developer/how-to/update-tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-03-08 10:39:27.000000 ibek-0.9.5b1/docs/developer/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 10:39:40.789657 ibek-0.9.5b1/docs/developer/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-03-08 10:39:27.000000 ibek-0.9.5b1/docs/developer/reference/standards.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 10:39:40.789657 ibek-0.9.5b1/docs/developer/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-03-08 10:39:27.000000 ibek-0.9.5b1/docs/developer/tutorials/dev-install.rst
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-08 10:39:27.000000 ibek-0.9.5b1/docs/genindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 10:39:40.789657 ibek-0.9.5b1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)     9465 2023-03-08 10:39:27.000000 ibek-0.9.5b1/docs/images/ibek-arch.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14318 2023-03-08 10:39:27.000000 ibek-0.9.5b1/docs/images/ibek-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-03-08 10:39:27.000000 ibek-0.9.5b1/docs/images/ibek-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-08 10:39:27.000000 ibek-0.9.5b1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 10:39:40.789657 ibek-0.9.5b1/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 10:39:40.789657 ibek-0.9.5b1/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-03-08 10:39:27.000000 ibek-0.9.5b1/docs/user/explanations/docs-structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 10:39:40.789657 ibek-0.9.5b1/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-08 10:39:27.000000 ibek-0.9.5b1/docs/user/how-to/edit-yaml.rst
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-03-08 10:39:27.000000 ibek-0.9.5b1/docs/user/how-to/run-container.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-03-08 10:39:27.000000 ibek-0.9.5b1/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 10:39:40.789657 ibek-0.9.5b1/docs/user/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-03-08 10:39:27.000000 ibek-0.9.5b1/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 10:39:40.789657 ibek-0.9.5b1/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-03-08 10:39:27.000000 ibek-0.9.5b1/docs/user/tutorials/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-08 10:39:27.000000 ibek-0.9.5b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-03-08 10:39:40.793657 ibek-0.9.5b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 10:39:40.781657 ibek-0.9.5b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 10:39:40.789657 ibek-0.9.5b1/src/ibek/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-08 10:39:27.000000 ibek-0.9.5b1/src/ibek/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-03-08 10:39:27.000000 ibek-0.9.5b1/src/ibek/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-08 10:39:40.000000 ibek-0.9.5b1/src/ibek/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-03-08 10:39:27.000000 ibek-0.9.5b1/src/ibek/gen_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-08 10:39:27.000000 ibek-0.9.5b1/src/ibek/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-03-08 10:39:27.000000 ibek-0.9.5b1/src/ibek/ioc.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-03-08 10:39:27.000000 ibek-0.9.5b1/src/ibek/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-03-08 10:39:27.000000 ibek-0.9.5b1/src/ibek/render.py
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-03-08 10:39:27.000000 ibek-0.9.5b1/src/ibek/support.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 10:39:40.789657 ibek-0.9.5b1/src/ibek/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-08 10:39:27.000000 ibek-0.9.5b1/src/ibek/templates/make_db.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-03-08 10:39:27.000000 ibek-0.9.5b1/src/ibek/templates/st.cmd.jinja
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 10:39:40.789657 ibek-0.9.5b1/src/ibek.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-03-08 10:39:40.000000 ibek-0.9.5b1/src/ibek.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-03-08 10:39:40.000000 ibek-0.9.5b1/src/ibek.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 10:39:40.000000 ibek-0.9.5b1/src/ibek.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-08 10:39:40.000000 ibek-0.9.5b1/src/ibek.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-03-08 10:39:40.000000 ibek-0.9.5b1/src/ibek.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-08 10:39:40.000000 ibek-0.9.5b1/src/ibek.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 10:39:40.793657 ibek-0.9.5b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 10:39:27.000000 ibek-0.9.5b1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-03-08 10:39:27.000000 ibek-0.9.5b1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 10:39:40.793657 ibek-0.9.5b1/tests/samples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 10:39:40.793657 ibek-0.9.5b1/tests/samples/boot_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-08 10:39:27.000000 ibek-0.9.5b1/tests/samples/boot_scripts/st.cmd
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-08 10:39:27.000000 ibek-0.9.5b1/tests/samples/boot_scripts/stIOC
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-03-08 10:39:27.000000 ibek-0.9.5b1/tests/samples/boot_scripts/stbl45p-mo-ioc-03
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-03-08 10:39:27.000000 ibek-0.9.5b1/tests/samples/boot_scripts/stbl45p-mo-ioc-04
--rwxr-xr-x   0 runner    (1001) docker     (123)     2170 2023-03-08 10:39:27.000000 ibek-0.9.5b1/tests/samples/generate_samples.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 10:39:40.793657 ibek-0.9.5b1/tests/samples/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-03-08 10:39:27.000000 ibek-0.9.5b1/tests/samples/schemas/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-03-08 10:39:27.000000 ibek-0.9.5b1/tests/samples/schemas/asyn.ibek.entities.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    31543 2023-03-08 10:39:27.000000 ibek-0.9.5b1/tests/samples/schemas/bl45p-mo-ioc-04.ibek.entities.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    32599 2023-03-08 10:39:27.000000 ibek-0.9.5b1/tests/samples/schemas/container.ibek.entities.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-03-08 10:39:27.000000 ibek-0.9.5b1/tests/samples/schemas/epics.ibek.defs.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-03-08 10:39:27.000000 ibek-0.9.5b1/tests/samples/schemas/epics.ibek.support.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-03-08 10:39:27.000000 ibek-0.9.5b1/tests/samples/schemas/ibek.defs.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    28721 2023-03-08 10:39:27.000000 ibek-0.9.5b1/tests/samples/schemas/pmac.ibek.entities.schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 10:39:40.793657 ibek-0.9.5b1/tests/samples/yaml/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-03-08 10:39:27.000000 ibek-0.9.5b1/tests/samples/yaml/bl45p-mo-ioc-02.ibek.entities.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-03-08 10:39:27.000000 ibek-0.9.5b1/tests/samples/yaml/bl45p-mo-ioc-03.ibek.entities.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-03-08 10:39:27.000000 ibek-0.9.5b1/tests/samples/yaml/bl45p-mo-ioc-04.ibek.entities.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-03-08 10:39:27.000000 ibek-0.9.5b1/tests/test_boilerplate_removed.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-03-08 10:39:27.000000 ibek-0.9.5b1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-03-08 10:39:27.000000 ibek-0.9.5b1/tests/test_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-08 10:39:27.000000 ibek-0.9.5b1/tests/test_ibek.py
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-03-08 10:39:27.000000 ibek-0.9.5b1/tests/test_render.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-03-08 10:39:27.000000 ibek-0.9.5b1/tests/test_temp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:09:25.452138 ibek-0.9.5b2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:09:25.440137 ibek-0.9.5b2/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-03-08 12:09:13.000000 ibek-0.9.5b2/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-03-08 12:09:13.000000 ibek-0.9.5b2/.devcontainer/devcontainer.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      537 2023-03-08 12:09:13.000000 ibek-0.9.5b2/.devcontainer/local_build.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:09:25.440137 ibek-0.9.5b2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-03-08 12:09:13.000000 ibek-0.9.5b2/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:09:25.432137 ibek-0.9.5b2/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:09:25.440137 ibek-0.9.5b2/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-03-08 12:09:13.000000 ibek-0.9.5b2/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-03-08 12:09:13.000000 ibek-0.9.5b2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:09:25.440137 ibek-0.9.5b2/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-08 12:09:13.000000 ibek-0.9.5b2/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-03-08 12:09:13.000000 ibek-0.9.5b2/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:09:25.440137 ibek-0.9.5b2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6501 2023-03-08 12:09:13.000000 ibek-0.9.5b2/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-03-08 12:09:13.000000 ibek-0.9.5b2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-03-08 12:09:13.000000 ibek-0.9.5b2/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-08 12:09:13.000000 ibek-0.9.5b2/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-03-08 12:09:13.000000 ibek-0.9.5b2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-08 12:09:13.000000 ibek-0.9.5b2/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-08 12:09:13.000000 ibek-0.9.5b2/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:09:25.440137 ibek-0.9.5b2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-08 12:09:13.000000 ibek-0.9.5b2/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-03-08 12:09:13.000000 ibek-0.9.5b2/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-03-08 12:09:13.000000 ibek-0.9.5b2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-03-08 12:09:13.000000 ibek-0.9.5b2/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-03-08 12:09:13.000000 ibek-0.9.5b2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-08 12:09:13.000000 ibek-0.9.5b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-03-08 12:09:25.452138 ibek-0.9.5b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    61767 2023-03-08 12:09:13.000000 ibek-0.9.5b2/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-03-08 12:09:13.000000 ibek-0.9.5b2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:09:25.444137 ibek-0.9.5b2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-03-08 12:09:13.000000 ibek-0.9.5b2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:09:25.444137 ibek-0.9.5b2/docs/developer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:09:25.444137 ibek-0.9.5b2/docs/developer/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:09:25.444137 ibek-0.9.5b2/docs/developer/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-08 12:09:13.000000 ibek-0.9.5b2/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-08 12:09:13.000000 ibek-0.9.5b2/docs/developer/explanations/decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-03-08 12:09:13.000000 ibek-0.9.5b2/docs/developer/explanations/entities.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:09:25.444137 ibek-0.9.5b2/docs/developer/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-03-08 12:09:13.000000 ibek-0.9.5b2/docs/developer/how-to/build-docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-08 12:09:13.000000 ibek-0.9.5b2/docs/developer/how-to/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-03-08 12:09:13.000000 ibek-0.9.5b2/docs/developer/how-to/lint.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-03-08 12:09:13.000000 ibek-0.9.5b2/docs/developer/how-to/make-release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-03-08 12:09:13.000000 ibek-0.9.5b2/docs/developer/how-to/run-tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-08 12:09:13.000000 ibek-0.9.5b2/docs/developer/how-to/static-analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-03-08 12:09:13.000000 ibek-0.9.5b2/docs/developer/how-to/update-tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-03-08 12:09:13.000000 ibek-0.9.5b2/docs/developer/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:09:25.444137 ibek-0.9.5b2/docs/developer/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-03-08 12:09:13.000000 ibek-0.9.5b2/docs/developer/reference/standards.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:09:25.444137 ibek-0.9.5b2/docs/developer/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-03-08 12:09:13.000000 ibek-0.9.5b2/docs/developer/tutorials/dev-install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-08 12:09:13.000000 ibek-0.9.5b2/docs/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:09:25.444137 ibek-0.9.5b2/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     9465 2023-03-08 12:09:13.000000 ibek-0.9.5b2/docs/images/ibek-arch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14318 2023-03-08 12:09:13.000000 ibek-0.9.5b2/docs/images/ibek-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-03-08 12:09:13.000000 ibek-0.9.5b2/docs/images/ibek-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-08 12:09:13.000000 ibek-0.9.5b2/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:09:25.444137 ibek-0.9.5b2/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:09:25.444137 ibek-0.9.5b2/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-03-08 12:09:13.000000 ibek-0.9.5b2/docs/user/explanations/docs-structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:09:25.444137 ibek-0.9.5b2/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-08 12:09:13.000000 ibek-0.9.5b2/docs/user/how-to/edit-yaml.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-03-08 12:09:13.000000 ibek-0.9.5b2/docs/user/how-to/run-container.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-03-08 12:09:13.000000 ibek-0.9.5b2/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:09:25.444137 ibek-0.9.5b2/docs/user/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-03-08 12:09:13.000000 ibek-0.9.5b2/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:09:25.448138 ibek-0.9.5b2/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-03-08 12:09:13.000000 ibek-0.9.5b2/docs/user/tutorials/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-08 12:09:13.000000 ibek-0.9.5b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-03-08 12:09:25.456138 ibek-0.9.5b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:09:25.436137 ibek-0.9.5b2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:09:25.448138 ibek-0.9.5b2/src/ibek/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-08 12:09:13.000000 ibek-0.9.5b2/src/ibek/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-03-08 12:09:13.000000 ibek-0.9.5b2/src/ibek/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-08 12:09:25.000000 ibek-0.9.5b2/src/ibek/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-03-08 12:09:13.000000 ibek-0.9.5b2/src/ibek/gen_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-08 12:09:13.000000 ibek-0.9.5b2/src/ibek/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-03-08 12:09:13.000000 ibek-0.9.5b2/src/ibek/ioc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-03-08 12:09:13.000000 ibek-0.9.5b2/src/ibek/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-03-08 12:09:13.000000 ibek-0.9.5b2/src/ibek/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-03-08 12:09:13.000000 ibek-0.9.5b2/src/ibek/support.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:09:25.448138 ibek-0.9.5b2/src/ibek/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-08 12:09:13.000000 ibek-0.9.5b2/src/ibek/templates/make_db.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-03-08 12:09:13.000000 ibek-0.9.5b2/src/ibek/templates/st.cmd.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:09:25.448138 ibek-0.9.5b2/src/ibek.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-03-08 12:09:25.000000 ibek-0.9.5b2/src/ibek.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-03-08 12:09:25.000000 ibek-0.9.5b2/src/ibek.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 12:09:25.000000 ibek-0.9.5b2/src/ibek.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-08 12:09:25.000000 ibek-0.9.5b2/src/ibek.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-03-08 12:09:25.000000 ibek-0.9.5b2/src/ibek.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-08 12:09:25.000000 ibek-0.9.5b2/src/ibek.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:09:25.452138 ibek-0.9.5b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-08 12:09:13.000000 ibek-0.9.5b2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-03-08 12:09:13.000000 ibek-0.9.5b2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:09:25.452138 ibek-0.9.5b2/tests/samples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:09:25.452138 ibek-0.9.5b2/tests/samples/boot_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-08 12:09:13.000000 ibek-0.9.5b2/tests/samples/boot_scripts/st.cmd
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-08 12:09:13.000000 ibek-0.9.5b2/tests/samples/boot_scripts/stIOC
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-03-08 12:09:13.000000 ibek-0.9.5b2/tests/samples/boot_scripts/stbl45p-mo-ioc-03
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-08 12:09:13.000000 ibek-0.9.5b2/tests/samples/boot_scripts/stbl45p-mo-ioc-04
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2170 2023-03-08 12:09:13.000000 ibek-0.9.5b2/tests/samples/generate_samples.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:09:25.452138 ibek-0.9.5b2/tests/samples/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-03-08 12:09:13.000000 ibek-0.9.5b2/tests/samples/schemas/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-03-08 12:09:13.000000 ibek-0.9.5b2/tests/samples/schemas/asyn.ibek.entities.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    32880 2023-03-08 12:09:13.000000 ibek-0.9.5b2/tests/samples/schemas/bl45p-mo-ioc-04.ibek.entities.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    32599 2023-03-08 12:09:13.000000 ibek-0.9.5b2/tests/samples/schemas/container.ibek.entities.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3542 2023-03-08 12:09:13.000000 ibek-0.9.5b2/tests/samples/schemas/epics.ibek.defs.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-03-08 12:09:13.000000 ibek-0.9.5b2/tests/samples/schemas/epics.ibek.support.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-03-08 12:09:13.000000 ibek-0.9.5b2/tests/samples/schemas/ibek.defs.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28721 2023-03-08 12:09:13.000000 ibek-0.9.5b2/tests/samples/schemas/pmac.ibek.entities.schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 12:09:25.452138 ibek-0.9.5b2/tests/samples/yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-03-08 12:09:13.000000 ibek-0.9.5b2/tests/samples/yaml/bl45p-mo-ioc-02.ibek.entities.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-03-08 12:09:13.000000 ibek-0.9.5b2/tests/samples/yaml/bl45p-mo-ioc-03.ibek.entities.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-03-08 12:09:13.000000 ibek-0.9.5b2/tests/samples/yaml/bl45p-mo-ioc-04.ibek.entities.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-03-08 12:09:13.000000 ibek-0.9.5b2/tests/test_boilerplate_removed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-03-08 12:09:13.000000 ibek-0.9.5b2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-03-08 12:09:13.000000 ibek-0.9.5b2/tests/test_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-08 12:09:13.000000 ibek-0.9.5b2/tests/test_ibek.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-03-08 12:09:13.000000 ibek-0.9.5b2/tests/test_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-03-08 12:09:13.000000 ibek-0.9.5b2/tests/test_temp.py
```

### Comparing `ibek-0.9.5b1/.devcontainer/Dockerfile` & `ibek-0.9.5b2/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/.devcontainer/devcontainer.json` & `ibek-0.9.5b2/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/.devcontainer/local_build.sh` & `ibek-0.9.5b2/.devcontainer/local_build.sh`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/.github/CONTRIBUTING.rst` & `ibek-0.9.5b2/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/.github/actions/install_requirements/action.yml` & `ibek-0.9.5b2/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/.github/dependabot.yml` & `ibek-0.9.5b2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/.github/pages/make_switcher.py` & `ibek-0.9.5b2/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/.github/workflows/code.yml` & `ibek-0.9.5b2/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/.github/workflows/docs.yml` & `ibek-0.9.5b2/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/.github/workflows/docs_clean.yml` & `ibek-0.9.5b2/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/.github/workflows/linkcheck.yml` & `ibek-0.9.5b2/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/.gitignore` & `ibek-0.9.5b2/.gitignore`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/.vscode/launch.json` & `ibek-0.9.5b2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/LICENSE` & `ibek-0.9.5b2/LICENSE`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/PKG-INFO` & `ibek-0.9.5b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibek
-Version: 0.9.5b1
+Version: 0.9.5b2
 Summary: IOC Builder for EPICS and Kubernetes
 Home-page: https://github.com/epics-containers/ibek
 Author: Tom Cobb
 Author-email: tom.cobb@diamond.ac.uk
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ibek-0.9.5b1/Pipfile.lock` & `ibek-0.9.5b2/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/README.rst` & `ibek-0.9.5b2/README.rst`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/docs/conf.py` & `ibek-0.9.5b2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/docs/developer/explanations/decisions.rst` & `ibek-0.9.5b2/docs/developer/explanations/decisions.rst`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/docs/developer/explanations/entities.rst` & `ibek-0.9.5b2/docs/developer/explanations/entities.rst`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/docs/developer/how-to/build-docs.rst` & `ibek-0.9.5b2/docs/developer/how-to/build-docs.rst`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/docs/developer/how-to/lint.rst` & `ibek-0.9.5b2/docs/developer/how-to/lint.rst`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/docs/developer/how-to/make-release.rst` & `ibek-0.9.5b2/docs/developer/how-to/make-release.rst`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/docs/developer/how-to/update-tools.rst` & `ibek-0.9.5b2/docs/developer/how-to/update-tools.rst`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/docs/developer/index.rst` & `ibek-0.9.5b2/docs/developer/index.rst`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/docs/developer/reference/standards.rst` & `ibek-0.9.5b2/docs/developer/reference/standards.rst`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/docs/developer/tutorials/dev-install.rst` & `ibek-0.9.5b2/docs/developer/tutorials/dev-install.rst`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/docs/images/ibek-arch.svg` & `ibek-0.9.5b2/docs/images/ibek-arch.svg`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/docs/images/ibek-favicon.ico` & `ibek-0.9.5b2/docs/images/ibek-favicon.ico`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/docs/images/ibek-logo.svg` & `ibek-0.9.5b2/docs/images/ibek-logo.svg`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/docs/index.rst` & `ibek-0.9.5b2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/docs/user/explanations/docs-structure.rst` & `ibek-0.9.5b2/docs/user/explanations/docs-structure.rst`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/docs/user/index.rst` & `ibek-0.9.5b2/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/docs/user/reference/api.rst` & `ibek-0.9.5b2/docs/user/reference/api.rst`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/docs/user/tutorials/installation.rst` & `ibek-0.9.5b2/docs/user/tutorials/installation.rst`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/setup.cfg` & `ibek-0.9.5b2/setup.cfg`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/src/ibek/__main__.py` & `ibek-0.9.5b2/src/ibek/__main__.py`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/src/ibek/gen_scripts.py` & `ibek-0.9.5b2/src/ibek/gen_scripts.py`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/src/ibek/ioc.py` & `ibek-0.9.5b2/src/ibek/ioc.py`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/src/ibek/render.py` & `ibek-0.9.5b2/src/ibek/render.py`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/src/ibek/support.py` & `ibek-0.9.5b2/src/ibek/support.py`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/src/ibek.egg-info/PKG-INFO` & `ibek-0.9.5b2/src/ibek.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibek
-Version: 0.9.5b1
+Version: 0.9.5b2
 Summary: IOC Builder for EPICS and Kubernetes
 Home-page: https://github.com/epics-containers/ibek
 Author: Tom Cobb
 Author-email: tom.cobb@diamond.ac.uk
 License: Apache License 2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `ibek-0.9.5b1/src/ibek.egg-info/SOURCES.txt` & `ibek-0.9.5b2/src/ibek.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/tests/conftest.py` & `ibek-0.9.5b2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/tests/samples/boot_scripts/stbl45p-mo-ioc-03` & `ibek-0.9.5b2/tests/samples/boot_scripts/stbl45p-mo-ioc-03`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,9 @@
 pmacCreateAxes(BL45P-MO-BRICK-01, 8)
 TODO provide Jinja to generate Startup Entries
 note this is interesting because builder.py has a few if clauses
 for generating the necessary script
 
 
 dbLoadRecords("/tmp/ioc.db")
-iocInit()
+iocInit()
+
```

### Comparing `ibek-0.9.5b1/tests/samples/generate_samples.sh` & `ibek-0.9.5b2/tests/samples/generate_samples.sh`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/tests/samples/schemas/asyn.ibek.entities.schema.json` & `ibek-0.9.5b2/tests/samples/schemas/asyn.ibek.entities.schema.json`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/tests/samples/schemas/bl45p-mo-ioc-04.ibek.entities.schema.json` & `ibek-0.9.5b2/tests/samples/schemas/bl45p-mo-ioc-04.ibek.entities.schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998511904761905%*

 * *Differences: {"'properties'": "{'entities': {'items': {'anyOf': {insert: [(4, OrderedDict([('type', 'object'), "*

 * *                 "('properties', OrderedDict([('entity_enabled', OrderedDict([('type', 'boolean'), "*

 * *                 "('default', True)])), ('command', OrderedDict([('type', 'string'), "*

 * *                 "('description', 'An arbitrary command in the startup script before iocInit')])), "*

 * *                 "('type', OrderedDict([('type', 'string'), ('const', 'epics.startupCommand'), "*

 * *                 "('defaul […]*

```diff
@@ -103,14 +103,58 @@
                             "value"
                         ],
                         "type": "object"
                     },
                     {
                         "additionalProperties": false,
                         "properties": {
+                            "command": {
+                                "description": "An arbitrary command in the startup script before iocInit",
+                                "type": "string"
+                            },
+                            "entity_enabled": {
+                                "default": true,
+                                "type": "boolean"
+                            },
+                            "type": {
+                                "const": "epics.startupCommand",
+                                "default": "epics.startupCommand",
+                                "type": "string"
+                            }
+                        },
+                        "required": [
+                            "command"
+                        ],
+                        "type": "object"
+                    },
+                    {
+                        "additionalProperties": false,
+                        "properties": {
+                            "command": {
+                                "description": "An arbitrary command in the startup script after iocInit",
+                                "type": "string"
+                            },
+                            "entity_enabled": {
+                                "default": true,
+                                "type": "boolean"
+                            },
+                            "type": {
+                                "const": "epics.postStartupCommand",
+                                "default": "epics.postStartupCommand",
+                                "type": "string"
+                            }
+                        },
+                        "required": [
+                            "command"
+                        ],
+                        "type": "object"
+                    },
+                    {
+                        "additionalProperties": false,
+                        "properties": {
                             "IP": {
                                 "description": "IP address of Power pmac",
                                 "type": "string"
                             },
                             "NOAUTOCONNECT": {
                                 "default": 0,
                                 "description": "Disables autoconnect if set to 1",
```

### Comparing `ibek-0.9.5b1/tests/samples/schemas/container.ibek.entities.schema.json` & `ibek-0.9.5b2/tests/samples/schemas/container.ibek.entities.schema.json`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/tests/samples/schemas/epics.ibek.defs.schema.json` & `ibek-0.9.5b2/tests/samples/schemas/epics.ibek.defs.schema.json`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/tests/samples/schemas/epics.ibek.support.schema.json` & `ibek-0.9.5b2/tests/samples/schemas/epics.ibek.support.schema.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996527777777778%*

 * *Differences: {"'properties'": "{'entities': {'items': {'anyOf': {insert: [(4, OrderedDict([('type', 'object'), "*

 * *                 "('properties', OrderedDict([('entity_enabled', OrderedDict([('type', 'boolean'), "*

 * *                 "('default', True)])), ('command', OrderedDict([('type', 'string'), "*

 * *                 "('description', 'An arbitrary command in the startup script before iocInit')])), "*

 * *                 "('type', OrderedDict([('type', 'string'), ('const', 'epics.startupCommand'), "*

 * *                 "('defaul […]*

```diff
@@ -99,14 +99,58 @@
                             }
                         },
                         "required": [
                             "name",
                             "value"
                         ],
                         "type": "object"
+                    },
+                    {
+                        "additionalProperties": false,
+                        "properties": {
+                            "command": {
+                                "description": "An arbitrary command in the startup script before iocInit",
+                                "type": "string"
+                            },
+                            "entity_enabled": {
+                                "default": true,
+                                "type": "boolean"
+                            },
+                            "type": {
+                                "const": "epics.startupCommand",
+                                "default": "epics.startupCommand",
+                                "type": "string"
+                            }
+                        },
+                        "required": [
+                            "command"
+                        ],
+                        "type": "object"
+                    },
+                    {
+                        "additionalProperties": false,
+                        "properties": {
+                            "command": {
+                                "description": "An arbitrary command in the startup script after iocInit",
+                                "type": "string"
+                            },
+                            "entity_enabled": {
+                                "default": true,
+                                "type": "boolean"
+                            },
+                            "type": {
+                                "const": "epics.postStartupCommand",
+                                "default": "epics.postStartupCommand",
+                                "type": "string"
+                            }
+                        },
+                        "required": [
+                            "command"
+                        ],
+                        "type": "object"
                     }
                 ]
             },
             "type": "array"
         },
         "generic_ioc_image": {
             "description": "The generic IOC container image registry URL",
```

### Comparing `ibek-0.9.5b1/tests/samples/schemas/ibek.defs.schema.json` & `ibek-0.9.5b2/tests/samples/schemas/ibek.defs.schema.json`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/tests/samples/schemas/pmac.ibek.entities.schema.json` & `ibek-0.9.5b2/tests/samples/schemas/pmac.ibek.entities.schema.json`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/tests/samples/yaml/bl45p-mo-ioc-02.ibek.entities.yaml` & `ibek-0.9.5b2/tests/samples/yaml/bl45p-mo-ioc-02.ibek.entities.yaml`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/tests/samples/yaml/bl45p-mo-ioc-03.ibek.entities.yaml` & `ibek-0.9.5b2/tests/samples/yaml/bl45p-mo-ioc-03.ibek.entities.yaml`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/tests/samples/yaml/bl45p-mo-ioc-04.ibek.entities.yaml` & `ibek-0.9.5b2/tests/samples/yaml/bl45p-mo-ioc-04.ibek.entities.yaml`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/tests/test_boilerplate_removed.py` & `ibek-0.9.5b2/tests/test_boilerplate_removed.py`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/tests/test_cli.py` & `ibek-0.9.5b2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/tests/test_conversions.py` & `ibek-0.9.5b2/tests/test_conversions.py`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/tests/test_render.py` & `ibek-0.9.5b2/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `ibek-0.9.5b1/tests/test_temp.py` & `ibek-0.9.5b2/tests/test_temp.py`

 * *Files identical despite different names*

