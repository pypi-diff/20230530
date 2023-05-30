# Comparing `tmp/nonebot-plugin-sky-2.2.8.tar.gz` & `tmp/nonebot-plugin-sky-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-sky-2.2.8.tar", last modified: Fri May 26 14:24:34 2023, max compression
+gzip compressed data, was "nonebot-plugin-sky-2.2.9.tar", last modified: Tue May 30 05:09:19 2023, max compression
```

## Comparing `nonebot-plugin-sky-2.2.8.tar` & `nonebot-plugin-sky-2.2.9.tar`

### file list

```diff
@@ -1,64 +1,62 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 14:24:34.601519 nonebot-plugin-sky-2.2.8/
--rw-rw-rw-   0        0        0    35823 2022-11-03 06:35:38.000000 nonebot-plugin-sky-2.2.8/LICENSE
--rw-rw-rw-   0        0        0    15639 2023-05-26 14:24:34.600521 nonebot-plugin-sky-2.2.8/PKG-INFO
--rw-rw-rw-   0        0        0    15115 2023-05-26 14:21:53.000000 nonebot-plugin-sky-2.2.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 14:24:34.402052 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/
--rw-rw-rw-   0        0        0     7665 2023-05-26 14:18:37.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 14:24:34.420006 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/config/
--rw-rw-rw-   0        0        0        0 2023-03-01 11:49:56.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/config/__init__.py
--rw-rw-rw-   0        0        0     5707 2023-03-07 11:28:55.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/config/command.py
--rw-rw-rw-   0        0        0     1810 2023-03-01 11:52:50.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/config/helper_at_all.py
--rw-rw-rw-   0        0        0     1258 2023-05-26 12:48:02.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/config/load_config.py
--rw-rw-rw-   0        0        0     1748 2023-05-26 12:48:02.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/config/msg_forward.py
--rw-rw-rw-   0        0        0     1628 2023-05-26 12:48:02.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/config/travelling_cache.py
-drwxrwxrwx   0        0        0        0 2023-05-26 14:24:34.436959 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/guild/
--rw-rw-rw-   0        0        0     1160 2023-02-24 11:32:34.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/guild/__init__.py
--rw-rw-rw-   0        0        0        0 2023-01-19 11:25:12.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/guild/light_beauty.py
--rw-rw-rw-   0        0        0        0 2023-01-19 11:25:12.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/guild/light_cute.py
-drwxrwxrwx   0        0        0        0 2023-05-26 14:24:34.460895 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/
--rw-rw-rw-   0        0        0        0 2023-03-01 11:48:13.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 14:24:34.476852 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/daily_tasks/
--rw-rw-rw-   0        0        0        0 2023-03-01 11:48:13.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/daily_tasks/__init__.py
--rw-rw-rw-   0        0        0     2547 2023-04-05 11:09:22.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/daily_tasks/international.py
--rw-rw-rw-   0        0        0     3077 2023-04-05 11:09:22.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/daily_tasks/national.py
--rw-rw-rw-   0        0        0   459817 2023-04-30 01:49:58.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/get_id.png
--rw-rw-rw-   0        0        0      637 2023-03-07 11:28:55.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/public_notice.py
--rw-rw-rw-   0        0        0    14200 2023-05-26 12:48:02.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/query_tools.py
--rw-rw-rw-   0        0        0     1083 2023-05-26 12:48:02.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/queue.py
-drwxrwxrwx   0        0        0        0 2023-05-26 14:24:34.484831 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/travelling_spirit/
--rw-rw-rw-   0        0        0        0 2023-03-01 12:32:18.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/travelling_spirit/__init__.py
--rw-rw-rw-   0        0        0     3225 2023-05-26 12:48:02.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/travelling_spirit/international.py
--rw-rw-rw-   0        0        0     3207 2023-05-26 12:48:02.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/travelling_spirit/national.py
-drwxrwxrwx   0        0        0        0 2023-05-26 14:24:34.493807 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/
--rw-rw-rw-   0        0        0        0 2023-03-01 11:50:17.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 14:24:34.553647 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/helper_image/
--rw-rw-rw-   0        0        0    16051 2022-12-30 12:12:29.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/helper_image/eating.jpg
--rw-rw-rw-   0        0        0    89789 2022-12-30 12:12:29.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/helper_image/face_braid.gif
--rw-rw-rw-   0        0        0    79644 2022-12-30 12:12:29.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/helper_image/face_bun.gif
--rw-rw-rw-   0        0        0    72146 2022-12-30 12:12:29.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/helper_image/face_cat.gif
--rw-rw-rw-   0        0        0    87935 2022-12-30 12:12:29.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/helper_image/face_fox.gif
--rw-rw-rw-   0        0        0    80542 2022-12-30 12:12:29.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/helper_image/face_white_cat.gif
--rw-rw-rw-   0        0        0    95522 2022-12-30 12:12:29.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/helper_image/go.jpg
--rw-rw-rw-   0        0        0      274 2023-01-02 06:48:03.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/menu.py
-drwxrwxrwx   0        0        0        0 2023-05-26 14:24:34.562624 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/menu_image/
--rw-rw-rw-   0        0        0   824527 2022-12-30 12:12:29.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/menu_image/menu.png
--rw-rw-rw-   0        0        0       97 2023-05-26 12:48:02.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/pusher.py
--rw-rw-rw-   0        0        0     3907 2023-05-26 12:48:02.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/scheduler.py
-drwxrwxrwx   0        0        0        0 2023-05-26 14:24:34.598527 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/utils_/
--rw-rw-rw-   0        0        0     2280 2023-04-05 11:09:22.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/utils_/__init__.py
--rw-rw-rw-   0        0        0      405 2022-12-22 07:28:55.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/utils_/bot_loader.py
--rw-rw-rw-   0        0        0      607 2023-03-01 12:37:46.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/utils_/chain_reply.py
--rw-rw-rw-   0        0        0     5064 2023-05-26 12:48:02.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/utils_/check_update.py
--rw-rw-rw-   0        0        0     6447 2023-05-26 12:48:02.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/utils_/data_pack.py
--rw-rw-rw-   0        0        0      391 2023-02-24 11:32:34.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/utils_/date_util.py
--rw-rw-rw-   0        0        0      746 2023-03-01 11:52:50.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/utils_/json_cards.py
--rw-rw-rw-   0        0        0     1264 2023-04-30 01:49:58.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/utils_/notice_board.py
--rw-rw-rw-   0        0        0     6565 2023-05-26 14:17:51.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/utils_/travel_cycle.py
-drwxrwxrwx   0        0        0        0 2023-05-26 14:24:34.410031 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky.egg-info/
--rw-rw-rw-   0        0        0    15639 2023-05-26 14:24:33.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2026 2023-05-26 14:24:34.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 14:24:33.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-05-26 14:24:33.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-26 14:24:33.000000 nonebot-plugin-sky-2.2.8/nonebot_plugin_sky.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 14:24:34.601519 nonebot-plugin-sky-2.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1450 2023-05-26 12:48:02.000000 nonebot-plugin-sky-2.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 05:09:19.166185 nonebot-plugin-sky-2.2.9/
+-rw-rw-rw-   0        0        0    35823 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/LICENSE
+-rw-rw-rw-   0        0        0    15786 2023-05-30 05:09:19.165188 nonebot-plugin-sky-2.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0    15262 2023-05-30 05:08:23.000000 nonebot-plugin-sky-2.2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 05:09:19.102356 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/
+-rw-rw-rw-   0        0        0     7697 2023-05-30 04:59:27.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 05:09:19.117315 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/config/
+-rw-rw-rw-   0        0        0        0 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/config/__init__.py
+-rw-rw-rw-   0        0        0     5707 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/config/command.py
+-rw-rw-rw-   0        0        0     1810 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/config/helper_at_all.py
+-rw-rw-rw-   0        0        0     1258 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/config/load_config.py
+-rw-rw-rw-   0        0        0     1748 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/config/msg_forward.py
+-rw-rw-rw-   0        0        0     1628 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/config/travelling_cache.py
+drwxrwxrwx   0        0        0        0 2023-05-30 05:09:19.121305 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/guild/
+-rw-rw-rw-   0        0        0     1160 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/guild/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/guild/light_beauty.py
+-rw-rw-rw-   0        0        0        0 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/guild/light_cute.py
+drwxrwxrwx   0        0        0        0 2023-05-30 05:09:19.124297 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/
+-rw-rw-rw-   0        0        0        0 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 05:09:19.128286 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/daily_tasks/
+-rw-rw-rw-   0        0        0        0 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/daily_tasks/__init__.py
+-rw-rw-rw-   0        0        0     2547 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/daily_tasks/international.py
+-rw-rw-rw-   0        0        0     3077 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/daily_tasks/national.py
+-rw-rw-rw-   0        0        0      637 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/public_notice.py
+-rw-rw-rw-   0        0        0     1083 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/queue.py
+drwxrwxrwx   0        0        0        0 2023-05-30 05:09:19.132275 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/travelling_spirit/
+-rw-rw-rw-   0        0        0        0 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/travelling_spirit/__init__.py
+-rw-rw-rw-   0        0        0     3225 2023-05-26 10:18:30.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/travelling_spirit/international.py
+-rw-rw-rw-   0        0        0     3369 2023-05-30 04:53:54.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/travelling_spirit/national.py
+drwxrwxrwx   0        0        0        0 2023-05-30 05:09:19.139257 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/
+-rw-rw-rw-   0        0        0        0 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 05:09:19.151224 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/helper_image/
+-rw-rw-rw-   0        0        0    16051 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/helper_image/eating.jpg
+-rw-rw-rw-   0        0        0    89789 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/helper_image/face_braid.gif
+-rw-rw-rw-   0        0        0    79644 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/helper_image/face_bun.gif
+-rw-rw-rw-   0        0        0    72146 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/helper_image/face_cat.gif
+-rw-rw-rw-   0        0        0    87935 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/helper_image/face_fox.gif
+-rw-rw-rw-   0        0        0    80542 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/helper_image/face_white_cat.gif
+-rw-rw-rw-   0        0        0    95522 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/helper_image/go.jpg
+-rw-rw-rw-   0        0        0      274 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/menu.py
+drwxrwxrwx   0        0        0        0 2023-05-30 05:09:19.153219 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/menu_image/
+-rw-rw-rw-   0        0        0   824527 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/menu_image/menu.png
+-rw-rw-rw-   0        0        0       97 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/pusher.py
+-rw-rw-rw-   0        0        0     3907 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/scheduler.py
+drwxrwxrwx   0        0        0        0 2023-05-30 05:09:19.164190 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/utils_/
+-rw-rw-rw-   0        0        0     2280 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/utils_/__init__.py
+-rw-rw-rw-   0        0        0      405 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/utils_/bot_loader.py
+-rw-rw-rw-   0        0        0      607 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/utils_/chain_reply.py
+-rw-rw-rw-   0        0        0     5064 2023-05-30 05:08:23.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/utils_/check_update.py
+-rw-rw-rw-   0        0        0     6447 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/utils_/data_pack.py
+-rw-rw-rw-   0        0        0      391 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/utils_/date_util.py
+-rw-rw-rw-   0        0        0      746 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/utils_/json_cards.py
+-rw-rw-rw-   0        0        0     1264 2023-05-26 02:54:29.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/utils_/notice_board.py
+-rw-rw-rw-   0        0        0     6554 2023-05-30 04:55:58.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/utils_/travel_cycle.py
+drwxrwxrwx   0        0        0        0 2023-05-30 05:09:19.110335 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky.egg-info/
+-rw-rw-rw-   0        0        0    15786 2023-05-30 05:09:19.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1954 2023-05-30 05:09:19.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 05:09:19.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-05-30 05:09:19.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-30 05:09:19.000000 nonebot-plugin-sky-2.2.9/nonebot_plugin_sky.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 05:09:19.166185 nonebot-plugin-sky-2.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1450 2023-05-30 05:08:23.000000 nonebot-plugin-sky-2.2.9/setup.py
```

### Comparing `nonebot-plugin-sky-2.2.8/LICENSE` & `nonebot-plugin-sky-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.8/PKG-INFO` & `nonebot-plugin-sky-2.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sky
-Version: 2.2.8
+Version: 2.2.9
 Summary: nonebot2 plugin sky
 Home-page: https://github.com/Kaguya233qwq/nonebot_plugin_sky
 Author: Kaguya233qwq
 Author-email: 1435608435@qq.com
 Keywords: pip,nonebot2,nonebot,sky光遇,光遇
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -280,14 +280,18 @@
 
 新浪微博@张张幼稚园 —> *攻略内容*
 
 新浪微博&哔哩哔哩@木易不高兴了啊 —> *攻略内容*
 
 ## ✨更新日志✨
 
