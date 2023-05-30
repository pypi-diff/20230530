# Comparing `tmp/teststack-0.8.5.tar.gz` & `tmp/teststack-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teststack-0.8.5.tar", last modified: Mon Oct 17 16:55:26 2022, max compression
+gzip compressed data, was "teststack-0.9.0.tar", last modified: Tue Oct 18 16:09:13 2022, max compression
```

## Comparing `teststack-0.8.5.tar` & `teststack-0.9.0.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-17 16:55:26.851846 teststack-0.8.5/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-17 16:55:26.843846 teststack-0.8.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-17 16:55:26.847846 teststack-0.8.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     2447 2022-10-17 16:55:16.000000 teststack-0.8.5/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (116)      698 2022-10-17 16:55:16.000000 teststack-0.8.5/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (116)      894 2022-10-17 16:55:16.000000 teststack-0.8.5/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (116)      160 2022-10-17 16:55:16.000000 teststack-0.8.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)      127 2022-10-17 16:55:16.000000 teststack-0.8.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)      253 2022-10-17 16:55:16.000000 teststack-0.8.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (116)     5228 2022-10-17 16:55:16.000000 teststack-0.8.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (116)       62 2022-10-17 16:55:16.000000 teststack-0.8.5/Dockerfile.j2
--rw-r--r--   0 runner    (1001) docker     (116)    11357 2022-10-17 16:55:16.000000 teststack-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      214 2022-10-17 16:55:16.000000 teststack-0.8.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (116)     4930 2022-10-17 16:55:26.851846 teststack-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3923 2022-10-17 16:55:16.000000 teststack-0.8.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-17 16:55:26.847846 teststack-0.8.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-17 16:55:26.847846 teststack-0.8.5/docs/commands/
--rw-r--r--   0 runner    (1001) docker     (116)      403 2022-10-17 16:55:16.000000 teststack-0.8.5/docs/commands/containers.rst
--rw-r--r--   0 runner    (1001) docker     (116)      156 2022-10-17 16:55:16.000000 teststack-0.8.5/docs/commands/environment.rst
--rw-r--r--   0 runner    (1001) docker     (116)      110 2022-10-17 16:55:16.000000 teststack-0.8.5/docs/commands/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1922 2022-10-17 16:55:16.000000 teststack-0.8.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)     4228 2022-10-17 16:55:16.000000 teststack-0.8.5/docs/config.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-17 16:55:26.847846 teststack-0.8.5/docs/containers/
--rw-r--r--   0 runner    (1001) docker     (116)       21 2022-10-17 16:55:16.000000 teststack-0.8.5/docs/containers/docker.rst
--rw-r--r--   0 runner    (1001) docker     (116)      107 2022-10-17 16:55:16.000000 teststack-0.8.5/docs/containers/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)       80 2022-10-17 16:55:16.000000 teststack-0.8.5/docs/containers/podman.rst
--rw-r--r--   0 runner    (1001) docker     (116)      653 2022-10-17 16:55:16.000000 teststack-0.8.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)     2491 2022-10-17 16:55:16.000000 teststack-0.8.5/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (116)      679 2022-10-17 16:55:16.000000 teststack-0.8.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)     1549 2022-10-17 16:55:26.851846 teststack-0.8.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)       58 2022-10-17 16:55:16.000000 teststack-0.8.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-17 16:55:26.843846 teststack-0.8.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-17 16:55:26.847846 teststack-0.8.5/src/teststack/
--rw-r--r--   0 runner    (1001) docker     (116)     2711 2022-10-17 16:55:16.000000 teststack-0.8.5/src/teststack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       99 2022-10-17 16:55:16.000000 teststack-0.8.5/src/teststack/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)      176 2022-10-17 16:55:26.000000 teststack-0.8.5/src/teststack/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-17 16:55:26.847846 teststack-0.8.5/src/teststack/commands/
--rw-r--r--   0 runner    (1001) docker     (116)     8376 2022-10-17 16:55:16.000000 teststack-0.8.5/src/teststack/commands/containers.py
--rw-r--r--   0 runner    (1001) docker     (116)     1854 2022-10-17 16:55:16.000000 teststack-0.8.5/src/teststack/commands/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-17 16:55:26.847846 teststack-0.8.5/src/teststack/containers/
--rw-r--r--   0 runner    (1001) docker     (116)     4399 2022-10-17 16:55:16.000000 teststack-0.8.5/src/teststack/containers/docker.py
--rw-r--r--   0 runner    (1001) docker     (116)     5411 2022-10-17 16:55:16.000000 teststack-0.8.5/src/teststack/containers/podman.py
--rw-r--r--   0 runner    (1001) docker     (116)       51 2022-10-17 16:55:16.000000 teststack-0.8.5/src/teststack/errors.py
--rw-r--r--   0 runner    (1001) docker     (116)      814 2022-10-17 16:55:16.000000 teststack-0.8.5/src/teststack/git.py
--rw-r--r--   0 runner    (1001) docker     (116)      749 2022-10-17 16:55:16.000000 teststack-0.8.5/src/teststack/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-17 16:55:26.847846 teststack-0.8.5/src/teststack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4930 2022-10-17 16:55:26.000000 teststack-0.8.5/src/teststack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1671 2022-10-17 16:55:26.000000 teststack-0.8.5/src/teststack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-10-17 16:55:26.000000 teststack-0.8.5/src/teststack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      250 2022-10-17 16:55:26.000000 teststack-0.8.5/src/teststack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-10-17 16:55:26.000000 teststack-0.8.5/src/teststack.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      196 2022-10-17 16:55:26.000000 teststack-0.8.5/src/teststack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       10 2022-10-17 16:55:26.000000 teststack-0.8.5/src/teststack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-17 16:55:26.851846 teststack-0.8.5/tests/
--rw-r--r--   0 runner    (1001) docker     (116)     1817 2022-10-17 16:55:16.000000 teststack-0.8.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-17 16:55:26.851846 teststack-0.8.5/tests/files/
--rw-r--r--   0 runner    (1001) docker     (116)     1004 2022-10-17 16:55:16.000000 teststack-0.8.5/tests/files/build.output
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-17 16:55:26.851846 teststack-0.8.5/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (116)     1259 2022-10-17 16:55:16.000000 teststack-0.8.5/tests/integration/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (116)      294 2022-10-17 16:55:16.000000 teststack-0.8.5/tests/integration/test_env.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-17 16:55:26.851846 teststack-0.8.5/tests/testapp/
--rw-r--r--   0 runner    (1001) docker     (116)      125 2022-10-17 16:55:16.000000 teststack-0.8.5/tests/testapp/Dockerfile.j2
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-17 16:55:26.851846 teststack-0.8.5/tests/testapp/app/
--rw-r--r--   0 runner    (1001) docker     (116)      434 2022-10-17 16:55:16.000000 teststack-0.8.5/tests/testapp/app/application.py
--rw-r--r--   0 runner    (1001) docker     (116)      907 2022-10-17 16:55:16.000000 teststack-0.8.5/tests/testapp/app/config.py
--rw-r--r--   0 runner    (1001) docker     (116)      298 2022-10-17 16:55:16.000000 teststack-0.8.5/tests/testapp/app/database.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-17 16:55:26.843846 teststack-0.8.5/tests/testapp/app/handlers/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-17 16:55:26.851846 teststack-0.8.5/tests/testapp/app/handlers/v1/
--rw-r--r--   0 runner    (1001) docker     (116)      188 2022-10-17 16:55:16.000000 teststack-0.8.5/tests/testapp/app/handlers/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      847 2022-10-17 16:55:16.000000 teststack-0.8.5/tests/testapp/app/handlers/v1/health.py
--rw-r--r--   0 runner    (1001) docker     (116)    45335 2022-10-17 16:55:16.000000 teststack-0.8.5/tests/testapp/poetry.lock
--rw-r--r--   0 runner    (1001) docker     (116)      899 2022-10-17 16:55:16.000000 teststack-0.8.5/tests/testapp/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-17 16:55:26.851846 teststack-0.8.5/tests/testapp/tests/
--rw-r--r--   0 runner    (1001) docker     (116)      172 2022-10-17 16:55:16.000000 teststack-0.8.5/tests/testapp/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-17 16:55:26.851846 teststack-0.8.5/tests/testapp/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (116)      148 2022-10-17 16:55:16.000000 teststack-0.8.5/tests/testapp/tests/unit/test_health.py
--rw-r--r--   0 runner    (1001) docker     (116)      927 2022-10-17 16:55:16.000000 teststack-0.8.5/tests/testapp/teststack.toml
--rw-r--r--   0 runner    (1001) docker     (116)       67 2022-10-17 16:55:16.000000 teststack-0.8.5/tests/testapp/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (116)      993 2022-10-17 16:55:16.000000 teststack-0.8.5/tests/teststack.podman.toml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-17 16:55:26.851846 teststack-0.8.5/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (116)      632 2022-10-17 16:55:16.000000 teststack-0.8.5/tests/unit/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (116)     7349 2022-10-17 16:55:16.000000 teststack-0.8.5/tests/unit/test_command_containers.py
--rw-r--r--   0 runner    (1001) docker     (116)     2021 2022-10-17 16:55:16.000000 teststack-0.8.5/tests/unit/test_command_env.py
--rw-r--r--   0 runner    (1001) docker     (116)      185 2022-10-17 16:55:16.000000 teststack-0.8.5/tests/unit/test_git.py
--rw-r--r--   0 runner    (1001) docker     (116)     1019 2022-10-17 16:55:16.000000 teststack-0.8.5/teststack.toml
--rw-r--r--   0 runner    (1001) docker     (116)      757 2022-10-17 16:55:16.000000 teststack-0.8.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-18 16:09:13.931094 teststack-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-18 16:09:13.923094 teststack-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-18 16:09:13.923094 teststack-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)     2447 2022-10-18 16:09:03.000000 teststack-0.9.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      698 2022-10-18 16:09:03.000000 teststack-0.9.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      894 2022-10-18 16:09:03.000000 teststack-0.9.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      160 2022-10-18 16:09:03.000000 teststack-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)      127 2022-10-18 16:09:03.000000 teststack-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)      253 2022-10-18 16:09:03.000000 teststack-0.9.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)     5228 2022-10-18 16:09:03.000000 teststack-0.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (116)       62 2022-10-18 16:09:03.000000 teststack-0.9.0/Dockerfile.j2
+-rw-r--r--   0 runner    (1001) docker     (116)    11357 2022-10-18 16:09:03.000000 teststack-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      214 2022-10-18 16:09:03.000000 teststack-0.9.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (116)     4930 2022-10-18 16:09:13.931094 teststack-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     3923 2022-10-18 16:09:03.000000 teststack-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-18 16:09:13.923094 teststack-0.9.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-18 16:09:13.927094 teststack-0.9.0/docs/commands/
+-rw-r--r--   0 runner    (1001) docker     (116)      403 2022-10-18 16:09:03.000000 teststack-0.9.0/docs/commands/containers.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      156 2022-10-18 16:09:03.000000 teststack-0.9.0/docs/commands/environment.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      110 2022-10-18 16:09:03.000000 teststack-0.9.0/docs/commands/index.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     1922 2022-10-18 16:09:03.000000 teststack-0.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4228 2022-10-18 16:09:03.000000 teststack-0.9.0/docs/config.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-18 16:09:13.927094 teststack-0.9.0/docs/containers/
+-rw-r--r--   0 runner    (1001) docker     (116)       21 2022-10-18 16:09:03.000000 teststack-0.9.0/docs/containers/docker.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      107 2022-10-18 16:09:03.000000 teststack-0.9.0/docs/containers/index.rst
+-rw-r--r--   0 runner    (1001) docker     (116)       80 2022-10-18 16:09:03.000000 teststack-0.9.0/docs/containers/podman.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      653 2022-10-18 16:09:03.000000 teststack-0.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     2491 2022-10-18 16:09:03.000000 teststack-0.9.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      679 2022-10-18 16:09:03.000000 teststack-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (116)     1549 2022-10-18 16:09:13.931094 teststack-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)       58 2022-10-18 16:09:03.000000 teststack-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-18 16:09:13.923094 teststack-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-18 16:09:13.927094 teststack-0.9.0/src/teststack/
+-rw-r--r--   0 runner    (1001) docker     (116)     2711 2022-10-18 16:09:03.000000 teststack-0.9.0/src/teststack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)       99 2022-10-18 16:09:03.000000 teststack-0.9.0/src/teststack/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      176 2022-10-18 16:09:13.000000 teststack-0.9.0/src/teststack/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-18 16:09:13.927094 teststack-0.9.0/src/teststack/commands/
+-rw-r--r--   0 runner    (1001) docker     (116)     8848 2022-10-18 16:09:03.000000 teststack-0.9.0/src/teststack/commands/containers.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1854 2022-10-18 16:09:03.000000 teststack-0.9.0/src/teststack/commands/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-18 16:09:13.927094 teststack-0.9.0/src/teststack/containers/
+-rw-r--r--   0 runner    (1001) docker     (116)     4439 2022-10-18 16:09:03.000000 teststack-0.9.0/src/teststack/containers/docker.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5445 2022-10-18 16:09:03.000000 teststack-0.9.0/src/teststack/containers/podman.py
+-rw-r--r--   0 runner    (1001) docker     (116)       51 2022-10-18 16:09:03.000000 teststack-0.9.0/src/teststack/errors.py
+-rw-r--r--   0 runner    (1001) docker     (116)      814 2022-10-18 16:09:03.000000 teststack-0.9.0/src/teststack/git.py
+-rw-r--r--   0 runner    (1001) docker     (116)      749 2022-10-18 16:09:03.000000 teststack-0.9.0/src/teststack/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-18 16:09:13.927094 teststack-0.9.0/src/teststack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     4930 2022-10-18 16:09:13.000000 teststack-0.9.0/src/teststack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1671 2022-10-18 16:09:13.000000 teststack-0.9.0/src/teststack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-10-18 16:09:13.000000 teststack-0.9.0/src/teststack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      250 2022-10-18 16:09:13.000000 teststack-0.9.0/src/teststack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2022-10-18 16:09:13.000000 teststack-0.9.0/src/teststack.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)      196 2022-10-18 16:09:13.000000 teststack-0.9.0/src/teststack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       10 2022-10-18 16:09:13.000000 teststack-0.9.0/src/teststack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-18 16:09:13.927094 teststack-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)     1817 2022-10-18 16:09:03.000000 teststack-0.9.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-18 16:09:13.927094 teststack-0.9.0/tests/files/
+-rw-r--r--   0 runner    (1001) docker     (116)     1004 2022-10-18 16:09:03.000000 teststack-0.9.0/tests/files/build.output
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-18 16:09:13.927094 teststack-0.9.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (116)     1259 2022-10-18 16:09:03.000000 teststack-0.9.0/tests/integration/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (116)      294 2022-10-18 16:09:03.000000 teststack-0.9.0/tests/integration/test_env.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-18 16:09:13.927094 teststack-0.9.0/tests/testapp/
+-rw-r--r--   0 runner    (1001) docker     (116)      125 2022-10-18 16:09:03.000000 teststack-0.9.0/tests/testapp/Dockerfile.j2
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-18 16:09:13.927094 teststack-0.9.0/tests/testapp/app/
+-rw-r--r--   0 runner    (1001) docker     (116)      434 2022-10-18 16:09:03.000000 teststack-0.9.0/tests/testapp/app/application.py
+-rw-r--r--   0 runner    (1001) docker     (116)      907 2022-10-18 16:09:03.000000 teststack-0.9.0/tests/testapp/app/config.py
+-rw-r--r--   0 runner    (1001) docker     (116)      298 2022-10-18 16:09:03.000000 teststack-0.9.0/tests/testapp/app/database.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-18 16:09:13.923094 teststack-0.9.0/tests/testapp/app/handlers/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-18 16:09:13.927094 teststack-0.9.0/tests/testapp/app/handlers/v1/
+-rw-r--r--   0 runner    (1001) docker     (116)      188 2022-10-18 16:09:03.000000 teststack-0.9.0/tests/testapp/app/handlers/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      847 2022-10-18 16:09:03.000000 teststack-0.9.0/tests/testapp/app/handlers/v1/health.py
+-rw-r--r--   0 runner    (1001) docker     (116)    45335 2022-10-18 16:09:03.000000 teststack-0.9.0/tests/testapp/poetry.lock
+-rw-r--r--   0 runner    (1001) docker     (116)      899 2022-10-18 16:09:03.000000 teststack-0.9.0/tests/testapp/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-18 16:09:13.927094 teststack-0.9.0/tests/testapp/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)      172 2022-10-18 16:09:03.000000 teststack-0.9.0/tests/testapp/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-18 16:09:13.927094 teststack-0.9.0/tests/testapp/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (116)      148 2022-10-18 16:09:03.000000 teststack-0.9.0/tests/testapp/tests/unit/test_health.py
+-rw-r--r--   0 runner    (1001) docker     (116)      927 2022-10-18 16:09:03.000000 teststack-0.9.0/tests/testapp/teststack.toml
+-rw-r--r--   0 runner    (1001) docker     (116)       67 2022-10-18 16:09:03.000000 teststack-0.9.0/tests/testapp/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (116)      993 2022-10-18 16:09:03.000000 teststack-0.9.0/tests/teststack.podman.toml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-10-18 16:09:13.931094 teststack-0.9.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (116)      632 2022-10-18 16:09:03.000000 teststack-0.9.0/tests/unit/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7349 2022-10-18 16:09:03.000000 teststack-0.9.0/tests/unit/test_command_containers.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2021 2022-10-18 16:09:03.000000 teststack-0.9.0/tests/unit/test_command_env.py
+-rw-r--r--   0 runner    (1001) docker     (116)      185 2022-10-18 16:09:03.000000 teststack-0.9.0/tests/unit/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1019 2022-10-18 16:09:03.000000 teststack-0.9.0/teststack.toml
+-rw-r--r--   0 runner    (1001) docker     (116)      757 2022-10-18 16:09:03.000000 teststack-0.9.0/tox.ini
```

### Comparing `teststack-0.8.5/.github/workflows/codeql-analysis.yml` & `teststack-0.9.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `teststack-0.8.5/.github/workflows/publish.yml` & `teststack-0.9.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `teststack-0.8.5/.github/workflows/tests.yml` & `teststack-0.9.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `teststack-0.8.5/CODE_OF_CONDUCT.md` & `teststack-0.9.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `teststack-0.8.5/LICENSE` & `teststack-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `teststack-0.8.5/PKG-INFO` & `teststack-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teststack
-Version: 0.8.5
+Version: 0.9.0
 Summary: Manage the infrastructure for running tests against
 Home-page: https://github.com/gtmanfred/teststack
 Author: Daniel Wallace
 Author-email: daniel@gtmanfred.com
 License: APACHE-2.0
 Project-URL: Repository, https://github.com/gtmanfred/teststack
 Project-URL: Documentation, https://teststack.readthedocs.org
```

