# Comparing `tmp/djangoldp_energiepartagee-0.0.8.tar.gz` & `tmp/djangoldp_energiepartagee-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_energiepartagee-0.0.8.tar", last modified: Wed Feb 10 13:58:41 2021, max compression
+gzip compressed data, was "dist/djangoldp_energiepartagee-0.0.9.tar", last modified: Fri Feb 12 15:45:41 2021, max compression
```

## Comparing `djangoldp_energiepartagee-0.0.8.tar` & `djangoldp_energiepartagee-0.0.9.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-10 13:58:41.000000 djangoldp_energiepartagee-0.0.8/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-10 13:58:41.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/
--rw-rw-rw-   0 root         (0) root         (0)       32 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/settings.py
--rw-rw-rw-   0 root         (0) root         (0)    16433 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/models.py
--rw-rw-rw-   0 root         (0) root         (0)       60 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     4138 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)      548 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/djangoldp_urls.py
--rw-rw-rw-   0 root         (0) root         (0)     8965 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/views.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-10 13:58:41.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/tests/
--rw-rw-rw-   0 root         (0) root         (0)    45573 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/tests/tests_permissions.py
--rw-rw-rw-   0 root         (0) root         (0)      454 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/tests/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1464 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/tests/runner.py
--rw-rw-rw-   0 root         (0) root         (0)    10023 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/tests/tests_post.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-10 13:58:41.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     2290 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0018_auto_20210122_1229.py
--rw-rw-rw-   0 root         (0) root         (0)      589 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0034_auto_20210209_1538.py
--rw-rw-rw-   0 root         (0) root         (0)     4132 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0025_auto_20210129_1841.py
--rw-rw-rw-   0 root         (0) root         (0)      903 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0014_auto_20210121_1750.py
--rw-rw-rw-   0 root         (0) root         (0)      691 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0009_auto_20210120_1439.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0019_auto_20210124_1728.py
--rw-rw-rw-   0 root         (0) root         (0)     1201 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0011_auto_20210120_1450.py
--rw-rw-rw-   0 root         (0) root         (0)      310 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0013_merge_20210120_1916.py
--rw-rw-rw-   0 root         (0) root         (0)     1314 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0023_auto_20210125_1646.py
--rw-rw-rw-   0 root         (0) root         (0)     3345 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0005_auto_20210118_1407.py
--rw-rw-rw-   0 root         (0) root         (0)      594 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0029_auto_20210204_1428.py
--rw-rw-rw-   0 root         (0) root         (0)      697 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0021_auto_20210125_1559.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0010_auto_20210120_1442.py
--rw-rw-rw-   0 root         (0) root         (0)      444 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0017_actor_iban.py
--rw-rw-rw-   0 root         (0) root         (0)      645 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0003_profile_user.py
--rw-rw-rw-   0 root         (0) root         (0)     4811 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0007_auto_20210120_1213.py
--rw-rw-rw-   0 root         (0) root         (0)      394 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0022_auto_20210125_1606.py
--rw-rw-rw-   0 root         (0) root         (0)      619 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0032_auto_20210209_1238.py
--rw-rw-rw-   0 root         (0) root         (0)     2519 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0027_auto_20210201_1617.py
--rw-rw-rw-   0 root         (0) root         (0)      866 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0004_auto_20210114_1652.py
--rw-rw-rw-   0 root         (0) root         (0)      362 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0002_auto_20210114_1101.py
--rw-rw-rw-   0 root         (0) root         (0)     1996 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0006_auto_20210119_1237.py
--rw-rw-rw-   0 root         (0) root         (0)      582 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0024_auto_20210125_2207.py
--rw-rw-rw-   0 root         (0) root         (0)      926 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0033_auto_20210209_1258.py
--rw-rw-rw-   0 root         (0) root         (0)    10829 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0015_auto_20210122_1044.py
--rw-rw-rw-   0 root         (0) root         (0)      535 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0008_auto_20210120_1215.py
--rw-rw-rw-   0 root         (0) root         (0)      787 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0026_auto_20210201_1343.py
--rw-rw-rw-   0 root         (0) root         (0)    19750 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      852 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0028_auto_20210202_1625.py
--rw-rw-rw-   0 root         (0) root         (0)      473 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0030_contribution_contributionnumber.py
--rw-rw-rw-   0 root         (0) root         (0)      886 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0009_auto_20210120_1911.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      972 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0031_auto_20210209_1235.py
--rw-rw-rw-   0 root         (0) root         (0)     2087 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0012_auto_20210120_1553.py
--rw-rw-rw-   0 root         (0) root         (0)     1497 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0016_auto_20210122_1146.py
--rw-rw-rw-   0 root         (0) root         (0)      654 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0020_auto_20210125_1131.py
--rw-rw-rw-   0 root         (0) root         (0)     1157 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-10 13:58:41.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-10 13:58:41.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/templates/emails/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-10 13:58:41.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/templates/emails/html/
--rw-rw-rw-   0 root         (0) root         (0)     2018 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/templates/emails/html/subscription_reminder.html
--rw-rw-rw-   0 root         (0) root         (0)     4001 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/templates/emails/html/subscription_call.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-10 13:58:41.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/templates/emails/txt/
--rw-rw-rw-   0 root         (0) root         (0)     1312 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/templates/emails/txt/subscription_reminder.txt
--rw-rw-rw-   0 root         (0) root         (0)     1302 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/templates/emails/txt/subscription_call.txt
--rw-rw-rw-   0 root         (0) root         (0)       56 2021-02-10 13:58:39.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-10 13:58:41.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2021-02-10 13:58:41.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2021-02-10 13:58:41.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2021-02-10 13:58:41.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     3450 2021-02-10 13:58:41.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1666 2021-02-10 13:58:41.000000 djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      588 2021-02-10 13:58:41.000000 djangoldp_energiepartagee-0.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1080 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)      230 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)       81 2021-02-10 13:58:26.000000 djangoldp_energiepartagee-0.0.8/setup.py
--rw-r--r--   0 root         (0) root         (0)     1666 2021-02-10 13:58:41.000000 djangoldp_energiepartagee-0.0.8/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-12 15:45:41.000000 djangoldp_energiepartagee-0.0.9/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-12 15:45:41.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    16433 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/models.py
+-rw-rw-rw-   0 root         (0) root         (0)       60 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      123 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     4138 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)      548 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/djangoldp_urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     8969 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/views.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/admin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-12 15:45:41.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    45573 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/tests/tests_permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/tests/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1464 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/tests/runner.py
+-rw-rw-rw-   0 root         (0) root         (0)    10023 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/tests/tests_post.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-12 15:45:41.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     2290 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0018_auto_20210122_1229.py
+-rw-rw-rw-   0 root         (0) root         (0)      589 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0034_auto_20210209_1538.py
+-rw-rw-rw-   0 root         (0) root         (0)     4132 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0025_auto_20210129_1841.py
+-rw-rw-rw-   0 root         (0) root         (0)      903 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0014_auto_20210121_1750.py
+-rw-rw-rw-   0 root         (0) root         (0)      691 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0009_auto_20210120_1439.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0019_auto_20210124_1728.py
+-rw-rw-rw-   0 root         (0) root         (0)     1201 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0011_auto_20210120_1450.py
+-rw-rw-rw-   0 root         (0) root         (0)      310 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0013_merge_20210120_1916.py
+-rw-rw-rw-   0 root         (0) root         (0)     1314 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0023_auto_20210125_1646.py
+-rw-rw-rw-   0 root         (0) root         (0)     3345 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0005_auto_20210118_1407.py
+-rw-rw-rw-   0 root         (0) root         (0)      594 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0029_auto_20210204_1428.py
+-rw-rw-rw-   0 root         (0) root         (0)      697 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0021_auto_20210125_1559.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0010_auto_20210120_1442.py
+-rw-rw-rw-   0 root         (0) root         (0)      444 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0017_actor_iban.py
+-rw-rw-rw-   0 root         (0) root         (0)      645 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0003_profile_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     4811 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0007_auto_20210120_1213.py
+-rw-rw-rw-   0 root         (0) root         (0)      394 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0022_auto_20210125_1606.py
+-rw-rw-rw-   0 root         (0) root         (0)      619 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0032_auto_20210209_1238.py
+-rw-rw-rw-   0 root         (0) root         (0)     2519 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0027_auto_20210201_1617.py
+-rw-rw-rw-   0 root         (0) root         (0)      866 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0004_auto_20210114_1652.py
+-rw-rw-rw-   0 root         (0) root         (0)      362 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0002_auto_20210114_1101.py
+-rw-rw-rw-   0 root         (0) root         (0)     1996 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0006_auto_20210119_1237.py
+-rw-rw-rw-   0 root         (0) root         (0)      582 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0024_auto_20210125_2207.py
+-rw-rw-rw-   0 root         (0) root         (0)      926 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0033_auto_20210209_1258.py
+-rw-rw-rw-   0 root         (0) root         (0)    10829 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0015_auto_20210122_1044.py
+-rw-rw-rw-   0 root         (0) root         (0)      535 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0008_auto_20210120_1215.py
+-rw-rw-rw-   0 root         (0) root         (0)      787 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0026_auto_20210201_1343.py
+-rw-rw-rw-   0 root         (0) root         (0)    19750 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      852 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0028_auto_20210202_1625.py
+-rw-rw-rw-   0 root         (0) root         (0)      473 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0030_contribution_contributionnumber.py
+-rw-rw-rw-   0 root         (0) root         (0)      886 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0009_auto_20210120_1911.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      972 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0031_auto_20210209_1235.py
+-rw-rw-rw-   0 root         (0) root         (0)     2087 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0012_auto_20210120_1553.py
+-rw-rw-rw-   0 root         (0) root         (0)     1497 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0016_auto_20210122_1146.py
+-rw-rw-rw-   0 root         (0) root         (0)      654 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0020_auto_20210125_1131.py
+-rw-rw-rw-   0 root         (0) root         (0)     1157 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-12 15:45:41.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-12 15:45:41.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/templates/emails/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-12 15:45:41.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/templates/emails/html/
+-rw-rw-rw-   0 root         (0) root         (0)     3572 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/templates/emails/html/subscription_reminder.html
+-rw-rw-rw-   0 root         (0) root         (0)     4001 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/templates/emails/html/subscription_call.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-12 15:45:41.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/templates/emails/txt/
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/templates/emails/txt/subscription_reminder.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/templates/emails/txt/subscription_call.txt
+-rw-rw-rw-   0 root         (0) root         (0)       56 2021-02-12 15:45:39.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-12 15:45:41.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2021-02-12 15:45:41.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2021-02-12 15:45:41.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2021-02-12 15:45:41.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     3450 2021-02-12 15:45:41.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1666 2021-02-12 15:45:41.000000 djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      588 2021-02-12 15:45:41.000000 djangoldp_energiepartagee-0.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1080 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      230 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)       81 2021-02-12 15:45:25.000000 djangoldp_energiepartagee-0.0.9/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2021-02-12 15:45:41.000000 djangoldp_energiepartagee-0.0.9/PKG-INFO
```

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/models.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/models.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/permissions.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/permissions.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/djangoldp_urls.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/djangoldp_urls.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/views.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
 
 class ContributionsReminderView(APIView):
     authentication_classes = (NoCSRFAuthentication,)
 
     def dispatch(self, request, *args, **kwargs):
         '''overriden dispatch method to append some custom headers'''
-        response = super(ContributionsCallView, self).dispatch(request, *args, **kwargs)
+        response = super(ContributionsReminderView, self).dispatch(request, *args, **kwargs)
         response["Access-Control-Allow-Origin"] = request.META.get('HTTP_ORIGIN')
         response["Access-Control-Allow-Methods"] = "POST"
         response["Access-Control-Allow-Headers"] = "authorization, Content-Type, if-match, accept, cache-control, pragma, user-agent"
         response["Access-Control-Expose-Headers"] = "Location, User"
         response["Access-Control-Allow-Credentials"] = 'true'
         response["Accept-Post"] = "*/*"
         response["Accept"] = "*/*"
```

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/tests/tests_permissions.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/tests/tests_permissions.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/tests/runner.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/tests/runner.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/tests/tests_post.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/tests/tests_post.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0018_auto_20210122_1229.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0018_auto_20210122_1229.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0034_auto_20210209_1538.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0034_auto_20210209_1538.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0025_auto_20210129_1841.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0025_auto_20210129_1841.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0014_auto_20210121_1750.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0014_auto_20210121_1750.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0009_auto_20210120_1439.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0009_auto_20210120_1439.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0019_auto_20210124_1728.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0019_auto_20210124_1728.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0011_auto_20210120_1450.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0011_auto_20210120_1450.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0023_auto_20210125_1646.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0023_auto_20210125_1646.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0005_auto_20210118_1407.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0005_auto_20210118_1407.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0029_auto_20210204_1428.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0029_auto_20210204_1428.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0021_auto_20210125_1559.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0021_auto_20210125_1559.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0010_auto_20210120_1442.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0010_auto_20210120_1442.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0003_profile_user.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0003_profile_user.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0007_auto_20210120_1213.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0007_auto_20210120_1213.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0032_auto_20210209_1238.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0032_auto_20210209_1238.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0027_auto_20210201_1617.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0027_auto_20210201_1617.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0004_auto_20210114_1652.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0004_auto_20210114_1652.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0006_auto_20210119_1237.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0006_auto_20210119_1237.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0024_auto_20210125_2207.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0024_auto_20210125_2207.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0033_auto_20210209_1258.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0033_auto_20210209_1258.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0015_auto_20210122_1044.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0015_auto_20210122_1044.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0008_auto_20210120_1215.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0008_auto_20210120_1215.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0026_auto_20210201_1343.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0026_auto_20210201_1343.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0001_initial.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0028_auto_20210202_1625.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0028_auto_20210202_1625.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0009_auto_20210120_1911.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0009_auto_20210120_1911.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0031_auto_20210209_1235.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0031_auto_20210209_1235.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0012_auto_20210120_1553.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0012_auto_20210120_1553.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0016_auto_20210122_1146.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0016_auto_20210122_1146.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/migrations/0020_auto_20210125_1131.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/migrations/0020_auto_20210125_1131.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/filters.py` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/filters.py`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/templates/emails/html/subscription_call.html` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/templates/emails/html/subscription_call.html`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             display: flex;
             position: relative;
             margin-bottom: 80px;
             border-radius: 20px 20px 0 0;
         }
         h2 {
             color: white;
-            font-size: 45px;
+            font-size: 35px;
             font-weight: 800;
             margin: auto;
         }
         .logo {
             height: 120px;
             width: 100px;
             position: absolute;
@@ -48,17 +48,17 @@
         }
         .email-content {
             max-width: 800px;
             margin: auto;
             width: 90%;
         }
         p {
-            font-size: 20px;
+            font-size: 16px;
             font-weight: 300;
-            line-height: 25px;
+            line-height: 20px;
             margin: 30px 0;
         }
         a {
             color:#65aa04;
         }
         b {
             font-weight: 600;
```

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/templates/emails/txt/subscription_reminder.txt` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/templates/emails/txt/subscription_call.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Relance d'appel à cotisation  {{contribution.year}}
+Appel à cotisation  {{contribution.year}}
 
 Bonjour {{user.name}},
 Nous avons le plaisir de compter {{actor.name}} parmi nos membres et vous êtes indiqué comme contact de gestion.
 
 
 
 Pour renouveler l’adhésion de votre structure au réseau de l’énergie citoyenne, nous vous invitons à récupérer votre appel à cotisation dans votre espace membre ici : https://membre.energie-partagee.org
```

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee/templates/emails/txt/subscription_call.txt` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee/templates/emails/txt/subscription_reminder.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,21 @@
-Appel à cotisation  {{contribution.year}}
+Relance d'appel à cotisation  {{contribution.year}}
 
 Bonjour {{user.name}},
-Nous avons le plaisir de compter {{actor.name}} parmi nos membres et vous êtes indiqué comme contact de gestion.
 
+Sauf erreur de notre part, nous n'avons pas reçu votre règlement pour l'adhésion {{contribution.year}}.
+Nous vous invitons à procéder au règlement de {{contribution.amount}}€.
 
+Référence :{{actor.regionalnetwork.code}}-{{contribution.year}}-{{contribution.contributionnumber}}
 
-Pour renouveler l’adhésion de votre structure au réseau de l’énergie citoyenne, nous vous invitons à récupérer votre appel à cotisation dans votre espace membre ici : https://membre.energie-partagee.org
+Vous trouverez votre appel à cotisation sur votre espace membre : https://membre.energie-partagee.org
 
-Grâce à cette double adhésion à {{actor.regionalnetwork.name}} et Energie Partagée vous avez accès à l'ensemble des services du réseau.
-
-Votre cotisation {{contribution.year}} est de {{contribution.amount}}€. 
-Référence : {{actor.regionalnetwork.code}}-{{contribution.year}}-{{contribution.id}}
-
-Nous vous invitons à régler
-- par virement (de préférence) :
-IBAN : {{actor.regionalnetwork.iban}}
-BIC : {{actor.regionalnetwork.bic}}
-- ou par chèque à l'ordre :
-{{actor.regionalnetwork.name}} 
-{{actor.regionalnetwork.address}} 
-{{actor.regionalnetwork.postcode}} {{actor.regionalnetwork.city}}
+Modalité de règlement :
+- par virement (de préférence) : IBAN : {{actor.regionalnetwork.iban}} - BIC {{actor.regionalnetwork.bic}}
+- ou par chèque à l'ordre de {{actor.regionalnetwork.name}}, {{actor.regionalnetwork.address}}, {{actor.regionalnetwork.postcode}} {{actor.regionalnetwork.city}}
 
 Après réception de votre cotisation, nous mettrons votre reçu à disposition dans votre espace membre.
 
-Pour toute question sur l'adhésion et la cotisation, n'hésitez pas à nous contacter.
-{{actor.regionalnetwork.usercontact.first_name}} {{actor.regionalnetwork.usercontact.last_name}}
+Pour toutes autres questions sur votre adhésion, nous restons à votre disposition.
+Cordialement,
+
+{{actor.regionalnetwork.usercontact.first_name}} {{actor.regionalnetwork.usercontact.last_name}}
```

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee.egg-info/SOURCES.txt` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/djangoldp_energiepartagee.egg-info/PKG-INFO` & `djangoldp_energiepartagee-0.0.9/djangoldp_energiepartagee.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangoldp-energiepartagee
-Version: 0.0.8
+Version: 0.0.9
 Summary: Custom DjangoLDP based package for Energie Partagee
 Home-page: UNKNOWN
 License: MIT
 Description: # djangoldp_energiepartagee
         How to install the project locally
         
         1- create virtual environement
```

### Comparing `djangoldp_energiepartagee-0.0.8/setup.cfg` & `djangoldp_energiepartagee-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/README.md` & `djangoldp_energiepartagee-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp_energiepartagee-0.0.8/PKG-INFO` & `djangoldp_energiepartagee-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangoldp_energiepartagee
-Version: 0.0.8
+Version: 0.0.9
 Summary: Custom DjangoLDP based package for Energie Partagee
 Home-page: UNKNOWN
 License: MIT
 Description: # djangoldp_energiepartagee
         How to install the project locally
         
         1- create virtual environement
```

