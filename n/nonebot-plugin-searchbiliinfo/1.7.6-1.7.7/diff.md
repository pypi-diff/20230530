# Comparing `tmp/nonebot_plugin_searchbiliinfo-1.7.6.tar.gz` & `tmp/nonebot_plugin_searchbiliinfo-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_searchbiliinfo-1.7.6.tar", max compression
+gzip compressed data, was "nonebot_plugin_searchbiliinfo-1.7.7.tar", max compression
```

## Comparing `nonebot_plugin_searchbiliinfo-1.7.6.tar` & `nonebot_plugin_searchbiliinfo-1.7.7.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1084 2022-12-03 13:20:36.036837 nonebot_plugin_searchbiliinfo-1.7.6/LICENSE
--rw-r--r--   0        0        0   102900 2023-04-10 09:15:46.214907 nonebot_plugin_searchbiliinfo-1.7.6/nonebot_plugin_searchBiliInfo/__init__.py
--rw-r--r--   0        0        0   356769 2023-03-07 03:59:53.911011 nonebot_plugin_searchbiliinfo-1.7.6/nonebot_plugin_searchBiliInfo/data.py
--rw-r--r--   0        0        0  6937547 2023-02-20 03:35:57.148057 nonebot_plugin_searchbiliinfo-1.7.6/nonebot_plugin_searchBiliInfo/data_medal.py
--rw-r--r--   0        0        0     3484 2023-02-24 08:29:21.055074 nonebot_plugin_searchbiliinfo-1.7.6/nonebot_plugin_searchBiliInfo/html/composition_page.html
--rw-r--r--   0        0        0     1264 2023-04-10 09:20:29.361603 nonebot_plugin_searchbiliinfo-1.7.6/pyproject.toml
--rw-r--r--   0        0        0    30178 2023-04-10 09:17:45.855439 nonebot_plugin_searchbiliinfo-1.7.6/README.md
--rw-r--r--   0        0        0    31306 1970-01-01 00:00:00.000000 nonebot_plugin_searchbiliinfo-1.7.6/setup.py
--rw-r--r--   0        0        0    30682 1970-01-01 00:00:00.000000 nonebot_plugin_searchbiliinfo-1.7.6/PKG-INFO
+-rw-r--r--   0        0        0     1084 2022-12-03 13:20:36.036837 nonebot_plugin_searchbiliinfo-1.7.7/LICENSE
+-rw-r--r--   0        0        0   105305 2023-05-30 06:53:00.675636 nonebot_plugin_searchbiliinfo-1.7.7/nonebot_plugin_searchBiliInfo/__init__.py
+-rw-r--r--   0        0        0   356769 2023-03-07 03:59:53.911011 nonebot_plugin_searchbiliinfo-1.7.7/nonebot_plugin_searchBiliInfo/data.py
+-rw-r--r--   0        0        0  6937547 2023-02-20 03:35:57.148057 nonebot_plugin_searchbiliinfo-1.7.7/nonebot_plugin_searchBiliInfo/data_medal.py
+-rw-r--r--   0        0        0     3484 2023-02-24 08:29:21.055074 nonebot_plugin_searchbiliinfo-1.7.7/nonebot_plugin_searchBiliInfo/html/composition_page.html
+-rw-r--r--   0        0        0     1264 2023-05-30 06:56:00.196509 nonebot_plugin_searchbiliinfo-1.7.7/pyproject.toml
+-rw-r--r--   0        0        0    30616 2023-05-30 06:54:55.337279 nonebot_plugin_searchbiliinfo-1.7.7/README.md
+-rw-r--r--   0        0        0    31110 1970-01-01 00:00:00.000000 nonebot_plugin_searchbiliinfo-1.7.7/PKG-INFO
```

### Comparing `nonebot_plugin_searchbiliinfo-1.7.6/LICENSE` & `nonebot_plugin_searchbiliinfo-1.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_searchbiliinfo-1.7.6/nonebot_plugin_searchBiliInfo/__init__.py` & `nonebot_plugin_searchbiliinfo-1.7.7/nonebot_plugin_searchBiliInfo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 /v急上升
 /v急下降
 /v舰团
 /vdd
 /v宏观
 /dmk查用户 昵称关键词或uid
 /dmk查直播 昵称关键词或uid
+/dmk分析 昵称关键词或uid
 /blg查弹幕 昵称关键词或uid
 /blg查入场 昵称关键词或uid
 /blg查礼物 昵称关键词或uid
 /blg直播记录 昵称关键词或uid
 /blg直播间sc 昵称关键词或uid
 /icu查直播 昵称关键词或uid
 /icu查直播 昵称关键词或uid
@@ -119,14 +120,15 @@
 catch_str30 = on_command('V急上升', aliases={"v急上升"})
 catch_str31 = on_command('V急下降', aliases={"v急下降"})
 catch_str32 = on_command('V舰团', aliases={"v舰团"})
 catch_str33 = on_command('VDD风云榜', aliases={"vdd风云榜", "vdd", "VDD"})
 catch_str34 = on_command('V宏观', aliases={"v宏观"})
 catch_str14 = on_command('dmk查用户', aliases={"DMK查用户", "danmakus查用户"})
 catch_str15 = on_command('dmk查直播', aliases={"DMK查直播", "danmakus查直播"})
+catch_str39 = on_command('dmk分析', aliases={"DMK分析", "danmakus分析"})
 catch_str16 = on_command('blg查弹幕', aliases={"BLG查弹幕", "biligank查弹幕"})
 catch_str17 = on_command('blg查入场', aliases={"BLG查入场", "biligank查入场"})
 catch_str18 = on_command('blg查礼物', aliases={"BLG查礼物", "biligank查礼物"})
 catch_str19 = on_command('blg直播记录', aliases={"BLG直播记录", "biligank直播记录"})
 catch_str20 = on_command('blg直播间sc', aliases={"BLG直播间sc", "blg直播间SC", "BLG直播间SC", "biligank直播间sc"})
 catch_str21 = on_command('icu查直播', aliases={"ICU查直播", "matsuri查直播"})
 catch_str23 = on_command('lap查用户', aliases={"LAP查用户"})
@@ -1256,14 +1258,63 @@
         pass
     except Exception as e:
         nonebot.logger.info(e)
         msg = '打开页面失败喵（看看后台日志吧）'
         await catch_str15.finish(Message(f'{msg}'), reply_message=True)
 
 
+# dmk分析
+@catch_str39.handle()
+async def _(bot: Bot, event: Event, msg: Message = CommandArg()):
+    content = msg.extract_plain_text()
+
+    temp = await data_preprocess(content)
+    if 0 == temp["code"]:
+        content = temp["uid"]
+    else:
+        nonebot.logger.info(temp)
+        msg = '查询不到：' + content + ' 的相关信息。\nError code：' + str(temp["code"])
+        await catch_str39.finish(Message(f'{msg}'), reply_message=True)
+
+    await catch_str39.send("正在获取数据中，请耐心等待...", reply_message=True)
+
+    try:
+        async with get_new_page(viewport={"width": 1000, "height": 1200}) as page:
+            url = "https://danmakus.com/analyze/" + content + "?startTime=1669874804320&endTime=" + await get_current_timestamp_seconds(1)
+            # print(url)
+            await page.goto(
+                url,
+                timeout=2 * 60 * 1000,
+                wait_until="networkidle",
+            )
+            # 等待页面加载完成
+            # await page.wait_for_selector('.echarts')
+            await page.wait_for_selector('.n-collapse-item__header-main', timeout=60 * 1000)
+            # 删除小作文
+            click_js = 'document.getElementsByClassName("n-collapse-item__header-main")[1].click()'
+            # 执行 JavaScript 代码
+            result = await page.evaluate(click_js)
+            nonebot.logger.debug(result)
+            await asyncio.sleep(5)
+            temp_path = "./data/danmakus.com_analyze" + await get_current_timestamp_seconds() + ".png"
+            pic = await page.screenshot(full_page=True, path=temp_path)
+
+        await catch_str39.finish(MessageSegment.image(pic))
+    except TimeoutError as e:
+        nonebot.logger.info(e)
+        msg = '打开页面超时喵~可能是网络问题或是对面寄了'
+        await catch_str39.finish(Message(f'{msg}'), reply_message=True)
+    except FinishedException:
+        pass
+    except Exception as e:
+        nonebot.logger.info(e)
+        msg = '打开页面失败喵（看看后台日志吧）'
+        await catch_str39.finish(Message(f'{msg}'), reply_message=True)
+
+
 # blg查弹幕
 @catch_str16.handle()
 async def _(bot: Bot, event: Event, msg: Message = CommandArg()):
     content = msg.extract_plain_text()
 
     temp = await data_preprocess(content)
     if 0 == temp["code"]:
@@ -2327,18 +2378,21 @@
 
 # markdown特殊字符过滤，并当字符串每超过20个时，在其后插入一个<br>
 async def filter_markdown(text):
     filtered_text = re.sub(r'[_*#->`]', '', text)
     return re.sub(r"(.{20})", r"\1<br>", filtered_text, 0, re.DOTALL)
 
 
-# 获取时间戳的当前的秒
-async def get_current_timestamp_seconds():
+# 获取时间戳的当前的秒/毫秒 默认0 秒，1 毫秒
+async def get_current_timestamp_seconds(type=0):
     current_timestamp = int(time.time())
-    return str(current_timestamp % 60)
+    if type == 0:
+        return str(current_timestamp % 60)
+    else:
+        return str(int(current_timestamp * 1000))
 
 
 # 获取年月日（y-m-d）字符串，可以传入日期偏移值
 async def get_date_str_with_offset(offset):
     # 获取今天的日期对象
     today = datetime.date.today()
     # 根据偏移值创建时间差对象
```

### Comparing `nonebot_plugin_searchbiliinfo-1.7.6/nonebot_plugin_searchBiliInfo/data.py` & `nonebot_plugin_searchbiliinfo-1.7.7/nonebot_plugin_searchBiliInfo/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_searchbiliinfo-1.7.6/nonebot_plugin_searchBiliInfo/data_medal.py` & `nonebot_plugin_searchbiliinfo-1.7.7/nonebot_plugin_searchBiliInfo/data_medal.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_searchbiliinfo-1.7.6/nonebot_plugin_searchBiliInfo/html/composition_page.html` & `nonebot_plugin_searchbiliinfo-1.7.7/nonebot_plugin_searchBiliInfo/html/composition_page.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_searchbiliinfo-1.7.6/pyproject.toml` & `nonebot_plugin_searchbiliinfo-1.7.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-searchbiliinfo"
-version = "1.7.6"
+version = "1.7.7"
 description = "A plugin for nonebot2. Query Bilibili user information（一个Nonebot2的插件，b站用户信息查询插件【粉丝、舰团信息；直播收益数据；直播观看信息；关键词搜昵称、UID；主播营收榜单；查成分；查牌子等】）"
 authors = ["Ikaros <327209194@qq.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_searchbiliinfo"}]
 homepage = "https://github.com/Ikaros-521/nonebot_plugin_searchBiliInfo"
 repository = "https://github.com/Ikaros-521/nonebot_plugin_searchBiliInfo"
