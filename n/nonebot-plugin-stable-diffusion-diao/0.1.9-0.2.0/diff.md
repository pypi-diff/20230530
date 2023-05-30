# Comparing `tmp/nonebot_plugin_stable_diffusion_diao-0.1.9.tar.gz` & `tmp/nonebot_plugin_stable_diffusion_diao-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.1.9.tar", last modified: Sun May 28 16:45:17 2023, max compression
+gzip compressed data, was "nonebot_plugin_stable_diffusion_diao-0.2.0.tar", last modified: Tue May 30 15:38:02 2023, max compression
```

## Comparing `nonebot_plugin_stable_diffusion_diao-0.1.9.tar` & `nonebot_plugin_stable_diffusion_diao-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.1.9/LICENSE
--rw-r--r--   0        0        0      686 2023-05-28 09:58:15.400842 nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/__init__.py
--rw-r--r--   0        0        0    18654 2023-05-28 09:58:15.401369 nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/aidraw.py
--rw-r--r--   0        0        0     6100 2023-05-28 12:48:55.161779 nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
--rw-r--r--   0        0        0    65592 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
--rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
--rw-r--r--   0        0        0    15370 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/backend/base.py
--rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
--rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
--rw-r--r--   0        0        0     6321 2023-05-28 09:58:15.405664 nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/backend/sd.py
--rw-r--r--   0        0        0    13617 2023-05-28 11:28:54.486210 nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/config.py
--rw-r--r--   0        0        0     9282 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
--rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
--rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
--rw-r--r--   0        0        0     1328 2023-05-28 09:58:15.407673 nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
--rw-r--r--   0        0        0     3751 2023-05-28 09:58:15.407673 nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
--rw-r--r--   0        0        0    11304 2023-05-28 09:58:15.407673 nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
--rw-r--r--   0        0        0     3668 2023-05-28 12:10:58.511567 nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
--rw-r--r--   0        0        0    28671 2023-05-28 16:27:22.765742 nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
--rw-r--r--   0        0        0     5964 2023-05-28 09:58:15.408672 nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/extension/translation.py
--rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/fifo.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/locales/en.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/locales/jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
--rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/locales/zh.py
--rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/manage.py
--rw-r--r--   0        0        0     1479 2023-05-28 09:58:15.412189 nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
--rw-r--r--   0        0        0     2314 2023-05-28 09:58:15.412189 nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/utils/data.py
--rw-r--r--   0        0        0     7541 2023-05-28 16:44:38.599239 nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
--rw-r--r--   0        0        0      647 2023-05-28 09:58:15.413187 nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
--rw-r--r--   0        0        0      727 2023-05-28 09:58:15.413187 nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/utils/save.py
--rw-r--r--   0        0        0     1994 2023-05-28 09:58:15.414188 nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/version.py
--rw-r--r--   0        0        0      701 2023-05-28 16:45:17.850098 nonebot_plugin_stable_diffusion_diao-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-05-28 09:58:15.375966 nonebot_plugin_stable_diffusion_diao-0.2.0/LICENSE
+-rw-r--r--   0        0        0      686 2023-05-28 09:58:15.400842 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/__init__.py
+-rw-r--r--   0        0        0    18654 2023-05-28 09:58:15.401369 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/aidraw.py
+-rw-r--r--   0        0        0     6100 2023-05-28 12:48:55.161779 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402430 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/amusement/ramdomgirl.py
+-rw-r--r--   0        0        0    65592 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py
+-rw-r--r--   0        0        0     2528 2023-05-30 15:35:38.313378 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/amusement/vits.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.402952 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/amusement/wordbank.py
+-rw-r--r--   0        0        0      699 2023-05-28 09:58:15.404033 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/backend/__init__.py
+-rw-r--r--   0        0        0    15349 2023-05-30 14:20:07.688799 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/backend/base.py
+-rw-r--r--   0        0        0     1279 2023-05-28 09:58:15.404557 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/backend/naifu.py
+-rw-r--r--   0        0        0     1659 2023-05-28 09:58:15.405158 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/backend/novelai.py
+-rw-r--r--   0        0        0     6300 2023-05-30 15:28:12.457021 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/backend/sd.py
+-rw-r--r--   0        0        0    13644 2023-05-30 14:02:44.198727 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/config.py
+-rw-r--r--   0        0        0     9282 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py
+-rw-r--r--   0        0        0     3340 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/extension/anlas.py
+-rw-r--r--   0        0        0     1935 2023-05-28 09:58:15.406675 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/extension/control_net.py
+-rw-r--r--   0        0        0     1449 2023-05-30 13:50:33.328475 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py
+-rw-r--r--   0        0        0     3751 2023-05-28 09:58:15.407673 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py
+-rw-r--r--   0        0        0    11882 2023-05-30 15:32:52.299649 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py
+-rw-r--r--   0        0        0     3668 2023-05-28 12:10:58.511567 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py
+-rw-r--r--   0        0        0    28671 2023-05-28 16:27:22.765742 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py
+-rw-r--r--   0        0        0     5964 2023-05-28 09:58:15.408672 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/extension/translation.py
+-rw-r--r--   0        0        0      400 2023-05-28 09:58:15.409671 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/fifo.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/locales/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/locales/en.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/locales/jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.410176 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/locales/moe_jp.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/locales/moe_zh.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/locales/zh.py
+-rw-r--r--   0        0        0     1905 2023-05-28 09:58:15.411183 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/manage.py
+-rw-r--r--   0        0        0     1479 2023-05-28 09:58:15.412189 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/utils/__init__.py
+-rw-r--r--   0        0        0     2314 2023-05-28 09:58:15.412189 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/utils/data.py
+-rw-r--r--   0        0        0     7499 2023-05-30 15:27:52.695256 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py
+-rw-r--r--   0        0        0      647 2023-05-28 09:58:15.413187 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py
+-rw-r--r--   0        0        0      727 2023-05-28 09:58:15.413187 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/utils/save.py
+-rw-r--r--   0        0        0     1994 2023-05-28 09:58:15.414188 nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/version.py
+-rw-r--r--   0        0        0      701 2023-05-30 15:38:02.449721 nonebot_plugin_stable_diffusion_diao-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      442 1970-01-01 00:00:00.000000 nonebot_plugin_stable_diffusion_diao-0.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.9/LICENSE` & `nonebot_plugin_stable_diffusion_diao-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/aidraw.py` & `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/aidraw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py` & `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/amusement/chatgpt_tagger.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py` & `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/amusement/today_girl.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/backend/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/backend/base.py` & `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/backend/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,16 +270,16 @@
                 tmp_history_list.append({self.start_time: spend_time})
                 tc = self.backend_info[self.backend_site][self.task_type]["info"]["tasks_count"]
                 tc -= 1
                 self.backend_info[self.backend_site][self.task_type]["info"]["tasks_count"] = tc
                 cur_status = "idel" if tc == 0 else self.task_type
                 self.backend_info["status"] = cur_status
                 self.backend_info[self.backend_site][self.task_type]["info"]["history"] = tmp_history_list
