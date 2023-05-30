# Comparing `tmp/nopaths-1.tar.gz` & `tmp/nopaths-2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nopaths-1.tar", last modified: Sat May 27 14:03:04 2023, max compression
+gzip compressed data, was "nopaths-2.tar", last modified: Tue May 30 01:17:51 2023, max compression
```

## Comparing `nopaths-1.tar` & `nopaths-2.tar`

### file list

```diff
@@ -1,54 +1,59 @@
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-27 14:03:04.082461 nopaths-1/
--rw-r--r--   0 nop       (1000) nop       (1000)     4429 2023-05-27 14:03:04.082461 nopaths-1/PKG-INFO
--rw-r--r--   0 nop       (1000) nop       (1000)     2819 2023-05-27 13:56:16.000000 nopaths-1/README.rst
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-27 14:03:04.082461 nopaths-1/nopaths/
--rw-r--r--   0 nop       (1000) nop       (1000)      235 2023-05-27 14:02:12.000000 nopaths-1/nopaths/__init__.py
--rw-r--r--   0 nop       (1000) nop       (1000)     2849 2023-05-27 13:52:26.000000 nopaths-1/nopaths/__main__.py
--rw-r--r--   0 nop       (1000) nop       (1000)      527 2023-05-27 09:45:38.000000 nopaths-1/nopaths/clients.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1050 2023-05-27 10:01:17.000000 nopaths-1/nopaths/clocked.py
--rw-r--r--   0 nop       (1000) nop       (1000)      923 2023-05-27 09:47:08.000000 nopaths-1/nopaths/command.py
--rw-r--r--   0 nop       (1000) nop       (1000)      760 2023-05-27 09:47:20.000000 nopaths-1/nopaths/decoder.py
--rw-r--r--   0 nop       (1000) nop       (1000)      341 2023-05-25 21:36:54.000000 nopaths-1/nopaths/default.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1149 2023-05-27 09:47:26.000000 nopaths-1/nopaths/encoder.py
--rw-r--r--   0 nop       (1000) nop       (1000)      368 2023-05-27 09:47:37.000000 nopaths-1/nopaths/errored.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1913 2023-05-27 12:12:22.000000 nopaths-1/nopaths/handler.py
--rw-r--r--   0 nop       (1000) nop       (1000)      903 2023-05-27 09:48:47.000000 nopaths-1/nopaths/listens.py
--rw-r--r--   0 nop       (1000) nop       (1000)      400 2023-05-27 09:48:56.000000 nopaths-1/nopaths/logging.py
--rw-r--r--   0 nop       (1000) nop       (1000)      929 2023-05-27 11:18:58.000000 nopaths-1/nopaths/message.py
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-27 14:03:04.082461 nopaths-1/nopaths/modules/
--rw-r--r--   0 nop       (1000) nop       (1000)      435 2023-05-27 07:50:18.000000 nopaths-1/nopaths/modules/__init__.py
--rw-r--r--   0 nop       (1000) nop       (1000)      158 2023-05-27 10:45:11.000000 nopaths-1/nopaths/modules/cmd.py
--rw-r--r--   0 nop       (1000) nop       (1000)      365 2023-05-27 10:45:22.000000 nopaths-1/nopaths/modules/err.py
--rw-r--r--   0 nop       (1000) nop       (1000)      402 2023-05-27 10:45:32.000000 nopaths-1/nopaths/modules/flt.py
--rw-r--r--   0 nop       (1000) nop       (1000)      948 2023-05-27 10:45:43.000000 nopaths-1/nopaths/modules/fnd.py
--rw-r--r--   0 nop       (1000) nop       (1000)    19809 2023-05-27 13:52:40.000000 nopaths-1/nopaths/modules/irc.py
--rw-r--r--   0 nop       (1000) nop       (1000)      668 2023-05-27 07:43:07.000000 nopaths-1/nopaths/modules/log.py
--rw-r--r--   0 nop       (1000) nop       (1000)      136 2023-05-27 10:46:22.000000 nopaths-1/nopaths/modules/mod.py
--rw-r--r--   0 nop       (1000) nop       (1000)     7638 2023-05-27 10:01:48.000000 nopaths-1/nopaths/modules/rss.py
--rw-r--r--   0 nop       (1000) nop       (1000)      295 2023-05-27 10:46:46.000000 nopaths-1/nopaths/modules/sts.py
--rw-r--r--   0 nop       (1000) nop       (1000)      892 2023-05-27 07:45:32.000000 nopaths-1/nopaths/modules/tdo.py
--rw-r--r--   0 nop       (1000) nop       (1000)      989 2023-05-27 10:44:37.000000 nopaths-1/nopaths/modules/thr.py
--rw-r--r--   0 nop       (1000) nop       (1000)      202 2023-05-27 10:44:51.000000 nopaths-1/nopaths/modules/upt.py
--rw-r--r--   0 nop       (1000) nop       (1000)      157 2023-05-27 10:47:40.000000 nopaths-1/nopaths/modules/ver.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1640 2023-05-27 09:50:07.000000 nopaths-1/nopaths/objects.py
--rw-r--r--   0 nop       (1000) nop       (1000)     2057 2023-05-27 10:27:52.000000 nopaths-1/nopaths/objfunc.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1756 2023-05-27 11:38:06.000000 nopaths-1/nopaths/parsers.py
--rw-r--r--   0 nop       (1000) nop       (1000)     3985 2023-05-27 10:37:50.000000 nopaths-1/nopaths/persist.py
--rw-r--r--   0 nop       (1000) nop       (1000)      287 2023-05-27 10:01:28.000000 nopaths-1/nopaths/repeats.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1427 2023-05-27 13:46:49.000000 nopaths-1/nopaths/runtime.py
--rw-r--r--   0 nop       (1000) nop       (1000)      878 2023-05-27 09:59:26.000000 nopaths-1/nopaths/threads.py
--rw-r--r--   0 nop       (1000) nop       (1000)     2884 2023-05-27 09:57:34.000000 nopaths-1/nopaths/utility.py
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-27 14:03:04.082461 nopaths-1/nopaths.egg-info/
--rw-r--r--   0 nop       (1000) nop       (1000)     4429 2023-05-27 14:03:03.000000 nopaths-1/nopaths.egg-info/PKG-INFO
--rw-r--r--   0 nop       (1000) nop       (1000)     1002 2023-05-27 14:03:04.000000 nopaths-1/nopaths.egg-info/SOURCES.txt
--rw-r--r--   0 nop       (1000) nop       (1000)        1 2023-05-27 14:03:03.000000 nopaths-1/nopaths.egg-info/dependency_links.txt
--rw-r--r--   0 nop       (1000) nop       (1000)        8 2023-05-27 14:03:03.000000 nopaths-1/nopaths.egg-info/top_level.txt
--rw-r--r--   0 nop       (1000) nop       (1000)        1 2023-05-27 14:03:03.000000 nopaths-1/nopaths.egg-info/zip-safe
--rw-r--r--   0 nop       (1000) nop       (1000)       38 2023-05-27 14:03:04.082461 nopaths-1/setup.cfg
--rw-r--r--   0 nop       (1000) nop       (1000)      787 2023-05-27 13:30:33.000000 nopaths-1/setup.py
-drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-27 14:03:04.082461 nopaths-1/test/
--rw-r--r--   0 nop       (1000) nop       (1000)      483 2023-05-27 13:41:06.000000 nopaths-1/test/test_decoder.py
--rw-r--r--   0 nop       (1000) nop       (1000)      377 2023-05-27 13:41:29.000000 nopaths-1/test/test_encoder.py
--rw-r--r--   0 nop       (1000) nop       (1000)      887 2023-05-27 13:41:52.000000 nopaths-1/test/test_inherit.py
--rw-r--r--   0 nop       (1000) nop       (1000)     4580 2023-05-27 13:48:54.000000 nopaths-1/test/test_objects.py
--rw-r--r--   0 nop       (1000) nop       (1000)     1051 2023-05-27 13:44:39.000000 nopaths-1/test/test_storage.py
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-30 01:17:51.633320 nopaths-2/
+-rw-r--r--   0 nop       (1000) nop       (1000)     4445 2023-05-30 01:17:51.633320 nopaths-2/PKG-INFO
+-rw-r--r--   0 nop       (1000) nop       (1000)     2835 2023-05-29 12:59:16.000000 nopaths-2/README.rst
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-30 01:17:51.629320 nopaths-2/nopaths/
+-rw-r--r--   0 nop       (1000) nop       (1000)      527 2023-05-29 13:03:22.000000 nopaths-2/nopaths/clients.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1050 2023-05-29 13:03:22.000000 nopaths-2/nopaths/clocked.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      923 2023-05-29 13:03:22.000000 nopaths-2/nopaths/command.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      127 2023-05-29 13:34:01.000000 nopaths-2/nopaths/configs.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      760 2023-05-29 13:03:22.000000 nopaths-2/nopaths/decoder.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      341 2023-05-29 13:03:22.000000 nopaths-2/nopaths/default.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      203 2023-05-29 13:31:30.000000 nopaths-2/nopaths/defines.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1149 2023-05-29 13:03:22.000000 nopaths-2/nopaths/encoder.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      368 2023-05-29 13:03:22.000000 nopaths-2/nopaths/errored.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1913 2023-05-29 13:03:22.000000 nopaths-2/nopaths/handler.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      903 2023-05-29 13:03:22.000000 nopaths-2/nopaths/listens.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      400 2023-05-29 13:03:22.000000 nopaths-2/nopaths/logging.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      929 2023-05-29 13:03:22.000000 nopaths-2/nopaths/message.py
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-30 01:17:51.633320 nopaths-2/nopaths/modules/
+-rw-r--r--   0 nop       (1000) nop       (1000)      520 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/__init__.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      561 2023-05-29 13:30:51.000000 nopaths-2/nopaths/modules/cfg.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      158 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/cmd.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      365 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/err.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      402 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/flt.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      948 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/fnd.py
+-rw-r--r--   0 nop       (1000) nop       (1000)    19809 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/irc.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      668 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/log.py
+-rw-r--r--   0 nop       (1000) nop       (1000)    17771 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/mdl.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      136 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/mod.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     2385 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/req.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     7638 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/rss.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      458 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/slg.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      295 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/sts.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      892 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/tdo.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      989 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/thr.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      202 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/upt.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     2727 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/usr.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      157 2023-05-29 13:03:28.000000 nopaths-2/nopaths/modules/ver.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1640 2023-05-29 13:03:22.000000 nopaths-2/nopaths/objects.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     2057 2023-05-29 13:03:22.000000 nopaths-2/nopaths/objfunc.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1756 2023-05-29 13:03:22.000000 nopaths-2/nopaths/parsers.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     3985 2023-05-29 13:03:22.000000 nopaths-2/nopaths/persist.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      325 2023-05-29 13:03:22.000000 nopaths-2/nopaths/repeats.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     2425 2023-05-30 00:56:36.000000 nopaths-2/nopaths/runtime.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      878 2023-05-29 13:03:22.000000 nopaths-2/nopaths/threads.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     2891 2023-05-29 13:03:22.000000 nopaths-2/nopaths/utility.py
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-30 01:17:51.629320 nopaths-2/nopaths.egg-info/
+-rw-r--r--   0 nop       (1000) nop       (1000)     4445 2023-05-30 01:17:51.000000 nopaths-2/nopaths.egg-info/PKG-INFO
+-rw-r--r--   0 nop       (1000) nop       (1000)     1115 2023-05-30 01:17:51.000000 nopaths-2/nopaths.egg-info/SOURCES.txt
+-rw-r--r--   0 nop       (1000) nop       (1000)        1 2023-05-30 01:17:51.000000 nopaths-2/nopaths.egg-info/dependency_links.txt
+-rw-r--r--   0 nop       (1000) nop       (1000)        8 2023-05-30 01:17:51.000000 nopaths-2/nopaths.egg-info/top_level.txt
+-rw-r--r--   0 nop       (1000) nop       (1000)        1 2023-05-30 01:17:51.000000 nopaths-2/nopaths.egg-info/zip-safe
+-rw-r--r--   0 nop       (1000) nop       (1000)       38 2023-05-30 01:17:51.633320 nopaths-2/setup.cfg
+-rw-r--r--   0 nop       (1000) nop       (1000)      787 2023-05-30 01:16:44.000000 nopaths-2/setup.py
+drwxr-xr-x   0 nop       (1000) nop       (1000)        0 2023-05-30 01:17:51.633320 nopaths-2/test/
+-rw-r--r--   0 nop       (1000) nop       (1000)      483 2023-05-29 12:59:16.000000 nopaths-2/test/test_decoder.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      377 2023-05-29 12:59:16.000000 nopaths-2/test/test_encoder.py
+-rw-r--r--   0 nop       (1000) nop       (1000)      887 2023-05-29 12:59:16.000000 nopaths-2/test/test_inherit.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     4580 2023-05-29 12:59:16.000000 nopaths-2/test/test_objects.py
+-rw-r--r--   0 nop       (1000) nop       (1000)     1051 2023-05-29 12:59:16.000000 nopaths-2/test/test_storage.py
```

### Comparing `nopaths-1/PKG-INFO` & `nopaths-2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nopaths
-Version: 1
+Version: 2
 Summary: there are no paths
 Home-page: http://github.com/nopaths/nopaths
 Author: No Paths <nopaths@proton.me>
 Author-email: nopaths@proton.me
 License: Public Domain
 Description: **NAME**
         
