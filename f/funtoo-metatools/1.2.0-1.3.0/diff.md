# Comparing `tmp/funtoo-metatools-1.2.0.tar.gz` & `tmp/funtoo-metatools-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/funtoo-metatools-1.2.0.tar", last modified: Fri Apr 28 13:38:27 2023, max compression
+gzip compressed data, was "funtoo-metatools-1.3.0.tar", last modified: Tue May 30 01:30:24 2023, max compression
```

## Comparing `funtoo-metatools-1.2.0.tar` & `funtoo-metatools-1.3.0.tar`

### file list

```diff
@@ -1,103 +1,109 @@
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       68 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/.gitignore
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1046 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      230 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/.pylintrc
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1237 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/PKG-INFO
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      755 2023-04-28 13:33:54.000000 funtoo-metatools-1.2.0/README.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        6 2023-04-28 13:35:25.000000 funtoo-metatools-1.2.0/VERSION
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/bin/
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1370 2022-07-01 21:12:13.000000 funtoo-metatools-1.2.0/bin/blos
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1736 2022-09-30 18:57:30.000000 funtoo-metatools-1.2.0/bin/deepdive
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      978 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/bin/deepquery
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)       90 2022-07-05 16:37:27.000000 funtoo-metatools-1.2.0/bin/direct-sync
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4602 2022-07-05 16:37:27.000000 funtoo-metatools-1.2.0/bin/distfile-kit-fetch
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4497 2022-04-15 18:46:15.000000 funtoo-metatools-1.2.0/bin/distfile-stats
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2845 2023-04-24 17:38:15.000000 funtoo-metatools-1.2.0/bin/doit
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4115 2022-07-02 21:37:50.000000 funtoo-metatools-1.2.0/bin/fastpull-daemon
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2201 2022-07-06 16:00:01.000000 funtoo-metatools-1.2.0/bin/fastpull-daemon-ng
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1534 2022-04-15 18:46:15.000000 funtoo-metatools-1.2.0/bin/fastpull-fixer
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1738 2023-04-24 17:38:15.000000 funtoo-metatools-1.2.0/bin/fetch
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      928 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/bin/interkit-links
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      628 2022-04-15 18:46:15.000000 funtoo-metatools-1.2.0/bin/list-kits
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      528 2022-04-15 18:46:15.000000 funtoo-metatools-1.2.0/bin/mcafee-tool
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1171 2023-03-12 20:53:30.000000 funtoo-metatools-1.2.0/bin/merge-gentoo-staging
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2271 2022-09-30 18:59:25.000000 funtoo-metatools-1.2.0/bin/merge-kits
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      974 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/bin/missing-links
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      452 2023-03-12 20:53:30.000000 funtoo-metatools-1.2.0/bin/prod-regen
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1256 2022-04-15 18:46:15.000000 funtoo-metatools-1.2.0/bin/release-yaml-test
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     3559 2022-05-27 22:00:31.000000 funtoo-metatools-1.2.0/bin/reposcan
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      525 2022-05-07 21:05:04.000000 funtoo-metatools-1.2.0/bin/storage-test
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1638 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/bin/test-metadata-extract
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/deprecated/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     3991 2022-04-15 18:46:15.000000 funtoo-metatools-1.2.0/deprecated/mongo_backends.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/docs/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      580 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/docs/Makefile
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/docs/_ext/
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/docs/_ext/_static/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1184 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/docs/_ext/_static/consoleoutput.css
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6297 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/docs/_ext/consoleoutput.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    17066 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/docs/autogen-dev.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4994 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/docs/autogen.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2063 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/docs/conf.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/docs/drafts/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    11938 2022-04-15 18:46:15.000000 funtoo-metatools-1.2.0/docs/drafts/fastpull_object_store.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4297 2022-04-15 18:46:15.000000 funtoo-metatools-1.2.0/docs/drafts/repo_defs.rst
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/docs/features/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    14475 2022-09-30 18:57:30.000000 funtoo-metatools-1.2.0/docs/features/dynamic-archives.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4371 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/docs/index.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2524 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/docs/install.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6051 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/docs/intro.rst
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6159 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/docs/meta-repo.rst
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/examples/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      192 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/examples/reposcan.gentoo.yaml
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/funtoo/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/funtoo/__init__.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/funtoo/pkgtools/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/funtoo/pkgtools/__init__.py
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)    25389 2023-04-24 17:38:15.000000 funtoo-metatools-1.2.0/funtoo/pkgtools/autogen.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    23084 2023-04-24 17:38:15.000000 funtoo-metatools-1.2.0/funtoo/pkgtools/ebuild.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6697 2023-04-26 20:36:15.000000 funtoo-metatools-1.2.0/funtoo/pkgtools/fetch.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    18724 2023-03-18 22:08:03.000000 funtoo-metatools-1.2.0/funtoo/pkgtools/github.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     9201 2023-04-24 17:38:15.000000 funtoo-metatools-1.2.0/funtoo/pkgtools/golang.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1851 2023-04-24 17:38:15.000000 funtoo-metatools-1.2.0/funtoo/pkgtools/http.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2915 2022-04-15 18:46:15.000000 funtoo-metatools-1.2.0/funtoo/pkgtools/meson.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     3148 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/funtoo/pkgtools/pages.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    10039 2022-08-17 14:46:41.000000 funtoo-metatools-1.2.0/funtoo/pkgtools/pyhelper.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     8465 2023-04-24 17:38:15.000000 funtoo-metatools-1.2.0/funtoo/pkgtools/rust.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/funtoo_metatools.egg-info/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1237 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/funtoo_metatools.egg-info/PKG-INFO
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1874 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/funtoo_metatools.egg-info/SOURCES.txt
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        1 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/funtoo_metatools.egg-info/dependency_links.txt
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      126 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/funtoo_metatools.egg-info/requires.txt
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       17 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/funtoo_metatools.egg-info/top_level.txt
--rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      535 2023-04-28 13:37:35.000000 funtoo-metatools-1.2.0/make.sh
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/metatools/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-04-15 18:46:15.000000 funtoo-metatools-1.2.0/metatools/__init__.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1049 2022-07-01 21:12:17.000000 funtoo-metatools-1.2.0/metatools/blos.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/metatools/config/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-04-15 18:46:15.000000 funtoo-metatools-1.2.0/metatools/config/__init__.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4770 2023-04-24 17:38:15.000000 funtoo-metatools-1.2.0/metatools/config/autogen.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2739 2023-04-24 17:38:15.000000 funtoo-metatools-1.2.0/metatools/config/base.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    21759 2023-04-24 17:38:15.000000 funtoo-metatools-1.2.0/metatools/config/merge.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      197 2022-04-15 18:46:15.000000 funtoo-metatools-1.2.0/metatools/config/mongodb.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1695 2023-04-24 17:38:15.000000 funtoo-metatools-1.2.0/metatools/context.py
-drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/metatools/fastpull/
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-04-15 18:46:15.000000 funtoo-metatools-1.2.0/metatools/fastpull/__init__.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     8855 2023-04-24 17:38:15.000000 funtoo-metatools-1.2.0/metatools/fastpull/core.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    27581 2023-04-26 20:35:17.000000 funtoo-metatools-1.2.0/metatools/fastpull/spider.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4759 2022-05-27 17:28:01.000000 funtoo-metatools-1.2.0/metatools/fetch_cache.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)      653 2022-07-01 21:12:17.000000 funtoo-metatools-1.2.0/metatools/hashutils.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    34325 2023-03-12 20:53:30.000000 funtoo-metatools-1.2.0/metatools/kit.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     5829 2023-04-26 21:05:34.000000 funtoo-metatools-1.2.0/metatools/kit_cache.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    14331 2022-07-07 19:53:49.000000 funtoo-metatools-1.2.0/metatools/metadata.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1225 2022-07-05 16:37:27.000000 funtoo-metatools-1.2.0/metatools/model.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7351 2022-04-15 18:46:15.000000 funtoo-metatools-1.2.0/metatools/pretty_logging.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    21883 2023-04-24 17:38:15.000000 funtoo-metatools-1.2.0/metatools/steps.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    11361 2022-07-02 21:37:50.000000 funtoo-metatools-1.2.0/metatools/store.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)    18518 2023-04-24 17:38:15.000000 funtoo-metatools-1.2.0/metatools/tree.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       22 2023-04-28 13:38:24.000000 funtoo-metatools-1.2.0/metatools/version.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1711 2022-04-15 18:46:15.000000 funtoo-metatools-1.2.0/metatools/yaml_util.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       38 2023-04-28 13:38:27.000000 funtoo-metatools-1.2.0/setup.cfg
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1101 2023-04-28 13:38:24.000000 funtoo-metatools-1.2.0/setup.py
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1107 2023-04-28 13:37:51.000000 funtoo-metatools-1.2.0/setup.py.in
--rw-r--r--   0 drobbins  (1000) drobbins  (1000)       45 2022-04-15 16:54:39.000000 funtoo-metatools-1.2.0/subpop.yaml
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-05-30 01:30:24.975848 funtoo-metatools-1.3.0/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       68 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/.gitignore
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1046 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      230 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/.pylintrc
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6778 2023-05-30 01:28:18.000000 funtoo-metatools-1.3.0/ChangeLog.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1237 2023-05-30 01:30:24.975848 funtoo-metatools-1.3.0/PKG-INFO
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      755 2023-04-29 23:29:32.000000 funtoo-metatools-1.3.0/README.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        6 2023-05-30 01:28:36.000000 funtoo-metatools-1.3.0/VERSION
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-05-30 01:30:24.967848 funtoo-metatools-1.3.0/bin/
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1370 2022-09-27 00:51:06.000000 funtoo-metatools-1.3.0/bin/blos
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1498 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/bin/deepdive
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     3982 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/bin/deepquery
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)       90 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/bin/direct-sync
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4602 2022-09-27 00:51:20.000000 funtoo-metatools-1.3.0/bin/distfile-kit-fetch
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4497 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/bin/distfile-stats
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     3809 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/bin/doit
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     4115 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/bin/fastpull-daemon
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2350 2023-05-10 22:09:00.000000 funtoo-metatools-1.3.0/bin/fastpull-daemon-ng
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1538 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/bin/fastpull-fixer
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1738 2023-04-29 23:29:32.000000 funtoo-metatools-1.3.0/bin/fetch
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      928 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/bin/interkit-links
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      628 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/bin/list-kits
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      528 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/bin/mcafee-tool
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1191 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/bin/merge-gentoo-staging
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2294 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/bin/merge-kits
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      974 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/bin/missing-links
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      452 2022-11-03 21:48:23.000000 funtoo-metatools-1.3.0/bin/prod-regen
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1256 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/bin/release-yaml-test
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     3559 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/bin/reposcan
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      525 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/bin/storage-test
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     1638 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/bin/test-metadata-extract
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-05-30 01:30:24.967848 funtoo-metatools-1.3.0/deprecated/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     3991 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/deprecated/mongo_backends.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-05-30 01:30:24.971848 funtoo-metatools-1.3.0/docs/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      580 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/docs/Makefile
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-05-30 01:30:24.971848 funtoo-metatools-1.3.0/docs/_ext/
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-05-30 01:30:24.971848 funtoo-metatools-1.3.0/docs/_ext/_static/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1184 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/docs/_ext/_static/consoleoutput.css
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6297 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/docs/_ext/consoleoutput.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    17066 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/docs/autogen-dev.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4994 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/docs/autogen.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2063 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/docs/conf.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-05-30 01:30:24.971848 funtoo-metatools-1.3.0/docs/drafts/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    11938 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/docs/drafts/fastpull_object_store.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4297 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/docs/drafts/repo_defs.rst
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-05-30 01:30:24.971848 funtoo-metatools-1.3.0/docs/features/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    14475 2022-09-26 22:11:31.000000 funtoo-metatools-1.3.0/docs/features/dynamic-archives.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4371 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/docs/index.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2524 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/docs/install.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6051 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/docs/intro.rst
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6159 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/docs/meta-repo.rst
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-05-30 01:30:24.971848 funtoo-metatools-1.3.0/examples/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      192 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/examples/reposcan.gentoo.yaml
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-05-30 01:30:24.971848 funtoo-metatools-1.3.0/funtoo/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/funtoo/__init__.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-05-30 01:30:24.971848 funtoo-metatools-1.3.0/funtoo/pkgtools/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/funtoo/pkgtools/__init__.py
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)    25532 2023-05-10 22:09:00.000000 funtoo-metatools-1.3.0/funtoo/pkgtools/autogen.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    23260 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/funtoo/pkgtools/ebuild.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     9879 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/funtoo/pkgtools/fetch.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    19138 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/funtoo/pkgtools/github.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     9201 2023-05-10 22:44:54.000000 funtoo-metatools-1.3.0/funtoo/pkgtools/golang.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1438 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/funtoo/pkgtools/http.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2915 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/funtoo/pkgtools/meson.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     3148 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/funtoo/pkgtools/pages.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    10066 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/funtoo/pkgtools/pyhelper.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     8494 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/funtoo/pkgtools/rust.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-05-30 01:30:24.971848 funtoo-metatools-1.3.0/funtoo_metatools.egg-info/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1237 2023-05-30 01:30:24.000000 funtoo-metatools-1.3.0/funtoo_metatools.egg-info/PKG-INFO
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2007 2023-05-30 01:30:24.000000 funtoo-metatools-1.3.0/funtoo_metatools.egg-info/SOURCES.txt
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        1 2023-05-30 01:30:24.000000 funtoo-metatools-1.3.0/funtoo_metatools.egg-info/dependency_links.txt
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      132 2023-05-30 01:30:24.000000 funtoo-metatools-1.3.0/funtoo_metatools.egg-info/requires.txt
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       17 2023-05-30 01:30:24.000000 funtoo-metatools-1.3.0/funtoo_metatools.egg-info/top_level.txt
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      511 2023-05-10 22:09:00.000000 funtoo-metatools-1.3.0/make.sh
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-05-30 01:30:24.971848 funtoo-metatools-1.3.0/metatools/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/metatools/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1049 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/metatools/blos.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-05-30 01:30:24.975848 funtoo-metatools-1.3.0/metatools/config/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/metatools/config/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     5547 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/metatools/config/autogen.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     2775 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/metatools/config/base.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    25753 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/metatools/config/merge.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      197 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/metatools/config/mongodb.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1695 2023-04-29 23:29:32.000000 funtoo-metatools-1.3.0/metatools/context.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-05-30 01:30:24.975848 funtoo-metatools-1.3.0/metatools/fastpull/
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)        0 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/metatools/fastpull/__init__.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     8854 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/metatools/fastpull/core.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    27038 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/metatools/fastpull/spider.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4416 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/metatools/fetch_cache.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)      653 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/metatools/hashutils.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    34989 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/metatools/kit.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     6283 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/metatools/kit_cache.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    15194 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/metatools/metadata.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1225 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/metatools/model.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     7351 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/metatools/pretty_logging.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    21741 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/metatools/steps.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    11361 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/metatools/store.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)    18866 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/metatools/tree.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       22 2023-05-30 01:30:21.000000 funtoo-metatools-1.3.0/metatools/version.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1711 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/metatools/yaml_util.py
+drwxr-xr-x   0 drobbins  (1000) drobbins  (1000)        0 2023-05-30 01:30:24.975848 funtoo-metatools-1.3.0/metatools/zmq/
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     5642 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/metatools/zmq/app_core.py
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)     2375 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/metatools/zmq/key_monkey.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     4165 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/metatools/zmq/zmq_msg_breezyops.py
+-rwxr-xr-x   0 drobbins  (1000) drobbins  (1000)      792 2023-05-29 23:29:50.000000 funtoo-metatools-1.3.0/metatools/zmq/zmq_msg_core.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       38 2023-05-30 01:30:24.975848 funtoo-metatools-1.3.0/setup.cfg
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1112 2023-05-30 01:30:21.000000 funtoo-metatools-1.3.0/setup.py
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)     1118 2023-05-30 01:30:12.000000 funtoo-metatools-1.3.0/setup.py.in
+-rw-r--r--   0 drobbins  (1000) drobbins  (1000)       45 2022-08-07 23:25:00.000000 funtoo-metatools-1.3.0/subpop.yaml
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `funtoo-metatools-1.2.0/.pre-commit-config.yaml` & `funtoo-metatools-1.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/PKG-INFO` & `funtoo-metatools-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funtoo-metatools
-Version: 1.2.0
+Version: 1.3.0
 Summary: Funtoo framework for auto-creation of ebuilds.
 Home-page: https://code.funtoo.org/bitbucket/users/drobbins/repos/funtoo-metatools/browse
 Author: Daniel Robbins
 Author-email: drobbins@funtoo.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `funtoo-metatools-1.2.0/README.rst` & `funtoo-metatools-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/bin/blos` & `funtoo-metatools-1.3.0/bin/blos`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/bin/distfile-kit-fetch` & `funtoo-metatools-1.3.0/bin/distfile-kit-fetch`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/bin/distfile-stats` & `funtoo-metatools-1.3.0/bin/distfile-stats`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/bin/doit` & `funtoo-metatools-1.3.0/bin/doit`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,28 @@
 #!/usr/bin/env python3
 
