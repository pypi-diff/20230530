# Comparing `tmp/Python_Road-0.0.0.2.tar.gz` & `tmp/Python_Road-0.0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Python_Road-0.0.0.2.tar", last modified: Tue May 30 12:35:32 2023, max compression
+gzip compressed data, was "Python_Road-0.0.0.3.tar", last modified: Tue May 30 13:41:03 2023, max compression
```

## Comparing `Python_Road-0.0.0.2.tar` & `Python_Road-0.0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 12:35:32.526504 Python_Road-0.0.0.2/
--rw-rw-rw-   0        0        0      134 2023-05-30 12:35:32.521983 Python_Road-0.0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-30 12:35:32.519372 Python_Road-0.0.0.2/Python_Road.egg-info/
--rw-rw-rw-   0        0        0      134 2023-05-30 12:35:32.000000 Python_Road-0.0.0.2/Python_Road.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      163 2023-05-30 12:35:32.000000 Python_Road-0.0.0.2/Python_Road.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 12:35:32.000000 Python_Road-0.0.0.2/Python_Road.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 12:35:32.000000 Python_Road-0.0.0.2/Python_Road.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4144 2023-05-30 12:31:03.000000 Python_Road-0.0.0.2/Python_Road.py
--rw-rw-rw-   0        0        0       42 2023-05-30 12:35:32.527506 Python_Road-0.0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      213 2023-05-30 12:34:29.000000 Python_Road-0.0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:41:03.094923 Python_Road-0.0.0.3/
+-rw-rw-rw-   0        0        0      134 2023-05-30 13:41:03.094923 Python_Road-0.0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-30 13:41:03.094923 Python_Road-0.0.0.3/Python_Road.egg-info/
+-rw-rw-rw-   0        0        0      134 2023-05-30 13:41:02.000000 Python_Road-0.0.0.3/Python_Road.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2023-05-30 13:41:03.000000 Python_Road-0.0.0.3/Python_Road.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 13:41:02.000000 Python_Road-0.0.0.3/Python_Road.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 13:41:02.000000 Python_Road-0.0.0.3/Python_Road.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4412 2023-05-30 13:26:29.000000 Python_Road-0.0.0.3/Python_Road.py
+-rw-rw-rw-   0        0        0       42 2023-05-30 13:41:03.094923 Python_Road-0.0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      213 2023-05-30 13:40:13.000000 Python_Road-0.0.0.3/setup.py
```

### Comparing `Python_Road-0.0.0.2/Python_Road.py` & `Python_Road-0.0.0.3/Python_Road.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import pygame
 import turtle
 import traceback
 import random
 
 
+all_func = [{"Size":["find_all_size","all_file_size","__get_all_size","__size_small"]},{"Math":["evolution","power","cipher"]},{"Random":["random_number","random_choice","random_number_with_step"]},"printer","eval_inputer","Download_with_progress_bar","if_not_error"]
 class Size:
 	def find_file_size(self, path="C:\\", max_or_min="max"):
 		size_path, size_list = self.__get_all_size(path)
 		if max_or_min == "max":
 			fsize = size_path[size_list.index(max(size_list))][0]
 		elif max_or_min == "min":
 			fsize = size_path[size_list.index(min(size_list))][0]
```

