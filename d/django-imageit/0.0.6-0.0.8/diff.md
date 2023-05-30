# Comparing `tmp/django-imageit-0.0.6.tar.gz` & `tmp/django-imageit-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-imageit-0.0.6.tar", last modified: Tue Jun 22 16:21:56 2021, max compression
+gzip compressed data, was "django-imageit-0.0.8.tar", last modified: Tue May 30 11:22:55 2023, max compression
```

## Comparing `django-imageit-0.0.6.tar` & `django-imageit-0.0.8.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 16:21:56.578150 django-imageit-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2021-06-22 16:21:36.000000 django-imageit-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      187 2021-06-22 16:21:36.000000 django-imageit-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6170 2021-06-22 16:21:56.578150 django-imageit-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4283 2021-06-22 16:21:36.000000 django-imageit-0.0.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 16:21:56.574150 django-imageit-0.0.6/django_imageit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6170 2021-06-22 16:21:56.000000 django-imageit-0.0.6/django_imageit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      756 2021-06-22 16:21:56.000000 django-imageit-0.0.6/django_imageit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-22 16:21:56.000000 django-imageit-0.0.6/django_imageit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       56 2021-06-22 16:21:56.000000 django-imageit-0.0.6/django_imageit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-06-22 16:21:56.000000 django-imageit-0.0.6/django_imageit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 16:21:56.578150 django-imageit-0.0.6/imageit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-06-22 16:21:36.000000 django-imageit-0.0.6/imageit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2021-06-22 16:21:36.000000 django-imageit-0.0.6/imageit/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      118 2021-06-22 16:21:36.000000 django-imageit-0.0.6/imageit/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     3260 2021-06-22 16:21:36.000000 django-imageit-0.0.6/imageit/fields.py
--rw-r--r--   0 runner    (1001) docker     (121)      437 2021-06-22 16:21:36.000000 django-imageit-0.0.6/imageit/filetypes.py
--rw-r--r--   0 runner    (1001) docker     (121)     3504 2021-06-22 16:21:36.000000 django-imageit-0.0.6/imageit/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2021-06-22 16:21:36.000000 django-imageit-0.0.6/imageit/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 16:21:56.574150 django-imageit-0.0.6/imageit/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 16:21:56.574150 django-imageit-0.0.6/imageit/static/imageit/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 16:21:56.574150 django-imageit-0.0.6/imageit/static/imageit/dist/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 16:21:56.578150 django-imageit-0.0.6/imageit/static/imageit/dist/css/
--rw-r--r--   0 runner    (1001) docker     (121)     2459 2021-06-22 16:21:55.000000 django-imageit-0.0.6/imageit/static/imageit/dist/css/imageit.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 16:21:56.578150 django-imageit-0.0.6/imageit/static/imageit/dist/img/
--rw-r--r--   0 runner    (1001) docker     (121)     1145 2021-06-22 16:21:55.000000 django-imageit-0.0.6/imageit/static/imageit/dist/img/folder.svg
--rw-r--r--   0 runner    (1001) docker     (121)      616 2021-06-22 16:21:55.000000 django-imageit-0.0.6/imageit/static/imageit/dist/img/image-icon.svg
--rw-r--r--   0 runner    (1001) docker     (121)     2046 2021-06-22 16:21:55.000000 django-imageit-0.0.6/imageit/static/imageit/dist/img/upload.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 16:21:56.578150 django-imageit-0.0.6/imageit/static/imageit/dist/js/
--rw-r--r--   0 runner    (1001) docker     (121)    39524 2021-06-22 16:21:55.000000 django-imageit-0.0.6/imageit/static/imageit/dist/js/imageit.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 16:21:56.574150 django-imageit-0.0.6/imageit/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 16:21:56.574150 django-imageit-0.0.6/imageit/templates/imageit/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-22 16:21:56.578150 django-imageit-0.0.6/imageit/templates/imageit/widgets/
--rw-r--r--   0 runner    (1001) docker     (121)      203 2021-06-22 16:21:36.000000 django-imageit-0.0.6/imageit/templates/imageit/widgets/crop_it_widget.html
--rw-r--r--   0 runner    (1001) docker     (121)     1680 2021-06-22 16:21:36.000000 django-imageit-0.0.6/imageit/templates/imageit/widgets/scale_it_widget.html
--rw-r--r--   0 runner    (1001) docker     (121)     7014 2021-06-22 16:21:36.000000 django-imageit-0.0.6/imageit/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       63 2021-06-22 16:21:36.000000 django-imageit-0.0.6/imageit/views.py
--rw-r--r--   0 runner    (1001) docker     (121)     1990 2021-06-22 16:21:36.000000 django-imageit-0.0.6/imageit/widgets.py
--rw-r--r--   0 runner    (1001) docker     (121)      496 2021-06-22 16:21:36.000000 django-imageit-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-22 16:21:56.578150 django-imageit-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1488 2021-06-22 16:21:36.000000 django-imageit-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:55.364229 django-imageit-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-30 11:22:27.000000 django-imageit-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-30 11:22:27.000000 django-imageit-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-05-30 11:22:55.364229 django-imageit-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-05-30 11:22:27.000000 django-imageit-0.0.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:55.360229 django-imageit-0.0.8/django_imageit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-05-30 11:22:55.000000 django-imageit-0.0.8/django_imageit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-30 11:22:55.000000 django-imageit-0.0.8/django_imageit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:22:55.000000 django-imageit-0.0.8/django_imageit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-30 11:22:55.000000 django-imageit-0.0.8/django_imageit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-30 11:22:55.000000 django-imageit-0.0.8/django_imageit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:55.364229 django-imageit-0.0.8/imageit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:27.000000 django-imageit-0.0.8/imageit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-30 11:22:27.000000 django-imageit-0.0.8/imageit/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-30 11:22:27.000000 django-imageit-0.0.8/imageit/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-05-30 11:22:27.000000 django-imageit-0.0.8/imageit/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-30 11:22:27.000000 django-imageit-0.0.8/imageit/filetypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-30 11:22:27.000000 django-imageit-0.0.8/imageit/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-30 11:22:27.000000 django-imageit-0.0.8/imageit/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:55.356229 django-imageit-0.0.8/imageit/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:55.356229 django-imageit-0.0.8/imageit/static/imageit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:55.356229 django-imageit-0.0.8/imageit/static/imageit/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:55.364229 django-imageit-0.0.8/imageit/static/imageit/dist/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-05-30 11:22:54.000000 django-imageit-0.0.8/imageit/static/imageit/dist/css/imageit.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:55.364229 django-imageit-0.0.8/imageit/static/imageit/dist/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-30 11:22:54.000000 django-imageit-0.0.8/imageit/static/imageit/dist/img/folder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-30 11:22:54.000000 django-imageit-0.0.8/imageit/static/imageit/dist/img/image-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-30 11:22:54.000000 django-imageit-0.0.8/imageit/static/imageit/dist/img/upload.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:55.364229 django-imageit-0.0.8/imageit/static/imageit/dist/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    39524 2023-05-30 11:22:54.000000 django-imageit-0.0.8/imageit/static/imageit/dist/js/imageit.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:55.360229 django-imageit-0.0.8/imageit/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:55.360229 django-imageit-0.0.8/imageit/templates/imageit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:22:55.364229 django-imageit-0.0.8/imageit/templates/imageit/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-30 11:22:27.000000 django-imageit-0.0.8/imageit/templates/imageit/widgets/crop_it_widget.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-30 11:22:27.000000 django-imageit-0.0.8/imageit/templates/imageit/widgets/scale_it_widget.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-05-30 11:22:27.000000 django-imageit-0.0.8/imageit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-30 11:22:27.000000 django-imageit-0.0.8/imageit/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-30 11:22:27.000000 django-imageit-0.0.8/imageit/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-30 11:22:27.000000 django-imageit-0.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 11:22:55.364229 django-imageit-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-30 11:22:27.000000 django-imageit-0.0.8/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 11:22:27.000000 django-imageit-0.0.8/version.txt
```

### Comparing `django-imageit-0.0.6/LICENSE` & `django-imageit-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django-imageit-0.0.6/PKG-INFO` & `django-imageit-0.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: django-imageit
-Version: 0.0.6
-Summary: Image processing plugin built for Django
+Version: 0.0.8
+Summary: Image upload & processing plugin built for Django
 Home-page: https://github.com/byite/django-imageit
 Author: Scott James
 Author-email: scottjames@byitegroup.com
 License: UNKNOWN
 Description: ================
         Django ImageIt
         ================
