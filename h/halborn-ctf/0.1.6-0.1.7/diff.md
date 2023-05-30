# Comparing `tmp/halborn_ctf-0.1.6.tar.gz` & `tmp/halborn_ctf-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halborn_ctf-0.1.6.tar", last modified: Tue May 30 07:17:58 2023, max compression
+gzip compressed data, was "halborn_ctf-0.1.7.tar", last modified: Tue May 30 07:45:28 2023, max compression
```

## Comparing `halborn_ctf-0.1.6.tar` & `halborn_ctf-0.1.7.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 07:17:58.505475 halborn_ctf-0.1.6/
--rw-r--r--   0 fr0zn      (501) staff       (20)      594 2023-04-28 12:46:11.000000 halborn_ctf-0.1.6/.coveragerc
--rw-r--r--   0 fr0zn      (501) staff       (20)      566 2023-04-28 12:46:11.000000 halborn_ctf-0.1.6/.gitignore
--rw-r--r--   0 fr0zn      (501) staff       (20)      530 2023-04-28 12:46:11.000000 halborn_ctf-0.1.6/.readthedocs.yml
--rw-r--r--   0 fr0zn      (501) staff       (20)       86 2023-05-02 06:37:24.000000 halborn_ctf-0.1.6/AUTHORS.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)      128 2023-04-28 12:46:11.000000 halborn_ctf-0.1.6/CHANGELOG.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)    13866 2023-04-29 17:50:20.000000 halborn_ctf-0.1.6/CONTRIBUTING.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)     1081 2023-05-02 06:37:24.000000 halborn_ctf-0.1.6/LICENSE.txt
--rw-r--r--   0 fr0zn      (501) staff       (20)     2182 2023-05-30 07:17:58.505555 halborn_ctf-0.1.6/PKG-INFO
--rw-r--r--   0 fr0zn      (501) staff       (20)     1687 2023-05-02 13:57:33.000000 halborn_ctf-0.1.6/README.rst
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 07:17:58.500986 halborn_ctf-0.1.6/docs/
--rw-r--r--   0 fr0zn      (501) staff       (20)     1154 2023-04-28 12:46:11.000000 halborn_ctf-0.1.6/docs/Makefile
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 07:17:58.501208 halborn_ctf-0.1.6/docs/_static/
--rw-r--r--   0 fr0zn      (501) staff       (20)       18 2023-04-28 12:46:11.000000 halborn_ctf-0.1.6/docs/_static/.gitignore
--rw-r--r--   0 fr0zn      (501) staff       (20)       41 2023-04-28 12:46:11.000000 halborn_ctf-0.1.6/docs/authors.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)       43 2023-04-28 12:46:11.000000 halborn_ctf-0.1.6/docs/changelog.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)     9819 2023-05-03 09:08:19.000000 halborn_ctf-0.1.6/docs/conf.py
--rw-r--r--   0 fr0zn      (501) staff       (20)       33 2023-04-28 12:46:11.000000 halborn_ctf-0.1.6/docs/contributing.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)     1646 2023-05-03 08:57:14.000000 halborn_ctf-0.1.6/docs/index.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)       67 2023-04-28 12:46:11.000000 halborn_ctf-0.1.6/docs/license.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)      231 2023-05-02 07:06:55.000000 halborn_ctf-0.1.6/docs/requirements.txt
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 07:17:58.497338 halborn_ctf-0.1.6/docs/src/
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 07:17:58.501623 halborn_ctf-0.1.6/docs/src/getting_started/
--rw-r--r--   0 fr0zn      (501) staff       (20)     2292 2023-05-03 09:12:11.000000 halborn_ctf-0.1.6/docs/src/getting_started/examples.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)     1325 2023-05-02 14:03:18.000000 halborn_ctf-0.1.6/docs/src/getting_started/installation.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)     8582 2023-05-03 08:43:10.000000 halborn_ctf-0.1.6/docs/src/getting_started/quick_start.rst
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 07:17:58.501745 halborn_ctf-0.1.6/docs/src/user_guide/
--rw-r--r--   0 fr0zn      (501) staff       (20)     1706 2023-05-03 09:31:00.000000 halborn_ctf-0.1.6/docs/src/user_guide/faq.rst
--rw-r--r--   0 fr0zn      (501) staff       (20)      346 2023-04-28 12:46:11.000000 halborn_ctf-0.1.6/pyproject.toml
--rw-r--r--   0 fr0zn      (501) staff       (20)     1323 2023-05-30 07:17:58.505925 halborn_ctf-0.1.6/setup.cfg
--rw-r--r--   0 fr0zn      (501) staff       (20)      708 2023-04-28 12:46:11.000000 halborn_ctf-0.1.6/setup.py
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 07:17:58.497488 halborn_ctf-0.1.6/src/
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 07:17:58.502486 halborn_ctf-0.1.6/src/halborn_ctf/
--rw-r--r--   0 fr0zn      (501) staff       (20)      643 2023-04-30 11:37:15.000000 halborn_ctf-0.1.6/src/halborn_ctf/__init__.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     4492 2023-05-02 09:22:23.000000 halborn_ctf-0.1.6/src/halborn_ctf/cli.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     1338 2023-05-02 18:37:52.000000 halborn_ctf-0.1.6/src/halborn_ctf/functions.py
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 07:17:58.503754 halborn_ctf-0.1.6/src/halborn_ctf/network/
--rw-r--r--   0 fr0zn      (501) staff       (20)      131 2023-05-02 18:10:52.000000 halborn_ctf-0.1.6/src/halborn_ctf/network/__init__.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     1409 2023-05-02 18:10:43.000000 halborn_ctf-0.1.6/src/halborn_ctf/network/_generic.py
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 07:17:58.504281 halborn_ctf-0.1.6/src/halborn_ctf/network/filters/
--rw-r--r--   0 fr0zn      (501) staff       (20)     1918 2023-05-01 07:37:02.000000 halborn_ctf-0.1.6/src/halborn_ctf/network/filters/__init__.py
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 07:17:58.504741 halborn_ctf-0.1.6/src/halborn_ctf/network/filters/_json_rpc/
--rw-r--r--   0 fr0zn      (501) staff       (20)     1314 2023-05-02 17:51:03.000000 halborn_ctf-0.1.6/src/halborn_ctf/network/filters/_json_rpc/filter_json_rpc_method.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     1333 2023-05-02 17:51:12.000000 halborn_ctf-0.1.6/src/halborn_ctf/network/filters/_json_rpc/whitelist_json_rpc_method.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     1611 2023-05-01 07:37:55.000000 halborn_ctf-0.1.6/src/halborn_ctf/network/filters/_utils.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     2968 2023-05-01 07:15:21.000000 halborn_ctf-0.1.6/src/halborn_ctf/network/filters/json_rpc.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     4159 2023-04-30 06:56:04.000000 halborn_ctf-0.1.6/src/halborn_ctf/shell.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     3675 2023-05-03 08:37:30.000000 halborn_ctf-0.1.6/src/halborn_ctf/state.py
--rw-r--r--   0 fr0zn      (501) staff       (20)    22569 2023-05-30 07:16:13.000000 halborn_ctf-0.1.6/src/halborn_ctf/templates.py
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 07:17:58.503491 halborn_ctf-0.1.6/src/halborn_ctf.egg-info/
--rw-r--r--   0 fr0zn      (501) staff       (20)     2182 2023-05-30 07:17:58.000000 halborn_ctf-0.1.6/src/halborn_ctf.egg-info/PKG-INFO
--rw-r--r--   0 fr0zn      (501) staff       (20)     1274 2023-05-30 07:17:58.000000 halborn_ctf-0.1.6/src/halborn_ctf.egg-info/SOURCES.txt
--rw-r--r--   0 fr0zn      (501) staff       (20)        1 2023-05-30 07:17:58.000000 halborn_ctf-0.1.6/src/halborn_ctf.egg-info/dependency_links.txt
--rw-r--r--   0 fr0zn      (501) staff       (20)       52 2023-05-30 07:17:58.000000 halborn_ctf-0.1.6/src/halborn_ctf.egg-info/entry_points.txt
--rw-r--r--   0 fr0zn      (501) staff       (20)        1 2023-04-28 12:47:06.000000 halborn_ctf-0.1.6/src/halborn_ctf.egg-info/not-zip-safe
--rw-r--r--   0 fr0zn      (501) staff       (20)      160 2023-05-30 07:17:58.000000 halborn_ctf-0.1.6/src/halborn_ctf.egg-info/requires.txt
--rw-r--r--   0 fr0zn      (501) staff       (20)       12 2023-05-30 07:17:58.000000 halborn_ctf-0.1.6/src/halborn_ctf.egg-info/top_level.txt
-drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 07:17:58.505234 halborn_ctf-0.1.6/tests/
--rw-r--r--   0 fr0zn      (501) staff       (20)      279 2023-04-28 12:46:11.000000 halborn_ctf-0.1.6/tests/conftest.py
--rw-r--r--   0 fr0zn      (501) staff       (20)      592 2023-05-02 06:37:24.000000 halborn_ctf-0.1.6/tests/test_skeleton.py
--rw-r--r--   0 fr0zn      (501) staff       (20)     2851 2023-04-28 12:46:11.000000 halborn_ctf-0.1.6/tox.ini
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 07:45:28.639001 halborn_ctf-0.1.7/
+-rw-r--r--   0 fr0zn      (501) staff       (20)      594 2023-04-28 12:46:11.000000 halborn_ctf-0.1.7/.coveragerc
+-rw-r--r--   0 fr0zn      (501) staff       (20)      566 2023-04-28 12:46:11.000000 halborn_ctf-0.1.7/.gitignore
+-rw-r--r--   0 fr0zn      (501) staff       (20)      530 2023-04-28 12:46:11.000000 halborn_ctf-0.1.7/.readthedocs.yml
+-rw-r--r--   0 fr0zn      (501) staff       (20)       86 2023-05-02 06:37:24.000000 halborn_ctf-0.1.7/AUTHORS.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)      128 2023-04-28 12:46:11.000000 halborn_ctf-0.1.7/CHANGELOG.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)    13866 2023-04-29 17:50:20.000000 halborn_ctf-0.1.7/CONTRIBUTING.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1081 2023-05-02 06:37:24.000000 halborn_ctf-0.1.7/LICENSE.txt
+-rw-r--r--   0 fr0zn      (501) staff       (20)     2182 2023-05-30 07:45:28.639097 halborn_ctf-0.1.7/PKG-INFO
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1687 2023-05-02 13:57:33.000000 halborn_ctf-0.1.7/README.rst
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 07:45:28.632644 halborn_ctf-0.1.7/docs/
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1154 2023-04-28 12:46:11.000000 halborn_ctf-0.1.7/docs/Makefile
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 07:45:28.632871 halborn_ctf-0.1.7/docs/_static/
+-rw-r--r--   0 fr0zn      (501) staff       (20)       18 2023-04-28 12:46:11.000000 halborn_ctf-0.1.7/docs/_static/.gitignore
+-rw-r--r--   0 fr0zn      (501) staff       (20)       41 2023-04-28 12:46:11.000000 halborn_ctf-0.1.7/docs/authors.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)       43 2023-04-28 12:46:11.000000 halborn_ctf-0.1.7/docs/changelog.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)     9819 2023-05-03 09:08:19.000000 halborn_ctf-0.1.7/docs/conf.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)       33 2023-04-28 12:46:11.000000 halborn_ctf-0.1.7/docs/contributing.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1646 2023-05-03 08:57:14.000000 halborn_ctf-0.1.7/docs/index.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)       67 2023-04-28 12:46:11.000000 halborn_ctf-0.1.7/docs/license.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)      231 2023-05-02 07:06:55.000000 halborn_ctf-0.1.7/docs/requirements.txt
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 07:45:28.628545 halborn_ctf-0.1.7/docs/src/
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 07:45:28.633514 halborn_ctf-0.1.7/docs/src/getting_started/
+-rw-r--r--   0 fr0zn      (501) staff       (20)     2292 2023-05-03 09:12:11.000000 halborn_ctf-0.1.7/docs/src/getting_started/examples.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1325 2023-05-02 14:03:18.000000 halborn_ctf-0.1.7/docs/src/getting_started/installation.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)     8582 2023-05-03 08:43:10.000000 halborn_ctf-0.1.7/docs/src/getting_started/quick_start.rst
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 07:45:28.633747 halborn_ctf-0.1.7/docs/src/user_guide/
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1706 2023-05-03 09:31:00.000000 halborn_ctf-0.1.7/docs/src/user_guide/faq.rst
+-rw-r--r--   0 fr0zn      (501) staff       (20)      346 2023-04-28 12:46:11.000000 halborn_ctf-0.1.7/pyproject.toml
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1323 2023-05-30 07:45:28.639502 halborn_ctf-0.1.7/setup.cfg
+-rw-r--r--   0 fr0zn      (501) staff       (20)      708 2023-04-28 12:46:11.000000 halborn_ctf-0.1.7/setup.py
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 07:45:28.628683 halborn_ctf-0.1.7/src/
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 07:45:28.635121 halborn_ctf-0.1.7/src/halborn_ctf/
+-rw-r--r--   0 fr0zn      (501) staff       (20)      643 2023-04-30 11:37:15.000000 halborn_ctf-0.1.7/src/halborn_ctf/__init__.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     4492 2023-05-02 09:22:23.000000 halborn_ctf-0.1.7/src/halborn_ctf/cli.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1338 2023-05-02 18:37:52.000000 halborn_ctf-0.1.7/src/halborn_ctf/functions.py
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 07:45:28.636799 halborn_ctf-0.1.7/src/halborn_ctf/network/
+-rw-r--r--   0 fr0zn      (501) staff       (20)      131 2023-05-02 18:10:52.000000 halborn_ctf-0.1.7/src/halborn_ctf/network/__init__.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1409 2023-05-02 18:10:43.000000 halborn_ctf-0.1.7/src/halborn_ctf/network/_generic.py
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 07:45:28.637696 halborn_ctf-0.1.7/src/halborn_ctf/network/filters/
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1918 2023-05-01 07:37:02.000000 halborn_ctf-0.1.7/src/halborn_ctf/network/filters/__init__.py
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 07:45:28.638170 halborn_ctf-0.1.7/src/halborn_ctf/network/filters/_json_rpc/
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1314 2023-05-02 17:51:03.000000 halborn_ctf-0.1.7/src/halborn_ctf/network/filters/_json_rpc/filter_json_rpc_method.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1333 2023-05-02 17:51:12.000000 halborn_ctf-0.1.7/src/halborn_ctf/network/filters/_json_rpc/whitelist_json_rpc_method.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1611 2023-05-01 07:37:55.000000 halborn_ctf-0.1.7/src/halborn_ctf/network/filters/_utils.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     2968 2023-05-01 07:15:21.000000 halborn_ctf-0.1.7/src/halborn_ctf/network/filters/json_rpc.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     4159 2023-04-30 06:56:04.000000 halborn_ctf-0.1.7/src/halborn_ctf/shell.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     3675 2023-05-03 08:37:30.000000 halborn_ctf-0.1.7/src/halborn_ctf/state.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)    22572 2023-05-30 07:45:07.000000 halborn_ctf-0.1.7/src/halborn_ctf/templates.py
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 07:45:28.636410 halborn_ctf-0.1.7/src/halborn_ctf.egg-info/
+-rw-r--r--   0 fr0zn      (501) staff       (20)     2182 2023-05-30 07:45:28.000000 halborn_ctf-0.1.7/src/halborn_ctf.egg-info/PKG-INFO
+-rw-r--r--   0 fr0zn      (501) staff       (20)     1274 2023-05-30 07:45:28.000000 halborn_ctf-0.1.7/src/halborn_ctf.egg-info/SOURCES.txt
+-rw-r--r--   0 fr0zn      (501) staff       (20)        1 2023-05-30 07:45:28.000000 halborn_ctf-0.1.7/src/halborn_ctf.egg-info/dependency_links.txt
+-rw-r--r--   0 fr0zn      (501) staff       (20)       52 2023-05-30 07:45:28.000000 halborn_ctf-0.1.7/src/halborn_ctf.egg-info/entry_points.txt
+-rw-r--r--   0 fr0zn      (501) staff       (20)        1 2023-04-28 12:47:06.000000 halborn_ctf-0.1.7/src/halborn_ctf.egg-info/not-zip-safe
+-rw-r--r--   0 fr0zn      (501) staff       (20)      160 2023-05-30 07:45:28.000000 halborn_ctf-0.1.7/src/halborn_ctf.egg-info/requires.txt
+-rw-r--r--   0 fr0zn      (501) staff       (20)       12 2023-05-30 07:45:28.000000 halborn_ctf-0.1.7/src/halborn_ctf.egg-info/top_level.txt
+drwxr-xr-x   0 fr0zn      (501) staff       (20)        0 2023-05-30 07:45:28.638802 halborn_ctf-0.1.7/tests/
+-rw-r--r--   0 fr0zn      (501) staff       (20)      279 2023-04-28 12:46:11.000000 halborn_ctf-0.1.7/tests/conftest.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)      592 2023-05-02 06:37:24.000000 halborn_ctf-0.1.7/tests/test_skeleton.py
+-rw-r--r--   0 fr0zn      (501) staff       (20)     2851 2023-04-28 12:46:11.000000 halborn_ctf-0.1.7/tox.ini
```

### Comparing `halborn_ctf-0.1.6/.coveragerc` & `halborn_ctf-0.1.7/.coveragerc`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.6/.gitignore` & `halborn_ctf-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.6/.readthedocs.yml` & `halborn_ctf-0.1.7/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.6/CONTRIBUTING.rst` & `halborn_ctf-0.1.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.6/LICENSE.txt` & `halborn_ctf-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.6/PKG-INFO` & `halborn_ctf-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halborn_ctf
-Version: 0.1.6
+Version: 0.1.7
 Summary: Add a short description here!
 Home-page: https://github.com/HalbornAcademy/halborn_ctf
 Author: ferran.celades
 Author-email: ferran.celades@halborn.com
 License: MIT
 Project-URL: Documentation, https://halborn-ctf.readthedocs.io/
 Platform: any
```

