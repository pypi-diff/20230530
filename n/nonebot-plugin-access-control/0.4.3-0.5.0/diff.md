# Comparing `tmp/nonebot_plugin_access_control-0.4.3.tar.gz` & `tmp/nonebot_plugin_access_control-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_access_control-0.4.3.tar", max compression
+gzip compressed data, was "nonebot_plugin_access_control-0.5.0.tar", max compression
```

## Comparing `nonebot_plugin_access_control-0.4.3.tar` & `nonebot_plugin_access_control-0.5.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     1085 2022-07-09 13:18:24.594000 nonebot_plugin_access_control-0.4.3/LICENSE
--rw-r--r--   0        0        0      989 2023-05-30 02:56:51.111023 nonebot_plugin_access_control-0.4.3/pyproject.toml
--rw-r--r--   0        0        0    18867 2023-05-30 02:55:49.596711 nonebot_plugin_access_control-0.4.3/README.MD
--rw-r--r--   0        0        0     1632 2023-05-30 02:55:20.700817 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/__init__.py
--rw-r--r--   0        0        0      579 2023-05-30 02:34:22.187998 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/config.py
--rw-r--r--   0        0        0      248 2023-02-14 09:17:25.623083 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/errors.py
--rw-r--r--   0        0        0     2363 2023-02-14 08:19:30.714606 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/event_bus.py
--rw-r--r--   0        0        0    10443 2023-03-13 03:19:06.942840 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/matchers/__init__.py
--rw-r--r--   0        0        0     1005 2023-02-13 06:25:49.446680 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/matchers/handle_error.py
--rw-r--r--   0        0        0     3263 2023-02-14 08:59:49.704358 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/matchers/parser.py
--rw-r--r--   0        0        0     3693 2023-03-13 03:28:05.306313 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/migrations/875c4dd8c271_.py
--rw-r--r--   0        0        0      172 2023-03-13 03:19:06.944840 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/models/__init__.py
--rw-r--r--   0        0        0      461 2023-03-13 03:19:06.944840 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/models/permission.py
--rw-r--r--   0        0        0     1754 2023-03-13 03:19:06.945840 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/models/rate_limit.py
--rw-r--r--   0        0        0      119 2023-03-13 03:19:06.946840 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/plugin_data.py
--rw-r--r--   0        0        0      159 2023-02-13 07:58:33.466319 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/__init__.py
--rw-r--r--   0        0        0     8872 2023-05-30 02:51:57.690417 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/base.py
--rw-r--r--   0        0        0        0 2023-02-13 08:30:50.046295 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/impl/__init__.py
--rw-r--r--   0        0        0     8257 2023-03-13 03:19:06.946840 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/impl/permission.py
--rw-r--r--   0        0        0    11920 2023-05-27 05:28:53.341561 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/impl/rate_limit.py
--rw-r--r--   0        0        0       31 2023-02-13 07:07:23.516417 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/interface/__init__.py
--rw-r--r--   0        0        0     2089 2023-05-30 02:47:39.681782 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/interface/base.py
--rw-r--r--   0        0        0     1630 2023-02-14 07:23:00.750461 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/interface/permission.py
--rw-r--r--   0        0        0     1948 2023-05-27 05:06:59.272662 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/interface/rate_limit.py
--rw-r--r--   0        0        0      680 2023-02-13 08:40:31.774931 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/interface/service.py
--rw-r--r--   0        0        0      334 2023-02-13 07:59:53.174308 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/interface/subservice_owner.py
--rw-r--r--   0        0        0      882 2023-02-14 07:23:39.399678 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/methods.py
--rw-r--r--   0        0        0     2392 2023-02-14 07:30:48.027513 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/nonebot.py
--rw-r--r--   0        0        0       36 2023-02-14 06:34:31.631671 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/permission/__init__.py
--rw-r--r--   0        0        0      224 2023-02-14 07:59:38.644831 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/permission/permission.py
--rw-r--r--   0        0        0      907 2023-02-13 07:53:46.438693 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/plugin.py
--rw-r--r--   0        0        0       74 2023-05-27 05:06:59.273662 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/rate_limit/__init__.py
--rw-r--r--   0        0        0      318 2023-02-14 09:29:28.023174 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/rate_limit/rule.py
--rw-r--r--   0        0        0      181 2023-05-27 05:06:59.273662 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/rate_limit/token.py
--rw-r--r--   0        0        0      840 2023-02-13 07:54:44.558096 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/subservice.py
--rw-r--r--   0        0        0     1645 2023-02-14 06:59:06.539473 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/subservice_owner.py
--rw-r--r--   0        0        0       26 2023-02-20 02:15:08.129834 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/subject/__init__.py
--rw-r--r--   0        0        0      501 2023-03-11 14:39:35.434800 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/subject/extractor/__init__.py
--rw-r--r--   0        0        0      681 2023-02-20 02:03:55.940528 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/subject/extractor/base.py
--rw-r--r--   0        0        0     1443 2023-02-20 02:14:18.251076 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/subject/extractor/union.py
--rw-r--r--   0        0        0        0 2022-12-10 06:08:59.849075 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/utils/__init__.py
--rw-r--r--   0        0        0      531 2023-03-13 03:19:06.948840 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/utils/session.py
--rw-r--r--   0        0        0      425 2023-02-20 04:34:52.815055 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/utils/superuser.py
--rw-r--r--   0        0        0     1015 2022-12-10 06:23:22.420137 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/utils/tree.py
--rw-r--r--   0        0        0      234 2023-02-20 02:14:18.267077 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control_kaiheila/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 01:49:13.238000 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control_kaiheila/subject/__init__.py
--rw-r--r--   0        0        0     1398 2023-03-11 14:39:35.402797 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control_kaiheila/subject/extractor/__init__.py
--rw-r--r--   0        0        0      324 2023-02-20 02:14:18.246077 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control_onebot/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 01:49:13.238036 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control_onebot/subject/__init__.py
--rw-r--r--   0        0        0       88 2023-02-20 02:08:23.170135 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control_onebot/subject/extractor/__init__.py
--rw-r--r--   0        0        0     1936 2023-03-11 14:39:35.464798 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control_onebot/subject/extractor/v11.py
--rw-r--r--   0        0        0     2350 2023-03-11 14:39:35.403797 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control_onebot/subject/extractor/v12.py
--rw-r--r--   0        0        0    19260 1970-01-01 00:00:00.000000 nonebot_plugin_access_control-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     1085 2022-07-09 13:18:24.594000 nonebot_plugin_access_control-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1025 2023-05-30 09:06:13.807707 nonebot_plugin_access_control-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    18867 2023-05-30 02:55:49.596711 nonebot_plugin_access_control-0.5.0/README.MD
+-rw-r--r--   0        0        0     1689 2023-05-30 08:27:00.675053 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/__init__.py
+-rw-r--r--   0        0        0      579 2023-05-30 02:34:22.187998 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/config.py
+-rw-r--r--   0        0        0      248 2023-02-14 09:17:25.623083 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/errors.py
+-rw-r--r--   0        0        0     2363 2023-02-14 08:19:30.714606 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/event_bus.py
+-rw-r--r--   0        0        0    10443 2023-03-13 03:19:06.942840 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/matchers/__init__.py
+-rw-r--r--   0        0        0     1005 2023-02-13 06:25:49.446680 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/matchers/handle_error.py
+-rw-r--r--   0        0        0     3263 2023-02-14 08:59:49.704358 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/matchers/parser.py
+-rw-r--r--   0        0        0     3693 2023-03-13 03:28:05.306313 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/migrations/875c4dd8c271_.py
+-rw-r--r--   0        0        0      172 2023-03-13 03:19:06.944840 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/models/__init__.py
+-rw-r--r--   0        0        0      461 2023-03-13 03:19:06.944840 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/models/permission.py
+-rw-r--r--   0        0        0     1754 2023-03-13 03:19:06.945840 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/models/rate_limit.py
+-rw-r--r--   0        0        0      119 2023-03-13 03:19:06.946840 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/plugin_data.py
+-rw-r--r--   0        0        0      159 2023-02-13 07:58:33.466319 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/service/__init__.py
+-rw-r--r--   0        0        0     8872 2023-05-30 03:15:13.076049 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/service/base.py
+-rw-r--r--   0        0        0        0 2023-02-13 08:30:50.046295 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/service/impl/__init__.py
+-rw-r--r--   0        0        0     8257 2023-03-13 03:19:06.946840 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/service/impl/permission.py
+-rw-r--r--   0        0        0    11920 2023-05-27 05:28:53.341561 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/service/impl/rate_limit.py
+-rw-r--r--   0        0        0       31 2023-02-13 07:07:23.516417 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/service/interface/__init__.py
+-rw-r--r--   0        0        0     2089 2023-05-30 02:47:39.681782 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/service/interface/base.py
+-rw-r--r--   0        0        0     1630 2023-02-14 07:23:00.750461 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/service/interface/permission.py
+-rw-r--r--   0        0        0     1948 2023-05-27 05:06:59.272662 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/service/interface/rate_limit.py
+-rw-r--r--   0        0        0      680 2023-02-13 08:40:31.774931 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/service/interface/service.py
+-rw-r--r--   0        0        0      334 2023-02-13 07:59:53.174308 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/service/interface/subservice_owner.py
+-rw-r--r--   0        0        0      882 2023-02-14 07:23:39.399678 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/service/methods.py
+-rw-r--r--   0        0        0     2392 2023-02-14 07:30:48.027513 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/service/nonebot.py
+-rw-r--r--   0        0        0       36 2023-02-14 06:34:31.631671 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/service/permission/__init__.py
+-rw-r--r--   0        0        0      224 2023-02-14 07:59:38.644831 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/service/permission/permission.py
+-rw-r--r--   0        0        0      907 2023-02-13 07:53:46.438693 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/service/plugin.py
+-rw-r--r--   0        0        0       74 2023-05-27 05:06:59.273662 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/service/rate_limit/__init__.py
+-rw-r--r--   0        0        0      318 2023-02-14 09:29:28.023174 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/service/rate_limit/rule.py
+-rw-r--r--   0        0        0      181 2023-05-27 05:06:59.273662 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/service/rate_limit/token.py
+-rw-r--r--   0        0        0      840 2023-02-13 07:54:44.558096 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/service/subservice.py
+-rw-r--r--   0        0        0     1645 2023-02-14 06:59:06.539473 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/service/subservice_owner.py
+-rw-r--r--   0        0        0       26 2023-02-20 02:15:08.129834 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/subject/__init__.py
+-rw-r--r--   0        0        0      501 2023-03-11 14:39:35.434800 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/subject/extractor/__init__.py
+-rw-r--r--   0        0        0      681 2023-02-20 02:03:55.940528 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/subject/extractor/base.py
+-rw-r--r--   0        0        0     1443 2023-02-20 02:14:18.251076 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/subject/extractor/union.py
+-rw-r--r--   0        0        0        0 2022-12-10 06:08:59.849075 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/utils/__init__.py
+-rw-r--r--   0        0        0      531 2023-03-13 03:19:06.948840 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/utils/session.py
+-rw-r--r--   0        0        0      425 2023-02-20 04:34:52.815055 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/utils/superuser.py
+-rw-r--r--   0        0        0     1015 2022-12-10 06:23:22.420137 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/utils/tree.py
+-rw-r--r--   0        0        0      234 2023-02-20 02:14:18.267077 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control_kaiheila/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-20 01:49:13.238000 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control_kaiheila/subject/__init__.py
+-rw-r--r--   0        0        0     1398 2023-03-11 14:39:35.402797 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control_kaiheila/subject/extractor/__init__.py
+-rw-r--r--   0        0        0      324 2023-02-20 02:14:18.246077 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control_onebot/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-20 01:49:13.238036 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control_onebot/subject/__init__.py
+-rw-r--r--   0        0        0       88 2023-02-20 02:08:23.170135 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control_onebot/subject/extractor/__init__.py
+-rw-r--r--   0        0        0     1936 2023-03-11 14:39:35.464798 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control_onebot/subject/extractor/v11.py
+-rw-r--r--   0        0        0     2350 2023-03-11 14:39:35.403797 nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control_onebot/subject/extractor/v12.py
+-rw-r--r--   0        0        0    19260 1970-01-01 00:00:00.000000 nonebot_plugin_access_control-0.5.0/PKG-INFO
```

### Comparing `nonebot_plugin_access_control-0.4.3/LICENSE` & `nonebot_plugin_access_control-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.3/pyproject.toml` & `nonebot_plugin_access_control-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-access-control"
-version = "0.4.3"
+version = "0.5.0"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 license = "MIT"
 readme = "README.MD"
 repository = "https://github.com/ssttkkl/nonebot-plugin-access-control"
 packages = [
     { include = "nonebot_plugin_access_control", from = "src" },
@@ -19,14 +19,15 @@
 nonebot-plugin-apscheduler = "^0.2.0"
 shortuuid = "^1.0.11"
 
 
 [tool.poetry.group.dev.dependencies]
 nonebot-adapter-onebot = "^2.1.5"
 nonebot-adapter-kaiheila = "^0.1.0"
+nonebot-adapter-qqguild = "^0.2.2"
 nb-cli = "^1.0.5"
 asyncpg = "^0.27.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_access_control-0.4.3/README.MD` & `nonebot_plugin_access_control-0.5.0/README.MD`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/__init__.py` & `nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from importlib import import_module
 from nonebot import logger, get_driver, get_loaded_plugins
 
 supported_modules = {
     "OneBot V11": "nonebot_plugin_access_control_onebot",
     "OneBot V12": "nonebot_plugin_access_control_onebot",
     "Kaiheila": "nonebot_plugin_access_control_kaiheila",
+    "QQ Guild": "nonebot_plugin_access_control_qqguild"
 }
 
 loaded_modules = []
 
 driver = get_driver()
 for adapter in driver._adapters:
     if adapter in supported_modules:
```

### Comparing `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/config.py` & `nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/event_bus.py` & `nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/event_bus.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/matchers/__init__.py` & `nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/matchers/handle_error.py` & `nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/matchers/handle_error.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/matchers/parser.py` & `nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/matchers/parser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/migrations/875c4dd8c271_.py` & `nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/migrations/875c4dd8c271_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/models/rate_limit.py` & `nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/models/rate_limit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/base.py` & `nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/service/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/impl/permission.py` & `nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/service/impl/permission.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/impl/rate_limit.py` & `nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/service/impl/rate_limit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/interface/base.py` & `nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/service/interface/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/interface/permission.py` & `nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/service/interface/permission.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/interface/rate_limit.py` & `nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/service/interface/rate_limit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/interface/service.py` & `nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/service/interface/service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/methods.py` & `nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/service/methods.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/nonebot.py` & `nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/service/nonebot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/plugin.py` & `nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/service/plugin.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/subservice.py` & `nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/service/subservice.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/subservice_owner.py` & `nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/service/subservice_owner.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/subject/extractor/base.py` & `nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/subject/extractor/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/subject/extractor/union.py` & `nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/subject/extractor/union.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/utils/session.py` & `nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/utils/session.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/utils/tree.py` & `nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control/utils/tree.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control_kaiheila/subject/extractor/__init__.py` & `nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control_kaiheila/subject/extractor/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control_onebot/subject/extractor/v11.py` & `nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control_onebot/subject/extractor/v11.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control_onebot/subject/extractor/v12.py` & `nonebot_plugin_access_control-0.5.0/src/nonebot_plugin_access_control_onebot/subject/extractor/v12.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.3/PKG-INFO` & `nonebot_plugin_access_control-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-access-control
-Version: 0.4.3
+Version: 0.5.0
 Summary: 
 Home-page: https://github.com/ssttkkl/nonebot-plugin-access-control
 License: MIT
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-access-control Version: 0.4.3
+Metadata-Version: 2.1 Name: nonebot-plugin-access-control Version: 0.5.0
 Summary: Home-page: https://github.com/ssttkkl/nonebot-plugin-access-control
 License: MIT Author: ssttkkl Author-email: huang.wen.long@hotmail.com Requires-
 Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: nonebot-
 plugin-apscheduler (>=0.2.0,<0.3.0) Requires-Dist: nonebot-plugin-datastore
```

