# Comparing `tmp/m9s_sale_payment_gateway-6.0.2.tar.gz` & `tmp/m9s_sale_payment_gateway-6.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m9s_sale_payment_gateway-6.0.2.tar", last modified: Fri Apr  8 10:07:28 2022, max compression
+gzip compressed data, was "m9s_sale_payment_gateway-6.0.3.tar", last modified: Tue May 30 16:25:35 2023, max compression
```

## Comparing `m9s_sale_payment_gateway-6.0.2.tar` & `m9s_sale_payment_gateway-6.0.3.tar`

### file list

```diff
@@ -1,61 +1,65 @@
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-04-08 10:07:28.360756 m9s_sale_payment_gateway-6.0.2/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       90 2022-01-26 10:04:15.000000 m9s_sale_payment_gateway-6.0.2/.coveragerc
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-01-26 10:04:15.000000 m9s_sale_payment_gateway-6.0.2/.drone.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2022-01-26 10:04:15.000000 m9s_sale_payment_gateway-6.0.2/.flake8
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      526 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.2/.gitignore
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1787 2022-01-26 10:04:15.000000 m9s_sale_payment_gateway-6.0.2/.gitlab-ci.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2022-01-26 10:04:15.000000 m9s_sale_payment_gateway-6.0.2/.isort.cfg
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      212 2018-02-28 18:26:37.000000 m9s_sale_payment_gateway-6.0.2/.travis.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      794 2022-01-28 16:17:31.000000 m9s_sale_payment_gateway-6.0.2/COPYRIGHT
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.2/INSTALL
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.2/LICENSE
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      125 2022-01-26 10:04:15.000000 m9s_sale_payment_gateway-6.0.2/MANIFEST.in
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      318 2018-02-28 18:26:37.000000 m9s_sale_payment_gateway-6.0.2/Makefile
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3418 2022-04-08 10:07:28.360756 m9s_sale_payment_gateway-6.0.2/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1287 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.2/README.md
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      192 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.2/README.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      612 2021-12-11 18:43:09.000000 m9s_sale_payment_gateway-6.0.2/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1417 2021-12-11 18:43:09.000000 m9s_sale_payment_gateway-6.0.2/configuration.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      464 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.2/configuration.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       77 2022-03-05 15:54:49.000000 m9s_sale_payment_gateway-6.0.2/dev_requirements.txt
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-04-08 10:07:28.360756 m9s_sale_payment_gateway-6.0.2/doc/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     6810 2018-02-28 18:26:37.000000 m9s_sale_payment_gateway-6.0.2/doc/Makefile
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     8268 2022-02-12 16:49:03.000000 m9s_sale_payment_gateway-6.0.2/doc/conf.py
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-04-08 10:07:28.360756 m9s_sale_payment_gateway-6.0.2/doc/de/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       55 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.2/doc/de/index.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      192 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.2/doc/index.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      444 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.2/ir.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      443 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.2/ir.xml
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-04-08 10:07:28.356756 m9s_sale_payment_gateway-6.0.2/locale/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    13072 2021-09-17 06:28:11.000000 m9s_sale_payment_gateway-6.0.2/locale/de.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     9491 2018-02-28 18:26:37.000000 m9s_sale_payment_gateway-6.0.2/locale/fr_FR.po
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-04-08 10:07:28.360756 m9s_sale_payment_gateway-6.0.2/m9s_sale_payment_gateway.egg-info/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3418 2022-04-08 10:07:28.000000 m9s_sale_payment_gateway-6.0.2/m9s_sale_payment_gateway.egg-info/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1471 2022-04-08 10:07:28.000000 m9s_sale_payment_gateway-6.0.2/m9s_sale_payment_gateway.egg-info/SOURCES.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2022-04-08 10:07:28.000000 m9s_sale_payment_gateway-6.0.2/m9s_sale_payment_gateway.egg-info/dependency_links.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       91 2022-04-08 10:07:28.000000 m9s_sale_payment_gateway-6.0.2/m9s_sale_payment_gateway.egg-info/entry_points.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2020-01-15 17:20:50.000000 m9s_sale_payment_gateway-6.0.2/m9s_sale_payment_gateway.egg-info/not-zip-safe
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      113 2022-04-08 10:07:28.000000 m9s_sale_payment_gateway-6.0.2/m9s_sale_payment_gateway.egg-info/requires.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2022-04-08 10:07:28.000000 m9s_sale_payment_gateway-6.0.2/m9s_sale_payment_gateway.egg-info/top_level.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2130 2022-02-12 15:28:50.000000 m9s_sale_payment_gateway-6.0.2/message.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    10230 2022-02-12 15:50:53.000000 m9s_sale_payment_gateway-6.0.2/payment.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3509 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.2/payment.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2022-01-26 10:04:15.000000 m9s_sale_payment_gateway-6.0.2/requirements.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    32513 2022-04-08 10:04:03.000000 m9s_sale_payment_gateway-6.0.2/sale.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3284 2022-02-12 16:48:41.000000 m9s_sale_payment_gateway-6.0.2/sale.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      270 2022-04-08 10:07:28.360756 m9s_sale_payment_gateway-6.0.2/setup.cfg
--rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4804 2022-02-12 12:08:23.000000 m9s_sale_payment_gateway-6.0.2/setup.py
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-04-08 10:07:28.356756 m9s_sale_payment_gateway-6.0.2/tests/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      353 2021-12-11 18:43:09.000000 m9s_sale_payment_gateway-6.0.2/tests/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    87062 2022-02-12 15:26:48.000000 m9s_sale_payment_gateway-6.0.2/tests/test_sale_payment_gateway.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      745 2022-01-26 10:04:15.000000 m9s_sale_payment_gateway-6.0.2/tox.ini
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      468 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.2/transaction.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      262 2022-02-12 16:49:03.000000 m9s_sale_payment_gateway-6.0.2/tryton.cfg
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-04-08 10:07:28.356756 m9s_sale_payment_gateway-6.0.2/view/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      507 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.2/view/configuration_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1211 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.2/view/sale_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1545 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.2/view/sale_payment_add_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      192 2021-05-12 10:43:20.000000 m9s_sale_payment_gateway-6.0.2/view/sale_payment_ask_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      980 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.2/view/sale_payment_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      346 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.2/view/sale_payment_tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      304 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.2/view/transaction_form.xml
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:25:35.143156 m9s_sale_payment_gateway-6.0.3/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       90 2022-01-26 10:04:15.000000 m9s_sale_payment_gateway-6.0.3/.coveragerc
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-01-26 10:04:15.000000 m9s_sale_payment_gateway-6.0.3/.drone.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2022-01-26 10:04:15.000000 m9s_sale_payment_gateway-6.0.3/.flake8
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      526 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.3/.gitignore
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1785 2022-11-13 14:32:56.000000 m9s_sale_payment_gateway-6.0.3/.gitlab-ci.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2022-01-26 10:04:15.000000 m9s_sale_payment_gateway-6.0.3/.isort.cfg
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      212 2018-02-28 18:26:37.000000 m9s_sale_payment_gateway-6.0.3/.travis.yml
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:25:35.139156 m9s_sale_payment_gateway-6.0.3/.woodpecker/
+-rwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2022-11-23 17:28:52.000000 m9s_sale_payment_gateway-6.0.3/.woodpecker/mail_curl.sh
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2022-11-23 20:42:33.000000 m9s_sale_payment_gateway-6.0.3/.woodpecker/report.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1468 2022-11-24 15:51:07.000000 m9s_sale_payment_gateway-6.0.3/.woodpecker/test.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      794 2022-01-28 16:17:31.000000 m9s_sale_payment_gateway-6.0.3/COPYRIGHT
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.3/INSTALL
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.3/LICENSE
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      125 2022-01-26 10:04:15.000000 m9s_sale_payment_gateway-6.0.3/MANIFEST.in
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      318 2018-02-28 18:26:37.000000 m9s_sale_payment_gateway-6.0.3/Makefile
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3398 2023-05-30 16:25:35.143156 m9s_sale_payment_gateway-6.0.3/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1287 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.3/README.md
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      192 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.3/README.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      612 2021-12-11 18:43:09.000000 m9s_sale_payment_gateway-6.0.3/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1417 2021-12-11 18:43:09.000000 m9s_sale_payment_gateway-6.0.3/configuration.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      464 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.3/configuration.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      121 2023-05-30 16:18:49.000000 m9s_sale_payment_gateway-6.0.3/dev_requirements.txt
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:25:35.143156 m9s_sale_payment_gateway-6.0.3/doc/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     6810 2018-02-28 18:26:37.000000 m9s_sale_payment_gateway-6.0.3/doc/Makefile
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     8268 2022-04-08 10:07:34.000000 m9s_sale_payment_gateway-6.0.3/doc/conf.py
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:25:35.143156 m9s_sale_payment_gateway-6.0.3/doc/de/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       55 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.3/doc/de/index.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      192 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.3/doc/index.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      444 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.3/ir.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      443 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.3/ir.xml
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:25:35.135156 m9s_sale_payment_gateway-6.0.3/locale/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    13072 2021-09-17 06:28:11.000000 m9s_sale_payment_gateway-6.0.3/locale/de.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     9491 2018-02-28 18:26:37.000000 m9s_sale_payment_gateway-6.0.3/locale/fr_FR.po
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:25:35.143156 m9s_sale_payment_gateway-6.0.3/m9s_sale_payment_gateway.egg-info/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3398 2023-05-30 16:25:34.000000 m9s_sale_payment_gateway-6.0.3/m9s_sale_payment_gateway.egg-info/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1540 2023-05-30 16:25:35.000000 m9s_sale_payment_gateway-6.0.3/m9s_sale_payment_gateway.egg-info/SOURCES.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2023-05-30 16:25:34.000000 m9s_sale_payment_gateway-6.0.3/m9s_sale_payment_gateway.egg-info/dependency_links.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       78 2023-05-30 16:25:34.000000 m9s_sale_payment_gateway-6.0.3/m9s_sale_payment_gateway.egg-info/entry_points.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2020-01-15 17:20:50.000000 m9s_sale_payment_gateway-6.0.3/m9s_sale_payment_gateway.egg-info/not-zip-safe
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      113 2023-05-30 16:25:34.000000 m9s_sale_payment_gateway-6.0.3/m9s_sale_payment_gateway.egg-info/requires.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2023-05-30 16:25:34.000000 m9s_sale_payment_gateway-6.0.3/m9s_sale_payment_gateway.egg-info/top_level.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2130 2022-02-12 15:28:50.000000 m9s_sale_payment_gateway-6.0.3/message.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    10237 2022-04-30 08:10:09.000000 m9s_sale_payment_gateway-6.0.3/payment.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3509 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.3/payment.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2022-01-26 10:04:15.000000 m9s_sale_payment_gateway-6.0.3/requirements.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    32347 2023-05-30 16:18:49.000000 m9s_sale_payment_gateway-6.0.3/sale.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3284 2022-02-12 16:48:41.000000 m9s_sale_payment_gateway-6.0.3/sale.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      270 2023-05-30 16:25:35.143156 m9s_sale_payment_gateway-6.0.3/setup.cfg
+-rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4804 2022-02-12 12:08:23.000000 m9s_sale_payment_gateway-6.0.3/setup.py
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:25:35.135156 m9s_sale_payment_gateway-6.0.3/tests/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      353 2021-12-11 18:43:09.000000 m9s_sale_payment_gateway-6.0.3/tests/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    87062 2022-02-12 15:26:48.000000 m9s_sale_payment_gateway-6.0.3/tests/test_sale_payment_gateway.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      843 2022-11-24 16:26:27.000000 m9s_sale_payment_gateway-6.0.3/tox.ini
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      468 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.3/transaction.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      262 2022-04-30 08:10:09.000000 m9s_sale_payment_gateway-6.0.3/tryton.cfg
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:25:35.139156 m9s_sale_payment_gateway-6.0.3/view/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      507 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.3/view/configuration_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1211 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.3/view/sale_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1545 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.3/view/sale_payment_add_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      192 2021-05-12 10:43:20.000000 m9s_sale_payment_gateway-6.0.3/view/sale_payment_ask_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      980 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.3/view/sale_payment_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      346 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.3/view/sale_payment_tree.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      304 2020-01-24 00:47:26.000000 m9s_sale_payment_gateway-6.0.3/view/transaction_form.xml
```

### Comparing `m9s_sale_payment_gateway-6.0.2/.drone.yml` & `m9s_sale_payment_gateway-6.0.3/.drone.yml`

 * *Files identical despite different names*

### Comparing `m9s_sale_payment_gateway-6.0.2/.gitignore` & `m9s_sale_payment_gateway-6.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `m9s_sale_payment_gateway-6.0.2/.gitlab-ci.yml` & `m9s_sale_payment_gateway-6.0.3/.gitlab-ci.yml`

 * *Files 2% similar despite different names*

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
```

### Comparing `m9s_sale_payment_gateway-6.0.2/COPYRIGHT` & `m9s_sale_payment_gateway-6.0.3/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `m9s_sale_payment_gateway-6.0.2/INSTALL` & `m9s_sale_payment_gateway-6.0.3/INSTALL`

 * *Files identical despite different names*

