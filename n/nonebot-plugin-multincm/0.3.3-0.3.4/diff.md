# Comparing `tmp/nonebot_plugin_multincm-0.3.3.tar.gz` & `tmp/nonebot_plugin_multincm-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_multincm-0.3.3.tar", last modified: Tue May 30 15:59:35 2023, max compression
+gzip compressed data, was "nonebot_plugin_multincm-0.3.4.tar", last modified: Tue May 30 19:35:15 2023, max compression
```

## Comparing `nonebot_plugin_multincm-0.3.3.tar` & `nonebot_plugin_multincm-0.3.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1069 2023-05-30 15:59:18.886468 nonebot_plugin_multincm-0.3.3/LICENSE
--rw-r--r--   0        0        0     8484 2023-05-30 15:59:18.886468 nonebot_plugin_multincm-0.3.3/README.md
--rw-r--r--   0        0        0     1646 2023-05-30 15:59:18.886468 nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/__init__.py
--rw-r--r--   0        0        0    12222 2023-05-30 15:59:18.886468 nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/__main__.py
--rw-r--r--   0        0        0      623 2023-05-30 15:59:18.886468 nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/config.py
--rw-r--r--   0        0        0      134 2023-05-30 15:59:18.886468 nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/const.py
--rw-r--r--   0        0        0     5556 2023-05-30 15:59:18.886468 nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/data_source.py
--rw-r--r--   0        0        0    11669 2023-05-30 15:59:18.886468 nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/draw.py
--rw-r--r--   0        0        0     2957 2023-05-30 15:59:18.886468 nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/lrc_parser.py
--rw-r--r--   0        0        0     2279 2023-05-30 15:59:18.886468 nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/msg_cache.py
--rw-r--r--   0        0        0   212591 2023-05-30 15:59:18.890468 nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/res/bg.jpg
--rw-r--r--   0        0        0     3007 2023-05-30 15:59:18.890468 nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/types.py
--rw-r--r--   0        0        0      851 2023-05-30 15:59:18.890468 nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/utils.py
--rw-r--r--   0        0        0      867 2023-05-30 15:59:35.358548 nonebot_plugin_multincm-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     9434 1970-01-01 00:00:00.000000 nonebot_plugin_multincm-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-30 19:34:59.605112 nonebot_plugin_multincm-0.3.4/LICENSE
+-rw-r--r--   0        0        0     8547 2023-05-30 19:34:59.605112 nonebot_plugin_multincm-0.3.4/README.md
+-rw-r--r--   0        0        0     1646 2023-05-30 19:34:59.605112 nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/__init__.py
+-rw-r--r--   0        0        0    12222 2023-05-30 19:34:59.605112 nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/__main__.py
+-rw-r--r--   0        0        0      623 2023-05-30 19:34:59.605112 nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/config.py
+-rw-r--r--   0        0        0      134 2023-05-30 19:34:59.605112 nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/const.py
+-rw-r--r--   0        0        0     5556 2023-05-30 19:34:59.605112 nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/data_source.py
+-rw-r--r--   0        0        0    11669 2023-05-30 19:34:59.605112 nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/draw.py
+-rw-r--r--   0        0        0     2928 2023-05-30 19:34:59.605112 nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/lrc_parser.py
+-rw-r--r--   0        0        0     2279 2023-05-30 19:34:59.605112 nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/msg_cache.py
+-rw-r--r--   0        0        0   212591 2023-05-30 19:34:59.609112 nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/res/bg.jpg
+-rw-r--r--   0        0        0     3007 2023-05-30 19:34:59.609112 nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/types.py
+-rw-r--r--   0        0        0      851 2023-05-30 19:34:59.609112 nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/utils.py
+-rw-r--r--   0        0        0      867 2023-05-30 19:35:15.541289 nonebot_plugin_multincm-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     9497 1970-01-01 00:00:00.000000 nonebot_plugin_multincm-0.3.4/PKG-INFO
```

### Comparing `nonebot_plugin_multincm-0.3.3/LICENSE` & `nonebot_plugin_multincm-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.3/README.md` & `nonebot_plugin_multincm-0.3.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -213,14 +213,18 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.3.4
+
+- 修复分割线下会显示歌词翻译的问题
+
 ### 0.3.3
 
 - 新增配置项 `NCM_ILLEGAL_CMD_FINISH`
 - 在未启用 `NCM_ILLEGAL_CMD_FINISH` 时输入错误指令将会提示用户退出点歌
 
 ### 0.3.2
