# Comparing `tmp/gidgethub-5.2.1.tar.gz` & `tmp/gidgethub-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gidgethub-5.2.1.tar", last modified: Tue Oct  4 21:54:45 2022, max compression
+gzip compressed data, was "gidgethub-5.3.0.tar", last modified: Tue May 30 19:50:10 2023, max compression
```

## Comparing `gidgethub-5.2.1.tar` & `gidgethub-5.3.0.tar`

### file list

```diff
@@ -1,78 +1,79 @@
--rw-r--r--   0        0        0      143 2022-05-27 18:59:43.526291 gidgethub-5.2.1/.github/dependabot.yml
--rw-r--r--   0        0        0        9 2022-05-27 18:59:43.526471 gidgethub-5.2.1/.github/pull_request_template.md
--rw-r--r--   0        0        0     2002 2022-10-04 21:22:02.209144 gidgethub-5.2.1/.github/workflows/main.yml
--rw-r--r--   0        0        0     1154 2022-10-04 21:51:55.767051 gidgethub-5.2.1/.gitignore
--rw-r--r--   0        0        0      412 2022-05-27 18:59:43.527009 gidgethub-5.2.1/.readthedocs.yaml
--rw-r--r--   0        0        0     3328 2022-05-27 18:59:43.527173 gidgethub-5.2.1/CONTRIBUTING.rst
--rw-r--r--   0        0        0    11342 2022-05-27 18:59:43.527408 gidgethub-5.2.1/LICENSE
--rw-r--r--   0        0        0     2082 2022-10-04 21:22:02.209905 gidgethub-5.2.1/README.rst
--rw-r--r--   0        0        0     1257 2022-05-27 18:59:43.527812 gidgethub-5.2.1/Third-Party Notices.md
--rw-r--r--   0        0        0      606 2022-05-27 18:59:43.528060 gidgethub-5.2.1/docs/Makefile
--rw-r--r--   0        0        0     3510 2022-05-27 18:59:43.528259 gidgethub-5.2.1/docs/__init__.rst
--rw-r--r--   0        0        0    11723 2022-05-31 18:55:24.251945 gidgethub-5.2.1/docs/abc.rst
--rw-r--r--   0        0        0     1818 2022-05-27 18:59:43.528661 gidgethub-5.2.1/docs/actions.rst
--rw-r--r--   0        0        0      678 2022-05-27 18:59:43.528817 gidgethub-5.2.1/docs/aiohttp.rst
--rw-r--r--   0        0        0     2036 2022-05-31 18:55:24.252876 gidgethub-5.2.1/docs/apps.rst
--rw-r--r--   0        0        0     7973 2022-10-04 21:30:12.823745 gidgethub-5.2.1/docs/changelog.rst
--rw-r--r--   0        0        0     5482 2022-10-04 21:22:02.211549 gidgethub-5.2.1/docs/conf.py
--rw-r--r--   0        0        0      652 2022-05-27 18:59:43.529482 gidgethub-5.2.1/docs/httpx.rst
--rw-r--r--   0        0        0     4944 2022-05-27 18:59:43.529653 gidgethub-5.2.1/docs/index.rst
--rw-r--r--   0        0        0      813 2022-05-27 18:59:43.529799 gidgethub-5.2.1/docs/make.bat
--rw-r--r--   0        0        0     3251 2022-05-27 18:59:43.529961 gidgethub-5.2.1/docs/routing.rst
--rw-r--r--   0        0        0    10575 2022-10-04 21:22:02.212725 gidgethub-5.2.1/docs/sansio.rst
--rw-r--r--   0        0        0      302 2022-05-27 18:59:43.530357 gidgethub-5.2.1/docs/tornado.rst
--rw-r--r--   0        0        0       38 2022-05-31 20:41:42.712788 gidgethub-5.2.1/docs_requirements.txt
--rw-r--r--   0        0        0     3992 2022-10-04 21:45:30.398026 gidgethub-5.2.1/gidgethub/__init__.py
--rw-r--r--   0        0        0    10633 2022-05-27 18:59:43.530940 gidgethub-5.2.1/gidgethub/abc.py
--rw-r--r--   0        0        0     2721 2022-10-04 21:22:02.214313 gidgethub-5.2.1/gidgethub/actions.py
--rw-r--r--   0        0        0      752 2022-05-27 18:59:43.531286 gidgethub-5.2.1/gidgethub/aiohttp.py
--rw-r--r--   0        0        0     1269 2022-05-27 18:59:43.531459 gidgethub-5.2.1/gidgethub/apps.py
--rw-r--r--   0        0        0      819 2022-05-27 18:59:43.531703 gidgethub-5.2.1/gidgethub/httpx.py
--rw-r--r--   0        0        0        1 2022-05-27 18:59:43.531880 gidgethub-5.2.1/gidgethub/py.typed
--rw-r--r--   0        0        0     3663 2022-05-27 18:59:43.532065 gidgethub-5.2.1/gidgethub/routing.py
--rw-r--r--   0        0        0    15952 2022-10-04 21:22:02.215018 gidgethub-5.2.1/gidgethub/sansio.py
--rw-r--r--   0        0        0     1368 2022-05-27 18:59:43.532548 gidgethub-5.2.1/gidgethub/tornado.py
--rw-r--r--   0        0        0     1177 2022-10-04 21:22:02.215572 gidgethub-5.2.1/noxfile.py
--rw-r--r--   0        0        0     1503 2022-10-04 21:22:02.216139 gidgethub-5.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-05-27 18:59:43.533018 gidgethub-5.2.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2022-05-27 18:59:43.533255 gidgethub-5.2.1/tests/samples/GraphQL/__init__.py
--rw-r--r--   0        0        0      121 2022-05-27 18:59:43.533418 gidgethub-5.2.1/tests/samples/GraphQL/bad-credentials-401.json
--rwxr-xr-x   0        0        0      423 2022-05-27 18:59:43.533564 gidgethub-5.2.1/tests/samples/GraphQL/curl-gql.sh
--rw-r--r--   0        0        0      127 2022-05-27 18:59:43.533713 gidgethub-5.2.1/tests/samples/GraphQL/malformed-json-400.json
--rw-r--r--   0        0        0      251 2022-05-27 18:59:43.533851 gidgethub-5.2.1/tests/samples/GraphQL/malformed-query-200.json
--rw-r--r--   0        0        0      551 2022-05-27 18:59:43.533993 gidgethub-5.2.1/tests/samples/GraphQL/missing-variable-in-request-200.json
--rw-r--r--   0        0        0      474 2022-05-27 18:59:43.534250 gidgethub-5.2.1/tests/samples/GraphQL/success-200.json
--rw-r--r--   0        0        0        0 2022-05-27 18:59:43.534350 gidgethub-5.2.1/tests/samples/__init__.py
--rw-r--r--   0        0        0      584 2022-05-27 18:59:43.534526 gidgethub-5.2.1/tests/samples/convert_headers.py
--rw-r--r--   0        0        0      292 2022-05-27 18:59:43.534764 gidgethub-5.2.1/tests/samples/ping_urlencoded/200.json
--rw-r--r--   0        0        0     8957 2022-05-27 18:59:43.534993 gidgethub-5.2.1/tests/samples/ping_urlencoded/body
--rw-r--r--   0        0        0     1058 2022-05-27 18:59:43.535397 gidgethub-5.2.1/tests/samples/pr_diff/200.json
--rw-r--r--   0        0        0     1555 2022-05-27 18:59:43.535587 gidgethub-5.2.1/tests/samples/pr_diff/body
--rw-r--r--   0        0        0      826 2022-05-27 18:59:43.535859 gidgethub-5.2.1/tests/samples/pr_merged/204.json
--rw-r--r--   0        0        0        0 2022-05-27 18:59:43.535931 gidgethub-5.2.1/tests/samples/pr_merged/body
--rw-r--r--   0        0        0      834 2022-05-27 18:59:43.536152 gidgethub-5.2.1/tests/samples/pr_not_found/404.json
--rw-r--r--   0        0        0      108 2022-05-27 18:59:43.536298 gidgethub-5.2.1/tests/samples/pr_not_found/body
--rw-r--r--   0        0        0     1155 2022-05-27 18:59:43.536527 gidgethub-5.2.1/tests/samples/pr_page_1/200.json
--rw-r--r--   0        0        0   499368 2022-05-27 18:59:43.538989 gidgethub-5.2.1/tests/samples/pr_page_1/body
--rw-r--r--   0        0        0     1304 2022-05-27 18:59:43.539825 gidgethub-5.2.1/tests/samples/pr_page_2/200.json
--rw-r--r--   0        0        0   508127 2022-05-27 18:59:43.541456 gidgethub-5.2.1/tests/samples/pr_page_2/body
--rw-r--r--   0        0        0     1156 2022-05-27 18:59:43.541850 gidgethub-5.2.1/tests/samples/pr_page_last/200.json
--rw-r--r--   0        0        0   101269 2022-05-27 18:59:43.542405 gidgethub-5.2.1/tests/samples/pr_page_last/body
--rw-r--r--   0        0        0     1056 2022-05-27 18:59:43.542764 gidgethub-5.2.1/tests/samples/pr_single/200.json
--rw-r--r--   0        0        0    16964 2022-05-27 18:59:43.543143 gidgethub-5.2.1/tests/samples/pr_single/body
--rw-r--r--   0        0        0        0 2022-05-27 18:59:43.543346 gidgethub-5.2.1/tests/samples/rsa_key/__init__.py
--rw-r--r--   0        0        0     1679 2022-05-27 18:59:43.543527 gidgethub-5.2.1/tests/samples/rsa_key/test_rsa_key
--rw-r--r--   0        0        0     1230 2022-05-27 18:59:43.543778 gidgethub-5.2.1/tests/samples/search_issues_page_1/200.json
--rw-r--r--   0        0        0    11837 2022-05-27 18:59:43.544058 gidgethub-5.2.1/tests/samples/search_issues_page_1/body
--rw-r--r--   0        0        0     1232 2022-05-27 18:59:43.544387 gidgethub-5.2.1/tests/samples/search_issues_page_last/200.json
--rw-r--r--   0        0        0    14621 2022-05-27 18:59:43.544567 gidgethub-5.2.1/tests/samples/search_issues_page_last/body
--rw-r--r--   0        0        0    34758 2022-10-04 21:22:02.216903 gidgethub-5.2.1/tests/test_abc.py
--rw-r--r--   0        0        0     6676 2022-05-27 18:59:43.545056 gidgethub-5.2.1/tests/test_actions.py
--rw-r--r--   0        0        0     1197 2022-05-27 18:59:43.545250 gidgethub-5.2.1/tests/test_aiohttp.py
--rw-r--r--   0        0        0     1479 2022-10-04 21:22:02.217484 gidgethub-5.2.1/tests/test_apps.py
--rw-r--r--   0        0        0     2960 2022-05-27 18:59:43.545620 gidgethub-5.2.1/tests/test_exceptions.py
--rw-r--r--   0        0        0     1168 2022-05-27 18:59:43.545820 gidgethub-5.2.1/tests/test_httpx.py
--rw-r--r--   0        0        0     5811 2022-05-27 18:59:43.546021 gidgethub-5.2.1/tests/test_routing.py
--rw-r--r--   0        0        0    23877 2022-10-04 21:22:02.218116 gidgethub-5.2.1/tests/test_sansio.py
--rw-r--r--   0        0        0     1746 2022-05-27 18:59:43.546557 gidgethub-5.2.1/tests/test_tornado.py
--rw-r--r--   0        0        0     3903 1970-01-01 00:00:00.000000 gidgethub-5.2.1/PKG-INFO
+-rw-r--r--   0        0        0      143 2023-05-30 19:50:02.038423 gidgethub-5.3.0/.github/dependabot.yml
+-rw-r--r--   0        0        0        9 2020-04-19 04:27:14.286567 gidgethub-5.3.0/.github/pull_request_template.md
+-rw-r--r--   0        0        0     2002 2023-05-30 19:50:02.039342 gidgethub-5.3.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1154 2023-05-30 19:50:02.039866 gidgethub-5.3.0/.gitignore
+-rw-r--r--   0        0        0      371 2023-05-30 19:50:02.040072 gidgethub-5.3.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     3328 2023-05-30 19:50:02.040641 gidgethub-5.3.0/CONTRIBUTING.rst
+-rw-r--r--   0        0        0    11342 2020-04-19 04:27:14.286994 gidgethub-5.3.0/LICENSE
+-rw-r--r--   0        0        0     2082 2023-05-30 19:50:02.041047 gidgethub-5.3.0/README.rst
+-rw-r--r--   0        0        0     1257 2020-04-19 04:27:14.287248 gidgethub-5.3.0/Third-Party Notices.md
+-rw-r--r--   0        0        0      606 2020-04-19 04:27:14.287500 gidgethub-5.3.0/docs/Makefile
+-rw-r--r--   0        0        0     3510 2023-05-30 19:50:02.041573 gidgethub-5.3.0/docs/__init__.rst
+-rw-r--r--   0        0        0    12819 2023-05-30 19:50:02.042016 gidgethub-5.3.0/docs/abc.rst
+-rw-r--r--   0        0        0     1818 2023-05-30 19:50:02.042804 gidgethub-5.3.0/docs/actions.rst
+-rw-r--r--   0        0        0      678 2020-04-19 04:27:14.288096 gidgethub-5.3.0/docs/aiohttp.rst
+-rw-r--r--   0        0        0     2069 2023-05-30 19:50:02.043391 gidgethub-5.3.0/docs/apps.rst
+-rw-r--r--   0        0        0     8247 2023-05-30 19:50:02.044200 gidgethub-5.3.0/docs/changelog.rst
+-rw-r--r--   0        0        0     5494 2023-05-30 19:50:02.044624 gidgethub-5.3.0/docs/conf.py
+-rw-r--r--   0        0        0      652 2020-04-19 04:27:14.288762 gidgethub-5.3.0/docs/httpx.rst
+-rw-r--r--   0        0        0     4944 2023-05-30 19:50:02.045334 gidgethub-5.3.0/docs/index.rst
+-rw-r--r--   0        0        0      813 2020-04-19 04:27:14.288998 gidgethub-5.3.0/docs/make.bat
+-rw-r--r--   0        0        0     3251 2023-05-30 19:50:02.045866 gidgethub-5.3.0/docs/routing.rst
+-rw-r--r--   0        0        0    10581 2023-05-30 19:50:02.046305 gidgethub-5.3.0/docs/sansio.rst
+-rw-r--r--   0        0        0      302 2020-04-19 04:27:14.289296 gidgethub-5.3.0/docs/tornado.rst
+-rw-r--r--   0        0        0       38 2023-05-30 19:50:02.046604 gidgethub-5.3.0/docs_requirements.txt
+-rw-r--r--   0        0        0     3992 2023-05-30 19:50:02.047119 gidgethub-5.3.0/gidgethub/__init__.py
+-rw-r--r--   0        0        0    12456 2023-05-30 19:50:02.047625 gidgethub-5.3.0/gidgethub/abc.py
+-rw-r--r--   0        0        0     2721 2023-05-30 19:50:02.048089 gidgethub-5.3.0/gidgethub/actions.py
+-rw-r--r--   0        0        0      752 2020-04-19 04:27:14.289860 gidgethub-5.3.0/gidgethub/aiohttp.py
+-rw-r--r--   0        0        0     1269 2023-05-30 19:50:02.048517 gidgethub-5.3.0/gidgethub/apps.py
+-rw-r--r--   0        0        0      819 2023-05-30 19:50:02.049551 gidgethub-5.3.0/gidgethub/httpx.py
+-rw-r--r--   0        0        0        1 2020-04-19 04:27:14.290135 gidgethub-5.3.0/gidgethub/py.typed
+-rw-r--r--   0        0        0     3663 2023-05-30 19:50:02.050205 gidgethub-5.3.0/gidgethub/routing.py
+-rw-r--r--   0        0        0    15952 2023-05-30 19:50:02.051091 gidgethub-5.3.0/gidgethub/sansio.py
+-rw-r--r--   0        0        0     1368 2020-04-19 04:27:14.290507 gidgethub-5.3.0/gidgethub/tornado.py
+-rw-r--r--   0        0        0     1177 2023-05-30 19:50:02.051870 gidgethub-5.3.0/noxfile.py
+-rw-r--r--   0        0        0     1503 2023-05-30 19:50:02.052395 gidgethub-5.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-04-19 04:27:14.290880 gidgethub-5.3.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-04-19 04:27:14.290994 gidgethub-5.3.0/tests/samples/GraphQL/__init__.py
+-rw-r--r--   0        0        0      121 2023-05-30 19:50:02.052983 gidgethub-5.3.0/tests/samples/GraphQL/bad-credentials-401.json
+-rwxr-xr-x   0        0        0      423 2020-04-19 04:27:14.291257 gidgethub-5.3.0/tests/samples/GraphQL/curl-gql.sh
+-rw-r--r--   0        0        0      127 2023-05-30 19:50:02.053444 gidgethub-5.3.0/tests/samples/GraphQL/malformed-json-400.json
+-rw-r--r--   0        0        0      251 2020-04-19 04:27:14.291417 gidgethub-5.3.0/tests/samples/GraphQL/malformed-query-200.json
+-rw-r--r--   0        0        0      551 2020-04-19 04:27:14.291553 gidgethub-5.3.0/tests/samples/GraphQL/missing-variable-in-request-200.json
+-rw-r--r--   0        0        0      474 2020-04-19 04:27:14.291649 gidgethub-5.3.0/tests/samples/GraphQL/success-200.json
+-rw-r--r--   0        0        0        0 2020-04-19 04:27:14.291696 gidgethub-5.3.0/tests/samples/__init__.py
+-rw-r--r--   0        0        0      584 2020-04-19 04:27:14.291792 gidgethub-5.3.0/tests/samples/convert_headers.py
+-rw-r--r--   0        0        0      292 2020-04-19 04:27:14.292055 gidgethub-5.3.0/tests/samples/ping_urlencoded/200.json
+-rw-r--r--   0        0        0     8957 2020-04-19 04:27:14.292206 gidgethub-5.3.0/tests/samples/ping_urlencoded/body
+-rw-r--r--   0        0        0     1058 2020-04-19 04:27:14.292445 gidgethub-5.3.0/tests/samples/pr_diff/200.json
+-rw-r--r--   0        0        0     1555 2020-04-19 04:27:14.292564 gidgethub-5.3.0/tests/samples/pr_diff/body
+-rw-r--r--   0        0        0      826 2020-04-19 04:27:14.292764 gidgethub-5.3.0/tests/samples/pr_merged/204.json
+-rw-r--r--   0        0        0        0 2020-04-19 04:27:14.292815 gidgethub-5.3.0/tests/samples/pr_merged/body
+-rw-r--r--   0        0        0      834 2020-04-19 04:27:14.292923 gidgethub-5.3.0/tests/samples/pr_not_found/404.json
+-rw-r--r--   0        0        0      108 2023-05-30 19:50:02.053974 gidgethub-5.3.0/tests/samples/pr_not_found/body
+-rw-r--r--   0        0        0     1155 2020-04-19 04:27:14.293126 gidgethub-5.3.0/tests/samples/pr_page_1/200.json
+-rw-r--r--   0        0        0   499368 2020-04-19 04:27:14.295148 gidgethub-5.3.0/tests/samples/pr_page_1/body
+-rw-r--r--   0        0        0     1304 2020-04-19 04:27:14.295368 gidgethub-5.3.0/tests/samples/pr_page_2/200.json
+-rw-r--r--   0        0        0   508127 2020-04-19 04:27:14.296610 gidgethub-5.3.0/tests/samples/pr_page_2/body
+-rw-r--r--   0        0        0     1156 2020-04-19 04:27:14.296824 gidgethub-5.3.0/tests/samples/pr_page_last/200.json
+-rw-r--r--   0        0        0   101269 2020-04-19 04:27:14.297151 gidgethub-5.3.0/tests/samples/pr_page_last/body
+-rw-r--r--   0        0        0     1056 2020-04-19 04:27:14.297375 gidgethub-5.3.0/tests/samples/pr_single/200.json
+-rw-r--r--   0        0        0    16964 2020-04-19 04:27:14.297708 gidgethub-5.3.0/tests/samples/pr_single/body
+-rw-r--r--   0        0        0        0 2020-04-19 04:27:14.297860 gidgethub-5.3.0/tests/samples/rsa_key/__init__.py
+-rw-r--r--   0        0        0     1679 2020-04-19 04:27:14.298005 gidgethub-5.3.0/tests/samples/rsa_key/test_rsa_key
+-rw-r--r--   0        0        0     1230 2020-04-19 04:27:14.298325 gidgethub-5.3.0/tests/samples/search_issues_page_1/200.json
+-rw-r--r--   0        0        0    11837 2020-04-19 04:27:14.298625 gidgethub-5.3.0/tests/samples/search_issues_page_1/body
+-rw-r--r--   0        0        0     1232 2020-04-19 04:27:14.298862 gidgethub-5.3.0/tests/samples/search_issues_page_last/200.json
+-rw-r--r--   0        0        0    14621 2023-05-30 19:50:02.054756 gidgethub-5.3.0/tests/samples/search_issues_page_last/body
+-rw-r--r--   0        0        0    38008 2023-05-30 19:50:02.055774 gidgethub-5.3.0/tests/test_abc.py
+-rw-r--r--   0        0        0     6676 2023-05-30 19:50:02.057242 gidgethub-5.3.0/tests/test_actions.py
+-rw-r--r--   0        0        0     1197 2020-04-19 04:27:14.299657 gidgethub-5.3.0/tests/test_aiohttp.py
+-rw-r--r--   0        0        0     1479 2023-05-30 19:50:02.057641 gidgethub-5.3.0/tests/test_apps.py
+-rw-r--r--   0        0        0     2960 2020-04-19 04:27:14.300109 gidgethub-5.3.0/tests/test_exceptions.py
+-rw-r--r--   0        0        0     1168 2020-04-19 04:27:14.300273 gidgethub-5.3.0/tests/test_httpx.py
+-rw-r--r--   0        0        0     5811 2023-05-30 19:50:02.057977 gidgethub-5.3.0/tests/test_routing.py
+-rw-r--r--   0        0        0    23877 2023-05-30 19:50:02.058368 gidgethub-5.3.0/tests/test_sansio.py
+-rw-r--r--   0        0        0     1746 2023-05-30 19:50:02.059715 gidgethub-5.3.0/tests/test_tornado.py
+-rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 gidgethub-5.3.0/setup.py
+-rw-r--r--   0        0        0      158 1970-01-01 00:00:00.000000 gidgethub-5.3.0/PKG-INFO
```

### Comparing `gidgethub-5.2.1/.github/workflows/main.yml` & `gidgethub-5.3.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/.gitignore` & `gidgethub-5.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/CONTRIBUTING.rst` & `gidgethub-5.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/LICENSE` & `gidgethub-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/README.rst` & `gidgethub-5.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/Third-Party Notices.md` & `gidgethub-5.3.0/Third-Party Notices.md`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/docs/Makefile` & `gidgethub-5.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/docs/__init__.rst` & `gidgethub-5.3.0/docs/__init__.rst`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/docs/abc.rst` & `gidgethub-5.3.0/docs/abc.rst`

 * *Files 3% similar despite different names*

```diff
@@ -44,15 +44,17 @@
     `URI template expansion <https://docs.github.com/en/free-pro-team@latest/rest/overview/resources-in-the-rest-api#hypermedia>`_
     via :func:`gidgethub.sansio.format_url`.The *accept* argument
     specifies what response format is acceptable and can be
     constructed by using :func:`gidgethub.sansio.accept_format`. For
     methods that send data to GitHub, there is a *data* argument which
     accepts an object which can be serialized to JSON (because
     ``None`` is a legitimate JSON value, ``""`` is used to represent
-    no data).
+    no data). The *extra_headers* argument optionally is ``dict[str, str]``,
+    and allows passing extra headers to the request specifying extra
+    options that the GitHub API allows.
 
     The returned value for GitHub requests is the decoded body of the
     response according to :func:`gidgethub.sansio.decipher_response`.
     If the status code returned by the HTTP request is anything other
     than ``200``, ``201``, or ``204``, then an appropriate
     :exc:`~gidgethub.HTTPException` is raised.
 
