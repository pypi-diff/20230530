# Comparing `tmp/nonebot_plugin_nagabus-0.1.4.post1.tar.gz` & `tmp/nonebot_plugin_nagabus-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nagabus-0.1.4.post1.tar", max compression
+gzip compressed data, was "nonebot_plugin_nagabus-0.1.5.tar", max compression
```

## Comparing `nonebot_plugin_nagabus-0.1.4.post1.tar` & `nonebot_plugin_nagabus-0.1.5.tar`

### file list

```diff
@@ -1,32 +1,35 @@
--rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448000 nonebot_plugin_nagabus-0.1.4.post1/LICENSE
--rw-r--r--   0        0        0     1131 2023-05-28 14:51:33.780852 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/__init__.py
--rw-r--r--   0        0        0      129 2023-05-27 04:29:09.849196 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/ac.py
--rw-r--r--   0        0        0     1197 2023-05-28 14:51:33.775850 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/config.py
--rw-r--r--   0        0        0        4 2023-05-26 13:11:24.775555 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/data/__init__.py
--rw-r--r--   0        0        0      116 2023-05-26 11:41:42.946553 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/data/base.py
--rw-r--r--   0        0        0      317 2023-05-26 11:41:42.956553 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/data/mjs.py
--rw-r--r--   0        0        0     1697 2023-05-27 07:16:52.720509 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/data/naga.py
--rw-r--r--   0        0        0      775 2023-05-26 11:41:42.960551 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/data/session.py
--rw-r--r--   0        0        0      713 2023-05-26 15:21:27.421204 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/data/utils/__init__.py
--rw-r--r--   0        0        0      761 2023-02-13 05:42:01.843000 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/data/utils/utc_datetime.py
--rw-r--r--   0        0        0       43 2023-05-28 14:51:33.785849 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/errors.py
--rw-r--r--   0        0        0       95 2023-05-28 01:19:53.575323 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/matchers/__init__.py
--rw-r--r--   0        0        0     2130 2023-05-28 01:19:53.557320 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/matchers/errors.py
--rw-r--r--   0        0        0     5612 2023-05-29 01:42:10.486630 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/matchers/naga_analyze.py
--rw-r--r--   0        0        0     2462 2023-05-28 01:19:53.563321 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/matchers/naga_statistic.py
--rw-r--r--   0        0        0     2278 2023-05-27 02:48:33.707764 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/migrations/24aec3c56623_.py
--rw-r--r--   0        0        0     1350 2023-05-27 07:17:07.623159 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py
--rw-r--r--   0        0        0     1009 2023-05-26 15:21:27.440185 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/mjs/__init__.py
--rw-r--r--   0        0        0      176 2023-05-25 15:39:25.419279 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/naga/__init__.py
--rw-r--r--   0        0        0     3758 2023-05-27 13:45:54.389899 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/naga/api.py
--rw-r--r--   0        0        0     3089 2023-05-29 12:30:46.127834 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/naga/fake_api.py
--rw-r--r--   0        0        0     1066 2023-05-27 02:48:01.485010 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/naga/model.py
--rw-r--r--   0        0        0    18823 2023-05-29 12:41:37.629257 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/naga/service.py
--rw-r--r--   0        0        0        0 2023-05-25 16:04:02.955709 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/utils/__init__.py
--rw-r--r--   0        0        0     1092 2023-05-25 16:06:56.701500 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/utils/integer.py
--rw-r--r--   0        0        0        0 2023-05-26 12:48:40.974521 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/utils/mapping.py
--rw-r--r--   0        0        0      101 2023-05-25 08:09:22.247000 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/utils/nonebot.py
--rw-r--r--   0        0        0       68 2023-05-26 15:50:47.559077 nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/utils/tz.py
--rw-r--r--   0        0        0      683 2023-05-29 12:41:50.868484 nonebot_plugin_nagabus-0.1.4.post1/pyproject.toml
--rw-r--r--   0        0        0     1789 2023-05-28 03:26:24.309853 nonebot_plugin_nagabus-0.1.4.post1/README.md
--rw-r--r--   0        0        0     2598 1970-01-01 00:00:00.000000 nonebot_plugin_nagabus-0.1.4.post1/PKG-INFO
+-rw-r--r--   0        0        0    35184 2022-12-04 13:51:12.448000 nonebot_plugin_nagabus-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1131 2023-05-28 14:51:33.780852 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/__init__.py
+-rw-r--r--   0        0        0      129 2023-05-27 04:29:09.849196 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/ac.py
+-rw-r--r--   0        0        0     1197 2023-05-28 14:51:33.775850 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/config.py
+-rw-r--r--   0        0        0        4 2023-05-26 13:11:24.775555 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/data/__init__.py
+-rw-r--r--   0        0        0      116 2023-05-26 11:41:42.946553 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/data/base.py
+-rw-r--r--   0        0        0      317 2023-05-26 11:41:42.956553 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/data/mjs.py
+-rw-r--r--   0        0        0     1697 2023-05-27 07:16:52.720509 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/data/naga.py
+-rw-r--r--   0        0        0      775 2023-05-26 11:41:42.960551 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/data/session.py
+-rw-r--r--   0        0        0      713 2023-05-26 15:21:27.421204 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/data/utils/__init__.py
+-rw-r--r--   0        0        0      761 2023-02-13 05:42:01.843000 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/data/utils/utc_datetime.py
+-rw-r--r--   0        0        0       43 2023-05-28 14:51:33.785849 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/errors.py
+-rw-r--r--   0        0        0       95 2023-05-28 01:19:53.575323 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/matchers/__init__.py
+-rw-r--r--   0        0        0      189 2023-05-30 02:32:55.940589 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/matchers/errors.py
+-rw-r--r--   0        0        0        0 2023-05-30 02:22:08.333037 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/matchers/interceptors/__init__.py
+-rw-r--r--   0        0        0     1090 2023-05-30 02:32:55.906573 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/matchers/interceptors/access_control.py
+-rw-r--r--   0        0        0     2392 2023-05-30 02:32:55.934567 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/matchers/interceptors/handle_error.py
+-rw-r--r--   0        0        0     4810 2023-05-30 02:36:34.180268 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/matchers/naga_analyze.py
+-rw-r--r--   0        0        0     2415 2023-05-30 02:32:55.921568 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/matchers/naga_statistic.py
+-rw-r--r--   0        0        0     2278 2023-05-27 02:48:33.707764 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/migrations/24aec3c56623_.py
+-rw-r--r--   0        0        0     1350 2023-05-27 07:17:07.623159 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py
+-rw-r--r--   0        0        0     1009 2023-05-26 15:21:27.440185 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/mjs/__init__.py
+-rw-r--r--   0        0        0      176 2023-05-25 15:39:25.419279 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/naga/__init__.py
+-rw-r--r--   0        0        0     3758 2023-05-27 13:45:54.389899 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/naga/api.py
+-rw-r--r--   0        0        0     3089 2023-05-29 12:30:46.127834 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/naga/fake_api.py
+-rw-r--r--   0        0        0     1066 2023-05-27 02:48:01.485010 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/naga/model.py
+-rw-r--r--   0        0        0    20455 2023-05-30 02:38:14.130387 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/naga/service.py
+-rw-r--r--   0        0        0        0 2023-05-25 16:04:02.955709 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/utils/__init__.py
+-rw-r--r--   0        0        0     1092 2023-05-25 16:06:56.701500 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/utils/integer.py
+-rw-r--r--   0        0        0        0 2023-05-26 12:48:40.974521 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/utils/mapping.py
+-rw-r--r--   0        0        0      101 2023-05-25 08:09:22.247000 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/utils/nonebot.py
+-rw-r--r--   0        0        0       68 2023-05-26 15:50:47.559077 nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/utils/tz.py
+-rw-r--r--   0        0        0      677 2023-05-30 02:38:28.516027 nonebot_plugin_nagabus-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1789 2023-05-28 03:26:24.309853 nonebot_plugin_nagabus-0.1.5/README.md
+-rw-r--r--   0        0        0     2592 1970-01-01 00:00:00.000000 nonebot_plugin_nagabus-0.1.5/PKG-INFO
```

### Comparing `nonebot_plugin_nagabus-0.1.4.post1/LICENSE` & `nonebot_plugin_nagabus-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/__init__.py` & `nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/config.py` & `nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/data/naga.py` & `nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/data/naga.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/data/session.py` & `nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/data/session.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/data/utils/__init__.py` & `nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/data/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/data/utils/utc_datetime.py` & `nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/data/utils/utc_datetime.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/matchers/naga_analyze.py` & `nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/matchers/naga_analyze.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,79 +1,63 @@
 import re
 from urllib.parse import urlparse, parse_qs
 
