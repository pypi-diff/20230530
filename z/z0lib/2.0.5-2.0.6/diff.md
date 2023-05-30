# Comparing `tmp/z0lib-2.0.5.tar.gz` & `tmp/z0lib-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/z0lib-2.0.5.tar", last modified: Mon May 22 08:42:42 2023, max compression
+gzip compressed data, was "dist/z0lib-2.0.6.tar", last modified: Tue May 30 10:35:37 2023, max compression
```

## Comparing `z0lib-2.0.5.tar` & `z0lib-2.0.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-22 08:42:42.000000 z0lib-2.0.5/
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-22 08:42:42.000000 z0lib-2.0.5/z0lib/
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 z0lib-2.0.5/z0lib/__main__.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-22 08:42:42.000000 z0lib-2.0.5/z0lib/tests/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     4853 2023-05-20 08:02:42.000000 z0lib-2.0.5/z0lib/tests/test_runtraced.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1269 2022-12-09 05:08:44.000000 z0lib-2.0.5/z0lib/tests/tmp.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      718 2022-12-09 05:08:44.000000 z0lib-2.0.5/z0lib/tests/tmp1.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3744 2023-05-20 08:02:43.000000 z0lib-2.0.5/z0lib/tests/test_z0lib.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       24 2022-12-09 05:08:44.000000 z0lib-2.0.5/z0lib/tests/__init__.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-22 08:42:42.000000 z0lib-2.0.5/z0lib/scripts/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1952 2023-05-20 08:36:29.000000 z0lib-2.0.5/z0lib/scripts/setup.info
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6801 2023-05-20 08:02:43.000000 z0lib-2.0.5/z0lib/scripts/main.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       43 2022-12-09 05:08:44.000000 z0lib-2.0.5/z0lib/scripts/__init__.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4039 2023-05-20 08:02:46.000000 z0lib-2.0.5/z0lib/xuname
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    57347 2023-05-20 08:02:46.000000 z0lib-2.0.5/z0lib/z0librc
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      106 2022-12-09 05:08:44.000000 z0lib-2.0.5/z0lib/explore_env.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4920 2023-05-20 08:02:46.000000 z0lib-2.0.5/z0lib/optargs
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)    20883 2023-05-20 08:02:46.000000 z0lib-2.0.5/z0lib/z0librun.py
--rwxrwxr-x   0 odoo      (1000) odoo      (1000)      148 2022-12-09 05:08:44.000000 z0lib-2.0.5/z0lib/__init__.py
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-05-22 08:42:42.000000 z0lib-2.0.5/setup.cfg
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     1650 2023-05-22 07:11:35.000000 z0lib-2.0.5/setup.py
-drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-22 08:42:42.000000 z0lib-2.0.5/z0lib.egg-info/
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        6 2023-05-22 08:42:42.000000 z0lib-2.0.5/z0lib.egg-info/top_level.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-05-22 08:42:42.000000 z0lib-2.0.5/z0lib.egg-info/dependency_links.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 08:08:41.000000 z0lib-2.0.5/z0lib.egg-info/not-zip-safe
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       56 2023-05-22 08:42:42.000000 z0lib-2.0.5/z0lib.egg-info/entry_points.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)      531 2023-05-22 08:42:42.000000 z0lib-2.0.5/z0lib.egg-info/SOURCES.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)       20 2023-05-22 08:42:42.000000 z0lib-2.0.5/z0lib.egg-info/requires.txt
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     9282 2023-05-22 08:42:42.000000 z0lib-2.0.5/z0lib.egg-info/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     9282 2023-05-22 08:42:42.000000 z0lib-2.0.5/PKG-INFO
--rw-rw-r--   0 odoo      (1000) odoo      (1000)     6379 2023-05-22 08:37:43.000000 z0lib-2.0.5/README.rst
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-30 10:35:37.000000 z0lib-2.0.6/
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-30 10:35:37.000000 z0lib-2.0.6/z0lib/
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      164 2022-12-09 05:08:44.000000 z0lib-2.0.6/z0lib/__main__.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-30 10:35:37.000000 z0lib-2.0.6/z0lib/tests/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     4853 2023-05-30 10:35:22.000000 z0lib-2.0.6/z0lib/tests/test_runtraced.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1269 2022-12-09 05:08:44.000000 z0lib-2.0.6/z0lib/tests/tmp.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      718 2022-12-09 05:08:44.000000 z0lib-2.0.6/z0lib/tests/tmp1.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     3744 2023-05-30 10:35:22.000000 z0lib-2.0.6/z0lib/tests/test_z0lib.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       24 2022-12-09 05:08:44.000000 z0lib-2.0.6/z0lib/tests/__init__.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-30 10:35:37.000000 z0lib-2.0.6/z0lib/scripts/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1650 2023-05-30 10:35:30.000000 z0lib-2.0.6/z0lib/scripts/setup.info
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6801 2023-05-30 10:35:22.000000 z0lib-2.0.6/z0lib/scripts/main.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       43 2022-12-09 05:08:44.000000 z0lib-2.0.6/z0lib/scripts/__init__.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4039 2023-05-30 10:35:22.000000 z0lib-2.0.6/z0lib/xuname
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    57347 2023-05-30 10:35:22.000000 z0lib-2.0.6/z0lib/z0librc
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      106 2022-12-09 05:08:44.000000 z0lib-2.0.6/z0lib/explore_env.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)     4920 2023-05-30 10:35:22.000000 z0lib-2.0.6/z0lib/optargs
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)    20883 2023-05-30 10:35:22.000000 z0lib-2.0.6/z0lib/z0librun.py
+-rwxrwxr-x   0 odoo      (1000) odoo      (1000)      148 2022-12-09 05:08:44.000000 z0lib-2.0.6/z0lib/__init__.py
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       38 2023-05-30 10:35:37.000000 z0lib-2.0.6/setup.cfg
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     1650 2023-05-30 10:35:22.000000 z0lib-2.0.6/setup.py
+drwxrwxr-x   0 odoo      (1000) odoo      (1000)        0 2023-05-30 10:35:37.000000 z0lib-2.0.6/z0lib.egg-info/
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        6 2023-05-30 10:35:37.000000 z0lib-2.0.6/z0lib.egg-info/top_level.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2023-05-30 10:35:37.000000 z0lib-2.0.6/z0lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)        1 2022-12-09 08:08:41.000000 z0lib-2.0.6/z0lib.egg-info/not-zip-safe
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       56 2023-05-30 10:35:37.000000 z0lib-2.0.6/z0lib.egg-info/entry_points.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)      531 2023-05-30 10:35:37.000000 z0lib-2.0.6/z0lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)       20 2023-05-30 10:35:37.000000 z0lib-2.0.6/z0lib.egg-info/requires.txt
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     9282 2023-05-30 10:35:37.000000 z0lib-2.0.6/z0lib.egg-info/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     9282 2023-05-30 10:35:37.000000 z0lib-2.0.6/PKG-INFO
+-rw-rw-r--   0 odoo      (1000) odoo      (1000)     6379 2023-05-30 10:35:28.000000 z0lib-2.0.6/README.rst
```

### Comparing `z0lib-2.0.5/z0lib/tests/test_runtraced.py` & `z0lib-2.0.6/z0lib/tests/test_runtraced.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 from __future__ import print_function, unicode_literals
 import os
 import sys
 from zerobug import z0test
 from z0lib import z0lib
 
