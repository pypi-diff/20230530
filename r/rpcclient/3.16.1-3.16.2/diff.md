# Comparing `tmp/rpcclient-3.16.1.tar.gz` & `tmp/rpcclient-3.16.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpcclient-3.16.1.tar", last modified: Mon May 29 12:38:08 2023, max compression
+gzip compressed data, was "rpcclient-3.16.2.tar", last modified: Tue May 30 11:07:53 2023, max compression
```

## Comparing `rpcclient-3.16.1.tar` & `rpcclient-3.16.2.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:38:08.430976 rpcclient-3.16.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-29 12:37:51.000000 rpcclient-3.16.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41718 2023-05-29 12:38:08.430976 rpcclient-3.16.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-29 12:37:51.000000 rpcclient-3.16.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-29 12:37:51.000000 rpcclient-3.16.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-29 12:37:51.000000 rpcclient-3.16.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:38:08.422976 rpcclient-3.16.1/rpcclient/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/allocated.py
--rw-r--r--   0 runner    (1001) docker     (123)    23530 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/client_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:38:08.426976 rpcclient-3.16.1/rpcclient/darwin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/darwin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/darwin/bluetooth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/darwin/cfpreferences.py
--rw-r--r--   0 runner    (1001) docker     (123)    12396 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/darwin/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/darwin/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    37890 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/darwin/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/darwin/core_graphics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/darwin/crash_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/darwin/darwin_lief.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/darwin/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/darwin/hid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/darwin/ioregistry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/darwin/keychain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/darwin/location.py
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/darwin/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/darwin/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/darwin/objc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/darwin/objective_c_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     7700 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/darwin/objective_c_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/darwin/power.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/darwin/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)    33780 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/darwin/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/darwin/reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/darwin/scpreferences.py
--rw-r--r--   0 runner    (1001) docker     (123)    29308 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/darwin/structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/darwin/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/darwin/syslog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/darwin/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/darwin/xpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20310 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/fs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:38:08.426976 rpcclient-3.16.1/rpcclient/ios/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/ios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17603 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/ios/accessibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/ios/amfi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/ios/backlight.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/ios/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/ios/lockdown.py
--rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/ios/mobile_gestalt.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/ios/screen_capture.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/ios/sprinboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/ios/telephony.py
--rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/ios/wifi.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/lief.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:38:08.426976 rpcclient-3.16.1/rpcclient/linux/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/linux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/linux/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/linux/structs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:38:08.426976 rpcclient-3.16.1/rpcclient/macos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/macos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/macos/apple_script.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/macos/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/network.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:38:08.430976 rpcclient-3.16.1/rpcclient/structs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/structs/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/structs/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/symbols_jar.py
--rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/sysctl.py
--rw-r--r--   0 runner    (1001) docker     (123)    24398 2023-05-29 12:37:51.000000 rpcclient-3.16.1/rpcclient/xonshrc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:38:08.422976 rpcclient-3.16.1/rpcclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41718 2023-05-29 12:38:08.000000 rpcclient-3.16.1/rpcclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-29 12:38:08.000000 rpcclient-3.16.1/rpcclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 12:38:08.000000 rpcclient-3.16.1/rpcclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-29 12:38:08.000000 rpcclient-3.16.1/rpcclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-29 12:38:08.000000 rpcclient-3.16.1/rpcclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-29 12:38:08.000000 rpcclient-3.16.1/rpcclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 12:38:08.430976 rpcclient-3.16.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:38:08.430976 rpcclient-3.16.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-29 12:37:51.000000 rpcclient-3.16.1/tests/test_allocation_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-29 12:37:51.000000 rpcclient-3.16.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-29 12:37:51.000000 rpcclient-3.16.1/tests/test_core_foundation_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-29 12:37:51.000000 rpcclient-3.16.1/tests/test_darwin_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-05-29 12:37:51.000000 rpcclient-3.16.1/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-29 12:37:51.000000 rpcclient-3.16.1/tests/test_keychain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-29 12:37:51.000000 rpcclient-3.16.1/tests/test_objc_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-29 12:37:51.000000 rpcclient-3.16.1/tests/test_power.py
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-05-29 12:37:51.000000 rpcclient-3.16.1/tests/test_preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-29 12:37:51.000000 rpcclient-3.16.1/tests/test_processes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-29 12:37:51.000000 rpcclient-3.16.1/tests/test_socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-29 12:37:51.000000 rpcclient-3.16.1/tests/test_spawn.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-29 12:37:51.000000 rpcclient-3.16.1/tests/test_thread_safe.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-29 12:37:51.000000 rpcclient-3.16.1/tests/test_time.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-29 12:37:51.000000 rpcclient-3.16.1/tests/test_worker_processes.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-29 12:37:51.000000 rpcclient-3.16.1/tests/test_xpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:07:53.588823 rpcclient-3.16.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-30 11:07:35.000000 rpcclient-3.16.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    41739 2023-05-30 11:07:53.588823 rpcclient-3.16.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-30 11:07:35.000000 rpcclient-3.16.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-30 11:07:35.000000 rpcclient-3.16.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-30 11:07:35.000000 rpcclient-3.16.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:07:53.580823 rpcclient-3.16.2/rpcclient/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/allocated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23530 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/client_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:07:53.584823 rpcclient-3.16.2/rpcclient/darwin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/bluetooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/cfpreferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12396 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37890 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/core_graphics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/crash_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/darwin_lief.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8438 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/hid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/ioregistry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/keychain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/objc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/objective_c_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7700 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/objective_c_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/power.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33780 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/scpreferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29308 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/syslog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/darwin/xpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20680 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/fs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:07:53.584823 rpcclient-3.16.2/rpcclient/ios/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/ios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17603 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/ios/accessibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/ios/amfi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/ios/backlight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/ios/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/ios/lockdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/ios/mobile_gestalt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/ios/screen_capture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/ios/sprinboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/ios/telephony.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7605 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/ios/wifi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/lief.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:07:53.584823 rpcclient-3.16.2/rpcclient/linux/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/linux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/linux/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/linux/structs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:07:53.584823 rpcclient-3.16.2/rpcclient/macos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/macos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/macos/apple_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/macos/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:07:53.584823 rpcclient-3.16.2/rpcclient/structs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/structs/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/structs/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/symbols_jar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/sysctl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24398 2023-05-30 11:07:35.000000 rpcclient-3.16.2/rpcclient/xonshrc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:07:53.580823 rpcclient-3.16.2/rpcclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41739 2023-05-30 11:07:53.000000 rpcclient-3.16.2/rpcclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-30 11:07:53.000000 rpcclient-3.16.2/rpcclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:07:53.000000 rpcclient-3.16.2/rpcclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-30 11:07:53.000000 rpcclient-3.16.2/rpcclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-30 11:07:53.000000 rpcclient-3.16.2/rpcclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-30 11:07:53.000000 rpcclient-3.16.2/rpcclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 11:07:53.588823 rpcclient-3.16.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:07:53.588823 rpcclient-3.16.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-30 11:07:35.000000 rpcclient-3.16.2/tests/test_allocation_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-30 11:07:35.000000 rpcclient-3.16.2/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-30 11:07:35.000000 rpcclient-3.16.2/tests/test_core_foundation_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-30 11:07:35.000000 rpcclient-3.16.2/tests/test_darwin_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-05-30 11:07:35.000000 rpcclient-3.16.2/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-30 11:07:35.000000 rpcclient-3.16.2/tests/test_keychain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-30 11:07:35.000000 rpcclient-3.16.2/tests/test_objc_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-30 11:07:35.000000 rpcclient-3.16.2/tests/test_power.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-05-30 11:07:35.000000 rpcclient-3.16.2/tests/test_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-30 11:07:35.000000 rpcclient-3.16.2/tests/test_processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-30 11:07:35.000000 rpcclient-3.16.2/tests/test_socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-30 11:07:35.000000 rpcclient-3.16.2/tests/test_spawn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-30 11:07:35.000000 rpcclient-3.16.2/tests/test_thread_safe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-30 11:07:35.000000 rpcclient-3.16.2/tests/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-30 11:07:35.000000 rpcclient-3.16.2/tests/test_worker_processes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-30 11:07:35.000000 rpcclient-3.16.2/tests/test_xpc.py
```

### Comparing `rpcclient-3.16.1/LICENSE` & `rpcclient-3.16.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/PKG-INFO` & `rpcclient-3.16.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpcclient
-Version: 3.16.1
+Version: 3.16.2
 Summary: rpcclient for connecting with the rpcserver
 Author-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
 Maintainer-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
