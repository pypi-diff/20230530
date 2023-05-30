# Comparing `tmp/py-Ayiin-0.4.3.tar.gz` & `tmp/py-Ayiin-0.4.4.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-Ayiin-0.4.3.tar", last modified: Mon May 29 09:20:58 2023, max compression
+gzip compressed data, was "py-Ayiin-0.4.4.dev1.tar", last modified: Tue May 30 07:26:18 2023, max compression
```

## Comparing `py-Ayiin-0.4.3.tar` & `py-Ayiin-0.4.4.dev1.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:20:58.851706 py-Ayiin-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-29 09:20:58.847706 py-Ayiin-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:20:58.827705 py-Ayiin-0.4.3/pyAyiin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:20:58.831705 py-Ayiin-0.4.3/pyAyiin/Clients/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/Clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12525 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/Clients/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/Clients/pytgcalls.py
--rw-r--r--   0 runner    (1001) docker     (123)    38642 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/Clients/startup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:20:58.835705 py-Ayiin-0.4.3/pyAyiin/dB/
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/dB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/dB/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/dB/absen.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/dB/admins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/dB/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/dB/blacklistfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/dB/blacklistgcast.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/dB/blacklistuser.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/dB/gban.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/dB/langs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/dB/logdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/dB/pmpermit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/dB/premium.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/dB/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/dB/sudo.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/dB/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/dB/videocalls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/dB/welcome.py
--rw-r--r--   0 runner    (1001) docker     (123)    33254 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:20:58.839705 py-Ayiin-0.4.3/pyAyiin/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/methods/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/methods/changer.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/methods/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/methods/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/methods/funcb.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/methods/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/methods/hosting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/methods/inlinebot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/methods/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/methods/thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:20:58.839705 py-Ayiin-0.4.3/pyAyiin/pyrogram/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/pyrogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/pyrogram/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/pyrogram/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/pyrogram/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/pyrogram/pastebin.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/pyrogram/sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/pyrogram/toolbot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/pyrogram/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:20:58.847706 py-Ayiin-0.4.3/pyAyiin/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    31343 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/resources/Youtube.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39497 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/resources/ayiin_music.jpg
--rw-r--r--   0 runner    (1001) docker     (123)  1808670 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/resources/ayiin_ubot.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    60539 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/resources/ayiin_userbot.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/resources/blank.png
--rw-r--r--   0 runner    (1001) docker     (123)    56364 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/resources/default.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   141612 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/resources/font.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   128248 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/resources/font2.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:20:58.847706 py-Ayiin-0.4.3/pyAyiin/telethon/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/telethon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:20:58.847706 py-Ayiin-0.4.3/pyAyiin/telethon/ayiin/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/telethon/ayiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/telethon/ayiin/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/telethon/ayiin/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/telethon/ayiin/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17263 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/pyAyiin/xd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:20:58.847706 py-Ayiin-0.4.3/py_Ayiin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-29 09:20:58.000000 py-Ayiin-0.4.3/py_Ayiin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-29 09:20:58.000000 py-Ayiin-0.4.3/py_Ayiin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 09:20:58.000000 py-Ayiin-0.4.3/py_Ayiin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-29 09:20:58.000000 py-Ayiin-0.4.3/py_Ayiin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-29 09:20:58.000000 py-Ayiin-0.4.3/py_Ayiin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 09:20:58.851706 py-Ayiin-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-29 09:20:41.000000 py-Ayiin-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:26:18.968206 py-Ayiin-0.4.4.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-30 07:26:18.968206 py-Ayiin-0.4.4.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:26:18.964205 py-Ayiin-0.4.4.dev1/pyAyiin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:26:18.964205 py-Ayiin-0.4.4.dev1/pyAyiin/Clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/Clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12525 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/Clients/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/Clients/pytgcalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38642 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/Clients/startup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:26:18.964205 py-Ayiin-0.4.4.dev1/pyAyiin/dB/
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/dB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/dB/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/dB/absen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/dB/admins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/dB/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/dB/blacklistfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/dB/blacklistgcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/dB/blacklistuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/dB/gban.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/dB/langs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/dB/logdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/dB/pmpermit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/dB/premium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/dB/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/dB/sudo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/dB/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/dB/videocalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/dB/welcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33254 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:26:18.964205 py-Ayiin-0.4.4.dev1/pyAyiin/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/methods/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/methods/changer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/methods/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/methods/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/methods/funcb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/methods/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/methods/hosting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/methods/inlinebot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/methods/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/methods/thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:26:18.964205 py-Ayiin-0.4.4.dev1/pyAyiin/pyrogram/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/pyrogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/pyrogram/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/pyrogram/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/pyrogram/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/pyrogram/pastebin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/pyrogram/sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/pyrogram/toolbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/pyrogram/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:26:18.968206 py-Ayiin-0.4.4.dev1/pyAyiin/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    31343 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/resources/Youtube.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39497 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/resources/ayiin_music.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)  1808670 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/resources/ayiin_ubot.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    60539 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/resources/ayiin_userbot.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/resources/blank.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56364 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/resources/default.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   141612 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/resources/font.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   128248 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/resources/font2.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:26:18.968206 py-Ayiin-0.4.4.dev1/pyAyiin/telethon/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/telethon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:26:18.968206 py-Ayiin-0.4.4.dev1/pyAyiin/telethon/ayiin/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/telethon/ayiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/telethon/ayiin/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/telethon/ayiin/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/telethon/ayiin/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17263 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/pyAyiin/xd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 07:26:18.968206 py-Ayiin-0.4.4.dev1/py_Ayiin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-30 07:26:18.000000 py-Ayiin-0.4.4.dev1/py_Ayiin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-30 07:26:18.000000 py-Ayiin-0.4.4.dev1/py_Ayiin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 07:26:18.000000 py-Ayiin-0.4.4.dev1/py_Ayiin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-30 07:26:18.000000 py-Ayiin-0.4.4.dev1/py_Ayiin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-30 07:26:18.000000 py-Ayiin-0.4.4.dev1/py_Ayiin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 07:26:18.968206 py-Ayiin-0.4.4.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-30 07:26:05.000000 py-Ayiin-0.4.4.dev1/setup.py
```

### Comparing `py-Ayiin-0.4.3/LICENSE` & `py-Ayiin-0.4.4.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/NOTICE` & `py-Ayiin-0.4.4.dev1/NOTICE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/PKG-INFO` & `py-Ayiin-0.4.4.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.4.3
+Version: 0.4.4.dev1
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.4.3/README.md` & `py-Ayiin-0.4.4.dev1/README.md`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/Clients/__init__.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/Clients/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/Clients/client.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/Clients/client.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/Clients/pytgcalls.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/Clients/pytgcalls.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/Clients/startup.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/Clients/startup.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/__init__.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 
 logs = logging.getLogger(__name__)
 
 
 __copyright__ = "Copyright (C) 2022-present AyiinXd <https://github.com/AyiinXd>"
 __license__ = "GNU General Public License v3.0 (GPL-3.0)"
-__version__ = "0.4.3"
+__version__ = "0.4.4.dev01"
 ayiin_ver = "0.1.1"
 
 
 DEVS = [
     607067484, # Ayiin
     997461844, #Ayang_Ayiin
     2130526178, # Alfa
```

