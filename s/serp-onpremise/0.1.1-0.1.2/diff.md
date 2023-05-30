# Comparing `tmp/serp_onpremise-0.1.1.tar.gz` & `tmp/serp_onpremise-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serp_onpremise-0.1.1.tar", last modified: Tue May 30 13:16:27 2023, max compression
+gzip compressed data, was "serp_onpremise-0.1.2.tar", max compression
```

## Comparing `serp_onpremise-0.1.1.tar` & `serp_onpremise-0.1.2.tar`

### file list

```diff
@@ -1,81 +1,42 @@
-drwxr-xr-x   0 golishchev   (501) staff       (20)        0 2023-05-30 13:16:27.851212 serp_onpremise-0.1.1/
--rw-r--r--   0 golishchev   (501) staff       (20)     1036 2023-05-30 11:09:39.000000 serp_onpremise-0.1.1/LICENSE
--rw-r--r--   0 golishchev   (501) staff       (20)     3819 2023-05-30 13:16:27.851400 serp_onpremise-0.1.1/PKG-INFO
--rw-r--r--   0 golishchev   (501) staff       (20)     3400 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/README.md
--rw-r--r--   0 golishchev   (501) staff       (20)      686 2023-05-30 13:02:49.000000 serp_onpremise-0.1.1/pyproject.toml
-drwxr-xr-x   0 golishchev   (501) staff       (20)        0 2023-05-30 13:16:27.841307 serp_onpremise-0.1.1/serp_onpremise/
--rw-r--r--   0 golishchev   (501) staff       (20)      217 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/__init__.py
-drwxr-xr-x   0 golishchev   (501) staff       (20)        0 2023-05-30 13:16:27.842326 serp_onpremise-0.1.1/serp_onpremise/asm/
--rw-r--r--   0 golishchev   (501) staff       (20)        0 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/asm/__init__.py
--rw-r--r--   0 golishchev   (501) staff       (20)      766 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/asm/v1.py
-drwxr-xr-x   0 golishchev   (501) staff       (20)        0 2023-05-30 13:16:27.842790 serp_onpremise-0.1.1/serp_onpremise/auth/
--rw-r--r--   0 golishchev   (501) staff       (20)        0 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/auth/__init__.py
--rw-r--r--   0 golishchev   (501) staff       (20)     2056 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/auth/v1.py
--rw-r--r--   0 golishchev   (501) staff       (20)      644 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/auth_token.py
--rw-r--r--   0 golishchev   (501) staff       (20)      374 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/base.py
--rw-r--r--   0 golishchev   (501) staff       (20)     3174 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/clients.py
-drwxr-xr-x   0 golishchev   (501) staff       (20)        0 2023-05-30 13:16:27.843164 serp_onpremise-0.1.1/serp_onpremise/compare/
--rw-r--r--   0 golishchev   (501) staff       (20)        0 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/compare/__init__.py
--rw-r--r--   0 golishchev   (501) staff       (20)     1040 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/compare/v1.py
--rw-r--r--   0 golishchev   (501) staff       (20)      437 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/constants.py
-drwxr-xr-x   0 golishchev   (501) staff       (20)        0 2023-05-30 13:16:27.843563 serp_onpremise-0.1.1/serp_onpremise/entries/
--rw-r--r--   0 golishchev   (501) staff       (20)        0 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/entries/__init__.py
--rw-r--r--   0 golishchev   (501) staff       (20)     2035 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/entries/v1.py
-drwxr-xr-x   0 golishchev   (501) staff       (20)        0 2023-05-30 13:16:27.843937 serp_onpremise-0.1.1/serp_onpremise/groups_profiles/
--rw-r--r--   0 golishchev   (501) staff       (20)        0 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/groups_profiles/__init__.py
--rw-r--r--   0 golishchev   (501) staff       (20)     5156 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/groups_profiles/v1.py
-drwxr-xr-x   0 golishchev   (501) staff       (20)        0 2023-05-30 13:16:27.844550 serp_onpremise-0.1.1/serp_onpremise/licenses/
--rw-r--r--   0 golishchev   (501) staff       (20)        0 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/licenses/__init__.py
--rw-r--r--   0 golishchev   (501) staff       (20)     1080 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/licenses/v1.py
-drwxr-xr-x   0 golishchev   (501) staff       (20)        0 2023-05-30 13:16:27.845278 serp_onpremise-0.1.1/serp_onpremise/liveness/
--rw-r--r--   0 golishchev   (501) staff       (20)        0 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/liveness/__init__.py
--rw-r--r--   0 golishchev   (501) staff       (20)     1044 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/liveness/v1.py
-drwxr-xr-x   0 golishchev   (501) staff       (20)        0 2023-05-30 13:16:27.845879 serp_onpremise-0.1.1/serp_onpremise/origins/
--rw-r--r--   0 golishchev   (501) staff       (20)        0 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/origins/__init__.py
--rw-r--r--   0 golishchev   (501) staff       (20)     6143 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/origins/v1.py
-drwxr-xr-x   0 golishchev   (501) staff       (20)        0 2023-05-30 13:16:27.846218 serp_onpremise-0.1.1/serp_onpremise/profiles/
--rw-r--r--   0 golishchev   (501) staff       (20)        0 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/profiles/__init__.py
--rw-r--r--   0 golishchev   (501) staff       (20)     4306 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/profiles/v1.py
-drwxr-xr-x   0 golishchev   (501) staff       (20)        0 2023-05-30 13:16:27.846549 serp_onpremise-0.1.1/serp_onpremise/spaces/
--rw-r--r--   0 golishchev   (501) staff       (20)        0 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/spaces/__init__.py
--rw-r--r--   0 golishchev   (501) staff       (20)     5344 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/spaces/v1.py
-drwxr-xr-x   0 golishchev   (501) staff       (20)        0 2023-05-30 13:16:27.846864 serp_onpremise-0.1.1/serp_onpremise/statistics/
--rw-r--r--   0 golishchev   (501) staff       (20)        0 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/statistics/__init__.py
--rw-r--r--   0 golishchev   (501) staff       (20)      561 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/statistics/v1.py
-drwxr-xr-x   0 golishchev   (501) staff       (20)        0 2023-05-30 13:16:27.847475 serp_onpremise-0.1.1/serp_onpremise/tokens/
--rw-r--r--   0 golishchev   (501) staff       (20)        0 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/tokens/__init__.py
-drwxr-xr-x   0 golishchev   (501) staff       (20)        0 2023-05-30 13:16:27.847663 serp_onpremise-0.1.1/serp_onpremise/tokens/access/
--rw-r--r--   0 golishchev   (501) staff       (20)        0 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/tokens/access/__init__.py
--rw-r--r--   0 golishchev   (501) staff       (20)     3260 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/tokens/access/v1.py
-drwxr-xr-x   0 golishchev   (501) staff       (20)        0 2023-05-30 13:16:27.848008 serp_onpremise-0.1.1/serp_onpremise/tokens/streams/
--rw-r--r--   0 golishchev   (501) staff       (20)        0 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/tokens/streams/__init__.py
--rw-r--r--   0 golishchev   (501) staff       (20)     3262 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/tokens/streams/v1.py
-drwxr-xr-x   0 golishchev   (501) staff       (20)        0 2023-05-30 13:16:27.848308 serp_onpremise-0.1.1/serp_onpremise/users/
--rw-r--r--   0 golishchev   (501) staff       (20)        0 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/users/__init__.py
--rw-r--r--   0 golishchev   (501) staff       (20)     1981 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/users/v1.py
--rw-r--r--   0 golishchev   (501) staff       (20)     2316 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/utils.py
-drwxr-xr-x   0 golishchev   (501) staff       (20)        0 2023-05-30 13:16:27.848563 serp_onpremise-0.1.1/serp_onpremise/whoami/
--rw-r--r--   0 golishchev   (501) staff       (20)        0 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/whoami/__init__.py
--rw-r--r--   0 golishchev   (501) staff       (20)      545 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/serp_onpremise/whoami/v1.py
-drwxr-xr-x   0 golishchev   (501) staff       (20)        0 2023-05-30 13:16:27.841988 serp_onpremise-0.1.1/serp_onpremise.egg-info/
--rw-r--r--   0 golishchev   (501) staff       (20)     3819 2023-05-30 13:16:27.000000 serp_onpremise-0.1.1/serp_onpremise.egg-info/PKG-INFO
--rw-r--r--   0 golishchev   (501) staff       (20)     1675 2023-05-30 13:16:27.000000 serp_onpremise-0.1.1/serp_onpremise.egg-info/SOURCES.txt
--rw-r--r--   0 golishchev   (501) staff       (20)        1 2023-05-30 13:16:27.000000 serp_onpremise-0.1.1/serp_onpremise.egg-info/dependency_links.txt
--rw-r--r--   0 golishchev   (501) staff       (20)       21 2023-05-30 13:16:27.000000 serp_onpremise-0.1.1/serp_onpremise.egg-info/top_level.txt
--rw-r--r--   0 golishchev   (501) staff       (20)       38 2023-05-30 13:16:27.851730 serp_onpremise-0.1.1/setup.cfg
--rw-r--r--   0 golishchev   (501) staff       (20)      594 2023-05-30 13:16:20.000000 serp_onpremise-0.1.1/setup.py
-drwxr-xr-x   0 golishchev   (501) staff       (20)        0 2023-05-30 13:16:27.851063 serp_onpremise-0.1.1/tests/
--rw-r--r--   0 golishchev   (501) staff       (20)        0 2023-05-30 11:09:39.000000 serp_onpremise-0.1.1/tests/__init__.py
--rw-r--r--   0 golishchev   (501) staff       (20)      906 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/tests/conftest.py
--rw-r--r--   0 golishchev   (501) staff       (20)     1686 2023-05-30 11:09:39.000000 serp_onpremise-0.1.1/tests/test_auth.py
--rw-r--r--   0 golishchev   (501) staff       (20)     5405 2023-05-30 11:09:39.000000 serp_onpremise-0.1.1/tests/test_entries.py
--rw-r--r--   0 golishchev   (501) staff       (20)     9405 2023-05-30 11:09:39.000000 serp_onpremise-0.1.1/tests/test_groups.py
--rw-r--r--   0 golishchev   (501) staff       (20)     7164 2023-05-30 11:09:39.000000 serp_onpremise-0.1.1/tests/test_origins.py
--rw-r--r--   0 golishchev   (501) staff       (20)     5792 2023-05-30 11:09:39.000000 serp_onpremise-0.1.1/tests/test_profiles.py
--rw-r--r--   0 golishchev   (501) staff       (20)     7014 2023-05-30 11:09:39.000000 serp_onpremise-0.1.1/tests/test_spaces.py
--rw-r--r--   0 golishchev   (501) staff       (20)      368 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/tests/test_sync_client.py
--rw-r--r--   0 golishchev   (501) staff       (20)     9926 2023-05-30 11:09:39.000000 serp_onpremise-0.1.1/tests/test_tokens.py
--rw-r--r--   0 golishchev   (501) staff       (20)     1672 2023-05-30 11:09:39.000000 serp_onpremise-0.1.1/tests/test_utility.py
--rw-r--r--   0 golishchev   (501) staff       (20)     3582 2023-05-30 12:54:13.000000 serp_onpremise-0.1.1/tests/test_utils.py
--rw-r--r--   0 golishchev   (501) staff       (20)      758 2023-05-30 11:09:39.000000 serp_onpremise-0.1.1/tests/test_whoami.py
--rw-r--r--   0 golishchev   (501) staff       (20)      416 2023-05-30 11:09:39.000000 serp_onpremise-0.1.1/tests/utils.py
+-rw-r--r--   0        0        0     1036 2023-05-30 11:09:39.464443 serp_onpremise-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3400 2023-05-30 12:54:13.756392 serp_onpremise-0.1.2/README.md
+-rw-r--r--   0        0        0      704 2023-05-30 13:38:55.087337 serp_onpremise-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      217 2023-05-30 12:54:13.759095 serp_onpremise-0.1.2/serp_onpremise/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 12:54:13.759173 serp_onpremise-0.1.2/serp_onpremise/asm/__init__.py
+-rw-r--r--   0        0        0      766 2023-05-30 12:54:13.759330 serp_onpremise-0.1.2/serp_onpremise/asm/v1.py
+-rw-r--r--   0        0        0        0 2023-05-30 12:54:13.759397 serp_onpremise-0.1.2/serp_onpremise/auth/__init__.py
+-rw-r--r--   0        0        0     2056 2023-05-30 12:54:13.759552 serp_onpremise-0.1.2/serp_onpremise/auth/v1.py
+-rw-r--r--   0        0        0      644 2023-05-30 12:54:13.759629 serp_onpremise-0.1.2/serp_onpremise/auth_token.py
+-rw-r--r--   0        0        0      374 2023-05-30 12:54:13.759700 serp_onpremise-0.1.2/serp_onpremise/base.py
+-rw-r--r--   0        0        0     3174 2023-05-30 12:54:13.759880 serp_onpremise-0.1.2/serp_onpremise/clients.py
+-rw-r--r--   0        0        0        0 2023-05-30 12:54:13.759957 serp_onpremise-0.1.2/serp_onpremise/compare/__init__.py
+-rw-r--r--   0        0        0     1040 2023-05-30 12:54:13.760114 serp_onpremise-0.1.2/serp_onpremise/compare/v1.py
+-rw-r--r--   0        0        0      437 2023-05-30 12:54:13.760188 serp_onpremise-0.1.2/serp_onpremise/constants.py
+-rw-r--r--   0        0        0        0 2023-05-30 12:54:13.760261 serp_onpremise-0.1.2/serp_onpremise/entries/__init__.py
+-rw-r--r--   0        0        0     2035 2023-05-30 12:54:13.760614 serp_onpremise-0.1.2/serp_onpremise/entries/v1.py
+-rw-r--r--   0        0        0        0 2023-05-30 12:54:13.760703 serp_onpremise-0.1.2/serp_onpremise/groups_profiles/__init__.py
+-rw-r--r--   0        0        0     5156 2023-05-30 12:54:13.760892 serp_onpremise-0.1.2/serp_onpremise/groups_profiles/v1.py
+-rw-r--r--   0        0        0        0 2023-05-30 12:54:13.760971 serp_onpremise-0.1.2/serp_onpremise/licenses/__init__.py
+-rw-r--r--   0        0        0     1080 2023-05-30 12:54:13.761123 serp_onpremise-0.1.2/serp_onpremise/licenses/v1.py
+-rw-r--r--   0        0        0        0 2023-05-30 12:54:13.761196 serp_onpremise-0.1.2/serp_onpremise/liveness/__init__.py
+-rw-r--r--   0        0        0     1044 2023-05-30 12:54:13.761342 serp_onpremise-0.1.2/serp_onpremise/liveness/v1.py
+-rw-r--r--   0        0        0        0 2023-05-30 12:54:13.761413 serp_onpremise-0.1.2/serp_onpremise/origins/__init__.py
+-rw-r--r--   0        0        0     6143 2023-05-30 12:54:13.761583 serp_onpremise-0.1.2/serp_onpremise/origins/v1.py
+-rw-r--r--   0        0        0        0 2023-05-30 12:54:13.761646 serp_onpremise-0.1.2/serp_onpremise/profiles/__init__.py
+-rw-r--r--   0        0        0     4306 2023-05-30 12:54:13.761875 serp_onpremise-0.1.2/serp_onpremise/profiles/v1.py
+-rw-r--r--   0        0        0        0 2023-05-30 12:54:13.761991 serp_onpremise-0.1.2/serp_onpremise/spaces/__init__.py
+-rw-r--r--   0        0        0     5344 2023-05-30 12:54:13.762203 serp_onpremise-0.1.2/serp_onpremise/spaces/v1.py
+-rw-r--r--   0        0        0        0 2023-05-30 12:54:13.762279 serp_onpremise-0.1.2/serp_onpremise/statistics/__init__.py
+-rw-r--r--   0        0        0      561 2023-05-30 12:54:13.762447 serp_onpremise-0.1.2/serp_onpremise/statistics/v1.py
+-rw-r--r--   0        0        0        0 2023-05-30 12:54:13.762529 serp_onpremise-0.1.2/serp_onpremise/tokens/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-30 12:54:13.762611 serp_onpremise-0.1.2/serp_onpremise/tokens/access/__init__.py
+-rw-r--r--   0        0        0     3260 2023-05-30 12:54:13.762780 serp_onpremise-0.1.2/serp_onpremise/tokens/access/v1.py
+-rw-r--r--   0        0        0        0 2023-05-30 12:54:13.762847 serp_onpremise-0.1.2/serp_onpremise/tokens/streams/__init__.py
+-rw-r--r--   0        0        0     3262 2023-05-30 12:54:13.763006 serp_onpremise-0.1.2/serp_onpremise/tokens/streams/v1.py
+-rw-r--r--   0        0        0        0 2023-05-30 12:54:13.763084 serp_onpremise-0.1.2/serp_onpremise/users/__init__.py
+-rw-r--r--   0        0        0     1981 2023-05-30 12:54:13.763244 serp_onpremise-0.1.2/serp_onpremise/users/v1.py
+-rw-r--r--   0        0        0     2316 2023-05-30 12:54:13.763402 serp_onpremise-0.1.2/serp_onpremise/utils.py
+-rw-r--r--   0        0        0        0 2023-05-30 12:54:13.763477 serp_onpremise-0.1.2/serp_onpremise/whoami/__init__.py
+-rw-r--r--   0        0        0      545 2023-05-30 12:54:13.763644 serp_onpremise-0.1.2/serp_onpremise/whoami/v1.py
+-rw-r--r--   0        0        0     4678 1970-01-01 00:00:00.000000 serp_onpremise-0.1.2/setup.py
+-rw-r--r--   0        0        0     4045 1970-01-01 00:00:00.000000 serp_onpremise-0.1.2/PKG-INFO
```

### Comparing `serp_onpremise-0.1.1/LICENSE` & `serp_onpremise-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `serp_onpremise-0.1.1/PKG-INFO` & `serp_onpremise-0.1.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: serp_onpremise
-Version: 0.1.1
-Summary: Python API client for SERP on-premise API
-Home-page: https://serptech.ru
-Author: astrotourist
-Author-email: d@orbl.io
-Classifier: Programming Language :: Python :: 3.7
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Python API client for SERP on-premise API
 
 ---
 
 This library is mirror of official SERP on-premise API in terms of methods and interfaces.
 
 For your convenience, you can make API calls using sync or async (asyncio) interface.
```