### Comparing `m9s_sale_payment_gateway-6.0.2/LICENSE` & `m9s_sale_payment_gateway-6.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `m9s_sale_payment_gateway-6.0.2/PKG-INFO` & `m9s_sale_payment_gateway-6.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: m9s_sale_payment_gateway
-Version: 6.0.2
+Version: 6.0.3
 Summary: Tryton Sale Payment Gateway Module
 Home-page: http://www.m9s.biz/
+Download-URL: https://gitlab.com/m9s/sale_payment_gateway.git
 Author: MBSolutions
 Author-email: info@m9s.biz
 License: GPL-3
-Download-URL: https://gitlab.com/m9s/sale_payment_gateway.git
 Project-URL: Bug Tracker, https://support.m9s.biz/
 Project-URL: Source Code, https://gitlab.com/m9s/sale_payment_gateway.git
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

### Comparing `m9s_sale_payment_gateway-6.0.2/README.md` & `m9s_sale_payment_gateway-6.0.3/README.md`

 * *Files identical despite different names*

### Comparing `m9s_sale_payment_gateway-6.0.2/__init__.py` & `m9s_sale_payment_gateway-6.0.3/__init__.py`

 * *Files identical despite different names*

### Comparing `m9s_sale_payment_gateway-6.0.2/configuration.py` & `m9s_sale_payment_gateway-6.0.3/configuration.py`

 * *Files identical despite different names*

