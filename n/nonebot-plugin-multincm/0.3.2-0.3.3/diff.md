# Comparing `tmp/nonebot_plugin_multincm-0.3.2.tar.gz` & `tmp/nonebot_plugin_multincm-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_multincm-0.3.2.tar", last modified: Mon May 29 16:49:23 2023, max compression
+gzip compressed data, was "nonebot_plugin_multincm-0.3.3.tar", last modified: Tue May 30 15:59:35 2023, max compression
```

## Comparing `nonebot_plugin_multincm-0.3.2.tar` & `nonebot_plugin_multincm-0.3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1069 2023-05-29 16:49:10.287833 nonebot_plugin_multincm-0.3.2/LICENSE
--rw-r--r--   0        0        0     8147 2023-05-29 16:49:10.287833 nonebot_plugin_multincm-0.3.2/README.md
--rw-r--r--   0        0        0     1646 2023-05-29 16:49:10.287833 nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/__init__.py
--rw-r--r--   0        0        0    12064 2023-05-29 16:49:10.287833 nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/__main__.py
--rw-r--r--   0        0        0      582 2023-05-29 16:49:10.287833 nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/config.py
--rw-r--r--   0        0        0      134 2023-05-29 16:49:10.287833 nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/const.py
--rw-r--r--   0        0        0     5556 2023-05-29 16:49:10.287833 nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/data_source.py
--rw-r--r--   0        0        0    11669 2023-05-29 16:49:10.287833 nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/draw.py
--rw-r--r--   0        0        0     2957 2023-05-29 16:49:10.287833 nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/lrc_parser.py
--rw-r--r--   0        0        0     2279 2023-05-29 16:49:10.287833 nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/msg_cache.py
--rw-r--r--   0        0        0   212591 2023-05-29 16:49:10.291833 nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/res/bg.jpg
--rw-r--r--   0        0        0     3007 2023-05-29 16:49:10.291833 nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/types.py
--rw-r--r--   0        0        0      851 2023-05-29 16:49:10.291833 nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/utils.py
--rw-r--r--   0        0        0      867 2023-05-29 16:49:23.299930 nonebot_plugin_multincm-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     9097 1970-01-01 00:00:00.000000 nonebot_plugin_multincm-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-30 15:59:18.886468 nonebot_plugin_multincm-0.3.3/LICENSE
+-rw-r--r--   0        0        0     8484 2023-05-30 15:59:18.886468 nonebot_plugin_multincm-0.3.3/README.md
+-rw-r--r--   0        0        0     1646 2023-05-30 15:59:18.886468 nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/__init__.py
+-rw-r--r--   0        0        0    12222 2023-05-30 15:59:18.886468 nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/__main__.py
+-rw-r--r--   0        0        0      623 2023-05-30 15:59:18.886468 nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/config.py
+-rw-r--r--   0        0        0      134 2023-05-30 15:59:18.886468 nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/const.py
+-rw-r--r--   0        0        0     5556 2023-05-30 15:59:18.886468 nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/data_source.py
+-rw-r--r--   0        0        0    11669 2023-05-30 15:59:18.886468 nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/draw.py
+-rw-r--r--   0        0        0     2957 2023-05-30 15:59:18.886468 nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/lrc_parser.py
+-rw-r--r--   0        0        0     2279 2023-05-30 15:59:18.886468 nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/msg_cache.py
+-rw-r--r--   0        0        0   212591 2023-05-30 15:59:18.890468 nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/res/bg.jpg
+-rw-r--r--   0        0        0     3007 2023-05-30 15:59:18.890468 nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/types.py
+-rw-r--r--   0        0        0      851 2023-05-30 15:59:18.890468 nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/utils.py
+-rw-r--r--   0        0        0      867 2023-05-30 15:59:35.358548 nonebot_plugin_multincm-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     9434 1970-01-01 00:00:00.000000 nonebot_plugin_multincm-0.3.3/PKG-INFO
```

### Comparing `nonebot_plugin_multincm-0.3.2/LICENSE` & `nonebot_plugin_multincm-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.2/README.md` & `nonebot_plugin_multincm-0.3.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -132,27 +132,28 @@
 
 如果你安装了 [nonebot-plugin-ncm](https://github.com/kitUIN/nonebot-plugin-ncm)，本插件会与其共用同一个 Session，就可以不用填下面的账号密码了
 
 下面配置中，手机号登录 和 邮箱登录、明文密码 和 MD5 密码哈希 各选其一填写即可
 
 在 nonebot2 项目的 `.env` 文件中添加下表中的必填配置
 
-|        配置项        | 必填 | 默认值  |                               说明                                |
-| :------------------: | :--: | :-----: | :---------------------------------------------------------------: |
-|     `NCM_CTCODE`     |  否  |  `86`   |                    手机号登录用，登录手机区号                     |
-|     `NCM_PHONE`      |  否  |   无    |                     手机号登录用，登录手机号                      |
-|     `NCM_EMAIL`      |  否  |   无    |                       邮箱登录用，登录邮箱                        |
-|    `NCM_PASSWORD`    |  否  |   无    |                帐号明文密码，邮箱登录时为邮箱密码                 |
-| `NCM_PASSWORD_HASH`  |  否  |   无    |              帐号密码 MD5 哈希，邮箱登录时为邮箱密码              |
-|   `NCM_LIST_LIMIT`   |  否  |  `20`   |                      歌曲列表每页的最大数量                       |
-|   `NCM_LIST_FONT`    |  否  |   无    |                      渲染歌曲列表使用的字体                       |
-|  `NCM_MAX_NAME_LEN`  |  否  |  `600`  |              歌曲列表中歌名列的最大文本宽度（像素）               |
-| `NCM_MAX_ARTIST_LEN` |  否  |  `400`  |              歌曲列表中歌手列的最大文本宽度（像素）               |
-| `NCM_MSG_CACHE_TIME` |  否  | `3600`  | 缓存 Bot 已发送音乐卡片的音乐 ID 及 用户最近一次操作 的时长（秒） |
-|  `NCM_AUTO_RESOLVE`  |  否  | `False` |         当用户发送音乐链接时，是否自动解析并发送音乐卡片          |
+|          配置项          | 必填 | 默认值  |                               说明                                |
+| :----------------------: | :--: | :-----: | :---------------------------------------------------------------: |
+|       `NCM_CTCODE`       |  否  |  `86`   |                    手机号登录用，登录手机区号                     |
+|       `NCM_PHONE`        |  否  |   无    |                     手机号登录用，登录手机号                      |
+|       `NCM_EMAIL`        |  否  |   无    |                       邮箱登录用，登录邮箱                        |
+|      `NCM_PASSWORD`      |  否  |   无    |                帐号明文密码，邮箱登录时为邮箱密码                 |
+|   `NCM_PASSWORD_HASH`    |  否  |   无    |              帐号密码 MD5 哈希，邮箱登录时为邮箱密码              |
+|     `NCM_LIST_LIMIT`     |  否  |  `20`   |                      歌曲列表每页的最大数量                       |
+|     `NCM_LIST_FONT`      |  否  |   无    |                      渲染歌曲列表使用的字体                       |
+|    `NCM_MAX_NAME_LEN`    |  否  |  `600`  |              歌曲列表中歌名列的最大文本宽度（像素）               |
+|   `NCM_MAX_ARTIST_LEN`   |  否  |  `400`  |              歌曲列表中歌手列的最大文本宽度（像素）               |
+|   `NCM_MSG_CACHE_TIME`   |  否  | `3600`  | 缓存 Bot 已发送音乐卡片的音乐 ID 及 用户最近一次操作 的时长（秒） |
+|    `NCM_AUTO_RESOLVE`    |  否  | `False` |         当用户发送音乐链接时，是否自动解析并发送音乐卡片          |
+| `NCM_ILLEGAL_CMD_FINISH` |  否  | `False` |          当用户在点歌时输入了非法指令，是否直接退出点歌           |
 
 ## 🎉 使用
 
 ### 指令
 
 - 点歌 [歌曲名 / 音乐 ID]
   - 介绍：搜索歌曲。当输入音乐 ID 时会直接发送对应音乐
@@ -212,14 +213,19 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.3.3
+
+- 新增配置项 `NCM_ILLEGAL_CMD_FINISH`
+- 在未启用 `NCM_ILLEGAL_CMD_FINISH` 时输入错误指令将会提示用户退出点歌
+
 ### 0.3.2
 
 - 新增配置项 `NCM_MSG_CACHE_TIME`、`NCM_AUTO_RESOLVE`
 - 调整登录流程到 `driver.on_startup` 中
 
 ### 0.3.1
```

#### html2text {}

```diff
@@ -27,32 +27,34 @@
 "nonebot_plugin_multincm" ] ```  ## âï¸ éç½® å¦æä½ å®è£äº [nonebot-
 plugin-ncm](https://github.com/kitUIN/nonebot-plugin-
 ncm)ï¼æ¬æä»¶ä¼ä¸å¶å±ç¨åä¸ä¸ª
 Sessionï¼å°±å¯ä»¥ä¸ç¨å¡«ä¸é¢çè´¦å·å¯ç äº
 ä¸é¢éç½®ä¸­ï¼ææºå·ç»å½ å é®ç®±ç»å½ãææå¯ç  å MD5
 å¯ç åå¸ åéå¶ä¸å¡«åå³å¯ å¨ nonebot2 é¡¹ç®ç `.env`
 æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« | é»è®¤å¼ |
-è¯´æ | | :------------------: | :--: | :-----: | :---------------------------
-------------------------------------: | | `NCM_CTCODE` | å¦ | `86` |
+è¯´æ | | :----------------------: | :--: | :-----: | :-----------------------
+----------------------------------------: | | `NCM_CTCODE` | å¦ | `86` |
 ææºå·ç»å½ç¨ï¼ç»å½ææºåºå· | | `NCM_PHONE` | å¦ | æ  |
 ææºå·ç»å½ç¨ï¼ç»å½ææºå· | | `NCM_EMAIL` | å¦ | æ  |
 é®ç®±ç»å½ç¨ï¼ç»å½é®ç®± | | `NCM_PASSWORD` | å¦ | æ  |
 å¸å·ææå¯ç ï¼é®ç®±ç»å½æ¶ä¸ºé®ç®±å¯ç  | | `NCM_PASSWORD_HASH` |
 å¦ | æ  | å¸å·å¯ç  MD5 åå¸ï¼é®ç®±ç»å½æ¶ä¸ºé®ç®±å¯ç  | |
 `NCM_LIST_LIMIT` | å¦ | `20` | æ­æ²åè¡¨æ¯é¡µçæå¤§æ°é | |
 `NCM_LIST_FONT` | å¦ | æ  | æ¸²ææ­æ²åè¡¨ä½¿ç¨çå­ä½ | |
 `NCM_MAX_NAME_LEN` | å¦ | `600` |
 æ­æ²åè¡¨ä¸­æ­ååçæå¤§ææ¬å®½åº¦ï¼åç´ ï¼ | |
 `NCM_MAX_ARTIST_LEN` | å¦ | `400` |
 æ­æ²åè¡¨ä¸­æ­æåçæå¤§ææ¬å®½åº¦ï¼åç´ ï¼ | |
 `NCM_MSG_CACHE_TIME` | å¦ | `3600` | ç¼å­ Bot å·²åéé³ä¹å¡ççé³ä¹
 ID å ç¨æ·æè¿ä¸æ¬¡æä½ çæ¶é¿ï¼ç§ï¼ | | `NCM_AUTO_RESOLVE` | å¦
 | `False` |
-å½ç¨æ·åéé³ä¹é¾æ¥æ¶ï¼æ¯å¦èªå¨è§£æå¹¶åéé³ä¹å¡ç | ##
-ð ä½¿ç¨ ### æä»¤ - ç¹æ­ [æ­æ²å / é³ä¹ ID] -
+å½ç¨æ·åéé³ä¹é¾æ¥æ¶ï¼æ¯å¦èªå¨è§£æå¹¶åéé³ä¹å¡ç | |
+`NCM_ILLEGAL_CMD_FINISH` | å¦ | `False` |
+å½ç¨æ·å¨ç¹æ­æ¶è¾å¥äºéæ³æä»¤ï¼æ¯å¦ç´æ¥éåºç¹æ­ | ## ð
+ä½¿ç¨ ### æä»¤ - ç¹æ­ [æ­æ²å / é³ä¹ ID] -
 ä»ç»ï¼æç´¢æ­æ²ãå½è¾å¥é³ä¹ ID æ¶ä¼ç´æ¥åéå¯¹åºé³ä¹ -
 å«åï¼`ç½æäº`ã`wyy` - çµå° [æ­æ²å / èç® ID] -
 ä»ç»ï¼æç´¢çµå°èç®ãå½è¾å¥çµå° ID æ¶ä¼ç´æ¥åéå¯¹åºèç®
 - å«åï¼`å£°é³`ã`ç½æçµå°`ã`wydt`ã`wydj` - è§£æ [åå¤
 é³ä¹å¡ç / é¾æ¥] - ä»ç»ï¼è·åè¯¥ é³ä¹ / çµå°èç®
 çæ­æ¾é¾æ¥å¹¶ä½¿ç¨èªå®ä¹å¡çåé -
 å«åï¼`resolve`ã`parse`ã`get` - æ­è¯ [åå¤ é³ä¹å¡ç / é¾æ¥] -
@@ -71,15 +73,17 @@
 é¡¹ç®ä½¿ç¨çç½æäº API è°ç¨åº ### [Binaryify/NeteaseCloudMusicApi]
 (https://github.com/Binaryify/NeteaseCloudMusicApi) é¡¹ç®çµå°ç¸å³ API
 æ¥æº ### [MeetWq/pil-utils](https://github.com/MeetWq/pil-utils) è¶å¥½ç¨ç
 Pillow è¾å©åº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.3.2 - æ°å¢éç½®é¡¹
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.3.3 - æ°å¢éç½®é¡¹
+`NCM_ILLEGAL_CMD_FINISH` - å¨æªå¯ç¨ `NCM_ILLEGAL_CMD_FINISH`
+æ¶è¾å¥éè¯¯æä»¤å°ä¼æç¤ºç¨æ·éåºç¹æ­ ### 0.3.2 - æ°å¢éç½®é¡¹
 `NCM_MSG_CACHE_TIME`ã`NCM_AUTO_RESOLVE` - è°æ´ç»å½æµç¨å°
 `driver.on_startup` ä¸­ ### 0.3.1 - ä¿®å¤çµå°ç¸å³ bug ### 0.3.0 -
 æ¯æçµå°èç®çè§£æä¸ç¹æ­ ### 0.2.5 - `è§£æ`ã`æ­è¯`ã`é¾æ¥`
 æä»¤å¯ä»¥ç´æ¥æ ¹æ® Bot åéçä¸ä¸ªé³ä¹å¡çä½åºååºäº -
 æ­è¯è§£æä¼åå¹¶å¤è¡ç©ºè¡åå»æé¦å°¾ç©ºè¡äº -
 ç°å¨æä»¶ä¼å®æ¶æ¸çèªèº«åå­ä¸­çç¼å­äº ### 0.2.4 -
 ä¿®å¤ä¸ä¸ªæ­è¯è§£æ bug ### 0.2.3 - å¾®è°æ­æ²åè¡¨æç -
```

