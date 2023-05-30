# Comparing `tmp/biblebot-0.4.2.tar.gz` & `tmp/biblebot-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\biblebot-0.4.2.tar", last modified: Sun Apr 23 07:50:07 2023, max compression
+gzip compressed data, was "dist\biblebot-0.4.3.tar", last modified: Tue May 30 13:00:33 2023, max compression
```

## Comparing `biblebot-0.4.2.tar` & `biblebot-0.4.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-23 07:50:07.000000 biblebot-0.4.2/
--rw-rw-rw-   0        0        0     1092 2023-04-23 07:47:19.000000 biblebot-0.4.2/LICENSE
--rw-rw-rw-   0        0        0    11662 2023-04-23 07:50:07.000000 biblebot-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0    10964 2023-04-23 07:47:19.000000 biblebot-0.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-23 07:50:06.000000 biblebot-0.4.2/biblebot/
--rw-rw-rw-   0        0        0      691 2021-02-02 08:18:09.000000 biblebot-0.4.2/biblebot/__init__.py
--rw-rw-rw-   0        0        0      557 2023-04-23 07:48:38.000000 biblebot-0.4.2/biblebot/__version__.py
-drwxrwxrwx   0        0        0        0 2023-04-23 07:50:06.000000 biblebot-0.4.2/biblebot/api/
--rw-rw-rw-   0        0        0     2494 2023-04-03 06:31:51.000000 biblebot-0.4.2/biblebot/api/__init__.py
--rw-rw-rw-   0        0        0     6463 2020-10-28 08:43:32.000000 biblebot-0.4.2/biblebot/api/_mileage.py
--rw-rw-rw-   0        0        0     2974 2020-10-28 08:43:32.000000 biblebot-0.4.2/biblebot/api/base.py
--rw-rw-rw-   0        0        0     3398 2023-04-03 06:31:51.000000 biblebot-0.4.2/biblebot/api/common.py
--rw-rw-rw-   0        0        0    19912 2023-04-03 06:31:51.000000 biblebot-0.4.2/biblebot/api/intranet.py
--rw-rw-rw-   0        0        0     4599 2020-10-28 08:43:32.000000 biblebot-0.4.2/biblebot/api/kbu.py
--rw-rw-rw-   0        0        0     6410 2023-04-03 06:31:51.000000 biblebot-0.4.2/biblebot/api/library.py
--rw-rw-rw-   0        0        0    13916 2022-05-31 09:04:43.000000 biblebot-0.4.2/biblebot/api/lms.py
--rw-rw-rw-   0        0        0     6692 2023-04-03 06:31:51.000000 biblebot-0.4.2/biblebot/api/mileage.py
--rw-rw-rw-   0        0        0     1387 2020-10-28 08:43:32.000000 biblebot-0.4.2/biblebot/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-23 07:50:07.000000 biblebot-0.4.2/biblebot/reqeust/
--rw-rw-rw-   0        0        0      377 2020-10-28 08:43:32.000000 biblebot-0.4.2/biblebot/reqeust/__init__.py
--rw-rw-rw-   0        0        0     2821 2021-02-04 04:00:45.000000 biblebot-0.4.2/biblebot/reqeust/aiohttp_conn.py
--rw-rw-rw-   0        0        0     5087 2020-10-28 08:43:32.000000 biblebot-0.4.2/biblebot/reqeust/base.py
--rw-rw-rw-   0        0        0     2312 2020-10-28 08:43:32.000000 biblebot-0.4.2/biblebot/reqeust/requests_conn.py
-drwxrwxrwx   0        0        0        0 2023-04-23 07:50:06.000000 biblebot-0.4.2/biblebot.egg-info/
--rw-rw-rw-   0        0        0    11662 2023-04-23 07:50:06.000000 biblebot-0.4.2/biblebot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      581 2023-04-23 07:50:06.000000 biblebot-0.4.2/biblebot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-23 07:50:06.000000 biblebot-0.4.2/biblebot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-04-23 07:50:06.000000 biblebot-0.4.2/biblebot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-23 07:50:06.000000 biblebot-0.4.2/biblebot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-23 07:50:07.000000 biblebot-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1258 2023-04-03 06:31:06.000000 biblebot-0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:00:33.000000 biblebot-0.4.3/
+-rw-rw-rw-   0        0        0     1092 2023-04-23 07:47:19.000000 biblebot-0.4.3/LICENSE
+-rw-rw-rw-   0        0        0    11402 2023-05-30 13:00:33.000000 biblebot-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0    10704 2023-05-30 12:58:58.000000 biblebot-0.4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 13:00:33.000000 biblebot-0.4.3/biblebot/
+-rw-rw-rw-   0        0        0      691 2021-02-02 08:18:09.000000 biblebot-0.4.3/biblebot/__init__.py
+-rw-rw-rw-   0        0        0      557 2023-05-30 12:58:58.000000 biblebot-0.4.3/biblebot/__version__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:00:33.000000 biblebot-0.4.3/biblebot/api/
+-rw-rw-rw-   0        0        0     2494 2023-04-03 06:31:51.000000 biblebot-0.4.3/biblebot/api/__init__.py
+-rw-rw-rw-   0        0        0     6463 2020-10-28 08:43:32.000000 biblebot-0.4.3/biblebot/api/_mileage.py
+-rw-rw-rw-   0        0        0     2974 2020-10-28 08:43:32.000000 biblebot-0.4.3/biblebot/api/base.py
+-rw-rw-rw-   0        0        0     3398 2023-04-03 06:31:51.000000 biblebot-0.4.3/biblebot/api/common.py
+-rw-rw-rw-   0        0        0    19912 2023-04-03 06:31:51.000000 biblebot-0.4.3/biblebot/api/intranet.py
+-rw-rw-rw-   0        0        0     4599 2020-10-28 08:43:32.000000 biblebot-0.4.3/biblebot/api/kbu.py
+-rw-rw-rw-   0        0        0     6410 2023-04-03 06:31:51.000000 biblebot-0.4.3/biblebot/api/library.py
+-rw-rw-rw-   0        0        0    13916 2022-05-31 09:04:43.000000 biblebot-0.4.3/biblebot/api/lms.py
+-rw-rw-rw-   0        0        0     6692 2023-04-03 06:31:51.000000 biblebot-0.4.3/biblebot/api/mileage.py
+-rw-rw-rw-   0        0        0     1387 2020-10-28 08:43:32.000000 biblebot-0.4.3/biblebot/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:00:33.000000 biblebot-0.4.3/biblebot/reqeust/
+-rw-rw-rw-   0        0        0      377 2020-10-28 08:43:32.000000 biblebot-0.4.3/biblebot/reqeust/__init__.py
+-rw-rw-rw-   0        0        0     2821 2021-02-04 04:00:45.000000 biblebot-0.4.3/biblebot/reqeust/aiohttp_conn.py
+-rw-rw-rw-   0        0        0     5087 2020-10-28 08:43:32.000000 biblebot-0.4.3/biblebot/reqeust/base.py
+-rw-rw-rw-   0        0        0     2312 2020-10-28 08:43:32.000000 biblebot-0.4.3/biblebot/reqeust/requests_conn.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:00:33.000000 biblebot-0.4.3/biblebot.egg-info/
+-rw-rw-rw-   0        0        0    11402 2023-05-30 13:00:32.000000 biblebot-0.4.3/biblebot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      581 2023-05-30 13:00:32.000000 biblebot-0.4.3/biblebot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 13:00:32.000000 biblebot-0.4.3/biblebot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-05-30 13:00:32.000000 biblebot-0.4.3/biblebot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-30 13:00:32.000000 biblebot-0.4.3/biblebot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 13:00:33.000000 biblebot-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1258 2023-04-03 06:31:06.000000 biblebot-0.4.3/setup.py
```

### Comparing `biblebot-0.4.2/LICENSE` & `biblebot-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `biblebot-0.4.2/PKG-INFO` & `biblebot-0.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biblebot
-Version: 0.4.2
+Version: 0.4.3
 Summary: Scraper for KBU students
 Home-page: https://github.com/rekyungmin/biblebot-scraper
 Author: Kyungmin Lee
 Author-email: rekyungmin@gmail.com
 Maintainer: Kyungmin Lee <rekyungmin@gmail.com>, Yongki Kim <ygflove@likelion.org>
 License: UNKNOWN
 Platform: UNKNOWN
@@ -22,16 +22,14 @@
 <p align="center">
 <a href="https://www.python.org/downloads/release/python-370/"><img alt="Python" src="https://img.shields.io/badge/python-3.7-blue?logo=python&logoColor=white"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 </p>
 
 성서봇 스크래이퍼는 한국성서대학교와 연관된 정보를 수집할 수 있는 파이썬 패키지입니다.
 
-이 패키지를 바탕으로, **성서봇** 모바일 애플리케이션([Android](https://play.google.com/store/apps/details?id=com.blogspot.ramming125.kbubot&hl=ko))이 한국성서대학교학생들에게 2018년부터 실서비스 되고 있습니다.
-
 이 패키지는 다섯 가지 웹사이트에 대한 스크래이퍼를 제공합니다.
 
 1. [한국성서대학교 인트라넷](https://kbuis.bible.ac.kr/) 스크래이퍼  
 2. [한국성서대학교 LMS](https://lms.bible.ac.kr/) 스크래이퍼
 3. [한국성서대학교 홈페이지](https://www.bible.ac.kr/) 스크래이퍼  
 4. [OKPOS 마일리지 시스템](https://asp.netusys.com/) 스크래이퍼  
 5. [한국성서대학교 도서관](https://lib.bible.ac.kr/) 스크래이퍼
```