@@ -115,15 +117,15 @@
         `rate limit <https://docs.github.com/en/free-pro-team@latest/rest/overview/resources-in-the-rest-api#rate-limiting>`_.
 
         .. versionchanged:: 2.0
 
             Renamed from ``_sleep()``.
 
 
-    .. py:method:: getitem(url, url_vars={}, *, accept=sansio.accept_format(), jwt=None, oauth_token=None)
+    .. py:method:: getitem(url, url_vars={}, *, accept=sansio.accept_format(), jwt=None, oauth_token=None, extra_headers=None)
         :async:
 
         Get a single item from GitHub.
 
         *jwt* is the value of the JSON web token, for authenticating as a GitHub
         App.
 
@@ -138,16 +140,35 @@
 
             Added *jwt* and *oauth_token*.
 
         .. note::
             For ``GET`` calls that can return multiple values and
             potentially require pagination, see ``getiter()``.
 
+    .. py:method:: getstatus(url, url_vars={}, *, accept=sansio.accept_format(), jwt=None, oauth_token=None)
+        :async:
+
+        Get a single item's *HTTP status* from GitHub.
+
+        *jwt* is the value of the JSON web token, for authenticating as a GitHub
+        App.
+
+        *oauth_token* is the value of the oauth token, for making an authenticated
+        API call.
+
+        Only one of *oauth_token* or *jwt* may be passed. A ``ValueError`` is
+        raised if both are passed. If neither was passed, it defaults to the
+        value of the *oauth_token* attribute.
+
+        .. note::
+            This method discards any returned content, and is only for use
+            on API endpoints like /orgs/{org}/members/{username} where the
+            HTTP response code is the relevant answer.
 
