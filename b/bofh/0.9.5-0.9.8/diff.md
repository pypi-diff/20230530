# Comparing `tmp/bofh-0.9.5.tar.gz` & `tmp/bofh-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bofh-0.9.5.tar", last modified: Fri Oct 30 10:46:02 2020, max compression
+gzip compressed data, was "bofh-0.9.8.tar", last modified: Thu May 25 14:12:02 2023, max compression
```

## Comparing `bofh-0.9.5.tar` & `bofh-0.9.8.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxr-x   0 andretol (128807) andretol (298784)        0 2020-10-30 10:46:02.000000 bofh-0.9.5/
-drwxrwxr-x   0 andretol (128807) andretol (298784)        0 2020-10-30 10:46:02.000000 bofh-0.9.5/bofh/
--rw-rw-r--   0 andretol (128807) andretol (298784)     2725 2020-06-10 09:08:26.000000 bofh-0.9.5/bofh/__init__.py
--rw-rw-r--   0 andretol (128807) andretol (298784)      838 2020-06-10 09:08:26.000000 bofh-0.9.5/bofh/__main__.py
--rwx------   0 andretol (128807) andretol (298784)     7196 2020-10-14 11:48:22.000000 bofh-0.9.5/bofh/cli.py
--rw-rw-r--   0 andretol (128807) andretol (298784)     5036 2020-06-10 09:08:26.000000 bofh-0.9.5/bofh/config.py
--rw-------   0 andretol (128807) andretol (298784)    11183 2020-10-20 10:04:51.000000 bofh-0.9.5/bofh/formatting.py
--rw-------   0 andretol (128807) andretol (298784)     2591 2020-10-19 06:39:04.000000 bofh-0.9.5/bofh/https.py
--rw-------   0 andretol (128807) andretol (298784)     6836 2020-10-14 11:48:22.000000 bofh-0.9.5/bofh/internal_commands.py
--rw-------   0 andretol (128807) andretol (298784)    23318 2020-10-14 11:48:22.000000 bofh-0.9.5/bofh/parser.py
--rw-------   0 andretol (128807) andretol (298784)    20649 2020-10-14 11:48:22.000000 bofh-0.9.5/bofh/proto.py
--rw-------   0 andretol (128807) andretol (298784)    11904 2020-10-14 11:48:22.000000 bofh-0.9.5/bofh/readlineui.py
--rw-rw-r--   0 andretol (128807) andretol (298784)     1212 2020-10-30 09:48:52.000000 bofh-0.9.5/bofh/version.py
-drwxrwxr-x   0 andretol (128807) andretol (298784)        0 2020-10-30 10:46:02.000000 bofh-0.9.5/bofh.egg-info/
--rw-rw-r--   0 andretol (128807) andretol (298784)     3629 2020-10-30 10:46:01.000000 bofh-0.9.5/bofh.egg-info/PKG-INFO
--rw-rw-r--   0 andretol (128807) andretol (298784)     1106 2020-10-30 10:46:02.000000 bofh-0.9.5/bofh.egg-info/SOURCES.txt
--rw-rw-r--   0 andretol (128807) andretol (298784)        1 2020-10-30 10:46:01.000000 bofh-0.9.5/bofh.egg-info/dependency_links.txt
--rw-rw-r--   0 andretol (128807) andretol (298784)       42 2020-10-30 10:46:01.000000 bofh-0.9.5/bofh.egg-info/entry_points.txt
--rw-rw-r--   0 andretol (128807) andretol (298784)       15 2020-10-30 10:46:01.000000 bofh-0.9.5/bofh.egg-info/requires.txt
--rw-rw-r--   0 andretol (128807) andretol (298784)        5 2020-10-30 10:46:01.000000 bofh-0.9.5/bofh.egg-info/top_level.txt
-drwxrwxr-x   0 andretol (128807) andretol (298784)        0 2020-10-30 10:46:02.000000 bofh-0.9.5/data/
--rw-rw-r--   0 andretol (128807) andretol (298784)     1391 2020-06-10 09:08:27.000000 bofh-0.9.5/data/cacerts.pem
-drwxrwxr-x   0 andretol (128807) andretol (298784)        0 2020-10-30 10:46:02.000000 bofh-0.9.5/docs/
-drwxrwxr-x   0 andretol (128807) andretol (298784)        0 2020-10-30 10:46:02.000000 bofh-0.9.5/docs/source/
-drwxrwxr-x   0 andretol (128807) andretol (298784)        0 2020-10-30 10:46:02.000000 bofh-0.9.5/docs/source/man/
--rw-rw-r--   0 andretol (128807) andretol (298784)     2631 2020-06-10 09:08:27.000000 bofh-0.9.5/docs/source/man/pybofh.rst
-drwxrwxr-x   0 andretol (128807) andretol (298784)        0 2020-10-30 10:46:02.000000 bofh-0.9.5/docs/source/modules/
--rw-rw-r--   0 andretol (128807) andretol (298784)       66 2020-06-10 09:08:27.000000 bofh-0.9.5/docs/source/modules/bofh.config.rst
--rw-rw-r--   0 andretol (128807) andretol (298784)       78 2020-06-10 09:08:27.000000 bofh-0.9.5/docs/source/modules/bofh.formatting.rst
--rw-rw-r--   0 andretol (128807) andretol (298784)       66 2020-06-10 09:08:27.000000 bofh-0.9.5/docs/source/modules/bofh.parser.rst
--rw-rw-r--   0 andretol (128807) andretol (298784)       90 2020-06-10 09:08:27.000000 bofh-0.9.5/docs/source/modules/bofh.proto.rst
--rw-rw-r--   0 andretol (128807) andretol (298784)      106 2020-06-10 09:08:28.000000 bofh-0.9.5/docs/source/modules/bofh.readlineui.rst
--rw-rw-r--   0 andretol (128807) andretol (298784)       45 2020-06-10 09:08:28.000000 bofh-0.9.5/docs/source/modules/bofh.rst
--rw-rw-r--   0 andretol (128807) andretol (298784)     2812 2020-06-10 09:08:28.000000 bofh-0.9.5/docs/source/modules/index.rst
--rw-rw-r--   0 andretol (128807) andretol (298784)     4390 2020-10-30 09:48:52.000000 bofh-0.9.5/docs/source/conf.py
--rw-rw-r--   0 andretol (128807) andretol (298784)     1520 2020-06-10 09:08:27.000000 bofh-0.9.5/docs/source/develop.rst
--rw-rw-r--   0 andretol (128807) andretol (298784)      721 2020-10-30 09:48:52.000000 bofh-0.9.5/docs/source/index.rst
--rw-rw-r--   0 andretol (128807) andretol (298784)     1837 2020-10-30 09:48:52.000000 bofh-0.9.5/docs/source/install.rst
--rw-rw-r--   0 andretol (128807) andretol (298784)      139 2020-10-22 12:39:38.000000 bofh-0.9.5/docs/source/intro.rst
--rw-rw-r--   0 andretol (128807) andretol (298784)      606 2020-06-10 09:08:27.000000 bofh-0.9.5/docs/Makefile
--rw-rw-r--   0 andretol (128807) andretol (298784)      541 2020-10-22 12:41:33.000000 bofh-0.9.5/docs/README.md
--rw-rw-r--   0 andretol (128807) andretol (298784)       58 2020-06-10 09:08:27.000000 bofh-0.9.5/docs/requirements.txt
-drwxrwxr-x   0 andretol (128807) andretol (298784)        0 2020-10-30 10:46:02.000000 bofh-0.9.5/examples/
--rwxrwxr-x   0 andretol (128807) andretol (298784)     1705 2020-06-10 09:08:28.000000 bofh-0.9.5/examples/change_password.py
-drwxrwxr-x   0 andretol (128807) andretol (298784)        0 2020-10-30 10:46:02.000000 bofh-0.9.5/scripts/
--rwxrwxr-x   0 andretol (128807) andretol (298784)     1001 2020-06-10 09:08:28.000000 bofh-0.9.5/scripts/bofh
-drwxrwxr-x   0 andretol (128807) andretol (298784)        0 2020-10-30 10:46:02.000000 bofh-0.9.5/tests/
--rw-rw-r--   0 andretol (128807) andretol (298784)     1767 2020-06-10 09:08:28.000000 bofh-0.9.5/tests/conftest.py
--rw-rw-r--   0 andretol (128807) andretol (298784)       34 2020-06-10 09:08:28.000000 bofh-0.9.5/tests/test_dummy.py
--rw-rw-r--   0 andretol (128807) andretol (298784)     2756 2020-06-10 09:08:28.000000 bofh-0.9.5/tests/test_formatting.py
--rw-rw-r--   0 andretol (128807) andretol (298784)      228 2020-06-10 09:08:28.000000 bofh-0.9.5/tests/test_parser_command.py
--rw-rw-r--   0 andretol (128807) andretol (298784)      780 2020-06-10 09:08:28.000000 bofh-0.9.5/tests/test_parser_lexer.py
--rw-rw-r--   0 andretol (128807) andretol (298784)      130 2020-10-30 09:48:52.000000 bofh-0.9.5/.gitignore
--rw-rw-r--   0 andretol (128807) andretol (298784)    35149 2020-06-10 09:08:26.000000 bofh-0.9.5/COPYING
--rw-rw-r--   0 andretol (128807) andretol (298784)     1452 2020-10-30 09:48:52.000000 bofh-0.9.5/Jenkinsfile
--rw-rw-r--   0 andretol (128807) andretol (298784)      477 2020-06-10 09:08:26.000000 bofh-0.9.5/Jenkinsfile-dependencies-check
--rw-rw-r--   0 andretol (128807) andretol (298784)       63 2020-06-10 09:08:26.000000 bofh-0.9.5/MANIFEST.in
--rw-rw-r--   0 andretol (128807) andretol (298784)     2017 2020-10-30 09:48:52.000000 bofh-0.9.5/README.md
--rw-------   0 andretol (128807) andretol (298784)       16 2020-10-21 12:41:27.000000 bofh-0.9.5/requirements-test.txt
--rw-rw-r--   0 andretol (128807) andretol (298784)       32 2020-06-10 09:08:28.000000 bofh-0.9.5/requirements.txt
--rwxrwxr-x   0 andretol (128807) andretol (298784)     5597 2020-10-30 09:48:52.000000 bofh-0.9.5/setup.py
--rw-------   0 andretol (128807) andretol (298784)      705 2020-10-21 12:41:27.000000 bofh-0.9.5/tox.ini
--rw-rw-r--   0 andretol (128807) andretol (298784)     3629 2020-10-30 10:46:02.000000 bofh-0.9.5/PKG-INFO
--rw-rw-r--   0 andretol (128807) andretol (298784)       38 2020-10-30 10:46:02.000000 bofh-0.9.5/setup.cfg
+drwxr-xr-x   0 fhl      (194183) fhl      (146680)        0 2023-05-25 14:12:02.256170 bofh-0.9.8/
+drwxr-xr-x   0 fhl      (194183) fhl      (146680)        0 2023-05-25 14:12:01.598335 bofh-0.9.8/.github/
+-rw-r--r--   0 fhl      (194183) fhl      (146680)      424 2023-05-25 13:50:07.000000 bofh-0.9.8/.github/CODEOWNERS
+-rw-r--r--   0 fhl      (194183) fhl      (146680)      130 2023-05-24 09:29:16.000000 bofh-0.9.8/.gitignore
+-rw-r--r--   0 fhl      (194183) fhl      (146680)    35149 2022-11-15 12:12:17.000000 bofh-0.9.8/COPYING
+-rw-r--r--   0 fhl      (194183) fhl      (146680)       63 2022-11-15 12:12:17.000000 bofh-0.9.8/MANIFEST.in
+-rw-r--r--   0 fhl      (194183) fhl      (146680)     3076 2023-05-25 14:12:02.255164 bofh-0.9.8/PKG-INFO
+-rw-r--r--   0 fhl      (194183) fhl      (146680)     2201 2023-05-25 14:07:41.000000 bofh-0.9.8/README.md
+drwxr-xr-x   0 fhl      (194183) fhl      (146680)        0 2023-05-25 14:12:01.753440 bofh-0.9.8/bofh/
+-rw-r--r--   0 fhl      (194183) fhl      (146680)     2740 2023-05-25 14:07:41.000000 bofh-0.9.8/bofh/__init__.py
+-rw-r--r--   0 fhl      (194183) fhl      (146680)      862 2023-05-25 14:07:41.000000 bofh-0.9.8/bofh/__main__.py
+-rwxr-xr-x   0 fhl      (194183) fhl      (146680)     7215 2023-05-25 14:07:41.000000 bofh-0.9.8/bofh/cli.py
+-rw-r--r--   0 fhl      (194183) fhl      (146680)     5042 2023-05-25 14:07:41.000000 bofh-0.9.8/bofh/config.py
+-rw-r--r--   0 fhl      (194183) fhl      (146680)    11202 2023-05-25 14:07:41.000000 bofh-0.9.8/bofh/formatting.py
+-rw-r--r--   0 fhl      (194183) fhl      (146680)     2610 2023-05-25 14:07:41.000000 bofh-0.9.8/bofh/https.py
+-rw-r--r--   0 fhl      (194183) fhl      (146680)     6853 2023-05-25 14:07:41.000000 bofh-0.9.8/bofh/internal_commands.py
+-rw-r--r--   0 fhl      (194183) fhl      (146680)    23337 2023-05-25 14:07:41.000000 bofh-0.9.8/bofh/parser.py
+-rw-r--r--   0 fhl      (194183) fhl      (146680)    20668 2023-05-25 14:07:41.000000 bofh-0.9.8/bofh/proto.py
+-rw-r--r--   0 fhl      (194183) fhl      (146680)    13250 2023-05-25 14:07:41.000000 bofh-0.9.8/bofh/readlineui.py
+-rw-r--r--   0 fhl      (194183) fhl      (146680)     1231 2023-05-25 14:07:41.000000 bofh-0.9.8/bofh/version.py
+drwxr-xr-x   0 fhl      (194183) fhl      (146680)        0 2023-05-25 14:12:01.844079 bofh-0.9.8/bofh.egg-info/
+-rw-r--r--   0 fhl      (194183) fhl      (146680)     3076 2023-05-25 14:12:00.000000 bofh-0.9.8/bofh.egg-info/PKG-INFO
+-rw-r--r--   0 fhl      (194183) fhl      (146680)     1082 2023-05-25 14:12:01.000000 bofh-0.9.8/bofh.egg-info/SOURCES.txt
+-rw-r--r--   0 fhl      (194183) fhl      (146680)        1 2023-05-25 14:12:00.000000 bofh-0.9.8/bofh.egg-info/dependency_links.txt
+-rw-r--r--   0 fhl      (194183) fhl      (146680)       41 2023-05-25 14:12:00.000000 bofh-0.9.8/bofh.egg-info/entry_points.txt
+-rw-r--r--   0 fhl      (194183) fhl      (146680)       15 2023-05-25 14:12:00.000000 bofh-0.9.8/bofh.egg-info/requires.txt
+-rw-r--r--   0 fhl      (194183) fhl      (146680)        5 2023-05-25 14:12:00.000000 bofh-0.9.8/bofh.egg-info/top_level.txt
+drwxr-xr-x   0 fhl      (194183) fhl      (146680)        0 2023-05-25 14:12:01.859179 bofh-0.9.8/data/
+-rw-r--r--   0 fhl      (194183) fhl      (146680)     1391 2022-11-15 12:12:18.000000 bofh-0.9.8/data/cacerts.pem
+drwxr-xr-x   0 fhl      (194183) fhl      (146680)        0 2023-05-25 14:12:01.912481 bofh-0.9.8/docs/
+-rw-r--r--   0 fhl      (194183) fhl      (146680)      606 2022-11-15 12:12:18.000000 bofh-0.9.8/docs/Makefile
+-rw-r--r--   0 fhl      (194183) fhl      (146680)      735 2023-05-25 14:07:41.000000 bofh-0.9.8/docs/README.md
+-rw-r--r--   0 fhl      (194183) fhl      (146680)      374 2023-05-24 09:29:16.000000 bofh-0.9.8/docs/requirements.txt
+drwxr-xr-x   0 fhl      (194183) fhl      (146680)        0 2023-05-25 14:12:01.984929 bofh-0.9.8/docs/source/
+-rw-r--r--   0 fhl      (194183) fhl      (146680)     4404 2023-05-25 14:07:41.000000 bofh-0.9.8/docs/source/conf.py
+-rw-r--r--   0 fhl      (194183) fhl      (146680)     2333 2023-05-25 14:07:41.000000 bofh-0.9.8/docs/source/develop.rst
+-rw-r--r--   0 fhl      (194183) fhl      (146680)      715 2023-05-25 14:07:41.000000 bofh-0.9.8/docs/source/index.rst
+-rw-r--r--   0 fhl      (194183) fhl      (146680)     1671 2023-05-25 14:07:41.000000 bofh-0.9.8/docs/source/install.rst
+-rw-r--r--   0 fhl      (194183) fhl      (146680)      136 2023-05-25 14:07:41.000000 bofh-0.9.8/docs/source/intro.rst
+drwxr-xr-x   0 fhl      (194183) fhl      (146680)        0 2023-05-25 14:12:02.006119 bofh-0.9.8/docs/source/man/
+-rw-r--r--   0 fhl      (194183) fhl      (146680)     2632 2023-05-25 14:07:41.000000 bofh-0.9.8/docs/source/man/pybofh.rst
+drwxr-xr-x   0 fhl      (194183) fhl      (146680)        0 2023-05-25 14:12:02.136208 bofh-0.9.8/docs/source/modules/
+-rw-r--r--   0 fhl      (194183) fhl      (146680)       66 2022-11-15 12:12:18.000000 bofh-0.9.8/docs/source/modules/bofh.config.rst
+-rw-r--r--   0 fhl      (194183) fhl      (146680)     2938 2023-05-25 14:07:41.000000 bofh-0.9.8/docs/source/modules/bofh.formatting.rst
+-rw-r--r--   0 fhl      (194183) fhl      (146680)       66 2022-11-15 12:12:18.000000 bofh-0.9.8/docs/source/modules/bofh.parser.rst
+-rw-r--r--   0 fhl      (194183) fhl      (146680)       90 2022-11-15 12:12:18.000000 bofh-0.9.8/docs/source/modules/bofh.proto.rst
+-rw-r--r--   0 fhl      (194183) fhl      (146680)      106 2022-11-15 12:12:18.000000 bofh-0.9.8/docs/source/modules/bofh.readlineui.rst
+-rw-r--r--   0 fhl      (194183) fhl      (146680)       45 2022-11-15 12:12:18.000000 bofh-0.9.8/docs/source/modules/bofh.rst
+-rw-r--r--   0 fhl      (194183) fhl      (146680)     2890 2023-05-25 14:07:41.000000 bofh-0.9.8/docs/source/modules/index.rst
+drwxr-xr-x   0 fhl      (194183) fhl      (146680)        0 2023-05-25 14:12:02.143277 bofh-0.9.8/examples/
+-rwxr-xr-x   0 fhl      (194183) fhl      (146680)     1789 2023-05-25 14:07:41.000000 bofh-0.9.8/examples/change_password.py
+-rw-r--r--   0 fhl      (194183) fhl      (146680)       16 2023-05-24 09:29:16.000000 bofh-0.9.8/requirements-test.txt
+-rw-r--r--   0 fhl      (194183) fhl      (146680)       32 2022-11-15 12:12:18.000000 bofh-0.9.8/requirements.txt
+drwxr-xr-x   0 fhl      (194183) fhl      (146680)        0 2023-05-25 14:12:02.149332 bofh-0.9.8/scripts/
+-rwxr-xr-x   0 fhl      (194183) fhl      (146680)      953 2023-05-25 14:07:41.000000 bofh-0.9.8/scripts/bofh
+-rw-r--r--   0 fhl      (194183) fhl      (146680)       38 2023-05-25 14:12:02.258187 bofh-0.9.8/setup.cfg
+-rwxr-xr-x   0 fhl      (194183) fhl      (146680)     6378 2023-05-25 14:07:41.000000 bofh-0.9.8/setup.py
+drwxr-xr-x   0 fhl      (194183) fhl      (146680)        0 2023-05-25 14:12:02.233036 bofh-0.9.8/tests/
+-rw-r--r--   0 fhl      (194183) fhl      (146680)     1767 2022-11-15 12:12:18.000000 bofh-0.9.8/tests/conftest.py
+-rw-r--r--   0 fhl      (194183) fhl      (146680)       34 2022-11-15 12:12:18.000000 bofh-0.9.8/tests/test_dummy.py
+-rw-r--r--   0 fhl      (194183) fhl      (146680)     2756 2022-11-15 12:12:18.000000 bofh-0.9.8/tests/test_formatting.py
+-rw-r--r--   0 fhl      (194183) fhl      (146680)      228 2022-11-15 12:12:18.000000 bofh-0.9.8/tests/test_parser_command.py
+-rw-r--r--   0 fhl      (194183) fhl      (146680)      780 2022-11-15 12:12:18.000000 bofh-0.9.8/tests/test_parser_lexer.py
+-rw-r--r--   0 fhl      (194183) fhl      (146680)      705 2023-05-24 09:29:16.000000 bofh-0.9.8/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bofh-0.9.5/bofh/__init__.py` & `bofh-0.9.8/bofh/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright 2010-2018 University of Oslo, Norway
+# This file is part of bofh.
+# Copyright (C) 2010-2023 University of Oslo, Norway
 #
