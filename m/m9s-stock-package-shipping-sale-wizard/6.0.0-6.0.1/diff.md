# Comparing `tmp/m9s_stock_package_shipping_sale_wizard-6.0.0.tar.gz` & `tmp/m9s_stock_package_shipping_sale_wizard-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m9s_stock_package_shipping_sale_wizard-6.0.0.tar", last modified: Mon Feb 14 19:36:24 2022, max compression
+gzip compressed data, was "m9s_stock_package_shipping_sale_wizard-6.0.1.tar", last modified: Tue May 30 16:28:43 2023, max compression
```

## Comparing `m9s_stock_package_shipping_sale_wizard-6.0.0.tar` & `m9s_stock_package_shipping_sale_wizard-6.0.1.tar`

### file list

```diff
@@ -1,43 +1,47 @@
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-02-14 19:36:24.793872 m9s_stock_package_shipping_sale_wizard-6.0.0/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      104 2022-02-13 19:23:06.000000 m9s_stock_package_shipping_sale_wizard-6.0.0/.coveragerc
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-02-13 19:23:06.000000 m9s_stock_package_shipping_sale_wizard-6.0.0/.drone.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2022-02-13 19:23:06.000000 m9s_stock_package_shipping_sale_wizard-6.0.0/.flake8
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1787 2022-02-13 19:23:06.000000 m9s_stock_package_shipping_sale_wizard-6.0.0/.gitlab-ci.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2022-02-13 19:23:06.000000 m9s_stock_package_shipping_sale_wizard-6.0.0/.isort.cfg
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      690 2022-01-28 16:16:16.000000 m9s_stock_package_shipping_sale_wizard-6.0.0/COPYRIGHT
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2020-04-22 20:31:44.000000 m9s_stock_package_shipping_sale_wizard-6.0.0/INSTALL
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2020-04-22 20:31:44.000000 m9s_stock_package_shipping_sale_wizard-6.0.0/LICENSE
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      125 2022-02-13 19:23:06.000000 m9s_stock_package_shipping_sale_wizard-6.0.0/MANIFEST.in
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3572 2022-02-14 19:36:24.793872 m9s_stock_package_shipping_sale_wizard-6.0.0/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1385 2020-04-22 22:12:59.000000 m9s_stock_package_shipping_sale_wizard-6.0.0/README.md
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       84 2020-04-22 20:31:44.000000 m9s_stock_package_shipping_sale_wizard-6.0.0/README.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      489 2021-12-11 18:43:11.000000 m9s_stock_package_shipping_sale_wizard-6.0.0/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       77 2022-02-13 19:23:06.000000 m9s_stock_package_shipping_sale_wizard-6.0.0/dev_requirements.txt
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-02-14 19:36:24.793872 m9s_stock_package_shipping_sale_wizard-6.0.0/doc/
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-02-14 19:36:24.793872 m9s_stock_package_shipping_sale_wizard-6.0.0/doc/de/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       83 2020-04-22 20:31:44.000000 m9s_stock_package_shipping_sale_wizard-6.0.0/doc/de/index.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       84 2020-04-22 20:31:44.000000 m9s_stock_package_shipping_sale_wizard-6.0.0/doc/index.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      714 2020-04-22 22:12:59.000000 m9s_stock_package_shipping_sale_wizard-6.0.0/invoice.py
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-02-14 19:36:24.793872 m9s_stock_package_shipping_sale_wizard-6.0.0/locale/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2119 2021-12-11 18:21:36.000000 m9s_stock_package_shipping_sale_wizard-6.0.0/locale/de.po
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-02-14 19:36:24.793872 m9s_stock_package_shipping_sale_wizard-6.0.0/m9s_stock_package_shipping_sale_wizard.egg-info/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3572 2022-02-14 19:36:24.000000 m9s_stock_package_shipping_sale_wizard-6.0.0/m9s_stock_package_shipping_sale_wizard.egg-info/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1018 2022-02-14 19:36:24.000000 m9s_stock_package_shipping_sale_wizard-6.0.0/m9s_stock_package_shipping_sale_wizard.egg-info/SOURCES.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2022-02-14 19:36:24.000000 m9s_stock_package_shipping_sale_wizard-6.0.0/m9s_stock_package_shipping_sale_wizard.egg-info/dependency_links.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      119 2022-02-14 19:36:24.000000 m9s_stock_package_shipping_sale_wizard-6.0.0/m9s_stock_package_shipping_sale_wizard.egg-info/entry_points.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2020-04-22 21:50:33.000000 m9s_stock_package_shipping_sale_wizard-6.0.0/m9s_stock_package_shipping_sale_wizard.egg-info/not-zip-safe
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      202 2022-02-14 19:36:24.000000 m9s_stock_package_shipping_sale_wizard-6.0.0/m9s_stock_package_shipping_sale_wizard.egg-info/requires.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2022-02-14 19:36:24.000000 m9s_stock_package_shipping_sale_wizard-6.0.0/m9s_stock_package_shipping_sale_wizard.egg-info/top_level.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      399 2022-02-14 19:35:29.000000 m9s_stock_package_shipping_sale_wizard-6.0.0/message.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2022-02-13 19:23:06.000000 m9s_stock_package_shipping_sale_wizard-6.0.0/requirements.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       38 2022-02-14 19:36:24.793872 m9s_stock_package_shipping_sale_wizard-6.0.0/setup.cfg
--rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4877 2022-02-14 19:32:36.000000 m9s_stock_package_shipping_sale_wizard-6.0.0/setup.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     8646 2021-12-11 18:43:11.000000 m9s_stock_package_shipping_sale_wizard-6.0.0/stock.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1706 2020-04-22 22:12:59.000000 m9s_stock_package_shipping_sale_wizard-6.0.0/stock.xml
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-02-14 19:36:24.793872 m9s_stock_package_shipping_sale_wizard-6.0.0/tests/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      354 2021-12-11 18:43:11.000000 m9s_stock_package_shipping_sale_wizard-6.0.0/tests/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      583 2021-12-11 18:43:11.000000 m9s_stock_package_shipping_sale_wizard-6.0.0/tests/test_stock_package_shipping_sale_wizard.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      745 2022-02-13 19:23:06.000000 m9s_stock_package_shipping_sale_wizard-6.0.0/tox.ini
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      208 2022-01-28 16:24:08.000000 m9s_stock_package_shipping_sale_wizard-6.0.0/tryton.cfg
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-02-14 19:36:24.793872 m9s_stock_package_shipping_sale_wizard-6.0.0/view/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      562 2020-04-22 22:12:59.000000 m9s_stock_package_shipping_sale_wizard-6.0.0/view/create_shipping_start_form.xml
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:28:43.290006 m9s_stock_package_shipping_sale_wizard-6.0.1/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      104 2022-02-13 19:23:06.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/.coveragerc
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-02-13 19:23:06.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/.drone.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2022-02-13 19:23:06.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/.flake8
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1787 2022-11-13 14:32:56.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/.gitlab-ci.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2022-02-13 19:23:06.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/.isort.cfg
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:28:43.286006 m9s_stock_package_shipping_sale_wizard-6.0.1/.woodpecker/
+-rwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2022-11-23 17:28:52.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/.woodpecker/mail_curl.sh
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2022-11-23 20:42:33.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/.woodpecker/report.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1468 2022-11-24 15:51:07.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/.woodpecker/test.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      690 2022-01-28 16:16:16.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/COPYRIGHT
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2020-04-22 20:31:44.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/INSTALL
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2020-04-22 20:31:44.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/LICENSE
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      125 2022-02-13 19:23:06.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/MANIFEST.in
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3552 2023-05-30 16:28:43.290006 m9s_stock_package_shipping_sale_wizard-6.0.1/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1385 2020-04-22 22:12:59.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/README.md
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       84 2020-04-22 20:31:44.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/README.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      489 2021-12-11 18:43:11.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      121 2023-02-14 11:02:16.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/dev_requirements.txt
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:28:43.286006 m9s_stock_package_shipping_sale_wizard-6.0.1/doc/
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:28:43.286006 m9s_stock_package_shipping_sale_wizard-6.0.1/doc/de/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       83 2020-04-22 20:31:44.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/doc/de/index.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       84 2020-04-22 20:31:44.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/doc/index.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      714 2020-04-22 22:12:59.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/invoice.py
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:28:43.286006 m9s_stock_package_shipping_sale_wizard-6.0.1/locale/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2119 2021-12-11 18:21:36.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/locale/de.po
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:28:43.286006 m9s_stock_package_shipping_sale_wizard-6.0.1/m9s_stock_package_shipping_sale_wizard.egg-info/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3552 2023-05-30 16:28:43.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/m9s_stock_package_shipping_sale_wizard.egg-info/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1087 2023-05-30 16:28:43.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/m9s_stock_package_shipping_sale_wizard.egg-info/SOURCES.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2023-05-30 16:28:43.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/m9s_stock_package_shipping_sale_wizard.egg-info/dependency_links.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2023-05-30 16:28:43.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/m9s_stock_package_shipping_sale_wizard.egg-info/entry_points.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2020-04-22 21:50:33.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/m9s_stock_package_shipping_sale_wizard.egg-info/not-zip-safe
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      202 2023-05-30 16:28:43.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/m9s_stock_package_shipping_sale_wizard.egg-info/requires.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2023-05-30 16:28:43.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/m9s_stock_package_shipping_sale_wizard.egg-info/top_level.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      399 2022-02-14 19:35:29.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/message.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2022-02-13 19:23:06.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/requirements.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       38 2023-05-30 16:28:43.290006 m9s_stock_package_shipping_sale_wizard-6.0.1/setup.cfg
+-rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4877 2022-02-14 19:32:36.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/setup.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     8646 2021-12-11 18:43:11.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/stock.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1706 2020-04-22 22:12:59.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/stock.xml
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:28:43.286006 m9s_stock_package_shipping_sale_wizard-6.0.1/tests/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      354 2021-12-11 18:43:11.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/tests/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      583 2021-12-11 18:43:11.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/tests/test_stock_package_shipping_sale_wizard.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      843 2022-11-24 16:26:27.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/tox.ini
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      208 2023-05-30 16:28:35.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/tryton.cfg
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2023-05-30 16:28:43.286006 m9s_stock_package_shipping_sale_wizard-6.0.1/view/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      562 2020-04-22 22:12:59.000000 m9s_stock_package_shipping_sale_wizard-6.0.1/view/create_shipping_start_form.xml
```

### Comparing `m9s_stock_package_shipping_sale_wizard-6.0.0/.drone.yml` & `m9s_stock_package_shipping_sale_wizard-6.0.1/.drone.yml`

 * *Files identical despite different names*

### Comparing `m9s_stock_package_shipping_sale_wizard-6.0.0/.gitlab-ci.yml` & `m9s_stock_package_shipping_sale_wizard-6.0.1/.gitlab-ci.yml`

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

### Comparing `m9s_stock_package_shipping_sale_wizard-6.0.0/COPYRIGHT` & `m9s_stock_package_shipping_sale_wizard-6.0.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `m9s_stock_package_shipping_sale_wizard-6.0.0/INSTALL` & `m9s_stock_package_shipping_sale_wizard-6.0.1/INSTALL`

 * *Files identical despite different names*

