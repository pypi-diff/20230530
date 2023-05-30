# Comparing `tmp/bofh-0.9.7.tar.gz` & `tmp/bofh-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bofh-0.9.7.tar", last modified: Wed May 24 09:21:51 2023, max compression
+gzip compressed data, was "bofh-0.9.8.tar", last modified: Thu May 25 14:12:02 2023, max compression
```

## Comparing `bofh-0.9.7.tar` & `bofh-0.9.8.tar`

### file list

```diff
@@ -1,62 +1,64 @@
-drwxr-xr-x   0 fhl      (194183) fhl      (146680)        0 2023-05-24 09:21:51.072494 bofh-0.9.7/
--rw-r--r--   0 fhl      (194183) fhl      (146680)      130 2023-01-16 16:02:46.000000 bofh-0.9.7/.gitignore
--rw-r--r--   0 fhl      (194183) fhl      (146680)    35149 2022-11-15 12:12:17.000000 bofh-0.9.7/COPYING
--rw-r--r--   0 fhl      (194183) fhl      (146680)       63 2022-11-15 12:12:17.000000 bofh-0.9.7/MANIFEST.in
--rw-r--r--   0 fhl      (194183) fhl      (146680)     3073 2023-05-24 09:21:51.070484 bofh-0.9.7/PKG-INFO
--rw-r--r--   0 fhl      (194183) fhl      (146680)     2198 2023-01-16 16:02:46.000000 bofh-0.9.7/README.md
-drwxr-xr-x   0 fhl      (194183) fhl      (146680)        0 2023-05-24 09:21:50.762836 bofh-0.9.7/bofh/
--rw-r--r--   0 fhl      (194183) fhl      (146680)     2725 2022-11-15 12:12:17.000000 bofh-0.9.7/bofh/__init__.py
--rw-r--r--   0 fhl      (194183) fhl      (146680)      838 2022-11-15 12:12:18.000000 bofh-0.9.7/bofh/__main__.py
--rwxr-xr-x   0 fhl      (194183) fhl      (146680)     7196 2022-11-15 12:12:18.000000 bofh-0.9.7/bofh/cli.py
--rw-r--r--   0 fhl      (194183) fhl      (146680)     5036 2022-11-15 12:12:18.000000 bofh-0.9.7/bofh/config.py
--rw-r--r--   0 fhl      (194183) fhl      (146680)    11183 2022-11-15 12:12:18.000000 bofh-0.9.7/bofh/formatting.py
--rw-r--r--   0 fhl      (194183) fhl      (146680)     2591 2022-11-15 12:12:18.000000 bofh-0.9.7/bofh/https.py
--rw-r--r--   0 fhl      (194183) fhl      (146680)     6836 2023-01-16 16:02:20.000000 bofh-0.9.7/bofh/internal_commands.py
--rw-r--r--   0 fhl      (194183) fhl      (146680)    23318 2022-11-15 12:12:18.000000 bofh-0.9.7/bofh/parser.py
--rw-r--r--   0 fhl      (194183) fhl      (146680)    20649 2023-01-16 16:02:46.000000 bofh-0.9.7/bofh/proto.py
--rw-r--r--   0 fhl      (194183) fhl      (146680)    13231 2023-01-16 16:02:46.000000 bofh-0.9.7/bofh/readlineui.py
--rw-r--r--   0 fhl      (194183) fhl      (146680)     1212 2023-01-16 16:02:46.000000 bofh-0.9.7/bofh/version.py
-drwxr-xr-x   0 fhl      (194183) fhl      (146680)        0 2023-05-24 09:21:50.822319 bofh-0.9.7/bofh.egg-info/
--rw-r--r--   0 fhl      (194183) fhl      (146680)     3073 2023-05-24 09:21:49.000000 bofh-0.9.7/bofh.egg-info/PKG-INFO
--rw-r--r--   0 fhl      (194183) fhl      (146680)     1063 2023-05-24 09:21:50.000000 bofh-0.9.7/bofh.egg-info/SOURCES.txt
--rw-r--r--   0 fhl      (194183) fhl      (146680)        1 2023-05-24 09:21:49.000000 bofh-0.9.7/bofh.egg-info/dependency_links.txt
--rw-r--r--   0 fhl      (194183) fhl      (146680)       41 2023-05-24 09:21:49.000000 bofh-0.9.7/bofh.egg-info/entry_points.txt
--rw-r--r--   0 fhl      (194183) fhl      (146680)       15 2023-05-24 09:21:49.000000 bofh-0.9.7/bofh.egg-info/requires.txt
--rw-r--r--   0 fhl      (194183) fhl      (146680)        5 2023-05-24 09:21:49.000000 bofh-0.9.7/bofh.egg-info/top_level.txt
-drwxr-xr-x   0 fhl      (194183) fhl      (146680)        0 2023-05-24 09:21:50.833371 bofh-0.9.7/data/
--rw-r--r--   0 fhl      (194183) fhl      (146680)     1391 2022-11-15 12:12:18.000000 bofh-0.9.7/data/cacerts.pem
-drwxr-xr-x   0 fhl      (194183) fhl      (146680)        0 2023-05-24 09:21:50.854495 bofh-0.9.7/docs/
--rw-r--r--   0 fhl      (194183) fhl      (146680)      606 2022-11-15 12:12:18.000000 bofh-0.9.7/docs/Makefile
--rw-r--r--   0 fhl      (194183) fhl      (146680)      541 2022-11-15 12:12:18.000000 bofh-0.9.7/docs/README.md
--rw-r--r--   0 fhl      (194183) fhl      (146680)      374 2023-03-13 10:04:06.000000 bofh-0.9.7/docs/requirements.txt
-drwxr-xr-x   0 fhl      (194183) fhl      (146680)        0 2023-05-24 09:21:50.944958 bofh-0.9.7/docs/source/
--rw-r--r--   0 fhl      (194183) fhl      (146680)     4390 2023-01-16 16:02:46.000000 bofh-0.9.7/docs/source/conf.py
--rw-r--r--   0 fhl      (194183) fhl      (146680)     2320 2023-01-16 16:02:46.000000 bofh-0.9.7/docs/source/develop.rst
--rw-r--r--   0 fhl      (194183) fhl      (146680)      721 2023-01-16 16:02:46.000000 bofh-0.9.7/docs/source/index.rst
--rw-r--r--   0 fhl      (194183) fhl      (146680)     1837 2023-01-16 16:02:46.000000 bofh-0.9.7/docs/source/install.rst
--rw-r--r--   0 fhl      (194183) fhl      (146680)      139 2022-11-15 12:12:18.000000 bofh-0.9.7/docs/source/intro.rst
-drwxr-xr-x   0 fhl      (194183) fhl      (146680)        0 2023-05-24 09:21:50.951985 bofh-0.9.7/docs/source/man/
--rw-r--r--   0 fhl      (194183) fhl      (146680)     2631 2022-11-15 12:12:18.000000 bofh-0.9.7/docs/source/man/pybofh.rst
-drwxr-xr-x   0 fhl      (194183) fhl      (146680)        0 2023-05-24 09:21:51.002195 bofh-0.9.7/docs/source/modules/
--rw-r--r--   0 fhl      (194183) fhl      (146680)       66 2022-11-15 12:12:18.000000 bofh-0.9.7/docs/source/modules/bofh.config.rst
--rw-r--r--   0 fhl      (194183) fhl      (146680)     2941 2023-01-16 16:02:46.000000 bofh-0.9.7/docs/source/modules/bofh.formatting.rst
--rw-r--r--   0 fhl      (194183) fhl      (146680)       66 2022-11-15 12:12:18.000000 bofh-0.9.7/docs/source/modules/bofh.parser.rst
--rw-r--r--   0 fhl      (194183) fhl      (146680)       90 2022-11-15 12:12:18.000000 bofh-0.9.7/docs/source/modules/bofh.proto.rst
--rw-r--r--   0 fhl      (194183) fhl      (146680)      106 2022-11-15 12:12:18.000000 bofh-0.9.7/docs/source/modules/bofh.readlineui.rst
--rw-r--r--   0 fhl      (194183) fhl      (146680)       45 2022-11-15 12:12:18.000000 bofh-0.9.7/docs/source/modules/bofh.rst
--rw-r--r--   0 fhl      (194183) fhl      (146680)     2812 2022-11-15 12:12:18.000000 bofh-0.9.7/docs/source/modules/index.rst
-drwxr-xr-x   0 fhl      (194183) fhl      (146680)        0 2023-05-24 09:21:51.013254 bofh-0.9.7/examples/
--rwxr-xr-x   0 fhl      (194183) fhl      (146680)     1705 2022-11-15 12:12:18.000000 bofh-0.9.7/examples/change_password.py
--rw-r--r--   0 fhl      (194183) fhl      (146680)       16 2023-01-16 16:02:46.000000 bofh-0.9.7/requirements-test.txt
--rw-r--r--   0 fhl      (194183) fhl      (146680)       32 2022-11-15 12:12:18.000000 bofh-0.9.7/requirements.txt
-drwxr-xr-x   0 fhl      (194183) fhl      (146680)        0 2023-05-24 09:21:51.021283 bofh-0.9.7/scripts/
--rwxr-xr-x   0 fhl      (194183) fhl      (146680)     1001 2022-11-15 12:12:18.000000 bofh-0.9.7/scripts/bofh
--rw-r--r--   0 fhl      (194183) fhl      (146680)       38 2023-05-24 09:21:51.074501 bofh-0.9.7/setup.cfg
--rwxr-xr-x   0 fhl      (194183) fhl      (146680)     6388 2023-01-16 16:02:46.000000 bofh-0.9.7/setup.py
-drwxr-xr-x   0 fhl      (194183) fhl      (146680)        0 2023-05-24 09:21:51.059439 bofh-0.9.7/tests/
--rw-r--r--   0 fhl      (194183) fhl      (146680)     1767 2022-11-15 12:12:18.000000 bofh-0.9.7/tests/conftest.py
--rw-r--r--   0 fhl      (194183) fhl      (146680)       34 2022-11-15 12:12:18.000000 bofh-0.9.7/tests/test_dummy.py
--rw-r--r--   0 fhl      (194183) fhl      (146680)     2756 2022-11-15 12:12:18.000000 bofh-0.9.7/tests/test_formatting.py
--rw-r--r--   0 fhl      (194183) fhl      (146680)      228 2022-11-15 12:12:18.000000 bofh-0.9.7/tests/test_parser_command.py
--rw-r--r--   0 fhl      (194183) fhl      (146680)      780 2022-11-15 12:12:18.000000 bofh-0.9.7/tests/test_parser_lexer.py
--rw-r--r--   0 fhl      (194183) fhl      (146680)      705 2023-01-16 16:02:46.000000 bofh-0.9.7/tox.ini
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

