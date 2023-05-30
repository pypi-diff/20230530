# Comparing `tmp/duckduckgo_search-3.6.0.tar.gz` & `tmp/duckduckgo_search-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckduckgo_search-3.6.0.tar", last modified: Sat May 27 20:49:17 2023, max compression
+gzip compressed data, was "duckduckgo_search-3.7.0.tar", last modified: Tue May 30 13:50:51 2023, max compression
```

## Comparing `duckduckgo_search-3.6.0.tar` & `duckduckgo_search-3.7.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 20:49:17.845033 duckduckgo_search-3.6.0/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-05-27 20:48:59.000000 duckduckgo_search-3.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    15018 2023-05-27 20:49:17.845033 duckduckgo_search-3.6.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    13903 2023-05-27 20:48:59.000000 duckduckgo_search-3.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 20:49:17.845033 duckduckgo_search-3.6.0/duckduckgo_search/
--rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-05-27 20:48:59.000000 duckduckgo_search-3.6.0/duckduckgo_search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-05-27 20:48:59.000000 duckduckgo_search-3.6.0/duckduckgo_search/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16030 2023-05-27 20:48:59.000000 duckduckgo_search-3.6.0/duckduckgo_search/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-27 20:48:59.000000 duckduckgo_search-3.6.0/duckduckgo_search/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    30492 2023-05-27 20:48:59.000000 duckduckgo_search-3.6.0/duckduckgo_search/duckduckgo_search.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-05-27 20:48:59.000000 duckduckgo_search-3.6.0/duckduckgo_search/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 20:49:17.845033 duckduckgo_search-3.6.0/duckduckgo_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15018 2023-05-27 20:49:17.000000 duckduckgo_search-3.6.0/duckduckgo_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-27 20:49:17.000000 duckduckgo_search-3.6.0/duckduckgo_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 20:49:17.000000 duckduckgo_search-3.6.0/duckduckgo_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-27 20:49:17.000000 duckduckgo_search-3.6.0/duckduckgo_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-27 20:49:17.000000 duckduckgo_search-3.6.0/duckduckgo_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-27 20:49:17.000000 duckduckgo_search-3.6.0/duckduckgo_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-05-27 20:48:59.000000 duckduckgo_search-3.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 20:49:17.845033 duckduckgo_search-3.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 20:49:17.845033 duckduckgo_search-3.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-05-27 20:48:59.000000 duckduckgo_search-3.6.0/tests/test_duckduckgo_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:50:51.841500 duckduckgo_search-3.7.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-05-30 13:50:33.000000 duckduckgo_search-3.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14816 2023-05-30 13:50:51.841500 duckduckgo_search-3.7.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13701 2023-05-30 13:50:33.000000 duckduckgo_search-3.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:50:51.841500 duckduckgo_search-3.7.0/duckduckgo_search/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-05-30 13:50:33.000000 duckduckgo_search-3.7.0/duckduckgo_search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-05-30 13:50:33.000000 duckduckgo_search-3.7.0/duckduckgo_search/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16033 2023-05-30 13:50:33.000000 duckduckgo_search-3.7.0/duckduckgo_search/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-05-30 13:50:33.000000 duckduckgo_search-3.7.0/duckduckgo_search/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32023 2023-05-30 13:50:33.000000 duckduckgo_search-3.7.0/duckduckgo_search/duckduckgo_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-05-30 13:50:33.000000 duckduckgo_search-3.7.0/duckduckgo_search/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:50:51.841500 duckduckgo_search-3.7.0/duckduckgo_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14816 2023-05-30 13:50:51.000000 duckduckgo_search-3.7.0/duckduckgo_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-30 13:50:51.000000 duckduckgo_search-3.7.0/duckduckgo_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:50:51.000000 duckduckgo_search-3.7.0/duckduckgo_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-30 13:50:51.000000 duckduckgo_search-3.7.0/duckduckgo_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-30 13:50:51.000000 duckduckgo_search-3.7.0/duckduckgo_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-30 13:50:51.000000 duckduckgo_search-3.7.0/duckduckgo_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-30 13:50:33.000000 duckduckgo_search-3.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 13:50:51.841500 duckduckgo_search-3.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:50:51.841500 duckduckgo_search-3.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-05-30 13:50:33.000000 duckduckgo_search-3.7.0/tests/test_duckduckgo_search.py
```

### Comparing `duckduckgo_search-3.6.0/LICENSE.md` & `duckduckgo_search-3.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.6.0/PKG-INFO` & `duckduckgo_search-3.7.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo_search
-Version: 3.6.0
+Version: 3.7.0
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -159,40 +159,33 @@
     wt-wt for No region
 ___
 </details>
 
 [Go To TOP](#TOP)
 
 ## Using proxy
-If you send too many requests the site blocks ip for up to one minute and DDGS will raise an exception 
-`requests.exceptions.HTTPError: 418 Client Error:  for url: https://duckduckgo.com/`.
-In this case, you need repeat again after a while or to use a proxy ([httpx documentation](https://www.python-httpx.org/advanced)).
+If you send too many requests the site blocks ip for up to one minute and DDGS will raise an exception.
+In this case, you need repeat again after a while or to use a proxy ([documentation](https://www.python-httpx.org/advanced/#http-proxying)).
 You can set a timeout if the proxy takes a long time to respond (default timeout=10).
 
 *1. The easiest way. Launch the Tor Browser*
 ```python3
 from duckduckgo_search import DDGS
 
-proxies = {
-    "all://": "socks5h://localhost:9150",
-}
-ddgs_text_gen = DDGS(proxies=proxies, timeout=20).text("something you need")
-for r in ddgs_text_gen:
-    print(r)
+with DDGS(proxies="socks5://localhost:9150", timeout=20) as ddgs:
+    for r in ddgs.text("something you need"):
+        print(r)
 ```
 *2. Use any proxy server* (*example with [iproyal residential proxies](https://iproyal.com?r=residential_proxies)*)
 ```python3
 from duckduckgo_search import DDGS
 
-proxies = {
-    "all://": "https://user:password@geo.iproyal.com:32325",
-}
-ddgs_text_gen = DDGS(proxies=proxies, timeout=20).text("something you need")
-for r in ddgs_text_gen:
-    print(r)
+with DDGS(proxies="socks5://user:password@geo.iproyal.com:32325", timeout=20) as ddgs:
+    for r in ddgs.text("something you need"):
+        print(r)
 ```
 
 [Go To TOP](#TOP)
 
 ## 1. text() - text search by by duckduckgo.com
 ```python
 def text(
@@ -218,33 +211,30 @@
 
     """
 ```
 ***Example***
 ```python
 from duckduckgo_search import DDGS
 
-ddgs = DDGS()
-
-keywords = 'live free or die'
-ddgs_text_gen = ddgs.text(keywords, region='wt-wt', safesearch='Off', timelimit='y')
-for r in ddgs_text_gen:
-    print(r)
+with DDGS() as ddgs:
+    for r in ddgs.text('live free or die', region='wt-wt', safesearch='Off', timelimit='y'):
+        print(r)
 
 # Searching for pdf files
-keywords = 'russia filetype:pdf'
-ddgs_text_gen = ddgs.text(keywords, region='wt-wt', safesearch='Off', timelimit='y')
-for r in ddgs_text_gen:
-    print(r)
+with DDGS() as ddgs:
+    for r in ddgs.text('russia filetype:pdf', region='wt-wt', safesearch='Off', timelimit='y'):
+        print(r)
 
 # Using lite backend and limit the number of results to 10
 from itertools import islice
 
-ddgs_text_gen = DDGS().text("notes from a dead house", backend="lite")
-for r in islice(ddgs_text_gen, 10):
-    print(r)
+with DDGS() as ddgs:
+    ddgs_gen = ddgs.text("notes from a dead house", backend="lite")
+    for r in islice(ddgs_gen, 10):
+        print(r)
 ```
 
 
 [Go To TOP](#TOP)
 
 ## 2. answers() - instant answers by duckduckgo.com
 
@@ -260,20 +250,17 @@
 
         """
 ```
 ***Example***
 ```python
 from duckduckgo_search import DDGS
 
-ddgs = DDGS()
-
-keywords = 'sun'
-ddgs_answers_gen = ddgs.answers(keywords)
-for r in ddgs_answers_gen:
-    print(r)
+with DDGS() as ddgs:
+    for r in ddgs.answers("sun"):
+        print(r)
 ```
 
 [Go To TOP](#TOP)
 
 ## 3. images() - image search by duckduckgo.com
 
 ```python
@@ -311,29 +298,28 @@
 
     """
 ```
 ***Example***
 ```python
 from duckduckgo_search import DDGS
 
-ddgs = DDGS()
-
-keywords = 'butterfly'
-ddgs_images_gen = ddgs.images(
-    keywords,
-    region="wt-wt",
-    safesearch="Off",
-    size=None,
-    color="Monochrome",
-    type_image=None,
-    layout=None,
-    license_image=None,
-)
-for r in ddgs_images_gen:
-    print(r)
+with DDGS() as ddgs:
+    keywords = 'butterfly'
+    ddgs_images_gen = ddgs.images(
+      keywords,
+      region="wt-wt",
+      safesearch="Off",
+      size=None,
+      color="Monochrome",
+      type_image=None,
+      layout=None,
+      license_image=None,
+    )
+    for r in ddgs_images_gen:
+        print(r)
 ```
 
 [Go To TOP](#TOP)
 
 ## 4. videos() - video search by duckduckgo.com
 
 ```python
@@ -362,27 +348,26 @@
 
     """
 ```
 ***Example***
 ```python
 from duckduckgo_search import DDGS
 
-ddgs = DDGS()
-
-keywords = 'tesla'
-ddgs_videos_gen = ddgs.videos(
-    keywords,
-    region="wt-wt",
-    safesearch="Off",
-    timelimit="w",
-    resolution="high",
-    duration="medium",
-)
-for r in ddgs_videos_gen:
-    print(r)
+with DDGS() as ddgs:
+    keywords = 'tesla'
+    ddgs_videos_gen = ddgs.videos(
+      keywords,
+      region="wt-wt",
+      safesearch="Off",
+      timelimit="w",
+      resolution="high",
+      duration="medium",
+    )
+    for r in ddgs_videos_gen:
+        print(r)
 ```
 
 
 [Go To TOP](#TOP)
 
 ## 5. news() - news search by duckduckgo.com
 
@@ -406,25 +391,24 @@
 
     """
 ```
 ***Example***
 ```python
 from duckduckgo_search import DDGS
 
-ddgs = DDGS()
-
-keywords = 'How soon the sun will die'
-ddgs_news_gen = ddgs.news(
-    keywords,
-    region="wt-wt",
-    safesearch="Off",
-    timelimit="m",
-)
-for r in ddgs_news_gen:
-    print(r)
+with DDGS() as ddgs:
+    keywords = 'How soon the sun will die'
+    ddgs_news_gen = ddgs.news(
+      keywords,
+      region="wt-wt",
+      safesearch="Off",
+      timelimit="m",
+    )
+    for r in ddgs_news_gen:
+        print(r)
 ```
 
 [Go To TOP](#TOP)
 
 ## 6. maps() - map search by duckduckgo.com
 
 ```python
@@ -462,23 +446,17 @@
 
         """
 ```
 ***Example***
 ```python
 from duckduckgo_search import DDGS
 
-ddgs = DDGS()
-
-keywords = 'school'
-ddgs_maps_gen = ddgs.maps(
-    keywords,
-    place="Uganda",
-)
-for r in ddgs_maps_gen:
-    print(r)
+with DDGS() as ddgs:
+    for r in ddgs.maps("school", place="Uganda"):
+        print(r)
 ```
 
 [Go To TOP](#TOP)
 
 ## 7. translate() - translation by duckduckgo.com
 
 ```python
@@ -499,19 +477,18 @@
         dict with translated keywords.
     """
 ```
 ***Example***
 ```python
 from duckduckgo_search import DDGS
 
-ddgs = DDGS()
-
-keywords = 'school'
-r = ddgs.translate(keywords, to="de")
-print(r)
+with DDGS() as ddgs:
+    keywords = 'school'
+    r = ddgs.translate(keywords, to="de")
+    print(r)
 ```
 
 [Go To TOP](#TOP)
 
 
 ## 8. suggestions() - suggestions by duckduckgo.com
 
@@ -530,16 +507,13 @@
         dict with suggestions results.
     """
 ```
 ***Example***
 ```python3
 from duckduckgo_search import DDGS
 
-ddgs = DDGS()
-
-keywords = 'fly'
-ddgs_suggestions_gen = ddgs.suggestions(keywords)
-for r in ddgs_suggestions_gen:
-    print(r)
+with DDGS() as ddgs:
+    for r in ddgs.suggestions("fly)
+        print(r)
 ```
 
 [Go To TOP](#TOP)
```

### Comparing `duckduckgo_search-3.6.0/README.md` & `duckduckgo_search-3.7.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -134,40 +134,33 @@
     wt-wt for No region
 ___
 </details>
 
 [Go To TOP](#TOP)
 
 ## Using proxy
-If you send too many requests the site blocks ip for up to one minute and DDGS will raise an exception 
-`requests.exceptions.HTTPError: 418 Client Error:  for url: https://duckduckgo.com/`.
-In this case, you need repeat again after a while or to use a proxy ([httpx documentation](https://www.python-httpx.org/advanced)).
+If you send too many requests the site blocks ip for up to one minute and DDGS will raise an exception.
+In this case, you need repeat again after a while or to use a proxy ([documentation](https://www.python-httpx.org/advanced/#http-proxying)).
 You can set a timeout if the proxy takes a long time to respond (default timeout=10).
 
 *1. The easiest way. Launch the Tor Browser*
 ```python3
 from duckduckgo_search import DDGS
 
-proxies = {
-    "all://": "socks5h://localhost:9150",
-}
-ddgs_text_gen = DDGS(proxies=proxies, timeout=20).text("something you need")
-for r in ddgs_text_gen:
-    print(r)
+with DDGS(proxies="socks5://localhost:9150", timeout=20) as ddgs:
+    for r in ddgs.text("something you need"):
+        print(r)
 ```
 *2. Use any proxy server* (*example with [iproyal residential proxies](https://iproyal.com?r=residential_proxies)*)
 ```python3
 from duckduckgo_search import DDGS
 
-proxies = {
-    "all://": "https://user:password@geo.iproyal.com:32325",
-}
-ddgs_text_gen = DDGS(proxies=proxies, timeout=20).text("something you need")
-for r in ddgs_text_gen:
-    print(r)
+with DDGS(proxies="socks5://user:password@geo.iproyal.com:32325", timeout=20) as ddgs:
+    for r in ddgs.text("something you need"):
+        print(r)
 ```
 
 [Go To TOP](#TOP)
 
 ## 1. text() - text search by by duckduckgo.com
 ```python
 def text(
@@ -193,33 +186,30 @@
 
     """
 ```
 ***Example***
 ```python
 from duckduckgo_search import DDGS
 
-ddgs = DDGS()
-
-keywords = 'live free or die'
-ddgs_text_gen = ddgs.text(keywords, region='wt-wt', safesearch='Off', timelimit='y')
-for r in ddgs_text_gen:
-    print(r)
+with DDGS() as ddgs:
+    for r in ddgs.text('live free or die', region='wt-wt', safesearch='Off', timelimit='y'):
+        print(r)
 
 # Searching for pdf files
-keywords = 'russia filetype:pdf'
-ddgs_text_gen = ddgs.text(keywords, region='wt-wt', safesearch='Off', timelimit='y')
-for r in ddgs_text_gen:
-    print(r)
+with DDGS() as ddgs:
+    for r in ddgs.text('russia filetype:pdf', region='wt-wt', safesearch='Off', timelimit='y'):
+        print(r)
 
 # Using lite backend and limit the number of results to 10
 from itertools import islice
 
-ddgs_text_gen = DDGS().text("notes from a dead house", backend="lite")
-for r in islice(ddgs_text_gen, 10):
-    print(r)
+with DDGS() as ddgs:
+    ddgs_gen = ddgs.text("notes from a dead house", backend="lite")
+    for r in islice(ddgs_gen, 10):
+        print(r)
 ```
 
 
 [Go To TOP](#TOP)
 
 ## 2. answers() - instant answers by duckduckgo.com
 
@@ -235,20 +225,17 @@
 
         """
 ```
 ***Example***
 ```python
 from duckduckgo_search import DDGS
 
-ddgs = DDGS()
-
-keywords = 'sun'
-ddgs_answers_gen = ddgs.answers(keywords)
-for r in ddgs_answers_gen:
-    print(r)
+with DDGS() as ddgs:
+    for r in ddgs.answers("sun"):
+        print(r)
 ```
 
 [Go To TOP](#TOP)
 
 ## 3. images() - image search by duckduckgo.com
 
 ```python
@@ -286,29 +273,28 @@
 
     """
 ```
 ***Example***
 ```python
 from duckduckgo_search import DDGS
 
-ddgs = DDGS()
-
-keywords = 'butterfly'
-ddgs_images_gen = ddgs.images(
-    keywords,
-    region="wt-wt",
-    safesearch="Off",
-    size=None,
-    color="Monochrome",
-    type_image=None,
-    layout=None,
-    license_image=None,
-)
-for r in ddgs_images_gen:
-    print(r)
+with DDGS() as ddgs:
+    keywords = 'butterfly'
+    ddgs_images_gen = ddgs.images(
+      keywords,
+      region="wt-wt",
+      safesearch="Off",
+      size=None,
+      color="Monochrome",
+      type_image=None,
+      layout=None,
+      license_image=None,
+    )
+    for r in ddgs_images_gen:
+        print(r)
 ```
 
 [Go To TOP](#TOP)
 
 ## 4. videos() - video search by duckduckgo.com
 
 ```python
@@ -337,27 +323,26 @@
 
     """
 ```
 ***Example***
 ```python
 from duckduckgo_search import DDGS
 
-ddgs = DDGS()
-
-keywords = 'tesla'
-ddgs_videos_gen = ddgs.videos(
-    keywords,
-    region="wt-wt",
-    safesearch="Off",
-    timelimit="w",
-    resolution="high",
-    duration="medium",
-)
-for r in ddgs_videos_gen:
-    print(r)
+with DDGS() as ddgs:
+    keywords = 'tesla'
+    ddgs_videos_gen = ddgs.videos(
+      keywords,
+      region="wt-wt",
+      safesearch="Off",
+      timelimit="w",
+      resolution="high",
+      duration="medium",
+    )
+    for r in ddgs_videos_gen:
+        print(r)
 ```
 
 
 [Go To TOP](#TOP)
 
 ## 5. news() - news search by duckduckgo.com
 
@@ -381,25 +366,24 @@
 
     """
 ```
 ***Example***
 ```python
 from duckduckgo_search import DDGS
 
-ddgs = DDGS()
-
-keywords = 'How soon the sun will die'
-ddgs_news_gen = ddgs.news(
-    keywords,
-    region="wt-wt",
-    safesearch="Off",
-    timelimit="m",
-)
-for r in ddgs_news_gen:
-    print(r)
+with DDGS() as ddgs:
+    keywords = 'How soon the sun will die'
+    ddgs_news_gen = ddgs.news(
+      keywords,
+      region="wt-wt",
+      safesearch="Off",
+      timelimit="m",
+    )
+    for r in ddgs_news_gen:
+        print(r)
 ```
 
 [Go To TOP](#TOP)
 
 ## 6. maps() - map search by duckduckgo.com
 
 ```python
@@ -437,23 +421,17 @@
 
         """
 ```
 ***Example***
 ```python
 from duckduckgo_search import DDGS
 
-ddgs = DDGS()
-
-keywords = 'school'
-ddgs_maps_gen = ddgs.maps(
-    keywords,
-    place="Uganda",
-)
-for r in ddgs_maps_gen:
-    print(r)
+with DDGS() as ddgs:
+    for r in ddgs.maps("school", place="Uganda"):
+        print(r)
 ```
 
 [Go To TOP](#TOP)
 
 ## 7. translate() - translation by duckduckgo.com
 
 ```python
@@ -474,19 +452,18 @@
         dict with translated keywords.
     """
 ```
 ***Example***
 ```python
 from duckduckgo_search import DDGS
 
-ddgs = DDGS()
-
-keywords = 'school'
-r = ddgs.translate(keywords, to="de")
-print(r)
+with DDGS() as ddgs:
+    keywords = 'school'
+    r = ddgs.translate(keywords, to="de")
+    print(r)
 ```
 
 [Go To TOP](#TOP)
 
 
 ## 8. suggestions() - suggestions by duckduckgo.com
 
@@ -505,16 +482,13 @@
         dict with suggestions results.
     """
 ```
 ***Example***
 ```python3
 from duckduckgo_search import DDGS
 
-ddgs = DDGS()
-
-keywords = 'fly'
-ddgs_suggestions_gen = ddgs.suggestions(keywords)
-for r in ddgs_suggestions_gen:
-    print(r)
+with DDGS() as ddgs:
+    for r in ddgs.suggestions("fly)
+        print(r)
 ```
 
 [Go To TOP](#TOP)
```

### Comparing `duckduckgo_search-3.6.0/duckduckgo_search/__init__.py` & `duckduckgo_search-3.7.0/duckduckgo_search/__init__.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.6.0/duckduckgo_search/cli.py` & `duckduckgo_search-3.7.0/duckduckgo_search/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import csv
 import json
 import logging
 import os
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from datetime import datetime
-from shutil import copyfileobj
+from random import choice
 from urllib.parse import unquote
 
 import click
 import httpx
 
 # isort: off
-from .duckduckgo_search import DDGS
+from .duckduckgo_search import DDGS, USERAGENTS
 from .version import __version__
 
 # isort: on
 
 logger = logging.getLogger(__name__)
 
 COLORS = {
@@ -73,31 +73,33 @@
                     text = v
                 click.secho(f"{k:<12}{text}", bg="black", fg=COLORS[j], overline=True)
             input()
 
 
 def sanitize_keywords(keywords):
     keywords = (
-        keywords.replace(" filetype:", "_")
+        keywords.replace("filetype", "")
+        .replace(":", "")
         .replace('"', "'")
-        .replace("site:", "")
+        .replace("site", "")
         .replace(" ", "_")
         .replace("/", "_")
         .replace("\\", "_")
+        .replace(" ", "")
     )
     return keywords
 
 
 def download_file(url, dir_path, filename):
     headers = {
-        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; rv:102.0) Gecko/20100101 Firefox/102.0",
+        "User-Agent": choice(USERAGENTS),
     }
     try:
-        with open(os.path.join(dir_path, filename), "wb") as file:
-            with httpx.stream("GET", url, headers=headers) as resp:
+        with httpx.stream("GET", url, headers=headers) as resp:
+            with open(os.path.join(dir_path, filename), "wb") as file:
                 for chunk in resp.iter_bytes():
                     file.write(chunk)
         logger.info(f"File downloaded {url}")
     except Exception as ex:
         logger.debug(f"download_file url={url} {type(ex).__name__} {ex}")
```

### Comparing `duckduckgo_search-3.6.0/duckduckgo_search/compat.py` & `duckduckgo_search-3.7.0/duckduckgo_search/compat.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.6.0/duckduckgo_search/duckduckgo_search.py` & `duckduckgo_search-3.7.0/duckduckgo_search/duckduckgo_search.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,30 +2,45 @@
 import re
 from collections import deque
 from dataclasses import dataclass
 from datetime import datetime
 from decimal import Decimal
 from html import unescape
 from itertools import cycle
+from random import choice
 from time import sleep
-from typing import Deque, Dict, Iterator, Optional, Set
+from typing import Deque, Dict, Iterator, Optional, Set, Union
 from urllib.parse import unquote
 
 import httpx
-import requests
 from lxml import html
 
 logger = logging.getLogger(__name__)
 
+REGEX_500_IN_URL = re.compile(r"[0-9]{3}-[0-9]{2}.js")
+REGEX_STRIP_TAGS = re.compile("<.*?>")
+
+USERAGENTS = [
+    "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36",
+    "Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36",
+    "Mozilla/5.0 (Windows NT 10.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36",
+    "Mozilla/5.0 (Macintosh; Intel Mac OS X 13_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36",
+    "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/113.0",
+    "Mozilla/5.0 (Macintosh; Intel Mac OS X 13.4; rv:109.0) Gecko/20100101 Firefox/113.0",
+    "Mozilla/5.0 (Macintosh; Intel Mac OS X 13_4) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/16.5 Safari/605.1.15",
+    "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36 Edg/113.0.1774.57",
+    "Mozilla/5.0 (Macintosh; Intel Mac OS X 13_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36 Edg/113.0.1774.57",
+    "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36 OPR/99.0.0.0",
+    "Mozilla/5.0 (Windows NT 10.0; WOW64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36 OPR/99.0.0.0",
+    "Mozilla/5.0 (Macintosh; Intel Mac OS X 13_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36 OPR/99.0.0.0",
+]
 HEADERS = {
-    "User-Agent": "Mozilla/5.0 (Windows NT 10.0; rv:102.0) Gecko/20100101 Firefox/102.0",
+    "User-Agent": choice(USERAGENTS),
     "Referer": "https://duckduckgo.com/",
 }
-REGEX_500_IN_URL = re.compile(r"[0-9]{3}-[0-9]{2}.js")
-REGEX_STRIP_TAGS = re.compile("<.*?>")
 
 
 @dataclass
 class MapsResult:
     title: Optional[str] = None
     address: Optional[str] = None
     country_code: Optional[str] = None
@@ -42,15 +57,15 @@
 
 class DDGS:
     """DuckDuckgo_search class to get search results from duckduckgo.com"""
 
     def __init__(
         self,
         headers: Optional[Dict[str, str]] = None,
-        proxies: Optional[Dict] = None,
+        proxies: Optional[Union[Dict, str]] = None,
         timeout: int = 10,
     ) -> None:
         self._client = httpx.Client(
             headers=headers if headers else HEADERS,
             proxies=proxies,
             timeout=timeout,
             http2=True,
@@ -63,15 +78,17 @@
         self._client.close()
 
     def _get_url(
         self, method: str, url: str, **kwargs
     ) -> Optional[httpx._models.Response]:
         for i in range(3):
             try:
-                resp = self._client.request(method, url, **kwargs)
+                resp = self._client.request(
+                    method, url, follow_redirects=True, **kwargs
+                )
                 if self._is_500_in_url(str(resp.url)) or resp.status_code == 202:
                     raise httpx._exceptions.HTTPError("")
                 resp.raise_for_status()
                 if resp.status_code == 200:
                     return resp
             except Exception as ex:
                 logger.warning(f"_get_url() {url} {type(ex).__name__} {ex}")
@@ -331,17 +348,17 @@
                     title = e.xpath(".//a//text()")[0]
                 elif i == 2:
                     body = e.xpath(".//td[@class='result-snippet']//text()")
                     body = "".join(body).strip()
                 elif i == 3:
                     result_exists = True
                     yield {
+                        "title": self._normalize(title),
                         "href": href,
-                        "title": title,
-                        "body": body,
+                        "body": self._normalize(body),
                     }
             if result_exists is False:
                 break
             sleep(0.75)
 
     def images(
         self,
@@ -664,17 +681,15 @@
 
         assert keywords, "keywords is mandatory"
 
         payload = {
             "q": keywords,
             "kl": region,
         }
-        resp = self._get_url(
-            "GET", "https://duckduckgo.com/ac", params=payload, follow_redirects=True
-        )
+        resp = self._get_url("GET", "https://duckduckgo.com/ac", params=payload)
         if resp is None:
             return None
         try:
             page_data = resp.json()
             for r in page_data:
                 yield r
         except Exception:
@@ -854,19 +869,21 @@
 
         vqd = self._get_vqd("translate")
         assert vqd, "error in getting vqd"
 
         payload = {
             "vqd": vqd,
             "query": "translate",
-            "from": from_,
             "to": to,
         }
+        if from_:
+            payload["from"] = from_
 
-        resp = requests.post(
+        resp = self._get_url(
+            "POST",
             "https://duckduckgo.com/translation.js",
             params=payload,
             data=keywords.encode(),
         )
         if resp is None:
             return None
         try:
```

### Comparing `duckduckgo_search-3.6.0/duckduckgo_search.egg-info/PKG-INFO` & `duckduckgo_search-3.7.0/duckduckgo_search.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo-search
-Version: 3.6.0
+Version: 3.7.0
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -159,40 +159,33 @@
     wt-wt for No region
 ___
 </details>
 
 [Go To TOP](#TOP)
 
 ## Using proxy
-If you send too many requests the site blocks ip for up to one minute and DDGS will raise an exception 
-`requests.exceptions.HTTPError: 418 Client Error:  for url: https://duckduckgo.com/`.
-In this case, you need repeat again after a while or to use a proxy ([httpx documentation](https://www.python-httpx.org/advanced)).
+If you send too many requests the site blocks ip for up to one minute and DDGS will raise an exception.
+In this case, you need repeat again after a while or to use a proxy ([documentation](https://www.python-httpx.org/advanced/#http-proxying)).
 You can set a timeout if the proxy takes a long time to respond (default timeout=10).
 
 *1. The easiest way. Launch the Tor Browser*
 ```python3
 from duckduckgo_search import DDGS
 
-proxies = {
-    "all://": "socks5h://localhost:9150",
-}
-ddgs_text_gen = DDGS(proxies=proxies, timeout=20).text("something you need")
-for r in ddgs_text_gen:
-    print(r)
+with DDGS(proxies="socks5://localhost:9150", timeout=20) as ddgs:
+    for r in ddgs.text("something you need"):
+        print(r)
 ```
 *2. Use any proxy server* (*example with [iproyal residential proxies](https://iproyal.com?r=residential_proxies)*)
 ```python3
 from duckduckgo_search import DDGS
 
-proxies = {
-    "all://": "https://user:password@geo.iproyal.com:32325",
-}
-ddgs_text_gen = DDGS(proxies=proxies, timeout=20).text("something you need")
-for r in ddgs_text_gen:
-    print(r)
+with DDGS(proxies="socks5://user:password@geo.iproyal.com:32325", timeout=20) as ddgs:
+    for r in ddgs.text("something you need"):
+        print(r)
 ```
 
 [Go To TOP](#TOP)
 
 ## 1. text() - text search by by duckduckgo.com
 ```python
 def text(
@@ -218,33 +211,30 @@
 
     """
 ```
 ***Example***
 ```python
 from duckduckgo_search import DDGS
 
-ddgs = DDGS()
-
-keywords = 'live free or die'
-ddgs_text_gen = ddgs.text(keywords, region='wt-wt', safesearch='Off', timelimit='y')
-for r in ddgs_text_gen:
-    print(r)
+with DDGS() as ddgs:
+    for r in ddgs.text('live free or die', region='wt-wt', safesearch='Off', timelimit='y'):
+        print(r)
 
 # Searching for pdf files
-keywords = 'russia filetype:pdf'
-ddgs_text_gen = ddgs.text(keywords, region='wt-wt', safesearch='Off', timelimit='y')
-for r in ddgs_text_gen:
-    print(r)
+with DDGS() as ddgs:
+    for r in ddgs.text('russia filetype:pdf', region='wt-wt', safesearch='Off', timelimit='y'):
+        print(r)
 
 # Using lite backend and limit the number of results to 10
 from itertools import islice
 
-ddgs_text_gen = DDGS().text("notes from a dead house", backend="lite")
-for r in islice(ddgs_text_gen, 10):
-    print(r)
+with DDGS() as ddgs:
+    ddgs_gen = ddgs.text("notes from a dead house", backend="lite")
+    for r in islice(ddgs_gen, 10):
+        print(r)
 ```
 
 
 [Go To TOP](#TOP)
 
 ## 2. answers() - instant answers by duckduckgo.com
 
@@ -260,20 +250,17 @@
 
         """
 ```
 ***Example***
 ```python
 from duckduckgo_search import DDGS
 
-ddgs = DDGS()
-
-keywords = 'sun'
-ddgs_answers_gen = ddgs.answers(keywords)
-for r in ddgs_answers_gen:
-    print(r)
+with DDGS() as ddgs:
+    for r in ddgs.answers("sun"):
+        print(r)
 ```
 
 [Go To TOP](#TOP)
 
 ## 3. images() - image search by duckduckgo.com
 
 ```python
@@ -311,29 +298,28 @@
 
     """
 ```
 ***Example***
 ```python
 from duckduckgo_search import DDGS
 
-ddgs = DDGS()
-
-keywords = 'butterfly'
-ddgs_images_gen = ddgs.images(
-    keywords,
-    region="wt-wt",
-    safesearch="Off",
-    size=None,
-    color="Monochrome",
-    type_image=None,
-    layout=None,
-    license_image=None,
-)
-for r in ddgs_images_gen:
-    print(r)
+with DDGS() as ddgs:
+    keywords = 'butterfly'
+    ddgs_images_gen = ddgs.images(
+      keywords,
+      region="wt-wt",
+      safesearch="Off",
+      size=None,
+      color="Monochrome",
+      type_image=None,
+      layout=None,
+      license_image=None,
+    )
+    for r in ddgs_images_gen:
+        print(r)
 ```
 
 [Go To TOP](#TOP)
 
 ## 4. videos() - video search by duckduckgo.com
 
 ```python
@@ -362,27 +348,26 @@
 
     """
 ```
 ***Example***
 ```python
 from duckduckgo_search import DDGS
 
-ddgs = DDGS()
-
-keywords = 'tesla'
-ddgs_videos_gen = ddgs.videos(
-    keywords,
-    region="wt-wt",
-    safesearch="Off",
-    timelimit="w",
-    resolution="high",
-    duration="medium",
-)
-for r in ddgs_videos_gen:
-    print(r)
+with DDGS() as ddgs:
+    keywords = 'tesla'
+    ddgs_videos_gen = ddgs.videos(
+      keywords,
+      region="wt-wt",
+      safesearch="Off",
+      timelimit="w",
+      resolution="high",
+      duration="medium",
+    )
+    for r in ddgs_videos_gen:
+        print(r)
 ```
 
 
 [Go To TOP](#TOP)
 
 ## 5. news() - news search by duckduckgo.com
 
@@ -406,25 +391,24 @@
 
     """
 ```
 ***Example***
 ```python
 from duckduckgo_search import DDGS
 
-ddgs = DDGS()
-
-keywords = 'How soon the sun will die'
-ddgs_news_gen = ddgs.news(
-    keywords,
-    region="wt-wt",
-    safesearch="Off",
-    timelimit="m",
-)
-for r in ddgs_news_gen:
-    print(r)
+with DDGS() as ddgs:
+    keywords = 'How soon the sun will die'
+    ddgs_news_gen = ddgs.news(
+      keywords,
+      region="wt-wt",
+      safesearch="Off",
+      timelimit="m",
+    )
+    for r in ddgs_news_gen:
+        print(r)
 ```
 
 [Go To TOP](#TOP)
 
 ## 6. maps() - map search by duckduckgo.com
 
 ```python
@@ -462,23 +446,17 @@
 
         """
 ```
 ***Example***
 ```python
 from duckduckgo_search import DDGS
 
-ddgs = DDGS()
-
-keywords = 'school'
-ddgs_maps_gen = ddgs.maps(
-    keywords,
-    place="Uganda",
-)
-for r in ddgs_maps_gen:
-    print(r)
+with DDGS() as ddgs:
+    for r in ddgs.maps("school", place="Uganda"):
+        print(r)
 ```
 
 [Go To TOP](#TOP)
 
 ## 7. translate() - translation by duckduckgo.com
 
 ```python
@@ -499,19 +477,18 @@
         dict with translated keywords.
     """
 ```
 ***Example***
 ```python
 from duckduckgo_search import DDGS
 
-ddgs = DDGS()
-
-keywords = 'school'
-r = ddgs.translate(keywords, to="de")
-print(r)
+with DDGS() as ddgs:
+    keywords = 'school'
+    r = ddgs.translate(keywords, to="de")
+    print(r)
 ```
 
 [Go To TOP](#TOP)
 
 
 ## 8. suggestions() - suggestions by duckduckgo.com
 
@@ -530,16 +507,13 @@
         dict with suggestions results.
     """
 ```
 ***Example***
 ```python3
 from duckduckgo_search import DDGS
 
-ddgs = DDGS()
-
-keywords = 'fly'
-ddgs_suggestions_gen = ddgs.suggestions(keywords)
-for r in ddgs_suggestions_gen:
-    print(r)
+with DDGS() as ddgs:
+    for r in ddgs.suggestions("fly)
+        print(r)
 ```
 
 [Go To TOP](#TOP)
```

### Comparing `duckduckgo_search-3.6.0/pyproject.toml` & `duckduckgo_search-3.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,15 @@
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Internet :: WWW/HTTP :: Indexing/Search",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
     "click>=8.1.3",
     "lxml>=4.9.2",
-    "httpx[http2]>=0.24.1",
-    "requests>=2.31.0",
+    "httpx[http2,socks]>=0.24.1",
 ]
 dynamic = ["version"]
 
 [project.urls]  # Optional
 "Homepage" = "https://github.com/deedy5/duckduckgo_search"
 
 [project.scripts]
```

### Comparing `duckduckgo_search-3.6.0/tests/test_duckduckgo_search.py` & `duckduckgo_search-3.7.0/tests/test_duckduckgo_search.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,126 +1,113 @@
 import os
 import shutil
+from itertools import islice
 
 from duckduckgo_search import DDGS
 from duckduckgo_search.cli import download_results, save_csv, save_json
 
 
 def test_text():
-    results_gen = DDGS().text("cat")
-    counter = 0
-    for i, x in enumerate(results_gen):
-        counter += 1
-        if i >= 25:
-            break
-    assert counter >= 25
+    with DDGS() as ddgs:
+        ddgs_gen = ddgs.text("cat")
+        results = [x for x in islice(ddgs_gen, 25)]
+        assert len(results) >= 20
+
+
+def test_text_html():
+    with DDGS() as ddgs:
+        ddgs_gen = ddgs.text("eagle", backend="html")
+        results = [x for x in islice(ddgs_gen, 25)]
+        assert len(results) >= 20
+
+
+def test_text_lite():
+    with DDGS() as ddgs:
+        ddgs_gen = ddgs.text("dog", backend="lite")
+        results = [x for x in islice(ddgs_gen, 25)]
+        assert len(results) >= 20
 
 
 def test_images():
-    results_gen = DDGS().images("cat")
-    counter = 0
-    for i, x in enumerate(results_gen):
-        counter += 1
-        if i >= 150:
-            break
-    assert counter >= 150
+    with DDGS() as ddgs:
+        ddgs_gen = ddgs.images("airplane")
+        results = [x for x in islice(ddgs_gen, 150)]
+        assert len(results) >= 140
 
 
 def test_videos():
-    results_gen = DDGS().videos("cat")
-    counter = 0
-    for i, x in enumerate(results_gen):
-        counter += 1
-        if i >= 40:
-            break
-    assert counter >= 40
+    with DDGS() as ddgs:
+        ddgs_gen = ddgs.videos("sea")
+        results = [x for x in islice(ddgs_gen, 50)]
+        assert len(results) >= 40
 
 
 def test_news():
-    results_gen = DDGS().news("cat")
-    counter = 0
-    for i, x in enumerate(results_gen):
-        counter += 1
-        if i >= 40:
-            break
-    assert counter >= 40
+    with DDGS() as ddgs:
+        ddgs_gen = ddgs.news("tesla")
+        results = [x for x in islice(ddgs_gen, 40)]
+        assert len(results) >= 30
 
 
 def test_maps():
-    results_gen = DDGS().maps("school", place="London")
-    counter = 0
-    for i, x in enumerate(results_gen):
-        counter += 1
-        if i >= 40:
-            break
-    assert counter >= 40
+    with DDGS() as ddgs:
+        ddgs_gen = ddgs.maps("school", place="London")
+        results = [x for x in islice(ddgs_gen, 40)]
+        assert len(results) >= 30
 
 
 def test_answers():
-    results_gen = DDGS().answers("cat")
-    counter = 0
-    for i, x in enumerate(results_gen):
-        counter += 1
-        if i >= 1:
-            break
-    assert counter >= 1
+    with DDGS() as ddgs:
+        ddgs_gen = ddgs.answers("sun")
+        results = [x for x in islice(ddgs_gen, 5)]
+        assert len(results) >= 1
 
 
 def test_suggestions():
-    results_gen = DDGS().suggestions("cat")
-    counter = 0
-    for i, x in enumerate(results_gen):
-        counter += 1
-        if i >= 10:
-            break
-    assert counter >= 1
+    with DDGS() as ddgs:
+        ddgs_gen = ddgs.suggestions("moon")
+        results = [x for x in islice(ddgs_gen, 5)]
+        assert len(results) >= 1
 
 
 def test_translate():
     results = DDGS().translate("school", to="de")
     assert results == {
         "detected_language": "en",
         "translated": "Schule",
         "original": "school",
     }
 
 
 def test_save_csv():
     keywords = "butterfly"
-    results_gen = DDGS().text(keywords)
-    results = []
-    for r in results_gen:
-        results.append(r)
-        if len(results) >= 20:
-            break
-    assert len(results) >= 20
+    with DDGS() as ddgs:
+        ddgs_gen = ddgs.text(keywords)
+        results = [x for x in islice(ddgs_gen, 25)]
+        assert len(results) >= 22
 
     save_csv(f"{keywords}.csv", results)
-    save_json(f"{keywords}.json", results)
 
     # delete files and folders contains keyword in name
     not_files = True
     for name in os.listdir():
         if keywords in name:
             if os.path.isfile(name):
                 os.remove(name)
                 not_files = False
     if not_files:
         raise AssertionError("csv not found")
 
 
 def test_save_json():
     keywords = "chicago"
-    results_gen = DDGS().text(keywords)
-    results = []
-    for r in results_gen:
-        results.append(r)
-        if len(results) >= 20:
-            break
-    assert len(results) >= 20
+    with DDGS() as ddgs:
+        ddgs_gen = ddgs.text(keywords)
+        results = [x for x in islice(ddgs_gen, 25)]
+        assert len(results) >= 22
 
     save_json(f"{keywords}.json", results)
 
     # delete files and folders contains keyword in name
     not_files = True
     for name in os.listdir():
         if keywords in name:
@@ -129,16 +116,16 @@
                 not_files = False
     if not_files:
         raise AssertionError("json not found")
 
 
 def test_text_download():
     keywords = "maradona"
-    results = [x for i, x in enumerate(DDGS().text(keywords)) if i <= 10]
-    assert len(results) >= 10
+    results = [x for x in islice(DDGS().text(keywords), 10)]
+    assert len(results) >= 8
 
     download_results(keywords, results)
 
     # delete files contains keyword in name
     files = False
     for dir in os.listdir("."):
         if keywords in dir:
@@ -155,16 +142,16 @@
         if f"{keywords}" in dir:
             if os.path.isdir(dir):
                 shutil.rmtree(dir)
 
 
 def test_images_download():
     keywords = "real madrid"
-    results = [x for i, x in enumerate(DDGS().images(keywords)) if i <= 10]
-    assert len(results) >= 10
+    results = [x for x in islice(DDGS().images(keywords), 10)]
+    assert len(results) >= 8
 
     download_results(keywords, results, images=True)
 
     # delete files contains keyword in name
     files = False
     for dir in os.listdir("."):
         if keywords in dir:
```

