# Comparing `tmp/craft-archives-1.0.0.tar.gz` & `tmp/craft-archives-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "craft-archives-1.0.0.tar", last modified: Wed May 24 18:13:32 2023, max compression
+gzip compressed data, was "craft-archives-1.1.0.tar", last modified: Tue May 30 17:09:56 2023, max compression
```

## Comparing `craft-archives-1.0.0.tar` & `craft-archives-1.1.0.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.593578 craft-archives-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-24 18:13:15.000000 craft-archives-1.0.0/.codespell_ignore_lines
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-24 18:13:15.000000 craft-archives-1.0.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.585578 craft-archives-1.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-24 18:13:15.000000 craft-archives-1.0.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-24 18:13:15.000000 craft-archives-1.0.0/.github/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-24 18:13:15.000000 craft-archives-1.0.0/.github/renovate.json5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.585578 craft-archives-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-24 18:13:15.000000 craft-archives-1.0.0/.github/workflows/cla-check.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-24 18:13:15.000000 craft-archives-1.0.0/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-24 18:13:15.000000 craft-archives-1.0.0/.github/workflows/release-drafter.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-24 18:13:15.000000 craft-archives-1.0.0/.github/workflows/release-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-24 18:13:15.000000 craft-archives-1.0.0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-24 18:13:15.000000 craft-archives-1.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-24 18:13:15.000000 craft-archives-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-24 18:13:15.000000 craft-archives-1.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 18:13:15.000000 craft-archives-1.0.0/.yamlignore
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-24 18:13:15.000000 craft-archives-1.0.0/.yamllint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-05-24 18:13:15.000000 craft-archives-1.0.0/HACKING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-24 18:13:15.000000 craft-archives-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-24 18:13:32.593578 craft-archives-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-24 18:13:15.000000 craft-archives-1.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.585578 craft-archives-1.0.0/craft_archives/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-24 18:13:15.000000 craft-archives-1.0.0/craft_archives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-24 18:13:32.000000 craft-archives-1.0.0/craft_archives/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-24 18:13:15.000000 craft-archives-1.0.0/craft_archives/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.585578 craft-archives-1.0.0/craft_archives/repo/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-24 18:13:15.000000 craft-archives-1.0.0/craft_archives/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10433 2023-05-24 18:13:15.000000 craft-archives-1.0.0/craft_archives/repo/apt_key_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-24 18:13:15.000000 craft-archives-1.0.0/craft_archives/repo/apt_ppa.py
--rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-05-24 18:13:15.000000 craft-archives-1.0.0/craft_archives/repo/apt_preferences_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-05-24 18:13:15.000000 craft-archives-1.0.0/craft_archives/repo/apt_sources_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-24 18:13:15.000000 craft-archives-1.0.0/craft_archives/repo/apt_uca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-24 18:13:15.000000 craft-archives-1.0.0/craft_archives/repo/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-05-24 18:13:15.000000 craft-archives-1.0.0/craft_archives/repo/installer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11312 2023-05-24 18:13:15.000000 craft-archives-1.0.0/craft_archives/repo/package_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-24 18:13:15.000000 craft-archives-1.0.0/craft_archives/repo/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-05-24 18:13:15.000000 craft-archives-1.0.0/craft_archives/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.585578 craft-archives-1.0.0/craft_archives.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-24 18:13:32.000000 craft-archives-1.0.0/craft_archives.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-24 18:13:32.000000 craft-archives-1.0.0/craft_archives.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 18:13:32.000000 craft-archives-1.0.0/craft_archives.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-24 18:13:32.000000 craft-archives-1.0.0/craft_archives.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-24 18:13:32.000000 craft-archives-1.0.0/craft_archives.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.589578 craft-archives-1.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.581578 craft-archives-1.0.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.589578 craft-archives-1.0.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-24 18:13:15.000000 craft-archives-1.0.0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-24 18:13:15.000000 craft-archives-1.0.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-24 18:13:15.000000 craft-archives-1.0.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.589578 craft-archives-1.0.0/docs/explanation/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-24 18:13:15.000000 craft-archives-1.0.0/docs/explanation/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.589578 craft-archives-1.0.0/docs/howto/
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-24 18:13:15.000000 craft-archives-1.0.0/docs/howto/add_repo.rst
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-24 18:13:15.000000 craft-archives-1.0.0/docs/howto/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-24 18:13:15.000000 craft-archives-1.0.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.589578 craft-archives-1.0.0/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-24 18:13:15.000000 craft-archives-1.0.0/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-05-24 18:13:15.000000 craft-archives-1.0.0/docs/reference/repo_properties.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.589578 craft-archives-1.0.0/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-24 18:13:15.000000 craft-archives-1.0.0/docs/tutorials/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-05-24 18:13:15.000000 craft-archives-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 18:13:32.593578 craft-archives-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.589578 craft-archives-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.589578 craft-archives-1.0.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.589578 craft-archives-1.0.0/tests/integration/repo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/integration/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/integration/repo/test_apt_key_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/integration/repo/test_installer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.589578 craft-archives-1.0.0/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/test_data/FC42E99D.asc
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/test_data/empty.preferences
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/test_data/expected.preferences
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/test_data/many_blank_lines.preferences
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/test_data/no_header.preferences
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/test_data/only_comment.preferences
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/test_data/with_header.preferences
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.589578 craft-archives-1.0.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:32.593578 craft-archives-1.0.0/tests/unit/repo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/unit/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/unit/repo/test_apt_key_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/unit/repo/test_apt_ppa.py
--rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/unit/repo/test_apt_preferences_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/unit/repo/test_apt_sources_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/unit/repo/test_apt_uca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/unit/repo/test_installer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16191 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/unit/repo/test_package_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tests/unit/repo/test_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-05-24 18:13:15.000000 craft-archives-1.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.202324 craft-archives-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-30 17:09:37.000000 craft-archives-1.1.0/.codespell_ignore_lines
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-30 17:09:37.000000 craft-archives-1.1.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.190324 craft-archives-1.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-30 17:09:37.000000 craft-archives-1.1.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-30 17:09:37.000000 craft-archives-1.1.0/.github/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-30 17:09:37.000000 craft-archives-1.1.0/.github/renovate.json5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.190324 craft-archives-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-30 17:09:37.000000 craft-archives-1.1.0/.github/workflows/cla-check.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-30 17:09:37.000000 craft-archives-1.1.0/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-30 17:09:37.000000 craft-archives-1.1.0/.github/workflows/release-drafter.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-30 17:09:37.000000 craft-archives-1.1.0/.github/workflows/release-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-05-30 17:09:37.000000 craft-archives-1.1.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-30 17:09:37.000000 craft-archives-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-30 17:09:37.000000 craft-archives-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-30 17:09:37.000000 craft-archives-1.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 17:09:37.000000 craft-archives-1.1.0/.yamlignore
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-30 17:09:37.000000 craft-archives-1.1.0/.yamllint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-05-30 17:09:37.000000 craft-archives-1.1.0/HACKING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-30 17:09:37.000000 craft-archives-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-30 17:09:56.202324 craft-archives-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-30 17:09:37.000000 craft-archives-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.194324 craft-archives-1.1.0/craft_archives/
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-30 17:09:37.000000 craft-archives-1.1.0/craft_archives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-30 17:09:56.000000 craft-archives-1.1.0/craft_archives/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-30 17:09:37.000000 craft-archives-1.1.0/craft_archives/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.194324 craft-archives-1.1.0/craft_archives/repo/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-30 17:09:37.000000 craft-archives-1.1.0/craft_archives/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10863 2023-05-30 17:09:37.000000 craft-archives-1.1.0/craft_archives/repo/apt_key_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-30 17:09:37.000000 craft-archives-1.1.0/craft_archives/repo/apt_ppa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6318 2023-05-30 17:09:37.000000 craft-archives-1.1.0/craft_archives/repo/apt_preferences_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10621 2023-05-30 17:09:37.000000 craft-archives-1.1.0/craft_archives/repo/apt_sources_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-30 17:09:37.000000 craft-archives-1.1.0/craft_archives/repo/apt_uca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-30 17:09:37.000000 craft-archives-1.1.0/craft_archives/repo/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-05-30 17:09:37.000000 craft-archives-1.1.0/craft_archives/repo/installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11312 2023-05-30 17:09:37.000000 craft-archives-1.1.0/craft_archives/repo/package_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-30 17:09:37.000000 craft-archives-1.1.0/craft_archives/repo/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-05-30 17:09:37.000000 craft-archives-1.1.0/craft_archives/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.194324 craft-archives-1.1.0/craft_archives.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-30 17:09:56.000000 craft-archives-1.1.0/craft_archives.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-30 17:09:56.000000 craft-archives-1.1.0/craft_archives.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 17:09:56.000000 craft-archives-1.1.0/craft_archives.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-30 17:09:56.000000 craft-archives-1.1.0/craft_archives.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-30 17:09:56.000000 craft-archives-1.1.0/craft_archives.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.194324 craft-archives-1.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.190324 craft-archives-1.1.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.194324 craft-archives-1.1.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-30 17:09:37.000000 craft-archives-1.1.0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-30 17:09:37.000000 craft-archives-1.1.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-30 17:09:37.000000 craft-archives-1.1.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.194324 craft-archives-1.1.0/docs/explanation/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-30 17:09:37.000000 craft-archives-1.1.0/docs/explanation/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.198324 craft-archives-1.1.0/docs/howto/
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-30 17:09:37.000000 craft-archives-1.1.0/docs/howto/add_repo.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-30 17:09:37.000000 craft-archives-1.1.0/docs/howto/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-30 17:09:37.000000 craft-archives-1.1.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.198324 craft-archives-1.1.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-30 17:09:37.000000 craft-archives-1.1.0/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-05-30 17:09:37.000000 craft-archives-1.1.0/docs/reference/repo_properties.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.198324 craft-archives-1.1.0/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-30 17:09:37.000000 craft-archives-1.1.0/docs/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-05-30 17:09:37.000000 craft-archives-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 17:09:56.202324 craft-archives-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.198324 craft-archives-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.198324 craft-archives-1.1.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.198324 craft-archives-1.1.0/tests/integration/repo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/integration/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/integration/repo/test_apt_key_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/integration/repo/test_installer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.198324 craft-archives-1.1.0/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/test_data/FC42E99D.asc
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/test_data/empty.preferences
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/test_data/expected.preferences
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/test_data/many_blank_lines.preferences
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/test_data/no_header.preferences
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/test_data/only_comment.preferences
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/test_data/with_header.preferences
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.198324 craft-archives-1.1.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:56.202324 craft-archives-1.1.0/tests/unit/repo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/unit/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14026 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/unit/repo/test_apt_key_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/unit/repo/test_apt_ppa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/unit/repo/test_apt_preferences_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8974 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/unit/repo/test_apt_sources_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/unit/repo/test_apt_uca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/unit/repo/test_installer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16191 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/unit/repo/test_package_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tests/unit/repo/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-05-30 17:09:37.000000 craft-archives-1.1.0/tox.ini
```

### Comparing `craft-archives-1.0.0/.editorconfig` & `craft-archives-1.1.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `craft-archives-1.0.0/.github/renovate.json5` & `craft-archives-1.1.0/.github/renovate.json5`

 * *Files identical despite different names*