-# This file is part of pybofh.
-#
-# pybofh is free software; you can redistribute it and/or modify it
-# under the terms of the GNU General Public License as published by
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# pybofh is distributed in the hope that it will be useful, but
-# WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-# General Public License for more details.
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with pybofh; if not, see <https://www.gnu.org/licenses/>.
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 The bofh library
 ----------------
 
 The bofh library is an XMLRPC client library for Cerebrum, and the main
-component of the pybofh distribution.
+component of the bofh distribution.
 
-This library can be used to automate common use cases of the pybofh cli script.
+This library can be used to automate common use cases of the bofh cli script.
 
 Typical usage would look something like:
 
 .. code:: python
 
     import bofh
     import getpass
```

### Comparing `bofh-0.9.5/bofh/__main__.py` & `bofh-0.9.8/bofh/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright 2018 University of Oslo, Norway
+# This file is part of bofh.
+# Copyright (C) 2018-2023 University of Oslo, Norway
 #
-# This file is part of pybofh.
-#
-# pybofh is free software; you can redistribute it and/or modify it
-# under the terms of the GNU General Public License as published by
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# pybofh is distributed in the hope that it will be useful, but
-# WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-# General Public License for more details.
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with pybofh; if not, see <https://www.gnu.org/licenses/>.
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """ python -m bofh """
 import bofh.cli
 
 
 if __name__ == '__main__':
     # it really should be...
     bofh.cli.main()
