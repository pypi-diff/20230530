# Comparing `tmp/gggdtparser-0.0.6.tar.gz` & `tmp/gggdtparser-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gggdtparser-0.0.6.tar", last modified: Tue Apr 11 07:58:51 2023, max compression
+gzip compressed data, was "gggdtparser-0.0.8.tar", last modified: Tue May 30 11:42:51 2023, max compression
```

## Comparing `gggdtparser-0.0.6.tar` & `gggdtparser-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 07:58:51.565783 gggdtparser-0.0.6/
--rw-rw-rw-   0        0        0     1088 2023-03-27 06:45:03.000000 gggdtparser-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     3404 2023-04-11 07:58:51.566780 gggdtparser-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2689 2023-04-10 04:20:03.000000 gggdtparser-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 07:58:51.560796 gggdtparser-0.0.6/gggdtparser/
--rw-rw-rw-   0        0        0      259 2023-03-28 10:39:47.000000 gggdtparser-0.0.6/gggdtparser/__init__.py
--rw-rw-rw-   0        0        0    12567 2023-04-11 07:54:36.000000 gggdtparser-0.0.6/gggdtparser/dtconfigs.py
--rw-rw-rw-   0        0        0    15812 2023-04-11 07:32:49.000000 gggdtparser-0.0.6/gggdtparser/dtparser.py
--rw-rw-rw-   0        0        0    41227 2023-04-11 06:55:56.000000 gggdtparser-0.0.6/gggdtparser/test.py
-drwxrwxrwx   0        0        0        0 2023-04-11 07:58:51.564786 gggdtparser-0.0.6/gggdtparser.egg-info/
--rw-rw-rw-   0        0        0     3404 2023-04-11 07:58:51.000000 gggdtparser-0.0.6/gggdtparser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-04-11 07:58:51.000000 gggdtparser-0.0.6/gggdtparser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 07:58:51.000000 gggdtparser-0.0.6/gggdtparser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-11 07:58:51.000000 gggdtparser-0.0.6/gggdtparser.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      775 2023-04-11 07:58:51.570961 gggdtparser-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      165 2023-03-27 07:16:57.000000 gggdtparser-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 11:42:51.316922 gggdtparser-0.0.8/
+-rw-rw-rw-   0        0        0     1088 2023-03-27 06:45:03.000000 gggdtparser-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     3404 2023-05-30 11:42:51.316922 gggdtparser-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2689 2023-04-10 04:20:03.000000 gggdtparser-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 11:42:51.265061 gggdtparser-0.0.8/gggdtparser/
+-rw-rw-rw-   0        0        0      227 2023-05-16 08:44:33.000000 gggdtparser-0.0.8/gggdtparser/__init__.py
+-rw-rw-rw-   0        0        0     2824 2023-05-30 08:08:48.000000 gggdtparser-0.0.8/gggdtparser/dtconfigs.py
+-rw-rw-rw-   0        0        0    17946 2023-05-30 06:56:51.000000 gggdtparser-0.0.8/gggdtparser/dtparser.py
+drwxrwxrwx   0        0        0        0 2023-05-30 11:42:51.299968 gggdtparser-0.0.8/gggdtparser/langs/
+-rw-rw-rw-   0        0        0       88 2023-04-20 07:19:51.000000 gggdtparser-0.0.8/gggdtparser/langs/__init__.py
+-rw-rw-rw-   0        0        0      235 2023-05-30 07:17:00.000000 gggdtparser-0.0.8/gggdtparser/langs/_id.py
+-rw-rw-rw-   0        0        0      246 2023-05-25 03:05:13.000000 gggdtparser-0.0.8/gggdtparser/langs/az.py
+-rw-rw-rw-   0        0        0      678 2023-05-25 03:05:13.000000 gggdtparser-0.0.8/gggdtparser/langs/de.py
+-rw-rw-rw-   0        0        0     4773 2023-05-30 07:53:40.000000 gggdtparser-0.0.8/gggdtparser/langs/default.py
+-rw-rw-rw-   0        0        0     3399 2023-05-30 08:20:26.000000 gggdtparser-0.0.8/gggdtparser/langs/en.py
+-rw-rw-rw-   0        0        0      703 2023-05-25 03:05:13.000000 gggdtparser-0.0.8/gggdtparser/langs/es.py
+-rw-rw-rw-   0        0        0      943 2023-05-25 03:05:13.000000 gggdtparser-0.0.8/gggdtparser/langs/fra.py
+-rw-rw-rw-   0        0        0      223 2023-05-30 08:08:07.000000 gggdtparser-0.0.8/gggdtparser/langs/hi.py
+-rw-rw-rw-   0        0        0      239 2023-05-30 06:33:25.000000 gggdtparser-0.0.8/gggdtparser/langs/ky.py
+-rw-rw-rw-   0        0        0      345 2023-05-30 07:58:49.000000 gggdtparser-0.0.8/gggdtparser/langs/mr.py
+-rw-rw-rw-   0        0        0      804 2023-05-30 07:50:28.000000 gggdtparser-0.0.8/gggdtparser/langs/ru.py
+-rw-rw-rw-   0        0        0      249 2023-05-30 07:52:16.000000 gggdtparser-0.0.8/gggdtparser/langs/rw.py
+-rw-rw-rw-   0        0        0      238 2023-05-30 08:00:58.000000 gggdtparser-0.0.8/gggdtparser/langs/si.py
+-rw-rw-rw-   0        0        0      230 2023-05-25 03:05:13.000000 gggdtparser-0.0.8/gggdtparser/langs/so.py
+-rw-rw-rw-   0        0        0      329 2023-05-30 07:55:53.000000 gggdtparser-0.0.8/gggdtparser/langs/sw.py
+-rw-rw-rw-   0        0        0      745 2023-05-25 03:05:13.000000 gggdtparser-0.0.8/gggdtparser/langs/swe.py
+-rw-rw-rw-   0        0        0      195 2023-05-30 08:05:09.000000 gggdtparser-0.0.8/gggdtparser/langs/tg.py
+-rw-rw-rw-   0        0        0      300 2023-05-30 08:05:26.000000 gggdtparser-0.0.8/gggdtparser/langs/tr.py
+-rw-rw-rw-   0        0        0      811 2023-05-30 07:48:04.000000 gggdtparser-0.0.8/gggdtparser/langs/uk.py
+-rw-rw-rw-   0        0        0      231 2023-05-30 06:37:38.000000 gggdtparser-0.0.8/gggdtparser/langs/ur.py
+-rw-rw-rw-   0        0        0      432 2023-05-25 03:05:13.000000 gggdtparser-0.0.8/gggdtparser/langs/vie.py
+-rw-rw-rw-   0        0        0      802 2023-05-25 03:05:13.000000 gggdtparser-0.0.8/gggdtparser/langs/zh.py
+-rw-rw-rw-   0        0        0      609 2023-05-25 03:05:13.000000 gggdtparser-0.0.8/gggdtparser/langs/zht.py
+drwxrwxrwx   0        0        0        0 2023-05-30 11:42:51.314927 gggdtparser-0.0.8/gggdtparser/test/
+-rw-rw-rw-   0        0        0    43437 2023-05-25 04:15:16.000000 gggdtparser-0.0.8/gggdtparser/test/__init__.py
+-rw-rw-rw-   0        0        0      112 2023-05-30 07:17:35.000000 gggdtparser-0.0.8/gggdtparser/test/_id.py
+-rw-rw-rw-   0        0        0      829 2023-04-20 08:57:23.000000 gggdtparser-0.0.8/gggdtparser/test/az.py
+-rw-rw-rw-   0        0        0      120 2023-05-30 08:08:48.000000 gggdtparser-0.0.8/gggdtparser/test/hi.py
+-rw-rw-rw-   0        0        0      118 2023-05-30 06:34:41.000000 gggdtparser-0.0.8/gggdtparser/test/ky.py
+-rw-rw-rw-   0        0        0      211 2023-05-30 07:59:04.000000 gggdtparser-0.0.8/gggdtparser/test/mr.py
+-rw-rw-rw-   0        0        0      117 2023-05-30 07:52:38.000000 gggdtparser-0.0.8/gggdtparser/test/ru.py
+-rw-rw-rw-   0        0        0      136 2023-05-30 07:52:38.000000 gggdtparser-0.0.8/gggdtparser/test/rw.py
+-rw-rw-rw-   0        0        0      129 2023-05-30 08:01:52.000000 gggdtparser-0.0.8/gggdtparser/test/si.py
+-rw-rw-rw-   0        0        0      158 2023-05-30 07:56:38.000000 gggdtparser-0.0.8/gggdtparser/test/sw.py
+-rw-rw-rw-   0        0        0      129 2023-05-30 08:06:27.000000 gggdtparser-0.0.8/gggdtparser/test/tg.py
+-rw-rw-rw-   0        0        0      127 2023-05-30 08:03:19.000000 gggdtparser-0.0.8/gggdtparser/test/tr.py
+-rw-rw-rw-   0        0        0      178 2023-05-30 07:49:10.000000 gggdtparser-0.0.8/gggdtparser/test/uk.py
+-rw-rw-rw-   0        0        0      140 2023-05-30 06:39:37.000000 gggdtparser-0.0.8/gggdtparser/test/ur.py
+-rw-rw-rw-   0        0        0      555 2023-05-30 11:38:37.000000 gggdtparser-0.0.8/gggdtparser/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-30 11:42:51.269050 gggdtparser-0.0.8/gggdtparser.egg-info/
+-rw-rw-rw-   0        0        0     3404 2023-05-30 11:42:51.000000 gggdtparser-0.0.8/gggdtparser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1191 2023-05-30 11:42:51.000000 gggdtparser-0.0.8/gggdtparser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 11:42:51.000000 gggdtparser-0.0.8/gggdtparser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-30 11:42:51.000000 gggdtparser-0.0.8/gggdtparser.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      775 2023-05-30 11:42:51.317919 gggdtparser-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      165 2023-03-27 07:16:57.000000 gggdtparser-0.0.8/setup.py
```

### Comparing `gggdtparser-0.0.6/LICENSE` & `gggdtparser-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.0.6/PKG-INFO` & `gggdtparser-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gggdtparser
-Version: 0.0.6
+Version: 0.0.8
 Summary: 通用、便捷、准确的字符串时间解析工具
 Home-page: https://github.com/kusen-alpha/gggdtparser
 Author: kusen
 Author-email: hu1194542196@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/kusen-alpha/gggdtparser/issues
 Project-URL: Documentation, https://github.com/kusen-alpha/gggdtparser/blob/master/README.md
