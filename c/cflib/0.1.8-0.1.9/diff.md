# Comparing `tmp/cflib-0.1.8.tar.gz` & `tmp/cflib-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cflib-0.1.8.tar", last modified: Thu Sep 26 14:31:59 2019, max compression
+gzip compressed data, was "dist/cflib-0.1.9.tar", last modified: Thu Feb  6 11:50:17 2020, max compression
```

## Comparing `cflib-0.1.8.tar` & `cflib-0.1.9.tar`

### file list

```diff
@@ -1,89 +1,88 @@
-drwxr-xr-x   0 arnaud    (1000) arnaud    (1000)        0 2019-09-26 14:31:59.000000 cflib-0.1.8/
--rw-r--r--   0 arnaud    (1000) arnaud    (1000)      784 2019-09-26 14:28:21.000000 cflib-0.1.8/setup.py
--rw-r--r--   0 arnaud    (1000) arnaud    (1000)      578 2019-09-26 14:31:59.000000 cflib-0.1.8/PKG-INFO
-drwxr-xr-x   0 arnaud    (1000) arnaud    (1000)        0 2019-09-26 14:31:59.000000 cflib-0.1.8/test/
-drwxr-xr-x   0 arnaud    (1000) arnaud    (1000)        0 2019-09-26 14:31:59.000000 cflib-0.1.8/test/crazyflie/
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)     6595 2018-01-17 13:55:46.000000 cflib-0.1.8/test/crazyflie/test_syncLogger.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)     6269 2018-01-17 13:55:46.000000 cflib-0.1.8/test/crazyflie/test_swarm.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)        0 2018-01-17 13:55:46.000000 cflib-0.1.8/test/crazyflie/__init__.py
--rw-r--r--   0 arnaud    (1000) arnaud    (1000)     4496 2019-06-18 14:37:53.000000 cflib-0.1.8/test/crazyflie/test_syncCrazyflie.py
-drwxr-xr-x   0 arnaud    (1000) arnaud    (1000)        0 2019-09-26 14:31:59.000000 cflib-0.1.8/test/positioning/
--rw-r--r--   0 arnaud    (1000) arnaud    (1000)    11409 2019-09-26 14:28:21.000000 cflib-0.1.8/test/positioning/test_position_hl_commander.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)        0 2018-01-17 13:55:46.000000 cflib-0.1.8/test/positioning/__init__.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)    14623 2018-01-17 13:55:46.000000 cflib-0.1.8/test/positioning/test_motion_commander.py
-drwxr-xr-x   0 arnaud    (1000) arnaud    (1000)        0 2019-09-26 14:31:59.000000 cflib-0.1.8/test/utils/
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)     2734 2018-01-17 13:55:46.000000 cflib-0.1.8/test/utils/test_callbacks.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)     9196 2018-03-22 13:11:25.000000 cflib-0.1.8/test/utils/test_multiranger.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)        0 2018-01-17 13:55:46.000000 cflib-0.1.8/test/utils/__init__.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)        0 2018-01-17 13:55:46.000000 cflib-0.1.8/test/__init__.py
-drwxr-xr-x   0 arnaud    (1000) arnaud    (1000)        0 2019-09-26 14:31:59.000000 cflib-0.1.8/test/support/
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)     1593 2018-01-17 13:55:46.000000 cflib-0.1.8/test/support/asyncCallbackCaller.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)        0 2018-01-17 13:55:46.000000 cflib-0.1.8/test/support/__init__.py
-drwxr-xr-x   0 arnaud    (1000) arnaud    (1000)        0 2019-09-26 14:31:59.000000 cflib-0.1.8/test/crtp/
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)        0 2018-01-17 13:55:46.000000 cflib-0.1.8/test/crtp/__init__.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)     2875 2018-01-17 13:55:46.000000 cflib-0.1.8/test/crtp/test_crtpstack.py
--rw-r--r--   0 arnaud    (1000) arnaud    (1000)     4599 2019-04-23 11:31:29.000000 cflib-0.1.8/README.md
-drwxr-xr-x   0 arnaud    (1000) arnaud    (1000)        0 2019-09-26 14:31:59.000000 cflib-0.1.8/sys_test/
-drwxr-xr-x   0 arnaud    (1000) arnaud    (1000)        0 2019-09-26 14:31:59.000000 cflib-0.1.8/sys_test/swarm_test_rig/
--rw-r--r--   0 arnaud    (1000) arnaud    (1000)     2805 2019-06-18 14:37:53.000000 cflib-0.1.8/sys_test/swarm_test_rig/test_logging.py
--rw-r--r--   0 arnaud    (1000) arnaud    (1000)     4020 2019-06-18 14:37:53.000000 cflib-0.1.8/sys_test/swarm_test_rig/test_memory_map.py
--rw-r--r--   0 arnaud    (1000) arnaud    (1000)     1033 2019-06-18 14:37:53.000000 cflib-0.1.8/sys_test/swarm_test_rig/__init__.py
--rw-r--r--   0 arnaud    (1000) arnaud    (1000)     4118 2019-06-18 14:37:53.000000 cflib-0.1.8/sys_test/swarm_test_rig/test_connection.py
--rw-r--r--   0 arnaud    (1000) arnaud    (1000)     4810 2019-06-18 14:37:53.000000 cflib-0.1.8/sys_test/swarm_test_rig/test_response_time.py
--rw-r--r--   0 arnaud    (1000) arnaud    (1000)     2828 2019-06-18 14:37:53.000000 cflib-0.1.8/sys_test/swarm_test_rig/rig_support.py
--rw-r--r--   0 arnaud    (1000) arnaud    (1000)        0 2019-06-18 14:37:53.000000 cflib-0.1.8/sys_test/__init__.py
-drwxr-xr-x   0 arnaud    (1000) arnaud    (1000)        0 2019-09-26 14:31:59.000000 cflib-0.1.8/cflib.egg-info/
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)      578 2019-09-26 14:31:59.000000 cflib-0.1.8/cflib.egg-info/PKG-INFO
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)     1983 2019-09-26 14:31:59.000000 cflib-0.1.8/cflib.egg-info/SOURCES.txt
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)       27 2019-09-26 14:31:59.000000 cflib-0.1.8/cflib.egg-info/top_level.txt
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)       15 2019-09-26 14:31:59.000000 cflib-0.1.8/cflib.egg-info/requires.txt
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)        1 2019-09-26 14:31:59.000000 cflib-0.1.8/cflib.egg-info/dependency_links.txt
-drwxr-xr-x   0 arnaud    (1000) arnaud    (1000)        0 2019-09-26 14:31:59.000000 cflib-0.1.8/cflib/
-drwxr-xr-x   0 arnaud    (1000) arnaud    (1000)        0 2019-09-26 14:31:59.000000 cflib-0.1.8/cflib/crazyflie/
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)     7974 2018-08-29 11:11:23.000000 cflib-0.1.8/cflib/crazyflie/toc.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)     6749 2018-10-10 16:42:45.000000 cflib-0.1.8/cflib/crazyflie/high_level_commander.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)    23248 2018-08-20 12:32:39.000000 cflib-0.1.8/cflib/crazyflie/log.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)     1660 2018-01-17 13:55:46.000000 cflib-0.1.8/cflib/crazyflie/extpos.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)     4188 2018-01-17 13:55:46.000000 cflib-0.1.8/cflib/crazyflie/toccache.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)    15848 2018-10-10 16:42:45.000000 cflib-0.1.8/cflib/crazyflie/__init__.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)     4817 2019-06-18 15:00:13.000000 cflib-0.1.8/cflib/crazyflie/commander.py
--rw-r--r--   0 arnaud    (1000) arnaud    (1000)    50321 2019-06-05 08:06:01.000000 cflib-0.1.8/cflib/crazyflie/mem.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)     4296 2018-09-05 11:49:33.000000 cflib-0.1.8/cflib/crazyflie/platformservice.py
--rw-r--r--   0 arnaud    (1000) arnaud    (1000)     3873 2019-06-18 14:37:53.000000 cflib-0.1.8/cflib/crazyflie/syncCrazyflie.py
--rw-r--r--   0 arnaud    (1000) arnaud    (1000)    12919 2019-03-18 15:43:07.000000 cflib-0.1.8/cflib/crazyflie/param.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)     6484 2018-01-25 13:44:07.000000 cflib-0.1.8/cflib/crazyflie/swarm.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)     1978 2018-01-17 13:55:46.000000 cflib-0.1.8/cflib/crazyflie/console.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)     3419 2018-01-17 13:55:46.000000 cflib-0.1.8/cflib/crazyflie/syncLogger.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)     4081 2018-01-17 13:55:46.000000 cflib-0.1.8/cflib/crazyflie/localization.py
-drwxr-xr-x   0 arnaud    (1000) arnaud    (1000)        0 2019-09-26 14:31:59.000000 cflib-0.1.8/cflib/positioning/
--rw-r--r--   0 arnaud    (1000) arnaud    (1000)     9578 2019-09-26 14:28:21.000000 cflib-0.1.8/cflib/positioning/position_hl_commander.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)    15496 2018-11-19 14:05:32.000000 cflib-0.1.8/cflib/positioning/motion_commander.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)     1033 2018-01-17 13:55:46.000000 cflib-0.1.8/cflib/positioning/__init__.py
-drwxr-xr-x   0 arnaud    (1000) arnaud    (1000)        0 2019-09-26 14:31:59.000000 cflib-0.1.8/cflib/utils/
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)     3700 2018-03-22 12:34:48.000000 cflib-0.1.8/cflib/utils/multiranger.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)     1153 2018-01-17 13:55:46.000000 cflib-0.1.8/cflib/utils/__init__.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)     1841 2018-01-17 13:55:46.000000 cflib-0.1.8/cflib/utils/callbacks.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)     2100 2018-01-17 13:55:46.000000 cflib-0.1.8/cflib/__init__.py
-drwxr-xr-x   0 arnaud    (1000) arnaud    (1000)        0 2019-09-26 14:31:59.000000 cflib-0.1.8/cflib/bootloader/
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)    14168 2018-11-19 14:05:32.000000 cflib-0.1.8/cflib/bootloader/__init__.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)     2969 2018-01-17 13:55:46.000000 cflib-0.1.8/cflib/bootloader/boottypes.py
--rw-r--r--   0 arnaud    (1000) arnaud    (1000)    13379 2019-05-02 12:20:52.000000 cflib-0.1.8/cflib/bootloader/cloader.py
-drwxr-xr-x   0 arnaud    (1000) arnaud    (1000)        0 2019-09-26 14:31:59.000000 cflib-0.1.8/cflib/crtp/
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)     1602 2018-01-17 13:55:46.000000 cflib-0.1.8/cflib/crtp/exceptions.py
--rw-r--r--   0 arnaud    (1000) arnaud    (1000)    19371 2019-06-05 08:06:01.000000 cflib-0.1.8/cflib/crtp/radiodriver.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)     3067 2018-05-30 13:56:03.000000 cflib-0.1.8/cflib/crtp/__init__.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)     2822 2018-01-17 13:55:46.000000 cflib-0.1.8/cflib/crtp/crtpdriver.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)     7733 2018-05-03 13:00:22.000000 cflib-0.1.8/cflib/crtp/radio2Driver.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)     4667 2018-10-10 16:42:45.000000 cflib-0.1.8/cflib/crtp/crtpstack.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)    39763 2018-11-19 14:05:32.000000 cflib-0.1.8/cflib/crtp/debugdriver.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)     1968 2018-01-17 13:55:46.000000 cflib-0.1.8/cflib/crtp/serialdriver.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)     7989 2018-01-17 13:55:46.000000 cflib-0.1.8/cflib/crtp/usbdriver.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)     3231 2018-01-17 13:55:46.000000 cflib-0.1.8/cflib/crtp/udpdriver.py
-drwxr-xr-x   0 arnaud    (1000) arnaud    (1000)        0 2019-09-26 14:31:59.000000 cflib-0.1.8/cflib/drivers/
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)     6451 2018-11-19 14:05:32.000000 cflib-0.1.8/cflib/drivers/cfusb.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)     1164 2018-01-17 13:55:46.000000 cflib-0.1.8/cflib/drivers/__init__.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)    10642 2019-04-23 12:39:21.000000 cflib-0.1.8/cflib/drivers/crazyradio.py
-drwxr-xr-x   0 arnaud    (1000) arnaud    (1000)        0 2019-09-26 14:31:59.000000 cflib-0.1.8/lpslib/
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)     1497 2018-01-17 13:55:46.000000 cflib-0.1.8/lpslib/__init__.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)     2540 2018-09-05 10:40:43.000000 cflib-0.1.8/lpslib/lopoanchor.py
--rw-rw-r--   0 arnaud    (1000) arnaud    (1000)       67 2019-09-26 14:31:59.000000 cflib-0.1.8/setup.cfg
+drwxr-xr-x   0 kristoffer   (501) staff       (20)        0 2020-02-06 11:50:17.000000 cflib-0.1.9/
+-rw-r--r--   0 kristoffer   (501) staff       (20)      578 2020-02-06 11:50:17.000000 cflib-0.1.9/PKG-INFO
+-rw-r--r--   0 kristoffer   (501) staff       (20)     4599 2020-02-06 11:49:32.000000 cflib-0.1.9/README.md
+drwxr-xr-x   0 kristoffer   (501) staff       (20)        0 2020-02-06 11:50:17.000000 cflib-0.1.9/cflib/
+-rw-r--r--   0 kristoffer   (501) staff       (20)     2100 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/__init__.py
+drwxr-xr-x   0 kristoffer   (501) staff       (20)        0 2020-02-06 11:50:17.000000 cflib-0.1.9/cflib/bootloader/
+-rw-r--r--   0 kristoffer   (501) staff       (20)    14168 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/bootloader/__init__.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)     2969 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/bootloader/boottypes.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)    13707 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/bootloader/cloader.py
+drwxr-xr-x   0 kristoffer   (501) staff       (20)        0 2020-02-06 11:50:17.000000 cflib-0.1.9/cflib/crazyflie/
+-rw-r--r--   0 kristoffer   (501) staff       (20)    15848 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/crazyflie/__init__.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)     4817 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/crazyflie/commander.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)     1978 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/crazyflie/console.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)     1979 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/crazyflie/extpos.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)     7429 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/crazyflie/high_level_commander.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)     4823 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/crazyflie/localization.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)    23248 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/crazyflie/log.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)    50321 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/crazyflie/mem.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)    12919 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/crazyflie/param.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)     4296 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/crazyflie/platformservice.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)     6484 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/crazyflie/swarm.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)     3873 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/crazyflie/syncCrazyflie.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)     3419 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/crazyflie/syncLogger.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)     7974 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/crazyflie/toc.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)     4188 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/crazyflie/toccache.py
+drwxr-xr-x   0 kristoffer   (501) staff       (20)        0 2020-02-06 11:50:17.000000 cflib-0.1.9/cflib/crtp/
+-rw-r--r--   0 kristoffer   (501) staff       (20)     3067 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/crtp/__init__.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)     2822 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/crtp/crtpdriver.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)     4667 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/crtp/crtpstack.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)    39763 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/crtp/debugdriver.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)     1602 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/crtp/exceptions.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)    19371 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/crtp/radiodriver.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)     1968 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/crtp/serialdriver.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)     3231 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/crtp/udpdriver.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)     7989 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/crtp/usbdriver.py
+drwxr-xr-x   0 kristoffer   (501) staff       (20)        0 2020-02-06 11:50:17.000000 cflib-0.1.9/cflib/drivers/
+-rw-r--r--   0 kristoffer   (501) staff       (20)     1164 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/drivers/__init__.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)     6487 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/drivers/cfusb.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)    10626 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/drivers/crazyradio.py
+drwxr-xr-x   0 kristoffer   (501) staff       (20)        0 2020-02-06 11:50:17.000000 cflib-0.1.9/cflib/positioning/
+-rw-r--r--   0 kristoffer   (501) staff       (20)     1033 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/positioning/__init__.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)    15496 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/positioning/motion_commander.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)     9578 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/positioning/position_hl_commander.py
+drwxr-xr-x   0 kristoffer   (501) staff       (20)        0 2020-02-06 11:50:17.000000 cflib-0.1.9/cflib/utils/
+-rw-r--r--   0 kristoffer   (501) staff       (20)     1153 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/utils/__init__.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)     1841 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/utils/callbacks.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)     3700 2020-02-06 11:49:32.000000 cflib-0.1.9/cflib/utils/multiranger.py
+drwxr-xr-x   0 kristoffer   (501) staff       (20)        0 2020-02-06 11:50:17.000000 cflib-0.1.9/cflib.egg-info/
+-rw-r--r--   0 kristoffer   (501) staff       (20)      578 2020-02-06 11:50:17.000000 cflib-0.1.9/cflib.egg-info/PKG-INFO
+-rw-r--r--   0 kristoffer   (501) staff       (20)     1956 2020-02-06 11:50:17.000000 cflib-0.1.9/cflib.egg-info/SOURCES.txt
+-rw-r--r--   0 kristoffer   (501) staff       (20)        1 2020-02-06 11:50:17.000000 cflib-0.1.9/cflib.egg-info/dependency_links.txt
+-rw-r--r--   0 kristoffer   (501) staff       (20)       15 2020-02-06 11:50:17.000000 cflib-0.1.9/cflib.egg-info/requires.txt
+-rw-r--r--   0 kristoffer   (501) staff       (20)       27 2020-02-06 11:50:17.000000 cflib-0.1.9/cflib.egg-info/top_level.txt
+drwxr-xr-x   0 kristoffer   (501) staff       (20)        0 2020-02-06 11:50:17.000000 cflib-0.1.9/lpslib/
+-rw-r--r--   0 kristoffer   (501) staff       (20)     1497 2020-02-06 11:49:32.000000 cflib-0.1.9/lpslib/__init__.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)     2540 2020-02-06 11:49:32.000000 cflib-0.1.9/lpslib/lopoanchor.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)       67 2020-02-06 11:50:17.000000 cflib-0.1.9/setup.cfg
+-rw-r--r--   0 kristoffer   (501) staff       (20)      784 2020-02-06 11:49:32.000000 cflib-0.1.9/setup.py
+drwxr-xr-x   0 kristoffer   (501) staff       (20)        0 2020-02-06 11:50:17.000000 cflib-0.1.9/sys_test/
+-rw-r--r--   0 kristoffer   (501) staff       (20)        0 2020-02-06 11:49:32.000000 cflib-0.1.9/sys_test/__init__.py
+drwxr-xr-x   0 kristoffer   (501) staff       (20)        0 2020-02-06 11:50:17.000000 cflib-0.1.9/sys_test/swarm_test_rig/
+-rw-r--r--   0 kristoffer   (501) staff       (20)     1033 2020-02-06 11:49:32.000000 cflib-0.1.9/sys_test/swarm_test_rig/__init__.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)     2828 2020-02-06 11:49:32.000000 cflib-0.1.9/sys_test/swarm_test_rig/rig_support.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)     4118 2020-02-06 11:49:32.000000 cflib-0.1.9/sys_test/swarm_test_rig/test_connection.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)     2805 2020-02-06 11:49:32.000000 cflib-0.1.9/sys_test/swarm_test_rig/test_logging.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)     4020 2020-02-06 11:49:32.000000 cflib-0.1.9/sys_test/swarm_test_rig/test_memory_map.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)     4810 2020-02-06 11:49:32.000000 cflib-0.1.9/sys_test/swarm_test_rig/test_response_time.py
+drwxr-xr-x   0 kristoffer   (501) staff       (20)        0 2020-02-06 11:50:17.000000 cflib-0.1.9/test/
+-rw-r--r--   0 kristoffer   (501) staff       (20)        0 2020-02-06 11:49:32.000000 cflib-0.1.9/test/__init__.py
+drwxr-xr-x   0 kristoffer   (501) staff       (20)        0 2020-02-06 11:50:17.000000 cflib-0.1.9/test/crazyflie/
+-rw-r--r--   0 kristoffer   (501) staff       (20)        0 2020-02-06 11:49:32.000000 cflib-0.1.9/test/crazyflie/__init__.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)     6269 2020-02-06 11:49:32.000000 cflib-0.1.9/test/crazyflie/test_swarm.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)     4496 2020-02-06 11:49:32.000000 cflib-0.1.9/test/crazyflie/test_syncCrazyflie.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)     6595 2020-02-06 11:49:32.000000 cflib-0.1.9/test/crazyflie/test_syncLogger.py
+drwxr-xr-x   0 kristoffer   (501) staff       (20)        0 2020-02-06 11:50:17.000000 cflib-0.1.9/test/crtp/
+-rw-r--r--   0 kristoffer   (501) staff       (20)        0 2020-02-06 11:49:32.000000 cflib-0.1.9/test/crtp/__init__.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)     2875 2020-02-06 11:49:32.000000 cflib-0.1.9/test/crtp/test_crtpstack.py
+drwxr-xr-x   0 kristoffer   (501) staff       (20)        0 2020-02-06 11:50:17.000000 cflib-0.1.9/test/positioning/
+-rw-r--r--   0 kristoffer   (501) staff       (20)        0 2020-02-06 11:49:32.000000 cflib-0.1.9/test/positioning/__init__.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)    14623 2020-02-06 11:49:32.000000 cflib-0.1.9/test/positioning/test_motion_commander.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)    11409 2020-02-06 11:49:32.000000 cflib-0.1.9/test/positioning/test_position_hl_commander.py
+drwxr-xr-x   0 kristoffer   (501) staff       (20)        0 2020-02-06 11:50:17.000000 cflib-0.1.9/test/support/
+-rw-r--r--   0 kristoffer   (501) staff       (20)        0 2020-02-06 11:49:32.000000 cflib-0.1.9/test/support/__init__.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)     1593 2020-02-06 11:49:32.000000 cflib-0.1.9/test/support/asyncCallbackCaller.py
+drwxr-xr-x   0 kristoffer   (501) staff       (20)        0 2020-02-06 11:50:17.000000 cflib-0.1.9/test/utils/
+-rw-r--r--   0 kristoffer   (501) staff       (20)        0 2020-02-06 11:49:32.000000 cflib-0.1.9/test/utils/__init__.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)     2734 2020-02-06 11:49:32.000000 cflib-0.1.9/test/utils/test_callbacks.py
+-rw-r--r--   0 kristoffer   (501) staff       (20)     9196 2020-02-06 11:49:32.000000 cflib-0.1.9/test/utils/test_multiranger.py
```

### Comparing `cflib-0.1.8/setup.py` & `cflib-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name='cflib',
-    version='0.1.8',
+    version='0.1.9',
     packages=find_packages(exclude=['examples', 'tests']),
 
     description='Crazyflie python driver',
     url='https://github.com/bitcraze/crazyflie-lib-python',
 
     author='Bitcraze and contributors',
     author_email='contact@bitcraze.io',