-from nonebot import on_command, logger, Bot
+from nonebot import on_command, Bot
 from nonebot.adapters.onebot.v11 import MessageEvent, Message, MessageSegment
 from nonebot.internal.matcher import Matcher
 from nonebot.params import CommandArg
-from nonebot_plugin_access_control.errors import RateLimitedError
-from tensoul.downloader import MajsoulDownloadError
 
-from .errors import BadRequestError, handle_error
+from .errors import BadRequestError
+from .interceptors.access_control import access_control
+from .interceptors.handle_error import handle_error
 from ..ac import ac
 from ..naga import naga
-from ..naga.service import InvalidKyokuHonbaError, UnsupportedGameError
+from ..naga.service import InvalidKyokuHonbaError
 from ..utils.integer import decode_integer
 from ..utils.nonebot import default_cmd_start
 
 analyze_srv = ac.create_subservice("analyze")
 
 
-async def analyze_majsoul(bot: Bot, event: MessageEvent, matcher: Matcher, uuid: str, kyoku: int, honba: int):
-    token = await analyze_srv.acquire_token_for_rate_limit(bot, event)
-    if token is None:
-        raise RateLimitedError()
-
+async def analyze_majsoul(event: MessageEvent, matcher: Matcher, uuid: str, kyoku: int, honba: int):
     try:
         report, cost_np = await naga.analyze_majsoul(uuid, kyoku, honba, event.user_id)
         msg = f"https://naga.dmv.nico/htmls/{report.report_id}.html?tw=0\n"
 
         if cost_np == 0:
             msg += "由于此前已解析过该局，本次解析消耗0NP"