```

### Comparing `nonebot_plugin_searchbiliinfo-1.7.6/README.md` & `nonebot_plugin_searchbiliinfo-1.7.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
   - [/v急上升 或 /V急上升](#v%E6%80%A5%E4%B8%8A%E5%8D%87-%E6%88%96-v%E6%80%A5%E4%B8%8A%E5%8D%87)
   - [/v急下降 或 /V急下降](#v%E6%80%A5%E4%B8%8B%E9%99%8D-%E6%88%96-v%E6%80%A5%E4%B8%8B%E9%99%8D)
   - [/v舰团 或 /V舰团](#v%E8%88%B0%E5%9B%A2-%E6%88%96-v%E8%88%B0%E5%9B%A2)
   - [/vdd 或 /VDD 或 /VDD风云榜 或 /vdd风云榜](#vdd-%E6%88%96-vdd-%E6%88%96-vdd%E9%A3%8E%E4%BA%91%E6%A6%9C-%E6%88%96-vdd%E9%A3%8E%E4%BA%91%E6%A6%9C)
   - [/V宏观 或 /v宏观](#v%E5%AE%8F%E8%A7%82-%E6%88%96-v%E5%AE%8F%E8%A7%82)
   - [/dmk查用户 或 /DMK查用户](#dmk%E6%9F%A5%E7%94%A8%E6%88%B7-%E6%88%96-dmk%E6%9F%A5%E7%94%A8%E6%88%B7)
   - [/dmk查直播 或 /DMK查直播](#dmk%E6%9F%A5%E7%9B%B4%E6%92%AD-%E6%88%96-dmk%E6%9F%A5%E7%9B%B4%E6%92%AD)
+  - [/dmk分析 或 /DMK分析](#dmk%E5%88%86%E6%9E%90-%E6%88%96-dmk%E5%88%86%E6%9E%90)
   - [/blg查弹幕 或 /BLG查弹幕](#blg%E6%9F%A5%E5%BC%B9%E5%B9%95-%E6%88%96-blg%E6%9F%A5%E5%BC%B9%E5%B9%95)
   - [/blg查入场 或 /BLG查入场](#blg%E6%9F%A5%E5%85%A5%E5%9C%BA-%E6%88%96-blg%E6%9F%A5%E5%85%A5%E5%9C%BA)
   - [/blg查礼物 或 /BLG查礼物](#blg%E6%9F%A5%E7%A4%BC%E7%89%A9-%E6%88%96-blg%E6%9F%A5%E7%A4%BC%E7%89%A9)
   - [/blg直播记录 或 /BLG直播记录](#blg%E7%9B%B4%E6%92%AD%E8%AE%B0%E5%BD%95-%E6%88%96-blg%E7%9B%B4%E6%92%AD%E8%AE%B0%E5%BD%95)
   - [/blg直播间sc 或 /BLG直播间SC](#blg%E7%9B%B4%E6%92%AD%E9%97%B4sc-%E6%88%96-blg%E7%9B%B4%E6%92%AD%E9%97%B4sc)
   - [/icu查直播 或 /ICU查直播 或 /matsuri查直播](#icu%E6%9F%A5%E7%9B%B4%E6%92%AD-%E6%88%96-icu%E6%9F%A5%E7%9B%B4%E6%92%AD-%E6%88%96-matsuri%E6%9F%A5%E7%9B%B4%E6%92%AD)
   - [/lap查用户 或 /LAP查用户](#lap%E6%9F%A5%E7%94%A8%E6%88%B7-%E6%88%96-lap%E6%9F%A5%E7%94%A8%E6%88%B7)
@@ -316,14 +317,20 @@
 
 ### /dmk查直播 或 /DMK查直播
 命令结构：```/dmk查直播 (uid:或UID:或：或:)+用户uid或昵称关键词```  
 例如：```/dmk查直播 uid:3709626``` 或 ```/DMK查直播 Love丶伊卡洛斯```  
 bot返回内容(图片)：  
 ![](docs/dmk_live.png)
 
+### /dmk分析 或 /DMK分析
+命令结构：```/dmk分析 (uid:或UID:或：或:)+用户uid或昵称关键词```  
+例如：```/dmk分析 uid:3709626``` 或 ```/DMK分析 Love丶伊卡洛斯```  
+bot返回内容(图片)：  
+![](docs/dmk_analyze.png)
+
 ### /blg查弹幕 或 /BLG查弹幕
 命令结构：```/blg查弹幕 (uid:或UID:或：或:)+用户uid或昵称关键词```  
 例如：```/blg查弹幕 uid:3709626``` 或 ```/BLG查弹幕 Love丶伊卡洛斯```  
 bot返回内容(图片)：  
 ![](docs/blg_danmu.png)
 
 ### /blg查入场 或 /BLG查入场
@@ -688,14 +695,17 @@
 
 ### 1.7.5
 bug修复  
 
 ### 1.7.6
 `查`命令，追加返回用户主页和直播间链接。    
 
+### 1.7.7
+新增`dmk分析`功能，由danmakus分析用户观看弹幕等数据。  
+
 </details>
 
 ## 致谢
 - [nonebot-plugin-htmlrender](https://github.com/kexue-z/nonebot-plugin-htmlrender) - 图片合成的好手
 - [danmakus.com](https://danmakus.com/) - b站主播、用户弹幕直播信息等来源（开放API接口很赞！）
 - [vtbs.moe](https://vtbs.moe) - VTB本地数据信息来源（还有数据提供，TQL）  
 - [laplace.live](https://laplace.live/) - 也是b站主播用户查询站点，部分数据也是源自danmakus，UI不错
```

#### html2text {}

```diff
@@ -38,21 +38,22 @@
 %E6%88%96-v%E8%88%B0%E5%9B%A2) - [/vdd æ /VDD æ /VDDé£äºæ¦ æ /
 vddé£äºæ¦](#vdd-%E6%88%96-vdd-%E6%88%96-vdd%E9%A3%8E%E4%BA%91%E6%A6%9C-
 %E6%88%96-vdd%E9%A3%8E%E4%BA%91%E6%A6%9C) - [/Vå®è§ æ /vå®è§]
 (#v%E5%AE%8F%E8%A7%82-%E6%88%96-v%E5%AE%8F%E8%A7%82) - [/dmkæ¥ç¨æ· æ /
 DMKæ¥ç¨æ·](#dmk%E6%9F%A5%E7%94%A8%E6%88%B7-%E6%88%96-
 dmk%E6%9F%A5%E7%94%A8%E6%88%B7) - [/dmkæ¥ç´æ­ æ /DMKæ¥ç´æ­]
 (#dmk%E6%9F%A5%E7%9B%B4%E6%92%AD-%E6%88%96-dmk%E6%9F%A5%E7%9B%B4%E6%92%AD) - [/
-blgæ¥å¼¹å¹ æ /BLGæ¥å¼¹å¹](#blg%E6%9F%A5%E5%BC%B9%E5%B9%95-%E6%88%96-
-blg%E6%9F%A5%E5%BC%B9%E5%B9%95) - [/blgæ¥å¥åº æ /BLGæ¥å¥åº]
-(#blg%E6%9F%A5%E5%85%A5%E5%9C%BA-%E6%88%96-blg%E6%9F%A5%E5%85%A5%E5%9C%BA) - [/
-blgæ¥ç¤¼ç© æ /BLGæ¥ç¤¼ç©](#blg%E6%9F%A5%E7%A4%BC%E7%89%A9-%E6%88%96-
-blg%E6%9F%A5%E7%A4%BC%E7%89%A9) - [/blgç´æ­è®°å½ æ /BLGç´æ­è®°å½]
-(#blg%E7%9B%B4%E6%92%AD%E8%AE%B0%E5%BD%95-%E6%88%96-
-blg%E7%9B%B4%E6%92%AD%E8%AE%B0%E5%BD%95) - [/blgç´æ­é´sc æ /
+dmkåæ æ /DMKåæ](#dmk%E5%88%86%E6%9E%90-%E6%88%96-
+dmk%E5%88%86%E6%9E%90) - [/blgæ¥å¼¹å¹ æ /BLGæ¥å¼¹å¹]
+(#blg%E6%9F%A5%E5%BC%B9%E5%B9%95-%E6%88%96-blg%E6%9F%A5%E5%BC%B9%E5%B9%95) - [/
+blgæ¥å¥åº æ /BLGæ¥å¥åº](#blg%E6%9F%A5%E5%85%A5%E5%9C%BA-%E6%88%96-
+blg%E6%9F%A5%E5%85%A5%E5%9C%BA) - [/blgæ¥ç¤¼ç© æ /BLGæ¥ç¤¼ç©]
+(#blg%E6%9F%A5%E7%A4%BC%E7%89%A9-%E6%88%96-blg%E6%9F%A5%E7%A4%BC%E7%89%A9) - [/
+blgç´æ­è®°å½ æ /BLGç´æ­è®°å½](#blg%E7%9B%B4%E6%92%AD%E8%AE%B0%E5%BD%95-
+%E6%88%96-blg%E7%9B%B4%E6%92%AD%E8%AE%B0%E5%BD%95) - [/blgç´æ­é´sc æ /
 BLGç´æ­é´SC](#blg%E7%9B%B4%E6%92%AD%E9%97%B4sc-%E6%88%96-
 blg%E7%9B%B4%E6%92%AD%E9%97%B4sc) - [/icuæ¥ç´æ­ æ /ICUæ¥ç´æ­ æ /
 matsuriæ¥ç´æ­](#icu%E6%9F%A5%E7%9B%B4%E6%92%AD-%E6%88%96-
 icu%E6%9F%A5%E7%9B%B4%E6%92%AD-%E6%88%96-matsuri%E6%9F%A5%E7%9B%B4%E6%92%AD) -
 [/lapæ¥ç¨æ· æ /LAPæ¥ç¨æ·](#lap%E6%9F%A5%E7%94%A8%E6%88%B7-%E6%88%96-
 lap%E6%9F%A5%E7%94%A8%E6%88%B7) - [/lapæ¥çå­ æ /LAPæ¥çå­]
 (#lap%E6%9F%A5%E7%89%8C%E5%AD%90-%E6%88%96-lap%E6%9F%A5%E7%89%8C%E5%AD%90) - [/
@@ -183,34 +184,37 @@
 DMKæ¥ç¨æ· å½ä»¤ç»æï¼```/dmkæ¥ç¨æ· (uid:æUID:æï¼æ:
 )+ç¨æ·uidææµç§°å³é®è¯``` ä¾å¦ï¼```/dmkæ¥ç¨æ· uid:3709626``` æ
 ```/DMKæ¥ç¨æ· Loveä¸¶ä¼å¡æ´æ¯``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/
 dmk_user.png) ### /dmkæ¥ç´æ­ æ /DMKæ¥ç´æ­ å½ä»¤ç»æï¼```/
 dmkæ¥ç´æ­ (uid:æUID:æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯```
 ä¾å¦ï¼```/dmkæ¥ç´æ­ uid:3709626``` æ ```/DMKæ¥ç´æ­
 Loveä¸¶ä¼å¡æ´æ¯``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/dmk_live.png) ### /
-blgæ¥å¼¹å¹ æ /BLGæ¥å¼¹å¹ å½ä»¤ç»æï¼```/blgæ¥å¼¹å¹ (uid:æUID:
-æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯``` ä¾å¦ï¼```/blgæ¥å¼¹å¹ uid:
-3709626``` æ ```/BLGæ¥å¼¹å¹ Loveä¸¶ä¼å¡æ´æ¯``` botè¿ååå®¹
-(å¾ç)ï¼ ![](docs/blg_danmu.png) ### /blgæ¥å¥åº æ /BLGæ¥å¥åº
-å½ä»¤ç»æï¼```/blgæ¥å¥åº (uid:æUID:æï¼æ:
-)+ç¨æ·uidææµç§°å³é®è¯``` ä¾å¦ï¼```/blgæ¥å¥åº uid:3709626``` æ
-```/BLGæ¥å¥åº Loveä¸¶ä¼å¡æ´æ¯``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/
-blg_enter.png) ### /blgæ¥ç¤¼ç© æ /BLGæ¥ç¤¼ç© å½ä»¤ç»æï¼```/
-blgæ¥ç¤¼ç© (uid:æUID:æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯```
-ä¾å¦ï¼```/blgæ¥ç¤¼ç© uid:3709626``` æ ```/BLGæ¥ç¤¼ç©
-Loveä¸¶ä¼å¡æ´æ¯``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/blg_gift.png) ### /
-blgç´æ­è®°å½ æ /BLGç´æ­è®°å½ å½ä»¤ç»æï¼```/blgç´æ­è®°å½ (uid:
-æUID:æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯``` ä¾å¦ï¼```/blgç´æ­è®°å½
-uid:3709626``` æ ```/BLGç´æ­è®°å½ Loveä¸¶ä¼å¡æ´æ¯``` botè¿ååå®¹
-(å¾ç)ï¼ ![](docs/blg_tp.png) ### /blgç´æ­é´sc æ /BLGç´æ­é´SC
-å½ä»¤ç»æï¼```/blgç´æ­é´sc (uid:æUID:æï¼æ:
-)+ç¨æ·uidææµç§°å³é®è¯``` ä¾å¦ï¼```/blgç´æ­é´sc uid:3709626``` æ
-```/BLGç´æ­é´SC Loveä¸¶ä¼å¡æ´æ¯``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/
-blg_sc.png) ### /icuæ¥ç´æ­ æ /ICUæ¥ç´æ­ æ /matsuriæ¥ç´æ­
-å½ä»¤ç»æï¼```/icuæ¥ç´æ­ (uid:æUID:æï¼æ:
+dmkåæ æ /DMKåæ å½ä»¤ç»æï¼```/dmkåæ (uid:æUID:æï¼æ:
+)+ç¨æ·uidææµç§°å³é®è¯``` ä¾å¦ï¼```/dmkåæ uid:3709626``` æ ```/
+DMKåæ Loveä¸¶ä¼å¡æ´æ¯``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/
+dmk_analyze.png) ### /blgæ¥å¼¹å¹ æ /BLGæ¥å¼¹å¹ å½ä»¤ç»æï¼```/
+blgæ¥å¼¹å¹ (uid:æUID:æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯```
+ä¾å¦ï¼```/blgæ¥å¼¹å¹ uid:3709626``` æ ```/BLGæ¥å¼¹å¹
+Loveä¸¶ä¼å¡æ´æ¯``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/blg_danmu.png) ### /
+blgæ¥å¥åº æ /BLGæ¥å¥åº å½ä»¤ç»æï¼```/blgæ¥å¥åº (uid:æUID:
+æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯``` ä¾å¦ï¼```/blgæ¥å¥åº uid:
+3709626``` æ ```/BLGæ¥å¥åº Loveä¸¶ä¼å¡æ´æ¯``` botè¿ååå®¹
+(å¾ç)ï¼ ![](docs/blg_enter.png) ### /blgæ¥ç¤¼ç© æ /BLGæ¥ç¤¼ç©
+å½ä»¤ç»æï¼```/blgæ¥ç¤¼ç© (uid:æUID:æï¼æ:
+)+ç¨æ·uidææµç§°å³é®è¯``` ä¾å¦ï¼```/blgæ¥ç¤¼ç© uid:3709626``` æ
+```/BLGæ¥ç¤¼ç© Loveä¸¶ä¼å¡æ´æ¯``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/
+blg_gift.png) ### /blgç´æ­è®°å½ æ /BLGç´æ­è®°å½ å½ä»¤ç»æï¼```/
+blgç´æ­è®°å½ (uid:æUID:æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯```
+ä¾å¦ï¼```/blgç´æ­è®°å½ uid:3709626``` æ ```/BLGç´æ­è®°å½
+Loveä¸¶ä¼å¡æ´æ¯``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/blg_tp.png) ### /
+blgç´æ­é´sc æ /BLGç´æ­é´SC å½ä»¤ç»æï¼```/blgç´æ­é´sc (uid:
+æUID:æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯``` ä¾å¦ï¼```/blgç´æ­é´sc
+uid:3709626``` æ ```/BLGç´æ­é´SC Loveä¸¶ä¼å¡æ´æ¯``` botè¿ååå®¹
+(å¾ç)ï¼ ![](docs/blg_sc.png) ### /icuæ¥ç´æ­ æ /ICUæ¥ç´æ­ æ /
+matsuriæ¥ç´æ­ å½ä»¤ç»æï¼```/icuæ¥ç´æ­ (uid:æUID:æï¼æ:
 )+ç¨æ·uidææµç§°å³é®è¯``` ä¾å¦ï¼```/icuæ¥ç´æ­ uid:3709626``` æ
 ```/ICUæ¥ç´æ­ Loveä¸¶ä¼å¡æ´æ¯``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/
 icu_live.png) ### /lapæ¥ç¨æ· æ /LAPæ¥ç¨æ· å½ä»¤ç»æï¼```/
 lapæ¥ç¨æ· (uid:æUID:æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯```
 ä¾å¦ï¼```/lapæ¥ç¨æ· uid:387636363``` æ ```/LAPæ¥ç¨æ· é«ãã```
 botè¿ååå®¹(å¾ç)ï¼ ![](docs/laplace_user.png) ### /lapæ¥çå­ æ /
 LAPæ¥çå­ å½ä»¤ç»æï¼```/lapæ¥çå­ (uid:æUID:æï¼æ:
@@ -349,15 +353,16 @@
 3.ä¼åè¯´æææ¡£ã ### 1.6.8 ä¿®å¤`lapdd`å½ä»¤ä¸ä¼ åçbugã ###
 1.6.9 æ°å¢æ­£åå¹éç`æè«`ç©æ³ï¼å·ä½çå½ä»¤è¯´æã ### 1.7.0
 ä¿®å¤htmlrenderå¯¼å¥é®é¢ã ### 1.7.1
 æ°å¢å½ä»¤`ehæ¥ç´æ­`æ`è¯¶å¿æ¥ç´æ­`ã ### 1.7.2
 ä¿®æ¹`ehæ¥ç´æ­`çè¯·æ±å°åä¸ºhttpï¼æå¡å¨ä¸è·è¯ä¹¦ä¸è¡ï¼ç»·ã
 ### 1.7.3 ä¿®æ¹`ehæ¥ç´æ­`ä¸ºplaywrightï¼é¾ç»·ã ### 1.7.4
 ä¿®æ¹`ehæ¥ç´æ­`ä¸ºç´æ¥è¯·æ±ï¼ä¸è¿è·³è¿äºsslã ### 1.7.5 bugä¿®å¤
-### 1.7.6 `æ¥`å½ä»¤ï¼è¿½å è¿åç¨æ·ä¸»é¡µåç´æ­é´é¾æ¥ã  ##
+### 1.7.6 `æ¥`å½ä»¤ï¼è¿½å è¿åç¨æ·ä¸»é¡µåç´æ­é´é¾æ¥ã ### 1.7.7
+æ°å¢`dmkåæ`åè½ï¼ç±danmakusåæç¨æ·è§çå¼¹å¹ç­æ°æ®ã  ##
 è´è°¢ - [nonebot-plugin-htmlrender](https://github.com/kexue-z/nonebot-plugin-
 htmlrender) - å¾çåæçå¥½æ - [danmakus.com](https://danmakus.com/) -
 bç«ä¸»æ­ãç¨æ·å¼¹å¹ç´æ­ä¿¡æ¯ç­æ¥æºï¼å¼æ¾APIæ¥å£å¾èµï¼ï¼ -
 [vtbs.moe](https://vtbs.moe) -
 VTBæ¬å°æ°æ®ä¿¡æ¯æ¥æºï¼è¿ææ°æ®æä¾ï¼TQLï¼ - [laplace.live]
 (https://laplace.live/) -
 ä¹æ¯bç«ä¸»æ­ç¨æ·æ¥è¯¢ç«ç¹ï¼é¨åæ°æ®ä¹æ¯æºèªdanmakusï¼UIä¸é
```

### Comparing `nonebot_plugin_searchbiliinfo-1.7.6/setup.py` & `nonebot_plugin_searchbiliinfo-1.7.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,808 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nonebot-plugin-searchbiliinfo
+Version: 1.7.7
+Summary: A plugin for nonebot2. Query Bilibili user information（一个Nonebot2的插件，b站用户信息查询插件【粉丝、舰团信息；直播收益数据；直播观看信息；关键词搜昵称、UID；主播营收榜单；查成分；查牌子等】）
+Home-page: https://github.com/Ikaros-521/nonebot_plugin_searchBiliInfo
+License: MIT
+Author: Ikaros
+Author-email: 327209194@qq.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.8.3,<4.0.0)
+Requires-Dist: asyncio (>=3.4.3,<4.0.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.1.3,<3.0.0)
+Requires-Dist: nonebot-plugin-htmlrender (>=0.2.0.1,<0.3.0.0)
+Requires-Dist: nonebot2 (>=2.0.0b5,<3.0.0)
+Project-URL: Documentation, https://github.com/Ikaros-521/nonebot_plugin_searchBiliInfo/blob/master/README.md
+Project-URL: Repository, https://github.com/Ikaros-521/nonebot_plugin_searchBiliInfo
+Description-Content-Type: text/markdown
 
-packages = \
-['nonebot_plugin_searchbiliinfo']
+<div align="center">
+  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
+  <br>
+  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
+</div>
 
-package_data = \
-{'': ['*'], 'nonebot_plugin_searchbiliinfo': ['html/*']}
+<div align="center">
 
-install_requires = \
-['aiohttp>=3.8.3,<4.0.0',
- 'asyncio>=3.4.3,<4.0.0',
- 'nonebot-adapter-onebot>=2.1.3,<3.0.0',
- 'nonebot-plugin-htmlrender>=0.2.0.1,<0.3.0.0',
- 'nonebot2>=2.0.0b5,<3.0.0']
-
-setup_kwargs = {
-    'name': 'nonebot-plugin-searchbiliinfo',
-    'version': '1.7.6',
-    'description': 'A plugin for nonebot2. Query Bilibili user information（一个Nonebot2的插件，b站用户信息查询插件【粉丝、舰团信息；直播收益数据；直播观看信息；关键词搜昵称、UID；主播营收榜单；查成分；查牌子等】）',
-    'long_description': '<div align="center">\n  <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>\n  <br>\n  <p><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>\n</div>\n\n<div align="center">\n\n# nonebot_plugin_searchBiliInfo\n  \n_✨ NoneBot b站用户信息查询插件 ✨_\n  \n<a href="https://github.com/Ikaros-521/nonebot_plugin_searchBiliInfo/stargazers">\n    <img alt="GitHub stars" src="https://img.shields.io/github/stars/Ikaros-521/nonebot_plugin_searchBiliInfo?color=%09%2300BFFF&style=flat-square">\n</a>\n<a href="https://github.com/Ikaros-521/nonebot_plugin_searchBiliInfo/issues">\n    <img alt="GitHub issues" src="https://img.shields.io/github/issues/Ikaros-521/nonebot_plugin_searchBiliInfo?color=Emerald%20green&style=flat-square">\n</a>\n<a href="https://github.com/Ikaros-521/nonebot_plugin_searchBiliInfo/network">\n    <img alt="GitHub forks" src="https://img.shields.io/github/forks/Ikaros-521/nonebot_plugin_searchBiliInfo?color=%2300BFFF&style=flat-square">\n</a>\n<a href="./LICENSE">\n    <img src="https://img.shields.io/github/license/Ikaros-521/nonebot_plugin_searchBiliInfo.svg" alt="license">\n</a>\n<a href="https://pypi.python.org/pypi/nonebot_plugin_searchBiliInfo">\n    <img src="https://img.shields.io/pypi/v/nonebot_plugin_searchBiliInfo.svg" alt="pypi">\n</a>\n<a href="https://www.python.org">\n    <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">\n</a>\n\n</div>\n\n适用于nonebot2 v11的b站用户信息查询插件【粉丝、舰团信息；直播收益数据；直播观看信息；关键词搜昵称、UID；主播营收榜单；查成分；查牌子等】  \n（ps：微调源码可以兼容其他版本）   \n调用的相关API源自b站官方接口、danmakus.com和vtbs.fun\n\n<!-- START doctoc generated TOC please keep comment here to allow auto update -->\n<!-- DON\'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->\n## 📖目录\n\n- [🔧 开发环境](#-%E5%BC%80%E5%8F%91%E7%8E%AF%E5%A2%83)\n- [💿 安装](#-%E5%AE%89%E8%A3%85)\n  - [1. nb-cli安装（推荐）](#1-nb-cli%E5%AE%89%E8%A3%85%E6%8E%A8%E8%8D%90)\n  - [2. 本地安装](#2-%E6%9C%AC%E5%9C%B0%E5%AE%89%E8%A3%85)\n  - [3. pip安装](#3-pip%E5%AE%89%E8%A3%85)\n  - [更新版本](#%E6%9B%B4%E6%96%B0%E7%89%88%E6%9C%AC)\n- [🔧 配置](#-%E9%85%8D%E7%BD%AE)\n  - [cookie获取方式](#cookie%E8%8E%B7%E5%8F%96%E6%96%B9%E5%BC%8F)\n  - [env配置](#env%E9%85%8D%E7%BD%AE)\n- [🎉 功能](#-%E5%8A%9F%E8%83%BD)\n- [👉 命令(命令前缀自行替换喵~)](#-%E5%91%BD%E4%BB%A4%E5%91%BD%E4%BB%A4%E5%89%8D%E7%BC%80%E8%87%AA%E8%A1%8C%E6%9B%BF%E6%8D%A2%E5%96%B5)\n  - [/查](#%E6%9F%A5)\n  - [/查直播](#%E6%9F%A5%E7%9B%B4%E6%92%AD)\n  - [/查舰团](#%E6%9F%A5%E8%88%B0%E5%9B%A2)\n  - [/查昵称](#%E6%9F%A5%E6%98%B5%E7%A7%B0)\n  - [/查收益](#%E6%9F%A5%E6%94%B6%E7%9B%8A)\n  - [/查观看](#%E6%9F%A5%E8%A7%82%E7%9C%8B)\n  - [/查观看2](#%E6%9F%A5%E8%A7%82%E7%9C%8B2)\n  - [/查弹幕](#%E6%9F%A5%E5%BC%B9%E5%B9%95)\n  - [/查弹幕2](#%E6%9F%A5%E5%BC%B9%E5%B9%952)\n  - [/查牌子](#%E6%9F%A5%E7%89%8C%E5%AD%90)\n  - [/查人气](#%E6%9F%A5%E4%BA%BA%E6%B0%94)\n  - [/查装扮](#%E6%9F%A5%E8%A3%85%E6%89%AE)\n  - [/营收](#%E8%90%A5%E6%94%B6)\n  - [/涨粉](#%E6%B6%A8%E7%B2%89)\n  - [/DD风云榜 或 /dd风云榜 或 /风云榜 (寄了)](#dd%E9%A3%8E%E4%BA%91%E6%A6%9C-%E6%88%96-dd%E9%A3%8E%E4%BA%91%E6%A6%9C-%E6%88%96-%E9%A3%8E%E4%BA%91%E6%A6%9C-%E5%AF%84%E4%BA%86)\n  - [/v详情 或 /V详情 或 /v详细 或 /V详细](#v%E8%AF%A6%E6%83%85-%E6%88%96-v%E8%AF%A6%E6%83%85-%E6%88%96-v%E8%AF%A6%E7%BB%86-%E6%88%96-v%E8%AF%A6%E7%BB%86)\n  - [/v直播势 或 /V直播势](#v%E7%9B%B4%E6%92%AD%E5%8A%BF-%E6%88%96-v%E7%9B%B4%E6%92%AD%E5%8A%BF)\n  - [/v急上升 或 /V急上升](#v%E6%80%A5%E4%B8%8A%E5%8D%87-%E6%88%96-v%E6%80%A5%E4%B8%8A%E5%8D%87)\n  - [/v急下降 或 /V急下降](#v%E6%80%A5%E4%B8%8B%E9%99%8D-%E6%88%96-v%E6%80%A5%E4%B8%8B%E9%99%8D)\n  - [/v舰团 或 /V舰团](#v%E8%88%B0%E5%9B%A2-%E6%88%96-v%E8%88%B0%E5%9B%A2)\n  - [/vdd 或 /VDD 或 /VDD风云榜 或 /vdd风云榜](#vdd-%E6%88%96-vdd-%E6%88%96-vdd%E9%A3%8E%E4%BA%91%E6%A6%9C-%E6%88%96-vdd%E9%A3%8E%E4%BA%91%E6%A6%9C)\n  - [/V宏观 或 /v宏观](#v%E5%AE%8F%E8%A7%82-%E6%88%96-v%E5%AE%8F%E8%A7%82)\n  - [/dmk查用户 或 /DMK查用户](#dmk%E6%9F%A5%E7%94%A8%E6%88%B7-%E6%88%96-dmk%E6%9F%A5%E7%94%A8%E6%88%B7)\n  - [/dmk查直播 或 /DMK查直播](#dmk%E6%9F%A5%E7%9B%B4%E6%92%AD-%E6%88%96-dmk%E6%9F%A5%E7%9B%B4%E6%92%AD)\n  - [/blg查弹幕 或 /BLG查弹幕](#blg%E6%9F%A5%E5%BC%B9%E5%B9%95-%E6%88%96-blg%E6%9F%A5%E5%BC%B9%E5%B9%95)\n  - [/blg查入场 或 /BLG查入场](#blg%E6%9F%A5%E5%85%A5%E5%9C%BA-%E6%88%96-blg%E6%9F%A5%E5%85%A5%E5%9C%BA)\n  - [/blg查礼物 或 /BLG查礼物](#blg%E6%9F%A5%E7%A4%BC%E7%89%A9-%E6%88%96-blg%E6%9F%A5%E7%A4%BC%E7%89%A9)\n  - [/blg直播记录 或 /BLG直播记录](#blg%E7%9B%B4%E6%92%AD%E8%AE%B0%E5%BD%95-%E6%88%96-blg%E7%9B%B4%E6%92%AD%E8%AE%B0%E5%BD%95)\n  - [/blg直播间sc 或 /BLG直播间SC](#blg%E7%9B%B4%E6%92%AD%E9%97%B4sc-%E6%88%96-blg%E7%9B%B4%E6%92%AD%E9%97%B4sc)\n  - [/icu查直播 或 /ICU查直播 或 /matsuri查直播](#icu%E6%9F%A5%E7%9B%B4%E6%92%AD-%E6%88%96-icu%E6%9F%A5%E7%9B%B4%E6%92%AD-%E6%88%96-matsuri%E6%9F%A5%E7%9B%B4%E6%92%AD)\n  - [/lap查用户 或 /LAP查用户](#lap%E6%9F%A5%E7%94%A8%E6%88%B7-%E6%88%96-lap%E6%9F%A5%E7%94%A8%E6%88%B7)\n  - [/lap查牌子 或 /LAP查牌子](#lap%E6%9F%A5%E7%89%8C%E5%AD%90-%E6%88%96-lap%E6%9F%A5%E7%89%8C%E5%AD%90)\n  - [/lap查充电 或 /LAP查充电](#lap%E6%9F%A5%E5%85%85%E7%94%B5-%E6%88%96-lap%E6%9F%A5%E5%85%85%E7%94%B5)\n  - [/lapdd 或 /LAPDD 或 /lapdd排行榜](#lapdd-%E6%88%96-lapdd-%E6%88%96-lapdd%E6%8E%92%E8%A1%8C%E6%A6%9C)\n  - [/zero查用户 或 /ZERO查用户](#zero%E6%9F%A5%E7%94%A8%E6%88%B7-%E6%88%96-zero%E6%9F%A5%E7%94%A8%E6%88%B7)\n  - [/zero被关注 或 /ZERO被关注](#zero%E8%A2%AB%E5%85%B3%E6%B3%A8-%E6%88%96-zero%E8%A2%AB%E5%85%B3%E6%B3%A8)\n  - [斗虫 或 主播pk 或 主播PK](#%E6%96%97%E8%99%AB-%E6%88%96-%E4%B8%BB%E6%92%ADpk-%E6%88%96-%E4%B8%BB%E6%92%ADpk)\n  - [eh查直播 或 诶嘿查直播 或 eihei查直播](#eh%E6%9F%A5%E7%9B%B4%E6%92%AD-%E6%88%96-%E8%AF%B6%E5%98%BF%E6%9F%A5%E7%9B%B4%E6%92%AD-%E6%88%96-eihei%E6%9F%A5%E7%9B%B4%E6%92%AD)\n  - [/vtb网站](#vtb%E7%BD%91%E7%AB%99)\n- [⚙ 拓展](#-%E6%8B%93%E5%B1%95)\n- [📝 更新日志](#-%E6%9B%B4%E6%96%B0%E6%97%A5%E5%BF%97)\n- [致谢](#%E8%87%B4%E8%B0%A2)\n- [项目打包上传至pypi](#%E9%A1%B9%E7%9B%AE%E6%89%93%E5%8C%85%E4%B8%8A%E4%BC%A0%E8%87%B3pypi)\n  - [poetry](#poetry)\n  - [twine](#twine)\n- [目录自动生成](#%E7%9B%AE%E5%BD%95%E8%87%AA%E5%8A%A8%E7%94%9F%E6%88%90)\n  - [安装](#%E5%AE%89%E8%A3%85)\n  - [使用](#%E4%BD%BF%E7%94%A8)\n\n<!-- END doctoc generated TOC please keep comment here to allow auto update -->\n\n## 🔧 开发环境\nNonebot2：2.0.0b5  \npython：3.8.13  \n操作系统：Windows10（CentOS7下正常运行，Linux兼容性问题不大）  \n编辑器：pycharm  \n\n## 💿 安装\n环境依赖`aiohttp`和`nonebot_plugin_htmlrender`库   \n部分功能需要获取自己的cookie，配置env后才能正常使用！  \n\n### 1. nb-cli安装（推荐）\n在你bot工程的文件夹下，运行cmd（运行路径要对啊），执行nb命令安装插件，插件配置会自动添加至配置文件  \n```\nnb plugin install nonebot_plugin_searchBiliInfo\n```\n\n### 2. 本地安装\n先安装下 `aiohttp` 和 `htmlrender`  \n```\npip install aiohttp\npip install nonebot_plugin_htmlrender\n```\n将项目clone到你的机器人插件下的对应插件目录内（一般为机器人文件夹下的`src/plugins`），然后把`nonebot_plugin_searchBiliInfo`文件夹里的内容拷贝至上一级目录即可。  \nclone命令参考（得先装`git`，懂的都懂）：\n```\ngit clone https://github.com/Ikaros-521/nonebot_plugin_searchBiliInfo.git\n``` \n也可以直接下载压缩包到插件目录解压，然后同样提取`nonebot_plugin_searchBiliInfo`至上一级目录。  \n目录结构： ```你的bot/src/plugins/nonebot_plugin_searchBiliInfo/__init__.py```  \n\n\n### 3. pip安装\n```\npip install nonebot_plugin_searchBiliInfo\n```  \n打开 nonebot2 项目的 ```bot.py``` 文件, 在其中写入  \n```nonebot.load_plugin(\'nonebot_plugin_searchBiliInfo\')```  \n当然，如果是默认nb-cli创建的nonebot2的话，在bot路径```pyproject.toml```的```[tool.nonebot]```的```plugins```中添加```nonebot_plugin_searchBiliInfo```即可  \npyproject.toml配置例如：  \n``` \n[tool.nonebot]\nplugin_dirs = ["src/plugins"]\nplugins = ["nonebot_plugin_searchBiliInfo"]\n``` \n\n### 更新版本\n```\nnb plugin update nonebot_plugin_searchBiliInfo\n```\n\n## 🔧 配置\n\n### cookie获取方式\n浏览器进入b站官网并登录: `https://www.bilibili.com/`  \nedge（或其他浏览器）按`f12`（或鼠标右键`“检查”` `“开发者工具”`等）, 然后点击右上角那个`">>"`符号, 进入`"网络"`  \n再按`ctrl+r`（或`f5`）刷新元素  \n随便点击一个请求, 在`“请求标头”`里面找到cookie（没有就换一个）  \ncookie冒号后面的就是cookie，复制一下, 可以把ta添加到env里  \n如果不想放太多cookie信息，只需要`buvid3`字段即可。  \n\n### env配置\n```\n# 在你的env文件中添加如下配置（我的是.env.prod） 仅需要buvid3字段即可\nsearchBiliInfo_cookie="buvid3=XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXXXXXXXinfoc;"\n```\n|       配置项        | 必填 | 默认值  |                      说明                      |\n|:----------------:|:----:|:----:|:----------------------------:|\n| `searchBiliInfo_cookie` | 否 | `""` | b站cookie，仅需要`buvid3`字段即可 |\n\n\n## 🎉 功能\n通过uid 或 设定好的短语 或 b站接口搜索查询指定b站用户的粉丝、舰团信息；直播收益数据；直播观看信息；关键词搜昵称、UID等信息；主播营收榜单。\n\n## 👉 命令(命令前缀自行替换喵~)\n\n### /查\n命令结构：```/查 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/查 uid:3709626``` 或 ```/查 :3709626``` 或 ```/查 bishi```  \nbot返回内容：  \n![](docs/search.png)\n\n### /查直播\n命令结构：```/查直播 (uid:或UID:或：或:)+用户uid或昵称关键词 场次数（默认不写为全部）```  \n例如：```/查直播 UID:3709626 1``` 或 ```/查直播 bishi```  \nbot返回内容（图片）：  \n![](docs/live_info.png)\n\n### /查舰团\n命令结构：```/查舰团 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/查舰团 ：3709626``` 或 ```/查舰团 bishi```  \nbot返回内容(图片)：  \n![](docs/guard.png)\n\n### /查昵称\n命令结构：```/查昵称 昵称关键词```  \n例如：```/查昵称 伊卡洛斯```\nbot返回内容(图片)：  \n![](docs/search_name.png)\n\n### /查收益\n命令结构：```/查收益 (uid:或UID:或：或:)+用户uid或昵称关键词 收益类型(默认1: 礼物，2: 上舰，3: SC) 倒叙第n场(从0开始)```  \n例如：```/查收益 :3709626 礼物 1``` 或 ```/查收益 bishi 2 0```  \nbot返回内容(图片)：  \n![](docs/income.png)\n\n### /查观看\n命令结构：```/查观看 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/查观看 UID:666666``` 或 ```/查观看 bishi```  \nbot返回内容(图片)：  \n![](docs/watch.png)\n\n### /查观看2\n命令结构：```/查观看2 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/查观看2 UID:666666``` 或 ```/查观看2 bishi```  \nbot返回内容(图片)：  \n![](docs/watch2.png)\n\n### /查弹幕\n命令结构：```/查弹幕 (uid:或UID:或：或:)+用户uid或昵称关键词 查询的主播昵称关键词或(uid:或UID:或：或:)+ 页数(可不填，默认0) 条数(可不填，默认3)```  \n例如：```/查弹幕 uid:3709626 Love丶伊卡洛斯 1 1``` 或 ```/查弹幕 uid:3709626 Love丶伊卡洛斯 1```   \nbot返回内容(图片)：  \n![](docs/danmu.png)\n\n### /查弹幕2\n命令结构：```/查弹幕2 (uid:或UID:或：或:)+用户uid或昵称关键词 页数(可不填，默认0) 条数(可不填，默认3)```  \n例如：```/查弹幕2 uid:3709626 2 2``` 或 ```/查弹幕2 uid:3709626 2```   \nbot返回内容(图片)：  \n![](docs/danmu2.png)\n\n### /查牌子\n命令结构：```/查牌子 主播牌子关键词```  \n例如：```/查牌子 天``` 或 ```/查牌子 天降```  \nbot返回内容(图片)：  \n![](docs/medal.png)\n\n### /查人气\n命令结构：```/查人气 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/查人气 uid:3709626``` 或 ```/查人气 Love丶伊卡洛斯```   \nbot返回内容(图片)：  \n![](docs/popularity.png)\n\n### /查装扮\n命令结构：```/查装扮 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/查装扮 uid:2``` 或 ```/查装扮 ：2```   \nbot返回内容(图片)：  \n![](docs/garb.png)\n\n### /营收\n命令结构：```/营收 日/周/月榜 人数（不填默认100）```  \n例如：```/营收 日榜 3``` 或 ```/营收 月榜```  \nbot返回内容(图片)：  \n![](docs/revenue.png)\n\n### /涨粉\n命令结构：```/涨粉 日/周/月榜 人数（不填默认100）```  \n例如：```/涨粉 日榜 3``` 或 ```/涨粉 月榜```  \nbot返回内容(图片)：  \n![](docs/incfans.png)\n\n### /DD风云榜 或 /dd风云榜 或 /风云榜 (寄了)\n命令结构：```/DD风云榜 top人数（不填默认10）```  \n例如：```/DD风云榜``` 或 ```/风云榜 20```  \nbot返回内容(图片)：  \n![](docs/ddstats.png)\n\n### /v详情 或 /V详情 或 /v详细 或 /V详细\n命令结构：```/v详情 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/v详情 uid:3709626``` 或 ```/V详情 ：2``` 或 ```/v详细 Love丶伊卡洛斯``` 或 ```/V详细 :2```    \nbot返回内容(图片)：  \n![](docs/v_detail.png)\n\n### /v直播势 或 /V直播势\n命令结构：```/v直播势```  \n例如：```/v直播势``` 或 ```/V直播势```  \nbot返回内容(图片)：  \n![](docs/v_live.png)\n\n### /v急上升 或 /V急上升\n命令结构：```/v急上升```  \n例如：```/v急上升``` 或 ```/V急上升```  \nbot返回内容(图片)：  \n![](docs/v_rise.png)\n\n### /v急下降 或 /V急下降\n命令结构：```/v急下降```  \n例如：```/v急下降``` 或 ```/V急下降```  \nbot返回内容(图片)：  \n![](docs/v_drop.png)\n\n### /v舰团 或 /V舰团\n命令结构：```/v舰团```  \n例如：```/v舰团``` 或 ```/V舰团```  \nbot返回内容(图片)：  \n![](docs/v_guard.png)\n\n### /vdd 或 /VDD 或 /VDD风云榜 或 /vdd风云榜\n命令结构：```/vdd```  \n例如：```/vdd``` 或 ```/VDD```  或 ```/vdd风云榜```   \nbot返回内容(图片)：  \n![](docs/v_dd.png)\n\n### /V宏观 或 /v宏观\n命令结构：```/vdd```  \n例如：```/V宏观``` 或 ```/v宏观```   \nbot返回内容(图片)：  \n![](docs/v_macro.png)\n\n### /dmk查用户 或 /DMK查用户\n命令结构：```/dmk查用户 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/dmk查用户 uid:3709626``` 或 ```/DMK查用户 Love丶伊卡洛斯```  \nbot返回内容(图片)：  \n![](docs/dmk_user.png)\n\n### /dmk查直播 或 /DMK查直播\n命令结构：```/dmk查直播 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/dmk查直播 uid:3709626``` 或 ```/DMK查直播 Love丶伊卡洛斯```  \nbot返回内容(图片)：  \n![](docs/dmk_live.png)\n\n### /blg查弹幕 或 /BLG查弹幕\n命令结构：```/blg查弹幕 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/blg查弹幕 uid:3709626``` 或 ```/BLG查弹幕 Love丶伊卡洛斯```  \nbot返回内容(图片)：  \n![](docs/blg_danmu.png)\n\n### /blg查入场 或 /BLG查入场\n命令结构：```/blg查入场 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/blg查入场 uid:3709626``` 或 ```/BLG查入场 Love丶伊卡洛斯```  \nbot返回内容(图片)：  \n![](docs/blg_enter.png)\n\n### /blg查礼物 或 /BLG查礼物\n命令结构：```/blg查礼物 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/blg查礼物 uid:3709626``` 或 ```/BLG查礼物 Love丶伊卡洛斯```  \nbot返回内容(图片)：  \n![](docs/blg_gift.png)\n\n### /blg直播记录 或 /BLG直播记录\n命令结构：```/blg直播记录 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/blg直播记录 uid:3709626``` 或 ```/BLG直播记录 Love丶伊卡洛斯```  \nbot返回内容(图片)：  \n![](docs/blg_tp.png)\n\n### /blg直播间sc 或 /BLG直播间SC\n命令结构：```/blg直播间sc (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/blg直播间sc uid:3709626``` 或 ```/BLG直播间SC Love丶伊卡洛斯```  \nbot返回内容(图片)：  \n![](docs/blg_sc.png)\n\n### /icu查直播 或 /ICU查直播 或 /matsuri查直播\n命令结构：```/icu查直播 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/icu查直播 uid:3709626``` 或 ```/ICU查直播 Love丶伊卡洛斯```  \nbot返回内容(图片)：  \n![](docs/icu_live.png)\n\n### /lap查用户 或 /LAP查用户\n命令结构：```/lap查用户 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/lap查用户 uid:387636363``` 或 ```/LAP查用户 雫るる```  \nbot返回内容(图片)：  \n![](docs/laplace_user.png)\n\n### /lap查牌子 或 /LAP查牌子\n命令结构：```/lap查牌子 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/lap查牌子 uid:387636363``` 或 ```/LAP查牌子 雫るる```  \nbot返回内容(图片)：  \n![](docs/laplace_medal.png)\n\n### /lap查充电 或 /LAP查充电\n命令结构：```/lap查充电 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/lap查充电 uid:387636363``` 或 ```/LAP查充电 雫るる```  \nbot返回内容(图片)：  \n![](docs/laplace_upower.png)\n\n### /lapdd 或 /LAPDD 或 /lapdd排行榜\n命令结构：```/lapdd 搜索类型(默认0: 月供，1: 总督，2: 提督，3：舰长)```  \n例如：```/lapdd``` 或 ```/lapdd 1``` 或 ```/LAPDD 舰长```  \nbot返回内容(图片)：  \n![](docs/laplace_dd.png)\n\n### /zero查用户 或 /ZERO查用户\n命令结构：```/zero查用户 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/zero查用户 uid:387636363``` 或 ```/ZERO查用户 雫るる```  \nbot返回内容(图片)：  \n![](docs/zeroroku_author.png)\n\n### /zero被关注 或 /ZERO被关注\n命令结构：```/zero被关注 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/zero被关注 uid:387636363``` 或 ```/ZERO被关注 雫るる```  \nbot返回内容(图片)：  \n![](docs/zeroroku_famous_fans.png)\n\n### 斗虫 或 主播pk 或 主播PK\n命令结构：`斗虫|主播pk|主播PK 用户1的uid或昵称关键词 用户2的uid或昵称关键词 用户n的uid或昵称关键词 #当天向过去偏移天(起始) 当天向过去偏移天数(结尾)`\n注意：`#`和后面的`日期偏移`可以默认不填，不填写的话默认是一个月前到今天的数据。另外，传入的用户必须大于等于2人以上。（`日期偏移`其实就是`数据区间`啦）\n例如：```斗虫 雫酱 neol``` 或 ```斗虫 雫酱 neol #5 0``` 或 ```主播pk 雫酱 雫 #15 0```    \nbot返回内容(图片)：  \n![](docs/stats_nailv_live_compare.png)\n\n\n### eh查直播 或 诶嘿查直播 或 eihei查直播\n命令结构：```/eh查直播 (uid:或UID:或：或:)+用户uid或昵称关键词```  \n例如：```/诶嘿查直播 uid:3493132603754688``` 或 ```/诶嘿查直播 罗亚Roya```  \nbot返回内容(图片)：  \n![](docs/eihei_livepic.png)\n\n### /vtb网站\n命令结构：```/vtb网站``` 或 ```/vtb资源```  \n例如：```/vtb网站``` 或 ```/vtb资源```  \nbot返回内容：  \n```\nVTB数据看板：https://ikaros-521.gitee.io/vtb_data_board/\nmatsuri：https://matsuri.icu/\ndanmakus：https://danmakus.com/\nvtbs.fun：http://www.vtbs.fun/\nbiligank：https://biligank.com/\n火龙榜：https://huolonglive.com/#/\nvtbs.moe：https://vtbs.moe/\nvup.loveava.top：https://vup.loveava.top/ranking\nddstats：https://ddstats.ericlamm.xyz/\nzeroroku：https://zeroroku.com/bilibili\nlaplace：https://laplace.live/\n```\n\n## ⚙ 拓展\n启用关键词搜索，需要在`.env.xx`中配置自己的`cookie`。\n\n命令修改：  \n昵称自定义，修改`data.py`，在文件头部追加你需要定义的用户的json串，注意json格式！！！  \n命令自定义，修改`__init__.py`，`catch_str = on_command`这部分的代码即可。  \n\nbot返回内容格式修改对应的msg、out_str变量的内容  \n\n## 📝 更新日志\n\n<details>\n<summary>展开/收起</summary>\n\n### 0.0.1\n\n- 插件初次发布\n\n### 0.1.0\n\n- 更新基于vtbs.moe的主播数据，添加关键词搜索功能\n\n### 1.0.0\n\n新增以下功能（其实是LX_Bot的相关命令融进来了）\n- /查 昵称关键词\n- /查直播 昵称关键词 场次数\n- /查舰团 昵称关键词\n- /查昵称 昵称关键词\n- /查收益 收益类型(默认1: 礼物，2: 上舰，3: SC) 用户uid或昵称关键词 倒叙第n场(从0开始)\n- /查成分 观看 昵称关键词\n- /查成分 弹幕 查询的目标人 查询的主播 页数 条数\n\n### 1.0.4\n\n优化针对uid解析方式\n\n### 1.0.5\n\n修改cookie配置从env获取，方便用户配置\n\n### 1.0.6\n\n修复 /查成分 弹幕 数据解析bug；\n优化整体代码实现；\n\n### 1.1.0\n新增功能\n- /营收 日/周/月榜 人数（不填默认100）\n\n### 1.2.0\n弃用requests库，改为aiohttp  \n\n### 1.2.1\n修复查命令aiohttp适配性bug  \n\n### 1.3.0\n修改 查成分 弹幕 和 查成分 观看 命令为 查弹幕 和 查观看。  \n优化命令解析实现。  \n修复查弹幕数据解析bug。  \n\n### 1.3.1\n新增 /查弹幕2 命令。  \n修复查弹幕数据解析bug。 \n图片UI优化。  \n\n### 1.3.2\n优化 /查弹幕2 命令，增加主播名。  \n\n### 1.3.3\n修复 /查观看 因为数据源有同一用户名不同uid的情况导致的越界bug。  \n\n### 1.3.4\n优化异常报错的处理。  \n优化UI设计和部分功能。  \n\n### 1.3.5\n新增`/查收益 xx 舰长`和`uid：`的匹配。（但是舰长仍然是所有上舰数据）    \n\n### 1.3.6\n优化API挂彩时候的异常捕获处理。  \n\n### 1.3.7\n插件补充元信息。 \n\n### 1.3.8\n新增`vtb网站` 或 `vtb资源` 命令（命令前缀自行添加） \n\n### 1.3.9\n补充2个VTB资源站点  \n\n### 1.3.10\n适配vtbs.fun的营收接口变动  \n\n### 1.4.0\n修改on_keyword为on_command，从而适配自定义的命令前缀  \n\n### 1.4.1\n修改danmakus.com到新域名danmakus.com，接口也同步替换了。  \n\n### 1.4.2\n新增markdown的特殊字符过滤和文本超长换行。  \nps：vtbs.fun挂了，`营收`功能暂时无法使用。\n\n### 1.4.3\nvtbs.fun活了，加了ssl，已兼容。  \n\n### 1.4.4\n新增命令 涨粉，接口源自vtbs.fun（和营收 基本一致）  \n\n### 1.4.5\n新增命令 DD风云榜，接口源自ddstats-api.ericlamm.xyz  \n\n### 1.4.6\n补充遗漏的插件元信息    \n\n### 1.4.7\n新增功能 查牌子，数据源自本地爬取（vtbs.moe中主播牌子信息，共4273条数据）   \n\n### 1.4.8\n补充插牌子遗漏的1条数据   \n\n### 1.4.9\n补充遗漏的 vtb网站 功能元信息   \n\n### 1.4.10\n新增功能`v详情` `dmk查用户` `dmk查直播`，直接采用浏览器页面截图形式返回结果。（流量消耗会多一些，酌情使用）     \n\n### 1.4.11\n延长`v详情` `dmk查用户` `dmk查直播`的请求超时至5min（服务器4M跑也超时，功能很吃紧）  \n\n### 1.4.12\n追加最新的vtbs.moe的主播信息，并同步更新了牌子信息。  \n缩短`v详情` `dmk查用户` `dmk查直播`的请求超时至2min（前面是对面服务器炸了）  \n\n### 1.4.13\n优化请求错误或无数据时的消息返回和日志打印。  \n\n### 1.5.0\n新增功能`blg查弹幕` `blg查入场` `blg查礼物` `blg直播记录` `blg直播间sc`，直接采用浏览器页面截图形式返回结果。（流量消耗会多一些，酌情使用）     \n\n### 1.5.1\n新增4000+的用户数据和牌子数据  \n\n### 1.5.2\n新增b站用户数据至10w  \n新增粉丝牌数据至4w+  \n\n### 1.5.3\n新增网站laplace.live  \n新增`icu查直播`命令，同样是playwright的直接加载  \n\n### 1.5.4\n新用户数据爬自b站直播间各大分区列表，比起直接uid爬全站更具有针对性，实际效果也很好。  \n新增b站用户数据至23w+  \n新增粉丝牌数据至6.7w+  \n\n### 1.5.5\n由于出现低配置设备内存不足导致的无法启动问题，已将本地数据`data.py`清空至一个demo配置。如有本地配置需要的可以去旧版获取。  \n\n### 1.5.6\n新增粉丝牌数据至8.6w+，爬了一周的直播页，正式收工。  \n\n### 1.5.7\n新增命令`查人气`，用于查询b站主播最近一场直播的人气峰值  \n\n### 1.5.8\n新增`lap查用户`命令，同样是playwright，并做了js内嵌  \n\n### 1.5.9\n优化`lap查用户`的内容加载样式，显示内容更加全面（也更卡，乐）  \n\n### 1.5.10\n增加耗时的网页截图查询反馈，优化异常处理，不让你的人生浪费在等待中  \n\n### 1.5.11\n新增`zero查用户`命令，同理  \n\n### 1.5.12\n修复文档描述错误（不影响功能，暂不发版）  \n文档新增目录    \n\n### 1.5.13\n新增`lap查牌子`命令，调用laplace.live的接口，全站太卡了，绷  \n\n### 1.5.14\n修复`lap查牌子`接口返回uid固定问题导致的显示错误  \n优化文档  \n\n### 1.5.15\n升级`查观看`功能，统计观看次数。  \n\n### 1.5.16\n新增`查观看2`命令（查观看plus版），统计观看次数，以饼图形式返回。  \n\n### 1.5.17\n优化网页截图相关功能的图片存储名，减少短时间多请求导致的数据覆盖问题  \n修复`查观看2`的提示语延迟问题  \n修订文档错误  \n\n### 1.5.18\n新增`lap查充电`命令，查询up的充电排行榜。  \n新增`zero被关注`命令，查询用户的被哪些知名up主关注。  \n升级`查观看2`的主题为夜间模式，增加高级感。  \n\n### 1.6.0\n对类似的GET请求做了优化，降低代码冗余。  \n\n### 1.6.1\n删除`lap查用户`的小作文  \n\n### 1.6.2\n1、新增以下命令：  \n- /v直播势  （大写也可以）\n- /v急上升  （大写也可以）\n- /v急下降  （大写也可以）\n- /v舰团  （大写也可以）\n- /vdd  （大写也可以）\n- /v宏观  （大写也可以）  \n2、优化异常处理\n\n### 1.6.3\n优化`v详情`的请求延时，帮助数据加载。  \n\n### 1.6.4\n新增`查装扮`命令。  \n优化文档排序。 \n\n### 1.6.5\n1.`v详情`增加别名`v详细`。  \n2.修复`查收益`的传参bug。  \n3.优化代码实现，增加提示互动。  \n\n### 1.6.6\n1.修复`查弹幕`和`查弹幕2`的bug（让GPT帮忙写，很好，bug写得不错）  \n\n### 1.6.7\n1.命令文本消息内容改艾特为回复。  \n2.新增命令`lapdd`或`lapdd排行榜`，截图laplace.live的dd页面。  \n3.优化说明文档。  \n\n### 1.6.8\n修复`lapdd`命令不传参的bug。  \n\n### 1.6.9\n新增正则匹配的`斗虫`玩法，具体看命令说明。  \n\n### 1.7.0\n修复htmlrender导入问题。  \n\n### 1.7.1\n新增命令`eh查直播`或`诶嘿查直播`。  \n\n### 1.7.2\n修改`eh查直播`的请求地址为http，服务器上跑证书不行，绷。  \n\n### 1.7.3\n修改`eh查直播`为playwright，难绷。  \n\n### 1.7.4\n修改`eh查直播`为直接请求，不过跳过了ssl。  \n\n### 1.7.5\nbug修复  \n\n### 1.7.6\n`查`命令，追加返回用户主页和直播间链接。    \n\n</details>\n\n## 致谢\n- [nonebot-plugin-htmlrender](https://github.com/kexue-z/nonebot-plugin-htmlrender) - 图片合成的好手\n- [danmakus.com](https://danmakus.com/) - b站主播、用户弹幕直播信息等来源（开放API接口很赞！）\n- [vtbs.moe](https://vtbs.moe) - VTB本地数据信息来源（还有数据提供，TQL）  \n- [laplace.live](https://laplace.live/) - 也是b站主播用户查询站点，部分数据也是源自danmakus，UI不错  \n\n## 项目打包上传至pypi\n\n官网：https://pypi.org，注册账号，在系统用户根目录下创建`.pypirc`，配置  \n``` \n[distutils] \nindex-servers=pypi \n \n[pypi] repository = https://upload.pypi.org/legacy/ \nusername = 用户名 \npassword = 密码\n```\n\n### poetry\n\n```\n# 参考 https://www.freesion.com/article/58051228882/\n\n# 1、安装poetry\npip install poetry\n\n# 2、初始化配置文件（根据提示填写）\npoetry init\n\n# 3、微调配置文件pyproject.toml\n\n# 4、运行 poetry install, 可生成 “poetry.lock” 文件（可跳过）\npoetry install\n\n# 5、编译，生成dist\npoetry build\n\n# 6、发布\npoetry publish\n\n```\n\n### twine\n\n```\n# 参考 https://www.cnblogs.com/danhuai/p/14915042.html\n#创建setup.py文件 填写相关信息\n\n# 1、可以先升级打包工具\npip install --upgrade setuptools wheel twine\n\n# 2、打包\npython setup.py sdist bdist_wheel\n\n# 3、可以先检查一下包\ntwine check dist/*\n\n# 4、上传包到pypi（需输入用户名、密码）\ntwine upload dist/*\n```\n\n## 目录自动生成\n\n[doctoc](https://github.com/thlorenz/doctoc),在本地git存储库中生成降价文件的目录。链接通过命令行标志兼容github或其他网站生成的锚。\n\n### 安装\n进入包含本地git项目的目录，键入: `npm install -g doctoc`  \n\n### 使用\n在`README.md`中，找个生成目录位置，写入如下代码，确认生成位置：\n```\n<!-- START doctoc -->\n<!-- END doctoc -->\n```\ncmd输入命令即可：`doctoc /path/to/file`  \n例如：`doctoc README.md`  \n\n',
-    'author': 'Ikaros',
-    'author_email': '327209194@qq.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/Ikaros-521/nonebot_plugin_searchBiliInfo',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+# nonebot_plugin_searchBiliInfo
+  
+_✨ NoneBot b站用户信息查询插件 ✨_
+  
+<a href="https://github.com/Ikaros-521/nonebot_plugin_searchBiliInfo/stargazers">
+    <img alt="GitHub stars" src="https://img.shields.io/github/stars/Ikaros-521/nonebot_plugin_searchBiliInfo?color=%09%2300BFFF&style=flat-square">
+</a>
+<a href="https://github.com/Ikaros-521/nonebot_plugin_searchBiliInfo/issues">
+    <img alt="GitHub issues" src="https://img.shields.io/github/issues/Ikaros-521/nonebot_plugin_searchBiliInfo?color=Emerald%20green&style=flat-square">
+</a>
+<a href="https://github.com/Ikaros-521/nonebot_plugin_searchBiliInfo/network">
+    <img alt="GitHub forks" src="https://img.shields.io/github/forks/Ikaros-521/nonebot_plugin_searchBiliInfo?color=%2300BFFF&style=flat-square">
+</a>
+<a href="./LICENSE">
+    <img src="https://img.shields.io/github/license/Ikaros-521/nonebot_plugin_searchBiliInfo.svg" alt="license">
+</a>
+<a href="https://pypi.python.org/pypi/nonebot_plugin_searchBiliInfo">
+    <img src="https://img.shields.io/pypi/v/nonebot_plugin_searchBiliInfo.svg" alt="pypi">
+</a>
+<a href="https://www.python.org">
+    <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
+</a>
+
+</div>
+
+适用于nonebot2 v11的b站用户信息查询插件【粉丝、舰团信息；直播收益数据；直播观看信息；关键词搜昵称、UID；主播营收榜单；查成分；查牌子等】  
+（ps：微调源码可以兼容其他版本）   
+调用的相关API源自b站官方接口、danmakus.com和vtbs.fun
+
+<!-- START doctoc generated TOC please keep comment here to allow auto update -->
+<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
+## 📖目录
+
+- [🔧 开发环境](#-%E5%BC%80%E5%8F%91%E7%8E%AF%E5%A2%83)
+- [💿 安装](#-%E5%AE%89%E8%A3%85)
+  - [1. nb-cli安装（推荐）](#1-nb-cli%E5%AE%89%E8%A3%85%E6%8E%A8%E8%8D%90)
+  - [2. 本地安装](#2-%E6%9C%AC%E5%9C%B0%E5%AE%89%E8%A3%85)
+  - [3. pip安装](#3-pip%E5%AE%89%E8%A3%85)
+  - [更新版本](#%E6%9B%B4%E6%96%B0%E7%89%88%E6%9C%AC)
+- [🔧 配置](#-%E9%85%8D%E7%BD%AE)
+  - [cookie获取方式](#cookie%E8%8E%B7%E5%8F%96%E6%96%B9%E5%BC%8F)
+  - [env配置](#env%E9%85%8D%E7%BD%AE)
+- [🎉 功能](#-%E5%8A%9F%E8%83%BD)
+- [👉 命令(命令前缀自行替换喵~)](#-%E5%91%BD%E4%BB%A4%E5%91%BD%E4%BB%A4%E5%89%8D%E7%BC%80%E8%87%AA%E8%A1%8C%E6%9B%BF%E6%8D%A2%E5%96%B5)
+  - [/查](#%E6%9F%A5)
+  - [/查直播](#%E6%9F%A5%E7%9B%B4%E6%92%AD)
+  - [/查舰团](#%E6%9F%A5%E8%88%B0%E5%9B%A2)
+  - [/查昵称](#%E6%9F%A5%E6%98%B5%E7%A7%B0)
+  - [/查收益](#%E6%9F%A5%E6%94%B6%E7%9B%8A)
+  - [/查观看](#%E6%9F%A5%E8%A7%82%E7%9C%8B)
+  - [/查观看2](#%E6%9F%A5%E8%A7%82%E7%9C%8B2)
+  - [/查弹幕](#%E6%9F%A5%E5%BC%B9%E5%B9%95)
+  - [/查弹幕2](#%E6%9F%A5%E5%BC%B9%E5%B9%952)
+  - [/查牌子](#%E6%9F%A5%E7%89%8C%E5%AD%90)
+  - [/查人气](#%E6%9F%A5%E4%BA%BA%E6%B0%94)
+  - [/查装扮](#%E6%9F%A5%E8%A3%85%E6%89%AE)
+  - [/营收](#%E8%90%A5%E6%94%B6)
+  - [/涨粉](#%E6%B6%A8%E7%B2%89)
+  - [/DD风云榜 或 /dd风云榜 或 /风云榜 (寄了)](#dd%E9%A3%8E%E4%BA%91%E6%A6%9C-%E6%88%96-dd%E9%A3%8E%E4%BA%91%E6%A6%9C-%E6%88%96-%E9%A3%8E%E4%BA%91%E6%A6%9C-%E5%AF%84%E4%BA%86)
+  - [/v详情 或 /V详情 或 /v详细 或 /V详细](#v%E8%AF%A6%E6%83%85-%E6%88%96-v%E8%AF%A6%E6%83%85-%E6%88%96-v%E8%AF%A6%E7%BB%86-%E6%88%96-v%E8%AF%A6%E7%BB%86)
+  - [/v直播势 或 /V直播势](#v%E7%9B%B4%E6%92%AD%E5%8A%BF-%E6%88%96-v%E7%9B%B4%E6%92%AD%E5%8A%BF)
+  - [/v急上升 或 /V急上升](#v%E6%80%A5%E4%B8%8A%E5%8D%87-%E6%88%96-v%E6%80%A5%E4%B8%8A%E5%8D%87)
+  - [/v急下降 或 /V急下降](#v%E6%80%A5%E4%B8%8B%E9%99%8D-%E6%88%96-v%E6%80%A5%E4%B8%8B%E9%99%8D)
+  - [/v舰团 或 /V舰团](#v%E8%88%B0%E5%9B%A2-%E6%88%96-v%E8%88%B0%E5%9B%A2)
+  - [/vdd 或 /VDD 或 /VDD风云榜 或 /vdd风云榜](#vdd-%E6%88%96-vdd-%E6%88%96-vdd%E9%A3%8E%E4%BA%91%E6%A6%9C-%E6%88%96-vdd%E9%A3%8E%E4%BA%91%E6%A6%9C)
+  - [/V宏观 或 /v宏观](#v%E5%AE%8F%E8%A7%82-%E6%88%96-v%E5%AE%8F%E8%A7%82)
+  - [/dmk查用户 或 /DMK查用户](#dmk%E6%9F%A5%E7%94%A8%E6%88%B7-%E6%88%96-dmk%E6%9F%A5%E7%94%A8%E6%88%B7)
+  - [/dmk查直播 或 /DMK查直播](#dmk%E6%9F%A5%E7%9B%B4%E6%92%AD-%E6%88%96-dmk%E6%9F%A5%E7%9B%B4%E6%92%AD)
+  - [/dmk分析 或 /DMK分析](#dmk%E5%88%86%E6%9E%90-%E6%88%96-dmk%E5%88%86%E6%9E%90)
+  - [/blg查弹幕 或 /BLG查弹幕](#blg%E6%9F%A5%E5%BC%B9%E5%B9%95-%E6%88%96-blg%E6%9F%A5%E5%BC%B9%E5%B9%95)
+  - [/blg查入场 或 /BLG查入场](#blg%E6%9F%A5%E5%85%A5%E5%9C%BA-%E6%88%96-blg%E6%9F%A5%E5%85%A5%E5%9C%BA)
+  - [/blg查礼物 或 /BLG查礼物](#blg%E6%9F%A5%E7%A4%BC%E7%89%A9-%E6%88%96-blg%E6%9F%A5%E7%A4%BC%E7%89%A9)
+  - [/blg直播记录 或 /BLG直播记录](#blg%E7%9B%B4%E6%92%AD%E8%AE%B0%E5%BD%95-%E6%88%96-blg%E7%9B%B4%E6%92%AD%E8%AE%B0%E5%BD%95)
+  - [/blg直播间sc 或 /BLG直播间SC](#blg%E7%9B%B4%E6%92%AD%E9%97%B4sc-%E6%88%96-blg%E7%9B%B4%E6%92%AD%E9%97%B4sc)
+  - [/icu查直播 或 /ICU查直播 或 /matsuri查直播](#icu%E6%9F%A5%E7%9B%B4%E6%92%AD-%E6%88%96-icu%E6%9F%A5%E7%9B%B4%E6%92%AD-%E6%88%96-matsuri%E6%9F%A5%E7%9B%B4%E6%92%AD)
+  - [/lap查用户 或 /LAP查用户](#lap%E6%9F%A5%E7%94%A8%E6%88%B7-%E6%88%96-lap%E6%9F%A5%E7%94%A8%E6%88%B7)
+  - [/lap查牌子 或 /LAP查牌子](#lap%E6%9F%A5%E7%89%8C%E5%AD%90-%E6%88%96-lap%E6%9F%A5%E7%89%8C%E5%AD%90)
+  - [/lap查充电 或 /LAP查充电](#lap%E6%9F%A5%E5%85%85%E7%94%B5-%E6%88%96-lap%E6%9F%A5%E5%85%85%E7%94%B5)
+  - [/lapdd 或 /LAPDD 或 /lapdd排行榜](#lapdd-%E6%88%96-lapdd-%E6%88%96-lapdd%E6%8E%92%E8%A1%8C%E6%A6%9C)
+  - [/zero查用户 或 /ZERO查用户](#zero%E6%9F%A5%E7%94%A8%E6%88%B7-%E6%88%96-zero%E6%9F%A5%E7%94%A8%E6%88%B7)
+  - [/zero被关注 或 /ZERO被关注](#zero%E8%A2%AB%E5%85%B3%E6%B3%A8-%E6%88%96-zero%E8%A2%AB%E5%85%B3%E6%B3%A8)
+  - [斗虫 或 主播pk 或 主播PK](#%E6%96%97%E8%99%AB-%E6%88%96-%E4%B8%BB%E6%92%ADpk-%E6%88%96-%E4%B8%BB%E6%92%ADpk)
+  - [eh查直播 或 诶嘿查直播 或 eihei查直播](#eh%E6%9F%A5%E7%9B%B4%E6%92%AD-%E6%88%96-%E8%AF%B6%E5%98%BF%E6%9F%A5%E7%9B%B4%E6%92%AD-%E6%88%96-eihei%E6%9F%A5%E7%9B%B4%E6%92%AD)
+  - [/vtb网站](#vtb%E7%BD%91%E7%AB%99)
+- [⚙ 拓展](#-%E6%8B%93%E5%B1%95)
+- [📝 更新日志](#-%E6%9B%B4%E6%96%B0%E6%97%A5%E5%BF%97)
+- [致谢](#%E8%87%B4%E8%B0%A2)
+- [项目打包上传至pypi](#%E9%A1%B9%E7%9B%AE%E6%89%93%E5%8C%85%E4%B8%8A%E4%BC%A0%E8%87%B3pypi)
+  - [poetry](#poetry)
+  - [twine](#twine)
+- [目录自动生成](#%E7%9B%AE%E5%BD%95%E8%87%AA%E5%8A%A8%E7%94%9F%E6%88%90)
+  - [安装](#%E5%AE%89%E8%A3%85)
+  - [使用](#%E4%BD%BF%E7%94%A8)
+
+<!-- END doctoc generated TOC please keep comment here to allow auto update -->
+
+## 🔧 开发环境
+Nonebot2：2.0.0b5  
+python：3.8.13  
+操作系统：Windows10（CentOS7下正常运行，Linux兼容性问题不大）  
+编辑器：pycharm  
+
+## 💿 安装
+环境依赖`aiohttp`和`nonebot_plugin_htmlrender`库   
+部分功能需要获取自己的cookie，配置env后才能正常使用！  
+
+### 1. nb-cli安装（推荐）
+在你bot工程的文件夹下，运行cmd（运行路径要对啊），执行nb命令安装插件，插件配置会自动添加至配置文件  
+```
+nb plugin install nonebot_plugin_searchBiliInfo
+```
+
+### 2. 本地安装
+先安装下 `aiohttp` 和 `htmlrender`  
+```
+pip install aiohttp
+pip install nonebot_plugin_htmlrender
+```
+将项目clone到你的机器人插件下的对应插件目录内（一般为机器人文件夹下的`src/plugins`），然后把`nonebot_plugin_searchBiliInfo`文件夹里的内容拷贝至上一级目录即可。  
+clone命令参考（得先装`git`，懂的都懂）：
+```
+git clone https://github.com/Ikaros-521/nonebot_plugin_searchBiliInfo.git
+``` 
+也可以直接下载压缩包到插件目录解压，然后同样提取`nonebot_plugin_searchBiliInfo`至上一级目录。  
+目录结构： ```你的bot/src/plugins/nonebot_plugin_searchBiliInfo/__init__.py```  
+
+
+### 3. pip安装
+```
+pip install nonebot_plugin_searchBiliInfo
+```  
+打开 nonebot2 项目的 ```bot.py``` 文件, 在其中写入  
+```nonebot.load_plugin('nonebot_plugin_searchBiliInfo')```  
+当然，如果是默认nb-cli创建的nonebot2的话，在bot路径```pyproject.toml```的```[tool.nonebot]```的```plugins```中添加```nonebot_plugin_searchBiliInfo```即可  
+pyproject.toml配置例如：  
+``` 
+[tool.nonebot]
+plugin_dirs = ["src/plugins"]
+plugins = ["nonebot_plugin_searchBiliInfo"]
+``` 
+
+### 更新版本
+```
+nb plugin update nonebot_plugin_searchBiliInfo
+```
+
+## 🔧 配置
+
+### cookie获取方式
+浏览器进入b站官网并登录: `https://www.bilibili.com/`  
+edge（或其他浏览器）按`f12`（或鼠标右键`“检查”` `“开发者工具”`等）, 然后点击右上角那个`">>"`符号, 进入`"网络"`  
+再按`ctrl+r`（或`f5`）刷新元素  
+随便点击一个请求, 在`“请求标头”`里面找到cookie（没有就换一个）  
+cookie冒号后面的就是cookie，复制一下, 可以把ta添加到env里  
+如果不想放太多cookie信息，只需要`buvid3`字段即可。  
+
+### env配置
+```
+# 在你的env文件中添加如下配置（我的是.env.prod） 仅需要buvid3字段即可
+searchBiliInfo_cookie="buvid3=XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXXXXXXXinfoc;"
+```
+|       配置项        | 必填 | 默认值  |                      说明                      |
+|:----------------:|:----:|:----:|:----------------------------:|
+| `searchBiliInfo_cookie` | 否 | `""` | b站cookie，仅需要`buvid3`字段即可 |
+
+
+## 🎉 功能
+通过uid 或 设定好的短语 或 b站接口搜索查询指定b站用户的粉丝、舰团信息；直播收益数据；直播观看信息；关键词搜昵称、UID等信息；主播营收榜单。
+
+## 👉 命令(命令前缀自行替换喵~)
+
+### /查
+命令结构：```/查 (uid:或UID:或：或:)+用户uid或昵称关键词```  
+例如：```/查 uid:3709626``` 或 ```/查 :3709626``` 或 ```/查 bishi```  
+bot返回内容：  
+![](docs/search.png)
+
+### /查直播
+命令结构：```/查直播 (uid:或UID:或：或:)+用户uid或昵称关键词 场次数（默认不写为全部）```  
+例如：```/查直播 UID:3709626 1``` 或 ```/查直播 bishi```  
+bot返回内容（图片）：  
+![](docs/live_info.png)
+
+### /查舰团
+命令结构：```/查舰团 (uid:或UID:或：或:)+用户uid或昵称关键词```  
+例如：```/查舰团 ：3709626``` 或 ```/查舰团 bishi```  
+bot返回内容(图片)：  
+![](docs/guard.png)
+
+### /查昵称
+命令结构：```/查昵称 昵称关键词```  
+例如：```/查昵称 伊卡洛斯```
+bot返回内容(图片)：  
+![](docs/search_name.png)
+
+### /查收益
+命令结构：```/查收益 (uid:或UID:或：或:)+用户uid或昵称关键词 收益类型(默认1: 礼物，2: 上舰，3: SC) 倒叙第n场(从0开始)```  
+例如：```/查收益 :3709626 礼物 1``` 或 ```/查收益 bishi 2 0```  
+bot返回内容(图片)：  
+![](docs/income.png)
+
+### /查观看
+命令结构：```/查观看 (uid:或UID:或：或:)+用户uid或昵称关键词```  
+例如：```/查观看 UID:666666``` 或 ```/查观看 bishi```  
+bot返回内容(图片)：  
+![](docs/watch.png)
+
+### /查观看2
+命令结构：```/查观看2 (uid:或UID:或：或:)+用户uid或昵称关键词```  
+例如：```/查观看2 UID:666666``` 或 ```/查观看2 bishi```  
+bot返回内容(图片)：  
+![](docs/watch2.png)
+
+### /查弹幕
+命令结构：```/查弹幕 (uid:或UID:或：或:)+用户uid或昵称关键词 查询的主播昵称关键词或(uid:或UID:或：或:)+ 页数(可不填，默认0) 条数(可不填，默认3)```  
+例如：```/查弹幕 uid:3709626 Love丶伊卡洛斯 1 1``` 或 ```/查弹幕 uid:3709626 Love丶伊卡洛斯 1```   
+bot返回内容(图片)：  
+![](docs/danmu.png)
+
+### /查弹幕2
+命令结构：```/查弹幕2 (uid:或UID:或：或:)+用户uid或昵称关键词 页数(可不填，默认0) 条数(可不填，默认3)```  
+例如：```/查弹幕2 uid:3709626 2 2``` 或 ```/查弹幕2 uid:3709626 2```   
+bot返回内容(图片)：  
+![](docs/danmu2.png)
+
+### /查牌子
+命令结构：```/查牌子 主播牌子关键词```  
+例如：```/查牌子 天``` 或 ```/查牌子 天降```  
+bot返回内容(图片)：  
+![](docs/medal.png)
+
+### /查人气
+命令结构：```/查人气 (uid:或UID:或：或:)+用户uid或昵称关键词```  
+例如：```/查人气 uid:3709626``` 或 ```/查人气 Love丶伊卡洛斯```   
+bot返回内容(图片)：  
+![](docs/popularity.png)
+
+### /查装扮
+命令结构：```/查装扮 (uid:或UID:或：或:)+用户uid或昵称关键词```  
+例如：```/查装扮 uid:2``` 或 ```/查装扮 ：2```   
+bot返回内容(图片)：  
+![](docs/garb.png)
+
+### /营收
+命令结构：```/营收 日/周/月榜 人数（不填默认100）```  
+例如：```/营收 日榜 3``` 或 ```/营收 月榜```  
+bot返回内容(图片)：  
+![](docs/revenue.png)
+
+### /涨粉
+命令结构：```/涨粉 日/周/月榜 人数（不填默认100）```  
+例如：```/涨粉 日榜 3``` 或 ```/涨粉 月榜```  
+bot返回内容(图片)：  
+![](docs/incfans.png)
+
+### /DD风云榜 或 /dd风云榜 或 /风云榜 (寄了)
+命令结构：```/DD风云榜 top人数（不填默认10）```  
+例如：```/DD风云榜``` 或 ```/风云榜 20```  
+bot返回内容(图片)：  
+![](docs/ddstats.png)
+
+### /v详情 或 /V详情 或 /v详细 或 /V详细
+命令结构：```/v详情 (uid:或UID:或：或:)+用户uid或昵称关键词```  
+例如：```/v详情 uid:3709626``` 或 ```/V详情 ：2``` 或 ```/v详细 Love丶伊卡洛斯``` 或 ```/V详细 :2```    
+bot返回内容(图片)：  
+![](docs/v_detail.png)
+
+### /v直播势 或 /V直播势
+命令结构：```/v直播势```  
+例如：```/v直播势``` 或 ```/V直播势```  
+bot返回内容(图片)：  
+![](docs/v_live.png)
+
+### /v急上升 或 /V急上升
+命令结构：```/v急上升```  
+例如：```/v急上升``` 或 ```/V急上升```  
+bot返回内容(图片)：  
+![](docs/v_rise.png)
+
+### /v急下降 或 /V急下降
+命令结构：```/v急下降```  
+例如：```/v急下降``` 或 ```/V急下降```  
+bot返回内容(图片)：  
+![](docs/v_drop.png)
+
+### /v舰团 或 /V舰团
+命令结构：```/v舰团```  
+例如：```/v舰团``` 或 ```/V舰团```  
+bot返回内容(图片)：  
+![](docs/v_guard.png)
+
+### /vdd 或 /VDD 或 /VDD风云榜 或 /vdd风云榜
+命令结构：```/vdd```  
+例如：```/vdd``` 或 ```/VDD```  或 ```/vdd风云榜```   
+bot返回内容(图片)：  
+![](docs/v_dd.png)
+
+### /V宏观 或 /v宏观
+命令结构：```/vdd```  
+例如：```/V宏观``` 或 ```/v宏观```   
+bot返回内容(图片)：  
+![](docs/v_macro.png)
+
+### /dmk查用户 或 /DMK查用户
+命令结构：```/dmk查用户 (uid:或UID:或：或:)+用户uid或昵称关键词```  
+例如：```/dmk查用户 uid:3709626``` 或 ```/DMK查用户 Love丶伊卡洛斯```  
+bot返回内容(图片)：  
+![](docs/dmk_user.png)
+
+### /dmk查直播 或 /DMK查直播
+命令结构：```/dmk查直播 (uid:或UID:或：或:)+用户uid或昵称关键词```  
+例如：```/dmk查直播 uid:3709626``` 或 ```/DMK查直播 Love丶伊卡洛斯```  
+bot返回内容(图片)：  
+![](docs/dmk_live.png)
+
+### /dmk分析 或 /DMK分析
+命令结构：```/dmk分析 (uid:或UID:或：或:)+用户uid或昵称关键词```  
+例如：```/dmk分析 uid:3709626``` 或 ```/DMK分析 Love丶伊卡洛斯```  
+bot返回内容(图片)：  
+![](docs/dmk_analyze.png)
+
+### /blg查弹幕 或 /BLG查弹幕
+命令结构：```/blg查弹幕 (uid:或UID:或：或:)+用户uid或昵称关键词```  
+例如：```/blg查弹幕 uid:3709626``` 或 ```/BLG查弹幕 Love丶伊卡洛斯```  
+bot返回内容(图片)：  
+![](docs/blg_danmu.png)
+
+### /blg查入场 或 /BLG查入场
+命令结构：```/blg查入场 (uid:或UID:或：或:)+用户uid或昵称关键词```  
+例如：```/blg查入场 uid:3709626``` 或 ```/BLG查入场 Love丶伊卡洛斯```  
+bot返回内容(图片)：  
+![](docs/blg_enter.png)
+
+### /blg查礼物 或 /BLG查礼物
+命令结构：```/blg查礼物 (uid:或UID:或：或:)+用户uid或昵称关键词```  
+例如：```/blg查礼物 uid:3709626``` 或 ```/BLG查礼物 Love丶伊卡洛斯```  
+bot返回内容(图片)：  
+![](docs/blg_gift.png)
+
+### /blg直播记录 或 /BLG直播记录
+命令结构：```/blg直播记录 (uid:或UID:或：或:)+用户uid或昵称关键词```  
+例如：```/blg直播记录 uid:3709626``` 或 ```/BLG直播记录 Love丶伊卡洛斯```  
+bot返回内容(图片)：  
+![](docs/blg_tp.png)
+
+### /blg直播间sc 或 /BLG直播间SC
+命令结构：```/blg直播间sc (uid:或UID:或：或:)+用户uid或昵称关键词```  
+例如：```/blg直播间sc uid:3709626``` 或 ```/BLG直播间SC Love丶伊卡洛斯```  
+bot返回内容(图片)：  
+![](docs/blg_sc.png)
+
+### /icu查直播 或 /ICU查直播 或 /matsuri查直播
+命令结构：```/icu查直播 (uid:或UID:或：或:)+用户uid或昵称关键词```  
+例如：```/icu查直播 uid:3709626``` 或 ```/ICU查直播 Love丶伊卡洛斯```  
+bot返回内容(图片)：  
+![](docs/icu_live.png)
+
+### /lap查用户 或 /LAP查用户
+命令结构：```/lap查用户 (uid:或UID:或：或:)+用户uid或昵称关键词```  
+例如：```/lap查用户 uid:387636363``` 或 ```/LAP查用户 雫るる```  
+bot返回内容(图片)：  
+![](docs/laplace_user.png)
+
+### /lap查牌子 或 /LAP查牌子
+命令结构：```/lap查牌子 (uid:或UID:或：或:)+用户uid或昵称关键词```  
+例如：```/lap查牌子 uid:387636363``` 或 ```/LAP查牌子 雫るる```  
+bot返回内容(图片)：  
+![](docs/laplace_medal.png)
+
+### /lap查充电 或 /LAP查充电
+命令结构：```/lap查充电 (uid:或UID:或：或:)+用户uid或昵称关键词```  
+例如：```/lap查充电 uid:387636363``` 或 ```/LAP查充电 雫るる```  
+bot返回内容(图片)：  
+![](docs/laplace_upower.png)
+
+### /lapdd 或 /LAPDD 或 /lapdd排行榜
+命令结构：```/lapdd 搜索类型(默认0: 月供，1: 总督，2: 提督，3：舰长)```  
+例如：```/lapdd``` 或 ```/lapdd 1``` 或 ```/LAPDD 舰长```  
+bot返回内容(图片)：  
+![](docs/laplace_dd.png)
+
+### /zero查用户 或 /ZERO查用户
+命令结构：```/zero查用户 (uid:或UID:或：或:)+用户uid或昵称关键词```  
+例如：```/zero查用户 uid:387636363``` 或 ```/ZERO查用户 雫るる```  
+bot返回内容(图片)：  
+![](docs/zeroroku_author.png)
+
+### /zero被关注 或 /ZERO被关注
+命令结构：```/zero被关注 (uid:或UID:或：或:)+用户uid或昵称关键词```  
+例如：```/zero被关注 uid:387636363``` 或 ```/ZERO被关注 雫るる```  
+bot返回内容(图片)：  
+![](docs/zeroroku_famous_fans.png)
+
+### 斗虫 或 主播pk 或 主播PK
+命令结构：`斗虫|主播pk|主播PK 用户1的uid或昵称关键词 用户2的uid或昵称关键词 用户n的uid或昵称关键词 #当天向过去偏移天(起始) 当天向过去偏移天数(结尾)`
+注意：`#`和后面的`日期偏移`可以默认不填，不填写的话默认是一个月前到今天的数据。另外，传入的用户必须大于等于2人以上。（`日期偏移`其实就是`数据区间`啦）
+例如：```斗虫 雫酱 neol``` 或 ```斗虫 雫酱 neol #5 0``` 或 ```主播pk 雫酱 雫 #15 0```    
+bot返回内容(图片)：  
+![](docs/stats_nailv_live_compare.png)
+
+
+### eh查直播 或 诶嘿查直播 或 eihei查直播
+命令结构：```/eh查直播 (uid:或UID:或：或:)+用户uid或昵称关键词```  
+例如：```/诶嘿查直播 uid:3493132603754688``` 或 ```/诶嘿查直播 罗亚Roya```  
+bot返回内容(图片)：  
+![](docs/eihei_livepic.png)
+
+### /vtb网站
+命令结构：```/vtb网站``` 或 ```/vtb资源```  
+例如：```/vtb网站``` 或 ```/vtb资源```  
+bot返回内容：  
+```
+VTB数据看板：https://ikaros-521.gitee.io/vtb_data_board/
+matsuri：https://matsuri.icu/
+danmakus：https://danmakus.com/
+vtbs.fun：http://www.vtbs.fun/
+biligank：https://biligank.com/
+火龙榜：https://huolonglive.com/#/
+vtbs.moe：https://vtbs.moe/
+vup.loveava.top：https://vup.loveava.top/ranking
+ddstats：https://ddstats.ericlamm.xyz/
+zeroroku：https://zeroroku.com/bilibili
+laplace：https://laplace.live/
+```
+
+## ⚙ 拓展
+启用关键词搜索，需要在`.env.xx`中配置自己的`cookie`。
+
+命令修改：  
+昵称自定义，修改`data.py`，在文件头部追加你需要定义的用户的json串，注意json格式！！！  
+命令自定义，修改`__init__.py`，`catch_str = on_command`这部分的代码即可。  
+
+bot返回内容格式修改对应的msg、out_str变量的内容  
+
+## 📝 更新日志
+
+<details>
+<summary>展开/收起</summary>
+
+### 0.0.1
+
+- 插件初次发布
+
+### 0.1.0
+
+- 更新基于vtbs.moe的主播数据，添加关键词搜索功能
+
+### 1.0.0
+
+新增以下功能（其实是LX_Bot的相关命令融进来了）
+- /查 昵称关键词
+- /查直播 昵称关键词 场次数
+- /查舰团 昵称关键词
+- /查昵称 昵称关键词
+- /查收益 收益类型(默认1: 礼物，2: 上舰，3: SC) 用户uid或昵称关键词 倒叙第n场(从0开始)
+- /查成分 观看 昵称关键词
+- /查成分 弹幕 查询的目标人 查询的主播 页数 条数
+
+### 1.0.4
+
+优化针对uid解析方式
+
+### 1.0.5
+
+修改cookie配置从env获取，方便用户配置
+
+### 1.0.6
+
+修复 /查成分 弹幕 数据解析bug；
+优化整体代码实现；
+
+### 1.1.0
+新增功能
+- /营收 日/周/月榜 人数（不填默认100）
+
+### 1.2.0
+弃用requests库，改为aiohttp  
+
+### 1.2.1
+修复查命令aiohttp适配性bug  
+
+### 1.3.0
+修改 查成分 弹幕 和 查成分 观看 命令为 查弹幕 和 查观看。  
+优化命令解析实现。  
+修复查弹幕数据解析bug。  
+
+### 1.3.1
+新增 /查弹幕2 命令。  
+修复查弹幕数据解析bug。 
+图片UI优化。  
+
+### 1.3.2
+优化 /查弹幕2 命令，增加主播名。  
+
+### 1.3.3
+修复 /查观看 因为数据源有同一用户名不同uid的情况导致的越界bug。  
+
+### 1.3.4
+优化异常报错的处理。  
+优化UI设计和部分功能。  
+
+### 1.3.5
+新增`/查收益 xx 舰长`和`uid：`的匹配。（但是舰长仍然是所有上舰数据）    
+
+### 1.3.6
+优化API挂彩时候的异常捕获处理。  
+
+### 1.3.7
+插件补充元信息。 
+
+### 1.3.8
+新增`vtb网站` 或 `vtb资源` 命令（命令前缀自行添加） 
+
+### 1.3.9
+补充2个VTB资源站点  
+
+### 1.3.10
+适配vtbs.fun的营收接口变动  
+
+### 1.4.0
+修改on_keyword为on_command，从而适配自定义的命令前缀  
+
+### 1.4.1
+修改danmakus.com到新域名danmakus.com，接口也同步替换了。  
+
+### 1.4.2
+新增markdown的特殊字符过滤和文本超长换行。  
+ps：vtbs.fun挂了，`营收`功能暂时无法使用。
+
+### 1.4.3
+vtbs.fun活了，加了ssl，已兼容。  
+
+### 1.4.4
+新增命令 涨粉，接口源自vtbs.fun（和营收 基本一致）  
+
+### 1.4.5
+新增命令 DD风云榜，接口源自ddstats-api.ericlamm.xyz  
+
+### 1.4.6
+补充遗漏的插件元信息    
+
+### 1.4.7
+新增功能 查牌子，数据源自本地爬取（vtbs.moe中主播牌子信息，共4273条数据）   
+
+### 1.4.8
+补充插牌子遗漏的1条数据   
+
+### 1.4.9
+补充遗漏的 vtb网站 功能元信息   
+
+### 1.4.10
+新增功能`v详情` `dmk查用户` `dmk查直播`，直接采用浏览器页面截图形式返回结果。（流量消耗会多一些，酌情使用）     
+
+### 1.4.11
+延长`v详情` `dmk查用户` `dmk查直播`的请求超时至5min（服务器4M跑也超时，功能很吃紧）  
+
+### 1.4.12
+追加最新的vtbs.moe的主播信息，并同步更新了牌子信息。  
+缩短`v详情` `dmk查用户` `dmk查直播`的请求超时至2min（前面是对面服务器炸了）  
+
+### 1.4.13
+优化请求错误或无数据时的消息返回和日志打印。  
+
+### 1.5.0
+新增功能`blg查弹幕` `blg查入场` `blg查礼物` `blg直播记录` `blg直播间sc`，直接采用浏览器页面截图形式返回结果。（流量消耗会多一些，酌情使用）     
+
+### 1.5.1
+新增4000+的用户数据和牌子数据  
+
+### 1.5.2
+新增b站用户数据至10w  
+新增粉丝牌数据至4w+  
+
+### 1.5.3
+新增网站laplace.live  
+新增`icu查直播`命令，同样是playwright的直接加载  
+
+### 1.5.4
+新用户数据爬自b站直播间各大分区列表，比起直接uid爬全站更具有针对性，实际效果也很好。  
+新增b站用户数据至23w+  
+新增粉丝牌数据至6.7w+  
+
+### 1.5.5
+由于出现低配置设备内存不足导致的无法启动问题，已将本地数据`data.py`清空至一个demo配置。如有本地配置需要的可以去旧版获取。  
+
+### 1.5.6
+新增粉丝牌数据至8.6w+，爬了一周的直播页，正式收工。  
+
+### 1.5.7
+新增命令`查人气`，用于查询b站主播最近一场直播的人气峰值  
+
+### 1.5.8
+新增`lap查用户`命令，同样是playwright，并做了js内嵌  
+
+### 1.5.9
+优化`lap查用户`的内容加载样式，显示内容更加全面（也更卡，乐）  
+
+### 1.5.10
+增加耗时的网页截图查询反馈，优化异常处理，不让你的人生浪费在等待中  
+
+### 1.5.11
+新增`zero查用户`命令，同理  
+
+### 1.5.12
+修复文档描述错误（不影响功能，暂不发版）  
+文档新增目录    
+
+### 1.5.13
+新增`lap查牌子`命令，调用laplace.live的接口，全站太卡了，绷  
+
+### 1.5.14
+修复`lap查牌子`接口返回uid固定问题导致的显示错误  
+优化文档  
+
+### 1.5.15
+升级`查观看`功能，统计观看次数。  
+
+### 1.5.16
+新增`查观看2`命令（查观看plus版），统计观看次数，以饼图形式返回。  
+
+### 1.5.17
+优化网页截图相关功能的图片存储名，减少短时间多请求导致的数据覆盖问题  
+修复`查观看2`的提示语延迟问题  
+修订文档错误  
+
+### 1.5.18
+新增`lap查充电`命令，查询up的充电排行榜。  
+新增`zero被关注`命令，查询用户的被哪些知名up主关注。  
+升级`查观看2`的主题为夜间模式，增加高级感。  
+
+### 1.6.0
+对类似的GET请求做了优化，降低代码冗余。  
+
+### 1.6.1
+删除`lap查用户`的小作文  
+
+### 1.6.2
+1、新增以下命令：  
+- /v直播势  （大写也可以）
+- /v急上升  （大写也可以）
+- /v急下降  （大写也可以）
+- /v舰团  （大写也可以）
+- /vdd  （大写也可以）
+- /v宏观  （大写也可以）  
+2、优化异常处理
+
+### 1.6.3
+优化`v详情`的请求延时，帮助数据加载。  
+
+### 1.6.4
+新增`查装扮`命令。  
+优化文档排序。 
+
+### 1.6.5
+1.`v详情`增加别名`v详细`。  
+2.修复`查收益`的传参bug。  
+3.优化代码实现，增加提示互动。  
+
+### 1.6.6
+1.修复`查弹幕`和`查弹幕2`的bug（让GPT帮忙写，很好，bug写得不错）  
+
+### 1.6.7
+1.命令文本消息内容改艾特为回复。  
+2.新增命令`lapdd`或`lapdd排行榜`，截图laplace.live的dd页面。  
+3.优化说明文档。  
+
+### 1.6.8
+修复`lapdd`命令不传参的bug。  
+
+### 1.6.9
+新增正则匹配的`斗虫`玩法，具体看命令说明。  
+
+### 1.7.0
+修复htmlrender导入问题。  
+
+### 1.7.1
+新增命令`eh查直播`或`诶嘿查直播`。  
+
+### 1.7.2
+修改`eh查直播`的请求地址为http，服务器上跑证书不行，绷。  
+
+### 1.7.3
+修改`eh查直播`为playwright，难绷。  
+
+### 1.7.4
+修改`eh查直播`为直接请求，不过跳过了ssl。  
+
+### 1.7.5
+bug修复  
+
+### 1.7.6
+`查`命令，追加返回用户主页和直播间链接。    
+
+### 1.7.7
+新增`dmk分析`功能，由danmakus分析用户观看弹幕等数据。  
+
+</details>
+
+## 致谢
+- [nonebot-plugin-htmlrender](https://github.com/kexue-z/nonebot-plugin-htmlrender) - 图片合成的好手
+- [danmakus.com](https://danmakus.com/) - b站主播、用户弹幕直播信息等来源（开放API接口很赞！）
+- [vtbs.moe](https://vtbs.moe) - VTB本地数据信息来源（还有数据提供，TQL）  
+- [laplace.live](https://laplace.live/) - 也是b站主播用户查询站点，部分数据也是源自danmakus，UI不错  
+
+## 项目打包上传至pypi
+
+官网：https://pypi.org，注册账号，在系统用户根目录下创建`.pypirc`，配置  
+``` 
+[distutils] 
+index-servers=pypi 
+ 
+[pypi] repository = https://upload.pypi.org/legacy/ 
+username = 用户名 
+password = 密码
+```
+
+### poetry
+
+```
+# 参考 https://www.freesion.com/article/58051228882/
+
+# 1、安装poetry
+pip install poetry
+
+# 2、初始化配置文件（根据提示填写）
+poetry init
+
+# 3、微调配置文件pyproject.toml
+
+# 4、运行 poetry install, 可生成 “poetry.lock” 文件（可跳过）
+poetry install
+
+# 5、编译，生成dist
+poetry build
+
+# 6、发布
+poetry publish
+
+```
+
+### twine
+
+```
+# 参考 https://www.cnblogs.com/danhuai/p/14915042.html
+#创建setup.py文件 填写相关信息
+
+# 1、可以先升级打包工具
+pip install --upgrade setuptools wheel twine
+
+# 2、打包
+python setup.py sdist bdist_wheel
+
+# 3、可以先检查一下包
+twine check dist/*
+
+# 4、上传包到pypi（需输入用户名、密码）
+twine upload dist/*
+```
+
+## 目录自动生成
+
+[doctoc](https://github.com/thlorenz/doctoc),在本地git存储库中生成降价文件的目录。链接通过命令行标志兼容github或其他网站生成的锚。
+
+### 安装
+进入包含本地git项目的目录，键入: `npm install -g doctoc`  
+
+### 使用
+在`README.md`中，找个生成目录位置，写入如下代码，确认生成位置：
+```
+<!-- START doctoc -->
+<!-- END doctoc -->
+```
+cmd输入命令即可：`doctoc /path/to/file`  
+例如：`doctoc README.md`  
 
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,427 +1,405 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['nonebot_plugin_searchbiliinfo'] package_data = \ {'': ['*'],
-'nonebot_plugin_searchbiliinfo': ['html/*']} install_requires = \
-['aiohttp>=3.8.3,<4.0.0', 'asyncio>=3.4.3,<4.0.0', 'nonebot-adapter-
-onebot>=2.1.3,<3.0.0', 'nonebot-plugin-htmlrender>=0.2.0.1,<0.3.0.0',
-'nonebot2>=2.0.0b5,<3.0.0'] setup_kwargs = { 'name': 'nonebot-plugin-
-searchbiliinfo', 'version': '1.7.6', 'description': 'A plugin for nonebot2.
-Query Bilibili user
-informationï¼ä¸ä¸ªNonebot2çæä»¶ï¼bç«ç¨æ·ä¿¡æ¯æ¥è¯¢æä»¶ãç²ä¸ãè°å¢ä¿¡æ¯ï¼ç´æ­æ¶çæ°æ®ï¼ç´æ­è§çä¿¡æ¯ï¼å³é®è¯ææµç§°ãUIDï¼ä¸»æ­è¥æ¶æ¦åï¼æ¥æåï¼æ¥çå­ç­ãï¼',
-'long_description': '
-                           \n [NoneBotPluginLogo]\n
-                                      \n
+Metadata-Version: 2.1 Name: nonebot-plugin-searchbiliinfo Version: 1.7.7
+Summary: A plugin for nonebot2. Query Bilibili user
+informationï¼ä¸ä¸ªNonebot2çæä»¶ï¼bç«ç¨æ·ä¿¡æ¯æ¥è¯¢æä»¶ãç²ä¸ãè°å¢ä¿¡æ¯ï¼ç´æ­æ¶çæ°æ®ï¼ç´æ­è§çä¿¡æ¯ï¼å³é®è¯ææµç§°ãUIDï¼ä¸»æ­è¥æ¶æ¦åï¼æ¥æåï¼æ¥çå­ç­ãï¼
+Home-page: https://github.com/Ikaros-521/nonebot_plugin_searchBiliInfo License:
+MIT Author: Ikaros Author-email: 327209194@qq.com Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiohttp (>=3.8.3,<4.0.0) Requires-Dist: asyncio (>=3.4.3,<4.0.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.1.3,<3.0.0) Requires-Dist: nonebot-
+plugin-htmlrender (>=0.2.0.1,<0.3.0.0) Requires-Dist: nonebot2
+(>=2.0.0b5,<3.0.0) Project-URL: Documentation, https://github.com/Ikaros-521/
+nonebot_plugin_searchBiliInfo/blob/master/README.md Project-URL: Repository,
+https://github.com/Ikaros-521/nonebot_plugin_searchBiliInfo Description-
+Content-Type: text/markdown
+                             [NoneBotPluginLogo]
                               [NoneBotPluginText]
-                                      \n
-\n\n
-             \n\n# nonebot_plugin_searchBiliInfo\n \n_â¨ NoneBot
-     bç«ç¨æ·ä¿¡æ¯æ¥è¯¢æä»¶ â¨_\n \n\n_[GitHub_stars]\n\n\n_[GitHub
-issues]\n\n\n_[GitHub_forks]\n\n\n_[license]\n\n\n_[pypi]\n\n\n_[python]\n\n\n
-\n\néç¨äºnonebot2
+# nonebot_plugin_searchBiliInfo _â¨ NoneBot bç«ç¨æ·ä¿¡æ¯æ¥è¯¢æä»¶ â¨_
+    [GitHub_stars] [GitHub_issues] [GitHub_forks] [license] [pypi] [python]
+éç¨äºnonebot2
 v11çbç«ç¨æ·ä¿¡æ¯æ¥è¯¢æä»¶ãç²ä¸ãè°å¢ä¿¡æ¯ï¼ç´æ­æ¶çæ°æ®ï¼ç´æ­è§çä¿¡æ¯ï¼å³é®è¯ææµç§°ãUIDï¼ä¸»æ­è¥æ¶æ¦åï¼æ¥æåï¼æ¥çå­ç­ã
-\nï¼psï¼å¾®è°æºç å¯ä»¥å¼å®¹å¶ä»çæ¬ï¼
-\nè°ç¨çç¸å³APIæºèªbç«å®æ¹æ¥å£ãdanmakus.comåvtbs.fun\n\n\n\n##
-ðç®å½\n\n- [ð§ å¼åç¯å¢](#-%E5%BC%80%E5%8F%91%E7%8E%AF%E5%A2%83)\n-
-[ð¿ å®è£](#-%E5%AE%89%E8%A3%85)\n - [1. nb-cliå®è£ï¼æ¨èï¼](#1-nb-
-cli%E5%AE%89%E8%A3%85%E6%8E%A8%E8%8D%90)\n - [2. æ¬å°å®è£](#2-
-%E6%9C%AC%E5%9C%B0%E5%AE%89%E8%A3%85)\n - [3. pipå®è£](#3-
-pip%E5%AE%89%E8%A3%85)\n - [æ´æ°çæ¬]
-(#%E6%9B%B4%E6%96%B0%E7%89%88%E6%9C%AC)\n- [ð§ éç½®](#-
-%E9%85%8D%E7%BD%AE)\n - [cookieè·åæ¹å¼]
-(#cookie%E8%8E%B7%E5%8F%96%E6%96%B9%E5%BC%8F)\n - [envéç½®]
-(#env%E9%85%8D%E7%BD%AE)\n- [ð åè½](#-%E5%8A%9F%E8%83%BD)\n- [ð å½ä»¤
+ï¼psï¼å¾®è°æºç å¯ä»¥å¼å®¹å¶ä»çæ¬ï¼
+è°ç¨çç¸å³APIæºèªbç«å®æ¹æ¥å£ãdanmakus.comåvtbs.fun   ##
+ðç®å½ - [ð§ å¼åç¯å¢](#-%E5%BC%80%E5%8F%91%E7%8E%AF%E5%A2%83) -
+[ð¿ å®è£](#-%E5%AE%89%E8%A3%85) - [1. nb-cliå®è£ï¼æ¨èï¼](#1-nb-
+cli%E5%AE%89%E8%A3%85%E6%8E%A8%E8%8D%90) - [2. æ¬å°å®è£](#2-
+%E6%9C%AC%E5%9C%B0%E5%AE%89%E8%A3%85) - [3. pipå®è£](#3-
+pip%E5%AE%89%E8%A3%85) - [æ´æ°çæ¬](#%E6%9B%B4%E6%96%B0%E7%89%88%E6%9C%AC)
+- [ð§ éç½®](#-%E9%85%8D%E7%BD%AE) - [cookieè·åæ¹å¼]
+(#cookie%E8%8E%B7%E5%8F%96%E6%96%B9%E5%BC%8F) - [envéç½®]
+(#env%E9%85%8D%E7%BD%AE) - [ð åè½](#-%E5%8A%9F%E8%83%BD) - [ð å½ä»¤
 (å½ä»¤åç¼èªè¡æ¿æ¢åµ~)](#-
-%E5%91%BD%E4%BB%A4%E5%91%BD%E4%BB%A4%E5%89%8D%E7%BC%80%E8%87%AA%E8%A1%8C%E6%9B%BF%E6%8D%A2%E5%96%B5)\n
-- [/æ¥](#%E6%9F%A5)\n - [/æ¥ç´æ­](#%E6%9F%A5%E7%9B%B4%E6%92%AD)\n - [/
-æ¥è°å¢](#%E6%9F%A5%E8%88%B0%E5%9B%A2)\n - [/æ¥æµç§°]
-(#%E6%9F%A5%E6%98%B5%E7%A7%B0)\n - [/æ¥æ¶ç](#%E6%9F%A5%E6%94%B6%E7%9B%8A)\n
-- [/æ¥è§ç](#%E6%9F%A5%E8%A7%82%E7%9C%8B)\n - [/æ¥è§ç2]
-(#%E6%9F%A5%E8%A7%82%E7%9C%8B2)\n - [/æ¥å¼¹å¹]
-(#%E6%9F%A5%E5%BC%B9%E5%B9%95)\n - [/æ¥å¼¹å¹2]
-(#%E6%9F%A5%E5%BC%B9%E5%B9%952)\n - [/æ¥çå­]
-(#%E6%9F%A5%E7%89%8C%E5%AD%90)\n - [/æ¥äººæ°](#%E6%9F%A5%E4%BA%BA%E6%B0%94)\n
-- [/æ¥è£æ®](#%E6%9F%A5%E8%A3%85%E6%89%AE)\n - [/è¥æ¶]
-(#%E8%90%A5%E6%94%B6)\n - [/æ¶¨ç²](#%E6%B6%A8%E7%B2%89)\n - [/DDé£äºæ¦ æ
-/ddé£äºæ¦ æ /é£äºæ¦ (å¯äº)](#dd%E9%A3%8E%E4%BA%91%E6%A6%9C-%E6%88%96-
+%E5%91%BD%E4%BB%A4%E5%91%BD%E4%BB%A4%E5%89%8D%E7%BC%80%E8%87%AA%E8%A1%8C%E6%9B%BF%E6%8D%A2%E5%96%B5)
+- [/æ¥](#%E6%9F%A5) - [/æ¥ç´æ­](#%E6%9F%A5%E7%9B%B4%E6%92%AD) - [/
+æ¥è°å¢](#%E6%9F%A5%E8%88%B0%E5%9B%A2) - [/æ¥æµç§°]
+(#%E6%9F%A5%E6%98%B5%E7%A7%B0) - [/æ¥æ¶ç](#%E6%9F%A5%E6%94%B6%E7%9B%8A) -
+[/æ¥è§ç](#%E6%9F%A5%E8%A7%82%E7%9C%8B) - [/æ¥è§ç2]
+(#%E6%9F%A5%E8%A7%82%E7%9C%8B2) - [/æ¥å¼¹å¹](#%E6%9F%A5%E5%BC%B9%E5%B9%95) -
+[/æ¥å¼¹å¹2](#%E6%9F%A5%E5%BC%B9%E5%B9%952) - [/æ¥çå­]
+(#%E6%9F%A5%E7%89%8C%E5%AD%90) - [/æ¥äººæ°](#%E6%9F%A5%E4%BA%BA%E6%B0%94) -
+[/æ¥è£æ®](#%E6%9F%A5%E8%A3%85%E6%89%AE) - [/è¥æ¶](#%E8%90%A5%E6%94%B6) -
+[/æ¶¨ç²](#%E6%B6%A8%E7%B2%89) - [/DDé£äºæ¦ æ /ddé£äºæ¦ æ /é£äºæ¦
+(å¯äº)](#dd%E9%A3%8E%E4%BA%91%E6%A6%9C-%E6%88%96-
 dd%E9%A3%8E%E4%BA%91%E6%A6%9C-%E6%88%96-%E9%A3%8E%E4%BA%91%E6%A6%9C-
-%E5%AF%84%E4%BA%86)\n - [/vè¯¦æ æ /Vè¯¦æ æ /vè¯¦ç» æ /Vè¯¦ç»]
+%E5%AF%84%E4%BA%86) - [/vè¯¦æ æ /Vè¯¦æ æ /vè¯¦ç» æ /Vè¯¦ç»]
 (#v%E8%AF%A6%E6%83%85-%E6%88%96-v%E8%AF%A6%E6%83%85-%E6%88%96-
-v%E8%AF%A6%E7%BB%86-%E6%88%96-v%E8%AF%A6%E7%BB%86)\n - [/vç´æ­å¿ æ /
+v%E8%AF%A6%E7%BB%86-%E6%88%96-v%E8%AF%A6%E7%BB%86) - [/vç´æ­å¿ æ /
 Vç´æ­å¿](#v%E7%9B%B4%E6%92%AD%E5%8A%BF-%E6%88%96-
-v%E7%9B%B4%E6%92%AD%E5%8A%BF)\n - [/væ¥ä¸å æ /Væ¥ä¸å]
-(#v%E6%80%A5%E4%B8%8A%E5%8D%87-%E6%88%96-v%E6%80%A5%E4%B8%8A%E5%8D%87)\n - [/
+v%E7%9B%B4%E6%92%AD%E5%8A%BF) - [/væ¥ä¸å æ /Væ¥ä¸å]
+(#v%E6%80%A5%E4%B8%8A%E5%8D%87-%E6%88%96-v%E6%80%A5%E4%B8%8A%E5%8D%87) - [/
 væ¥ä¸é æ /Væ¥ä¸é](#v%E6%80%A5%E4%B8%8B%E9%99%8D-%E6%88%96-
-v%E6%80%A5%E4%B8%8B%E9%99%8D)\n - [/vè°å¢ æ /Vè°å¢](#v%E8%88%B0%E5%9B%A2-
-%E6%88%96-v%E8%88%B0%E5%9B%A2)\n - [/vdd æ /VDD æ /VDDé£äºæ¦ æ /
+v%E6%80%A5%E4%B8%8B%E9%99%8D) - [/vè°å¢ æ /Vè°å¢](#v%E8%88%B0%E5%9B%A2-
+%E6%88%96-v%E8%88%B0%E5%9B%A2) - [/vdd æ /VDD æ /VDDé£äºæ¦ æ /
 vddé£äºæ¦](#vdd-%E6%88%96-vdd-%E6%88%96-vdd%E9%A3%8E%E4%BA%91%E6%A6%9C-
-%E6%88%96-vdd%E9%A3%8E%E4%BA%91%E6%A6%9C)\n - [/Vå®è§ æ /vå®è§]
-(#v%E5%AE%8F%E8%A7%82-%E6%88%96-v%E5%AE%8F%E8%A7%82)\n - [/dmkæ¥ç¨æ· æ /
+%E6%88%96-vdd%E9%A3%8E%E4%BA%91%E6%A6%9C) - [/Vå®è§ æ /vå®è§]
+(#v%E5%AE%8F%E8%A7%82-%E6%88%96-v%E5%AE%8F%E8%A7%82) - [/dmkæ¥ç¨æ· æ /
 DMKæ¥ç¨æ·](#dmk%E6%9F%A5%E7%94%A8%E6%88%B7-%E6%88%96-
-dmk%E6%9F%A5%E7%94%A8%E6%88%B7)\n - [/dmkæ¥ç´æ­ æ /DMKæ¥ç´æ­]
-(#dmk%E6%9F%A5%E7%9B%B4%E6%92%AD-%E6%88%96-dmk%E6%9F%A5%E7%9B%B4%E6%92%AD)\n -
-[/blgæ¥å¼¹å¹ æ /BLGæ¥å¼¹å¹](#blg%E6%9F%A5%E5%BC%B9%E5%B9%95-%E6%88%96-
-blg%E6%9F%A5%E5%BC%B9%E5%B9%95)\n - [/blgæ¥å¥åº æ /BLGæ¥å¥åº]
-(#blg%E6%9F%A5%E5%85%A5%E5%9C%BA-%E6%88%96-blg%E6%9F%A5%E5%85%A5%E5%9C%BA)\n -
-[/blgæ¥ç¤¼ç© æ /BLGæ¥ç¤¼ç©](#blg%E6%9F%A5%E7%A4%BC%E7%89%A9-%E6%88%96-
-blg%E6%9F%A5%E7%A4%BC%E7%89%A9)\n - [/blgç´æ­è®°å½ æ /BLGç´æ­è®°å½]
-(#blg%E7%9B%B4%E6%92%AD%E8%AE%B0%E5%BD%95-%E6%88%96-
-blg%E7%9B%B4%E6%92%AD%E8%AE%B0%E5%BD%95)\n - [/blgç´æ­é´sc æ /
+dmk%E6%9F%A5%E7%94%A8%E6%88%B7) - [/dmkæ¥ç´æ­ æ /DMKæ¥ç´æ­]
+(#dmk%E6%9F%A5%E7%9B%B4%E6%92%AD-%E6%88%96-dmk%E6%9F%A5%E7%9B%B4%E6%92%AD) - [/
+dmkåæ æ /DMKåæ](#dmk%E5%88%86%E6%9E%90-%E6%88%96-
+dmk%E5%88%86%E6%9E%90) - [/blgæ¥å¼¹å¹ æ /BLGæ¥å¼¹å¹]
+(#blg%E6%9F%A5%E5%BC%B9%E5%B9%95-%E6%88%96-blg%E6%9F%A5%E5%BC%B9%E5%B9%95) - [/
+blgæ¥å¥åº æ /BLGæ¥å¥åº](#blg%E6%9F%A5%E5%85%A5%E5%9C%BA-%E6%88%96-
+blg%E6%9F%A5%E5%85%A5%E5%9C%BA) - [/blgæ¥ç¤¼ç© æ /BLGæ¥ç¤¼ç©]
+(#blg%E6%9F%A5%E7%A4%BC%E7%89%A9-%E6%88%96-blg%E6%9F%A5%E7%A4%BC%E7%89%A9) - [/
+blgç´æ­è®°å½ æ /BLGç´æ­è®°å½](#blg%E7%9B%B4%E6%92%AD%E8%AE%B0%E5%BD%95-
+%E6%88%96-blg%E7%9B%B4%E6%92%AD%E8%AE%B0%E5%BD%95) - [/blgç´æ­é´sc æ /
 BLGç´æ­é´SC](#blg%E7%9B%B4%E6%92%AD%E9%97%B4sc-%E6%88%96-
-blg%E7%9B%B4%E6%92%AD%E9%97%B4sc)\n - [/icuæ¥ç´æ­ æ /ICUæ¥ç´æ­ æ /
+blg%E7%9B%B4%E6%92%AD%E9%97%B4sc) - [/icuæ¥ç´æ­ æ /ICUæ¥ç´æ­ æ /
 matsuriæ¥ç´æ­](#icu%E6%9F%A5%E7%9B%B4%E6%92%AD-%E6%88%96-
-icu%E6%9F%A5%E7%9B%B4%E6%92%AD-%E6%88%96-matsuri%E6%9F%A5%E7%9B%B4%E6%92%AD)\n
-- [/lapæ¥ç¨æ· æ /LAPæ¥ç¨æ·](#lap%E6%9F%A5%E7%94%A8%E6%88%B7-%E6%88%96-
-lap%E6%9F%A5%E7%94%A8%E6%88%B7)\n - [/lapæ¥çå­ æ /LAPæ¥çå­]
-(#lap%E6%9F%A5%E7%89%8C%E5%AD%90-%E6%88%96-lap%E6%9F%A5%E7%89%8C%E5%AD%90)\n -
-[/lapæ¥åçµ æ /LAPæ¥åçµ](#lap%E6%9F%A5%E5%85%85%E7%94%B5-%E6%88%96-
-lap%E6%9F%A5%E5%85%85%E7%94%B5)\n - [/lapdd æ /LAPDD æ /lapddæè¡æ¦]
-(#lapdd-%E6%88%96-lapdd-%E6%88%96-lapdd%E6%8E%92%E8%A1%8C%E6%A6%9C)\n - [/
+icu%E6%9F%A5%E7%9B%B4%E6%92%AD-%E6%88%96-matsuri%E6%9F%A5%E7%9B%B4%E6%92%AD) -
+[/lapæ¥ç¨æ· æ /LAPæ¥ç¨æ·](#lap%E6%9F%A5%E7%94%A8%E6%88%B7-%E6%88%96-
+lap%E6%9F%A5%E7%94%A8%E6%88%B7) - [/lapæ¥çå­ æ /LAPæ¥çå­]
+(#lap%E6%9F%A5%E7%89%8C%E5%AD%90-%E6%88%96-lap%E6%9F%A5%E7%89%8C%E5%AD%90) - [/
+lapæ¥åçµ æ /LAPæ¥åçµ](#lap%E6%9F%A5%E5%85%85%E7%94%B5-%E6%88%96-
+lap%E6%9F%A5%E5%85%85%E7%94%B5) - [/lapdd æ /LAPDD æ /lapddæè¡æ¦]
+(#lapdd-%E6%88%96-lapdd-%E6%88%96-lapdd%E6%8E%92%E8%A1%8C%E6%A6%9C) - [/
 zeroæ¥ç¨æ· æ /ZEROæ¥ç¨æ·](#zero%E6%9F%A5%E7%94%A8%E6%88%B7-%E6%88%96-
-zero%E6%9F%A5%E7%94%A8%E6%88%B7)\n - [/zeroè¢«å³æ³¨ æ /ZEROè¢«å³æ³¨]
-(#zero%E8%A2%AB%E5%85%B3%E6%B3%A8-%E6%88%96-zero%E8%A2%AB%E5%85%B3%E6%B3%A8)\n
-- [æè« æ ä¸»æ­pk æ ä¸»æ­PK](#%E6%96%97%E8%99%AB-%E6%88%96-
-%E4%B8%BB%E6%92%ADpk-%E6%88%96-%E4%B8%BB%E6%92%ADpk)\n - [ehæ¥ç´æ­ æ
+zero%E6%9F%A5%E7%94%A8%E6%88%B7) - [/zeroè¢«å³æ³¨ æ /ZEROè¢«å³æ³¨]
+(#zero%E8%A2%AB%E5%85%B3%E6%B3%A8-%E6%88%96-zero%E8%A2%AB%E5%85%B3%E6%B3%A8) -
+[æè« æ ä¸»æ­pk æ ä¸»æ­PK](#%E6%96%97%E8%99%AB-%E6%88%96-
+%E4%B8%BB%E6%92%ADpk-%E6%88%96-%E4%B8%BB%E6%92%ADpk) - [ehæ¥ç´æ­ æ
 è¯¶å¿æ¥ç´æ­ æ eiheiæ¥ç´æ­](#eh%E6%9F%A5%E7%9B%B4%E6%92%AD-%E6%88%96-
 %E8%AF%B6%E5%98%BF%E6%9F%A5%E7%9B%B4%E6%92%AD-%E6%88%96-
-eihei%E6%9F%A5%E7%9B%B4%E6%92%AD)\n - [/vtbç½ç«](#vtb%E7%BD%91%E7%AB%99)\n-
-[â æå±](#-%E6%8B%93%E5%B1%95)\n- [ð æ´æ°æ¥å¿](#-
-%E6%9B%B4%E6%96%B0%E6%97%A5%E5%BF%97)\n- [è´è°¢](#%E8%87%B4%E8%B0%A2)\n-
+eihei%E6%9F%A5%E7%9B%B4%E6%92%AD) - [/vtbç½ç«](#vtb%E7%BD%91%E7%AB%99) - [â
+æå±](#-%E6%8B%93%E5%B1%95) - [ð æ´æ°æ¥å¿](#-
+%E6%9B%B4%E6%96%B0%E6%97%A5%E5%BF%97) - [è´è°¢](#%E8%87%B4%E8%B0%A2) -
 [é¡¹ç®æåä¸ä¼ è³pypi]
-(#%E9%A1%B9%E7%9B%AE%E6%89%93%E5%8C%85%E4%B8%8A%E4%BC%A0%E8%87%B3pypi)\n -
-[poetry](#poetry)\n - [twine](#twine)\n- [ç®å½èªå¨çæ]
-(#%E7%9B%AE%E5%BD%95%E8%87%AA%E5%8A%A8%E7%94%9F%E6%88%90)\n - [å®è£]
-(#%E5%AE%89%E8%A3%85)\n - [ä½¿ç¨](#%E4%BD%BF%E7%94%A8)\n\n\n\n## ð§
-å¼åç¯å¢\nNonebot2ï¼2.0.0b5 \npythonï¼3.8.13
-\næä½ç³»ç»ï¼Windows10ï¼CentOS7ä¸æ­£å¸¸è¿è¡ï¼Linuxå¼å®¹æ§é®é¢ä¸å¤§ï¼
-\nç¼è¾å¨ï¼pycharm \n\n## ð¿
-å®è£\nç¯å¢ä¾èµ`aiohttp`å`nonebot_plugin_htmlrender`åº
-\né¨ååè½éè¦è·åèªå·±çcookieï¼éç½®envåæè½æ­£å¸¸ä½¿ç¨ï¼
-\n\n### 1. nb-
-cliå®è£ï¼æ¨èï¼\nå¨ä½ botå·¥ç¨çæä»¶å¤¹ä¸ï¼è¿è¡cmdï¼è¿è¡è·¯å¾è¦å¯¹åï¼ï¼æ§è¡nbå½ä»¤å®è£æä»¶ï¼æä»¶éç½®ä¼èªå¨æ·»å è³éç½®æä»¶
-\n```\nnb plugin install nonebot_plugin_searchBiliInfo\n```\n\n### 2.
-æ¬å°å®è£\nåå®è£ä¸ `aiohttp` å `htmlrender` \n```\npip install
-aiohttp\npip install
-nonebot_plugin_htmlrender\n```\nå°é¡¹ç®cloneå°ä½ çæºå¨äººæä»¶ä¸çå¯¹åºæä»¶ç®å½åï¼ä¸è¬ä¸ºæºå¨äººæä»¶å¤¹ä¸ç`src/
+(#%E9%A1%B9%E7%9B%AE%E6%89%93%E5%8C%85%E4%B8%8A%E4%BC%A0%E8%87%B3pypi) -
+[poetry](#poetry) - [twine](#twine) - [ç®å½èªå¨çæ]
+(#%E7%9B%AE%E5%BD%95%E8%87%AA%E5%8A%A8%E7%94%9F%E6%88%90) - [å®è£]
+(#%E5%AE%89%E8%A3%85) - [ä½¿ç¨](#%E4%BD%BF%E7%94%A8)  ## ð§ å¼åç¯å¢
+Nonebot2ï¼2.0.0b5 pythonï¼3.8.13
+æä½ç³»ç»ï¼Windows10ï¼CentOS7ä¸æ­£å¸¸è¿è¡ï¼Linuxå¼å®¹æ§é®é¢ä¸å¤§ï¼
+ç¼è¾å¨ï¼pycharm ## ð¿ å®è£
+ç¯å¢ä¾èµ`aiohttp`å`nonebot_plugin_htmlrender`åº
+é¨ååè½éè¦è·åèªå·±çcookieï¼éç½®envåæè½æ­£å¸¸ä½¿ç¨ï¼ ###
+1. nb-cliå®è£ï¼æ¨èï¼
+å¨ä½ botå·¥ç¨çæä»¶å¤¹ä¸ï¼è¿è¡cmdï¼è¿è¡è·¯å¾è¦å¯¹åï¼ï¼æ§è¡nbå½ä»¤å®è£æä»¶ï¼æä»¶éç½®ä¼èªå¨æ·»å è³éç½®æä»¶
+``` nb plugin install nonebot_plugin_searchBiliInfo ``` ### 2. æ¬å°å®è£
+åå®è£ä¸ `aiohttp` å `htmlrender` ``` pip install aiohttp pip install
+nonebot_plugin_htmlrender ```
+å°é¡¹ç®cloneå°ä½ çæºå¨äººæä»¶ä¸çå¯¹åºæä»¶ç®å½åï¼ä¸è¬ä¸ºæºå¨äººæä»¶å¤¹ä¸ç`src/
 plugins`ï¼ï¼ç¶åæ`nonebot_plugin_searchBiliInfo`æä»¶å¤¹éçåå®¹æ·è´è³ä¸ä¸çº§ç®å½å³å¯ã
-\ncloneå½ä»¤åèï¼å¾åè£`git`ï¼æçé½æï¼ï¼\n```\ngit clone
-https://github.com/Ikaros-521/nonebot_plugin_searchBiliInfo.git\n```
-\nä¹å¯ä»¥ç´æ¥ä¸è½½åç¼©åå°æä»¶ç®å½è§£åï¼ç¶ååæ ·æå`nonebot_plugin_searchBiliInfo`è³ä¸ä¸çº§ç®å½ã
-\nç®å½ç»æï¼ ```ä½ çbot/src/plugins/nonebot_plugin_searchBiliInfo/
-__init__.py``` \n\n\n### 3. pipå®è£\n```\npip install
-nonebot_plugin_searchBiliInfo\n``` \næå¼ nonebot2 é¡¹ç®ç ```bot.py```
-æä»¶, å¨å¶ä¸­åå¥ \n```nonebot.load_plugin
-(\'nonebot_plugin_searchBiliInfo\')``` \nå½ç¶ï¼å¦ææ¯é»è®¤nb-
+cloneå½ä»¤åèï¼å¾åè£`git`ï¼æçé½æï¼ï¼ ``` git clone https://
+github.com/Ikaros-521/nonebot_plugin_searchBiliInfo.git ```
+ä¹å¯ä»¥ç´æ¥ä¸è½½åç¼©åå°æä»¶ç®å½è§£åï¼ç¶ååæ ·æå`nonebot_plugin_searchBiliInfo`è³ä¸ä¸çº§ç®å½ã
+ç®å½ç»æï¼ ```ä½ çbot/src/plugins/nonebot_plugin_searchBiliInfo/
+__init__.py``` ### 3. pipå®è£ ``` pip install nonebot_plugin_searchBiliInfo
+``` æå¼ nonebot2 é¡¹ç®ç ```bot.py``` æä»¶, å¨å¶ä¸­åå¥
+```nonebot.load_plugin('nonebot_plugin_searchBiliInfo')```
+å½ç¶ï¼å¦ææ¯é»è®¤nb-
 cliåå»ºçnonebot2çè¯ï¼å¨botè·¯å¾```pyproject.toml```ç```
 [tool.nonebot]```ç```plugins```ä¸­æ·»å ```nonebot_plugin_searchBiliInfo```å³å¯
-\npyproject.tomléç½®ä¾å¦ï¼ \n``` \n[tool.nonebot]\nplugin_dirs = ["src/
-plugins"]\nplugins = ["nonebot_plugin_searchBiliInfo"]\n``` \n\n###
-æ´æ°çæ¬\n```\nnb plugin update nonebot_plugin_searchBiliInfo\n```\n\n##
-ð§ éç½®\n\n### cookieè·åæ¹å¼\næµè§å¨è¿å¥bç«å®ç½å¹¶ç»å½:
-`https://www.bilibili.com/
-` \nedgeï¼æå¶ä»æµè§å¨ï¼æ`f12`ï¼æé¼ æ å³é®`âæ£æ¥â`
+pyproject.tomléç½®ä¾å¦ï¼ ``` [tool.nonebot] plugin_dirs = ["src/plugins"]
+plugins = ["nonebot_plugin_searchBiliInfo"] ``` ### æ´æ°çæ¬ ``` nb plugin
+update nonebot_plugin_searchBiliInfo ``` ## ð§ éç½® ### cookieè·åæ¹å¼
+æµè§å¨è¿å¥bç«å®ç½å¹¶ç»å½: `https://www.bilibili.com/
+` edgeï¼æå¶ä»æµè§å¨ï¼æ`f12`ï¼æé¼ æ å³é®`âæ£æ¥â`
 `âå¼åèå·¥å·â`ç­ï¼, ç¶åç¹å»å³ä¸è§é£ä¸ª`">>"`ç¬¦å·,
-è¿å¥`"ç½ç»"` \nåæ`ctrl+r`ï¼æ`f5`ï¼å·æ°åç´ 
-\néä¾¿ç¹å»ä¸ä¸ªè¯·æ±,
+è¿å¥`"ç½ç»"` åæ`ctrl+r`ï¼æ`f5`ï¼å·æ°åç´ 
+éä¾¿ç¹å»ä¸ä¸ªè¯·æ±,
 å¨`âè¯·æ±æ å¤´â`éé¢æ¾å°cookieï¼æ²¡æå°±æ¢ä¸ä¸ªï¼
-\ncookieåå·åé¢çå°±æ¯cookieï¼å¤å¶ä¸ä¸, å¯ä»¥ætaæ·»å å°envé
-\nå¦æä¸æ³æ¾å¤ªå¤cookieä¿¡æ¯ï¼åªéè¦`buvid3`å­æ®µå³å¯ã \n\n###
-envéç½®\n```\n#
-å¨ä½ çenvæä»¶ä¸­æ·»å å¦ä¸éç½®ï¼æçæ¯.env.prodï¼
-ä»éè¦buvid3å­æ®µå³å¯\nsearchBiliInfo_cookie="buvid3=XXXXXXXX-XXXX-XXXX-
-XXXX-XXXXXXXXXXXXXXXXXinfoc;"\n```\n| éç½®é¡¹ | å¿å¡« | é»è®¤å¼ | è¯´æ
-|\n|:----------------:|:----:|:----:|:----------------------------:|\n|
+cookieåå·åé¢çå°±æ¯cookieï¼å¤å¶ä¸ä¸, å¯ä»¥ætaæ·»å å°envé
+å¦æä¸æ³æ¾å¤ªå¤cookieä¿¡æ¯ï¼åªéè¦`buvid3`å­æ®µå³å¯ã ###
+envéç½® ``` # å¨ä½ çenvæä»¶ä¸­æ·»å å¦ä¸éç½®ï¼æçæ¯.env.prodï¼
+ä»éè¦buvid3å­æ®µå³å¯ searchBiliInfo_cookie="buvid3=XXXXXXXX-XXXX-XXXX-
+XXXX-XXXXXXXXXXXXXXXXXinfoc;" ``` | éç½®é¡¹ | å¿å¡« | é»è®¤å¼ | è¯´æ |
+|:----------------:|:----:|:----:|:----------------------------:| |
 `searchBiliInfo_cookie` | å¦ | `""` |
-bç«cookieï¼ä»éè¦`buvid3`å­æ®µå³å¯ |\n\n\n## ð åè½\néè¿uid æ
+bç«cookieï¼ä»éè¦`buvid3`å­æ®µå³å¯ | ## ð åè½ éè¿uid æ
 è®¾å®å¥½çç­è¯­ æ
-bç«æ¥å£æç´¢æ¥è¯¢æå®bç«ç¨æ·çç²ä¸ãè°å¢ä¿¡æ¯ï¼ç´æ­æ¶çæ°æ®ï¼ç´æ­è§çä¿¡æ¯ï¼å³é®è¯ææµç§°ãUIDç­ä¿¡æ¯ï¼ä¸»æ­è¥æ¶æ¦åã\n\n##
-ð å½ä»¤(å½ä»¤åç¼èªè¡æ¿æ¢åµ~)\n\n### /æ¥\nå½ä»¤ç»æï¼```/æ¥
-(uid:æUID:æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯``` \nä¾å¦ï¼```/æ¥ uid:
-3709626``` æ ```/æ¥ :3709626``` æ ```/æ¥ bishi``` \nbotè¿ååå®¹ï¼
-\n![](docs/search.png)\n\n### /æ¥ç´æ­\nå½ä»¤ç»æï¼```/æ¥ç´æ­ (uid:
-æUID:æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯
-åºæ¬¡æ°ï¼é»è®¤ä¸åä¸ºå¨é¨ï¼``` \nä¾å¦ï¼```/æ¥ç´æ­ UID:3709626
-1``` æ ```/æ¥ç´æ­ bishi``` \nbotè¿ååå®¹ï¼å¾çï¼ï¼ \n![](docs/
-live_info.png)\n\n### /æ¥è°å¢\nå½ä»¤ç»æï¼```/æ¥è°å¢ (uid:æUID:
-æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯``` \nä¾å¦ï¼```/æ¥è°å¢
-ï¼3709626``` æ ```/æ¥è°å¢ bishi``` \nbotè¿ååå®¹(å¾ç)ï¼ \n![]
-(docs/guard.png)\n\n### /æ¥æµç§°\nå½ä»¤ç»æï¼```/æ¥æµç§°
-æµç§°å³é®è¯``` \nä¾å¦ï¼```/æ¥æµç§° ä¼å¡æ´æ¯```\nbotè¿ååå®¹
-(å¾ç)ï¼ \n![](docs/search_name.png)\n\n### /æ¥æ¶ç\nå½ä»¤ç»æï¼```/
-æ¥æ¶ç (uid:æUID:æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯ æ¶çç±»å
-(é»è®¤1: ç¤¼ç©ï¼2: ä¸è°ï¼3: SC) ååç¬¬nåº(ä»0å¼å§)```
-\nä¾å¦ï¼```/æ¥æ¶ç :3709626 ç¤¼ç© 1``` æ ```/æ¥æ¶ç bishi 2 0```
-\nbotè¿ååå®¹(å¾ç)ï¼ \n![](docs/income.png)\n\n### /
-æ¥è§ç\nå½ä»¤ç»æï¼```/æ¥è§ç (uid:æUID:æï¼æ:
-)+ç¨æ·uidææµç§°å³é®è¯``` \nä¾å¦ï¼```/æ¥è§ç UID:666666``` æ
-```/æ¥è§ç bishi``` \nbotè¿ååå®¹(å¾ç)ï¼ \n![](docs/
-watch.png)\n\n### /æ¥è§ç2\nå½ä»¤ç»æï¼```/æ¥è§ç2 (uid:æUID:
-æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯``` \nä¾å¦ï¼```/æ¥è§ç2 UID:
-666666``` æ ```/æ¥è§ç2 bishi``` \nbotè¿ååå®¹(å¾ç)ï¼ \n![](docs/
-watch2.png)\n\n### /æ¥å¼¹å¹\nå½ä»¤ç»æï¼```/æ¥å¼¹å¹ (uid:æUID:
-æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯ æ¥è¯¢çä¸»æ­æµç§°å³é®è¯æ(uid:
-æUID:æï¼æ:)+ é¡µæ°(å¯ä¸å¡«ï¼é»è®¤0) æ¡æ°(å¯ä¸å¡«ï¼é»è®¤3)```
-\nä¾å¦ï¼```/æ¥å¼¹å¹ uid:3709626 Loveä¸¶ä¼å¡æ´æ¯ 1 1``` æ ```/
-æ¥å¼¹å¹ uid:3709626 Loveä¸¶ä¼å¡æ´æ¯ 1``` \nbotè¿ååå®¹(å¾ç)ï¼ \n!
-[](docs/danmu.png)\n\n### /æ¥å¼¹å¹2\nå½ä»¤ç»æï¼```/æ¥å¼¹å¹2 (uid:
-æUID:æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯ é¡µæ°(å¯ä¸å¡«ï¼é»è®¤0)
-æ¡æ°(å¯ä¸å¡«ï¼é»è®¤3)``` \nä¾å¦ï¼```/æ¥å¼¹å¹2 uid:3709626 2 2``` æ
-```/æ¥å¼¹å¹2 uid:3709626 2``` \nbotè¿ååå®¹(å¾ç)ï¼ \n![](docs/
-danmu2.png)\n\n### /æ¥çå­\nå½ä»¤ç»æï¼```/æ¥çå­
-ä¸»æ­çå­å³é®è¯``` \nä¾å¦ï¼```/æ¥çå­ å¤©``` æ ```/æ¥çå­
-å¤©é``` \nbotè¿ååå®¹(å¾ç)ï¼ \n![](docs/medal.png)\n\n### /
-æ¥äººæ°\nå½ä»¤ç»æï¼```/æ¥äººæ° (uid:æUID:æï¼æ:
-)+ç¨æ·uidææµç§°å³é®è¯``` \nä¾å¦ï¼```/æ¥äººæ° uid:3709626``` æ
-```/æ¥äººæ° Loveä¸¶ä¼å¡æ´æ¯``` \nbotè¿ååå®¹(å¾ç)ï¼ \n![](docs/
-popularity.png)\n\n### /æ¥è£æ®\nå½ä»¤ç»æï¼```/æ¥è£æ® (uid:æUID:
-æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯``` \nä¾å¦ï¼```/æ¥è£æ® uid:2```
-æ ```/æ¥è£æ® ï¼2``` \nbotè¿ååå®¹(å¾ç)ï¼ \n![](docs/
-garb.png)\n\n### /è¥æ¶\nå½ä»¤ç»æï¼```/è¥æ¶ æ¥/å¨/ææ¦
-äººæ°ï¼ä¸å¡«é»è®¤100ï¼``` \nä¾å¦ï¼```/è¥æ¶ æ¥æ¦ 3``` æ ```/è¥æ¶
-ææ¦``` \nbotè¿ååå®¹(å¾ç)ï¼ \n![](docs/revenue.png)\n\n### /
-æ¶¨ç²\nå½ä»¤ç»æï¼```/æ¶¨ç² æ¥/å¨/ææ¦ äººæ°ï¼ä¸å¡«é»è®¤100ï¼```
-\nä¾å¦ï¼```/æ¶¨ç² æ¥æ¦ 3``` æ ```/æ¶¨ç² ææ¦``` \nbotè¿ååå®¹
-(å¾ç)ï¼ \n![](docs/incfans.png)\n\n### /DDé£äºæ¦ æ /ddé£äºæ¦ æ /
-é£äºæ¦ (å¯äº)\nå½ä»¤ç»æï¼```/DDé£äºæ¦
-topäººæ°ï¼ä¸å¡«é»è®¤10ï¼``` \nä¾å¦ï¼```/DDé£äºæ¦``` æ ```/
-é£äºæ¦ 20``` \nbotè¿ååå®¹(å¾ç)ï¼ \n![](docs/ddstats.png)\n\n### /
-vè¯¦æ æ /Vè¯¦æ æ /vè¯¦ç» æ /Vè¯¦ç»\nå½ä»¤ç»æï¼```/vè¯¦æ
-(uid:æUID:æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯``` \nä¾å¦ï¼```/vè¯¦æ
-uid:3709626``` æ ```/Vè¯¦æ ï¼2``` æ ```/vè¯¦ç» Loveä¸¶ä¼å¡æ´æ¯```
-æ ```/Vè¯¦ç» :2``` \nbotè¿ååå®¹(å¾ç)ï¼ \n![](docs/
-v_detail.png)\n\n### /vç´æ­å¿ æ /Vç´æ­å¿\nå½ä»¤ç»æï¼```/
-vç´æ­å¿``` \nä¾å¦ï¼```/vç´æ­å¿``` æ ```/Vç´æ­å¿```
-\nbotè¿ååå®¹(å¾ç)ï¼ \n![](docs/v_live.png)\n\n### /væ¥ä¸å æ /
-Væ¥ä¸å\nå½ä»¤ç»æï¼```/væ¥ä¸å``` \nä¾å¦ï¼```/væ¥ä¸å``` æ
-```/Væ¥ä¸å``` \nbotè¿ååå®¹(å¾ç)ï¼ \n![](docs/v_rise.png)\n\n### /
-væ¥ä¸é æ /Væ¥ä¸é\nå½ä»¤ç»æï¼```/væ¥ä¸é``` \nä¾å¦ï¼```/
-væ¥ä¸é``` æ ```/Væ¥ä¸é``` \nbotè¿ååå®¹(å¾ç)ï¼ \n![](docs/
-v_drop.png)\n\n### /vè°å¢ æ /Vè°å¢\nå½ä»¤ç»æï¼```/vè°å¢```
-\nä¾å¦ï¼```/vè°å¢``` æ ```/Vè°å¢``` \nbotè¿ååå®¹(å¾ç)ï¼ \n![]
-(docs/v_guard.png)\n\n### /vdd æ /VDD æ /VDDé£äºæ¦ æ /
-vddé£äºæ¦\nå½ä»¤ç»æï¼```/vdd``` \nä¾å¦ï¼```/vdd``` æ ```/VDD```
-æ ```/vddé£äºæ¦``` \nbotè¿ååå®¹(å¾ç)ï¼ \n![](docs/
-v_dd.png)\n\n### /Vå®è§ æ /vå®è§\nå½ä»¤ç»æï¼```/vdd```
-\nä¾å¦ï¼```/Vå®è§``` æ ```/vå®è§``` \nbotè¿ååå®¹(å¾ç)ï¼ \n![]
-(docs/v_macro.png)\n\n### /dmkæ¥ç¨æ· æ /DMKæ¥ç¨æ·\nå½ä»¤ç»æï¼```/
-dmkæ¥ç¨æ· (uid:æUID:æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯```
-\nä¾å¦ï¼```/dmkæ¥ç¨æ· uid:3709626``` æ ```/DMKæ¥ç¨æ·
-Loveä¸¶ä¼å¡æ´æ¯``` \nbotè¿ååå®¹(å¾ç)ï¼ \n![](docs/
-dmk_user.png)\n\n### /dmkæ¥ç´æ­ æ /DMKæ¥ç´æ­\nå½ä»¤ç»æï¼```/
+bç«æ¥å£æç´¢æ¥è¯¢æå®bç«ç¨æ·çç²ä¸ãè°å¢ä¿¡æ¯ï¼ç´æ­æ¶çæ°æ®ï¼ç´æ­è§çä¿¡æ¯ï¼å³é®è¯ææµç§°ãUIDç­ä¿¡æ¯ï¼ä¸»æ­è¥æ¶æ¦åã
+## ð å½ä»¤(å½ä»¤åç¼èªè¡æ¿æ¢åµ~) ### /æ¥ å½ä»¤ç»æï¼```/æ¥
+(uid:æUID:æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯``` ä¾å¦ï¼```/æ¥ uid:
+3709626``` æ ```/æ¥ :3709626``` æ ```/æ¥ bishi``` botè¿ååå®¹ï¼ ![]
+(docs/search.png) ### /æ¥ç´æ­ å½ä»¤ç»æï¼```/æ¥ç´æ­ (uid:æUID:
+æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯ åºæ¬¡æ°ï¼é»è®¤ä¸åä¸ºå¨é¨ï¼```
+ä¾å¦ï¼```/æ¥ç´æ­ UID:3709626 1``` æ ```/æ¥ç´æ­ bishi```
+botè¿ååå®¹ï¼å¾çï¼ï¼ ![](docs/live_info.png) ### /æ¥è°å¢
+å½ä»¤ç»æï¼```/æ¥è°å¢ (uid:æUID:æï¼æ:
+)+ç¨æ·uidææµç§°å³é®è¯``` ä¾å¦ï¼```/æ¥è°å¢ ï¼3709626``` æ ```/
+æ¥è°å¢ bishi``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/guard.png) ### /
+æ¥æµç§° å½ä»¤ç»æï¼```/æ¥æµç§° æµç§°å³é®è¯``` ä¾å¦ï¼```/
+æ¥æµç§° ä¼å¡æ´æ¯``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/search_name.png)
+### /æ¥æ¶ç å½ä»¤ç»æï¼```/æ¥æ¶ç (uid:æUID:æï¼æ:
+)+ç¨æ·uidææµç§°å³é®è¯ æ¶çç±»å(é»è®¤1: ç¤¼ç©ï¼2: ä¸è°ï¼3: SC)
+ååç¬¬nåº(ä»0å¼å§)``` ä¾å¦ï¼```/æ¥æ¶ç :3709626 ç¤¼ç© 1``` æ
+```/æ¥æ¶ç bishi 2 0``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/income.png) ###
+/æ¥è§ç å½ä»¤ç»æï¼```/æ¥è§ç (uid:æUID:æï¼æ:
+)+ç¨æ·uidææµç§°å³é®è¯``` ä¾å¦ï¼```/æ¥è§ç UID:666666``` æ ```/
+æ¥è§ç bishi``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/watch.png) ### /
+æ¥è§ç2 å½ä»¤ç»æï¼```/æ¥è§ç2 (uid:æUID:æï¼æ:
+)+ç¨æ·uidææµç§°å³é®è¯``` ä¾å¦ï¼```/æ¥è§ç2 UID:666666``` æ ```/
+æ¥è§ç2 bishi``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/watch2.png) ### /
+æ¥å¼¹å¹ å½ä»¤ç»æï¼```/æ¥å¼¹å¹ (uid:æUID:æï¼æ:
+)+ç¨æ·uidææµç§°å³é®è¯ æ¥è¯¢çä¸»æ­æµç§°å³é®è¯æ(uid:æUID:
+æï¼æ:)+ é¡µæ°(å¯ä¸å¡«ï¼é»è®¤0) æ¡æ°(å¯ä¸å¡«ï¼é»è®¤3)```
+ä¾å¦ï¼```/æ¥å¼¹å¹ uid:3709626 Loveä¸¶ä¼å¡æ´æ¯ 1 1``` æ ```/æ¥å¼¹å¹
+uid:3709626 Loveä¸¶ä¼å¡æ´æ¯ 1``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/
+danmu.png) ### /æ¥å¼¹å¹2 å½ä»¤ç»æï¼```/æ¥å¼¹å¹2 (uid:æUID:æï¼æ:
+)+ç¨æ·uidææµç§°å³é®è¯ é¡µæ°(å¯ä¸å¡«ï¼é»è®¤0) æ¡æ°
+(å¯ä¸å¡«ï¼é»è®¤3)``` ä¾å¦ï¼```/æ¥å¼¹å¹2 uid:3709626 2 2``` æ ```/
+æ¥å¼¹å¹2 uid:3709626 2``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/danmu2.png) ###
+/æ¥çå­ å½ä»¤ç»æï¼```/æ¥çå­ ä¸»æ­çå­å³é®è¯``` ä¾å¦ï¼```/
+æ¥çå­ å¤©``` æ ```/æ¥çå­ å¤©é``` botè¿ååå®¹(å¾ç)ï¼ ![]
+(docs/medal.png) ### /æ¥äººæ° å½ä»¤ç»æï¼```/æ¥äººæ° (uid:æUID:
+æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯``` ä¾å¦ï¼```/æ¥äººæ° uid:
+3709626``` æ ```/æ¥äººæ° Loveä¸¶ä¼å¡æ´æ¯``` botè¿ååå®¹(å¾ç)ï¼
+![](docs/popularity.png) ### /æ¥è£æ® å½ä»¤ç»æï¼```/æ¥è£æ® (uid:
+æUID:æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯``` ä¾å¦ï¼```/æ¥è£æ® uid:
+2``` æ ```/æ¥è£æ® ï¼2``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/garb.png)
+### /è¥æ¶ å½ä»¤ç»æï¼```/è¥æ¶ æ¥/å¨/ææ¦
+äººæ°ï¼ä¸å¡«é»è®¤100ï¼``` ä¾å¦ï¼```/è¥æ¶ æ¥æ¦ 3``` æ ```/è¥æ¶
+ææ¦``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/revenue.png) ### /æ¶¨ç²
+å½ä»¤ç»æï¼```/æ¶¨ç² æ¥/å¨/ææ¦ äººæ°ï¼ä¸å¡«é»è®¤100ï¼```
+ä¾å¦ï¼```/æ¶¨ç² æ¥æ¦ 3``` æ ```/æ¶¨ç² ææ¦``` botè¿ååå®¹
+(å¾ç)ï¼ ![](docs/incfans.png) ### /DDé£äºæ¦ æ /ddé£äºæ¦ æ /
+é£äºæ¦ (å¯äº) å½ä»¤ç»æï¼```/DDé£äºæ¦
+topäººæ°ï¼ä¸å¡«é»è®¤10ï¼``` ä¾å¦ï¼```/DDé£äºæ¦``` æ ```/é£äºæ¦
+20``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/ddstats.png) ### /vè¯¦æ æ /
+Vè¯¦æ æ /vè¯¦ç» æ /Vè¯¦ç» å½ä»¤ç»æï¼```/vè¯¦æ (uid:æUID:
+æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯``` ä¾å¦ï¼```/vè¯¦æ uid:3709626```
+æ ```/Vè¯¦æ ï¼2``` æ ```/vè¯¦ç» Loveä¸¶ä¼å¡æ´æ¯``` æ ```/Vè¯¦ç»
+:2``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/v_detail.png) ### /vç´æ­å¿ æ /
+Vç´æ­å¿ å½ä»¤ç»æï¼```/vç´æ­å¿``` ä¾å¦ï¼```/vç´æ­å¿``` æ ```/
+Vç´æ­å¿``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/v_live.png) ### /væ¥ä¸å
+æ /Væ¥ä¸å å½ä»¤ç»æï¼```/væ¥ä¸å``` ä¾å¦ï¼```/væ¥ä¸å``` æ
+```/Væ¥ä¸å``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/v_rise.png) ### /
+væ¥ä¸é æ /Væ¥ä¸é å½ä»¤ç»æï¼```/væ¥ä¸é``` ä¾å¦ï¼```/
+væ¥ä¸é``` æ ```/Væ¥ä¸é``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/
+v_drop.png) ### /vè°å¢ æ /Vè°å¢ å½ä»¤ç»æï¼```/vè°å¢```
+ä¾å¦ï¼```/vè°å¢``` æ ```/Vè°å¢``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/
+v_guard.png) ### /vdd æ /VDD æ /VDDé£äºæ¦ æ /vddé£äºæ¦
+å½ä»¤ç»æï¼```/vdd``` ä¾å¦ï¼```/vdd``` æ ```/VDD``` æ ```/
+vddé£äºæ¦``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/v_dd.png) ### /Vå®è§ æ
+/vå®è§ å½ä»¤ç»æï¼```/vdd``` ä¾å¦ï¼```/Vå®è§``` æ ```/vå®è§```
+botè¿ååå®¹(å¾ç)ï¼ ![](docs/v_macro.png) ### /dmkæ¥ç¨æ· æ /
+DMKæ¥ç¨æ· å½ä»¤ç»æï¼```/dmkæ¥ç¨æ· (uid:æUID:æï¼æ:
+)+ç¨æ·uidææµç§°å³é®è¯``` ä¾å¦ï¼```/dmkæ¥ç¨æ· uid:3709626``` æ
+```/DMKæ¥ç¨æ· Loveä¸¶ä¼å¡æ´æ¯``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/
+dmk_user.png) ### /dmkæ¥ç´æ­ æ /DMKæ¥ç´æ­ å½ä»¤ç»æï¼```/
 dmkæ¥ç´æ­ (uid:æUID:æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯```
-\nä¾å¦ï¼```/dmkæ¥ç´æ­ uid:3709626``` æ ```/DMKæ¥ç´æ­
-Loveä¸¶ä¼å¡æ´æ¯``` \nbotè¿ååå®¹(å¾ç)ï¼ \n![](docs/
-dmk_live.png)\n\n### /blgæ¥å¼¹å¹ æ /BLGæ¥å¼¹å¹\nå½ä»¤ç»æï¼```/
+ä¾å¦ï¼```/dmkæ¥ç´æ­ uid:3709626``` æ ```/DMKæ¥ç´æ­
+Loveä¸¶ä¼å¡æ´æ¯``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/dmk_live.png) ### /
+dmkåæ æ /DMKåæ å½ä»¤ç»æï¼```/dmkåæ (uid:æUID:æï¼æ:
+)+ç¨æ·uidææµç§°å³é®è¯``` ä¾å¦ï¼```/dmkåæ uid:3709626``` æ ```/
+DMKåæ Loveä¸¶ä¼å¡æ´æ¯``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/
+dmk_analyze.png) ### /blgæ¥å¼¹å¹ æ /BLGæ¥å¼¹å¹ å½ä»¤ç»æï¼```/
 blgæ¥å¼¹å¹ (uid:æUID:æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯```
-\nä¾å¦ï¼```/blgæ¥å¼¹å¹ uid:3709626``` æ ```/BLGæ¥å¼¹å¹
-Loveä¸¶ä¼å¡æ´æ¯``` \nbotè¿ååå®¹(å¾ç)ï¼ \n![](docs/
-blg_danmu.png)\n\n### /blgæ¥å¥åº æ /BLGæ¥å¥åº\nå½ä»¤ç»æï¼```/
-blgæ¥å¥åº (uid:æUID:æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯```
-\nä¾å¦ï¼```/blgæ¥å¥åº uid:3709626``` æ ```/BLGæ¥å¥åº
-Loveä¸¶ä¼å¡æ´æ¯``` \nbotè¿ååå®¹(å¾ç)ï¼ \n![](docs/
-blg_enter.png)\n\n### /blgæ¥ç¤¼ç© æ /BLGæ¥ç¤¼ç©\nå½ä»¤ç»æï¼```/
-blgæ¥ç¤¼ç© (uid:æUID:æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯```
-\nä¾å¦ï¼```/blgæ¥ç¤¼ç© uid:3709626``` æ ```/BLGæ¥ç¤¼ç©
-Loveä¸¶ä¼å¡æ´æ¯``` \nbotè¿ååå®¹(å¾ç)ï¼ \n![](docs/
-blg_gift.png)\n\n### /blgç´æ­è®°å½ æ /BLGç´æ­è®°å½\nå½ä»¤ç»æï¼```/
+ä¾å¦ï¼```/blgæ¥å¼¹å¹ uid:3709626``` æ ```/BLGæ¥å¼¹å¹
+Loveä¸¶ä¼å¡æ´æ¯``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/blg_danmu.png) ### /
+blgæ¥å¥åº æ /BLGæ¥å¥åº å½ä»¤ç»æï¼```/blgæ¥å¥åº (uid:æUID:
+æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯``` ä¾å¦ï¼```/blgæ¥å¥åº uid:
+3709626``` æ ```/BLGæ¥å¥åº Loveä¸¶ä¼å¡æ´æ¯``` botè¿ååå®¹
+(å¾ç)ï¼ ![](docs/blg_enter.png) ### /blgæ¥ç¤¼ç© æ /BLGæ¥ç¤¼ç©
+å½ä»¤ç»æï¼```/blgæ¥ç¤¼ç© (uid:æUID:æï¼æ:
+)+ç¨æ·uidææµç§°å³é®è¯``` ä¾å¦ï¼```/blgæ¥ç¤¼ç© uid:3709626``` æ
+```/BLGæ¥ç¤¼ç© Loveä¸¶ä¼å¡æ´æ¯``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/
+blg_gift.png) ### /blgç´æ­è®°å½ æ /BLGç´æ­è®°å½ å½ä»¤ç»æï¼```/
 blgç´æ­è®°å½ (uid:æUID:æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯```
-\nä¾å¦ï¼```/blgç´æ­è®°å½ uid:3709626``` æ ```/BLGç´æ­è®°å½
-Loveä¸¶ä¼å¡æ´æ¯``` \nbotè¿ååå®¹(å¾ç)ï¼ \n![](docs/
-blg_tp.png)\n\n### /blgç´æ­é´sc æ /BLGç´æ­é´SC\nå½ä»¤ç»æï¼```/
-blgç´æ­é´sc (uid:æUID:æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯```
-\nä¾å¦ï¼```/blgç´æ­é´sc uid:3709626``` æ ```/BLGç´æ­é´SC
-Loveä¸¶ä¼å¡æ´æ¯``` \nbotè¿ååå®¹(å¾ç)ï¼ \n![](docs/
-blg_sc.png)\n\n### /icuæ¥ç´æ­ æ /ICUæ¥ç´æ­ æ /
-matsuriæ¥ç´æ­\nå½ä»¤ç»æï¼```/icuæ¥ç´æ­ (uid:æUID:æï¼æ:
-)+ç¨æ·uidææµç§°å³é®è¯``` \nä¾å¦ï¼```/icuæ¥ç´æ­ uid:3709626``` æ
-```/ICUæ¥ç´æ­ Loveä¸¶ä¼å¡æ´æ¯``` \nbotè¿ååå®¹(å¾ç)ï¼ \n![]
-(docs/icu_live.png)\n\n### /lapæ¥ç¨æ· æ /LAPæ¥ç¨æ·\nå½ä»¤ç»æï¼```/
+ä¾å¦ï¼```/blgç´æ­è®°å½ uid:3709626``` æ ```/BLGç´æ­è®°å½
+Loveä¸¶ä¼å¡æ´æ¯``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/blg_tp.png) ### /
+blgç´æ­é´sc æ /BLGç´æ­é´SC å½ä»¤ç»æï¼```/blgç´æ­é´sc (uid:
+æUID:æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯``` ä¾å¦ï¼```/blgç´æ­é´sc
+uid:3709626``` æ ```/BLGç´æ­é´SC Loveä¸¶ä¼å¡æ´æ¯``` botè¿ååå®¹
+(å¾ç)ï¼ ![](docs/blg_sc.png) ### /icuæ¥ç´æ­ æ /ICUæ¥ç´æ­ æ /
+matsuriæ¥ç´æ­ å½ä»¤ç»æï¼```/icuæ¥ç´æ­ (uid:æUID:æï¼æ:
+)+ç¨æ·uidææµç§°å³é®è¯``` ä¾å¦ï¼```/icuæ¥ç´æ­ uid:3709626``` æ
+```/ICUæ¥ç´æ­ Loveä¸¶ä¼å¡æ´æ¯``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/
+icu_live.png) ### /lapæ¥ç¨æ· æ /LAPæ¥ç¨æ· å½ä»¤ç»æï¼```/
 lapæ¥ç¨æ· (uid:æUID:æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯```
-\nä¾å¦ï¼```/lapæ¥ç¨æ· uid:387636363``` æ ```/LAPæ¥ç¨æ· é«ãã```
-\nbotè¿ååå®¹(å¾ç)ï¼ \n![](docs/laplace_user.png)\n\n### /lapæ¥çå­
-æ /LAPæ¥çå­\nå½ä»¤ç»æï¼```/lapæ¥çå­ (uid:æUID:æï¼æ:
-)+ç¨æ·uidææµç§°å³é®è¯``` \nä¾å¦ï¼```/lapæ¥çå­ uid:387636363```
-æ ```/LAPæ¥çå­ é«ãã``` \nbotè¿ååå®¹(å¾ç)ï¼ \n![](docs/
-laplace_medal.png)\n\n### /lapæ¥åçµ æ /LAPæ¥åçµ\nå½ä»¤ç»æï¼```/
+ä¾å¦ï¼```/lapæ¥ç¨æ· uid:387636363``` æ ```/LAPæ¥ç¨æ· é«ãã```
+botè¿ååå®¹(å¾ç)ï¼ ![](docs/laplace_user.png) ### /lapæ¥çå­ æ /
+LAPæ¥çå­ å½ä»¤ç»æï¼```/lapæ¥çå­ (uid:æUID:æï¼æ:
+)+ç¨æ·uidææµç§°å³é®è¯``` ä¾å¦ï¼```/lapæ¥çå­ uid:387636363``` æ
+```/LAPæ¥çå­ é«ãã``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/
+laplace_medal.png) ### /lapæ¥åçµ æ /LAPæ¥åçµ å½ä»¤ç»æï¼```/
 lapæ¥åçµ (uid:æUID:æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯```
-\nä¾å¦ï¼```/lapæ¥åçµ uid:387636363``` æ ```/LAPæ¥åçµ é«ãã```
-\nbotè¿ååå®¹(å¾ç)ï¼ \n![](docs/laplace_upower.png)\n\n### /lapdd æ /
-LAPDD æ /lapddæè¡æ¦\nå½ä»¤ç»æï¼```/lapdd æç´¢ç±»å(é»è®¤0:
-æä¾ï¼1: æ»ç£ï¼2: æç£ï¼3ï¼è°é¿)``` \nä¾å¦ï¼```/lapdd``` æ
-```/lapdd 1``` æ ```/LAPDD è°é¿``` \nbotè¿ååå®¹(å¾ç)ï¼ \n![](docs/
-laplace_dd.png)\n\n### /zeroæ¥ç¨æ· æ /ZEROæ¥ç¨æ·\nå½ä»¤ç»æï¼```/
-zeroæ¥ç¨æ· (uid:æUID:æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯```
-\nä¾å¦ï¼```/zeroæ¥ç¨æ· uid:387636363``` æ ```/ZEROæ¥ç¨æ·
-é«ãã``` \nbotè¿ååå®¹(å¾ç)ï¼ \n![](docs/
-zeroroku_author.png)\n\n### /zeroè¢«å³æ³¨ æ /
-ZEROè¢«å³æ³¨\nå½ä»¤ç»æï¼```/zeroè¢«å³æ³¨ (uid:æUID:æï¼æ:
-)+ç¨æ·uidææµç§°å³é®è¯``` \nä¾å¦ï¼```/zeroè¢«å³æ³¨ uid:387636363```
-æ ```/ZEROè¢«å³æ³¨ é«ãã``` \nbotè¿ååå®¹(å¾ç)ï¼ \n![](docs/
-zeroroku_famous_fans.png)\n\n### æè« æ ä¸»æ­pk æ
-ä¸»æ­PK\nå½ä»¤ç»æï¼`æè«|ä¸»æ­pk|ä¸»æ­PK
-ç¨æ·1çuidææµç§°å³é®è¯ ç¨æ·2çuidææµç§°å³é®è¯
-ç¨æ·nçuidææµç§°å³é®è¯ #å½å¤©åè¿å»åç§»å¤©(èµ·å§)
-å½å¤©åè¿å»åç§»å¤©æ°
-(ç»å°¾)`\næ³¨æï¼`#`ååé¢ç`æ¥æåç§»`å¯ä»¥é»è®¤ä¸å¡«ï¼ä¸å¡«åçè¯é»è®¤æ¯ä¸ä¸ªæåå°ä»å¤©çæ°æ®ãå¦å¤ï¼ä¼ å¥çç¨æ·å¿é¡»å¤§äºç­äº2äººä»¥ä¸ãï¼`æ¥æåç§»`å¶å®å°±æ¯`æ°æ®åºé´`å¦ï¼\nä¾å¦ï¼```æè«
-é«é± neol``` æ ```æè« é«é± neol #5 0``` æ ```ä¸»æ­pk é«é± é« #15
-0``` \nbotè¿ååå®¹(å¾ç)ï¼ \n![](docs/
-stats_nailv_live_compare.png)\n\n\n### ehæ¥ç´æ­ æ è¯¶å¿æ¥ç´æ­ æ
-eiheiæ¥ç´æ­\nå½ä»¤ç»æï¼```/ehæ¥ç´æ­ (uid:æUID:æï¼æ:
-)+ç¨æ·uidææµç§°å³é®è¯``` \nä¾å¦ï¼```/è¯¶å¿æ¥ç´æ­ uid:
-3493132603754688``` æ ```/è¯¶å¿æ¥ç´æ­ ç½äºRoya``` \nbotè¿ååå®¹
-(å¾ç)ï¼ \n![](docs/eihei_livepic.png)\n\n### /
-vtbç½ç«\nå½ä»¤ç»æï¼```/vtbç½ç«``` æ ```/vtbèµæº``` \nä¾å¦ï¼```/
-vtbç½ç«``` æ ```/vtbèµæº``` \nbotè¿ååå®¹ï¼
-\n```\nVTBæ°æ®çæ¿ï¼https://ikaros-521.gitee.io/vtb_data_board/
-\nmatsuriï¼https://matsuri.icu/\ndanmakusï¼https://danmakus.com/
-\nvtbs.funï¼http://www.vtbs.fun/\nbiligankï¼https://biligank.com/
-\nç«é¾æ¦ï¼https://huolonglive.com/#/\nvtbs.moeï¼https://vtbs.moe/
-\nvup.loveava.topï¼https://vup.loveava.top/ranking\nddstatsï¼https://
-ddstats.ericlamm.xyz/\nzerorokuï¼https://zeroroku.com/
-bilibili\nlaplaceï¼https://laplace.live/\n```\n\n## â
-æå±\nå¯ç¨å³é®è¯æç´¢ï¼éè¦å¨`.env.xx`ä¸­éç½®èªå·±ç`cookie`ã\n\nå½ä»¤ä¿®æ¹ï¼
-\næµç§°èªå®ä¹ï¼ä¿®æ¹`data.py`ï¼å¨æä»¶å¤´é¨è¿½å ä½ éè¦å®ä¹çç¨æ·çjsonä¸²ï¼æ³¨æjsonæ ¼å¼ï¼ï¼ï¼
-\nå½ä»¤èªå®ä¹ï¼ä¿®æ¹`__init__.py`ï¼`catch_str =
+ä¾å¦ï¼```/lapæ¥åçµ uid:387636363``` æ ```/LAPæ¥åçµ é«ãã```
+botè¿ååå®¹(å¾ç)ï¼ ![](docs/laplace_upower.png) ### /lapdd æ /LAPDD
+æ /lapddæè¡æ¦ å½ä»¤ç»æï¼```/lapdd æç´¢ç±»å(é»è®¤0: æä¾ï¼1:
+æ»ç£ï¼2: æç£ï¼3ï¼è°é¿)``` ä¾å¦ï¼```/lapdd``` æ ```/lapdd 1```
+æ ```/LAPDD è°é¿``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/laplace_dd.png) ###
+/zeroæ¥ç¨æ· æ /ZEROæ¥ç¨æ· å½ä»¤ç»æï¼```/zeroæ¥ç¨æ· (uid:æUID:
+æï¼æ:)+ç¨æ·uidææµç§°å³é®è¯``` ä¾å¦ï¼```/zeroæ¥ç¨æ· uid:
+387636363``` æ ```/ZEROæ¥ç¨æ· é«ãã``` botè¿ååå®¹(å¾ç)ï¼ ![]
+(docs/zeroroku_author.png) ### /zeroè¢«å³æ³¨ æ /ZEROè¢«å³æ³¨
+å½ä»¤ç»æï¼```/zeroè¢«å³æ³¨ (uid:æUID:æï¼æ:
+)+ç¨æ·uidææµç§°å³é®è¯``` ä¾å¦ï¼```/zeroè¢«å³æ³¨ uid:387636363```
+æ ```/ZEROè¢«å³æ³¨ é«ãã``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/
+zeroroku_famous_fans.png) ### æè« æ ä¸»æ­pk æ ä¸»æ­PK
+å½ä»¤ç»æï¼`æè«|ä¸»æ­pk|ä¸»æ­PK ç¨æ·1çuidææµç§°å³é®è¯
+ç¨æ·2çuidææµç§°å³é®è¯ ç¨æ·nçuidææµç§°å³é®è¯
+#å½å¤©åè¿å»åç§»å¤©(èµ·å§) å½å¤©åè¿å»åç§»å¤©æ°(ç»å°¾)`
+æ³¨æï¼`#`ååé¢ç`æ¥æåç§»`å¯ä»¥é»è®¤ä¸å¡«ï¼ä¸å¡«åçè¯é»è®¤æ¯ä¸ä¸ªæåå°ä»å¤©çæ°æ®ãå¦å¤ï¼ä¼ å¥çç¨æ·å¿é¡»å¤§äºç­äº2äººä»¥ä¸ãï¼`æ¥æåç§»`å¶å®å°±æ¯`æ°æ®åºé´`å¦ï¼
+ä¾å¦ï¼```æè« é«é± neol``` æ ```æè« é«é± neol #5 0``` æ
+```ä¸»æ­pk é«é± é« #15 0``` botè¿ååå®¹(å¾ç)ï¼ ![](docs/
+stats_nailv_live_compare.png) ### ehæ¥ç´æ­ æ è¯¶å¿æ¥ç´æ­ æ
+eiheiæ¥ç´æ­ å½ä»¤ç»æï¼```/ehæ¥ç´æ­ (uid:æUID:æï¼æ:
+)+ç¨æ·uidææµç§°å³é®è¯``` ä¾å¦ï¼```/è¯¶å¿æ¥ç´æ­ uid:
+3493132603754688``` æ ```/è¯¶å¿æ¥ç´æ­ ç½äºRoya``` botè¿ååå®¹
+(å¾ç)ï¼ ![](docs/eihei_livepic.png) ### /vtbç½ç« å½ä»¤ç»æï¼```/
+vtbç½ç«``` æ ```/vtbèµæº``` ä¾å¦ï¼```/vtbç½ç«``` æ ```/
+vtbèµæº``` botè¿ååå®¹ï¼ ``` VTBæ°æ®çæ¿ï¼https://ikaros-
+521.gitee.io/vtb_data_board/ matsuriï¼https://matsuri.icu/ danmakusï¼https://
+danmakus.com/ vtbs.funï¼http://www.vtbs.fun/ biligankï¼https://biligank.com/
+ç«é¾æ¦ï¼https://huolonglive.com/#/ vtbs.moeï¼https://vtbs.moe/
+vup.loveava.topï¼https://vup.loveava.top/ranking ddstatsï¼https://
+ddstats.ericlamm.xyz/ zerorokuï¼https://zeroroku.com/bilibili laplaceï¼https:
+//laplace.live/ ``` ## â æå±
+å¯ç¨å³é®è¯æç´¢ï¼éè¦å¨`.env.xx`ä¸­éç½®èªå·±ç`cookie`ã
+å½ä»¤ä¿®æ¹ï¼
+æµç§°èªå®ä¹ï¼ä¿®æ¹`data.py`ï¼å¨æä»¶å¤´é¨è¿½å ä½ éè¦å®ä¹çç¨æ·çjsonä¸²ï¼æ³¨æjsonæ ¼å¼ï¼ï¼ï¼
+å½ä»¤èªå®ä¹ï¼ä¿®æ¹`__init__.py`ï¼`catch_str =
 on_command`è¿é¨åçä»£ç å³å¯ã
-\n\nbotè¿ååå®¹æ ¼å¼ä¿®æ¹å¯¹åºçmsgãout_stråéçåå®¹ \n\n##
-ð æ´æ°æ¥å¿\n\n\nå±å¼/æ¶èµ·\n\n### 0.0.1\n\n-
-æä»¶åæ¬¡åå¸\n\n### 0.1.0\n\n-
-æ´æ°åºäºvtbs.moeçä¸»æ­æ°æ®ï¼æ·»å å³é®è¯æç´¢åè½\n\n###
-1.0.0\n\næ°å¢ä»¥ä¸åè½ï¼å¶å®æ¯LX_Botçç¸å³å½ä»¤èè¿æ¥äºï¼\n-
-/æ¥ æµç§°å³é®è¯\n- /æ¥ç´æ­ æµç§°å³é®è¯ åºæ¬¡æ°\n- /æ¥è°å¢
-æµç§°å³é®è¯\n- /æ¥æµç§° æµç§°å³é®è¯\n- /æ¥æ¶ç æ¶çç±»å
-(é»è®¤1: ç¤¼ç©ï¼2: ä¸è°ï¼3: SC) ç¨æ·uidææµç§°å³é®è¯ ååç¬¬nåº
-(ä»0å¼å§)\n- /æ¥æå è§ç æµç§°å³é®è¯\n- /æ¥æå å¼¹å¹
-æ¥è¯¢çç®æ äºº æ¥è¯¢çä¸»æ­ é¡µæ° æ¡æ°\n\n###
-1.0.4\n\nä¼åéå¯¹uidè§£ææ¹å¼\n\n###
-1.0.5\n\nä¿®æ¹cookieéç½®ä»envè·åï¼æ¹ä¾¿ç¨æ·éç½®\n\n###
-1.0.6\n\nä¿®å¤ /æ¥æå å¼¹å¹
-æ°æ®è§£æbugï¼\nä¼åæ´ä½ä»£ç å®ç°ï¼\n\n### 1.1.0\næ°å¢åè½\n- /
-è¥æ¶ æ¥/å¨/ææ¦ äººæ°ï¼ä¸å¡«é»è®¤100ï¼\n\n###
-1.2.0\nå¼ç¨requestsåºï¼æ¹ä¸ºaiohttp \n\n###
-1.2.1\nä¿®å¤æ¥å½ä»¤aiohttpééæ§bug \n\n### 1.3.0\nä¿®æ¹ æ¥æå
-å¼¹å¹ å æ¥æå è§ç å½ä»¤ä¸º æ¥å¼¹å¹ å æ¥è§çã
-\nä¼åå½ä»¤è§£æå®ç°ã \nä¿®å¤æ¥å¼¹å¹æ°æ®è§£æbugã \n\n###
-1.3.1\næ°å¢ /æ¥å¼¹å¹2 å½ä»¤ã \nä¿®å¤æ¥å¼¹å¹æ°æ®è§£æbugã
-\nå¾çUIä¼åã \n\n### 1.3.2\nä¼å /æ¥å¼¹å¹2
-å½ä»¤ï¼å¢å ä¸»æ­åã \n\n### 1.3.3\nä¿®å¤ /æ¥è§ç
-å ä¸ºæ°æ®æºæåä¸ç¨æ·åä¸åuidçæåµå¯¼è´çè¶çbugã
-\n\n### 1.3.4\nä¼åå¼å¸¸æ¥éçå¤çã
-\nä¼åUIè®¾è®¡åé¨ååè½ã \n\n### 1.3.5\næ°å¢`/æ¥æ¶ç xx
-è°é¿`å`uidï¼`çå¹éãï¼ä½æ¯è°é¿ä»ç¶æ¯ææä¸è°æ°æ®ï¼
-\n\n### 1.3.6\nä¼åAPIæå½©æ¶åçå¼å¸¸æè·å¤çã \n\n###
-1.3.7\næä»¶è¡¥ååä¿¡æ¯ã \n\n### 1.3.8\næ°å¢`vtbç½ç«` æ
-`vtbèµæº` å½ä»¤ï¼å½ä»¤åç¼èªè¡æ·»å ï¼ \n\n###
-1.3.9\nè¡¥å2ä¸ªVTBèµæºç«ç¹ \n\n###
-1.3.10\néévtbs.funçè¥æ¶æ¥å£åå¨ \n\n###
-1.4.0\nä¿®æ¹on_keywordä¸ºon_commandï¼ä»èééèªå®ä¹çå½ä»¤åç¼
-\n\n###
-1.4.1\nä¿®æ¹danmakus.comå°æ°åådanmakus.comï¼æ¥å£ä¹åæ­¥æ¿æ¢äºã
-\n\n### 1.4.2\næ°å¢markdownçç¹æ®å­ç¬¦è¿æ»¤åææ¬è¶é¿æ¢è¡ã
-\npsï¼vtbs.funæäºï¼`è¥æ¶`åè½ææ¶æ æ³ä½¿ç¨ã\n\n###
-1.4.3\nvtbs.funæ´»äºï¼å äºsslï¼å·²å¼å®¹ã \n\n### 1.4.4\næ°å¢å½ä»¤
-æ¶¨ç²ï¼æ¥å£æºèªvtbs.funï¼åè¥æ¶ åºæ¬ä¸è´ï¼ \n\n###
-1.4.5\næ°å¢å½ä»¤ DDé£äºæ¦ï¼æ¥å£æºèªddstats-api.ericlamm.xyz \n\n###
-1.4.6\nè¡¥åéæ¼çæä»¶åä¿¡æ¯ \n\n### 1.4.7\næ°å¢åè½
+botè¿ååå®¹æ ¼å¼ä¿®æ¹å¯¹åºçmsgãout_stråéçåå®¹ ## ð
+æ´æ°æ¥å¿  å±å¼/æ¶èµ· ### 0.0.1 - æä»¶åæ¬¡åå¸ ### 0.1.0 -
+æ´æ°åºäºvtbs.moeçä¸»æ­æ°æ®ï¼æ·»å å³é®è¯æç´¢åè½ ### 1.0.0
+æ°å¢ä»¥ä¸åè½ï¼å¶å®æ¯LX_Botçç¸å³å½ä»¤èè¿æ¥äºï¼ - /æ¥
+æµç§°å³é®è¯ - /æ¥ç´æ­ æµç§°å³é®è¯ åºæ¬¡æ° - /æ¥è°å¢
+æµç§°å³é®è¯ - /æ¥æµç§° æµç§°å³é®è¯ - /æ¥æ¶ç æ¶çç±»å(é»è®¤1:
+ç¤¼ç©ï¼2: ä¸è°ï¼3: SC) ç¨æ·uidææµç§°å³é®è¯ ååç¬¬nåº
+(ä»0å¼å§) - /æ¥æå è§ç æµç§°å³é®è¯ - /æ¥æå å¼¹å¹
+æ¥è¯¢çç®æ äºº æ¥è¯¢çä¸»æ­ é¡µæ° æ¡æ° ### 1.0.4
+ä¼åéå¯¹uidè§£ææ¹å¼ ### 1.0.5
+ä¿®æ¹cookieéç½®ä»envè·åï¼æ¹ä¾¿ç¨æ·éç½® ### 1.0.6 ä¿®å¤ /æ¥æå
+å¼¹å¹ æ°æ®è§£æbugï¼ ä¼åæ´ä½ä»£ç å®ç°ï¼ ### 1.1.0 æ°å¢åè½ -
+/è¥æ¶ æ¥/å¨/ææ¦ äººæ°ï¼ä¸å¡«é»è®¤100ï¼ ### 1.2.0
+å¼ç¨requestsåºï¼æ¹ä¸ºaiohttp ### 1.2.1 ä¿®å¤æ¥å½ä»¤aiohttpééæ§bug
+### 1.3.0 ä¿®æ¹ æ¥æå å¼¹å¹ å æ¥æå è§ç å½ä»¤ä¸º æ¥å¼¹å¹ å
+æ¥è§çã ä¼åå½ä»¤è§£æå®ç°ã ä¿®å¤æ¥å¼¹å¹æ°æ®è§£æbugã ###
+1.3.1 æ°å¢ /æ¥å¼¹å¹2 å½ä»¤ã ä¿®å¤æ¥å¼¹å¹æ°æ®è§£æbugã
+å¾çUIä¼åã ### 1.3.2 ä¼å /æ¥å¼¹å¹2 å½ä»¤ï¼å¢å ä¸»æ­åã ###
+1.3.3 ä¿®å¤ /æ¥è§ç
+å ä¸ºæ°æ®æºæåä¸ç¨æ·åä¸åuidçæåµå¯¼è´çè¶çbugã ###
+1.3.4 ä¼åå¼å¸¸æ¥éçå¤çã ä¼åUIè®¾è®¡åé¨ååè½ã ### 1.3.5
+æ°å¢`/æ¥æ¶ç xx
+è°é¿`å`uidï¼`çå¹éãï¼ä½æ¯è°é¿ä»ç¶æ¯ææä¸è°æ°æ®ï¼ ###
+1.3.6 ä¼åAPIæå½©æ¶åçå¼å¸¸æè·å¤çã ### 1.3.7
+æä»¶è¡¥ååä¿¡æ¯ã ### 1.3.8 æ°å¢`vtbç½ç«` æ `vtbèµæº`
+å½ä»¤ï¼å½ä»¤åç¼èªè¡æ·»å ï¼ ### 1.3.9 è¡¥å2ä¸ªVTBèµæºç«ç¹ ###
+1.3.10 éévtbs.funçè¥æ¶æ¥å£åå¨ ### 1.4.0
+ä¿®æ¹on_keywordä¸ºon_commandï¼ä»èééèªå®ä¹çå½ä»¤åç¼ ### 1.4.1
+ä¿®æ¹danmakus.comå°æ°åådanmakus.comï¼æ¥å£ä¹åæ­¥æ¿æ¢äºã ###
+1.4.2 æ°å¢markdownçç¹æ®å­ç¬¦è¿æ»¤åææ¬è¶é¿æ¢è¡ã
+psï¼vtbs.funæäºï¼`è¥æ¶`åè½ææ¶æ æ³ä½¿ç¨ã ### 1.4.3
+vtbs.funæ´»äºï¼å äºsslï¼å·²å¼å®¹ã ### 1.4.4 æ°å¢å½ä»¤
+æ¶¨ç²ï¼æ¥å£æºèªvtbs.funï¼åè¥æ¶ åºæ¬ä¸è´ï¼ ### 1.4.5
+æ°å¢å½ä»¤ DDé£äºæ¦ï¼æ¥å£æºèªddstats-api.ericlamm.xyz ### 1.4.6
+è¡¥åéæ¼çæä»¶åä¿¡æ¯ ### 1.4.7 æ°å¢åè½
 æ¥çå­ï¼æ°æ®æºèªæ¬å°ç¬åï¼vtbs.moeä¸­ä¸»æ­çå­ä¿¡æ¯ï¼å±4273æ¡æ°æ®ï¼
-\n\n### 1.4.8\nè¡¥åæçå­éæ¼ç1æ¡æ°æ® \n\n###
-1.4.9\nè¡¥åéæ¼ç vtbç½ç« åè½åä¿¡æ¯ \n\n###
-1.4.10\næ°å¢åè½`vè¯¦æ` `dmkæ¥ç¨æ·`
+### 1.4.8 è¡¥åæçå­éæ¼ç1æ¡æ°æ® ### 1.4.9 è¡¥åéæ¼ç
+vtbç½ç« åè½åä¿¡æ¯ ### 1.4.10 æ°å¢åè½`vè¯¦æ` `dmkæ¥ç¨æ·`
 `dmkæ¥ç´æ­`ï¼ç´æ¥éç¨æµè§å¨é¡µé¢æªå¾å½¢å¼è¿åç»æãï¼æµéæ¶èä¼å¤ä¸äºï¼éæä½¿ç¨ï¼
-\n\n### 1.4.11\nå»¶é¿`vè¯¦æ` `dmkæ¥ç¨æ·`
+### 1.4.11 å»¶é¿`vè¯¦æ` `dmkæ¥ç¨æ·`
 `dmkæ¥ç´æ­`çè¯·æ±è¶æ¶è³5minï¼æå¡å¨4Mè·ä¹è¶æ¶ï¼åè½å¾åç´§ï¼
-\n\n###
-1.4.12\nè¿½å ææ°çvtbs.moeçä¸»æ­ä¿¡æ¯ï¼å¹¶åæ­¥æ´æ°äºçå­ä¿¡æ¯ã
-\nç¼©ç­`vè¯¦æ` `dmkæ¥ç¨æ·`
-`dmkæ¥ç´æ­`çè¯·æ±è¶æ¶è³2minï¼åé¢æ¯å¯¹é¢æå¡å¨ç¸äºï¼
-\n\n###
-1.4.13\nä¼åè¯·æ±éè¯¯ææ æ°æ®æ¶çæ¶æ¯è¿ååæ¥å¿æå°ã
-\n\n### 1.5.0\næ°å¢åè½`blgæ¥å¼¹å¹` `blgæ¥å¥åº` `blgæ¥ç¤¼ç©`
+### 1.4.12
+è¿½å ææ°çvtbs.moeçä¸»æ­ä¿¡æ¯ï¼å¹¶åæ­¥æ´æ°äºçå­ä¿¡æ¯ã
+ç¼©ç­`vè¯¦æ` `dmkæ¥ç¨æ·`
+`dmkæ¥ç´æ­`çè¯·æ±è¶æ¶è³2minï¼åé¢æ¯å¯¹é¢æå¡å¨ç¸äºï¼ ###
+1.4.13 ä¼åè¯·æ±éè¯¯ææ æ°æ®æ¶çæ¶æ¯è¿ååæ¥å¿æå°ã ###
+1.5.0 æ°å¢åè½`blgæ¥å¼¹å¹` `blgæ¥å¥åº` `blgæ¥ç¤¼ç©`
 `blgç´æ­è®°å½`
 `blgç´æ­é´sc`ï¼ç´æ¥éç¨æµè§å¨é¡µé¢æªå¾å½¢å¼è¿åç»æãï¼æµéæ¶èä¼å¤ä¸äºï¼éæä½¿ç¨ï¼
-\n\n### 1.5.1\næ°å¢4000+çç¨æ·æ°æ®åçå­æ°æ® \n\n###
-1.5.2\næ°å¢bç«ç¨æ·æ°æ®è³10w \næ°å¢ç²ä¸çæ°æ®è³4w+ \n\n###
-1.5.3\næ°å¢ç½ç«laplace.live
-\næ°å¢`icuæ¥ç´æ­`å½ä»¤ï¼åæ ·æ¯playwrightçç´æ¥å è½½ \n\n###
-1.5.4\næ°ç¨æ·æ°æ®ç¬èªbç«ç´æ­é´åå¤§ååºåè¡¨ï¼æ¯èµ·ç´æ¥uidç¬å¨ç«æ´å·æéå¯¹æ§ï¼å®éææä¹å¾å¥½ã
-\næ°å¢bç«ç¨æ·æ°æ®è³23w+ \næ°å¢ç²ä¸çæ°æ®è³6.7w+ \n\n###
-1.5.5\nç±äºåºç°ä½éç½®è®¾å¤åå­ä¸è¶³å¯¼è´çæ æ³å¯å¨é®é¢ï¼å·²å°æ¬å°æ°æ®`data.py`æ¸ç©ºè³ä¸ä¸ªdemoéç½®ãå¦ææ¬å°éç½®éè¦çå¯ä»¥å»æ§çè·åã
-\n\n###
-1.5.6\næ°å¢ç²ä¸çæ°æ®è³8.6w+ï¼ç¬äºä¸å¨çç´æ­é¡µï¼æ­£å¼æ¶å·¥ã
-\n\n###
-1.5.7\næ°å¢å½ä»¤`æ¥äººæ°`ï¼ç¨äºæ¥è¯¢bç«ä¸»æ­æè¿ä¸åºç´æ­çäººæ°å³°å¼
-\n\n###
-1.5.8\næ°å¢`lapæ¥ç¨æ·`å½ä»¤ï¼åæ ·æ¯playwrightï¼å¹¶åäºjsååµ
-\n\n###
-1.5.9\nä¼å`lapæ¥ç¨æ·`çåå®¹å è½½æ ·å¼ï¼æ¾ç¤ºåå®¹æ´å å¨é¢ï¼ä¹æ´å¡ï¼ä¹ï¼
-\n\n###
-1.5.10\nå¢å èæ¶çç½é¡µæªå¾æ¥è¯¢åé¦ï¼ä¼åå¼å¸¸å¤çï¼ä¸è®©ä½ çäººçæµªè´¹å¨ç­å¾ä¸­
-\n\n### 1.5.11\næ°å¢`zeroæ¥ç¨æ·`å½ä»¤ï¼åç \n\n###
-1.5.12\nä¿®å¤ææ¡£æè¿°éè¯¯ï¼ä¸å½±ååè½ï¼æä¸åçï¼
-\nææ¡£æ°å¢ç®å½ \n\n###
-1.5.13\næ°å¢`lapæ¥çå­`å½ä»¤ï¼è°ç¨laplace.liveçæ¥å£ï¼å¨ç«å¤ªå¡äºï¼ç»·
-\n\n###
-1.5.14\nä¿®å¤`lapæ¥çå­`æ¥å£è¿åuidåºå®é®é¢å¯¼è´çæ¾ç¤ºéè¯¯
-\nä¼åææ¡£ \n\n### 1.5.15\nåçº§`æ¥è§ç`åè½ï¼ç»è®¡è§çæ¬¡æ°ã
-\n\n###
-1.5.16\næ°å¢`æ¥è§ç2`å½ä»¤ï¼æ¥è§çplusçï¼ï¼ç»è®¡è§çæ¬¡æ°ï¼ä»¥é¥¼å¾å½¢å¼è¿åã
-\n\n###
-1.5.17\nä¼åç½é¡µæªå¾ç¸å³åè½çå¾çå­å¨åï¼åå°ç­æ¶é´å¤è¯·æ±å¯¼è´çæ°æ®è¦çé®é¢
-\nä¿®å¤`æ¥è§ç2`çæç¤ºè¯­å»¶è¿é®é¢ \nä¿®è®¢ææ¡£éè¯¯ \n\n###
-1.5.18\næ°å¢`lapæ¥åçµ`å½ä»¤ï¼æ¥è¯¢upçåçµæè¡æ¦ã
-\næ°å¢`zeroè¢«å³æ³¨`å½ä»¤ï¼æ¥è¯¢ç¨æ·çè¢«åªäºç¥åupä¸»å³æ³¨ã
-\nåçº§`æ¥è§ç2`çä¸»é¢ä¸ºå¤é´æ¨¡å¼ï¼å¢å é«çº§æã \n\n###
-1.6.0\nå¯¹ç±»ä¼¼çGETè¯·æ±åäºä¼åï¼éä½ä»£ç åä½ã \n\n###
-1.6.1\nå é¤`lapæ¥ç¨æ·`çå°ä½æ \n\n###
-1.6.2\n1ãæ°å¢ä»¥ä¸å½ä»¤ï¼ \n- /vç´æ­å¿ ï¼å¤§åä¹å¯ä»¥ï¼\n- /
-væ¥ä¸å ï¼å¤§åä¹å¯ä»¥ï¼\n- /væ¥ä¸é ï¼å¤§åä¹å¯ä»¥ï¼\n- /
-vè°å¢ ï¼å¤§åä¹å¯ä»¥ï¼\n- /vdd ï¼å¤§åä¹å¯ä»¥ï¼\n- /vå®è§
-ï¼å¤§åä¹å¯ä»¥ï¼ \n2ãä¼åå¼å¸¸å¤ç\n\n###
-1.6.3\nä¼å`vè¯¦æ`çè¯·æ±å»¶æ¶ï¼å¸®å©æ°æ®å è½½ã \n\n###
-1.6.4\næ°å¢`æ¥è£æ®`å½ä»¤ã \nä¼åææ¡£æåºã \n\n###
-1.6.5\n1.`vè¯¦æ`å¢å å«å`vè¯¦ç»`ã \n2.ä¿®å¤`æ¥æ¶ç`çä¼ åbugã
-\n3.ä¼åä»£ç å®ç°ï¼å¢å æç¤ºäºå¨ã \n\n###
-1.6.6\n1.ä¿®å¤`æ¥å¼¹å¹`å`æ¥å¼¹å¹2`çbugï¼è®©GPTå¸®å¿åï¼å¾å¥½ï¼bugåå¾ä¸éï¼
-\n\n### 1.6.7\n1.å½ä»¤ææ¬æ¶æ¯åå®¹æ¹è¾ç¹ä¸ºåå¤ã
-\n2.æ°å¢å½ä»¤`lapdd`æ`lapddæè¡æ¦`ï¼æªå¾laplace.liveçddé¡µé¢ã
-\n3.ä¼åè¯´æææ¡£ã \n\n### 1.6.8\nä¿®å¤`lapdd`å½ä»¤ä¸ä¼ åçbugã
-\n\n### 1.6.9\næ°å¢æ­£åå¹éç`æè«`ç©æ³ï¼å·ä½çå½ä»¤è¯´æã
-\n\n### 1.7.0\nä¿®å¤htmlrenderå¯¼å¥é®é¢ã \n\n###
-1.7.1\næ°å¢å½ä»¤`ehæ¥ç´æ­`æ`è¯¶å¿æ¥ç´æ­`ã \n\n###
-1.7.2\nä¿®æ¹`ehæ¥ç´æ­`çè¯·æ±å°åä¸ºhttpï¼æå¡å¨ä¸è·è¯ä¹¦ä¸è¡ï¼ç»·ã
-\n\n### 1.7.3\nä¿®æ¹`ehæ¥ç´æ­`ä¸ºplaywrightï¼é¾ç»·ã \n\n###
-1.7.4\nä¿®æ¹`ehæ¥ç´æ­`ä¸ºç´æ¥è¯·æ±ï¼ä¸è¿è·³è¿äºsslã \n\n###
-1.7.5\nbugä¿®å¤ \n\n###
-1.7.6\n`æ¥`å½ä»¤ï¼è¿½å è¿åç¨æ·ä¸»é¡µåç´æ­é´é¾æ¥ã \n\n\n\n##
-è´è°¢\n- [nonebot-plugin-htmlrender](https://github.com/kexue-z/nonebot-
-plugin-htmlrender) - å¾çåæçå¥½æ\n- [danmakus.com](https://
-danmakus.com/) -
-bç«ä¸»æ­ãç¨æ·å¼¹å¹ç´æ­ä¿¡æ¯ç­æ¥æºï¼å¼æ¾APIæ¥å£å¾èµï¼ï¼\n-
+### 1.5.1 æ°å¢4000+çç¨æ·æ°æ®åçå­æ°æ® ### 1.5.2
+æ°å¢bç«ç¨æ·æ°æ®è³10w æ°å¢ç²ä¸çæ°æ®è³4w+ ### 1.5.3
+æ°å¢ç½ç«laplace.live
+æ°å¢`icuæ¥ç´æ­`å½ä»¤ï¼åæ ·æ¯playwrightçç´æ¥å è½½ ### 1.5.4
+æ°ç¨æ·æ°æ®ç¬èªbç«ç´æ­é´åå¤§ååºåè¡¨ï¼æ¯èµ·ç´æ¥uidç¬å¨ç«æ´å·æéå¯¹æ§ï¼å®éææä¹å¾å¥½ã
+æ°å¢bç«ç¨æ·æ°æ®è³23w+ æ°å¢ç²ä¸çæ°æ®è³6.7w+ ### 1.5.5
+ç±äºåºç°ä½éç½®è®¾å¤åå­ä¸è¶³å¯¼è´çæ æ³å¯å¨é®é¢ï¼å·²å°æ¬å°æ°æ®`data.py`æ¸ç©ºè³ä¸ä¸ªdemoéç½®ãå¦ææ¬å°éç½®éè¦çå¯ä»¥å»æ§çè·åã
+### 1.5.6
+æ°å¢ç²ä¸çæ°æ®è³8.6w+ï¼ç¬äºä¸å¨çç´æ­é¡µï¼æ­£å¼æ¶å·¥ã ###
+1.5.7
+æ°å¢å½ä»¤`æ¥äººæ°`ï¼ç¨äºæ¥è¯¢bç«ä¸»æ­æè¿ä¸åºç´æ­çäººæ°å³°å¼
+### 1.5.8 æ°å¢`lapæ¥ç¨æ·`å½ä»¤ï¼åæ ·æ¯playwrightï¼å¹¶åäºjsååµ
+### 1.5.9
+ä¼å`lapæ¥ç¨æ·`çåå®¹å è½½æ ·å¼ï¼æ¾ç¤ºåå®¹æ´å å¨é¢ï¼ä¹æ´å¡ï¼ä¹ï¼
+### 1.5.10
+å¢å èæ¶çç½é¡µæªå¾æ¥è¯¢åé¦ï¼ä¼åå¼å¸¸å¤çï¼ä¸è®©ä½ çäººçæµªè´¹å¨ç­å¾ä¸­
+### 1.5.11 æ°å¢`zeroæ¥ç¨æ·`å½ä»¤ï¼åç ### 1.5.12
+ä¿®å¤ææ¡£æè¿°éè¯¯ï¼ä¸å½±ååè½ï¼æä¸åçï¼ ææ¡£æ°å¢ç®å½
+### 1.5.13
+æ°å¢`lapæ¥çå­`å½ä»¤ï¼è°ç¨laplace.liveçæ¥å£ï¼å¨ç«å¤ªå¡äºï¼ç»·
+### 1.5.14 ä¿®å¤`lapæ¥çå­`æ¥å£è¿åuidåºå®é®é¢å¯¼è´çæ¾ç¤ºéè¯¯
+ä¼åææ¡£ ### 1.5.15 åçº§`æ¥è§ç`åè½ï¼ç»è®¡è§çæ¬¡æ°ã ###
+1.5.16
+æ°å¢`æ¥è§ç2`å½ä»¤ï¼æ¥è§çplusçï¼ï¼ç»è®¡è§çæ¬¡æ°ï¼ä»¥é¥¼å¾å½¢å¼è¿åã
+### 1.5.17
+ä¼åç½é¡µæªå¾ç¸å³åè½çå¾çå­å¨åï¼åå°ç­æ¶é´å¤è¯·æ±å¯¼è´çæ°æ®è¦çé®é¢
+ä¿®å¤`æ¥è§ç2`çæç¤ºè¯­å»¶è¿é®é¢ ä¿®è®¢ææ¡£éè¯¯ ### 1.5.18
+æ°å¢`lapæ¥åçµ`å½ä»¤ï¼æ¥è¯¢upçåçµæè¡æ¦ã
+æ°å¢`zeroè¢«å³æ³¨`å½ä»¤ï¼æ¥è¯¢ç¨æ·çè¢«åªäºç¥åupä¸»å³æ³¨ã
+åçº§`æ¥è§ç2`çä¸»é¢ä¸ºå¤é´æ¨¡å¼ï¼å¢å é«çº§æã ### 1.6.0
+å¯¹ç±»ä¼¼çGETè¯·æ±åäºä¼åï¼éä½ä»£ç åä½ã ### 1.6.1
+å é¤`lapæ¥ç¨æ·`çå°ä½æ ### 1.6.2 1ãæ°å¢ä»¥ä¸å½ä»¤ï¼ - /
+vç´æ­å¿ ï¼å¤§åä¹å¯ä»¥ï¼ - /væ¥ä¸å ï¼å¤§åä¹å¯ä»¥ï¼ - /
+væ¥ä¸é ï¼å¤§åä¹å¯ä»¥ï¼ - /vè°å¢ ï¼å¤§åä¹å¯ä»¥ï¼ - /vdd
+ï¼å¤§åä¹å¯ä»¥ï¼ - /vå®è§ ï¼å¤§åä¹å¯ä»¥ï¼ 2ãä¼åå¼å¸¸å¤ç
+### 1.6.3 ä¼å`vè¯¦æ`çè¯·æ±å»¶æ¶ï¼å¸®å©æ°æ®å è½½ã ### 1.6.4
+æ°å¢`æ¥è£æ®`å½ä»¤ã ä¼åææ¡£æåºã ### 1.6.5
+1.`vè¯¦æ`å¢å å«å`vè¯¦ç»`ã 2.ä¿®å¤`æ¥æ¶ç`çä¼ åbugã
+3.ä¼åä»£ç å®ç°ï¼å¢å æç¤ºäºå¨ã ### 1.6.6
+1.ä¿®å¤`æ¥å¼¹å¹`å`æ¥å¼¹å¹2`çbugï¼è®©GPTå¸®å¿åï¼å¾å¥½ï¼bugåå¾ä¸éï¼
+### 1.6.7 1.å½ä»¤ææ¬æ¶æ¯åå®¹æ¹è¾ç¹ä¸ºåå¤ã
+2.æ°å¢å½ä»¤`lapdd`æ`lapddæè¡æ¦`ï¼æªå¾laplace.liveçddé¡µé¢ã
+3.ä¼åè¯´æææ¡£ã ### 1.6.8 ä¿®å¤`lapdd`å½ä»¤ä¸ä¼ åçbugã ###
+1.6.9 æ°å¢æ­£åå¹éç`æè«`ç©æ³ï¼å·ä½çå½ä»¤è¯´æã ### 1.7.0
+ä¿®å¤htmlrenderå¯¼å¥é®é¢ã ### 1.7.1
+æ°å¢å½ä»¤`ehæ¥ç´æ­`æ`è¯¶å¿æ¥ç´æ­`ã ### 1.7.2
+ä¿®æ¹`ehæ¥ç´æ­`çè¯·æ±å°åä¸ºhttpï¼æå¡å¨ä¸è·è¯ä¹¦ä¸è¡ï¼ç»·ã
+### 1.7.3 ä¿®æ¹`ehæ¥ç´æ­`ä¸ºplaywrightï¼é¾ç»·ã ### 1.7.4
+ä¿®æ¹`ehæ¥ç´æ­`ä¸ºç´æ¥è¯·æ±ï¼ä¸è¿è·³è¿äºsslã ### 1.7.5 bugä¿®å¤
+### 1.7.6 `æ¥`å½ä»¤ï¼è¿½å è¿åç¨æ·ä¸»é¡µåç´æ­é´é¾æ¥ã ### 1.7.7
+æ°å¢`dmkåæ`åè½ï¼ç±danmakusåæç¨æ·è§çå¼¹å¹ç­æ°æ®ã  ##
+è´è°¢ - [nonebot-plugin-htmlrender](https://github.com/kexue-z/nonebot-plugin-
+htmlrender) - å¾çåæçå¥½æ - [danmakus.com](https://danmakus.com/) -
+bç«ä¸»æ­ãç¨æ·å¼¹å¹ç´æ­ä¿¡æ¯ç­æ¥æºï¼å¼æ¾APIæ¥å£å¾èµï¼ï¼ -
 [vtbs.moe](https://vtbs.moe) -
-VTBæ¬å°æ°æ®ä¿¡æ¯æ¥æºï¼è¿ææ°æ®æä¾ï¼TQLï¼ \n- [laplace.live]
+VTBæ¬å°æ°æ®ä¿¡æ¯æ¥æºï¼è¿ææ°æ®æä¾ï¼TQLï¼ - [laplace.live]
 (https://laplace.live/) -
 ä¹æ¯bç«ä¸»æ­ç¨æ·æ¥è¯¢ç«ç¹ï¼é¨åæ°æ®ä¹æ¯æºèªdanmakusï¼UIä¸é
-\n\n## é¡¹ç®æåä¸ä¼ è³pypi\n\nå®ç½ï¼https://
+## é¡¹ç®æåä¸ä¼ è³pypi å®ç½ï¼https://
 pypi.orgï¼æ³¨åè´¦å·ï¼å¨ç³»ç»ç¨æ·æ ¹ç®å½ä¸åå»º`.pypirc`ï¼éç½®
-\n``` \n[distutils] \nindex-servers=pypi \n \n[pypi] repository = https://
-upload.pypi.org/legacy/ \nusername = ç¨æ·å \npassword = å¯ç \n```\n\n###
-poetry\n\n```\n# åè https://www.freesion.com/article/58051228882/\n\n#
-1ãå®è£poetry\npip install poetry\n\n#
-2ãåå§åéç½®æä»¶ï¼æ ¹æ®æç¤ºå¡«åï¼\npoetry init\n\n#
-3ãå¾®è°éç½®æä»¶pyproject.toml\n\n# 4ãè¿è¡ poetry install, å¯çæ
-âpoetry.lockâ æä»¶ï¼å¯è·³è¿ï¼\npoetry install\n\n#
-5ãç¼è¯ï¼çædist\npoetry build\n\n# 6ãåå¸\npoetry
-publish\n\n```\n\n### twine\n\n```\n# åè https://www.cnblogs.com/danhuai/p/
-14915042.html\n#åå»ºsetup.pyæä»¶ å¡«åç¸å³ä¿¡æ¯\n\n#
-1ãå¯ä»¥ååçº§æåå·¥å·\npip install --upgrade setuptools wheel
-twine\n\n# 2ãæå\npython setup.py sdist bdist_wheel\n\n#
-3ãå¯ä»¥åæ£æ¥ä¸ä¸å\ntwine check dist/*\n\n#
-4ãä¸ä¼ åå°pypiï¼éè¾å¥ç¨æ·åãå¯ç ï¼\ntwine upload dist/
-*\n```\n\n## ç®å½èªå¨çæ\n\n[doctoc](https://github.com/thlorenz/
-doctoc),å¨æ¬å°gitå­å¨åºä¸­çæéä»·æä»¶çç®å½ãé¾æ¥éè¿å½ä»¤è¡æ å¿å¼å®¹githubæå¶ä»ç½ç«çæçéã\n\n###
-å®è£\nè¿å¥åå«æ¬å°gité¡¹ç®çç®å½ï¼é®å¥: `npm install -g doctoc`
-\n\n###
-ä½¿ç¨\nå¨`README.md`ä¸­ï¼æ¾ä¸ªçæç®å½ä½ç½®ï¼åå¥å¦ä¸ä»£ç ï¼ç¡®è®¤çæä½ç½®ï¼\n```\n\n\n```\ncmdè¾å¥å½ä»¤å³å¯ï¼`doctoc
-/path/to/file` \nä¾å¦ï¼`doctoc README.md` \n\n', 'author': 'Ikaros',
-'author_email': '327209194@qq.com', 'maintainer': 'None', 'maintainer_email':
-'None', 'url': 'https://github.com/Ikaros-521/nonebot_plugin_searchBiliInfo',
-'packages': packages, 'package_data': package_data, 'install_requires':
-install_requires, 'python_requires': '>=3.8,<4.0', } setup(**setup_kwargs)
+``` [distutils] index-servers=pypi [pypi] repository = https://upload.pypi.org/
+legacy/ username = ç¨æ·å password = å¯ç  ``` ### poetry ``` # åè
+https://www.freesion.com/article/58051228882/ # 1ãå®è£poetry pip install
+poetry # 2ãåå§åéç½®æä»¶ï¼æ ¹æ®æç¤ºå¡«åï¼ poetry init #
+3ãå¾®è°éç½®æä»¶pyproject.toml # 4ãè¿è¡ poetry install, å¯çæ
+âpoetry.lockâ æä»¶ï¼å¯è·³è¿ï¼ poetry install #
+5ãç¼è¯ï¼çædist poetry build # 6ãåå¸ poetry publish ``` ### twine
+``` # åè https://www.cnblogs.com/danhuai/p/14915042.html
+#åå»ºsetup.pyæä»¶ å¡«åç¸å³ä¿¡æ¯ # 1ãå¯ä»¥ååçº§æåå·¥å· pip
+install --upgrade setuptools wheel twine # 2ãæå python setup.py sdist
+bdist_wheel # 3ãå¯ä»¥åæ£æ¥ä¸ä¸å twine check dist/* #
+4ãä¸ä¼ åå°pypiï¼éè¾å¥ç¨æ·åãå¯ç ï¼ twine upload dist/* ```
+## ç®å½èªå¨çæ [doctoc](https://github.com/thlorenz/
+doctoc),å¨æ¬å°gitå­å¨åºä¸­çæéä»·æä»¶çç®å½ãé¾æ¥éè¿å½ä»¤è¡æ å¿å¼å®¹githubæå¶ä»ç½ç«çæçéã
+### å®è£ è¿å¥åå«æ¬å°gité¡¹ç®çç®å½ï¼é®å¥: `npm install -
+g doctoc` ### ä½¿ç¨
+å¨`README.md`ä¸­ï¼æ¾ä¸ªçæç®å½ä½ç½®ï¼åå¥å¦ä¸ä»£ç ï¼ç¡®è®¤çæä½ç½®ï¼
+```   ``` cmdè¾å¥å½ä»¤å³å¯ï¼`doctoc /path/to/file` ä¾å¦ï¼`doctoc
+README.md`
```