```

### Comparing `cflib-0.1.8/PKG-INFO` & `cflib-0.1.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cflib
-Version: 0.1.8
+Version: 0.1.9
 Summary: Crazyflie python driver
 Home-page: https://github.com/bitcraze/crazyflie-lib-python
 Author: Bitcraze and contributors
 Author-email: contact@bitcraze.io
 License: GPLv3
 Description: UNKNOWN
 Keywords: driver crazyflie quadcopter
```

### Comparing `cflib-0.1.8/test/crazyflie/test_syncLogger.py` & `cflib-0.1.9/test/crazyflie/test_syncLogger.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/test/crazyflie/test_swarm.py` & `cflib-0.1.9/test/crazyflie/test_swarm.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/test/crazyflie/test_syncCrazyflie.py` & `cflib-0.1.9/test/crazyflie/test_syncCrazyflie.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/test/positioning/test_position_hl_commander.py` & `cflib-0.1.9/test/positioning/test_position_hl_commander.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/test/positioning/test_motion_commander.py` & `cflib-0.1.9/test/positioning/test_motion_commander.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/test/utils/test_callbacks.py` & `cflib-0.1.9/test/utils/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/test/utils/test_multiranger.py` & `cflib-0.1.9/test/utils/test_multiranger.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/test/support/asyncCallbackCaller.py` & `cflib-0.1.9/test/support/asyncCallbackCaller.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/test/crtp/test_crtpstack.py` & `cflib-0.1.9/test/crtp/test_crtpstack.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/README.md` & `cflib-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/sys_test/swarm_test_rig/test_logging.py` & `cflib-0.1.9/sys_test/swarm_test_rig/test_logging.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/sys_test/swarm_test_rig/test_memory_map.py` & `cflib-0.1.9/sys_test/swarm_test_rig/test_memory_map.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/sys_test/swarm_test_rig/__init__.py` & `cflib-0.1.9/sys_test/swarm_test_rig/__init__.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/sys_test/swarm_test_rig/test_connection.py` & `cflib-0.1.9/sys_test/swarm_test_rig/test_connection.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/sys_test/swarm_test_rig/test_response_time.py` & `cflib-0.1.9/sys_test/swarm_test_rig/test_response_time.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/sys_test/swarm_test_rig/rig_support.py` & `cflib-0.1.9/sys_test/swarm_test_rig/rig_support.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/cflib.egg-info/PKG-INFO` & `cflib-0.1.9/cflib.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cflib
-Version: 0.1.8
+Version: 0.1.9
 Summary: Crazyflie python driver
 Home-page: https://github.com/bitcraze/crazyflie-lib-python
 Author: Bitcraze and contributors
 Author-email: contact@bitcraze.io
 License: GPLv3
 Description: UNKNOWN
 Keywords: driver crazyflie quadcopter