### Comparing `bofh-0.9.7/COPYING` & `bofh-0.9.8/COPYING`

 * *Files identical despite different names*

### Comparing `bofh-0.9.7/PKG-INFO` & `bofh-0.9.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bofh
-Version: 0.9.7
+Version: 0.9.8
 Summary: Cerebrum bofh client
 Home-page: https://github.com/unioslo/pybofh
 Author: USIT, University of Oslo
 Author-email: bnt-int@usit.uio.no
 License: GPLv3
 Keywords: cerebrum bofh xmlrpc client
 Classifier: Development Status :: 4 - Beta
@@ -37,42 +37,41 @@
 
 bofh is implemented in Python and supports Python runtimes 2.7
 (>= 2.7.9, >= RHEL7 2.7.5), and 3.6 or newer.
 
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
@@ -89,25 +88,25 @@
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
 
 
 [Cerebrum]: https://github.com/unioslo/cerebrum
 [docs/Makefile]: https://github.com/unioslo/pybofh/blob/master/docs/Makefile
 [docs/README.md]: https://github.com/unioslo/pybofh/blob/master/docs/README.md
```

### Comparing `bofh-0.9.7/README.md` & `bofh-0.9.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -14,42 +14,41 @@
 
 bofh is implemented in Python and supports Python runtimes 2.7
 (>= 2.7.9, >= RHEL7 2.7.5), and 3.6 or newer.
 
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
@@ -66,25 +65,25 @@
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
 
 
 [Cerebrum]: https://github.com/unioslo/cerebrum
 [docs/Makefile]: https://github.com/unioslo/pybofh/blob/master/docs/Makefile
 [docs/README.md]: https://github.com/unioslo/pybofh/blob/master/docs/README.md