```

### Comparing `bofh-0.9.5/bofh/cli.py` & `bofh-0.9.8/bofh/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright 2010-2018 University of Oslo, Norway
+# This file is part of bofh.
+# Copyright (C) 2010-2023 University of Oslo, Norway
 #
-# This file is part of pybofh.
-#
-# pybofh is free software; you can redistribute it and/or modify it
-# under the terms of the GNU General Public License as published by
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# pybofh is distributed in the hope that it will be useful, but
-# WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-# General Public License for more details.
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with pybofh; if not, see <https://www.gnu.org/licenses/>.
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 An interactive Cerebrum XMLRPC cli client.
 """
 from __future__ import print_function, unicode_literals
 
 import argparse
 import getpass
```

### Comparing `bofh-0.9.5/bofh/config.py` & `bofh-0.9.8/bofh/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright 2018 University of Oslo, Norway
+# This file is part of bofh.
+# Copyright (C) 2018-2023 University of Oslo, Norway
 #
-# This file is part of pybofh.
-#
-# pybofh is free software; you can redistribute it and/or modify it
-# under the terms of the GNU General Public License as published by
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# pybofh is distributed in the hope that it will be useful, but
-# WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-# General Public License for more details.
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with pybofh; if not, see <https://www.gnu.org/licenses/>.
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
-This module provides configuration and defaults for pybofh.
+This module provides configuration and defaults for bofh.
 
 Currently, all confguration here is related to loading configurable resources,
 and specifying defaults for items that are intended to be configurable in the
 future.
 
 Configuration files and resources
 ---------------------------------
@@ -30,17 +29,17 @@
 .. py:data:: DEFAULT_CONFIG_PATH
 
     1. ~/.config/pybofh/
     2. /etc/pybofh/
     3. <prefix>/local/share/pybofh
     4. <prefix>/share/pybofh
 
-The last location is where pybofh installs default configuration files and
+The last location is where bofh installs default configuration files and
 resources.  Currently, the only file loaded from these locations are the CA
-certificate bundle used by pybofh.
+certificate bundle used by bofh.
 
 
 Environment variables
 ---------------------
 
 .. py:data:: PYBOFH_DEFAULT_URL
 
@@ -81,18 +80,18 @@
 # TODO: Replace default location with package_data for simplicity across
 #       platforms?
 DEFAULT_CONFIG_PATH = tuple((
     # Read from standard locations?
     os.path.expanduser('~/.config/pybofh'),
     '/etc/pybofh',
     # python installs data/cacerts.pem to <prefix>/share/pybofh/
-    os.path.join(sys.prefix, 'local', 'share', 'pybofh'),
-    os.path.join(sys.prefix, 'share', 'pybofh'),
+    os.path.join(sys.prefix, 'local/share/pybofh'),
+    os.path.join(sys.prefix, 'share/pybofh'),
     # At last, look in ../data/ in case we're developing
-    os.path.join(os.path.dirname(__file__), '..', 'data'),
+    os.path.join(os.path.dirname(__file__), '../data'),
 ))
 
 # Default XMLRPC server url
 # TODO: Change this to https://localhost/ and put this url in a config.
 DEFAULT_URL = 'https://cerebrum-uio.uio.no:8000/'
 
 # Default logging format
```

### Comparing `bofh-0.9.5/bofh/formatting.py` & `bofh-0.9.8/bofh/formatting.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright 2010-2019 University of Oslo, Norway
+# This file is part of bofh.
+# Copyright (C) 2010-2023 University of Oslo, Norway
 #
-# This file is part of pybofh.
-#
-# pybofh is free software; you can redistribute it and/or modify it
-# under the terms of the GNU General Public License as published by
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# pybofh is distributed in the hope that it will be useful, but
-# WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-# General Public License for more details.
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with pybofh; if not, see <https://www.gnu.org/licenses/>.
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 This module consists of formatting utils for displaying responses from the
 XMLRPC server in a human readable form.
 
 Most notably is the parsing and formatting according to the hints
 (format suggestions) given by the server.
```

### Comparing `bofh-0.9.5/bofh/https.py` & `bofh-0.9.8/bofh/https.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright 2014-2019 University of Oslo, Norway
+# This file is part of bofh.
+# Copyright (C) 2014-2023 University of Oslo, Norway
 #
-# This file is part of pybofh.
-#
-# pybofh is free software; you can redistribute it and/or modify it
-# under the terms of the GNU General Public License as published by
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# pybofh is distributed in the hope that it will be useful, but
-# WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-# General Public License for more details.
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with pybofh; if not, see <https://www.gnu.org/licenses/>.
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """Patches for xmlrpc that adds timeout."""
 from __future__ import absolute_import, unicode_literals
 # TODO: Rename file to transport.py?
 
 import logging
 import socket
```

### Comparing `bofh-0.9.5/bofh/internal_commands.py` & `bofh-0.9.8/bofh/internal_commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright 2010-2018 University of Oslo, Norway
+# This file is part of bofh.
+# Copyright (C) 2010-2023 University of Oslo, Norway
 #
-# This file is part of pybofh.
-#
-# pybofh is free software; you can redistribute it and/or modify it
-# under the terms of the GNU General Public License as published by
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# pybofh is distributed in the hope that it will be useful, but
-# WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-# General Public License for more details.
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with pybofh; if not, see <https://www.gnu.org/licenses/>.
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
-Implementation of internal pybofh commands.
+Implementation of internal bofh commands.
 
 Internal commands are commands that appear as regular commands in the
 interactive bofh client, but aren't sent (directly) to the XMLRPC server.
 
 Typically these functions would be called through the eval
 (:meth:`bofh.parser.Command.eval`) method of the object returned from
 :func:`bofh.parser.parse`.
```

### Comparing `bofh-0.9.5/bofh/parser.py` & `bofh-0.9.8/bofh/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright 2010-2018 University of Oslo, Norway
+# This file is part of bofh.
+# Copyright (C) 2010-2023 University of Oslo, Norway
 #
-# This file is part of pybofh.
-#
-# pybofh is free software; you can redistribute it and/or modify it
-# under the terms of the GNU General Public License as published by
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# pybofh is distributed in the hope that it will be useful, but
-# WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-# General Public License for more details.
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with pybofh; if not, see <https://www.gnu.org/licenses/>.
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 Implementation of the input command parsing in bofh.
 
 This module implements the input parsing of command strings entered into the
 interactive python client.
 
 Parsing input commands are neccessary in order to e.g. provide command
```

### Comparing `bofh-0.9.5/bofh/proto.py` & `bofh-0.9.8/bofh/proto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright 2010-2018 University of Oslo, Norway
+# This file is part of bofh.
+# Copyright (C) 2010-2023 University of Oslo, Norway
 #
-# This file is part of pybofh.
-#
-# pybofh is free software; you can redistribute it and/or modify it
-# under the terms of the GNU General Public License as published by
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# pybofh is distributed in the hope that it will be useful, but
-# WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-# General Public License for more details.
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with pybofh; if not, see <https://www.gnu.org/licenses/>.
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 Module to communicate with a bofh server.
 """
 from __future__ import absolute_import, unicode_literals
 
 import logging
 import socket