@@ -76,15 +76,15 @@
         list of modules::
         
             $ np mod
             cmd,err,flt,fnd,irc,log,mod,rss,sts,tdo,thr,upt
         
         start as daemon::
         
-            $ np -d
+            $ np mod=cmd,irc,rss -d
             $ 
         
         **CONFIGURATION**
         
         *irc*
```

### Comparing `nopaths-1/README.rst` & `nopaths-2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 list of modules::
 
     $ np mod
     cmd,err,flt,fnd,irc,log,mod,rss,sts,tdo,thr,upt
 
 start as daemon::
 
-    $ np -d
+    $ np mod=cmd,irc,rss -d
     $ 
 
 **CONFIGURATION**
 
 *irc*
```

### Comparing `nopaths-1/nopaths/clients.py` & `nopaths-2/nopaths/clients.py`

 * *Files identical despite different names*

### Comparing `nopaths-1/nopaths/clocked.py` & `nopaths-2/nopaths/clocked.py`

 * *Files identical despite different names*

### Comparing `nopaths-1/nopaths/command.py` & `nopaths-2/nopaths/command.py`

 * *Files identical despite different names*

### Comparing `nopaths-1/nopaths/decoder.py` & `nopaths-2/nopaths/decoder.py`

 * *Files identical despite different names*

### Comparing `nopaths-1/nopaths/encoder.py` & `nopaths-2/nopaths/encoder.py`

 * *Files identical despite different names*

### Comparing `nopaths-1/nopaths/handler.py` & `nopaths-2/nopaths/handler.py`

 * *Files identical despite different names*

### Comparing `nopaths-1/nopaths/listens.py` & `nopaths-2/nopaths/listens.py`

 * *Files identical despite different names*

### Comparing `nopaths-1/nopaths/message.py` & `nopaths-2/nopaths/message.py`

 * *Files identical despite different names*

### Comparing `nopaths-1/nopaths/modules/fnd.py` & `nopaths-2/nopaths/modules/fnd.py`

 * *Files identical despite different names*

### Comparing `nopaths-1/nopaths/modules/irc.py` & `nopaths-2/nopaths/modules/irc.py`

 * *Files identical despite different names*

### Comparing `nopaths-1/nopaths/modules/log.py` & `nopaths-2/nopaths/modules/log.py`

 * *Files identical despite different names*

### Comparing `nopaths-1/nopaths/modules/rss.py` & `nopaths-2/nopaths/modules/rss.py`

 * *Files identical despite different names*

### Comparing `nopaths-1/nopaths/modules/tdo.py` & `nopaths-2/nopaths/modules/tdo.py`

 * *Files identical despite different names*

### Comparing `nopaths-1/nopaths/modules/thr.py` & `nopaths-2/nopaths/modules/thr.py`

 * *Files identical despite different names*

### Comparing `nopaths-1/nopaths/objects.py` & `nopaths-2/nopaths/objects.py`

 * *Files identical despite different names*

### Comparing `nopaths-1/nopaths/objfunc.py` & `nopaths-2/nopaths/objfunc.py`

 * *Files identical despite different names*

### Comparing `nopaths-1/nopaths/parsers.py` & `nopaths-2/nopaths/parsers.py`

 * *Files identical despite different names*

### Comparing `nopaths-1/nopaths/persist.py` & `nopaths-2/nopaths/persist.py`

 * *Files identical despite different names*

### Comparing `nopaths-1/nopaths/threads.py` & `nopaths-2/nopaths/threads.py`

 * *Files identical despite different names*

### Comparing `nopaths-1/nopaths/utility.py` & `nopaths-2/nopaths/utility.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     if rest:
         tme += float('.' + rest)
     else:
         tme = 0
     return tme
 
 
