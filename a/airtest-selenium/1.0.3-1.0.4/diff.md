# Comparing `tmp/airtest-selenium-1.0.3.tar.gz` & `tmp/airtest-selenium-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\airtest-selenium-1.0.3.tar", last modified: Thu Sep  5 04:01:39 2019, max compression
+gzip compressed data, was "dist\airtest-selenium-1.0.4.tar", last modified: Tue May 30 03:53:28 2023, max compression
```

## Comparing `airtest-selenium-1.0.3.tar` & `airtest-selenium-1.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2019-09-05 04:01:39.000000 airtest-selenium-1.0.3/
-drwxrwxrwx   0        0        0        0 2019-09-05 04:01:39.000000 airtest-selenium-1.0.3/airtest_selenium/
--rw-rw-rw-   0        0        0     1543 2018-08-24 02:07:19.000000 airtest-selenium-1.0.3/airtest_selenium/exceptions.py
--rw-rw-rw-   0        0        0    32159 2019-09-05 03:53:27.000000 airtest-selenium-1.0.3/airtest_selenium/proxy.py
--rw-rw-rw-   0        0        0     4266 2019-09-05 03:53:27.000000 airtest-selenium-1.0.3/airtest_selenium/report.py
-drwxrwxrwx   0        0        0        0 2019-09-05 04:01:39.000000 airtest-selenium-1.0.3/airtest_selenium/utils/
--rw-rw-rw-   0        0        0     2599 2019-09-05 03:48:24.000000 airtest-selenium-1.0.3/airtest_selenium/utils/airtest_api.py
--rw-rw-rw-   0        0        0    30966 2018-08-24 02:07:19.000000 airtest-selenium-1.0.3/airtest_selenium/utils/six.py
--rw-rw-rw-   0        0        0        0 2018-08-24 02:07:19.000000 airtest-selenium-1.0.3/airtest_selenium/utils/__init__.py
--rw-rw-rw-   0        0        0       39 2018-08-24 02:07:19.000000 airtest-selenium-1.0.3/airtest_selenium/__init__.py
-drwxrwxrwx   0        0        0        0 2019-09-05 04:01:39.000000 airtest-selenium-1.0.3/airtest_selenium.egg-info/
--rw-rw-rw-   0        0        0        1 2019-09-05 04:01:39.000000 airtest-selenium-1.0.3/airtest_selenium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      449 2019-09-05 04:01:39.000000 airtest-selenium-1.0.3/airtest_selenium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       17 2019-09-05 04:01:39.000000 airtest-selenium-1.0.3/airtest_selenium.egg-info/requires.txt
--rw-rw-rw-   0        0        0      470 2019-09-05 04:01:39.000000 airtest-selenium-1.0.3/airtest_selenium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       17 2019-09-05 04:01:39.000000 airtest-selenium-1.0.3/airtest_selenium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11556 2018-06-26 11:06:39.000000 airtest-selenium-1.0.3/LICENSE
--rw-rw-rw-   0        0        0       76 2018-08-24 02:07:19.000000 airtest-selenium-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      449 2019-09-05 04:01:39.000000 airtest-selenium-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1440 2019-09-05 03:53:27.000000 airtest-selenium-1.0.3/README.md
--rw-rw-rw-   0        0        0       19 2018-08-24 02:07:19.000000 airtest-selenium-1.0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2019-09-05 04:01:39.000000 airtest-selenium-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      955 2019-09-05 04:00:58.000000 airtest-selenium-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 03:53:28.000000 airtest-selenium-1.0.4/
+drwxrwxrwx   0        0        0        0 2023-05-30 03:53:28.000000 airtest-selenium-1.0.4/airtest_selenium/
+-rw-rw-rw-   0        0        0     1543 2018-08-24 02:07:19.000000 airtest-selenium-1.0.4/airtest_selenium/exceptions.py
+-rw-rw-rw-   0        0        0    32234 2023-05-30 03:39:06.000000 airtest-selenium-1.0.4/airtest_selenium/proxy.py
+-rw-rw-rw-   0        0        0     5166 2020-07-28 03:58:43.000000 airtest-selenium-1.0.4/airtest_selenium/report.py
+drwxrwxrwx   0        0        0        0 2023-05-30 03:53:28.000000 airtest-selenium-1.0.4/airtest_selenium/utils/
+-rw-rw-rw-   0        0        0     2676 2020-07-24 09:57:07.000000 airtest-selenium-1.0.4/airtest_selenium/utils/airtest_api.py
+-rw-rw-rw-   0        0        0    30966 2018-08-24 02:07:19.000000 airtest-selenium-1.0.4/airtest_selenium/utils/six.py
+-rw-rw-rw-   0        0        0        0 2018-08-24 02:07:19.000000 airtest-selenium-1.0.4/airtest_selenium/utils/__init__.py
+-rw-rw-rw-   0        0        0       39 2018-08-24 02:07:19.000000 airtest-selenium-1.0.4/airtest_selenium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 03:53:28.000000 airtest-selenium-1.0.4/airtest_selenium.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-05-30 03:53:28.000000 airtest-selenium-1.0.4/airtest_selenium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      417 2023-05-30 03:53:28.000000 airtest-selenium-1.0.4/airtest_selenium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2023-05-30 03:53:28.000000 airtest-selenium-1.0.4/airtest_selenium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      470 2023-05-30 03:53:28.000000 airtest-selenium-1.0.4/airtest_selenium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       17 2023-05-30 03:53:28.000000 airtest-selenium-1.0.4/airtest_selenium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11556 2018-06-26 11:06:39.000000 airtest-selenium-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0       76 2018-08-24 02:07:19.000000 airtest-selenium-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      417 2023-05-30 03:53:28.000000 airtest-selenium-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1440 2019-09-05 03:53:27.000000 airtest-selenium-1.0.4/README.md
+-rw-rw-rw-   0        0        0       19 2018-08-24 02:07:19.000000 airtest-selenium-1.0.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 03:53:28.000000 airtest-selenium-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      923 2023-05-30 03:49:21.000000 airtest-selenium-1.0.4/setup.py
```

### Comparing `airtest-selenium-1.0.3/airtest_selenium/exceptions.py` & `airtest-selenium-1.0.4/airtest_selenium/exceptions.py`

 * *Files identical despite different names*

### Comparing `airtest-selenium-1.0.3/airtest_selenium/proxy.py` & `airtest-selenium-1.0.4/airtest_selenium/proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from selenium.webdriver import Chrome, ActionChains, Firefox, Remote
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.common.exceptions import NoSuchElementException
 from airtest.core.settings import Settings as ST
 from airtest.core.helper import logwrap
 from airtest import aircv
 from airtest.core.cv import Template
-from airtest_selenium.utils.airtest_api import loop_find
+from airtest_selenium.utils.airtest_api import loop_find, try_log_screen
 from airtest_selenium.exceptions import IsNotTemplateError
 from airtest.aircv import get_resolution
 from pynput.mouse import Controller, Button
 from airtest.core.error import TargetNotFoundError
 import os
 import time
 import sys