@@ -22,28 +22,23 @@
         * Crop images to user defined dimensions before being scaled.
         * Option to upscale smaller images.
         * Utilises cropper.js.
         * Accepts .svg images.
         * Django Admin support.
         
         
-        Documentation
-        =============
-        https://django-imageit.readthedocs.io/en/latest/
-        
-        
         Usage
         ============
         * Install django-imageit using pip
             .. code-block:: shell
         
                 pip install django-imageit
         
         
-        * Add 'imageit to INSTALLED_APPS in your settings.py
+        * Add 'imageit' to INSTALLED_APPS in your settings.py
             .. code-block:: python
         
                 INSTALLED_APPS = [
                     ...
                     'imageit',
                     ...
                 ]
```

### Comparing `django-imageit-0.0.6/README.rst` & `django-imageit-0.0.8/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -14,28 +14,23 @@
 * Crop images to user defined dimensions before being scaled.
 * Option to upscale smaller images.
 * Utilises cropper.js.
 * Accepts .svg images.
 * Django Admin support.
 
 
-Documentation
-=============
-https://django-imageit.readthedocs.io/en/latest/
-
-
 Usage
 ============
 * Install django-imageit using pip
     .. code-block:: shell
 
         pip install django-imageit
 
 
-* Add 'imageit to INSTALLED_APPS in your settings.py
+* Add 'imageit' to INSTALLED_APPS in your settings.py
     .. code-block:: python
 
         INSTALLED_APPS = [
             ...
             'imageit',
             ...
         ]
