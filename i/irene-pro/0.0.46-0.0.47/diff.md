# Comparing `tmp/irene_pro-0.0.46.tar.gz` & `tmp/irene_pro-0.0.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irene_pro-0.0.46.tar", last modified: Thu May 25 14:10:27 2023, max compression
+gzip compressed data, was "irene_pro-0.0.47.tar", last modified: Tue May 30 10:48:16 2023, max compression
```

## Comparing `irene_pro-0.0.46.tar` & `irene_pro-0.0.47.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 14:10:27.415086 irene_pro-0.0.46/
--rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.46/LICENSE
--rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.46/MANIFEST.in
--rw-rw-rw-   0        0        0     1740 2023-05-25 14:10:27.412094 irene_pro-0.0.46/PKG-INFO
--rw-rw-rw-   0        0        0     1165 2023-05-25 07:51:23.000000 irene_pro-0.0.46/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 14:10:27.332827 irene_pro-0.0.46/irene_pro/
--rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.46/irene_pro/__init__.py
--rw-rw-rw-   0        0        0     4001 2023-05-24 10:17:54.000000 irene_pro-0.0.46/irene_pro/logic.py
--rw-rw-rw-   0        0        0    31914 2023-05-25 14:09:46.000000 irene_pro-0.0.46/irene_pro/widgets.py
-drwxrwxrwx   0        0        0        0 2023-05-25 14:10:27.406111 irene_pro-0.0.46/irene_pro.egg-info/
--rw-rw-rw-   0        0        0     1740 2023-05-25 14:10:27.000000 irene_pro-0.0.46/irene_pro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-05-25 14:10:27.000000 irene_pro-0.0.46/irene_pro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 14:10:27.000000 irene_pro-0.0.46/irene_pro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-25 14:10:27.000000 irene_pro-0.0.46/irene_pro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-25 14:10:27.000000 irene_pro-0.0.46/irene_pro.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 14:10:27.416085 irene_pro-0.0.46/setup.cfg
--rw-rw-rw-   0        0        0     1164 2023-05-25 14:09:56.000000 irene_pro-0.0.46/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 10:48:16.336006 irene_pro-0.0.47/
+-rw-rw-rw-   0        0        0      227 2023-05-04 09:47:29.000000 irene_pro-0.0.47/LICENSE
+-rw-rw-rw-   0        0        0       14 2023-05-08 07:12:29.000000 irene_pro-0.0.47/MANIFEST.in
+-rw-rw-rw-   0        0        0     1740 2023-05-30 10:48:16.327030 irene_pro-0.0.47/PKG-INFO
+-rw-rw-rw-   0        0        0     1165 2023-05-25 07:51:23.000000 irene_pro-0.0.47/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 10:48:16.294118 irene_pro-0.0.47/irene_pro/
+-rw-rw-rw-   0        0        0        0 2023-05-04 13:31:01.000000 irene_pro-0.0.47/irene_pro/__init__.py
+-rw-rw-rw-   0        0        0     4980 2023-05-30 10:44:24.000000 irene_pro-0.0.47/irene_pro/logic.py
+-rw-rw-rw-   0        0        0    32045 2023-05-26 07:13:56.000000 irene_pro-0.0.47/irene_pro/widgets.py
+drwxrwxrwx   0        0        0        0 2023-05-30 10:48:16.324038 irene_pro-0.0.47/irene_pro.egg-info/
+-rw-rw-rw-   0        0        0     1740 2023-05-30 10:48:16.000000 irene_pro-0.0.47/irene_pro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-05-30 10:48:16.000000 irene_pro-0.0.47/irene_pro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 10:48:16.000000 irene_pro-0.0.47/irene_pro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-30 10:48:16.000000 irene_pro-0.0.47/irene_pro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-30 10:48:16.000000 irene_pro-0.0.47/irene_pro.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 10:48:16.337004 irene_pro-0.0.47/setup.cfg
+-rw-rw-rw-   0        0        0     1164 2023-05-30 10:46:49.000000 irene_pro-0.0.47/setup.py
```

### Comparing `irene_pro-0.0.46/PKG-INFO` & `irene_pro-0.0.47/irene_pro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: irene_pro
-Version: 0.0.46
+Name: irene-pro
+Version: 0.0.47
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.46/README.md` & `irene_pro-0.0.47/README.md`

 * *Files identical despite different names*

### Comparing `irene_pro-0.0.46/irene_pro/logic.py` & `irene_pro-0.0.47/irene_pro/logic.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,34 @@
 import pyperclip as copier
 import sqlite3
