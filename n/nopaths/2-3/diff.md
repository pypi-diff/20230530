# Comparing `tmp/nopaths-2.tar.gz` & `tmp/nopaths-3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nopaths-2.tar", last modified: Tue May 30 01:17:51 2023, max compression
+gzip compressed data, was "nopaths-3.tar", last modified: Tue May 30 02:01:08 2023, max compression
```

## Comparing `nopaths-2.tar` & `nopaths-3.tar`

### file list

```diff
@@ -1,59 +1,61 @@
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-30 01:17:51.633320 nopaths-2/
--rw-r--r--   0 nop       (1000) nop       (1000)     4445 2023-05-30 01:17:51.633320 nopaths-2/PKG-INFO
--rw-r--r--   0 nop       (1000) nop       (1000)     2835 2023-05-29 12:59:16.000000 nopaths-2/README.rst
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-30 01:17:51.629320 nopaths-2/nopaths/
--rw-r--r--   0 nop       (1000) nop       (1000)      527 2023-05-29 13:03:22.000000 nopaths-2/nopaths/clients.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1050 2023-05-29 13:03:22.000000 nopaths-2/nopaths/clocked.py
--rw-r--r--   0 nop       (1000) nop       (1000)      923 2023-05-29 13:03:22.000000 nopaths-2/nopaths/command.py
--rw-r--r--   0 nop       (1000) nop       (1000)      127 2023-05-29 13:34:01.000000 nopaths-2/nopaths/configs.py
--rw-r--r--   0 nop       (1000) nop       (1000)      760 2023-05-29 13:03:22.000000 nopaths-2/nopaths/decoder.py
--rw-r--r--   0 nop       (1000) nop       (1000)      341 2023-05-29 13:03:22.000000 nopaths-2/nopaths/default.py
--rw-r--r--   0 nop       (1000) nop       (1000)      203 2023-05-29 13:31:30.000000 nopaths-2/nopaths/defines.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1149 2023-05-29 13:03:22.000000 nopaths-2/nopaths/encoder.py
--rw-r--r--   0 nop       (1000) nop       (1000)      368 2023-05-29 13:03:22.000000 nopaths-2/nopaths/errored.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1913 2023-05-29 13:03:22.000000 nopaths-2/nopaths/handler.py
--rw-r--r--   0 nop       (1000) nop       (1000)      903 2023-05-29 13:03:22.000000 nopaths-2/nopaths/listens.py
--rw-r--r--   0 nop       (1000) nop       (1000)      400 2023-05-29 13:03:22.000000 nopaths-2/nopaths/logging.py
--rw-r--r--   0 nop       (1000) nop       (1000)      929 2023-05-29 13:03:22.000000 nopaths-2/nopaths/message.py
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-30 01:17:51.633320 nopaths-2/nopaths/modules/
--rw-r--r--   0 nop       (1000) nop       (1000)      520 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/__init__.py
--rw-r--r--   0 nop       (1000) nop       (1000)      561 2023-05-29 13:30:51.000000 nopaths-2/nopaths/modules/cfg.py
--rw-r--r--   0 nop       (1000) nop       (1000)      158 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/cmd.py
--rw-r--r--   0 nop       (1000) nop       (1000)      365 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/err.py
--rw-r--r--   0 nop       (1000) nop       (1000)      402 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/flt.py
--rw-r--r--   0 nop       (1000) nop       (1000)      948 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/fnd.py
--rw-r--r--   0 nop       (1000) nop       (1000)    19809 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/irc.py
--rw-r--r--   0 nop       (1000) nop       (1000)      668 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/log.py
--rw-r--r--   0 nop       (1000) nop       (1000)    17771 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/mdl.py
--rw-r--r--   0 nop       (1000) nop       (1000)      136 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/mod.py
--rw-r--r--   0 nop       (1000) nop       (1000)     2385 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/req.py
--rw-r--r--   0 nop       (1000) nop       (1000)     7638 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/rss.py
--rw-r--r--   0 nop       (1000) nop       (1000)      458 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/slg.py
--rw-r--r--   0 nop       (1000) nop       (1000)      295 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/sts.py
--rw-r--r--   0 nop       (1000) nop       (1000)      892 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/tdo.py
--rw-r--r--   0 nop       (1000) nop       (1000)      989 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/thr.py
--rw-r--r--   0 nop       (1000) nop       (1000)      202 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/upt.py
--rw-r--r--   0 nop       (1000) nop       (1000)     2727 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/usr.py
--rw-r--r--   0 nop       (1000) nop       (1000)      157 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/ver.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1640 2023-05-29 13:03:22.000000 nopaths-2/nopaths/objects.py
--rw-r--r--   0 nop       (1000) nop       (1000)     2057 2023-05-29 13:03:22.000000 nopaths-2/nopaths/objfunc.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1756 2023-05-29 13:03:22.000000 nopaths-2/nopaths/parsers.py
--rw-r--r--   0 nop       (1000) nop       (1000)     3985 2023-05-29 13:03:22.000000 nopaths-2/nopaths/persist.py
--rw-r--r--   0 nop       (1000) nop       (1000)      325 2023-05-29 13:03:22.000000 nopaths-2/nopaths/repeats.py
--rw-r--r--   0 nop       (1000) nop       (1000)     2425 2023-05-30 00:56:36.000000 nopaths-2/nopaths/runtime.py
--rw-r--r--   0 nop       (1000) nop       (1000)      878 2023-05-29 13:03:22.000000 nopaths-2/nopaths/threads.py
--rw-r--r--   0 nop       (1000) nop       (1000)     2891 2023-05-29 13:03:22.000000 nopaths-2/nopaths/utility.py
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-30 01:17:51.629320 nopaths-2/nopaths.egg-info/
--rw-r--r--   0 nop       (1000) nop       (1000)     4445 2023-05-30 01:17:51.000000 nopaths-2/nopaths.egg-info/PKG-INFO
--rw-r--r--   0 nop       (1000) nop       (1000)     1115 2023-05-30 01:17:51.000000 nopaths-2/nopaths.egg-info/SOURCES.txt
--rw-r--r--   0 nop       (1000) nop       (1000)        1 2023-05-30 01:17:51.000000 nopaths-2/nopaths.egg-info/dependency_links.txt
--rw-r--r--   0 nop       (1000) nop       (1000)        8 2023-05-30 01:17:51.000000 nopaths-2/nopaths.egg-info/top_level.txt
--rw-r--r--   0 nop       (1000) nop       (1000)        1 2023-05-30 01:17:51.000000 nopaths-2/nopaths.egg-info/zip-safe
--rw-r--r--   0 nop       (1000) nop       (1000)       38 2023-05-30 01:17:51.633320 nopaths-2/setup.cfg
--rw-r--r--   0 nop       (1000) nop       (1000)      787 2023-05-30 01:16:44.000000 nopaths-2/setup.py
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-30 01:17:51.633320 nopaths-2/test/
--rw-r--r--   0 nop       (1000) nop       (1000)      483 2023-05-29 12:59:16.000000 nopaths-2/test/test_decoder.py
--rw-r--r--   0 nop       (1000) nop       (1000)      377 2023-05-29 12:59:16.000000 nopaths-2/test/test_encoder.py
--rw-r--r--   0 nop       (1000) nop       (1000)      887 2023-05-29 12:59:16.000000 nopaths-2/test/test_inherit.py
--rw-r--r--   0 nop       (1000) nop       (1000)     4580 2023-05-29 12:59:16.000000 nopaths-2/test/test_objects.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1051 2023-05-29 12:59:16.000000 nopaths-2/test/test_storage.py
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-30 02:01:08.749209 nopaths-3/
+-rw-r--r--   0 nop       (1000) nop       (1000)     4445 2023-05-30 02:01:08.749209 nopaths-3/PKG-INFO
+-rw-r--r--   0 nop       (1000) nop       (1000)     2835 2023-05-29 12:59:16.000000 nopaths-3/README.rst
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-30 02:01:08.745209 nopaths-3/bin/
+-rwxr-xr-x   0 nop       (1000) nop       (1000)     2374 2023-05-30 00:51:00.000000 nopaths-3/bin/nopaths
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-30 02:01:08.745209 nopaths-3/nopaths/
+-rw-r--r--   0 nop       (1000) nop       (1000)      527 2023-05-29 13:03:22.000000 nopaths-3/nopaths/clients.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1050 2023-05-29 13:03:22.000000 nopaths-3/nopaths/clocked.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      923 2023-05-29 13:03:22.000000 nopaths-3/nopaths/command.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      127 2023-05-29 13:34:01.000000 nopaths-3/nopaths/configs.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      760 2023-05-29 13:03:22.000000 nopaths-3/nopaths/decoder.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      341 2023-05-29 13:03:22.000000 nopaths-3/nopaths/default.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      203 2023-05-29 13:31:30.000000 nopaths-3/nopaths/defines.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1149 2023-05-29 13:03:22.000000 nopaths-3/nopaths/encoder.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      368 2023-05-29 13:03:22.000000 nopaths-3/nopaths/errored.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1913 2023-05-29 13:03:22.000000 nopaths-3/nopaths/handler.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      903 2023-05-29 13:03:22.000000 nopaths-3/nopaths/listens.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      400 2023-05-29 13:03:22.000000 nopaths-3/nopaths/logging.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      929 2023-05-29 13:03:22.000000 nopaths-3/nopaths/message.py
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-30 02:01:08.749209 nopaths-3/nopaths/modules/
+-rw-r--r--   0 nop       (1000) nop       (1000)      520 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/__init__.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      561 2023-05-29 13:30:51.000000 nopaths-3/nopaths/modules/cfg.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      158 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/cmd.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      365 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/err.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      402 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/flt.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      948 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/fnd.py
+-rw-r--r--   0 nop       (1000) nop       (1000)    19809 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/irc.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      668 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/log.py
+-rw-r--r--   0 nop       (1000) nop       (1000)    17771 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/mdl.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      136 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/mod.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     2385 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/req.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     7638 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/rss.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      458 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/slg.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      295 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/sts.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      892 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/tdo.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      989 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/thr.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      202 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/upt.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     2727 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/usr.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      157 2023-05-29 13:03:28.000000 nopaths-3/nopaths/modules/ver.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1640 2023-05-29 13:03:22.000000 nopaths-3/nopaths/objects.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     2057 2023-05-29 13:03:22.000000 nopaths-3/nopaths/objfunc.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1756 2023-05-29 13:03:22.000000 nopaths-3/nopaths/parsers.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     3985 2023-05-29 13:03:22.000000 nopaths-3/nopaths/persist.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      325 2023-05-29 13:03:22.000000 nopaths-3/nopaths/repeats.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     2425 2023-05-30 00:56:36.000000 nopaths-3/nopaths/runtime.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      878 2023-05-29 13:03:22.000000 nopaths-3/nopaths/threads.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     2891 2023-05-29 13:03:22.000000 nopaths-3/nopaths/utility.py
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-30 02:01:08.749209 nopaths-3/nopaths.egg-info/
+-rw-r--r--   0 nop       (1000) nop       (1000)     4445 2023-05-30 02:01:08.000000 nopaths-3/nopaths.egg-info/PKG-INFO
+-rw-r--r--   0 nop       (1000) nop       (1000)     1127 2023-05-30 02:01:08.000000 nopaths-3/nopaths.egg-info/SOURCES.txt
+-rw-r--r--   0 nop       (1000) nop       (1000)        1 2023-05-30 02:01:08.000000 nopaths-3/nopaths.egg-info/dependency_links.txt
+-rw-r--r--   0 nop       (1000) nop       (1000)        8 2023-05-30 02:01:08.000000 nopaths-3/nopaths.egg-info/top_level.txt
+-rw-r--r--   0 nop       (1000) nop       (1000)        1 2023-05-30 02:01:08.000000 nopaths-3/nopaths.egg-info/zip-safe
+-rw-r--r--   0 nop       (1000) nop       (1000)       38 2023-05-30 02:01:08.749209 nopaths-3/setup.cfg
+-rw-r--r--   0 nop       (1000) nop       (1000)      816 2023-05-30 02:00:11.000000 nopaths-3/setup.py
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-30 02:01:08.749209 nopaths-3/test/
+-rw-r--r--   0 nop       (1000) nop       (1000)      483 2023-05-29 12:59:16.000000 nopaths-3/test/test_decoder.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      377 2023-05-29 12:59:16.000000 nopaths-3/test/test_encoder.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      887 2023-05-29 12:59:16.000000 nopaths-3/test/test_inherit.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     4580 2023-05-29 12:59:16.000000 nopaths-3/test/test_objects.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1051 2023-05-29 12:59:16.000000 nopaths-3/test/test_storage.py
```

### Comparing `nopaths-2/PKG-INFO` & `nopaths-3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nopaths
-Version: 2
+Version: 3
 Summary: there are no paths
 Home-page: http://github.com/nopaths/nopaths
 Author: No Paths <nopaths@proton.me>
 Author-email: nopaths@proton.me
 License: Public Domain
 Description: **NAME**