```

### Comparing `cflib-0.1.8/cflib.egg-info/SOURCES.txt` & `cflib-0.1.9/cflib.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 cflib/crazyflie/toc.py
 cflib/crazyflie/toccache.py
 cflib/crtp/__init__.py
 cflib/crtp/crtpdriver.py
 cflib/crtp/crtpstack.py
 cflib/crtp/debugdriver.py
 cflib/crtp/exceptions.py
-cflib/crtp/radio2Driver.py
 cflib/crtp/radiodriver.py
 cflib/crtp/serialdriver.py
 cflib/crtp/udpdriver.py
 cflib/crtp/usbdriver.py
 cflib/drivers/__init__.py
 cflib/drivers/cfusb.py
 cflib/drivers/crazyradio.py
```

### Comparing `cflib-0.1.8/cflib/crazyflie/toc.py` & `cflib-0.1.9/cflib/crazyflie/toc.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/cflib/crazyflie/high_level_commander.py` & `cflib-0.1.9/cflib/crazyflie/high_level_commander.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #
 #     ||          ____  _ __
 #  +------+      / __ )(_) /_______________ _____  ___
 #  | 0xBC |     / __  / / __/ ___/ ___/ __ `/_  / / _ \
 #  +------+    / /_/ / / /_/ /__/ /  / /_/ / / /_/  __/
 #   ||  ||    /_____/_/\__/\___/_/   \__,_/ /___/\___/
 #