```

### Comparing `bofh-0.9.5/bofh/readlineui.py` & `bofh-0.9.8/bofh/readlineui.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright 2010-2018 University of Oslo, Norway
+# This file is part of bofh.
+# Copyright (C) 2010-2023 University of Oslo, Norway
 #
-# This file is part of pybofh.
-#
-# pybofh is free software; you can redistribute it and/or modify it
-# under the terms of the GNU General Public License as published by
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# pybofh is distributed in the hope that it will be useful, but
-# WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-# General Public License for more details.
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with pybofh; if not, see <https://www.gnu.org/licenses/>.
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 Interactive bofh client.
 
 This module implements a REPL for implementing an interactive bofh client, and
 readline command completion.
 """
 from __future__ import print_function, unicode_literals
+import re
 
 import getpass
 import locale
 import logging
 import readline
 
 import six
@@ -213,16 +213,18 @@
             print(mapstr)
         # get input from user
         val = inputfunc(_prompt).strip()
         # Lines read at this stage, are params to a command.
         # We remove them from the history.
         # Note that we only do this for non-empty lines! If we do it for all
         # lines, we would remove history that should not be removed ;)
-        if val:
-            rlh_to_delete = readline.get_current_history_length()
+        # Only delete if there are history items
+        history_length = readline.get_current_history_length()
+        if val and history_length > 0:
+            rlh_to_delete = history_length
             readline.remove_history_item(rlh_to_delete-1)
 
         # only let empty value pass if default or optional
         if not val and not default:
             if optional:
                 return None
             continue
@@ -235,25 +237,47 @@
                 print("Sorry, no help available")
             else:
                 print(help)
         else:
             # if mapping, return the corresponding key,
             # else just return what the user typed.
             if map:
-                try:
-                    i = int(val)
-                    if i < 1:
-                        raise IndexError("Negative")
-                    return map[i-1]
-                except ValueError:
-                    print("Please type a number matching one of the items")
-                except IndexError:
-                    print("The item you selected does not exist")
-            else:
-                return val
+                selections = None
+                if val.isdigit():  # Single digit
+                    try:
+                        i = int(val)
+                    except ValueError:
+                        print("Please type a number matching one of the items")
+                    if i <= 0:
+                        return IndexError("Negative")
+                    try:
+                        return map[i - 1]  # -1 because human input is off by +1
+                    except IndexError:
+                        print("The item you selected does not exist")
+                elif re.search(r"\d+-\d+", val):    # range
+                    values = val.split("-")
+                    try:
+                        start = int(values[0]) - 1
+                        end = int(values[1]) - 1
+                        selections = map[start:end]
+                    except ValueError:
+                        print("Please specify a range, eg. 1-3")
+                    except IndexError:
+                        print("The item you selected does not exist")
+                    return selections
+                elif re.search(r"(\d+,)+\d", val):  # comma separated
+                    values = [elem.strip() for elem in val.split(',')]
+                    try:
+                        selections = [map[int(elem) - 1] for elem in values]
+                    except ValueError:
+                        print("Please specify a list separated by commas, eg. 1,2,3")
+                    except IndexError:
+                        print("The item you selected does not exist")
+                    return selections
+            return val
 
 
 def repl(bofh, charset=None, prompt=None):
     """
     Read Eval Print Loop
 
     The function of this is to