### Comparing `craft-archives-1.0.0/.github/workflows/docs.yaml` & `craft-archives-1.1.0/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `craft-archives-1.0.0/.github/workflows/release-drafter.yaml` & `craft-archives-1.1.0/.github/workflows/release-drafter.yaml`

 * *Files identical despite different names*

### Comparing `craft-archives-1.0.0/.github/workflows/release-publish.yaml` & `craft-archives-1.1.0/.github/workflows/release-publish.yaml`

 * *Files identical despite different names*

### Comparing `craft-archives-1.0.0/.github/workflows/tests.yaml` & `craft-archives-1.1.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `craft-archives-1.0.0/.gitignore` & `craft-archives-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `craft-archives-1.0.0/.pre-commit-config.yaml` & `craft-archives-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `craft-archives-1.0.0/HACKING.rst` & `craft-archives-1.1.0/HACKING.rst`

 * *Files identical despite different names*

### Comparing `craft-archives-1.0.0/LICENSE` & `craft-archives-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `craft-archives-1.0.0/PKG-INFO` & `craft-archives-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft-archives
-Version: 1.0.0
+Version: 1.1.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `craft-archives-1.0.0/README.rst` & `craft-archives-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `craft-archives-1.0.0/craft_archives/__init__.py` & `craft-archives-1.1.0/craft_archives/__init__.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.0.0/craft_archives/errors.py` & `craft-archives-1.1.0/craft_archives/errors.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.0.0/craft_archives/repo/__init__.py` & `craft-archives-1.1.0/craft_archives/repo/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """Package repository helpers."""
 
