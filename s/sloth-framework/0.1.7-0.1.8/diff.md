# Comparing `tmp/sloth-framework-0.1.7.tar.gz` & `tmp/sloth-framework-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sloth-framework-0.1.7.tar", last modified: Mon May 29 02:52:45 2023, max compression
+gzip compressed data, was "sloth-framework-0.1.8.tar", last modified: Tue May 30 11:20:12 2023, max compression
```

## Comparing `sloth-framework-0.1.7.tar` & `sloth-framework-0.1.8.tar`

### file list

```diff
@@ -1,311 +1,314 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.464303 sloth-framework-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-29 02:52:45.464303 sloth-framework-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 02:52:45.464303 sloth-framework-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.432301 sloth-framework-0.1.7/sloth/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.432301 sloth-framework-0.1.7/sloth/actions/
--rw-r--r--   0 runner    (1001) docker     (123)    40271 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/actions/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/actions/inputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.432301 sloth-framework-0.1.7/sloth/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20928 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.432301 sloth-framework-0.1.7/sloth/api/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16913 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.432301 sloth-framework-0.1.7/sloth/api/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.432301 sloth-framework-0.1.7/sloth/api/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.432301 sloth-framework-0.1.7/sloth/api/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/management/commands/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/management/commands/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/management/commands/reset_passwords.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/management/commands/selenium.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/management/commands/send_web_push_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/management/commands/startserver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/management/commands/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/management/commands/sync_roles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.436301 sloth-framework-0.1.7/sloth/api/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/migrations/0002_role_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/migrations/0003_alter_application_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/migrations/0004_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/migrations/0005_task_stopped_alter_task_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/migrations/0009_pushnotification.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/migrations/0010_alter_pushnotification_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/migrations/0011_alter_application_client_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/migrations/0012_authcode.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/migrations/0013_task_partial_task_total.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/migrations/0014_email.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11090 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.428301 sloth-framework-0.1.7/sloth/api/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.436301 sloth-framework-0.1.7/sloth/api/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)    58578 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/all.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    67289 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/bootstrap-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)   155845 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    33038 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/bpmn.css
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/colorpick.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.440301 sloth-framework-0.1.7/sloth/api/static/css/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   107280 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/fonts/Eina02-Bold.f8011405.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   116316 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/fonts/Eina02-Regular.2e682693.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   112880 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   111976 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/fonts/bootstrap-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)    83304 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/fonts/bootstrap-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    47832 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/fonts/bpmn.eot
--rw-r--r--   0 runner    (1001) docker     (123)   133048 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/fonts/bpmn.svg
--rw-r--r--   0 runner    (1001) docker     (123)    47680 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/fonts/bpmn.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    16004 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/fonts/bpmn.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13028 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/fonts/bpmn.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    30702 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/icons.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.440301 sloth-framework-0.1.7/sloth/api/static/css/images/
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/images/ui-icons_444444_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/images/ui-icons_555555_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)    35973 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/jquery-ui.css
--rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/leaflet.css
--rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/select2.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     9600 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/sloth.css
--rw-r--r--   0 runner    (1001) docker     (123)    17867 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/css/trumbowyg.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.428301 sloth-framework-0.1.7/sloth/api/static/icons/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.440301 sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/
--rw-r--r--   0 runner    (1001) docker     (123)   100170 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/fontawesome.min.css
--rw-r--r--   0 runner    (1001) docker     (123)  1726692 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/fontawesome.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.444301 sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/webfonts/
--rw-r--r--   0 runner    (1001) docker     (123)   181852 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   105536 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    60520 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    23940 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    10556 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.444301 sloth-framework-0.1.7/sloth/api/static/icons/materialicons/
--rw-r--r--   0 runner    (1001) docker     (123)   174176 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   127220 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   155604 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/icons/materialicons/materialicons.css
--rw-r--r--   0 runner    (1001) docker     (123)   135988 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.444301 sloth-framework-0.1.7/sloth/api/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)    57420 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/images/click.png
--rw-r--r--   0 runner    (1001) docker     (123)    55448 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/images/hand.png
--rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/images/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/images/icon.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.444301 sloth-framework-0.1.7/sloth/api/static/images/images/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/images/images/badge.png
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/images/images/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    45136 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/images/login.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)    22817 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    21495 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/images/no-image.png
--rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/images/sloth.png
--rw-r--r--   0 runner    (1001) docker     (123)    13670 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/images/user.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.452302 sloth-framework-0.1.7/sloth/api/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/api.js
--rw-r--r--   0 runner    (1001) docker     (123)    78743 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/bootstrap.bundle.min.js
--rw-r--r--   0 runner    (1001) docker     (123)  1665279 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/bpmn.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     4098 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/colorpick.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.452302 sloth-framework-0.1.7/sloth/api/static/js/i18n/
--rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/i18n/pt-BR.js
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/jquery-3.6.0.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   520714 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/jquery-ui.js
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/jquery.binarytransport.js
--rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/jquery.mask.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    80794 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/jquery.timepicker.js
--rw-r--r--   0 runner    (1001) docker     (123)   147555 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/leaflet.js
--rw-r--r--   0 runner    (1001) docker     (123)    24103 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/masonry.pkgd.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/popper.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    43994 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/qr-scanner-worker.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    15538 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/qr-scanner.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    19927 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/qrcode.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    73163 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/select2.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    17790 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/sloth.js
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/sw.js
--rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/tests.js
--rw-r--r--   0 runner    (1001) docker     (123)    28280 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/trumbowyg.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/static/js/wpn.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.452302 sloth-framework-0.1.7/sloth/api/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.428301 sloth-framework-0.1.7/sloth/api/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.452302 sloth-framework-0.1.7/sloth/api/templates/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/actions/execute_query.html
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/actions/execute_script.html
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/actions/show_icons.html
--rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/actions/workflow.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.452302 sloth-framework-0.1.7/sloth/api/templates/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/api/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.452302 sloth-framework-0.1.7/sloth/api/templates/charts/
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/charts/bar.html
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/charts/column.html
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/charts/donut.html
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/charts/legend.html
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/charts/pie.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.456302 sloth-framework-0.1.7/sloth/api/templates/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/actions.html
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/apps.html
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/bottom.html
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/cards.html
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/dashboards.html
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/default.html
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/form.html
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/grids.html
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/header.html
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/links.html
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/menu.html
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/messages.html
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/modal.html
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/plus.html
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/report.html
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/search.html
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/settings.html
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/shortcuts.html
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/tasks.html
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/dashboard/tools.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.456302 sloth-framework-0.1.7/sloth/api/templates/inputs/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/inputs/picker.html
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/inputs/qrcode.html
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/inputs/select.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.456302 sloth-framework-0.1.7/sloth/api/templates/queryset/
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/queryset/accordion.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.456302 sloth-framework-0.1.7/sloth/api/templates/queryset/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/queryset/actions/actions.html
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/queryset/actions/batch.html
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/queryset/actions/global.html
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/queryset/calendar.html
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/queryset/cards.html
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/queryset/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/queryset/datatable.html
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/queryset/filter.html
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/queryset/filters.html
--rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/queryset/queryset.html
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/queryset/rows.html
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/queryset/scroll.html
--rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/queryset/statistics.html
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/queryset/timeline.html
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/queryset/tree.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.428301 sloth-framework-0.1.7/sloth/api/templates/renderers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.456302 sloth-framework-0.1.7/sloth/api/templates/renderers/badges/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/badges/badge.html
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/badges/boolean.html
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/badges/danger.html
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/badges/primary.html
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/badges/status.html
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/badges/warning.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.456302 sloth-framework-0.1.7/sloth/api/templates/renderers/boolean/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/boolean/thumb.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.456302 sloth-framework-0.1.7/sloth/api/templates/renderers/calendar/
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/calendar/calendar.html
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/calendar/events.html
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/calendar/legend.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.456302 sloth-framework-0.1.7/sloth/api/templates/renderers/documents/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/documents/document.html
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/documents/popup.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.456302 sloth-framework-0.1.7/sloth/api/templates/renderers/images/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/images/banner.html
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/images/group.html
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/images/image.html
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/images/round.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.456302 sloth-framework-0.1.7/sloth/api/templates/renderers/links/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/links/file.html
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/links/url.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.456302 sloth-framework-0.1.7/sloth/api/templates/renderers/maps/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/maps/geolocation.html
--rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/maps/map.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.460302 sloth-framework-0.1.7/sloth/api/templates/renderers/messages/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/messages/custom.html
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/messages/danger.html
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/messages/message.html
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/messages/primary.html
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/messages/success.html
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/messages/warning.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.460302 sloth-framework-0.1.7/sloth/api/templates/renderers/photos/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/photos/photo.html
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/photos/round.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.460302 sloth-framework-0.1.7/sloth/api/templates/renderers/programing/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/programing/strtable.html
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/programing/terminal.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.460302 sloth-framework-0.1.7/sloth/api/templates/renderers/progress/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/progress/primary.html
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/progress/success.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.460302 sloth-framework-0.1.7/sloth/api/templates/renderers/steps/
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/steps/check.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.460302 sloth-framework-0.1.7/sloth/api/templates/renderers/tags/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/tags/primary.html
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/tags/tags.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.460302 sloth-framework-0.1.7/sloth/api/templates/renderers/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/utils/formatted.html
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/utils/progress.html
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/utils/qrcode.html
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/utils/steps.html
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/renderers/utils/table.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.460302 sloth-framework-0.1.7/sloth/api/templates/themes/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/themes/dark.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.460302 sloth-framework-0.1.7/sloth/api/templates/valueset/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/valueset/2-column.html
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/valueset/field.html
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/valueset/fieldset-group.html
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/valueset/fieldset-list.html
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/valueset/fieldset-tab.html
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/valueset/fieldset.html
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/valueset/primitive.html
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/valueset/value.html
--rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templates/valueset/valueset.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.460302 sloth-framework-0.1.7/sloth/api/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/templatetags/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    12451 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/api/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.460302 sloth-framework-0.1.7/sloth/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/cloud/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      688 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/cloud/printer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6116 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/cloud/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.460302 sloth-framework-0.1.7/sloth/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/conf/local_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/conf/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.460302 sloth-framework-0.1.7/sloth/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21773 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    42840 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/core/queryset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/core/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/core/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    21103 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/core/valueset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.464303 sloth-framework-0.1.7/sloth/db/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.464303 sloth-framework-0.1.7/sloth/db/models/
--rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/db/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.464303 sloth-framework-0.1.7/sloth/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.464303 sloth-framework-0.1.7/sloth/test/selenium/
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/test/selenium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/test/selenium/browser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.464303 sloth-framework-0.1.7/sloth/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.464303 sloth-framework-0.1.7/sloth/utils/formatter/
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/utils/formatter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.464303 sloth-framework-0.1.7/sloth/utils/http/
--rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/utils/http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.464303 sloth-framework-0.1.7/sloth/utils/icons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/utils/icons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28753 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/utils/icons/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)    53105 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/utils/icons/fontawesome.py
--rw-r--r--   0 runner    (1001) docker     (123)    20959 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/utils/icons/materialicons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.464303 sloth-framework-0.1.7/sloth/utils/log/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/utils/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-29 02:52:39.000000 sloth-framework-0.1.7/sloth/utils/log/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:52:45.464303 sloth-framework-0.1.7/sloth_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-29 02:52:45.000000 sloth-framework-0.1.7/sloth_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-05-29 02:52:45.000000 sloth-framework-0.1.7/sloth_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 02:52:45.000000 sloth-framework-0.1.7/sloth_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-29 02:52:45.000000 sloth-framework-0.1.7/sloth_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-29 02:52:45.000000 sloth-framework-0.1.7/sloth_framework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.750862 sloth-framework-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-30 11:20:12.750862 sloth-framework-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 11:20:12.750862 sloth-framework-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.722862 sloth-framework-0.1.8/sloth/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.722862 sloth-framework-0.1.8/sloth/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)    40361 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/actions/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/actions/inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.722862 sloth-framework-0.1.8/sloth/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21543 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.722862 sloth-framework-0.1.8/sloth/api/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17673 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.722862 sloth-framework-0.1.8/sloth/api/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.722862 sloth-framework-0.1.8/sloth/api/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.726862 sloth-framework-0.1.8/sloth/api/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/management/commands/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/management/commands/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/management/commands/reset_passwords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/management/commands/selenium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/management/commands/send_web_push_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/management/commands/startserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/management/commands/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/management/commands/sync_roles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.726862 sloth-framework-0.1.8/sloth/api/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/migrations/0002_role_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/migrations/0003_alter_application_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/migrations/0004_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/migrations/0005_task_stopped_alter_task_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/migrations/0009_pushnotification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/migrations/0010_alter_pushnotification_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/migrations/0011_alter_application_client_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/migrations/0012_authcode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/migrations/0013_task_partial_task_total.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/migrations/0014_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11090 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.722862 sloth-framework-0.1.8/sloth/api/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.726862 sloth-framework-0.1.8/sloth/api/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    58578 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/all.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    67289 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/bootstrap-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)   155845 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    33038 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/bpmn.css
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/colorpick.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.730862 sloth-framework-0.1.8/sloth/api/static/css/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   107280 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/fonts/Eina02-Bold.f8011405.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   116316 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/fonts/Eina02-Regular.2e682693.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   112880 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   111976 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/fonts/bootstrap-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    83304 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/fonts/bootstrap-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    47832 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/fonts/bpmn.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   133048 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/fonts/bpmn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    47680 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/fonts/bpmn.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    16004 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/fonts/bpmn.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13028 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/fonts/bpmn.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    30702 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/icons.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.730862 sloth-framework-0.1.8/sloth/api/static/css/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/images/ui-icons_444444_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35973 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/jquery-ui.css
+-rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/leaflet.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16264 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/select2.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9600 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/sloth.css
+-rw-r--r--   0 runner    (1001) docker     (123)    17867 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/css/trumbowyg.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.722862 sloth-framework-0.1.8/sloth/api/static/icons/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.730862 sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/
+-rw-r--r--   0 runner    (1001) docker     (123)   100170 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/fontawesome.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)  1726692 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/fontawesome.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.730862 sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   181852 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   105536 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    60520 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23940 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    10556 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.734862 sloth-framework-0.1.8/sloth/api/static/icons/materialicons/
+-rw-r--r--   0 runner    (1001) docker     (123)   174176 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   127220 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   155604 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/icons/materialicons/materialicons.css
+-rw-r--r--   0 runner    (1001) docker     (123)   135988 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.734862 sloth-framework-0.1.8/sloth/api/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    57420 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/images/click.png
+-rw-r--r--   0 runner    (1001) docker     (123)    55448 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/images/hand.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/images/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/images/icon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.734862 sloth-framework-0.1.8/sloth/api/static/images/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/images/images/badge.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/images/images/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    45136 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/images/login.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)    22817 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    21495 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/images/no-image.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/images/sloth.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13670 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/images/user.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.738862 sloth-framework-0.1.8/sloth/api/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/api.js
+-rw-r--r--   0 runner    (1001) docker     (123)    78743 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/bootstrap.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1665279 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/bpmn.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4098 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/colorpick.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.738862 sloth-framework-0.1.8/sloth/api/static/js/i18n/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      853 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/i18n/pt-BR.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/jquery-3.6.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   520714 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/jquery-ui.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/jquery.binarytransport.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8327 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/jquery.mask.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    80794 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/jquery.timepicker.js
+-rw-r--r--   0 runner    (1001) docker     (123)   147555 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/leaflet.js
+-rw-r--r--   0 runner    (1001) docker     (123)    24103 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/masonry.pkgd.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18453 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/popper.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43994 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/qr-scanner-worker.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15538 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/qr-scanner.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19927 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/qrcode.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    73163 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/select2.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17825 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/sloth.js
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/sw.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/tests.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28280 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/trumbowyg.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/static/js/wpn.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.738862 sloth-framework-0.1.8/sloth/api/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.722862 sloth-framework-0.1.8/sloth/api/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.738862 sloth-framework-0.1.8/sloth/api/templates/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/actions/execute_query.html
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/actions/execute_script.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/actions/show_icons.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/actions/workflow.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.738862 sloth-framework-0.1.8/sloth/api/templates/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/api/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.738862 sloth-framework-0.1.8/sloth/api/templates/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/charts/bar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/charts/column.html
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/charts/donut.html
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/charts/legend.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/charts/pie.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.742862 sloth-framework-0.1.8/sloth/api/templates/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/actions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/apps.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/bottom.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/cards.html
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/dashboards.html
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/default.html
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/grids.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/header.html
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/links.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/messages.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/modal.html
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/plus.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/report.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/selector.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/settings.html
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/shortcuts.html
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/tasks.html
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/dashboard/tools.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.742862 sloth-framework-0.1.8/sloth/api/templates/inputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/inputs/picker.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/inputs/qrcode.html
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/inputs/select.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.742862 sloth-framework-0.1.8/sloth/api/templates/queryset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/queryset/accordion.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.742862 sloth-framework-0.1.8/sloth/api/templates/queryset/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/queryset/actions/actions.html
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/queryset/actions/batch.html
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/queryset/actions/global.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/queryset/calendar.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/queryset/cards.html
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/queryset/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/queryset/datatable.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/queryset/filter.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/queryset/filters.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/queryset/queryset.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/queryset/rows.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/queryset/scroll.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/queryset/statistics.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/queryset/timeline.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/queryset/tree.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.722862 sloth-framework-0.1.8/sloth/api/templates/renderers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.742862 sloth-framework-0.1.8/sloth/api/templates/renderers/badges/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/badges/badge.html
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/badges/boolean.html
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/badges/danger.html
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/badges/primary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/badges/status.html
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/badges/warning.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.742862 sloth-framework-0.1.8/sloth/api/templates/renderers/boolean/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/boolean/thumb.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.742862 sloth-framework-0.1.8/sloth/api/templates/renderers/calendar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/calendar/calendar.html
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/calendar/events.html
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/calendar/legend.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.742862 sloth-framework-0.1.8/sloth/api/templates/renderers/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/documents/document.html
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/documents/popup.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.742862 sloth-framework-0.1.8/sloth/api/templates/renderers/images/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/images/banner.html
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/images/group.html
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/images/image.html
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/images/round.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.746862 sloth-framework-0.1.8/sloth/api/templates/renderers/links/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/links/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/links/url.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.746862 sloth-framework-0.1.8/sloth/api/templates/renderers/maps/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/maps/geolocation.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4551 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/maps/map.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.746862 sloth-framework-0.1.8/sloth/api/templates/renderers/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/messages/custom.html
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/messages/danger.html
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/messages/message.html
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/messages/primary.html
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/messages/success.html
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/messages/warning.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.746862 sloth-framework-0.1.8/sloth/api/templates/renderers/photos/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/photos/photo.html
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/photos/round.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.746862 sloth-framework-0.1.8/sloth/api/templates/renderers/programing/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/programing/strtable.html
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/programing/terminal.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.746862 sloth-framework-0.1.8/sloth/api/templates/renderers/progress/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/progress/primary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/progress/success.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.746862 sloth-framework-0.1.8/sloth/api/templates/renderers/statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/statistics/cards.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.746862 sloth-framework-0.1.8/sloth/api/templates/renderers/steps/
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/steps/check.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.746862 sloth-framework-0.1.8/sloth/api/templates/renderers/tags/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/tags/primary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/tags/tags.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.746862 sloth-framework-0.1.8/sloth/api/templates/renderers/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/utils/formatted.html
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/utils/progress.html
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/utils/qrcode.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/utils/steps.html
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/renderers/utils/table.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.746862 sloth-framework-0.1.8/sloth/api/templates/themes/
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/themes/dark.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.746862 sloth-framework-0.1.8/sloth/api/templates/valueset/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/valueset/2-column.html
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/valueset/field.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/valueset/fieldset-group.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/valueset/fieldset-list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/valueset/fieldset-tab.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/valueset/fieldset.html
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/valueset/primitive.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/valueset/value.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templates/valueset/valueset.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.746862 sloth-framework-0.1.8/sloth/api/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/templatetags/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12451 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/api/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.746862 sloth-framework-0.1.8/sloth/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/cloud/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      688 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/cloud/printer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6116 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/cloud/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.746862 sloth-framework-0.1.8/sloth/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/conf/local_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/conf/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.746862 sloth-framework-0.1.8/sloth/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21773 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43817 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/core/queryset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/core/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/core/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21157 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/core/valueset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.750862 sloth-framework-0.1.8/sloth/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.750862 sloth-framework-0.1.8/sloth/db/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/db/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.750862 sloth-framework-0.1.8/sloth/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.750862 sloth-framework-0.1.8/sloth/test/selenium/
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/test/selenium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/test/selenium/browser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.750862 sloth-framework-0.1.8/sloth/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.750862 sloth-framework-0.1.8/sloth/utils/formatter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/utils/formatter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.750862 sloth-framework-0.1.8/sloth/utils/http/
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/utils/http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.750862 sloth-framework-0.1.8/sloth/utils/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/utils/icons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28753 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/utils/icons/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53105 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/utils/icons/fontawesome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20959 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/utils/icons/materialicons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.750862 sloth-framework-0.1.8/sloth/utils/log/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/utils/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-30 11:20:08.000000 sloth-framework-0.1.8/sloth/utils/log/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:20:12.750862 sloth-framework-0.1.8/sloth_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-30 11:20:12.000000 sloth-framework-0.1.8/sloth_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10240 2023-05-30 11:20:12.000000 sloth-framework-0.1.8/sloth_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:20:12.000000 sloth-framework-0.1.8/sloth_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-30 11:20:12.000000 sloth-framework-0.1.8/sloth_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 11:20:12.000000 sloth-framework-0.1.8/sloth_framework.egg-info/top_level.txt
```

### Comparing `sloth-framework-0.1.7/PKG-INFO` & `sloth-framework-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sloth-framework
-Version: 0.1.7
+Version: 0.1.8
 Summary: Metadata-based web framework for the development of management information systems
 Home-page: http://sloth.aplicativo.click/
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `sloth-framework-0.1.7/setup.py` & `sloth-framework-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open(os.path.join(root_dir, 'sloth/requirements.txt')) as file:
     requirements = file.read().strip().splitlines()
 
 os.chdir(root_dir)
 
 setup(
     name='sloth-framework',
-    version='0.1.7',
+    version='0.1.8',
     packages=find_packages(),
     install_requires=requirements,
     extras_require={
         'dev': [],
         'production': [],
     },
     include_package_data=True,
```

