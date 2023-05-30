# Comparing `tmp/django-post_office-3.6.3.tar.gz` & `tmp/django-post_office-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-post_office-3.6.3.tar", last modified: Thu Oct 27 07:48:10 2022, max compression
+gzip compressed data, was "django-post_office-3.7.0.tar", last modified: Tue May 30 04:47:13 2023, max compression
```

## Comparing `django-post_office-3.6.3.tar` & `django-post_office-3.7.0.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2022-10-27 07:48:10.000000 django-post_office-3.6.3/
--rw-r--r--   0 selwin     (501) staff       (20)    32538 2022-10-27 07:48:10.000000 django-post_office-3.6.3/PKG-INFO
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2022-10-27 07:48:10.000000 django-post_office-3.6.3/django_post_office.egg-info/
--rw-r--r--   0 selwin     (501) staff       (20)    32538 2022-10-27 07:48:10.000000 django-post_office-3.6.3/django_post_office.egg-info/PKG-INFO
--rw-r--r--   0 selwin     (501) staff       (20)        1 2017-12-06 05:55:06.000000 django-post_office-3.6.3/django_post_office.egg-info/not-zip-safe
--rw-r--r--   0 selwin     (501) staff       (20)     2714 2022-10-27 07:48:10.000000 django-post_office-3.6.3/django_post_office.egg-info/SOURCES.txt
--rw-r--r--   0 selwin     (501) staff       (20)       83 2022-10-27 07:48:10.000000 django-post_office-3.6.3/django_post_office.egg-info/requires.txt
--rw-r--r--   0 selwin     (501) staff       (20)       12 2022-10-27 07:48:10.000000 django-post_office-3.6.3/django_post_office.egg-info/top_level.txt
--rw-r--r--   0 selwin     (501) staff       (20)        1 2022-10-27 07:48:10.000000 django-post_office-3.6.3/django_post_office.egg-info/dependency_links.txt
--rw-r--r--   0 selwin     (501) staff       (20)      257 2022-10-27 07:39:26.000000 django-post_office-3.6.3/MANIFEST.in
--rw-r--r--   0 selwin     (501) staff       (20)    24875 2022-10-07 02:18:01.000000 django-post_office-3.6.3/README.md
--rw-r--r--   0 selwin     (501) staff       (20)     2411 2022-10-27 07:39:26.000000 django-post_office-3.6.3/setup.py
--rw-r--r--   0 selwin     (501) staff       (20)      342 2021-12-21 05:02:58.000000 django-post_office-3.6.3/AUTHORS.rst
--rw-r--r--   0 selwin     (501) staff       (20)       38 2022-10-27 07:48:10.000000 django-post_office-3.6.3/setup.cfg
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2022-10-27 07:48:10.000000 django-post_office-3.6.3/post_office/
--rw-r--r--   0 selwin     (501) staff       (20)    12590 2022-10-07 02:18:01.000000 django-post_office-3.6.3/post_office/mail.py
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2022-10-27 07:48:10.000000 django-post_office-3.6.3/post_office/templatetags/
--rw-r--r--   0 selwin     (501) staff       (20)     1359 2020-08-22 01:45:58.000000 django-post_office-3.6.3/post_office/templatetags/post_office.py
--rw-r--r--   0 selwin     (501) staff       (20)        0 2020-02-28 08:42:53.000000 django-post_office-3.6.3/post_office/templatetags/__init__.py
--rw-r--r--   0 selwin     (501) staff       (20)      558 2021-12-21 05:02:58.000000 django-post_office-3.6.3/post_office/signals.py
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2022-10-27 07:48:10.000000 django-post_office-3.6.3/post_office/migrations/
--rw-r--r--   0 selwin     (501) staff       (20)     1481 2020-10-31 09:08:42.000000 django-post_office-3.6.3/post_office/migrations/0010_message_id.py
--rw-r--r--   0 selwin     (501) staff       (20)      370 2020-02-28 08:42:53.000000 django-post_office-3.6.3/post_office/migrations/0006_attachment_mimetype.py
--rw-r--r--   0 selwin     (501) staff       (20)     4960 2020-02-28 08:42:53.000000 django-post_office-3.6.3/post_office/migrations/0004_auto_20160607_0901.py
--rw-r--r--   0 selwin     (501) staff       (20)      912 2020-08-22 01:45:58.000000 django-post_office-3.6.3/post_office/migrations/0009_requeued_mode.py
--rw-r--r--   0 selwin     (501) staff       (20)     2512 2020-02-28 08:42:53.000000 django-post_office-3.6.3/post_office/migrations/0003_longer_subject.py
--rw-r--r--   0 selwin     (501) staff       (20)        0 2017-12-06 05:45:13.000000 django-post_office-3.6.3/post_office/migrations/__init__.py
--rw-r--r--   0 selwin     (501) staff       (20)      452 2020-02-28 08:42:53.000000 django-post_office-3.6.3/post_office/migrations/0008_attachment_headers.py
--rw-r--r--   0 selwin     (501) staff       (20)      433 2020-02-28 08:42:53.000000 django-post_office-3.6.3/post_office/migrations/0007_auto_20170731_1342.py
--rw-r--r--   0 selwin     (501) staff       (20)     5252 2020-02-28 08:42:53.000000 django-post_office-3.6.3/post_office/migrations/0002_add_i18n_and_backend_alias.py
--rw-r--r--   0 selwin     (501) staff       (20)     4569 2020-02-28 08:42:53.000000 django-post_office-3.6.3/post_office/migrations/0001_initial.py
--rw-r--r--   0 selwin     (501) staff       (20)      957 2020-11-05 07:48:55.000000 django-post_office-3.6.3/post_office/migrations/0011_models_help_text.py
--rw-r--r--   0 selwin     (501) staff       (20)      391 2020-02-28 08:42:53.000000 django-post_office-3.6.3/post_office/migrations/0005_auto_20170515_0013.py
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2022-10-27 07:48:10.000000 django-post_office-3.6.3/post_office/locale/
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2022-10-27 07:48:10.000000 django-post_office-3.6.3/post_office/locale/pl/
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2022-10-27 07:48:10.000000 django-post_office-3.6.3/post_office/locale/pl/LC_MESSAGES/
--rw-r--r--   0 selwin     (501) staff       (20)     2698 2017-12-06 05:45:13.000000 django-post_office-3.6.3/post_office/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 selwin     (501) staff       (20)     4300 2017-12-06 05:45:13.000000 django-post_office-3.6.3/post_office/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2022-10-27 07:48:10.000000 django-post_office-3.6.3/post_office/locale/it/
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2022-10-27 07:48:10.000000 django-post_office-3.6.3/post_office/locale/it/LC_MESSAGES/
--rw-r--r--   0 selwin     (501) staff       (20)     1573 2020-10-31 09:08:42.000000 django-post_office-3.6.3/post_office/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 selwin     (501) staff       (20)     2382 2020-10-31 09:08:42.000000 django-post_office-3.6.3/post_office/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2022-10-27 07:48:10.000000 django-post_office-3.6.3/post_office/locale/de/
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2022-10-27 07:48:10.000000 django-post_office-3.6.3/post_office/locale/de/LC_MESSAGES/
--rw-r--r--   0 selwin     (501) staff       (20)     2724 2020-02-28 08:42:53.000000 django-post_office-3.6.3/post_office/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 selwin     (501) staff       (20)     3710 2020-02-28 08:42:53.000000 django-post_office-3.6.3/post_office/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2022-10-27 07:48:10.000000 django-post_office-3.6.3/post_office/locale/ru_RU/
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2022-10-27 07:48:10.000000 django-post_office-3.6.3/post_office/locale/ru_RU/LC_MESSAGES/
--rw-r--r--   0 selwin     (501) staff       (20)     3274 2018-07-24 09:47:33.000000 django-post_office-3.6.3/post_office/locale/ru_RU/LC_MESSAGES/django.mo
--rw-r--r--   0 selwin     (501) staff       (20)     4901 2018-07-24 09:47:33.000000 django-post_office-3.6.3/post_office/locale/ru_RU/LC_MESSAGES/django.po
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2022-10-27 07:48:10.000000 django-post_office-3.6.3/post_office/locale/es/
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2022-10-27 07:48:10.000000 django-post_office-3.6.3/post_office/locale/es/LC_MESSAGES/
--rw-r--r--   0 selwin     (501) staff       (20)     1774 2021-12-21 05:02:58.000000 django-post_office-3.6.3/post_office/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 selwin     (501) staff       (20)     2420 2021-12-21 05:02:58.000000 django-post_office-3.6.3/post_office/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0 selwin     (501) staff       (20)     1534 2020-12-04 00:14:03.000000 django-post_office-3.6.3/post_office/tasks.py
--rw-r--r--   0 selwin     (501) staff       (20)     4844 2020-12-04 00:14:03.000000 django-post_office-3.6.3/post_office/lockfile.py
--rw-r--r--   0 selwin     (501) staff       (20)     5371 2022-10-07 02:18:01.000000 django-post_office-3.6.3/post_office/sanitizer.py
--rw-r--r--   0 selwin     (501) staff       (20)    13264 2022-10-27 07:35:22.000000 django-post_office-3.6.3/post_office/models.py
--rw-r--r--   0 selwin     (501) staff       (20)     1848 2020-08-22 01:45:58.000000 django-post_office-3.6.3/post_office/fields.py
--rw-r--r--   0 selwin     (501) staff       (20)     1365 2020-10-31 09:08:42.000000 django-post_office-3.6.3/post_office/validators.py
--rw-r--r--   0 selwin     (501) staff       (20)     1137 2020-02-28 08:42:53.000000 django-post_office-3.6.3/post_office/connections.py
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2022-10-27 07:48:10.000000 django-post_office-3.6.3/post_office/tests/
--rw-r--r--   0 selwin     (501) staff       (20)     2659 2020-08-22 01:45:58.000000 django-post_office-3.6.3/post_office/tests/test_forms.py
--rw-r--r--   0 selwin     (501) staff       (20)     8552 2020-02-28 08:42:53.000000 django-post_office-3.6.3/post_office/tests/test_utils.py
--rw-r--r--   0 selwin     (501) staff       (20)      459 2017-12-06 05:45:13.000000 django-post_office-3.6.3/post_office/tests/test_connections.py
--rw-r--r--   0 selwin     (501) staff       (20)    21508 2021-12-21 05:02:58.000000 django-post_office-3.6.3/post_office/tests/test_mail.py
--rw-r--r--   0 selwin     (501) staff       (20)      287 2017-12-06 05:45:13.000000 django-post_office-3.6.3/post_office/tests/__init__.py
--rw-r--r--   0 selwin     (501) staff       (20)     1943 2017-12-06 05:45:13.000000 django-post_office-3.6.3/post_office/tests/test_lockfile.py
--rw-r--r--   0 selwin     (501) staff       (20)     1129 2020-02-28 08:42:53.000000 django-post_office-3.6.3/post_office/tests/test_views.py
--rw-r--r--   0 selwin     (501) staff       (20)     6059 2018-07-24 09:47:33.000000 django-post_office-3.6.3/post_office/tests/test_commands.py
--rw-r--r--   0 selwin     (501) staff       (20)    15050 2020-02-28 08:42:53.000000 django-post_office-3.6.3/post_office/tests/test_models.py
--rw-r--r--   0 selwin     (501) staff       (20)     8271 2020-08-22 01:45:58.000000 django-post_office-3.6.3/post_office/tests/test_html_email.py
--rw-r--r--   0 selwin     (501) staff       (20)     7406 2022-10-27 07:39:26.000000 django-post_office-3.6.3/post_office/tests/test_backends.py
--rw-r--r--   0 selwin     (501) staff       (20)     1437 2017-12-06 05:45:13.000000 django-post_office-3.6.3/post_office/tests/test_cache.py
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2022-10-27 07:48:10.000000 django-post_office-3.6.3/post_office/template/
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2022-10-27 07:48:10.000000 django-post_office-3.6.3/post_office/template/backends/
--rw-r--r--   0 selwin     (501) staff       (20)     2177 2020-02-28 08:42:53.000000 django-post_office-3.6.3/post_office/template/backends/post_office.py
--rw-r--r--   0 selwin     (501) staff       (20)        0 2020-02-28 08:42:53.000000 django-post_office-3.6.3/post_office/template/backends/__init__.py
--rw-r--r--   0 selwin     (501) staff       (20)      712 2022-10-07 02:18:01.000000 django-post_office-3.6.3/post_office/template/__init__.py
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2022-10-27 07:48:10.000000 django-post_office-3.6.3/post_office/management/
--rw-r--r--   0 selwin     (501) staff       (20)        0 2017-12-06 05:45:13.000000 django-post_office-3.6.3/post_office/management/__init__.py
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2022-10-27 07:48:10.000000 django-post_office-3.6.3/post_office/management/commands/
--rw-r--r--   0 selwin     (501) staff       (20)        0 2017-12-06 05:45:13.000000 django-post_office-3.6.3/post_office/management/commands/__init__.py
--rw-r--r--   0 selwin     (501) staff       (20)     1191 2021-12-21 05:02:58.000000 django-post_office-3.6.3/post_office/management/commands/cleanup_mail.py
--rw-r--r--   0 selwin     (501) staff       (20)      855 2020-12-04 00:14:03.000000 django-post_office-3.6.3/post_office/management/commands/send_queued_mail.py
--rw-r--r--   0 selwin     (501) staff       (20)      646 2017-12-06 05:45:13.000000 django-post_office-3.6.3/post_office/cache.py
--rw-r--r--   0 selwin     (501) staff       (20)      323 2021-12-21 05:02:58.000000 django-post_office-3.6.3/post_office/__init__.py
--rw-r--r--   0 selwin     (501) staff       (20)     1072 2020-02-28 08:42:53.000000 django-post_office-3.6.3/post_office/logutils.py
--rw-r--r--   0 selwin     (501) staff       (20)      508 2022-10-07 02:18:01.000000 django-post_office-3.6.3/post_office/apps.py
--rw-r--r--   0 selwin     (501) staff       (20)     2836 2022-10-27 07:39:26.000000 django-post_office-3.6.3/post_office/backends.py
--rw-r--r--   0 selwin     (501) staff       (20)    12135 2022-10-07 09:48:58.000000 django-post_office-3.6.3/post_office/admin.py
--rw-r--r--   0 selwin     (501) staff       (20)     5572 2021-12-21 05:02:58.000000 django-post_office-3.6.3/post_office/utils.py
--rw-r--r--   0 selwin     (501) staff       (20)     3381 2020-12-04 00:14:03.000000 django-post_office-3.6.3/post_office/settings.py
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2022-10-27 07:48:10.000000 django-post_office-3.6.3/post_office/templates/
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2022-10-27 07:48:10.000000 django-post_office-3.6.3/post_office/templates/admin/
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2022-10-27 07:48:10.000000 django-post_office-3.6.3/post_office/templates/admin/post_office/
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2022-10-27 07:48:10.000000 django-post_office-3.6.3/post_office/templates/admin/post_office/emailtemplate/
--rw-r--r--   0 selwin     (501) staff       (20)     1676 2022-10-27 07:39:26.000000 django-post_office-3.6.3/post_office/templates/admin/post_office/emailtemplate/change_form.html
-drwxr-xr-x   0 selwin     (501) staff       (20)        0 2022-10-27 07:48:10.000000 django-post_office-3.6.3/post_office/templates/admin/post_office/email/
--rw-r--r--   0 selwin     (501) staff       (20)      259 2022-07-04 08:15:16.000000 django-post_office-3.6.3/post_office/templates/admin/post_office/email/change_form.html
--rw-r--r--   0 selwin     (501) staff       (20)        7 2022-10-27 07:42:52.000000 django-post_office-3.6.3/post_office/version.txt
--rw-r--r--   0 selwin     (501) staff       (20)      126 2021-12-21 05:02:58.000000 django-post_office-3.6.3/post_office/test_urls.py
--rw-r--r--   0 selwin     (501) staff       (20)       26 2017-12-06 05:45:13.000000 django-post_office-3.6.3/post_office/views.py
--rw-r--r--   0 selwin     (501) staff       (20)     3280 2021-12-21 05:02:58.000000 django-post_office-3.6.3/post_office/test_settings.py
--rw-r--r--   0 selwin     (501) staff       (20)     1053 2017-12-06 05:45:13.000000 django-post_office-3.6.3/LICENSE.txt
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.958333 django-post_office-3.7.0/
+-rw-r--r--   0 selwin     (501) staff       (20)      342 2021-12-21 05:02:58.000000 django-post_office-3.7.0/AUTHORS.rst
+-rw-r--r--   0 selwin     (501) staff       (20)     1053 2017-12-06 05:45:13.000000 django-post_office-3.7.0/LICENSE.txt
+-rw-r--r--   0 selwin     (501) staff       (20)      257 2022-10-27 07:39:26.000000 django-post_office-3.7.0/MANIFEST.in
+-rw-r--r--   0 selwin     (501) staff       (20)    26166 2023-05-30 04:47:13.958213 django-post_office-3.7.0/PKG-INFO
+-rw-r--r--   0 selwin     (501) staff       (20)    24967 2023-05-30 04:31:13.000000 django-post_office-3.7.0/README.md
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.947616 django-post_office-3.7.0/django_post_office.egg-info/
+-rw-r--r--   0 selwin     (501) staff       (20)    26166 2023-05-30 04:47:13.000000 django-post_office-3.7.0/django_post_office.egg-info/PKG-INFO
+-rw-r--r--   0 selwin     (501) staff       (20)     2714 2023-05-30 04:47:13.000000 django-post_office-3.7.0/django_post_office.egg-info/SOURCES.txt
+-rw-r--r--   0 selwin     (501) staff       (20)        1 2023-05-30 04:47:13.000000 django-post_office-3.7.0/django_post_office.egg-info/dependency_links.txt
+-rw-r--r--   0 selwin     (501) staff       (20)        1 2017-12-06 05:55:06.000000 django-post_office-3.7.0/django_post_office.egg-info/not-zip-safe
+-rw-r--r--   0 selwin     (501) staff       (20)       68 2023-05-30 04:47:13.000000 django-post_office-3.7.0/django_post_office.egg-info/requires.txt
+-rw-r--r--   0 selwin     (501) staff       (20)       12 2023-05-30 04:47:13.000000 django-post_office-3.7.0/django_post_office.egg-info/top_level.txt
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.951729 django-post_office-3.7.0/post_office/
+-rw-r--r--   0 selwin     (501) staff       (20)      323 2021-12-21 05:02:58.000000 django-post_office-3.7.0/post_office/__init__.py
+-rw-r--r--   0 selwin     (501) staff       (20)    12134 2022-11-19 11:28:46.000000 django-post_office-3.7.0/post_office/admin.py
+-rw-r--r--   0 selwin     (501) staff       (20)      508 2022-10-07 02:18:01.000000 django-post_office-3.7.0/post_office/apps.py
+-rw-r--r--   0 selwin     (501) staff       (20)     2687 2023-05-30 04:31:13.000000 django-post_office-3.7.0/post_office/backends.py
+-rw-r--r--   0 selwin     (501) staff       (20)      646 2017-12-06 05:45:13.000000 django-post_office-3.7.0/post_office/cache.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1137 2020-02-28 08:42:53.000000 django-post_office-3.7.0/post_office/connections.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1848 2020-08-22 01:45:58.000000 django-post_office-3.7.0/post_office/fields.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.945377 django-post_office-3.7.0/post_office/locale/
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.945055 django-post_office-3.7.0/post_office/locale/de/
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.952106 django-post_office-3.7.0/post_office/locale/de/LC_MESSAGES/
+-rw-r--r--   0 selwin     (501) staff       (20)     2724 2020-02-28 08:42:53.000000 django-post_office-3.7.0/post_office/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 selwin     (501) staff       (20)     3710 2020-02-28 08:42:53.000000 django-post_office-3.7.0/post_office/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.945144 django-post_office-3.7.0/post_office/locale/es/
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.952338 django-post_office-3.7.0/post_office/locale/es/LC_MESSAGES/
+-rw-r--r--   0 selwin     (501) staff       (20)     1774 2021-12-21 05:02:58.000000 django-post_office-3.7.0/post_office/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 selwin     (501) staff       (20)     2420 2021-12-21 05:02:58.000000 django-post_office-3.7.0/post_office/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.945236 django-post_office-3.7.0/post_office/locale/it/
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.952574 django-post_office-3.7.0/post_office/locale/it/LC_MESSAGES/
+-rw-r--r--   0 selwin     (501) staff       (20)     1573 2020-10-31 09:08:42.000000 django-post_office-3.7.0/post_office/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 selwin     (501) staff       (20)     2382 2020-10-31 09:08:42.000000 django-post_office-3.7.0/post_office/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.945325 django-post_office-3.7.0/post_office/locale/pl/
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.952811 django-post_office-3.7.0/post_office/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 selwin     (501) staff       (20)     2698 2017-12-06 05:45:13.000000 django-post_office-3.7.0/post_office/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 selwin     (501) staff       (20)     4300 2017-12-06 05:45:13.000000 django-post_office-3.7.0/post_office/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.945411 django-post_office-3.7.0/post_office/locale/ru_RU/
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.953081 django-post_office-3.7.0/post_office/locale/ru_RU/LC_MESSAGES/
+-rw-r--r--   0 selwin     (501) staff       (20)     3274 2018-07-24 09:47:33.000000 django-post_office-3.7.0/post_office/locale/ru_RU/LC_MESSAGES/django.mo
+-rw-r--r--   0 selwin     (501) staff       (20)     4901 2018-07-24 09:47:33.000000 django-post_office-3.7.0/post_office/locale/ru_RU/LC_MESSAGES/django.po
+-rw-r--r--   0 selwin     (501) staff       (20)     4844 2020-12-04 00:14:03.000000 django-post_office-3.7.0/post_office/lockfile.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1072 2020-02-28 08:42:53.000000 django-post_office-3.7.0/post_office/logutils.py
+-rw-r--r--   0 selwin     (501) staff       (20)    12590 2022-10-07 02:18:01.000000 django-post_office-3.7.0/post_office/mail.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.953274 django-post_office-3.7.0/post_office/management/
+-rw-r--r--   0 selwin     (501) staff       (20)        0 2017-12-06 05:45:13.000000 django-post_office-3.7.0/post_office/management/__init__.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.953583 django-post_office-3.7.0/post_office/management/commands/
+-rw-r--r--   0 selwin     (501) staff       (20)        0 2017-12-06 05:45:13.000000 django-post_office-3.7.0/post_office/management/commands/__init__.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1191 2021-12-21 05:02:58.000000 django-post_office-3.7.0/post_office/management/commands/cleanup_mail.py
+-rw-r--r--   0 selwin     (501) staff       (20)      855 2020-12-04 00:14:03.000000 django-post_office-3.7.0/post_office/management/commands/send_queued_mail.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.955220 django-post_office-3.7.0/post_office/migrations/
+-rw-r--r--   0 selwin     (501) staff       (20)     4526 2023-05-30 04:31:13.000000 django-post_office-3.7.0/post_office/migrations/0001_initial.py
+-rw-r--r--   0 selwin     (501) staff       (20)     5252 2020-02-28 08:42:53.000000 django-post_office-3.7.0/post_office/migrations/0002_add_i18n_and_backend_alias.py
+-rw-r--r--   0 selwin     (501) staff       (20)     2512 2020-02-28 08:42:53.000000 django-post_office-3.7.0/post_office/migrations/0003_longer_subject.py
+-rw-r--r--   0 selwin     (501) staff       (20)     4917 2023-05-30 04:31:13.000000 django-post_office-3.7.0/post_office/migrations/0004_auto_20160607_0901.py
+-rw-r--r--   0 selwin     (501) staff       (20)      391 2020-02-28 08:42:53.000000 django-post_office-3.7.0/post_office/migrations/0005_auto_20170515_0013.py
+-rw-r--r--   0 selwin     (501) staff       (20)      370 2020-02-28 08:42:53.000000 django-post_office-3.7.0/post_office/migrations/0006_attachment_mimetype.py
+-rw-r--r--   0 selwin     (501) staff       (20)      433 2020-02-28 08:42:53.000000 django-post_office-3.7.0/post_office/migrations/0007_auto_20170731_1342.py
+-rw-r--r--   0 selwin     (501) staff       (20)      426 2023-05-30 04:31:13.000000 django-post_office-3.7.0/post_office/migrations/0008_attachment_headers.py
+-rw-r--r--   0 selwin     (501) staff       (20)      912 2020-08-22 01:45:58.000000 django-post_office-3.7.0/post_office/migrations/0009_requeued_mode.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1481 2020-10-31 09:08:42.000000 django-post_office-3.7.0/post_office/migrations/0010_message_id.py
+-rw-r--r--   0 selwin     (501) staff       (20)      957 2020-11-05 07:48:55.000000 django-post_office-3.7.0/post_office/migrations/0011_models_help_text.py
+-rw-r--r--   0 selwin     (501) staff       (20)        0 2017-12-06 05:45:13.000000 django-post_office-3.7.0/post_office/migrations/__init__.py
+-rw-r--r--   0 selwin     (501) staff       (20)    13246 2023-05-30 04:31:13.000000 django-post_office-3.7.0/post_office/models.py
+-rw-r--r--   0 selwin     (501) staff       (20)     5371 2022-10-07 02:18:01.000000 django-post_office-3.7.0/post_office/sanitizer.py
+-rw-r--r--   0 selwin     (501) staff       (20)     3388 2023-05-30 04:31:13.000000 django-post_office-3.7.0/post_office/settings.py
+-rw-r--r--   0 selwin     (501) staff       (20)      558 2021-12-21 05:02:58.000000 django-post_office-3.7.0/post_office/signals.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1534 2020-12-04 00:14:03.000000 django-post_office-3.7.0/post_office/tasks.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.955294 django-post_office-3.7.0/post_office/template/
+-rw-r--r--   0 selwin     (501) staff       (20)      712 2022-10-07 02:18:01.000000 django-post_office-3.7.0/post_office/template/__init__.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.955599 django-post_office-3.7.0/post_office/template/backends/
+-rw-r--r--   0 selwin     (501) staff       (20)        0 2020-02-28 08:42:53.000000 django-post_office-3.7.0/post_office/template/backends/__init__.py
+-rw-r--r--   0 selwin     (501) staff       (20)     2177 2020-02-28 08:42:53.000000 django-post_office-3.7.0/post_office/template/backends/post_office.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.945783 django-post_office-3.7.0/post_office/templates/
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.945822 django-post_office-3.7.0/post_office/templates/admin/
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.945913 django-post_office-3.7.0/post_office/templates/admin/post_office/
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.955720 django-post_office-3.7.0/post_office/templates/admin/post_office/email/
+-rw-r--r--   0 selwin     (501) staff       (20)      259 2022-07-04 08:15:16.000000 django-post_office-3.7.0/post_office/templates/admin/post_office/email/change_form.html
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.955838 django-post_office-3.7.0/post_office/templates/admin/post_office/emailtemplate/
+-rw-r--r--   0 selwin     (501) staff       (20)     1676 2022-10-27 07:39:26.000000 django-post_office-3.7.0/post_office/templates/admin/post_office/emailtemplate/change_form.html
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.956237 django-post_office-3.7.0/post_office/templatetags/
+-rw-r--r--   0 selwin     (501) staff       (20)        0 2020-02-28 08:42:53.000000 django-post_office-3.7.0/post_office/templatetags/__init__.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1359 2020-08-22 01:45:58.000000 django-post_office-3.7.0/post_office/templatetags/post_office.py
+-rw-r--r--   0 selwin     (501) staff       (20)     3280 2021-12-21 05:02:58.000000 django-post_office-3.7.0/post_office/test_settings.py
+-rw-r--r--   0 selwin     (501) staff       (20)      126 2021-12-21 05:02:58.000000 django-post_office-3.7.0/post_office/test_urls.py
+drwxr-xr-x   0 selwin     (501) staff       (20)        0 2023-05-30 04:47:13.957996 django-post_office-3.7.0/post_office/tests/
+-rw-r--r--   0 selwin     (501) staff       (20)      287 2017-12-06 05:45:13.000000 django-post_office-3.7.0/post_office/tests/__init__.py
+-rw-r--r--   0 selwin     (501) staff       (20)     7406 2022-10-27 07:39:26.000000 django-post_office-3.7.0/post_office/tests/test_backends.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1437 2017-12-06 05:45:13.000000 django-post_office-3.7.0/post_office/tests/test_cache.py
+-rw-r--r--   0 selwin     (501) staff       (20)     6059 2018-07-24 09:47:33.000000 django-post_office-3.7.0/post_office/tests/test_commands.py
+-rw-r--r--   0 selwin     (501) staff       (20)      459 2017-12-06 05:45:13.000000 django-post_office-3.7.0/post_office/tests/test_connections.py
+-rw-r--r--   0 selwin     (501) staff       (20)     2659 2020-08-22 01:45:58.000000 django-post_office-3.7.0/post_office/tests/test_forms.py
+-rw-r--r--   0 selwin     (501) staff       (20)     8316 2023-05-30 04:31:13.000000 django-post_office-3.7.0/post_office/tests/test_html_email.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1943 2017-12-06 05:45:13.000000 django-post_office-3.7.0/post_office/tests/test_lockfile.py
+-rw-r--r--   0 selwin     (501) staff       (20)    21498 2023-05-30 04:31:13.000000 django-post_office-3.7.0/post_office/tests/test_mail.py
+-rw-r--r--   0 selwin     (501) staff       (20)    15050 2020-02-28 08:42:53.000000 django-post_office-3.7.0/post_office/tests/test_models.py
+-rw-r--r--   0 selwin     (501) staff       (20)     8552 2020-02-28 08:42:53.000000 django-post_office-3.7.0/post_office/tests/test_utils.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1129 2020-02-28 08:42:53.000000 django-post_office-3.7.0/post_office/tests/test_views.py
+-rw-r--r--   0 selwin     (501) staff       (20)     5572 2021-12-21 05:02:58.000000 django-post_office-3.7.0/post_office/utils.py
+-rw-r--r--   0 selwin     (501) staff       (20)     1365 2020-10-31 09:08:42.000000 django-post_office-3.7.0/post_office/validators.py
+-rw-r--r--   0 selwin     (501) staff       (20)        7 2023-05-30 04:42:50.000000 django-post_office-3.7.0/post_office/version.txt
+-rw-r--r--   0 selwin     (501) staff       (20)       26 2017-12-06 05:45:13.000000 django-post_office-3.7.0/post_office/views.py
+-rw-r--r--   0 selwin     (501) staff       (20)       38 2023-05-30 04:47:13.958363 django-post_office-3.7.0/setup.cfg
+-rw-r--r--   0 selwin     (501) staff       (20)     2435 2023-05-30 04:46:49.000000 django-post_office-3.7.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-post_office-3.6.3/django_post_office.egg-info/PKG-INFO` & `django-post_office-3.7.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,845 +1,850 @@
 Metadata-Version: 2.1
