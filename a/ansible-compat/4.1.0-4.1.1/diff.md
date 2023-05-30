# Comparing `tmp/ansible-compat-4.1.0.tar.gz` & `tmp/ansible-compat-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-compat-4.1.0.tar", last modified: Wed May 24 13:41:15 2023, max compression
+gzip compressed data, was "ansible-compat-4.1.1.tar", last modified: Tue May 30 11:49:11 2023, max compression
```

## Comparing `ansible-compat-4.1.0.tar` & `ansible-compat-4.1.1.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.346953 ansible-compat-4.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.322954 ansible-compat-4.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.322954 ansible-compat-4.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/.prettierrc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.322954 ansible-compat-4.1.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-24 13:41:15.346953 ansible-compat-4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/ansible.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.322954 ansible-compat-4.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/docs/api.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.326954 ansible-compat-4.1.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/docs/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.302954 ansible-compat-4.1.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.326954 ansible-compat-4.1.0/examples/reqs_broken/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/examples/reqs_broken/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.326954 ansible-compat-4.1.0/examples/reqs_v1/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/examples/reqs_v1/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.326954 ansible-compat-4.1.0/examples/reqs_v2/
--rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/examples/reqs_v2/community-molecule-0.1.0.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/examples/reqs_v2/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 13:41:15.346953 ansible-compat-4.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.302954 ansible-compat-4.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.330954 ansible-compat-4.1.0/src/ansible_compat/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/src/ansible_compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/src/ansible_compat/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/src/ansible_compat/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/src/ansible_compat/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/src/ansible_compat/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/src/ansible_compat/ports.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/src/ansible_compat/prerun.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/src/ansible_compat/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34257 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/src/ansible_compat/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/src/ansible_compat/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/src/ansible_compat/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.334954 ansible-compat-4.1.0/src/ansible_compat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-24 13:41:15.000000 ansible-compat-4.1.0/src/ansible_compat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-24 13:41:15.000000 ansible-compat-4.1.0/src/ansible_compat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:41:15.000000 ansible-compat-4.1.0/src/ansible_compat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-24 13:41:15.000000 ansible-compat-4.1.0/src/ansible_compat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-24 13:41:15.000000 ansible-compat-4.1.0/src/ansible_compat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.338954 ansible-compat-4.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.342954 ansible-compat-4.1.0/test/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/assets/requirements-invalid-collection.yml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/assets/requirements-invalid-role.yml
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/assets/validate0_data.json
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/assets/validate0_expected.json
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/assets/validate0_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.302954 ansible-compat-4.1.0/test/collections/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.342954 ansible-compat-4.1.0/test/collections/acme.broken/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/collections/acme.broken/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.342954 ansible-compat-4.1.0/test/collections/acme.goodies/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/collections/acme.goodies/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.306954 ansible-compat-4.1.0/test/collections/acme.goodies/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.342954 ansible-compat-4.1.0/test/collections/acme.goodies/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/collections/acme.goodies/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/collections/acme.goodies/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.306954 ansible-compat-4.1.0/test/collections/acme.goodies/roles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.306954 ansible-compat-4.1.0/test/collections/acme.goodies/roles/baz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.306954 ansible-compat-4.1.0/test/collections/acme.goodies/roles/baz/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.342954 ansible-compat-4.1.0/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.342954 ansible-compat-4.1.0/test/collections/acme.goodies/roles/baz/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/collections/acme.goodies/roles/baz/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.342954 ansible-compat-4.1.0/test/collections/acme.goodies/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/collections/acme.goodies/tests/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.310954 ansible-compat-4.1.0/test/roles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.346953 ansible-compat-4.1.0/test/roles/acme.missing_deps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.346953 ansible-compat-4.1.0/test/roles/acme.missing_deps/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/roles/acme.missing_deps/meta/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/roles/acme.missing_deps/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.310954 ansible-compat-4.1.0/test/roles/acme.sample2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.346953 ansible-compat-4.1.0/test/roles/acme.sample2/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/roles/acme.sample2/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.310954 ansible-compat-4.1.0/test/roles/ansible-role-sample/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.346953 ansible-compat-4.1.0/test/roles/ansible-role-sample/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/roles/ansible-role-sample/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.310954 ansible-compat-4.1.0/test/roles/sample3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.346953 ansible-compat-4.1.0/test/roles/sample3/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/roles/sample3/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.310954 ansible-compat-4.1.0/test/roles/sample4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:41:15.346953 ansible-compat-4.1.0/test/roles/sample4/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/roles/sample4/meta/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/test_configuration_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/test_prerun.py
--rw-r--r--   0 runner    (1001) docker     (123)    27639 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/test_runtime_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/test/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-05-24 13:40:59.000000 ansible-compat-4.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.425784 ansible-compat-4.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.417784 ansible-compat-4.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.421784 ansible-compat-4.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/.prettierrc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.421784 ansible-compat-4.1.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-30 11:49:11.425784 ansible-compat-4.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/ansible.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.421784 ansible-compat-4.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/docs/api.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.421784 ansible-compat-4.1.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/docs/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.413784 ansible-compat-4.1.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.421784 ansible-compat-4.1.1/examples/reqs_broken/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/examples/reqs_broken/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.421784 ansible-compat-4.1.1/examples/reqs_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/examples/reqs_v1/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.421784 ansible-compat-4.1.1/examples/reqs_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/examples/reqs_v2/community-molecule-0.1.0.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/examples/reqs_v2/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 11:49:11.425784 ansible-compat-4.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.413784 ansible-compat-4.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.421784 ansible-compat-4.1.1/src/ansible_compat/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/src/ansible_compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/src/ansible_compat/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/src/ansible_compat/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/src/ansible_compat/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/src/ansible_compat/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/src/ansible_compat/ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/src/ansible_compat/prerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/src/ansible_compat/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    34516 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/src/ansible_compat/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/src/ansible_compat/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/src/ansible_compat/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.421784 ansible-compat-4.1.1/src/ansible_compat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-30 11:49:11.000000 ansible-compat-4.1.1/src/ansible_compat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-30 11:49:11.000000 ansible-compat-4.1.1/src/ansible_compat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:49:11.000000 ansible-compat-4.1.1/src/ansible_compat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-30 11:49:11.000000 ansible-compat-4.1.1/src/ansible_compat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-30 11:49:11.000000 ansible-compat-4.1.1/src/ansible_compat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.425784 ansible-compat-4.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.425784 ansible-compat-4.1.1/test/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/test/assets/requirements-invalid-collection.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/test/assets/requirements-invalid-role.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/test/assets/validate0_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/test/assets/validate0_expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/test/assets/validate0_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.413784 ansible-compat-4.1.1/test/collections/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.425784 ansible-compat-4.1.1/test/collections/acme.broken/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/test/collections/acme.broken/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.425784 ansible-compat-4.1.1/test/collections/acme.goodies/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/test/collections/acme.goodies/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.413784 ansible-compat-4.1.1/test/collections/acme.goodies/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.425784 ansible-compat-4.1.1/test/collections/acme.goodies/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/test/collections/acme.goodies/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/test/collections/acme.goodies/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.413784 ansible-compat-4.1.1/test/collections/acme.goodies/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.413784 ansible-compat-4.1.1/test/collections/acme.goodies/roles/baz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.413784 ansible-compat-4.1.1/test/collections/acme.goodies/roles/baz/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.425784 ansible-compat-4.1.1/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.425784 ansible-compat-4.1.1/test/collections/acme.goodies/roles/baz/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/test/collections/acme.goodies/roles/baz/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.425784 ansible-compat-4.1.1/test/collections/acme.goodies/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/test/collections/acme.goodies/tests/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.413784 ansible-compat-4.1.1/test/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.425784 ansible-compat-4.1.1/test/roles/acme.missing_deps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.425784 ansible-compat-4.1.1/test/roles/acme.missing_deps/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/test/roles/acme.missing_deps/meta/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/test/roles/acme.missing_deps/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.413784 ansible-compat-4.1.1/test/roles/acme.sample2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.425784 ansible-compat-4.1.1/test/roles/acme.sample2/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/test/roles/acme.sample2/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.413784 ansible-compat-4.1.1/test/roles/ansible-role-sample/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.425784 ansible-compat-4.1.1/test/roles/ansible-role-sample/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/test/roles/ansible-role-sample/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.413784 ansible-compat-4.1.1/test/roles/sample3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.425784 ansible-compat-4.1.1/test/roles/sample3/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/test/roles/sample3/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.413784 ansible-compat-4.1.1/test/roles/sample4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:49:11.425784 ansible-compat-4.1.1/test/roles/sample4/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/test/roles/sample4/meta/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/test/test_configuration_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/test/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/test/test_prerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27639 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/test/test_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/test/test_runtime_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/test/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-05-30 11:48:54.000000 ansible-compat-4.1.1/tox.ini
```

### Comparing `ansible-compat-4.1.0/.github/dependabot.yml` & `ansible-compat-4.1.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.0/.github/workflows/release.yml` & `ansible-compat-4.1.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.0/.github/workflows/tox.yml` & `ansible-compat-4.1.1/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.0/.gitignore` & `ansible-compat-4.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.0/.pre-commit-config.yaml` & `ansible-compat-4.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.0/.readthedocs.yml` & `ansible-compat-4.1.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.0/.vscode/settings.json` & `ansible-compat-4.1.1/.vscode/settings.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9967948717948717%*

 * *Differences: {"'[python]'": "{'editor.codeActionsOnSave': {'source.fixAll.ruff': False}}"}*

