# Comparing `tmp/crabpy_pyramid-1.5.0.tar.gz` & `tmp/crabpy_pyramid-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crabpy_pyramid-1.5.0.tar", last modified: Tue May 23 09:30:17 2023, max compression
+gzip compressed data, was "crabpy_pyramid-1.6.0.tar", last modified: Tue May 30 09:38:17 2023, max compression
```

## Comparing `crabpy_pyramid-1.5.0.tar` & `crabpy_pyramid-1.6.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-23 09:30:17.489079 crabpy_pyramid-1.5.0/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     4699 2023-05-23 09:30:14.000000 crabpy_pyramid-1.5.0/CHANGES.rst
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1089 2023-04-13 13:30:11.000000 crabpy_pyramid-1.5.0/LICENSE
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       39 2023-04-13 13:30:11.000000 crabpy_pyramid-1.5.0/MANIFEST.in
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6729 2023-05-23 09:30:17.489079 crabpy_pyramid-1.5.0/PKG-INFO
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1326 2023-04-13 13:30:11.000000 crabpy_pyramid-1.5.0/README.rst
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-23 09:30:17.489079 crabpy_pyramid-1.5.0/crabpy_pyramid/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    11585 2023-05-23 09:30:14.000000 crabpy_pyramid-1.5.0/crabpy_pyramid/__init__.py
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-23 09:30:17.489079 crabpy_pyramid-1.5.0/crabpy_pyramid/renderers/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:11.000000 crabpy_pyramid-1.5.0/crabpy_pyramid/renderers/__init__.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6935 2023-05-09 05:35:34.000000 crabpy_pyramid-1.5.0/crabpy_pyramid/renderers/adressenregister.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     3726 2023-04-13 13:30:11.000000 crabpy_pyramid-1.5.0/crabpy_pyramid/renderers/capakey.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    15765 2023-04-13 13:30:11.000000 crabpy_pyramid-1.5.0/crabpy_pyramid/renderers/crab.py
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-23 09:30:17.489079 crabpy_pyramid-1.5.0/crabpy_pyramid/routes/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:11.000000 crabpy_pyramid-1.5.0/crabpy_pyramid/routes/__init__.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     3685 2023-05-23 09:30:14.000000 crabpy_pyramid-1.5.0/crabpy_pyramid/routes/adressenregister.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1901 2023-04-13 13:30:11.000000 crabpy_pyramid-1.5.0/crabpy_pyramid/routes/capakey.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     4825 2023-04-13 13:30:11.000000 crabpy_pyramid-1.5.0/crabpy_pyramid/routes/crab.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     2735 2023-04-13 13:30:11.000000 crabpy_pyramid-1.5.0/crabpy_pyramid/utils.py
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-23 09:30:17.489079 crabpy_pyramid-1.5.0/crabpy_pyramid/views/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:11.000000 crabpy_pyramid-1.5.0/crabpy_pyramid/views/__init__.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    12235 2023-05-23 09:30:14.000000 crabpy_pyramid-1.5.0/crabpy_pyramid/views/adressenregister.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     5610 2023-04-13 13:30:11.000000 crabpy_pyramid-1.5.0/crabpy_pyramid/views/capakey.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    13969 2023-04-13 13:30:11.000000 crabpy_pyramid-1.5.0/crabpy_pyramid/views/crab.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      599 2023-05-05 13:21:30.000000 crabpy_pyramid-1.5.0/crabpy_pyramid/views/exceptions.py
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-23 09:30:17.489079 crabpy_pyramid-1.5.0/crabpy_pyramid.egg-info/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6729 2023-05-23 09:30:17.000000 crabpy_pyramid-1.5.0/crabpy_pyramid.egg-info/PKG-INFO
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      839 2023-05-23 09:30:17.000000 crabpy_pyramid-1.5.0/crabpy_pyramid.egg-info/SOURCES.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-05-23 09:30:17.000000 crabpy_pyramid-1.5.0/crabpy_pyramid.egg-info/dependency_links.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       47 2023-05-23 09:30:17.000000 crabpy_pyramid-1.5.0/crabpy_pyramid.egg-info/entry_points.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-04-13 13:30:20.000000 crabpy_pyramid-1.5.0/crabpy_pyramid.egg-info/not-zip-safe
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       42 2023-05-23 09:30:17.000000 crabpy_pyramid-1.5.0/crabpy_pyramid.egg-info/requires.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       15 2023-05-23 09:30:17.000000 crabpy_pyramid-1.5.0/crabpy_pyramid.egg-info/top_level.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      173 2023-05-23 09:30:17.489079 crabpy_pyramid-1.5.0/setup.cfg
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1484 2023-05-23 09:30:14.000000 crabpy_pyramid-1.5.0/setup.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-30 09:38:17.150988 crabpy_pyramid-1.6.0/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     4781 2023-05-30 09:37:25.000000 crabpy_pyramid-1.6.0/CHANGES.rst
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1089 2023-04-13 13:30:11.000000 crabpy_pyramid-1.6.0/LICENSE
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       39 2023-04-13 13:30:11.000000 crabpy_pyramid-1.6.0/MANIFEST.in
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6811 2023-05-30 09:38:17.150988 crabpy_pyramid-1.6.0/PKG-INFO
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1326 2023-04-13 13:30:11.000000 crabpy_pyramid-1.6.0/README.rst
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-30 09:38:17.150988 crabpy_pyramid-1.6.0/crabpy_pyramid/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    11585 2023-05-23 09:30:14.000000 crabpy_pyramid-1.6.0/crabpy_pyramid/__init__.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-30 09:38:17.150988 crabpy_pyramid-1.6.0/crabpy_pyramid/renderers/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:11.000000 crabpy_pyramid-1.6.0/crabpy_pyramid/renderers/__init__.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6939 2023-05-30 09:37:25.000000 crabpy_pyramid-1.6.0/crabpy_pyramid/renderers/adressenregister.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     3726 2023-04-13 13:30:11.000000 crabpy_pyramid-1.6.0/crabpy_pyramid/renderers/capakey.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    15765 2023-04-13 13:30:11.000000 crabpy_pyramid-1.6.0/crabpy_pyramid/renderers/crab.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-30 09:38:17.150988 crabpy_pyramid-1.6.0/crabpy_pyramid/routes/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:11.000000 crabpy_pyramid-1.6.0/crabpy_pyramid/routes/__init__.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     3685 2023-05-23 09:30:14.000000 crabpy_pyramid-1.6.0/crabpy_pyramid/routes/adressenregister.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1901 2023-04-13 13:30:11.000000 crabpy_pyramid-1.6.0/crabpy_pyramid/routes/capakey.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     4825 2023-04-13 13:30:11.000000 crabpy_pyramid-1.6.0/crabpy_pyramid/routes/crab.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     2735 2023-04-13 13:30:11.000000 crabpy_pyramid-1.6.0/crabpy_pyramid/utils.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-30 09:38:17.150988 crabpy_pyramid-1.6.0/crabpy_pyramid/views/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-04-13 13:30:11.000000 crabpy_pyramid-1.6.0/crabpy_pyramid/views/__init__.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    12235 2023-05-23 09:30:14.000000 crabpy_pyramid-1.6.0/crabpy_pyramid/views/adressenregister.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     5610 2023-04-13 13:30:11.000000 crabpy_pyramid-1.6.0/crabpy_pyramid/views/capakey.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    13969 2023-04-13 13:30:11.000000 crabpy_pyramid-1.6.0/crabpy_pyramid/views/crab.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      599 2023-05-05 13:21:30.000000 crabpy_pyramid-1.6.0/crabpy_pyramid/views/exceptions.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-05-30 09:38:17.150988 crabpy_pyramid-1.6.0/crabpy_pyramid.egg-info/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6811 2023-05-30 09:38:17.000000 crabpy_pyramid-1.6.0/crabpy_pyramid.egg-info/PKG-INFO
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      839 2023-05-30 09:38:17.000000 crabpy_pyramid-1.6.0/crabpy_pyramid.egg-info/SOURCES.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-05-30 09:38:17.000000 crabpy_pyramid-1.6.0/crabpy_pyramid.egg-info/dependency_links.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       47 2023-05-30 09:38:17.000000 crabpy_pyramid-1.6.0/crabpy_pyramid.egg-info/entry_points.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-04-13 13:30:20.000000 crabpy_pyramid-1.6.0/crabpy_pyramid.egg-info/not-zip-safe
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       42 2023-05-30 09:38:17.000000 crabpy_pyramid-1.6.0/crabpy_pyramid.egg-info/requires.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       15 2023-05-30 09:38:17.000000 crabpy_pyramid-1.6.0/crabpy_pyramid.egg-info/top_level.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      173 2023-05-30 09:38:17.150988 crabpy_pyramid-1.6.0/setup.cfg
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1484 2023-05-30 09:37:25.000000 crabpy_pyramid-1.6.0/setup.py
```

### Comparing `crabpy_pyramid-1.5.0/CHANGES.rst` & `crabpy_pyramid-1.6.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+1.6.0 (30-05-2023)
+------------------
+
+- land.id vervangen door land.code (#191)
+
 1.5.0 (23-05-2023)
 ------------------
 
 - Nice to haves (#184)
 - Support voor py3.10+ (#187)
 
 1.4.0 (09-05-2023)
```

### Comparing `crabpy_pyramid-1.5.0/LICENSE` & `crabpy_pyramid-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.5.0/PKG-INFO` & `crabpy_pyramid-1.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crabpy_pyramid
-Version: 1.5.0
+Version: 1.6.0
 Summary: Bindings for the CRABpy webservices and the Pyramid framework.
 Home-page: http://github.com/OnroerendErfgoed/crabpy_pyramid
 Author: Onroerend Erfgoed
 Author-email: ict@onroerenderfgoed.be
 License: MIT
 Keywords: web wsgi pyramid CRAB CAPAKEY AGIV
 Classifier: Development Status :: 5 - Production/Stable
@@ -48,14 +48,19 @@
     # activate your virtual env
     $ pip install sphinx sphinxcontrib-httpdomain
     $ python setup.py develop
     $ cd docs
     $ make html
 
 
+1.6.0 (30-05-2023)
+------------------
+
+- land.id vervangen door land.code (#191)
+
 1.5.0 (23-05-2023)
 ------------------
 
 - Nice to haves (#184)
 - Support voor py3.10+ (#187)
 
 1.4.0 (09-05-2023)
```

### Comparing `crabpy_pyramid-1.5.0/README.rst` & `crabpy_pyramid-1.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.5.0/crabpy_pyramid/__init__.py` & `crabpy_pyramid-1.6.0/crabpy_pyramid/__init__.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.5.0/crabpy_pyramid/renderers/adressenregister.py` & `crabpy_pyramid-1.6.0/crabpy_pyramid/renderers/adressenregister.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
 
 def list_landen_adapter(obj, request):
     """
     Adapter for rendering a list of landen to json.
     """
     return {
-        "id": obj.alpha_2,
+        "code": obj.alpha_2,
         "naam": _(obj.name)
     }
 
 
 json_list_renderer.add_adapter(adressenregister.Gewest, list_gewesten_adapter)
 json_list_renderer.add_adapter(adressenregister.Provincie, list_provincie_adapter)
 json_list_renderer.add_adapter(adressenregister.Deelgemeente, list_deelgemeente_adapter)
@@ -231,15 +231,15 @@
 
 def item_land_adapter(obj, request):
     """
     Adapter for rendering an item of
     :class: `pycountry.db.Data` to json.
     """
     return {
-        "id": obj.alpha_2,
+        "code": obj.alpha_2,
         "alpha2": obj.alpha_2,
         "alpha3": obj.alpha_3,
         "naam": obj.name,
     }
 
 
 def list_postinfo_adapter(obj, request):
```

### Comparing `crabpy_pyramid-1.5.0/crabpy_pyramid/renderers/capakey.py` & `crabpy_pyramid-1.6.0/crabpy_pyramid/renderers/capakey.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.5.0/crabpy_pyramid/renderers/crab.py` & `crabpy_pyramid-1.6.0/crabpy_pyramid/renderers/crab.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.5.0/crabpy_pyramid/routes/adressenregister.py` & `crabpy_pyramid-1.6.0/crabpy_pyramid/routes/adressenregister.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.5.0/crabpy_pyramid/routes/capakey.py` & `crabpy_pyramid-1.6.0/crabpy_pyramid/routes/capakey.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.5.0/crabpy_pyramid/routes/crab.py` & `crabpy_pyramid-1.6.0/crabpy_pyramid/routes/crab.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.5.0/crabpy_pyramid/utils.py` & `crabpy_pyramid-1.6.0/crabpy_pyramid/utils.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.5.0/crabpy_pyramid/views/adressenregister.py` & `crabpy_pyramid-1.6.0/crabpy_pyramid/views/adressenregister.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.5.0/crabpy_pyramid/views/capakey.py` & `crabpy_pyramid-1.6.0/crabpy_pyramid/views/capakey.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.5.0/crabpy_pyramid/views/crab.py` & `crabpy_pyramid-1.6.0/crabpy_pyramid/views/crab.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.5.0/crabpy_pyramid/views/exceptions.py` & `crabpy_pyramid-1.6.0/crabpy_pyramid/views/exceptions.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.5.0/crabpy_pyramid.egg-info/PKG-INFO` & `crabpy_pyramid-1.6.0/crabpy_pyramid.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crabpy-pyramid
-Version: 1.5.0
+Version: 1.6.0
 Summary: Bindings for the CRABpy webservices and the Pyramid framework.
 Home-page: http://github.com/OnroerendErfgoed/crabpy_pyramid
 Author: Onroerend Erfgoed
 Author-email: ict@onroerenderfgoed.be
 License: MIT
 Keywords: web wsgi pyramid CRAB CAPAKEY AGIV
 Classifier: Development Status :: 5 - Production/Stable
@@ -48,14 +48,19 @@
     # activate your virtual env
     $ pip install sphinx sphinxcontrib-httpdomain
     $ python setup.py develop
     $ cd docs
     $ make html
 
 
+1.6.0 (30-05-2023)
+------------------
+
+- land.id vervangen door land.code (#191)
+
 1.5.0 (23-05-2023)
 ------------------
 
 - Nice to haves (#184)
 - Support voor py3.10+ (#187)
 
 1.4.0 (09-05-2023)
```

### Comparing `crabpy_pyramid-1.5.0/crabpy_pyramid.egg-info/SOURCES.txt` & `crabpy_pyramid-1.6.0/crabpy_pyramid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-1.5.0/setup.py` & `crabpy_pyramid-1.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     'coverage',
     'webtest'
 ]
 
 testing_extras = tests_requires + []
 
 setup(name='crabpy_pyramid',
-      version='1.5.0',
+      version='1.6.0',
       description='Bindings for the CRABpy webservices and the Pyramid framework.',
       long_description=README + '\n\n' + CHANGES,
       classifiers=[
         'Development Status :: 5 - Production/Stable',
         "Programming Language :: Python",
         'Programming Language :: Python :: 3.8',
         "Framework :: Pyramid",
```