-from .installer import install
+from .installer import install, install_in_root
 from .projects import validate_repository
 
 __all__ = [
     "install",
+    "install_in_root",
     "validate_repository",
 ]
```

### Comparing `craft-archives-1.0.0/craft_archives/repo/apt_key_manager.py` & `craft-archives-1.1.0/craft_archives/repo/apt_key_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -117,14 +117,27 @@
 
         if key_path.exists():
             return key_path
 
         return None
 
     @classmethod
+    def keyrings_path_for_root(
+        cls, root: Optional[pathlib.Path] = None
+    ) -> pathlib.Path:
+        """Get the location for Apt keyrings with ``root`` as the system root.
+
+        :param root: The optional system root to consider, or None to assume the standard
+          system root "/".
+        """
+        if root is None:
+            return KEYRINGS_PATH
+        return root / "etc/apt/keyrings"
+
+    @classmethod
     def get_key_fingerprints(cls, *, key: str) -> List[str]:
         """List fingerprints found in specified key.
 
         :param key: Key data (string) to parse.
 
         :returns: List of key fingerprints/IDs.
         """
```

### Comparing `craft-archives-1.0.0/craft_archives/repo/apt_ppa.py` & `craft-archives-1.1.0/craft_archives/repo/apt_ppa.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.0.0/craft_archives/repo/apt_preferences_manager.py` & `craft-archives-1.1.0/craft_archives/repo/apt_preferences_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,14 +111,25 @@
         path: typing.Optional[Path] = None,
         header: str = _DEFAULT_HEADER,
     ) -> None:
         self._header = header
         self._path = path or _DEFAULT_PREFERENCES_FILE
         self._preferences: typing.List[Preference] = []
 
