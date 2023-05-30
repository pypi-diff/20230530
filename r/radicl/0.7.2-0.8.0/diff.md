# Comparing `tmp/radicl-0.7.2.tar.gz` & `tmp/radicl-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radicl-0.7.2.tar", last modified: Fri Mar  3 06:45:33 2023, max compression
+gzip compressed data, was "radicl-0.8.0.tar", last modified: Tue May 30 21:04:14 2023, max compression
```

## Comparing `radicl-0.7.2.tar` & `radicl-0.8.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxr-x   0 micah     (1000) micah     (1000)        0 2023-03-03 06:45:33.579023 radicl-0.7.2/
--rw-rw-r--   0 micah     (1000) micah     (1000)     1507 2020-09-29 12:34:37.000000 radicl-0.7.2/LICENSE
--rw-rw-r--   0 micah     (1000) micah     (1000)      308 2020-09-29 12:34:37.000000 radicl-0.7.2/MANIFEST.in
--rw-rw-r--   0 micah     (1000) micah     (1000)     4296 2023-03-03 06:45:33.579023 radicl-0.7.2/PKG-INFO
--rw-rw-r--   0 micah     (1000) micah     (1000)     1114 2023-02-24 03:48:37.000000 radicl-0.7.2/README.rst
-drwxrwxr-x   0 micah     (1000) micah     (1000)        0 2023-03-03 06:45:33.575023 radicl-0.7.2/docs/
--rw-rw-r--   0 micah     (1000) micah     (1000)      607 2020-09-29 12:34:37.000000 radicl-0.7.2/docs/Makefile
-drwxrwxr-x   0 micah     (1000) micah     (1000)        0 2023-03-03 06:45:33.571023 radicl-0.7.2/docs/_build/
-drwxrwxr-x   0 micah     (1000) micah     (1000)        0 2023-03-03 06:45:33.571023 radicl-0.7.2/docs/_build/html/
-drwxrwxr-x   0 micah     (1000) micah     (1000)        0 2023-03-03 06:45:33.575023 radicl-0.7.2/docs/_build/html/_images/
--rw-rw-r--   0 micah     (1000) micah     (1000)    47196 2023-02-24 03:48:37.000000 radicl-0.7.2/docs/_build/html/_images/windows_python_installer.png
-drwxrwxr-x   0 micah     (1000) micah     (1000)        0 2023-03-03 06:45:33.575023 radicl-0.7.2/docs/_build/html/_static/
--rw-rw-r--   0 micah     (1000) micah     (1000)      286 2023-01-26 22:34:11.000000 radicl-0.7.2/docs/_build/html/_static/file.png
--rw-rw-r--   0 micah     (1000) micah     (1000)       90 2023-01-26 22:34:11.000000 radicl-0.7.2/docs/_build/html/_static/minus.png
--rw-rw-r--   0 micah     (1000) micah     (1000)       90 2023-01-26 22:34:11.000000 radicl-0.7.2/docs/_build/html/_static/plus.png
--rw-rw-r--   0 micah     (1000) micah     (1000)      136 2021-11-30 13:51:01.000000 radicl-0.7.2/docs/api.rst
--rw-rw-r--   0 micah     (1000) micah     (1000)      184 2020-09-29 12:34:37.000000 radicl-0.7.2/docs/authors.rst
--rwxrwxr-x   0 micah     (1000) micah     (1000)     4901 2022-01-29 13:57:26.000000 radicl-0.7.2/docs/conf.py
--rw-rw-r--   0 micah     (1000) micah     (1000)     3490 2021-11-30 16:52:59.000000 radicl-0.7.2/docs/contributing.rst
--rw-rw-r--   0 micah     (1000) micah     (1000)     2485 2023-02-24 03:48:37.000000 radicl-0.7.2/docs/history.rst
-drwxrwxr-x   0 micah     (1000) micah     (1000)        0 2023-03-03 06:45:33.575023 radicl-0.7.2/docs/images/
--rw-rw-r--   0 micah     (1000) micah     (1000)    47196 2023-02-24 03:48:37.000000 radicl-0.7.2/docs/images/windows_python_installer.png
--rw-rw-r--   0 micah     (1000) micah     (1000)      299 2021-11-30 13:51:01.000000 radicl-0.7.2/docs/index.rst
--rw-rw-r--   0 micah     (1000) micah     (1000)     4120 2023-02-26 21:10:22.000000 radicl-0.7.2/docs/installation.rst
--rw-rw-r--   0 micah     (1000) micah     (1000)      768 2020-09-29 12:34:37.000000 radicl-0.7.2/docs/make.bat
--rw-rw-r--   0 micah     (1000) micah     (1000)       55 2023-02-24 04:08:36.000000 radicl-0.7.2/docs/modules.rst
--rw-rw-r--   0 micah     (1000) micah     (1000)     1609 2023-02-24 04:08:36.000000 radicl-0.7.2/docs/radicl.rst
--rw-rw-r--   0 micah     (1000) micah     (1000)       27 2020-09-29 12:34:37.000000 radicl-0.7.2/docs/readme.rst
--rw-rw-r--   0 micah     (1000) micah     (1000)     3063 2023-02-24 03:48:37.000000 radicl-0.7.2/docs/usage.rst
-drwxrwxr-x   0 micah     (1000) micah     (1000)        0 2023-03-03 06:45:33.575023 radicl-0.7.2/radicl/
--rw-rw-r--   0 micah     (1000) micah     (1000)      169 2023-03-03 06:45:20.000000 radicl-0.7.2/radicl/__init__.py
--rw-rw-r--   0 micah     (1000) micah     (1000)    31970 2023-02-24 03:48:37.000000 radicl-0.7.2/radicl/api.py
--rw-rw-r--   0 micah     (1000) micah     (1000)     1137 2023-02-18 07:38:32.000000 radicl-0.7.2/radicl/calibrate.py
--rw-rw-r--   0 micah     (1000) micah     (1000)     1555 2023-02-24 03:48:37.000000 radicl-0.7.2/radicl/cli.py
--rw-rw-r--   0 micah     (1000) micah     (1000)     4864 2023-03-03 06:44:41.000000 radicl-0.7.2/radicl/com.py
--rw-rw-r--   0 micah     (1000) micah     (1000)     1074 2023-02-24 03:48:37.000000 radicl-0.7.2/radicl/commands.py
--rw-rw-r--   0 micah     (1000) micah     (1000)     1784 2023-03-03 06:44:41.000000 radicl-0.7.2/radicl/gps.py
--rw-rw-r--   0 micah     (1000) micah     (1000)     6244 2023-02-26 21:10:25.000000 radicl-0.7.2/radicl/high_resolution.py
--rw-rw-r--   0 micah     (1000) micah     (1000)    22971 2023-02-24 03:48:37.000000 radicl-0.7.2/radicl/interface.py
--rw-rw-r--   0 micah     (1000) micah     (1000)    13300 2023-02-24 03:48:37.000000 radicl-0.7.2/radicl/plotting.py
--rw-rw-r--   0 micah     (1000) micah     (1000)    34396 2023-02-24 03:48:37.000000 radicl-0.7.2/radicl/probe.py
--rw-rw-r--   0 micah     (1000) micah     (1000)     6195 2023-02-24 03:48:37.000000 radicl-0.7.2/radicl/ui_tools.py
--rw-rw-r--   0 micah     (1000) micah     (1000)    17428 2023-02-18 07:38:32.000000 radicl-0.7.2/radicl/update.py
-drwxrwxr-x   0 micah     (1000) micah     (1000)        0 2023-03-03 06:45:33.579023 radicl-0.7.2/radicl.egg-info/
--rw-rw-r--   0 micah     (1000) micah     (1000)     4296 2023-03-03 06:45:33.000000 radicl-0.7.2/radicl.egg-info/PKG-INFO
--rw-rw-r--   0 micah     (1000) micah     (1000)     1224 2023-03-03 06:45:33.000000 radicl-0.7.2/radicl.egg-info/SOURCES.txt
--rw-rw-r--   0 micah     (1000) micah     (1000)        1 2023-03-03 06:45:33.000000 radicl-0.7.2/radicl.egg-info/dependency_links.txt
--rw-rw-r--   0 micah     (1000) micah     (1000)      163 2023-03-03 06:45:33.000000 radicl-0.7.2/radicl.egg-info/entry_points.txt
--rw-rw-r--   0 micah     (1000) micah     (1000)        1 2023-03-03 06:45:33.000000 radicl-0.7.2/radicl.egg-info/not-zip-safe
--rw-rw-r--   0 micah     (1000) micah     (1000)      232 2023-03-03 06:45:33.000000 radicl-0.7.2/radicl.egg-info/requires.txt
--rw-rw-r--   0 micah     (1000) micah     (1000)        7 2023-03-03 06:45:33.000000 radicl-0.7.2/radicl.egg-info/top_level.txt
--rw-rw-r--   0 micah     (1000) micah     (1000)      124 2021-11-30 13:51:01.000000 radicl-0.7.2/requirements_dev.txt
--rw-rw-r--   0 micah     (1000) micah     (1000)       38 2023-03-03 06:45:33.579023 radicl-0.7.2/setup.cfg
--rw-rw-r--   0 micah     (1000) micah     (1000)     1782 2023-03-03 06:45:20.000000 radicl-0.7.2/setup.py
-drwxrwxr-x   0 micah     (1000) micah     (1000)        0 2023-03-03 06:45:33.579023 radicl-0.7.2/tests/
--rw-rw-r--   0 micah     (1000) micah     (1000)     2679 2023-02-26 21:10:25.000000 radicl-0.7.2/tests/__init__.py
--rw-rw-r--   0 micah     (1000) micah     (1000)      619 2023-02-24 03:48:37.000000 radicl-0.7.2/tests/conftest.py
-drwxrwxr-x   0 micah     (1000) micah     (1000)        0 2023-03-03 06:45:33.579023 radicl-0.7.2/tests/connected/
--rw-rw-r--   0 micah     (1000) micah     (1000)      133 2023-02-26 21:10:25.000000 radicl-0.7.2/tests/connected/__init__.py
--rw-rw-r--   0 micah     (1000) micah     (1000)      863 2023-02-24 03:48:37.000000 radicl-0.7.2/tests/connected/test_connected_api.py
--rw-rw-r--   0 micah     (1000) micah     (1000)      370 2023-02-26 21:10:25.000000 radicl-0.7.2/tests/connected/test_connected_gps.py
--rw-rw-r--   0 micah     (1000) micah     (1000)     4016 2023-02-26 21:10:25.000000 radicl-0.7.2/tests/connected/test_connected_probe.py
--rw-rw-r--   0 micah     (1000) micah     (1000)     1237 2023-02-24 03:48:37.000000 radicl-0.7.2/tests/test_api.py
--rw-rw-r--   0 micah     (1000) micah     (1000)     2946 2023-03-03 06:44:41.000000 radicl-0.7.2/tests/test_com.py
--rw-rw-r--   0 micah     (1000) micah     (1000)     1356 2023-02-26 21:10:25.000000 radicl-0.7.2/tests/test_gps.py
--rw-rw-r--   0 micah     (1000) micah     (1000)      566 2023-02-24 03:48:37.000000 radicl-0.7.2/tests/test_high_resolution.py
--rw-rw-r--   0 micah     (1000) micah     (1000)     1563 2023-02-24 03:48:37.000000 radicl-0.7.2/tests/test_interface.py
--rw-rw-r--   0 micah     (1000) micah     (1000)      985 2023-02-24 03:48:37.000000 radicl-0.7.2/tests/test_ui_tools.py
+drwxrwxr-x   0 micah     (1000) micah     (1000)        0 2023-05-30 21:04:14.945704 radicl-0.8.0/
+-rw-rw-r--   0 micah     (1000) micah     (1000)     1507 2020-09-29 12:34:37.000000 radicl-0.8.0/LICENSE
+-rw-rw-r--   0 micah     (1000) micah     (1000)      308 2020-09-29 12:34:37.000000 radicl-0.8.0/MANIFEST.in
+-rw-rw-r--   0 micah     (1000) micah     (1000)     4395 2023-05-30 21:04:14.945704 radicl-0.8.0/PKG-INFO
+-rw-rw-r--   0 micah     (1000) micah     (1000)     1090 2023-05-30 21:03:14.000000 radicl-0.8.0/README.rst
+drwxrwxr-x   0 micah     (1000) micah     (1000)        0 2023-05-30 21:04:14.941704 radicl-0.8.0/docs/
+-rw-rw-r--   0 micah     (1000) micah     (1000)      607 2020-09-29 12:34:37.000000 radicl-0.8.0/docs/Makefile
+drwxrwxr-x   0 micah     (1000) micah     (1000)        0 2023-05-30 21:04:14.937704 radicl-0.8.0/docs/_build/
+drwxrwxr-x   0 micah     (1000) micah     (1000)        0 2023-05-30 21:04:14.937704 radicl-0.8.0/docs/_build/html/
+drwxrwxr-x   0 micah     (1000) micah     (1000)        0 2023-05-30 21:04:14.941704 radicl-0.8.0/docs/_build/html/_images/
+-rw-rw-r--   0 micah     (1000) micah     (1000)    47196 2023-02-24 03:48:37.000000 radicl-0.8.0/docs/_build/html/_images/windows_python_installer.png
+drwxrwxr-x   0 micah     (1000) micah     (1000)        0 2023-05-30 21:04:14.941704 radicl-0.8.0/docs/_build/html/_static/
+-rw-rw-r--   0 micah     (1000) micah     (1000)      286 2023-01-26 22:34:11.000000 radicl-0.8.0/docs/_build/html/_static/file.png
+-rw-rw-r--   0 micah     (1000) micah     (1000)       90 2023-01-26 22:34:11.000000 radicl-0.8.0/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 micah     (1000) micah     (1000)       90 2023-01-26 22:34:11.000000 radicl-0.8.0/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 micah     (1000) micah     (1000)      136 2021-11-30 13:51:01.000000 radicl-0.8.0/docs/api.rst
+-rw-rw-r--   0 micah     (1000) micah     (1000)      184 2020-09-29 12:34:37.000000 radicl-0.8.0/docs/authors.rst
+-rwxrwxr-x   0 micah     (1000) micah     (1000)     4901 2022-01-29 13:57:26.000000 radicl-0.8.0/docs/conf.py
+-rw-rw-r--   0 micah     (1000) micah     (1000)     3490 2021-11-30 16:52:59.000000 radicl-0.8.0/docs/contributing.rst
+-rw-rw-r--   0 micah     (1000) micah     (1000)     2608 2023-05-30 21:02:17.000000 radicl-0.8.0/docs/history.rst
+drwxrwxr-x   0 micah     (1000) micah     (1000)        0 2023-05-30 21:04:14.941704 radicl-0.8.0/docs/images/
+-rw-rw-r--   0 micah     (1000) micah     (1000)    47196 2023-02-24 03:48:37.000000 radicl-0.8.0/docs/images/windows_python_installer.png
+-rw-rw-r--   0 micah     (1000) micah     (1000)      299 2021-11-30 13:51:01.000000 radicl-0.8.0/docs/index.rst
+-rw-rw-r--   0 micah     (1000) micah     (1000)     4120 2023-02-26 21:10:22.000000 radicl-0.8.0/docs/installation.rst
+-rw-rw-r--   0 micah     (1000) micah     (1000)      768 2020-09-29 12:34:37.000000 radicl-0.8.0/docs/make.bat
+-rw-rw-r--   0 micah     (1000) micah     (1000)       55 2023-02-24 04:08:36.000000 radicl-0.8.0/docs/modules.rst
+-rw-rw-r--   0 micah     (1000) micah     (1000)     1609 2023-02-24 04:08:36.000000 radicl-0.8.0/docs/radicl.rst
+-rw-rw-r--   0 micah     (1000) micah     (1000)       27 2020-09-29 12:34:37.000000 radicl-0.8.0/docs/readme.rst
+-rw-rw-r--   0 micah     (1000) micah     (1000)     3063 2023-02-24 03:48:37.000000 radicl-0.8.0/docs/usage.rst
+drwxrwxr-x   0 micah     (1000) micah     (1000)        0 2023-05-30 21:04:14.945704 radicl-0.8.0/radicl/
+-rw-rw-r--   0 micah     (1000) micah     (1000)      169 2023-05-30 21:03:45.000000 radicl-0.8.0/radicl/__init__.py
+-rw-rw-r--   0 micah     (1000) micah     (1000)    31970 2023-02-24 03:48:37.000000 radicl-0.8.0/radicl/api.py
+-rw-rw-r--   0 micah     (1000) micah     (1000)     1137 2023-02-18 07:38:32.000000 radicl-0.8.0/radicl/calibrate.py
+-rw-rw-r--   0 micah     (1000) micah     (1000)     1555 2023-02-24 03:48:37.000000 radicl-0.8.0/radicl/cli.py
+-rw-rw-r--   0 micah     (1000) micah     (1000)     4864 2023-03-03 06:44:41.000000 radicl-0.8.0/radicl/com.py
+-rw-rw-r--   0 micah     (1000) micah     (1000)     1074 2023-02-24 03:48:37.000000 radicl-0.8.0/radicl/commands.py
+-rw-rw-r--   0 micah     (1000) micah     (1000)     1784 2023-03-03 06:44:41.000000 radicl-0.8.0/radicl/gps.py
+-rw-rw-r--   0 micah     (1000) micah     (1000)     6244 2023-02-26 21:10:25.000000 radicl-0.8.0/radicl/high_resolution.py
+-rw-rw-r--   0 micah     (1000) micah     (1000)    22971 2023-02-24 03:48:37.000000 radicl-0.8.0/radicl/interface.py
+-rw-rw-r--   0 micah     (1000) micah     (1000)     9729 2023-05-30 21:01:07.000000 radicl-0.8.0/radicl/plotting.py
+-rw-rw-r--   0 micah     (1000) micah     (1000)    34396 2023-02-24 03:48:37.000000 radicl-0.8.0/radicl/probe.py
+-rw-rw-r--   0 micah     (1000) micah     (1000)     6195 2023-02-24 03:48:37.000000 radicl-0.8.0/radicl/ui_tools.py
+-rw-rw-r--   0 micah     (1000) micah     (1000)    17428 2023-02-18 07:38:32.000000 radicl-0.8.0/radicl/update.py
+drwxrwxr-x   0 micah     (1000) micah     (1000)        0 2023-05-30 21:04:14.945704 radicl-0.8.0/radicl.egg-info/
+-rw-rw-r--   0 micah     (1000) micah     (1000)     4395 2023-05-30 21:04:14.000000 radicl-0.8.0/radicl.egg-info/PKG-INFO
+-rw-rw-r--   0 micah     (1000) micah     (1000)     1224 2023-05-30 21:04:14.000000 radicl-0.8.0/radicl.egg-info/SOURCES.txt
+-rw-rw-r--   0 micah     (1000) micah     (1000)        1 2023-05-30 21:04:14.000000 radicl-0.8.0/radicl.egg-info/dependency_links.txt
+-rw-rw-r--   0 micah     (1000) micah     (1000)      163 2023-05-30 21:04:14.000000 radicl-0.8.0/radicl.egg-info/entry_points.txt
+-rw-rw-r--   0 micah     (1000) micah     (1000)        1 2023-05-30 21:04:14.000000 radicl-0.8.0/radicl.egg-info/not-zip-safe
+-rw-rw-r--   0 micah     (1000) micah     (1000)      232 2023-05-30 21:04:14.000000 radicl-0.8.0/radicl.egg-info/requires.txt
+-rw-rw-r--   0 micah     (1000) micah     (1000)        7 2023-05-30 21:04:14.000000 radicl-0.8.0/radicl.egg-info/top_level.txt
+-rw-rw-r--   0 micah     (1000) micah     (1000)      124 2021-11-30 13:51:01.000000 radicl-0.8.0/requirements_dev.txt
+-rw-rw-r--   0 micah     (1000) micah     (1000)       38 2023-05-30 21:04:14.945704 radicl-0.8.0/setup.cfg
+-rw-rw-r--   0 micah     (1000) micah     (1000)     1782 2023-05-30 21:03:45.000000 radicl-0.8.0/setup.py
+drwxrwxr-x   0 micah     (1000) micah     (1000)        0 2023-05-30 21:04:14.945704 radicl-0.8.0/tests/
+-rw-rw-r--   0 micah     (1000) micah     (1000)     2679 2023-02-26 21:10:25.000000 radicl-0.8.0/tests/__init__.py
+-rw-rw-r--   0 micah     (1000) micah     (1000)      619 2023-02-24 03:48:37.000000 radicl-0.8.0/tests/conftest.py
+drwxrwxr-x   0 micah     (1000) micah     (1000)        0 2023-05-30 21:04:14.945704 radicl-0.8.0/tests/connected/
+-rw-rw-r--   0 micah     (1000) micah     (1000)      133 2023-02-26 21:10:25.000000 radicl-0.8.0/tests/connected/__init__.py
+-rw-rw-r--   0 micah     (1000) micah     (1000)      863 2023-02-24 03:48:37.000000 radicl-0.8.0/tests/connected/test_connected_api.py
+-rw-rw-r--   0 micah     (1000) micah     (1000)      370 2023-02-26 21:10:25.000000 radicl-0.8.0/tests/connected/test_connected_gps.py
+-rw-rw-r--   0 micah     (1000) micah     (1000)     4016 2023-02-26 21:10:25.000000 radicl-0.8.0/tests/connected/test_connected_probe.py
+-rw-rw-r--   0 micah     (1000) micah     (1000)     1237 2023-02-24 03:48:37.000000 radicl-0.8.0/tests/test_api.py
+-rw-rw-r--   0 micah     (1000) micah     (1000)     2946 2023-03-03 06:44:41.000000 radicl-0.8.0/tests/test_com.py
+-rw-rw-r--   0 micah     (1000) micah     (1000)     1356 2023-02-26 21:10:25.000000 radicl-0.8.0/tests/test_gps.py
+-rw-rw-r--   0 micah     (1000) micah     (1000)      566 2023-02-24 03:48:37.000000 radicl-0.8.0/tests/test_high_resolution.py
+-rw-rw-r--   0 micah     (1000) micah     (1000)     1563 2023-02-24 03:48:37.000000 radicl-0.8.0/tests/test_interface.py
+-rw-rw-r--   0 micah     (1000) micah     (1000)      985 2023-02-24 03:48:37.000000 radicl-0.8.0/tests/test_ui_tools.py
```

### Comparing `radicl-0.7.2/LICENSE` & `radicl-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `radicl-0.7.2/PKG-INFO` & `radicl-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radicl
-Version: 0.7.2
+Version: 0.8.0
 Summary: Command line interface to the Realtime Adventure Data Lyte probe for measuring avalanche conditions
 Home-page: https://github.com/adventuredata/radicl
 Author: Micah Johnson
 Author-email: info@adventuredata.com
 License: BSD license
 Keywords: radicl
 Classifier: Development Status :: 4 - Beta
@@ -48,15 +48,14 @@
 
 * Command line interface to the Lyte probe (radicl)
 * Take Measurements (lyte_hi_res)
 * Change Probe Settings (radicl)
 * Update the Probe Firmware
 * Python API for interacting with the Lyte probe
 * Commandline script for plotting profiles taken through the app (lyteplot, plot_hi_res)
-* Open data processing!
 
 
 
 =======
 History
 =======
 
@@ -144,7 +143,13 @@
 * Added more tests and python 3.11
 * Rearranged project structure to be more editor friendly
 * Added plot time and repeat measurements to hi res script
 * Updated installation docs
 
 .. _25: https://github.com/AdventureData/radicl/issues/25
 .. _31: https://github.com/AdventureData/radicl/issues/31
+
+0.8.0 (2023-05-30)
+------------------
+* Migrated to using Study Lyte profile for plotting.
+* Added in windows daw script
+
```