```diff
@@ -1,14 +1,15 @@
 {
     "[markdown]": {
         "editor.defaultFormatter": "esbenp.prettier-vscode"
     },
     "[python]": {
         "editor.codeActionsOnSave": {
             "source.fixAll": true,
+            "source.fixAll.ruff": false,
             "source.organizeImports": false
         }
     },
     "editor.formatOnSave": true,
     "evenBetterToml.formatter.alignComments": false,
     "evenBetterToml.formatter.allowedBlankLines": 2,
     "files.exclude": {
```

### Comparing `ansible-compat-4.1.0/LICENSE` & `ansible-compat-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.0/PKG-INFO` & `ansible-compat-4.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-compat
-Version: 4.1.0
+Version: 4.1.1
 Summary: Ansible compatibility goodies
 Author-email: Sorin Sbarnea <ssbarnea@redhat.com>
 Maintainer-email: Sorin Sbarnea <ssbarnea@redhat.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible/ansible-compat
 Project-URL: documentation, https://ansible-compat.readthedocs.io/
 Project-URL: repository, https://github.com/ansible/ansible-compat
```

### Comparing `ansible-compat-4.1.0/README.md` & `ansible-compat-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.0/docs/images/favicon.ico` & `ansible-compat-4.1.1/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.0/docs/images/logo.png` & `ansible-compat-4.1.1/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.0/docs/images/logo.svg` & `ansible-compat-4.1.1/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.0/examples/reqs_v2/community-molecule-0.1.0.tar.gz` & `ansible-compat-4.1.1/examples/reqs_v2/community-molecule-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.0/mkdocs.yml` & `ansible-compat-4.1.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.0/pyproject.toml` & `ansible-compat-4.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.0/requirements.txt` & `ansible-compat-4.1.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.0/src/ansible_compat/config.py` & `ansible-compat-4.1.1/src/ansible_compat/config.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.0/src/ansible_compat/constants.py` & `ansible-compat-4.1.1/src/ansible_compat/constants.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.0/src/ansible_compat/errors.py` & `ansible-compat-4.1.1/src/ansible_compat/errors.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.0/src/ansible_compat/loaders.py` & `ansible-compat-4.1.1/src/ansible_compat/loaders.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.0/src/ansible_compat/prerun.py` & `ansible-compat-4.1.1/src/ansible_compat/prerun.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.0/src/ansible_compat/runtime.py` & `ansible-compat-4.1.1/src/ansible_compat/runtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,33 +323,38 @@
         :param retry: Retry network operations on failures.
         :param tee: Also pass captured stdout/stderr to system while running.
         """
         if tee:
             run_func: Callable[..., CompletedProcess] = subprocess_tee.run
         else:
             run_func = subprocess.run
+        env = self.environ if env is None else env.copy()
+        # Presence of ansible debug variable or config option will prevent us
+        # from parsing its JSON output due to extra debug messages on stdout.
+        env["ANSIBLE_DEBUG"] = "0"
 
         for _ in range(self.max_retries + 1 if retry else 1):
             result = run_func(
                 args,
                 universal_newlines=True,
                 check=False,
                 stdout=subprocess.PIPE,
                 stderr=subprocess.PIPE,
-                env=env or self.environ,
+                env=env,
                 cwd=str(cwd) if cwd else None,
             )
             if result.returncode == 0:
                 break
-            _logger.debug("Environment: %s", env or self.environ)
-            _logger.warning(
-                "Retrying execution failure %s of: %s",
-                result.returncode,
-                " ".join(args),
-            )
+            _logger.debug("Environment: %s", env)
+            if retry:
+                _logger.warning(
+                    "Retrying execution failure %s of: %s",
+                    result.returncode,
+                    " ".join(args),
+                )
         return result
 
     @property
     def version(self) -> Version:
         """Return current Version object for Ansible.
 
         If version is not mentioned, it returns current version as detected.