### Comparing `sloth-framework-0.1.7/sloth/Dockerfile` & `sloth-framework-0.1.8/sloth/Dockerfile`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/__init__.py` & `sloth-framework-0.1.8/sloth/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/__main__.py` & `sloth-framework-0.1.8/sloth/__main__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/actions/__init__.py` & `sloth-framework-0.1.8/sloth/actions/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,21 +247,24 @@
         if text:
             self.content['alert'].append(text)
 
     def danger(self, text):
         if text:
             self.content['danger'].append(text)
 
-    def parameter(self, name, default=None):
+    def parameters(self):
+        data = {}
         for token in self.request.path.split('/'):
             if '=' in token:
                 k, v = token.split('=')
-                if k == name:
-                    return v
-        return default
+                data[k] = int(v) if v.isdigit() else v
+        return data
+
+    def parameter(self, name, default=None):
+        return self.parameters().get(name, default)
 
     def objects(self, model_name):
         return apps.get_model(model_name).objects.contextualize(self.request)
 
     def clear(self):
         self.show_form = False
         for k, v in self.content.items():
```

### Comparing `sloth-framework-0.1.7/sloth/actions/fields.py` & `sloth-framework-0.1.8/sloth/actions/fields.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/actions/inputs.py` & `sloth-framework-0.1.8/sloth/actions/inputs.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/__init__.py` & `sloth-framework-0.1.8/sloth/api/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/actions.py` & `sloth-framework-0.1.8/sloth/api/actions.py`

 * *Files 3% similar despite different names*

```diff
@@ -587,7 +587,25 @@
     def view(self):
         command = self.request.GET.get('command')
         print(command)
         return command
 
     def has_permission(self, user):
         return 'test' in sys.argv