+# MODULE IMPORT SAFETY CHECK
+# ===============================================================================================================
+# This is here to remove the automatic adding of the current working directory as a module import path, which can
+# mess up if a dir name matches some module name that one of our python deps actually needs. In python-3.11+, the
+# use of the -P option to python can turn this off so this hack isn't needed:
+
+import sys, sysconfig
+orig_sys_path = sys.path
+sys.path = [sysconfig.get_path('purelib')]
+import os
+try:
+	orig_sys_path.remove(os.getcwd())
+except ValueError:
+	pass
+sys.path = orig_sys_path
+# ===============================================================================================================
+
 import argparse
 import asyncio
-import os
-import sys
 from datetime import timedelta
 
 from subpop.hub import Hub
 
 from metatools.config.autogen import AutogenConfig
 
 
@@ -19,24 +34,31 @@
 
 hub = DoItHub()
 
 import dyne.org.funtoo.metatools.pkgtools as pkgtools
 
 CLI_CONFIG = {
 	"immediate": {"default": False, "action": "store_true", "help": "Never cache HTTP(s) fetches (default 15 mins)"},
-	"fastpull_scope": {"default": "local", "action": "store", "help": "Default index into fastpull for collecting artifacts."},
+	"fastpull_scope": {"default": "local", "action": "store",
+					   "help": "Default index into fastpull for collecting artifacts."},
 	"debug": {"default": False, "action": "store_true"},
-	"fixups_url": {"default": "https://code.funtoo.org/bitbucket/scm/core/kit-fixups.git", "action": "store", "help": "kit-fixups URL to use for cloning (for generators)"},
-	"fixups_branch": {"default": "master", "action": "store", "help": "kit-fixups branch to use for cloning (for generators)"},
-	"fast": {"default": False, "action": "store_true", "help": "Skip updating kit-fixups repo (assume this has been done for us, and it's ready to go."},
+	"fixups_url": {"default": "https://code.funtoo.org/bitbucket/scm/core/kit-fixups.git", "action": "store",
+				   "help": "kit-fixups URL to use for cloning (for generators)"},
+	"fixups_branch": {"default": "master", "action": "store",
+					  "help": "kit-fixups branch to use for cloning (for generators)"},
+	"fast": {"default": False, "action": "store_true",
+			 "help": "Skip updating kit-fixups repo (assume this has been done for us, and it's ready to go."},
 	"cat": {"default": None, "action": "store", "help": "Only run autogens matching this category."},
 	"pkg": {"default": None, "action": "store", "help": "Only run autogens matching this package name."},
-	"autogens": {"default": [], "action": "store", "positional": True, "nargs": "*", "help": "Autogen.py/.yaml files to process (default is to recursively scan)"},
-	"prod": {"default": False, "action": "store_true", "help": "Indicate we are doing a production tree regen (default: just being run as a dev)"},
+	"autogens": {"default": [], "action": "store", "positional": True, "nargs": "*",
+				 "help": "Autogen.py/.yaml files to process (default is to recursively scan)"},
+	"prod": {"default": False, "action": "store_true",
+			 "help": "Indicate we are doing a production tree regen (default: just being run as a dev)"},
 	"force_dynamic": {"default": False, "action": "store_true", "help": "Force the regeneration of dynamic archives."},
+	"moonbeam": {"default": False, "action": "store_true", "help": "Enable ZeroMQ connection back to parent merge-kits process (for logging, etc.)"},
 }
 
 
 def parse_args():
 	ap = argparse.ArgumentParser()
 	for arg, kwargs in CLI_CONFIG.items():
 		if "positional" in kwargs and kwargs["positional"]:
@@ -52,28 +74,29 @@
 
 async def main_thread():
 	hub.OPT = parse_args()
 	kwargs = {}
 	for arg in set(CLI_CONFIG.keys()) - {"immediate"}:
 		kwargs[arg] = getattr(hub.OPT, arg)
 	if hub.OPT.immediate:
+		kwargs['immediate'] = True
 		kwargs['fetch_cache_interval'] = timedelta(seconds=0)
 	await pkgtools.launch(AutogenConfig, **kwargs)
+	pkgtools.model.moonbeam_msg({"hello": "there"})
 	result = await pkgtools.autogen.start()
 	pkgtools.model.log.debug("Stopping spider...")
 	await pkgtools.model.spider.stop()
 	pkgtools.model.log.debug("Spider stopped.")
 
 	return result
 
+
 if __name__ == "__main__":
 	success = asyncio.run(main_thread())
 
 	if not success:
 		sys.exit(1)
-	#	os._exit(1)
-	##	os._exit(0)
 
 # TODO: add 'facts' database concept to allow more resiliency on failures (fall back to cached facts from last
 #       successful run)
 
 # vim: ts=4 sw=4 noet
```

### Comparing `funtoo-metatools-1.2.0/bin/fastpull-daemon` & `funtoo-metatools-1.3.0/bin/fastpull-daemon`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/bin/fastpull-daemon-ng` & `funtoo-metatools-1.3.0/bin/fastpull-daemon-ng`

 * *Files 10% similar despite different names*

```diff
@@ -60,14 +60,16 @@
 
 class Application(tornado.web.Application):
 
 	name = "direct.funtoo.org distfile service"
 	handlers = [
 		(r"/up", UptimeHandler),
 		(r"/distfiles/layout.conf", DirectHashLayoutConfHandler),
+		(r"/layout.conf", DirectHashLayoutConfHandler),
+		(r"/([0-9a-f][0-9a-f])/([0-9a-f][0-9a-f])/([0-9a-f][0-9a-f])/([0-9a-f]*)", DistfileHashHandler),
 		(r"/distfiles/([0-9a-f][0-9a-f])/([0-9a-f][0-9a-f])/([0-9a-f][0-9a-f])/([0-9a-f]*)", DistfileHashHandler),
 	]
 
 	def __init__(self):
 		tornado.web.Application.__init__(self, self.handlers, **settings)
```

### Comparing `funtoo-metatools-1.2.0/bin/fastpull-fixer` & `funtoo-metatools-1.3.0/bin/fastpull-fixer`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,21 @@
 hub = Hub()
 
 import dyne.org.funtoo.metatools.merge as merge
 import dyne.org.funtoo.metatools.pkgtools as pkgtools
 
 
 async def main_thread(delete=False):
+	merge.FIXUP_REPO = merge.tree.GitTree(
+		"kit-fixups",
+		merge.model.MERGE_CONFIG.branch("kit-fixups"),
+		url=merge.model.MERGE_CONFIG.kit_fixups,
+		root=merge.model.MERGE_CONFIG.source_trees + "/kit-fixups",
+	)
+	await merge.FIXUP_REPO.initialize()
 	for fp_entry in merge.model.FASTPULL.find({}):
 		fp_path = merge.parent.get_disk_path(fp_entry["hashes"]["sha512"])
 		if os.path.exists(fp_path):
 			continue
 		if "genpatches" in fp_entry["filename"]:
 			continue
 		skip = False
@@ -39,19 +46,10 @@
 			print("Wiped ", uri)
 			continue
 		a = pkgtools.ebuild.Artifact(url=uri)
 		await a.ensure_fetched()
 
 
 if __name__ == "__main__":
-
-	merge.FIXUP_REPO = merge.tree.GitTree(
-		"kit-fixups",
-		merge.model.MERGE_CONFIG.branch("kit-fixups"),
-		url=merge.model.MERGE_CONFIG.kit_fixups,
-		root=merge.model.MERGE_CONFIG.source_trees + "/kit-fixups",
-	)
-	merge.FIXUP_REPO.initialize()
-
 	hub.LOOP.run_until_complete(main_thread(delete=True if "delete" in sys.argv[1:] else False))
 
 # vim: ts=4 sw=4 noet
```

### Comparing `funtoo-metatools-1.2.0/bin/fetch` & `funtoo-metatools-1.3.0/bin/fetch`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/bin/interkit-links` & `funtoo-metatools-1.3.0/bin/interkit-links`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/bin/list-kits` & `funtoo-metatools-1.3.0/bin/list-kits`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/bin/mcafee-tool` & `funtoo-metatools-1.3.0/bin/mcafee-tool`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/bin/merge-gentoo-staging` & `funtoo-metatools-1.3.0/bin/merge-gentoo-staging`

 * *Files 10% similar despite different names*

```diff
@@ -7,36 +7,37 @@
 from metatools.config.base import MinimalConfig
 from metatools.kit import SimpleKitGenerator
 
 hub = Hub()
 
 # This function updates the gentoo-staging tree with all the latest gentoo updates:
 
+
 async def gentoo_staging_update():
 	model = MinimalConfig()
 	await model.initialize()
 	gentoo_staging_w = GitTree(
 		"gentoo-staging",
 		"master",
 		url="ssh://git@code.funtoo.org:7999/auto/gentoo-staging.git",
 		root=model.dest_trees + "/gentoo-staging",
 		model=model
 	)
-	gentoo_staging_w.initialize()
+	await gentoo_staging_w.initialize()
 
 	kit_gen = SimpleKitGenerator(out_tree=gentoo_staging_w)
 	gentoo_src = GitTree("gentoo-x86", "master", url="https://github.com/gentoo/gentoo.git", pull=True, model=model)
-	gentoo_src.initialize()
+	await gentoo_src.initialize()
 
 	step = SyncFromTree(
 			gentoo_src,
 			exclude=[".gitignore", "eclass/.gitignore", "metadata/.gitignore", "/metadata/cache/**", "dev-util/metro"],
 		)
 
 	await step.run(kit_gen)
-	gentoo_staging_w.gitCommit(message="gentoo updates", push=True)
+	await gentoo_staging_w.git_commit(message="gentoo updates", push=True)
 
 
 if __name__ == "__main__":
 	hub.LOOP.run_until_complete(gentoo_staging_update())
 
 # vim: ts=4 sw=4 noet
```

### Comparing `funtoo-metatools-1.2.0/bin/merge-kits` & `funtoo-metatools-1.3.0/bin/merge-kits`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,16 @@
 	await model.initialize(
 		release=args.release,
 		prod=args.prod,
 		push=not args.nopush,
 		create_branches=args.create_branches,
 		fixups_url=args.fixups_url,
 		fixups_branch=args.fixups_branch,
-		debug=args.debug
+		debug=args.debug,
+		howdy=args.howdy
 	)
 	controller = MetaRepoJobController(model, write=True)
 	try:
 		success = await controller.generate()
 		return success
 	except KeyboardInterrupt:
 		model.log.error("Keyboard interrupt -- shutting down.")
@@ -63,18 +64,18 @@
 
 CLI_CONFIG = {
 	"fixups_url": {"type": str},
 	"fixups_branch": {"type": str, "default": "master"},
 	"force": {"action": "store_true", "default": False},
 	"nopush": {"action": "store_true", "default": False},
 	"prod": {"action": "store_true", "default": False},
-	"db": {"action": "store_true", "default": False},
 	"create_branches": {"action": "store_true", "default": False},
 	"release": {"positional": True},
-	"debug": {"action": "store_true", "default": False}
+	"debug": {"action": "store_true", "default": False},
+	"howdy": {"action": "store_true", "default": False}
 }
 
 
 def parse_args():
 	ap = argparse.ArgumentParser()
 	for arg, kwargs in CLI_CONFIG.items():
 		if "os" in kwargs:
```

### Comparing `funtoo-metatools-1.2.0/bin/missing-links` & `funtoo-metatools-1.3.0/bin/missing-links`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/bin/release-yaml-test` & `funtoo-metatools-1.3.0/bin/release-yaml-test`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/bin/reposcan` & `funtoo-metatools-1.3.0/bin/reposcan`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/bin/storage-test` & `funtoo-metatools-1.3.0/bin/storage-test`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/bin/test-metadata-extract` & `funtoo-metatools-1.3.0/bin/test-metadata-extract`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/deprecated/mongo_backends.py` & `funtoo-metatools-1.3.0/deprecated/mongo_backends.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/docs/Makefile` & `funtoo-metatools-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/docs/_ext/_static/consoleoutput.css` & `funtoo-metatools-1.3.0/docs/_ext/_static/consoleoutput.css`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/docs/_ext/consoleoutput.py` & `funtoo-metatools-1.3.0/docs/_ext/consoleoutput.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/docs/autogen-dev.rst` & `funtoo-metatools-1.3.0/docs/autogen-dev.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/docs/autogen.rst` & `funtoo-metatools-1.3.0/docs/autogen.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/docs/conf.py` & `funtoo-metatools-1.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/docs/drafts/fastpull_object_store.rst` & `funtoo-metatools-1.3.0/docs/drafts/fastpull_object_store.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/docs/drafts/repo_defs.rst` & `funtoo-metatools-1.3.0/docs/drafts/repo_defs.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/docs/features/dynamic-archives.rst` & `funtoo-metatools-1.3.0/docs/features/dynamic-archives.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/docs/index.rst` & `funtoo-metatools-1.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/docs/install.rst` & `funtoo-metatools-1.3.0/docs/install.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/docs/intro.rst` & `funtoo-metatools-1.3.0/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/docs/meta-repo.rst` & `funtoo-metatools-1.3.0/docs/meta-repo.rst`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/funtoo/pkgtools/autogen.py` & `funtoo-metatools-1.3.0/funtoo/pkgtools/autogen.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,15 +309,15 @@
 						if key is None or key == "latest":
 							if "version" in pkginfo:
 								del pkginfo["version"]
 						else:
 							pkginfo["version"] = key
 						new_pkginfo_list.append(pkginfo)
 				elif isinstance(pkginfo["version"], list):
-					raise TypeError(f"Lists are not yet supported for defining multiple versions. Was processing this: {pkginfo_list}")
+					raise TypeError(f"Lists are not yet supported for defining multiple versions. Was processing this: {pkginfo['version']} {autogen_id}")
 		pkginfo_list = new_pkginfo_list
 
 		# The generator now has the ability to make arbitrary modifications to our pkginfo_list (YAML).
 		# Packages can be dropped or added, or their pkginfo arbitrarily modified using Python code.
 		# See if ``preprocess_packages()`` exists in the generator -- and if it does, run it.
 
 		preprocess_func = getattr(generator_sub, "preprocess_packages", None)
@@ -647,22 +647,25 @@
 	if fail_list:
 		failure = True
 	if not failure:
 		generate_manifests()
 		pkgtools.model.log.debug(f"FINISH: start() complete for {pkgtools.model.current_repo.root} - path 1, return True")
 		return True
 	else:
-		pkgtools.model.log.error(f"Autogen failed (count: {len(fail_list)}).")
+		pkgtools.model.log.error(f"Autogen failed (count: {len(fail_list)}). {fail_list}")
 		extra_info = []
 		if len(fail_list):
-
 			for fail in fail_list:
 				fail_info = getattr(fail, 'info', None)
 				if fail_info:
 					extra_info.append(fail_info)
+				else:
+					exc_info = getattr(fail, 'exception', None)
+					if exc_info:
+						extra_info.append(exc_info())
 		if len(extra_info):
 			# This will remove all duplicates
 			extra_info_dedup = sorted(list(set(extra_info)))
 			if len(extra_info_dedup) != len(extra_info):
 				# TODO: this duplicate failure issue is an ongoing, unresolved bug.
 				pkgtools.model.log.error(
 					f"Number of failures ({len(extra_info)}) had duplicates {len(extra_info) - len(extra_info_dedup)})")
```

### Comparing `funtoo-metatools-1.2.0/funtoo/pkgtools/ebuild.py` & `funtoo-metatools-1.3.0/funtoo/pkgtools/ebuild.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from collections import OrderedDict
 from datetime import datetime
 from subprocess import getstatusoutput
 from typing import Optional, Tuple
 
 import jinja2
 
-from metatools.steps import run_bg
+from metatools.tree import run_bg
 from metatools.store import StoreObject
 from metatools.fastpull.spider import FetchError, FetchRequest
 
 log = logging.getLogger('metatools.autogen')
 
 import dyne.org.funtoo.metatools.pkgtools as pkgtools
 
@@ -343,14 +343,17 @@
 				password=None,
 				final_name=self.final_name
 			)
 			log.debug(f'Artifact.ensure_fetched:{threading.get_ident()} now fetching {self.url} using FetchRequest {req}')
 			# TODO: this used to be indexed by catpkg, and by final_name. So we are now indexing by source URL.
 			# TODO: what exceptions are we interested in here?
 			self.blos_object = await pkgtools.model.fastpull_session.get_file_by_url(req)
+			# This above call takes some IO, so if we are being hammered with ensure_fetched() calls, this allows
+			# downloads to stay responsive, hopefully.
+			await asyncio.sleep(0)
 		except FetchError as fe:
 			# We encountered some error retrieving the resource.
 			if throw:
 				raise fe
 			log.error(f"Fetch error: {fe}")
 			return False
 		return True
```

### Comparing `funtoo-metatools-1.2.0/funtoo/pkgtools/github.py` & `funtoo-metatools-1.3.0/funtoo/pkgtools/github.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,15 +271,15 @@
 		# Have most recent by version at the beginning:
 		versions_and_release_elements = sorted(versions_and_release_elements, key=lambda v: matcher.sortable(v[0]),
 											   reverse=True)
 	if tarball or assets:
 
 		# We will look for a single specified tarball, or use an assets dict to look for a collection of assets. GitHub calls
 		# these things "assets" officially. "Tarball" is sort of funtoo slang for a single asset. It doesn't need to actually
-		# be a tarballl, it just usually is.
+		# be a tarball, it just usually is.
 
 		# Make a singleton dictionary so we can use the same code as the assets processing code. We will convert it back
 		# after.
 
 		if tarball:
 			assets = {"default": tarball}
 
@@ -289,16 +289,19 @@
 			# Expand asset filenames using version, as well as any extra keyword arguments passed to this function. This allows
 			# assets to use {slot}, etc. if slot= is passed to this function, making the string expansion feature more capable.
 			# We will also include github_user, github_repo as these could potentially be used:
 
 			# Note: this expanded_assets dict is reversed. Filenames are keys, keys are values. Minor performance improvement, pain-free:
 
 			expanded_assets = {}
-
+			add_tag_tarball = False
 			for asset_key, asset_filename in assets.items():
+				if asset_filename == "<source.tar.gz>":
+					add_tag_tarball = asset_key
+					continue
 				expanded_assets[
 					asset_filename.format(version=version, github_user=github_user, github_repo=github_repo, tag=tag_name, key=asset_key, **kwargs)] = asset_key
 			hub.pkgtools.model.log.debug(f"github: Expanded assets: {expanded_assets}")
 			found_assets = {}
 
 			for asset in release['assets']:
 				if asset['name'] in expanded_assets:
@@ -320,15 +323,18 @@
 				for artifact_key, art_kwargs in found_assets.items():
 					artifacts[artifact_key] = hub.pkgtools.ebuild.Artifact(**art_kwargs)
 
 				for key, artifact in artifacts.items():
 					if artifact.final_name == "Cargo.lock":
 						await artifact.fetch()
 						crates_dict = await hub.pkgtools.rust.get_crates_artifacts(artifact.final_path)
-
+			if add_tag_tarball:
+				# add the default .tar.gz source code generated by GitHub:
+				url = f"https://github.com/{github_user}/{github_repo}/archive/refs/tags/{tag_name}.tar.gz"
+				artifacts[add_tag_tarball] = hub.pkgtools.ebuild.Artifact(url=url, final_name=f'{github_repo}-{version}.tar.gz')
 			out_dict = {
 				"version": version,
 				"artifacts": artifacts,
 				"tag": tag_name,
 			}
 
 			if crates_dict:
```

### Comparing `funtoo-metatools-1.2.0/funtoo/pkgtools/golang.py` & `funtoo-metatools-1.3.0/funtoo/pkgtools/golang.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/funtoo/pkgtools/http.py` & `funtoo-metatools-1.3.0/funtoo/pkgtools/http.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,40 @@
 #!/usr/bin/env python3
 
-import logging
-
 import dyne.org.funtoo.metatools.pkgtools as pkgtools
 import httpx
 
-from metatools.fastpull.spider import FetchRequest, FetchError
+from metatools.fastpull.spider import FetchRequest
 
 """
 This sub implements lower-level HTTP fetching logic, such as actually grabbing the data, sending the
 proper headers and authentication, etc.
 """
 
 
-def set_basic_auth(request: FetchRequest):
-	"""
-	Keyword arguments to get_page() GET requests for authentication to certain URLs based on configuration
-	in ~/.autogen (YAML format.)
-	"""
-	if "authentication" in pkgtools.model.config:
-		if request.hostname in pkgtools.model.config["authentication"]:
-			auth_info = pkgtools.model.config["authentication"][request.hostname]
-			request.set_auth(**auth_info)
-
-
 async def get_page(url, encoding=None, is_json=False):
 	"""
 	This function performs a simple HTTP fetch of a resource. The response is cached in memory,
 	and a decoded Python string is returned with the result. FetchError is thrown for an error
 	of any kind.
 
 	Use ``encoding`` if the HTTP resource does not have proper encoding and you have to set
 	a specific encoding. Normally, the encoding will be auto-detected and decoded for you.
 	"""
 	request = FetchRequest(url=url)
-	set_basic_auth(request)
+	pkgtools.fetch.set_basic_auth(request)
 	# Leverage the spider for this fetch. This bypasses the FPOS, etc:
-	result = await pkgtools.model.spider.http_fetch(request, encoding=encoding, is_json=is_json)
+	headers, result = await pkgtools.model.spider.http_fetch(request, encoding=encoding, is_json=is_json)
 	return result
 
 
 async def get_url_from_redirect(url):
 	return await pkgtools.model.spider.get_url_from_redirect(url)
 
 
-
 async def get_response_headers(url):
 	"""
 	This function will take a URL and grab its response headers. This is useful for obtaining
 	information about a URL without fetching its body.
 	"""
 	async with httpx.AsyncClient() as client:
 		resp = await client.get(url=url, follow_redirects=True)
```

### Comparing `funtoo-metatools-1.2.0/funtoo/pkgtools/meson.py` & `funtoo-metatools-1.3.0/funtoo/pkgtools/meson.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/funtoo/pkgtools/pages.py` & `funtoo-metatools-1.3.0/funtoo/pkgtools/pages.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/funtoo/pkgtools/pyhelper.py` & `funtoo-metatools-1.3.0/funtoo/pkgtools/pyhelper.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,27 +31,20 @@
 	This function initializes metadata for the package based on pypi (and also sets defaults for things like
 	inherit.)
 	"""
 	if "inherit" not in local_pkginfo:
 		local_pkginfo["inherit"] = []
 	if "distutils-r1" not in local_pkginfo["inherit"]:
 		local_pkginfo["inherit"].append("distutils-r1")
-
-	for el in ["desc", ("home_page", "homepage"), "project_url"]:
-		if isinstance(el, tuple):
-			el, local_el = el
-		else:
-			local_el = el
-		local_pkginfo[local_el] = json_dict["info"][el] if el in json_dict["info"] else ""
-		if not isinstance(local_pkginfo[local_el], str):
-			local_pkginfo[local_el] = ""
-
-	if local_pkginfo["project_url"] != "":
-		local_pkginfo["homepage"] += " " + local_pkginfo["project_url"]
-
+	if "desc" not in local_pkginfo and "summary" in json_dict["info"] and json_dict["info"]["summary"]:
+		local_pkginfo["desc"] = json_dict["info"]["summary"]
+	if "homepage" not in local_pkginfo and "home_page" in json_dict["info"]:
+		local_pkginfo["homepage"] = f"{json_dict['info']['home_page']}"
+		if "project_url" in json_dict["info"]:
+			local_pkginfo["homepage"] += f" {json_dict['info']['project_url']}"
 	if "license" not in local_pkginfo and "classifiers" in json_dict["info"]:
 		local_pkginfo["license"] = pypi_license_to_gentoo(json_dict["info"]["classifiers"])
 
 
 def sdist_artifact_url(releases, version):
 	# Sometimes a version does not have a source tarball. This function lets us know if our version is legit.
 	# Returns artifact_url for version, or None if no sdist release was available.
@@ -147,21 +140,21 @@
 	elif pydeplabel.dep_type == "use":
 		usespec = list(pydeplabel.specifiers)[0]
 
 	for atom in atoms:
 		out_atoms.append(expand_pydep(pkginfo, atom))
 
 	if usespec:
-		out = [f"{usespec}? ( {' '.join(out_atoms)} )"]
+		out = [f"{usespec}? ( {' '.join(sorted(out_atoms))} )"]
 	elif not len(pyspec):
 		# no condition -- these deps are for all python versions, so not a conditional dep:
 		out = out_atoms
 	else:
 		# stuff everything into a python_gen_cond_dep:
-		out = [r"$(python_gen_cond_dep '"] + out_atoms + [r"' " + " ".join(pyspec), ")"]
+		out = [r"$(python_gen_cond_dep '" + ' '.join(sorted(out_atoms)) + r"' " + " ".join(sorted(pyspec)) + ")"]
 	return out
 
 
 class InvalidPyDepLabel(Exception):
 
 	def __init__(self, label, errmsg=None):
 		self.label = label
```

### Comparing `funtoo-metatools-1.2.0/funtoo/pkgtools/rust.py` & `funtoo-metatools-1.3.0/funtoo/pkgtools/rust.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 import asyncio
 import hashlib
 import shutil
 
 import dyne.org.funtoo.metatools.pkgtools as pkgtools
 from subpop.util import AttrDict
 
+from metatools.tree import run_shell
+
 
 async def add_crates_bundle(
 	hub,
 	pkginfo,
 	cargo_lock_data=None,
 	cargo_lock_path=None,
 	src_artifact=None,
@@ -229,14 +231,14 @@
 	await src_artifact.fetch()
 	src_artifact.extract()
 
 	src_dir = glob.glob(os.path.join(src_artifact.extract_path, src_dir_glob))[0]
 
 	cargo_lock_path = os.path.join(src_dir, "Cargo.lock")
 	if not os.path.exists(cargo_lock_path):
-		cargo_cmd = subprocess.Popen(["cargo", "update"], cwd=src_dir).wait()
+		result = await run_shell(["cargo", "update"], chdir=src_dir)
 
 	artifacts = await get_crates_artifacts(cargo_lock_path)
 
 	src_artifact.cleanup()
 
 	return artifacts
```

### Comparing `funtoo-metatools-1.2.0/funtoo_metatools.egg-info/PKG-INFO` & `funtoo-metatools-1.3.0/funtoo_metatools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funtoo-metatools
-Version: 1.2.0
+Version: 1.3.0
 Summary: Funtoo framework for auto-creation of ebuilds.
 Home-page: https://code.funtoo.org/bitbucket/users/drobbins/repos/funtoo-metatools/browse
 Author: Daniel Robbins
 Author-email: drobbins@funtoo.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `funtoo-metatools-1.2.0/funtoo_metatools.egg-info/SOURCES.txt` & `funtoo-metatools-1.3.0/funtoo_metatools.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .gitignore
 .pre-commit-config.yaml
 .pylintrc
+ChangeLog.rst
 README.rst
 VERSION
 make.sh
 setup.py
 setup.py.in
 subpop.yaml
 bin/blos
@@ -79,8 +80,12 @@
 metatools/config/__init__.py
 metatools/config/autogen.py
 metatools/config/base.py
 metatools/config/merge.py
 metatools/config/mongodb.py
 metatools/fastpull/__init__.py
 metatools/fastpull/core.py
-metatools/fastpull/spider.py
+metatools/fastpull/spider.py
+metatools/zmq/app_core.py
+metatools/zmq/key_monkey.py
+metatools/zmq/zmq_msg_breezyops.py
+metatools/zmq/zmq_msg_core.py
```

### Comparing `funtoo-metatools-1.2.0/metatools/blos.py` & `funtoo-metatools-1.3.0/metatools/blos.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/metatools/config/autogen.py` & `funtoo-metatools-1.3.0/metatools/config/autogen.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import os
 from collections import defaultdict
+from datetime import timedelta
 
 import yaml
 
 from metatools.blos import BaseLayerObjectStore
 from metatools.config.base import MinimalConfig
 from metatools.context import OverlayLocator, GitRepositoryLocator
 from metatools.fastpull.core import IntegrityDatabase
 from metatools.fastpull.spider import WebSpider
 from metatools.fetch_cache import FileStoreFetchCache
 from metatools.tree import GitTree
+from metatools.zmq.app_core import DealerConnection
+from metatools.zmq.zmq_msg_breezyops import BreezyMessage, MessageType
 
 
 class StoreConfig(MinimalConfig):
 	"""
 	This is used by the fastpull-daemon for access to the stores, and as a base class for AutogenConfig (used
 	by the 'doit' command).
 	"""
@@ -40,16 +43,14 @@
 			spider=self.spider,
 			hashes=self.hashes
 		)
 		self.fastpull_session = self.fpos.get_scope(self.fastpull_scope)
 
 
 class StoreSpiderConfig(StoreConfig):
-
-
 	logger_name = 'metatools.spider'
 
 	async def initialize(self, fastpull_scope=None, debug=False):
 		self.spider = WebSpider(os.path.join(self.temp_path, "spider"), hashes=self.hashes)
 		await super().initialize(fastpull_scope=fastpull_scope, debug=debug)
 
 
@@ -77,25 +78,48 @@
 		"autogen": "~/.autogen"
 	}
 
 	@property
 	def kit_spy(self):
 		"""
 		kit_spy is used for creating an autogen ID::