### Comparing `radicl-0.7.2/README.rst` & `radicl-0.8.0/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -29,9 +29,8 @@
 
 * Command line interface to the Lyte probe (radicl)
 * Take Measurements (lyte_hi_res)
 * Change Probe Settings (radicl)
 * Update the Probe Firmware
 * Python API for interacting with the Lyte probe
 * Commandline script for plotting profiles taken through the app (lyteplot, plot_hi_res)
-* Open data processing!
```

### Comparing `radicl-0.7.2/docs/Makefile` & `radicl-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `radicl-0.7.2/docs/_build/html/_images/windows_python_installer.png` & `radicl-0.8.0/docs/_build/html/_images/windows_python_installer.png`

 * *Files identical despite different names*

### Comparing `radicl-0.7.2/docs/conf.py` & `radicl-0.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `radicl-0.7.2/docs/contributing.rst` & `radicl-0.8.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `radicl-0.7.2/docs/history.rst` & `radicl-0.8.0/docs/history.rst`

 * *Files 5% similar despite different names*

```diff
@@ -86,7 +86,13 @@
 * Added more tests and python 3.11
 * Rearranged project structure to be more editor friendly
 * Added plot time and repeat measurements to hi res script
 * Updated installation docs
 
 .. _25: https://github.com/AdventureData/radicl/issues/25
 .. _31: https://github.com/AdventureData/radicl/issues/31
+
+0.8.0 (2023-05-30)
+------------------
+* Migrated to using Study Lyte profile for plotting.
+* Added in windows daw script
+
```