```

### Comparing `gggdtparser-0.0.6/README.md` & `gggdtparser-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `gggdtparser-0.0.6/gggdtparser/dtparser.py` & `gggdtparser-0.0.8/gggdtparser/dtparser.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,122 +2,157 @@
 # -*- coding:utf-8 -*-
 # author: kusen
 # email: 1194542196@qq.com
 # date: 2023/3/24
 
 import re
 import random
+import logging
 import datetime
 from . import dtconfigs
 
 
 class StringDateTimeLanguageHandler(object):
+
     @classmethod
-    def handle(cls, s, langs):
+    def handle(cls, string_datetime, langs):
         """
         根据语言进行一些特殊处理
-        :param s:
+        :param string_datetime:
         :param langs:
         :return:
         """
         if not langs:
             langs = []
         if not langs:
-            for key, value in dtconfigs.SUB_TRANSLATE.items():
-                for conf in value:
-                    s = re.sub(conf[0], conf[1], s)
+            for _lang, sub_list in dtconfigs.LANG_SUB_TRANSLATE.items():
+                for sub in sub_list:
+                    string_datetime = re.sub(sub[0], sub[1], string_datetime)
         for lang in langs:
-            sub_translate = dtconfigs.SUB_TRANSLATE.get(lang.upper())
-            if not sub_translate:
-                continue
-            for conf in sub_translate:
-                s = re.sub(conf[0], conf[1], s)
-        return s
+            _sub_translate = dtconfigs.LANG_SUB_TRANSLATE.get(
+                lang) or []
+            for sub in _sub_translate:
+                string_datetime = re.sub(sub[0], sub[1], string_datetime)
+        return string_datetime
 
 
 class StringDateTimeRegexParser(object):
     # 默认时间顺序
     DEFAULT_DATETIME_SEQ = ['year', 'month', 'day', 'hour', 'minute', 'second']
 
     @classmethod
-    def parse(cls, s, regex_list=None, langs=None, accurately=True,
-              max_datetime=None):
+    def parse(cls, string_datetime, regex_list=None, langs=None,
+              result_accurately=True, extract_accurately=False,
+              max_datetime=None, min_datetime=None):
         """
         通过正则对文本的时间进行抽取和解析
-        :param s: 文本时间
+        :param string_datetime: 文本时间
         :param regex_list: 正则列表
         :param langs: 语言
-        :param accurately: 是否遵循严格判断
-        :param max_datetime: 最大时间，超过解析失败，默认为now
+        :param result_accurately: 是否遵循严格判断
+        :param extract_accurately: 是否只进行精确抽取
+        :param max_datetime: 最大时间，超过解析失败
+        :param min_datetime: 最小时间，超过解析失败
         :return:
         """
+        if not langs:
+            langs = []
+        _langs = []
+        for lang in langs:
+            try:
+                _langs.append(dtconfigs.LANG_MAPPING[lang.lower()])
+            except KeyError:
+                if lang.lower() in dtconfigs.TRANSLATE_LANGS:
+                    logging.warning("语言:%s推荐先进行翻译" % lang)
+                else:
+                    logging.error("语言:%s设置有误" % lang)
+                return
+        langs = _langs
         if not regex_list:
             regex_list = []
         if isinstance(regex_list, str):
             regex_list = [regex_list, ]
-        s = StringDateTimeLanguageHandler.handle(s, langs)
+        string_datetime = StringDateTimeLanguageHandler.handle(
+            string_datetime, langs)
         if regex_list:
-            result = cls.match_and_parse(s, regex_list, accurately,
-                                         max_datetime)
+            result = cls.match_and_parse(
+                string_datetime, regex_list, result_accurately,
+                max_datetime, min_datetime)
             if result:
                 return result
-        if langs:
-            for lang in langs:
-                regex_list = dtconfigs.OTHER_STRING_DATE_TIME_REGEX_LIST.get(
-                    lang.upper()
-                )
-                if not regex_list:
-                    continue
-                result = cls.match_and_parse(
-                    s, getattr(dtconfigs, regex_list),
-                    accurately, max_datetime)
-                if result:
-                    return result
+        regex_list = cls.get_default_regex_list(langs, extract_accurately)
         result = cls.match_and_parse(
-            s, dtconfigs.STRING_DATE_TIME_REGEX_LIST, accurately, max_datetime)
+            string_datetime, regex_list,
+            result_accurately, max_datetime, min_datetime)
         if result:
             return result
-        for lang, regex_list in dtconfigs.OTHER_STRING_DATE_TIME_REGEX_LIST.items():
-            result = cls.match_and_parse(
-                s, regex_list, accurately, max_datetime)
-            if result:
-                return result
-        return cls.match_and_parse(
-            s, dtconfigs.STRING_DATE_TIME_REGEX_LIST_FUZZY,
-            accurately, max_datetime)
 
     @classmethod
-    def match_and_parse(cls, s, regex_list, accurately, max_datetime):
+    def get_default_regex_list(cls, langs, extract_accurately):
+        regex_list = []
+        if langs:
+            if extract_accurately:
+                for lang in langs:
+                    regex_list.extend(cls._get_default_regex_list(lang, True))
+            else:
+                for lang in langs:
+                    regex_list.extend(cls._get_default_regex_list(lang, True))
+                for lang in langs:
+                    regex_list.extend(cls._get_default_regex_list(lang, False))
+            return regex_list
+        for value in dtconfigs.LANG_ACCURATE_REGEX_LIST.values():
+            regex_list.extend(value or [])
+        if not extract_accurately:
+            for value in dtconfigs.LANG_FUZZY_REGEX_LIST.values():
+                regex_list.extend(value or [])
+        return regex_list
+
+    @classmethod
+    def _get_default_regex_list(cls, lang, extract_accurately):
+        if extract_accurately:
+            return dtconfigs.LANG_ACCURATE_REGEX_LIST.get(lang) or []
+        return dtconfigs.LANG_FUZZY_REGEX_LIST.get(lang) or []
+
+    @classmethod
+    def match_and_parse(cls, string_datetime, regex_list,
+                        result_accurately, max_datetime, min_datetime):
         for regex in regex_list:
             try:
-                match_obj = re.search(regex, s, flags=re.M | re.I | re.S)
+                match_obj = re.search(
+                    regex, string_datetime, flags=re.M | re.I | re.S)
             except (ValueError, re.error) as e:
-                # print(regex, s, e)
                 continue
             if not match_obj:
                 continue
             group_dict = match_obj.groupdict()
             if group_dict:
                 try:
                     result = cls._parse_group_dict(
-                        group_dict, accurately, max_datetime)
+                        group_dict, result_accurately,
+                        max_datetime, min_datetime)
                     # print(regex)
                     return result
                 except Exception:
                     continue
 
     @classmethod
-    def _parse_group_dict(cls, group_dict, accurately, max_datetime):
-        un_accurately = not accurately
+    def _parse_group_dict(cls, group_dict, result_accurately, max_datetime,
+                          min_datetime):
+        un_result_accurately = not result_accurately
         now = datetime.datetime.now()
         timestamp = int(group_dict.get('ts') or 0)
         if timestamp:
             if len(str(timestamp)) == 13:
                 timestamp = int(timestamp) // 1000
-            return datetime.datetime.fromtimestamp(timestamp)
+            parse_datetime = datetime.datetime.fromtimestamp(timestamp)
+            if max_datetime and parse_datetime > max_datetime:
+                raise Exception('解析时间超出最大时间')
+            if min_datetime and parse_datetime < min_datetime:
+                raise Exception('解析时间超出最小时间')
+            return parse_datetime
         year = group_dict.get('Y')  # or now.year
         if year and isinstance(year, str) and len(year) == 2:
             year = '20' + year
         month = group_dict.get('m')
         day = group_dict.get('d')
         hour = group_dict.get('H')
         minute = group_dict.get('M')
@@ -140,22 +175,22 @@
         change_before['bm'] = int(group_dict.get('bm') or 0)
         change_before['bd'] = int(group_dict.get('bd') or 0)
         change_before['bH'] = int(group_dict.get('bH') or 0)
         change_before['bM'] = int(group_dict.get('bM') or 0)
         change_before['bS'] = int(group_dict.get('bS') or 0)
         change_before['ba'] = int(group_dict.get('ba') or 0)
         for key in change_before:
-            if change_before[key] <= 0 or accurately:
+            if change_before[key] <= 0 or result_accurately:
                 continue
             change_before[key] += round(random.random(), 2)
         if change_before['bY'] > 0:
             change_day += change_before['bY'] * 365
             cls._update_use_now_config(use_now_config, year=True,
-                                       month=not accurately,
-                                       day=not accurately)
+                                       month=not result_accurately,
+                                       day=not result_accurately)
         if change_before['bm'] > 0:
             change_day += change_before['bm'] * 30
             cls._update_use_now_config(use_now_config, year=True,
                                        month=True, day=True)
         if change_before['ba'] > 0:
             change_day += change_before['ba'] * 7
             cls._update_use_now_config(use_now_config, year=True,
@@ -183,22 +218,22 @@
         change_within['wm'] = int(group_dict.get('wm') or 0)
         change_within['wd'] = int(group_dict.get('wd') or 0)
         change_within['wH'] = int(group_dict.get('wH') or 0)
         change_within['wM'] = int(group_dict.get('wM') or 0)
         change_within['wS'] = int(group_dict.get('wS') or 0)
         change_within['wa'] = int(group_dict.get('wa') or 0)
         for key in change_within:
-            if change_within[key] <= 0 or accurately:
+            if change_within[key] <= 0 or result_accurately:
                 continue
             change_within[key] -= round(random.random(), 1)
         if change_within['wY'] > 0:
             change_day += change_within['wY'] * 365
             cls._update_use_now_config(use_now_config, year=True,
-                                       month=not accurately,
-                                       day=not accurately)
+                                       month=not result_accurately,
+                                       day=not result_accurately)
         if change_within['wm'] > 0:
             change_day += change_within['wm'] * 30
             cls._update_use_now_config(use_now_config, year=True,
                                        month=True, day=True)
         if change_within['wa'] > 0:
             change_day += change_within['wa'] * 7
             cls._update_use_now_config(use_now_config, year=True,
@@ -224,28 +259,28 @@
         special_day = group_dict.get('sd') or ''
         special_other = group_dict.get('so') or ''
         if special_day:
             if special_day == "今天":
                 change_day += 0
                 cls._update_use_now_config(
                     use_now_config, year=True, month=True, day=True,
-                    hour=un_accurately, minute=un_accurately,
-                    second=un_accurately)
+                    hour=un_result_accurately, minute=un_result_accurately,
+                    second=un_result_accurately)
             elif special_day == "昨天":
                 change_day += 1
                 cls._update_use_now_config(
                     use_now_config, year=True, month=True, day=True,
-                    hour=un_accurately, minute=un_accurately,
-                    second=un_accurately)
+                    hour=un_result_accurately, minute=un_result_accurately,
+                    second=un_result_accurately)
             elif special_day == "前天":
                 change_day += 2
                 cls._update_use_now_config(
                     use_now_config, year=True, month=True, day=True,
-                    hour=un_accurately, minute=un_accurately,
-                    second=un_accurately)
+                    hour=un_result_accurately, minute=un_result_accurately,
+                    second=un_result_accurately)
         if special_other:
             if special_other == '刚刚':
                 change_second += 5
                 cls._update_use_now_config(
                     use_now_config, year=True, month=True,
                     day=True, hour=True, minute=True, second=True)
         # 民国时间
@@ -254,115 +289,118 @@
             year = 1911 + int(mg_year)
             month = month if month else 1
         # 计算时间
         change_timedelta = datetime.timedelta(
             days=change_day, hours=change_hour,
             minutes=change_minute, seconds=change_second)
         year = cls._get_default_or_now(
-            accurately, use_now_config['year'], now.year, year)
+            result_accurately, use_now_config['year'], now.year, year)
         month = cls._get_default_or_now(
-            accurately, use_now_config['month'], now.month, month)
+            result_accurately, use_now_config['month'], now.month, month)
         day = cls._get_default_or_now(
-            accurately, use_now_config['day'], now.day, day)
+            result_accurately, use_now_config['day'], now.day, day)
         hour = cls._get_default_or_now(
-            accurately, use_now_config['hour'], now.hour, hour)
+            result_accurately, use_now_config['hour'], now.hour, hour)
         minute = cls._get_default_or_now(
-            accurately, use_now_config['minute'], now.minute, minute)
+            result_accurately, use_now_config['minute'], now.minute, minute)
         second = cls._get_default_or_now(
-            accurately, use_now_config['second'], now.second, second)
+            result_accurately, use_now_config['second'], now.second, second)
         month = 1 if not month else month
         day = 1 if not day else day
         # 上下午
         apm = group_dict.get('apm')
         if apm == 'pm':
             hour += 12 if hour and hour < 12 else hour
         parse_datetime = datetime.datetime(
             year=year, month=month,
             day=day, hour=hour,
             minute=minute, second=second) - change_timedelta
         if max_datetime and parse_datetime > max_datetime:
             raise Exception('解析时间超出最大时间')
+        if min_datetime and parse_datetime < min_datetime:
+            raise Exception('解析时间超出最小时间')
         return parse_datetime
 
     @classmethod
     def _update_use_now_config(cls, use_now_config, year=False, month=False,
                                day=False, hour=False, minute=False,
                                second=False):
         use_now_config['year'] = year
         use_now_config['month'] = month
         use_now_config['day'] = day
         use_now_config['hour'] = hour
         use_now_config['minute'] = minute
         use_now_config['second'] = second
 
     @classmethod
-    def _get_default_or_now(cls, accurately, use_now_enabled,
+    def _get_default_or_now(cls, result_accurately, use_now_enabled,
                             now_value, default_value):
         return int((now_value if default_value is None and (
-                use_now_enabled or not accurately) else default_value) or 0)
+                use_now_enabled or not result_accurately) else default_value) or 0)
 
     @classmethod
     def _update_use_now_config_by_has_parse(
             cls, use_now_config, year, month, day, hour, minute, second):
         parse_flag = '%s%s%s%s%s%s' % (
             int(bool(year)), int(bool(month)), int(bool(day)),
             int(bool(hour)), int(bool(minute)), int(bool(second))
         )
         for index, flag in enumerate(parse_flag):
             if flag == '1':
                 break
             use_now_config[cls.DEFAULT_DATETIME_SEQ[index]] = True
 
 
-parse_string_datetime_by_regex = StringDateTimeRegexParser.parse
+parse_by_regex = StringDateTimeRegexParser.parse
 
 
-def parse_string_datetime_by_format(s, format_list=None):
+def parse_by_format(string_datetime, format_list=None):
     """
     通过format进行时间解析
-    :param s:
-    :param fs:
-    :param accurately:
+    :param string_datetime:
+    :param format_list:
     :return:
     """
     if not format_list:
         format_list = []
     for f in format_list:
         try:
-            return datetime.datetime.strptime(s, f)
-        except ValueError:
-            continue
-    for f in dtconfigs.DATE_TIME_FORMATS:
-        try:
-            return datetime.datetime.strptime(s, f)
+            return datetime.datetime.strptime(string_datetime, f)
         except ValueError:
             continue
 
 
-def parse_string_datetime(s, format_list=None, regex_list=None,
-                          langs=None, accurately=True,
-                          max_datetime=None):
+def parse(string_datetime, format_list=None, regex_list=None,
+          langs=None, result_accurately=True, extract_accurately=False,
+          max_datetime=None, min_datetime=None, translate_func=None):
     """
     解析文本时间
-    :param s: 字符串时间文本
+    :param string_datetime: 字符串时间文本
     :param format_list: 时间解析模板列表，如%Y-%m-%d
     :param regex_list: 正则解析规则列表，统一为有名分组格式，参考dtconfigs.py
     :param langs: 语言列表，优先设置的语言进行翻译替换和解析
-    :param accurately: 是否为严格模式,format不支持非严格模式
+    :param result_accurately: 解析結果是否为严格模式,format不支持非严格模式
+    :param extract_accurately:  是否只进行精确抽取
     :param max_datetime: 最大时间
+    :param min_datetime: 最小时间
+    :param translate_func: 翻译函数
     :return: datetime.datetime
     """
     # format
     # regex
     # fanyi
-    result = parse_string_datetime_by_format(s, format_list)
+    if translate_func and callable(translate_func):
+        string_datetime = translate_func(string_datetime)
+    result = parse_by_format(string_datetime, format_list)
     if result:
         return result
-    result = parse_string_datetime_by_regex(s, regex_list, langs, accurately,
-                                            max_datetime=max_datetime)
+    result = parse_by_regex(
+        string_datetime, regex_list, langs, result_accurately,
+        max_datetime=max_datetime, min_datetime=min_datetime,
+        extract_accurately=extract_accurately)
     if result:
         return result
 
 
 def check(dst_dt, check_dt):
     """
     检测解析结果
@@ -372,12 +410,10 @@
     """
     if isinstance(check_dt, datetime.datetime):
         return dst_dt == check_dt
     start_dt, end_dt = check_dt
     return start_dt <= dst_dt <= end_dt
 
 
-parse = parse_string_datetime
-
 if __name__ == '__main__':
-    result1 = parse_string_datetime_by_format('2022年', fs=['%Y年'])
+    result1 = parse('2022年', fs=['%Y年'])
     print(result1)
```