@@ -690,13 +690,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
+Provides-Extra: docs
 License-File: LICENSE
 
 # rpcclient
 
 For details about this project please review:
 https://github.com/doronz88/rpc-project
```

### Comparing `rpcclient-3.16.1/pyproject.toml` & `rpcclient-3.16.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rpcclient"
-version = "3.16.1"
+version = "3.16.2"
 description = "rpcclient for connecting with the rpcserver"
 readme = "README.md"
 requires-python = ">=3.7"
 license = { file = "LICENSE" }
 keywords = ["ios", "macos", "linux", "automation", "remote-shell", "remote-control", "ipython"]
 authors = [
     { name = "doronz88", email = "doron88@gmail.com" },
@@ -25,14 +25,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
 ]
 dynamic = ["dependencies"]
 
 [project.optional-dependencies]
 test = ["pytest"]
+docs = ["toml", "myst_parser", "sphinx", "sphinx-rtd-theme"]
 
 [project.urls]
 "Homepage" = "https://github.com/doronz88/rpc-project"
 "Bug Reports" = "https://github.com/doronz88/rpc-project/issues"
 
 [project.scripts]
 rpcclient = "rpcclient.__main__:cli"
```

### Comparing `rpcclient-3.16.1/rpcclient/__main__.py` & `rpcclient-3.16.2/rpcclient/__main__.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/client.py` & `rpcclient-3.16.2/rpcclient/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/client_factory.py` & `rpcclient-3.16.2/rpcclient/client_factory.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/darwin/bluetooth.py` & `rpcclient-3.16.2/rpcclient/darwin/bluetooth.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/darwin/cfpreferences.py` & `rpcclient-3.16.2/rpcclient/darwin/cfpreferences.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/darwin/client.py` & `rpcclient-3.16.2/rpcclient/darwin/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/darwin/consts.py` & `rpcclient-3.16.2/rpcclient/darwin/consts.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/darwin/core_graphics.py` & `rpcclient-3.16.2/rpcclient/darwin/core_graphics.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/darwin/crash_reports.py` & `rpcclient-3.16.2/rpcclient/darwin/crash_reports.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/darwin/darwin_lief.py` & `rpcclient-3.16.2/rpcclient/darwin/darwin_lief.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/darwin/fs.py` & `rpcclient-3.16.2/rpcclient/darwin/fs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/darwin/hid.py` & `rpcclient-3.16.2/rpcclient/darwin/hid.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/darwin/ioregistry.py` & `rpcclient-3.16.2/rpcclient/darwin/ioregistry.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/darwin/keychain.py` & `rpcclient-3.16.2/rpcclient/darwin/keychain.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/darwin/location.py` & `rpcclient-3.16.2/rpcclient/darwin/location.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/darwin/media.py` & `rpcclient-3.16.2/rpcclient/darwin/media.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/darwin/network.py` & `rpcclient-3.16.2/rpcclient/darwin/network.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/darwin/objc.py` & `rpcclient-3.16.2/rpcclient/darwin/objc.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/darwin/objective_c_class.py` & `rpcclient-3.16.2/rpcclient/darwin/objective_c_class.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/darwin/objective_c_symbol.py` & `rpcclient-3.16.2/rpcclient/darwin/objective_c_symbol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/darwin/power.py` & `rpcclient-3.16.2/rpcclient/darwin/power.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,12 +72,15 @@
 
     def copy_scheduled_power_events(self) -> List[Mapping]:
         """ List all scheduled system power events """
         return self._client.symbols.IOPMCopyScheduledPowerEvents().py()
 
     def copy_assertions_status(self) -> Mapping[str, int]:
         """ Returns a list of available assertions and their system-wide levels """
