# Comparing `tmp/nonebot_plugin_access_control-0.4.2.tar.gz` & `tmp/nonebot_plugin_access_control-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_access_control-0.4.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_access_control-0.4.3.tar", max compression
```

## Comparing `nonebot_plugin_access_control-0.4.2.tar` & `nonebot_plugin_access_control-0.4.3.tar`

### file list

```diff
@@ -1,54 +1,53 @@
--rw-r--r--   0        0        0     1085 2022-07-09 13:18:24.594000 nonebot_plugin_access_control-0.4.2/LICENSE
--rw-r--r--   0        0        0      989 2023-05-27 05:12:28.758404 nonebot_plugin_access_control-0.4.2/pyproject.toml
--rw-r--r--   0        0        0    18871 2023-05-27 05:36:59.303416 nonebot_plugin_access_control-0.4.2/README.MD
--rw-r--r--   0        0        0      979 2023-05-27 05:06:59.270663 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/__init__.py
--rw-r--r--   0        0        0     2046 2023-02-14 08:42:38.604899 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/access_control.py
--rw-r--r--   0        0        0      579 2023-02-14 06:33:57.256438 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/config.py
--rw-r--r--   0        0        0      248 2023-02-14 09:17:25.623083 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/errors.py
--rw-r--r--   0        0        0     2363 2023-02-14 08:19:30.714606 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/event_bus.py
--rw-r--r--   0        0        0    10443 2023-03-13 03:19:06.942840 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/matchers/__init__.py
--rw-r--r--   0        0        0     1005 2023-02-13 06:25:49.446680 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/matchers/handle_error.py
--rw-r--r--   0        0        0     3263 2023-02-14 08:59:49.704358 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/matchers/parser.py
--rw-r--r--   0        0        0     3693 2023-03-13 03:28:05.306313 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/migrations/875c4dd8c271_.py
--rw-r--r--   0        0        0      172 2023-03-13 03:19:06.944840 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/models/__init__.py
--rw-r--r--   0        0        0      461 2023-03-13 03:19:06.944840 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/models/permission.py
--rw-r--r--   0        0        0     1754 2023-03-13 03:19:06.945840 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/models/rate_limit.py
--rw-r--r--   0        0        0      119 2023-03-13 03:19:06.946840 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/plugin_data.py
--rw-r--r--   0        0        0      159 2023-02-13 07:58:33.466319 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/__init__.py
--rw-r--r--   0        0        0     6791 2023-05-27 05:06:59.271662 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/base.py
--rw-r--r--   0        0        0        0 2023-02-13 08:30:50.046295 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/impl/__init__.py
--rw-r--r--   0        0        0     8257 2023-03-13 03:19:06.946840 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/impl/permission.py
--rw-r--r--   0        0        0    11920 2023-05-27 05:28:53.341561 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/impl/rate_limit.py
--rw-r--r--   0        0        0       31 2023-02-13 07:07:23.516417 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/interface/__init__.py
--rw-r--r--   0        0        0     1968 2023-02-14 08:42:38.593900 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/interface/base.py
--rw-r--r--   0        0        0     1630 2023-02-14 07:23:00.750461 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/interface/permission.py
--rw-r--r--   0        0        0     1948 2023-05-27 05:06:59.272662 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/interface/rate_limit.py
--rw-r--r--   0        0        0      680 2023-02-13 08:40:31.774931 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/interface/service.py
--rw-r--r--   0        0        0      334 2023-02-13 07:59:53.174308 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/interface/subservice_owner.py
--rw-r--r--   0        0        0      882 2023-02-14 07:23:39.399678 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/methods.py
--rw-r--r--   0        0        0     2392 2023-02-14 07:30:48.027513 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/nonebot.py
--rw-r--r--   0        0        0       36 2023-02-14 06:34:31.631671 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/permission/__init__.py
--rw-r--r--   0        0        0      224 2023-02-14 07:59:38.644831 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/permission/permission.py
--rw-r--r--   0        0        0      907 2023-02-13 07:53:46.438693 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/plugin.py
--rw-r--r--   0        0        0       74 2023-05-27 05:06:59.273662 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/rate_limit/__init__.py
--rw-r--r--   0        0        0      318 2023-02-14 09:29:28.023174 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/rate_limit/rule.py
--rw-r--r--   0        0        0      181 2023-05-27 05:06:59.273662 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/rate_limit/token.py
--rw-r--r--   0        0        0      840 2023-02-13 07:54:44.558096 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/subservice.py
--rw-r--r--   0        0        0     1645 2023-02-14 06:59:06.539473 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/subservice_owner.py
--rw-r--r--   0        0        0       26 2023-02-20 02:15:08.129834 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/subject/__init__.py
--rw-r--r--   0        0        0      501 2023-03-11 14:39:35.434800 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/subject/extractor/__init__.py
--rw-r--r--   0        0        0      681 2023-02-20 02:03:55.940528 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/subject/extractor/base.py
--rw-r--r--   0        0        0     1443 2023-02-20 02:14:18.251076 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/subject/extractor/union.py
--rw-r--r--   0        0        0        0 2022-12-10 06:08:59.849075 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/utils/__init__.py
--rw-r--r--   0        0        0      531 2023-03-13 03:19:06.948840 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/utils/session.py
--rw-r--r--   0        0        0      425 2023-02-20 04:34:52.815055 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/utils/superuser.py
--rw-r--r--   0        0        0     1015 2022-12-10 06:23:22.420137 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/utils/tree.py
--rw-r--r--   0        0        0      234 2023-02-20 02:14:18.267077 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control_kaiheila/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 01:49:13.238000 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control_kaiheila/subject/__init__.py
--rw-r--r--   0        0        0     1398 2023-03-11 14:39:35.402797 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control_kaiheila/subject/extractor/__init__.py
--rw-r--r--   0        0        0      324 2023-02-20 02:14:18.246077 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control_onebot/__init__.py
--rw-r--r--   0        0        0        0 2023-02-20 01:49:13.238036 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control_onebot/subject/__init__.py
--rw-r--r--   0        0        0       88 2023-02-20 02:08:23.170135 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control_onebot/subject/extractor/__init__.py
--rw-r--r--   0        0        0     1936 2023-03-11 14:39:35.464798 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control_onebot/subject/extractor/v11.py
--rw-r--r--   0        0        0     2350 2023-03-11 14:39:35.403797 nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control_onebot/subject/extractor/v12.py
--rw-r--r--   0        0        0    19263 1970-01-01 00:00:00.000000 nonebot_plugin_access_control-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1085 2022-07-09 13:18:24.594000 nonebot_plugin_access_control-0.4.3/LICENSE
+-rw-r--r--   0        0        0      989 2023-05-30 02:56:51.111023 nonebot_plugin_access_control-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0    18867 2023-05-30 02:55:49.596711 nonebot_plugin_access_control-0.4.3/README.MD
+-rw-r--r--   0        0        0     1632 2023-05-30 02:55:20.700817 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/__init__.py
+-rw-r--r--   0        0        0      579 2023-05-30 02:34:22.187998 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/config.py
+-rw-r--r--   0        0        0      248 2023-02-14 09:17:25.623083 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/errors.py
+-rw-r--r--   0        0        0     2363 2023-02-14 08:19:30.714606 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/event_bus.py
+-rw-r--r--   0        0        0    10443 2023-03-13 03:19:06.942840 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/matchers/__init__.py
+-rw-r--r--   0        0        0     1005 2023-02-13 06:25:49.446680 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/matchers/handle_error.py
+-rw-r--r--   0        0        0     3263 2023-02-14 08:59:49.704358 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/matchers/parser.py
+-rw-r--r--   0        0        0     3693 2023-03-13 03:28:05.306313 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/migrations/875c4dd8c271_.py
+-rw-r--r--   0        0        0      172 2023-03-13 03:19:06.944840 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/models/__init__.py
+-rw-r--r--   0        0        0      461 2023-03-13 03:19:06.944840 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/models/permission.py
+-rw-r--r--   0        0        0     1754 2023-03-13 03:19:06.945840 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/models/rate_limit.py
+-rw-r--r--   0        0        0      119 2023-03-13 03:19:06.946840 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/plugin_data.py
+-rw-r--r--   0        0        0      159 2023-02-13 07:58:33.466319 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/__init__.py
+-rw-r--r--   0        0        0     8872 2023-05-30 02:51:57.690417 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/base.py
+-rw-r--r--   0        0        0        0 2023-02-13 08:30:50.046295 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/impl/__init__.py
+-rw-r--r--   0        0        0     8257 2023-03-13 03:19:06.946840 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/impl/permission.py
+-rw-r--r--   0        0        0    11920 2023-05-27 05:28:53.341561 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/impl/rate_limit.py
+-rw-r--r--   0        0        0       31 2023-02-13 07:07:23.516417 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/interface/__init__.py
+-rw-r--r--   0        0        0     2089 2023-05-30 02:47:39.681782 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/interface/base.py
+-rw-r--r--   0        0        0     1630 2023-02-14 07:23:00.750461 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/interface/permission.py
+-rw-r--r--   0        0        0     1948 2023-05-27 05:06:59.272662 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/interface/rate_limit.py
+-rw-r--r--   0        0        0      680 2023-02-13 08:40:31.774931 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/interface/service.py
+-rw-r--r--   0        0        0      334 2023-02-13 07:59:53.174308 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/interface/subservice_owner.py
+-rw-r--r--   0        0        0      882 2023-02-14 07:23:39.399678 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/methods.py
+-rw-r--r--   0        0        0     2392 2023-02-14 07:30:48.027513 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/nonebot.py
+-rw-r--r--   0        0        0       36 2023-02-14 06:34:31.631671 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/permission/__init__.py
+-rw-r--r--   0        0        0      224 2023-02-14 07:59:38.644831 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/permission/permission.py
+-rw-r--r--   0        0        0      907 2023-02-13 07:53:46.438693 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/plugin.py
+-rw-r--r--   0        0        0       74 2023-05-27 05:06:59.273662 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/rate_limit/__init__.py
+-rw-r--r--   0        0        0      318 2023-02-14 09:29:28.023174 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/rate_limit/rule.py
+-rw-r--r--   0        0        0      181 2023-05-27 05:06:59.273662 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/rate_limit/token.py
+-rw-r--r--   0        0        0      840 2023-02-13 07:54:44.558096 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/subservice.py
+-rw-r--r--   0        0        0     1645 2023-02-14 06:59:06.539473 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/subservice_owner.py
+-rw-r--r--   0        0        0       26 2023-02-20 02:15:08.129834 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/subject/__init__.py
+-rw-r--r--   0        0        0      501 2023-03-11 14:39:35.434800 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/subject/extractor/__init__.py
+-rw-r--r--   0        0        0      681 2023-02-20 02:03:55.940528 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/subject/extractor/base.py
+-rw-r--r--   0        0        0     1443 2023-02-20 02:14:18.251076 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/subject/extractor/union.py
+-rw-r--r--   0        0        0        0 2022-12-10 06:08:59.849075 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/utils/__init__.py
+-rw-r--r--   0        0        0      531 2023-03-13 03:19:06.948840 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/utils/session.py
+-rw-r--r--   0        0        0      425 2023-02-20 04:34:52.815055 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/utils/superuser.py
+-rw-r--r--   0        0        0     1015 2022-12-10 06:23:22.420137 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/utils/tree.py
+-rw-r--r--   0        0        0      234 2023-02-20 02:14:18.267077 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control_kaiheila/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-20 01:49:13.238000 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control_kaiheila/subject/__init__.py
+-rw-r--r--   0        0        0     1398 2023-03-11 14:39:35.402797 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control_kaiheila/subject/extractor/__init__.py
+-rw-r--r--   0        0        0      324 2023-02-20 02:14:18.246077 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control_onebot/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-20 01:49:13.238036 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control_onebot/subject/__init__.py
+-rw-r--r--   0        0        0       88 2023-02-20 02:08:23.170135 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control_onebot/subject/extractor/__init__.py
+-rw-r--r--   0        0        0     1936 2023-03-11 14:39:35.464798 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control_onebot/subject/extractor/v11.py
+-rw-r--r--   0        0        0     2350 2023-03-11 14:39:35.403797 nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control_onebot/subject/extractor/v12.py
+-rw-r--r--   0        0        0    19260 1970-01-01 00:00:00.000000 nonebot_plugin_access_control-0.4.3/PKG-INFO
```

### Comparing `nonebot_plugin_access_control-0.4.2/LICENSE` & `nonebot_plugin_access_control-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.2/pyproject.toml` & `nonebot_plugin_access_control-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-access-control"
-version = "0.4.2"
+version = "0.4.3"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 license = "MIT"
 readme = "README.MD"
 repository = "https://github.com/ssttkkl/nonebot-plugin-access-control"
 packages = [
     { include = "nonebot_plugin_access_control", from = "src" },
```

### Comparing `nonebot_plugin_access_control-0.4.2/README.MD` & `nonebot_plugin_access_control-0.4.3/README.MD`

 * *Files 2% similar despite different names*

```diff
@@ -38,17 +38,15 @@
 
 ### 主体
 
 #### 概念
 
 当我们对用户进行权限控制时，我们想要的是针对拥有某种同样身份的所有用户进行配置，而不是对每一个具体用户分别配置。因此，我们引入主体的概念。 **主体（Subject）代表了拥有某种同样身份的用户的集合，也是设置权限的基本单位。** 当我们说用户具有某个主体，也就是说用户在该主体所代表的集合内。换句话说，主体就是一个用户所具有的身份。
 
-一个用户通常拥有多个主体。举个例子：QQ上群组G的用户U发送了一条消息，该用户同时具有“用户U”、“群组G成员”、“QQ用户”、“Bot用户”这几个主体。同时QQ上群组G的用户V也发送了一条消息，该用户该用户同时具有“用户V”、“群组G成员”、“QQ用户”、“Bot用户”这几个主体。用户拥有的所有主体，按照规模从小到大排序，呈现如下图的逐层包含关系：
-
-![](docs/img/1.svg)
+一个用户通常拥有多个主体。举个例子：QQ上群组G的用户U发送了一条消息，该用户同时具有“用户U”、“群组G成员”、“QQ用户”、“Bot用户”这几个主体。同时QQ上群组G的用户V也发送了一条消息，该用户该用户同时具有“用户V”、“群组G成员”、“QQ用户”、“Bot用户”这几个主体。
 
 当设置权限时，我们直接针对一个主体进行设置。当鉴权时，我们对用户的所有主体**按优先级从高到低的顺序**，逐一检查是否设置了权限。一旦检查到某个主体设置了权限，就以该主体设置的权限作为该用户的权限。
 
 回到上面的例子，假设我们对主体”群组G“禁用服务，但是对主体”用户V“启用服务。则用户U在群组G内将无法使用服务，但是用户V在群组G内可以使用。
 
 在插件使用中，我们用一个字符串表示主体，例如`qq:12345678`表示QQ用户12345678、`qq:g87654321`表示QQ群组87654321。
 
@@ -230,15 +228,15 @@
 require("nonebot_plugin_access_control")
 
 from nonebot_plugin_access_control.service import create_plugin_service
 
 plugin_service = create_plugin_service("nonebot_plugin_ac_demo")
 ```
 
-3. 通过PluginService.create_subservice创建SubService实例。调用`Service.patch_matcher()`应用至Matcher
+3. 通过PluginService.create_subservice创建SubService实例。调用`Service.patch_matcher()`应用至Matcher，或在事件处理函数上应用装饰器`Service.patch_handle()`。（二选一）
 
 ```python
 group1 = plugin_service.create_subservice("group1")
 
 a_matcher = on_command('a')
 a_service = group1.create_subservice('a')
 a_service.patch_matcher(a_matcher)
@@ -257,20 +255,21 @@
 @b_matcher.handle()
 async def _(matcher: Matcher):
     await matcher.send("b")
 
 
 c_matcher = on_command('c')
 c_service = plugin_service.create_subservice('c')
-c_service.patch_matcher(c_matcher)
 
 
 @c_matcher.handle()
+@c_service.patch_handler()  # 必须在 @c_matcher.handle() 之下
 async def _(matcher: Matcher):
     await matcher.send("c")
+
 ```
 
 插件服务的结构如下所示：
 
 ![](docs/img/2.svg)
 
 4. 通过指令配置服务权限
```

#### html2text {}

```diff
@@ -5,16 +5,15 @@
 æ¯æéå¶åä¸ç¨æ·å¨ä¸å®æ¶é´åçæä»¤è°ç¨æ¬¡æ° - [x]
 å¯¹æªééæä»¶æä¾**æä»¶çº§å«**çæ§å¶æ¯æ - æä»¶éé - [x]
 æ¯æ**åè½çº§å«**çç»ç²åº¦æ§å¶ - [x]
 æ¯æå¯¹æéå¼å³ç­äºä»¶è¿è¡è®¢é ## ä½¿ç¨ ### ä¸»ä½ #### æ¦å¿µ
 å½æä»¬å¯¹ç¨æ·è¿è¡æéæ§å¶æ¶ï¼æä»¬æ³è¦çæ¯éå¯¹æ¥ææç§åæ ·èº«ä»½çææç¨æ·è¿è¡éç½®ï¼èä¸æ¯å¯¹æ¯ä¸ä¸ªå·ä½ç¨æ·åå«éç½®ãå æ­¤ï¼æä»¬å¼å¥ä¸»ä½çæ¦å¿µã
 **ä¸»ä½ï¼Subjectï¼ä»£è¡¨äºæ¥ææç§åæ ·èº«ä»½çç¨æ·çéåï¼ä¹æ¯è®¾ç½®æéçåºæ¬åä½ã**
 å½æä»¬è¯´ç¨æ·å·ææä¸ªä¸»ä½ï¼ä¹å°±æ¯è¯´ç¨æ·å¨è¯¥ä¸»ä½æä»£è¡¨çéååãæ¢å¥è¯è¯´ï¼ä¸»ä½å°±æ¯ä¸ä¸ªç¨æ·æå·æçèº«ä»½ã
-ä¸ä¸ªç¨æ·éå¸¸æ¥æå¤ä¸ªä¸»ä½ãä¸¾ä¸ªä¾å­ï¼QQä¸ç¾¤ç»Gçç¨æ·Uåéäºä¸æ¡æ¶æ¯ï¼è¯¥ç¨æ·åæ¶å·æâç¨æ·Uâãâç¾¤ç»GæåâãâQQç¨æ·âãâBotç¨æ·âè¿å ä¸ªä¸»ä½ãåæ¶QQä¸ç¾¤ç»Gçç¨æ·Vä¹åéäºä¸æ¡æ¶æ¯ï¼è¯¥ç¨æ·è¯¥ç¨æ·åæ¶å·æâç¨æ·Vâãâç¾¤ç»GæåâãâQQç¨æ·âãâBotç¨æ·âè¿å ä¸ªä¸»ä½ãç¨æ·æ¥æçææä¸»ä½ï¼æç§è§æ¨¡ä»å°å°å¤§æåºï¼åç°å¦ä¸å¾çéå±åå«å³ç³»ï¼
-![](docs/img/1.svg)
+ä¸ä¸ªç¨æ·éå¸¸æ¥æå¤ä¸ªä¸»ä½ãä¸¾ä¸ªä¾å­ï¼QQä¸ç¾¤ç»Gçç¨æ·Uåéäºä¸æ¡æ¶æ¯ï¼è¯¥ç¨æ·åæ¶å·æâç¨æ·Uâãâç¾¤ç»GæåâãâQQç¨æ·âãâBotç¨æ·âè¿å ä¸ªä¸»ä½ãåæ¶QQä¸ç¾¤ç»Gçç¨æ·Vä¹åéäºä¸æ¡æ¶æ¯ï¼è¯¥ç¨æ·è¯¥ç¨æ·åæ¶å·æâç¨æ·Vâãâç¾¤ç»GæåâãâQQç¨æ·âãâBotç¨æ·âè¿å ä¸ªä¸»ä½ã
 å½è®¾ç½®æéæ¶ï¼æä»¬ç´æ¥éå¯¹ä¸ä¸ªä¸»ä½è¿è¡è®¾ç½®ãå½é´ææ¶ï¼æä»¬å¯¹ç¨æ·çææä¸»ä½**æä¼åçº§ä»é«å°ä½çé¡ºåº**ï¼éä¸æ£æ¥æ¯å¦è®¾ç½®äºæéãä¸æ¦æ£æ¥å°æä¸ªä¸»ä½è®¾ç½®äºæéï¼å°±ä»¥è¯¥ä¸»ä½è®¾ç½®çæéä½ä¸ºè¯¥ç¨æ·çæéã
 åå°ä¸é¢çä¾å­ï¼åè®¾æä»¬å¯¹ä¸»ä½âç¾¤ç»Gâç¦ç¨æå¡ï¼ä½æ¯å¯¹ä¸»ä½âç¨æ·Vâå¯ç¨æå¡ãåç¨æ·Uå¨ç¾¤ç»Gåå°æ æ³ä½¿ç¨æå¡ï¼ä½æ¯ç¨æ·Vå¨ç¾¤ç»Gåå¯ä»¥ä½¿ç¨ã
 å¨æä»¶ä½¿ç¨ä¸­ï¼æä»¬ç¨ä¸ä¸ªå­ç¬¦ä¸²è¡¨ç¤ºä¸»ä½ï¼ä¾å¦`qq:
 12345678`è¡¨ç¤ºQQç¨æ·12345678ã`qq:g87654321`è¡¨ç¤ºQQç¾¤ç»87654321ã
 æä»¬çº¦å®ï¼`all`è¡¨ç¤ºææç¨æ·ã`superuser`è¡¨ç¤ºè¶çº§ç¨æ·ã`<å¹³å°å>`è¡¨ç¤ºæææ­¤å¹³å°çç¨æ·ã`<åè®®å>`è¡¨ç¤ºæææ­¤åè®®çç¨æ·ãææä¸å¹³å°ç¸å³çä¸»ä½åä»¥`<å¹³å°å>:
 `å¼å¤´ãææä¸åè®®ç¸å³çä¸»ä½åä»¥`<åè®®å>:`å¼å¤´ã
 åééå¨çä¸»ä½å®ä¹å¦ä¸ï¼ - [OneBot V11](docs/onebot_v11.md) -
@@ -108,24 +107,26 @@
 nonebot_plugin_ac_demo/matcher_demo.py) 1.
 åå»ºä¸ä¸ªåä¸ºnonebot_plugin_ac_demoçæä»¶ 2.
 éè¿create_plugin_serviceå½æ°åå»ºä¸ä¸ªPluginServiceå®ä¾ï¼æ³¨æåæ°å¿é¡»ä¸ºæä»¶ååï¼
 ```python from nonebot import require require("nonebot_plugin_access_control")
 from nonebot_plugin_access_control.service import create_plugin_service
 plugin_service = create_plugin_service("nonebot_plugin_ac_demo") ``` 3.
 éè¿PluginService.create_subserviceåå»ºSubServiceå®ä¾ãè°ç¨`Service.patch_matcher
-()`åºç¨è³Matcher ```python group1 = plugin_service.create_subservice
+()`åºç¨è³Matcherï¼æå¨äºä»¶å¤çå½æ°ä¸åºç¨è£é¥°å¨`Service.patch_handle
+()`ãï¼äºéä¸ï¼ ```python group1 = plugin_service.create_subservice
 ("group1") a_matcher = on_command('a') a_service = group1.create_subservice
 ('a') a_service.patch_matcher(a_matcher) @a_matcher.handle() async def _
 (matcher: Matcher): await matcher.send("a") b_matcher = on_command('b')
 b_service = group1.create_subservice('b') b_service.patch_matcher(b_matcher)
 @b_matcher.handle() async def _(matcher: Matcher): await matcher.send("b")
 c_matcher = on_command('c') c_service = plugin_service.create_subservice('c')
-c_service.patch_matcher(c_matcher) @c_matcher.handle() async def _(matcher:
-Matcher): await matcher.send("c") ``` æä»¶æå¡çç»æå¦ä¸æç¤ºï¼ ![]
-(docs/img/2.svg) 4. éè¿æä»¤éç½®æå¡æé
+@c_matcher.handle() @c_service.patch_handler() # å¿é¡»å¨ @c_matcher.handle()
+ä¹ä¸ async def _(matcher: Matcher): await matcher.send("c") ```
+æä»¶æå¡çç»æå¦ä¸æç¤ºï¼ ![](docs/img/2.svg) 4.
+éè¿æä»¤éç½®æå¡æé
 æ§è¡ä¸é¢çæä»¤åï¼ææç¨æ·å°æ æ³è°ç¨æä»¤`/a`ä¸`/b` ``` /ac
 permission deny --sbj all --srv nonebot_plugin_ac_demo.group1 ```
 æ§è¡ä¸é¢çæä»¤åï¼QQç¨æ·12345678å°æ æ³è°ç¨æä»¤`/a` ``` /ac
 permission deny --sbj qq:12345678 --srv nonebot_plugin_ac_demo.group1.a ```
 æ§è¡ä¸é¢çæä»¤åï¼QQç¾¤ç»87654321çææç¨æ·å°æ æ³è°ç¨é¤`/
 c`ä»¥å¤çä»»ä½æä»¤ ``` /ac permission deny --sbj qq:g87654321 --srv
 nonebot_plugin_ac_demo /ac permission allow --sbj qq:g87654321 --srv
```

### Comparing `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/access_control.py` & `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,48 @@
-from typing import Type, Dict
+from nonebot import require
 
-import nonebot
-from nonebot import get_driver, logger, Bot
-from nonebot.exception import IgnoredException
-from nonebot.internal.adapter import Event
-from nonebot.internal.matcher import Matcher
-from nonebot.message import run_preprocessor
+require("nonebot_plugin_datastore")
+require("nonebot_plugin_apscheduler")
 
 from .config import conf
-from .errors import RateLimitedError, PermissionDeniedError
-from .service import Service, get_nonebot_service
+from .service import get_nonebot_service
 
-_matcher_service_mapping: Dict[Type[Matcher], Service] = {}
+from importlib import import_module
+from nonebot import logger, get_driver, get_loaded_plugins
 
+supported_modules = {
+    "OneBot V11": "nonebot_plugin_access_control_onebot",
+    "OneBot V12": "nonebot_plugin_access_control_onebot",
+    "Kaiheila": "nonebot_plugin_access_control_kaiheila",
+}
+
+loaded_modules = []
+
+driver = get_driver()
+for adapter in driver._adapters:
+    if adapter in supported_modules:
+        import_module(supported_modules[adapter])
+        loaded_modules.append(adapter)
+        logger.debug(f"Succeed to loaded plugin for {adapter}")
 
-def patch_matcher(matcher: Type[Matcher], service: Service) -> Type[Matcher]:
-    _matcher_service_mapping[matcher] = service
-    logger.debug(f"patched {matcher}  (with service {service.qualified_name})")
-    return matcher
-
-
-@run_preprocessor
-async def check(matcher: Matcher, bot: Bot, event: Event):
-    service = _matcher_service_mapping.get(type(matcher), None)
-    if service is None:
-        return
-
-    try:
-        await service.check(bot, event, throw_on_fail=True)
-    except PermissionDeniedError:
-        if conf.access_control_reply_on_permission_denied:
-            await matcher.send(conf.access_control_reply_on_permission_denied)
-        raise IgnoredException("permission denied (by nonebot_plugin_access_control)")
-    except RateLimitedError:
-        if conf.access_control_reply_on_rate_limited:
-            await matcher.send(conf.access_control_reply_on_rate_limited)
-        raise IgnoredException("rate limited (by nonebot_plugin_access_control)")
-
+if len(loaded_modules):
+    logger.success(f"Loaded plugin for: {', '.join(loaded_modules)}")
 
 if conf.access_control_auto_patch_enabled:
     @get_driver().on_startup
     def _():
         nonebot_service = get_nonebot_service()
 
-        for plugin in nonebot.get_loaded_plugins():
+        patched_plugins = []
+
+        for plugin in get_loaded_plugins():
             if plugin.name == 'nonebot_plugin_access_control' or plugin.name in conf.access_control_auto_patch_ignore:
                 continue
 
             service = nonebot_service.get_or_create_plugin_service(plugin.name)
             if service.auto_created:
                 for matcher in plugin.matcher:
-                    patch_matcher(matcher, service)
+                    service.patch_matcher(matcher)
+                patched_plugins.append(plugin)
+
+        logger.opt(colors=True).success(
+            "auto patched plugin(s): " + ', '.join([f'<y>{p.name}</y>' for p in patched_plugins]))
```

### Comparing `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/config.py` & `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/event_bus.py` & `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/event_bus.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/matchers/__init__.py` & `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/matchers/handle_error.py` & `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/matchers/handle_error.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/matchers/parser.py` & `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/matchers/parser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/migrations/875c4dd8c271_.py` & `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/migrations/875c4dd8c271_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/models/rate_limit.py` & `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/models/rate_limit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/base.py` & `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 from abc import ABC
 from datetime import timedelta
-from typing import Optional, Generic, TypeVar, Type, AsyncGenerator
+from functools import wraps
+from typing import Optional, Generic, TypeVar, Type, AsyncGenerator, Dict
 
-from nonebot import Bot
+from nonebot import Bot, logger
+from nonebot.exception import IgnoredException
 from nonebot.internal.adapter import Event
-from nonebot.internal.matcher import Matcher
+from nonebot.internal.matcher import Matcher, current_bot, current_event, current_matcher
+from nonebot.message import run_preprocessor
 
 from .impl.permission import ServicePermissionImpl
 from .impl.rate_limit import ServiceRateLimitImpl
 from .interface import IService
 from .interface.rate_limit import IRateLimitToken
 from .permission import Permission
 from .rate_limit import RateLimitRule
+from ..config import conf
 from ..errors import AccessControlError, PermissionDeniedError, RateLimitedError
 from ..event_bus import T_Listener
 from ..subject import extract_subjects
 
 T_ParentService = TypeVar('T_ParentService', bound=Optional["Service"], covariant=True)
 T_ChildService = TypeVar('T_ChildService', bound="Service", covariant=True)
 
 
 class Service(Generic[T_ParentService, T_ChildService],
               IService["Service", T_ParentService, T_ChildService],
               ABC):
+    _matcher_service_mapping: Dict[Type[Matcher], "Service"] = {}
+
     def __init__(self):
         self._permission_impl = ServicePermissionImpl[Service](self)
         self._rate_limit_impl = ServiceRateLimitImpl[Service](self)
 
     def __repr__(self):
         return self.qualified_name
 
@@ -46,16 +52,45 @@
     def get_child(self, name: str) -> Optional["Service"]:
         for s in self.children:
             if s.name == name:
                 return s
         return None
 
     def patch_matcher(self, matcher: Type[Matcher]) -> Type[Matcher]:
-        from ..access_control import patch_matcher
-        return patch_matcher(matcher, self)
+        self._matcher_service_mapping[matcher] = self
+        logger.debug(f"patched {matcher}  (with service {self.qualified_name})")
+        return matcher
+
+    def patch_handler(self, retire_on_throw: bool = False):
+        def decorator(func):
+            @wraps(func)
+            async def wrapped_func(*args, **kwargs):
+                bot = current_bot.get()
+                event = current_event.get()
+
+                if not await self.check(bot, event, acquire_rate_limit_token=False):
+                    raise PermissionDeniedError()
+
+                token = await self.acquire_token_for_rate_limit(bot, event)
+                if token is None:
+                    raise RateLimitedError()
+
+                matcher = current_matcher.get()
+                matcher.state["ac_token"] = token
+
+                try:
+                    return await func(*args, **kwargs)
+                except BaseException as e:
+                    if retire_on_throw:
+                        await token.retire()
+                    raise e
+
+            return wrapped_func
+
+        return decorator
 
     async def check(self, bot: Bot, event: Event,
                     *, acquire_rate_limit_token: bool = True,
                     throw_on_fail: bool = False) -> bool:
         subjects = extract_subjects(bot, event)
         return await self.check_by_subject(*subjects,
                                            acquire_rate_limit_token=acquire_rate_limit_token,
@@ -149,7 +184,25 @@
 
     async def acquire_token_for_rate_limit_by_subjects(self, *subject: str) -> Optional[IRateLimitToken]:
         return await self._rate_limit_impl.acquire_token_for_rate_limit_by_subjects(*subject)
 
     @classmethod
     async def clear_rate_limit_tokens(cls):
         return await ServiceRateLimitImpl.clear_rate_limit_tokens()
+
+
+@run_preprocessor
+async def check(matcher: Matcher, bot: Bot, event: Event):
+    service = Service._matcher_service_mapping.get(type(matcher), None)
+    if service is None:
+        return
+
+    try:
+        await service.check(bot, event, throw_on_fail=True)
+    except PermissionDeniedError:
+        if conf.access_control_reply_on_permission_denied:
+            await matcher.send(conf.access_control_reply_on_permission_denied)
+        raise IgnoredException("permission denied (by nonebot_plugin_access_control)")
+    except RateLimitedError:
+        if conf.access_control_reply_on_rate_limited:
+            await matcher.send(conf.access_control_reply_on_rate_limited)
+        raise IgnoredException("rate limited (by nonebot_plugin_access_control)")
```

### Comparing `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/impl/permission.py` & `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/impl/permission.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/impl/rate_limit.py` & `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/impl/rate_limit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/interface/base.py` & `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/interface/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,14 +42,18 @@
         raise NotImplementedError()
 
     @abstractmethod
     def patch_matcher(self, matcher: Type[Matcher]) -> Type[Matcher]:
         raise NotImplementedError()
 
     @abstractmethod
+    def patch_handler(self, retire_on_throw: bool = False):
+        raise NotImplementedError()
+
+    @abstractmethod
     async def check(self, bot: Bot, event: Event,
                     *, acquire_rate_limit_token: bool = True,
                     throw_on_fail: bool = False) -> bool:
         raise NotImplementedError()
 
     @abstractmethod
     async def check_by_subject(self, *subjects: str,
```

### Comparing `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/interface/permission.py` & `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/interface/permission.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/interface/rate_limit.py` & `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/interface/rate_limit.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/interface/service.py` & `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/interface/service.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/methods.py` & `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/methods.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/nonebot.py` & `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/nonebot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/plugin.py` & `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/plugin.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/subservice.py` & `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/subservice.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/service/subservice_owner.py` & `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/service/subservice_owner.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/subject/extractor/base.py` & `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/subject/extractor/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/subject/extractor/union.py` & `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/subject/extractor/union.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/utils/session.py` & `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/utils/session.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control/utils/tree.py` & `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control/utils/tree.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control_kaiheila/subject/extractor/__init__.py` & `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control_kaiheila/subject/extractor/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control_onebot/subject/extractor/v11.py` & `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control_onebot/subject/extractor/v11.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.2/src/nonebot_plugin_access_control_onebot/subject/extractor/v12.py` & `nonebot_plugin_access_control-0.4.3/src/nonebot_plugin_access_control_onebot/subject/extractor/v12.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_access_control-0.4.2/PKG-INFO` & `nonebot_plugin_access_control-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-access-control
-Version: 0.4.2
+Version: 0.4.3
 Summary: 
 Home-page: https://github.com/ssttkkl/nonebot-plugin-access-control
 License: MIT
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -59,17 +59,15 @@
 
 ### 主体
 
 #### 概念
 
 当我们对用户进行权限控制时，我们想要的是针对拥有某种同样身份的所有用户进行配置，而不是对每一个具体用户分别配置。因此，我们引入主体的概念。 **主体（Subject）代表了拥有某种同样身份的用户的集合，也是设置权限的基本单位。** 当我们说用户具有某个主体，也就是说用户在该主体所代表的集合内。换句话说，主体就是一个用户所具有的身份。
 
-一个用户通常拥有多个主体。举个例子：QQ上群组G的用户U发送了一条消息，该用户同时具有“用户U”、“群组G成员”、“QQ用户”、“Bot用户”这几个主体。同时QQ上群组G的用户V也发送了一条消息，该用户该用户同时具有“用户V”、“群组G成员”、“QQ用户”、“Bot用户”这几个主体。用户拥有的所有主体，按照规模从小到大排序，呈现如下图的逐层包含关系：
-
-![](docs/img/1.svg)
+一个用户通常拥有多个主体。举个例子：QQ上群组G的用户U发送了一条消息，该用户同时具有“用户U”、“群组G成员”、“QQ用户”、“Bot用户”这几个主体。同时QQ上群组G的用户V也发送了一条消息，该用户该用户同时具有“用户V”、“群组G成员”、“QQ用户”、“Bot用户”这几个主体。
 
 当设置权限时，我们直接针对一个主体进行设置。当鉴权时，我们对用户的所有主体**按优先级从高到低的顺序**，逐一检查是否设置了权限。一旦检查到某个主体设置了权限，就以该主体设置的权限作为该用户的权限。
 
 回到上面的例子，假设我们对主体”群组G“禁用服务，但是对主体”用户V“启用服务。则用户U在群组G内将无法使用服务，但是用户V在群组G内可以使用。
 
 在插件使用中，我们用一个字符串表示主体，例如`qq:12345678`表示QQ用户12345678、`qq:g87654321`表示QQ群组87654321。
 
@@ -251,15 +249,15 @@
 require("nonebot_plugin_access_control")
 
 from nonebot_plugin_access_control.service import create_plugin_service
 
 plugin_service = create_plugin_service("nonebot_plugin_ac_demo")
 ```
 
-3. 通过PluginService.create_subservice创建SubService实例。调用`Service.patch_matcher()`应用至Matcher
+3. 通过PluginService.create_subservice创建SubService实例。调用`Service.patch_matcher()`应用至Matcher，或在事件处理函数上应用装饰器`Service.patch_handle()`。（二选一）
 
 ```python
 group1 = plugin_service.create_subservice("group1")
 
 a_matcher = on_command('a')
 a_service = group1.create_subservice('a')
 a_service.patch_matcher(a_matcher)
@@ -278,20 +276,21 @@
 @b_matcher.handle()
 async def _(matcher: Matcher):
     await matcher.send("b")
 
 
 c_matcher = on_command('c')
 c_service = plugin_service.create_subservice('c')
-c_service.patch_matcher(c_matcher)
 
 
 @c_matcher.handle()
+@c_service.patch_handler()  # 必须在 @c_matcher.handle() 之下
 async def _(matcher: Matcher):
     await matcher.send("c")
+
 ```
 
 插件服务的结构如下所示：
 
 ![](docs/img/2.svg)
 
 4. 通过指令配置服务权限
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-access-control Version: 0.4.2
+Metadata-Version: 2.1 Name: nonebot-plugin-access-control Version: 0.4.3
 Summary: Home-page: https://github.com/ssttkkl/nonebot-plugin-access-control
 License: MIT Author: ssttkkl Author-email: huang.wen.long@hotmail.com Requires-
 Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: nonebot-
 plugin-apscheduler (>=0.2.0,<0.3.0) Requires-Dist: nonebot-plugin-datastore
@@ -16,16 +16,15 @@
 æ¯æéå¶åä¸ç¨æ·å¨ä¸å®æ¶é´åçæä»¤è°ç¨æ¬¡æ° - [x]
 å¯¹æªééæä»¶æä¾**æä»¶çº§å«**çæ§å¶æ¯æ - æä»¶éé - [x]
 æ¯æ**åè½çº§å«**çç»ç²åº¦æ§å¶ - [x]
 æ¯æå¯¹æéå¼å³ç­äºä»¶è¿è¡è®¢é ## ä½¿ç¨ ### ä¸»ä½ #### æ¦å¿µ
 å½æä»¬å¯¹ç¨æ·è¿è¡æéæ§å¶æ¶ï¼æä»¬æ³è¦çæ¯éå¯¹æ¥ææç§åæ ·èº«ä»½çææç¨æ·è¿è¡éç½®ï¼èä¸æ¯å¯¹æ¯ä¸ä¸ªå·ä½ç¨æ·åå«éç½®ãå æ­¤ï¼æä»¬å¼å¥ä¸»ä½çæ¦å¿µã
 **ä¸»ä½ï¼Subjectï¼ä»£è¡¨äºæ¥ææç§åæ ·èº«ä»½çç¨æ·çéåï¼ä¹æ¯è®¾ç½®æéçåºæ¬åä½ã**
 å½æä»¬è¯´ç¨æ·å·ææä¸ªä¸»ä½ï¼ä¹å°±æ¯è¯´ç¨æ·å¨è¯¥ä¸»ä½æä»£è¡¨çéååãæ¢å¥è¯è¯´ï¼ä¸»ä½å°±æ¯ä¸ä¸ªç¨æ·æå·æçèº«ä»½ã
-ä¸ä¸ªç¨æ·éå¸¸æ¥æå¤ä¸ªä¸»ä½ãä¸¾ä¸ªä¾å­ï¼QQä¸ç¾¤ç»Gçç¨æ·Uåéäºä¸æ¡æ¶æ¯ï¼è¯¥ç¨æ·åæ¶å·æâç¨æ·Uâãâç¾¤ç»GæåâãâQQç¨æ·âãâBotç¨æ·âè¿å ä¸ªä¸»ä½ãåæ¶QQä¸ç¾¤ç»Gçç¨æ·Vä¹åéäºä¸æ¡æ¶æ¯ï¼è¯¥ç¨æ·è¯¥ç¨æ·åæ¶å·æâç¨æ·Vâãâç¾¤ç»GæåâãâQQç¨æ·âãâBotç¨æ·âè¿å ä¸ªä¸»ä½ãç¨æ·æ¥æçææä¸»ä½ï¼æç§è§æ¨¡ä»å°å°å¤§æåºï¼åç°å¦ä¸å¾çéå±åå«å³ç³»ï¼
-![](docs/img/1.svg)
+ä¸ä¸ªç¨æ·éå¸¸æ¥æå¤ä¸ªä¸»ä½ãä¸¾ä¸ªä¾å­ï¼QQä¸ç¾¤ç»Gçç¨æ·Uåéäºä¸æ¡æ¶æ¯ï¼è¯¥ç¨æ·åæ¶å·æâç¨æ·Uâãâç¾¤ç»GæåâãâQQç¨æ·âãâBotç¨æ·âè¿å ä¸ªä¸»ä½ãåæ¶QQä¸ç¾¤ç»Gçç¨æ·Vä¹åéäºä¸æ¡æ¶æ¯ï¼è¯¥ç¨æ·è¯¥ç¨æ·åæ¶å·æâç¨æ·Vâãâç¾¤ç»GæåâãâQQç¨æ·âãâBotç¨æ·âè¿å ä¸ªä¸»ä½ã
 å½è®¾ç½®æéæ¶ï¼æä»¬ç´æ¥éå¯¹ä¸ä¸ªä¸»ä½è¿è¡è®¾ç½®ãå½é´ææ¶ï¼æä»¬å¯¹ç¨æ·çææä¸»ä½**æä¼åçº§ä»é«å°ä½çé¡ºåº**ï¼éä¸æ£æ¥æ¯å¦è®¾ç½®äºæéãä¸æ¦æ£æ¥å°æä¸ªä¸»ä½è®¾ç½®äºæéï¼å°±ä»¥è¯¥ä¸»ä½è®¾ç½®çæéä½ä¸ºè¯¥ç¨æ·çæéã
 åå°ä¸é¢çä¾å­ï¼åè®¾æä»¬å¯¹ä¸»ä½âç¾¤ç»Gâç¦ç¨æå¡ï¼ä½æ¯å¯¹ä¸»ä½âç¨æ·Vâå¯ç¨æå¡ãåç¨æ·Uå¨ç¾¤ç»Gåå°æ æ³ä½¿ç¨æå¡ï¼ä½æ¯ç¨æ·Vå¨ç¾¤ç»Gåå¯ä»¥ä½¿ç¨ã
 å¨æä»¶ä½¿ç¨ä¸­ï¼æä»¬ç¨ä¸ä¸ªå­ç¬¦ä¸²è¡¨ç¤ºä¸»ä½ï¼ä¾å¦`qq:
 12345678`è¡¨ç¤ºQQç¨æ·12345678ã`qq:g87654321`è¡¨ç¤ºQQç¾¤ç»87654321ã
 æä»¬çº¦å®ï¼`all`è¡¨ç¤ºææç¨æ·ã`superuser`è¡¨ç¤ºè¶çº§ç¨æ·ã`<å¹³å°å>`è¡¨ç¤ºæææ­¤å¹³å°çç¨æ·ã`<åè®®å>`è¡¨ç¤ºæææ­¤åè®®çç¨æ·ãææä¸å¹³å°ç¸å³çä¸»ä½åä»¥`<å¹³å°å>:
 `å¼å¤´ãææä¸åè®®ç¸å³çä¸»ä½åä»¥`<åè®®å>:`å¼å¤´ã
 åééå¨çä¸»ä½å®ä¹å¦ä¸ï¼ - [OneBot V11](docs/onebot_v11.md) -
@@ -119,24 +118,26 @@
 nonebot_plugin_ac_demo/matcher_demo.py) 1.
 åå»ºä¸ä¸ªåä¸ºnonebot_plugin_ac_demoçæä»¶ 2.
 éè¿create_plugin_serviceå½æ°åå»ºä¸ä¸ªPluginServiceå®ä¾ï¼æ³¨æåæ°å¿é¡»ä¸ºæä»¶ååï¼
 ```python from nonebot import require require("nonebot_plugin_access_control")
 from nonebot_plugin_access_control.service import create_plugin_service
 plugin_service = create_plugin_service("nonebot_plugin_ac_demo") ``` 3.
 éè¿PluginService.create_subserviceåå»ºSubServiceå®ä¾ãè°ç¨`Service.patch_matcher
-()`åºç¨è³Matcher ```python group1 = plugin_service.create_subservice
+()`åºç¨è³Matcherï¼æå¨äºä»¶å¤çå½æ°ä¸åºç¨è£é¥°å¨`Service.patch_handle
+()`ãï¼äºéä¸ï¼ ```python group1 = plugin_service.create_subservice
 ("group1") a_matcher = on_command('a') a_service = group1.create_subservice
 ('a') a_service.patch_matcher(a_matcher) @a_matcher.handle() async def _
 (matcher: Matcher): await matcher.send("a") b_matcher = on_command('b')
 b_service = group1.create_subservice('b') b_service.patch_matcher(b_matcher)
 @b_matcher.handle() async def _(matcher: Matcher): await matcher.send("b")
 c_matcher = on_command('c') c_service = plugin_service.create_subservice('c')
-c_service.patch_matcher(c_matcher) @c_matcher.handle() async def _(matcher:
-Matcher): await matcher.send("c") ``` æä»¶æå¡çç»æå¦ä¸æç¤ºï¼ ![]
-(docs/img/2.svg) 4. éè¿æä»¤éç½®æå¡æé
+@c_matcher.handle() @c_service.patch_handler() # å¿é¡»å¨ @c_matcher.handle()
+ä¹ä¸ async def _(matcher: Matcher): await matcher.send("c") ```
+æä»¶æå¡çç»æå¦ä¸æç¤ºï¼ ![](docs/img/2.svg) 4.
+éè¿æä»¤éç½®æå¡æé
 æ§è¡ä¸é¢çæä»¤åï¼ææç¨æ·å°æ æ³è°ç¨æä»¤`/a`ä¸`/b` ``` /ac
 permission deny --sbj all --srv nonebot_plugin_ac_demo.group1 ```
 æ§è¡ä¸é¢çæä»¤åï¼QQç¨æ·12345678å°æ æ³è°ç¨æä»¤`/a` ``` /ac
 permission deny --sbj qq:12345678 --srv nonebot_plugin_ac_demo.group1.a ```
 æ§è¡ä¸é¢çæä»¤åï¼QQç¾¤ç»87654321çææç¨æ·å°æ æ³è°ç¨é¤`/
 c`ä»¥å¤çä»»ä½æä»¤ ``` /ac permission deny --sbj qq:g87654321 --srv
 nonebot_plugin_ac_demo /ac permission allow --sbj qq:g87654321 --srv
```

