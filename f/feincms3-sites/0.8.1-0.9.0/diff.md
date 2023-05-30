# Comparing `tmp/feincms3-sites-0.8.1.tar.gz` & `tmp/feincms3-sites-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/feincms3-sites-0.8.1.tar", last modified: Mon Apr  8 12:26:12 2019, max compression
+gzip compressed data, was "dist/feincms3-sites-0.9.0.tar", last modified: Fri Sep 20 08:09:54 2019, max compression
```

## Comparing `feincms3-sites-0.8.1.tar` & `feincms3-sites-0.9.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2019-04-08 12:26:12.000000 feincms3-sites-0.8.1/
--rw-r--r--   0 matthias   (501) staff       (20)     1548 2019-04-08 12:17:14.000000 feincms3-sites-0.8.1/LICENSE
--rw-r--r--   0 matthias   (501) staff       (20)      184 2019-04-08 12:17:14.000000 feincms3-sites-0.8.1/MANIFEST.in
--rw-r--r--   0 matthias   (501) staff       (20)     1448 2019-04-08 12:26:12.000000 feincms3-sites-0.8.1/PKG-INFO
--rw-r--r--   0 matthias   (501) staff       (20)      473 2019-04-08 12:17:14.000000 feincms3-sites-0.8.1/README.rst
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2019-04-08 12:26:12.000000 feincms3-sites-0.8.1/feincms3_sites/
--rw-r--r--   0 matthias   (501) staff       (20)      121 2019-04-08 12:25:16.000000 feincms3-sites-0.8.1/feincms3_sites/__init__.py
--rw-r--r--   0 matthias   (501) staff       (20)     1144 2019-04-08 12:17:14.000000 feincms3-sites-0.8.1/feincms3_sites/admin.py
--rw-r--r--   0 matthias   (501) staff       (20)      232 2019-04-08 12:17:14.000000 feincms3-sites-0.8.1/feincms3_sites/apps.py
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2019-04-08 12:26:12.000000 feincms3-sites-0.8.1/feincms3_sites/locale/
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2019-04-08 12:26:12.000000 feincms3-sites-0.8.1/feincms3_sites/locale/de/
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2019-04-08 12:26:12.000000 feincms3-sites-0.8.1/feincms3_sites/locale/de/LC_MESSAGES/
--rw-r--r--   0 matthias   (501) staff       (20)     1964 2019-04-08 12:17:14.000000 feincms3-sites-0.8.1/feincms3_sites/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 matthias   (501) staff       (20)     2507 2019-04-08 12:17:14.000000 feincms3-sites-0.8.1/feincms3_sites/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0 matthias   (501) staff       (20)     2707 2019-04-08 12:17:14.000000 feincms3-sites-0.8.1/feincms3_sites/middleware.py
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2019-04-08 12:26:12.000000 feincms3-sites-0.8.1/feincms3_sites/migrations/
--rw-r--r--   0 matthias   (501) staff       (20)     1178 2019-04-08 12:17:14.000000 feincms3-sites-0.8.1/feincms3_sites/migrations/0001_initial.py
--rw-r--r--   0 matthias   (501) staff       (20)      532 2019-04-08 12:17:14.000000 feincms3-sites-0.8.1/feincms3_sites/migrations/0002_site_is_managed_re.py
--rw-r--r--   0 matthias   (501) staff       (20)      719 2019-04-08 12:17:14.000000 feincms3-sites-0.8.1/feincms3_sites/migrations/0003_site_default_language.py
--rw-r--r--   0 matthias   (501) staff       (20)      407 2019-04-08 12:17:14.000000 feincms3-sites-0.8.1/feincms3_sites/migrations/0004_site_is_active.py
--rw-r--r--   0 matthias   (501) staff       (20)        0 2019-04-08 12:17:14.000000 feincms3-sites-0.8.1/feincms3_sites/migrations/__init__.py
--rw-r--r--   0 matthias   (501) staff       (20)     4898 2019-04-08 12:20:54.000000 feincms3-sites-0.8.1/feincms3_sites/models.py
-drwxr-xr-x   0 matthias   (501) staff       (20)        0 2019-04-08 12:26:12.000000 feincms3-sites-0.8.1/feincms3_sites.egg-info/
--rw-r--r--   0 matthias   (501) staff       (20)     1448 2019-04-08 12:26:12.000000 feincms3-sites-0.8.1/feincms3_sites.egg-info/PKG-INFO
--rw-r--r--   0 matthias   (501) staff       (20)      735 2019-04-08 12:26:12.000000 feincms3-sites-0.8.1/feincms3_sites.egg-info/SOURCES.txt
--rw-r--r--   0 matthias   (501) staff       (20)        1 2019-04-08 12:26:12.000000 feincms3-sites-0.8.1/feincms3_sites.egg-info/dependency_links.txt
--rw-r--r--   0 matthias   (501) staff       (20)        1 2019-04-08 12:26:12.000000 feincms3-sites-0.8.1/feincms3_sites.egg-info/not-zip-safe
--rw-r--r--   0 matthias   (501) staff       (20)       56 2019-04-08 12:26:12.000000 feincms3-sites-0.8.1/feincms3_sites.egg-info/requires.txt
--rw-r--r--   0 matthias   (501) staff       (20)       15 2019-04-08 12:26:12.000000 feincms3-sites-0.8.1/feincms3_sites.egg-info/top_level.txt
--rw-r--r--   0 matthias   (501) staff       (20)      258 2019-04-08 12:26:12.000000 feincms3-sites-0.8.1/setup.cfg
--rwxr-xr-x   0 matthias   (501) staff       (20)     1578 2019-04-08 12:17:14.000000 feincms3-sites-0.8.1/setup.py
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2019-09-20 08:09:54.000000 feincms3-sites-0.9.0/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1548 2019-09-20 06:55:58.000000 feincms3-sites-0.9.0/LICENSE
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      184 2019-09-20 06:55:58.000000 feincms3-sites-0.9.0/MANIFEST.in
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1448 2019-09-20 08:09:54.000000 feincms3-sites-0.9.0/PKG-INFO
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      473 2019-09-20 06:55:58.000000 feincms3-sites-0.9.0/README.rst
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2019-09-20 08:09:54.000000 feincms3-sites-0.9.0/feincms3_sites/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      121 2019-09-20 08:08:50.000000 feincms3-sites-0.9.0/feincms3_sites/__init__.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1144 2019-09-20 06:55:58.000000 feincms3-sites-0.9.0/feincms3_sites/admin.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      232 2019-09-20 06:55:58.000000 feincms3-sites-0.9.0/feincms3_sites/apps.py
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2019-09-20 08:09:54.000000 feincms3-sites-0.9.0/feincms3_sites/locale/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2019-09-20 08:09:54.000000 feincms3-sites-0.9.0/feincms3_sites/locale/de/
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2019-09-20 08:09:54.000000 feincms3-sites-0.9.0/feincms3_sites/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1964 2019-09-20 06:55:58.000000 feincms3-sites-0.9.0/feincms3_sites/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2507 2019-09-20 06:55:58.000000 feincms3-sites-0.9.0/feincms3_sites/locale/de/LC_MESSAGES/django.po
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     2669 2019-09-20 06:56:27.000000 feincms3-sites-0.9.0/feincms3_sites/middleware.py
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2019-09-20 08:09:54.000000 feincms3-sites-0.9.0/feincms3_sites/migrations/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1178 2019-09-20 06:55:58.000000 feincms3-sites-0.9.0/feincms3_sites/migrations/0001_initial.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      532 2019-09-20 06:55:58.000000 feincms3-sites-0.9.0/feincms3_sites/migrations/0002_site_is_managed_re.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      719 2019-09-20 06:55:58.000000 feincms3-sites-0.9.0/feincms3_sites/migrations/0003_site_default_language.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      407 2019-09-20 06:55:58.000000 feincms3-sites-0.9.0/feincms3_sites/migrations/0004_site_is_active.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)        0 2019-09-20 06:55:58.000000 feincms3-sites-0.9.0/feincms3_sites/migrations/__init__.py
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     4941 2019-09-20 07:13:11.000000 feincms3-sites-0.9.0/feincms3_sites/models.py
+drwxrwxr-x   0 matthias  (1000) matthias  (1000)        0 2019-09-20 08:09:54.000000 feincms3-sites-0.9.0/feincms3_sites.egg-info/
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)     1448 2019-09-20 08:09:53.000000 feincms3-sites-0.9.0/feincms3_sites.egg-info/PKG-INFO
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      735 2019-09-20 08:09:54.000000 feincms3-sites-0.9.0/feincms3_sites.egg-info/SOURCES.txt
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)        1 2019-09-20 08:09:53.000000 feincms3-sites-0.9.0/feincms3_sites.egg-info/dependency_links.txt
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)        1 2019-09-20 07:12:45.000000 feincms3-sites-0.9.0/feincms3_sites.egg-info/not-zip-safe
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       56 2019-09-20 08:09:53.000000 feincms3-sites-0.9.0/feincms3_sites.egg-info/requires.txt
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)       15 2019-09-20 08:09:53.000000 feincms3-sites-0.9.0/feincms3_sites.egg-info/top_level.txt
+-rw-rw-r--   0 matthias  (1000) matthias  (1000)      258 2019-09-20 08:09:54.000000 feincms3-sites-0.9.0/setup.cfg
+-rwxrwxr-x   0 matthias  (1000) matthias  (1000)     1578 2019-09-20 06:55:58.000000 feincms3-sites-0.9.0/setup.py
```

### Comparing `feincms3-sites-0.8.1/LICENSE` & `feincms3-sites-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `feincms3-sites-0.8.1/PKG-INFO` & `feincms3-sites-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: feincms3-sites
-Version: 0.8.1
+Version: 0.9.0
 Summary: Multisite support for feincms3
 Home-page: https://github.com/matthiask/feincms3-sites/
 Author: Matthias Kestenholz
 Author-email: mk@feinheit.ch
 License: BSD License
 Description: ==============
         feincms3-sites
```