-    .. py:method:: getiter(url, url_vars={}, *, accept=sansio.accept_format(), jwt=None, oauth_token=None, iterable_key="items")
+    .. py:method:: getiter(url, url_vars={}, *, accept=sansio.accept_format(), jwt=None, oauth_token=None, iterable_key="items", extra_headers=None)
         :async:
 
         Get all items from a GitHub API endpoint.
 
         An asynchronous iterable is returned which will yield all items
         from the endpoint (i.e. use ``async for`` on the result). Any
         `pagination <https://docs.github.com/en/free-pro-team@latest/rest/overview/resources-in-the-rest-api#pagination>`_
@@ -180,15 +201,15 @@
             Added *iterable_key*.
 
         .. note::
             For ``GET`` calls that return only a single item, see
             :meth:`getitem`.
 
 
-    .. py:method:: post(url, url_vars={}, *, data, accept=sansio.accept_format(), jwt=None, oauth_token=None, content_type="application/json")
+    .. py:method:: post(url, url_vars={}, *, data, accept=sansio.accept_format(), jwt=None, oauth_token=None, content_type="application/json", extra_headers=None)
         :async:
 
         Send a ``POST`` request to GitHub.
 
         *jwt* is the value of the JSON web token, for authenticating as a GitHub
         App.
 
