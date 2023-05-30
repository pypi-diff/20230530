# Comparing `tmp/dcspy-2.0.0.tar.gz` & `tmp/dcspy-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcspy-2.0.0.tar", last modified: Wed May 17 11:21:43 2023, max compression
+gzip compressed data, was "dcspy-2.1.0.tar", last modified: Tue May 30 20:51:40 2023, max compression
```

## Comparing `dcspy-2.0.0.tar` & `dcspy-2.1.0.tar`

### file list

```diff
@@ -1,58 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 11:21:43.419128 dcspy-2.0.0/
--rw-rw-rw-   0        0        0      708 2023-05-17 11:16:07.000000 dcspy-2.0.0/.pre-commit-config.yaml
--rw-rw-rw-   0        0        0     9538 2023-05-17 11:16:07.000000 dcspy-2.0.0/CHANGELOG.md
--rw-rw-rw-   0        0        0     5348 2023-05-17 11:16:07.000000 dcspy-2.0.0/CODE_OF_CONDUCT.md
--rw-rw-rw-   0        0        0     4371 2023-05-17 11:16:07.000000 dcspy-2.0.0/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     1092 2023-05-17 11:16:07.000000 dcspy-2.0.0/LICENSE.md
--rw-rw-rw-   0        0        0       75 2023-05-17 11:16:07.000000 dcspy-2.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0    16889 2023-05-17 11:21:43.419128 dcspy-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4776 2023-05-17 11:16:07.000000 dcspy-2.0.0/README.md
--rw-rw-rw-   0        0        0      346 2023-05-17 11:16:07.000000 dcspy-2.0.0/SECURITY.md
-drwxrwxrwx   0        0        0        0 2023-05-17 11:21:43.403505 dcspy-2.0.0/dcspy/
--rw-rw-rw-   0        0        0     7792 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/G13.png
--rw-rw-rw-   0        0        0    11136 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/G15v1.png
--rw-rw-rw-   0        0        0    11673 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/G15v2.png
--rw-rw-rw-   0        0        0    13267 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/G19.png
--rw-rw-rw-   0        0        0    10850 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/G510.png
--rw-rw-rw-   0        0        0     4512 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/__init__.py
--rw-rw-rw-   0        0        0    54681 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/aircraft.py
--rw-rw-rw-   0        0        0      476 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/config.yaml
--rw-rw-rw-   0        0        0     6160 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/dcsbios.py
--rw-rw-rw-   0        0        0    23535 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/dcspy.ico
--rw-rw-rw-   0        0        0    35819 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/dcspy.png
--rw-rw-rw-   0        0        0    21792 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/dcspy_white.ico
--rw-rw-rw-   0        0        0    20420 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/falconded.ttf
--rw-rw-rw-   0        0        0      236 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/license.txt
--rw-rw-rw-   0        0        0     1235 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/log.py
--rw-rw-rw-   0        0        0     7433 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/logitech.py
--rw-rw-rw-   0        0        0        0 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/py.typed
--rw-rw-rw-   0        0        0     1312 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/run.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:21:43.403505 dcspy-2.0.0/dcspy/sdk/
--rw-rw-rw-   0        0        0     1409 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/sdk/__init__.py
--rw-rw-rw-   0        0        0     8629 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/sdk/lcd_sdk.py
--rw-rw-rw-   0        0        0     8069 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/sdk/led_sdk.py
--rw-rw-rw-   0        0        0     4318 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/starter.py
--rw-rw-rw-   0        0        0    41669 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/tk_gui.py
--rw-rw-rw-   0        0        0    12425 2023-05-17 11:16:07.000000 dcspy-2.0.0/dcspy/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:21:43.403505 dcspy-2.0.0/dcspy.egg-info/
--rw-rw-rw-   0        0        0    16889 2023-05-17 11:21:43.000000 dcspy-2.0.0/dcspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      969 2023-05-17 11:21:43.000000 dcspy-2.0.0/dcspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 11:21:43.000000 dcspy-2.0.0/dcspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2023-05-17 11:21:43.000000 dcspy-2.0.0/dcspy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      221 2023-05-17 11:21:43.000000 dcspy-2.0.0/dcspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-17 11:21:43.000000 dcspy-2.0.0/dcspy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1571 2023-05-17 11:21:42.000000 dcspy-2.0.0/file_version_info.txt
--rw-rw-rw-   0        0        0      535 2023-05-17 11:16:07.000000 dcspy-2.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      150 2023-05-17 11:16:07.000000 dcspy-2.0.0/requirements.txt
--rw-rw-rw-   0        0        0      298 2023-05-17 11:16:07.000000 dcspy-2.0.0/requirements_test.txt
--rw-rw-rw-   0        0        0     3760 2023-05-17 11:21:43.419128 dcspy-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0       73 2023-05-17 11:16:07.000000 dcspy-2.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-17 11:21:43.419128 dcspy-2.0.0/tests/
--rw-rw-rw-   0        0        0    23841 2023-05-17 11:16:07.000000 dcspy-2.0.0/tests/test_aircraft.py
--rw-rw-rw-   0        0        0      971 2023-05-17 11:16:07.000000 dcspy-2.0.0/tests/test_bios.py
--rw-rw-rw-   0        0        0     5193 2023-05-17 11:16:07.000000 dcspy-2.0.0/tests/test_dcsbios.py
--rw-rw-rw-   0        0        0     5476 2023-05-17 11:16:07.000000 dcspy-2.0.0/tests/test_lcd_sdk.py
--rw-rw-rw-   0        0        0     3905 2023-05-17 11:16:07.000000 dcspy-2.0.0/tests/test_led_sdk.py
--rw-rw-rw-   0        0        0     5559 2023-05-17 11:16:07.000000 dcspy-2.0.0/tests/test_logitech.py
--rw-rw-rw-   0        0        0     1321 2023-05-17 11:16:07.000000 dcspy-2.0.0/tests/test_starter.py
--rw-rw-rw-   0        0        0     8472 2023-05-17 11:16:07.000000 dcspy-2.0.0/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-30 20:51:40.716291 dcspy-2.1.0/
+-rw-rw-rw-   0        0        0     1092 2023-05-30 20:49:25.000000 dcspy-2.1.0/LICENSE.md
+-rw-rw-rw-   0        0        0     6298 2023-05-30 20:51:40.716291 dcspy-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4776 2023-05-30 20:49:25.000000 dcspy-2.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 20:51:40.700665 dcspy-2.1.0/dcspy/
+-rw-rw-rw-   0        0        0     7792 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/G13.png
+-rw-rw-rw-   0        0        0    11136 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/G15v1.png
+-rw-rw-rw-   0        0        0    11673 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/G15v2.png
+-rw-rw-rw-   0        0        0    13267 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/G19.png
+-rw-rw-rw-   0        0        0    10850 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/G510.png
+-rw-rw-rw-   0        0        0     4819 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/__init__.py
+-rw-rw-rw-   0        0        0    54818 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/aircraft.py
+-rw-rw-rw-   0        0        0      476 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/config.yaml
+-rw-rw-rw-   0        0        0     6139 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/dcsbios.py
+-rw-rw-rw-   0        0        0    21694 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/dcspy.ico
+-rw-rw-rw-   0        0        0    35819 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/dcspy.png
+-rw-rw-rw-   0        0        0    21614 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/dcspy_white.ico
+-rw-rw-rw-   0        0        0      236 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/license.txt
+-rw-rw-rw-   0        0        0     1235 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/log.py
+-rw-rw-rw-   0        0        0     7447 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/logitech.py
+-rw-rw-rw-   0        0        0        0 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/py.typed
+-rw-rw-rw-   0        0        0     1107 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/run.py
+drwxrwxrwx   0        0        0        0 2023-05-30 20:51:40.700665 dcspy-2.1.0/dcspy/sdk/
+-rw-rw-rw-   0        0        0     1464 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/sdk/__init__.py
+-rw-rw-rw-   0        0        0     8507 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/sdk/lcd_sdk.py
+-rw-rw-rw-   0        0        0     7924 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/sdk/led_sdk.py
+-rw-rw-rw-   0        0        0    31528 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/splash.png
+-rw-rw-rw-   0        0        0     4343 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/starter.py
+-rw-rw-rw-   0        0        0    43908 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/tk_gui.py
+-rw-rw-rw-   0        0        0    12457 2023-05-30 20:49:25.000000 dcspy-2.1.0/dcspy/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-30 20:51:40.700665 dcspy-2.1.0/dcspy.egg-info/
+-rw-rw-rw-   0        0        0     6298 2023-05-30 20:51:40.000000 dcspy-2.1.0/dcspy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      790 2023-05-30 20:51:40.000000 dcspy-2.1.0/dcspy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 20:51:40.000000 dcspy-2.1.0/dcspy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2023-05-30 20:51:40.000000 dcspy-2.1.0/dcspy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      343 2023-05-30 20:51:40.000000 dcspy-2.1.0/dcspy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-30 20:51:40.000000 dcspy-2.1.0/dcspy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3463 2023-05-30 20:49:25.000000 dcspy-2.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-30 20:51:40.716291 dcspy-2.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-30 20:51:40.716291 dcspy-2.1.0/tests/
+-rw-rw-rw-   0        0        0    18375 2023-05-30 20:49:25.000000 dcspy-2.1.0/tests/test_aircraft.py
+-rw-rw-rw-   0        0        0      971 2023-05-30 20:49:25.000000 dcspy-2.1.0/tests/test_bios.py
+-rw-rw-rw-   0        0        0     5197 2023-05-30 20:49:25.000000 dcspy-2.1.0/tests/test_dcsbios.py
+-rw-rw-rw-   0        0        0     4908 2023-05-30 20:49:25.000000 dcspy-2.1.0/tests/test_lcd_sdk.py
+-rw-rw-rw-   0        0        0     3586 2023-05-30 20:49:25.000000 dcspy-2.1.0/tests/test_led_sdk.py
+-rw-rw-rw-   0        0        0     7035 2023-05-30 20:49:25.000000 dcspy-2.1.0/tests/test_logitech.py
+-rw-rw-rw-   0        0        0     1323 2023-05-30 20:49:25.000000 dcspy-2.1.0/tests/test_starter.py
+-rw-rw-rw-   0        0        0     8585 2023-05-30 20:49:25.000000 dcspy-2.1.0/tests/test_utils.py
```

### Comparing `dcspy-2.0.0/LICENSE.md` & `dcspy-2.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dcspy-2.0.0/README.md` & `dcspy-2.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-[![image](https://img.shields.io/badge/pypi-v2.0.0-blue.svg)](https://pypi.org/project/dcspy/)
+[![image](https://img.shields.io/badge/pypi-v2.1.0-blue.svg)](https://pypi.org/project/dcspy/)
 [![Python CI](https://github.com/emcek/dcspy/actions/workflows/python-ci.yml/badge.svg?branch=master)](https://github.com/emcek/dcspy/actions/workflows/python-ci.yml)
 [![Coverage Status](https://coveralls.io/repos/github/emcek/dcspy/badge.svg?branch=master)](https://coveralls.io/github/emcek/dcspy?branch=master)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/5270a4fc2ba24261a3bfa7361150e8ff)](https://www.codacy.com/gh/emcek/dcspy/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=emcek/dcspy&amp;utm_campaign=Badge_Grade)
-[![License](https://img.shields.io/badge/Licence-MIT-blue.svg)](./LICENSE.md)
+[![License](https://img.shields.io/badge/License-MIT-blue.svg)](./LICENSE.md)
 [![Downloads](https://img.shields.io/github/downloads/emcek/dcspy/total?label=Downloads)](https://github.com/emcek/dcspy/releases)
 [![dcspy](https://snyk.io/advisor/python/dcspy/badge.svg)](https://snyk.io/advisor/python/dcspy)
 [![Patreon](https://img.shields.io/badge/Patreon-donate-ff424d?logo=patreon)](https://www.patreon.com/mplichta)
 [![Discord](https://img.shields.io/discord/672486999516774442?label=Discord&logo=discord&logoColor=lightblue)](https://discord.gg/SP5Yjx3)
 [![image](https://img.shields.io/badge/python-3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue.svg)](https://github.com/emcek/dcspy)
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/emcek/dcspy/master.svg)](https://results.pre-commit.ci/latest/github/emcek/dcspy/master)
 [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=emcek_dcspy&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=emcek_dcspy)
@@ -38,15 +38,15 @@
 * AV-8B Night Attack Harrier - Up Front Controller and Option Display Unit
 * AH-64D Apache - Enhanced Up Front Display
 * more to come....
 
 ## Requirements
 * [Logitech Gaming Software 9.04.49](https://support.logitech.com/software/lgs)
 * [DCS-BIOS 0.7.48](https://github.com/DCSFlightpanels/dcs-bios/releases/latest) or newer (can be installed directly from DCSpy)
-* DCS World: [2.8.4.39731](https://www.digitalcombatsimulator.com/en/news/changelog/openbeta/2.8.4.39731/) Open Beta (any release 2.8.* should work)
+* DCS World: [2.8.5.40170](https://www.digitalcombatsimulator.com/en/news/changelog/openbeta/2.8.5.40170/) Open Beta (any release 2.8.* should work)
 * (optional) [Python 3.11](https://www.python.org/downloads/) but 3.7+ should be fine (with tcl/tk support, see [installation](https://github.com/emcek/dcspy/wiki/installation))
 
 **Notes:**
 * If you upgrade DCSpy from 1.5.1 or older you can safely remove Logitech LCD SDK from `C:\Program Files\Logitech Gaming Software\LCDSDK_8.57.148`. Since DCSpy version 1.6.0 use built-in SDK in LGS (Logitech Gaming Software).
 
 ## New ideas
 I have lots of plans and new ideas how to improve it internally and form user's perspective, but don't hesitate to contact me. Maybe it will motivate me to implement some new stuff. Please open issue if you find bug or have any crazy idea.
```

### Comparing `dcspy-2.0.0/dcspy/G13.png` & `dcspy-2.1.0/dcspy/G13.png`

 * *Files identical despite different names*

### Comparing `dcspy-2.0.0/dcspy/G15v1.png` & `dcspy-2.1.0/dcspy/G15v1.png`

 * *Files identical despite different names*

### Comparing `dcspy-2.0.0/dcspy/G15v2.png` & `dcspy-2.1.0/dcspy/G15v2.png`

 * *Files identical despite different names*

### Comparing `dcspy-2.0.0/dcspy/G19.png` & `dcspy-2.1.0/dcspy/G19.png`

 * *Files identical despite different names*

### Comparing `dcspy-2.0.0/dcspy/G510.png` & `dcspy-2.1.0/dcspy/G510.png`

 * *Files identical despite different names*

### Comparing `dcspy-2.0.0/dcspy/__init__.py` & `dcspy-2.1.0/dcspy/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from dataclasses import dataclass
 from enum import Enum
 from logging import getLogger
 from os import name
 from pathlib import Path
-from platform import architecture, uname, python_implementation, python_version
+from platform import architecture, python_implementation, python_version, uname
 from sys import platform
-from typing import Union, Sequence
+from typing import Sequence, Tuple, Union
 
 from PIL import ImageFont
 
 from dcspy.log import config_logger
-from dcspy.sdk import lcd_sdk
-from dcspy.utils import load_cfg, set_defaults, get_default_yaml
+from dcspy.utils import get_default_yaml, load_cfg, set_defaults
+
 try:
     from typing import NotRequired
 except ImportError:
     from typing_extensions import NotRequired
 try:
     from typing import TypedDict
 except ImportError:
@@ -37,19 +37,31 @@
     'AV8BNA': {'name': 'AV-8B N/A Harrier', 'bios': 'AV8BNA'},
 }
 SEND_ADDR = ('127.0.0.1', 7778)
 RECV_ADDR = ('', 5010)
 MULTICAST_IP = '239.255.50.10'
 LOCAL_APPDATA = True
 
+# LCD types
+TYPE_MONO = 1
+TYPE_COLOR = 2
+
+# LCD Monochrome size
+MONO_WIDTH = 160
+MONO_HEIGHT = 43
+
+# LCD Color size
+COLOR_WIDTH = 320
+COLOR_HEIGHT = 240
+
 
 class LcdType(Enum):
     """LCD Type."""
-    MONO = lcd_sdk.TYPE_MONO
-    COLOR = lcd_sdk.TYPE_COLOR
+    MONO = TYPE_MONO
+    COLOR = TYPE_COLOR
 
 
 class LcdButton(Enum):
     """LCD Buttons."""
     NONE = 0x0
     ONE = 0x1
     TWO = 0x2
@@ -60,41 +72,47 @@
     OK = 0x400
     CANCEL = 0x800
     UP = 0x1000
     DOWN = 0x2000
     MENU = 0x4000
 
 
+class LcdMode(Enum):
+    """LCD Mode."""
+    BLACK_WHITE = '1'
+    TRUE_COLOR = 'RGBA'
+
+
 @dataclass
 class LcdInfo:
     """LCD info."""
     width: int
     height: int
     type: LcdType
     buttons: Sequence[LcdButton]
-    foreground: Union[int, Sequence[int]]
-    background: Union[int, Sequence[int]]
-    mode: str
+    foreground: Union[int, Tuple[int, int, int, int]]
+    background: Union[int, Tuple[int, int, int, int]]
+    mode: LcdMode
     font_xs: ImageFont.FreeTypeFont
     font_s: ImageFont.FreeTypeFont
     font_l: ImageFont.FreeTypeFont
 
 
 default_yaml = get_default_yaml(local_appdata=LOCAL_APPDATA)
 config = set_defaults(load_cfg(filename=default_yaml), filename=default_yaml)
-LcdMono = LcdInfo(width=lcd_sdk.MONO_WIDTH, height=lcd_sdk.MONO_HEIGHT, type=LcdType.MONO, foreground=255,
+LcdMono = LcdInfo(width=MONO_WIDTH, height=MONO_HEIGHT, type=LcdType.MONO, foreground=255,
                   buttons=(LcdButton.ONE, LcdButton.TWO, LcdButton.THREE, LcdButton.FOUR),
-                  background=0, mode='1', font_s=ImageFont.truetype(config['font_name'], config['font_mono_s']),
-                  font_l=ImageFont.truetype(config['font_name'], config['font_mono_l']),
-                  font_xs=ImageFont.truetype(config['font_name'], config['font_mono_xs']))
-LcdColor = LcdInfo(width=lcd_sdk.COLOR_WIDTH, height=lcd_sdk.COLOR_HEIGHT, type=LcdType.COLOR, foreground=(0, 255, 0, 255),
+                  background=0, mode=LcdMode.BLACK_WHITE, font_s=ImageFont.truetype(str(config['font_name']), int(config['font_mono_s'])),
+                  font_l=ImageFont.truetype(str(config['font_name']), int(config['font_mono_l'])),
+                  font_xs=ImageFont.truetype(str(config['font_name']), int(config['font_mono_xs'])))
+LcdColor = LcdInfo(width=COLOR_WIDTH, height=COLOR_HEIGHT, type=LcdType.COLOR, foreground=(0, 255, 0, 255),
                    buttons=(LcdButton.LEFT, LcdButton.RIGHT, LcdButton.UP, LcdButton.DOWN, LcdButton.OK, LcdButton.CANCEL, LcdButton.MENU),
-                   background=(0, 0, 0, 0), mode='RGBA', font_s=ImageFont.truetype(config['font_name'], config['font_color_s']),
-                   font_l=ImageFont.truetype(config['font_name'], config['font_color_l']),
-                   font_xs=ImageFont.truetype(config['font_name'], config['font_color_xs']))
+                   background=(0, 0, 0, 0), mode=LcdMode.TRUE_COLOR, font_s=ImageFont.truetype(str(config['font_name']), int(config['font_color_s'])),
+                   font_l=ImageFont.truetype(str(config['font_name']), int(config['font_color_l'])),
+                   font_xs=ImageFont.truetype(str(config['font_name']), int(config['font_color_xs'])))
 DED_FONT = ImageFont.truetype(str(Path(__file__).resolve().with_name('falconded.ttf')), 25)
 LCD_TYPES = {
     'G19': {'type': 'KeyboardColor', 'icon': 'G19.png'},
     'G510': {'type': 'KeyboardMono', 'icon': 'G510.png'},
     'G15 v1': {'type': 'KeyboardMono', 'icon': 'G15v1.png'},
     'G15 v2': {'type': 'KeyboardMono', 'icon': 'G15v2.png'},
     'G13': {'type': 'KeyboardMono', 'icon': 'G13.png'},
```

### Comparing `dcspy-2.0.0/dcspy/aircraft.py` & `dcspy-2.1.0/dcspy/aircraft.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from enum import Enum
-from functools import partial
 from itertools import chain, cycle
 from logging import getLogger
 from pathlib import Path
 from pprint import pformat
 from re import search, sub
 from string import whitespace
 from tempfile import gettempdir
-from typing import Dict, Union, Iterator, Sequence, List
+from typing import Dict, Iterator, List, Sequence, Tuple, Union
 
 from PIL import Image, ImageDraw, ImageFont
 
-from dcspy import LcdInfo, LcdButton, LcdType, SUPPORTED_CRAFTS, DED_FONT, config, BiosValue
+from dcspy import (DED_FONT, SUPPORTED_CRAFTS, BiosValue, LcdButton, LcdInfo,
+                   LcdType, config)
 from dcspy.sdk import lcd_sdk
 
-
 LOG = getLogger(__name__)
 
 
 class Aircraft:
     """Common Aircraft."""
     def __init__(self, lcd_type: LcdInfo) -> None:
         """
@@ -48,20 +47,16 @@
 
     def prepare_image(self) -> Image.Image:
         """
         Prepare image to be sent to correct type of LCD.
 
         :return: image instance ready display on LCD
         """
-        img_for_lcd = {'mono': partial(Image.new, mode='1', size=(self.lcd.width, self.lcd.height), color=self.lcd.background),
-                       'color': partial(Image.new, mode='RGBA', size=(self.lcd.width, self.lcd.height), color=self.lcd.background)}
-
-        lcd_type = self.lcd.type.name.lower()
-        img = img_for_lcd[lcd_type]()
-        getattr(self, f'draw_for_lcd_{lcd_type}')(img)
+        img = Image.new(mode=self.lcd.mode.value, size=(self.lcd.width, self.lcd.height), color=self.lcd.background)
+        getattr(self, f'draw_for_lcd_{self.lcd.type.name.lower()}')(img)
         if config.get('save_lcd', False):
             img.save(Path(gettempdir()) / f'{self.__class__.__name__}_{next(self._debug_img)}.png', 'PNG')
         return img
 
     def set_bios(self, selector: str, value: Union[str, int]) -> None:
         """
         Set value for DCS-BIOS selector.
@@ -144,15 +139,15 @@
             'IFEI_FUEL_DOWN': {'klass': 'StringBuffer', 'args': {'address': 0x748a, 'max_length': 6}, 'value': ''},
             'IFEI_FUEL_UP': {'klass': 'StringBuffer', 'args': {'address': 0x7490, 'max_length': 6}, 'value': ''},
             'HUD_ATT_SW': {'klass': 'IntegerBuffer', 'args': {'address': 0x742e, 'mask': 0x300, 'shift_by': 0x8}, 'value': int(), 'max_value': 2},
             'IFEI_DWN_BTN': {'klass': 'IntegerBuffer', 'args': {'address': 0x7466, 'mask': 0x10, 'shift_by': 0x4}, 'value': int(), 'max_value': 1},
             'IFEI_UP_BTN': {'klass': 'IntegerBuffer', 'args': {'address': 0x7466, 'mask': 0x8, 'shift_by': 0x3}, 'value': int(), 'max_value': 1}}
         self.cycle_buttons = {'HUD_ATT_SW': iter([0]), 'IFEI_DWN_BTN': iter([0]), 'IFEI_UP_BTN': iter([0])}
 
-    def _draw_common_data(self, draw: ImageDraw, scale: int) -> ImageDraw:
+    def _draw_common_data(self, draw: ImageDraw.ImageDraw, scale: int) -> ImageDraw.ImageDraw:
         """
         Draw common part (based on scale) for Mono and Color LCD.
 
         :param draw: ImageDraw instance
         :param scale: scaling factor (Mono 1, Color 2)
         :return: updated image to draw
         """
@@ -160,36 +155,36 @@
         scratch_2 = self.get_bios("UFC_SCRATCHPAD_STRING_2_DISPLAY")
         scratch_num = self.get_bios("UFC_SCRATCHPAD_NUMBER_DISPLAY")
         draw.text(xy=(0, 0), fill=self.lcd.foreground, font=self.lcd.font_l,
                   text=f'{scratch_1}{scratch_2}{scratch_num}')
         draw.line(xy=(0, 20 * scale, 115 * scale, 20 * scale), fill=self.lcd.foreground, width=1)
 
         draw.rectangle(xy=(0, 29 * scale, 20 * scale, 42 * scale), fill=self.lcd.background, outline=self.lcd.foreground)
-        draw.text(xy=(2 * scale, 29 * scale), text=self.get_bios('UFC_COMM1_DISPLAY'), fill=self.lcd.foreground, font=self.lcd.font_l)
+        draw.text(xy=(2 * scale, 29 * scale), text=str(self.get_bios('UFC_COMM1_DISPLAY')), fill=self.lcd.foreground, font=self.lcd.font_l)
 
         offset = 44 * scale
         draw.rectangle(xy=(139 * scale - offset, 29 * scale, 159 * scale - offset, 42 * scale), fill=self.lcd.background, outline=self.lcd.foreground)
-        draw.text(xy=(140 * scale - offset, 29 * scale), text=self.get_bios('UFC_COMM2_DISPLAY'), fill=self.lcd.foreground, font=self.lcd.font_l)
+        draw.text(xy=(140 * scale - offset, 29 * scale), text=str(self.get_bios('UFC_COMM2_DISPLAY')), fill=self.lcd.foreground, font=self.lcd.font_l)
 
         for i in range(1, 6):
             offset = (i - 1) * 8 * scale
             draw.text(xy=(120 * scale, offset), fill=self.lcd.foreground, font=self.lcd.font_s,
                       text=f'{i}{self.get_bios(f"UFC_OPTION_CUEING_{i}")}{self.get_bios(f"UFC_OPTION_DISPLAY_{i}")}')
 
-        draw.text(xy=(36 * scale, 29 * scale), text=self.get_bios('IFEI_FUEL_UP'), fill=self.lcd.foreground, font=self.lcd.font_l)
+        draw.text(xy=(36 * scale, 29 * scale), text=str(self.get_bios('IFEI_FUEL_UP')), fill=self.lcd.foreground, font=self.lcd.font_l)
         return draw
 
     def draw_for_lcd_mono(self, img: Image.Image) -> None:
         """Prepare image for F/A-18C Hornet for Mono LCD."""
         self._draw_common_data(draw=ImageDraw.Draw(img), scale=1)
 
     def draw_for_lcd_color(self, img: Image.Image) -> None:
         """Prepare image for F/A-18C Hornet for Color LCD."""
         draw = self._draw_common_data(draw=ImageDraw.Draw(img), scale=2)
-        draw.text(xy=(72, 100), text=self.get_bios('IFEI_FUEL_DOWN'), fill=self.lcd.foreground, font=self.lcd.font_l)
+        draw.text(xy=(72, 100), text=str(self.get_bios('IFEI_FUEL_DOWN')), fill=self.lcd.foreground, font=self.lcd.font_l)
 
     def set_bios(self, selector: str, value: Union[str, int]) -> None:
         """
         Set new data.
 
         :param selector:
         :param value:
@@ -251,24 +246,24 @@
             'DED_LINE_5': {'klass': 'StringBuffer', 'args': {'address': 0x4582, 'max_length': 29}, 'value': ''},
             'IFF_MASTER_KNB': {'klass': 'IntegerBuffer', 'args': {'address': 0x4450, 'mask': 0xe, 'shift_by': 0x1}, 'value': int(), 'max_value': 4},
             'IFF_ENABLE_SW': {'klass': 'IntegerBuffer', 'args': {'address': 0x4450, 'mask': 0x600, 'shift_by': 0x9}, 'value': int(), 'max_value': 2},
             'IFF_M4_CODE_SW': {'klass': 'IntegerBuffer', 'args': {'address': 0x4450, 'mask': 0x30, 'shift_by': 0x4}, 'value': int(), 'max_value': 2},
             'IFF_M4_REPLY_SW': {'klass': 'IntegerBuffer', 'args': {'address': 0x4450, 'mask': 0xc0, 'shift_by': 0x6}, 'value': int(), 'max_value': 2}}
         self.cycle_buttons = {'IFF_MASTER_KNB': iter([0]), 'IFF_ENABLE_SW': iter([0]), 'IFF_M4_CODE_SW': iter([0]), 'IFF_M4_REPLY_SW': iter([0])}
 
-    def _draw_common_data(self, draw: ImageDraw, separation: int) -> None:
+    def _draw_common_data(self, draw: ImageDraw.ImageDraw, separation: int) -> None:
         """
         Draw common part (based on scale) for Mono and Color LCD.
 
         :param draw: ImageDraw instance
         :param separation: between lines in pixels
         """
         for i in range(1, 6):
             offset = (i - 1) * separation
-            draw.text(xy=(0, offset), text=self.get_bios(f'DED_LINE_{i}'), fill=self.lcd.foreground, font=self.font)
+            draw.text(xy=(0, offset), text=str(self.get_bios(f'DED_LINE_{i}')), fill=self.lcd.foreground, font=self.font)
 
     def draw_for_lcd_mono(self, img: Image.Image) -> None:
         """Prepare image for F-16C Viper for Mono LCD."""
         self._draw_common_data(draw=ImageDraw.Draw(img), separation=8)
 
     def draw_for_lcd_color(self, img: Image.Image) -> None:
         """Prepare image for F-16C Viper for Color LCD."""
@@ -366,15 +361,15 @@
             'PVI_LINE2_TEXT': {'klass': 'StringBuffer', 'args': {'address': 0x192a, 'max_length': 6}, 'value': ''},
             'AP_ALT_HOLD_LED': {'klass': 'IntegerBuffer', 'args': {'address': 0x1936, 'mask': 0x8000, 'shift_by': 0xf}, 'value': int()},
             'AP_BANK_HOLD_LED': {'klass': 'IntegerBuffer', 'args': {'address': 0x1936, 'mask': 0x200, 'shift_by': 0x9}, 'value': int()},
             'AP_FD_LED': {'klass': 'IntegerBuffer', 'args': {'address': 0x1938, 'mask': 0x200, 'shift_by': 0x9}, 'value': int()},
             'AP_HDG_HOLD_LED': {'klass': 'IntegerBuffer', 'args': {'address': 0x1936, 'mask': 0x800, 'shift_by': 0xb}, 'value': int()},
             'AP_PITCH_HOLD_LED': {'klass': 'IntegerBuffer', 'args': {'address': 0x1936, 'mask': 0x2000, 'shift_by': 0xd}, 'value': int()}}
 
-    def _draw_common_data(self, draw: ImageDraw, scale: int) -> None:
+    def _draw_common_data(self, draw: ImageDraw.ImageDraw, scale: int) -> None:
         """
         Draw common part (based on scale) for Mono and Color LCD.
 
         :param draw: ImageDraw instance
         :param scale: scaling factor (Mono 1, Color 2)
         """
         for rect_xy in [
@@ -406,15 +401,15 @@
             l2_apostr1 = self.get_bios("PVI_LINE2_APOSTROPHE1")
             l2_apostr2 = self.get_bios("PVI_LINE2_APOSTROPHE2")
             text2 = f'{line2_text[-6:-3]}{l2_apostr1}{line2_text[-3:-1]}{l2_apostr2}{line2_text[-1]}'
         line1 = f'{self.get_bios("PVI_LINE1_SIGN")}{text1} {self.get_bios("PVI_LINE1_POINT")}'
         line2 = f'{self.get_bios("PVI_LINE2_SIGN")}{text2} {self.get_bios("PVI_LINE2_POINT")}'
         return line1, line2
 
-    def _auto_pilot_switch(self, draw_obj: ImageDraw, scale: int) -> None:
+    def _auto_pilot_switch(self, draw_obj: ImageDraw.ImageDraw, scale: int) -> None:
         """
         Draw rectangle and add text for autopilot channels in correct coordinates.
 
         :param draw_obj: ImageDraw object form PIL
         :param scale: scaling factor (Mono 1, Color 2)
         """
         for c_rect, c_text, ap_channel, turn_on in (
@@ -478,15 +473,15 @@
             'R863_CNL_SEL': {'klass': 'IntegerBuffer', 'args': {'address': 0x268c, 'mask': 0x1f, 'shift_by': 0x0}, 'value': int()},
             'R863_MOD': {'klass': 'IntegerBuffer', 'args': {'address': 0x263a, 'mask': 0x1000, 'shift_by': 0xc}, 'value': int()},
             'R863_FREQ': {'klass': 'StringBuffer', 'args': {'address': 0x2804, 'max_length': 7}, 'value': ''},
             'R828_PRST_CHAN_SEL': {'klass': 'IntegerBuffer', 'args': {'address': 0x268e, 'mask': 0x780, 'shift_by': 0x7}, 'value': int()},
             'YADRO1A_FREQ': {'klass': 'StringBuffer', 'args': {'address': 0x2692, 'max_length': 7}, 'value': ''},
         }
 
-    def _draw_common_data(self, draw: ImageDraw, scale: int) -> None:
+    def _draw_common_data(self, draw: ImageDraw.ImageDraw, scale: int) -> None:
         """
         Draw common part (based on scale) for Mono and Color LCD.
 
         :param draw: ImageDraw instance
         :param scale: scaling factor (Mono 1, Color 2)
         """
         for c_rect, c_text, ap_channel, turn_on in (
@@ -537,26 +532,26 @@
 
         :param lcd_type: LCD type
         """
         super().__init__(lcd_type)
         self.bios_data: Dict[str, BiosValue] = {
             'PLT_R863_CHAN': {'klass': 'IntegerBuffer', 'args': {'address': 0x69ec, 'mask': 0x3e0, 'shift_by': 0x5}, 'value': int()},
             'PLT_R863_MODUL': {'klass': 'IntegerBuffer', 'args': {'address': 0x69ec, 'mask': 0x2, 'shift_by': 0x1}, 'value': int()},
-            'PLT_R828_CHAN': {'klass': 'IntegerBuffer', 'args': {'address': 0x69fe, 'mask': 0xf00, 'shift_by': 0x8}, 'value': int()},
-            'JADRO_FREQ': {'klass': 'StringBuffer', 'args': {'address': 0x6a04, 'max_length': 7}, 'value': ''},
+            'PLT_R828_CHAN': {'klass': 'IntegerBuffer', 'args': {'address': 0x69fc, 'mask': 0xf00, 'shift_by': 0x8}, 'value': int()},
+            'JADRO_FREQ': {'klass': 'StringBuffer', 'args': {'address': 0x6a02, 'max_length': 7}, 'value': ''},
             'PLT_SAU_HOVER_MODE_ON_L': {'klass': 'IntegerBuffer', 'args': {'address': 0x68fc, 'mask': 0x8000, 'shift_by': 0xf}, 'value': int()},
             'PLT_SAU_ROUTE_MODE_ON_L': {'klass': 'IntegerBuffer', 'args': {'address': 0x68fc, 'mask': 0x2000, 'shift_by': 0xd}, 'value': int()},
             'PLT_SAU_ALT_MODE_ON_L': {'klass': 'IntegerBuffer', 'args': {'address': 0x6902, 'mask': 0x100, 'shift_by': 0x8}, 'value': int()},
             'PLT_SAU_H_ON_L': {'klass': 'IntegerBuffer', 'args': {'address': 0x68fc, 'mask': 0x80, 'shift_by': 0x7}, 'value': int()},
             'PLT_SAU_K_ON_L': {'klass': 'IntegerBuffer', 'args': {'address': 0x68fc, 'mask': 0x20, 'shift_by': 0x5}, 'value': int()},
             'PLT_SAU_T_ON_L': {'klass': 'IntegerBuffer', 'args': {'address': 0x68fc, 'mask': 0x800, 'shift_by': 0xb}, 'value': int()},
             'PLT_SAU_B_ON_L': {'klass': 'IntegerBuffer', 'args': {'address': 0x68fc, 'mask': 0x200, 'shift_by': 0x9}, 'value': int()},
         }
 
-    def _draw_common_data(self, draw: ImageDraw, scale: int) -> None:
+    def _draw_common_data(self, draw: ImageDraw.ImageDraw, scale: int) -> None:
         """
         Draw common part (based on scale) for Mono and Color LCD.
 
         :param draw: ImageDraw instance
         :param scale: scaling factor (Mono 1, Color 2)
         """
         for c_rect, c_text, ap_channel, turn_on in (
@@ -653,30 +648,30 @@
         if mode == 'pre':
             kwargs['xcords'] = [0] * 10
             kwargs['ycords'] = [j * 24 for j in range(0, 10)]
             kwargs['font'] = self.lcd.font_l
             del kwargs['scale']
         getattr(self, f'_draw_for_{mode}')(**kwargs)
 
-    def _draw_for_idm(self, draw: ImageDraw.Draw, scale: int):
+    def _draw_for_idm(self, draw: ImageDraw.ImageDraw, scale: int) -> None:
         """
         Draw image for IDM mode.
 
         :param draw: ImageDraw instance
         :param scale: scaling factor (Mono 1, Color 2)
         """
         for i in range(8, 13):
             offset = (i - 8) * 8 * scale
             mat = search(r'(.*\*)\s+(\d+)([.\dULCA]+)[-\sA-Z]*(\d+)([.\dULCA]+)[\s-]+', str(self.get_bios(f'PLT_EUFD_LINE{i}')))
             if mat:
                 spacer = ' ' * (6 - len(mat.group(3)))
                 text = f'{mat.group(1):>7}{mat.group(2):>4}{mat.group(3):5<}{spacer}{mat.group(4):>4}{mat.group(5):5<}'
                 draw.text(xy=(0, offset), text=text, fill=self.lcd.foreground, font=self.lcd.font_xs)
 
-    def _draw_for_wca(self, draw: ImageDraw.Draw, scale: int):
+    def _draw_for_wca(self, draw: ImageDraw.ImageDraw, scale: int) -> None:
         """
         Draw image for WCA mode.
 
         :param draw: ImageDraw instance
         :param scale: scaling factor (Mono 1, Color 2)
         """
         warnings = self._fetch_warning_list()
@@ -699,15 +694,15 @@
         warn = []
         for i in range(1, 8):
             mat = search(r'(.*)\|(.*)\|(.*)', str(self.get_bios(f'PLT_EUFD_LINE{i}')))
             if mat:
                 warn.extend([w for w in [mat.group(1).strip(), mat.group(2).strip(), mat.group(3).strip()] if w])
         return warn
 
-    def _draw_for_pre(self, draw: ImageDraw.Draw, xcords: List[int], ycords: List[int], font: ImageFont.FreeTypeFont):
+    def _draw_for_pre(self, draw: ImageDraw.ImageDraw, xcords: List[int], ycords: List[int], font: ImageFont.FreeTypeFont) -> None:
         """
         Draw image for PRE mode.
 
         :param draw: ImageDraw instance
         :param xcords: list of X coordinates
         :param ycords: list of Y coordinates
         :param font: font instance
@@ -856,15 +851,15 @@
         super().__init__(lcd_type)
         self.bios_data: Dict[str, BiosValue] = {
             'RIO_CAP_CLEAR': {'klass': 'IntegerBuffer', 'args': {'address': 0x12c4, 'mask': 0x4000, 'shift_by': 0xe}, 'value': int()},
             'RIO_CAP_SW': {'klass': 'IntegerBuffer', 'args': {'address': 0x12c4, 'mask': 0x2000, 'shift_by': 0xd}, 'value': int()},
             'RIO_CAP_NE': {'klass': 'IntegerBuffer', 'args': {'address': 0x12c4, 'mask': 0x1000, 'shift_by': 0xc}, 'value': int()},
             'RIO_CAP_ENTER': {'klass': 'IntegerBuffer', 'args': {'address': 0x12c4, 'mask': 0x8000, 'shift_by': 0xf}, 'value': int()}}
 
-    def _draw_common_data(self, draw: ImageDraw) -> None:
+    def _draw_common_data(self, draw: ImageDraw.ImageDraw) -> None:
         """
         Draw common part for Mono and Color LCD.
 
         :param draw: ImageDraw instance
         """
         draw.text(xy=(2, 3), text=f'{SUPPORTED_CRAFTS[self.__class__.__name__]["name"]}', fill=self.lcd.foreground, font=self.lcd.font_l)
 
@@ -923,30 +918,30 @@
             'AV8BNA_ODU_3_SELECT': {'klass': 'StringBuffer', 'args': {'address': 0x7972, 'max_length': 1}, 'value': ''},
             'AV8BNA_ODU_3_Text': {'klass': 'StringBuffer', 'args': {'address': 0x7974, 'max_length': 4}, 'value': ''},
             'AV8BNA_ODU_4_SELECT': {'klass': 'StringBuffer', 'args': {'address': 0x7978, 'max_length': 1}, 'value': ''},
             'AV8BNA_ODU_4_Text': {'klass': 'StringBuffer', 'args': {'address': 0x797a, 'max_length': 4}, 'value': ''},
             'AV8BNA_ODU_5_SELECT': {'klass': 'StringBuffer', 'args': {'address': 0x797e, 'max_length': 1}, 'value': ''},
             'AV8BNA_ODU_5_Text': {'klass': 'StringBuffer', 'args': {'address': 0x7980, 'max_length': 4}, 'value': ''}}
 
-    def _draw_common_data(self, draw: ImageDraw, scale: int) -> ImageDraw:
+    def _draw_common_data(self, draw: ImageDraw.ImageDraw, scale: int) -> ImageDraw.ImageDraw:
         """
         Draw common part (based on scale) for Mono and Color LCD.
 
         :param draw: ImageDraw instance
         :param scale: scaling factor (Mono 1, Color 2)
         :return: updated image to draw
         """
         draw.text(xy=(50 * scale, 0), fill=self.lcd.foreground, font=self.lcd.font_l, text=f'{self.get_bios("UFC_SCRATCHPAD")}')
         draw.line(xy=(50 * scale, 20 * scale, 160 * scale, 20 * scale), fill=self.lcd.foreground, width=1)
 
         draw.rectangle(xy=(50 * scale, 29 * scale, 70 * scale, 42 * scale), fill=self.lcd.background, outline=self.lcd.foreground)
-        draw.text(xy=(52 * scale, 29 * scale), text=self.get_bios('UFC_COMM1_DISPLAY'), fill=self.lcd.foreground, font=self.lcd.font_l)
+        draw.text(xy=(52 * scale, 29 * scale), text=str(self.get_bios('UFC_COMM1_DISPLAY')), fill=self.lcd.foreground, font=self.lcd.font_l)
 
         draw.rectangle(xy=(139 * scale, 29 * scale, 159 * scale, 42 * scale), fill=self.lcd.background, outline=self.lcd.foreground)
-        draw.text(xy=(140 * scale, 29 * scale), text=self.get_bios('UFC_COMM2_DISPLAY'), fill=self.lcd.foreground, font=self.lcd.font_l)
+        draw.text(xy=(140 * scale, 29 * scale), text=str(self.get_bios('UFC_COMM2_DISPLAY')), fill=self.lcd.foreground, font=self.lcd.font_l)
 
         for i in range(1, 6):
             offset = (i - 1) * 8 * scale
             draw.text(xy=(0 * scale, offset), fill=self.lcd.foreground, font=self.lcd.font_s,
                       text=f'{i}{self.get_bios(f"AV8BNA_ODU_{i}_SELECT")}{self.get_bios(f"AV8BNA_ODU_{i}_Text")}')
         return draw
 
@@ -976,15 +971,20 @@
                   LcdButton.LEFT: 'UFC_COM1_SEL -3200\n',
                   LcdButton.RIGHT: 'UFC_COM1_SEL 3200\n',
                   LcdButton.DOWN: 'UFC_COM2_SEL -3200\n',
                   LcdButton.UP: 'UFC_COM2_SEL 3200\n'}
         return super().button_request(button, action.get(button, '\n'))
 
 
-def draw_autopilot_channels(lcd: LcdInfo, ap_channel: str, c_rect: Sequence[int], c_text: Sequence[int], draw_obj: ImageDraw, turn_on: Union[str, int]) -> None:
+def draw_autopilot_channels(lcd: LcdInfo,
+                            ap_channel: str,
+                            c_rect: Tuple[float, float, float, float],
+                            c_text: Tuple[float, float],
+                            draw_obj: ImageDraw.ImageDraw,
+                            turn_on: Union[str, int]) -> None:
     """
     Draw rectangles with background for autopilot channels.
 
     :param lcd: instance of LCD
     :param ap_channel: channel name
     :param c_rect: coordinates for rectangle
     :param c_text: coordinates for name
```

### Comparing `dcspy-2.0.0/dcspy/dcsbios.py` & `dcspy-2.1.0/dcspy/dcsbios.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     DATA_HIGH = auto()
     WAIT_FOR_SYNC = auto()
 
 
 class ProtocolParser:
     """DCS_BIOS protocol parser."""
     def __init__(self) -> None:
-        """Basic constructor."""
+        """Initialize instance."""
         self.state = ParserState.WAIT_FOR_SYNC
         self.sync_byte_count = 0
         self.address = 0
         self.count = 0
         self.data = 0
         self.write_callbacks: Set[Callable] = set()
         self.frame_sync_callbacks: Set[Callable] = set()
@@ -45,91 +45,91 @@
         else:
             self.sync_byte_count = 0
 
         self._wait_for_sync()
 
     def _address_low(self, int_byte: int) -> None:
         """
-        Handling of ADDRESS_LOW state.
+        Handle ADDRESS_LOW state.
 
         :param int_byte: data to process
         """
         self.address = int_byte
         self.state = ParserState.ADDRESS_HIGH
 
     def _address_high(self, int_byte: int) -> None:
         """
-        Handling of ADDRESS_HIGH state.
+        Handle ADDRESS_HIGH state.
 
         :param int_byte: data to process
         """
         self.address += int_byte * 256
         if self.address != 0x5555:
             self.state = ParserState.COUNT_LOW
         else:
             self.state = ParserState.WAIT_FOR_SYNC
 
     def _count_low(self, int_byte: int) -> None:
         """
-        Handling of COUNT_LOW state.
+        Handle COUNT_LOW state.
 
         :param int_byte: data to process
         """
         self.count = int_byte
         self.state = ParserState.COUNT_HIGH
 
     def _count_high(self, int_byte: int) -> None:
         """
-        Handling of COUNT_HIGH state.
+        Handle COUNT_HIGH state.
 
         :param int_byte: data to process
         """
         self.count += 256 * int_byte
         self.state = ParserState.DATA_LOW
 
     def _data_low(self, int_byte: int) -> None:
         """
-        Handling of DATA_LOW state.
+        Handle DATA_LOW state.
 
         :param int_byte: data to process
         """
         self.data = int_byte
         self.count -= 1
         self.state = ParserState.DATA_HIGH
 
     def _data_high(self, int_byte: int) -> None:
         """
-        Handling of DATA_HIGH state.
+        Handle DATA_HIGH state.
 
         :param int_byte: data to process
         """
         self.data += 256 * int_byte
         self.count -= 1
         for callback in self.write_callbacks:
             callback(self.address, self.data)
         self.address += 2
         if self.count == 0:
             self.state = ParserState.ADDRESS_LOW
         else:
             self.state = ParserState.DATA_LOW
 
     def _wait_for_sync(self) -> None:
-        """Handling of WAIT_FOR_SYNC state."""
+        """Handle WAIT_FOR_SYNC state."""
         if self.sync_byte_count == 4:
             self.state = ParserState.ADDRESS_LOW
             self.sync_byte_count = 0
             for callback in self.frame_sync_callbacks:
                 callback()
 
 
 class StringBuffer:
     """String buffer for DCS-BIOS protocol."""
     def __init__(self, parser: ProtocolParser, address: int, max_length: int, callback: Callable) -> None:
         """
-        Basic constructor.
+        Initialize instance.
 
         :param parser:
         :param address:
         :param max_length:
         :param callback:
         """
         self.__address = address
@@ -149,15 +149,15 @@
         """
         if self.buffer[index] != char:
             self.buffer[index] = char
             self.__dirty = True
 
     def on_dcsbios_write(self, address: int, data: int) -> None:
         """
-        Callback function.
+        Set callback function.
 
         :param address:
         :param data:
         """
         if self.__address <= address < self.__address + self.__length:
             data_bytes = pack('<H', data)
             self.set_char(address - self.__address, data_bytes[0])
@@ -171,15 +171,15 @@
                 callback(str_buff)
 
 
 class IntegerBuffer:
     """Integer buffer for DCS-BIOS protocol."""
     def __init__(self, parser: ProtocolParser, address: int, mask: int, shift_by: int, callback: Callable) -> None:
         """
-        Basic constructor.
+        Initialize instance.
 
         :param parser:
         :param address:
         :param mask:
         :param shift_by:
         :param callback:
         """
@@ -189,15 +189,15 @@
         self.__value = int()
         self.callbacks: Set[Callable] = set()
         self.callbacks.add(callback)
         parser.write_callbacks.add(partial(self.on_dcsbios_write))
 
     def on_dcsbios_write(self, address: int, data: int) -> None:
         """
-        Callback function.
+        Set callback function.
 
         :param address:
         :param data:
         """
         if address == self.__address:
             value = (data & self.__mask) >> self.__shift_by
             if self.__value != value:
```

### Comparing `dcspy-2.0.0/dcspy/dcspy.png` & `dcspy-2.1.0/dcspy/dcspy.png`

 * *Files identical despite different names*

### Comparing `dcspy-2.0.0/dcspy/log.py` & `dcspy-2.1.0/dcspy/log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from logging import DEBUG, StreamHandler, INFO, Formatter, Logger
+from logging import DEBUG, INFO, Formatter, Logger, StreamHandler
 from logging.handlers import RotatingFileHandler
 from pathlib import Path
 from tempfile import gettempdir
 
 
 def config_logger(logger: Logger, verbose=False) -> None:
     """
```

### Comparing `dcspy-2.0.0/dcspy/logitech.py` & `dcspy-2.1.0/dcspy/logitech.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from logging import getLogger
 from pprint import pformat
 from socket import socket
 from typing import List
 
 from PIL import Image, ImageDraw
 
-from dcspy import LcdColor, LcdMono, SUPPORTED_CRAFTS, SEND_ADDR, LcdButton
+from dcspy import SEND_ADDR, SUPPORTED_CRAFTS, LcdButton, LcdColor, LcdMono
 from dcspy.aircraft import Aircraft
 from dcspy.dcsbios import ProtocolParser
 from dcspy.sdk import lcd_sdk
 
 LOG = getLogger(__name__)
 
 
@@ -134,15 +134,15 @@
         * sent action to DCS-BIOS via. network socket
         :param sock: network socket
         """
         button = self.check_buttons()
         if button.value:
             sock.sendto(bytes(self.plane.button_request(button), 'utf-8'), SEND_ADDR)
 
-    def clear(self, true_clear=False):
+    def clear(self, true_clear=False) -> None:
         """
         Clear LCD.
 
         :param true_clear:
         """
         LOG.debug(f'Clear LCD type: {self.lcd.type}')
         lcd_sdk.clear_display(true_clear)
@@ -151,15 +151,15 @@
         """
         Prepare image for base of LCD type.
 
         For G13/G15/G510 takes first 4 or fewer elements of list and display as 4 rows.
         For G19 takes first 8 or fewer elements of list and display as 8 rows.
         :return: image instance ready display on LCD
         """
-        img = Image.new(mode=self.lcd.mode, size=(self.lcd.width, self.lcd.height), color=self.lcd.background)
+        img = Image.new(mode=self.lcd.mode.value, size=(self.lcd.width, self.lcd.height), color=self.lcd.background)
         draw = ImageDraw.Draw(img)
         for line_no, line in enumerate(self._display):
             draw.text(xy=(0, self.vert_space * line_no), text=line, fill=self.lcd.foreground, font=self.lcd.font_s)
         return img
 
     def __str__(self) -> str:
         """
```

### Comparing `dcspy-2.0.0/dcspy/run.py` & `dcspy-2.1.0/dcspy/run.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 from logging import getLogger
 from pathlib import Path
-from threading import Event
 
 import customtkinter
 
-from dcspy import config, LCD_TYPES
-from dcspy.starter import dcspy_run
+from dcspy import config
 from dcspy.tk_gui import DcspyGui
 from dcspy.utils import check_dcs_ver
 
 LOG = getLogger(__name__)
-__version__ = '2.0.0'
+__version__ = '2.1.0'
 
 
-def run():
-    """Function to start DCSpy GUI."""
-    if config['show_gui']:
-        customtkinter.set_appearance_mode(config['theme_mode'])
-        customtkinter.set_default_color_theme(config['theme_color'])
-        LOG.info(f'dcspy {__version__} https://github.com/emcek/dcspy')
-        dcs_type, dcs_ver = check_dcs_ver(Path(str(config["dcs"])))
-        LOG.info(f'DCS {dcs_type} ver: {dcs_ver}')
-        root = customtkinter.CTk()
-        width, height = 770, 500
-        root.geometry(f'{width}x{height}')
-        root.minsize(width=width, height=height)
-        root.iconbitmap(Path(__file__).resolve().with_name('dcspy.ico'))
-        if config['theme_mode'] == 'dark':
-            root.iconbitmap(Path(__file__).resolve().with_name('dcspy_white.ico'))
-        root.title('DCSpy')
-        DcspyGui(master=root)
-        root.mainloop()
-    else:
-        dcspy_run(lcd_type=LCD_TYPES[config['keyboard']]['type'], event=Event())
+def run() -> None:
+    """Start DCSpy GUI."""
+    customtkinter.set_appearance_mode(config['theme_mode'])
+    customtkinter.set_default_color_theme(config['theme_color'])
+    LOG.info(f'dcspy {__version__} https://github.com/emcek/dcspy')
+    dcs_type, dcs_ver = check_dcs_ver(Path(str(config["dcs"])))
+    LOG.info(f'DCS {dcs_type} ver: {dcs_ver}')
+    root = customtkinter.CTk()
+    width, height = 770, 500
+    root.geometry(f'{width}x{height}')
+    root.minsize(width=width, height=height)
+    root.iconbitmap(Path(__file__).resolve().with_name('dcspy.ico'))
+    if config['theme_mode'] == 'dark':
+        root.iconbitmap(Path(__file__).resolve().with_name('dcspy_white.ico'))
+    root.title('DCSpy')
+    DcspyGui(master=root)
+    if not config['show_gui']:
+        root.withdraw()
+    root.mainloop()
 
 
 if __name__ == '__main__':
     run()
```

### Comparing `dcspy-2.0.0/dcspy/sdk/__init__.py` & `dcspy-2.1.0/dcspy/sdk/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,37 @@
-from ctypes import CDLL, sizeof, c_void_p
+from ctypes import CDLL, c_void_p, sizeof
 from logging import getLogger
 from os import environ
 from platform import architecture
 from sys import maxsize
 from typing import Optional
 
 LOG = getLogger(__name__)
 
 
 def _init_dll(lib_type: str) -> CDLL:
     """
-    Initialization of C dynamic linking library.
+    Initialize C dynamic linking library.
 
     :param lib_type: LCD or LED
     :return: C DLL instance
     """
     arch = 'x64' if all([architecture()[0] == '64bit', maxsize > 2 ** 32, sizeof(c_void_p) > 4]) else 'x86'
     try:
         prog_files = environ['PROGRAMW6432']
     except KeyError:
         prog_files = environ['PROGRAMFILES']
-    return CDLL(f"{prog_files}\\Logitech Gaming Software\\SDK\\{lib_type}\\{arch}\\Logitech{lib_type.capitalize()}.dll")
+    dll_path = f"{prog_files}\\Logitech Gaming Software\\SDK\\{lib_type}\\{arch}\\Logitech{lib_type.capitalize()}.dll"
+    LOG.debug(f'Selected DLL: {dll_path}')
+    return CDLL(dll_path)
 
 
 def load_dll(lib_type: str) -> Optional[CDLL]:
     """
-    Initialization and loading of C dynamic linking library.
+    Initialize and load of C dynamic linking library.
 
     :param lib_type: library to load: LCD or LED
     :return: C DLL instance
     """
     try:
         dll = _init_dll(lib_type)
         LOG.info(f'Loading of {lib_type} SDK success')
```

### Comparing `dcspy-2.0.0/dcspy/sdk/lcd_sdk.py` & `dcspy-2.1.0/dcspy/sdk/lcd_sdk.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,24 @@
-from ctypes import c_bool, c_wchar_p, c_int, c_ubyte
+from ctypes import c_bool, c_int, c_ubyte, c_wchar_p
 from logging import getLogger
 from typing import List, Tuple
 
 from PIL import Image
 
+from dcspy import (COLOR_HEIGHT, COLOR_WIDTH, MONO_HEIGHT, MONO_WIDTH,
+                   TYPE_COLOR, TYPE_MONO)
 from dcspy.sdk import load_dll
 
 LOG = getLogger(__name__)
-
-# LCD types
-TYPE_MONO = 1
-TYPE_COLOR = 2
-
-# LCD Monochrome size
-MONO_WIDTH = 160
-MONO_HEIGHT = 43
-
-# LCD Color size
-COLOR_WIDTH = 320
-COLOR_HEIGHT = 240
-
 LCD_DLL = load_dll('LCD')
 
 
 def logi_lcd_init(name: str, lcd_type: int) -> bool:
     """
-    Function makes necessary initializations.
+    Make necessary initializations.
 
     You must call this function prior to any other function in the library.
     :param name: the name of your applet, you can't change it after initialization
     :param lcd_type: defines the type of your applet lcd target
     :return: result
     """
     if LCD_DLL:
@@ -38,61 +27,61 @@
         logilcdinit.argtypes = (c_wchar_p, c_int)
         return logilcdinit(name, lcd_type)
     return False
 
 
 def logi_lcd_is_connected(lcd_type: int) -> bool:
     """
-    Function checks if a device of the type specified by the parameter is connected.
+    Check if a device of the type specified by the parameter is connected.
 
     :param lcd_type: defines the type of your applet lcd target
     :return: result
     """
     if LCD_DLL:
         logilcdisconnected = LCD_DLL['LogiLcdIsConnected']
         logilcdisconnected.restype = c_bool
         logilcdisconnected.argtypes = [c_int]
         return logilcdisconnected(lcd_type)
     return False
 
 
 def logi_lcd_is_button_pressed(button: int) -> bool:
     """
-    Function checks if the button specified by the parameter is being pressed.
+    Check if the button specified by the parameter is being pressed.
 
     :param button: defines the button to check on
     :return: result
     """
     if LCD_DLL:
         logilcdisbuttonpressed = LCD_DLL['LogiLcdIsButtonPressed']
         logilcdisbuttonpressed.restype = c_bool
         logilcdisbuttonpressed.argtypes = [c_int]
         return logilcdisbuttonpressed(button)
     return False
 
 
 def logi_lcd_update() -> None:
-    """Function updates the LCD."""
+    """Update the LCD."""
     if LCD_DLL:
         logilcdupdate = LCD_DLL['LogiLcdUpdate']
         logilcdupdate.restype = None
         logilcdupdate()
 
 
 def logi_lcd_shutdown() -> None:
-    """Function kills the applet and frees memory used by the SDK."""
+    """Kill the applet and frees memory used by the SDK."""
     if LCD_DLL:
         logilcdshutdown = LCD_DLL['LogiLcdShutdown']
         logilcdshutdown.restype = None
         logilcdshutdown()
 
 
 def logi_lcd_mono_set_background(pixels: List[int]) -> bool:
     """
-    The array of pixels is organized as a rectangular area, 160 bytes wide and 43 bytes high.
+    Set pixels as a rectangular area, 160 bytes wide and 43 bytes high.
 
     Despite the display being monochrome, 8 bits per pixel are used here for simple
     manipulation of individual pixels.
 
     Note: The image size must be 160x43 in order to use this function. The SDK will turn on
     the pixel on the screen if the value assigned to that byte is >= 128, it will remain off
     if the  value is < 128.
@@ -104,17 +93,17 @@
         logilcdmonosetbackground.restype = c_bool
         logilcdmonosetbackground.argtypes = [c_ubyte * (MONO_WIDTH * MONO_HEIGHT)]
         img_bytes = [pixel * 128 for pixel in pixels]
         return logilcdmonosetbackground((c_ubyte * (MONO_WIDTH * MONO_HEIGHT))(*img_bytes))
     return False
 
 
-def logi_lcd_mono_set_text(line_no: int, text: str):
+def logi_lcd_mono_set_text(line_no: int, text: str) -> bool:
     """
-    Function sets the specified text in the requested line on the monochrome lcd device connected.
+    Set the specified text in the requested line on the monochrome lcd device connected.
 
     :param line_no: The monochrome LCD has 4 lines, so this parameter can be any number from 0 to 3
     :param text: defines the text you want to display
     :return: result
     """
     if LCD_DLL:
         logilcdmonosettext = LCD_DLL['LogiLcdMonoSetText']
@@ -122,15 +111,15 @@
         logilcdmonosettext.argtypes = (c_int, c_wchar_p)
         return logilcdmonosettext(line_no, text)
     return False
 
 
 def logi_lcd_color_set_background(pixels: List[Tuple[int, int, int, int]]) -> bool:
     """
-    The array of pixels is organized as a rectangular area, 320 bytes wide and 240 bytes high.
+    Set array of pixels as a rectangular area, 320 bytes wide and 240 bytes high.
 
     Since the color lcd can display the full RGB gamma, 32 bits per pixel (4 bytes) are used.
     The size of the colorBitmap array has to be 320x240x4 = 307200 therefore.
     Note: The image size must be 320x240 in order to use this function.
     :param pixels: list of 307200 (320x240x4) pixels as int
     :return: result
     """
@@ -139,17 +128,17 @@
         logilcdcolorsetbackground.restype = c_bool
         logilcdcolorsetbackground.argtypes = [c_ubyte * (4 * COLOR_WIDTH * COLOR_HEIGHT)]
         img_bytes = [byte for pixel in pixels for byte in pixel]
         return logilcdcolorsetbackground((c_ubyte * (4 * COLOR_WIDTH * COLOR_HEIGHT))(*img_bytes))
     return False
 
 
-def logi_lcd_color_set_title(text: str, rgb: Tuple[int, int, int] = (255, 255, 255)):
+def logi_lcd_color_set_title(text: str, rgb: Tuple[int, int, int] = (255, 255, 255)) -> bool:
     """
-    Function sets the specified text in the first line on the color lcd device connected.
+    Set the specified text in the first line on the color lcd device connected.
 
     The font size that will be displayed is bigger than the one used in the other lines,
     so you can use this function to set the title of your applet/page.
     If you don't specify any color, your title will be white.
     :param text: defines the text you want to display as title
     :param rgb: tuple with integer values between 0 and 255 as red, green, blue
     :return: result
@@ -158,17 +147,17 @@
         logilcdcolorsettitle = LCD_DLL['LogiLcdColorSetTitle']
         logilcdcolorsettitle.restype = c_bool
         logilcdcolorsettitle.argtypes = (c_wchar_p, c_int, c_int, c_int)
         return logilcdcolorsettitle(text, *rgb)
     return False
 
 
-def logi_lcd_color_set_text(line_no: int, text: str, rgb: Tuple[int, int, int] = (255, 255, 255)):
+def logi_lcd_color_set_text(line_no: int, text: str, rgb: Tuple[int, int, int] = (255, 255, 255)) -> bool:
     """
-    Function sets the specified text in the requested line on the color lcd device connected.
+    Set the specified text in the requested line on the color lcd device connected.
 
     If you don't specify any color, your title will be white.
     :param line_no: The color LCD has 8 lines for standard text, so this parameter can be any number from 0 to 7
     :param text: defines the text you want to display
     :param rgb: tuple with integer values between 0 and 255 as red, green, blue
     :return: result
     """
@@ -196,15 +185,15 @@
         for line_no, line in enumerate(txt):
             logi_lcd_color_set_text(line_no, line)
         logi_lcd_update()
     else:
         LOG.warning('LCD is not connected')
 
 
-def update_display(image: Image) -> None:
+def update_display(image: Image.Image) -> None:
     """
     Update display LCD with image.
 
     :param image: image object from pillow library
     """
     if logi_lcd_is_connected(TYPE_MONO):
         logi_lcd_mono_set_background(list(image.getdata()))
@@ -225,27 +214,27 @@
     if logi_lcd_is_connected(TYPE_MONO):
         _clear_mono(true_clear)
     elif logi_lcd_is_connected(TYPE_COLOR):
         _clear_color(true_clear)
     logi_lcd_update()
 
 
-def _clear_mono(true_clear):
+def _clear_mono(true_clear) -> None:
     """
     Clear mono display.
 
     :param true_clear:
     """
     logi_lcd_mono_set_background([0] * MONO_WIDTH * MONO_HEIGHT)
     if true_clear:
         for i in range(4):
             logi_lcd_mono_set_text(i, '')
 
 
-def _clear_color(true_clear):
+def _clear_color(true_clear) -> None:
     """
     Clear color display.
 
     :param true_clear:
     """
     logi_lcd_color_set_background([(0,) * 4] * COLOR_WIDTH * COLOR_HEIGHT)
     if true_clear:
```

### Comparing `dcspy-2.0.0/dcspy/sdk/led_sdk.py` & `dcspy-2.1.0/dcspy/sdk/led_sdk.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ctypes import c_bool, c_wchar_p, c_int
+from ctypes import c_bool, c_int, c_wchar_p
 from logging import getLogger
 from threading import Event
 from time import sleep
 from typing import Tuple
 
 from dcspy.sdk import load_dll
 
@@ -14,30 +14,30 @@
 LOGI_DEVICETYPE_ALL = LOGI_DEVICETYPE_MONOCHROME | LOGI_DEVICETYPE_RGB
 
 LED_DLL = load_dll('LED')
 
 
 def logi_led_init() -> bool:
     """
-    The function makes sure there isn't already another instance running and then makes necessary initializations.
+    Make sure there isn't already another instance running and then makes necessary initializations.
 
     It saves the current lighting for all connected and supported devices. This function will also stop any effect
     currently going on the connected devices.
     :return: result
     """
     if LED_DLL:
         logiledinit = LED_DLL['LogiLedInit']
         logiledinit.restype = c_bool
         return logiledinit()
     return False
 
 
 def logi_led_init_with_name(name: str) -> bool:
     """
-    The function makes sure there isn't already another instance running and then makes necessary initializations.
+    Make sure there isn't already another instance running and then makes necessary initializations.
 
     It saves the current lighting for all connected and supported devices.
     This function will also stop any effect currently going on the connected devices. Passing a name into this
     function will make the integration show up with a given custom name. The name is set only once, the first
     time this function or logi_led_init() is called.
     :param name: The referred name for this integration to show u as
     :return: result
@@ -48,15 +48,15 @@
         logiledinitwithname.argtypes = (c_wchar_p,)
         return logiledinitwithname(name)
     return False
 
 
 def logi_led_set_target_device(target_device: int) -> bool:
     """
-    The function sets the target device type for future calls.
+    Set the target device type for future calls.
 
     The default target device is LOGI_DEVICETYPE_ALL, therefore, if no call is made to LogiLedSetTargetDevice
     the SDK will apply any function to all the connected devices.
     :param target_device: one or a combination of the following values:
                           LOGI_DEVICETYPE_MONOCHROME, LOGI_DEVICETYPE_RGB, LOGI_DEVICETYPE_ALL
     :return: result
     """
@@ -66,30 +66,30 @@
         logiledsettargetdevice.argtypes = (c_int,)
         return logiledsettargetdevice(target_device)
     return False
 
 
 def logi_led_save_current_lighting() -> bool:
     """
-    The function saves the current lighting so that it can be restored after a temporary effect is finished.
+    Save the current lighting so that it can be restored after a temporary effect is finished.
 
     For example if flashing a red warning sign for a few seconds, you would call the logi_led_save_current_lighting()
     function just before starting the warning effect.
     :return: result
     """
     if LED_DLL:
         logiledsavecurrentlighting = LED_DLL['LogiLedSaveCurrentLighting']
         logiledsavecurrentlighting.restype = c_bool
         return logiledsavecurrentlighting()
     return False
 
 
 def logi_led_restore_lighting() -> bool:
     """
-    The function restores the last saved lighting.
+    Restore the last saved lighting.
 
     It should be called after a temporary effect is finished.
     For example if flashing a red warning sign for a few seconds, you would call this function right
     after the warning effect is finished.
     :return: result
     """
     if LED_DLL:
@@ -97,15 +97,15 @@
         logiledrestorecurrentlighting.restype = c_bool
         return logiledrestorecurrentlighting()
     return False
 
 
 def logi_led_set_lighting(rgb: Tuple[int, int, int]) -> bool:
     """
-    The function sets the lighting on connected and supported devices.
+    Set the lighting on connected and supported devices.
 
     Do not call this function immediately after logi_led_init(). Instead of leave a little of time after logi_led_init().
     For devices that only support a single color, the highest percentage value given of the three colors will
     define the intensity. For monochrome device, Logitech Gaming Software will reduce
     proportionally the value of the highest color, according to the user hardware brightness setting.
 
     :param rgb: tuple with integer values range 0 to 100 as amount of red, green, blue
@@ -117,15 +117,15 @@
         logiledsetlighting.argtypes = (c_int, c_int, c_int)
         return logiledsetlighting(*rgb)
     return False
 
 
 def logi_led_flash_lighting(rgb: Tuple[int, int, int], duration: int, interval: int) -> bool:
     """
-    The function saves the current lighting, plays the flashing effect on the targeted devices.
+    Save the current lighting, plays the flashing effect on the targeted devices.
 
     Finally, restores the saved lighting.
     :param rgb: tuple with integer values range 0 to 100 as amount of red, green, blue
     :param duration: duration of the effect in milliseconds this parameter can be set to LOGI_LED_DURATION_INFINITE
                      to make the effect run until sto ed through logi_led_stop_effects()
     :param interval: duration of the flashing interval in milliseconds
     :return: result
@@ -136,15 +136,15 @@
         logiledflashlighting.argtypes = (c_int, c_int, c_int, c_int, c_int)
         return logiledflashlighting(*rgb, duration, interval)
     return False
 
 
 def logi_led_pulse_lighting(rgb: Tuple[int, int, int], duration: int, interval: int) -> bool:
     """
-    The function saves the current lighting, plays the pulsing effect on the targeted devices.
+    Save the current lighting, plays the pulsing effect on the targeted devices.
 
     Finally, restores the saved lighting.
     :param rgb: tuple with integer values range 0 to 100 as amount of red, green, blue
     :param duration: duration of the effect in milliseconds this parameter can be set to LOGI_LED_DURATION_INFINITE
                      to make the effect run until sto ed through logi_led_stop_effects()
     :param interval: duration of the flashing interval in milliseconds
     :return: result
@@ -155,37 +155,37 @@
         logiledpulselighting.argtypes = (c_int, c_int, c_int, c_int, c_int)
         return logiledpulselighting(*rgb, duration, interval)
     return False
 
 
 def logi_led_stop_effects() -> bool:
     """
-    The function stops any of the presets effects.
+    Stop any of the presets effects.
 
     Started from logi_led_flash_lighting() or logi_led_pulse_lighting().
     :return: result
     """
     if LED_DLL:
         logiledstopeffects = LED_DLL['LogiLedStopEffects']
         logiledstopeffects.restype = c_bool
         return logiledstopeffects()
     return False
 
 
 def logi_led_shutdown() -> None:
-    """The function restores the last saved lighting and frees memory used by the SDK."""
+    """Restore the last saved lighting and frees memory used by the SDK."""
     if LED_DLL:
         logiledshutdown = LED_DLL['LogiLedShutdown']
         logiledshutdown.restype = c_bool
         logiledshutdown()
 
 
-def start_led_pulse(rgb: Tuple[int, int, int], duration: int, interval: int, event: Event):
+def start_led_pulse(rgb: Tuple[int, int, int], duration: int, interval: int, event: Event) -> None:
     """
-    The function start the pulsing red effect in thread on the keyboard.
+    Start the pulsing red effect in thread on the keyboard.
 
     :param rgb: tuple with integer values range 0 to 100 as amount of red, green, blue
     :param duration: duration of the effect in milliseconds this parameter can be set to 0 (zero)
                      to make the effect run until event is set
     :param interval: duration of the flashing interval in milliseconds
     :param event: stop event for infinite loop
     """
```

### Comparing `dcspy-2.0.0/dcspy/starter.py` & `dcspy-2.1.0/dcspy/starter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import socket
 import struct
 from collections import deque
 from importlib import import_module
 from logging import getLogger
 from threading import Event
-from time import time, gmtime
+from time import gmtime, time
 from typing import Iterator
 
-from dcspy import RECV_ADDR, MULTICAST_IP, config
+from dcspy import MULTICAST_IP, RECV_ADDR, config
 from dcspy.dcsbios import ProtocolParser
 from dcspy.logitech import LogitechKeyboard
 from dcspy.utils import get_version_string
 
 LOG = getLogger(__name__)
 LOOP_FLAG = True
-__version__ = '2.0.0'
+__version__ = '2.1.0'
 
 
 def _handle_connection(logi_keyboard: LogitechKeyboard, parser: ProtocolParser, sock: socket.socket, event: Event) -> None:
     """
-    Main loop where all the magic is happened.
+    Handle main loop where all the magic is happened.
 
     :param logi_keyboard: type of Logitech keyboard with LCD
     :param parser: DCS protocol parser
     :param sock: multi-cast UDP socket
     :param event: stop event for main loop
     """
     start_time = time()
     ver_string = get_version_string(repo='emcek/dcspy', current_ver=__version__, check=config['check_ver'])
     LOG.info('Waiting for DCS connection...')
-    support_banner = _supporters(text='Huge thanks to: Sireyn, Nick Thain, BrotherBloat and others! For support and help! ', width=26)
+    support_banner = _supporters(text='Huge thanks to: Alexander Leschanz, Sireyn, Nick Thain, BrotherBloat and others! For support and help! ', width=26)
     while not event.is_set():
         try:
             dcs_bios_resp = sock.recv(2048)
             for int_byte in dcs_bios_resp:
                 parser.process_byte(int_byte)
             start_time = time()
             _load_new_plane_if_detected(logi_keyboard)
@@ -86,15 +86,15 @@
                              f'No data from DCS:   {wait_time.tm_min:02d}:{wait_time.tm_sec:02d}',
                              f'{next(support_iter)}',
                              ver_string]
 
 
 def _prepare_socket() -> socket.socket:
     """
-    Preparing multi-cast UDP socket for DCS-BIOS communication.
+    Prepare multi-cast UDP socket for DCS-BIOS communication.
 
     :return: socket object
     """
     sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM, socket.IPPROTO_UDP)
     sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
     sock.bind(RECV_ADDR)
     mreq = struct.pack('=4sl', socket.inet_aton(MULTICAST_IP), socket.INADDR_ANY)
```

### Comparing `dcspy-2.0.0/dcspy/tk_gui.py` & `dcspy-2.1.0/dcspy/tk_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 import tkinter as tk
 from functools import partial
 from logging import getLogger
 from pathlib import Path
-from platform import architecture, uname, python_implementation, python_version
+from platform import architecture, python_implementation, python_version, uname
 from re import search
-from shutil import unpack_archive, rmtree, copy, copytree
+from shutil import copy, copytree, rmtree, unpack_archive
 from tempfile import gettempdir
-from threading import Thread, Event
-from typing import Union, Optional
+from threading import Event, Thread
+from typing import Optional, Union
 from webbrowser import open_new
 
 import customtkinter
 from CTkMessagebox import CTkMessagebox
-from PIL import Image
 from packaging import version
+from PIL import Image
+from pystray import Icon, MenuItem
 
-from dcspy import LOCAL_APPDATA, LCD_TYPES, config
+from dcspy import LCD_TYPES, LOCAL_APPDATA, config
 from dcspy.starter import dcspy_run
-from dcspy.utils import save_cfg, check_ver_at_github, download_file, proc_is_running, defaults_cfg, ReleaseInfo, get_version_string, check_dcs_ver, \
-    check_github_repo, check_dcs_bios_entry, get_default_yaml
+from dcspy.utils import (ReleaseInfo, check_dcs_bios_entry, check_dcs_ver,
+                         check_github_repo, check_ver_at_github, defaults_cfg,
+                         download_file, get_default_yaml, get_version_string,
+                         proc_is_running, save_cfg)
 
-__version__ = '2.0.0'
+__version__ = '2.1.0'
 LOG = getLogger(__name__)
 
 
 class DcspyGui(tk.Frame):
     """Tkinter GUI."""
-    def __init__(self, master: customtkinter.CTk) -> None:
+    def __init__(self, master: tk.Tk) -> None:
         """
         Create basic GUI for dcspy application.
 
         :param master: Top level widget
         """
         super().__init__(master)
-        self.master = master
+        self.master: tk.Tk = master
         self.cfg_file = get_default_yaml(local_appdata=LOCAL_APPDATA)
         self.l_bios: Union[version.Version, version.LegacyVersion] = version.LegacyVersion('Not checked')
         self.r_bios: Union[version.Version, version.LegacyVersion] = version.LegacyVersion('Not checked')
         self.event = Event()
 
         self.status_txt = tk.StringVar()
         self.lcd_type = tk.StringVar()
@@ -70,17 +73,37 @@
 
         self._load_cfg()
         self.btn_start: customtkinter.CTkButton
         self.btn_stop: customtkinter.CTkButton
         self.git_bios_switch: customtkinter.CTkSwitch
         self.bios_git_label: customtkinter.CTkLabel
         self.bios_git: customtkinter.CTkEntry
+        self.sys_tray_icon = self._setup_system_tray()
+        self.sys_tray_icon.run_detached()
         self._init_widgets()
         if config.get('autostart', False):
-            self.start_dcspy()
+            self._start_dcspy()
+        if not config.get('show_gui', False):
+            self.sys_tray_icon.notify('Running in background.', 'DCSpy')
+
+    def _setup_system_tray(self) -> Icon:
+        """
+        Configure system tray icon and its menu callbacks.
+
+        :return: system ray icon instance
+        """
+        icon = Image.open(Path(__file__).resolve().with_name('dcspy.ico'))
+        menu = (MenuItem('Show', self._show_gui), MenuItem('Stop', self._stop), MenuItem('Quit', self._close_gui),)
+        self.master.protocol('WM_DELETE_WINDOW', self._withdraw_gui)
+        return Icon('dcspy', icon, 'DCSpy', menu)
+
+    def _withdraw_gui(self) -> None:
+        """Withdraw application and show notification."""
+        self.sys_tray_icon.notify('Still running at system tray.', 'DCSpy')
+        self.master.withdraw()
 
     def _init_widgets(self) -> None:
         """Init all GUI widgets."""
         self.master.grid_columnconfigure(index=0, weight=0)
         self.master.grid_columnconfigure(index=1, weight=1)
         self.master.grid_rowconfigure(index=0, weight=1)
         self.master.grid_rowconfigure(index=1, weight=1)
@@ -114,70 +137,76 @@
         logo_label.grid(row=0, column=0, padx=20, pady=(20, 10))
         reset = customtkinter.CTkButton(master=sidebar_frame, text='Reset to defaults', command=self._set_defaults_cfg)
         reset.grid(row=1, column=0, padx=20, pady=10)
         check_bios = customtkinter.CTkButton(master=sidebar_frame, text='Update DCS-BIOS', command=self._update_bios)
         check_bios.grid(row=2, column=0, padx=20, pady=10)
         check_ver = customtkinter.CTkButton(master=sidebar_frame, text='Check DCSpy version', command=self._check_version)
         check_ver.grid(row=3, column=0, padx=20, pady=10)
-        self.btn_start = customtkinter.CTkButton(master=sidebar_frame, text='Start', command=self.start_dcspy)
+        self.btn_start = customtkinter.CTkButton(master=sidebar_frame, text='Start', command=self._start_dcspy)
         logo_icon = customtkinter.CTkImage(Image.open(Path(__file__).resolve().with_name('dcspy.png')), size=(130, 60))
         logo_label = customtkinter.CTkLabel(master=sidebar_frame, text='', image=logo_icon)
         logo_label.grid(row=4, column=0, sticky=tk.W + tk.E)
         self.btn_start.grid(row=5, column=0, padx=20, pady=10)
         self.btn_stop = customtkinter.CTkButton(master=sidebar_frame, text='Stop', state=tk.DISABLED, command=self._stop)
         self.btn_stop.grid(row=6, column=0, padx=20, pady=10)
-        close = customtkinter.CTkButton(master=sidebar_frame, text='Close', command=self.master.destroy)
+        close = customtkinter.CTkButton(master=sidebar_frame, text='Close', command=self._close_gui)
         close.grid(row=7, column=0, padx=20, pady=10)
         self.btn_start.configure(state=tk.ACTIVE)
         self.btn_stop.configure(state=tk.DISABLED)
 
     def _keyboards(self, tabview: customtkinter.CTkTabview) -> None:
         """Configure keyboard tab GUI."""
         for i, text in enumerate(LCD_TYPES):
             icon = customtkinter.CTkImage(Image.open(Path(__file__).resolve().with_name(LCD_TYPES[text]['icon'])), size=(103, 70))
             label = customtkinter.CTkLabel(master=tabview.tab('Keyboards'), text='', image=icon)
             label.grid(row=i, column=0)
-            rb_lcd_type = customtkinter.CTkRadioButton(master=tabview.tab('Keyboards'), text=text, variable=self.lcd_type, value=text, command=self._lcd_type_selected)
+            rb_lcd_type = customtkinter.CTkRadioButton(master=tabview.tab('Keyboards'), text=text, variable=self.lcd_type, value=text,
+                                                       command=self._lcd_type_selected)
             rb_lcd_type.grid(row=i, column=1)
             if config.get('keyboard', 'G13') == text:
                 rb_lcd_type.select()
 
     def _general_settings(self, tabview: customtkinter.CTkTabview) -> None:
         """Configure general tab GUI."""
         tabview.tab('General').grid_columnconfigure(index=0, weight=0)
         tabview.tab('General').grid_columnconfigure(index=1, weight=1)
         autostart_label = customtkinter.CTkLabel(master=tabview.tab('General'), text='Autostart DCSpy:')
         autostart_label.grid(column=0, row=0, sticky=tk.W, pady=5)
-        autostart = customtkinter.CTkSwitch(master=tabview.tab('General'), text='', variable=self.autostart_switch, onvalue=True, offvalue=False, command=partial(self._save_cfg))
+        autostart = customtkinter.CTkSwitch(master=tabview.tab('General'), text='', variable=self.autostart_switch, onvalue=True, offvalue=False,
+                                            command=partial(self._save_cfg))
         autostart.grid(column=1, row=0, sticky=tk.W, padx=(10, 0), pady=5)
         showgui_label = customtkinter.CTkLabel(master=tabview.tab('General'), text='Show GUI:')
         showgui_label.grid(column=0, row=1, sticky=tk.W, pady=5)
-        showgui = customtkinter.CTkSwitch(master=tabview.tab('General'), text='', variable=self.showgui_switch, onvalue=True, offvalue=False, command=partial(self._save_cfg))
+        showgui = customtkinter.CTkSwitch(master=tabview.tab('General'), text='', variable=self.showgui_switch, onvalue=True, offvalue=False,
+                                          command=partial(self._save_cfg))
         showgui.grid(column=1, row=1, sticky=tk.W, padx=(10, 0), pady=5)
         checkver_label = customtkinter.CTkLabel(master=tabview.tab('General'), text='Check DCSpy version:')
         checkver_label.grid(column=0, row=2, sticky=tk.W, pady=5)
-        checkver = customtkinter.CTkSwitch(master=tabview.tab('General'), text='', variable=self.checkver_switch, onvalue=True, offvalue=False, command=partial(self._save_cfg))
+        checkver = customtkinter.CTkSwitch(master=tabview.tab('General'), text='', variable=self.checkver_switch, onvalue=True, offvalue=False,
+                                           command=partial(self._save_cfg))
         checkver.grid(column=1, row=2, sticky=tk.W, padx=(10, 0), pady=5)
         dcs_label = customtkinter.CTkLabel(master=tabview.tab('General'), text='DCS folder:')
         dcs_label.grid(column=0, row=3, sticky=tk.W, pady=5)
         dcs = customtkinter.CTkEntry(master=tabview.tab('General'), placeholder_text='DCS installation', width=390, textvariable=self.dcs_path,
                                      validate='key', validatecommand=(self.master.register(self._save_entry_text), '%P', '%W', '%V'))
         dcs.grid(column=1, row=3, sticky=tk.W + tk.E, padx=(10, 0), pady=5)
         bscbios_label = customtkinter.CTkLabel(master=tabview.tab('General'), text='DCS-BIOS folder:')
         bscbios_label.grid(column=0, row=4, sticky=tk.W, pady=5)
         dcsbios = customtkinter.CTkEntry(master=tabview.tab('General'), placeholder_text='Path to DCS-BIOS', width=390, textvariable=self.bios_path,
                                          validate='key', validatecommand=(self.master.register(self._save_entry_text), '%P', '%W', '%V'))
         dcsbios.grid(column=1, row=4, sticky=tk.W + tk.E, padx=(10, 0), pady=5)
         appearance_mode_label = customtkinter.CTkLabel(master=tabview.tab('General'), text='Appearance Mode:', anchor=tk.W)
         appearance_mode_label.grid(column=0, row=5, sticky=tk.W, pady=5)
-        appearance_mode = customtkinter.CTkOptionMenu(master=tabview.tab('General'), values=['Light', 'Dark', 'System'], variable=self.theme_mode, command=self._change_mode)
+        appearance_mode = customtkinter.CTkOptionMenu(master=tabview.tab('General'), values=['Light', 'Dark', 'System'], variable=self.theme_mode,
+                                                      command=self._change_mode)
         appearance_mode.grid(column=1, row=5, sticky=tk.W, padx=(10, 0), pady=5)
         color_theme_label = customtkinter.CTkLabel(master=tabview.tab('General'), text='Color Theme:', anchor=tk.W)
         color_theme_label.grid(column=0, row=6, sticky=tk.W, pady=5)
-        color_theme = customtkinter.CTkOptionMenu(master=tabview.tab('General'), values=['Blue', 'Green', 'Dark Blue'], variable=self.theme_color, command=self._change_color)
+        color_theme = customtkinter.CTkOptionMenu(master=tabview.tab('General'), values=['Blue', 'Green', 'Dark Blue'], variable=self.theme_color,
+                                                  command=self._change_color)
         color_theme.grid(column=1, row=6, sticky=tk.W, padx=(10, 0), pady=5)
 
     def _mono_settings(self, tabview: customtkinter.CTkTabview) -> None:
         """Configure mono tab GUI."""
         tabview.tab('Mono').grid_columnconfigure(index=0, weight=0)
         tabview.tab('Mono').grid_columnconfigure(index=1, weight=1)
         mono_l_label = customtkinter.CTkLabel(master=tabview.tab('Mono'), textvariable=self.mono_l)
@@ -228,40 +257,45 @@
 
     def _special_settings(self, tabview: customtkinter.CTkTabview) -> None:
         """Configure special tab GUI."""
         tabview.tab('Special').grid_columnconfigure(index=0, weight=0)
         tabview.tab('Special').grid_columnconfigure(index=1, weight=1)
         dedfont_label = customtkinter.CTkLabel(master=tabview.tab('Special'), text='F-16 DED Font (only G19):')
         dedfont_label.grid(column=0, row=1, sticky=tk.W, pady=5)
-        dedfont = customtkinter.CTkSwitch(master=tabview.tab('Special'), text='', variable=self.dedfont_switch, onvalue=True, offvalue=False, command=partial(self._save_cfg))
+        dedfont = customtkinter.CTkSwitch(master=tabview.tab('Special'), text='', variable=self.dedfont_switch, onvalue=True, offvalue=False,
+                                          command=partial(self._save_cfg))
         dedfont.grid(column=1, row=1, sticky=tk.W, padx=(10, 0), pady=5)
 
     def _advanced_settings(self, tabview: customtkinter.CTkTabview) -> None:
         """Configure advanced tab GUI."""
         tabview.tab('Advanced').grid_columnconfigure(index=0, weight=0)
         tabview.tab('Advanced').grid_columnconfigure(index=1, weight=1)
         save_lcd_label = customtkinter.CTkLabel(master=tabview.tab('Advanced'), text='Save LCD screenshot:')
         save_lcd_label.grid(column=0, row=0, sticky=tk.W, pady=5)
-        save_lcd = customtkinter.CTkSwitch(master=tabview.tab('Advanced'), text='', variable=self.savelcd_switch, onvalue=True, offvalue=False, command=partial(self._save_cfg))
+        save_lcd = customtkinter.CTkSwitch(master=tabview.tab('Advanced'), text='', variable=self.savelcd_switch, onvalue=True, offvalue=False,
+                                           command=partial(self._save_cfg))
         save_lcd.grid(column=1, row=0, sticky=tk.W, padx=(10, 0), pady=5)
         verbose_label = customtkinter.CTkLabel(master=tabview.tab('Advanced'), text='Show more logs:')
         verbose_label.grid(column=0, row=1, sticky=tk.W, pady=5)
-        verbose = customtkinter.CTkSwitch(master=tabview.tab('Advanced'), text='', variable=self.verbose_switch, onvalue=True, offvalue=False, command=partial(self._save_cfg))
+        verbose = customtkinter.CTkSwitch(master=tabview.tab('Advanced'), text='', variable=self.verbose_switch, onvalue=True, offvalue=False,
+                                          command=partial(self._save_cfg))
         verbose.grid(column=1, row=1, sticky=tk.W, padx=(10, 0), pady=5)
         update_bios_label = customtkinter.CTkLabel(master=tabview.tab('Advanced'), text='Auto Update DCS-BIOS:')
         update_bios_label.grid(column=0, row=2, sticky=tk.W, pady=5)
-        update_bios = customtkinter.CTkSwitch(master=tabview.tab('Advanced'), text='', variable=self.update_bios, onvalue=True, offvalue=False, command=partial(self._save_cfg))
+        update_bios = customtkinter.CTkSwitch(master=tabview.tab('Advanced'), text='', variable=self.update_bios, onvalue=True, offvalue=False,
+                                              command=partial(self._save_cfg))
         update_bios.grid(column=1, row=2, sticky=tk.W, padx=(10, 0), pady=5)
         git_bios_label = customtkinter.CTkLabel(master=tabview.tab('Advanced'), text='Use live DCS-BIOS version:')
         git_bios_label.grid(column=0, row=3, sticky=tk.W, pady=5)
-        self.git_bios_switch = customtkinter.CTkSwitch(master=tabview.tab('Advanced'), text='', variable=self.bios_git_switch, onvalue=True, offvalue=False, command=self._bios_git_switch)
+        self.git_bios_switch = customtkinter.CTkSwitch(master=tabview.tab('Advanced'), text='', variable=self.bios_git_switch, onvalue=True, offvalue=False,
+                                                       command=self._bios_git_switch)
         self.git_bios_switch.grid(column=1, row=3, sticky=tk.W, padx=(10, 0), pady=5)
         self.bios_git_label = customtkinter.CTkLabel(master=tabview.tab('Advanced'), text='DCS-BIOS Git reference:', state=tk.DISABLED)
-        self.bios_git = customtkinter.CTkEntry(master=tabview.tab('Advanced'), placeholder_text='git reference', width=390, textvariable=self.bios_git_ref, state=tk.DISABLED,
-                                               validate='key', validatecommand=(self.master.register(self._save_entry_text), '%P', '%W', '%V'))
+        self.bios_git = customtkinter.CTkEntry(master=tabview.tab('Advanced'), validatecommand=(self.master.register(self._save_entry_text), '%P', '%W', '%V'),
+                                               placeholder_text='git reference', width=390, textvariable=self.bios_git_ref, state=tk.DISABLED, validate='key')
         if self.bios_git_switch.get():
             self.bios_git_label.configure(state=tk.NORMAL)
             self.bios_git.configure(state=tk.NORMAL)
 
         self.bios_git_label.grid(column=0, row=4, sticky=tk.W, pady=5)
         self.bios_git.grid(column=1, row=4, sticky=tk.W + tk.E, padx=(10, 0), pady=5)
 
@@ -345,15 +379,15 @@
         """
         Open default web browser URL page.
 
         :param url: URL address of web page
         """
         open_new(url)
 
-    def _slider_event(self, label: str, value: float):
+    def _slider_event(self, label: str, value: float) -> None:
         """
         Update correct label when slider is moved.
 
         :param label:
         :param value:
         """
         getattr(self, label).set(f'Font {" ".join([word.capitalize() for word in label.split("_")])} : {int(value)}')
@@ -435,15 +469,15 @@
     def _set_defaults_cfg(self) -> None:
         """Set defaults and stop application."""
         save_cfg(cfg_dict=defaults_cfg, filename=self.cfg_file)
         CTkMessagebox(title='Restart', message='DCSpy needs to be close.\nPlease start again manually!', icon='warning', option_1='OK')
         self.master.destroy()
 
     def _lcd_type_selected(self) -> None:
-        """Handling selected LCD type."""
+        """Handle selected LCD type."""
         keyboard = self.lcd_type.get()
         LOG.debug(f'Logitech {keyboard} selected')
         self.status_txt.set(f'Logitech {keyboard} selected')
         self._save_cfg()
 
     def _change_mode(self, theme_mode: str) -> None:
         """
@@ -456,15 +490,16 @@
 
     def _change_color(self, theme_color: str) -> None:
         """
         Save color theme and show message box to restart DCSpy.
 
         :param theme_color: value of color theme
         """
-        msg = CTkMessagebox(title='Change theme color', message='DCSpy needs to be close.\nIn order to apply color changes.\n\nPlease start again manually!', icon='question', option_1='Yes', option_2='No')
+        msg = CTkMessagebox(title='Change theme color', icon='question', option_1='Yes', option_2='No',
+                            message='DCSpy needs to be close.\nIn order to apply color changes.\n\nPlease start again manually!')
         if msg.get() == 'Yes':
             self._save_cfg()
             LOG.debug(f'Select: {theme_color}')
             self.master.destroy()
 
     def _save_entry_text(self, what: str, widget: str, trigger: str) -> bool:
         """
@@ -491,15 +526,18 @@
     def _check_version(self) -> None:
         """Check version of DCSpy and show message box."""
         ver_string = get_version_string(repo='emcek/dcspy', current_ver=__version__, check=True)
         self.status_txt.set(ver_string)
         if 'please update' in ver_string:
             self.master.clipboard_clear()
             self.master.clipboard_append('pip install --upgrade dcspy')
-            CTkMessagebox(title='New version', message='Open Windows Command Prompt (cmd) and type:\n\npip install --upgrade dcspy\n\nNote: command copied to clipboard.')
+            CTkMessagebox(title='New version',
+                          message='OLD WAY\n1. Open Windows Command Prompt (cmd) and type:\n2. pip install --upgrade dcspy\n'
+                                  '3. Note: command copied to clipboard.\n\nNEW WAY:\n1. Download new executable from: github.com/emcek/dcspy')
+            self.sys_tray_icon.notify(f'New version: {ver_string}', 'DCSpy')
         elif 'latest' in ver_string:
             CTkMessagebox(title='No updates', message='You are running latest version')
         elif 'failed' in ver_string:
             CTkMessagebox(title='Warning', message='Unable to check DCSpy version online', icon='warning', option_1='OK')
 
     def _auto_update_bios(self, silence=False) -> None:
         """
@@ -707,28 +745,44 @@
             LOG.debug(f'{err.__class__.__name__}: {err.filename}')
             copy(src=temp_dir / lua, dst=lua_dst_path)
             LOG.debug(f'Copy Export.lua from: {temp_dir} to {lua_dst_path} ')
         else:
             result += check_dcs_bios_entry(lua_dst_data, lua_dst_path, temp_dir)
         return result
 
+    def _show_gui(self) -> None:
+        """Show main GUI application window from system tray."""
+        self.master.after(0, self.master.deiconify)
+
     def _stop(self) -> None:
         """Set event to stop DCSpy."""
         self.status_txt.set('Start again or close DCSpy')
         self.btn_start.configure(state=tk.ACTIVE)
         self.btn_stop.configure(state=tk.DISABLED)
         self.event.set()
 
-    def start_dcspy(self) -> None:
-        """Run real application."""
+    def _close_gui(self) -> None:
+        """
+        Quit DCSpy application.
+
+        * Stop system tray
+        * Stop dcspy thread
+        * Quit GUI window
+        """
+        self.sys_tray_icon.visible = False
+        self.sys_tray_icon.stop()
+        self.event.set()
+        self.master.quit()
+
+    def _start_dcspy(self) -> None:
+        """Run real application in thread."""
         self.event = Event()
         LOG.debug(f'Local DCS-BIOS version: {self._check_local_bios().ver}')
         keyboard = self.lcd_type.get()
         self._save_cfg()
         app_params = {'lcd_type': LCD_TYPES[keyboard]['type'], 'event': self.event}
         app_thread = Thread(target=dcspy_run, kwargs=app_params)
         app_thread.name = 'dcspy-app'
         LOG.debug(f'Starting thread {app_thread} for: {app_params}')
-        self.status_txt.set('You can close GUI')
         self.btn_start.configure(state=tk.DISABLED)
         self.btn_stop.configure(state=tk.ACTIVE)
         app_thread.start()
```

### Comparing `dcspy-2.0.0/dcspy/utils.py` & `dcspy-2.1.0/dcspy/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from datetime import datetime
 from logging import getLogger
 from os import environ, makedirs
 from pathlib import Path
 from re import search
 from shutil import rmtree
 from tempfile import gettempdir
-from typing import Dict, Union, Tuple, NamedTuple
+from typing import Dict, NamedTuple, Tuple, Union
 
 import git
 from git import Repo
 from git.exc import InvalidGitRepositoryError
 from packaging import version
 from psutil import process_iter
 from requests import get
-from yaml import load, FullLoader, parser, dump
+from yaml import FullLoader, dump, load, parser
 
 LOG = getLogger(__name__)
 ConfigDict = Dict[str, Union[str, int, bool]]
 defaults_cfg: ConfigDict = {
     'dcsbios': f'D:\\Users\\{environ.get("USERNAME", "UNKNOWN")}\\Saved Games\\DCS.openbeta\\Scripts\\DCS-BIOS',
     'dcs': 'C:\\Program Files\\Eagle Dynamics\\DCS World OpenBeta',
     'check_bios': True,
@@ -222,16 +222,16 @@
     Check if process is running and return its PID.
 
     If process name is not found, 0 (zero) is returned.
     :param name: process name
     :return: PID as int
     """
     for proc in process_iter(['pid', 'name']):
-        if name in proc.info['name']:
-            return proc.info['pid']
+        if name in proc.info['name']:  # type: ignore
+            return proc.info['pid']  # type: ignore
     return 0
 
 
 def check_dcs_ver(dcs_path: Path) -> Tuple[str, str]:
     """
     Check DCS version and release type.
```

### Comparing `dcspy-2.0.0/dcspy.egg-info/SOURCES.txt` & `dcspy-2.1.0/dcspy.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,28 @@
-.pre-commit-config.yaml
-CHANGELOG.md
-CODE_OF_CONDUCT.md
-CONTRIBUTING.md
 LICENSE.md
-MANIFEST.in
 README.md
-SECURITY.md
-file_version_info.txt
 pyproject.toml
-requirements.txt
-requirements_test.txt
-setup.cfg
-setup.py
 dcspy/G13.png
 dcspy/G15v1.png
 dcspy/G15v2.png
 dcspy/G19.png
 dcspy/G510.png
 dcspy/__init__.py
 dcspy/aircraft.py
 dcspy/config.yaml
 dcspy/dcsbios.py
 dcspy/dcspy.ico
 dcspy/dcspy.png
 dcspy/dcspy_white.ico
-dcspy/falconded.ttf
 dcspy/license.txt
 dcspy/log.py
 dcspy/logitech.py
 dcspy/py.typed
 dcspy/run.py
+dcspy/splash.png
 dcspy/starter.py
 dcspy/tk_gui.py
 dcspy/utils.py
 dcspy.egg-info/PKG-INFO
 dcspy.egg-info/SOURCES.txt
 dcspy.egg-info/dependency_links.txt
 dcspy.egg-info/entry_points.txt
```

### Comparing `dcspy-2.0.0/tests/test_aircraft.py` & `dcspy-2.1.0/tests/test_aircraft.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,64 @@
 from pathlib import Path
 from sys import platform
 from unittest.mock import patch
 
-import PIL
-from PIL import ImageChops
 from pytest import mark, raises
 
-from dcspy import LcdColor, LcdMono, LcdButton
-from tests.helpers import all_plane_list, set_bios_during_test
+from dcspy import LcdButton, LcdColor, LcdMono
+from tests.helpers import all_plane_list, compare_images, set_bios_during_test
 
 resources = Path(__file__).resolve().with_name('resources')
 
 
 # <=><=><=><=><=> Base Class <=><=><=><=><=>
-@mark.parametrize('model', all_plane_list)
+@mark.parametrize('model', all_plane_list, ids=[
+    'FA-18 Hornet',
+    'F-16C Viper',
+    'Ka-50 Black Shark II',
+    'Ka-50 Black Shark III',
+    'Mi-8MT Hip',
+    'Mi-24P Hind',
+    'AH-64D Apache',
+    'A-10C Warthog',
+    'A-10C II Tank Killer',
+    'F-14A',
+    'F-14B',
+    'AV-8B N/A Harrier'])
 def test_check_all_aircraft_inherit_from_correct_base_class(model, lcd_mono):
     from dcspy import aircraft
     airplane = getattr(aircraft, model)
     aircraft_model = airplane(lcd_mono)
     assert isinstance(aircraft_model, aircraft.Aircraft)
     assert issubclass(airplane, aircraft.Aircraft)
 
 
 @mark.parametrize('selector, data, value, c_func, effect, lcd', [
     ('field1', {'addr': 0xdeadbeef, 'len': 16, 'value': ''}, 'val1', 'logi_lcd_mono_set_background', [True], LcdMono),
     ('field2', {'addr': 0xdeadbeef, 'len': 16, 'value': ''}, 'val2', 'logi_lcd_color_set_background', [False, True], LcdColor),
-])
-def test_aircraft_base_class_set_bios_with_mono_color_lcd(selector, data, value, c_func, effect, lcd, aircraft):
+], ids=['Mono LCD', 'Color LCD'])
+def test_aircraft_base_class_set_bios(selector, data, value, c_func, effect, lcd, aircraft):
     from dcspy.sdk import lcd_sdk
     assert aircraft.bios_data == {}
     aircraft.bios_data = {selector: data}
     aircraft.lcd = lcd
     with patch.object(lcd_sdk, 'logi_lcd_is_connected', side_effect=effect), \
             patch.object(lcd_sdk, c_func, return_value=True), \
             patch.object(lcd_sdk, 'logi_lcd_update', return_value=True):
         assert aircraft.bios_data[selector]['value'] == ''
         assert aircraft.get_bios('none') == ''
         with raises(NotImplementedError):
             aircraft.set_bios(selector, value)
 
 
-@mark.parametrize('mode, c_func, lcd', [('1', 'logi_lcd_mono_set_background', LcdMono),
-                                        ('RGBA', 'logi_lcd_color_set_background', LcdColor)])
-def test_aircraft_base_class_prepare_img_with_mono_color_lcd(mode, c_func, lcd, aircraft):
+@mark.parametrize('c_func, lcd', [
+    ('logi_lcd_mono_set_background', LcdMono),
+    ('logi_lcd_color_set_background', LcdColor),
+], ids=['Mono LCD', 'Color LCD'])
+def test_aircraft_base_class_prepare_img(c_func, lcd, aircraft):
     from dcspy.sdk import lcd_sdk
     aircraft.lcd = lcd
     with patch.object(lcd_sdk, 'logi_lcd_is_connected', return_value=True), \
             patch.object(lcd_sdk, c_func, return_value=True), \
             patch.object(lcd_sdk, 'logi_lcd_update', return_value=True), \
             raises(NotImplementedError):
         aircraft.prepare_image()
@@ -147,29 +159,29 @@
     ('viper_color', LcdButton.OK, '\n'),
     ('apache_mono', LcdButton.NONE, '\n'),
     ('apache_mono', LcdButton.ONE, 'PLT_EUFD_IDM 0\nPLT_EUFD_IDM 1\n'),
     ('apache_mono', LcdButton.TWO, 'PLT_EUFD_RTS 0\nPLT_EUFD_RTS 1\n'),
     ('apache_mono', LcdButton.THREE, 'PLT_EUFD_PRESET 0\nPLT_EUFD_PRESET 1\n'),
     ('apache_mono', LcdButton.FOUR, 'PLT_EUFD_ENT 0\nPLT_EUFD_ENT 1\n'),
 ])
-def test_button_pressed_for_plane(plane, button, result, request):
+def test_button_pressed_for_planes(plane, button, result, request):
     plane = request.getfixturevalue(plane)
     assert plane.button_request(button) == result
 
 
 @mark.parametrize('button, result', [
     (LcdButton.NONE, '\n'),
     (LcdButton.LEFT, 'PLT_EUFD_WCA 0\nPLT_EUFD_WCA 1\n'),
     (LcdButton.RIGHT, 'PLT_EUFD_RTS 0\nPLT_EUFD_RTS 1\n'),
     (LcdButton.DOWN, 'PLT_EUFD_PRESET 0\nPLT_EUFD_PRESET 1\n'),
     (LcdButton.UP, 'PLT_EUFD_ENT 0\nPLT_EUFD_ENT 1\n'),
     (LcdButton.MENU, '\n'),
     (LcdButton.CANCEL, '\n'),
     (LcdButton.OK, '\n'),
-])
+], ids=['NONE', 'LEFT', 'RIGHT', 'DOWN', 'UP', 'MENU', 'CANCEL', 'OK'])
 def test_button_pressed_for_apache_color(button, result, apache_color):
     from dcspy.aircraft import ApacheEufdMode
     apache_color.mode = ApacheEufdMode.WCA
     assert apache_color.button_request(button) == result
 
 
 @mark.parametrize('plane, btn_name, btn, values', [
@@ -180,14 +192,26 @@
     ('viper_color', 'IFF_MASTER_KNB', LcdButton.LEFT, (1, 2, 3, 4, 3, 2, 1, 0, 1)),
     ('viper_color', 'IFF_ENABLE_SW', LcdButton.RIGHT, (1, 2, 1, 0, 1)),
     ('viper_color', 'IFF_M4_CODE_SW', LcdButton.DOWN, (1, 2, 1, 0, 1)),
     ('viper_color', 'IFF_M4_REPLY_SW', LcdButton.UP, (1, 2, 1, 0, 1)),
     ('hornet_color', 'HUD_ATT_SW', LcdButton.OK, (1, 2, 1, 0, 1)),
     ('hornet_color', 'IFEI_DWN_BTN', LcdButton.MENU, (1, 0, 1)),
     ('hornet_color', 'IFEI_UP_BTN', LcdButton.CANCEL, (1, 0, 1)),
+], ids=[
+    'ONE - Viper Mono',
+    'TWO - Viper Mono',
+    'THREE - Viper Mono',
+    'FOUR - Viper Mono',
+    'LEFT - Viper Color',
+    'RIGHT - Viper Color',
+    'DOWN - Viper Color',
+    'UP - Viper Color',
+    'OK - Hornet Color',
+    'MENU - Hornet Color',
+    'CANCEL - Hornet Color',
 ])
 def test_get_next_value_for_cycle_buttons(plane, btn_name, btn, values, request):
     from itertools import cycle
     plane = request.getfixturevalue(plane)
     assert not all([isinstance(cyc_btn, cycle) for cyc_btn in plane.cycle_buttons.values()])
     for val in values:
         assert plane.button_request(btn) == f'{btn_name} {val}\n'
@@ -236,237 +260,71 @@
 
 @mark.parametrize('plane, bios_pairs, mode', [
     ('apache_mono', [('PLT_EUFD_LINE1', 'ENGINE 1 OUT      |AFT FUEL LOW      |TAIL WHL LOCK SEL ')], 'IDM'),
     ('apache_mono', [('PLT_EUFD_LINE1', '                  |AFT FUEL LOW      |PRESET TUNE VHS ')], 'PRE'),
     ('apache_color', [('PLT_EUFD_LINE1', '                  |                  |TAIL WHL LOCK SEL ')], 'IDM'),
     ('apache_color', [('PLT_EUFD_LINE1', '                  |AFT FUEL LOW      |TAIL WHL LOCK SEL ')], 'IDM'),
     ('apache_color', [('PLT_EUFD_LINE1', 'ENGINE 1 OUT      |AFT FUEL LOW      |PRESET TUNE FM1 ')], 'PRE'),
-])
-def test_mode_switch_idm_pre_for_apache(plane, bios_pairs, mode, request):
+], ids=['Mono IDM', 'Mono PRE', 'Color IDM 1', 'Color IDM 2', 'Color PRE'])
+def test_apache_mode_switch_idm_pre_for_apache(plane, bios_pairs, mode, request):
     plane = request.getfixturevalue(plane)
     set_bios_during_test(plane, bios_pairs)
     assert plane.mode.name == mode
 
 
 # <=><=><=><=><=> Prepare Image <=><=><=><=><=>
-hornet_bios = [
-    ('UFC_SCRATCHPAD_STRING_1_DISPLAY', '11'),
-    ('UFC_SCRATCHPAD_STRING_2_DISPLAY', '22'),
-    ('UFC_SCRATCHPAD_NUMBER_DISPLAY', '1234567890'),
-    ('UFC_OPTION_DISPLAY_1', '1234'),
-    ('UFC_OPTION_DISPLAY_2', '2345'),
-    ('UFC_OPTION_DISPLAY_3', '3456'),
-    ('UFC_OPTION_DISPLAY_4', '4567'),
-    ('UFC_OPTION_DISPLAY_5', '5678'),
-    ('UFC_COMM1_DISPLAY', '11'),
-    ('UFC_COMM2_DISPLAY', '22'),
-    ('UFC_OPTION_CUEING_1', '1'),
-    ('UFC_OPTION_CUEING_2', '2'),
-    ('UFC_OPTION_CUEING_3', '3'),
-    ('UFC_OPTION_CUEING_4', '4'),
-    ('UFC_OPTION_CUEING_5', '5'),
-    ('IFEI_FUEL_DOWN', '123456'),
-    ('IFEI_FUEL_UP', '234567')
-]
-viper_bios = [
-    ('DED_LINE_1', "  INS  08.0/ 6        1a "),
-    ('DED_LINE_2', "  LAT *N 43o06.2'*       @"),
-    ('DED_LINE_3', "  LNG  E040o34.2'        "),
-    ('DED_LINE_4', " SALT      74FT          "),
-    ('DED_LINE_5', " THDG   25.0o   G/S    0 "),
-]
-shark_bios = [
-    ('PVI_LINE1_APOSTROPHE1', '`'),
-    ('PVI_LINE1_APOSTROPHE2', '`'),
-    ('PVI_LINE1_POINT', '1'),
-    ('PVI_LINE1_SIGN', '-'),
-    ('PVI_LINE1_TEXT', '123456'),
-    ('PVI_LINE2_APOSTROPHE1', '`'),
-    ('PVI_LINE2_APOSTROPHE2', '`'),
-    ('PVI_LINE2_POINT', '2'),
-    ('PVI_LINE2_SIGN', ' '),
-    ('PVI_LINE2_TEXT', '654321'),
-    ('AP_ALT_HOLD_LED', 1),
-    ('AP_BANK_HOLD_LED', 0),
-    ('AP_FD_LED', 1),
-    ('AP_HDG_HOLD_LED', 0),
-    ('AP_PITCH_HOLD_LED', 1)
-]
-hip_bios = [
-    ('LMP_AP_HDG_ON', 1),
-    ('LMP_AP_PITCH_ROLL_ON', 0),
-    ('LMP_AP_HEIGHT_ON', 1),
-    ('R863_CNL_SEL', 9),
-    ('R863_MOD', 1),
-    ('R863_FREQ', "123.525"),
-    ('R828_PRST_CHAN_SEL', 9),
-    ('YADRO1A_FREQ', "09091.9"),
-]
-hind_bios = [
-    ('PLT_R863_CHAN', 9),
-    ('PLT_R863_MODUL', 1),
-    ('PLT_R828_CHAN', 9),
-    ('JADRO_FREQ', "08082.8"),
-    ('PLT_SAU_HOVER_MODE_ON_L', 1),
-    ('PLT_SAU_ROUTE_MODE_ON_L', 0),
-    ('PLT_SAU_ALT_MODE_ON_L', 1),
-    ('PLT_SAU_H_ON_L', 0),
-    ('PLT_SAU_K_ON_L', 0),
-    ('PLT_SAU_T_ON_L', 0),
-    ('PLT_SAU_B_ON_L', 1),
-]
-apache_bios = [
-    ('PLT_EUFD_LINE8', '~<>VHF*  121.000   -----              121.500   -----   '),
-    ('PLT_EUFD_LINE9', ' ==UHF*  305.000   -----              305.000   -----   '),
-    ('PLT_EUFD_LINE10', ' ==FM1*   30.000   -----    NORM       30.000   -----   '),
-    ('PLT_EUFD_LINE11', ' ==FM2*   30.000   -----               30.000   -----   '),
-    ('PLT_EUFD_LINE12', ' ==HF *    2.0000A -----    LOW         2.0000A -----   ')
-]
-warthog_bios = [
-    ('VHFAM_FREQ1', '20'),
-    ('VHFAM_FREQ2', 1),
-    ('VHFAM_FREQ3', 1),
-    ('VHFAM_FREQ4', '30'),
-    ('VHFFM_FREQ1', '40'),
-    ('VHFFM_FREQ2', 2),
-    ('VHFFM_FREQ3', 2),
-    ('VHFFM_FREQ4', '50'),
-    ('UHF_100MHZ_SEL', '5'),
-    ('UHF_10MHZ_SEL', 3),
-    ('UHF_1MHZ_SEL', 2),
-    ('UHF_POINT1MHZ_SEL', 1),
-    ('UHF_POINT25_SEL', '25')
-]
-harrier_bios = [
-    ('UFC_SCRATCHPAD', '123456789012'),
-    ('UFC_COMM1_DISPLAY', '11'),
-    ('UFC_COMM2_DISPLAY', '22'),
-    ('AV8BNA_ODU_1_SELECT', '1'),
-    ('AV8BNA_ODU_1_Text', '1234'),
-    ('AV8BNA_ODU_2_SELECT', '2'),
-    ('AV8BNA_ODU_2_Text', '2345'),
-    ('AV8BNA_ODU_3_SELECT', '3'),
-    ('AV8BNA_ODU_3_Text', '3456'),
-    ('AV8BNA_ODU_4_SELECT', '4'),
-    ('AV8BNA_ODU_4_Text', '4567'),
-    ('AV8BNA_ODU_5_SELECT', '5'),
-    ('AV8BNA_ODU_5_Text', '5678')
-]
-
-
-@mark.parametrize('model, bios_pairs', [
-    ('hornet_mono', hornet_bios),
-    ('hornet_color', hornet_bios),
-    ('viper_mono', viper_bios),
-    ('viper_color', viper_bios),
-    ('shark_mono', shark_bios),
-    ('shark_color', shark_bios),
-    ('shark3_mono', shark_bios),
-    ('shark3_color', shark_bios),
-    ('hip_mono', hip_bios),
-    ('hip_color', hip_bios),
-    ('hind_mono', hind_bios),
-    ('hind_color', hind_bios),
-    ('apache_mono', apache_bios),
-    ('apache_color', apache_bios),
-    ('warthog_mono', warthog_bios),
-    ('warthog_color', warthog_bios),
-    ('warthog2_mono', warthog_bios),
-    ('warthog2_color', warthog_bios),
-    ('tomcata_mono', []),
-    ('tomcata_color', []),
-    ('tomcatb_mono', []),
-    ('tomcatb_color', []),
-    ('harrier_mono', harrier_bios),
-    ('harrier_color', harrier_bios),
-])
-def test_prepare_image_for_all_planes(model, bios_pairs, request):
-    aircraft_model = request.getfixturevalue(model)
+
+@mark.parametrize('lcd', ['mono', 'color'])
+@mark.parametrize('model', ['hornet', 'viper', 'shark', 'shark3', 'hip', 'hind', 'apache', 'warthog', 'warthog2', 'tomcata', 'tomcatb', 'harrier'])
+def test_prepare_image_for_all_planes(model, lcd, img_precision, request):
+    aircraft_model = request.getfixturevalue(f'{model}_{lcd}')
+    bios_pairs = request.getfixturevalue(f'{model}_{lcd}_bios')
     set_bios_during_test(aircraft_model, bios_pairs)
     img = aircraft_model.prepare_image()
-    assert isinstance(img, PIL.Image.Image)
-    ref_img = PIL.Image.open(resources / platform / f'{model}_{aircraft_model.__class__.__name__}.png')
-    assert img.tobytes() == ref_img.tobytes()
-    assert not ImageChops.difference(img, ref_img).getbbox()
+    assert compare_images(img=img, file_path=resources / platform / f'{model}_{lcd}_{aircraft_model.__class__.__name__}.png', precision=img_precision)
 
 
-def test_prepare_image_for_apache_mono_wca_mode(apache_mono):
+@mark.parametrize('model', ['apache_mono', 'apache_color'], ids=['Mono LCD', 'Color LCD'])
+def test_prepare_image_for_apache_wca_mode(model, img_precision, request):
     from dcspy.aircraft import ApacheEufdMode
+    apache = request.getfixturevalue(model)
     bios_pairs = [
         ('PLT_EUFD_LINE1', 'LOW ROTOR RPM     |RECTIFIER 2 FAIL  |CHARGER           '),
         ('PLT_EUFD_LINE2', 'ENGINE 2 OUT      |GENERATOR 2 FAIL  |TAIL WHL LOCK SEL '),
         ('PLT_EUFD_LINE3', 'ENGINE 1 OUT      |AFT FUEL LOW      |                  '),
         ('PLT_EUFD_LINE4', '                  |FORWARD FUEL LOW  |                  '),
         ('PLT_EUFD_LINE5', '                  |                  |                  ')
     ]
-    set_bios_during_test(apache_mono, bios_pairs)
-    apache_mono.mode = ApacheEufdMode.WCA
-    img = apache_mono.prepare_image()
-    assert isinstance(img, PIL.Image.Image)
-    ref_img = PIL.Image.open(resources / platform / 'apache_mono_wca_mode.png')
-    assert img.tobytes() == ref_img.tobytes()
-    assert not ImageChops.difference(img, ref_img).getbbox()
+    set_bios_during_test(apache, bios_pairs)
+    apache.mode = ApacheEufdMode.WCA
+    img = apache.prepare_image()
+    assert compare_images(img=img, file_path=resources / platform / f'{model}_wca_mode.png', precision=img_precision)
 
 
 # <=><=><=><=><=> Apache special <=><=><=><=><=>
-def test_apache_mono_wca_more_then_one_screen(apache_mono):
+@mark.parametrize('model', ['apache_mono', 'apache_color'], ids=['Mono LCD', 'Color LCD'])
+def test_apache_wca_more_then_one_screen_scrolled(model, img_precision, request):
     from dcspy.aircraft import ApacheEufdMode
+    apache = request.getfixturevalue(model)
     bios_pairs = [
         ('PLT_EUFD_LINE1', 'LOW ROTOR RPM     |RECTIFIER 2 FAIL  |CHARGER           '),
         ('PLT_EUFD_LINE2', 'ENGINE 2 OUT      |GENERATOR 2 FAIL  |TAIL WHL LOCK SEL '),
         ('PLT_EUFD_LINE3', 'ENGINE 1 OUT      |AFT FUEL LOW      |                  ')
     ]
-    set_bios_during_test(apache_mono, bios_pairs)
-    apache_mono.mode = ApacheEufdMode.WCA
+    set_bios_during_test(apache, bios_pairs)
+    apache.mode = ApacheEufdMode.WCA
 
-    for i in range(1, 5):
-        assert apache_mono.warning_line == i
-        apache_mono.warning_line += 1
-        apache_mono.prepare_image()
-    assert apache_mono.warning_line == 1
-    img = apache_mono.prepare_image()
-    assert isinstance(img, PIL.Image.Image)
-    ref_img = PIL.Image.open(resources / platform / 'apache_mono_wca_mode.png')
-    assert img.tobytes() == ref_img.tobytes()
-    assert not ImageChops.difference(img, ref_img).getbbox()
-
-
-apache_pre_mono_bios = [
-    ('PLT_EUFD_LINE1', 'LOW ROTOR RPM     |RECTIFIER 2 FAIL  |PRESET TUNE VHF   '),
-    ('PLT_EUFD_LINE2', 'ENGINE 2 OUT      |GENERATOR 2 FAIL  |!CO CMD   127.000 '),
-    ('PLT_EUFD_LINE3', 'ENGINE 1 OUT      |AFT FUEL LOW      | D/1/227  135.000 '),
-    ('PLT_EUFD_LINE4', '                  |FORWARD FUEL LOW  | JAAT     136.000 '),
-    ('PLT_EUFD_LINE5', '                  |                  | BDE/HIG  127.000 '),
-    ('PLT_EUFD_LINE6', '                                     | FAAD     125.000 '),
-    ('PLT_EUFD_LINE7', '                                     | JTAC     121.000 '),
-    ('PLT_EUFD_LINE8', '~<>VHF*  127.000   -----             | AWACS    141.000 '),
-    ('PLT_EUFD_LINE9', ' ==UHF*  305.000   -----             | FLIGHT   128.000 '),
-    ('PLT_EUFD_LINE10', ' ==FM1*   30.000   -----    NORM     | BATUMI   126.000 '),
-    ('PLT_EUFD_LINE11', ' ==FM2*   30.000   -----             | COMMAND  137.000 ')
-]
-apache_pre_color_bios = [
-    ('PLT_EUFD_LINE1', 'LOW ROTOR RPM     |RECTIFIER 2 FAIL  |PRESET TUNE VHF   '),
-    ('PLT_EUFD_LINE2', 'ENGINE 2 OUT      |GENERATOR 2 FAIL  |!CO CMD   127.000 '),
-    ('PLT_EUFD_LINE3', 'ENGINE 1 OUT      |AFT FUEL LOW      | D/1/227  135.000 '),
-    ('PLT_EUFD_LINE4', '                  |FORWARD FUEL LOW  | JAAT     136.000 '),
-    ('PLT_EUFD_LINE5', '                  |                  | BDE/HIG  127.000 '),
-    ('PLT_EUFD_LINE6', '                                     | FAAD     125.000 '),
-    ('PLT_EUFD_LINE7', '                                     | JTAC     121.000 '),
-    ('PLT_EUFD_LINE8', '~<>VHF*  127.000   -----             | AWACS    141.000 '),
-    ('PLT_EUFD_LINE9', ' ==UHF*  305.000   -----             | FLIGHT   128.000 '),
-    ('PLT_EUFD_LINE10', ' ==FM1*   30.000   -----    NORM     | BATUMI   126.000 '),
-    ('PLT_EUFD_LINE11', ' ==FM2*   30.000   -----             | COMMAND  137.000 ')
-]
-
-
-@mark.parametrize('model, bios_pairs, filename', [
-    ('apache_mono', apache_pre_mono_bios, 'apache_mono_pre_mode.png'),
-    ('apache_color', apache_pre_color_bios, 'apache_color_pre_mode.png')
-])
-def test_apache_pre_mode(model, bios_pairs, filename, request):
-    aircraft_model = request.getfixturevalue(model)
-    set_bios_during_test(aircraft_model, bios_pairs)
-    img = aircraft_model.prepare_image()
-    assert isinstance(img, PIL.Image.Image)
-    ref_img = PIL.Image.open(resources / platform / filename)
-    assert img.tobytes() == ref_img.tobytes()
-    assert not ImageChops.difference(img, ref_img).getbbox()
+    for i in range(1, 3):
+        assert apache.warning_line == i
+        apache.warning_line += 1
+        apache.prepare_image()
+    assert apache.warning_line == 3
+    img = apache.prepare_image()
+    assert compare_images(img=img, file_path=resources / platform / f'{model}_wca_mode_scroll.png', precision=img_precision)
+
+
+@mark.parametrize('model', ['apache_mono', 'apache_color'], ids=['Mono LCD', 'Color LCD'])
+def test_apache_pre_mode(model, apache_pre_mode_bios_data, img_precision, request):
+    apache = request.getfixturevalue(model)
+    set_bios_during_test(apache, apache_pre_mode_bios_data)
+    img = apache.prepare_image()
+    assert compare_images(img=img, file_path=resources / platform / f'{model}_pre_mode.png', precision=img_precision)
```

### Comparing `dcspy-2.0.0/tests/test_bios.py` & `dcspy-2.1.0/tests/test_bios.py`

 * *Files identical despite different names*

### Comparing `dcspy-2.0.0/tests/test_dcsbios.py` & `dcspy-2.1.0/tests/test_dcsbios.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,14 +111,15 @@
 
     buff = getattr(dcsbios, class_name)(parser=protocol_parser, callback=lambda x: x, **params)
     assert 'on_dcsbios_write' in dir(buff)
 
 
 def test_integer_buffer_callback(protocol_parser):
     from functools import partial
+
     from dcspy.dcsbios import IntegerBuffer
 
     def _callback(*args, **kwargs):
         assert args == (1,)
         assert kwargs == dict()
 
     IntegerBuffer(parser=protocol_parser, address=0x1938, mask=0x200, shift_by=0x9, callback=partial(_callback))
@@ -127,14 +128,15 @@
     protocol_parser.address = 0x1938
     protocol_parser.data = 0x927  # 0x827
     protocol_parser.process_byte(0x1)
 
 
 def test_string_buffer_callback(protocol_parser):
     from functools import partial
+
     from dcspy.dcsbios import StringBuffer
 
     def _callback(*args, **kwargs):
         assert args == (1,)
         assert kwargs == dict()
 
     StringBuffer(parser=protocol_parser, address=0x1930, max_length=1, callback=partial(_callback))
```

### Comparing `dcspy-2.0.0/tests/test_lcd_sdk.py` & `dcspy-2.1.0/tests/test_lcd_sdk.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,81 +1,107 @@
-from unittest.mock import Mock, patch, call
+from unittest.mock import Mock, call, patch
 
 from pytest import mark
 
 
-@mark.parametrize('function, args, result', [('logi_lcd_init', ('test', 1), False),
-                                             ('logi_lcd_is_connected', (1,), False),
-                                             ('logi_lcd_is_button_pressed', (1,), False),
-                                             ('logi_lcd_update', (), None),
-                                             ('logi_lcd_shutdown', (), None),
-                                             ('logi_lcd_mono_set_background', ([1, 2, 3],), False),
-                                             ('logi_lcd_mono_set_text', (1, ''), False),
-                                             ('logi_lcd_color_set_background', ([1, 2, 3],), False),
-                                             ('logi_lcd_color_set_title', ('', (1, 2, 3)), False),
-                                             ('logi_lcd_color_set_text', (1, '', (1, 2, 3)), False)])
+@mark.parametrize('function, args, result', [
+    ('logi_lcd_init', ('test', 1), False),
+    ('logi_lcd_is_connected', (1,), False),
+    ('logi_lcd_is_button_pressed', (1,), False),
+    ('logi_lcd_update', (), None),
+    ('logi_lcd_shutdown', (), None),
+    ('logi_lcd_mono_set_background', ([1, 2, 3],), False),
+    ('logi_lcd_mono_set_text', (1, ''), False),
+    ('logi_lcd_color_set_background', ([1, 2, 3],), False),
+    ('logi_lcd_color_set_title', ('', (1, 2, 3)), False),
+    ('logi_lcd_color_set_text', (1, '', (1, 2, 3)), False)
+], ids=[
+    'init',
+    'is connected',
+    'is button pressed',
+    'update',
+    'shutdown',
+    'mono set background',
+    'mono set text',
+    'color set background',
+    'color_set title',
+    'color set text',
+])
 def test_all_failure_cases(function, args, result):
     from dcspy.sdk import lcd_sdk
     lcd_sdk.LCD_DLL = None
     assert getattr(lcd_sdk, function)(*args) is result
 
 
-@mark.parametrize('py_func, c_func, args, result', [('logi_lcd_init', 'LogiLcdInit', ('test', 1), True),
-                                                    ('logi_lcd_is_connected', 'LogiLcdIsConnected', (1,), True),
-                                                    ('logi_lcd_is_button_pressed', 'LogiLcdIsButtonPressed', (1,), True),
-                                                    ('logi_lcd_update', 'LogiLcdUpdate', (), None),
-                                                    ('logi_lcd_shutdown', 'LogiLcdShutdown', (), None),
-                                                    ('logi_lcd_mono_set_background', 'LogiLcdMonoSetBackground', ([1, 2, 3],), True),
-                                                    ('logi_lcd_mono_set_text', 'LogiLcdMonoSetText', (1, ''), True),
-                                                    ('logi_lcd_color_set_background', 'LogiLcdColorSetBackground', ([(1,) * 2],), True),
-                                                    ('logi_lcd_color_set_title', 'LogiLcdColorSetTitle', ('', (1, 2, 3)), True),
-                                                    ('logi_lcd_color_set_text', 'LogiLcdColorSetText', (1, '', (1, 2, 3)), True)])
+@mark.parametrize('py_func, c_func, args, result', [
+    ('logi_lcd_init', 'LogiLcdInit', ('test', 1), True),
+    ('logi_lcd_is_connected', 'LogiLcdIsConnected', (1,), True),
+    ('logi_lcd_is_button_pressed', 'LogiLcdIsButtonPressed', (1,), True),
+    ('logi_lcd_update', 'LogiLcdUpdate', (), None),
+    ('logi_lcd_shutdown', 'LogiLcdShutdown', (), None),
+    ('logi_lcd_mono_set_background', 'LogiLcdMonoSetBackground', ([1, 2, 3],), True),
+    ('logi_lcd_mono_set_text', 'LogiLcdMonoSetText', (1, ''), True),
+    ('logi_lcd_color_set_background', 'LogiLcdColorSetBackground', ([(1,) * 2],), True),
+    ('logi_lcd_color_set_title', 'LogiLcdColorSetTitle', ('', (1, 2, 3)), True),
+    ('logi_lcd_color_set_text', 'LogiLcdColorSetText', (1, '', (1, 2, 3)), True)
+], ids=[
+    'init',
+    'is connected',
+    'is button pressed',
+    'update',
+    'shutdown',
+    'mono set background',
+    'mono set text',
+    'color set background',
+    'color_set title',
+    'color set text',
+])
 def test_all_success_cases(py_func, c_func, args, result):
     from dcspy.sdk import lcd_sdk
     mocked_c_func = Mock()
     mocked_c_func.return_value = result
     lcd_sdk.LCD_DLL = {c_func: mocked_c_func}
     assert getattr(lcd_sdk, py_func)(*args) is result
 
 
-@mark.parametrize('c_func, effect, lcd, size', [('logi_lcd_mono_set_background', [True], 1, (16, 4)),
-                                                ('logi_lcd_color_set_background', [False, True], 2, (32, 24))])
+@mark.parametrize('c_func, effect, lcd, size', [
+    ('logi_lcd_mono_set_background', [True], 1, (16, 4)),
+    ('logi_lcd_color_set_background', [False, True], 2, (32, 24))
+], ids=['Mono', 'Color'])
 def test_update_display(c_func, effect, lcd, size):
-    from dcspy.sdk import lcd_sdk
     from PIL import Image
+
+    from dcspy.sdk import lcd_sdk
     with patch.object(lcd_sdk, 'logi_lcd_is_connected', side_effect=effect) as connected, \
             patch.object(lcd_sdk, c_func, return_value=True) as set_background, \
             patch.object(lcd_sdk, 'logi_lcd_update', return_value=True):
         lcd_sdk.update_display(Image.new('1', (size[0], size[1]), 0))
         connected.assert_called_with(lcd)
         set_background.assert_called_once_with([0] * size[0] * size[1])
 
 
-@mark.parametrize('c_func, effect, lcd, list_txt', [('logi_lcd_mono_set_text', [True], 1,
-                                                     ['1', '2', '3', '4']),
-                                                    ('logi_lcd_color_set_text', [False, True], 2,
-                                                     ['1', '2', '3', '4', '5', '6', '7', '8'])])
+@mark.parametrize('c_func, effect, lcd, list_txt', [
+    ('logi_lcd_mono_set_text', [True], 1, ['1', '2', '3', '4']),
+    ('logi_lcd_color_set_text', [False, True], 2, ['1', '2', '3', '4', '5', '6', '7', '8'])
+], ids=['Mono', 'Color'])
 def test_update_text(c_func, effect, lcd, list_txt):
     from dcspy.sdk import lcd_sdk
     with patch.object(lcd_sdk, 'logi_lcd_is_connected', side_effect=effect) as connected:
         with patch.object(lcd_sdk, c_func, return_value=True) as set_text:
             with patch.object(lcd_sdk, 'logi_lcd_update', return_value=True):
                 lcd_sdk.update_text(list_txt)
                 connected.assert_called_with(lcd)
                 set_text.assert_has_calls([call(i, j) for i, j in enumerate(list_txt)])
 
 
-@mark.parametrize('c_funcs, effect, lcd, clear, text',
-                  [(('logi_lcd_mono_set_background', 'logi_lcd_mono_set_text'),
-                    [True], 1, [0] * 160 * 43,
-                    [call(0, ''), call(1, ''), call(2, ''), call(3, '')]),
-                   (('logi_lcd_color_set_background', 'logi_lcd_color_set_text'),
-                    [False, True], 2, [(0,) * 4] * 320 * 240,
-                    [call(0, ''), call(1, ''), call(2, ''), call(3, ''),
-                     call(4, ''), call(5, ''), call(6, ''), call(7, '')])])
+@mark.parametrize('c_funcs, effect, lcd, clear, text', [
+    (('logi_lcd_mono_set_background', 'logi_lcd_mono_set_text'), [True], 1, [0] * 160 * 43, [call(0, ''), call(1, ''), call(2, ''), call(3, '')]),
+    (('logi_lcd_color_set_background', 'logi_lcd_color_set_text'), [False, True], 2, [(0,) * 4] * 320 * 240,
+     [call(0, ''), call(1, ''), call(2, ''), call(3, ''), call(4, ''), call(5, ''), call(6, ''), call(7, '')])
+], ids=['Mono', 'Color'])
 def test_clear_display(c_funcs, effect, lcd, clear, text):
     from dcspy.sdk import lcd_sdk
     with patch.object(lcd_sdk, 'logi_lcd_is_connected', side_effect=effect) as connected, \
             patch.object(lcd_sdk, c_funcs[0], return_value=True) as set_background, \
             patch.object(lcd_sdk, c_funcs[1], return_value=True) as set_text, \
             patch.object(lcd_sdk, 'logi_lcd_update', return_value=True):
         lcd_sdk.clear_display(true_clear=True)
```

### Comparing `dcspy-2.0.0/tests/test_logitech.py` & `dcspy-2.1.0/tests/test_logitech.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from unittest.mock import call, patch
 
 from pytest import mark
 
-from dcspy import LcdType, LcdButton
+from dcspy import LcdButton, LcdMode, LcdType
 from dcspy.logitech import KeyboardColor, KeyboardMono
 from tests.helpers import all_plane_list
 
 
 def test_keyboard_base_basic_check(keyboard_base):
     from dcspy.sdk import lcd_sdk
 
@@ -17,100 +17,133 @@
     for test_string in data:
         assert test_string in logitech_repr
 
     with patch.object(lcd_sdk, 'clear_display', return_value=True):
         keyboard_base.clear()
 
 
-@mark.parametrize('pressed1, effect, chk_btn, calls, pressed2', [
-    (False, [False, False, False, True], LcdButton.FOUR, [call(1), call(2), call(4), call(8)], True),
-    (True, [True, False, False, False], LcdButton.NONE, [call(1)], True),
-    (False, [False, False, False, False], LcdButton.NONE, [call(1), call(2), call(4), call(8)], False),
-])
-def test_keyboard_mono_check_buttons(pressed1, effect, chk_btn, calls, pressed2, keyboard_mono):
+@mark.parametrize('keyboard, pressed1, effect, chk_btn, calls, pressed2', [
+    ('keyboard_mono', False, [False] * 3 + [True], LcdButton.FOUR, [call(1), call(2), call(4), call(8)], True),
+    ('keyboard_color', False, [False] * 4 + [True] + [False] * 2, LcdButton.OK, [call(256), call(512), call(4096), call(8192), call(1024)], True),
+    ('keyboard_mono', True, [True, False, False, False], LcdButton.NONE, [call(1)], True),
+    ('keyboard_color', True, [True] + [False] * 6, LcdButton.NONE, [call(256)], True),
+    ('keyboard_mono', False, [False] * 4, LcdButton.NONE, [call(1), call(2), call(4), call(8)], False),
+    ('keyboard_color', False, [False] * 8, LcdButton.NONE, [call(256), call(512), call(4096), call(8192), call(1024), call(2048), call(16384)], False),
+], ids=['Mono 4 Button', 'Color Ok Button', 'Mono None already_pressed', 'Color None already_pressed', 'Mono None Button', 'Color None Button'])
+def test_keyboard_mono_check_buttons(keyboard, pressed1, effect, chk_btn, calls, pressed2, request):
     from dcspy.sdk import lcd_sdk
-    keyboard_mono.already_pressed = pressed1
+    keyboard = request.getfixturevalue(keyboard)
+    keyboard.already_pressed = pressed1
     with patch.object(lcd_sdk, 'logi_lcd_is_button_pressed', side_effect=effect) as lcd_btn_pressed:
-        assert keyboard_mono.check_buttons() == chk_btn
+        assert keyboard.check_buttons() == chk_btn
     lcd_btn_pressed.assert_has_calls(calls)
-    assert keyboard_mono.already_pressed is pressed2
+    assert keyboard.already_pressed is pressed2
 
 
-def test_keyboard_color_button_handle(keyboard_color, sock):
+@mark.parametrize('keyboard', ['keyboard_mono', 'keyboard_color'], ids=['Mono Keyboard', 'Color Keyboard'])
+def test_keyboard_color_button_handle(keyboard, sock, request):
     from dcspy.sdk import lcd_sdk
+    keyboard = request.getfixturevalue(keyboard)
     with patch.object(lcd_sdk, 'logi_lcd_is_button_pressed', side_effect=[True]):
-        keyboard_color.button_handle(sock)
+        keyboard.button_handle(sock)
     sock.sendto.assert_called_once_with(b'\n', ('127.0.0.1', 7778))
 
 
 @mark.parametrize('plane_str, plane, display, detect', [
     ('FA-18C_hornet', 'FA18Chornet', ['Detected aircraft:', 'F/A-18C Hornet'], True),
     ('F-16C_50', 'F16C50', ['Detected aircraft:', 'F-16C Viper'], True),
     ('Ka-50', 'Ka50', ['Detected aircraft:', 'Ka-50 Black Shark II'], True),
     ('Ka-503', 'Ka503', ['Detected aircraft:', 'Ka-50 Black Shark III'], True),
     ('Mi-8MT', 'Mi8MT', ['Detected aircraft:', 'Mi-8MTV2 Magnificent Eight'], True),
     ('Mi-24P', 'Mi24P', ['Detected aircraft:', 'Mi-24P Hind'], True),
     ('AH-64D_BLKII', 'AH64DBLKII', ['Detected aircraft:', 'AH-64D Apache'], True),
     ('A-10C', 'A10C', ['Detected aircraft:', 'A-10C Warthog'], True),
     ('A-10C_2', 'A10C2', ['Detected aircraft:', 'A-10C II Tank Killer'], True),
-    ('F-14B', 'F14B', ['Detected aircraft:', 'F-14B Tomcat'], True),
     ('F14A135GR', 'F14A135GR', ['Detected aircraft:', 'F-14A Tomcat'], True),
+    ('F-14B', 'F14B', ['Detected aircraft:', 'F-14B Tomcat'], True),
     ('AV8BNA', 'AV8BNA', ['Detected aircraft:', 'AV-8B N/A Harrier'], True),
     ('F-117_Nighthawk', 'F117Nighthawk', ['Detected aircraft:', 'F117Nighthawk', 'Not supported yet!'], False),
     ('', '', [], False),
-])
+], ids=['FA-18 Hornet',
+        'F-16C Viper',
+        'Ka-50 Black Shark II',
+        'Ka-50 Black Shark III',
+        'Mi-8MT Hip',
+        'Mi-24P Hind',
+        'AH-64D Apache',
+        'A-10C Warthog',
+        'A-10C II Tank Killer',
+        'F-14A',
+        'F-14B',
+        'AV-8B N/A Harrier',
+        'F-117 Nighthawk',
+        'Empty'])
 def test_keyboard_mono_detecting_plane(plane_str, plane, display, detect, keyboard_mono):
     from dcspy.sdk import lcd_sdk
     with patch.object(lcd_sdk, 'logi_lcd_is_connected', return_value=True), \
             patch.object(lcd_sdk, 'logi_lcd_mono_set_background', return_value=True), \
             patch.object(lcd_sdk, 'logi_lcd_update', return_value=True):
         keyboard_mono.detecting_plane(plane_str)
     assert keyboard_mono.plane_name == plane
     assert keyboard_mono._display == display
     assert keyboard_mono.plane_detected is detect
 
 
-@mark.parametrize('mode, size,  lcd_type, keyboard', [('1', (160, 43), LcdType.MONO, KeyboardMono),
-                                                      ('RGBA', (320, 240), LcdType.COLOR, KeyboardColor)])
+@mark.parametrize('mode, size,  lcd_type, keyboard', [
+    (LcdMode.BLACK_WHITE, (160, 43), LcdType.MONO, KeyboardMono),
+    (LcdMode.TRUE_COLOR, (320, 240), LcdType.COLOR, KeyboardColor)
+], ids=['Mono Keyboard', 'Color Keyboard'])
 def test_check_keyboard_display_and_prepare_image(mode, size, lcd_type, keyboard, protocol_parser):
+    from dcspy import LcdInfo
     from dcspy.aircraft import Aircraft
     from dcspy.sdk import lcd_sdk
-    from dcspy import LcdInfo
 
     with patch.object(lcd_sdk, 'logi_lcd_init', return_value=True):
         keyboard = keyboard(protocol_parser)
     assert isinstance(keyboard.plane, Aircraft)
     assert isinstance(keyboard.lcd, LcdInfo)
     assert keyboard.lcd.type == lcd_type
     assert isinstance(keyboard.display, list)
     with patch.object(lcd_sdk, 'update_display', return_value=True):
         keyboard.display = ['1', '2']
         assert len(keyboard.display) == 2
 
     img = keyboard._prepare_image()
-    assert img.mode == mode
+    assert img.mode == mode.value
     assert img.size == size
 
 
-@mark.parametrize('keyboard', [KeyboardMono, KeyboardColor])
+@mark.parametrize('keyboard', [KeyboardMono, KeyboardColor], ids=['Mono Keyboard', 'Color Keyboard'])
 def test_check_keyboard_text(keyboard, protocol_parser):
     from dcspy.sdk import lcd_sdk
 
     with patch.object(lcd_sdk, 'logi_lcd_init', return_value=True):
         keyboard = keyboard(protocol_parser)
 
     with patch.object(lcd_sdk, 'update_text', return_value=True) as upd_txt:
         keyboard.text(['1', '2'])
         upd_txt.assert_called()
 
 
-@mark.parametrize('model', all_plane_list)
+@mark.parametrize('model', all_plane_list, ids=[
+    'FA-18 Hornet',
+    'F-16C Viper',
+    'Ka-50 Black Shark II',
+    'Ka-50 Black Shark III',
+    'Mi-8MT Hip',
+    'Mi-24P Hind',
+    'AH-64D Apache',
+    'A-10C Warthog',
+    'A-10C II Tank Killer',
+    'F-14A',
+    'F-14B',
+    'AV-8B N/A Harrier'])
 def test_keyboard_mono_load_plane(model, keyboard_mono):
-    from dcspy.sdk import lcd_sdk
     from dcspy.aircraft import Aircraft
+    from dcspy.sdk import lcd_sdk
     with patch.object(lcd_sdk, 'logi_lcd_is_connected', return_value=True), \
             patch.object(lcd_sdk, 'logi_lcd_mono_set_background', return_value=True), \
             patch.object(lcd_sdk, 'logi_lcd_update', return_value=True):
         keyboard_mono.plane_name = model
         keyboard_mono.load_new_plane()
     assert isinstance(keyboard_mono.plane, Aircraft)
     assert model in keyboard_mono.plane.__class__.__name__
```

### Comparing `dcspy-2.0.0/tests/test_starter.py` & `dcspy-2.1.0/tests/test_starter.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,17 @@
     from dcspy import starter
     with patch.object(starter, 'LogitechKeyboard') as lcd:
         starter._load_new_plane_if_detected(lcd)
         lcd.load_new_plane.assert_called_once_with()
 
 
 def test_sock_err_handler():
-    from dcspy import starter
     from time import time
+
+    from dcspy import starter
     ver_string = f'v{starter.__version__} (latest)'
     start_time = time()
     with patch.object(starter, 'LogitechKeyboard') as logi_key:
         starter._sock_err_handler(logi_keyboard=logi_key, start_time=start_time, ver_string=ver_string,
                                   support_iter=(i for i in '12'), exp=Exception())
         assert logi_key.display == ['Logitech LCD OK', 'No data from DCS:   00:00', '1', ver_string]
```

### Comparing `dcspy-2.0.0/tests/test_utils.py` & `dcspy-2.1.0/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from pathlib import Path
-from unittest.mock import patch, PropertyMock, MagicMock, mock_open
+from unittest.mock import MagicMock, PropertyMock, mock_open, patch
 
 from packaging import version
 from pytest import mark
 
 from dcspy import utils
 
 
 @mark.parametrize('online_tag, result', [
     ('1.1.1', utils.ReleaseInfo(True, version.parse('1.1.1'), 'github.com/fake.tgz', '09 August 2021', 'Pre-release', 'fake.tgz')),
     ('3.2.1', utils.ReleaseInfo(False, version.parse('3.2.1'), 'github.com/fake.tgz', '09 August 2021', 'Pre-release', 'fake.tgz'))
-])
+], ids=['No update', 'New version'])
 def test_check_ver_is_possible(online_tag, result):
     with patch.object(utils, 'get') as response_get:
         type(response_get.return_value).ok = PropertyMock(return_value=True)
         type(response_get.return_value).json = MagicMock(return_value={'tag_name': online_tag, 'prerelease': True,
                                                                        'assets': [{'browser_download_url': 'github.com/fake.tgz'}],
                                                                        'published_at': '2021-08-09T16:41:51Z'})
         assert utils.check_ver_at_github(repo='fake1/package1', current_ver='1.1.1') == result
@@ -30,15 +30,15 @@
     with patch.object(utils, 'get', side_effect=Exception('Connection error')):
         assert utils.check_ver_at_github(repo='fake3/package3', current_ver='3.3.3') == utils.ReleaseInfo(False, version.parse('unknown'), '', '', 'Regular', '')
 
 
 @mark.parametrize('online_tag, result', [
     ('1.1.1', 'v1.1.1 (latest)'),
     ('3.2.1', 'v1.1.1 (please update!)')
-])
+], ids=['No update', 'New version'])
 def test_get_version_string_is_possible(online_tag, result):
     with patch.object(utils, 'get') as response_get:
         type(response_get.return_value).ok = PropertyMock(return_value=True)
         type(response_get.return_value).json = MagicMock(return_value={'tag_name': online_tag, 'prerelease': True,
                                                                        'assets': [{'browser_download_url': 'github.com/fake.tgz'}],
                                                                        'published_at': '2021-08-09T16:41:51Z'})
         assert utils.get_version_string(repo='fake1/package1', current_ver='1.1.1', check=True) == result
@@ -49,15 +49,15 @@
 
 
 def test_get_version_string_exception():
     with patch.object(utils, 'get', side_effect=Exception('Connection error')):
         assert utils.get_version_string(repo='fake4/package4', current_ver='4.4.4', check=True) == 'v4.4.4 (failed)'
 
 
-@mark.parametrize('response, result', [(False, False), (True, True)])
+@mark.parametrize('response, result', [(False, False), (True, True)], ids=['Download failed', 'Download success'])
 def test_download_file(response, result, tmp_path):
     dl_file = str(tmp_path / 'tmp.txt')
     with patch.object(utils, 'get') as response_get:
         type(response_get.return_value).ok = PropertyMock(return_value=response)
         type(response_get.return_value).iter_content = MagicMock(return_value=[b'1', b'0', b'0', b'1'])
         assert utils.download_file('https://test.com', dl_file) is result
```