### Comparing `teststack-0.8.5/README.rst` & `teststack-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `teststack-0.8.5/docs/conf.py` & `teststack-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `teststack-0.8.5/docs/config.rst` & `teststack-0.9.0/docs/config.rst`

 * *Files identical despite different names*

### Comparing `teststack-0.8.5/docs/index.rst` & `teststack-0.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `teststack-0.8.5/docs/usage.rst` & `teststack-0.9.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `teststack-0.8.5/pyproject.toml` & `teststack-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `teststack-0.8.5/setup.cfg` & `teststack-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `teststack-0.8.5/src/teststack/__init__.py` & `teststack-0.9.0/src/teststack/__init__.py`

 * *Files identical despite different names*

### Comparing `teststack-0.8.5/src/teststack/commands/containers.py` & `teststack-0.9.0/src/teststack/commands/containers.py`

 * *Files 2% similar despite different names*

```diff
@@ -311,12 +311,27 @@
 
     steps = ctx.obj['tests'].get('steps', {})
     if step:
         commands = [steps.get(step, '{posargs}')]
     else:
         commands = steps.values()
     for command in commands:
+        user = None
         if isinstance(command, list):
             for cmd in command:
-                client.run_command(container, cmd.format(posargs=' '.join(posargs)))
+                if isinstance(cmd, dict):
+                    cmd, user = cmd['command'], cmd.get('user')
+                client.run_command(
+                    container,
+                    cmd.format(posargs=' '.join(posargs)),
+                    user=user,
+                )
+        elif isinstance(command, dict):
+            cmd, user = command['command'], command['user']
+
+            client.run_command(
+                container,
+                cmd.format(posargs=' '.join(posargs)),
+                user=user,
+            )
         else:
             client.run_command(container, command.format(posargs=' '.join(posargs)))
```

