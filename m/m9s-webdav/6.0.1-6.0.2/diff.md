# Comparing `tmp/m9s_webdav-6.0.1.tar.gz` & `tmp/m9s_webdav-6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m9s_webdav-6.0.1.tar", last modified: Sun Apr 10 11:31:11 2022, max compression
+gzip compressed data, was "m9s_webdav-6.0.2.tar", last modified: Tue May 30 16:24:40 2023, max compression
```

## Comparing `m9s_webdav-6.0.1.tar` & `m9s_webdav-6.0.2.tar`

### file list

```diff
@@ -1,73 +1,77 @@
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-04-10 11:31:11.567749 m9s_webdav-6.0.1/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       76 2022-01-26 10:04:20.000000 m9s_webdav-6.0.1/.coveragerc
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-01-26 10:04:20.000000 m9s_webdav-6.0.1/.drone.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2022-01-26 10:04:20.000000 m9s_webdav-6.0.1/.flake8
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1787 2022-01-26 10:04:20.000000 m9s_webdav-6.0.1/.gitlab-ci.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2022-01-26 10:04:20.000000 m9s_webdav-6.0.1/.isort.cfg
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      263 2018-03-07 14:37:46.000000 m9s_webdav-6.0.1/CHANGELOG
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      764 2022-01-28 16:16:16.000000 m9s_webdav-6.0.1/COPYRIGHT
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2020-03-19 21:27:37.000000 m9s_webdav-6.0.1/INSTALL
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2020-03-19 21:27:37.000000 m9s_webdav-6.0.1/LICENSE
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      125 2022-01-26 10:04:20.000000 m9s_webdav-6.0.1/MANIFEST.in
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3264 2022-04-10 11:31:11.567749 m9s_webdav-6.0.1/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      545 2018-03-07 14:37:46.000000 m9s_webdav-6.0.1/README
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1189 2020-03-19 21:27:37.000000 m9s_webdav-6.0.1/README.md
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      509 2020-03-28 17:27:47.000000 m9s_webdav-6.0.1/README.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      401 2022-04-10 11:30:46.000000 m9s_webdav-6.0.1/__init__.py
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-04-10 11:31:11.567749 m9s_webdav-6.0.1/bin/
--rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     1832 2021-12-11 18:43:12.000000 m9s_webdav-6.0.1/bin/trytond-webdav
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       77 2022-03-05 15:41:55.000000 m9s_webdav-6.0.1/dev_requirements.txt
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-04-10 11:31:11.567749 m9s_webdav-6.0.1/doc/
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-04-10 11:31:11.567749 m9s_webdav-6.0.1/doc/de/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       27 2020-03-19 21:27:37.000000 m9s_webdav-6.0.1/doc/de/index.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      509 2020-03-28 17:27:47.000000 m9s_webdav-6.0.1/doc/index.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      225 2022-04-10 11:30:46.000000 m9s_webdav-6.0.1/exceptions.py
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-04-10 11:31:11.563749 m9s_webdav-6.0.1/locale/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4110 2018-03-07 14:37:46.000000 m9s_webdav-6.0.1/locale/bg_BG.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4094 2018-03-07 14:37:46.000000 m9s_webdav-6.0.1/locale/ca_ES.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3345 2018-03-07 14:37:46.000000 m9s_webdav-6.0.1/locale/cs_CZ.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3211 2022-03-10 16:55:05.000000 m9s_webdav-6.0.1/locale/de.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4156 2018-03-07 14:37:46.000000 m9s_webdav-6.0.1/locale/es_AR.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4171 2018-03-07 14:37:46.000000 m9s_webdav-6.0.1/locale/es_CO.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4163 2018-03-07 14:37:46.000000 m9s_webdav-6.0.1/locale/es_EC.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4154 2018-03-07 14:37:46.000000 m9s_webdav-6.0.1/locale/es_ES.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4199 2018-03-07 14:37:46.000000 m9s_webdav-6.0.1/locale/es_MX.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4089 2018-03-07 14:37:46.000000 m9s_webdav-6.0.1/locale/fr_FR.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3345 2018-03-07 14:37:46.000000 m9s_webdav-6.0.1/locale/hu_HU.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3345 2018-03-07 14:37:46.000000 m9s_webdav-6.0.1/locale/it_IT.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3345 2018-03-07 14:37:46.000000 m9s_webdav-6.0.1/locale/ja_JP.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3345 2018-03-07 14:37:46.000000 m9s_webdav-6.0.1/locale/lo_LA.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3345 2018-03-07 14:37:46.000000 m9s_webdav-6.0.1/locale/lt_LT.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3725 2018-03-07 14:37:46.000000 m9s_webdav-6.0.1/locale/nl_NL.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4069 2018-03-07 14:37:46.000000 m9s_webdav-6.0.1/locale/pt_BR.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4658 2018-03-07 14:37:46.000000 m9s_webdav-6.0.1/locale/ru_RU.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3909 2018-03-07 14:37:46.000000 m9s_webdav-6.0.1/locale/sl_SI.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3832 2018-03-07 14:37:46.000000 m9s_webdav-6.0.1/locale/zh_CN.po
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-04-10 11:31:11.567749 m9s_webdav-6.0.1/m9s_webdav.egg-info/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3264 2022-04-10 11:31:11.000000 m9s_webdav-6.0.1/m9s_webdav.egg-info/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1724 2022-04-10 11:31:11.000000 m9s_webdav-6.0.1/m9s_webdav.egg-info/SOURCES.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2022-04-10 11:31:11.000000 m9s_webdav-6.0.1/m9s_webdav.egg-info/dependency_links.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       63 2022-04-10 11:31:11.000000 m9s_webdav-6.0.1/m9s_webdav.egg-info/entry_points.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2020-03-28 18:41:07.000000 m9s_webdav-6.0.1/m9s_webdav.egg-info/not-zip-safe
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2022-04-10 11:31:11.000000 m9s_webdav-6.0.1/m9s_webdav.egg-info/requires.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2022-04-10 11:31:11.000000 m9s_webdav-6.0.1/m9s_webdav.egg-info/top_level.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      705 2022-02-02 11:10:02.000000 m9s_webdav-6.0.1/message.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    21828 2022-04-10 11:30:46.000000 m9s_webdav-6.0.1/protocol.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2022-01-26 10:04:20.000000 m9s_webdav-6.0.1/requirements.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3588 2022-04-10 11:30:46.000000 m9s_webdav-6.0.1/server.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       38 2022-04-10 11:31:11.567749 m9s_webdav-6.0.1/setup.cfg
--rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4580 2022-02-02 11:09:18.000000 m9s_webdav-6.0.1/setup.py
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-04-10 11:31:11.563749 m9s_webdav-6.0.1/tests/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      259 2020-03-19 21:27:37.000000 m9s_webdav-6.0.1/tests/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      479 2021-12-11 18:43:12.000000 m9s_webdav-6.0.1/tests/test_webdav.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      745 2022-01-26 10:04:20.000000 m9s_webdav-6.0.1/tox.ini
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       83 2022-02-02 11:12:28.000000 m9s_webdav-6.0.1/tryton.cfg
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-04-10 11:31:11.567749 m9s_webdav-6.0.1/view/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      505 2020-03-28 19:01:42.000000 m9s_webdav-6.0.1/view/attachment_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      405 2020-03-28 19:01:42.000000 m9s_webdav-6.0.1/view/collection_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      207 2020-03-28 19:01:42.000000 m9s_webdav-6.0.1/view/collection_list.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      299 2020-03-28 19:01:42.000000 m9s_webdav-6.0.1/view/collection_tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      634 2020-03-28 19:01:42.000000 m9s_webdav-6.0.1/view/share_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      242 2020-03-28 19:01:42.000000 m9s_webdav-6.0.1/view/share_list.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    32552 2022-04-10 11:30:46.000000 m9s_webdav-6.0.1/webdav.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     6738 2020-03-28 19:01:53.000000 m9s_webdav-6.0.1/webdav.xml
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:24:40.507490 m9s_webdav-6.0.2/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       76 2022-01-26 10:04:20.000000 m9s_webdav-6.0.2/.coveragerc
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-01-26 10:04:20.000000 m9s_webdav-6.0.2/.drone.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2022-01-26 10:04:20.000000 m9s_webdav-6.0.2/.flake8
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1787 2022-11-13 14:32:56.000000 m9s_webdav-6.0.2/.gitlab-ci.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2022-01-26 10:04:20.000000 m9s_webdav-6.0.2/.isort.cfg
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:24:40.507490 m9s_webdav-6.0.2/.woodpecker/
+-rwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2022-11-23 17:28:52.000000 m9s_webdav-6.0.2/.woodpecker/mail_curl.sh
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2022-11-23 20:42:33.000000 m9s_webdav-6.0.2/.woodpecker/report.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1468 2022-11-24 15:51:07.000000 m9s_webdav-6.0.2/.woodpecker/test.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      263 2018-03-07 14:37:46.000000 m9s_webdav-6.0.2/CHANGELOG
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      764 2022-01-28 16:16:16.000000 m9s_webdav-6.0.2/COPYRIGHT
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2020-03-19 21:27:37.000000 m9s_webdav-6.0.2/INSTALL
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2020-03-19 21:27:37.000000 m9s_webdav-6.0.2/LICENSE
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      125 2022-01-26 10:04:20.000000 m9s_webdav-6.0.2/MANIFEST.in
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3244 2023-05-30 16:24:40.507490 m9s_webdav-6.0.2/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      545 2018-03-07 14:37:46.000000 m9s_webdav-6.0.2/README
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1189 2020-03-19 21:27:37.000000 m9s_webdav-6.0.2/README.md
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      509 2020-03-28 17:27:47.000000 m9s_webdav-6.0.2/README.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      401 2022-04-10 11:30:46.000000 m9s_webdav-6.0.2/__init__.py
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:24:40.507490 m9s_webdav-6.0.2/bin/
+-rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     1832 2021-12-11 18:43:12.000000 m9s_webdav-6.0.2/bin/trytond-webdav
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       77 2022-03-05 15:41:55.000000 m9s_webdav-6.0.2/dev_requirements.txt
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:24:40.507490 m9s_webdav-6.0.2/doc/
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:24:40.507490 m9s_webdav-6.0.2/doc/de/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       27 2020-03-19 21:27:37.000000 m9s_webdav-6.0.2/doc/de/index.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      509 2020-03-28 17:27:47.000000 m9s_webdav-6.0.2/doc/index.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      225 2022-04-10 11:30:46.000000 m9s_webdav-6.0.2/exceptions.py
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:24:40.503491 m9s_webdav-6.0.2/locale/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4110 2018-03-07 14:37:46.000000 m9s_webdav-6.0.2/locale/bg_BG.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4094 2018-03-07 14:37:46.000000 m9s_webdav-6.0.2/locale/ca_ES.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3345 2018-03-07 14:37:46.000000 m9s_webdav-6.0.2/locale/cs_CZ.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3211 2022-03-10 16:55:05.000000 m9s_webdav-6.0.2/locale/de.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4156 2018-03-07 14:37:46.000000 m9s_webdav-6.0.2/locale/es_AR.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4171 2018-03-07 14:37:46.000000 m9s_webdav-6.0.2/locale/es_CO.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4163 2018-03-07 14:37:46.000000 m9s_webdav-6.0.2/locale/es_EC.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4154 2018-03-07 14:37:46.000000 m9s_webdav-6.0.2/locale/es_ES.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4199 2018-03-07 14:37:46.000000 m9s_webdav-6.0.2/locale/es_MX.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4089 2018-03-07 14:37:46.000000 m9s_webdav-6.0.2/locale/fr_FR.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3345 2018-03-07 14:37:46.000000 m9s_webdav-6.0.2/locale/hu_HU.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3345 2018-03-07 14:37:46.000000 m9s_webdav-6.0.2/locale/it_IT.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3345 2018-03-07 14:37:46.000000 m9s_webdav-6.0.2/locale/ja_JP.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3345 2018-03-07 14:37:46.000000 m9s_webdav-6.0.2/locale/lo_LA.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3345 2018-03-07 14:37:46.000000 m9s_webdav-6.0.2/locale/lt_LT.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3725 2018-03-07 14:37:46.000000 m9s_webdav-6.0.2/locale/nl_NL.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4069 2018-03-07 14:37:46.000000 m9s_webdav-6.0.2/locale/pt_BR.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4658 2018-03-07 14:37:46.000000 m9s_webdav-6.0.2/locale/ru_RU.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3909 2018-03-07 14:37:46.000000 m9s_webdav-6.0.2/locale/sl_SI.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3832 2018-03-07 14:37:46.000000 m9s_webdav-6.0.2/locale/zh_CN.po
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:24:40.507490 m9s_webdav-6.0.2/m9s_webdav.egg-info/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3244 2023-05-30 16:24:40.000000 m9s_webdav-6.0.2/m9s_webdav.egg-info/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1793 2023-05-30 16:24:40.000000 m9s_webdav-6.0.2/m9s_webdav.egg-info/SOURCES.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2023-05-30 16:24:40.000000 m9s_webdav-6.0.2/m9s_webdav.egg-info/dependency_links.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       50 2023-05-30 16:24:40.000000 m9s_webdav-6.0.2/m9s_webdav.egg-info/entry_points.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2020-03-28 18:41:07.000000 m9s_webdav-6.0.2/m9s_webdav.egg-info/not-zip-safe
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2023-05-30 16:24:40.000000 m9s_webdav-6.0.2/m9s_webdav.egg-info/requires.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2023-05-30 16:24:40.000000 m9s_webdav-6.0.2/m9s_webdav.egg-info/top_level.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      705 2022-02-02 11:10:02.000000 m9s_webdav-6.0.2/message.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    21846 2023-05-30 16:18:50.000000 m9s_webdav-6.0.2/protocol.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2022-01-26 10:04:20.000000 m9s_webdav-6.0.2/requirements.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3367 2023-05-30 16:18:50.000000 m9s_webdav-6.0.2/server.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       38 2023-05-30 16:24:40.507490 m9s_webdav-6.0.2/setup.cfg
+-rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4580 2022-02-02 11:09:18.000000 m9s_webdav-6.0.2/setup.py
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:24:40.503491 m9s_webdav-6.0.2/tests/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      259 2020-03-19 21:27:37.000000 m9s_webdav-6.0.2/tests/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      479 2021-12-11 18:43:12.000000 m9s_webdav-6.0.2/tests/test_webdav.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      843 2022-11-24 16:26:27.000000 m9s_webdav-6.0.2/tox.ini
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       83 2022-04-10 11:31:18.000000 m9s_webdav-6.0.2/tryton.cfg
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:24:40.503491 m9s_webdav-6.0.2/view/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      505 2020-03-28 19:01:42.000000 m9s_webdav-6.0.2/view/attachment_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      405 2020-03-28 19:01:42.000000 m9s_webdav-6.0.2/view/collection_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      207 2020-03-28 19:01:42.000000 m9s_webdav-6.0.2/view/collection_list.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      299 2020-03-28 19:01:42.000000 m9s_webdav-6.0.2/view/collection_tree.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      634 2020-03-28 19:01:42.000000 m9s_webdav-6.0.2/view/share_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      242 2020-03-28 19:01:42.000000 m9s_webdav-6.0.2/view/share_list.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    32724 2023-05-30 16:18:50.000000 m9s_webdav-6.0.2/webdav.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     6738 2020-03-28 19:01:53.000000 m9s_webdav-6.0.2/webdav.xml
```

### Comparing `m9s_webdav-6.0.1/.drone.yml` & `m9s_webdav-6.0.2/.drone.yml`

 * *Files identical despite different names*

### Comparing `m9s_webdav-6.0.1/.gitlab-ci.yml` & `m9s_webdav-6.0.2/.gitlab-ci.yml`

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

### Comparing `m9s_webdav-6.0.1/COPYRIGHT` & `m9s_webdav-6.0.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `m9s_webdav-6.0.1/INSTALL` & `m9s_webdav-6.0.2/INSTALL`

 * *Files identical despite different names*