```

### Comparing `django-imageit-0.0.6/django_imageit.egg-info/PKG-INFO` & `django-imageit-0.0.8/django_imageit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: django-imageit
-Version: 0.0.6
-Summary: Image processing plugin built for Django
+Version: 0.0.8
+Summary: Image upload & processing plugin built for Django
 Home-page: https://github.com/byite/django-imageit
 Author: Scott James
 Author-email: scottjames@byitegroup.com
 License: UNKNOWN
 Description: ================
         Django ImageIt
         ================
@@ -22,28 +22,23 @@
         * Crop images to user defined dimensions before being scaled.
         * Option to upscale smaller images.
         * Utilises cropper.js.
         * Accepts .svg images.
         * Django Admin support.
         
         
-        Documentation
-        =============
-        https://django-imageit.readthedocs.io/en/latest/
-        
-        
         Usage
         ============
         * Install django-imageit using pip
             .. code-block:: shell
         
                 pip install django-imageit
         
         
-        * Add 'imageit to INSTALLED_APPS in your settings.py
+        * Add 'imageit' to INSTALLED_APPS in your settings.py
             .. code-block:: python
         
                 INSTALLED_APPS = [
                     ...
                     'imageit',
                     ...
                 ]
```

### Comparing `django-imageit-0.0.6/django_imageit.egg-info/SOURCES.txt` & `django-imageit-0.0.8/django_imageit.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 MANIFEST.in
 README.rst
 requirements.txt
 setup.py
+version.txt
 django_imageit.egg-info/PKG-INFO
 django_imageit.egg-info/SOURCES.txt
 django_imageit.egg-info/dependency_links.txt
 django_imageit.egg-info/requires.txt
 django_imageit.egg-info/top_level.txt
 imageit/__init__.py
 imageit/admin.py
