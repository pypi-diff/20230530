# Comparing `tmp/irails-1.3.34.tar.gz` & `tmp/irails-1.3.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.3.34.tar", last modified: Mon May 29 12:31:05 2023, max compression
+gzip compressed data, was "irails-1.3.35.tar", last modified: Tue May 30 07:17:59 2023, max compression
```

## Comparing `irails-1.3.34.tar` & `irails-1.3.35.tar`

### file list

```diff
@@ -1,105 +1,106 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.759971 irails-1.3.34/
--rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.34/MANIFEST.in
--rw-rw-rw-   0        0        0     4956 2023-05-29 12:31:05.758976 irails-1.3.34/PKG-INFO
--rw-rw-rw-   0        0        0     4174 2023-05-27 12:12:58.000000 irails-1.3.34/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.608878 irails-1.3.34/irails/
--rw-rw-rw-   0        0        0      307 2023-05-29 12:26:25.000000 irails-1.3.34/irails/__init__.py
--rw-rw-rw-   0        0        0     4887 2023-05-21 14:33:24.000000 irails-1.3.34/irails/_i18n.py
--rw-rw-rw-   0        0        0     4358 2023-05-29 06:44:16.000000 irails-1.3.34/irails/_loader.py
--rw-rw-rw-   0        0        0     5605 2023-05-29 06:19:25.000000 irails-1.3.34/irails/_utils.py
--rw-rw-rw-   0        0        0    15325 2023-05-29 12:21:14.000000 irails-1.3.34/irails/auth.py
--rw-rw-rw-   0        0        0    12705 2023-05-18 07:46:03.000000 irails-1.3.34/irails/base_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.616382 irails-1.3.34/irails/casbin_adapters/
-drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.619374 irails-1.3.34/irails/casbin_adapters/__pycache__/
--rw-rw-rw-   0        0        0     9307 2023-05-29 06:35:41.000000 irails-1.3.34/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc
--rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.34/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
--rw-rw-rw-   0        0        0    10617 2023-05-29 06:35:35.000000 irails-1.3.34/irails/casbin_adapters/sqlalchemy_adapter.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.34/irails/cbv.py
--rw-rw-rw-   0        0        0     6357 2023-05-25 10:46:48.000000 irails-1.3.34/irails/config.py
--rw-rw-rw-   0        0        0    13203 2023-05-26 14:20:32.000000 irails-1.3.34/irails/controller_utils.py
--rw-rw-rw-   0        0        0    26096 2023-05-29 06:20:04.000000 irails-1.3.34/irails/core.py
--rw-rw-rw-   0        0        0    20962 2023-05-29 08:27:47.000000 irails-1.3.34/irails/database.py
--rw-rw-rw-   0        0        0     1592 2023-05-25 14:19:01.000000 irails-1.3.34/irails/log.py
--rw-rw-rw-   0        0        0     8876 2023-05-27 05:49:02.000000 irails-1.3.34/irails/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.34/irails/midware_casbin.py
--rw-rw-rw-   0        0        0     9103 2023-05-16 08:16:43.000000 irails-1.3.34/irails/midware_session.py
--rw-rw-rw-   0        0        0     4219 2023-05-27 10:24:12.000000 irails-1.3.34/irails/mvc_router.py
-drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.632426 irails-1.3.34/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.34/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     7862 2023-05-13 15:04:27.000000 irails-1.3.34/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     6892 2023-05-19 07:21:20.000000 irails-1.3.34/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     7763 2023-05-21 13:57:03.000000 irails-1.3.34/irails/scripts/_i18n.py
--rw-rw-rw-   0        0        0     1332 2023-05-21 08:39:33.000000 irails-1.3.34/irails/scripts/_migrate.py
--rw-rw-rw-   0        0        0     3774 2023-05-14 13:34:33.000000 irails-1.3.34/irails/scripts/_model.py
--rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.34/irails/scripts/_project.py
--rw-rw-rw-   0        0        0     1399 2023-05-26 14:27:13.000000 irails-1.3.34/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.34/irails/scripts/_shell.py
--rw-rw-rw-   0        0        0     5750 2023-05-29 06:31:52.000000 irails-1.3.34/irails/scripts/_test.py
--rw-rw-rw-   0        0        0     2900 2023-05-21 08:16:21.000000 irails-1.3.34/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.578959 irails-1.3.34/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.645392 irails-1.3.34/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.34/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.34/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.34/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.34/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0     1023 2023-05-19 12:27:03.000000 irails-1.3.34/irails/scripts/tpls/app/model.jinja
--rw-rw-rw-   0        0        0      197 2023-05-24 11:06:24.000000 irails-1.3.34/irails/scripts/tpls/app/service.jinja
--rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.34/irails/scripts/tpls/app/test_controller.jinja
--rw-rw-rw-   0        0        0      908 2023-05-24 14:14:47.000000 irails-1.3.34/irails/scripts/tpls/app/test_service.jinja
--rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.34/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.656364 irails-1.3.34/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.34/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.658358 irails-1.3.34/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.34/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.704235 irails-1.3.34/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.34/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0      179 2023-05-13 09:22:15.000000 irails-1.3.34/irails/scripts/tpls/project/configs/authencation.yaml
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.34/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.34/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.34/irails/scripts/tpls/project/configs/casbin-model.conf
-drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.726177 irails-1.3.34/irails/scripts/tpls/project/configs/casbin_templates/
--rw-rw-rw-   0        0        0      204 2023-05-18 07:46:03.000000 irails-1.3.34/irails/scripts/tpls/project/configs/casbin_templates/ALC.conf
--rw-rw-rw-   0        0        0       37 2023-05-18 07:46:03.000000 irails-1.3.34/irails/scripts/tpls/project/configs/casbin_templates/ALC.csv
--rw-rw-rw-   0        0        0      236 2023-05-18 07:46:03.000000 irails-1.3.34/irails/scripts/tpls/project/configs/casbin_templates/RBAC.conf
--rw-rw-rw-   0        0        0      125 2023-05-18 07:46:03.000000 irails-1.3.34/irails/scripts/tpls/project/configs/casbin_templates/RBAC.csv
--rw-rw-rw-   0        0        0      249 2023-05-18 07:46:03.000000 irails-1.3.34/irails/scripts/tpls/project/configs/casbin_templates/RBACR.conf
--rw-rw-rw-   0        0        0      159 2023-05-18 07:46:03.000000 irails-1.3.34/irails/scripts/tpls/project/configs/casbin_templates/RBACR.csv
--rw-rw-rw-   0        0        0      319 2023-05-29 12:26:50.000000 irails-1.3.34/irails/scripts/tpls/project/configs/casbin_templates/RBACT.conf
--rw-rw-rw-   0        0        0      178 2023-05-18 07:46:03.000000 irails-1.3.34/irails/scripts/tpls/project/configs/casbin_templates/RBACT.csv
--rw-rw-rw-   0        0        0      222 2023-05-18 07:46:03.000000 irails-1.3.34/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.conf
--rw-rw-rw-   0        0        0      152 2023-05-18 07:46:03.000000 irails-1.3.34/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.csv
--rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.34/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.34/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.34/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.34/irails/scripts/tpls/project/configs/upload.yaml
-drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.581950 irails-1.3.34/irails/scripts/tpls/project/data/
-drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.730165 irails-1.3.34/irails/scripts/tpls/project/data/alembic/
--rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.34/irails/scripts/tpls/project/data/alembic/README
--rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.34/irails/scripts/tpls/project/data/alembic/env.py
--rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.34/irails/scripts/tpls/project/data/alembic/script.py.mako
--rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.34/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.733492 irails-1.3.34/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.34/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.34/irails/scripts/tpls/project/public/error_500.html
-drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.736498 irails-1.3.34/irails/scripts/tpls/project/public/libs/
-drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.583946 irails-1.3.34/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
-drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.744758 irails-1.3.34/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
--rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.34/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
-drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.750492 irails-1.3.34/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
--rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.34/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
--rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.34/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
--rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.34/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
-drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.584942 irails-1.3.34/irails/scripts/tpls/project/public/vue@3.2.36/
-drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.753627 irails-1.3.34/irails/scripts/tpls/project/public/vue@3.2.36/dist/
--rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.34/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
--rw-rw-rw-   0        0        0     1731 2023-05-29 05:12:03.000000 irails-1.3.34/irails/unit_test.py
--rw-rw-rw-   0        0        0     3034 2023-05-16 08:15:25.000000 irails-1.3.34/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-05-29 12:31:05.615382 irails-1.3.34/irails.egg-info/
--rw-rw-rw-   0        0        0     4956 2023-05-29 12:31:05.000000 irails-1.3.34/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3185 2023-05-29 12:31:05.000000 irails-1.3.34/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 12:31:05.000000 irails-1.3.34/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-29 12:31:05.000000 irails-1.3.34/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      367 2023-05-29 12:31:05.000000 irails-1.3.34/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-29 12:31:05.000000 irails-1.3.34/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 12:31:05.759971 irails-1.3.34/setup.cfg
--rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.34/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 07:17:59.204176 irails-1.3.35/
+-rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.35/MANIFEST.in
+-rw-rw-rw-   0        0        0     4956 2023-05-30 07:17:59.203176 irails-1.3.35/PKG-INFO
+-rw-rw-rw-   0        0        0     4174 2023-05-27 12:12:58.000000 irails-1.3.35/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 07:17:59.096302 irails-1.3.35/irails/
+-rw-rw-rw-   0        0        0      307 2023-05-30 07:17:04.000000 irails-1.3.35/irails/__init__.py
+-rw-rw-rw-   0        0        0     4887 2023-05-21 14:33:24.000000 irails-1.3.35/irails/_i18n.py
+-rw-rw-rw-   0        0        0     4358 2023-05-29 06:44:16.000000 irails-1.3.35/irails/_loader.py
+-rw-rw-rw-   0        0        0     5605 2023-05-29 06:19:25.000000 irails-1.3.35/irails/_utils.py
+-rw-rw-rw-   0        0        0    15325 2023-05-29 12:21:14.000000 irails-1.3.35/irails/auth.py
+-rw-rw-rw-   0        0        0    13497 2023-05-30 07:16:08.000000 irails-1.3.35/irails/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-30 07:17:59.105926 irails-1.3.35/irails/casbin_adapters/
+drwxrwxrwx   0        0        0        0 2023-05-30 07:17:59.109916 irails-1.3.35/irails/casbin_adapters/__pycache__/
+-rw-rw-rw-   0        0        0     9307 2023-05-29 06:35:41.000000 irails-1.3.35/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc
+-rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.35/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10617 2023-05-29 06:35:35.000000 irails-1.3.35/irails/casbin_adapters/sqlalchemy_adapter.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.35/irails/cbv.py
+-rw-rw-rw-   0        0        0     6357 2023-05-25 10:46:48.000000 irails-1.3.35/irails/config.py
+-rw-rw-rw-   0        0        0    13203 2023-05-26 14:20:32.000000 irails-1.3.35/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    27136 2023-05-30 06:40:15.000000 irails-1.3.35/irails/core.py
+-rw-rw-rw-   0        0        0    20962 2023-05-29 08:27:47.000000 irails-1.3.35/irails/database.py
+-rw-rw-rw-   0        0        0     1592 2023-05-25 14:19:01.000000 irails-1.3.35/irails/log.py
+-rw-rw-rw-   0        0        0     8876 2023-05-27 05:49:02.000000 irails-1.3.35/irails/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.35/irails/midware_casbin.py
+-rw-rw-rw-   0        0        0     9103 2023-05-16 08:16:43.000000 irails-1.3.35/irails/midware_session.py
+-rw-rw-rw-   0        0        0     4219 2023-05-27 10:24:12.000000 irails-1.3.35/irails/mvc_router.py
+drwxrwxrwx   0        0        0        0 2023-05-30 07:17:59.121342 irails-1.3.35/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.35/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7862 2023-05-13 15:04:27.000000 irails-1.3.35/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     6892 2023-05-19 07:21:20.000000 irails-1.3.35/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     7763 2023-05-21 13:57:03.000000 irails-1.3.35/irails/scripts/_i18n.py
+-rw-rw-rw-   0        0        0     1332 2023-05-21 08:39:33.000000 irails-1.3.35/irails/scripts/_migrate.py
+-rw-rw-rw-   0        0        0     3774 2023-05-14 13:34:33.000000 irails-1.3.35/irails/scripts/_model.py
+-rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.35/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0     1399 2023-05-26 14:27:13.000000 irails-1.3.35/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.35/irails/scripts/_shell.py
+-rw-rw-rw-   0        0        0     5750 2023-05-29 06:31:52.000000 irails-1.3.35/irails/scripts/_test.py
+-rw-rw-rw-   0        0        0     2900 2023-05-21 08:16:21.000000 irails-1.3.35/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-05-30 07:17:59.059855 irails-1.3.35/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-05-30 07:17:59.137301 irails-1.3.35/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.35/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.35/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.35/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.35/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0     1023 2023-05-19 12:27:03.000000 irails-1.3.35/irails/scripts/tpls/app/model.jinja
+-rw-rw-rw-   0        0        0      197 2023-05-24 11:06:24.000000 irails-1.3.35/irails/scripts/tpls/app/service.jinja
+-rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.35/irails/scripts/tpls/app/test_controller.jinja
+-rw-rw-rw-   0        0        0      908 2023-05-24 14:14:47.000000 irails-1.3.35/irails/scripts/tpls/app/test_service.jinja
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.35/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-05-30 07:17:59.140292 irails-1.3.35/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.35/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-30 07:17:59.142287 irails-1.3.35/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.35/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 07:17:59.155252 irails-1.3.35/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.35/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0      323 2023-05-30 07:17:46.000000 irails-1.3.35/irails/scripts/tpls/project/configs/authencation.yaml
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.35/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.35/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.35/irails/scripts/tpls/project/configs/casbin-model.conf
+drwxrwxrwx   0        0        0        0 2023-05-30 07:17:59.169215 irails-1.3.35/irails/scripts/tpls/project/configs/casbin_templates/
+-rw-rw-rw-   0        0        0      204 2023-05-18 07:46:03.000000 irails-1.3.35/irails/scripts/tpls/project/configs/casbin_templates/ALC.conf
+-rw-rw-rw-   0        0        0       37 2023-05-18 07:46:03.000000 irails-1.3.35/irails/scripts/tpls/project/configs/casbin_templates/ALC.csv
+-rw-rw-rw-   0        0        0      236 2023-05-18 07:46:03.000000 irails-1.3.35/irails/scripts/tpls/project/configs/casbin_templates/RBAC.conf
+-rw-rw-rw-   0        0        0      125 2023-05-18 07:46:03.000000 irails-1.3.35/irails/scripts/tpls/project/configs/casbin_templates/RBAC.csv
+-rw-rw-rw-   0        0        0      249 2023-05-18 07:46:03.000000 irails-1.3.35/irails/scripts/tpls/project/configs/casbin_templates/RBACR.conf
+-rw-rw-rw-   0        0        0      159 2023-05-18 07:46:03.000000 irails-1.3.35/irails/scripts/tpls/project/configs/casbin_templates/RBACR.csv
+-rw-rw-rw-   0        0        0      319 2023-05-29 12:26:50.000000 irails-1.3.35/irails/scripts/tpls/project/configs/casbin_templates/RBACT.conf
+-rw-rw-rw-   0        0        0      178 2023-05-18 07:46:03.000000 irails-1.3.35/irails/scripts/tpls/project/configs/casbin_templates/RBACT.csv
+-rw-rw-rw-   0        0        0      222 2023-05-18 07:46:03.000000 irails-1.3.35/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.conf
+-rw-rw-rw-   0        0        0      152 2023-05-18 07:46:03.000000 irails-1.3.35/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.csv
+-rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.35/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.35/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.35/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.35/irails/scripts/tpls/project/configs/upload.yaml
+drwxrwxrwx   0        0        0        0 2023-05-30 07:17:59.063844 irails-1.3.35/irails/scripts/tpls/project/data/
+drwxrwxrwx   0        0        0        0 2023-05-30 07:17:59.173203 irails-1.3.35/irails/scripts/tpls/project/data/alembic/
+-rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.35/irails/scripts/tpls/project/data/alembic/README
+-rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.35/irails/scripts/tpls/project/data/alembic/env.py
+-rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.35/irails/scripts/tpls/project/data/alembic/script.py.mako
+-rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.35/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-05-30 07:17:59.178192 irails-1.3.35/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.35/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.35/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-05-30 07:17:59.182180 irails-1.3.35/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-05-30 07:17:59.067834 irails-1.3.35/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-05-30 07:17:59.189732 irails-1.3.35/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.35/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-05-30 07:17:59.196719 irails-1.3.35/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.35/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.35/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.35/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-05-30 07:17:59.069828 irails-1.3.35/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-05-30 07:17:59.199786 irails-1.3.35/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.35/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0     1048 2023-05-30 07:13:21.000000 irails-1.3.35/irails/scripts/tpls/project/public/vue_home.html
+-rw-rw-rw-   0        0        0     1731 2023-05-29 05:12:03.000000 irails-1.3.35/irails/unit_test.py
+-rw-rw-rw-   0        0        0     3053 2023-05-30 07:10:08.000000 irails-1.3.35/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-05-30 07:17:59.103931 irails-1.3.35/irails.egg-info/
+-rw-rw-rw-   0        0        0     4956 2023-05-30 07:17:58.000000 irails-1.3.35/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3234 2023-05-30 07:17:58.000000 irails-1.3.35/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 07:17:58.000000 irails-1.3.35/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-30 07:17:58.000000 irails-1.3.35/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      367 2023-05-30 07:17:58.000000 irails-1.3.35/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-30 07:17:58.000000 irails-1.3.35/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 07:17:59.204176 irails-1.3.35/setup.cfg
+-rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.35/setup.py
```

### Comparing `irails-1.3.34/PKG-INFO` & `irails-1.3.35/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.34
+Version: 1.3.35
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.3.34/README.md` & `irails-1.3.35/README.md`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/_i18n.py` & `irails-1.3.35/irails/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/_loader.py` & `irails-1.3.35/irails/_loader.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/_utils.py` & `irails-1.3.35/irails/_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/auth.py` & `irails-1.3.35/irails/auth.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/base_controller.py` & `irails-1.3.35/irails/base_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,16 +144,33 @@
     def _user_logout(self,msg="You are successed logout!",redirect='/'):
         """return Response for logout to root('/')"""
         pass
 
     def _verity_error(self,msg="User authentication failed!"):
         """return Response for show Verity failed infomation"""
         pass
-     
-    # @property
+    def vue_sfc_app(self,path="./public/vue_home.html", main_vue="main.vue"):
+        """
+        return a view based vue3 used ElementPlus and use vue3_sfc_loader
+        """
+        from jinja2 import Template
+        from .view import get_view_configure
+        view_config = get_view_configure()
+        context = {'main':main_vue}
+        if not os.path.isabs(path):
+            path = os.path.abspath(os.path.join(ROOT_PATH,path))
+        if os.path.exists(path):
+            with open(path,'r',encoding='utf-8') as f:
+                content = f.read()
+            dest_content = content 
+            template = Template(content,**view_config)
+            dest_content = template.render(context)
+            return HTMLResponse(content=dest_content)
+        raise FileNotFoundError(path)
+ 
     def view(self,content:str="",view_path:str="", format:str="html", context: dict=None,local2context:bool=True,**kwargs): 
         """
         return a Response by template file
         if :view_path is empty ,it's will look for current method in the view directory(offen is app dir views\controller's name)
         """
         if not context:
             context={}
```