-def name(obj):
+def name(obj) -> str:
     typ = type(obj)
     if isinstance(typ, types.ModuleType):
         return obj.__name__
     if '__self__' in dir(obj):
         return '%s.%s' % (obj.__self__.__class__.__name__, obj.__name__)
     if '__class__' in dir(obj) and '__name__' in dir(obj):
         return '%s.%s' % (obj.__class__.__name__, obj.__name__)
```

### Comparing `nopaths-1/nopaths.egg-info/PKG-INFO` & `nopaths-2/nopaths.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nopaths
-Version: 1
+Version: 2
 Summary: there are no paths
 Home-page: http://github.com/nopaths/nopaths
 Author: No Paths <nopaths@proton.me>
 Author-email: nopaths@proton.me
 License: Public Domain
 Description: **NAME**
         
@@ -76,15 +76,15 @@
         list of modules::
         
             $ np mod
             cmd,err,flt,fnd,irc,log,mod,rss,sts,tdo,thr,upt
         
         start as daemon::
         
-            $ np -d
+            $ np mod=cmd,irc,rss -d
             $ 
         
         **CONFIGURATION**
         
         *irc*
```

### Comparing `nopaths-1/nopaths.egg-info/SOURCES.txt` & `nopaths-2/nopaths.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 README.rst
 setup.py