```

### Comparing `bofh-0.9.7/bofh/__init__.py` & `bofh-0.9.8/bofh/__init__.py`

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

### Comparing `bofh-0.9.7/bofh/__main__.py` & `bofh-0.9.8/bofh/__main__.py`

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

### Comparing `bofh-0.9.7/bofh/cli.py` & `bofh-0.9.8/bofh/cli.py`

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

### Comparing `bofh-0.9.7/bofh/config.py` & `bofh-0.9.8/bofh/config.py`

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

### Comparing `bofh-0.9.7/bofh/formatting.py` & `bofh-0.9.8/bofh/formatting.py`

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

### Comparing `bofh-0.9.7/bofh/https.py` & `bofh-0.9.8/bofh/https.py`

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

### Comparing `bofh-0.9.7/bofh/internal_commands.py` & `bofh-0.9.8/bofh/internal_commands.py`

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

### Comparing `bofh-0.9.7/bofh/parser.py` & `bofh-0.9.8/bofh/parser.py`

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

### Comparing `bofh-0.9.7/bofh/proto.py` & `bofh-0.9.8/bofh/proto.py`

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

### Comparing `bofh-0.9.7/bofh/readlineui.py` & `bofh-0.9.8/bofh/readlineui.py`

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
 Interactive bofh client.
 
 This module implements a REPL for implementing an interactive bofh client, and
 readline command completion.
 """
 from __future__ import print_function, unicode_literals
```

