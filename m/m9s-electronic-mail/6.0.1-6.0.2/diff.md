# Comparing `tmp/m9s_electronic_mail-6.0.1.tar.gz` & `tmp/m9s_electronic_mail-6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m9s_electronic_mail-6.0.1.tar", last modified: Fri Nov 11 10:58:03 2022, max compression
+gzip compressed data, was "m9s_electronic_mail-6.0.2.tar", last modified: Tue May 30 16:22:23 2023, max compression
```

## Comparing `m9s_electronic_mail-6.0.1.tar` & `m9s_electronic_mail-6.0.2.tar`

### file list

```diff
@@ -1,64 +1,68 @@
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-11 10:58:03.291845 m9s_electronic_mail-6.0.1/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       85 2022-01-26 10:04:01.000000 m9s_electronic_mail-6.0.1/.coveragerc
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-01-26 10:04:01.000000 m9s_electronic_mail-6.0.1/.drone.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2022-01-26 10:04:01.000000 m9s_electronic_mail-6.0.1/.flake8
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1787 2022-11-11 10:54:21.000000 m9s_electronic_mail-6.0.1/.gitlab-ci.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2022-01-26 10:04:01.000000 m9s_electronic_mail-6.0.1/.isort.cfg
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      479 2018-02-28 18:25:29.000000 m9s_electronic_mail-6.0.1/.travis.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      726 2022-01-28 16:16:15.000000 m9s_electronic_mail-6.0.1/COPYRIGHT
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2020-02-01 23:15:46.000000 m9s_electronic_mail-6.0.1/INSTALL
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2018-02-28 18:25:29.000000 m9s_electronic_mail-6.0.1/LICENSE
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      125 2022-01-26 10:04:01.000000 m9s_electronic_mail-6.0.1/MANIFEST.in
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3343 2022-11-11 10:58:03.291845 m9s_electronic_mail-6.0.1/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1252 2020-02-01 23:15:46.000000 m9s_electronic_mail-6.0.1/README.md
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2020-01-23 15:59:27.000000 m9s_electronic_mail-6.0.1/README.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      789 2021-12-11 18:42:45.000000 m9s_electronic_mail-6.0.1/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1024 2022-02-11 20:23:08.000000 m9s_electronic_mail-6.0.1/action.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      450 2020-02-01 23:15:46.000000 m9s_electronic_mail-6.0.1/action.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      640 2022-03-05 15:28:26.000000 m9s_electronic_mail-6.0.1/activity.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       77 2022-03-05 15:29:46.000000 m9s_electronic_mail-6.0.1/dev_requirements.txt
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-11 10:58:03.287845 m9s_electronic_mail-6.0.1/doc/
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-11 10:58:03.287845 m9s_electronic_mail-6.0.1/doc/de/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       45 2020-02-01 23:15:46.000000 m9s_electronic_mail-6.0.1/doc/de/index.rst
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-11 10:58:03.287845 m9s_electronic_mail-6.0.1/doc/es/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2018-02-28 18:25:29.000000 m9s_electronic_mail-6.0.1/doc/es/index.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2020-01-23 15:59:27.000000 m9s_electronic_mail-6.0.1/doc/index.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1011 2020-02-01 23:15:46.000000 m9s_electronic_mail-6.0.1/electronic_mail.xml
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-11 10:58:03.287845 m9s_electronic_mail-6.0.1/locale/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     8397 2020-02-01 22:27:37.000000 m9s_electronic_mail-6.0.1/locale/ca.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     7257 2022-03-10 16:54:47.000000 m9s_electronic_mail-6.0.1/locale/de.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     8542 2020-02-01 22:27:37.000000 m9s_electronic_mail-6.0.1/locale/es.po
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-11 10:58:03.291845 m9s_electronic_mail-6.0.1/m9s_electronic_mail.egg-info/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3343 2022-11-11 10:58:03.000000 m9s_electronic_mail-6.0.1/m9s_electronic_mail.egg-info/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1581 2022-11-11 10:58:03.000000 m9s_electronic_mail-6.0.1/m9s_electronic_mail.egg-info/SOURCES.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2022-11-11 10:58:03.000000 m9s_electronic_mail-6.0.1/m9s_electronic_mail.egg-info/dependency_links.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       68 2022-11-11 10:58:03.000000 m9s_electronic_mail-6.0.1/m9s_electronic_mail.egg-info/entry_points.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2021-03-04 23:59:25.000000 m9s_electronic_mail-6.0.1/m9s_electronic_mail.egg-info/not-zip-safe
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       70 2022-11-11 10:58:03.000000 m9s_electronic_mail-6.0.1/m9s_electronic_mail.egg-info/requires.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2022-11-11 10:58:03.000000 m9s_electronic_mail-6.0.1/m9s_electronic_mail.egg-info/top_level.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      881 2022-02-11 21:02:20.000000 m9s_electronic_mail-6.0.1/message.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2022-01-26 10:04:01.000000 m9s_electronic_mail-6.0.1/requirements.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       38 2022-11-11 10:58:03.291845 m9s_electronic_mail-6.0.1/setup.cfg
--rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4793 2022-11-11 10:47:02.000000 m9s_electronic_mail-6.0.1/setup.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    20034 2022-11-11 10:47:02.000000 m9s_electronic_mail-6.0.1/template.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3865 2021-12-11 18:21:18.000000 m9s_electronic_mail-6.0.1/template.xml
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-11 10:58:03.287845 m9s_electronic_mail-6.0.1/tests/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      297 2021-12-11 18:42:45.000000 m9s_electronic_mail-6.0.1/tests/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2739 2021-12-16 10:01:02.000000 m9s_electronic_mail-6.0.1/tests/t.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2727 2021-12-11 18:42:45.000000 m9s_electronic_mail-6.0.1/tests/test_electronic_mail.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      749 2022-04-30 07:53:53.000000 m9s_electronic_mail-6.0.1/tox.ini
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      716 2022-02-11 21:05:39.000000 m9s_electronic_mail-6.0.1/trigger.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      426 2020-02-01 23:15:46.000000 m9s_electronic_mail-6.0.1/trigger.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      166 2022-02-11 21:06:47.000000 m9s_electronic_mail-6.0.1/tryton.cfg
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      509 2022-02-11 20:19:37.000000 m9s_electronic_mail-6.0.1/user.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      416 2020-02-01 23:15:46.000000 m9s_electronic_mail-6.0.1/user.xml
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-11 10:58:03.287845 m9s_electronic_mail-6.0.1/view/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      342 2022-02-11 20:56:08.000000 m9s_electronic_mail-6.0.1/view/action_report_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      947 2020-02-01 23:15:46.000000 m9s_electronic_mail-6.0.1/view/send_template_start.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2198 2021-12-11 18:21:18.000000 m9s_electronic_mail-6.0.1/view/template_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      268 2021-12-11 18:21:18.000000 m9s_electronic_mail-6.0.1/view/template_report_view_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      212 2021-12-11 18:21:18.000000 m9s_electronic_mail-6.0.1/view/template_report_view_list.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      232 2021-12-11 18:21:18.000000 m9s_electronic_mail-6.0.1/view/template_report_view_list_sequence.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      291 2020-02-01 23:15:46.000000 m9s_electronic_mail-6.0.1/view/template_tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      324 2022-02-11 20:54:05.000000 m9s_electronic_mail-6.0.1/view/trigger_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      368 2020-02-01 23:15:46.000000 m9s_electronic_mail-6.0.1/view/user_form.xml
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:22:23.416330 m9s_electronic_mail-6.0.2/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       85 2022-01-26 10:04:01.000000 m9s_electronic_mail-6.0.2/.coveragerc
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-01-26 10:04:01.000000 m9s_electronic_mail-6.0.2/.drone.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2022-01-26 10:04:01.000000 m9s_electronic_mail-6.0.2/.flake8
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1787 2022-11-13 14:32:56.000000 m9s_electronic_mail-6.0.2/.gitlab-ci.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2022-01-26 10:04:01.000000 m9s_electronic_mail-6.0.2/.isort.cfg
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      479 2018-02-28 18:25:29.000000 m9s_electronic_mail-6.0.2/.travis.yml
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:22:23.412330 m9s_electronic_mail-6.0.2/.woodpecker/
+-rwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2022-11-23 17:28:52.000000 m9s_electronic_mail-6.0.2/.woodpecker/mail_curl.sh
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2022-11-23 20:42:33.000000 m9s_electronic_mail-6.0.2/.woodpecker/report.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1468 2022-11-24 15:51:07.000000 m9s_electronic_mail-6.0.2/.woodpecker/test.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      726 2022-01-28 16:16:15.000000 m9s_electronic_mail-6.0.2/COPYRIGHT
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2020-02-01 23:15:46.000000 m9s_electronic_mail-6.0.2/INSTALL
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2018-02-28 18:25:29.000000 m9s_electronic_mail-6.0.2/LICENSE
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      125 2022-01-26 10:04:01.000000 m9s_electronic_mail-6.0.2/MANIFEST.in
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3343 2023-05-30 16:22:23.416330 m9s_electronic_mail-6.0.2/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1252 2020-02-01 23:15:46.000000 m9s_electronic_mail-6.0.2/README.md
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2020-01-23 15:59:27.000000 m9s_electronic_mail-6.0.2/README.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      789 2021-12-11 18:42:45.000000 m9s_electronic_mail-6.0.2/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1024 2022-02-11 20:23:08.000000 m9s_electronic_mail-6.0.2/action.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      450 2020-02-01 23:15:46.000000 m9s_electronic_mail-6.0.2/action.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      640 2022-03-05 15:28:26.000000 m9s_electronic_mail-6.0.2/activity.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       77 2022-03-05 15:29:46.000000 m9s_electronic_mail-6.0.2/dev_requirements.txt
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:22:23.416330 m9s_electronic_mail-6.0.2/doc/
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:22:23.416330 m9s_electronic_mail-6.0.2/doc/de/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       45 2020-02-01 23:15:46.000000 m9s_electronic_mail-6.0.2/doc/de/index.rst
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:22:23.416330 m9s_electronic_mail-6.0.2/doc/es/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2018-02-28 18:25:29.000000 m9s_electronic_mail-6.0.2/doc/es/index.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2020-01-23 15:59:27.000000 m9s_electronic_mail-6.0.2/doc/index.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1011 2020-02-01 23:15:46.000000 m9s_electronic_mail-6.0.2/electronic_mail.xml
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:22:23.408330 m9s_electronic_mail-6.0.2/locale/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     8397 2020-02-01 22:27:37.000000 m9s_electronic_mail-6.0.2/locale/ca.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     7257 2022-03-10 16:54:47.000000 m9s_electronic_mail-6.0.2/locale/de.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     8542 2020-02-01 22:27:37.000000 m9s_electronic_mail-6.0.2/locale/es.po
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:22:23.416330 m9s_electronic_mail-6.0.2/m9s_electronic_mail.egg-info/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3343 2023-05-30 16:22:23.000000 m9s_electronic_mail-6.0.2/m9s_electronic_mail.egg-info/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1650 2023-05-30 16:22:23.000000 m9s_electronic_mail-6.0.2/m9s_electronic_mail.egg-info/SOURCES.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2023-05-30 16:22:23.000000 m9s_electronic_mail-6.0.2/m9s_electronic_mail.egg-info/dependency_links.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       68 2023-05-30 16:22:23.000000 m9s_electronic_mail-6.0.2/m9s_electronic_mail.egg-info/entry_points.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2021-03-04 23:59:25.000000 m9s_electronic_mail-6.0.2/m9s_electronic_mail.egg-info/not-zip-safe
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       70 2023-05-30 16:22:23.000000 m9s_electronic_mail-6.0.2/m9s_electronic_mail.egg-info/requires.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2023-05-30 16:22:23.000000 m9s_electronic_mail-6.0.2/m9s_electronic_mail.egg-info/top_level.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      881 2022-02-11 21:02:20.000000 m9s_electronic_mail-6.0.2/message.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2022-01-26 10:04:01.000000 m9s_electronic_mail-6.0.2/requirements.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       38 2023-05-30 16:22:23.416330 m9s_electronic_mail-6.0.2/setup.cfg
+-rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4793 2022-11-11 10:47:02.000000 m9s_electronic_mail-6.0.2/setup.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    20085 2022-11-24 17:10:21.000000 m9s_electronic_mail-6.0.2/template.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3865 2021-12-11 18:21:18.000000 m9s_electronic_mail-6.0.2/template.xml
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:22:23.412330 m9s_electronic_mail-6.0.2/tests/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      297 2021-12-11 18:42:45.000000 m9s_electronic_mail-6.0.2/tests/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2739 2021-12-16 10:01:02.000000 m9s_electronic_mail-6.0.2/tests/t.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2727 2021-12-11 18:42:45.000000 m9s_electronic_mail-6.0.2/tests/test_electronic_mail.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      843 2022-11-24 17:09:09.000000 m9s_electronic_mail-6.0.2/tox.ini
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      716 2022-02-11 21:05:39.000000 m9s_electronic_mail-6.0.2/trigger.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      426 2020-02-01 23:15:46.000000 m9s_electronic_mail-6.0.2/trigger.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      166 2022-11-11 10:58:11.000000 m9s_electronic_mail-6.0.2/tryton.cfg
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      509 2022-02-11 20:19:37.000000 m9s_electronic_mail-6.0.2/user.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      416 2020-02-01 23:15:46.000000 m9s_electronic_mail-6.0.2/user.xml
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:22:23.412330 m9s_electronic_mail-6.0.2/view/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      342 2022-02-11 20:56:08.000000 m9s_electronic_mail-6.0.2/view/action_report_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      947 2020-02-01 23:15:46.000000 m9s_electronic_mail-6.0.2/view/send_template_start.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2198 2021-12-11 18:21:18.000000 m9s_electronic_mail-6.0.2/view/template_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      268 2021-12-11 18:21:18.000000 m9s_electronic_mail-6.0.2/view/template_report_view_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      212 2021-12-11 18:21:18.000000 m9s_electronic_mail-6.0.2/view/template_report_view_list.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      232 2021-12-11 18:21:18.000000 m9s_electronic_mail-6.0.2/view/template_report_view_list_sequence.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      291 2020-02-01 23:15:46.000000 m9s_electronic_mail-6.0.2/view/template_tree.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      324 2022-02-11 20:54:05.000000 m9s_electronic_mail-6.0.2/view/trigger_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      368 2020-02-01 23:15:46.000000 m9s_electronic_mail-6.0.2/view/user_form.xml
```

### Comparing `m9s_electronic_mail-6.0.1/.drone.yml` & `m9s_electronic_mail-6.0.2/.drone.yml`

 * *Files identical despite different names*

### Comparing `m9s_electronic_mail-6.0.1/.gitlab-ci.yml` & `m9s_electronic_mail-6.0.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `m9s_electronic_mail-6.0.1/COPYRIGHT` & `m9s_electronic_mail-6.0.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `m9s_electronic_mail-6.0.1/INSTALL` & `m9s_electronic_mail-6.0.2/INSTALL`

 * *Files identical despite different names*

### Comparing `m9s_electronic_mail-6.0.1/LICENSE` & `m9s_electronic_mail-6.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `m9s_electronic_mail-6.0.1/PKG-INFO` & `m9s_electronic_mail-6.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m9s_electronic_mail
-Version: 6.0.1
+Version: 6.0.2
 Summary: Tryton Electronic Mail Module
 Home-page: http://www.m9s.biz/
 Download-URL: https://gitlab.com/m9s/electronic_mail.git
 Author: MBSolutions
 Author-email: info@m9s.biz
 License: GPL-3
 Project-URL: Bug Tracker, https://support.m9s.biz/
```