+
+
+class SetSessionLookup(actions.ActionView):
+
+    def view(self):
+        for k, v in self.parameters().items():
+            if v == 0:
+                self.request.session['session_lookups'][k]['value'] = None
+                self.request.session.save()
+                break
+            for pk, _ in self.request.session['session_lookups'][k]['choices']:
+                if str(pk) == str(v):
+                    self.request.session['session_lookups'][k]['value'] = pk
+                    self.request.session.save()
+        return 'OK'
+
+    def has_permission(self, user):
+        return user.is_authenticated
```

### Comparing `sloth-framework-0.1.7/sloth/api/backends/__init__.py` & `sloth-framework-0.1.8/sloth/api/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/dashboard.py` & `sloth-framework-0.1.8/sloth/api/dashboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,14 +159,28 @@
         self._load('search', items, app=app)
 
     def menu(self, *items, app=None, hierarchy=None, icon=None):
         item = self._load('menu', items, app=app)
         if item:
             item.update(hierarchy=hierarchy, menu_icon=icon)
 
+    def session_lookup(self, **kwargs):
+        # del self.request.session['session_lookups']
+        for key, qs in kwargs.items():
+            if 'session_lookups' not in self.request.session:
+                self.request.session['session_lookups'] = {}
+                self.request.session.save()
+            if key not in self.request.session['session_lookups'] :
+                self.request.session['session_lookups'][key] = dict(
+                    choices=[[obj.pk, str(obj)] for obj in qs],
+                    value=None,
+                    label=qs.model.metaclass().verbose_name
+                )
+                self.request.session.save()
+
     def top_menu(self, *items, modal=False, app=None):
         self._load('links', items, modal=modal, app=app)
 
     def add_link(self, url, label, app=None):
         self._item('links', url, label, app=app)
 
     def shortcuts(self, *items, app=None):
