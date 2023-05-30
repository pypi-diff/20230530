# Comparing `tmp/deebot-client-2.0.0b2.tar.gz` & `tmp/deebot-client-2.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deebot-client-2.0.0b2.tar", last modified: Thu May 25 20:02:24 2023, max compression
+gzip compressed data, was "deebot-client-2.0.0b3.tar", last modified: Tue May 30 16:03:20 2023, max compression
```

## Comparing `deebot-client-2.0.0b2.tar` & `deebot-client-2.0.0b3.tar`

### file list

```diff
@@ -1,96 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:02:24.093160 deebot-client-2.0.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-25 20:02:24.093160 deebot-client-2.0.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:02:24.085160 deebot-client-2.0.0b2/deebot_client/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13640 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:02:24.089160 deebot-client-2.0.0b2/deebot_client/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/advanced_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/battery.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/carpet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/charge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/charge_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/clean_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/clean_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/clean_preference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/continuous_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/fan_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/life_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/map.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/multimap_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/play_sound.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/pos.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/relocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/true_detect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/commands/water_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:02:24.089160 deebot-client-2.0.0b2/deebot_client/events/
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/events/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/events/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/events/event_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/events/map.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/events/water_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/logging_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21238 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/map.py
--rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:02:24.089160 deebot-client-2.0.0b2/deebot_client/messages/
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/messages/battery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/messages/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    11145 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/mqtt_client.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/deebot_client/vacuum_bot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:02:24.085160 deebot-client-2.0.0b2/deebot_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-25 20:02:24.000000 deebot-client-2.0.0b2/deebot_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-25 20:02:24.000000 deebot-client-2.0.0b2/deebot_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 20:02:24.000000 deebot-client-2.0.0b2/deebot_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-25 20:02:24.000000 deebot-client-2.0.0b2/deebot_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 20:02:24.000000 deebot-client-2.0.0b2/deebot_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-25 20:02:24.093160 deebot-client-2.0.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:02:24.081160 deebot-client-2.0.0b2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:02:24.093160 deebot-client-2.0.0b2/tests/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/test_advanced_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/test_battery.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/test_carpet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/test_charge.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/test_charge_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/test_clean_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/test_clean_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/test_clean_preference.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/test_continuous_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/test_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/test_fan_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/test_life_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/test_map.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/test_mulitmap_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/test_true_detect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/commands/test_water_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:02:24.093160 deebot-client-2.0.0b2/tests/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/events/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/events/test_water_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:02:24.093160 deebot-client-2.0.0b2/tests/messages/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/messages/test_battery.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/messages/test_get_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/messages/test_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-25 20:02:18.000000 deebot-client-2.0.0b2/tests/messages/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:03:20.133942 deebot-client-2.0.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-30 16:03:20.133942 deebot-client-2.0.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:03:20.125941 deebot-client-2.0.0b3/deebot_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13794 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:03:20.129942 deebot-client-2.0.0b3/deebot_client/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/commands/advanced_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/commands/battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/commands/carpet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/commands/charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/commands/charge_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/commands/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/commands/clean_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/commands/clean_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/commands/clean_preference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/commands/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/commands/continuous_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/commands/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/commands/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/commands/fan_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/commands/life_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9403 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/commands/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/commands/multimap_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/commands/play_sound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/commands/pos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/commands/relocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/commands/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/commands/true_detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/commands/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/commands/water_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:03:20.129942 deebot-client-2.0.0b3/deebot_client/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     3675 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/events/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/events/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/events/event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/events/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/events/water_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/logging_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21442 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5787 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:03:20.129942 deebot-client-2.0.0b3/deebot_client/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/messages/battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/messages/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11145 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/mqtt_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/deebot_client/vacuum_bot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:03:20.125941 deebot-client-2.0.0b3/deebot_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-30 16:03:20.000000 deebot-client-2.0.0b3/deebot_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-30 16:03:20.000000 deebot-client-2.0.0b3/deebot_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 16:03:20.000000 deebot-client-2.0.0b3/deebot_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-30 16:03:20.000000 deebot-client-2.0.0b3/deebot_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-30 16:03:20.000000 deebot-client-2.0.0b3/deebot_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-30 16:03:20.133942 deebot-client-2.0.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:03:20.121941 deebot-client-2.0.0b3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:03:20.133942 deebot-client-2.0.0b3/tests/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/tests/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/tests/commands/test_advanced_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/tests/commands/test_battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/tests/commands/test_carpet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/tests/commands/test_charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/tests/commands/test_charge_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/tests/commands/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/tests/commands/test_clean_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/tests/commands/test_clean_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/tests/commands/test_clean_preference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/tests/commands/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/tests/commands/test_continuous_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/tests/commands/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/tests/commands/test_fan_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/tests/commands/test_life_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/tests/commands/test_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/tests/commands/test_mulitmap_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/tests/commands/test_true_detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/tests/commands/test_water_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:03:20.133942 deebot-client-2.0.0b3/tests/events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/tests/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/tests/events/test_event_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/tests/events/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/tests/events/test_water_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 16:03:20.133942 deebot-client-2.0.0b3/tests/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/tests/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/tests/messages/test_battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/tests/messages/test_get_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/tests/messages/test_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-05-30 16:03:13.000000 deebot-client-2.0.0b3/tests/messages/test_stats.py
```

### Comparing `deebot-client-2.0.0b2/LICENSE.txt` & `deebot-client-2.0.0b3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/PKG-INFO` & `deebot-client-2.0.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deebot-client
-Version: 2.0.0b2
+Version: 2.0.0b3
 Summary: a library for controlling certain deebot vacuums
 Home-page: https://github.com/DeebotUniverse/client.py
 Author: DeebotUniverse
 Author-email: deebotuniverse@knatschig-as-hell.info
 License: GPL-3.0
 Keywords: home automation vacuum robot deebot ecovacs
 Classifier: Development Status :: 4 - Beta
