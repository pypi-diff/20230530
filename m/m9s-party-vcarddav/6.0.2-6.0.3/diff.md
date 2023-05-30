# Comparing `tmp/m9s_party_vcarddav-6.0.2.tar.gz` & `tmp/m9s_party_vcarddav-6.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m9s_party_vcarddav-6.0.2.tar", last modified: Sun Apr 10 11:31:55 2022, max compression
+gzip compressed data, was "m9s_party_vcarddav-6.0.3.tar", last modified: Tue May 30 16:26:56 2023, max compression
```

## Comparing `m9s_party_vcarddav-6.0.2.tar` & `m9s_party_vcarddav-6.0.3.tar`

### file list

```diff
@@ -1,63 +1,67 @@
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-04-10 11:31:55.275443 m9s_party_vcarddav-6.0.2/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       84 2022-01-26 10:04:07.000000 m9s_party_vcarddav-6.0.2/.coveragerc
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-01-26 10:04:07.000000 m9s_party_vcarddav-6.0.2/.drone.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2022-01-26 10:04:07.000000 m9s_party_vcarddav-6.0.2/.flake8
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1787 2022-01-26 10:04:07.000000 m9s_party_vcarddav-6.0.2/.gitlab-ci.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2022-01-26 10:04:07.000000 m9s_party_vcarddav-6.0.2/.isort.cfg
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1089 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.2/CHANGELOG
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      805 2022-01-28 16:16:15.000000 m9s_party_vcarddav-6.0.2/COPYRIGHT
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2020-03-19 21:27:16.000000 m9s_party_vcarddav-6.0.2/INSTALL
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2020-03-19 21:27:16.000000 m9s_party_vcarddav-6.0.2/LICENSE
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      125 2022-01-26 10:04:07.000000 m9s_party_vcarddav-6.0.2/MANIFEST.in
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3352 2022-04-10 11:31:55.275443 m9s_party_vcarddav-6.0.2/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      588 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.2/README
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1245 2020-03-19 21:27:16.000000 m9s_party_vcarddav-6.0.2/README.md
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      615 2020-03-28 19:35:38.000000 m9s_party_vcarddav-6.0.2/README.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      494 2021-12-11 18:43:04.000000 m9s_party_vcarddav-6.0.2/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1877 2022-02-02 11:19:55.000000 m9s_party_vcarddav-6.0.2/carddav.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       77 2022-03-05 15:33:25.000000 m9s_party_vcarddav-6.0.2/dev_requirements.txt
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-04-10 11:31:55.275443 m9s_party_vcarddav-6.0.2/doc/
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-04-10 11:31:55.275443 m9s_party_vcarddav-6.0.2/doc/de/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       43 2020-03-19 21:27:16.000000 m9s_party_vcarddav-6.0.2/doc/de/index.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      615 2020-03-28 19:35:38.000000 m9s_party_vcarddav-6.0.2/doc/index.rst
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-04-10 11:31:55.271443 m9s_party_vcarddav-6.0.2/locale/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      504 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.2/locale/bg_BG.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      502 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.2/locale/ca_ES.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      424 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.2/locale/cs_CZ.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      380 2021-02-28 00:11:00.000000 m9s_party_vcarddav-6.0.2/locale/de.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      506 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.2/locale/es_AR.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      504 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.2/locale/es_CO.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      504 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.2/locale/es_EC.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      505 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.2/locale/es_ES.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      507 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.2/locale/es_MX.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      500 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.2/locale/fr_FR.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      505 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.2/locale/hu_HU.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      424 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.2/locale/it_IT.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      424 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.2/locale/ja_JP.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      424 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.2/locale/lo_LA.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      424 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.2/locale/lt_LT.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      424 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.2/locale/nl_NL.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      501 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.2/locale/pt_BR.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      590 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.2/locale/ru_RU.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      508 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.2/locale/sl_SI.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      424 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.2/locale/zh_CN.po
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-04-10 11:31:55.275443 m9s_party_vcarddav-6.0.2/m9s_party_vcarddav.egg-info/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3352 2022-04-10 11:31:55.000000 m9s_party_vcarddav-6.0.2/m9s_party_vcarddav.egg-info/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1436 2022-04-10 11:31:55.000000 m9s_party_vcarddav-6.0.2/m9s_party_vcarddav.egg-info/SOURCES.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2022-04-10 11:31:55.000000 m9s_party_vcarddav-6.0.2/m9s_party_vcarddav.egg-info/dependency_links.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       79 2022-04-10 11:31:55.000000 m9s_party_vcarddav-6.0.2/m9s_party_vcarddav.egg-info/entry_points.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2020-03-28 19:43:29.000000 m9s_party_vcarddav-6.0.2/m9s_party_vcarddav.egg-info/not-zip-safe
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2022-04-10 11:31:55.000000 m9s_party_vcarddav-6.0.2/m9s_party_vcarddav.egg-info/requires.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2022-04-10 11:31:55.000000 m9s_party_vcarddav-6.0.2/m9s_party_vcarddav.egg-info/top_level.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    13671 2022-03-17 22:34:11.000000 m9s_party_vcarddav-6.0.2/party.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      741 2020-03-28 19:51:46.000000 m9s_party_vcarddav-6.0.2/party.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2022-01-26 10:04:07.000000 m9s_party_vcarddav-6.0.2/requirements.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       38 2022-04-10 11:31:55.275443 m9s_party_vcarddav-6.0.2/setup.cfg
--rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4710 2022-02-02 11:18:18.000000 m9s_party_vcarddav-6.0.2/setup.py
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-04-10 11:31:55.275443 m9s_party_vcarddav-6.0.2/tests/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      283 2020-03-19 21:27:16.000000 m9s_party_vcarddav-6.0.2/tests/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1072 2021-12-16 10:01:07.000000 m9s_party_vcarddav-6.0.2/tests/t.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1088 2021-12-11 18:43:04.000000 m9s_party_vcarddav-6.0.2/tests/test_party_vcarddav.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      745 2022-01-26 10:04:07.000000 m9s_party_vcarddav-6.0.2/tox.ini
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       87 2022-03-17 22:36:47.000000 m9s_party_vcarddav-6.0.2/tryton.cfg
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    13947 2022-04-10 11:31:48.000000 m9s_party_vcarddav-6.0.2/webdav.py
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:26:56.862656 m9s_party_vcarddav-6.0.3/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       84 2022-01-26 10:04:07.000000 m9s_party_vcarddav-6.0.3/.coveragerc
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-01-26 10:04:07.000000 m9s_party_vcarddav-6.0.3/.drone.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2022-01-26 10:04:07.000000 m9s_party_vcarddav-6.0.3/.flake8
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1787 2022-11-13 14:32:56.000000 m9s_party_vcarddav-6.0.3/.gitlab-ci.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2022-01-26 10:04:07.000000 m9s_party_vcarddav-6.0.3/.isort.cfg
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:26:56.862656 m9s_party_vcarddav-6.0.3/.woodpecker/
+-rwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2022-11-23 17:28:52.000000 m9s_party_vcarddav-6.0.3/.woodpecker/mail_curl.sh
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2022-11-23 20:42:33.000000 m9s_party_vcarddav-6.0.3/.woodpecker/report.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1468 2022-11-24 15:51:07.000000 m9s_party_vcarddav-6.0.3/.woodpecker/test.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1089 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.3/CHANGELOG
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      805 2022-01-28 16:16:15.000000 m9s_party_vcarddav-6.0.3/COPYRIGHT
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2020-03-19 21:27:16.000000 m9s_party_vcarddav-6.0.3/INSTALL
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2020-03-19 21:27:16.000000 m9s_party_vcarddav-6.0.3/LICENSE
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      125 2022-01-26 10:04:07.000000 m9s_party_vcarddav-6.0.3/MANIFEST.in
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3332 2023-05-30 16:26:56.862656 m9s_party_vcarddav-6.0.3/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      588 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.3/README
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1245 2020-03-19 21:27:16.000000 m9s_party_vcarddav-6.0.3/README.md
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      615 2020-03-28 19:35:38.000000 m9s_party_vcarddav-6.0.3/README.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      494 2021-12-11 18:43:04.000000 m9s_party_vcarddav-6.0.3/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1877 2022-02-02 11:19:55.000000 m9s_party_vcarddav-6.0.3/carddav.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       77 2022-03-05 15:33:25.000000 m9s_party_vcarddav-6.0.3/dev_requirements.txt
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:26:56.862656 m9s_party_vcarddav-6.0.3/doc/
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:26:56.862656 m9s_party_vcarddav-6.0.3/doc/de/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       43 2020-03-19 21:27:16.000000 m9s_party_vcarddav-6.0.3/doc/de/index.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      615 2020-03-28 19:35:38.000000 m9s_party_vcarddav-6.0.3/doc/index.rst
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:26:56.858657 m9s_party_vcarddav-6.0.3/locale/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      504 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.3/locale/bg_BG.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      502 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.3/locale/ca_ES.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      424 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.3/locale/cs_CZ.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      380 2021-02-28 00:11:00.000000 m9s_party_vcarddav-6.0.3/locale/de.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      506 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.3/locale/es_AR.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      504 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.3/locale/es_CO.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      504 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.3/locale/es_EC.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      505 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.3/locale/es_ES.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      507 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.3/locale/es_MX.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      500 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.3/locale/fr_FR.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      505 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.3/locale/hu_HU.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      424 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.3/locale/it_IT.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      424 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.3/locale/ja_JP.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      424 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.3/locale/lo_LA.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      424 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.3/locale/lt_LT.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      424 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.3/locale/nl_NL.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      501 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.3/locale/pt_BR.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      590 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.3/locale/ru_RU.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      508 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.3/locale/sl_SI.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      424 2018-03-07 14:37:46.000000 m9s_party_vcarddav-6.0.3/locale/zh_CN.po
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:26:56.862656 m9s_party_vcarddav-6.0.3/m9s_party_vcarddav.egg-info/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3332 2023-05-30 16:26:56.000000 m9s_party_vcarddav-6.0.3/m9s_party_vcarddav.egg-info/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1505 2023-05-30 16:26:56.000000 m9s_party_vcarddav-6.0.3/m9s_party_vcarddav.egg-info/SOURCES.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2023-05-30 16:26:56.000000 m9s_party_vcarddav-6.0.3/m9s_party_vcarddav.egg-info/dependency_links.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       66 2023-05-30 16:26:56.000000 m9s_party_vcarddav-6.0.3/m9s_party_vcarddav.egg-info/entry_points.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2020-03-28 19:43:29.000000 m9s_party_vcarddav-6.0.3/m9s_party_vcarddav.egg-info/not-zip-safe
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2023-05-30 16:26:56.000000 m9s_party_vcarddav-6.0.3/m9s_party_vcarddav.egg-info/requires.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2023-05-30 16:26:56.000000 m9s_party_vcarddav-6.0.3/m9s_party_vcarddav.egg-info/top_level.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    13671 2022-03-17 22:34:11.000000 m9s_party_vcarddav-6.0.3/party.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      741 2020-03-28 19:51:46.000000 m9s_party_vcarddav-6.0.3/party.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2022-01-26 10:04:07.000000 m9s_party_vcarddav-6.0.3/requirements.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       38 2023-05-30 16:26:56.862656 m9s_party_vcarddav-6.0.3/setup.cfg
+-rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4710 2022-02-02 11:18:18.000000 m9s_party_vcarddav-6.0.3/setup.py
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:26:56.862656 m9s_party_vcarddav-6.0.3/tests/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      283 2020-03-19 21:27:16.000000 m9s_party_vcarddav-6.0.3/tests/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1072 2021-12-16 10:01:07.000000 m9s_party_vcarddav-6.0.3/tests/t.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1088 2021-12-11 18:43:04.000000 m9s_party_vcarddav-6.0.3/tests/test_party_vcarddav.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      843 2022-11-24 16:26:27.000000 m9s_party_vcarddav-6.0.3/tox.ini
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       87 2022-04-10 11:32:01.000000 m9s_party_vcarddav-6.0.3/tryton.cfg
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    14111 2023-05-30 16:18:46.000000 m9s_party_vcarddav-6.0.3/webdav.py
```

### Comparing `m9s_party_vcarddav-6.0.2/.drone.yml` & `m9s_party_vcarddav-6.0.3/.drone.yml`

 * *Files identical despite different names*

### Comparing `m9s_party_vcarddav-6.0.2/.gitlab-ci.yml` & `m9s_party_vcarddav-6.0.3/.gitlab-ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 stages:
   - test
   - pages
 
 .test_base: &test_base
   stage: test