@@ -257,17 +271,18 @@
         from sloth.core.base import ValueSet
         return ValueSet(self, names)
 
     def has_attr_permission(self, user, name):
         attr = getattr(self, 'has_{}_permission'.format(name), None)
         return attr is None or attr(user)
 
-    @staticmethod
-    def objects(model_name):
-        return apps.get_model(model_name).objects
+    def objects(self, model_name):
+        qs = apps.get_model(model_name).objects.all()
+        qs.request = self.request
+        return qs.apply_role_lookups(self.request.user, self.request.session)
 
     @classmethod
     def get_attr_metadata(cls, lookup):
         attr = getattr(cls, lookup)
         template = getattr(attr, '__template__', None)
         metadata = getattr(attr, '__metadata__', None)
         if template:
```

### Comparing `sloth-framework-0.1.7/sloth/api/management/commands/cloud.py` & `sloth-framework-0.1.8/sloth/api/management/commands/cloud.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/management/commands/query.py` & `sloth-framework-0.1.8/sloth/api/management/commands/query.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/management/commands/send_web_push_notification.py` & `sloth-framework-0.1.8/sloth/api/management/commands/send_web_push_notification.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/management/commands/startserver.py` & `sloth-framework-0.1.8/sloth/api/management/commands/startserver.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/management/commands/sync.py` & `sloth-framework-0.1.8/sloth/api/management/commands/sync.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/migrations/0001_initial.py` & `sloth-framework-0.1.8/sloth/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/migrations/0002_role_user.py` & `sloth-framework-0.1.8/sloth/api/migrations/0002_role_user.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/migrations/0003_alter_application_user.py` & `sloth-framework-0.1.8/sloth/api/migrations/0003_alter_application_user.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/migrations/0004_task.py` & `sloth-framework-0.1.8/sloth/api/migrations/0004_task.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/migrations/0005_task_stopped_alter_task_message.py` & `sloth-framework-0.1.8/sloth/api/migrations/0005_task_stopped_alter_task_message.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py` & `sloth-framework-0.1.8/sloth/api/migrations/0006_role_active_alter_role_name_alter_role_scope_key_and_more.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py` & `sloth-framework-0.1.8/sloth/api/migrations/0007_alter_scope_description_alter_task_error.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py` & `sloth-framework-0.1.8/sloth/api/migrations/0008_alter_application_available_scopes_and_more.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/migrations/0009_pushnotification.py` & `sloth-framework-0.1.8/sloth/api/migrations/0009_pushnotification.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/migrations/0010_alter_pushnotification_user.py` & `sloth-framework-0.1.8/sloth/api/migrations/0010_alter_pushnotification_user.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/migrations/0011_alter_application_client_secret.py` & `sloth-framework-0.1.8/sloth/api/migrations/0011_alter_application_client_secret.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/migrations/0012_authcode.py` & `sloth-framework-0.1.8/sloth/api/migrations/0012_authcode.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/migrations/0013_task_partial_task_total.py` & `sloth-framework-0.1.8/sloth/api/migrations/0013_task_partial_task_total.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/migrations/0014_email.py` & `sloth-framework-0.1.8/sloth/api/migrations/0014_email.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/models.py` & `sloth-framework-0.1.8/sloth/api/models.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/css/all.min.css` & `sloth-framework-0.1.8/sloth/api/static/css/all.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/css/bootstrap-icons.css` & `sloth-framework-0.1.8/sloth/api/static/css/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/css/bootstrap.min.css` & `sloth-framework-0.1.8/sloth/api/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/css/bpmn.css` & `sloth-framework-0.1.8/sloth/api/static/css/bpmn.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/css/colorpick.min.css` & `sloth-framework-0.1.8/sloth/api/static/css/colorpick.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/css/fonts/Eina02-Bold.f8011405.ttf` & `sloth-framework-0.1.8/sloth/api/static/css/fonts/Eina02-Bold.f8011405.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/css/fonts/Eina02-Regular.2e682693.ttf` & `sloth-framework-0.1.8/sloth/api/static/css/fonts/Eina02-Regular.2e682693.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf` & `sloth-framework-0.1.8/sloth/api/static/css/fonts/Eina02-SemiBold.c5f9b8e3.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/css/fonts/bootstrap-icons.woff` & `sloth-framework-0.1.8/sloth/api/static/css/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/css/fonts/bootstrap-icons.woff2` & `sloth-framework-0.1.8/sloth/api/static/css/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/css/fonts/bpmn.eot` & `sloth-framework-0.1.8/sloth/api/static/css/fonts/bpmn.eot`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/css/fonts/bpmn.svg` & `sloth-framework-0.1.8/sloth/api/static/css/fonts/bpmn.svg`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/css/fonts/bpmn.ttf` & `sloth-framework-0.1.8/sloth/api/static/css/fonts/bpmn.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/css/fonts/bpmn.woff` & `sloth-framework-0.1.8/sloth/api/static/css/fonts/bpmn.woff`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/css/fonts/bpmn.woff2` & `sloth-framework-0.1.8/sloth/api/static/css/fonts/bpmn.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/css/icons.svg` & `sloth-framework-0.1.8/sloth/api/static/css/icons.svg`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/css/images/ui-icons_444444_256x240.png` & `sloth-framework-0.1.8/sloth/api/static/css/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/css/images/ui-icons_555555_256x240.png` & `sloth-framework-0.1.8/sloth/api/static/css/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/css/jquery-ui.css` & `sloth-framework-0.1.8/sloth/api/static/css/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/css/leaflet.css` & `sloth-framework-0.1.8/sloth/api/static/css/leaflet.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/css/select2.min.css` & `sloth-framework-0.1.8/sloth/api/static/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/css/sloth.css` & `sloth-framework-0.1.8/sloth/api/static/css/sloth.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/css/trumbowyg.min.css` & `sloth-framework-0.1.8/sloth/api/static/css/trumbowyg.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/fontawesome.min.css` & `sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/fontawesome.min.js` & `sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/fontawesome.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.ttf` & `sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.woff2` & `sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.ttf` & `sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.woff2` & `sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf` & `sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2` & `sloth-framework-0.1.8/sloth/api/static/icons/fontawesome/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2` & `sloth-framework-0.1.8/sloth/api/static/icons/materialicons/LDItaoyNOAY6Uewc665JcIzCKsKc_M9flwmPq_HTTw.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2` & `sloth-framework-0.1.8/sloth/api/static/icons/materialicons/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2` & `sloth-framework-0.1.8/sloth/api/static/icons/materialicons/gok-H7zzDkdnRel8-DQ6KAXJ69wP1tGnf4ZGhUcel5euIg.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/icons/materialicons/materialicons.css` & `sloth-framework-0.1.8/sloth/api/static/icons/materialicons/materialicons.css`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2` & `sloth-framework-0.1.8/sloth/api/static/icons/materialicons/oPWQ_lt5nv4pWNJpghLP75WiFR4kLh3kvmvRImcycg.woff2`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/images/click.png` & `sloth-framework-0.1.8/sloth/api/static/images/click.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/images/hand.png` & `sloth-framework-0.1.8/sloth/api/static/images/hand.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/images/icon.png` & `sloth-framework-0.1.8/sloth/api/static/images/icon.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/images/icon.svg` & `sloth-framework-0.1.8/sloth/api/static/images/icon.svg`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/images/images/badge.png` & `sloth-framework-0.1.8/sloth/api/static/images/images/badge.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/images/images/icon.png` & `sloth-framework-0.1.8/sloth/api/static/images/images/icon.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/images/login.jpeg` & `sloth-framework-0.1.8/sloth/api/static/images/login.jpeg`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/images/logo.png` & `sloth-framework-0.1.8/sloth/api/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/images/logo.svg` & `sloth-framework-0.1.8/sloth/api/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/images/no-image.png` & `sloth-framework-0.1.8/sloth/api/static/images/no-image.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/images/sloth.png` & `sloth-framework-0.1.8/sloth/api/static/images/sloth.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/images/user.png` & `sloth-framework-0.1.8/sloth/api/static/images/user.png`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/js/api.js` & `sloth-framework-0.1.8/sloth/api/static/js/api.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/js/bootstrap.bundle.min.js` & `sloth-framework-0.1.8/sloth/api/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/js/bpmn.js` & `sloth-framework-0.1.8/sloth/api/static/js/bpmn.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/js/colorpick.min.js` & `sloth-framework-0.1.8/sloth/api/static/js/colorpick.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/js/i18n/pt-BR.js` & `sloth-framework-0.1.8/sloth/api/static/js/i18n/pt-BR.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/js/jquery-3.6.0.min.js` & `sloth-framework-0.1.8/sloth/api/static/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/js/jquery-ui.js` & `sloth-framework-0.1.8/sloth/api/static/js/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/js/jquery.binarytransport.js` & `sloth-framework-0.1.8/sloth/api/static/js/jquery.binarytransport.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/js/jquery.mask.min.js` & `sloth-framework-0.1.8/sloth/api/static/js/jquery.mask.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/js/jquery.timepicker.js` & `sloth-framework-0.1.8/sloth/api/static/js/jquery.timepicker.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/js/leaflet.js` & `sloth-framework-0.1.8/sloth/api/static/js/leaflet.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/js/masonry.pkgd.min.js` & `sloth-framework-0.1.8/sloth/api/static/js/masonry.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/js/popper.min.js` & `sloth-framework-0.1.8/sloth/api/static/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/js/qr-scanner-worker.min.js` & `sloth-framework-0.1.8/sloth/api/static/js/qr-scanner-worker.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/js/qr-scanner.min.js` & `sloth-framework-0.1.8/sloth/api/static/js/qr-scanner.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/js/qrcode.min.js` & `sloth-framework-0.1.8/sloth/api/static/js/qrcode.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/js/select2.min.js` & `sloth-framework-0.1.8/sloth/api/static/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/js/sloth.js` & `sloth-framework-0.1.8/sloth/api/static/js/sloth.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -293,52 +293,32 @@
             $(this).closest('.select2-search__field').focus();
         });
         $('.fieldset-tab').map(function(i, item) {
             var fieldsets = $(this).find('.reloadable-fieldset, .reloadable-queryset');
             if (fieldsets.length == 1) fieldsets.find('.queryset-title, .fieldset-title').hide();
         });
 
-        if (window.testlogger) {
+        if (window.testlogger && false) {
             function formatValue(value) {
                 if (value && value.length == 10 && value.indexOf('-') == 4) {
                     var tokens = value.split('-');
                     if (tokens.length == 3) return tokens[2] + '/' + tokens[1] + '/' + tokens[0];
                 }
                 return value;
             }
-            $(this).find('input, textarea').not('input[type=checkbox]').blur(function() {
-                testlogger("self.enter('" + $(this).parent().find('label').html().trim().replace('*', '') + "', '" + formatValue($(this).val()) + "')")
-            });
-            $(this).find('select').change(function() {
-                testlogger("self.choose('" + $(this).parent().find('label').html().trim().replace('*', '') + "', '" + $(this).find('option:selected').html() + "')")
-            });
-            $(this).find('a:not(.btn):not(.nav-link):not(.menu-item):not(.menu-subitem):not(.search-menu-item)').click(function() {
-                testlogger("self.click_link('" + $(this).text().replace("Loading...", "").trim() + "')")
-            });
-            $(this).find('a.nav-link').click(function() {
-                testlogger("self.click_tab('" + $(this).find('.nav-link-text').text().trim() + "')")
-            });
-            $(this).find('a.menu-subitem').click(function() {
-                testlogger("self.click_menu" + $(this).data("hierarchy") + "")
-            });
-            $(this).find('a.search-menu-item').click(function() {
-                testlogger("self.search_menu('" + $(this).text().trim() + "')")
-            });
-            $(this).find('a.btn').click(function() {
-                testlogger("self.click_button('" + $(this).text().trim() + "')")
-            });
-            $(this).find('button').click(function() {
-                testlogger("self.click_button('" + $(this).text().replace("Loading...", "").trim() + "')")
-            });
-            $(this).find('input[type=checkbox]').click(function() {
-                testlogger("self.check('" + $(this).parent().find('label').html().trim().replace('*', '') + "')")
-            });
-            $(this).find('btn i.bi').click(function() {
-                testlogger("self.click_icon('" + $(this).attr('class').replace("bi ", "").replace("bi-", "") + "')")
-            });
+            //            $(this).find('input, textarea').not('input[type=checkbox]').blur(function(){testlogger("self.enter('"+$(this).parent().find('label').html().trim().replace('*', '')+"', '"+formatValue($(this).val())+"')")});
+            //            $(this).find('select').change(function(){testlogger("self.choose('"+$(this).parent().find('label').html().trim().replace('*', '')+"', '"+$(this).find('option:selected').html()+"')")});
+            //            $(this).find('a:not(.btn):not(.nav-link):not(.menu-item):not(.menu-subitem):not(.search-menu-item)').click(function(){testlogger("self.click_link('"+$(this).text().replace("Loading...", "").trim()+"')")});
+            //            $(this).find('a.nav-link').click(function(){testlogger("self.click_tab('"+$(this).find('.nav-link-text').text().trim()+"')")});
+            //            $(this).find('a.menu-subitem').click(function(){testlogger("self.click_menu"+$(this).data("hierarchy")+"")});
+            //            $(this).find('a.search-menu-item').click(function(){testlogger("self.search_menu('"+$(this).text().trim()+"')")});
+            //            $(this).find('a.btn').click(function(){testlogger("self.click_button('"+$(this).text().trim()+"')")});
+            //            $(this).find('button').click(function(){testlogger("self.click_button('"+$(this).text().replace("Loading...", "").trim()+"')")});
+            //            $(this).find('input[type=checkbox]').click(function(){testlogger("self.check('"+($(this).parent().find('label').html()||"").trim().replace('*', '')+"')")});
+            //            $(this).find('btn i.bi').click(function(){testlogger("self.click_icon('"+$(this).attr('class').replace("bi ", "").replace("bi-", "")+"')")});
         }
         return this;
     },
     refresh: function(areas) {
         function reloadAreas() {
             $('.reloadable-fieldset, .reloadable-queryset').map(
                 function(i, item) {
```