### Comparing `feincms3-sites-0.8.1/feincms3_sites/admin.py` & `feincms3-sites-0.9.0/feincms3_sites/admin.py`

 * *Files identical despite different names*

### Comparing `feincms3-sites-0.8.1/feincms3_sites/locale/de/LC_MESSAGES/django.mo` & `feincms3-sites-0.9.0/feincms3_sites/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `feincms3-sites-0.8.1/feincms3_sites/locale/de/LC_MESSAGES/django.po` & `feincms3-sites-0.9.0/feincms3_sites/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `feincms3-sites-0.8.1/feincms3_sites/middleware.py` & `feincms3-sites-0.9.0/feincms3_sites/middleware.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 
 def redirect_to_site_middleware(get_response):
     def middleware(request):
         if not hasattr(request, "site"):
             raise ImproperlyConfigured(
                 'No "site" attribute on request. Insert site_middleware'
-                " or apps_middleware before redirect_to_site_middleware."
+                " before redirect_to_site_middleware."
             )
 
         # Host matches, and either no HTTPS enforcement or already HTTPS
         if request.get_host() == request.site.host and (
             not settings.SECURE_SSL_REDIRECT or request.is_secure()
         ):
             return get_response(request)
@@ -62,15 +62,15 @@
 
 
 def default_language_middleware(get_response):
     def middleware(request):
         if not hasattr(request, "site"):
             raise ImproperlyConfigured(
                 'No "site" attribute on request. Insert site_middleware'
-                " or apps_middleware before default_language_middleware."
+                " before default_language_middleware."
             )
 
         # No i18n_patterns handling for now.
         if request.site.default_language:
             language = request.site.default_language
         else:
             language = translation.get_language_from_request(request)