### Comparing `m9s_sale_payment_gateway-6.0.2/doc/Makefile` & `m9s_sale_payment_gateway-6.0.3/doc/Makefile`

 * *Files identical despite different names*

### Comparing `m9s_sale_payment_gateway-6.0.2/doc/conf.py` & `m9s_sale_payment_gateway-6.0.3/doc/conf.py`

 * *Files identical despite different names*

### Comparing `m9s_sale_payment_gateway-6.0.2/locale/de.po` & `m9s_sale_payment_gateway-6.0.3/locale/de.po`

 * *Files identical despite different names*

### Comparing `m9s_sale_payment_gateway-6.0.2/locale/fr_FR.po` & `m9s_sale_payment_gateway-6.0.3/locale/fr_FR.po`

 * *Files identical despite different names*

### Comparing `m9s_sale_payment_gateway-6.0.2/m9s_sale_payment_gateway.egg-info/PKG-INFO` & `m9s_sale_payment_gateway-6.0.3/m9s_sale_payment_gateway.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: m9s-sale-payment-gateway
-Version: 6.0.2
+Version: 6.0.3
 Summary: Tryton Sale Payment Gateway Module
 Home-page: http://www.m9s.biz/
+Download-URL: https://gitlab.com/m9s/sale_payment_gateway.git
 Author: MBSolutions
 Author-email: info@m9s.biz
 License: GPL-3