### Comparing `sloth-framework-0.1.7/sloth/api/static/js/sw.js` & `sloth-framework-0.1.8/sloth/api/static/js/sw.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/js/tests.js` & `sloth-framework-0.1.8/sloth/api/static/js/tests.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/js/trumbowyg.min.js` & `sloth-framework-0.1.8/sloth/api/static/js/trumbowyg.min.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/static/js/wpn.js` & `sloth-framework-0.1.8/sloth/api/static/js/wpn.js`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/tasks/__init__.py` & `sloth-framework-0.1.8/sloth/api/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/actions/execute_query.html` & `sloth-framework-0.1.8/sloth/api/templates/actions/execute_query.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/actions/show_icons.html` & `sloth-framework-0.1.8/sloth/api/templates/actions/show_icons.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/actions/workflow.html` & `sloth-framework-0.1.8/sloth/api/templates/actions/workflow.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/api/index.html` & `sloth-framework-0.1.8/sloth/api/templates/api/index.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/charts/bar.html` & `sloth-framework-0.1.8/sloth/api/templates/charts/bar.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/charts/column.html` & `sloth-framework-0.1.8/sloth/api/templates/charts/column.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/charts/pie.html` & `sloth-framework-0.1.8/sloth/api/templates/charts/pie.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/dashboard/actions.html` & `sloth-framework-0.1.8/sloth/api/templates/dashboard/actions.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/dashboard/apps.html` & `sloth-framework-0.1.8/sloth/api/templates/dashboard/apps.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/dashboard/base.html` & `sloth-framework-0.1.8/sloth/api/templates/dashboard/base.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/dashboard/bottom.html` & `sloth-framework-0.1.8/sloth/api/templates/dashboard/bottom.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/dashboard/cards.html` & `sloth-framework-0.1.8/sloth/api/templates/dashboard/cards.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/dashboard/footer.html` & `sloth-framework-0.1.8/sloth/api/templates/dashboard/footer.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/dashboard/form.html` & `sloth-framework-0.1.8/sloth/api/templates/dashboard/form.html`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 {% with title=self.get_verbose_name %}
     {% if title %}<h2>{{ self.get_metadata.icon|icontag }} {{ title }}</h2>{% endif %}
 {% endwith %}
 
 {% if self.get_image %}
     <div align="center">