-        return self._client.symbols.IOPMCopyAssertionsStatus().py()
+        with self._client.safe_malloc(8) as result:
+            if 0 != self._client.symbols.IOPMCopyAssertionsStatus(result):
+                raise BadReturnValueError('IOPMCopyAssertionsStatus() failed')
+            return result[0].py()
 
     def reboot(self) -> None:
         if self._client.symbols.reboot().c_int64 == -1:
             raise BadReturnValueError()
```

### Comparing `rpcclient-3.16.1/rpcclient/darwin/processes.py` & `rpcclient-3.16.2/rpcclient/darwin/processes.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/darwin/reports.py` & `rpcclient-3.16.2/rpcclient/darwin/reports.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/darwin/scpreferences.py` & `rpcclient-3.16.2/rpcclient/darwin/scpreferences.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/darwin/structs.py` & `rpcclient-3.16.2/rpcclient/darwin/structs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/darwin/symbol.py` & `rpcclient-3.16.2/rpcclient/darwin/symbol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/darwin/syslog.py` & `rpcclient-3.16.2/rpcclient/darwin/syslog.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/darwin/time.py` & `rpcclient-3.16.2/rpcclient/darwin/time.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/darwin/xpc.py` & `rpcclient-3.16.2/rpcclient/darwin/xpc.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/exceptions.py` & `rpcclient-3.16.2/rpcclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/fs.py` & `rpcclient-3.16.2/rpcclient/fs.py`

 * *Files 5% similar despite different names*

```diff
@@ -298,14 +298,22 @@
             if self._client.symbols.readlink(path, buf, MAXPATHLEN).c_int64 < 0:
                 self._client.raise_errno_exception(f'readlink failed for: {path}')
             if absolute:
                 return str(Path(path).parent / buf.peek_str())
             return buf.peek_str()
 
     @path_to_str('path')