### Comparing `m9s_stock_package_shipping_sale_wizard-6.0.0/LICENSE` & `m9s_stock_package_shipping_sale_wizard-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `m9s_stock_package_shipping_sale_wizard-6.0.0/PKG-INFO` & `m9s_stock_package_shipping_sale_wizard-6.0.1/m9s_stock_package_shipping_sale_wizard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
-Name: m9s_stock_package_shipping_sale_wizard
-Version: 6.0.0
+Name: m9s-stock-package-shipping-sale-wizard
+Version: 6.0.1
 Summary: Tryton Stock Package Shipping Sale Wizard Module
 Home-page: http://www.m9s.biz/
+Download-URL: https://gitlab.com/m9s/stock_package_shipping_sale_wizard.git
 Author: MBSolutions
 Author-email: info@m9s.biz
 License: GPL-3
-Download-URL: https://gitlab.com/m9s/stock_package_shipping_sale_wizard.git
 Project-URL: Bug Tracker, https://support.m9s.biz/
 Project-URL: Source Code, https://gitlab.com/m9s/stock_package_shipping_sale_wizard.git
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

### Comparing `m9s_stock_package_shipping_sale_wizard-6.0.0/README.md` & `m9s_stock_package_shipping_sale_wizard-6.0.1/README.md`

 * *Files identical despite different names*

