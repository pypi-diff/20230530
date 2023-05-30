# Comparing `tmp/sfapi_client-0.0.4.tar.gz` & `tmp/sfapi_client-0.0.5.tar.gz`

## Comparing `sfapi_client-0.0.4.tar` & `sfapi_client-0.0.5.tar`

### file list

```diff
@@ -1,86 +1,86 @@
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/LEGAL
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/mkdocs.yml
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/pytest.ini
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/requirements-dev.txt
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/.github/workflows/pypi.yml
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/.github/workflows/pytest.yml
--rwxr-xr-x   0        0        0     1097 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/gen_examples.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/gen_sync.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/index.md
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/community/contributing.md
--rw-r--r--   0        0        0    52808 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/examples/check_current_and_past_jobs.ipynb
--rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/examples/getting_bearer_token.ipynb
--rw-r--r--   0        0        0    11986 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/examples/run_job_and_check_status.ipynb
--rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/javascript/apiselector.js
--rw-r--r--   0        0        0    12002 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/quickstart/index.md
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/reference/SUMMARY.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/reference/async/client/index.md
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/reference/async/compute/index.md
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/reference/async/exceptions/index.md
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/reference/async/groups/index.md
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/reference/async/jobs/index.md
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/reference/async/paths/index.md
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/reference/async/projects/index.md
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/reference/async/resources/index.md
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/docs/reference/async/users/index.md
--rw-r--r--   0        0        0     6448 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/scripts/run.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/__init__.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_compute.py
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_jobs.py
--rw-r--r--   0        0        0     5971 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_monitor.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_utils.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/client.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/compute.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/exceptions.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/groups.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/jobs.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/paths.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/projects.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/resources.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/users.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_async/__init__.py
--rw-r--r--   0        0        0    15934 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_async/client.py
--rw-r--r--   0        0        0     6564 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_async/compute.py
--rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_async/groups.py
--rw-r--r--   0        0        0     7630 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_async/jobs.py
--rw-r--r--   0        0        0    11133 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_async/paths.py
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_async/projects.py
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_async/users.py
--rw-r--r--   0        0        0     8019 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_models/__init__.py
--rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_models/job_status_response_sacct.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_models/job_status_response_squeue.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_models/resources.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_sync/__init__.py
--rw-r--r--   0        0        0    14484 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_sync/_models.py
--rw-r--r--   0        0        0    15536 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_sync/client.py
--rw-r--r--   0        0        0     6318 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_sync/compute.py
--rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_sync/groups.py
--rw-r--r--   0        0        0     7356 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_sync/jobs.py
--rw-r--r--   0        0        0    11414 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_sync/paths.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_sync/projects.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/src/sfapi_client/_sync/users.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/conftest.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_api.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_api_async.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_client.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_client_async.py
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_compute.py
--rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_compute_async.py
--rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_groups.py
--rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_groups_async.py
--rwxr-xr-x   0        0        0     4647 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_jobs.py
--rwxr-xr-x   0        0        0     6378 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_jobs_async.py
--rw-r--r--   0        0        0     8037 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_paths.py
--rw-r--r--   0        0        0     9334 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_paths_async.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_projects.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_projects_async.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_resources.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_resources_async.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_users.py
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/tests/test_users_async.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/.gitignore
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/LICENSE
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/README.md
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 sfapi_client-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/LEGAL
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/mkdocs.yml
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/pytest.ini
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/requirements-dev.txt
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/.github/workflows/pytest.yml
+-rwxr-xr-x   0        0        0     1097 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/docs/gen_examples.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/docs/gen_sync.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/docs/index.md
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/docs/community/contributing.md
+-rw-r--r--   0        0        0    52808 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/docs/examples/check_current_and_past_jobs.ipynb
+-rw-r--r--   0        0        0     3044 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/docs/examples/getting_bearer_token.ipynb
+-rw-r--r--   0        0        0    11986 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/docs/examples/run_job_and_check_status.ipynb
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/docs/javascript/apiselector.js
+-rw-r--r--   0        0        0    12002 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/docs/quickstart/index.md
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/docs/reference/SUMMARY.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/docs/reference/async/client/index.md
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/docs/reference/async/compute/index.md
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/docs/reference/async/exceptions/index.md
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/docs/reference/async/groups/index.md
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/docs/reference/async/jobs/index.md
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/docs/reference/async/paths/index.md
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/docs/reference/async/projects/index.md
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/docs/reference/async/resources/index.md
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/docs/reference/async/users/index.md
+-rw-r--r--   0        0        0     6487 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/scripts/run.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/src/sfapi_client/__init__.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/src/sfapi_client/_compute.py
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/src/sfapi_client/_jobs.py
+-rw-r--r--   0        0        0     5971 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/src/sfapi_client/_monitor.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/src/sfapi_client/_utils.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/src/sfapi_client/client.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/src/sfapi_client/compute.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/src/sfapi_client/exceptions.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/src/sfapi_client/groups.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/src/sfapi_client/jobs.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/src/sfapi_client/paths.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/src/sfapi_client/projects.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/src/sfapi_client/resources.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/src/sfapi_client/users.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/src/sfapi_client/_async/__init__.py
+-rw-r--r--   0        0        0    15934 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/src/sfapi_client/_async/client.py
+-rw-r--r--   0        0        0     6564 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/src/sfapi_client/_async/compute.py
+-rw-r--r--   0        0        0     3754 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/src/sfapi_client/_async/groups.py
+-rw-r--r--   0        0        0     7630 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/src/sfapi_client/_async/jobs.py
+-rw-r--r--   0        0        0    11133 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/src/sfapi_client/_async/paths.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/src/sfapi_client/_async/projects.py
+-rw-r--r--   0        0        0     2908 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/src/sfapi_client/_async/users.py
+-rw-r--r--   0        0        0     8254 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/src/sfapi_client/_models/__init__.py
+-rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/src/sfapi_client/_models/job_status_response_sacct.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/src/sfapi_client/_models/job_status_response_squeue.py
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/src/sfapi_client/_models/resources.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/src/sfapi_client/_sync/__init__.py
+-rw-r--r--   0        0        0    14484 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/src/sfapi_client/_sync/_models.py
+-rw-r--r--   0        0        0    15536 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/src/sfapi_client/_sync/client.py
+-rw-r--r--   0        0        0     6318 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/src/sfapi_client/_sync/compute.py
+-rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/src/sfapi_client/_sync/groups.py
+-rw-r--r--   0        0        0     7356 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/src/sfapi_client/_sync/jobs.py
+-rw-r--r--   0        0        0    11414 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/src/sfapi_client/_sync/paths.py
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/src/sfapi_client/_sync/projects.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/src/sfapi_client/_sync/users.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/tests/conftest.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/tests/test_api.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/tests/test_api_async.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/tests/test_client.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/tests/test_client_async.py
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/tests/test_compute.py
+-rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/tests/test_compute_async.py
+-rw-r--r--   0        0        0     3914 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/tests/test_groups.py
+-rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/tests/test_groups_async.py
+-rwxr-xr-x   0        0        0     4647 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/tests/test_jobs.py
+-rwxr-xr-x   0        0        0     6378 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/tests/test_jobs_async.py
+-rw-r--r--   0        0        0     8037 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/tests/test_paths.py
+-rw-r--r--   0        0        0     9334 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/tests/test_paths_async.py
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/tests/test_projects.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/tests/test_projects_async.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/tests/test_resources.py
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/tests/test_resources_async.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/tests/test_users.py
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/tests/test_users_async.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/.gitignore
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/README.md
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2816 2020-02-02 00:00:00.000000 sfapi_client-0.0.5/PKG-INFO
```