-__version__ = "2.0.5"
+__version__ = "2.0.6"
 
 MODULE_ID = 'z0lib'
 TEST_FAILED = 1
 TEST_SUCCESS = 0
 
 
 def version():
```

### Comparing `z0lib-2.0.5/z0lib/tests/tmp.py` & `z0lib-2.0.6/z0lib/tests/tmp.py`

 * *Files identical despite different names*

### Comparing `z0lib-2.0.5/z0lib/tests/tmp1.py` & `z0lib-2.0.6/z0lib/tests/tmp1.py`

 * *Files identical despite different names*

### Comparing `z0lib-2.0.5/z0lib/tests/test_z0lib.py` & `z0lib-2.0.6/z0lib/tests/test_z0lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # import pdb
 import os
 
 # import sys
 # from zerobug import Z0test
 from z0lib import z0lib
 
-__version__ = "2.0.5"
+__version__ = "2.0.6"
 
 MODULE_ID = 'z0lib'
 TEST_FAILED = 1
 TEST_SUCCESS = 0
 
 
 def version():
```

### Comparing `z0lib-2.0.5/z0lib/scripts/setup.info` & `z0lib-2.0.6/z0lib/scripts/setup.info`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,54 @@
 from setuptools import find_packages, setup
 
+author = "Antonio Maria Vigliotti"
+author_email = "<info@shs-av.com>"
+source_url = "https://github.com/zeroincombenze/tools"
+doc_url = "https://github.com/zeroincombenze/tools"
+changelog_url = "%s/blob/master/z0lib/egg-info/CHANGELOG.rst" % source_url
+
+
 setup(
-    name='z0lib',
-    version='2.0.5',
-    description='Bash zeroincombenze lib',
-    long_description="""
-General purpose bash and python library for zeroincombenze(R) tools
-
-Features:
-
-* xuname: unix/linux platform recognizer (tested on various environments)
-* parseoptargs: line command parser; expands python argparse and adds same functionalities to bash scripts
-* tracelog: manage tracelog (only bash)
-* findpkg: find package in file system (only bash)
-* run_traced: execute (or dry_run) shell command (only bash)
-* CFG: local dictionary values from config file like python ConfigParser (only bash)
-""",
+    name="z0lib",
+    version="2.0.6",
+    description="Bash zeroincombenze lib",
+    long_description=open("README.rst").read(),
     classifiers=[
-        'Development Status :: 4 - Beta',
-        'License :: OSI Approved :: GNU Affero General Public License v3',
-        'Operating System :: POSIX',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Intended Audience :: Developers',
-        'Topic :: Software Development',
-        'Topic :: Software Development :: Libraries',
-        'Topic :: System :: System Shells',
+        "Development Status :: 4 - Beta",
+        "License :: OSI Approved :: GNU Affero General Public License v3",
+        "Operating System :: POSIX",
+        "Programming Language :: Python :: 2.7",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Intended Audience :: Developers",
+        "Topic :: Software Development",
+        "Topic :: Software Development :: Libraries",
+        "Topic :: System :: System Shells",
     ],
-    keywords='bash, optargs',
-    url='https://zeroincombenze-tools.readthedocs.io',
+    keywords="bash, optargs",
+    url="https://zeroincombenze-tools.readthedocs.io",
     project_urls={
-        'Documentation': 'https://zeroincombenze-tools.readthedocs.io',
-        'Source': 'https://github.com/zeroincombenze/tools',
+        "Documentation": doc_url,
+        "Source": source_url,
+        "Changelog": changelog_url,
     },
-    author='Antonio Maria Vigliotti',
-    author_email='antoniomaria.vigliotti@gmail.com',
-    license='Affero GPL',
-    install_requires=['configparser', 'future'],
-    packages=find_packages(exclude=['docs', 'examples', 'tests', 'egg-info', 'junk']),
-    package_data={'': ['scripts/setup.info', './optargs', './xuname', './z0librc']},
-    entry_points={'console_scripts': ['z0lib-info = z0lib.scripts.main:main']},
+    author=author,
+    author_email=author_email,
+    license="Affero GPL",
+    install_requires=["configparser", "future"],
+    packages=find_packages(exclude=["docs", "examples", "tests", "junk"]),
+    package_data={"": ["scripts/setup.info", "./optargs", "./xuname", "./z0librc"]},
+    entry_points={"console_scripts": ["z0lib-info = z0lib.scripts.main:main"]},
     zip_safe=False,
 )
+
+
+
+
+
+
+
+
+
+
```