+    def realpath(self, path: str) -> str:
+        """ realpath() at remote. read man for more details. """
+        with self._client.safe_malloc(MAXPATHLEN) as buf:
+            if self._client.symbols.realpath(path, buf) == 0:
+                self._client.raise_errno_exception(f'realpath failed for: {path}')
+            return buf.peek_str()
+
+    @path_to_str('path')
     def is_symlink(self, path: str) -> bool:
         try:
             self.readlink(path)
             return True
         except BadReturnValueError:
             return False
```

### Comparing `rpcclient-3.16.1/rpcclient/ios/accessibility.py` & `rpcclient-3.16.2/rpcclient/ios/accessibility.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/ios/amfi.py` & `rpcclient-3.16.2/rpcclient/ios/amfi.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/ios/backlight.py` & `rpcclient-3.16.2/rpcclient/ios/backlight.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/ios/client.py` & `rpcclient-3.16.2/rpcclient/ios/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/ios/lockdown.py` & `rpcclient-3.16.2/rpcclient/ios/lockdown.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/ios/mobile_gestalt.py` & `rpcclient-3.16.2/rpcclient/ios/mobile_gestalt.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/ios/screen_capture.py` & `rpcclient-3.16.2/rpcclient/ios/screen_capture.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/ios/sprinboard.py` & `rpcclient-3.16.2/rpcclient/ios/sprinboard.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/ios/telephony.py` & `rpcclient-3.16.2/rpcclient/ios/telephony.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/ios/wifi.py` & `rpcclient-3.16.2/rpcclient/ios/wifi.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/lief.py` & `rpcclient-3.16.2/rpcclient/lief.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/linux/client.py` & `rpcclient-3.16.2/rpcclient/linux/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/linux/structs.py` & `rpcclient-3.16.2/rpcclient/linux/structs.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/macos/apple_script.py` & `rpcclient-3.16.2/rpcclient/macos/apple_script.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/macos/client.py` & `rpcclient-3.16.2/rpcclient/macos/client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/network.py` & `rpcclient-3.16.2/rpcclient/network.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/processes.py` & `rpcclient-3.16.2/rpcclient/processes.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/protocol.py` & `rpcclient-3.16.2/rpcclient/protocol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/structs/consts.py` & `rpcclient-3.16.2/rpcclient/structs/consts.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/structs/generic.py` & `rpcclient-3.16.2/rpcclient/structs/generic.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/symbol.py` & `rpcclient-3.16.2/rpcclient/symbol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/symbols_jar.py` & `rpcclient-3.16.2/rpcclient/symbols_jar.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/sysctl.py` & `rpcclient-3.16.2/rpcclient/sysctl.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient/xonshrc.py` & `rpcclient-3.16.2/rpcclient/xonshrc.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/rpcclient.egg-info/PKG-INFO` & `rpcclient-3.16.2/rpcclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpcclient
-Version: 3.16.1
+Version: 3.16.2
 Summary: rpcclient for connecting with the rpcserver
 Author-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
 Maintainer-email: doronz88 <doron88@gmail.com>, matan <matan1008@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
