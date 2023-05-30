# Comparing `tmp/jdReplace-3.1.tar.gz` & `tmp/jdReplace-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jdReplace-3.1.tar", last modified: Thu Jul 28 14:11:19 2022, max compression
+gzip compressed data, was "jdReplace-4.0.tar", last modified: Tue May 30 13:22:36 2023, max compression
```

## Comparing `jdReplace-3.1.tar` & `jdReplace-4.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-28 14:11:19.636763 jdReplace-3.1/
--rw-rw-rw-   0 root         (0) root         (0)    35065 2022-07-28 14:11:11.000000 jdReplace-3.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       77 2022-07-28 14:11:11.000000 jdReplace-3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1541 2022-07-28 14:11:19.636763 jdReplace-3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       80 2022-07-28 14:11:11.000000 jdReplace-3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-28 14:11:19.633763 jdReplace-3.1/jdReplace/
--rw-rw-rw-   0 root         (0) root         (0)     9169 2022-07-28 14:11:11.000000 jdReplace-3.1/jdReplace/Logo.svg
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-28 14:11:11.000000 jdReplace-3.1/jdReplace/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    10017 2022-07-28 14:11:11.000000 jdReplace-3.1/jdReplace/jdReplace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-28 14:11:19.636763 jdReplace-3.1/jdReplace/translation/
--rw-rw-rw-   0 root         (0) root         (0)     1016 2022-07-28 14:11:11.000000 jdReplace-3.1/jdReplace/translation/de.lang
--rw-rw-rw-   0 root         (0) root         (0)      927 2022-07-28 14:11:11.000000 jdReplace-3.1/jdReplace/translation/en.lang
--rw-rw-rw-   0 root         (0) root         (0)     1004 2022-07-28 14:11:11.000000 jdReplace-3.1/jdReplace/translation/nl.lang
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-28 14:11:19.635763 jdReplace-3.1/jdReplace.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1541 2022-07-28 14:11:19.000000 jdReplace-3.1/jdReplace.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      392 2022-07-28 14:11:19.000000 jdReplace-3.1/jdReplace.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-28 14:11:19.000000 jdReplace-3.1/jdReplace.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2022-07-28 14:11:19.000000 jdReplace-3.1/jdReplace.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       26 2022-07-28 14:11:19.000000 jdReplace-3.1/jdReplace.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2022-07-28 14:11:19.000000 jdReplace-3.1/jdReplace.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-07-28 14:11:19.636763 jdReplace-3.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1896 2022-07-28 14:11:11.000000 jdReplace-3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:22:36.702765 jdReplace-4.0/
+-rw-r--r--   0 root         (0) root         (0)     2202 2023-05-30 13:15:47.000000 jdReplace-4.0/BuildBackend.py
+-rw-r--r--   0 root         (0) root         (0)    35075 2023-05-30 13:15:47.000000 jdReplace-4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      102 2023-05-30 13:15:47.000000 jdReplace-4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4722 2023-05-30 13:22:36.702765 jdReplace-4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3243 2023-05-30 13:15:47.000000 jdReplace-4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:22:36.702765 jdReplace-4.0/jdReplace/
+-rw-r--r--   0 root         (0) root         (0)     9169 2023-05-30 13:15:47.000000 jdReplace-4.0/jdReplace/Logo.svg
+-rwxr-xr-x   0 root         (0) root         (0)    11037 2023-05-30 13:15:47.000000 jdReplace-4.0/jdReplace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       25 2023-05-30 13:15:47.000000 jdReplace-4.0/jdReplace/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:22:36.702765 jdReplace-4.0/jdReplace/translations/
+-rw-r--r--   0 root         (0) root         (0)     4476 2023-05-30 13:15:47.000000 jdReplace-4.0/jdReplace/translations/jdReplace_de.ts
+-rw-r--r--   0 root         (0) root         (0)     4448 2023-05-30 13:15:47.000000 jdReplace-4.0/jdReplace/translations/jdReplace_nl.ts
+-rw-r--r--   0 root         (0) root         (0)        3 2023-05-30 13:15:47.000000 jdReplace-4.0/jdReplace/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 13:22:36.702765 jdReplace-4.0/jdReplace.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4722 2023-05-30 13:22:36.000000 jdReplace-4.0/jdReplace.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      423 2023-05-30 13:22:36.000000 jdReplace-4.0/jdReplace.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 13:22:36.000000 jdReplace-4.0/jdReplace.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2023-05-30 13:22:36.000000 jdReplace-4.0/jdReplace.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-30 13:22:36.000000 jdReplace-4.0/jdReplace.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-30 13:22:36.000000 jdReplace-4.0/jdReplace.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1715 2023-05-30 13:15:47.000000 jdReplace-4.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 13:22:36.702765 jdReplace-4.0/setup.cfg
```

### Comparing `jdReplace-3.1/LICENSE` & `jdReplace-4.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -628,15 +628,15 @@
 
   To do so, attach the following notices to the program.  It is safest
 to attach them to the start of each source file to most effectively
 state the exclusion of warranty; and each file should have at least
 the "copyright" line and a pointer to where the full notice is found.
 
     jdReplace
-    Copyright (C) 2019  JakobDev
+    Copyright (C) 2019-2023  JakobDev
 
     This program is free software: you can redistribute it and/or modify
     it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
 
     This program is distributed in the hope that it will be useful,
@@ -648,15 +648,15 @@
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 Also add information on how to contact you by electronic and paper mail.
 
   If the program does terminal interaction, make it output a short
 notice like this when it starts in an interactive mode:
 
-    jdReplace  Copyright (C) 2019  JakobDev
+    jdReplace  Copyright (C) 2019-2023  JakobDev
     This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
     This is free software, and you are welcome to redistribute it
     under certain conditions; type `show c' for details.
 
 The hypothetical commands `show w' and `show c' should show the appropriate
 parts of the General Public License.  Of course, your program's commands
 might be different; for a GUI interface, you would use an "about box".
```

### Comparing `jdReplace-3.1/jdReplace/Logo.svg` & `jdReplace-4.0/jdReplace/Logo.svg`

 * *Files identical despite different names*