-Download-URL: https://gitlab.com/m9s/sale_payment_gateway.git
 Project-URL: Bug Tracker, https://support.m9s.biz/
 Project-URL: Source Code, https://gitlab.com/m9s/sale_payment_gateway.git
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

### Comparing `m9s_sale_payment_gateway-6.0.2/m9s_sale_payment_gateway.egg-info/SOURCES.txt` & `m9s_sale_payment_gateway-6.0.3/m9s_sale_payment_gateway.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -48,14 +48,17 @@
 ./view/configuration_form.xml
 ./view/sale_form.xml
 ./view/sale_payment_add_form.xml
 ./view/sale_payment_ask_form.xml
 ./view/sale_payment_form.xml
 ./view/sale_payment_tree.xml
 ./view/transaction_form.xml
+.woodpecker/mail_curl.sh
+.woodpecker/report.yml
+.woodpecker/test.yml
 doc/Makefile
 doc/conf.py
 doc/index.rst
 doc/de/index.rst
 locale/de.po
 locale/fr_FR.po
 m9s_sale_payment_gateway.egg-info/PKG-INFO
```

### Comparing `m9s_sale_payment_gateway-6.0.2/message.xml` & `m9s_sale_payment_gateway-6.0.3/message.xml`

 * *Files identical despite different names*

### Comparing `m9s_sale_payment_gateway-6.0.2/payment.py` & `m9s_sale_payment_gateway-6.0.3/payment.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,16 +134,16 @@
     def __setup__(cls):
         super(Payment, cls).__setup__()
         cls._order.insert(0, ('sequence', 'ASC'))
 
     @fields.depends('sale', '_parent_sale.id')
     def on_change_with_credit_account(self, name=None):
         if self.sale and self.sale.party:
