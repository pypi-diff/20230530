# Comparing `tmp/hyperthought-transfer-0.2.tar.gz` & `tmp/hyperthought-transfer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Jason\Documents\repos\hyperthought-transfer\dist\tmpe8cs9m8h\hyperthought-transfer-0.2.tar", last modified: Wed May 24 16:49:59 2023, max compression
+gzip compressed data, was "C:\Users\Jason\Documents\repos\hyperthought-transfer\dist\tmpr_sjnx35\hyperthought-transfer-0.2.1.tar", last modified: Tue May 30 11:51:34 2023, max compression
```

## Comparing `hyperthought-transfer-0.2.tar` & `hyperthought-transfer-0.2.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 16:49:59.000000 hyperthought-transfer-0.2/
--rw-rw-rw-   0        0        0      632 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2/.coveragerc
--rw-rw-rw-   0        0        0      661 2023-01-03 12:02:08.000000 hyperthought-transfer-0.2/.gitignore
--rw-rw-rw-   0        0        0      514 2023-01-03 12:02:08.000000 hyperthought-transfer-0.2/.readthedocs.yml
--rw-rw-rw-   0        0        0       84 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2/AUTHORS.rst
--rw-rw-rw-   0        0        0      141 2022-05-17 15:55:48.000000 hyperthought-transfer-0.2/CHANGELOG.rst
--rw-rw-rw-   0        0        0    14388 2022-12-27 15:26:41.000000 hyperthought-transfer-0.2/CONTRIBUTING.rst
-drwxrwxrwx   0        0        0        0 2023-05-24 16:49:59.000000 hyperthought-transfer-0.2/docs/
--rw-rw-rw-   0        0        0       43 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2/docs/authors.rst
--rw-rw-rw-   0        0        0       45 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2/docs/changelog.rst
--rw-rw-rw-   0        0        0    10090 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2/docs/conf.py
--rw-rw-rw-   0        0        0       34 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2/docs/contributing.rst
--rw-rw-rw-   0        0        0     2430 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2/docs/index.rst
--rw-rw-rw-   0        0        0       74 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2/docs/license.rst
--rw-rw-rw-   0        0        0     1183 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2/docs/Makefile
--rw-rw-rw-   0        0        0       41 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2/docs/readme.rst
--rw-rw-rw-   0        0        0      238 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-05-24 16:49:59.000000 hyperthought-transfer-0.2/docs/_static/
--rw-rw-rw-   0        0        0       19 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2/docs/_static/.gitignore
--rw-rw-rw-   0        0        0     1100 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      150 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2764 2023-05-24 16:49:59.000000 hyperthought-transfer-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2198 2022-05-17 15:55:48.000000 hyperthought-transfer-0.2/README.rst
--rw-rw-rw-   0        0        0     1335 2023-05-24 16:49:59.000000 hyperthought-transfer-0.2/setup.cfg
--rw-rw-rw-   0        0        0     1023 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 16:49:59.000000 hyperthought-transfer-0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-24 16:49:59.000000 hyperthought-transfer-0.2/src/hyperthought_transfer/
-drwxrwxrwx   0        0        0        0 2023-05-24 16:49:59.000000 hyperthought-transfer-0.2/src/hyperthought_transfer/antivirus/
--rw-rw-rw-   0        0        0     2513 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2/src/hyperthought_transfer/antivirus/base.py
--rw-rw-rw-   0        0        0     2928 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2/src/hyperthought_transfer/antivirus/_mcafee.py
--rw-rw-rw-   0        0        0     2992 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2/src/hyperthought_transfer/antivirus/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 16:49:59.000000 hyperthought-transfer-0.2/src/hyperthought_transfer/filebinner/
--rw-rw-rw-   0        0        0      798 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2/src/hyperthought_transfer/filebinner/data.py
-drwxrwxrwx   0        0        0        0 2023-05-24 16:49:59.000000 hyperthought-transfer-0.2/src/hyperthought_transfer/filebinner/database/
--rw-rw-rw-   0        0        0     1224 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2/src/hyperthought_transfer/filebinner/database/connect.py
-drwxrwxrwx   0        0        0        0 2023-05-24 16:49:59.000000 hyperthought-transfer-0.2/src/hyperthought_transfer/filebinner/database/template/
--rw-rw-rw-   0        0        0     1419 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2/src/hyperthought_transfer/filebinner/database/template/create.py
--rw-rw-rw-   0        0        0    40960 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2/src/hyperthought_transfer/filebinner/database/template/template.db
--rw-rw-rw-   0        0        0        0 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2/src/hyperthought_transfer/filebinner/database/template/__init__.py
--rw-rw-rw-   0        0        0     4130 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2/src/hyperthought_transfer/filebinner/database/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 16:49:59.000000 hyperthought-transfer-0.2/src/hyperthought_transfer/filebinner/process/
--rw-rw-rw-   0        0        0     6642 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2/src/hyperthought_transfer/filebinner/process/filebinner.py
--rw-rw-rw-   0        0        0       40 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2/src/hyperthought_transfer/filebinner/process/__init__.py
--rw-rw-rw-   0        0        0       47 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2/src/hyperthought_transfer/filebinner/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 16:49:59.000000 hyperthought-transfer-0.2/src/hyperthought_transfer/manifest/
-drwxrwxrwx   0        0        0        0 2023-05-24 16:49:59.000000 hyperthought-transfer-0.2/src/hyperthought_transfer/manifest/database/
--rw-rw-rw-   0        0        0     3216 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2/src/hyperthought_transfer/manifest/database/connect.py
-drwxrwxrwx   0        0        0        0 2023-05-24 16:49:59.000000 hyperthought-transfer-0.2/src/hyperthought_transfer/manifest/database/template/
--rw-rw-rw-   0        0        0     1596 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2/src/hyperthought_transfer/manifest/database/template/create.py
--rw-rw-rw-   0        0        0   147456 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2/src/hyperthought_transfer/manifest/database/template/template.db
--rw-rw-rw-   0        0        0       36 2023-02-01 16:27:41.000000 hyperthought-transfer-0.2/src/hyperthought_transfer/manifest/database/template/__init__.py
--rw-rw-rw-   0        0        0    71738 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2/src/hyperthought_transfer/manifest/database/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 16:49:59.000000 hyperthought-transfer-0.2/src/hyperthought_transfer/manifest/processes/
--rw-rw-rw-   0        0        0     6857 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2/src/hyperthought_transfer/manifest/processes/rules.py
--rw-rw-rw-   0        0        0        0 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2/src/hyperthought_transfer/manifest/processes/__init__.py
--rw-rw-rw-   0        0        0     2046 2023-01-03 12:02:08.000000 hyperthought-transfer-0.2/src/hyperthought_transfer/manifest/utils.py
--rw-rw-rw-   0        0        0    48947 2023-05-24 16:48:51.000000 hyperthought-transfer-0.2/src/hyperthought_transfer/manifest/__init__.py
--rw-rw-rw-   0        0        0      713 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2/src/hyperthought_transfer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 16:49:59.000000 hyperthought-transfer-0.2/src/hyperthought_transfer.egg-info/
--rw-rw-rw-   0        0        0        1 2023-05-24 16:49:59.000000 hyperthought-transfer-0.2/src/hyperthought_transfer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-05-16 11:27:09.000000 hyperthought-transfer-0.2/src/hyperthought_transfer.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     2764 2023-05-24 16:49:59.000000 hyperthought-transfer-0.2/src/hyperthought_transfer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       86 2023-05-24 16:49:59.000000 hyperthought-transfer-0.2/src/hyperthought_transfer.egg-info/requires.txt
--rw-rw-rw-   0        0        0     1840 2023-05-24 16:49:59.000000 hyperthought-transfer-0.2/src/hyperthought_transfer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       22 2023-05-24 16:49:59.000000 hyperthought-transfer-0.2/src/hyperthought_transfer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-24 16:49:59.000000 hyperthought-transfer-0.2/tests/
--rw-rw-rw-   0        0        0      299 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2/tests/conftest.py
--rw-rw-rw-   0        0        0     2659 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2/tox.ini
+drwxrwxrwx   0        0        0        0 2023-05-30 11:51:34.000000 hyperthought-transfer-0.2.1/
+-rw-rw-rw-   0        0        0      632 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.1/.coveragerc
+-rw-rw-rw-   0        0        0      661 2023-01-03 12:02:08.000000 hyperthought-transfer-0.2.1/.gitignore
+-rw-rw-rw-   0        0        0      514 2023-01-03 12:02:08.000000 hyperthought-transfer-0.2.1/.readthedocs.yml
+-rw-rw-rw-   0        0        0       84 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.1/AUTHORS.rst
+-rw-rw-rw-   0        0        0      141 2022-05-17 15:55:48.000000 hyperthought-transfer-0.2.1/CHANGELOG.rst
+-rw-rw-rw-   0        0        0    14388 2022-12-27 15:26:41.000000 hyperthought-transfer-0.2.1/CONTRIBUTING.rst
+drwxrwxrwx   0        0        0        0 2023-05-30 11:51:34.000000 hyperthought-transfer-0.2.1/docs/
+-rw-rw-rw-   0        0        0       43 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.1/docs/authors.rst
+-rw-rw-rw-   0        0        0       45 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.1/docs/changelog.rst
+-rw-rw-rw-   0        0        0    10090 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.1/docs/conf.py
+-rw-rw-rw-   0        0        0       34 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.1/docs/contributing.rst
+-rw-rw-rw-   0        0        0     2430 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.1/docs/index.rst
+-rw-rw-rw-   0        0        0       74 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.1/docs/license.rst
+-rw-rw-rw-   0        0        0     1183 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.1/docs/Makefile
+-rw-rw-rw-   0        0        0       41 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.1/docs/readme.rst
+-rw-rw-rw-   0        0        0      238 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.1/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 11:51:34.000000 hyperthought-transfer-0.2.1/docs/_static/
+-rw-rw-rw-   0        0        0       19 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.1/docs/_static/.gitignore
+-rw-rw-rw-   0        0        0     1100 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      150 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2766 2023-05-30 11:51:34.000000 hyperthought-transfer-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2198 2022-05-17 15:55:48.000000 hyperthought-transfer-0.2.1/README.rst
+-rw-rw-rw-   0        0        0     1335 2023-05-30 11:51:34.000000 hyperthought-transfer-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1025 2023-05-30 11:51:16.000000 hyperthought-transfer-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 11:51:34.000000 hyperthought-transfer-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-30 11:51:34.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer/
+drwxrwxrwx   0        0        0        0 2023-05-30 11:51:34.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer/antivirus/
+-rw-rw-rw-   0        0        0     2513 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer/antivirus/base.py
+-rw-rw-rw-   0        0        0     2928 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer/antivirus/_mcafee.py
+-rw-rw-rw-   0        0        0     2992 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer/antivirus/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 11:51:34.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer/filebinner/
+-rw-rw-rw-   0        0        0      798 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer/filebinner/data.py
+drwxrwxrwx   0        0        0        0 2023-05-30 11:51:34.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer/filebinner/database/
+-rw-rw-rw-   0        0        0     1224 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer/filebinner/database/connect.py
+drwxrwxrwx   0        0        0        0 2023-05-30 11:51:34.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer/filebinner/database/template/
+-rw-rw-rw-   0        0        0     1419 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer/filebinner/database/template/create.py
+-rw-rw-rw-   0        0        0    40960 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer/filebinner/database/template/template.db
+-rw-rw-rw-   0        0        0        0 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer/filebinner/database/template/__init__.py
+-rw-rw-rw-   0        0        0     4130 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer/filebinner/database/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 11:51:34.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer/filebinner/process/
+-rw-rw-rw-   0        0        0     6642 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer/filebinner/process/filebinner.py
+-rw-rw-rw-   0        0        0       40 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer/filebinner/process/__init__.py
+-rw-rw-rw-   0        0        0       47 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer/filebinner/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 11:51:34.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer/manifest/
+drwxrwxrwx   0        0        0        0 2023-05-30 11:51:34.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer/manifest/database/
+-rw-rw-rw-   0        0        0     3216 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer/manifest/database/connect.py
+drwxrwxrwx   0        0        0        0 2023-05-30 11:51:34.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer/manifest/database/template/
+-rw-rw-rw-   0        0        0     1596 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer/manifest/database/template/create.py
+-rw-rw-rw-   0        0        0   147456 2023-05-30 11:50:42.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer/manifest/database/template/template.db
+-rw-rw-rw-   0        0        0       36 2023-02-01 16:27:41.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer/manifest/database/template/__init__.py
+-rw-rw-rw-   0        0        0    71738 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer/manifest/database/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 11:51:34.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer/manifest/processes/
+-rw-rw-rw-   0        0        0     6857 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer/manifest/processes/rules.py
+-rw-rw-rw-   0        0        0        0 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer/manifest/processes/__init__.py
+-rw-rw-rw-   0        0        0     2046 2023-01-03 12:02:08.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer/manifest/utils.py
+-rw-rw-rw-   0        0        0    48947 2023-05-24 16:48:51.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer/manifest/__init__.py
+-rw-rw-rw-   0        0        0      713 2023-05-23 13:02:41.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 11:51:34.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-05-30 11:51:34.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-05-16 11:27:09.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     2766 2023-05-30 11:51:34.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2023-05-30 11:51:34.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     1840 2023-05-30 11:51:34.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       22 2023-05-30 11:51:34.000000 hyperthought-transfer-0.2.1/src/hyperthought_transfer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 11:51:34.000000 hyperthought-transfer-0.2.1/tests/
+-rw-rw-rw-   0        0        0      299 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.1/tests/conftest.py
+-rw-rw-rw-   0        0        0     2659 2022-04-26 15:06:17.000000 hyperthought-transfer-0.2.1/tox.ini
```

### Comparing `hyperthought-transfer-0.2/.coveragerc` & `hyperthought-transfer-0.2.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2/.gitignore` & `hyperthought-transfer-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2/.readthedocs.yml` & `hyperthought-transfer-0.2.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2/CONTRIBUTING.rst` & `hyperthought-transfer-0.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2/docs/conf.py` & `hyperthought-transfer-0.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2/docs/index.rst` & `hyperthought-transfer-0.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2/docs/Makefile` & `hyperthought-transfer-0.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2/LICENSE.txt` & `hyperthought-transfer-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2/PKG-INFO` & `hyperthought-transfer-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperthought-transfer
-Version: 0.2
+Version: 0.2.1
 Summary: Package used to upload files to and download files from the HyperThought® content management system.
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Jason Thiese
 Author-email: jthiese@ues.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `hyperthought-transfer-0.2/README.rst` & `hyperthought-transfer-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2/setup.cfg` & `hyperthought-transfer-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2/setup.py` & `hyperthought-transfer-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 from setuptools import setup, find_packages
 
 
 if __name__ == "__main__":
     try:
         setup(
-            version="0.2",
+            version="0.2.1",
             use_scm_version={
                 "version_scheme": "no-guess-dev",
                 "local-scheme": "no-local-version",
             },
             packages=find_packages(where="src"),
             package_dir={"": "src"},
             include_package_data=True,
```