```

### Comparing `deebot-client-2.0.0b2/README.md` & `deebot-client-2.0.0b3/README.md`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/deebot_client/api_client.py` & `deebot-client-2.0.0b3/deebot_client/api_client.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/deebot_client/authentication.py` & `deebot-client-2.0.0b3/deebot_client/authentication.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Authentication module."""
 import asyncio
 import time
-from collections.abc import Awaitable, Callable, Mapping
+from collections.abc import Callable, Coroutine, Mapping
 from typing import Any
 from urllib.parse import urljoin
 
 from aiohttp import ClientResponseError, hdrs
 
 from .const import REALM
 from .exceptions import ApiError, AuthenticationError, InvalidAuthenticationError
 from .logging_filter import get_logger
 from .models import Configuration, Credentials
-from .util import md5
+from .util import cancel, create_task, md5
 
 _LOGGER = get_logger(__name__)
 
 _CLIENT_KEY = "1520391301804"
 _CLIENT_SECRET = "6c319b2a5cd3e66e39159c2e28f2fce9"
 _AUTH_CLIENT_KEY = "1520391491841"
 _AUTH_CLIENT_SECRET = "77ef58ce3afbe337da74aa8c5ab963a9"
@@ -306,18 +306,19 @@
             config,
             account_id,
             password_hash,
         )
 
         self._lock = asyncio.Lock()
         self._on_credentials_changed: set[
-            Callable[[Credentials], Awaitable[None]]
+            Callable[[Credentials], Coroutine[Any, Any, None]]
         ] = set()
         self._credentials: Credentials | None = None
         self._refresh_handle: asyncio.TimerHandle | None = None
+        self._tasks: set[asyncio.Future[Any]] = set()
 
     async def authenticate(self, force: bool = False) -> Credentials:
         """Authenticate on ecovacs servers."""
         async with self._lock:
             should_login = False
             if self._credentials is None or force:
                 _LOGGER.debug("No cached credentials, performing login")
@@ -328,21 +329,21 @@
 
             if should_login:
                 self._credentials = await self._auth_client.login()
                 self._cancel_refresh_task()
                 self._create_refresh_task()
 
                 for on_changed in self._on_credentials_changed:
-                    await on_changed(self._credentials)
+                    create_task(self._tasks, on_changed(self._credentials))
 
             assert self._credentials is not None
             return self._credentials
 
     def subscribe(
-        self, callback: Callable[[Credentials], Awaitable[None]]
+        self, callback: Callable[[Credentials], Coroutine[Any, Any, None]]
     ) -> Callable[[], None]:
         """Add callback on new credentials and return subscribe callback."""
 
         def unsubscribe() -> None:
             self._on_credentials_changed.remove(callback)
 
         self._on_credentials_changed.add(callback)
@@ -364,14 +365,15 @@
             headers=headers,
             credentials=await self.authenticate(),
         )
 
     async def teardown(self) -> None:
         """Teardown authenticator."""
         self._cancel_refresh_task()
+        await cancel(self._tasks)
 
     def _cancel_refresh_task(self) -> None:
         if self._refresh_handle and not self._refresh_handle.cancelled():
             self._refresh_handle.cancel()
 
     def _create_refresh_task(self) -> None:
         # refresh at 99% of validity
@@ -382,14 +384,14 @@
                 try:
                     await self.authenticate(True)
                 except Exception:  # pylint: disable=broad-except
                     _LOGGER.error(
                         "An exception occurred during refreshing token", exc_info=True
                     )
 
-            asyncio.create_task(async_refresh())
+            create_task(self._tasks, async_refresh())
             self._refresh_handle = None
 
         assert self._credentials is not None
         validity = (self._credentials.expires_at - time.time()) * 0.99
 
         self._refresh_handle = asyncio.get_event_loop().call_later(validity, refresh)
```

### Comparing `deebot-client-2.0.0b2/deebot_client/command.py` & `deebot-client-2.0.0b3/deebot_client/command.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/deebot_client/commands/__init__.py` & `deebot-client-2.0.0b3/deebot_client/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/deebot_client/commands/charge.py` & `deebot-client-2.0.0b3/deebot_client/commands/charge.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Charge commands."""
 from typing import Any
 
-from ..events import StatusEvent
+from ..events import StateEvent
 from ..logging_filter import get_logger
 from ..message import HandlingResult
 from ..models import VacuumState
 from .common import EventBus, ExecuteCommand
 from .const import CODE
 
 _LOGGER = get_logger(__name__)
@@ -23,16 +23,16 @@
     def _handle_body(cls, event_bus: EventBus, body: dict[str, Any]) -> HandlingResult:
         """Handle message->body and notify the correct event subscribers.
 
         :return: A message response
         """
         code = int(body.get(CODE, -1))
         if code == 0:
-            event_bus.notify(StatusEvent(True, VacuumState.RETURNING))
+            event_bus.notify(StateEvent(VacuumState.RETURNING))
             return HandlingResult.success()
 
         if code == 30007:
             # bot is already charging
-            event_bus.notify(StatusEvent(True, VacuumState.DOCKED))
+            event_bus.notify(StateEvent(VacuumState.DOCKED))
             return HandlingResult.success()
 
         return super()._handle_body(event_bus, body)
```

### Comparing `deebot-client-2.0.0b2/deebot_client/commands/charge_state.py` & `deebot-client-2.0.0b3/deebot_client/commands/charge_state.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Charge state commands."""
 from typing import Any
 
-from ..events import StatusEvent
+from ..events import StateEvent
 from ..message import HandlingResult, MessageBodyDataDict
 from ..models import VacuumState
 from .common import EventBus, NoArgsCommand
 from .const import CODE
 
 
 class GetChargeState(NoArgsCommand, MessageBodyDataDict):
@@ -18,15 +18,15 @@
         cls, event_bus: EventBus, data: dict[str, Any]
     ) -> HandlingResult:
         """Handle message->body->data and notify the correct event subscribers.
 
         :return: A message response
         """
         if data.get("isCharging") == 1:
-            event_bus.notify(StatusEvent(True, VacuumState.DOCKED))
+            event_bus.notify(StateEvent(VacuumState.DOCKED))
         return HandlingResult.success()
 
     @classmethod
     def _handle_body(cls, event_bus: EventBus, body: dict[str, Any]) -> HandlingResult:
         if body.get(CODE, 0) == 0:
             # Call this also if code is not in the body
             return super()._handle_body(event_bus, body)
@@ -37,11 +37,11 @@
                 status = VacuumState.DOCKED
             elif body["code"] == "5":  # Busy with another command
                 status = VacuumState.ERROR
             elif body["code"] == "3":  # Bot in stuck state, example dust bin out
                 status = VacuumState.ERROR
 
         if status:
-            event_bus.notify(StatusEvent(True, VacuumState.DOCKED))
+            event_bus.notify(StateEvent(VacuumState.DOCKED))
             return HandlingResult.success()
 
         return HandlingResult.analyse()
```

### Comparing `deebot-client-2.0.0b2/deebot_client/commands/clean.py` & `deebot-client-2.0.0b3/deebot_client/commands/clean.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Clean commands."""
 from enum import Enum, unique
 from typing import Any
 
 from ..authentication import Authenticator
 from ..command import CommandResult