### Comparing `radicl-0.7.2/docs/images/windows_python_installer.png` & `radicl-0.8.0/docs/images/windows_python_installer.png`

 * *Files identical despite different names*

### Comparing `radicl-0.7.2/docs/installation.rst` & `radicl-0.8.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `radicl-0.7.2/docs/make.bat` & `radicl-0.8.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `radicl-0.7.2/docs/radicl.rst` & `radicl-0.8.0/docs/radicl.rst`

 * *Files identical despite different names*

### Comparing `radicl-0.7.2/docs/usage.rst` & `radicl-0.8.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `radicl-0.7.2/radicl/api.py` & `radicl-0.8.0/radicl/api.py`

 * *Files identical despite different names*

### Comparing `radicl-0.7.2/radicl/calibrate.py` & `radicl-0.8.0/radicl/calibrate.py`

 * *Files identical despite different names*

### Comparing `radicl-0.7.2/radicl/cli.py` & `radicl-0.8.0/radicl/cli.py`

 * *Files identical despite different names*

### Comparing `radicl-0.7.2/radicl/com.py` & `radicl-0.8.0/radicl/com.py`

 * *Files identical despite different names*

### Comparing `radicl-0.7.2/radicl/commands.py` & `radicl-0.8.0/radicl/commands.py`

 * *Files identical despite different names*

