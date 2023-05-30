# Comparing `tmp/ansible-runner-2.3.2.tar.gz` & `tmp/ansible-runner-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-runner-2.3.2.tar", last modified: Wed Mar  1 21:11:50 2023, max compression
+gzip compressed data, was "ansible-runner-2.3.3.tar", last modified: Tue May 30 15:45:54 2023, max compression
```

## Comparing `ansible-runner-2.3.2.tar` & `ansible-runner-2.3.3.tar`

### file list

```diff
@@ -1,317 +1,318 @@
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.527440 ansible-runner-2.3.2/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      209 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/.cherry_picker.toml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      287 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/.coveragerc
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        5 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/.dockerignore
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.514440 ansible-runner-2.3.2/.github/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      162 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/.github/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.515440 ansible-runner-2.3.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1939 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       27 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      611 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/.github/ISSUE_TEMPLATE/documentation_report.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      588 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       23 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/.github/issue_labeler.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      117 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/.github/patchback.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       37 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/.github/pr_labeler_existing.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       90 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/.github/pr_labeler_new.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.515440 ansible-runner-2.3.2/.github/workflows/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     3011 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/.github/workflows/ci.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      763 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/.github/workflows/triage_existing.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      734 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/.github/workflows/triage_new.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      114 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/.pre-commit-config.yaml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      334 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/.readthedocs.yaml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      466 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/.yamllint
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.515440 ansible-runner-2.3.2/.zuul.d/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     8029 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/.zuul.d/jobs.yaml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.515440 ansible-runner-2.3.2/.zuul.d/playbooks/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/.zuul.d/playbooks/.zuul.ignore
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.515440 ansible-runner-2.3.2/.zuul.d/playbooks/ansible-runner-container-image-base/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      331 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/.zuul.d/playbooks/ansible-runner-container-image-base/pre.yaml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      795 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/.zuul.d/project.yaml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     4288 2023-03-01 21:11:50.000000 ansible-runner-2.3.2/AUTHORS
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      306 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/CODEOWNERS
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1422 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/CONTRIBUTING.md
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)    49412 2023-03-01 21:11:50.000000 ansible-runner-2.3.2/ChangeLog
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     2547 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/Dockerfile
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     9304 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/LICENSE.md
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       55 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/MANIFEST.in
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     5345 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/Makefile
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     2441 2023-03-01 21:11:50.527440 ansible-runner-2.3.2/PKG-INFO
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     2044 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/README.md
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      313 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/SECURITY.md
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.516440 ansible-runner-2.3.2/ansible_runner/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      669 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/ansible_runner/__init__.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)    35722 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/ansible_runner/__main__.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     6609 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/ansible_runner/cleanup.py
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.517440 ansible-runner-2.3.2/ansible_runner/config/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/ansible_runner/config/__init__.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)    29029 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/ansible_runner/config/_base.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     3381 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/ansible_runner/config/ansible_cfg.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     4323 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/ansible_runner/config/command.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     6418 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/ansible_runner/config/doc.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     4897 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/ansible_runner/config/inventory.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)    17441 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/ansible_runner/config/runner.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      408 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/ansible_runner/defaults.py
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.517440 ansible-runner-2.3.2/ansible_runner/display_callback/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/ansible_runner/display_callback/__init__.py
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.517440 ansible-runner-2.3.2/ansible_runner/display_callback/callback/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/ansible_runner/display_callback/callback/__init__.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)    31150 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/ansible_runner/display_callback/callback/awx_display.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      256 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/ansible_runner/exceptions.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)    64207 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/ansible_runner/interface.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     5986 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/ansible_runner/loader.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     3008 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/ansible_runner/output.py
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.517440 ansible-runner-2.3.2/ansible_runner/plugins/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/ansible_runner/plugins/__init__.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)    25381 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/ansible_runner/runner.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      905 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/ansible_runner/runner_config.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)    14152 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/ansible_runner/streaming.py
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.518440 ansible-runner-2.3.2/ansible_runner/utils/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)    17031 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/ansible_runner/utils/__init__.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)    11731 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/ansible_runner/utils/base64io.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1719 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/ansible_runner/utils/capacity.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     4931 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/ansible_runner/utils/streaming.py
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.517440 ansible-runner-2.3.2/ansible_runner.egg-info/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     2441 2023-03-01 21:11:50.000000 ansible-runner-2.3.2/ansible_runner.egg-info/PKG-INFO
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     7411 2023-03-01 21:11:50.000000 ansible-runner-2.3.2/ansible_runner.egg-info/SOURCES.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        1 2023-03-01 21:11:50.000000 ansible-runner-2.3.2/ansible_runner.egg-info/dependency_links.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       64 2023-03-01 21:11:50.000000 ansible-runner-2.3.2/ansible_runner.egg-info/entry_points.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        1 2023-03-01 21:08:06.000000 ansible-runner-2.3.2/ansible_runner.egg-info/not-zip-safe
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       47 2023-03-01 21:11:50.000000 ansible-runner-2.3.2/ansible_runner.egg-info/pbr.json
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       48 2023-03-01 21:11:50.000000 ansible-runner-2.3.2/ansible_runner.egg-info/requires.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       15 2023-03-01 21:11:50.000000 ansible-runner-2.3.2/ansible_runner.egg-info/top_level.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      155 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/bindep.txt
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.509440 ansible-runner-2.3.2/demo/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.518440 ansible-runner-2.3.2/demo/env/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       18 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/demo/env/envvars
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       40 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/demo/env/extravars
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       39 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/demo/env/passwords
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       60 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/demo/env/settings
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/demo/env/ssh_key
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.518440 ansible-runner-2.3.2/demo/inventory/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       94 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/demo/inventory/hosts
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.518440 ansible-runner-2.3.2/demo/project/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.509440 ansible-runner-2.3.2/demo/project/roles/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.518440 ansible-runner-2.3.2/demo/project/roles/testrole/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1328 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/demo/project/roles/testrole/README.md
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.518440 ansible-runner-2.3.2/demo/project/roles/testrole/defaults/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       33 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/demo/project/roles/testrole/defaults/main.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.518440 ansible-runner-2.3.2/demo/project/roles/testrole/handlers/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       33 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/demo/project/roles/testrole/handlers/main.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.518440 ansible-runner-2.3.2/demo/project/roles/testrole/meta/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1767 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/demo/project/roles/testrole/meta/main.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.518440 ansible-runner-2.3.2/demo/project/roles/testrole/tasks/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      129 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/demo/project/roles/testrole/tasks/main.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.519440 ansible-runner-2.3.2/demo/project/roles/testrole/tests/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       11 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/demo/project/roles/testrole/tests/inventory
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       67 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/demo/project/roles/testrole/tests/test.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.519440 ansible-runner-2.3.2/demo/project/roles/testrole/vars/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       29 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/demo/project/roles/testrole/vars/main.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       51 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/demo/project/test.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.520440 ansible-runner-2.3.2/docs/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      611 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/docs/Makefile
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      225 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/docs/ansible_runner.config.rst
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      445 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/docs/ansible_runner.display_callback.rst
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1142 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/docs/ansible_runner.rst
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     5594 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/docs/conf.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1749 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/docs/container.rst
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     5153 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/docs/execution_environments.rst
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     2339 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/docs/external_interface.rst
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     2288 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/docs/index.rst
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1793 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/docs/install.rst
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)    18971 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/docs/intro.rst
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      818 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/docs/make.bat
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       97 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/docs/modules.rst
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)    17999 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/docs/python_interface.rst
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     4146 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/docs/remote_jobs.rst
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       36 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/docs/requirements.in
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      625 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/docs/requirements.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     5917 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/docs/standalone.rst
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.510440 ansible-runner-2.3.2/packaging/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.520440 ansible-runner-2.3.2/packaging/debian/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      129 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/packaging/debian/changelog
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        2 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/packaging/debian/compat
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      802 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/packaging/debian/control
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     9703 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/packaging/debian/copyright
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.520440 ansible-runner-2.3.2/packaging/debian/docker/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      302 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/packaging/debian/docker/Dockerfile
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      284 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/packaging/debian/docker/docker-compose.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       32 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/packaging/debian/pydist-overrides
--rwxr-xr-x   0 mdavis    (1000) mdavis    (1000)      264 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/packaging/debian/rules
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.520440 ansible-runner-2.3.2/packaging/debian/source/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       12 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/packaging/debian/source/format
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.521440 ansible-runner-2.3.2/packaging/rpm/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      236 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/packaging/rpm/Dockerfile.epel-7-x86_64
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      277 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/packaging/rpm/Dockerfile.epel-8-x86_64
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     4832 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/packaging/rpm/ansible-runner.spec.j2
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      460 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/packaging/rpm/docker-compose.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      339 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/pytest.ini
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       48 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/requirements.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      748 2023-03-01 21:11:50.528440 ansible-runner-2.3.2/setup.cfg
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      104 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/setup.py
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.521440 ansible-runner-2.3.2/test/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/__init__.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     2916 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/conftest.py
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.510440 ansible-runner-2.3.2/test/fixtures/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.511440 ansible-runner-2.3.2/test/fixtures/projects/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.521440 ansible-runner-2.3.2/test/fixtures/projects/collection_role/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.510440 ansible-runner-2.3.2/test/fixtures/projects/collection_role/collections/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.510440 ansible-runner-2.3.2/test/fixtures/projects/collection_role/collections/ansible_collections/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.510440 ansible-runner-2.3.2/test/fixtures/projects/collection_role/collections/ansible_collections/groovy/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.521440 ansible-runner-2.3.2/test/fixtures/projects/collection_role/collections/ansible_collections/groovy/peanuts/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/collection_role/collections/ansible_collections/groovy/peanuts/README.md
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      290 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/collection_role/collections/ansible_collections/groovy/peanuts/galaxy.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.510440 ansible-runner-2.3.2/test/fixtures/projects/collection_role/collections/ansible_collections/groovy/peanuts/roles/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.510440 ansible-runner-2.3.2/test/fixtures/projects/collection_role/collections/ansible_collections/groovy/peanuts/roles/hello/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.521440 ansible-runner-2.3.2/test/fixtures/projects/collection_role/collections/ansible_collections/groovy/peanuts/roles/hello/tasks/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       34 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/collection_role/collections/ansible_collections/groovy/peanuts/roles/hello/tasks/main.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.521440 ansible-runner-2.3.2/test/fixtures/projects/collection_role/env/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       26 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/collection_role/env/envvars
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.521440 ansible-runner-2.3.2/test/fixtures/projects/collection_role/inventory/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      126 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/collection_role/inventory/hosts
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       74 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/collection_role/use_role.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.510440 ansible-runner-2.3.2/test/fixtures/projects/containerized/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.521440 ansible-runner-2.3.2/test/fixtures/projects/containerized/env/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       26 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/containerized/env/envvars
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       78 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/containerized/env/settings
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.521440 ansible-runner-2.3.2/test/fixtures/projects/containerized/inventory/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      126 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/containerized/inventory/hosts
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.521440 ansible-runner-2.3.2/test/fixtures/projects/containerized/project/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      266 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/containerized/project/test-container.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.510440 ansible-runner-2.3.2/test/fixtures/projects/debug/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.522440 ansible-runner-2.3.2/test/fixtures/projects/debug/env/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       26 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/debug/env/envvars
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.522440 ansible-runner-2.3.2/test/fixtures/projects/debug/inventory/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       91 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/debug/inventory/inv_1
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       91 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/debug/inventory/inv_2
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.522440 ansible-runner-2.3.2/test/fixtures/projects/debug/project/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       55 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/debug/project/debug.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.510440 ansible-runner-2.3.2/test/fixtures/projects/debug/project/roles/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.511440 ansible-runner-2.3.2/test/fixtures/projects/debug/project/roles/hello_world/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.522440 ansible-runner-2.3.2/test/fixtures/projects/debug/project/roles/hello_world/tasks/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       62 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/debug/project/roles/hello_world/tasks/main.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.511440 ansible-runner-2.3.2/test/fixtures/projects/directory_isolation/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.522440 ansible-runner-2.3.2/test/fixtures/projects/directory_isolation/env/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      103 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/directory_isolation/env/settings
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.522440 ansible-runner-2.3.2/test/fixtures/projects/directory_isolation/project/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       86 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/directory_isolation/project/main.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.522440 ansible-runner-2.3.2/test/fixtures/projects/files/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       70 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/files/test_ee.py
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.522440 ansible-runner-2.3.2/test/fixtures/projects/host_status/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.522440 ansible-runner-2.3.2/test/fixtures/projects/host_status/env/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       26 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/host_status/env/envvars
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      187 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/host_status/inventory
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.522440 ansible-runner-2.3.2/test/fixtures/projects/host_status/project/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1068 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/host_status/project/gen_host_status.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.511440 ansible-runner-2.3.2/test/fixtures/projects/job_env/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.522440 ansible-runner-2.3.2/test/fixtures/projects/job_env/env/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       42 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/job_env/env/envvars
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       28 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/job_env/env/settings
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.522440 ansible-runner-2.3.2/test/fixtures/projects/job_env/inventory/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      126 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/job_env/inventory/hosts
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.522440 ansible-runner-2.3.2/test/fixtures/projects/job_env/project/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       97 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/job_env/project/printenv.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.511440 ansible-runner-2.3.2/test/fixtures/projects/music/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.511440 ansible-runner-2.3.2/test/fixtures/projects/music/project/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.511440 ansible-runner-2.3.2/test/fixtures/projects/music/project/roles/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.511440 ansible-runner-2.3.2/test/fixtures/projects/music/project/roles/Into_The_Mystic/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.523440 ansible-runner-2.3.2/test/fixtures/projects/music/project/roles/Into_The_Mystic/meta/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      405 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/music/project/roles/Into_The_Mystic/meta/argument_specs.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.511440 ansible-runner-2.3.2/test/fixtures/projects/printenv/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.523440 ansible-runner-2.3.2/test/fixtures/projects/printenv/env/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       26 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/printenv/env/envvars
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.523440 ansible-runner-2.3.2/test/fixtures/projects/printenv/inventory/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      126 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/printenv/inventory/hosts
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.523440 ansible-runner-2.3.2/test/fixtures/projects/printenv/project/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.523440 ansible-runner-2.3.2/test/fixtures/projects/printenv/project/action_plugins/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      618 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/printenv/project/action_plugins/look_at_environment.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       69 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/printenv/project/get_environment.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.511440 ansible-runner-2.3.2/test/fixtures/projects/sleep/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.523440 ansible-runner-2.3.2/test/fixtures/projects/sleep/env/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       26 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/sleep/env/envvars
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.523440 ansible-runner-2.3.2/test/fixtures/projects/sleep/inventory/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      126 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/sleep/inventory/hosts
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.523440 ansible-runner-2.3.2/test/fixtures/projects/sleep/project/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      226 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/sleep/project/sleep.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.523440 ansible-runner-2.3.2/test/fixtures/projects/use_role/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.523440 ansible-runner-2.3.2/test/fixtures/projects/use_role/env/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       26 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/use_role/env/envvars
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.523440 ansible-runner-2.3.2/test/fixtures/projects/use_role/inventory/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      126 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/use_role/inventory/hosts
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.511440 ansible-runner-2.3.2/test/fixtures/projects/use_role/roles/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.512440 ansible-runner-2.3.2/test/fixtures/projects/use_role/roles/benthomasson.hello_role/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.523440 ansible-runner-2.3.2/test/fixtures/projects/use_role/roles/benthomasson.hello_role/meta/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       60 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/use_role/roles/benthomasson.hello_role/meta/.galaxy_install_info
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      184 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/use_role/roles/benthomasson.hello_role/meta/main.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.523440 ansible-runner-2.3.2/test/fixtures/projects/use_role/roles/benthomasson.hello_role/tasks/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       13 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/use_role/roles/benthomasson.hello_role/tasks/main.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       77 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/fixtures/projects/use_role/use_role.yml
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.524440 ansible-runner-2.3.2/test/integration/
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.524440 ansible-runner-2.3.2/test/integration/callback/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      298 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/integration/callback/other_callback.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     2131 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/integration/conftest.py
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.524440 ansible-runner-2.3.2/test/integration/containerized/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     2350 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/integration/containerized/test_cleanup_images.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     2676 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/integration/containerized/test_cli_containerized.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     5952 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/integration/containerized/test_container_management.py
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.525440 ansible-runner-2.3.2/test/integration/exec_env/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      262 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/integration/exec_env/Containerfile
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1052 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/integration/exec_env/demo.yml
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       87 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/integration/exec_env/inventory.ini
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     4685 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/integration/test___main__.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1561 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/integration/test_config.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)    13911 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/integration/test_display_callback.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     6796 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/integration/test_events.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)    16766 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/integration/test_interface.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     6042 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/integration/test_main.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     8641 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/integration/test_runner.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)    18432 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/integration/test_transmit_worker_process.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       94 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/requirements.txt
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.525440 ansible-runner-2.3.2/test/unit/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/unit/__init__.py
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.525440 ansible-runner-2.3.2/test/unit/__main__/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/unit/__main__/__init__.py
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.525440 ansible-runner-2.3.2/test/unit/__main__/main/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1782 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/unit/__main__/main/test_worker.py
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.526440 ansible-runner-2.3.2/test/unit/config/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/unit/config/__init__.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)    12787 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/unit/config/test__base.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     3635 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/unit/config/test_ansible_cfg.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     4062 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/unit/config/test_command.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     7830 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/unit/config/test_container_volmount_generation.py
--rwxr-xr-x   0 mdavis    (1000) mdavis    (1000)     6317 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/unit/config/test_doc.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     5672 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/unit/config/test_inventory.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)    25407 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/unit/config/test_runner.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      214 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/unit/conftest.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     3074 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/unit/test_cleanup.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     6299 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/unit/test_event_filter.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      914 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/unit/test_interface.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     3727 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/unit/test_loader.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     6937 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/unit/test_runner.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      394 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/unit/test_utils.py
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.526440 ansible-runner-2.3.2/test/unit/utils/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/unit/utils/__init__.py
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.526440 ansible-runner-2.3.2/test/unit/utils/capacity/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/unit/utils/capacity/__init__.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     3125 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/unit/utils/capacity/test_uuid.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      659 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/unit/utils/test_cleanup_folder.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     6476 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/unit/utils/test_dump_artifacts.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      621 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/unit/utils/test_fifo_pipe.py
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)    10741 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/unit/utils/test_utils.py
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.526440 ansible-runner-2.3.2/test/utils/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1162 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/test/utils/common.py
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.527440 ansible-runner-2.3.2/tools/
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      947 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/tools/bindep.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       24 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/tools/build-requirements.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      187 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/tools/requirements-stable-2.10.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      187 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/tools/requirements-stable-2.11.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      187 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/tools/requirements-stable-2.12.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      182 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/tools/requirements-stable-2.9.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)      187 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/tools/requirements.txt
--rwxr-xr-x   0 mdavis    (1000) mdavis    (1000)      455 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/tools/test-setup.sh
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       18 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/tools/upper-constraints-stable-2.10.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       18 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/tools/upper-constraints-stable-2.11.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       13 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/tools/upper-constraints-stable-2.12.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)       13 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/tools/upper-constraints-stable-2.9.txt
--rw-r--r--   0 mdavis    (1000) mdavis    (1000)     1341 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/tox.ini
-drwxr-xr-x   0 mdavis    (1000) mdavis    (1000)        0 2023-03-01 21:11:50.527440 ansible-runner-2.3.2/utils/
--rwxr-xr-x   0 mdavis    (1000) mdavis    (1000)     4291 2023-03-01 21:06:43.000000 ansible-runner-2.3.2/utils/entrypoint.sh
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.644988 ansible-runner-2.3.3/
+-rw-r--r--   0 akasurde   (501) wheel        (0)      209 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/.cherry_picker.toml
+-rw-r--r--   0 akasurde   (501) wheel        (0)      287 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/.coveragerc
+-rw-r--r--   0 akasurde   (501) wheel        (0)        5 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/.dockerignore
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.609625 ansible-runner-2.3.3/.github/
+-rw-r--r--   0 akasurde   (501) wheel        (0)      162 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/.github/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.610391 ansible-runner-2.3.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 akasurde   (501) wheel        (0)     1939 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 akasurde   (501) wheel        (0)       27 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 akasurde   (501) wheel        (0)      611 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/.github/ISSUE_TEMPLATE/documentation_report.yml
+-rw-r--r--   0 akasurde   (501) wheel        (0)      588 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 akasurde   (501) wheel        (0)       23 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/.github/issue_labeler.yml
+-rw-r--r--   0 akasurde   (501) wheel        (0)      117 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/.github/patchback.yml
+-rw-r--r--   0 akasurde   (501) wheel        (0)       37 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/.github/pr_labeler_existing.yml
+-rw-r--r--   0 akasurde   (501) wheel        (0)       90 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/.github/pr_labeler_new.yml
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.610930 ansible-runner-2.3.3/.github/workflows/
+-rw-r--r--   0 akasurde   (501) wheel        (0)     3011 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/.github/workflows/ci.yml
+-rw-r--r--   0 akasurde   (501) wheel        (0)      763 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/.github/workflows/triage_existing.yml
+-rw-r--r--   0 akasurde   (501) wheel        (0)      734 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/.github/workflows/triage_new.yml
+-rw-r--r--   0 akasurde   (501) wheel        (0)      114 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/.pre-commit-config.yaml
+-rw-r--r--   0 akasurde   (501) wheel        (0)      334 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/.readthedocs.yaml
+-rw-r--r--   0 akasurde   (501) wheel        (0)      466 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/.yamllint
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.611291 ansible-runner-2.3.3/.zuul.d/
+-rw-r--r--   0 akasurde   (501) wheel        (0)     8029 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/.zuul.d/jobs.yaml
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.611473 ansible-runner-2.3.3/.zuul.d/playbooks/
+-rw-r--r--   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/.zuul.d/playbooks/.zuul.ignore
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.611695 ansible-runner-2.3.3/.zuul.d/playbooks/ansible-runner-container-image-base/
+-rw-r--r--   0 akasurde   (501) wheel        (0)      331 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/.zuul.d/playbooks/ansible-runner-container-image-base/pre.yaml
+-rw-r--r--   0 akasurde   (501) wheel        (0)      795 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/.zuul.d/project.yaml
+-rw-r--r--   0 akasurde   (501) wheel        (0)     4358 2023-05-30 15:45:54.000000 ansible-runner-2.3.3/AUTHORS
+-rw-r--r--   0 akasurde   (501) wheel        (0)      306 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/CODEOWNERS
+-rw-r--r--   0 akasurde   (501) wheel        (0)     1422 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/CONTRIBUTING.md
+-rw-r--r--   0 akasurde   (501) wheel        (0)    49585 2023-05-30 15:45:54.000000 ansible-runner-2.3.3/ChangeLog
+-rw-r--r--   0 akasurde   (501) wheel        (0)     2547 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/Dockerfile
+-rw-r--r--   0 akasurde   (501) wheel        (0)     9304 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/LICENSE.md
+-rw-r--r--   0 akasurde   (501) wheel        (0)       55 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/MANIFEST.in
+-rw-r--r--   0 akasurde   (501) wheel        (0)     5345 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/Makefile
+-rw-r--r--   0 akasurde   (501) wheel        (0)     3313 2023-05-30 15:45:54.645141 ansible-runner-2.3.3/PKG-INFO
+-rw-r--r--   0 akasurde   (501) wheel        (0)     2044 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/README.md
+-rw-r--r--   0 akasurde   (501) wheel        (0)      313 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/SECURITY.md
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.613872 ansible-runner-2.3.3/ansible_runner/
+-rw-r--r--   0 akasurde   (501) wheel        (0)      708 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/ansible_runner/__init__.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)    35764 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/ansible_runner/__main__.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)     6609 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/ansible_runner/cleanup.py
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.616351 ansible-runner-2.3.3/ansible_runner/config/
+-rw-r--r--   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/ansible_runner/config/__init__.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)    29029 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/ansible_runner/config/_base.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)     3381 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/ansible_runner/config/ansible_cfg.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)     4323 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/ansible_runner/config/command.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)     6418 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/ansible_runner/config/doc.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)     4897 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/ansible_runner/config/inventory.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)    17441 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/ansible_runner/config/runner.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)      408 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/ansible_runner/defaults.py
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.616531 ansible-runner-2.3.3/ansible_runner/display_callback/
+-rw-r--r--   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/ansible_runner/display_callback/__init__.py
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.616833 ansible-runner-2.3.3/ansible_runner/display_callback/callback/
+-rw-r--r--   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/ansible_runner/display_callback/callback/__init__.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)    31150 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/ansible_runner/display_callback/callback/awx_display.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)      256 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/ansible_runner/exceptions.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)    64207 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/ansible_runner/interface.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)     5986 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/ansible_runner/loader.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)     3008 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/ansible_runner/output.py
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.617034 ansible-runner-2.3.3/ansible_runner/plugins/
+-rw-r--r--   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/ansible_runner/plugins/__init__.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)    25381 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/ansible_runner/runner.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)      905 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/ansible_runner/runner_config.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)    14152 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/ansible_runner/streaming.py
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.617884 ansible-runner-2.3.3/ansible_runner/utils/
+-rw-r--r--   0 akasurde   (501) wheel        (0)    17031 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/ansible_runner/utils/__init__.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)    11731 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/ansible_runner/utils/base64io.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)     1719 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/ansible_runner/utils/capacity.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)      159 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/ansible_runner/utils/importlib_compat.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)     4931 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/ansible_runner/utils/streaming.py
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.615214 ansible-runner-2.3.3/ansible_runner.egg-info/
+-rw-r--r--   0 akasurde   (501) wheel        (0)     3313 2023-05-30 15:45:54.000000 ansible-runner-2.3.3/ansible_runner.egg-info/PKG-INFO
+-rw-r--r--   0 akasurde   (501) wheel        (0)     7452 2023-05-30 15:45:54.000000 ansible-runner-2.3.3/ansible_runner.egg-info/SOURCES.txt
+-rw-r--r--   0 akasurde   (501) wheel        (0)        1 2023-05-30 15:45:54.000000 ansible-runner-2.3.3/ansible_runner.egg-info/dependency_links.txt
+-rw-r--r--   0 akasurde   (501) wheel        (0)       64 2023-05-30 15:45:54.000000 ansible-runner-2.3.3/ansible_runner.egg-info/entry_points.txt
+-rw-r--r--   0 akasurde   (501) wheel        (0)        1 2023-05-30 15:45:54.000000 ansible-runner-2.3.3/ansible_runner.egg-info/not-zip-safe
+-rw-r--r--   0 akasurde   (501) wheel        (0)       46 2023-05-30 15:45:54.000000 ansible-runner-2.3.3/ansible_runner.egg-info/pbr.json
+-rw-r--r--   0 akasurde   (501) wheel        (0)       77 2023-05-30 15:45:54.000000 ansible-runner-2.3.3/ansible_runner.egg-info/requires.txt
+-rw-r--r--   0 akasurde   (501) wheel        (0)       15 2023-05-30 15:45:54.000000 ansible-runner-2.3.3/ansible_runner.egg-info/top_level.txt
+-rw-r--r--   0 akasurde   (501) wheel        (0)      155 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/bindep.txt
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.595709 ansible-runner-2.3.3/demo/
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.618710 ansible-runner-2.3.3/demo/env/
+-rw-r--r--   0 akasurde   (501) wheel        (0)       18 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/demo/env/envvars
+-rw-r--r--   0 akasurde   (501) wheel        (0)       40 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/demo/env/extravars
+-rw-r--r--   0 akasurde   (501) wheel        (0)       39 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/demo/env/passwords
+-rw-r--r--   0 akasurde   (501) wheel        (0)       60 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/demo/env/settings
+-rw-r--r--   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/demo/env/ssh_key
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.618843 ansible-runner-2.3.3/demo/inventory/
+-rw-r--r--   0 akasurde   (501) wheel        (0)       94 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/demo/inventory/hosts
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.619129 ansible-runner-2.3.3/demo/project/
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.595898 ansible-runner-2.3.3/demo/project/roles/
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.619355 ansible-runner-2.3.3/demo/project/roles/testrole/
+-rw-r--r--   0 akasurde   (501) wheel        (0)     1328 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/demo/project/roles/testrole/README.md
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.619565 ansible-runner-2.3.3/demo/project/roles/testrole/defaults/
+-rw-r--r--   0 akasurde   (501) wheel        (0)       33 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/demo/project/roles/testrole/defaults/main.yml
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.619759 ansible-runner-2.3.3/demo/project/roles/testrole/handlers/
+-rw-r--r--   0 akasurde   (501) wheel        (0)       33 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/demo/project/roles/testrole/handlers/main.yml
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.619933 ansible-runner-2.3.3/demo/project/roles/testrole/meta/
+-rw-r--r--   0 akasurde   (501) wheel        (0)     1767 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/demo/project/roles/testrole/meta/main.yml
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.620107 ansible-runner-2.3.3/demo/project/roles/testrole/tasks/
+-rw-r--r--   0 akasurde   (501) wheel        (0)      129 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/demo/project/roles/testrole/tasks/main.yml
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.620475 ansible-runner-2.3.3/demo/project/roles/testrole/tests/
+-rw-r--r--   0 akasurde   (501) wheel        (0)       11 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/demo/project/roles/testrole/tests/inventory
+-rw-r--r--   0 akasurde   (501) wheel        (0)       67 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/demo/project/roles/testrole/tests/test.yml
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.620641 ansible-runner-2.3.3/demo/project/roles/testrole/vars/
+-rw-r--r--   0 akasurde   (501) wheel        (0)       29 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/demo/project/roles/testrole/vars/main.yml
+-rw-r--r--   0 akasurde   (501) wheel        (0)       51 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/demo/project/test.yml
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.623791 ansible-runner-2.3.3/docs/
+-rw-r--r--   0 akasurde   (501) wheel        (0)      611 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/docs/Makefile
+-rw-r--r--   0 akasurde   (501) wheel        (0)      225 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/docs/ansible_runner.config.rst
+-rw-r--r--   0 akasurde   (501) wheel        (0)      445 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/docs/ansible_runner.display_callback.rst
+-rw-r--r--   0 akasurde   (501) wheel        (0)     1142 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/docs/ansible_runner.rst
+-rw-r--r--   0 akasurde   (501) wheel        (0)     5594 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/docs/conf.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)     1749 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/docs/container.rst
+-rw-r--r--   0 akasurde   (501) wheel        (0)     5153 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/docs/execution_environments.rst
+-rw-r--r--   0 akasurde   (501) wheel        (0)     2339 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/docs/external_interface.rst
+-rw-r--r--   0 akasurde   (501) wheel        (0)     2288 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/docs/index.rst
+-rw-r--r--   0 akasurde   (501) wheel        (0)     1793 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/docs/install.rst
+-rw-r--r--   0 akasurde   (501) wheel        (0)    18971 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/docs/intro.rst
+-rw-r--r--   0 akasurde   (501) wheel        (0)      818 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/docs/make.bat
+-rw-r--r--   0 akasurde   (501) wheel        (0)       97 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/docs/modules.rst
+-rw-r--r--   0 akasurde   (501) wheel        (0)    17999 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/docs/python_interface.rst
+-rw-r--r--   0 akasurde   (501) wheel        (0)     4146 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/docs/remote_jobs.rst
+-rw-r--r--   0 akasurde   (501) wheel        (0)       36 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/docs/requirements.in
+-rw-r--r--   0 akasurde   (501) wheel        (0)      625 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/docs/requirements.txt
+-rw-r--r--   0 akasurde   (501) wheel        (0)     5917 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/docs/standalone.rst
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.597289 ansible-runner-2.3.3/packaging/
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.624830 ansible-runner-2.3.3/packaging/debian/
+-rw-r--r--   0 akasurde   (501) wheel        (0)      129 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/packaging/debian/changelog
+-rw-r--r--   0 akasurde   (501) wheel        (0)        2 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/packaging/debian/compat
+-rw-r--r--   0 akasurde   (501) wheel        (0)      802 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/packaging/debian/control
+-rw-r--r--   0 akasurde   (501) wheel        (0)     9703 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/packaging/debian/copyright
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.625207 ansible-runner-2.3.3/packaging/debian/docker/
+-rw-r--r--   0 akasurde   (501) wheel        (0)      302 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/packaging/debian/docker/Dockerfile
+-rw-r--r--   0 akasurde   (501) wheel        (0)      284 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/packaging/debian/docker/docker-compose.yml
+-rw-r--r--   0 akasurde   (501) wheel        (0)       32 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/packaging/debian/pydist-overrides
+-rwxr-xr-x   0 akasurde   (501) wheel        (0)      264 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/packaging/debian/rules
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.625389 ansible-runner-2.3.3/packaging/debian/source/
+-rw-r--r--   0 akasurde   (501) wheel        (0)       12 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/packaging/debian/source/format
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.626132 ansible-runner-2.3.3/packaging/rpm/
+-rw-r--r--   0 akasurde   (501) wheel        (0)      236 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/packaging/rpm/Dockerfile.epel-7-x86_64
+-rw-r--r--   0 akasurde   (501) wheel        (0)      277 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/packaging/rpm/Dockerfile.epel-8-x86_64
+-rw-r--r--   0 akasurde   (501) wheel        (0)     4832 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/packaging/rpm/ansible-runner.spec.j2
+-rw-r--r--   0 akasurde   (501) wheel        (0)      460 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/packaging/rpm/docker-compose.yml
+-rw-r--r--   0 akasurde   (501) wheel        (0)      339 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/pytest.ini
+-rw-r--r--   0 akasurde   (501) wheel        (0)      185 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/requirements.txt
+-rw-r--r--   0 akasurde   (501) wheel        (0)     1472 2023-05-30 15:45:54.645667 ansible-runner-2.3.3/setup.cfg
+-rw-r--r--   0 akasurde   (501) wheel        (0)      104 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/setup.py
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.626634 ansible-runner-2.3.3/test/
+-rw-r--r--   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/__init__.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)     2739 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/conftest.py
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.597626 ansible-runner-2.3.3/test/fixtures/
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.602433 ansible-runner-2.3.3/test/fixtures/projects/
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.626801 ansible-runner-2.3.3/test/fixtures/projects/collection_role/
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.597932 ansible-runner-2.3.3/test/fixtures/projects/collection_role/collections/
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.598015 ansible-runner-2.3.3/test/fixtures/projects/collection_role/collections/ansible_collections/
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.598101 ansible-runner-2.3.3/test/fixtures/projects/collection_role/collections/ansible_collections/groovy/
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.627122 ansible-runner-2.3.3/test/fixtures/projects/collection_role/collections/ansible_collections/groovy/peanuts/
+-rw-r--r--   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/collection_role/collections/ansible_collections/groovy/peanuts/README.md
+-rw-r--r--   0 akasurde   (501) wheel        (0)      290 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/collection_role/collections/ansible_collections/groovy/peanuts/galaxy.yml
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.598329 ansible-runner-2.3.3/test/fixtures/projects/collection_role/collections/ansible_collections/groovy/peanuts/roles/
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.598422 ansible-runner-2.3.3/test/fixtures/projects/collection_role/collections/ansible_collections/groovy/peanuts/roles/hello/
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.627285 ansible-runner-2.3.3/test/fixtures/projects/collection_role/collections/ansible_collections/groovy/peanuts/roles/hello/tasks/
+-rw-r--r--   0 akasurde   (501) wheel        (0)       34 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/collection_role/collections/ansible_collections/groovy/peanuts/roles/hello/tasks/main.yml
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.627461 ansible-runner-2.3.3/test/fixtures/projects/collection_role/env/
+-rw-r--r--   0 akasurde   (501) wheel        (0)       26 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/collection_role/env/envvars
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.627617 ansible-runner-2.3.3/test/fixtures/projects/collection_role/inventory/
+-rw-r--r--   0 akasurde   (501) wheel        (0)      126 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/collection_role/inventory/hosts
+-rw-r--r--   0 akasurde   (501) wheel        (0)       74 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/collection_role/use_role.yml
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.599116 ansible-runner-2.3.3/test/fixtures/projects/containerized/
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.627947 ansible-runner-2.3.3/test/fixtures/projects/containerized/env/
+-rw-r--r--   0 akasurde   (501) wheel        (0)       26 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/containerized/env/envvars
+-rw-r--r--   0 akasurde   (501) wheel        (0)       78 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/containerized/env/settings
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.628110 ansible-runner-2.3.3/test/fixtures/projects/containerized/inventory/
+-rw-r--r--   0 akasurde   (501) wheel        (0)      126 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/containerized/inventory/hosts
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.628329 ansible-runner-2.3.3/test/fixtures/projects/containerized/project/
+-rw-r--r--   0 akasurde   (501) wheel        (0)      266 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/containerized/project/test-container.yml
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.599644 ansible-runner-2.3.3/test/fixtures/projects/debug/
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.628491 ansible-runner-2.3.3/test/fixtures/projects/debug/env/
+-rw-r--r--   0 akasurde   (501) wheel        (0)       26 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/debug/env/envvars
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.628836 ansible-runner-2.3.3/test/fixtures/projects/debug/inventory/
+-rw-r--r--   0 akasurde   (501) wheel        (0)       91 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/debug/inventory/inv_1
+-rw-r--r--   0 akasurde   (501) wheel        (0)       91 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/debug/inventory/inv_2
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.629006 ansible-runner-2.3.3/test/fixtures/projects/debug/project/
+-rw-r--r--   0 akasurde   (501) wheel        (0)       55 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/debug/project/debug.yml
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.599865 ansible-runner-2.3.3/test/fixtures/projects/debug/project/roles/
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.599948 ansible-runner-2.3.3/test/fixtures/projects/debug/project/roles/hello_world/
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.629182 ansible-runner-2.3.3/test/fixtures/projects/debug/project/roles/hello_world/tasks/
+-rw-r--r--   0 akasurde   (501) wheel        (0)       62 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/debug/project/roles/hello_world/tasks/main.yml
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.600237 ansible-runner-2.3.3/test/fixtures/projects/directory_isolation/
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.629354 ansible-runner-2.3.3/test/fixtures/projects/directory_isolation/env/
+-rw-r--r--   0 akasurde   (501) wheel        (0)      103 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/directory_isolation/env/settings
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.629525 ansible-runner-2.3.3/test/fixtures/projects/directory_isolation/project/
+-rw-r--r--   0 akasurde   (501) wheel        (0)       86 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/directory_isolation/project/main.yml
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.629711 ansible-runner-2.3.3/test/fixtures/projects/files/
+-rw-r--r--   0 akasurde   (501) wheel        (0)       70 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/files/test_ee.py
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.629937 ansible-runner-2.3.3/test/fixtures/projects/host_status/
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.630101 ansible-runner-2.3.3/test/fixtures/projects/host_status/env/
+-rw-r--r--   0 akasurde   (501) wheel        (0)       26 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/host_status/env/envvars
+-rw-r--r--   0 akasurde   (501) wheel        (0)      187 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/host_status/inventory
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.630273 ansible-runner-2.3.3/test/fixtures/projects/host_status/project/
+-rw-r--r--   0 akasurde   (501) wheel        (0)     1068 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/host_status/project/gen_host_status.yml
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.601014 ansible-runner-2.3.3/test/fixtures/projects/job_env/
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.630621 ansible-runner-2.3.3/test/fixtures/projects/job_env/env/
+-rw-r--r--   0 akasurde   (501) wheel        (0)       42 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/job_env/env/envvars
+-rw-r--r--   0 akasurde   (501) wheel        (0)       28 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/job_env/env/settings
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.630799 ansible-runner-2.3.3/test/fixtures/projects/job_env/inventory/
+-rw-r--r--   0 akasurde   (501) wheel        (0)      126 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/job_env/inventory/hosts
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.630974 ansible-runner-2.3.3/test/fixtures/projects/job_env/project/
+-rw-r--r--   0 akasurde   (501) wheel        (0)       97 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/job_env/project/printenv.yml
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.601193 ansible-runner-2.3.3/test/fixtures/projects/music/
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.601270 ansible-runner-2.3.3/test/fixtures/projects/music/project/
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.601341 ansible-runner-2.3.3/test/fixtures/projects/music/project/roles/
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.601411 ansible-runner-2.3.3/test/fixtures/projects/music/project/roles/Into_The_Mystic/
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.631145 ansible-runner-2.3.3/test/fixtures/projects/music/project/roles/Into_The_Mystic/meta/
+-rw-r--r--   0 akasurde   (501) wheel        (0)      405 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/music/project/roles/Into_The_Mystic/meta/argument_specs.yml
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.601810 ansible-runner-2.3.3/test/fixtures/projects/printenv/
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.631416 ansible-runner-2.3.3/test/fixtures/projects/printenv/env/
+-rw-r--r--   0 akasurde   (501) wheel        (0)       26 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/printenv/env/envvars
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.631585 ansible-runner-2.3.3/test/fixtures/projects/printenv/inventory/
+-rw-r--r--   0 akasurde   (501) wheel        (0)      126 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/printenv/inventory/hosts
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.631762 ansible-runner-2.3.3/test/fixtures/projects/printenv/project/
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.631950 ansible-runner-2.3.3/test/fixtures/projects/printenv/project/action_plugins/
+-rw-r--r--   0 akasurde   (501) wheel        (0)      618 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/printenv/project/action_plugins/look_at_environment.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)       69 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/printenv/project/get_environment.yml
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.602320 ansible-runner-2.3.3/test/fixtures/projects/sleep/
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.632147 ansible-runner-2.3.3/test/fixtures/projects/sleep/env/
+-rw-r--r--   0 akasurde   (501) wheel        (0)       26 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/sleep/env/envvars
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.632310 ansible-runner-2.3.3/test/fixtures/projects/sleep/inventory/
+-rw-r--r--   0 akasurde   (501) wheel        (0)      126 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/sleep/inventory/hosts
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.632490 ansible-runner-2.3.3/test/fixtures/projects/sleep/project/
+-rw-r--r--   0 akasurde   (501) wheel        (0)      226 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/sleep/project/sleep.yml
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.632656 ansible-runner-2.3.3/test/fixtures/projects/use_role/
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.632840 ansible-runner-2.3.3/test/fixtures/projects/use_role/env/
+-rw-r--r--   0 akasurde   (501) wheel        (0)       26 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/use_role/env/envvars
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.633020 ansible-runner-2.3.3/test/fixtures/projects/use_role/inventory/
+-rw-r--r--   0 akasurde   (501) wheel        (0)      126 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/use_role/inventory/hosts
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.602857 ansible-runner-2.3.3/test/fixtures/projects/use_role/roles/
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.603058 ansible-runner-2.3.3/test/fixtures/projects/use_role/roles/benthomasson.hello_role/
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.633428 ansible-runner-2.3.3/test/fixtures/projects/use_role/roles/benthomasson.hello_role/meta/
+-rw-r--r--   0 akasurde   (501) wheel        (0)       60 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/use_role/roles/benthomasson.hello_role/meta/.galaxy_install_info
+-rw-r--r--   0 akasurde   (501) wheel        (0)      184 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/use_role/roles/benthomasson.hello_role/meta/main.yml
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.633639 ansible-runner-2.3.3/test/fixtures/projects/use_role/roles/benthomasson.hello_role/tasks/
+-rw-r--r--   0 akasurde   (501) wheel        (0)       13 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/use_role/roles/benthomasson.hello_role/tasks/main.yml
+-rw-r--r--   0 akasurde   (501) wheel        (0)       77 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/fixtures/projects/use_role/use_role.yml
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.635339 ansible-runner-2.3.3/test/integration/
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.635543 ansible-runner-2.3.3/test/integration/callback/
+-rw-r--r--   0 akasurde   (501) wheel        (0)      298 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/integration/callback/other_callback.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)     2131 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/integration/conftest.py
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.636087 ansible-runner-2.3.3/test/integration/containerized/
+-rw-r--r--   0 akasurde   (501) wheel        (0)     2350 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/integration/containerized/test_cleanup_images.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)     2676 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/integration/containerized/test_cli_containerized.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)     5952 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/integration/containerized/test_container_management.py
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.636654 ansible-runner-2.3.3/test/integration/exec_env/
+-rw-r--r--   0 akasurde   (501) wheel        (0)      262 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/integration/exec_env/Containerfile
+-rw-r--r--   0 akasurde   (501) wheel        (0)     1052 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/integration/exec_env/demo.yml
+-rw-r--r--   0 akasurde   (501) wheel        (0)       87 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/integration/exec_env/inventory.ini
+-rw-r--r--   0 akasurde   (501) wheel        (0)     4685 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/integration/test___main__.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)     1561 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/integration/test_config.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)    13911 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/integration/test_display_callback.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)     6796 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/integration/test_events.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)    16766 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/integration/test_interface.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)     6042 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/integration/test_main.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)     8641 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/integration/test_runner.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)    18432 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/integration/test_transmit_worker_process.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)       94 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/requirements.txt
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.638109 ansible-runner-2.3.3/test/unit/
+-rw-r--r--   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/unit/__init__.py
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.638485 ansible-runner-2.3.3/test/unit/__main__/
+-rw-r--r--   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/unit/__main__/__init__.py
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.638656 ansible-runner-2.3.3/test/unit/__main__/main/
+-rw-r--r--   0 akasurde   (501) wheel        (0)     1782 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/unit/__main__/main/test_worker.py
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.640187 ansible-runner-2.3.3/test/unit/config/
+-rw-r--r--   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/unit/config/__init__.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)    12787 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/unit/config/test__base.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)     3635 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/unit/config/test_ansible_cfg.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)     4062 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/unit/config/test_command.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)     7830 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/unit/config/test_container_volmount_generation.py
+-rwxr-xr-x   0 akasurde   (501) wheel        (0)     6317 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/unit/config/test_doc.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)     5672 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/unit/config/test_inventory.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)    25407 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/unit/config/test_runner.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)      214 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/unit/conftest.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)     3074 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/unit/test_cleanup.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)     6299 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/unit/test_event_filter.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)      914 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/unit/test_interface.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)     3727 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/unit/test_loader.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)     6937 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/unit/test_runner.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)      394 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/unit/test_utils.py
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.641103 ansible-runner-2.3.3/test/unit/utils/
+-rw-r--r--   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/unit/utils/__init__.py
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.641430 ansible-runner-2.3.3/test/unit/utils/capacity/
+-rw-r--r--   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/unit/utils/capacity/__init__.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)     3125 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/unit/utils/capacity/test_uuid.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)      659 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/unit/utils/test_cleanup_folder.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)     6476 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/unit/utils/test_dump_artifacts.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)      621 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/unit/utils/test_fifo_pipe.py
+-rw-r--r--   0 akasurde   (501) wheel        (0)    10741 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/unit/utils/test_utils.py
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.641600 ansible-runner-2.3.3/test/utils/
+-rw-r--r--   0 akasurde   (501) wheel        (0)     1162 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/test/utils/common.py
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.644524 ansible-runner-2.3.3/tools/
+-rw-r--r--   0 akasurde   (501) wheel        (0)      947 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/tools/bindep.txt
+-rw-r--r--   0 akasurde   (501) wheel        (0)       24 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/tools/build-requirements.txt
+-rw-r--r--   0 akasurde   (501) wheel        (0)      187 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/tools/requirements-stable-2.10.txt
+-rw-r--r--   0 akasurde   (501) wheel        (0)      187 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/tools/requirements-stable-2.11.txt
+-rw-r--r--   0 akasurde   (501) wheel        (0)      187 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/tools/requirements-stable-2.12.txt
+-rw-r--r--   0 akasurde   (501) wheel        (0)      182 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/tools/requirements-stable-2.9.txt
+-rw-r--r--   0 akasurde   (501) wheel        (0)      187 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/tools/requirements.txt
+-rwxr-xr-x   0 akasurde   (501) wheel        (0)      455 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/tools/test-setup.sh
+-rw-r--r--   0 akasurde   (501) wheel        (0)       18 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/tools/upper-constraints-stable-2.10.txt
+-rw-r--r--   0 akasurde   (501) wheel        (0)       18 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/tools/upper-constraints-stable-2.11.txt
+-rw-r--r--   0 akasurde   (501) wheel        (0)       13 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/tools/upper-constraints-stable-2.12.txt
+-rw-r--r--   0 akasurde   (501) wheel        (0)       13 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/tools/upper-constraints-stable-2.9.txt
+-rw-r--r--   0 akasurde   (501) wheel        (0)     1341 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/tox.ini
+drwxr-xr-x   0 akasurde   (501) wheel        (0)        0 2023-05-30 15:45:54.644756 ansible-runner-2.3.3/utils/
+-rwxr-xr-x   0 akasurde   (501) wheel        (0)     4291 2023-05-30 15:45:25.000000 ansible-runner-2.3.3/utils/entrypoint.sh
```

### Comparing `ansible-runner-2.3.2/.github/ISSUE_TEMPLATE/bug_report.yml` & `ansible-runner-2.3.3/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/.github/ISSUE_TEMPLATE/documentation_report.yml` & `ansible-runner-2.3.3/.github/ISSUE_TEMPLATE/documentation_report.yml`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/.github/ISSUE_TEMPLATE/feature_request.yml` & `ansible-runner-2.3.3/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/.github/workflows/ci.yml` & `ansible-runner-2.3.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/.github/workflows/triage_existing.yml` & `ansible-runner-2.3.3/.github/workflows/triage_existing.yml`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/.github/workflows/triage_new.yml` & `ansible-runner-2.3.3/.github/workflows/triage_new.yml`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/.zuul.d/jobs.yaml` & `ansible-runner-2.3.3/.zuul.d/jobs.yaml`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/.zuul.d/project.yaml` & `ansible-runner-2.3.3/.zuul.d/project.yaml`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/AUTHORS` & `ansible-runner-2.3.3/AUTHORS`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 John R Barker <jobarker@redhat.com>
 John Westcott IV <32551173+john-westcott-iv@users.noreply.github.com>
 Joshua "jag" Ginsberg <jag@flowtheory.net>
 Lavinia Lee <Tranquilled@users.noreply.github.com>
 Lavinia Lee <llee@vlp-mtllee.us.drwholdings.com>
 Marek Hulan <mhulan@redhat.com>
 Matt Davis <6775756+nitzmahone@users.noreply.github.com>