-from ..events import StatusEvent
+from ..events import StateEvent
 from ..logging_filter import get_logger
 from ..message import HandlingResult, MessageBodyDataDict
 from ..models import DeviceInfo, VacuumState
 from .common import EventBus, ExecuteCommand, NoArgsCommand
 
 _LOGGER = get_logger(__name__)
 
@@ -40,24 +40,24 @@
     def __init__(self, action: CleanAction) -> None:
         super().__init__(self.__get_args(action))
 
     async def _execute(
         self, authenticator: Authenticator, device_info: DeviceInfo, event_bus: EventBus
     ) -> CommandResult:
         """Execute command."""
-        status = event_bus.get_last_event(StatusEvent)
-        if status and isinstance(self._args, dict):
+        state = event_bus.get_last_event(StateEvent)
+        if state and isinstance(self._args, dict):
             if (
                 self._args["act"] == CleanAction.RESUME.value
-                and status.state != VacuumState.PAUSED
+                and state.state != VacuumState.PAUSED
             ):
                 self._args = self.__get_args(CleanAction.START)
             elif (
                 self._args["act"] == CleanAction.START.value
-                and status.state == VacuumState.PAUSED
+                and state.state == VacuumState.PAUSED
             ):
                 self._args = self.__get_args(CleanAction.RESUME)
 
         return await super()._execute(authenticator, device_info, event_bus)
 
     @staticmethod
     def __get_args(action: CleanAction) -> dict[str, Any]:
@@ -122,11 +122,11 @@
 
         elif state == "goCharging":
             status = VacuumState.RETURNING
         elif state == "idle":
             status = VacuumState.IDLE
 
         if status:
-            event_bus.notify(StatusEvent(True, status))
+            event_bus.notify(StateEvent(status))
             return HandlingResult.success()
 
         return HandlingResult.analyse()
```

### Comparing `deebot-client-2.0.0b2/deebot_client/commands/clean_count.py` & `deebot-client-2.0.0b3/deebot_client/commands/clean_count.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/deebot_client/commands/clean_logs.py` & `deebot-client-2.0.0b3/deebot_client/commands/clean_logs.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/deebot_client/commands/common.py` & `deebot-client-2.0.0b3/deebot_client/commands/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,63 @@
 """Base commands."""
 from abc import ABC, abstractmethod
 from collections.abc import Mapping
 from typing import Any
 
 from ..command import Command, CommandResult
-from ..events import EnableEvent
+from ..events import AvailabilityEvent, EnableEvent
 from ..events.event_bus import EventBus
 from ..logging_filter import get_logger
 from ..message import HandlingResult, HandlingState, Message, MessageBodyDataDict
 from .const import CODE
 
 _LOGGER = get_logger(__name__)
 
 
 class CommandWithMessageHandling(Command, Message, ABC):
     """Command, which handle response by itself."""
 
+    _is_available_check: bool = False
+
     def _handle_response(
         self, event_bus: EventBus, response: dict[str, Any]
     ) -> CommandResult:
         """Handle response from a command.
 
         :return: A message response
         """
         if response.get("ret") == "ok":
             data = response.get("resp", response)
             result = self.handle(event_bus, data)
             return CommandResult(result.state, result.args)
 
-        _LOGGER.warning('Command "%s" was not successfully: %s', self.name, response)
-        return CommandResult(HandlingState.FAILED)
+        if errno := response.get("errno", None):
+            match errno:
+                case 4200:
+                    # bot offline
+                    _LOGGER.info(
+                        'Vacuum is offline. Could not execute command "%s"', self.name
+                    )
+                    event_bus.notify(AvailabilityEvent(False))
+                    return CommandResult(HandlingState.FAILED)
+                case 500:
+                    if self._is_available_check:
+                        _LOGGER.info(
+                            'No response received for command "%s" during availability-check.',
+                            self.name,
+                        )
+                    else:
+                        _LOGGER.warning(
+                            'No response received for command "%s". This can happen if the vacuum has network issues or does not support the command',
+                            self.name,
+                        )
+                    return CommandResult(HandlingState.FAILED)
+
+        _LOGGER.warning('Command "%s" was not successfully.', self.name)
+        return CommandResult(HandlingState.ANALYSE)
 
 
 class CommandHandlingMqttP2P(CommandWithMessageHandling, ABC):
     """Command which handles also mqtt p2p messages."""
 
     @abstractmethod
     def handle_mqtt_p2p(self, event_bus: EventBus, response: dict[str, Any]) -> None:
```

### Comparing `deebot-client-2.0.0b2/deebot_client/commands/custom.py` & `deebot-client-2.0.0b3/deebot_client/commands/custom.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/deebot_client/commands/error.py` & `deebot-client-2.0.0b3/deebot_client/commands/error.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Error commands."""
 from typing import Any
 
-from ..events import ErrorEvent, StatusEvent
+from ..events import ErrorEvent, StateEvent
 from ..message import HandlingResult, MessageBodyDataDict
 from ..models import VacuumState
 from .common import EventBus, NoArgsCommand
 
 
 class GetError(NoArgsCommand, MessageBodyDataDict):
     """Get error command."""
@@ -24,15 +24,15 @@
         if codes:
             # the last error code
             error = codes[-1]
 
             if error is not None:
                 description = _ERROR_CODES.get(error)
                 if error != 0:
-                    event_bus.notify(StatusEvent(True, VacuumState.ERROR))
+                    event_bus.notify(StateEvent(VacuumState.ERROR))
                 event_bus.notify(ErrorEvent(error, description))
                 return HandlingResult.success()
 
         return HandlingResult.analyse()
 
 
 # from https://github.com/mrbungle64/ecovacs-deebot.js/blob/master/library/errorCodes.js
```

### Comparing `deebot-client-2.0.0b2/deebot_client/commands/fan_speed.py` & `deebot-client-2.0.0b3/deebot_client/commands/fan_speed.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/deebot_client/commands/life_span.py` & `deebot-client-2.0.0b3/deebot_client/commands/life_span.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/deebot_client/commands/map.py` & `deebot-client-2.0.0b3/deebot_client/commands/map.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/deebot_client/commands/pos.py` & `deebot-client-2.0.0b3/deebot_client/commands/pos.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/deebot_client/commands/stats.py` & `deebot-client-2.0.0b3/deebot_client/commands/stats.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/deebot_client/commands/volume.py` & `deebot-client-2.0.0b3/deebot_client/commands/volume.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/deebot_client/commands/water_info.py` & `deebot-client-2.0.0b3/deebot_client/commands/water_info.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/deebot_client/events/__init__.py` & `deebot-client-2.0.0b3/deebot_client/events/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,19 +137,25 @@
 
     area: int
     time: int
     cleanings: int
 
 
 @dataclass(frozen=True)
-class StatusEvent(Event):
-    """Status event representation."""
+class AvailabilityEvent(Event):
+    """Availability event."""
 
     available: bool
-    state: VacuumState | None
+
+
+@dataclass(frozen=True)
+class StateEvent(Event):
+    """State event representation."""
+
+    state: VacuumState
 
 
 @dataclass(frozen=True)
 class VolumeEvent(Event):
     """Volume event."""
 
     volume: int
```

### Comparing `deebot-client-2.0.0b2/deebot_client/events/const.py` & `deebot-client-2.0.0b3/deebot_client/events/const.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     GetTotalStats,
     GetTrueDetect,
     GetVolume,
     GetWaterInfo,
 )
 from . import (
     AdvancedModeEvent,
+    AvailabilityEvent,
     BatteryEvent,
     CarpetAutoFanBoostEvent,
     CleanCountEvent,
     CleanLogEvent,
     CleanPreferenceEvent,
     ContinuousCleaningEvent,
     CustomCommandEvent,
@@ -39,16 +40,16 @@
     Event,
     FanSpeedEvent,
     LifeSpanEvent,
     MultimapStateEvent,
     PositionsEvent,
     ReportStatsEvent,
     RoomsEvent,
+    StateEvent,
     StatsEvent,
-    StatusEvent,
     TotalStatsEvent,
     TrueDetectEvent,
     VolumeEvent,
     WaterInfoEvent,
 )
 from .map import (
     CachedMapInfoEvent,
@@ -56,14 +57,15 @@
     MapSetEvent,
     MapSubsetEvent,
     MapTraceEvent,
     MinorMapEvent,
 )
 
 EVENT_DTO_REFRESH_COMMANDS: Mapping[type[Event], list[Command]] = {
+    AvailabilityEvent: [],
     AdvancedModeEvent: [GetAdvancedMode()],
     BatteryEvent: [GetBattery()],
     CachedMapInfoEvent: [GetCachedMapInfo()],
     CarpetAutoFanBoostEvent: [GetCarpetAutoFanBoost()],
     CleanLogEvent: [GetCleanLogs()],
     CleanCountEvent: [GetCleanCount()],
     CleanPreferenceEvent: [GetCleanPreference()],
@@ -78,13 +80,13 @@
     MapTraceEvent: [GetMapTrace()],
     MinorMapEvent: [],
     MultimapStateEvent: [GetMultimapState()],
     PositionsEvent: [GetPos()],
     ReportStatsEvent: [],  # ReportStats cannot be pulled
     RoomsEvent: [GetCachedMapInfo()],
     StatsEvent: [GetStats()],
-    StatusEvent: [GetChargeState(), GetCleanInfo()],
+    StateEvent: [GetChargeState(), GetCleanInfo()],
     TotalStatsEvent: [GetTotalStats()],
     TrueDetectEvent: [GetTrueDetect()],
     VolumeEvent: [GetVolume()],
     WaterInfoEvent: [GetWaterInfo()],
 }
```

### Comparing `deebot-client-2.0.0b2/deebot_client/events/event_bus.py` & `deebot-client-2.0.0b3/deebot_client/events/event_bus.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import asyncio
 import threading
 from collections.abc import Callable, Coroutine
 from typing import TYPE_CHECKING, Any, Final, Generic, TypeVar
 
 from ..logging_filter import get_logger
 from ..models import VacuumState
-from . import Event, StatusEvent
+from ..util import cancel, create_task
+from . import AvailabilityEvent, Event, StateEvent
 
 if TYPE_CHECKING:
     from ..command import Command
 
 _LOGGER = get_logger(__name__)
 
 T = TypeVar("T", bound=Event)
@@ -58,14 +59,16 @@
 
     def __init__(
         self,
         execute_command: Callable[["Command"], Coroutine[Any, Any, None]],
     ):
         self._event_processing_dict: dict[type[Event], _EventProcessingData] = {}
         self._lock = threading.Lock()
+        self._tasks: set[asyncio.Future[Any]] = set()
+
         self._execute_command: Final = execute_command
 
     def has_subscribers(self, event: type[T]) -> bool:
         """Return True, if emitter has subscribers."""
         return (
             len(self._event_processing_dict[event].subscribers) > 0
             if event in self._event_processing_dict
@@ -81,54 +84,69 @@
         event_processing_data = self._get_or_create_event_processing_data(event_type)
 
         listener = EventListener(event_processing_data, callback)
         event_processing_data.subscribers.append(listener)
 
         if event_processing_data.last_event:
             # Notify subscriber directly with the last event
-            asyncio.create_task(listener.callback(event_processing_data.last_event))
+            create_task(
+                self._tasks, listener.callback(event_processing_data.last_event)
+            )
         elif len(event_processing_data.subscribers) == 1:
             # first subscriber therefore do refresh
             self.request_refresh(event_type)
 
         return listener
 
     def notify(self, event: T) -> bool:
         """Notify subscriber with given event representation."""
         event_processing_data = self._get_or_create_event_processing_data(type(event))
 
         if (
-            isinstance(event, StatusEvent)
+            isinstance(event, StateEvent)
             and event.state == VacuumState.IDLE
             and event_processing_data.last_event
-            and event_processing_data.last_event.available == event.available  # type: ignore[attr-defined]
             and event_processing_data.last_event.state == VacuumState.DOCKED  # type: ignore[attr-defined]
         ):
             # todo distinguish better between docked and idle and outside event bus. # pylint: disable=fixme
             # Problem getCleanInfo will return state=idle, when bot is charging
-            event = StatusEvent(event.available, VacuumState.DOCKED)  # type: ignore[assignment]
+            event = StateEvent(VacuumState.DOCKED)  # type: ignore[assignment]
+        elif (
+            isinstance(event, AvailabilityEvent)
+            and event.available
+            and event_processing_data.last_event
+            and not event_processing_data.last_event.available  # type: ignore[attr-defined]
+        ):
+            # unavailable -> available: refresh everything
+            for event_type, _ in self._event_processing_dict.items():
+                if event_type != AvailabilityEvent:
+                    self.request_refresh(event_type)
 
         if event == event_processing_data.last_event:
             _LOGGER.debug("Event is the same! Skipping (%s)", event)
             return False
 
         event_processing_data.last_event = event
         if event_processing_data.subscribers:
             _LOGGER.debug("Notify subscribers with %s", event)
             for subscriber in event_processing_data.subscribers:
-                asyncio.create_task(subscriber.callback(event))
+                create_task(self._tasks, subscriber.callback(event))
             return True
 
         _LOGGER.debug("No subscribers... Discharging %s", event)
         return False
 
     def request_refresh(self, event_class: type[T]) -> None:
         """Request manual refresh."""
         if self.has_subscribers(event_class):
-            asyncio.create_task(self._call_refresh_function(event_class))
+            create_task(self._tasks, self._call_refresh_function(event_class))
+
+    async def teardown(self) -> None:
+        """Teardown eventbus."""
+        await cancel(self._tasks)
 
     async def _call_refresh_function(self, event_class: type[T]) -> None:
         semaphore = self._event_processing_dict[event_class].semaphore
         if semaphore.locked():
             _LOGGER.debug("Already refresh function running. Skipping...")
             return
```

### Comparing `deebot-client-2.0.0b2/deebot_client/events/map.py` & `deebot-client-2.0.0b3/deebot_client/events/map.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/deebot_client/logging_filter.py` & `deebot-client-2.0.0b3/deebot_client/logging_filter.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/deebot_client/map.py` & `deebot-client-2.0.0b3/deebot_client/map.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     PositionType,
     RoomsEvent,
 )
 from .events.event_bus import EventBus, EventListener
 from .exceptions import MapError
 from .logging_filter import get_logger
 from .models import Room
-from .util import OnChangedDict, OnChangedList
+from .util import OnChangedDict, OnChangedList, cancel, create_task
 
 _LOGGER = get_logger(__name__)
 _PIXEL_WIDTH = 50
 _POSITION_PNG = {
     PositionType.DEEBOT: "iVBORw0KGgoAAAANSUhEUgAAAAYAAAAGCAIAAABvrngfAAAACXBIWXMAAAsTAAALEwEAmpwYAAAF0WlUWHRYTUw6Y29tLmFkb2JlLnhtcAAAAAAAPD94cGFja2V0IGJlZ2luPSLvu78iIGlkPSJXNU0wTXBDZWhpSHpyZVN6TlRjemtjOWQiPz4gPHg6eG1wbWV0YSB4bWxuczp4PSJhZG9iZTpuczptZXRhLyIgeDp4bXB0az0iQWRvYmUgWE1QIENvcmUgNS42LWMxNDUgNzkuMTYzNDk5LCAyMDE4LzA4LzEzLTE2OjQwOjIyICAgICAgICAiPiA8cmRmOlJERiB4bWxuczpyZGY9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkvMDIvMjItcmRmLXN5bnRheC1ucyMiPiA8cmRmOkRlc2NyaXB0aW9uIHJkZjphYm91dD0iIiB4bWxuczp4bXA9Imh0dHA6Ly9ucy5hZG9iZS5jb20veGFwLzEuMC8iIHhtbG5zOnhtcE1NPSJodHRwOi8vbnMuYWRvYmUuY29tL3hhcC8xLjAvbW0vIiB4bWxuczpzdEV2dD0iaHR0cDovL25zLmFkb2JlLmNvbS94YXAvMS4wL3NUeXBlL1Jlc291cmNlRXZlbnQjIiB4bWxuczpkYz0iaHR0cDovL3B1cmwub3JnL2RjL2VsZW1lbnRzLzEuMS8iIHhtbG5zOnBob3Rvc2hvcD0iaHR0cDovL25zLmFkb2JlLmNvbS9waG90b3Nob3AvMS4wLyIgeG1wOkNyZWF0b3JUb29sPSJBZG9iZSBQaG90b3Nob3AgQ0MgMjAxOSAoV2luZG93cykiIHhtcDpDcmVhdGVEYXRlPSIyMDIwLTA1LTI0VDEyOjAzOjE2KzAyOjAwIiB4bXA6TWV0YWRhdGFEYXRlPSIyMDIwLTA1LTI0VDEyOjAzOjE2KzAyOjAwIiB4bXA6TW9kaWZ5RGF0ZT0iMjAyMC0wNS0yNFQxMjowMzoxNiswMjowMCIgeG1wTU06SW5zdGFuY2VJRD0ieG1wLmlpZDo0YWM4NWY5MC1hNWMwLTE2NDktYTQ0MC0xMWM0NWY5OGQ1MDYiIHhtcE1NOkRvY3VtZW50SUQ9ImFkb2JlOmRvY2lkOnBob3Rvc2hvcDo3Zjk3MTZjMi1kZDM1LWJiNDItYjMzZS1hYjYwY2Y4ZTZlZDYiIHhtcE1NOk9yaWdpbmFsRG9jdW1lbnRJRD0ieG1wLmRpZDpiMzhiNGZlMS1lOGNkLTJjNDctYmQwZC1lNmZiNzRhMjFkMDciIGRjOmZvcm1hdD0iaW1hZ2UvcG5nIiBwaG90b3Nob3A6Q29sb3JNb2RlPSIzIj4gPHhtcE1NOkhpc3Rvcnk+IDxyZGY6U2VxPiA8cmRmOmxpIHN0RXZ0OmFjdGlvbj0iY3JlYXRlZCIgc3RFdnQ6aW5zdGFuY2VJRD0ieG1wLmlpZDpiMzhiNGZlMS1lOGNkLTJjNDctYmQwZC1lNmZiNzRhMjFkMDciIHN0RXZ0OndoZW49IjIwMjAtMDUtMjRUMTI6MDM6MTYrMDI6MDAiIHN0RXZ0OnNvZnR3YXJlQWdlbnQ9IkFkb2JlIFBob3Rvc2hvcCBDQyAyMDE5IChXaW5kb3dzKSIvPiA8cmRmOmxpIHN0RXZ0OmFjdGlvbj0ic2F2ZWQiIHN0RXZ0Omluc3RhbmNlSUQ9InhtcC5paWQ6NGFjODVmOTAtYTVjMC0xNjQ5LWE0NDAtMTFjNDVmOThkNTA2IiBzdEV2dDp3aGVuPSIyMDIwLTA1LTI0VDEyOjAzOjE2KzAyOjAwIiBzdEV2dDpzb2Z0d2FyZUFnZW50PSJBZG9iZSBQaG90b3Nob3AgQ0MgMjAxOSAoV2luZG93cykiIHN0RXZ0OmNoYW5nZWQ9Ii8iLz4gPC9yZGY6U2VxPiA8L3htcE1NOkhpc3Rvcnk+IDwvcmRmOkRlc2NyaXB0aW9uPiA8L3JkZjpSREY+IDwveDp4bXBtZXRhPiA8P3hwYWNrZXQgZW5kPSJyIj8+AP7+NwAAAFpJREFUCJllzEEKgzAQhtFvMkSsEKj30oUXrYserELA1obhd+nCd4BnksZ53X4Cnr193ov59Iq+o2SA2vz4p/iKkgkRouTYlbhJ/jBqww03avPBTNI4rdtx9ScfWyYCg52e0gAAAABJRU5ErkJggg==",  # nopep8
     PositionType.CHARGER: "iVBORw0KGgoAAAANSUhEUgAAAAoAAAAOCAYAAAAWo42rAAAAdUlEQVQoU2NkQAP/nzD8BwkxyjAwIkuhcEASRCmEKYKZhGwq3ER0ReiKSVOIyzRkU8EmwhUyKzAwSNyHyL9QZGD4+wDMBLmVEasimFHIiuEKpcHBhwmeQryBMJFohcjuw2s1SBKHZ8BWo/gauyshvobJEYoZAEOSPXnhzwZnAAAAAElFTkSuQmCC",  # nopep8
 }
@@ -140,14 +140,15 @@
         self._execute_command = execute_command
         self._event_bus = event_bus
 
         self._map_data: Final[MapData] = MapData()
         self._amount_rooms: int = 0
         self._last_image: LastImage | None = None
         self._listeners: list[EventListener] = []
+        self._tasks: set[asyncio.Future[Any]] = set()
 
         async def on_map_set(event: MapSetEvent) -> None:
             if event.type == MapSetType.ROOMS:
                 self._amount_rooms = len(event.subsets)
                 for room_id, _ in self._map_data.rooms.copy().items():
                     if room_id not in event.subsets:
                         self._map_data.rooms.pop(room_id, None)
@@ -225,15 +226,15 @@
                             draw.point((point_x, point_y), fill=_COLORS[pixel_type])
 
     def enable(self) -> None:
         """Enable map."""
         if self._listeners:
             return
 
-        asyncio.create_task(self._execute_command(GetCachedMapInfo()))
+        create_task(self._tasks, self._execute_command(GetCachedMapInfo()))
 
         async def on_position(event: PositionsEvent) -> None:
             self._map_data.positions = event.positions
 
         self._listeners.append(self._event_bus.subscribe(PositionsEvent, on_position))
 
         async def on_map_trace(event: MapTraceEvent) -> None:
@@ -363,14 +364,19 @@
         base64_image = base64.b64encode(buffered.getvalue())
         self._map_data.reset_changed()
         self._last_image = LastImage(base64_image, width)
         _LOGGER.debug("[get_base64_map] Finish")
 
         return base64_image
 
+    async def teardown(self) -> None:
+        """Teardown map."""
+        self.disable()
+        await cancel(self._tasks)
+
 
 class MapPiece:
     """Map piece representation."""
 
     _NOT_INUSE_CRC32: int = 1295764014
 
     def __init__(self, on_change: Callable[[], None], index: int) -> None:
```

### Comparing `deebot-client-2.0.0b2/deebot_client/message.py` & `deebot-client-2.0.0b3/deebot_client/message.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/deebot_client/messages/__init__.py` & `deebot-client-2.0.0b3/deebot_client/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/deebot_client/messages/battery.py` & `deebot-client-2.0.0b3/deebot_client/messages/battery.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/deebot_client/messages/stats.py` & `deebot-client-2.0.0b3/deebot_client/messages/stats.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/deebot_client/models.py` & `deebot-client-2.0.0b3/deebot_client/models.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/deebot_client/mqtt_client.py` & `deebot-client-2.0.0b3/deebot_client/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/deebot_client/util.py` & `deebot-client-2.0.0b3/deebot_client/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,50 @@
 """Util module."""
 from __future__ import annotations
 
+import asyncio
 import hashlib
-from collections.abc import Callable, Iterable, Mapping
+from collections.abc import Callable, Coroutine, Iterable, Mapping
+from contextlib import suppress
 from enum import IntEnum, unique
-from typing import TYPE_CHECKING, SupportsIndex, TypeVar, overload
+from typing import TYPE_CHECKING, Any, SupportsIndex, TypeVar, overload
 
 if TYPE_CHECKING:
     from _typeshed import SupportsKeysAndGetItem
 
+_T = TypeVar("_T")
+_S = TypeVar("_S")
+
 
 def md5(text: str) -> str:
     """Hash text using md5."""
     return hashlib.md5(bytes(str(text), "utf8")).hexdigest()
 
 
+def create_task(
+    tasks: set[asyncio.Future[Any]], target: Coroutine[Any, Any, _T]
+) -> asyncio.Task[_T]:
+    """Create task with done callback to remove it from tasks and add it to tasks."""
+    task = asyncio.create_task(target)
+    tasks.add(task)
+    task.add_done_callback(tasks.remove)
+    return task
+
+
+async def cancel(tasks: set[asyncio.Future[Any]]) -> None:
+    """Cancel all tasks and wait for their completion."""
+    tasks_to_wait = set()
+    for task in tasks:
+        if task.cancel():
+            tasks_to_wait.add(task)
+
+    with suppress(asyncio.CancelledError):
+        await asyncio.gather(*tasks_to_wait)
+
+
 @unique
 class DisplayNameIntEnum(IntEnum):
     """Int enum with a property "display_name"."""
 
     def __new__(cls, *args: int, **_: Mapping) -> DisplayNameIntEnum:
         """Create new DisplayNameIntEnum."""
         obj = int.__new__(cls)
@@ -59,18 +85,14 @@
     def __ne__(self, x: object) -> bool:
         return not self.__eq__(x)
 
     def __hash__(self) -> int:
         return hash(self._value_)
 
 
-_T = TypeVar("_T")
-_S = TypeVar("_S")
-
-
 class OnChangedList(list[_T]):
     """List, which will call passed on_change if a change happens."""
 
     def __init__(self, on_change: Callable[[], None], iterable: Iterable[_T] = ()):
         super().__init__(iterable)
         self._on_change = on_change
```

### Comparing `deebot-client-2.0.0b2/deebot_client/vacuum_bot.py` & `deebot-client-2.0.0b3/deebot_client/vacuum_bot.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """Vacuum bot module."""
 import asyncio
-import inspect
 import json
 from collections.abc import Callable
 from contextlib import suppress
 from datetime import datetime
 from typing import Any, Final
 
 from deebot_client.commands.battery import GetBattery
 from deebot_client.mqtt_client import MqttClient, SubscriberInfo
 
 from .authentication import Authenticator
 from .command import Command
 from .events import (
+    AvailabilityEvent,
     CleanLogEvent,
     CustomCommandEvent,
     LifeSpanEvent,
     PositionsEvent,
     PositionType,
+    StateEvent,
     StatsEvent,
-    StatusEvent,
     TotalStatsEvent,
 )
 from .events.event_bus import EventBus
 from .logging_filter import get_logger
 from .map import Map
 from .messages import get_message
 from .models import DeviceInfo, VacuumState
@@ -40,58 +40,49 @@
         device_info: DeviceInfo,
         authenticator: Authenticator,
     ):
         self.device_info: Final[DeviceInfo] = device_info
         self._authenticator = authenticator
 
         self._semaphore = asyncio.Semaphore(3)
-        self._status: StatusEvent = StatusEvent(device_info.status == 1, None)
+        self._state: StateEvent | None = None
         self._last_time_available: datetime = datetime.now()
         self._available_task: asyncio.Task | None = None
         self._unsubscribe: Callable[[], None] | None = None
 
         self.fw_version: str | None = None
         self.events: Final[EventBus] = EventBus(self.execute_command)
 
         self.map: Final[Map] = Map(self.execute_command, self.events)
 
         async def on_pos(event: PositionsEvent) -> None:
-            if self._status == StatusEvent(True, VacuumState.DOCKED):
+            if self._state == StateEvent(VacuumState.DOCKED):
                 return
 
             deebot = next(p for p in event.positions if p.type == PositionType.DEEBOT)
 
             if deebot:
                 on_charger = filter(
                     lambda p: p.type == PositionType.CHARGER
                     and p.x == deebot.x
                     and p.y == deebot.y,
                     event.positions,
                 )
                 if on_charger:
                     # deebot on charger so the status should be docked... Checking
-                    self.events.request_refresh(StatusEvent)
+                    self.events.request_refresh(StateEvent)
 
         self.events.subscribe(PositionsEvent, on_pos)
 
-        async def on_status(event: StatusEvent) -> None:
-            last_status = self._status
-            self._status = event
-            if (not last_status.available) and event.available:
-                # bot was unavailable
-                for name, obj in inspect.getmembers(
-                    self.events, lambda obj: isinstance(obj, EventBus)
-                ):
-                    if name != "status":
-                        obj.request_refresh()
-            elif event.state == VacuumState.DOCKED:
+        async def on_state(event: StateEvent) -> None:
+            if event.state == VacuumState.DOCKED:
                 self.events.request_refresh(CleanLogEvent)
                 self.events.request_refresh(TotalStatsEvent)
 
-        self.events.subscribe(StatusEvent, on_status)
+        self.events.subscribe(StateEvent, on_state)
 
         async def on_stats(_: StatsEvent) -> None:
             self.events.request_refresh(LifeSpanEvent)
 
         self.events.subscribe(StatsEvent, on_stats)
 
         async def on_custom_command(event: CustomCommandEvent) -> None:
@@ -119,22 +110,25 @@
             self._unsubscribe()
             self._unsubscribe = None
 
         if self._available_task and self._available_task.cancel():
             with suppress(asyncio.CancelledError):
                 await self._available_task
 
+        await self.events.teardown()
+        await self.map.teardown()
+
     async def _available_task_worker(self) -> None:
         while True:
             if (datetime.now() - self._last_time_available).total_seconds() > (
                 _AVAILABLE_CHECK_INTERVAL - 1
             ):
                 # request GetBattery to check availability
                 try:
-                    self._set_available(await self._execute_command(GetBattery()))
+                    self._set_available(await self._execute_command(GetBattery(True)))
                 except Exception:  # pylint: disable=broad-exception-caught
                     _LOGGER.debug(
                         "An exception occurred during the available check",
                         exc_info=True,
                     )
             await asyncio.sleep(_AVAILABLE_CHECK_INTERVAL)
 
@@ -150,16 +144,15 @@
         return False
 
     def _set_available(self, available: bool) -> None:
         """Set available."""
         if available:
             self._last_time_available = datetime.now()
 
-        status = StatusEvent(available, self._status.state)
-        self.events.notify(status)
+        self.events.notify(AvailabilityEvent(available))
 
     def _handle_message(
         self, message_name: str, message_data: str | bytes | bytearray | dict[str, Any]
     ) -> None:
         """Handle the given message.
 
         :param message_name: message name