@@ -214,15 +235,15 @@
 
 
         .. versionchanged:: 3.0
 
             Added *jwt* and *oauth_token*.
 
 
-    .. py:method:: patch(url, url_vars={}, *, data, accept=sansio.accept_format(), jwt=None, oauth_token=None)
+    .. py:method:: patch(url, url_vars={}, *, data, accept=sansio.accept_format(), jwt=None, oauth_token=None, extra_headers=None)
         :async:
 
         Send a ``PATCH`` request to GitHub.
 
         *jwt* is the value of the JSON web token, for authenticating as a GitHub
         App.
 
@@ -234,15 +255,15 @@
         value of the *oauth_token* attribute.
 
         .. versionchanged:: 3.0
 
             Added *jwt* and *oauth_token*.
 
 
-    .. py:method:: put(url, url_vars={}, *, data=b"", accept=sansio.accept_format(), jwt=None, oauth_token=None)
+    .. py:method:: put(url, url_vars={}, *, data=b"", accept=sansio.accept_format(), jwt=None, oauth_token=None, extra_headers=None)
         :async:
 
         Send a ``PUT`` request to GitHub.
 
         Be aware that some ``PUT`` endpoints such as
         `locking an issue <https://docs.github.com/en/rest/issues/issues#lock-an-issue>`_
         will return no content, leading to ``None`` being returned.