```

#### html2text {}

```diff
@@ -73,15 +73,16 @@
 é¡¹ç®ä½¿ç¨çç½æäº API è°ç¨åº ### [Binaryify/NeteaseCloudMusicApi]
 (https://github.com/Binaryify/NeteaseCloudMusicApi) é¡¹ç®çµå°ç¸å³ API
 æ¥æº ### [MeetWq/pil-utils](https://github.com/MeetWq/pil-utils) è¶å¥½ç¨ç
 Pillow è¾å©åº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.3.3 - æ°å¢éç½®é¡¹
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.3.4 -
+ä¿®å¤åå²çº¿ä¸ä¼æ¾ç¤ºæ­è¯ç¿»è¯çé®é¢ ### 0.3.3 - æ°å¢éç½®é¡¹
 `NCM_ILLEGAL_CMD_FINISH` - å¨æªå¯ç¨ `NCM_ILLEGAL_CMD_FINISH`
 æ¶è¾å¥éè¯¯æä»¤å°ä¼æç¤ºç¨æ·éåºç¹æ­ ### 0.3.2 - æ°å¢éç½®é¡¹
 `NCM_MSG_CACHE_TIME`ã`NCM_AUTO_RESOLVE` - è°æ´ç»å½æµç¨å°
 `driver.on_startup` ä¸­ ### 0.3.1 - ä¿®å¤çµå°ç¸å³ bug ### 0.3.0 -
 æ¯æçµå°èç®çè§£æä¸ç¹æ­ ### 0.2.5 - `è§£æ`ã`æ­è¯`ã`é¾æ¥`
 æä»¤å¯ä»¥ç´æ¥æ ¹æ® Bot åéçä¸ä¸ªé³ä¹å¡çä½åºååºäº -
 æ­è¯è§£æä¼åå¹¶å¤è¡ç©ºè¡åå»æé¦å°¾ç©ºè¡äº -
```

### Comparing `nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/__init__.py` & `nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from nonebot.plugin import PluginMetadata, require
 
 require("nonebot_plugin_apscheduler")
 
 from . import __main__ as __main__  # noqa: E402
 from .config import ConfigModel  # noqa: E402
 
-__version__ = "0.3.3"
+__version__ = "0.3.4"
 __plugin_meta__ = PluginMetadata(
     "MultiNCM",
     "网易云多选点歌",
     (
         "指令列表：\n"
         "▶ 点歌 [歌曲名 / 音乐 ID]\n"
         "    ▷ 介绍：搜索歌曲。当输入音乐 ID 时会直接发送对应音乐\n"
```

### Comparing `nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/__main__.py` & `nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/__main__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/config.py` & `nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/data_source.py` & `nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/draw.py` & `nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/draw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/lrc_parser.py` & `nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/lrc_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import re
 from dataclasses import dataclass
-from typing import Callable, List, Optional, TypeVar
-
-T = TypeVar("T")
+from typing import List, Optional
 
 
 @dataclass
 class LrcLine:
     time: int
     """Lyric Time (ms)"""
     lrc: str
@@ -14,22 +12,14 @@
     skip_merge: bool = False
 
 
 LRC_TIME_REGEX = r"(?P<min>\d+):(?P<sec>\d+)([\.:](?P<mili>\d+))?(-(?P<meta>\d))?"
 LRC_LINE_REGEX = re.compile(rf"^((\[{LRC_TIME_REGEX}\])+)(?P<lrc>.*)$", re.M)
 
 
-def find_last(array: List[T], predicate: Callable[[T], bool]) -> Optional[T]:
-    for i in range(len(array) - 1, -1, -1):
-        it = array[i]
-        if predicate(it):
-            return it
-    return None
-
-
 def parse(
     lrc: str,
     ignore_empty: bool = False,
     merge_empty: bool = True,
 ) -> List[LrcLine]:
     parsed = []
     for line in re.finditer(LRC_LINE_REGEX, lrc):
@@ -65,32 +55,39 @@
 
         parsed = new_parsed
 
     parsed.sort(key=lambda x: x.time)
     return parsed
 
 
+def strip_lrc_lines(lines: List[LrcLine]) -> List[LrcLine]:
+    for lrc in lines:
+        lrc.lrc = lrc.lrc.strip()
+    return lines
+
+
 def merge(
     *lyrics: List[LrcLine],
     threshold: int = 20,
     replace_empty_line: Optional[str] = "--------",
 ) -> List[List[LrcLine]]:
     lyrics = tuple(x.copy() for x in lyrics)
 
     for lrc in lyrics:
         while not lrc[-1].lrc:
             lrc.pop()
 
-    main_lyric = lyrics[0]
-    sub_lyrics = lyrics[1:]
+    main_lyric = strip_lrc_lines(lyrics[0])
+    sub_lyrics = [strip_lrc_lines(x) for x in lyrics[1:]]
 
     if replace_empty_line:
         for x in main_lyric:
             if not x.lrc:
                 x.lrc = replace_empty_line
+                x.skip_merge = True
 
     merged: List[List[LrcLine]] = [[x] for x in main_lyric]
     for merged_line in merged:
         main_line = merged_line[0]
         main_time = main_line.time
 
         for sub_lrc in sub_lyrics:
```

### Comparing `nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/msg_cache.py` & `nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/msg_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/res/bg.jpg` & `nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/res/bg.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/types.py` & `nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/types.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.3/nonebot_plugin_multincm/utils.py` & `nonebot_plugin_multincm-0.3.4/nonebot_plugin_multincm/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.3.3/pyproject.toml` & `nonebot_plugin_multincm-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-multincm"
-version = "0.3.3"
+version = "0.3.4"
 description = "NCM Song Searcher"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0-rc.1",
     "nonebot-adapter-onebot>=2.2.0",
```

### Comparing `nonebot_plugin_multincm-0.3.3/PKG-INFO` & `nonebot_plugin_multincm-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-multincm
-Version: 0.3.3
+Version: 0.3.4
 Summary: NCM Song Searcher
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
 Requires-Python: <4.0,>=3.8
 Requires-Dist: nonebot2>=2.0.0-rc.1
@@ -239,14 +239,18 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.3.4
+
+- 修复分割线下会显示歌词翻译的问题
+
 ### 0.3.3
 
 - 新增配置项 `NCM_ILLEGAL_CMD_FINISH`
 - 在未启用 `NCM_ILLEGAL_CMD_FINISH` 时输入错误指令将会提示用户退出点歌
 
 ### 0.3.2
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-multincm Version: 0.3.3 Summary: NCM
+Metadata-Version: 2.1 Name: nonebot-plugin-multincm Version: 0.3.4 Summary: NCM
 Song Searcher Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
 Author-Email: student_2333
 126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
 nonebot-plugin-multincm Requires-Python: <4.0,>=3.8 Requires-Dist:
 nonebot2>=2.0.0-rc.1 Requires-Dist: nonebot-adapter-onebot>=2.2.0 Requires-
 Dist: pydantic>=1.10.4 Requires-Dist: pil-utils>=0.1.7 Requires-Dist:
 pyncm>=1.6.8.9.1 Requires-Dist: typing-extensions>=4.5.0 Requires-Dist:
@@ -87,15 +87,16 @@
 é¡¹ç®ä½¿ç¨çç½æäº API è°ç¨åº ### [Binaryify/NeteaseCloudMusicApi]
 (https://github.com/Binaryify/NeteaseCloudMusicApi) é¡¹ç®çµå°ç¸å³ API
 æ¥æº ### [MeetWq/pil-utils](https://github.com/MeetWq/pil-utils) è¶å¥½ç¨ç
 Pillow è¾å©åº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.3.3 - æ°å¢éç½®é¡¹
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.3.4 -
+ä¿®å¤åå²çº¿ä¸ä¼æ¾ç¤ºæ­è¯ç¿»è¯çé®é¢ ### 0.3.3 - æ°å¢éç½®é¡¹
 `NCM_ILLEGAL_CMD_FINISH` - å¨æªå¯ç¨ `NCM_ILLEGAL_CMD_FINISH`
 æ¶è¾å¥éè¯¯æä»¤å°ä¼æç¤ºç¨æ·éåºç¹æ­ ### 0.3.2 - æ°å¢éç½®é¡¹
 `NCM_MSG_CACHE_TIME`ã`NCM_AUTO_RESOLVE` - è°æ´ç»å½æµç¨å°
 `driver.on_startup` ä¸­ ### 0.3.1 - ä¿®å¤çµå°ç¸å³ bug ### 0.3.0 -
 æ¯æçµå°èç®çè§£æä¸ç¹æ­ ### 0.2.5 - `è§£æ`ã`æ­è¯`ã`é¾æ¥`
 æä»¤å¯ä»¥ç´æ¥æ ¹æ® Bot åéçä¸ä¸ªé³ä¹å¡çä½åºååºäº -
 æ­è¯è§£æä¼åå¹¶å¤è¡ç©ºè¡åå»æé¦å°¾ç©ºè¡äº -
```

