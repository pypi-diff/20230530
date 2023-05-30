# Comparing `tmp/rivalcfg-4.8.0.tar.gz` & `tmp/rivalcfg-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rivalcfg-4.8.0.tar", last modified: Wed Dec 28 12:33:36 2022, max compression
+gzip compressed data, was "rivalcfg-4.9.0.tar", last modified: Tue May 30 11:04:20 2023, max compression
```

## Comparing `rivalcfg-4.8.0.tar` & `rivalcfg-4.9.0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 12:33:36.431553 rivalcfg-4.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20335 2022-12-28 12:33:36.431553 rivalcfg-4.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19660 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 12:33:36.423552 rivalcfg-4.8.0/rivalcfg/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/color_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 12:33:36.427553 rivalcfg-4.8.0/rivalcfg/devices/
--rw-r--r--   0 runner    (1001) docker     (123)     9063 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6170 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/devices/aerox3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/devices/aerox3_wireless_wired.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/devices/aerox3_wireless_wireless.py
--rw-r--r--   0 runner    (1001) docker     (123)     7035 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/devices/aerox5_wireless_wired.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/devices/aerox5_wireless_wireless.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/devices/aerox9_wireless_wired.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/devices/aerox9_wireless_wireless.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/devices/kanav2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/devices/kinzuv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/devices/prime.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/devices/prime_wireless_wired.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/devices/prime_wireless_wireless.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/devices/rival100.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/devices/rival110.py
--rw-r--r--   0 runner    (1001) docker     (123)     5840 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/devices/rival3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6634 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/devices/rival300.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/devices/rival300s.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/devices/rival310.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/devices/rival3_wireless.py
--rw-r--r--   0 runner    (1001) docker     (123)     5260 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/devices/rival500.py
--rw-r--r--   0 runner    (1001) docker     (123)     6745 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/devices/rival600.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/devices/rival650.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/devices/rival700.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/devices/rival95.py
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/devices/sensei310.py
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/devices/sensei_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/devices/sensei_ten.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 12:33:36.427553 rivalcfg-4.8.0/rivalcfg/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/handlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 12:33:36.431553 rivalcfg-4.8.0/rivalcfg/handlers/buttons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/handlers/buttons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11098 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/handlers/buttons/buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/handlers/buttons/layout_multimedia.py
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/handlers/buttons/layout_qwerty.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/handlers/choice.py
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/handlers/multidpi_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/handlers/none.py
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/handlers/range.py
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/handlers/reactive_rgbcolor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/handlers/rgbcolor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11428 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/handlers/rgbgradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     8919 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/handlers/rgbgradientv2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11507 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/mouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     7348 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/mouse_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/udev.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/usbhid.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/rivalcfg/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 12:33:36.423552 rivalcfg-4.8.0/rivalcfg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20335 2022-12-28 12:33:36.000000 rivalcfg-4.8.0/rivalcfg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2022-12-28 12:33:36.000000 rivalcfg-4.8.0/rivalcfg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-28 12:33:36.000000 rivalcfg-4.8.0/rivalcfg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2022-12-28 12:33:36.000000 rivalcfg-4.8.0/rivalcfg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2022-12-28 12:33:36.000000 rivalcfg-4.8.0/rivalcfg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2022-12-28 12:33:36.000000 rivalcfg-4.8.0/rivalcfg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-28 12:33:36.431553 rivalcfg-4.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 12:33:36.431553 rivalcfg-4.8.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/test/test_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/test/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     9499 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/test/test_mouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/test/test_mouse_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/test/test_udev.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2022-12-28 12:33:31.000000 rivalcfg-4.8.0/test/test_usbhid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:04:20.554217 rivalcfg-4.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21438 2023-05-30 11:04:20.554217 rivalcfg-4.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20763 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:04:20.538217 rivalcfg-4.9.0/rivalcfg/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/color_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:04:20.550217 rivalcfg-4.9.0/rivalcfg/devices/
+-rw-r--r--   0 runner    (1001) docker     (123)     9063 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/aerox3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/aerox3_wireless_wired.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/aerox3_wireless_wireless.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/aerox5_wireless_wired.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/aerox5_wireless_wireless.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/aerox9_wireless_wired.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/aerox9_wireless_wireless.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/kanav2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/kinzuv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/prime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/prime_wireless_wired.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/prime_wireless_wireless.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/rival100.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/rival110.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/rival3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/rival300.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/rival300s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/rival310.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/rival3_wireless.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/rival500.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/rival600.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/rival650.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/rival700.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/rival95.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/sensei310.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/sensei_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/devices/sensei_ten.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:04:20.550217 rivalcfg-4.9.0/rivalcfg/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/handlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:04:20.550217 rivalcfg-4.9.0/rivalcfg/handlers/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/handlers/buttons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11098 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/handlers/buttons/buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/handlers/buttons/layout_multimedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/handlers/buttons/layout_qwerty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/handlers/choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/handlers/multidpi_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/handlers/none.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/handlers/range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/handlers/reactive_rgbcolor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/handlers/rgbcolor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11428 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/handlers/rgbgradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/handlers/rgbgradientv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11507 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/mouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/mouse_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/udev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/usbhid.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/rivalcfg/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:04:20.542217 rivalcfg-4.9.0/rivalcfg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21438 2023-05-30 11:04:20.000000 rivalcfg-4.9.0/rivalcfg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-30 11:04:20.000000 rivalcfg-4.9.0/rivalcfg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 11:04:20.000000 rivalcfg-4.9.0/rivalcfg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-30 11:04:20.000000 rivalcfg-4.9.0/rivalcfg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-30 11:04:20.000000 rivalcfg-4.9.0/rivalcfg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-30 11:04:20.000000 rivalcfg-4.9.0/rivalcfg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 11:04:20.554217 rivalcfg-4.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 11:04:20.554217 rivalcfg-4.9.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/test/test_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/test/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/test/test_mouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/test/test_mouse_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/test/test_udev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-30 11:04:16.000000 rivalcfg-4.9.0/test/test_usbhid.py
```

### Comparing `rivalcfg-4.8.0/PKG-INFO` & `rivalcfg-4.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rivalcfg
-Version: 4.8.0
+Version: 4.9.0
 Summary: Configure SteelSeries gaming mice
 Home-page: https://github.com/flozz/rivalcfg
 Author: Fabien LOISON
 License: WTFPL
 Project-URL: Source Code, https://github.com/flozz/rivalcfg
 Project-URL: Documentation, https://flozz.github.io/rivalcfg/
 Project-URL: Changelog, https://github.com/flozz/rivalcfg#changelog
