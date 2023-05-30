# Comparing `tmp/streamlit-chat-askgdpr-0.2.tar.gz` & `tmp/streamlit-chat-askgdpr-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-chat-askgdpr-0.2.tar", last modified: Sun May 28 21:49:26 2023, max compression
+gzip compressed data, was "streamlit-chat-askgdpr-0.3.tar", last modified: Tue May 30 16:13:59 2023, max compression
```

## Comparing `streamlit-chat-askgdpr-0.2.tar` & `streamlit-chat-askgdpr-0.3.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:49:26.399790 streamlit-chat-askgdpr-0.2/
--rw-r--r--   0 grek       (501) staff       (20)     1064 2023-05-28 17:24:10.000000 streamlit-chat-askgdpr-0.2/LICENSE
--rw-r--r--   0 grek       (501) staff       (20)       50 2023-05-28 17:24:10.000000 streamlit-chat-askgdpr-0.2/MANIFEST.in
--rw-r--r--   0 grek       (501) staff       (20)     4154 2023-05-28 21:49:26.399591 streamlit-chat-askgdpr-0.2/PKG-INFO
--rw-r--r--   0 grek       (501) staff       (20)     3687 2023-05-28 17:24:10.000000 streamlit-chat-askgdpr-0.2/README.md
--rw-r--r--   0 grek       (501) staff       (20)       38 2023-05-28 21:49:26.399841 streamlit-chat-askgdpr-0.2/setup.cfg
--rw-r--r--   0 grek       (501) staff       (20)      924 2023-05-28 21:49:13.000000 streamlit-chat-askgdpr-0.2/setup.py
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:49:26.373478 streamlit-chat-askgdpr-0.2/streamlit_chat/
--rw-r--r--   0 grek       (501) staff       (20)     3594 2023-05-28 21:49:21.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/__init__.py
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:49:26.372173 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:49:26.375414 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/
--rw-r--r--   0 grek       (501) staff       (20)     1150 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/asset-manifest.json
--rw-r--r--   0 grek       (501) staff       (20)   197459 2023-05-28 21:32:34.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/bootstrap.min.css
--rw-r--r--   0 grek       (501) staff       (20)   646432 2023-05-28 21:32:34.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/bootstrap.min.css.map
--rw-r--r--   0 grek       (501) staff       (20)     2209 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/index.html
--rw-r--r--   0 grek       (501) staff       (20)     8091 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/precache-manifest.913e70ff508b34716fa805cc28b9d423.js
--rw-r--r--   0 grek       (501) staff       (20)     1183 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/service-worker.js
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:49:26.372483 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:49:26.376000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/css/
--rw-r--r--   0 grek       (501) staff       (20)    48144 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/css/2.4fdd6c40.chunk.css
--rw-r--r--   0 grek       (501) staff       (20)    64407 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/css/2.4fdd6c40.chunk.css.map
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:49:26.388444 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/js/
--rw-r--r--   0 grek       (501) staff       (20)  1608824 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js
--rw-r--r--   0 grek       (501) staff       (20)     2015 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js.LICENSE.txt
--rw-r--r--   0 grek       (501) staff       (20)  5402535 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js.map
--rw-r--r--   0 grek       (501) staff       (20)     2106 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/js/main.e9a08b4d.chunk.js
--rw-r--r--   0 grek       (501) staff       (20)     5207 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/js/main.e9a08b4d.chunk.js.map
--rw-r--r--   0 grek       (501) staff       (20)     1598 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js
--rw-r--r--   0 grek       (501) staff       (20)     8317 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js.map
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:49:26.398717 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/
--rw-r--r--   0 grek       (501) staff       (20)    33516 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.10824af7.woff
--rw-r--r--   0 grek       (501) staff       (20)    63632 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.56573229.ttf
--rw-r--r--   0 grek       (501) staff       (20)    28076 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.66c67820.woff2
--rw-r--r--   0 grek       (501) staff       (20)    12368 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.497bf407.ttf
--rw-r--r--   0 grek       (501) staff       (20)     6912 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.a9e9b095.woff2
--rw-r--r--   0 grek       (501) staff       (20)     7716 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.de2ba279.woff
--rw-r--r--   0 grek       (501) staff       (20)     6908 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.08d95d99.woff2
--rw-r--r--   0 grek       (501) staff       (20)     7656 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.a25140fb.woff
--rw-r--r--   0 grek       (501) staff       (20)    12344 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.e6fb499f.ttf
--rw-r--r--   0 grek       (501) staff       (20)    13296 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.40934fc0.woff
--rw-r--r--   0 grek       (501) staff       (20)    11348 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.796f3797.woff2
--rw-r--r--   0 grek       (501) staff       (20)    19584 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.b9d7c449.ttf
--rw-r--r--   0 grek       (501) staff       (20)    19572 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.97a699d8.ttf
--rw-r--r--   0 grek       (501) staff       (20)    13208 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.e435cda5.woff
--rw-r--r--   0 grek       (501) staff       (20)    11316 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.f9e6a99f.woff2
--rw-r--r--   0 grek       (501) staff       (20)    29912 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.4cdba646.woff
--rw-r--r--   0 grek       (501) staff       (20)    51336 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.8e431f7e.ttf
--rw-r--r--   0 grek       (501) staff       (20)    25324 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.a9382e25.woff2
--rw-r--r--   0 grek       (501) staff       (20)    32968 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.52fb39b0.ttf
--rw-r--r--   0 grek       (501) staff       (20)    19412 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.5f875f98.woff
--rw-r--r--   0 grek       (501) staff       (20)    16780 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.d8737343.woff2
--rw-r--r--   0 grek       (501) staff       (20)    33580 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.39349e0a.ttf
--rw-r--r--   0 grek       (501) staff       (20)    16988 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.65297062.woff2
--rw-r--r--   0 grek       (501) staff       (20)    19676 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.8ffd28f6.woff
--rw-r--r--   0 grek       (501) staff       (20)    53580 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.818582da.ttf
--rw-r--r--   0 grek       (501) staff       (20)    30772 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.f1cdb692.woff
--rw-r--r--   0 grek       (501) staff       (20)    26272 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.f8a7f19f.woff2
--rw-r--r--   0 grek       (501) staff       (20)    16400 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.1320454d.woff2
--rw-r--r--   0 grek       (501) staff       (20)    18668 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.48155e43.woff
--rw-r--r--   0 grek       (501) staff       (20)    31196 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.6589c4f1.ttf
--rw-r--r--   0 grek       (501) staff       (20)    16440 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.d8b7a801.woff2
--rw-r--r--   0 grek       (501) staff       (20)    18748 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.ed7aea12.woff
--rw-r--r--   0 grek       (501) staff       (20)    31308 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.fe5ed587.ttf
--rw-r--r--   0 grek       (501) staff       (20)    14408 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.0e897d27.woff
--rw-r--r--   0 grek       (501) staff       (20)    12216 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.ad546b47.woff2
--rw-r--r--   0 grek       (501) staff       (20)    24504 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.f2ac7312.ttf
--rw-r--r--   0 grek       (501) staff       (20)    12028 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.e934cbc8.woff2
--rw-r--r--   0 grek       (501) staff       (20)    14112 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.ef725de5.woff
--rw-r--r--   0 grek       (501) staff       (20)    22364 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.f60b4a34.ttf
--rw-r--r--   0 grek       (501) staff       (20)    10344 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.1ac3ed6e.woff2
--rw-r--r--   0 grek       (501) staff       (20)    19436 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.3243452e.ttf
--rw-r--r--   0 grek       (501) staff       (20)    12316 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.5f8637ee.woff
--rw-r--r--   0 grek       (501) staff       (20)     9644 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.1b3161eb.woff2
--rw-r--r--   0 grek       (501) staff       (20)    16648 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.a189c37d.ttf
--rw-r--r--   0 grek       (501) staff       (20)    10588 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.a82fa2a7.woff
--rw-r--r--   0 grek       (501) staff       (20)    12228 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.0d8d9204.ttf
--rw-r--r--   0 grek       (501) staff       (20)     6496 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.4788ba5b.woff
--rw-r--r--   0 grek       (501) staff       (20)     5468 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.82ef26dc.woff2
--rw-r--r--   0 grek       (501) staff       (20)    11508 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.1fdda0e5.ttf
--rw-r--r--   0 grek       (501) staff       (20)     5208 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.95a1da91.woff2
--rw-r--r--   0 grek       (501) staff       (20)     6188 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.b0628bfd.woff
--rw-r--r--   0 grek       (501) staff       (20)     4420 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.4de844d4.woff
--rw-r--r--   0 grek       (501) staff       (20)     3624 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.9108a400.woff2
--rw-r--r--   0 grek       (501) staff       (20)     7588 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.963af864.ttf
--rw-r--r--   0 grek       (501) staff       (20)    10364 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.27a23ee6.ttf
--rw-r--r--   0 grek       (501) staff       (20)     5980 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.3045a61f.woff
--rw-r--r--   0 grek       (501) staff       (20)     4928 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.61522cd3.woff2
--rw-r--r--   0 grek       (501) staff       (20)    16028 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.0e046058.woff
--rw-r--r--   0 grek       (501) staff       (20)    27556 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.6bf42875.ttf
--rw-r--r--   0 grek       (501) staff       (20)    13568 2023-05-28 21:32:51.000000 streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.b8b8393d.woff2
-drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-28 21:49:26.399353 streamlit-chat-askgdpr-0.2/streamlit_chat_askgdpr.egg-info/
--rw-r--r--   0 grek       (501) staff       (20)     4154 2023-05-28 21:49:26.000000 streamlit-chat-askgdpr-0.2/streamlit_chat_askgdpr.egg-info/PKG-INFO
--rw-r--r--   0 grek       (501) staff       (20)     5876 2023-05-28 21:49:26.000000 streamlit-chat-askgdpr-0.2/streamlit_chat_askgdpr.egg-info/SOURCES.txt
--rw-r--r--   0 grek       (501) staff       (20)        1 2023-05-28 21:49:26.000000 streamlit-chat-askgdpr-0.2/streamlit_chat_askgdpr.egg-info/dependency_links.txt
--rw-r--r--   0 grek       (501) staff       (20)       16 2023-05-28 21:49:26.000000 streamlit-chat-askgdpr-0.2/streamlit_chat_askgdpr.egg-info/requires.txt
--rw-r--r--   0 grek       (501) staff       (20)       15 2023-05-28 21:49:26.000000 streamlit-chat-askgdpr-0.2/streamlit_chat_askgdpr.egg-info/top_level.txt
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-30 16:13:59.016345 streamlit-chat-askgdpr-0.3/
+-rw-r--r--   0 grek       (501) staff       (20)     1064 2023-05-28 17:24:10.000000 streamlit-chat-askgdpr-0.3/LICENSE
+-rw-r--r--   0 grek       (501) staff       (20)       50 2023-05-28 17:24:10.000000 streamlit-chat-askgdpr-0.3/MANIFEST.in
+-rw-r--r--   0 grek       (501) staff       (20)     4154 2023-05-30 16:13:59.016165 streamlit-chat-askgdpr-0.3/PKG-INFO
+-rw-r--r--   0 grek       (501) staff       (20)     3687 2023-05-28 17:24:10.000000 streamlit-chat-askgdpr-0.3/README.md
+-rw-r--r--   0 grek       (501) staff       (20)       38 2023-05-30 16:13:59.016394 streamlit-chat-askgdpr-0.3/setup.cfg
+-rw-r--r--   0 grek       (501) staff       (20)      924 2023-05-30 16:10:10.000000 streamlit-chat-askgdpr-0.3/setup.py
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-30 16:13:58.992524 streamlit-chat-askgdpr-0.3/streamlit_chat/
+-rw-r--r--   0 grek       (501) staff       (20)     3594 2023-05-30 16:06:18.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/__init__.py
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-30 16:13:58.991371 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-30 16:13:58.994109 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/
+-rw-r--r--   0 grek       (501) staff       (20)     1150 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/asset-manifest.json
+-rw-r--r--   0 grek       (501) staff       (20)   197459 2023-05-30 16:11:19.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/bootstrap.min.css
+-rw-r--r--   0 grek       (501) staff       (20)   646432 2023-05-30 16:11:19.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/bootstrap.min.css.map
+-rw-r--r--   0 grek       (501) staff       (20)     2209 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/index.html
+-rw-r--r--   0 grek       (501) staff       (20)     8091 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/precache-manifest.4deaf86e5f803571108bd8b87b0eca85.js
+-rw-r--r--   0 grek       (501) staff       (20)     1183 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/service-worker.js
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-30 16:13:58.991646 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-30 16:13:58.994401 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/css/
+-rw-r--r--   0 grek       (501) staff       (20)    48144 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/css/2.4fdd6c40.chunk.css
+-rw-r--r--   0 grek       (501) staff       (20)    64407 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/css/2.4fdd6c40.chunk.css.map
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-30 16:13:59.002967 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/js/
+-rw-r--r--   0 grek       (501) staff       (20)  1608824 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js
+-rw-r--r--   0 grek       (501) staff       (20)     2015 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js.LICENSE.txt
+-rw-r--r--   0 grek       (501) staff       (20)  5402535 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js.map
+-rw-r--r--   0 grek       (501) staff       (20)     2060 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/js/main.e5b32794.chunk.js
+-rw-r--r--   0 grek       (501) staff       (20)     5076 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/js/main.e5b32794.chunk.js.map
+-rw-r--r--   0 grek       (501) staff       (20)     1598 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js
+-rw-r--r--   0 grek       (501) staff       (20)     8317 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js.map
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-30 16:13:59.015241 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/
+-rw-r--r--   0 grek       (501) staff       (20)    33516 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.10824af7.woff
+-rw-r--r--   0 grek       (501) staff       (20)    63632 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.56573229.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    28076 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.66c67820.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    12368 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.497bf407.ttf
+-rw-r--r--   0 grek       (501) staff       (20)     6912 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.a9e9b095.woff2
+-rw-r--r--   0 grek       (501) staff       (20)     7716 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.de2ba279.woff
+-rw-r--r--   0 grek       (501) staff       (20)     6908 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.08d95d99.woff2
+-rw-r--r--   0 grek       (501) staff       (20)     7656 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.a25140fb.woff
+-rw-r--r--   0 grek       (501) staff       (20)    12344 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.e6fb499f.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    13296 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.40934fc0.woff
+-rw-r--r--   0 grek       (501) staff       (20)    11348 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.796f3797.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    19584 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.b9d7c449.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    19572 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.97a699d8.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    13208 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.e435cda5.woff
+-rw-r--r--   0 grek       (501) staff       (20)    11316 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.f9e6a99f.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    29912 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.4cdba646.woff
+-rw-r--r--   0 grek       (501) staff       (20)    51336 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.8e431f7e.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    25324 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.a9382e25.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    32968 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.52fb39b0.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    19412 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.5f875f98.woff
+-rw-r--r--   0 grek       (501) staff       (20)    16780 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.d8737343.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    33580 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.39349e0a.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    16988 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.65297062.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    19676 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.8ffd28f6.woff
+-rw-r--r--   0 grek       (501) staff       (20)    53580 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.818582da.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    30772 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.f1cdb692.woff
+-rw-r--r--   0 grek       (501) staff       (20)    26272 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.f8a7f19f.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    16400 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.1320454d.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    18668 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.48155e43.woff
+-rw-r--r--   0 grek       (501) staff       (20)    31196 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.6589c4f1.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    16440 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.d8b7a801.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    18748 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.ed7aea12.woff
+-rw-r--r--   0 grek       (501) staff       (20)    31308 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.fe5ed587.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    14408 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.0e897d27.woff
+-rw-r--r--   0 grek       (501) staff       (20)    12216 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.ad546b47.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    24504 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.f2ac7312.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    12028 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.e934cbc8.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    14112 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.ef725de5.woff
+-rw-r--r--   0 grek       (501) staff       (20)    22364 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.f60b4a34.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    10344 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.1ac3ed6e.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    19436 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.3243452e.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    12316 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.5f8637ee.woff
+-rw-r--r--   0 grek       (501) staff       (20)     9644 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.1b3161eb.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    16648 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.a189c37d.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    10588 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.a82fa2a7.woff
+-rw-r--r--   0 grek       (501) staff       (20)    12228 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.0d8d9204.ttf
+-rw-r--r--   0 grek       (501) staff       (20)     6496 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.4788ba5b.woff
+-rw-r--r--   0 grek       (501) staff       (20)     5468 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.82ef26dc.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    11508 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.1fdda0e5.ttf
+-rw-r--r--   0 grek       (501) staff       (20)     5208 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.95a1da91.woff2
+-rw-r--r--   0 grek       (501) staff       (20)     6188 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.b0628bfd.woff
+-rw-r--r--   0 grek       (501) staff       (20)     4420 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.4de844d4.woff
+-rw-r--r--   0 grek       (501) staff       (20)     3624 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.9108a400.woff2
+-rw-r--r--   0 grek       (501) staff       (20)     7588 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.963af864.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    10364 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.27a23ee6.ttf
+-rw-r--r--   0 grek       (501) staff       (20)     5980 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.3045a61f.woff
+-rw-r--r--   0 grek       (501) staff       (20)     4928 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.61522cd3.woff2
+-rw-r--r--   0 grek       (501) staff       (20)    16028 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.0e046058.woff
+-rw-r--r--   0 grek       (501) staff       (20)    27556 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.6bf42875.ttf
+-rw-r--r--   0 grek       (501) staff       (20)    13568 2023-05-30 16:11:26.000000 streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.b8b8393d.woff2
+drwxr-xr-x   0 grek       (501) staff       (20)        0 2023-05-30 16:13:59.015946 streamlit-chat-askgdpr-0.3/streamlit_chat_askgdpr.egg-info/
+-rw-r--r--   0 grek       (501) staff       (20)     4154 2023-05-30 16:13:58.000000 streamlit-chat-askgdpr-0.3/streamlit_chat_askgdpr.egg-info/PKG-INFO
+-rw-r--r--   0 grek       (501) staff       (20)     5876 2023-05-30 16:13:58.000000 streamlit-chat-askgdpr-0.3/streamlit_chat_askgdpr.egg-info/SOURCES.txt
+-rw-r--r--   0 grek       (501) staff       (20)        1 2023-05-30 16:13:58.000000 streamlit-chat-askgdpr-0.3/streamlit_chat_askgdpr.egg-info/dependency_links.txt
+-rw-r--r--   0 grek       (501) staff       (20)       16 2023-05-30 16:13:58.000000 streamlit-chat-askgdpr-0.3/streamlit_chat_askgdpr.egg-info/requires.txt
+-rw-r--r--   0 grek       (501) staff       (20)       15 2023-05-30 16:13:58.000000 streamlit-chat-askgdpr-0.3/streamlit_chat_askgdpr.egg-info/top_level.txt
```

### Comparing `streamlit-chat-askgdpr-0.2/LICENSE` & `streamlit-chat-askgdpr-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/PKG-INFO` & `streamlit-chat-askgdpr-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-chat-askgdpr
-Version: 0.2
+Version: 0.3
 Summary: A streamlit component, to make chatbots
 Home-page: https://github.com/AI-Yash/st-chat
 Author: Grzegorz Kossakowski, Maciej Zdanowicz
 Author-email: yashpawarp@gmail.com
 Keywords: chat streamlit streamlit-component
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `streamlit-chat-askgdpr-0.2/README.md` & `streamlit-chat-askgdpr-0.3/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/setup.py` & `streamlit-chat-askgdpr-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setuptools.setup(
     name="streamlit-chat-askgdpr",
-    version="0.2",
+    version="0.3",
     author="Grzegorz Kossakowski, Maciej Zdanowicz",
     author_email="yashpawarp@gmail.com",
     description="A streamlit component, to make chatbots",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/AI-Yash/st-chat",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/__init__.py` & `streamlit-chat-askgdpr-0.3/streamlit_chat/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/asset-manifest.json` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/asset-manifest.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8464285714285714%*

 * *Differences: {"'entrypoints'": "{insert: [(3, 'static/js/main.e5b32794.chunk.js')], delete: [3]}",*

 * * "'files'": "{'main.js': './static/js/main.e5b32794.chunk.js', 'main.js.map': "*

 * *            "'./static/js/main.e5b32794.chunk.js.map', "*

 * *            "'precache-manifest.4deaf86e5f803571108bd8b87b0eca85.js': "*

 * *            "'./precache-manifest.4deaf86e5f803571108bd8b87b0eca85.js', delete: "*

 * *            "['precache-manifest.913e70ff508b34716fa805cc28b9d423.js']}"}*

