# Comparing `tmp/oopgrade-0.8.0.tar.gz` & `tmp/oopgrade-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/oopgrade-0.8.0.tar", last modified: Fri May 28 12:18:59 2021, max compression
+gzip compressed data, was "dist/oopgrade-0.9.0.tar", last modified: Wed Sep 14 07:24:44 2022, max compression
```

## Comparing `oopgrade-0.8.0.tar` & `oopgrade-0.9.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2021-05-28 12:18:59.000000 oopgrade-0.8.0/
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      744 2021-05-28 12:18:52.000000 oopgrade-0.8.0/setup.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       38 2021-05-28 12:18:59.000000 oopgrade-0.8.0/setup.cfg
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2021-05-28 12:18:59.000000 oopgrade-0.8.0/spec/
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     7301 2020-12-27 20:37:17.000000 oopgrade-0.8.0/spec/data_migration_spec.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        0 2020-12-27 20:37:17.000000 oopgrade-0.8.0/spec/__init__.py
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2021-05-28 12:18:59.000000 oopgrade-0.8.0/spec/fixtures/
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      142 2020-12-27 20:37:17.000000 oopgrade-0.8.0/spec/fixtures/__init__.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2065 2020-12-27 20:37:17.000000 oopgrade-0.8.0/spec/version_spec.py
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2021-05-28 12:18:59.000000 oopgrade-0.8.0/oopgrade/
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     1079 2021-05-28 12:18:52.000000 oopgrade-0.8.0/oopgrade/cli.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     5541 2020-12-27 20:37:17.000000 oopgrade-0.8.0/oopgrade/data.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2385 2021-05-28 12:18:52.000000 oopgrade-0.8.0/oopgrade/utils.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      221 2021-05-28 12:18:52.000000 oopgrade-0.8.0/oopgrade/__init__.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2283 2020-12-27 20:37:17.000000 oopgrade-0.8.0/oopgrade/log.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     1941 2021-05-28 12:18:46.000000 oopgrade-0.8.0/oopgrade/version.py
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)    15857 2021-05-28 12:18:52.000000 oopgrade-0.8.0/oopgrade/oopgrade.py
-drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2021-05-28 12:18:59.000000 oopgrade-0.8.0/oopgrade.egg-info/
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       14 2021-05-28 12:18:59.000000 oopgrade-0.8.0/oopgrade.egg-info/top_level.txt
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       66 2021-05-28 12:18:59.000000 oopgrade-0.8.0/oopgrade.egg-info/entry_points.txt
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       46 2021-05-28 12:18:59.000000 oopgrade-0.8.0/oopgrade.egg-info/requires.txt
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      434 2021-05-28 12:18:59.000000 oopgrade-0.8.0/oopgrade.egg-info/SOURCES.txt
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        1 2021-05-28 12:18:59.000000 oopgrade-0.8.0/oopgrade.egg-info/dependency_links.txt
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      870 2021-05-28 12:18:59.000000 oopgrade-0.8.0/oopgrade.egg-info/PKG-INFO
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      523 2020-12-27 20:37:17.000000 oopgrade-0.8.0/README.rst
--rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      870 2021-05-28 12:18:59.000000 oopgrade-0.8.0/PKG-INFO
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2022-09-14 07:24:44.000000 oopgrade-0.9.0/
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      763 2022-09-14 07:24:15.000000 oopgrade-0.9.0/setup.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       38 2022-09-14 07:24:44.000000 oopgrade-0.9.0/setup.cfg
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2022-09-14 07:24:44.000000 oopgrade-0.9.0/spec/
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     7301 2021-11-29 09:56:15.000000 oopgrade-0.9.0/spec/data_migration_spec.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        0 2021-11-29 09:56:15.000000 oopgrade-0.9.0/spec/__init__.py
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2022-09-14 07:24:44.000000 oopgrade-0.9.0/spec/fixtures/
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      142 2021-11-29 09:56:15.000000 oopgrade-0.9.0/spec/fixtures/__init__.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2065 2020-12-27 20:37:17.000000 oopgrade-0.9.0/spec/version_spec.py
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2022-09-14 07:24:44.000000 oopgrade-0.9.0/oopgrade/
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     1273 2022-09-14 07:24:05.000000 oopgrade-0.9.0/oopgrade/cli.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     5541 2021-11-29 09:56:15.000000 oopgrade-0.9.0/oopgrade/data.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2385 2022-09-14 07:06:06.000000 oopgrade-0.9.0/oopgrade/utils.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      221 2021-11-29 09:56:15.000000 oopgrade-0.9.0/oopgrade/__init__.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     2283 2020-12-27 20:37:17.000000 oopgrade-0.9.0/oopgrade/log.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)     1941 2021-11-04 10:24:34.000000 oopgrade-0.9.0/oopgrade/version.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        0 2022-07-11 14:35:25.000000 oopgrade-0.9.0/oopgrade/modules.py
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)    15857 2021-11-29 09:56:15.000000 oopgrade-0.9.0/oopgrade/oopgrade.py
+drwxrwxr-x   0 ecarreras  (1000) ecarreras  (1000)        0 2022-09-14 07:24:44.000000 oopgrade-0.9.0/oopgrade.egg-info/
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       14 2022-09-14 07:24:44.000000 oopgrade-0.9.0/oopgrade.egg-info/top_level.txt
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       66 2022-09-14 07:24:44.000000 oopgrade-0.9.0/oopgrade.egg-info/entry_points.txt
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)       53 2022-09-14 07:24:44.000000 oopgrade-0.9.0/oopgrade.egg-info/requires.txt
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      454 2022-09-14 07:24:44.000000 oopgrade-0.9.0/oopgrade.egg-info/SOURCES.txt
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)        1 2022-09-14 07:24:44.000000 oopgrade-0.9.0/oopgrade.egg-info/dependency_links.txt
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      870 2022-09-14 07:24:44.000000 oopgrade-0.9.0/oopgrade.egg-info/PKG-INFO
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      523 2021-11-29 09:56:15.000000 oopgrade-0.9.0/README.rst
+-rw-rw-r--   0 ecarreras  (1000) ecarreras  (1000)      870 2022-09-14 07:24:44.000000 oopgrade-0.9.0/PKG-INFO
```

### Comparing `oopgrade-0.8.0/setup.py` & `oopgrade-0.9.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,29 +8,30 @@
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 dirname = os.path.dirname(__file__)
 
 setup(
     name='oopgrade',
-    version='0.8.0',
+    version='0.9.0',
     description='Upgrade and migration tools',
     long_description=readme,
     author='GISCE-TI, S.L.',
     author_email='devel@gisce.net',
     url='https://github.com/gisce/oopgrade',
     packages=find_packages(),
     install_requires=[
         'ooquery',
         'semver',
         'lxml',
         'python-sql',
         'tqdm',
         'click',
-        'pip'
+        'pip',
+        'osconf',
     ],
     license='AGPL-3',
     entry_points='''
       [console_scripts]
       oopgrade=oopgrade.cli:oopgrade
     '''
 )
