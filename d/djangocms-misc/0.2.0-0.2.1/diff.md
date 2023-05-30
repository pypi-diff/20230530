# Comparing `tmp/djangocms-misc-0.2.0.tar.gz` & `tmp/djangocms-misc-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-misc-0.2.0.tar", last modified: Mon Apr 11 21:15:50 2022, max compression
+gzip compressed data, was "djangocms-misc-0.2.1.tar", last modified: Tue May 30 12:48:24 2023, max compression
```

## Comparing `djangocms-misc-0.2.0.tar` & `djangocms-misc-0.2.1.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.973564 djangocms-misc-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1068 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      349 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-04-11 21:15:50.973564 djangocms-misc-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      468 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/PYPI.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9239 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.957564 djangocms-misc-0.2.0/djangocms_misc/
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.957564 djangocms-misc-0.2.0/djangocms_misc/admin_style/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/admin_style/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.953564 djangocms-misc-0.2.0/djangocms_misc/admin_style/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.953564 djangocms-misc-0.2.0/djangocms_misc/admin_style/static/admin/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.953564 djangocms-misc-0.2.0/djangocms_misc/admin_style/static/admin/djangocms_misc/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.957564 djangocms-misc-0.2.0/djangocms_misc/admin_style/static/admin/djangocms_misc/css/
--rw-r--r--   0 runner    (1001) docker     (121)     2997 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/admin_style/static/admin/djangocms_misc/css/admin_style.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.957564 djangocms-misc-0.2.0/djangocms_misc/admin_style/static/admin/djangocms_misc/sass/
--rw-r--r--   0 runner    (1001) docker     (121)     3976 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/admin_style/static/admin/djangocms_misc/sass/admin_style.sass
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.953564 djangocms-misc-0.2.0/djangocms_misc/admin_style/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.953564 djangocms-misc-0.2.0/djangocms_misc/admin_style/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.957564 djangocms-misc-0.2.0/djangocms_misc/admin_style/templates/admin/inc/
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/admin_style/templates/admin/inc/extrastyle.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.961564 djangocms-misc-0.2.0/djangocms_misc/alternate_toolbar/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/alternate_toolbar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5102 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/alternate_toolbar/cms_toolbars.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.961564 djangocms-misc-0.2.0/djangocms_misc/apphook_templates/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/apphook_templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.961564 djangocms-misc-0.2.0/djangocms_misc/autopublisher/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/autopublisher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4786 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/autopublisher/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.953564 djangocms-misc-0.2.0/djangocms_misc/autopublisher/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.953564 djangocms-misc-0.2.0/djangocms_misc/autopublisher/static/autopublisher/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.961564 djangocms-misc-0.2.0/djangocms_misc/autopublisher/static/autopublisher/css/
--rw-r--r--   0 runner    (1001) docker     (121)       71 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/autopublisher/static/autopublisher/css/autopublisher.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.961564 djangocms-misc-0.2.0/djangocms_misc/autopublisher/static/autopublisher/sass/
--rw-r--r--   0 runner    (1001) docker     (121)      311 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/autopublisher/static/autopublisher/sass/autopublisher.sass
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.961564 djangocms-misc-0.2.0/djangocms_misc/basic/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      960 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.961564 djangocms-misc-0.2.0/djangocms_misc/basic/app_template/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/app_template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      622 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/app_template/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      408 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/app_template/cms_apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      766 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/app_template/cms_menus.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/app_template/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.961564 djangocms-misc-0.2.0/djangocms_misc/basic/app_template/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/app_template/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/app_template/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.953564 djangocms-misc-0.2.0/djangocms_misc/basic/app_template/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.961564 djangocms-misc-0.2.0/djangocms_misc/basic/app_template/templates/app/
--rw-r--r--   0 runner    (1001) docker     (121)      722 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/app_template/templates/app/app_detail.html
--rw-r--r--   0 runner    (1001) docker     (121)     1128 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/app_template/templates/app/app_list.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.961564 djangocms-misc-0.2.0/djangocms_misc/basic/app_template/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/app_template/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      312 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/app_template/tests/tst_app_basic.py
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/app_template/translation.py
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/app_template/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      410 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/app_template/views.py
--rw-r--r--   0 runner    (1001) docker     (121)     1143 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/app_template/views_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      802 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      401 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/context_processors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.961564 djangocms-misc-0.2.0/djangocms_misc/basic/management/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.965564 djangocms-misc-0.2.0/djangocms_misc/basic/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4215 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/management/commands/djangocms_misc_add_cms_group.py
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/management/commands/djangocms_misc_add_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)     3724 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/management/commands/djangocms_misc_startapp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.969564 djangocms-misc-0.2.0/djangocms_misc/basic/middleware/
--rw-r--r--   0 runner    (1001) docker     (121)      271 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      950 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/middleware/bot404.py
--rw-r--r--   0 runner    (1001) docker     (121)     1236 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/middleware/password_protected.py
--rw-r--r--   0 runner    (1001) docker     (121)     1271 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/middleware/redirect_subpage.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.957564 djangocms-misc-0.2.0/djangocms_misc/basic/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.957564 djangocms-misc-0.2.0/djangocms_misc/basic/static/admin/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.957564 djangocms-misc-0.2.0/djangocms_misc/basic/static/admin/djangocms_misc/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.969564 djangocms-misc-0.2.0/djangocms_misc/basic/static/admin/djangocms_misc/css/
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/static/admin/djangocms_misc/css/language_tabs.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.969564 djangocms-misc-0.2.0/djangocms_misc/basic/static/admin/djangocms_misc/js/
--rw-r--r--   0 runner    (1001) docker     (121)     3346 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/static/admin/djangocms_misc/js/language_tabs.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.969564 djangocms-misc-0.2.0/djangocms_misc/basic/static/admin/djangocms_misc/sass/
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/static/admin/djangocms_misc/sass/language_tabs.sass
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.957564 djangocms-misc-0.2.0/djangocms_misc/basic/static/djangocms_misc/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.969564 djangocms-misc-0.2.0/djangocms_misc/basic/static/djangocms_misc/css/
--rw-r--r--   0 runner    (1001) docker     (121)      309 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/static/djangocms_misc/css/cms_frontend_adjust.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.969564 djangocms-misc-0.2.0/djangocms_misc/basic/static/djangocms_misc/sass/
--rw-r--r--   0 runner    (1001) docker     (121)      549 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/static/djangocms_misc/sass/cms_frontend_adjust.sass
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.957564 djangocms-misc-0.2.0/djangocms_misc/basic/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.957564 djangocms-misc-0.2.0/djangocms_misc/basic/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.969564 djangocms-misc-0.2.0/djangocms_misc/basic/templates/admin/djangocms_misc/
--rw-r--r--   0 runner    (1001) docker     (121)      731 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/templates/admin/djangocms_misc/modeltranslation_lang_tabs_change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.957564 djangocms-misc-0.2.0/djangocms_misc/basic/templates/djangocms_misc/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.969564 djangocms-misc-0.2.0/djangocms_misc/basic/templates/djangocms_misc/tags/
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/templates/djangocms_misc/tags/page_link.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.969564 djangocms-misc-0.2.0/djangocms_misc/basic/templates/menu/
--rw-r--r--   0 runner    (1001) docker     (121)      717 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/templates/menu/menu.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.969564 djangocms-misc-0.2.0/djangocms_misc/basic/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4192 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/basic/templatetags/djangocms_misc_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.969564 djangocms-misc-0.2.0/djangocms_misc/editmode_fallback_placeholder/
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/editmode_fallback_placeholder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      525 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/editmode_fallback_placeholder/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)      322 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/editmode_fallback_placeholder/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     4534 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/editmode_fallback_placeholder/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.969564 djangocms-misc-0.2.0/djangocms_misc/global_untranslated_placeholder/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/global_untranslated_placeholder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/global_untranslated_placeholder/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      910 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/global_untranslated_placeholder/models-up-to-3.4-only.py
--rw-r--r--   0 runner    (1001) docker     (121)     1427 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/global_untranslated_placeholder/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     2628 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/global_untranslated_placeholder/signals.py
--rw-r--r--   0 runner    (1001) docker     (121)      385 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/global_untranslated_placeholder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.969564 djangocms-misc-0.2.0/djangocms_misc/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5270 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)       95 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/tests/settings_autopublisher.py
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/tests/settings_pw_protected.py
--rw-r--r--   0 runner    (1001) docker     (121)      798 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/tests/test_admin_style.py
--rw-r--r--   0 runner    (1001) docker     (121)     1730 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/tests/test_alternate_toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.973564 djangocms-misc-0.2.0/djangocms_misc/tests/test_app/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/tests/test_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      784 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/tests/test_app/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/tests/test_app/cms_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.973564 djangocms-misc-0.2.0/djangocms_misc/tests/test_app/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     1401 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/tests/test_app/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)     1240 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/tests/test_app/migrations/0002_auto_20170805_0136.py
--rw-r--r--   0 runner    (1001) docker     (121)      671 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/tests/test_app/migrations/0003_auto_20171014_0359.py
--rw-r--r--   0 runner    (1001) docker     (121)      486 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/tests/test_app/migrations/0004_testpluginmodel_field1_fr.py
--rw-r--r--   0 runner    (1001) docker     (121)      837 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/tests/test_app/migrations/0005_auto_20200211_1615.py
--rw-r--r--   0 runner    (1001) docker     (121)     1398 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/tests/test_app/migrations/0006_auto_20200928_0724.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/tests/test_app/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1002 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/tests/test_app/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      606 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/tests/test_app/translation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3777 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/tests/test_autopublisher.py
--rw-r--r--   0 runner    (1001) docker     (121)     5028 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (121)     2267 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/tests/test_untranslated_placeholders.py
--rw-r--r--   0 runner    (1001) docker     (121)      506 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/tests/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.973564 djangocms-misc-0.2.0/djangocms_misc/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/tests/utils/django_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2242 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/tests/utils/selenium_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.973564 djangocms-misc-0.2.0/djangocms_misc/untranslated_placeholder_original/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/untranslated_placeholder_original/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/untranslated_placeholder_original/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     3981 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/untranslated_placeholder_original/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.973564 djangocms-misc-0.2.0/djangocms_misc/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      529 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/djangocms_misc/utils/edit_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-11 21:15:50.957564 djangocms-misc-0.2.0/djangocms_misc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2022-04-11 21:15:50.000000 djangocms-misc-0.2.0/djangocms_misc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5008 2022-04-11 21:15:50.000000 djangocms-misc-0.2.0/djangocms_misc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-11 21:15:50.000000 djangocms-misc-0.2.0/djangocms_misc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-11 21:15:50.000000 djangocms-misc-0.2.0/djangocms_misc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-04-11 21:15:50.000000 djangocms-misc-0.2.0/djangocms_misc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-04-11 21:15:50.000000 djangocms-misc-0.2.0/djangocms_misc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-04-11 21:15:50.973564 djangocms-misc-0.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1190 2022-04-11 21:15:38.000000 djangocms-misc-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.511720 djangocms-misc-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-30 12:48:24.511720 djangocms-misc-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/PYPI.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9426 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.499719 djangocms-misc-0.2.1/djangocms_misc/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.503719 djangocms-misc-0.2.1/djangocms_misc/admin_style/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/admin_style/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.495720 djangocms-misc-0.2.1/djangocms_misc/admin_style/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.495720 djangocms-misc-0.2.1/djangocms_misc/admin_style/static/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.495720 djangocms-misc-0.2.1/djangocms_misc/admin_style/static/admin/djangocms_misc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.503719 djangocms-misc-0.2.1/djangocms_misc/admin_style/static/admin/djangocms_misc/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/admin_style/static/admin/djangocms_misc/css/admin_style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.503719 djangocms-misc-0.2.1/djangocms_misc/admin_style/static/admin/djangocms_misc/sass/
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/admin_style/static/admin/djangocms_misc/sass/admin_style.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.495720 djangocms-misc-0.2.1/djangocms_misc/admin_style/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.495720 djangocms-misc-0.2.1/djangocms_misc/admin_style/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.503719 djangocms-misc-0.2.1/djangocms_misc/admin_style/templates/admin/inc/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/admin_style/templates/admin/inc/extrastyle.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.503719 djangocms-misc-0.2.1/djangocms_misc/alternate_toolbar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/alternate_toolbar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5101 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/alternate_toolbar/cms_toolbars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.503719 djangocms-misc-0.2.1/djangocms_misc/apphook_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/apphook_templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.503719 djangocms-misc-0.2.1/djangocms_misc/autopublisher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/autopublisher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/autopublisher/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.499719 djangocms-misc-0.2.1/djangocms_misc/autopublisher/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.499719 djangocms-misc-0.2.1/djangocms_misc/autopublisher/static/autopublisher/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.503719 djangocms-misc-0.2.1/djangocms_misc/autopublisher/static/autopublisher/css/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/autopublisher/static/autopublisher/css/autopublisher.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.503719 djangocms-misc-0.2.1/djangocms_misc/autopublisher/static/autopublisher/sass/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/autopublisher/static/autopublisher/sass/autopublisher.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.503719 djangocms-misc-0.2.1/djangocms_misc/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.503719 djangocms-misc-0.2.1/djangocms_misc/basic/app_template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/app_template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/app_template/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/app_template/cms_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/app_template/cms_menus.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/app_template/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.503719 djangocms-misc-0.2.1/djangocms_misc/basic/app_template/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/app_template/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/app_template/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.499719 djangocms-misc-0.2.1/djangocms_misc/basic/app_template/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.503719 djangocms-misc-0.2.1/djangocms_misc/basic/app_template/templates/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/app_template/templates/app/app_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/app_template/templates/app/app_list.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.503719 djangocms-misc-0.2.1/djangocms_misc/basic/app_template/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/app_template/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/app_template/tests/tst_app_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/app_template/translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/app_template/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/app_template/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/app_template/views_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/context_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.503719 djangocms-misc-0.2.1/djangocms_misc/basic/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.507720 djangocms-misc-0.2.1/djangocms_misc/basic/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/management/commands/djangocms_misc_add_cms_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/management/commands/djangocms_misc_add_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/management/commands/djangocms_misc_startapp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.507720 djangocms-misc-0.2.1/djangocms_misc/basic/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/middleware/bot404.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/middleware/password_protected.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/middleware/redirect_subpage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.499719 djangocms-misc-0.2.1/djangocms_misc/basic/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.499719 djangocms-misc-0.2.1/djangocms_misc/basic/static/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.499719 djangocms-misc-0.2.1/djangocms_misc/basic/static/admin/djangocms_misc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.507720 djangocms-misc-0.2.1/djangocms_misc/basic/static/admin/djangocms_misc/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/static/admin/djangocms_misc/css/language_tabs.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.507720 djangocms-misc-0.2.1/djangocms_misc/basic/static/admin/djangocms_misc/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/static/admin/djangocms_misc/js/language_tabs.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.507720 djangocms-misc-0.2.1/djangocms_misc/basic/static/admin/djangocms_misc/sass/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/static/admin/djangocms_misc/sass/language_tabs.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.499719 djangocms-misc-0.2.1/djangocms_misc/basic/static/djangocms_misc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.507720 djangocms-misc-0.2.1/djangocms_misc/basic/static/djangocms_misc/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/static/djangocms_misc/css/cms_frontend_adjust.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.507720 djangocms-misc-0.2.1/djangocms_misc/basic/static/djangocms_misc/sass/
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/static/djangocms_misc/sass/cms_frontend_adjust.sass
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.499719 djangocms-misc-0.2.1/djangocms_misc/basic/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.499719 djangocms-misc-0.2.1/djangocms_misc/basic/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.507720 djangocms-misc-0.2.1/djangocms_misc/basic/templates/admin/djangocms_misc/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/templates/admin/djangocms_misc/modeltranslation_lang_tabs_change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.499719 djangocms-misc-0.2.1/djangocms_misc/basic/templates/djangocms_misc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.507720 djangocms-misc-0.2.1/djangocms_misc/basic/templates/djangocms_misc/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/templates/djangocms_misc/tags/page_link.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.507720 djangocms-misc-0.2.1/djangocms_misc/basic/templates/menu/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/templates/menu/menu.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.507720 djangocms-misc-0.2.1/djangocms_misc/basic/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/basic/templatetags/djangocms_misc_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.507720 djangocms-misc-0.2.1/djangocms_misc/editmode_fallback_placeholder/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/editmode_fallback_placeholder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/editmode_fallback_placeholder/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/editmode_fallback_placeholder/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/editmode_fallback_placeholder/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.507720 djangocms-misc-0.2.1/djangocms_misc/global_untranslated_placeholder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/global_untranslated_placeholder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/global_untranslated_placeholder/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/global_untranslated_placeholder/models-up-to-3.4-only.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/global_untranslated_placeholder/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/global_untranslated_placeholder/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/global_untranslated_placeholder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.511720 djangocms-misc-0.2.1/djangocms_misc/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/tests/settings_autopublisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/tests/settings_pw_protected.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/tests/test_admin_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/tests/test_alternate_toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.511720 djangocms-misc-0.2.1/djangocms_misc/tests/test_app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/tests/test_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/tests/test_app/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/tests/test_app/cms_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.511720 djangocms-misc-0.2.1/djangocms_misc/tests/test_app/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/tests/test_app/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/tests/test_app/migrations/0002_auto_20170805_0136.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/tests/test_app/migrations/0003_auto_20171014_0359.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/tests/test_app/migrations/0004_testpluginmodel_field1_fr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/tests/test_app/migrations/0005_auto_20200211_1615.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/tests/test_app/migrations/0006_auto_20200928_0724.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/tests/test_app/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/tests/test_app/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/tests/test_app/translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/tests/test_autopublisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/tests/test_untranslated_placeholders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.511720 djangocms-misc-0.2.1/djangocms_misc/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/tests/utils/django_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/tests/utils/selenium_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.511720 djangocms-misc-0.2.1/djangocms_misc/untranslated_placeholder_original/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/untranslated_placeholder_original/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/untranslated_placeholder_original/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/untranslated_placeholder_original/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.511720 djangocms-misc-0.2.1/djangocms_misc/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/djangocms_misc/utils/edit_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 12:48:24.503719 djangocms-misc-0.2.1/djangocms_misc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-30 12:48:24.000000 djangocms-misc-0.2.1/djangocms_misc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-05-30 12:48:24.000000 djangocms-misc-0.2.1/djangocms_misc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:48:24.000000 djangocms-misc-0.2.1/djangocms_misc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 12:48:24.000000 djangocms-misc-0.2.1/djangocms_misc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-30 12:48:24.000000 djangocms-misc-0.2.1/djangocms_misc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-30 12:48:24.000000 djangocms-misc-0.2.1/djangocms_misc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-30 12:48:24.511720 djangocms-misc-0.2.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1224 2023-05-30 12:48:12.000000 djangocms-misc-0.2.1/setup.py
```

### Comparing `djangocms-misc-0.2.0/LICENSE` & `djangocms-misc-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms-misc-0.2.0/PKG-INFO` & `djangocms-misc-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: djangocms-misc
-Version: 0.2.0
+Version: 0.2.1
 Summary: djangocms misc
 Home-page: https://github.com/bnzk/djangocms-misc
 Author: Ben Stähli
 Author-email: bnzk@bnzk.ch
 License: MIT Licence
 Platform: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