### Comparing `halborn_ctf-0.1.6/README.rst` & `halborn_ctf-0.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.6/docs/Makefile` & `halborn_ctf-0.1.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.6/docs/conf.py` & `halborn_ctf-0.1.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.6/docs/index.rst` & `halborn_ctf-0.1.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.6/docs/src/getting_started/examples.rst` & `halborn_ctf-0.1.7/docs/src/getting_started/examples.rst`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.6/docs/src/getting_started/installation.rst` & `halborn_ctf-0.1.7/docs/src/getting_started/installation.rst`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.6/docs/src/getting_started/quick_start.rst` & `halborn_ctf-0.1.7/docs/src/getting_started/quick_start.rst`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.6/docs/src/user_guide/faq.rst` & `halborn_ctf-0.1.7/docs/src/user_guide/faq.rst`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.6/setup.cfg` & `halborn_ctf-0.1.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.6/setup.py` & `halborn_ctf-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.6/src/halborn_ctf/__init__.py` & `halborn_ctf-0.1.7/src/halborn_ctf/__init__.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.6/src/halborn_ctf/cli.py` & `halborn_ctf-0.1.7/src/halborn_ctf/cli.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.6/src/halborn_ctf/functions.py` & `halborn_ctf-0.1.7/src/halborn_ctf/functions.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.6/src/halborn_ctf/network/_generic.py` & `halborn_ctf-0.1.7/src/halborn_ctf/network/_generic.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.6/src/halborn_ctf/network/filters/__init__.py` & `halborn_ctf-0.1.7/src/halborn_ctf/network/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.6/src/halborn_ctf/network/filters/_json_rpc/filter_json_rpc_method.py` & `halborn_ctf-0.1.7/src/halborn_ctf/network/filters/_json_rpc/filter_json_rpc_method.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.6/src/halborn_ctf/network/filters/_json_rpc/whitelist_json_rpc_method.py` & `halborn_ctf-0.1.7/src/halborn_ctf/network/filters/_json_rpc/whitelist_json_rpc_method.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.6/src/halborn_ctf/network/filters/_utils.py` & `halborn_ctf-0.1.7/src/halborn_ctf/network/filters/_utils.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.6/src/halborn_ctf/network/filters/json_rpc.py` & `halborn_ctf-0.1.7/src/halborn_ctf/network/filters/json_rpc.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.6/src/halborn_ctf/shell.py` & `halborn_ctf-0.1.7/src/halborn_ctf/shell.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.6/src/halborn_ctf/state.py` & `halborn_ctf-0.1.7/src/halborn_ctf/state.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.6/src/halborn_ctf/templates.py` & `halborn_ctf-0.1.7/src/halborn_ctf/templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -521,16 +521,16 @@
             except Exception as e:
                 self.log.exception(e)
 
         response = {
             'solved': self.solved
         }
 