+2023.5.30 v2.2.9
+
+这个版本修复了上版本复刻缓存方法调用错误的问题，现在可以智能化识别国服通常复刻周期
+
 2023.5.22 v2.2.8
 
 新增国服通用复刻周期函数，国服复刻已更新，国际服复刻维护中。新增若干随机文案
 
 2023.4.30 v2.2.7
 
 1.在这个版本之后所有querytools命令均废弃不再生效。
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sky Version: 2.2.8 Summary: nonebot2
+Metadata-Version: 2.1 Name: nonebot-plugin-sky Version: 2.2.9 Summary: nonebot2
 plugin sky Home-page: https://github.com/Kaguya233qwq/nonebot_plugin_sky
 Author: Kaguya233qwq Author-email: 1435608435@qq.com Keywords:
 pip,nonebot2,nonebot,skyåé,åé Platform: any Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Natural Language :: Chinese (Simplified)
 Description-Content-Type: text/markdown License-File: LICENSE
                                      [sky]
@@ -106,15 +106,17 @@
 (ç¾¤æä»¶æä¸é®å¯å¨å)
                                      [sky]
 ## â¨æè°¢ååï¼ä¸åååï¼â¨ æ°æµªå¾®å@åéééååå â>
 *æ»ç¥åå®¹* æ°æµªå¾®å@æ§æ¥ä¸æ¥ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@ä»å¤©æ¸¸ç¦»ç¿»è½¦äºå â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@å¼ å¼ å¹¼ç¨å­ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å&åå©åå©@æ¨æä¸é«å´äºå â> *æ»ç¥åå®¹* ##
