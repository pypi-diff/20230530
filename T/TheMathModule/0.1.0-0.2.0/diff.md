# Comparing `tmp/TheMathModule-0.1.0.tar.gz` & `tmp/TheMathModule-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TheMathModule-0.1.0.tar", last modified: Tue May 30 07:13:58 2023, max compression
+gzip compressed data, was "TheMathModule-0.2.0.tar", last modified: Tue May 30 09:25:54 2023, max compression
```

## Comparing `TheMathModule-0.1.0.tar` & `TheMathModule-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 07:13:58.796649 TheMathModule-0.1.0/
--rw-rw-rw-   0        0        0      293 2023-05-30 07:13:58.796649 TheMathModule-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-30 07:13:58.780656 TheMathModule-0.1.0/TheMathModule/
--rw-rw-rw-   0        0        0        0 2023-05-30 06:13:20.000000 TheMathModule-0.1.0/TheMathModule/__init__.py
--rw-rw-rw-   0        0        0      247 2023-05-30 04:39:25.000000 TheMathModule-0.1.0/TheMathModule/avg_or_mean.py
-drwxrwxrwx   0        0        0        0 2023-05-30 07:13:58.792660 TheMathModule-0.1.0/TheMathModule.egg-info/
--rw-rw-rw-   0        0        0      293 2023-05-30 07:13:58.000000 TheMathModule-0.1.0/TheMathModule.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2023-05-30 07:13:58.000000 TheMathModule-0.1.0/TheMathModule.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 07:13:58.000000 TheMathModule-0.1.0/TheMathModule.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-30 07:13:58.000000 TheMathModule-0.1.0/TheMathModule.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 07:13:58.797646 TheMathModule-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      380 2023-05-30 07:09:32.000000 TheMathModule-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 09:25:54.781204 TheMathModule-0.2.0/
+-rw-rw-rw-   0        0        0      356 2023-05-30 09:25:54.780208 TheMathModule-0.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-30 09:25:54.763252 TheMathModule-0.2.0/TheMathModule/
+-rw-rw-rw-   0        0        0        0 2023-05-30 06:13:20.000000 TheMathModule-0.2.0/TheMathModule/__init__.py
+-rw-rw-rw-   0        0        0      217 2023-05-30 07:30:32.000000 TheMathModule-0.2.0/TheMathModule/avg_or_mean.py
+drwxrwxrwx   0        0        0        0 2023-05-30 09:25:54.777215 TheMathModule-0.2.0/TheMathModule.egg-info/
+-rw-rw-rw-   0        0        0      356 2023-05-30 09:25:54.000000 TheMathModule-0.2.0/TheMathModule.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2023-05-30 09:25:54.000000 TheMathModule-0.2.0/TheMathModule.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 09:25:54.000000 TheMathModule-0.2.0/TheMathModule.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-30 09:25:54.000000 TheMathModule-0.2.0/TheMathModule.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 09:25:54.781204 TheMathModule-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      445 2023-05-30 07:38:27.000000 TheMathModule-0.2.0/setup.py
```

