# Comparing `tmp/home-assistant-intents-2023.4.26.tar.gz` & `tmp/home-assistant-intents-2023.5.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "home-assistant-intents-2023.4.26.tar", last modified: Wed Apr 26 14:50:58 2023, max compression
+gzip compressed data, was "home-assistant-intents-2023.5.30.tar", last modified: Tue May 30 16:41:22 2023, max compression
```

## Comparing `home-assistant-intents-2023.4.26.tar` & `home-assistant-intents-2023.5.30.tar`

### file list

```diff
@@ -1,123 +1,125 @@
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-26 14:50:58.773475 home-assistant-intents-2023.4.26/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    18657 2023-02-15 17:17:10.000000 home-assistant-intents-2023.4.26/LICENSE.md
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       72 2023-01-11 16:06:16.000000 home-assistant-intents-2023.4.26/MANIFEST.in
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      903 2023-04-26 14:50:58.773475 home-assistant-intents-2023.4.26/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      190 2023-01-12 16:56:58.000000 home-assistant-intents-2023.4.26/README.md
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-26 14:50:58.765475 home-assistant-intents-2023.4.26/home_assistant_intents/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      935 2023-04-17 16:30:47.000000 home-assistant-intents-2023.4.26/home_assistant_intents/__init__.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-26 14:50:58.765475 home-assistant-intents-2023.4.26/home_assistant_intents/data/
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-26 14:50:58.769475 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    15762 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/ar.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    54166 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/bg.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1903 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/bn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12544 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/ca.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    21247 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/cs.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    19985 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/da.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    19633 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/de-CH.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    29471 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/de.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     8325 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/el.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    56696 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/en.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14729 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/es.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2885 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/fa.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    40173 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/fi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6747 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/fr-CA.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    23581 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/fr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5245 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/gl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1373 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/gu.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16181 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/he.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1525 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/hi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    18547 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/hr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7330 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/hu.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3603 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/id.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3834 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/is.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14790 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/it.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3331 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/ka.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1197 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/kn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11801 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/lb.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11322 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/lt.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     8002 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/lv.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11714 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/ml.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1367 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/mn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4824 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/ms.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16333 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/nb.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    74600 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/nl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    28352 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/pl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7860 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/pt-br.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    13050 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/pt.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    51451 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/ro.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14961 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/ru.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11029 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/sk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3079 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/sl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4312 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/sr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11472 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/sv.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1197 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/sw.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1296 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/te.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5477 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/tr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14445 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/uk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14341 2023-04-26 14:50:55.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/ur.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12024 2023-04-26 14:50:55.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/vi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16782 2023-04-26 14:50:55.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/zh-cn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    13464 2023-04-26 14:50:55.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/zh-hk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    37672 2023-04-26 14:50:55.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/zh-tw.json
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-26 14:50:58.773475 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3727 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/ar.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4257 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/bg.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/bn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      725 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/ca.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3620 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/cs.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1479 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/da.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1696 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/de-CH.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1918 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/de.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1526 2023-04-26 14:50:53.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/el.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3236 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/en.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1608 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/es.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/fa.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5421 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/fi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1876 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/fr-CA.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1385 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/fr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1350 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/gl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/gu.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1223 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/he.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/hi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2274 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/hr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1723 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/hu.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1258 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/id.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      422 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/is.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1774 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/it.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      598 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/ka.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/kn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2574 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/lb.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2145 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/lt.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2062 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/lv.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2720 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/ml.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/mn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1368 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/ms.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2174 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/nb.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2594 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/nl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1163 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/pl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      419 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/pt-br.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1950 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/pt.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3315 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/ro.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1857 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/ru.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1548 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/sk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/sl.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1554 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/sr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2563 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/sv.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/sw.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/te.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/tr.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1681 2023-04-26 14:50:54.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/uk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1405 2023-04-26 14:50:55.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/ur.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1510 2023-04-26 14:50:55.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/vi.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2172 2023-04-26 14:50:55.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/zh-cn.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2008 2023-04-26 14:50:55.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/zh-hk.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2126 2023-04-26 14:50:55.000000 home-assistant-intents-2023.4.26/home_assistant_intents/data/light/zh-tw.json
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1572 2023-04-26 14:50:55.000000 home-assistant-intents-2023.4.26/home_assistant_intents/domains.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-26 14:50:58.765475 home-assistant-intents-2023.4.26/home_assistant_intents.egg-info/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      903 2023-04-26 14:50:58.000000 home-assistant-intents-2023.4.26/home_assistant_intents.egg-info/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5161 2023-04-26 14:50:58.000000 home-assistant-intents-2023.4.26/home_assistant_intents.egg-info/SOURCES.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-04-26 14:50:58.000000 home-assistant-intents-2023.4.26/home_assistant_intents.egg-info/dependency_links.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       23 2023-04-26 14:50:58.000000 home-assistant-intents-2023.4.26/home_assistant_intents.egg-info/top_level.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-01-12 16:57:45.000000 home-assistant-intents-2023.4.26/home_assistant_intents.egg-info/zip-safe
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      990 2023-04-26 14:50:44.000000 home-assistant-intents-2023.4.26/pyproject.toml
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-04-26 14:50:58.773475 home-assistant-intents-2023.4.26/setup.cfg
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-30 16:41:22.618410 home-assistant-intents-2023.5.30/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    18657 2023-02-15 17:17:10.000000 home-assistant-intents-2023.5.30/LICENSE.md
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       72 2023-01-11 16:06:16.000000 home-assistant-intents-2023.5.30/MANIFEST.in
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1290 2023-05-30 16:41:22.618410 home-assistant-intents-2023.5.30/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      577 2023-05-30 16:40:56.000000 home-assistant-intents-2023.5.30/README.md
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-30 16:41:22.610411 home-assistant-intents-2023.5.30/home_assistant_intents/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      935 2023-04-17 16:30:47.000000 home-assistant-intents-2023.5.30/home_assistant_intents/__init__.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-30 16:41:22.610411 home-assistant-intents-2023.5.30/home_assistant_intents/data/
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-30 16:41:22.614410 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    15762 2023-05-30 16:41:15.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/ar.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    54166 2023-05-30 16:41:15.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/bg.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1903 2023-05-30 16:41:15.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/bn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12544 2023-05-30 16:41:15.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/ca.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    21247 2023-05-30 16:41:15.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/cs.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    19985 2023-05-30 16:41:15.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/da.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    19712 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/de-CH.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    35266 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/de.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    61958 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/el.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    56864 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/en.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14986 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/es.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2885 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/fa.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    40173 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/fi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     6747 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/fr-CA.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    78566 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/fr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5245 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/gl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1373 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/gu.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16181 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/he.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1525 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/hi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    18547 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/hr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7330 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/hu.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3603 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/id.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3834 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/is.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14790 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/it.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3331 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/ka.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1197 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/kn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3160 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/ko.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11801 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/lb.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11322 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/lt.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     8002 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/lv.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11714 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/ml.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1367 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/mn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4824 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/ms.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16333 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/nb.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    74600 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/nl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    28368 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/pl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     7860 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/pt-br.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    13050 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/pt.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    51451 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/ro.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14961 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/ru.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11029 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/sk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3079 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/sl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4312 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/sr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    11472 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/sv.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1197 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/sw.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1296 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/te.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5477 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/tr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14445 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/uk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    14341 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/ur.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    12024 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/vi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    16782 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/zh-cn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    13464 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/zh-hk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    38206 2023-05-30 16:41:17.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/zh-tw.json
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-30 16:41:22.614410 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3727 2023-05-30 16:41:15.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/ar.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     4257 2023-05-30 16:41:15.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/bg.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-05-30 16:41:15.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/bn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      725 2023-05-30 16:41:15.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/ca.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3620 2023-05-30 16:41:15.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/cs.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1479 2023-05-30 16:41:15.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/da.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1696 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/de-CH.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1656 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/de.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1209 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/el.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3236 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/en.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1608 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/es.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/fa.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5421 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/fi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1876 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/fr-CA.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3063 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/fr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1350 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/gl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/gu.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1223 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/he.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/hi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2274 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/hr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1723 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/hu.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1258 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/id.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      422 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/is.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1774 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/it.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      598 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/ka.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/kn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      180 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/ko.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2574 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/lb.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2145 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/lt.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2062 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/lv.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2720 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/ml.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/mn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1368 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/ms.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2174 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/nb.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2594 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/nl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1163 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/pl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      419 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/pt-br.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1950 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/pt.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3315 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/ro.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1857 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/ru.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1548 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/sk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/sl.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1554 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/sr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2563 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/sv.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/sw.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/te.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      416 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/tr.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1681 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/uk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1405 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/ur.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1510 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/vi.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2172 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/zh-cn.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2008 2023-05-30 16:41:16.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/zh-hk.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2322 2023-05-30 16:41:17.000000 home-assistant-intents-2023.5.30/home_assistant_intents/data/light/zh-tw.json
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1600 2023-05-30 16:41:17.000000 home-assistant-intents-2023.5.30/home_assistant_intents/domains.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-05-30 16:41:22.610411 home-assistant-intents-2023.5.30/home_assistant_intents.egg-info/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1290 2023-05-30 16:41:22.000000 home-assistant-intents-2023.5.30/home_assistant_intents.egg-info/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5253 2023-05-30 16:41:22.000000 home-assistant-intents-2023.5.30/home_assistant_intents.egg-info/SOURCES.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-05-30 16:41:22.000000 home-assistant-intents-2023.5.30/home_assistant_intents.egg-info/dependency_links.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       23 2023-05-30 16:41:22.000000 home-assistant-intents-2023.5.30/home_assistant_intents.egg-info/top_level.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-05-30 16:35:50.000000 home-assistant-intents-2023.5.30/home_assistant_intents.egg-info/zip-safe
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      990 2023-05-30 16:41:12.000000 home-assistant-intents-2023.5.30/pyproject.toml
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       38 2023-05-30 16:41:22.618410 home-assistant-intents-2023.5.30/setup.cfg
```

### Comparing `home-assistant-intents-2023.4.26/LICENSE.md` & `home-assistant-intents-2023.5.30/LICENSE.md`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/__init__.py` & `home-assistant-intents-2023.5.30/home_assistant_intents/__init__.py`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/ar.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/ar.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/bg.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/bg.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/bn.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/bn.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/ca.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/ca.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/cs.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/cs.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/da.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/da.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/de-CH.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/de-CH.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9965995592948719%*

 * *Differences: {"'expansion_rules'": "{'a_y': '(a|aa|y|ii|ih)'}",*

 * * "'intents'": '{\'HassTurnOff\': {\'data\': {4: {\'sentences\': ["(Zünd|Mach|Lösch|Schalt|Schaut) '*

 * *              '[(<Liecht> |(d\'[ ]|d |de |dr |der |die |ds |s ))]<name> <ab_us>"]}}}, '*

 * *              '\'HassTurnOn\': {\'data\': {0: {\'sentences\': ["(Zünd|Mach|Schalt|Schaut) '*

 * *              '[(<Liecht> |(d\'[ ]|d |de |dr |der |die |ds |s ))]<name> [<a_y>]"]}}}}'}*