### Comparing `m9s_webdav-6.0.1/LICENSE` & `m9s_webdav-6.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `m9s_webdav-6.0.1/PKG-INFO` & `m9s_webdav-6.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: m9s_webdav
-Version: 6.0.1
+Version: 6.0.2
 Summary: Tryton Webdav Module
 Home-page: http://www.m9s.biz/
+Download-URL: https://gitlab.com/m9s/webdav.git
 Author: MBSolutions
 Author-email: info@m9s.biz
 License: GPL-3
-Download-URL: https://gitlab.com/m9s/webdav.git
 Project-URL: Bug Tracker, https://support.m9s.biz/
 Project-URL: Source Code, https://gitlab.com/m9s/webdav.git
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

### Comparing `m9s_webdav-6.0.1/README` & `m9s_webdav-6.0.2/README`

 * *Files identical despite different names*

### Comparing `m9s_webdav-6.0.1/README.md` & `m9s_webdav-6.0.2/README.md`

 * *Files identical despite different names*

### Comparing `m9s_webdav-6.0.1/bin/trytond-webdav` & `m9s_webdav-6.0.2/bin/trytond-webdav`

 * *Files identical despite different names*

### Comparing `m9s_webdav-6.0.1/locale/bg_BG.po` & `m9s_webdav-6.0.2/locale/bg_BG.po`

 * *Files identical despite different names*