```diff
@@ -1,19 +1,19 @@
 {
     "entrypoints": [
         "static/js/runtime-main.11ec9aca.js",
         "static/css/2.4fdd6c40.chunk.css",
         "static/js/2.96b2a504.chunk.js",
-        "static/js/main.e9a08b4d.chunk.js"
+        "static/js/main.e5b32794.chunk.js"
     ],
     "files": {
         "index.html": "./index.html",
-        "main.js": "./static/js/main.e9a08b4d.chunk.js",
-        "main.js.map": "./static/js/main.e9a08b4d.chunk.js.map",
-        "precache-manifest.913e70ff508b34716fa805cc28b9d423.js": "./precache-manifest.913e70ff508b34716fa805cc28b9d423.js",
+        "main.js": "./static/js/main.e5b32794.chunk.js",
+        "main.js.map": "./static/js/main.e5b32794.chunk.js.map",
+        "precache-manifest.4deaf86e5f803571108bd8b87b0eca85.js": "./precache-manifest.4deaf86e5f803571108bd8b87b0eca85.js",
         "runtime-main.js": "./static/js/runtime-main.11ec9aca.js",
         "runtime-main.js.map": "./static/js/runtime-main.11ec9aca.js.map",
         "service-worker.js": "./service-worker.js",
         "static/css/2.4fdd6c40.chunk.css": "./static/css/2.4fdd6c40.chunk.css",
         "static/css/2.4fdd6c40.chunk.css.map": "./static/css/2.4fdd6c40.chunk.css.map",
         "static/js/2.96b2a504.chunk.js": "./static/js/2.96b2a504.chunk.js",
         "static/js/2.96b2a504.chunk.js.LICENSE.txt": "./static/js/2.96b2a504.chunk.js.LICENSE.txt",
```

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/bootstrap.min.css` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/bootstrap.min.css.map` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/index.html` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/><style>table,td,th{border:1px solid}</style><link href="./static/css/2.4fdd6c40.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,a=t[0],p=t[1],i=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in p)Object.prototype.hasOwnProperty.call(p,n)&&(e[n]=p[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var p=r[a];0!==o[p]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],p=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var f=p;r()}([])</script><script src="./static/js/2.96b2a504.chunk.js"></script><script src="./static/js/main.e9a08b4d.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/><style>table,td,th{border:1px solid}</style><link href="./static/css/2.4fdd6c40.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,a=t[0],p=t[1],i=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in p)Object.prototype.hasOwnProperty.call(p,n)&&(e[n]=p[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var p=r[a];0!==o[p]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],p=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var f=p;r()}([])</script><script src="./static/js/2.96b2a504.chunk.js"></script><script src="./static/js/main.e5b32794.chunk.js"></script></body></html>
```

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/precache-manifest.913e70ff508b34716fa805cc28b9d423.js` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/precache-manifest.4deaf86e5f803571108bd8b87b0eca85.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,22 +1,22 @@
 self.__precacheManifest = (self.__precacheManifest || []).concat([{
-    "revision": "d3737756586c638b2122a660934b5273",
+    "revision": "059c9f27320892109640c6142441d778",
     "url": "./index.html"
 }, {
     "revision": "69ed66f17e024c470102",
     "url": "./static/css/2.4fdd6c40.chunk.css"
 }, {
     "revision": "69ed66f17e024c470102",
     "url": "./static/js/2.96b2a504.chunk.js"
 }, {
     "revision": "d448927d184e31601f199ee8b38a43f4",
     "url": "./static/js/2.96b2a504.chunk.js.LICENSE.txt"
 }, {
-    "revision": "97ba086a3245ea63db60",
-    "url": "./static/js/main.e9a08b4d.chunk.js"
+    "revision": "e0d6fbf200f7d7f1103a",
+    "url": "./static/js/main.e5b32794.chunk.js"
 }, {
     "revision": "7c26bca7e16783d14d15",
     "url": "./static/js/runtime-main.11ec9aca.js"
 }, {
     "revision": "10824af77e9961cfd548c8a458f10851",
     "url": "./static/media/KaTeX_AMS-Regular.10824af7.woff"
 }, {
```

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/service-worker.js` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/service-worker.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -10,15 +10,15 @@
  * and re-run your build process.
  * See https://goo.gl/2aRDsh
  */
 
 importScripts("https://storage.googleapis.com/workbox-cdn/releases/4.3.1/workbox-sw.js");
 
 importScripts(
-    "./precache-manifest.913e70ff508b34716fa805cc28b9d423.js"
+    "./precache-manifest.4deaf86e5f803571108bd8b87b0eca85.js"
 );
 
 self.addEventListener('message', (event) => {
     if (event.data && event.data.type === 'SKIP_WAITING') {
         self.skipWaiting();
     }
 });
```

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/css/2.4fdd6c40.chunk.css` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/css/2.4fdd6c40.chunk.css`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/css/2.4fdd6c40.chunk.css.map` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/css/2.4fdd6c40.chunk.css.map`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js.LICENSE.txt` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js.map` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/js/main.e9a08b4d.chunk.js` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/js/main.e5b32794.chunk.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,103 +1,101 @@
 (this.webpackJsonpstreamlit_component_template = this.webpackJsonpstreamlit_component_template || []).push([
     [0], {
-        153: function(e, a, t) {
-            e.exports = t(209)
+        153: function(e, t, a) {
+            e.exports = a(209)
         },
-        209: function(e, a, t) {
+        209: function(e, t, a) {
             "use strict";
-            t.r(a);
-            var r, n, i = t(10),
-                c = t.n(i),
-                o = t(99),
-                s = t.n(o),
-                l = t(7),
-                d = t(81),
-                p = t(0),
-                m = t(1),
-                u = t(2),
-                b = t(3),
-                g = t(68),
-                h = t(69),
-                f = t(50),
-                v = t(245),
-                x = t(145),
-                j = t(147),
-                w = t(146),
-                O = t(144),
-                y = t(248),
-                k = (t(161), t(162), t(163), function(e) {
-                    Object(u.a)(t, e);
-                    var a = Object(b.a)(t);
+            a.r(t);
+            var r, n, i = a(10),
+                c = a.n(i),
+                o = a(99),
+                s = a.n(o),
+                l = a(7),
+                d = a(81),
+                m = a(0),
+                p = a(1),
+                u = a(2),
+                b = a(3),
+                g = a(68),
+                h = a(69),
+                f = a(50),
+                v = a(245),
+                x = a(145),
+                j = a(147),
+                O = a(146),
+                w = a(144),
+                y = a(248),
+                k = (a(161), a(162), a(163), function(e) {
+                    Object(u.a)(a, e);
+                    var t = Object(b.a)(a);
 
-                    function t() {
+                    function a() {
                         var e;
-                        Object(m.a)(this, t);
+                        Object(p.a)(this, a);
                         for (var i = arguments.length, o = new Array(i), s = 0; s < i; s++) o[s] = arguments[s];
-                        return (e = a.call.apply(a, [this].concat(o))).render = function() {
+                        return (e = t.call.apply(t, [this].concat(o))).render = function() {
                             g.a.setFrameHeight(window.innerHeight);
-                            var a = e.props.args,
-                                t = a.isUser,
-                                i = a.avatarStyle,
-                                o = a.seed,
-                                s = a.message,
-                                p = a.allow_html,
-                                m = a.is_table,
-                                u = "https://api.dicebear.com/5.x/".concat(i, "/svg?seed=").concat(o),
-                                b = e.props.theme;
-                            if (!b) return c.a.createElement("div", null, "Theme is undefined, please check streamlit version.");
-                            var k = h.a.img({
+                            var t = e.props.args,
+                                a = t.isUser,
+                                i = t.avatarStyle,
+                                o = t.seed,
+                                s = t.message,
+                                m = t.allow_html,
+                                p = "https://api.dicebear.com/5.x/".concat(i, "/svg?seed=").concat(o),
+                                u = e.props.theme;
+                            if (!u) return c.a.createElement("div", null, "Theme is undefined, please check streamlit version.");
+                            var b = h.a.img({
                                     border: "1px solid transparent",
                                     borderRadius: "50%",
                                     height: "3rem",
                                     width: "3rem",
                                     margin: 0
                                 }),
-                                E = h.a.div({
+                                k = h.a.div({
                                     display: "inline-block",
-                                    background: b.secondaryBackgroundColor,
+                                    background: u.secondaryBackgroundColor,
                                     border: "1px solid transparent",
                                     borderRadius: "10px",
                                     padding: "10px 14px",
                                     margin: "5px 20px",
-                                    maxWidth: "70%",
-                                    whiteSpace: m ? "normal" : "pre-line"
+                                    maxWidth: "70%"
                                 }),
-                                _ = h.a.div({
+                                E = h.a.div({
                                     display: "flex",
-                                    fontFamily: "".concat(b.font, ", 'Segoe UI', 'Roboto', sans-serif"),
+                                    fontFamily: "".concat(u.font, ", 'Segoe UI', 'Roboto', sans-serif"),
                                     height: "auto",
                                     margin: 0,
                                     width: "100%"
                                 }, (function(e) {
                                     return e.isUser ? Object(f.a)(r || (r = Object(d.a)(["\n          flex-direction: row-reverse;\n          & > div {\n            text-align: right;\n          }\n        "]))) : Object(f.a)(n || (n = Object(d.a)([""])))
                                 })),
-                                S = [x.a, O.a],
-                                U = [j.a].concat(Object(l.a)(p ? [w.a] : []));
-                            return c.a.createElement(_, {
-                                isUser: t,
+                                _ = [x.a, w.a],
+                                U = [j.a].concat(Object(l.a)(m ? [O.a] : []));
+                            return c.a.createElement(E, {
+                                isUser: a,
                                 className: "markdown-body"
-                            }, c.a.createElement(k, {
-                                src: u,
+                            }, c.a.createElement(b, {
+                                src: p,
                                 alt: "profile",
                                 draggable: "false"
-                            }), c.a.createElement(E, null, c.a.createElement(v.a, {
-                                remarkPlugins: S,
+                            }), c.a.createElement(k, null, c.a.createElement(v.a, {
+                                remarkPlugins: _,
                                 rehypePlugins: [].concat(Object(l.a)(U), [
                                     [y.a, {
                                         detect: !0
                                     }]
                                 ])
                             }, s)))
                         }, e
                     }
-                    return Object(p.a)(t)
+                    return Object(m.a)(a)
                 }(g.b)),
                 E = Object(g.c)(k);
             s.a.render(c.a.createElement(c.a.StrictMode, null, c.a.createElement(E, null)), document.getElementById("root"))
         }
     },
     [
         [153, 1, 2]
     ]
 ]);
-//# sourceMappingURL=main.e9a08b4d.chunk.js.map
+//# sourceMappingURL=main.e5b32794.chunk.js.map
```

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/js/main.e9a08b4d.chunk.js.map` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/js/main.e5b32794.chunk.js.map`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8068283917340521%*

 * *Differences: {"'file'": "'static/js/main.e5b32794.chunk.js'",*

 * * "'mappings'": "'8VAqBMA,G,iOACGC,OAAS,WACdC,IAAUC,eAAeC,OAAOC,aAChC,MAA2D,EAAKC,MAAMC,KAA9DC,EAAR,EAAQA,OAAQC,EAAhB,EAAgBA,YAAaC,EAA7B,EAA6BA,KAAMC,EAAnC,EAAmCA,QAASC,EAA5C,EAA4CA,WACtCC,EAAS,uCAAmCJ,EAAnC,qBAA2DC,GAKlEI,EAAU,EAAKR,MAAfQ,MAIR,IAAKA,EACH,OAAO,oFAIT,IAAMC,EAASC,IAAOC,IAAI,CACxBC,OAAO,wBACPC,aAAc,MACdC,OAAQ,OACRC,MAAO,OACPC,OAAQ,IAIJC,EAAUP,IAAOQ,IAAI,CACzBC,QAAS,eACTC,WAAYZ,EAAMa,yBAClBT,OAAQ,wBACRC,aAAc,OACdS,QAAS,YACTN,OAAQ,WACRO,SAAU,QAIN7B […]*

```diff
@@ -1,25 +1,24 @@
 {
-    "file": "static/js/main.e9a08b4d.chunk.js",
-    "mappings": "8VAqBMA,G,iOACGC,OAAS,WACdC,IAAUC,eAAeC,OAAOC,aAChC,MAAqE,EAAKC,MAAMC,KAAxEC,EAAR,EAAQA,OAAQC,EAAhB,EAAgBA,YAAaC,EAA7B,EAA6BA,KAAMC,EAAnC,EAAmCA,QAASC,EAA5C,EAA4CA,WAAYC,EAAxD,EAAwDA,SAClDC,EAAS,uCAAmCL,EAAnC,qBAA2DC,GAKlEK,EAAU,EAAKT,MAAfS,MAIR,IAAKA,EACH,OAAO,oFAIT,IAAMC,EAASC,IAAOC,IAAI,CACxBC,OAAO,wBACPC,aAAc,MACdC,OAAQ,OACRC,MAAO,OACPC,OAAQ,IAIJC,EAAUP,IAAOQ,IAAI,CACzBC,QAAS,eACTC,WAAYZ,EAAMa,yBAClBT,OAAQ,wBACRC,aAAc,OACdS,QAAS,YACTN,OAAQ,WACRO,SAAU,MACVC,WAAalB,EAAwB,SAAb,aAIpBb,EAAOiB,IAAOQ,IAAI,CACtBC,QAAS,OAETM,WAAW,GAAD,OAAKjB,EAAMkB,KAAX,sCACVZ,OAAQ,OACRE,OAAQ,EACRD,MAAO,SAET,SAAChB,GACC,OAAIA,EAAME,OACD0B,YAAP,8IAOKA,YAAP,6BAIIC,EAAgB,CACpBC,IACAC,KAEIC,EAAa,CACjBC,KADiB,mBAEb3B,EAAa,CAAC4B,KAAa,KAGjC,OACE,kBAAC,EAAD,CAAMhC,OAAQA,EAAQiC,UAAU,iBAC9B,kBAACzB,EAAD,CAAQ0B,IAAK5B,EAAW6B,IAAI,UAAUC,UAAU,UAChD,kBAACpB,EAAD,KACE,kBAAC,IAAD,CACEW,cAAeA,EACfG,cAAa,sBAAMA,GAAN,CAAqB,CAACO,IAAiB,CAACC,QAAQ,OAE5DnC,M,yBA7EMoC,MAqFJC,cAAwBhD,GCtGvCiD,IAAShD,OACP,kBAAC,IAAMiD,WAAP,KACE,kBAAC,EAAD,OAEFC,SAASC,eAAe,W",
+    "file": "static/js/main.e5b32794.chunk.js",
+    "mappings": "8VAqBMA,G,iOACGC,OAAS,WACdC,IAAUC,eAAeC,OAAOC,aAChC,MAA2D,EAAKC,MAAMC,KAA9DC,EAAR,EAAQA,OAAQC,EAAhB,EAAgBA,YAAaC,EAA7B,EAA6BA,KAAMC,EAAnC,EAAmCA,QAASC,EAA5C,EAA4CA,WACtCC,EAAS,uCAAmCJ,EAAnC,qBAA2DC,GAKlEI,EAAU,EAAKR,MAAfQ,MAIR,IAAKA,EACH,OAAO,oFAIT,IAAMC,EAASC,IAAOC,IAAI,CACxBC,OAAO,wBACPC,aAAc,MACdC,OAAQ,OACRC,MAAO,OACPC,OAAQ,IAIJC,EAAUP,IAAOQ,IAAI,CACzBC,QAAS,eACTC,WAAYZ,EAAMa,yBAClBT,OAAQ,wBACRC,aAAc,OACdS,QAAS,YACTN,OAAQ,WACRO,SAAU,QAIN7B,EAAOgB,IAAOQ,IAAI,CACtBC,QAAS,OAETK,WAAW,GAAD,OAAKhB,EAAMiB,KAAX,sCACVX,OAAQ,OACRE,OAAQ,EACRD,MAAO,SAET,SAACf,GACC,OAAIA,EAAME,OACDwB,YAAP,8IAOKA,YAAP,6BAIIC,EAAgB,CACpBC,IACAC,KAEIC,EAAa,CACjBC,KADiB,mBAEbzB,EAAa,CAAC0B,KAAa,KAGjC,OACE,kBAAC,EAAD,CAAM9B,OAAQA,EAAQ+B,UAAU,iBAC9B,kBAACxB,EAAD,CAAQyB,IAAK3B,EAAW4B,IAAI,UAAUC,UAAU,UAChD,kBAACnB,EAAD,KACE,kBAAC,IAAD,CACEU,cAAeA,EACfG,cAAa,sBAAMA,GAAN,CAAqB,CAACO,IAAiB,CAACC,QAAQ,OAE5DjC,M,yBA5EMkC,MAoFJC,cAAwB9C,GCrGvC+C,IAAS9C,OACP,kBAAC,IAAM+C,WAAP,KACE,kBAAC,EAAD,OAEFC,SAASC,eAAe,W",
     "names": [
         "Chat",
         "render",
         "Streamlit",
         "setFrameHeight",
         "window",
         "innerHeight",
         "props",
         "args",
         "isUser",
         "avatarStyle",
         "seed",
         "message",
         "allow_html",
-        "is_table",
         "avatarUrl",
         "theme",
         "Avatar",
         "styled",
         "img",
         "border",
         "borderRadius",
@@ -29,15 +28,14 @@
         "Message",
         "div",
         "display",
         "background",
         "secondaryBackgroundColor",
         "padding",
         "maxWidth",
-        "whiteSpace",
         "fontFamily",
         "font",
         "css",
         "remarkPlugins",
         "remarkMath",
         "remarkGfm",
         "rehypePlugins",
@@ -58,12 +56,12 @@
     ],
     "sourceRoot": "",
     "sources": [
         "stChat.tsx",
         "index.tsx"
     ],
     "sourcesContent": [
-        "import {\n  // eslint-disable-next-line \n  Streamlit,\n  StreamlitComponentBase,\n  withStreamlitConnection,\n} from \"streamlit-component-lib\"\nimport React, { ReactNode } from \"react\"\nimport styled from '@emotion/styled'\nimport { css } from '@emotion/react'\n\nimport ReactMarkdown from \"react-markdown\"\nimport remarkMath from \"remark-math\"\nimport rehypeKatex from \"rehype-katex\"\nimport rehypeRaw from \"rehype-raw\"\nimport remarkGfm from \"remark-gfm\"\nimport rehypeHighlight from \"rehype-highlight\"\n\nimport 'katex/dist/katex.min.css'\nimport 'highlight.js/styles/monokai-sublime.css'\nimport 'github-markdown-css/github-markdown.css'\n\nclass Chat extends StreamlitComponentBase {\n  public render = (): ReactNode => {\n    Streamlit.setFrameHeight(window.innerHeight)\n    const { isUser, avatarStyle, seed, message, allow_html, is_table } = this.props.args;\n    const avatarUrl = `https://api.dicebear.com/5.x/${avatarStyle}/svg?seed=${seed}`\n    \n    // Streamlit sends us a theme object via props that we can use to ensure\n    // that our component has visuals that match the active theme in a\n    // streamlit app.\n    const { theme } = this.props\n    \n    // Maintain compatibility with older versions of Streamlit that don't send\n    // a theme object.\n    if (!theme) {\n      return <div>Theme is undefined, please check streamlit version.</div>\n    }\n    \n    // styles for the avatar image\n    const Avatar = styled.img({\n      border: `1px solid transparent`,\n      borderRadius: '50%',\n      height: '3rem',\n      width: '3rem',\n      margin: 0\n    })\n    \n    // styles for the message box\n    const Message = styled.div({\n      display: 'inline-block',\n      background: theme.secondaryBackgroundColor,\n      border: '1px solid transparent',\n      borderRadius: '10px',\n      padding: '10px 14px',\n      margin: '5px 20px',\n      maxWidth: '70%',\n      whiteSpace: !is_table ? 'pre-line' : 'normal'\n    })\n    \n    // styles for the container\n    const Chat = styled.div({\n      display: 'flex',\n      // flexDirection: 'row',\n      fontFamily: `${theme.font}, 'Segoe UI', 'Roboto', sans-serif`, \n      height: 'auto',\n      margin: 0,\n      width: '100%'\n    },\n    (props: {isUser: boolean}) => {  // specific styles\n      if (props.isUser){\n        return css`\n          flex-direction: row-reverse;\n          & > div {\n            text-align: right;\n          }\n        `\n      }\n      return css``\n    })\n\n    // Init React Markdown plugins\n    const remarkPlugins = [\n      remarkMath, \n      remarkGfm\n    ]\n    const rehypePlugins = [\n      rehypeKatex,\n      ...(allow_html ? [rehypeRaw] : [])\n    ]\n\n    return (\n      <Chat isUser={isUser} className='markdown-body'>\n        <Avatar src={avatarUrl} alt=\"profile\" draggable=\"false\"/>\n        <Message>\n          <ReactMarkdown \n            remarkPlugins={remarkPlugins}\n            rehypePlugins={[...rehypePlugins, [rehypeHighlight, {detect: true}]]}\n          >\n            {message}\n          </ReactMarkdown>\n        </Message>\n      </Chat>\n    )\n  }\n}\n\nexport default withStreamlitConnection(Chat);\n",
+        "import {\n  // eslint-disable-next-line \n  Streamlit,\n  StreamlitComponentBase,\n  withStreamlitConnection,\n} from \"streamlit-component-lib\"\nimport React, { ReactNode } from \"react\"\nimport styled from '@emotion/styled'\nimport { css } from '@emotion/react'\n\nimport ReactMarkdown from \"react-markdown\"\nimport remarkMath from \"remark-math\"\nimport rehypeKatex from \"rehype-katex\"\nimport rehypeRaw from \"rehype-raw\"\nimport remarkGfm from \"remark-gfm\"\nimport rehypeHighlight from \"rehype-highlight\"\n\nimport 'katex/dist/katex.min.css'\nimport 'highlight.js/styles/monokai-sublime.css'\nimport 'github-markdown-css/github-markdown.css'\n\nclass Chat extends StreamlitComponentBase {\n  public render = (): ReactNode => {\n    Streamlit.setFrameHeight(window.innerHeight)\n    const { isUser, avatarStyle, seed, message, allow_html } = this.props.args;\n    const avatarUrl = `https://api.dicebear.com/5.x/${avatarStyle}/svg?seed=${seed}`\n    \n    // Streamlit sends us a theme object via props that we can use to ensure\n    // that our component has visuals that match the active theme in a\n    // streamlit app.\n    const { theme } = this.props\n    \n    // Maintain compatibility with older versions of Streamlit that don't send\n    // a theme object.\n    if (!theme) {\n      return <div>Theme is undefined, please check streamlit version.</div>\n    }\n    \n    // styles for the avatar image\n    const Avatar = styled.img({\n      border: `1px solid transparent`,\n      borderRadius: '50%',\n      height: '3rem',\n      width: '3rem',\n      margin: 0\n    })\n    \n    // styles for the message box\n    const Message = styled.div({\n      display: 'inline-block',\n      background: theme.secondaryBackgroundColor,\n      border: '1px solid transparent',\n      borderRadius: '10px',\n      padding: '10px 14px',\n      margin: '5px 20px',\n      maxWidth: '70%',\n    })\n    \n    // styles for the container\n    const Chat = styled.div({\n      display: 'flex',\n      // flexDirection: 'row',\n      fontFamily: `${theme.font}, 'Segoe UI', 'Roboto', sans-serif`, \n      height: 'auto',\n      margin: 0,\n      width: '100%'\n    },\n    (props: {isUser: boolean}) => {  // specific styles\n      if (props.isUser){\n        return css`\n          flex-direction: row-reverse;\n          & > div {\n            text-align: right;\n          }\n        `\n      }\n      return css``\n    })\n\n    // Init React Markdown plugins\n    const remarkPlugins = [\n      remarkMath, \n      remarkGfm\n    ]\n    const rehypePlugins = [\n      rehypeKatex,\n      ...(allow_html ? [rehypeRaw] : [])\n    ]\n\n    return (\n      <Chat isUser={isUser} className='markdown-body'>\n        <Avatar src={avatarUrl} alt=\"profile\" draggable=\"false\"/>\n        <Message>\n          <ReactMarkdown \n            remarkPlugins={remarkPlugins}\n            rehypePlugins={[...rehypePlugins, [rehypeHighlight, {detect: true}]]}\n          >\n            {message}\n          </ReactMarkdown>\n        </Message>\n      </Chat>\n    )\n  }\n}\n\nexport default withStreamlitConnection(Chat);\n",
         "import React from \"react\"\nimport ReactDOM from \"react-dom\"\nimport Chat from \"./stChat\"\n\nReactDOM.render(\n  <React.StrictMode>\n    <Chat />\n  </React.StrictMode>,\n  document.getElementById(\"root\")\n)\n"
     ],
     "version": 3
 }