-â¨æ´æ°æ¥å¿â¨ 2023.5.22 v2.2.8
+â¨æ´æ°æ¥å¿â¨ 2023.5.30 v2.2.9
+è¿ä¸ªçæ¬ä¿®å¤äºä¸çæ¬å¤å»ç¼å­æ¹æ³è°ç¨éè¯¯çé®é¢ï¼ç°å¨å¯ä»¥æºè½åè¯å«å½æéå¸¸å¤å»å¨æ
+2023.5.22 v2.2.8
 æ°å¢å½æéç¨å¤å»å¨æå½æ°ï¼å½æå¤å»å·²æ´æ°ï¼å½éæå¤å»ç»´æ¤ä¸­ãæ°å¢è¥å¹²éæºææ¡
 2023.4.30 v2.2.7
 1.å¨è¿ä¸ªçæ¬ä¹åææquerytoolså½ä»¤ååºå¼ä¸åçæã
 2.æ´æ°å­£èæ¶é´ï¼ææ¶ä¸æ¯å¾åç¡® 2023.4.25 v2.2.6
 1.ä¿®å¤è·åuidå¸®å©å¾çæ æ³åéçé®é¢
 2.å½å¤äºå­£èçç©ºææ¶æ¥è¯¢å­£è¡ãè¡çæ°è¿åç¸åºæç¤º
 2023.4.12 v2.2.5.post2 ä¿®å¤å·²ç¥é®é¢ 2023.4.4 v2.2.5.post1
