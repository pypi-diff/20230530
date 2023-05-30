# Comparing `tmp/KiwiCoder-0.2.3.4.tar.gz` & `tmp/KiwiCoder-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KiwiCoder-0.2.3.4.tar", last modified: Wed Mar  1 02:52:59 2023, max compression
+gzip compressed data, was "KiwiCoder-0.3.tar", last modified: Tue May 30 06:09:23 2023, max compression
```

## Comparing `KiwiCoder-0.2.3.4.tar` & `KiwiCoder-0.3.tar`

### file list

```diff
@@ -1,18 +1,76 @@
-drwxrwxrwx   0        0        0        0 2023-03-01 02:52:59.613177 KiwiCoder-0.2.3.4/
-drwxrwxrwx   0        0        0        0 2023-03-01 02:52:57.408548 KiwiCoder-0.2.3.4/KiwiCoder.egg-info/
--rw-rw-rw-   0        0        0      276 2023-03-01 02:52:57.000000 KiwiCoder-0.2.3.4/KiwiCoder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2023-03-01 02:52:57.000000 KiwiCoder-0.2.3.4/KiwiCoder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-01 02:52:57.000000 KiwiCoder-0.2.3.4/KiwiCoder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      106 2023-03-01 02:52:57.000000 KiwiCoder-0.2.3.4/KiwiCoder.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-03-01 02:52:57.000000 KiwiCoder-0.2.3.4/KiwiCoder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11558 2023-01-05 05:57:12.000000 KiwiCoder-0.2.3.4/LICENSE
--rw-rw-rw-   0        0        0      276 2023-03-01 02:52:59.613177 KiwiCoder-0.2.3.4/PKG-INFO
--rw-rw-rw-   0        0        0       62 2023-02-27 12:22:24.000000 KiwiCoder-0.2.3.4/README.md
-drwxrwxrwx   0        0        0        0 2023-03-01 02:52:57.410547 KiwiCoder-0.2.3.4/kiwi/
--rw-rw-rw-   0        0        0       51 2023-02-28 06:07:41.000000 KiwiCoder-0.2.3.4/kiwi/__init__.py
--rw-rw-rw-   0        0        0      401 2023-03-01 02:52:59.614178 KiwiCoder-0.2.3.4/setup.cfg
--rw-rw-rw-   0        0        0      326 2023-02-28 05:25:49.000000 KiwiCoder-0.2.3.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-01 02:52:59.568266 KiwiCoder-0.2.3.4/tests/
--rw-rw-rw-   0        0        0     1014 2023-02-28 05:25:21.000000 KiwiCoder-0.2.3.4/tests/test_app.py
--rw-rw-rw-   0        0        0      438 2023-02-28 05:25:21.000000 KiwiCoder-0.2.3.4/tests/test_eventbus.py
--rw-rw-rw-   0        0        0      713 2023-02-28 05:25:21.000000 KiwiCoder-0.2.3.4/tests/test_mock.py
+drwxrwxrwx   0        0        0        0 2023-05-30 06:09:23.833599 KiwiCoder-0.3/
+drwxrwxrwx   0        0        0        0 2023-05-30 06:09:23.763378 KiwiCoder-0.3/KiwiCoder.egg-info/
+-rw-rw-rw-   0        0        0      260 2023-05-30 06:09:23.000000 KiwiCoder-0.3/KiwiCoder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1445 2023-05-30 06:09:23.000000 KiwiCoder-0.3/KiwiCoder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 06:09:23.000000 KiwiCoder-0.3/KiwiCoder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-30 06:09:23.000000 KiwiCoder-0.3/KiwiCoder.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      106 2023-05-30 06:09:23.000000 KiwiCoder-0.3/KiwiCoder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-30 06:09:23.000000 KiwiCoder-0.3/KiwiCoder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11558 2023-01-05 05:57:12.000000 KiwiCoder-0.3/LICENSE
+-rw-rw-rw-   0        0        0      260 2023-05-30 06:09:23.833599 KiwiCoder-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    11206 2023-05-16 14:24:47.000000 KiwiCoder-0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 06:09:23.765376 KiwiCoder-0.3/kiwi/
+-rw-rw-rw-   0        0        0       83 2023-03-12 05:16:30.000000 KiwiCoder-0.3/kiwi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 06:09:23.767420 KiwiCoder-0.3/kiwi/apps/
+-rw-rw-rw-   0        0        0       37 2023-03-12 05:16:30.000000 KiwiCoder-0.3/kiwi/apps/__init__.py
+-rw-rw-rw-   0        0        0     1542 2023-04-07 10:06:26.000000 KiwiCoder-0.3/kiwi/apps/app.py
+drwxrwxrwx   0        0        0        0 2023-05-30 06:09:23.769376 KiwiCoder-0.3/kiwi/cli/
+-rw-rw-rw-   0        0        0       34 2023-03-04 04:13:41.000000 KiwiCoder-0.3/kiwi/cli/__init__.py
+-rw-rw-rw-   0        0        0     5718 2023-04-07 10:06:26.000000 KiwiCoder-0.3/kiwi/cli/command.py
+drwxrwxrwx   0        0        0        0 2023-05-30 06:09:23.779379 KiwiCoder-0.3/kiwi/common/
+-rw-rw-rw-   0        0        0      142 2023-03-04 04:13:41.000000 KiwiCoder-0.3/kiwi/common/__init__.py
+-rw-rw-rw-   0        0        0     7107 2023-04-07 10:06:26.000000 KiwiCoder-0.3/kiwi/common/common.py
+-rw-rw-rw-   0        0        0     7271 2023-05-16 14:28:07.000000 KiwiCoder-0.3/kiwi/common/constant.py
+-rw-rw-rw-   0        0        0     2496 2023-04-07 10:06:26.000000 KiwiCoder-0.3/kiwi/common/exception.py
+-rw-rw-rw-   0        0        0      488 2023-02-18 10:01:09.000000 KiwiCoder-0.3/kiwi/common/message.py
+drwxrwxrwx   0        0        0        0 2023-05-30 06:09:23.798376 KiwiCoder-0.3/kiwi/core/
+-rw-rw-rw-   0        0        0      239 2023-03-12 05:16:30.000000 KiwiCoder-0.3/kiwi/core/__init__.py
+-rw-rw-rw-   0        0        0     2363 2023-05-04 08:38:21.000000 KiwiCoder-0.3/kiwi/core/bio_entity.py
+-rw-rw-rw-   0        0        0     3974 2023-05-16 14:24:47.000000 KiwiCoder-0.3/kiwi/core/bio_obj.py
+-rw-rw-rw-   0        0        0    23460 2023-05-16 14:24:47.000000 KiwiCoder-0.3/kiwi/core/bio_op.py
+-rw-rw-rw-   0        0        0     3982 2023-05-04 08:38:21.000000 KiwiCoder-0.3/kiwi/core/bio_periphery.py
+-rw-rw-rw-   0        0        0     3459 2023-04-07 10:06:26.000000 KiwiCoder-0.3/kiwi/core/bio_quantity.py
+-rw-rw-rw-   0        0        0      576 2023-04-07 10:06:26.000000 KiwiCoder-0.3/kiwi/core/globals.py
+-rw-rw-rw-   0        0        0    20478 2023-05-16 14:39:50.000000 KiwiCoder-0.3/kiwi/core/kiwi_sys.py
+-rw-rw-rw-   0        0        0     3158 2023-05-04 08:38:21.000000 KiwiCoder-0.3/kiwi/core/report.py
+-rw-rw-rw-   0        0        0     5752 2023-05-16 16:36:50.000000 KiwiCoder-0.3/kiwi/core/sched.py
+-rw-rw-rw-   0        0        0     5305 2023-05-16 16:26:55.000000 KiwiCoder-0.3/kiwi/core/step.py
+-rw-rw-rw-   0        0        0     1357 2023-04-07 10:06:26.000000 KiwiCoder-0.3/kiwi/core/watch.py
+drwxrwxrwx   0        0        0        0 2023-05-30 06:09:23.800377 KiwiCoder-0.3/kiwi/endpoint/
+-rw-rw-rw-   0        0        0       44 2023-04-07 10:06:26.000000 KiwiCoder-0.3/kiwi/endpoint/__init__.py
+-rw-rw-rw-   0        0        0     2442 2023-04-07 10:06:26.000000 KiwiCoder-0.3/kiwi/endpoint/server.py
+drwxrwxrwx   0        0        0        0 2023-05-30 06:09:23.802376 KiwiCoder-0.3/kiwi/plugin/
+-rw-rw-rw-   0        0        0        0 2023-02-14 15:35:59.000000 KiwiCoder-0.3/kiwi/plugin/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 06:09:23.802376 KiwiCoder-0.3/kiwi/plugin/hardware/
+-rw-rw-rw-   0        0        0        2 2023-02-14 15:35:59.000000 KiwiCoder-0.3/kiwi/plugin/hardware/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 06:09:23.805377 KiwiCoder-0.3/kiwi/plugin/hardware/control/
+-rw-rw-rw-   0        0        0       24 2023-02-14 15:35:59.000000 KiwiCoder-0.3/kiwi/plugin/hardware/control/__init__.py
+-rw-rw-rw-   0        0        0     3053 2023-04-07 10:06:26.000000 KiwiCoder-0.3/kiwi/plugin/hardware/control/phidget.py
+drwxrwxrwx   0        0        0        0 2023-05-30 06:09:23.812404 KiwiCoder-0.3/kiwi/plugin/hardware/instrum/
+-rw-rw-rw-   0        0        0       50 2023-02-14 15:35:59.000000 KiwiCoder-0.3/kiwi/plugin/hardware/instrum/__init__.py
+-rw-rw-rw-   0        0        0      523 2023-04-07 10:06:26.000000 KiwiCoder-0.3/kiwi/plugin/hardware/instrum/amplify.py
+-rw-rw-rw-   0        0        0     1874 2023-05-04 08:38:21.000000 KiwiCoder-0.3/kiwi/plugin/hardware/instrum/flowmeter.py
+-rw-rw-rw-   0        0        0      695 2023-05-04 08:38:21.000000 KiwiCoder-0.3/kiwi/plugin/hardware/instrum/pipettor.py
+drwxrwxrwx   0        0        0        0 2023-05-30 06:09:23.815375 KiwiCoder-0.3/kiwi/plugin/hardware/signal/
+-rw-rw-rw-   0        0        0       43 2023-02-14 15:35:59.000000 KiwiCoder-0.3/kiwi/plugin/hardware/signal/__init__.py
+-rw-rw-rw-   0        0        0      919 2023-05-04 08:38:21.000000 KiwiCoder-0.3/kiwi/plugin/hardware/signal/pump.py
+-rw-rw-rw-   0        0        0      806 2023-05-04 08:38:21.000000 KiwiCoder-0.3/kiwi/plugin/hardware/signal/valve.py
+drwxrwxrwx   0        0        0        0 2023-05-30 06:09:23.821095 KiwiCoder-0.3/kiwi/util/
+-rw-rw-rw-   0        0        0      118 2023-03-04 04:13:41.000000 KiwiCoder-0.3/kiwi/util/__init__.py
+-rw-rw-rw-   0        0        0      680 2023-04-05 08:29:47.000000 KiwiCoder-0.3/kiwi/util/encoder.py
+-rw-rw-rw-   0        0        0     2693 2023-02-28 05:25:21.000000 KiwiCoder-0.3/kiwi/util/event.py
+-rw-rw-rw-   0        0        0     3696 2023-03-12 05:16:30.000000 KiwiCoder-0.3/kiwi/util/graph.py
+-rw-rw-rw-   0        0        0     2375 2023-02-28 05:25:21.000000 KiwiCoder-0.3/kiwi/util/tree.py
+drwxrwxrwx   0        0        0        0 2023-05-30 06:09:23.826100 KiwiCoder-0.3/kiwi/wrapper/
+-rw-rw-rw-   0        0        0       75 2023-03-12 05:16:30.000000 KiwiCoder-0.3/kiwi/wrapper/__init__.py
+-rw-rw-rw-   0        0        0     9929 2023-05-04 08:38:21.000000 KiwiCoder-0.3/kiwi/wrapper/op_wrapper.py
+-rw-rw-rw-   0        0        0     6790 2023-05-16 15:39:32.000000 KiwiCoder-0.3/kiwi/wrapper/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-05-30 06:09:23.829100 KiwiCoder-0.3/scripts/
+-rw-rw-rw-   0        0        0        0 2023-03-04 04:13:41.000000 KiwiCoder-0.3/scripts/__init__.py
+-rw-rw-rw-   0        0        0     2641 2023-04-07 10:06:26.000000 KiwiCoder-0.3/scripts/gen.py
+-rw-rw-rw-   0        0        0      397 2023-05-30 06:09:23.834611 KiwiCoder-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      262 2023-03-04 04:13:41.000000 KiwiCoder-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 06:09:23.833098 KiwiCoder-0.3/tests/
+-rw-rw-rw-   0        0        0     1014 2023-03-04 04:13:41.000000 KiwiCoder-0.3/tests/test_app.py
+-rw-rw-rw-   0        0        0      438 2023-02-28 05:25:21.000000 KiwiCoder-0.3/tests/test_eventbus.py
+-rw-rw-rw-   0        0        0      713 2023-03-04 04:13:41.000000 KiwiCoder-0.3/tests/test_mock.py
```

### Comparing `KiwiCoder-0.2.3.4/LICENSE` & `KiwiCoder-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `KiwiCoder-0.2.3.4/tests/test_app.py` & `KiwiCoder-0.3/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `KiwiCoder-0.2.3.4/tests/test_mock.py` & `KiwiCoder-0.3/tests/test_mock.py`

 * *Files identical despite different names*

