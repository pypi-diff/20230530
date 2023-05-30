# Comparing `tmp/tibis-1.0.5.tar.gz` & `tmp/tibis-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tibis-1.0.5.tar", max compression
+gzip compressed data, was "tibis-1.0.6.tar", max compression
```

## Comparing `tibis-1.0.5.tar` & `tibis-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1317 2023-03-06 21:38:44.122690 tibis-1.0.5/LICENSE
--rw-r--r--   0        0        0     1494 2023-03-06 21:38:44.122690 tibis-1.0.5/README.md
--rw-r--r--   0        0        0      517 2023-03-06 21:38:44.122690 tibis-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     1602 2023-03-06 21:38:44.122690 tibis-1.0.5/tibis/lib/args_parser.py
--rw-r--r--   0        0        0     4972 2023-03-06 21:38:44.122690 tibis-1.0.5/tibis/lib/common.py
--rw-r--r--   0        0        0      366 2023-03-06 21:38:44.122690 tibis-1.0.5/tibis/lib/config.py
--rw-r--r--   0        0        0     2956 2023-03-06 21:38:44.122690 tibis-1.0.5/tibis/lib/create.py
--rw-r--r--   0        0        0      935 2023-03-06 21:38:44.122690 tibis-1.0.5/tibis/lib/delete.py
--rw-r--r--   0        0        0     1267 2023-03-06 21:38:44.122690 tibis-1.0.5/tibis/lib/first_time.py
--rw-r--r--   0        0        0      562 2023-03-06 21:38:44.122690 tibis-1.0.5/tibis/lib/list.py
--rw-r--r--   0        0        0     1054 2023-03-06 21:38:44.122690 tibis-1.0.5/tibis/lib/lock.py
--rw-r--r--   0        0        0      540 2023-03-06 21:38:44.122690 tibis-1.0.5/tibis/lib/logger.py
--rw-r--r--   0        0        0     1180 2023-03-06 21:38:44.122690 tibis-1.0.5/tibis/lib/static.py
--rw-r--r--   0        0        0     1643 2023-03-06 21:38:44.122690 tibis-1.0.5/tibis/lib/unlock.py
--rw-r--r--   0        0        0      729 2023-03-06 21:38:44.122690 tibis-1.0.5/tibis/tibis.py
--rw-r--r--   0        0        0     2290 1970-01-01 00:00:00.000000 tibis-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1317 2022-05-04 07:11:06.352528 tibis-1.0.6/LICENSE
+-rw-r--r--   0        0        0     3298 2023-03-07 15:28:13.653463 tibis-1.0.6/README.md
+-rw-r--r--   0        0        0      499 2023-05-30 15:54:32.843837 tibis-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1602 2022-05-04 07:11:06.355861 tibis-1.0.6/tibis/lib/args_parser.py
+-rw-r--r--   0        0        0     4972 2023-03-06 20:46:55.708576 tibis-1.0.6/tibis/lib/common.py
+-rw-r--r--   0        0        0      366 2022-11-15 15:00:51.186221 tibis-1.0.6/tibis/lib/config.py
+-rw-r--r--   0        0        0     2956 2022-11-15 15:00:41.092868 tibis-1.0.6/tibis/lib/create.py
+-rw-r--r--   0        0        0      935 2022-05-04 07:11:06.355861 tibis-1.0.6/tibis/lib/delete.py
+-rw-r--r--   0        0        0     1267 2022-05-04 07:40:49.614937 tibis-1.0.6/tibis/lib/first_time.py
+-rw-r--r--   0        0        0      562 2022-05-04 07:11:06.355861 tibis-1.0.6/tibis/lib/list.py
+-rw-r--r--   0        0        0     1054 2022-05-04 08:17:44.853283 tibis-1.0.6/tibis/lib/lock.py
+-rw-r--r--   0        0        0      540 2022-05-04 07:11:06.355861 tibis-1.0.6/tibis/lib/logger.py
+-rw-r--r--   0        0        0     1180 2023-05-30 15:54:51.797261 tibis-1.0.6/tibis/lib/static.py
+-rw-r--r--   0        0        0     1643 2023-03-07 09:14:53.679647 tibis-1.0.6/tibis/lib/unlock.py
+-rw-r--r--   0        0        0      729 2022-05-04 07:28:38.614261 tibis-1.0.6/tibis/tibis.py
+-rw-r--r--   0        0        0     4055 1970-01-01 00:00:00.000000 tibis-1.0.6/PKG-INFO
```

### Comparing `tibis-1.0.5/LICENSE` & `tibis-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tibis-1.0.5/tibis/lib/args_parser.py` & `tibis-1.0.6/tibis/lib/args_parser.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.5/tibis/lib/common.py` & `tibis-1.0.6/tibis/lib/common.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.5/tibis/lib/create.py` & `tibis-1.0.6/tibis/lib/create.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.5/tibis/lib/delete.py` & `tibis-1.0.6/tibis/lib/delete.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.5/tibis/lib/first_time.py` & `tibis-1.0.6/tibis/lib/first_time.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.5/tibis/lib/list.py` & `tibis-1.0.6/tibis/lib/list.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.5/tibis/lib/lock.py` & `tibis-1.0.6/tibis/lib/lock.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.5/tibis/lib/logger.py` & `tibis-1.0.6/tibis/lib/logger.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.5/tibis/lib/static.py` & `tibis-1.0.6/tibis/lib/static.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pathlib import Path
 
-version  = '1.0.5'
+version  = '1.0.6'
 codename = "Ibis is born"
 
 tibis_config_file="config.yml"
 tibis_config_location=str(Path.home())+"/.config/tibis/"
 tibis_full_config_location=tibis_config_location+tibis_config_file
 
 tibis_keys_location=tibis_config_location+"keys"
```

### Comparing `tibis-1.0.5/tibis/lib/unlock.py` & `tibis-1.0.6/tibis/lib/unlock.py`

 * *Files identical despite different names*

### Comparing `tibis-1.0.5/tibis/tibis.py` & `tibis-1.0.6/tibis/tibis.py`

 * *Files identical despite different names*