-  image: python:latest
+  image: python:3.10
 
   # Pip's cache doesn't store the python packages
   # https://pip.pypa.io/en/stable/reference/pip_install/#caching
   #
   # If you want to also cache the installed packages, you have to install
   # them in a virtualenv and cache it as well.
   cache:
@@ -41,23 +41,23 @@
     POSTGRES_USER: test
     POSTGRES_PASSWORD: test
     DB_NAME: test
   services:
     - postgres
   script:
     - pip install psycopg2-binary tox flake8
-    - tox -e py39-postgresql
+    - tox -e py310-postgresql
   tags:
     - postgres
 
 test-sqlite:
   <<: *test_base
   script:
     - pip install tox flake8 coverage coverage-badge
-    - tox -e py39-sqlite
+    - tox -e py310-sqlite
     - coverage html
     - coverage report -m
     - coverage-badge
 
   coverage: '/TOTAL.+ ([0-9]{1,3}%)/'
       
   artifacts:
```

### Comparing `m9s_party_vcarddav-6.0.2/CHANGELOG` & `m9s_party_vcarddav-6.0.3/CHANGELOG`

 * *Files identical despite different names*

### Comparing `m9s_party_vcarddav-6.0.2/COPYRIGHT` & `m9s_party_vcarddav-6.0.3/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `m9s_party_vcarddav-6.0.2/INSTALL` & `m9s_party_vcarddav-6.0.3/INSTALL`

 * *Files identical despite different names*