@@ -258,15 +279,15 @@
         value of the *oauth_token* attribute.
 
         .. versionchanged:: 3.0
 
             Added *jwt* and *oauth_token*.
 
 
-    .. py:method:: delete(url, url_vars={}, *, data=b"", accept=sansio.accept_format(), jwt=None, oauth_token=None)
+    .. py:method:: delete(url, url_vars={}, *, data=b"", accept=sansio.accept_format(), jwt=None, oauth_token=None, extra_headers=None)
         :async:
 
         Send a ``DELETE`` request to GitHub.
 
         *jwt* is the value of the JSON web token, for authenticating as a GitHub
         App.
```

### Comparing `gidgethub-5.2.1/docs/actions.rst` & `gidgethub-5.3.0/docs/actions.rst`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/docs/aiohttp.rst` & `gidgethub-5.3.0/docs/aiohttp.rst`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/docs/apps.rst` & `gidgethub-5.3.0/docs/apps.rst`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     **installation_id** is the GitHub App installation's id.
 
     **app_id** is the GitHub App's identifier.
 
     **private_key** is the content of the GitHub App's private key (``.PEM`` format) file.
 
     It returns the response from GitHub's
-    `Authenticating as an installation <https://docs.github.com/en/free-pro-team@latest/developers/apps/authenticating-with-github-apps#authenticating-as-an-installation>`_ API endpoint.
+    `Authenticating as an installation <https://docs.github.com/en/apps/creating-github-apps/authenticating-with-a-github-app/about-authentication-with-a-github-app#authentication-as-an-app-installation>`_ API endpoint.
 
 
 .. function:: get_jwt(*, app_id, private_key)
 
    Construct the JWT (JSON Web Token), that can be used to access endpoints
    that require it.
```

### Comparing `gidgethub-5.2.1/docs/changelog.rst` & `gidgethub-5.3.0/docs/changelog.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 Changelog
 =========
 
+5.3.0
+-----
+
+- Add support passing ``extra_headers`` when making requests
+  (`PR #192 <https://github.com/brettcannon/gidgethub/pull/192>`_)
+
+- Add a getstatus() method for APIs that do not return content.
+  (`PR #194 <https://github.com/brettcannon/gidgethub/pull/194>`_)
+
 5.2.1
 -----
 
 - Fix cgi and importlib_resources deprecations.
-  (`PR #185 <https://github.com/brettcannon/gidgethub/pull/185>_`)
+  (`PR #185 <https://github.com/brettcannon/gidgethub/pull/185>`_)
 
 - Add support for Python 3.11 and drop EOL Python 3.6
-  (`PR #184 <https://github.com/brettcannon/gidgethub/pull/184>_`)
+  (`PR #184 <https://github.com/brettcannon/gidgethub/pull/184>`_)
 
 5.2.0
 -----
 
 - Make the minimum version of PyJWT be v2.4.0.
 
 5.1.0
```

### Comparing `gidgethub-5.2.1/docs/conf.py` & `gidgethub-5.3.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,15 @@
         "One line description of project.",
         "Miscellaneous",
     )
 ]
 
 
 # Example configuration for intersphinx: refer to the Python standard library.