### Comparing `irails-1.3.34/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc` & `irails-1.3.35/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc` & `irails-1.3.35/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/casbin_adapters/sqlalchemy_adapter.py` & `irails-1.3.35/irails/casbin_adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/cbv.py` & `irails-1.3.35/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/config.py` & `irails-1.3.35/irails/config.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/controller_utils.py` & `irails-1.3.35/irails/controller_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/core.py` & `irails-1.3.35/irails/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,14 +114,41 @@
      
     @property 
     def data_engine(self)->database.Engine:
         return self._data_engine
     @data_engine.setter
     def data_engine(self,value):
         self._data_engine = value
+
+    def app_list(self,group_by_controller=False)->List:
+        import copy
+        apps = []
+        for app_name in self.apps:
+            manifest=copy.copy(self.apps[app_name]['manifest'])
+            route_map = copy.copy(self.apps[app_name]['route_map'])
+            for item in route_map:
+                if 'endpoint' in route_map[item]:
+                    del route_map[item]['endpoint']
+            if group_by_controller:
+                funcs={}
+            else:
+                funcs = []
+            for item in route_map:
+                _item = route_map[item]
+                _item.update({'function':item})
+                if group_by_controller:
+                    ctrl_name = item.split(".")[0]
+                    funcs[ctrl_name] = _item
+                    pass
+                else:
+                    funcs.append(_item)
+            manifest.update({'app_name':app_name,'routes':funcs})
+             
+            apps.append(manifest)
+        return apps
     def __repr__(self):
         return f'<IRails:{self.title}>'
     def route(self, *args,**kwargs):
         '''disabled'''
         raise RuntimeError(_("Please use api.http,MVC app not allow to use this direct!"))
         #return super().route(path, methods, name, include_in_schema)
     def post(self, *args,**kwargs):
