# Comparing `tmp/orbit_component_base-0.99.1.tar.gz` & `tmp/orbit_component_base-0.99.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orbit_component_base-0.99.1.tar", max compression
+gzip compressed data, was "orbit_component_base-0.99.2.tar", max compression
```

## Comparing `orbit_component_base-0.99.1.tar` & `orbit_component_base-0.99.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1099 2023-05-30 10:22:19.434839 orbit_component_base-0.99.1/LICENSE.md
--rw-r--r--   0        0        0      307 2023-05-30 10:24:05.900452 orbit_component_base-0.99.1/README.md
--rw-r--r--   0        0        0      248 2023-05-26 21:23:29.392298 orbit_component_base-0.99.1/orbit_component_base/__init__.py
--rw-r--r--   0        0        0      698 2023-05-26 14:58:49.369068 orbit_component_base-0.99.1/orbit_component_base/plugin.py
--rw-r--r--   0        0        0     1020 2023-05-26 15:16:14.168223 orbit_component_base-0.99.1/orbit_component_base/schema/OrbitSessions.py
--rw-r--r--   0        0        0      343 2023-05-26 15:16:31.111878 orbit_component_base-0.99.1/orbit_component_base/schema/OrbitUsers.py
--rwxr-xr-x   0        0        0     3489 2023-05-26 15:35:41.416368 orbit_component_base-0.99.1/orbit_component_base/src/orbit_app.py
--rw-r--r--   0        0        0     6315 2023-05-26 15:07:46.174514 orbit_component_base-0.99.1/orbit_component_base/src/orbit_auth.py
--rw-r--r--   0        0        0     6348 2023-05-26 15:11:22.310156 orbit_component_base-0.99.1/orbit_component_base/src/orbit_config.py
--rw-r--r--   0        0        0     1232 2023-05-26 15:11:34.365912 orbit_component_base-0.99.1/orbit_component_base/src/orbit_database.py
--rw-r--r--   0        0        0     3749 2023-05-09 09:42:38.245588 orbit_component_base-0.99.1/orbit_component_base/src/orbit_decorators.py
--rw-r--r--   0        0        0      290 2023-03-24 17:01:29.910135 orbit_component_base-0.99.1/orbit_component_base/src/orbit_logger.py
--rw-r--r--   0        0        0      834 2023-05-26 15:11:48.925617 orbit_component_base-0.99.1/orbit_component_base/src/orbit_make_ssl.py
--rw-r--r--   0        0        0     8612 2023-05-26 15:12:25.840869 orbit_component_base-0.99.1/orbit_component_base/src/orbit_nql.py
--rw-r--r--   0        0        0     3534 2023-03-28 12:50:44.012670 orbit_component_base-0.99.1/orbit_component_base/src/orbit_nql_buffer.py
--rw-r--r--   0        0        0      895 2023-04-03 10:19:17.442215 orbit_component_base-0.99.1/orbit_component_base/src/orbit_nql_emitter.py
--rw-r--r--   0        0        0     4442 2023-05-23 12:28:15.559177 orbit_component_base-0.99.1/orbit_component_base/src/orbit_nql_session.py
--rw-r--r--   0        0        0     6409 2023-05-25 11:09:33.029380 orbit_component_base-0.99.1/orbit_component_base/src/orbit_orm.py
--rw-r--r--   0        0        0     2293 2023-05-26 21:23:57.215737 orbit_component_base-0.99.1/orbit_component_base/src/orbit_plugin.py
--rw-r--r--   0        0        0     1243 2023-05-26 16:04:04.125398 orbit_component_base-0.99.1/orbit_component_base/src/orbit_plugins.py
--rw-r--r--   0        0        0     2329 2023-05-26 15:13:02.796118 orbit_component_base-0.99.1/orbit_component_base/src/orbit_router.py
--rw-r--r--   0        0        0      629 2023-05-23 16:46:20.522320 orbit_component_base-0.99.1/orbit_component_base/src/orbit_shared.py
--rw-r--r--   0        0        0       21 2023-05-24 17:39:08.131348 orbit_component_base-0.99.1/orbit_component_base/src/orbit_version.py
--rw-r--r--   0        0        0       76 2023-05-26 15:02:23.180928 orbit_component_base-0.99.1/orbit_component_base/tests/test_main.py
--rw-r--r--   0        0        0      584 2023-05-30 10:25:13.534933 orbit_component_base-0.99.1/pyproject.toml
--rw-r--r--   0        0        0     1054 1970-01-01 00:00:00.000000 orbit_component_base-0.99.1/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-05-30 10:22:19.434839 orbit_component_base-0.99.2/LICENSE.md
+-rw-r--r--   0        0        0      307 2023-05-30 10:24:05.900452 orbit_component_base-0.99.2/README.md
+-rw-r--r--   0        0        0      248 2023-05-26 21:23:29.392298 orbit_component_base-0.99.2/orbit_component_base/__init__.py
+-rw-r--r--   0        0        0      698 2023-05-26 14:58:49.369068 orbit_component_base-0.99.2/orbit_component_base/plugin.py
+-rw-r--r--   0        0        0     1020 2023-05-26 15:16:14.168223 orbit_component_base-0.99.2/orbit_component_base/schema/OrbitSessions.py
+-rw-r--r--   0        0        0      343 2023-05-26 15:16:31.111878 orbit_component_base-0.99.2/orbit_component_base/schema/OrbitUsers.py
+-rwxr-xr-x   0        0        0     3489 2023-05-26 15:35:41.416368 orbit_component_base-0.99.2/orbit_component_base/src/orbit_app.py
+-rw-r--r--   0        0        0     6315 2023-05-26 15:07:46.174514 orbit_component_base-0.99.2/orbit_component_base/src/orbit_auth.py
+-rw-r--r--   0        0        0     6348 2023-05-26 15:11:22.310156 orbit_component_base-0.99.2/orbit_component_base/src/orbit_config.py
+-rw-r--r--   0        0        0     1232 2023-05-26 15:11:34.365912 orbit_component_base-0.99.2/orbit_component_base/src/orbit_database.py
+-rw-r--r--   0        0        0     3749 2023-05-09 09:42:38.245588 orbit_component_base-0.99.2/orbit_component_base/src/orbit_decorators.py
+-rw-r--r--   0        0        0      290 2023-03-24 17:01:29.910135 orbit_component_base-0.99.2/orbit_component_base/src/orbit_logger.py
+-rw-r--r--   0        0        0      834 2023-05-26 15:11:48.925617 orbit_component_base-0.99.2/orbit_component_base/src/orbit_make_ssl.py
+-rw-r--r--   0        0        0     8612 2023-05-26 15:12:25.840869 orbit_component_base-0.99.2/orbit_component_base/src/orbit_nql.py
+-rw-r--r--   0        0        0     3534 2023-03-28 12:50:44.012670 orbit_component_base-0.99.2/orbit_component_base/src/orbit_nql_buffer.py
+-rw-r--r--   0        0        0      895 2023-04-03 10:19:17.442215 orbit_component_base-0.99.2/orbit_component_base/src/orbit_nql_emitter.py
+-rw-r--r--   0        0        0     4442 2023-05-23 12:28:15.559177 orbit_component_base-0.99.2/orbit_component_base/src/orbit_nql_session.py
+-rw-r--r--   0        0        0     6409 2023-05-25 11:09:33.029380 orbit_component_base-0.99.2/orbit_component_base/src/orbit_orm.py
+-rw-r--r--   0        0        0     2293 2023-05-26 21:23:57.215737 orbit_component_base-0.99.2/orbit_component_base/src/orbit_plugin.py
+-rw-r--r--   0        0        0     1243 2023-05-26 16:04:04.125398 orbit_component_base-0.99.2/orbit_component_base/src/orbit_plugins.py
+-rw-r--r--   0        0        0     2329 2023-05-26 15:13:02.796118 orbit_component_base-0.99.2/orbit_component_base/src/orbit_router.py
+-rw-r--r--   0        0        0      629 2023-05-23 16:46:20.522320 orbit_component_base-0.99.2/orbit_component_base/src/orbit_shared.py
+-rw-r--r--   0        0        0       21 2023-05-24 17:39:08.131348 orbit_component_base-0.99.2/orbit_component_base/src/orbit_version.py
+-rw-r--r--   0        0        0       76 2023-05-26 15:02:23.180928 orbit_component_base-0.99.2/orbit_component_base/tests/test_main.py
+-rw-r--r--   0        0        0     1395 2023-05-30 11:29:01.775331 orbit_component_base-0.99.2/pyproject.toml
+-rw-r--r--   0        0        0     1593 1970-01-01 00:00:00.000000 orbit_component_base-0.99.2/PKG-INFO
```

### Comparing `orbit_component_base-0.99.1/LICENSE.md` & `orbit_component_base-0.99.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.1/orbit_component_base/plugin.py` & `orbit_component_base-0.99.2/orbit_component_base/plugin.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.1/orbit_component_base/schema/OrbitSessions.py` & `orbit_component_base-0.99.2/orbit_component_base/schema/OrbitSessions.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.1/orbit_component_base/src/orbit_app.py` & `orbit_component_base-0.99.2/orbit_component_base/src/orbit_app.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.1/orbit_component_base/src/orbit_auth.py` & `orbit_component_base-0.99.2/orbit_component_base/src/orbit_auth.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.1/orbit_component_base/src/orbit_config.py` & `orbit_component_base-0.99.2/orbit_component_base/src/orbit_config.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.1/orbit_component_base/src/orbit_database.py` & `orbit_component_base-0.99.2/orbit_component_base/src/orbit_database.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.1/orbit_component_base/src/orbit_decorators.py` & `orbit_component_base-0.99.2/orbit_component_base/src/orbit_decorators.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.1/orbit_component_base/src/orbit_make_ssl.py` & `orbit_component_base-0.99.2/orbit_component_base/src/orbit_make_ssl.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.1/orbit_component_base/src/orbit_nql.py` & `orbit_component_base-0.99.2/orbit_component_base/src/orbit_nql.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.1/orbit_component_base/src/orbit_nql_buffer.py` & `orbit_component_base-0.99.2/orbit_component_base/src/orbit_nql_buffer.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.1/orbit_component_base/src/orbit_nql_emitter.py` & `orbit_component_base-0.99.2/orbit_component_base/src/orbit_nql_emitter.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.1/orbit_component_base/src/orbit_nql_session.py` & `orbit_component_base-0.99.2/orbit_component_base/src/orbit_nql_session.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.1/orbit_component_base/src/orbit_orm.py` & `orbit_component_base-0.99.2/orbit_component_base/src/orbit_orm.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.1/orbit_component_base/src/orbit_plugin.py` & `orbit_component_base-0.99.2/orbit_component_base/src/orbit_plugin.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.1/orbit_component_base/src/orbit_plugins.py` & `orbit_component_base-0.99.2/orbit_component_base/src/orbit_plugins.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.1/orbit_component_base/src/orbit_router.py` & `orbit_component_base-0.99.2/orbit_component_base/src/orbit_router.py`

 * *Files identical despite different names*

### Comparing `orbit_component_base-0.99.1/orbit_component_base/src/orbit_shared.py` & `orbit_component_base-0.99.2/orbit_component_base/src/orbit_shared.py`

 * *Files identical despite different names*

