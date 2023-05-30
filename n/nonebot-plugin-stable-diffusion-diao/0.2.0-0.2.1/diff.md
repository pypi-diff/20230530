# Comparing `tmp/nonebot_plugin_stable_diffusion_diao-0.2.0.tar.gz` & `tmp/nonebot_plugin_stable_diffusion_diao-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.2.0.tar", last modified: Tue May 30 15:38:02 2023, max compression
+gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.2.1.tar", last modified: Tue May 30 17:07:19 2023, max compression
```

## Comparing `nonebot_plugin_stable_diffusion_diao-0.2.0.tar` & `nonebot_plugin_stable_diffusion_diao-0.2.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.2.0/LICENSE
--rw-r--r--   0        0        0      686 2023-05-28 09:58:15.400842 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/__init__.py
--rw-r--r--   0        0        0    18654 2023-05-28 09:58:15.401369 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/aidraw.py
--rw-r--r--   0        0        0     6100 2023-05-28 12:48:55.161779 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
--rw-r--r--   0        0        0    65592 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
--rw-r--r--   0        0        0     2528 2023-05-30 15:35:38.313378 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
--rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
--rw-r--r--   0        0        0    15349 2023-05-30 14:20:07.688799 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/backend/base.py
--rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
--rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
--rw-r--r--   0        0        0     6300 2023-05-30 15:28:12.457021 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/backend/sd.py
--rw-r--r--   0        0        0    13644 2023-05-30 14:02:44.198727 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/config.py
--rw-r--r--   0        0        0     9282 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
--rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
--rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
--rw-r--r--   0        0        0     1449 2023-05-30 13:50:33.328475 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
--rw-r--r--   0        0        0     3751 2023-05-28 09:58:15.407673 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
--rw-r--r--   0        0        0    11882 2023-05-30 15:32:52.299649 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
--rw-r--r--   0        0        0     3668 2023-05-28 12:10:58.511567 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
--rw-r--r--   0        0        0    28671 2023-05-28 16:27:22.765742 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
--rw-r--r--   0        0        0     5964 2023-05-28 09:58:15.408672 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/extension/translation.py
--rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/fifo.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/locales/en.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/locales/jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/locales/zh.py
--rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/manage.py
--rw-r--r--   0        0        0     1479 2023-05-28 09:58:15.412189 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
--rw-r--r--   0        0        0     2314 2023-05-28 09:58:15.412189 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/utils/data.py
--rw-r--r--   0        0        0     7499 2023-05-30 15:27:52.695256 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
--rw-r--r--   0        0        0      647 2023-05-28 09:58:15.413187 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
--rw-r--r--   0        0        0      727 2023-05-28 09:58:15.413187 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/utils/save.py
--rw-r--r--   0        0        0     1994 2023-05-28 09:58:15.414188 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/version.py
--rw-r--r--   0        0        0      701 2023-05-30 15:38:02.449721 nonebot_plugin_stable_diffusion_diao-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.2.1/LICENSE
+-rw-r--r--   0        0        0      686 2023-05-28 09:58:15.400842 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/__init__.py
+-rw-r--r--   0        0        0    18642 2023-05-30 17:04:49.624751 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/aidraw.py
+-rw-r--r--   0        0        0     6213 2023-05-30 17:03:22.535709 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
+-rw-r--r--   0        0        0    65703 2023-05-30 17:03:23.970846 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
+-rw-r--r--   0        0        0     2528 2023-05-30 15:35:38.313378 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
+-rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
+-rw-r--r--   0        0        0    15349 2023-05-30 14:20:07.688799 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/backend/base.py
+-rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
+-rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
+-rw-r--r--   0        0        0     6300 2023-05-30 15:28:12.457021 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/backend/sd.py
+-rw-r--r--   0        0        0    13640 2023-05-30 17:06:09.122349 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/config.py
+-rw-r--r--   0        0        0     9282 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
+-rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
+-rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
+-rw-r--r--   0        0        0     1102 2023-05-30 17:05:34.472127 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
+-rw-r--r--   0        0        0     3751 2023-05-28 09:58:15.407673 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
+-rw-r--r--   0        0        0    11882 2023-05-30 15:32:52.299649 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
+-rw-r--r--   0        0        0     3668 2023-05-28 12:10:58.511567 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
+-rw-r--r--   0        0        0    28782 2023-05-30 17:03:26.416767 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
+-rw-r--r--   0        0        0     5964 2023-05-28 09:58:15.408672 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/extension/translation.py
+-rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/fifo.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/locales/en.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/locales/jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/locales/zh.py
+-rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/manage.py
+-rw-r--r--   0        0        0     1479 2023-05-28 09:58:15.412189 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
+-rw-r--r--   0        0        0     2314 2023-05-28 09:58:15.412189 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/utils/data.py
+-rw-r--r--   0        0        0     7499 2023-05-30 15:27:52.695256 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
+-rw-r--r--   0        0        0      647 2023-05-28 09:58:15.413187 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
+-rw-r--r--   0        0        0      727 2023-05-28 09:58:15.413187 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/utils/save.py
+-rw-r--r--   0        0        0     1994 2023-05-28 09:58:15.414188 nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/version.py
+-rw-r--r--   0        0        0      701 2023-05-30 17:07:19.612767 nonebot_plugin_stable_diffusion_diao-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.2.1/PKG-INFO
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.0/LICENSE` & `nonebot_plugin_stable_diffusion_diao-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/aidraw.py` & `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/aidraw.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from nonebot.log import logger
 from nonebot.params import ShellCommandArgs
 
 from .config import config, nickname
 from .utils.data import lowQuality, basetag, htags
 from .backend import AIDRAW
 from .extension.anlas import anlas_check, anlas_set