### Comparing `m9s_electronic_mail-6.0.1/README.md` & `m9s_electronic_mail-6.0.2/README.md`

 * *Files identical despite different names*

### Comparing `m9s_electronic_mail-6.0.1/__init__.py` & `m9s_electronic_mail-6.0.2/__init__.py`

 * *Files identical despite different names*

### Comparing `m9s_electronic_mail-6.0.1/action.py` & `m9s_electronic_mail-6.0.2/action.py`

 * *Files identical despite different names*

### Comparing `m9s_electronic_mail-6.0.1/activity.py` & `m9s_electronic_mail-6.0.2/activity.py`

 * *Files identical despite different names*

### Comparing `m9s_electronic_mail-6.0.1/electronic_mail.xml` & `m9s_electronic_mail-6.0.2/electronic_mail.xml`

 * *Files identical despite different names*

### Comparing `m9s_electronic_mail-6.0.1/locale/ca.po` & `m9s_electronic_mail-6.0.2/locale/ca.po`

 * *Files identical despite different names*

### Comparing `m9s_electronic_mail-6.0.1/locale/de.po` & `m9s_electronic_mail-6.0.2/locale/de.po`

 * *Files identical despite different names*

### Comparing `m9s_electronic_mail-6.0.1/locale/es.po` & `m9s_electronic_mail-6.0.2/locale/es.po`

 * *Files identical despite different names*