+Matt Martz <matt@sivel.net>
 Matt Phillips <mphillips34@gmail.com>
 Matthew Jones <bsdmatburt@gmail.com>
 Matthew Jones <matburt@redhat.com>
 Michael Alan Tucker <matucker@juniper.net>
 Michael Tucker <matucker@juniper.net>
 Nick LaMuro <nicklamuro@gmail.com>
 Nick Smith <clickthisnick@users.noreply.github.com>
@@ -81,14 +82,15 @@
 Thomas Bechtold <tbechtold@suse.com>
 Thomas C. Foulds <me@thomascfoulds.com>
 Tim Rozet <trozet@redhat.com>
 Toshio Kuratomi <a.badger@gmail.com>
 Victor da Costa <victorockeiro@gmail.com>
 Vlad Romanenko <vlad-ro@users.noreply.github.com>
 Wayne Witzel III <wayne@riotousliving.com>
+Wong Hoi Sing Edison <hswong3i@gmail.com>
 Yanis Guenane <yanis@guenane.org>
 Yujun Zhang <zhang.yujunz@zte.com.cn>
 akira6592 <akira6592@gmail.com>
 amerck <alexander.t.merck@gmail.com>
 ansible-zuul[bot] <48994755+ansible-zuul[bot]@users.noreply.github.com>
 ansible-zuul[bot] <ansible-zuul[bot]@users.noreply.github.com>
 ashwini-mhatre <mashu97@gmail.com>