#### html2text {}

```diff
@@ -1,41 +1,38 @@
-Metadata-Version: 2.1 Name: biblebot Version: 0.4.2 Summary: Scraper for KBU
+Metadata-Version: 2.1 Name: biblebot Version: 0.4.3 Summary: Scraper for KBU
 students Home-page: https://github.com/rekyungmin/biblebot-scraper Author:
 Kyungmin Lee Author-email: rekyungmin@gmail.com Maintainer: Kyungmin Lee
 gmail.com>, Yongki Kim
 likelion.org> License: UNKNOWN Platform: UNKNOWN Classifier: License :: OSI
 Approved :: MIT License Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Requires-Python:
 >=3.7 Description-Content-Type: text/markdown Provides-Extra: http License-
 File: LICENSE
                         ****** Biblebot Scraper ******
                          [Python] [Code_style:_black]
 ì±ìë´ ì¤í¬ëì´í¼ë íêµ­ì±ìëíêµì ì°ê´ë ì ë³´ë¥¼
-ìì§í  ì ìë íì´ì¬ í¨í¤ì§ìëë¤. ì´ í¨í¤ì§ë¥¼
-ë°íì¼ë¡, **ì±ìë´** ëª¨ë°ì¼ ì íë¦¬ì¼ì´ì([Android](https://
-play.google.com/store/apps/details?id=com.blogspot.ramming125.kbubot&hl=ko))ì´
-íêµ­ì±ìëíêµíìë¤ìê² 2018ëë¶í° ì¤ìë¹ì¤ ëê³ 
-ììµëë¤. ì´ í¨í¤ì§ë ë¤ì¯ ê°ì§ ì¹ì¬ì´í¸ì ëí
-ì¤í¬ëì´í¼ë¥¼ ì ê³µí©ëë¤. 1. [íêµ­ì±ìëíêµ ì¸í¸ë¼ë·]
-(https://kbuis.bible.ac.kr/) ì¤í¬ëì´í¼ 2. [íêµ­ì±ìëíêµ LMS]
-(https://lms.bible.ac.kr/) ì¤í¬ëì´í¼ 3. [íêµ­ì±ìëíêµ
-ííì´ì§](https://www.bible.ac.kr/) ì¤í¬ëì´í¼ 4. [OKPOS ë§ì¼ë¦¬ì§
-ìì¤í](https://asp.netusys.com/) ì¤í¬ëì´í¼ 5. [íêµ­ì±ìëíêµ
-ëìê´](https://lib.bible.ac.kr/) ì¤í¬ëì´í¼ ## Installation ``` $ pip
-install 'biblebot[http]' ``` ## Requirements - `beautifulsoup4`: htmlê³¼ xml
-ìì ë°ì´í°ë¥¼ ì¶ì¶íê¸° ìí´ ì¬ì©í©ëë¤. - `aiohttp`: HTTP
-ìì²­ì ìí´ ì¬ì©í©ëë¤. (OPTIONAL) HTTP ìì²­ì ìí´ HTTP ìì²­
-í¨í¤ì§ê° íìí©ëë¤. `aiohttp` ëë `requests` í¨í¤ì§ê°
-ì¡´ì¬í  ê²½ì° ìëì¼ë¡ ì¸ìíì¬ ì¬ì©í©ëë¤. ê·¸ ì¸ì HTTP
-ìì²­ í¨í¤ì§ë¥¼ ì´ì©íê³  ì¶ë¤ë©´ `BaseRequest` ì¶ìí´ëì¤ë¥¼
-ììë°ì êµ¬íí ë¤, `HTTPClient.set`ì ì´ì©íì¬ ë±ë¡í´
-ì¬ì©í  ì ììµëë¤. ## ð Documentation [APIs document](docs/APIs.md)
-## Get started ### ê³µì§ì¬í­ ê°ì ¸ì¤ê¸° ````python import asyncio from
-pprint import pprint from biblebot import KbuAPI async def main(): resp = await
+ìì§í  ì ìë íì´ì¬ í¨í¤ì§ìëë¤. ì´ í¨í¤ì§ë ë¤ì¯
+ê°ì§ ì¹ì¬ì´í¸ì ëí ì¤í¬ëì´í¼ë¥¼ ì ê³µí©ëë¤. 1.
+[íêµ­ì±ìëíêµ ì¸í¸ë¼ë·](https://kbuis.bible.ac.kr/
+) ì¤í¬ëì´í¼ 2. [íêµ­ì±ìëíêµ LMS](https://lms.bible.ac.kr/
+) ì¤í¬ëì´í¼ 3. [íêµ­ì±ìëíêµ ííì´ì§](https://
+www.bible.ac.kr/) ì¤í¬ëì´í¼ 4. [OKPOS ë§ì¼ë¦¬ì§ ìì¤í](https://
+asp.netusys.com/) ì¤í¬ëì´í¼ 5. [íêµ­ì±ìëíêµ ëìê´](https://
+lib.bible.ac.kr/) ì¤í¬ëì´í¼ ## Installation ``` $ pip install 'biblebot
+[http]' ``` ## Requirements - `beautifulsoup4`: htmlê³¼ xml ìì ë°ì´í°ë¥¼
+ì¶ì¶íê¸° ìí´ ì¬ì©í©ëë¤. - `aiohttp`: HTTP ìì²­ì ìí´
+ì¬ì©í©ëë¤. (OPTIONAL) HTTP ìì²­ì ìí´ HTTP ìì²­ í¨í¤ì§ê°
+íìí©ëë¤. `aiohttp` ëë `requests` í¨í¤ì§ê° ì¡´ì¬í  ê²½ì°
+ìëì¼ë¡ ì¸ìíì¬ ì¬ì©í©ëë¤. ê·¸ ì¸ì HTTP ìì²­ í¨í¤ì§ë¥¼
+ì´ì©íê³  ì¶ë¤ë©´ `BaseRequest` ì¶ìí´ëì¤ë¥¼ ììë°ì êµ¬íí
+ë¤, `HTTPClient.set`ì ì´ì©íì¬ ë±ë¡í´ ì¬ì©í  ì ììµëë¤. ##
+ð Documentation [APIs document](docs/APIs.md) ## Get started ###
+ê³µì§ì¬í­ ê°ì ¸ì¤ê¸° ````python import asyncio from pprint import pprint
+from biblebot import KbuAPI async def main(): resp = await
 KbuAPI.MainNotice.fetch(page=2) # ê³µì§ì¬í­ 2íì´ì§ result =
 KbuAPI.MainNotice.parse(resp) pprint(result.data) asyncio.run(main()) ````
 **Output:** ```json { "notice": [ { "seq": "3742", "title": "[ëíì ìì]
 2020íëë íê¸° íêµ­ì±ìëíêµ ëíì ì ìì ëª¨ì§",
 "author": "ì¥ì±í¬", "date": "2020-07-31", "url": "https://www.bible.ac.kr/
 ko/life/notice/view/46649?p=2" }, { "seq": "3741", "title": "[ê¸°ì´êµì¡ì]
 2020-2íê¸° ìê°ì ì²­ ê¸°ì´êµì¡ì, ìì´êµì¡ì¼í° ê³µì§ì¬í­
```