### Comparing `m9s_webdav-6.0.1/locale/ca_ES.po` & `m9s_webdav-6.0.2/locale/ca_ES.po`

 * *Files identical despite different names*

### Comparing `m9s_webdav-6.0.1/locale/cs_CZ.po` & `m9s_webdav-6.0.2/locale/cs_CZ.po`

 * *Files identical despite different names*

### Comparing `m9s_webdav-6.0.1/locale/de.po` & `m9s_webdav-6.0.2/locale/de.po`

 * *Files identical despite different names*

### Comparing `m9s_webdav-6.0.1/locale/es_AR.po` & `m9s_webdav-6.0.2/locale/es_AR.po`

 * *Files identical despite different names*

### Comparing `m9s_webdav-6.0.1/locale/es_CO.po` & `m9s_webdav-6.0.2/locale/es_CO.po`

 * *Files identical despite different names*

### Comparing `m9s_webdav-6.0.1/locale/es_EC.po` & `m9s_webdav-6.0.2/locale/es_EC.po`

 * *Files identical despite different names*

### Comparing `m9s_webdav-6.0.1/locale/es_ES.po` & `m9s_webdav-6.0.2/locale/es_ES.po`

 * *Files identical despite different names*

### Comparing `m9s_webdav-6.0.1/locale/es_MX.po` & `m9s_webdav-6.0.2/locale/es_MX.po`

 * *Files identical despite different names*