-        <img style="max-height:75;max-width:100%;margin-bottom:30" src="{{ self.get_image }}">
+        <img style="max-width:100%" src="{{ self.get_image }}">
     </div>
 {% endif %}
 
 {% for text in self.content.info %}
     <div class="alert alert-primary" role="alert">{{ text|breaklines|safe }}</div>
 {% endfor %}
```

### Comparing `sloth-framework-0.1.7/sloth/api/templates/dashboard/grids.html` & `sloth-framework-0.1.8/sloth/api/templates/dashboard/grids.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/dashboard/header.html` & `sloth-framework-0.1.8/sloth/api/templates/dashboard/header.html`

 * *Files 1% similar despite different names*

```diff
@@ -33,19 +33,20 @@
               </li>
             {% endfor %}
           </ul>
         </div>
 
         <div class="collapse navbar-collapse">
           {% include "dashboard/search.html" %}
+          {% include "dashboard/selector.html" %}
           {% include "dashboard/tools.html" %}
           {% include "dashboard/tasks.html" %}
           {% include "dashboard/plus.html" %}
           {% include "dashboard/apps.html" %}
           {% if request.user.is_authenticated %}
-          {% include "dashboard/settings.html" %}
+            {% include "dashboard/settings.html" %}
           {% endif %}
         </div>
 
       </div>
     </nav>
 {% endif %}
```

#### html2text {}

```diff
@@ -5,12 +5,13 @@
 {{_dashboard.data.header.logo_}}]_{%_endif_%}_{%_if_dashboard.data.header.title
 %}_{{_dashboard.data.header.title_}}_{%_endif_%} {% if
 dashboard.data.header.text and not request|mobile %} {
 { dashboard.data.header.text }} {% endif %}
     * {% for action in dashboard.data.actions %}
     * {{_action.icon|icontag_}}_{{_action.label_}}
     * {% endfor %}
-{% include "dashboard/search.html" %} {% include "dashboard/tools.html" %} {%
-include "dashboard/tasks.html" %} {% include "dashboard/plus.html" %} {%
-include "dashboard/apps.html" %} {% if request.user.is_authenticated %} {%
-include "dashboard/settings.html" %} {% endif %}
+{% include "dashboard/search.html" %} {% include "dashboard/selector.html" %}
+{% include "dashboard/tools.html" %} {% include "dashboard/tasks.html" %} {%
+include "dashboard/plus.html" %} {% include "dashboard/apps.html" %} {% if
+request.user.is_authenticated %} {% include "dashboard/settings.html" %} {%
+endif %}
  {% endif %}