-Name: django-post-office
-Version: 3.6.3
+Name: django-post_office
+Version: 3.7.0
 Summary: A Django app to monitor and send mail asynchronously, complete with template support.
 Home-page: https://github.com/ui/django-post_office
 Author: Selwin Ong
 Author-email: selwin.ong@gmail.com
 License: MIT
-Description: # Django Post Office
-        
-        Django Post Office is a simple app to send and manage your emails in
-        Django. Some awesome features are:
-        
-        -   Allows you to send email asynchronously
-        -   Multi backend support
-        -   Supports HTML email
-        -   Supports inlined images in HTML email
-        -   Supports database based email templates
-        -   Supports multilingual email templates (i18n)
-        -   Built in scheduling support
-        -   Works well with task queues like [RQ](http://python-rq.org) or
-            [Celery](http://www.celeryproject.org)
-        -   Uses multiprocessing (and threading) to send a large number of
-            emails in parallel
-        
-        ## Dependencies
-        
-        -   [django \>= 2.2](https://djangoproject.com/)
-        -   [jsonfield](https://github.com/rpkilby/jsonfield)
-        -   [bleach](https://bleach.readthedocs.io/)
-        
-        With this optional dependency, HTML emails are nicely rendered
-        inside the Django admin backend. Without this library, all HTML tags
-        will otherwise be stripped for security reasons.
-        
-        ## Installation
-        
-        [![Build
-        Status](https://travis-ci.org/ui/django-post_office.png?branch=master)](https://travis-ci.org/ui/django-post_office) [![PyPI version](https://img.shields.io/pypi/v/django-post_office.svg)](https://pypi.org/project/django-post_office/) ![Software license](https://img.shields.io/pypi/l/django-post_office.svg)
-        
-        Install from PyPI (or [manually download from PyPI](http://pypi.python.org/pypi/django-post_office)):
-        
-        ```sh
-        pip install django-post_office
-        ```
-        
-        Add `post_office` to your INSTALLED_APPS in django's `settings.py`:
-        
-        ```python
-        INSTALLED_APPS = (
-            # other apps
-            "post_office",
-        )
-        ```
-        
-        Run `migrate`:
-        
-        ```sh
-        python manage.py migrate
-        ```
-        
-        Set `post_office.EmailBackend` as your `EMAIL_BACKEND` in Django's `settings.py`:
-        
-        ```python
-        EMAIL_BACKEND = 'post_office.EmailBackend'
-        ```
-        
-        ## Quickstart
-        
-        Send a simple email is really easy:
-        
-        ```python
-        from post_office import mail
-        
-        mail.send(
-            'recipient@example.com', # List of email addresses also accepted
-            'from@example.com',
-            subject='My email',
-            message='Hi there!',
-            html_message='Hi <strong>there</strong>!',
-        )
-        ```
-        
-        If you want to use templates, ensure that Django's admin interface is
-        enabled. Create an `EmailTemplate` instance via `admin` and do the
-        following:
-        
-        ```python
-        from post_office import mail
-        
-        mail.send(
-            'recipient@example.com', # List of email addresses also accepted
-            'from@example.com',
-            template='welcome_email', # Could be an EmailTemplate instance or name
-            context={'foo': 'bar'},
-        )
-        ```
-        
-        The above command will put your email on the queue so you can use the
-        command in your webapp without slowing down the request/response cycle
-        too much. To actually send them out, run
-        `python manage.py send_queued_mail`. You can schedule this management
-        command to run regularly via cron:
-        
-            * * * * * (/usr/bin/python manage.py send_queued_mail >> send_mail.log 2>&1)
-        
-        ## Usage
-        
-        ### mail.send()
-        
-        `mail.send` is the most important function in this library, it takes
-        these arguments:
-        
-        | Argument | Required | Description |
-        | --- | --- | --- |
-        | recipients | Yes | List of recipient email addresses |
-        | sender | No | Defaults to `settings.DEFAULT_FROM_EMAIL`, display name like `John <john@a.com>` is allowed |
-        | subject | No | Email subject (if `template` is not specified) |
-        | message | No | Email content (if `template` is not specified) |
-        | html_message | No | HTML content (if `template` is not specified) |
-        | template | No | `EmailTemplate` instance or name of template |
-        | language | No | Language in which you want to send the email in (if you have multilingual email templates). |
-        | cc | No | List of emails, will appear in `cc` field |
-        | bcc | No | List of emails, will appear in `bcc` field |
-        | attachments | No | Email attachments - a dict where the keys are the filenames and the values are files, file-like-objects or path to file |
-        | context | No | A dict, used to render templated email |
-        | headers | No | A dictionary of extra headers on the message |
-        | scheduled_time | No | A date/datetime object indicating when the email should be sent |
-        | expires_at | No | If specified, mails that are not yet sent won't be delivered after this date. |
-        | priority | No | `high`, `medium`, `low` or `now` (sent immediately) |
-        | backend | No | Alias of the backend you want to use, `default` will be used if not specified. |
-        | render_on_delivery | No | Setting this to `True` causes email to be lazily rendered during delivery. `template` is required when `render_on_delivery` is True. With this option, the full email content is never stored in the DB. May result in significant space savings if you're sending many emails using the same template. |
-        
-        Here are a few examples.
-        
-        If you just want to send out emails without using database templates.
-        You can call the `send` command without the `template` argument.
-        
-        ```python
-        from post_office import mail
-        
-        mail.send(
-            ['recipient1@example.com'],
-            'from@example.com',
-            subject='Welcome!',
-            message='Welcome home, {{ name }}!',
-            html_message='Welcome home, <b>{{ name }}</b>!',
-            headers={'Reply-to': 'reply@example.com'},
-            scheduled_time=date(2014, 1, 1),
-            context={'name': 'Alice'},
-        )
-        ```
-        
-        `post_office` is also task queue friendly. Passing `now` as priority
-        into `send_mail` will deliver the email right away (instead of queuing
-        it), regardless of how many emails you have in your queue:
-        
-        ```python
-        from post_office import mail
-        
-        mail.send(
-            ['recipient1@example.com'],
-            'from@example.com',
-            template='welcome_email',
-            context={'foo': 'bar'},
-            priority='now',
-        )
-        ```
-        
-        This is useful if you already use something like [django-rq](https://github.com/ui/django-rq) to send emails
-        asynchronously and only need to store email related activities and logs.
-        
-        If you want to send an email with attachments:
-        
-        ```python
-        from django.core.files.base import ContentFile
-        from post_office import mail
-        
-        mail.send(
-            ['recipient1@example.com'],
-            'from@example.com',
-            template='welcome_email',
-            context={'foo': 'bar'},
-            priority='now',
-            attachments={
-                'attachment1.doc': '/path/to/file/file1.doc',
-                'attachment2.txt': ContentFile('file content'),
-                'attachment3.txt': {'file': ContentFile('file content'), 'mimetype': 'text/plain'},
-            }
-        )
-        ```
-        
-        ### Template Tags and Variables
-        
-        `post-office` supports Django's template tags and variables. For
-        example, if you put `Hello, {{ name }}` in the subject line and pass in
-        `{'name': 'Alice'}` as context, you will get `Hello, Alice` as subject:
-        
-        ```python
-        from post_office.models import EmailTemplate
-        from post_office import mail
-        
-        EmailTemplate.objects.create(
-            name='morning_greeting',
-            subject='Morning, {{ name|capfirst }}',
-            content='Hi {{ name }}, how are you feeling today?',
-            html_content='Hi <strong>{{ name }}</strong>, how are you feeling today?',
-        )
-        
-        mail.send(
-            ['recipient@example.com'],
-            'from@example.com',
-            template='morning_greeting',
-            context={'name': 'alice'},
-        )
-        
-        # This will create an email with the following content:
-        subject = 'Morning, Alice',
-        content = 'Hi alice, how are you feeling today?'
-        content = 'Hi <strong>alice</strong>, how are you feeling today?'
-        ```
-        
-        ### Multilingual Email Templates
-        
-        You can easily create email templates in various different languages.
-        For example:
-        
-        ```python
-        template = EmailTemplate.objects.create(
-            name='hello',
-            subject='Hello world!',
-        )
-        
-        # Add an Indonesian version of this template:
-        indonesian_template = template.translated_templates.create(
-            language='id',
-            subject='Halo Dunia!'
-        )
-        ```
-        
-        Sending an email using template in a non default language is similarly easy:
-        
-        ```python
-        mail.send(
-            ['recipient@example.com'],
-            'from@example.com',
-            template=template, # Sends using the default template
-        )
-        
-        mail.send(
-            ['recipient@example.com'],
-            'from@example.com',
-            template=template,
-            language='id', # Sends using Indonesian template
-        )
-        ```
-        
-        ### Inlined Images
-        
-        Often one wants to render images inside a template, which are attached
-        as inlined `MIMEImage` to the outgoing email. This requires a slightly
-        modified Django Template Engine, keeping a list of inlined images, which
-        later will be added to the outgoing message.
-        
-        First we must add a special Django template backend to our list of template engines:
-        
-        ```python
-        TEMPLATES = [
-            {
-                ...
-            }, {
-                'BACKEND': 'post_office.template.backends.post_office.PostOfficeTemplates',
-                'APP_DIRS': True,
-                'DIRS': [],
-                'OPTIONS': {
-                    'context_processors': [
-                        'django.contrib.auth.context_processors.auth',
-                        'django.template.context_processors.debug',
-                        'django.template.context_processors.i18n',
-                        'django.template.context_processors.media',
-                        'django.template.context_processors.static',
-                        'django.template.context_processors.tz',
-                        'django.template.context_processors.request',
-                    ]
-                }
-            }
-        ]
-        ```
-        
-        then we must tell Post-Office to use this template engine:
-        
-        ```python
-        POST_OFFICE = {
-            'TEMPLATE_ENGINE': 'post_office',
-        }
-        ```
-        
-        In templates used to render HTML for emails add
-        
-        ```
-        {% load post_office %}
-        
-        <p>... somewhere in the body ...</p>
-        <img src="{% inline_image 'path/to/image.png' %}" />
-        ```
-        
-        Here the templatetag named `inline_image` is used to keep track of
-        inlined images. It takes a single parameter. This can either be the
-        relative path to an image file located in one of the `static`
-        directories, or the absolute path to an image file, or an image-file
-        object itself. Templates rendered using this templatetag, render a
-        reference ID for each given image, and store these images inside the
-        context of the adopted template engine. Later on, when the rendered
-        template is passed to the mailing library, those images will be
-        transferred to the email message object as `MIMEImage`-attachments.
-        
-        To send an email containing both, a plain text body and some HTML with
-        inlined images, use the following code snippet:
-        
-        ```python
-        from django.core.mail import EmailMultiAlternatives
-        
-        subject, body = "Hello", "Plain text body"
-        from_email, to_email = "no-reply@example.com", "john@example.com"
-        email_message = EmailMultiAlternatives(subject, body, from_email, [to_email])
-        template = get_template('email-template-name.html', using='post_office')
-        context = {...}
-        html = template.render(context)
-        email_message.attach_alternative(html, 'text/html')
-        template.attach_related(email_message)
-        email_message.send()
-        ```
-        
-        To send an email containing HTML with inlined images, but without a
-        plain text body, use this code snippet:
-        
-        ```python
-        from django.core.mail import EmailMultiAlternatives
-        
-        subject, from_email, to_email = "Hello", "no-reply@example.com", "john@example.com"
-        template = get_template('email-template-name.html', using='post_office')
-        context = {...}
-        html = template.render(context)
-        email_message = EmailMultiAlternatives(subject, html, from_email, [to_email])
-        email_message.content_subtype = 'html'
-        template.attach_related(email_message)
-        email_message.send()
-        ```
-        
-        ### Custom Email Backends
-        
-        By default, `post_office` uses django's `smtp.EmailBackend`. If you want
-        to use a different backend, you can do so by configuring `BACKENDS`.
-        
-        For example if you want to use [django-ses](https://github.com/hmarr/django-ses):
-        
-        ```python
-        # Put this in settings.py
-        POST_OFFICE = {
-            ...
-            'BACKENDS': {
-                'default': 'smtp.EmailBackend',
-                'ses': 'django_ses.SESBackend',
-            }
-        }
-        ```
-        
-        You can then choose what backend you want to use when sending mail:
-        
-        ```python
-        # If you omit `backend_alias` argument, `default` will be used
-        mail.send(
-            ['recipient@example.com'],
-            'from@example.com',
-            subject='Hello',
-        )
-        
-        # If you want to send using `ses` backend
-        mail.send(
-            ['recipient@example.com'],
-            'from@example.com',
-            subject='Hello',
-            backend='ses',
-        )
-        ```
-        
-        ### Management Commands
-        
-        -   `send_queued_mail` - send queued emails, those aren't successfully
-            sent will be marked as `failed`. Accepts the following arguments:
-        
-          | Argument | Description |
-          | --- | --- |
-          |`--processes` or `-p` | Number of parallel processes to send email. Defaults to 1 |
-          | `--lockfile` or `-L` | Full path to file used as lock file. Defaults to `/tmp/post_office.lock` |
-        
-        
-        -   `cleanup_mail` - delete all emails created before an X number of
-            days (defaults to 90).
-        
-        | Argument | Description |
-        | --- | --- |
-        | `--days` or `-d` | Email older than this argument will be deleted. Defaults to 90 |
-        | `--delete-attachments` | Flag to delete orphaned attachment records and files on disk. If not specified, attachments won't be deleted. |
-        
-        You may want to set these up via cron to run regularly:
-        
-            * * * * * (cd $PROJECT; python manage.py send_queued_mail --processes=1 >> $PROJECT/cron_mail.log 2>&1)
-            0 1 * * * (cd $PROJECT; python manage.py cleanup_mail --days=30 --delete-attachments >> $PROJECT/cron_mail_cleanup.log 2>&1)
-        
-        
-        ## Settings
-        
-        This section outlines all the settings and configurations that you can
-        put in Django's `settings.py` to fine tune `post-office`'s behavior.
-        
-        
-        ### Batch Size
-        
-        If you may want to limit the number of emails sent in a batch (sometimes
-        useful in a low memory environment), use the `BATCH_SIZE` argument to
-        limit the number of queued emails fetched in one batch.
-        
-        ```python
-        # Put this in settings.py
-        POST_OFFICE = {
-            ...
-            'BATCH_SIZE': 50,
-        }
-        ```
-        
-        ### Default Priority
-        
-        The default priority for emails is `medium`, but this can be altered by
-        setting `DEFAULT_PRIORITY`. Integration with asynchronous email backends
-        (e.g. based on Celery) becomes trivial when set to `now`.
-        
-        ```python
-        # Put this in settings.py
-        POST_OFFICE = {
-            ...
-            'DEFAULT_PRIORITY': 'now',
-        }
-        ```
-        
-        ### Override Recipients
-        
-        Defaults to `None`. This option is useful if you want to redirect all
-        emails to specified a few email for development purposes.
-        
-        ```python
-        # Put this in settings.py
-        POST_OFFICE = {
-            ...
-            'OVERRIDE_RECIPIENTS': ['to@example.com', 'to2@example.com'],
-        }
-        ```
-        
-        ### Message-ID
-        
-        The SMTP standard requires that each email contains a unique [Message-ID](https://tools.ietf.org/html/rfc2822#section-3.6.4). Typically the Message-ID consists of two parts separated by the `@`
-        symbol: The left part is a generated pseudo random number. The right
-        part is a constant string, typically denoting the full qualified domain
-        name of the sending server.
-        
-        By default, **Django** generates such a Message-ID during email
-        delivery. Since **django-post_office** keeps track of all delivered
-        emails, it can be very useful to create and store this Message-ID while
-        creating each email in the database. This identifier then can be looked
-        up in the Django admin backend.
-        
-        To enable this feature, add this to your Post-Office settings:
-        
-        ```python
-        # Put this in settings.py
-        POST_OFFICE = {
-            ...
-            'MESSAGE_ID_ENABLED': True,
-        }
-        ```
-        
-        It can further be fine tuned, using for instance another full qualified
-        domain name:
-        
-        ```python
-        # Put this in settings.py
-        POST_OFFICE = {
-            ...
-            'MESSAGE_ID_ENABLED': True,
-            'MESSAGE_ID_FQDN': 'example.com',
-        }
-        ```
-        
-        Otherwise, if `MESSAGE_ID_FQDN` is unset (the default),
-        **django-post_office** falls back to the DNS name of the server, which
-        is determined by the network settings of the host.
-        
-        ### Retry
-        
-        Not activated by default. You can automatically requeue failed email deliveries.
-        You can also configure failed deliveries to be retried after a specific time interval.
-        
-        ```python
-        # Put this in settings.py
-        POST_OFFICE = {
-            ...
-            'MAX_RETRIES': 4,
-            'RETRY_INTERVAL': datetime.timedelta(minutes=15),  # Schedule to be retried 15 minutes later
-        }
-        ```
-        
-        ### Log Level
-        
-        Logs are stored in the database and is browsable via Django admin.
-        The default log level is 2 (logs both successful and failed deliveries)
-        This behavior can be changed by setting `LOG_LEVEL`.
-        
-        ```python
-        # Put this in settings.py
-        POST_OFFICE = {
-            ...
-            'LOG_LEVEL': 1, # Log only failed deliveries
-        }
-        ```
-        
-        The different options are:
-        
-        * `0` logs nothing
-        * `1` logs only failed deliveries
-        * `2` logs everything (both successful and failed delivery attempts)
-        
-        ### Sending Order
-        
-        The default sending order for emails is `-priority`, but this can be
-        altered by setting `SENDING_ORDER`. For example, if you want to send
-        queued emails in FIFO order :
-        
-        ```python
-        # Put this in settings.py
-        POST_OFFICE = {
-            ...
-            'SENDING_ORDER': ['created'],
-        }
-        ```
-        
-        ### Context Field Serializer
-        
-        If you need to store complex Python objects for deferred rendering (i.e.
-        setting `render_on_delivery=True`), you can specify your own context
-        field class to store context variables. For example if you want to use
-        [django-picklefield](https://github.com/gintas/django-picklefield/tree/master/src/picklefield):
-        
-        ```python
-        # Put this in settings.py
-        POST_OFFICE = {
-            ...
-            'CONTEXT_FIELD_CLASS': 'picklefield.fields.PickledObjectField',
-        }
-        ```
-        
-        `CONTEXT_FIELD_CLASS` defaults to `jsonfield.JSONField`.
-        
-        ### Logging
-        
-        You can configure `post-office`'s logging from Django's `settings.py`.
-        For example:
-        
-        ```python
-        LOGGING = {
-            "version": 1,
-            "disable_existing_loggers": False,
-            "formatters": {
-                "post_office": {
-                    "format": "[%(levelname)s]%(asctime)s PID %(process)d: %(message)s",
-                    "datefmt": "%d-%m-%Y %H:%M:%S",
-                },
-            },
-            "handlers": {
-                "post_office": {
-                    "level": "DEBUG",
-                    "class": "logging.StreamHandler",
-                    "formatter": "post_office"
-                },
-                # If you use sentry for logging
-                'sentry': {
-                    'level': 'ERROR',
-                    'class': 'raven.contrib.django.handlers.SentryHandler',
-                },
-            },
-            'loggers': {
-                "post_office": {
-                    "handlers": ["post_office", "sentry"],
-                    "level": "INFO"
-                },
-            },
-        }
-        ```
-        
-        ### Threads
-        
-        `post-office` >= 3.0 allows you to use multiple threads to dramatically
-        speed up the speed at which emails are sent. By default, `post-office`
-        uses 5 threads per process. You can tweak this setting by changing
-        `THREADS_PER_PROCESS` setting.
-        
-        This may dramatically increase the speed of bulk email delivery,
-        depending on which email backends you use. In my tests, multi threading
-        speeds up email backends that use HTTP based (REST) delivery mechanisms
-        but doesn't seem to help SMTP based backends.
-        
-        ```python
-        # Put this in settings.py
-        POST_OFFICE = {
-            ...
-            'THREADS_PER_PROCESS': 10,
-        }
-        ```
-        
-        Performance
-        -----------
-        
-        ### Caching
-        
-        if Django's caching mechanism is configured, `post_office` will cache
-        `EmailTemplate` instances . If for some reason you want to disable
-        caching, set `POST_OFFICE_CACHE` to `False` in `settings.py`:
-        
-        ```python
-        ## All cache key will be prefixed by post_office:template:
-        ## To turn OFF caching, you need to explicitly set POST_OFFICE_CACHE to False in settings
-        POST_OFFICE_CACHE = False
-        
-        ## Optional: to use a non default cache backend, add a "post_office" entry in CACHES
-        CACHES = {
-            'post_office': {
-                'BACKEND': 'django.core.cache.backends.memcached.PyLibMCCache',
-                'LOCATION': '127.0.0.1:11211',
-            }
-        }
-        ```
-        
-        ### send_many()
-        
-        `send_many()` is much more performant (generates less database queries)
-        when sending a large number of emails. `send_many()` is almost identical
-        to `mail.send()`, with the exception that it accepts a list of keyword
-        arguments that you'd usually pass into `mail.send()`:
-        
-        ```python
-        from post_office import mail
-        
-        first_email = {
-            'sender': 'from@example.com',
-            'recipients': ['alice@example.com'],
-            'subject': 'Hi!',
-            'message': 'Hi Alice!'
-        }
-        second_email = {
-            'sender': 'from@example.com',
-            'recipients': ['bob@example.com'],
-            'subject': 'Hi!',
-            'message': 'Hi Bob!'
-        }
-        kwargs_list = [first_email, second_email]
-        
-        mail.send_many(kwargs_list)
-        ```
-        
-        Attachments are not supported with `mail.send_many()`.
-        
-        ## Running Tests
-        
-        To run the test suite:
-        
-        ```python
-        `which django-admin.py` test post_office --settings=post_office.test_settings --pythonpath=.
-        ```
-        
-        You can run the full test suite for all supported versions of Django and Python with:
-        
-        ```python
-        tox
-        ```
-        
-        or:
-        
-        ```python
-        python setup.py test
-        ```
-        
-        
-        ## Integration with Celery
-        
-        If your Django project runs in a Celery enabled configuration, you can use its worker to send out
-        queued emails. Compared to the solution with cron (see above), or the solution with uWSGI timers
-        (see below) this setup has the big advantage that queued emails are send *immediately* after they
-        have been added to the mail queue. The delivery is still performed in a separate and asynchronous
-        task, which prevents sending emails during the request/response-cycle.
-        
-        If you [configured Celery](https://docs.celeryproject.org/en/latest/userguide/application.html)
-        in your project and started the
-        [Celery worker](https://docs.celeryproject.org/en/latest/userguide/workers.html),
-        you should see something such as:
-        
-        ```
-        --------------- celery@halcyon.local v4.0 (latentcall)
-        --- ***** -----
-        -- ******* ---- [Configuration]
-        - *** --- * --- . broker:      amqp://guest@localhost:5672//
-        - ** ---------- . app:         __main__:0x1012d8590
-        - ** ---------- . concurrency: 8 (processes)
-        - ** ---------- . events:      OFF (enable -E to monitor this worker)
-        - ** ----------
-        - *** --- * --- [Queues]
-        -- ******* ---- . celery:      exchange:celery(direct) binding:celery
-        --- ***** -----
-        
-        [tasks]
-        . post_office.tasks.cleanup_expired_mails
-        . post_office.tasks.send_queued_mail
-        ```
-        
-        Delivering emails through the Celery worker must be explicitly enabled:
-        
-        ```python
-        # Put this in settings.py
-        POST_OFFICE = {
-            ...
-            'CELERY_ENABLED': True,
-        }
-        ```
-        
-        Emails will then be delivered immediately after they have been queued. In order to make this happen,
-        the project's `celery.py` setup shall invoke the
-        [autodiscoverttasks](https://docs.celeryproject.org/en/latest/reference/celery.html#celery.Celery.autodiscover_tasks)
-        function. In case of a temporary delivery failure, we might want retrying to send those emails by a
-        periodic task. This can be scheduled with a simple
-        [Celery beat configuration](https://docs.celeryproject.org/en/latest/userguide/periodic-tasks.html#entries),
-        for instance through
-        
-        ```python
-        app.conf.beat_schedule = {
-            'send-queued-mail': {
-                'task': 'post_office.tasks.send_queued_mail',
-                'schedule': 600.0,
-            },
-        }
-        ```
-        
-        The email queue now will be processed every 10 minutes. If you are using
-        [Django Celery Beat](https://django-celery-beat.readthedocs.io/en/latest/),
-        then use the Django-Admin backend and add a periodic tasks for `post_office.tasks.send_queued_mail`.
-        
-        Depending on your policy, you may also want to remove expired emails from the queue. This can be
-        done by adding another periodic tasks for `post_office.tasks.cleanup_mail`, which may run once a
-        week or month.
-        
-        
-        ## Integration with uWSGI
-        
-        If setting up Celery is too daunting and you use
-        [uWSGI](https://uwsgi-docs.readthedocs.org/en/latest/) as application
-        server, then uWSGI decorators can act as a poor men's scheduler. Just
-        add this short snipped to the project's `wsgi.py` file:
-        
-        ```python
-        from django.core.wsgi import get_wsgi_application
-        
-        application = get_wsgi_application()
-        
-        # add this block of code
-        try:
-            import uwsgidecorators
-            from django.core.management import call_command
-        
-            @uwsgidecorators.timer(10)
-            def send_queued_mail(num):
-                """Send queued mail every 10 seconds"""
-                call_command('send_queued_mail', processes=1)
-        
-        except ImportError:
-            print("uwsgidecorators not found. Cron and timers are disabled")
-        ```
-        
-        Alternatively you can also use the decorator
-        `@uwsgidecorators.cron(minute, hour, day, month, weekday)`. This will
-        schedule a task at specific times. Use `-1` to signal any time, it
-        corresponds to the `*` in cron.
-        
-        Please note that `uwsgidecorators` are available only, if the
-        application has been started with **uWSGI**. However, Django's internal
-        `./manange.py runserver` also access this file, therefore wrap the block
-        into an exception handler as shown above.
-        
-        This configuration can be useful in environments, such as Docker
-        containers, where you don't have a running cron-daemon.
-        
-        ## Signals
-        
-        Each time an email is added to the mail queue, Post Office emits a
-        special [Django
-        signal](https://docs.djangoproject.com/en/stable/topics/signals/).
-        Whenever a third party application wants to be informed about this
-        event, it shall connect a callback function to the Post Office's signal
-        handler `email_queued`, for instance:
-        
-        ```python
-        from django.dispatch import receiver
-        from post_office.signals import email_queued
-        
-        @receiver(email_queued)
-        def my_callback(sender, emails, **kwargs):
-            print("Added {} mails to the sending queue".format(len(emails)))
-        ```
-        
-        The Emails objects added to the queue are passed as list to the callback
-        handler.
-        
-        
-        ## Changelog
-        
-        Full changelog can be found [here](https://github.com/ui/django-post_office/blob/master/CHANGELOG.md).
-        
-        Created and maintained by the cool guys at [Stamps](https://stamps.co.id), Indonesia's most elegant
-        CRM/loyalty platform.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Communications :: Email
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: prevent-XSS
+License-File: LICENSE.txt
+License-File: AUTHORS.rst
+
+# Django Post Office
+
+Django Post Office is a simple app to send and manage your emails in
+Django. Some awesome features are:
+
+-   Allows you to send email asynchronously
+-   Multi backend support
+-   Supports HTML email
+-   Supports inlined images in HTML email
+-   Supports database based email templates
+-   Supports multilingual email templates (i18n)
+-   Built in scheduling support
+-   Works well with task queues like [RQ](http://python-rq.org) or
+    [Celery](http://www.celeryproject.org)
+-   Uses multiprocessing (and threading) to send a large number of
+    emails in parallel
+
+## Dependencies
+
+-   [django \>= 2.2](https://djangoproject.com/)
+-   [jsonfield](https://github.com/rpkilby/jsonfield)
+-   [bleach](https://bleach.readthedocs.io/)
+
+With this optional dependency, HTML emails are nicely rendered
+inside the Django admin backend. Without this library, all HTML tags
+will otherwise be stripped for security reasons.
+
+## Installation
+
+[![Build Status](https://github.com/ui/django-post_office/actions/workflows/test.yml/badge.svg)](https://github.com/ui/django-post_office/actions)
+[![PyPI](https://img.shields.io/pypi/pyversions/django-post_office.svg)]()
+[![PyPI version](https://img.shields.io/pypi/v/django-post_office.svg)](https://pypi.python.org/pypi/django-post_office)
+[![PyPI](https://img.shields.io/pypi/l/django-post_office.svg)]()
+
+
+```sh
+pip install django-post_office
+```
+
+Add `post_office` to your INSTALLED_APPS in django's `settings.py`:
+
+```python
+INSTALLED_APPS = (
+    # other apps
+    "post_office",
+)
+```
+
+Run `migrate`:
+
+```sh
+python manage.py migrate
+```
+
+Set `post_office.EmailBackend` as your `EMAIL_BACKEND` in Django's `settings.py`:
+
+```python
+EMAIL_BACKEND = 'post_office.EmailBackend'
+```
+
+## Quickstart
+
+Send a simple email is really easy:
+
+```python
+from post_office import mail
+
+mail.send(
+    'recipient@example.com', # List of email addresses also accepted
+    'from@example.com',
+    subject='My email',
+    message='Hi there!',
+    html_message='Hi <strong>there</strong>!',
+)
+```
+
+If you want to use templates, ensure that Django's admin interface is
+enabled. Create an `EmailTemplate` instance via `admin` and do the
+following:
+
+```python
+from post_office import mail
+
+mail.send(
+    'recipient@example.com', # List of email addresses also accepted
+    'from@example.com',
+    template='welcome_email', # Could be an EmailTemplate instance or name
+    context={'foo': 'bar'},
+)
+```
+
+The above command will put your email on the queue so you can use the
+command in your webapp without slowing down the request/response cycle
+too much. To actually send them out, run
+`python manage.py send_queued_mail`. You can schedule this management
+command to run regularly via cron:
+
+    * * * * * (/usr/bin/python manage.py send_queued_mail >> send_mail.log 2>&1)
+
+## Usage
+
+### mail.send()
+
+`mail.send` is the most important function in this library, it takes
+these arguments:
+
+| Argument | Required | Description |
+| --- | --- | --- |
+| recipients | Yes | List of recipient email addresses |
+| sender | No | Defaults to `settings.DEFAULT_FROM_EMAIL`, display name like `John <john@a.com>` is allowed |
+| subject | No | Email subject (if `template` is not specified) |
+| message | No | Email content (if `template` is not specified) |
+| html_message | No | HTML content (if `template` is not specified) |
+| template | No | `EmailTemplate` instance or name of template |
+| language | No | Language in which you want to send the email in (if you have multilingual email templates). |
+| cc | No | List of emails, will appear in `cc` field |
+| bcc | No | List of emails, will appear in `bcc` field |
+| attachments | No | Email attachments - a dict where the keys are the filenames and the values are files, file-like-objects or path to file |
+| context | No | A dict, used to render templated email |
+| headers | No | A dictionary of extra headers on the message |
+| scheduled_time | No | A date/datetime object indicating when the email should be sent |
+| expires_at | No | If specified, mails that are not yet sent won't be delivered after this date. |
+| priority | No | `high`, `medium`, `low` or `now` (sent immediately) |
+| backend | No | Alias of the backend you want to use, `default` will be used if not specified. |
+| render_on_delivery | No | Setting this to `True` causes email to be lazily rendered during delivery. `template` is required when `render_on_delivery` is True. With this option, the full email content is never stored in the DB. May result in significant space savings if you're sending many emails using the same template. |
+
+Here are a few examples.
+
+If you just want to send out emails without using database templates.
+You can call the `send` command without the `template` argument.
+
+```python
+from post_office import mail
+
+mail.send(
+    ['recipient1@example.com'],
+    'from@example.com',
+    subject='Welcome!',
+    message='Welcome home, {{ name }}!',
+    html_message='Welcome home, <b>{{ name }}</b>!',
+    headers={'Reply-to': 'reply@example.com'},
+    scheduled_time=date(2014, 1, 1),
+    context={'name': 'Alice'},
+)
+```
+
+`post_office` is also task queue friendly. Passing `now` as priority
+into `send_mail` will deliver the email right away (instead of queuing
+it), regardless of how many emails you have in your queue:
+
+```python
+from post_office import mail
+
+mail.send(
+    ['recipient1@example.com'],
+    'from@example.com',
+    template='welcome_email',
+    context={'foo': 'bar'},
+    priority='now',
+)
+```
+
+This is useful if you already use something like [django-rq](https://github.com/ui/django-rq) to send emails
+asynchronously and only need to store email related activities and logs.
+
+If you want to send an email with attachments:
+
+```python
+from django.core.files.base import ContentFile
+from post_office import mail
+
+mail.send(
+    ['recipient1@example.com'],
+    'from@example.com',
+    template='welcome_email',
+    context={'foo': 'bar'},
+    priority='now',
+    attachments={
+        'attachment1.doc': '/path/to/file/file1.doc',
+        'attachment2.txt': ContentFile('file content'),
+        'attachment3.txt': {'file': ContentFile('file content'), 'mimetype': 'text/plain'},
+    }
+)
+```
+
+### Template Tags and Variables
+
+`post-office` supports Django's template tags and variables. For
+example, if you put `Hello, {{ name }}` in the subject line and pass in
+`{'name': 'Alice'}` as context, you will get `Hello, Alice` as subject:
+
+```python
+from post_office.models import EmailTemplate
+from post_office import mail
+
+EmailTemplate.objects.create(
+    name='morning_greeting',
+    subject='Morning, {{ name|capfirst }}',
+    content='Hi {{ name }}, how are you feeling today?',
+    html_content='Hi <strong>{{ name }}</strong>, how are you feeling today?',
+)
+
+mail.send(
+    ['recipient@example.com'],
+    'from@example.com',
+    template='morning_greeting',
+    context={'name': 'alice'},
+)
+
+# This will create an email with the following content:
+subject = 'Morning, Alice',
+content = 'Hi alice, how are you feeling today?'
+content = 'Hi <strong>alice</strong>, how are you feeling today?'
+```
+
+### Multilingual Email Templates
+
+You can easily create email templates in various different languages.
+For example:
+
+```python
+template = EmailTemplate.objects.create(
+    name='hello',
+    subject='Hello world!',
+)
+
+# Add an Indonesian version of this template:
+indonesian_template = template.translated_templates.create(
+    language='id',
+    subject='Halo Dunia!'
+)
+```
+
+Sending an email using template in a non default language is similarly easy:
+
+```python
+mail.send(
+    ['recipient@example.com'],
+    'from@example.com',
+    template=template, # Sends using the default template
+)
+
+mail.send(
+    ['recipient@example.com'],
+    'from@example.com',
+    template=template,
+    language='id', # Sends using Indonesian template
+)
+```
+
+### Inlined Images
+
+Often one wants to render images inside a template, which are attached
+as inlined `MIMEImage` to the outgoing email. This requires a slightly
+modified Django Template Engine, keeping a list of inlined images, which
+later will be added to the outgoing message.
+
+First we must add a special Django template backend to our list of template engines:
+
+```python
+TEMPLATES = [
+    {
+        ...
+    }, {
+        'BACKEND': 'post_office.template.backends.post_office.PostOfficeTemplates',
+        'APP_DIRS': True,
+        'DIRS': [],
+        'OPTIONS': {
+            'context_processors': [
+                'django.contrib.auth.context_processors.auth',
+                'django.template.context_processors.debug',
+                'django.template.context_processors.i18n',
+                'django.template.context_processors.media',
+                'django.template.context_processors.static',
+                'django.template.context_processors.tz',
+                'django.template.context_processors.request',
+            ]
+        }
+    }
+]
+```
+
+then we must tell Post-Office to use this template engine:
+
+```python
+POST_OFFICE = {
+    'TEMPLATE_ENGINE': 'post_office',
+}
+```
+
+In templates used to render HTML for emails add
+
+```
+{% load post_office %}
+
+<p>... somewhere in the body ...</p>
+<img src="{% inline_image 'path/to/image.png' %}" />
+```
+
+Here the templatetag named `inline_image` is used to keep track of
+inlined images. It takes a single parameter. This can either be the
+relative path to an image file located in one of the `static`
+directories, or the absolute path to an image file, or an image-file
+object itself. Templates rendered using this templatetag, render a
+reference ID for each given image, and store these images inside the
+context of the adopted template engine. Later on, when the rendered
+template is passed to the mailing library, those images will be
+transferred to the email message object as `MIMEImage`-attachments.
+
+To send an email containing both, a plain text body and some HTML with
+inlined images, use the following code snippet:
+
+```python
+from django.core.mail import EmailMultiAlternatives
+from django.template.loader import get_template
+
+subject, body = "Hello", "Plain text body"
+from_email, to_email = "no-reply@example.com", "john@example.com"
+email_message = EmailMultiAlternatives(subject, body, from_email, [to_email])
+template = get_template('email-template-name.html', using='post_office')
+context = {...}
+html = template.render(context)
+email_message.attach_alternative(html, 'text/html')
+template.attach_related(email_message)
+email_message.send()
+```
+
+To send an email containing HTML with inlined images, but without a
+plain text body, use this code snippet:
+
+```python
+from django.core.mail import EmailMultiAlternatives
+from django.template.loader import get_template
+
+subject, from_email, to_email = "Hello", "no-reply@example.com", "john@example.com"
+template = get_template('email-template-name.html', using='post_office')
+context = {...}
+html = template.render(context)
+email_message = EmailMultiAlternatives(subject, html, from_email, [to_email])
+email_message.content_subtype = 'html'
+template.attach_related(email_message)
+email_message.send()
+```
+
+### Custom Email Backends
+
+By default, `post_office` uses django's `smtp.EmailBackend`. If you want
+to use a different backend, you can do so by configuring `BACKENDS`.
+
+For example if you want to use [django-ses](https://github.com/hmarr/django-ses):
+
+```python
+# Put this in settings.py
+POST_OFFICE = {
+    ...
+    'BACKENDS': {
+        'default': 'smtp.EmailBackend',
+        'ses': 'django_ses.SESBackend',
+    }
+}
+```
+
+You can then choose what backend you want to use when sending mail:
+
+```python
+# If you omit `backend_alias` argument, `default` will be used
+mail.send(
+    ['recipient@example.com'],
+    'from@example.com',
+    subject='Hello',
+)
+
+# If you want to send using `ses` backend
+mail.send(
+    ['recipient@example.com'],
+    'from@example.com',
+    subject='Hello',
+    backend='ses',
+)
+```
+
+### Management Commands
+
+-   `send_queued_mail` - send queued emails, those aren't successfully
+    sent will be marked as `failed`. Accepts the following arguments:
+
+  | Argument | Description |
+  | --- | --- |
+  |`--processes` or `-p` | Number of parallel processes to send email. Defaults to 1 |
+  | `--lockfile` or `-L` | Full path to file used as lock file. Defaults to `/tmp/post_office.lock` |
+
+
+-   `cleanup_mail` - delete all emails created before an X number of
+    days (defaults to 90).
+
+| Argument | Description |
+| --- | --- |
+| `--days` or `-d` | Email older than this argument will be deleted. Defaults to 90 |
+| `--delete-attachments` | Flag to delete orphaned attachment records and files on disk. If not specified, attachments won't be deleted. |
+
+You may want to set these up via cron to run regularly:
+
+    * * * * * (cd $PROJECT; python manage.py send_queued_mail --processes=1 >> $PROJECT/cron_mail.log 2>&1)
+    0 1 * * * (cd $PROJECT; python manage.py cleanup_mail --days=30 --delete-attachments >> $PROJECT/cron_mail_cleanup.log 2>&1)
+
+
+## Settings
+
+This section outlines all the settings and configurations that you can
+put in Django's `settings.py` to fine tune `post-office`'s behavior.
+
+
+### Batch Size
+
+If you may want to limit the number of emails sent in a batch (sometimes
+useful in a low memory environment), use the `BATCH_SIZE` argument to
+limit the number of queued emails fetched in one batch.
+
+```python
+# Put this in settings.py
+POST_OFFICE = {
+    ...
+    'BATCH_SIZE': 50,
+}
+```
+
+### Default Priority
+
+The default priority for emails is `medium`, but this can be altered by
+setting `DEFAULT_PRIORITY`. Integration with asynchronous email backends
+(e.g. based on Celery) becomes trivial when set to `now`.
+
+```python
+# Put this in settings.py
+POST_OFFICE = {
+    ...
+    'DEFAULT_PRIORITY': 'now',
+}
+```
+
+### Override Recipients
+
+Defaults to `None`. This option is useful if you want to redirect all
+emails to specified a few email for development purposes.
+
+```python
+# Put this in settings.py
+POST_OFFICE = {
+    ...
+    'OVERRIDE_RECIPIENTS': ['to@example.com', 'to2@example.com'],
+}
+```
+
+### Message-ID
+
+The SMTP standard requires that each email contains a unique [Message-ID](https://tools.ietf.org/html/rfc2822#section-3.6.4). Typically the Message-ID consists of two parts separated by the `@`
+symbol: The left part is a generated pseudo random number. The right
+part is a constant string, typically denoting the full qualified domain
+name of the sending server.
+
+By default, **Django** generates such a Message-ID during email
+delivery. Since **django-post_office** keeps track of all delivered
+emails, it can be very useful to create and store this Message-ID while
+creating each email in the database. This identifier then can be looked
+up in the Django admin backend.
+
+To enable this feature, add this to your Post-Office settings:
+
+```python
+# Put this in settings.py
+POST_OFFICE = {
+    ...
+    'MESSAGE_ID_ENABLED': True,
+}
+```
+
+It can further be fine tuned, using for instance another full qualified
+domain name:
+
+```python
+# Put this in settings.py
+POST_OFFICE = {
+    ...
+    'MESSAGE_ID_ENABLED': True,
+    'MESSAGE_ID_FQDN': 'example.com',
+}
+```
+
+Otherwise, if `MESSAGE_ID_FQDN` is unset (the default),
+**django-post_office** falls back to the DNS name of the server, which
+is determined by the network settings of the host.
+
+### Retry
+
+Not activated by default. You can automatically requeue failed email deliveries.
+You can also configure failed deliveries to be retried after a specific time interval.
+
+```python
+# Put this in settings.py
+POST_OFFICE = {
+    ...
+    'MAX_RETRIES': 4,
+    'RETRY_INTERVAL': datetime.timedelta(minutes=15),  # Schedule to be retried 15 minutes later
+}
+```
+
+### Log Level
+
+Logs are stored in the database and is browsable via Django admin.
+The default log level is 2 (logs both successful and failed deliveries)
+This behavior can be changed by setting `LOG_LEVEL`.
+
+```python
+# Put this in settings.py
+POST_OFFICE = {
+    ...
+    'LOG_LEVEL': 1, # Log only failed deliveries
+}
+```
+
+The different options are:
+
+* `0` logs nothing
+* `1` logs only failed deliveries
+* `2` logs everything (both successful and failed delivery attempts)
+
+### Sending Order
+
+The default sending order for emails is `-priority`, but this can be
+altered by setting `SENDING_ORDER`. For example, if you want to send
+queued emails in FIFO order :
+
+```python
+# Put this in settings.py
+POST_OFFICE = {
+    ...
+    'SENDING_ORDER': ['created'],
+}
+```
+
+### Context Field Serializer
+
+If you need to store complex Python objects for deferred rendering (i.e.
+setting `render_on_delivery=True`), you can specify your own context
+field class to store context variables. For example if you want to use
+[django-picklefield](https://github.com/gintas/django-picklefield/tree/master/src/picklefield):
+
+```python
+# Put this in settings.py
+POST_OFFICE = {
+    ...
+    'CONTEXT_FIELD_CLASS': 'picklefield.fields.PickledObjectField',
+}
+```
+
+`CONTEXT_FIELD_CLASS` defaults to `django.db.models.JSONField`.
+
+### Logging
+
+You can configure `post-office`'s logging from Django's `settings.py`.
+For example:
+
+```python
+LOGGING = {
+    "version": 1,
+    "disable_existing_loggers": False,
+    "formatters": {
+        "post_office": {
+            "format": "[%(levelname)s]%(asctime)s PID %(process)d: %(message)s",
+            "datefmt": "%d-%m-%Y %H:%M:%S",
+        },
+    },
+    "handlers": {
+        "post_office": {
+            "level": "DEBUG",
+            "class": "logging.StreamHandler",
+            "formatter": "post_office"
+        },
+        # If you use sentry for logging
+        'sentry': {
+            'level': 'ERROR',
+            'class': 'raven.contrib.django.handlers.SentryHandler',
+        },
+    },
+    'loggers': {
+        "post_office": {
+            "handlers": ["post_office", "sentry"],
+            "level": "INFO"
+        },
+    },
+}
+```
+
+### Threads
+
+`post-office` >= 3.0 allows you to use multiple threads to dramatically
+speed up the speed at which emails are sent. By default, `post-office`
+uses 5 threads per process. You can tweak this setting by changing
+`THREADS_PER_PROCESS` setting.
+
+This may dramatically increase the speed of bulk email delivery,
+depending on which email backends you use. In my tests, multi threading
+speeds up email backends that use HTTP based (REST) delivery mechanisms
+but doesn't seem to help SMTP based backends.
+
+```python
+# Put this in settings.py
+POST_OFFICE = {
+    ...
+    'THREADS_PER_PROCESS': 10,
+}
+```
+
+Performance
+-----------
+
+### Caching
+
+if Django's caching mechanism is configured, `post_office` will cache
+`EmailTemplate` instances . If for some reason you want to disable
+caching, set `POST_OFFICE_CACHE` to `False` in `settings.py`:
+
+```python
+## All cache key will be prefixed by post_office:template:
+## To turn OFF caching, you need to explicitly set POST_OFFICE_CACHE to False in settings
+POST_OFFICE_CACHE = False
+
+## Optional: to use a non default cache backend, add a "post_office" entry in CACHES
+CACHES = {
+    'post_office': {
+        'BACKEND': 'django.core.cache.backends.memcached.PyLibMCCache',
+        'LOCATION': '127.0.0.1:11211',
+    }
+}
+```
+
+### send_many()
+
+`send_many()` is much more performant (generates less database queries)
+when sending a large number of emails. `send_many()` is almost identical
+to `mail.send()`, with the exception that it accepts a list of keyword
+arguments that you'd usually pass into `mail.send()`:
+
+```python
+from post_office import mail
+
+first_email = {
+    'sender': 'from@example.com',
+    'recipients': ['alice@example.com'],
+    'subject': 'Hi!',
+    'message': 'Hi Alice!'
+}
+second_email = {
+    'sender': 'from@example.com',
+    'recipients': ['bob@example.com'],
+    'subject': 'Hi!',
+    'message': 'Hi Bob!'
+}
+kwargs_list = [first_email, second_email]
+
+mail.send_many(kwargs_list)
+```
+
+Attachments are not supported with `mail.send_many()`.
+
+## Running Tests
+
+To run the test suite:
+
+```python
+`which django-admin.py` test post_office --settings=post_office.test_settings --pythonpath=.
+```
+
+You can run the full test suite for all supported versions of Django and Python with:
+
+```python
+tox
+```
+
+or:
+
+```python
+python setup.py test
+```
+
+
+## Integration with Celery
+
+If your Django project runs in a Celery enabled configuration, you can use its worker to send out
+queued emails. Compared to the solution with cron (see above), or the solution with uWSGI timers
+(see below) this setup has the big advantage that queued emails are send *immediately* after they
+have been added to the mail queue. The delivery is still performed in a separate and asynchronous
+task, which prevents sending emails during the request/response-cycle.
+
+If you [configured Celery](https://docs.celeryproject.org/en/latest/userguide/application.html)
+in your project and started the
+[Celery worker](https://docs.celeryproject.org/en/latest/userguide/workers.html),
+you should see something such as:
+
+```
+--------------- celery@halcyon.local v4.0 (latentcall)
+--- ***** -----
+-- ******* ---- [Configuration]
+- *** --- * --- . broker:      amqp://guest@localhost:5672//
+- ** ---------- . app:         __main__:0x1012d8590
+- ** ---------- . concurrency: 8 (processes)
+- ** ---------- . events:      OFF (enable -E to monitor this worker)
+- ** ----------
+- *** --- * --- [Queues]
+-- ******* ---- . celery:      exchange:celery(direct) binding:celery
+--- ***** -----
+
+[tasks]
+. post_office.tasks.cleanup_expired_mails
+. post_office.tasks.send_queued_mail
+```
+
+Delivering emails through the Celery worker must be explicitly enabled:
+
+```python
+# Put this in settings.py
+POST_OFFICE = {
+    ...
+    'CELERY_ENABLED': True,
+}
+```
+
+Emails will then be delivered immediately after they have been queued. In order to make this happen,
+the project's `celery.py` setup shall invoke the
+[autodiscoverttasks](https://docs.celeryproject.org/en/latest/reference/celery.html#celery.Celery.autodiscover_tasks)
+function. In case of a temporary delivery failure, we might want retrying to send those emails by a
+periodic task. This can be scheduled with a simple
+[Celery beat configuration](https://docs.celeryproject.org/en/latest/userguide/periodic-tasks.html#entries),
+for instance through
+
+```python
+app.conf.beat_schedule = {
+    'send-queued-mail': {
+        'task': 'post_office.tasks.send_queued_mail',
+        'schedule': 600.0,
+    },
+}
+```
+
+The email queue now will be processed every 10 minutes. If you are using
+[Django Celery Beat](https://django-celery-beat.readthedocs.io/en/latest/),
+then use the Django-Admin backend and add a periodic tasks for `post_office.tasks.send_queued_mail`.
+
+Depending on your policy, you may also want to remove expired emails from the queue. This can be
+done by adding another periodic tasks for `post_office.tasks.cleanup_mail`, which may run once a
+week or month.
+
+
+## Integration with uWSGI
+
+If setting up Celery is too daunting and you use
+[uWSGI](https://uwsgi-docs.readthedocs.org/en/latest/) as application
+server, then uWSGI decorators can act as a poor men's scheduler. Just
+add this short snipped to the project's `wsgi.py` file:
+
+```python
+from django.core.wsgi import get_wsgi_application
+
+application = get_wsgi_application()
+
+# add this block of code
+try:
+    import uwsgidecorators
+    from django.core.management import call_command
+
+    @uwsgidecorators.timer(10)
+    def send_queued_mail(num):
+        """Send queued mail every 10 seconds"""
+        call_command('send_queued_mail', processes=1)
+
+except ImportError:
+    print("uwsgidecorators not found. Cron and timers are disabled")
+```
+
+Alternatively you can also use the decorator
+`@uwsgidecorators.cron(minute, hour, day, month, weekday)`. This will
+schedule a task at specific times. Use `-1` to signal any time, it
+corresponds to the `*` in cron.
+
+Please note that `uwsgidecorators` are available only, if the
+application has been started with **uWSGI**. However, Django's internal
+`./manange.py runserver` also access this file, therefore wrap the block
+into an exception handler as shown above.
+
+This configuration can be useful in environments, such as Docker
+containers, where you don't have a running cron-daemon.
+
+## Signals
+
+Each time an email is added to the mail queue, Post Office emits a
+special [Django
+signal](https://docs.djangoproject.com/en/stable/topics/signals/).
+Whenever a third party application wants to be informed about this
+event, it shall connect a callback function to the Post Office's signal
+handler `email_queued`, for instance:
+
+```python
+from django.dispatch import receiver
+from post_office.signals import email_queued
+
+@receiver(email_queued)
+def my_callback(sender, emails, **kwargs):
+    print("Added {} mails to the sending queue".format(len(emails)))
+```
+
+The Emails objects added to the queue are passed as list to the callback
+handler.
+
+
+## Changelog
+
+Full changelog can be found [here](https://github.com/ui/django-post_office/blob/master/CHANGELOG.md).
+
+Created and maintained by the cool guys at [Stamps](https://stamps.co.id), Indonesia's most elegant
+CRM/loyalty platform.
```

### Comparing `django-post_office-3.6.3/django_post_office.egg-info/SOURCES.txt` & `django-post_office-3.7.0/django_post_office.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/README.md` & `django-post_office-3.7.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -23,18 +23,19 @@
 
 With this optional dependency, HTML emails are nicely rendered
 inside the Django admin backend. Without this library, all HTML tags
 will otherwise be stripped for security reasons.
 
 ## Installation
 
-[![Build
-Status](https://travis-ci.org/ui/django-post_office.png?branch=master)](https://travis-ci.org/ui/django-post_office) [![PyPI version](https://img.shields.io/pypi/v/django-post_office.svg)](https://pypi.org/project/django-post_office/) ![Software license](https://img.shields.io/pypi/l/django-post_office.svg)
+[![Build Status](https://github.com/ui/django-post_office/actions/workflows/test.yml/badge.svg)](https://github.com/ui/django-post_office/actions)
+[![PyPI](https://img.shields.io/pypi/pyversions/django-post_office.svg)]()
+[![PyPI version](https://img.shields.io/pypi/v/django-post_office.svg)](https://pypi.python.org/pypi/django-post_office)
+[![PyPI](https://img.shields.io/pypi/l/django-post_office.svg)]()
 
-Install from PyPI (or [manually download from PyPI](http://pypi.python.org/pypi/django-post_office)):
 
 ```sh
 pip install django-post_office
 ```
 
 Add `post_office` to your INSTALLED_APPS in django's `settings.py`:
 
@@ -307,14 +308,15 @@
 transferred to the email message object as `MIMEImage`-attachments.
 
 To send an email containing both, a plain text body and some HTML with
 inlined images, use the following code snippet:
 
 ```python
 from django.core.mail import EmailMultiAlternatives
+from django.template.loader import get_template
 
 subject, body = "Hello", "Plain text body"
 from_email, to_email = "no-reply@example.com", "john@example.com"
 email_message = EmailMultiAlternatives(subject, body, from_email, [to_email])
 template = get_template('email-template-name.html', using='post_office')
 context = {...}
 html = template.render(context)
@@ -324,14 +326,15 @@
 ```
 
 To send an email containing HTML with inlined images, but without a
 plain text body, use this code snippet:
 
 ```python
 from django.core.mail import EmailMultiAlternatives
+from django.template.loader import get_template
 
 subject, from_email, to_email = "Hello", "no-reply@example.com", "john@example.com"
 template = get_template('email-template-name.html', using='post_office')
 context = {...}
 html = template.render(context)
 email_message = EmailMultiAlternatives(subject, html, from_email, [to_email])
 email_message.content_subtype = 'html'
@@ -546,15 +549,15 @@
 # Put this in settings.py
 POST_OFFICE = {
     ...
     'CONTEXT_FIELD_CLASS': 'picklefield.fields.PickledObjectField',
 }
 ```
 
-`CONTEXT_FIELD_CLASS` defaults to `jsonfield.JSONField`.
+`CONTEXT_FIELD_CLASS` defaults to `django.db.models.JSONField`.
 
 ### Logging
 
 You can configure `post-office`'s logging from Django's `settings.py`.
 For example:
 
 ```python
```

### Comparing `django-post_office-3.6.3/setup.py` & `django-post_office-3.7.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,16 +45,15 @@
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     zip_safe=False,
     include_package_data=True,
     package_data={'': ['README.rst']},
     install_requires=[
         'bleach[css]',
-        'django>=2.2',
-        'jsonfield>=3.0',
+        'django>=3.2',
         'pytz',
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Web Environment',
         'Framework :: Django',
         'Intended Audience :: Developers',
@@ -62,14 +61,15 @@
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Topic :: Communications :: Email',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     tests_require=TESTS_REQUIRE,
     extras_require={
         'test': TESTS_REQUIRE,
```

### Comparing `django-post_office-3.6.3/post_office/mail.py` & `django-post_office-3.7.0/post_office/mail.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/templatetags/post_office.py` & `django-post_office-3.7.0/post_office/templatetags/post_office.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/signals.py` & `django-post_office-3.7.0/post_office/signals.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/migrations/0010_message_id.py` & `django-post_office-3.7.0/post_office/migrations/0010_message_id.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/migrations/0004_auto_20160607_0901.py` & `django-post_office-3.7.0/post_office/migrations/0004_auto_20160607_0901.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Generated by Django 1.9.6 on 2016-06-07 07:01
 from django.db import migrations, models
 import django.db.models.deletion
-import jsonfield.fields
+
 import post_office.models
 
 
 class Migration(migrations.Migration):
 
     dependencies = [
         ('post_office', '0003_longer_subject'),
@@ -43,20 +43,20 @@
             model_name='email',
             name='backend_alias',
             field=models.CharField(blank=True, default='', max_length=64, verbose_name='Backend alias'),
         ),
         migrations.AlterField(
             model_name='email',
             name='context',
-            field=jsonfield.fields.JSONField(blank=True, null=True, verbose_name='Context'),
+            field=models.JSONField(blank=True, null=True, verbose_name='Context'),
         ),
         migrations.AlterField(
             model_name='email',
             name='headers',
-            field=jsonfield.fields.JSONField(blank=True, null=True, verbose_name='Headers'),
+            field=models.JSONField(blank=True, null=True, verbose_name='Headers'),
         ),
         migrations.AlterField(
             model_name='email',
             name='priority',
             field=models.PositiveSmallIntegerField(blank=True, choices=[(0, 'low'), (1, 'medium'), (2, 'high'), (3, 'now')], null=True, verbose_name='Priority'),
         ),
         migrations.AlterField(
```

### Comparing `django-post_office-3.6.3/post_office/migrations/0009_requeued_mode.py` & `django-post_office-3.7.0/post_office/migrations/0009_requeued_mode.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/migrations/0003_longer_subject.py` & `django-post_office-3.7.0/post_office/migrations/0003_longer_subject.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/migrations/0002_add_i18n_and_backend_alias.py` & `django-post_office-3.7.0/post_office/migrations/0002_add_i18n_and_backend_alias.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/migrations/0001_initial.py` & `django-post_office-3.7.0/post_office/migrations/0001_initial.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.db import models, migrations
-import jsonfield.fields
+
 import post_office.fields
 import post_office.validators
 import post_office.models
 
 
 class Migration(migrations.Migration):
 
@@ -34,16 +34,16 @@
                 ('message', models.TextField(blank=True)),
                 ('html_message', models.TextField(blank=True)),
                 ('status', models.PositiveSmallIntegerField(blank=True, null=True, db_index=True, choices=[(0, 'sent'), (1, 'failed'), (2, 'queued')])),
                 ('priority', models.PositiveSmallIntegerField(blank=True, null=True, choices=[(0, 'low'), (1, 'medium'), (2, 'high'), (3, 'now')])),
                 ('created', models.DateTimeField(auto_now_add=True, db_index=True)),
                 ('last_updated', models.DateTimeField(auto_now=True, db_index=True)),
                 ('scheduled_time', models.DateTimeField(db_index=True, null=True, blank=True)),
-                ('headers', jsonfield.fields.JSONField(null=True, blank=True)),
-                ('context', jsonfield.fields.JSONField(null=True, blank=True)),
+                ('headers', models.JSONField(null=True, blank=True)),
+                ('context', models.JSONField(null=True, blank=True)),
             ],
             options={
             },
             bases=(models.Model,),
         ),
         migrations.CreateModel(
             name='EmailTemplate',
```

### Comparing `django-post_office-3.6.3/post_office/migrations/0011_models_help_text.py` & `django-post_office-3.7.0/post_office/migrations/0011_models_help_text.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/locale/pl/LC_MESSAGES/django.mo` & `django-post_office-3.7.0/post_office/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/locale/pl/LC_MESSAGES/django.po` & `django-post_office-3.7.0/post_office/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/locale/it/LC_MESSAGES/django.mo` & `django-post_office-3.7.0/post_office/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/locale/it/LC_MESSAGES/django.po` & `django-post_office-3.7.0/post_office/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/locale/de/LC_MESSAGES/django.mo` & `django-post_office-3.7.0/post_office/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/locale/de/LC_MESSAGES/django.po` & `django-post_office-3.7.0/post_office/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/locale/ru_RU/LC_MESSAGES/django.mo` & `django-post_office-3.7.0/post_office/locale/ru_RU/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/locale/ru_RU/LC_MESSAGES/django.po` & `django-post_office-3.7.0/post_office/locale/ru_RU/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/locale/es/LC_MESSAGES/django.mo` & `django-post_office-3.7.0/post_office/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/locale/es/LC_MESSAGES/django.po` & `django-post_office-3.7.0/post_office/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/tasks.py` & `django-post_office-3.7.0/post_office/tasks.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/lockfile.py` & `django-post_office-3.7.0/post_office/lockfile.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/sanitizer.py` & `django-post_office-3.7.0/post_office/sanitizer.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/models.py` & `django-post_office-3.7.0/post_office/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 from django.core.exceptions import ValidationError
 from django.core.mail import EmailMessage, EmailMultiAlternatives
 from django.db import models
 from django.utils.encoding import smart_str
 from django.utils.translation import pgettext_lazy, gettext_lazy as _
 from django.utils import timezone
-from jsonfield import JSONField
 
 from post_office import cache
 from post_office.fields import CommaSeparatedEmailField
 
 from .connections import connections
 from .logutils import setup_loghandlers
 from .settings import context_field_class, get_log_level, get_template_engine, get_override_recipients
@@ -64,15 +63,15 @@
                                           blank=True, null=True, db_index=True,
                                           help_text=_("The scheduled sending time"))
     expires_at = models.DateTimeField(_("Expires"),
                                       blank=True, null=True,
                                       help_text=_("Email won't be sent after this timestamp"))
     message_id = models.CharField("Message-ID", null=True, max_length=255, editable=False)
     number_of_retries = models.PositiveIntegerField(null=True, blank=True)
-    headers = JSONField(_('Headers'), blank=True, null=True)
+    headers = models.JSONField(_('Headers'), blank=True, null=True)
     template = models.ForeignKey('post_office.EmailTemplate', blank=True,
                                  null=True, verbose_name=_("Email template"),
                                  on_delete=models.CASCADE)
     context = context_field_class(_('Context'), blank=True, null=True)
     backend_alias = models.CharField(_("Backend alias"), blank=True, default='',
                                      max_length=64)
 
@@ -312,15 +311,15 @@
     A model describing an email attachment.
     """
     file = models.FileField(_('File'), upload_to=get_upload_path)
     name = models.CharField(_('Name'), max_length=255, help_text=_("The original filename"))
     emails = models.ManyToManyField(Email, related_name='attachments',
                                     verbose_name=_('Emails'))
     mimetype = models.CharField(max_length=255, default='', blank=True)
-    headers = JSONField(_('Headers'), blank=True, null=True)
+    headers = models.JSONField(_('Headers'), blank=True, null=True)
 
     class Meta:
         app_label = 'post_office'
         verbose_name = _("Attachment")
         verbose_name_plural = _("Attachments")
 
     def __str__(self):
```

### Comparing `django-post_office-3.6.3/post_office/fields.py` & `django-post_office-3.7.0/post_office/fields.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/validators.py` & `django-post_office-3.7.0/post_office/validators.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/connections.py` & `django-post_office-3.7.0/post_office/connections.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/tests/test_forms.py` & `django-post_office-3.7.0/post_office/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/tests/test_utils.py` & `django-post_office-3.7.0/post_office/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/tests/test_mail.py` & `django-post_office-3.7.0/post_office/tests/test_mail.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,15 +319,15 @@
         )
         today = timezone.datetime.today()
         current_year = today.year
         self.assertEqual(email.subject, 'Subject %d' % current_year)
         self.assertEqual(email.message, 'Content %d' % current_year)
         self.assertEqual(email.html_message, 'HTML %d' % current_year)
         self.assertEqual(email.context, None)
-        self.assertEqual(email.template, None)
+        self.assertIsNotNone(email.template)
 
     def test_backend_alias(self):
         """Test backend_alias field is properly set."""
 
         email = send(recipients=['a@example.com'],
                      sender='from@example.com', message='message',
                      subject='subject')
@@ -365,25 +365,25 @@
         email = send(recipients=['to@example.com'], sender='from@example.com',
                      template=template, context=context)
         email = Email.objects.get(id=email.id)
         self.assertEqual(email.subject, 'Subject test')
         self.assertEqual(email.message, 'Content test')
         self.assertEqual(email.html_message, 'HTML test')
         self.assertEqual(email.context, None)
-        self.assertEqual(email.template, None)
+        self.assertIsNotNone(email.template)
 
         # check, if we use the Russian version
         email = send(recipients=['to@example.com'], sender='from@example.com',
                      template=russian_template, context=context)
         email = Email.objects.get(id=email.id)
         self.assertEqual(email.subject, 'предмет test')
         self.assertEqual(email.message, 'содержание test')
         self.assertEqual(email.html_message, 'HTML test')
         self.assertEqual(email.context, None)
-        self.assertEqual(email.template, None)
+        self.assertIsNotNone(email.template)
 
         # Check that send picks template with the right language
         email = send(recipients=['to@example.com'], sender='from@example.com',
                      template=template, context=context, language='ru')
         email = Email.objects.get(id=email.id)
         self.assertEqual(email.subject, 'предмет test')
 
@@ -398,15 +398,15 @@
             content='Content {{ name }}',
             html_content='HTML {{ name }}'
         )
         email = Email.objects.create(to='to@example.com', from_email='from@example.com',
                                      template=template, status=STATUS.queued)
         _send_bulk([email], uses_multiprocessing=False)
         email = Email.objects.get(id=email.id)
-        self.assertEqual(email.status, STATUS.requeued)
+        self.assertEqual(email.status, STATUS.sent)
 
     def test_retry_failed(self):
         self.assertEqual(get_retry_timedelta(), timezone.timedelta(minutes=15))
         self.assertEqual(get_max_retries(), 2)
 
         # attempt to send email for the first time
         with patch('django.utils.timezone.now', side_effect=lambda: timezone.datetime(2020, 5, 18, 8, 0, 0)):
```

### Comparing `django-post_office-3.6.3/post_office/tests/test_lockfile.py` & `django-post_office-3.7.0/post_office/tests/test_lockfile.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/tests/test_views.py` & `django-post_office-3.7.0/post_office/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/tests/test_commands.py` & `django-post_office-3.7.0/post_office/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/tests/test_models.py` & `django-post_office-3.7.0/post_office/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/tests/test_html_email.py` & `django-post_office-3.7.0/post_office/tests/test_html_email.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,20 +144,21 @@
         subject = "[Django Post-Office unit tests] attached image"
         msg = EmailMultiAlternatives(subject, body, to=['john@example.com'])
         msg.content_subtype = 'html'
         template.attach_related(msg)
         msg.send()
 
         # check that in the Email's detail view, the message is rendered
+        self.assertEqual(Email.objects.count(), 1)  # TODO: remove this
         email = Email.objects.latest('id')
         parts = email.email_message().message().walk()
         part = next(parts)
-        self.assertEqual(part.get_content_type(), 'multipart/mixed')
+        self.assertIsInstance(part, SafeMIMEMultipart)
         part = next(parts)
-        self.assertEqual(part.get_content_type(), 'text/html')
+        self.assertIsInstance(part, SafeMIMEText)
         part = next(parts)
         self.assertEqual(part.get_content_type(), 'image/png')
         content_id = part['Content-Id'][1:33]
         email_change_url = reverse('admin:post_office_email_change', args=(email.pk,))
         response = self.client.get(email_change_url, follow=True)
         self.assertContains(response, "[Django Post-Office unit tests] attached image")
         email_image_url = reverse('admin:post_office_email_image', kwargs={'pk': email.pk, 'content_id': content_id})
```

### Comparing `django-post_office-3.6.3/post_office/tests/test_backends.py` & `django-post_office-3.7.0/post_office/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/tests/test_cache.py` & `django-post_office-3.7.0/post_office/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/template/backends/post_office.py` & `django-post_office-3.7.0/post_office/template/backends/post_office.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/template/__init__.py` & `django-post_office-3.7.0/post_office/template/__init__.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/management/commands/cleanup_mail.py` & `django-post_office-3.7.0/post_office/management/commands/cleanup_mail.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/management/commands/send_queued_mail.py` & `django-post_office-3.7.0/post_office/management/commands/send_queued_mail.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/cache.py` & `django-post_office-3.7.0/post_office/cache.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/logutils.py` & `django-post_office-3.7.0/post_office/logutils.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/backends.py` & `django-post_office-3.7.0/post_office/backends.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from collections import OrderedDict
 from email.mime.base import MIMEBase
 from django.core.files.base import ContentFile
 from django.core.mail.backends.base import BaseEmailBackend
-
+import quopri
 from .settings import get_default_priority
 
-
 class EmailBackend(BaseEmailBackend):
 
     def open(self):
         pass
 
     def close(self):
         pass
@@ -30,27 +29,20 @@
         for email_message in email_messages:
             subject = email_message.subject
             from_email = email_message.from_email
             headers = email_message.extra_headers
             if email_message.reply_to:
                 reply_to_header = ", ".join(str(v) for v in email_message.reply_to)
                 headers.setdefault("Reply-To", reply_to_header)
-            message = email_message.message()
-
-            # Look for first 'text/plain' and 'text/html' alternative in email
-            plaintext_body = html_body = ''
-            for part in message.walk():
-                if part.get_content_type() == 'text/plain':
-                    plaintext_body = part.get_payload()
-                    if html_body:
-                        break
-                if part.get_content_type() == 'text/html':
-                    html_body = part.get_payload()
-                    if plaintext_body:
-                        break
+            message = email_message.body # The plaintext message is called body
+            html_body = ''  # The default if no html body can be found
+            if hasattr(email_message, 'alternatives') and len(email_message.alternatives) > 0:
+                for alternative in email_message.alternatives:
+                    if alternative[1] == 'text/html':
+                        html_body  = alternative[0]
 
             attachment_files = {}
             for attachment in email_message.attachments:
                 if isinstance(attachment, MIMEBase):
                     attachment_files[attachment.get_filename()] = {
                         'file': ContentFile(attachment.get_payload()),
                         'mimetype': attachment.get_content_type(),
@@ -58,15 +50,15 @@
                     }
                 else:
                     attachment_files[attachment[0]] = ContentFile(attachment[1])
 
             email = create(sender=from_email,
                            recipients=email_message.to, cc=email_message.cc,
                            bcc=email_message.bcc, subject=subject,
-                           message=plaintext_body, html_message=html_body,
+                           message=message, html_message=html_body,
                            headers=headers)
 
             if attachment_files:
                 attachments = create_attachments(attachment_files)
 
                 email.attachments.add(*attachments)
```

### Comparing `django-post_office-3.6.3/post_office/admin.py` & `django-post_office-3.7.0/post_office/admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
     to_display.admin_order_field = 'to'
     truncated_message_id.short_description = "Message-ID"
 
     def has_add_permission(self, request):
         return False
 
     def shortened_subject(self, instance):
-        if instance.template:
+        if instance.context:
             template_cache_key = '_subject_template_' + str(instance.template_id)
             template = getattr(self, template_cache_key, None)
             if template is None:
                 # cache compiled template to speed up rendering of list view
                 template = Template(instance.template.subject)
                 setattr(self, template_cache_key, template)
             subject = template.render(Context(instance.context))
```

### Comparing `django-post_office-3.6.3/post_office/utils.py` & `django-post_office-3.7.0/post_office/utils.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/settings.py` & `django-post_office-3.7.0/post_office/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,9 +121,9 @@
 
 
 def get_message_id_fqdn():
     return get_config().get('MESSAGE_ID_FQDN', DNS_NAME)
 
 
 CONTEXT_FIELD_CLASS = get_config().get('CONTEXT_FIELD_CLASS',
-                                       'jsonfield.JSONField')
+                                       'django.db.models.JSONField')
 context_field_class = import_string(CONTEXT_FIELD_CLASS)
```

### Comparing `django-post_office-3.6.3/post_office/templates/admin/post_office/emailtemplate/change_form.html` & `django-post_office-3.7.0/post_office/templates/admin/post_office/emailtemplate/change_form.html`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/post_office/test_settings.py` & `django-post_office-3.7.0/post_office/test_settings.py`

 * *Files identical despite different names*

### Comparing `django-post_office-3.6.3/LICENSE.txt` & `django-post_office-3.7.0/LICENSE.txt`

 * *Files identical despite different names*