-		 	task_args["autogen_id"] = f"{pkgtools.model.kit_spy}:{task_args['gen_path'][len(base)+1:]}"
+			task_args["autogen_id"] = f"{pkgtools.model.kit_spy}:{task_args['gen_path'][len(base)+1:]}"
 		The autogen_id is intended to be used in the distfile integrity database, to tell use which autogen
 		referenced the artifact, in the situation where we don't have a specific BreezyBuild. This was a recent
 		add and may not be fully implemented or make sense based on our current architecture -- needs review
 		so TODO
 		"""
 		return "/".join(self.locator.root.split("/")[-2:])
 
-	async def initialize(self, fetch_cache_interval=None, fastpull_scope=None, debug=False, fixups_url=None, prod=False, force_dynamic=False, fixups_branch=None, fast=None, cat=None, pkg=None, autogens=None):
+	def moonbeam_msg(self, json_dict):
+		if not self.moonbeam:
+			return
+		msg_obj = BreezyMessage(msg_type=MessageType.INFO, service="doit", action="info", json_dict=json_dict)
+		msg_obj.send(self.moonbeam_client.client)
+		self.log.debug(f"Moonbeam: sent: {json_dict}")
+
+	async def initialize(self,
+						 immediate=False,
+						 fetch_cache_interval=None,
+						 fastpull_scope=None,
+						 debug=False,
+						 fixups_url=None,
+						 prod=False,
+						 force_dynamic=False,
+						 fixups_branch=None,
+						 fast=None,
+						 cat=None,
+						 pkg=None,
+						 autogens=None,
+						 moonbeam=False):
 		await super().initialize(fastpull_scope=fastpull_scope, debug=debug)
-
+		self.immediate = immediate
+		self.moonbeam = moonbeam
+		if self.moonbeam:
+			self.moonbeam_client = DealerConnection("moonbeam", endpoint=f"ipc://{self.moonbeam_socket}")
 		self.fetch_cache = FileStoreFetchCache(db_base_path=self.store_path)
 
 		# Process specified autogens instead of recursing:
 		self.autogens = autogens
 		self.prod = prod
 		self.force_dynamic = force_dynamic
 
@@ -134,14 +158,16 @@
 			else:
 				self.log.info(f"Generators will be sourced from {kit_fixups_root}")
 			self.kit_fixups_repo = GitRepositoryLocator(start_path=kit_fixups_root)
 
 		if fetch_cache_interval is not None:
 			# use our default unless another timedelta specified:
 			self.fetch_cache_interval = fetch_cache_interval
+		else:
+			self.fetch_cache_interval = timedelta(minutes=15)
 
 		repo_name = None
 		repo_name_path = os.path.join(self.locator.root, "profiles/repo_name")
 		if os.path.exists(repo_name_path):
 			with open(repo_name_path, "r") as repof:
 				repo_name = repof.read().strip()
 		if repo_name is None:
```

### Comparing `funtoo-metatools-1.2.0/metatools/config/base.py` & `funtoo-metatools-1.3.0/metatools/config/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 #!/usr/bin/python3
 import atexit
 import logging
 import os
 
-from metatools.model import set_model
-from metatools.pretty_logging import TornadoPrettyLogFormatter
+from rich.logging import RichHandler
 from subpop.config import SubPopModel
 
-import logging
-from rich.logging import RichHandler
+from metatools.model import set_model
 
 
 class MinimalConfig(SubPopModel):
 	"""
 	This class contains configuration settings common to all the metatools plugins and tools.
 	"""
 
@@ -25,15 +23,15 @@
 		self.log = logging.getLogger(self.logger_name)
 		self.log.propagate = False
 		if debug:
 			self.debug = debug
 			self.log.setLevel(logging.DEBUG)
 		else:
 			self.log.setLevel(logging.INFO)
-		handler = RichHandler(show_path=False)
+		handler = RichHandler(show_path=False, show_time=False)
 		self.log.addHandler(handler)
 		atexit.register(lambda: print("\x1b[?25h"))
 		if debug:
 			self.log.warning("DEBUG enabled")
 		set_model(self.logger_name, self)
 
 	@property
@@ -41,14 +39,18 @@
 		home = self.home()
 		if home:
 			return os.path.join(home, "repo_tmp")
 		else:
 			return "/var/tmp/repo_tmp"
 
 	@property
+	def moonbeam_socket(self):
+		return os.path.join(self.temp_path, "moonbeam_socket")
+
+	@property
 	def source_trees(self):
 		return os.path.join(self.work_path, "source-trees")
 
 	@property
 	def store_path(self):
 		return os.path.join(self.work_path, "stores")
```

### Comparing `funtoo-metatools-1.2.0/metatools/config/merge.py` & `funtoo-metatools-1.3.0/metatools/config/merge.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,92 +17,100 @@
 """
 This file contains classes used to create an object model for the contents of a releases/<release>.yaml file,
 to more easily interact with the logical contents of this file without having to know the intricacies of the
 actual file format.
 """
 
 
-class MergeConfig(MinimalConfig):
+class MinimalMergeConfig(MinimalConfig):
 	"""
-	This configuration is used for tree regen, also known as 'merge-kits'.
+	This configuration is for minimal tools that use merge-related data, like deepdive, for example.
+	Deepdive can use this to access the release YAML without worrying about more complex data.
 	"""
 
 	# Configuration bits:
 
 	release_yaml = None
+	release = None
 	context = None
 	locator = None
-	meta_repo = None
-	prod = False
-	release = None
-	push = False
-	create_branches = False
-	mirror_repos = False
-	nest_kits = True
-	git_class = AutoCreatedGitTree
-	git_kwargs = {}
 	fixups_url = None
 	fixups_branch = None
-
 	# Things used during runtime processing:
 	kit_fixups: GitTree = None
-	# TODO: should probably review the error/warning stats variables here:
-	metadata_error_stats = []
-	processing_warning_stats = []
-	processing_error_stats = []
-	start_time: datetime = None
-	current_source_def = None
+	logger_name = "metatools.merge"
 	log = None
 	debug = False
-	logger_name = "metatools.merge"
 
-	async def initialize(self, prod=False, push=False, release=None, create_branches=False, fixups_url=None,
-						 fixups_branch=None, debug=False):
+	async def initialize(self, release=None, fixups_url=None, fixups_branch=None, debug=False):
 		await super().initialize(debug=debug)
-		self.prod = prod
-		self.push = push
-		self.release = release
-		self.create_branches = create_branches
-		self.fixups_url = fixups_url
-		self.fixups_branch = fixups_branch
-		self.debug = debug
-
 		self.log.debug("Trying to find kit-fixups")
-
 		# TODO: refuse to use any source repository that has local changes (use git status --porcelain | wc -l)
 		self.context = os.path.join(self.source_trees, "kit-fixups")
 		self.kit_fixups = GitTree(
 			name='kit-fixups',
 			root=self.context,
 			model=self,
 			url=fixups_url,
 			branch=fixups_branch,
 			keep_branch=True
 		)
 		self.log.debug("Initializing kit-fixups repository in model init")
-		self.kit_fixups.initialize()
+		await self.kit_fixups.initialize()
 		self.locator = GitRepositoryLocator(start_path=self.kit_fixups.root)
-
+		self.release = release
 		self.release_yaml = ReleaseYAML(self)
 
+
+class MergeConfig(MinimalMergeConfig):
+	"""
+	This configuration is used for tree regen, also known as 'merge-kits'.
+	"""
+
+	meta_repo = None
+	prod = False
+	push = False
+	create_branches = False
+	mirror_repos = False
+	nest_kits = True
+	git_class = AutoCreatedGitTree
+	git_kwargs = {}
+	howdy = False
+
+	# TODO: should probably review the error/warning stats variables here:
+	metadata_error_stats = []
+	processing_warning_stats = []
+	processing_error_stats = []
+	start_time: datetime = None
+	current_source_def = None
+
+	async def initialize(self, prod=False, push=False, release=None, create_branches=False, fixups_url=None,
+						 fixups_branch=None, debug=False, howdy=False):
+
+		self.prod = prod
+		self.push = push
+		self.create_branches = create_branches
+		self.howdy = howdy
+
 		# TODO: add a means to override the remotes in the release.yaml using a local config file.
 
 		if not self.prod:
 			# The ``push`` keyword argument only makes sense in prod mode. If not in prod mode, we don't push.
 			self.push = False
 		else:
-
 			# In this mode, we're actually wanting to update real kits, and likely are going to push our updates to remotes (unless
 			# --nopush is specified as an arg.) This might be used by people generating their own custom kits for use on other systems,
 			# or by Funtoo itself for updating official kits and meta-repo.
 			self.push = push
 			self.nest_kits = False
 			self.mirror_repos = push
 			self.git_class = GitTree
 			self.git_kwargs = {"checkout_all_branches": True}
+
+		await super().initialize(release=release, fixups_url=fixups_url, fixups_branch=fixups_branch, debug=debug)
 		self.log.debug("Model initialization complete.")
 
 
 class SourceRepository:
 	"""
 	This SourceRepository represents a single source repository referenced in the YAML. This source repository
 	is used as a source tree for copying in ebuilds and eclasses into a kit.
@@ -112,63 +120,105 @@
 				 notes=None):
 		self.yaml = yaml
 		assert yaml is not None
 		self.name = name
 		self.copyright = copyright
 		self.url = url
 		self.eclasses = eclasses
+		self.notes = notes
+		# This can be used to track a GitTree associated with the source repository.
+		self.tree = None
 		self.src_sha1 = src_sha1
-		self.branch = branch if branch else "master"
+		self.branch = branch
+		self.initialized = False
+
+	async def initialize(self):
+		# This is a simple source repository -- we only want to initialize it once:
+		if self.initialized:
+			return
+		self.yaml.model.log.info(
+			f"Initializing: Source Repository {self.name} branch: {self.branch} SHA1: {self.src_sha1} {self.url}")
+		self.tree = GitTree(
+			self.name,
+			url=self.url,
+			root="%s/%s" % (self.yaml.model.source_trees, self.name),
+			branch=self.branch,
+			commit_sha1=self.src_sha1,
+			origin_check=False,
+			reclone=False,
+			model=self.yaml.model
+		)
+		await self.tree.initialize()
+		self.initialized = True
+
+	def find_license(self, license):
+		try:
+			return self.tree.find_license(license)
+		except FileNotFoundError:
+			self.yaml.model.log.error(f"No license named '{license}' found in SourceRepository {self.name}")
+
+
+class SharedSourceRepository(SourceRepository):
+	"""
+	SharedSourceRepository is a source repository referenced by a source collection. Source collections can be shared.
+
+	Different kits can use different snapshots of the same source repository, so special care needs to be given to
+	allowing a re-initialization of the tree so it is on the proper SHA1/branch. This is done by the initialize() call
+	rather than the constructor.
+
+	There is special code in here to attempt to not unnecessarily re-initialize git repositories that are already ready
+	for use. SharedSourceRepository objects can be used by multiple SourceCollections. There is a 1:1 mapping between
+	SharedSourceRepository and the underlying GitTree() object. So we only have one GitTree() for a particular repo,
+	such as a gentoo-staging repo, even if different source collections leverage different SHA1 snapshots.
+	"""
+
+	def __init__(self, yaml=None, name=None, copyright=None, url=None, eclasses=None, notes=None):
+		self.yaml = yaml
+		assert yaml is not None
+		self.name = name
+		self.copyright = copyright
+		self.url = url
+		self.eclasses = eclasses
 		self.notes = notes
 		# This can be used to track a GitTree associated with the source repository.
 		self.tree = None
 
-	def initialize(self, branch="master"):
+	async def initialize(self, branch=None, src_sha1=None):
 		if self.tree:
-			if branch == self.branch:
+			if (branch is None or self.tree.branch == branch) and src_sha1 == self.tree.commit_sha1:
+				self.yaml.model.log.info(
+					f"Keeping existing source repository {self.name} branch: {self.tree.branch} SHA1: {self.tree.commit_sha1} {self.url}")
 				return
 			else:
-				self.yaml.model.log.info(f"Checkout: Source Repository {self.name} {self.branch} {self.url}")
-				self.branch = branch
-				self.tree.gitCheckout(self.branch)
+				self.yaml.model.log.info(
+					f"src repo {self.name}: initialize: {self.tree.branch}/{self.tree.commit_sha1} -> {branch}/{src_sha1}")
+				self.yaml.model.log.info(
+					f"Checkout: Source Repository {self.name} branch: {branch} SHA1: {src_sha1} {self.url}")
+				await self.tree.git_checkout(branch=branch, sha1=src_sha1)
 		else:
-			self.yaml.model.log.info(f"Initializing: Source Repository {self.name} {self.branch} {self.url}")
+			self.yaml.model.log.info(
+				f"Initializing: Source Repository {self.name} branch: {branch} SHA1: {src_sha1} {self.url}")
 			self.tree = GitTree(
 				self.name,
 				url=self.url,
 				root="%s/%s" % (self.yaml.model.source_trees, self.name),
-				branch=self.branch,
-				commit_sha1=self.src_sha1,
+				branch=branch,
+				commit_sha1=src_sha1,
 				origin_check=False,
 				reclone=False,
 				model=self.yaml.model
 			)
-			self.tree.initialize()
-
-	def find_license(self, license):
-		try:
-			return self.tree.find_license(license)
-		except FileNotFoundError:
-			self.yaml.model.log.error(f"No license named '{license}' found in SourceRepository {self.name}")
-
-	def is_equivalent(self, other):
-		"""
-		This allows comparison of source repositories. We don't ensure singletons on source repos so this allows
-		the auto-checking-out of source collections to see if the repo is the 'same' as a previously-checked-out
-		repo:
-		"""
-		if not isinstance(other, SourceRepository):
-			return NotImplementedError()
-		return self.name == other.name and self.url == other.url and self.src_sha1 == other.src_sha1 and self.branch == other.branch
+			await self.tree.initialize()
 
 
 class SourceCollection:
 	"""
-	A SourceCollection in the YAML is, as the name says, a collection of source repositories. Each kit can reference
-	one SourceCollection and copy ebuilds and eclasses from the SourceRepositories defined in each collection.
+	A SourceCollection in the YAML is, as the name says, a collection of source repositories, and it's worth
+	noting that SourceCollections aren't used by sourced kits at all. So this logic all assumes we are dealing
+	with auto-generated kits that can reference multiple repos in their packages.yaml.
 	"""
 
 	def __init__(self, name=None, yaml=None, repo_defs=None):
 		self.yaml = yaml
 		self.name = name
 		# Contains abstract definitions of repos, which we can instantiate
 		self.repo_defs = repo_defs
@@ -179,41 +229,48 @@
 			try:
 				license = self.repositories[repo].tree.find_license(license)
 			except FileNotFoundError:
 				continue
 			return license
 		self.yaml.model.log.error(f"No license named '{license}' found in SourceCollection {self.name}")
 
-	def initialize(self, repo_names=None):
+	async def initialize(self, repo_names=None):
 
 		"""
 		This method initializes the source repositories referenced by the kit to ensure that they are all initialized to the
 		proper branch and/or SHA1. Some internal checking is done to avoid re-initializing repositories unnecessarily, so if
 		they are already set up properly then no action will be taken.
+
+		Note: Due to the nature of what we're doing, these repositories are all SharedSourceRepositories.
 		"""
 
-		repo_futures = []
-		with ThreadPoolExecutor(max_workers=2) as executor:
-			for repo_name, repo_def in self.repo_defs.items():
-				# Skip any repos that we aren't using right now....
-				if repo_names is not None and repo_name not in repo_names:
-					continue
-				# If repo already exists, don't create it from scratch. Should be faster:
-				if repo_name in self.yaml.all_repo_objs:
-					self.repositories[repo_name] = self.yaml.all_repo_objs[repo_name]
-				else:
-					self.yaml.all_repo_objs[repo_name] = self.repositories[repo_name] = SourceRepository(**repo_def, yaml=self.yaml, name=repo_name)
-			for repo_name, repo in self.repositories.items():
-				fut = executor.submit(repo.initialize, repo_def["branch"] if "branch" in repo_def else "master")
-				repo_futures.append(fut)
-			for repo_fut in as_completed(repo_futures):
-				# Getting .result() will also cause any exception to be thrown:
-				repo_dict = repo_fut.result()
+		for repo_name, repo_def in self.repo_defs.items():
+			# Skip any repos that we aren't using right now....
+			if repo_names is not None and repo_name not in repo_names:
 				continue