-nopaths/__init__.py
-nopaths/__main__.py
 nopaths/clients.py
 nopaths/clocked.py
 nopaths/command.py
+nopaths/configs.py
 nopaths/decoder.py
 nopaths/default.py
+nopaths/defines.py
 nopaths/encoder.py
 nopaths/errored.py
 nopaths/handler.py
 nopaths/listens.py
 nopaths/logging.py
 nopaths/message.py
 nopaths/objects.py
@@ -23,25 +23,30 @@
 nopaths/utility.py
 nopaths.egg-info/PKG-INFO
 nopaths.egg-info/SOURCES.txt
 nopaths.egg-info/dependency_links.txt
 nopaths.egg-info/top_level.txt
 nopaths.egg-info/zip-safe
 nopaths/modules/__init__.py
+nopaths/modules/cfg.py
 nopaths/modules/cmd.py
 nopaths/modules/err.py
 nopaths/modules/flt.py
 nopaths/modules/fnd.py
 nopaths/modules/irc.py
 nopaths/modules/log.py
+nopaths/modules/mdl.py
 nopaths/modules/mod.py
+nopaths/modules/req.py
 nopaths/modules/rss.py
+nopaths/modules/slg.py
 nopaths/modules/sts.py
 nopaths/modules/tdo.py
 nopaths/modules/thr.py
 nopaths/modules/upt.py
+nopaths/modules/usr.py
 nopaths/modules/ver.py
 test/test_decoder.py
 test/test_encoder.py
 test/test_inherit.py
 test/test_objects.py
 test/test_storage.py
```

### Comparing `nopaths-1/setup.py` & `nopaths-2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 def read():
     return open("README.rst", "r").read()
 
 
 setup(
     name="nopaths",
-    version="1",
+    version="2",
     author="No Paths <nopaths@proton.me>",
     author_email="nopaths@proton.me",
     url="http://github.com/nopaths/nopaths",
     zip_safe=True,
     description="there are no paths",
     long_description=read(),
     long_description_content_type="text/x-rst",
```

### Comparing `nopaths-1/test/test_inherit.py` & `nopaths-2/test/test_inherit.py`

 * *Files identical despite different names*

### Comparing `nopaths-1/test/test_objects.py` & `nopaths-2/test/test_objects.py`

 * *Files identical despite different names*

### Comparing `nopaths-1/test/test_storage.py` & `nopaths-2/test/test_storage.py`

 * *Files identical despite different names*

