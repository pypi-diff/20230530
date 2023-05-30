# Comparing `tmp/nonebot-plugin-alconna-0.6.0.tar.gz` & `tmp/nonebot-plugin-alconna-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-alconna-0.6.0.tar", last modified: Fri May 26 08:54:56 2023, max compression
+gzip compressed data, was "nonebot-plugin-alconna-0.6.1.tar", last modified: Tue May 30 09:10:17 2023, max compression
```

## Comparing `nonebot-plugin-alconna-0.6.0.tar` & `nonebot-plugin-alconna-0.6.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 nonebot-plugin-alconna-0.6.0/LICENSE
--rw-r--r--   0        0        0     1135 2023-05-26 08:51:03.270110 nonebot-plugin-alconna-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     8401 2023-05-18 16:06:27.910527 nonebot-plugin-alconna-0.6.0/README.md
--rw-r--r--   0        0        0     1241 2023-05-18 15:49:31.978140 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/__init__.py
--rw-r--r--   0        0        0      383 2023-05-11 04:41:26.166268 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/__init__.py
--rw-r--r--   0        0        0      523 2023-05-10 10:09:15.599546 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/bilibili.py
--rw-r--r--   0        0        0     1007 2023-05-10 10:09:15.573188 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/console.py
--rw-r--r--   0        0        0     1661 2023-05-10 10:09:15.609172 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/ding.py
--rw-r--r--   0        0        0     2141 2023-05-10 10:09:15.564123 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/feishu.py
--rw-r--r--   0        0        0      519 2023-05-10 10:09:15.541809 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/github.py
--rw-r--r--   0        0        0     1163 2023-05-10 10:09:15.636179 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/kook.py
--rw-r--r--   0        0        0      761 2023-05-10 10:09:15.651191 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/minecraft.py
--rw-r--r--   0        0        0     3155 2023-05-10 10:09:15.519983 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/mirai.py
--rw-r--r--   0        0        0     1088 2023-05-10 10:09:15.628175 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/ntchat.py
--rw-r--r--   0        0        0     3177 2023-05-10 10:09:15.618177 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/onebot11.py
--rw-r--r--   0        0        0     2517 2023-05-10 10:09:15.661217 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/onebot12.py
--rw-r--r--   0        0        0     3227 2023-05-10 10:09:15.529594 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/qqguild.py
--rw-r--r--   0        0        0     3126 2023-05-10 10:09:15.670151 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/telegram.py
--rw-r--r--   0        0        0      581 2023-05-10 10:09:15.553296 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/argv.py
--rw-r--r--   0        0        0      405 2023-05-10 09:00:57.054628 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/config.py
--rw-r--r--   0        0        0      180 2023-05-10 08:33:24.079951 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/consts.py
--rw-r--r--   0        0        0      109 2023-05-11 15:42:43.320472 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/i18n/.config.json
--rw-r--r--   0        0        0      301 2023-05-11 15:42:18.920450 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/i18n/en-US.json
--rw-r--r--   0        0        0      262 2023-05-11 15:42:18.885191 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/i18n/zh-CN.json
--rw-r--r--   0        0        0     2405 2023-05-18 15:49:32.019141 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/matcher.py
--rw-r--r--   0        0        0     1231 2023-05-18 15:49:32.003141 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/matcher.pyi
--rw-r--r--   0        0        0     1478 2023-05-26 08:51:03.247079 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/model.py
--rw-r--r--   0        0        0     3830 2023-05-26 08:51:03.151926 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/params.py
--rw-r--r--   0        0        0     9020 2023-05-26 08:51:03.217077 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/rule.py
--rw-r--r--   0        0        0     1967 2023-05-11 04:48:52.932671 nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/typings.py
--rw-r--r--   0        0        0     8484 1970-01-01 00:00:00.000000 nonebot-plugin-alconna-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524011 nonebot-plugin-alconna-0.6.1/LICENSE
+-rw-r--r--   0        0        0     1135 2023-05-30 09:08:03.666783 nonebot-plugin-alconna-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     8401 2023-05-18 16:06:27.910527 nonebot-plugin-alconna-0.6.1/README.md
+-rw-r--r--   0        0        0     1241 2023-05-18 15:49:31.978140 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/__init__.py
+-rw-r--r--   0        0        0      383 2023-05-11 04:41:26.166268 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/__init__.py
+-rw-r--r--   0        0        0      523 2023-05-10 10:09:15.599546 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/bilibili.py
+-rw-r--r--   0        0        0     1007 2023-05-10 10:09:15.573188 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/console.py
+-rw-r--r--   0        0        0     1661 2023-05-10 10:09:15.609172 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/ding.py
+-rw-r--r--   0        0        0     2141 2023-05-10 10:09:15.564123 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/feishu.py
+-rw-r--r--   0        0        0      519 2023-05-10 10:09:15.541809 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/github.py
+-rw-r--r--   0        0        0     1163 2023-05-10 10:09:15.636179 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/kook.py
+-rw-r--r--   0        0        0      761 2023-05-10 10:09:15.651191 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/minecraft.py
+-rw-r--r--   0        0        0     3155 2023-05-10 10:09:15.519983 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/mirai.py
+-rw-r--r--   0        0        0     1088 2023-05-10 10:09:15.628175 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/ntchat.py
+-rw-r--r--   0        0        0     3177 2023-05-10 10:09:15.618177 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/onebot11.py
+-rw-r--r--   0        0        0     2517 2023-05-10 10:09:15.661217 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/onebot12.py
+-rw-r--r--   0        0        0     3227 2023-05-10 10:09:15.529594 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/qqguild.py
+-rw-r--r--   0        0        0     3126 2023-05-10 10:09:15.670151 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/telegram.py
+-rw-r--r--   0        0        0      581 2023-05-10 10:09:15.553296 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/argv.py
+-rw-r--r--   0        0        0      405 2023-05-10 09:00:57.054628 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/config.py
+-rw-r--r--   0        0        0      180 2023-05-10 08:33:24.079951 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/consts.py
+-rw-r--r--   0        0        0      109 2023-05-11 15:42:43.320472 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/i18n/.config.json
+-rw-r--r--   0        0        0      301 2023-05-11 15:42:18.920450 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/i18n/en-US.json
+-rw-r--r--   0        0        0      262 2023-05-11 15:42:18.885191 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/i18n/zh-CN.json
+-rw-r--r--   0        0        0     2277 2023-05-30 09:08:03.646906 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/matcher.py
+-rw-r--r--   0        0        0     1093 2023-05-30 09:08:03.613798 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/matcher.pyi
+-rw-r--r--   0        0        0     1478 2023-05-26 08:51:03.247079 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/model.py
+-rw-r--r--   0        0        0     3830 2023-05-26 08:51:03.151926 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/params.py
+-rw-r--r--   0        0        0     8721 2023-05-30 09:08:03.602783 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/rule.py
+-rw-r--r--   0        0        0     2092 2023-05-30 09:08:03.637783 nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/typings.py
+-rw-r--r--   0        0        0     8484 1970-01-01 00:00:00.000000 nonebot-plugin-alconna-0.6.1/PKG-INFO
```

### Comparing `nonebot-plugin-alconna-0.6.0/LICENSE` & `nonebot-plugin-alconna-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.6.0/pyproject.toml` & `nonebot-plugin-alconna-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-alconna"
-version = "0.6.0"
+version = "0.6.1"
 description = "Alconna Adapter for Nonebot"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0rc4",
     "arclet-alconna<2.0.0, >=1.7.7",