+            token = matcher.state["ac_token"]
             await token.retire()
         else:
             msg += f"本次解析消耗{cost_np}NP"
 
         await matcher.send(Message([
             MessageSegment.reply(event.message_id),
             MessageSegment.text(msg)
         ]))
-    except MajsoulDownloadError as e:
-        await token.retire()
-        logger.opt(colors=True).warning(f"Failed to download paipu <y>{uuid}</y>, code: {e.code}")
-        if e.code == 1203:
-            raise BadRequestError("牌谱不存在") from e
-        else:
-            raise e
     except InvalidKyokuHonbaError as e:
-        await token.retire()
         kyoku_honba = []
         for kyoku, honba in e.available_kyoku_honba:
             if kyoku <= 3:
                 kyoku_honba.append(f"东{kyoku + 1}局{honba}本场")
             elif kyoku <= 7:
                 kyoku_honba.append(f"南{kyoku - 3}局{honba}本场")
             else:
                 kyoku_honba.append(f"西{kyoku - 7}局{honba}本场")
 
         raise BadRequestError(f"请输入正确的场次与本场（{'、'.join(kyoku_honba)}）") from e
-    except UnsupportedGameError as e:
-        raise BadRequestError("只支持四麻牌谱") from e
-
 
-async def analyze_tenhou(bot: Bot, event: MessageEvent, matcher: Matcher, haihu_id: str, seat: int):
-    token = await analyze_srv.acquire_token_for_rate_limit(bot, event)
-    if token is None:
-        raise RateLimitedError()
 