```

### Comparing `nonebot-plugin-sky-2.2.8/README.md` & `nonebot-plugin-sky-2.2.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -265,14 +265,18 @@
 
 新浪微博@张张幼稚园 —> *攻略内容*
 
 新浪微博&哔哩哔哩@木易不高兴了啊 —> *攻略内容*
 
 ## ✨更新日志✨
 
+2023.5.30 v2.2.9
+
+这个版本修复了上版本复刻缓存方法调用错误的问题，现在可以智能化识别国服通常复刻周期
+
 2023.5.22 v2.2.8
 
 新增国服通用复刻周期函数，国服复刻已更新，国际服复刻维护中。新增若干随机文案
 
 2023.4.30 v2.2.7
 
 1.在这个版本之后所有querytools命令均废弃不再生效。
```

#### html2text {}

```diff
@@ -99,15 +99,17 @@
 (ç¾¤æä»¶æä¸é®å¯å¨å)
                                      [sky]
 ## â¨æè°¢ååï¼ä¸åååï¼â¨ æ°æµªå¾®å@åéééååå â>
 *æ»ç¥åå®¹* æ°æµªå¾®å@æ§æ¥ä¸æ¥ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@ä»å¤©æ¸¸ç¦»ç¿»è½¦äºå â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@å¼ å¼ å¹¼ç¨å­ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å&åå©åå©@æ¨æä¸é«å´äºå â> *æ»ç¥åå®¹* ##