```

### Comparing `sloth-framework-0.1.7/sloth/api/templates/dashboard/links.html` & `sloth-framework-0.1.8/sloth/api/templates/dashboard/links.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/dashboard/menu.html` & `sloth-framework-0.1.8/sloth/api/templates/dashboard/menu.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/dashboard/messages.html` & `sloth-framework-0.1.8/sloth/api/templates/dashboard/messages.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/dashboard/modal.html` & `sloth-framework-0.1.8/sloth/api/templates/dashboard/modal.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/dashboard/plus.html` & `sloth-framework-0.1.8/sloth/api/templates/dashboard/plus.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/dashboard/report.html` & `sloth-framework-0.1.8/sloth/api/templates/dashboard/report.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/dashboard/search.html` & `sloth-framework-0.1.8/sloth/api/templates/dashboard/search.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/dashboard/settings.html` & `sloth-framework-0.1.8/sloth/api/templates/dashboard/settings.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/dashboard/shortcuts.html` & `sloth-framework-0.1.8/sloth/api/templates/dashboard/shortcuts.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/dashboard/tasks.html` & `sloth-framework-0.1.8/sloth/api/templates/dashboard/tasks.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/dashboard/tools.html` & `sloth-framework-0.1.8/sloth/api/templates/dashboard/tools.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/inputs/picker.html` & `sloth-framework-0.1.8/sloth/api/templates/inputs/picker.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/inputs/qrcode.html` & `sloth-framework-0.1.8/sloth/api/templates/inputs/qrcode.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/inputs/select.html` & `sloth-framework-0.1.8/sloth/api/templates/inputs/select.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/queryset/accordion.html` & `sloth-framework-0.1.8/sloth/api/templates/queryset/accordion.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/queryset/calendar.html` & `sloth-framework-0.1.8/sloth/api/templates/queryset/calendar.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/queryset/cards.html` & `sloth-framework-0.1.8/sloth/api/templates/queryset/cards.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/queryset/datatable.html` & `sloth-framework-0.1.8/sloth/api/templates/queryset/datatable.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/queryset/filter.html` & `sloth-framework-0.1.8/sloth/api/templates/queryset/filter.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/queryset/filters.html` & `sloth-framework-0.1.8/sloth/api/templates/queryset/filters.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/queryset/queryset.html` & `sloth-framework-0.1.8/sloth/api/templates/queryset/queryset.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 {% load tags %}
+{% if data.data or not data.metadata.on_demand %}
 <div class="reloadable-queryset {% if not data.metadata.is_admin%}box{% endif %}" id="{{ data.key }}" data-path="{{ data.path }}">
     <div class="queryset {% if data.metadata.is_admin %}admin-queryset{% endif %}" id="queryset-{{ data.uuid }}">
         {% if data.name %}
             {% if data.metadata.is_admin %}
                 <div class="queryset-title">
                     <h2>{{ data.icon|icontag }} {{ data.name }}</h2>
                 </div>
@@ -204,9 +205,10 @@
         </div>
         </div>
     </div>
     {% if data.metadata.scrollable %}
         {% include "queryset/scroll.html" %}
     {% endif %}
 </div>
+{% endif %}
```

### Comparing `sloth-framework-0.1.7/sloth/api/templates/queryset/rows.html` & `sloth-framework-0.1.8/sloth/api/templates/queryset/rows.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/queryset/scroll.html` & `sloth-framework-0.1.8/sloth/api/templates/queryset/scroll.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/queryset/statistics.html` & `sloth-framework-0.1.8/sloth/api/templates/queryset/statistics.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/queryset/timeline.html` & `sloth-framework-0.1.8/sloth/api/templates/queryset/timeline.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/queryset/tree.html` & `sloth-framework-0.1.8/sloth/api/templates/queryset/tree.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/renderers/calendar/calendar.html` & `sloth-framework-0.1.8/sloth/api/templates/renderers/calendar/calendar.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/renderers/maps/map.html` & `sloth-framework-0.1.8/sloth/api/templates/renderers/maps/map.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/renderers/programing/strtable.html` & `sloth-framework-0.1.8/sloth/api/templates/renderers/programing/strtable.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/renderers/steps/check.html` & `sloth-framework-0.1.8/sloth/api/templates/renderers/steps/check.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/renderers/utils/steps.html` & `sloth-framework-0.1.8/sloth/api/templates/renderers/utils/steps.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/renderers/utils/table.html` & `sloth-framework-0.1.8/sloth/api/templates/renderers/utils/table.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/themes/dark.html` & `sloth-framework-0.1.8/sloth/api/templates/themes/dark.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/valueset/fieldset-group.html` & `sloth-framework-0.1.8/sloth/api/templates/valueset/fieldset-group.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/valueset/fieldset-list.html` & `sloth-framework-0.1.8/sloth/api/templates/valueset/fieldset-list.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/valueset/fieldset.html` & `sloth-framework-0.1.8/sloth/api/templates/valueset/fieldset.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/valueset/value.html` & `sloth-framework-0.1.8/sloth/api/templates/valueset/value.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templates/valueset/valueset.html` & `sloth-framework-0.1.8/sloth/api/templates/valueset/valueset.html`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/templatetags/tags.py` & `sloth-framework-0.1.8/sloth/api/templatetags/tags.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/urls.py` & `sloth-framework-0.1.8/sloth/api/urls.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/api/views.py` & `sloth-framework-0.1.8/sloth/api/views.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/cloud/printer.py` & `sloth-framework-0.1.8/sloth/cloud/printer.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/cloud/server.py` & `sloth-framework-0.1.8/sloth/cloud/server.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/conf/settings.py` & `sloth-framework-0.1.8/sloth/conf/settings.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/core/base.py` & `sloth-framework-0.1.8/sloth/core/base.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/core/queryset.py` & `sloth-framework-0.1.8/sloth/core/queryset.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     def reset(self):
         self.metadata = dict(uuid=uuid1().hex if self.model is None else self.model.__name__.lower(), subset=None,
             display=[], view=[], filters={}, dfilters={}, search=None,
             page=1, limit=20, interval='', total=0, ignore=[], only={}, is_admin=False, ordering=[],
             actions=[], attach=[], template=None, attr=None, source=None, aggregations=[], calendar=None,
             global_actions=[], batch_actions=[], inline_actions=[], lookups=[], collapsed=True, compact=False,
-            verbose_name=None, related_field=None, scrollable=False, tree=None
+            verbose_name=None, related_field=None, scrollable=False, tree=None, session_lookups=[], on_demand=False
         )
         if self.model and getattr(self.model.metaclass(), 'autouser', False):
             self.lookups(autouser='pk')
             self.ignore('autouser')
 
     def _clone(self):
         clone = super()._clone()
@@ -77,28 +77,38 @@
         return self.ignore(name)
 
     def role_lookups(self, *names, **scopes):
         for name in names:
             self.metadata['lookups'].append((name, scopes))
         return self
 
+    def session_lookups(self, *names, **scopes):
+        for name in names or ('Usuário',):
+            self.metadata['session_lookups'].append((name, scopes))
+        return self
+
     def lookups(self, name='Usuário', *names, **scopes):
         self.role_lookups(*((name,) + names), **scopes)
         return self
 
     def readonly(self):
         for key in ('actions', 'inline_actions', 'batch_actions'):
             self.metadata[key].clear()
         return self
 
     def has_permission(self, user):
         if user.is_authenticated:
             return user.is_superuser or user.roles.contains(*(t[0] for t in self.metadata['lookups']))
         return False
 
+    def on_demand(self):
+        qs = self.clone()
+        qs.metadata['on_demand'] = True
+        return qs
+
     def has_attr_permission(self, user, name):
         if user.is_superuser:
             return True
         qs = self.model.objects
         if name == 'all' or name in qs.metadata['attach']:
             return qs.has_permission(user)
         return getattr(self._clone(), name)().has_permission(user)
@@ -111,15 +121,16 @@
         if recursive:
             for attach in self.metadata['attach']:
                 allowed.extend(getattr(self._clone(), attach)().get_allowed_attrs(recursive=False))
         for view in self.metadata['view']:
             allowed.append('view' if view['name'] == 'self' else view['name'])
         return allowed
 
-    def apply_role_lookups(self, user):
+    def apply_role_lookups(self, user, session=None):
+        qs = None
         if user.is_superuser:
             return self
         else:
             for field_name, role_names in self.metadata['only'].items():
                 if not self.request.user.roles.contains(*role_names):
                     self.ignore(field_name)
         if self.metadata['lookups']:
@@ -130,18 +141,28 @@
                         if scope_key == 'username':
                             lookups.append(Q(**{scope_value_attr: user.username}))
                         else:
                             for scope_value in user.roles.filter(active=True, name=name, scope_key=scope_key).values_list('scope_value', flat=True):
                                 lookups.append(Q(**{scope_value_attr: scope_value}))
                 else:
                     if user.roles.contains(name):
-                        return self
+                        qs = self
+            qs = self.filter(reduce(operator.__or__, lookups)) if lookups else self
+        if session and self.metadata['session_lookups']:
+            lookups = []
+            for name, scopes in self.metadata['session_lookups']:
+                if user.roles.contains(name):
+                    for k, v in scopes.items():
+                        if v in session['session_lookups'] and session['session_lookups'][v]['value']:
+                            lookups.append(Q(**{k: session['session_lookups'][v]['value']}))
             if lookups:
-                return self.filter(reduce(operator.__or__, lookups))
-        return self.none() if self.metadata['is_admin'] else self
+                qs = qs.filter(reduce(operator.__or__, lookups))
+        if qs is None:
+            return self.none() if self.metadata['is_admin'] else self
+        return qs
 
     def append(self, *names):
         from sloth.core.valueset import ValueSet
         return ValueSet(self, names)
 
     def value_set(self, *names):
         from sloth.core.valueset import ValueSet
@@ -488,15 +509,15 @@
                 data.update(attach=attach)
 
             if not lazy:
                 collapsed = bool(self.request and self.request.GET.get('collapsed', self.metadata['collapsed']) or 0)
                 subset = self.request and self.request.GET.get('subset', 'all') or 'all'
                 data['metadata'].update(
                     search=search, display=display, filters=filters, pagination=pagination,
-                    collapsed=collapsed, subset=subset,
+                    collapsed=collapsed, subset=subset, on_demand=self.metadata['on_demand'],
                     compact=self.metadata['compact'], is_admin=self.metadata['is_admin']# , state=self.dumps()
                 )
                 if calendar:
                     data['metadata']['calendar'] = calendar
                 if self.metadata['tree']:
                     data['metadata']['tree'] = self.metadata['tree']
 
@@ -836,15 +857,15 @@
                 raise JsonReadyResponseException(
                     self.process_request(request).choices(request)
                 )
             if 'tree-nodes' in request.GET:
                 raise JsonReadyResponseException(
                     self.process_request(request).tree_nodes()
                 )
-            component = self.process_request(request).apply_role_lookups(request.user)
+            component = self.process_request(request).apply_role_lookups(request.user, request.session)
             if request.path.startswith('/app/'):
                 raise HtmlReadyResponseException(component.html())
             else:
                 meta = request.path.startswith('/meta/')
                 raise JsonReadyResponseException(component.serialize(wrap=meta))
             return self.apply_role_lookups(request.user)
         return self
```