### Comparing `bofh-0.9.7/bofh/version.py` & `bofh-0.9.8/bofh/version.py`

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

### Comparing `bofh-0.9.7/bofh.egg-info/PKG-INFO` & `bofh-0.9.8/bofh.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bofh
-Version: 0.9.7
+Version: 0.9.8
 Summary: Cerebrum bofh client
 Home-page: https://github.com/unioslo/pybofh
 Author: USIT, University of Oslo
 Author-email: bnt-int@usit.uio.no
 License: GPLv3
 Keywords: cerebrum bofh xmlrpc client
 Classifier: Development Status :: 4 - Beta
@@ -37,42 +37,41 @@
 
 bofh is implemented in Python and supports Python runtimes 2.7
 (>= 2.7.9, >= RHEL7 2.7.5), and 3.6 or newer.
 
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
@@ -89,25 +88,25 @@
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
 
 
 [Cerebrum]: https://github.com/unioslo/cerebrum
 [docs/Makefile]: https://github.com/unioslo/pybofh/blob/master/docs/Makefile
 [docs/README.md]: https://github.com/unioslo/pybofh/blob/master/docs/README.md
```

### Comparing `bofh-0.9.7/bofh.egg-info/SOURCES.txt` & `bofh-0.9.8/bofh.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 COPYING
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

### Comparing `bofh-0.9.7/data/cacerts.pem` & `bofh-0.9.8/data/cacerts.pem`

 * *Files identical despite different names*

### Comparing `bofh-0.9.7/docs/Makefile` & `bofh-0.9.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bofh-0.9.7/docs/source/conf.py` & `bofh-0.9.8/docs/source/conf.py`

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

### Comparing `bofh-0.9.7/docs/source/develop.rst` & `bofh-0.9.8/docs/source/develop.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,86 +1,85 @@
 .. highlight:: bash
 
-Developing pybofh
-=================
+Developing bofh
+===============
 
 Environment
 -----------
-
 Install bofh into a `virtualenv`_ using `pip`_ to test your ongoing
 changes::
 
         % virtualenv ~/venv
         % source ~/venv/bin/activate
         % pip install -e .
 
 
 Tests
 -----
-
 Unit tests live under the ``tests/`` directory and are written using the
 `pytest`_ testing framework.  The tests are typically invoked through
 `tox`_ to ensure compatibility with supported Python runtimes.
 
 The following are all equal ways to run all the tests on all supported
 configurations, and presupposes that you have the necessary Python
 runtimes installed::
 
-        % ./setup.py test
+        % python setup.py test
         % tox
         % python -m tox
 
 Tests may also be invoked directly with `pytest`_::
 
         % pytest
         % python -m pytest
 
 
 Code style
 ----------
-
 Code style is not strictly enforced, but some general advice applies:
 
 * Write pretty code
 * Never use tab indents in Python code
 * Follow PEPs to the best of your ability (`PEP-8`_, `PEP-257`_)
 * Docstrings should work with `sphinx`_
 
 Apply all the linters.  The author recommends running ``flake8`` with
 plugins: ``naming``, ``pycodestyle``, ``pyflakes``.
 
 
 Releasing
 ---------