-
+			# If repo already exists, don't create it from scratch. Should be faster:
+			if repo_name in self.yaml.all_repo_objs:
+				self.repositories[repo_name] = self.yaml.all_repo_objs[repo_name]
+			else:
+				# note that src_sha1 and branch get passed as keyword arguments to initialize() in the next loop.
+				kwargs = repo_def.copy()
+				for arg in ["src_sha1", "branch"]:
+					if arg in kwargs:
+						del kwargs[arg]
+				self.yaml.all_repo_objs[repo_name] = self.repositories[repo_name] = SharedSourceRepository(**kwargs,
+																										   yaml=self.yaml,
+																										   name=repo_name)
+		for repo_name, repo in self.repositories.items():
+			branch = None
+			src_sha1 = None
+			if "src_sha1" in self.repo_defs[repo_name]:
+				src_sha1 = self.repo_defs[repo_name]["src_sha1"]
+			if "branch" in self.repo_defs[repo_name]:
+				branch = self.repo_defs[repo_name]["branch"]
+			await repo.initialize(branch=branch, src_sha1=src_sha1)
 		self.yaml.model.current_source_def = self
 
 
 class Kit:
 	"""
 	This class represents Kit defined in the release's YAML. It contains settings from the YAML data related to how the
 	kit should be assembled. It does not contain a reference to the actual Git repository of the kit, as it is just designed
@@ -236,16 +293,16 @@
 		self.eclasses = eclasses if eclasses is not None else {}
 		self.priority = priority
 		self.aliases = aliases if aliases else []
 		self.masters = masters if masters else []
 		self.sync_url = sync_url.format(kit_name=name) if sync_url else None
 		self.settings = settings if settings is not None else {}
 
-	def initialize_sources(self):
-		self.source.initialize()
+	async def initialize_sources(self):
+		pass
 
 	def get_copyright_rst(self):
 		cur_year = str(datetime.now().year)
 		out = self.release.get_default_copyright_rst().replace("{{cur_year}}", cur_year)
 		if isinstance(self, AutoGeneratedKit):
 			for source_name in sorted(self.source.repositories.keys()):
 				source = self.source.repositories[source_name]
@@ -262,14 +319,17 @@
 class SourcedKit(Kit):
 	source: SourceRepository = None
 
 	def __init__(self, source: SourceRepository = None, **kwargs):
 		super().__init__(**kwargs)
 		self.source = source
 
+	async def initialize_sources(self):
+		await self.source.initialize()
+
 
 class AutoGeneratedKit(Kit):
 	_package_data = None
 	source: SourceCollection = None
 
 	def __init__(self, source: SourceCollection = None, **kwargs):
 		super().__init__(**kwargs)
@@ -277,35 +337,49 @@
 
 	@property
 	def package_data(self):
 		if self._package_data is None:
 			self._package_data = self._get_package_data()
 		return self._package_data
 
-	def initialize_sources(self):
+	async def initialize_sources(self):
+		"""
+		This method is used to get the SourceCollection's SharedSourceRepository objects initialized so we are ready to copy ebuilds/eclasses from
+		the right branch/SHA1.
+
+		The use of repo_names exists to inform the initialize() call of what repos we are actually going to use. There is no point in performing
+		significant IO to initialize repos that we are not actually using.
+		"""
 		repo_names = []
 		for repo_name, extra in self.get_kit_items():
 			repo_names.append(repo_name)
 		for repo_name, extra in self.get_kit_items(section="copyfiles"):
 			repo_names.append(repo_name)
 		for repo_name, extra in self.get_kit_items(section="eclasses"):
 			repo_names.append(repo_name)
-		self.source.initialize(repo_names=repo_names)
-
-	def _get_package_data(self):
+		await self.source.initialize(repo_names=repo_names)
 
+	@property
+	def packages_yaml(self):
 		# Look for branch-specific packages.yaml:
-		fn = f"{self.kit_fixups.root}/{self.name}/{self.branch}/packages.yaml"
+		fn = self.specific_packages_yaml
 		# Fallback to curated packages.yaml:
 		if not os.path.exists(fn):
 			fn = f"{self.kit_fixups.root}/{self.name}/curated/packages.yaml"
 		# Fallback to kit-wide packages.yaml:
 		if not os.path.exists(fn):
 			fn = f"{self.kit_fixups.root}/{self.name}/packages.yaml"
-		with open(fn, "r") as f:
+		return fn
+
+	@property
+	def specific_packages_yaml(self):
+		return f"{self.kit_fixups.root}/{self.name}/{self.branch}/packages.yaml"
+
+	def _get_package_data(self):
+		with open(self.packages_yaml, "r") as f:
 			return yaml.safe_load(f)
 
 	def yaml_walk(self, yaml_dict):
 		"""
 		This method will scan a section of loaded YAML and return all list elements -- the leaf items.
 		"""
 		retval = []
@@ -406,17 +480,18 @@
 	source_collections = None
 	kits = None
 	filename = None
 	remotes = None
 	masters = None
 	all_repo_objs = dict()
 
-	def __init__(self, model: MergeConfig):
+	def __init__(self, model: MinimalMergeConfig):
 		self.model = model
-		self.mode = "prod" if self.model.prod is True else "dev"
+		if isinstance(model, MergeConfig):
+			self.mode = "prod" if self.model.prod is True else "dev"
 		filename = f'{self.model.locator.root}/releases/{self.model.release}/repositories.yaml'
 		if not os.path.exists(filename):
 			raise ConfigurationError(f"Cannot find expected {filename}")
 		self.filename = filename
 		with open(filename, 'r') as f:
 			super().__init__(f)
 
@@ -430,18 +505,22 @@
 	def get_release_metadata(self):
 		return self.get_elem("release/metadata")
 
 	def get_repo_config(self, repo_name):
 		"""
 		Given a repo/kit named ``repo_name``, determine its remote based on whether we are running in dev or prod mode.
 		"""
+		if self.mode is None:
+			raise NotImplementedError("To use ReleaseYAML.get_repo_config(), use a MergeConfig() rather than MinimalMergeConfig()")
+
 		if self.mode not in self.remotes:
 			raise ConfigurationError(f"No remotes defined for '{self.mode}' in {self.filename}.")
 		if 'url' not in self.remotes[self.mode]:
 			raise ConfigurationError(f"No URL defined for '{self.mode}' in {self.filename}.")
+		self.model.log.debug(f"get_repo_config: self.mode {self.mode} url: {self.remotes[self.mode]}")
 		mirrs = []
 		if 'mirrors' in self.remotes[self.mode]:
 			for mirr in self.remotes[self.mode]['mirrors']:
 				mirrs.append(mirr)
 		return {
 			"url": self.remotes[self.mode]['url'].format(repo=repo_name),
 			"mirrors": mirrs
@@ -463,29 +542,28 @@
 
 	def _source_collections(self):
 		"""
 		A kit's packages.yaml file can be used to reference catpkgs in external overlays, as well as eclasses,
 		that should be copied into the kit when it is generated. This group of source repositories is called a
 		'source collection', and is  represented by a SourceCollection object.
 
-		One source collection is mapped to each kit in a release, in the release.yaml file 'source' YAML element.
-		A source collection has one or more repositories defined. Each source repository is represented by a
-		SourceRepository object.
+		One source collection is mapped to each auto-generated kit in a release, in the release.yaml file
+		'source' YAML element. A source collection has one or more repositories defined. Each source repository
+		is represented by a SourceRepository object.
 
 		This method returns an OrderedDict() of all SourceCollections defined in the YAML, which is indexed by
 		the YAML name of the source collection. Each kit defined in the YAML can reference one of these source
 		collections by name.
 
 		When kits are parsed by the self.kits() method, the source collection referenced by each kit will be
 		passed to the kit's constructor.
 		"""
 		source_collections = OrderedDict()
 		repositories = self._repositories()
 		for collection_name, collection_items in self.iter_groups("release/source-collections"):
-			collection_objs = []
 			names = set()
 			repo_defs = OrderedDict()
 			for repo_def in collection_items:
 				repo_name = None
 				if isinstance(repo_def, str):
 					# str -> actual pre-defined repository dict
 					repo_name = repo_def
@@ -500,14 +578,15 @@
 					repo_def = repositories[repo_name].copy()
 					repo_def.update(repo_dict)
 				if repo_name in names:
 					raise ValueError(f"Duplicate repository name {repo_name} in source collection {collection_name}")
 				names.add(repo_name)
 				repo_defs[repo_name] = repo_def
 			source_collections[collection_name] = SourceCollection(yaml=self, name=collection_name, repo_defs=repo_defs)
+			self.model.log.info(f"Added to source collection {collection_name}:\n  {repo_defs}")
 		return source_collections
 
 	def _remotes(self):
 		return self.get_elem("release/remotes")
 
 	def _kits(self):
 		"""
@@ -525,14 +604,17 @@
 			kit_name = None
 			if isinstance(kit_el, str):
 				kit_name = kit_el
 			elif isinstance(kit_el, dict):
 				kit_name = list(kit_el.keys())[0]
 				kit_insides.update(kit_el[kit_name])
 
+			# This part of the code handles parsing the YAML, and creating Kit objects, which contain the proper info
+			# within to reference the proper source repositories or source repository (in the case of sourced kits.)
+
 			kind = KitKind.AUTOGENERATED if "kind" not in kit_insides else KitKind(kit_insides["kind"])
 			if "kind" in kit_insides:
 				del kit_insides["kind"]
 			if 'source' not in kit_insides:
 				raise KeyError(f"source value for kit {kit_name} not defined -- this is likely an error.")
 			if kind == KitKind.AUTOGENERATED:
 				# autogenerated kits have kit_insides['source'] set to reference a SourceCollection object.
@@ -565,17 +647,25 @@
 														 src_sha1=s_src_sha1)
 				kits[kit_name].append(
 					SourcedKit(locator=self.model.locator, release=self, name=kit_name, **kit_insides))
 			else:
 				raise KeyError(f"Unknown kit kind '{kind}'")
 		return kits
 
-	def iter_kits(self, name=None):
+	def iter_kits(self, name=None, primary=None):
 		"""
-		This is a handy way to iterate over all kits that meet certain criteria (currently supporting kit
-		name.) This is used to get all python-kit kits for auto-USE-flag generation.
+		This is a handy way to iterate over all kits that meet certain criteria. By default, this will yield
+		individual kits, with the primary kit listed first (if there are multiple kits of the same name)
+
+		If 'name' is specified, then only yield those kits with matching name.
+		If 'primary' is True, then yield only primary kits (first kit in YAML).
 		"""
 		for kit_name, kit_list in self.kits.items():
 			if name is not None and kit_name != name:
 				continue
-			for kit in kit_list:
-				yield kit
+			if primary:
+				yield kit_list[0]
+			else:
+				for kit in kit_list:
+					yield kit
+
+# vim: ts=4 sw=4 noet
```

### Comparing `funtoo-metatools-1.2.0/metatools/context.py` & `funtoo-metatools-1.3.0/metatools/context.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/metatools/fastpull/core.py` & `funtoo-metatools-1.3.0/metatools/fastpull/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 import logging
 from datetime import datetime
 from typing import Tuple
 
 from metatools.blos import BaseLayerObjectStore
 from metatools.fastpull.spider import FetchRequest, Download
-from metatools.steps import run_bg
+from metatools.tree import run_bg
 from metatools.store import Store, FileStorageBackend, DerivedKey, StoreObject
 
 log = logging.getLogger('metatools.autogen')
 
 
 class FileIntegrityError(Exception):
 	pass
```

### Comparing `funtoo-metatools-1.2.0/metatools/fastpull/spider.py` & `funtoo-metatools-1.3.0/metatools/fastpull/spider.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 import logging
 import os
 import random
 import string
 import threading
 from collections import defaultdict
 from contextlib import asynccontextmanager
-from datetime import datetime, timedelta
+from datetime import datetime
 from json import JSONDecodeError
+from typing import Tuple, Dict
 from urllib.parse import urlparse
 
 import httpx
 import rich.progress
 
 log = logging.getLogger('metatools.autogen')
 
 
 class FetchRequest:
 
-	def __init__(self, url, retry=True, extra_headers=None, mirror_urls=None, username=None, password=None, expected_hashes=None, final_name=None):
+	def __init__(self, url, retry=True, extra_headers=None, mirror_urls=None, username=None, password=None,
+				 expected_hashes=None, final_name=None):
 		assert url is not None
 		self.url = url
 		self.retry = retry
 		self.extra_headers = extra_headers if extra_headers else {}
 		self.mirror_urls = mirror_urls if mirror_urls else []
 		# for basic auth
 		self.username = username
@@ -50,15 +52,14 @@
 		self.password = password
 
 	def __repr__(self):
 		return f"metatools.fastpull.spider.FetchRequest<{self.url}>"
 
 
 class FetchResponse:
-
 	"""
 	FetchResponse will be returned in the case of a successful download of a file. ``fetch_request``, the
 	only argument, references the original request associated with this response.
 
 	When a fetch has completed successfully, a FetchResponse will be in the following state: ``temp_path`` will
 	point to the location where the file has been downloaded. ``final_data`` will be populated to contain
 	calculated hashes and size for the downloaded file. ``completion_result`` will be set to the ultimate
@@ -143,34 +144,38 @@
 		else:
 			max_attempts = 1
 		completed = False
 
 		while not completed and attempts < max_attempts:
 			try:
 				self.reset()
-				async with client.stream("GET", url=self.request.url, headers=headers, auth=auth, follow_redirects=True) as response:
+				async with client.stream("GET", url=self.request.url, headers=headers, auth=auth,
+										 follow_redirects=True) as response:
 					if response.status_code not in [200, 206]:
 						if response.status_code in [400, 404, 410]:
 							# These are legitimate responses that indicate that the file does not exist. Therefore, we
 							# should not retry, as we should expect to get the same result.
 							retry = False
 						else:
 							retry = True
-						raise FetchError(self.request, f"HTTP fetch_stream Error {response.status_code}: {response.reason_phrase[:120]}", retry=retry)
+						raise FetchError(self.request,
+										 f"HTTP fetch_stream Error {response.status_code}: {response.reason_phrase[:120]}",
+										 retry=retry)
 					if "Content-Length" in response.headers:
 						self.total = int(response.headers["Content-Length"])
 					else:
 						self.total = 0
 					# download_task can legitimately be zero, so check explicitly against None (our "null"):
 					if self.download_task is None:
 						# Only start download progress display if the download takes a minimum # of seconds...
 						filename = self.request.filename
 						if self.total == 0:
 							filename = f"(stream) {filename}"
-						self.download_task = self.spider.progress.add_task("Download", filename=filename, total=self.total)
+						self.download_task = self.spider.progress.add_task("Download", filename=filename,
+																		   total=self.total)
 						log.debug(f"Added download task {self.download_task}, total {self.total}")
 					# DO NOT USE aiter_raw(), below!! It will result in invalid downloads from some sites!
 					async for chunk in response.aiter_bytes():
 						on_chunk(chunk, response)
 					completed = True
 			except httpx.RequestError as e:
 				log.error(f"Download failure for {self.request.url}: {str(e)}")
@@ -205,20 +210,20 @@
 			self.hash_calc_dict[h] = getattr(hashlib, h)()
 
 	def on_chunk(self, chunk, response):
 		self.fd.write(chunk)
 		for hash in self.hashes:
 			self.hash_calc_dict[hash].update(chunk)
 		self.filesize += len(chunk)
-		log.debug(f"chunk! {self.download_task} {self.request.filename}: total {self.total, type(self.total)}: {response.num_bytes_downloaded}/{self.total}")
 		if self.download_task is not None:
 			if self.total:
 				self.spider.progress.update(self.download_task, completed=response.num_bytes_downloaded)
 			else:
-				self.spider.progress.update(self.download_task, completed=response.num_bytes_downloaded, total=response.num_bytes_downloaded)
+				self.spider.progress.update(self.download_task, completed=response.num_bytes_downloaded,
+											total=response.num_bytes_downloaded)
 
 	async def launch(self) -> None:
 		"""
 		This is the lower-level download method that wraps the _http_fetch_stream() call, and ensures hashes are generated.
 
 		Upon successful completion of the download, this function will set self.final_data to the final_data (hashes and
 		size) of the downloaded file. It will also execute the completion pipeline, if any. It will return None if you