### Comparing `radicl-0.7.2/radicl/gps.py` & `radicl-0.8.0/radicl/gps.py`

 * *Files identical despite different names*

### Comparing `radicl-0.7.2/radicl/high_resolution.py` & `radicl-0.8.0/radicl/high_resolution.py`

 * *Files identical despite different names*

### Comparing `radicl-0.7.2/radicl/interface.py` & `radicl-0.8.0/radicl/interface.py`

 * *Files identical despite different names*

### Comparing `radicl-0.7.2/radicl/probe.py` & `radicl-0.8.0/radicl/probe.py`

 * *Files identical despite different names*

### Comparing `radicl-0.7.2/radicl/ui_tools.py` & `radicl-0.8.0/radicl/ui_tools.py`

 * *Files identical despite different names*

### Comparing `radicl-0.7.2/radicl/update.py` & `radicl-0.8.0/radicl/update.py`

 * *Files identical despite different names*

### Comparing `radicl-0.7.2/radicl.egg-info/PKG-INFO` & `radicl-0.8.0/radicl.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radicl
-Version: 0.7.2
+Version: 0.8.0
 Summary: Command line interface to the Realtime Adventure Data Lyte probe for measuring avalanche conditions
 Home-page: https://github.com/adventuredata/radicl
 Author: Micah Johnson
 Author-email: info@adventuredata.com
 License: BSD license
 Keywords: radicl
 Classifier: Development Status :: 4 - Beta