+async def analyze_tenhou(event: MessageEvent, matcher: Matcher, haihu_id: str, seat: int):
     report, cost_np = await naga.analyze_tenhou(haihu_id, seat, event.user_id)
     msg = f"https://naga.dmv.nico/htmls/{report.report_id}.html?tw=0\n"
 
     if cost_np == 0:
         msg += "由于此前已解析过该局，本次解析消耗0NP"
+        token = matcher.state["ac_token"]
         await token.retire()
     else:
         msg += f"本次解析消耗{cost_np}NP"
 
     await matcher.send(Message([
         MessageSegment.reply(event.message_id),
         MessageSegment.text(msg)
@@ -84,19 +68,17 @@
 
 uuid_reg = re.compile(r"\d{6}-[\da-fA-F]{8}-[\da-fA-F]{4}-[\da-fA-F]{4}-[\da-fA-F]{4}-[\da-fA-F]{12}")
 
 kyoku_honba_reg = re.compile(r"([东南西])([一二三四1234])局([0123456789零一两二三四五六七八九十百千万亿]+)本场")
 
 
 @naga_analyze_matcher.handle()
-@handle_error(naga_analyze_matcher)
-async def naga_analyze(bot: Bot, event: MessageEvent, matcher: Matcher, cmd_args=CommandArg()):
-    if not await analyze_srv.check(bot, event, acquire_rate_limit_token=False):
-        await matcher.finish()
-
+@handle_error()
+@access_control(analyze_srv)
+async def naga_analyze(event: MessageEvent, matcher: Matcher, cmd_args=CommandArg()):
     args = cmd_args.extract_plain_text().split(' ')
     if "maj-soul" in args[0]:
         mat = uuid_reg.search(args[0])
         if not mat:
             raise BadRequestError("不正确的雀魂牌谱")
 
         uuid = mat.group(0)
@@ -117,29 +99,29 @@
                         kyoku += 8
 
                     honba = decode_integer(raw_honba)
                 except ValueError:
                     pass
 
         if kyoku is None or honba is None:
-            await analyze_majsoul(bot, event, matcher, uuid, -1, -1)  # 让其发送该局的场次本场信息
+            await analyze_majsoul(event, matcher, uuid, -1, -1)  # 让其发送该局的场次本场信息
         else:
-            await analyze_majsoul(bot, event, matcher, uuid, kyoku, honba)
+            await analyze_majsoul(event, matcher, uuid, kyoku, honba)
     elif "tenhou" in args[0]:
         tenhou_url = args[0].strip()
 
         _, _, _, _, tenhou_query, _ = urlparse(tenhou_url)
         tenhou_query = parse_qs(tenhou_query)
 
         haihu_id = tenhou_query["log"][0]
         seat = 0
         if "tw" in tenhou_query and len(tenhou_query["tw"]) > 0:
             seat = int(tenhou_query["tw"][0])
 
-        await analyze_tenhou(bot, event, matcher, haihu_id, seat)
+        await analyze_tenhou(event, matcher, haihu_id, seat)
     else:
         await matcher.send(Message([
             MessageSegment.reply(event.message_id),
             MessageSegment.text("用法：\n"
                                 f"{default_cmd_start}naga <雀魂牌谱链接> <东/南x局x本场>：消耗10NP解析雀魂小局\n"
                                 f"{default_cmd_start}naga <天凤牌谱链接>：消耗50NP解析天凤半庄")
         ]))
```

### Comparing `nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/matchers/naga_statistic.py` & `nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/matchers/naga_statistic.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from io import StringIO
 
 from monthdelta import monthdelta
 from nonebot import on_command
 from nonebot.adapters.onebot.v11 import MessageEvent, Bot, GroupMessageEvent, Message, MessageSegment
 from nonebot.internal.matcher import Matcher
 
-from .errors import handle_error
+from .interceptors.handle_error import handle_error
 from ..ac import ac
 from ..naga import naga
 from ..utils.tz import TZ_TOKYO
 
 statistic_srv = ac.create_subservice("statistic")
 
 
@@ -46,22 +46,22 @@
 
 
 naga_statistic_this_month_matcher = on_command("naga本月使用情况", priority=5, block=True)
 statistic_srv.patch_matcher(naga_statistic_this_month_matcher)
 
 
 @naga_statistic_this_month_matcher.handle()
-@handle_error(naga_statistic_this_month_matcher)
+@handle_error()
 async def naga_statistic_this_month(bot: Bot, event: MessageEvent, matcher: Matcher):
     cur = datetime.now(tz=TZ_TOKYO)
     await naga_statistic(bot, event, matcher, cur.year, cur.month)
 
 
 naga_statistic_prev_month_matcher = on_command("naga上月使用情况", priority=5, block=True)
 statistic_srv.patch_matcher(naga_statistic_prev_month_matcher)
 
 
 @naga_statistic_prev_month_matcher.handle()
-@handle_error(naga_statistic_this_month_matcher)
+@handle_error()
 async def naga_statistic_prev_month(bot: Bot, event: MessageEvent, matcher: Matcher):
     prev_month = datetime.now(tz=TZ_TOKYO) - monthdelta(months=1)
     await naga_statistic(bot, event, matcher, prev_month.year, prev_month.month)
```

### Comparing `nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/migrations/24aec3c56623_.py` & `nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/migrations/24aec3c56623_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py` & `nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/migrations/ab4d80c20047_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/mjs/__init__.py` & `nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/mjs/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/naga/api.py` & `nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/naga/api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/naga/fake_api.py` & `nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/naga/fake_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/naga/model.py` & `nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/naga/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/naga/service.py` & `nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/naga/service.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import asyncio
 import json
+import re
 from asyncio import Lock
 from datetime import datetime, timezone
 from inspect import isawaitable
 from typing import Dict, Union, Optional, List, Tuple
 
 from monthdelta import monthdelta
 from nonebot import logger
 from sqlalchemy import select, update
+from tensoul.downloader import MajsoulDownloadError
 
 from .api import NagaApi, OrderReportList
 from .fake_api import FakeNagaApi
 from .model import NagaGameRule, NagaHanchanModelType, NagaTonpuuModelType, NagaOrder, NagaReport, NagaOrderStatus, \
     NagaServiceOrder, NagaServiceUserStatistic
 from ..config import conf
 from ..data.naga import MajsoulOrderOrm, NagaOrderOrm, NagaOrderSource
@@ -63,25 +65,31 @@
     ...
 
 
 class OrderError(NagaError):
     ...
 
 
+class InvalidGameError(NagaError):
+    ...
+
+
 class UnsupportedGameError(NagaError):
     ...
 
 
 class InvalidKyokuHonbaError(NagaError):
     def __init__(self, available_kyoku_honba: List[Tuple[int, int]]):
         super().__init__()
         self.available_kyoku_honba = available_kyoku_honba
 
 
 class NagaService:
+    _tenhou_haihu_id_reg = re.compile(r"^20\d{8}gm-[a-f\d]{4}-[a-z\d]{4,5}-[a-zA-Z\d]{8}$")
+
     def __init__(self, cookies: Dict[str, str], timeout: float = 90.0):
         if conf.naga_fake_api:
             self.api = FakeNagaApi()
             logger.warning("using fake naga api")
         else:
             self.api = NagaApi(cookies)
 
@@ -172,18 +180,26 @@
 
     async def analyze_majsoul(self, majsoul_uuid: str, kyoku: int, honba: int,
                               customer_id: int,
                               *,
                               model_type: Union[NagaHanchanModelType,
                                                 NagaTonpuuModelType, None] = None) -> NagaServiceOrder:
         sess = get_session()
-        data = await get_majsoul_paipu(majsoul_uuid)
+
+        try:
+            data = await get_majsoul_paipu(majsoul_uuid)
+        except MajsoulDownloadError as e:
+            logger.opt(colors=True).warning(f"Failed to download paipu <y>{majsoul_uuid}</y>, code: {e.code}")
+            if e.code == 1203:
+                raise InvalidGameError(f"invalid majsoul_uuid: {majsoul_uuid}") from e
+            else:
+                raise e
 
         if len(data["name"]) != 4:
-            raise UnsupportedGameError()
+            raise UnsupportedGameError("only yonma game is supported")
 
         if "東" in data["rule"]["disp"]:
             rule = NagaGameRule.tonpuu
         else:
             rule = NagaGameRule.hanchan
 
         if model_type is None:
@@ -314,17 +330,42 @@
         res = await self.api.analyze_tenhou(haihu_id, seat, model_type)
         if res.status != 200:
             raise OrderError(res.msg)
 
     # needs test
     async def analyze_tenhou(self, haihu_id: str, seat: int, customer_id: int,
                              *,
-                             model_type: NagaHanchanModelType = NagaHanchanModelType.nishiki) -> NagaServiceOrder:
+                             model_type: Union[NagaHanchanModelType,
+                                               NagaTonpuuModelType, None] = None) -> NagaServiceOrder:
         sess = get_session()
 
+        if not self._tenhou_haihu_id_reg.match(haihu_id):
+            raise InvalidGameError(f"invalid haihu_id: {haihu_id}")
+
+        haihu_element = haihu_id.split('-')
+        if len(haihu_element) != 4:
+            raise InvalidGameError(f"invalid haihu_id: {haihu_id}")
+
+        haihu_rule = int(haihu_element[1], 16)
+        is_yonma = not bool(haihu_rule & 16)
+        is_hanchan = bool(haihu_rule & 8)
+        is_kuitan = not bool(haihu_rule & 4)
+        is_online = bool(haihu_rule & 1)
+
+        if is_yonma and is_kuitan and is_online:
+            rule = NagaGameRule.hanchan if is_hanchan else NagaGameRule.tonpuu
+        else:
+            raise UnsupportedGameError("only online kuitan yonma game is supported")
+
+        if model_type is None:
+            if rule == NagaGameRule.hanchan:
+                model_type = NagaHanchanModelType.nishiki
+            else:
+                model_type = NagaTonpuuModelType.sigma
+
         new_order = False
 
         async def _get_local_order() -> Optional[NagaOrderOrm]:
             stmt = select(NagaOrderOrm).where(NagaOrderOrm.haihu_id == haihu_id,
                                               NagaOrderOrm.model_type == model_type.value)
 
             order_orm: Optional[NagaOrderOrm] = (await sess.execute(stmt)).scalar_one_or_none()
@@ -352,15 +393,15 @@
 
                     await self._order_tenhou(haihu_id, seat, model_type)
 
                     new_order = True
 
                     order_orm = NagaOrderOrm(haihu_id=haihu_id,
                                              customer_id=customer_id,
-                                             cost_np=50,
+                                             cost_np=50 if rule == NagaGameRule.hanchan else 30,
                                              source=NagaOrderSource.tenhou,
                                              model_type=model_type.value,
                                              status=NagaOrderStatus.analyzing,
                                              create_time=datetime.now(tz=timezone.utc),
                                              update_time=datetime.now(tz=timezone.utc))
 
                     sess.add(order_orm)
```

### Comparing `nonebot_plugin_nagabus-0.1.4.post1/nonebot_plugin_nagabus/utils/integer.py` & `nonebot_plugin_nagabus-0.1.5/nonebot_plugin_nagabus/utils/integer.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.4.post1/pyproject.toml` & `nonebot_plugin_nagabus-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-nagabus"
-version = "0.1.4.post1"
+version = "0.1.5"
 description = ""
 authors = ["ssttkkl <huang.wen.long@hotmail.com>"]
 readme = "README.md"
 packages = [{ include = "nonebot_plugin_nagabus" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `nonebot_plugin_nagabus-0.1.4.post1/README.md` & `nonebot_plugin_nagabus-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nagabus-0.1.4.post1/PKG-INFO` & `nonebot_plugin_nagabus-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nagabus
-Version: 0.1.4.post1
+Version: 0.1.5
 Summary: 
 Author: ssttkkl
 Author-email: huang.wen.long@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