### Comparing `z0lib-2.0.5/z0lib/scripts/main.py` & `z0lib-2.0.6/z0lib/scripts/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import os
 import sys
 import pkg_resources
 import gzip
 import shutil
 
 
-__version__ = "2.0.5"
+__version__ = "2.0.6"
 
 
 def fake_setup(**kwargs):
     globals()["setup_args"] = kwargs
 
 
 def read_setup():
```

### Comparing `z0lib-2.0.5/z0lib/xuname` & `z0lib-2.0.6/z0lib/xuname`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.5
+__version__=2.0.6
 
 
 # Main program
 OPTOPTS=(h        a       c       d       f        i       k       m       p       r       s       v       V           x)
 OPTDEST=(opt_help opt_prm opt_prm opt_prm opt_prm  opt_prm opt_prm opt_prm opt_prm opt_prm opt_prm opt_prm opt_version opt_prm)
 OPTACTI=("+"      "*>"    "*>"    "*>"    "*>"     "*>"    "*>"    "*>"    "*>"    "*>"    "*>"    "*>"    "*>"        "*>")
 OPTDEFL=(1        ""      ""      ""      ""       ""      ""      ""      ""      ""      ""      ""      ""          "")
```

### Comparing `z0lib-2.0.5/z0lib/z0librc` & `z0lib-2.0.6/z0lib/z0librc`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) SHS-AV s.r.l. (<http://ww.zeroincombenze.it>)
 # This software is free software under GNU Affero GPL3
 # Bash general purpose library