-#  Copyright (C) 2018 Bitcraze AB
+#  Copyright (C) 2018-2020 Bitcraze AB
 #
 #  Crazyflie Nano Quadcopter Client
 #
 #  This program is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU General Public License
 #  as published by the Free Software Foundation; either version 2
 #  of the License, or (at your option) any later version.
@@ -38,20 +38,20 @@
 
 class HighLevelCommander():
     """
     Used for sending high level setpoints to the Crazyflie
     """
 
     COMMAND_SET_GROUP_MASK = 0
-    COMMAND_TAKEOFF = 1
-    COMMAND_LAND = 2
     COMMAND_STOP = 3
     COMMAND_GO_TO = 4
     COMMAND_START_TRAJECTORY = 5
     COMMAND_DEFINE_TRAJECTORY = 6
+    COMMAND_TAKEOFF_2 = 7
+    COMMAND_LAND_2 = 8
 
     ALL_GROUPS = 0
 
     TRAJECTORY_LOCATION_MEM = 1
     TRAJECTORY_TYPE_POLY4D = 0
 
     def __init__(self, crazyflie=None):
@@ -66,42 +66,62 @@
 
         :param group_mask: mask for which groups this CF belongs to
         """
         self._send_packet(struct.pack('<BB',
                                       self.COMMAND_SET_GROUP_MASK,
                                       group_mask))
 
-    def takeoff(self, absolute_height_m, duration_s, group_mask=ALL_GROUPS):
+    def takeoff(self, absolute_height_m, duration_s, group_mask=ALL_GROUPS,
+                yaw=0.0):
         """
         vertical takeoff from current x-y position to given height
 
         :param absolute_height_m: absolut (m)
         :param duration_s: time it should take until target height is
                            reached (s)
         :param group_mask: mask for which CFs this should apply to