### Comparing `biblebot-0.4.2/README.md` & `biblebot-0.4.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 <p align="center">
 <a href="https://www.python.org/downloads/release/python-370/"><img alt="Python" src="https://img.shields.io/badge/python-3.7-blue?logo=python&logoColor=white"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 </p>
 
 성서봇 스크래이퍼는 한국성서대학교와 연관된 정보를 수집할 수 있는 파이썬 패키지입니다.
 
-이 패키지를 바탕으로, **성서봇** 모바일 애플리케이션([Android](https://play.google.com/store/apps/details?id=com.blogspot.ramming125.kbubot&hl=ko))이 한국성서대학교학생들에게 2018년부터 실서비스 되고 있습니다.
-
 이 패키지는 다섯 가지 웹사이트에 대한 스크래이퍼를 제공합니다.
 
 1. [한국성서대학교 인트라넷](https://kbuis.bible.ac.kr/) 스크래이퍼  
 2. [한국성서대학교 LMS](https://lms.bible.ac.kr/) 스크래이퍼
 3. [한국성서대학교 홈페이지](https://www.bible.ac.kr/) 스크래이퍼  
 4. [OKPOS 마일리지 시스템](https://asp.netusys.com/) 스크래이퍼  
 5. [한국성서대학교 도서관](https://lib.bible.ac.kr/) 스크래이퍼
```

#### html2text {}

```diff
@@ -1,31 +1,28 @@
                         ****** Biblebot Scraper ******
                          [Python] [Code_style:_black]
 ì±ìë´ ì¤í¬ëì´í¼ë íêµ­ì±ìëíêµì ì°ê´ë ì ë³´ë¥¼
-ìì§í  ì ìë íì´ì¬ í¨í¤ì§ìëë¤. ì´ í¨í¤ì§ë¥¼
-ë°íì¼ë¡, **ì±ìë´** ëª¨ë°ì¼ ì íë¦¬ì¼ì´ì([Android](https://
-play.google.com/store/apps/details?id=com.blogspot.ramming125.kbubot&hl=ko))ì´
-íêµ­ì±ìëíêµíìë¤ìê² 2018ëë¶í° ì¤ìë¹ì¤ ëê³ 
-ììµëë¤. ì´ í¨í¤ì§ë ë¤ì¯ ê°ì§ ì¹ì¬ì´í¸ì ëí
-ì¤í¬ëì´í¼ë¥¼ ì ê³µí©ëë¤. 1. [íêµ­ì±ìëíêµ ì¸í¸ë¼ë·]
-(https://kbuis.bible.ac.kr/) ì¤í¬ëì´í¼ 2. [íêµ­ì±ìëíêµ LMS]
-(https://lms.bible.ac.kr/) ì¤í¬ëì´í¼ 3. [íêµ­ì±ìëíêµ
-ííì´ì§](https://www.bible.ac.kr/) ì¤í¬ëì´í¼ 4. [OKPOS ë§ì¼ë¦¬ì§
-ìì¤í](https://asp.netusys.com/) ì¤í¬ëì´í¼ 5. [íêµ­ì±ìëíêµ
-ëìê´](https://lib.bible.ac.kr/) ì¤í¬ëì´í¼ ## Installation ``` $ pip
-install 'biblebot[http]' ``` ## Requirements - `beautifulsoup4`: htmlê³¼ xml
-ìì ë°ì´í°ë¥¼ ì¶ì¶íê¸° ìí´ ì¬ì©í©ëë¤. - `aiohttp`: HTTP
-ìì²­ì ìí´ ì¬ì©í©ëë¤. (OPTIONAL) HTTP ìì²­ì ìí´ HTTP ìì²­
-í¨í¤ì§ê° íìí©ëë¤. `aiohttp` ëë `requests` í¨í¤ì§ê°
-ì¡´ì¬í  ê²½ì° ìëì¼ë¡ ì¸ìíì¬ ì¬ì©í©ëë¤. ê·¸ ì¸ì HTTP
-ìì²­ í¨í¤ì§ë¥¼ ì´ì©íê³  ì¶ë¤ë©´ `BaseRequest` ì¶ìí´ëì¤ë¥¼
-ììë°ì êµ¬íí ë¤, `HTTPClient.set`ì ì´ì©íì¬ ë±ë¡í´
-ì¬ì©í  ì ììµëë¤. ## ð Documentation [APIs document](docs/APIs.md)
-## Get started ### ê³µì§ì¬í­ ê°ì ¸ì¤ê¸° ````python import asyncio from
-pprint import pprint from biblebot import KbuAPI async def main(): resp = await
+ìì§í  ì ìë íì´ì¬ í¨í¤ì§ìëë¤. ì´ í¨í¤ì§ë ë¤ì¯
+ê°ì§ ì¹ì¬ì´í¸ì ëí ì¤í¬ëì´í¼ë¥¼ ì ê³µí©ëë¤. 1.
+[íêµ­ì±ìëíêµ ì¸í¸ë¼ë·](https://kbuis.bible.ac.kr/
+) ì¤í¬ëì´í¼ 2. [íêµ­ì±ìëíêµ LMS](https://lms.bible.ac.kr/
+) ì¤í¬ëì´í¼ 3. [íêµ­ì±ìëíêµ ííì´ì§](https://
+www.bible.ac.kr/) ì¤í¬ëì´í¼ 4. [OKPOS ë§ì¼ë¦¬ì§ ìì¤í](https://
+asp.netusys.com/) ì¤í¬ëì´í¼ 5. [íêµ­ì±ìëíêµ ëìê´](https://
+lib.bible.ac.kr/) ì¤í¬ëì´í¼ ## Installation ``` $ pip install 'biblebot
+[http]' ``` ## Requirements - `beautifulsoup4`: htmlê³¼ xml ìì ë°ì´í°ë¥¼
+ì¶ì¶íê¸° ìí´ ì¬ì©í©ëë¤. - `aiohttp`: HTTP ìì²­ì ìí´
+ì¬ì©í©ëë¤. (OPTIONAL) HTTP ìì²­ì ìí´ HTTP ìì²­ í¨í¤ì§ê°
+íìí©ëë¤. `aiohttp` ëë `requests` í¨í¤ì§ê° ì¡´ì¬í  ê²½ì°
+ìëì¼ë¡ ì¸ìíì¬ ì¬ì©í©ëë¤. ê·¸ ì¸ì HTTP ìì²­ í¨í¤ì§ë¥¼
+ì´ì©íê³  ì¶ë¤ë©´ `BaseRequest` ì¶ìí´ëì¤ë¥¼ ììë°ì êµ¬íí
+ë¤, `HTTPClient.set`ì ì´ì©íì¬ ë±ë¡í´ ì¬ì©í  ì ììµëë¤. ##
+ð Documentation [APIs document](docs/APIs.md) ## Get started ###
+ê³µì§ì¬í­ ê°ì ¸ì¤ê¸° ````python import asyncio from pprint import pprint
+from biblebot import KbuAPI async def main(): resp = await
 KbuAPI.MainNotice.fetch(page=2) # ê³µì§ì¬í­ 2íì´ì§ result =
 KbuAPI.MainNotice.parse(resp) pprint(result.data) asyncio.run(main()) ````
 **Output:** ```json { "notice": [ { "seq": "3742", "title": "[ëíì ìì]
 2020íëë íê¸° íêµ­ì±ìëíêµ ëíì ì ìì ëª¨ì§",
 "author": "ì¥ì±í¬", "date": "2020-07-31", "url": "https://www.bible.ac.kr/
 ko/life/notice/view/46649?p=2" }, { "seq": "3741", "title": "[ê¸°ì´êµì¡ì]
 2020-2íê¸° ìê°ì ì²­ ê¸°ì´êµì¡ì, ìì´êµì¡ì¼í° ê³µì§ì¬í­
```

### Comparing `biblebot-0.4.2/biblebot/__init__.py` & `biblebot-0.4.3/biblebot/__init__.py`

 * *Files identical despite different names*

### Comparing `biblebot-0.4.2/biblebot/__version__.py` & `biblebot-0.4.3/biblebot/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,13 +9,13 @@
     "__copyright__",
     "__contributors__",
 )
 
 __title__ = "biblebot"
 __description__ = "Scraper for KBU students"
 __url__ = "https://github.com/rekyungmin/biblebot-scraper"
-__version__ = "0.4.2"
+__version__ = "0.4.3"
 __author__ = "Kyungmin Lee"
 __author_email__ = "rekyungmin@gmail.com"
 __license__ = "MIT"
 __copyright__ = "Copyright 2023 Kyungmin Lee"
 __contributors__ = "Yongki Kim <ygflove@likelion.org>",
```

### Comparing `biblebot-0.4.2/biblebot/api/__init__.py` & `biblebot-0.4.3/biblebot/api/__init__.py`

 * *Files identical despite different names*

### Comparing `biblebot-0.4.2/biblebot/api/_mileage.py` & `biblebot-0.4.3/biblebot/api/_mileage.py`

 * *Files identical despite different names*

### Comparing `biblebot-0.4.2/biblebot/api/base.py` & `biblebot-0.4.3/biblebot/api/base.py`

 * *Files identical despite different names*

### Comparing `biblebot-0.4.2/biblebot/api/common.py` & `biblebot-0.4.3/biblebot/api/common.py`

 * *Files identical despite different names*

### Comparing `biblebot-0.4.2/biblebot/api/intranet.py` & `biblebot-0.4.3/biblebot/api/intranet.py`

 * *Files identical despite different names*

### Comparing `biblebot-0.4.2/biblebot/api/kbu.py` & `biblebot-0.4.3/biblebot/api/kbu.py`

 * *Files identical despite different names*

### Comparing `biblebot-0.4.2/biblebot/api/library.py` & `biblebot-0.4.3/biblebot/api/library.py`

 * *Files identical despite different names*

### Comparing `biblebot-0.4.2/biblebot/api/lms.py` & `biblebot-0.4.3/biblebot/api/lms.py`

 * *Files identical despite different names*

### Comparing `biblebot-0.4.2/biblebot/api/mileage.py` & `biblebot-0.4.3/biblebot/api/mileage.py`

 * *Files identical despite different names*

### Comparing `biblebot-0.4.2/biblebot/exceptions.py` & `biblebot-0.4.3/biblebot/exceptions.py`

 * *Files identical despite different names*

### Comparing `biblebot-0.4.2/biblebot/reqeust/aiohttp_conn.py` & `biblebot-0.4.3/biblebot/reqeust/aiohttp_conn.py`

 * *Files identical despite different names*

### Comparing `biblebot-0.4.2/biblebot/reqeust/base.py` & `biblebot-0.4.3/biblebot/reqeust/base.py`

 * *Files identical despite different names*

### Comparing `biblebot-0.4.2/biblebot/reqeust/requests_conn.py` & `biblebot-0.4.3/biblebot/reqeust/requests_conn.py`

 * *Files identical despite different names*

### Comparing `biblebot-0.4.2/biblebot.egg-info/PKG-INFO` & `biblebot-0.4.3/biblebot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biblebot
-Version: 0.4.2
+Version: 0.4.3
 Summary: Scraper for KBU students
 Home-page: https://github.com/rekyungmin/biblebot-scraper
 Author: Kyungmin Lee
 Author-email: rekyungmin@gmail.com
 Maintainer: Kyungmin Lee <rekyungmin@gmail.com>, Yongki Kim <ygflove@likelion.org>
 License: UNKNOWN
 Platform: UNKNOWN
@@ -22,16 +22,14 @@
 <p align="center">
 <a href="https://www.python.org/downloads/release/python-370/"><img alt="Python" src="https://img.shields.io/badge/python-3.7-blue?logo=python&logoColor=white"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 </p>
 
 성서봇 스크래이퍼는 한국성서대학교와 연관된 정보를 수집할 수 있는 파이썬 패키지입니다.
 
-이 패키지를 바탕으로, **성서봇** 모바일 애플리케이션([Android](https://play.google.com/store/apps/details?id=com.blogspot.ramming125.kbubot&hl=ko))이 한국성서대학교학생들에게 2018년부터 실서비스 되고 있습니다.
-
 이 패키지는 다섯 가지 웹사이트에 대한 스크래이퍼를 제공합니다.
 
 1. [한국성서대학교 인트라넷](https://kbuis.bible.ac.kr/) 스크래이퍼  
 2. [한국성서대학교 LMS](https://lms.bible.ac.kr/) 스크래이퍼
 3. [한국성서대학교 홈페이지](https://www.bible.ac.kr/) 스크래이퍼  
 4. [OKPOS 마일리지 시스템](https://asp.netusys.com/) 스크래이퍼  
 5. [한국성서대학교 도서관](https://lib.bible.ac.kr/) 스크래이퍼
```

#### html2text {}

```diff
@@ -1,41 +1,38 @@
-Metadata-Version: 2.1 Name: biblebot Version: 0.4.2 Summary: Scraper for KBU
+Metadata-Version: 2.1 Name: biblebot Version: 0.4.3 Summary: Scraper for KBU
 students Home-page: https://github.com/rekyungmin/biblebot-scraper Author:
 Kyungmin Lee Author-email: rekyungmin@gmail.com Maintainer: Kyungmin Lee
 gmail.com>, Yongki Kim
 likelion.org> License: UNKNOWN Platform: UNKNOWN Classifier: License :: OSI
 Approved :: MIT License Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Requires-Python:
 >=3.7 Description-Content-Type: text/markdown Provides-Extra: http License-
 File: LICENSE
                         ****** Biblebot Scraper ******
                          [Python] [Code_style:_black]
 ì±ìë´ ì¤í¬ëì´í¼ë íêµ­ì±ìëíêµì ì°ê´ë ì ë³´ë¥¼
-ìì§í  ì ìë íì´ì¬ í¨í¤ì§ìëë¤. ì´ í¨í¤ì§ë¥¼
-ë°íì¼ë¡, **ì±ìë´** ëª¨ë°ì¼ ì íë¦¬ì¼ì´ì([Android](https://
-play.google.com/store/apps/details?id=com.blogspot.ramming125.kbubot&hl=ko))ì´
-íêµ­ì±ìëíêµíìë¤ìê² 2018ëë¶í° ì¤ìë¹ì¤ ëê³ 
-ììµëë¤. ì´ í¨í¤ì§ë ë¤ì¯ ê°ì§ ì¹ì¬ì´í¸ì ëí
-ì¤í¬ëì´í¼ë¥¼ ì ê³µí©ëë¤. 1. [íêµ­ì±ìëíêµ ì¸í¸ë¼ë·]
-(https://kbuis.bible.ac.kr/) ì¤í¬ëì´í¼ 2. [íêµ­ì±ìëíêµ LMS]
-(https://lms.bible.ac.kr/) ì¤í¬ëì´í¼ 3. [íêµ­ì±ìëíêµ
-ííì´ì§](https://www.bible.ac.kr/) ì¤í¬ëì´í¼ 4. [OKPOS ë§ì¼ë¦¬ì§
-ìì¤í](https://asp.netusys.com/) ì¤í¬ëì´í¼ 5. [íêµ­ì±ìëíêµ
-ëìê´](https://lib.bible.ac.kr/) ì¤í¬ëì´í¼ ## Installation ``` $ pip
-install 'biblebot[http]' ``` ## Requirements - `beautifulsoup4`: htmlê³¼ xml
-ìì ë°ì´í°ë¥¼ ì¶ì¶íê¸° ìí´ ì¬ì©í©ëë¤. - `aiohttp`: HTTP
-ìì²­ì ìí´ ì¬ì©í©ëë¤. (OPTIONAL) HTTP ìì²­ì ìí´ HTTP ìì²­
-í¨í¤ì§ê° íìí©ëë¤. `aiohttp` ëë `requests` í¨í¤ì§ê°
-ì¡´ì¬í  ê²½ì° ìëì¼ë¡ ì¸ìíì¬ ì¬ì©í©ëë¤. ê·¸ ì¸ì HTTP
-ìì²­ í¨í¤ì§ë¥¼ ì´ì©íê³  ì¶ë¤ë©´ `BaseRequest` ì¶ìí´ëì¤ë¥¼
-ììë°ì êµ¬íí ë¤, `HTTPClient.set`ì ì´ì©íì¬ ë±ë¡í´
-ì¬ì©í  ì ììµëë¤. ## ð Documentation [APIs document](docs/APIs.md)
-## Get started ### ê³µì§ì¬í­ ê°ì ¸ì¤ê¸° ````python import asyncio from
-pprint import pprint from biblebot import KbuAPI async def main(): resp = await
+ìì§í  ì ìë íì´ì¬ í¨í¤ì§ìëë¤. ì´ í¨í¤ì§ë ë¤ì¯
+ê°ì§ ì¹ì¬ì´í¸ì ëí ì¤í¬ëì´í¼ë¥¼ ì ê³µí©ëë¤. 1.
+[íêµ­ì±ìëíêµ ì¸í¸ë¼ë·](https://kbuis.bible.ac.kr/
+) ì¤í¬ëì´í¼ 2. [íêµ­ì±ìëíêµ LMS](https://lms.bible.ac.kr/
+) ì¤í¬ëì´í¼ 3. [íêµ­ì±ìëíêµ ííì´ì§](https://
+www.bible.ac.kr/) ì¤í¬ëì´í¼ 4. [OKPOS ë§ì¼ë¦¬ì§ ìì¤í](https://
+asp.netusys.com/) ì¤í¬ëì´í¼ 5. [íêµ­ì±ìëíêµ ëìê´](https://
+lib.bible.ac.kr/) ì¤í¬ëì´í¼ ## Installation ``` $ pip install 'biblebot
+[http]' ``` ## Requirements - `beautifulsoup4`: htmlê³¼ xml ìì ë°ì´í°ë¥¼
+ì¶ì¶íê¸° ìí´ ì¬ì©í©ëë¤. - `aiohttp`: HTTP ìì²­ì ìí´
+ì¬ì©í©ëë¤. (OPTIONAL) HTTP ìì²­ì ìí´ HTTP ìì²­ í¨í¤ì§ê°
+íìí©ëë¤. `aiohttp` ëë `requests` í¨í¤ì§ê° ì¡´ì¬í  ê²½ì°
+ìëì¼ë¡ ì¸ìíì¬ ì¬ì©í©ëë¤. ê·¸ ì¸ì HTTP ìì²­ í¨í¤ì§ë¥¼
+ì´ì©íê³  ì¶ë¤ë©´ `BaseRequest` ì¶ìí´ëì¤ë¥¼ ììë°ì êµ¬íí
+ë¤, `HTTPClient.set`ì ì´ì©íì¬ ë±ë¡í´ ì¬ì©í  ì ììµëë¤. ##
+ð Documentation [APIs document](docs/APIs.md) ## Get started ###
+ê³µì§ì¬í­ ê°ì ¸ì¤ê¸° ````python import asyncio from pprint import pprint
+from biblebot import KbuAPI async def main(): resp = await
 KbuAPI.MainNotice.fetch(page=2) # ê³µì§ì¬í­ 2íì´ì§ result =
 KbuAPI.MainNotice.parse(resp) pprint(result.data) asyncio.run(main()) ````
 **Output:** ```json { "notice": [ { "seq": "3742", "title": "[ëíì ìì]
 2020íëë íê¸° íêµ­ì±ìëíêµ ëíì ì ìì ëª¨ì§",
 "author": "ì¥ì±í¬", "date": "2020-07-31", "url": "https://www.bible.ac.kr/
 ko/life/notice/view/46649?p=2" }, { "seq": "3741", "title": "[ê¸°ì´êµì¡ì]
 2020-2íê¸° ìê°ì ì²­ ê¸°ì´êµì¡ì, ìì´êµì¡ì¼í° ê³µì§ì¬í­
```

### Comparing `biblebot-0.4.2/biblebot.egg-info/SOURCES.txt` & `biblebot-0.4.3/biblebot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biblebot-0.4.2/setup.py` & `biblebot-0.4.3/setup.py`

 * *Files identical despite different names*