-â¨æ´æ°æ¥å¿â¨ 2023.5.22 v2.2.8
+â¨æ´æ°æ¥å¿â¨ 2023.5.30 v2.2.9
+è¿ä¸ªçæ¬ä¿®å¤äºä¸çæ¬å¤å»ç¼å­æ¹æ³è°ç¨éè¯¯çé®é¢ï¼ç°å¨å¯ä»¥æºè½åè¯å«å½æéå¸¸å¤å»å¨æ
+2023.5.22 v2.2.8
 æ°å¢å½æéç¨å¤å»å¨æå½æ°ï¼å½æå¤å»å·²æ´æ°ï¼å½éæå¤å»ç»´æ¤ä¸­ãæ°å¢è¥å¹²éæºææ¡
 2023.4.30 v2.2.7
 1.å¨è¿ä¸ªçæ¬ä¹åææquerytoolså½ä»¤ååºå¼ä¸åçæã
 2.æ´æ°å­£èæ¶é´ï¼ææ¶ä¸æ¯å¾åç¡® 2023.4.25 v2.2.6
 1.ä¿®å¤è·åuidå¸®å©å¾çæ æ³åéçé®é¢
 2.å½å¤äºå­£èçç©ºææ¶æ¥è¯¢å­£è¡ãè¡çæ°è¿åç¸åºæç¤º
 2023.4.12 v2.2.5.post2 ä¿®å¤å·²ç¥é®é¢ 2023.4.4 v2.2.5.post1
```

### Comparing `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/__init__.py` & `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,27 +9,26 @@
 from nonebot.adapters.onebot.v11 import NetworkError, ActionFailed, Bot, MessageEvent
 
 from .config.command import *
 from .config.msg_forward import *
 from .sky.daily_tasks.international import SkyDaily as Task_in
 from .sky.daily_tasks.national import SkyDaily as Task_cn
 from .sky.public_notice import get_sky_notice
-from .sky.query_tools import *
 from .sky.queue import get_state
 from .sky.travelling_spirit.international import get_data
 from .sky.travelling_spirit.national import Travelling as Travelling_cn
 from .tools.menu import get_menu
 from .tools.scheduler import *
 from .utils_ import send_forward_msg
 from .utils_.chain_reply import chain_reply
 from .utils_.check_update import *
 from .utils_.data_pack import *
 from .utils_.notice_board import *
 from .config.travelling_cache import *
-from .utils_.travel_cycle import download_img, is_exist, NormalTravel,bot_tips
+from .utils_.travel_cycle import download_img, is_exist, NormalTravel, bot_tips
 
 Menu = on_command("Sky", aliases=get_cmd_alias("sky_menu"))
 DailyCN = on_command("sky -cn", aliases=get_cmd_alias("sky_cn"))
 DailyIN = on_command("sky -in", aliases=get_cmd_alias("sky_in"))
 TravellingCN = on_command("travel -cn", aliases=get_cmd_alias("travel_cn"))
 TravellingIN = on_command("travel -in", aliases=get_cmd_alias("travel_in"))
 RemainCN = on_command("remain -cn", aliases=get_cmd_alias("remain_cn"))