### Comparing `m9s_party_vcarddav-6.0.2/LICENSE` & `m9s_party_vcarddav-6.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `m9s_party_vcarddav-6.0.2/PKG-INFO` & `m9s_party_vcarddav-6.0.3/m9s_party_vcarddav.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
-Name: m9s_party_vcarddav
-Version: 6.0.2
+Name: m9s-party-vcarddav
+Version: 6.0.3
 Summary: Tryton Party Vcarddav Module
 Home-page: http://www.m9s.biz/
+Download-URL: https://gitlab.com/m9s/party_vcarddav.git
 Author: MBSolutions
 Author-email: info@m9s.biz
 License: GPL-3
-Download-URL: https://gitlab.com/m9s/party_vcarddav.git
 Project-URL: Bug Tracker, https://support.m9s.biz/
 Project-URL: Source Code, https://gitlab.com/m9s/party_vcarddav.git
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -99,9 +98,7 @@
 See LICENSE
 
 Copyright
 ---------
 
 See COPYRIGHT
 
-
-
```

### Comparing `m9s_party_vcarddav-6.0.2/README` & `m9s_party_vcarddav-6.0.3/README`

 * *Files identical despite different names*

### Comparing `m9s_party_vcarddav-6.0.2/README.md` & `m9s_party_vcarddav-6.0.3/README.md`

 * *Files identical despite different names*

### Comparing `m9s_party_vcarddav-6.0.2/README.rst` & `m9s_party_vcarddav-6.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `m9s_party_vcarddav-6.0.2/carddav.py` & `m9s_party_vcarddav-6.0.3/carddav.py`

 * *Files identical despite different names*