@@ -690,13 +690,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
+Provides-Extra: docs
 License-File: LICENSE
 
 # rpcclient
 
 For details about this project please review:
 https://github.com/doronz88/rpc-project
```

### Comparing `rpcclient-3.16.1/rpcclient.egg-info/SOURCES.txt` & `rpcclient-3.16.2/rpcclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/tests/test_allocation_cleanup.py` & `rpcclient-3.16.2/tests/test_allocation_cleanup.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/tests/test_client.py` & `rpcclient-3.16.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/tests/test_darwin_client.py` & `rpcclient-3.16.2/tests/test_darwin_client.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/tests/test_fs.py` & `rpcclient-3.16.2/tests/test_fs.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,18 @@
     symlink = (tmp_path / 'temp1.txt')
     client.fs.touch(file)
     client.fs.symlink(file, symlink)
     assert client.fs.accessible(symlink)
     assert client.fs.readlink(symlink) == str(file)
 
 
+def test_realpath(client, tmp_path):
+    assert client.fs.realpath(tmp_path / '././') == str(tmp_path)
+
+
 def test_link(client, tmp_path):
     client.fs.write_file(tmp_path / 'temp.txt', b'hello')
     client.fs.link((tmp_path / 'temp.txt'), (tmp_path / 'temp1.txt'))
     assert client.fs.read_file(tmp_path / 'temp1.txt') == b'hello'
 
 
 def test_listdir(client, tmp_path):
```

### Comparing `rpcclient-3.16.1/tests/test_objc_symbol.py` & `rpcclient-3.16.2/tests/test_objc_symbol.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/tests/test_power.py` & `rpcclient-3.16.2/tests/test_power.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 import pytest
 
 from rpcclient.darwin.consts import IOPMUserActiveType
 
 pytestmark = pytest.mark.darwin
 
 
+def test_copy_assertions_status(client):
+    """
+    :param rpcclient.darwin.client.DarwinClient client:
+    """
+    assertions = client.power.copy_assertions_status()
+    assert len(assertions) > 0
+
+
 def test_copy_assertions_by_process(client):
     """
     :param rpcclient.darwin.client.DarwinClient client:
     """
     assertions = client.power.copy_assertions_by_process()
     assert len(assertions) > 0
```

### Comparing `rpcclient-3.16.1/tests/test_preferences.py` & `rpcclient-3.16.2/tests/test_preferences.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/tests/test_processes.py` & `rpcclient-3.16.2/tests/test_processes.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/tests/test_socket.py` & `rpcclient-3.16.2/tests/test_socket.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/tests/test_spawn.py` & `rpcclient-3.16.2/tests/test_spawn.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/tests/test_thread_safe.py` & `rpcclient-3.16.2/tests/test_thread_safe.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/tests/test_time.py` & `rpcclient-3.16.2/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `rpcclient-3.16.1/tests/test_xpc.py` & `rpcclient-3.16.2/tests/test_xpc.py`

 * *Files identical despite different names*