@@ -48,15 +48,14 @@
 
 * Command line interface to the Lyte probe (radicl)
 * Take Measurements (lyte_hi_res)
 * Change Probe Settings (radicl)
 * Update the Probe Firmware
 * Python API for interacting with the Lyte probe
 * Commandline script for plotting profiles taken through the app (lyteplot, plot_hi_res)
-* Open data processing!
 
 
 
 =======
 History
 =======
 
@@ -144,7 +143,13 @@
 * Added more tests and python 3.11
 * Rearranged project structure to be more editor friendly
 * Added plot time and repeat measurements to hi res script
 * Updated installation docs
 
 .. _25: https://github.com/AdventureData/radicl/issues/25
 .. _31: https://github.com/AdventureData/radicl/issues/31
+
+0.8.0 (2023-05-30)
+------------------
+* Migrated to using Study Lyte profile for plotting.
+* Added in windows daw script
+
```

### Comparing `radicl-0.7.2/radicl.egg-info/SOURCES.txt` & `radicl-0.8.0/radicl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `radicl-0.7.2/setup.py` & `radicl-0.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     keywords='radicl',
     name='radicl',
     packages=find_packages(include=['radicl', 'radicl.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/adventuredata/radicl',
-    version='0.7.2',
+    version='0.8.0',
     zip_safe=False,
     entry_points={
         'console_scripts': [
             'radicl = radicl.cli:main',
             'plotlyte = radicl.plotting:main',
             'lyte_hi_res = radicl.high_resolution:main',
             'plot_hi_res = radicl.plotting:plot_hi_res_cli',
```