### Comparing `m9s_webdav-6.0.1/locale/fr_FR.po` & `m9s_webdav-6.0.2/locale/fr_FR.po`

 * *Files identical despite different names*

### Comparing `m9s_webdav-6.0.1/locale/hu_HU.po` & `m9s_webdav-6.0.2/locale/hu_HU.po`

 * *Files identical despite different names*

### Comparing `m9s_webdav-6.0.1/locale/it_IT.po` & `m9s_webdav-6.0.2/locale/it_IT.po`

 * *Files identical despite different names*

### Comparing `m9s_webdav-6.0.1/locale/ja_JP.po` & `m9s_webdav-6.0.2/locale/ja_JP.po`

 * *Files identical despite different names*

### Comparing `m9s_webdav-6.0.1/locale/lo_LA.po` & `m9s_webdav-6.0.2/locale/lo_LA.po`

 * *Files identical despite different names*

### Comparing `m9s_webdav-6.0.1/locale/lt_LT.po` & `m9s_webdav-6.0.2/locale/lt_LT.po`

 * *Files identical despite different names*

### Comparing `m9s_webdav-6.0.1/locale/nl_NL.po` & `m9s_webdav-6.0.2/locale/nl_NL.po`

 * *Files identical despite different names*

### Comparing `m9s_webdav-6.0.1/locale/pt_BR.po` & `m9s_webdav-6.0.2/locale/pt_BR.po`

 * *Files identical despite different names*