@@ -123,37 +122,38 @@
     travel = NormalTravel()
     try:
 
         status = travel.national()
         tips = bot_tips(status)
         if status.get('status') is True:
             # 如果在复刻期间内就判断有无缓存
-            release_time = status.get('current_release').strip(' 12:00:00')
+            release_time = status.get('current_release').replace(' 12:00:00', '')
             cache = is_exist(release_time)
             if cache:
                 # 如果有复刻缓存则发送缓存
                 await TravellingCN.send(MessageSegment.image(cache))
             else:
                 # 没有就执行实时调用
                 travelling = Travelling_cn()
                 img_url = await travelling.get_data()
                 if img_url:
-                    # 将收到的url下载下来并发送
-                    await download_img(img_url, release_time)
                     cache = is_exist(release_time)
-                    await TravellingCN.send(cache)
+                    if cache:
+                        await TravellingCN.send(MessageSegment.image(cache))
+                    else:
+                        await TravellingCN.send('发送图片缓存失败！请联系开发者解决')
                 else:
                     await TravellingCN.send('没有找到国服复刻先祖的数据')
         else:
             # 如果不在复刻期间，则发送提示信息
             await TravellingCN.send(
                 f'当前无复刻先祖信息，下次复刻公布时间：\n{status.get("next_release")}'
             )
-            await asyncio.sleep(2)
-            await TravellingCN.send(tips)
+        await asyncio.sleep(2)
+        await TravellingCN.send(tips)
     except (NetworkError, ActionFailed):
         logger.error('网络环境较差，调用发送信息接口超时')
         await TravellingCN.send(
             message='网络环境较差，调用发送信息接口超时'
         )
```

### Comparing `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/config/command.py` & `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/config/command.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/config/helper_at_all.py` & `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/config/helper_at_all.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/config/load_config.py` & `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/config/load_config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/config/msg_forward.py` & `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/config/msg_forward.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/config/travelling_cache.py` & `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/config/travelling_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/guild/__init__.py` & `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/guild/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/daily_tasks/international.py` & `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/daily_tasks/international.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/daily_tasks/national.py` & `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/daily_tasks/national.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/public_notice.py` & `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/public_notice.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/queue.py` & `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/queue.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/travelling_spirit/international.py` & `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/travelling_spirit/international.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/sky/travelling_spirit/national.py` & `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/sky/travelling_spirit/national.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 from typing import Union
 
 import httpx
 from nonebot import logger
-from nonebot.adapters.onebot.v11 import MessageSegment
 
+from ...utils_.travel_cycle import NormalTravel
 from ...utils_ import time_no_more, weibo_image
 
 
 class Travelling:
     """国服复刻类"""
 
     def __init__(self):
@@ -54,24 +54,27 @@
                             return log
                 else:
                     return 'invalid'
         return None
 
     async def get_data(self) -> Union[str, None]:
         """获取复刻数据"""
+        travel = NormalTravel()
+        status = travel.national()
         results = ''
         overhead = await self.get_mblog(2)
         if overhead == 'invalid':
             return '超过未登录能获取页数的最大值：2'
         if overhead:
             pic_infos = overhead.get('pic_infos')
             if pic_infos:
                 for pic in pic_infos:
                     large_url = pic_infos[pic]['largest']['url']
-                    path = await weibo_image(large_url, pic)
+                    release_time = status.get('current_release').replace(' 12:00:00', '')
+                    path = await weibo_image(large_url, release_time)
                     results = path
             else:
                 results = None
         else:
             notice = '没有找到国服复刻先祖的数据'
             logger.warning(notice)
             results = None