```

### Comparing `bofh-0.9.5/bofh/version.py` & `bofh-0.9.8/bofh/version.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright 2010-2018 University of Oslo, Norway
+# This file is part of bofh.
+# Copyright (C) 2010-2023 University of Oslo, Norway
 #
-# This file is part of pybofh.
-#
-# pybofh is free software; you can redistribute it and/or modify it
-# under the terms of the GNU General Public License as published by
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# pybofh is distributed in the hope that it will be useful, but
-# WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-# General Public License for more details.
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with pybofh; if not, see <https://www.gnu.org/licenses/>.
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """ bofh versioning utils """
 import os
 import pkg_resources
 
 
 DISTRIBUTION_NAME = 'bofh'
```

### Comparing `bofh-0.9.5/bofh.egg-info/SOURCES.txt` & `bofh-0.9.8/bofh.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 .gitignore
 COPYING
-Jenkinsfile
-Jenkinsfile-dependencies-check
 MANIFEST.in
 README.md
 requirements-test.txt
 requirements.txt
 setup.py
 tox.ini
+.github/CODEOWNERS
 bofh/__init__.py
 bofh/__main__.py
 bofh/cli.py
 bofh/config.py
 bofh/formatting.py
 bofh/https.py
 bofh/internal_commands.py
```

### Comparing `bofh-0.9.5/data/cacerts.pem` & `bofh-0.9.8/data/cacerts.pem`

 * *Files identical despite different names*

### Comparing `bofh-0.9.5/docs/source/man/pybofh.rst` & `bofh-0.9.8/docs/source/man/pybofh.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 pybofh
-======
+=======
 
 Synopsis
 --------
 
 **pybofh** [*options*]