@@ -268,15 +273,14 @@
 			#       FileNotFoundError: [Errno 2] No such file or directory: '/home/drobbins/repo_tmp/tmp/spider/8dafbe2c08150bfbeeec719150b5ae1d'
 			return completion_result
 		else:
 			return None
 
 
 class FetchError(Exception):
-
 	"""
 	When this exception is raised, we can set retry to True if the failure is something that could conceivably be
 	retried, such as a network failure. However, if we are reading from a cache, then it's just going to fail again,
 	and thus retry should have the default value of False.
 
 	This exception should be raised for *all* fetch-related errors in metatools. The ``retry`` field is used internally
 	to determine whether this is a request we should legitimately retry (like intermittent network issues) or if this
@@ -288,16 +292,19 @@
 		self.msg = msg
 		self.retry = retry
 
 	def __repr__(self):
 		return f"{self.request.url}: {self.msg}"
 
 
-class WebSpider:
+class ContentNotModified(Exception):
+	pass
 
+
+class WebSpider:
 	"""
 	This class implements a Web Spider, which is used to quickly download a lot of things. This spider takes care
 	of downloading the files, and will also calculate cryptographic hashes for what it downloads. This is because
 	it's more efficient to calculate hashes while the download is being streamed rather than doing it after the
 	file has been completely downloaded.
 
 	Locking Code
@@ -326,23 +333,22 @@
 
 	def __init__(self, temp_path, hashes):
 		self.fetch_count = 0
 		self.temp_path = temp_path
 		self.hashes = hashes - {'size'}
 		self.rich = True
 		self.progress = rich.progress.Progress(
-				"[progress.percentage]{task.percentage:>3.0f}%",
-				rich.progress.TextColumn("[bold blue]{task.fields[filename]}", justify="right"),
-				rich.progress.BarColumn(bar_width=None),
-				rich.progress.DownloadColumn(),
-				rich.progress.TransferSpeedColumn(),
-				transient=True
+			"[progress.percentage]{task.percentage:>3.0f}%",
+			rich.progress.TextColumn("[bold blue]{task.fields[filename]}", justify="right"),
+			rich.progress.BarColumn(bar_width=None),
+			rich.progress.DownloadColumn(),
+			rich.progress.TransferSpeedColumn(),
+			transient=True
 		)
 
-
 	@property
 	def http_clients(self):
 		http_clients = getattr(self.thread_ctx, "http_clients", None)
 		if http_clients is None:
 			http_clients = self.thread_ctx.http_clients = {}
 		return http_clients
 
@@ -432,15 +438,16 @@
 		if completion_pipeline is None:
 			completion_pipeline = []
 		download: Download = self.get_existing_download(request)
 		if download:
 			log.debug(f"Webspider.download:{threading.get_ident()} waiting on existing download for {request.url}")
 			fut = download.get_download_future()
 			result = await fut
-			log.debug(f"Webspider.download:{threading.get_ident()} existing download for {request.url} completed, got {fut} {result}")
+			log.debug(
+				f"Webspider.download:{threading.get_ident()} existing download for {request.url} completed, got {fut} {result}")
 			return result
 		else:
 			log.debug(f"Webspider.download:{threading.get_ident()} starting new download for {request.url}")
 			download = Download(self, request, hashes=self.hashes, completion_pipeline=completion_pipeline)
 			async with self.acquire_download_slot():
 				async with self.start_download(download):
 					try:
@@ -462,18 +469,21 @@
 			try:
 				os.unlink(response.temp_path)
 			except FileNotFoundError:
 				# FL-8301: address possible race condition
 				pass
 
 	async def acquire_http_client(self, request):
-		log.debug(f"acquire_http_client: count: {len(self.http_clients)} (request for {request.hostname}) count: {self.fetch_count}")
+		# log.debug(f"acquire_http_client: count: {len(self.http_clients)} (request for {request.hostname}) count: {self.fetch_count}")
 		if request.hostname not in self.http_clients:
 			headers, auth = self.get_headers_and_auth(request)
-			client = self.http_clients[request.hostname] = httpx.AsyncClient(transport=self.transport, http2=True, base_url=request.hostname, headers=headers, auth=auth, follow_redirects=True, timeout=8)
+			client = self.http_clients[request.hostname] = httpx.AsyncClient(transport=self.transport, http2=True,
+																			 base_url=request.hostname, headers=headers,
+																			 auth=auth, follow_redirects=True,
+																			 timeout=8)
 			return client
 		else:
 			return self.http_clients[request.hostname]
 
 	def get_headers_and_auth(self, request):
 		headers = self.fetch_headers.copy()
 		if request.extra_headers:
@@ -482,15 +492,15 @@
 			headers = self.fetch_headers
 		if request.username and request.password:
 			auth = (request.username, request.password)
 		else:
 			auth = None
 		return headers, auth
 
-	async def http_fetch(self, request: FetchRequest, is_json=False, encoding=None) -> str:
+	async def http_fetch(self, request: FetchRequest, is_json=False, encoding=None, extra_headers=None) -> Tuple[Dict, str]:
 		"""
 		UBER-NOTE:
 
 		This is a non-streaming HTTP fetcher that will properly convert the request to a Python string and return the entire
 		content as a string.
 
 		Use ``encoding`` if the HTTP resource does not have proper encoding and you have to set a specific encoding for string
@@ -506,71 +516,64 @@
 		we get a 304 back, we should just use the cached resource. If we get a 200, we should update the resource.
 		This means that for every request, we should intentionally look in our fetch cache first, and see if we have
 		a resource with a "Last-Modified" header. And if we do, we use this in our request, and potentially we return
 		the entry from our fetch cache.
 
 		ETag should also be used, which will use an "If-None-Match: "etag"" request header and similarly return a 304.
 
-		We should try to have our API hit the fetch cache only once.
-
 		In addition to this, metatools has its own built-in fetch_harness() which applies a level of caching, using
 		refresh_interval. Technically, this isn't a "cache" but just a default setting for how "fresh" we need something
 		to be for us to use it. By default, the refresh_interval is set to 15 minutes. (HOWEVER, IT LOOKS LIKE WE HAVE
 		A BUG WHERE THIS DEFAULTS to ZERO).
 
 		In addition to all this, we also have a 3-time-retry-the-fetch feature, which helps with flaky network and
 		intermittent Internet connectivity issues. Plus the ability to fall back to the cached resource if the fetch failed. In
 		this case, we are intentionally using a stale resource just for the sake of getting the autogen to work, and
 		we want this -- but we also currently don't really log these in a good way, and especially for production
 		tree regen, we would not see these unless we had a way to create a report that ran at the end of autogen.
 		I have a bug open to try to fix this.
 
-		It would be really good to implement something new to fix all these things.
-
 		New logic:
-
-		first, determine if we already have the resource and we are within our fetch cache interval. If so, let's
-		just use the resource.
-
-		if we don't have the resource, obviously we don't have a cached version to use, so we need to fetch the
-		resource.
-
-		If we have a resource already but are outside of our cached interval, we should attempt to update the
-		resource, using ETag and Modified-Since if we have those cached too. We should make several attempts
-		to update the resource (3) -- and if everything fails, we can fall back and use the stale resource.
-		But hopefully we have an updated or re-checked resource. When the resource is re-checked, even if it is
-		not actually updated, we should update our "refreshed" date so it remains inside our "refresh interval"
-		for longer.
 		"""
+		accept_304 = False
 		async with self.acquire_fetch_slot(request):
 			http_client = await self.acquire_http_client(request)
 			headers, auth = self.get_headers_and_auth(request)
 			# TODO: add code to explicitly close all clients, above:
 			try:
-				log.debug(f'http_fetch: GET {request.url}')
+				if extra_headers:
+					if "If-None-Match" in extra_headers or "If-Modified-Since" in headers:
+						accept_304 = True
+					headers.update(extra_headers)
+
 				response = await http_client.get(request.url, headers=headers, auth=auth, follow_redirects=True, timeout=15)
+				log.debug(f'http_fetch: GET {response.status_code} {request.url}')
+				if accept_304 and response.status_code == 304:
+					raise ContentNotModified()
 				if response.status_code != 200:
 					if response.status_code in [400, 404, 410]:
 						# No need to retry as the server has just told us that the resource does not exist.
 						retry = False
 					else:
 						retry = True
 					try:
 						err_response = response.json()
 					except JSONDecodeError:
 						err_response = response.text
-					log.error(f"Fetch failure for {request.url}: {response.status_code} {response.reason_phrase} {err_response}")
-					raise FetchError(request, f"HTTP fetch Error: {request.url}: {response.status_code}: {response.reason_phrase} {err_response}", retry=retry)
+					log.error(
+						f"Fetch failure for {request.url}: {response.status_code} {response.reason_phrase} {err_response}")
+					raise FetchError(request,
+									 f"HTTP fetch Error: {request.url}: {response.status_code}: {response.reason_phrase} {err_response}",
+									 retry=retry)
 				if is_json:
-					return response.json()
+					return response.headers, response.json()
 				if encoding:
-					result = response.content.decode(encoding)
+					result = response.headers, response.content.decode(encoding)
 				else:
-					result = response.text
-				log.info(f'Fetched {request.url} {len(result)} bytes')
+					result = response.headers, response.text
 				return result
 			except httpx.RequestError as re:
 				raise FetchError(request, f"Could not connect to {request.url}: {repr(re)}", retry=False)
 
 	@asynccontextmanager
 	async def acquire_download_slot(self):
 		"""
@@ -639,13 +642,14 @@
 
 	def get_existing_download(self, request: FetchRequest):
 		"""
 		Get a download object for the file we're interested in if one is already being downloaded.
 		"""
 		with self.DL_ACTIVE_LOCK:
 			if request.url in self.DL_ACTIVE:
-				log.warn(f"WebSpider.get_existing_download:{threading.get_ident()} found active download for {request.url}")
+				log.warning(
+					f"WebSpider.get_existing_download:{threading.get_ident()} found active download for {request.url}")
 
 				return self.DL_ACTIVE[request.url]
 
 			log.debug(f"WebSpider.get_existing_download:{threading.get_ident()} no active download for {request.url}")
 			return None
```

### Comparing `funtoo-metatools-1.2.0/metatools/fetch_cache.py` & `funtoo-metatools-1.3.0/metatools/fetch_cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 log = logging.getLogger('metatools.autogen')
 
 class FetchCache:
 
 	async def write(self, key_dict, body=None):
 		pass
 
-	async def read(self, key_dict, max_age=None, refresh_interval=None):
+	async def read(self, key_dict, refresh_interval=None):
 		pass
 
 	async def record_fetch_failure(self, key_dict, failure_reason):
 		pass
 
 
 class FileStoreFetchCache(FetchCache):
@@ -41,32 +41,29 @@
 			"last_attempt": now,
 			"fetched_on": now,
 			"body": body
 		})
 		log.debug(f"Wrote to fetch cache, fetched_on: {now}")
 		self.store.write(key_dict)
 
-	async def read(self, key_dict, max_age=None, refresh_interval=None):
-		log.debug(f"In FileStoreFetchCache.read, refresh_interval={refresh_interval}")
-		# content_kwargs is stored at None if there are none, not an empty dict:
+	async def read(self, key_dict, refresh_interval=None):
 		try:
 			result: StoreObject = self.store.read(key_dict)
 		except NotFoundError:
 			log.debug(f"File not found in store.")
 			raise CacheMiss()
 		if result is None or "fetched_on" not in result.data:
 			log.debug(f"File found but fetched_on missing.")
 			raise CacheMiss()
+		# refresh_interval is not being used by regular get_page but is used for redirects, etc:
 		elif refresh_interval is not None:
 			if datetime.utcnow() - result.data["fetched_on"] <= refresh_interval:
 				return result.data
 			else:
 				raise CacheMiss()
-		elif max_age is not None and datetime.utcnow() - result.data["fetched_on"] > max_age:
-			raise CacheMiss()
 		else:
 			return result.data
 
 	async def record_fetch_failure(self, key_dict, failure_reason):
 		now = datetime.utcnow()
 		key_dict.update({
 			"last_attempt": now,
@@ -97,36 +94,34 @@
 
 		self.fc.update_one(
 			key_dict,
 			{"$set": {"last_attempt": now, "fetched_on": now, "metadata": metadata, "body": body}},
 			upsert=True,
 		)
 
-	async def read(self, key_dict, max_age=None, refresh_interval=None):
+	async def read(self, key_dict, refresh_interval=None):
 		"""
 		Attempt to see if the network resource or Artifact is in our fetch cache. We will return the entire MongoDB
 		document. In the case of a network resource, this includes the cached value in the 'result' field. In the
 		case of an Artifact, the 'metadata' field will include its hashes and filesize.
 	
-		``max_age`` and ``refresh_interval`` parameters are used to set criteria for what is acceptable for the
-		caller. If criteria don't match, None is returned instead of the MongoDB document.
+		The ``refresh_interval`` parameter is used to set criteria for what freshness is acceptable for the
+		caller. If criteria don't match, ``CacheMiss()`` is raised.
 	
-		In the case the document is not found or does not meet criteria, we will raise a CacheMiss exception.
+		In the case the document is not found or does not meet criteria, we will raise a ``CacheMiss`` exception.
 		"""
 
 		result = self.fc.find_one(key_dict)
 		if result is None or "fetched_on" not in result:
 			raise CacheMiss()
 		elif refresh_interval is not None:
 			if datetime.utcnow() - result["fetched_on"] <= refresh_interval:
 				return result
 			else:
 				raise CacheMiss()
-		elif max_age is not None and datetime.utcnow() - result["fetched_on"] > max_age:
-			raise CacheMiss()
 		else:
 			return result
 
 	async def record_fetch_failure(self, key_dict, failure_reason):
 		"""
 		It is important to document when fetches fail, and that is what this method is for.
 		"""
```

### Comparing `funtoo-metatools-1.2.0/metatools/hashutils.py` & `funtoo-metatools-1.3.0/metatools/hashutils.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/metatools/kit.py` & `funtoo-metatools-1.3.0/metatools/kit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #!/usr/bin/env python3
+import asyncio
 import glob
 import json
 import os
 import sys
 import threading
 from collections import defaultdict
 from concurrent.futures import as_completed
@@ -15,14 +16,15 @@
 
 import metatools.steps
 from metatools.config.merge import AutoGeneratedKit, SourcedKit
 from metatools.hashutils import get_md5
 from metatools.metadata import AUXDB_LINES, get_catpkg_relations_from_depstring, get_filedata, extract_ebuild_metadata, strip_rev
 from metatools.model import get_model
 from metatools.tree import GitTreeError, run_shell, Tree
+from metatools.zmq.app_core import RouterListener
 
 model = get_model("metatools.merge")
 
 
 class EclassHashCollection:
 	"""
 	This is just a simple class for storing the path where we grabbed all the eclasses from plus
@@ -102,14 +104,15 @@
 	active_repos = set()
 
 	kit_cache = None
 
 	eclasses = None
 	merged_eclasses = None
 	is_master = None
