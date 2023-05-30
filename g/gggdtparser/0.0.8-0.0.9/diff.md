# Comparing `tmp/gggdtparser-0.0.8.tar.gz` & `tmp/gggdtparser-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gggdtparser-0.0.8.tar", last modified: Tue May 30 11:42:51 2023, max compression
+gzip compressed data, was "gggdtparser-0.0.9.tar", last modified: Tue May 30 11:55:17 2023, max compression
```

## Comparing `gggdtparser-0.0.8.tar` & `gggdtparser-0.0.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 11:42:51.316922 gggdtparser-0.0.8/
--rw-rw-rw-   0        0        0     1088 2023-03-27 06:45:03.000000 gggdtparser-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     3404 2023-05-30 11:42:51.316922 gggdtparser-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2689 2023-04-10 04:20:03.000000 gggdtparser-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-30 11:42:51.265061 gggdtparser-0.0.8/gggdtparser/
--rw-rw-rw-   0        0        0      227 2023-05-16 08:44:33.000000 gggdtparser-0.0.8/gggdtparser/__init__.py
--rw-rw-rw-   0        0        0     2824 2023-05-30 08:08:48.000000 gggdtparser-0.0.8/gggdtparser/dtconfigs.py
--rw-rw-rw-   0        0        0    17946 2023-05-30 06:56:51.000000 gggdtparser-0.0.8/gggdtparser/dtparser.py
-drwxrwxrwx   0        0        0        0 2023-05-30 11:42:51.299968 gggdtparser-0.0.8/gggdtparser/langs/
--rw-rw-rw-   0        0        0       88 2023-04-20 07:19:51.000000 gggdtparser-0.0.8/gggdtparser/langs/__init__.py
--rw-rw-rw-   0        0        0      235 2023-05-30 07:17:00.000000 gggdtparser-0.0.8/gggdtparser/langs/_id.py
--rw-rw-rw-   0        0        0      246 2023-05-25 03:05:13.000000 gggdtparser-0.0.8/gggdtparser/langs/az.py
--rw-rw-rw-   0        0        0      678 2023-05-25 03:05:13.000000 gggdtparser-0.0.8/gggdtparser/langs/de.py
--rw-rw-rw-   0        0        0     4773 2023-05-30 07:53:40.000000 gggdtparser-0.0.8/gggdtparser/langs/default.py
--rw-rw-rw-   0        0        0     3399 2023-05-30 08:20:26.000000 gggdtparser-0.0.8/gggdtparser/langs/en.py
--rw-rw-rw-   0        0        0      703 2023-05-25 03:05:13.000000 gggdtparser-0.0.8/gggdtparser/langs/es.py
--rw-rw-rw-   0        0        0      943 2023-05-25 03:05:13.000000 gggdtparser-0.0.8/gggdtparser/langs/fra.py
--rw-rw-rw-   0        0        0      223 2023-05-30 08:08:07.000000 gggdtparser-0.0.8/gggdtparser/langs/hi.py
--rw-rw-rw-   0        0        0      239 2023-05-30 06:33:25.000000 gggdtparser-0.0.8/gggdtparser/langs/ky.py
--rw-rw-rw-   0        0        0      345 2023-05-30 07:58:49.000000 gggdtparser-0.0.8/gggdtparser/langs/mr.py
--rw-rw-rw-   0        0        0      804 2023-05-30 07:50:28.000000 gggdtparser-0.0.8/gggdtparser/langs/ru.py
--rw-rw-rw-   0        0        0      249 2023-05-30 07:52:16.000000 gggdtparser-0.0.8/gggdtparser/langs/rw.py
--rw-rw-rw-   0        0        0      238 2023-05-30 08:00:58.000000 gggdtparser-0.0.8/gggdtparser/langs/si.py
--rw-rw-rw-   0        0        0      230 2023-05-25 03:05:13.000000 gggdtparser-0.0.8/gggdtparser/langs/so.py
--rw-rw-rw-   0        0        0      329 2023-05-30 07:55:53.000000 gggdtparser-0.0.8/gggdtparser/langs/sw.py
--rw-rw-rw-   0        0        0      745 2023-05-25 03:05:13.000000 gggdtparser-0.0.8/gggdtparser/langs/swe.py
--rw-rw-rw-   0        0        0      195 2023-05-30 08:05:09.000000 gggdtparser-0.0.8/gggdtparser/langs/tg.py
--rw-rw-rw-   0        0        0      300 2023-05-30 08:05:26.000000 gggdtparser-0.0.8/gggdtparser/langs/tr.py
--rw-rw-rw-   0        0        0      811 2023-05-30 07:48:04.000000 gggdtparser-0.0.8/gggdtparser/langs/uk.py
--rw-rw-rw-   0        0        0      231 2023-05-30 06:37:38.000000 gggdtparser-0.0.8/gggdtparser/langs/ur.py
--rw-rw-rw-   0        0        0      432 2023-05-25 03:05:13.000000 gggdtparser-0.0.8/gggdtparser/langs/vie.py
--rw-rw-rw-   0        0        0      802 2023-05-25 03:05:13.000000 gggdtparser-0.0.8/gggdtparser/langs/zh.py
--rw-rw-rw-   0        0        0      609 2023-05-25 03:05:13.000000 gggdtparser-0.0.8/gggdtparser/langs/zht.py
-drwxrwxrwx   0        0        0        0 2023-05-30 11:42:51.314927 gggdtparser-0.0.8/gggdtparser/test/
--rw-rw-rw-   0        0        0    43437 2023-05-25 04:15:16.000000 gggdtparser-0.0.8/gggdtparser/test/__init__.py
--rw-rw-rw-   0        0        0      112 2023-05-30 07:17:35.000000 gggdtparser-0.0.8/gggdtparser/test/_id.py
--rw-rw-rw-   0        0        0      829 2023-04-20 08:57:23.000000 gggdtparser-0.0.8/gggdtparser/test/az.py
--rw-rw-rw-   0        0        0      120 2023-05-30 08:08:48.000000 gggdtparser-0.0.8/gggdtparser/test/hi.py
--rw-rw-rw-   0        0        0      118 2023-05-30 06:34:41.000000 gggdtparser-0.0.8/gggdtparser/test/ky.py
--rw-rw-rw-   0        0        0      211 2023-05-30 07:59:04.000000 gggdtparser-0.0.8/gggdtparser/test/mr.py
--rw-rw-rw-   0        0        0      117 2023-05-30 07:52:38.000000 gggdtparser-0.0.8/gggdtparser/test/ru.py
--rw-rw-rw-   0        0        0      136 2023-05-30 07:52:38.000000 gggdtparser-0.0.8/gggdtparser/test/rw.py
--rw-rw-rw-   0        0        0      129 2023-05-30 08:01:52.000000 gggdtparser-0.0.8/gggdtparser/test/si.py
--rw-rw-rw-   0        0        0      158 2023-05-30 07:56:38.000000 gggdtparser-0.0.8/gggdtparser/test/sw.py
--rw-rw-rw-   0        0        0      129 2023-05-30 08:06:27.000000 gggdtparser-0.0.8/gggdtparser/test/tg.py
--rw-rw-rw-   0        0        0      127 2023-05-30 08:03:19.000000 gggdtparser-0.0.8/gggdtparser/test/tr.py
--rw-rw-rw-   0        0        0      178 2023-05-30 07:49:10.000000 gggdtparser-0.0.8/gggdtparser/test/uk.py
--rw-rw-rw-   0        0        0      140 2023-05-30 06:39:37.000000 gggdtparser-0.0.8/gggdtparser/test/ur.py
--rw-rw-rw-   0        0        0      555 2023-05-30 11:38:37.000000 gggdtparser-0.0.8/gggdtparser/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-30 11:42:51.269050 gggdtparser-0.0.8/gggdtparser.egg-info/
--rw-rw-rw-   0        0        0     3404 2023-05-30 11:42:51.000000 gggdtparser-0.0.8/gggdtparser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1191 2023-05-30 11:42:51.000000 gggdtparser-0.0.8/gggdtparser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 11:42:51.000000 gggdtparser-0.0.8/gggdtparser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-30 11:42:51.000000 gggdtparser-0.0.8/gggdtparser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      775 2023-05-30 11:42:51.317919 gggdtparser-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      165 2023-03-27 07:16:57.000000 gggdtparser-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 11:55:17.916194 gggdtparser-0.0.9/
+-rw-rw-rw-   0        0        0     1088 2023-03-27 06:45:03.000000 gggdtparser-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3404 2023-05-30 11:55:17.916194 gggdtparser-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2689 2023-04-10 04:20:03.000000 gggdtparser-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 11:55:17.873308 gggdtparser-0.0.9/gggdtparser/
+-rw-rw-rw-   0        0        0      227 2023-05-16 08:44:33.000000 gggdtparser-0.0.9/gggdtparser/__init__.py
+-rw-rw-rw-   0        0        0     2824 2023-05-30 08:08:48.000000 gggdtparser-0.0.9/gggdtparser/dtconfigs.py
+-rw-rw-rw-   0        0        0    17946 2023-05-30 06:56:51.000000 gggdtparser-0.0.9/gggdtparser/dtparser.py
+drwxrwxrwx   0        0        0        0 2023-05-30 11:55:17.901234 gggdtparser-0.0.9/gggdtparser/langs/
+-rw-rw-rw-   0        0        0       88 2023-04-20 07:19:51.000000 gggdtparser-0.0.9/gggdtparser/langs/__init__.py
+-rw-rw-rw-   0        0        0      235 2023-05-30 07:17:00.000000 gggdtparser-0.0.9/gggdtparser/langs/_id.py
+-rw-rw-rw-   0        0        0      246 2023-05-25 03:05:13.000000 gggdtparser-0.0.9/gggdtparser/langs/az.py
+-rw-rw-rw-   0        0        0      678 2023-05-25 03:05:13.000000 gggdtparser-0.0.9/gggdtparser/langs/de.py
+-rw-rw-rw-   0        0        0     4773 2023-05-30 07:53:40.000000 gggdtparser-0.0.9/gggdtparser/langs/default.py
+-rw-rw-rw-   0        0        0     3399 2023-05-30 08:20:26.000000 gggdtparser-0.0.9/gggdtparser/langs/en.py
+-rw-rw-rw-   0        0        0      703 2023-05-25 03:05:13.000000 gggdtparser-0.0.9/gggdtparser/langs/es.py
+-rw-rw-rw-   0        0        0      943 2023-05-25 03:05:13.000000 gggdtparser-0.0.9/gggdtparser/langs/fra.py
+-rw-rw-rw-   0        0        0      223 2023-05-30 08:08:07.000000 gggdtparser-0.0.9/gggdtparser/langs/hi.py
+-rw-rw-rw-   0        0        0      239 2023-05-30 06:33:25.000000 gggdtparser-0.0.9/gggdtparser/langs/ky.py
+-rw-rw-rw-   0        0        0      345 2023-05-30 07:58:49.000000 gggdtparser-0.0.9/gggdtparser/langs/mr.py
+-rw-rw-rw-   0        0        0      804 2023-05-30 07:50:28.000000 gggdtparser-0.0.9/gggdtparser/langs/ru.py
+-rw-rw-rw-   0        0        0      249 2023-05-30 07:52:16.000000 gggdtparser-0.0.9/gggdtparser/langs/rw.py
+-rw-rw-rw-   0        0        0      238 2023-05-30 08:00:58.000000 gggdtparser-0.0.9/gggdtparser/langs/si.py
+-rw-rw-rw-   0        0        0      230 2023-05-25 03:05:13.000000 gggdtparser-0.0.9/gggdtparser/langs/so.py
+-rw-rw-rw-   0        0        0      329 2023-05-30 07:55:53.000000 gggdtparser-0.0.9/gggdtparser/langs/sw.py
+-rw-rw-rw-   0        0        0      745 2023-05-25 03:05:13.000000 gggdtparser-0.0.9/gggdtparser/langs/swe.py
+-rw-rw-rw-   0        0        0      195 2023-05-30 08:05:09.000000 gggdtparser-0.0.9/gggdtparser/langs/tg.py
+-rw-rw-rw-   0        0        0      300 2023-05-30 08:05:26.000000 gggdtparser-0.0.9/gggdtparser/langs/tr.py
+-rw-rw-rw-   0        0        0      811 2023-05-30 07:48:04.000000 gggdtparser-0.0.9/gggdtparser/langs/uk.py
+-rw-rw-rw-   0        0        0      231 2023-05-30 06:37:38.000000 gggdtparser-0.0.9/gggdtparser/langs/ur.py
+-rw-rw-rw-   0        0        0      432 2023-05-25 03:05:13.000000 gggdtparser-0.0.9/gggdtparser/langs/vie.py
+-rw-rw-rw-   0        0        0      802 2023-05-25 03:05:13.000000 gggdtparser-0.0.9/gggdtparser/langs/zh.py
+-rw-rw-rw-   0        0        0      609 2023-05-25 03:05:13.000000 gggdtparser-0.0.9/gggdtparser/langs/zht.py
+drwxrwxrwx   0        0        0        0 2023-05-30 11:55:17.915197 gggdtparser-0.0.9/gggdtparser/test/
+-rw-rw-rw-   0        0        0    43437 2023-05-25 04:15:16.000000 gggdtparser-0.0.9/gggdtparser/test/__init__.py
+-rw-rw-rw-   0        0        0      112 2023-05-30 07:17:35.000000 gggdtparser-0.0.9/gggdtparser/test/_id.py
+-rw-rw-rw-   0        0        0      829 2023-04-20 08:57:23.000000 gggdtparser-0.0.9/gggdtparser/test/az.py
+-rw-rw-rw-   0        0        0      120 2023-05-30 08:08:48.000000 gggdtparser-0.0.9/gggdtparser/test/hi.py
+-rw-rw-rw-   0        0        0      118 2023-05-30 06:34:41.000000 gggdtparser-0.0.9/gggdtparser/test/ky.py
+-rw-rw-rw-   0        0        0      211 2023-05-30 07:59:04.000000 gggdtparser-0.0.9/gggdtparser/test/mr.py
+-rw-rw-rw-   0        0        0      117 2023-05-30 07:52:38.000000 gggdtparser-0.0.9/gggdtparser/test/ru.py
+-rw-rw-rw-   0        0        0      136 2023-05-30 07:52:38.000000 gggdtparser-0.0.9/gggdtparser/test/rw.py
+-rw-rw-rw-   0        0        0      129 2023-05-30 08:01:52.000000 gggdtparser-0.0.9/gggdtparser/test/si.py
+-rw-rw-rw-   0        0        0      158 2023-05-30 07:56:38.000000 gggdtparser-0.0.9/gggdtparser/test/sw.py
+-rw-rw-rw-   0        0        0      129 2023-05-30 08:06:27.000000 gggdtparser-0.0.9/gggdtparser/test/tg.py
+-rw-rw-rw-   0        0        0      127 2023-05-30 08:03:19.000000 gggdtparser-0.0.9/gggdtparser/test/tr.py
+-rw-rw-rw-   0        0        0      178 2023-05-30 07:49:10.000000 gggdtparser-0.0.9/gggdtparser/test/uk.py
+-rw-rw-rw-   0        0        0      140 2023-05-30 06:39:37.000000 gggdtparser-0.0.9/gggdtparser/test/ur.py
+-rw-rw-rw-   0        0        0      570 2023-05-30 11:54:30.000000 gggdtparser-0.0.9/gggdtparser/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-30 11:55:17.877297 gggdtparser-0.0.9/gggdtparser.egg-info/
+-rw-rw-rw-   0        0        0     3404 2023-05-30 11:55:17.000000 gggdtparser-0.0.9/gggdtparser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1191 2023-05-30 11:55:17.000000 gggdtparser-0.0.9/gggdtparser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 11:55:17.000000 gggdtparser-0.0.9/gggdtparser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-30 11:55:17.000000 gggdtparser-0.0.9/gggdtparser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      775 2023-05-30 11:55:17.917191 gggdtparser-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      165 2023-03-27 07:16:57.000000 gggdtparser-0.0.9/setup.py
```

### Comparing `gggdtparser-0.0.8/LICENSE` & `gggdtparser-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.0.8/PKG-INFO` & `gggdtparser-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gggdtparser
-Version: 0.0.8
+Version: 0.0.9
 Summary: 通用、便捷、准确的字符串时间解析工具
 Home-page: https://github.com/kusen-alpha/gggdtparser
 Author: kusen
 Author-email: hu1194542196@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/kusen-alpha/gggdtparser/issues
 Project-URL: Documentation, https://github.com/kusen-alpha/gggdtparser/blob/master/README.md