### Comparing `radicl-0.7.2/tests/__init__.py` & `radicl-0.8.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `radicl-0.7.2/tests/conftest.py` & `radicl-0.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `radicl-0.7.2/tests/connected/test_connected_api.py` & `radicl-0.8.0/tests/connected/test_connected_api.py`

 * *Files identical despite different names*

### Comparing `radicl-0.7.2/tests/connected/test_connected_probe.py` & `radicl-0.8.0/tests/connected/test_connected_probe.py`

 * *Files identical despite different names*

### Comparing `radicl-0.7.2/tests/test_api.py` & `radicl-0.8.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `radicl-0.7.2/tests/test_com.py` & `radicl-0.8.0/tests/test_com.py`

 * *Files identical despite different names*

### Comparing `radicl-0.7.2/tests/test_gps.py` & `radicl-0.8.0/tests/test_gps.py`

 * *Files identical despite different names*

### Comparing `radicl-0.7.2/tests/test_high_resolution.py` & `radicl-0.8.0/tests/test_high_resolution.py`

 * *Files identical despite different names*

### Comparing `radicl-0.7.2/tests/test_interface.py` & `radicl-0.8.0/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `radicl-0.7.2/tests/test_ui_tools.py` & `radicl-0.8.0/tests/test_ui_tools.py`

 * *Files identical despite different names*