```

### Comparing `nopaths-2/README.rst` & `nopaths-3/README.rst`

 * *Files identical despite different names*

### Comparing `nopaths-2/nopaths/clients.py` & `nopaths-3/nopaths/clients.py`

 * *Files identical despite different names*

### Comparing `nopaths-2/nopaths/clocked.py` & `nopaths-3/nopaths/clocked.py`

 * *Files identical despite different names*

### Comparing `nopaths-2/nopaths/command.py` & `nopaths-3/nopaths/command.py`

 * *Files identical despite different names*

### Comparing `nopaths-2/nopaths/decoder.py` & `nopaths-3/nopaths/decoder.py`

 * *Files identical despite different names*

### Comparing `nopaths-2/nopaths/encoder.py` & `nopaths-3/nopaths/encoder.py`

 * *Files identical despite different names*

### Comparing `nopaths-2/nopaths/handler.py` & `nopaths-3/nopaths/handler.py`

 * *Files identical despite different names*

### Comparing `nopaths-2/nopaths/listens.py` & `nopaths-3/nopaths/listens.py`

 * *Files identical despite different names*

### Comparing `nopaths-2/nopaths/message.py` & `nopaths-3/nopaths/message.py`

 * *Files identical despite different names*

### Comparing `nopaths-2/nopaths/modules/__init__.py` & `nopaths-3/nopaths/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `nopaths-2/nopaths/modules/cfg.py` & `nopaths-3/nopaths/modules/cfg.py`

 * *Files identical despite different names*