### Comparing `serp_onpremise-0.1.1/pyproject.toml` & `serp_onpremise-0.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tool.poetry]
 name = "serp_onpremise"
-version = "0.1.1"
+version = "0.1.2"
 description = "A Python package for interacting with SERP on-premise API"
 authors = ["serptech.ru"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.7.0"
+python = "^3.8.0"
 httpx = ">=0.19.0"
 websockets = "^10.0"
+sphinx = "^7.0.1"
 
 [tool.poetry.dev-dependencies]
 bandit = "^1.7.0"
 safety = "^1.10.3"
 isort = "^5.9.3"
 flake8 = "^5.0.4"
 black = {version = "^22.3", allow-prereleases = true}
```

### Comparing `serp_onpremise-0.1.1/serp_onpremise/asm/v1.py` & `serp_onpremise-0.1.2/serp_onpremise/asm/v1.py`

 * *Files identical despite different names*

### Comparing `serp_onpremise-0.1.1/serp_onpremise/auth/v1.py` & `serp_onpremise-0.1.2/serp_onpremise/auth/v1.py`

 * *Files identical despite different names*

### Comparing `serp_onpremise-0.1.1/serp_onpremise/auth_token.py` & `serp_onpremise-0.1.2/serp_onpremise/auth_token.py`

 * *Files identical despite different names*

### Comparing `serp_onpremise-0.1.1/serp_onpremise/clients.py` & `serp_onpremise-0.1.2/serp_onpremise/clients.py`

 * *Files identical despite different names*

### Comparing `serp_onpremise-0.1.1/serp_onpremise/compare/v1.py` & `serp_onpremise-0.1.2/serp_onpremise/compare/v1.py`

 * *Files identical despite different names*

### Comparing `serp_onpremise-0.1.1/serp_onpremise/entries/v1.py` & `serp_onpremise-0.1.2/serp_onpremise/entries/v1.py`

 * *Files identical despite different names*

### Comparing `serp_onpremise-0.1.1/serp_onpremise/groups_profiles/v1.py` & `serp_onpremise-0.1.2/serp_onpremise/groups_profiles/v1.py`

 * *Files identical despite different names*

### Comparing `serp_onpremise-0.1.1/serp_onpremise/licenses/v1.py` & `serp_onpremise-0.1.2/serp_onpremise/licenses/v1.py`

 * *Files identical despite different names*

### Comparing `serp_onpremise-0.1.1/serp_onpremise/liveness/v1.py` & `serp_onpremise-0.1.2/serp_onpremise/liveness/v1.py`

 * *Files identical despite different names*

### Comparing `serp_onpremise-0.1.1/serp_onpremise/origins/v1.py` & `serp_onpremise-0.1.2/serp_onpremise/origins/v1.py`

 * *Files identical despite different names*

### Comparing `serp_onpremise-0.1.1/serp_onpremise/profiles/v1.py` & `serp_onpremise-0.1.2/serp_onpremise/profiles/v1.py`

 * *Files identical despite different names*

### Comparing `serp_onpremise-0.1.1/serp_onpremise/spaces/v1.py` & `serp_onpremise-0.1.2/serp_onpremise/spaces/v1.py`

 * *Files identical despite different names*

### Comparing `serp_onpremise-0.1.1/serp_onpremise/statistics/v1.py` & `serp_onpremise-0.1.2/serp_onpremise/statistics/v1.py`

 * *Files identical despite different names*

### Comparing `serp_onpremise-0.1.1/serp_onpremise/tokens/access/v1.py` & `serp_onpremise-0.1.2/serp_onpremise/tokens/access/v1.py`

 * *Files identical despite different names*

### Comparing `serp_onpremise-0.1.1/serp_onpremise/tokens/streams/v1.py` & `serp_onpremise-0.1.2/serp_onpremise/tokens/streams/v1.py`

 * *Files identical despite different names*

### Comparing `serp_onpremise-0.1.1/serp_onpremise/users/v1.py` & `serp_onpremise-0.1.2/serp_onpremise/users/v1.py`

 * *Files identical despite different names*

### Comparing `serp_onpremise-0.1.1/serp_onpremise/utils.py` & `serp_onpremise-0.1.2/serp_onpremise/utils.py`

 * *Files identical despite different names*

### Comparing `serp_onpremise-0.1.1/serp_onpremise/whoami/v1.py` & `serp_onpremise-0.1.2/serp_onpremise/whoami/v1.py`

 * *Files identical despite different names*

### Comparing `serp_onpremise-0.1.1/serp_onpremise.egg-info/PKG-INFO` & `serp_onpremise-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: serp-onpremise
-Version: 0.1.1
-Summary: Python API client for SERP on-premise API
-Home-page: https://serptech.ru
-Author: astrotourist
-Author-email: d@orbl.io
-Classifier: Programming Language :: Python :: 3.7
+Version: 0.1.2
+Summary: A Python package for interacting with SERP on-premise API
+License: MIT
+Author: serptech.ru
+Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: httpx (>=0.19.0)
+Requires-Dist: sphinx (>=7.0.1,<8.0.0)
+Requires-Dist: websockets (>=10.0,<11.0)
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # Python API client for SERP on-premise API
 
 ---
 
 This library is mirror of official SERP on-premise API in terms of methods and interfaces.
 
@@ -140,7 +144,8 @@
 
 ## Contributing
 
 1. Create your feature branch (`git checkout -b feature/fooBar`)
 2. Commit your changes (`git commit -am 'Add some fooBar'`)
 3. Push to the branch (`git push origin feature/fooBar`)
 4. Create a new Pull Request
+
```