@@ -153,15 +180,15 @@
         raise RuntimeError(_("Please use api.patch,MVC app not allow to use this direct!"))
         #return super().patch(path, response_model=response_model, status_code=status_code, tags=tags, dependencies=dependencies, summary=summary, description=description, response_description=response_description, responses=responses, deprecated=deprecated, operation_id=operation_id, response_model_include=response_model_include, response_model_exclude=response_model_exclude, response_model_by_alias=response_model_by_alias, response_model_exclude_unset=response_model_exclude_unset, response_model_exclude_defaults=response_model_exclude_defaults, response_model_exclude_none=response_model_exclude_none, include_in_schema=include_in_schema, response_class=response_class, name=name, callbacks=callbacks, openapi_extra=openapi_extra, generate_unique_id_function=generate_unique_id_function)
     def trace(self, *args,**kwargs):
         '''disabled'''
         raise RuntimeError(_("Please use api.trace,MVC app not allow to use this direct!"))
         #return super().trace(path, response_model=response_model, status_code=status_code, tags=tags, dependencies=dependencies, summary=summary, description=description, response_description=response_description, responses=responses, deprecated=deprecated, operation_id=operation_id, response_model_include=response_model_include, response_model_exclude=response_model_exclude, response_model_by_alias=response_model_by_alias, response_model_exclude_unset=response_model_exclude_unset, response_model_exclude_defaults=response_model_exclude_defaults, response_model_exclude_none=response_model_exclude_none, include_in_schema=include_in_schema, response_class=response_class, name=name, callbacks=callbacks, openapi_extra=openapi_extra, generate_unique_id_function=generate_unique_id_function)
     