### Comparing `nopaths-2/nopaths/modules/fnd.py` & `nopaths-3/nopaths/modules/fnd.py`

 * *Files identical despite different names*

### Comparing `nopaths-2/nopaths/modules/irc.py` & `nopaths-3/nopaths/modules/irc.py`

 * *Files identical despite different names*

### Comparing `nopaths-2/nopaths/modules/log.py` & `nopaths-3/nopaths/modules/log.py`

 * *Files identical despite different names*

### Comparing `nopaths-2/nopaths/modules/mdl.py` & `nopaths-3/nopaths/modules/mdl.py`

 * *Files identical despite different names*

### Comparing `nopaths-2/nopaths/modules/req.py` & `nopaths-3/nopaths/modules/req.py`

 * *Files identical despite different names*

### Comparing `nopaths-2/nopaths/modules/rss.py` & `nopaths-3/nopaths/modules/rss.py`

 * *Files identical despite different names*

### Comparing `nopaths-2/nopaths/modules/tdo.py` & `nopaths-3/nopaths/modules/tdo.py`

 * *Files identical despite different names*

### Comparing `nopaths-2/nopaths/modules/thr.py` & `nopaths-3/nopaths/modules/thr.py`

 * *Files identical despite different names*

### Comparing `nopaths-2/nopaths/modules/usr.py` & `nopaths-3/nopaths/modules/usr.py`

 * *Files identical despite different names*