```

### Comparing `gggdtparser-0.0.8/README.md` & `gggdtparser-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.0.8/gggdtparser/dtconfigs.py` & `gggdtparser-0.0.9/gggdtparser/dtconfigs.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.0.8/gggdtparser/dtparser.py` & `gggdtparser-0.0.9/gggdtparser/dtparser.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.0.8/gggdtparser/langs/de.py` & `gggdtparser-0.0.9/gggdtparser/langs/de.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.0.8/gggdtparser/langs/default.py` & `gggdtparser-0.0.9/gggdtparser/langs/default.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.0.8/gggdtparser/langs/en.py` & `gggdtparser-0.0.9/gggdtparser/langs/en.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.0.8/gggdtparser/langs/es.py` & `gggdtparser-0.0.9/gggdtparser/langs/es.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.0.8/gggdtparser/langs/fra.py` & `gggdtparser-0.0.9/gggdtparser/langs/fra.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.0.8/gggdtparser/langs/ru.py` & `gggdtparser-0.0.9/gggdtparser/langs/ru.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.0.8/gggdtparser/langs/swe.py` & `gggdtparser-0.0.9/gggdtparser/langs/swe.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.0.8/gggdtparser/langs/uk.py` & `gggdtparser-0.0.9/gggdtparser/langs/uk.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.0.8/gggdtparser/langs/zh.py` & `gggdtparser-0.0.9/gggdtparser/langs/zh.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.0.8/gggdtparser/langs/zht.py` & `gggdtparser-0.0.9/gggdtparser/langs/zht.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.0.8/gggdtparser/test/__init__.py` & `gggdtparser-0.0.9/gggdtparser/test/__init__.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.0.8/gggdtparser/test/az.py` & `gggdtparser-0.0.9/gggdtparser/test/az.py`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.0.8/gggdtparser/utils.py` & `gggdtparser-0.0.9/gggdtparser/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,9 +15,10 @@
     """
     if not sort_list:
         return d
     if sys.version_info >= (3, 9):
         return {k: d[k] for k in sort_list if k in d} | {k: d[
             k] for k in d if k not in sort_list}
     else:
-        return {k: d[k] for k in sort_list if k in d}.update({k: d[
-            k] for k in d if k not in sort_list})
+        _d = {k: d[k] for k in sort_list if k in d}
+        _d.update({k: d[k] for k in d if k not in sort_list})
+        return _d
```