### Comparing `sloth-framework-0.1.7/sloth/core/statistics.py` & `sloth-framework-0.1.8/sloth/core/statistics.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/core/validation.py` & `sloth-framework-0.1.8/sloth/core/validation.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/core/valueset.py` & `sloth-framework-0.1.8/sloth/core/valueset.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,14 +250,15 @@
                         qs = value if isinstance(value, QuerySet) else value.filter() # ManyRelatedManager
                         qs.instantiator = self.instance
                         qs.metadata['uuid'] = attr_name
                         qs.metadata['path'] = path
                         verbose_name = getattr(attr, '__verbose_name__', qs.metadata['verbose_name'])
                         if verbose_name is None:
                             verbose_name = pretty(attr_name)
+                        qs.verbose_name(verbose_name)
                         template = getattr(attr, '__template__', None)
                         template = 'renderers/{}.html'.format(template) if template else None
                         if self.request:
                             qs = qs.contextualize(self.request).apply_role_lookups(self.request.user)
                         if wrap:
                             if template or (self.metadata['primitive'] and deep > 0):
                                 data = dict(value=serialize(qs), width=width, type='primitive', path=path, template=template)
```

### Comparing `sloth-framework-0.1.7/sloth/db/models/__init__.py` & `sloth-framework-0.1.8/sloth/db/models/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/test/__init__.py` & `sloth-framework-0.1.8/sloth/test/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/test/selenium/__init__.py` & `sloth-framework-0.1.8/sloth/test/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/test/selenium/browser.py` & `sloth-framework-0.1.8/sloth/test/selenium/browser.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/utils/__init__.py` & `sloth-framework-0.1.8/sloth/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/utils/formatter/__init__.py` & `sloth-framework-0.1.8/sloth/utils/formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/utils/http/__init__.py` & `sloth-framework-0.1.8/sloth/utils/http/__init__.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/utils/icons/bootstrap.py` & `sloth-framework-0.1.8/sloth/utils/icons/bootstrap.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/utils/icons/fontawesome.py` & `sloth-framework-0.1.8/sloth/utils/icons/fontawesome.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/utils/icons/materialicons.py` & `sloth-framework-0.1.8/sloth/utils/icons/materialicons.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth/utils/log/sql.py` & `sloth-framework-0.1.8/sloth/utils/log/sql.py`

 * *Files identical despite different names*

### Comparing `sloth-framework-0.1.7/sloth_framework.egg-info/PKG-INFO` & `sloth-framework-0.1.8/sloth_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sloth-framework
-Version: 0.1.7
+Version: 0.1.8
 Summary: Metadata-based web framework for the development of management information systems
 Home-page: http://sloth.aplicativo.click/
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `sloth-framework-0.1.7/sloth_framework.egg-info/SOURCES.txt` & `sloth-framework-0.1.8/sloth_framework.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -136,14 +136,15 @@
 sloth/api/templates/dashboard/links.html
 sloth/api/templates/dashboard/menu.html
 sloth/api/templates/dashboard/messages.html
 sloth/api/templates/dashboard/modal.html
 sloth/api/templates/dashboard/plus.html
 sloth/api/templates/dashboard/report.html
 sloth/api/templates/dashboard/search.html
+sloth/api/templates/dashboard/selector.html
 sloth/api/templates/dashboard/settings.html
 sloth/api/templates/dashboard/shortcuts.html
 sloth/api/templates/dashboard/tasks.html
 sloth/api/templates/dashboard/tools.html
 sloth/api/templates/inputs/picker.html
 sloth/api/templates/inputs/qrcode.html
 sloth/api/templates/inputs/select.html
@@ -191,14 +192,15 @@
 sloth/api/templates/renderers/messages/warning.html
 sloth/api/templates/renderers/photos/photo.html
 sloth/api/templates/renderers/photos/round.html
 sloth/api/templates/renderers/programing/strtable.html
 sloth/api/templates/renderers/programing/terminal.html
 sloth/api/templates/renderers/progress/primary.html
 sloth/api/templates/renderers/progress/success.html
+sloth/api/templates/renderers/statistics/cards.html
 sloth/api/templates/renderers/steps/check.html
 sloth/api/templates/renderers/tags/primary.html
 sloth/api/templates/renderers/tags/tags.html
 sloth/api/templates/renderers/utils/formatted.html
 sloth/api/templates/renderers/utils/progress.html
 sloth/api/templates/renderers/utils/qrcode.html
 sloth/api/templates/renderers/utils/steps.html
```