+        :param yaw: yaw (rad). Use current yaw if set to None.
         """
-        self._send_packet(struct.pack('<BBff',
-                                      self.COMMAND_TAKEOFF,
+        target_yaw = yaw
+        useCurrentYaw = False
+        if yaw is None:
+            target_yaw = 0.0
+            useCurrentYaw = True
+
+        self._send_packet(struct.pack('<BBff?f',
+                                      self.COMMAND_TAKEOFF_2,
                                       group_mask,
                                       absolute_height_m,
+                                      target_yaw,
+                                      useCurrentYaw,
                                       duration_s))
 
-    def land(self, absolute_height_m, duration_s, group_mask=ALL_GROUPS):
+    def land(self, absolute_height_m, duration_s, group_mask=ALL_GROUPS,
+             yaw=0.0):
         """
         vertical land from current x-y position to given height
 
         :param absolute_height_m: absolut (m)
         :param duration_s: time it should take until target height is
                            reached (s)
         :param group_mask: mask for which CFs this should apply to
+        :param yaw: yaw (rad). Use current yaw if set to None.
         """
-        self._send_packet(struct.pack('<BBff',
-                                      self.COMMAND_LAND,
+        target_yaw = yaw
+        useCurrentYaw = False
+        if yaw is None:
+            target_yaw = 0.0
+            useCurrentYaw = True
+
+        self._send_packet(struct.pack('<BBff?f',
+                                      self.COMMAND_LAND_2,
                                       group_mask,
                                       absolute_height_m,
+                                      target_yaw,
+                                      useCurrentYaw,
                                       duration_s))
 
     def stop(self, group_mask=ALL_GROUPS):
         """
         stops the current trajectory (turns off the motors)
 
         :param group_mask: mask for which CFs this should apply to