### Comparing `sfapi_client-0.0.4/LEGAL` & `sfapi_client-0.0.5/LEGAL`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/mkdocs.yml` & `sfapi_client-0.0.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/.github/workflows/mkdocs.yml` & `sfapi_client-0.0.5/.github/workflows/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/.github/workflows/pypi.yml` & `sfapi_client-0.0.5/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/.github/workflows/pytest.yml` & `sfapi_client-0.0.5/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/docs/gen_examples.py` & `sfapi_client-0.0.5/docs/gen_examples.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/docs/gen_sync.py` & `sfapi_client-0.0.5/docs/gen_sync.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/docs/index.md` & `sfapi_client-0.0.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/docs/examples/check_current_and_past_jobs.ipynb` & `sfapi_client-0.0.5/docs/examples/check_current_and_past_jobs.ipynb`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/docs/examples/getting_bearer_token.ipynb` & `sfapi_client-0.0.5/docs/examples/getting_bearer_token.ipynb`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/docs/examples/run_job_and_check_status.ipynb` & `sfapi_client-0.0.5/docs/examples/run_job_and_check_status.ipynb`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/docs/javascript/apiselector.js` & `sfapi_client-0.0.5/docs/javascript/apiselector.js`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/docs/quickstart/index.md` & `sfapi_client-0.0.5/docs/quickstart/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/docs/reference/SUMMARY.txt` & `sfapi_client-0.0.5/docs/reference/SUMMARY.txt`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/docs/reference/async/compute/index.md` & `sfapi_client-0.0.5/docs/reference/async/compute/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/docs/reference/async/groups/index.md` & `sfapi_client-0.0.5/docs/reference/async/groups/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/docs/reference/async/jobs/index.md` & `sfapi_client-0.0.5/docs/reference/async/jobs/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/docs/reference/async/paths/index.md` & `sfapi_client-0.0.5/docs/reference/async/paths/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/docs/reference/async/projects/index.md` & `sfapi_client-0.0.5/docs/reference/async/projects/index.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/scripts/run.py` & `sfapi_client-0.0.5/scripts/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         "AsyncApi": "Api",
         "AsyncResources": "Resources",
         "AsyncCompute": "Compute",
         "AsyncGroup": "Group",
         "AsyncGroupMember": "GroupMember",
         "AsyncRemotePath": "RemotePath",
         "AsyncProject": "Project",
