# Comparing `tmp/django-large-image-0.8.2.tar.gz` & `tmp/django-large-image-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-large-image-0.8.2.tar", last modified: Sun Feb 19 20:53:28 2023, max compression
+gzip compressed data, was "django-large-image-0.9.0.tar", last modified: Thu Feb 23 19:19:05 2023, max compression
```

## Comparing `django-large-image-0.8.2.tar` & `django-large-image-0.9.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 20:53:28.502217 django-large-image-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-19 20:53:21.000000 django-large-image-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-02-19 20:53:21.000000 django-large-image-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-02-19 20:53:21.000000 django-large-image-0.8.2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)    17831 2023-02-19 20:53:28.502217 django-large-image-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16953 2023-02-19 20:53:21.000000 django-large-image-0.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 20:53:28.486216 django-large-image-0.8.2/django_large_image/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-02-19 20:53:21.000000 django-large-image-0.8.2/django_large_image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-02-19 20:53:21.000000 django-large-image-0.8.2/django_large_image/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-02-19 20:53:21.000000 django-large-image-0.8.2/django_large_image/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 20:53:28.494217 django-large-image-0.8.2/django_large_image/rest/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-02-19 20:53:21.000000 django-large-image-0.8.2/django_large_image/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-02-19 20:53:21.000000 django-large-image-0.8.2/django_large_image/rest/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-02-19 20:53:21.000000 django-large-image-0.8.2/django_large_image/rest/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6546 2023-02-19 20:53:21.000000 django-large-image-0.8.2/django_large_image/rest/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-02-19 20:53:21.000000 django-large-image-0.8.2/django_large_image/rest/params.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-02-19 20:53:21.000000 django-large-image-0.8.2/django_large_image/rest/renderers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-02-19 20:53:21.000000 django-large-image-0.8.2/django_large_image/rest/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-02-19 20:53:21.000000 django-large-image-0.8.2/django_large_image/rest/standalone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-02-19 20:53:21.000000 django-large-image-0.8.2/django_large_image/rest/tiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-02-19 20:53:21.000000 django-large-image-0.8.2/django_large_image/rest/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 20:53:28.482216 django-large-image-0.8.2/django_large_image/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 20:53:28.482216 django-large-image-0.8.2/django_large_image/static/django_large_image/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 20:53:28.494217 django-large-image-0.8.2/django_large_image/static/django_large_image/js/
--rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-02-19 20:53:21.000000 django-large-image-0.8.2/django_large_image/static/django_large_image/js/cesium.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 20:53:28.482216 django-large-image-0.8.2/django_large_image/static/django_large_image/js/geojs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 20:53:28.494217 django-large-image-0.8.2/django_large_image/static/django_large_image/js/geojs/1.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)  3465593 2023-02-19 20:53:21.000000 django-large-image-0.8.2/django_large_image/static/django_large_image/js/geojs/1.8.3/geo.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 20:53:28.498216 django-large-image-0.8.2/django_large_image/static/django_large_image/styles/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-02-19 20:53:21.000000 django-large-image-0.8.2/django_large_image/static/django_large_image/styles/cesium.css
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-02-19 20:53:21.000000 django-large-image-0.8.2/django_large_image/static/django_large_image/styles/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 20:53:28.482216 django-large-image-0.8.2/django_large_image/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 20:53:28.482216 django-large-image-0.8.2/django_large_image/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 20:53:28.482216 django-large-image-0.8.2/django_large_image/templates/admin/django_large_image/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 20:53:28.498216 django-large-image-0.8.2/django_large_image/templates/admin/django_large_image/_include/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-02-19 20:53:21.000000 django-large-image-0.8.2/django_large_image/templates/admin/django_large_image/_include/geojs.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 20:53:28.498216 django-large-image-0.8.2/django_large_image/templates/django_large_image/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 20:53:28.498216 django-large-image-0.8.2/django_large_image/templates/django_large_image/_include/
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-02-19 20:53:21.000000 django-large-image-0.8.2/django_large_image/templates/django_large_image/_include/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-02-19 20:53:21.000000 django-large-image-0.8.2/django_large_image/templates/django_large_image/_include/cesium.html
--rw-r--r--   0 runner    (1001) docker     (123)    13360 2023-02-19 20:53:21.000000 django-large-image-0.8.2/django_large_image/templates/django_large_image/_include/colors.html
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-02-19 20:53:21.000000 django-large-image-0.8.2/django_large_image/templates/django_large_image/_include/geojs.html
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-02-19 20:53:21.000000 django-large-image-0.8.2/django_large_image/templates/django_large_image/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-02-19 20:53:21.000000 django-large-image-0.8.2/django_large_image/templates/django_large_image/cesiumViewer.html
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-02-19 20:53:21.000000 django-large-image-0.8.2/django_large_image/templates/django_large_image/geojsViewer.html
--rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-02-19 20:53:21.000000 django-large-image-0.8.2/django_large_image/tilesource.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-02-19 20:53:21.000000 django-large-image-0.8.2/django_large_image/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-02-19 20:53:21.000000 django-large-image-0.8.2/django_large_image/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 20:53:28.490216 django-large-image-0.8.2/django_large_image.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17831 2023-02-19 20:53:28.000000 django-large-image-0.8.2/django_large_image.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-02-19 20:53:28.000000 django-large-image-0.8.2/django_large_image.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-19 20:53:28.000000 django-large-image-0.8.2/django_large_image.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-19 20:53:28.000000 django-large-image-0.8.2/django_large_image.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-02-19 20:53:28.000000 django-large-image-0.8.2/django_large_image.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-19 20:53:28.000000 django-large-image-0.8.2/django_large_image.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-02-19 20:53:21.000000 django-large-image-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-19 20:53:28.502217 django-large-image-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-02-19 20:53:21.000000 django-large-image-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 19:19:05.752039 django-large-image-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-23 19:18:58.000000 django-large-image-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-02-23 19:18:58.000000 django-large-image-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-02-23 19:18:58.000000 django-large-image-0.9.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    17831 2023-02-23 19:19:05.752039 django-large-image-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16953 2023-02-23 19:18:58.000000 django-large-image-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 19:19:05.740039 django-large-image-0.9.0/django_large_image/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-02-23 19:18:58.000000 django-large-image-0.9.0/django_large_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-02-23 19:18:58.000000 django-large-image-0.9.0/django_large_image/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-02-23 19:18:58.000000 django-large-image-0.9.0/django_large_image/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 19:19:05.744039 django-large-image-0.9.0/django_large_image/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-02-23 19:18:58.000000 django-large-image-0.9.0/django_large_image/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-02-23 19:18:58.000000 django-large-image-0.9.0/django_large_image/rest/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-02-23 19:18:58.000000 django-large-image-0.9.0/django_large_image/rest/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-02-23 19:18:58.000000 django-large-image-0.9.0/django_large_image/rest/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-02-23 19:18:58.000000 django-large-image-0.9.0/django_large_image/rest/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-02-23 19:18:58.000000 django-large-image-0.9.0/django_large_image/rest/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-02-23 19:18:58.000000 django-large-image-0.9.0/django_large_image/rest/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-02-23 19:18:58.000000 django-large-image-0.9.0/django_large_image/rest/standalone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-02-23 19:18:58.000000 django-large-image-0.9.0/django_large_image/rest/tiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-02-23 19:18:58.000000 django-large-image-0.9.0/django_large_image/rest/viewsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 19:19:05.736039 django-large-image-0.9.0/django_large_image/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 19:19:05.736039 django-large-image-0.9.0/django_large_image/static/django_large_image/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 19:19:05.744039 django-large-image-0.9.0/django_large_image/static/django_large_image/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-02-23 19:18:58.000000 django-large-image-0.9.0/django_large_image/static/django_large_image/js/cesium.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 19:19:05.736039 django-large-image-0.9.0/django_large_image/static/django_large_image/js/geojs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 19:19:05.744039 django-large-image-0.9.0/django_large_image/static/django_large_image/js/geojs/1.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)  3465593 2023-02-23 19:18:58.000000 django-large-image-0.9.0/django_large_image/static/django_large_image/js/geojs/1.8.3/geo.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 19:19:05.748039 django-large-image-0.9.0/django_large_image/static/django_large_image/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-02-23 19:18:58.000000 django-large-image-0.9.0/django_large_image/static/django_large_image/styles/cesium.css
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-02-23 19:18:58.000000 django-large-image-0.9.0/django_large_image/static/django_large_image/styles/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 19:19:05.736039 django-large-image-0.9.0/django_large_image/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 19:19:05.736039 django-large-image-0.9.0/django_large_image/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 19:19:05.736039 django-large-image-0.9.0/django_large_image/templates/admin/django_large_image/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 19:19:05.748039 django-large-image-0.9.0/django_large_image/templates/admin/django_large_image/_include/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-02-23 19:18:58.000000 django-large-image-0.9.0/django_large_image/templates/admin/django_large_image/_include/geojs.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 19:19:05.752039 django-large-image-0.9.0/django_large_image/templates/django_large_image/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 19:19:05.752039 django-large-image-0.9.0/django_large_image/templates/django_large_image/_include/
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-02-23 19:18:58.000000 django-large-image-0.9.0/django_large_image/templates/django_large_image/_include/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-02-23 19:18:58.000000 django-large-image-0.9.0/django_large_image/templates/django_large_image/_include/cesium.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13360 2023-02-23 19:18:58.000000 django-large-image-0.9.0/django_large_image/templates/django_large_image/_include/colors.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-02-23 19:18:58.000000 django-large-image-0.9.0/django_large_image/templates/django_large_image/_include/geojs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-02-23 19:18:58.000000 django-large-image-0.9.0/django_large_image/templates/django_large_image/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-02-23 19:18:58.000000 django-large-image-0.9.0/django_large_image/templates/django_large_image/cesiumViewer.html
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-02-23 19:18:58.000000 django-large-image-0.9.0/django_large_image/templates/django_large_image/geojsViewer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-02-23 19:18:58.000000 django-large-image-0.9.0/django_large_image/tilesource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-02-23 19:18:58.000000 django-large-image-0.9.0/django_large_image/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-02-23 19:18:58.000000 django-large-image-0.9.0/django_large_image/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 19:19:05.744039 django-large-image-0.9.0/django_large_image.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17831 2023-02-23 19:19:05.000000 django-large-image-0.9.0/django_large_image.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-02-23 19:19:05.000000 django-large-image-0.9.0/django_large_image.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 19:19:05.000000 django-large-image-0.9.0/django_large_image.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-23 19:19:05.000000 django-large-image-0.9.0/django_large_image.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-23 19:19:05.000000 django-large-image-0.9.0/django_large_image.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-23 19:19:05.000000 django-large-image-0.9.0/django_large_image.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-02-23 19:18:58.000000 django-large-image-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 19:19:05.752039 django-large-image-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-02-23 19:18:58.000000 django-large-image-0.9.0/setup.py
```

### Comparing `django-large-image-0.8.2/LICENSE` & `django-large-image-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-large-image-0.8.2/NOTICE` & `django-large-image-0.9.0/NOTICE`

 * *Files identical despite different names*

### Comparing `django-large-image-0.8.2/PKG-INFO` & `django-large-image-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-large-image
-Version: 0.8.2
+Version: 0.9.0
 Summary: Dynamic tile server in Django built on top of large-image (and GDAL)
 Home-page: https://github.com/girder/django-large-image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-large-image Version: 0.8.2 Summary: Dynamic