```

### Comparing `bofh-0.9.5/docs/source/modules/index.rst` & `bofh-0.9.8/docs/source/modules/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -3,64 +3,61 @@
 
 TODO: Some of this should be moved to the source code as module docstrings, etc.
 TODO: Some of this should be moved to the documentation of a specific module.
 
 
 Usage
 -----
-
+A short example that connects to a bofh server, performs login, and runs the
+``user_info`` bofh command with argument ``foo``:
 ::
 
    import bofh
    from getpass import getuser, getpass
 
    # Get a client by connecting to bofhd
    url = 'https://example.org:8000'
-   cacert = '/path/to/ca.pem'
-   client = bofh.connect(url=url, cert=cacert)
+   client = bofh.connect(url=url)
 
    # You'll need to authenticate to access restricted commands
    client.login(getuser(), getpass())
 
    # Call commands on the client object
    try:
        client.user.info('foo')
        client.run_command('user_info', 'foo')
    finally:
        client.logout()
 
 
 ``run_command`` vs ``<group>.<command>``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
 The ``run_command`` command returns de-serialized, structured data, as returned by
 the XML-RPC server. This is probably what you want to use:
 
 ::
 
    >>> client.run_command('group_list', 'foo')
    [{'expired': None, 'type': u'account', 'id': 42, 'name': u'foo'}]
 
 
 The generated ``<group>.<command>`` attributes calls
 ``run_command('<group>_<command>')``, and formats the structured output
 according to suggestions provided by the XML-RPC server. This is really only
 useful if you're building a REPL/interactive client:
-
 ::
 
-   >>> print client.group.list('foo')
+   >>> print(client.group.list('foo'))
    Type       Name       Expired
    account    foo        <not set>
 
 
 Errors
 ~~~~~~
-Any error from the XML-RPC server is raised as an exception in pybofh:
-
+Any error from the XML-RPC server is raised as an exception in bofh:
 ::
 
    >>> client.user.info('does_not_exist')
    Traceback (most recent call last):
      File "<stdin>", line 1, in <module>
      File "bofh/proto.py", line 211, in __call__
        ret = self._bofh.run_command(self._fullname, *args)
@@ -71,15 +68,14 @@
      File "bofh/proto.py", line 459, in run_command
        raise BofhError(msg)
    bofh.proto.BofhError: Could not find Account with name=does_not_exist
 
 
 Timeouts
 ~~~~~~~~