-__app = MvcApp( ) 
+__app = MvcApp(docs_url=None,redoc_url=None ) 
 
 __all_controller__ = {}
 
 application = __app
 api.init(application)
```

### Comparing `irails-1.3.34/irails/database.py` & `irails-1.3.35/irails/database.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/log.py` & `irails-1.3.35/irails/log.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/midware.py` & `irails-1.3.35/irails/midware.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/midware_casbin.py` & `irails-1.3.35/irails/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/midware_session.py` & `irails-1.3.35/irails/midware_session.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/mvc_router.py` & `irails-1.3.35/irails/mvc_router.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/scripts/_app.py` & `irails-1.3.35/irails/scripts/_app.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/scripts/_controller.py` & `irails-1.3.35/irails/scripts/_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/scripts/_i18n.py` & `irails-1.3.35/irails/scripts/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/scripts/_migrate.py` & `irails-1.3.35/irails/scripts/_migrate.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/scripts/_model.py` & `irails-1.3.35/irails/scripts/_model.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/scripts/_project.py` & `irails-1.3.35/irails/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/scripts/_run.py` & `irails-1.3.35/irails/scripts/_run.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/scripts/_shell.py` & `irails-1.3.35/irails/scripts/_shell.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/scripts/_test.py` & `irails-1.3.35/irails/scripts/_test.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/scripts/main.py` & `irails-1.3.35/irails/scripts/main.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/scripts/tpls/app/home.css.tpl` & `irails-1.3.35/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/scripts/tpls/app/home.tpl` & `irails-1.3.35/irails/scripts/tpls/app/home.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/scripts/tpls/app/model.jinja` & `irails-1.3.35/irails/scripts/tpls/app/model.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/scripts/tpls/app/test_service.jinja` & `irails-1.3.35/irails/scripts/tpls/app/test_service.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.3.35/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.3.35/irails/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/scripts/tpls/project/configs/general.yaml` & `irails-1.3.35/irails/scripts/tpls/project/configs/general.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/scripts/tpls/project/data/alembic/env.py` & `irails-1.3.35/irails/scripts/tpls/project/data/alembic/env.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/scripts/tpls/project/public/error_404.html` & `irails-1.3.35/irails/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/scripts/tpls/project/public/error_500.html` & `irails-1.3.35/irails/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js` & `irails-1.3.35/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css` & `irails-1.3.35/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js` & `irails-1.3.35/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js` & `irails-1.3.35/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js` & `irails-1.3.35/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/unit_test.py` & `irails-1.3.35/irails/unit_test.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.34/irails/view.py` & `irails-1.3.35/irails/view.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,25 +8,26 @@
 from .config import ROOT_PATH, config
 from .log import _log
 from ._i18n import _
 env_configs = {}
 static_format = []
 
 