```

### Comparing `deebot-client-2.0.0b2/deebot_client.egg-info/PKG-INFO` & `deebot-client-2.0.0b3/deebot_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deebot-client
-Version: 2.0.0b2
+Version: 2.0.0b3
 Summary: a library for controlling certain deebot vacuums
 Home-page: https://github.com/DeebotUniverse/client.py
 Author: DeebotUniverse
 Author-email: deebotuniverse@knatschig-as-hell.info
 License: GPL-3.0
 Keywords: home automation vacuum robot deebot ecovacs
 Classifier: Development Status :: 4 - Beta
```

### Comparing `deebot-client-2.0.0b2/deebot_client.egg-info/SOURCES.txt` & `deebot-client-2.0.0b3/deebot_client.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -63,23 +63,25 @@
 tests/commands/test_carpet.py
 tests/commands/test_charge.py
 tests/commands/test_charge_state.py
 tests/commands/test_clean.py
 tests/commands/test_clean_count.py
 tests/commands/test_clean_log.py
 tests/commands/test_clean_preference.py
+tests/commands/test_common.py
 tests/commands/test_continuous_cleaning.py
 tests/commands/test_custom.py
 tests/commands/test_fan_speed.py
 tests/commands/test_life_span.py
 tests/commands/test_map.py
 tests/commands/test_mulitmap_state.py
 tests/commands/test_true_detect.py
 tests/commands/test_water_info.py
 tests/events/__init__.py