### Comparing `gggdtparser-0.0.6/gggdtparser.egg-info/PKG-INFO` & `gggdtparser-0.0.8/gggdtparser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gggdtparser
-Version: 0.0.6
+Version: 0.0.8
 Summary: 通用、便捷、准确的字符串时间解析工具
 Home-page: https://github.com/kusen-alpha/gggdtparser
 Author: kusen
 Author-email: hu1194542196@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/kusen-alpha/gggdtparser/issues
 Project-URL: Documentation, https://github.com/kusen-alpha/gggdtparser/blob/master/README.md
```

### Comparing `gggdtparser-0.0.6/setup.cfg` & `gggdtparser-0.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 6767 6474 7061 7273 6572 0d0a   = gggdtparser..
-00000020: 7665 7273 696f 6e20 3d20 302e 302e 360d  version = 0.0.6.
+00000020: 7665 7273 696f 6e20 3d20 302e 302e 380d  version = 0.0.8.
 00000030: 0a61 7574 686f 7220 3d20 6b75 7365 6e0d  .author = kusen.
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 6875 3131 3934 3534 3231 3936 4071 712e  hu1194542196@qq.
 00000060: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000070: 203d 20cd a8d3 c3a1 a2b1 e3bd dda1 a2d7   = .............
 00000080: bcc8 b7b5 c4d7 d6b7 fbb4 aeca b1bc e4bd  ................
 00000090: e2ce f6b9 a4be df0d 0a6c 6f6e 675f 6465  .........long_de
```

