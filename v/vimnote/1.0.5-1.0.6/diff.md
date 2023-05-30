# Comparing `tmp/vimnote-1.0.5.tar.gz` & `tmp/vimnote-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vimnote-1.0.5.tar", max compression
+gzip compressed data, was "vimnote-1.0.6.tar", max compression
```

## Comparing `vimnote-1.0.5.tar` & `vimnote-1.0.6.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0      384 2022-01-18 12:32:38.061233 vimnote-1.0.5/pyproject.toml
--rwxr-xr-x   0        0        0     2629 2022-01-14 09:57:54.302262 vimnote-1.0.5/vimnote/__init__.py
--rw-r--r--   0        0        0      605 2021-12-04 13:26:03.707052 vimnote-1.0.5/vimnote/bookpreview.py
--rw-r--r--   0        0        0     2723 2022-01-14 09:20:10.648541 vimnote-1.0.5/vimnote/bookview.py
--rw-r--r--   0        0        0     1204 2021-12-04 10:11:01.504942 vimnote-1.0.5/vimnote/config.py
--rw-r--r--   0        0        0     2528 2021-12-03 14:40:59.240110 vimnote-1.0.5/vimnote/deletedialog.py
--rw-r--r--   0        0        0      458 2021-12-03 10:51:51.639807 vimnote-1.0.5/vimnote/exceptions.py
--rw-r--r--   0        0        0      610 2021-12-04 12:51:11.668608 vimnote-1.0.5/vimnote/notepreview.py
--rw-r--r--   0        0        0     3293 2022-01-14 09:21:54.501623 vimnote-1.0.5/vimnote/noteview.py
--rw-r--r--   0        0        0      437 2021-12-04 12:50:50.505314 vimnote-1.0.5/vimnote/preview.py
--rw-r--r--   0        0        0    15104 2022-01-14 09:53:30.985983 vimnote-1.0.5/vimnote/tableview.py
--rw-r--r--   0        0        0     2556 2021-12-04 05:42:21.232462 vimnote-1.0.5/vimnote/textbox.py
--rw-r--r--   0        0        0      623 2022-01-18 12:32:45.886412 vimnote-1.0.5/setup.py
--rw-r--r--   0        0        0      336 2022-01-18 12:32:45.886682 vimnote-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0      384 2023-05-30 11:37:46.066714 vimnote-1.0.6/pyproject.toml
+-rwxr-xr-x   0        0        0     2629 2022-01-14 09:57:54.302262 vimnote-1.0.6/vimnote/__init__.py
+-rw-r--r--   0        0        0      605 2021-12-04 13:26:03.707052 vimnote-1.0.6/vimnote/bookpreview.py
+-rw-r--r--   0        0        0     2723 2022-01-14 09:20:10.648541 vimnote-1.0.6/vimnote/bookview.py
+-rw-r--r--   0        0        0     1204 2021-12-04 10:11:01.504942 vimnote-1.0.6/vimnote/config.py
+-rw-r--r--   0        0        0     2528 2021-12-03 14:40:59.240110 vimnote-1.0.6/vimnote/deletedialog.py
+-rw-r--r--   0        0        0      458 2021-12-03 10:51:51.639807 vimnote-1.0.6/vimnote/exceptions.py
+-rw-r--r--   0        0        0      610 2021-12-04 12:51:11.668608 vimnote-1.0.6/vimnote/notepreview.py
+-rw-r--r--   0        0        0     3293 2022-01-14 09:21:54.501623 vimnote-1.0.6/vimnote/noteview.py
+-rw-r--r--   0        0        0      437 2021-12-04 12:50:50.505314 vimnote-1.0.6/vimnote/preview.py
+-rw-r--r--   0        0        0    15104 2022-01-14 09:53:30.985983 vimnote-1.0.6/vimnote/tableview.py
+-rw-r--r--   0        0        0     2556 2021-12-04 05:42:21.232462 vimnote-1.0.6/vimnote/textbox.py
+-rw-r--r--   0        0        0      387 1970-01-01 00:00:00.000000 vimnote-1.0.6/PKG-INFO
```

### Comparing `vimnote-1.0.5/vimnote/__init__.py` & `vimnote-1.0.6/vimnote/__init__.py`

 * *Files identical despite different names*

### Comparing `vimnote-1.0.5/vimnote/bookpreview.py` & `vimnote-1.0.6/vimnote/bookpreview.py`

 * *Files identical despite different names*

### Comparing `vimnote-1.0.5/vimnote/bookview.py` & `vimnote-1.0.6/vimnote/bookview.py`

 * *Files identical despite different names*

### Comparing `vimnote-1.0.5/vimnote/config.py` & `vimnote-1.0.6/vimnote/config.py`

 * *Files identical despite different names*

### Comparing `vimnote-1.0.5/vimnote/deletedialog.py` & `vimnote-1.0.6/vimnote/deletedialog.py`

 * *Files identical despite different names*

### Comparing `vimnote-1.0.5/vimnote/notepreview.py` & `vimnote-1.0.6/vimnote/notepreview.py`

 * *Files identical despite different names*

### Comparing `vimnote-1.0.5/vimnote/noteview.py` & `vimnote-1.0.6/vimnote/noteview.py`

 * *Files identical despite different names*

### Comparing `vimnote-1.0.5/vimnote/tableview.py` & `vimnote-1.0.6/vimnote/tableview.py`

 * *Files identical despite different names*

### Comparing `vimnote-1.0.5/vimnote/textbox.py` & `vimnote-1.0.6/vimnote/textbox.py`

 * *Files identical despite different names*