```

### Comparing `cflib-0.1.8/cflib/crazyflie/log.py` & `cflib-0.1.9/cflib/crazyflie/log.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/cflib/crazyflie/extpos.py` & `cflib-0.1.9/cflib/crazyflie/extpos.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #
 #     ||          ____  _ __
 #  +------+      / __ )(_) /_______________ _____  ___
 #  | 0xBC |     / __  / / __/ ___/ ___/ __ `/_  / / _ \
 #  +------+    / /_/ / / /_/ /__/ /  / /_/ / / /_/  __/
 #   ||  ||    /_____/_/\__/\___/_/   \__,_/ /___/\___/
 #
-#  Copyright (C) 2011-2013 Bitcraze AB
+#  Copyright (C) 2011-2020 Bitcraze AB
 #
 #  Crazyflie Nano Quadcopter Client
 #
 #  This program is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU General Public License
 #  as published by the Free Software Foundation; either version 2
 #  of the License, or (at your option) any later version.
@@ -46,7 +46,15 @@
     def send_extpos(self, x, y, z):
         """
         Send the current Crazyflie X, Y, Z position. This is going to be
         forwarded to the Crazyflie's position estimator.
         """
 
         self._cf.loc.send_extpos([x, y, z])
+
+    def send_extpose(self, x, y, z, qx, qy, qz, qw):
+        """
+        Send the current Crazyflie X, Y, Z position and attitude as a
+        normalized quaternion. This is going to be forwarded to the
+        Crazyflie's position estimator.
+        """
+        self._cf.loc.send_extpose([x, y, z], [qx, qy, qz, qw])
```

### Comparing `cflib-0.1.8/cflib/crazyflie/toccache.py` & `cflib-0.1.9/cflib/crazyflie/toccache.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/cflib/crazyflie/__init__.py` & `cflib-0.1.9/cflib/crazyflie/__init__.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/cflib/crazyflie/commander.py` & `cflib-0.1.9/cflib/crazyflie/commander.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/cflib/crazyflie/mem.py` & `cflib-0.1.9/cflib/crazyflie/mem.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/cflib/crazyflie/platformservice.py` & `cflib-0.1.9/cflib/crazyflie/platformservice.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/cflib/crazyflie/syncCrazyflie.py` & `cflib-0.1.9/cflib/crazyflie/syncCrazyflie.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/cflib/crazyflie/param.py` & `cflib-0.1.9/cflib/crazyflie/param.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/cflib/crazyflie/swarm.py` & `cflib-0.1.9/cflib/crazyflie/swarm.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/cflib/crazyflie/console.py` & `cflib-0.1.9/cflib/crazyflie/console.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/cflib/crazyflie/syncLogger.py` & `cflib-0.1.9/cflib/crazyflie/syncLogger.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/cflib/crazyflie/localization.py` & `cflib-0.1.9/cflib/crazyflie/localization.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #
 #     ||          ____  _ __
 #  +------+      / __ )(_) /_______________ _____  ___
 #  | 0xBC |     / __  / / __/ ___/ ___/ __ `/_  / / _ \
 #  +------+    / /_/ / / /_/ /__/ /  / /_/ / / /_/  __/
 #   ||  ||    /_____/_/\__/\___/_/   \__,_/ /___/\___/
 #