-            return self.sale.party.account_receivable and \
-                self.sale.party.account_receivable.id
+            receivable = self.sale.party.account_receivable_used
+            return receivable and receivable.id or None
 
     @fields.depends('sale', '_parent_sale.id')
     def on_change_with_company(self, name=None):
         return self.sale and self.sale.company.id or None
 
     @fields.depends('sale', '_parent_sale.id')
     def on_change_with_party(self, name=None):
```

### Comparing `m9s_sale_payment_gateway-6.0.2/payment.xml` & `m9s_sale_payment_gateway-6.0.3/payment.xml`

 * *Files identical despite different names*

### Comparing `m9s_sale_payment_gateway-6.0.2/sale.py` & `m9s_sale_payment_gateway-6.0.3/sale.py`

 * *Files 1% similar despite different names*

```diff
@@ -799,38 +799,36 @@
 
     def default_ask(self, data):
         return {
             'message': self.ask.message,
             }
 
     def default_payment_info(self, fields=None):
-        Sale = Pool().get('sale.sale')
-
-        sale = Sale(Transaction().context.get('active_id'))
-
+        sale = self.record
+        receivable = sale.party.account_receivable_used
         res = {
             'sale': sale.id,
             'company': sale.company.id,
             'party': sale.party.id,
-            'credit_account': sale.party.account_receivable.id,
+            'credit_account': receivable.id if receivable else None,
             'owner': sale.party.name,
             'currency_digits': sale.currency_digits,
             'amount': sale._get_amount_to_checkout(),
             'user': Transaction().user,
         }
         return res
 
     def transition_check(self):
         """
         Check step to show evtl. problems before proceeding
         """
         Sale = Pool().get('sale.sale')
 
         # Check for evtl. missing shipment costs
