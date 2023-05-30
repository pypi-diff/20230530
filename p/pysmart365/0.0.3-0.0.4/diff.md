# Comparing `tmp/pysmart365-0.0.3.tar.gz` & `tmp/pysmart365-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysmart365-0.0.3.tar", last modified: Sun May 28 18:52:55 2023, max compression
+gzip compressed data, was "pysmart365-0.0.4.tar", last modified: Tue May 30 15:09:17 2023, max compression
```

## Comparing `pysmart365-0.0.3.tar` & `pysmart365-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 18:52:55.765820 pysmart365-0.0.3/
--rw-rw-rw-   0        0        0    35802 2023-05-27 14:51:46.000000 pysmart365-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      445 2023-05-28 18:52:55.763820 pysmart365-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      583 2023-05-28 11:36:50.000000 pysmart365-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 18:52:55.726818 pysmart365-0.0.3/pysmart365/
--rw-rw-rw-   0        0        0      475 2023-05-28 18:25:21.000000 pysmart365-0.0.3/pysmart365/MicroSoftware.py
--rw-rw-rw-   0        0        0     2275 2023-05-28 18:19:39.000000 pysmart365-0.0.3/pysmart365/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 18:52:55.756820 pysmart365-0.0.3/pysmart365.egg-info/
--rw-rw-rw-   0        0        0      445 2023-05-28 18:52:55.000000 pysmart365-0.0.3/pysmart365.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2023-05-28 18:52:55.000000 pysmart365-0.0.3/pysmart365.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 18:52:55.000000 pysmart365-0.0.3/pysmart365.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-28 18:52:55.000000 pysmart365-0.0.3/pysmart365.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 18:52:55.767820 pysmart365-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      491 2023-05-28 18:52:36.000000 pysmart365-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:09:17.659386 pysmart365-0.0.4/
+-rw-rw-rw-   0        0        0    35802 2023-05-27 14:51:46.000000 pysmart365-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      467 2023-05-30 15:09:17.643786 pysmart365-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      583 2023-05-28 11:36:50.000000 pysmart365-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 15:09:17.628186 pysmart365-0.0.4/pysmart365/
+-rw-rw-rw-   0        0        0     1103 2023-05-29 17:14:25.000000 pysmart365-0.0.4/pysmart365/MicroSoftware.py
+-rw-rw-rw-   0        0        0     2319 2023-05-29 11:53:59.000000 pysmart365-0.0.4/pysmart365/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:09:17.643786 pysmart365-0.0.4/pysmart365.egg-info/
+-rw-rw-rw-   0        0        0      467 2023-05-30 15:09:17.000000 pysmart365-0.0.4/pysmart365.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2023-05-30 15:09:17.000000 pysmart365-0.0.4/pysmart365.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 15:09:17.000000 pysmart365-0.0.4/pysmart365.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-30 15:09:17.000000 pysmart365-0.0.4/pysmart365.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 15:09:17.659386 pysmart365-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      505 2023-05-29 17:53:53.000000 pysmart365-0.0.4/setup.py
```

### Comparing `pysmart365-0.0.3/LICENSE` & `pysmart365-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pysmart365-0.0.3/README.md` & `pysmart365-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pysmart365-0.0.3/pysmart365/__init__.py` & `pysmart365-0.0.4/pysmart365/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 class main():
     print("Welcome to pysmart365 0.0.3")
 
 import subprocess
 import platform
 from customtkinter import *
 from tkinter import messagebox
+import sys
 
 def turn_off(time):
     '''
     Shutdown pc directly without gui graphics.
     '''
     if time is None or 0:
         subprocess.run(['shutdown', '-s', '-t', '0'])
@@ -55,9 +56,11 @@
     '''
     Enter the copyright text that will be displayed with the name that you can customize and the year using the attribute 'company' for the name and 'year' for the year.
     Example if i write copyright_view(year='2022 - 2023', company= 'Informatic365')
     then displays "© Copyright 2022 - 2023 Informatic365".
     '''
     get = f'© Copyright {year} {company}'
     return get
+class close():
+    sys.exit()
 if __name__ == '__main__':
     main()
```