-#  Copyright (C) 2017 Bitcraze AB
+#  Copyright (C) 2017-2020 Bitcraze AB
 #
 #  Crazyflie Nano Quadcopter Client
 #
 #  This program is free software; you can redistribute it and/or
 #  modify it under the terms of the GNU General Public License
 #  as published by the Free Software Foundation; either version 2
 #  of the License, or (at your option) any later version.
@@ -52,17 +52,23 @@
     """
 
     # Implemented channels
     POSITION_CH = 0
     GENERIC_CH = 1
 
     # Location message types for generig channel
-    RANGE_STREAM_REPORT = 0x00
-    RANGE_STREAM_REPORT_FP16 = 0x01
-    LPS_SHORT_LPP_PACKET = 0x02
+    RANGE_STREAM_REPORT = 0
+    RANGE_STREAM_REPORT_FP16 = 1
+    LPS_SHORT_LPP_PACKET = 2
+    EMERGENCY_STOP = 3
+    EMERGENCY_STOP_WATCHDOG = 4
+    COMM_GNSS_NMEA = 6
+    COMM_GNSS_PROPRIETARY = 7
+    EXT_POSE = 8
+    EXT_POSE_PACKED = 9
 
     def __init__(self, crazyflie=None):
         """
         Initialize the Extpos object.
         """
         self._cf = crazyflie
 
@@ -106,14 +112,30 @@
 
         pk = CRTPPacket()
         pk.port = CRTPPort.LOCALIZATION
         pk.channel = self.POSITION_CH
         pk.data = struct.pack('<fff', pos[0], pos[1], pos[2])
         self._cf.send_packet(pk)
 
+    def send_extpose(self, pos, quat):
+        """
+        Send the current Crazyflie pose (position [x, y, z] and
+        attitude quaternion [qx, qy, qz, qw]). This is going to be forwarded
+        to the Crazyflie's position estimator.
+        """
+
+        pk = CRTPPacket()
+        pk.port = CRTPPort.LOCALIZATION
+        pk.channel = self.GENERIC_CH
+        pk.data = struct.pack('<Bfffffff',
+                              self.EXT_POSE,
+                              pos[0], pos[1], pos[2],
+                              quat[0], quat[1], quat[2], quat[3])
+        self._cf.send_packet(pk)
+
     def send_short_lpp_packet(self, dest_id, data):
         """
         Send ultra-wide-band LPP packet to dest_id
         """
 
         pk = CRTPPacket()
         pk.port = CRTPPort.LOCALIZATION
```

### Comparing `cflib-0.1.8/cflib/positioning/position_hl_commander.py` & `cflib-0.1.9/cflib/positioning/position_hl_commander.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/cflib/positioning/motion_commander.py` & `cflib-0.1.9/cflib/positioning/motion_commander.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/cflib/positioning/__init__.py` & `cflib-0.1.9/cflib/positioning/__init__.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/cflib/utils/multiranger.py` & `cflib-0.1.9/cflib/utils/multiranger.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/cflib/utils/__init__.py` & `cflib-0.1.9/cflib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/cflib/utils/callbacks.py` & `cflib-0.1.9/cflib/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/cflib/__init__.py` & `cflib-0.1.9/cflib/__init__.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/cflib/bootloader/__init__.py` & `cflib-0.1.9/cflib/bootloader/__init__.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/cflib/bootloader/boottypes.py` & `cflib-0.1.9/cflib/bootloader/boottypes.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/cflib/bootloader/cloader.py` & `cflib-0.1.9/cflib/bootloader/cloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -377,15 +377,22 @@
                 struct.unpack('<BB', pk.data[0:2]) != (addr, 0x18)) and
                retry_counter >= 0):
             pk = CRTPPacket()
             pk.set_header(0xFF, 0xFF)
             pk.data = struct.pack('<BBHHH', addr, 0x18, page_buffer,
                                   target_page, page_count)
             self.link.send_packet(pk)
-            pk = self.link.receive_packet(1)
+
+            # Timeout for writing to flash is raised from 1s (used elsewhere
+            # in this module) to 2.5s because it may take more than a second
+            # to erase a page on the STM32F405.
+            #
+            # See https://github.com/bitcraze/crazyflie-lib-python/issues/98
+            # for more details.
+            pk = self.link.receive_packet(2.5)
             retry_counter -= 1
 
         if retry_counter < 0:
             self.error_code = -1
             return False
 
         self.error_code = pk.data[3]
```

### Comparing `cflib-0.1.8/cflib/crtp/exceptions.py` & `cflib-0.1.9/cflib/crtp/exceptions.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/cflib/crtp/radiodriver.py` & `cflib-0.1.9/cflib/crtp/radiodriver.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/cflib/crtp/__init__.py` & `cflib-0.1.9/cflib/crtp/__init__.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/cflib/crtp/crtpdriver.py` & `cflib-0.1.9/cflib/crtp/crtpdriver.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/cflib/crtp/crtpstack.py` & `cflib-0.1.9/cflib/crtp/crtpstack.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/cflib/crtp/debugdriver.py` & `cflib-0.1.9/cflib/crtp/debugdriver.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/cflib/crtp/serialdriver.py` & `cflib-0.1.9/cflib/crtp/serialdriver.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/cflib/crtp/usbdriver.py` & `cflib-0.1.9/cflib/crtp/usbdriver.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/cflib/crtp/udpdriver.py` & `cflib-0.1.9/cflib/crtp/udpdriver.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/cflib/drivers/cfusb.py` & `cflib-0.1.9/cflib/drivers/cfusb.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,16 @@
     ret = []
 
     logger.info('Looking for devices....')
 
     if pyusb1:
         for d in usb.core.find(idVendor=USB_VID, idProduct=USB_PID, find_all=1,
                                backend=pyusb_backend):
-            ret.append(d)
+            if d.manufacturer == 'Bitcraze AB':
+                ret.append(d)
     else:
         busses = usb.busses()
         for bus in busses:
             for device in bus.devices:
                 if device.idVendor == USB_VID:
                     if device.idProduct == USB_PID:
                         ret += [device, ]
@@ -116,18 +117,17 @@
         except (usb.core.USBError, ValueError):
             return usb.util.get_string(self.dev, self.dev.iSerialNumber)
 
     def close(self):
         if (pyusb1 is False):
             if self.handle:
                 self.handle.releaseInterface()
-                self.handle.reset()
         else:
             if self.dev:
-                self.dev.reset()
+                usb.util.dispose_resources(self.dev)
 
         self.handle = None
         self.dev = None
 
     def scan(self):
         # TODO: Currently only supports one device
         if self.dev:
```

### Comparing `cflib-0.1.8/cflib/drivers/__init__.py` & `cflib-0.1.9/cflib/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/cflib/drivers/crazyradio.py` & `cflib-0.1.9/cflib/drivers/crazyradio.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,18 +165,17 @@
             self.set_ard_bytes(32)
             self.set_ack_enable(True)
 
     def close(self):
         if (pyusb1 is False):
             if self.handle:
                 self.handle.releaseInterface()
-                self.handle.reset()
         else:
             if self.dev:
-                self.dev.reset()
+                usb.util.dispose_resources(self.dev)
 
         self.handle = None
         self.dev = None
 
         self.current_channel = None
         self.current_address = None
         self.current_datarate = None
```

### Comparing `cflib-0.1.8/lpslib/__init__.py` & `cflib-0.1.9/lpslib/__init__.py`

 * *Files identical despite different names*

### Comparing `cflib-0.1.8/lpslib/lopoanchor.py` & `cflib-0.1.9/lpslib/lopoanchor.py`

 * *Files identical despite different names*