@@ -217,14 +217,16 @@
             v: target to touch, either a Template instance or absolute coordinates (x, y)
         Returns:
             Finial position to be clicked.
         """
         if isinstance(v, Template):
             _pos = loop_find(v, timeout=ST.FIND_TIMEOUT, driver=self)
         else:
+            screen = self.screenshot()
+            try_log_screen(screen)
             _pos = v
         x, y = _pos
         # self.action_chains.move_to_element_with_offset(root_element, x, y)
         # self.action_chains.click()
         pos = self._get_left_up_offset()
         pos = (pos[0] + x, pos[1] + y)
         self._move_to_pos(pos)
@@ -644,15 +646,15 @@
 
     def __init__(self, firefox_profile=None, firefox_binary=None,
                  timeout=30, capabilities=None, proxy=None,
                  executable_path="geckodriver", options=None, firefox_options=None,
                  service_args=None, desired_capabilities=None, log_path=None):
         print("Please make sure your geckodriver is in your path before proceeding using this driver")
         super(WebFirefox, self).__init__(firefox_profile=firefox_profile, firefox_binary=firefox_binary,
-                 timeout=timeout, capabilities=capabilities, proxy=proxy,
+                 capabilities=capabilities, proxy=proxy,
                  executable_path=executable_path, options=options, firefox_options=firefox_options,
                  service_args=service_args, desired_capabilities=desired_capabilities, log_path=log_path)
         self.father_number = {0: 0}
         self.action_chains = ActionChains(self)
         self.number = 0
         self.mouse = Controller()
         self.operation_to_func = {"xpath": self.find_element_by_xpath, "id": self.find_element_by_id,
```

### Comparing `airtest-selenium-1.0.3/airtest_selenium/report.py` & `airtest-selenium-1.0.4/airtest_selenium/report.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,267 +1,323 @@
 00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
 00000010: 662d 3820 2d2a 2d0d 0a69 6d70 6f72 7420  f-8 -*-..import 
-00000020: 6f73 0d0a 696d 706f 7274 2061 6972 7465  os..import airte
-00000030: 7374 2e72 6570 6f72 742e 7265 706f 7274  st.report.report
-00000040: 2061 7320 7265 706f 7274 0d0a 0d0a 4c4f   as report....LO
-00000050: 4744 4952 203d 2022 6c6f 6722 0d0a 0d0a  GDIR = "log"....
-00000060: 6f6c 645f 7472 616e 735f 7363 7265 656e  old_trans_screen
-00000070: 203d 2072 6570 6f72 742e 4c6f 6754 6f48   = report.LogToH
-00000080: 746d 6c2e 5f74 7261 6e73 6c61 7465 5f73  tml._translate_s
-00000090: 6372 6565 6e0d 0a6f 6c64 5f74 7261 6e73  creen..old_trans
-000000a0: 5f64 6573 6320 3d20 7265 706f 7274 2e4c  _desc = report.L
-000000b0: 6f67 546f 4874 6d6c 2e5f 7472 616e 736c  ogToHtml._transl
-000000c0: 6174 655f 6465 7363 0d0a 6f6c 645f 7472  ate_desc..old_tr
-000000d0: 616e 735f 636f 6465 203d 2072 6570 6f72  ans_code = repor
-000000e0: 742e 4c6f 6754 6f48 746d 6c2e 5f74 7261  t.LogToHtml._tra
-000000f0: 6e73 6c61 7465 5f63 6f64 650d 0a0d 0a73  nslate_code....s
-00000100: 6372 6565 6e5f 6675 6e63 203d 205b 2266  creen_func = ["f
-00000110: 696e 645f 656c 656d 656e 745f 6279 5f78  ind_element_by_x
-00000120: 7061 7468 222c 2022 6669 6e64 5f65 6c65  path", "find_ele
-00000130: 6d65 6e74 5f62 795f 6964 222c 2022 6669  ment_by_id", "fi
-00000140: 6e64 5f65 6c65 6d65 6e74 5f62 795f 6e61  nd_element_by_na
-00000150: 6d65 222c 2022 6173 7365 7274 5f65 7869  me", "assert_exi
-00000160: 7374 222c 0d0a 2020 2020 2020 2020 2020  st",..          
-00000170: 2020 2020 2022 6261 636b 222c 2022 666f       "back", "fo
-00000180: 7277 6172 6422 2c20 2273 7769 7463 685f  rward", "switch_
-00000190: 746f 5f6e 6577 5f74 6162 222c 2022 7377  to_new_tab", "sw
-000001a0: 6974 6368 5f74 6f5f 7072 6576 696f 7573  itch_to_previous
-000001b0: 5f74 6162 222c 2022 6765 7422 2c0d 0a20  _tab", "get",.. 
-000001c0: 2020 2020 2020 2020 2020 2020 2020 2263                "c
-000001d0: 6c69 636b 222c 2022 7365 6e64 5f6b 6579  lick", "send_key
-000001e0: 7322 5d0d 0a0d 0a73 6563 6f6e 645f 7363  s"]....second_sc
-000001f0: 7265 656e 5f66 756e 6320 3d20 5b22 636c  reen_func = ["cl
-00000200: 6963 6b22 2c20 2273 656e 645f 6b65 7973  ick", "send_keys
-00000210: 225d 0d0a 6f74 6865 725f 6675 6e63 203d  "]..other_func =
-00000220: 205b 5d0d 0a0d 0a64 6566 206e 6577 5f74   []....def new_t
-00000230: 7261 6e73 5f73 6372 6565 6e28 7365 6c66  rans_screen(self
-00000240: 2c20 7374 6570 2c20 636f 6465 293a 0d0a  , step, code):..
-00000250: 2020 2020 7472 616e 7320 3d20 6f6c 645f      trans = old_
-00000260: 7472 616e 735f 7363 7265 656e 2873 656c  trans_screen(sel
-00000270: 662c 2073 7465 702c 2063 6f64 6529 0d0a  f, step, code)..
-00000280: 2020 2020 6966 2022 6e61 6d65 2220 696e      if "name" in
-00000290: 2073 7465 705b 2764 6174 6127 5d20 616e   step['data'] an
-000002a0: 6420 7374 6570 5b27 6461 7461 275d 5b22  d step['data']["
-000002b0: 6e61 6d65 225d 2069 6e20 7363 7265 656e  name"] in screen
-000002c0: 5f66 756e 633a 0d0a 2020 2020 2020 2020  _func:..        
-000002d0: 7363 7265 656e 203d 207b 0d0a 2020 2020  screen = {..    
-000002e0: 2020 2020 2020 2020 2273 7263 223a 204e          "src": N
-000002f0: 6f6e 652c 0d0a 2020 2020 2020 2020 2020  one,..          
-00000300: 2020 2272 6563 7422 3a20 5b5d 2c0d 0a20    "rect": [],.. 
-00000310: 2020 2020 2020 2020 2020 2022 706f 7322             "pos"
-00000320: 3a20 5b5d 2c0d 0a20 2020 2020 2020 2020  : [],..         
-00000330: 2020 2022 7665 6374 6f72 223a 205b 5d2c     "vector": [],
-00000340: 0d0a 2020 2020 2020 2020 2020 2020 2263  ..            "c
-00000350: 6f6e 6669 6465 6e63 6522 3a20 4e6f 6e65  onfidence": None
-00000360: 2c0d 0a20 2020 2020 2020 207d 0d0a 0d0a  ,..        }....
-00000370: 2020 2020 2020 2020 7372 6320 3d20 2222          src = ""
-00000380: 0d0a 2020 2020 2020 2020 6966 2073 7465  ..        if ste
-00000390: 705b 2264 6174 6122 5d5b 226e 616d 6522  p["data"]["name"
-000003a0: 5d20 696e 2073 6563 6f6e 645f 7363 7265  ] in second_scre
-000003b0: 656e 5f66 756e 633a 0d0a 2020 2020 2020  en_func:..      
-000003c0: 2020 2020 2020 7265 7320 3d20 7374 6570        res = step
-000003d0: 5b22 6461 7461 225d 5b27 7265 7427 5d0d  ["data"]['ret'].
-000003e0: 0a20 2020 2020 2020 2020 2020 2073 7263  .            src
-000003f0: 203d 2072 6573 5b22 7363 7265 656e 225d   = res["screen"]
-00000400: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00000410: 2022 706f 7322 2069 6e20 7265 733a 0d0a   "pos" in res:..
-00000420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000430: 7363 7265 656e 5b22 706f 7322 5d20 3d20  screen["pos"] = 
-00000440: 7265 735b 2270 6f73 225d 0d0a 0d0a 2020  res["pos"]....  
-00000450: 2020 2020 2020 666f 7220 6974 656d 2069        for item i
-00000460: 6e20 7374 6570 5b22 5f5f 6368 696c 6472  n step["__childr
-00000470: 656e 5f5f 225d 3a0d 0a20 2020 2020 2020  en__"]:..       
-00000480: 2020 2020 2069 6620 6974 656d 5b22 6461       if item["da
-00000490: 7461 225d 5b22 6e61 6d65 225d 203d 3d20  ta"]["name"] == 
-000004a0: 225f 6765 6e5f 7363 7265 656e 5f6c 6f67  "_gen_screen_log
-000004b0: 223a 0d0a 2020 2020 2020 2020 2020 2020  ":..            
-000004c0: 2020 2020 7265 7320 3d20 6974 656d 5b22      res = item["
-000004d0: 6461 7461 225d 5b27 7265 7427 5d0d 0a20  data"]['ret'].. 
-000004e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000004f0: 7263 203d 2072 6573 5b22 7363 7265 656e  rc = res["screen
-00000500: 225d 0d0a 2020 2020 2020 2020 2020 2020  "]..            
-00000510: 2020 2020 6966 2022 706f 7322 2069 6e20      if "pos" in 
-00000520: 7265 733a 0d0a 2020 2020 2020 2020 2020  res:..          
-00000530: 2020 2020 2020 2020 2020 7363 7265 656e            screen
-00000540: 5b22 706f 7322 5d20 3d20 7265 735b 2270  ["pos"] = res["p
-00000550: 6f73 225d 0d0a 2020 2020 2020 2020 2020  os"]..          
-00000560: 2020 2020 2020 6272 6561 6b0d 0a0d 0a20        break.... 
-00000570: 2020 2020 2020 2069 6620 7365 6c66 2e65         if self.e
-00000580: 7870 6f72 745f 6469 7220 616e 6420 7372  xport_dir and sr
-00000590: 633a 0d0a 2020 2020 2020 2020 2020 2020  c:..            
-000005a0: 7372 6320 3d20 6f73 2e70 6174 682e 6a6f  src = os.path.jo
-000005b0: 696e 284c 4f47 4449 522c 2073 7263 290d  in(LOGDIR, src).
-000005c0: 0a20 2020 2020 2020 2073 6372 6565 6e5b  .        screen[
-000005d0: 2273 7263 225d 203d 2073 7263 0d0a 0d0a  "src"] = src....
-000005e0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000005f0: 6372 6565 6e0d 0a20 2020 2065 6c73 653a  creen..    else:
-00000600: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00000610: 2074 7261 6e73 0d0a 0d0a 6465 6620 6e65   trans....def ne
-00000620: 775f 7472 616e 736c 6174 655f 6465 7363  w_translate_desc
-00000630: 2873 656c 662c 2073 7465 702c 2063 6f64  (self, step, cod
-00000640: 6529 3a0d 0a20 2020 2074 7261 6e73 203d  e):..    trans =
-00000650: 206f 6c64 5f74 7261 6e73 5f64 6573 6328   old_trans_desc(
-00000660: 7365 6c66 2c20 7374 6570 2c20 636f 6465  self, step, code
-00000670: 290d 0a20 2020 2069 6620 226e 616d 6522  )..    if "name"
-00000680: 2069 6e20 7374 6570 5b27 6461 7461 275d   in step['data']
-00000690: 2061 6e64 2028 7374 6570 5b27 6461 7461   and (step['data
-000006a0: 275d 5b22 6e61 6d65 225d 2069 6e20 7363  ']["name"] in sc
-000006b0: 7265 656e 5f66 756e 6320 6f72 2073 7465  reen_func or ste
-000006c0: 705b 2264 6174 6122 5d5b 226e 616d 6522  p["data"]["name"
-000006d0: 5d20 696e 206f 7468 6572 5f66 756e 6329  ] in other_func)
-000006e0: 3a0d 0a20 2020 2020 2020 206e 616d 6520  :..        name 
-000006f0: 3d20 7374 6570 5b22 6461 7461 225d 5b22  = step["data"]["
-00000700: 6e61 6d65 225d 0d0a 2020 2020 2020 2020  name"]..        
-00000710: 6172 6773 203d 207b 695b 226b 6579 225d  args = {i["key"]
-00000720: 3a20 695b 2276 616c 7565 225d 2066 6f72  : i["value"] for
-00000730: 2069 2069 6e20 636f 6465 5b22 6172 6773   i in code["args
-00000740: 225d 7d0d 0a20 2020 2020 2020 2064 6573  "]}..        des
-00000750: 6320 3d20 7b0d 0a20 2020 2020 2020 2020  c = {..         
-00000760: 2020 2022 6669 6e64 5f65 6c65 6d65 6e74     "find_element
-00000770: 5f62 795f 7870 6174 6822 3a20 6c61 6d62  _by_xpath": lamb
-00000780: 6461 3a20 7522 4669 6e64 2065 6c65 6d65  da: u"Find eleme
-00000790: 6e74 2062 7920 7870 6174 683a 2025 7322  nt by xpath: %s"
-000007a0: 2025 2061 7267 732e 6765 7428 2278 7061   % args.get("xpa
-000007b0: 7468 2229 2c0d 0a20 2020 2020 2020 2020  th"),..         
-000007c0: 2020 2022 6669 6e64 5f65 6c65 6d65 6e74     "find_element
-000007d0: 5f62 795f 6964 223a 206c 616d 6264 613a  _by_id": lambda:
-000007e0: 2075 2246 696e 6420 656c 656d 656e 7420   u"Find element 
-000007f0: 6279 2069 643a 2025 7322 2025 2061 7267  by id: %s" % arg
-00000800: 732e 6765 7428 2269 6422 292c 0d0a 2020  s.get("id"),..  
-00000810: 2020 2020 2020 2020 2020 2266 696e 645f            "find_
-00000820: 656c 656d 656e 745f 6279 5f6e 616d 6522  element_by_name"
-00000830: 3a20 6c61 6d62 6461 3a20 7522 4669 6e64  : lambda: u"Find
-00000840: 2065 6c65 6d65 6e74 2062 7920 6e61 6d65   element by name
-00000850: 3a20 2573 2220 2520 6172 6773 2e67 6574  : %s" % args.get
-00000860: 2822 6e61 6d65 2229 2c0d 0a20 2020 2020  ("name"),..     
-00000870: 2020 2020 2020 2022 6173 7365 7274 5f65         "assert_e
-00000880: 7869 7374 223a 2075 2241 7373 6572 7420  xist": u"Assert 
-00000890: 656c 656d 656e 7420 6578 6973 7473 2e22  element exists."
-000008a0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-000008b0: 636c 6963 6b22 3a20 7522 436c 6963 6b20  click": u"Click 
-000008c0: 7468 6520 656c 656d 656e 7420 7468 6174  the element that
-000008d0: 2062 6565 6e20 666f 756e 642e 222c 0d0a   been found.",..
-000008e0: 2020 2020 2020 2020 2020 2020 2273 656e              "sen
-000008f0: 645f 6b65 7973 223a 2075 2253 656e 6420  d_keys": u"Send 
-00000900: 736f 6d65 2074 6578 7420 616e 6420 6b65  some text and ke
-00000910: 7962 6f61 7264 2065 7665 6e74 2074 6f20  yboard event to 
-00000920: 7468 6520 656c 656d 656e 7420 7468 6174  the element that
-00000930: 2062 6565 6e20 666f 756e 642e 222c 0d0a   been found.",..
-00000940: 2020 2020 2020 2020 2020 2020 2267 6574              "get
-00000950: 223a 206c 616d 6264 613a 2075 2247 6574  ": lambda: u"Get
-00000960: 2074 6865 2077 6562 2061 6464 7265 7373   the web address
-00000970: 3a20 2573 2220 2520 6172 6773 2e67 6574  : %s" % args.get
-00000980: 2822 6164 6472 6573 7322 292c 0d0a 2020  ("address"),..  
-00000990: 2020 2020 2020 2020 2020 2273 7769 7463            "switc
-000009a0: 685f 746f 5f6c 6173 745f 7769 6e64 6f77  h_to_last_window
-000009b0: 223a 2075 2253 7769 7463 6820 746f 2074  ": u"Switch to t
-000009c0: 6865 206c 6173 7420 7461 622e 222c 0d0a  he last tab.",..
-000009d0: 2020 2020 2020 2020 2020 2020 2273 7769              "swi
-000009e0: 7463 685f 746f 5f6c 6174 6573 745f 7769  tch_to_latest_wi
-000009f0: 6e64 6f77 223a 2075 2253 7769 7463 6820  ndow": u"Switch 
-00000a00: 746f 2074 6865 206e 6577 2074 6162 2e22  to the new tab."
-00000a10: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00000a20: 6261 636b 223a 2075 2242 6163 6b20 746f  back": u"Back to
-00000a30: 2074 6865 206c 6173 7420 7061 6765 2e22   the last page."
-00000a40: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00000a50: 666f 7277 6172 6422 3a20 7522 466f 7277  forward": u"Forw
-00000a60: 6172 6420 746f 2074 6865 206e 6578 7420  ard to the next 
-00000a70: 7061 6765 2e22 2c0d 0a20 2020 2020 2020  page.",..       
-00000a80: 2020 2020 2022 736e 6170 7368 6f74 223a       "snapshot":
-00000a90: 2075 2253 6e6f 7073 686f 7420 6375 7272   u"Snopshot curr
-00000aa0: 656e 7420 7061 6765 2e22 0d0a 2020 2020  ent page."..    
-00000ab0: 2020 2020 7d0d 0a0d 0a20 2020 2020 2020      }....       
-00000ac0: 2064 6573 635f 7a68 203d 207b 0d0a 2020   desc_zh = {..  
-00000ad0: 2020 2020 2020 2020 2020 2266 696e 645f            "find_
-00000ae0: 656c 656d 656e 745f 6279 5f78 7061 7468  element_by_xpath
-00000af0: 223a 206c 616d 6264 613a 2075 22e5 afbb  ": lambda: u"...
-00000b00: e689 bee6 8c87 e5ae 9ae9 a1b5 e99d a2e5  ................
-00000b10: 8583 e7b4 a03a 205c 2225 735c 2222 2025  .....: \"%s\"" %
-00000b20: 2061 7267 732e 6765 7428 2278 7061 7468   args.get("xpath
-00000b30: 2229 2c0d 0a20 2020 2020 2020 2020 2020  "),..           
-00000b40: 2022 6669 6e64 5f65 6c65 6d65 6e74 5f62   "find_element_b
-00000b50: 795f 6964 223a 206c 616d 6264 613a 2075  y_id": lambda: u
-00000b60: 22e5 afbb e689 bee6 8c87 e5ae 9ae9 a1b5  "...............
-00000b70: e99d a2e5 8583 e7b4 a03a 205c 2225 735c  .........: \"%s\
-00000b80: 2222 2025 2061 7267 732e 6765 7428 2269  "" % args.get("i
-00000b90: 6422 292c 0d0a 2020 2020 2020 2020 2020  d"),..          
-00000ba0: 2020 2266 696e 645f 656c 656d 656e 745f    "find_element_
-00000bb0: 6279 5f6e 616d 6522 3a20 6c61 6d62 6461  by_name": lambda
-00000bc0: 3a20 7522 e5af bbe6 89be e68c 87e5 ae9a  : u"............
-00000bd0: e9a1 b5e9 9da2 e585 83e7 b4a0 3a20 5c22  ............: \"
-00000be0: 2573 5c22 2220 2520 6172 6773 2e67 6574  %s\"" % args.get
-00000bf0: 2822 6e61 6d65 2229 2c0d 0a20 2020 2020  ("name"),..     
-00000c00: 2020 2020 2020 2022 6173 7365 7274 5f65         "assert_e
-00000c10: 7869 7374 223a 2075 22e6 96ad e8a8 80e9  xist": u".......
-00000c20: a1b5 e99d a2e5 8583 e7b4 a0e5 ad98 e59c  ................
-00000c30: a82e 222c 0d0a 2020 2020 2020 2020 2020  ..",..          
-00000c40: 2020 2263 6c69 636b 223a 2075 22e7 82b9    "click": u"...
-00000c50: e587 bbe6 89be e588 b0e7 9a84 e9a1 b5e9  ................
-00000c60: 9da2 e585 83e7 b4a0 2e22 2c0d 0a20 2020  .........",..   
-00000c70: 2020 2020 2020 2020 2022 7365 6e64 5f6b           "send_k
-00000c80: 6579 7322 3a20 7522 e4bc a0e9 8081 e696  eys": u"........
-00000c90: 87e6 9cac 5c22 2573 5c22 e588 b0e9 8089  ....\"%s\"......
-00000ca0: e4b8 ade6 9687 e69c ace6 a186 2e22 2025  ............." %
-00000cb0: 2028 6172 6773 2e67 6574 2822 7465 7874   (args.get("text
-00000cc0: 222c 2022 2229 292c 0d0a 2020 2020 2020  ", "")),..      
-00000cd0: 2020 2020 2020 2267 6574 223a 206c 616d        "get": lam
-00000ce0: 6264 613a 2075 22e8 aebf e997 aee7 bd91  bda: u".........
-00000cf0: e7bb 9ce5 9cb0 e59d 803a 2025 7322 2025  .........: %s" %
-00000d00: 2061 7267 732e 6765 7428 2261 6464 7265   args.get("addre
-00000d10: 7373 2229 2c0d 0a20 2020 2020 2020 2020  ss"),..         
-00000d20: 2020 2022 7377 6974 6368 5f74 6f5f 6c61     "switch_to_la
-00000d30: 7374 5f77 696e 646f 7722 3a20 7522 e588  st_window": u"..
-00000d40: 87e6 8da2 e588 b0e4 b88a e4b8 80e4 b8aa  ................
-00000d50: e6a0 87e7 adbe e9a1 b52e 222c 0d0a 2020  ..........",..  
-00000d60: 2020 2020 2020 2020 2020 2273 7769 7463            "switc
-00000d70: 685f 746f 5f6c 6174 6573 745f 7769 6e64  h_to_latest_wind
-00000d80: 6f77 223a 2075 22e5 8887 e68d a2e5 88b0  ow": u".........
-00000d90: e69c 80e6 96b0 e6a0 87e7 adbe e9a1 b52e  ................
-00000da0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00000db0: 2262 6163 6b22 3a20 7522 e590 8ee9 8080  "back": u"......
-00000dc0: e588 b0e4 b88a e4b8 80e4 b8aa e9a1 b5e9  ................
-00000dd0: 9da2 2e22 2c0d 0a20 2020 2020 2020 2020  ...",..         
-00000de0: 2020 2022 666f 7277 6172 6422 3a20 7522     "forward": u"
-00000df0: e589 8de8 bf9b e588 b0e4 b88b e4b8 80e4  ................
-00000e00: b8aa e9a1 b5e9 9da2 2e22 2c0d 0a20 2020  .........",..   
-00000e10: 2020 2020 2020 2020 2022 736e 6170 7368           "snapsh
-00000e20: 6f74 223a 2075 22e6 88aa e58f 96e5 bd93  ot": u".........
-00000e30: e589 8de9 a1b5 e99d a22e 220d 0a20 2020  .........."..   
-00000e40: 2020 2020 207d 0d0a 0d0a 2020 2020 2020       }....      
-00000e50: 2020 6966 2073 656c 662e 6c61 6e67 203d    if self.lang =
-00000e60: 3d20 277a 6827 3a0d 0a20 2020 2020 2020  = 'zh':..       
-00000e70: 2020 2020 2064 6573 6320 3d20 6465 7363       desc = desc
-00000e80: 5f7a 680d 0a20 2020 2020 2020 2072 6574  _zh..        ret
-00000e90: 203d 2064 6573 632e 6765 7428 6e61 6d65   = desc.get(name
-00000ea0: 290d 0a20 2020 2020 2020 2069 6620 6361  )..        if ca
-00000eb0: 6c6c 6162 6c65 2872 6574 293a 0d0a 2020  llable(ret):..  
-00000ec0: 2020 2020 2020 2020 2020 7265 7420 3d20            ret = 
-00000ed0: 7265 7428 290d 0a20 2020 2020 2020 2072  ret()..        r
-00000ee0: 6574 7572 6e20 7265 740d 0a20 2020 2065  eturn ret..    e
-00000ef0: 6c73 653a 0d0a 2020 2020 2020 2020 7265  lse:..        re
-00000f00: 7475 726e 2074 7261 6e73 0d0a 0d0a 6465  turn trans....de
-00000f10: 6620 6e65 775f 7472 616e 736c 6174 655f  f new_translate_
-00000f20: 636f 6465 2873 656c 662c 2073 7465 7029  code(self, step)
-00000f30: 3a0d 0a20 2020 2074 7261 6e73 203d 206f  :..    trans = o
-00000f40: 6c64 5f74 7261 6e73 5f63 6f64 6528 7365  ld_trans_code(se
-00000f50: 6c66 2c20 7374 6570 290d 0a20 2020 2069  lf, step)..    i
-00000f60: 6620 7472 616e 733a 0d0a 2020 2020 2020  f trans:..      
-00000f70: 2020 666f 7220 6964 782c 2069 7465 6d20    for idx, item 
-00000f80: 696e 2065 6e75 6d65 7261 7465 2874 7261  in enumerate(tra
-00000f90: 6e73 5b22 6172 6773 225d 293a 0d0a 2020  ns["args"]):..  
-00000fa0: 2020 2020 2020 2020 2020 6966 2069 7465            if ite
-00000fb0: 6d5b 226b 6579 225d 203d 3d20 2273 656c  m["key"] == "sel
-00000fc0: 6622 3a0d 0a20 2020 2020 2020 2020 2020  f":..           
-00000fd0: 2020 2020 2074 7261 6e73 5b22 6172 6773       trans["args
-00000fe0: 225d 2e70 6f70 2869 6478 290d 0a20 2020  "].pop(idx)..   
-00000ff0: 2072 6574 7572 6e20 7472 616e 730d 0a0d   return trans...
-00001000: 0a0d 0a72 6570 6f72 742e 4c6f 6754 6f48  ...report.LogToH
-00001010: 746d 6c2e 5f74 7261 6e73 6c61 7465 5f73  tml._translate_s
-00001020: 6372 6565 6e20 3d20 6e65 775f 7472 616e  creen = new_tran
-00001030: 735f 7363 7265 656e 0d0a 7265 706f 7274  s_screen..report
-00001040: 2e4c 6f67 546f 4874 6d6c 2e5f 7472 616e  .LogToHtml._tran
-00001050: 736c 6174 655f 6465 7363 203d 206e 6577  slate_desc = new
-00001060: 5f74 7261 6e73 6c61 7465 5f64 6573 630d  _translate_desc.
-00001070: 0a72 6570 6f72 742e 4c6f 6754 6f48 746d  .report.LogToHtm
-00001080: 6c2e 5f74 7261 6e73 6c61 7465 5f63 6f64  l._translate_cod
-00001090: 6520 3d20 6e65 775f 7472 616e 736c 6174  e = new_translat
-000010a0: 655f 636f 6465 0d0a 0d0a                 e_code....
+00000020: 6f73 0d0a 6672 6f6d 2075 726c 6c69 622e  os..from urllib.
+00000030: 7061 7273 6520 696d 706f 7274 2075 6e71  parse import unq
+00000040: 756f 7465 0d0a 696d 706f 7274 2061 6972  uote..import air
+00000050: 7465 7374 2e72 6570 6f72 742e 7265 706f  test.report.repo
+00000060: 7274 2061 7320 7265 706f 7274 0d0a 0d0a  rt as report....
+00000070: 4c4f 4744 4952 203d 2022 6c6f 6722 0d0a  LOGDIR = "log"..
+00000080: 0d0a 6f6c 645f 7472 616e 735f 7363 7265  ..old_trans_scre
+00000090: 656e 203d 2072 6570 6f72 742e 4c6f 6754  en = report.LogT
+000000a0: 6f48 746d 6c2e 5f74 7261 6e73 6c61 7465  oHtml._translate
+000000b0: 5f73 6372 6565 6e0d 0a6f 6c64 5f74 7261  _screen..old_tra
+000000c0: 6e73 5f64 6573 6320 3d20 7265 706f 7274  ns_desc = report
+000000d0: 2e4c 6f67 546f 4874 6d6c 2e5f 7472 616e  .LogToHtml._tran
+000000e0: 736c 6174 655f 6465 7363 0d0a 6f6c 645f  slate_desc..old_
+000000f0: 7472 616e 735f 636f 6465 203d 2072 6570  trans_code = rep
+00000100: 6f72 742e 4c6f 6754 6f48 746d 6c2e 5f74  ort.LogToHtml._t
+00000110: 7261 6e73 6c61 7465 5f63 6f64 650d 0a0d  ranslate_code...
+00000120: 0a73 6372 6565 6e5f 6675 6e63 203d 205b  .screen_func = [
+00000130: 2266 696e 645f 656c 656d 656e 745f 6279  "find_element_by
+00000140: 5f78 7061 7468 222c 2022 6669 6e64 5f65  _xpath", "find_e
+00000150: 6c65 6d65 6e74 5f62 795f 6964 222c 2022  lement_by_id", "
+00000160: 6669 6e64 5f65 6c65 6d65 6e74 5f62 795f  find_element_by_
+00000170: 6e61 6d65 222c 2022 6173 7365 7274 5f65  name", "assert_e
+00000180: 7869 7374 222c 0d0a 2020 2020 2020 2020  xist",..        
+00000190: 2020 2020 2020 2022 6261 636b 222c 2022         "back", "
+000001a0: 666f 7277 6172 6422 2c20 2273 7769 7463  forward", "switc
+000001b0: 685f 746f 5f6e 6577 5f74 6162 222c 2022  h_to_new_tab", "
+000001c0: 7377 6974 6368 5f74 6f5f 7072 6576 696f  switch_to_previo
+000001d0: 7573 5f74 6162 222c 2022 6765 7422 2c0d  us_tab", "get",.
+000001e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000001f0: 2263 6c69 636b 222c 2022 7365 6e64 5f6b  "click", "send_k
+00000200: 6579 7322 2c20 2273 6e61 7073 686f 7422  eys", "snapshot"
+00000210: 5d0d 0a0d 0a73 6563 6f6e 645f 7363 7265  ]....second_scre
+00000220: 656e 5f66 756e 6320 3d20 5b22 636c 6963  en_func = ["clic
+00000230: 6b22 2c20 2273 656e 645f 6b65 7973 225d  k", "send_keys"]
+00000240: 0d0a 6f74 6865 725f 6675 6e63 203d 205b  ..other_func = [
+00000250: 5d0d 0a0d 0a64 6566 206e 6577 5f74 7261  ]....def new_tra
+00000260: 6e73 5f73 6372 6565 6e28 7365 6c66 2c20  ns_screen(self, 
+00000270: 7374 6570 2c20 636f 6465 293a 0d0a 2020  step, code):..  
+00000280: 2020 7472 616e 7320 3d20 6f6c 645f 7472    trans = old_tr
+00000290: 616e 735f 7363 7265 656e 2873 656c 662c  ans_screen(self,
+000002a0: 2073 7465 702c 2063 6f64 6529 0d0a 2020   step, code)..  
+000002b0: 2020 6966 2022 6e61 6d65 2220 696e 2073    if "name" in s
+000002c0: 7465 705b 2764 6174 6127 5d20 616e 6420  tep['data'] and 
+000002d0: 7374 6570 5b27 6461 7461 275d 5b22 6e61  step['data']["na
+000002e0: 6d65 225d 2069 6e20 7363 7265 656e 5f66  me"] in screen_f
+000002f0: 756e 633a 0d0a 2020 2020 2020 2020 7363  unc:..        sc
+00000300: 7265 656e 203d 207b 0d0a 2020 2020 2020  reen = {..      
+00000310: 2020 2020 2020 2273 7263 223a 204e 6f6e        "src": Non
+00000320: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00000330: 2272 6563 7422 3a20 5b5d 2c0d 0a20 2020  "rect": [],..   
+00000340: 2020 2020 2020 2020 2022 706f 7322 3a20           "pos": 
+00000350: 5b5d 2c0d 0a20 2020 2020 2020 2020 2020  [],..           
+00000360: 2022 7665 6374 6f72 223a 205b 5d2c 0d0a   "vector": [],..
+00000370: 2020 2020 2020 2020 2020 2020 2263 6f6e              "con
+00000380: 6669 6465 6e63 6522 3a20 4e6f 6e65 2c0d  fidence": None,.
+00000390: 0a20 2020 2020 2020 207d 0d0a 0d0a 2020  .        }....  
+000003a0: 2020 2020 2020 7372 6320 3d20 2222 0d0a        src = ""..
+000003b0: 2020 2020 2020 2020 6966 2073 7465 705b          if step[
+000003c0: 2264 6174 6122 5d5b 226e 616d 6522 5d20  "data"]["name"] 
+000003d0: 696e 2073 6563 6f6e 645f 7363 7265 656e  in second_screen
+000003e0: 5f66 756e 633a 0d0a 2020 2020 2020 2020  _func:..        
+000003f0: 2020 2020 7265 7320 3d20 7374 6570 5b22      res = step["
+00000400: 6461 7461 225d 5b27 7265 7427 5d0d 0a20  data"]['ret'].. 
+00000410: 2020 2020 2020 2020 2020 2073 7263 203d             src =
+00000420: 2072 6573 5b22 7363 7265 656e 225d 0d0a   res["screen"]..
+00000430: 2020 2020 2020 2020 2020 2020 6966 2022              if "
+00000440: 706f 7322 2069 6e20 7265 733a 0d0a 2020  pos" in res:..  
+00000450: 2020 2020 2020 2020 2020 2020 2020 7363                sc
+00000460: 7265 656e 5b22 706f 7322 5d20 3d20 7265  reen["pos"] = re
+00000470: 735b 2270 6f73 225d 0d0a 0d0a 2020 2020  s["pos"]....    
+00000480: 2020 2020 666f 7220 6974 656d 2069 6e20      for item in 
+00000490: 7374 6570 5b22 5f5f 6368 696c 6472 656e  step["__children
+000004a0: 5f5f 225d 3a0d 0a20 2020 2020 2020 2020  __"]:..         
+000004b0: 2020 2069 6620 6974 656d 5b22 6461 7461     if item["data
+000004c0: 225d 5b22 6e61 6d65 225d 2069 6e20 5b22  "]["name"] in ["
+000004d0: 5f67 656e 5f73 6372 6565 6e5f 6c6f 6722  _gen_screen_log"
+000004e0: 2c20 2274 7279 5f6c 6f67 5f73 6372 6565  , "try_log_scree
+000004f0: 6e22 5d3a 0d0a 2020 2020 2020 2020 2020  n"]:..          
+00000500: 2020 2020 2020 7265 7320 3d20 6974 656d        res = item
+00000510: 5b22 6461 7461 225d 5b27 7265 7427 5d0d  ["data"]['ret'].
+00000520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000530: 2073 7263 203d 2072 6573 5b22 7363 7265   src = res["scre
+00000540: 656e 225d 0d0a 2020 2020 2020 2020 2020  en"]..          
+00000550: 2020 2020 2020 6966 2022 706f 7322 2069        if "pos" i
+00000560: 6e20 7265 733a 0d0a 2020 2020 2020 2020  n res:..        
+00000570: 2020 2020 2020 2020 2020 2020 7363 7265              scre
+00000580: 656e 5b22 706f 7322 5d20 3d20 7265 735b  en["pos"] = res[
+00000590: 2270 6f73 225d 0d0a 2020 2020 2020 2020  "pos"]..        
+000005a0: 2020 2020 2020 2020 6272 6561 6b0d 0a0d          break...
+000005b0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000005c0: 2e65 7870 6f72 745f 6469 7220 616e 6420  .export_dir and 
+000005d0: 7372 633a 0d0a 2020 2020 2020 2020 2020  src:..          
+000005e0: 2020 7372 6320 3d20 6f73 2e70 6174 682e    src = os.path.
+000005f0: 6a6f 696e 284c 4f47 4449 522c 2073 7263  join(LOGDIR, src
+00000600: 290d 0a20 2020 2020 2020 2073 6372 6565  )..        scree
+00000610: 6e5b 2273 7263 225d 203d 2073 7263 0d0a  n["src"] = src..
+00000620: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00000630: 2073 6372 6565 6e0d 0a20 2020 2065 6c73   screen..    els
+00000640: 653a 0d0a 2020 2020 2020 2020 6966 2073  e:..        if s
+00000650: 7465 705b 2264 6174 6122 5d5b 226e 616d  tep["data"]["nam
+00000660: 6522 5d20 696e 205b 2261 6972 7465 7374  e"] in ["airtest
+00000670: 5f74 6f75 6368 225d 3a0d 0a20 2020 2020  _touch"]:..     
+00000680: 2020 2020 2020 2023 20e5 b086 e59b bee5         # .......
+00000690: 838f e58c b9e9 858d e5be 97e5 88b0 e79a  ................
+000006a0: 8470 6f73 e4bf aee6 ada3 e4b8 bae6 9c80  .pos............
+000006b0: e7bb 8870 6f73 0d0a 2020 2020 2020 2020  ...pos..        
+000006c0: 2020 2020 6469 7370 6c61 795f 706f 7320      display_pos 
+000006d0: 3d20 4e6f 6e65 0d0a 2020 2020 2020 2020  = None..        
+000006e0: 2020 2020 6966 2073 656c 662e 6973 5f70      if self.is_p
+000006f0: 6f73 2873 7465 705b 2264 6174 6122 5d2e  os(step["data"].
+00000700: 6765 7428 2272 6574 2229 293a 0d0a 2020  get("ret")):..  
+00000710: 2020 2020 2020 2020 2020 2020 2020 6469                di
+00000720: 7370 6c61 795f 706f 7320 3d20 7374 6570  splay_pos = step
+00000730: 5b22 6461 7461 225d 5b22 7265 7422 5d0d  ["data"]["ret"].
+00000740: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+00000750: 6620 7365 6c66 2e69 735f 706f 7328 7374  f self.is_pos(st
+00000760: 6570 5b22 6461 7461 225d 5b22 6361 6c6c  ep["data"]["call
+00000770: 5f61 7267 7322 5d2e 6765 7428 2276 2229  _args"].get("v")
+00000780: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+00000790: 2020 2020 6469 7370 6c61 795f 706f 7320      display_pos 
+000007a0: 3d20 7374 6570 5b22 6461 7461 225d 5b22  = step["data"]["
+000007b0: 6361 6c6c 5f61 7267 7322 5d5b 2276 225d  call_args"]["v"]
+000007c0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+000007d0: 2064 6973 706c 6179 5f70 6f73 3a0d 0a20   display_pos:.. 
+000007e0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000007f0: 7261 6e73 5b22 706f 7322 5d20 3d20 5b64  rans["pos"] = [d
+00000800: 6973 706c 6179 5f70 6f73 5d0d 0a20 2020  isplay_pos]..   
+00000810: 2020 2020 2072 6574 7572 6e20 7472 616e       return tran
+00000820: 730d 0a0d 0a0d 0a64 6566 206e 6577 5f74  s......def new_t
+00000830: 7261 6e73 6c61 7465 5f64 6573 6328 7365  ranslate_desc(se
+00000840: 6c66 2c20 7374 6570 2c20 636f 6465 293a  lf, step, code):
+00000850: 0d0a 2020 2020 7472 616e 7320 3d20 6f6c  ..    trans = ol
+00000860: 645f 7472 616e 735f 6465 7363 2873 656c  d_trans_desc(sel
+00000870: 662c 2073 7465 702c 2063 6f64 6529 0d0a  f, step, code)..
+00000880: 2020 2020 6966 2022 6e61 6d65 2220 696e      if "name" in
+00000890: 2073 7465 705b 2764 6174 6127 5d20 616e   step['data'] an
+000008a0: 6420 2873 7465 705b 2764 6174 6127 5d5b  d (step['data'][
+000008b0: 226e 616d 6522 5d20 696e 2073 6372 6565  "name"] in scree
+000008c0: 6e5f 6675 6e63 206f 7220 7374 6570 5b22  n_func or step["
+000008d0: 6461 7461 225d 5b22 6e61 6d65 225d 2069  data"]["name"] i
+000008e0: 6e20 6f74 6865 725f 6675 6e63 293a 0d0a  n other_func):..
+000008f0: 2020 2020 2020 2020 6e61 6d65 203d 2073          name = s
+00000900: 7465 705b 2264 6174 6122 5d5b 226e 616d  tep["data"]["nam
+00000910: 6522 5d0d 0a20 2020 2020 2020 2061 7267  e"]..        arg
+00000920: 7320 3d20 7b7d 0d0a 2020 2020 2020 2020  s = {}..        
+00000930: 7572 6c20 3d20 2222 0d0a 2020 2020 2020  url = ""..      
+00000940: 2020 666f 7220 6974 656d 2069 6e20 636f    for item in co
+00000950: 6465 5b22 6172 6773 225d 3a0d 0a20 2020  de["args"]:..   
+00000960: 2020 2020 2020 2020 2069 6620 286e 616d           if (nam
+00000970: 653d 3d27 6765 7427 293a 0d0a 2020 2020  e=='get'):..    
+00000980: 2020 2020 2020 2020 2020 2020 7572 6c20              url 
+00000990: 3d20 756e 7175 6f74 6528 6974 656d 5b27  = unquote(item['
+000009a0: 7661 6c75 6527 5d29 0d0a 2020 2020 2020  value'])..      
+000009b0: 2020 2020 2020 2020 2020 6974 656d 5b27            item['
+000009c0: 7661 6c75 6527 5d20 3d20 223c 6120 6872  value'] = "<a hr
+000009d0: 6566 3d27 2573 2720 7461 7267 6574 3d27  ef='%s' target='
+000009e0: 5f62 6c61 6e6b 2720 7374 796c 653d 2763  _blank' style='c
+000009f0: 6f6c 6f72 3a63 6f72 6e66 6c6f 7765 7262  olor:cornflowerb
+00000a00: 6c75 6527 3e25 733c 2f61 3e22 2025 2028  lue'>%s</a>" % (
+00000a10: 7572 6c2c 2075 726c 290d 0a20 2020 2020  url, url)..     
+00000a20: 2020 2020 2020 2061 7267 735b 6974 656d         args[item
+00000a30: 5b27 6b65 7927 5d5d 203d 2069 7465 6d5b  ['key']] = item[
+00000a40: 2776 616c 7565 275d 0d0a 2020 2020 2020  'value']..      
+00000a50: 2020 6465 7363 203d 207b 0d0a 2020 2020    desc = {..    
+00000a60: 2020 2020 2020 2020 2266 696e 645f 656c          "find_el
+00000a70: 656d 656e 745f 6279 5f78 7061 7468 223a  ement_by_xpath":
+00000a80: 206c 616d 6264 613a 2075 2246 696e 6420   lambda: u"Find 
+00000a90: 656c 656d 656e 7420 6279 2078 7061 7468  element by xpath
+00000aa0: 3a20 2573 2220 2520 6172 6773 2e67 6574  : %s" % args.get
+00000ab0: 2822 7870 6174 6822 292c 0d0a 2020 2020  ("xpath"),..    
+00000ac0: 2020 2020 2020 2020 2266 696e 645f 656c          "find_el
+00000ad0: 656d 656e 745f 6279 5f69 6422 3a20 6c61  ement_by_id": la
+00000ae0: 6d62 6461 3a20 7522 4669 6e64 2065 6c65  mbda: u"Find ele
+00000af0: 6d65 6e74 2062 7920 6964 3a20 2573 2220  ment by id: %s" 
+00000b00: 2520 6172 6773 2e67 6574 2822 6964 2229  % args.get("id")
+00000b10: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+00000b20: 6669 6e64 5f65 6c65 6d65 6e74 5f62 795f  find_element_by_
+00000b30: 6e61 6d65 223a 206c 616d 6264 613a 2075  name": lambda: u
+00000b40: 2246 696e 6420 656c 656d 656e 7420 6279  "Find element by
+00000b50: 206e 616d 653a 2025 7322 2025 2061 7267   name: %s" % arg
+00000b60: 732e 6765 7428 226e 616d 6522 292c 0d0a  s.get("name"),..
+00000b70: 2020 2020 2020 2020 2020 2020 2261 7373              "ass
+00000b80: 6572 745f 6578 6973 7422 3a20 7522 4173  ert_exist": u"As
+00000b90: 7365 7274 2065 6c65 6d65 6e74 2065 7869  sert element exi
+00000ba0: 7374 732e 222c 0d0a 2020 2020 2020 2020  sts.",..        
+00000bb0: 2020 2020 2263 6c69 636b 223a 2075 2243      "click": u"C
+00000bc0: 6c69 636b 2074 6865 2065 6c65 6d65 6e74  lick the element
+00000bd0: 2074 6861 7420 6265 656e 2066 6f75 6e64   that been found
+00000be0: 2e22 2c0d 0a20 2020 2020 2020 2020 2020  .",..           
+00000bf0: 2022 7365 6e64 5f6b 6579 7322 3a20 7522   "send_keys": u"
+00000c00: 5365 6e64 2073 6f6d 6520 7465 7874 2061  Send some text a
+00000c10: 6e64 206b 6579 626f 6172 6420 6576 656e  nd keyboard even
+00000c20: 7420 746f 2074 6865 2065 6c65 6d65 6e74  t to the element
+00000c30: 2074 6861 7420 6265 656e 2066 6f75 6e64   that been found
+00000c40: 2e22 2c0d 0a20 2020 2020 2020 2020 2020  .",..           
+00000c50: 2022 6765 7422 3a20 6c61 6d62 6461 3a20   "get": lambda: 
+00000c60: 7522 4765 7420 7468 6520 7765 6220 6164  u"Get the web ad
+00000c70: 6472 6573 733a 2025 7322 2025 2028 7572  dress: %s" % (ur
+00000c80: 6c29 2c0d 0a20 2020 2020 2020 2020 2020  l),..           
+00000c90: 2022 7377 6974 6368 5f74 6f5f 6c61 7374   "switch_to_last
+00000ca0: 5f77 696e 646f 7722 3a20 7522 5377 6974  _window": u"Swit
+00000cb0: 6368 2074 6f20 7468 6520 6c61 7374 2074  ch to the last t
+00000cc0: 6162 2e22 2c0d 0a20 2020 2020 2020 2020  ab.",..         
+00000cd0: 2020 2022 7377 6974 6368 5f74 6f5f 6c61     "switch_to_la
+00000ce0: 7465 7374 5f77 696e 646f 7722 3a20 7522  test_window": u"
+00000cf0: 5377 6974 6368 2074 6f20 7468 6520 6e65  Switch to the ne
+00000d00: 7720 7461 622e 222c 0d0a 2020 2020 2020  w tab.",..      
+00000d10: 2020 2020 2020 2262 6163 6b22 3a20 7522        "back": u"
+00000d20: 4261 636b 2074 6f20 7468 6520 6c61 7374  Back to the last
+00000d30: 2070 6167 652e 222c 0d0a 2020 2020 2020   page.",..      
+00000d40: 2020 2020 2020 2266 6f72 7761 7264 223a        "forward":
+00000d50: 2075 2246 6f72 7761 7264 2074 6f20 7468   u"Forward to th
+00000d60: 6520 6e65 7874 2070 6167 652e 222c 0d0a  e next page.",..
+00000d70: 2020 2020 2020 2020 2020 2020 2273 6e61              "sna
+00000d80: 7073 686f 7422 3a20 6c61 6d62 6461 3a20  pshot": lambda: 
+00000d90: 2875 2253 6372 6565 6e73 686f 7420 6465  (u"Screenshot de
+00000da0: 7363 7269 7074 696f 6e3a 2025 7322 2025  scription: %s" %
+00000db0: 2061 7267 732e 6765 7428 226d 7367 2229   args.get("msg")
+00000dc0: 2920 6966 2061 7267 732e 6765 7428 226d  ) if args.get("m
+00000dd0: 7367 2229 2065 6c73 6520 7522 536e 6170  sg") else u"Snap
+00000de0: 7368 6f74 2063 7572 7265 6e74 2070 6167  shot current pag
+00000df0: 6522 2c0d 0a20 2020 2020 2020 207d 0d0a  e",..        }..
+00000e00: 0d0a 2020 2020 2020 2020 6465 7363 5f7a  ..        desc_z
+00000e10: 6820 3d20 7b0d 0a20 2020 2020 2020 2020  h = {..         
+00000e20: 2020 2022 6669 6e64 5f65 6c65 6d65 6e74     "find_element
+00000e30: 5f62 795f 7870 6174 6822 3a20 6c61 6d62  _by_xpath": lamb
+00000e40: 6461 3a20 7522 e5af bbe6 89be e68c 87e5  da: u"..........
+00000e50: ae9a e9a1 b5e9 9da2 e585 83e7 b4a0 3a20  ..............: 
+00000e60: 5c22 2573 5c22 2220 2520 6172 6773 2e67  \"%s\"" % args.g
+00000e70: 6574 2822 7870 6174 6822 292c 0d0a 2020  et("xpath"),..  
+00000e80: 2020 2020 2020 2020 2020 2266 696e 645f            "find_
+00000e90: 656c 656d 656e 745f 6279 5f69 6422 3a20  element_by_id": 
+00000ea0: 6c61 6d62 6461 3a20 7522 e5af bbe6 89be  lambda: u"......
+00000eb0: e68c 87e5 ae9a e9a1 b5e9 9da2 e585 83e7  ................
+00000ec0: b4a0 3a20 5c22 2573 5c22 2220 2520 6172  ..: \"%s\"" % ar
+00000ed0: 6773 2e67 6574 2822 6964 2229 2c0d 0a20  gs.get("id"),.. 
+00000ee0: 2020 2020 2020 2020 2020 2022 6669 6e64             "find
+00000ef0: 5f65 6c65 6d65 6e74 5f62 795f 6e61 6d65  _element_by_name
+00000f00: 223a 206c 616d 6264 613a 2075 22e5 afbb  ": lambda: u"...
+00000f10: e689 bee6 8c87 e5ae 9ae9 a1b5 e99d a2e5  ................
+00000f20: 8583 e7b4 a03a 205c 2225 735c 2222 2025  .....: \"%s\"" %
+00000f30: 2061 7267 732e 6765 7428 226e 616d 6522   args.get("name"
+00000f40: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+00000f50: 2261 7373 6572 745f 6578 6973 7422 3a20  "assert_exist": 
+00000f60: 7522 e696 ade8 a880 e9a1 b5e9 9da2 e585  u"..............
+00000f70: 83e7 b4a0 e5ad 98e5 9ca8 2e22 2c0d 0a20  ...........",.. 
+00000f80: 2020 2020 2020 2020 2020 2022 636c 6963             "clic
+00000f90: 6b22 3a20 7522 e782 b9e5 87bb e689 bee5  k": u"..........
+00000fa0: 88b0 e79a 84e9 a1b5 e99d a2e5 8583 e7b4  ................
+00000fb0: a02e 222c 0d0a 2020 2020 2020 2020 2020  ..",..          
+00000fc0: 2020 2273 656e 645f 6b65 7973 223a 2075    "send_keys": u
+00000fd0: 22e4 bca0 e980 81e6 9687 e69c ac5c 2225  "............\"%
+00000fe0: 735c 22e5 88b0 e980 89e4 b8ad e696 87e6  s\".............
+00000ff0: 9cac e6a1 862e 2220 2520 2861 7267 732e  ......" % (args.
+00001000: 6765 7428 2274 6578 7422 2c20 2222 2929  get("text", ""))
+00001010: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+00001020: 6765 7422 3a20 6c61 6d62 6461 3a20 7522  get": lambda: u"
+00001030: e8ae bfe9 97ae e7bd 91e7 bb9c e59c b0e5  ................
+00001040: 9d80 3a20 2573 2220 2520 2875 726c 292c  ..: %s" % (url),
+00001050: 0d0a 2020 2020 2020 2020 2020 2020 2273  ..            "s
+00001060: 7769 7463 685f 746f 5f6c 6173 745f 7769  witch_to_last_wi
+00001070: 6e64 6f77 223a 2075 22e5 8887 e68d a2e5  ndow": u".......
+00001080: 88b0 e4b8 8ae4 b880 e4b8 aae6 a087 e7ad  ................
+00001090: bee9 a1b5 2e22 2c0d 0a20 2020 2020 2020  .....",..       
+000010a0: 2020 2020 2022 7377 6974 6368 5f74 6f5f       "switch_to_
+000010b0: 6c61 7465 7374 5f77 696e 646f 7722 3a20  latest_window": 
+000010c0: 7522 e588 87e6 8da2 e588 b0e6 9c80 e696  u"..............
+000010d0: b0e6 a087 e7ad bee9 a1b5 2e22 2c0d 0a20  ...........",.. 
+000010e0: 2020 2020 2020 2020 2020 2022 6261 636b             "back
+000010f0: 223a 2075 22e5 908e e980 80e5 88b0 e4b8  ": u"...........
+00001100: 8ae4 b880 e4b8 aae9 a1b5 e99d a22e 222c  ..............",
+00001110: 0d0a 2020 2020 2020 2020 2020 2020 2266  ..            "f
+00001120: 6f72 7761 7264 223a 2075 22e5 898d e8bf  orward": u".....
+00001130: 9be5 88b0 e4b8 8be4 b880 e4b8 aae9 a1b5  ................
+00001140: e99d a22e 222c 0d0a 2020 2020 2020 2020  ....",..        
+00001150: 2020 2020 2273 6e61 7073 686f 7422 3a20      "snapshot": 
+00001160: 6c61 6d62 6461 3a20 2875 22e6 88aa e59b  lambda: (u".....
+00001170: bee6 8f8f e8bf b03a 2025 7322 2025 2061  .......: %s" % a
+00001180: 7267 732e 6765 7428 226d 7367 2229 2920  rgs.get("msg")) 
+00001190: 6966 2061 7267 732e 6765 7428 226d 7367  if args.get("msg
+000011a0: 2229 2065 6c73 6520 7522 e688 aae5 8f96  ") else u"......
+000011b0: e5bd 93e5 898d e9a1 b5e9 9da2 220d 0a20  ............".. 
+000011c0: 2020 2020 2020 207d 0d0a 0d0a 2020 2020         }....    
+000011d0: 2020 2020 6966 2073 656c 662e 6c61 6e67      if self.lang
+000011e0: 203d 3d20 277a 6827 3a0d 0a20 2020 2020   == 'zh':..     
+000011f0: 2020 2020 2020 2064 6573 6320 3d20 6465         desc = de
+00001200: 7363 5f7a 680d 0a20 2020 2020 2020 2072  sc_zh..        r
+00001210: 6574 203d 2064 6573 632e 6765 7428 6e61  et = desc.get(na
+00001220: 6d65 290d 0a20 2020 2020 2020 2069 6620  me)..        if 
+00001230: 6361 6c6c 6162 6c65 2872 6574 293a 0d0a  callable(ret):..
+00001240: 2020 2020 2020 2020 2020 2020 7265 7420              ret 
+00001250: 3d20 7265 7428 290d 0a20 2020 2020 2020  = ret()..       
+00001260: 2072 6574 7572 6e20 7265 740d 0a20 2020   return ret..   
+00001270: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00001280: 7265 7475 726e 2074 7261 6e73 0d0a 0d0a  return trans....
+00001290: 0d0a 6465 6620 6e65 775f 7472 616e 736c  ..def new_transl
+000012a0: 6174 655f 636f 6465 2873 656c 662c 2073  ate_code(self, s
+000012b0: 7465 7029 3a0d 0a20 2020 2074 7261 6e73  tep):..    trans
+000012c0: 203d 206f 6c64 5f74 7261 6e73 5f63 6f64   = old_trans_cod
+000012d0: 6528 7365 6c66 2c20 7374 6570 290d 0a20  e(self, step).. 
+000012e0: 2020 2069 6620 7472 616e 733a 0d0a 2020     if trans:..  
+000012f0: 2020 2020 2020 666f 7220 6964 782c 2069        for idx, i
+00001300: 7465 6d20 696e 2065 6e75 6d65 7261 7465  tem in enumerate
+00001310: 2874 7261 6e73 5b22 6172 6773 225d 293a  (trans["args"]):
+00001320: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00001330: 2069 7465 6d5b 226b 6579 225d 203d 3d20   item["key"] == 
+00001340: 2273 656c 6622 3a0d 0a20 2020 2020 2020  "self":..       
+00001350: 2020 2020 2020 2020 2074 7261 6e73 5b22           trans["
+00001360: 6172 6773 225d 2e70 6f70 2869 6478 290d  args"].pop(idx).
+00001370: 0a20 2020 2072 6574 7572 6e20 7472 616e  .    return tran
+00001380: 730d 0a0d 0a0d 0a72 6570 6f72 742e 4c6f  s......report.Lo
+00001390: 6754 6f48 746d 6c2e 5f74 7261 6e73 6c61  gToHtml._transla
+000013a0: 7465 5f73 6372 6565 6e20 3d20 6e65 775f  te_screen = new_
+000013b0: 7472 616e 735f 7363 7265 656e 0d0a 7265  trans_screen..re
+000013c0: 706f 7274 2e4c 6f67 546f 4874 6d6c 2e5f  port.LogToHtml._
+000013d0: 7472 616e 736c 6174 655f 6465 7363 203d  translate_desc =
+000013e0: 206e 6577 5f74 7261 6e73 6c61 7465 5f64   new_translate_d
+000013f0: 6573 630d 0a72 6570 6f72 742e 4c6f 6754  esc..report.LogT
+00001400: 6f48 746d 6c2e 5f74 7261 6e73 6c61 7465  oHtml._translate
+00001410: 5f63 6f64 6520 3d20 6e65 775f 7472 616e  _code = new_tran
+00001420: 736c 6174 655f 636f 6465 0d0a 0d0a       slate_code....
```

### Comparing `airtest-selenium-1.0.3/airtest_selenium/utils/airtest_api.py` & `airtest-selenium-1.0.4/airtest_selenium/utils/airtest_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     """
     if not ST.LOG_DIR:
         return
     if screen is None:
         screen = G.DEVICE.snapshot()
     filename = "%(time)d.jpg" % {'time': time.time() * 1000}
     filepath = os.path.join(ST.LOG_DIR, filename)
