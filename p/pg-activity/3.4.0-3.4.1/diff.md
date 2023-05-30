# Comparing `tmp/pg-activity-3.4.0.tar.gz` & `tmp/pg-activity-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pg-activity-3.4.0.tar", last modified: Mon May 15 09:04:31 2023, max compression
+gzip compressed data, was "pg-activity-3.4.1.tar", last modified: Tue May 30 07:20:56 2023, max compression
```

## Comparing `pg-activity-3.4.0.tar` & `pg-activity-3.4.1.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2023-05-15 09:04:31.022173 pg-activity-3.4.0/
--rw-r--r--   0 denis     (1000) denis     (1000)       61 2023-02-01 11:56:00.000000 pg-activity-3.4.0/.codespellrc
--rw-r--r--   0 denis     (1000) denis     (1000)       45 2021-02-01 14:14:21.000000 pg-activity-3.4.0/.coveragerc
--rw-r--r--   0 denis     (1000) denis     (1000)      106 2021-02-01 14:14:21.000000 pg-activity-3.4.0/.editorconfig
--rw-r--r--   0 denis     (1000) denis     (1000)      301 2022-11-28 15:05:59.000000 pg-activity-3.4.0/.flake8
--rw-r--r--   0 denis     (1000) denis     (1000)     1346 2021-07-19 12:31:38.000000 pg-activity-3.4.0/AUTHORS.md
--rw-r--r--   0 denis     (1000) denis     (1000)    13650 2023-05-15 08:58:50.000000 pg-activity-3.4.0/CHANGELOG.md
--rw-r--r--   0 denis     (1000) denis     (1000)      942 2021-02-01 14:14:21.000000 pg-activity-3.4.0/LICENSE.txt
--rw-r--r--   0 denis     (1000) denis     (1000)      355 2023-04-11 07:41:54.000000 pg-activity-3.4.0/MANIFEST.in
--rw-r--r--   0 denis     (1000) denis     (1000)    12315 2023-05-15 09:04:31.022173 pg-activity-3.4.0/PKG-INFO
--rw-r--r--   0 denis     (1000) denis     (1000)    11059 2023-05-15 08:24:59.000000 pg-activity-3.4.0/README.md
--rw-r--r--   0 denis     (1000) denis     (1000)     1830 2023-01-24 12:51:39.000000 pg-activity-3.4.0/RELEASE.md
-drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2023-05-15 09:04:30.978172 pg-activity-3.4.0/docs/
-drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2023-05-15 09:04:30.990172 pg-activity-3.4.0/docs/imgs/
--rw-r--r--   0 denis     (1000) denis     (1000)    28659 2020-05-27 08:10:17.000000 pg-activity-3.4.0/docs/imgs/logo-horizontal.png
--rw-r--r--   0 denis     (1000) denis     (1000)     5296 2020-05-27 08:10:17.000000 pg-activity-3.4.0/docs/imgs/logo-horizontal.svg
--rw-r--r--   0 denis     (1000) denis     (1000)     4546 2020-05-27 08:10:17.000000 pg-activity-3.4.0/docs/imgs/logo.svg
--rw-r--r--   0 denis     (1000) denis     (1000)   337072 2022-09-21 07:26:09.000000 pg-activity-3.4.0/docs/imgs/screenshot.png
-drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2023-05-15 09:04:30.990172 pg-activity-3.4.0/docs/man/
--rwxr-xr-x   0 denis     (1000) denis     (1000)      194 2023-05-15 08:58:50.000000 pg-activity-3.4.0/docs/man/build-man.sh
--rw-r--r--   0 denis     (1000) denis     (1000)    27465 2023-05-15 08:58:50.000000 pg-activity-3.4.0/docs/man/pg_activity.1
--rw-r--r--   0 denis     (1000) denis     (1000)    13648 2023-03-10 09:40:53.000000 pg-activity-3.4.0/docs/man/pg_activity.pod
--rw-r--r--   0 denis     (1000) denis     (1000)      244 2023-03-16 14:51:38.000000 pg-activity-3.4.0/mypy.ini
-drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2023-05-15 09:04:30.994172 pg-activity-3.4.0/pg_activity.egg-info/
--rw-r--r--   0 denis     (1000) denis     (1000)    12315 2023-05-15 09:04:30.000000 pg-activity-3.4.0/pg_activity.egg-info/PKG-INFO
--rw-r--r--   0 denis     (1000) denis     (1000)     2789 2023-05-15 09:04:30.000000 pg-activity-3.4.0/pg_activity.egg-info/SOURCES.txt
--rw-r--r--   0 denis     (1000) denis     (1000)        1 2023-05-15 09:04:30.000000 pg-activity-3.4.0/pg_activity.egg-info/dependency_links.txt
--rw-r--r--   0 denis     (1000) denis     (1000)       52 2023-05-15 09:04:30.000000 pg-activity-3.4.0/pg_activity.egg-info/entry_points.txt
--rw-r--r--   0 denis     (1000) denis     (1000)      345 2023-05-15 09:04:30.000000 pg-activity-3.4.0/pg_activity.egg-info/requires.txt
--rw-r--r--   0 denis     (1000) denis     (1000)       35 2023-05-15 09:04:30.000000 pg-activity-3.4.0/pg_activity.egg-info/top_level.txt
-drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2023-05-15 09:04:31.002172 pg-activity-3.4.0/pgactivity/
--rw-r--r--   0 denis     (1000) denis     (1000)       22 2023-05-15 08:58:50.000000 pg-activity-3.4.0/pgactivity/__init__.py
--rw-r--r--   0 denis     (1000) denis     (1000)       61 2021-07-19 12:31:38.000000 pg-activity-3.4.0/pgactivity/__main__.py
--rw-r--r--   0 denis     (1000) denis     (1000)    11874 2023-04-24 08:53:46.000000 pg-activity-3.4.0/pgactivity/activities.py
--rwxr-xr-x   0 denis     (1000) denis     (1000)    11203 2023-05-15 08:24:59.000000 pg-activity-3.4.0/pgactivity/cli.py
--rw-r--r--   0 denis     (1000) denis     (1000)     3081 2023-03-22 07:46:12.000000 pg-activity-3.4.0/pgactivity/colors.py
--rw-r--r--   0 denis     (1000) denis     (1000)      798 2023-04-20 08:45:15.000000 pg-activity-3.4.0/pgactivity/compat.py
--rw-r--r--   0 denis     (1000) denis     (1000)     8282 2023-05-15 08:24:59.000000 pg-activity-3.4.0/pgactivity/config.py
--rw-r--r--   0 denis     (1000) denis     (1000)    20141 2023-03-28 15:13:08.000000 pg-activity-3.4.0/pgactivity/data.py
--rw-r--r--   0 denis     (1000) denis     (1000)     3861 2023-04-24 10:05:47.000000 pg-activity-3.4.0/pgactivity/handlers.py
--rw-r--r--   0 denis     (1000) denis     (1000)     3782 2022-04-28 08:55:55.000000 pg-activity-3.4.0/pgactivity/keys.py
--rw-r--r--   0 denis     (1000) denis     (1000)     9933 2023-03-30 07:02:41.000000 pg-activity-3.4.0/pgactivity/pg.py
-drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2023-05-15 09:04:31.014172 pg-activity-3.4.0/pgactivity/queries/
--rw-r--r--   0 denis     (1000) denis     (1000)      217 2021-03-08 15:28:57.000000 pg-activity-3.4.0/pgactivity/queries/__init__.py
--rw-r--r--   0 denis     (1000) denis     (1000)       37 2021-07-19 12:31:38.000000 pg-activity-3.4.0/pgactivity/queries/disable_log_min_duration_sample.sql
--rw-r--r--   0 denis     (1000) denis     (1000)       40 2021-12-16 08:04:47.000000 pg-activity-3.4.0/pgactivity/queries/disable_log_min_duration_statement.sql
--rw-r--r--   0 denis     (1000) denis     (1000)      146 2021-12-16 08:04:48.000000 pg-activity-3.4.0/pgactivity/queries/do_pg_cancel_backend.sql
--rw-r--r--   0 denis     (1000) denis     (1000)      128 2021-12-16 08:04:49.000000 pg-activity-3.4.0/pgactivity/queries/do_pg_terminate_backend.sql
--rw-r--r--   0 denis     (1000) denis     (1000)     4716 2023-04-03 06:51:35.000000 pg-activity-3.4.0/pgactivity/queries/get_blocking_oldest.sql
--rw-r--r--   0 denis     (1000) denis     (1000)     4527 2023-04-03 06:51:35.000000 pg-activity-3.4.0/pgactivity/queries/get_blocking_post_090200.sql
--rw-r--r--   0 denis     (1000) denis     (1000)     4455 2023-04-03 06:51:35.000000 pg-activity-3.4.0/pgactivity/queries/get_blocking_post_090600.sql
--rw-r--r--   0 denis     (1000) denis     (1000)       52 2022-09-07 07:03:25.000000 pg-activity-3.4.0/pgactivity/queries/get_data_directory.sql
--rw-r--r--   0 denis     (1000) denis     (1000)     1317 2023-04-03 06:51:35.000000 pg-activity-3.4.0/pgactivity/queries/get_pg_activity_oldest.sql
--rw-r--r--   0 denis     (1000) denis     (1000)     1063 2023-04-03 06:51:35.000000 pg-activity-3.4.0/pgactivity/queries/get_pg_activity_post_090200.sql
--rw-r--r--   0 denis     (1000) denis     (1000)     1086 2023-04-03 06:51:35.000000 pg-activity-3.4.0/pgactivity/queries/get_pg_activity_post_090600.sql
--rw-r--r--   0 denis     (1000) denis     (1000)     1130 2023-04-03 06:51:35.000000 pg-activity-3.4.0/pgactivity/queries/get_pg_activity_post_100000.sql
--rw-r--r--   0 denis     (1000) denis     (1000)     1045 2023-04-03 06:51:35.000000 pg-activity-3.4.0/pgactivity/queries/get_pg_activity_post_110000.sql
--rw-r--r--   0 denis     (1000) denis     (1000)     1040 2023-04-03 06:51:35.000000 pg-activity-3.4.0/pgactivity/queries/get_pg_activity_post_130000.sql
--rw-r--r--   0 denis     (1000) denis     (1000)      131 2021-12-16 08:05:04.000000 pg-activity-3.4.0/pgactivity/queries/get_pga_inet_addresses.sql
--rw-r--r--   0 denis     (1000) denis     (1000)      144 2022-09-05 11:40:07.000000 pg-activity-3.4.0/pgactivity/queries/get_replication_slots_post_140000.sql
--rw-r--r--   0 denis     (1000) denis     (1000)     2508 2023-02-01 11:56:00.000000 pg-activity-3.4.0/pgactivity/queries/get_server_info_oldest.sql
--rw-r--r--   0 denis     (1000) denis     (1000)     2571 2023-02-01 11:56:00.000000 pg-activity-3.4.0/pgactivity/queries/get_server_info_post_090100.sql
--rw-r--r--   0 denis     (1000) denis     (1000)     2516 2023-02-01 11:56:00.000000 pg-activity-3.4.0/pgactivity/queries/get_server_info_post_090200.sql
--rw-r--r--   0 denis     (1000) denis     (1000)     2619 2023-02-01 11:56:00.000000 pg-activity-3.4.0/pgactivity/queries/get_server_info_post_090400.sql
--rw-r--r--   0 denis     (1000) denis     (1000)     2626 2023-02-01 11:56:00.000000 pg-activity-3.4.0/pgactivity/queries/get_server_info_post_090600.sql
--rw-r--r--   0 denis     (1000) denis     (1000)     2980 2023-02-01 11:56:00.000000 pg-activity-3.4.0/pgactivity/queries/get_server_info_post_100000.sql
--rw-r--r--   0 denis     (1000) denis     (1000)     3091 2023-02-01 11:56:00.000000 pg-activity-3.4.0/pgactivity/queries/get_server_info_post_110000.sql
--rw-r--r--   0 denis     (1000) denis     (1000)     1331 2022-09-05 11:40:07.000000 pg-activity-3.4.0/pgactivity/queries/get_temporary_files_oldest.sql
--rw-r--r--   0 denis     (1000) denis     (1000)     1373 2022-09-05 11:40:07.000000 pg-activity-3.4.0/pgactivity/queries/get_temporary_files_post_090100.sql
--rw-r--r--   0 denis     (1000) denis     (1000)     1436 2022-09-05 11:40:07.000000 pg-activity-3.4.0/pgactivity/queries/get_temporary_files_post_090500.sql
--rw-r--r--   0 denis     (1000) denis     (1000)      245 2022-09-05 11:40:07.000000 pg-activity-3.4.0/pgactivity/queries/get_temporary_files_post_120000.sql
--rw-r--r--   0 denis     (1000) denis     (1000)       60 2021-12-16 08:05:06.000000 pg-activity-3.4.0/pgactivity/queries/get_version.sql
--rw-r--r--   0 denis     (1000) denis     (1000)     1429 2023-04-03 06:51:35.000000 pg-activity-3.4.0/pgactivity/queries/get_waiting_oldest.sql
--rw-r--r--   0 denis     (1000) denis     (1000)     1205 2023-04-03 06:51:35.000000 pg-activity-3.4.0/pgactivity/queries/get_waiting_post_090200.sql
--rw-r--r--   0 denis     (1000) denis     (1000)      130 2022-09-05 11:40:07.000000 pg-activity-3.4.0/pgactivity/queries/get_wal_receivers_post_090600.sql
--rw-r--r--   0 denis     (1000) denis     (1000)      124 2022-09-05 11:40:07.000000 pg-activity-3.4.0/pgactivity/queries/get_wal_senders_post_090100.sql
--rw-r--r--   0 denis     (1000) denis     (1000)       25 2022-09-05 11:40:07.000000 pg-activity-3.4.0/pgactivity/queries/reset_statement_timeout.sql
--rw-r--r--   0 denis     (1000) denis     (1000)    30898 2023-05-15 08:24:59.000000 pg-activity-3.4.0/pgactivity/types.py
--rw-r--r--   0 denis     (1000) denis     (1000)    11181 2023-05-15 08:24:59.000000 pg-activity-3.4.0/pgactivity/ui.py
--rw-r--r--   0 denis     (1000) denis     (1000)     9806 2023-03-22 07:46:12.000000 pg-activity-3.4.0/pgactivity/utils.py
--rw-r--r--   0 denis     (1000) denis     (1000)    19014 2023-04-24 10:05:47.000000 pg-activity-3.4.0/pgactivity/views.py
--rw-r--r--   0 denis     (1000) denis     (1000)      919 2022-01-11 13:53:15.000000 pg-activity-3.4.0/pgactivity/widgets.py
--rw-r--r--   0 denis     (1000) denis     (1000)     2259 2023-04-24 11:18:21.000000 pg-activity-3.4.0/pyproject.toml
--rw-r--r--   0 denis     (1000) denis     (1000)       37 2021-03-18 15:43:32.000000 pg-activity-3.4.0/pytest.ini
--rw-r--r--   0 denis     (1000) denis     (1000)       38 2023-05-15 09:04:31.022173 pg-activity-3.4.0/setup.cfg
--rw-r--r--   0 denis     (1000) denis     (1000)       38 2023-04-20 09:37:05.000000 pg-activity-3.4.0/setup.py
-drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2023-05-15 09:04:31.018172 pg-activity-3.4.0/tests/
--rw-r--r--   0 denis     (1000) denis     (1000)     3103 2023-03-22 07:46:12.000000 pg-activity-3.4.0/tests/conftest.py
-drwxr-xr-x   0 denis     (1000) denis     (1000)        0 2023-05-15 09:04:31.018172 pg-activity-3.4.0/tests/data/
--rw-r--r--   0 denis     (1000) denis     (1000)    62239 2023-04-03 06:51:35.000000 pg-activity-3.4.0/tests/data/local-processes-input.json
--rw-r--r--   0 denis     (1000) denis     (1000)     4081 2023-03-22 07:46:12.000000 pg-activity-3.4.0/tests/test_activities.py
--rw-r--r--   0 denis     (1000) denis     (1000)     1712 2023-05-15 08:24:59.000000 pg-activity-3.4.0/tests/test_config.py
--rw-r--r--   0 denis     (1000) denis     (1000)     6413 2023-03-22 07:46:12.000000 pg-activity-3.4.0/tests/test_data.py
--rw-r--r--   0 denis     (1000) denis     (1000)     3108 2023-04-03 06:51:35.000000 pg-activity-3.4.0/tests/test_scroll.txt
--rw-r--r--   0 denis     (1000) denis     (1000)      165 2023-04-24 10:05:47.000000 pg-activity-3.4.0/tests/test_types.py
--rw-r--r--   0 denis     (1000) denis     (1000)    40923 2023-05-15 08:24:59.000000 pg-activity-3.4.0/tests/test_ui.txt
--rw-r--r--   0 denis     (1000) denis     (1000)     1817 2023-04-24 10:05:47.000000 pg-activity-3.4.0/tests/test_views.py
--rw-r--r--   0 denis     (1000) denis     (1000)    24193 2023-04-24 10:05:47.000000 pg-activity-3.4.0/tests/test_views.txt
--rw-r--r--   0 denis     (1000) denis     (1000)      796 2021-03-08 15:28:57.000000 pg-activity-3.4.0/tests/test_widgets.txt
--rw-r--r--   0 denis     (1000) denis     (1000)      717 2023-04-24 11:18:21.000000 pg-activity-3.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:20:56.130953 pg-activity-3.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-30 07:20:42.000000 pg-activity-3.4.1/.codespellrc
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-30 07:20:42.000000 pg-activity-3.4.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-30 07:20:42.000000 pg-activity-3.4.1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-30 07:20:42.000000 pg-activity-3.4.1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-30 07:20:42.000000 pg-activity-3.4.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13753 2023-05-30 07:20:42.000000 pg-activity-3.4.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-30 07:20:42.000000 pg-activity-3.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-30 07:20:42.000000 pg-activity-3.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12315 2023-05-30 07:20:56.130953 pg-activity-3.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11059 2023-05-30 07:20:42.000000 pg-activity-3.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-30 07:20:42.000000 pg-activity-3.4.1/RELEASE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:20:56.102953 pg-activity-3.4.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:20:56.110953 pg-activity-3.4.1/docs/imgs/
+-rw-r--r--   0 runner    (1001) docker     (123)    28659 2023-05-30 07:20:42.000000 pg-activity-3.4.1/docs/imgs/logo-horizontal.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-05-30 07:20:42.000000 pg-activity-3.4.1/docs/imgs/logo-horizontal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-30 07:20:42.000000 pg-activity-3.4.1/docs/imgs/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   337072 2023-05-30 07:20:42.000000 pg-activity-3.4.1/docs/imgs/screenshot.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:20:56.114953 pg-activity-3.4.1/docs/man/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      194 2023-05-30 07:20:42.000000 pg-activity-3.4.1/docs/man/build-man.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    27465 2023-05-30 07:20:42.000000 pg-activity-3.4.1/docs/man/pg_activity.1
+-rw-r--r--   0 runner    (1001) docker     (123)    13648 2023-05-30 07:20:42.000000 pg-activity-3.4.1/docs/man/pg_activity.pod
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-30 07:20:42.000000 pg-activity-3.4.1/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:20:56.114953 pg-activity-3.4.1/pg_activity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12315 2023-05-30 07:20:56.000000 pg-activity-3.4.1/pg_activity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-30 07:20:56.000000 pg-activity-3.4.1/pg_activity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 07:20:56.000000 pg-activity-3.4.1/pg_activity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-30 07:20:56.000000 pg-activity-3.4.1/pg_activity.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-30 07:20:56.000000 pg-activity-3.4.1/pg_activity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-30 07:20:56.000000 pg-activity-3.4.1/pg_activity.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:20:56.118953 pg-activity-3.4.1/pgactivity/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/activities.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11203 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20141 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/pg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:20:56.130953 pg-activity-3.4.1/pgactivity/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/disable_log_min_duration_sample.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/disable_log_min_duration_statement.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/do_pg_cancel_backend.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/do_pg_terminate_backend.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_blocking_oldest.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_blocking_post_090200.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_blocking_post_090600.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_data_directory.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_pg_activity_oldest.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_pg_activity_post_090200.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_pg_activity_post_090600.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_pg_activity_post_100000.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_pg_activity_post_110000.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_pg_activity_post_130000.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_pga_inet_addresses.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_replication_slots_post_140000.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_server_info_oldest.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_server_info_post_090100.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_server_info_post_090200.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_server_info_post_090400.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_server_info_post_090600.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_server_info_post_100000.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_server_info_post_110000.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1331 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_temporary_files_oldest.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_temporary_files_post_090100.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_temporary_files_post_090500.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_temporary_files_post_120000.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_version.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_waiting_oldest.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_waiting_post_090200.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_wal_receivers_post_090600.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/get_wal_senders_post_090100.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/queries/reset_statement_timeout.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    30898 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9806 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19014 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pgactivity/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-30 07:20:42.000000 pg-activity-3.4.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 07:20:56.130953 pg-activity-3.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 07:20:42.000000 pg-activity-3.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:20:56.130953 pg-activity-3.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-05-30 07:20:42.000000 pg-activity-3.4.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:20:56.130953 pg-activity-3.4.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    62239 2023-05-30 07:20:42.000000 pg-activity-3.4.1/tests/data/local-processes-input.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-30 07:20:42.000000 pg-activity-3.4.1/tests/test_activities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-30 07:20:42.000000 pg-activity-3.4.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-05-30 07:20:42.000000 pg-activity-3.4.1/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-30 07:20:42.000000 pg-activity-3.4.1/tests/test_scroll.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-30 07:20:42.000000 pg-activity-3.4.1/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40923 2023-05-30 07:20:42.000000 pg-activity-3.4.1/tests/test_ui.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-30 07:20:42.000000 pg-activity-3.4.1/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24193 2023-05-30 07:20:42.000000 pg-activity-3.4.1/tests/test_views.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-30 07:20:42.000000 pg-activity-3.4.1/tests/test_widgets.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-30 07:20:42.000000 pg-activity-3.4.1/tox.ini
```

### Comparing `pg-activity-3.4.0/AUTHORS.md` & `pg-activity-3.4.1/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/CHANGELOG.md` & `pg-activity-3.4.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Change log
 