+Metadata-Version: 2.1 Name: django-large-image Version: 0.9.0 Summary: Dynamic
 tile server in Django built on top of large-image (and GDAL) Home-page: https:/
 /github.com/girder/django-large-image Author: Kitware, Inc. Author-email:
 kitware@kitware.com License: Apache 2.0 Platform: UNKNOWN Classifier:
 Development Status :: 3 - Alpha Classifier: Environment :: Web Environment
 Classifier: Framework :: Django :: 3.0 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: OS Independent
```

### Comparing `django-large-image-0.8.2/README.md` & `django-large-image-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `django-large-image-0.8.2/django_large_image/apps.py` & `django-large-image-0.9.0/django_large_image/apps.py`

 * *Files identical despite different names*

### Comparing `django-large-image-0.8.2/django_large_image/cache.py` & `django-large-image-0.9.0/django_large_image/cache.py`

 * *Files identical despite different names*

### Comparing `django-large-image-0.8.2/django_large_image/rest/base.py` & `django-large-image-0.9.0/django_large_image/rest/base.py`

 * *Files identical despite different names*

### Comparing `django-large-image-0.8.2/django_large_image/rest/data.py` & `django-large-image-0.9.0/django_large_image/rest/data.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.http import HttpResponse
-from drf_yasg.utils import swagger_auto_schema
+from drf_spectacular.utils import extend_schema
 from rest_framework.decorators import action
 from rest_framework.exceptions import ValidationError
 from rest_framework.request import Request
 from rest_framework.response import Response
 
 from django_large_image import tilesource, utilities
 from django_large_image.rest import params