+	initialized = False
 
 	def __repr__(self):
 		return f"KitGenerator(kit.name={self.kit.name}, kit.branch={self.kit.branch}, kit.kind={self.kit.__class__.__name__})"
 
 	def __init__(self, controller, kit: Union[SourcedKit, AutoGeneratedKit], is_master=False):
 		self.controller = controller
 		self.kit = kit
@@ -128,16 +131,22 @@
 			root=root,
 			origin_check=True if model.prod else None,
 			mirrors=kit_config['mirrors'],
 			create_branches=model.create_branches,
 			model=model,
 			**model.git_kwargs
 		)
-		self.out_tree.initialize()
-		self.kit_cache = KitCache(name=kit.name, branch=kit.branch)
+		self.kit_cache = KitCache(model.release, name=kit.name, branch=kit.branch)
+
+	async def initialize(self):
+		await self.out_tree.initialize()
+		# load on-disk JSON metadata cache into memory:
+
+		self.kit_cache.load()
+		self.initialized = True
 
 	async def run(self, steps):
 		"""
 		This command runs a series of steps. What I need to add is proper propagation of errors to caller.
 		"""
 		for step in steps:
 			if step is not None:
@@ -353,16 +362,16 @@
 		else:
 			model.log.warning(f"No ebuilds were found when processing metadata.")
 		return all_licenses
 
 	async def fail(self):
 		raise GitTreeError()
 
-	def initialize_sources(self):
-		self.kit.initialize_sources()
+	async def initialize_sources(self):
+		await self.kit.initialize_sources()
 
 	async def generate_sourced(self):
 		"""
 		This function contains the full steps used for generating a "sourced" kit. These steps are:
 
 		1. Run autogen in the sourced tree.
 		2. Copy everything over from the sourced tree.
@@ -398,46 +407,41 @@
 		the kit is ready for finalization (gencache, etc.) and a git commit which will contain the new changes.
 		"""
 
 		await self.run(self.copy_eclasses_steps())
 		await self.run(self.packages_yaml_copy_ebuilds_steps())
 		await self.run([metatools.steps.RemoveFiles(self.kit.get_excludes())])
 
-		self.out_tree.gitAdd()
+		self.out_tree.git_add()
 
 		await self.run(self.autogen_and_copy_from_kit_fixups())
 
-	def copy_licenses(self, used_licenses=None):
+	async def copy_licenses(self, used_licenses=None):
 		needed_licenses = set()
 		os.makedirs(f"{self.out_tree.root}/licenses", exist_ok=True)
 
 		for license in used_licenses:
 			if not os.path.exists(f"{self.out_tree.root}/licenses/{license}"):
 				needed_licenses.add(license)
 
 		for license in needed_licenses:
 			found = self.kit.source.find_license(license)
 			if found:
-				run_shell(f"cp {found} {self.out_tree.root}/licenses", logger=model.log)
+				await run_shell(f"cp {found} {self.out_tree.root}/licenses", logger=model.log)
 
 	async def distfile_scan(self):
 		self.kit_cache.load()
 		# We can now perform the steps in distfile-kit-fetch as we have access to the kit-cache.
 		# TODO: add code here
 		# TODO: add extra code here to log any issues. We should temp. hook into the log handler
 		#		to re-route any messages to an appropriate log file. This would actually be a good
 		#		general idea as we don't have this mechanism in the autogen process right now
 		#		(separated logs don't go to disk.) So maybe we want to implement this outside this
 		#		method, in the KitJob.
 
-	async def reposcan(self):
-		self.fetch_kit()
-		self.gen_cache()
-		self.flush_kit()
-
 	async def generate(self):
 		"""
 		This function contains the full step-flow for updating a kit. This function handles both autogenerated kits
 		and sourced kits.
 
 		Here is a basic overview of the process:
 
@@ -448,18 +452,16 @@
 		4. Various miscellaneous tasks will be executed -- creating a global licensing information file, cleaning up of Manifests, etc.
 		5. The Portage metadata cache will be updated and stored inside the kit.
 		6. Auto-generation of Python USE settings will be performed. This optimizes the Python USE experience for Funtoo users.
 		7. Licenses used by the ebuilds will be copied over to the ``licenses/`` directory.
 		7. A new git commit within the kit will be created based on the result of these steps.
 		8. The HEAD SHA1 will be recorded so that we can record it later within the meta-repo metadata.
 		"""
-
-		# load on-disk JSON metadata cache into memory:
-
-		self.kit_cache.load()
+		if not self.initialized:
+			await self.initialize()
 
 		await self.run([
 			metatools.steps.CleanTree(),
 			metatools.steps.GenerateRepoMetadata(self.kit.name, aliases=self.kit.aliases, masters=self.kit.masters, priority=self.kit.priority),
 			metatools.steps.SyncFiles(model.kit_fixups.root, {"LICENSE.txt": "LICENSE.txt"}),
 		])
 
@@ -502,15 +504,15 @@
 		self.merged_eclasses += self.eclasses
 
 		############################################################################################################
 		# Use lots of CPU (potentially) to generate/update metadata cache:
 		############################################################################################################
 
 		used_licenses = self.gen_cache()
-		self.copy_licenses(used_licenses=used_licenses)
+		await self.copy_licenses(used_licenses=used_licenses)
 
 		############################################################################################################
 		# Python USE settings auto-generation and other finalization steps:
 		############################################################################################################
 
 		# We can now run all the steps that require access to metadata:
 
@@ -524,15 +526,15 @@
 		# When 'ego sync' runs, it will ensure that these settings are automatically enabled based upon what
 		# your currently-active python-kit is. This means that even if you have multiple python-kit branches
 		# defined in your release, switching between them is seamless and Python USE settings for all packages
 		# in the repository will auto-adapt to whatever Python kit is currently enabled.
 
 		await self.run([metatools.steps.GenPythonUse()])
 		update_msg = "Autogenerated tree updates."
-		self.out_tree.gitCommit(message=update_msg, push=model.push)
+		await self.out_tree.git_commit(message=update_msg, push=model.push)
 
 		# save in-memory metadata cache to JSON:
 		self.kit_cache.save()
 		self.kit_sha1 = self.out_tree.head()
 		# This will get passed as the "result" if run in a ThreadPoolGenerator() (when we call get_result())
 		return self
 
@@ -665,41 +667,56 @@
 	def __init__(self, jobs, method="generate"):
 		self.jobs = jobs
 		self.method = method
 
 	async def run(self):
 		for kit_job in self.jobs:
 			model.log.debug(f"KitExecutionPool: running job {kit_job}")
-			kit_job.initialize_sources()
+			await kit_job.initialize_sources()
 			method = getattr(kit_job, self.method)
 			try:
 				await method()
 				model.log.debug(f"KitExecutionPool: job {kit_job} complete")
 			except Exception as e:
 				model.log.exception("Kit job failure:")
 				return False
 		return True
 
 
+class MoonBeam(RouterListener):
+
+	def setup(self):
+		if  model.howdy:
+			asyncio.create_task(self.howdy())
+
+	async def howdy(self):
+		while True:
+			print("HOWDY")
+			await asyncio.sleep(0.1)
+
+
 class MetaRepoJobController:
 	"""
 	This class is designed to run the full meta-repo and kit regeneration process -- in other words, the entire
 	technical flow of 'merge-kits' when it creates or updates kits and meta-repo. It is designed to "go through"
 	all the kits in a release.
 	"""
 
 	master_jobs = {}
 	kit_jobs = []
 	model = None
 	meta_repo = None
 	# Does this job controller update meta-repo? If so, this get set to True, otherwise False.
 	write = False
+	moonbeam = None
+	moonbeam_task = None
 
 	def __init__(self, model, write=None):
 		self.model = model
+		self.moonbeam = MoonBeam("merge-kits", bind_addr=f"ipc://{self.model.moonbeam_socket}")
 		if write:
 			self.write = write
 		assert isinstance(self.write, bool)
 
 	def cleanup_error_logs(self):
 		# This should be explicitly called at the beginning of every command that generates metadata for kits:
 
@@ -799,36 +816,34 @@
 		if not success:
 			return False
 
 		other_pool = KitExecutionPool(jobs=other_jobs_list, method=method)
 		success = await other_pool.run()
 		return success
 
-	async def reposcan(self):
-		await self.process_all_kits_in_release(method="reposcan")
-
 	async def distfile_sync(self):
 		await self.process_all_kits_in_release(method="distfile_scan")
 
 	async def generate(self):
-
+		self.moonbeam_task = asyncio.create_task(self.moonbeam.start())
+		model.log.debug(f"moonbeam: {self.moonbeam} {self.moonbeam_task}")
 		meta_repo_config = model.release_yaml.get_repo_config("meta-repo")
 		self.meta_repo = model.git_class(
 			name="meta-repo",
 			branch=model.release,
 			url=meta_repo_config['url'] if model.prod else None,
 			root=model.dest_trees + "/meta-repo",
 			origin_check=True if model.prod else None,
 			mirrors=meta_repo_config['mirrors'],
 			create_branches=model.create_branches,
 			model=model,
 			**model.git_kwargs
 		)
 
-		self.meta_repo.initialize()
+		await self.meta_repo.initialize()
 		model.log.debug("In generate() start")
 		self.cleanup_error_logs()
 
 		success = await self.process_all_kits_in_release(method="generate")
 		if not success:
 			self.display_error_summary()
 			model.log.debug("FAILURE in process_all_kits_in_release")
@@ -836,15 +851,15 @@
 
 		if not self.write:
 			model.log.debug("not doing commit, so exiting from job controller early")
 			return True
 
 		# Create meta-repo commit referencing our updated kits:
 		self.generate_metarepo_metadata()
-		self.meta_repo.gitCommit(message="kit updates", skip=["kits"], push=model.push)
+		await self.meta_repo.git_commit(message="kit updates", skip=["kits"], push=model.push)
 
 		# TODO: implement this
 		# if not model.prod:
 		#	# check out preferred kit branches, because there's a good chance we'll be using it locally.
 		#	for name, ctx in self.get_kit_preferred_branches().items():
 		#		model.log.info(f"Checking out {name} {ctx.kit.branch}...")
 		#		await self.checkout_kit(ctx, pull=False)
@@ -852,47 +867,48 @@
 		if not model.mirror_repos:
 			model.log.debug("not mirroring repos, so exiting from job controller early")
 			self.display_error_summary()
 			return True
 
 		# Mirroring to GitHub happens here:
 		if model.push:
-			self.mirror_all_repositories()
+			await self.mirror_all_repositories()
 		model.log.debug("exiting from job controller")
 		self.display_error_summary()
 		return True
 
-	def mirror_repository(self, repo: Tree, base_path, mirror):
+	async def mirror_repository(self, repo: Tree, base_path, mirror):
 		"""
 		Mirror a repository to its mirror location, ie. GitHub.
 		"""
 
 		os.makedirs(base_path, exist_ok=True)