### Comparing `hyperthought-transfer-0.2/src/hyperthought_transfer/antivirus/base.py` & `hyperthought-transfer-0.2.1/src/hyperthought_transfer/antivirus/base.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2/src/hyperthought_transfer/antivirus/_mcafee.py` & `hyperthought-transfer-0.2.1/src/hyperthought_transfer/antivirus/_mcafee.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2/src/hyperthought_transfer/antivirus/__init__.py` & `hyperthought-transfer-0.2.1/src/hyperthought_transfer/antivirus/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2/src/hyperthought_transfer/filebinner/data.py` & `hyperthought-transfer-0.2.1/src/hyperthought_transfer/filebinner/data.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2/src/hyperthought_transfer/filebinner/database/connect.py` & `hyperthought-transfer-0.2.1/src/hyperthought_transfer/filebinner/database/connect.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2/src/hyperthought_transfer/filebinner/database/template/create.py` & `hyperthought-transfer-0.2.1/src/hyperthought_transfer/filebinner/database/template/create.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2/src/hyperthought_transfer/filebinner/database/template/template.db` & `hyperthought-transfer-0.2.1/src/hyperthought_transfer/filebinner/database/template/template.db`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2/src/hyperthought_transfer/filebinner/database/__init__.py` & `hyperthought-transfer-0.2.1/src/hyperthought_transfer/filebinner/database/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2/src/hyperthought_transfer/filebinner/process/filebinner.py` & `hyperthought-transfer-0.2.1/src/hyperthought_transfer/filebinner/process/filebinner.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2/src/hyperthought_transfer/manifest/database/connect.py` & `hyperthought-transfer-0.2.1/src/hyperthought_transfer/manifest/database/connect.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2/src/hyperthought_transfer/manifest/database/template/create.py` & `hyperthought-transfer-0.2.1/src/hyperthought_transfer/manifest/database/template/create.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2/src/hyperthought_transfer/manifest/database/template/template.db` & `hyperthought-transfer-0.2.1/src/hyperthought_transfer/manifest/database/template/template.db`

 * *Files 5% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -22,24 +22,25 @@
 INSERT INTO FileStatus VALUES(6,'Created');
 INSERT INTO FileStatus VALUES(7,'Not Ready');
 INSERT INTO FileStatus VALUES(8,'Hash Mismatch');
 INSERT INTO FileStatus VALUES(9,'Malware Detected');
 INSERT INTO FileStatus VALUES(10,'Upload Error');
 INSERT INTO FileStatus VALUES(11,'Creation Error');
 INSERT INTO FileStatus VALUES(12,'Unknown Error');