### Comparing `nopaths-2/nopaths/objects.py` & `nopaths-3/nopaths/objects.py`

 * *Files identical despite different names*

### Comparing `nopaths-2/nopaths/objfunc.py` & `nopaths-3/nopaths/objfunc.py`

 * *Files identical despite different names*

### Comparing `nopaths-2/nopaths/parsers.py` & `nopaths-3/nopaths/parsers.py`

 * *Files identical despite different names*

### Comparing `nopaths-2/nopaths/persist.py` & `nopaths-3/nopaths/persist.py`

 * *Files identical despite different names*

### Comparing `nopaths-2/nopaths/runtime.py` & `nopaths-3/nopaths/runtime.py`

 * *Files identical despite different names*

### Comparing `nopaths-2/nopaths/threads.py` & `nopaths-3/nopaths/threads.py`

 * *Files identical despite different names*

### Comparing `nopaths-2/nopaths/utility.py` & `nopaths-3/nopaths/utility.py`

 * *Files identical despite different names*

### Comparing `nopaths-2/nopaths.egg-info/PKG-INFO` & `nopaths-3/nopaths.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nopaths
-Version: 2
+Version: 3
 Summary: there are no paths
 Home-page: http://github.com/nopaths/nopaths
 Author: No Paths <nopaths@proton.me>
 Author-email: nopaths@proton.me
 License: Public Domain
 Description: **NAME**
```

### Comparing `nopaths-2/nopaths.egg-info/SOURCES.txt` & `nopaths-3/nopaths.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 README.rst
 setup.py
+bin/nopaths
 nopaths/clients.py
 nopaths/clocked.py
 nopaths/command.py
 nopaths/configs.py
 nopaths/decoder.py
 nopaths/default.py
 nopaths/defines.py
```

### Comparing `nopaths-2/setup.py` & `nopaths-3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,27 +6,28 @@
 
 def read():
     return open("README.rst", "r").read()
 
 
 setup(
     name="nopaths",
-    version="2",
+    version="3",
     author="No Paths <nopaths@proton.me>",
     author_email="nopaths@proton.me",
     url="http://github.com/nopaths/nopaths",
     zip_safe=True,
     description="there are no paths",
     long_description=read(),
     long_description_content_type="text/x-rst",
     license="Public Domain",
     packages=[
               "nopaths",
               'nopaths.modules'
              ],
+    scripts=["bin/nopaths"],
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: Public Domain",
         "Programming Language :: Python :: 3 :: Only",
         "Topic :: Software Development :: Libraries :: Python Modules",
      ],
 )
```

### Comparing `nopaths-2/test/test_inherit.py` & `nopaths-3/test/test_inherit.py`

 * *Files identical despite different names*

### Comparing `nopaths-2/test/test_objects.py` & `nopaths-3/test/test_objects.py`

 * *Files identical despite different names*

### Comparing `nopaths-2/test/test_storage.py` & `nopaths-3/test/test_storage.py`

 * *Files identical despite different names*