+    @classmethod
+    def preferences_path_for_root(cls, root: typing.Optional[Path] = None) -> Path:
+        """Get the location for the Apt preferences file with ``root`` as the system root.
+
+        :param root: The optional system root to consider, or None to assume the standard
+          system root "/".
+        """
+        if root is None:
+            return _DEFAULT_PREFERENCES_FILE
+        return root / "etc/apt/preferences.d/craft-archives"
+
     def read(self) -> None:
         """Read the preferences file and populate Preferences objects."""
         if not self._path.exists():
             logger.debug("No preferences read.")
             return
         paragraphs = self._path.read_text().split("\n\n")
         for paragraph in paragraphs:
```

### Comparing `craft-archives-1.0.0/craft_archives/repo/apt_sources_manager.py` & `craft-archives-1.1.0/craft_archives/repo/apt_sources_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from craft_archives import utils
 
 from . import apt_key_manager, apt_ppa, apt_uca, errors, package_repository
 
 logger = logging.getLogger(__name__)
 
 _DEFAULT_SOURCES_DIRECTORY = Path("/etc/apt/sources.list.d")
+_DEFAULT_SIGNED_BY_ROOT = Path("/")
 
 
 def _construct_deb822_source(  # noqa: PLR0913
     *,
     architectures: Optional[List[str]] = None,
     components: Optional[List[str]] = None,
     formats: Optional[List[str]] = None,
@@ -81,17 +82,39 @@
 
     # pylint: disable=too-few-public-methods
     def __init__(
         self,
         *,
         sources_list_d: Optional[Path] = None,
         keyrings_dir: Optional[Path] = None,
+        signed_by_root: Optional[Path] = None,
     ) -> None:
+        """Create a manager for Apt repository sources listings.
+
+        :param sources_list_d: The path to the directory containing the sources listings.
+        :param keyrings_dir: The path to the directory containing the (already installed)
+          keyrings.
+        :param signed_by_root: The path that should be considered as "system root" when
+          filling the "Signed-By" field in the sources listings. Used to configure an
+          Apt-based system that will eventually be chrooted into.
+        """
         self._sources_list_d = sources_list_d or _DEFAULT_SOURCES_DIRECTORY
         self._keyrings_dir = keyrings_dir or apt_key_manager.KEYRINGS_PATH
+        self._signed_by_root = signed_by_root or _DEFAULT_SIGNED_BY_ROOT
+
+    @classmethod
+    def sources_path_for_root(cls, root: Optional[Path] = None) -> Path:
+        """Get the location for Apt source listings with ``root`` as the system root.
+
+        :param root: The optional system root to consider, or None to assume the standard
+          system root "/".
+        """
+        if root is None:
+            return _DEFAULT_SOURCES_DIRECTORY
+        return root / "etc/apt/sources.list.d"
 
     def _install_sources(  # noqa: PLR0913
         self,
         *,
         architectures: Optional[List[str]] = None,
         components: Optional[List[str]] = None,
         formats: Optional[List[str]] = None,
@@ -106,14 +129,16 @@
         /etc/apt/sources.list.d/craft-<name>.sources
 
         :returns: True if configuration was changed.
         """
         if keyring_path and not keyring_path.is_file():
             raise errors.AptGPGKeyringError(keyring_path)
 
+        keyring_path = Path("/") / keyring_path.relative_to(self._signed_by_root)
+
         config = _construct_deb822_source(
             architectures=architectures,
             components=components,
             formats=formats,
             suites=suites,
             url=url,
             signed_by=keyring_path,
@@ -262,18 +287,21 @@
         if isinstance(package_repo, package_repository.PackageRepositoryAptUCA):
             return self._install_sources_uca(package_repo=package_repo)
 
         if isinstance(package_repo, package_repository.PackageRepositoryApt):
             changed = self._install_sources_apt(package_repo=package_repo)
             architectures = package_repo.architectures
             if changed and architectures:
-                _add_architecture(architectures)
+                _add_architecture(architectures, root=self._signed_by_root)
             return changed
 
         raise RuntimeError(f"unhandled package repository: {package_repository!r}")
 
 
-def _add_architecture(architectures: List[str]) -> None:
+def _add_architecture(architectures: List[str], root: Path) -> None:
     """Add package repository architecture."""
     for arch in architectures:
         logger.info(f"Add repository architecture: {arch}")
-        subprocess.run(["dpkg", "--add-architecture", arch], check=True)
+        subprocess.run(
+            ["dpkg", "--add-architecture", arch, "--root", str(root)],
+            check=True,
+        )
```

### Comparing `craft-archives-1.0.0/craft_archives/repo/apt_uca.py` & `craft-archives-1.1.0/craft_archives/repo/apt_uca.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.0.0/craft_archives/repo/errors.py` & `craft-archives-1.1.0/craft_archives/repo/errors.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.0.0/craft_archives/repo/installer.py` & `craft-archives-1.1.0/craft_archives/repo/installer.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """Package repository installer."""
 
 import pathlib
-from typing import Any, Dict, List
+from typing import Any, Dict, List, Optional
 
 from . import errors
 from .apt_key_manager import AptKeyManager
 from .apt_preferences_manager import AptPreferencesManager
 from .apt_sources_manager import AptSourcesManager
 from .package_repository import (
     PackageRepository,
@@ -37,17 +37,56 @@
     """Add package repositories to the host system.
 
     :param project_repositories: A list of package repositories to install.
     :param key_assets: The directory containing repository keys.
 
     :return: Whether a package list refresh is required.
     """
-    key_manager = AptKeyManager(key_assets=key_assets)
-    sources_manager = AptSourcesManager()
-    preferences_manager = AptPreferencesManager()
+    return _install_repos(
+        project_repositories=project_repositories, key_assets=key_assets
+    )
+
+
+def install_in_root(
+    project_repositories: List[Dict[str, Any]],
+    root: pathlib.Path,
+    *,
+    key_assets: pathlib.Path,
+) -> bool:
+    """Add package repositories to the system located at ``root``.
+
+    :param project_repositories: A list of package repositories to install.
+    :param key_assets: The directory containing repository keys.
+    :param root: The directory containing the Apt-based system installation.
+
+    :return: Whether a package list refresh is required.
+    """
+    return _install_repos(
+        project_repositories=project_repositories, root=root, key_assets=key_assets
+    )
+
+
+def _install_repos(
+    *,
+    project_repositories: List[Dict[str, Any]],
+    root: Optional[pathlib.Path] = None,
+    key_assets: pathlib.Path,
+) -> bool:
+    keyrings_path = AptKeyManager.keyrings_path_for_root(root)
+    key_manager = AptKeyManager(keyrings_path=keyrings_path, key_assets=key_assets)
+
+    sources_list_d = AptSourcesManager.sources_path_for_root(root)
+    sources_manager = AptSourcesManager(
+        sources_list_d=sources_list_d,
+        keyrings_dir=keyrings_path,
+        signed_by_root=root,
+    )
+
+    preferences_path = AptPreferencesManager.preferences_path_for_root(root)
+    preferences_manager = AptPreferencesManager(path=preferences_path)
 
     package_repositories = _unmarshal_repositories(project_repositories)
 
     refresh_required = False
     for package_repo in package_repositories:
         refresh_required |= key_manager.install_package_repository_key(
             package_repo=package_repo
```

### Comparing `craft-archives-1.0.0/craft_archives/repo/package_repository.py` & `craft-archives-1.1.0/craft_archives/repo/package_repository.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.0.0/craft_archives/repo/projects.py` & `craft-archives-1.1.0/craft_archives/repo/projects.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.0.0/craft_archives/utils.py` & `craft-archives-1.1.0/craft_archives/utils.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.0.0/craft_archives.egg-info/PKG-INFO` & `craft-archives-1.1.0/craft_archives.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craft-archives
-Version: 1.0.0
+Version: 1.1.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: POSIX :: Linux
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `craft-archives-1.0.0/craft_archives.egg-info/SOURCES.txt` & `craft-archives-1.1.0/craft_archives.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `craft-archives-1.0.0/docs/conf.py` & `craft-archives-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.0.0/docs/howto/add_repo.rst` & `craft-archives-1.1.0/docs/howto/add_repo.rst`

 * *Files identical despite different names*

### Comparing `craft-archives-1.0.0/docs/index.rst` & `craft-archives-1.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `craft-archives-1.0.0/docs/reference/repo_properties.rst` & `craft-archives-1.1.0/docs/reference/repo_properties.rst`

 * *Files identical despite different names*

### Comparing `craft-archives-1.0.0/pyproject.toml` & `craft-archives-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `craft-archives-1.0.0/tests/conftest.py` & `craft-archives-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.0.0/tests/integration/repo/test_apt_key_manager.py` & `craft-archives-1.1.0/tests/integration/repo/test_apt_key_manager.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.0.0/tests/integration/repo/test_installer.py` & `craft-archives-1.1.0/tests/integration/repo/test_installer.py`

 * *Files 12% similar despite different names*

```diff
@@ -83,33 +83,43 @@
     Pin: origin "ubuntu-cloud.archive.canonical.com"
     Pin-Priority: 123
 
     """
 ).lstrip()
 
 
+def create_etc_apt_dirs(etc_apt: Path):
+    etc_apt.mkdir(parents=True)
+
+    keyrings_dir = etc_apt / "keyrings"
+    keyrings_dir.mkdir()
+
+    sources_dir = etc_apt / "sources.list.d"
+    sources_dir.mkdir()
+
+    preferences_dir = etc_apt / "preferences.d"
+    preferences_dir.mkdir()
+
+
 @pytest.fixture
 def fake_etc_apt(tmp_path, mocker) -> Path:
     """Mock the default paths used to store keys, sources and preferences."""
     etc_apt = tmp_path / "etc/apt"
-    etc_apt.mkdir(parents=True)
+    create_etc_apt_dirs(etc_apt)
 
     keyrings_dir = etc_apt / "keyrings"
-    keyrings_dir.mkdir()
     mocker.patch("craft_archives.repo.apt_key_manager.KEYRINGS_PATH", new=keyrings_dir)
 
     sources_dir = etc_apt / "sources.list.d"
-    sources_dir.mkdir()
     mocker.patch(
         "craft_archives.repo.apt_sources_manager._DEFAULT_SOURCES_DIRECTORY",
         new=sources_dir,
     )
 
     preferences_dir = etc_apt / "preferences.d"
-    preferences_dir.mkdir()
     preferences_dir = preferences_dir / "craft-archives"
     mocker.patch(
         "craft_archives.repo.apt_preferences_manager._DEFAULT_PREFERENCES_FILE",
         new=preferences_dir,
     )
 
     return etc_apt
@@ -156,54 +166,68 @@
 
 def test_install(fake_etc_apt, all_repo_types, test_keys_dir):
     """Integrated test that checks the configuration of keys, sources and pins."""
 
     assert repo.install(project_repositories=all_repo_types, key_assets=test_keys_dir)
 
     check_keyrings(fake_etc_apt)
-    check_sources(fake_etc_apt)
+    check_sources(fake_etc_apt, signed_by_location=fake_etc_apt / "keyrings")
     check_preferences(fake_etc_apt)
 
 
+def test_install_in_root(tmp_path, all_repo_types, test_keys_dir):
+    """Integrated test that checks the configuration of keys, sources and pins."""
+    etc_apt = tmp_path / "etc/apt"
+    create_etc_apt_dirs(etc_apt)
+
+    assert repo.install_in_root(
+        project_repositories=all_repo_types, key_assets=test_keys_dir, root=tmp_path
+    )
+
+    check_keyrings(etc_apt)
+    check_sources(etc_apt, signed_by_location=Path("/etc/apt/keyrings"))
+    check_preferences(etc_apt)
+
+
 def check_keyrings(etc_apt_dir: Path) -> None:
     keyrings_dir = etc_apt_dir / "keyrings"
 
     # Must have exactly these keyring files, one for each repo
     expected_key_ids = ("6A755776", "FC42E99D", "EC4926EA")
 
     assert len(list(keyrings_dir.iterdir())) == len(expected_key_ids)
     for key_id in expected_key_ids:
         keyring_file = keyrings_dir / f"craft-{key_id}.gpg"
         assert keyring_file.is_file()
 
 
-def check_sources(etc_apt_dir: Path) -> None:
+def check_sources(etc_apt_dir: Path, signed_by_location: Path) -> None:
     sources_dir = etc_apt_dir / "sources.list.d"
 
-    keyrings_location = etc_apt_dir / "keyrings"
+    keyrings_on_fs = etc_apt_dir / "keyrings"
 
     cloud_name = CLOUD_DATA["cloud"]
     codename = CLOUD_DATA["codename"]
 
     # Must have exactly these sources files, one for each repo
     source_to_contents = {
         "http_ppa_launchpad_net_snappy_dev_snapcraft_daily_ubuntu": APT_SOURCES.format(
-            key_location=keyrings_location
+            key_location=signed_by_location
         ),
         "ppa-deadsnakes_ppa": PPA_SOURCES.format(
-            codename=VERSION_CODENAME, key_location=keyrings_location
+            codename=VERSION_CODENAME, key_location=signed_by_location
         ),
         f"cloud-{cloud_name}": CLOUD_SOURCES.format(
             cloud=cloud_name,
             codename=codename,
-            key_location=keyrings_location,
+            key_location=signed_by_location,
         ),
     }
 
-    assert len(list(keyrings_location.iterdir())) == len(source_to_contents)
+    assert len(list(keyrings_on_fs.iterdir())) == len(source_to_contents)
 
     for source_repo, expected_contents in source_to_contents.items():
         source_file = sources_dir / f"craft-{source_repo}.sources"
         assert source_file.is_file()
         assert source_file.read_text() == expected_contents
```

### Comparing `craft-archives-1.0.0/tests/test_data/FC42E99D.asc` & `craft-archives-1.1.0/tests/test_data/FC42E99D.asc`

 * *Files identical despite different names*

### Comparing `craft-archives-1.0.0/tests/unit/repo/test_apt_key_manager.py` & `craft-archives-1.1.0/tests/unit/repo/test_apt_key_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,20 +11,21 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 import logging
 import subprocess
+from pathlib import Path
 from unittest import mock
 from unittest.mock import call
 
 import pytest
 from craft_archives.repo import apt_ppa, errors, package_repository
-from craft_archives.repo.apt_key_manager import AptKeyManager
+from craft_archives.repo.apt_key_manager import KEYRINGS_PATH, AptKeyManager
 from craft_archives.repo.package_repository import (
     PackageRepositoryApt,
     PackageRepositoryAptPPA,
     PackageRepositoryAptUCA,
 )
 
 # pyright: reportGeneralTypeIssues=false
@@ -464,7 +465,14 @@
     package_repo = PackageRepositoryAptUCA(type="apt", cloud="antelope")
     updated = apt_gpg.install_package_repository_key(package_repo=package_repo)
 
     assert updated is True
     assert mock_install_key_from_keyserver.mock_calls == [
         call(key_id="FAKE-UCA-KEY-ID", key_server="keyserver.ubuntu.com")
     ]
+
+
+def test_keyrings_path_for_root():
+    assert AptKeyManager.keyrings_path_for_root() == KEYRINGS_PATH
+    assert AptKeyManager.keyrings_path_for_root(Path("/my/root")) == Path(
+        "/my/root/etc/apt/keyrings"
+    )
```

### Comparing `craft-archives-1.0.0/tests/unit/repo/test_apt_ppa.py` & `craft-archives-1.1.0/tests/unit/repo/test_apt_ppa.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.0.0/tests/unit/repo/test_apt_preferences_manager.py` & `craft-archives-1.1.0/tests/unit/repo/test_apt_preferences_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,20 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 """Tests for apt_preferencs_manager"""
 import shutil
+from pathlib import Path
 from textwrap import dedent
 
 import pytest
 from craft_archives.repo.apt_preferences_manager import (
+    _DEFAULT_PREFERENCES_FILE,
     AptPreferencesManager,
     Preference,
 )
 from craft_archives.repo.errors import AptPreferencesError
 
 VALID_PRIORITY_STRINGS = ("always", "prefer", "defer")
 VALID_PRIORITY_INTS = (1000, 990, 100, 500, 1, -1)
@@ -230,8 +232,17 @@
     for pref in preferences:
         manager.add(**pref)
     manager.write()
 
     assert actual_path.read_text() == expected_path.read_text()
 
 
+def test_preferences_path_for_root():
+    assert (
+        AptPreferencesManager.preferences_path_for_root() == _DEFAULT_PREFERENCES_FILE
+    )
+    assert AptPreferencesManager.preferences_path_for_root(Path("/my/root")) == Path(
+        "/my/root/etc/apt/preferences.d/craft-archives"
+    )
+
+
 # endregion
```

### Comparing `craft-archives-1.0.0/tests/unit/repo/test_apt_sources_manager.py` & `craft-archives-1.1.0/tests/unit/repo/test_apt_sources_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,21 +13,26 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 
 import http
 import urllib.error
+from pathlib import Path
 from textwrap import dedent
 from unittest import mock
 from unittest.mock import call, patch
 
 import distro
 import pytest
 from craft_archives.repo import apt_ppa, apt_sources_manager, errors
+from craft_archives.repo.apt_sources_manager import (
+    _DEFAULT_SOURCES_DIRECTORY,
+    AptSourcesManager,
+)
 from craft_archives.repo.package_repository import (
     PackageRepositoryApt,
     PackageRepositoryAptPPA,
     PackageRepositoryAptUCA,
 )
 
 # pyright: reportGeneralTypeIssues=false
@@ -71,18 +76,37 @@
 def apt_sources_mgr(tmp_path):
     sources_list_d = tmp_path / "sources.list.d"
     sources_list_d.mkdir(parents=True)
     keyrings_dir = tmp_path / "keyrings"
     keyrings_dir.mkdir(parents=True)
 
     yield apt_sources_manager.AptSourcesManager(
-        sources_list_d=sources_list_d, keyrings_dir=keyrings_dir
+        sources_list_d=sources_list_d,
+        keyrings_dir=keyrings_dir,
     )
 
 
+def create_apt_sources_mgr(tmp_path: Path, *, use_signed_by_root: bool):
+    signed_by_root = None
+    if use_signed_by_root:
+        signed_by_root = tmp_path
+
+    sources_list_d = tmp_path / "sources.list.d"
+    sources_list_d.mkdir(parents=True)
+    keyrings_dir = tmp_path / "keyrings"
+    keyrings_dir.mkdir(parents=True)
+
+    return apt_sources_manager.AptSourcesManager(
+        sources_list_d=sources_list_d,
+        keyrings_dir=keyrings_dir,
+        signed_by_root=signed_by_root,
+    )
+
+
+@pytest.mark.parametrize("use_signed_by_root", [False, True])
 @pytest.mark.parametrize(
     "package_repo,name,content_template",
     [
         (
             PackageRepositoryApt(
                 type="apt",
                 architectures=["amd64", "arm64"],
@@ -150,38 +174,66 @@
                 Architectures: FAKE-HOST-ARCH
                 Signed-By: {keyring_path}
                 """
             ),
         ),
     ],
 )
-def test_install(package_repo, name, content_template, apt_sources_mgr, mocker):
+def test_install(
+    tmp_path,
+    package_repo,
+    name,
+    content_template,
+    use_signed_by_root,
+    mocker,
+):
     run_mock = mocker.patch("subprocess.run")
     mocker.patch("urllib.request.urlopen")
+
+    apt_sources_mgr = create_apt_sources_mgr(
+        tmp_path, use_signed_by_root=use_signed_by_root
+    )
     sources_path = apt_sources_mgr._sources_list_d / name
 
     keyring_path = apt_sources_mgr._keyrings_dir / "craft-AAAAAAAA.gpg"
     keyring_path.touch(exist_ok=True)
-    content = content_template.format(keyring_path=keyring_path).encode()
+
+    if use_signed_by_root:
+        signed_by_path = "/keyrings/craft-AAAAAAAA.gpg"
+    else:
+        signed_by_path = str(keyring_path)
+
+    content = content_template.format(keyring_path=signed_by_path).encode()
     mock_keyring_path = mocker.patch(
         "craft_archives.repo.apt_key_manager.get_keyring_path"
     )
     mock_keyring_path.return_value = keyring_path
 
     changed = apt_sources_mgr.install_package_repository_sources(
         package_repo=package_repo
     )
 
     assert changed is True
     assert sources_path.read_bytes() == content
 
+    if use_signed_by_root:
+        expected_root = str(tmp_path)
+    else:
+        expected_root = "/"
+
     if isinstance(package_repo, PackageRepositoryApt) and package_repo.architectures:
         assert run_mock.mock_calls == [
-            call(["dpkg", "--add-architecture", "amd64"], check=True),
-            call(["dpkg", "--add-architecture", "arm64"], check=True),
+            call(
+                ["dpkg", "--add-architecture", "amd64", "--root", expected_root],
+                check=True,
+            ),
+            call(
+                ["dpkg", "--add-architecture", "arm64", "--root", expected_root],
+                check=True,
+            ),
         ]
     else:
         assert run_mock.mock_calls == []
 
     run_mock.reset_mock()
 
     # Verify a second-run does not incur any changes.
@@ -231,7 +283,14 @@
         type="apt",
         architectures=["amd64"],
         url="https://example.com",
         key_id="A" * 40,
     )
     with pytest.raises(errors.AptGPGKeyringError):
         apt_sources_mgr._install_sources_apt(package_repo=repo)
+
+
+def test_preferences_path_for_root():
+    assert AptSourcesManager.sources_path_for_root() == _DEFAULT_SOURCES_DIRECTORY
+    assert AptSourcesManager.sources_path_for_root(Path("/my/root")) == Path(
+        "/my/root/etc/apt/sources.list.d"
+    )
```

### Comparing `craft-archives-1.0.0/tests/unit/repo/test_apt_uca.py` & `craft-archives-1.1.0/tests/unit/repo/test_apt_uca.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.0.0/tests/unit/repo/test_package_repository.py` & `craft-archives-1.1.0/tests/unit/repo/test_package_repository.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.0.0/tests/unit/repo/test_projects.py` & `craft-archives-1.1.0/tests/unit/repo/test_projects.py`

 * *Files identical despite different names*

### Comparing `craft-archives-1.0.0/tox.ini` & `craft-archives-1.1.0/tox.ini`

 * *Files identical despite different names*