```

### Comparing `ansible-compat-4.1.0/src/ansible_compat/schema.py` & `ansible-compat-4.1.1/src/ansible_compat/schema.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.0/src/ansible_compat/types.py` & `ansible-compat-4.1.1/src/ansible_compat/types.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.0/src/ansible_compat.egg-info/PKG-INFO` & `ansible-compat-4.1.1/src/ansible_compat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-compat
-Version: 4.1.0
+Version: 4.1.1
 Summary: Ansible compatibility goodies
 Author-email: Sorin Sbarnea <ssbarnea@redhat.com>
 Maintainer-email: Sorin Sbarnea <ssbarnea@redhat.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible/ansible-compat
 Project-URL: documentation, https://ansible-compat.readthedocs.io/
 Project-URL: repository, https://github.com/ansible/ansible-compat
```

### Comparing `ansible-compat-4.1.0/src/ansible_compat.egg-info/SOURCES.txt` & `ansible-compat-4.1.1/src/ansible_compat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.0/test/assets/validate0_expected.json` & `ansible-compat-4.1.1/test/assets/validate0_expected.json`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.0/test/collections/acme.goodies/galaxy.yml` & `ansible-compat-4.1.1/test/collections/acme.goodies/galaxy.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.0/test/conftest.py` & `ansible-compat-4.1.1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.0/test/test_config.py` & `ansible-compat-4.1.1/test/test_config.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.0/test/test_runtime.py` & `ansible-compat-4.1.1/test/test_runtime.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.0/test/test_runtime_example.py` & `ansible-compat-4.1.1/test/test_runtime_example.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.0/test/test_schema.py` & `ansible-compat-4.1.1/test/test_schema.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.0/tox.ini` & `ansible-compat-4.1.1/tox.ini`

 * *Files identical despite different names*