+        "AsyncRole": "Role",
         "AsyncUser": "User",
         "AsyncJob": "Job",
         "AsyncJobSacct": "JobSacct",
         "AsyncJobSqueue": "JobSqueue",
         "AsyncOAuth2Client": "OAuth2Client",
         "aclose": "close",
         "_ASYNC_SLEEP": "_SLEEP",
@@ -147,15 +148,16 @@
         / "_models"
         / "resources.py",
         dir_okay=False,
         writable=True,
     ),
 ):
 
-    import requests, datetime
+    import requests
+    import datetime
     api_url = "https://api.nersc.gov/api/v1.2/status"
     response = requests.get(api_url)
     status = response.json()
     names = []
     for s in status:
         name = s['name']
         value = s['name']
```

### Comparing `sfapi_client-0.0.4/src/sfapi_client/_jobs.py` & `sfapi_client-0.0.5/src/sfapi_client/_jobs.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/src/sfapi_client/_monitor.py` & `sfapi_client-0.0.5/src/sfapi_client/_monitor.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/src/sfapi_client/_async/client.py` & `sfapi_client-0.0.5/src/sfapi_client/_async/client.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/src/sfapi_client/_async/compute.py` & `sfapi_client-0.0.5/src/sfapi_client/_async/compute.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/src/sfapi_client/_async/groups.py` & `sfapi_client-0.0.5/src/sfapi_client/_async/groups.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/src/sfapi_client/_async/jobs.py` & `sfapi_client-0.0.5/src/sfapi_client/_async/jobs.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/src/sfapi_client/_async/paths.py` & `sfapi_client-0.0.5/src/sfapi_client/_async/paths.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/src/sfapi_client/_async/projects.py` & `sfapi_client-0.0.5/src/sfapi_client/_async/projects.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 from typing import Optional
 from pydantic import ValidationError, Field
 
 from .._models import (
     ProjectStats as ProjectBase,
+    RoleStats as RoleBase
 )
 from ..exceptions import SfApiError
 
 