+from datetime import datetime
+from time import strftime
+
+class DateTime:
+    def __init__(self, week = datetime.today().isocalendar()[1], day = strftime("%Y-%m-%d"), 
+                 month = strftime("%Y-%m"), year = strftime("%Y"), current_weeks = None, combined = int(strftime("%Y%m%d%H%M")),
+                   combined_date = None) -> None:
+        self.week = week
+        self.day = day
+        self.month = month
+        self.year = year
+        self.current_weeks = current_weeks
+        self.current_weeks = str(week) + str(year)
+        self.combined = combined
+        self.combined_date = combined_date
+
+    def datedelta(self, start, end):
+        date1 = datetime.strptime(start, "%Y-%m-%d %H:%M:%S")
+        date2 = datetime.strptime(end, "%Y-%m-%d %H:%M:%S")
+        delta = date2 - date1
+        return delta
+    @property
+    def combinedDate(self):
+        return [self.year, self.month, self.current_weeks, self.day, self.combined]
+
 def separate(numbers):
     floating = []
     new_str = ""
     float_pos = 0
     decision = ""
     sign_negative = ""
     str_num = str(numbers)
```

### Comparing `irene_pro-0.0.46/irene_pro/widgets.py` & `irene_pro-0.0.47/irene_pro/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -749,15 +749,16 @@
         status.pack(side = TOP, padx = w(1), pady = h(0), fill=X, expand = True, anchor = NW)
 
         # to get the data analysis of single clicked employee or else member
         details = btn(fr, text = btn_labels['4'], activebackground = fr.cget('bg'), bg = "#ffaa00")
         details.bind("<Button-1>", lambda e: fr.destroy(), add = "+")
         details.pack(side = TOP, padx = w(1), pady = h(0), fill=X, expand = True, anchor = NW)
 
-        # self.parent.bind("<Button-1>", lambda e: fr.destroy(), add = "+")
+        close_btn = btn(fr, text = "close",activebackground = fr.cget('bg'), command = lambda: fr.destroy())
+        close_btn.pack(side = TOP, padx = w(1), pady = h(0), fill=X, expand = True, anchor = NW)
 
         return delete_btn, edit_btn, status, details
 
 # CONSTANTS
 comb_syle = 'comb.TCombobox'
 check_style = "TCheckbutton"
 radio_style = "Custom.TRadiobutton"
```

### Comparing `irene_pro-0.0.46/irene_pro.egg-info/PKG-INFO` & `irene_pro-0.0.47/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: irene-pro
-Version: 0.0.46
+Name: irene_pro
+Version: 0.0.47
 Summary: Use customized GUI
 Author: Irene coldsober
 Author-email: <irene.study.2023@gmail.com>
 Keywords: tkinter,widget,gui
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `irene_pro-0.0.46/setup.py` & `irene_pro-0.0.47/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 00000090: 286f 732e 7061 7468 2e6a 6f69 6e28 6865  (os.path.join(he
 000000a0: 7265 2c20 2252 4541 444d 452e 6d64 2229  re, "README.md")
 000000b0: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
 000000c0: 3822 2920 6173 2066 683a 0d0a 2020 2020  8") as fh:..    
 000000d0: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 000000e0: 203d 2022 5c6e 2220 2b20 6668 2e72 6561   = "\n" + fh.rea
 000000f0: 6428 290d 0a0d 0a56 4552 5349 4f4e 203d  d()....VERSION =
-00000100: 2027 302e 302e 3436 270d 0a44 4553 4352   '0.0.46'..DESCR
+00000100: 2027 302e 302e 3437 270d 0a44 4553 4352   '0.0.47'..DESCR
 00000110: 4950 5449 4f4e 203d 2027 5573 6520 6375  IPTION = 'Use cu
 00000120: 7374 6f6d 697a 6564 2047 5549 270d 0a4c  stomized GUI'..L
 00000130: 4f4e 475f 4445 5343 5249 5054 494f 4e20  ONG_DESCRIPTION 
 00000140: 3d20 2741 2070 6163 6b61 6765 2074 6861  = 'A package tha
 00000150: 7420 616c 6c6f 7773 2079 6f75 2074 6f20  t allows you to 
 00000160: 7573 6520 7374 796c 6573 2061 6e64 2077  use styles and w
 00000170: 6964 6765 7420 6f66 2073 7570 6572 206c  idget of super l
```