-                async with aiofiles.open("data/novelai/load_balance.json", "w") as f:
-                    await f.write(json.dumps(self.backend_info))
+                with open("data/novelai/load_balance.json", "w") as f:
+                    f.write(json.dumps(self.backend_info))
                 img = await self.fromresp(resp)
                 logger.debug(f"获取到返回图片，正在处理")
                 # 将图片转化为jpg
                 if config.novelai_save == 1:
                     image_new = await png2jpg(img)
                 else:
                     image_new = base64.b64decode(img)
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/backend/naifu.py` & `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/backend/naifu.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/backend/novelai.py` & `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/backend/novelai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/backend/sd.py` & `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/backend/sd.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,16 +97,16 @@
                 parameters.update(config.novelai_ControlNet_payload[1])
                 parameters["controlnet_units"][0]["input_image"] = self.image           
         return header, post_api, parameters
 
     async def post(self):
         global defult_site
         defult_site = None # 所有后端失效后, 尝试使用默认后端
-        async with aiofiles.open("data/novelai/load_balance.json", "r", encoding="utf-8") as f:
-            content = await f.read()
+        with open("data/novelai/load_balance.json", "r", encoding="utf-8") as f:
+            content = f.read()
             self.backend_info = json.loads(content)
         # 失效自动重试 
         for retry_times in range(config.novelai_retry):
             try:
                 self.start_time = time.time()
                 parameters_tuple = await self.post_parameters()
                 await self.post_(*parameters_tuple)
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/config.py` & `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,15 @@
     novelai_extra_pic_audit = False # 是否为二次元的我, chatgpt生成tag等功能添加审核功能
     # 翻译API设置
     bing_key: str = None  # bing的翻译key
     deepl_key: str = None  # deepL的翻译key
     baidu_translate_key: dict = None # 例:{"SECRET_KEY": "", "API_KEY": ""} # https://console.bce.baidu.com/ai/?_=1685076516634#/ai/machinetranslation/overview/index
     novelai_todaygirl = 1 # 可选值 1 和 2 两种不同的方式
     novelai_tagger_site: str = None # 分析功能的地址 例如 127.0.0.1:7860