### Comparing `gggdtparser-0.0.8/gggdtparser.egg-info/PKG-INFO` & `gggdtparser-0.0.9/gggdtparser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gggdtparser
-Version: 0.0.8
+Version: 0.0.9
 Summary: 通用、便捷、准确的字符串时间解析工具
 Home-page: https://github.com/kusen-alpha/gggdtparser
 Author: kusen
 Author-email: hu1194542196@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/kusen-alpha/gggdtparser/issues
 Project-URL: Documentation, https://github.com/kusen-alpha/gggdtparser/blob/master/README.md
```

### Comparing `gggdtparser-0.0.8/gggdtparser.egg-info/SOURCES.txt` & `gggdtparser-0.0.9/gggdtparser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.0.8/setup.cfg` & `gggdtparser-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 6767 6474 7061 7273 6572 0d0a   = gggdtparser..
-00000020: 7665 7273 696f 6e20 3d20 302e 302e 380d  version = 0.0.8.
+00000020: 7665 7273 696f 6e20 3d20 302e 302e 390d  version = 0.0.9.
 00000030: 0a61 7574 686f 7220 3d20 6b75 7365 6e0d  .author = kusen.
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 6875 3131 3934 3534 3231 3936 4071 712e  hu1194542196@qq.
 00000060: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000070: 203d 20cd a8d3 c3a1 a2b1 e3bd dda1 a2d7   = .............
 00000080: bcc8 b7b5 c4d7 d6b7 fbb4 aeca b1bc e4bd  ................
 00000090: e2ce f6b9 a4be df0d 0a6c 6f6e 675f 6465  .........long_de
```