```

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js.map` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js.map`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.10824af7.woff` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.10824af7.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.56573229.ttf` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.56573229.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.66c67820.woff2` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.66c67820.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.497bf407.ttf` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.497bf407.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.a9e9b095.woff2` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.a9e9b095.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.de2ba279.woff` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.de2ba279.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.08d95d99.woff2` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.08d95d99.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.a25140fb.woff` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.a25140fb.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.e6fb499f.ttf` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Regular.e6fb499f.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.40934fc0.woff` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.40934fc0.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.796f3797.woff2` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.796f3797.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.b9d7c449.ttf` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Bold.b9d7c449.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.97a699d8.ttf` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.97a699d8.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.e435cda5.woff` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.e435cda5.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.f9e6a99f.woff2` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Fraktur-Regular.f9e6a99f.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.4cdba646.woff` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.4cdba646.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.8e431f7e.ttf` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.8e431f7e.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.a9382e25.woff2` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Bold.a9382e25.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.52fb39b0.ttf` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.52fb39b0.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.5f875f98.woff` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.5f875f98.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.d8737343.woff2` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-BoldItalic.d8737343.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.39349e0a.ttf` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.39349e0a.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.65297062.woff2` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.65297062.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.8ffd28f6.woff` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Italic.8ffd28f6.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.818582da.ttf` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.818582da.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.f1cdb692.woff` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.f1cdb692.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.f8a7f19f.woff2` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Main-Regular.f8a7f19f.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.1320454d.woff2` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.1320454d.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.48155e43.woff` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.48155e43.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.6589c4f1.ttf` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-BoldItalic.6589c4f1.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.d8b7a801.woff2` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.d8b7a801.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.ed7aea12.woff` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.ed7aea12.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.fe5ed587.ttf` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Math-Italic.fe5ed587.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.0e897d27.woff` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.0e897d27.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.ad546b47.woff2` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.ad546b47.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.f2ac7312.ttf` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Bold.f2ac7312.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.e934cbc8.woff2` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.e934cbc8.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.ef725de5.woff` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.ef725de5.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.f60b4a34.ttf` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Italic.f60b4a34.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.1ac3ed6e.woff2` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.1ac3ed6e.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.3243452e.ttf` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.3243452e.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.5f8637ee.woff` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_SansSerif-Regular.5f8637ee.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.1b3161eb.woff2` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.1b3161eb.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.a189c37d.ttf` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.a189c37d.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.a82fa2a7.woff` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Script-Regular.a82fa2a7.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.0d8d9204.ttf` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.0d8d9204.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.4788ba5b.woff` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.4788ba5b.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.82ef26dc.woff2` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Size1-Regular.82ef26dc.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.1fdda0e5.ttf` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.1fdda0e5.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.95a1da91.woff2` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.95a1da91.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.b0628bfd.woff` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Size2-Regular.b0628bfd.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.4de844d4.woff` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.4de844d4.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.9108a400.woff2` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.9108a400.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.963af864.ttf` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Size3-Regular.963af864.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.27a23ee6.ttf` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.27a23ee6.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.3045a61f.woff` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.3045a61f.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.61522cd3.woff2` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Size4-Regular.61522cd3.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.0e046058.woff` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.0e046058.woff`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.6bf42875.ttf` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.6bf42875.ttf`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.b8b8393d.woff2` & `streamlit-chat-askgdpr-0.3/streamlit_chat/frontend/build/static/media/KaTeX_Typewriter-Regular.b8b8393d.woff2`

 * *Files identical despite different names*

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat_askgdpr.egg-info/PKG-INFO` & `streamlit-chat-askgdpr-0.3/streamlit_chat_askgdpr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-chat-askgdpr
-Version: 0.2
+Version: 0.3
 Summary: A streamlit component, to make chatbots
 Home-page: https://github.com/AI-Yash/st-chat
 Author: Grzegorz Kossakowski, Maciej Zdanowicz
 Author-email: yashpawarp@gmail.com
 Keywords: chat streamlit streamlit-component
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `streamlit-chat-askgdpr-0.2/streamlit_chat_askgdpr.egg-info/SOURCES.txt` & `streamlit-chat-askgdpr-0.3/streamlit_chat_askgdpr.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 README.md
 setup.py
 streamlit_chat/__init__.py
 streamlit_chat/frontend/build/asset-manifest.json
 streamlit_chat/frontend/build/bootstrap.min.css
 streamlit_chat/frontend/build/bootstrap.min.css.map
 streamlit_chat/frontend/build/index.html