+    vits_site: str = None
 
     # 允许单群设置的设置
     def keys(cls):
         return ("novelai_cd", "novelai_tags", "novelai_on", "novelai_ntags", "novelai_revoke", "novelai_h", "novelai_htype", "novelai_picaudit", "novelai_pure", "novelai_site")
 
     def __getitem__(cls, item):
         return getattr(cls, item)
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py` & `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/extension/aidraw_help.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/extension/anlas.py` & `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/extension/anlas.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/extension/control_net.py` & `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/extension/control_net.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py` & `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/extension/daylimit.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,40 +4,41 @@
 from ..config import config
 import aiofiles
 
 
 class DayLimit():
     filename = "data/novelai/day_limit_data.json"
     day: int = time.localtime(time.time()).tm_yday
+    json_data = {"date": day, "count": {}}
+    data = json_data["count"]
     if os.path.exists(filename):
         with open(filename, "r") as file:
             content = file.read()
-            data: dict = json.loads(content)
-    else:
-        data = {}
-
-    @classmethod
-    async def load_data(cls):
-        filename = "data/novelai/day_limit_data.json"
-        async with aiofiles.open(filename, "r") as file:
-            content = await file.read()
-        return json.loads(content)
+            json_data: dict = json.loads(content)
+            try:
+                data = json_data["count"]
+            except KeyError:
+                json_data = {"date": day, "count": {}}
+                data = {}
+        if json_data["date"] != day:
+            json_data = {"date": day, "count": {}}
+            data = json_data["count"]
 
     @classmethod
     async def save_data(cls):
-        filename = "data/novelai/day_limit_data.json"
-        async with aiofiles.open(filename, "w") as file:
-            await file.write(json.dumps(cls.data))
+        async with aiofiles.open(cls.filename, "w") as file:
+            cls.json_data["count"] = cls.data
+            await file.write(json.dumps(cls.json_data))
 
     @classmethod
     async def count(cls, user: str, num):
-        day_ = time.localtime(time.time()).tm_yday
-        if day_ != cls.day:
-            cls.day = day_
-            cls.data = await cls.load_data()
+        # day_ = time.localtime(time.time()).tm_yday
+        # if day_ != cls.day:
+        #     cls.day = day_
+        #     cls.data = await cls.load_data()
         count: int = cls.data.get(user, 0) + num
         if count > config.novelai_daylimit:
             return -1
         else:
             cls.data[user] = count
             await cls.save_data()
             return config.novelai_daylimit - count
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py` & `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/extension/deepdanbooru.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py` & `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/extension/explicit_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import base64
 import aiohttp, aiofiles
 import nonebot
 import os
 import urllib
 import re
 from PIL import Image
-from nonebot.adapters.onebot.v11 import MessageSegment, Bot, GroupMessageEvent, ActionFailed
+from nonebot.adapters.onebot.v11 import MessageSegment, Bot, GroupMessageEvent, ActionFailed, PrivateMessageEvent
 from nonebot.log import logger
 from ..config import config 
 import qrcode
 import time
 
 
 async def send_qr_code(bot, fifo, img_url):