### Comparing `m9s_electronic_mail-6.0.1/m9s_electronic_mail.egg-info/PKG-INFO` & `m9s_electronic_mail-6.0.2/m9s_electronic_mail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m9s-electronic-mail
-Version: 6.0.1
+Version: 6.0.2
 Summary: Tryton Electronic Mail Module
 Home-page: http://www.m9s.biz/
 Download-URL: https://gitlab.com/m9s/electronic_mail.git
 Author: MBSolutions
 Author-email: info@m9s.biz
 License: GPL-3
 Project-URL: Bug Tracker, https://support.m9s.biz/
```

### Comparing `m9s_electronic_mail-6.0.1/m9s_electronic_mail.egg-info/SOURCES.txt` & `m9s_electronic_mail-6.0.2/m9s_electronic_mail.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,17 @@
 ./view/template_form.xml
 ./view/template_report_view_form.xml
 ./view/template_report_view_list.xml
 ./view/template_report_view_list_sequence.xml
 ./view/template_tree.xml
 ./view/trigger_form.xml
 ./view/user_form.xml
+.woodpecker/mail_curl.sh
+.woodpecker/report.yml
+.woodpecker/test.yml
 doc/index.rst
 doc/de/index.rst
 doc/es/index.rst
 locale/ca.po
 locale/de.po
 locale/es.po
 m9s_electronic_mail.egg-info/PKG-INFO