-from .extension.daylimit import DayLimit
+from .extension.daylimit import count
 from .extension.explicit_api import check_safe_method
 from .utils.save import save_img
 from .utils.prepocess import prepocess_tags
 from .version import version
 from .utils import sendtosuperuser
 from .extension.safe_method import send_forward_msg
 from .extension.sd_extra_api_func import change_model
@@ -105,15 +105,15 @@
         group_id = str(event.group_id)
     global bot_id
     bot_id = bot.self_id
     # 判断是否禁用，若没禁用，进入处理流程
     if await config.get_value(group_id, "on"):
         message = ""
         if config.novelai_daylimit and not await SUPERUSER(bot, event):
-            left = await DayLimit.count(user_id, 1)
+            left = await count(user_id, 1)
             if left == -1:
                 await aidraw.finish(f"今天你的次数不够了哦")
             else:
                 message = message + f"，今天你还能够生成{left}张"
         # 判断cd
         nowtime = time.time()
         deltatime = nowtime - cd.get(user_id, 0)
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py` & `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 from ..backend import AIDRAW
 from ..config import config
 from ..utils.save import save_img
 
 from nonebot import on_command
 from nonebot.adapters.onebot.v11 import MessageEvent, MessageSegment, Bot, Message, ActionFailed
 from nonebot.params import CommandArg