-intersphinx_mapping = {"https://docs.python.org/3/": None}
+intersphinx_mapping = {"python": ("https://docs.python.org/3/", None)}
 
 
 html_sidebars = {
     "**": [
         "about.html",
         "navigation.html",
         "relations.html",
```

### Comparing `gidgethub-5.2.1/docs/httpx.rst` & `gidgethub-5.3.0/docs/httpx.rst`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/docs/index.rst` & `gidgethub-5.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/docs/make.bat` & `gidgethub-5.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/docs/routing.rst` & `gidgethub-5.3.0/docs/routing.rst`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/docs/sansio.rst` & `gidgethub-5.3.0/docs/sansio.rst`

 * *Files 3% similar despite different names*

```diff
@@ -87,19 +87,19 @@
 Requests
 ''''''''
 
 This module provides functions to help in the construction of a URL request
 by helping to automate the GitHub-specific aspects of a REST call.
 ::
 
-  import requests
+  import httpx
 
   request_headers = create_headers("brettcannon", oauth_token=auth)
   url = "https://api.github.com/repos/brettcannon/gidgethub/issues/1"
-  response = requests.get(url, headers=request_headers)
+  response = httpx.get(url, headers=request_headers)
 
 .. function:: accept_format(*, version="v3", media=None, json=True)
 
    Construct the specification of the format that a request should return. This
    is used in the ``accept`` header field of a request to specify the
    `media type <https://docs.github.com/en/free-pro-team@latest/rest/overview/media-types>`_.
 
@@ -138,15 +138,15 @@
 
    The *oauth_token* allows making an
    `authenticated request <https://docs.github.com/en/free-pro-team@latest/rest/overview/resources-in-the-rest-api#authentication>`_.
    This can be important if you need the expanded rate limit provided by an
    authenticated request.
 
    The *jwt* allows making an authenticated request as a `GitHub App
-   <https://docs.github.com/en/free-pro-team@latest/developers/apps/authenticating-with-github-apps#authenticating-as-a-github-app>`_.
+   <https://docs.github.com/en/apps/creating-github-apps/authenticating-with-a-github-app/about-authentication-with-a-github-app#authentication-as-a-github-app>`_.
    You can pass only one: *oauth_token* or *jwt*, but not both.
 
    ``ValueError`` will be raised if both *jwt* and *oauth_token* are supplied.
 
    For consistency, all keys in the returned dict will be lowercased.
 
    .. versionchanged:: 3.0
@@ -156,29 +156,29 @@
 
 Responses
 '''''''''
 
 Decipher a response from the GitHub API gather together all of the details
 that are provided to you. Continuing from the example in the Requests_ section::
 
-  # Assuming `response` contains a requests.Response object.
+  # Assuming `response` contains a httpx.Response object.
   import datetime
 
 
   status_code = response.status_code
   headers = response.headers
   body = response.content
   data, rate, more = decipher_response(status_code, headers, body)
   # Response details are in `data`.
   if more:
       if not rate.remaining:
           now = datetime.datetime.now(datetime.tzinfo.utc)
           wait = rate.reset_datetime - now
           time.sleep(wait.total_seconds())
-      response_more = requests.get(more, headers=request_headers)
+      response_more = httpx.get(more, headers=request_headers)
       # Decipher `response_more` ...
 
 .. class:: RateLimit(*, limit, remaining, reset_epoch)
 
     The `rate limit <https://docs.github.com/en/free-pro-team@latest/rest/overview/resources-in-the-rest-api#rate-limiting>`_ imposed
     upon the requester.
 
@@ -225,18 +225,18 @@
     no errors which lead to an exception being raised, a 3-item tuple
     is returned. The first item is the decoded body (typically a JSON
     object, but possibly ``None`` or a string depending on the content
     type of the body). The second item is a :class:`RateLimit` instance
     based on what the response specified.
 
     The last item of the tuple is the URL where to request the
-    `next set of results <https://docs.github.com/en/free-pro-team@latest/rest/overview/resources-in-the-rest-api#pagination>`_.
+    `next set of results <https://docs.github.com/en/rest/overview/resources-in-the-rest-api?apiVersion=latest#hypermedia>`_.
     If there are no more results then ``None`` is returned. Do be aware
     that the URL
-    `can be a URI template <https://docs.github.com/en/free-pro-team@latest/rest/overview/resources-in-the-rest-api#link-header>`_
+    `can be a URI template <https://docs.github.com/en/rest/overview/resources-in-the-rest-api?apiVersion=latest#hypermedia>`_
     and so it may need to be expanded.
 
     If the status code is anything other than ``200``, ``201``, or ``204``,
     then an appropriate :exc:`~gidgethub.HTTPException` is raised.
 
 
 Utilities
@@ -252,11 +252,11 @@
 
     The dict provided in *url_vars* is used in
     `URI template expansion <https://docs.github.com/en/free-pro-team@latest/rest/overview/resources-in-the-rest-api#hypermedia>`_.
     Appropriate URL quoting is automatically done on the values of the dict.
 
     Enterprise GitHub users can specify their custom base URL in *base_url*.
     By default, https://api.github.com/ is used as the base URL.
-    
+
     .. versionchanged:: 4.0
 
        Added ``base_url`` argument.
```

### Comparing `gidgethub-5.2.1/gidgethub/__init__.py` & `gidgethub-5.3.0/gidgethub/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """An async GitHub API library"""
-__version__ = "5.2.1"
+__version__ = "5.3.0"
 
 import http
 from typing import Any, Optional
 
 
 class GitHubException(Exception):
```

### Comparing `gidgethub-5.2.1/gidgethub/abc.py` & `gidgethub-5.3.0/gidgethub/abc.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from uritemplate import variable
 
 from . import (
     BadGraphQLRequest,
     GitHubBroken,
     GraphQLAuthorizationFailure,
     GraphQLException,
+    HTTPException,
     QueryError,
     GraphQLResponseTypeError,
 )
 from . import sansio
 
 
 # Value represents etag, last-modified, data, and next page.
@@ -61,15 +62,16 @@
         url: str,
         url_vars: Optional[variable.VariableValueDict],
         data: Any,
         accept: str,
         jwt: Opt[str] = None,
         oauth_token: Opt[str] = None,
         content_type: str = JSON_CONTENT_TYPE,
-    ) -> Tuple[bytes, Opt[str]]:
+        extra_headers: Optional[Dict[str, str]] = None,
+    ) -> Tuple[bytes, Opt[str], int]:
         """Construct and make an HTTP request."""
         if oauth_token is not None and jwt is not None:
             raise ValueError("Cannot pass both oauth_token and jwt.")
         filled_url = sansio.format_url(url, url_vars, base_url=self.base_url)
         if jwt is not None:
             request_headers = sansio.create_headers(
                 self.requester, accept=accept, jwt=jwt
@@ -79,14 +81,16 @@
                 self.requester, accept=accept, oauth_token=oauth_token
             )
         else:
             # fallback to using oauth_token
             request_headers = sansio.create_headers(
                 self.requester, accept=accept, oauth_token=self.oauth_token
             )
+        if extra_headers is not None:
+            request_headers.update(extra_headers)
         cached = cacheable = False
         # Can't use None as a "no body" sentinel as it's a legitimate JSON type.
         if data == b"":
             body = b""
             request_headers["content-length"] = "0"
             if method == "GET" and self._cache is not None:
                 cacheable = True
@@ -116,45 +120,81 @@
         if not (response[0] == 304 and cached):
             data, self.rate_limit, more = sansio.decipher_response(*response)
             has_cache_details = "etag" in response[1] or "last-modified" in response[1]
             if self._cache is not None and cacheable and has_cache_details:
                 etag = response[1].get("etag")
                 last_modified = response[1].get("last-modified")
                 self._cache[filled_url] = etag, last_modified, data, more
-        return data, more
+        return data, more, response[0]
 
     async def getitem(
         self,
         url: str,
         url_vars: Optional[variable.VariableValueDict] = {},
         *,
         accept: str = sansio.accept_format(),
         jwt: Opt[str] = None,
         oauth_token: Opt[str] = None,
+        extra_headers: Optional[Dict[str, str]] = None,
     ) -> Any:
         """Send a GET request for a single item to the specified endpoint."""
 
-        data, _ = await self._make_request(
-            "GET", url, url_vars, b"", accept, jwt=jwt, oauth_token=oauth_token
+        data, _, _ = await self._make_request(
+            "GET",
+            url,
+            url_vars,
+            b"",
+            accept,
+            jwt=jwt,
+            oauth_token=oauth_token,
+            extra_headers=extra_headers,
         )
         return data
 
+    async def getstatus(
+        self,
+        url: str,
+        url_vars: Optional[variable.VariableValueDict] = {},
+        *,
+        accept: str = sansio.accept_format(),
+        jwt: Opt[str] = None,
+        oauth_token: Opt[str] = None,
+    ) -> int:
+        """Send a GET request for a single item to the specifie endpoint and return its status code."""
+
+        try:
+            _, _, status_code = await self._make_request(
+                "GET", url, url_vars, b"", accept, jwt=jwt, oauth_token=oauth_token
+            )
+        except HTTPException as e:
+            status_code = e.status_code
+
+        return status_code
+
     async def getiter(
         self,
         url: str,
         url_vars: Optional[variable.VariableValueDict] = {},
         *,
         accept: str = sansio.accept_format(),
         jwt: Opt[str] = None,
         oauth_token: Opt[str] = None,
+        extra_headers: Optional[Dict[str, str]] = None,
         iterable_key: Opt[str] = ITERABLE_KEY,
     ) -> AsyncGenerator[Any, None]:
         """Return an async iterable for all the items at a specified endpoint."""
-        data, more = await self._make_request(
-            "GET", url, url_vars, b"", accept, jwt=jwt, oauth_token=oauth_token
+        data, more, _ = await self._make_request(
+            "GET",
+            url,
+            url_vars,
+            b"",
+            accept,
+            jwt=jwt,
+            oauth_token=oauth_token,
+            extra_headers=extra_headers,
         )
 
         if isinstance(data, dict) and iterable_key in data:
             data = data[iterable_key]
         for item in data:
             yield item
         if more:
@@ -162,82 +202,109 @@
             async for item in self.getiter(
                 more,
                 url_vars,
                 accept=accept,
                 jwt=jwt,
                 oauth_token=oauth_token,
                 iterable_key=iterable_key,
+                extra_headers=extra_headers,
             ):
                 yield item  # pragma: nocover
 
     async def post(
         self,
         url: str,
         url_vars: Optional[variable.VariableValueDict] = {},
         *,
         data: Any,
         accept: str = sansio.accept_format(),
         jwt: Opt[str] = None,
         oauth_token: Opt[str] = None,
+        extra_headers: Optional[Dict[str, str]] = None,
         content_type: str = JSON_CONTENT_TYPE,
     ) -> Any:
-        data, _ = await self._make_request(
+        data, _, _ = await self._make_request(
             "POST",
             url,
             url_vars,
             data,
             accept,
             jwt=jwt,
             oauth_token=oauth_token,
             content_type=content_type,
+            extra_headers=extra_headers,
         )
         return data
 
     async def patch(
         self,
         url: str,
         url_vars: Optional[variable.VariableValueDict] = {},
         *,
         data: Any,
         accept: str = sansio.accept_format(),
         jwt: Opt[str] = None,
         oauth_token: Opt[str] = None,
+        extra_headers: Optional[Dict[str, str]] = None,
     ) -> Any:
-        data, _ = await self._make_request(
-            "PATCH", url, url_vars, data, accept, jwt=jwt, oauth_token=oauth_token
+        data, _, _ = await self._make_request(
+            "PATCH",
+            url,
+            url_vars,
+            data,
+            accept,
+            jwt=jwt,
+            oauth_token=oauth_token,
+            extra_headers=extra_headers,
         )
         return data
 
     async def put(
         self,
         url: str,
         url_vars: Optional[variable.VariableValueDict] = {},
         *,
         data: Any = b"",
         accept: str = sansio.accept_format(),
         jwt: Opt[str] = None,
         oauth_token: Opt[str] = None,
+        extra_headers: Optional[Dict[str, str]] = None,
     ) -> Any:
-        data, _ = await self._make_request(
-            "PUT", url, url_vars, data, accept, jwt=jwt, oauth_token=oauth_token
+        data, _, _ = await self._make_request(
+            "PUT",
+            url,
+            url_vars,
+            data,
+            accept,
+            jwt=jwt,
+            oauth_token=oauth_token,
+            extra_headers=extra_headers,
         )
         return data
 
     async def delete(
         self,
         url: str,
         url_vars: Optional[variable.VariableValueDict] = {},
         *,
         data: Any = b"",
         accept: str = sansio.accept_format(),
         jwt: Opt[str] = None,
         oauth_token: Opt[str] = None,
+        extra_headers: Optional[Dict[str, str]] = None,
     ) -> None:
         await self._make_request(
-            "DELETE", url, url_vars, data, accept, jwt=jwt, oauth_token=oauth_token
+            "DELETE",
+            url,
+            url_vars,
+            data,
+            accept,
+            jwt=jwt,
+            oauth_token=oauth_token,
+            extra_headers=extra_headers,
         )
 
     async def graphql(
         self,
         query: str,
         *,
         endpoint: str = "https://api.github.com/graphql",
```

### Comparing `gidgethub-5.2.1/gidgethub/actions.py` & `gidgethub-5.3.0/gidgethub/actions.py`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/gidgethub/aiohttp.py` & `gidgethub-5.3.0/gidgethub/aiohttp.py`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/gidgethub/apps.py` & `gidgethub-5.3.0/gidgethub/apps.py`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/gidgethub/httpx.py` & `gidgethub-5.3.0/gidgethub/httpx.py`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/gidgethub/routing.py` & `gidgethub-5.3.0/gidgethub/routing.py`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/gidgethub/sansio.py` & `gidgethub-5.3.0/gidgethub/sansio.py`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/gidgethub/tornado.py` & `gidgethub-5.3.0/gidgethub/tornado.py`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/noxfile.py` & `gidgethub-5.3.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/pyproject.toml` & `gidgethub-5.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/tests/samples/GraphQL/missing-variable-in-request-200.json` & `gidgethub-5.3.0/tests/samples/GraphQL/missing-variable-in-request-200.json`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/tests/samples/convert_headers.py` & `gidgethub-5.3.0/tests/samples/convert_headers.py`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/tests/samples/ping_urlencoded/body` & `gidgethub-5.3.0/tests/samples/ping_urlencoded/body`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/tests/samples/pr_diff/200.json` & `gidgethub-5.3.0/tests/samples/pr_diff/200.json`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/tests/samples/pr_diff/body` & `gidgethub-5.3.0/tests/samples/pr_diff/body`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/tests/samples/pr_merged/204.json` & `gidgethub-5.3.0/tests/samples/pr_merged/204.json`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/tests/samples/pr_not_found/404.json` & `gidgethub-5.3.0/tests/samples/pr_not_found/404.json`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/tests/samples/pr_page_1/200.json` & `gidgethub-5.3.0/tests/samples/pr_page_1/200.json`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/tests/samples/pr_page_1/body` & `gidgethub-5.3.0/tests/samples/pr_page_1/body`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/tests/samples/pr_page_2/200.json` & `gidgethub-5.3.0/tests/samples/pr_page_2/200.json`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/tests/samples/pr_page_2/body` & `gidgethub-5.3.0/tests/samples/pr_page_2/body`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/tests/samples/pr_page_last/200.json` & `gidgethub-5.3.0/tests/samples/pr_page_last/200.json`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/tests/samples/pr_page_last/body` & `gidgethub-5.3.0/tests/samples/pr_page_last/body`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/tests/samples/pr_single/200.json` & `gidgethub-5.3.0/tests/samples/pr_single/200.json`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/tests/samples/pr_single/body` & `gidgethub-5.3.0/tests/samples/pr_single/body`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/tests/samples/rsa_key/test_rsa_key` & `gidgethub-5.3.0/tests/samples/rsa_key/test_rsa_key`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/tests/samples/search_issues_page_1/200.json` & `gidgethub-5.3.0/tests/samples/search_issues_page_1/200.json`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/tests/samples/search_issues_page_1/body` & `gidgethub-5.3.0/tests/samples/search_issues_page_1/body`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/tests/samples/search_issues_page_last/200.json` & `gidgethub-5.3.0/tests/samples/search_issues_page_last/200.json`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/tests/samples/search_issues_page_last/body` & `gidgethub-5.3.0/tests/samples/search_issues_page_last/body`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/tests/test_abc.py` & `gidgethub-5.3.0/tests/test_abc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,31 @@
-import asyncio
-import datetime
 import http
 import json
 import re
-import types
 
 import importlib_resources
 import pytest
 
 from gidgethub import (
     BadGraphQLRequest,
     GitHubBroken,
     GraphQLAuthorizationFailure,
     GraphQLException,
+    GraphQLResponseTypeError,
     QueryError,
     RedirectionException,
-    GraphQLResponseTypeError,
+    sansio,
 )
 from gidgethub import abc as gh_abc
-from gidgethub import sansio
+from gidgethub.abc import JSON_UTF_8_CHARSET
 
 from .samples import GraphQL as graphql_samples
 
-from gidgethub.abc import JSON_UTF_8_CHARSET
-
 
 class MockGitHubAPI(gh_abc.GitHubAPI):
-
     DEFAULT_HEADERS = {
         "x-ratelimit-limit": "2",
         "x-ratelimit-remaining": "1",
         "x-ratelimit-reset": "0",
         "content-type": JSON_UTF_8_CHARSET,
     }
 
@@ -165,28 +160,41 @@
         """Test that appropriate decoding occurs."""
         original_data = {"hello": "world"}
         headers = MockGitHubAPI.DEFAULT_HEADERS.copy()
         headers["content-type"] = "application/json; charset=utf-8"
         gh = MockGitHubAPI(
             headers=headers, body=json.dumps(original_data).encode("utf8")
         )
-        data, _ = await gh._make_request(
+        data, _, _ = await gh._make_request(
             "GET", "/rate_limit", {}, "", sansio.accept_format()
         )
         assert data == original_data
 
     @pytest.mark.asyncio
     async def test_more(self):
         """The 'next' link is returned appropriately."""
         headers = MockGitHubAPI.DEFAULT_HEADERS.copy()
         headers["link"] = "<https://api.github.com/fake?page=2>; " 'rel="next"'
         gh = MockGitHubAPI(headers=headers)
-        _, more = await gh._make_request("GET", "/fake", {}, "", sansio.accept_format())
+        _, more, _ = await gh._make_request(
+            "GET", "/fake", {}, "", sansio.accept_format()
+        )
         assert more == "https://api.github.com/fake?page=2"
 
+    @pytest.mark.asyncio
+    async def test_status_code(self):
+        """The status code is returned appropriately."""
+        headers = MockGitHubAPI.DEFAULT_HEADERS.copy()
+        headers["link"] = "<https://api.github.com/fake?page=2>; " 'rel="next"'
+        gh = MockGitHubAPI(headers=headers)
+        _, _, status_code = await gh._make_request(
+            "GET", "/fake", {}, "", sansio.accept_format()
+        )
+        assert status_code == 200
+
 
 class TestGitHubAPIGetitem:
     @pytest.mark.asyncio
     async def test_getitem(self):
         original_data = {"hello": "world"}
         headers = MockGitHubAPI.DEFAULT_HEADERS.copy()
         headers["content-type"] = "application/json; charset=UTF-8"
@@ -233,14 +241,46 @@
             await gh.getitem(
                 "/fake", oauth_token="my oauth token", jwt="json web token"
             )
 
         assert str(exc_info.value) == "Cannot pass both oauth_token and jwt."
 
 
+class TestGitHubAPIGetStatus:
+    @pytest.mark.asyncio
+    async def test_getstatus(self):
+        original_status = 204
+        headers = MockGitHubAPI.DEFAULT_HEADERS.copy()
+        headers["content-type"] = "application/json; charset=UTF-8"
+        gh = MockGitHubAPI(headers=headers, status_code=original_status)
+        data = await gh.getstatus("/fake")
+        assert gh.method == "GET"
+        assert data == original_status
+
+    @pytest.mark.asyncio
+    async def test_getstatus_4xx(self):
+        original_status = 404
+        headers = MockGitHubAPI.DEFAULT_HEADERS.copy()
+        headers["content-type"] = "application/json; charset=UTF-8"
+        gh = MockGitHubAPI(headers=headers, status_code=original_status)
+        data = await gh.getstatus("/fake")
+        assert gh.method == "GET"
+        assert data == original_status
+
+    @pytest.mark.asyncio
+    async def test_getstatus_5xx(self):
+        original_status = 504
+        headers = MockGitHubAPI.DEFAULT_HEADERS.copy()
+        headers["content-type"] = "application/json; charset=UTF-8"
+        gh = MockGitHubAPI(headers=headers, status_code=original_status)
+        data = await gh.getstatus("/fake")
+        assert gh.method == "GET"
+        assert data == original_status
+
+
 class TestGitHubAPIGetiter:
     @pytest.mark.asyncio
     async def test_getiter(self):
         """Test that getiter() returns an async iterable as well as URI expansion."""
         original_data = [1, 2]
         next_url = "https://api.github.com/fake{/extra}?page=2"
         headers = MockGitHubAPI.DEFAULT_HEADERS.copy()
@@ -257,14 +297,39 @@
         assert len(data) == 4
         assert data[0] == 1
         assert data[1] == 2
         assert data[2] == 1
         assert data[3] == 2
 
     @pytest.mark.asyncio
+    async def test_getiter_with_extra_headers(self):
+        """Test that getiter() sends extra headers correctly."""
+        original_data = [1, 2]
+        next_url = "https://api.github.com/fake{/extra}?page=2"
+        headers = MockGitHubAPI.DEFAULT_HEADERS.copy()
+        headers["content-type"] = "application/json; charset=UTF-8"
+        headers["link"] = f'<{next_url}>; rel="next"'
+        gh = MockGitHubAPI(
+            headers=headers, body=json.dumps(original_data).encode("utf8")
+        )
+        extra_headers = {"X-Custom-Header": "custom_value"}
+        data = []
+        async for item in gh.getiter(
+            "/fake", {"extra": "stuff"}, extra_headers=extra_headers
+        ):
+            data.append(item)
+        assert gh.method == "GET"
+        assert gh.headers["X-Custom-Header"] == "custom_value"
+        assert len(data) == 4
+        assert data[0] == 1
+        assert data[1] == 2
+        assert data[2] == 1
+        assert data[3] == 2
+
+    @pytest.mark.asyncio
     async def test_with_passed_jwt(self):
         original_data = [1, 2]
         next_url = "https://api.github.com/fake{/extra}?page=2"
         headers = MockGitHubAPI.DEFAULT_HEADERS.copy()
         headers["content-type"] = "application/json; charset=UTF-8"
         headers["link"] = f'<{next_url}>; rel="next"'
         gh = MockGitHubAPI(
@@ -357,14 +422,28 @@
         assert gh.url == "https://api.github.com/fake/stuff?page=2"
         assert len(data) == 4
         assert data[0] == 1
         assert data[1] == 2
         assert data[2] == 1
         assert data[3] == 2
 
+    @pytest.mark.asyncio
+    async def test_extra_headers(self):
+        """Test that extra headers are passed correctly."""
+        accept = sansio.accept_format()
+        extra_headers = {"X-Custom-Header": "custom_value"}
+        gh = MockGitHubAPI()
+        await gh._make_request(
+            "GET", "/rate_limit", {}, "", accept, extra_headers=extra_headers
+        )
+        assert gh.headers["user-agent"] == "test_abc"
+        assert gh.headers["accept"] == accept
+        assert "X-Custom-Header" in gh.headers
+        assert gh.headers["X-Custom-Header"] == "custom_value"
+
 
 class TestGitHubAPIPost:
     @pytest.mark.asyncio
     async def test_post(self):
         send = [1, 2, 3]
         send_json = json.dumps(send).encode("utf-8")
         receive = {"hello": "world"}
```

### Comparing `gidgethub-5.2.1/tests/test_actions.py` & `gidgethub-5.3.0/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/tests/test_aiohttp.py` & `gidgethub-5.3.0/tests/test_aiohttp.py`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/tests/test_apps.py` & `gidgethub-5.3.0/tests/test_apps.py`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/tests/test_exceptions.py` & `gidgethub-5.3.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/tests/test_httpx.py` & `gidgethub-5.3.0/tests/test_httpx.py`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/tests/test_routing.py` & `gidgethub-5.3.0/tests/test_routing.py`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/tests/test_sansio.py` & `gidgethub-5.3.0/tests/test_sansio.py`

 * *Files identical despite different names*

### Comparing `gidgethub-5.2.1/tests/test_tornado.py` & `gidgethub-5.3.0/tests/test_tornado.py`

 * *Files identical despite different names*