```

### Comparing `nonebot-plugin-alconna-0.6.0/README.md` & `nonebot-plugin-alconna-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/__init__.py` & `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/bilibili.py` & `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/bilibili.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/console.py` & `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/console.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/ding.py` & `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/ding.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/feishu.py` & `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/feishu.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/github.py` & `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/github.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/kook.py` & `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/kook.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/minecraft.py` & `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/minecraft.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/mirai.py` & `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/mirai.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/ntchat.py` & `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/ntchat.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/onebot11.py` & `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/onebot11.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/onebot12.py` & `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/onebot12.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/qqguild.py` & `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/qqguild.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/adapters/telegram.py` & `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/adapters/telegram.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/argv.py` & `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/argv.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/matcher.py` & `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/matcher.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 from __future__ import annotations
 
-from typing import Callable, Awaitable
-
 from arclet.alconna import Alconna, command_manager
 from arclet.alconna.tools import AlconnaString
 from nonebot.matcher import Matcher
-from nonebot.adapters import Message
 from nonebot.plugin.on import on_message
 from nonebot.rule import Rule
 from nonebot.typing import T_RuleChecker
 
 from .rule import alconna
 from .model import CompConfig
-from .typings import OutputType
+from .typings import TConvert
 
 
 def on_alconna(
     command: Alconna | str,
     rule: Rule | T_RuleChecker | None = None,
     skip_for_unmatch: bool = True,
     auto_send_output: bool = False,
-    output_converter: Callable[[OutputType, str], Message | Awaitable[Message]] | None = None,
+    output_converter: TConvert | None = None,
     aliases: set[str | tuple[str, ...]] | None = None,
     comp_config: CompConfig | None = None,
     *args,
     _depth: int = 0,
     **kwargs,
 ) -> type[Matcher]:
     """注册一个消息事件响应器，并且当消息由指定 Alconna 解析并传出有效结果时响应。
@@ -46,15 +43,15 @@
         state: 默认 state
     """
     if isinstance(command, str):
         command = AlconnaString(command)
     if aliases and command.command:
         command_manager.delete(command)
         aliases.add(str(command.command))