### Comparing `teststack-0.8.5/src/teststack/commands/environment.py` & `teststack-0.9.0/src/teststack/commands/environment.py`

 * *Files identical despite different names*

### Comparing `teststack-0.8.5/src/teststack/containers/docker.py` & `teststack-0.9.0/src/teststack/containers/docker.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,22 +84,23 @@
 
     def image_get(self, tag):
         try:
             return self.client.images.get(tag).id
         except docker.errors.ImageNotFound:
             return None
 
-    def run_command(self, container, command):
+    def run_command(self, container, command, user=None):
         container = self.client.containers.get(container)
         click.echo(click.style(f'Run Command: {command}', fg='green'))
         sock = container.exec_run(
             cmd=command,
             tty=True,
             stdin=True,
             socket=True,
+            user=user or '',
         ).output
 
         with read_from_stdin() as fd:
             if fd is not None:  # pragma: no cover
                 BREAK = False
                 while not BREAK:
                     reads, _, _ = select.select([sock._sock, fd], [], [], 0.0)
```

### Comparing `teststack-0.8.5/src/teststack/containers/podman.py` & `teststack-0.9.0/src/teststack/containers/podman.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,21 +155,22 @@
 
     def image_get(self, tag):
         try:
             return self.client.images.get(self._process_image_shortname(tag)).id
         except podman.errors.ImageNotFound:
             return None
 