@@ -17,18 +17,18 @@
 pixel_summary = 'Returns single pixel.'
 pixel_parameters = params.BASE + [params.left, params.top] + params.STYLE
 histogram_summary = 'Returns histogram'
 histogram_parameters = params.BASE + params.HISTOGRAM
 
 
 class DataMixin(LargeImageMixinBase):
-    @swagger_auto_schema(
-        method='GET',
-        operation_summary=thumbnail_summary,
-        manual_parameters=thumbnail_parameters,
+    @extend_schema(
+        methods=['GET'],
+        summary=thumbnail_summary,
+        parameters=thumbnail_parameters,
     )
     @action(
         detail=False,
         url_path=f'data/thumbnail.{params.FORMAT_URL_PATTERN}',
         renderer_classes=image_renderers,
     )
     def thumbnail(
@@ -37,18 +37,18 @@
         encoding = tilesource.format_to_encoding(fmt)
         width = int(self.get_query_param(request, 'max_width', 256))
         height = int(self.get_query_param(request, 'max_height', 256))
         source = self.get_tile_source(request, pk, encoding=encoding)
         thumb_data, mime_type = source.getThumbnail(encoding=encoding, width=width, height=height)
         return HttpResponse(thumb_data, content_type=mime_type)
 
-    @swagger_auto_schema(
-        method='GET',
-        operation_summary=region_summary,
-        manual_parameters=region_parameters + params.STYLE,
+    @extend_schema(
+        methods=['GET'],
+        summary=region_summary,
+        parameters=region_parameters + params.STYLE,
     )
     @action(
         detail=False,
         url_path=f'data/region.{params.FORMAT_URL_PATTERN}',
         renderer_classes=image_data_renderers,
     )
     def region(self, request: Request, pk: int = None, fmt: str = 'tiff', **kwargs) -> HttpResponse:
@@ -81,31 +81,31 @@
         if not path:
             raise ValidationError(
                 'No output generated, check that the bounds of your ROI overlap source imagery and that your `projection` and `units` are correct.'
             )
         tile_binary = open(path, 'rb')
         return HttpResponse(tile_binary, content_type=mime_type)
 
-    @swagger_auto_schema(
-        method='GET',
-        operation_summary=pixel_summary,
-        manual_parameters=pixel_parameters,
+    @extend_schema(
+        methods=['GET'],
+        summary=pixel_summary,
+        parameters=pixel_parameters,
     )
     @action(detail=False, url_path='data/pixel')
     def pixel(self, request: Request, pk: int = None, **kwargs) -> Response:
         left = int(self.get_query_param(request, 'left'))
         top = int(self.get_query_param(request, 'top'))
         source = self.get_tile_source(request, pk)
         metadata = source.getPixel(region={'left': left, 'top': top, 'units': 'pixels'})
         return Response(metadata)
 
-    @swagger_auto_schema(
-        method='GET',
-        operation_summary=histogram_summary,
-        manual_parameters=histogram_parameters,
+    @extend_schema(
+        methods=['GET'],
+        summary=histogram_summary,
+        parameters=histogram_parameters,
     )
     @action(detail=False, url_path='data/histogram')
     def histogram(self, request: Request, pk: int = None, **kwargs) -> Response:
         only_min_max = not utilities.param_nully(self.get_query_param(request, 'onlyMinMax', False))
         density = not utilities.param_nully(self.get_query_param(request, 'density', False))
         kwargs = dict(
             onlyMinMax=only_min_max,
@@ -124,52 +124,52 @@
                 for key in {'min', 'max', 'samples'}:
                     if key in entry:
                         entry[key] = float(entry[key])
         return Response(result)
 
 
 class DataDetailMixin(DataMixin):
-    @swagger_auto_schema(
-        method='GET',
-        operation_summary=thumbnail_summary,
-        manual_parameters=thumbnail_parameters,
+    @extend_schema(
+        methods=['GET'],
+        summary=thumbnail_summary,
+        parameters=thumbnail_parameters,
     )
     @action(
         detail=True,
         url_path=f'data/thumbnail.{params.FORMAT_URL_PATTERN}',
         renderer_classes=image_renderers,
     )
     def thumbnail(
         self, request: Request, pk: int = None, fmt: str = 'png', **kwargs
     ) -> HttpResponse:
         return super().thumbnail(request, pk, fmt)
 
-    @swagger_auto_schema(
-        method='GET',
-        operation_summary=region_summary,
-        manual_parameters=region_parameters + params.STYLE,
+    @extend_schema(
+        methods=['GET'],
+        summary=region_summary,
+        parameters=region_parameters + params.STYLE,
     )
     @action(
         detail=True,
         url_path=f'data/region.{params.FORMAT_URL_PATTERN}',
         renderer_classes=image_data_renderers,
     )
     def region(self, request: Request, pk: int = None, fmt: str = 'tiff', **kwargs) -> HttpResponse:
         return super().region(request, pk, fmt)
 
-    @swagger_auto_schema(
-        method='GET',
-        operation_summary=pixel_summary,
-        manual_parameters=pixel_parameters,
+    @extend_schema(
+        methods=['GET'],
+        summary=pixel_summary,
+        parameters=pixel_parameters,
     )
     @action(detail=True, url_path='data/pixel')
     def pixel(self, request: Request, pk: int = None, **kwargs) -> Response:
         return super().pixel(request, pk)
 
-    @swagger_auto_schema(
-        method='GET',
-        operation_summary=histogram_summary,
-        manual_parameters=histogram_parameters,
+    @extend_schema(
+        methods=['GET'],
+        summary=histogram_summary,
+        parameters=histogram_parameters,
     )
     @action(detail=True, url_path='data/histogram')
     def histogram(self, request: Request, pk: int = None, **kwargs) -> Response:
         return super().histogram(request, pk)
```

### Comparing `django-large-image-0.8.2/django_large_image/rest/metadata.py` & `django-large-image-0.9.0/django_large_image/rest/metadata.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import io
 import json
 import pathlib
 
-from drf_yasg.utils import swagger_auto_schema
+from drf_spectacular.utils import extend_schema
 from rest_framework.decorators import action
 from rest_framework.exceptions import APIException, ValidationError
 from rest_framework.request import Request
 from rest_framework.response import Response
 
 from django_large_image import tilesource
 from django_large_image.rest import params
@@ -29,74 +29,74 @@
 band_parameters = params.BASE + [params.band]
 frames_summary = 'Retrieve all channels/bands for each frame. This is used to generate a UI to control how the image is displayed.'
 frames_parameters = params.BASE
 tiffdump_summary = 'Returns tifftools tiffdump JSON. This will raise a `ValidationError` if the image is not a Tiff.'
 
 
 class MetaDataMixin(LargeImageMixinBase):
-    @swagger_auto_schema(
-        method='GET',
-        operation_summary=metadata_summary,
-        manual_parameters=metadata_parameters,
+    @extend_schema(
+        methods=['GET'],
+        summary=metadata_summary,
+        parameters=metadata_parameters,
     )
     @action(detail=False, url_path='info/metadata')
     def metadata(self, request: Request, pk: int = None, **kwargs) -> Response:
         source = self.get_tile_source(request, pk, style=False)
         metadata = tilesource.get_metadata(source)
         return Response(metadata)
 
-    @swagger_auto_schema(
-        method='GET',
-        operation_summary=metadata_internal_summary,
-        manual_parameters=metadata_internal_parameters,
+    @extend_schema(
+        methods=['GET'],
+        summary=metadata_internal_summary,
+        parameters=metadata_internal_parameters,
     )
     @action(detail=False, url_path='info/metadata_internal')
     def metadata_internal(self, request: Request, pk: int = None, **kwargs) -> Response:
         source = self.get_tile_source(request, pk, style=False)
         metadata = tilesource.get_metadata_internal(source)
         return Response(metadata)
 
-    @swagger_auto_schema(
-        method='GET',
-        operation_summary=bands_summary,
-        manual_parameters=bands_parameters,
+    @extend_schema(
+        methods=['GET'],
+        summary=bands_summary,
+        parameters=bands_parameters,
     )
     @action(detail=False, url_path='info/bands')
     def bands(self, request: Request, pk: int = None, **kwargs) -> Response:
         source = self.get_tile_source(request, pk, style=False)
         metadata = source.getBandInformation()
         return Response(metadata)
 
-    @swagger_auto_schema(
-        method='GET',
-        operation_summary=bands_summary,
-        manual_parameters=band_parameters,
+    @extend_schema(
+        methods=['GET'],
+        summary=bands_summary,
+        parameters=band_parameters,
     )
     @action(detail=False, url_path='info/band')
     def band(self, request: Request, pk: int = None, **kwargs) -> Response:
         # TODO: handle frame choice
         band = int(self.get_query_param(request, 'band', 1))
         source = self.get_tile_source(request, pk, style=False)
         metadata = source.getOneBandInformation(band)
         return Response(metadata)
 
-    @swagger_auto_schema(
-        method='GET',
-        operation_summary=frames_summary,
-        manual_parameters=frames_parameters,
+    @extend_schema(
+        methods=['GET'],
+        summary=frames_summary,
+        parameters=frames_parameters,
     )
     @action(detail=False, url_path='info/frames')
     def frames(self, request: Request, pk: int = None, **kwargs) -> Response:
         source = self.get_tile_source(request, pk, style=False)
         data = tilesource.get_frames(source)
         return Response(data)
 
-    @swagger_auto_schema(
-        method='GET',
-        operation_summary=tiffdump_summary,
+    @extend_schema(
+        methods=['GET'],
+        summary=tiffdump_summary,
     )
     @action(detail=False, url_path='info/tiffdump')
     def tiffdump(self, request: Request, pk: int = None, **kwargs) -> Response:
         if tifftools is None:  # pragma: no cover
             raise APIException('`tifftools` is not installed on the server.')
         source = self.get_tile_source(request, pk, style=False)
         # This will only work for local files (path on disk)
@@ -114,59 +114,59 @@
         except (TifftoolsError, OSError) as e:
             raise ValidationError(str(e))
         output.seek(0)
         return Response(json.loads(output.read()))
 
 
 class MetaDataDetailMixin(MetaDataMixin):
-    @swagger_auto_schema(
-        method='GET',
-        operation_summary=metadata_summary,
-        manual_parameters=metadata_parameters,
+    @extend_schema(
+        methods=['GET'],
+        summary=metadata_summary,
+        parameters=metadata_parameters,
     )
     @action(detail=True, url_path='info/metadata')
     def metadata(self, request: Request, pk: int = None, **kwargs) -> Response:
         return super().metadata(request, pk)
 
-    @swagger_auto_schema(
-        method='GET',
-        operation_summary=metadata_internal_summary,
-        manual_parameters=metadata_internal_parameters,
+    @extend_schema(
+        methods=['GET'],
+        summary=metadata_internal_summary,
+        parameters=metadata_internal_parameters,
     )
     @action(detail=True, url_path='info/metadata_internal')
     def metadata_internal(self, request: Request, pk: int = None, **kwargs) -> Response:
         return super().metadata_internal(request, pk)
 
-    @swagger_auto_schema(
-        method='GET',
-        operation_summary=bands_summary,
-        manual_parameters=bands_parameters,
+    @extend_schema(
+        methods=['GET'],
+        summary=bands_summary,
+        parameters=bands_parameters,
     )
     @action(detail=True, url_path='info/bands')
     def bands(self, request: Request, pk: int = None, **kwargs) -> Response:
         return super().bands(request, pk)
 
-    @swagger_auto_schema(
-        method='GET',
-        operation_summary=bands_summary,
-        manual_parameters=band_parameters,
+    @extend_schema(
+        methods=['GET'],
+        summary=bands_summary,
+        parameters=band_parameters,
     )
     @action(detail=True, url_path='info/band')
     def band(self, request: Request, pk: int = None, **kwargs) -> Response:
         return super().band(request, pk)
 
-    @swagger_auto_schema(
-        method='GET',
-        operation_summary=frames_summary,
-        manual_parameters=frames_parameters,
+    @extend_schema(
+        methods=['GET'],
+        summary=frames_summary,
+        parameters=frames_parameters,
     )
     @action(detail=True, url_path='info/frames')
     def frames(self, request: Request, pk: int = None, **kwargs) -> Response:
         return super().frames(request, pk)
 
-    @swagger_auto_schema(
-        method='GET',
-        operation_summary=tiffdump_summary,
+    @extend_schema(
+        methods=['GET'],
+        summary=tiffdump_summary,
     )
     @action(detail=True, url_path='info/tiffdump')
     def tiffdump(self, request: Request, pk: int = None, **kwargs) -> Response:
         return super().tiffdump(request, pk)
```

### Comparing `django-large-image-0.8.2/django_large_image/rest/params.py` & `django-large-image-0.9.0/django_large_image/rest/params.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,168 +1,185 @@
-from drf_yasg import openapi
+from drf_spectacular.openapi import OpenApiTypes
+from drf_spectacular.utils import OpenApiParameter
 
 from django_large_image.tilesource import get_formats
 
 FORMAT_URL_PATTERN = rf'(?P<fmt>{r"|".join(get_formats())})'
 
-projection = openapi.Parameter(
+projection = OpenApiParameter(
     'projection',
-    openapi.IN_QUERY,
+    location=OpenApiParameter.QUERY,
     description='The projection in which to open the image (try `EPSG:3857`).',
-    type=openapi.TYPE_STRING,
+    type=OpenApiTypes.STR,
 )
-source = openapi.Parameter(
+source = OpenApiParameter(
     'source',
-    openapi.IN_QUERY,
+    location=OpenApiParameter.QUERY,
     description='The source to use when opening the image. Use the `large-image/sources` endpoint to list the available sources.',
-    type=openapi.TYPE_STRING,
+    type=OpenApiTypes.STR,
 )
 
 BASE = [projection, source]
 
-fmt_png = openapi.Parameter(
+fmt_png = OpenApiParameter(
     'fmt',
-    openapi.IN_PATH,
+    location=OpenApiParameter.PATH,
     description=f'Image format ({" | ".join(get_formats())})',
-    type=openapi.TYPE_STRING,
+    type=OpenApiTypes.STR,
     default='png',
 )
-fmt_tiff = openapi.Parameter(
+fmt_tiff = OpenApiParameter(
     'fmt',
-    openapi.IN_PATH,
+    location=OpenApiParameter.PATH,
     description=f'Image format ({" | ".join(get_formats())})',
-    type=openapi.TYPE_STRING,
+    type=OpenApiTypes.STR,
     default='tiff',
 )
 
-z = openapi.Parameter(
+z = OpenApiParameter(
     'z',
-    openapi.IN_PATH,
+    location=OpenApiParameter.PATH,
     description='The Z level of the tile. May range from [0, levels], where 0 is the lowest resolution, single tile for the whole source.',
-    type=openapi.TYPE_INTEGER,
+    type=OpenApiTypes.INT,
 )
-x = openapi.Parameter(
+x = OpenApiParameter(
     'x',
-    openapi.IN_PATH,
+    location=OpenApiParameter.PATH,
     description='The 0-based X position of the tile on the specified Z level.',
-    type=openapi.TYPE_INTEGER,
+    type=OpenApiTypes.INT,
 )
-y = openapi.Parameter(
+y = OpenApiParameter(
     'y',
-    openapi.IN_PATH,
+    location=OpenApiParameter.PATH,
     description='The 0-based Y position of the tile on the specified Z level.',
-    type=openapi.TYPE_INTEGER,
+    type=OpenApiTypes.INT,
 )
 
 # Style Parameters
-palette = openapi.Parameter(
+palette = OpenApiParameter(
     'palette',
-    openapi.IN_QUERY,
+    location=OpenApiParameter.QUERY,
     description='The color palette to map the band values (named Matplotlib colormaps or palettable palettes). `cmap` alias supported.',
-    type=openapi.TYPE_STRING,
+    type=OpenApiTypes.STR,
 )
-band = openapi.Parameter(
+band = OpenApiParameter(
     'band',
-    openapi.IN_QUERY,
+    location=OpenApiParameter.QUERY,
     description='The band number to use.',
-    type=openapi.TYPE_INTEGER,
+    type=OpenApiTypes.INT,
 )
-vmin = openapi.Parameter(
+vmin = OpenApiParameter(
     'min',
-    openapi.IN_QUERY,
+    location=OpenApiParameter.QUERY,
     description='The minimum value for the color mapping.',
-    type=openapi.TYPE_NUMBER,
+    type=OpenApiTypes.NUMBER,
 )
-vmax = openapi.Parameter(
+vmax = OpenApiParameter(
     'max',
-    openapi.IN_QUERY,
+    location=OpenApiParameter.QUERY,
     description='The maximum value for the color mapping.',
-    type=openapi.TYPE_NUMBER,
+    type=OpenApiTypes.NUMBER,
 )
-nodata = openapi.Parameter(
+nodata = OpenApiParameter(
     'nodata',
-    openapi.IN_QUERY,
+    location=OpenApiParameter.QUERY,
     description='The value to map as no data (often made transparent).',
-    type=openapi.TYPE_NUMBER,
+    type=OpenApiTypes.NUMBER,
 )
-scheme = openapi.Parameter(
+scheme = OpenApiParameter(
     'scheme',
-    openapi.IN_QUERY,
+    location=OpenApiParameter.QUERY,
     description='This is either ``linear`` (the default) or ``discrete``. If a palette is specified, ``linear`` uses a piecewise linear interpolation, and ``discrete`` uses exact colors from the palette with the range of the data mapped into the specified number of colors (e.g., a palette with two colors will split exactly halfway between the min and max values).',
-    type=openapi.TYPE_STRING,
+    type=OpenApiTypes.STR,
 )
-style = openapi.Parameter(
+style = OpenApiParameter(
     'style',
-    openapi.IN_QUERY,
+    location=OpenApiParameter.QUERY,
     description='Encoded string of JSON style following https://girder.github.io/large_image/tilesource_options.html#style',
-    type=openapi.TYPE_STRING,
+    type=OpenApiTypes.STR,
 )
 
 STYLE = [palette, band, vmin, vmax, nodata, scheme, style]
 
 # Region Parameters
-left = openapi.Parameter(
-    'left', openapi.IN_QUERY, description='left', type=openapi.TYPE_NUMBER, required=True
+left = OpenApiParameter(
+    'left',
+    location=OpenApiParameter.QUERY,
+    description='left',
+    type=OpenApiTypes.NUMBER,
+    required=True,
+)
+right = OpenApiParameter(
+    'right',
+    location=OpenApiParameter.QUERY,
+    description='right',
+    type=OpenApiTypes.NUMBER,
+    required=True,
+)
+top = OpenApiParameter(
+    'top',
+    location=OpenApiParameter.QUERY,
+    description='top',
+    type=OpenApiTypes.NUMBER,
+    required=True,
+)
+bottom = OpenApiParameter(
+    'bottom',
+    location=OpenApiParameter.QUERY,
+    description='bottom',
+    type=OpenApiTypes.NUMBER,
+    required=True,
 )
-right = openapi.Parameter(
-    'right', openapi.IN_QUERY, description='right', type=openapi.TYPE_NUMBER, required=True
-)
-top = openapi.Parameter(
-    'top', openapi.IN_QUERY, description='top', type=openapi.TYPE_NUMBER, required=True
-)
-bottom = openapi.Parameter(
-    'bottom', openapi.IN_QUERY, description='bottom', type=openapi.TYPE_NUMBER, required=True
-)
-units = openapi.Parameter(
+units = OpenApiParameter(
     'units',
-    openapi.IN_QUERY,
+    location=OpenApiParameter.QUERY,
     description='The projection/units of the region coordinates.',
-    type=openapi.TYPE_STRING,
+    type=OpenApiTypes.STR,
 )
 
 REGION = [left, right, top, bottom, units, fmt_tiff]
 
 # Histogram Parameters
-only = openapi.Parameter(
+only = OpenApiParameter(
     'onlyMinMax',
-    openapi.IN_QUERY,
-    type=openapi.TYPE_BOOLEAN,
+    location=OpenApiParameter.QUERY,
+    type=OpenApiTypes.BOOL,
     default=False,
 )
-bins = openapi.Parameter(
+bins = OpenApiParameter(
     'bins',
-    openapi.IN_QUERY,
-    type=openapi.TYPE_INTEGER,
+    location=OpenApiParameter.QUERY,
+    type=OpenApiTypes.INT,
     default=256,
 )
-density = openapi.Parameter(
+density = OpenApiParameter(
     'density',
-    openapi.IN_QUERY,
-    type=openapi.TYPE_BOOLEAN,
+    location=OpenApiParameter.QUERY,
+    type=OpenApiTypes.BOOL,
     default=False,
 )
-format = openapi.Parameter(
+format = OpenApiParameter(
     'format',
-    openapi.IN_QUERY,
-    type=openapi.TYPE_STRING,
+    location=OpenApiParameter.QUERY,
+    type=OpenApiTypes.STR,
 )
 
 HISTOGRAM = [only, bins, density, format]
 
 
 # Thumbnail Parameters
-max_width = openapi.Parameter(
+max_width = OpenApiParameter(
     'max_width',
-    openapi.IN_QUERY,
+    location=OpenApiParameter.QUERY,
     description='maximum width in pixels.',
-    type=openapi.TYPE_INTEGER,
+    type=OpenApiTypes.INT,
     default=256,
 )
-max_height = openapi.Parameter(
+max_height = OpenApiParameter(
     'max_height',
-    openapi.IN_QUERY,
+    location=OpenApiParameter.QUERY,
     description='maximum height in pixels.',
-    type=openapi.TYPE_INTEGER,
+    type=OpenApiTypes.INT,
     default=256,
 )
 
 THUMBNAIL = [fmt_png, max_height, max_width]
```

### Comparing `django-large-image-0.8.2/django_large_image/rest/renderers.py` & `django-large-image-0.9.0/django_large_image/rest/renderers.py`

 * *Files identical despite different names*

### Comparing `django-large-image-0.8.2/django_large_image/rest/serializers.py` & `django-large-image-0.9.0/django_large_image/rest/serializers.py`

 * *Files identical despite different names*

### Comparing `django-large-image-0.8.2/django_large_image/rest/standalone.py` & `django-large-image-0.9.0/django_large_image/rest/standalone.py`

 * *Files identical despite different names*

### Comparing `django-large-image-0.8.2/django_large_image/rest/tiles.py` & `django-large-image-0.9.0/django_large_image/rest/tiles.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.http import HttpResponse
-from drf_yasg.utils import swagger_auto_schema
+from drf_spectacular.utils import extend_schema
 from large_image.exceptions import TileSourceXYZRangeError
 from rest_framework.decorators import action
 from rest_framework.exceptions import ValidationError
 from rest_framework.request import Request
 from rest_framework.response import Response
 
 from django_large_image import tilesource
@@ -17,30 +17,30 @@
 tile_summary = 'Returns tile image binary.'
 tile_parameters = params.BASE + [params.z, params.x, params.y, params.fmt_png] + params.STYLE
 tile_corners_summary = 'Returns bounds of a tile for a given x, y, z index.'
 tile_corners_parameters = params.BASE + [params.z, params.x, params.y]
 
 
 class TilesMixin(LargeImageMixinBase):
-    @swagger_auto_schema(
-        method='GET',
-        operation_summary=tile_metadata_summary,
-        manual_parameters=tile_metadata_parameters,
+    @extend_schema(
+        methods=['GET'],
+        summary=tile_metadata_summary,
+        parameters=tile_metadata_parameters,
     )
     @action(detail=False, url_path=r'tiles/metadata')
     def tiles_metadata(self, request: Request, pk: int = None, **kwargs) -> Response:
         source = self.get_tile_source(request, pk, style=False)
         source.dli_geospatial = tilesource.is_geospatial(source)
         serializer = TileMetadataSerializer(source)
         return Response(serializer.data)
 
-    @swagger_auto_schema(
-        method='GET',
-        operation_summary=tile_summary,
-        manual_parameters=tile_parameters,
+    @extend_schema(
+        methods=['GET'],
+        summary=tile_summary,
+        parameters=tile_parameters,
     )
     @action(
         detail=False,
         url_path=rf'tiles/(?P<z>\d+)/(?P<x>\d+)/(?P<y>\d+).{params.FORMAT_URL_PATTERN}',
         renderer_classes=image_renderers,
     )
     def tile(
@@ -51,18 +51,18 @@
         try:
             tile_binary = source.getTile(int(x), int(y), int(z))
         except TileSourceXYZRangeError as e:
             raise ValidationError(e)
         mime_type = source.getTileMimeType()
         return HttpResponse(tile_binary, content_type=mime_type)
 
-    @swagger_auto_schema(
-        method='GET',
-        operation_summary=tile_corners_summary,
-        manual_parameters=tile_corners_parameters,
+    @extend_schema(
+        methods=['GET'],
+        summary=tile_corners_summary,
+        parameters=tile_corners_parameters,
     )
     @action(
         detail=False, methods=['get'], url_path=r'tiles/(?P<z>\d+)/(?P<x>\d+)/(?P<y>\d+)/corners'
     )
     def tile_corners(
         self, request: Request, x: int, y: int, z: int, pk: int = None, **kwargs
     ) -> HttpResponse:
@@ -75,42 +75,42 @@
             'ymax': ymax,
             'proj4': source.getProj4String(),
         }
         return Response(metadata)
 
 
 class TilesDetailMixin(TilesMixin):
-    @swagger_auto_schema(
-        method='GET',
-        operation_summary=tile_metadata_summary,
-        manual_parameters=tile_metadata_parameters,
+    @extend_schema(
+        methods=['GET'],
+        summary=tile_metadata_summary,
+        parameters=tile_metadata_parameters,
     )
     @action(detail=True, url_path=r'tiles/metadata')
     def tiles_metadata(self, request: Request, pk: int = None, **kwargs) -> Response:
         return super().tiles_metadata(request, pk)
 
-    @swagger_auto_schema(
-        method='GET',
-        operation_summary=tile_summary,
-        manual_parameters=tile_parameters,
+    @extend_schema(
+        methods=['GET'],
+        summary=tile_summary,
+        parameters=tile_parameters,
     )
     @action(
         detail=True,
         url_path=rf'tiles/(?P<z>\d+)/(?P<x>\d+)/(?P<y>\d+).{params.FORMAT_URL_PATTERN}',
         renderer_classes=image_renderers,
     )
     def tile(
         self, request: Request, x: int, y: int, z: int, pk: int = None, fmt: str = 'png', **kwargs
     ) -> HttpResponse:
         return super().tile(request, x, y, z, pk, fmt)
 
-    @swagger_auto_schema(
-        method='GET',
-        operation_summary=tile_corners_summary,
-        manual_parameters=tile_corners_parameters,
+    @extend_schema(
+        methods=['GET'],
+        summary=tile_corners_summary,
+        parameters=tile_corners_parameters,
     )
     @action(
         detail=True, methods=['get'], url_path=r'tiles/(?P<z>\d+)/(?P<x>\d+)/(?P<y>\d+)/corners'
     )
     def tile_corners(
         self, request: Request, x: int, y: int, z: int, pk: int = None, **kwargs
     ) -> HttpResponse:
```

### Comparing `django-large-image-0.8.2/django_large_image/rest/viewsets.py` & `django-large-image-0.9.0/django_large_image/rest/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-large-image-0.8.2/django_large_image/static/django_large_image/js/cesium.js` & `django-large-image-0.9.0/django_large_image/static/django_large_image/js/cesium.js`

 * *Files identical despite different names*

### Comparing `django-large-image-0.8.2/django_large_image/static/django_large_image/js/geojs/1.8.3/geo.min.js` & `django-large-image-0.9.0/django_large_image/static/django_large_image/js/geojs/1.8.3/geo.min.js`

 * *Files identical despite different names*

### Comparing `django-large-image-0.8.2/django_large_image/templates/admin/django_large_image/_include/geojs.html` & `django-large-image-0.9.0/django_large_image/templates/admin/django_large_image/_include/geojs.html`

 * *Files identical despite different names*

### Comparing `django-large-image-0.8.2/django_large_image/templates/django_large_image/_include/base.html` & `django-large-image-0.9.0/django_large_image/templates/django_large_image/_include/base.html`

 * *Files identical despite different names*

### Comparing `django-large-image-0.8.2/django_large_image/templates/django_large_image/_include/cesium.html` & `django-large-image-0.9.0/django_large_image/templates/django_large_image/_include/cesium.html`

 * *Files identical despite different names*

### Comparing `django-large-image-0.8.2/django_large_image/templates/django_large_image/_include/colors.html` & `django-large-image-0.9.0/django_large_image/templates/django_large_image/_include/colors.html`

 * *Files identical despite different names*

### Comparing `django-large-image-0.8.2/django_large_image/templates/django_large_image/_include/geojs.html` & `django-large-image-0.9.0/django_large_image/templates/django_large_image/_include/geojs.html`

 * *Files identical despite different names*

### Comparing `django-large-image-0.8.2/django_large_image/templates/django_large_image/base.html` & `django-large-image-0.9.0/django_large_image/templates/django_large_image/base.html`

 * *Files identical despite different names*

### Comparing `django-large-image-0.8.2/django_large_image/tilesource.py` & `django-large-image-0.9.0/django_large_image/tilesource.py`

 * *Files identical despite different names*

### Comparing `django-large-image-0.8.2/django_large_image/utilities.py` & `django-large-image-0.9.0/django_large_image/utilities.py`

 * *Files identical despite different names*

### Comparing `django-large-image-0.8.2/django_large_image.egg-info/PKG-INFO` & `django-large-image-0.9.0/django_large_image.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-large-image
-Version: 0.8.2
+Version: 0.9.0
 Summary: Dynamic tile server in Django built on top of large-image (and GDAL)
 Home-page: https://github.com/girder/django-large-image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-large-image Version: 0.8.2 Summary: Dynamic
+Metadata-Version: 2.1 Name: django-large-image Version: 0.9.0 Summary: Dynamic
 tile server in Django built on top of large-image (and GDAL) Home-page: https:/
 /github.com/girder/django-large-image Author: Kitware, Inc. Author-email:
 kitware@kitware.com License: Apache 2.0 Platform: UNKNOWN Classifier:
 Development Status :: 3 - Alpha Classifier: Environment :: Web Environment
 Classifier: Framework :: Django :: 3.0 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: OS Independent
```

### Comparing `django-large-image-0.8.2/django_large_image.egg-info/SOURCES.txt` & `django-large-image-0.9.0/django_large_image.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-large-image-0.8.2/pyproject.toml` & `django-large-image-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-large-image-0.8.2/setup.py` & `django-large-image-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         long_description = f.read()
 else:
     # When this is first installed in development Docker, README.md is not available
     long_description = ''
 
 setup(
     name='django-large-image',
-    version='0.8.2',
+    version='0.9.0',
     description='Dynamic tile server in Django built on top of large-image (and GDAL)',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='Apache 2.0',
     author='Kitware, Inc.',
     author_email='kitware@kitware.com',
     url='https://github.com/girder/django-large-image',
@@ -36,15 +36,15 @@
     ],
     python_requires='>=3.8',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'django',
         'djangorestframework',
-        'drf-yasg',
+        'drf-spectacular',
         'filelock',
         'large-image>=1.16.2',
     ],
     extras_require={
         'colormaps': [
             'matplotlib',
             'cmocean',
```