```

### Comparing `oopgrade-0.8.0/spec/data_migration_spec.py` & `oopgrade-0.9.0/spec/data_migration_spec.py`

 * *Files identical despite different names*

### Comparing `oopgrade-0.8.0/spec/version_spec.py` & `oopgrade-0.9.0/spec/version_spec.py`

 * *Files identical despite different names*

### Comparing `oopgrade-0.8.0/oopgrade/cli.py` & `oopgrade-0.9.0/oopgrade/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 # coding=utf-8
 from __future__ import absolute_import
 import click
 from tqdm import tqdm
 import psycopg2
 import ConfigParser
+from osconf import config_from_environment
 
 
 @click.group()
-@click.option('--config')
+@click.option('--config', required=False, default=None)
 @click.pass_context
 def oopgrade(ctx, config):
-    conf = ConfigParser.ConfigParser()
-    conf.read(config)
-    ctx.obj = dict(conf.items('options'))
+    ctx.obj = {}
+    if config:
+        conf = ConfigParser.ConfigParser()
+        conf.read(config)
+        ctx.obj = dict(conf.items('options'))
+    envconf = config_from_environment('OPENERP')
+    ctx.obj.update(envconf)
 
 
 @oopgrade.group()
 def requirements():
     pass
```

### Comparing `oopgrade-0.8.0/oopgrade/data.py` & `oopgrade-0.9.0/oopgrade/data.py`

 * *Files identical despite different names*

### Comparing `oopgrade-0.8.0/oopgrade/utils.py` & `oopgrade-0.9.0/oopgrade/utils.py`

 * *Files identical despite different names*

### Comparing `oopgrade-0.8.0/oopgrade/log.py` & `oopgrade-0.9.0/oopgrade/log.py`

 * *Files identical despite different names*

### Comparing `oopgrade-0.8.0/oopgrade/version.py` & `oopgrade-0.9.0/oopgrade/version.py`

 * *Files identical despite different names*

### Comparing `oopgrade-0.8.0/oopgrade/oopgrade.py` & `oopgrade-0.9.0/oopgrade/oopgrade.py`

 * *Files identical despite different names*

### Comparing `oopgrade-0.8.0/oopgrade.egg-info/PKG-INFO` & `oopgrade-0.9.0/oopgrade.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: oopgrade
-Version: 0.8.0
+Version: 0.9.0
 Summary: Upgrade and migration tools
 Home-page: https://github.com/gisce/oopgrade
 Author: GISCE-TI, S.L.
 Author-email: devel@gisce.net
 License: AGPL-3
 Description: OOpgrade
         ========
```

### Comparing `oopgrade-0.8.0/README.rst` & `oopgrade-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `oopgrade-0.8.0/PKG-INFO` & `oopgrade-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: oopgrade
-Version: 0.8.0
+Version: 0.9.0
 Summary: Upgrade and migration tools
 Home-page: https://github.com/gisce/oopgrade
 Author: GISCE-TI, S.L.
 Author-email: devel@gisce.net
 License: AGPL-3
 Description: OOpgrade
         ========
```