-    def run_command(self, container, command):
+    def run_command(self, container, command, user=None):
         container = self.client.containers.get(container)
         click.echo(click.style(f'Run Command: {command}', fg='green'))
         socket = container.exec_run(
             cmd=command,
             tty=True,
             socket=True,
+            user=user,
         )
 
         for line in socket.output:
             click.echo(line, nl=False)
 
     def build(self, dockerfile, tag, rebuild):
         image, _ = self.client.images.build(path='.', dockerfile=dockerfile, tag=tag, nocache=rebuild, rm=True)
```

### Comparing `teststack-0.8.5/src/teststack/git.py` & `teststack-0.9.0/src/teststack/git.py`

 * *Files identical despite different names*

### Comparing `teststack-0.8.5/src/teststack/utils.py` & `teststack-0.9.0/src/teststack/utils.py`

 * *Files identical despite different names*

### Comparing `teststack-0.8.5/src/teststack.egg-info/PKG-INFO` & `teststack-0.9.0/src/teststack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teststack
-Version: 0.8.5
+Version: 0.9.0
 Summary: Manage the infrastructure for running tests against
 Home-page: https://github.com/gtmanfred/teststack
 Author: Daniel Wallace
 Author-email: daniel@gtmanfred.com
 License: APACHE-2.0
 Project-URL: Repository, https://github.com/gtmanfred/teststack
 Project-URL: Documentation, https://teststack.readthedocs.org