@@ -75,19 +75,27 @@
 | SteelSeries Aerox 3 Wireless (wired mode)                    | 1038:183a |
 +--------------------------------------------------------------+-----------+
 | SteelSeries Aerox 3 Wireless (2.4 GHz wireless mode)         | 1038:1838 |
 +--------------------------------------------------------------+-----------+
 
 SteelSeries Aerox 5 Wireless:
 
-+--------------------------------------------------------------+-----------+
-| SteelSeries Aerox 5 Wireless (wired mode)                    | 1038:1854 |
-+--------------------------------------------------------------+-----------+
-| SteelSeries Aerox 5 Wireless (2.4 GHz wireless mode)         | 1038:1852 |
-+--------------------------------------------------------------+-----------+
++------------------------------------------------------------------------+-----------+
+| SteelSeries Aerox 5 Wireless (wired mode)                              | 1038:1854 |
++------------------------------------------------------------------------+-----------+
+| SteelSeries Aerox 5 Wireless Destiny 2 Edition (wired mode)            | 1038:185e |
++------------------------------------------------------------------------+-----------+
+| SteelSeries Aerox 5 Wireless Diablo IV Edition (wired mode)            | 1038:1862 |
++------------------------------------------------------------------------+-----------+
+| SteelSeries Aerox 5 Wireless (2.4 GHz wireless mode)                   | 1038:1852 |
++------------------------------------------------------------------------+-----------+
+| SteelSeries Aerox 5 Wireless Destiny 2 Edition (2.4 GHz wireless mode) | 1038:185c |
++------------------------------------------------------------------------+-----------+
+| SteelSeries Aerox 5 Wireless Diablo IV Edition (2.4 GHz wireless mode) | 1038:1860 |
++------------------------------------------------------------------------+-----------+
 
 SteelSeries Aerox 9 Wireless:
 
 +--------------------------------------------------------------+-----------+
 | SteelSeries Aerox 9 Wireless (wired mode)                    | 1038:185a |
 +--------------------------------------------------------------+-----------+
 | SteelSeries Aerox 9 Wireless (2.4 GHz wireless mode)         | 1038:1858 |