### Comparing `nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/__init__.py` & `nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from nonebot.plugin import PluginMetadata, require
 
 require("nonebot_plugin_apscheduler")
 
 from . import __main__ as __main__  # noqa: E402
 from .config import ConfigModel  # noqa: E402
 
-__version__ = "0.3.2"
+__version__ = "0.3.3"
 __plugin_meta__ = PluginMetadata(
     "MultiNCM",
     "网易云多选点歌",
     (
         "指令列表：\n"
         "▶ 点歌 [歌曲名 / 音乐 ID]\n"
         "    ▷ 介绍：搜索歌曲。当输入音乐 ID 时会直接发送对应音乐\n"
```

### Comparing `nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/__main__.py` & `nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -335,15 +335,18 @@
     if arg.isdigit():
         cache: Dict[int, SearchResult] = state["cache"]
         song = await get_cache_by_index(cache, int(arg))
         if not song:
             await matcher.reject("序号输入有误，请重新输入")
         await send_music(matcher, song)
 
-    await matcher.reject("非正确指令，请重新输入")
+    if config.ncm_illegal_cmd_finish:
+        await matcher.finish("非正确指令，已退出点歌")
+
+    await matcher.reject("非正确指令，请重新输入\nTip: 你可以发送 `退出` 来退出点歌模式")
 
 
 cmd_get_song = on_command(
     "解析",
     aliases={"resolve", "parse", "get"},
     rule=music_msg_matcher_rule,
 )
```

### Comparing `nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/config.py` & `nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,10 +12,11 @@
     ncm_password_hash: Optional[str] = None
     ncm_list_limit: int = 20
     ncm_list_font: Optional[str] = None
     ncm_max_name_len: int = 600
     ncm_max_artist_len: int = 400
     ncm_msg_cache_time: int = 3600
     ncm_auto_resolve: bool = False
+    ncm_illegal_cmd_finish: bool = False
 
 
 config: ConfigModel = ConfigModel.parse_obj(get_driver().config.dict())
```

### Comparing `nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/data_source.py` & `nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/draw.py` & `nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/draw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/lrc_parser.py` & `nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/lrc_parser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/msg_cache.py` & `nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/msg_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/res/bg.jpg` & `nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/res/bg.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/types.py` & `nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/types.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.2/nonebot_plugin_multincm/utils.py` & `nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.2/pyproject.toml` & `nonebot_plugin_multincm-0.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-multincm"
-version = "0.3.2"
+version = "0.3.3"
 description = "NCM Song Searcher"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0-rc.1",
     "nonebot-adapter-onebot>=2.2.0",
```

### Comparing `nonebot_plugin_multincm-0.3.2/PKG-INFO` & `nonebot_plugin_multincm-0.3.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-multincm
-Version: 0.3.2
+Version: 0.3.3
 Summary: NCM Song Searcher
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
 Requires-Python: <4.0,>=3.8
 Requires-Dist: nonebot2>=2.0.0-rc.1
@@ -158,27 +158,28 @@
 
 如果你安装了 [nonebot-plugin-ncm](https://github.com/kitUIN/nonebot-plugin-ncm)，本插件会与其共用同一个 Session，就可以不用填下面的账号密码了
 
 下面配置中，手机号登录 和 邮箱登录、明文密码 和 MD5 密码哈希 各选其一填写即可
 
 在 nonebot2 项目的 `.env` 文件中添加下表中的必填配置
 
-|        配置项        | 必填 | 默认值  |                               说明                                |
-| :------------------: | :--: | :-----: | :---------------------------------------------------------------: |
-|     `NCM_CTCODE`     |  否  |  `86`   |                    手机号登录用，登录手机区号                     |
-|     `NCM_PHONE`      |  否  |   无    |                     手机号登录用，登录手机号                      |
-|     `NCM_EMAIL`      |  否  |   无    |                       邮箱登录用，登录邮箱                        |
-|    `NCM_PASSWORD`    |  否  |   无    |                帐号明文密码，邮箱登录时为邮箱密码                 |
-| `NCM_PASSWORD_HASH`  |  否  |   无    |              帐号密码 MD5 哈希，邮箱登录时为邮箱密码              |
-|   `NCM_LIST_LIMIT`   |  否  |  `20`   |                      歌曲列表每页的最大数量                       |
-|   `NCM_LIST_FONT`    |  否  |   无    |                      渲染歌曲列表使用的字体                       |
-|  `NCM_MAX_NAME_LEN`  |  否  |  `600`  |              歌曲列表中歌名列的最大文本宽度（像素）               |
-| `NCM_MAX_ARTIST_LEN` |  否  |  `400`  |              歌曲列表中歌手列的最大文本宽度（像素）               |
-| `NCM_MSG_CACHE_TIME` |  否  | `3600`  | 缓存 Bot 已发送音乐卡片的音乐 ID 及 用户最近一次操作 的时长（秒） |
-|  `NCM_AUTO_RESOLVE`  |  否  | `False` |         当用户发送音乐链接时，是否自动解析并发送音乐卡片          |
+|          配置项          | 必填 | 默认值  |                               说明                                |
+| :----------------------: | :--: | :-----: | :---------------------------------------------------------------: |
+|       `NCM_CTCODE`       |  否  |  `86`   |                    手机号登录用，登录手机区号                     |
+|       `NCM_PHONE`        |  否  |   无    |                     手机号登录用，登录手机号                      |
+|       `NCM_EMAIL`        |  否  |   无    |                       邮箱登录用，登录邮箱                        |
+|      `NCM_PASSWORD`      |  否  |   无    |                帐号明文密码，邮箱登录时为邮箱密码                 |
+|   `NCM_PASSWORD_HASH`    |  否  |   无    |              帐号密码 MD5 哈希，邮箱登录时为邮箱密码              |
+|     `NCM_LIST_LIMIT`     |  否  |  `20`   |                      歌曲列表每页的最大数量                       |
+|     `NCM_LIST_FONT`      |  否  |   无    |                      渲染歌曲列表使用的字体                       |
+|    `NCM_MAX_NAME_LEN`    |  否  |  `600`  |              歌曲列表中歌名列的最大文本宽度（像素）               |
+|   `NCM_MAX_ARTIST_LEN`   |  否  |  `400`  |              歌曲列表中歌手列的最大文本宽度（像素）               |
+|   `NCM_MSG_CACHE_TIME`   |  否  | `3600`  | 缓存 Bot 已发送音乐卡片的音乐 ID 及 用户最近一次操作 的时长（秒） |
+|    `NCM_AUTO_RESOLVE`    |  否  | `False` |         当用户发送音乐链接时，是否自动解析并发送音乐卡片          |
+| `NCM_ILLEGAL_CMD_FINISH` |  否  | `False` |          当用户在点歌时输入了非法指令，是否直接退出点歌           |
 
 ## 🎉 使用
 
 ### 指令
 
 - 点歌 [歌曲名 / 音乐 ID]
   - 介绍：搜索歌曲。当输入音乐 ID 时会直接发送对应音乐
@@ -238,14 +239,19 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.3.3
+
+- 新增配置项 `NCM_ILLEGAL_CMD_FINISH`
+- 在未启用 `NCM_ILLEGAL_CMD_FINISH` 时输入错误指令将会提示用户退出点歌
+
 ### 0.3.2
 
 - 新增配置项 `NCM_MSG_CACHE_TIME`、`NCM_AUTO_RESOLVE`
 - 调整登录流程到 `driver.on_startup` 中
 
 ### 0.3.1
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-multincm Version: 0.3.2 Summary: NCM
+Metadata-Version: 2.1 Name: nonebot-plugin-multincm Version: 0.3.3 Summary: NCM
 Song Searcher Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
 Author-Email: student_2333
 126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
 nonebot-plugin-multincm Requires-Python: <4.0,>=3.8 Requires-Dist:
 nonebot2>=2.0.0-rc.1 Requires-Dist: nonebot-adapter-onebot>=2.2.0 Requires-
 Dist: pydantic>=1.10.4 Requires-Dist: pil-utils>=0.1.7 Requires-Dist:
 pyncm>=1.6.8.9.1 Requires-Dist: typing-extensions>=4.5.0 Requires-Dist:
@@ -41,32 +41,34 @@
 "nonebot_plugin_multincm" ] ```  ## âï¸ éç½® å¦æä½ å®è£äº [nonebot-
 plugin-ncm](https://github.com/kitUIN/nonebot-plugin-
 ncm)ï¼æ¬æä»¶ä¼ä¸å¶å±ç¨åä¸ä¸ª
 Sessionï¼å°±å¯ä»¥ä¸ç¨å¡«ä¸é¢çè´¦å·å¯ç äº
 ä¸é¢éç½®ä¸­ï¼ææºå·ç»å½ å é®ç®±ç»å½ãææå¯ç  å MD5
 å¯ç åå¸ åéå¶ä¸å¡«åå³å¯ å¨ nonebot2 é¡¹ç®ç `.env`
 æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« | é»è®¤å¼ |
-è¯´æ | | :------------------: | :--: | :-----: | :---------------------------
-------------------------------------: | | `NCM_CTCODE` | å¦ | `86` |
+è¯´æ | | :----------------------: | :--: | :-----: | :-----------------------
+----------------------------------------: | | `NCM_CTCODE` | å¦ | `86` |
 ææºå·ç»å½ç¨ï¼ç»å½ææºåºå· | | `NCM_PHONE` | å¦ | æ  |
 ææºå·ç»å½ç¨ï¼ç»å½ææºå· | | `NCM_EMAIL` | å¦ | æ  |
 é®ç®±ç»å½ç¨ï¼ç»å½é®ç®± | | `NCM_PASSWORD` | å¦ | æ  |
 å¸å·ææå¯ç ï¼é®ç®±ç»å½æ¶ä¸ºé®ç®±å¯ç  | | `NCM_PASSWORD_HASH` |
 å¦ | æ  | å¸å·å¯ç  MD5 åå¸ï¼é®ç®±ç»å½æ¶ä¸ºé®ç®±å¯ç  | |
 `NCM_LIST_LIMIT` | å¦ | `20` | æ­æ²åè¡¨æ¯é¡µçæå¤§æ°é | |
 `NCM_LIST_FONT` | å¦ | æ  | æ¸²ææ­æ²åè¡¨ä½¿ç¨çå­ä½ | |
 `NCM_MAX_NAME_LEN` | å¦ | `600` |
 æ­æ²åè¡¨ä¸­æ­ååçæå¤§ææ¬å®½åº¦ï¼åç´ ï¼ | |
 `NCM_MAX_ARTIST_LEN` | å¦ | `400` |
 æ­æ²åè¡¨ä¸­æ­æåçæå¤§ææ¬å®½åº¦ï¼åç´ ï¼ | |
 `NCM_MSG_CACHE_TIME` | å¦ | `3600` | ç¼å­ Bot å·²åéé³ä¹å¡ççé³ä¹
 ID å ç¨æ·æè¿ä¸æ¬¡æä½ çæ¶é¿ï¼ç§ï¼ | | `NCM_AUTO_RESOLVE` | å¦
 | `False` |
-å½ç¨æ·åéé³ä¹é¾æ¥æ¶ï¼æ¯å¦èªå¨è§£æå¹¶åéé³ä¹å¡ç | ##
-ð ä½¿ç¨ ### æä»¤ - ç¹æ­ [æ­æ²å / é³ä¹ ID] -
+å½ç¨æ·åéé³ä¹é¾æ¥æ¶ï¼æ¯å¦èªå¨è§£æå¹¶åéé³ä¹å¡ç | |
+`NCM_ILLEGAL_CMD_FINISH` | å¦ | `False` |
+å½ç¨æ·å¨ç¹æ­æ¶è¾å¥äºéæ³æä»¤ï¼æ¯å¦ç´æ¥éåºç¹æ­ | ## ð
+ä½¿ç¨ ### æä»¤ - ç¹æ­ [æ­æ²å / é³ä¹ ID] -
 ä»ç»ï¼æç´¢æ­æ²ãå½è¾å¥é³ä¹ ID æ¶ä¼ç´æ¥åéå¯¹åºé³ä¹ -
 å«åï¼`ç½æäº`ã`wyy` - çµå° [æ­æ²å / èç® ID] -
 ä»ç»ï¼æç´¢çµå°èç®ãå½è¾å¥çµå° ID æ¶ä¼ç´æ¥åéå¯¹åºèç®
 - å«åï¼`å£°é³`ã`ç½æçµå°`ã`wydt`ã`wydj` - è§£æ [åå¤
 é³ä¹å¡ç / é¾æ¥] - ä»ç»ï¼è·åè¯¥ é³ä¹ / çµå°èç®
 çæ­æ¾é¾æ¥å¹¶ä½¿ç¨èªå®ä¹å¡çåé -
 å«åï¼`resolve`ã`parse`ã`get` - æ­è¯ [åå¤ é³ä¹å¡ç / é¾æ¥] -
@@ -85,15 +87,17 @@
 é¡¹ç®ä½¿ç¨çç½æäº API è°ç¨åº ### [Binaryify/NeteaseCloudMusicApi]
 (https://github.com/Binaryify/NeteaseCloudMusicApi) é¡¹ç®çµå°ç¸å³ API
 æ¥æº ### [MeetWq/pil-utils](https://github.com/MeetWq/pil-utils) è¶å¥½ç¨ç
 Pillow è¾å©åº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.3.2 - æ°å¢éç½®é¡¹
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.3.3 - æ°å¢éç½®é¡¹
+`NCM_ILLEGAL_CMD_FINISH` - å¨æªå¯ç¨ `NCM_ILLEGAL_CMD_FINISH`
+æ¶è¾å¥éè¯¯æä»¤å°ä¼æç¤ºç¨æ·éåºç¹æ­ ### 0.3.2 - æ°å¢éç½®é¡¹
 `NCM_MSG_CACHE_TIME`ã`NCM_AUTO_RESOLVE` - è°æ´ç»å½æµç¨å°
 `driver.on_startup` ä¸­ ### 0.3.1 - ä¿®å¤çµå°ç¸å³ bug ### 0.3.0 -
 æ¯æçµå°èç®çè§£æä¸ç¹æ­ ### 0.2.5 - `è§£æ`ã`æ­è¯`ã`é¾æ¥`
 æä»¤å¯ä»¥ç´æ¥æ ¹æ® Bot åéçä¸ä¸ªé³ä¹å¡çä½åºååºäº -
 æ­è¯è§£æä¼åå¹¶å¤è¡ç©ºè¡åå»æé¦å°¾ç©ºè¡äº -
 ç°å¨æä»¶ä¼å®æ¶æ¸çèªèº«åå­ä¸­çç¼å­äº ### 0.2.4 -
 ä¿®å¤ä¸ä¸ªæ­è¯è§£æ bug ### 0.2.3 - å¾®è°æ­æ²åè¡¨æç -
```