+tests/events/test_event_bus.py
 tests/events/test_events.py
 tests/events/test_water_info.py
 tests/messages/__init__.py
 tests/messages/test_battery.py
 tests/messages/test_get_messages.py
 tests/messages/test_messages.py
 tests/messages/test_stats.py
```

### Comparing `deebot-client-2.0.0b2/setup.py` & `deebot-client-2.0.0b3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = file.read()
 
 with open("requirements.txt", encoding="utf-8") as file:
     install_requires = list(val.strip() for val in file)
 
 setup(
     name="deebot-client",
-    version="2.0.0b2",
+    version="2.0.0b3",
     url="https://github.com/DeebotUniverse/client.py",
     description="a library for controlling certain deebot vacuums",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="DeebotUniverse",
     author_email="deebotuniverse@knatschig-as-hell.info",
     license="GPL-3.0",
```

### Comparing `deebot-client-2.0.0b2/tests/commands/__init__.py` & `deebot-client-2.0.0b3/tests/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/tests/commands/test_advanced_mode.py` & `deebot-client-2.0.0b3/tests/commands/test_advanced_mode.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/tests/commands/test_carpet.py` & `deebot-client-2.0.0b3/tests/commands/test_carpet.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/tests/commands/test_charge.py` & `deebot-client-2.0.0b3/tests/commands/test_charge.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any
 
 import pytest
 from testfixtures import LogCapture
 
 from deebot_client.commands import Charge
-from deebot_client.events import StatusEvent
+from deebot_client.events import StateEvent
 from deebot_client.models import VacuumState
 from tests.commands import assert_command
 from tests.helpers import get_request_json
 
 
 def _prepare_json(code: int, msg: str = "ok") -> dict[str, Any]:
     json = get_request_json(None)
@@ -20,19 +20,19 @@
     )
     return json
 
 
 @pytest.mark.parametrize(
     "json, expected",
     [
-        (get_request_json(None), StatusEvent(True, VacuumState.RETURNING)),
-        (_prepare_json(30007), StatusEvent(True, VacuumState.DOCKED)),
+        (get_request_json(None), StateEvent(VacuumState.RETURNING)),
+        (_prepare_json(30007), StateEvent(VacuumState.DOCKED)),
     ],
 )