@@ -41,14 +41,26 @@
     raw_message = f"\n{nickname}已经"
     label = ""
     # 判读是否进行图片审核
     h = await config.get_value(fifo.group_id, "h")
     nsfw_count = 0
     for i in img_bytes:
         # try:
+        if isinstance(fifo.event, PrivateMessageEvent):
+            if config.novelai_SuperRes_generate:
+                try:
+                    from ..extension.sd_extra_api_func import super_res_api_func
+                    resp_tuple = await super_res_api_func(i, 3)
+                    i = resp_tuple[0]
+                except:
+                    logger.debug("超分API失效")
+            if save_img_:
+                await save_img(fifo, i, fifo.group_id)
+            message.append(MessageSegment.image(i))
+            return message
         if await config.get_value(fifo.group_id, "picaudit") in [1, 2, 4] or config.novelai_picaudit in [1, 2, 4]:
             try:
                 label, h_value = await check_safe(i, fifo)
             except RuntimeError as e:
                 logger.error(f"NSFWAPI调用失败，错误代码为{e.args}")
                 label = "unknown"
             if label in ["safe", "general", "sensitive"]:
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py` & `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/extension/safe_method.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py` & `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/extension/sd_extra_api_func.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/extension/translation.py` & `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/extension/translation.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/manage.py` & `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/manage.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/utils/__init__.py` & `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/utils/data.py` & `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/utils/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py` & `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/utils/load_balance.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,16 +93,16 @@
 
 async def sd_LoadBalance(addtional_site=None, task_counts=None, task_type=None, state_dict=None):
     '''
     分别返回可用后端索引, 后端对应ip和名称(元组), 显存占用
     '''
     backend_url_dict = config.novelai_backend_url_dict
     if state_dict is None:
-        async with aiofiles.open("data/novelai/load_balance.json", "r", encoding="utf-8") as f:
-            content = await f.read()
+        with open("data/novelai/load_balance.json", "r", encoding="utf-8") as f:
+            content = f.read()
             state_dict = json.loads(content)
     else:
         pass
     if addtional_site:
         backend_url_dict.update({"群专属后端": f"{addtional_site}"})
     reverse_dict = {value: key for key, value in backend_url_dict.items()}
     tasks = []
@@ -161,12 +161,12 @@
 
     logger.info(f"已选择后端{ava_url}")
     tc = int(state_dict[ava_url][task_type]["info"]["tasks_count"])
     tc += 1
     state_dict[ava_url]["status"] = task_type
     state_dict[ava_url]["start_time"] = time.time()
     state_dict[ava_url][task_type]["info"]["tasks_count"] = tc
-    async with aiofiles.open("data/novelai/load_balance.json", "w", encoding="utf-8") as f:
-        await f.write(json.dumps(state_dict))
+    with open("data/novelai/load_balance.json", "w", encoding="utf-8") as f:
+        f.write(json.dumps(state_dict))
     ava_url_index = list(backend_url_dict.values()).index(ava_url)
     ava_url_tuple = (ava_url, reverse_dict[ava_url], all_resp, len(normal_backend))
     return ava_url_index, ava_url_tuple, normal_backend, state_dict
```

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py` & `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/utils/prepocess.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/utils/save.py` & `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/utils/save.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.9/nonebot_plugin_stable_diffusion_diao/version.py` & `nonebot_plugin_stable_diffusion_diao-0.2.0/nonebot_plugin_stable_diffusion_diao/version.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_stable_diffusion_diao-0.1.9/pyproject.toml` & `nonebot_plugin_stable_diffusion_diao-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-stable-diffusion-diao"
-version = "0.1.9"
+version = "0.2.0"
 description = "主要面对stable-diffusion-webui-api的nonebot2插件"
 authors = [
     { name = "DiaoDaiaChan", email = "diaodaiachan@qq.com" },
 ]
 dependencies = [
     "aiofiles>=23.1.0",
     "aiohttp>=3.8.4",
```