-		run_shell(f"git clone --bare {repo.root} {base_path}/{repo.name}.pushme", logger=model.log)
-		run_shell(
+		await run_shell(f"git clone --bare {repo.root} {base_path}/{repo.name}.pushme", logger=model.log)
+		await run_shell(
 			f"cd {base_path}/{repo.name}.pushme && git remote add upstream {mirror} && git push --mirror upstream",
 			logger=model.log
 		)
-		run_shell(f"rm -rf {base_path}/{repo.name}.pushme", logger=model.log)
+		await run_shell(f"rm -rf {base_path}/{repo.name}.pushme", logger=model.log)
 		return repo.name
 
-	def mirror_all_repositories(self):
+	# TODO: this can easily be made faster with gather:
+	async def mirror_all_repositories(self):
 		base_path = os.path.join(model.temp_path, "mirror_repos")
-		run_shell(f"rm -rf {base_path}", logger=model.log)
+		await run_shell(f"rm -rf {base_path}", logger=model.log)
 		kit_mirror_futures = []
 		for kit_job in self.kit_jobs:
 			if not kit_job.out_tree.mirrors:
 				continue
 			kit = kit_job.kit
 			for mirror in kit_job.out_tree.mirrors:
 				mirror = mirror.format(repo=kit_job.kit.name)
-				self.mirror_repository(kit_job.out_tree, base_path, mirror)
+				await self.mirror_repository(kit_job.out_tree, base_path, mirror)
 		for mirror in self.meta_repo.mirrors:
 			mirror = mirror.format(repo=self.meta_repo.name)
-			self.mirror_repository(self.meta_repo, base_path, mirror)
+			await self.mirror_repository(self.meta_repo, base_path, mirror)
 		print("Mirroring of meta-repo complete.")
 
 
 """
 class MetaRepoGenerator:
 
 	def __init__(self):
```

### Comparing `funtoo-metatools-1.2.0/metatools/kit_cache.py` & `funtoo-metatools-1.3.0/metatools/kit_cache.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,24 +11,33 @@
 
 model = get_model("metatools")
 
 
 class KitCache:
 	json_data = None
 
-	def __init__(self, name, branch):
+	def __init__(self, release, name, branch):
+		self.release = release
 		self.name = name
 		self.branch = branch
 		self.writes = set()
 		self.misses = set()
 		self.retrieved_atoms = set()
 		self.metadata_errors = {}
 		self.processing_warnings = []
 
 	def load(self):
+		# Upgrade to new path format, keeping old kit-cache:
+		if not os.path.exists(self.path):
+			if os.path.exists(self.old_path):
+				os.makedirs(os.path.dirname(self.path), exist_ok=True)
+				os.link(self.old_path, self.path)
+				os.unlink(self.old_path)
+
+		# This is the regular load logic:
 		if os.path.exists(self.path):
 			self.json_data = self.load_json()
 		else:
 			self.json_data = {"atoms": {}}
 
 	def load_json(self, validate=True):
 		"""
@@ -50,14 +59,18 @@
 					model.log.error(
 						f"Cache data version is {kit_cache_data['cache_data_version']} but needing {CACHE_DATA_VERSION}")
 					return None
 			return kit_cache_data
 
 	@property
 	def path(self):
+		return os.path.join(model.temp_path, "kit_cache", self.release, f"{self.name}-{self.branch}")
+
+	@property
+	def old_path(self):
 		return os.path.join(model.temp_path, "kit_cache", f"{self.name}-{self.branch}")
 
 	def __setitem__(self, atom, value):
 		self.json_data["atoms"][atom] = value
 		self.writes.add(atom)
 
 	def items(self):
```

### Comparing `funtoo-metatools-1.2.0/metatools/metadata.py` & `funtoo-metatools-1.3.0/metatools/metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -390,14 +390,15 @@
 	# Shall not be None:
 	assert def_python
 	# TODO: This should be fixed or replaced, because there's hard-coded thangs in here.
 	#       Best solution would be to move it to the release metadata.
 	ebs = {}
 	for cpv in cpv_list:
 		if "metadata" not in kit_gen.kit_cache[cpv]:
+			logging.warning(f"NO METADATA FOR {cpv}")
 			continue
 		metadata = kit_gen.kit_cache[cpv]["metadata"]
 		if not metadata:
 			imps = []
 		else:
 			imps = metadata["PYTHON_COMPAT"].split()
 
@@ -423,44 +424,57 @@
 				new_imps.update(["python2_7", "python3_7", "python3_8", "python3_9", "python3_10"])
 			else:
 				new_imps.add(imp)
 		imps = list(new_imps)
 		if len(imps):
 			ebs[cpv] = imps
 
-	# ebs now is a dict containing catpkg -> PYTHON_COMPAT settings for each ebuild in the catpkg. We want to see if they are identical
+	# ebs now is a dict containing catpkgversion -> PYTHON_COMPAT settings for each ebuild in the catpkg. We want to see if they are identical
 	# if split == False, then we will do one global setting for the catpkg. If split == True, we will do individual settings for each version
 	# of the catpkg, since there are differences. This saves space in our python-use file while keeping everything correct.
 
-	oldval = None
+	all_imps = None
 	split = False
-	for key, val in ebs.items():
-		if oldval is None:
-			oldval = val
+	for key, imps in ebs.items():
+		if all_imps is None:
+			all_imps = imps
 		else:
-			if oldval != val:
+			if all_imps != imps:
 				split = True
 				break
 	lines = []
 	if len(ebs.keys()):
 		if not split:
-			line = do_package_use_line(catpkg, def_python, bk_python, oldval)
+			logging.debug(f"package.use line: {catpkg}: def/bk: {def_python} {bk_python} imps: {all_imps} (NOT SPLIT)")
+			line = do_package_use_line(catpkg, def_python, bk_python, all_imps)
 			if line is not None:
 				lines.append(line)
 		else:
-			for key, val in ebs.items():
-				line = do_package_use_line("=%s" % key, def_python, bk_python, val)
+			for key, imps in ebs.items():
+				logging.debug(f"package.use line: {catpkg}: def/bk: {def_python} {bk_python} imps: {imps} (SPLIT)")
+				line = do_package_use_line("=%s" % key, def_python, bk_python, imps)
 				if line is not None:
 					lines.append(line)
 	return lines
 
 
 def do_package_use_line(pkg, def_python, bk_python, imps):
 	out = None
 	if def_python not in imps:
 		if bk_python and bk_python in imps:
 			out = "%s python_single_target_%s" % (pkg, bk_python)
 		else:
-			out = "%s python_single_target_%s python_targets_%s" % (pkg, imps[0], imps[0])
+			# This is a non-deterministic race condition as to what single implementation we choose, since imps is a
+			# list and we use imps[0]. So let's try to enforce an order. First, we will try to remove all "pypy" imps
+			# if possible, and then sort the list and use the first non-pypi implementation. This will give us
+			# consistent results regen to regen.
+			non_pypy_imps = []
+			for imp in imps:
+				if not imp.startswith("pypy"):
+					non_pypy_imps.append(imp)
+			if not len(non_pypy_imps):
+				non_pypy_imps = imps
+			non_pypy_imps = sorted(non_pypy_imps)
+			out = "%s python_single_target_%s python_targets_%s" % (pkg, non_pypy_imps[0], non_pypy_imps[0])
 	return out
 
 # vim: ts=4 sw=4 noet
```

### Comparing `funtoo-metatools-1.2.0/metatools/model.py` & `funtoo-metatools-1.3.0/metatools/model.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/metatools/pretty_logging.py` & `funtoo-metatools-1.3.0/metatools/pretty_logging.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/metatools/steps.py` & `funtoo-metatools-1.3.0/metatools/steps.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python3
-import asyncio
 import itertools
 import os
 import re
 import shutil
 import jinja2
 
 from metatools import metadata
@@ -13,23 +12,14 @@
 model = get_model("metatools.merge")
 
 
 def run_shell(cmd_list, abort_on_failure=True, chdir=None):
 	return metatools.tree.run_shell(cmd_list, abort_on_failure=abort_on_failure, chdir=chdir, logger=model.log)
 
 
-async def run_bg(cmd):
-	proc = await asyncio.create_subprocess_shell(cmd,
-	stdout=asyncio.subprocess.PIPE,
-	stderr=asyncio.subprocess.STDOUT)
-
-	stdout, stderr = await proc.communicate()
-	return proc, stdout
-
-
 class MergeStep:
 
 	# This is only used for Repository Steps:
 	collector = None
 
 	async def run(self, kit_gen):
 		pass
@@ -95,28 +85,28 @@
 			os.makedirs(dest)
 		cmd = 'rsync -a --exclude CVS --exclude .svn --filter="hide /.git" --filter="protect /.git" '
 		for e in self.exclude:
 			cmd += "--exclude %s " % e
 		if self.delete:
 			cmd += "--delete --delete-excluded "
 		cmd += "%s %s" % (src, dest)
-		run_shell(cmd)
+		await run_shell(cmd)
 
 
 class SyncFromTree(SyncDir):
 	# sync a full portage tree, deleting any excess files in the target dir:
 	def __init__(self, src_tree, exclude=None, delete=True):
 		if exclude is None:
 			exclude = []
 		self.src_tree = src_tree
 		SyncDir.__init__(self, src_tree, srcdir=None, destdir=None, exclude=exclude, delete=delete)
 
 	async def run(self, kit_gen):
 		await SyncDir.run(self, kit_gen)
-		kit_gen.out_tree.logTree(self.src_tree)
+		kit_gen.out_tree.log_tree(self.src_tree)
 
 
 class GenerateRepoMetadata(MergeStep):
 	def __init__(self, name, masters=None, aliases=None, priority=None):
 		self.name = name
 		self.aliases = aliases if aliases is not None else []
 		self.masters = masters if masters is not None else []
@@ -166,27 +156,27 @@
 		if globs is None:
 			globs = []
 		self.globs = globs
 
 	async def run(self, kit_gen):
 		for glob in self.globs:
 			cmd = f"find {kit_gen.out_tree.root} -name {glob} -exec rm -rf {{}} +"
-			run_shell(cmd, abort_on_failure=False)
+			await run_shell(cmd, abort_on_failure=False)
 
 
 class RemoveFiles(MergeStep):
 	def __init__(self, globs=None):
 		if globs is None:
 			globs = []
 		self.globs = globs
 
 	async def run(self, kit_gen):
 		for glob in self.globs:
 			cmd = "rm -rf %s/%s" % (kit_gen.out_tree.root, glob)
-			run_shell(cmd)
+			await run_shell(cmd)
 
 
 class CopyFiles(MergeStep):
 	"""
 	Copy regular files from source tree `srctree` to destination.
 
 	`file_map_tuples` has the format::
@@ -213,30 +203,30 @@
 				raise FileNotFoundError(f"Source file not found: {f_src_path}.")
 			f_dst_path = os.path.join(kit_gen.out_tree.root, dst_path)
 			if os.path.exists(f_dst_path):
 				os.unlink(f_dst_path)
 			parent = os.path.dirname(f_dst_path)
 			if not os.path.exists(parent):
 				os.makedirs(parent, exist_ok=True)
-			run_shell(f"cp -a {f_src_path} {f_dst_path}")
+			await run_shell(f"cp -a {f_src_path} {f_dst_path}")
 
 
 class CopyAndRename(MergeStep):
 	def __init__(self, src, dest, ren_fun):
 		self.src = src
 		self.dest = dest
 		# renaming function ... accepts source file path, and returns destination filename
 		self.ren_fun = ren_fun
 
 	async def run(self, kit_gen):
 		srcpath = os.path.join(kit_gen.out_tree.root, self.src)
 		for f in os.listdir(srcpath):
 			destfile = os.path.join(kit_gen.out_tree.root, self.dest)
 			destfile = os.path.join(destfile, self.ren_fun(f))
-			run_shell(f"cp -a {srcpath}/{f} {destfile}")
+			await run_shell(f"cp -a {srcpath}/{f} {destfile}")
 
 
 class SyncFiles(MergeStep):
 	def __init__(self, srcroot, files):
 		self.srcroot = srcroot
 		self.files = files
 		if not isinstance(files, dict):
@@ -277,15 +267,15 @@
 		files = ""
 		for fn in os.listdir(kit_gen.out_tree.root):
 			if fn[:1] == ".":
 				continue
 			if fn in self.exclude:
 				continue
 			files += " '" + fn + "'"
-		run_shell(f"cd {kit_gen.out_tree.root} && rm -rf {files[1:]}")
+		await run_shell(f"cd {kit_gen.out_tree.root} && rm -rf {files[1:]}")
 
 
 class ELTSymlinkWorkaround(MergeStep):
 	async def run(self, kit_gen):
 		dest = os.path.join(kit_gen.out_tree.root + "/eclass/ELT-patches")
 		if not os.path.lexists(dest):
 			os.makedirs(dest)
@@ -300,15 +290,15 @@
 		self.suffixfilter = suffixfilter
 		self.select = select
 		self.srctree = srctree
 		self.skip = skip
 		self.src_offset = src_offset
 
 	async def run(self, kit_gen):
-		kit_gen.out_tree.logTree(self.srctree)
+		kit_gen.out_tree.log_tree(self.srctree)
 		src = self.srctree.root
 		if self.src_offset:
 			src = os.path.join(src, self.src_offset)
 		if self.subdir:
 			src = os.path.join(src, self.subdir)
 		if not os.path.exists(src):
 			return
@@ -328,15 +318,15 @@
 					continue
 			if isinstance(self.skip, list):
 				if e in self.skip:
 					continue
 			elif isinstance(self.skip, regextype):
 				if self.skip.match(e):
 					continue
-			run_shell("cp -a %s/%s %s" % (src, e, dst))
+			await run_shell("cp -a %s/%s %s" % (src, e, dst))
 
 
 class PruneLicenses(MergeStep):
 
 	"""
 
 	This step will remove all files in licenses/ that is not actually used by any ebuild in the kit. This
@@ -384,15 +374,15 @@
 		self.select = select
 		self.srctree = srctree
 		self.branch = branch
 
 	async def run(self, kit_gen):
 		if self.branch is not None:
 			# Allow dynamic switching to different branches/commits to grab things we want:
-			self.srctree.gitCheckout(branch=self.branch)
+			self.srctree.git_checkout(branch=self.branch)
 		# Figure out what categories to process:
 		dest_cat_path = os.path.join(kit_gen.out_tree.root, "profiles/categories")
 		if os.path.exists(dest_cat_path):
 			with open(dest_cat_path, "r") as f:
 				dest_cat_set = set(f.read().splitlines())
 		else:
 			dest_cat_set = set()
@@ -406,15 +396,15 @@
 			if not os.path.isdir(src_catdir):
 				continue
 			for src_pkg in os.listdir(src_catdir):
 				dest_pkgdir = os.path.join(kit_gen.out_tree.root, cat, src_pkg)
 				if not os.path.exists(dest_pkgdir):
 					# don't need to zap as it doesn't exist
 					continue
-				run_shell("rm -rf %s" % dest_pkgdir)
+				await run_shell("rm -rf %s" % dest_pkgdir)
 
 
 class Autogen(MergeStep):
 
 	def __init__(self, srctree, ebuildloc=None, scope=None):
 		self.srctree = srctree
 		self.ebuildloc = ebuildloc
@@ -492,15 +482,15 @@
 		checks = []
 
 		if self.ebuildloc:
 			srctree_root = self.srctree.root + "/" + self.ebuildloc
 		else:
 			srctree_root = self.srctree.root
 
-		kit_gen.out_tree.logTree(self.srctree)
+		kit_gen.out_tree.log_tree(self.srctree)
 		# Figure out what categories to process:
 		src_cat_path = os.path.join(srctree_root, "profiles/categories")
 		dest_cat_path = os.path.join(kit_gen.out_tree.root, "profiles/categories")
 		if self.categories is not None:
 			# categories specified in __init__:
 			src_cat_set = set(self.categories)
 		else:
@@ -596,15 +586,15 @@
 			os.makedirs(os.path.dirname(temp_out), exist_ok=True)
 			#sys.stdout.write(f"Written to {temp_out}:\n")
 			#sys.stdout.write(script_out)
 			#sys.stdout.write("\n")
 			with open(temp_out, "w") as f:
 				f.write("#!/bin/bash\n")
 				f.write(script_out)
-			run_shell(f"/bin/bash {temp_out}")
+			await run_shell(f"/bin/bash {temp_out}")
 			os.unlink(temp_out)
 		for check in checks:
 			if not os.path.exists(check):
 				raise FileNotFoundError(
 					f"It appears that {check} was not copied successfully. Maybe missing from {self.srctree.name}?"
 				)
 
@@ -618,15 +608,15 @@
 			a = open(fpath, "r")
 			for line in a:
 				if line[0:1] == "#":
 					continue
 				sp = line.split()
 				if len(sp) >= 2:
 					prof_path = sp[1]
-					run_shell("rm -f %s/profiles/%s/deprecated" % (kit_gen.out_tree.root, prof_path))
+					await run_shell("rm -f %s/profiles/%s/deprecated" % (kit_gen.out_tree.root, prof_path))
 
 
 class RunSed(MergeStep):
 	"""
 	Run sed commands on specified files.
 
 	files: List of files.
@@ -637,23 +627,23 @@
 	def __init__(self, files, commands):
 		self.files = files
 		self.commands = commands
 
 	async def run(self, kit_gen):
 		commands = list(itertools.chain.from_iterable(("-e", command) for command in self.commands))
 		files = [os.path.join(kit_gen.out_tree.root, file) for file in self.files]
-		run_shell(["sed"] + commands + ["-i"] + files)
+		await run_shell(["sed"] + commands + ["-i"] + files)
 
 
 class Minify(MergeStep):
 	"""Minify removes ChangeLogs and shrinks Manifests."""
 
 	async def run(self, kit_gen):
-		run_shell("( cd %s && find -iname ChangeLog | xargs rm -f )" % kit_gen.out_tree.root, abort_on_failure=False)
-		run_shell("( cd %s && find -iname Manifest | xargs -i@ sed -ni '/^DIST/p' @ )" % kit_gen.out_tree.root)
+		await run_shell("( cd %s && find -iname ChangeLog | xargs rm -f )" % kit_gen.out_tree.root, abort_on_failure=False)
+		await run_shell("( cd %s && find -iname Manifest | xargs -i@ sed -ni '/^DIST/p' @ )" % kit_gen.out_tree.root)
 
 
 class GenPythonUse(MergeStep):
 	def __init__(self):
 		kit = model.release_yaml.kits["python-kit"][0]
 		pydata = kit.settings
 		out_subpath = f"funtoo/kits/python-kit/{kit.branch}"
```

### Comparing `funtoo-metatools-1.2.0/metatools/store.py` & `funtoo-metatools-1.3.0/metatools/store.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/metatools/yaml_util.py` & `funtoo-metatools-1.3.0/metatools/yaml_util.py`

 * *Files identical despite different names*

### Comparing `funtoo-metatools-1.2.0/setup.py` & `funtoo-metatools-1.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 pkgr = Packager()
 
 with open("README.rst", "r") as fh:
 	long_description = fh.read()
 
 setuptools.setup(
 	name="funtoo-metatools",
-	version="1.2.0",
+	version="1.3.0",
 	author="Daniel Robbins",
 	author_email="drobbins@funtoo.org",
 	description="Funtoo framework for auto-creation of ebuilds.",
 	long_description=long_description,
 	long_description_content_type="text/x-rst",
 	url="https://code.funtoo.org/bitbucket/users/drobbins/repos/funtoo-metatools/browse",
 	scripts=["bin/doit", "bin/merge-kits"],
@@ -28,14 +28,15 @@
 		"dict_toolbox",
 		"httpx[http2]",
 		"Jinja2 >= 3",
 		"packaging",
 		"psutil",
 		"pymongo",
 		"PyYAML",
+		"pyzmq",
 		"rich",
 		"toml",
 		"xmltodict",
 		"colorama",
 	],
 	packages=setuptools.find_packages(),
 	data_files=pkgr.generate_data_files(),
```

### Comparing `funtoo-metatools-1.2.0/setup.py.in` & `funtoo-metatools-1.3.0/setup.py.in`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 		"dict_toolbox",
 		"httpx[http2]",
 		"Jinja2 >= 3",
 		"packaging",
 		"psutil",
 		"pymongo",
 		"PyYAML",
+		"pyzmq",
 		"rich",
 		"toml",
 		"xmltodict",
 		"colorama",
 	],
 	packages=setuptools.find_packages(),
 	data_files=pkgr.generate_data_files(),
```