### Comparing `m9s_party_vcarddav-6.0.2/doc/index.rst` & `m9s_party_vcarddav-6.0.3/doc/index.rst`

 * *Files identical despite different names*

### Comparing `m9s_party_vcarddav-6.0.2/locale/ru_RU.po` & `m9s_party_vcarddav-6.0.3/locale/ru_RU.po`

 * *Files identical despite different names*

### Comparing `m9s_party_vcarddav-6.0.2/m9s_party_vcarddav.egg-info/PKG-INFO` & `m9s_party_vcarddav-6.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
-Name: m9s-party-vcarddav
-Version: 6.0.2
+Name: m9s_party_vcarddav
+Version: 6.0.3
 Summary: Tryton Party Vcarddav Module
 Home-page: http://www.m9s.biz/
+Download-URL: https://gitlab.com/m9s/party_vcarddav.git
 Author: MBSolutions
 Author-email: info@m9s.biz
 License: GPL-3
-Download-URL: https://gitlab.com/m9s/party_vcarddav.git
 Project-URL: Bug Tracker, https://support.m9s.biz/
 Project-URL: Source Code, https://gitlab.com/m9s/party_vcarddav.git
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Intended Audience :: Legal Industry
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -99,9 +98,7 @@
 See LICENSE
 
 Copyright
 ---------
 
 See COPYRIGHT
 