-    aircv.imwrite(filepath, screen)
-    return filename
+    aircv.imwrite(filepath, screen, ST.SNAPSHOT_QUALITY)
+    return {"screen": filename, "resolution": aircv.get_resolution(screen)}
 
 if __name__ == "__main__":
     from airtest.core.api import connect_device
     from airtest.core.error import AdbError, InstallMultipleError
     dev = connect_device("android://10.252.60.147:5039/AAQKYTY9MVRGOFIV")
     dev.install_multiple_app("E://windows//Test.apk")
```

### Comparing `airtest-selenium-1.0.3/airtest_selenium/utils/six.py` & `airtest-selenium-1.0.4/airtest_selenium/utils/six.py`

 * *Files identical despite different names*

### Comparing `airtest-selenium-1.0.3/LICENSE` & `airtest-selenium-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `airtest-selenium-1.0.3/README.md` & `airtest-selenium-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `airtest-selenium-1.0.3/setup.py` & `airtest-selenium-1.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,20 +6,20 @@
     """ load requirements from a pip requirements file. (replacing from pip.req import parse_requirements)"""
     lineiter = (line.strip() for line in open(filename))
     return [line for line in lineiter if line and not line.startswith("#")]
 
 
 setup(
     name='airtest-selenium',
-    version='1.0.3',
+    version='1.0.4',
     keywords="selenium, automation test, web ui automation",
     description='Selenium with airtest test framework.',
     long_description='Selenium with airtest test framework. 2018 present by NetEase Games',
     packages=find_packages(),
     include_package_data=True,
     install_requires=parse_requirements(),
     license='Apache License 2.0',
 
     author='Netease Games',
-    author_email='zxfn4514@corp.netease.com, gzliuxin@corp.netease.com',
+    author_email='rockywhisper@163.com',
     url='https://github.com/AirtestProject/airtest-selenium',
 )
```