@@ -291,15 +299,23 @@
 
 
 Changelog
 ---------
 
 * **[NEXT]** (changes on ``master`` that have not been released yet):
 
-  * Nothing yet :)
+  * Nothing yet ;)
+
+* **v4.9.0:**
+
+  * Added Aerox 5 Wireless Destiny 2 Editon support (@flozz, #205)
+  * Added Aerox 5 Wireless Diablo IV Edition support (@flozz, #206)
+  * Updated HIDAPI to v0.14 to fix a macOS Ventura issue (@flozz, #200)
+  * Removed the default lighting option for the Prime mouse (reported not
+    working and not needed on this device) (@flozz, #196)
 
 * **v4.8.0:**
 
   * Improved CLI startup time (@gryzus24, #194)
   * Added default lighting setting to following devices (@flozz, #191, #195):
 
     * Aerox 3
```

### Comparing `rivalcfg-4.8.0/README.rst` & `rivalcfg-4.9.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -56,19 +56,27 @@
 | SteelSeries Aerox 3 Wireless (wired mode)                    | 1038:183a |
 +--------------------------------------------------------------+-----------+
 | SteelSeries Aerox 3 Wireless (2.4 GHz wireless mode)         | 1038:1838 |
 +--------------------------------------------------------------+-----------+
 
 SteelSeries Aerox 5 Wireless:
 
-+--------------------------------------------------------------+-----------+
-| SteelSeries Aerox 5 Wireless (wired mode)                    | 1038:1854 |
-+--------------------------------------------------------------+-----------+
-| SteelSeries Aerox 5 Wireless (2.4 GHz wireless mode)         | 1038:1852 |
-+--------------------------------------------------------------+-----------+
++------------------------------------------------------------------------+-----------+
+| SteelSeries Aerox 5 Wireless (wired mode)                              | 1038:1854 |
++------------------------------------------------------------------------+-----------+
+| SteelSeries Aerox 5 Wireless Destiny 2 Edition (wired mode)            | 1038:185e |
++------------------------------------------------------------------------+-----------+
+| SteelSeries Aerox 5 Wireless Diablo IV Edition (wired mode)            | 1038:1862 |
++------------------------------------------------------------------------+-----------+
+| SteelSeries Aerox 5 Wireless (2.4 GHz wireless mode)                   | 1038:1852 |
++------------------------------------------------------------------------+-----------+
+| SteelSeries Aerox 5 Wireless Destiny 2 Edition (2.4 GHz wireless mode) | 1038:185c |
++------------------------------------------------------------------------+-----------+
+| SteelSeries Aerox 5 Wireless Diablo IV Edition (2.4 GHz wireless mode) | 1038:1860 |
++------------------------------------------------------------------------+-----------+
 
 SteelSeries Aerox 9 Wireless:
 
 +--------------------------------------------------------------+-----------+
 | SteelSeries Aerox 9 Wireless (wired mode)                    | 1038:185a |
 +--------------------------------------------------------------+-----------+
 | SteelSeries Aerox 9 Wireless (2.4 GHz wireless mode)         | 1038:1858 |
@@ -272,15 +280,23 @@
 
 
 Changelog
 ---------
 
 * **[NEXT]** (changes on ``master`` that have not been released yet):
 
-  * Nothing yet :)
+  * Nothing yet ;)
+
+* **v4.9.0:**
+
+  * Added Aerox 5 Wireless Destiny 2 Editon support (@flozz, #205)
+  * Added Aerox 5 Wireless Diablo IV Edition support (@flozz, #206)
+  * Updated HIDAPI to v0.14 to fix a macOS Ventura issue (@flozz, #200)
+  * Removed the default lighting option for the Prime mouse (reported not
+    working and not needed on this device) (@flozz, #196)
 
 * **v4.8.0:**
 
   * Improved CLI startup time (@gryzus24, #194)
   * Added default lighting setting to following devices (@flozz, #191, #195):
 
     * Aerox 3
```

### Comparing `rivalcfg-4.8.0/rivalcfg/__init__.py` & `rivalcfg-4.9.0/rivalcfg/__init__.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/__main__.py` & `rivalcfg-4.9.0/rivalcfg/__main__.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/cli.py` & `rivalcfg-4.9.0/rivalcfg/cli.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/color_helpers.py` & `rivalcfg-4.9.0/rivalcfg/color_helpers.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/debug.py` & `rivalcfg-4.9.0/rivalcfg/debug.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/devices/__init__.py` & `rivalcfg-4.9.0/rivalcfg/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/devices/aerox3.py` & `rivalcfg-4.9.0/rivalcfg/devices/aerox3.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/devices/aerox3_wireless_wired.py` & `rivalcfg-4.9.0/rivalcfg/devices/aerox3_wireless_wired.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/devices/aerox3_wireless_wireless.py` & `rivalcfg-4.9.0/rivalcfg/devices/aerox3_wireless_wireless.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/devices/aerox5_wireless_wired.py` & `rivalcfg-4.9.0/rivalcfg/devices/aerox5_wireless_wired.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,26 @@
     "models": [
         {
             "name": "SteelSeries Aerox 5 Wireless (wired mode)",
             "vendor_id": 0x1038,
             "product_id": 0x1854,
             "endpoint": 3,
         },
+        {
+            "name": "SteelSeries Aerox 5 Wireless Destiny 2 Edition (wired mode)",
+            "vendor_id": 0x1038,
+            "product_id": 0x185E,
+            "endpoint": 3,
+        },
+        {
+            "name": "SteelSeries Aerox 5 Wireless Diablo IV Edition (wired mode)",
+            "vendor_id": 0x1038,
+            "product_id": 0x1862,
+            "endpoint": 3,
+        },
     ],
     "settings": {
         "sensitivity": {
             "label": "Sensibility presets",
             "description": "Set sensitivity preset (DPI)",
             "cli": ["-s", "--sensitivity"],
             "report_type": usbhid.HID_REPORT_TYPE_OUTPUT,
```

### Comparing `rivalcfg-4.8.0/rivalcfg/devices/aerox5_wireless_wireless.py` & `rivalcfg-4.9.0/rivalcfg/devices/aerox9_wireless_wireless.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from . import aerox5_wireless_wired
+from . import aerox9_wireless_wired
 
 
 _WIRELESS_FLAG = 0b01000000
 _READBACK_LENGTH = 64
 
 
 def _patch_command(info):
@@ -14,23 +14,23 @@
     result["command"][0] = result["command"][0] | _WIRELESS_FLAG
     # Add readback
     result["readback_length"] = _READBACK_LENGTH
     return result
 
 
 profile = {
-    "name": "SteelSeries Aerox 5 Wireless",
+    "name": "SteelSeries Aerox 9 Wireless",
     "models": [
         {
-            "name": "SteelSeries Aerox 5 Wireless (2.4 GHz wireless mode)",
+            "name": "SteelSeries Aerox 9 Wireless (2.4 GHz wireless mode)",
             "vendor_id": 0x1038,
-            "product_id": 0x1852,
+            "product_id": 0x1858,
             "endpoint": 3,
         },
     ],
     "settings": {
         name: _patch_command(info)
-        for name, info in aerox5_wireless_wired.profile["settings"].items()
+        for name, info in aerox9_wireless_wired.profile["settings"].items()
     },
-    "battery_level": _patch_command(aerox5_wireless_wired.profile["battery_level"]),
-    "save_command": _patch_command(aerox5_wireless_wired.profile["save_command"]),
+    "battery_level": _patch_command(aerox9_wireless_wired.profile["battery_level"]),
+    "save_command": _patch_command(aerox9_wireless_wired.profile["save_command"]),
 }
```

### Comparing `rivalcfg-4.8.0/rivalcfg/devices/aerox9_wireless_wired.py` & `rivalcfg-4.9.0/rivalcfg/devices/aerox9_wireless_wired.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/devices/aerox9_wireless_wireless.py` & `rivalcfg-4.9.0/rivalcfg/devices/prime_wireless_wireless.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from . import aerox9_wireless_wired
+from . import prime_wireless_wired
 
 
 _WIRELESS_FLAG = 0b01000000
 _READBACK_LENGTH = 64
 
 
 def _patch_command(info):
@@ -14,23 +14,23 @@
     result["command"][0] = result["command"][0] | _WIRELESS_FLAG
     # Add readback
     result["readback_length"] = _READBACK_LENGTH
     return result
 
 
 profile = {
-    "name": "SteelSeries Aerox 9 Wireless",
+    "name": "SteelSeries Prime Wireless",
     "models": [
         {
-            "name": "SteelSeries Aerox 9 Wireless (2.4 GHz wireless mode)",
+            "name": "SteelSeries Prime Wireless (2.4 GHz wireless mode)",
             "vendor_id": 0x1038,
-            "product_id": 0x1858,
+            "product_id": 0x1840,
             "endpoint": 3,
         },
     ],
     "settings": {
         name: _patch_command(info)
-        for name, info in aerox9_wireless_wired.profile["settings"].items()
+        for name, info in prime_wireless_wired.profile["settings"].items()
     },
-    "battery_level": _patch_command(aerox9_wireless_wired.profile["battery_level"]),
-    "save_command": _patch_command(aerox9_wireless_wired.profile["save_command"]),
+    "battery_level": _patch_command(prime_wireless_wired.profile["battery_level"]),
+    "save_command": _patch_command(prime_wireless_wired.profile["save_command"]),
 }
```

### Comparing `rivalcfg-4.8.0/rivalcfg/devices/kanav2.py` & `rivalcfg-4.9.0/rivalcfg/devices/kanav2.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/devices/kinzuv2.py` & `rivalcfg-4.9.0/rivalcfg/devices/kinzuv2.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/devices/prime.py` & `rivalcfg-4.9.0/rivalcfg/devices/prime.py`

 * *Files 18% similar despite different names*

```diff
@@ -89,26 +89,13 @@
             "command": [0x5F],
             "value_type": "range",
             "input_range": [0, 256, 1],
             "output_range": [0, 256, 1],
             "range_length_byte": 2,
             "default": 256,
         },
-        "default_lighting": {
-            "label": "Default lighting",
-            "description": "Set default lighting at mouse startup",
-            "cli": ["-d", "--default-lighting"],
-            "report_type": usbhid.HID_REPORT_TYPE_OUTPUT,
-            "command": [0x27],
-            "value_type": "choice",
-            "choices": {
-                "off": 0x00,
-                "rainbow": 0x01,
-            },
-            "default": "rainbow",
-        },
     },
     "save_command": {
         "report_type": usbhid.HID_REPORT_TYPE_OUTPUT,
         "command": [0x59],
     },
 }
```

### Comparing `rivalcfg-4.8.0/rivalcfg/devices/prime_wireless_wired.py` & `rivalcfg-4.9.0/rivalcfg/devices/prime_wireless_wired.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/devices/prime_wireless_wireless.py` & `rivalcfg-4.9.0/rivalcfg/devices/aerox5_wireless_wireless.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from . import prime_wireless_wired
+from . import aerox5_wireless_wired
 
 
 _WIRELESS_FLAG = 0b01000000
 _READBACK_LENGTH = 64
 
 
 def _patch_command(info):
@@ -14,23 +14,35 @@
     result["command"][0] = result["command"][0] | _WIRELESS_FLAG
     # Add readback
     result["readback_length"] = _READBACK_LENGTH
     return result
 
 
 profile = {
-    "name": "SteelSeries Prime Wireless",
+    "name": "SteelSeries Aerox 5 Wireless",
     "models": [
         {
-            "name": "SteelSeries Prime Wireless (2.4 GHz wireless mode)",
+            "name": "SteelSeries Aerox 5 Wireless (2.4 GHz wireless mode)",
             "vendor_id": 0x1038,
-            "product_id": 0x1840,
+            "product_id": 0x1852,
+            "endpoint": 3,
+        },
+        {
+            "name": "SteelSeries Aerox 5 Wireless Destiny 2 Edition (2.4 GHz wireless mode)",
+            "vendor_id": 0x1038,
+            "product_id": 0x185C,
+            "endpoint": 3,
+        },
+        {
+            "name": "SteelSeries Aerox 5 Wireless Diablo IV Edition (2.4 GHz wireless mode)",
+            "vendor_id": 0x1038,
+            "product_id": 0x1860,
             "endpoint": 3,
         },
     ],
     "settings": {
         name: _patch_command(info)
-        for name, info in prime_wireless_wired.profile["settings"].items()
+        for name, info in aerox5_wireless_wired.profile["settings"].items()
     },
-    "battery_level": _patch_command(prime_wireless_wired.profile["battery_level"]),
-    "save_command": _patch_command(prime_wireless_wired.profile["save_command"]),
+    "battery_level": _patch_command(aerox5_wireless_wired.profile["battery_level"]),
+    "save_command": _patch_command(aerox5_wireless_wired.profile["save_command"]),
 }
```

### Comparing `rivalcfg-4.8.0/rivalcfg/devices/rival100.py` & `rivalcfg-4.9.0/rivalcfg/devices/rival100.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/devices/rival110.py` & `rivalcfg-4.9.0/rivalcfg/devices/rival110.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/devices/rival3.py` & `rivalcfg-4.9.0/rivalcfg/devices/rival3.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/devices/rival300.py` & `rivalcfg-4.9.0/rivalcfg/devices/rival300.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/devices/rival310.py` & `rivalcfg-4.9.0/rivalcfg/devices/rival310.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/devices/rival3_wireless.py` & `rivalcfg-4.9.0/rivalcfg/devices/rival3_wireless.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/devices/rival500.py` & `rivalcfg-4.9.0/rivalcfg/devices/rival500.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/devices/rival600.py` & `rivalcfg-4.9.0/rivalcfg/devices/rival600.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/devices/rival650.py` & `rivalcfg-4.9.0/rivalcfg/devices/rival650.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/devices/rival700.py` & `rivalcfg-4.9.0/rivalcfg/devices/rival700.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/devices/rival95.py` & `rivalcfg-4.9.0/rivalcfg/devices/rival95.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/devices/sensei310.py` & `rivalcfg-4.9.0/rivalcfg/devices/sensei310.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/devices/sensei_raw.py` & `rivalcfg-4.9.0/rivalcfg/devices/sensei_raw.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/devices/sensei_ten.py` & `rivalcfg-4.9.0/rivalcfg/devices/sensei_ten.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/handlers/buttons/buttons.py` & `rivalcfg-4.9.0/rivalcfg/handlers/buttons/buttons.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/handlers/buttons/layout_multimedia.py` & `rivalcfg-4.9.0/rivalcfg/handlers/buttons/layout_multimedia.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/handlers/buttons/layout_qwerty.py` & `rivalcfg-4.9.0/rivalcfg/handlers/buttons/layout_qwerty.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/handlers/choice.py` & `rivalcfg-4.9.0/rivalcfg/handlers/choice.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/handlers/multidpi_range.py` & `rivalcfg-4.9.0/rivalcfg/handlers/multidpi_range.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/handlers/none.py` & `rivalcfg-4.9.0/rivalcfg/handlers/none.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/handlers/range.py` & `rivalcfg-4.9.0/rivalcfg/handlers/range.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/handlers/reactive_rgbcolor.py` & `rivalcfg-4.9.0/rivalcfg/handlers/reactive_rgbcolor.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/handlers/rgbcolor.py` & `rivalcfg-4.9.0/rivalcfg/handlers/rgbcolor.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/handlers/rgbgradient.py` & `rivalcfg-4.9.0/rivalcfg/handlers/rgbgradient.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/handlers/rgbgradientv2.py` & `rivalcfg-4.9.0/rivalcfg/handlers/rgbgradientv2.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/helpers.py` & `rivalcfg-4.9.0/rivalcfg/helpers.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/mouse.py` & `rivalcfg-4.9.0/rivalcfg/mouse.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/mouse_settings.py` & `rivalcfg-4.9.0/rivalcfg/mouse_settings.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/udev.py` & `rivalcfg-4.9.0/rivalcfg/udev.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg/usbhid.py` & `rivalcfg-4.9.0/rivalcfg/usbhid.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/rivalcfg.egg-info/PKG-INFO` & `rivalcfg-4.9.0/rivalcfg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rivalcfg
-Version: 4.8.0
+Version: 4.9.0
 Summary: Configure SteelSeries gaming mice
 Home-page: https://github.com/flozz/rivalcfg
 Author: Fabien LOISON
 License: WTFPL
 Project-URL: Source Code, https://github.com/flozz/rivalcfg
 Project-URL: Documentation, https://flozz.github.io/rivalcfg/
 Project-URL: Changelog, https://github.com/flozz/rivalcfg#changelog
@@ -75,19 +75,27 @@
 | SteelSeries Aerox 3 Wireless (wired mode)                    | 1038:183a |
 +--------------------------------------------------------------+-----------+
 | SteelSeries Aerox 3 Wireless (2.4 GHz wireless mode)         | 1038:1838 |
 +--------------------------------------------------------------+-----------+
 
 SteelSeries Aerox 5 Wireless:
 
-+--------------------------------------------------------------+-----------+
-| SteelSeries Aerox 5 Wireless (wired mode)                    | 1038:1854 |
-+--------------------------------------------------------------+-----------+
-| SteelSeries Aerox 5 Wireless (2.4 GHz wireless mode)         | 1038:1852 |
-+--------------------------------------------------------------+-----------+
++------------------------------------------------------------------------+-----------+
+| SteelSeries Aerox 5 Wireless (wired mode)                              | 1038:1854 |
++------------------------------------------------------------------------+-----------+
+| SteelSeries Aerox 5 Wireless Destiny 2 Edition (wired mode)            | 1038:185e |
++------------------------------------------------------------------------+-----------+
+| SteelSeries Aerox 5 Wireless Diablo IV Edition (wired mode)            | 1038:1862 |
++------------------------------------------------------------------------+-----------+
+| SteelSeries Aerox 5 Wireless (2.4 GHz wireless mode)                   | 1038:1852 |
++------------------------------------------------------------------------+-----------+
+| SteelSeries Aerox 5 Wireless Destiny 2 Edition (2.4 GHz wireless mode) | 1038:185c |
++------------------------------------------------------------------------+-----------+
+| SteelSeries Aerox 5 Wireless Diablo IV Edition (2.4 GHz wireless mode) | 1038:1860 |
++------------------------------------------------------------------------+-----------+
 
 SteelSeries Aerox 9 Wireless:
 
 +--------------------------------------------------------------+-----------+
 | SteelSeries Aerox 9 Wireless (wired mode)                    | 1038:185a |
 +--------------------------------------------------------------+-----------+
 | SteelSeries Aerox 9 Wireless (2.4 GHz wireless mode)         | 1038:1858 |
@@ -291,15 +299,23 @@
 
 
 Changelog
 ---------
 
 * **[NEXT]** (changes on ``master`` that have not been released yet):
 
-  * Nothing yet :)
+  * Nothing yet ;)
+
+* **v4.9.0:**
+
+  * Added Aerox 5 Wireless Destiny 2 Editon support (@flozz, #205)
+  * Added Aerox 5 Wireless Diablo IV Edition support (@flozz, #206)
+  * Updated HIDAPI to v0.14 to fix a macOS Ventura issue (@flozz, #200)
+  * Removed the default lighting option for the Prime mouse (reported not
+    working and not needed on this device) (@flozz, #196)
 
 * **v4.8.0:**
 
   * Improved CLI startup time (@gryzus24, #194)
   * Added default lighting setting to following devices (@flozz, #191, #195):
 
     * Aerox 3
```

### Comparing `rivalcfg-4.8.0/rivalcfg.egg-info/SOURCES.txt` & `rivalcfg-4.9.0/rivalcfg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/setup.py` & `rivalcfg-4.9.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         long_description = open("README.rst", "r").read()
 except Exception as error:
     print("Unable to read the README file: " + str(error))
 
 
 setup(
     name="rivalcfg",
-    version="4.8.0",
+    version="4.9.0",
     description="Configure SteelSeries gaming mice",
     url="https://github.com/flozz/rivalcfg",
     project_urls={
         "Source Code": "https://github.com/flozz/rivalcfg",
         "Documentation": "https://flozz.github.io/rivalcfg/",
         "Changelog": "https://github.com/flozz/rivalcfg#changelog",
         "Issues": "https://github.com/flozz/rivalcfg/issues",
@@ -34,15 +34,15 @@
 
     keywords="steelseries rival sensei mouse",
     platforms=["Linux", "Windows"],
 
     packages=find_packages(),
 
     install_requires=[
-        "hidapi>=0.7.99.post20",
+        "hidapi>=0.14.0",
         "setuptools",
     ],
 
     extras_require={
         "dev": [
             "flake8",
             "pytest",
```

### Comparing `rivalcfg-4.8.0/test/test_devices.py` & `rivalcfg-4.9.0/test/test_devices.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/test/test_main.py` & `rivalcfg-4.9.0/test/test_main.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/test/test_mouse.py` & `rivalcfg-4.9.0/test/test_mouse.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/test/test_mouse_settings.py` & `rivalcfg-4.9.0/test/test_mouse_settings.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/test/test_udev.py` & `rivalcfg-4.9.0/test/test_udev.py`

 * *Files identical despite different names*

### Comparing `rivalcfg-4.8.0/test/test_usbhid.py` & `rivalcfg-4.9.0/test/test_usbhid.py`

 * *Files identical despite different names*