-#__version__=2.0.5
+#__version__=2.0.6
 [ $BASH_VERSINFO -lt 4 ] && echo "This script $0 requires bash 4.0+!" && exit 4
 [ "${BASH_SOURCE-}" == "$0" ] && echo "You must source this script: \$ source $0" >&2 && exit 33
 STS_FAILED=1
 STS_SUCCESS=0
 
 ##############################################################################
 # Install this lib file in /etc if version is more recent
```

### Comparing `z0lib-2.0.5/z0lib/optargs` & `z0lib-2.0.6/z0lib/optargs`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 link_cfg $DIST_CONF $TCONF
 [[ $TRAVIS_DEBUG_MODE -ge 8 ]] && echo "DIST_CONF=$DIST_CONF" && echo "TCONF=$TCONF"
 get_pypi_param ALL
 RED="\e[1;31m"
 GREEN="\e[1;32m"
 CLR="\e[0m"
 
-__version__=2.0.5
+__version__=2.0.6
 
 if [ "$OPTARGS_TEST_1_2" ]; then
   test_1_2=$OPTARGS_TEST_1_2
 else
   test_1_2=1
 fi
 if [ $test_1_2 -eq 1 ]; then
```

### Comparing `z0lib-2.0.5/z0lib/z0librun.py` & `z0lib-2.0.6/z0lib/z0librun.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     "/etc/openerp-server.conf",
     "/etc/odoo/openerp-server.conf",
     "/etc/openerp/odoo-server.conf",
 ]
 # Read Odoo configuration file (False or /etc/openerp-server.conf)
 OE_CONF = False
 DEFDCT = {}
-__version__ = "2.0.5"
+__version__ = "2.0.6"
 
 
 def nakedname(path):
     return os.path.splitext(os.path.basename(path))[0]
 
 
 def run_traced(cmd, verbose=None, dry_run=None, disable_alias=None, is_alias=None):
```

### Comparing `z0lib-2.0.5/setup.py` & `z0lib-2.0.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 source_url = "https://github.com/zeroincombenze/tools"
 doc_url = "https://github.com/zeroincombenze/tools"
 changelog_url = "%s/blob/master/z0lib/egg-info/CHANGELOG.rst" % source_url
 
 
 setup(
     name="z0lib",
-    version="2.0.5",
+    version="2.0.6",
     description="Bash zeroincombenze lib",
     long_description=open("README.rst").read(),
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 2.7",
```

### Comparing `z0lib-2.0.5/z0lib.egg-info/SOURCES.txt` & `z0lib-2.0.6/z0lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `z0lib-2.0.5/z0lib.egg-info/PKG-INFO` & `z0lib-2.0.6/z0lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 1.2
 Name: z0lib
-Version: 2.0.5
+Version: 2.0.6
 Summary: Bash zeroincombenze lib
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: <info@shs-av.com>
 License: Affero GPL
 Project-URL: Source, https://github.com/zeroincombenze/tools
 Project-URL: Documentation, https://github.com/zeroincombenze/tools
 Project-URL: Changelog, https://github.com/zeroincombenze/tools/blob/master/z0lib/egg-info/CHANGELOG.rst
 Description: 
         ======
-         2.0.5
+         2.0.6
         ======
         
         
         
         |Maturity| |license gpl|
```

### Comparing `z0lib-2.0.5/PKG-INFO` & `z0lib-2.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 1.2
 Name: z0lib
-Version: 2.0.5
+Version: 2.0.6
 Summary: Bash zeroincombenze lib
 Home-page: https://zeroincombenze-tools.readthedocs.io
 Author: Antonio Maria Vigliotti
 Author-email: <info@shs-av.com>
 License: Affero GPL
 Project-URL: Source, https://github.com/zeroincombenze/tools
 Project-URL: Documentation, https://github.com/zeroincombenze/tools
 Project-URL: Changelog, https://github.com/zeroincombenze/tools/blob/master/z0lib/egg-info/CHANGELOG.rst
 Description: 
         ======
-         2.0.5
+         2.0.6
         ======
         
         
         
         |Maturity| |license gpl|
```

### Comparing `z0lib-2.0.5/README.rst` & `z0lib-2.0.6/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 ======
- 2.0.5
+ 2.0.6
 ======
 
 
 
 |Maturity| |license gpl|
```

