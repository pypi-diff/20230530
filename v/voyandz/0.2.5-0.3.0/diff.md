# Comparing `tmp/voyandz-0.2.5.tar.gz` & `tmp/voyandz-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/voyandz-0.2.5.tar", last modified: Mon Jun 21 12:57:08 2021, max compression
+gzip compressed data, was "voyandz-0.3.0.tar", last modified: Tue May 30 13:22:21 2023, max compression
```

## Comparing `voyandz-0.2.5.tar` & `voyandz-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 R.Zalewski (11752) adb      (10000)        0 2021-06-21 12:57:08.000000 voyandz-0.2.5/
--rw-r--r--   0 R.Zalewski (11752) adb      (10000)     7184 2021-06-21 12:57:08.000000 voyandz-0.2.5/PKG-INFO
-drwxr-xr-x   0 R.Zalewski (11752) adb      (10000)        0 2021-06-21 12:57:08.000000 voyandz-0.2.5/voyandz.egg-info/
--rw-r--r--   0 R.Zalewski (11752) adb      (10000)     7184 2021-06-21 12:57:08.000000 voyandz-0.2.5/voyandz.egg-info/PKG-INFO
--rw-r--r--   0 R.Zalewski (11752) adb      (10000)        1 2021-06-21 12:57:08.000000 voyandz-0.2.5/voyandz.egg-info/not-zip-safe
--rw-r--r--   0 R.Zalewski (11752) adb      (10000)      472 2021-06-21 12:57:08.000000 voyandz-0.2.5/voyandz.egg-info/SOURCES.txt
--rw-r--r--   0 R.Zalewski (11752) adb      (10000)       46 2021-06-21 12:57:08.000000 voyandz-0.2.5/voyandz.egg-info/entry_points.txt
--rw-r--r--   0 R.Zalewski (11752) adb      (10000)        8 2021-06-21 12:57:08.000000 voyandz-0.2.5/voyandz.egg-info/top_level.txt
--rw-r--r--   0 R.Zalewski (11752) adb      (10000)        1 2021-06-21 12:57:08.000000 voyandz-0.2.5/voyandz.egg-info/dependency_links.txt
--rw-r--r--   0 R.Zalewski (11752) adb      (10000)       13 2021-06-21 12:57:08.000000 voyandz-0.2.5/voyandz.egg-info/requires.txt
--rw-r--r--   0 R.Zalewski (11752) adb      (10000)      741 2021-06-21 12:48:40.000000 voyandz-0.2.5/setup.py
--rw-r--r--   0 R.Zalewski (11752) adb      (10000)       38 2021-06-21 12:57:08.000000 voyandz-0.2.5/setup.cfg
--rw-r--r--   0 R.Zalewski (11752) adb      (10000)       72 2018-07-30 07:11:40.000000 voyandz-0.2.5/MANIFEST.in
--rw-r--r--   0 R.Zalewski (11752) adb      (10000)     1097 2021-04-21 12:37:48.000000 voyandz-0.2.5/LICENSE
-drwxr-xr-x   0 R.Zalewski (11752) adb      (10000)        0 2021-06-21 12:57:08.000000 voyandz-0.2.5/voyandz/
--rw-r--r--   0 R.Zalewski (11752) adb      (10000)       79 2021-06-21 12:49:13.000000 voyandz-0.2.5/voyandz/version.py
--rw-r--r--   0 R.Zalewski (11752) adb      (10000)     5838 2021-04-21 12:36:57.000000 voyandz-0.2.5/voyandz/server.py
--rw-r--r--   0 R.Zalewski (11752) adb      (10000)     2496 2018-09-11 13:48:34.000000 voyandz-0.2.5/voyandz/logging.py
--rw-r--r--   0 R.Zalewski (11752) adb      (10000)     1742 2018-08-06 07:49:20.000000 voyandz-0.2.5/voyandz/cli.py
--rw-r--r--   0 R.Zalewski (11752) adb      (10000)    24883 2021-06-21 12:28:21.000000 voyandz-0.2.5/voyandz/piping.py
-drwxr-xr-x   0 R.Zalewski (11752) adb      (10000)        0 2021-06-21 12:57:08.000000 voyandz-0.2.5/voyandz/templates/
--rw-r--r--   0 R.Zalewski (11752) adb      (10000)      703 2018-07-31 07:44:32.000000 voyandz-0.2.5/voyandz/templates/home.html
--rw-r--r--   0 R.Zalewski (11752) adb      (10000)     2079 2018-08-06 07:49:20.000000 voyandz-0.2.5/voyandz/templates/stat.html
--rw-r--r--   0 R.Zalewski (11752) adb      (10000)     1767 2018-07-30 07:11:40.000000 voyandz-0.2.5/voyandz/stats.py
--rw-r--r--   0 R.Zalewski (11752) adb      (10000)      140 2018-07-09 07:13:50.000000 voyandz-0.2.5/voyandz/__init__.py
--rw-r--r--   0 R.Zalewski (11752) adb      (10000)     3628 2018-09-19 13:54:14.000000 voyandz-0.2.5/voyandz/config.py
--rw-r--r--   0 R.Zalewski (11752) adb      (10000)      476 2018-08-06 07:59:33.000000 voyandz-0.2.5/voyandz/util.py
--rw-r--r--   0 R.Zalewski (11752) adb      (10000)     4498 2018-09-17 14:16:21.000000 voyandz-0.2.5/README.md
+drwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)        0 2023-05-30 13:22:21.761526 voyandz-0.3.0/
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     1103 2023-05-30 08:12:33.000000 voyandz-0.3.0/LICENSE
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)       76 2023-05-30 13:21:52.000000 voyandz-0.3.0/MANIFEST.in
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     6029 2023-05-30 13:22:21.761526 voyandz-0.3.0/PKG-INFO
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     4430 2023-05-30 13:21:52.000000 voyandz-0.3.0/README.md
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)      602 2023-05-30 13:22:21.761526 voyandz-0.3.0/setup.cfg
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)       54 2023-05-30 13:15:38.000000 voyandz-0.3.0/setup.py
+drwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)        0 2023-05-30 13:22:21.761526 voyandz-0.3.0/src/
+drwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)        0 2023-05-30 13:22:21.761526 voyandz-0.3.0/src/voyandz/
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)      140 2023-05-30 13:15:38.000000 voyandz-0.3.0/src/voyandz/__init__.py
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     1742 2023-05-30 13:15:38.000000 voyandz-0.3.0/src/voyandz/cli.py
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     3628 2023-05-30 13:15:38.000000 voyandz-0.3.0/src/voyandz/config.py
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     2496 2023-05-30 13:15:38.000000 voyandz-0.3.0/src/voyandz/logging.py
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)    24883 2023-05-30 13:15:38.000000 voyandz-0.3.0/src/voyandz/piping.py
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     5887 2023-05-30 13:21:52.000000 voyandz-0.3.0/src/voyandz/server.py
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     1767 2023-05-30 13:15:38.000000 voyandz-0.3.0/src/voyandz/stats.py
+drwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)        0 2023-05-30 13:22:21.761526 voyandz-0.3.0/src/voyandz/templates/
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)      703 2023-05-30 13:15:38.000000 voyandz-0.3.0/src/voyandz/templates/home.html
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     2150 2023-05-30 13:21:52.000000 voyandz-0.3.0/src/voyandz/templates/stat.html
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)      476 2023-05-30 13:15:38.000000 voyandz-0.3.0/src/voyandz/util.py
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)       76 2023-05-30 13:21:52.000000 voyandz-0.3.0/src/voyandz/version.py
+drwxr-xr-x   0 r.zalewski (1563407192) domain users (1563400513)        0 2023-05-30 13:22:21.761526 voyandz-0.3.0/src/voyandz.egg-info/
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)     6029 2023-05-30 13:22:21.000000 voyandz-0.3.0/src/voyandz.egg-info/PKG-INFO
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)      554 2023-05-30 13:22:21.000000 voyandz-0.3.0/src/voyandz.egg-info/SOURCES.txt
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)        1 2023-05-30 13:22:21.000000 voyandz-0.3.0/src/voyandz.egg-info/dependency_links.txt
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)       46 2023-05-30 13:22:21.000000 voyandz-0.3.0/src/voyandz.egg-info/entry_points.txt
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)        1 2023-05-30 13:22:21.000000 voyandz-0.3.0/src/voyandz.egg-info/not-zip-safe
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)       25 2023-05-30 13:22:21.000000 voyandz-0.3.0/src/voyandz.egg-info/requires.txt
+-rw-r--r--   0 r.zalewski (1563407192) domain users (1563400513)        8 2023-05-30 13:22:21.000000 voyandz-0.3.0/src/voyandz.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `voyandz-0.2.5/PKG-INFO` & `voyandz-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,26 @@
 Metadata-Version: 2.1
 Name: voyandz
-Version: 0.2.5
-Summary: Voyoffnik Andzej - an AV HTTP piping server
-Home-page: UNKNOWN
+Version: 0.3.0
+Summary: an AV HTTP piping server
+Home-page: https://github.com/Zalewa/voyandz
 Author: Robikz
 Author-email: zalewapl@gmail.com
-Description-Content-Type: text/markdown
-License: MIT License
-
-Copyright (c) 2018, 2020 - 2021 Robikz <zalewapl@gmail.com>
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
-Description: Voyoffnik Andzej
-        ================
-        
-        Voyoffnik Andzej (voyandz) is a real-time AV streaming server akin to
-        the discontinued `ffserver`. Its primary purpose is to enable network
-        streaming of audio, video or audio & video in form of continuous,
-        non-seekable streams. The source feed can be any feed that can be
-        provided in a streamable form through a preinstalled program such as
-        `ffmpeg`. The output stream can be any stream that can be produced by
-        a preinstalled program such as `ffmpeg`. Voyoffnik Andzej itself
-        doesn't delve into codec details, but merely deals with piping.
+License: MIT
+Description: Voyandz
+        =======
+        
+        Voyandz is a real-time AV streaming server akin to the discontinued
+        `ffserver`. Its primary purpose is to enable network streaming of audio,
+        video or audio & video in form of continuous, non-seekable streams. The
+        source feed can be any feed that can be provided in a streamable form
+        through a preinstalled program such as `ffmpeg`. The output stream can
+        be any stream that can be produced by a preinstalled program such as
+        `ffmpeg`. Voyandz itself doesn't delve into codec details, but merely
+        deals with piping.
         
         `ffmpeg` not attached.
         
         Home page: https://github.com/Zalewa/voyandz/
         
         Installation
         ============
@@ -147,16 +125,16 @@
           |- sandbox - development scraps, experiments
           \- voyandz - application code
         ```
         
         Name
         ====
         