+class AsyncRole(RoleBase):
+    client: Optional["AsyncClient"]
+
+
 class AsyncProject(ProjectBase):
     client: Optional["AsyncClient"]
     name: str = Field(alias="repo_name")
 
     async def create_group(self, name: str) -> "AsyncGroup":
         """
         Create a new project.
```

### Comparing `sfapi_client-0.0.4/src/sfapi_client/_async/users.py` & `sfapi_client-0.0.5/src/sfapi_client/_async/users.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Optional, Callable
 from functools import wraps
 
 from .._models import (
     UserInfo as UserBase,
     GroupList as GroupsResponse,
 )
-from .projects import AsyncProject
+from .projects import AsyncProject, AsyncRole
 from ..exceptions import SfApiError
 
 
 def check_auth(method: Callable):
     @wraps(method)
     def wrapper(self, *args, **kwargs):
         if self._client_id is None:
@@ -65,20 +65,41 @@
     async def projects(self) -> List[AsyncProject]:
         """
         The projects the user is associate with.
         """
         if self.name != (await self.client._user()).name:
             raise SfApiError(f"Can only fetch projects for authenticated user.")
 
-        r = await self.client.get("account/roles")
+        r = await self.client.get("account/projects")
 
         json_response = r.json()
 
         projects = [AsyncProject.parse_obj(p) for p in json_response]
 
         def _set_client(p):
             p.client = self.client
             return p
 
         projects = map(_set_client, projects)
 
         return list(projects)
+
+    async def roles(self) -> List[AsyncRole]:
+        """
+        The roles the user is associate with.
+        """
+        if self.name != (await self.client._user()).name:
+            raise SfApiError(f"Can only fetch roles for authenticated user.")
+
+        r = await self.client.get("account/roles")
+
+        json_response = r.json()
+
+        roles = [AsyncRole.parse_obj(p) for p in json_response]
+
+        def _set_client(p):
+            p.client = self.client
+            return p
+
+        roles = map(_set_client, roles)
+
+        return list(roles)
```

### Comparing `sfapi_client-0.0.4/src/sfapi_client/_models/__init__.py` & `sfapi_client-0.0.5/src/sfapi_client/_models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,21 @@
 
 class PublicHost(str, Enum):
     cori = "cori"
     dtn01 = "dtn01"
     perlmutter = "perlmutter"
 
 
+class RoleStats(BaseModel):
+    id: int = Field(..., title="Id")
+    description: str = Field(..., title="Description")
+    repo_name: str = Field(..., title="Repo Name")
+    iris_role: Optional[str] = Field(None, title="Iris Role")
+
+
 class StatusValue(str, Enum):
     active = "active"
     unavailable = "unavailable"
     degraded = "degraded"
     other = "other"
```

### Comparing `sfapi_client-0.0.4/src/sfapi_client/_models/job_status_response_sacct.py` & `sfapi_client-0.0.5/src/sfapi_client/_models/job_status_response_sacct.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/src/sfapi_client/_models/job_status_response_squeue.py` & `sfapi_client-0.0.5/src/sfapi_client/_models/job_status_response_squeue.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/src/sfapi_client/_models/resources.py` & `sfapi_client-0.0.5/src/sfapi_client/_models/resources.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/src/sfapi_client/_sync/_models.py` & `sfapi_client-0.0.5/src/sfapi_client/_sync/_models.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/src/sfapi_client/_sync/client.py` & `sfapi_client-0.0.5/src/sfapi_client/_sync/client.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/src/sfapi_client/_sync/compute.py` & `sfapi_client-0.0.5/src/sfapi_client/_sync/compute.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/src/sfapi_client/_sync/groups.py` & `sfapi_client-0.0.5/src/sfapi_client/_sync/groups.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/src/sfapi_client/_sync/jobs.py` & `sfapi_client-0.0.5/src/sfapi_client/_sync/jobs.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/src/sfapi_client/_sync/paths.py` & `sfapi_client-0.0.5/src/sfapi_client/_sync/paths.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/src/sfapi_client/_sync/projects.py` & `sfapi_client-0.0.5/src/sfapi_client/_sync/projects.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 from typing import Optional
 from pydantic import ValidationError, Field
 
 from .._models import (
     ProjectStats as ProjectBase,
+    RoleStats as RoleBase
 )
 from ..exceptions import SfApiError
 
 
+class Role(RoleBase):
+    client: Optional["Client"]
+
+
 class Project(ProjectBase):
     client: Optional["Client"]
     name: str = Field(alias="repo_name")
 
     def create_group(self, name: str) -> "Group":
         """
         Create a new project.