```

### Comparing `django-imageit-0.0.6/imageit/fields.py` & `django-imageit-0.0.8/imageit/fields.py`

 * *Files identical despite different names*

### Comparing `django-imageit-0.0.6/imageit/models.py` & `django-imageit-0.0.8/imageit/models.py`

 * *Files identical despite different names*

### Comparing `django-imageit-0.0.6/imageit/settings.py` & `django-imageit-0.0.8/imageit/settings.py`

 * *Files identical despite different names*

### Comparing `django-imageit-0.0.6/imageit/static/imageit/dist/css/imageit.css` & `django-imageit-0.0.8/imageit/static/imageit/dist/css/imageit.css`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-.imageit-container{display:flex;flex-direction:column;width:100%}.imageit-pseudo-selector{background-color:#79aec8;border:1px solid #49a4d1;border-radius:4px;color:#fff;cursor:pointer;display:none;font-weight:600;padding:.5rem 1.5rem!important;text-align:center;width:calc(100% - 3rem - 2px)!important}.imageit-selector-icon{height:1.5em;margin-right:1.5em}.imageit-preview{margin:1.5rem 0;max-width:100%;min-height:75px;padding:0 .5rem}.imageit-preview-content{align-items:center;display:flex;justify-content:space-between;width:100%}.imageit-clear-button{border:2px solid #ff3466;border-radius:50%;color:#ff3466;height:2rem;width:2rem}.imageit-clear-button,.imageit-undo-button{align-items:center;cursor:pointer;display:flex;justify-content:center}.imageit-undo-button{background-color:#79aec8;border:1px solid #49a4d1;border-radius:4px;color:#fff;padding:.5rem 1.5rem!important}.imageit-text-light{color:#a4b7bd}.imageit-inactive{display:none}.imageit-error{color:#ff3466;padding:1rem 0;text-align:center;width:100%}.imageit-preview-text{flex-grow:1;flex-shrink:100;padding:0 1rem}.imageit-preview-text p{word-break:break-all}.imageit-preview-image{box-shadow:2px 2px 5px rgba(0,0,0,.4);max-height:150px;max-width:150px}.imageit-preview-cropit-content{align-items:center;flex-direction:column;justify-content:space-between}.imageit-cropit-container{width:100%}.imageit-cropper-content{display:flex;flex-direction:column;max-width:100%;min-height:75px}.imageit-cropper-image-container{max-height:80vh}.imageit-cropper-image{max-height:100%;max-width:100%}.imageit-clear-button.imageit-cancel-crop{border:2px solid #ff3466;border-radius:4px;color:#ff3466;cursor:pointer;height:2rem;margin-bottom:1.5rem;text-align:center;width:calc(100% - 4px)}.loading{opacity:.5;position:relative}.loading:before{border-radius:5px;content:"";display:flex;height:110%;left:-5%;position:absolute;top:-5%;width:110%}.loading:after{animation:rotate 3s ease-in-out infinite;border-color:#ff0 #ff0 transparent transparent;border-radius:50%;border-style:solid;box-sizing:border-box;height:70px;left:calc(50% - 35px);position:absolute;top:calc(50% - 35px);transform:rotate(-200deg);width:70px}@keyframes rotate{0%{border-right-color:#ff0;border-top-color:#ff0;border-width:10px}25%{border-width:3px}50%{border-right-color:pink;border-top-color:pink;border-width:10px;transform:rotate(115deg)}75%{border-width:3px}to{border-right-color:#ff0;border-top-color:#ff0;border-width:10px}}
+.imageit-container{display:flex;flex-direction:column;width:100%}.imageit-pseudo-selector{background-color:#79aec8;border:1px solid #49a4d1;border-radius:4px;color:#fff;cursor:pointer;display:none;font-weight:600;padding:.5rem 1.5rem!important;text-align:center;width:calc(100% - 2px)!important}.imageit-selector-icon{height:1.5em;margin-right:1.5em}.imageit-preview{margin:1.5rem 0;max-width:100%;min-height:75px;padding:0 .5rem}.imageit-preview-content{align-items:center;display:flex;justify-content:space-between;width:100%}.imageit-clear-button{border:2px solid #ff3466;border-radius:50%;color:#ff3466;height:2rem;width:2rem}.imageit-clear-button,.imageit-undo-button{align-items:center;cursor:pointer;display:flex;justify-content:center}.imageit-undo-button{background-color:#79aec8;border:1px solid #49a4d1;border-radius:4px;color:#fff;padding:.5rem 1.5rem!important}.imageit-text-light{color:#a4b7bd}.imageit-inactive{display:none}.imageit-error{color:#ff3466;padding:1rem 0;text-align:center;width:100%}.imageit-preview-text{flex-grow:1;flex-shrink:100;padding:0 1rem}.imageit-preview-text p{word-break:break-all}.imageit-preview-image{box-shadow:2px 2px 5px rgba(0,0,0,.4);max-height:150px;max-width:150px}.imageit-preview-cropit-content{align-items:center;flex-direction:column;justify-content:space-between}.imageit-cropit-container{width:100%}.imageit-cropper-content{display:flex;flex-direction:column;max-width:100%;min-height:75px}.imageit-cropper-image-container{max-height:80vh}.imageit-cropper-image{max-height:100%;max-width:100%}.imageit-clear-button.imageit-cancel-crop{border:2px solid #ff3466;border-radius:4px;color:#ff3466;cursor:pointer;height:2rem;margin-bottom:1.5rem;text-align:center;width:calc(100% - 4px)}.loading{opacity:.5;position:relative}.loading:before{border-radius:5px;content:"";display:flex;height:110%;left:-5%;position:absolute;top:-5%;width:110%}.loading:after{animation:rotate 3s ease-in-out infinite;border-color:#ff0 #ff0 transparent transparent;border-radius:50%;border-style:solid;box-sizing:border-box;height:70px;left:calc(50% - 35px);position:absolute;top:calc(50% - 35px);transform:rotate(-200deg);width:70px}@keyframes rotate{0%{border-right-color:#ff0;border-top-color:#ff0;border-width:10px}25%{border-width:3px}50%{border-right-color:pink;border-top-color:pink;border-width:10px;transform:rotate(115deg)}75%{border-width:3px}to{border-right-color:#ff0;border-top-color:#ff0;border-width:10px}}
```