```

### Comparing `ansible-runner-2.3.2/CONTRIBUTING.md` & `ansible-runner-2.3.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/ChangeLog` & `ansible-runner-2.3.3/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 CHANGES
 =======
 
+2.3.3
+-----
+
+* Remove pkg\_resources use (#1224) (#1230)
+* Add license and classifiers metadata (#1213) (#1214)
+* [devel] Add \`python\_requires = >= 3.8\` (#1206) (#1212)
+
 2.3.2
 -----
 
 * Emit periodic keepalive events from \`Worker\` (#1191) (#1201)
 * [backport][release\_2.3] Fix artifact file permissions
 * Fix Github CI (#1171) (#1172)
```

### Comparing `ansible-runner-2.3.2/Dockerfile` & `ansible-runner-2.3.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/LICENSE.md` & `ansible-runner-2.3.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/Makefile` & `ansible-runner-2.3.3/Makefile`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/PKG-INFO` & `ansible-runner-2.3.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: ansible-runner
-Version: 2.3.2
-Summary: "Consistent Ansible Python API and CLI with container and process isolation runtime capabilities"
-Home-page: https://ansible-runner.readthedocs.io
-Author: Ansible, Inc.
-Author-email: info@ansible.com
-Project-URL: Source, https://github.com/ansible/ansible-runner
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 Ansible Runner
 ==============
 
 [![PyPi](https://img.shields.io/pypi/v/ansible-runner.svg?logo=Python)](https://pypi.org/project/ansible-runner/)
 [![Documentation](https://readthedocs.org/projects/ansible-runner/badge/?version=stable)](https://ansible-runner.readthedocs.io/en/latest/)
 [![Code of Conduct](https://img.shields.io/badge/Code%20of%20Conduct-Ansible-silver.svg)](https://docs.ansible.com/ansible/latest/community/code_of_conduct.html)
 [![Ansible Mailing lists](https://img.shields.io/badge/Mailing%20lists-Ansible-orange.svg)](https://docs.ansible.com/ansible/latest/community/communication.html#mailing-list-information)
@@ -34,8 +23,7 @@
 
 [GitHub issues]: https://github.com/ansible/ansible-runner/issues
 [GitHub Milestones]: https://github.com/ansible/ansible-runner/milestones
 [contributing guide]: https://github.com/ansible/ansible-runner/blob/devel/CONTRIBUTING.md
 [irc]: https://groups.google.com/forum/#!forum/awx-project
 [Ansible Mailing lists]: https://docs.ansible.com/ansible/latest/community/communication.html#mailing-list-information
 [latest documentation]: https://ansible-runner.readthedocs.io/en/latest/
-
```

### Comparing `ansible-runner-2.3.2/ansible_runner/__init__.py` & `ansible-runner-2.3.3/ansible_runner/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-import pkg_resources
-
+from .utils.importlib_compat import importlib_metadata
 from .interface import run, run_async, \
                         run_command, run_command_async, \
                         get_plugin_docs, get_plugin_docs_async, get_plugin_list, \
                         get_role_list, get_role_argspec, \
                         get_inventory, \
                         get_ansible_config     # noqa
 from .exceptions import AnsibleRunnerException, ConfigurationError, CallbackError # noqa
 from .runner_config import RunnerConfig # noqa
 from .runner import Runner # noqa
 
 plugins = {
     entry_point.name: entry_point.load()
     for entry_point
-    in pkg_resources.iter_entry_points('ansible_runner.plugins')
+    in importlib_metadata.entry_points(group='ansible_runner.plugins')
 }
```

### Comparing `ansible-runner-2.3.2/ansible_runner/__main__.py` & `ansible-runner-2.3.3/ansible_runner/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 #
 import ast
-import pkg_resources
 import threading
 import traceback
 import argparse
 import logging
 import signal
 import sys
 import errno
@@ -38,18 +37,19 @@
 from yaml import safe_dump, safe_load
 
 from ansible_runner import run
 from ansible_runner import output
 from ansible_runner import cleanup
 from ansible_runner.utils import dump_artifact, Bunch, register_for_cleanup
 from ansible_runner.utils.capacity import get_cpu_count, get_mem_in_bytes, ensure_uuid
+from ansible_runner.utils.importlib_compat import importlib_metadata
 from ansible_runner.runner import Runner
 from ansible_runner.exceptions import AnsibleRunnerException
 
-VERSION = pkg_resources.require("ansible_runner")[0].version
+VERSION = importlib_metadata.version("ansible_runner")
 
 DEFAULT_ROLES_PATH = os.getenv('ANSIBLE_ROLES_PATH', None)
 DEFAULT_RUNNER_BINARY = os.getenv('RUNNER_BINARY', None)
 DEFAULT_RUNNER_PLAYBOOK = os.getenv('RUNNER_PLAYBOOK', None)
 DEFAULT_RUNNER_ROLE = os.getenv('RUNNER_ROLE', None)
 DEFAULT_RUNNER_MODULE = os.getenv('RUNNER_MODULE', None)
 DEFAULT_UUID = uuid4()
```

### Comparing `ansible-runner-2.3.2/ansible_runner/cleanup.py` & `ansible-runner-2.3.3/ansible_runner/cleanup.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/ansible_runner/config/_base.py` & `ansible-runner-2.3.3/ansible_runner/config/_base.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/ansible_runner/config/ansible_cfg.py` & `ansible-runner-2.3.3/ansible_runner/config/ansible_cfg.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/ansible_runner/config/command.py` & `ansible-runner-2.3.3/ansible_runner/config/command.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/ansible_runner/config/doc.py` & `ansible-runner-2.3.3/ansible_runner/config/doc.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/ansible_runner/config/inventory.py` & `ansible-runner-2.3.3/ansible_runner/config/inventory.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/ansible_runner/config/runner.py` & `ansible-runner-2.3.3/ansible_runner/config/runner.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/ansible_runner/display_callback/callback/awx_display.py` & `ansible-runner-2.3.3/ansible_runner/display_callback/callback/awx_display.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/ansible_runner/interface.py` & `ansible-runner-2.3.3/ansible_runner/interface.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/ansible_runner/loader.py` & `ansible-runner-2.3.3/ansible_runner/loader.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/ansible_runner/output.py` & `ansible-runner-2.3.3/ansible_runner/output.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/ansible_runner/runner.py` & `ansible-runner-2.3.3/ansible_runner/runner.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/ansible_runner/runner_config.py` & `ansible-runner-2.3.3/ansible_runner/runner_config.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/ansible_runner/streaming.py` & `ansible-runner-2.3.3/ansible_runner/streaming.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/ansible_runner/utils/__init__.py` & `ansible-runner-2.3.3/ansible_runner/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/ansible_runner/utils/base64io.py` & `ansible-runner-2.3.3/ansible_runner/utils/base64io.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/ansible_runner/utils/capacity.py` & `ansible-runner-2.3.3/ansible_runner/utils/capacity.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/ansible_runner/utils/streaming.py` & `ansible-runner-2.3.3/ansible_runner/utils/streaming.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/ansible_runner.egg-info/SOURCES.txt` & `ansible-runner-2.3.3/ansible_runner.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 ansible_runner/display_callback/__init__.py
 ansible_runner/display_callback/callback/__init__.py
 ansible_runner/display_callback/callback/awx_display.py
 ansible_runner/plugins/__init__.py
 ansible_runner/utils/__init__.py
 ansible_runner/utils/base64io.py
 ansible_runner/utils/capacity.py
+ansible_runner/utils/importlib_compat.py
 ansible_runner/utils/streaming.py
 demo/env/envvars
 demo/env/extravars
 demo/env/passwords
 demo/env/settings
 demo/env/ssh_key
 demo/inventory/hosts
```

### Comparing `ansible-runner-2.3.2/demo/project/roles/testrole/README.md` & `ansible-runner-2.3.3/demo/project/roles/testrole/README.md`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/demo/project/roles/testrole/meta/main.yml` & `ansible-runner-2.3.3/demo/project/roles/testrole/meta/main.yml`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/docs/Makefile` & `ansible-runner-2.3.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/docs/ansible_runner.rst` & `ansible-runner-2.3.3/docs/ansible_runner.rst`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/docs/conf.py` & `ansible-runner-2.3.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/docs/container.rst` & `ansible-runner-2.3.3/docs/container.rst`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/docs/execution_environments.rst` & `ansible-runner-2.3.3/docs/execution_environments.rst`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/docs/external_interface.rst` & `ansible-runner-2.3.3/docs/external_interface.rst`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/docs/index.rst` & `ansible-runner-2.3.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/docs/install.rst` & `ansible-runner-2.3.3/docs/install.rst`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/docs/intro.rst` & `ansible-runner-2.3.3/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/docs/make.bat` & `ansible-runner-2.3.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/docs/python_interface.rst` & `ansible-runner-2.3.3/docs/python_interface.rst`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/docs/remote_jobs.rst` & `ansible-runner-2.3.3/docs/remote_jobs.rst`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/docs/requirements.txt` & `ansible-runner-2.3.3/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/docs/standalone.rst` & `ansible-runner-2.3.3/docs/standalone.rst`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/packaging/debian/control` & `ansible-runner-2.3.3/packaging/debian/control`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/packaging/debian/copyright` & `ansible-runner-2.3.3/packaging/debian/copyright`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/packaging/rpm/ansible-runner.spec.j2` & `ansible-runner-2.3.3/packaging/rpm/ansible-runner.spec.j2`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/test/conftest.py` & `ansible-runner-2.3.3/test/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import shutil
 
 from pathlib import Path
 from packaging.version import Version
-import subprocess
 
 from ansible_runner import defaults
+from ansible_runner.utils.importlib_compat import importlib_metadata
 
-import pkg_resources
 import pytest
 
 
 CONTAINER_RUNTIMES = (
     'docker',
     'podman',
 )
@@ -31,42 +30,34 @@
     """
     Check if the version of Ansible is less than 2.11.
 
     CI tests with either ansible-core (>=2.11), ansible-base (==2.10), and ansible (<=2.9).
     """
 
     try:
-        if pkg_resources.get_distribution('ansible-core').version:
+        if importlib_metadata.version("ansible-core"):
             return False
-    except pkg_resources.DistributionNotFound:
+    except importlib_metadata.PackageNotFoundError:
         # Must be ansible-base or ansible
         return True
 
 
 @pytest.fixture(scope='session')
 def skipif_pre_ansible211(is_pre_ansible211):
     if is_pre_ansible211:
         pytest.skip("Valid only on Ansible 2.11+")
 
 
 @pytest.fixture(scope="session")
 def is_pre_ansible212():
     try:
-        base_version = (
-            subprocess.run(
-                "python -c 'import ansible; print(ansible.__version__)'",
-                capture_output=True,
-                shell=True,
-            )
-            .stdout.strip()
-            .decode()
-        )
+        base_version = importlib_metadata.version("ansible")
         if Version(base_version) < Version("2.12"):
             return True
-    except pkg_resources.DistributionNotFound:
+    except importlib_metadata.PackageNotFoundError:
         pass
 
 
 @pytest.fixture(scope="session")
 def skipif_pre_ansible212(is_pre_ansible212):
     if is_pre_ansible212:
         pytest.skip("Valid only on Ansible 2.12+")
```

### Comparing `ansible-runner-2.3.2/test/fixtures/projects/host_status/project/gen_host_status.yml` & `ansible-runner-2.3.3/test/fixtures/projects/host_status/project/gen_host_status.yml`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/test/fixtures/projects/printenv/project/action_plugins/look_at_environment.py` & `ansible-runner-2.3.3/test/fixtures/projects/printenv/project/action_plugins/look_at_environment.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/test/integration/conftest.py` & `ansible-runner-2.3.3/test/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/test/integration/containerized/test_cleanup_images.py` & `ansible-runner-2.3.3/test/integration/containerized/test_cleanup_images.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/test/integration/containerized/test_cli_containerized.py` & `ansible-runner-2.3.3/test/integration/containerized/test_cli_containerized.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/test/integration/containerized/test_container_management.py` & `ansible-runner-2.3.3/test/integration/containerized/test_container_management.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/test/integration/exec_env/demo.yml` & `ansible-runner-2.3.3/test/integration/exec_env/demo.yml`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/test/integration/test___main__.py` & `ansible-runner-2.3.3/test/integration/test___main__.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/test/integration/test_config.py` & `ansible-runner-2.3.3/test/integration/test_config.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/test/integration/test_display_callback.py` & `ansible-runner-2.3.3/test/integration/test_display_callback.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/test/integration/test_events.py` & `ansible-runner-2.3.3/test/integration/test_events.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/test/integration/test_interface.py` & `ansible-runner-2.3.3/test/integration/test_interface.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/test/integration/test_main.py` & `ansible-runner-2.3.3/test/integration/test_main.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/test/integration/test_runner.py` & `ansible-runner-2.3.3/test/integration/test_runner.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/test/integration/test_transmit_worker_process.py` & `ansible-runner-2.3.3/test/integration/test_transmit_worker_process.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/test/unit/__main__/main/test_worker.py` & `ansible-runner-2.3.3/test/unit/__main__/main/test_worker.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/test/unit/config/test__base.py` & `ansible-runner-2.3.3/test/unit/config/test__base.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/test/unit/config/test_ansible_cfg.py` & `ansible-runner-2.3.3/test/unit/config/test_ansible_cfg.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/test/unit/config/test_command.py` & `ansible-runner-2.3.3/test/unit/config/test_command.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/test/unit/config/test_container_volmount_generation.py` & `ansible-runner-2.3.3/test/unit/config/test_container_volmount_generation.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/test/unit/config/test_doc.py` & `ansible-runner-2.3.3/test/unit/config/test_doc.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/test/unit/config/test_inventory.py` & `ansible-runner-2.3.3/test/unit/config/test_inventory.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/test/unit/config/test_runner.py` & `ansible-runner-2.3.3/test/unit/config/test_runner.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/test/unit/test_cleanup.py` & `ansible-runner-2.3.3/test/unit/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/test/unit/test_event_filter.py` & `ansible-runner-2.3.3/test/unit/test_event_filter.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/test/unit/test_interface.py` & `ansible-runner-2.3.3/test/unit/test_interface.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/test/unit/test_loader.py` & `ansible-runner-2.3.3/test/unit/test_loader.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/test/unit/test_runner.py` & `ansible-runner-2.3.3/test/unit/test_runner.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/test/unit/utils/capacity/test_uuid.py` & `ansible-runner-2.3.3/test/unit/utils/capacity/test_uuid.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/test/unit/utils/test_cleanup_folder.py` & `ansible-runner-2.3.3/test/unit/utils/test_cleanup_folder.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/test/unit/utils/test_dump_artifacts.py` & `ansible-runner-2.3.3/test/unit/utils/test_dump_artifacts.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/test/unit/utils/test_fifo_pipe.py` & `ansible-runner-2.3.3/test/unit/utils/test_fifo_pipe.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/test/unit/utils/test_utils.py` & `ansible-runner-2.3.3/test/unit/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/test/utils/common.py` & `ansible-runner-2.3.3/test/utils/common.py`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/tools/bindep.txt` & `ansible-runner-2.3.3/tools/bindep.txt`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/tox.ini` & `ansible-runner-2.3.3/tox.ini`

 * *Files identical despite different names*

### Comparing `ansible-runner-2.3.2/utils/entrypoint.sh` & `ansible-runner-2.3.3/utils/entrypoint.sh`

 * *Files identical despite different names*