+## pg\_activity 3.4.1 - 2023-05-30
+
+### Fixed
+
+* Add more compatibility for old attr versions (#376).
+
 ## pg\_activity 3.4.0 - 2023-05-15
 
 ### Added
 
 * Improve rendering of the `client` column by possibly abbreviating IP
   addresses.
 * Add support for configuring pg\_activity from a configuration file in INI
```

### Comparing `pg-activity-3.4.0/LICENSE.txt` & `pg-activity-3.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/PKG-INFO` & `pg-activity-3.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pg-activity
-Version: 3.4.0
+Version: 3.4.1
 Summary: Command line tool for PostgreSQL server activity monitoring.
 Author-email: Julien Tachoires <julmon@gmail.com>, Benoit Lobréau <benoit.lobreau@dalibo.com>, Denis Laxalde <denis.laxalde@dalibo.com>, Dalibo <contact@dalibo.com>
 Maintainer-email: Denis Laxalde <denis.laxalde@dalibo.com>, Benoit Lobréau <benoit.lobreau@dalibo.com>
 License: PostgreSQL
 Project-URL: Bug Tracker, https://github.com/dalibo/pg_activity/issues/
 Project-URL: Changelog, https://github.com/dalibo/pg_activity/blob/master/CHANGELOG.md
 Project-URL: Homepage, https://github.com/dalibo/pg_activity
```

### Comparing `pg-activity-3.4.0/README.md` & `pg-activity-3.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/RELEASE.md` & `pg-activity-3.4.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/docs/imgs/logo-horizontal.png` & `pg-activity-3.4.1/docs/imgs/logo-horizontal.png`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/docs/imgs/logo-horizontal.svg` & `pg-activity-3.4.1/docs/imgs/logo-horizontal.svg`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/docs/imgs/logo.svg` & `pg-activity-3.4.1/docs/imgs/logo.svg`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/docs/imgs/screenshot.png` & `pg-activity-3.4.1/docs/imgs/screenshot.png`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/docs/man/pg_activity.1` & `pg-activity-3.4.1/docs/man/pg_activity.1`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 .    ds ae ae
 .    ds Ae AE
 .\}
 .rm #[ #] #H #V #F C
 .\" ========================================================================
 .\"
 .IX Title "PG_ACTIVITY 1"
-.TH PG_ACTIVITY 1 "2023-05-15" "pg_activity 3.4.0" "Command line tool for PostgreSQL server activity monitoring."
+.TH PG_ACTIVITY 1 "2023-05-30" "pg_activity 3.4.1" "Command line tool for PostgreSQL server activity monitoring."
 .\" For nroff, turn off justification.  Always turn off hyphenation; it makes
 .\" way too many mistakes in technical documents.
 .if n .ad l
 .nh
 .SH "NAME"
 pg_activity \- Realtime PostgreSQL database server monitoring tool
 .SH "SYNOPSIS"
```

### Comparing `pg-activity-3.4.0/docs/man/pg_activity.pod` & `pg-activity-3.4.1/docs/man/pg_activity.pod`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/pg_activity.egg-info/PKG-INFO` & `pg-activity-3.4.1/pg_activity.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pg-activity
-Version: 3.4.0
+Version: 3.4.1
 Summary: Command line tool for PostgreSQL server activity monitoring.
 Author-email: Julien Tachoires <julmon@gmail.com>, Benoit Lobréau <benoit.lobreau@dalibo.com>, Denis Laxalde <denis.laxalde@dalibo.com>, Dalibo <contact@dalibo.com>
 Maintainer-email: Denis Laxalde <denis.laxalde@dalibo.com>, Benoit Lobréau <benoit.lobreau@dalibo.com>
 License: PostgreSQL
 Project-URL: Bug Tracker, https://github.com/dalibo/pg_activity/issues/
 Project-URL: Changelog, https://github.com/dalibo/pg_activity/blob/master/CHANGELOG.md
 Project-URL: Homepage, https://github.com/dalibo/pg_activity
```

### Comparing `pg-activity-3.4.0/pg_activity.egg-info/SOURCES.txt` & `pg-activity-3.4.1/pg_activity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/pgactivity/activities.py` & `pg-activity-3.4.1/pgactivity/activities.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/pgactivity/cli.py` & `pg-activity-3.4.1/pgactivity/cli.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/pgactivity/colors.py` & `pg-activity-3.4.1/pgactivity/colors.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/pgactivity/config.py` & `pg-activity-3.4.1/pgactivity/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import os
 from pathlib import Path
 from typing import IO, Any, Dict, List, Optional, Type, TypeVar
 
 import attr
 from attr import validators
 
+from .compat import gt
+
 
 class ConfigurationError(Exception):
     def __init__(self, filename: str, *args: Any) -> None:
         super().__init__(*args)
         self.filename = filename
 
     @property
@@ -157,24 +159,22 @@
             flag ^= cls.IOWAIT
         return flag
 
 
 @attr.s(auto_attribs=True, frozen=True, slots=True)
 class UISection:
     hidden: bool = False
-    width: Optional[int] = attr.ib(
-        default=None, validator=validators.optional(validators.gt(0))
-    )
+    width: Optional[int] = attr.ib(default=None, validator=validators.optional(gt(0)))
 
     _T = TypeVar("_T", bound="UISection")
 
     @classmethod
     def from_config_section(cls: Type[_T], section: configparser.SectionProxy) -> _T:
         values: Dict[str, Any] = {}
-        known_options = {f.alias: f for f in attr.fields(cls)}
+        known_options = {f.name: f for f in attr.fields(cls)}
         unknown_options = set(section) - set(known_options)
         if unknown_options:
             raise ValueError(f"invalid option(s): {', '.join(sorted(unknown_options))}")
         for opt, getter in (("hidden", section.getboolean), ("width", section.getint)):
             try:
                 values[opt] = getter(opt)
             except configparser.NoOptionError:
```

### Comparing `pg-activity-3.4.0/pgactivity/data.py` & `pg-activity-3.4.1/pgactivity/data.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/pgactivity/handlers.py` & `pg-activity-3.4.1/pgactivity/handlers.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/pgactivity/keys.py` & `pg-activity-3.4.1/pgactivity/keys.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/pgactivity/pg.py` & `pg-activity-3.4.1/pgactivity/pg.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/pgactivity/queries/get_blocking_oldest.sql` & `pg-activity-3.4.1/pgactivity/queries/get_blocking_oldest.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/pgactivity/queries/get_blocking_post_090200.sql` & `pg-activity-3.4.1/pgactivity/queries/get_blocking_post_090200.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/pgactivity/queries/get_blocking_post_090600.sql` & `pg-activity-3.4.1/pgactivity/queries/get_blocking_post_090600.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/pgactivity/queries/get_pg_activity_oldest.sql` & `pg-activity-3.4.1/pgactivity/queries/get_pg_activity_oldest.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/pgactivity/queries/get_pg_activity_post_090200.sql` & `pg-activity-3.4.1/pgactivity/queries/get_pg_activity_post_090200.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/pgactivity/queries/get_pg_activity_post_090600.sql` & `pg-activity-3.4.1/pgactivity/queries/get_pg_activity_post_090600.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/pgactivity/queries/get_pg_activity_post_100000.sql` & `pg-activity-3.4.1/pgactivity/queries/get_pg_activity_post_100000.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/pgactivity/queries/get_pg_activity_post_110000.sql` & `pg-activity-3.4.1/pgactivity/queries/get_pg_activity_post_110000.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/pgactivity/queries/get_pg_activity_post_130000.sql` & `pg-activity-3.4.1/pgactivity/queries/get_pg_activity_post_130000.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/pgactivity/queries/get_server_info_oldest.sql` & `pg-activity-3.4.1/pgactivity/queries/get_server_info_oldest.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/pgactivity/queries/get_server_info_post_090100.sql` & `pg-activity-3.4.1/pgactivity/queries/get_server_info_post_090100.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/pgactivity/queries/get_server_info_post_090200.sql` & `pg-activity-3.4.1/pgactivity/queries/get_server_info_post_090200.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/pgactivity/queries/get_server_info_post_090400.sql` & `pg-activity-3.4.1/pgactivity/queries/get_server_info_post_090400.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/pgactivity/queries/get_server_info_post_090600.sql` & `pg-activity-3.4.1/pgactivity/queries/get_server_info_post_090600.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/pgactivity/queries/get_server_info_post_100000.sql` & `pg-activity-3.4.1/pgactivity/queries/get_server_info_post_100000.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/pgactivity/queries/get_server_info_post_110000.sql` & `pg-activity-3.4.1/pgactivity/queries/get_server_info_post_110000.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/pgactivity/queries/get_temporary_files_oldest.sql` & `pg-activity-3.4.1/pgactivity/queries/get_temporary_files_oldest.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/pgactivity/queries/get_temporary_files_post_090100.sql` & `pg-activity-3.4.1/pgactivity/queries/get_temporary_files_post_090100.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/pgactivity/queries/get_temporary_files_post_090500.sql` & `pg-activity-3.4.1/pgactivity/queries/get_temporary_files_post_090500.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/pgactivity/queries/get_waiting_oldest.sql` & `pg-activity-3.4.1/pgactivity/queries/get_waiting_oldest.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/pgactivity/queries/get_waiting_post_090200.sql` & `pg-activity-3.4.1/pgactivity/queries/get_waiting_post_090200.sql`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/pgactivity/types.py` & `pg-activity-3.4.1/pgactivity/types.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/pgactivity/ui.py` & `pg-activity-3.4.1/pgactivity/ui.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/pgactivity/utils.py` & `pg-activity-3.4.1/pgactivity/utils.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/pgactivity/views.py` & `pg-activity-3.4.1/pgactivity/views.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/pgactivity/widgets.py` & `pg-activity-3.4.1/pgactivity/widgets.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/pyproject.toml` & `pg-activity-3.4.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     "Environment :: Console",
     "Environment :: Console :: Curses",
     "License :: OSI Approved :: PostgreSQL License",
     "Programming Language :: Python :: 3",
     "Topic :: Database",
 ]
 dependencies = [
-    "attrs >= 17, !=21.1",
+    "attrs >= 17.4, !=21.1",
     "blessed >= 1.15.0",
     "humanize >= 0.5.1",
     "importlib_metadata; python_version < '3.8'",
     "psutil >= 2.0.0",
 ]
 
 [project.optional-dependencies]
```

### Comparing `pg-activity-3.4.0/tests/conftest.py` & `pg-activity-3.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/tests/data/local-processes-input.json` & `pg-activity-3.4.1/tests/data/local-processes-input.json`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/tests/test_activities.py` & `pg-activity-3.4.1/tests/test_activities.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/tests/test_config.py` & `pg-activity-3.4.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/tests/test_data.py` & `pg-activity-3.4.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/tests/test_scroll.txt` & `pg-activity-3.4.1/tests/test_scroll.txt`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/tests/test_ui.txt` & `pg-activity-3.4.1/tests/test_ui.txt`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/tests/test_views.py` & `pg-activity-3.4.1/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/tests/test_views.txt` & `pg-activity-3.4.1/tests/test_views.txt`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/tests/test_widgets.txt` & `pg-activity-3.4.1/tests/test_widgets.txt`

 * *Files identical despite different names*

### Comparing `pg-activity-3.4.0/tox.ini` & `pg-activity-3.4.1/tox.ini`

 * *Files identical despite different names*