-        V stands for Video, A stands for Audio, ff implies purpose.
-        The rest is gibberish. Short name is `voyandz`, all lower-case.
+        The name is `voyandz`, all lower-case. V stands for video,
+        A stands for Audio, the rest is gibberish.
         
         Troubleshooting
         ===============
         
         **Problem:** Running on Linux and getting
         "cannot modify pipe size: [Errno 1] Operation not permitted"
         error upon heavy load.
@@ -193,7 +171,8 @@
         `/etc/sysctl.d/`.
         
         More info: http://man7.org/linux/man-pages/man7/pipe.7.html
         
         Keywords: pipe-user-pages-soft, PermissionError, Operation not permitted
         
 Platform: UNKNOWN
+Description-Content-Type: text/markdown
```

### Comparing `voyandz-0.2.5/voyandz.egg-info/PKG-INFO` & `voyandz-0.3.0/src/voyandz.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,26 @@
 Metadata-Version: 2.1
 Name: voyandz
-Version: 0.2.5
-Summary: Voyoffnik Andzej - an AV HTTP piping server
-Home-page: UNKNOWN
+Version: 0.3.0
+Summary: an AV HTTP piping server
+Home-page: https://github.com/Zalewa/voyandz
 Author: Robikz
 Author-email: zalewapl@gmail.com