+INSERT INTO FileStatus VALUES(13,'Metadata Update Error');
 CREATE TABLE File (
     id                      INTEGER PRIMARY KEY AUTOINCREMENT,
     file_status_id          INTEGER NOT NULL DEFAULT 1,
     name                    TEXT NOT NULL,
     -- path will generally only be null for folders that don't exist locally.
     path                    TEXT UNIQUE,
     hyperthought_id         TEXT NOT NULL,
     -- hyperthought_id_path corresponds to content.path in MarkLogic
     -- documents.  It is a comma-delimited path that includes all parent
-    -- folder hypertthought ids, e.g. ",uuid,uuid,uuid,"
+    -- folder hyperthought ids, e.g. ",uuid,uuid,uuid,"
     hyperthought_id_path    TEXT NOT NULL,
     is_folder               BOOLEAN NOT NULL,
     end_bytes               TEXT,
     size                    INTEGER,
     file_hash               TEXT,
     -- The backend key is the identifier per the backend, e.g. an s3 key.
     backend_key             TEXT,
@@ -110,15 +111,15 @@
     rule_id                     INTEGER NOT NULL,
     parser_id                   INTEGER NOT NULL,
     FOREIGN KEY (rule_id) REFERENCES Rule(id) ON DELETE CASCADE,
     FOREIGN KEY (parser_id) REFERENCES Parser(id) ON DELETE CASCADE,
     CONSTRAINT rule_id__parser_id UNIQUE (rule_id, parser_id)
 );
 DELETE FROM sqlite_sequence;
