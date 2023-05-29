# Comparing `tmp/xblock-utils-3.0.0.tar.gz` & `tmp/xblock-utils-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xblock-utils-3.0.0.tar", last modified: Tue Feb 22 10:12:12 2022, max compression
+gzip compressed data, was "xblock-utils-3.1.0.tar", last modified: Mon May 29 23:23:17 2023, max compression
```

## Comparing `xblock-utils-3.0.0.tar` & `xblock-utils-3.1.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 10:12:12.392373 xblock-utils-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)    34500 2022-02-22 10:11:58.000000 xblock-utils-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-02-22 10:11:58.000000 xblock-utils-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9531 2022-02-22 10:12:12.392373 xblock-utils-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7346 2022-02-22 10:11:58.000000 xblock-utils-3.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 10:12:12.388373 xblock-utils-3.0.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-02-22 10:11:58.000000 xblock-utils-3.0.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-02-22 10:12:12.392373 xblock-utils-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3699 2022-02-22 10:11:58.000000 xblock-utils-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 10:12:12.388373 xblock-utils-3.0.0/xblock_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9531 2022-02-22 10:12:11.000000 xblock-utils-3.0.0/xblock_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      735 2022-02-22 10:12:12.000000 xblock-utils-3.0.0/xblock_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-22 10:12:11.000000 xblock-utils-3.0.0/xblock_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-02-22 10:12:11.000000 xblock-utils-3.0.0/xblock_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-02-22 10:12:11.000000 xblock-utils-3.0.0/xblock_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 10:12:12.388373 xblock-utils-3.0.0/xblockutils/
--rw-r--r--   0 runner    (1001) docker     (121)       97 2022-02-22 10:11:58.000000 xblock-utils-3.0.0/xblockutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7680 2022-02-22 10:11:58.000000 xblock-utils-3.0.0/xblockutils/base_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      894 2022-02-22 10:11:58.000000 xblock-utils-3.0.0/xblockutils/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 10:12:12.388373 xblock-utils-3.0.0/xblockutils/public/
--rw-r--r--   0 runner    (1001) docker     (121)     2357 2022-02-22 10:11:58.000000 xblock-utils-3.0.0/xblockutils/public/studio_container.js
--rw-r--r--   0 runner    (1001) docker     (121)     7605 2022-02-22 10:11:58.000000 xblock-utils-3.0.0/xblockutils/public/studio_edit.js
--rw-r--r--   0 runner    (1001) docker     (121)     2062 2022-02-22 10:11:58.000000 xblock-utils-3.0.0/xblockutils/publish_event.py
--rw-r--r--   0 runner    (1001) docker     (121)     4875 2022-02-22 10:11:58.000000 xblock-utils-3.0.0/xblockutils/resources.py
--rw-r--r--   0 runner    (1001) docker     (121)     3526 2022-02-22 10:11:58.000000 xblock-utils-3.0.0/xblockutils/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)    22121 2022-02-22 10:11:58.000000 xblock-utils-3.0.0/xblockutils/studio_editable.py
--rw-r--r--   0 runner    (1001) docker     (121)     3327 2022-02-22 10:11:58.000000 xblock-utils-3.0.0/xblockutils/studio_editable_test.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 10:12:12.388373 xblock-utils-3.0.0/xblockutils/templates/
--rw-r--r--   0 runner    (1001) docker     (121)      809 2022-02-22 10:11:58.000000 xblock-utils-3.0.0/xblockutils/templates/add_buttons.html
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-02-22 10:11:58.000000 xblock-utils-3.0.0/xblockutils/templates/default_preview_view.html
--rw-r--r--   0 runner    (1001) docker     (121)     5584 2022-02-22 10:11:58.000000 xblock-utils-3.0.0/xblockutils/templates/studio_edit.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 10:12:12.388373 xblock-utils-3.0.0/xblockutils/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-22 10:11:58.000000 xblock-utils-3.0.0/xblockutils/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2256 2022-02-22 10:11:58.000000 xblock-utils-3.0.0/xblockutils/templatetags/i18n.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 23:23:17.445969 xblock-utils-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    34500 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    15928 2023-05-29 23:23:17.445969 xblock-utils-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    12387 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 23:23:17.441969 xblock-utils-3.1.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      164 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      225 2023-05-29 23:23:17.445969 xblock-utils-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3703 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 23:23:17.445969 xblock-utils-3.1.0/xblock_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    15928 2023-05-29 23:23:17.000000 xblock-utils-3.1.0/xblock_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-05-29 23:23:17.000000 xblock-utils-3.1.0/xblock_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 23:23:17.000000 xblock-utils-3.1.0/xblock_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-05-29 23:23:17.000000 xblock-utils-3.1.0/xblock_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-29 23:23:17.000000 xblock-utils-3.1.0/xblock_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 23:23:17.445969 xblock-utils-3.1.0/xblockutils/
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/xblockutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7680 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/xblockutils/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/xblockutils/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 23:23:17.445969 xblock-utils-3.1.0/xblockutils/public/
+-rw-r--r--   0 runner    (1001) docker     (122)     2357 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/xblockutils/public/studio_container.js
+-rw-r--r--   0 runner    (1001) docker     (122)     7605 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/xblockutils/public/studio_edit.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2062 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/xblockutils/publish_event.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4875 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/xblockutils/resources.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3526 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/xblockutils/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22344 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/xblockutils/studio_editable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3327 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/xblockutils/studio_editable_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 23:23:17.445969 xblock-utils-3.1.0/xblockutils/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      809 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/xblockutils/templates/add_buttons.html
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/xblockutils/templates/default_preview_view.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5584 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/xblockutils/templates/studio_edit.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 23:23:17.445969 xblock-utils-3.1.0/xblockutils/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/xblockutils/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2256 2023-05-29 23:23:15.000000 xblock-utils-3.1.0/xblockutils/templatetags/i18n.py
```

### Comparing `xblock-utils-3.0.0/LICENSE` & `xblock-utils-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.0.0/setup.py` & `xblock-utils-3.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     author='edX',
     author_email='oscm@edx.org',
     packages=[
         'xblockutils',
     ],
     install_requires=load_requirements('requirements/base.in'),
     package_data=package_data("xblockutils", ["public", "templates", "templatetags"]),