```

### Comparing `sfapi_client-0.0.4/src/sfapi_client/_sync/users.py` & `sfapi_client-0.0.5/src/sfapi_client/_sync/users.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Optional, Callable
 from functools import wraps
 
 from .._models import (
     UserInfo as UserBase,
     GroupList as GroupsResponse,
 )
-from .projects import Project
+from .projects import Project, Role
 from ..exceptions import SfApiError
 
 
 def check_auth(method: Callable):
     @wraps(method)
     def wrapper(self, *args, **kwargs):
         if self._client_id is None:
@@ -65,20 +65,41 @@
     def projects(self) -> List[Project]:
         """
         The projects the user is associate with.
         """
         if self.name != (self.client._user()).name:
             raise SfApiError(f"Can only fetch projects for authenticated user.")
 
-        r = self.client.get("account/roles")
+        r = self.client.get("account/projects")
 
         json_response = r.json()
 
         projects = [Project.parse_obj(p) for p in json_response]
 
         def _set_client(p):
             p.client = self.client
             return p
 
         projects = map(_set_client, projects)
 
         return list(projects)
+
+    def roles(self) -> List[Role]:
+        """
+        The roles the user is associate with.
+        """
+        if self.name != (self.client._user()).name:
+            raise SfApiError(f"Can only fetch roles for authenticated user.")
+
+        r = self.client.get("account/roles")
+
+        json_response = r.json()
+
+        roles = [Role.parse_obj(p) for p in json_response]
+
+        def _set_client(p):
+            p.client = self.client
+            return p
+
+        roles = map(_set_client, roles)
+
+        return list(roles)
```

### Comparing `sfapi_client-0.0.4/tests/conftest.py` & `sfapi_client-0.0.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/tests/test_compute.py` & `sfapi_client-0.0.5/tests/test_compute.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/tests/test_compute_async.py` & `sfapi_client-0.0.5/tests/test_compute_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/tests/test_groups.py` & `sfapi_client-0.0.5/tests/test_groups.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/tests/test_groups_async.py` & `sfapi_client-0.0.5/tests/test_groups_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/tests/test_jobs.py` & `sfapi_client-0.0.5/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/tests/test_jobs_async.py` & `sfapi_client-0.0.5/tests/test_jobs_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/tests/test_paths.py` & `sfapi_client-0.0.5/tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/tests/test_paths_async.py` & `sfapi_client-0.0.5/tests/test_paths_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/tests/test_projects_async.py` & `sfapi_client-0.0.5/tests/test_projects_async.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,7 +22,27 @@
                 break
 
         assert project
 
         group = await project.create_group(test_group_create)
 
         assert group.name == test_create_group
+
+
+@pytest.mark.asyncio
+async def test_projects(
+    client_id, client_secret
+):
+    async with AsyncClient(client_id, client_secret) as client:
+        user = await client.user()
+        projects = await user.projects()
+        assert projects
+
+
+@pytest.mark.asyncio
+async def test_roles(
+    client_id, client_secret
+):
+    async with AsyncClient(client_id, client_secret) as client:
+        user = await client.user()
+        roles = await user.roles()
+        assert roles
```

### Comparing `sfapi_client-0.0.4/tests/test_resources.py` & `sfapi_client-0.0.5/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/tests/test_resources_async.py` & `sfapi_client-0.0.5/tests/test_resources_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/tests/test_users.py` & `sfapi_client-0.0.5/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/tests/test_users_async.py` & `sfapi_client-0.0.5/tests/test_users_async.py`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/LICENSE` & `sfapi_client-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/README.md` & `sfapi_client-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/pyproject.toml` & `sfapi_client-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sfapi_client-0.0.4/PKG-INFO` & `sfapi_client-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sfapi_client
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python client for NERSC SF API
 Author-email: Chris Harris <cjh@lbl.gov>, Nicholas Tyler <tylern@lbl.gov>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