-def __get_view_configure():
+def get_view_configure():
     global static_format, env_configs
     # {'variable_start_string':'${','variable_end_string':'}'}
     env_options = config.get("view")
     if env_options:
         static_format = env_options.get('static_format', [])
         env_options = env_options.get("jinja2")
         env_configs = env_options.config
 
+    return env_configs
 
-__get_view_configure()
+get_view_configure()
 
 
 class _View(object):
     def __init__(self, request, response=None, tmpl_path: str = f"{os.path.abspath('')}/app/views"):
         self._views_directory = tmpl_path
 
         self._templates = Jinja2Templates(
```

### Comparing `irails-1.3.34/irails.egg-info/PKG-INFO` & `irails-1.3.35/irails.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.34
+Version: 1.3.35
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.3.34/irails.egg-info/SOURCES.txt` & `irails-1.3.35/irails.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -72,12 +72,13 @@
 irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.conf
 irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.csv
 irails/scripts/tpls/project/data/alembic/README
 irails/scripts/tpls/project/data/alembic/env.py
 irails/scripts/tpls/project/data/alembic/script.py.mako
 irails/scripts/tpls/project/public/error_404.html
 irails/scripts/tpls/project/public/error_500.html
+irails/scripts/tpls/project/public/vue_home.html
 irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
 irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
 irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
 irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
 irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
```

### Comparing `irails-1.3.34/setup.py` & `irails-1.3.35/setup.py`

 * *Files identical despite different names*