-from ..extension.daylimit import DayLimit
+from nonebot.permission import SUPERUSER
+
+from ..extension.daylimit import count
 from ..extension.explicit_api import check_safe_method
 from ..extension.safe_method import risk_control
 from ..utils.data import basetag, lowQuality
 
 sys_text = f'''
 You can output a prompt based on the input given by the user,
 The prompts are used to guide the AI drawing model in creating images.
@@ -70,17 +72,18 @@
     if user_id not in user_session:
         user_session[user_id] = Session(user_id)
     return user_session[user_id]
 
 
 @chatgpt.handle()
 async def _(event: MessageEvent, bot: Bot, msg: Message = CommandArg()):
-    left = await DayLimit.count(str(event.user_id), 1)
-    if left == -1:
-        await chatgpt.finish(f"今天你的次数不够了哦，明天再来找我玩吧")
+    if config.novelai_daylimit and not await SUPERUSER(bot, event):
+        left = await count(str(event.user_id), 1)
+        if left == -1:
+            await chatgpt.finish(f"今天你的次数不够了哦，明天再来找我玩吧")
     user_msg = msg.extract_plain_text().strip()
     to_openai = user_msg + "prompt"
     prompt = await get_user_session(event.get_session_id()).main(to_openai)
 
     await risk_control(
                     bot, 
                     event,
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py` & `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from nonebot import on_command, logger
 from nonebot.adapters.onebot.v11 import MessageEvent, MessageSegment, Bot, ActionFailed, PrivateMessageEvent, Message
 from nonebot.params import CommandArg
+from nonebot.permission import SUPERUSER
 
 from ..backend import AIDRAW
 from ..extension.translation import translate_deepl, translate
-from ..extension.daylimit import DayLimit
+from ..extension.daylimit import count
 from ..config import config
 from ..utils.data import basetag, lowQuality
 from ..utils.save import save_img
 from ..aidraw import get_message_at
 from ..extension.explicit_api import check_safe_method
 
 import random, time, json, re, base64, aiohttp, aiofiles
@@ -1263,17 +1264,18 @@
         if isinstance(event, PrivateMessageEvent):
          user_name = event.sender.nickname
         else:
             get_info = await bot.get_group_member_info(group_id=event.group_id, user_id=user_id)
             user_name = get_info["nickname"]
     else:
         user_name = message
-    left = await DayLimit.count(str(event.user_id), 1)
-    if left == -1:
-        await today_girl.finish(f"今天你的次数不够了哦，明天再来找我玩吧")
+    if config.novelai_daylimit and not await SUPERUSER(bot, event):
+        left = await count(str(event.user_id), 1)
+        if left == -1:
+            await today_girl.finish(f"今天你的次数不够了哦，明天再来找我玩吧")
     img_url = None
     random_int_str = str(random.randint(0, 65535))
 
     at_id = await get_message_at(event.json())
     if at_id:
         img_url = f"https://q1.qlogo.cn/g?b=qq&nk={at_id}&s=640"
         user_id = str(at_id)
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/amusement/vits.py` & `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/amusement/vits.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/backend/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/backend/base.py` & `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/backend/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/backend/naifu.py` & `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/backend/naifu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/backend/novelai.py` & `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/backend/novelai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/backend/sd.py` & `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/backend/sd.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/config.py` & `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     novelai_site: str = "127.0.0.1:7860"
     # 后台设置
     novelai_save: int = 2  # 是否保存图片至本地,0为不保存，1保存，2同时保存追踪信息
     novelai_save_png: bool = False # 是否保存为PNG格式
     novelai_paid: int = 3  # 0为禁用付费模式，1为点数制，2为不限制
     novelai_pure: bool = True  # 是否启用简洁返回模式（只返回图片，不返回tag等数据）
     novelai_limit: bool = False  # 是否开启限速
-    novelai_daylimit: int = 20204  # 每日次数限制，0为禁用
+    novelai_daylimit: int = 0  # 每日次数限制，0为禁用
     novelai_h: int = 1  # 是否允许H, 0为不允许, 1为删除屏蔽词, 2允许
     novelai_htype: int = 2 # 1为发现H后私聊用户返回图片, 2为返回群消息但是只返回图片url并且主人直接私吞H图(, 3发送二维码(无论参数如何都会保存图片到本地)
     novelai_antireport: bool = True  # 玄学选项。开启后，合并消息内发送者将会显示为调用指令的人而不是bot
     novelai_max: int = 3  # 每次能够生成的最大数量
     # 允许生成的图片最大分辨率，对应(值)^2.默认为1024（即1024*1024）。如果服务器比较寄，建议改成640（640*640）或者根据能够承受的情况修改。naifu和novelai会分别限制最大长宽为1024
     # 可运行更改的设置
     novelai_tags: str = ""  # 内置的tag
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py` & `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/extension/anlas.py` & `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/extension/anlas.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/extension/control_net.py` & `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/extension/control_net.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py` & `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py` & `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py` & `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py` & `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,21 +18,22 @@
 from ..extension.translation import translate
 from ..extension.explicit_api import check_safe_method
 from .translation import translate
 from ..backend import AIDRAW
 from ..utils.data import lowQuality, basetag
 from ..utils.load_balance import sd_LoadBalance
 from .safe_method import send_forward_msg, risk_control
-from ..extension.daylimit import DayLimit
+from ..extension.daylimit import count
 
 from nonebot import on_command, on_shell_command
 from nonebot.adapters.onebot.v11 import Bot, MessageEvent, Message, MessageSegment, ActionFailed, PrivateMessageEvent
 from nonebot.params import CommandArg, Arg, ArgPlainText, ShellCommandArgs
 from nonebot.typing import T_State
 from nonebot.rule import ArgumentParser
+from nonebot.permission import SUPERUSER
 from nonebot import logger
 from collections import Counter
 
 
 async def func_init(event):
     '''
     获取当前群的后端设置
@@ -450,17 +451,18 @@
 
 @control_net.got('tag', "请输入绘画的关键词")
 async def __():
     pass
 
 @control_net.got("net", "你的图图呢？")
 async def _(event: MessageEvent, bot: Bot, tag: str = ArgPlainText("tag"), msg: Message = Arg("net")):
-    left = await DayLimit.count(str(event.user_id), 2)
-    if left == -1:
-        await control_net.finish(f"今天你的次数不够了哦，明天再来找我玩吧")
+    if config.novelai_daylimit and not await SUPERUSER(bot, event):
+        left = await count(str(event.user_id), 2)
+        if left == -1:
+            await control_net.finish(f"今天你的次数不够了哦，明天再来找我玩吧")
     await func_init(event)
     start = time.time()
     tags_en = None
     reply= event.reply
     await bot.send(event=event, message=f"control_net以图生图中")
     if msg[0].type == "image":
             img_url = msg[0].data["url"]
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/extension/translation.py` & `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/extension/translation.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/manage.py` & `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/manage.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/utils/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/utils/data.py` & `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/utils/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py` & `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py` & `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/utils/save.py` & `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/utils/save.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/version.py` & `nonebot_plugin_stable_diffusion_diao-0.2.1/nonebot_plugin_stable_diffusion_diao/version.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.2.0/pyproject.toml` & `nonebot_plugin_stable_diffusion_diao-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-stable-diffusion-diao"
-version = "0.2.0"
+version = "0.2.1"
 description = "主要面对stable-diffusion-webui-api的nonebot2插件"
 authors = [
     { name = "DiaoDaiaChan", email = "diaodaiachan@qq.com" },
 ]
 dependencies = [
     "aiofiles>=23.1.0",
     "aiohttp>=3.8.4",
```