-streamlit_chat/frontend/build/precache-manifest.913e70ff508b34716fa805cc28b9d423.js
+streamlit_chat/frontend/build/precache-manifest.4deaf86e5f803571108bd8b87b0eca85.js
 streamlit_chat/frontend/build/service-worker.js
 streamlit_chat/frontend/build/static/css/2.4fdd6c40.chunk.css
 streamlit_chat/frontend/build/static/css/2.4fdd6c40.chunk.css.map
 streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js
 streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js.LICENSE.txt
 streamlit_chat/frontend/build/static/js/2.96b2a504.chunk.js.map
-streamlit_chat/frontend/build/static/js/main.e9a08b4d.chunk.js
-streamlit_chat/frontend/build/static/js/main.e9a08b4d.chunk.js.map
+streamlit_chat/frontend/build/static/js/main.e5b32794.chunk.js
+streamlit_chat/frontend/build/static/js/main.e5b32794.chunk.js.map
 streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js
 streamlit_chat/frontend/build/static/js/runtime-main.11ec9aca.js.map
 streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.10824af7.woff
 streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.56573229.ttf
 streamlit_chat/frontend/build/static/media/KaTeX_AMS-Regular.66c67820.woff2
 streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.497bf407.ttf
 streamlit_chat/frontend/build/static/media/KaTeX_Caligraphic-Bold.a9e9b095.woff2
```