-Description-Content-Type: text/markdown
-License: MIT License
-
-Copyright (c) 2018, 2020 - 2021 Robikz <zalewapl@gmail.com>
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
-Description: Voyoffnik Andzej
-        ================
-        
-        Voyoffnik Andzej (voyandz) is a real-time AV streaming server akin to
-        the discontinued `ffserver`. Its primary purpose is to enable network
-        streaming of audio, video or audio & video in form of continuous,
-        non-seekable streams. The source feed can be any feed that can be
-        provided in a streamable form through a preinstalled program such as
-        `ffmpeg`. The output stream can be any stream that can be produced by
-        a preinstalled program such as `ffmpeg`. Voyoffnik Andzej itself
-        doesn't delve into codec details, but merely deals with piping.
+License: MIT
+Description: Voyandz
+        =======
+        
+        Voyandz is a real-time AV streaming server akin to the discontinued
+        `ffserver`. Its primary purpose is to enable network streaming of audio,
+        video or audio & video in form of continuous, non-seekable streams. The
+        source feed can be any feed that can be provided in a streamable form
+        through a preinstalled program such as `ffmpeg`. The output stream can
+        be any stream that can be produced by a preinstalled program such as
+        `ffmpeg`. Voyandz itself doesn't delve into codec details, but merely
+        deals with piping.
         
         `ffmpeg` not attached.
         
         Home page: https://github.com/Zalewa/voyandz/
         
         Installation
         ============