### Comparing `django-imageit-0.0.6/imageit/static/imageit/dist/img/folder.svg` & `django-imageit-0.0.8/imageit/static/imageit/dist/img/folder.svg`

 * *Files identical despite different names*

### Comparing `django-imageit-0.0.6/imageit/static/imageit/dist/img/image-icon.svg` & `django-imageit-0.0.8/imageit/static/imageit/dist/img/image-icon.svg`

 * *Files identical despite different names*

### Comparing `django-imageit-0.0.6/imageit/static/imageit/dist/img/upload.svg` & `django-imageit-0.0.8/imageit/static/imageit/dist/img/upload.svg`

 * *Files identical despite different names*

### Comparing `django-imageit-0.0.6/imageit/static/imageit/dist/js/imageit.js` & `django-imageit-0.0.8/imageit/static/imageit/dist/js/imageit.js`

 * *Files identical despite different names*

### Comparing `django-imageit-0.0.6/imageit/templates/imageit/widgets/scale_it_widget.html` & `django-imageit-0.0.8/imageit/templates/imageit/widgets/scale_it_widget.html`

 * *Files identical despite different names*

### Comparing `django-imageit-0.0.6/imageit/utils.py` & `django-imageit-0.0.8/imageit/utils.py`

 * *Files identical despite different names*

### Comparing `django-imageit-0.0.6/imageit/widgets.py` & `django-imageit-0.0.8/imageit/widgets.py`

 * *Files identical despite different names*

### Comparing `django-imageit-0.0.6/setup.py` & `django-imageit-0.0.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,23 @@
+import os
 from setuptools import setup
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 
+with open("version.txt", "r") as version_file:
+    version = version_file.read().strip()
+
 setup(
     name='django-imageit',
-    version='0.0.6',
+    version=version,
     url="https://github.com/byite/django-imageit",
     author="Scott James",
     author_email="scottjames@byitegroup.com",
-    description="Image processing plugin built for Django",
+    description="Image upload & processing plugin built for Django",
     packages=['imageit'],
     include_package_data=True,
     long_description=long_description,
     long_description_content_type="text/x-rst",
 
     install_requires = [
         "django >= 3",
```