### Comparing `py-Ayiin-0.4.3/pyAyiin/__main__.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/__main__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/assistant.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/assistant.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/config.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/config.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/dB/__init__.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/dB/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/dB/absen.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/dB/absen.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/dB/admins.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/dB/admins.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/dB/auth.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/dB/auth.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/dB/blacklistfilter.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/dB/blacklistfilter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/dB/blacklistgcast.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/dB/blacklistgcast.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/dB/blacklistuser.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/dB/blacklistuser.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/dB/gban.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/dB/gban.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/dB/langs.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/dB/langs.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/dB/logdb.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/dB/logdb.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/dB/pmpermit.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/dB/pmpermit.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/dB/premium.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/dB/premium.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/dB/start.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/dB/start.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/dB/sudo.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/dB/sudo.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/dB/variable.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/dB/variable.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/dB/videocalls.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/dB/videocalls.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/dB/welcome.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/dB/welcome.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/decorator.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/decorator.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/exceptions.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/methods/__init__.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/methods/_misc.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/methods/_misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/methods/changer.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/methods/changer.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/methods/converter.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/methods/converter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/methods/func.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/methods/func.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/methods/funcb.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/methods/funcb.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/methods/helpers.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/methods/helpers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/methods/hosting.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/methods/hosting.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/methods/inlinebot.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/methods/inlinebot.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/methods/queue.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/methods/queue.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/methods/thumbnail.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/methods/thumbnail.py`

 * *Files 15% similar despite different names*

