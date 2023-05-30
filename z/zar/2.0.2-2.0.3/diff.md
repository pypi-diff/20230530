# Comparing `tmp/zar-2.0.2.tar.gz` & `tmp/zar-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zar-2.0.2.tar", last modified: Thu May 25 08:54:11 2023, max compression
+gzip compressed data, was "dist/zar-2.0.3.tar", last modified: Tue May 30 10:34:27 2023, max compression
```

## Comparing `zar-2.0.2.tar` & `zar-2.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:54:11.000000 zar-2.0.2/
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:54:11.000000 zar-2.0.2/zar/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 zar-2.0.2/zar/__main__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)       46 2022-12-09 05:08:44.000000 zar-2.0.2/zar/__init__.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-25 08:54:11.000000 zar-2.0.2/zar.egg-info/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        4 2023-05-25 08:54:11.000000 zar-2.0.2/zar.egg-info/top_level.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-05-25 08:54:11.000000 zar-2.0.2/zar.egg-info/dependency_links.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 09:05:11.000000 zar-2.0.2/zar.egg-info/not-zip-safe
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      185 2023-05-25 08:54:11.000000 zar-2.0.2/zar.egg-info/SOURCES.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1250 2023-05-25 08:54:11.000000 zar-2.0.2/zar.egg-info/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-05-25 08:54:11.000000 zar-2.0.2/setup.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1359 2023-05-20 08:03:42.000000 zar-2.0.2/setup.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1250 2023-05-25 08:54:11.000000 zar-2.0.2/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     5707 2023-05-21 13:34:30.000000 zar-2.0.2/README.rst
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-30 10:34:27.000000 zar-2.0.3/
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-30 10:34:27.000000 zar-2.0.3/zar/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 zar-2.0.3/zar/__main__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)       46 2022-12-09 05:08:44.000000 zar-2.0.3/zar/__init__.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-30 10:34:27.000000 zar-2.0.3/zar.egg-info/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        4 2023-05-30 10:34:27.000000 zar-2.0.3/zar.egg-info/top_level.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-05-30 10:34:27.000000 zar-2.0.3/zar.egg-info/dependency_links.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 09:05:11.000000 zar-2.0.3/zar.egg-info/not-zip-safe
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      185 2023-05-30 10:34:27.000000 zar-2.0.3/zar.egg-info/SOURCES.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1250 2023-05-30 10:34:27.000000 zar-2.0.3/zar.egg-info/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-05-30 10:34:27.000000 zar-2.0.3/setup.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1359 2023-05-30 10:34:05.000000 zar-2.0.3/setup.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1250 2023-05-30 10:34:27.000000 zar-2.0.3/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6659 2023-05-21 05:46:49.000000 zar-2.0.3/README.rst
```

### Comparing `zar-2.0.2/zar.egg-info/PKG-INFO` & `zar-2.0.3/zar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: zar
-Version: 2.0.2
+Version: 2.0.3
 Summary: Zeroincombenze Archive Replica
 Home-page: UNKNOWN
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
 Project-URL: Source, https://github.com/zeroincombenze/tools
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
```

### Comparing `zar-2.0.2/setup.py` & `zar-2.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup
 
 setup(
     name='zar',
-    version='2.0.2',
+    version='2.0.3',
     description='Zeroincombenze Archive Replica',
     long_description="""
 ZAR stand for Zeroincombenze® Archive Replica.
 It is a tool kit to backup, restore, replicate files and/or database.
 
 ZAR manages easily backup for Odoo database, keeps last nth copies and purges oldest copies.
 """,
```

### Comparing `zar-2.0.2/PKG-INFO` & `zar-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: zar
-Version: 2.0.2
+Version: 2.0.3
 Summary: Zeroincombenze Archive Replica
 Home-page: UNKNOWN
 Author: Antonio Maria Vigliotti
 Author-email: antoniomaria.vigliotti@gmail.com
 License: Affero GPL
 Project-URL: Source, https://github.com/zeroincombenze/tools
 Project-URL: Documentation, https://zeroincombenze-tools.readthedocs.io
```

### Comparing `zar-2.0.2/README.rst` & `zar-2.0.3/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,29 @@
 
 =========
 zar 2.0.2
 =========
 
 
 
-|Maturity| |license gpl|
+|Maturity| |Build Status| |Coverage Status| |license gpl|
+
+
+
+
+Overview
+========
+
+=========
+zar 2.0.2
+=========
+
+
+
+|Maturity| |Build Status| |Coverage Status| |license gpl|
 
 
 
 
 Overview
 ========
 
@@ -38,96 +52,86 @@
 * automatic purging of oldest copies
 * configuration based on host name: it works on duplicate host image too
 * backup on same host or on remote host
 
 
 |
 
-Usage
-=====
 
-zar should be execute by postgres user
 
-Execute zar_upd to install and configure.
-Configuration file is zar.conf
-Execute zar_bck to do backup or restore, based on host role
-Execute zar_rest to do restore
-
-To execute in cron, use zar_bck -k
-
-
-There are avaiable two postgresql facilities:
-
-* pg_db_active
-* pg_db_reassign owner
-
-`pg_db_active` show and kill postgres session. It can kill oldest session out of pool.
+|
 
-`pg_db_reassign_owner` can reassign owner to database. It reassign the ownership of all objects.
+Features
+--------
 
+* backup and restore odoo database
+* backup and restore based on rules by configuration file
+* restore database with automatic actions disabled
+* multiple copies of database by configuration file
+* automatic purging of oldest copies
+* configuration based on host name: it works on duplicate host image too
+* backup on same host or on remote host
 
 |
 |
 
 Getting started
 ===============
 
 
-For stable version:
-
-`pip install zar`
-
-For current version:
+Installation
+------------
 
-`cd $HOME`
-`git@github.com:zeroincombenze/tools.git`
-`cd $HOME/tools`
-`./install_tools.sh`
+Zeroincombenze tools require:
 
-
-Upgrade
--------
+* Linux Centos 7/8 or Debian 9/10 or Ubuntu 18/20/22
+* python 2.7+, some tools require python 3.6+
+* bash 5.0+
 
 Stable version via Python Package
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 ::
 
-    pip install zar -U
+    pip install zar
 
 |
 
 Current version via Git
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 ::
 
     cd $HOME
-    ./install_tools.sh -U
+    git clone https://github.com/zeroincombenze/tools.git
+    cd ./tools
+    ./install_tools.sh -p
     source $HOME/devel/activate_tools
 
 
-History
+Upgrade
 -------
 
-2.0.2 (2023-05-14)
-~~~~~~~~~~~~~~~~~~
+Stable version via Python Package
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-* [IMP] reassing_owner accept db_port
+::
 
-2.0.1 (2023-02-25)
-~~~~~~~~~~~~~~~~~~
+    pip install zar -U
 
-* [IMP] Remote bckdir different from local
+|
 
-2.0.0 (2022-10-20)
-~~~~~~~~~~~~~~~~~~
+Current version via Git
+~~~~~~~~~~~~~~~~~~~~~~~
 
-* [IMP] Stable version
+::
 
+    cd $HOME
+    ./install_tools.sh -U
+    source $HOME/devel/activate_tools
 
 
 |
 |
 
 Credits
 =======
@@ -138,44 +142,59 @@
 SHS-AV s.r.l. <https://www.shs-av.com/>
 
 
 Contributors
 ------------
 
 * Antonio M. Vigliotti <info@shs-av.com>
-* Antonio Maria Vigliotti <antoniomaria.vigliotti@gmail.com>
 Contributors
 ------------
 
+* Antonio Maria Vigliotti <antoniomaria.vigliotti@gmail.com>
 
 
 |
 
 This module is part of tools project.
 
 Last Update / Ultimo aggiornamento: 2023-05-21
 
 .. |Maturity| image:: https://img.shields.io/badge/maturity-Alfa-black.png
     :target: https://odoo-community.org/page/development-status
     :alt: 
+.. |Build Status| image:: https://travis-ci.org/zeroincombenze/tools.svg?branch=master
+    :target: https://travis-ci.com/zeroincombenze/tools
+    :alt: github.com
 .. |license gpl| image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
     :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
     :alt: License: AGPL-3
 .. |license opl| image:: https://img.shields.io/badge/licence-OPL-7379c3.svg
     :target: https://www.odoo.com/documentation/user/9.0/legal/licenses/licenses.html
     :alt: License: OPL
+.. |Coverage Status| image:: https://coveralls.io/repos/github/zeroincombenze/tools/badge.svg?branch=master
+    :target: https://coveralls.io/github/zeroincombenze/tools?branch=2.0
+    :alt: Coverage
+.. |Codecov Status| image:: https://codecov.io/gh/zeroincombenze/tools/branch/2.0/graph/badge.svg
+    :target: https://codecov.io/gh/zeroincombenze/tools/branch/2.0
+    :alt: Codecov
 .. |Tech Doc| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-docs-2.svg
     :target: https://wiki.zeroincombenze.org/en/Odoo/2.0/dev
     :alt: Technical Documentation
 .. |Help| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-help-2.svg
     :target: https://wiki.zeroincombenze.org/it/Odoo/2.0/man
     :alt: Technical Documentation
 .. |Try Me| image:: https://www.zeroincombenze.it/wp-content/uploads/ci-ct/prd/button-try-it-2.svg
     :target: https://erp2.zeroincombenze.it
     :alt: Try Me
+.. |OCA Codecov| image:: https://codecov.io/gh/OCA/tools/branch/2.0/graph/badge.svg
+    :target: https://codecov.io/gh/OCA/tools/branch/2.0
+    :alt: Codecov
+.. |Odoo Italia Associazione| image:: https://www.odoo-italia.org/images/Immagini/Odoo%20Italia%20-%20126x56.png
+   :target: https://odoo-italia.org
+   :alt: Odoo Italia Associazione
 .. |Zeroincombenze| image:: https://avatars0.githubusercontent.com/u/6972555?s=460&v=4
    :target: https://www.zeroincombenze.it/
    :alt: Zeroincombenze
 .. |en| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/flags/en_US.png
    :target: https://www.facebook.com/Zeroincombenze-Software-gestionale-online-249494305219415/
 .. |it| image:: https://raw.githubusercontent.com/zeroincombenze/grymb/master/flags/it_IT.png
    :target: https://www.facebook.com/Zeroincombenze-Software-gestionale-online-249494305219415/
```