-async def test_Charge(json: dict[str, Any], expected: StatusEvent) -> None:
+async def test_Charge(json: dict[str, Any], expected: StateEvent) -> None:
     await assert_command(Charge(), json, expected)
 
 
 async def test_Charge_failed() -> None:
     with LogCapture() as log:
         json = _prepare_json(500, "fail")
         await assert_command(Charge(), json, None)
```

### Comparing `deebot-client-2.0.0b2/tests/commands/test_clean.py` & `deebot-client-2.0.0b3/tests/commands/test_clean_count.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,17 @@
-from typing import Any
-
 import pytest
 
-from deebot_client.commands import GetCleanInfo
-from deebot_client.events import StatusEvent
-from deebot_client.models import VacuumState
-from tests.commands import assert_command
+from deebot_client.commands import GetCleanCount, SetCleanCount
+from deebot_client.events import CleanCountEvent
+from tests.commands import assert_command, assert_set_command
 from tests.helpers import get_request_json
 
 
-@pytest.mark.parametrize(
-    "json, expected",
-    [
-        (
-            get_request_json({"trigger": "none", "state": "idle"}),
-            StatusEvent(True, VacuumState.IDLE),
-        ),
-    ],
-)
-async def test_GetCleanInfo(json: dict[str, Any], expected: StatusEvent) -> None:
-    await assert_command(GetCleanInfo(), json, expected)
+async def test_GetCleanCount() -> None:
+    json = get_request_json({"count": 2})
+    await assert_command(GetCleanCount(), json, CleanCountEvent(2))
+
+
+@pytest.mark.parametrize("count", [1, 2, 3])
+async def test_SetCleanCount(count: int) -> None:
+    args = {"count": count}
+    await assert_set_command(SetCleanCount(count), args, CleanCountEvent(count))
```

### Comparing `deebot-client-2.0.0b2/tests/commands/test_clean_log.py` & `deebot-client-2.0.0b3/tests/commands/test_clean_log.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/tests/commands/test_clean_preference.py` & `deebot-client-2.0.0b3/tests/commands/test_clean_preference.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/tests/commands/test_continuous_cleaning.py` & `deebot-client-2.0.0b3/tests/commands/test_continuous_cleaning.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/tests/commands/test_custom.py` & `deebot-client-2.0.0b3/tests/commands/test_custom.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/tests/commands/test_fan_speed.py` & `deebot-client-2.0.0b3/tests/commands/test_fan_speed.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/tests/commands/test_life_span.py` & `deebot-client-2.0.0b3/tests/commands/test_life_span.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/tests/commands/test_map.py` & `deebot-client-2.0.0b3/tests/commands/test_map.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/tests/commands/test_mulitmap_state.py` & `deebot-client-2.0.0b3/tests/commands/test_mulitmap_state.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/tests/commands/test_true_detect.py` & `deebot-client-2.0.0b3/tests/commands/test_true_detect.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/tests/commands/test_water_info.py` & `deebot-client-2.0.0b3/tests/commands/test_water_info.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/tests/messages/test_battery.py` & `deebot-client-2.0.0b3/tests/messages/test_battery.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/tests/messages/test_get_messages.py` & `deebot-client-2.0.0b3/tests/messages/test_get_messages.py`

 * *Files identical despite different names*

### Comparing `deebot-client-2.0.0b2/tests/messages/test_stats.py` & `deebot-client-2.0.0b3/tests/messages/test_stats.py`

 * *Files identical despite different names*

