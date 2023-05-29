# Comparing `tmp/Hunabku_scienti-0.0.4.tar.gz` & `tmp/Hunabku_scienti-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Hunabku_scienti-0.0.4.tar", last modified: Fri Mar 31 00:32:32 2023, max compression
+gzip compressed data, was "Hunabku_scienti-0.0.5.tar", last modified: Mon May 29 22:23:55 2023, max compression
```

## Comparing `Hunabku_scienti-0.0.4.tar` & `Hunabku_scienti-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 00:32:32.777614 Hunabku_scienti-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 00:32:32.777614 Hunabku_scienti-0.0.4/Hunabku_scienti.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-03-31 00:32:32.000000 Hunabku_scienti-0.0.4/Hunabku_scienti.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-03-31 00:32:32.000000 Hunabku_scienti-0.0.4/Hunabku_scienti.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 00:32:32.000000 Hunabku_scienti-0.0.4/Hunabku_scienti.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-31 00:32:32.000000 Hunabku_scienti-0.0.4/Hunabku_scienti.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-31 00:32:32.000000 Hunabku_scienti-0.0.4/Hunabku_scienti.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-03-31 00:32:13.000000 Hunabku_scienti-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-31 00:32:13.000000 Hunabku_scienti-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-03-31 00:32:32.777614 Hunabku_scienti-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-03-31 00:32:13.000000 Hunabku_scienti-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 00:32:32.777614 Hunabku_scienti-0.0.4/hunabku_scienti/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 00:32:13.000000 Hunabku_scienti-0.0.4/hunabku_scienti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-03-31 00:32:13.000000 Hunabku_scienti-0.0.4/hunabku_scienti/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 00:32:32.777614 Hunabku_scienti-0.0.4/hunabku_scienti/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)    32839 2023-03-31 00:32:13.000000 Hunabku_scienti-0.0.4/hunabku_scienti/endpoints/Scienti.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 00:32:32.777614 Hunabku_scienti-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-03-31 00:32:13.000000 Hunabku_scienti-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:23:55.371066 Hunabku_scienti-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:23:55.371066 Hunabku_scienti-0.0.5/Hunabku_scienti.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-29 22:23:55.000000 Hunabku_scienti-0.0.5/Hunabku_scienti.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-29 22:23:55.000000 Hunabku_scienti-0.0.5/Hunabku_scienti.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 22:23:55.000000 Hunabku_scienti-0.0.5/Hunabku_scienti.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-29 22:23:55.000000 Hunabku_scienti-0.0.5/Hunabku_scienti.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 22:23:55.000000 Hunabku_scienti-0.0.5/Hunabku_scienti.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-29 22:23:36.000000 Hunabku_scienti-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-29 22:23:36.000000 Hunabku_scienti-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-29 22:23:55.371066 Hunabku_scienti-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-29 22:23:36.000000 Hunabku_scienti-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:23:55.371066 Hunabku_scienti-0.0.5/hunabku_scienti/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 22:23:36.000000 Hunabku_scienti-0.0.5/hunabku_scienti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-29 22:23:36.000000 Hunabku_scienti-0.0.5/hunabku_scienti/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:23:55.371066 Hunabku_scienti-0.0.5/hunabku_scienti/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)    32842 2023-05-29 22:23:36.000000 Hunabku_scienti-0.0.5/hunabku_scienti/endpoints/Scienti.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 22:23:55.371066 Hunabku_scienti-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-29 22:23:36.000000 Hunabku_scienti-0.0.5/setup.py
```

### Comparing `Hunabku_scienti-0.0.4/Hunabku_scienti.egg-info/PKG-INFO` & `Hunabku_scienti-0.0.5/Hunabku_scienti.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Hunabku-scienti
-Version: 0.0.4
+Version: 0.0.5
 Summary: Hunabku scienti plugin
 Home-page: https://github.com/colav/Hunabku_plugins
 Author: Colav
 Author-email: colav@udea.edu.co
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Hunabku_scienti-0.0.4/LICENSE` & `Hunabku_scienti-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Hunabku_scienti-0.0.4/PKG-INFO` & `Hunabku_scienti-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Hunabku_scienti
-Version: 0.0.4
+Version: 0.0.5
 Summary: Hunabku scienti plugin
 Home-page: https://github.com/colav/Hunabku_plugins
 Author: Colav
 Author-email: colav@udea.edu.co
 License: BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Hunabku_scienti-0.0.4/README.md` & `Hunabku_scienti-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `Hunabku_scienti-0.0.4/hunabku_scienti/endpoints/Scienti.py` & `Hunabku_scienti-0.0.5/hunabku_scienti/endpoints/Scienti.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
             model_year = self.request.args.get('model_year')
             institution = self.request.args.get('institution')
 
             response = self.check_required_parameters(self.request.args)
             if response is not None:
                 return response
             response = self.check_parameters(
-                ['apikey','COD_RH', 'COD_PRODUCTO', 'SGL_CATEGORIA', 'model_year', 'institution'], self.request.args.keys())
+                ['apikey', 'COD_RH', 'COD_PRODUCTO', 'SGL_CATEGORIA', 'model_year', 'institution'], self.request.args.keys())
             if response is not None:
                 return response
 
             db_name = f'scienti_{institution}_{model_year}'
 
             response = self.check_db(db_name)
             if response is not None:
@@ -491,23 +491,23 @@
         else:
             return self.apikey_error()
 
     @endpoint('/scienti/patent', methods=['GET'])
     def scienti_patent(self):
         """
         @api {get} /scienti/patent Scienti patent endpoint
-        @apiName event
+        @apiName patent
         @apiGroup Scienti
         @apiDescription Allows to perform queries for patents,
                         model_year is mandatory parameter, if model year is the only
                         parameter passed, the endpoint returns all the dump of the database.
 
         @apiParam {String} apikey  Credential for authentication
         @apiParam {String} COD_RH  User primary key
-        @apiParam {String} COD_PATENTE  event key (require COD_RH)
+        @apiParam {String} COD_PATENTE  patent key (require COD_RH)
         @apiParam {String} SGL_CATEGORIA  category of the network
         @apiParam {String} model_year  year of the scienti model, example: 2022
         @apiParam {String} institution institution initials. supported example: udea, uec, unaula
 
         @apiSuccess {Object}  Resgisters from MongoDB in Json format.
 
         @apiError (Error 401) msg  The HTTP 401 Unauthorized invalid authentication apikey for the target resource.
```

### Comparing `Hunabku_scienti-0.0.4/setup.py` & `Hunabku_scienti-0.0.5/setup.py`

 * *Files identical despite different names*