```diff
@@ -37,26 +37,32 @@
         newHeight = int(heightRatio * image.size[1])
         newImage = image.resize((newWidth, newHeight))
         return newImage
 
 
     async def gen_thumb(
         self, 
-        client, 
+        client,
+        chat_id,
         videoid,
+        file_path,
+        cache,
+        cache_thumb,
+        fonts,
+        fonts2,
     ):
         # cache = f"cache/{videoid}.png"
         # cache_thumb = f"cache/thumb{videoid}.png"
         # fonts = "assets/font.ttf"
         # fonts2 = "assets/font2.ttf"
-        if not os.path.isdir('../cache/'):
-            os.makedirs('../cache/')
+        if not os.path.isdir(file_path):
+            os.makedirs(file_path)
 
-        if os.path.isfile(f"cache/{videoid}.png"):
-            return f"cache/{videoid}.png"
+        if os.path.isfile(cache):
+            return cache
 
         url = f"https://www.youtube.com/watch?v={videoid}"
         try:
             results = VideosSearch(url, limit=1)
             for result in (await results.next())["result"]:
                 try:
                     title = result["title"]
@@ -78,20 +84,20 @@
                 except BaseException:
                     channel = "Unknown Channel"
 
             async with aiohttp.ClientSession() as session:
                 async with session.get(thumbnail) as resp:
                     if resp.status == 200:
                         f = await aiofiles.open(
-                            f"cache/thumb{videoid}.png", mode="wb"
+                            cache_thumb, mode="wb"
                         )
                         await f.write(await resp.read())
                         await f.close()
 
-            youtube = Image.open(f"cache/thumb{videoid}.png")
+            youtube = Image.open(cache_thumb)
             image1 = self.changeImageSize(1280, 720, youtube)
             image2 = image1.convert("RGBA")
             background = image2.filter(filter=ImageFilter.BoxBlur(30))
             enhancer = ImageEnhance.Brightness(background)
             background = enhancer.enhance(0.6)
             Xcenter = youtube.width / 2
             Ycenter = youtube.height / 2
@@ -100,18 +106,18 @@
             x2 = Xcenter + 250
             y2 = Ycenter + 250
             logo = youtube.crop((x1, y1, x2, y2))
             logo.thumbnail((520, 520), Image.ANTIALIAS)
             logo = ImageOps.expand(logo, border=15, fill="white")
             background.paste(logo, (50, 100))
             draw = ImageDraw.Draw(background)
-            font = ImageFont.truetype("./resources/font.ttf2", 40)
-            font2 = ImageFont.truetype("./resources/font.ttf2", 70)
-            arial = ImageFont.truetype("./resources/font.ttf2", 30)
-            name_font = ImageFont.truetype("./resources/font.ttf", 35)
+            font = ImageFont.truetype(fonts2, 40)
+            font2 = ImageFont.truetype(fonts2, 70)
+            arial = ImageFont.truetype(fonts2, 30)
+            name_font = ImageFont.truetype(fonts, 35)
             para = textwrap.wrap(title, width=32)
             me = await client.get_me()
             uname = me.username
             music_name = f'{uname.upper()} UBOT' if uname else 'AYIIN UBOT'
             j = 0
             draw.text(
                 (30, 5), f"{music_name}", fill="white", font=name_font
@@ -161,17 +167,18 @@
             draw.text(
                 (600, 550),
                 f"Channel : {channel}",
                 (255, 255, 255),
                 font=arial,
             )
             try:
-                os.remove(f"cache/thumb{videoid}.png")
+                os.remove(cache_thumb)
             except BaseException:
                 pass
-            background.save(f"cache/{videoid}.png")
-            return f"cache/{videoid}.png"
-        except Exception:
+            background.save(cache)
+            return cache
+        except BaseException as e:
+            await client.send_message(chat_id, f'THUMBNAIL ERROR: {e}')
             results = VideosSearch(url, limit=1)
             for result in results.result()["result"]:
                 thumbnail = result["thumbnails"][0]["url"].split("?")[0]
             return thumbnail
```

### Comparing `py-Ayiin-0.4.3/pyAyiin/pyrogram/__init__.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/pyrogram/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/pyrogram/_wrappers.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/pyrogram/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/pyrogram/func.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/pyrogram/func.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/pyrogram/misc.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/pyrogram/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/pyrogram/pastebin.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/pyrogram/pastebin.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/pyrogram/sections.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/pyrogram/sections.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/pyrogram/toolbot.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/pyrogram/toolbot.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/pyrogram/tools.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/pyrogram/tools.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/resources/Youtube.jpeg` & `py-Ayiin-0.4.4.dev1/pyAyiin/resources/Youtube.jpeg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/resources/ayiin_music.jpg` & `py-Ayiin-0.4.4.dev1/pyAyiin/resources/ayiin_music.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/resources/ayiin_ubot.jpg` & `py-Ayiin-0.4.4.dev1/pyAyiin/resources/ayiin_ubot.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/resources/ayiin_userbot.jpg` & `py-Ayiin-0.4.4.dev1/pyAyiin/resources/ayiin_userbot.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/resources/blank.png` & `py-Ayiin-0.4.4.dev1/pyAyiin/resources/blank.png`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/resources/default.ttf` & `py-Ayiin-0.4.4.dev1/pyAyiin/resources/default.ttf`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/resources/font.ttf` & `py-Ayiin-0.4.4.dev1/pyAyiin/resources/font.ttf`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/resources/font2.ttf` & `py-Ayiin-0.4.4.dev1/pyAyiin/resources/font2.ttf`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/telethon/ayiin/_wrappers.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/telethon/ayiin/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/telethon/ayiin/events.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/telethon/ayiin/events.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/telethon/ayiin/misc.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/telethon/ayiin/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/pyAyiin/xd.py` & `py-Ayiin-0.4.4.dev1/pyAyiin/xd.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/py_Ayiin.egg-info/PKG-INFO` & `py-Ayiin-0.4.4.dev1/py_Ayiin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.4.3
+Version: 0.4.4.dev1
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.4.3/py_Ayiin.egg-info/SOURCES.txt` & `py-Ayiin-0.4.4.dev1/py_Ayiin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.3/setup.py` & `py-Ayiin-0.4.4.dev1/setup.py`

 * *Files identical despite different names*