-.. image:: https://github.com/bnzk/djangocms-misc/actions/workflows/ci.yml/badge.svg
-    :target: https://github.com/bnzk/djangocms-misc/actions/workflows/ci.yml
-.. image:: https://img.shields.io/pypi/v/djangocms-misc.svg
-    :target: https://pypi.python.org/pypi/djangocms-misc/
-.. image:: https://img.shields.io/pypi/l/djangocms-misc.svg
-    :target: https://pypi.python.org/pypi/djangocms-misc/
-
-Development and Docs on `<https://github.com/bnzk/djangocms-misc/>`_
+# djangocms-misc
 
+[![CI](https://github.com/bnzk/djangocms-misc/actions/workflows/ci.yml/badge.svg)](https://github.com/bnzk/djangocms-misc/actions/workflows/ci.yml)
+[![Version](https://img.shields.io/pypi/v/djangocms-misc.svg?style=flat-square "Version")](https://pypi.python.org/pypi/djangocms-misc/)
+[![Licence](https://img.shields.io/github/license/bnzk/djangocms-misc.svg?style=flat-square "Licence")](https://pypi.python.org/pypi/djangocms-misc/)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/djangocms-misc?style=flat-square "PyPi Downloads")](https://pypistats.org/packages/djangocms-misc)
 
+Development and docs on https://github.com/bnzk/djangocms-misc/
```

### Comparing `djangocms-misc-0.2.0/README.md` & `djangocms-misc-0.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # djangocms-misc
 
 [![CI](https://github.com/bnzk/djangocms-misc/actions/workflows/ci.yml/badge.svg)](https://github.com/bnzk/djangocms-misc/actions/workflows/ci.yml)
-[![PyPi Version](https://img.shields.io/pypi/v/djangocms-misc.svg "PyPi Version")](https://pypi.python.org/pypi/djangocms-misc/)
-[![Licence](https://img.shields.io/pypi/l/djangocms-misc.svg "Licence")](https://pypi.python.org/pypi/djangocms-misc/)
+[![Version](https://img.shields.io/pypi/v/djangocms-misc.svg?style=flat-square "Version")](https://pypi.python.org/pypi/djangocms-misc/)
+[![Licence](https://img.shields.io/github/license/bnzk/djangocms-misc.svg?style=flat-square "Licence")](https://pypi.python.org/pypi/djangocms-misc/)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/djangocms-misc?style=flat-square "PyPi Downloads")](https://pypistats.org/packages/djangocms-misc)
 
 customizing [django-cms](https://github.com/divio/django-cms), as a set of diferent apps, that can be installed individually
 
 
 ## Features
 
 - [djangocms_misc.basic](#basic) (various tools and helpers)
@@ -136,15 +137,15 @@
   - as is
 - Clipboard
   - more visible
 
 Add `djangocms_misc.alternate_toolbar` to `INSTALLED_APPS`, and you'll have it as is.
 If you want custom items in your administration menu, create your own `cms_toolbars.py`, as follows:
 
-    from django.utils.translation import ugettext_lazy as _
+    from django.utils.translation import gettext_lazy as _
     from cms.toolbar_pool import toolbar_pool
     from cms.utils.urlutils import admin_reverse
     from djangocms_misc.alternate_toolbar.cms_toolbars import AlternateBasicToolbar
 
 
     toolbar_pool.unregister(AlternateBasicToolbar)
```

### Comparing `djangocms-misc-0.2.0/djangocms_misc/admin_style/static/admin/djangocms_misc/css/admin_style.css` & `djangocms-misc-0.2.1/djangocms_misc/admin_style/static/admin/djangocms_misc/css/admin_style.css`

 * *Files identical despite different names*

### Comparing `djangocms-misc-0.2.0/djangocms_misc/admin_style/static/admin/djangocms_misc/sass/admin_style.sass` & `djangocms-misc-0.2.1/djangocms_misc/admin_style/static/admin/djangocms_misc/sass/admin_style.sass`

 * *Files identical despite different names*

### Comparing `djangocms-misc-0.2.0/djangocms_misc/alternate_toolbar/cms_toolbars.py` & `djangocms-misc-0.2.1/djangocms_misc/alternate_toolbar/cms_toolbars.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django.conf import settings
 from django.contrib.auth import get_user_model, get_permission_codename
 from django.contrib import admin
 from django.urls import reverse
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 from cms.utils.urlutils import admin_reverse
 from cms.toolbar_pool import toolbar_pool
 from cms.cms_toolbars import BasicToolbar, ADMIN_MENU_IDENTIFIER, ADMINISTRATION_BREAK
 
 from djangocms_misc.utils.edit_mode import is_edit_or_build_mode
 
 USER_MENU_IDENTIFIER = 'user-menu'
```

### Comparing `djangocms-misc-0.2.0/djangocms_misc/autopublisher/models.py` & `djangocms-misc-0.2.1/djangocms_misc/autopublisher/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,37 @@
-from __future__ import unicode_literals
-
 # from cms.admin.static_placeholder import StaticPlaceholderAdmin
 # from django.conf import settings
 # from django.urls import resolve
 from cms.models import CMSPlugin, StaticPlaceholder
 from cms.signals import post_placeholder_operation  # post_obj_operation
 from django.db.models.signals import post_save
 from django.dispatch import receiver
 
 # ugly
 from cms import __version__ as cms_version
 CMS_VERSION_36 = cms_version.startswith('3.6.')
 CMS_VERSION_37 = cms_version.startswith('3.7.')
 CMS_VERSION_38 = cms_version.startswith('3.8.')
+CMS_VERSION_39 = cms_version.startswith('3.9.')
+CMS_VERSION_310 = cms_version.startswith('3.10.')
 
 
 def check_publish(title_obj, force_non_dirty=False):
     page = title_obj.page
     if title_obj.published and page.publisher_is_draft:
         # print("published and draft!")
         # print(title_obj.is_dirty())
         # not dirty, after plugin add, in cms 3.6!
-        if title_obj.is_dirty() or force_non_dirty or CMS_VERSION_36 or CMS_VERSION_37 or CMS_VERSION_38:
+        if title_obj.is_dirty() or \
+                force_non_dirty or \
+                CMS_VERSION_36 or \
+                CMS_VERSION_37 or \
+                CMS_VERSION_38 or \
+                CMS_VERSION_39 or \
+                CMS_VERSION_310:
             # print("NEEEEEDs publishing")
             page.publish(title_obj.language)
             # from cms.api import publish_page
             # publish_page(page, user, title_obj.language)
             # print("done publishing")
     else:
         pass
```

### Comparing `djangocms-misc-0.2.0/djangocms_misc/basic/admin.py` & `djangocms-misc-0.2.1/djangocms_misc/basic/admin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import unicode_literals
-
 from django.conf import settings
 
 
 # thx to @wullerot https://gist.github.com/wullerot/9fe3151101e57a9ee6fadb3cababb619
 class LanguageTabsMixin(object):
     change_form_template = 'admin/djangocms_misc/modeltranslation_lang_tabs_change_form.html'
```

### Comparing `djangocms-misc-0.2.0/djangocms_misc/basic/app_template/admin.py` & `djangocms-misc-0.2.1/djangocms_misc/basic/app_template/admin.py`

 * *Files identical despite different names*

### Comparing `djangocms-misc-0.2.0/djangocms_misc/basic/app_template/cms_menus.py` & `djangocms-misc-0.2.1/djangocms_misc/basic/app_template/cms_menus.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,11 @@
-# coding: utf-8
-from __future__ import unicode_literals
-
 from cms.menu_bases import CMSAttachMenu  # , Menu
 from django.conf import settings
 from menus.base import NavigationNode
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 from .models import AppTemplate
 
 
 class AppTemplateMenu(CMSAttachMenu):
     name = _('AppTemplate Menu')
```

### Comparing `djangocms-misc-0.2.0/djangocms_misc/basic/app_template/models.py` & `djangocms-misc-0.2.1/djangocms_misc/basic/app_template/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# coding: utf-8
-from __future__ import unicode_literals
-
 from cms.models import PlaceholderField
 from django.urls import reverse
 from django.db import models
 from django.utils.text import slugify
 # from filer.fields.image import FilerImageField
 from filer_addons.filer_gui.fields import FilerImageField
```

### Comparing `djangocms-misc-0.2.0/djangocms_misc/basic/app_template/templates/app/app_detail.html` & `djangocms-misc-0.2.1/djangocms_misc/basic/app_template/templates/app/app_detail.html`

 * *Files identical despite different names*

### Comparing `djangocms-misc-0.2.0/djangocms_misc/basic/app_template/templates/app/app_list.html` & `djangocms-misc-0.2.1/djangocms_misc/basic/app_template/templates/app/app_list.html`

 * *Files identical despite different names*

### Comparing `djangocms-misc-0.2.0/djangocms_misc/basic/app_template/views_utils.py` & `djangocms-misc-0.2.1/djangocms_misc/basic/app_template/views_utils.py`

 * *Files identical despite different names*

### Comparing `djangocms-misc-0.2.0/djangocms_misc/basic/conf.py` & `djangocms-misc-0.2.1/djangocms_misc/basic/conf.py`

 * *Files identical despite different names*

### Comparing `djangocms-misc-0.2.0/djangocms_misc/basic/management/commands/djangocms_misc_add_cms_group.py` & `djangocms-misc-0.2.1/djangocms_misc/basic/management/commands/djangocms_misc_add_cms_group.py`

 * *Files identical despite different names*

### Comparing `djangocms-misc-0.2.0/djangocms_misc/basic/management/commands/djangocms_misc_add_groups.py` & `djangocms-misc-0.2.1/djangocms_misc/basic/management/commands/djangocms_misc_add_groups.py`

 * *Files identical despite different names*

### Comparing `djangocms-misc-0.2.0/djangocms_misc/basic/management/commands/djangocms_misc_startapp.py` & `djangocms-misc-0.2.1/djangocms_misc/basic/management/commands/djangocms_misc_startapp.py`

 * *Files identical despite different names*

### Comparing `djangocms-misc-0.2.0/djangocms_misc/basic/middleware/bot404.py` & `djangocms-misc-0.2.1/djangocms_misc/basic/middleware/bot404.py`

 * *Files identical despite different names*

### Comparing `djangocms-misc-0.2.0/djangocms_misc/basic/middleware/password_protected.py` & `djangocms-misc-0.2.1/djangocms_misc/basic/middleware/password_protected.py`

 * *Files identical despite different names*

### Comparing `djangocms-misc-0.2.0/djangocms_misc/basic/middleware/redirect_subpage.py` & `djangocms-misc-0.2.1/djangocms_misc/basic/middleware/redirect_subpage.py`

 * *Files identical despite different names*

### Comparing `djangocms-misc-0.2.0/djangocms_misc/basic/static/admin/djangocms_misc/js/language_tabs.js` & `djangocms-misc-0.2.1/djangocms_misc/basic/static/admin/djangocms_misc/js/language_tabs.js`

 * *Files identical despite different names*

### Comparing `djangocms-misc-0.2.0/djangocms_misc/basic/static/djangocms_misc/sass/cms_frontend_adjust.sass` & `djangocms-misc-0.2.1/djangocms_misc/basic/static/djangocms_misc/sass/cms_frontend_adjust.sass`

 * *Files identical despite different names*

### Comparing `djangocms-misc-0.2.0/djangocms_misc/basic/templates/admin/djangocms_misc/modeltranslation_lang_tabs_change_form.html` & `djangocms-misc-0.2.1/djangocms_misc/basic/templates/admin/djangocms_misc/modeltranslation_lang_tabs_change_form.html`

 * *Files identical despite different names*

### Comparing `djangocms-misc-0.2.0/djangocms_misc/basic/templates/menu/menu.html` & `djangocms-misc-0.2.1/djangocms_misc/basic/templates/menu/menu.html`

 * *Files identical despite different names*

### Comparing `djangocms-misc-0.2.0/djangocms_misc/basic/templatetags/djangocms_misc_tags.py` & `djangocms-misc-0.2.1/djangocms_misc/basic/templatetags/djangocms_misc_tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # coding: utf-8
-from __future__ import unicode_literals
 
 from cms.models import Page, Placeholder
 from django.conf import settings
 from django import template
 
 from djangocms_misc.utils.edit_mode import is_edit_mode
```

### Comparing `djangocms-misc-0.2.0/djangocms_misc/editmode_fallback_placeholder/apps.py` & `djangocms-misc-0.2.1/djangocms_misc/editmode_fallback_placeholder/apps.py`

 * *Files identical despite different names*

### Comparing `djangocms-misc-0.2.0/djangocms_misc/editmode_fallback_placeholder/plugins.py` & `djangocms-misc-0.2.1/djangocms_misc/editmode_fallback_placeholder/plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-misc-0.2.0/djangocms_misc/global_untranslated_placeholder/models-up-to-3.4-only.py` & `djangocms-misc-0.2.1/djangocms_misc/global_untranslated_placeholder/models-up-to-3.4-only.py`

 * *Files identical despite different names*

### Comparing `djangocms-misc-0.2.0/djangocms_misc/global_untranslated_placeholder/models.py` & `djangocms-misc-0.2.1/djangocms_misc/global_untranslated_placeholder/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-misc-0.2.0/djangocms_misc/global_untranslated_placeholder/signals.py` & `djangocms-misc-0.2.1/djangocms_misc/global_untranslated_placeholder/signals.py`

 * *Files identical despite different names*

### Comparing `djangocms-misc-0.2.0/djangocms_misc/tests/settings.py` & `djangocms-misc-0.2.1/djangocms_misc/tests/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,28 @@
 
 SITE_ID = 1
 
 # from selenium.webdriver.firefox import webdriver
 # from selenium.webdriver.phantomjs import webdriver
 # SELENIUM_WEBDRIVER = webdriver
 
+DEFAULT_AUTO_FIELD = 'django.db.models.AutoField'
+
 APP_ROOT = os.path.abspath(
     os.path.join(os.path.dirname(__file__), ".."))
 
 DATABASES = {
     'default': {
         'ENGINE': 'django.db.backends.sqlite3',
         'NAME': 'db.sqlite',
     }
 }
 
+X_FRAME_OPTIONS = 'SAMESITE'
+
 LANGUAGE_CODE = 'en'
 LANGUAGES = (
     ('en', 'English', ),
     ('de', 'Deutsch', ),
     ('fr', 'Frentsch', ),
 )
```

### Comparing `djangocms-misc-0.2.0/djangocms_misc/tests/test_admin_style.py` & `djangocms-misc-0.2.1/djangocms_misc/tests/test_admin_style.py`

 * *Files identical despite different names*

### Comparing `djangocms-misc-0.2.0/djangocms_misc/tests/test_alternate_toolbar.py` & `djangocms-misc-0.2.1/djangocms_misc/tests/test_alternate_toolbar.py`

 * *Files identical despite different names*

### Comparing `djangocms-misc-0.2.0/djangocms_misc/tests/test_app/admin.py` & `djangocms-misc-0.2.1/djangocms_misc/tests/test_app/admin.py`

 * *Files identical despite different names*

### Comparing `djangocms-misc-0.2.0/djangocms_misc/tests/test_app/migrations/0001_initial.py` & `djangocms-misc-0.2.1/djangocms_misc/tests/test_app/migrations/0001_initial.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # -*- coding: utf-8 -*-
 # Generated by Django 1.10.7 on 2017-07-04 15:20
-from __future__ import unicode_literals
 
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
```

### Comparing `djangocms-misc-0.2.0/djangocms_misc/tests/test_app/migrations/0002_auto_20170805_0136.py` & `djangocms-misc-0.2.1/djangocms_misc/tests/test_app/migrations/0002_auto_20170805_0136.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # -*- coding: utf-8 -*-
 # Generated by Django 1.10.7 on 2017-08-05 01:36
-from __future__ import unicode_literals
 
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
```

### Comparing `djangocms-misc-0.2.0/djangocms_misc/tests/test_app/migrations/0003_auto_20171014_0359.py` & `djangocms-misc-0.2.1/djangocms_misc/tests/test_app/migrations/0003_auto_20171014_0359.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # -*- coding: utf-8 -*-
 # Generated by Django 1.9.13 on 2017-10-14 03:59
-from __future__ import unicode_literals
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
```

### Comparing `djangocms-misc-0.2.0/djangocms_misc/tests/test_app/migrations/0006_auto_20200928_0724.py` & `djangocms-misc-0.2.1/djangocms_misc/tests/test_app/migrations/0006_auto_20200928_0724.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # -*- coding: utf-8 -*-
 # Generated by Django 1.11.29 on 2020-09-28 07:24
-from __future__ import unicode_literals
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
```

### Comparing `djangocms-misc-0.2.0/djangocms_misc/tests/test_app/models.py` & `djangocms-misc-0.2.1/djangocms_misc/tests/test_app/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-misc-0.2.0/djangocms_misc/tests/test_app/translation.py` & `djangocms-misc-0.2.1/djangocms_misc/tests/test_app/translation.py`

 * *Files identical despite different names*

### Comparing `djangocms-misc-0.2.0/djangocms_misc/tests/test_autopublisher.py` & `djangocms-misc-0.2.1/djangocms_misc/tests/test_autopublisher.py`

 * *Files identical despite different names*

### Comparing `djangocms-misc-0.2.0/djangocms_misc/tests/test_basic.py` & `djangocms-misc-0.2.1/djangocms_misc/tests/test_basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # -*- coding: utf-8 -*-
-from __future__ import unicode_literals
 
 from cms.api import create_page, create_title, add_plugin
 from django.contrib.auth.models import User
 from django.test import TestCase, Client, modify_settings
 
 from djangocms_misc.basic.templatetags.djangocms_misc_tags import djangocms_misc_placeholder_empty
 from djangocms_misc.tests.test_app.cms_plugins import TestPlugin
```

### Comparing `djangocms-misc-0.2.0/djangocms_misc/tests/test_untranslated_placeholders.py` & `djangocms-misc-0.2.1/djangocms_misc/tests/test_untranslated_placeholders.py`

 * *Files identical despite different names*

### Comparing `djangocms-misc-0.2.0/djangocms_misc/tests/utils/selenium_utils.py` & `djangocms-misc-0.2.1/djangocms_misc/tests/utils/selenium_utils.py`

 * *Files identical despite different names*

### Comparing `djangocms-misc-0.2.0/djangocms_misc/untranslated_placeholder_original/plugins.py` & `djangocms-misc-0.2.1/djangocms_misc/untranslated_placeholder_original/plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-misc-0.2.0/djangocms_misc/utils/edit_mode.py` & `djangocms-misc-0.2.1/djangocms_misc/utils/edit_mode.py`

 * *Files identical despite different names*

### Comparing `djangocms-misc-0.2.0/djangocms_misc.egg-info/PKG-INFO` & `djangocms-misc-0.2.1/djangocms_misc.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: djangocms-misc
-Version: 0.2.0
+Version: 0.2.1
 Summary: djangocms misc
 Home-page: https://github.com/bnzk/djangocms-misc
 Author: Ben Stähli
 Author-email: bnzk@bnzk.ch
 License: MIT Licence
 Platform: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
-.. image:: https://github.com/bnzk/djangocms-misc/actions/workflows/ci.yml/badge.svg
-    :target: https://github.com/bnzk/djangocms-misc/actions/workflows/ci.yml
-.. image:: https://img.shields.io/pypi/v/djangocms-misc.svg
-    :target: https://pypi.python.org/pypi/djangocms-misc/
-.. image:: https://img.shields.io/pypi/l/djangocms-misc.svg
-    :target: https://pypi.python.org/pypi/djangocms-misc/
-
-Development and Docs on `<https://github.com/bnzk/djangocms-misc/>`_
+# djangocms-misc
 
+[![CI](https://github.com/bnzk/djangocms-misc/actions/workflows/ci.yml/badge.svg)](https://github.com/bnzk/djangocms-misc/actions/workflows/ci.yml)
+[![Version](https://img.shields.io/pypi/v/djangocms-misc.svg?style=flat-square "Version")](https://pypi.python.org/pypi/djangocms-misc/)
+[![Licence](https://img.shields.io/github/license/bnzk/djangocms-misc.svg?style=flat-square "Licence")](https://pypi.python.org/pypi/djangocms-misc/)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/djangocms-misc?style=flat-square "PyPi Downloads")](https://pypistats.org/packages/djangocms-misc)
 
+Development and docs on https://github.com/bnzk/djangocms-misc/
```

### Comparing `djangocms-misc-0.2.0/djangocms_misc.egg-info/SOURCES.txt` & `djangocms-misc-0.2.1/djangocms_misc.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 LICENSE
 MANIFEST.in
-PYPI.rst
+PYPI.md
 README.md
 setup.cfg
 setup.py
 djangocms_misc/__init__.py
 djangocms_misc.egg-info/PKG-INFO
 djangocms_misc.egg-info/SOURCES.txt
 djangocms_misc.egg-info/dependency_links.txt
```

### Comparing `djangocms-misc-0.2.0/setup.py` & `djangocms-misc-0.2.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# coding: utf-8
 from setuptools import setup, find_packages
 import os
 
 
 # not so bad: http://joebergantine.com/blog/2015/jul/17/releasing-package-pypi/
 version = __import__('djangocms_misc').__version__
 
@@ -15,15 +14,16 @@
 setup(
     name="djangocms-misc",
     version=version,
     url='https://github.com/bnzk/djangocms-misc',
     license='MIT Licence',
     platforms=['OS Independent'],
     description="djangocms misc",
-    long_description=read('PYPI.rst'),
+    long_description=read('PYPI.md'),
+    long_description_content_type="text/markdown",
     author=u'Ben Stähli',
     author_email='bnzk@bnzk.ch',
     packages=find_packages(),
     install_requires=(
         # 'Django>=1.3,<1.5',  # no need to limit while in development
         'django>=1.8',
         'django-appconf>=1.0'
```