-
 To prepare a new release of bofh you should first ensure all tests are
-passing on all target Python runtimes::
+passing on all target Python runtimes:
+::
 
-        % ./setup.py test
+        % python setup.py test
 
 After you have ensured there are no uncommitted changes in the repository,
 you can go ahead and tag the release with the desired version number.
-The package version number is derived from this tag, so pick it wisely::
+The package version number is derived from this tag, so pick it wisely:
+::
 
         % git tag -a vX.Y.Z
 
-First we publish the source code as so::
+First we publish the source code as so:
+::
 
         % git push
         % git push --tags
 
-The final step is to release bofh to `PyPI`_::
+The final step is to release bofh to `PyPI`_
+::
 
         % git checkout vX.Y.Z
-        % ./setup.py publish
+        % python setup.py publish
 
 
 Contribution guidelines
 -----------------------
-
 TODO: Make a ``CONTRIBUTE.rst`` in the root, and include?
 
 
 .. References
 .. ----------
 .. _flake-8: http://flake8.pycqa.org/
 .. _pep-257: https://www.python.org/dev/peps/pep-0257/
```

### Comparing `bofh-0.9.7/docs/source/index.rst` & `bofh-0.9.8/docs/source/index.rst`

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

### Comparing `bofh-0.9.7/docs/source/man/pybofh.rst` & `bofh-0.9.8/docs/source/man/pybofh.rst`

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

### Comparing `bofh-0.9.7/docs/source/modules/bofh.formatting.rst` & `bofh-0.9.8/docs/source/modules/bofh.formatting.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 bofh.formatting
 ===============
 
 The formatting module consists of utilities for displaying responses from the
 XMLRPC server in a human readable form.
 
-Most notably is the parsing and formatting according to the hints (`format
-suggestions`_) given by the server.
+Most notably is the parsing and formatting according to the hints (format
+suggestions) given by the server.
 
 Not all commands will have format suggestions. An XMLRPC command will either:
 
 - Not use format suggestions and return a pre-formatted string
 - Use format suggestions and return a dictionary or list of dictionaries.
 
 For commands with format suggestions, the formatting class
```

### Comparing `bofh-0.9.7/docs/source/modules/index.rst` & `bofh-0.9.8/docs/source/modules/index.rst`

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

### Comparing `bofh-0.9.7/examples/change_password.py` & `bofh-0.9.8/examples/change_password.py`

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

### Comparing `bofh-0.9.7/scripts/bofh` & `bofh-0.9.8/scripts/bofh`

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

### Comparing `bofh-0.9.7/setup.py` & `bofh-0.9.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,39 @@
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
 import errno
 import glob
 import io
 import os
 import shutil
 import sys
 
 import setuptools
 from setuptools import Command
-from distutils.command.clean import clean as CleanCommand
-from setuptools.command.test import test as TestCommand
+from distutils.command.clean import clean as clean_command
+from setuptools.command.test import test as test_command
 
 
 here = os.path.abspath(os.path.dirname(__file__))
 dist = os.path.join(here, "dist")
 
 
 def mock_mbcs_windows():
@@ -69,17 +66,17 @@
 
 
 def get_packages():
     """ List of (sub)packages to install. """
     return setuptools.find_packages('.', include=('bofh', 'bofh.*'))
 
 
-class Clean(CleanCommand):
+class Clean(clean_command):
     def run(self):
-        CleanCommand.run(self)
+        super(Clean, self).run()
         rm(".cache/")
         rm(".eggs/")
         rm(".pytest_cache/")
         rm(".tox/")
         rm("__pycache__/")
         rm("*.egg-info/")
         rm("dist/")
@@ -88,15 +85,16 @@
         rm("**/*.pyc")
 
 
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
 
@@ -110,23 +108,23 @@
 
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
```

### Comparing `bofh-0.9.7/tests/conftest.py` & `bofh-0.9.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bofh-0.9.7/tests/test_formatting.py` & `bofh-0.9.8/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `bofh-0.9.7/tests/test_parser_lexer.py` & `bofh-0.9.8/tests/test_parser_lexer.py`

 * *Files identical despite different names*

### Comparing `bofh-0.9.7/tox.ini` & `bofh-0.9.8/tox.ini`

 * *Files identical despite different names*