-
 The ``bofh.connect()`` method accepts a ``timeout`` argument. This can be used
 to abort from long-running command executions. This however, does not imply that
 the command is aborted on the server side, it will run until completion. If the
 response of the command is essential, do not set a timeout.
 
 When a timeout occurs, ``socket.timeout`` will be raised.
```

### Comparing `bofh-0.9.5/docs/source/conf.py` & `bofh-0.9.8/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
           else str(INITIAL_YEAR)),
     who=author,
 )
 
 
 # version hack
 # from pkg_resources import get_distribution
-import bofh
+import bofh  # noqa: E402
 release = bofh.__version__
 # The short X.Y version
 # version = ''
 version = '.'.join(release.split('.')[:2])
 # The full version, including alpha/beta/rc tags
 # release = ''
 
@@ -61,15 +61,15 @@
 master_doc = 'index'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path .
 exclude_patterns = []
 
 # The name of the Pygments (syntax highlighting) style to use.
```

### Comparing `bofh-0.9.5/docs/source/index.rst` & `bofh-0.9.8/docs/source/index.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-pybofh documentation
-====================
-
-*pybofh*, short for *brukerorganisering for hvermannsen*, is a `Cerebrum`_
+bofh documentation
+===================
+*bofh*, short for *brukerorganisering for hvermannsen*, is a `Cerebrum`_
 administration tool.
 
 It is an interactive XML/RPC CLI client for a ``Cerebrum.modules.bofhd``
 server.  It is unlikely you want to use this software unless you know
 what Cerebrum is.
 
 .. toctree::
```

### Comparing `bofh-0.9.5/docs/Makefile` & `bofh-0.9.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bofh-0.9.5/examples/change_password.py` & `bofh-0.9.8/examples/change_password.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,59 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-
-# Copyright 2010 University of Oslo, Norway
 #
-# This file is part of PyBofh.
+# This file is part of bofh.
+# Copyright (C) 2010-2023 University of Oslo, Norway
 #
-# PyBofh is free software; you can redistribute it and/or modify it
-# under the terms of the GNU General Public License as published by
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PyBofh is distributed in the hope that it will be useful, but
-# WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-# General Public License for more details.
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PyBofh; if not, write to the Free Software Foundation,
-# Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307, USA.
-
-import getpass, bofh.version, locale
-import bofh.proto
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+from __future__ import (
+    absolute_import,
+    division,
+    print_function,
+    unicode_literals,
+)
+import getpass
 import sys
+import textwrap
 
-print (u"""This is PyBofh version %s
+import bofh.proto
+import bofh.version
 
-Copyright (c) 2010 University of Oslo, Norway
-This is free software; see the source for copying conditions. There is NO
-warranty, not even for MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.""" 
-% bofh.version.version).encode(
-        locale.getpreferredencoding())
+header = textwrap.dedent(
+    """
+    This is bofh version {}
+
+    Copyright (C) 2010-2023 University of Oslo, Norway
+    This is free software; see the source for copying conditions. There is NO
+    warranty, not even for MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+    """
+).strip().format(bofh.version.version)
+print(header)
 
 try:
     bofhcom = bofh.connect(getpass.getuser(), getpass.getpass())
-except bofh.proto.BofhError, e:
-    print e.args[0]
+except bofh.proto.BofhError as e:
+    print(e.args[0], file=sys.stderr)
     sys.exit(1)
 
-# print bofhcom.motd
-
-newpass = getpass.getpass(u"New password: ")
+newpass = getpass.getpass("New password: ")
 
-if newpass != getpass.getpass(u"Repeat: "):
-    print u"Passwords doesn't match"
+if newpass != getpass.getpass("Repeat: "):
+    print("Passwords doesn't match")
 else:
     try:
-        print bofhcom.user.password(getpass.getuser(), newpass)
-        print u"Password changed".encode(locale.getpreferredencoding())
-    except bofh.proto.BofhError, e:
-        print e.message
+        print(bofhcom.user.password(getpass.getuser(), newpass))
+        print("Password changed")
+    except bofh.proto.BofhError as e:
+        print(e.message, file=sys.stderr)
         sys.exit(1)
```

### Comparing `bofh-0.9.5/scripts/bofh` & `bofh-0.9.8/scripts/bofh`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-
-# Copyright 2010-2018 University of Oslo, Norway
 #
-# This file is part of PyBofh.
+# This file is part of bofh.
+# Copyright (C) 2010-2023 University of Oslo, Norway
 #
-# PyBofh is free software; you can redistribute it and/or modify it
-# under the terms of the GNU General Public License as published by
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PyBofh is distributed in the hope that it will be useful, but
-# WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-# General Public License for more details.
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PyBofh; if not, write to the Free Software Foundation,
-# Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307, USA.
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """ legacy bofh script
 
-This script is kept for legacy reasons (e.g. running pybofh without running
+This script is kept for legacy reasons (e.g. running bofh without running
 setup.py install).
 """
 import bofh.cli
 
 
 if __name__ == '__main__':
     bofh.cli.main()
```

### Comparing `bofh-0.9.5/tests/conftest.py` & `bofh-0.9.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bofh-0.9.5/tests/test_formatting.py` & `bofh-0.9.8/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `bofh-0.9.5/tests/test_parser_lexer.py` & `bofh-0.9.8/tests/test_parser_lexer.py`

 * *Files identical despite different names*

### Comparing `bofh-0.9.5/COPYING` & `bofh-0.9.8/COPYING`

 * *Files identical despite different names*

### Comparing `bofh-0.9.5/README.md` & `bofh-0.9.8/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -8,48 +8,47 @@
 `Cerebrum.modules.bofhd` server.  It is unlikely you want to use this
 software unless you know what Cerebrum is.
 
 
 Install
 -------
 
-bofh is implemented in Python and supports Python runtimes 2.7 (>= 2.7.9,
->= RHEL7 2.7.5), and 3.6 or newer.
+bofh is implemented in Python and supports Python runtimes 2.7
+(>= 2.7.9, >= RHEL7 2.7.5), and 3.6 or newer.
 
 If you are on RHEL we recommend that you install the bofh RPM package
 from the university package repository:
 
-	# dnf install pybofh
+    # dnf install python3-bofh
 
 On other systems we recommend installing from the official Python package
 index (PyPI) into a [virtualenv]:
 