```

### Comparing `m9s_electronic_mail-6.0.1/message.xml` & `m9s_electronic_mail-6.0.2/message.xml`

 * *Files identical despite different names*

### Comparing `m9s_electronic_mail-6.0.1/setup.py` & `m9s_electronic_mail-6.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `m9s_electronic_mail-6.0.1/template.py` & `m9s_electronic_mail-6.0.2/template.py`

 * *Files 0% similar despite different names*

```diff
@@ -512,14 +512,16 @@
                 gettext('electronic_mail.msg_missing_template'))
         total = len(active_ids)
 
         # TODO IMP to load first record and not browse all active ids
         records = pool.get(template.model.model).browse(active_ids)
 
         default = {}
+        if not records:
+            return default
         default['template'] = template.id
         default['total'] = total
         for k, v in list(template.pre_render(records)[0].items()):
             default[k] = v
         return default
 
     def transition_send(self):
```

### Comparing `m9s_electronic_mail-6.0.1/template.xml` & `m9s_electronic_mail-6.0.2/template.xml`

 * *Files identical despite different names*

### Comparing `m9s_electronic_mail-6.0.1/tests/t.py` & `m9s_electronic_mail-6.0.2/tests/t.py`

 * *Files identical despite different names*

### Comparing `m9s_electronic_mail-6.0.1/tests/test_electronic_mail.py` & `m9s_electronic_mail-6.0.2/tests/test_electronic_mail.py`

 * *Files identical despite different names*

### Comparing `m9s_electronic_mail-6.0.1/trigger.py` & `m9s_electronic_mail-6.0.2/trigger.py`

 * *Files identical despite different names*

### Comparing `m9s_electronic_mail-6.0.1/view/send_template_start.xml` & `m9s_electronic_mail-6.0.2/view/send_template_start.xml`

 * *Files identical despite different names*

### Comparing `m9s_electronic_mail-6.0.1/view/template_form.xml` & `m9s_electronic_mail-6.0.2/view/template_form.xml`

 * *Files identical despite different names*