-
-
```

### Comparing `m9s_party_vcarddav-6.0.2/m9s_party_vcarddav.egg-info/SOURCES.txt` & `m9s_party_vcarddav-6.0.3/m9s_party_vcarddav.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,17 @@
 ./locale/pt_BR.po
 ./locale/ru_RU.po
 ./locale/sl_SI.po
 ./locale/zh_CN.po
 ./tests/__init__.py
 ./tests/t.py
 ./tests/test_party_vcarddav.py
+.woodpecker/mail_curl.sh
+.woodpecker/report.yml
+.woodpecker/test.yml
 doc/index.rst
 doc/de/index.rst
 locale/bg_BG.po
 locale/ca_ES.po
 locale/cs_CZ.po
 locale/de.po
 locale/es_AR.po
```

### Comparing `m9s_party_vcarddav-6.0.2/party.py` & `m9s_party_vcarddav-6.0.3/party.py`

 * *Files identical despite different names*

### Comparing `m9s_party_vcarddav-6.0.2/party.xml` & `m9s_party_vcarddav-6.0.3/party.xml`

 * *Files identical despite different names*

### Comparing `m9s_party_vcarddav-6.0.2/setup.py` & `m9s_party_vcarddav-6.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `m9s_party_vcarddav-6.0.2/tests/t.py` & `m9s_party_vcarddav-6.0.3/tests/t.py`

 * *Files identical despite different names*

### Comparing `m9s_party_vcarddav-6.0.2/tests/test_party_vcarddav.py` & `m9s_party_vcarddav-6.0.3/tests/test_party_vcarddav.py`

 * *Files identical despite different names*

### Comparing `m9s_party_vcarddav-6.0.2/webdav.py` & `m9s_party_vcarddav-6.0.3/webdav.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,18 +192,19 @@
             for sub_ids in grouped_slice(ids):
                 red_sql = reduce_ids(party.id, sub_ids)
                 cursor.execute(*party.select(party.id,
                         Extract('EPOCH', party.create_date),
                         where=red_sql))
                 for party_id2, date in cursor.fetchall():
                     if party_id2 == party_id:
-                        res = date
+                        # Python 3.11 returns Decimal, pywebdav needs float
+                        res = float(date)
                     if cache is not None:
                         cache['_contact'].setdefault(party_id2, {})
-                        cache['_contact'][party_id2]['creationdate'] = date
+                        cache['_contact'][party_id2]['creationdate'] = res
             if res is not None:
                 return res
         return super(Collection, cls).get_creationdate(uri, cache=cache)
 
     @classmethod
     def get_lastmodified(cls, uri, cache=None):
         pool = Pool()
@@ -244,18 +245,19 @@
                                     contact_mechanism.create_date))),
                         where=red_sql,
                         group_by=party.id))
                 for party_id2, date_p, date_a, date_c in cursor.fetchall():
                     dates = list(filter(None, [date_p, date_a, date_c]))
                     date = max(dates)
                     if party_id2 == party_id:
-                        res = date
+                        # Python 3.11 returns Decimal, pywebdav needs float
+                        res = float(date)
                     if cache is not None:
                         cache['_contact'].setdefault(party_id2, {})
-                        cache['_contact'][party_id2]['lastmodified'] = date
+                        cache['_contact'][party_id2]['lastmodified'] = res
             if res is not None:
                 return res
         return super(Collection, cls).get_lastmodified(uri, cache=cache)
 
     @classmethod
     def get_data(cls, uri, cache=None):
         Vcard = Pool().get('party_vcarddav.party.vcard', type='report')
```