### Comparing `m9s_stock_package_shipping_sale_wizard-6.0.0/invoice.py` & `m9s_stock_package_shipping_sale_wizard-6.0.1/invoice.py`

 * *Files identical despite different names*

### Comparing `m9s_stock_package_shipping_sale_wizard-6.0.0/locale/de.po` & `m9s_stock_package_shipping_sale_wizard-6.0.1/locale/de.po`

 * *Files identical despite different names*

### Comparing `m9s_stock_package_shipping_sale_wizard-6.0.0/m9s_stock_package_shipping_sale_wizard.egg-info/PKG-INFO` & `m9s_stock_package_shipping_sale_wizard-6.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
-Name: m9s-stock-package-shipping-sale-wizard
-Version: 6.0.0
+Name: m9s_stock_package_shipping_sale_wizard
+Version: 6.0.1
 Summary: Tryton Stock Package Shipping Sale Wizard Module
 Home-page: http://www.m9s.biz/
+Download-URL: https://gitlab.com/m9s/stock_package_shipping_sale_wizard.git
 Author: MBSolutions
 Author-email: info@m9s.biz
 License: GPL-3
-Download-URL: https://gitlab.com/m9s/stock_package_shipping_sale_wizard.git
 Project-URL: Bug Tracker, https://support.m9s.biz/
 Project-URL: Source Code, https://gitlab.com/m9s/stock_package_shipping_sale_wizard.git
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