-INSERT INTO sqlite_sequence VALUES('FileStatus',12);
+INSERT INTO sqlite_sequence VALUES('FileStatus',13);
 INSERT INTO sqlite_sequence VALUES('ParserStatus',3);
 INSERT INTO sqlite_sequence VALUES('TargetRule',5);
 CREATE INDEX idx__File__file_status_id ON File (file_status_id);
 CREATE INDEX idx__File__path ON File (path);
 CREATE INDEX idx__File__is_folder ON File (is_folder);
 CREATE INDEX idx__Metadata__file_id ON Metadata (file_id);
 CREATE INDEX idx__MetadataApplication__metadata_id
```

### Comparing `hyperthought-transfer-0.2/src/hyperthought_transfer/manifest/database/__init__.py` & `hyperthought-transfer-0.2.1/src/hyperthought_transfer/manifest/database/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2/src/hyperthought_transfer/manifest/processes/rules.py` & `hyperthought-transfer-0.2.1/src/hyperthought_transfer/manifest/processes/rules.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2/src/hyperthought_transfer/manifest/utils.py` & `hyperthought-transfer-0.2.1/src/hyperthought_transfer/manifest/utils.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2/src/hyperthought_transfer/manifest/__init__.py` & `hyperthought-transfer-0.2.1/src/hyperthought_transfer/manifest/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2/src/hyperthought_transfer/__init__.py` & `hyperthought-transfer-0.2.1/src/hyperthought_transfer/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2/src/hyperthought_transfer.egg-info/PKG-INFO` & `hyperthought-transfer-0.2.1/src/hyperthought_transfer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperthought-transfer
-Version: 0.2
+Version: 0.2.1
 Summary: Package used to upload files to and download files from the HyperThought® content management system.
 Home-page: https://github.com/pyscaffold/pyscaffold/
 Author: Jason Thiese
 Author-email: jthiese@ues.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `hyperthought-transfer-0.2/src/hyperthought_transfer.egg-info/SOURCES.txt` & `hyperthought-transfer-0.2.1/src/hyperthought_transfer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyperthought-transfer-0.2/tox.ini` & `hyperthought-transfer-0.2.1/tox.ini`

 * *Files identical despite different names*