### Comparing `m9s_webdav-6.0.1/locale/ru_RU.po` & `m9s_webdav-6.0.2/locale/ru_RU.po`

 * *Files identical despite different names*

### Comparing `m9s_webdav-6.0.1/locale/sl_SI.po` & `m9s_webdav-6.0.2/locale/sl_SI.po`

 * *Files identical despite different names*

### Comparing `m9s_webdav-6.0.1/locale/zh_CN.po` & `m9s_webdav-6.0.2/locale/zh_CN.po`

 * *Files identical despite different names*

### Comparing `m9s_webdav-6.0.1/m9s_webdav.egg-info/PKG-INFO` & `m9s_webdav-6.0.2/m9s_webdav.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: m9s-webdav
-Version: 6.0.1
+Version: 6.0.2
 Summary: Tryton Webdav Module
 Home-page: http://www.m9s.biz/
+Download-URL: https://gitlab.com/m9s/webdav.git
 Author: MBSolutions
 Author-email: info@m9s.biz
 License: GPL-3
-Download-URL: https://gitlab.com/m9s/webdav.git
 Project-URL: Bug Tracker, https://support.m9s.biz/
 Project-URL: Source Code, https://gitlab.com/m9s/webdav.git
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

### Comparing `m9s_webdav-6.0.1/m9s_webdav.egg-info/SOURCES.txt` & `m9s_webdav-6.0.2/m9s_webdav.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -55,14 +55,17 @@
 ./tests/test_webdav.py
 ./view/attachment_form.xml
 ./view/collection_form.xml
 ./view/collection_list.xml
 ./view/collection_tree.xml
 ./view/share_form.xml
 ./view/share_list.xml