@@ -147,16 +125,16 @@
           |- sandbox - development scraps, experiments
           \- voyandz - application code
         ```
         
         Name
         ====
         
-        V stands for Video, A stands for Audio, ff implies purpose.
-        The rest is gibberish. Short name is `voyandz`, all lower-case.
+        The name is `voyandz`, all lower-case. V stands for video,
+        A stands for Audio, the rest is gibberish.
         
         Troubleshooting
         ===============
         
         **Problem:** Running on Linux and getting
         "cannot modify pipe size: [Errno 1] Operation not permitted"
         error upon heavy load.
@@ -193,7 +171,8 @@
         `/etc/sysctl.d/`.
         
         More info: http://man7.org/linux/man-pages/man7/pipe.7.html
         
         Keywords: pipe-user-pages-soft, PermissionError, Operation not permitted
         
 Platform: UNKNOWN
+Description-Content-Type: text/markdown
```

### Comparing `voyandz-0.2.5/LICENSE` & `voyandz-0.3.0/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2018, 2020 - 2021 Robikz <zalewapl@gmail.com>
+Copyright (c) 2018, 2020 - 2021, 2023 Robikz <zalewapl@gmail.com>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `voyandz-0.2.5/voyandz/server.py` & `voyandz-0.3.0/src/voyandz/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from voyandz import app, config, logging, piping, stats
+from voyandz import app, config, logging, piping, stats, version
 
 import flask
 import werkzeug.serving
 
 from io import BytesIO
 import datetime
 import json
@@ -71,15 +71,16 @@
     stream_stats = [piping.stream_stats(stream) for stream in all_streams]
     return flask.render_template(
         'stat.html',
         start_date=_start_date.strftime(_DATETIME_FORMAT),
         current_date=now_date.strftime(_DATETIME_FORMAT),
         uptime=uptime,
         feeds=feeds_stats, streams=stream_stats,
-        totals=stats.Totals(feed_stats=feeds_stats, stream_stats=stream_stats))
+        totals=stats.Totals(feed_stats=feeds_stats, stream_stats=stream_stats),
+        server_version=version.VERSION)
 
 
 @app.before_first_request
 def init():
     # Known problem: this can't configure listen port and listen address.
     if not _is_cfg_loaded():
         config.init_app_config(app, None)
```