-    url='https://github.com/edx/xblock-utils',
+    url='https://github.com/openedx/xblock-utils',
     classifiers=[
         'Framework :: Django :: 3.2',
         'Framework :: Django :: 4.0',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: Implementation :: CPython',
```

### Comparing `xblock-utils-3.0.0/xblock_utils.egg-info/SOURCES.txt` & `xblock-utils-3.1.0/xblock_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.0.0/xblockutils/base_test.py` & `xblock-utils-3.1.0/xblockutils/base_test.py`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.0.0/xblockutils/helpers.py` & `xblock-utils-3.1.0/xblockutils/helpers.py`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.0.0/xblockutils/public/studio_container.js` & `xblock-utils-3.1.0/xblockutils/public/studio_container.js`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.0.0/xblockutils/public/studio_edit.js` & `xblock-utils-3.1.0/xblockutils/public/studio_edit.js`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.0.0/xblockutils/publish_event.py` & `xblock-utils-3.1.0/xblockutils/publish_event.py`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.0.0/xblockutils/resources.py` & `xblock-utils-3.1.0/xblockutils/resources.py`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.0.0/xblockutils/settings.py` & `xblock-utils-3.1.0/xblockutils/settings.py`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.0.0/xblockutils/studio_editable.py` & `xblock-utils-3.1.0/xblockutils/studio_editable.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # Imports ###########################################################
 
 
 import logging
 import simplejson as json
 
-from xblock.core import XBlock
+from xblock.core import XBlock, XBlockMixin
 from xblock.fields import Scope, JSONField, List, Integer, Float, Boolean, String, DateTime
 from xblock.exceptions import JsonHandlerError, NoSuchViewError
 from web_fragments.fragment import Fragment
 from xblock.validation import Validation
 
 from xblockutils.resources import ResourceLoader
 
@@ -265,15 +265,16 @@
         only for validation not related to this block's field values.
         """
         validation = super().validate()
         self.validate_field_data(validation, self)
         return validation
 
 
-class StudioContainerXBlockMixin:
+@XBlock.needs('mako')
+class StudioContainerXBlockMixin(XBlockMixin):
     """
     An XBlock mixin to provide convenient use of an XBlock in Studio
     that wants to allow the user to assign children to it.
     """
     has_author_view = True  # Without this flag, studio will use student_view on newly-added blocks :/
 
     def render_children(self, context, fragment, can_reorder=True, can_add=False):
@@ -296,15 +297,18 @@
             fragment.add_fragment_resources(rendered_child)
 
             contents.append({
                 'id': str(child.scope_ids.usage_id),
                 'content': rendered_child.content
             })
 
-        fragment.add_content(self.runtime.render_template("studio_render_children_view.html", {
+        mako_service = self.runtime.service(self, 'mako')
+        # 'lms.' namespace_prefix is required for rendering in studio
+        mako_service.namespace_prefix = 'lms.'
+        fragment.add_content(mako_service.render_template("studio_render_children_view.html", {
             'items': contents,
             'xblock_context': context,
             'can_add': can_add,
             'can_reorder': can_reorder,
         }))
 
     def author_view(self, context):
```

### Comparing `xblock-utils-3.0.0/xblockutils/studio_editable_test.py` & `xblock-utils-3.1.0/xblockutils/studio_editable_test.py`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.0.0/xblockutils/templates/add_buttons.html` & `xblock-utils-3.1.0/xblockutils/templates/add_buttons.html`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.0.0/xblockutils/templates/studio_edit.html` & `xblock-utils-3.1.0/xblockutils/templates/studio_edit.html`

 * *Files identical despite different names*

### Comparing `xblock-utils-3.0.0/xblockutils/templatetags/i18n.py` & `xblock-utils-3.1.0/xblockutils/templatetags/i18n.py`

 * *Files identical despite different names*