```

### Comparing `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/helper_image/eating.jpg` & `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/helper_image/eating.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/helper_image/face_braid.gif` & `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/helper_image/face_braid.gif`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/helper_image/face_bun.gif` & `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/helper_image/face_bun.gif`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/helper_image/face_cat.gif` & `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/helper_image/face_cat.gif`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/helper_image/face_fox.gif` & `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/helper_image/face_fox.gif`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/helper_image/face_white_cat.gif` & `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/helper_image/face_white_cat.gif`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/helper_image/go.jpg` & `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/helper_image/go.jpg`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/menu_image/menu.png` & `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/menu_image/menu.png`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/tools/scheduler.py` & `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/tools/scheduler.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/utils_/__init__.py` & `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/utils_/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/utils_/chain_reply.py` & `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/utils_/chain_reply.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/utils_/check_update.py` & `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/utils_/check_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import logging
 
 from nonebot import on_command, logger
 from ..config.command import get_cmd_alias
 
 logging.captureWarnings(True)  # 去掉建议使用SSL验证的显示
 
-Version = '2.2.8'  # 全局插件版本信息  （不用加v！）
+Version = '2.2.9'  # 全局插件版本信息  （不用加v！）
 
 
 async def get_datapack_ver():
     """
     检查本地数据包版本
     """
     try:
```

### Comparing `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/utils_/data_pack.py` & `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/utils_/data_pack.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/utils_/json_cards.py` & `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/utils_/json_cards.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/utils_/notice_board.py` & `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/utils_/notice_board.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky/utils_/travel_cycle.py` & `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky/utils_/travel_cycle.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
 
 async def download_img(img_url: str, file_name: str):
     """
     下载复刻图片到本地
     """
     try:
-        path = f'Sky/TravelCache/{file_name}.jpg'
+        path = f'Sky/Cache/{file_name}.jpg'
         async with httpx.AsyncClient() as client:
             res = await client.get(
                 url=img_url
             ).content
         with open(path, 'wb') as f:
             f.write(res)
         logger.success('复刻先祖图片保存成功')
@@ -92,16 +92,16 @@
 
 
 def is_exist(file_name: str):
     """
     本地是否存在复刻缓存
     :return:
     """