+.woodpecker/mail_curl.sh
+.woodpecker/report.yml
+.woodpecker/test.yml
 bin/trytond-webdav
 doc/index.rst
 doc/de/index.rst
 locale/bg_BG.po
 locale/ca_ES.po
 locale/cs_CZ.po
 locale/de.po
```

### Comparing `m9s_webdav-6.0.1/message.xml` & `m9s_webdav-6.0.2/message.xml`

 * *Files identical despite different names*

### Comparing `m9s_webdav-6.0.1/protocol.py` & `m9s_webdav-6.0.2/protocol.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
             for child in Collection.get_childs(dburi, filter=filter,
                     cache=LOCAL.cache):
 
                 path_child = path + child
                 res.append(urllib.parse.urlunparse((scheme, netloc,
                             path_child, params, query,
                             fragment)))
-        except KeyError:
+        except (AttributeError, KeyError):
             return res
         except (
             DAV_Error, DAV_NotFound, DAV_Secret, DAV_Forbidden) as exception:
             self._log_exception(exception)
             raise
         except Exception as exception:
             self._log_exception(exception)
```

### Comparing `m9s_webdav-6.0.1/server.py` & `m9s_webdav-6.0.2/server.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,17 +16,14 @@
 
 
 class TrytonWebdavServer(object):
 
     def __init__(self, options):
 
         config.update_etc(options.configfile)
-        print('__init__', dir(config))
-        print('__init__', config.sections())
-        print('__init__', config.get('database', 'uri'))
 
         if options.logconf:
             logging.config.fileConfig(options.logconf)
             logging.getLogger('server').info('using %s as logging '
                 'configuration file', options.logconf)
         else:
             logformat = ('%(process)s %(thread)s [%(asctime)s] '
@@ -57,16 +54,14 @@
         if hasattr(signal, 'SIGUSR1'):
             signal.signal(signal.SIGUSR1, lambda *a: self.restart())
 
         if self.options.pidfile:
             with open(self.options.pidfile, 'w') as fd_pid:
                 fd_pid.write("%d" % (os.getpid()))
 
-        print(self.options)
-        print('run', config.get('database', 'uri'))
         for db_name in self.options.database_names:
             Pool(db_name).init()
 
         self.start_servers()
 
         while True:
             if self.options.dev:
```

### Comparing `m9s_webdav-6.0.1/setup.py` & `m9s_webdav-6.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `m9s_webdav-6.0.1/view/share_form.xml` & `m9s_webdav-6.0.2/view/share_form.xml`

 * *Files identical despite different names*

### Comparing `m9s_webdav-6.0.1/webdav.py` & `m9s_webdav-6.0.2/webdav.py`

 * *Files 2% similar despite different names*

```diff
@@ -432,19 +432,20 @@
                 for sub_ids in grouped_slice(ids):
                     red_sql = reduce_ids(table.id, sub_ids)
                     cursor.execute(*table.select(table.id,
                             Extract('EPOCH', table.create_date),
                             where=red_sql))
                     for object_id2, date in cursor.fetchall():
                         if object_id2 == object_id:
-                            res = date
+                            # Python 3.11 returns Decimal, pywebdav needs float
+                            res = float(date)
                         if cache is not None:
                             cache[Model.__name__].setdefault(object_id2, {})
                             cache[Model.__name__][object_id2][
-                                'creationdate'] = date
+                                'creationdate'] = res
                 if res is not None:
                     return res
         return time.time()
 
     @classmethod
     def get_lastmodified(cls, uri, cache=None):
         pool = Pool()
@@ -469,19 +470,20 @@
                     red_sql = reduce_ids(table.id, sub_ids)
                     cursor.execute(*table.select(table.id,
                             Extract('EPOCH',
                                 Coalesce(table.write_date, table.create_date)),
                             where=red_sql))
                     for object_id2, date in cursor.fetchall():
                         if object_id2 == object_id:
-                            res = date
+                            # Python 3.11 returns Decimal, pywebdav needs float
+                            res = float(date)
                         if cache is not None:
                             cache[Model.__name__].setdefault(object_id2, {})
                             cache[Model.__name__][object_id2][
-                                'lastmodified'] = date
+                                'lastmodified'] = res
                 if res is not None:
                     return res
         return time.time()
 
     @classmethod
     def get_data(cls, uri, cache=None):
         from pywebdav.lib.errors import DAV_NotFound
```

### Comparing `m9s_webdav-6.0.1/webdav.xml` & `m9s_webdav-6.0.2/webdav.xml`

 * *Files identical despite different names*