-        sale = Sale(Transaction().context.get('active_id'))
+        sale = self.record
         if (hasattr(Sale, 'carrier')
                 and sale.state == 'draft'
                 and sale.carrier):
             if not [l for l in sale.lines if l.shipment_cost]:
                 msg = gettext(
                     'sale_payment_gateway.msg_ask_shipment_cost',
                     sale=sale.rec_name)
@@ -840,18 +838,17 @@
 
     def create_sale_payment(self, profile=None):
         """
         Helper function to create a new payment
         or return an existing payment for the gateway.
         """
         pool = Pool()
-        Sale = pool.get('sale.sale')
         SalePayment = pool.get('sale.payment')
 
-        sale = Sale(Transaction().context.get('active_id'))
+        sale = self.record
         payments = [p for p in sale.payments
             if p.gateway == self.payment_info.gateway]
         if payments:
             return payments[0]
         payment_profile = profile
         if self.payment_info.method != 'credit_card':
             payment_profile = None
@@ -867,15 +864,14 @@
         )
         return payment
 
     def create_payment_profile(self):
         """
         Helper function to create payment profile
         """
-        Sale = Pool().get('sale.sale')
         ProfileWizard = Pool().get(
             'party.party.payment_profile.add', type="wizard"
         )
         profile_wizard = ProfileWizard(
             ProfileWizard.create()[0]
         )
         profile_wizard.card_info.owner = self.payment_info.owner
@@ -883,17 +879,15 @@
         profile_wizard.card_info.expiry_month = self.payment_info.expiry_month
         profile_wizard.card_info.expiry_year = self.payment_info.expiry_year
         profile_wizard.card_info.csc = self.payment_info.csc or ''
         profile_wizard.card_info.gateway = self.payment_info.gateway
         profile_wizard.card_info.provider = self.payment_info.gateway.provider
         profile_wizard.card_info.party = self.payment_info.party
 
-        billing_address = Sale(
-            Transaction().context.get('active_id')
-        ).invoice_address
+        billing_address = self.record.invoice_address
         if not billing_address:
             # If no billing address fallback to party's invoice address
             try:
                 billing_address = self.payment_info.party.address_get(
                     type='invoice'
                 )
             except AttributeError:
@@ -918,7 +912,10 @@
     def transition_finish(self):
         """
         Ends the wizard
 
         Override to append further processing (e.g. card data)
         """
         return 'end'
+
+    def end(self):
+        return 'reload'
```

### Comparing `m9s_sale_payment_gateway-6.0.2/sale.xml` & `m9s_sale_payment_gateway-6.0.3/sale.xml`

 * *Files identical despite different names*

### Comparing `m9s_sale_payment_gateway-6.0.2/setup.py` & `m9s_sale_payment_gateway-6.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `m9s_sale_payment_gateway-6.0.2/tests/test_sale_payment_gateway.py` & `m9s_sale_payment_gateway-6.0.3/tests/test_sale_payment_gateway.py`

 * *Files identical despite different names*

### Comparing `m9s_sale_payment_gateway-6.0.2/view/sale_form.xml` & `m9s_sale_payment_gateway-6.0.3/view/sale_form.xml`

 * *Files identical despite different names*

### Comparing `m9s_sale_payment_gateway-6.0.2/view/sale_payment_add_form.xml` & `m9s_sale_payment_gateway-6.0.3/view/sale_payment_add_form.xml`

 * *Files identical despite different names*

### Comparing `m9s_sale_payment_gateway-6.0.2/view/sale_payment_form.xml` & `m9s_sale_payment_gateway-6.0.3/view/sale_payment_form.xml`

 * *Files identical despite different names*