### Comparing `m9s_stock_package_shipping_sale_wizard-6.0.0/m9s_stock_package_shipping_sale_wizard.egg-info/SOURCES.txt` & `m9s_stock_package_shipping_sale_wizard-6.0.1/m9s_stock_package_shipping_sale_wizard.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 ./stock.py
 ./stock.xml
 ./tryton.cfg
 ./locale/de.po
 ./tests/__init__.py
 ./tests/test_stock_package_shipping_sale_wizard.py
 ./view/create_shipping_start_form.xml
+.woodpecker/mail_curl.sh
+.woodpecker/report.yml
+.woodpecker/test.yml
 doc/index.rst
 doc/de/index.rst
 locale/de.po
 m9s_stock_package_shipping_sale_wizard.egg-info/PKG-INFO
 m9s_stock_package_shipping_sale_wizard.egg-info/SOURCES.txt
 m9s_stock_package_shipping_sale_wizard.egg-info/dependency_links.txt
 m9s_stock_package_shipping_sale_wizard.egg-info/entry_points.txt
```

### Comparing `m9s_stock_package_shipping_sale_wizard-6.0.0/setup.py` & `m9s_stock_package_shipping_sale_wizard-6.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `m9s_stock_package_shipping_sale_wizard-6.0.0/stock.py` & `m9s_stock_package_shipping_sale_wizard-6.0.1/stock.py`

 * *Files identical despite different names*

### Comparing `m9s_stock_package_shipping_sale_wizard-6.0.0/stock.xml` & `m9s_stock_package_shipping_sale_wizard-6.0.1/stock.xml`

 * *Files identical despite different names*

### Comparing `m9s_stock_package_shipping_sale_wizard-6.0.0/tests/test_stock_package_shipping_sale_wizard.py` & `m9s_stock_package_shipping_sale_wizard-6.0.1/tests/test_stock_package_shipping_sale_wizard.py`

 * *Files identical despite different names*

### Comparing `m9s_stock_package_shipping_sale_wizard-6.0.0/view/create_shipping_start_form.xml` & `m9s_stock_package_shipping_sale_wizard-6.0.1/view/create_shipping_start_form.xml`

 * *Files identical despite different names*