```

### Comparing `teststack-0.8.5/src/teststack.egg-info/SOURCES.txt` & `teststack-0.9.0/src/teststack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `teststack-0.8.5/tests/conftest.py` & `teststack-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `teststack-0.8.5/tests/files/build.output` & `teststack-0.9.0/tests/files/build.output`

 * *Files identical despite different names*

### Comparing `teststack-0.8.5/tests/integration/test_containers.py` & `teststack-0.9.0/tests/integration/test_containers.py`

 * *Files identical despite different names*

### Comparing `teststack-0.8.5/tests/testapp/app/config.py` & `teststack-0.9.0/tests/testapp/app/config.py`

 * *Files identical despite different names*

### Comparing `teststack-0.8.5/tests/testapp/app/handlers/v1/health.py` & `teststack-0.9.0/tests/testapp/app/handlers/v1/health.py`

 * *Files identical despite different names*

### Comparing `teststack-0.8.5/tests/testapp/poetry.lock` & `teststack-0.9.0/tests/testapp/poetry.lock`

 * *Files identical despite different names*

### Comparing `teststack-0.8.5/tests/testapp/pyproject.toml` & `teststack-0.9.0/tests/testapp/pyproject.toml`

 * *Files identical despite different names*

### Comparing `teststack-0.8.5/tests/testapp/teststack.toml` & `teststack-0.9.0/tests/testapp/teststack.toml`

 * *Files identical despite different names*

### Comparing `teststack-0.8.5/tests/teststack.podman.toml` & `teststack-0.9.0/tests/teststack.podman.toml`

 * *Files identical despite different names*

### Comparing `teststack-0.8.5/tests/unit/test_cli.py` & `teststack-0.9.0/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `teststack-0.8.5/tests/unit/test_command_containers.py` & `teststack-0.9.0/tests/unit/test_command_containers.py`

 * *Files identical despite different names*

### Comparing `teststack-0.8.5/tests/unit/test_command_env.py` & `teststack-0.9.0/tests/unit/test_command_env.py`

 * *Files identical despite different names*

### Comparing `teststack-0.8.5/teststack.toml` & `teststack-0.9.0/teststack.toml`

 * *Files identical despite different names*

### Comparing `teststack-0.8.5/tox.ini` & `teststack-0.9.0/tox.ini`

 * *Files identical despite different names*