```diff
@@ -1,13 +1,13 @@
 {
     "expansion_rules": {
         "Ger\u00e4te": "([(d'[ ]|d |alli |aui )](Gr\u00e4t|Entit\u00e4te|Entit\u00e4t\u00e4))",
         "Liecht": "([(ds|s)] Liecht|[(d |d'[ ])]Lampe|[(d |d'[ ])]Lamp\u00e4)",
         "Liechter": "([(d'[ ]|d |alli |aui )]Liechter|[(d'[ ]|d |alli |aui )]Lamp\u00e4|[(d'[ ]|d |alli |aui )]Lampe|[(d'[ ]|d |alli |aui )]Lamp\u00e4ne)",
-        "a_y": "(a|y|ii|ih)",
+        "a_y": "(a|aa|y|ii|ih)",
         "ab_us": "(ab|us|uus|uis)",
         "area": "[(idr|i dr|im|ir|ide|id\u00e4|i d\u00e4|i de|i dr|i der)] {area}",
         "brightness": "{brightness}[(%| %| Prozent)]",
         "cover": "[(d'[' ']|d |alli |aui )]([Sunne]s[ch]tore|Vorhang|Vorh\u00e4ng|T\u00fcr[e]|Tor|Abdeckig[e]|F\u00e4nschter[l(a|\u00e4)de])",
         "mach": "(mach|tue|la[s])",
         "name": "[(d'[ ]|d |de |dr |der |die |ds |s )]{name}",
         "schliessen": "(tue {name} (zue|abe)|mach {name} (zue|abe)|schliess {name})",
@@ -264,15 +264,15 @@
                 },
                 {
                     "requires_context": {
                         "domain": "light"
                     },
                     "response": "light",
                     "sentences": [
-                        "(Z\u00fcnd|Mach|L\u00f6sch|Schalt|Schaut) [<Liecht>] <name> <ab_us>"
+                        "(Z\u00fcnd|Mach|L\u00f6sch|Schalt|Schaut) [(<Liecht> |(d'[ ]|d |de |dr |der |die |ds |s ))]<name> <ab_us>"
                     ],
                     "slots": {
                         "domain": "light"
                     }
                 },
                 {
                     "response": "lights_area",
@@ -312,15 +312,15 @@
             "data": [
                 {
                     "requires_context": {
                         "domain": "light"
                     },
                     "response": "light",
                     "sentences": [
-                        "(Z\u00fcnd|Mach|Schalt|Schaut) [<Liecht>] <name> [<a_y>]"
+                        "(Z\u00fcnd|Mach|Schalt|Schaut) [(<Liecht> |(d'[ ]|d |de |dr |der |die |ds |s ))]<name> [<a_y>]"
                     ],
                     "slots": {
                         "domain": "light"
                     }
                 },
                 {
                     "response": "lights_area",
```

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/de.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/de.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9573478147045855%*

 * *Differences: {"'expansion_rules'": "{'schliessen': '(schlie(ß|ss)[e|en]|zumachen|zu machen)', "*

 * *                      "'alle_abdeckungen': '<alle> "*

 * *                      "(Rollos|Abdeckungen|Rolll(a|ä)den|Jalousien|Raffstores|Markisen)', "*

 * *                      "'alle_garagen': '<alle> (Garagen|Garagentore)', 'alle_tore': '<alle> "*

 * *                      "(Tore|Garagentore)', 'alle_lichter': '(<alle>[r] <lichter>|von allen "*

 * *                      "[Lichtern|Lampen|Leuchten|Beleuchtungen]|[die] ganze Beleuchtung)', "*

 * *    […]*

```diff
@@ -1,45 +1,53 @@
 {
     "expansion_rules": {
         "abdeckung": "(das Rollo|die Rollos|die (Abdeckung|Abdeckungen)|(den|die) Rolll(a|\u00e4)den|die (Jalousie|Jalousien)|(den|die) Raffstore[s]|die (Markise|Markisen))",
         "absperren": "(zu|ab)<sperren>|verrieg(el|le)[n]",
         "aktivieren": "aktivier[e|en]",
-        "alle_abdeckungen": "alle (Rollos|Abdeckungen|Rolll(a|\u00e4)den|Jalousien|Raffstores|Markisen)",
-        "alle_garagen": "(alle Garagen|alle Garagentore)",
-        "alle_lichter": "(alle[r] <lichter>|von allen [Lichtern|Lampen|Leuchten|Beleuchtungen]|[die] ganze Beleuchtung)",
+        "alle": "(alle|s\u00e4mtliche|jede[r|s|n]|[die] (ganze|komplette)[n]) [der]",
+        "alle_abdeckungen": "<alle> (Rollos|Abdeckungen|Rolll(a|\u00e4)den|Jalousien|Raffstores|Markisen)",
+        "alle_garagen": "<alle> (Garagen|Garagentore)",
+        "alle_lichter": "(<alle>[r] <lichter>|von allen [Lichtern|Lampen|Leuchten|Beleuchtungen]|[die] ganze Beleuchtung)",
         "alle_luefter": "alle (Ventilatoren|L\u00fcfter)",
-        "alle_tore": "alle (Tore|Garagentore)",
+        "alle_tore": "<alle> (Tore|Garagentore)",
         "an": "(an|ein|auf)",
         "area": "((in|an|auf) (der|dem)|im|am) {area}",
         "auf": "(auf|hoch|rauf|nach oben)",
         "aus": "(aus|ab|zu)",
         "ausfuehren": "(start[e|en]|ausf\u00fchren)",
         "batterie": "[die|der|des] (Batterie[n]|Akku[s])",
         "brightness": "{brightness} [Prozent|%]",
+        "co": "Kohlen[stoff]monoxid",
+        "co-sensor": "<co>[-]Sensor[en]",
         "deaktivieren": "de<aktivieren>",
+        "ding": "((Ding|Ger\u00e4t)[e]|Sensor[en]|Gegenstand|Gegenst\u00e4nde)",
         "entsperren": "((ent|auf)<sperren>|\u00f6ffne|entrieg(el|le))[n]",
+        "etwas": "[irgend][et]was",
         "garage": "(die Garage|die Garagen|das Garagentor|die Garagentore)",
-        "irgend": "(irgend(ein[e][s]|welche)|einige)",
+        "irgend": "(irgend(ein[e][s|r]|welche[s])|einige[s]) [der]",
         "ladestand": "[der] [Lade][zu]Stand",
         "licht": "([das] Licht|[die] Lampe|[die] Beleuchtung)",
         "lichter": "[die|der|von den] (Lichter|Lichtern|Lampen|Leuchten|Beleuchtungen)",
         "luefter": "(den Ventilator|die Ventilatoren|(den|die) L\u00fcfter)",
         "machen": "(mach[e|en])",
         "name": "[(der|den|dem|die|das)] {name}",
-        "schliessen": "(schlie(\u00df|ss)|schlie(\u00df|ss)e|zumachen|zu machen)",
+        "schalten": "(schalt[e|en])",
+        "schliessen": "(schlie(\u00df|ss)[e|en]|zumachen|zu machen)",
         "schloss": "[das|die] (Schloss|Schl\u00f6sser)",
         "setzen": "(setz[e|en]|stell[e|en]|einstellen|\u00e4nder[e|n]|ver\u00e4nder[e|n])",
         "skript": "[das] Skript",
         "sperren": "(sperr|schlie(ss|\u00df))[e|en]",
         "szene": "[die] Szene",
         "temperature": "{temperature} [Grad] [{temperature_unit}]",
         "tor": "(das Tor|die Tore)",
         "tuer": "[die] T\u00fcr[e|en]",
         "von_dem": "(von [dem]|vom)",
-        "zu": "(zu|[he]runter|nach unten)"
+        "welche": "(welche[r|s]|was f\u00fcr [ein[e][r|s]]) [der]",
+        "zu": "(zu|[he]runter|nach unten)",
+        "\u00f6ffnen": "(\u00f6ffne[n]|aufmachen|auf machen)"
     },
     "intents": {
         "HassGetState": {
             "data": [
                 {
                     "requires_context": {
                         "device_class": "battery",
@@ -64,25 +72,25 @@
                         "device_class": "battery",
                         "domain": "binary_sensor"
                     }
                 },
                 {
                     "response": "alle",
                     "sentences": [
-                        "sind alle <batterie> [<area>] {bs_battery_states:state}"
+                        "sind <alle> <batterie> [<area>] {bs_battery_states:state}"
                     ],
                     "slots": {
                         "device_class": "battery",
                         "domain": "binary_sensor"
                     }
                 },
                 {
                     "response": "welches",
                     "sentences": [
-                        "(welche[r]) <batterie> [<area>] (ist|sind) {bs_battery_states:state}"
+                        "<welche> <batterie> [<area>] (ist|sind) {bs_battery_states:state}"
                     ],
                     "slots": {
                         "device_class": "battery",
                         "domain": "binary_sensor"
                     }
                 },
                 {
@@ -120,43 +128,180 @@
                         "device_class": "battery_charging",
                         "domain": "binary_sensor"
                     }
                 },
                 {
                     "response": "alle",
                     "sentences": [
-                        "werden alle <batterie> [<area>] {bs_battery_charging_states:state}",
-                        "{bs_battery_charging_states:state} alle <batterie> [<area>] [auf]"
+                        "werden <alle> <batterie> [<area>] {bs_battery_charging_states:state}",
+                        "{bs_battery_charging_states:state} <alle> <batterie> [<area>] [auf]"
                     ],
                     "slots": {
                         "device_class": "battery_charging",
                         "domain": "binary_sensor"
                     }
                 },
                 {
                     "response": "welches",
                     "sentences": [
-                        "(welche[r]) <batterie> [<area>] [wird|werden] {bs_battery_charging_states:state}"
+                        "<welche> <batterie> [<area>] [wird|werden] {bs_battery_charging_states:state}"
                     ],
                     "slots": {
                         "device_class": "battery_charging",
                         "domain": "binary_sensor"
                     }
                 },
                 {
                     "response": "wie_viele",
                     "sentences": [
-                        "wie viele <batterie> [<area>] [wird|werden] {bs_battery_charging_states:state}"
+                        "wie viele <batterie> [<area>] [werden] {bs_battery_charging_states:state}"
                     ],
                     "slots": {
                         "device_class": "battery_charging",
                         "domain": "binary_sensor"
                     }
                 },
                 {
+                    "requires_context": {
+                        "device_class": "carbon_monoxide",
+                        "domain": "binary_sensor"
+                    },
+                    "response": "einzeln_janein",
+                    "sentences": [
+                        "(ist|wurde) <name> [<area>] {bs_carbon_monoxide_states:state}"
+                    ],
+                    "slots": {
+                        "device_class": "carbon_monoxide",
+                        "domain": "binary_sensor"
+                    }
+                },
+                {
+                    "response": "irgendeins",
+                    "sentences": [
+                        "(ist|sind|wurde[n]) <irgend> <co-sensor> [<area>] {bs_carbon_monoxide_states:state}"
+                    ],
+                    "slots": {
+                        "device_class": "carbon_monoxide",
+                        "domain": "binary_sensor"
+                    }
+                },
+                {
+                    "response": "irgendeins",
+                    "sentences": [
+                        "(gibt es|ist) [<irgend>] <co> <area>",
+                        "(wird|wurde) [<irgend>] <co> <area> {bs_carbon_monoxide_states:state}"
+                    ],
+                    "slots": {
+                        "device_class": "carbon_monoxide",
+                        "domain": "binary_sensor",
+                        "state": "on"
+                    }
+                },
+                {
+                    "response": "alle",
+                    "sentences": [
+                        "(sind|wurden) <alle> <co-sensor> [<area>] {bs_carbon_monoxide_states:state}"
+                    ],
+                    "slots": {
+                        "device_class": "carbon_monoxide",
+                        "domain": "binary_sensor"
+                    }
+                },
+                {
+                    "response": "welches",
+                    "sentences": [
+                        "<welche> <co-sensor> (ist|sind|wurde[n]) [<area>] {bs_carbon_monoxide_states:state}"
+                    ],
+                    "slots": {
+                        "device_class": "carbon_monoxide",
+                        "domain": "binary_sensor"
+                    }
+                },
+                {
+                    "response": "wie_viele",
+                    "sentences": [
+                        "wie viele <co-sensor> (sind|wurden) [<area>] {bs_carbon_monoxide_states:state}"
+                    ],
+                    "slots": {
+                        "device_class": "carbon_monoxide",
+                        "domain": "binary_sensor"
+                    }
+                },
+                {
+                    "requires_context": {
+                        "device_class": "cold",
+                        "domain": "binary_sensor"
+                    },
+                    "response": "einzeln_janein",
+                    "sentences": [
+                        "ist <name> [<area>] {bs_cold_states:state}",
+                        "ist <area> <name> {bs_cold_states:state}",
+                        "ist <name> {bs_cold_states:state} <area>"
+                    ],
+                    "slots": {
+                        "device_class": "cold",
+                        "domain": "binary_sensor"
+                    }
+                },
+                {
+                    "response": "irgendeins",
+                    "sentences": [
+                        "(ist|sind) [<irgend>] <ding> [<area>] kalt",
+                        "(ist|sind) [<irgend>] <ding> kalt <area>",
+                        "(ist|sind) <area> [<irgend>] <ding> kalt",
+                        "ist <etwas> [<area>] kalt",
+                        "ist <etwas> kalt <area>",
+                        "ist <area> <etwas> kalt"
+                    ],
+                    "slots": {
+                        "device_class": "cold",
+                        "domain": "binary_sensor",
+                        "state": "on"
+                    }
+                },
+                {
+                    "response": "alle",
+                    "sentences": [
+                        "sind <alle> <ding> [<area>] kalt",
+                        "sind <alle> <ding> kalt <area>",
+                        "sind <area> <alle> <ding> kalt"
+                    ],
+                    "slots": {
+                        "device_class": "cold",
+                        "domain": "binary_sensor",
+                        "state": "on"
+                    }
+                },
+                {
+                    "response": "welches",
+                    "sentences": [
+                        "<welche> <ding> (ist|sind) [<area>] kalt",
+                        "<welche> <ding> (ist|sind) kalt <area>",
+                        "<welche> <ding> <area> (ist|sind) kalt"
+                    ],
+                    "slots": {
+                        "device_class": "cold",
+                        "domain": "binary_sensor",
+                        "state": "on"
+                    }
+                },
+                {
+                    "response": "wie_viele",
+                    "sentences": [
+                        "wie viele <ding> sind [<area>] kalt",
+                        "wie viele <ding> sind kalt <area>",
+                        "wie viele <ding> <area> sind kalt"
+                    ],
+                    "slots": {
+                        "device_class": "cold",
+                        "domain": "binary_sensor",
+                        "state": "on"
+                    }
+                },
+                {
                     "excludes_context": {
                         "domain": [
                             "scene",
                             "script"
                         ]
                     },
                     "response": "einzeln",
@@ -281,39 +426,39 @@
                     "slots": {
                         "domain": "lock"
                     }
                 },
                 {
                     "response": "irgendeins",
                     "sentences": [
-                        "sind [irgendwelche|einige] {lock_domains:domain} {lock_states:state} [<area>]",
-                        "sind [irgendwelche|einige] {lock_domains:domain} [<area>] {lock_states:state}",
-                        "sind [<area>] [irgendwelche|einige] {lock_domains:domain} {lock_states:state}"
+                        "(ist|sind) [<irgend>] {lock_domains:domain} {lock_states:state} [<area>]",
+                        "(ist|sind) [<irgend>] {lock_domains:domain} [<area>] {lock_states:state}",
+                        "(ist|sind) [<area>] [<irgend>] {lock_domains:domain} {lock_states:state}"
                     ],
                     "slots": {
                         "domain": "lock"
                     }
                 },
                 {
                     "response": "alle",
                     "sentences": [
-                        "(sind alle|ist jede[(r|s)]) {lock_domains:domain} {lock_states:state} [<area>]",
-                        "(sind alle|ist jede[(r|s)]) {lock_domains:domain} [<area>] {lock_states:state}",
-                        "(sind|ist) [<area>] (alle|jede[(r|s)]) {lock_domains:domain} {lock_states:state}"
+                        "(sind|ist) <alle> {lock_domains:domain} {lock_states:state} [<area>]",
+                        "(sind|ist) <alle> {lock_domains:domain} [<area>] {lock_states:state}",
+                        "(sind|ist) [<area>] <alle> {lock_domains:domain} {lock_states:state}"
                     ],
                     "slots": {
                         "domain": "lock"
                     }
                 },
                 {
                     "response": "welches",
                     "sentences": [
-                        "welche[(r|s)] {lock_domains:domain} (ist|sind) {lock_states:state} [<area>]",
-                        "welche[(r|s)] {lock_domains:domain} (ist|sind) [<area>] {lock_states:state}",
-                        "welche[(r|s)] {lock_domains:domain} [<area>] (ist|sind) {lock_states:state}"
+                        "<welche> {lock_domains:domain} (ist|sind) {lock_states:state} [<area>]",
+                        "<welche> {lock_domains:domain} (ist|sind) [<area>] {lock_states:state}",
+                        "<welche> {lock_domains:domain} [<area>] (ist|sind) {lock_states:state}"
                     ],
                     "slots": {
                         "domain": "lock"
                     }
                 },
                 {
                     "response": "wie_viele",
@@ -327,14 +472,15 @@
                     }
                 }
             ]
         },
         "HassTurnOff": {
             "data": [
                 {
+                    "response": "fan_all",
                     "sentences": [
                         "schalte <luefter> <area> <aus>",
                         "schalte <area> <luefter> <aus>",
                         "stoppe <luefter> <area> [<aus>]",
                         "stoppe <area> <luefter> [<aus>]",
                         "(mach|mache) <luefter> <area> <aus>",
                         "(mach|mache) <area> <luefter> <aus>",
@@ -349,53 +495,71 @@
                         "domain": "fan",
                         "name": "all"
                     }
                 },
                 {
                     "excludes_context": {
                         "domain": [
+                            "binary_sensor",
                             "cover",
                             "lock",
                             "scene",
-                            "script"
+                            "script",
+                            "sensor"
                         ]
                     },
                     "sentences": [
-                        "schalte <name> <aus>",
+                        "(<schalten>|<machen>) <name> <aus>",
                         "stoppe <name>",
                         "<deaktivieren> <name>",
                         "<name> <deaktivieren>",
-                        "<name> <aus>[schalten]"
+                        "<name> <aus>[<schalten>|<machen>]"
                     ]
                 },
                 {
+                    "response": "light",
                     "sentences": [
-                        "Schalte (<licht>|<lichter>) <area> <aus>",
-                        "Schalte <area> (<licht>|<lichter>) <aus>",
-                        "(<licht>|<lichter>) <area> <aus>schalten",
-                        "<area> (<licht>|<lichter>) <aus>schalten",
+                        "<schalten> (<licht>|<lichter>) <area> <aus>",
+                        "<schalten> <area> (<licht>|<lichter>) <aus>",
+                        "(<licht>|<lichter>) <area> <aus>[<schalten>]",
+                        "<area> (<licht>|<lichter>) <aus>[<schalten>]",
                         "<machen> (<licht>|<lichter>) <area> <aus>",
                         "<machen> <area> (<licht>|<lichter>) <aus>",
                         "(<licht>|<lichter>) <area> <aus><machen>",
                         "<area> (<licht>|<lichter>) <aus><machen>",
-                        "Schalte [<lichter>|<alle_lichter>] [<area>] <aus>",
-                        "Schalte [<area>] [<lichter>|<alle_lichter>] <aus>",
-                        "[<lichter>|<alle_lichter>] [<area>] <aus>schalten",
-                        "[<area>] [<lichter>|<alle_lichter>] <aus>schalten",
+                        "<schalten> [<lichter>|<alle_lichter>] [<area>] <aus>",
+                        "<schalten> [<area>] [<lichter>|<alle_lichter>] <aus>",
+                        "[<lichter>|<alle_lichter>] [<area>] <aus>[<schalten>]",
+                        "[<area>] [<lichter>|<alle_lichter>] <aus>[<schalten>]",
                         "<machen> [<lichter>|<alle_lichter>] [<area>] <aus>",
                         "<machen> [<area>] [<lichter>|<alle_lichter>] <aus>",
                         "[<lichter>|<alle_lichter>] [<area>] <aus><machen>",
                         "<machen> [<area>] [<lichter>|<alle_lichter>] <aus><machen>"
                     ],
                     "slots": {
                         "domain": "light"
                     }
                 },
                 {
-                    "response": "cover_area",
+                    "requires_context": {
+                        "domain": "cover"
+                    },
+                    "response": "cover",
+                    "sentences": [
+                        "<schliessen> <name>",
+                        "<name> <schliessen>",
+                        "<machen> <name> <zu>",
+                        "<name> <zu>[<machen>]"
+                    ],
+                    "slots": {
+                        "domain": "cover"
+                    }
+                },
+                {
+                    "response": "cover",
                     "sentences": [
                         "<schliessen> <area> (<abdeckung>|<tor>|<garage>)",
                         "<schliessen> (<abdeckung>|<tor>|<garage>) <area>",
                         "<machen> <area> (<abdeckung>|<tor>|<garage>) <zu>",
                         "<machen> (<abdeckung>|<tor>|<garage>) <area> <zu>"
                     ],
                     "slots": {
@@ -431,20 +595,20 @@
                 {
                     "requires_context": {
                         "domain": "lock",
                         "name": "all"
                     },
                     "response": "lock",
                     "sentences": [
-                        "<entsperren> [alle] (<tuer>|<schloss>) <area>",
-                        "<entsperren> <area> [alle] (<tuer>|<schloss>)",
-                        "(<sperren>|<machen>) [alle] (<tuer>|<schloss>) <area> auf",
-                        "(<sperren>|<machen>) <area> [alle] (<tuer>|<schloss>) auf",
-                        "[alle] (<tuer>|<schloss>) <area> (auf[machen]|<entsperren>)",
-                        "<area> [alle] (<tuer>|<schloss>) (auf[machen]|<entsperren>)"
+                        "<entsperren> [<alle>] (<tuer>|<schloss>) <area>",
+                        "<entsperren> <area> [<alle>] (<tuer>|<schloss>)",
+                        "(<sperren>|<machen>) [<alle>] (<tuer>|<schloss>) <area> auf",
+                        "(<sperren>|<machen>) <area> [<alle>] (<tuer>|<schloss>) auf",
+                        "[<alle>] (<tuer>|<schloss>) <area> (auf[machen]|<entsperren>)",
+                        "<area> [<alle>] (<tuer>|<schloss>) (auf[machen]|<entsperren>)"
                     ]
                 }
             ]
         },
         "HassTurnOn": {
             "data": [
                 {
@@ -461,65 +625,82 @@
                         "<aktivieren> <name> <szene>"
                     ],
                     "slots": {
                         "domain": "scene"
                     }
                 },
                 {
+                    "response": "light",
                     "sentences": [
-                        "Schalte (<licht>|<lichter>) <area> <an>",
-                        "Schalte <area> (<licht>|<lichter>) <an>",
-                        "(<licht>|<lichter>) <area> <an>schalten",
-                        "<area> (<licht>|<lichter>) <an>schalten",
+                        "<schalten> (<licht>|<lichter>) <area> <an>",
+                        "<schalten> <area> (<licht>|<lichter>) <an>",
+                        "(<licht>|<lichter>) <area> <an>[<schalten>]",
+                        "<area> (<licht>|<lichter>) <an>[<schalten>]",
                         "<machen> <area> (<licht>|<lichter>) <an>",
                         "<machen> (<licht>|<lichter>) <area> <an>",
                         "<area> (<licht>|<lichter>) <an><machen>",
                         "(<licht>|<lichter>) <area> <an><machen>",
-                        "Schalte [<lichter>|<alle_lichter>] [<area>] <an>",
-                        "Schalte [<area>] [<lichter>|<alle_lichter>] <an>",
-                        "[<lichter>|<alle_lichter>] [<area>] <an>schalten",
-                        "[<area>] [<lichter>|<alle_lichter>] <an>schalten",
+                        "<schalten> [<lichter>|<alle_lichter>] [<area>] <an>",
+                        "<schalten> [<area>] [<lichter>|<alle_lichter>] <an>",
+                        "[<lichter>|<alle_lichter>] [<area>] <an>[<schalten>]",
+                        "[<area>] [<lichter>|<alle_lichter>] <an>[<schalten>]",
                         "<machen> [<area>] [<lichter>|<alle_lichter>] <an>",
                         "<machen> [<lichter>|<alle_lichter>] [<area>] <an>",
                         "[<area>] [<lichter>|<alle_lichter>] <an><machen>",
                         "[<lichter>|<alle_lichter>] [<area>] <an><machen>"
                     ],
                     "slots": {
                         "domain": "light"
                     }
                 },
                 {
-                    "response": "cover_area",
+                    "requires_context": {
+                        "domain": "cover"
+                    },
+                    "response": "cover",
+                    "sentences": [
+                        "<\u00f6ffnen> <name>",
+                        "<name> <\u00f6ffnen>",
+                        "<machen> <name> <auf>",
+                        "<name> <auf>[<machen>]"
+                    ],
+                    "slots": {
+                        "domain": "cover"
+                    }
+                },
+                {
+                    "response": "cover",
                     "sentences": [
-                        "\u00f6ffne <area> (<abdeckung>|<tor>|<garage>)",
-                        "\u00f6ffne (<abdeckung>|<tor>|<garage>) <area>",
+                        "<\u00f6ffnen> <area> (<abdeckung>|<tor>|<garage>)",
+                        "<\u00f6ffnen> (<abdeckung>|<tor>|<garage>) <area>",
                         "<machen> <area> (<abdeckung>|<tor>|<garage>) <auf>",
                         "<machen> (<abdeckung>|<tor>|<garage>) <area> <auf>"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
                     "response": "open_all",
                     "sentences": [
-                        "\u00f6ffne <area> (<alle_tore>|<alle_garagen>)",
-                        "\u00f6ffne (<alle_tore>|<alle_garagen>) <area>",
+                        "<\u00f6ffnen> <area> (<alle_tore>|<alle_garagen>)",
+                        "<\u00f6ffnen> (<alle_tore>|<alle_garagen>) <area>",
                         "<machen> <area> (<alle_tore>|<alle_garagen>) <auf>",
                         "<machen> (<alle_tore>|<alle_garagen>) <area> <auf>",
-                        "\u00f6ffne [<area>] (<alle_abdeckungen>|<alle_tore>|<alle_garagen>)",
-                        "\u00f6ffne (<alle_abdeckungen>|<alle_tore>|<alle_garagen>) [<area>]",
+                        "<\u00f6ffnen> [<area>] (<alle_abdeckungen>|<alle_tore>|<alle_garagen>)",
+                        "<\u00f6ffnen> (<alle_abdeckungen>|<alle_tore>|<alle_garagen>) [<area>]",
                         "<machen> [<area>] (<alle_abdeckungen>|<alle_tore>|<alle_garagen>) <auf>",
                         "<machen> (<alle_abdeckungen>|<alle_tore>|<alle_garagen>) [<area>] <auf>"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
+                    "response": "fan_all",
                     "sentences": [
                         "schalte <luefter> <area> <an>",
                         "schalte <area> <luefter> <an>",
                         "starte <luefter> <area> [<an>]",
                         "starte <area> <luefter> [<an>]",
                         "(mach|mache) <luefter> <area> <an>",
                         "(mach|mache) <area> <luefter> <an>",
@@ -552,20 +733,20 @@
                 {
                     "requires_context": {
                         "domain": "lock",
                         "name": "all"
                     },
                     "response": "lock",
                     "sentences": [
-                        "(<sperren>|<machen>) [alle] (<tuer>|<schloss>) <area> [zu|ab]",
-                        "(<sperren>|<machen>) <area> [alle] (<tuer>|<schloss>) [zu|ab]",
-                        "[alle] (<tuer>|<schloss>) <area> (zu[machen]|<absperren>)",
-                        "<area> [alle] (<tuer>|<schloss>) (zu[machen]|<absperren>)",
-                        "<absperren> [alle] (<tuer>|<schloss>) <area>",
-                        "<absperren> <area> [alle] (<tuer>|<schloss>)"
+                        "(<sperren>|<machen>) [<alle>] (<tuer>|<schloss>) <area> [zu|ab]",
+                        "(<sperren>|<machen>) <area> [<alle>] (<tuer>|<schloss>) [zu|ab]",
+                        "[<alle>] (<tuer>|<schloss>) <area> (zu[machen]|<absperren>)",
+                        "<area> [<alle>] (<tuer>|<schloss>) (zu[machen]|<absperren>)",
+                        "<absperren> [<alle>] (<tuer>|<schloss>) <area>",
+                        "<absperren> <area> [<alle>] (<tuer>|<schloss>)"
                     ]
                 },
                 {
                     "requires_context": {
                         "domain": "script"
                     },
                     "response": "script",
@@ -580,26 +761,28 @@
                     "slots": {
                         "domain": "script"
                     }
                 },
                 {
                     "excludes_context": {
                         "domain": [
+                            "binary_sensor",
                             "cover",
                             "lock",
                             "scene",
-                            "script"
+                            "script",
+                            "sensor"
                         ]
                     },
                     "sentences": [
-                        "schalte <name> <an>",
+                        "(<schalten>|<machen>) <name> <an>",
                         "starte <name>",
                         "<aktivieren> <name>",
                         "<name> <aktivieren>",
-                        "<name> <an>[schalten]"
+                        "<name> <an>[<schalten>|<machen>]"
                     ]
                 }
             ]
         }
     },
     "language": "de",
     "lists": {
@@ -630,14 +813,38 @@
                 },
                 {
                     "in": "normal",
                     "out": "off"
                 }
             ]
         },
+        "bs_carbon_monoxide_states": {
+            "values": [
+                {
+                    "in": "(entdeckt|ausgel\u00f6st|erkannt|an)",
+                    "out": "on"
+                },
+                {
+                    "in": "(klar|rein|sauber|sicher)",
+                    "out": "off"
+                }
+            ]
+        },
+        "bs_cold_states": {
+            "values": [
+                {
+                    "in": "kalt",
+                    "out": "on"
+                },
+                {
+                    "in": "normal",
+                    "out": "off"
+                }
+            ]
+        },
         "color": {
             "values": [
                 {
                     "in": "wei(\u00df|ss)",
                     "out": "white"
                 },
                 {
@@ -818,27 +1025,25 @@
                 "einzeln_janein": "{% if query.matched %}\n  Ja\n{% else %}\n  Nein\n{% endif %}\n",
                 "irgendeins": "{% if query.matched %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length > 4 %}\n    Ja, {{ match[:3] | join(\", \") }} und {{ (match | length - 3) }} weitere\n  {%- else -%}\n    Ja,\n    {% for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} und {% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% else %}\n  Nein\n{% endif %}\n",
                 "welches": "{% if not query.matched %}\n  Keins\n{% else: %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length > 4 %}\n    {{ match[:3] | join(\", \") }} und {{ (match | length - 3) }} weitere\n  {% else %}\n    {%- for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} und {% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% endif %}\n",
                 "wie_viele": "{{ query.matched | length }}\n"
             },
             "HassTurnOff": {
                 "close_all": "alle geschlossen",
-                "cover": "{{ slots.name }} geschlossen",
-                "cover_area": "{{ slots.area }} geschlossen",
+                "cover": "geschlossen",
                 "default": "{{ slots.name }} ausgeschaltet",
-                "fans_area": "Die Ventilatoren in {{ slots.area }} sind ausgeschaltet",
-                "lights_area": "Die Lampen in {{ slots.area }} sind ausgeschaltet",
+                "fan_all": "Die Ventilatoren sind ausgeschaltet",
+                "light": "Licht ausgeschaltet",
                 "lock": "entsperrt"
             },
             "HassTurnOn": {
-                "cover": "{{ slots.name }} ge\u00f6ffnet",
-                "cover_area": "{{ slots.area }} ge\u00f6ffnet",
+                "cover": "ge\u00f6ffnet",
                 "default": "{{ slots.name }} eingeschaltet",
-                "fans_area": "Die Ventilatoren in {{ slots.area }} sind eingeschaltet",
-                "lights_area": "Die Lampen in {{ slots.area }} sind eingeschaltet",
+                "fan_all": "Die Ventilatoren sind eingeschaltet",
+                "light": "Licht eingeschaltet",
                 "lock": "abgeschlossen",
                 "open_all": "alle ge\u00f6ffnet",
                 "scene": "{{ slots.name }} aktiviert",
                 "script": "{{ slots.name }} gestartet"
             }
         }
     },
```

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/en.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/en.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9965044429510156%*

 * *Differences: {"'expansion_rules'": "{'set': '(set|make|change|turn)'}",*

 * * "'intents'": "{'HassGetState': {'data': {108: {'sentences': ['(do you know|tell me|<what_is>) "*

 * *              "[the [current] (state|value) of] <name> [in <area>]']}, 111: {'sentences': ['are "*

 * *              'all [the] {on_off_domains:domain} [(switched|turned|set[ to])] '*

 * *              "{on_off_states:state} [in <area>]', 'are all [the] {on_off_domains:domain} in "*

 * *              "<area> [(switched|turned|set[ to])] {on_off_states:state}']}}}}"}*

```diff
@@ -3,15 +3,15 @@
         "area": "[the] {area}",
         "brightness": "{brightness}[ ][%|percent]",
         "close": "(close|shut|lower)",
         "light": "[the] (light|lights|lighting)",
         "name": "[the] {name}",
         "numeric_value_set": "(set|change|turn|increase|decrease|make)",
         "open": "(open | raise)",
-        "set": "(set|change|turn)",
+        "set": "(set|make|change|turn)",
         "temp": "(temp|temperature)",
         "temperature": "{temperature}[ ][\u00b0|degrees][ ][{temperature_unit}]",
         "turn": "(turn|switch|change)",
         "what_is": "(what's|whats|what is)"
     },
     "intents": {
         "HassGetState": {
@@ -1237,15 +1237,15 @@
                         "domain": [
                             "scene",
                             "script"
                         ]
                     },
                     "response": "one",
                     "sentences": [
-                        "(do you know|tell me|what is) [the state of] <name> [in <area>]"
+                        "(do you know|tell me|<what_is>) [the [current] (state|value) of] <name> [in <area>]"
                     ]
                 },
                 {
                     "excludes_context": {
                         "domain": [
                             "cover"
                         ]
@@ -1261,15 +1261,16 @@
                         "(is|are) [there] any {on_off_domains:domain} {on_off_states:state} [in <area>]",
                         "(do you know|tell me) if there are any {on_off_domains:domain} {on_off_states:state} [in <area>]"
                     ]
                 },
                 {
                     "response": "all",
                     "sentences": [
-                        "are all [the] {on_off_domains:domain} {on_off_states:state} [in <area>]"
+                        "are all [the] {on_off_domains:domain} [(switched|turned|set[ to])] {on_off_states:state} [in <area>]",
+                        "are all [the] {on_off_domains:domain} in <area> [(switched|turned|set[ to])] {on_off_states:state}"
                     ]
                 },
                 {
                     "response": "which",
                     "sentences": [
                         "[do you know] (which|what) {on_off_domains:domain} (is|are) {on_off_states:state} [in <area>]"
                     ]
```

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/es.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/es.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9561743233618234%*

 * *Differences: {"'expansion_rules'": "{'abre': '(abre|abra|abrir|abrí|sube|suba|subir|subí)', 'apaga': "*

 * *                      "'(apaga|apague|apagar|apagá|desconecta|desconecte|desconectar|desconectá|desactiva|desactive|desactivar|desactivá)', "*

 * *                      "'cierra': '(cierra|cierre|cerrar|cerrá|baja|baje|bajar|bajá)', 'enciende': "*

 * *                      "'(enciende|encienda|encender|encendé|conecta|conecte|conectar|conectá|activa|active|activar|activá|prende|prenda|prender|prendé)', "*

 * *                      "' […]*

```diff
@@ -1,19 +1,19 @@
 {
     "expansion_rules": {
-        "abre": "(abre|abra|abrir|sube|suba|subir)",
-        "apaga": "(apaga|apague|apagar|desconecta|desconecte|desconectar|desactiva|desactive|desactivar)",
+        "abre": "(abre|abra|abrir|abr\u00ed|sube|suba|subir|sub\u00ed)",
+        "apaga": "(apaga|apague|apagar|apag\u00e1|desconecta|desconecte|desconectar|desconect\u00e1|desactiva|desactive|desactivar|desactiv\u00e1)",
         "area": "[en|en el|en la|la|de la|del|de|el] {area}",
         "brightness": "{brightness}[ ][%|porciento|por ciento]",
-        "cierra": "(cierra|cierre|cerrar|baja|baje|bajar)",
-        "enciende": "(enciende|encienda|encender|conecta|conecte|conectar|activa|active|activar|prende|prenda|prender)",
-        "establece": "(pon|ponga|poner|establece|establezca|establecer|ajusta|ajuste|ajustar|configura|configure|configurar)",
-        "establece_sube_baja": "(pon|ponga|poner|establece|establezca|establecer|ajusta|ajuste|ajustar|configura|configure|configurar|sube|suba|subir|baja|baje|bajar)",
+        "cierra": "(cierra|cierre|cerrar|cerr\u00e1|baja|baje|bajar|baj\u00e1)",
+        "enciende": "(enciende|encienda|encender|encend\u00e9|conecta|conecte|conectar|conect\u00e1|activa|active|activar|activ\u00e1|prende|prenda|prender|prend\u00e9)",
+        "establece": "(pon|ponga|poner|pon\u00e9|establece|establezca|establecer|establec\u00e9|ajusta|ajuste|ajustar|ajust\u00e1|configura|configure|configurar|configur\u00e1)",
+        "establece_sube_baja": "(pon|ponga|poner|pon\u00e9|establece|establezca|establecer|establec\u00e9|ajusta|ajuste|ajustar|ajust\u00e1|configura|configure|configurar|configur\u00e1|sube|suba|subir|sub\u00ed|baja|baje|bajar|baj\u00e1)",
         "name": "[el|la] {name}",
-        "puerta": "[el|la] (puerta|port\u00f3n|cancela|verja|reja|compuerta)",
+        "puerta": "[el|la] (puerta|port\u00f3n|cancela|verja|reja|compuerta|portillo)",
         "temp": "[el|la] (temperatura|calor|grados)",
         "temperature": "{temperature}[ ][grados][ ][{temperature_unit}]"
     },
     "intents": {
         "HassGetState": {
             "data": [
                 {
@@ -286,15 +286,15 @@
                     "out": "black"
                 },
                 {
                     "in": "rojo",
                     "out": "red"
                 },
                 {
-                    "in": "naranja",
+                    "in": "(naranja|anaranjado)",
                     "out": "orange"
                 },
                 {
                     "in": "amarillo",
                     "out": "yellow"
                 },
                 {
@@ -382,15 +382,15 @@
                     "out": "light"
                 },
                 {
                     "in": "ventilador[es]",
                     "out": "fan"
                 },
                 {
-                    "in": "interruptor[es]",
+                    "in": "interruptor[es]|llave[s]",
                     "out": "switch"
                 }
             ]
         },
         "on_off_states": {
             "values": [
                 {
@@ -468,13 +468,16 @@
     "skip_words": [
         "por favor",
         "porfa",
         "gracias",
         "podr\u00edas",
         "podr\u00eda",
         "puedes",
+        "pod\u00e9s",
         "te importar\u00eda",
         "te importa",
         "le importa",
-        "le importar\u00eda"
+        "le importar\u00eda",
+        "te animas a",
+        "te anim\u00e1s a"
     ]
 }
```

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/fa.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/fa.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/fi.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/fi.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/fr-CA.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/fr-CA.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/fr.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/pl.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6910408026224912%*

 * *Differences: {"'expansion_rules'": "{'name': '{name}', 'area': '[w|na] {area}', 'brightness': '{brightness}[%| "*

 * *                      "procent]', 'temperature': '{temperature}[°| stopni] [{temperature_unit}]', "*

 * *                      "'set': '(ustaw|zmień|przestaw|nastaw)', 'what_is': 'Jak[a|i] jest', 'all': "*

 * *                      "'(wszystkie|każde)', 'how_many_is': 'Ile jest', 'activate': "*

 * *                      "'(aktywuj|uaktywnij|rozpocznij|zacznij|uruchom)', 'lock': 'zablokuj', "*

 * *                      "'unlock': […]*

```diff
@@ -1,789 +1,920 @@
 {
     "expansion_rules": {
-        "allume": "(allume|allumer|active|activer|d\u00e9marre|d\u00e9marrer)",
-        "area": "[le |la |[l']]{area}",
-        "brightness": "{brightness:brightness}[%| pourcent]",
-        "dans": "(dans|du|de)",
-        "eteins": "(\u00e9teint|\u00e9teins|\u00e9teindre|d\u00e9sactive|d\u00e9sactiver|stoppe|stopper|arr\u00eate|arr\u00eater|coupe|couper)",
-        "ferme": "(ferme|fermer|baisse|baisser) ",
-        "garage": "([la ]porte (du |de )garage)|([le ]garage)",
-        "lumiere": "([la ](lumi\u00e8re|lampe)|[l']ampoule)",
-        "lumieres": "[les ](lumi\u00e8res|lampes|ampoules)",
-        "name": "[le |la |les |[l']]{name}",
-        "ouvre": "(ouvre|ouvrir|monte|monter)",
-        "regle": "(r\u00e8gle|r\u00e9gler|met|mets|mettre|ajuste|ajuster|change|changer)",
-        "temperature": "{temperature}[\u00b0| degr\u00e9s] [{temperature_unit}]",
-        "ventilateur": "[le ](ventilateur|brasseur d'air)",
-        "ventilateurs": "[les ](ventilateurs|brasseurs d'air)",
-        "volet": "([le ](volet|store))",
-        "volets": "[les ](volets|stores)",
-        "yatil": "(y a-t-il|il y a|y a t il|y a t'il|y a-t'il)"
+        "activate": "(aktywuj|uaktywnij|rozpocznij|zacznij|uruchom)",
+        "all": "(wszystkie|ka\u017cde)",
+        "area": "[w|na] {area}",
+        "brightness": "{brightness}[%| procent]",
+        "close": "(zamknij|przymknij)",
+        "close_blind": "(zas\u0142o\u0144|opu\u015b\u0107)",
+        "close_curtain": "(zasuni\u0119te|zas\u0142oni\u0119te)",
+        "how_many_is": "Ile jest",
+        "lock": "zablokuj",
+        "name": "{name}",
+        "open": "otw\u00f3rz",
+        "open_blind": "(ods\u0142o\u0144|podnie\u015b)",
+        "open_curtain": "(odsuni\u0119te|ods\u0142oni\u0119te)",
+        "set": "(ustaw|zmie\u0144|przestaw|nastaw)",
+        "temp": "temperatur(a|\u0119|y)|stopni|zimno|gor\u0105co",
+        "temperature": "{temperature}[\u00b0| stopni] [{temperature_unit}]",
+        "turn_off": "(wy\u0142\u0105cz|zatrzymaj)",
+        "turn_off_light": "zga\u015b",
+        "turn_on": "(w\u0142\u0105cz|uruchom)",
+        "turn_on_light": "(zapal|o\u015bwie\u0107|za\u015bwie\u0107)",
+        "unlock": "odblokuj",
+        "what_is": "Jak[a|i] jest"
     },
     "intents": {
         "HassGetState": {
             "data": [
                 {
-                    "requires_context": {
-                        "device_class": "battery",
-                        "domain": "binary_sensor"
+                    "excludes_context": {
+                        "domain": [
+                            "scene",
+                            "script"
+                        ]
+                    },
+                    "response": "one",
+                    "sentences": [
+                        "jak(i|a|e) jest <name> [<area>]"
+                    ]
+                },
+                {
+                    "excludes_context": {
+                        "domain": [
+                            "scene",
+                            "script"
+                        ]
+                    },
+                    "response": "one_state",
+                    "sentences": [
+                        "jak(i|a|e) jest stan <name> [<area>]"
+                    ]
+                },
+                {
+                    "excludes_context": {
+                        "domain": [
+                            "scene",
+                            "script"
+                        ]
+                    },
+                    "response": "one_status",
+                    "sentences": [
+                        "jak(i|a|e) jest status <name> [<area>]"
+                    ]
+                },
+                {
+                    "excludes_context": {
+                        "domain": [
+                            "scene",
+                            "script"
+                        ]
+                    },
+                    "response": "one_value",
+                    "sentences": [
+                        "jak(i|a|e) jest warto\u015b\u0107 <name> [<area>]"
+                    ]
+                },
+                {
+                    "excludes_context": {
+                        "domain": [
+                            "cover"
+                        ]
                     },
                     "response": "one_yesno",
                     "sentences": [
-                        "[la|les] [batteri(e|es)] <dans> <name> [est|sont] [elle[s]] {bs_battery_states:state} [<dans> <area>]"
-                    ],
-                    "slots": {
-                        "device_class": "battery",
-                        "domain": "binary_sensor"
-                    }
+                        "czy [stan|status|warto\u015b\u0107] <name> jest {on_off_states:state} [<area>]",
+                        "czy [stan|status|warto\u015b\u0107] <name> [<area>] jest {on_off_states:state}"
+                    ]
+                },
+                {
+                    "response": "any",
+                    "sentences": [
+                        "(czy jest|czy s\u0105) [jaki\u015b|jakie\u015b] {on_off_domains:domain} {on_off_states:state} [<area>]",
+                        "(czy jest|czy s\u0105) [<area>] [jaki\u015b|jakie\u015b] {on_off_domains:domain} {on_off_states:state}",
+                        "czy [<area>] (jest|s\u0105) [jaki\u015b|jakie\u015b] {on_off_states:state} {on_off_domains:domain}"
+                    ]
                 },
                 {
                     "response": "all",
                     "sentences": [
-                        "Toute[s] [les] batterie[s] sont elle[s] {bs_battery_states:state} [<dans> <area>]"
-                    ],
-                    "slots": {
-                        "device_class": "battery",
-                        "domain": "binary_sensor"
-                    }
+                        "czy <all> {on_off_domains:domain} (jest|s\u0105) {on_off_states:state} [<area>]",
+                        "czy [<area>] <all> {on_off_domains:domain} (jest|s\u0105) {on_off_states:state}"
+                    ]
                 },
                 {
                     "response": "which",
                     "sentences": [
-                        "(quelle[s]|liste) [sont] [les] (appareil[s]|batterie[s]) (est|sont) {bs_battery_states:state} [<dans>  <area>]"
+                        "kt\u00f3r(y|e|a) {on_off_domains:domain} (jest|s\u0105) {on_off_states:state} [<area>]"
+                    ]
+                },
+                {
+                    "response": "how_many",
+                    "sentences": [
+                        "ile {on_off_domains:domain} (jest|s\u0105) {on_off_states:state} [<area>]",
+                        "<how_many_is> {on_off_states:state} {on_off_domains:domain} [<area>]"
+                    ]
+                },
+                {
+                    "requires_context": {
+                        "domain": "cover"
+                    },
+                    "response": "one_yesno_cover",
+                    "sentences": [
+                        "czy <name> jest {cover_states:state} [<area>]",
+                        "czy [<area>] <name> jest {cover_states:state}",
+                        "czy jest {cover_states:state} <name> [<area>]"
                     ],
                     "slots": {
-                        "device_class": "battery",
-                        "domain": "binary_sensor"
+                        "domain": "cover"
                     }
                 },
                 {
-                    "response": "how_many",
+                    "response": "any",
                     "sentences": [
-                        "Combien [de] batterie[s] [sont] [elle[s]] {bs_battery_states:state} [<dans>  <area>]"
+                        "czy jest [jaka\u015b] {cover_states:state} (roleta|\u017caluzja) [<area>]",
+                        "czy [<area>] jest [jaka\u015b] {cover_states:state} (roleta|\u017caluzja)",
+                        "czy [<area>] jest {cover_states:state} [jaka\u015b] (roleta|\u017caluzja)",
+                        "czy s\u0105 [jakie\u015b|kt\u00f3re\u015b|jaiekolwiek|kt\u00f3rekowliek] (rolety|\u017caluzje) {cover_states:state} [<area>]",
+                        "czy s\u0105 [jakie\u015b|kt\u00f3re\u015b|jaiekolwiek|kt\u00f3rekowliek] {cover_states:state} (rolety|\u017caluzje) [<area>]"
                     ],
                     "slots": {
-                        "device_class": "battery",
-                        "domain": "binary_sensor"
+                        "device_class": [
+                            "blind",
+                            "shade",
+                            "shutter"
+                        ],
+                        "domain": "cover"
                     }
                 },
                 {
-                    "requires_context": {
-                        "device_class": "battery_charging",
-                        "domain": "binary_sensor"
-                    },
-                    "response": "one_yesno",
+                    "response": "any",
                     "sentences": [
-                        "[la batterie] [<dans>] <name> [est] [(il|elle)] [en] {bs_battery_charging_states:state} [<dans>  <area>]"
+                        "czy jest [jaka\u015b] {cover_states:state} zas\u0142ona [<area>]",
+                        "czy [<area>] jest [jaka\u015b] {cover_states:state} zas\u0142ona",
+                        "czy [<area>] jest {cover_states:state} [jaka\u015b] zas\u0142ona",
+                        "czy s\u0105 [jakie\u015b|kt\u00f3re\u015b|jaiekolwiek|kt\u00f3rekowliek] zas\u0142ony {cover_states:state} [<area>]",
+                        "czy s\u0105 [jakie\u015b|kt\u00f3re\u015b|jaiekolwiek|kt\u00f3rekowliek] {cover_states:state} zas\u0142ony [<area>]"
                     ],
                     "slots": {
-                        "device_class": "battery_charging",
-                        "domain": "binary_sensor"
+                        "device_class": "curtain",
+                        "domain": "cover"
                     }
                 },
                 {
-                    "response": "any",
+                    "response": "all",
                     "sentences": [
-                        "[<yatil>] (des|plusieurs) (appareil[s]|batterie[s]) [(qui|en)] {bs_battery_charging_states:state} [<dans> <area>]"
+                        "czy <all> (rolety|\u017caluzje) s\u0105 {cover_states:state} [<area>]",
+                        "czy <all> (rolety|\u017caluzje) [<area>] s\u0105 {cover_states:state}"
                     ],
                     "slots": {
-                        "device_class": "battery_charging",
-                        "domain": "binary_sensor"
+                        "device_class": [
+                            "blind",
+                            "shade",
+                            "shutter"
+                        ],
+                        "domain": "cover"
                     }
                 },
                 {
                     "response": "all",
                     "sentences": [
-                        "Toute[s] [les] batterie[s] sont [elle[s]] {bs_battery_charging_states:state} [<dans> <area>]"
+                        "czy <all> zas\u0142ony s\u0105 {cover_states:state} [<area>]",
+                        "czy <all> zas\u0142ony [<area>] s\u0105 {cover_states:state}"
                     ],
                     "slots": {
-                        "device_class": "battery_charging",
-                        "domain": "binary_sensor"
+                        "device_class": "curtain",
+                        "domain": "cover"
                     }
                 },
                 {
                     "response": "which",
                     "sentences": [
-                        "(quel[le][s]|liste) [sont] [les] (appareil[s]|batterie[s]) [qui] [sont] {bs_battery_charging_states:state} [<dans> <area>]"
+                        "(kt\u00f3re|jakie) zas\u0142ony s\u0105 {cover_states:state} [<area>]"
                     ],
                     "slots": {
-                        "device_class": "battery_charging",
-                        "domain": "binary_sensor"
+                        "device_class": "curtain",
+                        "domain": "cover"
+                    }
+                },
+                {
+                    "response": "which_cover",
+                    "sentences": [
+                        "(kt\u00f3re|jakie) (rolety|\u017caluzje) s\u0105 {cover_states:state} [<area>]",
+                        "(kt\u00f3re|jakie) {cover_classes:device_class} s\u0105 {cover_states:state} [<area>]"
+                    ],
+                    "slots": {
+                        "device_class": [
+                            "blind",
+                            "shade",
+                            "shutter"
+                        ],
+                        "domain": "cover"
                     }
                 },
                 {
                     "response": "how_many",
                     "sentences": [
-                        "(combien|compte) [<dans>] [les] (appareil[s]|batterie[s]) [qui] [ne] [sont] {bs_battery_charging_states:state} [<dans> <area>]"
+                        "ile (rolet|\u017caluzji|zas\u0142on) jest {cover_states:state} [<area>]",
+                        "ile {cover_classes:device_class} jest {cover_states:state} [<area>]"
                     ],
                     "slots": {
-                        "device_class": "battery_charging",
-                        "domain": "binary_sensor"
+                        "domain": "cover"
                     }
                 },
                 {
                     "requires_context": {
-                        "device_class": "carbon_monoxide",
-                        "domain": "binary_sensor"
+                        "domain": "lock"
                     },
                     "response": "one_yesno",
                     "sentences": [
-                        "[<dans>] <name> [(a t|est)] [il] [(est|\u00e9t\u00e9)] [au statut] {bs_carbon_monoxide_states:state} [<dans> <area>]"
+                        "czy <name> s\u0105 {lock_states:state} [<area>]"
                     ],
                     "slots": {
-                        "device_class": "carbon_monoxide",
-                        "domain": "binary_sensor"
+                        "domain": "lock"
                     }
                 },
                 {
                     "response": "any",
                     "sentences": [
-                        "[<dans>] (CO2|monoxyde [de carbone]) [(a t|est)] [il] [(est|\u00e9t\u00e9)] {bs_carbon_monoxide_states:state} [<dans> <area>]"
+                        "czy s\u0105 [jakie\u015b|kt\u00f3re\u015b|jakiekolwiek|kt\u00f3rekolwiek] (drzwi|zamki) {lock_states:state} [<area>]",
+                        "czy s\u0105 [jakie\u015b|kt\u00f3re\u015b|jakiekolwiek|kt\u00f3rekolwiek] {lock_states:state} (drzwi|zamki) [<area>]"
                     ],
                     "slots": {
-                        "device_class": "carbon_monoxide",
-                        "domain": "binary_sensor"
+                        "domain": "lock"
                     }
                 },
                 {
-                    "response": "any",
+                    "response": "all",
                     "sentences": [
-                        "[<yatil>] [(un|le) capteur de] [une alerte] (monoxyde de carbone|CO2) [(est-il|est il|de)] [{bs_carbon_monoxide_states:state}] [<dans> <area>]"
+                        "czy <all> (drzwi|zamki) s\u0105 {lock_states:state} [<area>]"
                     ],
                     "slots": {
-                        "device_class": "carbon_monoxide",
-                        "domain": "binary_sensor",
-                        "state": "on"
+                        "domain": "lock"
                     }
                 },
                 {
-                    "response": "all",
+                    "response": "which",
                     "sentences": [
-                        "Tou(t|s) [les] capteurs [de] (CO2|monoxyde[ de carbone]) sont [ils] {bs_carbon_monoxide_states:state} [<dans> <area>]"
+                        "kt\u00f3re (drzwi|zamki) s\u0105 {lock_states:state} [<area>]",
+                        "kt\u00f3ry zamek jest {lock_states:state} [<area>]"
                     ],
                     "slots": {
-                        "device_class": "carbon_monoxide",
-                        "domain": "binary_sensor"
+                        "domain": "lock"
                     }
                 },
                 {
-                    "response": "which",
+                    "response": "how_many",
+                    "sentences": [
+                        "ile (drzwi|zamk\u00f3w) jest {lock_states:state} [<area>]"
+                    ],
+                    "slots": {
+                        "domain": "lock"
+                    }
+                }
+            ]
+        },
+        "HassTurnOff": {
+            "data": [
+                {
+                    "response": "fan_area",
                     "sentences": [
-                        "quel[s][le][s] capteur[s] [de] (CO2|monoxyde[de carbone]) (est|sont) [il][s] {bs_carbon_monoxide_states:state} [<dans> <area>]",
-                        "O\u00f9 du (CO2|monoxyde[ de carbone]) est [il] {bs_carbon_monoxide_states:state} "
+                        "<turn_off> (wentylator|wiatrak) <area>",
+                        "<turn_off> <area> (wentylator|wiatrak)"
                     ],
                     "slots": {
-                        "device_class": "carbon_monoxide",
-                        "domain": "binary_sensor"
+                        "domain": "fan",
+                        "name": "all"
                     }
                 },
                 {
-                    "response": "how_many",
+                    "response": "fans_area",
                     "sentences": [
-                        "(combien|compte) (de|le[s]) capteur[s] [de] (CO2|monoxyde[de carbone]) [qui] [sont] [ils] {bs_carbon_monoxide_states:state} [dans <area>]"
+                        "<turn_off> [<all>] (wentylatory|wiatraki) <area>",
+                        "<turn_off> <area> [<all>] (wentylatory|wiatraki)"
                     ],
                     "slots": {
-                        "device_class": "carbon_monoxide",
-                        "domain": "binary_sensor"
+                        "domain": "fan",
+                        "name": "all"
                     }
                 },
                 {
-                    "excludes_context": {
-                        "domain": [
-                            "scene",
-                            "script"
-                        ]
-                    },
-                    "response": "one",
+                    "response": "fans_all",
                     "sentences": [
-                        "quel est [l'etat de|le statut de ] <name> [<dans> <area>]"
-                    ]
+                        "<turn_off> <all> (wentylatory|wiatraki)"
+                    ],
+                    "slots": {
+                        "area": "all",
+                        "domain": "fan",
+                        "name": "all"
+                    }
                 },
                 {
                     "excludes_context": {
                         "domain": [
-                            "cover"
+                            "binary_sensor",
+                            "cover",
+                            "lock",
+                            "scene",
+                            "script",
+                            "sensor"
                         ]
                     },
-                    "response": "one_yesno",
                     "sentences": [
-                        "<name> [<dans> <area>] (est|est-elle) {on_off_states:state}"
+                        "(<turn_off>|<turn_off_light>) <name>"
                     ]
                 },
                 {
-                    "response": "any",
-                    "sentences": [
-                        "(certains|certaines) {on_off_domains:domain} [sont|sont-ils|sont-elles] {on_off_states:state} [<dans> <area>]"
-                    ]
-                },
-                {
-                    "response": "all",
+                    "response": "lights_area",
                     "sentences": [
-                        "(tous|toutes) les {on_off_domains:domain} [sont|sont-ils|sont-elles] {on_off_states:state} [<dans> <area>]"
-                    ]
+                        "(<turn_off>|<turn_off_light>) [<all>] [\u015bwiat\u0142a|\u015bwiat\u0142o] <area>",
+                        "(<turn_off>|<turn_off_light>) <area> [<all>] [\u015bwiat\u0142a|\u015bwiat\u0142o]"
+                    ],
+                    "slots": {
+                        "domain": "light"
+                    }
                 },
                 {
-                    "response": "which",
+                    "response": "light_all",
                     "sentences": [
-                        "(quelle[s]|quel[s]) sont les {on_off_domains:domain} {on_off_states:state} [<dans> <area>]"
-                    ]
+                        "(<turn_off>|<turn_off_light>) [<all>] \u015bwiat\u0142a"
+                    ],
+                    "slots": {
+                        "area": "all",
+                        "domain": "light",
+                        "name": "all"
+                    }
                 },
                 {
-                    "response": "how_many",
+                    "requires_context": {
+                        "domain": "cover"
+                    },
+                    "response": "cover",
                     "sentences": [
-                        "combien [(il y a|y a-t-il)] de {on_off_domains:domain} [sont] [d']{on_off_states:state} [<dans> <area>]"
+                        "(<close>|<close_blind>) <name>"
                     ]
                 },
                 {
                     "requires_context": {
                         "domain": "cover"
                     },
-                    "response": "one_yesno",
+                    "response": "cover_area_blind",
                     "sentences": [
-                        "<name> (est|est-il) {cover_states:state} [dans <area>]"
-                    ],
-                    "slots": {
-                        "domain": "cover"
-                    }
-                },
-                {
-                    "response": "any",
-                    "sentences": [
-                        "[Y a-t-il][il y a] (des|certains) {cover_classes:device_class} {cover_states:state} [dans <area>]"
-                    ],
-                    "slots": {
-                        "domain": "cover"
-                    }
+                        "(<close>|<close_blind>) <name> <area>"
+                    ]
                 },
                 {
-                    "response": "any",
+                    "response": "cover_garage",
                     "sentences": [
-                        "certains des {cover_classes:device_class} [<dans>] [<area>] [sont-ils] {cover_states:state}"
+                        "<close> gara\u017c",
+                        "<close> (drzwi|bram\u0119) (gara\u017cowe|gara\u017cow\u0105| od gara\u017cu)",
+                        "(drzwi|bram\u0119) (gara\u017cowe|gara\u017cow\u0105|od gara\u017cu) <close>"
                     ],
                     "slots": {
+                        "device_class": "garage",
                         "domain": "cover"
                     }
                 },
                 {
-                    "response": "all",
+                    "response": "cover_blind",
                     "sentences": [
-                        "tous [les] {cover_classes:device_class} [sont|sont-ils] {cover_states:state} [<dans> <area>]"
+                        "(<close>|<close_blind>) [<all>] rolety"
                     ],
                     "slots": {
+                        "device_class": [
+                            "curtain",
+                            "shutter",
+                            "curtain"
+                        ],
                         "domain": "cover"
                     }
                 },
                 {
-                    "response": "which",
+                    "response": "cover_area_blinds",
                     "sentences": [
-                        "(quel|quels) {cover_classes:device_class} (sont) {cover_states:state} [<dans> <area>]"
+                        "(<close>|<close_blind>) [<all>] rolety <area>",
+                        "(<close>|<close_blind>) <area> [<all>] rolety"
                     ],
                     "slots": {
                         "domain": "cover"
                     }
                 },
                 {
-                    "response": "how_many",
+                    "requires_context": {
+                        "domain": "lock"
+                    },
+                    "response": "lock_unlock_door",
                     "sentences": [
-                        "combien [Y a-t-il][il y a] de {cover_classes:device_class} [(sont|sont-ils|de)] {cover_states:state} [<dans> <area>]"
-                    ],
-                    "slots": {
-                        "domain": "cover"
-                    }
+                        "<unlock> <name> [<area>]"
+                    ]
                 },
                 {
                     "requires_context": {
                         "domain": "lock"
                     },
-                    "response": "one_yesno",
+                    "response": "lock_open_door",
                     "sentences": [
-                        "<name> (est|est-elle) {lock_states:state} [\u00e0 cl\u00e9|\u00e0 clef] [<dans> <area>]"
-                    ],
-                    "slots": {
-                        "domain": "lock"
-                    }
+                        "<open> <name> [<area>]"
+                    ]
                 },
                 {
-                    "response": "any",
+                    "response": "lock_unlock_door",
                     "sentences": [
-                        "(y a-t-il|il y a) (des|une) porte[s] [de] {lock_states:state} [<dans> <area>]"
+                        "<unlock> [<all>] drzwi <area>",
+                        "<unlock> <area> [<all>] drzwi",
+                        "<area> <unlock> [<all>] drzwi"
                     ],
                     "slots": {
-                        "domain": "lock"
+                        "domain": "lock",
+                        "name": "all"
                     }
                 },
                 {
-                    "response": "all",
+                    "response": "lock_unlock_lock",
                     "sentences": [
-                        "Toutes les porte[s] (sont|sont-elles) {lock_states:state} [<dans> <area>]"
+                        "<unlock> [<all>] zamki <area>",
+                        "<unlock> <area> [<all>] zamki",
+                        "<area> <unlock> [<all>] zamki"
                     ],
                     "slots": {
-                        "domain": "lock"
+                        "domain": "lock",
+                        "name": "all"
                     }
                 },
                 {
-                    "response": "which",
+                    "response": "lock_open_door",
                     "sentences": [
-                        "(quelles|quelle) porte[s] (sont|est) {lock_states:state} [<dans> <area>]"
+                        "<open> [<all>] drzwi <area>",
+                        "<open> <area> [<all>] drzwi",
+                        "<area> <open> [<all>] drzwi"
                     ],
                     "slots": {
-                        "domain": "lock"
+                        "domain": "lock",
+                        "name": "all"
                     }
                 },
                 {
-                    "response": "how_many",
+                    "response": "lock_open_lock",
                     "sentences": [
-                        "combien de porte[s] sont {lock_states:state} [<dans> <area>]"
+                        "<open> [<all>] zamki <area>",
+                        "<open> <area> [<all>] zamki",
+                        "<area> <open> [<all>] zamki"
                     ],
                     "slots": {
-                        "domain": "lock"
+                        "domain": "lock",
+                        "name": "all"
                     }
                 }
             ]
         },
-        "HassTurnOff": {
+        "HassTurnOn": {
             "data": [
                 {
-                    "response": "fan_all",
+                    "requires_context": {
+                        "domain": "scene"
+                    },
+                    "response": "scene",
                     "sentences": [
-                        "<eteins> [tous] <ventilateurs> <dans> [<area>]"
+                        "(<activate>|<turn_on>) [scen\u0119] <name>",
+                        "scena <name>"
                     ],
                     "slots": {
-                        "domain": "fan",
-                        "name": "all"
+                        "domain": "scene"
                     }
                 },
                 {
-                    "response": "fans_area",
+                    "response": "lights_area",
                     "sentences": [
-                        "<eteins> <ventilateur> [<dans>] [<area>]"
+                        "(<turn_on>|<turn_on_light>) [<all>] [\u015bwiat\u0142a|\u015bwiat\u0142o] <area>",
+                        "(<turn_on>|<turn_on_light>) <area> [<all>] [\u015bwiat\u0142a|\u015bwiat\u0142o]"
                     ],
                     "slots": {
-                        "domain": "fan"
+                        "domain": "light"
                     }
                 },
                 {
+                    "response": "light_all",
                     "sentences": [
-                        "<eteins> <name>",
-                        "<eteins> <name> <dans> <area>"
-                    ]
+                        "(<turn_on>|<turn_on_light>) <all> \u015bwiat\u0142a"
+                    ],
+                    "slots": {
+                        "area": "all",
+                        "domain": "light",
+                        "name": "all"
+                    }
                 },
                 {
+                    "requires_context": {
+                        "domain": "cover"
+                    },
                     "response": "cover",
                     "sentences": [
-                        "<ferme> <name>"
+                        "(<open>|<open_blind>) <name>"
                     ]
                 },
                 {
-                    "response": "cover_area",
+                    "requires_context": {
+                        "domain": "cover"
+                    },
+                    "response": "cover_area_blind",
                     "sentences": [
-                        "<ferme> <name> <dans> <area>"
+                        "(<open>|<open_blind>) <name> <area>"
                     ]
                 },
                 {
+                    "response": "cover_garage",
                     "sentences": [
-                        "<eteins> [toutes] (<lumiere> | <lumieres>) <dans> <area>"
+                        "<open> gara\u017c",
+                        "<open> (drzwi|bram\u0119) (gara\u017cowe|gara\u017cow\u0105| od gara\u017cu)",
+                        "(Drzwi|Bram\u0119) (gara\u017cowe|gara\u017cow\u0105| od gara\u017cu) <open>"
                     ],
                     "slots": {
-                        "domain": "light"
+                        "device_class": "garage",
+                        "domain": "cover"
                     }
                 },
                 {
-                    "response": "cover_device_class",
+                    "response": "cover_blind",
                     "sentences": [
-                        "<ferme> <garage>"
+                        "(<open>|<open_blind>) [<all>] rolety"
                     ],
                     "slots": {
-                        "device_class": "garage",
+                        "device_class": "curtain",
                         "domain": "cover"
                     }
                 },
                 {
-                    "response": "cover_area",
+                    "response": "cover_area_blinds",
                     "sentences": [
-                        "<ferme> [tous] (<volets>|<volet>) <dans> <area>"
+                        "(<open>|<open_blind>) [<all>] rolety <area>",
+                        "(<open>|<open_blind>) <area> [<all>] rolety"
                     ],
                     "slots": {
-                        "device_class": [
-                            "blind",
-                            "curtain",
-                            "shutter"
-                        ],
                         "domain": "cover"
                     }
                 },
                 {
-                    "response": "cover_device_class",
+                    "response": "fan_area",
                     "sentences": [
-                        "<ferme> tous (<volets>|<volet>)"
+                        "<turn_on> (wentylator|wiatrak) <area>",
+                        "<turn_on> <area> (wentylator|wiatrak)"
                     ],
                     "slots": {
-                        "device_class": [
-                            "blind",
-                            "curtain",
-                            "shutter"
-                        ],
-                        "domain": "cover",
+                        "domain": "fan",
                         "name": "all"
                     }
-                }
-            ]
-        },
-        "HassTurnOn": {
-            "data": [
+                },
                 {
+                    "response": "fans_area",
                     "sentences": [
-                        "<allume> [toutes] (<lumiere> | <lumieres>) <dans> <area>"
+                        "<turn_on> [<all>] (wentylatory|wiatraki) <area>",
+                        "<turn_on> <area> [<all>] (wentylatory|wiatraki)"
                     ],
                     "slots": {
-                        "domain": "light"
+                        "domain": "fan",
+                        "name": "all"
                     }
                 },
                 {
-                    "response": "cover_device_class",
+                    "response": "fans_all",
                     "sentences": [
-                        "<ouvre> <garage>"
+                        "<turn_on> <all> (wentylatory|wiatraki)"
                     ],
                     "slots": {
-                        "device_class": "garage",
-                        "domain": "cover"
+                        "area": "all",
+                        "domain": "fan",
+                        "name": "all"
                     }
                 },
                 {
-                    "response": "cover_area",
+                    "requires_context": {
+                        "domain": "lock"
+                    },
+                    "response": "lock_lock_door",
                     "sentences": [
-                        "<ouvre> [tous] (<volets>|<volet>) <dans> <area>"
-                    ],
-                    "slots": {
-                        "device_class": [
-                            "blind",
-                            "curtain",
-                            "shutter"
-                        ],
-                        "domain": "cover"
-                    }
+                        "<lock> <name> [<area>]"
+                    ]
+                },
+                {
+                    "requires_context": {
+                        "domain": "lock"
+                    },
+                    "response": "lock_close_door",
+                    "sentences": [
+                        "<close> <name> [<area>]"
+                    ]
                 },
                 {
-                    "response": "cover_device_class",
+                    "response": "lock_lock_door",
                     "sentences": [
-                        "<ouvre> tous [les] (<volets>|<volet>)"
+                        "<lock> [<all>] drzwi <area>",
+                        "<lock> <area> [<all>] drzwi"
                     ],
                     "slots": {
-                        "device_class": [
-                            "blind",
-                            "curtain",
-                            "shutter"
-                        ],
-                        "domain": "cover",
+                        "domain": "lock",
                         "name": "all"
                     }
                 },
                 {
-                    "response": "fan_all",
+                    "response": "lock_lock_lock",
                     "sentences": [
-                        "<allume> [tous] (<ventilateur> | <ventilateurs>) <dans> [<area>]"
+                        "<lock> [<all>] zamki <area>",
+                        "<lock> <area> [<all>] zamki"
                     ],
                     "slots": {
-                        "domain": "fan",
+                        "domain": "lock",
                         "name": "all"
                     }
                 },
                 {
-                    "response": "fans_area",
+                    "response": "lock_close_door",
                     "sentences": [
-                        "<allume> (<ventilateur> | <ventilateurs>) [<dans>] [<area>]"
+                        "<close> [<all>] drzwi <area>",
+                        "<close> <area> [<all>] drzwi"
                     ],
                     "slots": {
-                        "domain": "fan"
+                        "domain": "lock",
+                        "name": "all"
                     }
                 },
                 {
+                    "response": "lock_close_lock",
                     "sentences": [
-                        "<allume> <name>",
-                        "<allume> <name> <dans> <area>"
-                    ]
+                        "<close> [<all>] zamki <area>",
+                        "<close> <area> [<all>] zamki"
+                    ],
+                    "slots": {
+                        "domain": "lock",
+                        "name": "all"
+                    }
                 },
                 {
-                    "response": "cover",
+                    "requires_context": {
+                        "domain": "script"
+                    },
+                    "response": "script",
                     "sentences": [
-                        "<ouvre> <name>"
-                    ]
+                        "[<activate>|<turn_on>] [skrypt] <name>"
+                    ],
+                    "slots": {
+                        "domain": "script"
+                    }
                 },
                 {
-                    "response": "cover_area",
+                    "excludes_context": {
+                        "domain": [
+                            "binary_sensor",
+                            "cover",
+                            "lock",
+                            "scene",
+                            "script",
+                            "sensor"
+                        ]
+                    },
                     "sentences": [
-                        "<ouvre> <name> <dans> <area>"
+                        "(<turn_on>|<turn_on_light>) <name>"
                     ]
                 }
             ]
         }
     },
-    "language": "fr",
+    "language": "pl",
     "lists": {
         "brightness": {
             "range": {
                 "from": 0,
                 "to": 100,
                 "type": "percentage"
             }
         },
-        "bs_battery_charging_states": {
-            "values": [
-                {
-                    "in": "([en] [cours de] charge[ment]|en[ ]train de charger)",
-                    "out": "on"
-                },
-                {
-                    "in": "pas en charge",
-                    "out": "off"
-                }
-            ]
-        },
-        "bs_battery_states": {
+        "brightness_level": {
             "values": [
                 {
-                    "in": "(basse[s]|faible[s]|vide[s]|d\u00e9charg\u00e9[e][s])",
-                    "out": "on"
-                },
-                {
-                    "in": "(normale[s]|charg\u00e9e[s]|pleine[s])",
-                    "out": "off"
-                }
-            ]
-        },
-        "bs_carbon_monoxide_states": {
-            "values": [
-                {
-                    "in": "(d\u00e9clench\u00e9[e][s]|d\u00e9tect\u00e9[e][s]|en alarme)",
-                    "out": "on"
+                    "in": "(maksymalny | najja\u015bniej | maksa)",
+                    "out": 100
                 },
                 {
-                    "in": "(non d\u00e9tect\u00e9[e][s]|s\u00e9curis\u00e9[e][s])",
-                    "out": "off"
+                    "in": "(minimalnie | najciemniej | minimum)",
+                    "out": 1
                 }
             ]
         },
         "color": {
             "values": [
                 {
-                    "in": "(blanc|blanche)",
+                    "in": "biel|bia\u0142(y|o|e)",
                     "out": "white"
                 },
                 {
-                    "in": "(noir|noire)",
+                    "in": "czer\u0144|czarn(y|o|e)",
                     "out": "black"
                 },
                 {
-                    "in": "rouge",
+                    "in": "czerwie\u0144|czerwon(y|o|e)",
                     "out": "red"
                 },
                 {
-                    "in": "orange",
+                    "in": "pomara\u0144cz|pomara\u0144czow(y|o|e)",
                     "out": "orange"
                 },
                 {
-                    "in": "jaune",
+                    "in": "\u017c\u00f3\u0142t(y|o|e)",
                     "out": "yellow"
                 },
                 {
-                    "in": "(vert|verte)",
+                    "in": "ziele\u0144|zielon(y|o|e)",
                     "out": "green"
                 },
                 {
-                    "in": "(bleu|bleue)",
+                    "in": "niebiesk(i|o|ie)",
                     "out": "blue"
                 },
                 {
-                    "in": "(violet|violette)",
+                    "in": "fiolet|fioletow(y|o|e)",
                     "out": "purple"
                 },
                 {
-                    "in": "marron",
+                    "in": "br\u0105z|br\u0105zow(y|o|e)",
                     "out": "brown"
-                },
-                {
-                    "in": "rose",
-                    "out": "pink"
                 }
             ]
         },
         "cover_classes": {
             "values": [
                 {
-                    "in": "store[s]",
-                    "out": "awning"
+                    "in": "(drzwi gara\u017cowe|drzwi w gara\u017cu)",
+                    "out": "garage"
                 },
                 {
-                    "in": "store[s]",
-                    "out": "blind"
+                    "in": "bram(a|y)",
+                    "out": "gate"
                 },
                 {
-                    "in": "rideau[x]",
+                    "in": "zas\u0142on(a|y)",
                     "out": "curtain"
                 },
                 {
-                    "in": "porte[s]",
-                    "out": "door"
-                },
-                {
-                    "in": "portes[s] de garage[s]",
-                    "out": "garage door"
+                    "in": "markiz(a|y)",
+                    "out": "awning"
                 },
                 {
-                    "in": "portail[s]",
-                    "out": "gate"
+                    "in": "rolet(a|y)",
+                    "out": "blind"
                 },
                 {
-                    "in": "store[s]",
+                    "in": "rolet(a|y)",
                     "out": "shade"
                 },
                 {
-                    "in": "volet[s]",
+                    "in": "\u017caluzj(a|e)",
                     "out": "shutter"
-                },
-                {
-                    "in": "fen\u00eatre[s]",
-                    "out": "window"
                 }
             ]
         },
         "cover_states": {
             "values": [
                 {
-                    "in": "ouvert[e][s]",
+                    "in": "(otw(\u00f3rz|arta|arte|artych)|odsuni\u0119t(e|ych)|ods\u0142oni\u0119t(e|ych))",
                     "out": "open"
                 },
                 {
-                    "in": "ferm\u00e9[e][s]",
+                    "in": "(zamkni(j|\u0119ta|\u0119te|\u0119tych)|zasuni\u0119t(e|ych)|zas\u0142oni\u0119t(e|ych))",
                     "out": "closed"
                 },
                 {
-                    "in": "ouverture",
+                    "in": "otwieranie",
                     "out": "opening"
                 },
                 {
-                    "in": "fermeture",
+                    "in": "zamykanie",
                     "out": "closing"
                 }
             ]
         },
         "lock_states": {
             "values": [
                 {
-                    "in": "verrouill[e][er][\u00e9][\u00e9e][s]",
-                    "out": "locked"
-                },
-                {
-                    "in": "ferm[e][er][\u00e9][\u00e9e][s]",
+                    "in": "zablokowan(e|y|ych)|zamkni\u0119t(y|e|ych)",
                     "out": "locked"
                 },
                 {
-                    "in": "d\u00e9verrouill[e][er][\u00e9][\u00e9e][s]",
-                    "out": "unlocked"
-                },
-                {
-                    "in": "ouvert[e][s]",
-                    "out": "unlocked"
-                },
-                {
-                    "in": "ouvr[e][s]",
+                    "in": "odblokowan(e|y|ych)|otwart(e|y|ych)",
                     "out": "unlocked"
                 }
             ]
         },
         "on_off_domains": {
             "values": [
                 {
-                    "in": "lampe[s]|lumi\u00e8re[s]",
+                    "in": "\u015bwiat(\u0142o|\u0142a|e\u0142)|lamp(a|y)",
                     "out": "light"
                 },
                 {
-                    "in": "ventilateur[s]",
+                    "in": "wentylator[y|\u00f3w]|wiatrak[i|\u00f3w]",
                     "out": "fan"
                 },
                 {
-                    "in": "interrupteur[s]",
+                    "in": "prze\u0142\u0105cznik[i|\u00f3w]|kontakt[y|\u00f3w]",
                     "out": "switch"
                 }
             ]
         },
         "on_off_states": {
             "values": [
                 {
-                    "in": "allum\u00e9[e][s]",
+                    "in": "w\u0142\u0105cz[ony|one|ona|onych]",
                     "out": "on"
                 },
                 {
-                    "in": "\u00e9teint[e][s]",
+                    "in": "wy\u0142\u0105cz[ony|one|ona|onych]",
                     "out": "off"
                 }
             ]
         },
         "temperature": {
             "range": {
                 "from": 0,
                 "to": 100,
                 "type": "temperature"
             }
         },
         "temperature_unit": {
             "values": [
-                "celsius",
                 {
-                    "in": "c",
+                    "in": "c|celsjusza",
                     "out": "celsius"
                 },
-                "fahrenheit",
                 {
-                    "in": "f",
+                    "in": "f|fahrenheita",
                     "out": "fahrenheit"
                 }
             ]
         }
     },
     "responses": {
         "errors": {
-            "handle_error": "Une erreur est intervenue pendant le traitement",
-            "no_area": "Aucune zone appel\u00e9e {{ area }}",
-            "no_device_class": "{{ area }} ne contient pas de {{ device_class }}",
-            "no_domain": "{{ area }} ne contient pas de {{ domain }}",
-            "no_entity": "Aucun appareil ou entit\u00e9 appel\u00e9 {{ entity }}",
-            "no_intent": "D\u00e9sol\u00e9, je n'ai pas compris"
+            "handle_error": "Podczas przetwarzania zapytania wyst\u0105pi\u0142 nieoczekiwany b\u0142\u0105d",
+            "no_area": "Brak obszaru nazwanego {{ area }}",
+            "no_device_class": "Obszar {{ area }} nie zawiera {{ device_class }}",
+            "no_domain": "W obszarze {{ area }} nie ma {{ domain }}",
+            "no_entity": "Brak urz\u0105dzenia lub encji nazwanej {{ entity }}",
+            "no_intent": "Wybacz, niestety nie mog\u0119 tego zrozumie\u0107"
         },
         "intents": {
             "HassGetState": {
-                "all": "{% if not query.unmatched: %}\n  Oui\n{% else %}\n  {% set no_match = query.unmatched | map(attribute=\"name\") | sort | list %}\n  {% set count_match = no_match | length | int %}\n  {% if no_match | length > 4 %}\n    Non,pas  {{ no_match[:3] | join(\", \") }} et {{ (no_match | length - 3) }} autres\n  {% elif no_match | length == 1 %}\n    Non, pas l'appareil\n    {% for name in no_match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} et {% endif -%}\n      {{ name }}\n    {%- endfor %}\n  {%- else -%}\n    Non, pas les appareils \n    {% for name in no_match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} et {% endif -%}\n      {{ name }}\n    {%- endfor %}\n  {% endif %}\n{% endif %}\n",
-                "any": "{% if query.matched %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% set count_match = no_match | length | int %}\n  {% if match | length > 4 %}\n    Oui, {{ match[:3] | join(\", \") }} et {{ (match | length - 3) }} autres\n  {% elif match | length == 1 %}\n    Oui, l'appareil\n    {% for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} et {% endif -%}\n      {{ name }}\n    {% endfor %}\n    est {{ state.state_with_unit }}\n  {%- else -%}\n    Oui, les appareils\n    {% for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} et {% endif -%}\n      {{ name }}\n    {% endfor %}\n    sont {{ state.state_with_unit }}\n  {% endif %}\n{% else %}\n  Non\n{% endif %}\n",
+                "all": "{% if not query.unmatched: %}\n  Tak\n{% else %}\n  {% set no_match = query.unmatched | map(attribute=\"name\") | sort | list %}\n  {% if no_match | length > 4 %}\n    Nie, {{ no_match[:3] | join(\", \") }} oraz {{ (no_match | length - 3) }} nie ma ju\u017c wi\u0119cej\n  {%- else -%}\n    Nie,\n    {% for name in no_match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} i {% endif -%}\n      {{ name }}\n    {%- endfor %} nie {% if state.attributes.device_class == \"curtain\" and no_match|length|int|abs == 1 -%}jest\n      {%- elif state.attributes.device_class == \"lock\" and no_match|length|int|abs == 1 -%}jest\n      {%- elif state.attributes.device_class == \"door\" and no_match|length|int|abs == 1 -%}s\u0105\n      {%- else -%}{{ 's\u0105' if no_match|length|int|abs == 1 else 's\u0105' if no_match|length|int | abs in [2,3,4] else 's\u0105' if (no_match|length|string)[-1] | int | abs in [2,3,4] else 'jest' }}\n      {%- endif -%}\n  {% endif %}\n{% endif %}\n",
+                "any": "{% if query.matched %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length > 4 %}\n    Tak, {{ match[:3] | join(\", \") }} oraz {{ (match | length - 3) }} wi\u0119cej\n  {%- else -%}\n    Tak,\n    {% for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} i {% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% else %}\n  Nie\n{% endif %}\n",
                 "how_many": "{{ query.matched | length }}\n",
-                "one": "L'etat de l'appareil {{ slots.name | capitalize }} est {{ state.state_with_unit }}\n",
-                "one_yesno": "{% if query.matched %}\n  Oui\n{% else %}\n  Non, {{ state.state_with_unit }}\n{% endif %}\n",
-                "which": "{% if not query.matched %}\n  Aucun appareil\n{% else: %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% set count_match = match | length | int %}\n  {% if match | count > 4 %}\n    Les appareils \n    {{ match[:3] | join(\", \") }} et {{ (match | length - 3) }} autres\n  {% elif match | count == 1 %}\n    L'appareil \n    {% for name in match %}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} et {% endif -%}\n      {{ name }}\n    {% endfor %}\n    est {{ state.state_with_unit }}\n  {% else %}\n    Les appareils \n    {% for name in match %}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} et {% endif -%}\n      {{ name }}\n    {% endfor %}\n    sont {{ state.state_with_unit }}s\n  {% endif %}\n{% endif %}\n"
+                "one": "{{ slots.name | capitalize }} jest {{ state.state_with_unit }}\n",
+                "one_state": "Stan {{ slots.name | capitalize }} to {{ state.state_with_unit }}\n",
+                "one_status": "Status {{ slots.name | capitalize }} to {{ state.state_with_unit }}\n",
+                "one_value": "Warto\u015b\u0107 {{ slots.name | capitalize }} to {{ state.state_with_unit }}\n",
+                "one_yesno": "{% if query.matched: %}\nTak\n{% else: %}\nNie, {{ slots.name }} jest {{ state.state_with_unit }}\n{% endif %}\n",
+                "one_yesno_cover": "{% if query.matched: %}\nTak\n{% else: %}\nNie, {{ slots.name }} jest {{ 'otwarta' if state.state_with_unit == 'open' else 'zamkni\u0119ta' }}\n{% endif %}\n",
+                "which": "{% if not query.matched %}\n  \u017baden\n{% else: %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length > 4 %}\n    {{ match[:3] | join(\", \") }} oraz {{ (match | length - 3) }} inne\n  {% else %}\n    {%- for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} i {% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% endif %}\n",
+                "which_cover": "{% if not query.matched %}\n  \u017badne\n{% else: %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length > 4 %}\n    {{ match[:3] | join(\", \") }} oraz {{ (match | length - 3) }} inne\n  {% else %}\n    {%- for name in match -%}\n      {% if not loop.first and not loop.last %}, {% elif loop.last and not loop.first %} i {% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% endif %}\n"
             },
             "HassTurnOff": {
-                "cover": "{{ slots.name }} ferm\u00e9",
-                "cover_area": "Ouvrants de {{ slots.area }} ferm\u00e9s",
-                "cover_device_class": "{{ slots.device_class }} ferm\u00e9",
-                "default": "{{ slots.name }} \u00e9teint",
-                "fan_all": "Tous les ventilateurs sont \u00e9teints",
-                "fans_area": "Ventilateurs de {{ slots.area }} \u00e9teints",
-                "light_all": "Toutes les lumi\u00e8res sont \u00e9teintes",
-                "lights_area": "Lumi\u00e8res de {{ slots.area }} \u00e9teintes"
+                "cover": "Zamkni\u0119to {{ slots.name }}",
+                "cover_area_blind": "Zamkni\u0119to rolet\u0119 w {{ slots.area }}",
+                "cover_area_blinds": "Zamkni\u0119to rolety w {{ slots.area }}",
+                "cover_area_garage": "Zamkni\u0119to gara\u017c w {{ slots.area }}",
+                "cover_blind": "Zamkni\u0119to rolety",
+                "cover_garage": "Zamkni\u0119to gara\u017c",
+                "default": "Wy\u0142\u0105czono {{ slots.name }}",
+                "fan_area": "Wy\u0142\u0105czono wentylator w {{ slots.area }}",
+                "fans_all": "Wy\u0142\u0105czono wszystkie wentylatory",
+                "fans_area": "Wy\u0142\u0105czono wentylatory w {{ slots.area }}",
+                "light_all": "Wy\u0142\u0105czono wszystkie \u015bwiat\u0142a",
+                "lights_area": "Wy\u0142\u0105czono \u015bwiat\u0142o w {{ slots.area }}",
+                "lock_open_door": "Otwarto {{ slots.name if slots.name != 'all' else 'wszystkie drzwi' }}",
+                "lock_open_lock": "Otwarto {{ slots.name if slots.name != 'all' else 'wszystkie zamki' }}",
+                "lock_unlock_door": "Odblokowano {{ slots.name if slots.name != 'all' else 'wszystkie drzwi' }}",
+                "lock_unlock_lock": "Odblokowano {{ slots.name if slots.name != 'all' else 'wszystkie zamki' }}"
             },
             "HassTurnOn": {
-                "cover": "{{ slots.name }} ouvert",
-                "cover_all": "Ouvre tous les ouvrants de {{ slots.area }}",
-                "cover_area": "Ouvrants de {{ slots.area }} ouverts",
-                "cover_device_class": "{{ slots.device_class }} ouvert",
-                "default": "{{ slots.name }} allum\u00e9",
-                "fan_all": "Allume tous les ventilateurs",
-                "fans_area": "Ventilateurs de {{ slots.area }} allum\u00e9s",
-                "light_all": "Allume toutes les lumi\u00e8res",
-                "lights_area": "Lumi\u00e8res de {{ slots.area }} allum\u00e9es"
+                "cover": "Otwarto {{ slots.name }}",
+                "cover_area_blind": "Otwarto rolet\u0119 w {{ slots.area }}",
+                "cover_area_blinds": "Otwarto rolety w {{ slots.area }}",
+                "cover_area_garage": "Otwarto gara\u017c w {{ slots.area }}",
+                "cover_blind": "Otwarto rolety",
+                "cover_garage": "Otwarto gara\u017c",
+                "default": "W\u0142\u0105czono {{ slots.name }}",
+                "fan_area": "W\u0142\u0105czono wentylator w {{ slots.area }}",
+                "fans_all": "W\u0142\u0105czono wszystkie wentylatory",
+                "fans_area": "W\u0142\u0105czono wentylatory w {{ slots.area }}",
+                "light_all": "W\u0142\u0105czono wszystkie \u015bwiat\u0142a",
+                "lights_area": "W\u0142\u0105czono \u015bwiat\u0142o w {{ slots.area }}",
+                "lock_close_door": "Zamkni\u0119to {{ slots.name if slots.name != 'all' else 'wszystkie drzwi' }}",
+                "lock_close_lock": "Zamkni\u0119to {{ slots.name if slots.name != 'all' else 'wszystkie zamki' }}",
+                "lock_lock_door": "Zablokowano {{ slots.name if slots.name != 'all' else 'wszystkie drzwi' }}",
+                "lock_lock_lock": "Zablokowano {{ slots.name if slots.name != 'all' else 'wszystkie zamki' }}",
+                "scene": "Aktywowano scen\u0119 {{ slots.name }}",
+                "script": "Uruchomiono skrypt {{ slots.name }}"
             }
         }
     },
     "skip_words": [
-        "s'il te pla\u00eet",
-        "merci",
-        "est ce que"
+        "Prosz\u0119",
+        "Poprosz\u0119"
     ]
 }
```

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/gl.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/gl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/gu.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/gu.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/he.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/he.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/hi.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/hi.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/hr.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/hr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/hu.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/hu.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/id.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/id.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/is.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/is.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/it.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/it.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9975490196078431%*

 * *Differences: {"'expansion_rules'": "{'cover': '(tend(a|e)[ da "*

 * *                      "sole]|serrand(a|e)|tapparell(a|e)|persian(a|e)|port(a|e)|saracinesc(a|he)|venezian(a|e)|cancell(o|i)|finestr(a|e))'}"}*

```diff
@@ -1,13 +1,13 @@
 {
     "expansion_rules": {
         "area": "{area}",
         "brightness": "{brightness}[%| percento]",
         "close": "(chiud(i|ere) | abbass(a|are))",
-        "cover": "(tend(a|e)[ da sole]|serrand(a|e)|tapparell(a|e)|persian(a|e)|port(a|e)|saracinesc(a|he)|venezian(a|e)|cancell(o|i)|finestr(a|i))",
+        "cover": "(tend(a|e)[ da sole]|serrand(a|e)|tapparell(a|e)|persian(a|e)|port(a|e)|saracinesc(a|he)|venezian(a|e)|cancell(o|i)|finestr(a|e))",
         "fan": "(ventol(a|e) | ventilator(e|i) | ventilazione | climatizzator(e|i) | condizionator(e|i))",
         "in": "(in | ne[i|gli|l[lo|la|le]])",
         "name": "{name}",
         "of": "(de[i|gli|l[lo|la|le]]|di)",
         "open": "(apr(i|ire) | alz(a|are))",
         "set": "(impost(a|are) | cambi(a|are) | mett(i|ere) | modific(a|are))",
         "temp": "[la] (temperatura)",
```

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/ka.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/ka.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/kn.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/kn.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/lb.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/lb.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/lt.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/lt.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/lv.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/lv.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/ml.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/ml.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/mn.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/mn.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/ms.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/ms.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/nb.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/nb.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/nl.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/nl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/pt-br.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/pt-br.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/pt.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/pt.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/ro.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/ro.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/ru.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/ru.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/sk.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/sk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/sl.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/sl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/sr.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/sr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/sv.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/sv.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/sw.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/sw.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/te.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/te.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/tr.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/tr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/uk.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/uk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/ur.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/ur.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/vi.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/vi.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/zh-cn.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/zh-cn.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/zh-hk.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/zh-hk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/homeassistant/zh-tw.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/homeassistant/zh-tw.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9634566252869824%*

 * *Differences: {"'expansion_rules'": "{'name': '{name}[的]', 'area': '{area}[的]', 'let': '[把|將]', 'all': "*

 * *                      "'(全部|所有)[的]', 'how_many_is': '(是多少|有多少|有幾個)', 'brightness': '[百分之] "*

 * *                      "{brightness}[ ][%|趴]', 'set_to': '(設|設定|設置|調|調整|變更)(為|到|成|至)', 'turn_on': "*

 * *                      "'(打開|開|開啟)', 'turn_off': '(關|關掉|關閉|關上)', 'open': '(打開|開啟|開)', 'close': "*

 * *                      "'(關|關閉|關上)', 'light': '(燈|燈光|照明|桌燈|檯燈|床頭燈|壁燈|吸頂燈|崁燈|嵌燈)[的]', 'fan': "*

 * *                      "'(電扇|電風扇|風扇|循環扇|吊扇 […]*

```diff
@@ -1,33 +1,33 @@
 {
     "expansion_rules": {
-        "all": "(\u5168\u90e8 | \u6240\u6709) [\u7684]",
-        "area": "{area} [\u7684]",
-        "brightness": "[\u767e\u5206\u4e4b]  {brightness}[ ][%|\u8db4]",
-        "close": "(\u95dc | \u95dc\u9589 | \u95dc\u4e0a)",
+        "all": "(\u5168\u90e8|\u6240\u6709)[\u7684]",
+        "area": "{area}[\u7684]",
+        "brightness": "[\u767e\u5206\u4e4b] {brightness}[ ][%|\u8db4]",
+        "close": "(\u95dc|\u95dc\u9589|\u95dc\u4e0a)",
         "door": "(\u9580|\u5927\u9580)",
-        "fan": "(\u96fb\u6247 | \u96fb\u98a8\u6247 | \u98a8\u6247 | \u5faa\u74b0\u6247 | \u540a\u6247)",
-        "how_many": "(\u662f\u591a\u5c11 | \u6709\u591a\u5c11 | \u6709\u5e7e\u500b)",
-        "how_many_is": "(\u662f\u591a\u5c11 | \u6709\u591a\u5c11 | \u6709\u5e7e\u500b)",
-        "let": "[\u628a | \u5c07]",
-        "light": "(\u71c8 |  \u71c8\u5149 | \u7167\u660e | \u684c\u71c8 | \u6aaf\u71c8 | \u5e8a\u982d\u71c8 | \u58c1\u71c8 | \u5438\u9802\u71c8 | \u5d01\u71c8) [\u7684]",
-        "name": "{name} [\u7684]",
-        "open": "(\u6253\u958b | \u958b\u555f | \u958b)",
-        "set": "(\u8a2d | \u8a2d\u5b9a | \u8a2d\u7f6e | \u8abf | \u8abf\u6574 | \u8b8a\u66f4 )",
-        "set_to": "(\u8a2d | \u8a2d\u5b9a | \u8a2d\u7f6e | \u8abf | \u8abf\u6574 | \u8b8a\u66f4 ) (\u70ba | \u5230 | \u6210 | \u81f3)",
+        "fan": "(\u96fb\u6247|\u96fb\u98a8\u6247|\u98a8\u6247|\u5faa\u74b0\u6247|\u540a\u6247|\u58c1\u639b\u6247|\u58c1\u6247|\u639b\u6247)",
+        "how_many": "(\u662f\u591a\u5c11|\u6709\u591a\u5c11|\u6709\u5e7e\u500b)",
+        "how_many_is": "(\u662f\u591a\u5c11|\u6709\u591a\u5c11|\u6709\u5e7e\u500b)",
+        "let": "[\u628a|\u5c07]",
+        "light": "(\u71c8|\u71c8\u5149|\u7167\u660e|\u684c\u71c8|\u6aaf\u71c8|\u5e8a\u982d\u71c8|\u58c1\u71c8|\u5438\u9802\u71c8|\u5d01\u71c8|\u5d4c\u71c8)[\u7684]",
+        "name": "{name}[\u7684]",
+        "open": "(\u6253\u958b|\u958b\u555f|\u958b)",
+        "set": "(\u8a2d|\u8a2d\u5b9a|\u8a2d\u7f6e|\u8abf|\u8abf\u6574|\u8b8a\u66f4 )",
+        "set_to": "(\u8a2d|\u8a2d\u5b9a|\u8a2d\u7f6e|\u8abf|\u8abf\u6574|\u8b8a\u66f4)(\u70ba|\u5230|\u6210|\u81f3)",
         "switch": "(\u958b\u95dc|\u96fb\u6e90|\u63d2\u5ea7|\u7e3d\u958b\u95dc|\u71c8\u5149)",
         "temp": "\u6eab\u5ea6",
-        "temperature": "{temperature} [{temperature_unit}]",
+        "temperature": "{temperature}[{temperature_unit}]",
         "to": "(\u70ba|\u5230|\u6210|\u81f3)",
-        "turn": "(\u8a2d | \u8a2d\u5b9a | \u8a2d\u7f6e | \u8abf | \u8abf\u6574 | \u8b8a\u66f4 ) (\u70ba | \u5230 | \u6210 | \u81f3)",
-        "turn_off": "(\u95dc | \u95dc\u6389 | \u95dc\u9589 | \u95dc\u4e0a)",
-        "turn_on": "(\u6253\u958b | \u958b | \u958b\u555f)",
+        "turn": "(\u8a2d|\u8a2d\u5b9a|\u8a2d\u7f6e|\u8abf|\u8abf\u6574|\u8b8a\u66f4)(\u70ba|\u5230|\u6210|\u81f3)",
+        "turn_off": "(\u95dc|\u95dc\u6389|\u95dc\u9589|\u95dc\u4e0a)",
+        "turn_on": "(\u6253\u958b|\u958b|\u958b\u555f)",
         "what_is": "\u662f\u4ec0\u9ebc",
-        "which": "[\u6709 | \u6709\u6c92\u6709] \u54ea [\u4e00] (\u500b | \u4e9b | \u6247 | \u76de | \u9053)",
-        "window": "(\u7a97\u6236 | \u7a97\u7c3e | \u6372\u7c3e | \u7f85\u99ac\u7c3e  | \u767e\u8449\u7a97)"
+        "which": "[\u6709|\u6709\u6c92\u6709]\u54ea[\u4e00](\u500b|\u4e9b|\u6247|\u76de|\u9053)",
+        "window": "(\u7a97\u6236|\u7a97\u7c3e|\u6372\u7c3e|\u7f85\u99ac\u7c3e|\u767e\u8449\u7a97)"
     },
     "intents": {
         "HassGetState": {
             "data": [
                 {
                     "requires_context": {
                         "device_class": "battery",
@@ -785,14 +785,24 @@
                     ],
                     "slots": {
                         "domain": "fan",
                         "name": "all"
                     }
                 },
                 {
+                    "response": "fans_area",
+                    "sentences": [
+                        "[<let>]<area>(\u98a8\u6247|\u540a\u6247)<turn_on>"
+                    ],
+                    "slots": {
+                        "domain": "fan",
+                        "name": "all"
+                    }
+                },
+                {
                     "requires_context": {
                         "domain": "lock"
                     },
                     "response": "lock",
                     "sentences": [
                         "(\u95dc\u4e0a|\u95dc\u9589|\u4e0a\u9396|\u9396\u4e0a)[<area>]<name>"
                     ]
@@ -837,18 +847,20 @@
                     "slots": {
                         "domain": "script"
                     }
                 },
                 {
                     "excludes_context": {
                         "domain": [
+                            "binary_sensor",
                             "cover",
+                            "lock",
                             "scene",
-                            "sensor",
-                            "script"
+                            "script",
+                            "sensor"
                         ]
                     },
                     "sentences": [
                         "<turn_on> [<area>] <name>[(<light>|<switch>)]",
                         "[<let>][<area>]<name>[(<light>|<switch>)]<turn_on>"
                     ]
                 }
@@ -1079,19 +1091,19 @@
                     "out": "off"
                 }
             ]
         },
         "bs_presence_states": {
             "values": [
                 {
-                    "in": "(\u5728\u5bb6|\u5728\u5834)",
+                    "in": "(\u5728\u5bb6|\u5728\u5834|\u6709\u4eba)",
                     "out": "on"
                 },
                 {
-                    "in": "(\u96e2\u5bb6|\u4e0d\u5728\u5834)",
+                    "in": "(\u96e2\u5bb6|\u4e0d\u5728\u5834|\u6c92\u4eba)",
                     "out": "off"
                 }
             ]
         },
         "bs_problem_states": {
             "values": [
                 {
@@ -1239,67 +1251,67 @@
                     "out": "brown"
                 }
             ]
         },
         "cover_classes": {
             "values": [
                 {
-                    "in": "(\u906e\u967d\u68da | \u906e\u96e8\u68da | \u96e8\u68da)",
+                    "in": "(\u906e\u967d\u68da|\u906e\u96e8\u68da|\u96e8\u68da)",
                     "out": "awning"
                 },
                 {
-                    "in": "(\u7a97\u7c3e | \u767e\u8449\u7a97 | \u7f85\u99ac\u7c3e | \u6372\u7c3e)",
+                    "in": "(\u7a97\u7c3e|\u767e\u8449\u7a97|\u7f85\u99ac\u7c3e|\u6372\u7c3e|\u7d17\u7c3e|\u9580\u7c3e|\u906e\u5149\u7c3e)",
                     "out": "blind"
                 },
                 {
-                    "in": "(\u7a97\u7c3e | \u767e\u8449\u7a97 | \u7f85\u99ac\u7c3e | \u6372\u7c3e)",
+                    "in": "(\u7a97\u7c3e|\u767e\u8449\u7a97|\u7f85\u99ac\u7c3e|\u6372\u7c3e|\u7d17\u7c3e|\u9580\u7c3e|\u906e\u5149\u7c3e)",
                     "out": "curtain"
                 },
                 {
-                    "in": "(\u9580 | \u623f\u9593\u9580 | \u623f\u9580)",
+                    "in": "(\u9580|\u623f\u9593\u9580|\u623f\u9580)",
                     "out": "door"
                 },
                 {
-                    "in": "(\u8eca\u5eab\u9580 | \u8eca\u5eab)",
+                    "in": "(\u8eca\u5eab\u9580|\u8eca\u5eab)",
                     "out": "garage"
                 },
                 {
                     "in": "\u5927\u9580",
                     "out": "gate"
                 },
                 {
-                    "in": "(\u906e\u967d\u68da | \u906e\u96e8\u68da | \u96e8\u68da)",
+                    "in": "(\u906e\u967d\u68da|\u906e\u96e8\u68da|\u96e8\u68da)",
                     "out": "shade"
                 },
                 {
-                    "in": "(\u7a97\u7c3e | \u767e\u8449\u7a97 | \u7f85\u99ac\u7c3e | \u6372\u7c3e)",
+                    "in": "(\u7a97\u7c3e|\u767e\u8449\u7a97|\u7f85\u99ac\u7c3e|\u6372\u7c3e|\u7d17\u7c3e|\u9580\u7c3e|\u906e\u5149\u7c3e)",
                     "out": "shutter"
                 },
                 {
-                    "in": "(\u7a97\u6236 | \u843d\u5730\u7a97 | \u92c1\u7a97)",
+                    "in": "(\u7a97\u6236|\u843d\u5730\u7a97|\u92c1\u7a97)",
                     "out": "window"
                 }
             ]
         },
         "cover_states": {
             "values": [
                 {
-                    "in": "(\u958b\u555f | \u6253\u958b | \u958b\u8457 | \u958b) [\u7684]",
+                    "in": "(\u958b\u555f|\u6253\u958b|\u958b\u8457|\u958b)[\u7684]",
                     "out": "open"
                 },
                 {
-                    "in": "(\u95dc\u9589 | \u95dc\u4e0a | \u95dc\u8457 | \u95dc) [\u7684]",
+                    "in": "(\u95dc\u9589|\u95dc\u4e0a|\u95dc\u8457|\u95dc)[\u7684]",
                     "out": "closed"
                 },
                 {
-                    "in": "(\u958b\u555f\u4e2d | \u6253\u958b\u4e2d | \u6b63\u5728\u958b\u555f | \u6b63\u5728\u6253\u958b)",
+                    "in": "(\u958b\u555f\u4e2d|\u6253\u958b\u4e2d|\u6b63\u5728\u958b\u555f|\u6b63\u5728\u6253\u958b|\u6b63\u6253\u958b)",
                     "out": "opening"
                 },
                 {
-                    "in": "(\u95dc\u9589\u4e2d | \u95dc\u9589\u4e2d | \u6b63\u5728\u95dc\u9589 | \u6b63\u5728\u95dc\u4e0a)",
+                    "in": "(\u95dc\u9589\u4e2d|\u6b63\u5728\u95dc\u9589|\u6b63\u5728\u95dc\u4e0a|\u6b63\u95dc\u4e0a)",
                     "out": "closing"
                 }
             ]
         },
         "lock_states": {
             "values": [
                 {
@@ -1311,96 +1323,96 @@
                     "out": "unlocked"
                 }
             ]
         },
         "on_off_domains": {
             "values": [
                 {
-                    "in": "(\u71c8 | \u7167\u660e | \u684c\u71c8 | \u6aaf\u71c8 | \u5e8a\u982d\u71c8 | \u58c1\u71c8 | \u5438\u9802\u71c8 | \u5d01\u71c8) [\u7684]",
+                    "in": "(\u71c8|\u7167\u660e|\u684c\u71c8|\u6aaf\u71c8|\u5e8a\u982d\u71c8|\u58c1\u71c8|\u5438\u9802\u71c8|\u5d01\u71c8|\u5d4c\u71c8)[\u7684]",
                     "out": "light"
                 },
                 {
-                    "in": "(\u96fb\u6247 | \u96fb\u98a8\u6247 | \u98a8\u6247 | \u5faa\u74b0\u6247 | \u540a\u6247)",
+                    "in": "(\u96fb\u6247|\u96fb\u98a8\u6247|\u98a8\u6247|\u5faa\u74b0\u6247|\u540a\u6247|\u58c1\u639b\u6247|\u58c1\u6247|\u639b\u6247)",
                     "out": "fan"
                 },
                 {
-                    "in": "(\u958b\u95dc | \u96fb\u6e90 | \u63d2\u5ea7 | \u7e3d\u958b\u95dc | \u71c8\u5149)",
+                    "in": "(\u958b\u95dc|\u96fb\u6e90|\u63d2\u5ea7|\u7e3d\u958b\u95dc|\u71c8\u5149)",
                     "out": "switch"
                 }
             ]
         },
         "on_off_states": {
             "values": [
                 {
-                    "in": "(\u958b\u555f | \u6253\u958b | \u958b) [\u7684]",
+                    "in": "(\u958b\u555f|\u6253\u958b|\u958b)[\u7684]",
                     "out": "on"
                 },
                 {
-                    "in": "(\u95dc\u9589 | \u95dc\u4e0a | \u95dc) [\u7684]",
+                    "in": "(\u95dc\u9589|\u95dc\u4e0a|\u95dc)[\u7684]",
                     "out": "off"
                 }
             ]
         },
         "temperature": {
             "range": {
                 "from": 0,
                 "to": 100,
                 "type": "temperature"
             }
         },
         "temperature_unit": {
             "values": [
                 {
-                    "in": "\u5ea6C|\u651d\u6c0f\u5ea6|\u5ea6",
+                    "in": "(\u5ea6C|\u651d\u6c0f\u5ea6|\u5ea6|\u00b0C)",
                     "out": "celsius"
                 },
                 {
-                    "in": "\u5ea6F|\u83ef\u6c0f\u5ea6",
+                    "in": "(\u5ea6F|\u83ef\u6c0f\u5ea6|\u5ea6|\u00b0F)",
                     "out": "fahrenheit"
                 }
             ]
         }
     },
     "responses": {
         "errors": {
-            "handle_error": "\u8655\u7406\u60a8\u7684\u65e8\u610f\u6642\uff0c\u767c\u751f\u4e86\u610f\u5916\u932f\u8aa4",
-            "no_area": "\u300c{{ area }}\u300d\u9019\u500b\u5340\u57df\u4e26\u4e0d\u5b58\u5728",
+            "handle_error": "\u8655\u7406\u60a8\u7684\u6307\u4ee4\u6642\uff0c\u767c\u751f\u4e86\u610f\u5916\u932f\u8aa4",
+            "no_area": "\u300c{{ area }}\u300d\u9019\u500b\u5206\u5340\u4e26\u4e0d\u5b58\u5728",
             "no_device_class": "{{ area }}\u88e1\u9762\u4e26\u6c92\u6709\u4efb\u4f55{{ device_class }}",
             "no_domain": "{{ area }}\u88e1\u9762\u6c92\u6709\u4efb\u4f55{{ domain }}",
             "no_entity": "\u300c{{ entity }}\u300d\u9019\u500b\u5be6\u9ad4\u4e26\u4e0d\u5b58\u5728",
-            "no_intent": "\u62cd\u8b1d\uff0c\u6211\u6c92\u807d\u5f88\u61c2"
+            "no_intent": "\u62b1\u6b49\uff0c\u6211\u6c92\u807d\u61c2"
         },
         "intents": {
             "HassGetState": {
                 "all": "{% if not query.unmatched: %}\n  \u662f\u7684\n{% else %}\n  {% set no_match = query.unmatched | map(attribute=\"name\") | sort | list %}\n  {% if no_match | length > 4 %}\n    \u6c92\u6709\u3001{{ no_match[:3]|join(\"\u3001\") }}\u53ca\u53e6\u5916{{ (no_match|length - 3) }}\u500b\u4e0d\u662f\n  {%- else -%}\n    \u6c92\u6709\u3001{% for name in no_match -%}{% if not loop.first and not loop.last %}\u3001{% elif loop.last and not loop.first %}\u53ca{% endif -%}{{ name }}{%- endfor %}\u4e0d\u662f\n  {% endif %}\n{% endif %}\n",
                 "any": "{% if query.matched %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match|length > 4 %}\n    \u662f\u7684\u3001{{ match[:3]|join(\"\u3001\") }}\u53ca\u53e6\u5916{{ (match|length - 3) }}\u500b\n  {%- else -%}\n    \u662f\u7684\u3001{% for name in match -%}{% if not loop.first and not loop.last %}\u3001{% elif loop.last and not loop.first %}\u53ca{% endif -%}{{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% else %}\n  \u6c92\u6709\n{% endif %}\n",
                 "how_many": "{{ query.matched | length }}\n",
                 "one": "{{ slots.name | capitalize }}\u70ba {{ state.state_with_unit }}\n",
                 "one_yesno": "{% if query.matched: %}\n  \u662f\u7684\n{% else: %}\n  \u6c92\u6709\u3001{{ slots.name }}\u662f{{ state.state_with_unit }}\u7684\n{% endif %}\n",
                 "which": "{% if not query.matched %}\n  \u6c92\u6709\u4efb\u4f55\n{% else: %}\n  {% set match = query.matched | map(attribute=\"name\") | sort | list %}\n  {% if match | length > 4 %}\n    {{ match[:3]|join(\"\u3001\") }}\u53ca\u53e6\u5916{{ (match | length - 3) }}\u500b\n  {% else %}\n    {%- for name in match -%}\n      {% if not loop.first and not loop.last %}\u3001{% elif loop.last and not loop.first %}\u53ca{% endif -%}\n      {{ name }}\n    {%- endfor -%}\n  {% endif %}\n{% endif %}\n"
             },
             "HassTurnOff": {
-                "cover": "\u5df2\u95dc\u9589",
-                "cover_device_class": "{{ slots.device_class }}\u5df2\u95dc\u9589",
-                "default": "{{ state.domain }}\u5df2\u95dc\u9589",
+                "cover": "{{ slots.name|default('') }}\u5df2\u95dc\u9589",
+                "cover_device_class": "{{ slots.area|default('') }}{{ slots.device_class }}\u5df2\u95dc\u9589",
+                "default": "{{ slots.name|default('') }}\u5df2\u95dc\u9589",
                 "fan_all": "\u6240\u6709\u98a8\u6247\u5df2\u95dc\u9589",
-                "fans_area": "\u98a8\u6247\u5df2\u95dc\u9589",
+                "fans_area": "{{ slots.area }}\u98a8\u6247\u5df2\u95dc\u9589",
                 "light_all": "\u6240\u6709\u71c8\u5149\u5df2\u95dc\u9589",
-                "lights_area": "\u71c8\u5149\u5df2\u95dc\u9589",
-                "lock": "\u5df2\u89e3\u9396"
+                "lights_area": "{{ slots.area }}\u71c8\u5149\u5df2\u95dc\u9589",
+                "lock": "{{ slots.name|default('') }}\u5df2\u89e3\u9396"
             },
             "HassTurnOn": {
-                "cover": "\u5df2\u6253\u958b",
-                "cover_device_class": "{{ slots.device_class }}\u5df2\u6253\u958b",
-                "default": "{{ state.domain }}\u5df2\u6253\u958b",
-                "fans_area": "\u98a8\u6247\u5df2\u6253\u958b",
-                "lights_area": "\u71c8\u5149\u5df2\u6253\u958b",
-                "lock": "\u5df2\u4e0a\u9396",
-                "scene": "\u5df2\u555f\u7528",
-                "script": "\u5df2\u958b\u59cb"
+                "cover": "{{ slots.name|default('') }}\u5df2\u6253\u958b",
+                "cover_device_class": "{{ slots.area|default('') }}{{ slots.device_class }}\u5df2\u6253\u958b",
+                "default": "{{ slots.name|default('') }}\u5df2\u6253\u958b",
+                "fans_area": "{{ slots.area }}\u98a8\u6247\u5df2\u6253\u958b",
+                "lights_area": "{{ slots.area }}\u71c8\u5149\u5df2\u6253\u958b",
+                "lock": "{{ slots.name|default('') }}\u5df2\u4e0a\u9396",
+                "scene": "{{ slots.name|default('') }}\u5df2\u555f\u7528",
+                "script": "{{ slots.name|default('') }}\u5df2\u958b\u59cb"
             }
         }
     },
     "settings": {
         "ignore_whitespace": true
     },
     "skip_words": [
```

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/ar.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/ar.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/bg.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/bg.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/ca.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/ca.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/cs.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/cs.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/da.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/da.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/de-CH.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/de-CH.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/de.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/de.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9635416666666666%*

 * *Differences: {"'intents'": "{'HassLightSet': {'data': {1: {'response': 'brightness'}, 3: {'response': "*

 * *              "'color'}}}}",*

 * * "'responses'": "{'intents': {'HassLightSet': {'brightness': 'Helligkeit eingestellt', 'color': "*

 * *                "'Farbe eingestellt', delete: ['brightness_area', 'color_area']}}}"}*

```diff
@@ -8,15 +8,15 @@
                         "<setzen> [die] Helligkeit von <name> auf <brightness> [ein]",
                         "[die] Helligkeit von <name> auf <brightness> <setzen>",
                         "dimme [[die] Helligkeit [von] der] <name> [auf|zu] <brightness>",
                         "<name> [auf|zu] <brightness> dimmen"
                     ]
                 },
                 {
-                    "response": "brightness_area",
+                    "response": "brightness",
                     "sentences": [
                         "<setzen> [die] Helligkeit [<lichter>|<alle_lichter>] [<area>] auf <brightness> [ein]",
                         "[die] Helligkeit [<lichter>|<alle_lichter>] [<area>] auf <brightness> <setzen>",
                         "dimme [<lichter>|<alle_lichter>] [<area>] [auf|zu] <brightness>",
                         "[<lichter>|<alle_lichter>] [<area>] [auf|zu] <brightness> dimmen"
                     ]
                 },
@@ -26,28 +26,26 @@
                         "<setzen> [die Farbe (von|[von] der)] <name> [auf|zu] {color}",
                         "[die Farbe (von|[von] der)] <name> auf {color} <setzen>",
                         "Lass[e] <name> {color} [er]leuchten",
                         "<name> {color} [er]leuchten lassen"
                     ]
                 },
                 {
-                    "response": "color_area",
+                    "response": "color",
                     "sentences": [
                         "<setzen> die Farbe [<lichter>|<alle_lichter>] [<area>] auf {color}",
                         "die Farbe [<lichter>|<alle_lichter>] [<area>] auf {color} <setzen>"
                     ]
                 }
             ]
         }
     },
     "language": "de",
     "responses": {
         "intents": {
             "HassLightSet": {
-                "brightness": "{{ slots.name }} Helligkeit auf {{ slots.brightness }} gesetzt",
-                "brightness_area": "Helligkeit in {{ slots.area }} auf {{ slots.brightness }} gesetzt",
-                "color": "{{ slots.name }} Farbe auf {{ slots.color }} gesetzt",
-                "color_area": "Farbe in {{ slots.area }} auf {{ slots.color }} gesetzt"
+                "brightness": "Helligkeit eingestellt",
+                "color": "Farbe eingestellt"
             }
         }
     }
 }
```

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/en.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/en.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/es.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/es.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/fi.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/fi.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/fr-CA.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/fr-CA.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/fr.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/pl.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7881944444444445%*

 * *Differences: {"'intents'": "{'HassLightSet': {'data': {1: {'sentences': ['<set> [jasność] <area> na "*

 * *              "<brightness>']}, 2: {'sentences': ['<set> [kolor] <name> na {color}'], 'response': "*

 * *              "'color'}, 3: {'sentences': ['<set> [wszystkie kolory|kolory] <area> na {color}']}, "*

 * *              "insert: [(0, OrderedDict([('sentences', ['<set> [jasność] <name> na "*

 * *              "<brightness>']), ('response', 'brightness')]))], delete: [2]}}}",*

 * * "'language'": "'pl'",*

 * * "'responses'": "{'intents': {'Has […]*

```diff
@@ -1,49 +1,46 @@
 {
     "intents": {
         "HassLightSet": {
             "data": [
                 {
+                    "response": "brightness",
+                    "sentences": [
+                        "<set> [jasno\u015b\u0107] <name> na <brightness>"
+                    ]
+                },
+                {
                     "response": "brightness_area",
                     "sentences": [
-                        "<regle> [toutes] <lumieres> <dans> <area> \u00e0 <brightness>"
+                        "<set> [jasno\u015b\u0107] <area> na <brightness>"
                     ],
                     "slots": {
                         "name": "all"
                     }
                 },
                 {
-                    "response": "brightness_area",
+                    "response": "color",
                     "sentences": [
-                        "<regle> <name> <dans> <area> \u00e0 <brightness>"
+                        "<set> [kolor] <name> na {color}"
                     ]
                 },
                 {
                     "response": "color_area",
                     "sentences": [
-                        "<regle> [la couleur] [de | des] [toutes] <lumieres> <dans> <area> [avec la couleur | de couleur | en] {color}"
-                    ],
-                    "slots": {
-                        "name": "all"
-                    }
-                },
-                {
-                    "response": "color_area",
-                    "sentences": [
-                        "<regle> [la couleur de] <name> <dans> <area> [avec la couleur | de couleur | en] {color}"
+                        "<set> [wszystkie kolory|kolory] <area> na {color}"
                     ]
                 }
             ]
         }
     },
-    "language": "fr",
+    "language": "pl",
     "responses": {
         "intents": {
             "HassLightSet": {
-                "brightness": "Luminosit\u00e9 de {{ slots.name }} r\u00e9gl\u00e9e sur {{ slots.brightness }}",
-                "brightness_area": "Luminosit\u00e9 de {{ slots.area }} r\u00e9gl\u00e9e sur {{ slots.brightness }}",
-                "color": "Couleur de {{ slots.name }} r\u00e9gl\u00e9e en {{ slots.color }}",
-                "color_area": "Couleur de {{ slots.area }} r\u00e9gl\u00e9e en {{ slots.color }}"
+                "brightness": "Ustawiono jasno\u015b\u0107 {{ slots.name }} na {{ slots.brightness }}",
+                "brightness_area": "Ustawiono jasno\u015b\u0107 w {{ slots.area }} na {{ slots.brightness }}",
+                "color": "Ustawiono kolor {{ slots.name }} na {{ slots.color }}",
+                "color_area": "Ustawiono kolor w {{ slots.area }} na {{ slots.color }}"
             }
         }
     }
 }
```

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/gl.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/gl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/he.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/he.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/hr.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/hr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/hu.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/hu.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/id.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/id.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/it.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/it.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/ka.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/ka.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/lb.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/lb.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/lt.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/lt.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/lv.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/lv.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/ml.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/ml.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/ms.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/ms.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/nb.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/nb.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/nl.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/nl.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/pl.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/zh-tw.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7847222222222222%*

 * *Differences: {"'intents'": "{'HassLightSet': {'data': {2: {'sentences': "*

 * *              "['<let><name>[(燈|燈光)][亮度]<set_to>{brightness_level:brightness}', "*

 * *              "'<set><name>[(燈|燈光)][亮度][<to>]{brightness_level:brightness}'], 'requires_context': "*

 * *              "OrderedDict([('domain', 'light')])}, 3: {'sentences': "*

 * *              "['<let><area>[(照明|燈光)][亮度]<set_to>{brightness_level:brightness}', "*

 * *              "'<set><area>[(照明|燈光)][亮度][<to>]{brightness_level:brightness}'], 'response': "*

 * *              "'bright […]*

```diff
@@ -1,46 +1,79 @@
 {
     "intents": {
         "HassLightSet": {
             "data": [
                 {
+                    "requires_context": {
+                        "domain": "light"
+                    },
                     "response": "brightness",
                     "sentences": [
-                        "<set> [jasno\u015b\u0107] <name> na <brightness>"
+                        "[<let>]<name>[(\u71c8|\u71c8\u5149)][\u4eae\u5ea6]<set_to><brightness>",
+                        "<set><name>[(\u71c8|\u71c8\u5149)][\u4eae\u5ea6]<to><brightness>"
                     ]
                 },
                 {
-                    "response": "brightness_area",
+                    "response": "brightness",
                     "sentences": [
-                        "<set> [jasno\u015b\u0107] <area> na <brightness>"
+                        "<let><area>[(\u7167\u660e|\u71c8\u5149)][\u4eae\u5ea6]<set_to><brightness>",
+                        "<set><area>[(\u7167\u660e|\u71c8\u5149)][\u4eae\u5ea6][<to>]<brightness>"
                     ],
                     "slots": {
                         "name": "all"
                     }
                 },
                 {
-                    "response": "color",
+                    "requires_context": {
+                        "domain": "light"
+                    },
+                    "response": "brightness",
                     "sentences": [
-                        "<set> [kolor] <name> na {color}"
+                        "<let><name>[(\u71c8|\u71c8\u5149)][\u4eae\u5ea6]<set_to>{brightness_level:brightness}",
+                        "<set><name>[(\u71c8|\u71c8\u5149)][\u4eae\u5ea6][<to>]{brightness_level:brightness}"
                     ]
                 },
                 {
-                    "response": "color_area",
+                    "response": "brightness",
+                    "sentences": [
+                        "<let><area>[(\u7167\u660e|\u71c8\u5149)][\u4eae\u5ea6]<set_to>{brightness_level:brightness}",
+                        "<set><area>[(\u7167\u660e|\u71c8\u5149)][\u4eae\u5ea6][<to>]{brightness_level:brightness}"
+                    ],
+                    "slots": {
+                        "name": "all"
+                    }
+                },
+                {
+                    "requires_context": {
+                        "domain": "light"
+                    },
+                    "response": "color",
                     "sentences": [
-                        "<set> [wszystkie kolory|kolory] <area> na {color}"
+                        "<let><name>[(\u7167\u660e|\u71c8\u5149)][(\u984f\u8272|\u8272\u6eab)][<set_to>]{color}",
+                        "<set><name>[(\u7167\u660e|\u71c8\u5149)][(\u984f\u8272|\u8272\u6eab)]<to>{color}"
                     ]
+                },
+                {
+                    "response": "color",
+                    "sentences": [
+                        "<let><area>[(\u7167\u660e|\u71c8\u5149)][(\u984f\u8272|\u8272\u6eab)][<set_to>]{color}",
+                        "<set><area>[(\u7167\u660e|\u71c8\u5149)][(\u984f\u8272|\u8272\u6eab)]<to>{color}"
+                    ],
+                    "slots": {
+                        "name": "all"
+                    }
                 }
             ]
         }
     },
-    "language": "pl",
+    "language": "zh-tw",
     "responses": {
         "intents": {
             "HassLightSet": {
-                "brightness": "Ustawiono jasno\u015b\u0107 {{ slots.name }} na {{ slots.brightness }}",
-                "brightness_area": "Ustawiono jasno\u015b\u0107 w {{ slots.area }} na {{ slots.brightness }}",
-                "color": "Ustawiono kolor {{ slots.name }} na {{ slots.color }}",
-                "color_area": "Ustawiono kolor w {{ slots.area }} na {{ slots.color }}"
+                "brightness": "{{ slots.name }}\u4eae\u5ea6\u5df2\u8abf\u6574",
+                "brightness_area": "{{ slots.area }}\u4eae\u5ea6\u5df2\u8abf\u6574\u70ba{{ slots.brightness }}",
+                "color": "{{ slots.area }}\u984f\u8272\u5df2\u8abf\u6574",
+                "color_area": "{{ slots.area }}\u984f\u8272\u5df2\u8abf\u6574\u70ba{{ slots.color }}"
             }
         }
     }
 }
```

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/pt.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/pt.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/ro.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/ro.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/ru.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/ru.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/sk.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/sk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/sr.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/sr.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/sv.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/sv.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/uk.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/uk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/ur.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/ur.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/vi.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/vi.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/zh-cn.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/zh-cn.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/data/light/zh-hk.json` & `home-assistant-intents-2023.5.30/home_assistant_intents/data/light/zh-hk.json`

 * *Files identical despite different names*

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents/domains.py` & `home-assistant-intents-2023.5.30/home_assistant_intents/domains.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         "hr",
         "hu",
         "id",
         "is",
         "it",
         "ka",
         "kn",
+        "ko",
         "lb",
         "lt",
         "lv",
         "ml",
         "mn",
         "ms",
         "nb",
@@ -76,14 +77,15 @@
         "hr",
         "hu",
         "id",
         "is",
         "it",
         "ka",
         "kn",
+        "ko",
         "lb",
         "lt",
         "lv",
         "ml",
         "mn",
         "ms",
         "nb",
```

### Comparing `home-assistant-intents-2023.4.26/home_assistant_intents.egg-info/SOURCES.txt` & `home-assistant-intents-2023.5.30/home_assistant_intents.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 home_assistant_intents/data/homeassistant/hr.json
 home_assistant_intents/data/homeassistant/hu.json
 home_assistant_intents/data/homeassistant/id.json
 home_assistant_intents/data/homeassistant/is.json
 home_assistant_intents/data/homeassistant/it.json
 home_assistant_intents/data/homeassistant/ka.json
 home_assistant_intents/data/homeassistant/kn.json
+home_assistant_intents/data/homeassistant/ko.json
 home_assistant_intents/data/homeassistant/lb.json
 home_assistant_intents/data/homeassistant/lt.json
 home_assistant_intents/data/homeassistant/lv.json
 home_assistant_intents/data/homeassistant/ml.json
 home_assistant_intents/data/homeassistant/mn.json
 home_assistant_intents/data/homeassistant/ms.json
 home_assistant_intents/data/homeassistant/nb.json
@@ -83,14 +84,15 @@
 home_assistant_intents/data/light/hr.json
 home_assistant_intents/data/light/hu.json
 home_assistant_intents/data/light/id.json
 home_assistant_intents/data/light/is.json
 home_assistant_intents/data/light/it.json
 home_assistant_intents/data/light/ka.json
 home_assistant_intents/data/light/kn.json
+home_assistant_intents/data/light/ko.json
 home_assistant_intents/data/light/lb.json
 home_assistant_intents/data/light/lt.json
 home_assistant_intents/data/light/lv.json
 home_assistant_intents/data/light/ml.json
 home_assistant_intents/data/light/mn.json
 home_assistant_intents/data/light/ms.json
 home_assistant_intents/data/light/nb.json
```

### Comparing `home-assistant-intents-2023.4.26/pyproject.toml` & `home-assistant-intents-2023.5.30/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "home-assistant-intents"
-version     = "2023.4.26"
+version     = "2023.5.30"
 license     = {text = "Apache-2.0"}
 description = "Intents for Home Assistant"
 readme      = "README.md"
 authors     = [
     {name = "The Home Assistant Authors", email = "hello@home-assistant.io"}
 ]
 keywords    = ["home", "assistant", "intent", "recognition"]
```