-	% virtualenv ~/venv
-	% source ~/venv/bin/activate
-	(venv) % pip install bofh
+    % virtualenv ~/venv
+    % source ~/venv/bin/activate
+    (venv) % pip install bofh
 
 
 Use
 ---
 
-	pybofh --help
-	python -m bofh --help
+    pybofh --help
+    python -m bofh --help
 
 
 Module usage
 ------------
 
 ```python
 import bofh
 from getpass import getuser, getpass
 
 # Get a client by connecting to bofhd
 url = 'https://example.org:8000'
-cacert = '/path/to/ca.pem'
-client = bofh.connect(url=url, cert=cacert)
+client = bofh.connect(url=url)
 
 # You'll need to authenticate to access restricted commands
 client.login(getuser(), getpass())
 
 # Call commands on the client object
 try:
     # formatted output
@@ -66,26 +65,27 @@
 -------------
 
 You'll have to build the bofh documentation yourself (for now).
 
 Documentation is built using *sphinx*, and build requirements are
 specified in the [docs/requirements.txt] file.
 
-	% python setup.py build_sphinx -b html
-	% cd build/sphinx/html
-	% python3 -m http.server
+    % python setup.py build_sphinx -b html
+    % cd build/sphinx/html
+    % python3 -m http.server
 
 Then go to http://localhost:8000/.
 
-There is also also a troff man-page for the bofh script, which can be
+There is also also a troff man-page for the pybofh script, which can be
 built with:
 
-	% python setup.py build_sphinx -b man
-	% man ./build/sphinx/man/bofh.1
+    % python setup.py build_sphinx -b man
+    % man ./build/sphinx/man/pybofh.1
 
 For other documentation formats, see [docs/README.md] and [docs/Makefile].
 
 
-[docs/Makefile]: docs/Makefile
-[docs/README.md]: docs/README.md
-[docs/requirements.txt]: docs/requirements.txt
+[Cerebrum]: https://github.com/unioslo/cerebrum
+[docs/Makefile]: https://github.com/unioslo/pybofh/blob/master/docs/Makefile
+[docs/README.md]: https://github.com/unioslo/pybofh/blob/master/docs/README.md
+[docs/requirements.txt]: https://github.com/unioslo/pybofh/blob/master/requirements.txt
 [virtualenv]: https://virtualenv.pypa.io/
```

### Comparing `bofh-0.9.5/setup.py` & `bofh-0.9.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-
-# Copyright 2010-2020 University of Oslo
 #
-# This file is part of pybofh.
+# This file is part of bofh.
+# Copyright (C) 2010-2023 University of Oslo, Norway
 #
-# PyBofh is free software; you can redistribute it and/or modify it
-# under the terms of the GNU General Public License as published by
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# PyBofh is distributed in the hope that it will be useful, but
-# WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
-# General Public License for more details.
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with PyBofh; if not, write to the Free Software Foundation,
-# Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307, USA.
-
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from __future__ import print_function
 
 import codecs
+import errno
+import glob
 import io
 import os
 import shutil
 import sys
 
 import setuptools
 from setuptools import Command
-from setuptools.command.test import test as TestCommand
+from distutils.command.clean import clean as clean_command
+from setuptools.command.test import test as test_command
 
 
 here = os.path.abspath(os.path.dirname(__file__))
 dist = os.path.join(here, "dist")
 
 
 def mock_mbcs_windows():
@@ -66,19 +66,35 @@
 
 
 def get_packages():
     """ List of (sub)packages to install. """
     return setuptools.find_packages('.', include=('bofh', 'bofh.*'))
 
 
+class Clean(clean_command):
+    def run(self):
+        super(Clean, self).run()
+        rm(".cache/")
+        rm(".eggs/")
+        rm(".pytest_cache/")
+        rm(".tox/")
+        rm("__pycache__/")
+        rm("*.egg-info/")
+        rm("dist/")
+        rm("docs/build/")
+        rm("junit-*.xml")
+        rm("**/*.pyc")
+
+
 class Publish(Command):
     """Support publishing to PyPI via setup.py."""
 
     description = "Build and publish package."
-    user_options = [("repository=", None, "target package index (default: pypi)")]
+    user_options = [("repository=", None,
+                     "target package index (default: pypi)")]
 
     def initialize_options(self):
         self.repository = "pypi"
 
     def finalize_options(self):
         pass
 
@@ -92,23 +108,23 @@
 
         print("uploading to %s via twine" % self.repository)
         execl("twine", "upload", "--repository", self.repository, "dist/*")
 
         # TODO(andretol): consider git tagging here
 
 
-class Tox(TestCommand):
+class Tox(test_command):
     user_options = [('tox-args=', None, "Arguments to pass to tox")]
 
     def initialize_options(self):
-        TestCommand.initialize_options(self)
+        super(Tox, self).initialize_options()
         self.tox_args = ''
 
     def finalize_options(self):
-        TestCommand.finalize_options(self)
+        super(Tox, self).finalize_options()
         self.test_args = []
         self.test_suite = True
 
     def run_tests(self):
         import tox
         errno = tox.cmdline(args=self.tox_args.split())
         sys.exit(errno)
@@ -162,20 +178,34 @@
             'Programming Language :: Python :: 3.8',
             'Programming Language :: Python :: 3.9',
             'Topic :: Software Development :: Libraries',
             'Topic :: System :: Systems Administration',
         ],
         keywords='cerebrum bofh xmlrpc client',
         cmdclass={
+            'clean': Clean,
             'test': Tox,
             'publish': Publish,
         },
     )
 
 
+def rm(pattern):
+    """Deletes files and directories using a glob pattern, not unlike rm(1)."""
+    for path in glob.glob(pattern):
+        try:
+            if os.path.isdir(path):
+                shutil.rmtree(path)
+            else:
+                os.remove(path)
+        except OSError as e:
+            if e.errno != errno.ENOENT:
+                raise
+
+
 def execl(path, *args):
     exit_code = os.system("%s %s" % (path, " ".join(args)))
     if exit_code != 0:
         fatal("%s ended with exit code: %s" % (path, exit_code))
 
 
 def fatal(*args):
```

### Comparing `bofh-0.9.5/tox.ini` & `bofh-0.9.8/tox.ini`

 * *Files identical despite different names*