### Comparing `voyandz-0.2.5/voyandz/logging.py` & `voyandz-0.3.0/src/voyandz/logging.py`

 * *Files identical despite different names*

### Comparing `voyandz-0.2.5/voyandz/cli.py` & `voyandz-0.3.0/src/voyandz/cli.py`

 * *Files identical despite different names*

### Comparing `voyandz-0.2.5/voyandz/piping.py` & `voyandz-0.3.0/src/voyandz/piping.py`

 * *Files identical despite different names*

### Comparing `voyandz-0.2.5/voyandz/templates/home.html` & `voyandz-0.3.0/src/voyandz/templates/home.html`

 * *Files identical despite different names*

### Comparing `voyandz-0.2.5/voyandz/templates/stat.html` & `voyandz-0.3.0/src/voyandz/templates/stat.html`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 			.running { background-color: lime; }
 		</style>
 	</header>
 	<body>
 		<h1>voyandz - stats</h1>
 		<h2>Server</h2>
 		<table>
+			<tr class="data"><th>Version:</th><td>{{ server_version}}</td></tr>
 			<tr class="data"><th>Started on:</th><td>{{ start_date }}</td></tr>
 			<tr class="data"><th>Current time:</th><td>{{ current_date }}</td></tr>
 			<tr class="data"><th>Uptime:</th><td>{{ uptime }}</td></tr>
 		</table>
 		<h2>Totals</h2>
 		<table>
 			<tr class="header">
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
 
 ****** voyandz - stats ******
 ***** Server *****
+Version:      {{ server_version}}
 Started on:   {{ start_date }}
 Current time: {{ current_date }}
 Uptime:       {{ uptime }}
 ***** Totals *****
 Client Transfer              Internal Transfer              Current Clients
 {                            {
 {                            {                              {{ totals.clients
```

### Comparing `voyandz-0.2.5/voyandz/stats.py` & `voyandz-0.3.0/src/voyandz/stats.py`

 * *Files identical despite different names*

### Comparing `voyandz-0.2.5/voyandz/config.py` & `voyandz-0.3.0/src/voyandz/config.py`

 * *Files identical despite different names*

### Comparing `voyandz-0.2.5/README.md` & `voyandz-0.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-Voyoffnik Andzej
-================
+Voyandz
+=======
 
-Voyoffnik Andzej (voyandz) is a real-time AV streaming server akin to
-the discontinued `ffserver`. Its primary purpose is to enable network
-streaming of audio, video or audio & video in form of continuous,
-non-seekable streams. The source feed can be any feed that can be
-provided in a streamable form through a preinstalled program such as
-`ffmpeg`. The output stream can be any stream that can be produced by
-a preinstalled program such as `ffmpeg`. Voyoffnik Andzej itself
-doesn't delve into codec details, but merely deals with piping.
+Voyandz is a real-time AV streaming server akin to the discontinued
+`ffserver`. Its primary purpose is to enable network streaming of audio,
+video or audio & video in form of continuous, non-seekable streams. The
+source feed can be any feed that can be provided in a streamable form
+through a preinstalled program such as `ffmpeg`. The output stream can
+be any stream that can be produced by a preinstalled program such as
+`ffmpeg`. Voyandz itself doesn't delve into codec details, but merely
+deals with piping.
 
 `ffmpeg` not attached.
 
 Home page: https://github.com/Zalewa/voyandz/
 
 Installation
 ============
@@ -117,16 +117,16 @@
   |- sandbox - development scraps, experiments
   \- voyandz - application code
 ```
 
 Name
 ====
 
-V stands for Video, A stands for Audio, ff implies purpose.
-The rest is gibberish. Short name is `voyandz`, all lower-case.
+The name is `voyandz`, all lower-case. V stands for video,
+A stands for Audio, the rest is gibberish.
 
 Troubleshooting
 ===============
 
 **Problem:** Running on Linux and getting
 "cannot modify pipe size: [Errno 1] Operation not permitted"
 error upon heavy load.
```