```

### Comparing `feincms3-sites-0.8.1/feincms3_sites/migrations/0001_initial.py` & `feincms3-sites-0.9.0/feincms3_sites/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `feincms3-sites-0.8.1/feincms3_sites/migrations/0002_site_is_managed_re.py` & `feincms3-sites-0.9.0/feincms3_sites/migrations/0002_site_is_managed_re.py`

 * *Files identical despite different names*

### Comparing `feincms3-sites-0.8.1/feincms3_sites/migrations/0003_site_default_language.py` & `feincms3-sites-0.9.0/feincms3_sites/migrations/0003_site_default_language.py`

 * *Files identical despite different names*

### Comparing `feincms3-sites-0.8.1/feincms3_sites/models.py` & `feincms3-sites-0.9.0/feincms3_sites/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,17 @@
         ordering = ["position"]
         unique_together = (("site", "path"),)
         verbose_name = _("page")
         verbose_name_plural = _("pages")
 
     def _path_clash_candidates(self):
         return self.__class__._default_manager.exclude(
-            ~Q(site=self.site_id) | Q(pk__in=self.descendants()) | Q(pk=self.pk)
+            ~Q(site=self.site_id)
+            | Q(pk__in=self.descendants(), static_path=False)
+            | Q(pk=self.pk)
         )
 
     def clean_fields(self, exclude=None):
         """
         Since the ``SiteForeignKey`` adds ``required=False`` we have to add
         our own check here.
         """
```

### Comparing `feincms3-sites-0.8.1/feincms3_sites.egg-info/PKG-INFO` & `feincms3-sites-0.9.0/feincms3_sites.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: feincms3-sites
-Version: 0.8.1
+Version: 0.9.0
 Summary: Multisite support for feincms3
 Home-page: https://github.com/matthiask/feincms3-sites/
 Author: Matthias Kestenholz
 Author-email: mk@feinheit.ch
 License: BSD License
 Description: ==============
         feincms3-sites
```

### Comparing `feincms3-sites-0.8.1/feincms3_sites.egg-info/SOURCES.txt` & `feincms3-sites-0.9.0/feincms3_sites.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feincms3-sites-0.8.1/setup.py` & `feincms3-sites-0.9.0/setup.py`

 * *Files identical despite different names*