-    path = f'Sky/TravelCache/{file_name}.jpg'
-    if os.path.isdir(path):
+    path = f'Sky/Cache/{file_name}.jpg'
+    if os.path.isfile(path):
         abs_path = os.path.abspath(path)
         return f'file:///{abs_path}'
     return False
 
 
 def bot_tips(struct: dict) -> str:
     """
```

### Comparing `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky.egg-info/PKG-INFO` & `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sky
-Version: 2.2.8
+Version: 2.2.9
 Summary: nonebot2 plugin sky
 Home-page: https://github.com/Kaguya233qwq/nonebot_plugin_sky
 Author: Kaguya233qwq
 Author-email: 1435608435@qq.com
 Keywords: pip,nonebot2,nonebot,sky光遇,光遇
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -280,14 +280,18 @@
 
 新浪微博@张张幼稚园 —> *攻略内容*
 
 新浪微博&哔哩哔哩@木易不高兴了啊 —> *攻略内容*
 
 ## ✨更新日志✨
 
+2023.5.30 v2.2.9
+
+这个版本修复了上版本复刻缓存方法调用错误的问题，现在可以智能化识别国服通常复刻周期
+
 2023.5.22 v2.2.8
 
 新增国服通用复刻周期函数，国服复刻已更新，国际服复刻维护中。新增若干随机文案
 
 2023.4.30 v2.2.7
 
 1.在这个版本之后所有querytools命令均废弃不再生效。
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sky Version: 2.2.8 Summary: nonebot2
+Metadata-Version: 2.1 Name: nonebot-plugin-sky Version: 2.2.9 Summary: nonebot2
 plugin sky Home-page: https://github.com/Kaguya233qwq/nonebot_plugin_sky
 Author: Kaguya233qwq Author-email: 1435608435@qq.com Keywords:
 pip,nonebot2,nonebot,skyåé,åé Platform: any Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Natural Language :: Chinese (Simplified)
 Description-Content-Type: text/markdown License-File: LICENSE
                                      [sky]
@@ -106,15 +106,17 @@
 (ç¾¤æä»¶æä¸é®å¯å¨å)
                                      [sky]
 ## â¨æè°¢ååï¼ä¸åååï¼â¨ æ°æµªå¾®å@åéééååå â>
 *æ»ç¥åå®¹* æ°æµªå¾®å@æ§æ¥ä¸æ¥ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@ä»å¤©æ¸¸ç¦»ç¿»è½¦äºå â> *æ»ç¥åå®¹*
 æ°æµªå¾®å@å¼ å¼ å¹¼ç¨å­ â> *æ»ç¥åå®¹*
 æ°æµªå¾®å&åå©åå©@æ¨æä¸é«å´äºå â> *æ»ç¥åå®¹* ##
-â¨æ´æ°æ¥å¿â¨ 2023.5.22 v2.2.8
+â¨æ´æ°æ¥å¿â¨ 2023.5.30 v2.2.9
+è¿ä¸ªçæ¬ä¿®å¤äºä¸çæ¬å¤å»ç¼å­æ¹æ³è°ç¨éè¯¯çé®é¢ï¼ç°å¨å¯ä»¥æºè½åè¯å«å½æéå¸¸å¤å»å¨æ
+2023.5.22 v2.2.8
 æ°å¢å½æéç¨å¤å»å¨æå½æ°ï¼å½æå¤å»å·²æ´æ°ï¼å½éæå¤å»ç»´æ¤ä¸­ãæ°å¢è¥å¹²éæºææ¡
 2023.4.30 v2.2.7
 1.å¨è¿ä¸ªçæ¬ä¹åææquerytoolså½ä»¤ååºå¼ä¸åçæã
 2.æ´æ°å­£èæ¶é´ï¼ææ¶ä¸æ¯å¾åç¡® 2023.4.25 v2.2.6
 1.ä¿®å¤è·åuidå¸®å©å¾çæ æ³åéçé®é¢
 2.å½å¤äºå­£èçç©ºææ¶æ¥è¯¢å­£è¡ãè¡çæ°è¿åç¸åºæç¤º
 2023.4.12 v2.2.5.post2 ä¿®å¤å·²ç¥é®é¢ 2023.4.4 v2.2.5.post1
```

### Comparing `nonebot-plugin-sky-2.2.8/nonebot_plugin_sky.egg-info/SOURCES.txt` & `nonebot-plugin-sky-2.2.9/nonebot_plugin_sky.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,15 @@
 nonebot_plugin_sky/config/load_config.py
 nonebot_plugin_sky/config/msg_forward.py
 nonebot_plugin_sky/config/travelling_cache.py
 nonebot_plugin_sky/guild/__init__.py
 nonebot_plugin_sky/guild/light_beauty.py
 nonebot_plugin_sky/guild/light_cute.py
 nonebot_plugin_sky/sky/__init__.py
-nonebot_plugin_sky/sky/get_id.png
 nonebot_plugin_sky/sky/public_notice.py
-nonebot_plugin_sky/sky/query_tools.py
 nonebot_plugin_sky/sky/queue.py
 nonebot_plugin_sky/sky/daily_tasks/__init__.py
 nonebot_plugin_sky/sky/daily_tasks/international.py
 nonebot_plugin_sky/sky/daily_tasks/national.py
 nonebot_plugin_sky/sky/travelling_spirit/__init__.py
 nonebot_plugin_sky/sky/travelling_spirit/international.py
 nonebot_plugin_sky/sky/travelling_spirit/national.py
```

### Comparing `nonebot-plugin-sky-2.2.8/setup.py` & `nonebot-plugin-sky-2.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 Files = get_files(r'nonebot_plugin_sky/tools/helper_image')
 
 with open("README.md", "r", encoding="utf-8", errors="ignore") as f:
     long_description = f.read()
 setuptools.setup(
     name='nonebot-plugin-sky',
-    version='v2.2.8',
+    version='v2.2.9',
     author='Kaguya233qwq',
     author_email='1435608435@qq.com',
     keywords=["pip", "nonebot2", "nonebot", "sky光遇", "光遇"],
     url='https://github.com/Kaguya233qwq/nonebot_plugin_sky',
     description='''nonebot2 plugin sky''',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