-        command.command = "(" + "|".join(aliases) + ")"
+        command.command = "re:(" + "|".join(aliases) + ")"
         command._hash = command._calc_hash()
         command_manager.register(command)
     return on_message(
         alconna(
             command,
             skip_for_unmatch,
             auto_send_output,
```

### Comparing `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/matcher.pyi` & `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/matcher.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 from __future__ import annotations
 
 from datetime import datetime, timedelta
-from typing import Awaitable, Callable
 
-from arclet.alconna import Alconna, Arparma
-from nonebot.adapters import Message
+from arclet.alconna import Alconna
 from nonebot.dependencies import Dependent
 from nonebot.matcher import Matcher
 from nonebot.permission import Permission
 from nonebot.rule import Rule
 from nonebot.typing import T_Handler, T_PermissionChecker, T_RuleChecker, T_State
-from nonebot_plugin_alconna.typings import OutputType
+from nonebot_plugin_alconna.typings import TConvert
 from nonebot_plugin_alconna.model import CompConfig
 
 
 def on_alconna(
     command: Alconna | str,
     rule: Rule | T_RuleChecker | None = None,
     skip_for_unmatch: bool = True,
     auto_send_output: bool = False,
-    output_converter: Callable[[OutputType, str], Message | Awaitable[Message]] | None = None,
+    output_converter: TConvert | None = None,
     aliases: set[str | tuple[str, ...]] | None = None,
     comp_config: CompConfig | None = None,
     permission: Permission | T_PermissionChecker | None = ...,
     *,
     handlers: list[T_Handler | Dependent] | None = ...,
     temp: bool = ...,
     expire_time: datetime | timedelta | None = ...,
```

### Comparing `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/model.py` & `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/model.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/params.py` & `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/params.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/rule.py` & `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/rule.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import asyncio
-from typing import Awaitable, Callable, ClassVar, Optional, Union, Dict
+from typing import ClassVar, Optional, Union, Dict
 
 from arclet.alconna import (
     Alconna,
     Arparma,
     Args,
     CompSession,
     AllParam,
@@ -22,48 +22,44 @@
 from nonebot.typing import T_State
 from nonebot.utils import is_coroutine_callable, run_sync
 from tarina import lang
 
 from .config import Config
 from .consts import ALCONNA_RESULT
 from .model import CommandResult, CompConfig
-from .typings import OutputType
+from .typings import TConvert
 
 
 class AlconnaRule:
     """检查消息字符串是否能够通过此 Alconna 命令。
 
     参数:
         command: Alconna 命令
         skip_for_unmatch: 是否在命令不匹配时跳过该响应
         auto_send_output: 是否自动发送输出信息并跳过响应
         output_converter: 输出信息字符串转换为 Message 方法
         comp_config: 自动补全配置
     """
 
-    default_converter: ClassVar[
-        Callable[[OutputType, str], Union[Message, Awaitable[Message]]]
-    ] = lambda _, x: Message(x)
+    default_converter: ClassVar[TConvert] = lambda _, x: Message(x)
 
     __slots__ = (
         "command",
         "skip",
         "auto_send",
         "output_converter",
         "comp_config",
     )
 
     def __init__(
         self,
         command: Alconna,
         skip_for_unmatch: bool = True,
         auto_send_output: bool = False,
-        output_converter: Optional[
-            Callable[[OutputType, str], Union[Message, Awaitable[Message]]]
-        ] = None,
+        output_converter: Optional[TConvert] = None,
         comp_config: Optional[CompConfig] = None,
     ):
         self.comp_config = comp_config
         try:
             global_config = get_driver().config
             config = Config.parse_obj(global_config)
             self.auto_send = auto_send_output or config.alconna_auto_send_output
@@ -206,25 +202,23 @@
             return event.get_message().__class__(text)
 
 
 def alconna(
     command: Alconna,
     skip_for_unmatch: bool = True,
     auto_send_output: bool = False,
-    output_converter: Optional[
-        Callable[[OutputType, str], Union[Message, Awaitable[Message]]]
-    ] = None,
+    output_converter: Optional[TConvert] = None,
     comp_config: Optional[CompConfig] = None,
 ) -> Rule:
     return Rule(
         AlconnaRule(
             command,
             skip_for_unmatch,
             auto_send_output,
             output_converter,
             comp_config,
         )
     )
 
 
-def set_output_converter(fn: Callable[[OutputType, str], Union[Message, Awaitable[Message]]]):
+def set_output_converter(fn: TConvert):
     AlconnaRule.default_converter = fn
```

### Comparing `nonebot-plugin-alconna-0.6.0/src/nonebot_plugin_alconna/typings.py` & `nonebot-plugin-alconna-0.6.1/src/nonebot_plugin_alconna/typings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
-from typing import Callable, Any, TypeVar, Generic, Literal
-from typing_extensions import ParamSpec
+from typing import Callable, Any, TypeVar, Generic, Literal, Awaitable, Union
+from typing_extensions import ParamSpec, TypeAlias
 from tarina import lang
 from nepattern import BasePattern, PatternModel, MatchFailed
-from nonebot.internal.adapter.message import MessageSegment
+from nonebot.internal.adapter.message import MessageSegment, Message
 
 TMS = TypeVar("TMS", bound=MessageSegment)
 P = ParamSpec("P")
 
 
 class SegmentPattern(BasePattern[TMS], Generic[TMS, P]):
     def __init__(
@@ -40,14 +40,15 @@
         return input_
 
     def __call__(self, *args: P.args, **kwargs: P.kwargs) -> TMS:
         return self.call(*args, **kwargs)  # type: ignore
 
 
 OutputType = Literal["help", "shortcut", "completion"]
+TConvert: TypeAlias = Callable[[OutputType, str], Union[Message, Awaitable[Message]]]
 
 
 def _isinstance(seg: MessageSegment, accepts: set[str]):
     return seg if seg.type.lower() in accepts else None
 
 
 def gen_unit(
```

### Comparing `nonebot-plugin-alconna-0.6.0/PKG-INFO` & `nonebot-plugin-alconna-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-alconna
-Version: 0.6.0
+Version: 0.6.1
 Summary: Alconna Adapter for Nonebot
 License: MIT
 Keywords: command,argparse,cli,alconna,nonebot
 Author-email: RF-Tar-Railt <rf_tar_railt@qq.com>
 Requires-Python: >=3.8
 Project-URL: repository, https://github.com/ArcletProject/nonebot-plugin-alconna
 Description-Content-Type: text/markdown
```