-        if self.solved_msg:
-            response['msg'] = self.solved_msg
+        if self._solved_msg:
+            response['msg'] = self._solved_msg
         else:
             response['msg'] = 'Solved' if self.solved else 'Not solved'
 
         if self.solved and self.FLAG_TYPE == FlagType.DYNAMIC:
             response['flag'] = os.environ.get('FLAG', 'HAL{PLACEHOLDER}')
 
         return response
@@ -683,8 +683,8 @@
         """
         pass
 
     @abstractmethod
     def solver(self):
         """Refer to :obj:`HAS_SOLVER`
         """
-        pass
+        pass
```

### Comparing `halborn_ctf-0.1.6/src/halborn_ctf.egg-info/PKG-INFO` & `halborn_ctf-0.1.7/src/halborn_ctf.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halborn-ctf
-Version: 0.1.6
+Version: 0.1.7
 Summary: Add a short description here!
 Home-page: https://github.com/HalbornAcademy/halborn_ctf
 Author: ferran.celades
 Author-email: ferran.celades@halborn.com
 License: MIT
 Project-URL: Documentation, https://halborn-ctf.readthedocs.io/
 Platform: any
```

### Comparing `halborn_ctf-0.1.6/src/halborn_ctf.egg-info/SOURCES.txt` & `halborn_ctf-0.1.7/src/halborn_ctf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.6/tests/test_skeleton.py` & `halborn_ctf-0.1.7/tests/test_skeleton.py`

 * *Files identical despite different names*

### Comparing `halborn_ctf-0.1.6/tox.ini` & `halborn_ctf-0.1.7/tox.ini`

 * *Files identical despite different names*

